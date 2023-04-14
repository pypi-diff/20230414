# Comparing `tmp/pyttsx4-3.0.6-py3-none-any.whl.zip` & `tmp/pyttsx4-3.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 33344 bytes, number of entries: 16
+Zip file size: 33422 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      814 b- defN 23-Apr-07 13:37 pyttsx4/__init__.py
 -rw-r--r--  2.0 unx     7429 b- defN 23-Apr-07 17:19 pyttsx4/driver.py
 -rw-r--r--  2.0 unx     7224 b- defN 23-Apr-07 13:37 pyttsx4/engine.py
 -rw-r--r--  2.0 unx    29524 b- defN 23-Apr-11 03:46 pyttsx4/six.py
 -rw-r--r--  2.0 unx      431 b- defN 23-Apr-07 13:37 pyttsx4/voice.py
 -rw-r--r--  2.0 unx      853 b- defN 23-Apr-11 03:47 pyttsx4/drivers/__init__.py
 -rw-r--r--  2.0 unx    19495 b- defN 23-Apr-07 13:37 pyttsx4/drivers/_espeak.py
 -rw-r--r--  2.0 unx     6182 b- defN 23-Apr-07 13:37 pyttsx4/drivers/dummy.py
 -rw-r--r--  2.0 unx     7448 b- defN 23-Apr-11 03:43 pyttsx4/drivers/espeak.py
 -rw-r--r--  2.0 unx     3895 b- defN 23-Apr-12 08:25 pyttsx4/drivers/nsss.py
--rw-r--r--  2.0 unx     6552 b- defN 23-Apr-11 03:47 pyttsx4/drivers/sapi5.py
--rw-r--r--  2.0 unx    17098 b- defN 23-Apr-12 08:28 pyttsx4-3.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     1821 b- defN 23-Apr-12 08:28 pyttsx4-3.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 08:28 pyttsx4-3.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Apr-12 08:28 pyttsx4-3.0.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1244 b- defN 23-Apr-12 08:28 pyttsx4-3.0.6.dist-info/RECORD
-16 files, 110110 bytes uncompressed, 31324 bytes compressed:  71.6%
+-rw-r--r--  2.0 unx     6751 b- defN 23-Apr-14 05:23 pyttsx4/drivers/sapi5.py
+-rw-r--r--  2.0 unx    17098 b- defN 23-Apr-14 05:24 pyttsx4-3.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1821 b- defN 23-Apr-14 05:24 pyttsx4-3.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 05:24 pyttsx4-3.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Apr-14 05:24 pyttsx4-3.0.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1244 b- defN 23-Apr-14 05:24 pyttsx4-3.0.7.dist-info/RECORD
+16 files, 110309 bytes uncompressed, 31402 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: pyttsx4/drivers/nsss.py
 Comment: 
 
 Filename: pyttsx4/drivers/sapi5.py
 Comment: 
 
-Filename: pyttsx4-3.0.6.dist-info/LICENSE
+Filename: pyttsx4-3.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: pyttsx4-3.0.6.dist-info/METADATA
+Filename: pyttsx4-3.0.7.dist-info/METADATA
 Comment: 
 
-Filename: pyttsx4-3.0.6.dist-info/WHEEL
+Filename: pyttsx4-3.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: pyttsx4-3.0.6.dist-info/top_level.txt
+Filename: pyttsx4-3.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: pyttsx4-3.0.6.dist-info/RECORD
+Filename: pyttsx4-3.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyttsx4/drivers/sapi5.py

```diff
@@ -43,14 +43,17 @@
         self._looping = False
         self._speaking = False
         self._stopping = False
         # initial rate
         self._rateWpm = 200
         self.setProperty('voice', self.getProperty('voice'))
 
+        #-10=>+10
+        self.pitch= 0
+
     def destroy(self):
         self._tts.EventInterests = 0
 
     def say(self, text):
         self._proxy.setBusy(True)
         self._proxy.notify('started-utterance')
         self._speaking = True
@@ -119,15 +122,16 @@
         elif name == 'voice':
             return self._tts.Voice.Id
         elif name == 'rate':
             return self._rateWpm
         elif name == 'volume':
             return self._tts.Volume / 100.0
         elif name == 'pitch':
-            print("Pitch adjustment not supported when using SAPI5")
+            return self.pitch
+            #print("Pitch adjustment not supported when using SAPI5")
         else:
             raise KeyError('unknown property %s' % name)
 
     def setProperty(self, name, value):
         if name == 'voice':
             token = self._tokenFromId(value)
             self._tts.Voice = token
@@ -148,15 +152,18 @@
             self._rateWpm = value
         elif name == 'volume':
             try:
                 self._tts.Volume = int(round(value * 100, 2))
             except TypeError as e:
                 raise ValueError(str(e))
         elif name == 'pitch':
-            print("Pitch adjustment not supported when using SAPI5")
+            #-10 ->10
+            self.pitch = value
+            self._tts.Speak('<pitch absmiddle="'+str(value)+'"/>')
+            print("Pitch adjustment is not tested when using SAPI5")
         else:
             raise KeyError('unknown property %s' % name)
 
     def startLoop(self):
         self._looping = True
         first = True
         while self._looping:
```

