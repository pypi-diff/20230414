# Comparing `tmp/magicsoup-0.3.5.tar.gz` & `tmp/magicsoup-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magicsoup-0.3.5.tar", last modified: Wed Apr 12 15:01:06 2023, max compression
+gzip compressed data, was "magicsoup-0.3.6.tar", last modified: Fri Apr 14 20:16:29 2023, max compression
```

## Comparing `magicsoup-0.3.5.tar` & `magicsoup-0.3.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-12 15:01:06.880493 magicsoup-0.3.5/
--rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.3.5/LICENSE
--rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-12 15:01:06.880493 magicsoup-0.3.5/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)     4360 2023-04-07 09:06:36.000000 magicsoup-0.3.5/README.md
--rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.3.5/pyproject.toml
--rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-04-12 15:01:06.880493 magicsoup-0.3.5/setup.cfg
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-12 15:01:06.876493 magicsoup-0.3.5/src/
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-12 15:01:06.876493 magicsoup-0.3.5/src/magicsoup/
--rw-rw-r--   0 marc      (1000) marc      (1003)      151 2023-04-12 15:00:55.000000 magicsoup-0.3.5/src/magicsoup/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-08 10:04:41.000000 magicsoup-0.3.5/src/magicsoup/constants.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    23599 2023-04-07 15:09:15.000000 magicsoup-0.3.5/src/magicsoup/containers.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-12 15:01:06.876493 magicsoup-0.3.5/src/magicsoup/examples/
--rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.3.5/src/magicsoup/examples/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.3.5/src/magicsoup/examples/n2_fixing.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.3.5/src/magicsoup/examples/reverse_krebs.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1930 2023-02-16 21:19:27.000000 magicsoup-0.3.5/src/magicsoup/examples/wood_ljungdahl.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    11993 2023-04-06 09:43:57.000000 magicsoup-0.3.5/src/magicsoup/genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    28797 2023-04-07 15:20:43.000000 magicsoup-0.3.5/src/magicsoup/kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-04-12 14:59:48.000000 magicsoup-0.3.5/src/magicsoup/mutations.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.3.5/src/magicsoup/util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    43105 2023-04-11 15:46:53.000000 magicsoup-0.3.5/src/magicsoup/world.py
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-12 15:01:06.876493 magicsoup-0.3.5/src/magicsoup.egg-info/
--rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-12 15:01:06.000000 magicsoup-0.3.5/src/magicsoup.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1003)      647 2023-04-12 15:01:06.000000 magicsoup-0.3.5/src/magicsoup.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-04-12 15:01:06.000000 magicsoup-0.3.5/src/magicsoup.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-04-12 15:01:06.000000 magicsoup-0.3.5/src/magicsoup.egg-info/top_level.txt
-drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-12 15:01:06.880493 magicsoup-0.3.5/tests/
--rw-rw-r--   0 marc      (1000) marc      (1003)      710 2023-02-09 10:42:28.000000 magicsoup-0.3.5/tests/test_containers.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     6012 2023-04-06 09:44:07.000000 magicsoup-0.3.5/tests/test_genetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    46955 2023-04-06 09:24:16.000000 magicsoup-0.3.5/tests/test_kinetics.py
--rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-04-03 15:10:20.000000 magicsoup-0.3.5/tests/test_util.py
--rw-rw-r--   0 marc      (1000) marc      (1003)    18649 2023-04-11 15:52:20.000000 magicsoup-0.3.5/tests/test_world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-14 20:16:29.920780 magicsoup-0.3.6/
+-rw-rw-r--   0 marc      (1000) marc      (1003)    34888 2023-01-23 15:27:37.000000 magicsoup-0.3.6/LICENSE
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-14 20:16:29.916780 magicsoup-0.3.6/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4360 2023-04-07 09:06:36.000000 magicsoup-0.3.6/README.md
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1092 2023-01-26 15:22:43.000000 magicsoup-0.3.6/pyproject.toml
+-rw-rw-r--   0 marc      (1000) marc      (1003)       38 2023-04-14 20:16:29.920780 magicsoup-0.3.6/setup.cfg
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-14 20:16:29.916780 magicsoup-0.3.6/src/
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-14 20:16:29.916780 magicsoup-0.3.6/src/magicsoup/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      151 2023-04-14 20:15:25.000000 magicsoup-0.3.6/src/magicsoup/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1109 2023-04-08 10:04:41.000000 magicsoup-0.3.6/src/magicsoup/constants.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    23599 2023-04-07 15:09:15.000000 magicsoup-0.3.6/src/magicsoup/containers.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-14 20:16:29.916780 magicsoup-0.3.6/src/magicsoup/examples/
+-rw-rw-r--   0 marc      (1000) marc      (1003)        0 2023-01-23 15:27:37.000000 magicsoup-0.3.6/src/magicsoup/examples/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)      833 2023-01-23 15:27:37.000000 magicsoup-0.3.6/src/magicsoup/examples/n2_fixing.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1473 2023-01-23 15:27:37.000000 magicsoup-0.3.6/src/magicsoup/examples/reverse_krebs.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1930 2023-02-16 21:19:27.000000 magicsoup-0.3.6/src/magicsoup/examples/wood_ljungdahl.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    12180 2023-04-14 19:52:19.000000 magicsoup-0.3.6/src/magicsoup/genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    30687 2023-04-14 20:12:02.000000 magicsoup-0.3.6/src/magicsoup/kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     4143 2023-04-12 14:59:48.000000 magicsoup-0.3.6/src/magicsoup/mutations.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5288 2023-04-07 13:25:00.000000 magicsoup-0.3.6/src/magicsoup/util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    42712 2023-04-14 20:13:45.000000 magicsoup-0.3.6/src/magicsoup/world.py
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-14 20:16:29.916780 magicsoup-0.3.6/src/magicsoup.egg-info/
+-rw-rw-r--   0 marc      (1000) marc      (1003)     5297 2023-04-14 20:16:29.000000 magicsoup-0.3.6/src/magicsoup.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1003)      647 2023-04-14 20:16:29.000000 magicsoup-0.3.6/src/magicsoup.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)        1 2023-04-14 20:16:29.000000 magicsoup-0.3.6/src/magicsoup.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1003)       10 2023-04-14 20:16:29.000000 magicsoup-0.3.6/src/magicsoup.egg-info/top_level.txt
+drwxrwxr-x   0 marc      (1000) marc      (1003)        0 2023-04-14 20:16:29.916780 magicsoup-0.3.6/tests/
+-rw-rw-r--   0 marc      (1000) marc      (1003)      710 2023-02-09 10:42:28.000000 magicsoup-0.3.6/tests/test_containers.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     6012 2023-04-06 09:44:07.000000 magicsoup-0.3.6/tests/test_genetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    46955 2023-04-06 09:24:16.000000 magicsoup-0.3.6/tests/test_kinetics.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)     1433 2023-04-03 15:10:20.000000 magicsoup-0.3.6/tests/test_util.py
+-rw-rw-r--   0 marc      (1000) marc      (1003)    18649 2023-04-11 15:52:20.000000 magicsoup-0.3.6/tests/test_world.py
```

### Comparing `magicsoup-0.3.5/LICENSE` & `magicsoup-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.5/PKG-INFO` & `magicsoup-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.3.5
+Version: 0.3.6
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.3.5/README.md` & `magicsoup-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.5/pyproject.toml` & `magicsoup-0.3.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.5/src/magicsoup/constants.py` & `magicsoup-0.3.6/src/magicsoup/constants.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.5/src/magicsoup/containers.py` & `magicsoup-0.3.6/src/magicsoup/containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.5/src/magicsoup/examples/n2_fixing.py` & `magicsoup-0.3.6/src/magicsoup/examples/n2_fixing.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.5/src/magicsoup/examples/reverse_krebs.py` & `magicsoup-0.3.6/src/magicsoup/examples/reverse_krebs.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.5/src/magicsoup/examples/wood_ljungdahl.py` & `magicsoup-0.3.6/src/magicsoup/examples/wood_ljungdahl.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.5/src/magicsoup/genetics.py` & `magicsoup-0.3.6/src/magicsoup/genetics.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,16 @@
         )
     return n
 
 
 def _get_coding_regions(
     seq: str,
     min_cds_size: int,
-    start_codons: tuple[str, ...],
-    stop_codons: tuple[str, ...],
+    start_codons: list[str],
+    stop_codons: list[str],
 ) -> list[str]:
     s = CODON_SIZE
     n = len(seq)
     max_start_idx = n - min_cds_size
 
     start_idxs = []
     for start_codon in start_codons:
