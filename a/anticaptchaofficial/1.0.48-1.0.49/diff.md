# Comparing `tmp/anticaptchaofficial-1.0.48-py3-none-any.whl.zip` & `tmp/anticaptchaofficial-1.0.49-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 17142 bytes, number of entries: 23
+Zip file size: 17174 bytes, number of entries: 23
 -rw-r--r--  2.0 unx      172 b- defN 20-Mar-11 07:55 anticaptchaofficial/__init__.py
 -rw-r--r--  2.0 unx     1013 b- defN 23-Jan-07 03:37 anticaptchaofficial/antibotcookietask.py
 -rw-r--r--  2.0 unx     2720 b- defN 22-Sep-27 14:01 anticaptchaofficial/antigatetask.py
 -rw-r--r--  2.0 unx     6467 b- defN 22-Jun-01 07:45 anticaptchaofficial/antinetworking.py
 -rw-r--r--  2.0 unx     1149 b- defN 22-Jun-01 07:46 anticaptchaofficial/funcaptchaproxyless.py
 -rw-r--r--  2.0 unx     1430 b- defN 22-Jun-01 07:46 anticaptchaofficial/funcaptchaproxyon.py
 -rw-r--r--  2.0 unx     1619 b- defN 22-Jun-01 07:46 anticaptchaofficial/geetestproxyless.py
 -rw-r--r--  2.0 unx     1900 b- defN 22-Jun-01 07:46 anticaptchaofficial/geetestproxyon.py
 -rw-r--r--  2.0 unx     1215 b- defN 23-Apr-08 04:42 anticaptchaofficial/hcaptchaproxyless.py
--rw-r--r--  2.0 unx     1302 b- defN 22-Jun-01 07:46 anticaptchaofficial/hcaptchaproxyon.py
+-rw-r--r--  2.0 unx     1491 b- defN 23-Apr-14 03:41 anticaptchaofficial/hcaptchaproxyon.py
 -rw-r--r--  2.0 unx     1176 b- defN 22-Jun-01 07:46 anticaptchaofficial/imagecaptcha.py
 -rw-r--r--  2.0 unx      956 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav2enterpriseproxyless.py
 -rw-r--r--  2.0 unx     1278 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav2enterpriseproxyon.py
 -rw-r--r--  2.0 unx     1045 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav2proxyless.py
 -rw-r--r--  2.0 unx     1339 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav2proxyon.py
 -rw-r--r--  2.0 unx     1318 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav3enterpriseproxyless.py
 -rw-r--r--  2.0 unx     1270 b- defN 22-Jun-01 07:46 anticaptchaofficial/recaptchav3proxyless.py
 -rw-r--r--  2.0 unx      826 b- defN 22-Nov-02 07:37 anticaptchaofficial/turnstileproxyless.py
 -rw-r--r--  2.0 unx     1135 b- defN 22-Nov-02 07:37 anticaptchaofficial/turnstileproxyon.py
--rw-r--r--  2.0 unx     9673 b- defN 23-Apr-08 04:48 anticaptchaofficial-1.0.48.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-08 04:48 anticaptchaofficial-1.0.48.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 23-Apr-08 04:48 anticaptchaofficial-1.0.48.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2208 b- defN 23-Apr-08 04:48 anticaptchaofficial-1.0.48.dist-info/RECORD
-23 files, 41323 bytes uncompressed, 13456 bytes compressed:  67.4%
+-rw-r--r--  2.0 unx     9673 b- defN 23-Apr-14 03:43 anticaptchaofficial-1.0.49.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 03:43 anticaptchaofficial-1.0.49.dist-info/WHEEL
+-rw-r--r--  2.0 unx       20 b- defN 23-Apr-14 03:43 anticaptchaofficial-1.0.49.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2208 b- defN 23-Apr-14 03:43 anticaptchaofficial-1.0.49.dist-info/RECORD
+23 files, 41512 bytes uncompressed, 13488 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -51,20 +51,20 @@
 
 Filename: anticaptchaofficial/turnstileproxyless.py
 Comment: 
 
 Filename: anticaptchaofficial/turnstileproxyon.py
 Comment: 
 
-Filename: anticaptchaofficial-1.0.48.dist-info/METADATA
+Filename: anticaptchaofficial-1.0.49.dist-info/METADATA
 Comment: 
 
-Filename: anticaptchaofficial-1.0.48.dist-info/WHEEL
+Filename: anticaptchaofficial-1.0.49.dist-info/WHEEL
 Comment: 
 
-Filename: anticaptchaofficial-1.0.48.dist-info/top_level.txt
+Filename: anticaptchaofficial-1.0.49.dist-info/top_level.txt
 Comment: 
 
-Filename: anticaptchaofficial-1.0.48.dist-info/RECORD
+Filename: anticaptchaofficial-1.0.49.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## anticaptchaofficial/hcaptchaproxyon.py

```diff
@@ -1,13 +1,16 @@
 from anticaptchaofficial.antinetworking import *
 import time
 
 
 class hCaptchaProxyon(antiNetworking):
 
+    def get_user_agent(self):
+        return self.user_agent;
+
     def solve_and_return_solution(self):
         if self.create_task({
             "clientKey": self.client_key,
             "task": {
                 "type": "HCaptchaTask",
                 "websiteURL": self.website_url,
                 "websiteKey": self.website_key,
@@ -30,8 +33,10 @@
             return 0
         #checking result
         time.sleep(3)
         task_result = self.wait_for_result(300)
         if task_result == 0:
             return 0
         else:
+            if "userAgent" in task_result["solution"]:
+                self.user_agent = task_result["solution"]["userAgent"]
             return task_result["solution"]["gRecaptchaResponse"]
```

