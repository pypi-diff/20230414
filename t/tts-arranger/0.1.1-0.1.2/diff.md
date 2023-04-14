# Comparing `tmp/tts_arranger-0.1.1.tar.gz` & `tmp/tts_arranger-0.1.2.tar.gz`

## Comparing `tts_arranger-0.1.1.tar` & `tts_arranger-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/requirements.txt
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0    26358 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/tts_processor.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/tts_processor_example.py
--rw-r--r--   0        0        0     4502 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/tts_simple_writer.py
--rw-r--r--   0        0        0    15087 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/tts_writer.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/data/replace.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/data/replace_de.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/data/replace_en.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/items/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/items/tts_chapter.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/items/tts_item.py
--rw-r--r--   0        0        0     5142 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/items/tts_project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0     1272 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/utils/audio.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0    16954 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/LICENSE
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/README.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 tts_arranger-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/requirements.txt
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0    26369 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/tts_processor.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/tts_processor_example.py
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/tts_simple_writer.py
+-rw-r--r--   0        0        0    15112 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/tts_writer.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/data/replace.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/data/replace_de.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/data/replace_en.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/items/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/items/tts_chapter.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/items/tts_item.py
+-rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/items/tts_project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/utils/audio.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0    18265 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/README.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/PKG-INFO
```

### Comparing `tts_arranger-0.1.1/src/tts_arranger/tts_processor.py` & `tts_arranger-0.1.2/src/tts_arranger/tts_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -503,59 +503,56 @@
         merged_items = self._merge_similar_items(tts_items)
 
         for tts_item in merged_items:
             final_items += self._prepare_item(tts_item)
 
         return final_items
 
-    def _merge_similar_items(self, items=[]) -> list:
+    def _merge_similar_items(self, items: list[TTS_Item]) -> list[TTS_Item]:
         """
         Merge similar items for smoother synthesizing and avoiding unwanted pauses
 
         :param items: A list of TTS items to merge
         :type items: list
 
         :return: A list of merged TTS items
-        :rtype: list
+        :rtype: list[TTS_Item]
         """
+
         final_items: list[TTS_Item] = []
+        merged_item: Optional[TTS_Item] = None
 
         if items:
-            start_item = -1
-            merged_item = TTS_Item()
-
-            for i, item in enumerate(items):
-                if start_item < 0:
+            for item in items:
+                if not merged_item:
                     # Scanning not started
-                    start_item = i
                     merged_item = item
-                else:
-                    # Scanning started
-                    if merged_item.speaker == item.speaker and merged_item.speaker_idx == item.speaker_idx:
-                        # Starting item and current are similar, add to merge item text and length
-                        if merged_item.text and item.text:
-                            merged_item.text += ' ' + item.text
-                        merged_item.length += item.length
-                    else:
-                        # Starting item and current are not similar, add last and current item, set this item as new starting item
-                        if final_items:
-                            if final_items[-1] != merged_item:
-                                final_items.append(merged_item)
-                        else:
-                            final_items.append(merged_item)
-                        final_items.append(item)
-                        merged_item = item
-                        start_item = i
-
-                if i == len(items) - 1:
-                    if final_items:
-                        if final_items[-1] != merged_item:
-                            final_items.append(merged_item)
+                elif merged_item.speaker == item.speaker and merged_item.speaker_idx == item.speaker_idx:
+                    # Starting item and current are similar, add to merge item text and length
+                    if merged_item.text and item.text:
+                        merged_item = merged_item.__class__(
+                            text=f'{merged_item.text.strip()} {item.text.strip()}',
+                            speaker=merged_item.speaker,
+                            speaker_idx=merged_item.speaker_idx,
+                            length=merged_item.length + item.length
+                        )
                     else:
-                        final_items.append(merged_item)
+                        merged_item = merged_item.__class__(
+                            text=f'{merged_item.text}{item.text}',
+                            speaker=merged_item.speaker,
+                            speaker_idx=merged_item.speaker_idx,
+                            length=merged_item.length + item.length
+                        )
+                else:
+                    # Starting item and current are not similar, add last and current item, set this item as new starting item
+                    final_items.append(merged_item)
+                    merged_item = item
+
+            if merged_item is not None:
+                final_items.append(merged_item)
 
         return final_items
 
     def synthesize_tts_item(self, tts_item: TTS_Item) -> AudioSegment:
         """
         Synthesize a single item and return a PyDub AudioSegment object
```

### Comparing `tts_arranger-0.1.1/src/tts_arranger/tts_processor_example.py` & `tts_arranger-0.1.2/src/tts_arranger/tts_processor_example.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.1/src/tts_arranger/tts_simple_writer.py` & `tts_arranger-0.1.2/src/tts_arranger/tts_simple_writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             except Exception as e:
                 # with open(self.temp_dir.name + '/tts-error.log', 'a+') as f:
                 #     f.write(f'Error synthesizing "{output_filename}"\n')
                 log(LOG_TYPE.ERROR, f'Error synthesizing "{output_filename}": {e}')
                 sys.exit()
 
         self._write(segments, output_filename)
-        log(LOG_TYPE.SUCCESS, f'Synthesizing finished, file saved under {output_filename}.')
+        log(LOG_TYPE.SUCCESS, f'Synthesizing finished, file saved as {output_filename}')
 
     def _write(self, segment: AudioSegment, output_filename: str) -> None:
         """
         Compress, convert and write AudioSegment as a given output file path and name
 
         :param segment: AudioSegment to be written
         :type segment: AudioSegment
