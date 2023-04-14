# Comparing `tmp/xfaster-1.1.0.tar.gz` & `tmp/xfaster-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfaster-1.1.0.tar", last modified: Fri Jul 22 03:56:22 2022, max compression
+gzip compressed data, was "xfaster-1.1.1.tar", last modified: Fri Apr 14 18:19:05 2023, max compression
```

## Comparing `xfaster-1.1.0.tar` & `xfaster-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 03:56:22.549463 xfaster-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-07-22 03:55:52.000000 xfaster-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-07-22 03:55:52.000000 xfaster-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-07-22 03:56:22.549463 xfaster-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-07-22 03:55:52.000000 xfaster-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-22 03:56:22.549463 xfaster-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-07-22 03:55:52.000000 xfaster-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 03:56:22.549463 xfaster-1.1.0/xfaster/
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-07-22 03:55:52.000000 xfaster-1.1.0/xfaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27143 2022-07-22 03:55:52.000000 xfaster-1.1.0/xfaster/batch_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    30647 2022-07-22 03:55:52.000000 xfaster-1.1.0/xfaster/parse_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)    10046 2022-07-22 03:55:52.000000 xfaster-1.1.0/xfaster/spec_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)   262659 2022-07-22 03:55:52.000000 xfaster-1.1.0/xfaster/xfaster_class.py
--rw-r--r--   0 runner    (1001) docker     (121)    62631 2022-07-22 03:55:52.000000 xfaster-1.1.0/xfaster/xfaster_exec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 03:56:22.549463 xfaster-1.1.0/xfaster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      903 2022-07-22 03:56:22.000000 xfaster-1.1.0/xfaster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      364 2022-07-22 03:56:22.000000 xfaster-1.1.0/xfaster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-22 03:56:22.000000 xfaster-1.1.0/xfaster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-07-22 03:56:22.000000 xfaster-1.1.0/xfaster.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-07-22 03:56:22.000000 xfaster-1.1.0/xfaster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-22 03:56:22.000000 xfaster-1.1.0/xfaster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:19:05.496826 xfaster-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-14 18:18:30.000000 xfaster-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 18:18:30.000000 xfaster-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-14 18:19:05.496826 xfaster-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-14 18:18:30.000000 xfaster-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 18:19:05.496826 xfaster-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-14 18:18:30.000000 xfaster-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:19:05.496826 xfaster-1.1.1/xfaster/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-14 18:18:30.000000 xfaster-1.1.1/xfaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27143 2023-04-14 18:18:30.000000 xfaster-1.1.1/xfaster/batch_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30647 2023-04-14 18:18:30.000000 xfaster-1.1.1/xfaster/parse_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10046 2023-04-14 18:18:30.000000 xfaster-1.1.1/xfaster/spec_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)   262967 2023-04-14 18:18:30.000000 xfaster-1.1.1/xfaster/xfaster_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66070 2023-04-14 18:18:30.000000 xfaster-1.1.1/xfaster/xfaster_exec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:19:05.496826 xfaster-1.1.1/xfaster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-04-14 18:19:05.000000 xfaster-1.1.1/xfaster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-14 18:19:05.000000 xfaster-1.1.1/xfaster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:19:05.000000 xfaster-1.1.1/xfaster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-14 18:19:05.000000 xfaster-1.1.1/xfaster.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-14 18:19:05.000000 xfaster-1.1.1/xfaster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 18:19:05.000000 xfaster-1.1.1/xfaster.egg-info/top_level.txt
```

### Comparing `xfaster-1.1.0/LICENSE` & `xfaster-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xfaster-1.1.0/setup.py` & `xfaster-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `xfaster-1.1.0/xfaster/batch_tools.py` & `xfaster-1.1.1/xfaster/batch_tools.py`

 * *Files identical despite different names*

### Comparing `xfaster-1.1.0/xfaster/parse_tools.py` & `xfaster-1.1.1/xfaster/parse_tools.py`

 * *Files identical despite different names*

### Comparing `xfaster-1.1.0/xfaster/spec_tools.py` & `xfaster-1.1.1/xfaster/spec_tools.py`

 * *Files identical despite different names*

### Comparing `xfaster-1.1.0/xfaster/xfaster_class.py` & `xfaster-1.1.1/xfaster/xfaster_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -2257,15 +2257,20 @@
         else:
             reference_type = None
 
         if template_specs is None:
             template_specs = self.specs
 
         # ensure dictionary
-        if template_alpha is None or null_run or template_type is None:
+        if (
+            template_alpha is None
+            or null_run
+            or (update_template and self.template_type is None)
+            or (not update_template and template_type is None)
+        ):
             template_alpha = OrderedDict()
         else:
             # ensure tagged by original tags
             template_alpha = OrderedDict(
                 [(k, v) for k, v in template_alpha.items() if k in self.map_tags_orig]
             )
 
