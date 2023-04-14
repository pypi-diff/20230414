# Comparing `tmp/genopype-2020.3.27.tar.gz` & `tmp/genopype-2023.4.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/genopype-2020.3.27.tar", last modified: Fri Mar 27 19:02:20 2020, max compression
+gzip compressed data, was "genopype-2023.4.13.tar", last modified: Fri Apr 14 00:02:36 2023, max compression
```

## Comparing `genopype-2020.3.27.tar` & `genopype-2023.4.13.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 mu         (501) staff       (20)        0 2020-03-27 19:02:20.000000 genopype-2020.3.27/
--rw-------   0 mu         (501) staff       (20)       37 2019-07-12 20:48:35.000000 genopype-2020.3.27/MANIFEST.in
--rw-r--r--   0 mu         (501) staff       (20)      269 2020-03-27 19:02:20.000000 genopype-2020.3.27/PKG-INFO
--rw-------   0 mu         (501) staff       (20)      959 2020-03-27 17:43:39.000000 genopype-2020.3.27/README.md
-drwxr-xr-x   0 mu         (501) staff       (20)        0 2020-03-27 19:02:20.000000 genopype-2020.3.27/genopype/
--rw-------   0 mu         (501) staff       (20)     2768 2020-03-27 18:51:25.000000 genopype-2020.3.27/genopype/__init__.py
--rw-------   0 mu         (501) staff       (20)    36294 2020-03-27 18:38:08.000000 genopype-2020.3.27/genopype/genopype.py
-drwxr-xr-x   0 mu         (501) staff       (20)        0 2020-03-27 19:02:20.000000 genopype-2020.3.27/genopype.egg-info/
--rw-r--r--   0 mu         (501) staff       (20)      269 2020-03-27 19:02:19.000000 genopype-2020.3.27/genopype.egg-info/PKG-INFO
--rw-r--r--   0 mu         (501) staff       (20)      231 2020-03-27 19:02:19.000000 genopype-2020.3.27/genopype.egg-info/SOURCES.txt
--rw-r--r--   0 mu         (501) staff       (20)        1 2020-03-27 19:02:19.000000 genopype-2020.3.27/genopype.egg-info/dependency_links.txt
--rw-r--r--   0 mu         (501) staff       (20)       34 2020-03-27 19:02:19.000000 genopype-2020.3.27/genopype.egg-info/requires.txt
--rw-r--r--   0 mu         (501) staff       (20)        9 2020-03-27 19:02:19.000000 genopype-2020.3.27/genopype.egg-info/top_level.txt
--rw-r--r--   0 mu         (501) staff       (20)       38 2020-03-27 19:02:20.000000 genopype-2020.3.27/setup.cfg
--rw-------   0 mu         (501) staff       (20)      718 2020-03-27 18:54:03.000000 genopype-2020.3.27/setup.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-04-14 00:02:36.920054 genopype-2023.4.13/
+-rw-------   0 jespinoz  (3456) staff       (20)     1524 2023-03-22 04:17:10.000000 genopype-2023.4.13/LICENSE
+-rw-------   0 jespinoz  (3456) staff       (20)     2023 2023-04-13 20:32:03.000000 genopype-2023.4.13/LICENSE.txt
+-rw-------   0 jespinoz  (3456) staff       (20)      193 2023-04-13 20:32:03.000000 genopype-2023.4.13/MANIFEST.in
+-rw-r--r--   0 jespinoz  (3456) staff       (20)      278 2023-04-14 00:02:36.919658 genopype-2023.4.13/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)     7261 2023-04-13 20:32:03.000000 genopype-2023.4.13/README.md
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-04-14 00:02:36.916243 genopype-2023.4.13/genopype/
+-rw-------   0 jespinoz  (3456) staff       (20)     2769 2023-04-14 00:01:29.000000 genopype-2023.4.13/genopype/__init__.py
+-rw-------   0 jespinoz  (3456) staff       (20)    38712 2023-04-14 00:00:38.000000 genopype-2023.4.13/genopype/genopype.py
+drwxr-xr-x   0 jespinoz  (3456) staff       (20)        0 2023-04-14 00:02:36.919114 genopype-2023.4.13/genopype.egg-info/
+-rw-------   0 jespinoz  (3456) staff       (20)      278 2023-04-14 00:02:36.000000 genopype-2023.4.13/genopype.egg-info/PKG-INFO
+-rw-------   0 jespinoz  (3456) staff       (20)      251 2023-04-14 00:02:36.000000 genopype-2023.4.13/genopype.egg-info/SOURCES.txt
+-rw-------   0 jespinoz  (3456) staff       (20)        1 2023-04-14 00:02:36.000000 genopype-2023.4.13/genopype.egg-info/dependency_links.txt
+-rw-------   0 jespinoz  (3456) staff       (20)       34 2023-04-14 00:02:36.000000 genopype-2023.4.13/genopype.egg-info/requires.txt
+-rw-------   0 jespinoz  (3456) staff       (20)        9 2023-04-14 00:02:36.000000 genopype-2023.4.13/genopype.egg-info/top_level.txt
+-rw-r--r--   0 jespinoz  (3456) staff       (20)       38 2023-04-14 00:02:36.920177 genopype-2023.4.13/setup.cfg
+-rw-------   0 jespinoz  (3456) staff       (20)      718 2023-04-13 20:32:03.000000 genopype-2023.4.13/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `genopype-2020.3.27/genopype/__init__.py` & `genopype-2023.4.13/genopype/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ==============
-# goomba
+# genopype
 # ==============
 # Architecture for creating bash pipelines, in particular, for bioinformatics
 # ------------------------------------
 # GitHub: https://github.com/jolespin/genopype
 # PyPI: https://pypi.org/project/genopype/
 # ------------------------------------
 # =======
@@ -29,15 +29,15 @@
 #
 # THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 #
 # =======
 # Version
 # =======
-__version__= "2020.03.27"
+__version__= "2023.4.13"
 __author__ = "Josh L. Espinoza"
 __email__ = "jespinoz@jcvi.org, jol.espinoz@gmail.com"
 __url__ = "https://github.com/jolespin/genopype"
 __cite__ = "https://github.com/jolespin/genopype"
 __license__ = "BSD-3"
 __developmental__ = True
 __all__ = ["Command","ExecutablePipeline","DisplayablePath", "get_directory_tree", "get_directory_size",  "check_filename", "format_filename", "create_directory", "validate_file_existence"]
```