```

### Comparing `tts_arranger-0.1.1/src/tts_arranger/tts_writer.py` & `tts_arranger-0.1.2/src/tts_arranger/tts_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         cumulative_time = 0
 
         for i, chapter in enumerate(chapters):
             audio = AudioSegment.empty()
 
             temp_format = 'wav'
 
-            filename = temp_dir + '/' + f'tts_part_{i}.{temp_format}'
+            filename = os.path.join(temp_dir, f'tts_part_{i}.{temp_format}')
 
             log(LOG_TYPE.INFO, f'Synthesizing chapter {i + 1} of {len(chapters)}')
 
             for j, tts_item in enumerate(chapter.tts_items):
                 if tts_item.text:
                     log(LOG_TYPE.INFO, f'Synthesizing item {j + 1} of {len(chapter.tts_items)} ("{tts_item.speaker}", {tts_item.speaker_idx}, {tts_item.length}ms):{bcolors.ENDC} {tts_item.text}')
                 else:
@@ -126,15 +126,15 @@
             current_total_items += len(chapter.tts_items)
 
             self._write_temp_audio(audio, filename)
 
             num_zeros = len(str(len(self.temp_files)))
             chapter_title = f'{i + 1:0{num_zeros}} - {chapter.title}'
 
-            filename_out = temp_dir + '/' + f'tts_part_{i}.{temp_format}'
+            filename_out = os.path.join(temp_dir, f'tts_part_{i}.{temp_format}')
 
             # Add temp files for concatenating later
             self.temp_files.append((chapter_title, filename_out))
 
             chapter.start_time = cumulative_time
             chapter.end_time = cumulative_time + self._get_nanoseconds_for_file(filename)
             cumulative_time = chapter.end_time
@@ -186,15 +186,15 @@
         :raises: ValueError if the provided `image` is not a PIL Image instance, or if either `input_file` or `output_file` are not valid file paths.
         """
 
         image_width, image_height = image.size
 
         with tempfile.TemporaryDirectory() as temp_dir:
             audio = ffmpeg.input(input_file)['a']
-            image_path = temp_dir + '/tts_image.jpeg'
+            image_path = os.path.join(temp_dir, 'tts_image.jpeg')
 
             # Fix for ffmpeg problem when image size is not divisible by 2
             image.crop((0, 0, math.ceil(image_width/2)*2, math.ceil(image_height/2)*2)).save(image_path)
 
             cover = ffmpeg.input(image_path)['v']
 
             (
@@ -320,15 +320,15 @@
 
                     # Remove last map parameter (workaround for ffmpeg-python bug)
                     cmd = self._remove_last_arg(cmd, '-map')
 
                     subprocess.call(cmd)
 
                     output_files.append(output_path)
-                    log(LOG_TYPE.SUCCESS, f'Synthesizing project {self.project.title} finished, file saved as {output_path}.')
+                    log(LOG_TYPE.SUCCESS, f'Synthesizing project {self.project.title} finished, file saved as {output_path}')
                 else:
                     # Don’t concatenate, convert the chapter temp files to the target format
                     os.makedirs(output_filename, exist_ok=True)
 
                     for name, file in self.temp_files:
                         output_chapter_filename = os.path.join(output_filename, name + output_extension)
 
@@ -342,15 +342,15 @@
                             ffmpeg
                             .input(file)
                             .output(output_chapter_filename, **output_args, loglevel='error')
                             .run(overwrite_output=True)
                         )
 
                         output_files.append(output_chapter_filename)
-                    log(LOG_TYPE.SUCCESS, f'Synthesizing project {self.project.title} finished, chapter files saved under {output_filename}.')
+                    log(LOG_TYPE.SUCCESS, f'Synthesizing project {self.project.title} finished, chapter files saved under {output_filename}/')
 
                 if self.project.image_bytes:
                     if self.output_format in ['m4b', 'm4a', 'mp3']:
                         image_bytes = base64.b64decode(self.project.image_bytes)
                         image_file = io.BytesIO(image_bytes)
                         image = Image.open(image_file)
```

### Comparing `tts_arranger-0.1.1/src/tts_arranger/items/tts_chapter.py` & `tts_arranger-0.1.2/src/tts_arranger/items/tts_chapter.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.1/src/tts_arranger/items/tts_item.py` & `tts_arranger-0.1.2/src/tts_arranger/items/tts_item.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.1/src/tts_arranger/items/tts_project.py` & `tts_arranger-0.1.2/src/tts_arranger/items/tts_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import datetime
 from io import BytesIO
 import pickle
 from dataclasses import dataclass, field
 from PIL import Image
 
 
-import requests
+import requests  # type: ignore
 
 from ..utils.log import LOG_TYPE, log
 from .tts_chapter import TTS_Chapter  # type: ignore
 from .tts_item import TTS_Item  # type: ignore
 
 
 @dataclass
```

### Comparing `tts_arranger-0.1.1/src/tts_arranger/utils/audio.py` & `tts_arranger-0.1.2/src/tts_arranger/utils/audio.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     :param sample_rate: Sample rate of the audio data.
     :type sample_rate: int
 
     :return: The audio data as an AudioSegment object.
     :rtype: AudioSegment
     """
     wav = numpy_wav.astype(np.float32)