@@ -99,15 +99,14 @@
         is_useful_prot = False
 
         i = 0
         j = dom_size
         while i + dom_size <= len(cds):
             dom_type_seq = cds[i : i + dom_type_size]
             if dom_type_seq in dom_type_map:
-
                 # 1=catal, 2=trnsp, 3=reg
                 dom_type = dom_type_map[dom_type_seq]
                 if dom_type != 3:
                     is_useful_prot = True
 
                 dom_spec_seq = cds[i + dom_type_size : i + dom_size]
                 idx0 = one_codon_map[dom_spec_seq[idx0_slice]]
@@ -127,16 +126,16 @@
 
     return prot_doms
 
 
 def _translate_genome(
     genome: str,
     dom_size: int,
-    start_codons: tuple[str, ...],
-    stop_codons: tuple[str, ...],
+    start_codons: list[str],
+    stop_codons: list[str],
     dom_type_map: dict[str, int],
     one_codon_map: dict[str, int],
     two_codon_map: dict[str, int],
 ) -> list[list[tuple[int, int, int, int, int]]]:
     dom_type_size = len(next(iter(dom_type_map)))
 
     cdsf = _get_coding_regions(
@@ -225,16 +224,16 @@
                 f" {','.join(str(d) for d in set(start_codons) & set(stop_codons))}"
             )
         if p_catal_dom + p_transp_dom + p_reg_dom > 1.0:
             raise ValueError(
                 "p_catal_dom, p_transp_dom, p_reg_dom together must not be greater 1.0"
             )
 
