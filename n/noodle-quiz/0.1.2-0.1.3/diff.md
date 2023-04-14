# Comparing `tmp/noodle_quiz-0.1.2.tar.gz` & `tmp/noodle_quiz-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noodle_quiz-0.1.2.tar", last modified: Tue Apr 11 13:20:21 2023, max compression
+gzip compressed data, was "noodle_quiz-0.1.3.tar", last modified: Fri Apr 14 15:14:23 2023, max compression
```

## Comparing `noodle_quiz-0.1.2.tar` & `noodle_quiz-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rafaellopez   (502) staff       (20)        0 2023-04-11 13:20:21.443212 noodle_quiz-0.1.2/
--rw-r--r--   0 rafaellopez   (502) staff       (20)     1069 2023-04-10 07:34:44.000000 noodle_quiz-0.1.2/LICENSE
--rw-r--r--   0 rafaellopez   (502) staff       (20)       17 2023-04-10 08:01:18.000000 noodle_quiz-0.1.2/MANIFEST.in
--rw-r--r--   0 rafaellopez   (502) staff       (20)      889 2023-04-11 13:20:21.443088 noodle_quiz-0.1.2/PKG-INFO
--rw-r--r--   0 rafaellopez   (502) staff       (20)      385 2023-04-11 13:20:03.000000 noodle_quiz-0.1.2/README.md
-drwxr-xr-x   0 rafaellopez   (502) staff       (20)        0 2023-04-11 13:20:21.442291 noodle_quiz-0.1.2/noodle_quiz/
--rw-r--r--   0 rafaellopez   (502) staff       (20)     1065 2023-04-11 13:20:03.000000 noodle_quiz-0.1.2/noodle_quiz/__init__.py
--rw-r--r--   0 rafaellopez   (502) staff       (20)     2405 2023-04-11 13:20:03.000000 noodle_quiz-0.1.2/noodle_quiz/answer_types.py
--rw-r--r--   0 rafaellopez   (502) staff       (20)      507 2023-04-11 13:20:03.000000 noodle_quiz-0.1.2/noodle_quiz/exc.py
--rw-r--r--   0 rafaellopez   (502) staff       (20)     6189 2023-04-11 13:20:03.000000 noodle_quiz-0.1.2/noodle_quiz/question_types.py
-drwxr-xr-x   0 rafaellopez   (502) staff       (20)        0 2023-04-11 13:20:21.442947 noodle_quiz-0.1.2/noodle_quiz.egg-info/
--rw-r--r--   0 rafaellopez   (502) staff       (20)      889 2023-04-11 13:20:21.000000 noodle_quiz-0.1.2/noodle_quiz.egg-info/PKG-INFO
--rw-r--r--   0 rafaellopez   (502) staff       (20)      313 2023-04-11 13:20:21.000000 noodle_quiz-0.1.2/noodle_quiz.egg-info/SOURCES.txt
--rw-r--r--   0 rafaellopez   (502) staff       (20)        1 2023-04-11 13:20:21.000000 noodle_quiz-0.1.2/noodle_quiz.egg-info/dependency_links.txt
--rw-r--r--   0 rafaellopez   (502) staff       (20)        1 2023-04-10 14:42:54.000000 noodle_quiz-0.1.2/noodle_quiz.egg-info/not-zip-safe
--rw-r--r--   0 rafaellopez   (502) staff       (20)       12 2023-04-11 13:20:21.000000 noodle_quiz-0.1.2/noodle_quiz.egg-info/top_level.txt
--rw-r--r--   0 rafaellopez   (502) staff       (20)       38 2023-04-11 13:20:21.443249 noodle_quiz-0.1.2/setup.cfg
--rw-r--r--   0 rafaellopez   (502) staff       (20)      781 2023-04-11 13:20:03.000000 noodle_quiz-0.1.2/setup.py
+drwxr-xr-x   0 rafaellopez   (502) staff       (20)        0 2023-04-14 15:14:23.604799 noodle_quiz-0.1.3/
+-rw-r--r--   0 rafaellopez   (502) staff       (20)     1069 2023-04-10 07:34:44.000000 noodle_quiz-0.1.3/LICENSE
+-rw-r--r--   0 rafaellopez   (502) staff       (20)       17 2023-04-10 08:01:18.000000 noodle_quiz-0.1.3/MANIFEST.in
+-rw-r--r--   0 rafaellopez   (502) staff       (20)     1375 2023-04-14 15:14:23.604679 noodle_quiz-0.1.3/PKG-INFO
+-rw-r--r--   0 rafaellopez   (502) staff       (20)      871 2023-04-12 14:57:07.000000 noodle_quiz-0.1.3/README.md
+drwxr-xr-x   0 rafaellopez   (502) staff       (20)        0 2023-04-14 15:14:23.603886 noodle_quiz-0.1.3/noodle_quiz/
+-rw-r--r--   0 rafaellopez   (502) staff       (20)     1065 2023-04-11 13:20:03.000000 noodle_quiz-0.1.3/noodle_quiz/__init__.py
+-rw-r--r--   0 rafaellopez   (502) staff       (20)     3046 2023-04-12 07:30:21.000000 noodle_quiz-0.1.3/noodle_quiz/answer_types.py
+-rw-r--r--   0 rafaellopez   (502) staff       (20)      507 2023-04-11 13:20:03.000000 noodle_quiz-0.1.3/noodle_quiz/exc.py
+-rw-r--r--   0 rafaellopez   (502) staff       (20)    10375 2023-04-12 14:13:49.000000 noodle_quiz-0.1.3/noodle_quiz/question_types.py
+drwxr-xr-x   0 rafaellopez   (502) staff       (20)        0 2023-04-14 15:14:23.604533 noodle_quiz-0.1.3/noodle_quiz.egg-info/
+-rw-r--r--   0 rafaellopez   (502) staff       (20)     1375 2023-04-14 15:14:23.000000 noodle_quiz-0.1.3/noodle_quiz.egg-info/PKG-INFO
+-rw-r--r--   0 rafaellopez   (502) staff       (20)      313 2023-04-14 15:14:23.000000 noodle_quiz-0.1.3/noodle_quiz.egg-info/SOURCES.txt
+-rw-r--r--   0 rafaellopez   (502) staff       (20)        1 2023-04-14 15:14:23.000000 noodle_quiz-0.1.3/noodle_quiz.egg-info/dependency_links.txt
+-rw-r--r--   0 rafaellopez   (502) staff       (20)        1 2023-04-10 14:42:54.000000 noodle_quiz-0.1.3/noodle_quiz.egg-info/not-zip-safe
+-rw-r--r--   0 rafaellopez   (502) staff       (20)       12 2023-04-14 15:14:23.000000 noodle_quiz-0.1.3/noodle_quiz.egg-info/top_level.txt
+-rw-r--r--   0 rafaellopez   (502) staff       (20)       38 2023-04-14 15:14:23.604827 noodle_quiz-0.1.3/setup.cfg
+-rw-r--r--   0 rafaellopez   (502) staff       (20)      781 2023-04-14 15:13:52.000000 noodle_quiz-0.1.3/setup.py
```

### Comparing `noodle_quiz-0.1.2/LICENSE` & `noodle_quiz-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `noodle_quiz-0.1.2/noodle_quiz/__init__.py` & `noodle_quiz-0.1.3/noodle_quiz/__init__.py`

 * *Files identical despite different names*

