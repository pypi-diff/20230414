# Comparing `tmp/xqute-0.2.0.tar.gz` & `tmp/xqute-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xqute-0.2.0.tar", max compression
+gzip compressed data, was "xqute-0.2.1.tar", max compression
```

## Comparing `xqute-0.2.0.tar` & `xqute-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1063 2023-04-13 04:44:12.633953 xqute-0.2.0/LICENSE
--rw-r--r--   0        0        0     4795 2023-04-13 04:44:12.633953 xqute-0.2.0/README.md
--rw-r--r--   0        0        0     1173 2023-04-13 04:44:12.637953 xqute-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      246 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/__init__.py
--rw-r--r--   0        0        0     3352 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/defaults.py
--rw-r--r--   0        0        0     8595 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/job.py
--rw-r--r--   0        0        0     3017 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/plugin.py
--rw-r--r--   0        0        0     8109 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/scheduler.py
--rw-r--r--   0        0        0      633 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/__init__.py
--rw-r--r--   0        0        0     2361 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/local_scheduler.py
--rw-r--r--   0        0        0     4225 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/sge_scheduler.py
--rw-r--r--   0        0        0     7155 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/slurm_scheduler.py
--rw-r--r--   0        0        0       44 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/ssh_scheduler/__init__.py
--rw-r--r--   0        0        0     3547 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/ssh_scheduler/client.py
--rw-r--r--   0        0        0     2548 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/ssh_scheduler/scheduler.py
--rw-r--r--   0        0        0      691 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/schedulers/ssh_scheduler/submitter.py
--rw-r--r--   0        0        0     2176 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/utils.py
--rw-r--r--   0        0        0     9511 2023-04-13 04:44:12.637953 xqute-0.2.0/xqute/xqute.py
--rw-r--r--   0        0        0     5943 1970-01-01 00:00:00.000000 xqute-0.2.0/setup.py
--rw-r--r--   0        0        0     5679 1970-01-01 00:00:00.000000 xqute-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-04-14 00:56:20.902778 xqute-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4751 2023-04-14 00:56:20.902778 xqute-0.2.1/README.md
+-rw-r--r--   0        0        0     1173 2023-04-14 00:56:20.906779 xqute-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/__init__.py
+-rw-r--r--   0        0        0     3352 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/defaults.py
+-rw-r--r--   0        0        0     8595 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/job.py
+-rw-r--r--   0        0        0     3017 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/plugin.py
+-rw-r--r--   0        0        0     8109 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/scheduler.py
+-rw-r--r--   0        0        0      633 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/__init__.py
+-rw-r--r--   0        0        0     2361 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/local_scheduler.py
+-rw-r--r--   0        0        0     4225 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/sge_scheduler.py
+-rw-r--r--   0        0        0     7155 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/slurm_scheduler.py
+-rw-r--r--   0        0        0       44 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/ssh_scheduler/__init__.py
+-rw-r--r--   0        0        0     3547 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/ssh_scheduler/client.py
+-rw-r--r--   0        0        0     2548 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/ssh_scheduler/scheduler.py
+-rw-r--r--   0        0        0      691 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/schedulers/ssh_scheduler/submitter.py
+-rw-r--r--   0        0        0     2206 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/utils.py
+-rw-r--r--   0        0        0     9380 2023-04-14 00:56:20.906779 xqute-0.2.1/xqute/xqute.py
+-rw-r--r--   0        0        0     5898 1970-01-01 00:00:00.000000 xqute-0.2.1/setup.py
+-rw-r--r--   0        0        0     5635 1970-01-01 00:00:00.000000 xqute-0.2.1/PKG-INFO
```

### Comparing `xqute-0.2.0/LICENSE` & `xqute-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xqute-0.2.0/README.md` & `xqute-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 
 An xqute is initialized by:
 ```python
 xqute = Xqute(...)
 ```
 Available arguments are:
 
-- loglevel: The log level (Default: `INFO`)
 - scheduler: The scheduler class or name
 - plugins: The plugins to enable/disable for this session
 - job_metadir: The job meta directory (Default: `./.xqute/`)
 - job_error_strategy: The strategy when there is error happened
 - job_num_retries: Max number of retries when job_error_strategy is retry
 - job_submission_batch: The number of consumers to submit jobs
 - scheduler_forks: Max number of job forks