### Comparing `genopype-2020.3.27/genopype/genopype.py` & `genopype-2023.4.13/genopype/genopype.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 from __future__ import print_function, division
-import os, sys, glob, time,subprocess, random
+import os, sys, glob, time,subprocess, random, warnings
 from collections import OrderedDict, Counter
 # Pathlib
 try:
     import pathlib
 except ImportError:
     import pathlib2 as pathlib
 # Scandir
@@ -15,15 +15,14 @@
 # Soothsayer utils
 from soothsayer_utils import *
 
 
 # Know Bugs:
 # * Currently (2019.07.26), the "completed_message" parameter does not work.
 
-
 # Check filename
 def check_filename(filename, acceptable_characters={".","-","_"}):
     status_ok = True
     for character in str(filename).lower():
         conditions = [
         character.isalnum(),
         character in acceptable_characters,
@@ -54,15 +53,18 @@
     assert is_path_like(directory, path_must_exist=False)
     # directory = os.path.realpath(directory)
     if not os.path.exists(directory):
         os.makedirs(directory)
     return directory
 
 # Validating file existence
-def validate_file_existence(paths, prologue="Validating the following files:", minimum_filesize=2, f_verbose=None):
+def validate_file_existence(paths, prologue="Validating the following files:", minimum_filesize=2, f_verbose=None, whitelist_empty_files=[]):
+    if whitelist_empty_files is None: 
+        whitelist_empty_files = []
+
     if is_file_like(f_verbose) or (f_verbose is None):
         print(prologue, file=f_verbose)
 
     paths_expanded = list()
     for path in paths:
         if "*" in path:
             paths_expanded += glob.glob(path)
@@ -79,15 +81,21 @@
         # original_path = None
         # symlink = None
         if os.path.islink(path):
             path = os.readlink(path)
         if not os.path.isdir(path):
             size_bytes = os.path.getsize(path)
 
-            assert size_bytes >= minimum_filesize, "The following file appears to be empty ({} bytes): {}".format(size_bytes, path)
+            if path not in whitelist_empty_files:
+                # print(path, whitelist_empty_files)
+                assert size_bytes >= minimum_filesize, "The following file appears to be empty ({} bytes): {}".format(size_bytes, path)
+            else:
+                if size_bytes >= minimum_filesize:
+                    warnings.warn("The following file appears to be empty ({} bytes): {}".format(size_bytes, path))
+
             if is_file_like(f_verbose) or (f_verbose is None):
                 size_mb = size_bytes >> 20
                 if size_mb < 1:
                     print("[=] File exists ({} bytes):".format(size_bytes), path, file=f_verbose)
 
                 else:
                     print("[=] File exists ({} MB):".format(size_mb), path, file=f_verbose)
@@ -335,15 +343,15 @@
     sys.stdout.flush()
 
     """
     def __init__(self, cmd, name=None, description=None, f_cmds=sys.stdout ):
 
         if isinstance(cmd, str):
             cmd = [cmd]
-        cmd = " ".join(cmd)
+        cmd = " ".join(list(filter(bool, map(str, cmd))))
         self.cmd = cmd
         if not is_file_like(f_cmds):
             if is_path_like(f_cmds, path_must_exist=False):
                 f_cmds = open(f_cmds, "w")
         self.f_cmds = f_cmds
         self.name = name
         self.description = description
@@ -384,14 +392,16 @@
         checkpoint_message_exists="Loading. .. ... .....",
         error_message=None,
         completed_message=None,
         f_verbose=None,
         n_linebreaks=1,
         acceptable_returncodes=[0],
         popen_kws=dict(),
+        shell_executable="/bin/bash",
+
         ):
         """
         Should future versions should have separate prologue and epilogue for f_cmds and f_verbose?
         """
         # Verbose
         if f_verbose is None:
             f_verbose = sys.stdout
@@ -446,15 +456,15 @@
                 write_stdout = format_path(write_stdout)
                 f_stdout = open(write_stdout, "wb")
             f_stderr = subprocess.PIPE
             if write_stderr is not None:
                 write_stderr = format_path(write_stderr)
                 f_stderr = open(write_stderr, "wb")
             # Execute the process
-            self.process_ = subprocess.Popen(self.cmd, shell=True, stdout=f_stdout, stderr=f_stderr, **popen_kws) #! Future: Use file objects instead here so it can be written in real time
+            self.process_ = subprocess.Popen(self.cmd, shell=True, stdout=f_stdout, stderr=f_stderr, executable=shell_executable, **popen_kws) #! Future: Use file objects instead here so it can be written in real time
             # Wait until process is complete and return stdout/stderr
             self.stdout_, self.stderr_ = self.process_.communicate() # Use this .communicate instead of .wait to avoid zombie process that hangs due to defunct. Removed timeout b/c it's not available in Python 2
 
             # Set stdout and stderr to the contents of the file object created...or just the path then do a get_stdout() function
 
             if hasattr(f_stdout, "close"):
                 f_stdout.close()
@@ -473,16 +483,14 @@
             # if isinstance(self.stderr_, bytes):
             #     self.stderr_ = self.stderr_.decode("utf-8")
             # self._write_output(data=self.stderr_, filepath=write_stderr)
 
             # Return code
             self._write_output(data=self.returncode_, filepath=write_returncode)
 
-
-
             # Check
             if not errors_ok:
                 if self.returncode_ not in acceptable_returncodes:
                     if error_message is not None:
                         print(error_message, file=f_verbose)
                     sys.exit(self.returncode_)
             if self.returncode_ in acceptable_returncodes:
@@ -555,14 +563,16 @@
                 output_filepaths=None,
                 # Utility
                 dry="infer",
                 errors_ok=False,
                 validate_inputs=True,
                 validate_outputs=True,
                 acceptable_returncodes=[0],
+                whitelist_empty_input_files=[], 
+                whitelist_empty_output_files=[], 
                 ):
         # Step
         if step == "infer":
             step = len(self.executables) + 1
         assert isinstance(step, int), "Please specify an integer step."
 
         # if bypass_io_validation_if_checkpoint_exists:
@@ -597,15 +607,16 @@
         attrs["checkpoint"] = None
         attrs["write_stdout"] = None
         attrs["write_stderr"] = None
         attrs["write_returncode"] = None
         attrs["error_message"] = None
         attrs["completed_message"] = None
         attrs["acceptable_returncodes"] = acceptable_returncodes
-
+        attrs["whitelist_empty_input_files"] = whitelist_empty_input_files
+        attrs["whitelist_empty_output_files"] = whitelist_empty_output_files
 
         # Checkpoint
         attrs["dry"] = dry
 
         # Validation
         attrs["errors_ok"] = errors_ok
         attrs["validate_inputs"] = validate_inputs
@@ -676,31 +687,43 @@
 
 
         # Compiled
         self.compiled = True
         return self
 
     # Execute pipeline
-    def execute(self, steps=None, description="Executing pipeline", restart_from_checkpoint=None):
+    def execute(self, steps=None, description="Executing pipeline", restart_from_checkpoint=None, stop_at_checkpoint=None, shell_executable="/bin/bash"):
         start_time = time.time()
         assert self.compiled, "Please compile before continuing."
         if steps is None:
             steps = list(self.compiled_steps_.keys())
         if self.name is not None:
             if self.description is None:
                 print(format_header(". .. ... {} ... .. .".format(self.name), "_"), file=self.f_verbose)
             else:
                 print(format_header(". .. ... {} || {} ... .. .".format(self.name, self.description), "_"), file=self.f_verbose)
             print("", file=self.f_verbose)
+
+        if stop_at_checkpoint is None:
+            stop_at_checkpoint = steps[-1]
+        stop_at_checkpoint = int(stop_at_checkpoint)
+        assert stop_at_checkpoint in steps, "Cannot stop at checkpoint `{}` because it does not exist".format(stop_at_checkpoint)
+        
         if restart_from_checkpoint is not None:
             restart_from_checkpoint = int(restart_from_checkpoint)
+            if restart_from_checkpoint < 0:
+                assert abs(restart_from_checkpoint) <= len(steps), "Cannot have restart_from_checkpoint == {} for N = {} steps: {}".format(restart_from_checkpoint, len(steps), steps)
+                restart_from_checkpoint = steps[restart_from_checkpoint]
             assert restart_from_checkpoint in steps, "Cannot restart from checkpoint `{}` because it does not exist".format(restart_from_checkpoint)
             if self.checkpoint_directory is not None:
-                if restart_from_checkpoint == "preprocessing":
-                    restart_from_checkpoint = 1
+                # Need to test
+                # ------------
+                if restart_from_checkpoint < 0: 
+                    restart_from_checkpoint = sorted(steps)[restart_from_checkpoint]
+                # -------------
 
                 target_checkpoint = restart_from_checkpoint
                 print("Restarting pipeline from checkpoint:", target_checkpoint, file=self.f_verbose)
                 for file in scandir(self.checkpoint_directory):
                     if "_" in file.name:
                         query_checkpoint = int(file.name.split("_")[0].split(".")[0])
                         if query_checkpoint >= target_checkpoint:
@@ -748,15 +771,15 @@
                         # for path in input_filepaths:
                         #     if "*" in path:
                         #         paths_expanded += glob.glob(path)
                         #     else:
                         #         # path = os.path.realpath(path)
                         #         paths_expanded.append(path)
                         # self.executables[id]["input_filepaths"] = paths_expanded
-                        validate_file_existence(input_filepaths, prologue="Validating the following input files:", f_verbose=self.f_verbose)
+                        validate_file_existence(input_filepaths, prologue="Validating the following input files:", f_verbose=self.f_verbose, whitelist_empty_files=attrs["whitelist_empty_input_files"])
                         print("", file=self.f_verbose)
 
 
                 # Execute
                 executable.run(
                     prologue=id,
                     dry=attrs["dry"],
@@ -767,25 +790,31 @@
                     checkpoint_message_notexists=self.checkpoint_message_notexists,
                     checkpoint_message_exists=self.checkpoint_message_exists,
                     write_stdout=attrs["write_stdout"],
                     write_stderr=attrs["write_stderr"],
                     write_returncode=attrs["write_returncode"],
                     acceptable_returncodes=attrs["acceptable_returncodes"],
                     f_verbose=self.f_verbose,
+                    shell_executable=shell_executable,
                 )
                 # Check outputs
                 if attrs["validate_outputs"]:
                     output_filepaths = attrs["output_filepaths"]
                     if bool(output_filepaths):
                         assert is_nonstring_iterable(output_filepaths),  "`output_filepaths` must be a non-string iterable"
-                        validate_file_existence(output_filepaths, prologue="\nValidating the following output files:", f_verbose=self.f_verbose)
+                        validate_file_existence(output_filepaths, prologue="\nValidating the following output files:", f_verbose=self.f_verbose, whitelist_empty_files=attrs["whitelist_empty_output_files"])
                         # print("", file=self.f_verbose)
 
                 print("\nDuration: {}\n".format(format_duration(start_time)), file=self.f_verbose)
 
+                if step == stop_at_checkpoint:
+                    if step != steps[-1]:
+                        print("Stopping at checkpoint: {}".format(stop_at_checkpoint), file=sys.stdout)
+                        break
+
         self.duration_ = format_duration(start_time)
         print("\n", format_header("Total duration: {}".format(self.duration_), "."), sep="", file=self.f_verbose)
         return self
 
 #     # Save object
 #     def to_file(self, path, compression="infer", protocol=pickle.HIGHEST_PROTOCOL, *args):
 #         # Cannot serialize file objects while open so we need make placeholders
@@ -823,34 +852,38 @@
     directories["checkpoints"] = create_directory(os.path.join(directories["output"], "checkpoints"))
     directories["logs"] = create_directory(os.path.join(directories["output"], "logs"))
 
 
     with open(os.path.join(directories["output"], "commands.sh"), "w") as f_cmds:
         ep = ExecutablePipeline(name="Sith", description="The rule of two", f_cmds=f_cmds, checkpoint_directory=directories["checkpoints"], log_directory=directories["logs"], bypass_io_validation_if_checkpoints_exist=True)
         # Step 1
-        output_filepaths = [os.path.join(directories["output"], "holocron.txt")]
+        output_filepaths = [os.path.join(directories["output"], "holocron.txt"), os.path.join(directories["output"], "empty.txt")]
         message = "Two there should be; no more, no less. One to embody the power, the other to crave it.\n"
         ep.add_step(id="Darth Bane",
-                    cmd="echo '{}' > {}".format(message, output_filepaths[0]),
+                    cmd="echo $0 && echo '{}' > {} && >{}".format(message, output_filepaths[0], output_filepaths[1]),
                     output_filepaths=output_filepaths,
                     description = "Begin the rule of two",
                     errors_ok=False,
                     validate_outputs=True,
+                    whitelist_empty_output_files=[output_filepaths[1]],
        )
         # Step 2
-        input_filepaths = [os.path.join(directories["output"], "holocron.txt")]
+        input_filepaths = [os.path.join(directories["output"], "holocron.txt"), os.path.join(directories["output"], "empty.txt")]
         output_filepaths = [os.path.join(directories["output"], "*.txt")]
         ep.add_step(id="Darth Plagueis",
-                    cmd="(cat {} && echo 'jedi') > {} ".format(input_filepaths[0], os.path.join(directories["output"], "wisdom.txt")),
+                    cmd="echo $0 && (cat {} && echo 'jedi') > {} && echo 'This file is empty and it is ok {}'".format(os.path.join(directories["output"], "holocron.txt"), os.path.join(directories["output"], "wisdom.txt"), os.path.join(directories["output"], "empty.txt")),
                     input_filepaths=input_filepaths,
                     output_filepaths=output_filepaths,
                     description = "Read the holocron",
                     errors_ok=False,
                     validate_inputs=True,
                     validate_outputs=True,
+                    whitelist_empty_input_files=[input_filepaths[1]],
+                    whitelist_empty_output_files=[input_filepaths[1]],
+
        )
         # Step 3
         input_filepaths = [os.path.join(directories["output"], "holocron.txt"), os.path.join(directories["output"], "wisdom.txt")]
         output_directory = create_directory(os.path.join(directories["output"], "temple"))
         output_filepaths = [os.path.join(output_directory, "data-crystal.txt"), output_directory]
         cmds = [
         "(",
@@ -863,13 +896,14 @@
         ep.add_step(id="Darth Sidious",
                     cmd=cmds,
                     input_filepaths=input_filepaths,
                     output_filepaths=output_filepaths,
                     description = "Move the data",
        )
         ep.compile()
-        ep.execute(restart_from_checkpoint=3)
+        ep.execute(restart_from_checkpoint=1, shell_executable="/bin/bash")
 
         # Directory structure
         print("\n", format_header("Directory structure:","_"), "\n", get_directory_tree(directories["output"], ascii=True), sep="", file=sys.stdout)
+
 if __name__ == "__main__":
     main()
```

### Comparing `genopype-2020.3.27/setup.py` & `genopype-2023.4.13/setup.py`

 * *Files identical despite different names*

