# Comparing `tmp/whisper-ctranslate2-0.1.7.tar.gz` & `tmp/whisper-ctranslate2-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whisper-ctranslate2-0.1.7.tar", last modified: Wed Apr 12 17:51:16 2023, max compression
+gzip compressed data, was "whisper-ctranslate2-0.1.8.tar", last modified: Fri Apr 14 15:18:48 2023, max compression
```

## Comparing `whisper-ctranslate2-0.1.7.tar` & `whisper-ctranslate2-0.1.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 17:51:16.823864 whisper-ctranslate2-0.1.7/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.1.7/LICENSE
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4209 2023-04-12 17:51:16.823864 whisper-ctranslate2-0.1.7/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     3558 2023-04-12 17:25:24.000000 whisper-ctranslate2-0.1.7/README.md
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-12 17:51:16.823864 whisper-ctranslate2-0.1.7/setup.cfg
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     1499 2023-04-12 16:34:42.000000 whisper-ctranslate2-0.1.7/setup.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 17:51:16.823864 whisper-ctranslate2-0.1.7/src/
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 17:51:16.823864 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/languages.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4310 2023-04-12 17:25:24.000000 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/live.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4674 2023-04-10 14:05:51.000000 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/models.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5319 2023-04-12 17:25:24.000000 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/transcribe.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-04-10 14:05:51.000000 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/version.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)    12169 2023-04-12 17:25:24.000000 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/whisper_ctranslate2.py
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     5527 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/writers.py
-drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-12 17:51:16.823864 whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/
--rw-rw-r--   0 jordi     (1000) jordi     (1000)     4209 2023-04-12 17:51:16.000000 whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/PKG-INFO
--rw-rw-r--   0 jordi     (1000) jordi     (1000)      554 2023-04-12 17:51:16.000000 whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/SOURCES.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-12 17:51:16.000000 whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/dependency_links.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-12 17:51:16.000000 whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/entry_points.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       98 2023-04-12 17:51:16.000000 whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/requires.txt
--rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-12 17:51:16.000000 whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/top_level.txt
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-14 15:18:48.537725 whisper-ctranslate2-0.1.8/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1066 2023-03-17 10:20:50.000000 whisper-ctranslate2-0.1.8/LICENSE
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4209 2023-04-14 15:18:48.537725 whisper-ctranslate2-0.1.8/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     3558 2023-04-12 17:25:24.000000 whisper-ctranslate2-0.1.8/README.md
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       94 2023-04-14 15:18:48.537725 whisper-ctranslate2-0.1.8/setup.cfg
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     1499 2023-04-14 14:47:47.000000 whisper-ctranslate2-0.1.8/setup.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-14 15:18:48.533725 whisper-ctranslate2-0.1.8/src/
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-14 15:18:48.533725 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     2846 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/languages.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4620 2023-04-14 12:45:32.000000 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/live.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4674 2023-04-10 14:05:51.000000 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/models.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     6124 2023-04-14 14:47:43.000000 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/transcribe.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       22 2023-04-12 17:52:10.000000 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/version.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)    13134 2023-04-14 14:38:43.000000 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/whisper_ctranslate2.py
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     5527 2023-04-03 16:36:09.000000 whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/writers.py
+drwxrwxr-x   0 jordi     (1000) jordi     (1000)        0 2023-04-14 15:18:48.533725 whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)     4209 2023-04-14 15:18:48.000000 whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/PKG-INFO
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)      554 2023-04-14 15:18:48.000000 whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)        1 2023-04-14 15:18:48.000000 whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       90 2023-04-14 15:18:48.000000 whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/entry_points.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       98 2023-04-14 15:18:48.000000 whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/requires.txt
+-rw-rw-r--   0 jordi     (1000) jordi     (1000)       24 2023-04-14 15:18:48.000000 whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/top_level.txt
```

### Comparing `whisper-ctranslate2-0.1.7/LICENSE` & `whisper-ctranslate2-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.7/PKG-INFO` & `whisper-ctranslate2-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.1.7
+Version: 0.1.8
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/jordimas/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `whisper-ctranslate2-0.1.7/README.md` & `whisper-ctranslate2-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.7/setup.py` & `whisper-ctranslate2-0.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/languages.py` & `whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/languages.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/live.py` & `whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/live.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 # Based on code from https://github.com/Nikorasu/LiveWhisper/blob/main/livewhisper.py
 
 import numpy as np
-import sounddevice as sd
 from .transcribe import Transcribe, TranscriptionOptions
 from typing import Union, List
 
 SampleRate = 16000  # Stream device recording frequency per second
 BlockSize = 30  # Block size in milliseconds
 Threshold = 0.2  # Minimum volume threshold to activate listening
 Vocals = [50, 1000]  # Frequency range to detect sounds that could be speech
 EndBlocks = 33 * 2  # Number of blocks to wait before sending (30 ms is block)
 FlushBlocks = 33 * 10  # Number of blocks to wait before sending
 
+try:
+    import sounddevice as sd
+
+    sounddevice_available = True
+
+except Exception as e:
+    sounddevice_available = False
+    sounddevice_exception = e
+
 
 class Live:
     def __init__(
         self,
         model_path: str,
         task: str,
         language: str,
@@ -39,14 +47,22 @@
         self.running = True
         self.waiting = 0
         self.prevblock = self.buffer = np.zeros((0, 1))
         self.speaking = False
         self.blocks_speaking = 0
         self.buffers_to_process = []
 
+    @staticmethod
+    def is_available():
+        return sounddevice_available
+
+    @staticmethod
+    def force_not_available_exception():
+        raise (sounddevice_exception)
+
     def _is_there_voice(self, indata, frames):
         freq = np.argmax(np.abs(np.fft.rfft(indata[:, 0]))) * SampleRate / frames
         volume = np.sqrt(np.mean(indata**2))
 
         return volume > Threshold and Vocals[0] <= freq <= Vocals[1]
 
     def _save_to_process(self):
```

