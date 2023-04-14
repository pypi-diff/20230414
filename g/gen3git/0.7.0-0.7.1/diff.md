# Comparing `tmp/gen3git-0.7.0.tar.gz` & `tmp/gen3git-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen3git-0.7.0.tar", last modified: Mon Jan 30 15:28:10 2023, max compression
+gzip compressed data, was "gen3git-0.7.1.tar", last modified: Fri Apr 14 18:24:26 2023, max compression
```

## Comparing `gen3git-0.7.0.tar` & `gen3git-0.7.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-30 15:28:10.369669 gen3git-0.7.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-01-30 15:27:22.000000 gen3git-0.7.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2023-01-30 15:27:22.000000 gen3git-0.7.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      558 2023-01-30 15:27:22.000000 gen3git-0.7.0/NOTICE
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-01-30 15:28:10.365666 gen3git-0.7.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      177 2023-01-30 15:27:22.000000 gen3git-0.7.0/Pipfile
--rw-r--r--   0 travis    (2000) travis    (2000)    25450 2023-01-30 15:27:35.000000 gen3git-0.7.0/Pipfile.lock
--rw-rw-r--   0 travis    (2000) travis    (2000)     1716 2023-01-30 15:27:22.000000 gen3git-0.7.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-01-30 15:28:10.365666 gen3git-0.7.0/gen3git.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-01-30 15:28:10.000000 gen3git-0.7.0/gen3git.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      265 2023-01-30 15:28:10.000000 gen3git-0.7.0/gen3git.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-01-30 15:28:10.000000 gen3git-0.7.0/gen3git.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       41 2023-01-30 15:28:10.000000 gen3git-0.7.0/gen3git.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2023-01-30 15:28:10.000000 gen3git-0.7.0/gen3git.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-01-30 15:28:10.000000 gen3git-0.7.0/gen3git.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    19928 2023-01-30 15:27:22.000000 gen3git-0.7.0/gen3git.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-01-30 15:28:10.369669 gen3git-0.7.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      928 2023-01-30 15:27:55.000000 gen3git-0.7.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-14 18:24:26.822392 gen3git-0.7.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11357 2023-04-14 18:23:33.000000 gen3git-0.7.1/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       68 2023-04-14 18:23:33.000000 gen3git-0.7.1/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      558 2023-04-14 18:23:33.000000 gen3git-0.7.1/NOTICE
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-04-14 18:24:26.818390 gen3git-0.7.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      177 2023-04-14 18:23:33.000000 gen3git-0.7.1/Pipfile
+-rw-r--r--   0 travis    (2000) travis    (2000)    27222 2023-04-14 18:23:48.000000 gen3git-0.7.1/Pipfile.lock
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1716 2023-04-14 18:23:33.000000 gen3git-0.7.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2023-04-14 18:24:26.818390 gen3git-0.7.1/gen3git.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2023-04-14 18:24:26.000000 gen3git-0.7.1/gen3git.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)      265 2023-04-14 18:24:26.000000 gen3git-0.7.1/gen3git.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2023-04-14 18:24:26.000000 gen3git-0.7.1/gen3git.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       41 2023-04-14 18:24:26.000000 gen3git-0.7.1/gen3git.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       60 2023-04-14 18:24:26.000000 gen3git-0.7.1/gen3git.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        8 2023-04-14 18:24:26.000000 gen3git-0.7.1/gen3git.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20714 2023-04-14 18:23:33.000000 gen3git-0.7.1/gen3git.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2023-04-14 18:24:26.822392 gen3git-0.7.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      928 2023-04-14 18:24:10.000000 gen3git-0.7.1/setup.py
```

### Comparing `gen3git-0.7.0/LICENSE` & `gen3git-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gen3git-0.7.0/NOTICE` & `gen3git-0.7.1/NOTICE`

 * *Files identical despite different names*

### Comparing `gen3git-0.7.0/README.md` & `gen3git-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `gen3git-0.7.0/gen3git.py` & `gen3git-0.7.1/gen3git.py`

 * *Files 6% similar despite different names*

```diff
@@ -349,18 +349,21 @@
     desc_bodies = []
     # add 1 second to the start date because the start commit should
     # be excluded from the result:
     start_date = start_tag.commit.commit.author.date + timedelta(0, 1)
     stop_date = datetime.utcnow()
 
     # If dates are specified by the user, they override dates from tags/commits
-    if hasattr(args, "from_date") and args.from_date is not None:
-        start_date = datetime.strptime(args.from_date, "%Y-%m-%d")
-    if hasattr(args, "to_date") and args.to_date is not None:
-        stop_date = datetime.strptime(args.to_date, "%Y-%m-%d")
+    from_date = getattr(args, "from_date", None)
+    if from_date:
+        start_date = datetime.strptime(from_date, "%Y-%m-%d")
+    to_date = getattr(args, "to_date", None)
+    if to_date:
+        stop_date = datetime.strptime(to_date, "%Y-%m-%d")
+    print("Start date: %s; Stop date: %s" % (start_date, stop_date))
 
     # TODO: Revisit this whole logic to adopt proper githubapi requests
     # instead of this `branch_commits` approach that is not compatible with private repos. See ticket PXP-7714
     # Skipping private repos for now
     private_check = requests.get(
         "https://api.github.com/repos/%s" % (uri),
         headers=headers,
@@ -381,15 +384,30 @@
             hasattr(args, "release_tag"),
             getattr(args, "markdown", False),
             getattr(args, "html", False),
         ]
     ):
         output_type = "text"
 
-    for commit in repo.get_commits(since=start_date, until=stop_date):
+    if not to_tag:
+        # get the commits on master branch
+        commits = repo.get_commits(since=start_date, until=stop_date)
+    else:
+        # only get the commits that are included in the specified tag.
+        # handles edge case when the tag includes a recent commit and `stop_date` is more recent
+        # than some master branch commits that should not be included. Example:
+        # - master branch commits:
+        #     01/20: commit2 (not in tag) <-------------------- should not be included
+        #     01/01: commit1 (in tag)
+        # - tag commits:
+        #     01/25: merge commit or cherry-pick commit <------ `stop_date` = 01/25
+        #     01/01: commit1
+        commits = repo.get_commits(since=start_date, until=stop_date, sha=to_tag)
+
+    for commit in commits:
         # https://platform.github.community/t/get-pull-request-associated-with-merge-commit/6936
         # https://github.blog/2014-10-13-linking-merged-pull-requests-from-commits/
         # We are not using the search API because its rate limit is too low.
         # This doesn't work for private repos, and we can't attach headers
         # because it's not a GitHub API endpoint. See ticket PXP-7714
         resp = requests.get(
             "https://github.com/%s/branch_commits/%s" % (uri, commit.sha)
```

### Comparing `gen3git-0.7.0/setup.py` & `gen3git-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,14 +16,14 @@
             "distribution; please either download the source from PyPI, or check out "
             "from GitHub and make sure that the git CLI is available."
         )
 
 
 setup(
     name="gen3git",
-    version='0.7.0',
+    version='0.7.1',
     description="Helps with release.",
     license="Apache",
     py_modules=["gen3git"],
     install_requires=['enum;python_version<"3.4"', "PyGithub", "requests", "gitpython"],
     entry_points={"console_scripts": ["gen3git=gen3git:main"]},
 )
```

