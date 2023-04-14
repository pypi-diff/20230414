# Comparing `tmp/songbird_py-0.1.7.tar.gz` & `tmp/songbird_py-0.1.9.tar.gz`

## Comparing `songbird_py-0.1.7.tar` & `songbird_py-0.1.9.tar`

### file list

```diff
@@ -1,48 +1,50 @@
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 songbird_py-0.1.7/Cargo.toml
--rw-r--r--   0     1001      121     3801 2022-07-23 11:01:11.000000 songbird_py-0.1.7/.github/workflows/publish.yml
--rw-r--r--   0     1001      121      304 2022-07-23 11:01:11.000000 songbird_py-0.1.7/.gitignore
--rw-r--r--   0     1001      121      331 2022-07-23 11:01:11.000000 songbird_py-0.1.7/.readthedocs.yaml
--rw-r--r--   0     1001      121    18092 2022-07-23 11:01:11.000000 songbird_py-0.1.7/LICENSE
--rw-r--r--   0     1001      121       43 2022-07-23 11:01:11.000000 songbird_py-0.1.7/MANIFEST.in
--rw-r--r--   0     1001      121     2756 2022-07-23 11:01:11.000000 songbird_py-0.1.7/README.md
--rw-r--r--   0     1001      121      634 2022-07-23 11:01:11.000000 songbird_py-0.1.7/docs/Makefile
--rw-r--r--   0     1001      121     4618 2022-07-23 11:01:11.000000 songbird_py-0.1.7/docs/conf.py
--rw-r--r--   0     1001      121      129 2022-07-23 11:01:11.000000 songbird_py-0.1.7/docs/exceptions.rst
--rw-r--r--   0     1001      121     7545 2022-07-23 11:01:11.000000 songbird_py-0.1.7/docs/extensions/autotypehint.py
--rw-r--r--   0     1001      121     1294 2022-07-23 11:01:11.000000 songbird_py-0.1.7/docs/extensions/docstrings.py
--rw-r--r--   0     1001      121      229 2022-07-23 11:01:11.000000 songbird_py-0.1.7/docs/hikari.rst
--rw-r--r--   0     1001      121      734 2022-07-23 11:01:11.000000 songbird_py-0.1.7/docs/index.rst
--rw-r--r--   0     1001      121      800 2022-07-23 11:01:11.000000 songbird_py-0.1.7/docs/make.bat
--rw-r--r--   0     1001      121      220 2022-07-23 11:01:11.000000 songbird_py-0.1.7/docs/pincer.rst
--rw-r--r--   0     1001      121      343 2022-07-23 11:01:11.000000 songbird_py-0.1.7/docs/queue.rst
--rw-r--r--   0     1001      121       43 2022-07-23 11:01:11.000000 songbird_py-0.1.7/docs/requirements.txt
--rw-r--r--   0     1001      121    75078 2022-07-23 11:01:11.000000 songbird_py-0.1.7/docs/songbird.png
--rw-r--r--   0     1001      121      141 2022-07-23 11:01:11.000000 songbird_py-0.1.7/docs/songbird.rst
--rw-r--r--   0     1001      121      183 2022-07-23 11:01:11.000000 songbird_py-0.1.7/examples/README.md
--rw-r--r--   0     1001      121      517 2022-07-23 11:01:11.000000 songbird_py-0.1.7/examples/hikari.py
--rw-r--r--   0     1001      121     3297 2022-07-23 11:01:11.000000 songbird_py-0.1.7/examples/pincer.py
--rw-r--r--   0     1001      121      867 2022-07-23 11:01:11.000000 songbird_py-0.1.7/pyproject.toml
--rw-r--r--   0     1001      121       17 2022-07-23 11:01:11.000000 songbird_py-0.1.7/requirements.txt
--rw-r--r--   0     1001      121       78 2022-07-23 11:01:11.000000 songbird_py-0.1.7/requirements_dev.txt
--rw-r--r--   0     1001      121     1197 2022-07-23 11:01:11.000000 songbird_py-0.1.7/setup.py
--rw-r--r--   0     1001      121      189 2022-07-23 11:01:11.000000 songbird_py-0.1.7/songbird/__init__.py
--rw-r--r--   0     1001      121      368 2022-07-23 11:01:11.000000 songbird_py-0.1.7/songbird/exceptions.py
--rw-r--r--   0     1001      121      485 2022-07-23 11:01:11.000000 songbird_py-0.1.7/songbird/helpers.py
--rw-r--r--   0     1001      121     3438 2022-07-23 11:01:11.000000 songbird_py-0.1.7/songbird/hikari.py
--rw-r--r--   0     1001      121     1927 2022-07-23 11:01:11.000000 songbird_py-0.1.7/songbird/pincer.py
--rw-r--r--   0     1001      121     1095 2022-07-23 11:01:11.000000 songbird_py-0.1.7/songbird/playlist.py
--rw-r--r--   0     1001      121        0 2022-07-23 11:01:11.000000 songbird_py-0.1.7/songbird/py.typed
--rw-r--r--   0     1001      121     4856 2022-07-23 11:01:11.000000 songbird_py-0.1.7/songbird/queue.py
--rw-r--r--   0     1001      121     8888 2022-07-23 11:01:11.000000 songbird_py-0.1.7/songbird/songbird.pyi
--rw-r--r--   0     1001      121     1773 2022-07-23 11:01:11.000000 songbird_py-0.1.7/songbird/voicebox_base.py
--rw-r--r--   0     1001      121     6440 2022-07-23 11:01:11.000000 songbird_py-0.1.7/src/config.rs
--rw-r--r--   0     1001      121    10719 2022-07-23 11:01:11.000000 songbird_py-0.1.7/src/driver.rs
--rw-r--r--   0     1001      121    20717 2022-07-23 11:01:11.000000 songbird_py-0.1.7/src/event.rs
--rw-r--r--   0     1001      121      572 2022-07-23 11:01:11.000000 songbird_py-0.1.7/src/exceptions.rs
--rw-r--r--   0     1001      121     2340 2022-07-23 11:01:11.000000 songbird_py-0.1.7/src/lib.rs
--rw-r--r--   0     1001      121     5253 2022-07-23 11:01:11.000000 songbird_py-0.1.7/src/source.rs
--rw-r--r--   0     1001      121     7159 2022-07-23 11:01:11.000000 songbird_py-0.1.7/src/track.rs
--rw-r--r--   0     1001      121     9188 2022-07-23 11:01:11.000000 songbird_py-0.1.7/src/track_handle.rs
--rw-r--r--   0     1001      121      381 2022-07-23 11:01:11.000000 songbird_py-0.1.7/src/utils.rs
--rw-r--r--   0     1001      121     8888 2022-07-23 11:01:11.000000 songbird_py-0.1.7/songbird/songbird.pyi
--rw-r--r--   0        0        0     3663 1970-01-01 00:00:00.000000 songbird_py-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 songbird_py-0.1.9/Cargo.toml
+-rw-r--r--   0     1001      123     3801 2023-04-14 19:22:27.000000 songbird_py-0.1.9/.github/workflows/publish.yml
+-rw-r--r--   0     1001      123      304 2023-04-14 19:22:27.000000 songbird_py-0.1.9/.gitignore
+-rw-r--r--   0     1001      123      331 2023-04-14 19:22:27.000000 songbird_py-0.1.9/.readthedocs.yaml
+-rw-r--r--   0     1001      123    18092 2023-04-14 19:22:27.000000 songbird_py-0.1.9/LICENSE
+-rw-r--r--   0     1001      123       43 2023-04-14 19:22:27.000000 songbird_py-0.1.9/MANIFEST.in
+-rw-r--r--   0     1001      123     2879 2023-04-14 19:22:27.000000 songbird_py-0.1.9/README.md
+-rw-r--r--   0     1001      123      634 2023-04-14 19:22:27.000000 songbird_py-0.1.9/docs/Makefile
+-rw-r--r--   0     1001      123     4618 2023-04-14 19:22:27.000000 songbird_py-0.1.9/docs/conf.py
+-rw-r--r--   0     1001      123      129 2023-04-14 19:22:27.000000 songbird_py-0.1.9/docs/exceptions.rst
+-rw-r--r--   0     1001      123     7545 2023-04-14 19:22:27.000000 songbird_py-0.1.9/docs/extensions/autotypehint.py
+-rw-r--r--   0     1001      123     1294 2023-04-14 19:22:27.000000 songbird_py-0.1.9/docs/extensions/docstrings.py
+-rw-r--r--   0     1001      123      229 2023-04-14 19:22:27.000000 songbird_py-0.1.9/docs/hikari.rst
+-rw-r--r--   0     1001      123      734 2023-04-14 19:22:27.000000 songbird_py-0.1.9/docs/index.rst
+-rw-r--r--   0     1001      123      800 2023-04-14 19:22:27.000000 songbird_py-0.1.9/docs/make.bat
+-rw-r--r--   0     1001      123      220 2023-04-14 19:22:27.000000 songbird_py-0.1.9/docs/pincer.rst
+-rw-r--r--   0     1001      123      343 2023-04-14 19:22:27.000000 songbird_py-0.1.9/docs/queue.rst
+-rw-r--r--   0     1001      123       43 2023-04-14 19:22:27.000000 songbird_py-0.1.9/docs/requirements.txt
+-rw-r--r--   0     1001      123    75078 2023-04-14 19:22:27.000000 songbird_py-0.1.9/docs/songbird.png
+-rw-r--r--   0     1001      123      141 2023-04-14 19:22:27.000000 songbird_py-0.1.9/docs/songbird.rst
+-rw-r--r--   0     1001      123      183 2023-04-14 19:22:27.000000 songbird_py-0.1.9/examples/README.md
+-rw-r--r--   0     1001      123      533 2023-04-14 19:22:27.000000 songbird_py-0.1.9/examples/hikari.py
+-rw-r--r--   0     1001      123     3297 2023-04-14 19:22:27.000000 songbird_py-0.1.9/examples/pincer.py
+-rw-r--r--   0     1001      123     1237 2023-04-14 19:22:27.000000 songbird_py-0.1.9/examples/seeking.py
+-rw-r--r--   0     1001      123      866 2023-04-14 19:22:27.000000 songbird_py-0.1.9/pyproject.toml
+-rw-r--r--   0     1001      123       17 2023-04-14 19:22:27.000000 songbird_py-0.1.9/requirements.txt
+-rw-r--r--   0     1001      123       78 2023-04-14 19:22:27.000000 songbird_py-0.1.9/requirements_dev.txt
+-rw-r--r--   0     1001      123     1197 2023-04-14 19:22:27.000000 songbird_py-0.1.9/setup.py
+-rw-r--r--   0     1001      123      189 2023-04-14 19:22:27.000000 songbird_py-0.1.9/songbird/__init__.py
+-rw-r--r--   0     1001      123      368 2023-04-14 19:22:27.000000 songbird_py-0.1.9/songbird/exceptions.py
+-rw-r--r--   0     1001      123      485 2023-04-14 19:22:27.000000 songbird_py-0.1.9/songbird/helpers.py
+-rw-r--r--   0     1001      123     3438 2023-04-14 19:22:27.000000 songbird_py-0.1.9/songbird/hikari.py
+-rw-r--r--   0     1001      123     1927 2023-04-14 19:22:27.000000 songbird_py-0.1.9/songbird/pincer.py
+-rw-r--r--   0     1001      123     1095 2023-04-14 19:22:27.000000 songbird_py-0.1.9/songbird/playlist.py
+-rw-r--r--   0     1001      123        0 2023-04-14 19:22:27.000000 songbird_py-0.1.9/songbird/py.typed
+-rw-r--r--   0     1001      123     4856 2023-04-14 19:22:27.000000 songbird_py-0.1.9/songbird/queue.py
+-rw-r--r--   0     1001      123     9440 2023-04-14 19:22:27.000000 songbird_py-0.1.9/songbird/songbird.pyi
+-rw-r--r--   0     1001      123     1773 2023-04-14 19:22:27.000000 songbird_py-0.1.9/songbird/voicebox_base.py
+-rw-r--r--   0     1001      123     6941 2023-04-14 19:22:27.000000 songbird_py-0.1.9/src/config.rs
+-rw-r--r--   0     1001      123    10719 2023-04-14 19:22:27.000000 songbird_py-0.1.9/src/driver.rs
+-rw-r--r--   0     1001      123    20717 2023-04-14 19:22:27.000000 songbird_py-0.1.9/src/event.rs
+-rw-r--r--   0     1001      123      638 2023-04-14 19:22:27.000000 songbird_py-0.1.9/src/exceptions.rs
+-rw-r--r--   0     1001      123     2500 2023-04-14 19:22:27.000000 songbird_py-0.1.9/src/lib.rs
+-rw-r--r--   0     1001      123     4071 2023-04-14 19:22:27.000000 songbird_py-0.1.9/src/seekable.rs
+-rw-r--r--   0     1001      123     5323 2023-04-14 19:22:27.000000 songbird_py-0.1.9/src/source.rs
+-rw-r--r--   0     1001      123     7159 2023-04-14 19:22:27.000000 songbird_py-0.1.9/src/track.rs
+-rw-r--r--   0     1001      123     9075 2023-04-14 19:22:27.000000 songbird_py-0.1.9/src/track_handle.rs
+-rw-r--r--   0     1001      123      381 2023-04-14 19:22:27.000000 songbird_py-0.1.9/src/utils.rs
+-rw-r--r--   0     1001      123    51292 2023-04-14 19:22:27.000000 songbird_py-0.1.9/Cargo.lock
+-rw-r--r--   0        0        0     3785 1970-01-01 00:00:00.000000 songbird_py-0.1.9/PKG-INFO
```