```

### Comparing `xqute-0.2.0/pyproject.toml` & `xqute-0.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xqute"
-version = "0.2.0"
+version = "0.2.1"
 description = "A job management system for python"
 authors = ["pwwang <pwwang@pwwang.com>"]
 license = "MIT"
 homepage = "https://github.com/pwwang/xqute"
 repository  = "https://github.com/pwwang/xqute"
 readme = "README.md"
```

### Comparing `xqute-0.2.0/xqute/defaults.py` & `xqute-0.2.1/xqute/defaults.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.0/xqute/job.py` & `xqute-0.2.1/xqute/job.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.0/xqute/plugin.py` & `xqute-0.2.1/xqute/plugin.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.0/xqute/scheduler.py` & `xqute-0.2.1/xqute/scheduler.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.0/xqute/schedulers/__init__.py` & `xqute-0.2.1/xqute/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.0/xqute/schedulers/local_scheduler.py` & `xqute-0.2.1/xqute/schedulers/local_scheduler.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.0/xqute/schedulers/sge_scheduler.py` & `xqute-0.2.1/xqute/schedulers/sge_scheduler.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.0/xqute/schedulers/slurm_scheduler.py` & `xqute-0.2.1/xqute/schedulers/slurm_scheduler.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.0/xqute/schedulers/ssh_scheduler/client.py` & `xqute-0.2.1/xqute/schedulers/ssh_scheduler/client.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.0/xqute/schedulers/ssh_scheduler/scheduler.py` & `xqute-0.2.1/xqute/schedulers/ssh_scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.0/xqute/schedulers/ssh_scheduler/submitter.py` & `xqute-0.2.1/xqute/schedulers/ssh_scheduler/submitter.py`

 * *Files identical despite different names*

### Comparing `xqute-0.2.0/xqute/utils.py` & `xqute-0.2.1/xqute/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,7 +79,8 @@
         self.prev_msg = message
         return True
 
 
 logger = logging.getLogger(LOGGER_NAME)
 logger.addHandler(RichHandler(show_path=False, omit_repeated_times=False))
 logger.addFilter(DuplicateFilter())
+logger.setLevel(logging.INFO)
```

### Comparing `xqute-0.2.0/xqute/xqute.py` & `xqute-0.2.1/xqute/xqute.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 
         buffer_queue: A buffer queue to save the pushed jobs
         queue: The job queue
         scheduler: The scheduler
         task: The task of producer and consumers
 
     Args:
-        loglevel: The log level
         scheduler: The scheduler class or name
         plugins: The plugins to be enabled or disabled
             to disable a plugin, using `no:plugin_name`
             either all plugin names should be prefixed with 'no:' or none
             of them should
             To enabled plugins, objects are
         job_metadir: The job meta directory
@@ -75,28 +74,24 @@
     EMPTY_BUFFER_SLEEP_TIME: int = 1
 
     def __init__(
         self,
         scheduler: str | Type[Scheduler] = "local",
         plugins: List[Any] | None = None,
         *,
-        loglevel: str = "INFO",
         job_metadir: PathLike = DEFAULT_JOB_METADIR,
         job_submission_batch: int = DEFAULT_JOB_SUBMISSION_BATCH,
         job_error_strategy: str = DEFAULT_JOB_ERROR_STRATEGY,
         job_num_retries: int = DEFAULT_JOB_NUM_RETRIES,
         scheduler_forks: int = DEFAULT_SCHEDULER_FORKS,
         scheduler_prescript: str = "",
         scheduler_postscript: str = "",
         **scheduler_opts,
     ) -> None:
         """Construct"""
-        # Set log level
-        logger.setLevel(loglevel.upper())
-
         self.jobs: List[Job] = []
 
         if plugins is not None:
             no_plugins = [
                 isinstance(plug, str) and plug.startswith("no:")
                 for plug in plugins
             ]
