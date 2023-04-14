# Comparing `tmp/commit_check-0.5.5-py3-none-any.whl.zip` & `tmp/commit_check-0.5.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 11183 bytes, number of entries: 13
--rw-r--r--  2.0 unx     1735 b- defN 23-Apr-12 06:50 commit_check/__init__.py
--rw-r--r--  2.0 unx     1117 b- defN 23-Apr-12 06:50 commit_check/author.py
--rw-r--r--  2.0 unx      926 b- defN 23-Apr-12 06:50 commit_check/branch.py
--rw-r--r--  2.0 unx     1508 b- defN 23-Apr-12 06:50 commit_check/commit.py
--rw-r--r--  2.0 unx     2675 b- defN 23-Apr-12 06:50 commit_check/error.py
--rw-r--r--  2.0 unx     2919 b- defN 23-Apr-12 06:50 commit_check/main.py
--rw-r--r--  2.0 unx     4748 b- defN 23-Apr-12 06:50 commit_check/util.py
--rw-r--r--  2.0 unx     1095 b- defN 23-Apr-12 06:51 commit_check-0.5.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     8716 b- defN 23-Apr-12 06:51 commit_check-0.5.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-12 06:51 commit_check-0.5.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       56 b- defN 23-Apr-12 06:51 commit_check-0.5.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       13 b- defN 23-Apr-12 06:51 commit_check-0.5.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1060 b- defN 23-Apr-12 06:51 commit_check-0.5.5.dist-info/RECORD
-13 files, 26660 bytes uncompressed, 9413 bytes compressed:  64.7%
+Zip file size: 11194 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     1735 b- defN 23-Apr-14 08:47 commit_check/__init__.py
+-rw-r--r--  2.0 unx     1117 b- defN 23-Apr-14 08:47 commit_check/author.py
+-rw-r--r--  2.0 unx      926 b- defN 23-Apr-14 08:47 commit_check/branch.py
+-rw-r--r--  2.0 unx     1637 b- defN 23-Apr-14 08:47 commit_check/commit.py
+-rw-r--r--  2.0 unx     2675 b- defN 23-Apr-14 08:47 commit_check/error.py
+-rw-r--r--  2.0 unx     2919 b- defN 23-Apr-14 08:47 commit_check/main.py
+-rw-r--r--  2.0 unx     4748 b- defN 23-Apr-14 08:47 commit_check/util.py
+-rw-r--r--  2.0 unx     1095 b- defN 23-Apr-14 08:48 commit_check-0.5.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8716 b- defN 23-Apr-14 08:48 commit_check-0.5.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-14 08:48 commit_check-0.5.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       56 b- defN 23-Apr-14 08:48 commit_check-0.5.6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       13 b- defN 23-Apr-14 08:48 commit_check-0.5.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1060 b- defN 23-Apr-14 08:48 commit_check-0.5.6.dist-info/RECORD
+13 files, 26789 bytes uncompressed, 9424 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: commit_check/main.py
 Comment: 
 
 Filename: commit_check/util.py
 Comment: 
 
-Filename: commit_check-0.5.5.dist-info/LICENSE
+Filename: commit_check-0.5.6.dist-info/LICENSE
 Comment: 
 
-Filename: commit_check-0.5.5.dist-info/METADATA
+Filename: commit_check-0.5.6.dist-info/METADATA
 Comment: 
 
-Filename: commit_check-0.5.5.dist-info/WHEEL
+Filename: commit_check-0.5.6.dist-info/WHEEL
 Comment: 
 
-Filename: commit_check-0.5.5.dist-info/entry_points.txt
+Filename: commit_check-0.5.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: commit_check-0.5.5.dist-info/top_level.txt
+Filename: commit_check-0.5.6.dist-info/top_level.txt
 Comment: 
 
-Filename: commit_check-0.5.5.dist-info/RECORD
+Filename: commit_check-0.5.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## commit_check/commit.py

