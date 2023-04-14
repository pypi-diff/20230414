# Comparing `tmp/xcffib-v0.1.3.tar.gz` & `tmp/xcffib-v0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xcffib-v0.1.3.tar", last modified: Sat Aug  2 02:56:27 2014, max compression
+gzip compressed data, was "dist/xcffib-v0.1.4.tar", last modified: Thu Aug 14 17:43:42 2014, max compression
```

## Comparing `xcffib-v0.1.3.tar` & `xcffib-v0.1.4.tar`

### file list

```diff
@@ -1,47 +1,46 @@
-drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2014-08-02 02:56:27.000000 xcffib-v0.1.3/
--rw-rw-r--   0 tycho     (1000) tycho     (1000)       59 2014-08-02 02:56:27.000000 xcffib-v0.1.3/setup.cfg
-drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2014-08-02 02:56:27.000000 xcffib-v0.1.3/xcffib.egg-info/
--rw-rw-r--   0 tycho     (1000) tycho     (1000)        1 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib.egg-info/not-zip-safe
--rw-rw-r--   0 tycho     (1000) tycho     (1000)        7 2014-08-02 02:56:27.000000 xcffib-v0.1.3/xcffib.egg-info/top_level.txt
--rw-rw-r--   0 tycho     (1000) tycho     (1000)      780 2014-08-02 02:56:27.000000 xcffib-v0.1.3/xcffib.egg-info/SOURCES.txt
--rw-rw-r--   0 tycho     (1000) tycho     (1000)       15 2014-08-02 02:56:27.000000 xcffib-v0.1.3/xcffib.egg-info/requires.txt
--rw-rw-r--   0 tycho     (1000) tycho     (1000)        1 2014-08-02 02:56:27.000000 xcffib-v0.1.3/xcffib.egg-info/dependency_links.txt
--rw-rw-r--   0 tycho     (1000) tycho     (1000)      298 2014-08-02 02:56:27.000000 xcffib-v0.1.3/xcffib.egg-info/PKG-INFO
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1255 2014-08-02 02:56:26.000000 xcffib-v0.1.3/setup.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)      298 2014-08-02 02:56:27.000000 xcffib-v0.1.3/PKG-INFO
-drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2014-08-02 02:56:27.000000 xcffib-v0.1.3/xcffib/
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     7415 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/record.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    15927 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/xv.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    21317 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/render.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     7657 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/res.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    31593 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/randr.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     7454 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/xf86dri.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    96363 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/xproto.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1993 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/xc_misc.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     3309 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/xevie.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     5368 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/shape.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)      745 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/bigreq.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     3331 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/screensaver.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)   102014 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/xinput.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     8466 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/ffi.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     3123 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/dri3.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)      882 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/ge.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2558 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/damage.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     5680 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/xvmc.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    11792 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/sync.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     4534 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/shm.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1102 2014-07-05 23:26:37.000000 xcffib-v0.1.3/xcffib/xcb.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    62470 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/glx.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     7058 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/present.py
-drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2014-08-02 02:56:27.000000 xcffib-v0.1.3/xcffib/__pycache__/
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    58453 2014-08-02 02:56:27.000000 xcffib-v0.1.3/xcffib/__pycache__/_cffi__xe30fa035xc8917695.c
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     1938 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/xtest.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     3058 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/composite.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     2811 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/testing.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    12782 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/xf86vidmode.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    17303 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/__init__.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    13288 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/xselinux.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     3325 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/dpms.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)     4062 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/xinerama.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    12360 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/xfixes.py
--rw-rw-r--   0 tycho     (1000) tycho     (1000)    10587 2014-08-02 02:56:26.000000 xcffib-v0.1.3/xcffib/dri2.py
+drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2014-08-14 17:43:42.000000 xcffib-v0.1.4/
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     1255 2014-08-14 17:43:41.000000 xcffib-v0.1.4/setup.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)       59 2014-08-14 17:43:42.000000 xcffib-v0.1.4/setup.cfg
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)      298 2014-08-14 17:43:42.000000 xcffib-v0.1.4/PKG-INFO
+drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2014-08-14 17:43:42.000000 xcffib-v0.1.4/xcffib/
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     3290 2014-08-14 17:43:08.000000 xcffib-v0.1.4/xcffib/composite.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     4064 2014-08-14 17:43:17.000000 xcffib-v0.1.4/xcffib/screensaver.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     3731 2014-08-14 17:43:09.000000 xcffib-v0.1.4/xcffib/dpms.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)      753 2014-08-14 17:43:07.000000 xcffib-v0.1.4/xcffib/bigreq.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    14358 2014-08-14 17:43:27.000000 xcffib-v0.1.4/xcffib/xselinux.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     1050 2014-08-14 17:43:10.000000 xcffib-v0.1.4/xcffib/ge.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     8795 2014-08-14 17:43:12.000000 xcffib-v0.1.4/xcffib/present.py
+drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2014-08-14 17:43:42.000000 xcffib-v0.1.4/xcffib/__pycache__/
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    58453 2014-08-14 17:43:42.000000 xcffib-v0.1.4/xcffib/__pycache__/_cffi__xe30fa035xc8917695.c
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2305 2014-08-14 17:43:25.000000 xcffib-v0.1.4/xcffib/xtest.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    25501 2014-08-14 17:43:17.000000 xcffib-v0.1.4/xcffib/render.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     8121 2014-08-14 17:43:13.000000 xcffib-v0.1.4/xcffib/record.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     8369 2014-08-14 17:43:09.000000 xcffib-v0.1.4/xcffib/ffi.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    12892 2014-08-14 17:43:20.000000 xcffib-v0.1.4/xcffib/sync.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2814 2014-08-14 17:43:19.000000 xcffib-v0.1.4/xcffib/testing.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     8171 2014-08-14 17:43:22.000000 xcffib-v0.1.4/xcffib/xf86dri.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)   113599 2014-08-14 17:43:41.000000 xcffib-v0.1.4/xcffib/xproto.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     3729 2014-08-14 17:43:09.000000 xcffib-v0.1.4/xcffib/dri3.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    16211 2014-08-14 17:43:24.000000 xcffib-v0.1.4/xcffib/xf86vidmode.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    12087 2014-08-14 17:43:10.000000 xcffib-v0.1.4/xcffib/dri2.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)   122832 2014-08-14 17:43:41.000000 xcffib-v0.1.4/xcffib/xinput.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2284 2014-08-14 17:43:20.000000 xcffib-v0.1.4/xcffib/xc_misc.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     8134 2014-08-14 17:43:15.000000 xcffib-v0.1.4/xcffib/res.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    72652 2014-08-14 17:43:23.000000 xcffib-v0.1.4/xcffib/glx.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     3569 2014-08-14 17:43:21.000000 xcffib-v0.1.4/xcffib/xevie.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     6650 2014-08-14 17:43:30.000000 xcffib-v0.1.4/xcffib/xvmc.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     6700 2014-08-14 17:43:18.000000 xcffib-v0.1.4/xcffib/shape.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    14235 2014-08-14 17:43:24.000000 xcffib-v0.1.4/xcffib/xfixes.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     2843 2014-08-14 17:43:08.000000 xcffib-v0.1.4/xcffib/damage.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    37369 2014-08-14 17:43:17.000000 xcffib-v0.1.4/xcffib/randr.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    20175 2014-08-14 17:43:30.000000 xcffib-v0.1.4/xcffib/xv.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     5925 2014-08-14 17:43:19.000000 xcffib-v0.1.4/xcffib/shm.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)    18859 2014-08-14 17:43:09.000000 xcffib-v0.1.4/xcffib/__init__.py
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)     4420 2014-08-14 17:43:23.000000 xcffib-v0.1.4/xcffib/xinerama.py
+drwxrwxr-x   0 tycho     (1000) tycho     (1000)        0 2014-08-14 17:43:42.000000 xcffib-v0.1.4/xcffib.egg-info/
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)        1 2014-08-14 17:43:42.000000 xcffib-v0.1.4/xcffib.egg-info/not-zip-safe
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)       15 2014-08-14 17:43:42.000000 xcffib-v0.1.4/xcffib.egg-info/requires.txt
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)      298 2014-08-14 17:43:42.000000 xcffib-v0.1.4/xcffib.egg-info/PKG-INFO
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)        7 2014-08-14 17:43:42.000000 xcffib-v0.1.4/xcffib.egg-info/top_level.txt
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)      766 2014-08-14 17:43:42.000000 xcffib-v0.1.4/xcffib.egg-info/SOURCES.txt
+-rw-rw-r--   0 tycho     (1000) tycho     (1000)        1 2014-08-14 17:43:42.000000 xcffib-v0.1.4/xcffib.egg-info/dependency_links.txt
```

### Comparing `xcffib-v0.1.3/xcffib.egg-info/SOURCES.txt` & `xcffib-v0.1.4/xcffib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 xcffib/res.py
 xcffib/screensaver.py
 xcffib/shape.py
 xcffib/shm.py
 xcffib/sync.py
 xcffib/testing.py
 xcffib/xc_misc.py
-xcffib/xcb.py
 xcffib/xevie.py
 xcffib/xf86dri.py
 xcffib/xf86vidmode.py
 xcffib/xfixes.py
 xcffib/xinerama.py
 xcffib/xinput.py
 xcffib/xproto.py
```

### Comparing `xcffib-v0.1.3/setup.py` & `xcffib-v0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     setup_requires hasn't run yet.
     """
     def finalize_options(self):
         import xcffib
         self.distribution.ext_modules = [xcffib.ffi.verifier.get_extension()]
         build.finalize_options(self)
 
-version = "v0.1.3"
+version = "v0.1.4"
 dependencies = ['six', 'cffi>=0.8.2']
 
 setup(
     name="xcffib",
     version=version,
     description="A drop in replacement for xpyb, an XCB python binding",
     keywords="xcb xpyb cffi x11 x windows",
```

### Comparing `xcffib-v0.1.3/xcffib/record.py` & `xcffib-v0.1.4/xcffib/record.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,50 +2,65 @@
 import struct
 import six
 MAJOR_VERSION = 1
 MINOR_VERSION = 13
 key = xcffib.ExtensionKey("RECORD")
 _events = {}
 _errors = {}
+
+
 class Range8(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.first, self.last = unpacker.unpack("BB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=BB", self.first, self.last))
         return buf.getvalue()
     fixed_size = 2
+
+
 class Range16(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.first, self.last = unpacker.unpack("HH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=HH", self.first, self.last))
         return buf.getvalue()
     fixed_size = 4
+
+
 class ExtRange(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.major = Range8(unpacker)
         unpacker.pad(Range16)
         self.minor = Range16(unpacker)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(self.major.pack())
         buf.write(self.minor.pack())
         return buf.getvalue()
+
+
 class Range(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.core_requests = Range8(unpacker)
         unpacker.pad(Range8)
         self.core_replies = Range8(unpacker)
         unpacker.pad(ExtRange)
@@ -56,115 +71,203 @@
         self.delivered_events = Range8(unpacker)
         unpacker.pad(Range8)
         self.device_events = Range8(unpacker)
         unpacker.pad(Range8)
         self.errors = Range8(unpacker)
         self.client_started, self.client_died = unpacker.unpack("BB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=BB", self.client_started, self.client_died))
         buf.write(self.core_requests.pack())
         buf.write(self.core_replies.pack())
         buf.write(self.ext_requests.pack())
         buf.write(self.ext_replies.pack())
         buf.write(self.delivered_events.pack())
         buf.write(self.device_events.pack())
         buf.write(self.errors.pack())
         return buf.getvalue()
+
+
 class HType:
     FromServerTime = 1 << 0
     FromClientTime = 1 << 1
     FromClientSequence = 1 << 2
+
+
 class CS:
     CurrentClients = 1
     FutureClients = 2
     AllClients = 3
+
+
 class ClientInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.client_resource, self.num_ranges = unpacker.unpack("II")
         self.ranges = xcffib.List(unpacker, Range, self.num_ranges)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=II", self.client_resource, self.num_ranges))
         buf.write(xcffib.pack_list(self.ranges, Range))
         return buf.getvalue()
+
+
 class BadContextError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
         self.invalid_record, = unpacker.unpack("xx2xI")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=I", self.invalid_record))
         return buf.getvalue()
 BadBadContext = BadContextError
 _errors[0] = BadContextError
+
+
 class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.major_version, self.minor_version = unpacker.unpack("xx2x4xHH")
         self.bufsize = unpacker.offset - base
+
+
 class QueryVersionCookie(xcffib.Cookie):
     reply_type = QueryVersionReply
+
+
 class GetContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.enabled, self.element_header, self.num_intercepted_clients = unpacker.unpack("xB2x4xB3xI16x")
-        self.intercepted_clients = xcffib.List(unpacker, ClientInfo, self.num_intercepted_clients)
+        self.enabled, self.element_header, self.num_intercepted_clients = unpacker.unpack(
+            "xB2x4xB3xI16x")
+        self.intercepted_clients = xcffib.List(
+            unpacker,
+            ClientInfo,
+            self.num_intercepted_clients)
         self.bufsize = unpacker.offset - base
+
+
 class GetContextCookie(xcffib.Cookie):
     reply_type = GetContextReply
+
+
 class EnableContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.category, self.element_header, self.client_swapped, self.xid_base, self.server_time, self.rec_sequence_num = unpacker.unpack("xB2x4xBB2xIII8x")
+        self.category, self.element_header, self.client_swapped, self.xid_base, self.server_time, self.rec_sequence_num = unpacker.unpack(
+            "xB2x4xBB2xIII8x")
         self.data = xcffib.List(unpacker, "B", self.length * 4)
         self.bufsize = unpacker.offset - base
+
+
 class EnableContextCookie(xcffib.Cookie):
     reply_type = EnableContextReply
+
+
 class recordExtension(xcffib.Extension):
+
     def QueryVersion(self, major_version, minor_version, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xHH", major_version, minor_version))
-        return self.send_request(0, buf, QueryVersionCookie, is_checked=is_checked)
-    def CreateContext(self, context, element_header, num_client_specs, num_ranges, client_specs, ranges, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIB3xII", context, element_header, num_client_specs, num_ranges))
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
+    def CreateContext(
+            self,
+            context,
+            element_header,
+            num_client_specs,
+            num_ranges,
+            client_specs,
+            ranges,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIB3xII",
+                context,
+                element_header,
+                num_client_specs,
+                num_ranges))
         buf.write(xcffib.pack_list(client_specs, "I"))
         buf.write(xcffib.pack_list(ranges, Range))
         return self.send_request(1, buf, is_checked=is_checked)
-    def RegisterClients(self, context, element_header, num_client_specs, num_ranges, client_specs, ranges, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIB3xII", context, element_header, num_client_specs, num_ranges))
+
+    def RegisterClients(
+            self,
+            context,
+            element_header,
+            num_client_specs,
+            num_ranges,
+            client_specs,
+            ranges,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIB3xII",
+                context,
+                element_header,
+                num_client_specs,
+                num_ranges))
         buf.write(xcffib.pack_list(client_specs, "I"))
         buf.write(xcffib.pack_list(ranges, Range))
         return self.send_request(2, buf, is_checked=is_checked)
-    def UnregisterClients(self, context, num_client_specs, client_specs, is_checked=False):
+
+    def UnregisterClients(
+            self,
+            context,
+            num_client_specs,
+            client_specs,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", context, num_client_specs))
         buf.write(xcffib.pack_list(client_specs, "I"))
         return self.send_request(3, buf, is_checked=is_checked)
+
     def GetContext(self, context, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context))
-        return self.send_request(4, buf, GetContextCookie, is_checked=is_checked)
+        return self.send_request(
+            4,
+            buf,
+            GetContextCookie,
+            is_checked=is_checked)
+
     def EnableContext(self, context, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context))
-        return self.send_request(5, buf, EnableContextCookie, is_checked=is_checked)
+        return self.send_request(
+            5,
+            buf,
+            EnableContextCookie,
+            is_checked=is_checked)
+
     def DisableContext(self, context, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context))
         return self.send_request(6, buf, is_checked=is_checked)
+
     def FreeContext(self, context, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context))
         return self.send_request(7, buf, is_checked=is_checked)
 xcffib._add_ext(key, recordExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/xv.py` & `xcffib-v0.1.4/xcffib/dri2.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,325 +1,423 @@
 import xcffib
 import struct
 import six
-MAJOR_VERSION = 2
-MINOR_VERSION = 2
-key = xcffib.ExtensionKey("XVideo")
+MAJOR_VERSION = 1
+MINOR_VERSION = 4
+key = xcffib.ExtensionKey("DRI2")
 _events = {}
 _errors = {}
 from . import xproto
-from . import shm
-class Type:
-    InputMask = 1 << 0
-    OutputMask = 1 << 1
-    VideoMask = 1 << 2
-    StillMask = 1 << 3
-    ImageMask = 1 << 4
-class ImageFormatInfoType:
-    RGB = 0
-    YUV = 1
-class ImageFormatInfoFormat:
-    Packed = 0
-    Planar = 1
-class AttributeFlag:
-    Gettable = 1 << 0
-    Settable = 1 << 1
-class VideoNotifyReason:
-    Started = 0
-    Stopped = 1
-    Busy = 2
-    Preempted = 3
-    HardError = 4
-class ScanlineOrder:
-    TopToBottom = 0
-    BottomToTop = 1
-class GrabPortStatus:
-    Success = 0
-    BadExtension = 1
-    AlreadyGrabbed = 2
-    InvalidTime = 3
-    BadReply = 4
-    BadAlloc = 5
-class Rational(xcffib.Struct):
+
+
+class Attachment:
+    BufferFrontLeft = 0
+    BufferBackLeft = 1
+    BufferFrontRight = 2
+    BufferBackRight = 3
+    BufferDepth = 4
+    BufferStencil = 5
+    BufferAccum = 6
+    BufferFakeFrontLeft = 7
+    BufferFakeFrontRight = 8
+    BufferDepthStencil = 9
+    BufferHiz = 10
+
+
+class DriverType:
+    DRI = 0
+    VDPAU = 1
+
+
+class EventType:
+    ExchangeComplete = 1
+    BlitComplete = 2
+    FlipComplete = 3
+
+
+class DRI2Buffer(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.numerator, self.denominator = unpacker.unpack("ii")
+        self.attachment, self.name, self.pitch, self.cpp, self.flags = unpacker.unpack(
+            "IIIII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=ii", self.numerator, self.denominator))
+        buf.write(
+            struct.pack(
+                "=IIIII",
+                self.attachment,
+                self.name,
+                self.pitch,
+                self.cpp,
+                self.flags))
         return buf.getvalue()
-    fixed_size = 8
-class Format(xcffib.Struct):
+    fixed_size = 20
+
+
+class AttachFormat(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.visual, self.depth = unpacker.unpack("IB3x")
+        self.attachment, self.format = unpacker.unpack("II")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IB3x", self.visual, self.depth))
+        buf.write(struct.pack("=II", self.attachment, self.format))
         return buf.getvalue()
     fixed_size = 8
-class AdaptorInfo(xcffib.Struct):
+
+
+class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
-        xcffib.Struct.__init__(self, unpacker)
+        xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.base_id, self.name_size, self.num_ports, self.num_formats, self.type = unpacker.unpack("IHHHBx")
-        self.name = xcffib.List(unpacker, "c", self.name_size)
-        unpacker.pad(Format)
-        self.formats = xcffib.List(unpacker, Format, self.num_formats)
+        self.major_version, self.minor_version = unpacker.unpack("xx2x4xII")
         self.bufsize = unpacker.offset - base
-    def pack(self):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=IHHHBx", self.base_id, self.name_size, self.num_ports, self.num_formats, self.type))
-        buf.write(xcffib.pack_list(self.name, "c"))
-        buf.write(xcffib.pack_list(self.formats, Format))
-        return buf.getvalue()
-class EncodingInfo(xcffib.Struct):
+
+
+class QueryVersionCookie(xcffib.Cookie):
+    reply_type = QueryVersionReply
+
+
+class ConnectReply(xcffib.Reply):
+
     def __init__(self, unpacker):
-        xcffib.Struct.__init__(self, unpacker)
+        xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.encoding, self.name_size, self.width, self.height = unpacker.unpack("IHHH2x")
-        self.rate = Rational(unpacker)
+        self.driver_name_length, self.device_name_length = unpacker.unpack(
+            "xx2x4xII16x")
+        self.driver_name = xcffib.List(unpacker, "c", self.driver_name_length)
         unpacker.pad("c")
-        self.name = xcffib.List(unpacker, "c", self.name_size)
-        self.bufsize = unpacker.offset - base
-    def pack(self):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=IHHH2x", self.encoding, self.name_size, self.width, self.height))
-        buf.write(self.rate.pack())
-        buf.write(xcffib.pack_list(self.name, "c"))
-        return buf.getvalue()
-class Image(xcffib.Struct):
-    def __init__(self, unpacker):
-        xcffib.Struct.__init__(self, unpacker)
-        base = unpacker.offset
-        self.id, self.width, self.height, self.data_size, self.num_planes = unpacker.unpack("IHHII")
-        self.pitches = xcffib.List(unpacker, "I", self.num_planes)
-        unpacker.pad("I")
-        self.offsets = xcffib.List(unpacker, "I", self.num_planes)
-        unpacker.pad("B")
-        self.data = xcffib.List(unpacker, "B", self.data_size)
-        self.bufsize = unpacker.offset - base
-    def pack(self):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=IHHII", self.id, self.width, self.height, self.data_size, self.num_planes))
-        buf.write(xcffib.pack_list(self.pitches, "I"))
-        buf.write(xcffib.pack_list(self.offsets, "I"))
-        buf.write(xcffib.pack_list(self.data, "B"))
-        return buf.getvalue()
-class AttributeInfo(xcffib.Struct):
-    def __init__(self, unpacker):
-        xcffib.Struct.__init__(self, unpacker)
-        base = unpacker.offset
-        self.flags, self.min, self.max, self.size = unpacker.unpack("IiiI")
-        self.name = xcffib.List(unpacker, "c", self.size)
-        self.bufsize = unpacker.offset - base
-    def pack(self):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=IiiI", self.flags, self.min, self.max, self.size))
-        buf.write(xcffib.pack_list(self.name, "c"))
-        return buf.getvalue()
-class ImageFormatInfo(xcffib.Struct):
-    def __init__(self, unpacker):
-        xcffib.Struct.__init__(self, unpacker)
-        base = unpacker.offset
-        self.id, self.type, self.byte_order = unpacker.unpack("IBB2x")
-        self.guid = xcffib.List(unpacker, "B", 16)
-        self.bpp, self.num_planes, self.depth, self.red_mask, self.green_mask, self.blue_mask, self.format, self.y_sample_bits, self.u_sample_bits, self.v_sample_bits, self.vhorz_y_period, self.vhorz_u_period, self.vhorz_v_period, self.vvert_y_period, self.vvert_u_period, self.vvert_v_period = unpacker.unpack("BB2xB3xIIIB3xIIIIIIIII")
-        unpacker.pad("B")
-        self.vcomp_order = xcffib.List(unpacker, "B", 32)
-        self.vscanline_order, = unpacker.unpack("B11x")
+        self.alignment_pad = xcffib.List(
+            unpacker,
+            "c",
+            ((self.driver_name_length +
+              3) & (
+                ~ 3)) -
+            self.driver_name_length)
+        unpacker.pad("c")
+        self.device_name = xcffib.List(unpacker, "c", self.device_name_length)
         self.bufsize = unpacker.offset - base
-    def pack(self):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=IBB2xBB2xB3xIIIB3xIIIIIIIIIB11x", self.id, self.type, self.byte_order, self.bpp, self.num_planes, self.depth, self.red_mask, self.green_mask, self.blue_mask, self.format, self.y_sample_bits, self.u_sample_bits, self.v_sample_bits, self.vhorz_y_period, self.vhorz_u_period, self.vhorz_v_period, self.vvert_y_period, self.vvert_u_period, self.vvert_v_period, self.vscanline_order))
-        buf.write(xcffib.pack_list(self.guid, "B"))
-        buf.write(xcffib.pack_list(self.vcomp_order, "B"))
-        return buf.getvalue()
-    fixed_size = 128
-class VideoNotifyEvent(xcffib.Event):
+
+
+class ConnectCookie(xcffib.Cookie):
+    reply_type = ConnectReply
+
+
+class AuthenticateReply(xcffib.Reply):
+
     def __init__(self, unpacker):
-        xcffib.Event.__init__(self, unpacker)
+        xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.reason, self.time, self.drawable, self.port = unpacker.unpack("xB2xIII")
+        self.authenticated, = unpacker.unpack("xx2x4xI")
         self.bufsize = unpacker.offset - base
-    def pack(self):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=BIII", self.reason, self.time, self.drawable, self.port))
-        return buf.getvalue()
-_events[0] = VideoNotifyEvent
-class PortNotifyEvent(xcffib.Event):
+
+
+class AuthenticateCookie(xcffib.Cookie):
+    reply_type = AuthenticateReply
+
+
+class GetBuffersReply(xcffib.Reply):
+
     def __init__(self, unpacker):
-        xcffib.Event.__init__(self, unpacker)
+        xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.time, self.port, self.attribute, self.value = unpacker.unpack("xx2xIIIi")
+        self.width, self.height, self.count = unpacker.unpack("xx2x4xIII12x")
+        self.buffers = xcffib.List(unpacker, DRI2Buffer, self.count)
         self.bufsize = unpacker.offset - base
-    def pack(self):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xIIIi", self.time, self.port, self.attribute, self.value))
-        return buf.getvalue()
-_events[1] = PortNotifyEvent
-class QueryExtensionReply(xcffib.Reply):
+
+
+class GetBuffersCookie(xcffib.Cookie):
+    reply_type = GetBuffersReply
+
+
+class CopyRegionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.major, self.minor = unpacker.unpack("xx2x4xHH")
+        unpacker.unpack("xx2x4x")
         self.bufsize = unpacker.offset - base
-class QueryExtensionCookie(xcffib.Cookie):
-    reply_type = QueryExtensionReply
-class QueryAdaptorsReply(xcffib.Reply):
+
+
+class CopyRegionCookie(xcffib.Cookie):
+    reply_type = CopyRegionReply
+
+
+class GetBuffersWithFormatReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.num_adaptors, = unpacker.unpack("xx2x4xH22x")
-        self.info = xcffib.List(unpacker, AdaptorInfo, self.num_adaptors)
+        self.width, self.height, self.count = unpacker.unpack("xx2x4xIII12x")
+        self.buffers = xcffib.List(unpacker, DRI2Buffer, self.count)
         self.bufsize = unpacker.offset - base
-class QueryAdaptorsCookie(xcffib.Cookie):
-    reply_type = QueryAdaptorsReply
-class QueryEncodingsReply(xcffib.Reply):
+
+
+class GetBuffersWithFormatCookie(xcffib.Cookie):
+    reply_type = GetBuffersWithFormatReply
+
+
+class SwapBuffersReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.num_encodings, = unpacker.unpack("xx2x4xH22x")
-        self.info = xcffib.List(unpacker, EncodingInfo, self.num_encodings)
+        self.swap_hi, self.swap_lo = unpacker.unpack("xx2x4xII")
         self.bufsize = unpacker.offset - base
-class QueryEncodingsCookie(xcffib.Cookie):
-    reply_type = QueryEncodingsReply
-class GrabPortReply(xcffib.Reply):
+
+
+class SwapBuffersCookie(xcffib.Cookie):
+    reply_type = SwapBuffersReply
+
+
+class GetMSCReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.result, = unpacker.unpack("xB2x4x")
+        self.ust_hi, self.ust_lo, self.msc_hi, self.msc_lo, self.sbc_hi, self.sbc_lo = unpacker.unpack(
+            "xx2x4xIIIIII")
         self.bufsize = unpacker.offset - base
-class GrabPortCookie(xcffib.Cookie):
-    reply_type = GrabPortReply
-class QueryBestSizeReply(xcffib.Reply):
+
+
+class GetMSCCookie(xcffib.Cookie):
+    reply_type = GetMSCReply
+
+
+class WaitMSCReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.actual_width, self.actual_height = unpacker.unpack("xx2x4xHH")
+        self.ust_hi, self.ust_lo, self.msc_hi, self.msc_lo, self.sbc_hi, self.sbc_lo = unpacker.unpack(
+            "xx2x4xIIIIII")
         self.bufsize = unpacker.offset - base
-class QueryBestSizeCookie(xcffib.Cookie):
-    reply_type = QueryBestSizeReply
-class GetPortAttributeReply(xcffib.Reply):
+
+
+class WaitMSCCookie(xcffib.Cookie):
+    reply_type = WaitMSCReply
+
+
+class WaitSBCReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.value, = unpacker.unpack("xx2x4xi")
+        self.ust_hi, self.ust_lo, self.msc_hi, self.msc_lo, self.sbc_hi, self.sbc_lo = unpacker.unpack(
+            "xx2x4xIIIIII")
         self.bufsize = unpacker.offset - base
-class GetPortAttributeCookie(xcffib.Cookie):
-    reply_type = GetPortAttributeReply
-class QueryPortAttributesReply(xcffib.Reply):
+
+
+class WaitSBCCookie(xcffib.Cookie):
+    reply_type = WaitSBCReply
+
+
+class GetParamReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.num_attributes, self.text_size = unpacker.unpack("xx2x4xII16x")
-        self.attributes = xcffib.List(unpacker, AttributeInfo, self.num_attributes)
+        self.is_param_recognized, self.value_hi, self.value_lo = unpacker.unpack(
+            "xB2x4xII")
         self.bufsize = unpacker.offset - base
-class QueryPortAttributesCookie(xcffib.Cookie):
-    reply_type = QueryPortAttributesReply
-class ListImageFormatsReply(xcffib.Reply):
+
+
+class GetParamCookie(xcffib.Cookie):
+    reply_type = GetParamReply
+
+
+class BufferSwapCompleteEvent(xcffib.Event):
+
     def __init__(self, unpacker):
-        xcffib.Reply.__init__(self, unpacker)
+        xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.num_formats, = unpacker.unpack("xx2x4xI20x")
-        self.format = xcffib.List(unpacker, ImageFormatInfo, self.num_formats)
+        self.event_type, self.drawable, self.ust_hi, self.ust_lo, self.msc_hi, self.msc_lo, self.sbc = unpacker.unpack(
+            "xx2xH2xIIIIII")
         self.bufsize = unpacker.offset - base
-class ListImageFormatsCookie(xcffib.Cookie):
-    reply_type = ListImageFormatsReply
-class QueryImageAttributesReply(xcffib.Reply):
+
+    def pack(self):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xH2xIIIIII",
+                self.event_type,
+                self.drawable,
+                self.ust_hi,
+                self.ust_lo,
+                self.msc_hi,
+                self.msc_lo,
+                self.sbc))
+        return buf.getvalue()
+_events[0] = BufferSwapCompleteEvent
+
+
+class InvalidateBuffersEvent(xcffib.Event):
+
     def __init__(self, unpacker):
-        xcffib.Reply.__init__(self, unpacker)
+        xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.num_planes, self.data_size, self.width, self.height = unpacker.unpack("xx2x4xIIHH12x")
-        self.pitches = xcffib.List(unpacker, "I", self.num_planes)
-        unpacker.pad("I")
-        self.offsets = xcffib.List(unpacker, "I", self.num_planes)
+        self.drawable, = unpacker.unpack("xx2xI")
         self.bufsize = unpacker.offset - base
-class QueryImageAttributesCookie(xcffib.Cookie):
-    reply_type = QueryImageAttributesReply
-class xvExtension(xcffib.Extension):
-    def QueryExtension(self, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2x"))
-        return self.send_request(0, buf, QueryExtensionCookie, is_checked=is_checked)
-    def QueryAdaptors(self, window, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(1, buf, QueryAdaptorsCookie, is_checked=is_checked)
-    def QueryEncodings(self, port, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", port))
-        return self.send_request(2, buf, QueryEncodingsCookie, is_checked=is_checked)
-    def GrabPort(self, port, time, is_checked=True):
+
+    def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xII", port, time))
-        return self.send_request(3, buf, GrabPortCookie, is_checked=is_checked)
-    def UngrabPort(self, port, time, is_checked=False):
+        buf.write(struct.pack("=xI", self.drawable))
+        return buf.getvalue()
+_events[1] = InvalidateBuffersEvent
+
+
+class dri2Extension(xcffib.Extension):
+
+    def QueryVersion(self, major_version, minor_version, is_checked=True):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xII", major_version, minor_version))
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
+    def Connect(self, window, driver_type, is_checked=True):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xII", window, driver_type))
+        return self.send_request(1, buf, ConnectCookie, is_checked=is_checked)
+
+    def Authenticate(self, window, magic, is_checked=True):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xII", window, magic))
+        return self.send_request(
+            2,
+            buf,
+            AuthenticateCookie,
+            is_checked=is_checked)
+
+    def CreateDrawable(self, drawable, is_checked=False):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xI", drawable))
+        return self.send_request(3, buf, is_checked=is_checked)
+
+    def DestroyDrawable(self, drawable, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xII", port, time))
+        buf.write(struct.pack("=xx2xI", drawable))
         return self.send_request(4, buf, is_checked=is_checked)
-    def PutVideo(self, port, drawable, gc, vid_x, vid_y, vid_w, vid_h, drw_x, drw_y, drw_w, drw_h, is_checked=False):
+
+    def GetBuffers(self, drawable, count, attachments, is_checked=True):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIhhHHhhHH", port, drawable, gc, vid_x, vid_y, vid_w, vid_h, drw_x, drw_y, drw_w, drw_h))
-        return self.send_request(5, buf, is_checked=is_checked)
-    def PutStill(self, port, drawable, gc, vid_x, vid_y, vid_w, vid_h, drw_x, drw_y, drw_w, drw_h, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIhhHHhhHH", port, drawable, gc, vid_x, vid_y, vid_w, vid_h, drw_x, drw_y, drw_w, drw_h))
-        return self.send_request(6, buf, is_checked=is_checked)
-    def GetVideo(self, port, drawable, gc, vid_x, vid_y, vid_w, vid_h, drw_x, drw_y, drw_w, drw_h, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIhhHHhhHH", port, drawable, gc, vid_x, vid_y, vid_w, vid_h, drw_x, drw_y, drw_w, drw_h))
-        return self.send_request(7, buf, is_checked=is_checked)
-    def GetStill(self, port, drawable, gc, vid_x, vid_y, vid_w, vid_h, drw_x, drw_y, drw_w, drw_h, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIhhHHhhHH", port, drawable, gc, vid_x, vid_y, vid_w, vid_h, drw_x, drw_y, drw_w, drw_h))
-        return self.send_request(8, buf, is_checked=is_checked)
-    def StopVideo(self, port, drawable, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xII", port, drawable))
-        return self.send_request(9, buf, is_checked=is_checked)
-    def SelectVideoNotify(self, drawable, onoff, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIB3x", drawable, onoff))
-        return self.send_request(10, buf, is_checked=is_checked)
-    def SelectPortNotify(self, port, onoff, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIB3x", port, onoff))
-        return self.send_request(11, buf, is_checked=is_checked)
-    def QueryBestSize(self, port, vid_w, vid_h, drw_w, drw_h, motion, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIHHHHB3x", port, vid_w, vid_h, drw_w, drw_h, motion))
-        return self.send_request(12, buf, QueryBestSizeCookie, is_checked=is_checked)
-    def SetPortAttribute(self, port, attribute, value, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIi", port, attribute, value))
-        return self.send_request(13, buf, is_checked=is_checked)
-    def GetPortAttribute(self, port, attribute, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xII", port, attribute))
-        return self.send_request(14, buf, GetPortAttributeCookie, is_checked=is_checked)
-    def QueryPortAttributes(self, port, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", port))
-        return self.send_request(15, buf, QueryPortAttributesCookie, is_checked=is_checked)
-    def ListImageFormats(self, port, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", port))
-        return self.send_request(16, buf, ListImageFormatsCookie, is_checked=is_checked)
-    def QueryImageAttributes(self, port, id, width, height, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIHH", port, id, width, height))
-        return self.send_request(17, buf, QueryImageAttributesCookie, is_checked=is_checked)
-    def PutImage(self, port, drawable, gc, id, src_x, src_y, src_w, src_h, drw_x, drw_y, drw_w, drw_h, width, height, data, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIIhhHHhhHHHH", port, drawable, gc, id, src_x, src_y, src_w, src_h, drw_x, drw_y, drw_w, drw_h, width, height))
-        buf.write(xcffib.pack_list(data, "B"))
-        return self.send_request(18, buf, is_checked=is_checked)
-    def ShmPutImage(self, port, drawable, gc, shmseg, id, offset, src_x, src_y, src_w, src_h, drw_x, drw_y, drw_w, drw_h, width, height, send_event, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIIIIhhHHhhHHHHB3x", port, drawable, gc, shmseg, id, offset, src_x, src_y, src_w, src_h, drw_x, drw_y, drw_w, drw_h, width, height, send_event))
-        return self.send_request(19, buf, is_checked=is_checked)
-xcffib._add_ext(key, xvExtension, _events, _errors)
+        buf.write(struct.pack("=xx2xII", drawable, count))
+        buf.write(xcffib.pack_list(attachments, "I"))
+        return self.send_request(
+            5,
+            buf,
+            GetBuffersCookie,
+            is_checked=is_checked)
+
+    def CopyRegion(self, drawable, region, dest, src, is_checked=True):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xIIII", drawable, region, dest, src))
+        return self.send_request(
+            6,
+            buf,
+            CopyRegionCookie,
+            is_checked=is_checked)
+
+    def GetBuffersWithFormat(
+            self,
+            drawable,
+            count,
+            attachments,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xII", drawable, count))
+        buf.write(xcffib.pack_list(attachments, AttachFormat))
+        return self.send_request(
+            7,
+            buf,
+            GetBuffersWithFormatCookie,
+            is_checked=is_checked)
+
+    def SwapBuffers(
+            self,
+            drawable,
+            target_msc_hi,
+            target_msc_lo,
+            divisor_hi,
+            divisor_lo,
+            remainder_hi,
+            remainder_lo,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIIIII",
+                drawable,
+                target_msc_hi,
+                target_msc_lo,
+                divisor_hi,
+                divisor_lo,
+                remainder_hi,
+                remainder_lo))
+        return self.send_request(
+            8,
+            buf,
+            SwapBuffersCookie,
+            is_checked=is_checked)
+
+    def GetMSC(self, drawable, is_checked=True):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xI", drawable))
+        return self.send_request(9, buf, GetMSCCookie, is_checked=is_checked)
+
+    def WaitMSC(
+            self,
+            drawable,
+            target_msc_hi,
+            target_msc_lo,
+            divisor_hi,
+            divisor_lo,
+            remainder_hi,
+            remainder_lo,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIIIII",
+                drawable,
+                target_msc_hi,
+                target_msc_lo,
+                divisor_hi,
+                divisor_lo,
+                remainder_hi,
+                remainder_lo))
+        return self.send_request(10, buf, WaitMSCCookie, is_checked=is_checked)
+
+    def WaitSBC(self, drawable, target_sbc_hi, target_sbc_lo, is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIII",
+                drawable,
+                target_sbc_hi,
+                target_sbc_lo))
+        return self.send_request(11, buf, WaitSBCCookie, is_checked=is_checked)
+
+    def SwapInterval(self, drawable, interval, is_checked=False):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xII", drawable, interval))
+        return self.send_request(12, buf, is_checked=is_checked)
+
+    def GetParam(self, drawable, param, is_checked=True):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xII", drawable, param))
+        return self.send_request(
+            13,
+            buf,
+            GetParamCookie,
+            is_checked=is_checked)
+xcffib._add_ext(key, dri2Extension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/render.py` & `xcffib-v0.1.4/xcffib/render.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,19 +3,25 @@
 import six
 MAJOR_VERSION = 0
 MINOR_VERSION = 11
 key = xcffib.ExtensionKey("RENDER")
 _events = {}
 _errors = {}
 from . import xproto
+
+
 class PictType:
     Indexed = 0
     Direct = 1
+
+
 class Picture:
     _None = 0
+
+
 class PictOp:
     Clear = 0
     Src = 1
     Dst = 2
     Over = 3
     OverReverse = 4
     In = 5
@@ -62,434 +68,854 @@
     SoftLight = 56
     Difference = 57
     Exclusion = 58
     HSLHue = 59
     HSLSaturation = 60
     HSLColor = 61
     HSLLuminosity = 62
+
+
 class PolyEdge:
     Sharp = 0
     Smooth = 1
+
+
 class PolyMode:
     Precise = 0
     Imprecise = 1
+
+
 class CP:
     Repeat = 1 << 0
     AlphaMap = 1 << 1
     AlphaXOrigin = 1 << 2
     AlphaYOrigin = 1 << 3
     ClipXOrigin = 1 << 4
     ClipYOrigin = 1 << 5
     ClipMask = 1 << 6
     GraphicsExposure = 1 << 7
     SubwindowMode = 1 << 8
     PolyEdge = 1 << 9
     PolyMode = 1 << 10
     Dither = 1 << 11
     ComponentAlpha = 1 << 12
+
+
 class SubPixel:
     Unknown = 0
     HorizontalRGB = 1
     HorizontalBGR = 2
     VerticalRGB = 3
     VerticalBGR = 4
     _None = 5
+
+
 class Repeat:
     _None = 0
     Normal = 1
     Pad = 2
     Reflect = 3
+
+
 class DIRECTFORMAT(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.red_shift, self.red_mask, self.green_shift, self.green_mask, self.blue_shift, self.blue_mask, self.alpha_shift, self.alpha_mask = unpacker.unpack("HHHHHHHH")
+        self.red_shift, self.red_mask, self.green_shift, self.green_mask, self.blue_shift, self.blue_mask, self.alpha_shift, self.alpha_mask = unpacker.unpack(
+            "HHHHHHHH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHHHHHHH", self.red_shift, self.red_mask, self.green_shift, self.green_mask, self.blue_shift, self.blue_mask, self.alpha_shift, self.alpha_mask))
+        buf.write(
+            struct.pack(
+                "=HHHHHHHH",
+                self.red_shift,
+                self.red_mask,
+                self.green_shift,
+                self.green_mask,
+                self.blue_shift,
+                self.blue_mask,
+                self.alpha_shift,
+                self.alpha_mask))
         return buf.getvalue()
     fixed_size = 16
+
+
 class PICTFORMINFO(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.id, self.type, self.depth = unpacker.unpack("IBB2x")
         self.direct = DIRECTFORMAT(unpacker)
         self.colormap, = unpacker.unpack("I")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IBB2xI", self.id, self.type, self.depth, self.colormap))
+        buf.write(
+            struct.pack(
+                "=IBB2xI",
+                self.id,
+                self.type,
+                self.depth,
+                self.colormap))
         buf.write(self.direct.pack())
         return buf.getvalue()
+
+
 class PICTVISUAL(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.visual, self.format = unpacker.unpack("II")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=II", self.visual, self.format))
         return buf.getvalue()
     fixed_size = 8
+
+
 class PICTDEPTH(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.depth, self.num_visuals = unpacker.unpack("BxH4x")
         self.visuals = xcffib.List(unpacker, PICTVISUAL, self.num_visuals)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=BxH4x", self.depth, self.num_visuals))
         buf.write(xcffib.pack_list(self.visuals, PICTVISUAL))
         return buf.getvalue()
+
+
 class PICTSCREEN(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.num_depths, self.fallback = unpacker.unpack("II")
         self.depths = xcffib.List(unpacker, PICTDEPTH, self.num_depths)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=II", self.num_depths, self.fallback))
         buf.write(xcffib.pack_list(self.depths, PICTDEPTH))
         return buf.getvalue()
+
+
 class INDEXVALUE(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.pixel, self.red, self.green, self.blue, self.alpha = unpacker.unpack("IHHHH")
+        self.pixel, self.red, self.green, self.blue, self.alpha = unpacker.unpack(
+            "IHHHH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHHHH", self.pixel, self.red, self.green, self.blue, self.alpha))
+        buf.write(
+            struct.pack(
+                "=IHHHH",
+                self.pixel,
+                self.red,
+                self.green,
+                self.blue,
+                self.alpha))
         return buf.getvalue()
     fixed_size = 12
+
+
 class COLOR(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.red, self.green, self.blue, self.alpha = unpacker.unpack("HHHH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHHH", self.red, self.green, self.blue, self.alpha))
+        buf.write(
+            struct.pack(
+                "=HHHH",
+                self.red,
+                self.green,
+                self.blue,
+                self.alpha))
         return buf.getvalue()
     fixed_size = 8
+
+
 class POINTFIX(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.x, self.y = unpacker.unpack("ii")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=ii", self.x, self.y))
         return buf.getvalue()
     fixed_size = 8
+
+
 class LINEFIX(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.p1 = POINTFIX(unpacker)
         unpacker.pad(POINTFIX)
         self.p2 = POINTFIX(unpacker)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(self.p1.pack())
         buf.write(self.p2.pack())
         return buf.getvalue()
+
+
 class TRIANGLE(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.p1 = POINTFIX(unpacker)
         unpacker.pad(POINTFIX)
         self.p2 = POINTFIX(unpacker)
         unpacker.pad(POINTFIX)
         self.p3 = POINTFIX(unpacker)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(self.p1.pack())
         buf.write(self.p2.pack())
         buf.write(self.p3.pack())
         return buf.getvalue()
+
+
 class TRAPEZOID(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.top, self.bottom = unpacker.unpack("ii")
         self.left = LINEFIX(unpacker)
         unpacker.pad(LINEFIX)
         self.right = LINEFIX(unpacker)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=ii", self.top, self.bottom))
         buf.write(self.left.pack())
         buf.write(self.right.pack())
         return buf.getvalue()
+
+
 class GLYPHINFO(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.width, self.height, self.x, self.y, self.x_off, self.y_off = unpacker.unpack("HHhhhh")
+        self.width, self.height, self.x, self.y, self.x_off, self.y_off = unpacker.unpack(
+            "HHhhhh")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHhhhh", self.width, self.height, self.x, self.y, self.x_off, self.y_off))
+        buf.write(
+            struct.pack(
+                "=HHhhhh",
+                self.width,
+                self.height,
+                self.x,
+                self.y,
+                self.x_off,
+                self.y_off))
         return buf.getvalue()
     fixed_size = 12
+
+
 class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.major_version, self.minor_version = unpacker.unpack("xx2x4xII16x")
         self.bufsize = unpacker.offset - base
+
+
 class QueryVersionCookie(xcffib.Cookie):
     reply_type = QueryVersionReply
+
+
 class QueryPictFormatsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.num_formats, self.num_screens, self.num_depths, self.num_visuals, self.num_subpixel = unpacker.unpack("xx2x4xIIIII4x")
+        self.num_formats, self.num_screens, self.num_depths, self.num_visuals, self.num_subpixel = unpacker.unpack(
+            "xx2x4xIIIII4x")
         self.formats = xcffib.List(unpacker, PICTFORMINFO, self.num_formats)
         unpacker.pad(PICTSCREEN)
         self.screens = xcffib.List(unpacker, PICTSCREEN, self.num_screens)
         unpacker.pad("I")
         self.subpixels = xcffib.List(unpacker, "I", self.num_subpixel)
         self.bufsize = unpacker.offset - base
+
+
 class QueryPictFormatsCookie(xcffib.Cookie):
     reply_type = QueryPictFormatsReply
+
+
 class QueryPictIndexValuesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_values, = unpacker.unpack("xx2x4xI20x")
         self.values = xcffib.List(unpacker, INDEXVALUE, self.num_values)
         self.bufsize = unpacker.offset - base
+
+
 class QueryPictIndexValuesCookie(xcffib.Cookie):
     reply_type = QueryPictIndexValuesReply
+
+
 class TRANSFORM(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.matrix11, self.matrix12, self.matrix13, self.matrix21, self.matrix22, self.matrix23, self.matrix31, self.matrix32, self.matrix33 = unpacker.unpack("iiiiiiiii")
+        self.matrix11, self.matrix12, self.matrix13, self.matrix21, self.matrix22, self.matrix23, self.matrix31, self.matrix32, self.matrix33 = unpacker.unpack(
+            "iiiiiiiii")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=iiiiiiiii", self.matrix11, self.matrix12, self.matrix13, self.matrix21, self.matrix22, self.matrix23, self.matrix31, self.matrix32, self.matrix33))
+        buf.write(
+            struct.pack(
+                "=iiiiiiiii",
+                self.matrix11,
+                self.matrix12,
+                self.matrix13,
+                self.matrix21,
+                self.matrix22,
+                self.matrix23,
+                self.matrix31,
+                self.matrix32,
+                self.matrix33))
         return buf.getvalue()
     fixed_size = 36
+
+
 class QueryFiltersReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_aliases, self.num_filters = unpacker.unpack("xx2x4xII16x")
         self.aliases = xcffib.List(unpacker, "H", self.num_aliases)
         unpacker.pad(xproto.STR)
         self.filters = xcffib.List(unpacker, xproto.STR, self.num_filters)
         self.bufsize = unpacker.offset - base
+
+
 class QueryFiltersCookie(xcffib.Cookie):
     reply_type = QueryFiltersReply
+
+
 class ANIMCURSORELT(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.cursor, self.delay = unpacker.unpack("II")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=II", self.cursor, self.delay))
         return buf.getvalue()
     fixed_size = 8
+
+
 class SPANFIX(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.l, self.r, self.y = unpacker.unpack("iii")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=iii", self.l, self.r, self.y))
         return buf.getvalue()
     fixed_size = 12
+
+
 class TRAP(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.top = SPANFIX(unpacker)
         unpacker.pad(SPANFIX)
         self.bot = SPANFIX(unpacker)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(self.top.pack())
         buf.write(self.bot.pack())
         return buf.getvalue()
+
+
 class renderExtension(xcffib.Extension):
-    def QueryVersion(self, client_major_version, client_minor_version, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xII", client_major_version, client_minor_version))
-        return self.send_request(0, buf, QueryVersionCookie, is_checked=is_checked)
+
+    def QueryVersion(
+            self,
+            client_major_version,
+            client_minor_version,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xII",
+                client_major_version,
+                client_minor_version))
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
     def QueryPictFormats(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(1, buf, QueryPictFormatsCookie, is_checked=is_checked)
+        return self.send_request(
+            1,
+            buf,
+            QueryPictFormatsCookie,
+            is_checked=is_checked)
+
     def QueryPictIndexValues(self, format, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", format))
-        return self.send_request(2, buf, QueryPictIndexValuesCookie, is_checked=is_checked)
-    def CreatePicture(self, pid, drawable, format, value_mask, value_list, is_checked=False):
+        return self.send_request(
+            2,
+            buf,
+            QueryPictIndexValuesCookie,
+            is_checked=is_checked)
+
+    def CreatePicture(
+            self,
+            pid,
+            drawable,
+            format,
+            value_mask,
+            value_list,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", pid, drawable, format))
         buf.write(struct.pack("=I", value_mask))
         buf.write(xcffib.pack_list(value_list, "I"))
         return self.send_request(4, buf, is_checked=is_checked)
+
     def ChangePicture(self, picture, value_mask, value_list, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", picture))
         buf.write(struct.pack("=I", value_mask))
         buf.write(xcffib.pack_list(value_list, "I"))
         return self.send_request(5, buf, is_checked=is_checked)
-    def SetPictureClipRectangles(self, picture, clip_x_origin, clip_y_origin, rectangles, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIhh", picture, clip_x_origin, clip_y_origin))
+
+    def SetPictureClipRectangles(
+            self,
+            picture,
+            clip_x_origin,
+            clip_y_origin,
+            rectangles,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIhh",
+                picture,
+                clip_x_origin,
+                clip_y_origin))
         buf.write(xcffib.pack_list(rectangles, xproto.RECTANGLE))
         return self.send_request(6, buf, is_checked=is_checked)
+
     def FreePicture(self, picture, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", picture))
         return self.send_request(7, buf, is_checked=is_checked)
-    def Composite(self, op, src, mask, dst, src_x, src_y, mask_x, mask_y, dst_x, dst_y, width, height, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2x3xIIIhhhhhhHH", op, src, mask, dst, src_x, src_y, mask_x, mask_y, dst_x, dst_y, width, height))
+
+    def Composite(
+            self,
+            op,
+            src,
+            mask,
+            dst,
+            src_x,
+            src_y,
+            mask_x,
+            mask_y,
+            dst_x,
+            dst_y,
+            width,
+            height,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2x3xIIIhhhhhhHH",
+                op,
+                src,
+                mask,
+                dst,
+                src_x,
+                src_y,
+                mask_x,
+                mask_y,
+                dst_x,
+                dst_y,
+                width,
+                height))
         return self.send_request(8, buf, is_checked=is_checked)
-    def Trapezoids(self, op, src, dst, mask_format, src_x, src_y, traps, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2x3xIIIhh", op, src, dst, mask_format, src_x, src_y))
+
+    def Trapezoids(
+            self,
+            op,
+            src,
+            dst,
+            mask_format,
+            src_x,
+            src_y,
+            traps,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2x3xIIIhh",
+                op,
+                src,
+                dst,
+                mask_format,
+                src_x,
+                src_y))
         buf.write(xcffib.pack_list(traps, TRAPEZOID))
         return self.send_request(10, buf, is_checked=is_checked)
-    def Triangles(self, op, src, dst, mask_format, src_x, src_y, triangles, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2x3xIIIhh", op, src, dst, mask_format, src_x, src_y))
+
+    def Triangles(
+            self,
+            op,
+            src,
+            dst,
+            mask_format,
+            src_x,
+            src_y,
+            triangles,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2x3xIIIhh",
+                op,
+                src,
+                dst,
+                mask_format,
+                src_x,
+                src_y))
         buf.write(xcffib.pack_list(triangles, TRIANGLE))
         return self.send_request(11, buf, is_checked=is_checked)
-    def TriStrip(self, op, src, dst, mask_format, src_x, src_y, points, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2x3xIIIhh", op, src, dst, mask_format, src_x, src_y))
+
+    def TriStrip(
+            self,
+            op,
+            src,
+            dst,
+            mask_format,
+            src_x,
+            src_y,
+            points,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2x3xIIIhh",
+                op,
+                src,
+                dst,
+                mask_format,
+                src_x,
+                src_y))
         buf.write(xcffib.pack_list(points, POINTFIX))
         return self.send_request(12, buf, is_checked=is_checked)
-    def TriFan(self, op, src, dst, mask_format, src_x, src_y, points, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2x3xIIIhh", op, src, dst, mask_format, src_x, src_y))
+
+    def TriFan(
+            self,
+            op,
+            src,
+            dst,
+            mask_format,
+            src_x,
+            src_y,
+            points,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2x3xIIIhh",
+                op,
+                src,
+                dst,
+                mask_format,
+                src_x,
+                src_y))
         buf.write(xcffib.pack_list(points, POINTFIX))
         return self.send_request(13, buf, is_checked=is_checked)
+
     def CreateGlyphSet(self, gsid, format, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", gsid, format))
         return self.send_request(17, buf, is_checked=is_checked)
+
     def ReferenceGlyphSet(self, gsid, existing, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", gsid, existing))
         return self.send_request(18, buf, is_checked=is_checked)
+
     def FreeGlyphSet(self, glyphset, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", glyphset))
         return self.send_request(19, buf, is_checked=is_checked)
-    def AddGlyphs(self, glyphset, glyphs_len, glyphids, glyphs, data, is_checked=False):
+
+    def AddGlyphs(
+            self,
+            glyphset,
+            glyphs_len,
+            glyphids,
+            glyphs,
+            data,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", glyphset, glyphs_len))
         buf.write(xcffib.pack_list(glyphids, "I"))
         buf.write(xcffib.pack_list(glyphs, GLYPHINFO))
         buf.write(xcffib.pack_list(data, "B"))
         return self.send_request(20, buf, is_checked=is_checked)
+
     def FreeGlyphs(self, glyphset, glyphs, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", glyphset))
         buf.write(xcffib.pack_list(glyphs, "I"))
         return self.send_request(22, buf, is_checked=is_checked)
-    def CompositeGlyphs8(self, op, src, dst, mask_format, glyphset, src_x, src_y, glyphcmds, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2x3xIIIIhh", op, src, dst, mask_format, glyphset, src_x, src_y))
+
+    def CompositeGlyphs8(
+            self,
+            op,
+            src,
+            dst,
+            mask_format,
+            glyphset,
+            src_x,
+            src_y,
+            glyphcmds,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2x3xIIIIhh",
+                op,
+                src,
+                dst,
+                mask_format,
+                glyphset,
+                src_x,
+                src_y))
         buf.write(xcffib.pack_list(glyphcmds, "B"))
         return self.send_request(23, buf, is_checked=is_checked)
-    def CompositeGlyphs16(self, op, src, dst, mask_format, glyphset, src_x, src_y, glyphcmds, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2x3xIIIIhh", op, src, dst, mask_format, glyphset, src_x, src_y))
+
+    def CompositeGlyphs16(
+            self,
+            op,
+            src,
+            dst,
+            mask_format,
+            glyphset,
+            src_x,
+            src_y,
+            glyphcmds,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2x3xIIIIhh",
+                op,
+                src,
+                dst,
+                mask_format,
+                glyphset,
+                src_x,
+                src_y))
         buf.write(xcffib.pack_list(glyphcmds, "B"))
         return self.send_request(24, buf, is_checked=is_checked)
-    def CompositeGlyphs32(self, op, src, dst, mask_format, glyphset, src_x, src_y, glyphcmds, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2x3xIIIIhh", op, src, dst, mask_format, glyphset, src_x, src_y))
+
+    def CompositeGlyphs32(
+            self,
+            op,
+            src,
+            dst,
+            mask_format,
+            glyphset,
+            src_x,
+            src_y,
+            glyphcmds,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2x3xIIIIhh",
+                op,
+                src,
+                dst,
+                mask_format,
+                glyphset,
+                src_x,
+                src_y))
         buf.write(xcffib.pack_list(glyphcmds, "B"))
         return self.send_request(25, buf, is_checked=is_checked)
+
     def FillRectangles(self, op, dst, color, rects, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x3xI", op, dst))
         buf.write(color.pack())
         buf.write(xcffib.pack_list(rects, xproto.RECTANGLE))
         return self.send_request(26, buf, is_checked=is_checked)
+
     def CreateCursor(self, cid, source, x, y, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIHH", cid, source, x, y))
         return self.send_request(27, buf, is_checked=is_checked)
+
     def SetPictureTransform(self, picture, transform, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", picture))
         buf.write(transform.pack())
         return self.send_request(28, buf, is_checked=is_checked)
+
     def QueryFilters(self, drawable, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", drawable))
-        return self.send_request(29, buf, QueryFiltersCookie, is_checked=is_checked)
-    def SetPictureFilter(self, picture, filter_len, filter, values, is_checked=False):
+        return self.send_request(
+            29,
+            buf,
+            QueryFiltersCookie,
+            is_checked=is_checked)
+
+    def SetPictureFilter(
+            self,
+            picture,
+            filter_len,
+            filter,
+            values,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIH2x", picture, filter_len))
         buf.write(xcffib.pack_list(filter, "c"))
         buf.write(xcffib.pack_list(values, "i"))
         return self.send_request(30, buf, is_checked=is_checked)
+
     def CreateAnimCursor(self, cid, cursors, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", cid))
         buf.write(xcffib.pack_list(cursors, ANIMCURSORELT))
         return self.send_request(31, buf, is_checked=is_checked)
+
     def AddTraps(self, picture, x_off, y_off, traps, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIhh", picture, x_off, y_off))
         buf.write(xcffib.pack_list(traps, TRAP))
         return self.send_request(32, buf, is_checked=is_checked)
+
     def CreateSolidFill(self, picture, color, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", picture))
         buf.write(color.pack())
         return self.send_request(33, buf, is_checked=is_checked)
-    def CreateLinearGradient(self, picture, num_stops, p1, p2, stops, colors, is_checked=False):
+
+    def CreateLinearGradient(
+            self,
+            picture,
+            num_stops,
+            p1,
+            p2,
+            stops,
+            colors,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", picture, num_stops))
         buf.write(p1.pack())
         buf.write(p2.pack())
         buf.write(xcffib.pack_list(stops, "i"))
         buf.write(xcffib.pack_list(colors, COLOR))
         return self.send_request(34, buf, is_checked=is_checked)
-    def CreateRadialGradient(self, picture, inner_radius, outer_radius, num_stops, inner, outer, stops, colors, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIiiI", picture, inner_radius, outer_radius, num_stops))
+
+    def CreateRadialGradient(
+            self,
+            picture,
+            inner_radius,
+            outer_radius,
+            num_stops,
+            inner,
+            outer,
+            stops,
+            colors,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIiiI",
+                picture,
+                inner_radius,
+                outer_radius,
+                num_stops))
         buf.write(inner.pack())
         buf.write(outer.pack())
         buf.write(xcffib.pack_list(stops, "i"))
         buf.write(xcffib.pack_list(colors, COLOR))
         return self.send_request(35, buf, is_checked=is_checked)
-    def CreateConicalGradient(self, picture, angle, num_stops, center, stops, colors, is_checked=False):
+
+    def CreateConicalGradient(
+            self,
+            picture,
+            angle,
+            num_stops,
+            center,
+            stops,
+            colors,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIiI", picture, angle, num_stops))
         buf.write(center.pack())
         buf.write(xcffib.pack_list(stops, "i"))
         buf.write(xcffib.pack_list(colors, COLOR))
         return self.send_request(36, buf, is_checked=is_checked)
 xcffib._add_ext(key, renderExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/res.py` & `xcffib-v0.1.4/xcffib/res.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,176 +3,276 @@
 import six
 MAJOR_VERSION = 1
 MINOR_VERSION = 2
 key = xcffib.ExtensionKey("X-Resource")
 _events = {}
 _errors = {}
 from . import xproto
+
+
 class Client(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.resource_base, self.resource_mask = unpacker.unpack("II")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=II", self.resource_base, self.resource_mask))
         return buf.getvalue()
     fixed_size = 8
+
+
 class Type(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.resource_type, self.count = unpacker.unpack("II")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=II", self.resource_type, self.count))
         return buf.getvalue()
     fixed_size = 8
+
+
 class ClientIdMask:
     ClientXID = 1 << 0
     LocalClientPID = 1 << 1
+
+
 class ClientIdSpec(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.client, self.mask = unpacker.unpack("II")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=II", self.client, self.mask))
         return buf.getvalue()
     fixed_size = 8
+
+
 class ClientIdValue(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.spec = ClientIdSpec(unpacker)
         self.length, = unpacker.unpack("I")
         unpacker.pad("I")
         self.value = xcffib.List(unpacker, "I", self.length)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=I", self.length))
         buf.write(self.spec.pack())
         buf.write(xcffib.pack_list(self.value, "I"))
         return buf.getvalue()
+
+
 class ResourceIdSpec(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.resource, self.type = unpacker.unpack("II")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=II", self.resource, self.type))
         return buf.getvalue()
     fixed_size = 8
+
+
 class ResourceSizeSpec(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.spec = ResourceIdSpec(unpacker)
         self.bytes, self.ref_count, self.use_count = unpacker.unpack("III")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=III", self.bytes, self.ref_count, self.use_count))
+        buf.write(
+            struct.pack(
+                "=III",
+                self.bytes,
+                self.ref_count,
+                self.use_count))
         buf.write(self.spec.pack())
         return buf.getvalue()
+
+
 class ResourceSizeValue(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.size = ResourceSizeSpec(unpacker)
         self.num_cross_references, = unpacker.unpack("I")
         unpacker.pad(ResourceSizeSpec)
-        self.cross_references = xcffib.List(unpacker, ResourceSizeSpec, self.num_cross_references)
+        self.cross_references = xcffib.List(
+            unpacker,
+            ResourceSizeSpec,
+            self.num_cross_references)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=I", self.num_cross_references))
         buf.write(self.size.pack())
         buf.write(xcffib.pack_list(self.cross_references, ResourceSizeSpec))
         return buf.getvalue()
+
+
 class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.server_major, self.server_minor = unpacker.unpack("xx2x4xHH")
         self.bufsize = unpacker.offset - base
+
+
 class QueryVersionCookie(xcffib.Cookie):
     reply_type = QueryVersionReply
+
+
 class QueryClientsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_clients, = unpacker.unpack("xx2x4xI20x")
         self.clients = xcffib.List(unpacker, Client, self.num_clients)
         self.bufsize = unpacker.offset - base
+
+
 class QueryClientsCookie(xcffib.Cookie):
     reply_type = QueryClientsReply
+
+
 class QueryClientResourcesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_types, = unpacker.unpack("xx2x4xI20x")
         self.types = xcffib.List(unpacker, Type, self.num_types)
         self.bufsize = unpacker.offset - base
+
+
 class QueryClientResourcesCookie(xcffib.Cookie):
     reply_type = QueryClientResourcesReply
+
+
 class QueryClientPixmapBytesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.bytes, self.bytes_overflow = unpacker.unpack("xx2x4xII")
         self.bufsize = unpacker.offset - base
+
+
 class QueryClientPixmapBytesCookie(xcffib.Cookie):
     reply_type = QueryClientPixmapBytesReply
+
+
 class QueryClientIdsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_ids, = unpacker.unpack("xx2x4xI20x")
         self.ids = xcffib.List(unpacker, ClientIdValue, self.num_ids)
         self.bufsize = unpacker.offset - base
+
+
 class QueryClientIdsCookie(xcffib.Cookie):
     reply_type = QueryClientIdsReply
+
+
 class QueryResourceBytesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_sizes, = unpacker.unpack("xx2x4xI20x")
         self.sizes = xcffib.List(unpacker, ResourceSizeValue, self.num_sizes)
         self.bufsize = unpacker.offset - base
+
+
 class QueryResourceBytesCookie(xcffib.Cookie):
     reply_type = QueryResourceBytesReply
+
+
 class resExtension(xcffib.Extension):
+
     def QueryVersion(self, client_major, client_minor, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xB", client_major, client_minor))
-        return self.send_request(0, buf, QueryVersionCookie, is_checked=is_checked)
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
     def QueryClients(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(1, buf, QueryClientsCookie, is_checked=is_checked)
+        return self.send_request(
+            1,
+            buf,
+            QueryClientsCookie,
+            is_checked=is_checked)
+
     def QueryClientResources(self, xid, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", xid))
-        return self.send_request(2, buf, QueryClientResourcesCookie, is_checked=is_checked)
+        return self.send_request(
+            2,
+            buf,
+            QueryClientResourcesCookie,
+            is_checked=is_checked)
+
     def QueryClientPixmapBytes(self, xid, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", xid))
-        return self.send_request(3, buf, QueryClientPixmapBytesCookie, is_checked=is_checked)
+        return self.send_request(
+            3,
+            buf,
+            QueryClientPixmapBytesCookie,
+            is_checked=is_checked)
+
     def QueryClientIds(self, num_specs, specs, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", num_specs))
         buf.write(xcffib.pack_list(specs, ClientIdSpec))
-        return self.send_request(4, buf, QueryClientIdsCookie, is_checked=is_checked)
+        return self.send_request(
+            4,
+            buf,
+            QueryClientIdsCookie,
+            is_checked=is_checked)
+
     def QueryResourceBytes(self, client, num_specs, specs, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", client, num_specs))
         buf.write(xcffib.pack_list(specs, ResourceIdSpec))
-        return self.send_request(5, buf, QueryResourceBytesCookie, is_checked=is_checked)
+        return self.send_request(
+            5,
+            buf,
+            QueryResourceBytesCookie,
+            is_checked=is_checked)
 xcffib._add_ext(key, resExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/randr.py` & `xcffib-v0.1.4/xcffib/randr.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,92 +4,142 @@
 MAJOR_VERSION = 1
 MINOR_VERSION = 4
 key = xcffib.ExtensionKey("RANDR")
 _events = {}
 _errors = {}
 from . import xproto
 from . import render
+
+
 class Rotation:
     Rotate_0 = 1 << 0
     Rotate_90 = 1 << 1
     Rotate_180 = 1 << 2
     Rotate_270 = 1 << 3
     Reflect_X = 1 << 4
     Reflect_Y = 1 << 5
+
+
 class ScreenSize(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.width, self.height, self.mwidth, self.mheight = unpacker.unpack("HHHH")
+        self.width, self.height, self.mwidth, self.mheight = unpacker.unpack(
+            "HHHH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHHH", self.width, self.height, self.mwidth, self.mheight))
+        buf.write(
+            struct.pack(
+                "=HHHH",
+                self.width,
+                self.height,
+                self.mwidth,
+                self.mheight))
         return buf.getvalue()
     fixed_size = 8
+
+
 class RefreshRates(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.nRates, = unpacker.unpack("H")
         self.rates = xcffib.List(unpacker, "H", self.nRates)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=H", self.nRates))
         buf.write(xcffib.pack_list(self.rates, "H"))
         return buf.getvalue()
+
+
 class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.major_version, self.minor_version = unpacker.unpack("xx2x4xII16x")
         self.bufsize = unpacker.offset - base
+
+
 class QueryVersionCookie(xcffib.Cookie):
     reply_type = QueryVersionReply
+
+
 class SetConfig:
     Success = 0
     InvalidConfigTime = 1
     InvalidTime = 2
     Failed = 3
+
+
 class SetScreenConfigReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.status, self.new_timestamp, self.config_timestamp, self.root, self.subpixel_order = unpacker.unpack("xB2x4xIIIH10x")
+        self.status, self.new_timestamp, self.config_timestamp, self.root, self.subpixel_order = unpacker.unpack(
+            "xB2x4xIIIH10x")
         self.bufsize = unpacker.offset - base
+
+
 class SetScreenConfigCookie(xcffib.Cookie):
     reply_type = SetScreenConfigReply
+
+
 class NotifyMask:
     ScreenChange = 1 << 0
     CrtcChange = 1 << 1
     OutputChange = 1 << 2
     OutputProperty = 1 << 3
     ProviderChange = 1 << 4
     ProviderProperty = 1 << 5
     ResourceChange = 1 << 6
+
+
 class GetScreenInfoReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.rotations, self.root, self.timestamp, self.config_timestamp, self.nSizes, self.sizeID, self.rotation, self.rate, self.nInfo = unpacker.unpack("xB2x4xIIIHHHHH2x")
+        self.rotations, self.root, self.timestamp, self.config_timestamp, self.nSizes, self.sizeID, self.rotation, self.rate, self.nInfo = unpacker.unpack(
+            "xB2x4xIIIHHHHH2x")
         self.sizes = xcffib.List(unpacker, ScreenSize, self.nSizes)
         unpacker.pad(RefreshRates)
-        self.rates = xcffib.List(unpacker, RefreshRates, self.nInfo - self.nSizes)
+        self.rates = xcffib.List(
+            unpacker,
+            RefreshRates,
+            self.nInfo -
+            self.nSizes)
         self.bufsize = unpacker.offset - base
+
+
 class GetScreenInfoCookie(xcffib.Cookie):
     reply_type = GetScreenInfoReply
+
+
 class GetScreenSizeRangeReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.min_width, self.min_height, self.max_width, self.max_height = unpacker.unpack("xx2x4xHHHH16x")
+        self.min_width, self.min_height, self.max_width, self.max_height = unpacker.unpack(
+            "xx2x4xHHHH16x")
         self.bufsize = unpacker.offset - base
+
+
 class GetScreenSizeRangeCookie(xcffib.Cookie):
     reply_type = GetScreenSizeRangeReply
+
+
 class ModeFlag:
     HsyncPositive = 1 << 0
     HsyncNegative = 1 << 1
     VsyncPositive = 1 << 2
     VsyncNegative = 1 << 3
     Interlace = 1 << 4
     DoubleScan = 1 << 5
@@ -97,531 +147,1108 @@
     CsyncPositive = 1 << 7
     CsyncNegative = 1 << 8
     HskewPresent = 1 << 9
     Bcast = 1 << 10
     PixelMultiplex = 1 << 11
     DoubleClock = 1 << 12
     HalveClock = 1 << 13
+
+
 class ModeInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.id, self.width, self.height, self.dot_clock, self.hsync_start, self.hsync_end, self.htotal, self.hskew, self.vsync_start, self.vsync_end, self.vtotal, self.name_len, self.mode_flags = unpacker.unpack("IHHIHHHHHHHHI")
+        self.id, self.width, self.height, self.dot_clock, self.hsync_start, self.hsync_end, self.htotal, self.hskew, self.vsync_start, self.vsync_end, self.vtotal, self.name_len, self.mode_flags = unpacker.unpack(
+            "IHHIHHHHHHHHI")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHHIHHHHHHHHI", self.id, self.width, self.height, self.dot_clock, self.hsync_start, self.hsync_end, self.htotal, self.hskew, self.vsync_start, self.vsync_end, self.vtotal, self.name_len, self.mode_flags))
+        buf.write(
+            struct.pack(
+                "=IHHIHHHHHHHHI",
+                self.id,
+                self.width,
+                self.height,
+                self.dot_clock,
+                self.hsync_start,
+                self.hsync_end,
+                self.htotal,
+                self.hskew,
+                self.vsync_start,
+                self.vsync_end,
+                self.vtotal,
+                self.name_len,
+                self.mode_flags))
         return buf.getvalue()
     fixed_size = 32
+
+
 class GetScreenResourcesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.timestamp, self.config_timestamp, self.num_crtcs, self.num_outputs, self.num_modes, self.names_len = unpacker.unpack("xx2x4xIIHHHH8x")
+        self.timestamp, self.config_timestamp, self.num_crtcs, self.num_outputs, self.num_modes, self.names_len = unpacker.unpack(
+            "xx2x4xIIHHHH8x")
         self.crtcs = xcffib.List(unpacker, "I", self.num_crtcs)
         unpacker.pad("I")
         self.outputs = xcffib.List(unpacker, "I", self.num_outputs)
         unpacker.pad(ModeInfo)
         self.modes = xcffib.List(unpacker, ModeInfo, self.num_modes)
         unpacker.pad("B")
         self.names = xcffib.List(unpacker, "B", self.names_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetScreenResourcesCookie(xcffib.Cookie):
     reply_type = GetScreenResourcesReply
+
+
 class Connection:
     Connected = 0
     Disconnected = 1
     Unknown = 2
+
+
 class GetOutputInfoReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.status, self.timestamp, self.crtc, self.mm_width, self.mm_height, self.connection, self.subpixel_order, self.num_crtcs, self.num_modes, self.num_preferred, self.num_clones, self.name_len = unpacker.unpack("xB2x4xIIIIBBHHHHH")
+        self.status, self.timestamp, self.crtc, self.mm_width, self.mm_height, self.connection, self.subpixel_order, self.num_crtcs, self.num_modes, self.num_preferred, self.num_clones, self.name_len = unpacker.unpack(
+            "xB2x4xIIIIBBHHHHH")
         self.crtcs = xcffib.List(unpacker, "I", self.num_crtcs)
         unpacker.pad("I")
         self.modes = xcffib.List(unpacker, "I", self.num_modes)
         unpacker.pad("I")
         self.clones = xcffib.List(unpacker, "I", self.num_clones)
         unpacker.pad("B")
         self.name = xcffib.List(unpacker, "B", self.name_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetOutputInfoCookie(xcffib.Cookie):
     reply_type = GetOutputInfoReply
+
+
 class ListOutputPropertiesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_atoms, = unpacker.unpack("xx2x4xH22x")
         self.atoms = xcffib.List(unpacker, "I", self.num_atoms)
         self.bufsize = unpacker.offset - base
+
+
 class ListOutputPropertiesCookie(xcffib.Cookie):
     reply_type = ListOutputPropertiesReply
+
+
 class QueryOutputPropertyReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.pending, self.range, self.immutable = unpacker.unpack("xx2x4xBBB21x")
+        self.pending, self.range, self.immutable = unpacker.unpack(
+            "xx2x4xBBB21x")
         self.validValues = xcffib.List(unpacker, "i", self.length)
         self.bufsize = unpacker.offset - base
+
+
 class QueryOutputPropertyCookie(xcffib.Cookie):
     reply_type = QueryOutputPropertyReply
+
+
 class GetOutputPropertyReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.format, self.type, self.bytes_after, self.num_items = unpacker.unpack("xB2x4xIII12x")
-        self.data = xcffib.List(unpacker, "B", self.num_items * (self.format // 8))
+        self.format, self.type, self.bytes_after, self.num_items = unpacker.unpack(
+            "xB2x4xIII12x")
+        self.data = xcffib.List(
+            unpacker, "B", self.num_items * (self.format // 8))
         self.bufsize = unpacker.offset - base
+
+
 class GetOutputPropertyCookie(xcffib.Cookie):
     reply_type = GetOutputPropertyReply
+
+
 class CreateModeReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.mode, = unpacker.unpack("xx2x4xI20x")
         self.bufsize = unpacker.offset - base
+
+
 class CreateModeCookie(xcffib.Cookie):
     reply_type = CreateModeReply
+
+
 class GetCrtcInfoReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.status, self.timestamp, self.x, self.y, self.width, self.height, self.mode, self.rotation, self.rotations, self.num_outputs, self.num_possible_outputs = unpacker.unpack("xB2x4xIhhHHIHHHH")
+        self.status, self.timestamp, self.x, self.y, self.width, self.height, self.mode, self.rotation, self.rotations, self.num_outputs, self.num_possible_outputs = unpacker.unpack(
+            "xB2x4xIhhHHIHHHH")
         self.outputs = xcffib.List(unpacker, "I", self.num_outputs)
         unpacker.pad("I")
         self.possible = xcffib.List(unpacker, "I", self.num_possible_outputs)
         self.bufsize = unpacker.offset - base
+
+
 class GetCrtcInfoCookie(xcffib.Cookie):
     reply_type = GetCrtcInfoReply
+
+
 class SetCrtcConfigReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, self.timestamp = unpacker.unpack("xB2x4xI20x")
         self.bufsize = unpacker.offset - base
+
+
 class SetCrtcConfigCookie(xcffib.Cookie):
     reply_type = SetCrtcConfigReply
+
+
 class GetCrtcGammaSizeReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.size, = unpacker.unpack("xx2x4xH22x")
         self.bufsize = unpacker.offset - base
+
+
 class GetCrtcGammaSizeCookie(xcffib.Cookie):
     reply_type = GetCrtcGammaSizeReply
+
+
 class GetCrtcGammaReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.size, = unpacker.unpack("xx2x4xH22x")
         self.red = xcffib.List(unpacker, "H", self.size)
         unpacker.pad("H")
         self.green = xcffib.List(unpacker, "H", self.size)
         unpacker.pad("H")
         self.blue = xcffib.List(unpacker, "H", self.size)
         self.bufsize = unpacker.offset - base
+
+
 class GetCrtcGammaCookie(xcffib.Cookie):
     reply_type = GetCrtcGammaReply
+
+
 class GetScreenResourcesCurrentReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.timestamp, self.config_timestamp, self.num_crtcs, self.num_outputs, self.num_modes, self.names_len = unpacker.unpack("xx2x4xIIHHHH8x")
+        self.timestamp, self.config_timestamp, self.num_crtcs, self.num_outputs, self.num_modes, self.names_len = unpacker.unpack(
+            "xx2x4xIIHHHH8x")
         self.crtcs = xcffib.List(unpacker, "I", self.num_crtcs)
         unpacker.pad("I")
         self.outputs = xcffib.List(unpacker, "I", self.num_outputs)
         unpacker.pad(ModeInfo)
         self.modes = xcffib.List(unpacker, ModeInfo, self.num_modes)
         unpacker.pad("B")
         self.names = xcffib.List(unpacker, "B", self.names_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetScreenResourcesCurrentCookie(xcffib.Cookie):
     reply_type = GetScreenResourcesCurrentReply
+
+
 class Transform:
     Unit = 1 << 0
     ScaleUp = 1 << 1
     ScaleDown = 1 << 2
     Projective = 1 << 3
+
+
 class GetCrtcTransformReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x")
         self.pending_transform = render.TRANSFORM(unpacker)
         self.has_transforms, = unpacker.unpack("B3x")
         unpacker.pad(render.TRANSFORM)
         self.current_transform = render.TRANSFORM(unpacker)
-        self.pending_len, self.pending_nparams, self.current_len, self.current_nparams = unpacker.unpack("4xHHHH")
+        self.pending_len, self.pending_nparams, self.current_len, self.current_nparams = unpacker.unpack(
+            "4xHHHH")
         unpacker.pad("c")
         self.pending_filter_name = xcffib.List(unpacker, "c", self.pending_len)
         unpacker.pad("i")
         self.pending_params = xcffib.List(unpacker, "i", self.pending_nparams)
         unpacker.pad("c")
         self.current_filter_name = xcffib.List(unpacker, "c", self.current_len)
         unpacker.pad("i")
         self.current_params = xcffib.List(unpacker, "i", self.current_nparams)
         self.bufsize = unpacker.offset - base
+
+
 class GetCrtcTransformCookie(xcffib.Cookie):
     reply_type = GetCrtcTransformReply
+
+
 class GetPanningReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.status, self.timestamp, self.left, self.top, self.width, self.height, self.track_left, self.track_top, self.track_width, self.track_height, self.border_left, self.border_top, self.border_right, self.border_bottom = unpacker.unpack("xB2x4xIHHHHHHHHhhhh")
+        self.status, self.timestamp, self.left, self.top, self.width, self.height, self.track_left, self.track_top, self.track_width, self.track_height, self.border_left, self.border_top, self.border_right, self.border_bottom = unpacker.unpack(
+            "xB2x4xIHHHHHHHHhhhh")
         self.bufsize = unpacker.offset - base
+
+
 class GetPanningCookie(xcffib.Cookie):
     reply_type = GetPanningReply
+
+
 class SetPanningReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, self.timestamp = unpacker.unpack("xB2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class SetPanningCookie(xcffib.Cookie):
     reply_type = SetPanningReply
+
+
 class GetOutputPrimaryReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.output, = unpacker.unpack("xx2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class GetOutputPrimaryCookie(xcffib.Cookie):
     reply_type = GetOutputPrimaryReply
+
+
 class GetProvidersReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.timestamp, self.num_providers = unpacker.unpack("xx2x4xIH18x")
         self.providers = xcffib.List(unpacker, "I", self.num_providers)
         self.bufsize = unpacker.offset - base
+
+
 class GetProvidersCookie(xcffib.Cookie):
     reply_type = GetProvidersReply
+
+
 class ProviderCapability:
     SourceOutput = 1 << 0
     SinkOutput = 1 << 1
     SourceOffload = 1 << 2
     SinkOffload = 1 << 3
+
+
 class GetProviderInfoReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.status, self.timestamp, self.capabilities, self.num_crtcs, self.num_outputs, self.num_associated_providers, self.name_len = unpacker.unpack("xB2x4xIIHHHH8x")
+        self.status, self.timestamp, self.capabilities, self.num_crtcs, self.num_outputs, self.num_associated_providers, self.name_len = unpacker.unpack(
+            "xB2x4xIIHHHH8x")
         self.crtcs = xcffib.List(unpacker, "I", self.num_crtcs)
         unpacker.pad("I")
         self.outputs = xcffib.List(unpacker, "I", self.num_outputs)
         unpacker.pad("I")
-        self.associated_providers = xcffib.List(unpacker, "I", self.num_associated_providers)
+        self.associated_providers = xcffib.List(
+            unpacker,
+            "I",
+            self.num_associated_providers)
         unpacker.pad("I")
-        self.associated_capability = xcffib.List(unpacker, "I", self.num_associated_providers)
+        self.associated_capability = xcffib.List(
+            unpacker,
+            "I",
+            self.num_associated_providers)
         unpacker.pad("c")
         self.name = xcffib.List(unpacker, "c", self.name_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetProviderInfoCookie(xcffib.Cookie):
     reply_type = GetProviderInfoReply
+
+
 class ListProviderPropertiesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_atoms, = unpacker.unpack("xx2x4xH22x")
         self.atoms = xcffib.List(unpacker, "I", self.num_atoms)
         self.bufsize = unpacker.offset - base
+
+
 class ListProviderPropertiesCookie(xcffib.Cookie):
     reply_type = ListProviderPropertiesReply
+
+
 class QueryProviderPropertyReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.pending, self.range, self.immutable = unpacker.unpack("xx2x4xBBB21x")
+        self.pending, self.range, self.immutable = unpacker.unpack(
+            "xx2x4xBBB21x")
         self.valid_values = xcffib.List(unpacker, "i", self.length)
         self.bufsize = unpacker.offset - base
+
+
 class QueryProviderPropertyCookie(xcffib.Cookie):
     reply_type = QueryProviderPropertyReply
+
+
 class GetProviderPropertyReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.format, self.type, self.bytes_after, self.num_items = unpacker.unpack("xB2x4xIII12x")
-        self.data = xcffib.List(unpacker, "c", self.num_items * (self.format // 8))
+        self.format, self.type, self.bytes_after, self.num_items = unpacker.unpack(
+            "xB2x4xIII12x")
+        self.data = xcffib.List(
+            unpacker, "c", self.num_items * (self.format // 8))
         self.bufsize = unpacker.offset - base
+
+
 class GetProviderPropertyCookie(xcffib.Cookie):
     reply_type = GetProviderPropertyReply
+
+
 class ScreenChangeNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.rotation, self.timestamp, self.config_timestamp, self.root, self.request_window, self.sizeID, self.subpixel_order, self.width, self.height, self.mwidth, self.mheight = unpacker.unpack("xB2xIIIIHHHHHH")
+        self.rotation, self.timestamp, self.config_timestamp, self.root, self.request_window, self.sizeID, self.subpixel_order, self.width, self.height, self.mwidth, self.mheight = unpacker.unpack(
+            "xB2xIIIIHHHHHH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIIHHHHHH", self.rotation, self.timestamp, self.config_timestamp, self.root, self.request_window, self.sizeID, self.subpixel_order, self.width, self.height, self.mwidth, self.mheight))
+        buf.write(
+            struct.pack(
+                "=BIIIIHHHHHH",
+                self.rotation,
+                self.timestamp,
+                self.config_timestamp,
+                self.root,
+                self.request_window,
+                self.sizeID,
+                self.subpixel_order,
+                self.width,
+                self.height,
+                self.mwidth,
+                self.mheight))
         return buf.getvalue()
 _events[0] = ScreenChangeNotifyEvent
+
+
 class Notify:
     CrtcChange = 0
     OutputChange = 1
     OutputProperty = 2
     ProviderChange = 3
     ProviderProperty = 4
     ResourceChange = 5
+
+
 class CrtcChange(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.timestamp, self.window, self.crtc, self.mode, self.rotation, self.x, self.y, self.width, self.height = unpacker.unpack("IIIIH2xhhHH")
+        self.timestamp, self.window, self.crtc, self.mode, self.rotation, self.x, self.y, self.width, self.height = unpacker.unpack(
+            "IIIIH2xhhHH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IIIIH2xhhHH", self.timestamp, self.window, self.crtc, self.mode, self.rotation, self.x, self.y, self.width, self.height))
+        buf.write(
+            struct.pack(
+                "=IIIIH2xhhHH",
+                self.timestamp,
+                self.window,
+                self.crtc,
+                self.mode,
+                self.rotation,
+                self.x,
+                self.y,
+                self.width,
+                self.height))
         return buf.getvalue()
     fixed_size = 28
+
+
 class OutputChange(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.timestamp, self.config_timestamp, self.window, self.output, self.crtc, self.mode, self.rotation, self.connection, self.subpixel_order = unpacker.unpack("IIIIIIHBB")
+        self.timestamp, self.config_timestamp, self.window, self.output, self.crtc, self.mode, self.rotation, self.connection, self.subpixel_order = unpacker.unpack(
+            "IIIIIIHBB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IIIIIIHBB", self.timestamp, self.config_timestamp, self.window, self.output, self.crtc, self.mode, self.rotation, self.connection, self.subpixel_order))
+        buf.write(
+            struct.pack(
+                "=IIIIIIHBB",
+                self.timestamp,
+                self.config_timestamp,
+                self.window,
+                self.output,
+                self.crtc,
+                self.mode,
+                self.rotation,
+                self.connection,
+                self.subpixel_order))
         return buf.getvalue()
     fixed_size = 28
+
+
 class OutputProperty(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.window, self.output, self.atom, self.timestamp, self.status = unpacker.unpack("IIIIB11x")
+        self.window, self.output, self.atom, self.timestamp, self.status = unpacker.unpack(
+            "IIIIB11x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IIIIB11x", self.window, self.output, self.atom, self.timestamp, self.status))
+        buf.write(
+            struct.pack(
+                "=IIIIB11x",
+                self.window,
+                self.output,
+                self.atom,
+                self.timestamp,
+                self.status))
         return buf.getvalue()
     fixed_size = 28
+
+
 class ProviderChange(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.timestamp, self.window, self.provider = unpacker.unpack("III16x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=III16x", self.timestamp, self.window, self.provider))
+        buf.write(
+            struct.pack(
+                "=III16x",
+                self.timestamp,
+                self.window,
+                self.provider))
         return buf.getvalue()
     fixed_size = 28
+
+
 class ProviderProperty(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.window, self.provider, self.atom, self.timestamp, self.state = unpacker.unpack("IIIIB11x")
+        self.window, self.provider, self.atom, self.timestamp, self.state = unpacker.unpack(
+            "IIIIB11x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IIIIB11x", self.window, self.provider, self.atom, self.timestamp, self.state))
+        buf.write(
+            struct.pack(
+                "=IIIIB11x",
+                self.window,
+                self.provider,
+                self.atom,
+                self.timestamp,
+                self.state))
         return buf.getvalue()
     fixed_size = 28
+
+
 class ResourceChange(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.timestamp, self.window = unpacker.unpack("II20x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=II20x", self.timestamp, self.window))
         return buf.getvalue()
     fixed_size = 28
+
+
 class NotifyData(xcffib.Union):
+
     def __init__(self, unpacker):
         xcffib.Union.__init__(self, unpacker)
-        self.cc = CrtcChange(unpacker)
-        self.oc = OutputChange(unpacker)
-        self.op = OutputProperty(unpacker)
-        self.pc = ProviderChange(unpacker)
-        self.pp = ProviderProperty(unpacker)
-        self.rc = ResourceChange(unpacker)
+        self.cc = CrtcChange(unpacker.copy())
+        self.oc = OutputChange(unpacker.copy())
+        self.op = OutputProperty(unpacker.copy())
+        self.pc = ProviderChange(unpacker.copy())
+        self.pp = ProviderProperty(unpacker.copy())
+        self.rc = ResourceChange(unpacker.copy())
+
+
 class NotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         self.subCode, = unpacker.unpack("xB2x")
         self.u = NotifyData(unpacker)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=B", self.subCode))
         buf.write(self.u.pack())
         return buf.getvalue()
 _events[1] = NotifyEvent
+
+
 class randrExtension(xcffib.Extension):
+
     def QueryVersion(self, major_version, minor_version, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", major_version, minor_version))
-        return self.send_request(0, buf, QueryVersionCookie, is_checked=is_checked)
-    def SetScreenConfig(self, window, timestamp, config_timestamp, sizeID, rotation, rate, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIHHH2x", window, timestamp, config_timestamp, sizeID, rotation, rate))
-        return self.send_request(2, buf, SetScreenConfigCookie, is_checked=is_checked)
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
+    def SetScreenConfig(
+            self,
+            window,
+            timestamp,
+            config_timestamp,
+            sizeID,
+            rotation,
+            rate,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIHHH2x",
+                window,
+                timestamp,
+                config_timestamp,
+                sizeID,
+                rotation,
+                rate))
+        return self.send_request(
+            2,
+            buf,
+            SetScreenConfigCookie,
+            is_checked=is_checked)
+
     def SelectInput(self, window, enable, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIH2x", window, enable))
         return self.send_request(4, buf, is_checked=is_checked)
+
     def GetScreenInfo(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(5, buf, GetScreenInfoCookie, is_checked=is_checked)
+        return self.send_request(
+            5,
+            buf,
+            GetScreenInfoCookie,
+            is_checked=is_checked)
+
     def GetScreenSizeRange(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(6, buf, GetScreenSizeRangeCookie, is_checked=is_checked)
-    def SetScreenSize(self, window, width, height, mm_width, mm_height, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIHHII", window, width, height, mm_width, mm_height))
+        return self.send_request(
+            6,
+            buf,
+            GetScreenSizeRangeCookie,
+            is_checked=is_checked)
+
+    def SetScreenSize(
+            self,
+            window,
+            width,
+            height,
+            mm_width,
+            mm_height,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIHHII",
+                window,
+                width,
+                height,
+                mm_width,
+                mm_height))
         return self.send_request(7, buf, is_checked=is_checked)
+
     def GetScreenResources(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(8, buf, GetScreenResourcesCookie, is_checked=is_checked)
+        return self.send_request(
+            8,
+            buf,
+            GetScreenResourcesCookie,
+            is_checked=is_checked)
+
     def GetOutputInfo(self, output, config_timestamp, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", output, config_timestamp))
-        return self.send_request(9, buf, GetOutputInfoCookie, is_checked=is_checked)
+        return self.send_request(
+            9,
+            buf,
+            GetOutputInfoCookie,
+            is_checked=is_checked)
+
     def ListOutputProperties(self, output, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", output))
-        return self.send_request(10, buf, ListOutputPropertiesCookie, is_checked=is_checked)
+        return self.send_request(
+            10,
+            buf,
+            ListOutputPropertiesCookie,
+            is_checked=is_checked)
+
     def QueryOutputProperty(self, output, property, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", output, property))
-        return self.send_request(11, buf, QueryOutputPropertyCookie, is_checked=is_checked)
-    def ConfigureOutputProperty(self, output, property, pending, range, values, is_checked=False):
+        return self.send_request(
+            11,
+            buf,
+            QueryOutputPropertyCookie,
+            is_checked=is_checked)
+
+    def ConfigureOutputProperty(
+            self,
+            output,
+            property,
+            pending,
+            range,
+            values,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIBB2x", output, property, pending, range))
         buf.write(xcffib.pack_list(values, "i"))
         return self.send_request(12, buf, is_checked=is_checked)
-    def ChangeOutputProperty(self, output, property, type, format, mode, num_units, data, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIBB2xI", output, property, type, format, mode, num_units))
+
+    def ChangeOutputProperty(
+            self,
+            output,
+            property,
+            type,
+            format,
+            mode,
+            num_units,
+            data,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIBB2xI",
+                output,
+                property,
+                type,
+                format,
+                mode,
+                num_units))
         buf.write(xcffib.pack_list(data, "c"))
         return self.send_request(13, buf, is_checked=is_checked)
+
     def DeleteOutputProperty(self, output, property, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", output, property))
         return self.send_request(14, buf, is_checked=is_checked)
-    def GetOutputProperty(self, output, property, type, long_offset, long_length, delete, pending, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIIIBB2x", output, property, type, long_offset, long_length, delete, pending))
-        return self.send_request(15, buf, GetOutputPropertyCookie, is_checked=is_checked)
+
+    def GetOutputProperty(
+            self,
+            output,
+            property,
+            type,
+            long_offset,
+            long_length,
+            delete,
+            pending,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIIIBB2x",
+                output,
+                property,
+                type,
+                long_offset,
+                long_length,
+                delete,
+                pending))
+        return self.send_request(
+            15,
+            buf,
+            GetOutputPropertyCookie,
+            is_checked=is_checked)
+
     def CreateMode(self, window, mode_info, name, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
         buf.write(mode_info.pack())
         buf.write(xcffib.pack_list(name, "c"))
-        return self.send_request(16, buf, CreateModeCookie, is_checked=is_checked)
+        return self.send_request(
+            16,
+            buf,
+            CreateModeCookie,
+            is_checked=is_checked)
+
     def DestroyMode(self, mode, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", mode))
         return self.send_request(17, buf, is_checked=is_checked)
+
     def AddOutputMode(self, output, mode, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", output, mode))
         return self.send_request(18, buf, is_checked=is_checked)
+
     def DeleteOutputMode(self, output, mode, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", output, mode))
         return self.send_request(19, buf, is_checked=is_checked)
+
     def GetCrtcInfo(self, crtc, config_timestamp, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", crtc, config_timestamp))
-        return self.send_request(20, buf, GetCrtcInfoCookie, is_checked=is_checked)
-    def SetCrtcConfig(self, crtc, timestamp, config_timestamp, x, y, mode, rotation, outputs, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIhhIH2x", crtc, timestamp, config_timestamp, x, y, mode, rotation))
+        return self.send_request(
+            20,
+            buf,
+            GetCrtcInfoCookie,
+            is_checked=is_checked)
+
+    def SetCrtcConfig(
+            self,
+            crtc,
+            timestamp,
+            config_timestamp,
+            x,
+            y,
+            mode,
+            rotation,
+            outputs,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIhhIH2x",
+                crtc,
+                timestamp,
+                config_timestamp,
+                x,
+                y,
+                mode,
+                rotation))
         buf.write(xcffib.pack_list(outputs, "I"))
-        return self.send_request(21, buf, SetCrtcConfigCookie, is_checked=is_checked)
+        return self.send_request(
+            21,
+            buf,
+            SetCrtcConfigCookie,
+            is_checked=is_checked)
+
     def GetCrtcGammaSize(self, crtc, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", crtc))
-        return self.send_request(22, buf, GetCrtcGammaSizeCookie, is_checked=is_checked)
+        return self.send_request(
+            22,
+            buf,
+            GetCrtcGammaSizeCookie,
+            is_checked=is_checked)
+
     def GetCrtcGamma(self, crtc, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", crtc))
-        return self.send_request(23, buf, GetCrtcGammaCookie, is_checked=is_checked)
+        return self.send_request(
+            23,
+            buf,
+            GetCrtcGammaCookie,
+            is_checked=is_checked)
+
     def SetCrtcGamma(self, crtc, size, red, green, blue, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIH2x", crtc, size))
         buf.write(xcffib.pack_list(red, "H"))
         buf.write(xcffib.pack_list(green, "H"))
         buf.write(xcffib.pack_list(blue, "H"))
         return self.send_request(24, buf, is_checked=is_checked)
+
     def GetScreenResourcesCurrent(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(25, buf, GetScreenResourcesCurrentCookie, is_checked=is_checked)
-    def SetCrtcTransform(self, crtc, filter_len, transform, filter_name, filter_params, is_checked=False):
+        return self.send_request(
+            25,
+            buf,
+            GetScreenResourcesCurrentCookie,
+            is_checked=is_checked)
+
+    def SetCrtcTransform(
+            self,
+            crtc,
+            filter_len,
+            transform,
+            filter_name,
+            filter_params,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIH2x", crtc, filter_len))
         buf.write(transform.pack())
         buf.write(xcffib.pack_list(filter_name, "c"))
         buf.write(xcffib.pack_list(filter_params, "i"))
         return self.send_request(26, buf, is_checked=is_checked)
+
     def GetCrtcTransform(self, crtc, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", crtc))
-        return self.send_request(27, buf, GetCrtcTransformCookie, is_checked=is_checked)
+        return self.send_request(
+            27,
+            buf,
+            GetCrtcTransformCookie,
+            is_checked=is_checked)
+
     def GetPanning(self, crtc, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", crtc))
-        return self.send_request(28, buf, GetPanningCookie, is_checked=is_checked)
-    def SetPanning(self, crtc, timestamp, left, top, width, height, track_left, track_top, track_width, track_height, border_left, border_top, border_right, border_bottom, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIHHHHHHHHhhhh", crtc, timestamp, left, top, width, height, track_left, track_top, track_width, track_height, border_left, border_top, border_right, border_bottom))
-        return self.send_request(29, buf, SetPanningCookie, is_checked=is_checked)
+        return self.send_request(
+            28,
+            buf,
+            GetPanningCookie,
+            is_checked=is_checked)
+
+    def SetPanning(
+            self,
+            crtc,
+            timestamp,
+            left,
+            top,
+            width,
+            height,
+            track_left,
+            track_top,
+            track_width,
+            track_height,
+            border_left,
+            border_top,
+            border_right,
+            border_bottom,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIHHHHHHHHhhhh",
+                crtc,
+                timestamp,
+                left,
+                top,
+                width,
+                height,
+                track_left,
+                track_top,
+                track_width,
+                track_height,
+                border_left,
+                border_top,
+                border_right,
+                border_bottom))
+        return self.send_request(
+            29,
+            buf,
+            SetPanningCookie,
+            is_checked=is_checked)
+
     def SetOutputPrimary(self, window, output, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", window, output))
         return self.send_request(30, buf, is_checked=is_checked)
+
     def GetOutputPrimary(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(31, buf, GetOutputPrimaryCookie, is_checked=is_checked)
+        return self.send_request(
+            31,
+            buf,
+            GetOutputPrimaryCookie,
+            is_checked=is_checked)
+
     def GetProviders(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(32, buf, GetProvidersCookie, is_checked=is_checked)
+        return self.send_request(
+            32,
+            buf,
+            GetProvidersCookie,
+            is_checked=is_checked)
+
     def GetProviderInfo(self, provider, config_timestamp, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", provider, config_timestamp))
-        return self.send_request(33, buf, GetProviderInfoCookie, is_checked=is_checked)
-    def SetProviderOffloadSink(self, provider, sink_provider, config_timestamp, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIII", provider, sink_provider, config_timestamp))
+        return self.send_request(
+            33,
+            buf,
+            GetProviderInfoCookie,
+            is_checked=is_checked)
+
+    def SetProviderOffloadSink(
+            self,
+            provider,
+            sink_provider,
+            config_timestamp,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIII",
+                provider,
+                sink_provider,
+                config_timestamp))
         return self.send_request(34, buf, is_checked=is_checked)
-    def SetProviderOutputSource(self, provider, source_provider, config_timestamp, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIII", provider, source_provider, config_timestamp))
+
+    def SetProviderOutputSource(
+            self,
+            provider,
+            source_provider,
+            config_timestamp,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIII",
+                provider,
+                source_provider,
+                config_timestamp))
         return self.send_request(35, buf, is_checked=is_checked)
+
     def ListProviderProperties(self, provider, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", provider))
-        return self.send_request(36, buf, ListProviderPropertiesCookie, is_checked=is_checked)
+        return self.send_request(
+            36,
+            buf,
+            ListProviderPropertiesCookie,
+            is_checked=is_checked)
+
     def QueryProviderProperty(self, provider, property, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", provider, property))
-        return self.send_request(37, buf, QueryProviderPropertyCookie, is_checked=is_checked)
-    def ConfigureProviderProperty(self, provider, property, pending, range, values, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIBB2x", provider, property, pending, range))
+        return self.send_request(
+            37,
+            buf,
+            QueryProviderPropertyCookie,
+            is_checked=is_checked)
+
+    def ConfigureProviderProperty(
+            self,
+            provider,
+            property,
+            pending,
+            range,
+            values,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIBB2x",
+                provider,
+                property,
+                pending,
+                range))
         buf.write(xcffib.pack_list(values, "i"))
         return self.send_request(38, buf, is_checked=is_checked)
-    def ChangeProviderProperty(self, provider, property, type, format, mode, num_items, data, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIBB2xI", provider, property, type, format, mode, num_items))
+
+    def ChangeProviderProperty(
+            self,
+            provider,
+            property,
+            type,
+            format,
+            mode,
+            num_items,
+            data,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIBB2xI",
+                provider,
+                property,
+                type,
+                format,
+                mode,
+                num_items))
         buf.write(xcffib.pack_list(data, "c"))
         return self.send_request(39, buf, is_checked=is_checked)
+
     def DeleteProviderProperty(self, provider, property, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", provider, property))
         return self.send_request(40, buf, is_checked=is_checked)
-    def GetProviderProperty(self, provider, property, type, long_offset, long_length, delete, pending, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIIIBB2x", provider, property, type, long_offset, long_length, delete, pending))
-        return self.send_request(41, buf, GetProviderPropertyCookie, is_checked=is_checked)
+
+    def GetProviderProperty(
+            self,
+            provider,
+            property,
+            type,
+            long_offset,
+            long_length,
+            delete,
+            pending,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIIIBB2x",
+                provider,
+                property,
+                type,
+                long_offset,
+                long_length,
+                delete,
+                pending))
+        return self.send_request(
+            41,
+            buf,
+            GetProviderPropertyCookie,
+            is_checked=is_checked)
 xcffib._add_ext(key, randrExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/xf86dri.py` & `xcffib-v0.1.4/xcffib/xf86dri.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,146 +2,262 @@
 import struct
 import six
 MAJOR_VERSION = 4
 MINOR_VERSION = 1
 key = xcffib.ExtensionKey("XFree86-DRI")
 _events = {}
 _errors = {}
+
+
 class DrmClipRect(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.x1, self.y1, self.x2, self.x3 = unpacker.unpack("hhhh")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=hhhh", self.x1, self.y1, self.x2, self.x3))
         return buf.getvalue()
     fixed_size = 8
+
+
 class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.dri_major_version, self.dri_minor_version, self.dri_minor_patch = unpacker.unpack("xx2x4xHHI")
+        self.dri_major_version, self.dri_minor_version, self.dri_minor_patch = unpacker.unpack(
+            "xx2x4xHHI")
         self.bufsize = unpacker.offset - base
+
+
 class QueryVersionCookie(xcffib.Cookie):
     reply_type = QueryVersionReply
+
+
 class QueryDirectRenderingCapableReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.is_capable, = unpacker.unpack("xx2x4xB")
         self.bufsize = unpacker.offset - base
+
+
 class QueryDirectRenderingCapableCookie(xcffib.Cookie):
     reply_type = QueryDirectRenderingCapableReply
+
+
 class OpenConnectionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.sarea_handle_low, self.sarea_handle_high, self.bus_id_len = unpacker.unpack("xx2x4xIII12x")
+        self.sarea_handle_low, self.sarea_handle_high, self.bus_id_len = unpacker.unpack(
+            "xx2x4xIII12x")
         self.bus_id = xcffib.List(unpacker, "c", self.bus_id_len)
         self.bufsize = unpacker.offset - base
+
+
 class OpenConnectionCookie(xcffib.Cookie):
     reply_type = OpenConnectionReply
+
+
 class GetClientDriverNameReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.client_driver_major_version, self.client_driver_minor_version, self.client_driver_patch_version, self.client_driver_name_len = unpacker.unpack("xx2x4xIIII8x")
-        self.client_driver_name = xcffib.List(unpacker, "c", self.client_driver_name_len)
+        self.client_driver_major_version, self.client_driver_minor_version, self.client_driver_patch_version, self.client_driver_name_len = unpacker.unpack(
+            "xx2x4xIIII8x")
+        self.client_driver_name = xcffib.List(
+            unpacker,
+            "c",
+            self.client_driver_name_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetClientDriverNameCookie(xcffib.Cookie):
     reply_type = GetClientDriverNameReply
+
+
 class CreateContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.hw_context, = unpacker.unpack("xx2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class CreateContextCookie(xcffib.Cookie):
     reply_type = CreateContextReply
+
+
 class CreateDrawableReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.hw_drawable_handle, = unpacker.unpack("xx2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class CreateDrawableCookie(xcffib.Cookie):
     reply_type = CreateDrawableReply
+
+
 class GetDrawableInfoReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.drawable_table_index, self.drawable_table_stamp, self.drawable_origin_X, self.drawable_origin_Y, self.drawable_size_W, self.drawable_size_H, self.num_clip_rects, self.back_x, self.back_y, self.num_back_clip_rects = unpacker.unpack("xx2x4xIIhhhhIhhI")
-        self.clip_rects = xcffib.List(unpacker, DrmClipRect, self.num_clip_rects)
+        self.drawable_table_index, self.drawable_table_stamp, self.drawable_origin_X, self.drawable_origin_Y, self.drawable_size_W, self.drawable_size_H, self.num_clip_rects, self.back_x, self.back_y, self.num_back_clip_rects = unpacker.unpack(
+            "xx2x4xIIhhhhIhhI")
+        self.clip_rects = xcffib.List(
+            unpacker,
+            DrmClipRect,
+            self.num_clip_rects)
         unpacker.pad(DrmClipRect)
-        self.back_clip_rects = xcffib.List(unpacker, DrmClipRect, self.num_back_clip_rects)
+        self.back_clip_rects = xcffib.List(
+            unpacker,
+            DrmClipRect,
+            self.num_back_clip_rects)
         self.bufsize = unpacker.offset - base
+
+
 class GetDrawableInfoCookie(xcffib.Cookie):
     reply_type = GetDrawableInfoReply
+
+
 class GetDeviceInfoReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.framebuffer_handle_low, self.framebuffer_handle_high, self.framebuffer_origin_offset, self.framebuffer_size, self.framebuffer_stride, self.device_private_size = unpacker.unpack("xx2x4xIIIIII")
-        self.device_private = xcffib.List(unpacker, "I", self.device_private_size)
+        self.framebuffer_handle_low, self.framebuffer_handle_high, self.framebuffer_origin_offset, self.framebuffer_size, self.framebuffer_stride, self.device_private_size = unpacker.unpack(
+            "xx2x4xIIIIII")
+        self.device_private = xcffib.List(
+            unpacker,
+            "I",
+            self.device_private_size)
         self.bufsize = unpacker.offset - base
+
+
 class GetDeviceInfoCookie(xcffib.Cookie):
     reply_type = GetDeviceInfoReply
+
+
 class AuthConnectionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.authenticated, = unpacker.unpack("xx2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class AuthConnectionCookie(xcffib.Cookie):
     reply_type = AuthConnectionReply
+
+
 class xf86driExtension(xcffib.Extension):
+
     def QueryVersion(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(0, buf, QueryVersionCookie, is_checked=is_checked)
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
     def QueryDirectRenderingCapable(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", screen))
-        return self.send_request(1, buf, QueryDirectRenderingCapableCookie, is_checked=is_checked)
+        return self.send_request(
+            1,
+            buf,
+            QueryDirectRenderingCapableCookie,
+            is_checked=is_checked)
+
     def OpenConnection(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", screen))
-        return self.send_request(2, buf, OpenConnectionCookie, is_checked=is_checked)
+        return self.send_request(
+            2,
+            buf,
+            OpenConnectionCookie,
+            is_checked=is_checked)
+
     def CloseConnection(self, screen, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", screen))
         return self.send_request(3, buf, is_checked=is_checked)
+
     def GetClientDriverName(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", screen))
-        return self.send_request(4, buf, GetClientDriverNameCookie, is_checked=is_checked)
+        return self.send_request(
+            4,
+            buf,
+            GetClientDriverNameCookie,
+            is_checked=is_checked)
+
     def CreateContext(self, screen, visual, context, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", screen, visual, context))
-        return self.send_request(5, buf, CreateContextCookie, is_checked=is_checked)
+        return self.send_request(
+            5,
+            buf,
+            CreateContextCookie,
+            is_checked=is_checked)
+
     def DestroyContext(self, screen, context, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", screen, context))
         return self.send_request(6, buf, is_checked=is_checked)
+
     def CreateDrawable(self, screen, drawable, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", screen, drawable))
-        return self.send_request(7, buf, CreateDrawableCookie, is_checked=is_checked)
+        return self.send_request(
+            7,
+            buf,
+            CreateDrawableCookie,
+            is_checked=is_checked)
+
     def DestroyDrawable(self, screen, drawable, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", screen, drawable))
         return self.send_request(8, buf, is_checked=is_checked)
+
     def GetDrawableInfo(self, screen, drawable, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", screen, drawable))
-        return self.send_request(9, buf, GetDrawableInfoCookie, is_checked=is_checked)
+        return self.send_request(
+            9,
+            buf,
+            GetDrawableInfoCookie,
+            is_checked=is_checked)
+
     def GetDeviceInfo(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", screen))
-        return self.send_request(10, buf, GetDeviceInfoCookie, is_checked=is_checked)
+        return self.send_request(
+            10,
+            buf,
+            GetDeviceInfoCookie,
+            is_checked=is_checked)
+
     def AuthConnection(self, screen, magic, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", screen, magic))
-        return self.send_request(11, buf, AuthConnectionCookie, is_checked=is_checked)
+        return self.send_request(
+            11,
+            buf,
+            AuthConnectionCookie,
+            is_checked=is_checked)
 xcffib._add_ext(key, xf86driExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/xproto.py` & `xcffib-v0.1.4/xcffib/xproto.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,160 @@
 import xcffib
 import struct
 import six
 _events = {}
 _errors = {}
+
+
 class CHAR2B(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.byte1, self.byte2 = unpacker.unpack("BB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=BB", self.byte1, self.byte2))
         return buf.getvalue()
     fixed_size = 2
+
+
 class POINT(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.x, self.y = unpacker.unpack("hh")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=hh", self.x, self.y))
         return buf.getvalue()
     fixed_size = 4
+
+
 class RECTANGLE(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.x, self.y, self.width, self.height = unpacker.unpack("hhHH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=hhHH", self.x, self.y, self.width, self.height))
+        buf.write(
+            struct.pack(
+                "=hhHH",
+                self.x,
+                self.y,
+                self.width,
+                self.height))
         return buf.getvalue()
     fixed_size = 8
+
+
 class ARC(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.x, self.y, self.width, self.height, self.angle1, self.angle2 = unpacker.unpack("hhHHhh")
+        self.x, self.y, self.width, self.height, self.angle1, self.angle2 = unpacker.unpack(
+            "hhHHhh")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=hhHHhh", self.x, self.y, self.width, self.height, self.angle1, self.angle2))
+        buf.write(
+            struct.pack(
+                "=hhHHhh",
+                self.x,
+                self.y,
+                self.width,
+                self.height,
+                self.angle1,
+                self.angle2))
         return buf.getvalue()
     fixed_size = 12
+
+
 class FORMAT(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.depth, self.bits_per_pixel, self.scanline_pad = unpacker.unpack("BBB5x")
+        self.depth, self.bits_per_pixel, self.scanline_pad = unpacker.unpack(
+            "BBB5x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBB5x", self.depth, self.bits_per_pixel, self.scanline_pad))
+        buf.write(
+            struct.pack(
+                "=BBB5x",
+                self.depth,
+                self.bits_per_pixel,
+                self.scanline_pad))
         return buf.getvalue()
     fixed_size = 8
+
+
 class VisualClass:
     StaticGray = 0
     GrayScale = 1
     StaticColor = 2
     PseudoColor = 3
     TrueColor = 4
     DirectColor = 5
+
+
 class VISUALTYPE(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.visual_id, self._class, self.bits_per_rgb_value, self.colormap_entries, self.red_mask, self.green_mask, self.blue_mask = unpacker.unpack("IBBHIII4x")
+        self.visual_id, self._class, self.bits_per_rgb_value, self.colormap_entries, self.red_mask, self.green_mask, self.blue_mask = unpacker.unpack(
+            "IBBHIII4x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IBBHIII4x", self.visual_id, self._class, self.bits_per_rgb_value, self.colormap_entries, self.red_mask, self.green_mask, self.blue_mask))
+        buf.write(
+            struct.pack(
+                "=IBBHIII4x",
+                self.visual_id,
+                self._class,
+                self.bits_per_rgb_value,
+                self.colormap_entries,
+                self.red_mask,
+                self.green_mask,
+                self.blue_mask))
         return buf.getvalue()
     fixed_size = 24
+
+
 class DEPTH(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.depth, self.visuals_len = unpacker.unpack("BxH4x")
         self.visuals = xcffib.List(unpacker, VISUALTYPE, self.visuals_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=BxH4x", self.depth, self.visuals_len))
         buf.write(xcffib.pack_list(self.visuals, VISUALTYPE))
         return buf.getvalue()
+
+
 class EventMask:
     NoEvent = 0
     KeyPress = 1 << 0
     KeyRelease = 1 << 1
     ButtonPress = 1 << 2
     ButtonRelease = 1 << 3
     EnterWindow = 1 << 4
@@ -111,461 +174,895 @@
     ResizeRedirect = 1 << 18
     SubstructureNotify = 1 << 19
     SubstructureRedirect = 1 << 20
     FocusChange = 1 << 21
     PropertyChange = 1 << 22
     ColorMapChange = 1 << 23
     OwnerGrabButton = 1 << 24
+
+
 class BackingStore:
     NotUseful = 0
     WhenMapped = 1
     Always = 2
+
+
 class SCREEN(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.root, self.default_colormap, self.white_pixel, self.black_pixel, self.current_input_masks, self.width_in_pixels, self.height_in_pixels, self.width_in_millimeters, self.height_in_millimeters, self.min_installed_maps, self.max_installed_maps, self.root_visual, self.backing_stores, self.save_unders, self.root_depth, self.allowed_depths_len = unpacker.unpack("IIIIIHHHHHHIBBBB")
-        self.allowed_depths = xcffib.List(unpacker, DEPTH, self.allowed_depths_len)
-        self.bufsize = unpacker.offset - base
-    def pack(self):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=IIIIIHHHHHHIBBBB", self.root, self.default_colormap, self.white_pixel, self.black_pixel, self.current_input_masks, self.width_in_pixels, self.height_in_pixels, self.width_in_millimeters, self.height_in_millimeters, self.min_installed_maps, self.max_installed_maps, self.root_visual, self.backing_stores, self.save_unders, self.root_depth, self.allowed_depths_len))
+        self.root, self.default_colormap, self.white_pixel, self.black_pixel, self.current_input_masks, self.width_in_pixels, self.height_in_pixels, self.width_in_millimeters, self.height_in_millimeters, self.min_installed_maps, self.max_installed_maps, self.root_visual, self.backing_stores, self.save_unders, self.root_depth, self.allowed_depths_len = unpacker.unpack(
+            "IIIIIHHHHHHIBBBB")
+        self.allowed_depths = xcffib.List(
+            unpacker,
+            DEPTH,
+            self.allowed_depths_len)
+        self.bufsize = unpacker.offset - base
+
+    def pack(self):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=IIIIIHHHHHHIBBBB",
+                self.root,
+                self.default_colormap,
+                self.white_pixel,
+                self.black_pixel,
+                self.current_input_masks,
+                self.width_in_pixels,
+                self.height_in_pixels,
+                self.width_in_millimeters,
+                self.height_in_millimeters,
+                self.min_installed_maps,
+                self.max_installed_maps,
+                self.root_visual,
+                self.backing_stores,
+                self.save_unders,
+                self.root_depth,
+                self.allowed_depths_len))
         buf.write(xcffib.pack_list(self.allowed_depths, DEPTH))
         return buf.getvalue()
+
+
 class SetupRequest(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.byte_order, self.protocol_major_version, self.protocol_minor_version, self.authorization_protocol_name_len, self.authorization_protocol_data_len = unpacker.unpack("BxHHHH2x")
-        self.authorization_protocol_name = xcffib.List(unpacker, "c", self.authorization_protocol_name_len)
+        self.byte_order, self.protocol_major_version, self.protocol_minor_version, self.authorization_protocol_name_len, self.authorization_protocol_data_len = unpacker.unpack(
+            "BxHHHH2x")
+        self.authorization_protocol_name = xcffib.List(
+            unpacker,
+            "c",
+            self.authorization_protocol_name_len)
         unpacker.pad("c")
-        self.authorization_protocol_data = xcffib.List(unpacker, "c", self.authorization_protocol_data_len)
-        self.bufsize = unpacker.offset - base
-    def pack(self):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=BxHHHH2x", self.byte_order, self.protocol_major_version, self.protocol_minor_version, self.authorization_protocol_name_len, self.authorization_protocol_data_len))
+        self.authorization_protocol_data = xcffib.List(
+            unpacker,
+            "c",
+            self.authorization_protocol_data_len)
+        self.bufsize = unpacker.offset - base
+
+    def pack(self):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=BxHHHH2x",
+                self.byte_order,
+                self.protocol_major_version,
+                self.protocol_minor_version,
+                self.authorization_protocol_name_len,
+                self.authorization_protocol_data_len))
         buf.write(xcffib.pack_list(self.authorization_protocol_name, "c"))
         buf.write(xcffib.pack_list(self.authorization_protocol_data, "c"))
         return buf.getvalue()
+
+
 class SetupFailed(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.status, self.reason_len, self.protocol_major_version, self.protocol_minor_version, self.length = unpacker.unpack("BBHHH")
+        self.status, self.reason_len, self.protocol_major_version, self.protocol_minor_version, self.length = unpacker.unpack(
+            "BBHHH")
         self.reason = xcffib.List(unpacker, "c", self.reason_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBHHH", self.status, self.reason_len, self.protocol_major_version, self.protocol_minor_version, self.length))
+        buf.write(
+            struct.pack(
+                "=BBHHH",
+                self.status,
+                self.reason_len,
+                self.protocol_major_version,
+                self.protocol_minor_version,
+                self.length))
         buf.write(xcffib.pack_list(self.reason, "c"))
         return buf.getvalue()
+
+
 class SetupAuthenticate(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.status, self.length = unpacker.unpack("B5xH")
         self.reason = xcffib.List(unpacker, "c", self.length * 4)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=B5xH", self.status, self.length))
         buf.write(xcffib.pack_list(self.reason, "c"))
         return buf.getvalue()
+
+
 class ImageOrder:
     LSBFirst = 0
     MSBFirst = 1
+
+
 class Setup(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.status, self.protocol_major_version, self.protocol_minor_version, self.length, self.release_number, self.resource_id_base, self.resource_id_mask, self.motion_buffer_size, self.vendor_len, self.maximum_request_length, self.roots_len, self.pixmap_formats_len, self.image_byte_order, self.bitmap_format_bit_order, self.bitmap_format_scanline_unit, self.bitmap_format_scanline_pad, self.min_keycode, self.max_keycode = unpacker.unpack("BxHHHIIIIHHBBBBBBBB4x")
+        self.status, self.protocol_major_version, self.protocol_minor_version, self.length, self.release_number, self.resource_id_base, self.resource_id_mask, self.motion_buffer_size, self.vendor_len, self.maximum_request_length, self.roots_len, self.pixmap_formats_len, self.image_byte_order, self.bitmap_format_bit_order, self.bitmap_format_scanline_unit, self.bitmap_format_scanline_pad, self.min_keycode, self.max_keycode = unpacker.unpack(
+            "BxHHHIIIIHHBBBBBBBB4x")
         self.vendor = xcffib.List(unpacker, "c", self.vendor_len)
         unpacker.pad(FORMAT)
-        self.pixmap_formats = xcffib.List(unpacker, FORMAT, self.pixmap_formats_len)
+        self.pixmap_formats = xcffib.List(
+            unpacker,
+            FORMAT,
+            self.pixmap_formats_len)
         unpacker.pad(SCREEN)
         self.roots = xcffib.List(unpacker, SCREEN, self.roots_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BxHHHIIIIHHBBBBBBBB4x", self.status, self.protocol_major_version, self.protocol_minor_version, self.length, self.release_number, self.resource_id_base, self.resource_id_mask, self.motion_buffer_size, self.vendor_len, self.maximum_request_length, self.roots_len, self.pixmap_formats_len, self.image_byte_order, self.bitmap_format_bit_order, self.bitmap_format_scanline_unit, self.bitmap_format_scanline_pad, self.min_keycode, self.max_keycode))
+        buf.write(
+            struct.pack(
+                "=BxHHHIIIIHHBBBBBBBB4x",
+                self.status,
+                self.protocol_major_version,
+                self.protocol_minor_version,
+                self.length,
+                self.release_number,
+                self.resource_id_base,
+                self.resource_id_mask,
+                self.motion_buffer_size,
+                self.vendor_len,
+                self.maximum_request_length,
+                self.roots_len,
+                self.pixmap_formats_len,
+                self.image_byte_order,
+                self.bitmap_format_bit_order,
+                self.bitmap_format_scanline_unit,
+                self.bitmap_format_scanline_pad,
+                self.min_keycode,
+                self.max_keycode))
         buf.write(xcffib.pack_list(self.vendor, "c"))
         buf.write(xcffib.pack_list(self.pixmap_formats, FORMAT))
         buf.write(xcffib.pack_list(self.roots, SCREEN))
         return buf.getvalue()
+
+
 class ModMask:
     Shift = 1 << 0
     Lock = 1 << 1
     Control = 1 << 2
     _1 = 1 << 3
     _2 = 1 << 4
     _3 = 1 << 5
     _4 = 1 << 6
     _5 = 1 << 7
     Any = 1 << 15
+
+
 class KeyButMask:
     Shift = 1 << 0
     Lock = 1 << 1
     Control = 1 << 2
     Mod1 = 1 << 3
     Mod2 = 1 << 4
     Mod3 = 1 << 5
     Mod4 = 1 << 6
     Mod5 = 1 << 7
     Button1 = 1 << 8
     Button2 = 1 << 9
     Button3 = 1 << 10
     Button4 = 1 << 11
     Button5 = 1 << 12
+
+
 class Window:
     _None = 0
+
+
 class KeyPressEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen = unpacker.unpack("xB2xIIIIhhhhHBx")
+        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen = unpacker.unpack(
+            "xB2xIIIIhhhhHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIIhhhhHBx", self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen))
+        buf.write(
+            struct.pack(
+                "=BIIIIhhhhHBx",
+                self.detail,
+                self.time,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.state,
+                self.same_screen))
         return buf.getvalue()
 _events[2] = KeyPressEvent
+
+
 class KeyReleaseEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen = unpacker.unpack("xB2xIIIIhhhhHBx")
+        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen = unpacker.unpack(
+            "xB2xIIIIhhhhHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIIhhhhHBx", self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen))
+        buf.write(
+            struct.pack(
+                "=BIIIIhhhhHBx",
+                self.detail,
+                self.time,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.state,
+                self.same_screen))
         return buf.getvalue()
 _events[3] = KeyReleaseEvent
+
+
 class ButtonMask:
     _1 = 1 << 8
     _2 = 1 << 9
     _3 = 1 << 10
     _4 = 1 << 11
     _5 = 1 << 12
     Any = 1 << 15
+
+
 class ButtonPressEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen = unpacker.unpack("xB2xIIIIhhhhHBx")
+        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen = unpacker.unpack(
+            "xB2xIIIIhhhhHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIIhhhhHBx", self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen))
+        buf.write(
+            struct.pack(
+                "=BIIIIhhhhHBx",
+                self.detail,
+                self.time,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.state,
+                self.same_screen))
         return buf.getvalue()
 _events[4] = ButtonPressEvent
+
+
 class ButtonReleaseEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen = unpacker.unpack("xB2xIIIIhhhhHBx")
+        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen = unpacker.unpack(
+            "xB2xIIIIhhhhHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIIhhhhHBx", self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen))
+        buf.write(
+            struct.pack(
+                "=BIIIIhhhhHBx",
+                self.detail,
+                self.time,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.state,
+                self.same_screen))
         return buf.getvalue()
 _events[5] = ButtonReleaseEvent
+
+
 class Motion:
     Normal = 0
     Hint = 1
+
+
 class MotionNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen = unpacker.unpack("xB2xIIIIhhhhHBx")
+        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen = unpacker.unpack(
+            "xB2xIIIIhhhhHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIIhhhhHBx", self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen))
+        buf.write(
+            struct.pack(
+                "=BIIIIhhhhHBx",
+                self.detail,
+                self.time,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.state,
+                self.same_screen))
         return buf.getvalue()
 _events[6] = MotionNotifyEvent
+
+
 class NotifyDetail:
     Ancestor = 0
     Virtual = 1
     Inferior = 2
     Nonlinear = 3
     NonlinearVirtual = 4
     Pointer = 5
     PointerRoot = 6
     _None = 7
+
+
 class NotifyMode:
     Normal = 0
     Grab = 1
     Ungrab = 2
     WhileGrabbed = 3
+
+
 class EnterNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.mode, self.same_screen_focus = unpacker.unpack("xB2xIIIIhhhhHBB")
+        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.mode, self.same_screen_focus = unpacker.unpack(
+            "xB2xIIIIhhhhHBB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIIhhhhHBB", self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.mode, self.same_screen_focus))
+        buf.write(
+            struct.pack(
+                "=BIIIIhhhhHBB",
+                self.detail,
+                self.time,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.state,
+                self.mode,
+                self.same_screen_focus))
         return buf.getvalue()
 _events[7] = EnterNotifyEvent
+
+
 class LeaveNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.mode, self.same_screen_focus = unpacker.unpack("xB2xIIIIhhhhHBB")
+        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.mode, self.same_screen_focus = unpacker.unpack(
+            "xB2xIIIIhhhhHBB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIIhhhhHBB", self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.mode, self.same_screen_focus))
+        buf.write(
+            struct.pack(
+                "=BIIIIhhhhHBB",
+                self.detail,
+                self.time,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.state,
+                self.mode,
+                self.same_screen_focus))
         return buf.getvalue()
 _events[8] = LeaveNotifyEvent
+
+
 class FocusInEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         self.detail, self.event, self.mode = unpacker.unpack("xB2xIB3x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=BIB3x", self.detail, self.event, self.mode))
         return buf.getvalue()
 _events[9] = FocusInEvent
+
+
 class FocusOutEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         self.detail, self.event, self.mode = unpacker.unpack("xB2xIB3x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=BIB3x", self.detail, self.event, self.mode))
         return buf.getvalue()
 _events[10] = FocusOutEvent
+
+
 class KeymapNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("x")
         self.keys = xcffib.List(unpacker, "B", 31)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(xcffib.pack_list(self.keys, "B"))
         return buf.getvalue()
 _events[11] = KeymapNotifyEvent
+
+
 class ExposeEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.window, self.x, self.y, self.width, self.height, self.count = unpacker.unpack("xx2xIHHHHH2x")
+        self.window, self.x, self.y, self.width, self.height, self.count = unpacker.unpack(
+            "xx2xIHHHHH2x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xIHHHHH2x", self.window, self.x, self.y, self.width, self.height, self.count))
+        buf.write(
+            struct.pack(
+                "=xIHHHHH2x",
+                self.window,
+                self.x,
+                self.y,
+                self.width,
+                self.height,
+                self.count))
         return buf.getvalue()
 _events[12] = ExposeEvent
+
+
 class GraphicsExposureEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.drawable, self.x, self.y, self.width, self.height, self.minor_opcode, self.count, self.major_opcode = unpacker.unpack("xx2xIHHHHHHB3x")
+        self.drawable, self.x, self.y, self.width, self.height, self.minor_opcode, self.count, self.major_opcode = unpacker.unpack(
+            "xx2xIHHHHHHB3x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xIHHHHHHB3x", self.drawable, self.x, self.y, self.width, self.height, self.minor_opcode, self.count, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=xIHHHHHHB3x",
+                self.drawable,
+                self.x,
+                self.y,
+                self.width,
+                self.height,
+                self.minor_opcode,
+                self.count,
+                self.major_opcode))
         return buf.getvalue()
 _events[13] = GraphicsExposureEvent
+
+
 class NoExposureEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.drawable, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.drawable, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xIHBx", self.drawable, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=xIHBx",
+                self.drawable,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 _events[14] = NoExposureEvent
+
+
 class Visibility:
     Unobscured = 0
     PartiallyObscured = 1
     FullyObscured = 2
+
+
 class VisibilityNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         self.window, self.state = unpacker.unpack("xx2xIB3x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=xIB3x", self.window, self.state))
         return buf.getvalue()
 _events[15] = VisibilityNotifyEvent
+
+
 class CreateNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.parent, self.window, self.x, self.y, self.width, self.height, self.border_width, self.override_redirect = unpacker.unpack("xx2xIIhhHHHBx")
+        self.parent, self.window, self.x, self.y, self.width, self.height, self.border_width, self.override_redirect = unpacker.unpack(
+            "xx2xIIhhHHHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xIIhhHHHBx", self.parent, self.window, self.x, self.y, self.width, self.height, self.border_width, self.override_redirect))
+        buf.write(
+            struct.pack(
+                "=xIIhhHHHBx",
+                self.parent,
+                self.window,
+                self.x,
+                self.y,
+                self.width,
+                self.height,
+                self.border_width,
+                self.override_redirect))
         return buf.getvalue()
 _events[16] = CreateNotifyEvent
+
+
 class DestroyNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         self.event, self.window = unpacker.unpack("xx2xII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=xII", self.event, self.window))
         return buf.getvalue()
 _events[17] = DestroyNotifyEvent
+
+
 class UnmapNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.event, self.window, self.from_configure = unpacker.unpack("xx2xIIB3x")
+        self.event, self.window, self.from_configure = unpacker.unpack(
+            "xx2xIIB3x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xIIB3x", self.event, self.window, self.from_configure))
+        buf.write(
+            struct.pack(
+                "=xIIB3x",
+                self.event,
+                self.window,
+                self.from_configure))
         return buf.getvalue()
 _events[18] = UnmapNotifyEvent
+
+
 class MapNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.event, self.window, self.override_redirect = unpacker.unpack("xx2xIIB3x")
+        self.event, self.window, self.override_redirect = unpacker.unpack(
+            "xx2xIIB3x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xIIB3x", self.event, self.window, self.override_redirect))
+        buf.write(
+            struct.pack(
+                "=xIIB3x",
+                self.event,
+                self.window,
+                self.override_redirect))
         return buf.getvalue()
 _events[19] = MapNotifyEvent
+
+
 class MapRequestEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         self.parent, self.window = unpacker.unpack("xx2xII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=xII", self.parent, self.window))
         return buf.getvalue()
 _events[20] = MapRequestEvent
+
+
 class ReparentNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.event, self.window, self.parent, self.x, self.y, self.override_redirect = unpacker.unpack("xx2xIIIhhB3x")
+        self.event, self.window, self.parent, self.x, self.y, self.override_redirect = unpacker.unpack(
+            "xx2xIIIhhB3x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xIIIhhB3x", self.event, self.window, self.parent, self.x, self.y, self.override_redirect))
+        buf.write(
+            struct.pack(
+                "=xIIIhhB3x",
+                self.event,
+                self.window,
+                self.parent,
+                self.x,
+                self.y,
+                self.override_redirect))
         return buf.getvalue()
 _events[21] = ReparentNotifyEvent
+
+
 class ConfigureNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.event, self.window, self.above_sibling, self.x, self.y, self.width, self.height, self.border_width, self.override_redirect = unpacker.unpack("xx2xIIIhhHHHBx")
+        self.event, self.window, self.above_sibling, self.x, self.y, self.width, self.height, self.border_width, self.override_redirect = unpacker.unpack(
+            "xx2xIIIhhHHHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xIIIhhHHHBx", self.event, self.window, self.above_sibling, self.x, self.y, self.width, self.height, self.border_width, self.override_redirect))
+        buf.write(
+            struct.pack(
+                "=xIIIhhHHHBx",
+                self.event,
+                self.window,
+                self.above_sibling,
+                self.x,
+                self.y,
+                self.width,
+                self.height,
+                self.border_width,
+                self.override_redirect))
         return buf.getvalue()
 _events[22] = ConfigureNotifyEvent
+
+
 class ConfigureRequestEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.stack_mode, self.parent, self.window, self.sibling, self.x, self.y, self.width, self.height, self.border_width, self.value_mask = unpacker.unpack("xB2xIIIhhHHHH")
+        self.stack_mode, self.parent, self.window, self.sibling, self.x, self.y, self.width, self.height, self.border_width, self.value_mask = unpacker.unpack(
+            "xB2xIIIhhHHHH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIhhHHHH", self.stack_mode, self.parent, self.window, self.sibling, self.x, self.y, self.width, self.height, self.border_width, self.value_mask))
+        buf.write(
+            struct.pack(
+                "=BIIIhhHHHH",
+                self.stack_mode,
+                self.parent,
+                self.window,
+                self.sibling,
+                self.x,
+                self.y,
+                self.width,
+                self.height,
+                self.border_width,
+                self.value_mask))
         return buf.getvalue()
 _events[23] = ConfigureRequestEvent
+
+
 class GravityNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         self.event, self.window, self.x, self.y = unpacker.unpack("xx2xIIhh")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xIIhh", self.event, self.window, self.x, self.y))
+        buf.write(
+            struct.pack(
+                "=xIIhh",
+                self.event,
+                self.window,
+                self.x,
+                self.y))
         return buf.getvalue()
 _events[24] = GravityNotifyEvent
+
+
 class ResizeRequestEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         self.window, self.width, self.height = unpacker.unpack("xx2xIHH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=xIHH", self.window, self.width, self.height))
         return buf.getvalue()
 _events[25] = ResizeRequestEvent
+
+
 class Place:
     OnTop = 0
     OnBottom = 1
+
+
 class CirculateNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         self.event, self.window, self.place = unpacker.unpack("xx2xII4xB3x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xII4xB3x", self.event, self.window, self.place))
+        buf.write(
+            struct.pack(
+                "=xII4xB3x",
+                self.event,
+                self.window,
+                self.place))
         return buf.getvalue()
 _events[26] = CirculateNotifyEvent
+
+
 class CirculateRequestEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         self.event, self.window, self.place = unpacker.unpack("xx2xII4xB3x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xII4xB3x", self.event, self.window, self.place))
+        buf.write(
+            struct.pack(
+                "=xII4xB3x",
+                self.event,
+                self.window,
+                self.place))
         return buf.getvalue()
 _events[27] = CirculateRequestEvent
+
+
 class Property:
     NewValue = 0
     Delete = 1
+
+
 class PropertyNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.window, self.atom, self.time, self.state = unpacker.unpack("xx2xIIIB3x")
+        self.window, self.atom, self.time, self.state = unpacker.unpack(
+            "xx2xIIIB3x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xIIIB3x", self.window, self.atom, self.time, self.state))
+        buf.write(
+            struct.pack(
+                "=xIIIB3x",
+                self.window,
+                self.atom,
+                self.time,
+                self.state))
         return buf.getvalue()
 _events[28] = PropertyNotifyEvent
+
+
 class SelectionClearEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         self.time, self.owner, self.selection = unpacker.unpack("xx2xIII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=xIII", self.time, self.owner, self.selection))
         return buf.getvalue()
 _events[29] = SelectionClearEvent
+
+
 class Time:
     CurrentTime = 0
+
+
 class Atom:
     _None = 0
     Any = 0
     PRIMARY = 1
     SECONDARY = 2
     ARC = 3
     ATOM = 4
@@ -629,305 +1126,542 @@
     NOTICE = 62
     FONT_NAME = 63
     FAMILY_NAME = 64
     FULL_NAME = 65
     CAP_HEIGHT = 66
     WM_CLASS = 67
     WM_TRANSIENT_FOR = 68
+
+
 class SelectionRequestEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.time, self.owner, self.requestor, self.selection, self.target, self.property = unpacker.unpack("xx2xIIIIII")
+        self.time, self.owner, self.requestor, self.selection, self.target, self.property = unpacker.unpack(
+            "xx2xIIIIII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xIIIIII", self.time, self.owner, self.requestor, self.selection, self.target, self.property))
+        buf.write(
+            struct.pack(
+                "=xIIIIII",
+                self.time,
+                self.owner,
+                self.requestor,
+                self.selection,
+                self.target,
+                self.property))
         return buf.getvalue()
 _events[30] = SelectionRequestEvent
+
+
 class SelectionNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.time, self.requestor, self.selection, self.target, self.property = unpacker.unpack("xx2xIIIII")
+        self.time, self.requestor, self.selection, self.target, self.property = unpacker.unpack(
+            "xx2xIIIII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xIIIII", self.time, self.requestor, self.selection, self.target, self.property))
+        buf.write(
+            struct.pack(
+                "=xIIIII",
+                self.time,
+                self.requestor,
+                self.selection,
+                self.target,
+                self.property))
         return buf.getvalue()
 _events[31] = SelectionNotifyEvent
+
+
 class ColormapState:
     Uninstalled = 0
     Installed = 1
+
+
 class Colormap:
     _None = 0
+
+
 class ColormapNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.window, self.colormap, self.new, self.state = unpacker.unpack("xx2xIIBB2x")
+        self.window, self.colormap, self.new, self.state = unpacker.unpack(
+            "xx2xIIBB2x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xIIBB2x", self.window, self.colormap, self.new, self.state))
+        buf.write(
+            struct.pack(
+                "=xIIBB2x",
+                self.window,
+                self.colormap,
+                self.new,
+                self.state))
         return buf.getvalue()
 _events[32] = ColormapNotifyEvent
+
+
 class ClientMessageData(xcffib.Union):
+
     def __init__(self, unpacker):
         xcffib.Union.__init__(self, unpacker)
-        self.data8 = xcffib.List(unpacker, "B", 20)
-        self.data16 = xcffib.List(unpacker, "H", 10)
-        self.data32 = xcffib.List(unpacker, "I", 5)
+        self.data8 = xcffib.List(unpacker.copy(), "B", 20)
+        self.data16 = xcffib.List(unpacker.copy(), "H", 10)
+        self.data32 = xcffib.List(unpacker.copy(), "I", 5)
+
+
 class ClientMessageEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         self.format, self.window, self.type = unpacker.unpack("xB2xII")
         self.data = ClientMessageData(unpacker)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=BII", self.format, self.window, self.type))
         buf.write(self.data.pack())
         return buf.getvalue()
 _events[33] = ClientMessageEvent
+
+
 class Mapping:
     Modifier = 0
     Keyboard = 1
     Pointer = 2
+
+
 class MappingNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.request, self.first_keycode, self.count = unpacker.unpack("xx2xBBBx")
+        self.request, self.first_keycode, self.count = unpacker.unpack(
+            "xx2xBBBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xBBBx", self.request, self.first_keycode, self.count))
+        buf.write(
+            struct.pack(
+                "=xBBBx",
+                self.request,
+                self.first_keycode,
+                self.count))
         return buf.getvalue()
 _events[34] = MappingNotifyEvent
+
+
 class GeGenericEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x22x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=22x"))
         return buf.getvalue()
 _events[35] = GeGenericEvent
+
+
 class RequestError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadRequest = RequestError
 _errors[1] = RequestError
+
+
 class ValueError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadValue = ValueError
 _errors[2] = ValueError
+
+
 class WindowError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadWindow = WindowError
 _errors[3] = WindowError
+
+
 class PixmapError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadPixmap = PixmapError
 _errors[4] = PixmapError
+
+
 class AtomError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadAtom = AtomError
 _errors[5] = AtomError
+
+
 class CursorError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadCursor = CursorError
 _errors[6] = CursorError
+
+
 class FontError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadFont = FontError
 _errors[7] = FontError
+
+
 class MatchError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadMatch = MatchError
 _errors[8] = MatchError
+
+
 class DrawableError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadDrawable = DrawableError
 _errors[9] = DrawableError
+
+
 class AccessError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadAccess = AccessError
 _errors[10] = AccessError
+
+
 class AllocError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadAlloc = AllocError
 _errors[11] = AllocError
+
+
 class ColormapError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadColormap = ColormapError
 _errors[12] = ColormapError
+
+
 class GContextError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadGContext = GContextError
 _errors[13] = GContextError
+
+
 class IDChoiceError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadIDChoice = IDChoiceError
 _errors[14] = IDChoiceError
+
+
 class NameError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadName = NameError
 _errors[15] = NameError
+
+
 class LengthError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadLength = LengthError
 _errors[16] = LengthError
+
+
 class ImplementationError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHBx")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHBx", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadImplementation = ImplementationError
 _errors[17] = ImplementationError
+
+
 class WindowClass:
     CopyFromParent = 0
     InputOutput = 1
     InputOnly = 2
+
+
 class CW:
     BackPixmap = 1 << 0
     BackPixel = 1 << 1
     BorderPixmap = 1 << 2
     BorderPixel = 1 << 3
     BitGravity = 1 << 4
     WinGravity = 1 << 5
@@ -936,331 +1670,504 @@
     BackingPixel = 1 << 8
     OverrideRedirect = 1 << 9
     SaveUnder = 1 << 10
     EventMask = 1 << 11
     DontPropagate = 1 << 12
     Colormap = 1 << 13
     Cursor = 1 << 14
+
+
 class BackPixmap:
     _None = 0
     ParentRelative = 1
+
+
 class Gravity:
     BitForget = 0
     WinUnmap = 0
     NorthWest = 1
     North = 2
     NorthEast = 3
     West = 4
     Center = 5
     East = 6
     SouthWest = 7
     South = 8
     SouthEast = 9
     Static = 10
+
+
 class MapState:
     Unmapped = 0
     Unviewable = 1
     Viewable = 2
+
+
 class GetWindowAttributesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.backing_store, self.visual, self._class, self.bit_gravity, self.win_gravity, self.backing_planes, self.backing_pixel, self.save_under, self.map_is_installed, self.map_state, self.override_redirect, self.colormap, self.all_event_masks, self.your_event_mask, self.do_not_propagate_mask = unpacker.unpack("xB2x4xIHBBIIBBBBIIIH2x")
+        self.backing_store, self.visual, self._class, self.bit_gravity, self.win_gravity, self.backing_planes, self.backing_pixel, self.save_under, self.map_is_installed, self.map_state, self.override_redirect, self.colormap, self.all_event_masks, self.your_event_mask, self.do_not_propagate_mask = unpacker.unpack(
+            "xB2x4xIHBBIIBBBBIIIH2x")
         self.bufsize = unpacker.offset - base
+
+
 class GetWindowAttributesCookie(xcffib.Cookie):
     reply_type = GetWindowAttributesReply
+
+
 class SetMode:
     Insert = 0
     Delete = 1
+
+
 class ConfigWindow:
     X = 1 << 0
     Y = 1 << 1
     Width = 1 << 2
     Height = 1 << 3
     BorderWidth = 1 << 4
     Sibling = 1 << 5
     StackMode = 1 << 6
+
+
 class StackMode:
     Above = 0
     Below = 1
     TopIf = 2
     BottomIf = 3
     Opposite = 4
+
+
 class Circulate:
     RaiseLowest = 0
     LowerHighest = 1
+
+
 class GetGeometryReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.depth, self.root, self.x, self.y, self.width, self.height, self.border_width = unpacker.unpack("xB2x4xIhhHHH2x")
+        self.depth, self.root, self.x, self.y, self.width, self.height, self.border_width = unpacker.unpack(
+            "xB2x4xIhhHHH2x")
         self.bufsize = unpacker.offset - base
+
+
 class GetGeometryCookie(xcffib.Cookie):
     reply_type = GetGeometryReply
+
+
 class QueryTreeReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.root, self.parent, self.children_len = unpacker.unpack("xx2x4xIIH14x")
+        self.root, self.parent, self.children_len = unpacker.unpack(
+            "xx2x4xIIH14x")
         self.children = xcffib.List(unpacker, "I", self.children_len)
         self.bufsize = unpacker.offset - base
+
+
 class QueryTreeCookie(xcffib.Cookie):
     reply_type = QueryTreeReply
+
+
 class InternAtomReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.atom, = unpacker.unpack("xx2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class InternAtomCookie(xcffib.Cookie):
     reply_type = InternAtomReply
+
+
 class GetAtomNameReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.name_len, = unpacker.unpack("xx2x4xH22x")
         self.name = xcffib.List(unpacker, "c", self.name_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetAtomNameCookie(xcffib.Cookie):
     reply_type = GetAtomNameReply
+
+
 class PropMode:
     Replace = 0
     Prepend = 1
     Append = 2
+
+
 class GetPropertyType:
     Any = 0
+
+
 class GetPropertyReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.format, self.type, self.bytes_after, self.value_len = unpacker.unpack("xB2x4xIII12x")
-        self.value = xcffib.List(unpacker, "c", self.value_len * (self.format // 8))
+        self.format, self.type, self.bytes_after, self.value_len = unpacker.unpack(
+            "xB2x4xIII12x")
+        self.value = xcffib.List(
+            unpacker, "c", self.value_len * (self.format // 8))
         self.bufsize = unpacker.offset - base
+
+
 class GetPropertyCookie(xcffib.Cookie):
     reply_type = GetPropertyReply
+
+
 class ListPropertiesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.atoms_len, = unpacker.unpack("xx2x4xH22x")
         self.atoms = xcffib.List(unpacker, "I", self.atoms_len)
         self.bufsize = unpacker.offset - base
+
+
 class ListPropertiesCookie(xcffib.Cookie):
     reply_type = ListPropertiesReply
+
+
 class GetSelectionOwnerReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.owner, = unpacker.unpack("xx2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class GetSelectionOwnerCookie(xcffib.Cookie):
     reply_type = GetSelectionOwnerReply
+
+
 class SendEventDest:
     PointerWindow = 0
     ItemFocus = 1
+
+
 class GrabMode:
     Sync = 0
     Async = 1
+
+
 class GrabStatus:
     Success = 0
     AlreadyGrabbed = 1
     InvalidTime = 2
     NotViewable = 3
     Frozen = 4
+
+
 class Cursor:
     _None = 0
+
+
 class GrabPointerReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, = unpacker.unpack("xB2x4x")
         self.bufsize = unpacker.offset - base
+
+
 class GrabPointerCookie(xcffib.Cookie):
     reply_type = GrabPointerReply
+
+
 class ButtonIndex:
     Any = 0
     _1 = 1
     _2 = 2
     _3 = 3
     _4 = 4
     _5 = 5
+
+
 class GrabKeyboardReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, = unpacker.unpack("xB2x4x")
         self.bufsize = unpacker.offset - base
+
+
 class GrabKeyboardCookie(xcffib.Cookie):
     reply_type = GrabKeyboardReply
+
+
 class Grab:
     Any = 0
+
+
 class Allow:
     AsyncPointer = 0
     SyncPointer = 1
     ReplayPointer = 2
     AsyncKeyboard = 3
     SyncKeyboard = 4
     ReplayKeyboard = 5
     AsyncBoth = 6
     SyncBoth = 7
+
+
 class QueryPointerReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.same_screen, self.root, self.child, self.root_x, self.root_y, self.win_x, self.win_y, self.mask = unpacker.unpack("xB2x4xIIhhhhH2x")
+        self.same_screen, self.root, self.child, self.root_x, self.root_y, self.win_x, self.win_y, self.mask = unpacker.unpack(
+            "xB2x4xIIhhhhH2x")
         self.bufsize = unpacker.offset - base
+
+
 class QueryPointerCookie(xcffib.Cookie):
     reply_type = QueryPointerReply
+
+
 class TIMECOORD(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.time, self.x, self.y = unpacker.unpack("Ihh")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=Ihh", self.time, self.x, self.y))
         return buf.getvalue()
     fixed_size = 8
+
+
 class GetMotionEventsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.events_len, = unpacker.unpack("xx2x4xI20x")
         self.events = xcffib.List(unpacker, TIMECOORD, self.events_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetMotionEventsCookie(xcffib.Cookie):
     reply_type = GetMotionEventsReply
+
+
 class TranslateCoordinatesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.same_screen, self.child, self.dst_x, self.dst_y = unpacker.unpack("xB2x4xIhh")
+        self.same_screen, self.child, self.dst_x, self.dst_y = unpacker.unpack(
+            "xB2x4xIhh")
         self.bufsize = unpacker.offset - base
+
+
 class TranslateCoordinatesCookie(xcffib.Cookie):
     reply_type = TranslateCoordinatesReply
+
+
 class InputFocus:
     _None = 0
     PointerRoot = 1
     Parent = 2
     FollowKeyboard = 3
+
+
 class GetInputFocusReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.revert_to, self.focus = unpacker.unpack("xB2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class GetInputFocusCookie(xcffib.Cookie):
     reply_type = GetInputFocusReply
+
+
 class QueryKeymapReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x")
         self.keys = xcffib.List(unpacker, "B", 32)
         self.bufsize = unpacker.offset - base
+
+
 class QueryKeymapCookie(xcffib.Cookie):
     reply_type = QueryKeymapReply
+
+
 class FontDraw:
     LeftToRight = 0
     RightToLeft = 1
+
+
 class FONTPROP(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.name, self.value = unpacker.unpack("II")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=II", self.name, self.value))
         return buf.getvalue()
     fixed_size = 8
+
+
 class CHARINFO(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.left_side_bearing, self.right_side_bearing, self.character_width, self.ascent, self.descent, self.attributes = unpacker.unpack("hhhhhH")
+        self.left_side_bearing, self.right_side_bearing, self.character_width, self.ascent, self.descent, self.attributes = unpacker.unpack(
+            "hhhhhH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=hhhhhH", self.left_side_bearing, self.right_side_bearing, self.character_width, self.ascent, self.descent, self.attributes))
+        buf.write(
+            struct.pack(
+                "=hhhhhH",
+                self.left_side_bearing,
+                self.right_side_bearing,
+                self.character_width,
+                self.ascent,
+                self.descent,
+                self.attributes))
         return buf.getvalue()
     fixed_size = 12
+
+
 class QueryFontReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x")
         self.min_bounds = CHARINFO(unpacker)
         unpacker.unpack("4x")
         unpacker.pad(CHARINFO)
         self.max_bounds = CHARINFO(unpacker)
-        self.min_char_or_byte2, self.max_char_or_byte2, self.default_char, self.properties_len, self.draw_direction, self.min_byte1, self.max_byte1, self.all_chars_exist, self.font_ascent, self.font_descent, self.char_infos_len = unpacker.unpack("4xHHHHBBBBhhI")
+        self.min_char_or_byte2, self.max_char_or_byte2, self.default_char, self.properties_len, self.draw_direction, self.min_byte1, self.max_byte1, self.all_chars_exist, self.font_ascent, self.font_descent, self.char_infos_len = unpacker.unpack(
+            "4xHHHHBBBBhhI")
         unpacker.pad(FONTPROP)
         self.properties = xcffib.List(unpacker, FONTPROP, self.properties_len)
         unpacker.pad(CHARINFO)
         self.char_infos = xcffib.List(unpacker, CHARINFO, self.char_infos_len)
         self.bufsize = unpacker.offset - base
+
+
 class QueryFontCookie(xcffib.Cookie):
     reply_type = QueryFontReply
+
+
 class QueryTextExtentsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.draw_direction, self.font_ascent, self.font_descent, self.overall_ascent, self.overall_descent, self.overall_width, self.overall_left, self.overall_right = unpacker.unpack("xB2x4xhhhhiii")
+        self.draw_direction, self.font_ascent, self.font_descent, self.overall_ascent, self.overall_descent, self.overall_width, self.overall_left, self.overall_right = unpacker.unpack(
+            "xB2x4xhhhhiii")
         self.bufsize = unpacker.offset - base
+
+
 class QueryTextExtentsCookie(xcffib.Cookie):
     reply_type = QueryTextExtentsReply
+
+
 class STR(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.name_len, = unpacker.unpack("B")
         self.name = xcffib.List(unpacker, "c", self.name_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=B", self.name_len))
         buf.write(xcffib.pack_list(self.name, "c"))
         return buf.getvalue()
+
+
 class ListFontsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.names_len, = unpacker.unpack("xx2x4xH22x")
         self.names = xcffib.List(unpacker, STR, self.names_len)
         self.bufsize = unpacker.offset - base
+
+
 class ListFontsCookie(xcffib.Cookie):
     reply_type = ListFontsReply
+
+
 class ListFontsWithInfoReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.name_len, = unpacker.unpack("xB2x4x")
         self.min_bounds = CHARINFO(unpacker)
         unpacker.unpack("4x")
         unpacker.pad(CHARINFO)
         self.max_bounds = CHARINFO(unpacker)
-        self.min_char_or_byte2, self.max_char_or_byte2, self.default_char, self.properties_len, self.draw_direction, self.min_byte1, self.max_byte1, self.all_chars_exist, self.font_ascent, self.font_descent, self.replies_hint = unpacker.unpack("4xHHHHBBBBhhI")
+        self.min_char_or_byte2, self.max_char_or_byte2, self.default_char, self.properties_len, self.draw_direction, self.min_byte1, self.max_byte1, self.all_chars_exist, self.font_ascent, self.font_descent, self.replies_hint = unpacker.unpack(
+            "4xHHHHBBBBhhI")
         unpacker.pad(FONTPROP)
         self.properties = xcffib.List(unpacker, FONTPROP, self.properties_len)
         unpacker.pad("c")
         self.name = xcffib.List(unpacker, "c", self.name_len)
         self.bufsize = unpacker.offset - base
+
+
 class ListFontsWithInfoCookie(xcffib.Cookie):
     reply_type = ListFontsWithInfoReply
+
+
 class GetFontPathReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.path_len, = unpacker.unpack("xx2x4xH22x")
         self.path = xcffib.List(unpacker, STR, self.path_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetFontPathCookie(xcffib.Cookie):
     reply_type = GetFontPathReply
+
+
 class GC:
     Function = 1 << 0
     PlaneMask = 1 << 1
     Foreground = 1 << 2
     Background = 1 << 3
     LineWidth = 1 << 4
     LineStyle = 1 << 5
@@ -1277,14 +2184,16 @@
     GraphicsExposures = 1 << 16
     ClipOriginX = 1 << 17
     ClipOriginY = 1 << 18
     ClipMask = 1 << 19
     DashOffset = 1 << 20
     DashList = 1 << 21
     ArcMode = 1 << 22
+
+
 class GX:
     clear = 0
     _and = 1
     andReverse = 2
     copy = 3
     andInverted = 4
     noop = 5
@@ -1294,870 +2203,1878 @@
     equiv = 9
     invert = 10
     orReverse = 11
     copyInverted = 12
     orInverted = 13
     nand = 14
     set = 15
+
+
 class LineStyle:
     Solid = 0
     OnOffDash = 1
     DoubleDash = 2
+
+
 class CapStyle:
     NotLast = 0
     Butt = 1
     Round = 2
     Projecting = 3
+
+
 class JoinStyle:
     Miter = 0
     Round = 1
     Bevel = 2
+
+
 class FillStyle:
     Solid = 0
     Tiled = 1
     Stippled = 2
     OpaqueStippled = 3
+
+
 class FillRule:
     EvenOdd = 0
     Winding = 1
+
+
 class SubwindowMode:
     ClipByChildren = 0
     IncludeInferiors = 1
+
+
 class ArcMode:
     Chord = 0
     PieSlice = 1
+
+
 class ClipOrdering:
     Unsorted = 0
     YSorted = 1
     YXSorted = 2
     YXBanded = 3
+
+
 class CoordMode:
     Origin = 0
     Previous = 1
+
+
 class SEGMENT(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.x1, self.y1, self.x2, self.y2 = unpacker.unpack("hhhh")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=hhhh", self.x1, self.y1, self.x2, self.y2))
         return buf.getvalue()
     fixed_size = 8
+
+
 class PolyShape:
     Complex = 0
     Nonconvex = 1
     Convex = 2
+
+
 class ImageFormat:
     XYBitmap = 0
     XYPixmap = 1
     ZPixmap = 2
+
+
 class GetImageReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.depth, self.visual = unpacker.unpack("xB2x4xI20x")
         self.data = xcffib.List(unpacker, "B", self.length * 4)
         self.bufsize = unpacker.offset - base
+
+
 class GetImageCookie(xcffib.Cookie):
     reply_type = GetImageReply
+
+
 class ColormapAlloc:
     _None = 0
     All = 1
+
+
 class ListInstalledColormapsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.cmaps_len, = unpacker.unpack("xx2x4xH22x")
         self.cmaps = xcffib.List(unpacker, "I", self.cmaps_len)
         self.bufsize = unpacker.offset - base
+
+
 class ListInstalledColormapsCookie(xcffib.Cookie):
     reply_type = ListInstalledColormapsReply
+
+
 class AllocColorReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.red, self.green, self.blue, self.pixel = unpacker.unpack("xx2x4xHHH2xI")
+        self.red, self.green, self.blue, self.pixel = unpacker.unpack(
+            "xx2x4xHHH2xI")
         self.bufsize = unpacker.offset - base
+
+
 class AllocColorCookie(xcffib.Cookie):
     reply_type = AllocColorReply
+
+
 class AllocNamedColorReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.pixel, self.exact_red, self.exact_green, self.exact_blue, self.visual_red, self.visual_green, self.visual_blue = unpacker.unpack("xx2x4xIHHHHHH")
+        self.pixel, self.exact_red, self.exact_green, self.exact_blue, self.visual_red, self.visual_green, self.visual_blue = unpacker.unpack(
+            "xx2x4xIHHHHHH")
         self.bufsize = unpacker.offset - base
+
+
 class AllocNamedColorCookie(xcffib.Cookie):
     reply_type = AllocNamedColorReply
+
+
 class AllocColorCellsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.pixels_len, self.masks_len = unpacker.unpack("xx2x4xHH20x")
         self.pixels = xcffib.List(unpacker, "I", self.pixels_len)
         unpacker.pad("I")
         self.masks = xcffib.List(unpacker, "I", self.masks_len)
         self.bufsize = unpacker.offset - base
+
+
 class AllocColorCellsCookie(xcffib.Cookie):
     reply_type = AllocColorCellsReply
+
+
 class AllocColorPlanesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.pixels_len, self.red_mask, self.green_mask, self.blue_mask = unpacker.unpack("xx2x4xH2xIII8x")
+        self.pixels_len, self.red_mask, self.green_mask, self.blue_mask = unpacker.unpack(
+            "xx2x4xH2xIII8x")
         self.pixels = xcffib.List(unpacker, "I", self.pixels_len)
         self.bufsize = unpacker.offset - base
+
+
 class AllocColorPlanesCookie(xcffib.Cookie):
     reply_type = AllocColorPlanesReply
+
+
 class ColorFlag:
     Red = 1 << 0
     Green = 1 << 1
     Blue = 1 << 2
+
+
 class COLORITEM(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.pixel, self.red, self.green, self.blue, self.flags = unpacker.unpack("IHHHBx")
+        self.pixel, self.red, self.green, self.blue, self.flags = unpacker.unpack(
+            "IHHHBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHHHBx", self.pixel, self.red, self.green, self.blue, self.flags))
+        buf.write(
+            struct.pack(
+                "=IHHHBx",
+                self.pixel,
+                self.red,
+                self.green,
+                self.blue,
+                self.flags))
         return buf.getvalue()
     fixed_size = 12
+
+
 class RGB(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.red, self.green, self.blue = unpacker.unpack("HHH2x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=HHH2x", self.red, self.green, self.blue))
         return buf.getvalue()
     fixed_size = 8
+
+
 class QueryColorsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.colors_len, = unpacker.unpack("xx2x4xH22x")
         self.colors = xcffib.List(unpacker, RGB, self.colors_len)
         self.bufsize = unpacker.offset - base
+
+
 class QueryColorsCookie(xcffib.Cookie):
     reply_type = QueryColorsReply
+
+
 class LookupColorReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.exact_red, self.exact_green, self.exact_blue, self.visual_red, self.visual_green, self.visual_blue = unpacker.unpack("xx2x4xHHHHHH")
+        self.exact_red, self.exact_green, self.exact_blue, self.visual_red, self.visual_green, self.visual_blue = unpacker.unpack(
+            "xx2x4xHHHHHH")
         self.bufsize = unpacker.offset - base
+
+
 class LookupColorCookie(xcffib.Cookie):
     reply_type = LookupColorReply
+
+
 class Pixmap:
     _None = 0
+
+
 class Font:
     _None = 0
+
+
 class QueryShapeOf:
     LargestCursor = 0
     FastestTile = 1
     FastestStipple = 2
+
+
 class QueryBestSizeReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.width, self.height = unpacker.unpack("xx2x4xHH")
         self.bufsize = unpacker.offset - base
+
+
 class QueryBestSizeCookie(xcffib.Cookie):
     reply_type = QueryBestSizeReply
+
+
 class QueryExtensionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.present, self.major_opcode, self.first_event, self.first_error = unpacker.unpack("xx2x4xBBBB")
+        self.present, self.major_opcode, self.first_event, self.first_error = unpacker.unpack(
+            "xx2x4xBBBB")
         self.bufsize = unpacker.offset - base
+
+
 class QueryExtensionCookie(xcffib.Cookie):
     reply_type = QueryExtensionReply
+
+
 class ListExtensionsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.names_len, = unpacker.unpack("xB2x4x24x")
         self.names = xcffib.List(unpacker, STR, self.names_len)
         self.bufsize = unpacker.offset - base
+
+
 class ListExtensionsCookie(xcffib.Cookie):
     reply_type = ListExtensionsReply
+
+
 class GetKeyboardMappingReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.keysyms_per_keycode, = unpacker.unpack("xB2x4x24x")
         self.keysyms = xcffib.List(unpacker, "I", self.length)
         self.bufsize = unpacker.offset - base
+
+
 class GetKeyboardMappingCookie(xcffib.Cookie):
     reply_type = GetKeyboardMappingReply
+
+
 class KB:
     KeyClickPercent = 1 << 0
     BellPercent = 1 << 1
     BellPitch = 1 << 2
     BellDuration = 1 << 3
     Led = 1 << 4
     LedMode = 1 << 5
     Key = 1 << 6
     AutoRepeatMode = 1 << 7
+
+
 class LedMode:
     Off = 0
     On = 1
+
+
 class AutoRepeatMode:
     Off = 0
     On = 1
     Default = 2
+
+
 class GetKeyboardControlReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.global_auto_repeat, self.led_mask, self.key_click_percent, self.bell_percent, self.bell_pitch, self.bell_duration = unpacker.unpack("xB2x4xIBBHH2x")
+        self.global_auto_repeat, self.led_mask, self.key_click_percent, self.bell_percent, self.bell_pitch, self.bell_duration = unpacker.unpack(
+            "xB2x4xIBBHH2x")
         self.auto_repeats = xcffib.List(unpacker, "B", 32)
         self.bufsize = unpacker.offset - base
+
+
 class GetKeyboardControlCookie(xcffib.Cookie):
     reply_type = GetKeyboardControlReply
+
+
 class GetPointerControlReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.acceleration_numerator, self.acceleration_denominator, self.threshold = unpacker.unpack("xx2x4xHHH18x")
+        self.acceleration_numerator, self.acceleration_denominator, self.threshold = unpacker.unpack(
+            "xx2x4xHHH18x")
         self.bufsize = unpacker.offset - base
+
+
 class GetPointerControlCookie(xcffib.Cookie):
     reply_type = GetPointerControlReply
+
+
 class Blanking:
     NotPreferred = 0
     Preferred = 1
     Default = 2
+
+
 class Exposures:
     NotAllowed = 0
     Allowed = 1
     Default = 2
+
+
 class GetScreenSaverReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.timeout, self.interval, self.prefer_blanking, self.allow_exposures = unpacker.unpack("xx2x4xHHBB18x")
+        self.timeout, self.interval, self.prefer_blanking, self.allow_exposures = unpacker.unpack(
+            "xx2x4xHHBB18x")
         self.bufsize = unpacker.offset - base
+
+
 class GetScreenSaverCookie(xcffib.Cookie):
     reply_type = GetScreenSaverReply
+
+
 class HostMode:
     Insert = 0
     Delete = 1
+
+
 class Family:
     Internet = 0
     DECnet = 1
     Chaos = 2
     ServerInterpreted = 5
     Internet6 = 6
+
+
 class HOST(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.family, self.address_len = unpacker.unpack("BxH")
         self.address = xcffib.List(unpacker, "B", self.address_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=BxH", self.family, self.address_len))
         buf.write(xcffib.pack_list(self.address, "B"))
         return buf.getvalue()
+
+
 class ListHostsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.mode, self.hosts_len = unpacker.unpack("xB2x4xH22x")
         self.hosts = xcffib.List(unpacker, HOST, self.hosts_len)
         self.bufsize = unpacker.offset - base
+
+
 class ListHostsCookie(xcffib.Cookie):
     reply_type = ListHostsReply
+
+
 class AccessControl:
     Disable = 0
     Enable = 1
+
+
 class CloseDown:
     DestroyAll = 0
     RetainPermanent = 1
     RetainTemporary = 2
+
+
 class Kill:
     AllTemporary = 0
+
+
 class ScreenSaver:
     Reset = 0
     Active = 1
+
+
 class MappingStatus:
     Success = 0
     Busy = 1
     Failure = 2
+
+
 class SetPointerMappingReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, = unpacker.unpack("xB2x4x")
         self.bufsize = unpacker.offset - base
+
+
 class SetPointerMappingCookie(xcffib.Cookie):
     reply_type = SetPointerMappingReply
+
+
 class GetPointerMappingReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.map_len, = unpacker.unpack("xB2x4x24x")
         self.map = xcffib.List(unpacker, "B", self.map_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetPointerMappingCookie(xcffib.Cookie):
     reply_type = GetPointerMappingReply
+
+
 class MapIndex:
     Shift = 0
     Lock = 1
     Control = 2
     _1 = 3
     _2 = 4
     _3 = 5
     _4 = 6
     _5 = 7
+
+
 class SetModifierMappingReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, = unpacker.unpack("xB2x4x")
         self.bufsize = unpacker.offset - base
+
+
 class SetModifierMappingCookie(xcffib.Cookie):
     reply_type = SetModifierMappingReply
+
+
 class GetModifierMappingReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.keycodes_per_modifier, = unpacker.unpack("xB2x4x24x")
-        self.keycodes = xcffib.List(unpacker, "B", self.keycodes_per_modifier * 8)
+        self.keycodes = xcffib.List(
+            unpacker,
+            "B",
+            self.keycodes_per_modifier *
+            8)
         self.bufsize = unpacker.offset - base
+
+
 class GetModifierMappingCookie(xcffib.Cookie):
     reply_type = GetModifierMappingReply
+
+
 class xprotoExtension(xcffib.Extension):
-    def CreateWindow(self, depth, wid, parent, x, y, width, height, border_width, _class, visual, value_mask, value_list, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xIIhhHHHHI", depth, wid, parent, x, y, width, height, border_width, _class, visual))
+
+    def CreateWindow(
+            self,
+            depth,
+            wid,
+            parent,
+            x,
+            y,
+            width,
+            height,
+            border_width,
+            _class,
+            visual,
+            value_mask,
+            value_list,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xIIhhHHHHI",
+                depth,
+                wid,
+                parent,
+                x,
+                y,
+                width,
+                height,
+                border_width,
+                _class,
+                visual))
         buf.write(struct.pack("=I", value_mask))
         buf.write(xcffib.pack_list(value_list, "I"))
         return self.send_request(1, buf, is_checked=is_checked)
-    def ChangeWindowAttributes(self, window, value_mask, value_list, is_checked=False):
+
+    def ChangeWindowAttributes(
+            self,
+            window,
+            value_mask,
+            value_list,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
         buf.write(struct.pack("=I", value_mask))
         buf.write(xcffib.pack_list(value_list, "I"))
         return self.send_request(2, buf, is_checked=is_checked)
+
     def GetWindowAttributes(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(3, buf, GetWindowAttributesCookie, is_checked=is_checked)
+        return self.send_request(
+            3,
+            buf,
+            GetWindowAttributesCookie,
+            is_checked=is_checked)
+
     def DestroyWindow(self, window, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
         return self.send_request(4, buf, is_checked=is_checked)
+
     def DestroySubwindows(self, window, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
         return self.send_request(5, buf, is_checked=is_checked)
+
     def ChangeSaveSet(self, mode, window, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xI", mode, window))
         return self.send_request(6, buf, is_checked=is_checked)
+
     def ReparentWindow(self, window, parent, x, y, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIhh", window, parent, x, y))
         return self.send_request(7, buf, is_checked=is_checked)
+
     def MapWindow(self, window, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
         return self.send_request(8, buf, is_checked=is_checked)
+
     def MapSubwindows(self, window, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
         return self.send_request(9, buf, is_checked=is_checked)
+
     def UnmapWindow(self, window, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
         return self.send_request(10, buf, is_checked=is_checked)
+
     def UnmapSubwindows(self, window, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
         return self.send_request(11, buf, is_checked=is_checked)
-    def ConfigureWindow(self, window, value_mask, value_list, is_checked=False):
+
+    def ConfigureWindow(
+            self,
+            window,
+            value_mask,
+            value_list,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIH2x", window, value_mask))
         buf.write(xcffib.pack_list(value_list, "I"))
         return self.send_request(12, buf, is_checked=is_checked)
+
     def CirculateWindow(self, direction, window, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xI", direction, window))
         return self.send_request(13, buf, is_checked=is_checked)
+
     def GetGeometry(self, drawable, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", drawable))
-        return self.send_request(14, buf, GetGeometryCookie, is_checked=is_checked)
+        return self.send_request(
+            14,
+            buf,
+            GetGeometryCookie,
+            is_checked=is_checked)
+
     def QueryTree(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(15, buf, QueryTreeCookie, is_checked=is_checked)
+        return self.send_request(
+            15,
+            buf,
+            QueryTreeCookie,
+            is_checked=is_checked)
+
     def InternAtom(self, only_if_exists, name_len, name, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xH2x", only_if_exists, name_len))
         buf.write(xcffib.pack_list(name, "c"))
-        return self.send_request(16, buf, InternAtomCookie, is_checked=is_checked)
+        return self.send_request(
+            16,
+            buf,
+            InternAtomCookie,
+            is_checked=is_checked)
+
     def GetAtomName(self, atom, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", atom))
-        return self.send_request(17, buf, GetAtomNameCookie, is_checked=is_checked)
-    def ChangeProperty(self, mode, window, property, type, format, data_len, data, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xIIIB3xI", mode, window, property, type, format, data_len))
+        return self.send_request(
+            17,
+            buf,
+            GetAtomNameCookie,
+            is_checked=is_checked)
+
+    def ChangeProperty(
+            self,
+            mode,
+            window,
+            property,
+            type,
+            format,
+            data_len,
+            data,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xIIIB3xI",
+                mode,
+                window,
+                property,
+                type,
+                format,
+                data_len))
         buf.write(xcffib.pack_list(data, "c"))
         return self.send_request(18, buf, is_checked=is_checked)
+
     def DeleteProperty(self, window, property, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", window, property))
         return self.send_request(19, buf, is_checked=is_checked)
-    def GetProperty(self, delete, window, property, type, long_offset, long_length, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xIIIII", delete, window, property, type, long_offset, long_length))
-        return self.send_request(20, buf, GetPropertyCookie, is_checked=is_checked)
+
+    def GetProperty(
+            self,
+            delete,
+            window,
+            property,
+            type,
+            long_offset,
+            long_length,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xIIIII",
+                delete,
+                window,
+                property,
+                type,
+                long_offset,
+                long_length))
+        return self.send_request(
+            20,
+            buf,
+            GetPropertyCookie,
+            is_checked=is_checked)
+
     def ListProperties(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(21, buf, ListPropertiesCookie, is_checked=is_checked)
+        return self.send_request(
+            21,
+            buf,
+            ListPropertiesCookie,
+            is_checked=is_checked)
+
     def SetSelectionOwner(self, owner, selection, time, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", owner, selection, time))
         return self.send_request(22, buf, is_checked=is_checked)
+
     def GetSelectionOwner(self, selection, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", selection))
-        return self.send_request(23, buf, GetSelectionOwnerCookie, is_checked=is_checked)
-    def ConvertSelection(self, requestor, selection, target, property, time, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIII", requestor, selection, target, property, time))
+        return self.send_request(
+            23,
+            buf,
+            GetSelectionOwnerCookie,
+            is_checked=is_checked)
+
+    def ConvertSelection(
+            self,
+            requestor,
+            selection,
+            target,
+            property,
+            time,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIII",
+                requestor,
+                selection,
+                target,
+                property,
+                time))
         return self.send_request(24, buf, is_checked=is_checked)
-    def SendEvent(self, propagate, destination, event_mask, event, is_checked=False):
+
+    def SendEvent(
+            self,
+            propagate,
+            destination,
+            event_mask,
+            event,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xII", propagate, destination, event_mask))
         buf.write(xcffib.pack_list(event, "c"))
         return self.send_request(25, buf, is_checked=is_checked)
-    def GrabPointer(self, owner_events, grab_window, event_mask, pointer_mode, keyboard_mode, confine_to, cursor, time, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xIHBBIII", owner_events, grab_window, event_mask, pointer_mode, keyboard_mode, confine_to, cursor, time))
-        return self.send_request(26, buf, GrabPointerCookie, is_checked=is_checked)
+
+    def GrabPointer(
+            self,
+            owner_events,
+            grab_window,
+            event_mask,
+            pointer_mode,
+            keyboard_mode,
+            confine_to,
+            cursor,
+            time,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xIHBBIII",
+                owner_events,
+                grab_window,
+                event_mask,
+                pointer_mode,
+                keyboard_mode,
+                confine_to,
+                cursor,
+                time))
+        return self.send_request(
+            26,
+            buf,
+            GrabPointerCookie,
+            is_checked=is_checked)
+
     def UngrabPointer(self, time, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", time))
         return self.send_request(27, buf, is_checked=is_checked)
-    def GrabButton(self, owner_events, grab_window, event_mask, pointer_mode, keyboard_mode, confine_to, cursor, button, modifiers, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xIHBBIIBxH", owner_events, grab_window, event_mask, pointer_mode, keyboard_mode, confine_to, cursor, button, modifiers))
+
+    def GrabButton(
+            self,
+            owner_events,
+            grab_window,
+            event_mask,
+            pointer_mode,
+            keyboard_mode,
+            confine_to,
+            cursor,
+            button,
+            modifiers,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xIHBBIIBxH",
+                owner_events,
+                grab_window,
+                event_mask,
+                pointer_mode,
+                keyboard_mode,
+                confine_to,
+                cursor,
+                button,
+                modifiers))
         return self.send_request(28, buf, is_checked=is_checked)
+
     def UngrabButton(self, button, grab_window, modifiers, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xIH2x", button, grab_window, modifiers))
         return self.send_request(29, buf, is_checked=is_checked)
-    def ChangeActivePointerGrab(self, cursor, time, event_mask, is_checked=False):
+
+    def ChangeActivePointerGrab(
+            self,
+            cursor,
+            time,
+            event_mask,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIH2x", cursor, time, event_mask))
         return self.send_request(30, buf, is_checked=is_checked)
-    def GrabKeyboard(self, owner_events, grab_window, time, pointer_mode, keyboard_mode, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xIIBB2x", owner_events, grab_window, time, pointer_mode, keyboard_mode))
-        return self.send_request(31, buf, GrabKeyboardCookie, is_checked=is_checked)
+
+    def GrabKeyboard(
+            self,
+            owner_events,
+            grab_window,
+            time,
+            pointer_mode,
+            keyboard_mode,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xIIBB2x",
+                owner_events,
+                grab_window,
+                time,
+                pointer_mode,
+                keyboard_mode))
+        return self.send_request(
+            31,
+            buf,
+            GrabKeyboardCookie,
+            is_checked=is_checked)
+
     def UngrabKeyboard(self, time, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", time))
         return self.send_request(32, buf, is_checked=is_checked)
-    def GrabKey(self, owner_events, grab_window, modifiers, key, pointer_mode, keyboard_mode, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xIHBBB3x", owner_events, grab_window, modifiers, key, pointer_mode, keyboard_mode))
+
+    def GrabKey(
+            self,
+            owner_events,
+            grab_window,
+            modifiers,
+            key,
+            pointer_mode,
+            keyboard_mode,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xIHBBB3x",
+                owner_events,
+                grab_window,
+                modifiers,
+                key,
+                pointer_mode,
+                keyboard_mode))
         return self.send_request(33, buf, is_checked=is_checked)
+
     def UngrabKey(self, key, grab_window, modifiers, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xIH2x", key, grab_window, modifiers))
         return self.send_request(34, buf, is_checked=is_checked)
+
     def AllowEvents(self, mode, time, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xI", mode, time))
         return self.send_request(35, buf, is_checked=is_checked)
+
     def GrabServer(self, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
         return self.send_request(36, buf, is_checked=is_checked)
+
     def UngrabServer(self, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
         return self.send_request(37, buf, is_checked=is_checked)
+
     def QueryPointer(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(38, buf, QueryPointerCookie, is_checked=is_checked)
+        return self.send_request(
+            38,
+            buf,
+            QueryPointerCookie,
+            is_checked=is_checked)
+
     def GetMotionEvents(self, window, start, stop, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", window, start, stop))
-        return self.send_request(39, buf, GetMotionEventsCookie, is_checked=is_checked)
-    def TranslateCoordinates(self, src_window, dst_window, src_x, src_y, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIhh", src_window, dst_window, src_x, src_y))
-        return self.send_request(40, buf, TranslateCoordinatesCookie, is_checked=is_checked)
-    def WarpPointer(self, src_window, dst_window, src_x, src_y, src_width, src_height, dst_x, dst_y, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIhhHHhh", src_window, dst_window, src_x, src_y, src_width, src_height, dst_x, dst_y))
+        return self.send_request(
+            39,
+            buf,
+            GetMotionEventsCookie,
+            is_checked=is_checked)
+
+    def TranslateCoordinates(
+            self,
+            src_window,
+            dst_window,
+            src_x,
+            src_y,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIhh",
+                src_window,
+                dst_window,
+                src_x,
+                src_y))
+        return self.send_request(
+            40,
+            buf,
+            TranslateCoordinatesCookie,
+            is_checked=is_checked)
+
+    def WarpPointer(
+            self,
+            src_window,
+            dst_window,
+            src_x,
+            src_y,
+            src_width,
+            src_height,
+            dst_x,
+            dst_y,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIhhHHhh",
+                src_window,
+                dst_window,
+                src_x,
+                src_y,
+                src_width,
+                src_height,
+                dst_x,
+                dst_y))
         return self.send_request(41, buf, is_checked=is_checked)
+
     def SetInputFocus(self, revert_to, focus, time, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xII", revert_to, focus, time))
         return self.send_request(42, buf, is_checked=is_checked)
+
     def GetInputFocus(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(43, buf, GetInputFocusCookie, is_checked=is_checked)
+        return self.send_request(
+            43,
+            buf,
+            GetInputFocusCookie,
+            is_checked=is_checked)
+
     def QueryKeymap(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(44, buf, QueryKeymapCookie, is_checked=is_checked)
+        return self.send_request(
+            44,
+            buf,
+            QueryKeymapCookie,
+            is_checked=is_checked)
+
     def OpenFont(self, fid, name_len, name, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIH2x", fid, name_len))
         buf.write(xcffib.pack_list(name, "c"))
         return self.send_request(45, buf, is_checked=is_checked)
+
     def CloseFont(self, font, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", font))
         return self.send_request(46, buf, is_checked=is_checked)
+
     def QueryFont(self, font, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", font))
-        return self.send_request(47, buf, QueryFontCookie, is_checked=is_checked)
+        return self.send_request(
+            47,
+            buf,
+            QueryFontCookie,
+            is_checked=is_checked)
+
     def QueryTextExtents(self, font, string_len, string, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", font))
         buf.write(struct.pack("=B", string_len & 1))
         buf.write(xcffib.pack_list(string, CHAR2B))
-        return self.send_request(48, buf, QueryTextExtentsCookie, is_checked=is_checked)
+        return self.send_request(
+            48,
+            buf,
+            QueryTextExtentsCookie,
+            is_checked=is_checked)
+
     def ListFonts(self, max_names, pattern_len, pattern, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xHH", max_names, pattern_len))
         buf.write(xcffib.pack_list(pattern, "c"))
-        return self.send_request(49, buf, ListFontsCookie, is_checked=is_checked)
-    def ListFontsWithInfo(self, max_names, pattern_len, pattern, is_checked=True):
+        return self.send_request(
+            49,
+            buf,
+            ListFontsCookie,
+            is_checked=is_checked)
+
+    def ListFontsWithInfo(
+            self,
+            max_names,
+            pattern_len,
+            pattern,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xHH", max_names, pattern_len))
         buf.write(xcffib.pack_list(pattern, "c"))
-        return self.send_request(50, buf, ListFontsWithInfoCookie, is_checked=is_checked)
+        return self.send_request(
+            50,
+            buf,
+            ListFontsWithInfoCookie,
+            is_checked=is_checked)
+
     def SetFontPath(self, font_qty, font, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2x", font_qty))
         buf.write(xcffib.pack_list(font, STR))
         return self.send_request(51, buf, is_checked=is_checked)
+
     def GetFontPath(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(52, buf, GetFontPathCookie, is_checked=is_checked)
-    def CreatePixmap(self, depth, pid, drawable, width, height, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xIIHH", depth, pid, drawable, width, height))
+        return self.send_request(
+            52,
+            buf,
+            GetFontPathCookie,
+            is_checked=is_checked)
+
+    def CreatePixmap(
+            self,
+            depth,
+            pid,
+            drawable,
+            width,
+            height,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xIIHH",
+                depth,
+                pid,
+                drawable,
+                width,
+                height))
         return self.send_request(53, buf, is_checked=is_checked)
+
     def FreePixmap(self, pixmap, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", pixmap))
         return self.send_request(54, buf, is_checked=is_checked)
-    def CreateGC(self, cid, drawable, value_mask, value_list, is_checked=False):
+
+    def CreateGC(
+            self,
+            cid,
+            drawable,
+            value_mask,
+            value_list,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", cid, drawable))
         buf.write(struct.pack("=I", value_mask))
         buf.write(xcffib.pack_list(value_list, "I"))
         return self.send_request(55, buf, is_checked=is_checked)
+
     def ChangeGC(self, gc, value_mask, value_list, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", gc))
         buf.write(struct.pack("=I", value_mask))
         buf.write(xcffib.pack_list(value_list, "I"))
         return self.send_request(56, buf, is_checked=is_checked)
+
     def CopyGC(self, src_gc, dst_gc, value_mask, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", src_gc, dst_gc, value_mask))
         return self.send_request(57, buf, is_checked=is_checked)
+
     def SetDashes(self, gc, dash_offset, dashes_len, dashes, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIHH", gc, dash_offset, dashes_len))
         buf.write(xcffib.pack_list(dashes, "B"))
         return self.send_request(58, buf, is_checked=is_checked)
-    def SetClipRectangles(self, ordering, gc, clip_x_origin, clip_y_origin, rectangles, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xIhh", ordering, gc, clip_x_origin, clip_y_origin))
+
+    def SetClipRectangles(
+            self,
+            ordering,
+            gc,
+            clip_x_origin,
+            clip_y_origin,
+            rectangles,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xIhh",
+                ordering,
+                gc,
+                clip_x_origin,
+                clip_y_origin))
         buf.write(xcffib.pack_list(rectangles, RECTANGLE))
         return self.send_request(59, buf, is_checked=is_checked)
+
     def FreeGC(self, gc, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", gc))
         return self.send_request(60, buf, is_checked=is_checked)
-    def ClearArea(self, exposures, window, x, y, width, height, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xIhhHH", exposures, window, x, y, width, height))
+
+    def ClearArea(
+            self,
+            exposures,
+            window,
+            x,
+            y,
+            width,
+            height,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xIhhHH",
+                exposures,
+                window,
+                x,
+                y,
+                width,
+                height))
         return self.send_request(61, buf, is_checked=is_checked)
-    def CopyArea(self, src_drawable, dst_drawable, gc, src_x, src_y, dst_x, dst_y, width, height, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIhhhhHH", src_drawable, dst_drawable, gc, src_x, src_y, dst_x, dst_y, width, height))
+
+    def CopyArea(
+            self,
+            src_drawable,
+            dst_drawable,
+            gc,
+            src_x,
+            src_y,
+            dst_x,
+            dst_y,
+            width,
+            height,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIhhhhHH",
+                src_drawable,
+                dst_drawable,
+                gc,
+                src_x,
+                src_y,
+                dst_x,
+                dst_y,
+                width,
+                height))
         return self.send_request(62, buf, is_checked=is_checked)
-    def CopyPlane(self, src_drawable, dst_drawable, gc, src_x, src_y, dst_x, dst_y, width, height, bit_plane, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIhhhhHHI", src_drawable, dst_drawable, gc, src_x, src_y, dst_x, dst_y, width, height, bit_plane))
+
+    def CopyPlane(
+            self,
+            src_drawable,
+            dst_drawable,
+            gc,
+            src_x,
+            src_y,
+            dst_x,
+            dst_y,
+            width,
+            height,
+            bit_plane,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIhhhhHHI",
+                src_drawable,
+                dst_drawable,
+                gc,
+                src_x,
+                src_y,
+                dst_x,
+                dst_y,
+                width,
+                height,
+                bit_plane))
         return self.send_request(63, buf, is_checked=is_checked)
-    def PolyPoint(self, coordinate_mode, drawable, gc, points, is_checked=False):
+
+    def PolyPoint(
+            self,
+            coordinate_mode,
+            drawable,
+            gc,
+            points,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xII", coordinate_mode, drawable, gc))
         buf.write(xcffib.pack_list(points, POINT))
         return self.send_request(64, buf, is_checked=is_checked)
-    def PolyLine(self, coordinate_mode, drawable, gc, points, is_checked=False):
+
+    def PolyLine(
+            self,
+            coordinate_mode,
+            drawable,
+            gc,
+            points,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xII", coordinate_mode, drawable, gc))
         buf.write(xcffib.pack_list(points, POINT))
         return self.send_request(65, buf, is_checked=is_checked)
+
     def PolySegment(self, drawable, gc, segments, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", drawable, gc))
         buf.write(xcffib.pack_list(segments, SEGMENT))
         return self.send_request(66, buf, is_checked=is_checked)
+
     def PolyRectangle(self, drawable, gc, rectangles, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", drawable, gc))
         buf.write(xcffib.pack_list(rectangles, RECTANGLE))
         return self.send_request(67, buf, is_checked=is_checked)
+
     def PolyArc(self, drawable, gc, arcs, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", drawable, gc))
         buf.write(xcffib.pack_list(arcs, ARC))
         return self.send_request(68, buf, is_checked=is_checked)
-    def FillPoly(self, drawable, gc, shape, coordinate_mode, points, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIBB2x", drawable, gc, shape, coordinate_mode))
+
+    def FillPoly(
+            self,
+            drawable,
+            gc,
+            shape,
+            coordinate_mode,
+            points,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIBB2x",
+                drawable,
+                gc,
+                shape,
+                coordinate_mode))
         buf.write(xcffib.pack_list(points, POINT))
         return self.send_request(69, buf, is_checked=is_checked)
+
     def PolyFillRectangle(self, drawable, gc, rectangles, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", drawable, gc))
         buf.write(xcffib.pack_list(rectangles, RECTANGLE))
         return self.send_request(70, buf, is_checked=is_checked)
+
     def PolyFillArc(self, drawable, gc, arcs, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", drawable, gc))
         buf.write(xcffib.pack_list(arcs, ARC))
         return self.send_request(71, buf, is_checked=is_checked)
-    def PutImage(self, format, drawable, gc, width, height, dst_x, dst_y, left_pad, depth, data, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xIIHHhhBB2x", format, drawable, gc, width, height, dst_x, dst_y, left_pad, depth))
+
+    def PutImage(
+            self,
+            format,
+            drawable,
+            gc,
+            width,
+            height,
+            dst_x,
+            dst_y,
+            left_pad,
+            depth,
+            data,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xIIHHhhBB2x",
+                format,
+                drawable,
+                gc,
+                width,
+                height,
+                dst_x,
+                dst_y,
+                left_pad,
+                depth))
         buf.write(xcffib.pack_list(data, "B"))
         return self.send_request(72, buf, is_checked=is_checked)
-    def GetImage(self, format, drawable, x, y, width, height, plane_mask, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xIhhHHI", format, drawable, x, y, width, height, plane_mask))
-        return self.send_request(73, buf, GetImageCookie, is_checked=is_checked)
+
+    def GetImage(
+            self,
+            format,
+            drawable,
+            x,
+            y,
+            width,
+            height,
+            plane_mask,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xIhhHHI",
+                format,
+                drawable,
+                x,
+                y,
+                width,
+                height,
+                plane_mask))
+        return self.send_request(
+            73,
+            buf,
+            GetImageCookie,
+            is_checked=is_checked)
+
     def PolyText8(self, drawable, gc, x, y, items, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIhh", drawable, gc, x, y))
         buf.write(xcffib.pack_list(items, "B"))
         return self.send_request(74, buf, is_checked=is_checked)
+
     def PolyText16(self, drawable, gc, x, y, items, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIhh", drawable, gc, x, y))
         buf.write(xcffib.pack_list(items, "B"))
         return self.send_request(75, buf, is_checked=is_checked)
-    def ImageText8(self, string_len, drawable, gc, x, y, string, is_checked=False):
+
+    def ImageText8(
+            self,
+            string_len,
+            drawable,
+            gc,
+            x,
+            y,
+            string,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xIIhh", string_len, drawable, gc, x, y))
         buf.write(xcffib.pack_list(string, "c"))
         return self.send_request(76, buf, is_checked=is_checked)
-    def ImageText16(self, string_len, drawable, gc, x, y, string, is_checked=False):
+
+    def ImageText16(
+            self,
+            string_len,
+            drawable,
+            gc,
+            x,
+            y,
+            string,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xIIhh", string_len, drawable, gc, x, y))
         buf.write(xcffib.pack_list(string, CHAR2B))
         return self.send_request(77, buf, is_checked=is_checked)
+
     def CreateColormap(self, alloc, mid, window, visual, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xIII", alloc, mid, window, visual))
         return self.send_request(78, buf, is_checked=is_checked)
+
     def FreeColormap(self, cmap, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", cmap))
         return self.send_request(79, buf, is_checked=is_checked)
+
     def CopyColormapAndFree(self, mid, src_cmap, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", mid, src_cmap))
         return self.send_request(80, buf, is_checked=is_checked)
+
     def InstallColormap(self, cmap, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", cmap))
         return self.send_request(81, buf, is_checked=is_checked)
+
     def UninstallColormap(self, cmap, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", cmap))
         return self.send_request(82, buf, is_checked=is_checked)
+
     def ListInstalledColormaps(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(83, buf, ListInstalledColormapsCookie, is_checked=is_checked)
+        return self.send_request(
+            83,
+            buf,
+            ListInstalledColormapsCookie,
+            is_checked=is_checked)
+
     def AllocColor(self, cmap, red, green, blue, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIHHH2x", cmap, red, green, blue))
-        return self.send_request(84, buf, AllocColorCookie, is_checked=is_checked)
+        return self.send_request(
+            84,
+            buf,
+            AllocColorCookie,
+            is_checked=is_checked)
+
     def AllocNamedColor(self, cmap, name_len, name, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIH2x", cmap, name_len))
         buf.write(xcffib.pack_list(name, "c"))
-        return self.send_request(85, buf, AllocNamedColorCookie, is_checked=is_checked)
-    def AllocColorCells(self, contiguous, cmap, colors, planes, is_checked=True):
+        return self.send_request(
+            85,
+            buf,
+            AllocNamedColorCookie,
+            is_checked=is_checked)
+
+    def AllocColorCells(
+            self,
+            contiguous,
+            cmap,
+            colors,
+            planes,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xIHH", contiguous, cmap, colors, planes))
-        return self.send_request(86, buf, AllocColorCellsCookie, is_checked=is_checked)
-    def AllocColorPlanes(self, contiguous, cmap, colors, reds, greens, blues, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xIHHHH", contiguous, cmap, colors, reds, greens, blues))
-        return self.send_request(87, buf, AllocColorPlanesCookie, is_checked=is_checked)
+        return self.send_request(
+            86,
+            buf,
+            AllocColorCellsCookie,
+            is_checked=is_checked)
+
+    def AllocColorPlanes(
+            self,
+            contiguous,
+            cmap,
+            colors,
+            reds,
+            greens,
+            blues,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xIHHHH",
+                contiguous,
+                cmap,
+                colors,
+                reds,
+                greens,
+                blues))
+        return self.send_request(
+            87,
+            buf,
+            AllocColorPlanesCookie,
+            is_checked=is_checked)
+
     def FreeColors(self, cmap, plane_mask, pixels, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", cmap, plane_mask))
         buf.write(xcffib.pack_list(pixels, "I"))
         return self.send_request(88, buf, is_checked=is_checked)
+
     def StoreColors(self, cmap, items, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", cmap))
         buf.write(xcffib.pack_list(items, COLORITEM))
         return self.send_request(89, buf, is_checked=is_checked)
-    def StoreNamedColor(self, flags, cmap, pixel, name_len, name, is_checked=False):
+
+    def StoreNamedColor(
+            self,
+            flags,
+            cmap,
+            pixel,
+            name_len,
+            name,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xIIH2x", flags, cmap, pixel, name_len))
         buf.write(xcffib.pack_list(name, "c"))
         return self.send_request(90, buf, is_checked=is_checked)
+
     def QueryColors(self, cmap, pixels, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", cmap))
         buf.write(xcffib.pack_list(pixels, "I"))
-        return self.send_request(91, buf, QueryColorsCookie, is_checked=is_checked)
+        return self.send_request(
+            91,
+            buf,
+            QueryColorsCookie,
+            is_checked=is_checked)
+
     def LookupColor(self, cmap, name_len, name, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIH2x", cmap, name_len))
         buf.write(xcffib.pack_list(name, "c"))
-        return self.send_request(92, buf, LookupColorCookie, is_checked=is_checked)
-    def CreateCursor(self, cid, source, mask, fore_red, fore_green, fore_blue, back_red, back_green, back_blue, x, y, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIHHHHHHHH", cid, source, mask, fore_red, fore_green, fore_blue, back_red, back_green, back_blue, x, y))
+        return self.send_request(
+            92,
+            buf,
+            LookupColorCookie,
+            is_checked=is_checked)
+
+    def CreateCursor(
+            self,
+            cid,
+            source,
+            mask,
+            fore_red,
+            fore_green,
+            fore_blue,
+            back_red,
+            back_green,
+            back_blue,
+            x,
+            y,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIHHHHHHHH",
+                cid,
+                source,
+                mask,
+                fore_red,
+                fore_green,
+                fore_blue,
+                back_red,
+                back_green,
+                back_blue,
+                x,
+                y))
         return self.send_request(93, buf, is_checked=is_checked)
-    def CreateGlyphCursor(self, cid, source_font, mask_font, source_char, mask_char, fore_red, fore_green, fore_blue, back_red, back_green, back_blue, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIHHHHHHHH", cid, source_font, mask_font, source_char, mask_char, fore_red, fore_green, fore_blue, back_red, back_green, back_blue))
+
+    def CreateGlyphCursor(
+            self,
+            cid,
+            source_font,
+            mask_font,
+            source_char,
+            mask_char,
+            fore_red,
+            fore_green,
+            fore_blue,
+            back_red,
+            back_green,
+            back_blue,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIHHHHHHHH",
+                cid,
+                source_font,
+                mask_font,
+                source_char,
+                mask_char,
+                fore_red,
+                fore_green,
+                fore_blue,
+                back_red,
+                back_green,
+                back_blue))
         return self.send_request(94, buf, is_checked=is_checked)
+
     def FreeCursor(self, cursor, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", cursor))
         return self.send_request(95, buf, is_checked=is_checked)
-    def RecolorCursor(self, cursor, fore_red, fore_green, fore_blue, back_red, back_green, back_blue, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIHHHHHH", cursor, fore_red, fore_green, fore_blue, back_red, back_green, back_blue))
+
+    def RecolorCursor(
+            self,
+            cursor,
+            fore_red,
+            fore_green,
+            fore_blue,
+            back_red,
+            back_green,
+            back_blue,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIHHHHHH",
+                cursor,
+                fore_red,
+                fore_green,
+                fore_blue,
+                back_red,
+                back_green,
+                back_blue))
         return self.send_request(96, buf, is_checked=is_checked)
+
     def QueryBestSize(self, _class, drawable, width, height, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xIHH", _class, drawable, width, height))
-        return self.send_request(97, buf, QueryBestSizeCookie, is_checked=is_checked)
+        return self.send_request(
+            97,
+            buf,
+            QueryBestSizeCookie,
+            is_checked=is_checked)
+
     def QueryExtension(self, name_len, name, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2x", name_len))
         buf.write(xcffib.pack_list(name, "c"))
-        return self.send_request(98, buf, QueryExtensionCookie, is_checked=is_checked)
+        return self.send_request(
+            98,
+            buf,
+            QueryExtensionCookie,
+            is_checked=is_checked)
+
     def ListExtensions(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(99, buf, ListExtensionsCookie, is_checked=is_checked)
-    def ChangeKeyboardMapping(self, keycode_count, first_keycode, keysyms_per_keycode, keysyms, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xBB2x", keycode_count, first_keycode, keysyms_per_keycode))
+        return self.send_request(
+            99,
+            buf,
+            ListExtensionsCookie,
+            is_checked=is_checked)
+
+    def ChangeKeyboardMapping(
+            self,
+            keycode_count,
+            first_keycode,
+            keysyms_per_keycode,
+            keysyms,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xBB2x",
+                keycode_count,
+                first_keycode,
+                keysyms_per_keycode))
         buf.write(xcffib.pack_list(keysyms, "I"))
         return self.send_request(100, buf, is_checked=is_checked)
+
     def GetKeyboardMapping(self, first_keycode, count, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xBB", first_keycode, count))
-        return self.send_request(101, buf, GetKeyboardMappingCookie, is_checked=is_checked)
+        return self.send_request(
+            101,
+            buf,
+            GetKeyboardMappingCookie,
+            is_checked=is_checked)
+
     def ChangeKeyboardControl(self, value_mask, value_list, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
         buf.write(struct.pack("=I", value_mask))
         buf.write(xcffib.pack_list(value_list, "I"))
         return self.send_request(102, buf, is_checked=is_checked)
+
     def GetKeyboardControl(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(103, buf, GetKeyboardControlCookie, is_checked=is_checked)
+        return self.send_request(
+            103,
+            buf,
+            GetKeyboardControlCookie,
+            is_checked=is_checked)
+
     def Bell(self, percent, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xb2x", percent))
         return self.send_request(104, buf, is_checked=is_checked)
-    def ChangePointerControl(self, acceleration_numerator, acceleration_denominator, threshold, do_acceleration, do_threshold, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xhhhBB", acceleration_numerator, acceleration_denominator, threshold, do_acceleration, do_threshold))
+
+    def ChangePointerControl(
+            self,
+            acceleration_numerator,
+            acceleration_denominator,
+            threshold,
+            do_acceleration,
+            do_threshold,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xhhhBB",
+                acceleration_numerator,
+                acceleration_denominator,
+                threshold,
+                do_acceleration,
+                do_threshold))
         return self.send_request(105, buf, is_checked=is_checked)
+
     def GetPointerControl(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(106, buf, GetPointerControlCookie, is_checked=is_checked)
-    def SetScreenSaver(self, timeout, interval, prefer_blanking, allow_exposures, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xhhBB", timeout, interval, prefer_blanking, allow_exposures))
+        return self.send_request(
+            106,
+            buf,
+            GetPointerControlCookie,
+            is_checked=is_checked)
+
+    def SetScreenSaver(
+            self,
+            timeout,
+            interval,
+            prefer_blanking,
+            allow_exposures,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xhhBB",
+                timeout,
+                interval,
+                prefer_blanking,
+                allow_exposures))
         return self.send_request(107, buf, is_checked=is_checked)
+
     def GetScreenSaver(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(108, buf, GetScreenSaverCookie, is_checked=is_checked)
-    def ChangeHosts(self, mode, family, address_len, address, is_checked=False):
+        return self.send_request(
+            108,
+            buf,
+            GetScreenSaverCookie,
+            is_checked=is_checked)
+
+    def ChangeHosts(
+            self,
+            mode,
+            family,
+            address_len,
+            address,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xBxH", mode, family, address_len))
         buf.write(xcffib.pack_list(address, "B"))
         return self.send_request(109, buf, is_checked=is_checked)
+
     def ListHosts(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(110, buf, ListHostsCookie, is_checked=is_checked)
+        return self.send_request(
+            110,
+            buf,
+            ListHostsCookie,
+            is_checked=is_checked)
+
     def SetAccessControl(self, mode, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x", mode))
         return self.send_request(111, buf, is_checked=is_checked)
+
     def SetCloseDownMode(self, mode, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x", mode))
         return self.send_request(112, buf, is_checked=is_checked)
+
     def KillClient(self, resource, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", resource))
         return self.send_request(113, buf, is_checked=is_checked)
-    def RotateProperties(self, window, atoms_len, delta, atoms, is_checked=False):
+
+    def RotateProperties(
+            self,
+            window,
+            atoms_len,
+            delta,
+            atoms,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIHh", window, atoms_len, delta))
         buf.write(xcffib.pack_list(atoms, "I"))
         return self.send_request(114, buf, is_checked=is_checked)
+
     def ForceScreenSaver(self, mode, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x", mode))
         return self.send_request(115, buf, is_checked=is_checked)
+
     def SetPointerMapping(self, map_len, map, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x", map_len))
         buf.write(xcffib.pack_list(map, "B"))
-        return self.send_request(116, buf, SetPointerMappingCookie, is_checked=is_checked)
+        return self.send_request(
+            116,
+            buf,
+            SetPointerMappingCookie,
+            is_checked=is_checked)
+
     def GetPointerMapping(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(117, buf, GetPointerMappingCookie, is_checked=is_checked)
-    def SetModifierMapping(self, keycodes_per_modifier, keycodes, is_checked=True):
+        return self.send_request(
+            117,
+            buf,
+            GetPointerMappingCookie,
+            is_checked=is_checked)
+
+    def SetModifierMapping(
+            self,
+            keycodes_per_modifier,
+            keycodes,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x", keycodes_per_modifier))
         buf.write(xcffib.pack_list(keycodes, "B"))
-        return self.send_request(118, buf, SetModifierMappingCookie, is_checked=is_checked)
+        return self.send_request(
+            118,
+            buf,
+            SetModifierMappingCookie,
+            is_checked=is_checked)
+
     def GetModifierMapping(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(119, buf, GetModifierMappingCookie, is_checked=is_checked)
+        return self.send_request(
+            119,
+            buf,
+            GetModifierMappingCookie,
+            is_checked=is_checked)
+
     def NoOperation(self, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
         return self.send_request(127, buf, is_checked=is_checked)
 xcffib._add_core(xprotoExtension, Setup, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/xc_misc.py` & `xcffib-v0.1.4/xcffib/xc_misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,46 +2,87 @@
 import struct
 import six
 MAJOR_VERSION = 1
 MINOR_VERSION = 1
 key = xcffib.ExtensionKey("XC-MISC")
 _events = {}
 _errors = {}
+
+
 class GetVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.server_major_version, self.server_minor_version = unpacker.unpack("xx2x4xHH")
+        self.server_major_version, self.server_minor_version = unpacker.unpack(
+            "xx2x4xHH")
         self.bufsize = unpacker.offset - base
+
+
 class GetVersionCookie(xcffib.Cookie):
     reply_type = GetVersionReply
+
+
 class GetXIDRangeReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.start_id, self.count = unpacker.unpack("xx2x4xII")
         self.bufsize = unpacker.offset - base
+
+
 class GetXIDRangeCookie(xcffib.Cookie):
     reply_type = GetXIDRangeReply
+
+
 class GetXIDListReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.ids_len, = unpacker.unpack("xx2x4xI20x")
         self.ids = xcffib.List(unpacker, "I", self.ids_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetXIDListCookie(xcffib.Cookie):
     reply_type = GetXIDListReply
+
+
 class xc_miscExtension(xcffib.Extension):
-    def GetVersion(self, client_major_version, client_minor_version, is_checked=True):
+
+    def GetVersion(
+            self,
+            client_major_version,
+            client_minor_version,
+            is_checked=True):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xHH", client_major_version, client_minor_version))
-        return self.send_request(0, buf, GetVersionCookie, is_checked=is_checked)
+        buf.write(
+            struct.pack(
+                "=xx2xHH",
+                client_major_version,
+                client_minor_version))
+        return self.send_request(
+            0,
+            buf,
+            GetVersionCookie,
+            is_checked=is_checked)
+
     def GetXIDRange(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(1, buf, GetXIDRangeCookie, is_checked=is_checked)
+        return self.send_request(
+            1,
+            buf,
+            GetXIDRangeCookie,
+            is_checked=is_checked)
+
     def GetXIDList(self, count, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", count))
-        return self.send_request(2, buf, GetXIDListCookie, is_checked=is_checked)
+        return self.send_request(
+            2,
+            buf,
+            GetXIDListCookie,
+            is_checked=is_checked)
 xcffib._add_ext(key, xc_miscExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/xevie.py` & `xcffib-v0.1.4/xcffib/xevie.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,84 +2,139 @@
 import struct
 import six
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
 key = xcffib.ExtensionKey("XEVIE")
 _events = {}
 _errors = {}
+
+
 class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.server_major_version, self.server_minor_version = unpacker.unpack("xx2x4xHH20x")
+        self.server_major_version, self.server_minor_version = unpacker.unpack(
+            "xx2x4xHH20x")
         self.bufsize = unpacker.offset - base
+
+
 class QueryVersionCookie(xcffib.Cookie):
     reply_type = QueryVersionReply
+
+
 class StartReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x24x")
         self.bufsize = unpacker.offset - base
+
+
 class StartCookie(xcffib.Cookie):
     reply_type = StartReply
+
+
 class EndReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x24x")
         self.bufsize = unpacker.offset - base
+
+
 class EndCookie(xcffib.Cookie):
     reply_type = EndReply
+
+
 class Datatype:
     Unmodified = 0
     Modified = 1
+
+
 class Event(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("32x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=32x"))
         return buf.getvalue()
     fixed_size = 32
+
+
 class SendReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x24x")
         self.bufsize = unpacker.offset - base
+
+
 class SendCookie(xcffib.Cookie):
     reply_type = SendReply
+
+
 class SelectInputReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x24x")
         self.bufsize = unpacker.offset - base
+
+
 class SelectInputCookie(xcffib.Cookie):
     reply_type = SelectInputReply
+
+
 class xevieExtension(xcffib.Extension):
-    def QueryVersion(self, client_major_version, client_minor_version, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xHH", client_major_version, client_minor_version))
-        return self.send_request(0, buf, QueryVersionCookie, is_checked=is_checked)
+
+    def QueryVersion(
+            self,
+            client_major_version,
+            client_minor_version,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xHH",
+                client_major_version,
+                client_minor_version))
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
     def Start(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", screen))
         return self.send_request(1, buf, StartCookie, is_checked=is_checked)
+
     def End(self, cmap, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", cmap))
         return self.send_request(2, buf, EndCookie, is_checked=is_checked)
+
     def Send(self, data_type, event, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI64x", data_type))
         buf.write(event.pack())
         return self.send_request(3, buf, SendCookie, is_checked=is_checked)
+
     def SelectInput(self, event_mask, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", event_mask))
-        return self.send_request(4, buf, SelectInputCookie, is_checked=is_checked)
+        return self.send_request(
+            4,
+            buf,
+            SelectInputCookie,
+            is_checked=is_checked)
 xcffib._add_ext(key, xevieExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/shape.py` & `xcffib-v0.1.4/xcffib/shm.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,220 @@
 import xcffib
 import struct
 import six
 MAJOR_VERSION = 1
-MINOR_VERSION = 1
-key = xcffib.ExtensionKey("SHAPE")
+MINOR_VERSION = 2
+key = xcffib.ExtensionKey("MIT-SHM")
 _events = {}
 _errors = {}
 from . import xproto
-class SO:
-    Set = 0
-    Union = 1
-    Intersect = 2
-    Subtract = 3
-    Invert = 4
-class SK:
-    Bounding = 0
-    Clip = 1
-    Input = 2
-class NotifyEvent(xcffib.Event):
+
+
+class CompletionEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.shape_kind, self.affected_window, self.extents_x, self.extents_y, self.extents_width, self.extents_height, self.server_time, self.shaped = unpacker.unpack("xB2xIhhHHIB11x")
+        self.drawable, self.minor_event, self.major_event, self.shmseg, self.offset = unpacker.unpack(
+            "xx2xIHBxII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIhhHHIB11x", self.shape_kind, self.affected_window, self.extents_x, self.extents_y, self.extents_width, self.extents_height, self.server_time, self.shaped))
+        buf.write(
+            struct.pack(
+                "=xIHBxII",
+                self.drawable,
+                self.minor_event,
+                self.major_event,
+                self.shmseg,
+                self.offset))
         return buf.getvalue()
-_events[0] = NotifyEvent
-class QueryVersionReply(xcffib.Reply):
+_events[0] = CompletionEvent
+
+
+class BadSegError(xcffib.Error):
+
     def __init__(self, unpacker):
-        xcffib.Reply.__init__(self, unpacker)
+        xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.major_version, self.minor_version = unpacker.unpack("xx2x4xHH")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHBx")
         self.bufsize = unpacker.offset - base
-class QueryVersionCookie(xcffib.Cookie):
-    reply_type = QueryVersionReply
-class QueryExtentsReply(xcffib.Reply):
+
+    def pack(self):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=IHBx",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
+        return buf.getvalue()
+BadBadSeg = BadSegError
+_errors[0] = BadSegError
+
+
+class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.bounding_shaped, self.clip_shaped, self.bounding_shape_extents_x, self.bounding_shape_extents_y, self.bounding_shape_extents_width, self.bounding_shape_extents_height, self.clip_shape_extents_x, self.clip_shape_extents_y, self.clip_shape_extents_width, self.clip_shape_extents_height = unpacker.unpack("xx2x4xBB2xhhHHhhHH")
+        self.shared_pixmaps, self.major_version, self.minor_version, self.uid, self.gid, self.pixmap_format = unpacker.unpack(
+            "xB2x4xHHHHB15x")
         self.bufsize = unpacker.offset - base
-class QueryExtentsCookie(xcffib.Cookie):
-    reply_type = QueryExtentsReply
-class InputSelectedReply(xcffib.Reply):
+
+
+class QueryVersionCookie(xcffib.Cookie):
+    reply_type = QueryVersionReply
+
+
+class GetImageReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.enabled, = unpacker.unpack("xB2x4x")
+        self.depth, self.visual, self.size = unpacker.unpack("xB2x4xII")
         self.bufsize = unpacker.offset - base
-class InputSelectedCookie(xcffib.Cookie):
-    reply_type = InputSelectedReply
-class GetRectanglesReply(xcffib.Reply):
+
+
+class GetImageCookie(xcffib.Cookie):
+    reply_type = GetImageReply
+
+
+class CreateSegmentReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.ordering, self.rectangles_len = unpacker.unpack("xB2x4xI20x")
-        self.rectangles = xcffib.List(unpacker, xproto.RECTANGLE, self.rectangles_len)
+        self.nfd, = unpacker.unpack("xB2x4x24x")
         self.bufsize = unpacker.offset - base
-class GetRectanglesCookie(xcffib.Cookie):
-    reply_type = GetRectanglesReply
-class shapeExtension(xcffib.Extension):
+
+
+class CreateSegmentCookie(xcffib.Cookie):
+    reply_type = CreateSegmentReply
+
+
+class shmExtension(xcffib.Extension):
+
     def QueryVersion(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(0, buf, QueryVersionCookie, is_checked=is_checked)
-    def Rectangles(self, operation, destination_kind, ordering, destination_window, x_offset, y_offset, rectangles, is_checked=False):
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
+    def Attach(self, shmseg, shmid, read_only, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xBBxIhh", operation, destination_kind, ordering, destination_window, x_offset, y_offset))
-        buf.write(xcffib.pack_list(rectangles, xproto.RECTANGLE))
+        buf.write(struct.pack("=xx2xIIB3x", shmseg, shmid, read_only))
         return self.send_request(1, buf, is_checked=is_checked)
-    def Mask(self, operation, destination_kind, destination_window, x_offset, y_offset, source_bitmap, is_checked=False):
+
+    def Detach(self, shmseg, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xB2xIhhI", operation, destination_kind, destination_window, x_offset, y_offset, source_bitmap))
+        buf.write(struct.pack("=xx2xI", shmseg))
         return self.send_request(2, buf, is_checked=is_checked)
-    def Combine(self, operation, destination_kind, source_kind, destination_window, x_offset, y_offset, source_window, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xBBxIhhI", operation, destination_kind, source_kind, destination_window, x_offset, y_offset, source_window))
+
+    def PutImage(
+            self,
+            drawable,
+            gc,
+            total_width,
+            total_height,
+            src_x,
+            src_y,
+            src_width,
+            src_height,
+            dst_x,
+            dst_y,
+            depth,
+            format,
+            send_event,
+            shmseg,
+            offset,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIHHHHHHhhBBBxII",
+                drawable,
+                gc,
+                total_width,
+                total_height,
+                src_x,
+                src_y,
+                src_width,
+                src_height,
+                dst_x,
+                dst_y,
+                depth,
+                format,
+                send_event,
+                shmseg,
+                offset))
         return self.send_request(3, buf, is_checked=is_checked)
-    def Offset(self, destination_kind, destination_window, x_offset, y_offset, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2x3xIhh", destination_kind, destination_window, x_offset, y_offset))
-        return self.send_request(4, buf, is_checked=is_checked)
-    def QueryExtents(self, destination_window, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", destination_window))
-        return self.send_request(5, buf, QueryExtentsCookie, is_checked=is_checked)
-    def SelectInput(self, destination_window, enable, is_checked=False):
+
+    def GetImage(
+            self,
+            drawable,
+            x,
+            y,
+            width,
+            height,
+            plane_mask,
+            format,
+            shmseg,
+            offset,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIhhHHIB3xII",
+                drawable,
+                x,
+                y,
+                width,
+                height,
+                plane_mask,
+                format,
+                shmseg,
+                offset))
+        return self.send_request(4, buf, GetImageCookie, is_checked=is_checked)
+
+    def CreatePixmap(
+            self,
+            pid,
+            drawable,
+            width,
+            height,
+            depth,
+            shmseg,
+            offset,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIHHB3xII",
+                pid,
+                drawable,
+                width,
+                height,
+                depth,
+                shmseg,
+                offset))
+        return self.send_request(5, buf, is_checked=is_checked)
+
+    def AttachFd(self, shmseg, read_only, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIB3x", destination_window, enable))
+        buf.write(struct.pack("=xx2xIB3x", shmseg, read_only))
         return self.send_request(6, buf, is_checked=is_checked)
-    def InputSelected(self, destination_window, is_checked=True):
+
+    def CreateSegment(self, shmseg, size, read_only, is_checked=True):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", destination_window))
-        return self.send_request(7, buf, InputSelectedCookie, is_checked=is_checked)
-    def GetRectangles(self, window, source_kind, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIB3x", window, source_kind))
-        return self.send_request(8, buf, GetRectanglesCookie, is_checked=is_checked)
-xcffib._add_ext(key, shapeExtension, _events, _errors)
+        buf.write(struct.pack("=xx2xIIB3x", shmseg, size, read_only))
+        return self.send_request(
+            7,
+            buf,
+            CreateSegmentCookie,
+            is_checked=is_checked)
+xcffib._add_ext(key, shmExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/bigreq.py` & `xcffib-v0.1.4/xcffib/bigreq.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,21 +2,29 @@
 import struct
 import six
 MAJOR_VERSION = 0
 MINOR_VERSION = 0
 key = xcffib.ExtensionKey("BIG-REQUESTS")
 _events = {}
 _errors = {}
+
+
 class EnableReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.maximum_request_length, = unpacker.unpack("xx2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class EnableCookie(xcffib.Cookie):
     reply_type = EnableReply
+
+
 class bigreqExtension(xcffib.Extension):
+
     def Enable(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
         return self.send_request(0, buf, EnableCookie, is_checked=is_checked)
 xcffib._add_ext(key, bigreqExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/screensaver.py` & `xcffib-v0.1.4/xcffib/screensaver.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,74 +3,153 @@
 import six
 MAJOR_VERSION = 1
 MINOR_VERSION = 1
 key = xcffib.ExtensionKey("MIT-SCREEN-SAVER")
 _events = {}
 _errors = {}
 from . import xproto
+
+
 class Kind:
     Blanked = 0
     Internal = 1
     External = 2
+
+
 class Event:
     NotifyMask = 1 << 0
     CycleMask = 1 << 1
+
+
 class State:
     Off = 0
     On = 1
     Cycle = 2
     Disabled = 3
+
+
 class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.server_major_version, self.server_minor_version = unpacker.unpack("xx2x4xHH20x")
+        self.server_major_version, self.server_minor_version = unpacker.unpack(
+            "xx2x4xHH20x")
         self.bufsize = unpacker.offset - base
+
+
 class QueryVersionCookie(xcffib.Cookie):
     reply_type = QueryVersionReply
+
+
 class QueryInfoReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.state, self.saver_window, self.ms_until_server, self.ms_since_user_input, self.event_mask, self.kind = unpacker.unpack("xB2x4xIIIIB7x")
+        self.state, self.saver_window, self.ms_until_server, self.ms_since_user_input, self.event_mask, self.kind = unpacker.unpack(
+            "xB2x4xIIIIB7x")
         self.bufsize = unpacker.offset - base
+
+
 class QueryInfoCookie(xcffib.Cookie):
     reply_type = QueryInfoReply
+
+
 class NotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.state, self.time, self.root, self.window, self.kind, self.forced = unpacker.unpack("xB2xIIIBB14x")
+        self.state, self.time, self.root, self.window, self.kind, self.forced = unpacker.unpack(
+            "xB2xIIIBB14x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIBB14x", self.state, self.time, self.root, self.window, self.kind, self.forced))
+        buf.write(
+            struct.pack(
+                "=BIIIBB14x",
+                self.state,
+                self.time,
+                self.root,
+                self.window,
+                self.kind,
+                self.forced))
         return buf.getvalue()
 _events[0] = NotifyEvent
+
+
 class screensaverExtension(xcffib.Extension):
-    def QueryVersion(self, client_major_version, client_minor_version, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xB2x", client_major_version, client_minor_version))
-        return self.send_request(0, buf, QueryVersionCookie, is_checked=is_checked)
+
+    def QueryVersion(
+            self,
+            client_major_version,
+            client_minor_version,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xB2x",
+                client_major_version,
+                client_minor_version))
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
     def QueryInfo(self, drawable, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", drawable))
-        return self.send_request(1, buf, QueryInfoCookie, is_checked=is_checked)
+        return self.send_request(
+            1,
+            buf,
+            QueryInfoCookie,
+            is_checked=is_checked)
+
     def SelectInput(self, drawable, event_mask, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", drawable, event_mask))
         return self.send_request(2, buf, is_checked=is_checked)
-    def SetAttributes(self, drawable, x, y, width, height, border_width, _class, depth, visual, value_mask, value_list, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIhhHHHBBI", drawable, x, y, width, height, border_width, _class, depth, visual))
+
+    def SetAttributes(
+            self,
+            drawable,
+            x,
+            y,
+            width,
+            height,
+            border_width,
+            _class,
+            depth,
+            visual,
+            value_mask,
+            value_list,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIhhHHHBBI",
+                drawable,
+                x,
+                y,
+                width,
+                height,
+                border_width,
+                _class,
+                depth,
+                visual))
         buf.write(struct.pack("=I", value_mask))
         buf.write(xcffib.pack_list(value_list, "I"))
         return self.send_request(3, buf, is_checked=is_checked)
+
     def UnsetAttributes(self, drawable, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", drawable))
         return self.send_request(4, buf, is_checked=is_checked)
+
     def Suspend(self, suspend, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x3x", suspend))
         return self.send_request(5, buf, is_checked=is_checked)
 xcffib._add_ext(key, screensaverExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/xinput.py` & `xcffib-v0.1.4/xcffib/xinput.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,830 +4,1475 @@
 MAJOR_VERSION = 2
 MINOR_VERSION = 3
 key = xcffib.ExtensionKey("XInputExtension")
 _events = {}
 _errors = {}
 from . import xfixes
 from . import xproto
+
+
 class FP3232(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.integral, self.frac = unpacker.unpack("iI")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=iI", self.integral, self.frac))
         return buf.getvalue()
     fixed_size = 8
+
+
 class GetExtensionVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.server_major, self.server_minor, self.present = unpacker.unpack("xx2x4xHHB19x")
+        self.server_major, self.server_minor, self.present = unpacker.unpack(
+            "xx2x4xHHB19x")
         self.bufsize = unpacker.offset - base
+
+
 class GetExtensionVersionCookie(xcffib.Cookie):
     reply_type = GetExtensionVersionReply
+
+
 class DeviceUse:
     IsXPointer = 0
     IsXKeyboard = 1
     IsXExtensionDevice = 2
     IsXExtensionKeyboard = 3
     IsXExtensionPointer = 4
+
+
 class InputClass:
     Key = 0
     Button = 1
     Valuator = 2
     Feedback = 3
     Proximity = 4
     Focus = 5
     Other = 6
+
+
 class ValuatorMode:
     Relative = 0
     Absolute = 1
+
+
 class DeviceInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.device_type, self.device_id, self.num_class_info, self.device_use = unpacker.unpack("IBBBx")
+        self.device_type, self.device_id, self.num_class_info, self.device_use = unpacker.unpack(
+            "IBBBx")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IBBBx", self.device_type, self.device_id, self.num_class_info, self.device_use))
+        buf.write(
+            struct.pack(
+                "=IBBBx",
+                self.device_type,
+                self.device_id,
+                self.num_class_info,
+                self.device_use))
         return buf.getvalue()
     fixed_size = 8
+
+
 class KeyInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.class_id, self.len, self.min_keycode, self.max_keycode, self.num_keys = unpacker.unpack("BBBBH2x")
+        self.class_id, self.len, self.min_keycode, self.max_keycode, self.num_keys = unpacker.unpack(
+            "BBBBH2x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBBBH2x", self.class_id, self.len, self.min_keycode, self.max_keycode, self.num_keys))
+        buf.write(
+            struct.pack(
+                "=BBBBH2x",
+                self.class_id,
+                self.len,
+                self.min_keycode,
+                self.max_keycode,
+                self.num_keys))
         return buf.getvalue()
     fixed_size = 8
+
+
 class ButtonInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.class_id, self.len, self.num_buttons = unpacker.unpack("BBH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBH", self.class_id, self.len, self.num_buttons))
+        buf.write(
+            struct.pack(
+                "=BBH",
+                self.class_id,
+                self.len,
+                self.num_buttons))
         return buf.getvalue()
     fixed_size = 4
+
+
 class AxisInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.resolution, self.minimum, self.maximum = unpacker.unpack("Iii")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=Iii", self.resolution, self.minimum, self.maximum))
+        buf.write(
+            struct.pack(
+                "=Iii",
+                self.resolution,
+                self.minimum,
+                self.maximum))
         return buf.getvalue()
     fixed_size = 12
+
+
 class ValuatorInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.class_id, self.len, self.axes_len, self.mode, self.motion_size = unpacker.unpack("BBBBI")
+        self.class_id, self.len, self.axes_len, self.mode, self.motion_size = unpacker.unpack(
+            "BBBBI")
         self.axes = xcffib.List(unpacker, AxisInfo, self.axes_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBBBI", self.class_id, self.len, self.axes_len, self.mode, self.motion_size))
+        buf.write(
+            struct.pack(
+                "=BBBBI",
+                self.class_id,
+                self.len,
+                self.axes_len,
+                self.mode,
+                self.motion_size))
         buf.write(xcffib.pack_list(self.axes, AxisInfo))
         return buf.getvalue()
+
+
 class InputInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.class_id, self.len = unpacker.unpack("BB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=BB", self.class_id, self.len))
         return buf.getvalue()
     fixed_size = 2
+
+
 class DeviceName(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.len, = unpacker.unpack("B")
         self.string = xcffib.List(unpacker, "c", self.len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=B", self.len))
         buf.write(xcffib.pack_list(self.string, "c"))
         return buf.getvalue()
+
+
 class ListInputDevicesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.devices_len, = unpacker.unpack("xx2x4xB23x")
         self.devices = xcffib.List(unpacker, DeviceInfo, self.devices_len)
         self.bufsize = unpacker.offset - base
+
+
 class ListInputDevicesCookie(xcffib.Cookie):
     reply_type = ListInputDevicesReply
+
+
 class InputClassInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.class_id, self.event_type_base = unpacker.unpack("BB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=BB", self.class_id, self.event_type_base))
         return buf.getvalue()
     fixed_size = 2
+
+
 class OpenDeviceReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_classes, = unpacker.unpack("xx2x4xB23x")
-        self.class_info = xcffib.List(unpacker, InputClassInfo, self.num_classes)
+        self.class_info = xcffib.List(
+            unpacker,
+            InputClassInfo,
+            self.num_classes)
         self.bufsize = unpacker.offset - base
+
+
 class OpenDeviceCookie(xcffib.Cookie):
     reply_type = OpenDeviceReply
+
+
 class SetDeviceModeReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, = unpacker.unpack("xx2x4xB23x")
         self.bufsize = unpacker.offset - base
+
+
 class SetDeviceModeCookie(xcffib.Cookie):
     reply_type = SetDeviceModeReply
+
+
 class GetSelectedExtensionEventsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.num_this_classes, self.num_all_classes = unpacker.unpack("xx2x4xHH20x")
+        self.num_this_classes, self.num_all_classes = unpacker.unpack(
+            "xx2x4xHH20x")
         self.this_classes = xcffib.List(unpacker, "I", self.num_this_classes)
         unpacker.pad("I")
         self.all_classes = xcffib.List(unpacker, "I", self.num_all_classes)
         self.bufsize = unpacker.offset - base
+
+
 class GetSelectedExtensionEventsCookie(xcffib.Cookie):
     reply_type = GetSelectedExtensionEventsReply
+
+
 class PropagateMode:
     AddToList = 0
     DeleteFromList = 1
+
+
 class GetDeviceDontPropagateListReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_classes, = unpacker.unpack("xx2x4xH22x")
         self.classes = xcffib.List(unpacker, "I", self.num_classes)
         self.bufsize = unpacker.offset - base
+
+
 class GetDeviceDontPropagateListCookie(xcffib.Cookie):
     reply_type = GetDeviceDontPropagateListReply
+
+
 class DeviceTimeCoord(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.time, = unpacker.unpack("I")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=I", self.time))
         return buf.getvalue()
     fixed_size = 4
+
+
 class GetDeviceMotionEventsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.num_events, self.num_axes, self.device_mode = unpacker.unpack("xx2x4xIBB18x")
+        self.num_events, self.num_axes, self.device_mode = unpacker.unpack(
+            "xx2x4xIBB18x")
         self.bufsize = unpacker.offset - base
+
+
 class GetDeviceMotionEventsCookie(xcffib.Cookie):
     reply_type = GetDeviceMotionEventsReply
+
+
 class ChangeKeyboardDeviceReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, = unpacker.unpack("xx2x4xB23x")
         self.bufsize = unpacker.offset - base
+
+
 class ChangeKeyboardDeviceCookie(xcffib.Cookie):
     reply_type = ChangeKeyboardDeviceReply
+
+
 class ChangePointerDeviceReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, = unpacker.unpack("xx2x4xB23x")
         self.bufsize = unpacker.offset - base
+
+
 class ChangePointerDeviceCookie(xcffib.Cookie):
     reply_type = ChangePointerDeviceReply
+
+
 class GrabDeviceReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, = unpacker.unpack("xx2x4xB23x")
         self.bufsize = unpacker.offset - base
+
+
 class GrabDeviceCookie(xcffib.Cookie):
     reply_type = GrabDeviceReply
+
+
 class DeviceInputMode:
     AsyncThisDevice = 0
     SyncThisDevice = 1
     ReplayThisDevice = 2
     AsyncOtherDevices = 3
     AsyncAll = 4
     SyncAll = 5
+
+
 class GetDeviceFocusReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.focus, self.time, self.revert_to = unpacker.unpack("xx2x4xIIB15x")
         self.bufsize = unpacker.offset - base
+
+
 class GetDeviceFocusCookie(xcffib.Cookie):
     reply_type = GetDeviceFocusReply
+
+
 class FeedbackClass:
     Keyboard = 0
     Pointer = 1
     String = 2
     Integer = 3
     Led = 4
     Bell = 5
+
+
 class KbdFeedbackState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.class_id, self.feedback_id, self.len, self.pitch, self.duration, self.led_mask, self.led_values, self.global_auto_repeat, self.click, self.percent = unpacker.unpack("BBHHHIIBBBx")
+        self.class_id, self.feedback_id, self.len, self.pitch, self.duration, self.led_mask, self.led_values, self.global_auto_repeat, self.click, self.percent = unpacker.unpack(
+            "BBHHHIIBBBx")
         self.auto_repeats = xcffib.List(unpacker, "B", 32)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBHHHIIBBBx", self.class_id, self.feedback_id, self.len, self.pitch, self.duration, self.led_mask, self.led_values, self.global_auto_repeat, self.click, self.percent))
+        buf.write(
+            struct.pack(
+                "=BBHHHIIBBBx",
+                self.class_id,
+                self.feedback_id,
+                self.len,
+                self.pitch,
+                self.duration,
+                self.led_mask,
+                self.led_values,
+                self.global_auto_repeat,
+                self.click,
+                self.percent))
         buf.write(xcffib.pack_list(self.auto_repeats, "B"))
         return buf.getvalue()
     fixed_size = 52
+
+
 class PtrFeedbackState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.class_id, self.feedback_id, self.len, self.accel_num, self.accel_denom, self.threshold = unpacker.unpack("BBH2xHHH")
+        self.class_id, self.feedback_id, self.len, self.accel_num, self.accel_denom, self.threshold = unpacker.unpack(
+            "BBH2xHHH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBH2xHHH", self.class_id, self.feedback_id, self.len, self.accel_num, self.accel_denom, self.threshold))
+        buf.write(
+            struct.pack(
+                "=BBH2xHHH",
+                self.class_id,
+                self.feedback_id,
+                self.len,
+                self.accel_num,
+                self.accel_denom,
+                self.threshold))
         return buf.getvalue()
     fixed_size = 12
+
+
 class IntegerFeedbackState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.class_id, self.feedback_id, self.len, self.resolution, self.min_value, self.max_value = unpacker.unpack("BBHIii")
+        self.class_id, self.feedback_id, self.len, self.resolution, self.min_value, self.max_value = unpacker.unpack(
+            "BBHIii")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBHIii", self.class_id, self.feedback_id, self.len, self.resolution, self.min_value, self.max_value))
+        buf.write(
+            struct.pack(
+                "=BBHIii",
+                self.class_id,
+                self.feedback_id,
+                self.len,
+                self.resolution,
+                self.min_value,
+                self.max_value))
         return buf.getvalue()
     fixed_size = 16
+
+
 class StringFeedbackState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.class_id, self.feedback_id, self.len, self.max_symbols, self.num_keysyms = unpacker.unpack("BBHHH")
+        self.class_id, self.feedback_id, self.len, self.max_symbols, self.num_keysyms = unpacker.unpack(
+            "BBHHH")
         self.keysyms = xcffib.List(unpacker, "I", self.num_keysyms)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBHHH", self.class_id, self.feedback_id, self.len, self.max_symbols, self.num_keysyms))
+        buf.write(
+            struct.pack(
+                "=BBHHH",
+                self.class_id,
+                self.feedback_id,
+                self.len,
+                self.max_symbols,
+                self.num_keysyms))
         buf.write(xcffib.pack_list(self.keysyms, "I"))
         return buf.getvalue()
+
+
 class BellFeedbackState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.class_id, self.feedback_id, self.len, self.percent, self.pitch, self.duration = unpacker.unpack("BBHB3xHH")
+        self.class_id, self.feedback_id, self.len, self.percent, self.pitch, self.duration = unpacker.unpack(
+            "BBHB3xHH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBHB3xHH", self.class_id, self.feedback_id, self.len, self.percent, self.pitch, self.duration))
+        buf.write(
+            struct.pack(
+                "=BBHB3xHH",
+                self.class_id,
+                self.feedback_id,
+                self.len,
+                self.percent,
+                self.pitch,
+                self.duration))
         return buf.getvalue()
     fixed_size = 12
+
+
 class LedFeedbackState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.class_id, self.feedback_id, self.len, self.led_mask, self.led_values = unpacker.unpack("BBHII")
+        self.class_id, self.feedback_id, self.len, self.led_mask, self.led_values = unpacker.unpack(
+            "BBHII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBHII", self.class_id, self.feedback_id, self.len, self.led_mask, self.led_values))
+        buf.write(
+            struct.pack(
+                "=BBHII",
+                self.class_id,
+                self.feedback_id,
+                self.len,
+                self.led_mask,
+                self.led_values))
         return buf.getvalue()
     fixed_size = 12
+
+
 class FeedbackState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.class_id, self.feedback_id, self.len = unpacker.unpack("BBH")
         self.uninterpreted_data = xcffib.List(unpacker, "B", self.len - 4)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBH", self.class_id, self.feedback_id, self.len))
+        buf.write(
+            struct.pack(
+                "=BBH",
+                self.class_id,
+                self.feedback_id,
+                self.len))
         buf.write(xcffib.pack_list(self.uninterpreted_data, "B"))
         return buf.getvalue()
+
+
 class GetFeedbackControlReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_feedbacks, = unpacker.unpack("xx2x4xH22x")
-        self.feedbacks = xcffib.List(unpacker, FeedbackState, self.num_feedbacks)
+        self.feedbacks = xcffib.List(
+            unpacker,
+            FeedbackState,
+            self.num_feedbacks)
         self.bufsize = unpacker.offset - base
+
+
 class GetFeedbackControlCookie(xcffib.Cookie):
     reply_type = GetFeedbackControlReply
+
+
 class KbdFeedbackCtl(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.class_id, self.feedback_id, self.len, self.key, self.auto_repeat_mode, self.key_click_percent, self.bell_percent, self.bell_pitch, self.bell_duration, self.led_mask, self.led_values = unpacker.unpack("BBHBBbbhhII")
+        self.class_id, self.feedback_id, self.len, self.key, self.auto_repeat_mode, self.key_click_percent, self.bell_percent, self.bell_pitch, self.bell_duration, self.led_mask, self.led_values = unpacker.unpack(
+            "BBHBBbbhhII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBHBBbbhhII", self.class_id, self.feedback_id, self.len, self.key, self.auto_repeat_mode, self.key_click_percent, self.bell_percent, self.bell_pitch, self.bell_duration, self.led_mask, self.led_values))
+        buf.write(
+            struct.pack(
+                "=BBHBBbbhhII",
+                self.class_id,
+                self.feedback_id,
+                self.len,
+                self.key,
+                self.auto_repeat_mode,
+                self.key_click_percent,
+                self.bell_percent,
+                self.bell_pitch,
+                self.bell_duration,
+                self.led_mask,
+                self.led_values))
         return buf.getvalue()
     fixed_size = 20
+
+
 class PtrFeedbackCtl(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.class_id, self.feedback_id, self.len, self.num, self.denom, self.threshold = unpacker.unpack("BBH2xhhh")
+        self.class_id, self.feedback_id, self.len, self.num, self.denom, self.threshold = unpacker.unpack(
+            "BBH2xhhh")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBH2xhhh", self.class_id, self.feedback_id, self.len, self.num, self.denom, self.threshold))
+        buf.write(
+            struct.pack(
+                "=BBH2xhhh",
+                self.class_id,
+                self.feedback_id,
+                self.len,
+                self.num,
+                self.denom,
+                self.threshold))
         return buf.getvalue()
     fixed_size = 12
+
+
 class IntegerFeedbackCtl(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.class_id, self.feedback_id, self.len, self.int_to_display = unpacker.unpack("BBHi")
+        self.class_id, self.feedback_id, self.len, self.int_to_display = unpacker.unpack(
+            "BBHi")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBHi", self.class_id, self.feedback_id, self.len, self.int_to_display))
+        buf.write(
+            struct.pack(
+                "=BBHi",
+                self.class_id,
+                self.feedback_id,
+                self.len,
+                self.int_to_display))
         return buf.getvalue()
     fixed_size = 8
+
+
 class StringFeedbackCtl(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.class_id, self.feedback_id, self.len, self.num_keysyms = unpacker.unpack("BBH2xH")
+        self.class_id, self.feedback_id, self.len, self.num_keysyms = unpacker.unpack(
+            "BBH2xH")
         self.keysyms = xcffib.List(unpacker, "I", self.num_keysyms)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBH2xH", self.class_id, self.feedback_id, self.len, self.num_keysyms))
+        buf.write(
+            struct.pack(
+                "=BBH2xH",
+                self.class_id,
+                self.feedback_id,
+                self.len,
+                self.num_keysyms))
         buf.write(xcffib.pack_list(self.keysyms, "I"))
         return buf.getvalue()
+
+
 class BellFeedbackCtl(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.class_id, self.feedback_id, self.len, self.percent, self.pitch, self.duration = unpacker.unpack("BBHb3xhh")
+        self.class_id, self.feedback_id, self.len, self.percent, self.pitch, self.duration = unpacker.unpack(
+            "BBHb3xhh")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBHb3xhh", self.class_id, self.feedback_id, self.len, self.percent, self.pitch, self.duration))
+        buf.write(
+            struct.pack(
+                "=BBHb3xhh",
+                self.class_id,
+                self.feedback_id,
+                self.len,
+                self.percent,
+                self.pitch,
+                self.duration))
         return buf.getvalue()
     fixed_size = 12
+
+
 class LedFeedbackCtl(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.class_id, self.feedback_id, self.len, self.led_mask, self.led_values = unpacker.unpack("BBHII")
+        self.class_id, self.feedback_id, self.len, self.led_mask, self.led_values = unpacker.unpack(
+            "BBHII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBHII", self.class_id, self.feedback_id, self.len, self.led_mask, self.led_values))
+        buf.write(
+            struct.pack(
+                "=BBHII",
+                self.class_id,
+                self.feedback_id,
+                self.len,
+                self.led_mask,
+                self.led_values))
         return buf.getvalue()
     fixed_size = 12
+
+
 class FeedbackCtl(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.class_id, self.feedback_id, self.len = unpacker.unpack("BBH")
         self.uninterpreted_data = xcffib.List(unpacker, "B", self.len - 4)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBH", self.class_id, self.feedback_id, self.len))
+        buf.write(
+            struct.pack(
+                "=BBH",
+                self.class_id,
+                self.feedback_id,
+                self.len))
         buf.write(xcffib.pack_list(self.uninterpreted_data, "B"))
         return buf.getvalue()
+
+
 class GetDeviceKeyMappingReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.keysyms_per_keycode, = unpacker.unpack("xx2x4xB23x")
         self.keysyms = xcffib.List(unpacker, "I", self.length)
         self.bufsize = unpacker.offset - base
+
+
 class GetDeviceKeyMappingCookie(xcffib.Cookie):
     reply_type = GetDeviceKeyMappingReply
+
+
 class GetDeviceModifierMappingReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.keycodes_per_modifier, = unpacker.unpack("xx2x4xB23x")
-        self.keymaps = xcffib.List(unpacker, "B", self.keycodes_per_modifier * 8)
+        self.keymaps = xcffib.List(
+            unpacker,
+            "B",
+            self.keycodes_per_modifier *
+            8)
         self.bufsize = unpacker.offset - base
+
+
 class GetDeviceModifierMappingCookie(xcffib.Cookie):
     reply_type = GetDeviceModifierMappingReply
+
+
 class SetDeviceModifierMappingReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, = unpacker.unpack("xx2x4xB23x")
         self.bufsize = unpacker.offset - base
+
+
 class SetDeviceModifierMappingCookie(xcffib.Cookie):
     reply_type = SetDeviceModifierMappingReply
+
+
 class GetDeviceButtonMappingReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.map_size, = unpacker.unpack("xx2x4xB23x")
         self.map = xcffib.List(unpacker, "B", self.map_size)
         self.bufsize = unpacker.offset - base
+
+
 class GetDeviceButtonMappingCookie(xcffib.Cookie):
     reply_type = GetDeviceButtonMappingReply
+
+
 class SetDeviceButtonMappingReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, = unpacker.unpack("xx2x4xB23x")
         self.bufsize = unpacker.offset - base
+
+
 class SetDeviceButtonMappingCookie(xcffib.Cookie):
     reply_type = SetDeviceButtonMappingReply
+
+
 class KeyState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.class_id, self.len, self.num_keys = unpacker.unpack("BBBx")
         self.keys = xcffib.List(unpacker, "B", 32)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=BBBx", self.class_id, self.len, self.num_keys))
         buf.write(xcffib.pack_list(self.keys, "B"))
         return buf.getvalue()
     fixed_size = 36
+
+
 class ButtonState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.class_id, self.len, self.num_buttons = unpacker.unpack("BBBx")
         self.buttons = xcffib.List(unpacker, "B", 32)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBBx", self.class_id, self.len, self.num_buttons))
+        buf.write(
+            struct.pack(
+                "=BBBx",
+                self.class_id,
+                self.len,
+                self.num_buttons))
         buf.write(xcffib.pack_list(self.buttons, "B"))
         return buf.getvalue()
     fixed_size = 36
+
+
 class ValuatorState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.class_id, self.len, self.num_valuators, self.mode = unpacker.unpack("BBBB")
+        self.class_id, self.len, self.num_valuators, self.mode = unpacker.unpack(
+            "BBBB")
         self.valuators = xcffib.List(unpacker, "I", self.num_valuators)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBBB", self.class_id, self.len, self.num_valuators, self.mode))
+        buf.write(
+            struct.pack(
+                "=BBBB",
+                self.class_id,
+                self.len,
+                self.num_valuators,
+                self.mode))
         buf.write(xcffib.pack_list(self.valuators, "I"))
         return buf.getvalue()
+
+
 class InputState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.class_id, self.len, self.num_items = unpacker.unpack("BBBx")
         self.uninterpreted_data = xcffib.List(unpacker, "B", self.len - 4)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBBx", self.class_id, self.len, self.num_items))
+        buf.write(
+            struct.pack(
+                "=BBBx",
+                self.class_id,
+                self.len,
+                self.num_items))
         buf.write(xcffib.pack_list(self.uninterpreted_data, "B"))
         return buf.getvalue()
+
+
 class QueryDeviceStateReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_classes, = unpacker.unpack("xx2x4xB23x")
         self.classes = xcffib.List(unpacker, InputState, self.num_classes)
         self.bufsize = unpacker.offset - base
+
+
 class QueryDeviceStateCookie(xcffib.Cookie):
     reply_type = QueryDeviceStateReply
+
+
 class SetDeviceValuatorsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, = unpacker.unpack("xx2x4xB23x")
         self.bufsize = unpacker.offset - base
+
+
 class SetDeviceValuatorsCookie(xcffib.Cookie):
     reply_type = SetDeviceValuatorsReply
+
+
 class DeviceControl:
     resolution = 1
     abs_calib = 2
     core = 3
     enable = 4
     abs_area = 5
+
+
 class DeviceResolutionState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.control_id, self.len, self.num_valuators = unpacker.unpack("HHI")
         self.resolution_values = xcffib.List(unpacker, "I", self.num_valuators)
         unpacker.pad("I")
         self.resolution_min = xcffib.List(unpacker, "I", self.num_valuators)
         unpacker.pad("I")
         self.resolution_max = xcffib.List(unpacker, "I", self.num_valuators)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHI", self.control_id, self.len, self.num_valuators))
+        buf.write(
+            struct.pack(
+                "=HHI",
+                self.control_id,
+                self.len,
+                self.num_valuators))
         buf.write(xcffib.pack_list(self.resolution_values, "I"))
         buf.write(xcffib.pack_list(self.resolution_min, "I"))
         buf.write(xcffib.pack_list(self.resolution_max, "I"))
         return buf.getvalue()
+
+
 class DeviceAbsCalibState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.control_id, self.len, self.min_x, self.max_x, self.min_y, self.max_y, self.flip_x, self.flip_y, self.rotation, self.button_threshold = unpacker.unpack("HHiiiiIIII")
+        self.control_id, self.len, self.min_x, self.max_x, self.min_y, self.max_y, self.flip_x, self.flip_y, self.rotation, self.button_threshold = unpacker.unpack(
+            "HHiiiiIIII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHiiiiIIII", self.control_id, self.len, self.min_x, self.max_x, self.min_y, self.max_y, self.flip_x, self.flip_y, self.rotation, self.button_threshold))
+        buf.write(
+            struct.pack(
+                "=HHiiiiIIII",
+                self.control_id,
+                self.len,
+                self.min_x,
+                self.max_x,
+                self.min_y,
+                self.max_y,
+                self.flip_x,
+                self.flip_y,
+                self.rotation,
+                self.button_threshold))
         return buf.getvalue()
     fixed_size = 36
+
+
 class DeviceAbsAreaState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.control_id, self.len, self.offset_x, self.offset_y, self.width, self.height, self.screen, self.following = unpacker.unpack("HHIIIIII")
+        self.control_id, self.len, self.offset_x, self.offset_y, self.width, self.height, self.screen, self.following = unpacker.unpack(
+            "HHIIIIII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHIIIIII", self.control_id, self.len, self.offset_x, self.offset_y, self.width, self.height, self.screen, self.following))
+        buf.write(
+            struct.pack(
+                "=HHIIIIII",
+                self.control_id,
+                self.len,
+                self.offset_x,
+                self.offset_y,
+                self.width,
+                self.height,
+                self.screen,
+                self.following))
         return buf.getvalue()
     fixed_size = 28
+
+
 class DeviceCoreState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.control_id, self.len, self.status, self.iscore = unpacker.unpack("HHBB2x")
+        self.control_id, self.len, self.status, self.iscore = unpacker.unpack(
+            "HHBB2x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHBB2x", self.control_id, self.len, self.status, self.iscore))
+        buf.write(
+            struct.pack(
+                "=HHBB2x",
+                self.control_id,
+                self.len,
+                self.status,
+                self.iscore))
         return buf.getvalue()
     fixed_size = 8
+
+
 class DeviceEnableState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.control_id, self.len, self.enable = unpacker.unpack("HHB3x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHB3x", self.control_id, self.len, self.enable))
+        buf.write(
+            struct.pack(
+                "=HHB3x",
+                self.control_id,
+                self.len,
+                self.enable))
         return buf.getvalue()
     fixed_size = 8
+
+
 class DeviceState(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.control_id, self.len = unpacker.unpack("HH")
         self.uninterpreted_data = xcffib.List(unpacker, "B", self.len - 4)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=HH", self.control_id, self.len))
         buf.write(xcffib.pack_list(self.uninterpreted_data, "B"))
         return buf.getvalue()
+
+
 class GetDeviceControlReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, = unpacker.unpack("xx2x4xB23x")
         self.control = DeviceState(unpacker)
         self.bufsize = unpacker.offset - base
+
+
 class GetDeviceControlCookie(xcffib.Cookie):
     reply_type = GetDeviceControlReply
+
+
 class DeviceResolutionCtl(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.control_id, self.len, self.first_valuator, self.num_valuators = unpacker.unpack("HHBB")
+        self.control_id, self.len, self.first_valuator, self.num_valuators = unpacker.unpack(
+            "HHBB")
         self.resolution_values = xcffib.List(unpacker, "I", self.num_valuators)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHBB", self.control_id, self.len, self.first_valuator, self.num_valuators))
+        buf.write(
+            struct.pack(
+                "=HHBB",
+                self.control_id,
+                self.len,
+                self.first_valuator,
+                self.num_valuators))
         buf.write(xcffib.pack_list(self.resolution_values, "I"))
         return buf.getvalue()
+
+
 class DeviceAbsCalibCtl(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.control_id, self.len, self.min_x, self.max_x, self.min_y, self.max_y, self.flip_x, self.flip_y, self.rotation, self.button_threshold = unpacker.unpack("HHiiiiIIII")
+        self.control_id, self.len, self.min_x, self.max_x, self.min_y, self.max_y, self.flip_x, self.flip_y, self.rotation, self.button_threshold = unpacker.unpack(
+            "HHiiiiIIII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHiiiiIIII", self.control_id, self.len, self.min_x, self.max_x, self.min_y, self.max_y, self.flip_x, self.flip_y, self.rotation, self.button_threshold))
+        buf.write(
+            struct.pack(
+                "=HHiiiiIIII",
+                self.control_id,
+                self.len,
+                self.min_x,
+                self.max_x,
+                self.min_y,
+                self.max_y,
+                self.flip_x,
+                self.flip_y,
+                self.rotation,
+                self.button_threshold))
         return buf.getvalue()
     fixed_size = 36
+
+
 class DeviceAbsAreaCtrl(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.control_id, self.len, self.offset_x, self.offset_y, self.width, self.height, self.screen, self.following = unpacker.unpack("HHIIiiiI")
+        self.control_id, self.len, self.offset_x, self.offset_y, self.width, self.height, self.screen, self.following = unpacker.unpack(
+            "HHIIiiiI")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHIIiiiI", self.control_id, self.len, self.offset_x, self.offset_y, self.width, self.height, self.screen, self.following))
+        buf.write(
+            struct.pack(
+                "=HHIIiiiI",
+                self.control_id,
+                self.len,
+                self.offset_x,
+                self.offset_y,
+                self.width,
+                self.height,
+                self.screen,
+                self.following))
         return buf.getvalue()
     fixed_size = 28
+
+
 class DeviceCoreCtrl(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.control_id, self.len, self.status = unpacker.unpack("HHB3x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHB3x", self.control_id, self.len, self.status))
+        buf.write(
+            struct.pack(
+                "=HHB3x",
+                self.control_id,
+                self.len,
+                self.status))
         return buf.getvalue()
     fixed_size = 8
+
+
 class DeviceEnableCtrl(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.control_id, self.len, self.enable = unpacker.unpack("HHB3x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHB3x", self.control_id, self.len, self.enable))
+        buf.write(
+            struct.pack(
+                "=HHB3x",
+                self.control_id,
+                self.len,
+                self.enable))
         return buf.getvalue()
     fixed_size = 8
+
+
 class DeviceCtl(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.control_id, self.len = unpacker.unpack("HH")
         self.uninterpreted_data = xcffib.List(unpacker, "B", self.len - 4)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=HH", self.control_id, self.len))
         buf.write(xcffib.pack_list(self.uninterpreted_data, "B"))
         return buf.getvalue()
+
+
 class ChangeDeviceControlReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, = unpacker.unpack("xx2x4xB23x")
         self.bufsize = unpacker.offset - base
+
+
 class ChangeDeviceControlCookie(xcffib.Cookie):
     reply_type = ChangeDeviceControlReply
+
+
 class ListDevicePropertiesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_atoms, = unpacker.unpack("xx2x4xH22x")
         self.atoms = xcffib.List(unpacker, "I", self.num_atoms)
         self.bufsize = unpacker.offset - base
+
+
 class ListDevicePropertiesCookie(xcffib.Cookie):
     reply_type = ListDevicePropertiesReply
+
+
 class PropertyFormat:
     _8Bits = 8
     _16Bits = 16
     _32Bits = 32
+
+
 class GetDevicePropertyReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.type, self.bytes_after, self.num_items, self.format, self.device_id = unpacker.unpack("xx2x4xIIIBB10x")
+        self.type, self.bytes_after, self.num_items, self.format, self.device_id = unpacker.unpack(
+            "xx2x4xIIIBB10x")
         self.bufsize = unpacker.offset - base
+
+
 class GetDevicePropertyCookie(xcffib.Cookie):
     reply_type = GetDevicePropertyReply
+
+
 class Device:
     All = 0
     AllMaster = 1
+
+
 class GroupInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.base, self.latched, self.locked, self.effective = unpacker.unpack("BBBB")
+        self.base, self.latched, self.locked, self.effective = unpacker.unpack(
+            "BBBB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBBB", self.base, self.latched, self.locked, self.effective))
+        buf.write(
+            struct.pack(
+                "=BBBB",
+                self.base,
+                self.latched,
+                self.locked,
+                self.effective))
         return buf.getvalue()
     fixed_size = 4
+
+
 class ModifierInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.base, self.latched, self.locked, self.effective = unpacker.unpack("IIII")
+        self.base, self.latched, self.locked, self.effective = unpacker.unpack(
+            "IIII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IIII", self.base, self.latched, self.locked, self.effective))
+        buf.write(
+            struct.pack(
+                "=IIII",
+                self.base,
+                self.latched,
+                self.locked,
+                self.effective))
         return buf.getvalue()
     fixed_size = 16
+
+
 class XIQueryPointerReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.root, self.child, self.root_x, self.root_y, self.win_x, self.win_y, self.same_screen, self.buttons_len = unpacker.unpack("xx2x4xIIiiiiBxH")
+        self.root, self.child, self.root_x, self.root_y, self.win_x, self.win_y, self.same_screen, self.buttons_len = unpacker.unpack(
+            "xx2x4xIIiiiiBxH")
         self.mods = ModifierInfo(unpacker)
         unpacker.pad(GroupInfo)
         self.group = GroupInfo(unpacker)
         unpacker.pad("I")
         self.buttons = xcffib.List(unpacker, "I", self.buttons_len)
         self.bufsize = unpacker.offset - base
+
+
 class XIQueryPointerCookie(xcffib.Cookie):
     reply_type = XIQueryPointerReply
+
+
 class HierarchyChangeType:
     AddMaster = 1
     RemoveMaster = 2
     AttachSlave = 3
     DetachSlave = 4
+
+
 class ChangeMode:
     Attach = 1
     Float = 2
+
+
 class AddMaster(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.type, self.len, self.name_len, self.send_core, self.enable = unpacker.unpack("HHHBB")
+        self.type, self.len, self.name_len, self.send_core, self.enable = unpacker.unpack(
+            "HHHBB")
         self.name = xcffib.List(unpacker, "c", self.name_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHHBB", self.type, self.len, self.name_len, self.send_core, self.enable))
+        buf.write(
+            struct.pack(
+                "=HHHBB",
+                self.type,
+                self.len,
+                self.name_len,
+                self.send_core,
+                self.enable))
         buf.write(xcffib.pack_list(self.name, "c"))
         return buf.getvalue()
+
+
 class RemoveMaster(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.type, self.len, self.deviceid, self.return_mode, self.return_pointer, self.return_keyboard = unpacker.unpack("HHHBxHH")
+        self.type, self.len, self.deviceid, self.return_mode, self.return_pointer, self.return_keyboard = unpacker.unpack(
+            "HHHBxHH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHHBxHH", self.type, self.len, self.deviceid, self.return_mode, self.return_pointer, self.return_keyboard))
+        buf.write(
+            struct.pack(
+                "=HHHBxHH",
+                self.type,
+                self.len,
+                self.deviceid,
+                self.return_mode,
+                self.return_pointer,
+                self.return_keyboard))
         return buf.getvalue()
     fixed_size = 12
+
+
 class AttachSlave(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.type, self.len, self.deviceid, self.master = unpacker.unpack("HHHH")
+        self.type, self.len, self.deviceid, self.master = unpacker.unpack(
+            "HHHH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHHH", self.type, self.len, self.deviceid, self.master))
+        buf.write(
+            struct.pack(
+                "=HHHH",
+                self.type,
+                self.len,
+                self.deviceid,
+                self.master))
         return buf.getvalue()
     fixed_size = 8
+
+
 class DetachSlave(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.type, self.len, self.deviceid = unpacker.unpack("HHH2x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=HHH2x", self.type, self.len, self.deviceid))
         return buf.getvalue()
     fixed_size = 8
+
+
 class HierarchyChange(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.type, self.len = unpacker.unpack("HH")
-        self.uninterpreted_data = xcffib.List(unpacker, "B", (self.len * 4) - 4)
+        self.uninterpreted_data = xcffib.List(
+            unpacker,
+            "B",
+            (self.len * 4) - 4)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=HH", self.type, self.len))
         buf.write(xcffib.pack_list(self.uninterpreted_data, "B"))
         return buf.getvalue()
+
+
 class XIGetClientPointerReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.set, self.deviceid = unpacker.unpack("xx2x4xBxH20x")
         self.bufsize = unpacker.offset - base
+
+
 class XIGetClientPointerCookie(xcffib.Cookie):
     reply_type = XIGetClientPointerReply
+
+
 class XIEventMask:
     DeviceChanged = 1 << 1
     KeyPress = 1 << 2
     KeyRelease = 1 << 3
     ButtonPress = 1 << 4
     ButtonRelease = 1 << 5
     Motion = 1 << 6
@@ -847,1213 +1492,2635 @@
     TouchEnd = 1 << 20
     TouchOwnership = 1 << 21
     RawTouchBegin = 1 << 22
     RawTouchUpdate = 1 << 23
     RawTouchEnd = 1 << 24
     BarrierHit = 1 << 25
     BarrierLeave = 1 << 26
+
+
 class EventMask(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.deviceid, self.mask_len = unpacker.unpack("HH")
         self.mask = xcffib.List(unpacker, "I", self.mask_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=HH", self.deviceid, self.mask_len))
         buf.write(xcffib.pack_list(self.mask, "I"))
         return buf.getvalue()
+
+
 class XIQueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.major_version, self.minor_version = unpacker.unpack("xx2x4xHH20x")
         self.bufsize = unpacker.offset - base
+
+
 class XIQueryVersionCookie(xcffib.Cookie):
     reply_type = XIQueryVersionReply
+
+
 class DeviceClassType:
     Key = 0
     Button = 1
     Valuator = 2
     Scroll = 3
     Touch = 8
+
+
 class DeviceType:
     MasterPointer = 1
     MasterKeyboard = 2
     SlavePointer = 3
     SlaveKeyboard = 4
     FloatingSlave = 5
+
+
 class ScrollFlags:
     NoEmulation = 1 << 0
     Preferred = 1 << 1
+
+
 class ScrollType:
     Vertical = 1
     Horizontal = 2
+
+
 class TouchMode:
     Direct = 1
     Dependent = 2
+
+
 class ButtonClass(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.type, self.len, self.sourceid, self.num_buttons = unpacker.unpack("HHHH")
+        self.type, self.len, self.sourceid, self.num_buttons = unpacker.unpack(
+            "HHHH")
         self.state = xcffib.List(unpacker, "I", (self.num_buttons + 31) // 32)
         unpacker.pad("I")
         self.labels = xcffib.List(unpacker, "I", self.num_buttons)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHHH", self.type, self.len, self.sourceid, self.num_buttons))
+        buf.write(
+            struct.pack(
+                "=HHHH",
+                self.type,
+                self.len,
+                self.sourceid,
+                self.num_buttons))
         buf.write(xcffib.pack_list(self.state, "I"))
         buf.write(xcffib.pack_list(self.labels, "I"))
         return buf.getvalue()
+
+
 class KeyClass(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.type, self.len, self.sourceid, self.num_keys = unpacker.unpack("HHHH")
+        self.type, self.len, self.sourceid, self.num_keys = unpacker.unpack(
+            "HHHH")
         self.keys = xcffib.List(unpacker, "I", self.num_keys)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHHH", self.type, self.len, self.sourceid, self.num_keys))
+        buf.write(
+            struct.pack(
+                "=HHHH",
+                self.type,
+                self.len,
+                self.sourceid,
+                self.num_keys))
         buf.write(xcffib.pack_list(self.keys, "I"))
         return buf.getvalue()
+
+
 class ScrollClass(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.type, self.len, self.sourceid, self.number, self.scroll_type, self.flags = unpacker.unpack("HHHHH2xI")
+        self.type, self.len, self.sourceid, self.number, self.scroll_type, self.flags = unpacker.unpack(
+            "HHHHH2xI")
         self.increment = FP3232(unpacker)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHHHH2xI", self.type, self.len, self.sourceid, self.number, self.scroll_type, self.flags))
+        buf.write(
+            struct.pack(
+                "=HHHHH2xI",
+                self.type,
+                self.len,
+                self.sourceid,
+                self.number,
+                self.scroll_type,
+                self.flags))
         buf.write(self.increment.pack())
         return buf.getvalue()
+
+
 class TouchClass(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.type, self.len, self.sourceid, self.mode, self.num_touches = unpacker.unpack("HHHBB")
+        self.type, self.len, self.sourceid, self.mode, self.num_touches = unpacker.unpack(
+            "HHHBB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHHBB", self.type, self.len, self.sourceid, self.mode, self.num_touches))
+        buf.write(
+            struct.pack(
+                "=HHHBB",
+                self.type,
+                self.len,
+                self.sourceid,
+                self.mode,
+                self.num_touches))
         return buf.getvalue()
     fixed_size = 8
+
+
 class ValuatorClass(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.type, self.len, self.sourceid, self.number, self.label = unpacker.unpack("HHHHI")
+        self.type, self.len, self.sourceid, self.number, self.label = unpacker.unpack(
+            "HHHHI")
         self.min = FP3232(unpacker)
         unpacker.pad(FP3232)
         self.max = FP3232(unpacker)
         unpacker.pad(FP3232)
         self.value = FP3232(unpacker)
         self.resolution, self.mode = unpacker.unpack("IB3x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHHHIIB3x", self.type, self.len, self.sourceid, self.number, self.label, self.resolution, self.mode))
+        buf.write(
+            struct.pack(
+                "=HHHHIIB3x",
+                self.type,
+                self.len,
+                self.sourceid,
+                self.number,
+                self.label,
+                self.resolution,
+                self.mode))
         buf.write(self.min.pack())
         buf.write(self.max.pack())
         buf.write(self.value.pack())
         return buf.getvalue()
+
+
 class DeviceClass(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.type, self.len, self.sourceid = unpacker.unpack("HHH2x")
-        self.uninterpreted_data = xcffib.List(unpacker, "B", (self.len * 4) - 8)
+        self.uninterpreted_data = xcffib.List(
+            unpacker,
+            "B",
+            (self.len * 4) - 8)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=HHH2x", self.type, self.len, self.sourceid))
         buf.write(xcffib.pack_list(self.uninterpreted_data, "B"))
         return buf.getvalue()
+
+
 class XIDeviceInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.type, self.attachment, self.num_classes, self.name_len, self.enabled = unpacker.unpack("HHHHHBx")
+        self.deviceid, self.type, self.attachment, self.num_classes, self.name_len, self.enabled = unpacker.unpack(
+            "HHHHHBx")
         self.name = xcffib.List(unpacker, "c", ((self.name_len + 3) // 4) * 4)
         unpacker.pad(DeviceClass)
         self.classes = xcffib.List(unpacker, DeviceClass, self.num_classes)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHHHHBx", self.deviceid, self.type, self.attachment, self.num_classes, self.name_len, self.enabled))
+        buf.write(
+            struct.pack(
+                "=HHHHHBx",
+                self.deviceid,
+                self.type,
+                self.attachment,
+                self.num_classes,
+                self.name_len,
+                self.enabled))
         buf.write(xcffib.pack_list(self.name, "c"))
         buf.write(xcffib.pack_list(self.classes, DeviceClass))
         return buf.getvalue()
+
+
 class XIQueryDeviceReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_infos, = unpacker.unpack("xx2x4xH22x")
         self.infos = xcffib.List(unpacker, XIDeviceInfo, self.num_infos)
         self.bufsize = unpacker.offset - base
+
+
 class XIQueryDeviceCookie(xcffib.Cookie):
     reply_type = XIQueryDeviceReply
+
+
 class XIGetFocusReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.focus, = unpacker.unpack("xx2x4xI20x")
         self.bufsize = unpacker.offset - base
+
+
 class XIGetFocusCookie(xcffib.Cookie):
     reply_type = XIGetFocusReply
+
+
 class GrabOwner:
     NoOwner = 0
     Owner = 1
+
+
 class XIGrabDeviceReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, = unpacker.unpack("xx2x4xB23x")
         self.bufsize = unpacker.offset - base
+
+
 class XIGrabDeviceCookie(xcffib.Cookie):
     reply_type = XIGrabDeviceReply
+
+
 class EventMode:
     AsyncDevice = 0
     SyncDevice = 1
     ReplayDevice = 2
     AsyncPairedDevice = 3
     AsyncPair = 4
     SyncPair = 5
     AcceptTouch = 6
     RejectTouch = 7
+
+
 class GrabMode22:
     Sync = 0
     Async = 1
     Touch = 2
+
+
 class GrabType:
     Button = 0
     Keycode = 1
     Enter = 2
     FocusIn = 3
     TouchBegin = 4
+
+
 class ModifierMask:
     Any = 1 << 31
+
+
 class GrabModifierInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.modifiers, self.status = unpacker.unpack("IB3x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=IB3x", self.modifiers, self.status))
         return buf.getvalue()
     fixed_size = 8
+
+
 class XIPassiveGrabDeviceReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_modifiers, = unpacker.unpack("xx2x4xH22x")
-        self.modifiers = xcffib.List(unpacker, GrabModifierInfo, self.num_modifiers)
+        self.modifiers = xcffib.List(
+            unpacker,
+            GrabModifierInfo,
+            self.num_modifiers)
         self.bufsize = unpacker.offset - base
+
+
 class XIPassiveGrabDeviceCookie(xcffib.Cookie):
     reply_type = XIPassiveGrabDeviceReply
+
+
 class XIListPropertiesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_properties, = unpacker.unpack("xx2x4xH22x")
         self.properties = xcffib.List(unpacker, "I", self.num_properties)
         self.bufsize = unpacker.offset - base
+
+
 class XIListPropertiesCookie(xcffib.Cookie):
     reply_type = XIListPropertiesReply
+
+
 class XIGetPropertyReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.type, self.bytes_after, self.num_items, self.format = unpacker.unpack("xx2x4xIIIB11x")
+        self.type, self.bytes_after, self.num_items, self.format = unpacker.unpack(
+            "xx2x4xIIIB11x")
         self.bufsize = unpacker.offset - base
+
+
 class XIGetPropertyCookie(xcffib.Cookie):
     reply_type = XIGetPropertyReply
+
+
 class XIGetSelectedEventsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_masks, = unpacker.unpack("xx2x4xH22x")
         self.masks = xcffib.List(unpacker, EventMask, self.num_masks)
         self.bufsize = unpacker.offset - base
+
+
 class XIGetSelectedEventsCookie(xcffib.Cookie):
     reply_type = XIGetSelectedEventsReply
+
+
 class BarrierReleasePointerInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
         self.deviceid, self.barrier, self.eventid = unpacker.unpack("H2xII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=H2xII", self.deviceid, self.barrier, self.eventid))
+        buf.write(
+            struct.pack(
+                "=H2xII",
+                self.deviceid,
+                self.barrier,
+                self.eventid))
         return buf.getvalue()
     fixed_size = 12
+
+
 class DeviceValuatorEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.device_id, self.device_state, self.num_valuators, self.first_valuator = unpacker.unpack("xB2xHBB")
+        self.device_id, self.device_state, self.num_valuators, self.first_valuator = unpacker.unpack(
+            "xB2xHBB")
         self.valuators = xcffib.List(unpacker, "i", 6)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BHBB", self.device_id, self.device_state, self.num_valuators, self.first_valuator))
+        buf.write(
+            struct.pack(
+                "=BHBB",
+                self.device_id,
+                self.device_state,
+                self.num_valuators,
+                self.first_valuator))
         buf.write(xcffib.pack_list(self.valuators, "i"))
         return buf.getvalue()
 _events[0] = DeviceValuatorEvent
+
+
 class DeviceKeyPressEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id = unpacker.unpack("xB2xIIIIhhhhHBB")
+        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id = unpacker.unpack(
+            "xB2xIIIIhhhhHBB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIIhhhhHBB", self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id))
+        buf.write(
+            struct.pack(
+                "=BIIIIhhhhHBB",
+                self.detail,
+                self.time,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.state,
+                self.same_screen,
+                self.device_id))
         return buf.getvalue()
 _events[1] = DeviceKeyPressEvent
+
+
 class DeviceKeyReleaseEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id = unpacker.unpack("xB2xIIIIhhhhHBB")
+        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id = unpacker.unpack(
+            "xB2xIIIIhhhhHBB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIIhhhhHBB", self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id))
+        buf.write(
+            struct.pack(
+                "=BIIIIhhhhHBB",
+                self.detail,
+                self.time,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.state,
+                self.same_screen,
+                self.device_id))
         return buf.getvalue()
 _events[2] = DeviceKeyReleaseEvent
+
+
 class DeviceButtonPressEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id = unpacker.unpack("xB2xIIIIhhhhHBB")
+        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id = unpacker.unpack(
+            "xB2xIIIIhhhhHBB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIIhhhhHBB", self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id))
+        buf.write(
+            struct.pack(
+                "=BIIIIhhhhHBB",
+                self.detail,
+                self.time,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.state,
+                self.same_screen,
+                self.device_id))
         return buf.getvalue()
 _events[3] = DeviceButtonPressEvent
+
+
 class DeviceButtonReleaseEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id = unpacker.unpack("xB2xIIIIhhhhHBB")
+        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id = unpacker.unpack(
+            "xB2xIIIIhhhhHBB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIIhhhhHBB", self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id))
+        buf.write(
+            struct.pack(
+                "=BIIIIhhhhHBB",
+                self.detail,
+                self.time,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.state,
+                self.same_screen,
+                self.device_id))
         return buf.getvalue()
 _events[4] = DeviceButtonReleaseEvent
+
+
 class DeviceMotionNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id = unpacker.unpack("xB2xIIIIhhhhHBB")
+        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id = unpacker.unpack(
+            "xB2xIIIIhhhhHBB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIIhhhhHBB", self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id))
+        buf.write(
+            struct.pack(
+                "=BIIIIhhhhHBB",
+                self.detail,
+                self.time,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.state,
+                self.same_screen,
+                self.device_id))
         return buf.getvalue()
 _events[5] = DeviceMotionNotifyEvent
+
+
 class DeviceFocusInEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.window, self.mode, self.device_id = unpacker.unpack("xB2xIIBB18x")
+        self.detail, self.time, self.window, self.mode, self.device_id = unpacker.unpack(
+            "xB2xIIBB18x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIBB18x", self.detail, self.time, self.window, self.mode, self.device_id))
+        buf.write(
+            struct.pack(
+                "=BIIBB18x",
+                self.detail,
+                self.time,
+                self.window,
+                self.mode,
+                self.device_id))
         return buf.getvalue()
 _events[6] = DeviceFocusInEvent
+
+
 class DeviceFocusOutEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.window, self.mode, self.device_id = unpacker.unpack("xB2xIIBB18x")
+        self.detail, self.time, self.window, self.mode, self.device_id = unpacker.unpack(
+            "xB2xIIBB18x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIBB18x", self.detail, self.time, self.window, self.mode, self.device_id))
+        buf.write(
+            struct.pack(
+                "=BIIBB18x",
+                self.detail,
+                self.time,
+                self.window,
+                self.mode,
+                self.device_id))
         return buf.getvalue()
 _events[7] = DeviceFocusOutEvent
+
+
 class ProximityInEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id = unpacker.unpack("xB2xIIIIhhhhHBB")
+        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id = unpacker.unpack(
+            "xB2xIIIIhhhhHBB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIIhhhhHBB", self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id))
+        buf.write(
+            struct.pack(
+                "=BIIIIhhhhHBB",
+                self.detail,
+                self.time,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.state,
+                self.same_screen,
+                self.device_id))
         return buf.getvalue()
 _events[8] = ProximityInEvent
+
+
 class ProximityOutEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id = unpacker.unpack("xB2xIIIIhhhhHBB")
+        self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id = unpacker.unpack(
+            "xB2xIIIIhhhhHBB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIIIhhhhHBB", self.detail, self.time, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.state, self.same_screen, self.device_id))
+        buf.write(
+            struct.pack(
+                "=BIIIIhhhhHBB",
+                self.detail,
+                self.time,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.state,
+                self.same_screen,
+                self.device_id))
         return buf.getvalue()
 _events[9] = ProximityOutEvent
+
+
 class DeviceStateNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.device_id, self.time, self.num_keys, self.num_buttons, self.num_valuators, self.classes_reported = unpacker.unpack("xB2xIBBBB")
+        self.device_id, self.time, self.num_keys, self.num_buttons, self.num_valuators, self.classes_reported = unpacker.unpack(
+            "xB2xIBBBB")
         self.buttons = xcffib.List(unpacker, "B", 4)
         unpacker.pad("B")
         self.keys = xcffib.List(unpacker, "B", 4)
         unpacker.pad("I")
         self.valuators = xcffib.List(unpacker, "I", 3)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIBBBB", self.device_id, self.time, self.num_keys, self.num_buttons, self.num_valuators, self.classes_reported))
+        buf.write(
+            struct.pack(
+                "=BIBBBB",
+                self.device_id,
+                self.time,
+                self.num_keys,
+                self.num_buttons,
+                self.num_valuators,
+                self.classes_reported))
         buf.write(xcffib.pack_list(self.buttons, "B"))
         buf.write(xcffib.pack_list(self.keys, "B"))
         buf.write(xcffib.pack_list(self.valuators, "I"))
         return buf.getvalue()
 _events[10] = DeviceStateNotifyEvent
+
+
 class DeviceMappingNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.device_id, self.request, self.first_keycode, self.count, self.time = unpacker.unpack("xB2xBBBxI20x")
+        self.device_id, self.request, self.first_keycode, self.count, self.time = unpacker.unpack(
+            "xB2xBBBxI20x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BBBBxI20x", self.device_id, self.request, self.first_keycode, self.count, self.time))
+        buf.write(
+            struct.pack(
+                "=BBBBxI20x",
+                self.device_id,
+                self.request,
+                self.first_keycode,
+                self.count,
+                self.time))
         return buf.getvalue()
 _events[11] = DeviceMappingNotifyEvent
+
+
 class ChangeDeviceNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         self.device_id, self.time, self.request = unpacker.unpack("xB2xIB23x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIB23x", self.device_id, self.time, self.request))
+        buf.write(
+            struct.pack(
+                "=BIB23x",
+                self.device_id,
+                self.time,
+                self.request))
         return buf.getvalue()
 _events[12] = ChangeDeviceNotifyEvent
+
+
 class DeviceKeyStateNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         self.device_id, = unpacker.unpack("xB2x")
         self.keys = xcffib.List(unpacker, "B", 28)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=B", self.device_id))
         buf.write(xcffib.pack_list(self.keys, "B"))
         return buf.getvalue()
 _events[13] = DeviceKeyStateNotifyEvent
+
+
 class DeviceButtonStateNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
         self.device_id, = unpacker.unpack("xB2x")
         self.buttons = xcffib.List(unpacker, "B", 28)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
         buf.write(struct.pack("=B", self.device_id))
         buf.write(xcffib.pack_list(self.buttons, "B"))
         return buf.getvalue()
 _events[14] = DeviceButtonStateNotifyEvent
+
+
 class DeviceChange:
     Added = 0
     Removed = 1
     Enabled = 2
     Disabled = 3
     Unrecoverable = 4
     ControlChanged = 5
+
+
 class DevicePresenceNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.time, self.devchange, self.device_id, self.control = unpacker.unpack("xx2xIBBH20x")
+        self.time, self.devchange, self.device_id, self.control = unpacker.unpack(
+            "xx2xIBBH20x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xIBBH20x", self.time, self.devchange, self.device_id, self.control))
+        buf.write(
+            struct.pack(
+                "=xIBBH20x",
+                self.time,
+                self.devchange,
+                self.device_id,
+                self.control))
         return buf.getvalue()
 _events[15] = DevicePresenceNotifyEvent
+
+
 class DevicePropertyNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.state, self.time, self.property, self.device_id = unpacker.unpack("xB2xII19xB")
+        self.state, self.time, self.property, self.device_id = unpacker.unpack(
+            "xB2xII19xB")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BII19xB", self.state, self.time, self.property, self.device_id))
+        buf.write(
+            struct.pack(
+                "=BII19xB",
+                self.state,
+                self.time,
+                self.property,
+                self.device_id))
         return buf.getvalue()
 _events[16] = DevicePropertyNotifyEvent
+
+
 class ChangeReason:
     SlaveSwitch = 1
     DeviceChange = 2
+
+
 class DeviceChangedEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.num_classes, self.sourceid, self.reason = unpacker.unpack("xx2xHIHHB11x")
+        self.deviceid, self.time, self.num_classes, self.sourceid, self.reason = unpacker.unpack(
+            "xx2xHIHHB11x")
         self.classes = xcffib.List(unpacker, DeviceClass, self.num_classes)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIHHB11x", self.deviceid, self.time, self.num_classes, self.sourceid, self.reason))
+        buf.write(
+            struct.pack(
+                "=HIHHB11x",
+                self.deviceid,
+                self.time,
+                self.num_classes,
+                self.sourceid,
+                self.reason))
         buf.write(xcffib.pack_list(self.classes, DeviceClass))
         return buf.getvalue()
 _events[1] = DeviceChangedEvent
+
+
 class KeyEventFlags:
     KeyRepeat = 1 << 16
+
+
 class KeyPressEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack("xx2xHIIIIIiiiiHHH2xI")
+        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack(
+            "xx2xHIIIIIiiiiHHH2xI")
         self.mods = ModifierInfo(unpacker)
         unpacker.pad(GroupInfo)
         self.group = GroupInfo(unpacker)
         unpacker.pad("I")
         self.button_mask = xcffib.List(unpacker, "I", self.buttons_len)
         unpacker.pad("I")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIIIIiiiiHHH2xI", self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIIIIiiiiHHH2xI",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.buttons_len,
+                self.valuators_len,
+                self.sourceid,
+                self.flags))
         buf.write(self.mods.pack())
         buf.write(self.group.pack())
         buf.write(xcffib.pack_list(self.button_mask, "I"))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[2] = KeyPressEvent
+
+
 class KeyReleaseEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack("xx2xHIIIIIiiiiHHH2xI")
+        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack(
+            "xx2xHIIIIIiiiiHHH2xI")
         self.mods = ModifierInfo(unpacker)
         unpacker.pad(GroupInfo)
         self.group = GroupInfo(unpacker)
         unpacker.pad("I")
         self.button_mask = xcffib.List(unpacker, "I", self.buttons_len)
         unpacker.pad("I")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIIIIiiiiHHH2xI", self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIIIIiiiiHHH2xI",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.buttons_len,
+                self.valuators_len,
+                self.sourceid,
+                self.flags))
         buf.write(self.mods.pack())
         buf.write(self.group.pack())
         buf.write(xcffib.pack_list(self.button_mask, "I"))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[3] = KeyReleaseEvent
+
+
 class PointerEventFlags:
     PointerEmulated = 1 << 16
+
+
 class ButtonPressEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack("xx2xHIIIIIiiiiHHH2xI")
+        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack(
+            "xx2xHIIIIIiiiiHHH2xI")
         self.mods = ModifierInfo(unpacker)
         unpacker.pad(GroupInfo)
         self.group = GroupInfo(unpacker)
         unpacker.pad("I")
         self.button_mask = xcffib.List(unpacker, "I", self.buttons_len)
         unpacker.pad("I")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIIIIiiiiHHH2xI", self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIIIIiiiiHHH2xI",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.buttons_len,
+                self.valuators_len,
+                self.sourceid,
+                self.flags))
         buf.write(self.mods.pack())
         buf.write(self.group.pack())
         buf.write(xcffib.pack_list(self.button_mask, "I"))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[4] = ButtonPressEvent
+
+
 class ButtonReleaseEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack("xx2xHIIIIIiiiiHHH2xI")
+        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack(
+            "xx2xHIIIIIiiiiHHH2xI")
         self.mods = ModifierInfo(unpacker)
         unpacker.pad(GroupInfo)
         self.group = GroupInfo(unpacker)
         unpacker.pad("I")
         self.button_mask = xcffib.List(unpacker, "I", self.buttons_len)
         unpacker.pad("I")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIIIIiiiiHHH2xI", self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIIIIiiiiHHH2xI",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.buttons_len,
+                self.valuators_len,
+                self.sourceid,
+                self.flags))
         buf.write(self.mods.pack())
         buf.write(self.group.pack())
         buf.write(xcffib.pack_list(self.button_mask, "I"))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[5] = ButtonReleaseEvent
+
+
 class MotionEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack("xx2xHIIIIIiiiiHHH2xI")
+        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack(
+            "xx2xHIIIIIiiiiHHH2xI")
         self.mods = ModifierInfo(unpacker)
         unpacker.pad(GroupInfo)
         self.group = GroupInfo(unpacker)
         unpacker.pad("I")
         self.button_mask = xcffib.List(unpacker, "I", self.buttons_len)
         unpacker.pad("I")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIIIIiiiiHHH2xI", self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIIIIiiiiHHH2xI",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.buttons_len,
+                self.valuators_len,
+                self.sourceid,
+                self.flags))
         buf.write(self.mods.pack())
         buf.write(self.group.pack())
         buf.write(xcffib.pack_list(self.button_mask, "I"))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[6] = MotionEvent
+
+
 class NotifyMode:
     Normal = 0
     Grab = 1
     Ungrab = 2
     WhileGrabbed = 3
     PassiveGrab = 4
     PassiveUngrab = 5
+
+
 class NotifyDetail:
     Ancestor = 0
     Virtual = 1
     Inferior = 2
     Nonlinear = 3
     NonlinearVirtual = 4
     Pointer = 5
     PointerRoot = 6
     _None = 7
+
+
 class EnterEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.sourceid, self.mode, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.same_screen, self.focus, self.buttons_len = unpacker.unpack("xx2xHIHBBIIIiiiiBBH")
+        self.deviceid, self.time, self.sourceid, self.mode, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.same_screen, self.focus, self.buttons_len = unpacker.unpack(
+            "xx2xHIHBBIIIiiiiBBH")
         self.mods = ModifierInfo(unpacker)
         unpacker.pad(GroupInfo)
         self.group = GroupInfo(unpacker)
         unpacker.pad("I")
         self.buttons = xcffib.List(unpacker, "I", self.buttons_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIHBBIIIiiiiBBH", self.deviceid, self.time, self.sourceid, self.mode, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.same_screen, self.focus, self.buttons_len))
+        buf.write(
+            struct.pack(
+                "=HIHBBIIIiiiiBBH",
+                self.deviceid,
+                self.time,
+                self.sourceid,
+                self.mode,
+                self.detail,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.same_screen,
+                self.focus,
+                self.buttons_len))
         buf.write(self.mods.pack())
         buf.write(self.group.pack())
         buf.write(xcffib.pack_list(self.buttons, "I"))
         return buf.getvalue()
 _events[7] = EnterEvent
+
+
 class LeaveEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.sourceid, self.mode, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.same_screen, self.focus, self.buttons_len = unpacker.unpack("xx2xHIHBBIIIiiiiBBH")
+        self.deviceid, self.time, self.sourceid, self.mode, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.same_screen, self.focus, self.buttons_len = unpacker.unpack(
+            "xx2xHIHBBIIIiiiiBBH")
         self.mods = ModifierInfo(unpacker)
         unpacker.pad(GroupInfo)
         self.group = GroupInfo(unpacker)
         unpacker.pad("I")
         self.buttons = xcffib.List(unpacker, "I", self.buttons_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIHBBIIIiiiiBBH", self.deviceid, self.time, self.sourceid, self.mode, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.same_screen, self.focus, self.buttons_len))
+        buf.write(
+            struct.pack(
+                "=HIHBBIIIiiiiBBH",
+                self.deviceid,
+                self.time,
+                self.sourceid,
+                self.mode,
+                self.detail,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.same_screen,
+                self.focus,
+                self.buttons_len))
         buf.write(self.mods.pack())
         buf.write(self.group.pack())
         buf.write(xcffib.pack_list(self.buttons, "I"))
         return buf.getvalue()
 _events[8] = LeaveEvent
+
+
 class FocusInEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.sourceid, self.mode, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.same_screen, self.focus, self.buttons_len = unpacker.unpack("xx2xHIHBBIIIiiiiBBH")
+        self.deviceid, self.time, self.sourceid, self.mode, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.same_screen, self.focus, self.buttons_len = unpacker.unpack(
+            "xx2xHIHBBIIIiiiiBBH")
         self.mods = ModifierInfo(unpacker)
         unpacker.pad(GroupInfo)
         self.group = GroupInfo(unpacker)
         unpacker.pad("I")
         self.buttons = xcffib.List(unpacker, "I", self.buttons_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIHBBIIIiiiiBBH", self.deviceid, self.time, self.sourceid, self.mode, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.same_screen, self.focus, self.buttons_len))
+        buf.write(
+            struct.pack(
+                "=HIHBBIIIiiiiBBH",
+                self.deviceid,
+                self.time,
+                self.sourceid,
+                self.mode,
+                self.detail,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.same_screen,
+                self.focus,
+                self.buttons_len))
         buf.write(self.mods.pack())
         buf.write(self.group.pack())
         buf.write(xcffib.pack_list(self.buttons, "I"))
         return buf.getvalue()
 _events[9] = FocusInEvent
+
+
 class FocusOutEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.sourceid, self.mode, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.same_screen, self.focus, self.buttons_len = unpacker.unpack("xx2xHIHBBIIIiiiiBBH")
+        self.deviceid, self.time, self.sourceid, self.mode, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.same_screen, self.focus, self.buttons_len = unpacker.unpack(
+            "xx2xHIHBBIIIiiiiBBH")
         self.mods = ModifierInfo(unpacker)
         unpacker.pad(GroupInfo)
         self.group = GroupInfo(unpacker)
         unpacker.pad("I")
         self.buttons = xcffib.List(unpacker, "I", self.buttons_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIHBBIIIiiiiBBH", self.deviceid, self.time, self.sourceid, self.mode, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.same_screen, self.focus, self.buttons_len))
+        buf.write(
+            struct.pack(
+                "=HIHBBIIIiiiiBBH",
+                self.deviceid,
+                self.time,
+                self.sourceid,
+                self.mode,
+                self.detail,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.same_screen,
+                self.focus,
+                self.buttons_len))
         buf.write(self.mods.pack())
         buf.write(self.group.pack())
         buf.write(xcffib.pack_list(self.buttons, "I"))
         return buf.getvalue()
 _events[10] = FocusOutEvent
+
+
 class HierarchyMask:
     MasterAdded = 1 << 0
     MasterRemoved = 1 << 1
     SlaveAdded = 1 << 2
     SlaveRemoved = 1 << 3
     SlaveAttached = 1 << 4
     SlaveDetached = 1 << 5
     DeviceEnabled = 1 << 6
     DeviceDisabled = 1 << 7
+
+
 class HierarchyInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.attachment, self.type, self.enabled, self.flags = unpacker.unpack("HHBB2xI")
+        self.deviceid, self.attachment, self.type, self.enabled, self.flags = unpacker.unpack(
+            "HHBB2xI")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HHBB2xI", self.deviceid, self.attachment, self.type, self.enabled, self.flags))
+        buf.write(
+            struct.pack(
+                "=HHBB2xI",
+                self.deviceid,
+                self.attachment,
+                self.type,
+                self.enabled,
+                self.flags))
         return buf.getvalue()
     fixed_size = 12
+
+
 class HierarchyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.flags, self.num_infos = unpacker.unpack("xx2xHIIH10x")
+        self.deviceid, self.time, self.flags, self.num_infos = unpacker.unpack(
+            "xx2xHIIH10x")
         self.infos = xcffib.List(unpacker, HierarchyInfo, self.num_infos)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIH10x", self.deviceid, self.time, self.flags, self.num_infos))
+        buf.write(
+            struct.pack(
+                "=HIIH10x",
+                self.deviceid,
+                self.time,
+                self.flags,
+                self.num_infos))
         buf.write(xcffib.pack_list(self.infos, HierarchyInfo))
         return buf.getvalue()
 _events[11] = HierarchyEvent
+
+
 class PropertyFlag:
     Deleted = 0
     Created = 1
     Modified = 2
+
+
 class PropertyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.property, self.what = unpacker.unpack("xx2xHIIB11x")
+        self.deviceid, self.time, self.property, self.what = unpacker.unpack(
+            "xx2xHIIB11x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIB11x", self.deviceid, self.time, self.property, self.what))
+        buf.write(
+            struct.pack(
+                "=HIIB11x",
+                self.deviceid,
+                self.time,
+                self.property,
+                self.what))
         return buf.getvalue()
 _events[12] = PropertyEvent
+
+
 class RawKeyPressEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack("xx2xHIIHHI4x")
+        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack(
+            "xx2xHIIHHI4x")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIHHI4x", self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIHHI4x",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.sourceid,
+                self.valuators_len,
+                self.flags))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[13] = RawKeyPressEvent
+
+
 class RawKeyReleaseEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack("xx2xHIIHHI4x")
+        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack(
+            "xx2xHIIHHI4x")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIHHI4x", self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIHHI4x",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.sourceid,
+                self.valuators_len,
+                self.flags))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[14] = RawKeyReleaseEvent
+
+
 class RawButtonPressEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack("xx2xHIIHHI4x")
+        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack(
+            "xx2xHIIHHI4x")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIHHI4x", self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIHHI4x",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.sourceid,
+                self.valuators_len,
+                self.flags))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[15] = RawButtonPressEvent
+
+
 class RawButtonReleaseEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack("xx2xHIIHHI4x")
+        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack(
+            "xx2xHIIHHI4x")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIHHI4x", self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIHHI4x",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.sourceid,
+                self.valuators_len,
+                self.flags))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[16] = RawButtonReleaseEvent
+
+
 class RawMotionEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack("xx2xHIIHHI4x")
+        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack(
+            "xx2xHIIHHI4x")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIHHI4x", self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIHHI4x",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.sourceid,
+                self.valuators_len,
+                self.flags))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[17] = RawMotionEvent
+
+
 class TouchEventFlags:
     TouchPendingEnd = 1 << 16
     TouchEmulatingPointer = 1 << 17
+
+
 class TouchBeginEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack("xx2xHIIIIIiiiiHHH2xI")
+        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack(
+            "xx2xHIIIIIiiiiHHH2xI")
         self.mods = ModifierInfo(unpacker)
         unpacker.pad(GroupInfo)
         self.group = GroupInfo(unpacker)
         unpacker.pad("I")
         self.button_mask = xcffib.List(unpacker, "I", self.buttons_len)
         unpacker.pad("I")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIIIIiiiiHHH2xI", self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIIIIiiiiHHH2xI",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.buttons_len,
+                self.valuators_len,
+                self.sourceid,
+                self.flags))
         buf.write(self.mods.pack())
         buf.write(self.group.pack())
         buf.write(xcffib.pack_list(self.button_mask, "I"))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[18] = TouchBeginEvent
+
+
 class TouchUpdateEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack("xx2xHIIIIIiiiiHHH2xI")
+        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack(
+            "xx2xHIIIIIiiiiHHH2xI")
         self.mods = ModifierInfo(unpacker)
         unpacker.pad(GroupInfo)
         self.group = GroupInfo(unpacker)
         unpacker.pad("I")
         self.button_mask = xcffib.List(unpacker, "I", self.buttons_len)
         unpacker.pad("I")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIIIIiiiiHHH2xI", self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIIIIiiiiHHH2xI",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.buttons_len,
+                self.valuators_len,
+                self.sourceid,
+                self.flags))
         buf.write(self.mods.pack())
         buf.write(self.group.pack())
         buf.write(xcffib.pack_list(self.button_mask, "I"))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[19] = TouchUpdateEvent
+
+
 class TouchEndEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack("xx2xHIIIIIiiiiHHH2xI")
+        self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags = unpacker.unpack(
+            "xx2xHIIIIIiiiiHHH2xI")
         self.mods = ModifierInfo(unpacker)
         unpacker.pad(GroupInfo)
         self.group = GroupInfo(unpacker)
         unpacker.pad("I")
         self.button_mask = xcffib.List(unpacker, "I", self.buttons_len)
         unpacker.pad("I")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIIIIiiiiHHH2xI", self.deviceid, self.time, self.detail, self.root, self.event, self.child, self.root_x, self.root_y, self.event_x, self.event_y, self.buttons_len, self.valuators_len, self.sourceid, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIIIIiiiiHHH2xI",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.root,
+                self.event,
+                self.child,
+                self.root_x,
+                self.root_y,
+                self.event_x,
+                self.event_y,
+                self.buttons_len,
+                self.valuators_len,
+                self.sourceid,
+                self.flags))
         buf.write(self.mods.pack())
         buf.write(self.group.pack())
         buf.write(xcffib.pack_list(self.button_mask, "I"))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[20] = TouchEndEvent
+
+
 class TouchOwnershipFlags:
     _None = 0
+
+
 class TouchOwnershipEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.touchid, self.root, self.event, self.child, self.sourceid, self.flags = unpacker.unpack("xx2xHIIIIIH2xI8x")
+        self.deviceid, self.time, self.touchid, self.root, self.event, self.child, self.sourceid, self.flags = unpacker.unpack(
+            "xx2xHIIIIIH2xI8x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIIIIH2xI8x", self.deviceid, self.time, self.touchid, self.root, self.event, self.child, self.sourceid, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIIIIH2xI8x",
+                self.deviceid,
+                self.time,
+                self.touchid,
+                self.root,
+                self.event,
+                self.child,
+                self.sourceid,
+                self.flags))
         return buf.getvalue()
 _events[21] = TouchOwnershipEvent
+
+
 class RawTouchBeginEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack("xx2xHIIHHI4x")
+        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack(
+            "xx2xHIIHHI4x")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIHHI4x", self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIHHI4x",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.sourceid,
+                self.valuators_len,
+                self.flags))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[22] = RawTouchBeginEvent
+
+
 class RawTouchUpdateEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack("xx2xHIIHHI4x")
+        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack(
+            "xx2xHIIHHI4x")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIHHI4x", self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIHHI4x",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.sourceid,
+                self.valuators_len,
+                self.flags))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[23] = RawTouchUpdateEvent
+
+
 class RawTouchEndEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack("xx2xHIIHHI4x")
+        self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags = unpacker.unpack(
+            "xx2xHIIHHI4x")
         self.valuator_mask = xcffib.List(unpacker, "I", self.valuators_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIHHI4x", self.deviceid, self.time, self.detail, self.sourceid, self.valuators_len, self.flags))
+        buf.write(
+            struct.pack(
+                "=HIIHHI4x",
+                self.deviceid,
+                self.time,
+                self.detail,
+                self.sourceid,
+                self.valuators_len,
+                self.flags))
         buf.write(xcffib.pack_list(self.valuator_mask, "I"))
         return buf.getvalue()
 _events[24] = RawTouchEndEvent
+
+
 class BarrierHitEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.eventid, self.root, self.event, self.barrier, self.dtime, self.flags, self.sourceid, self.root_x, self.root_y = unpacker.unpack("xx2xHIIIIIIIH2xii")
+        self.deviceid, self.time, self.eventid, self.root, self.event, self.barrier, self.dtime, self.flags, self.sourceid, self.root_x, self.root_y = unpacker.unpack(
+            "xx2xHIIIIIIIH2xii")
         self.dx = FP3232(unpacker)
         unpacker.pad(FP3232)
         self.dy = FP3232(unpacker)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIIIIIIH2xii", self.deviceid, self.time, self.eventid, self.root, self.event, self.barrier, self.dtime, self.flags, self.sourceid, self.root_x, self.root_y))
+        buf.write(
+            struct.pack(
+                "=HIIIIIIIH2xii",
+                self.deviceid,
+                self.time,
+                self.eventid,
+                self.root,
+                self.event,
+                self.barrier,
+                self.dtime,
+                self.flags,
+                self.sourceid,
+                self.root_x,
+                self.root_y))
         buf.write(self.dx.pack())
         buf.write(self.dy.pack())
         return buf.getvalue()
 _events[25] = BarrierHitEvent
+
+
 class BarrierLeaveEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.deviceid, self.time, self.eventid, self.root, self.event, self.barrier, self.dtime, self.flags, self.sourceid, self.root_x, self.root_y = unpacker.unpack("xx2xHIIIIIIIH2xii")
+        self.deviceid, self.time, self.eventid, self.root, self.event, self.barrier, self.dtime, self.flags, self.sourceid, self.root_x, self.root_y = unpacker.unpack(
+            "xx2xHIIIIIIIH2xii")
         self.dx = FP3232(unpacker)
         unpacker.pad(FP3232)
         self.dy = FP3232(unpacker)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=HIIIIIIIH2xii", self.deviceid, self.time, self.eventid, self.root, self.event, self.barrier, self.dtime, self.flags, self.sourceid, self.root_x, self.root_y))
+        buf.write(
+            struct.pack(
+                "=HIIIIIIIH2xii",
+                self.deviceid,
+                self.time,
+                self.eventid,
+                self.root,
+                self.event,
+                self.barrier,
+                self.dtime,
+                self.flags,
+                self.sourceid,
+                self.root_x,
+                self.root_y))
         buf.write(self.dx.pack())
         buf.write(self.dy.pack())
         return buf.getvalue()
 _events[26] = BarrierLeaveEvent
+
+
 class xinputExtension(xcffib.Extension):
+
     def GetExtensionVersion(self, name_len, name, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2x", name_len))
         buf.write(xcffib.pack_list(name, "c"))
-        return self.send_request(1, buf, GetExtensionVersionCookie, is_checked=is_checked)
+        return self.send_request(
+            1,
+            buf,
+            GetExtensionVersionCookie,
+            is_checked=is_checked)
+
     def ListInputDevices(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(2, buf, ListInputDevicesCookie, is_checked=is_checked)
+        return self.send_request(
+            2,
+            buf,
+            ListInputDevicesCookie,
+            is_checked=is_checked)
+
     def OpenDevice(self, device_id, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x3x", device_id))
-        return self.send_request(3, buf, OpenDeviceCookie, is_checked=is_checked)
+        return self.send_request(
+            3,
+            buf,
+            OpenDeviceCookie,
+            is_checked=is_checked)
+
     def CloseDevice(self, device_id, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x3x", device_id))
         return self.send_request(4, buf, is_checked=is_checked)
+
     def SetDeviceMode(self, device_id, mode, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xB2x", device_id, mode))
-        return self.send_request(5, buf, SetDeviceModeCookie, is_checked=is_checked)
-    def SelectExtensionEvent(self, window, num_classes, classes, is_checked=False):
+        return self.send_request(
+            5,
+            buf,
+            SetDeviceModeCookie,
+            is_checked=is_checked)
+
+    def SelectExtensionEvent(
+            self,
+            window,
+            num_classes,
+            classes,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIH2x", window, num_classes))
         buf.write(xcffib.pack_list(classes, "I"))
         return self.send_request(6, buf, is_checked=is_checked)
+
     def GetSelectedExtensionEvents(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(7, buf, GetSelectedExtensionEventsCookie, is_checked=is_checked)
-    def ChangeDeviceDontPropagateList(self, window, num_classes, mode, classes, is_checked=False):
+        return self.send_request(
+            7,
+            buf,
+            GetSelectedExtensionEventsCookie,
+            is_checked=is_checked)
+
+    def ChangeDeviceDontPropagateList(
+            self,
+            window,
+            num_classes,
+            mode,
+            classes,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIHBx", window, num_classes, mode))
         buf.write(xcffib.pack_list(classes, "I"))
         return self.send_request(8, buf, is_checked=is_checked)
+
     def GetDeviceDontPropagateList(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(9, buf, GetDeviceDontPropagateListCookie, is_checked=is_checked)
+        return self.send_request(
+            9,
+            buf,
+            GetDeviceDontPropagateListCookie,
+            is_checked=is_checked)
+
     def GetDeviceMotionEvents(self, start, stop, device_id, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIB", start, stop, device_id))
-        return self.send_request(10, buf, GetDeviceMotionEventsCookie, is_checked=is_checked)
+        return self.send_request(
+            10,
+            buf,
+            GetDeviceMotionEventsCookie,
+            is_checked=is_checked)
+
     def ChangeKeyboardDevice(self, device_id, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x3x", device_id))
-        return self.send_request(11, buf, ChangeKeyboardDeviceCookie, is_checked=is_checked)
+        return self.send_request(
+            11,
+            buf,
+            ChangeKeyboardDeviceCookie,
+            is_checked=is_checked)
+
     def ChangePointerDevice(self, x_axis, y_axis, device_id, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xBBx", x_axis, y_axis, device_id))
-        return self.send_request(12, buf, ChangePointerDeviceCookie, is_checked=is_checked)
-    def GrabDevice(self, grab_window, time, num_classes, this_device_mode, other_device_mode, owner_events, device_id, classes, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIHBBBB2x", grab_window, time, num_classes, this_device_mode, other_device_mode, owner_events, device_id))
+        return self.send_request(
+            12,
+            buf,
+            ChangePointerDeviceCookie,
+            is_checked=is_checked)
+
+    def GrabDevice(
+            self,
+            grab_window,
+            time,
+            num_classes,
+            this_device_mode,
+            other_device_mode,
+            owner_events,
+            device_id,
+            classes,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIHBBBB2x",
+                grab_window,
+                time,
+                num_classes,
+                this_device_mode,
+                other_device_mode,
+                owner_events,
+                device_id))
         buf.write(xcffib.pack_list(classes, "I"))
-        return self.send_request(13, buf, GrabDeviceCookie, is_checked=is_checked)
+        return self.send_request(
+            13,
+            buf,
+            GrabDeviceCookie,
+            is_checked=is_checked)
+
     def UngrabDevice(self, time, device_id, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIB", time, device_id))
         return self.send_request(14, buf, is_checked=is_checked)
-    def GrabDeviceKey(self, grab_window, num_classes, modifiers, modifier_device, grabbed_device, key, this_device_mode, other_device_mode, owner_events, classes, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIHHBBBBBB2x", grab_window, num_classes, modifiers, modifier_device, grabbed_device, key, this_device_mode, other_device_mode, owner_events))
+
+    def GrabDeviceKey(
+            self,
+            grab_window,
+            num_classes,
+            modifiers,
+            modifier_device,
+            grabbed_device,
+            key,
+            this_device_mode,
+            other_device_mode,
+            owner_events,
+            classes,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIHHBBBBBB2x",
+                grab_window,
+                num_classes,
+                modifiers,
+                modifier_device,
+                grabbed_device,
+                key,
+                this_device_mode,
+                other_device_mode,
+                owner_events))
         buf.write(xcffib.pack_list(classes, "I"))
         return self.send_request(15, buf, is_checked=is_checked)
-    def UngrabDeviceKey(self, grabWindow, modifiers, modifier_device, key, grabbed_device, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIHBBB", grabWindow, modifiers, modifier_device, key, grabbed_device))
+
+    def UngrabDeviceKey(
+            self,
+            grabWindow,
+            modifiers,
+            modifier_device,
+            key,
+            grabbed_device,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIHBBB",
+                grabWindow,
+                modifiers,
+                modifier_device,
+                key,
+                grabbed_device))
         return self.send_request(16, buf, is_checked=is_checked)
-    def GrabDeviceButton(self, grab_window, grabbed_device, modifier_device, num_classes, modifiers, this_device_mode, other_device_mode, button, owner_events, classes, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIBBHHBBBB2x", grab_window, grabbed_device, modifier_device, num_classes, modifiers, this_device_mode, other_device_mode, button, owner_events))
+
+    def GrabDeviceButton(
+            self,
+            grab_window,
+            grabbed_device,
+            modifier_device,
+            num_classes,
+            modifiers,
+            this_device_mode,
+            other_device_mode,
+            button,
+            owner_events,
+            classes,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIBBHHBBBB2x",
+                grab_window,
+                grabbed_device,
+                modifier_device,
+                num_classes,
+                modifiers,
+                this_device_mode,
+                other_device_mode,
+                button,
+                owner_events))
         buf.write(xcffib.pack_list(classes, "I"))
         return self.send_request(17, buf, is_checked=is_checked)
-    def UngrabDeviceButton(self, grab_window, modifiers, modifier_device, button, grabbed_device, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIHBBB", grab_window, modifiers, modifier_device, button, grabbed_device))
+
+    def UngrabDeviceButton(
+            self,
+            grab_window,
+            modifiers,
+            modifier_device,
+            button,
+            grabbed_device,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIHBBB",
+                grab_window,
+                modifiers,
+                modifier_device,
+                button,
+                grabbed_device))
         return self.send_request(18, buf, is_checked=is_checked)
+
     def AllowDeviceEvents(self, time, mode, device_id, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIBB", time, mode, device_id))
         return self.send_request(19, buf, is_checked=is_checked)
+
     def GetDeviceFocus(self, device_id, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x3x", device_id))
-        return self.send_request(20, buf, GetDeviceFocusCookie, is_checked=is_checked)
-    def SetDeviceFocus(self, focus, time, revert_to, device_id, is_checked=False):
+        return self.send_request(
+            20,
+            buf,
+            GetDeviceFocusCookie,
+            is_checked=is_checked)
+
+    def SetDeviceFocus(
+            self,
+            focus,
+            time,
+            revert_to,
+            device_id,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIBB", focus, time, revert_to, device_id))
         return self.send_request(21, buf, is_checked=is_checked)
+
     def GetFeedbackControl(self, device_id, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x3x", device_id))
-        return self.send_request(22, buf, GetFeedbackControlCookie, is_checked=is_checked)
-    def ChangeFeedbackControl(self, mask, device_id, feedback_id, feedback, is_checked=False):
+        return self.send_request(
+            22,
+            buf,
+            GetFeedbackControlCookie,
+            is_checked=is_checked)
+
+    def ChangeFeedbackControl(
+            self,
+            mask,
+            device_id,
+            feedback_id,
+            feedback,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIBB", mask, device_id, feedback_id))
         buf.write(feedback.pack())
         return self.send_request(23, buf, is_checked=is_checked)
-    def GetDeviceKeyMapping(self, device_id, first_keycode, count, is_checked=True):
+
+    def GetDeviceKeyMapping(
+            self,
+            device_id,
+            first_keycode,
+            count,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xBB", device_id, first_keycode, count))
-        return self.send_request(24, buf, GetDeviceKeyMappingCookie, is_checked=is_checked)
-    def ChangeDeviceKeyMapping(self, device_id, first_keycode, keysyms_per_keycode, keycode_count, keysyms, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xBBB", device_id, first_keycode, keysyms_per_keycode, keycode_count))
+        return self.send_request(
+            24,
+            buf,
+            GetDeviceKeyMappingCookie,
+            is_checked=is_checked)
+
+    def ChangeDeviceKeyMapping(
+            self,
+            device_id,
+            first_keycode,
+            keysyms_per_keycode,
+            keycode_count,
+            keysyms,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xBBB",
+                device_id,
+                first_keycode,
+                keysyms_per_keycode,
+                keycode_count))
         buf.write(xcffib.pack_list(keysyms, "I"))
         return self.send_request(25, buf, is_checked=is_checked)
+
     def GetDeviceModifierMapping(self, device_id, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x3x", device_id))
-        return self.send_request(26, buf, GetDeviceModifierMappingCookie, is_checked=is_checked)
-    def SetDeviceModifierMapping(self, device_id, keycodes_per_modifier, keymaps, is_checked=True):
+        return self.send_request(
+            26,
+            buf,
+            GetDeviceModifierMappingCookie,
+            is_checked=is_checked)
+
+    def SetDeviceModifierMapping(
+            self,
+            device_id,
+            keycodes_per_modifier,
+            keymaps,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xBx", device_id, keycodes_per_modifier))
         buf.write(xcffib.pack_list(keymaps, "B"))
-        return self.send_request(27, buf, SetDeviceModifierMappingCookie, is_checked=is_checked)
+        return self.send_request(
+            27,
+            buf,
+            SetDeviceModifierMappingCookie,
+            is_checked=is_checked)
+
     def GetDeviceButtonMapping(self, device_id, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x3x", device_id))
-        return self.send_request(28, buf, GetDeviceButtonMappingCookie, is_checked=is_checked)
-    def SetDeviceButtonMapping(self, device_id, map_size, map, is_checked=True):
+        return self.send_request(
+            28,
+            buf,
+            GetDeviceButtonMappingCookie,
+            is_checked=is_checked)
+
+    def SetDeviceButtonMapping(
+            self,
+            device_id,
+            map_size,
+            map,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xB2x", device_id, map_size))
         buf.write(xcffib.pack_list(map, "B"))
-        return self.send_request(29, buf, SetDeviceButtonMappingCookie, is_checked=is_checked)
+        return self.send_request(
+            29,
+            buf,
+            SetDeviceButtonMappingCookie,
+            is_checked=is_checked)
+
     def QueryDeviceState(self, device_id, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x3x", device_id))
-        return self.send_request(30, buf, QueryDeviceStateCookie, is_checked=is_checked)
-    def SendExtensionEvent(self, destination, device_id, propagate, num_classes, num_events, events, classes, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIBBHB3x", destination, device_id, propagate, num_classes, num_events))
+        return self.send_request(
+            30,
+            buf,
+            QueryDeviceStateCookie,
+            is_checked=is_checked)
+
+    def SendExtensionEvent(
+            self,
+            destination,
+            device_id,
+            propagate,
+            num_classes,
+            num_events,
+            events,
+            classes,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIBBHB3x",
+                destination,
+                device_id,
+                propagate,
+                num_classes,
+                num_events))
         buf.write(xcffib.pack_list(events, "B"))
         buf.write(xcffib.pack_list(classes, "I"))
         return self.send_request(31, buf, is_checked=is_checked)
-    def DeviceBell(self, device_id, feedback_id, feedback_class, percent, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xBBb", device_id, feedback_id, feedback_class, percent))
+
+    def DeviceBell(
+            self,
+            device_id,
+            feedback_id,
+            feedback_class,
+            percent,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xBBb",
+                device_id,
+                feedback_id,
+                feedback_class,
+                percent))
         return self.send_request(32, buf, is_checked=is_checked)
-    def SetDeviceValuators(self, device_id, first_valuator, num_valuators, valuators, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xBBx", device_id, first_valuator, num_valuators))
+
+    def SetDeviceValuators(
+            self,
+            device_id,
+            first_valuator,
+            num_valuators,
+            valuators,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xB2xBBx",
+                device_id,
+                first_valuator,
+                num_valuators))
         buf.write(xcffib.pack_list(valuators, "i"))
-        return self.send_request(33, buf, SetDeviceValuatorsCookie, is_checked=is_checked)
+        return self.send_request(
+            33,
+            buf,
+            SetDeviceValuatorsCookie,
+            is_checked=is_checked)
+
     def GetDeviceControl(self, control_id, device_id, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xHBx", control_id, device_id))
-        return self.send_request(34, buf, GetDeviceControlCookie, is_checked=is_checked)
-    def ChangeDeviceControl(self, control_id, device_id, control, is_checked=True):
+        return self.send_request(
+            34,
+            buf,
+            GetDeviceControlCookie,
+            is_checked=is_checked)
+
+    def ChangeDeviceControl(
+            self,
+            control_id,
+            device_id,
+            control,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xHBx", control_id, device_id))
         buf.write(control.pack())
-        return self.send_request(35, buf, ChangeDeviceControlCookie, is_checked=is_checked)
+        return self.send_request(
+            35,
+            buf,
+            ChangeDeviceControlCookie,
+            is_checked=is_checked)
+
     def ListDeviceProperties(self, device_id, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x3x", device_id))
-        return self.send_request(36, buf, ListDevicePropertiesCookie, is_checked=is_checked)
-    def ChangeDeviceProperty(self, property, type, device_id, format, mode, num_items, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIBBBxI", property, type, device_id, format, mode, num_items))
+        return self.send_request(
+            36,
+            buf,
+            ListDevicePropertiesCookie,
+            is_checked=is_checked)
+
+    def ChangeDeviceProperty(
+            self,
+            property,
+            type,
+            device_id,
+            format,
+            mode,
+            num_items,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIBBBxI",
+                property,
+                type,
+                device_id,
+                format,
+                mode,
+                num_items))
         return self.send_request(37, buf, is_checked=is_checked)
+
     def DeleteDeviceProperty(self, property, device_id, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIB3x", property, device_id))
         return self.send_request(38, buf, is_checked=is_checked)
-    def GetDeviceProperty(self, property, type, offset, len, device_id, delete, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIIBB2x", property, type, offset, len, device_id, delete))
-        return self.send_request(39, buf, GetDevicePropertyCookie, is_checked=is_checked)
+
+    def GetDeviceProperty(
+            self,
+            property,
+            type,
+            offset,
+            len,
+            device_id,
+            delete,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIIBB2x",
+                property,
+                type,
+                offset,
+                len,
+                device_id,
+                delete))
+        return self.send_request(
+            39,
+            buf,
+            GetDevicePropertyCookie,
+            is_checked=is_checked)
+
     def XIQueryPointer(self, window, deviceid, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIH2x", window, deviceid))
-        return self.send_request(40, buf, XIQueryPointerCookie, is_checked=is_checked)
-    def XIWarpPointer(self, src_win, dst_win, src_x, src_y, src_width, src_height, dst_x, dst_y, deviceid, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIiiHHiiH2x", src_win, dst_win, src_x, src_y, src_width, src_height, dst_x, dst_y, deviceid))
+        return self.send_request(
+            40,
+            buf,
+            XIQueryPointerCookie,
+            is_checked=is_checked)
+
+    def XIWarpPointer(
+            self,
+            src_win,
+            dst_win,
+            src_x,
+            src_y,
+            src_width,
+            src_height,
+            dst_x,
+            dst_y,
+            deviceid,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIiiHHiiH2x",
+                src_win,
+                dst_win,
+                src_x,
+                src_y,
+                src_width,
+                src_height,
+                dst_x,
+                dst_y,
+                deviceid))
         return self.send_request(41, buf, is_checked=is_checked)
+
     def XIChangeCursor(self, window, cursor, deviceid, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIH2x", window, cursor, deviceid))
         return self.send_request(42, buf, is_checked=is_checked)
+
     def XIChangeHierarchy(self, num_changes, changes, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2x", num_changes))
         buf.write(xcffib.pack_list(changes, HierarchyChange))
         return self.send_request(43, buf, is_checked=is_checked)
+
     def XISetClientPointer(self, window, deviceid, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIH2x", window, deviceid))
         return self.send_request(44, buf, is_checked=is_checked)
+
     def XIGetClientPointer(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(45, buf, XIGetClientPointerCookie, is_checked=is_checked)
+        return self.send_request(
+            45,
+            buf,
+            XIGetClientPointerCookie,
+            is_checked=is_checked)
+
     def XISelectEvents(self, window, num_mask, masks, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIH2x", window, num_mask))
         buf.write(xcffib.pack_list(masks, EventMask))
         return self.send_request(46, buf, is_checked=is_checked)
+
     def XIQueryVersion(self, major_version, minor_version, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xHH", major_version, minor_version))
-        return self.send_request(47, buf, XIQueryVersionCookie, is_checked=is_checked)
+        return self.send_request(
+            47,
+            buf,
+            XIQueryVersionCookie,
+            is_checked=is_checked)
+
     def XIQueryDevice(self, deviceid, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2x", deviceid))
-        return self.send_request(48, buf, XIQueryDeviceCookie, is_checked=is_checked)
+        return self.send_request(
+            48,
+            buf,
+            XIQueryDeviceCookie,
+            is_checked=is_checked)
+
     def XISetFocus(self, window, time, deviceid, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIH2x", window, time, deviceid))
         return self.send_request(49, buf, is_checked=is_checked)
+
     def XIGetFocus(self, deviceid, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2x", deviceid))
-        return self.send_request(50, buf, XIGetFocusCookie, is_checked=is_checked)
-    def XIGrabDevice(self, window, time, cursor, deviceid, mode, paired_device_mode, owner_events, mask_len, mask, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIHBBBxH", window, time, cursor, deviceid, mode, paired_device_mode, owner_events, mask_len))
+        return self.send_request(
+            50,
+            buf,
+            XIGetFocusCookie,
+            is_checked=is_checked)
+
+    def XIGrabDevice(
+            self,
+            window,
+            time,
+            cursor,
+            deviceid,
+            mode,
+            paired_device_mode,
+            owner_events,
+            mask_len,
+            mask,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIHBBBxH",
+                window,
+                time,
+                cursor,
+                deviceid,
+                mode,
+                paired_device_mode,
+                owner_events,
+                mask_len))
         buf.write(xcffib.pack_list(mask, "I"))
-        return self.send_request(51, buf, XIGrabDeviceCookie, is_checked=is_checked)
+        return self.send_request(
+            51,
+            buf,
+            XIGrabDeviceCookie,
+            is_checked=is_checked)
+
     def XIUngrabDevice(self, time, deviceid, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIH2x", time, deviceid))
         return self.send_request(52, buf, is_checked=is_checked)
-    def XIAllowEvents(self, time, deviceid, event_mode, touchid, grab_window, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIHBxII", time, deviceid, event_mode, touchid, grab_window))
+
+    def XIAllowEvents(
+            self,
+            time,
+            deviceid,
+            event_mode,
+            touchid,
+            grab_window,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIHBxII",
+                time,
+                deviceid,
+                event_mode,
+                touchid,
+                grab_window))
         return self.send_request(53, buf, is_checked=is_checked)
-    def XIPassiveGrabDevice(self, time, grab_window, cursor, detail, deviceid, num_modifiers, mask_len, grab_type, grab_mode, paired_device_mode, owner_events, mask, modifiers, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIIHHHBBBB2x", time, grab_window, cursor, detail, deviceid, num_modifiers, mask_len, grab_type, grab_mode, paired_device_mode, owner_events))
+
+    def XIPassiveGrabDevice(
+            self,
+            time,
+            grab_window,
+            cursor,
+            detail,
+            deviceid,
+            num_modifiers,
+            mask_len,
+            grab_type,
+            grab_mode,
+            paired_device_mode,
+            owner_events,
+            mask,
+            modifiers,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIIHHHBBBB2x",
+                time,
+                grab_window,
+                cursor,
+                detail,
+                deviceid,
+                num_modifiers,
+                mask_len,
+                grab_type,
+                grab_mode,
+                paired_device_mode,
+                owner_events))
         buf.write(xcffib.pack_list(mask, "I"))
         buf.write(xcffib.pack_list(modifiers, "I"))
-        return self.send_request(54, buf, XIPassiveGrabDeviceCookie, is_checked=is_checked)
-    def XIPassiveUngrabDevice(self, grab_window, detail, deviceid, num_modifiers, grab_type, modifiers, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIHHB3x", grab_window, detail, deviceid, num_modifiers, grab_type))
+        return self.send_request(
+            54,
+            buf,
+            XIPassiveGrabDeviceCookie,
+            is_checked=is_checked)
+
+    def XIPassiveUngrabDevice(
+            self,
+            grab_window,
+            detail,
+            deviceid,
+            num_modifiers,
+            grab_type,
+            modifiers,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIHHB3x",
+                grab_window,
+                detail,
+                deviceid,
+                num_modifiers,
+                grab_type))
         buf.write(xcffib.pack_list(modifiers, "I"))
         return self.send_request(55, buf, is_checked=is_checked)
+
     def XIListProperties(self, deviceid, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2x", deviceid))
-        return self.send_request(56, buf, XIListPropertiesCookie, is_checked=is_checked)
-    def XIChangeProperty(self, deviceid, mode, format, property, type, num_items, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xHBBIII", deviceid, mode, format, property, type, num_items))
+        return self.send_request(
+            56,
+            buf,
+            XIListPropertiesCookie,
+            is_checked=is_checked)
+
+    def XIChangeProperty(
+            self,
+            deviceid,
+            mode,
+            format,
+            property,
+            type,
+            num_items,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xHBBIII",
+                deviceid,
+                mode,
+                format,
+                property,
+                type,
+                num_items))
         return self.send_request(57, buf, is_checked=is_checked)
+
     def XIDeleteProperty(self, deviceid, property, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2xI", deviceid, property))
         return self.send_request(58, buf, is_checked=is_checked)
-    def XIGetProperty(self, deviceid, delete, property, type, offset, len, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xHBxIIII", deviceid, delete, property, type, offset, len))
-        return self.send_request(59, buf, XIGetPropertyCookie, is_checked=is_checked)
+
+    def XIGetProperty(
+            self,
+            deviceid,
+            delete,
+            property,
+            type,
+            offset,
+            len,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xHBxIIII",
+                deviceid,
+                delete,
+                property,
+                type,
+                offset,
+                len))
+        return self.send_request(
+            59,
+            buf,
+            XIGetPropertyCookie,
+            is_checked=is_checked)
+
     def XIGetSelectedEvents(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(60, buf, XIGetSelectedEventsCookie, is_checked=is_checked)
-    def XIBarrierReleasePointer(self, num_barriers, barriers, is_checked=False):
+        return self.send_request(
+            60,
+            buf,
+            XIGetSelectedEventsCookie,
+            is_checked=is_checked)
+
+    def XIBarrierReleasePointer(
+            self,
+            num_barriers,
+            barriers,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", num_barriers))
         buf.write(xcffib.pack_list(barriers, BarrierReleasePointerInfo))
         return self.send_request(61, buf, is_checked=is_checked)
 xcffib._add_ext(key, xinputExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/ffi.py` & `xcffib-v0.1.4/xcffib/ffi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from cffi import FFI
-from six.moves import range as srange
 
 ffi = FFI()
 
 CONSTANTS = [
     "X_PROTOCOL",
     "X_PROTOCOL_REVISION",
     "X_TCP_PORT",
@@ -14,16 +13,16 @@
     "XCB_NO_SYMBOL",
 
     "XCB_CONN_ERROR",
     "XCB_CONN_CLOSED_EXT_NOTSUPPORTED",
     "XCB_CONN_CLOSED_MEM_INSUFFICIENT",
     "XCB_CONN_CLOSED_REQ_LEN_EXCEED",
     "XCB_CONN_CLOSED_PARSE_ERR",
-#    "XCB_CONN_CLOSED_INVALID_SCREEN",
-#    "XCB_CONN_CLOSED_FDPASSING_FAILED",
+    #    "XCB_CONN_CLOSED_INVALID_SCREEN",
+    #    "XCB_CONN_CLOSED_FDPASSING_FAILED",
 
     "XCB_REQUEST_CHECKED",
 ]
 
 
 # constants
 ffi.cdef('\n'.join("#define %s ..." % c for c in CONSTANTS))
@@ -219,20 +218,17 @@
 C = ffi.verify("""
     #include <stdlib.h>
     #include <xcb/xcb.h>
     #include <xcb/xcbext.h>
     #include <xcb/render.h>
 """, libraries=['xcb'])
 
-def bytes_to_cdata(bs):
-    buf = ffi.new('char[]', bs)
-    return buf
 
-# cfficairo needs an xcb_visualtype_t
 def visualtype_to_c_struct(vt):
+    # cfficairo needs an xcb_visualtype_t
     s = ffi.new("xcb_visualtype_t *")
 
     s.visual_id = vt.visual_id
     s._class = vt._class
     s.bits_per_rgb_value = vt.bits_per_rgb_value
     s.colormap_entries = vt.colormap_entries
     s.red_mask = vt.red_mask
```

### Comparing `xcffib-v0.1.3/xcffib/dri3.py` & `xcffib-v0.1.4/xcffib/composite.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,106 @@
 import xcffib
 import struct
 import six
-MAJOR_VERSION = 1
-MINOR_VERSION = 0
-key = xcffib.ExtensionKey("DRI3")
+MAJOR_VERSION = 0
+MINOR_VERSION = 4
+key = xcffib.ExtensionKey("Composite")
 _events = {}
 _errors = {}
 from . import xproto
+from . import xfixes
+
+
+class Redirect:
+    Automatic = 0
+    Manual = 1
+
+
 class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.major_version, self.minor_version = unpacker.unpack("xx2x4xII")
+        self.major_version, self.minor_version = unpacker.unpack("xx2x4xII16x")
         self.bufsize = unpacker.offset - base
+
+
 class QueryVersionCookie(xcffib.Cookie):
     reply_type = QueryVersionReply
-class OpenReply(xcffib.Reply):
+
+
+class GetOverlayWindowReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.nfd, = unpacker.unpack("xB2x4x24x")
+        self.overlay_win, = unpacker.unpack("xx2x4xI20x")
         self.bufsize = unpacker.offset - base
-class OpenCookie(xcffib.Cookie):
-    reply_type = OpenReply
-class BufferFromPixmapReply(xcffib.Reply):
-    def __init__(self, unpacker):
-        xcffib.Reply.__init__(self, unpacker)
-        base = unpacker.offset
-        self.nfd, self.size, self.width, self.height, self.stride, self.depth, self.bpp = unpacker.unpack("xB2x4xIHHHBB12x")
-        self.bufsize = unpacker.offset - base
-class BufferFromPixmapCookie(xcffib.Cookie):
-    reply_type = BufferFromPixmapReply
-class FDFromFenceReply(xcffib.Reply):
-    def __init__(self, unpacker):
-        xcffib.Reply.__init__(self, unpacker)
-        base = unpacker.offset
-        self.nfd, = unpacker.unpack("xB2x4x24x")
-        self.bufsize = unpacker.offset - base
-class FDFromFenceCookie(xcffib.Cookie):
-    reply_type = FDFromFenceReply
-class dri3Extension(xcffib.Extension):
-    def QueryVersion(self, major_version, minor_version, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xII", major_version, minor_version))
-        return self.send_request(0, buf, QueryVersionCookie, is_checked=is_checked)
-    def Open(self, drawable, provider, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xII", drawable, provider))
-        return self.send_request(1, buf, OpenCookie, is_checked=is_checked)
-    def PixmapFromBuffer(self, pixmap, drawable, size, width, height, stride, depth, bpp, is_checked=False):
+
+
+class GetOverlayWindowCookie(xcffib.Cookie):
+    reply_type = GetOverlayWindowReply
+
+
+class compositeExtension(xcffib.Extension):
+
+    def QueryVersion(
+            self,
+            client_major_version,
+            client_minor_version,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xII",
+                client_major_version,
+                client_minor_version))
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
+    def RedirectWindow(self, window, update, is_checked=False):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xIB3x", window, update))
+        return self.send_request(1, buf, is_checked=is_checked)
+
+    def RedirectSubwindows(self, window, update, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIHHHBB", pixmap, drawable, size, width, height, stride, depth, bpp))
+        buf.write(struct.pack("=xx2xIB3x", window, update))
         return self.send_request(2, buf, is_checked=is_checked)
-    def BufferFromPixmap(self, pixmap, is_checked=True):
+
+    def UnredirectWindow(self, window, update, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", pixmap))
-        return self.send_request(3, buf, BufferFromPixmapCookie, is_checked=is_checked)
-    def FenceFromFD(self, drawable, fence, initially_triggered, is_checked=False):
+        buf.write(struct.pack("=xx2xIB3x", window, update))
+        return self.send_request(3, buf, is_checked=is_checked)
+
+    def UnredirectSubwindows(self, window, update, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIB3x", drawable, fence, initially_triggered))
+        buf.write(struct.pack("=xx2xIB3x", window, update))
         return self.send_request(4, buf, is_checked=is_checked)
-    def FDFromFence(self, drawable, fence, is_checked=True):
+
+    def CreateRegionFromBorderClip(self, region, window, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xII", drawable, fence))
-        return self.send_request(5, buf, FDFromFenceCookie, is_checked=is_checked)
-xcffib._add_ext(key, dri3Extension, _events, _errors)
+        buf.write(struct.pack("=xx2xII", region, window))
+        return self.send_request(5, buf, is_checked=is_checked)
+
+    def NameWindowPixmap(self, window, pixmap, is_checked=False):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xII", window, pixmap))
+        return self.send_request(6, buf, is_checked=is_checked)
+
+    def GetOverlayWindow(self, window, is_checked=True):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xI", window))
+        return self.send_request(
+            7,
+            buf,
+            GetOverlayWindowCookie,
+            is_checked=is_checked)
+
+    def ReleaseOverlayWindow(self, window, is_checked=False):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xI", window))
+        return self.send_request(8, buf, is_checked=is_checked)
+xcffib._add_ext(key, compositeExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/damage.py` & `xcffib-v0.1.4/xcffib/damage.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,58 +4,95 @@
 MAJOR_VERSION = 1
 MINOR_VERSION = 1
 key = xcffib.ExtensionKey("DAMAGE")
 _events = {}
 _errors = {}
 from . import xproto
 from . import xfixes
+
+
 class ReportLevel:
     RawRectangles = 0
     DeltaRectangles = 1
     BoundingBox = 2
     NonEmpty = 3
+
+
 class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.major_version, self.minor_version = unpacker.unpack("xx2x4xII16x")
         self.bufsize = unpacker.offset - base
+
+
 class QueryVersionCookie(xcffib.Cookie):
     reply_type = QueryVersionReply
+
+
 class NotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.level, self.drawable, self.damage, self.timestamp = unpacker.unpack("xB2xIII")
+        self.level, self.drawable, self.damage, self.timestamp = unpacker.unpack(
+            "xB2xIII")
         self.area = xproto.RECTANGLE(unpacker)
         unpacker.pad(xproto.RECTANGLE)
         self.geometry = xproto.RECTANGLE(unpacker)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIII", self.level, self.drawable, self.damage, self.timestamp))
+        buf.write(
+            struct.pack(
+                "=BIII",
+                self.level,
+                self.drawable,
+                self.damage,
+                self.timestamp))
         buf.write(self.area.pack())
         buf.write(self.geometry.pack())
         return buf.getvalue()
 _events[0] = NotifyEvent
+
+
 class damageExtension(xcffib.Extension):
-    def QueryVersion(self, client_major_version, client_minor_version, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xII", client_major_version, client_minor_version))
-        return self.send_request(0, buf, QueryVersionCookie, is_checked=is_checked)
+
+    def QueryVersion(
+            self,
+            client_major_version,
+            client_minor_version,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xII",
+                client_major_version,
+                client_minor_version))
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
     def Create(self, damage, drawable, level, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIB3x", damage, drawable, level))
         return self.send_request(1, buf, is_checked=is_checked)
+
     def Destroy(self, damage, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", damage))
         return self.send_request(2, buf, is_checked=is_checked)
+
     def Subtract(self, damage, repair, parts, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", damage, repair, parts))
         return self.send_request(3, buf, is_checked=is_checked)
+
     def Add(self, drawable, region, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", drawable, region))
         return self.send_request(4, buf, is_checked=is_checked)
 xcffib._add_ext(key, damageExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/xvmc.py` & `xcffib-v0.1.4/xcffib/xvmc.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,112 +3,225 @@
 import six
 MAJOR_VERSION = 1
 MINOR_VERSION = 1
 key = xcffib.ExtensionKey("XVideo-MotionCompensation")
 _events = {}
 _errors = {}
 from . import xv
+
+
 class SurfaceInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.id, self.chroma_format, self.pad0, self.max_width, self.max_height, self.subpicture_max_width, self.subpicture_max_height, self.mc_type, self.flags = unpacker.unpack("IHHHHHHII")
+        self.id, self.chroma_format, self.pad0, self.max_width, self.max_height, self.subpicture_max_width, self.subpicture_max_height, self.mc_type, self.flags = unpacker.unpack(
+            "IHHHHHHII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHHHHHHII", self.id, self.chroma_format, self.pad0, self.max_width, self.max_height, self.subpicture_max_width, self.subpicture_max_height, self.mc_type, self.flags))
+        buf.write(
+            struct.pack(
+                "=IHHHHHHII",
+                self.id,
+                self.chroma_format,
+                self.pad0,
+                self.max_width,
+                self.max_height,
+                self.subpicture_max_width,
+                self.subpicture_max_height,
+                self.mc_type,
+                self.flags))
         return buf.getvalue()
     fixed_size = 24
+
+
 class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.major, self.minor = unpacker.unpack("xx2x4xII")
         self.bufsize = unpacker.offset - base
+
+
 class QueryVersionCookie(xcffib.Cookie):
     reply_type = QueryVersionReply
+
+
 class ListSurfaceTypesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num, = unpacker.unpack("xx2x4xI20x")
         self.surfaces = xcffib.List(unpacker, SurfaceInfo, self.num)
         self.bufsize = unpacker.offset - base
+
+
 class ListSurfaceTypesCookie(xcffib.Cookie):
     reply_type = ListSurfaceTypesReply
+
+
 class CreateContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.width_actual, self.height_actual, self.flags_return = unpacker.unpack("xx2x4xHHI20x")
+        self.width_actual, self.height_actual, self.flags_return = unpacker.unpack(
+            "xx2x4xHHI20x")
         self.priv_data = xcffib.List(unpacker, "I", self.length)
         self.bufsize = unpacker.offset - base
+
+
 class CreateContextCookie(xcffib.Cookie):
     reply_type = CreateContextReply
+
+
 class CreateSurfaceReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x24x")
         self.priv_data = xcffib.List(unpacker, "I", self.length)
         self.bufsize = unpacker.offset - base
+
+
 class CreateSurfaceCookie(xcffib.Cookie):
     reply_type = CreateSurfaceReply
+
+
 class CreateSubpictureReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.width_actual, self.height_actual, self.num_palette_entries, self.entry_bytes = unpacker.unpack("xx2x4xHHHH")
+        self.width_actual, self.height_actual, self.num_palette_entries, self.entry_bytes = unpacker.unpack(
+            "xx2x4xHHHH")
         self.component_order = xcffib.List(unpacker, "B", 4)
         unpacker.unpack("12x")
         unpacker.pad("I")
         self.priv_data = xcffib.List(unpacker, "I", self.length)
         self.bufsize = unpacker.offset - base
+
+
 class CreateSubpictureCookie(xcffib.Cookie):
     reply_type = CreateSubpictureReply
+
+
 class ListSubpictureTypesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num, = unpacker.unpack("xx2x4xI20x")
         self.types = xcffib.List(unpacker, xv.ImageFormatInfo, self.num)
         self.bufsize = unpacker.offset - base
+
+
 class ListSubpictureTypesCookie(xcffib.Cookie):
     reply_type = ListSubpictureTypesReply
+
+
 class xvmcExtension(xcffib.Extension):
+
     def QueryVersion(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(0, buf, QueryVersionCookie, is_checked=is_checked)
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
     def ListSurfaceTypes(self, port_id, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", port_id))
-        return self.send_request(1, buf, ListSurfaceTypesCookie, is_checked=is_checked)
-    def CreateContext(self, context_id, port_id, surface_id, width, height, flags, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIHHI", context_id, port_id, surface_id, width, height, flags))
-        return self.send_request(2, buf, CreateContextCookie, is_checked=is_checked)
+        return self.send_request(
+            1,
+            buf,
+            ListSurfaceTypesCookie,
+            is_checked=is_checked)
+
+    def CreateContext(
+            self,
+            context_id,
+            port_id,
+            surface_id,
+            width,
+            height,
+            flags,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIHHI",
+                context_id,
+                port_id,
+                surface_id,
+                width,
+                height,
+                flags))
+        return self.send_request(
+            2,
+            buf,
+            CreateContextCookie,
+            is_checked=is_checked)
+
     def DestroyContext(self, context_id, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context_id))
         return self.send_request(3, buf, is_checked=is_checked)
+
     def CreateSurface(self, surface_id, context_id, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", surface_id, context_id))
-        return self.send_request(4, buf, CreateSurfaceCookie, is_checked=is_checked)
+        return self.send_request(
+            4,
+            buf,
+            CreateSurfaceCookie,
+            is_checked=is_checked)
+
     def DestroySurface(self, surface_id, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", surface_id))
         return self.send_request(5, buf, is_checked=is_checked)
-    def CreateSubpicture(self, subpicture_id, context, xvimage_id, width, height, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIHH", subpicture_id, context, xvimage_id, width, height))
-        return self.send_request(6, buf, CreateSubpictureCookie, is_checked=is_checked)
+
+    def CreateSubpicture(
+            self,
+            subpicture_id,
+            context,
+            xvimage_id,
+            width,
+            height,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIHH",
+                subpicture_id,
+                context,
+                xvimage_id,
+                width,
+                height))
+        return self.send_request(
+            6,
+            buf,
+            CreateSubpictureCookie,
+            is_checked=is_checked)
+
     def DestroySubpicture(self, subpicture_id, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", subpicture_id))
         return self.send_request(7, buf, is_checked=is_checked)
+
     def ListSubpictureTypes(self, port_id, surface_id, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", port_id, surface_id))
-        return self.send_request(8, buf, ListSubpictureTypesCookie, is_checked=is_checked)
+        return self.send_request(
+            8,
+            buf,
+            ListSubpictureTypesCookie,
+            is_checked=is_checked)
 xcffib._add_ext(key, xvmcExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/sync.py` & `xcffib-v0.1.4/xcffib/xfixes.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,280 +1,468 @@
 import xcffib
 import struct
 import six
-MAJOR_VERSION = 3
-MINOR_VERSION = 1
-key = xcffib.ExtensionKey("SYNC")
+MAJOR_VERSION = 5
+MINOR_VERSION = 0
+key = xcffib.ExtensionKey("XFIXES")
 _events = {}
 _errors = {}
 from . import xproto
-class ALARMSTATE:
-    Active = 0
-    Inactive = 1
-    Destroyed = 2
-class TESTTYPE:
-    PositiveTransition = 0
-    NegativeTransition = 1
-    PositiveComparison = 2
-    NegativeComparison = 3
-class VALUETYPE:
-    Absolute = 0
-    Relative = 1
-class CA:
-    Counter = 1 << 0
-    ValueType = 1 << 1
-    Value = 1 << 2
-    TestType = 1 << 3
-    Delta = 1 << 4
-    Events = 1 << 5
-class INT64(xcffib.Struct):
+from . import render
+from . import shape
+
+
+class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
-        xcffib.Struct.__init__(self, unpacker)
-        base = unpacker.offset
-        self.hi, self.lo = unpacker.unpack("iI")
-        self.bufsize = unpacker.offset - base
-    def pack(self):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=iI", self.hi, self.lo))
-        return buf.getvalue()
-    fixed_size = 8
-class SYSTEMCOUNTER(xcffib.Struct):
-    def __init__(self, unpacker):
-        xcffib.Struct.__init__(self, unpacker)
-        base = unpacker.offset
-        self.counter, = unpacker.unpack("I")
-        self.resolution = INT64(unpacker)
-        self.name_len, = unpacker.unpack("H")
-        unpacker.pad("c")
-        self.name = xcffib.List(unpacker, "c", self.name_len)
-        self.bufsize = unpacker.offset - base
-    def pack(self):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=IH", self.counter, self.name_len))
-        buf.write(self.resolution.pack())
-        buf.write(xcffib.pack_list(self.name, "c"))
-        return buf.getvalue()
-class TRIGGER(xcffib.Struct):
-    def __init__(self, unpacker):
-        xcffib.Struct.__init__(self, unpacker)
-        base = unpacker.offset
-        self.counter, self.wait_type = unpacker.unpack("II")
-        self.wait_value = INT64(unpacker)
-        self.test_type, = unpacker.unpack("I")
-        self.bufsize = unpacker.offset - base
-    def pack(self):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=III", self.counter, self.wait_type, self.test_type))
-        buf.write(self.wait_value.pack())
-        return buf.getvalue()
-class WAITCONDITION(xcffib.Struct):
-    def __init__(self, unpacker):
-        xcffib.Struct.__init__(self, unpacker)
+        xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.trigger = TRIGGER(unpacker)
-        unpacker.pad(INT64)
-        self.event_threshold = INT64(unpacker)
+        self.major_version, self.minor_version = unpacker.unpack("xx2x4xII16x")
         self.bufsize = unpacker.offset - base
-    def pack(self):
-        buf = six.BytesIO()
-        buf.write(self.trigger.pack())
-        buf.write(self.event_threshold.pack())
-        return buf.getvalue()
-class CounterError(xcffib.Error):
+
+
+class QueryVersionCookie(xcffib.Cookie):
+    reply_type = QueryVersionReply
+
+
+class SaveSetMode:
+    Insert = 0
+    Delete = 1
+
+
+class SaveSetTarget:
+    Nearest = 0
+    Root = 1
+
+
+class SaveSetMapping:
+    Map = 0
+    Unmap = 1
+
+
+class SelectionEvent:
+    SetSelectionOwner = 0
+    SelectionWindowDestroy = 1
+    SelectionClientClose = 2
+
+
+class SelectionEventMask:
+    SetSelectionOwner = 1 << 0
+    SelectionWindowDestroy = 1 << 1
+    SelectionClientClose = 1 << 2
+
+
+class SelectionNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
-        xcffib.Error.__init__(self, unpacker)
+        xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_counter, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB")
+        self.subtype, self.window, self.owner, self.selection, self.timestamp, self.selection_timestamp = unpacker.unpack(
+            "xB2xIIIII8x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB", self.bad_counter, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=BIIIII8x",
+                self.subtype,
+                self.window,
+                self.owner,
+                self.selection,
+                self.timestamp,
+                self.selection_timestamp))
         return buf.getvalue()
-BadCounter = CounterError
-_errors[0] = CounterError
-class AlarmError(xcffib.Error):
+_events[0] = SelectionNotifyEvent
+
+
+class CursorNotify:
+    DisplayCursor = 0
+
+
+class CursorNotifyMask:
+    DisplayCursor = 1 << 0
+
+
+class CursorNotifyEvent(xcffib.Event):
+
     def __init__(self, unpacker):
-        xcffib.Error.__init__(self, unpacker)
+        xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_alarm, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB")
+        self.subtype, self.window, self.cursor_serial, self.timestamp, self.name = unpacker.unpack(
+            "xB2xIIII12x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB", self.bad_alarm, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=BIIII12x",
+                self.subtype,
+                self.window,
+                self.cursor_serial,
+                self.timestamp,
+                self.name))
         return buf.getvalue()
-BadAlarm = AlarmError
-_errors[1] = AlarmError
-class InitializeReply(xcffib.Reply):
+_events[1] = CursorNotifyEvent
+
+
+class GetCursorImageReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.major_version, self.minor_version = unpacker.unpack("xx2x4xBB22x")
-        self.bufsize = unpacker.offset - base
-class InitializeCookie(xcffib.Cookie):
-    reply_type = InitializeReply
-class ListSystemCountersReply(xcffib.Reply):
-    def __init__(self, unpacker):
-        xcffib.Reply.__init__(self, unpacker)
-        base = unpacker.offset
-        self.counters_len, = unpacker.unpack("xx2x4xI20x")
-        self.counters = xcffib.List(unpacker, SYSTEMCOUNTER, self.counters_len)
-        self.bufsize = unpacker.offset - base
-class ListSystemCountersCookie(xcffib.Cookie):
-    reply_type = ListSystemCountersReply
-class QueryCounterReply(xcffib.Reply):
+        self.x, self.y, self.width, self.height, self.xhot, self.yhot, self.cursor_serial = unpacker.unpack(
+            "xx2x4xhhHHHHI8x")
+        self.cursor_image = xcffib.List(
+            unpacker,
+            "I",
+            self.width *
+            self.height)
+        self.bufsize = unpacker.offset - base
+
+
+class GetCursorImageCookie(xcffib.Cookie):
+    reply_type = GetCursorImageReply
+
+
+class Region:
+    _None = 0
+
+
+class FetchRegionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x")
-        self.counter_value = INT64(unpacker)
-        self.bufsize = unpacker.offset - base
-class QueryCounterCookie(xcffib.Cookie):
-    reply_type = QueryCounterReply
-class QueryAlarmReply(xcffib.Reply):
+        self.extents = xproto.RECTANGLE(unpacker)
+        unpacker.unpack("16x")
+        unpacker.pad(xproto.RECTANGLE)
+        self.rectangles = xcffib.List(
+            unpacker,
+            xproto.RECTANGLE,
+            self.length // 2)
+        self.bufsize = unpacker.offset - base
+
+
+class FetchRegionCookie(xcffib.Cookie):
+    reply_type = FetchRegionReply
+
+
+class GetCursorNameReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        unpacker.unpack("xx2x4x")
-        self.trigger = TRIGGER(unpacker)
-        unpacker.pad(INT64)
-        self.delta = INT64(unpacker)
-        self.events, self.state = unpacker.unpack("BB2x")
-        self.bufsize = unpacker.offset - base
-class QueryAlarmCookie(xcffib.Cookie):
-    reply_type = QueryAlarmReply
-class GetPriorityReply(xcffib.Reply):
-    def __init__(self, unpacker):
-        xcffib.Reply.__init__(self, unpacker)
-        base = unpacker.offset
-        self.priority, = unpacker.unpack("xx2x4xi")
+        self.atom, self.nbytes = unpacker.unpack("xx2x4xIH18x")
+        self.name = xcffib.List(unpacker, "c", self.nbytes)
         self.bufsize = unpacker.offset - base
-class GetPriorityCookie(xcffib.Cookie):
-    reply_type = GetPriorityReply
-class QueryFenceReply(xcffib.Reply):
+
+
+class GetCursorNameCookie(xcffib.Cookie):
+    reply_type = GetCursorNameReply
+
+
+class GetCursorImageAndNameReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.triggered, = unpacker.unpack("xx2x4xB23x")
-        self.bufsize = unpacker.offset - base
-class QueryFenceCookie(xcffib.Cookie):
-    reply_type = QueryFenceReply
-class CounterNotifyEvent(xcffib.Event):
-    def __init__(self, unpacker):
-        xcffib.Event.__init__(self, unpacker)
-        base = unpacker.offset
-        self.kind, self.counter = unpacker.unpack("xB2xI")
-        self.wait_value = INT64(unpacker)
-        unpacker.pad(INT64)
-        self.counter_value = INT64(unpacker)
-        self.timestamp, self.count, self.destroyed = unpacker.unpack("IHBx")
-        self.bufsize = unpacker.offset - base
-    def pack(self):
+        self.x, self.y, self.width, self.height, self.xhot, self.yhot, self.cursor_serial, self.cursor_atom, self.nbytes = unpacker.unpack(
+            "xx2x4xhhHHHHIIH2x")
+        self.name = xcffib.List(unpacker, "c", self.nbytes)
+        unpacker.pad("I")
+        self.cursor_image = xcffib.List(
+            unpacker,
+            "I",
+            self.width *
+            self.height)
+        self.bufsize = unpacker.offset - base
+
+
+class GetCursorImageAndNameCookie(xcffib.Cookie):
+    reply_type = GetCursorImageAndNameReply
+
+
+class BarrierDirections:
+    PositiveX = 1 << 0
+    PositiveY = 1 << 1
+    NegativeX = 1 << 2
+    NegativeY = 1 << 3
+
+
+class xfixesExtension(xcffib.Extension):
+
+    def QueryVersion(
+            self,
+            client_major_version,
+            client_minor_version,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xII",
+                client_major_version,
+                client_minor_version))
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
+    def ChangeSaveSet(self, mode, target, map, window, is_checked=False):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xB2xBBxI", mode, target, map, window))
+        return self.send_request(1, buf, is_checked=is_checked)
+
+    def SelectSelectionInput(
+            self,
+            window,
+            selection,
+            event_mask,
+            is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIHBx", self.kind, self.counter, self.timestamp, self.count, self.destroyed))
-        buf.write(self.wait_value.pack())
-        buf.write(self.counter_value.pack())
-        return buf.getvalue()
-_events[0] = CounterNotifyEvent
-class AlarmNotifyEvent(xcffib.Event):
-    def __init__(self, unpacker):
-        xcffib.Event.__init__(self, unpacker)
-        base = unpacker.offset
-        self.kind, self.alarm = unpacker.unpack("xB2xI")
-        self.counter_value = INT64(unpacker)
-        unpacker.pad(INT64)
-        self.alarm_value = INT64(unpacker)
-        self.timestamp, self.state = unpacker.unpack("IB3x")
-        self.bufsize = unpacker.offset - base
-    def pack(self):
+        buf.write(struct.pack("=xx2xIII", window, selection, event_mask))
+        return self.send_request(2, buf, is_checked=is_checked)
+
+    def SelectCursorInput(self, window, event_mask, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=BIIB3x", self.kind, self.alarm, self.timestamp, self.state))
-        buf.write(self.counter_value.pack())
-        buf.write(self.alarm_value.pack())
-        return buf.getvalue()
-_events[1] = AlarmNotifyEvent
-class syncExtension(xcffib.Extension):
-    def Initialize(self, desired_major_version, desired_minor_version, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xB2xB", desired_major_version, desired_minor_version))
-        return self.send_request(0, buf, InitializeCookie, is_checked=is_checked)
-    def ListSystemCounters(self, is_checked=True):
+        buf.write(struct.pack("=xx2xII", window, event_mask))
+        return self.send_request(3, buf, is_checked=is_checked)
+
+    def GetCursorImage(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(1, buf, ListSystemCountersCookie, is_checked=is_checked)
-    def CreateCounter(self, id, initial_value, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", id))
-        buf.write(initial_value.pack())
-        return self.send_request(2, buf, is_checked=is_checked)
-    def DestroyCounter(self, counter, is_checked=False):
+        return self.send_request(
+            4,
+            buf,
+            GetCursorImageCookie,
+            is_checked=is_checked)
+
+    def CreateRegion(self, region, rectangles, is_checked=False):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xI", region))
+        buf.write(xcffib.pack_list(rectangles, xproto.RECTANGLE))
+        return self.send_request(5, buf, is_checked=is_checked)
+
+    def CreateRegionFromBitmap(self, region, bitmap, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", counter))
+        buf.write(struct.pack("=xx2xII", region, bitmap))
         return self.send_request(6, buf, is_checked=is_checked)
-    def QueryCounter(self, counter, is_checked=True):
+
+    def CreateRegionFromWindow(self, region, window, kind, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", counter))
-        return self.send_request(5, buf, QueryCounterCookie, is_checked=is_checked)
-    def Await(self, wait_list, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2x"))
-        buf.write(xcffib.pack_list(wait_list, WAITCONDITION))
+        buf.write(struct.pack("=xx2xIIB3x", region, window, kind))
         return self.send_request(7, buf, is_checked=is_checked)
-    def ChangeCounter(self, counter, amount, is_checked=False):
+
+    def CreateRegionFromGC(self, region, gc, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", counter))
-        buf.write(amount.pack())
-        return self.send_request(4, buf, is_checked=is_checked)
-    def SetCounter(self, counter, value, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", counter))
-        buf.write(value.pack())
-        return self.send_request(3, buf, is_checked=is_checked)
-    def CreateAlarm(self, id, value_mask, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xII", id, value_mask))
+        buf.write(struct.pack("=xx2xII", region, gc))
         return self.send_request(8, buf, is_checked=is_checked)
-    def ChangeAlarm(self, id, value_mask, is_checked=False):
+
+    def CreateRegionFromPicture(self, region, picture, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xII", id, value_mask))
+        buf.write(struct.pack("=xx2xII", region, picture))
         return self.send_request(9, buf, is_checked=is_checked)
-    def DestroyAlarm(self, alarm, is_checked=False):
+
+    def DestroyRegion(self, region, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", alarm))
-        return self.send_request(11, buf, is_checked=is_checked)
-    def QueryAlarm(self, alarm, is_checked=True):
+        buf.write(struct.pack("=xx2xI", region))
+        return self.send_request(10, buf, is_checked=is_checked)
+
+    def SetRegion(self, region, rectangles, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", alarm))
-        return self.send_request(10, buf, QueryAlarmCookie, is_checked=is_checked)
-    def SetPriority(self, id, priority, is_checked=False):
+        buf.write(struct.pack("=xx2xI", region))
+        buf.write(xcffib.pack_list(rectangles, xproto.RECTANGLE))
+        return self.send_request(11, buf, is_checked=is_checked)
+
+    def CopyRegion(self, source, destination, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIi", id, priority))
+        buf.write(struct.pack("=xx2xII", source, destination))
         return self.send_request(12, buf, is_checked=is_checked)
-    def GetPriority(self, id, is_checked=True):
+
+    def UnionRegion(self, source1, source2, destination, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", id))
-        return self.send_request(13, buf, GetPriorityCookie, is_checked=is_checked)
-    def CreateFence(self, drawable, fence, initially_triggered, is_checked=False):
+        buf.write(struct.pack("=xx2xIII", source1, source2, destination))
+        return self.send_request(13, buf, is_checked=is_checked)
+
+    def IntersectRegion(self, source1, source2, destination, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIB", drawable, fence, initially_triggered))
+        buf.write(struct.pack("=xx2xIII", source1, source2, destination))
         return self.send_request(14, buf, is_checked=is_checked)
-    def TriggerFence(self, fence, is_checked=False):
+
+    def SubtractRegion(self, source1, source2, destination, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", fence))
+        buf.write(struct.pack("=xx2xIII", source1, source2, destination))
         return self.send_request(15, buf, is_checked=is_checked)
-    def ResetFence(self, fence, is_checked=False):
+
+    def InvertRegion(self, source, destination, bounds, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", fence))
+        buf.write(struct.pack("=xx2xII", source, destination))
+        buf.write(bounds.pack())
         return self.send_request(16, buf, is_checked=is_checked)
-    def DestroyFence(self, fence, is_checked=False):
+
+    def TranslateRegion(self, region, dx, dy, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", fence))
+        buf.write(struct.pack("=xx2xIhh", region, dx, dy))
         return self.send_request(17, buf, is_checked=is_checked)
-    def QueryFence(self, fence, is_checked=True):
+
+    def RegionExtents(self, source, destination, is_checked=False):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xI", fence))
-        return self.send_request(18, buf, QueryFenceCookie, is_checked=is_checked)
-    def AwaitFence(self, fence_list, is_checked=False):
+        buf.write(struct.pack("=xx2xII", source, destination))
+        return self.send_request(18, buf, is_checked=is_checked)
+
+    def FetchRegion(self, region, is_checked=True):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xI", region))
+        return self.send_request(
+            19,
+            buf,
+            FetchRegionCookie,
+            is_checked=is_checked)
+
+    def SetGCClipRegion(
+            self,
+            gc,
+            region,
+            x_origin,
+            y_origin,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xIIhh", gc, region, x_origin, y_origin))
+        return self.send_request(20, buf, is_checked=is_checked)
+
+    def SetWindowShapeRegion(
+            self,
+            dest,
+            dest_kind,
+            x_offset,
+            y_offset,
+            region,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIB3xhhI",
+                dest,
+                dest_kind,
+                x_offset,
+                y_offset,
+                region))
+        return self.send_request(21, buf, is_checked=is_checked)
+
+    def SetPictureClipRegion(
+            self,
+            picture,
+            region,
+            x_origin,
+            y_origin,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIhh",
+                picture,
+                region,
+                x_origin,
+                y_origin))
+        return self.send_request(22, buf, is_checked=is_checked)
+
+    def SetCursorName(self, cursor, nbytes, name, is_checked=False):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xIH2x", cursor, nbytes))
+        buf.write(xcffib.pack_list(name, "c"))
+        return self.send_request(23, buf, is_checked=is_checked)
+
+    def GetCursorName(self, cursor, is_checked=True):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xI", cursor))
+        return self.send_request(
+            24,
+            buf,
+            GetCursorNameCookie,
+            is_checked=is_checked)
+
+    def GetCursorImageAndName(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        buf.write(xcffib.pack_list(fence_list, "I"))
-        return self.send_request(19, buf, is_checked=is_checked)
-xcffib._add_ext(key, syncExtension, _events, _errors)
+        return self.send_request(
+            25,
+            buf,
+            GetCursorImageAndNameCookie,
+            is_checked=is_checked)
+
+    def ChangeCursor(self, source, destination, is_checked=False):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xII", source, destination))
+        return self.send_request(26, buf, is_checked=is_checked)
+
+    def ChangeCursorByName(self, src, nbytes, name, is_checked=False):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xIH2x", src, nbytes))
+        buf.write(xcffib.pack_list(name, "c"))
+        return self.send_request(27, buf, is_checked=is_checked)
+
+    def ExpandRegion(
+            self,
+            source,
+            destination,
+            left,
+            right,
+            top,
+            bottom,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIHHHH",
+                source,
+                destination,
+                left,
+                right,
+                top,
+                bottom))
+        return self.send_request(28, buf, is_checked=is_checked)
+
+    def HideCursor(self, window, is_checked=False):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xI", window))
+        return self.send_request(29, buf, is_checked=is_checked)
+
+    def ShowCursor(self, window, is_checked=False):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xI", window))
+        return self.send_request(30, buf, is_checked=is_checked)
+
+    def CreatePointerBarrier(
+            self,
+            barrier,
+            window,
+            x1,
+            y1,
+            x2,
+            y2,
+            directions,
+            num_devices,
+            devices,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIHHHHI2xH",
+                barrier,
+                window,
+                x1,
+                y1,
+                x2,
+                y2,
+                directions,
+                num_devices))
+        buf.write(xcffib.pack_list(devices, "H"))
+        return self.send_request(31, buf, is_checked=is_checked)
+
+    def DeletePointerBarrier(self, barrier, is_checked=False):
+        buf = six.BytesIO()
+        buf.write(struct.pack("=xx2xI", barrier))
+        return self.send_request(32, buf, is_checked=is_checked)
+xcffib._add_ext(key, xfixesExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/glx.py` & `xcffib-v0.1.4/xcffib/glx.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,246 +3,448 @@
 import six
 MAJOR_VERSION = 1
 MINOR_VERSION = 4
 key = xcffib.ExtensionKey("GLX")
 _events = {}
 _errors = {}
 from . import xproto
+
+
 class GenericError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB21x")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHB21x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB21x", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHB21x",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadGeneric = GenericError
 _errors[-1] = GenericError
+
+
 class BadContextError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB21x")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHB21x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB21x", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHB21x",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadBadContext = BadContextError
 _errors[0] = BadContextError
+
+
 class BadContextStateError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB21x")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHB21x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB21x", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHB21x",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadBadContextState = BadContextStateError
 _errors[1] = BadContextStateError
+
+
 class BadDrawableError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB21x")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHB21x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB21x", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHB21x",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadBadDrawable = BadDrawableError
 _errors[2] = BadDrawableError
+
+
 class BadPixmapError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB21x")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHB21x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB21x", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHB21x",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadBadPixmap = BadPixmapError
 _errors[3] = BadPixmapError
+
+
 class BadContextTagError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB21x")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHB21x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB21x", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHB21x",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadBadContextTag = BadContextTagError
 _errors[4] = BadContextTagError
+
+
 class BadCurrentWindowError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB21x")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHB21x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB21x", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHB21x",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadBadCurrentWindow = BadCurrentWindowError
 _errors[5] = BadCurrentWindowError
+
+
 class BadRenderRequestError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB21x")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHB21x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB21x", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHB21x",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadBadRenderRequest = BadRenderRequestError
 _errors[6] = BadRenderRequestError
+
+
 class BadLargeRequestError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB21x")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHB21x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB21x", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHB21x",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadBadLargeRequest = BadLargeRequestError
 _errors[7] = BadLargeRequestError
+
+
 class UnsupportedPrivateRequestError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB21x")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHB21x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB21x", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHB21x",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadUnsupportedPrivateRequest = UnsupportedPrivateRequestError
 _errors[8] = UnsupportedPrivateRequestError
+
+
 class BadFBConfigError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB21x")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHB21x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB21x", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHB21x",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadBadFBConfig = BadFBConfigError
 _errors[9] = BadFBConfigError
+
+
 class BadPbufferError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB21x")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHB21x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB21x", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHB21x",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadBadPbuffer = BadPbufferError
 _errors[10] = BadPbufferError
+
+
 class BadCurrentDrawableError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB21x")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHB21x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB21x", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHB21x",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadBadCurrentDrawable = BadCurrentDrawableError
 _errors[11] = BadCurrentDrawableError
+
+
 class BadWindowError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB21x")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHB21x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB21x", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHB21x",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadBadWindow = BadWindowError
 _errors[12] = BadWindowError
+
+
 class GLXBadProfileARBError(xcffib.Error):
+
     def __init__(self, unpacker):
         xcffib.Error.__init__(self, unpacker)
         base = unpacker.offset
-        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack("xx2xIHB21x")
+        self.bad_value, self.minor_opcode, self.major_opcode = unpacker.unpack(
+            "xx2xIHB21x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHB21x", self.bad_value, self.minor_opcode, self.major_opcode))
+        buf.write(
+            struct.pack(
+                "=IHB21x",
+                self.bad_value,
+                self.minor_opcode,
+                self.major_opcode))
         return buf.getvalue()
 BadGLXBadProfileARB = GLXBadProfileARBError
 _errors[13] = GLXBadProfileARBError
+
+
 class PbufferClobberEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.event_type, self.draw_type, self.drawable, self.b_mask, self.aux_buffer, self.x, self.y, self.width, self.height, self.count = unpacker.unpack("xx2xHHIIHHHHHH4x")
+        self.event_type, self.draw_type, self.drawable, self.b_mask, self.aux_buffer, self.x, self.y, self.width, self.height, self.count = unpacker.unpack(
+            "xx2xHHIIHHHHHH4x")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xHHIIHHHHHH4x", self.event_type, self.draw_type, self.drawable, self.b_mask, self.aux_buffer, self.x, self.y, self.width, self.height, self.count))
+        buf.write(
+            struct.pack(
+                "=xHHIIHHHHHH4x",
+                self.event_type,
+                self.draw_type,
+                self.drawable,
+                self.b_mask,
+                self.aux_buffer,
+                self.x,
+                self.y,
+                self.width,
+                self.height,
+                self.count))
         return buf.getvalue()
 _events[0] = PbufferClobberEvent
+
+
 class BufferSwapCompleteEvent(xcffib.Event):
+
     def __init__(self, unpacker):
         xcffib.Event.__init__(self, unpacker)
         base = unpacker.offset
-        self.event_type, self.drawable, self.ust_hi, self.ust_lo, self.msc_hi, self.msc_lo, self.sbc = unpacker.unpack("xx2xH2xIIIIII")
+        self.event_type, self.drawable, self.ust_hi, self.ust_lo, self.msc_hi, self.msc_lo, self.sbc = unpacker.unpack(
+            "xx2xH2xIIIIII")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=xH2xIIIIII", self.event_type, self.drawable, self.ust_hi, self.ust_lo, self.msc_hi, self.msc_lo, self.sbc))
+        buf.write(
+            struct.pack(
+                "=xH2xIIIIII",
+                self.event_type,
+                self.drawable,
+                self.ust_hi,
+                self.ust_lo,
+                self.msc_hi,
+                self.msc_lo,
+                self.sbc))
         return buf.getvalue()
 _events[1] = BufferSwapCompleteEvent
+
+
 class PBCET:
     Damaged = 32791
     Saved = 32792
+
+
 class PBCDT:
     Window = 32793
     Pbuffer = 32794
+
+
 class MakeCurrentReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.context_tag, = unpacker.unpack("xx2x4xI20x")
         self.bufsize = unpacker.offset - base
+
+
 class MakeCurrentCookie(xcffib.Cookie):
     reply_type = MakeCurrentReply
+
+
 class IsDirectReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.is_direct, = unpacker.unpack("xx2x4xB23x")
         self.bufsize = unpacker.offset - base
+
+
 class IsDirectCookie(xcffib.Cookie):
     reply_type = IsDirectReply
+
+
 class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.major_version, self.minor_version = unpacker.unpack("xx2x4xII16x")
         self.bufsize = unpacker.offset - base
+
+
 class QueryVersionCookie(xcffib.Cookie):
     reply_type = QueryVersionReply
+
+
 class GC:
     GL_CURRENT_BIT = 1 << 0
     GL_POINT_BIT = 1 << 1
     GL_LINE_BIT = 1 << 2
     GL_POLYGON_BIT = 1 << 3
     GL_POLYGON_STIPPLE_BIT = 1 << 4
     GL_PIXEL_MODE_BIT = 1 << 5
@@ -257,993 +459,2024 @@
     GL_COLOR_BUFFER_BIT = 1 << 14
     GL_HINT_BIT = 1 << 15
     GL_EVAL_BIT = 1 << 16
     GL_LIST_BIT = 1 << 17
     GL_TEXTURE_BIT = 1 << 18
     GL_SCISSOR_BIT = 1 << 19
     GL_ALL_ATTRIB_BITS = 16777215
+
+
 class GetVisualConfigsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_visuals, self.num_properties = unpacker.unpack("xx2x4xII16x")
         self.property_list = xcffib.List(unpacker, "I", self.length)
         self.bufsize = unpacker.offset - base
+
+
 class GetVisualConfigsCookie(xcffib.Cookie):
     reply_type = GetVisualConfigsReply
+
+
 class VendorPrivateWithReplyReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.retval, = unpacker.unpack("xx2x4xI")
         self.data1 = xcffib.List(unpacker, "B", 24)
         unpacker.pad("B")
         self.data2 = xcffib.List(unpacker, "B", self.length * 4)
         self.bufsize = unpacker.offset - base
+
+
 class VendorPrivateWithReplyCookie(xcffib.Cookie):
     reply_type = VendorPrivateWithReplyReply
+
+
 class QueryExtensionsStringReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, = unpacker.unpack("xx2x4x4xI16x")
         self.bufsize = unpacker.offset - base
+
+
 class QueryExtensionsStringCookie(xcffib.Cookie):
     reply_type = QueryExtensionsStringReply
+
+
 class QueryServerStringReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.str_len, = unpacker.unpack("xx2x4x4xI16x")
         self.string = xcffib.List(unpacker, "c", self.str_len)
         self.bufsize = unpacker.offset - base
+
+
 class QueryServerStringCookie(xcffib.Cookie):
     reply_type = QueryServerStringReply
+
+
 class GetFBConfigsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.num_FB_configs, self.num_properties = unpacker.unpack("xx2x4xII16x")
+        self.num_FB_configs, self.num_properties = unpacker.unpack(
+            "xx2x4xII16x")
         self.property_list = xcffib.List(unpacker, "I", self.length)
         self.bufsize = unpacker.offset - base
+
+
 class GetFBConfigsCookie(xcffib.Cookie):
     reply_type = GetFBConfigsReply
+
+
 class QueryContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_attribs, = unpacker.unpack("xx2x4xI20x")
         self.attribs = xcffib.List(unpacker, "I", self.num_attribs * 2)
         self.bufsize = unpacker.offset - base
+
+
 class QueryContextCookie(xcffib.Cookie):
     reply_type = QueryContextReply
+
+
 class MakeContextCurrentReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.context_tag, = unpacker.unpack("xx2x4xI20x")
         self.bufsize = unpacker.offset - base
+
+
 class MakeContextCurrentCookie(xcffib.Cookie):
     reply_type = MakeContextCurrentReply
+
+
 class GetDrawableAttributesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.num_attribs, = unpacker.unpack("xx2x4xI20x")
         self.attribs = xcffib.List(unpacker, "I", self.num_attribs * 2)
         self.bufsize = unpacker.offset - base
+
+
 class GetDrawableAttributesCookie(xcffib.Cookie):
     reply_type = GetDrawableAttributesReply
+
+
 class GenListsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.ret_val, = unpacker.unpack("xx2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class GenListsCookie(xcffib.Cookie):
     reply_type = GenListsReply
+
+
 class RenderModeReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.ret_val, self.n, self.new_mode = unpacker.unpack("xx2x4xIII12x")
         self.data = xcffib.List(unpacker, "I", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class RenderModeCookie(xcffib.Cookie):
     reply_type = RenderModeReply
+
+
 class RM:
     GL_RENDER = 7168
     GL_FEEDBACK = 7169
     GL_SELECT = 7170
+
+
 class FinishReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x")
         self.bufsize = unpacker.offset - base
+
+
 class FinishCookie(xcffib.Cookie):
     reply_type = FinishReply
+
+
 class ReadPixelsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x24x")
         self.data = xcffib.List(unpacker, "B", self.length * 4)
         self.bufsize = unpacker.offset - base
+
+
 class ReadPixelsCookie(xcffib.Cookie):
     reply_type = ReadPixelsReply
+
+
 class GetBooleanvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIB15x")
         self.data = xcffib.List(unpacker, "B", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetBooleanvCookie(xcffib.Cookie):
     reply_type = GetBooleanvReply
+
+
 class GetClipPlaneReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x24x")
         self.data = xcffib.List(unpacker, "d", self.length // 2)
         self.bufsize = unpacker.offset - base
+
+
 class GetClipPlaneCookie(xcffib.Cookie):
     reply_type = GetClipPlaneReply
+
+
 class GetDoublevReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xId8x")
         self.data = xcffib.List(unpacker, "d", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetDoublevCookie(xcffib.Cookie):
     reply_type = GetDoublevReply
+
+
 class GetErrorReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.error, = unpacker.unpack("xx2x4xi")
         self.bufsize = unpacker.offset - base
+
+
 class GetErrorCookie(xcffib.Cookie):
     reply_type = GetErrorReply
+
+
 class GetFloatvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIf12x")
         self.data = xcffib.List(unpacker, "f", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetFloatvCookie(xcffib.Cookie):
     reply_type = GetFloatvReply
+
+
 class GetIntegervReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIi12x")
         self.data = xcffib.List(unpacker, "i", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetIntegervCookie(xcffib.Cookie):
     reply_type = GetIntegervReply
+
+
 class GetLightfvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIf12x")
         self.data = xcffib.List(unpacker, "f", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetLightfvCookie(xcffib.Cookie):
     reply_type = GetLightfvReply
+
+
 class GetLightivReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIi12x")
         self.data = xcffib.List(unpacker, "i", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetLightivCookie(xcffib.Cookie):
     reply_type = GetLightivReply
+
+
 class GetMapdvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xId8x")
         self.data = xcffib.List(unpacker, "d", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetMapdvCookie(xcffib.Cookie):
     reply_type = GetMapdvReply
+
+
 class GetMapfvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIf12x")
         self.data = xcffib.List(unpacker, "f", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetMapfvCookie(xcffib.Cookie):
     reply_type = GetMapfvReply
+
+
 class GetMapivReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIi12x")
         self.data = xcffib.List(unpacker, "i", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetMapivCookie(xcffib.Cookie):
     reply_type = GetMapivReply
+
+
 class GetMaterialfvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIf12x")
         self.data = xcffib.List(unpacker, "f", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetMaterialfvCookie(xcffib.Cookie):
     reply_type = GetMaterialfvReply
+
+
 class GetMaterialivReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIi12x")
         self.data = xcffib.List(unpacker, "i", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetMaterialivCookie(xcffib.Cookie):
     reply_type = GetMaterialivReply
+
+
 class GetPixelMapfvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIf12x")
         self.data = xcffib.List(unpacker, "f", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetPixelMapfvCookie(xcffib.Cookie):
     reply_type = GetPixelMapfvReply
+
+
 class GetPixelMapuivReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xII12x")
         self.data = xcffib.List(unpacker, "I", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetPixelMapuivCookie(xcffib.Cookie):
     reply_type = GetPixelMapuivReply
+
+
 class GetPixelMapusvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIH16x")
         self.data = xcffib.List(unpacker, "H", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetPixelMapusvCookie(xcffib.Cookie):
     reply_type = GetPixelMapusvReply
+
+
 class GetPolygonStippleReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x24x")
         self.data = xcffib.List(unpacker, "B", self.length * 4)
         self.bufsize = unpacker.offset - base
+
+
 class GetPolygonStippleCookie(xcffib.Cookie):
     reply_type = GetPolygonStippleReply
+
+
 class GetStringReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, = unpacker.unpack("xx2x4x4xI16x")
         self.string = xcffib.List(unpacker, "c", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetStringCookie(xcffib.Cookie):
     reply_type = GetStringReply
+
+
 class GetTexEnvfvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIf12x")
         self.data = xcffib.List(unpacker, "f", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetTexEnvfvCookie(xcffib.Cookie):
     reply_type = GetTexEnvfvReply
+
+
 class GetTexEnvivReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIi12x")
         self.data = xcffib.List(unpacker, "i", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetTexEnvivCookie(xcffib.Cookie):
     reply_type = GetTexEnvivReply
+
+
 class GetTexGendvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xId8x")
         self.data = xcffib.List(unpacker, "d", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetTexGendvCookie(xcffib.Cookie):
     reply_type = GetTexGendvReply
+
+
 class GetTexGenfvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIf12x")
         self.data = xcffib.List(unpacker, "f", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetTexGenfvCookie(xcffib.Cookie):
     reply_type = GetTexGenfvReply
+
+
 class GetTexGenivReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIi12x")
         self.data = xcffib.List(unpacker, "i", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetTexGenivCookie(xcffib.Cookie):
     reply_type = GetTexGenivReply
+
+
 class GetTexImageReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.width, self.height, self.depth = unpacker.unpack("xx2x4x8xiii4x")
         self.data = xcffib.List(unpacker, "B", self.length * 4)
         self.bufsize = unpacker.offset - base
+
+
 class GetTexImageCookie(xcffib.Cookie):
     reply_type = GetTexImageReply
+
+
 class GetTexParameterfvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIf12x")
         self.data = xcffib.List(unpacker, "f", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetTexParameterfvCookie(xcffib.Cookie):
     reply_type = GetTexParameterfvReply
+
+
 class GetTexParameterivReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIi12x")
         self.data = xcffib.List(unpacker, "i", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetTexParameterivCookie(xcffib.Cookie):
     reply_type = GetTexParameterivReply
+
+
 class GetTexLevelParameterfvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIf12x")
         self.data = xcffib.List(unpacker, "f", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetTexLevelParameterfvCookie(xcffib.Cookie):
     reply_type = GetTexLevelParameterfvReply
+
+
 class GetTexLevelParameterivReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIi12x")
         self.data = xcffib.List(unpacker, "i", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetTexLevelParameterivCookie(xcffib.Cookie):
     reply_type = GetTexLevelParameterivReply
+
+
 class IsListReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.ret_val, = unpacker.unpack("xx2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class IsListCookie(xcffib.Cookie):
     reply_type = IsListReply
+
+
 class AreTexturesResidentReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.ret_val, = unpacker.unpack("xx2x4xI20x")
         self.data = xcffib.List(unpacker, "B", self.length * 4)
         self.bufsize = unpacker.offset - base
+
+
 class AreTexturesResidentCookie(xcffib.Cookie):
     reply_type = AreTexturesResidentReply
+
+
 class GenTexturesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x24x")
         self.data = xcffib.List(unpacker, "I", self.length)
         self.bufsize = unpacker.offset - base
+
+
 class GenTexturesCookie(xcffib.Cookie):
     reply_type = GenTexturesReply
+
+
 class IsTextureReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.ret_val, = unpacker.unpack("xx2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class IsTextureCookie(xcffib.Cookie):
     reply_type = IsTextureReply
+
+
 class GetColorTableReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.width, = unpacker.unpack("xx2x4x8xi12x")
         self.data = xcffib.List(unpacker, "B", self.length * 4)
         self.bufsize = unpacker.offset - base
+
+
 class GetColorTableCookie(xcffib.Cookie):
     reply_type = GetColorTableReply
+
+
 class GetColorTableParameterfvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIf12x")
         self.data = xcffib.List(unpacker, "f", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetColorTableParameterfvCookie(xcffib.Cookie):
     reply_type = GetColorTableParameterfvReply
+
+
 class GetColorTableParameterivReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIi12x")
         self.data = xcffib.List(unpacker, "i", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetColorTableParameterivCookie(xcffib.Cookie):
     reply_type = GetColorTableParameterivReply
+
+
 class GetConvolutionFilterReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.width, self.height = unpacker.unpack("xx2x4x8xii8x")
         self.data = xcffib.List(unpacker, "B", self.length * 4)
         self.bufsize = unpacker.offset - base
+
+
 class GetConvolutionFilterCookie(xcffib.Cookie):
     reply_type = GetConvolutionFilterReply
+
+
 class GetConvolutionParameterfvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIf12x")
         self.data = xcffib.List(unpacker, "f", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetConvolutionParameterfvCookie(xcffib.Cookie):
     reply_type = GetConvolutionParameterfvReply
+
+
 class GetConvolutionParameterivReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIi12x")
         self.data = xcffib.List(unpacker, "i", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetConvolutionParameterivCookie(xcffib.Cookie):
     reply_type = GetConvolutionParameterivReply
+
+
 class GetSeparableFilterReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.row_w, self.col_h = unpacker.unpack("xx2x4x8xii8x")
         self.rows_and_cols = xcffib.List(unpacker, "B", self.length * 4)
         self.bufsize = unpacker.offset - base
+
+
 class GetSeparableFilterCookie(xcffib.Cookie):
     reply_type = GetSeparableFilterReply
+
+
 class GetHistogramReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.width, = unpacker.unpack("xx2x4x8xi12x")
         self.data = xcffib.List(unpacker, "B", self.length * 4)
         self.bufsize = unpacker.offset - base
+
+
 class GetHistogramCookie(xcffib.Cookie):
     reply_type = GetHistogramReply
+
+
 class GetHistogramParameterfvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIf12x")
         self.data = xcffib.List(unpacker, "f", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetHistogramParameterfvCookie(xcffib.Cookie):
     reply_type = GetHistogramParameterfvReply
+
+
 class GetHistogramParameterivReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIi12x")
         self.data = xcffib.List(unpacker, "i", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetHistogramParameterivCookie(xcffib.Cookie):
     reply_type = GetHistogramParameterivReply
+
+
 class GetMinmaxReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x24x")
         self.data = xcffib.List(unpacker, "B", self.length * 4)
         self.bufsize = unpacker.offset - base
+
+
 class GetMinmaxCookie(xcffib.Cookie):
     reply_type = GetMinmaxReply
+
+
 class GetMinmaxParameterfvReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIf12x")
         self.data = xcffib.List(unpacker, "f", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetMinmaxParameterfvCookie(xcffib.Cookie):
     reply_type = GetMinmaxParameterfvReply
+
+
 class GetMinmaxParameterivReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIi12x")
         self.data = xcffib.List(unpacker, "i", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetMinmaxParameterivCookie(xcffib.Cookie):
     reply_type = GetMinmaxParameterivReply
+
+
 class GetCompressedTexImageARBReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.size, = unpacker.unpack("xx2x4x8xi12x")
         self.data = xcffib.List(unpacker, "B", self.length * 4)
         self.bufsize = unpacker.offset - base
+
+
 class GetCompressedTexImageARBCookie(xcffib.Cookie):
     reply_type = GetCompressedTexImageARBReply
+
+
 class GenQueriesARBReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         unpacker.unpack("xx2x4x24x")
         self.data = xcffib.List(unpacker, "I", self.length)
         self.bufsize = unpacker.offset - base
+
+
 class GenQueriesARBCookie(xcffib.Cookie):
     reply_type = GenQueriesARBReply
+
+
 class IsQueryARBReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.ret_val, = unpacker.unpack("xx2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class IsQueryARBCookie(xcffib.Cookie):
     reply_type = IsQueryARBReply
+
+
 class GetQueryivARBReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIi12x")
         self.data = xcffib.List(unpacker, "i", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetQueryivARBCookie(xcffib.Cookie):
     reply_type = GetQueryivARBReply
+
+
 class GetQueryObjectivARBReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xIi12x")
         self.data = xcffib.List(unpacker, "i", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetQueryObjectivARBCookie(xcffib.Cookie):
     reply_type = GetQueryObjectivARBReply
+
+
 class GetQueryObjectuivARBReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.n, self.datum = unpacker.unpack("xx2x4x4xII12x")
         self.data = xcffib.List(unpacker, "I", self.n)
         self.bufsize = unpacker.offset - base
+
+
 class GetQueryObjectuivARBCookie(xcffib.Cookie):
     reply_type = GetQueryObjectuivARBReply
+
+
 class glxExtension(xcffib.Extension):
+
     def Render(self, context_tag, data, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context_tag))
         buf.write(xcffib.pack_list(data, "B"))
         return self.send_request(1, buf, is_checked=is_checked)
-    def RenderLarge(self, context_tag, request_num, request_total, data_len, data, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIHHI", context_tag, request_num, request_total, data_len))
+
+    def RenderLarge(
+            self,
+            context_tag,
+            request_num,
+            request_total,
+            data_len,
+            data,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIHHI",
+                context_tag,
+                request_num,
+                request_total,
+                data_len))
         buf.write(xcffib.pack_list(data, "B"))
         return self.send_request(2, buf, is_checked=is_checked)
-    def CreateContext(self, context, visual, screen, share_list, is_direct, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIIB3x", context, visual, screen, share_list, is_direct))
+
+    def CreateContext(
+            self,
+            context,
+            visual,
+            screen,
+            share_list,
+            is_direct,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIIB3x",
+                context,
+                visual,
+                screen,
+                share_list,
+                is_direct))
         return self.send_request(3, buf, is_checked=is_checked)
+
     def DestroyContext(self, context, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context))
         return self.send_request(4, buf, is_checked=is_checked)
+
     def MakeCurrent(self, drawable, context, old_context_tag, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", drawable, context, old_context_tag))
-        return self.send_request(5, buf, MakeCurrentCookie, is_checked=is_checked)
+        return self.send_request(
+            5,
+            buf,
+            MakeCurrentCookie,
+            is_checked=is_checked)
+
     def IsDirect(self, context, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context))
         return self.send_request(6, buf, IsDirectCookie, is_checked=is_checked)
+
     def QueryVersion(self, major_version, minor_version, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", major_version, minor_version))
-        return self.send_request(7, buf, QueryVersionCookie, is_checked=is_checked)
+        return self.send_request(
+            7,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
     def WaitGL(self, context_tag, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context_tag))
         return self.send_request(8, buf, is_checked=is_checked)
+
     def WaitX(self, context_tag, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context_tag))
         return self.send_request(9, buf, is_checked=is_checked)
+
     def CopyContext(self, src, dest, mask, src_context_tag, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIII", src, dest, mask, src_context_tag))
         return self.send_request(10, buf, is_checked=is_checked)
+
     def SwapBuffers(self, context_tag, drawable, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", context_tag, drawable))
         return self.send_request(11, buf, is_checked=is_checked)
-    def UseXFont(self, context_tag, font, first, count, list_base, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIII", context_tag, font, first, count, list_base))
+
+    def UseXFont(
+            self,
+            context_tag,
+            font,
+            first,
+            count,
+            list_base,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIII",
+                context_tag,
+                font,
+                first,
+                count,
+                list_base))
         return self.send_request(12, buf, is_checked=is_checked)
-    def CreateGLXPixmap(self, screen, visual, pixmap, glx_pixmap, is_checked=False):
+
+    def CreateGLXPixmap(
+            self,
+            screen,
+            visual,
+            pixmap,
+            glx_pixmap,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIII", screen, visual, pixmap, glx_pixmap))
         return self.send_request(13, buf, is_checked=is_checked)
+
     def GetVisualConfigs(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", screen))
-        return self.send_request(14, buf, GetVisualConfigsCookie, is_checked=is_checked)
+        return self.send_request(
+            14,
+            buf,
+            GetVisualConfigsCookie,
+            is_checked=is_checked)
+
     def DestroyGLXPixmap(self, glx_pixmap, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", glx_pixmap))
         return self.send_request(15, buf, is_checked=is_checked)
+
     def VendorPrivate(self, vendor_code, context_tag, data, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", vendor_code, context_tag))
         buf.write(xcffib.pack_list(data, "B"))
         return self.send_request(16, buf, is_checked=is_checked)
-    def VendorPrivateWithReply(self, vendor_code, context_tag, data, is_checked=True):
+
+    def VendorPrivateWithReply(
+            self,
+            vendor_code,
+            context_tag,
+            data,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", vendor_code, context_tag))
         buf.write(xcffib.pack_list(data, "B"))
-        return self.send_request(17, buf, VendorPrivateWithReplyCookie, is_checked=is_checked)
+        return self.send_request(
+            17,
+            buf,
+            VendorPrivateWithReplyCookie,
+            is_checked=is_checked)
+
     def QueryExtensionsString(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", screen))
-        return self.send_request(18, buf, QueryExtensionsStringCookie, is_checked=is_checked)
+        return self.send_request(
+            18,
+            buf,
+            QueryExtensionsStringCookie,
+            is_checked=is_checked)
+
     def QueryServerString(self, screen, name, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", screen, name))
-        return self.send_request(19, buf, QueryServerStringCookie, is_checked=is_checked)
-    def ClientInfo(self, major_version, minor_version, str_len, string, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIII", major_version, minor_version, str_len))
+        return self.send_request(
+            19,
+            buf,
+            QueryServerStringCookie,
+            is_checked=is_checked)
+
+    def ClientInfo(
+            self,
+            major_version,
+            minor_version,
+            str_len,
+            string,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIII",
+                major_version,
+                minor_version,
+                str_len))
         buf.write(xcffib.pack_list(string, "c"))
         return self.send_request(20, buf, is_checked=is_checked)
+
     def GetFBConfigs(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", screen))
-        return self.send_request(21, buf, GetFBConfigsCookie, is_checked=is_checked)
-    def CreatePixmap(self, screen, fbconfig, pixmap, glx_pixmap, num_attribs, attribs, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIII", screen, fbconfig, pixmap, glx_pixmap, num_attribs))
+        return self.send_request(
+            21,
+            buf,
+            GetFBConfigsCookie,
+            is_checked=is_checked)
+
+    def CreatePixmap(
+            self,
+            screen,
+            fbconfig,
+            pixmap,
+            glx_pixmap,
+            num_attribs,
+            attribs,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIII",
+                screen,
+                fbconfig,
+                pixmap,
+                glx_pixmap,
+                num_attribs))
         buf.write(xcffib.pack_list(attribs, "I"))
         return self.send_request(22, buf, is_checked=is_checked)
+
     def DestroyPixmap(self, glx_pixmap, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", glx_pixmap))
         return self.send_request(23, buf, is_checked=is_checked)
-    def CreateNewContext(self, context, fbconfig, screen, render_type, share_list, is_direct, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIIIB3x", context, fbconfig, screen, render_type, share_list, is_direct))
+
+    def CreateNewContext(
+            self,
+            context,
+            fbconfig,
+            screen,
+            render_type,
+            share_list,
+            is_direct,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIIIB3x",
+                context,
+                fbconfig,
+                screen,
+                render_type,
+                share_list,
+                is_direct))
         return self.send_request(24, buf, is_checked=is_checked)
+
     def QueryContext(self, context, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context))
-        return self.send_request(25, buf, QueryContextCookie, is_checked=is_checked)
-    def MakeContextCurrent(self, old_context_tag, drawable, read_drawable, context, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIII", old_context_tag, drawable, read_drawable, context))
-        return self.send_request(26, buf, MakeContextCurrentCookie, is_checked=is_checked)
-    def CreatePbuffer(self, screen, fbconfig, pbuffer, num_attribs, attribs, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIII", screen, fbconfig, pbuffer, num_attribs))
+        return self.send_request(
+            25,
+            buf,
+            QueryContextCookie,
+            is_checked=is_checked)
+
+    def MakeContextCurrent(
+            self,
+            old_context_tag,
+            drawable,
+            read_drawable,
+            context,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIII",
+                old_context_tag,
+                drawable,
+                read_drawable,
+                context))
+        return self.send_request(
+            26,
+            buf,
+            MakeContextCurrentCookie,
+            is_checked=is_checked)
+
+    def CreatePbuffer(
+            self,
+            screen,
+            fbconfig,
+            pbuffer,
+            num_attribs,
+            attribs,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIII",
+                screen,
+                fbconfig,
+                pbuffer,
+                num_attribs))
         buf.write(xcffib.pack_list(attribs, "I"))
         return self.send_request(27, buf, is_checked=is_checked)
+
     def DestroyPbuffer(self, pbuffer, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", pbuffer))
         return self.send_request(28, buf, is_checked=is_checked)
+
     def GetDrawableAttributes(self, drawable, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", drawable))
-        return self.send_request(29, buf, GetDrawableAttributesCookie, is_checked=is_checked)
-    def ChangeDrawableAttributes(self, drawable, num_attribs, attribs, is_checked=False):
+        return self.send_request(
+            29,
+            buf,
+            GetDrawableAttributesCookie,
+            is_checked=is_checked)
+
+    def ChangeDrawableAttributes(
+            self,
+            drawable,
+            num_attribs,
+            attribs,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", drawable, num_attribs))
         buf.write(xcffib.pack_list(attribs, "I"))
         return self.send_request(30, buf, is_checked=is_checked)
-    def CreateWindow(self, screen, fbconfig, window, glx_window, num_attribs, attribs, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIII", screen, fbconfig, window, glx_window, num_attribs))
+
+    def CreateWindow(
+            self,
+            screen,
+            fbconfig,
+            window,
+            glx_window,
+            num_attribs,
+            attribs,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIII",
+                screen,
+                fbconfig,
+                window,
+                glx_window,
+                num_attribs))
         buf.write(xcffib.pack_list(attribs, "I"))
         return self.send_request(31, buf, is_checked=is_checked)
+
     def DeleteWindow(self, glxwindow, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", glxwindow))
         return self.send_request(32, buf, is_checked=is_checked)
-    def SetClientInfoARB(self, major_version, minor_version, num_versions, gl_str_len, glx_str_len, gl_versions, gl_extension_string, glx_extension_string, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIII", major_version, minor_version, num_versions, gl_str_len, glx_str_len))
+
+    def SetClientInfoARB(
+            self,
+            major_version,
+            minor_version,
+            num_versions,
+            gl_str_len,
+            glx_str_len,
+            gl_versions,
+            gl_extension_string,
+            glx_extension_string,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIII",
+                major_version,
+                minor_version,
+                num_versions,
+                gl_str_len,
+                glx_str_len))
         buf.write(xcffib.pack_list(gl_versions, "I"))
         buf.write(xcffib.pack_list(gl_extension_string, "c"))
         buf.write(xcffib.pack_list(glx_extension_string, "c"))
         return self.send_request(33, buf, is_checked=is_checked)
-    def CreateContextAttribsARB(self, context, fbconfig, screen, share_list, is_direct, num_attribs, attribs, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIIB3xI", context, fbconfig, screen, share_list, is_direct, num_attribs))
+
+    def CreateContextAttribsARB(
+            self,
+            context,
+            fbconfig,
+            screen,
+            share_list,
+            is_direct,
+            num_attribs,
+            attribs,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIIB3xI",
+                context,
+                fbconfig,
+                screen,
+                share_list,
+                is_direct,
+                num_attribs))
         buf.write(xcffib.pack_list(attribs, "I"))
         return self.send_request(34, buf, is_checked=is_checked)
-    def SetClientInfo2ARB(self, major_version, minor_version, num_versions, gl_str_len, glx_str_len, gl_versions, gl_extension_string, glx_extension_string, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIII", major_version, minor_version, num_versions, gl_str_len, glx_str_len))
+
+    def SetClientInfo2ARB(
+            self,
+            major_version,
+            minor_version,
+            num_versions,
+            gl_str_len,
+            glx_str_len,
+            gl_versions,
+            gl_extension_string,
+            glx_extension_string,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIII",
+                major_version,
+                minor_version,
+                num_versions,
+                gl_str_len,
+                glx_str_len))
         buf.write(xcffib.pack_list(gl_versions, "I"))
         buf.write(xcffib.pack_list(gl_extension_string, "c"))
         buf.write(xcffib.pack_list(glx_extension_string, "c"))
         return self.send_request(35, buf, is_checked=is_checked)
+
     def NewList(self, context_tag, list, mode, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, list, mode))
         return self.send_request(101, buf, is_checked=is_checked)
+
     def EndList(self, context_tag, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context_tag))
         return self.send_request(102, buf, is_checked=is_checked)
+
     def DeleteLists(self, context_tag, list, range, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIi", context_tag, list, range))
         return self.send_request(103, buf, is_checked=is_checked)
+
     def GenLists(self, context_tag, range, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIi", context_tag, range))
-        return self.send_request(104, buf, GenListsCookie, is_checked=is_checked)
+        return self.send_request(
+            104,
+            buf,
+            GenListsCookie,
+            is_checked=is_checked)
+
     def FeedbackBuffer(self, context_tag, size, type, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIii", context_tag, size, type))
         return self.send_request(105, buf, is_checked=is_checked)
+
     def SelectBuffer(self, context_tag, size, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIi", context_tag, size))
         return self.send_request(106, buf, is_checked=is_checked)
+
     def RenderMode(self, context_tag, mode, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", context_tag, mode))
-        return self.send_request(107, buf, RenderModeCookie, is_checked=is_checked)
+        return self.send_request(
+            107,
+            buf,
+            RenderModeCookie,
+            is_checked=is_checked)
+
     def Finish(self, context_tag, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context_tag))
         return self.send_request(108, buf, FinishCookie, is_checked=is_checked)
+
     def PixelStoref(self, context_tag, pname, datum, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIf", context_tag, pname, datum))
         return self.send_request(109, buf, is_checked=is_checked)
+
     def PixelStorei(self, context_tag, pname, datum, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIi", context_tag, pname, datum))
         return self.send_request(110, buf, is_checked=is_checked)
-    def ReadPixels(self, context_tag, x, y, width, height, format, type, swap_bytes, lsb_first, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIiiiiIIBB", context_tag, x, y, width, height, format, type, swap_bytes, lsb_first))
-        return self.send_request(111, buf, ReadPixelsCookie, is_checked=is_checked)
+
+    def ReadPixels(
+            self,
+            context_tag,
+            x,
+            y,
+            width,
+            height,
+            format,
+            type,
+            swap_bytes,
+            lsb_first,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIiiiiIIBB",
+                context_tag,
+                x,
+                y,
+                width,
+                height,
+                format,
+                type,
+                swap_bytes,
+                lsb_first))
+        return self.send_request(
+            111,
+            buf,
+            ReadPixelsCookie,
+            is_checked=is_checked)
+
     def GetBooleanv(self, context_tag, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIi", context_tag, pname))
-        return self.send_request(112, buf, GetBooleanvCookie, is_checked=is_checked)
+        return self.send_request(
+            112,
+            buf,
+            GetBooleanvCookie,
+            is_checked=is_checked)
+
     def GetClipPlane(self, context_tag, plane, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIi", context_tag, plane))
-        return self.send_request(113, buf, GetClipPlaneCookie, is_checked=is_checked)
+        return self.send_request(
+            113,
+            buf,
+            GetClipPlaneCookie,
+            is_checked=is_checked)
+
     def GetDoublev(self, context_tag, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", context_tag, pname))
-        return self.send_request(114, buf, GetDoublevCookie, is_checked=is_checked)
+        return self.send_request(
+            114,
+            buf,
+            GetDoublevCookie,
+            is_checked=is_checked)
+
     def GetError(self, context_tag, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context_tag))
-        return self.send_request(115, buf, GetErrorCookie, is_checked=is_checked)
+        return self.send_request(
+            115,
+            buf,
+            GetErrorCookie,
+            is_checked=is_checked)
+
     def GetFloatv(self, context_tag, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", context_tag, pname))
-        return self.send_request(116, buf, GetFloatvCookie, is_checked=is_checked)
+        return self.send_request(
+            116,
+            buf,
+            GetFloatvCookie,
+            is_checked=is_checked)
+
     def GetIntegerv(self, context_tag, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", context_tag, pname))
-        return self.send_request(117, buf, GetIntegervCookie, is_checked=is_checked)
+        return self.send_request(
+            117,
+            buf,
+            GetIntegervCookie,
+            is_checked=is_checked)
+
     def GetLightfv(self, context_tag, light, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, light, pname))
-        return self.send_request(118, buf, GetLightfvCookie, is_checked=is_checked)
+        return self.send_request(
+            118,
+            buf,
+            GetLightfvCookie,
+            is_checked=is_checked)
+
     def GetLightiv(self, context_tag, light, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, light, pname))
-        return self.send_request(119, buf, GetLightivCookie, is_checked=is_checked)
+        return self.send_request(
+            119,
+            buf,
+            GetLightivCookie,
+            is_checked=is_checked)
+
     def GetMapdv(self, context_tag, target, query, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, query))
-        return self.send_request(120, buf, GetMapdvCookie, is_checked=is_checked)
+        return self.send_request(
+            120,
+            buf,
+            GetMapdvCookie,
+            is_checked=is_checked)
+
     def GetMapfv(self, context_tag, target, query, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, query))
-        return self.send_request(121, buf, GetMapfvCookie, is_checked=is_checked)
+        return self.send_request(
+            121,
+            buf,
+            GetMapfvCookie,
+            is_checked=is_checked)
+
     def GetMapiv(self, context_tag, target, query, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, query))
-        return self.send_request(122, buf, GetMapivCookie, is_checked=is_checked)
+        return self.send_request(
+            122,
+            buf,
+            GetMapivCookie,
+            is_checked=is_checked)
+
     def GetMaterialfv(self, context_tag, face, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, face, pname))
-        return self.send_request(123, buf, GetMaterialfvCookie, is_checked=is_checked)
+        return self.send_request(
+            123,
+            buf,
+            GetMaterialfvCookie,
+            is_checked=is_checked)
+
     def GetMaterialiv(self, context_tag, face, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, face, pname))
-        return self.send_request(124, buf, GetMaterialivCookie, is_checked=is_checked)
+        return self.send_request(
+            124,
+            buf,
+            GetMaterialivCookie,
+            is_checked=is_checked)
+
     def GetPixelMapfv(self, context_tag, map, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", context_tag, map))
-        return self.send_request(125, buf, GetPixelMapfvCookie, is_checked=is_checked)
+        return self.send_request(
+            125,
+            buf,
+            GetPixelMapfvCookie,
+            is_checked=is_checked)
+
     def GetPixelMapuiv(self, context_tag, map, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", context_tag, map))
-        return self.send_request(126, buf, GetPixelMapuivCookie, is_checked=is_checked)
+        return self.send_request(
+            126,
+            buf,
+            GetPixelMapuivCookie,
+            is_checked=is_checked)
+
     def GetPixelMapusv(self, context_tag, map, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", context_tag, map))
-        return self.send_request(127, buf, GetPixelMapusvCookie, is_checked=is_checked)
+        return self.send_request(
+            127,
+            buf,
+            GetPixelMapusvCookie,
+            is_checked=is_checked)
+
     def GetPolygonStipple(self, context_tag, lsb_first, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIB", context_tag, lsb_first))
-        return self.send_request(128, buf, GetPolygonStippleCookie, is_checked=is_checked)
+        return self.send_request(
+            128,
+            buf,
+            GetPolygonStippleCookie,
+            is_checked=is_checked)
+
     def GetString(self, context_tag, name, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", context_tag, name))
-        return self.send_request(129, buf, GetStringCookie, is_checked=is_checked)
+        return self.send_request(
+            129,
+            buf,
+            GetStringCookie,
+            is_checked=is_checked)
+
     def GetTexEnvfv(self, context_tag, target, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, pname))
-        return self.send_request(130, buf, GetTexEnvfvCookie, is_checked=is_checked)
+        return self.send_request(
+            130,
+            buf,
+            GetTexEnvfvCookie,
+            is_checked=is_checked)
+
     def GetTexEnviv(self, context_tag, target, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, pname))
-        return self.send_request(131, buf, GetTexEnvivCookie, is_checked=is_checked)
+        return self.send_request(
+            131,
+            buf,
+            GetTexEnvivCookie,
+            is_checked=is_checked)
+
     def GetTexGendv(self, context_tag, coord, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, coord, pname))
-        return self.send_request(132, buf, GetTexGendvCookie, is_checked=is_checked)
+        return self.send_request(
+            132,
+            buf,
+            GetTexGendvCookie,
+            is_checked=is_checked)
+
     def GetTexGenfv(self, context_tag, coord, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, coord, pname))
-        return self.send_request(133, buf, GetTexGenfvCookie, is_checked=is_checked)
+        return self.send_request(
+            133,
+            buf,
+            GetTexGenfvCookie,
+            is_checked=is_checked)
+
     def GetTexGeniv(self, context_tag, coord, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, coord, pname))
-        return self.send_request(134, buf, GetTexGenivCookie, is_checked=is_checked)
-    def GetTexImage(self, context_tag, target, level, format, type, swap_bytes, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIiIIB", context_tag, target, level, format, type, swap_bytes))
-        return self.send_request(135, buf, GetTexImageCookie, is_checked=is_checked)
+        return self.send_request(
+            134,
+            buf,
+            GetTexGenivCookie,
+            is_checked=is_checked)
+
+    def GetTexImage(
+            self,
+            context_tag,
+            target,
+            level,
+            format,
+            type,
+            swap_bytes,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIiIIB",
+                context_tag,
+                target,
+                level,
+                format,
+                type,
+                swap_bytes))
+        return self.send_request(
+            135,
+            buf,
+            GetTexImageCookie,
+            is_checked=is_checked)
+
     def GetTexParameterfv(self, context_tag, target, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, pname))
-        return self.send_request(136, buf, GetTexParameterfvCookie, is_checked=is_checked)
+        return self.send_request(
+            136,
+            buf,
+            GetTexParameterfvCookie,
+            is_checked=is_checked)
+
     def GetTexParameteriv(self, context_tag, target, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, pname))
-        return self.send_request(137, buf, GetTexParameterivCookie, is_checked=is_checked)
-    def GetTexLevelParameterfv(self, context_tag, target, level, pname, is_checked=True):
+        return self.send_request(
+            137,
+            buf,
+            GetTexParameterivCookie,
+            is_checked=is_checked)
+
+    def GetTexLevelParameterfv(
+            self,
+            context_tag,
+            target,
+            level,
+            pname,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIiI", context_tag, target, level, pname))
-        return self.send_request(138, buf, GetTexLevelParameterfvCookie, is_checked=is_checked)
-    def GetTexLevelParameteriv(self, context_tag, target, level, pname, is_checked=True):
+        return self.send_request(
+            138,
+            buf,
+            GetTexLevelParameterfvCookie,
+            is_checked=is_checked)
+
+    def GetTexLevelParameteriv(
+            self,
+            context_tag,
+            target,
+            level,
+            pname,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIiI", context_tag, target, level, pname))
-        return self.send_request(139, buf, GetTexLevelParameterivCookie, is_checked=is_checked)
+        return self.send_request(
+            139,
+            buf,
+            GetTexLevelParameterivCookie,
+            is_checked=is_checked)
+
     def IsList(self, context_tag, list, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", context_tag, list))
         return self.send_request(141, buf, IsListCookie, is_checked=is_checked)
+
     def Flush(self, context_tag, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context_tag))
         return self.send_request(142, buf, is_checked=is_checked)
+
     def AreTexturesResident(self, context_tag, n, textures, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIi", context_tag, n))
         buf.write(xcffib.pack_list(textures, "I"))
-        return self.send_request(143, buf, AreTexturesResidentCookie, is_checked=is_checked)
+        return self.send_request(
+            143,
+            buf,
+            AreTexturesResidentCookie,
+            is_checked=is_checked)
+
     def DeleteTextures(self, context_tag, n, textures, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIi", context_tag, n))
         buf.write(xcffib.pack_list(textures, "I"))
         return self.send_request(144, buf, is_checked=is_checked)
+
     def GenTextures(self, context_tag, n, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIi", context_tag, n))
-        return self.send_request(145, buf, GenTexturesCookie, is_checked=is_checked)
+        return self.send_request(
+            145,
+            buf,
+            GenTexturesCookie,
+            is_checked=is_checked)
+
     def IsTexture(self, context_tag, texture, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", context_tag, texture))
-        return self.send_request(146, buf, IsTextureCookie, is_checked=is_checked)
-    def GetColorTable(self, context_tag, target, format, type, swap_bytes, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIIB", context_tag, target, format, type, swap_bytes))
-        return self.send_request(147, buf, GetColorTableCookie, is_checked=is_checked)
-    def GetColorTableParameterfv(self, context_tag, target, pname, is_checked=True):
+        return self.send_request(
+            146,
+            buf,
+            IsTextureCookie,
+            is_checked=is_checked)
+
+    def GetColorTable(
+            self,
+            context_tag,
+            target,
+            format,
+            type,
+            swap_bytes,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIIB",
+                context_tag,
+                target,
+                format,
+                type,
+                swap_bytes))
+        return self.send_request(
+            147,
+            buf,
+            GetColorTableCookie,
+            is_checked=is_checked)
+
+    def GetColorTableParameterfv(
+            self,
+            context_tag,
+            target,
+            pname,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, pname))
-        return self.send_request(148, buf, GetColorTableParameterfvCookie, is_checked=is_checked)
-    def GetColorTableParameteriv(self, context_tag, target, pname, is_checked=True):
+        return self.send_request(
+            148,
+            buf,
+            GetColorTableParameterfvCookie,
+            is_checked=is_checked)
+
+    def GetColorTableParameteriv(
+            self,
+            context_tag,
+            target,
+            pname,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, pname))
-        return self.send_request(149, buf, GetColorTableParameterivCookie, is_checked=is_checked)
-    def GetConvolutionFilter(self, context_tag, target, format, type, swap_bytes, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIIB", context_tag, target, format, type, swap_bytes))
-        return self.send_request(150, buf, GetConvolutionFilterCookie, is_checked=is_checked)
-    def GetConvolutionParameterfv(self, context_tag, target, pname, is_checked=True):
+        return self.send_request(
+            149,
+            buf,
+            GetColorTableParameterivCookie,
+            is_checked=is_checked)
+
+    def GetConvolutionFilter(
+            self,
+            context_tag,
+            target,
+            format,
+            type,
+            swap_bytes,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIIB",
+                context_tag,
+                target,
+                format,
+                type,
+                swap_bytes))
+        return self.send_request(
+            150,
+            buf,
+            GetConvolutionFilterCookie,
+            is_checked=is_checked)
+
+    def GetConvolutionParameterfv(
+            self,
+            context_tag,
+            target,
+            pname,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, pname))
-        return self.send_request(151, buf, GetConvolutionParameterfvCookie, is_checked=is_checked)
-    def GetConvolutionParameteriv(self, context_tag, target, pname, is_checked=True):
+        return self.send_request(
+            151,
+            buf,
+            GetConvolutionParameterfvCookie,
+            is_checked=is_checked)
+
+    def GetConvolutionParameteriv(
+            self,
+            context_tag,
+            target,
+            pname,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, pname))
-        return self.send_request(152, buf, GetConvolutionParameterivCookie, is_checked=is_checked)
-    def GetSeparableFilter(self, context_tag, target, format, type, swap_bytes, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIIB", context_tag, target, format, type, swap_bytes))
-        return self.send_request(153, buf, GetSeparableFilterCookie, is_checked=is_checked)
-    def GetHistogram(self, context_tag, target, format, type, swap_bytes, reset, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIIBB", context_tag, target, format, type, swap_bytes, reset))
-        return self.send_request(154, buf, GetHistogramCookie, is_checked=is_checked)
-    def GetHistogramParameterfv(self, context_tag, target, pname, is_checked=True):
+        return self.send_request(
+            152,
+            buf,
+            GetConvolutionParameterivCookie,
+            is_checked=is_checked)
+
+    def GetSeparableFilter(
+            self,
+            context_tag,
+            target,
+            format,
+            type,
+            swap_bytes,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIIB",
+                context_tag,
+                target,
+                format,
+                type,
+                swap_bytes))
+        return self.send_request(
+            153,
+            buf,
+            GetSeparableFilterCookie,
+            is_checked=is_checked)
+
+    def GetHistogram(
+            self,
+            context_tag,
+            target,
+            format,
+            type,
+            swap_bytes,
+            reset,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIIBB",
+                context_tag,
+                target,
+                format,
+                type,
+                swap_bytes,
+                reset))
+        return self.send_request(
+            154,
+            buf,
+            GetHistogramCookie,
+            is_checked=is_checked)
+
+    def GetHistogramParameterfv(
+            self,
+            context_tag,
+            target,
+            pname,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, pname))
-        return self.send_request(155, buf, GetHistogramParameterfvCookie, is_checked=is_checked)
-    def GetHistogramParameteriv(self, context_tag, target, pname, is_checked=True):
+        return self.send_request(
+            155,
+            buf,
+            GetHistogramParameterfvCookie,
+            is_checked=is_checked)
+
+    def GetHistogramParameteriv(
+            self,
+            context_tag,
+            target,
+            pname,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, pname))
-        return self.send_request(156, buf, GetHistogramParameterivCookie, is_checked=is_checked)
-    def GetMinmax(self, context_tag, target, format, type, swap_bytes, reset, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIIIBB", context_tag, target, format, type, swap_bytes, reset))
-        return self.send_request(157, buf, GetMinmaxCookie, is_checked=is_checked)
-    def GetMinmaxParameterfv(self, context_tag, target, pname, is_checked=True):
+        return self.send_request(
+            156,
+            buf,
+            GetHistogramParameterivCookie,
+            is_checked=is_checked)
+
+    def GetMinmax(
+            self,
+            context_tag,
+            target,
+            format,
+            type,
+            swap_bytes,
+            reset,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIIIBB",
+                context_tag,
+                target,
+                format,
+                type,
+                swap_bytes,
+                reset))
+        return self.send_request(
+            157,
+            buf,
+            GetMinmaxCookie,
+            is_checked=is_checked)
+
+    def GetMinmaxParameterfv(
+            self,
+            context_tag,
+            target,
+            pname,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, pname))
-        return self.send_request(158, buf, GetMinmaxParameterfvCookie, is_checked=is_checked)
-    def GetMinmaxParameteriv(self, context_tag, target, pname, is_checked=True):
+        return self.send_request(
+            158,
+            buf,
+            GetMinmaxParameterfvCookie,
+            is_checked=is_checked)
+
+    def GetMinmaxParameteriv(
+            self,
+            context_tag,
+            target,
+            pname,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, pname))
-        return self.send_request(159, buf, GetMinmaxParameterivCookie, is_checked=is_checked)
-    def GetCompressedTexImageARB(self, context_tag, target, level, is_checked=True):
+        return self.send_request(
+            159,
+            buf,
+            GetMinmaxParameterivCookie,
+            is_checked=is_checked)
+
+    def GetCompressedTexImageARB(
+            self,
+            context_tag,
+            target,
+            level,
+            is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIIi", context_tag, target, level))
-        return self.send_request(160, buf, GetCompressedTexImageARBCookie, is_checked=is_checked)
+        return self.send_request(
+            160,
+            buf,
+            GetCompressedTexImageARBCookie,
+            is_checked=is_checked)
+
     def DeleteQueriesARB(self, context_tag, n, ids, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIi", context_tag, n))
         buf.write(xcffib.pack_list(ids, "I"))
         return self.send_request(161, buf, is_checked=is_checked)
+
     def GenQueriesARB(self, context_tag, n, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIi", context_tag, n))
-        return self.send_request(162, buf, GenQueriesARBCookie, is_checked=is_checked)
+        return self.send_request(
+            162,
+            buf,
+            GenQueriesARBCookie,
+            is_checked=is_checked)
+
     def IsQueryARB(self, context_tag, id, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", context_tag, id))
-        return self.send_request(163, buf, IsQueryARBCookie, is_checked=is_checked)
+        return self.send_request(
+            163,
+            buf,
+            IsQueryARBCookie,
+            is_checked=is_checked)
+
     def GetQueryivARB(self, context_tag, target, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, target, pname))
-        return self.send_request(164, buf, GetQueryivARBCookie, is_checked=is_checked)
+        return self.send_request(
+            164,
+            buf,
+            GetQueryivARBCookie,
+            is_checked=is_checked)
+
     def GetQueryObjectivARB(self, context_tag, id, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, id, pname))
-        return self.send_request(165, buf, GetQueryObjectivARBCookie, is_checked=is_checked)
+        return self.send_request(
+            165,
+            buf,
+            GetQueryObjectivARBCookie,
+            is_checked=is_checked)
+
     def GetQueryObjectuivARB(self, context_tag, id, pname, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xIII", context_tag, id, pname))
-        return self.send_request(166, buf, GetQueryObjectuivARBCookie, is_checked=is_checked)
+        return self.send_request(
+            166,
+            buf,
+            GetQueryObjectuivARBCookie,
+            is_checked=is_checked)
 xcffib._add_ext(key, glxExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/__pycache__/_cffi__xe30fa035xc8917695.c` & `xcffib-v0.1.4/xcffib/__pycache__/_cffi__xe30fa035xc8917695.c`

 * *Files identical despite different names*

### Comparing `xcffib-v0.1.3/xcffib/testing.py` & `xcffib-v0.1.4/xcffib/testing.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 import os
 import time
 import errno
 import subprocess
 
 from . import Connection, ConnectionException
 
+
 def lock_path(display):
     return '/tmp/.X%d-lock' % display
 
+
 class XvfbTest(object):
+
     """ A helper class for testing things with nosetests. This class will run
     each test in its own fresh xvfb, leaving you with an xcffib connection to
     that X session as `self.conn` for use in testing. """
 
     def spawn(self, cmd):
         """ Spawn a command but swallow its output. """
         discard = open(os.devnull)
```

### Comparing `xcffib-v0.1.3/xcffib/xf86vidmode.py` & `xcffib-v0.1.4/xcffib/xf86vidmode.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,236 +2,568 @@
 import struct
 import six
 MAJOR_VERSION = 2
 MINOR_VERSION = 2
 key = xcffib.ExtensionKey("XFree86-VidModeExtension")
 _events = {}
 _errors = {}
+
+
 class ModeFlag:
     Positive_HSync = 1 << 0
     Negative_HSync = 1 << 1
     Positive_VSync = 1 << 2
     Negative_VSync = 1 << 3
     Interlace = 1 << 4
     Composite_Sync = 1 << 5
     Positive_CSync = 1 << 6
     Negative_CSync = 1 << 7
     HSkew = 1 << 8
     Broadcast = 1 << 9
     Pixmux = 1 << 10
     Double_Clock = 1 << 11
     Half_Clock = 1 << 12
+
+
 class ClockFlag:
     Programable = 1 << 0
+
+
 class Permission:
     Read = 1 << 0
     Write = 1 << 1
+
+
 class ModeInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.dotclock, self.hdisplay, self.hsyncstart, self.hsyncend, self.htotal, self.hskew, self.vdisplay, self.vsyncstart, self.vsyncend, self.vtotal, self.flags, self.privsize = unpacker.unpack("IHHHHIHHHH4xI12xI")
+        self.dotclock, self.hdisplay, self.hsyncstart, self.hsyncend, self.htotal, self.hskew, self.vdisplay, self.vsyncstart, self.vsyncend, self.vtotal, self.flags, self.privsize = unpacker.unpack(
+            "IHHHHIHHHH4xI12xI")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=IHHHHIHHHH4xI12xI", self.dotclock, self.hdisplay, self.hsyncstart, self.hsyncend, self.htotal, self.hskew, self.vdisplay, self.vsyncstart, self.vsyncend, self.vtotal, self.flags, self.privsize))
+        buf.write(
+            struct.pack(
+                "=IHHHHIHHHH4xI12xI",
+                self.dotclock,
+                self.hdisplay,
+                self.hsyncstart,
+                self.hsyncend,
+                self.htotal,
+                self.hskew,
+                self.vdisplay,
+                self.vsyncstart,
+                self.vsyncend,
+                self.vtotal,
+                self.flags,
+                self.privsize))
         return buf.getvalue()
     fixed_size = 48
+
+
 class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.major_version, self.minor_version = unpacker.unpack("xx2x4xHH")
         self.bufsize = unpacker.offset - base
+
+
 class QueryVersionCookie(xcffib.Cookie):
     reply_type = QueryVersionReply
+
+
 class GetModeLineReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.dotclock, self.hdisplay, self.hsyncstart, self.hsyncend, self.htotal, self.hskew, self.vdisplay, self.vsyncstart, self.vsyncend, self.vtotal, self.flags, self.privsize = unpacker.unpack("xx2x4xIHHHHHHHHH2xI12xI")
+        self.dotclock, self.hdisplay, self.hsyncstart, self.hsyncend, self.htotal, self.hskew, self.vdisplay, self.vsyncstart, self.vsyncend, self.vtotal, self.flags, self.privsize = unpacker.unpack(
+            "xx2x4xIHHHHHHHHH2xI12xI")
         self.private = xcffib.List(unpacker, "B", self.privsize)
         self.bufsize = unpacker.offset - base
+
+
 class GetModeLineCookie(xcffib.Cookie):
     reply_type = GetModeLineReply
+
+
 class GetMonitorReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.vendor_length, self.model_length, self.num_hsync, self.num_vsync = unpacker.unpack("xx2x4xBBBB20x")
+        self.vendor_length, self.model_length, self.num_hsync, self.num_vsync = unpacker.unpack(
+            "xx2x4xBBBB20x")
         self.hsync = xcffib.List(unpacker, "I", self.num_hsync)
         unpacker.pad("I")
         self.vsync = xcffib.List(unpacker, "I", self.num_vsync)
         unpacker.pad("c")
         self.vendor = xcffib.List(unpacker, "c", self.vendor_length)
         unpacker.pad("c")
-        self.alignment_pad = xcffib.List(unpacker, "c", ((self.vendor_length + 3) & (~ 3)) - self.vendor_length)
+        self.alignment_pad = xcffib.List(
+            unpacker,
+            "c",
+            ((self.vendor_length +
+              3) & (
+                ~ 3)) -
+            self.vendor_length)
         unpacker.pad("c")
         self.model = xcffib.List(unpacker, "c", self.model_length)
         self.bufsize = unpacker.offset - base
+
+
 class GetMonitorCookie(xcffib.Cookie):
     reply_type = GetMonitorReply
+
+
 class GetAllModeLinesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.modecount, = unpacker.unpack("xx2x4xI20x")
         self.modeinfo = xcffib.List(unpacker, ModeInfo, self.modecount)
         self.bufsize = unpacker.offset - base
+
+
 class GetAllModeLinesCookie(xcffib.Cookie):
     reply_type = GetAllModeLinesReply
+
+
 class ValidateModeLineReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.status, = unpacker.unpack("xx2x4xI20x")
         self.bufsize = unpacker.offset - base
+
+
 class ValidateModeLineCookie(xcffib.Cookie):
     reply_type = ValidateModeLineReply
+
+
 class GetViewPortReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.x, self.y = unpacker.unpack("xx2x4xII16x")
         self.bufsize = unpacker.offset - base
+
+
 class GetViewPortCookie(xcffib.Cookie):
     reply_type = GetViewPortReply
+
+
 class GetDotClocksReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.flags, self.clocks, self.maxclocks = unpacker.unpack("xx2x4xIII12x")
-        self.clock = xcffib.List(unpacker, "I", (1 - (self.flags & 1)) * self.clocks)
+        self.flags, self.clocks, self.maxclocks = unpacker.unpack(
+            "xx2x4xIII12x")
+        self.clock = xcffib.List(
+            unpacker, "I", (1 - (self.flags & 1)) * self.clocks)
         self.bufsize = unpacker.offset - base
+
+
 class GetDotClocksCookie(xcffib.Cookie):
     reply_type = GetDotClocksReply
+
+
 class GetGammaReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.red, self.green, self.blue = unpacker.unpack("xx2x4xIII12x")
         self.bufsize = unpacker.offset - base
+
+
 class GetGammaCookie(xcffib.Cookie):
     reply_type = GetGammaReply
+
+
 class GetGammaRampReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.size, = unpacker.unpack("xx2x4xH22x")
         self.red = xcffib.List(unpacker, "H", (self.size + 1) & (~ 1))
         unpacker.pad("H")
         self.green = xcffib.List(unpacker, "H", (self.size + 1) & (~ 1))
         unpacker.pad("H")
         self.blue = xcffib.List(unpacker, "H", (self.size + 1) & (~ 1))
         self.bufsize = unpacker.offset - base
+
+
 class GetGammaRampCookie(xcffib.Cookie):
     reply_type = GetGammaRampReply
+
+
 class GetGammaRampSizeReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.size, = unpacker.unpack("xx2x4xH22x")
         self.bufsize = unpacker.offset - base
+
+
 class GetGammaRampSizeCookie(xcffib.Cookie):
     reply_type = GetGammaRampSizeReply
+
+
 class GetPermissionsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.permissions, = unpacker.unpack("xx2x4xI20x")
         self.bufsize = unpacker.offset - base
+
+
 class GetPermissionsCookie(xcffib.Cookie):
     reply_type = GetPermissionsReply
+
+
 class xf86vidmodeExtension(xcffib.Extension):
+
     def QueryVersion(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(0, buf, QueryVersionCookie, is_checked=is_checked)
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
     def GetModeLine(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2x", screen))
-        return self.send_request(1, buf, GetModeLineCookie, is_checked=is_checked)
-    def ModModeLine(self, screen, hdisplay, hsyncstart, hsyncend, htotal, hskew, vdisplay, vsyncstart, vsyncend, vtotal, flags, privsize, private, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIHHHHHHHHH2xI12xI", screen, hdisplay, hsyncstart, hsyncend, htotal, hskew, vdisplay, vsyncstart, vsyncend, vtotal, flags, privsize))
+        return self.send_request(
+            1,
+            buf,
+            GetModeLineCookie,
+            is_checked=is_checked)
+
+    def ModModeLine(
+            self,
+            screen,
+            hdisplay,
+            hsyncstart,
+            hsyncend,
+            htotal,
+            hskew,
+            vdisplay,
+            vsyncstart,
+            vsyncend,
+            vtotal,
+            flags,
+            privsize,
+            private,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIHHHHHHHHH2xI12xI",
+                screen,
+                hdisplay,
+                hsyncstart,
+                hsyncend,
+                htotal,
+                hskew,
+                vdisplay,
+                vsyncstart,
+                vsyncend,
+                vtotal,
+                flags,
+                privsize))
         buf.write(xcffib.pack_list(private, "B"))
         return self.send_request(2, buf, is_checked=is_checked)
+
     def SwitchMode(self, screen, zoom, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xHH", screen, zoom))
         return self.send_request(3, buf, is_checked=is_checked)
+
     def GetMonitor(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2x", screen))
-        return self.send_request(4, buf, GetMonitorCookie, is_checked=is_checked)
+        return self.send_request(
+            4,
+            buf,
+            GetMonitorCookie,
+            is_checked=is_checked)
+
     def LockModeSwitch(self, screen, lock, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xHH", screen, lock))
         return self.send_request(5, buf, is_checked=is_checked)
+
     def GetAllModeLines(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2x", screen))
-        return self.send_request(6, buf, GetAllModeLinesCookie, is_checked=is_checked)
-    def AddModeLine(self, screen, dotclock, hdisplay, hsyncstart, hsyncend, htotal, hskew, vdisplay, vsyncstart, vsyncend, vtotal, flags, privsize, after_dotclock, after_hdisplay, after_hsyncstart, after_hsyncend, after_htotal, after_hskew, after_vdisplay, after_vsyncstart, after_vsyncend, after_vtotal, after_flags, private, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIHHHHHHHHH2xI12xIIHHHHHHHHH2xI12x", screen, dotclock, hdisplay, hsyncstart, hsyncend, htotal, hskew, vdisplay, vsyncstart, vsyncend, vtotal, flags, privsize, after_dotclock, after_hdisplay, after_hsyncstart, after_hsyncend, after_htotal, after_hskew, after_vdisplay, after_vsyncstart, after_vsyncend, after_vtotal, after_flags))
+        return self.send_request(
+            6,
+            buf,
+            GetAllModeLinesCookie,
+            is_checked=is_checked)
+
+    def AddModeLine(
+            self,
+            screen,
+            dotclock,
+            hdisplay,
+            hsyncstart,
+            hsyncend,
+            htotal,
+            hskew,
+            vdisplay,
+            vsyncstart,
+            vsyncend,
+            vtotal,
+            flags,
+            privsize,
+            after_dotclock,
+            after_hdisplay,
+            after_hsyncstart,
+            after_hsyncend,
+            after_htotal,
+            after_hskew,
+            after_vdisplay,
+            after_vsyncstart,
+            after_vsyncend,
+            after_vtotal,
+            after_flags,
+            private,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIHHHHHHHHH2xI12xIIHHHHHHHHH2xI12x",
+                screen,
+                dotclock,
+                hdisplay,
+                hsyncstart,
+                hsyncend,
+                htotal,
+                hskew,
+                vdisplay,
+                vsyncstart,
+                vsyncend,
+                vtotal,
+                flags,
+                privsize,
+                after_dotclock,
+                after_hdisplay,
+                after_hsyncstart,
+                after_hsyncend,
+                after_htotal,
+                after_hskew,
+                after_vdisplay,
+                after_vsyncstart,
+                after_vsyncend,
+                after_vtotal,
+                after_flags))
         buf.write(xcffib.pack_list(private, "B"))
         return self.send_request(7, buf, is_checked=is_checked)
-    def DeleteModeLine(self, screen, dotclock, hdisplay, hsyncstart, hsyncend, htotal, hskew, vdisplay, vsyncstart, vsyncend, vtotal, flags, privsize, private, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIHHHHHHHHH2xI12xI", screen, dotclock, hdisplay, hsyncstart, hsyncend, htotal, hskew, vdisplay, vsyncstart, vsyncend, vtotal, flags, privsize))
+
+    def DeleteModeLine(
+            self,
+            screen,
+            dotclock,
+            hdisplay,
+            hsyncstart,
+            hsyncend,
+            htotal,
+            hskew,
+            vdisplay,
+            vsyncstart,
+            vsyncend,
+            vtotal,
+            flags,
+            privsize,
+            private,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIHHHHHHHHH2xI12xI",
+                screen,
+                dotclock,
+                hdisplay,
+                hsyncstart,
+                hsyncend,
+                htotal,
+                hskew,
+                vdisplay,
+                vsyncstart,
+                vsyncend,
+                vtotal,
+                flags,
+                privsize))
         buf.write(xcffib.pack_list(private, "B"))
         return self.send_request(8, buf, is_checked=is_checked)
-    def ValidateModeLine(self, screen, dotclock, hdisplay, hsyncstart, hsyncend, htotal, hskew, vdisplay, vsyncstart, vsyncend, vtotal, flags, privsize, private, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIHHHHHHHHH2xI12xI", screen, dotclock, hdisplay, hsyncstart, hsyncend, htotal, hskew, vdisplay, vsyncstart, vsyncend, vtotal, flags, privsize))
+
+    def ValidateModeLine(
+            self,
+            screen,
+            dotclock,
+            hdisplay,
+            hsyncstart,
+            hsyncend,
+            htotal,
+            hskew,
+            vdisplay,
+            vsyncstart,
+            vsyncend,
+            vtotal,
+            flags,
+            privsize,
+            private,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIHHHHHHHHH2xI12xI",
+                screen,
+                dotclock,
+                hdisplay,
+                hsyncstart,
+                hsyncend,
+                htotal,
+                hskew,
+                vdisplay,
+                vsyncstart,
+                vsyncend,
+                vtotal,
+                flags,
+                privsize))
         buf.write(xcffib.pack_list(private, "B"))
-        return self.send_request(9, buf, ValidateModeLineCookie, is_checked=is_checked)
-    def SwitchToMode(self, screen, dotclock, hdisplay, hsyncstart, hsyncend, htotal, hskew, vdisplay, vsyncstart, vsyncend, vtotal, flags, privsize, private, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xIIHHHHHHHHH2xI12xI", screen, dotclock, hdisplay, hsyncstart, hsyncend, htotal, hskew, vdisplay, vsyncstart, vsyncend, vtotal, flags, privsize))
+        return self.send_request(
+            9,
+            buf,
+            ValidateModeLineCookie,
+            is_checked=is_checked)
+
+    def SwitchToMode(
+            self,
+            screen,
+            dotclock,
+            hdisplay,
+            hsyncstart,
+            hsyncend,
+            htotal,
+            hskew,
+            vdisplay,
+            vsyncstart,
+            vsyncend,
+            vtotal,
+            flags,
+            privsize,
+            private,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xIIHHHHHHHHH2xI12xI",
+                screen,
+                dotclock,
+                hdisplay,
+                hsyncstart,
+                hsyncend,
+                htotal,
+                hskew,
+                vdisplay,
+                vsyncstart,
+                vsyncend,
+                vtotal,
+                flags,
+                privsize))
         buf.write(xcffib.pack_list(private, "B"))
         return self.send_request(10, buf, is_checked=is_checked)
+
     def GetViewPort(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2x", screen))
-        return self.send_request(11, buf, GetViewPortCookie, is_checked=is_checked)
+        return self.send_request(
+            11,
+            buf,
+            GetViewPortCookie,
+            is_checked=is_checked)
+
     def SetViewPort(self, screen, x, y, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2xII", screen, x, y))
         return self.send_request(12, buf, is_checked=is_checked)
+
     def GetDotClocks(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2x", screen))
-        return self.send_request(13, buf, GetDotClocksCookie, is_checked=is_checked)
+        return self.send_request(
+            13,
+            buf,
+            GetDotClocksCookie,
+            is_checked=is_checked)
+
     def SetClientVersion(self, major, minor, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xHH", major, minor))
         return self.send_request(14, buf, is_checked=is_checked)
+
     def SetGamma(self, screen, red, green, blue, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2xIII12x", screen, red, green, blue))
         return self.send_request(15, buf, is_checked=is_checked)
+
     def GetGamma(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH26x", screen))
-        return self.send_request(16, buf, GetGammaCookie, is_checked=is_checked)
+        return self.send_request(
+            16,
+            buf,
+            GetGammaCookie,
+            is_checked=is_checked)
+
     def GetGammaRamp(self, screen, size, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xHH", screen, size))
-        return self.send_request(17, buf, GetGammaRampCookie, is_checked=is_checked)
+        return self.send_request(
+            17,
+            buf,
+            GetGammaRampCookie,
+            is_checked=is_checked)
+
     def SetGammaRamp(self, screen, size, red, green, blue, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xHH", screen, size))
         buf.write(xcffib.pack_list(red, "H"))
         buf.write(xcffib.pack_list(green, "H"))
         buf.write(xcffib.pack_list(blue, "H"))
         return self.send_request(18, buf, is_checked=is_checked)
+
     def GetGammaRampSize(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2x", screen))
-        return self.send_request(19, buf, GetGammaRampSizeCookie, is_checked=is_checked)
+        return self.send_request(
+            19,
+            buf,
+            GetGammaRampSizeCookie,
+            is_checked=is_checked)
+
     def GetPermissions(self, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH2x", screen))
-        return self.send_request(20, buf, GetPermissionsCookie, is_checked=is_checked)
+        return self.send_request(
+            20,
+            buf,
+            GetPermissionsCookie,
+            is_checked=is_checked)
 xcffib._add_ext(key, xf86vidmodeExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/__init__.py` & `xcffib-v0.1.4/xcffib/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import division, absolute_import
 
+__xcb_proto_version__ = "1.10"
+
 import functools
 import six
 import struct
+import weakref
 
-from .ffi import ffi, C, bytes_to_cdata, visualtype_to_c_struct
+from .ffi import ffi, C, visualtype_to_c_struct  # noqa
 
 X_PROTOCOL = C.X_PROTOCOL
 X_PROTOCOL_REVISION = C.X_PROTOCOL_REVISION
 
 XCB_NONE = C.XCB_NONE
 XCB_COPY_FROM_PARENT = C.XCB_COPY_FROM_PARENT
 XCB_CURRENT_TIME = C.XCB_CURRENT_TIME
@@ -24,22 +27,24 @@
 XCB_CONN_CLOSED_EXT_NOTSUPPORTED = C.XCB_CONN_CLOSED_EXT_NOTSUPPORTED
 XCB_CONN_CLOSED_MEM_INSUFFICIENT = C.XCB_CONN_CLOSED_MEM_INSUFFICIENT
 XCB_CONN_CLOSED_REQ_LEN_EXCEED = C.XCB_CONN_CLOSED_REQ_LEN_EXCEED
 XCB_CONN_CLOSED_PARSE_ERR = C.XCB_CONN_CLOSED_PARSE_ERR
 # XCB_CONN_CLOSED_INVALID_SCREEN = C.XCB_CONN_CLOSED_INVALID_SCREEN
 # XCB_CONN_CLOSED_FDPASSING_FAILED = C.XCB_CONN_CLOSED_FDPASSING_FAILED
 
+cffi_explicit_lifetimes = weakref.WeakKeyDictionary()
+
 
 def type_pad(t, i):
     return -i & (3 if t > 4 else t - 1)
 
 
 class Unpacker(object):
 
-    def __init__(self, cdata, known_max=None, needs_pad=False):
+    def __init__(self, cdata, known_max=None):
         self.cdata = cdata
         self.size = 0
         self.offset = 0
         self.known_max = known_max
         if self.known_max is not None:
             self._resize(known_max)
 
@@ -47,15 +52,16 @@
         if self.offset + increment > self.size:
             if self.known_max is not None:
                 assert self.size + increment <= self.known_max
             self.size = self.offset + increment
             self.buf = ffi.buffer(self.cdata, self.size)
 
     def pad(self, thing):
-        if isinstance(thing, type) and any([issubclass(thing, c) for c in [Struct, Union]]):
+        if isinstance(thing, type) and any(
+                [issubclass(thing, c) for c in [Struct, Union]]):
             if hasattr(thing, "fixed_size"):
                 size = thing.fixed_size
             else:
                 size = 4
         else:
             size = struct.calcsize(thing)
 
@@ -70,20 +76,26 @@
             self.offset += size
         return ret
 
     def cast(self, typ):
         assert self.offset == 0
         return ffi.cast(typ, self.cdata)
 
+    def copy(self):
+        new = Unpacker(self.cdata, self.known_max)
+        new.offset = self.offset
+        return new
+
 
 def popcount(n):
     return bin(n).count('1')
 
 
 class XcffibException(Exception):
+
     """ Generic XcbException; replaces xcb.Exception. """
     pass
 
 
 class ConnectionException(XcffibException):
     REASONS = {
         C.XCB_CONN_ERROR: (
@@ -95,19 +107,19 @@
             'malloc(), calloc() and realloc() error upon failure, '
             'for eg ENOMEM'),
         C.XCB_CONN_CLOSED_REQ_LEN_EXCEED: (
             'Connection closed, exceeding request length that server '
             'accepts.'),
         C.XCB_CONN_CLOSED_PARSE_ERR: (
             'Connection closed, error during parsing display string.'),
-#        C.XCB_CONN_CLOSED_INVALID_SCREEN: (
-#            'Connection closed because the server does not have a screen '
-#            'matching the display.'),
-#        C.XCB_CONN_CLOSED_FDPASSING_FAILED: (
-#            'Connection closed because some FD passing operation failed'),
+        #        C.XCB_CONN_CLOSED_INVALID_SCREEN: (
+        #            'Connection closed because the server does not have a screen '
+        #            'matching the display.'),
+        #        C.XCB_CONN_CLOSED_FDPASSING_FAILED: (
+        #            'Connection closed because some FD passing operation failed'),
     }
 
     def __init__(self, err):
         XcffibException.__init__(
             self, self.REASONS.get(err, "Unknown connection error."))
 
 
@@ -120,17 +132,20 @@
 core_errors = None
 setup = None
 
 extensions = {}
 
 # This seems a bit over engineered to me; it seems unlikely there will ever be
 # a core besides xproto, so why not just hardcode that?
+
+
 def _add_core(value, _setup, events, errors):
     if not issubclass(value, Extension):
-        raise XcffibException("Extension type not derived from xcffib.Extension")
+        raise XcffibException(
+            "Extension type not derived from xcffib.Extension")
     if not issubclass(_setup, Struct):
         raise XcffibException("Setup type not derived from xcffib.Struct")
 
     global core
     global core_events
     global core_errors
     global setup
@@ -139,34 +154,46 @@
     core_events = events
     core_errors = errors
     setup = _setup
 
 
 def _add_ext(key, value, events, errors):
     if not issubclass(value, Extension):
-        raise XcffibException("Extension type not derived from xcffib.Extension")
+        raise XcffibException(
+            "Extension type not derived from xcffib.Extension")
     extensions[key] = (value, events, errors)
 
 
 class ExtensionKey(object):
+
     """ This definitely isn't needed, but we keep it around for compatibilty
     with xpyb.
     """
+
     def __init__(self, name):
         self.name = name
 
     def __hash__(self):
         return hash(self.name)
 
     def __eq__(self, o):
         return self.name == o.name
 
     def __ne__(self, o):
         return self.name != o.name
 
+    def to_cffi(self):
+        c_key = ffi.new("struct xcb_extension_t *")
+        c_key.name = name = ffi.new('char[]', self.name.encode())
+        cffi_explicit_lifetimes[c_key] = name
+        # xpyb doesn't ever set global_id, which seems wrong, but whatever.
+        c_key.global_id = 0
+
+        return c_key
+
 
 class Protobj(object):
 
     """ Note: Unlike xcb.Protobj, this does NOT implement the sequence
     protocol. I found this behavior confusing: Protobj would implement the
     sequence protocol on self.buf, and then List would go and implement it on
     List. Additionally, as near as I can tell internally we only need the size
@@ -188,24 +215,26 @@
     @classmethod
     def synthetic(cls, **kwargs):
         self = cls.__new__(cls)
         for k, v in kwargs.items():
             setattr(self, k, v)
         return self
 
+
 class Struct(Protobj):
     pass
 
 
 class Union(Protobj):
     pass
 
 
 class Cookie(object):
     reply_type = None
+
     def __init__(self, conn, sequence, is_checked):
         self.conn = conn
         self.sequence = sequence
         self.is_checked = is_checked
 
     def reply(self):
         data = self.conn.wait_for_reply(self.sequence)
@@ -215,52 +244,47 @@
         # Request is not void and checked.
         assert self.is_checked and self.reply_type is None, (
             "Request is not void and checked")
         self.conn.request_check(self.sequence)
 
 
 class VoidCookie(Cookie):
+
     def reply(self):
         raise XcffibException("No reply for this message type")
 
 
 class Extension(object):
+
     def __init__(self, conn, key=None):
         self.conn = conn
+
         if key is None:
-            self.ext_name = None
+            self.c_key = ffi.NULL
         else:
-            self.ext_name = key.name
+            self.c_key = key.to_cffi()
 
     def send_request(self, opcode, data, cookie=VoidCookie, reply=None,
                      is_checked=False):
         data = data.getvalue()
 
         assert len(data) > 3, "xcb_send_request data must be ast least 4 bytes"
 
         xcb_req = ffi.new("xcb_protocol_request_t *")
         xcb_req.count = 2
-
-        if self.ext_name is not None:
-            key = ffi.new("struct xcb_extension_t *")
-            key.name = bytes_to_cdata(self.ext_name.encode())
-            # xpyb doesn't ever set global_id, which seems wrong, but whatever.
-            key.global_id = 0
-            xcb_req.ext = key
-        else:
-            xcb_req.ext = ffi.NULL
-
+        xcb_req.ext = self.c_key
         xcb_req.opcode = opcode
         xcb_req.isvoid = issubclass(cookie, VoidCookie)
 
         xcb_parts = ffi.new("struct iovec[2]")
-        xcb_parts[0].iov_base = bytes_to_cdata(data)
+        xcb_parts[0].iov_base = iov_base = ffi.new('char[]', data)
         xcb_parts[0].iov_len = len(data)
         xcb_parts[1].iov_base = ffi.NULL
         xcb_parts[1].iov_len = -len(data) & 3  # is this really necessary?
+        cffi_explicit_lifetimes[xcb_parts] = iov_base
 
         flags = C.XCB_REQUEST_CHECKED if is_checked else 0
 
         seq = self.conn.send_request(flags, xcb_parts, xcb_req)
 
         return cookie(self.conn, seq, is_checked)
 
@@ -276,14 +300,15 @@
 
         real = getattr(self, real)
 
         return functools.partial(real, is_checked=is_checked)
 
 
 class List(Protobj):
+
     def __init__(self, unpacker, typ, count=None):
         Protobj.__init__(self, unpacker)
 
         self.list = []
         old = unpacker.offset
 
         if isinstance(typ, str):
@@ -320,49 +345,83 @@
     def __delitem__(self, key):
         del self.list[key]
 
     def to_string(self):
         """ A helper for converting a List of chars to a native string. Dies if
         the list contents are not something that could be reasonably converted
         to a string. """
-        return b''.join(self).decode('latin1')
+        return ''.join(chr(six.byte2int(i)) for i in self)
 
     def to_atoms(self):
         """ A helper for converting a List of chars to an array of atoms """
         return struct.unpack("=" + "I" * (len(self) // 4), b''.join(self))
 
     def buf(self):
         return b''.join(self.list)
 
+
+class OffsetMap(object):
+
+    def __init__(self, core):
+        self.offsets = [(0, core)]
+
+    def add(self, offset, things):
+        self.offsets.append((offset, things))
+        self.offsets.sort(key=lambda x: x[0], reverse=True)
+
+    def __getitem__(self, item):
+        try:
+            offset, things = next((k, v) for k, v in self.offsets if item >= k)
+            return things[item - offset]
+        except StopIteration:
+            raise IndexError(item)
+
+
 class Connection(object):
 
     def __init__(self, display=None, fd=-1, auth=None):
         if auth is not None:
             c_auth = ffi.new("xcb_auth_info_t *")
             if C.xpyb_parse_auth(auth, len(auth), c_auth) < 0:
                 raise XcffibException("invalid xauth")
         else:
             c_auth = ffi.NULL
-        display = display.encode('latin1')
+
+        if display is None:
+            display = ffi.NULL
+        else:
+            display = display.encode('latin1')
 
         i = ffi.new("int *")
-        i[0] = 0
 
         if fd > 0:
             self._conn = C.xcb_connect_to_fd(fd, c_auth)
         elif c_auth != ffi.NULL:
             self._conn = C.xcb_connect_to_display_with_auth(display, c_auth, i)
         else:
             self._conn = C.xcb_connect(display, i)
         self.pref_screen = i[0]
         self.invalid()
 
         self.core = core(self)
         self.setup = self.get_setup()
 
+        self._event_offsets = OffsetMap(core_events)
+        self._error_offsets = OffsetMap(core_errors)
+        self._setup_extensions()
+
+    def _setup_extensions(self):
+        for key, (_, events, errors) in extensions.items():
+            # We're explicitly not putting this as an argument to the next call
+            # as a hack for lifetime management.
+            c_ext = key.to_cffi()
+            reply = C.xcb_get_extension_data(self._conn, c_ext)
+            self._event_offsets.add(reply.first_event, events)
+            self._error_offsets.add(reply.first_error, errors)
+
     def __call__(self, key):
         return extensions[key][0](self, key)
 
     def invalid(self):
         if self._conn is None:
             raise XcffibException("Invalid connection.")
         err = C.xcb_connection_has_error(self._conn)
@@ -437,15 +496,15 @@
     def disconnect(self):
         self.invalid()
         return C.xcb_disconnect(self._conn)
 
     def _process_error(self, c_error):
         self.invalid()
         if c_error != ffi.NULL:
-            error = core_errors[c_error.error_code]
+            error = self._error_offsets[c_error.error_code]
             buf = Unpacker(c_error)
             raise error(buf)
 
     @ensure_connected
     def wait_for_reply(self, sequence):
         error_p = ffi.new("xcb_generic_error_t **")
         data = C.xcb_wait_for_reply(self._conn, sequence, error_p)
@@ -475,96 +534,97 @@
         self._process_error(err)
 
     def hoist_event(self, e):
         """ Hoist an xcb_generic_event_t to the right xcffib structure. """
         if e.response_type == 0:
             return self._process_error(ffi.cast("xcb_generic_error_t *", e))
 
-        assert core_events, "You probably need to import xcffib.xproto"
         # We mask off the high bit here because events sent with SendEvent have
         # this bit set. We don't actually care where the event came from, so we
         # just throw this away. Maybe we could expose this, if anyone actually
         # cares about it.
-        event = core_events[e.response_type & 0x7f]
+        event = self._event_offsets[e.response_type & 0x7f]
 
         buf = Unpacker(e)
         return event(buf)
 
+    @ensure_connected
     def send_request(self, flags, xcb_parts, xcb_req):
-        self.invalid()
         return C.xcb_send_request(self._conn, flags, xcb_parts, xcb_req)
 
+
 # More backwards compatibility
 connect = Connection
 
 
 class Response(Protobj):
+
     def __init__(self, unpacker):
         Protobj.__init__(self, unpacker)
 
         # These (and the ones in Reply) aren't used internally and I suspect
         # they're not used by anyone else, but they're here for xpyb
         # compatibility.
         resp = unpacker.cast("xcb_generic_event_t *")
         self.response_type = resp.response_type
         self.sequence = resp.sequence
 
 
 class Reply(Response):
+
     def __init__(self, unpacker):
         Response.__init__(self, unpacker)
 
         # also for compat
         resp = unpacker.cast("xcb_generic_reply_t *")
         self.length = resp.length
 
 
 class Event(Response):
     pass
 
 
 class Error(Response, XcffibException):
+
     def __init__(self, unpacker):
         Response.__init__(self, unpacker)
         XcffibException.__init__(self)
         self.code = unpacker.unpack('B', increment=False)
 
 
 def pack_list(from_, pack_type):
     """ Return the wire packed version of `from_`. `pack_type` should be some
     subclass of `xcffib.Struct`, or a string that can be passed to
     `struct.pack`. You must pass `size` if `pack_type` is a struct.pack string.
     """
-
-    if six.PY3:
-        # If a string is passed as `from_` in Python 3, it has to be encoded
-        if isinstance(from_, str):
-            from_ = [b.encode('latin1') for b in from_]
-        # PY3 is "helpful" in that when you do tuple(b'foo') you get
-        # (102, 111, 111) instead of something more reasonable like
-        # (b'f', b'o', b'o'), so we have to add this other special case.
-        elif isinstance(from_, bytes):
-            from_ = [bytes([b]) for b in from_]
-
-    try:
-        elt_type = type(from_[0])
-    except IndexError:
+    # We need from_ to not be empty
+    if len(from_) == 0:
         return bytes()
 
-    # Pack from_ as char array, where from_ may be an array of ints possibly
-    # greater than 256
-    if pack_type == 'c' and issubclass(elt_type, int):
-        def to_bytes(v):
-            for _ in range(4):
-                v, r = divmod(v, 256)
-                yield r
-        from_ = [bytes(bytearray([b])) for i in from_ for b in to_bytes(i)]
+    if pack_type == 'c':
+        if isinstance(from_, bytes):
+            # PY3 is "helpful" in that when you do tuple(b'foo') you get
+            # (102, 111, 111) instead of something more reasonable like
+            # (b'f', b'o', b'o'), so we rebuild from_ as a tuple of bytes
+            from_ = [six.int2byte(b) for b in six.iterbytes(from_)]
+        elif isinstance(from_, str):
+            # Only run in Python 3, where bytes are different than strings
+            # Here we create the tuple of bytes by encoding each character
+            from_ = [b.encode('latin-1') for b in from_]
+        elif isinstance(from_[0], int):
+            # Pack from_ as char array, where from_ may be an array of ints
+            # possibly greater than 256
+            def to_bytes(v):
+                for _ in range(4):
+                    v, r = divmod(v, 256)
+                    yield r
+            from_ = [six.int2byte(b) for i in from_ for b in to_bytes(i)]
 
     if isinstance(pack_type, six.string_types):
-        return struct.pack("=" + pack_type * len(from_), *tuple(from_))
+        return struct.pack("=" + pack_type * len(from_), *from_)
     else:
         buf = six.BytesIO()
         for item in from_:
             # If we can't pack it, you'd better have packed it yourself...
             if isinstance(item, Struct):
                 buf.write(item.pack())
             else:
```

### Comparing `xcffib-v0.1.3/xcffib/xselinux.py` & `xcffib-v0.1.4/xcffib/xselinux.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,266 +3,452 @@
 import six
 MAJOR_VERSION = 1
 MINOR_VERSION = 0
 key = xcffib.ExtensionKey("SELinux")
 _events = {}
 _errors = {}
 from . import xproto
+
+
 class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.server_major, self.server_minor = unpacker.unpack("xx2x4xHH")
         self.bufsize = unpacker.offset - base
+
+
 class QueryVersionCookie(xcffib.Cookie):
     reply_type = QueryVersionReply
+
+
 class GetDeviceCreateContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.context_len, = unpacker.unpack("xx2x4xI20x")
         self.context = xcffib.List(unpacker, "c", self.context_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetDeviceCreateContextCookie(xcffib.Cookie):
     reply_type = GetDeviceCreateContextReply
+
+
 class GetDeviceContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.context_len, = unpacker.unpack("xx2x4xI20x")
         self.context = xcffib.List(unpacker, "c", self.context_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetDeviceContextCookie(xcffib.Cookie):
     reply_type = GetDeviceContextReply
+
+
 class GetWindowCreateContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.context_len, = unpacker.unpack("xx2x4xI20x")
         self.context = xcffib.List(unpacker, "c", self.context_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetWindowCreateContextCookie(xcffib.Cookie):
     reply_type = GetWindowCreateContextReply
+
+
 class GetWindowContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.context_len, = unpacker.unpack("xx2x4xI20x")
         self.context = xcffib.List(unpacker, "c", self.context_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetWindowContextCookie(xcffib.Cookie):
     reply_type = GetWindowContextReply
+
+
 class ListItem(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.name, self.object_context_len, self.data_context_len = unpacker.unpack("III")
-        self.object_context = xcffib.List(unpacker, "c", self.object_context_len)
+        self.name, self.object_context_len, self.data_context_len = unpacker.unpack(
+            "III")
+        self.object_context = xcffib.List(
+            unpacker,
+            "c",
+            self.object_context_len)
         unpacker.pad("c")
         self.data_context = xcffib.List(unpacker, "c", self.data_context_len)
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=III", self.name, self.object_context_len, self.data_context_len))
+        buf.write(
+            struct.pack(
+                "=III",
+                self.name,
+                self.object_context_len,
+                self.data_context_len))
         buf.write(xcffib.pack_list(self.object_context, "c"))
         buf.write(xcffib.pack_list(self.data_context, "c"))
         return buf.getvalue()
+
+
 class GetPropertyCreateContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.context_len, = unpacker.unpack("xx2x4xI20x")
         self.context = xcffib.List(unpacker, "c", self.context_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetPropertyCreateContextCookie(xcffib.Cookie):
     reply_type = GetPropertyCreateContextReply
+
+
 class GetPropertyUseContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.context_len, = unpacker.unpack("xx2x4xI20x")
         self.context = xcffib.List(unpacker, "c", self.context_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetPropertyUseContextCookie(xcffib.Cookie):
     reply_type = GetPropertyUseContextReply
+
+
 class GetPropertyContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.context_len, = unpacker.unpack("xx2x4xI20x")
         self.context = xcffib.List(unpacker, "c", self.context_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetPropertyContextCookie(xcffib.Cookie):
     reply_type = GetPropertyContextReply
+
+
 class GetPropertyDataContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.context_len, = unpacker.unpack("xx2x4xI20x")
         self.context = xcffib.List(unpacker, "c", self.context_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetPropertyDataContextCookie(xcffib.Cookie):
     reply_type = GetPropertyDataContextReply
+
+
 class ListPropertiesReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.properties_len, = unpacker.unpack("xx2x4xI20x")
         self.properties = xcffib.List(unpacker, ListItem, self.properties_len)
         self.bufsize = unpacker.offset - base
+
+
 class ListPropertiesCookie(xcffib.Cookie):
     reply_type = ListPropertiesReply
+
+
 class GetSelectionCreateContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.context_len, = unpacker.unpack("xx2x4xI20x")
         self.context = xcffib.List(unpacker, "c", self.context_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetSelectionCreateContextCookie(xcffib.Cookie):
     reply_type = GetSelectionCreateContextReply
+
+
 class GetSelectionUseContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.context_len, = unpacker.unpack("xx2x4xI20x")
         self.context = xcffib.List(unpacker, "c", self.context_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetSelectionUseContextCookie(xcffib.Cookie):
     reply_type = GetSelectionUseContextReply
+
+
 class GetSelectionContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.context_len, = unpacker.unpack("xx2x4xI20x")
         self.context = xcffib.List(unpacker, "c", self.context_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetSelectionContextCookie(xcffib.Cookie):
     reply_type = GetSelectionContextReply
+
+
 class GetSelectionDataContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.context_len, = unpacker.unpack("xx2x4xI20x")
         self.context = xcffib.List(unpacker, "c", self.context_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetSelectionDataContextCookie(xcffib.Cookie):
     reply_type = GetSelectionDataContextReply
+
+
 class ListSelectionsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.selections_len, = unpacker.unpack("xx2x4xI20x")
         self.selections = xcffib.List(unpacker, ListItem, self.selections_len)
         self.bufsize = unpacker.offset - base
+
+
 class ListSelectionsCookie(xcffib.Cookie):
     reply_type = ListSelectionsReply
+
+
 class GetClientContextReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.context_len, = unpacker.unpack("xx2x4xI20x")
         self.context = xcffib.List(unpacker, "c", self.context_len)
         self.bufsize = unpacker.offset - base
+
+
 class GetClientContextCookie(xcffib.Cookie):
     reply_type = GetClientContextReply
+
+
 class xselinuxExtension(xcffib.Extension):
+
     def QueryVersion(self, client_major, client_minor, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xB", client_major, client_minor))
-        return self.send_request(0, buf, QueryVersionCookie, is_checked=is_checked)
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
     def SetDeviceCreateContext(self, context_len, context, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context_len))
         buf.write(xcffib.pack_list(context, "c"))
         return self.send_request(1, buf, is_checked=is_checked)
+
     def GetDeviceCreateContext(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(2, buf, GetDeviceCreateContextCookie, is_checked=is_checked)
+        return self.send_request(
+            2,
+            buf,
+            GetDeviceCreateContextCookie,
+            is_checked=is_checked)
+
     def SetDeviceContext(self, device, context_len, context, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", device, context_len))
         buf.write(xcffib.pack_list(context, "c"))
         return self.send_request(3, buf, is_checked=is_checked)
+
     def GetDeviceContext(self, device, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", device))
-        return self.send_request(4, buf, GetDeviceContextCookie, is_checked=is_checked)
+        return self.send_request(
+            4,
+            buf,
+            GetDeviceContextCookie,
+            is_checked=is_checked)
+
     def SetWindowCreateContext(self, context_len, context, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context_len))
         buf.write(xcffib.pack_list(context, "c"))
         return self.send_request(5, buf, is_checked=is_checked)
+
     def GetWindowCreateContext(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(6, buf, GetWindowCreateContextCookie, is_checked=is_checked)
+        return self.send_request(
+            6,
+            buf,
+            GetWindowCreateContextCookie,
+            is_checked=is_checked)
+
     def GetWindowContext(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(7, buf, GetWindowContextCookie, is_checked=is_checked)
+        return self.send_request(
+            7,
+            buf,
+            GetWindowContextCookie,
+            is_checked=is_checked)
+
     def SetPropertyCreateContext(self, context_len, context, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context_len))
         buf.write(xcffib.pack_list(context, "c"))
         return self.send_request(8, buf, is_checked=is_checked)
+
     def GetPropertyCreateContext(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(9, buf, GetPropertyCreateContextCookie, is_checked=is_checked)
+        return self.send_request(
+            9,
+            buf,
+            GetPropertyCreateContextCookie,
+            is_checked=is_checked)
+
     def SetPropertyUseContext(self, context_len, context, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context_len))
         buf.write(xcffib.pack_list(context, "c"))
         return self.send_request(10, buf, is_checked=is_checked)
+
     def GetPropertyUseContext(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(11, buf, GetPropertyUseContextCookie, is_checked=is_checked)
+        return self.send_request(
+            11,
+            buf,
+            GetPropertyUseContextCookie,
+            is_checked=is_checked)
+
     def GetPropertyContext(self, window, property, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", window, property))
-        return self.send_request(12, buf, GetPropertyContextCookie, is_checked=is_checked)
+        return self.send_request(
+            12,
+            buf,
+            GetPropertyContextCookie,
+            is_checked=is_checked)
+
     def GetPropertyDataContext(self, window, property, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", window, property))
-        return self.send_request(13, buf, GetPropertyDataContextCookie, is_checked=is_checked)
+        return self.send_request(
+            13,
+            buf,
+            GetPropertyDataContextCookie,
+            is_checked=is_checked)
+
     def ListProperties(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(14, buf, ListPropertiesCookie, is_checked=is_checked)
-    def SetSelectionCreateContext(self, context_len, context, is_checked=False):
+        return self.send_request(
+            14,
+            buf,
+            ListPropertiesCookie,
+            is_checked=is_checked)
+
+    def SetSelectionCreateContext(
+            self,
+            context_len,
+            context,
+            is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context_len))
         buf.write(xcffib.pack_list(context, "c"))
         return self.send_request(15, buf, is_checked=is_checked)
+
     def GetSelectionCreateContext(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(16, buf, GetSelectionCreateContextCookie, is_checked=is_checked)
+        return self.send_request(
+            16,
+            buf,
+            GetSelectionCreateContextCookie,
+            is_checked=is_checked)
+
     def SetSelectionUseContext(self, context_len, context, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", context_len))
         buf.write(xcffib.pack_list(context, "c"))
         return self.send_request(17, buf, is_checked=is_checked)
+
     def GetSelectionUseContext(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(18, buf, GetSelectionUseContextCookie, is_checked=is_checked)
+        return self.send_request(
+            18,
+            buf,
+            GetSelectionUseContextCookie,
+            is_checked=is_checked)
+
     def GetSelectionContext(self, selection, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", selection))
-        return self.send_request(19, buf, GetSelectionContextCookie, is_checked=is_checked)
+        return self.send_request(
+            19,
+            buf,
+            GetSelectionContextCookie,
+            is_checked=is_checked)
+
     def GetSelectionDataContext(self, selection, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", selection))
-        return self.send_request(20, buf, GetSelectionDataContextCookie, is_checked=is_checked)
+        return self.send_request(
+            20,
+            buf,
+            GetSelectionDataContextCookie,
+            is_checked=is_checked)
+
     def ListSelections(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(21, buf, ListSelectionsCookie, is_checked=is_checked)
+        return self.send_request(
+            21,
+            buf,
+            ListSelectionsCookie,
+            is_checked=is_checked)
+
     def GetClientContext(self, resource, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", resource))
-        return self.send_request(22, buf, GetClientContextCookie, is_checked=is_checked)
+        return self.send_request(
+            22,
+            buf,
+            GetClientContextCookie,
+            is_checked=is_checked)
 xcffib._add_ext(key, xselinuxExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/dpms.py` & `xcffib-v0.1.4/xcffib/dpms.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,78 +2,138 @@
 import struct
 import six
 MAJOR_VERSION = 0
 MINOR_VERSION = 0
 key = xcffib.ExtensionKey("DPMS")
 _events = {}
 _errors = {}
+
+
 class GetVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.server_major_version, self.server_minor_version = unpacker.unpack("xx2x4xHH")
+        self.server_major_version, self.server_minor_version = unpacker.unpack(
+            "xx2x4xHH")
         self.bufsize = unpacker.offset - base
+
+
 class GetVersionCookie(xcffib.Cookie):
     reply_type = GetVersionReply
+
+
 class CapableReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.capable, = unpacker.unpack("xx2x4xB23x")
         self.bufsize = unpacker.offset - base
+
+
 class CapableCookie(xcffib.Cookie):
     reply_type = CapableReply
+
+
 class GetTimeoutsReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.standby_timeout, self.suspend_timeout, self.off_timeout = unpacker.unpack("xx2x4xHHH18x")
+        self.standby_timeout, self.suspend_timeout, self.off_timeout = unpacker.unpack(
+            "xx2x4xHHH18x")
         self.bufsize = unpacker.offset - base
+
+
 class GetTimeoutsCookie(xcffib.Cookie):
     reply_type = GetTimeoutsReply
+
+
 class DPMSMode:
     On = 0
     Standby = 1
     Suspend = 2
     Off = 3
+
+
 class InfoReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.power_level, self.state = unpacker.unpack("xx2x4xHB21x")
         self.bufsize = unpacker.offset - base
+
+
 class InfoCookie(xcffib.Cookie):
     reply_type = InfoReply
+
+
 class dpmsExtension(xcffib.Extension):
-    def GetVersion(self, client_major_version, client_minor_version, is_checked=True):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xHH", client_major_version, client_minor_version))
-        return self.send_request(0, buf, GetVersionCookie, is_checked=is_checked)
+
+    def GetVersion(
+            self,
+            client_major_version,
+            client_minor_version,
+            is_checked=True):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xHH",
+                client_major_version,
+                client_minor_version))
+        return self.send_request(
+            0,
+            buf,
+            GetVersionCookie,
+            is_checked=is_checked)
+
     def Capable(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
         return self.send_request(1, buf, CapableCookie, is_checked=is_checked)
+
     def GetTimeouts(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(2, buf, GetTimeoutsCookie, is_checked=is_checked)
-    def SetTimeouts(self, standby_timeout, suspend_timeout, off_timeout, is_checked=False):
-        buf = six.BytesIO()
-        buf.write(struct.pack("=xx2xHHH", standby_timeout, suspend_timeout, off_timeout))
+        return self.send_request(
+            2,
+            buf,
+            GetTimeoutsCookie,
+            is_checked=is_checked)
+
+    def SetTimeouts(
+            self,
+            standby_timeout,
+            suspend_timeout,
+            off_timeout,
+            is_checked=False):
+        buf = six.BytesIO()
+        buf.write(
+            struct.pack(
+                "=xx2xHHH",
+                standby_timeout,
+                suspend_timeout,
+                off_timeout))
         return self.send_request(3, buf, is_checked=is_checked)
+
     def Enable(self, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
         return self.send_request(4, buf, is_checked=is_checked)
+
     def Disable(self, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
         return self.send_request(5, buf, is_checked=is_checked)
+
     def ForceLevel(self, power_level, is_checked=False):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xH", power_level))
         return self.send_request(6, buf, is_checked=is_checked)
+
     def Info(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
         return self.send_request(7, buf, InfoCookie, is_checked=is_checked)
 xcffib._add_ext(key, dpmsExtension, _events, _errors)
```

### Comparing `xcffib-v0.1.3/xcffib/xinerama.py` & `xcffib-v0.1.4/xcffib/xinerama.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,93 +3,159 @@
 import six
 MAJOR_VERSION = 1
 MINOR_VERSION = 1
 key = xcffib.ExtensionKey("XINERAMA")
 _events = {}
 _errors = {}
 from . import xproto
+
+
 class ScreenInfo(xcffib.Struct):
+
     def __init__(self, unpacker):
         xcffib.Struct.__init__(self, unpacker)
         base = unpacker.offset
-        self.x_org, self.y_org, self.width, self.height = unpacker.unpack("hhHH")
+        self.x_org, self.y_org, self.width, self.height = unpacker.unpack(
+            "hhHH")
         self.bufsize = unpacker.offset - base
+
     def pack(self):
         buf = six.BytesIO()
-        buf.write(struct.pack("=hhHH", self.x_org, self.y_org, self.width, self.height))
+        buf.write(
+            struct.pack(
+                "=hhHH",
+                self.x_org,
+                self.y_org,
+                self.width,
+                self.height))
         return buf.getvalue()
     fixed_size = 8
+
+
 class QueryVersionReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.major, self.minor = unpacker.unpack("xx2x4xHH")
         self.bufsize = unpacker.offset - base
+
+
 class QueryVersionCookie(xcffib.Cookie):
     reply_type = QueryVersionReply
+
+
 class GetStateReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.state, self.window = unpacker.unpack("xB2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class GetStateCookie(xcffib.Cookie):
     reply_type = GetStateReply
+
+
 class GetScreenCountReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.screen_count, self.window = unpacker.unpack("xB2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class GetScreenCountCookie(xcffib.Cookie):
     reply_type = GetScreenCountReply
+
+
 class GetScreenSizeReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
-        self.width, self.height, self.window, self.screen = unpacker.unpack("xx2x4xIIII")
+        self.width, self.height, self.window, self.screen = unpacker.unpack(
+            "xx2x4xIIII")
         self.bufsize = unpacker.offset - base
+
+
 class GetScreenSizeCookie(xcffib.Cookie):
     reply_type = GetScreenSizeReply
+
+
 class IsActiveReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.state, = unpacker.unpack("xx2x4xI")
         self.bufsize = unpacker.offset - base
+
+
 class IsActiveCookie(xcffib.Cookie):
     reply_type = IsActiveReply
+
+
 class QueryScreensReply(xcffib.Reply):
+
     def __init__(self, unpacker):
         xcffib.Reply.__init__(self, unpacker)
         base = unpacker.offset
         self.number, = unpacker.unpack("xx2x4xI20x")
         self.screen_info = xcffib.List(unpacker, ScreenInfo, self.number)
         self.bufsize = unpacker.offset - base
+
+
 class QueryScreensCookie(xcffib.Cookie):
     reply_type = QueryScreensReply
+
+
 class xineramaExtension(xcffib.Extension):
+
     def QueryVersion(self, major, minor, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xB2xB", major, minor))
-        return self.send_request(0, buf, QueryVersionCookie, is_checked=is_checked)
+        return self.send_request(
+            0,
+            buf,
+            QueryVersionCookie,
+            is_checked=is_checked)
+
     def GetState(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
         return self.send_request(1, buf, GetStateCookie, is_checked=is_checked)
+
     def GetScreenCount(self, window, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xI", window))
-        return self.send_request(2, buf, GetScreenCountCookie, is_checked=is_checked)
+        return self.send_request(
+            2,
+            buf,
+            GetScreenCountCookie,
+            is_checked=is_checked)
+
     def GetScreenSize(self, window, screen, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2xII", window, screen))
-        return self.send_request(3, buf, GetScreenSizeCookie, is_checked=is_checked)
+        return self.send_request(
+            3,
+            buf,
+            GetScreenSizeCookie,
+            is_checked=is_checked)
+
     def IsActive(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
         return self.send_request(4, buf, IsActiveCookie, is_checked=is_checked)
+
     def QueryScreens(self, is_checked=True):
         buf = six.BytesIO()
         buf.write(struct.pack("=xx2x"))
-        return self.send_request(5, buf, QueryScreensCookie, is_checked=is_checked)
+        return self.send_request(
+            5,
+            buf,
+            QueryScreensCookie,
+            is_checked=is_checked)
 xcffib._add_ext(key, xineramaExtension, _events, _errors)
```

