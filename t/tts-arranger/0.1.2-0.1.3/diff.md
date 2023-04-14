# Comparing `tmp/tts_arranger-0.1.2.tar.gz` & `tmp/tts_arranger-0.1.3.tar.gz`

## Comparing `tts_arranger-0.1.2.tar` & `tts_arranger-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/requirements.txt
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/__init__.py
--rw-r--r--   0        0        0    26369 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/tts_processor.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/tts_processor_example.py
--rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/tts_simple_writer.py
--rw-r--r--   0        0        0    15112 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/tts_writer.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/data/replace.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/data/replace_de.json
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/data/replace_en.json
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/items/__init__.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/items/tts_chapter.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/items/tts_item.py
--rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/items/tts_project.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/utils/__init__.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/utils/audio.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/src/tts_arranger/utils/log.py
--rw-r--r--   0        0        0    18265 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/tests/tts_arranger_test.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/LICENSE
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/README.md
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 tts_arranger-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/requirements.txt
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/__init__.py
+-rw-r--r--   0        0        0    25903 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/tts_processor.py
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/tts_processor_example.py
+-rw-r--r--   0        0        0     4498 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/tts_simple_writer.py
+-rw-r--r--   0        0        0    15112 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/tts_writer.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/data/replace.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/data/replace_de.json
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/data/replace_en.json
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/items/__init__.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/items/tts_chapter.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/items/tts_item.py
+-rw-r--r--   0        0        0     5158 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/items/tts_project.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/utils/__init__.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/utils/audio.py
+-rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/src/tts_arranger/utils/log.py
+-rw-r--r--   0        0        0    18265 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/tests/tts_arranger_test.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/README.md
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 tts_arranger-0.1.3/PKG-INFO
```

### Comparing `tts_arranger-0.1.2/src/tts_arranger/tts_processor.py` & `tts_arranger-0.1.3/src/tts_arranger/tts_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -524,28 +524,20 @@
         if items:
             for item in items:
                 if not merged_item:
                     # Scanning not started
                     merged_item = item
                 elif merged_item.speaker == item.speaker and merged_item.speaker_idx == item.speaker_idx:
                     # Starting item and current are similar, add to merge item text and length
-                    if merged_item.text and item.text:
-                        merged_item = merged_item.__class__(
-                            text=f'{merged_item.text.strip()} {item.text.strip()}',
-                            speaker=merged_item.speaker,
-                            speaker_idx=merged_item.speaker_idx,
-                            length=merged_item.length + item.length
-                        )
-                    else:
-                        merged_item = merged_item.__class__(
-                            text=f'{merged_item.text}{item.text}',
-                            speaker=merged_item.speaker,
-                            speaker_idx=merged_item.speaker_idx,
-                            length=merged_item.length + item.length
-                        )
+                    merged_item = merged_item.__class__(
+                        text=f'{merged_item.text}{item.text}',
+                        speaker=merged_item.speaker,
+                        speaker_idx=merged_item.speaker_idx,
+                        length=merged_item.length + item.length
+                    )
                 else:
                     # Starting item and current are not similar, add last and current item, set this item as new starting item
                     final_items.append(merged_item)
                     merged_item = item
 
             if merged_item is not None:
                 final_items.append(merged_item)
```

### Comparing `tts_arranger-0.1.2/src/tts_arranger/tts_processor_example.py` & `tts_arranger-0.1.3/src/tts_arranger/tts_processor_example.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,19 +3,19 @@
                           TTS_Simple_Writer, TTS_Writer)
 
 # Simple example using Simple Writer (using a simple list of TTS items)
 
 tts_items = []
 
 tts_items.append(TTS_Item('This is a test', 'p330'))
-tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 'ED\n', length=10000))
+tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 'p273', length=10000))
 tts_items.append(TTS_Item(length=2000))  # Insert pause
 
 simple_writer = TTS_Simple_Writer(tts_items)
-simple_writer.synthesize_and_write('/tmp/tts_arranger_example_output/test2.mp3')
+simple_writer.synthesize_and_write('/tmp/tts_arranger_example_output/test.mp3')
 
 # English example using tts_models/en/vctk/vits (with multispeaker support)
 
 items1 = []
 items1.append(TTS_Item('This is a test:', speaker_idx=0))
 items1.append(TTS_Item('This is another test:',  speaker_idx=1))
 
@@ -28,16 +28,16 @@
 chapter.append(TTS_Chapter(items2, 'Chapter 2'))
 
 project = TTS_Project(chapter, 'Project title', 'This is a subtitle', author='Some author')
 
 # Add a cover image
 project.add_image_from_url('https://coqui.ai/static/38a06ec53309f617be3eb3b8b9367abf/598c3/logo-wordmark.png')
 
-writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', output_format='mp3')
-writer.synthesize_and_write(project.author + ' - ' + project.title, concat=False)
+writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/')
+writer.synthesize_and_write(project.author + ' - ' + project.title)
 
 # German example using Thorsten voice (no multispeaker support)
 
 items1 = []
 items1.append(TTS_Item('Dies ist ein Test:', speaker_idx=0))
 items1.append(TTS_Item('Noch ein Test:',  speaker_idx=1))
 
@@ -47,9 +47,9 @@
 
 chapter = []
 chapter.append(TTS_Chapter(items1, 'Kapitel 1'))
 chapter.append(TTS_Chapter(items2, 'Kapitel 2'))
 
 project = TTS_Project(chapter, 'Projektname', 'Dies ist ein Untertitel', author='Ein Autor', lang_code='de')
 
-writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', model='tts_models/de/thorsten/tacotron2-DDC', vocoder='vocoder_models/de/thorsten/hifigan_v1')
-writer.synthesize_and_write(project.author + ' - ' + project.title)
+writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', model='tts_models/de/thorsten/tacotron2-DDC', vocoder='vocoder_models/de/thorsten/hifigan_v1', output_format='mp3')
+writer.synthesize_and_write(project.author + ' - ' + project.title, concat=False)
```

### Comparing `tts_arranger-0.1.2/src/tts_arranger/tts_simple_writer.py` & `tts_arranger-0.1.3/src/tts_arranger/tts_simple_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.2/src/tts_arranger/tts_writer.py` & `tts_arranger-0.1.3/src/tts_arranger/tts_writer.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.2/src/tts_arranger/items/tts_chapter.py` & `tts_arranger-0.1.3/src/tts_arranger/items/tts_chapter.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.2/src/tts_arranger/items/tts_item.py` & `tts_arranger-0.1.3/src/tts_arranger/items/tts_item.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.2/src/tts_arranger/items/tts_project.py` & `tts_arranger-0.1.3/src/tts_arranger/items/tts_project.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.2/src/tts_arranger/utils/audio.py` & `tts_arranger-0.1.3/src/tts_arranger/utils/audio.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.2/src/tts_arranger/utils/log.py` & `tts_arranger-0.1.3/src/tts_arranger/utils/log.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.2/tests/tts_arranger_test.py` & `tts_arranger-0.1.3/tests/tts_arranger_test.py`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.2/LICENSE` & `tts_arranger-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tts_arranger-0.1.2/README.md` & `tts_arranger-0.1.3/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -9,19 +9,19 @@
                           TTS_Simple_Writer, TTS_Writer)
 
 # Simple example using Simple Writer (using a simple list of TTS items)
 
 tts_items = []
 
 tts_items.append(TTS_Item('This is a test', 'p330'))
-tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 'ED\n', length=10000))
+tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 'p273', length=10000))
 tts_items.append(TTS_Item(length=2000))  # Insert pause
 
 simple_writer = TTS_Simple_Writer(tts_items)
-simple_writer.synthesize_and_write('/tmp/tts_arranger_example_output/test2.mp3')
+simple_writer.synthesize_and_write('/tmp/tts_arranger_example_output/test.mp3')
 
 # English example using tts_models/en/vctk/vits (with multispeaker support)
 
 items1 = []
 items1.append(TTS_Item('This is a test:', speaker_idx=0))
 items1.append(TTS_Item('This is another test:',  speaker_idx=1))
 
@@ -34,10 +34,10 @@
 chapter.append(TTS_Chapter(items2, 'Chapter 2'))
 
 project = TTS_Project(chapter, 'Project title', 'This is a subtitle', author='Some author')
 
 # Add a cover image
 project.add_image_from_url('https://coqui.ai/static/38a06ec53309f617be3eb3b8b9367abf/598c3/logo-wordmark.png')
 
-writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', output_format='mp3')
-writer.synthesize_and_write(project.author + ' - ' + project.title, concat=False)
+writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/')
+writer.synthesize_and_write(project.author + ' - ' + project.title)
 ```
```

### Comparing `tts_arranger-0.1.2/pyproject.toml` & `tts_arranger-0.1.3/pyproject.toml`

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
-version = "0.1.2"
+version = "0.1.3"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/knochenhans/tts_arranger/issues"
 "Homepage" = "https://github.com/knochenhans/tts_arranger"
 
 [tool.hatch.build]
 exclude = [
```

### Comparing `tts_arranger-0.1.2/PKG-INFO` & `tts_arranger-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tts_arranger
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simplifies arranging text fragments with multiple speakers and processing it with coqui.ai TTS
 Project-URL: Bug Tracker, https://github.com/knochenhans/tts_arranger/issues
 Project-URL: Homepage, https://github.com/knochenhans/tts_arranger
 Author-email: Andre Jonas <nipsky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -23,19 +23,19 @@
                           TTS_Simple_Writer, TTS_Writer)
 
 # Simple example using Simple Writer (using a simple list of TTS items)
 
 tts_items = []
 
 tts_items.append(TTS_Item('This is a test', 'p330'))
-tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 'ED\n', length=10000))
+tts_items.append(TTS_Item('This is a test with another speaker and a fixed minimum length', 'p273', length=10000))
 tts_items.append(TTS_Item(length=2000))  # Insert pause
 
 simple_writer = TTS_Simple_Writer(tts_items)
-simple_writer.synthesize_and_write('/tmp/tts_arranger_example_output/test2.mp3')
+simple_writer.synthesize_and_write('/tmp/tts_arranger_example_output/test.mp3')
 
 # English example using tts_models/en/vctk/vits (with multispeaker support)
 
 items1 = []
 items1.append(TTS_Item('This is a test:', speaker_idx=0))
 items1.append(TTS_Item('This is another test:',  speaker_idx=1))
 
@@ -48,10 +48,10 @@
 chapter.append(TTS_Chapter(items2, 'Chapter 2'))
 
 project = TTS_Project(chapter, 'Project title', 'This is a subtitle', author='Some author')
 
 # Add a cover image
 project.add_image_from_url('https://coqui.ai/static/38a06ec53309f617be3eb3b8b9367abf/598c3/logo-wordmark.png')
 
-writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/', output_format='mp3')
-writer.synthesize_and_write(project.author + ' - ' + project.title, concat=False)
+writer = TTS_Writer(project, '/tmp/tts_arranger_example_output/')
+writer.synthesize_and_write(project.author + ' - ' + project.title)
 ```
```