-        self.start_codons = start_codons
-        self.stop_codons = stop_codons
+        self.start_codons = list(start_codons)
+        self.stop_codons = list(stop_codons)
         self.workers = workers
 
         # Domain structure:
         # domain type definition (domain type codons)
         # 3 x 1-codon specifications (3 simple tokens)
         # 1 x 2-codon specification (1 complex token)
         # a domain can begin and end with start/stop codons
@@ -268,14 +267,18 @@
             self.one_codon_map[seq] = i + 1
 
         # the second codon is allowed to be a stop codon
         self.two_codon_map: dict[str, int] = {}
         for i, seq in enumerate(self._get_double_codons()):
             self.two_codon_map[seq] = i + 1
 
+        # inverse maps for genome generation
+        self.idx_2_one_codon = {v: k for k, v in self.one_codon_map.items()}
+        self.idx_2_two_codon = {v: k for k, v in self.two_codon_map.items()}
+
     def translate_genomes(
         self, genomes: list[str]
     ) -> list[list[list[tuple[int, int, int, int, int]]]]:
         """
         Translate all genomes into proteomes
 
         Arguments:
```

### Comparing `magicsoup-0.3.5/src/magicsoup/kinetics.py` & `magicsoup-0.3.6/src/magicsoup/kinetics.py`

 * *Files 6% similar despite different names*

```diff
@@ -53,14 +53,21 @@
         signs = torch.tensor([zero_value] + random.choices(choices, k=max_token))
         self.signs = signs.to(device)
 
     def __call__(self, t: torch.Tensor) -> torch.Tensor:
         """t: long (c, p, d)"""
         return self.signs[t]
 
+    def inverse(self) -> dict[bool, list[int]]:
+        sign_map = {}
+        M = self.signs
+        sign_map[True] = torch.argwhere(M == 1.0).flatten().tolist()
+        sign_map[False] = torch.argwhere(M == -1.0).flatten().tolist()
+        return sign_map
+
 
 class _VectorMapFact:
     """
     Create an object that maps tokens
     to a list of vectors. Each vector will be mapped with
     the same frequency.
     """
@@ -138,14 +145,32 @@
             vectors=vectors,
             n_signals=n_signals,
             max_token=max_token,
             device=device,
             zero_value=zero_value,
         )
 
+    def inverse(
+        self,
+        molmap: dict[Molecule, int],
+        reactions: list[tuple[list[Molecule], list[Molecule]]],
+        n_signals: int,
+    ) -> dict[tuple[tuple[Molecule, ...], tuple[Molecule, ...]], list[int]]:
+        react_map = {}
+        for subs, prods in reactions:
+            t = torch.zeros(n_signals)
+            for sub in subs:
+                t[molmap[sub]] -= 1
+            for prod in prods:
+                t[molmap[prod]] += 1
+            M = self.M
+            idxs = torch.argwhere((M == t).all(dim=1)).flatten().tolist()
+            react_map[(tuple(subs), tuple(prods))] = idxs
+        return react_map
+
 
 class _TransporterMapFact(_VectorMapFact):
     """
     Create an object that maps tokens to vectors.
     Each vector has signals length and represents the
     stoichiometry of a molecule transport into or out of the cell.
     """
@@ -171,14 +196,22 @@
             vectors=vectors,
             n_signals=n_signals,
             max_token=max_token,
             device=device,
             zero_value=zero_value,
         )
 
+    def inverse(self, molecules: list[Molecule]) -> dict[Molecule, list[int]]:
+        trnsp_map = {}
+        for mi, mol in enumerate(molecules):
+            M = self.M
+            idxs = torch.argwhere(M[:, mi] != 0).flatten().tolist()
+            trnsp_map[mol] = idxs
+        return trnsp_map
+
 
 class _RegulatoryMapFact(_VectorMapFact):
     """
     Create an object that maps tokens to vectors.
     Each vector has signals length and represents the
     either activating (+1) or inhibiting (-1) effect
     of an effector molecule.