### Comparing `noodle_quiz-0.1.2/noodle_quiz/answer_types.py` & `noodle_quiz-0.1.3/noodle_quiz/answer_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -70,7 +70,28 @@
         s = self.text_before + '\n{'
         s += f'{str(self.score)}:{self.cloze_type}:'
         for item in self.items:
             s += str(item)
         s += '}\n'
         s += f'{self.text_after}'
         return s
+
+
+class MultipleChoiceAnswer(Answer):
+    def __init__(self, fraction, value, feedback_text=''):
+        if fraction is None:
+            raise MandatoryFieldMissing('fraction')
+
+        self.fraction = fraction
+
+        if value is None:
+            raise MandatoryFieldMissing('value')
+
+        self.value = value
+        self.feedback_text = feedback_text
+
+    def __str__(self):
+        s = f'<answer fraction="{self.fraction}" format="html">'
+        s += f'<text><![CDATA[{self.value}]]></text>'
+        s += f'<feedback format="html"><text><![CDATA[{self.feedback_text}]]></text></feedback>'
+        s += '</answer>'
+        return s
```

### Comparing `noodle_quiz-0.1.2/setup.py` & `noodle_quiz-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def readme():
     with open('README.md') as f:
         return f.read()
 
 
 setup(name='noodle_quiz',
-      version='0.1.2',
+      version='0.1.3',
       description='Noodle-Quiz (Not Moodle Quiz generator) is a set of utilities to generate quizzes for Moodle',
       long_description=readme(),
       long_description_content_type='text/markdown',
       classifiers=[
           'Development Status :: 3 - Alpha',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3.10',
```