@@ -2918,14 +2923,16 @@
         signal_files2 = self.signal_files2 if null_run else None
         num_signal = self.num_signal
 
         if do_noise:
             noise_files = self.noise_files
             noise_files2 = self.noise_files2 if null_run else None
             num_noise = self.num_noise
+        else:
+            num_noise = 0
 
         # process signal, noise, and S+N
         cls_sig = OrderedDict()
         cls_null_sig = OrderedDict() if null_run else None
         cls_noise = OrderedDict() if do_noise else None
         cls_null_noise = OrderedDict() if null_run and do_noise else None
         cls_tot = OrderedDict()
@@ -6747,14 +6754,17 @@
                 self.log("MCMC iteration {}".format(sampler.iteration), "debug")
             # check convergence every 100 steps
             if sampler.iteration % 100:
                 continue
 
             # compute autocorrelation time
             tau = sampler.get_autocorr_time(tol=0)
+            if np.isnan(tau).any():
+                self.log('Found nan autocorr time! Stopping.', "error")
+                break
 
             # check convergence
             converged = np.all(tau / converge_criteria < sampler.iteration)
             converged &= np.all(np.abs(old_tau - tau) / tau < converge_criteria)
             self.log(
                 "MCMC iteration {} autocorr time: mean {:.1f} min {:.1f} max {:.1f}".format(
                     sampler.iteration, np.mean(tau), np.min(tau), np.max(tau)
```

### Comparing `xfaster-1.1.0/xfaster/xfaster_exec.py` & `xfaster-1.1.1/xfaster/xfaster_exec.py`

 * *Files 2% similar despite different names*

```diff
@@ -870,14 +870,15 @@
     -------
     args : dict
         Dictionary of parsed options
     """
 
     import argparse as ap
     from textwrap import dedent
+    from . import __version__ as version
 
     parser_opts = dict(
         description="Run the XFaster algorithm",
         formatter_class=ap.ArgumentDefaultsHelpFormatter,
     )
 
     # initialize parser
@@ -897,14 +898,17 @@
                 )
                 raise RuntimeError(msg)
 
         P = TestParser(**parser_opts)
     else:
         P = ap.ArgumentParser(**parser_opts)
 
+    # add --version option
+    P.add_argument("--version", action="version", version="%(prog)s " + version)
+
     # get default argument values from xfaster_run
     defaults = get_func_defaults(xfaster_run)
     defaults.pop("add_log", None)
     rem_args = list(defaults)
 
     # argument docstrings
     docstr = dedent(xfaster_run.__doc__).split("\n---------\n")[1]
@@ -929,15 +933,24 @@
                             "If False, ",
                             "If {}set, ".format("not " if not defaults[arg] else ""),
                         )
                 arg_docs[arg] = argdoc
             arg = line.split(":")[0].strip()
             argdoc = ""
 
-    def add_arg(P, name, argtype=None, default=None, short=None, help=None, **kwargs):
+    def add_arg(
+        P,
+        name,
+        argtype=None,
+        default=None,
+        short=None,
+        help=None,
+        positional=False,
+        **kwargs
+    ):
         """
         Helper function for populating command line arguments. Wrapper
         for ArgumentParser.add_argument.
 
         Arguments
         ---------
         P : argument parser instance
@@ -953,26 +966,31 @@
             Description of argument
         """
 
         if help is None:
             help = arg_docs.get(name, None)
 
         name = name.replace("-", "_")
-        argname = "--{}".format(name.replace("_", "-"))
+        if positional:
+            argname = name
+        else:
+            argname = "--{}".format(name.replace("_", "-"))
         altname = kwargs.pop("altname", None)
 
         if default is None:
             default = defaults.get(name, None)
         if name in rem_args:
             rem_args.remove(name)
 
         if help is None:
             raise ValueError("Missing help text for argument {}".format(name))
 
-        opts = dict(default=default, help=help, dest=name, action="store")
+        opts = dict(default=default, help=help, action="store")
+        if not positional:
+            opts["dest"] = name
         opts.update(**kwargs)
 
         if default is True:
             argname = "--no-{}".format(name.replace("_", "-"))
             opts["action"] = "store_false"
         elif default is False:
             opts["action"] = "store_true"
@@ -1003,14 +1021,15 @@
     parser_opts.pop("description")
 
     # populate subparsers
     for mode, helptext in [
         ("run", "run xfaster"),
         ("submit", "submit xfaster job"),
         ("dump", "dump archive from xfaster job to stdout"),
+        ("diff", "compare two archive files"),
     ]:
 
         PP = S.add_parser(mode, help=helptext, **parser_opts)
 
         if mode == "dump":
             E = PP.add_mutually_exclusive_group(required=True)
             add_arg(E, "output_file", short="-f", help="Archive filename to print")
@@ -1037,14 +1056,34 @@
                 short="-v",
                 default=False,
                 action="store_true",
                 help="Print complete entries",
             )
             continue
 
+        if mode == "diff":
+            add_arg(PP, "file1", positional=True, help="File to compare")
+            add_arg(PP, "file2", positional=True, help="File to compare")
+            add_arg(
+                PP,
+                "keys",
+                short="-k",
+                nargs="+",
+                help="Select keys to print from each file",
+            )
+            add_arg(
+                PP,
+                "verbose",
+                short="-v",
+                default=False,
+                action="store_true",
+                help="Print status of all entries",
+            )
+            continue
+
         # common options
         G = PP.add_argument_group("common options")
         add_arg(G, "config", required=True)
         add_arg(G, "output_root", default=os.getcwd())
         add_arg(G, "output_tag")
         add_arg(
             G,
@@ -1307,15 +1346,15 @@
     for k, v in vars(args).items():
         if str(v).lower().strip() == "none":
             setattr(args, k, None)
         elif not np.isscalar(v) and len(v) == 1:
             v = v[0]
 
     # test mode
-    if args.mode not in ["submit", "dump"]:
+    if args.mode not in ["submit", "dump", "diff"]:
         if args.test:
             msg = ",\n".join(
                 "{}={!r}".format(k, v) for k, v in sorted(vars(args).items())
             )
             P.exit(0, "{}\nargument test\n".format(msg))
         delattr(args, "test")
 
@@ -1719,14 +1758,82 @@
                             txt = "shape {} array of {}".format(v.shape, repr(v.dtype))
                     else:
                         txt = txt[0] + " ..."
             print("    '{}': {},".format(k, txt))
         print("}")
 
 
+def xfaster_diff(file1, file2, keys=None, verbose=False):
+    """
+    Compare two output archive files to each other.  Uses setdiff or numpy.diff
+    as appropriate.
+
+    Arguments
+    ---------
+    file1 : str
+    file2 : str
+        Filenames to compare to each other
+    keys : list of str
+        List of keys to compare between files
+    verbose : bool
+        If True, print the status of all keys, even if identical.  Otherwise,
+        only print the status for keys that do not match between files.
+    """
+
+    def load1(f):
+        d = pt.load_and_parse(f)
+        if keys is not None:
+            d = {k: d[k] for k in keys if k in d}
+        return d
+
+    data1, data2 = [load1(f) for f in [file1, file2]]
+
+    def compare(d1, d2, prefix=""):
+        if isinstance(d1, (str, int, float)) or d1 is None:
+            if (d1 is None and d2 is not None) or (d1 is not None and d1 != d2):
+                print("{}{} != {}".format(prefix, d1, d2))
+            elif verbose:
+                print("{} SAME: {}".format(prefix, d1))
+
+        elif isinstance(d1, (list, np.ndarray)):
+            d1, d2 = [np.asarray(x) for x in [d1, d2]]
+            if d1.dtype.kind in ['U', 'S']:
+                s1 = set(d1.ravel())
+                s2 = set(d2.ravel())
+                sd = s1 - s2
+                if sd:
+                    print("{}only in {}: {}".format(prefix, file1, sd))
+                sd = s2 - s1
+                if sd:
+                    print("{}only in {}: {}".format(prefix, file2, sd))
+                if verbose and not s1 ^ s2:
+                    print("{}SAME".format(prefix))
+
+            elif not np.allclose(d1, d2):
+                print("{}{}".format(prefix, d1 - d2))
+
+            elif verbose:
+                print("{}ALL CLOSE".format(prefix))
+
+        elif isinstance(d1, dict):
+            all_keys = sorted(set(d1) | set(d2))
+            for k in all_keys:
+                if k not in d1:
+                    print("{}{}: only in {}".format(prefix, k, file2))
+                elif k not in d2:
+                    print("{}{}: only in {}".format(prefix, k, file1))
+                else:
+                    compare(d1[k], d2[k], "{}{}: ".format(prefix, k))
+
+        else:
+            raise ValueError("{}: parser error: {} {}".format(prefix, type(d1), d1))
+
+    compare(data1, data2)
+
+
 def xfaster_main():
     """
     Main entry point for command-line interface.
     """
     # parse arguments
     args = xfaster_parse()
     mode = args.pop("mode")
@@ -1738,7 +1845,11 @@
     elif mode == "run":
         # run the analysis
         xfaster_run(**args)
 
     elif mode == "dump":
         # dump archive files to stdout
         xfaster_dump(**args)
+
+    elif mode == "diff":
+        # diff archive files
+        xfaster_diff(**args)
```