@@ -202,14 +235,22 @@
             vectors=vectors,
             n_signals=n_signals,
             max_token=max_token,
             device=device,
             zero_value=zero_value,
         )
 
+    def inverse(self, molecules: list[Molecule]) -> dict[Molecule, list[int]]:
+        reg_map = {}
+        for mi, mol in enumerate(molecules):
+            M = self.M
+            idxs = torch.argwhere(M[:, mi] != 0).flatten().tolist()
+            reg_map[mol] = idxs
+        return reg_map
+
 
 class Kinetics:
     """
     Class holding logic for simulating protein work.
     Usually this class is instantiated automatically when initializing [World][magicsoup.world.World].
     You can access it on `world.kinetics`.
 
@@ -323,14 +364,22 @@
             n_molecules=len(molecules), max_token=vector_enc_size, device=device
         )
 
         self.effector_map = _RegulatoryMapFact(
             n_molecules=len(molecules), max_token=vector_enc_size, device=device
         )
 
+        # derive inverse maps for genome generation
+        self.sign_2_idxs = self.sign_map.inverse()
+        self.trnsp_2_idxs = self.transport_map.inverse(molecules=molecules)
+        self.regul_2_idxs = self.effector_map.inverse(molecules=molecules)
+        self.catal_2_idxs = self.reaction_map.inverse(
+            molmap=self.mol_2_mi, reactions=reactions, n_signals=n_signals
+        )
+
     def get_proteome(
         self, proteome: list[list[tuple[int, int, int, int, int]]]
     ) -> list[Protein]:
         """
         Calculate cell parameters for a single proteome and return it as
         a list of proteins
```

### Comparing `magicsoup-0.3.5/src/magicsoup/mutations.py` & `magicsoup-0.3.6/src/magicsoup/mutations.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.5/src/magicsoup/util.py` & `magicsoup-0.3.6/src/magicsoup/util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.5/src/magicsoup/world.py` & `magicsoup-0.3.6/src/magicsoup/world.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,26 @@
 import pickle
 from pathlib import Path
 import torch
 from magicsoup.constants import CODON_SIZE
 from magicsoup.util import moore_nghbrhd, round_down, random_genome, randstr
 from magicsoup.containers import (
     Cell,
+    Molecule,
     Chemistry,
     ProteinFact,
     CatalyticDomainFact,
     TransporterDomainFact,
     RegulatoryDomainFact,
 )
 from magicsoup.kinetics import Kinetics
 from magicsoup.genetics import Genetics
 
