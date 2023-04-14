# Comparing `tmp/SentenceMatcher-0.0.1.tar.gz` & `tmp/SentenceMatcher-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\SentenceMatcher-0.0.1.tar", last modified: Thu Apr 13 20:40:10 2023, max compression
+gzip compressed data, was "dist\SentenceMatcher-0.0.2.tar", last modified: Fri Apr 14 10:26:14 2023, max compression
```

## Comparing `SentenceMatcher-0.0.1.tar` & `SentenceMatcher-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 20:40:10.126523 SentenceMatcher-0.0.1/
--rw-rw-rw-   0        0        0     3254 2023-04-13 20:40:10.125154 SentenceMatcher-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2507 2023-04-13 20:38:19.000000 SentenceMatcher-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 20:40:10.077953 SentenceMatcher-0.0.1/SentenceMatcher/
--rw-rw-rw-   0        0        0     2935 2023-04-13 20:31:50.000000 SentenceMatcher-0.0.1/SentenceMatcher/SentenceMatcher.py
--rw-rw-rw-   0        0        0       41 2023-04-13 20:38:44.000000 SentenceMatcher-0.0.1/SentenceMatcher/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-13 20:40:10.123153 SentenceMatcher-0.0.1/SentenceMatcher.egg-info/
--rw-rw-rw-   0        0        0     3254 2023-04-13 20:40:09.000000 SentenceMatcher-0.0.1/SentenceMatcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-04-13 20:40:10.000000 SentenceMatcher-0.0.1/SentenceMatcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 20:40:09.000000 SentenceMatcher-0.0.1/SentenceMatcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-13 20:40:09.000000 SentenceMatcher-0.0.1/SentenceMatcher.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-13 20:40:10.126523 SentenceMatcher-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1260 2023-04-13 20:38:03.000000 SentenceMatcher-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:26:14.747941 SentenceMatcher-0.0.2/
+-rw-rw-rw-   0        0        0      468 2023-04-14 10:26:14.746942 SentenceMatcher-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2507 2023-04-13 20:51:14.000000 SentenceMatcher-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-14 10:26:14.747941 SentenceMatcher-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      929 2023-04-14 10:25:30.000000 SentenceMatcher-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 10:26:14.737940 SentenceMatcher-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-04-14 10:26:14.744951 SentenceMatcher-0.0.2/src/SentenceMatcher.egg-info/
+-rw-rw-rw-   0        0        0      468 2023-04-14 10:26:14.000000 SentenceMatcher-0.0.2/src/SentenceMatcher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-04-14 10:26:14.000000 SentenceMatcher-0.0.2/src/SentenceMatcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 10:26:14.000000 SentenceMatcher-0.0.2/src/SentenceMatcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-04-14 10:26:14.000000 SentenceMatcher-0.0.2/src/SentenceMatcher.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2630 2023-04-14 10:18:35.000000 SentenceMatcher-0.0.2/src/SentenceMatcher.py
```

### Comparing `SentenceMatcher-0.0.1/PKG-INFO` & `SentenceMatcher-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,45 @@
-Metadata-Version: 2.1
-Name: SentenceMatcher
-Version: 0.0.1
-Summary: A simple yet useful module that allows you to match a sentence against a list of sentences and return the closest match.
-Author: MahdiTaz (Mahdi Tajwar)
-Author-email: <mahdi05tazwar@gmail.com>
-Keywords: python,ai,sentencematch,sentence,match,difflib,closestmatch,language,naturallanguage
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-
-
-# SentenceMatcher
-### A simple yet useful module that allows you to match a sentence against a list of sentences and return the closest match
-
-<br>
-
-Sample Code:
-```python
-from SentenceMatcher import SentenceMatch
-list_of_sentences = ["Hey there!", "How're you?", "How's your day going?", "So tell me about yourself please!"]
-sentence = "Please tell me about you."
-
-output, accr = SentenceMatch(sentence, list_of_sentences)
-print("Closest Match:", sentence)
-print("Accuracy:", accr)
-```
-
-Output:
-```
-Closest Match: So tell me about yourself please!
-Accuracy: 80.0
-```
-
-<br>
-
-## Explanation
-The module contains only one function: SentenceMatch(to_be_matched, list_to_match_against)
-The first parameter is for the sentence that you want to match against a list of sentences, and the second parameter is for that list of sentences. The function returns 2 values, the output followed by the accuracy of the output.
-Behind the scenes, the function matches the sentence against every sentence in the list of sentences and calculates a percentage (accuracy) value for each. It then returns the sentence with the highest accuracy and returns both the sentence and that accuracy.
-
-HOWEVER:
-Common symbols aren't taken into account, and the case of the letters isn't taken into account as well. It's better to avoid symbols anyways.
-
-<br>
-<h2 style="text-align:center">Mahdi Tajwar, 2023</h2>
-<br><br>
-
-
-# License
-Copyright 2023 Mahdi Tajwar
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+# SentenceMatcher
+### A simple yet useful module that allows you to match a sentence against a list of sentences and return the closest match
+
+<br>
+
+Sample Code:
+```python
+from sentencematcher import SentenceMatch
+list_of_sentences = ["Hey there!", "How're you?", "How's your day going?", "So tell me about yourself please!"]
+sentence = "Please tell me about you."
+
+output, accr = SentenceMatch(sentence, list_of_sentences)
+print("Closest Match:", sentence)
+print("Accuracy:", accr)
+```
+
+Output:
+```
+Closest Match: So tell me about yourself please!
+Accuracy: 80.0
+```
+
+<br>
+
+## Explanation
+The module contains only one function: SentenceMatch(to_be_matched, list_to_match_against)
+The first parameter is for the sentence that you want to match against a list of sentences, and the second parameter is for that list of sentences. The function returns 2 values, the output followed by the accuracy of the output.
+Behind the scenes, the function matches the sentence against every sentence in the list of sentences and calculates a percentage (accuracy) value for each. It then returns the sentence with the highest accuracy and returns both the sentence and that accuracy.
+
+HOWEVER:
+Common symbols aren't taken into account, and the case of the letters isn't taken into account as well. It's better to avoid symbols anyways.
+
+<br>
+<h2 style="text-align:center">Mahdi Tajwar, 2023</h2>
+<br><br>
+
+
+# License
+Copyright 2023 Mahdi Tajwar
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `SentenceMatcher-0.0.1/SentenceMatcher/SentenceMatcher.py` & `SentenceMatcher-0.0.2/src/SentenceMatcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,18 +73,8 @@
         if accr > max_accr:
             max_accr = accr
 
     index_of_sentence_with_max_accr = percentage_accrs.index(max_accr)
     output = sentences_original[index_of_sentence_with_max_accr]
 
     max_accr = "%.1f" % max_accr
-    return output, max_accr
-
-
-
-
-new_list_of_sentences = ["Hey there!", "How're you?", "How's your day going?", "So tell me about yourself please!"]
-new_sentence = "Please tell me about you."
-
-output, new_accr = SentenceMatch(new_sentence, new_list_of_sentences)
-print("Closest Match:", output)
-print("Accuracy:", new_accr)
+    return output, max_accr
```

