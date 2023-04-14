# Comparing `tmp/cribbage_scorer-0.2.2.tar.gz` & `tmp/cribbage_scorer-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cribbage_scorer-0.2.2.tar", last modified: Sun May  8 15:53:28 2022, max compression
+gzip compressed data, was "cribbage_scorer-0.2.3.tar", last modified: Fri Apr 14 19:29:11 2023, max compression
```

## Comparing `cribbage_scorer-0.2.2.tar` & `cribbage_scorer-0.2.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 15:53:28.641435 cribbage_scorer-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)     5826 2022-05-08 15:53:28.641435 cribbage_scorer-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5361 2022-05-08 15:53:23.000000 cribbage_scorer-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 15:53:28.641435 cribbage_scorer-0.2.2/cribbage_scorer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-08 15:53:23.000000 cribbage_scorer-0.2.2/cribbage_scorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11836 2022-05-08 15:53:23.000000 cribbage_scorer-0.2.2/cribbage_scorer/cribbage_scorer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 15:53:28.641435 cribbage_scorer-0.2.2/cribbage_scorer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5826 2022-05-08 15:53:28.000000 cribbage_scorer-0.2.2/cribbage_scorer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-05-08 15:53:28.000000 cribbage_scorer-0.2.2/cribbage_scorer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-08 15:53:28.000000 cribbage_scorer-0.2.2/cribbage_scorer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-05-08 15:53:28.000000 cribbage_scorer-0.2.2/cribbage_scorer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-05-08 15:53:28.000000 cribbage_scorer-0.2.2/cribbage_scorer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-08 15:53:28.641435 cribbage_scorer-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-05-08 15:53:23.000000 cribbage_scorer-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:29:11.683847 cribbage_scorer-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-14 19:29:11.683847 cribbage_scorer-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-04-14 19:29:01.000000 cribbage_scorer-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:29:11.683847 cribbage_scorer-0.2.3/cribbage_scorer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 19:29:01.000000 cribbage_scorer-0.2.3/cribbage_scorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11735 2023-04-14 19:29:01.000000 cribbage_scorer-0.2.3/cribbage_scorer/cribbage_scorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 19:29:11.683847 cribbage_scorer-0.2.3/cribbage_scorer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-14 19:29:11.000000 cribbage_scorer-0.2.3/cribbage_scorer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-14 19:29:11.000000 cribbage_scorer-0.2.3/cribbage_scorer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 19:29:11.000000 cribbage_scorer-0.2.3/cribbage_scorer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 19:29:11.000000 cribbage_scorer-0.2.3/cribbage_scorer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-14 19:29:11.000000 cribbage_scorer-0.2.3/cribbage_scorer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 19:29:11.683847 cribbage_scorer-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 19:29:01.000000 cribbage_scorer-0.2.3/setup.py
```

### Comparing `cribbage_scorer-0.2.2/PKG-INFO` & `cribbage_scorer-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cribbage_scorer
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Cribbage scoring tool
 Home-page: https://github.com/phoughton/cribbage_scorer
 Author: Peter Houghton
 Author-email: pete@investigatingsoftware.co.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 
 Cribbage scorer is a simple scoring engine for the classic card game.
 
 For details, history and a good summary of the rules of the game see [Wikipedia](https://en.wikipedia.org/wiki/Cribbage)
 
 For instruction on how to play and the rules see the [American Cribbage Congress](http://www.cribbage.org/NewSite/rules) (see link to PDF)
 
-The code for the web server front end that uses this python API can be [found on GitHub](https://github.com/phoughton/cribbage_server). Raise a bug here if you find any.
+The code for the web server front end that uses this python API can be [found on GitHub](https://github.com/phoughton/cribbage_server). Raise a bug here if you find any. This server is also now available as a [Docker container](https://hub.docker.com/r/phoughton/python-cribbage).
 
 
 This package is tested against against Python versions: "3.6", "3.7", "3.8", "3.9", "3.10" on Ubuntu-latest. (But should work on Windows and Mac etc.)
 
 ## Installation 
 ```bash
 pip install cribbage-scorer
@@ -138,15 +138,15 @@
 ```
 Results:
 ```
 (29, "Four of a kind: 5s (12pts), Made 15 from [(5, 'D'), (11, 'D')] (2pts), Made 15 from [(5, 'S'), (11, 'D')] (2pts), Made 15 from [(5, 'C'), (11, 'D')] (2pts), Made 15 from [(11, 'D'), (5, 'D')] (2pts), Made 15 from [(5, 'D'), (5, 'S'), (5, 'C')] (2pts), Made 15 from [(5, 'D'), (5, 'S'), (5, 'D')] (2pts), Made 15 from [(5, 'D'), (5, 'C'), (5, 'D')] (2pts), Made 15 from [(5, 'S'), (5, 'C'), (5, 'D')] (2pts), One for his nobs (1pt)")
 ```
 
 ### License:
-Copyright © 2022 Peter Houghton
+Copyright © 2023 Peter Houghton
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `cribbage_scorer-0.2.2/README.md` & `cribbage_scorer-0.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Cribbage scorer is a simple scoring engine for the classic card game.
 
 For details, history and a good summary of the rules of the game see [Wikipedia](https://en.wikipedia.org/wiki/Cribbage)
 
 For instruction on how to play and the rules see the [American Cribbage Congress](http://www.cribbage.org/NewSite/rules) (see link to PDF)
 
-The code for the web server front end that uses this python API can be [found on GitHub](https://github.com/phoughton/cribbage_server). Raise a bug here if you find any.
+The code for the web server front end that uses this python API can be [found on GitHub](https://github.com/phoughton/cribbage_server). Raise a bug here if you find any. This server is also now available as a [Docker container](https://hub.docker.com/r/phoughton/python-cribbage).
 
 
 This package is tested against against Python versions: "3.6", "3.7", "3.8", "3.9", "3.10" on Ubuntu-latest. (But should work on Windows and Mac etc.)
 
 ## Installation 
 ```bash
 pip install cribbage-scorer
@@ -123,14 +123,14 @@
 ```
 Results:
 ```
 (29, "Four of a kind: 5s (12pts), Made 15 from [(5, 'D'), (11, 'D')] (2pts), Made 15 from [(5, 'S'), (11, 'D')] (2pts), Made 15 from [(5, 'C'), (11, 'D')] (2pts), Made 15 from [(11, 'D'), (5, 'D')] (2pts), Made 15 from [(5, 'D'), (5, 'S'), (5, 'C')] (2pts), Made 15 from [(5, 'D'), (5, 'S'), (5, 'D')] (2pts), Made 15 from [(5, 'D'), (5, 'C'), (5, 'D')] (2pts), Made 15 from [(5, 'S'), (5, 'C'), (5, 'D')] (2pts), One for his nobs (1pt)")
 ```
 
 ### License:
-Copyright © 2022 Peter Houghton
+Copyright © 2023 Peter Houghton
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `cribbage_scorer-0.2.2/cribbage_scorer/cribbage_scorer.py` & `cribbage_scorer-0.2.3/cribbage_scorer/cribbage_scorer.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,35 +54,30 @@
         cards = played_cards[0:index]
         go_played_by = None
 
         if cards[-1] == (0, "GO"):
             go_played_by = last_player(cards, players)
             players_in_play.remove(go_played_by)
 
-        cards = remove_goes(cards)
+        # Remove GOs
+        cards = [card for card in cards if card != (0, "GO")]
 
         count, score, msg = play_score_ongoing(cards, index == len(played_cards))
 
         point_winner = last_player(cards, players_in_play)
         scores[point_winner] += score
 
         if score > 0:
             play_log.append(f"Count: {count}, {point_winner}: {msg}, score so far: {scores[point_winner]} ")
         else:
             play_log.append(f"Count: {count}, No Points scored, {go_played_by} said Go. ")
 
-    return dict(scores), count, play_log
+    return scores, count, play_log
 
 
-def remove_goes(played_cards):
-    cards = played_cards.copy()
-    while (0, "GO") in cards:
-        cards.remove((0, "GO"))
-    return cards
-
 
 def play_score_ongoing(played_cards, last_card=False):
     
     dupe_check(played_cards)
 
     scores = []
     count = count_cards(played_cards)
```

### Comparing `cribbage_scorer-0.2.2/cribbage_scorer.egg-info/PKG-INFO` & `cribbage_scorer-0.2.3/cribbage_scorer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cribbage-scorer
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Cribbage scoring tool
 Home-page: https://github.com/phoughton/cribbage_scorer
 Author: Peter Houghton
 Author-email: pete@investigatingsoftware.co.uk
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 
 Cribbage scorer is a simple scoring engine for the classic card game.
 
 For details, history and a good summary of the rules of the game see [Wikipedia](https://en.wikipedia.org/wiki/Cribbage)
 
 For instruction on how to play and the rules see the [American Cribbage Congress](http://www.cribbage.org/NewSite/rules) (see link to PDF)
 
-The code for the web server front end that uses this python API can be [found on GitHub](https://github.com/phoughton/cribbage_server). Raise a bug here if you find any.
+The code for the web server front end that uses this python API can be [found on GitHub](https://github.com/phoughton/cribbage_server). Raise a bug here if you find any. This server is also now available as a [Docker container](https://hub.docker.com/r/phoughton/python-cribbage).
 
 
 This package is tested against against Python versions: "3.6", "3.7", "3.8", "3.9", "3.10" on Ubuntu-latest. (But should work on Windows and Mac etc.)
 
 ## Installation 
 ```bash
 pip install cribbage-scorer
@@ -138,15 +138,15 @@
 ```
 Results:
 ```
 (29, "Four of a kind: 5s (12pts), Made 15 from [(5, 'D'), (11, 'D')] (2pts), Made 15 from [(5, 'S'), (11, 'D')] (2pts), Made 15 from [(5, 'C'), (11, 'D')] (2pts), Made 15 from [(11, 'D'), (5, 'D')] (2pts), Made 15 from [(5, 'D'), (5, 'S'), (5, 'C')] (2pts), Made 15 from [(5, 'D'), (5, 'S'), (5, 'D')] (2pts), Made 15 from [(5, 'D'), (5, 'C'), (5, 'D')] (2pts), Made 15 from [(5, 'S'), (5, 'C'), (5, 'D')] (2pts), One for his nobs (1pt)")
 ```
 
 ### License:
-Copyright © 2022 Peter Houghton
+Copyright © 2023 Peter Houghton
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `cribbage_scorer-0.2.2/setup.py` & `cribbage_scorer-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cribbage_scorer",
-    version="0.2.2",
+    version="0.2.3",
     author="Peter Houghton",
     author_email="pete@investigatingsoftware.co.uk",
     description="A Cribbage scoring tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/phoughton/cribbage_scorer",
     packages=setuptools.find_packages(),
```

