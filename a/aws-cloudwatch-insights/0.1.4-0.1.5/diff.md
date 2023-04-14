# Comparing `tmp/aws_cloudwatch_insights-0.1.4.tar.gz` & `tmp/aws_cloudwatch_insights-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aws_cloudwatch_insights-0.1.4.tar", last modified: Fri Mar  3 20:00:45 2023, max compression
+gzip compressed data, was "dist/aws_cloudwatch_insights-0.1.5.tar", last modified: Fri Apr 14 20:13:02 2023, max compression
```

## Comparing `aws_cloudwatch_insights-0.1.4.tar` & `aws_cloudwatch_insights-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:00:45.000000 aws_cloudwatch_insights-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-03 20:00:37.000000 aws_cloudwatch_insights-0.1.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-03-03 20:00:45.000000 aws_cloudwatch_insights-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-03-03 20:00:37.000000 aws_cloudwatch_insights-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:00:45.000000 aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-03 20:00:37.000000 aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-03-03 20:00:37.000000 aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights/aws_cloudwatch_insights.py
--rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-03-03 20:00:37.000000 aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 20:00:45.000000 aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8089 2023-03-03 20:00:45.000000 aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-03 20:00:45.000000 aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 20:00:45.000000 aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-03 20:00:45.000000 aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 20:00:45.000000 aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-03 20:00:45.000000 aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-03 20:00:45.000000 aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-03 20:00:45.000000 aws_cloudwatch_insights-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-03-03 20:00:37.000000 aws_cloudwatch_insights-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:13:02.000000 aws_cloudwatch_insights-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-14 20:12:52.000000 aws_cloudwatch_insights-0.1.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-04-14 20:13:02.000000 aws_cloudwatch_insights-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4652 2023-04-14 20:12:52.000000 aws_cloudwatch_insights-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:13:02.000000 aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-14 20:12:52.000000 aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-04-14 20:12:52.000000 aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights/aws_cloudwatch_insights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9735 2023-04-14 20:12:52.000000 aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:13:02.000000 aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6925 2023-04-14 20:13:01.000000 aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-04-14 20:13:02.000000 aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:13:01.000000 aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-14 20:13:01.000000 aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:13:01.000000 aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-14 20:13:01.000000 aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-14 20:13:01.000000 aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-14 20:13:02.000000 aws_cloudwatch_insights-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-14 20:12:52.000000 aws_cloudwatch_insights-0.1.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-14 20:12:52.000000 aws_cloudwatch_insights-0.1.5/version.txt
```

### Comparing `aws_cloudwatch_insights-0.1.4/PKG-INFO` & `aws_cloudwatch_insights-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,217 +1,191 @@
 Metadata-Version: 2.1
 Name: aws_cloudwatch_insights
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library and cli for querying AWS Cloudwatch Insights
 Home-page: https://github.com/valmikirao/aws_cloudwatch_insights
 Author: Valmiki Rao
 Author-email: valmikirao@gmail.com
 License: MIT license
-Description: 
-        AWS Cloudwatch Insights
-        =======================
-        
-        
-        .. image:: https://img.shields.io/pypi/v/aws_cloudwatch_insights
-           :target: https://img.shields.io/pypi/v/aws_cloudwatch_insights
-           :alt: version
-        
-        
-        .. image:: https://img.shields.io/pypi/pyversions/aws_cloudwatch_insights
-           :target: https://img.shields.io/pypi/pyversions/aws_cloudwatch_insights
-           :alt: python versions
-        
-        
-        .. image:: https://img.shields.io/github/actions/workflow/status/valmikirao/aws_cloudwatch_insights/push-workflow.yml?branch=master
-           :target: https://img.shields.io/github/actions/workflow/status/valmikirao/aws_cloudwatch_insights/push-workflow.yml?branch=master
-           :alt: build
+Description: # AWS Cloudwatch Insights
         