-    wav_io = io.BytesIO()
-    scipy.io.wavfile.write(wav_io, sample_rate, wav)
-    wav_io.seek(0)
-    return AudioSegment.from_wav(wav_io)
+    with io.BytesIO() as wav_io:
+        scipy.io.wavfile.write(wav_io, sample_rate, wav)
+        wav_io.seek(0)
+        return AudioSegment.from_wav(wav_io)
 
 
 def segment_to_numpy(segment: AudioSegment) -> np.ndarray:
     """
     Convert an AudioSegment object to a numpy array of audio samples.
 
     :param segment: Audio data as an AudioSegment object.
```

### Comparing `tts_arranger-0.1.1/src/tts_arranger/utils/log.py` & `tts_arranger-0.1.2/src/tts_arranger/utils/log.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.1/tests/tts_arranger_test.py` & `tts_arranger-0.1.2/tests/tts_arranger_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+import os
 import unittest
+from tempfile import TemporaryDirectory
 
-from tts_arranger import TTS_Processor
-from tts_arranger.items.tts_item import TTS_Item
+from tts_arranger import (TTS_Chapter, TTS_Item, TTS_Processor, TTS_Project,
+                          TTS_Writer)
 
 
 class Test(unittest.TestCase):
     def test_break1(self):
         t = TTS_Processor()
 
         tts_item = TTS_Item('This. Is: A t:est!', 'p330')
@@ -311,7 +313,37 @@
         tts_item = TTS_Item('candle- ?, ?')
 
         tts_items = t._prepare_item(tts_item)
         # tts_items = t.break_speakers(tts_items, ('‘', '’'), True)
         # tts_items = t.break_speakers(tts_items, ('"', '"'), True)
 
         self.assertEqual(tts_items[0].text, 'candle-')
+
+    def test_synthesize_and_write(self):
+        items1 = []
+        items1.append(TTS_Item('This is a test:', speaker_idx=0))
+        items1.append(TTS_Item('This is another test:',  speaker_idx=1))
+
+        items2 = []
+        items2.append(TTS_Item('Another test',  speaker_idx=0))
+        items2.append(TTS_Item('This is getting boring!',  speaker_idx=1))
+
+        chapter = []
+        chapter.append(TTS_Chapter(items1, 'Chapter 1'))
+        chapter.append(TTS_Chapter(items2, 'Chapter 2'))
+
+        project = TTS_Project(chapter, 'Project title', 'This is a subtitle', author='Some author')
+
+        with TemporaryDirectory() as tmpdir:
+            output_dir = tmpdir
+            output_format = 'mp3'
+
+            writer = TTS_Writer(project, output_dir, output_format=output_format)
+            writer.synthesize_and_write(project.author + ' - ' + project.title)
+
+            output_file_path = os.path.join(output_dir, f'{project.author} - {project.title}.{output_format}')
+
+            # Ensure that the output file was created
+            self.assertTrue(os.path.exists(output_file_path))
+
+            # Ensure that the output file has a non-zero size
+            self.assertGreater(os.path.getsize(output_file_path), 0)
```

### Comparing `tts_arranger-0.1.1/LICENSE` & `tts_arranger-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.1/pyproject.toml` & `tts_arranger-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   "Operating System :: OS Independent",
 ]
 description = "Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS"
 dynamic = ["dependencies"]
 name = "tts_arranger"
 readme = "README.md"
 requires-python = ">=3.7"
-version = "0.1.1"
+version = "0.1.2"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/knochenhans/tts_arranger/issues"
 "Homepage" = "https://github.com/knochenhans/tts_arranger"
 
 [tool.hatch.build]
 exclude = [
```

### Comparing `tts_arranger-0.1.1/PKG-INFO` & `tts_arranger-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tts_arranger
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS
 Project-URL: Bug Tracker, https://github.com/knochenhans/tts_arranger/issues
 Project-URL: Homepage, https://github.com/knochenhans/tts_arranger
 Author-email: Andre Jonas <nipsky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # TTS Arranger
 
-A set of classes that simplify arranging text fragments with multiple speakers and processing it using coqui.ai TTS.
+A library that simplifies arranging text items fragments with multiple speakers and processing them using coqui.ai TTS to write audio files. 
 
 # Examples
 
 ```python
 from tts_arranger import (TTS_Chapter, TTS_Item, TTS_Project,
                           TTS_Simple_Writer, TTS_Writer)
```