```diff
@@ -21,14 +21,17 @@
                 commit_msg_file = PurePath(git_dir, "COMMIT_EDITMSG")
                 try:
                     with open(commit_msg_file, 'r') as f:
                         commit_msg = f.read()
                 except FileNotFoundError:
                     # check the message of the last commit
                     commit_msg = str(get_commits_info("s"))
+            else:
+                # check the message of the last commit
+                commit_msg = str(get_commits_info("s"))
             result = re.match(check['regex'], commit_msg)
             if result is None:
                 print_error_message(
                     check['check'], check['regex'],
                     check['error'], commit_msg,
                 )
                 if check['suggest']:
```

## Comparing `commit_check-0.5.5.dist-info/LICENSE` & `commit_check-0.5.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `commit_check-0.5.5.dist-info/METADATA` & `commit_check-0.5.6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commit-check
-Version: 0.5.5
+Version: 0.5.6
 Summary: Check commit message formatting, branch naming, commit author, email, and more.
 Author-email: Peter Shen <xianpeng.shen@gmail.com>
 License: MIT License
 Project-URL: source, https://github.com/commit-check/commit-check
 Project-URL: tracker, https://github.com/commit-check/commit-check/issues
 Keywords: commit conventions,conventional commits,branch naming,commit-check,message,lint message
 Classifier: Development Status :: 4 - Beta
```

## Comparing `commit_check-0.5.5.dist-info/RECORD` & `commit_check-0.5.6.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 commit_check/__init__.py,sha256=kTDjVl3aBz6rp3HHv10dhOm7B1_ZmTMHzNg_0earx0k,1735
 commit_check/author.py,sha256=Vo642jgwY_4Y9Ea48dFd_Dvfr5uzzBW9yVNTETFHnCA,1117
 commit_check/branch.py,sha256=4Vt5qf3NniQdMA5x19kE3xLClyLDGFKRZhP_veXn7y0,926
-commit_check/commit.py,sha256=rlpj1cYArAGLyDGd_2cNBPJ2_q7cVi5DcGDcbI34ig8,1508
+commit_check/commit.py,sha256=YTagvxFV9fl20GG9-weO9k0usFc1vEvawDA4KTxZ-ps,1637
 commit_check/error.py,sha256=z3WQRKII6WPqEBgBQVeclg8AYqwr4lqX1ssQs3bKZLQ,2675
 commit_check/main.py,sha256=mSC05heXp0ZDGWT-yQKVa8WyuXVAnwO0aRN7xs51P5I,2919
 commit_check/util.py,sha256=bWnRFp7G-OBBxEmn_xe0laVbFEJzOMPAcclIZKITROU,4748
-commit_check-0.5.5.dist-info/LICENSE,sha256=VAJ9TE1ov8aUKmeoBRYqciMs0CXag1TeDCoLhwbeQmA,1095
-commit_check-0.5.5.dist-info/METADATA,sha256=gLGis6SlOee2ds4cke1aWuzLzW5-emZeWYMJiC93nP4,8716
-commit_check-0.5.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-commit_check-0.5.5.dist-info/entry_points.txt,sha256=2IMogDXLAFnwmH_-_EFBwYixY9sTvcwxze59OFs8ybA,56
-commit_check-0.5.5.dist-info/top_level.txt,sha256=Wf46u-ooHBMJNHbhfrBNQw3wC5_m8wt-o_Lfbc4QpRg,13
-commit_check-0.5.5.dist-info/RECORD,,
+commit_check-0.5.6.dist-info/LICENSE,sha256=VAJ9TE1ov8aUKmeoBRYqciMs0CXag1TeDCoLhwbeQmA,1095
+commit_check-0.5.6.dist-info/METADATA,sha256=P9sVoAJB5BU3WLiTVAWYpXSVG_ZSABaLQc3tXH-dsa4,8716
+commit_check-0.5.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+commit_check-0.5.6.dist-info/entry_points.txt,sha256=2IMogDXLAFnwmH_-_EFBwYixY9sTvcwxze59OFs8ybA,56
+commit_check-0.5.6.dist-info/top_level.txt,sha256=Wf46u-ooHBMJNHbhfrBNQw3wC5_m8wt-o_Lfbc4QpRg,13
+commit_check-0.5.6.dist-info/RECORD,,
```