+import time
+
 
 def _torch_load(map_loc: str | None = None):
     # Closure rather than a lambda to preserve map_loc
     return lambda b: torch.load(BytesIO(b), map_location=map_loc)
 
 
 class _CPU_Unpickler(pickle.Unpickler):
@@ -177,14 +180,29 @@
         self.cell_survival: torch.Tensor = torch.zeros(0).to(device).int()
         self.cell_divisions: torch.Tensor = torch.zeros(0).to(device).int()
         self.cell_molecules: torch.Tensor = torch.zeros(0, self.n_molecules).to(device)
         self.molecule_map: torch.Tensor = self._get_molecule_map(
             n=self.n_molecules, size=map_size, init=mol_map_init
         )
 
+    def _get_catal_2_idxs(
+        self,
+    ) -> dict[tuple[tuple[Molecule, ...], tuple[Molecule, ...]], list[int]]:
+        react_map = {}
+        for subs, prods in self.chemistry.reactions:
+            t = torch.zeros(self.n_molecules * 2)
+            for sub in subs:
+                t[self.kinetics.mol_2_mi[sub]] -= 1
+            for prod in prods:
+                t[self.kinetics.mol_2_mi[prod]] += 1
+            M = self.kinetics.reaction_map.M
+            idxs = torch.argwhere((M == t).all(dim=1)).flatten().tolist()
+            react_map[(tuple(subs), tuple(prods))] = idxs
+        return react_map
+
     def get_cell(
         self,
         by_idx: int | None = None,
         by_position: tuple[int, int] | None = None,
     ) -> Cell:
         """
         Get a cell with information about its current environment.
@@ -304,29 +322,31 @@
         pad_size = n_pad_nts / (n_p_pads * 0.7 + n_d_pads * 0.3)
         d_pad_size = round_down(pad_size * 0.3, to=3)
         d_pad_total = n_d_pads * d_pad_size
         p_pad_size = round_down((n_pad_nts - d_pad_total) / n_p_pads, to=1)
         p_pad_total = n_p_pads * p_pad_size
         remaining_nts = n_pad_nts - d_pad_total - p_pad_total
 
-        excl_cdss = list(self.genetics.start_codons) + list(self.genetics.stop_codons)
+        start_codons = self.genetics.start_codons
+        stop_codons = self.genetics.stop_codons
+        excl_cdss = start_codons + stop_codons
         excl_doms = excl_cdss + list(self.genetics.domain_map)
         p_pads = [random_genome(s=p_pad_size, excl=excl_cdss) for _ in range(n_p_pads)]
         d_pads = [random_genome(s=d_pad_size, excl=excl_doms) for _ in range(n_d_pads)]
         tail = random_genome(s=remaining_nts, excl=excl_cdss)
 
         parts: list[str] = []
         for cds in cdss:
             parts.append(p_pads.pop())
-            parts.append(random.choice(self.genetics.start_codons))
+            parts.append(random.choice(start_codons))
             for dom_seq in cds:
                 parts.append(d_pads.pop())
                 parts.append(dom_seq)
             parts.append(d_pads.pop())
-            parts.append(random.choice(self.genetics.stop_codons))
+            parts.append(random.choice(stop_codons))
         parts.append(p_pads.pop())
         parts.append(tail)
 
         return "".join(parts)
 
     def add_cells(self, genomes: list[str]) -> list[int]:
         """