## Comparing `pyttsx4-3.0.6.dist-info/LICENSE` & `pyttsx4-3.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyttsx4-3.0.6.dist-info/METADATA` & `pyttsx4-3.0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyttsx4
-Version: 3.0.6
+Version: 3.0.7
 Summary: Text to Speech (TTS) library for Python 3. Works without internet connection or delay. Supports multiple TTS engines, including Sapi5, nsss, and espeak.
 Home-page: https://github.com/Jiangshan00001/pyttsx4
 Author: Natesh M Bhat
 Author-email: 710806594@qq.com
 License: UNKNOWN
 Keywords: pyttsx,ivona,pyttsx for python3,TTS for python3,pyttsx3,text to speech for python,tts,text to speech,speech,speech synthesis,offline text to speech,offline tts,gtts
 Platform: UNKNOWN
```

## Comparing `pyttsx4-3.0.6.dist-info/RECORD` & `pyttsx4-3.0.7.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -4,13 +4,13 @@
 pyttsx4/six.py,sha256=yVeu0rLX2Qv1P1UaJtvamDmMrjnxNsJkSuztEvVyGG8,29524
 pyttsx4/voice.py,sha256=GYZLgGtnmjLrg93Wh7_lqDcs6zMaTS_QRr3KZM7RZnY,431
 pyttsx4/drivers/__init__.py,sha256=EFf83iBpSVF4joEh4gQmq5Rl22tngVNuR1zBeWfCdjQ,853
 pyttsx4/drivers/_espeak.py,sha256=Gj0N4aFf3YGZO9fq8K5BFbiwkIExqDu1nBXUn7EZVzY,19495
 pyttsx4/drivers/dummy.py,sha256=d7K46sijjOxwmAJHbgEALwbYwGcktLfW1FcX1iG5I8E,6182
 pyttsx4/drivers/espeak.py,sha256=5QcaVaCyb3xLKXs6_fjnGv0-mioUXINzendba95mpgs,7448
 pyttsx4/drivers/nsss.py,sha256=n0_ysxWeZhqQuiaxpzZo5RYOIl2Ef0yvX7Kj4du30yo,3895
-pyttsx4/drivers/sapi5.py,sha256=EiEEwvammMCS4YI7aWG0fmtQZm_0-bPJqC9nndUUpp4,6552
-pyttsx4-3.0.6.dist-info/LICENSE,sha256=JoTeFzAOCkNGhvHsf4r2BFIHpLRXo_4EsrnOZV58XVA,17098
-pyttsx4-3.0.6.dist-info/METADATA,sha256=GIyd80nO4G1JqUOWIR4p8t5WAWdqNh5Y6TK7kINJD6w,1821
-pyttsx4-3.0.6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyttsx4-3.0.6.dist-info/top_level.txt,sha256=RZW_EXmaQg7go8T0q583RzqdJUlYm0NeSHGpyq92tiY,8
-pyttsx4-3.0.6.dist-info/RECORD,,
+pyttsx4/drivers/sapi5.py,sha256=N0wxVKHhPBKkHgD5fg5KPC5NTwXOwKglfExP7-8oKnk,6751
+pyttsx4-3.0.7.dist-info/LICENSE,sha256=JoTeFzAOCkNGhvHsf4r2BFIHpLRXo_4EsrnOZV58XVA,17098
+pyttsx4-3.0.7.dist-info/METADATA,sha256=Q43LurrEUphjuCAx5qmdH_J8NAm19YL8CqBGc3a9qNQ,1821
+pyttsx4-3.0.7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pyttsx4-3.0.7.dist-info/top_level.txt,sha256=RZW_EXmaQg7go8T0q583RzqdJUlYm0NeSHGpyq92tiY,8
+pyttsx4-3.0.7.dist-info/RECORD,,
```