### Comparing `songbird_py-0.1.7/Cargo.toml` & `songbird_py-0.1.9/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 [dependencies]
 tokio = { version = "1.20.0", features = ["sync"] }
 async-trait = "0.1.53"
 pyo3-log = "0.6.0"
 log = "0.4.17"
 
 [dependencies.songbird]
-version = "0.3.0"
+version = "0.3.2"
 features = ["driver", "yt-dlp"]
 
 [dependencies.pyo3]
 version = "0.16.4"
 features = ["extension-module"]
 
 [dependencies.pyo3-asyncio]
```

### Comparing `songbird_py-0.1.7/.github/workflows/publish.yml` & `songbird_py-0.1.9/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/LICENSE` & `songbird_py-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/README.md` & `songbird_py-0.1.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+> ⚠️ This library is on lifeline support and I am looking for a new maintainer. Please DM me if you
+> are interested.
+
 # Songbird-Py
 Songbird bindings for python. The goal is to provide an easy to use alternitive to Lavalink.
 Its written with rust-bindings to [Songbird](https://github.com/serenity-rs/songbird).
 
 [Songbird-py Docs](https://songbird-py.readthedocs.io/en/latest/)
 
 ## Dependencies
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `songbird_py-0.1.7/docs/Makefile` & `songbird_py-0.1.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/docs/conf.py` & `songbird_py-0.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/docs/extensions/autotypehint.py` & `songbird_py-0.1.9/docs/extensions/autotypehint.py`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/docs/extensions/docstrings.py` & `songbird_py-0.1.9/docs/extensions/docstrings.py`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/docs/index.rst` & `songbird_py-0.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/docs/make.bat` & `songbird_py-0.1.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/docs/songbird.png` & `songbird_py-0.1.9/docs/songbird.png`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/examples/pincer.py` & `songbird_py-0.1.9/examples/pincer.py`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/pyproject.toml` & `songbird_py-0.1.9/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 build-backend = "maturin"
 requires = ["maturin>=0.12,<0.13"]
 
 [project]
-version = "0.1.7"
+version = "0.1.9"
 description = "A Discord voice library using Python Songbird bindings."
 classifiers = [
   "Programming Language :: Rust",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
   "Operating System :: OS Independent",
@@ -19,11 +19,11 @@
 [project.optional-dependencies]
 hikari = ["hikari"]
 pincer = ["pincer"]
 
 [project.urls]
 "Bug Tracker" = "https://github.com/Lunarmagpie/Songbird-Py/issues"
 Docs = "https://songbird-py.readthedocs.io/en/latest/"
-GitHub = "https://github.com/Lunarmagpie/Songbird-Py"
+GitHub = "https://github.com/magpie-dev/Songbird-Py"
 
 [tool.maturin]
 sdist-include = ["songbird/*.pyi"]
```

### Comparing `songbird_py-0.1.7/setup.py` & `songbird_py-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/songbird/hikari.py` & `songbird_py-0.1.9/songbird/hikari.py`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/songbird/pincer.py` & `songbird_py-0.1.9/songbird/pincer.py`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/songbird/playlist.py` & `songbird_py-0.1.9/songbird/playlist.py`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/songbird/queue.py` & `songbird_py-0.1.9/songbird/queue.py`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/songbird/songbird.pyi` & `songbird_py-0.1.9/songbird/songbird.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -64,18 +64,29 @@
     @staticmethod
     async def ffmpeg(filename: str, pre_input_args=None,
                      args=None) -> Source: ...
 
     @staticmethod
     async def ytdl(url: str) -> Source: ...
     @staticmethod
-    def file(url: str) -> Source: ...
+    def file(filename: str) -> Source: ...
     async def metadata(self) -> Metadata: ...
     async def stereo(self) -> bool: ...
 
+class RestartableSource:
+    def into_source(self) -> Source: ...
+    @classmethod
+    async def ytdl(cls, url: str, lazy: bool) -> RestartableSource: ...
+    @classmethod
+    async def ffmpeg(cls, filename: str, lazy: bool) -> RestartableSource: ...
+
+class CompressedSource:
+    def into_source(self) -> Source: ...
+    @classmethod
+    async def from_source(cls, input: Source, bitrate: Bitrate) -> CompressedSource: ...
 
 class CryptoMode:
     Normal: CryptoMode
     Suffix: CryptoMode
     Lite: CryptoMode
 
 
@@ -361,7 +372,13 @@
     Illegal_2: RtpType
     Illegal_3: RtpType
     Illegal_4: RtpType
     Illegal_5: RtpType
     Illegal_6: RtpType
     Illegal_7: RtpType
     Illegal_8: RtpType
+
+class Bitrate:
+    AUTO: Bitrate
+    MAX: Bitrate
+    @classmethod
+    def bits_per_second(cls, bits: int) -> Bitrate: ...
```

### Comparing `songbird_py-0.1.7/songbird/voicebox_base.py` & `songbird_py-0.1.9/songbird/voicebox_base.py`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/src/config.rs` & `songbird_py-0.1.9/src/config.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::time::Duration;
 
 use pyo3::prelude::*;
 use songbird::driver::{
     retry::{ExponentialBackoff, Retry, Strategy},
-    CryptoMode, DecodeMode,
+    Bitrate, CryptoMode, DecodeMode,
 };
 use songbird::Config;
 
 use crate::utils::{unwrap_duration, unwrap_f64_to_duration};
 
 /// Variants of the XSalsa20Poly1305 encryption scheme.
 #[pyclass(name = "CryptoMode")]
@@ -116,19 +116,19 @@
     #[classattr]
     fn Decode() -> Self {
         Self::from(DecodeMode::Decode)
     }
 }
 
 /// Config objects are how you set a driver's configuration.
-/// 
+///
 /// .. note::
-/// 
+///
 ///     Changes in a Config object are only passed to the ``Driver`` with the ``set_config`` method.
-/// 
+///
 #[pyclass(name = "Config")]
 #[pyo3(text_signature = "(/)")]
 pub struct PyConfig {
     pub config: Config,
 }
 
 #[pymethods]
@@ -214,7 +214,35 @@
     /// Sets the timeout for joining a voice channel.
     #[pyo3(text_signature = "($self, crypto_mode: Optional[float])")]
     fn set_gateway_timeout(&mut self, gateway_timeout: Option<f64>) {
         let config = self.config.clone();
         self.config = config.gateway_timeout(unwrap_f64_to_duration(gateway_timeout))
     }
 }
+
+#[pyclass(name = "Bitrate")]
+pub struct PyBitrate {
+    pub bitrate: Bitrate
+}
+
+#[pymethods]
+#[allow(non_snake_case)]
+impl PyBitrate {
+    #[classattr]
+    fn AUTO() -> Self {
+        Self {
+            bitrate: Bitrate::Auto
+        }
+    }
+    #[classattr]
+    fn MAX() -> Self {
+        Self {
+            bitrate: Bitrate::Max
+        }
+    }
+    #[staticmethod]
+    fn bits_per_second(bits: i32) -> Self {
+        Self {
+            bitrate: Bitrate::BitsPerSecond(bits)
+        }
+    }
+}
```

### Comparing `songbird_py-0.1.7/src/driver.rs` & `songbird_py-0.1.9/src/driver.rs`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/src/event.rs` & `songbird_py-0.1.9/src/event.rs`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/src/exceptions.rs` & `songbird_py-0.1.9/src/exceptions.rs`

 * *Files 14% similar despite different names*

```diff
@@ -3,10 +3,11 @@
 // Base Exception for all songbird errors
 create_exception!(module, SongbirdError, pyo3::exceptions::PyException);
 
 create_exception!(module, UseAsyncConstructorError, SongbirdError);
 create_exception!(module, CouldNotConnectToRTPError, SongbirdError);
 create_exception!(module, ConsumedSourceError, SongbirdError);
 create_exception!(module, CouldNotOpenFileError, SongbirdError);
+create_exception!(module, CouldNotConstructError, SongbirdError);
 create_exception!(module, YtdlError, SongbirdError);
 create_exception!(module, FfmpegError, SongbirdError);
 create_exception!(module, TrackError, SongbirdError);
```

### Comparing `songbird_py-0.1.7/src/lib.rs` & `songbird_py-0.1.9/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -7,32 +7,36 @@
     SongbirdError, TrackError, UseAsyncConstructorError, YtdlError,
 };
 
 mod config;
 mod driver;
 mod event;
 mod source;
+mod seekable;
 mod track;
 mod track_handle;
 mod utils;
 
 /// The Songbird Python/Rust bindings
 /// This module is written in Rust 🚀
 #[pymodule]
 fn songbird(py: Python, m: &PyModule) -> PyResult<()> {
     let _ = Logger::new(py, Caching::LoggersAndLevels)?.install();
 
     m.add_class::<driver::PyDriver>()?;
     m.add_class::<source::PySource>()?;
+    m.add_class::<seekable::PyRestartableSource>()?;
+    m.add_class::<seekable::PyCompressedSource>()?;
 
     // Config
     m.add_class::<config::PyConfig>()?;
     m.add_class::<config::PyCryptoMode>()?;
     m.add_class::<config::PyDecodeMode>()?;
     m.add_class::<config::PyStrategy>()?;
+    m.add_class::<config::PyBitrate>()?;
 
     // Track_handler
     m.add_class::<track_handle::PyPlayMode>()?;
     m.add_class::<track_handle::PyTrackHandle>()?;
     m.add_class::<track_handle::PyTrackState>()?;
     m.add_class::<track_handle::PyLoopState>()?;
     m.add_class::<track_handle::PyMetadata>()?;
```

### Comparing `songbird_py-0.1.7/src/source.rs` & `songbird_py-0.1.9/src/source.rs`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     /// This method of creating inputs allows you to use an Input multiple times in
     /// Python, which is probably expected.
     pub source: Arc<Mutex<Option<Input>>>,
     consumed: bool,
 }
 
 impl PySource {
-    fn from(input: Input) -> Self {
+    pub fn from(input: Input) -> Self {
         Self {
             source: Arc::from(Mutex::from(Some(input))),
             consumed: false,
         }
     }
 
     pub fn raise_if_consumed(&mut self) -> Result<(), PyErr> {
@@ -63,14 +63,15 @@
 }
 
 #[pymethods]
 impl PySource {
     /// Use youtube dl to play a video from a URL
     ///
     /// Example
+    ///
     /// .. code-block:: python
     ///
     ///     await driver.play(Source.ytdl("https://www.youtube.com/watch?v=n5n7CSGPzqw"))
     #[staticmethod]
     fn ytdl<'p>(py: Python, url: String) -> PyResult<&PyAny> {
         pyo3_asyncio::tokio::future_into_py(py, async move {
             match songbird::ytdl(url).await {
@@ -126,15 +127,18 @@
         };
 
         pyo3_asyncio::tokio::future_into_py(py, async move {
             let pre_input_args: Vec<&str> = pre_input_args.iter().map(String::as_str).collect();
             let args: Vec<&str> = args.iter().map(String::as_str).collect();
 
             if !std::path::Path::new(&filepath).exists() {
-                return Err(builtins::FileNotFoundError::new_err(format!("File `{}` does not exist", filepath)));
+                return Err(builtins::FileNotFoundError::new_err(format!(
+                    "File `{}` does not exist",
+                    filepath
+                )));
             };
 
             match if pre_input_args.is_empty() && args.is_empty() {
                 songbird::ffmpeg(filepath).await
             } else {
                 songbird::input::ffmpeg_optioned(filepath, pre_input_args.as_ref(), args.as_ref())
                     .await
```

### Comparing `songbird_py-0.1.7/src/track.rs` & `songbird_py-0.1.9/src/track.rs`

 * *Files identical despite different names*

### Comparing `songbird_py-0.1.7/src/track_handle.rs` & `songbird_py-0.1.9/src/track_handle.rs`

 * *Files 2% similar despite different names*

```diff
@@ -260,16 +260,15 @@
         handle_track_result(self.track_handle.pause())
     }
     /// Sets the volume of the track.
     #[pyo3(text_signature = "($self, volume)")]
     fn set_volume(&self, volume: f32) -> PyResult<()> {
         handle_track_result(self.track_handle.set_volume(volume))
     }
-    /// Makes a lazily initialized track playable. This does not matter to the current
-    /// functionality of the lib because ``Restartable`` is not implemented.
+    /// Makes a lazily initialized track playable.
     #[pyo3(text_signature = "($self)")]
     fn make_playable(&self) -> PyResult<()> {
         handle_track_result(self.track_handle.make_playable())
     }
     #[getter]
     fn is_seekable(&self) -> bool {
         self.track_handle.is_seekable()
```

### Comparing `songbird_py-0.1.7/PKG-INFO` & `songbird_py-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 Metadata-Version: 2.1
 Name: songbird-py
-Version: 0.1.7
+Version: 0.1.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
 Requires-Dist: yt-dlp>=2021.12.1
-Requires-Dist: pincer; extra == 'pincer'
 Requires-Dist: hikari; extra == 'hikari'
-Provides-Extra: pincer
+Requires-Dist: pincer; extra == 'pincer'
 Provides-Extra: hikari
+Provides-Extra: pincer
 License-File: LICENSE
 Summary: A Discord voice library using Python Songbird bindings.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Docs, https://songbird-py.readthedocs.io/en/latest/
-Project-URL: GitHub, https://github.com/Lunarmagpie/Songbird-Py
 Project-URL: Bug Tracker, https://github.com/Lunarmagpie/Songbird-Py/issues
+Project-URL: Docs, https://songbird-py.readthedocs.io/en/latest/
+Project-URL: GitHub, https://github.com/magpie-dev/Songbird-Py
+
+> ⚠️ This library is on lifeline support and I am looking for a new maintainer. Please DM me if you
+> are interested.
 
 # Songbird-Py
 Songbird bindings for python. The goal is to provide an easy to use alternitive to Lavalink.
 Its written with rust-bindings to [Songbird](https://github.com/serenity-rs/songbird).
 
 [Songbird-py Docs](https://songbird-py.readthedocs.io/en/latest/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