@@ -715,14 +735,18 @@
         Returns:
             A new `world` instance.
         """
         with open(rundir / name, "rb") as fh:
             unpickler = _CPU_Unpickler(fh, map_location=device)
             obj: "World" = unpickler.load()
 
+        if device is not None:
+            obj.device = device
+            obj.kinetics.device = device
+
         if workers is not None:
             obj.workers = workers
             obj.genetics.workers = workers
 
         return obj
 
     def save_state(self, statedir: Path):
@@ -754,45 +778,43 @@
         with open(statedir / "cells.fasta", "w", encoding="utf-8") as fh:
             fh.write("\n".join(lines))
 
     def load_state(
         self,
         statedir: Path,
         ignore_cell_params: bool = False,
-        device: str | None = None,
     ):
         """
         Load a saved world state.
         The state had to be saved with [save_state()][magicsoup.world.World.save_state] previously.
 
         Parameters:
             statedir: Directory that contains all files of that state
             ignore_cell_params: Whether to not update cell parameters as well.
                 If you are only interested in the cells' genomes and molecules
                 you can set this to `True` to make loading a lot faster.
-            device: Optionally set device to which tensors should be loaded.
-                Default is the current `world.device`.
         """
-        device = device or self.device
 
         self.cell_molecules = torch.load(
-            statedir / "cell_molecules.pt", map_location=device
+            statedir / "cell_molecules.pt", map_location=self.device
         )
-        self.cell_map = torch.load(statedir / "cell_map.pt", map_location=device).bool()
+        self.cell_map = torch.load(
+            statedir / "cell_map.pt", map_location=self.device
+        ).bool()
         self.molecule_map = torch.load(
-            statedir / "molecule_map.pt", map_location=device
+            statedir / "molecule_map.pt", map_location=self.device
         )
         self.cell_survival = torch.load(
-            statedir / "cell_survival.pt", map_location=device
+            statedir / "cell_survival.pt", map_location=self.device
         ).int()
         self.cell_positions = torch.load(
-            statedir / "cell_positions.pt", map_location=device
+            statedir / "cell_positions.pt", map_location=self.device
         ).int()
         self.cell_divisions = torch.load(
-            statedir / "cell_divisions.pt", map_location=device
+            statedir / "cell_divisions.pt", map_location=self.device
         ).int()
 
         with open(statedir / "cells.fasta", "r", encoding="utf-8") as fh:
             text: str = fh.read()
             entries = [d.strip() for d in text.split(">") if len(d.strip()) > 0]
 
         genome_idx_pairs: list[tuple[str, int]] = []
@@ -854,49 +876,22 @@
         chosen = pxls[idxs]
         return chosen
 
     def _get_genome_sequences(self, proteome: list[ProteinFact]) -> list[list[str]]:
         proteome = proteome.copy()
         random.shuffle(proteome)
 
-        all_mols = self.chemistry.molecules
-        all_reacts = self.chemistry.reactions
-        stops = list(self.genetics.start_codons)
-
+        stop_codons = self.genetics.start_codons
         dom_type_map = self.genetics.domain_types
-        one_codon_map = {v: k for k, v in self.genetics.one_codon_map.items()}
-        two_codon_map = {v: k for k, v in self.genetics.two_codon_map.items()}
-
-        react_map = {}
-        for subs, prods in all_reacts:
-            t = torch.zeros(self.n_molecules * 2)
-            for sub in subs:
-                t[self.kinetics.mol_2_mi[sub]] -= 1
-            for prod in prods:
-                t[self.kinetics.mol_2_mi[prod]] += 1
-            M = self.kinetics.reaction_map.M
-            idxs = torch.argwhere((M == t).all(dim=1)).flatten().tolist()
-            react_map[(tuple(subs), tuple(prods))] = idxs
-
-        trnsp_map = {}
-        for mi, mol in enumerate(all_mols):
-            M = self.kinetics.transport_map.M
-            idxs = torch.argwhere(M[:, mi] != 0).flatten().tolist()
-            trnsp_map[mol] = idxs
-
-        reg_map = {}
-        for mi, mol in enumerate(all_mols):
-            M = self.kinetics.effector_map.M
-            idxs = torch.argwhere(M[:, mi] != 0).flatten().tolist()
-            reg_map[mol] = idxs
-
-        sign_map = {}
-        M = self.kinetics.sign_map.signs
-        sign_map[True] = torch.argwhere(M == 1.0).flatten().tolist()
-        sign_map[False] = torch.argwhere(M == -1.0).flatten().tolist()
+        one_codon_map = self.genetics.idx_2_one_codon
+        two_codon_map = self.genetics.idx_2_two_codon
+        react_map = self.kinetics.catal_2_idxs
+        trnsp_map = self.kinetics.trnsp_2_idxs
+        reg_map = self.kinetics.regul_2_idxs
+        sign_map = self.kinetics.sign_2_idxs
 
         cdss: list[list[str]] = []
         for prot in proteome:
             cds = []
             for dom in prot.domain_facts:
                 # Domain structure:
                 # 0: domain type definition (1=catalytic, 2=transporter, 3=regulatory)
@@ -910,31 +905,31 @@
                         react = (tuple(dom.products), tuple(dom.substrates))
                         is_fwd = False
                     i3 = random.choice(sign_map[is_fwd])
                     i4 = random.choice(react_map[react])
                     dom_seq = random.choice(dom_type_map[1])
                     sign_seq = one_codon_map[i3]
                     react_seq = two_codon_map[i4]
-                    mm_seq = random_genome(s=2 * CODON_SIZE, excl=stops)
+                    mm_seq = random_genome(s=2 * CODON_SIZE, excl=stop_codons)
                     cds.append(dom_seq + mm_seq + sign_seq + react_seq)
 
                 if isinstance(dom, TransporterDomainFact):
                     i4 = random.choice(trnsp_map[dom.molecule])
                     dom_seq = random.choice(dom_type_map[2])
                     mol_seq = two_codon_map[i4]
-                    mm_seq = random_genome(s=2 * CODON_SIZE, excl=stops)
-                    sign_seq = random_genome(s=CODON_SIZE, excl=stops)
+                    mm_seq = random_genome(s=2 * CODON_SIZE, excl=stop_codons)
+                    sign_seq = random_genome(s=CODON_SIZE, excl=stop_codons)
                     cds.append(dom_seq + mm_seq + sign_seq + mol_seq)
 
                 if isinstance(dom, RegulatoryDomainFact):
                     i4 = random.choice(reg_map[dom.effector])
                     dom_seq = random.choice(dom_type_map[3])
                     mol_seq = two_codon_map[i4]
-                    mm_seq = random_genome(s=2 * CODON_SIZE, excl=stops)
-                    sign_seq = random_genome(s=CODON_SIZE, excl=stops)
+                    mm_seq = random_genome(s=2 * CODON_SIZE, excl=stop_codons)
+                    sign_seq = random_genome(s=CODON_SIZE, excl=stop_codons)
                     cds.append(dom_seq + mm_seq + sign_seq + mol_seq)
 
             cdss.append(cds)
 
         return cdss
 
     def _get_molecule_map(self, n: int, size: int, init: str) -> torch.Tensor:
```

### Comparing `magicsoup-0.3.5/src/magicsoup.egg-info/PKG-INFO` & `magicsoup-0.3.6/src/magicsoup.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magicsoup
-Version: 0.3.5
+Version: 0.3.6
 Summary: Simulation for cell metabolic and transduction pathway evolution
 Author-email: Marc <schweringmarc01@gmail.com>
 Project-URL: Documentation, https://magic-soup.readthedocs.io/
 Project-URL: Homepage, https://github.com/mRcSchwering/magic-soup
 Project-URL: Bug Tracker, https://github.com/mRcSchwering/magic-soup/issues
 Classifier: Environment :: Console
 Classifier: Environment :: GPU
```

### Comparing `magicsoup-0.3.5/src/magicsoup.egg-info/SOURCES.txt` & `magicsoup-0.3.6/src/magicsoup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.5/tests/test_containers.py` & `magicsoup-0.3.6/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.5/tests/test_genetics.py` & `magicsoup-0.3.6/tests/test_genetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.5/tests/test_kinetics.py` & `magicsoup-0.3.6/tests/test_kinetics.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.5/tests/test_util.py` & `magicsoup-0.3.6/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `magicsoup-0.3.5/tests/test_world.py` & `magicsoup-0.3.6/tests/test_world.py`

 * *Files identical despite different names*