+        ![version](https://img.shields.io/pypi/v/aws_cloudwatch_insights)
+        ![python versions](https://img.shields.io/pypi/pyversions/aws_cloudwatch_insights)
+        ![build](https://img.shields.io/github/actions/workflow/status/valmikirao/aws_cloudwatch_insights/push-workflow.yml?branch=master)
         
         Both a command line tool and a python API to simplify interacting with AWS cloudwatch insights
         
-        CLI
-        ---
-        
-        Installation
-        ^^^^^^^^^^^^
-        
-        .. code-block:: shell
+        ## CLI
         
-           # globally
-           $ pipx install 'aws_cloudwatch_insights[cli]'
-           # or in a particular virtual env
-           $ pip install 'aws_cloudwatch_insights[cli]'
+        ### Installation
         
-        Usage
-        ^^^^^
+        ```shell
+        # globally
+        $ pipx install 'aws_cloudwatch_insights[cli]'
+        # or in a particular virtual env
+        $ pip install 'aws_cloudwatch_insights[cli]'
+        ```
         
-        Run via the ``acwi`` command.  Results returned in json.
+        ### Usage
         
-        It takes either a file of AWS Inisghts code or a yaml file with a ``query`` argument and other options.
+        Run via the `acwi` command.  Results returned in json.
         
-        For example, if file ``acwi.acwi`` contained this:
+        It takes either a file of AWS Inisghts code or a yaml file with a `query` argument and other options.
         
-        .. code-block::
+        For example, if file `acwi.acwi` contained this:
         
-           fields @timestamp, @message, @logStream, @log
-           | sort @timestamp desc
-           | limit 20
+        ```
+        fields @timestamp, @message, @logStream, @log
+        | sort @timestamp desc
+        | limit 20
+        ```
         
         And you ran this:
         
-        .. code-block:: shell
-        
-           $ acwi --group-names /aws/lambda/log_maker --region us-west-2 --start -30d tmp/acwi.acwi --out results.json
+        ```shell
+        $ acwi --group-names /aws/lambda/log_maker --region us-west-2 --start -30d tmp/acwi.acwi --out results.json
+        ```
         
         It would run the query against the stated log group in the stated region from 30 days ago.
         
-        Alternatively, if you had a file ``acwi.yml`` containing this:
-        
-        .. code-block:: yaml
+        Alternatively, if you had a file `acwi.yml` containing this:
         
-           query: |
-            fields @timestamp, @message, @logStream, @log
-            | sort @timestamp desc
-            | limit 20
-           groups:
-             - /aws/lambda/log_maker
-           region: us-west-2
-           start: -30d
-           out_file: results.json
+        ```yaml
+        query: |
+         fields @timestamp, @message, @logStream, @log
+         | sort @timestamp desc
+         | limit 20
+        groups:
+          - /aws/lambda/log_maker
+        region: us-west-2
+        start: -30d
+        out_file: results.json
+        ```
         
         And running this:
         
-        .. code-block:: shell
-        
-           $ acwi acwi.yml
+        ```shell
+        $ acwi acwi.yml
+        ```
         
         You would get the same result.
         
         If an option is on both the command line of in the .yml file, the command line overrides the value in the file.
         
-        There is some fancy partial results returned as the query runs.  You can shut these off using the ``--quiet`` option.
-        
-        API
-        ---
+        There is some fancy partial results returned as the query runs.  You can shut these off using the `--quiet` option.
         
-        If you're only using the api, you don't need to install with the ``[cli]`` extras.
+        ## API
         
-        .. code-block:: shell
+        If you're only using the api, you don't need to install with the `[cli]` extras.
         
-           $ pip install aws_cloudwatch_insights
+        ```shell
+        $ pip install aws_cloudwatch_insights
+        ```
         
-        Usage
-        -----
+        ## Usage
         
-        Examples
-        ^^^^^^^^
+        ### Examples
         
-        .. code-block:: python
+        ```python
+        from aws_cloudwatch_insights import Insights
+        from datetime import timedelta
         
-           from aws_cloudwatch_insights import Insights
-           from datetime import timedelta
+        insights = Insights()
+        query = """
+        fields @timestamp, @message, @logStream, @log
+        | sort @timestamp desc
+        | limit 20
+        """
         
-           insights = Insights()
-           query = """
-           fields @timestamp, @message, @logStream, @log
-           | sort @timestamp desc
-           | limit 20
-           """
+        results = insights.get_insights(
+            query, group_names=["/aws/lambda/log_maker"], result_limit=20,
+            start_time=-timedelta(days=1)
+        )
         
-           results = insights.get_insights(
-               query, group_names=["/aws/lambda/log_maker"], result_limit=20,
-               start_time=-timedelta(days=1)
-           )
+        ```
         
-        Reference
-        ^^^^^^^^^
+        ### Reference
         
         From the inline documentation:
         
-        .. code-block:: python
+        ```python
+        class Insights:
+            def __init__(self, logs_client: Optional[BaseClient] = None):
+                """
+                Object for querying AWS Cloudwatch.  Optionally takes a boto3 client as an argument, otherwise creates its own
+                """
+                ...
+        
+            def get_insights(self, query: str, result_limit: int, group_names: List[str], start_time: Union[int, datetime, timedelta],
+                             end_time: Union[int, datetime, timedelta, None] = None, callback: Optional[CallbackFunction] = None,
+                             error: Optional[ErrorFunction] = None, jsonify: bool = True) -> Iterable[GenericDict]:
+                """
+                Gets elements from AWS Cloudwatch Logs using an Insights query:
+        
+                Returns an iterable of dicts
+        
+                query: The Insights query
+                result_limit: Limit of the number of results returned
+                group_names: The log groups searched through
+                start_time: The time of the earliest record the query looks for.  Can be an int timestamp, a datetime, or a
+                 timedelta.  If it's a timedelta, the start time is now offset by the delta
+                end_time: The time of the latest record the query looks for.  Accepts same values as `start_time`
+                callback: A function witch is called when partial results are returned, before the function returns the final
+                    results.  Takes the partial results as an argument.
+                error: If included, this function is called when an exception is encountered (instead of not catching the
+                  exception).  The arguments passed to the function are the Exception instance and the partial results.  If
+                  this function doesn't through an exception, get_insights() returns the returned value of this function, empty
+                  list if that value is None
+                jsonify: If set to True, attempts to parse suspected json objects.  If parsing fails, just returns the string.
+                  Default: True
+                """
+                ...
+        ```
+        
+        ## Development
+        
+        Requires make:
+        
+        ```shell
+        # setting up dev environment
+        $ make develop
+        
+        # run tests
+        $ make test
+        # ... or
+        $ pytest
         
-           class Insights:
-               def __init__(self, logs_client: Optional[BaseClient] = None):
-                   """
-                   Object for querying AWS Cloudwatch.  Optionally takes a boto3 client as an argument, otherwise creates its own
-                   """
-                   ...
-        
-               def get_insights(self, query: str, result_limit: int, group_names: List[str], start_time: Union[int, datetime, timedelta],
-                                end_time: Union[int, datetime, timedelta, None] = None, callback: Optional[CallbackFunction] = None,
-                                error: Optional[ErrorFunction] = None, jsonify: bool = True) -> Iterable[GenericDict]:
-                   """
-                   Gets elements from AWS Cloudwatch Logs using an Insights query:
-        
-                   Returns an iterable of dicts
-        
-                   query: The Insights query
-                   result_limit: Limit of the number of results returned
-                   group_names: The log groups searched through
-                   start_time: The time of the earliest record the query looks for.  Can be an int timestamp, a datetime, or a
-                    timedelta.  If it's a timedelta, the start time is now offset by the delta
-                   end_time: The time of the latest record the query looks for.  Accepts same values as `start_time`
-                   callback: A function witch is called when partial results are returned, before the function returns the final
-                       results.  Takes the partial results as an argument.
-                   error: If included, this function is called when an exception is encountered (instead of not catching the
-                     exception).  The arguments passed to the function are the Exception instance and the partial results.  If
-                     this function doesn't through an exception, get_insights() returns the returned value of this function, empty
-                     list if that value is None
-                   jsonify: If set to True, attempts to parse suspected json objects.  If parsing fails, just returns the string.
-                     Default: True
-                   """
-                   ...
-        
-        Development
-        -----------
-        
-        Requires make, docker, and docker-compose:
-        
-        .. code-block:: shell
-        
-           # setting up dev environment
-           $ make develop
-        
-           # run tests
-           $ make test
-           # ... or
-           $ pytest
-        
-           # run tests for all environments
-           $ make test-all
-           $ make test-all-build  # checks to see if images need rebuilding
-           # ... you can use the underlying script to pass args to docker-compose directly:
-           $ ./scripts/run_tests_all.sh --build py36-no-cli py37  # runs for python 3.7 and python 3.6 with no cli
+        # run tests for all environments
+        $ make test-all
         
-        No CI/CD or coverage yet
-        
-        To Do
-        -----
+        ```
         
+        No CI/CD or coverage yet
         
+        ## To Do
         * If someone tells me they actually use this, I'll bump it to v1.0.0
         * More extensive CLI unit tests
-        * ``--csv`` output option
+        * `--csv` output option
         * Integration tests
         
-        Credits
-        -------
+        ## Credits
         
-        This package was created with *cookiecutter* and the ``audreyr/cookiecutter-pypackage`` project template.
+        This package was created with _cookiecutter_ and the `audreyr/cookiecutter-pypackage` project template.
         
 Keywords: aws,cloudwatch,insights
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 Provides-Extra: cli
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: types
```

### Comparing `aws_cloudwatch_insights-0.1.4/README.md` & `aws_cloudwatch_insights-0.1.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -131,30 +131,27 @@
           Default: True
         """
         ...
 ```
 
 ## Development
 
-Requires make, docker, and docker-compose:
+Requires make:
 
 ```shell
 # setting up dev environment
 $ make develop
 
 # run tests
 $ make test
 # ... or
 $ pytest
 
 # run tests for all environments
 $ make test-all
-$ make test-all-build  # checks to see if images need rebuilding
-# ... you can use the underlying script to pass args to docker-compose directly:
-$ ./scripts/run_tests_all.sh --build py36-no-cli py37  # runs for python 3.7 and python 3.6 with no cli
 
 ```
 
 No CI/CD or coverage yet
 
 ## To Do
 * If someone tells me they actually use this, I'll bump it to v1.0.0
```

### Comparing `aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights/aws_cloudwatch_insights.py` & `aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights/aws_cloudwatch_insights.py`

 * *Files identical despite different names*

### Comparing `aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights/cli.py` & `aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights/cli.py`

 * *Files identical despite different names*

### Comparing `aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights.egg-info/PKG-INFO` & `aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,217 +1,191 @@
 Metadata-Version: 2.1
 Name: aws-cloudwatch-insights
-Version: 0.1.4
+Version: 0.1.5
 Summary: Library and cli for querying AWS Cloudwatch Insights
 Home-page: https://github.com/valmikirao/aws_cloudwatch_insights
 Author: Valmiki Rao
 Author-email: valmikirao@gmail.com
 License: MIT license
-Description: 
-        AWS Cloudwatch Insights
-        =======================
-        
-        
-        .. image:: https://img.shields.io/pypi/v/aws_cloudwatch_insights
-           :target: https://img.shields.io/pypi/v/aws_cloudwatch_insights
-           :alt: version
-        
-        
-        .. image:: https://img.shields.io/pypi/pyversions/aws_cloudwatch_insights
-           :target: https://img.shields.io/pypi/pyversions/aws_cloudwatch_insights
-           :alt: python versions
-        
-        
-        .. image:: https://img.shields.io/github/actions/workflow/status/valmikirao/aws_cloudwatch_insights/push-workflow.yml?branch=master
-           :target: https://img.shields.io/github/actions/workflow/status/valmikirao/aws_cloudwatch_insights/push-workflow.yml?branch=master
-           :alt: build
+Description: # AWS Cloudwatch Insights
         
+        ![version](https://img.shields.io/pypi/v/aws_cloudwatch_insights)
+        ![python versions](https://img.shields.io/pypi/pyversions/aws_cloudwatch_insights)
+        ![build](https://img.shields.io/github/actions/workflow/status/valmikirao/aws_cloudwatch_insights/push-workflow.yml?branch=master)
         
         Both a command line tool and a python API to simplify interacting with AWS cloudwatch insights
         
-        CLI
-        ---
-        
-        Installation
-        ^^^^^^^^^^^^
-        
-        .. code-block:: shell
+        ## CLI
         
-           # globally
-           $ pipx install 'aws_cloudwatch_insights[cli]'
-           # or in a particular virtual env
-           $ pip install 'aws_cloudwatch_insights[cli]'
+        ### Installation
         
-        Usage
-        ^^^^^
+        ```shell
+        # globally
+        $ pipx install 'aws_cloudwatch_insights[cli]'
+        # or in a particular virtual env
+        $ pip install 'aws_cloudwatch_insights[cli]'
+        ```
         
-        Run via the ``acwi`` command.  Results returned in json.
+        ### Usage
         
-        It takes either a file of AWS Inisghts code or a yaml file with a ``query`` argument and other options.
+        Run via the `acwi` command.  Results returned in json.
         
-        For example, if file ``acwi.acwi`` contained this:
+        It takes either a file of AWS Inisghts code or a yaml file with a `query` argument and other options.
         
-        .. code-block::
+        For example, if file `acwi.acwi` contained this:
         
-           fields @timestamp, @message, @logStream, @log
-           | sort @timestamp desc
-           | limit 20
+        ```
+        fields @timestamp, @message, @logStream, @log
+        | sort @timestamp desc
+        | limit 20
+        ```
         
         And you ran this:
         
-        .. code-block:: shell
-        
-           $ acwi --group-names /aws/lambda/log_maker --region us-west-2 --start -30d tmp/acwi.acwi --out results.json
+        ```shell
+        $ acwi --group-names /aws/lambda/log_maker --region us-west-2 --start -30d tmp/acwi.acwi --out results.json
+        ```
         
         It would run the query against the stated log group in the stated region from 30 days ago.
         
-        Alternatively, if you had a file ``acwi.yml`` containing this:
-        
-        .. code-block:: yaml
+        Alternatively, if you had a file `acwi.yml` containing this:
         
-           query: |
-            fields @timestamp, @message, @logStream, @log
-            | sort @timestamp desc
-            | limit 20
-           groups:
-             - /aws/lambda/log_maker
-           region: us-west-2
-           start: -30d
-           out_file: results.json
+        ```yaml
+        query: |
+         fields @timestamp, @message, @logStream, @log
+         | sort @timestamp desc
+         | limit 20
+        groups:
+          - /aws/lambda/log_maker
+        region: us-west-2
+        start: -30d
+        out_file: results.json
+        ```
         
         And running this:
         
-        .. code-block:: shell
-        
-           $ acwi acwi.yml
+        ```shell
+        $ acwi acwi.yml
+        ```
         
         You would get the same result.
         
         If an option is on both the command line of in the .yml file, the command line overrides the value in the file.
         
-        There is some fancy partial results returned as the query runs.  You can shut these off using the ``--quiet`` option.
-        
-        API
-        ---
+        There is some fancy partial results returned as the query runs.  You can shut these off using the `--quiet` option.
         
-        If you're only using the api, you don't need to install with the ``[cli]`` extras.
+        ## API
         
-        .. code-block:: shell
+        If you're only using the api, you don't need to install with the `[cli]` extras.
         
-           $ pip install aws_cloudwatch_insights
+        ```shell
+        $ pip install aws_cloudwatch_insights
+        ```
         
-        Usage
-        -----
+        ## Usage
         
-        Examples
-        ^^^^^^^^
+        ### Examples
         
-        .. code-block:: python
+        ```python
+        from aws_cloudwatch_insights import Insights
+        from datetime import timedelta
         
-           from aws_cloudwatch_insights import Insights
-           from datetime import timedelta
+        insights = Insights()
+        query = """
+        fields @timestamp, @message, @logStream, @log
+        | sort @timestamp desc
+        | limit 20
+        """
         
-           insights = Insights()
-           query = """
-           fields @timestamp, @message, @logStream, @log
-           | sort @timestamp desc
-           | limit 20
-           """
+        results = insights.get_insights(
+            query, group_names=["/aws/lambda/log_maker"], result_limit=20,
+            start_time=-timedelta(days=1)
+        )
         
-           results = insights.get_insights(
-               query, group_names=["/aws/lambda/log_maker"], result_limit=20,
-               start_time=-timedelta(days=1)
-           )
+        ```
         
-        Reference
-        ^^^^^^^^^
+        ### Reference
         
         From the inline documentation:
         
-        .. code-block:: python
+        ```python
+        class Insights:
+            def __init__(self, logs_client: Optional[BaseClient] = None):
+                """
+                Object for querying AWS Cloudwatch.  Optionally takes a boto3 client as an argument, otherwise creates its own
+                """
+                ...
+        
+            def get_insights(self, query: str, result_limit: int, group_names: List[str], start_time: Union[int, datetime, timedelta],
+                             end_time: Union[int, datetime, timedelta, None] = None, callback: Optional[CallbackFunction] = None,
+                             error: Optional[ErrorFunction] = None, jsonify: bool = True) -> Iterable[GenericDict]:
+                """
+                Gets elements from AWS Cloudwatch Logs using an Insights query:
+        
+                Returns an iterable of dicts
+        
+                query: The Insights query
+                result_limit: Limit of the number of results returned
+                group_names: The log groups searched through
+                start_time: The time of the earliest record the query looks for.  Can be an int timestamp, a datetime, or a
+                 timedelta.  If it's a timedelta, the start time is now offset by the delta
+                end_time: The time of the latest record the query looks for.  Accepts same values as `start_time`
+                callback: A function witch is called when partial results are returned, before the function returns the final
+                    results.  Takes the partial results as an argument.
+                error: If included, this function is called when an exception is encountered (instead of not catching the
+                  exception).  The arguments passed to the function are the Exception instance and the partial results.  If
+                  this function doesn't through an exception, get_insights() returns the returned value of this function, empty
+                  list if that value is None
+                jsonify: If set to True, attempts to parse suspected json objects.  If parsing fails, just returns the string.
+                  Default: True
+                """
+                ...
+        ```
+        
+        ## Development
+        
+        Requires make:
+        
+        ```shell
+        # setting up dev environment
+        $ make develop
+        
+        # run tests
+        $ make test
+        # ... or
+        $ pytest
         
-           class Insights:
-               def __init__(self, logs_client: Optional[BaseClient] = None):
-                   """
-                   Object for querying AWS Cloudwatch.  Optionally takes a boto3 client as an argument, otherwise creates its own
-                   """
-                   ...
-        
-               def get_insights(self, query: str, result_limit: int, group_names: List[str], start_time: Union[int, datetime, timedelta],
-                                end_time: Union[int, datetime, timedelta, None] = None, callback: Optional[CallbackFunction] = None,
-                                error: Optional[ErrorFunction] = None, jsonify: bool = True) -> Iterable[GenericDict]:
-                   """
-                   Gets elements from AWS Cloudwatch Logs using an Insights query:
-        
-                   Returns an iterable of dicts
-        
-                   query: The Insights query
-                   result_limit: Limit of the number of results returned
-                   group_names: The log groups searched through
-                   start_time: The time of the earliest record the query looks for.  Can be an int timestamp, a datetime, or a
-                    timedelta.  If it's a timedelta, the start time is now offset by the delta
-                   end_time: The time of the latest record the query looks for.  Accepts same values as `start_time`
-                   callback: A function witch is called when partial results are returned, before the function returns the final
-                       results.  Takes the partial results as an argument.
-                   error: If included, this function is called when an exception is encountered (instead of not catching the
-                     exception).  The arguments passed to the function are the Exception instance and the partial results.  If
-                     this function doesn't through an exception, get_insights() returns the returned value of this function, empty
-                     list if that value is None
-                   jsonify: If set to True, attempts to parse suspected json objects.  If parsing fails, just returns the string.
-                     Default: True
-                   """
-                   ...
-        
-        Development
-        -----------
-        
-        Requires make, docker, and docker-compose:
-        
-        .. code-block:: shell
-        
-           # setting up dev environment
-           $ make develop
-        
-           # run tests
-           $ make test
-           # ... or
-           $ pytest
-        
-           # run tests for all environments
-           $ make test-all
-           $ make test-all-build  # checks to see if images need rebuilding
-           # ... you can use the underlying script to pass args to docker-compose directly:
-           $ ./scripts/run_tests_all.sh --build py36-no-cli py37  # runs for python 3.7 and python 3.6 with no cli
+        # run tests for all environments
+        $ make test-all
         
-        No CI/CD or coverage yet
-        
-        To Do
-        -----
+        ```
         
+        No CI/CD or coverage yet
         
+        ## To Do
         * If someone tells me they actually use this, I'll bump it to v1.0.0
         * More extensive CLI unit tests
-        * ``--csv`` output option
+        * `--csv` output option
         * Integration tests
         
-        Credits
-        -------
+        ## Credits
         
-        This package was created with *cookiecutter* and the ``audreyr/cookiecutter-pypackage`` project template.
+        This package was created with _cookiecutter_ and the `audreyr/cookiecutter-pypackage` project template.
         
 Keywords: aws,cloudwatch,insights
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 Provides-Extra: cli
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: types
```

### Comparing `aws_cloudwatch_insights-0.1.4/aws_cloudwatch_insights.egg-info/requires.txt` & `aws_cloudwatch_insights-0.1.5/aws_cloudwatch_insights.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aws_cloudwatch_insights-0.1.4/setup.py` & `aws_cloudwatch_insights-0.1.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,18 @@
 #!/usr/bin/env python
 
 """The setup script."""
 
 from setuptools import setup, find_packages
-from configparser import ConfigParser
 
-m2r_installed = False
-
-try:
-    import m2r
-    m2r_installed = True
-except ModuleNotFoundError as e:
-    pass
-
-with open('README.md') as readme_file:
+with open('README.md', 'r') as readme_file:
     readme = readme_file.read()
-if m2r_installed:
-    # only needed for publishing not for, say, running tests
-    readme = m2r.convert(readme)
-
-cfg = ConfigParser()
-cfg.read('setup.cfg')
-version = cfg['bumpversion']['current_version']
+with open('version.txt', 'r') as version_file:
+    version = version_file.read()
+    version = version.strip()
 
 requirements = [
     'boto3>=1.21.40,<2.0.0',
     'botocore>=1.21.40,<2.0.0'
 ]
 
 cli_requirements = [
@@ -54,15 +41,14 @@
     'types-colorama>=0.4.15.8,<1.0.0',
     'types-docutils>=0.19.1.6,<1.0.0',
     'types-python-dateutil>=2.8.19.9,<3.0.0',
     'types-setuptools>=67.4.0.3,<68.0.0'
 ]
 
 
-
 setup(
     author="Valmiki Rao",
     author_email='valmikirao@gmail.com',
     python_requires='>=3.7',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
@@ -86,14 +72,15 @@
         'cli': cli_requirements,
         'test': test_requirements,
         'lint': lint_requirements,
         'types': types_requirements
     },
     license="MIT license",
     long_description=readme,
+    long_description_content_type='text/markdown',
     include_package_data=True,
     keywords=['aws', 'cloudwatch', 'insights'],
     name='aws_cloudwatch_insights',
     packages=find_packages(include=['aws_cloudwatch_insights', 'aws_cloudwatch_insights.*']),
     url='https://github.com/valmikirao/aws_cloudwatch_insights',
     version=version,
     zip_safe=False,
```