### Comparing `whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/models.py` & `whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/models.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/transcribe.py` & `whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/transcribe.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,17 @@
     #    without_timestamps: bool
     #    max_initial_timestamp: float
     word_timestamps: bool
     print_colors: bool
     prepend_punctuations: str
     append_punctuations: str
     vad_filter: bool
+    vad_threshold: Optional[float]
+    vad_min_speech_duration_ms: Optional[int]
+    vad_max_speech_duration_s: Optional[int]
     vad_min_silence_duration_ms: Optional[int]
 
 
 class Transcribe:
     def _get_colored_text(self, words):
         k_colors = [
             "\033[38;5;196m",
@@ -67,14 +70,35 @@
             p = word.probability
             col = max(0, min(n_colors - 1, (int)(pow(p, 3) * n_colors)))
             end_mark = "\033[0m"
             text_words += f"{k_colors[col]}{word.word}{end_mark}"
 
         return text_words
 
+    def _get_vad_parameters_dictionary(self, options):
+        vad_parameters = {}
+
+        if options.vad_threshold:
+            vad_parameters["threshold"] = options.vad_threshold
+
+        if options.vad_min_speech_duration_ms:
+            vad_parameters[
+                "min_speech_duration_ms"
+            ] = options.vad_min_speech_duration_ms
+
+        if options.vad_max_speech_duration_s:
+            vad_parameters["max_speech_duration_s"] = options.vad_max_speech_duration_s
+
+        if options.vad_min_silence_duration_ms:
+            vad_parameters[
+                "min_silence_duration_ms"
+            ] = options.vad_min_silence_duration_ms
+
+        return vad_parameters
+
     def inference(
         self,
         audio: Union[str, BinaryIO, np.ndarray],
         model_path: str,
         task: str,
         language: str,
         threads: int,
@@ -89,14 +113,16 @@
             model_path,
             device=device,
             device_index=device_index,
             compute_type=compute_type,
             cpu_threads=threads,
         )
 
+        vad_parameters = self._get_vad_parameters_dictionary(options)
+
         segments, info = model.transcribe(
             audio=audio,
             language=language,
             task=task,
             beam_size=options.beam_size,
             best_of=options.best_of,
             patience=options.patience,
@@ -108,17 +134,15 @@
             condition_on_previous_text=options.condition_on_previous_text,
             initial_prompt=options.initial_prompt,
             suppress_tokens=options.suppress_tokens,
             word_timestamps=True if options.print_colors else options.word_timestamps,
             prepend_punctuations=options.prepend_punctuations,
             append_punctuations=options.append_punctuations,
             vad_filter=options.vad_filter,
-            vad_parameters={
-                "min_silence_duration_ms": options.vad_min_silence_duration_ms
-            },
+            vad_parameters=vad_parameters,
         )
 
         language_name = LANGUAGES[info.language].title()
         if not live:
             print(
                 "Detected language '%s' with probability %f"
                 % (language_name, info.language_probability)
```

### Comparing `whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/whisper_ctranslate2.py` & `whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/whisper_ctranslate2.py`

 * *Files 4% similar despite different names*

```diff
@@ -192,18 +192,39 @@
         "--vad_filter",
         type=bool,
         default=False,
         help="Enable the voice activity detection (VAD) to filter out parts of the audio without speech. This step is using the Silero VAD model https://github.com/snakers4/silero-vad.",
     )
 
     parser.add_argument(
+        "--vad_threshold",
+        type=float,
+        default=None,
+        help="When `vad_filter` is enabled, probabilities above this value are considered as speech.",
+    )
+
+    parser.add_argument(
+        "--vad_min_speech_duration_ms",
+        type=int,
+        default=None,
+        help="When `vad_filter` is enabled, final speech chunks shorter min_speech_duration_ms are thrown out.",
+    )
+
+    parser.add_argument(
+        "--vad_max_speech_duration_s",
+        type=int,
+        default=None,
+        help="When `vad_filter` is enabled, Maximum duration of speech chunks in seconds. Longer will be split at the timestamp of the last silence.",
+    )
+
+    parser.add_argument(
         "--vad_min_silence_duration_ms",
         type=int,
-        default=2000,
-        help="When `vad_filter` is enabled, audio segments without speech for at least this number of milliseconds will be ignored.",
+        default=None,
+        help="When `vad_filter` is enabled, in the end of each speech chunk time to wait before separating it.",
     )
 
     # CTranslate2 specific parameters
     parser.add_argument(
         "--device_index",
         nargs="*",
         type=int,
@@ -306,20 +327,26 @@
         initial_prompt=args.pop("initial_prompt"),
         suppress_tokens=suppress_tokens,
         word_timestamps=args.pop("word_timestamps"),
         prepend_punctuations=args.pop("prepend_punctuations"),
         append_punctuations=args.pop("append_punctuations"),
         print_colors=args.pop("print_colors"),
         vad_filter=args.pop("vad_filter"),
+        vad_threshold=args.pop("vad_threshold"),
+        vad_min_speech_duration_ms=args.pop("vad_min_speech_duration_ms"),
+        vad_max_speech_duration_s=args.pop("vad_max_speech_duration_s"),
         vad_min_silence_duration_ms=args.pop("vad_min_silence_duration_ms"),
     )
 
     if not verbose and options.print_colors:
         raise RuntimeError("You cannot disable verbose and enable print colors")
 
+    if live_transcribe and not Live.is_available():
+        Live.force_not_available_exception()
+
     if verbose and not language:
         print(
             "Detecting language using up to the first 30 seconds. Use `--language` to specify the language"
         )
 
     if options.print_colors and output_dir and not options.word_timestamps:
         print(
```

### Comparing `whisper-ctranslate2-0.1.7/src/whisper_ctranslate2/writers.py` & `whisper-ctranslate2-0.1.8/src/whisper_ctranslate2/writers.py`

 * *Files identical despite different names*

### Comparing `whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/PKG-INFO` & `whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whisper-ctranslate2
-Version: 0.1.7
+Version: 0.1.8
 Summary: Whisper command line client that uses CTranslate2
 Home-page: https://github.com/jordimas/whisper-ctranslate2
 Author: Jordi Mas
 Author-email: jmas@softcatala.org
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `whisper-ctranslate2-0.1.7/whisper_ctranslate2.egg-info/SOURCES.txt` & `whisper-ctranslate2-0.1.8/whisper_ctranslate2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