## Comparing `anticaptchaofficial-1.0.48.dist-info/METADATA` & `anticaptchaofficial-1.0.49.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anticaptchaofficial
-Version: 1.0.48
+Version: 1.0.49
 Summary: Official anti-captcha.com library
 Home-page: https://github.com/AdminAnticaptcha/anticaptcha-python
 Author: Anti Admin
 Author-email: admin@anti-captcha.com
 License: MIT
 Keywords: anticaptcha anti captcha recognition solve bypass recaptcha enterprise funcaptcha arkoselabs geetest hcaptcha antigate turnstile
 Platform: UNKNOWN
```

## Comparing `anticaptchaofficial-1.0.48.dist-info/RECORD` & `anticaptchaofficial-1.0.49.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 anticaptchaofficial/antigatetask.py,sha256=A9yzevmMuyXiH6Ixlu_bcxxzvp4MLQpl3DwFNXU_Gek,2720
 anticaptchaofficial/antinetworking.py,sha256=4sxfJ2Yv36I215qR8Aw2fVtmDjdr8ggKrFKUCbXuzEQ,6467
 anticaptchaofficial/funcaptchaproxyless.py,sha256=5ORFsWFo_xZK1TRpBnP2R1ELkyG3HsBuyqKb88fmGls,1149
 anticaptchaofficial/funcaptchaproxyon.py,sha256=7LNgSSAvNfdeDUXEtZrOdjY5iYVgvq3ocxIzgNx_5Ac,1430
 anticaptchaofficial/geetestproxyless.py,sha256=ggfg6PcTlPO6Ri9vsO9nZ_23d9rFvUapWjzi-cUojFk,1619
 anticaptchaofficial/geetestproxyon.py,sha256=q6YVGLc3IIPzhzCVx_ayLujTFVej1h3rvaX2KNWKXBQ,1900
 anticaptchaofficial/hcaptchaproxyless.py,sha256=3YPVqMlLUUJR0bXDtfwFwyWkPR054smwKoSvDp10DvE,1215
-anticaptchaofficial/hcaptchaproxyon.py,sha256=OOmM0cLcqnB4r536uB3xe37O4Gi1WLNkJTiNhZzbSvI,1302
+anticaptchaofficial/hcaptchaproxyon.py,sha256=6aBwVWBqS1hGS6h0P95QMFW3EAOgidFjq-s8v3ZQm3I,1491
 anticaptchaofficial/imagecaptcha.py,sha256=aKupUYdeNjuQanbY4aI8TuK6uty32e8XzP0Uzg3RL7I,1176
 anticaptchaofficial/recaptchav2enterpriseproxyless.py,sha256=XnDx-6-KsETqXySaT0RDWtuh-9Sk3gSWy2rF8Jy1gLk,956
 anticaptchaofficial/recaptchav2enterpriseproxyon.py,sha256=p7sdV0qHScbrIrhw00624pH_2hQeG95RTGjRQDutxs4,1278
 anticaptchaofficial/recaptchav2proxyless.py,sha256=12fviOgw1waeeRbyzwvSctIoc1w3qCBYJY7GYi0FSJc,1045
 anticaptchaofficial/recaptchav2proxyon.py,sha256=KKjm72dfxdCChyj3Qn5y5Twm8qT3sZsvSGSfjbdrIM8,1339
 anticaptchaofficial/recaptchav3enterpriseproxyless.py,sha256=exQ-sgvOdcSpsh0mWsUDKEGudM4k23SrROVZ9p0pU5M,1318
 anticaptchaofficial/recaptchav3proxyless.py,sha256=Fv0nfDG-Jp8Vzz8C4-vccz3BJ0hm89MTAs3y9Okzctw,1270
 anticaptchaofficial/turnstileproxyless.py,sha256=k12CETrs6iRhZj3shXrOZrCf8EBvFodXcRa3N6rXKJU,826
 anticaptchaofficial/turnstileproxyon.py,sha256=6yx5EBxQgi2m4yfvkichbZNB87xMg9LveApeKYVLkII,1135
-anticaptchaofficial-1.0.48.dist-info/METADATA,sha256=Z1MGg4uSpFriOqjOZrgEQa3vozh-MJlR9IfacrIJvNI,9673
-anticaptchaofficial-1.0.48.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-anticaptchaofficial-1.0.48.dist-info/top_level.txt,sha256=lLc0em6A2B5BH-M8v9OP54jTh3u65A4xb2trGoI2_5A,20
-anticaptchaofficial-1.0.48.dist-info/RECORD,,
+anticaptchaofficial-1.0.49.dist-info/METADATA,sha256=P9V50kSHTVatlsw54bFXUcoTBmm3sfsTSblBbpHNsJk,9673
+anticaptchaofficial-1.0.49.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+anticaptchaofficial-1.0.49.dist-info/top_level.txt,sha256=lLc0em6A2B5BH-M8v9OP54jTh3u65A4xb2trGoI2_5A,20
+anticaptchaofficial-1.0.49.dist-info/RECORD,,
```