```

### Comparing `xqute-0.2.0/setup.py` & `xqute-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 extras_require = \
 {':python_version < "3.10"': ['aiopath>=0.5.0,<0.6.0'],
  ':python_version >= "3.10"': ['aiopath>=0.6,<0.7']}
 
 setup_kwargs = {
     'name': 'xqute',
-    'version': '0.2.0',
+    'version': '0.2.1',
     'description': 'A job management system for python',
-    'long_description': '# xqute\n\nA job management system for python\n\n## Features\n\n- Written in async\n- Plugin system\n- Scheduler adaptor\n- Job retrying/pipeline halting when failed\n\n## Installation\n\n```\npip install xqute\n```\n\n## A toy example\n```python\nimport asyncio\nfrom xqute import Xqute\n\nasync def main():\n    # 3 jobs allowed to run at the same time\n    xqute = Xqute(scheduler_forks=3)\n    for _ in range(10):\n        await xqute.put(\'sleep 1\')\n    await xqute.run_until_complete()\n\nif __name__ == \'__main__\':\n    asyncio.run(main())\n```\n\n![xqute](./xqute.png)\n\n\n## API\nhttps://pwwang.github.io/xqute/\n\n## Usage\n\n### Xqute object\n\nAn xqute is initialized by:\n```python\nxqute = Xqute(...)\n```\nAvailable arguments are:\n\n- loglevel: The log level (Default: `INFO`)\n- scheduler: The scheduler class or name\n- plugins: The plugins to enable/disable for this session\n- job_metadir: The job meta directory (Default: `./.xqute/`)\n- job_error_strategy: The strategy when there is error happened\n- job_num_retries: Max number of retries when job_error_strategy is retry\n- job_submission_batch: The number of consumers to submit jobs\n- scheduler_forks: Max number of job forks\n- **scheduler_opts: Additional keyword arguments for scheduler\n\nNote that the producer must be initialized in an event loop.\n\nTo push a job into the queue:\n```python\nawait xqute.put([\'echo\', 1])\n```\n\n### Using SGE scheduler\n```python\nxqute = Xqute(\n    \'sge\',\n    scheduler_forks=100,\n    qsub=\'path to qsub\',\n    qdel=\'path to qdel\',\n    qstat=\'path to qstat\',\n    sge_q=\'1-day\',  # or qsub_q=\'1-day\'\n    ...\n)\n```\nKeyword-arguments with names starting with `sge_` will be interpreted as `qsub` options. `list` or `tuple` option values will be expanded. For example:\n`sge_l=[\'h_vmem=2G\', \'gpu=1\']` will be expanded in wrapped script like this:\n```shell\n# ...\n\n#$ -l h_vmem=2G\n#$ -l gpu=1\n\n# ...\n```\n\n\n### Using Slurm scheduler\n\n```python\nxqute = Xqute(\n    \'slurm\',\n    scheduler_forks=100,\n    sbatch=\'path to sbatch\',\n    scancel=\'path to scancel\',\n    squeue=\'path to squeue\',\n    sbatch_partition=\'1-day\',  # or slurm_partition=\'1-day\'\n    sbatch_time=\'01:00:00\',\n    ...\n)\n```\n\n### Using ssh scheduler\n\n```python\nxqute = Xqute(\n    \'ssh\',\n    scheduler_forks=100,\n    ssh=\'path to ssh\',\n    ssh_servers={\n        "server1": {\n            "user": ...,\n            "port": 22,\n            "keyfile": ...,\n            # How long to keep the ssh connection alive\n            "ctrl_persist": 600,\n            # Where to store the control socket\n            "ctrl_dir": "/tmp",\n        },\n        ...\n    }\n    ...\n)\n```\n\nSSH servers must share the same filesystem and using keyfile authentication.\n\n### Plugins\n\nTo write a plugin for `xqute`, you will need to implement the following hooks:\n\n- `on_init(scheduler)`: Right after scheduler object is initialized\n- `on_shutdown(scheduler, sig)`: When scheduler is shutting down\n- `on_job_init(scheduler, job)`: When the job is initialized\n- `on_job_queued(scheduler, job)`: When the job is queued\n- `on_job_submitted(scheduler, job)`: When the job is submitted\n- `on_job_killing(scheduler, job)`: When the job is being killed\n- `on_job_killed(scheduler, job)`: When the job is killed\n- `on_job_failed(scheduler, job)`: When the job is failed\n- `on_job_succeeded(scheduler, job)`: When the job is succeeded\n\nNote that all hooks are corotines except `on_init` and `on_shutdown`, that means you should also implement them as corotines (sync implementations are allowed but will be warned).\n\nTo implement a hook, you have to fetch the plugin manager:\n\n```python\nfrom simplug import Simplug\npm = Simplug(\'xqute\')\n\n# or\nfrom xqute import simplug as pm\n```\n\nand then use the decorator `pm.impl`:\n\n```python\n@pm.impl\ndef on_init(scheduler):\n    ...\n```\n\n### Implementing a scheduler\n\nCurrently there are only 2 builtin schedulers: `local` and `sge`.\n\nOne can implement a scheduler by subclassing the `Scheduler` abstract class. There are three abstract methods that have to be implemented in the subclass:\n\n```python\nfrom xqute import Scheduer\n\nclass MyScheduler(Scheduler):\n    name = \'my\'\n    job_class: MyJob\n\n    async def submit_job(self, job):\n        """How to submit a job, return a unique id in the scheduler system\n        (the pid for local scheduler for example)\n        """\n\n    async def kill_job(self, job):\n        """How to kill a job"""\n\n    async def job_is_running(self, job):\n        """Check if a job is running"""\n```\n\nAs you may see, we may also need to implement a job class before `MyScheduler`. The only abstract method to be implemented is `wrap_cmd`:\n```python\nfrom xqute import Job\n\nclass MyJob(Job):\n\n    async def wrap_cmd(self, scheduler):\n        ...\n```\n\nYou have to use the trap command in the wrapped script to update job status, return code and clear the job id file.\n',
+    'long_description': '# xqute\n\nA job management system for python\n\n## Features\n\n- Written in async\n- Plugin system\n- Scheduler adaptor\n- Job retrying/pipeline halting when failed\n\n## Installation\n\n```\npip install xqute\n```\n\n## A toy example\n```python\nimport asyncio\nfrom xqute import Xqute\n\nasync def main():\n    # 3 jobs allowed to run at the same time\n    xqute = Xqute(scheduler_forks=3)\n    for _ in range(10):\n        await xqute.put(\'sleep 1\')\n    await xqute.run_until_complete()\n\nif __name__ == \'__main__\':\n    asyncio.run(main())\n```\n\n![xqute](./xqute.png)\n\n\n## API\nhttps://pwwang.github.io/xqute/\n\n## Usage\n\n### Xqute object\n\nAn xqute is initialized by:\n```python\nxqute = Xqute(...)\n```\nAvailable arguments are:\n\n- scheduler: The scheduler class or name\n- plugins: The plugins to enable/disable for this session\n- job_metadir: The job meta directory (Default: `./.xqute/`)\n- job_error_strategy: The strategy when there is error happened\n- job_num_retries: Max number of retries when job_error_strategy is retry\n- job_submission_batch: The number of consumers to submit jobs\n- scheduler_forks: Max number of job forks\n- **scheduler_opts: Additional keyword arguments for scheduler\n\nNote that the producer must be initialized in an event loop.\n\nTo push a job into the queue:\n```python\nawait xqute.put([\'echo\', 1])\n```\n\n### Using SGE scheduler\n```python\nxqute = Xqute(\n    \'sge\',\n    scheduler_forks=100,\n    qsub=\'path to qsub\',\n    qdel=\'path to qdel\',\n    qstat=\'path to qstat\',\n    sge_q=\'1-day\',  # or qsub_q=\'1-day\'\n    ...\n)\n```\nKeyword-arguments with names starting with `sge_` will be interpreted as `qsub` options. `list` or `tuple` option values will be expanded. For example:\n`sge_l=[\'h_vmem=2G\', \'gpu=1\']` will be expanded in wrapped script like this:\n```shell\n# ...\n\n#$ -l h_vmem=2G\n#$ -l gpu=1\n\n# ...\n```\n\n\n### Using Slurm scheduler\n\n```python\nxqute = Xqute(\n    \'slurm\',\n    scheduler_forks=100,\n    sbatch=\'path to sbatch\',\n    scancel=\'path to scancel\',\n    squeue=\'path to squeue\',\n    sbatch_partition=\'1-day\',  # or slurm_partition=\'1-day\'\n    sbatch_time=\'01:00:00\',\n    ...\n)\n```\n\n### Using ssh scheduler\n\n```python\nxqute = Xqute(\n    \'ssh\',\n    scheduler_forks=100,\n    ssh=\'path to ssh\',\n    ssh_servers={\n        "server1": {\n            "user": ...,\n            "port": 22,\n            "keyfile": ...,\n            # How long to keep the ssh connection alive\n            "ctrl_persist": 600,\n            # Where to store the control socket\n            "ctrl_dir": "/tmp",\n        },\n        ...\n    }\n    ...\n)\n```\n\nSSH servers must share the same filesystem and using keyfile authentication.\n\n### Plugins\n\nTo write a plugin for `xqute`, you will need to implement the following hooks:\n\n- `on_init(scheduler)`: Right after scheduler object is initialized\n- `on_shutdown(scheduler, sig)`: When scheduler is shutting down\n- `on_job_init(scheduler, job)`: When the job is initialized\n- `on_job_queued(scheduler, job)`: When the job is queued\n- `on_job_submitted(scheduler, job)`: When the job is submitted\n- `on_job_killing(scheduler, job)`: When the job is being killed\n- `on_job_killed(scheduler, job)`: When the job is killed\n- `on_job_failed(scheduler, job)`: When the job is failed\n- `on_job_succeeded(scheduler, job)`: When the job is succeeded\n\nNote that all hooks are corotines except `on_init` and `on_shutdown`, that means you should also implement them as corotines (sync implementations are allowed but will be warned).\n\nTo implement a hook, you have to fetch the plugin manager:\n\n```python\nfrom simplug import Simplug\npm = Simplug(\'xqute\')\n\n# or\nfrom xqute import simplug as pm\n```\n\nand then use the decorator `pm.impl`:\n\n```python\n@pm.impl\ndef on_init(scheduler):\n    ...\n```\n\n### Implementing a scheduler\n\nCurrently there are only 2 builtin schedulers: `local` and `sge`.\n\nOne can implement a scheduler by subclassing the `Scheduler` abstract class. There are three abstract methods that have to be implemented in the subclass:\n\n```python\nfrom xqute import Scheduer\n\nclass MyScheduler(Scheduler):\n    name = \'my\'\n    job_class: MyJob\n\n    async def submit_job(self, job):\n        """How to submit a job, return a unique id in the scheduler system\n        (the pid for local scheduler for example)\n        """\n\n    async def kill_job(self, job):\n        """How to kill a job"""\n\n    async def job_is_running(self, job):\n        """Check if a job is running"""\n```\n\nAs you may see, we may also need to implement a job class before `MyScheduler`. The only abstract method to be implemented is `wrap_cmd`:\n```python\nfrom xqute import Job\n\nclass MyJob(Job):\n\n    async def wrap_cmd(self, scheduler):\n        ...\n```\n\nYou have to use the trap command in the wrapped script to update job status, return code and clear the job id file.\n',
     'author': 'pwwang',
     'author_email': 'pwwang@pwwang.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/pwwang/xqute',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `xqute-0.2.0/PKG-INFO` & `xqute-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xqute
-Version: 0.2.0
+Version: 0.2.1
 Summary: A job management system for python
 Home-page: https://github.com/pwwang/xqute
 License: MIT
 Author: pwwang
 Author-email: pwwang@pwwang.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -67,15 +67,14 @@
 
 An xqute is initialized by:
 ```python
 xqute = Xqute(...)
 ```
 Available arguments are:
 
-- loglevel: The log level (Default: `INFO`)
 - scheduler: The scheduler class or name
 - plugins: The plugins to enable/disable for this session
 - job_metadir: The job meta directory (Default: `./.xqute/`)
 - job_error_strategy: The strategy when there is error happened
 - job_num_retries: Max number of retries when job_error_strategy is retry
 - job_submission_batch: The number of consumers to submit jobs
 - scheduler_forks: Max number of job forks
```

