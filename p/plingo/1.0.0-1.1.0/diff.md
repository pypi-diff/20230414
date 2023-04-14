# Comparing `tmp/plingo-1.0.0.tar.gz` & `tmp/plingo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plingo-1.0.0.tar", last modified: Tue Jun  7 11:59:11 2022, max compression
+gzip compressed data, was "plingo-1.1.0.tar", last modified: Fri Apr 14 18:13:01 2023, max compression
```

## Comparing `plingo-1.0.0.tar` & `plingo-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 11:59:11.832620 plingo-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-06-07 11:58:58.000000 plingo-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6626 2022-06-07 11:59:11.832620 plingo-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6348 2022-06-07 11:58:58.000000 plingo-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 11:59:11.832620 plingo-1.0.0/plingo/
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-06-07 11:58:58.000000 plingo-1.0.0/plingo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9504 2022-06-07 11:58:58.000000 plingo-1.0.0/plingo/opt.py
--rw-r--r--   0 runner    (1001) docker     (121)    10850 2022-06-07 11:58:58.000000 plingo-1.0.0/plingo/plingo_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     6316 2022-06-07 11:58:58.000000 plingo-1.0.0/plingo/plog.py
--rw-r--r--   0 runner    (1001) docker     (121)     2934 2022-06-07 11:58:58.000000 plingo-1.0.0/plingo/probability.py
--rw-r--r--   0 runner    (1001) docker     (121)     2292 2022-06-07 11:58:58.000000 plingo-1.0.0/plingo/query.py
--rw-r--r--   0 runner    (1001) docker     (121)    10703 2022-06-07 11:58:58.000000 plingo-1.0.0/plingo/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 11:59:11.832620 plingo-1.0.0/plingo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6626 2022-06-07 11:59:11.000000 plingo-1.0.0/plingo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-06-07 11:59:11.000000 plingo-1.0.0/plingo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 11:59:11.000000 plingo-1.0.0/plingo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-06-07 11:59:11.000000 plingo-1.0.0/plingo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-07 11:59:11.000000 plingo-1.0.0/plingo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-07 11:59:11.000000 plingo-1.0.0/plingo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-06-07 11:59:11.832620 plingo-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      102 2022-06-07 11:58:58.000000 plingo-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:13:01.794988 plingo-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-14 18:12:53.000000 plingo-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-04-14 18:13:01.794988 plingo-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7185 2023-04-14 18:12:53.000000 plingo-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:13:01.794988 plingo-1.1.0/plingo/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-14 18:12:53.000000 plingo-1.1.0/plingo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9728 2023-04-14 18:12:53.000000 plingo-1.1.0/plingo/meta_problog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-04-14 18:12:53.000000 plingo-1.1.0/plingo/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12184 2023-04-14 18:12:53.000000 plingo-1.1.0/plingo/plingo_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-04-14 18:12:53.000000 plingo-1.1.0/plingo/plog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-04-14 18:12:53.000000 plingo-1.1.0/plingo/probability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-14 18:12:53.000000 plingo-1.1.0/plingo/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-04-14 18:12:53.000000 plingo-1.1.0/plingo/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 18:13:01.794988 plingo-1.1.0/plingo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-04-14 18:13:01.000000 plingo-1.1.0/plingo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-14 18:13:01.000000 plingo-1.1.0/plingo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 18:13:01.000000 plingo-1.1.0/plingo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-14 18:13:01.000000 plingo-1.1.0/plingo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-14 18:13:01.000000 plingo-1.1.0/plingo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 18:13:01.000000 plingo-1.1.0/plingo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-14 18:13:01.794988 plingo-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 18:12:53.000000 plingo-1.1.0/setup.py
```

### Comparing `plingo-1.0.0/LICENSE` & `plingo-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plingo-1.0.0/PKG-INFO` & `plingo-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,44 @@
-Metadata-Version: 2.1
-Name: plingo
-Version: 1.0.0
-Summary: Probabilistic extension for clingo
-Home-page: https://github.com/nrueh/plingo/
-Author: Nicolas Rühling
-Author-email: nruehling@uni-potsdam.de
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Plingo
 
 A system for **probabilistic reasoning in clingo**.
 
 The system is based on LP^MLN, and provides **front-ends** for different probabilistic logic languages:
 - *lpmln* [[1]](#1)
 - *p-log* [[2]](#2)
 - *problog* [[3]](#3).
 
 While the basic **syntax** of *plingo* is the same as the one of *clingo*, its **semantics** relies on re-interpreting the cost of a stable model at priority level `0` as a measure of its probability.
 
 Solving exploits the relation between most probable stable models and optimal stable models [[4]](#4); it relies on *clingo*'s optimization and enumeration modes, as well as an **approximation method** based on answer set enumeration in the order of optimality [[5]](#5).
 
 The *plingo* system can be used to solve two **reasoning tasks**:
-- MAP inference: find a most probable stable model
+- MPE inference: find a most probable explanation (stable model)
 - Marginal inference: find all stable models and their probabilities
 
 A number of **examples** can be found [here](https://github.com/potassco/plingo/tree/main/examples). There are also sub-directories containing examples using our front-ends for the other probabilistic logic languages.
 
 ## Installation
 
-#### With coda 
+#### With coda
 
 ```
 conda install -c potassco plingo
 ```
 
 #### With pip
 
 ```
 pip install plingo
 ```
 
-#### From source 
+#### From source
 
 ```
-git clone https://github.com/nrueh/plingo.git
+git clone https://github.com/potassco/plingo.git
 cd plingo
 pip install .
 ```
 
 
 ## Usage
 
@@ -70,41 +59,50 @@
 
 - `--evid=file`
 
     Provides an evidence file to the program (`.lp` file with clingo syntax rules)
 
 - `--frontend=mode`
 
-    Specifies which frontend to use (´lpmln´, ´lpmln-alt´, ´problog´, ´plog´).
-    Mode ´lpmln-alt´ is the alternative definition where hard rules have to be satisfied. 
-    When using mode ´lpmln hard rules are also translated which can be useful for debugging or resolving inconsistencies in the program.
+    Specifies which frontend to use (`lpmln`, `lpmln-alt`, `problog`, `plog`).
+    Mode `lpmln-alt` is the alternative definition where hard rules have to be satisfied.
+    When using mode `lpmln` hard rules are also translated which can be useful for debugging or resolving inconsistencies in the program.
+
+- `--problog=output'`
+
+    Uses reificiation to translate a plingo program to a program which be can be given as input to the ProbLog system.
+    The ProbLog program is saved under the path given in `output`.
+    The input can also be given in any of the frontends (`lpmln`, `lpmln-alt`, `problog`, `plog`).
+
 
 - `--query='atom'`
 
     Adds a query atom `atom`, e.g. using the example from above `--query='bird(jo)'`. The argument has to be inside single quotation marks (otherwise the command-line might not be able to parse it correctly).
 
 - `--two-solve-calls`
 
     Uses two solve calls: The first one finds the minimal bound for weak constraints priorities higher than 0. The second one solves for probabilistic stable models of LP^MLN.
 
 - `--unsat`
 
     Uses the conversion with `unsat` atoms
 
-#### Examples 
-##### MAP estimate
+#### Examples
+
+##### MPE
+
 
 Find a most probable stable model
 
 
 ```
 plingo examples/lpmln/birds.plp --frontend lpmln-alt
 ```
 ```
-plingo version 1.0.0
+plingo version 1.1.0
 Reading from examples/birds.lp
 Solving...
 Answer: 1
 
 Optimization: 300000
 Answer: 2
 residentBird(jo) bird(jo)
@@ -117,21 +115,21 @@
 Calls        : 1
 Time         : 0.005s (Solving: 0.00s 1st Model: 0.00s Unsat: 0.00s)
 CPU Time     : 0.005s
 ```
 
 ##### Marginal probabilities
 
-To list all stable models, add the flag `--all`. 
+To list all stable models, add the flag `--all`.
 
 ```
 plingo examples/lpmln/birds.plp --all --frontend lpmln-alt
 ```
 ```
-plingo version 1.0.0
+plingo version 1.1.0
 Reading from examples/birds.lp
 Solving...
 Answer: 1
 
 Optimization: 300000
 Answer: 2
 residentBird(jo) bird(jo)
@@ -152,49 +150,62 @@
   Optimum    : yes
 Calls        : 1
 Time         : 0.006s (Solving: 0.00s 1st Model: 0.00s Unsat: 0.00s)
 CPU Time     : 0.006s
 ```
 
 #### Approximation algorithm
-For large problems it is infeasible to determine all stable models. 
+For large problems it is infeasible to determine all stable models.
 Plingo offers an option to determine approximate probabilities using
 answer set enumeration by optimality (ASEO) [[1]](#1).
 
 For approximation of probabilistic queries it is recommended to use the `--opt-enum` option together with `--balanced=N`.
 
 - `--opt-enum`
 
-    Enumerates stable models by optimality. 
+    Enumerates stable models by optimality.
     This can be used for approximating probabilities and queries.
     Recommended to use along with -q1 to suppress printing of intermediate models
-    
+
 - `--balanced=N`
 
     Approximates a query in a balanced way, i.e. it will determine N stable models containing the query, and N stable models *not* containing the query. This overwrites clingo's `--models` option. Works only for a single ground query atom!
 - `--use-backend`
 
     Adds constraints for query approximation in backend instead of using assumptions.
 
+#### Using ProbLog as a solver
+With the `--problog` option it is possible to translate a plingo program to a problog program
+which can be solved by the ProbLog system (https://github.com/ML-KULeuven/problog).
+This can also be combined with using any of the frontends.
+The input file needs to contain at least one query when using marginal inference.
+```
+plingo examples/lpmln/birds.plp examples/lpmln/birds_query.plp --frontend=lpmln-alt --problog=problog.lp >/dev/null; problog problog.lp
+```
+```
+show(residentBird(jo)): 0.66524095
+```
+
 
 ## Input Language
-Syntactically, LPMLN differs between "soft" rules and "hard" rules, where "soft" rules have a (real number) weight and "hard" rules the weight "alpha". 
+Syntactically, LPMLN differs between "soft" rules and "hard" rules, where "soft" rules have a (real number) weight and "hard" rules the weight "alpha".
 
 Weights can be added by the theory atom `&weight/1` to the body of a rule. The argument has to be an integer or a string containing a float or an expression like `2/3`. For example
 ```
 a(X) :- b(X), &weight(5).
 b(X) :- &weight("-2/3").
 ```
 Further it is possible to use the theory atoms `&log/1` or `&problog/1` which only accept strings as arguments. The atom `&log/1` uses the natural logarithm `log(p)` of its argument `p` as weight. The atom `&problog/1` uses the natural logarithm of `p/(1-p)` as its weight.
 Rules that do not have any weight in the body are assumed to be hard rules.
 
 To compute LPMLN programs, a rule in an LPMLN program is converted to ASP with weak constraints
 
 By default, only soft rules are converted. To convert hard rules as well, the `--hr` flag can be added on the command line. This option essentially makes hard rules optional, whereas in the default setting all hard rules have to be satisfied as usually in ASP.
 
+
 ## References
 <a id="1">[1]</a>
 J. Lee and Y. Wang. (2016).
 Weighted Rules under the Stable Model Semantics
 
 
 <a id="2">[2]</a>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `plingo-1.0.0/README.md` & `plingo-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,55 @@
+Metadata-Version: 2.1
+Name: plingo
+Version: 1.1.0
+Summary: Probabilistic extension for clingo
+Home-page: https://github.com/nrueh/plingo/
+Author: Nicolas Rühling
+Author-email: nruehling@uni-potsdam.de
+License: MIT
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Plingo
 
 A system for **probabilistic reasoning in clingo**.
 
 The system is based on LP^MLN, and provides **front-ends** for different probabilistic logic languages:
 - *lpmln* [[1]](#1)
 - *p-log* [[2]](#2)
 - *problog* [[3]](#3).
 
 While the basic **syntax** of *plingo* is the same as the one of *clingo*, its **semantics** relies on re-interpreting the cost of a stable model at priority level `0` as a measure of its probability.
 
 Solving exploits the relation between most probable stable models and optimal stable models [[4]](#4); it relies on *clingo*'s optimization and enumeration modes, as well as an **approximation method** based on answer set enumeration in the order of optimality [[5]](#5).
 
 The *plingo* system can be used to solve two **reasoning tasks**:
-- MAP inference: find a most probable stable model
+- MPE inference: find a most probable explanation (stable model)
 - Marginal inference: find all stable models and their probabilities
 
 A number of **examples** can be found [here](https://github.com/potassco/plingo/tree/main/examples). There are also sub-directories containing examples using our front-ends for the other probabilistic logic languages.
 
 ## Installation
 
-#### With coda 
+#### With coda
 
 ```
 conda install -c potassco plingo
 ```
 
 #### With pip
 
 ```
 pip install plingo
 ```
 
-#### From source 
+#### From source
 
 ```
-git clone https://github.com/nrueh/plingo.git
+git clone https://github.com/potassco/plingo.git
 cd plingo
 pip install .
 ```
 
 
 ## Usage
 
@@ -59,41 +70,50 @@
 
 - `--evid=file`
 
     Provides an evidence file to the program (`.lp` file with clingo syntax rules)
 
 - `--frontend=mode`
 
-    Specifies which frontend to use (´lpmln´, ´lpmln-alt´, ´problog´, ´plog´).
-    Mode ´lpmln-alt´ is the alternative definition where hard rules have to be satisfied. 
-    When using mode ´lpmln hard rules are also translated which can be useful for debugging or resolving inconsistencies in the program.
+    Specifies which frontend to use (`lpmln`, `lpmln-alt`, `problog`, `plog`).
+    Mode `lpmln-alt` is the alternative definition where hard rules have to be satisfied.
+    When using mode `lpmln` hard rules are also translated which can be useful for debugging or resolving inconsistencies in the program.
+
+- `--problog=output'`
+
+    Uses reificiation to translate a plingo program to a program which be can be given as input to the ProbLog system.
+    The ProbLog program is saved under the path given in `output`.
+    The input can also be given in any of the frontends (`lpmln`, `lpmln-alt`, `problog`, `plog`).
+
 
 - `--query='atom'`
 
     Adds a query atom `atom`, e.g. using the example from above `--query='bird(jo)'`. The argument has to be inside single quotation marks (otherwise the command-line might not be able to parse it correctly).
 
 - `--two-solve-calls`
 
     Uses two solve calls: The first one finds the minimal bound for weak constraints priorities higher than 0. The second one solves for probabilistic stable models of LP^MLN.
 
 - `--unsat`
 
     Uses the conversion with `unsat` atoms
 
-#### Examples 
-##### MAP estimate
+#### Examples
+
+##### MPE
+
 
 Find a most probable stable model
 
 
 ```
 plingo examples/lpmln/birds.plp --frontend lpmln-alt
 ```
 ```
-plingo version 1.0.0
+plingo version 1.1.0
 Reading from examples/birds.lp
 Solving...
 Answer: 1
 
 Optimization: 300000
 Answer: 2
 residentBird(jo) bird(jo)
@@ -106,21 +126,21 @@
 Calls        : 1
 Time         : 0.005s (Solving: 0.00s 1st Model: 0.00s Unsat: 0.00s)
 CPU Time     : 0.005s
 ```
 
 ##### Marginal probabilities
 
-To list all stable models, add the flag `--all`. 
+To list all stable models, add the flag `--all`.
 
 ```
 plingo examples/lpmln/birds.plp --all --frontend lpmln-alt
 ```
 ```
-plingo version 1.0.0
+plingo version 1.1.0
 Reading from examples/birds.lp
 Solving...
 Answer: 1
 
 Optimization: 300000
 Answer: 2
 residentBird(jo) bird(jo)
@@ -141,49 +161,62 @@
   Optimum    : yes
 Calls        : 1
 Time         : 0.006s (Solving: 0.00s 1st Model: 0.00s Unsat: 0.00s)
 CPU Time     : 0.006s
 ```
 
 #### Approximation algorithm
-For large problems it is infeasible to determine all stable models. 
+For large problems it is infeasible to determine all stable models.
 Plingo offers an option to determine approximate probabilities using
 answer set enumeration by optimality (ASEO) [[1]](#1).
 
 For approximation of probabilistic queries it is recommended to use the `--opt-enum` option together with `--balanced=N`.
 
 - `--opt-enum`
 
-    Enumerates stable models by optimality. 
+    Enumerates stable models by optimality.
     This can be used for approximating probabilities and queries.
     Recommended to use along with -q1 to suppress printing of intermediate models
-    
+
 - `--balanced=N`
 
     Approximates a query in a balanced way, i.e. it will determine N stable models containing the query, and N stable models *not* containing the query. This overwrites clingo's `--models` option. Works only for a single ground query atom!
 - `--use-backend`
 
     Adds constraints for query approximation in backend instead of using assumptions.
 
+#### Using ProbLog as a solver
+With the `--problog` option it is possible to translate a plingo program to a problog program
+which can be solved by the ProbLog system (https://github.com/ML-KULeuven/problog).
+This can also be combined with using any of the frontends.
+The input file needs to contain at least one query when using marginal inference.
+```
+plingo examples/lpmln/birds.plp examples/lpmln/birds_query.plp --frontend=lpmln-alt --problog=problog.lp >/dev/null; problog problog.lp
+```
+```
+show(residentBird(jo)): 0.66524095
+```
+
 
 ## Input Language
-Syntactically, LPMLN differs between "soft" rules and "hard" rules, where "soft" rules have a (real number) weight and "hard" rules the weight "alpha". 
+Syntactically, LPMLN differs between "soft" rules and "hard" rules, where "soft" rules have a (real number) weight and "hard" rules the weight "alpha".
 
 Weights can be added by the theory atom `&weight/1` to the body of a rule. The argument has to be an integer or a string containing a float or an expression like `2/3`. For example
 ```
 a(X) :- b(X), &weight(5).
 b(X) :- &weight("-2/3").
 ```
 Further it is possible to use the theory atoms `&log/1` or `&problog/1` which only accept strings as arguments. The atom `&log/1` uses the natural logarithm `log(p)` of its argument `p` as weight. The atom `&problog/1` uses the natural logarithm of `p/(1-p)` as its weight.
 Rules that do not have any weight in the body are assumed to be hard rules.
 
 To compute LPMLN programs, a rule in an LPMLN program is converted to ASP with weak constraints
 
 By default, only soft rules are converted. To convert hard rules as well, the `--hr` flag can be added on the command line. This option essentially makes hard rules optional, whereas in the default setting all hard rules have to be satisfied as usually in ASP.
 
+
 ## References
 <a id="1">[1]</a>
 J. Lee and Y. Wang. (2016).
 Weighted Rules under the Stable Model Semantics
 
 
 <a id="2">[2]</a>
```

### Comparing `plingo-1.0.0/plingo/opt.py` & `plingo-1.1.0/plingo/opt.py`

 * *Files identical despite different names*

### Comparing `plingo-1.0.0/plingo/plingo_app.py` & `plingo-1.1.0/plingo/plingo_app.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from typing import cast, Sequence, List, Tuple, Optional
+from os.path import join
 import sys
+from tempfile import mkdtemp
+from typing import cast, Sequence, List, Tuple, Optional
 
 from clingo.application import Application, ApplicationOptions, Flag
 from clingo.ast import AST, ProgramBuilder, parse_files, parse_string
 from clingo.configuration import Configuration
 from clingo.control import Control
 from clingo.script import enable_python
 from clingo.symbol import Function, Symbol
 
+from .meta_problog import create_reified_problog
 from .transformer import PlingoTransformer
 from .query import collect_query, check_model_for_query
 from .opt import MinObs, OptEnum
 from .plog import get_meta_encoding
 from .probability import ProbabilityModule
 
 THEORY = """
@@ -39,29 +42,33 @@
     opt_enum: Flag
     use_backend: Flag
     frontend: str
     query: List[Tuple[Symbol, List[int]]]
     evidence_file: str
     balanced_models: Optional[int]
     power_of_ten: int
+    temp: str
+    problog: str
 
     program_name: str = "plingo"
-    version: str = "1.0.0"
+    version: str = "1.1.0"
 
     def __init__(self):
         self.display_all_probs = Flag(False)
         self.use_unsat_approach = Flag(False)
         self.two_solve_calls = Flag(False)
         self.opt_enum = Flag(False)
         self.use_backend = Flag(False)
         self.frontend = 'plingo'
         self.query = []
         self.evidence_file = ''
         self.balanced_models = None
         self.power_of_ten = 5
+        self.temp = join(mkdtemp(), 'temp.lp')
+        self.problog = ''
 
     def _parse_frontend(self, value: str) -> bool:
         """
         Parse the given frontend mode.
         Possible options are:
         lpmln, lpmln-alt, problog and plog.
         By default the variable is set to plingo.
@@ -109,14 +116,20 @@
             return True
         except ValueError:
             print(
                 "Warning: --balanced N has to be set to an integer large than 0."
             )
             return False
 
+    def _parse_problog(self, value) -> bool:
+        with open(self.temp, 'w') as temp:
+            temp.write('#show query/1.\n')
+        self.problog = value
+        return True
+
     def register_options(self, options: ApplicationOptions) -> None:
         """
         Register application option.
         """
         group = 'Plingo Options'
         options.add_flag(group, 'all,a', 'Display all probabilities',
                          self.display_all_probs)
@@ -149,14 +162,18 @@
                             This overwrites the --models option
                             This works only for a single (ground) query atom!''',
             self._parse_balanced_query)
         options.add_flag(
             group, 'use-backend',
             'Adds constraints for query approximation in backend instead of using assumptions.',
             self.use_backend)
+        options.add(
+            group, 'problog',
+            '''Translate input to ProbLog program and save in a file.
+                            Use as --problog=output.lp''', self._parse_problog)
 
     def validate_options(self) -> bool:
         if self.two_solve_calls and self.frontend != 'lpmln':
             print(
                 'The two-solve-calls mode only works if hard rules are translated (--frontend lpmln).'
             )
             return False
@@ -174,36 +191,53 @@
 
     def _read(self, path: str):
         if path == "-":
             return sys.stdin.read()
         with open(path) as file_:
             return file_.read()
 
+    def _save_translation(self, rule):
+        rule = str(rule)
+        if rule != '#program base.':
+            with open(self.temp, 'a') as lp:
+                lp.write(f'{rule}\n')
+
     def _convert(self, ctl: Control, files: Sequence[str]):
         options = [
             self.frontend, self.use_unsat_approach, self.two_solve_calls,
             self.power_of_ten
         ]
-        with ProgramBuilder(ctl) as b:
-            pt = PlingoTransformer(options)
-            parse_files(files, lambda stm: b.add(cast(AST, pt.visit(stm, b))))
+        pt = PlingoTransformer(options)
+        if self.problog:
+            parse_files(
+                files, lambda stm: self._save_translation(
+                    pt.visit(stm, file=self.temp)))
+        else:
+            with ProgramBuilder(ctl) as b:
+                parse_files(
+                    files,
+                    lambda stm: b.add(cast(AST, pt.visit(stm, builder=b))))
 
     def _preprocessing(self, ctl: Control,
                        files: Sequence[str]) -> Tuple[Configuration, MinObs]:
         '''
         Performs some preprocessing.
         '''
         ctl.add("base", [], THEORY)
         ctl.add("base", [], self.evidence_file)
 
         # Add meta file for calculating P-Log
         if self.frontend == 'plog':
             enable_python()
             ctl.add("base", [], get_meta_encoding())
             ctl.add("base", [], f'#const _plingo_factor={self.power_of_ten}.')
+            if self.problog:
+                with open(self.temp, 'a') as lp:
+                    lp.write(f'{get_meta_encoding()}\n')
+                    lp.write(f'#const _plingo_factor={self.power_of_ten}.\n')
         if self.two_solve_calls:
             ctl.add("base", [], '#external _plingo_ext_helper.')
         # TODO: Make sure the _ext_helper atom is not contained in the program.
         # TODO: Change number of underscores for _ext_helper and plog meta atoms
 
         if not files:
             files = ["-"]
@@ -279,13 +313,16 @@
             probs.get_query_probability(self.query)
 
     def main(self, ctl: Control, files: Sequence[str]):
         '''
         Parse clingo program with weights and convert to ASP with weak constraints.
         '''
         obs = self._preprocessing(ctl, files)
-        ctl.ground([("base", [])])
-        self.query = collect_query(ctl.theory_atoms, self.balanced_models)
-        model_costs = self._solve(ctl, obs)
+        if self.problog:
+            create_reified_problog(self.temp, self.problog)
+        else:
+            ctl.ground([("base", [])])
+            self.query = collect_query(ctl.theory_atoms, self.balanced_models)
+            model_costs = self._solve(ctl, obs)
 
-        if model_costs != []:
-            self._probabilities(model_costs, obs.priorities)
+            if model_costs != []:
+                self._probabilities(model_costs, obs.priorities)
```

### Comparing `plingo-1.0.0/plingo/plog.py` & `plingo-1.1.0/plingo/plog.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,30 +153,37 @@
 
 _plingo_numsum(E,Y) :- _plingo_default(E), Y = #sum { @intpr(Pr),A : _plingo_random(E,A), _plingo_pr(E,A,Pr) }.
 _plingo_densum(E,M) :- _plingo_default(E), M = #count{ A : _plingo_random(E,A), not _plingo_pr(E,A,_) }.
 
 :~ _plingo_pr(E,Pr), _plingo_no_int(E).       [   -@log(Pr,_plingo_factor),E]
 :- _plingo_pr(E,Pr), _plingo_no_int(E),           Pr = 0.
 
+% Weight calculation for default probabilities:
+% We calculate (1-Y)/M, with Y the total assigned probability
+% and M the number of default outcomes
+% This corresponds to log(1-Y)-log(M) (with negative weights because of optimization)
+
 :~ _plingo_numsum(E,Y), @intpr(1)-Y > 0.   [-@log(@frac(@intpr(1)-Y,@intpr(1)),_plingo_factor),num,E]
 :- _plingo_numsum(E,Y),                    @intpr(1) - Y <= 0.
 
-:~ _plingo_densum(E,M), M > 1.             [-@log(@frac(1,M),_plingo_factor),den,E]
+:~ _plingo_densum(E,M), M > 1.             [@log(M,_plingo_factor),den,E]
 :- _plingo_densum(E,M),                    M = 0.
 
-
 #script (python)
 from clingo import Number, String
 from math import log as mathlog
 
 def log(a, factor):
     factor = factor.number
-    ln = mathlog(float(eval(a.string)))
-    weight = Number(int(ln * (10**factor)))
-    return weight
+    if str(a.type) == 'SymbolType.String':
+        a =  float(eval(a.string))
+    elif str(a.type) == 'SymbolType.Number':
+        a = a.number
+    ln = mathlog(a)
+    return Number(int(ln * (10**factor)))
 
 def frac(n,d):
     return String(f'{n.number}/{d.number}')
 
 def intpr(a):
     factor = 10**6
     if str(a.type) == 'SymbolType.String':
```

### Comparing `plingo-1.0.0/plingo/probability.py` & `plingo-1.1.0/plingo/probability.py`

 * *Files identical despite different names*

### Comparing `plingo-1.0.0/plingo/query.py` & `plingo-1.1.0/plingo/query.py`

 * *Files identical despite different names*

### Comparing `plingo-1.0.0/plingo/transformer.py` & `plingo-1.1.0/plingo/transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -152,19 +152,22 @@
                 body.insert(0, ext_helper_atom)
 
             weak_constraint = ast.Minimize(loc, constraint_weight, priority,
                                            [idx, self.global_variables], body)
             asp_rules.append(weak_constraint)
             return asp_rules
 
-    def visit_Rule(self, rule: AST, builder: ProgramBuilder):
+    def visit_Rule(self, rule: AST, **kwargs):  #*builder: ProgramBuilder):
         """
         Visits an LP^MLN rule, converts it to three ASP rules
         if necessary and adds the result to the program builder.
         """
+        builder = kwargs.get('builder', None)
+        file = kwargs.get('file', None)
+
         # Set weight to alpha by default
         head = rule.head
         body = rule.body
 
         if self.frontend != 'lpmln' and str(
                 head.ast_type) != 'ASTType.TheoryAtom' and len(body) == 0:
             return rule
@@ -175,14 +178,23 @@
 
         # Traverse head and body to look for weights and variables
         head = self.visit(head)
         body = self.visit(body)
 
         # Query theory atoms are grounded and then processed
         if self.theory_type == 'query':
+            if file:
+                query_arg = rule.head.term.arguments[0]
+                if str(query_arg.ast_type) == 'ASTType.SymbolicTerm':
+                    show_atom = f'#show {query_arg}/0.'
+                else:
+                    show_atom = f'#show {query_arg.name}/{len(query_arg.arguments)}.'
+                rule = str(rule)
+                rule = rule[1:rule.rfind(')') + 1] + '.'
+                rule = f'{rule}\n{show_atom}'
             return rule
 
         # Evidence theory atoms are converted to integrity constraints
         elif self.theory_type == 'evidence':
             int_constraint_head = ast.Literal(head.location, ast.Sign.NoSign,
                                               ast.BooleanConstant(False))
             return ast.Rule(rule.location, int_constraint_head, [head])
@@ -199,15 +211,19 @@
             return rule
         else:
             asp_rules = self._convert_rule(head, body)
             self.rule_idx += 1
 
         # We might obtain more than one rule,
         for r in asp_rules[:-1]:
-            builder.add(r)
+            if builder:
+                builder.add(r)
+            elif file:
+                with open(file, 'a') as lp:
+                    lp.write(f'{str(r)}\n')
 
         return asp_rules[-1]
 
     def visit_Minimize(self, rule: AST, *args: Any, **kwargs: Any) -> AST:
         if self.frontend == 'plingo':
             # In plingo weak constraint weights can be strings
             symbol = rule.weight.symbol
```

### Comparing `plingo-1.0.0/plingo.egg-info/PKG-INFO` & `plingo-1.1.0/plingo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plingo
-Version: 1.0.0
+Version: 1.1.0
 Summary: Probabilistic extension for clingo
 Home-page: https://github.com/nrueh/plingo/
 Author: Nicolas Rühling
 Author-email: nruehling@uni-potsdam.de
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -19,37 +19,37 @@
 - *problog* [[3]](#3).
 
 While the basic **syntax** of *plingo* is the same as the one of *clingo*, its **semantics** relies on re-interpreting the cost of a stable model at priority level `0` as a measure of its probability.
 
 Solving exploits the relation between most probable stable models and optimal stable models [[4]](#4); it relies on *clingo*'s optimization and enumeration modes, as well as an **approximation method** based on answer set enumeration in the order of optimality [[5]](#5).
 
 The *plingo* system can be used to solve two **reasoning tasks**:
-- MAP inference: find a most probable stable model
+- MPE inference: find a most probable explanation (stable model)
 - Marginal inference: find all stable models and their probabilities
 
 A number of **examples** can be found [here](https://github.com/potassco/plingo/tree/main/examples). There are also sub-directories containing examples using our front-ends for the other probabilistic logic languages.
 
 ## Installation
 
-#### With coda 
+#### With coda
 
 ```
 conda install -c potassco plingo
 ```
 
 #### With pip
 
 ```
 pip install plingo
 ```
 
-#### From source 
+#### From source
 
 ```
-git clone https://github.com/nrueh/plingo.git
+git clone https://github.com/potassco/plingo.git
 cd plingo
 pip install .
 ```
 
 
 ## Usage
 
@@ -70,41 +70,50 @@
 
 - `--evid=file`
 
     Provides an evidence file to the program (`.lp` file with clingo syntax rules)
 
 - `--frontend=mode`
 
-    Specifies which frontend to use (´lpmln´, ´lpmln-alt´, ´problog´, ´plog´).
-    Mode ´lpmln-alt´ is the alternative definition where hard rules have to be satisfied. 
-    When using mode ´lpmln hard rules are also translated which can be useful for debugging or resolving inconsistencies in the program.
+    Specifies which frontend to use (`lpmln`, `lpmln-alt`, `problog`, `plog`).
+    Mode `lpmln-alt` is the alternative definition where hard rules have to be satisfied.
+    When using mode `lpmln` hard rules are also translated which can be useful for debugging or resolving inconsistencies in the program.
+
+- `--problog=output'`
+
+    Uses reificiation to translate a plingo program to a program which be can be given as input to the ProbLog system.
+    The ProbLog program is saved under the path given in `output`.
+    The input can also be given in any of the frontends (`lpmln`, `lpmln-alt`, `problog`, `plog`).
+
 
 - `--query='atom'`
 
     Adds a query atom `atom`, e.g. using the example from above `--query='bird(jo)'`. The argument has to be inside single quotation marks (otherwise the command-line might not be able to parse it correctly).
 
 - `--two-solve-calls`
 
     Uses two solve calls: The first one finds the minimal bound for weak constraints priorities higher than 0. The second one solves for probabilistic stable models of LP^MLN.
 
 - `--unsat`
 
     Uses the conversion with `unsat` atoms
 
-#### Examples 
-##### MAP estimate
+#### Examples
+
+##### MPE
+
 
 Find a most probable stable model
 
 
 ```
 plingo examples/lpmln/birds.plp --frontend lpmln-alt
 ```
 ```
-plingo version 1.0.0
+plingo version 1.1.0
 Reading from examples/birds.lp
 Solving...
 Answer: 1
 
 Optimization: 300000
 Answer: 2
 residentBird(jo) bird(jo)
@@ -117,21 +126,21 @@
 Calls        : 1
 Time         : 0.005s (Solving: 0.00s 1st Model: 0.00s Unsat: 0.00s)
 CPU Time     : 0.005s
 ```
 
 ##### Marginal probabilities
 
-To list all stable models, add the flag `--all`. 
+To list all stable models, add the flag `--all`.
 
 ```
 plingo examples/lpmln/birds.plp --all --frontend lpmln-alt
 ```
 ```
-plingo version 1.0.0
+plingo version 1.1.0
 Reading from examples/birds.lp
 Solving...
 Answer: 1
 
 Optimization: 300000
 Answer: 2
 residentBird(jo) bird(jo)
@@ -152,49 +161,62 @@
   Optimum    : yes
 Calls        : 1
 Time         : 0.006s (Solving: 0.00s 1st Model: 0.00s Unsat: 0.00s)
 CPU Time     : 0.006s
 ```
 
 #### Approximation algorithm
-For large problems it is infeasible to determine all stable models. 
+For large problems it is infeasible to determine all stable models.
 Plingo offers an option to determine approximate probabilities using
 answer set enumeration by optimality (ASEO) [[1]](#1).
 
 For approximation of probabilistic queries it is recommended to use the `--opt-enum` option together with `--balanced=N`.
 
 - `--opt-enum`
 
-    Enumerates stable models by optimality. 
+    Enumerates stable models by optimality.
     This can be used for approximating probabilities and queries.
     Recommended to use along with -q1 to suppress printing of intermediate models
-    
+
 - `--balanced=N`
 
     Approximates a query in a balanced way, i.e. it will determine N stable models containing the query, and N stable models *not* containing the query. This overwrites clingo's `--models` option. Works only for a single ground query atom!
 - `--use-backend`
 
     Adds constraints for query approximation in backend instead of using assumptions.
 
+#### Using ProbLog as a solver
+With the `--problog` option it is possible to translate a plingo program to a problog program
+which can be solved by the ProbLog system (https://github.com/ML-KULeuven/problog).
+This can also be combined with using any of the frontends.
+The input file needs to contain at least one query when using marginal inference.
+```
+plingo examples/lpmln/birds.plp examples/lpmln/birds_query.plp --frontend=lpmln-alt --problog=problog.lp >/dev/null; problog problog.lp
+```
+```
+show(residentBird(jo)): 0.66524095
+```
+
 
 ## Input Language
-Syntactically, LPMLN differs between "soft" rules and "hard" rules, where "soft" rules have a (real number) weight and "hard" rules the weight "alpha". 
+Syntactically, LPMLN differs between "soft" rules and "hard" rules, where "soft" rules have a (real number) weight and "hard" rules the weight "alpha".
 
 Weights can be added by the theory atom `&weight/1` to the body of a rule. The argument has to be an integer or a string containing a float or an expression like `2/3`. For example
 ```
 a(X) :- b(X), &weight(5).
 b(X) :- &weight("-2/3").
 ```
 Further it is possible to use the theory atoms `&log/1` or `&problog/1` which only accept strings as arguments. The atom `&log/1` uses the natural logarithm `log(p)` of its argument `p` as weight. The atom `&problog/1` uses the natural logarithm of `p/(1-p)` as its weight.
 Rules that do not have any weight in the body are assumed to be hard rules.
 
 To compute LPMLN programs, a rule in an LPMLN program is converted to ASP with weak constraints
 
 By default, only soft rules are converted. To convert hard rules as well, the `--hr` flag can be added on the command line. This option essentially makes hard rules optional, whereas in the default setting all hard rules have to be satisfied as usually in ASP.
 
+
 ## References
 <a id="1">[1]</a>
 J. Lee and Y. Wang. (2016).
 Weighted Rules under the Stable Model Semantics
 
 
 <a id="2">[2]</a>
```

