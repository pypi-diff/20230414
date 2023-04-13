# Comparing `tmp/matchmaps-0.1.3.tar.gz` & `tmp/matchmaps-0.1.4.tar.gz`

## Comparing `matchmaps-0.1.3.tar` & `matchmaps-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 matchmaps-0.1.3/.github_changelog_generator
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 matchmaps-0.1.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 matchmaps-0.1.3/setup.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 matchmaps-0.1.3/tox.ini
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 matchmaps-0.1.3/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 matchmaps-0.1.3/.github/TEST_FAIL_TEMPLATE.md
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 matchmaps-0.1.3/.github/dependabot.yml
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 matchmaps-0.1.3/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 matchmaps-0.1.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 matchmaps-0.1.3/.github/workflows/cron.yml
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 matchmaps-0.1.3/docs/Makefile
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 matchmaps-0.1.3/docs/cli.rst
--rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 matchmaps-0.1.3/docs/conf.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 matchmaps-0.1.3/docs/index.md
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 matchmaps-0.1.3/docs/make.bat
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 matchmaps-0.1.3/docs/_static/custom.css
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 matchmaps-0.1.3/src/matchmaps/__init__.py
--rwxr-xr-x   0        0        0    13302 2020-02-02 00:00:00.000000 matchmaps-0.1.3/src/matchmaps/_compute_nonisomorphous_diff.py
--rw-r--r--   0        0        0     9765 2020-02-02 00:00:00.000000 matchmaps-0.1.3/src/matchmaps/_utils.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 matchmaps-0.1.3/tests/test_matchmaps.py
--rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 matchmaps-0.1.3/.gitignore
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 matchmaps-0.1.3/LICENSE
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 matchmaps-0.1.3/README.md
--rw-r--r--   0        0        0     5332 2020-02-02 00:00:00.000000 matchmaps-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 matchmaps-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.github_changelog_generator
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 matchmaps-0.1.4/setup.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 matchmaps-0.1.4/tox.ini
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.github/TEST_FAIL_TEMPLATE.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.github/dependabot.yml
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.github/workflows/cron.yml
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 matchmaps-0.1.4/docs/Makefile
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 matchmaps-0.1.4/docs/cli.rst
+-rw-r--r--   0        0        0     6252 2020-02-02 00:00:00.000000 matchmaps-0.1.4/docs/conf.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 matchmaps-0.1.4/docs/index.md
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 matchmaps-0.1.4/docs/make.bat
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 matchmaps-0.1.4/docs/_static/custom.css
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 matchmaps-0.1.4/src/matchmaps/__init__.py
+-rwxr-xr-x   0        0        0    11679 2020-02-02 00:00:00.000000 matchmaps-0.1.4/src/matchmaps/_compute_realspace_diff.py
+-rw-r--r--   0        0        0    17638 2020-02-02 00:00:00.000000 matchmaps-0.1.4/src/matchmaps/_utils.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 matchmaps-0.1.4/tests/test_matchmaps.py
+-rw-r--r--   0        0        0     1269 2020-02-02 00:00:00.000000 matchmaps-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 matchmaps-0.1.4/LICENSE
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 matchmaps-0.1.4/README.md
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 matchmaps-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 matchmaps-0.1.4/PKG-INFO
```

### Comparing `matchmaps-0.1.3/.pre-commit-config.yaml` & `matchmaps-0.1.4/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -22,20 +22,20 @@
 #  - repo: https://github.com/charliermarsh/ruff-pre-commit
 #    rev: v0.0.256
 #    hooks:
 #      - id: ruff
 #        args: [--fix]
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.12.1
+    rev: v0.12.2
     hooks:
       - id: validate-pyproject
 
 #   - repo: https://github.com/pre-commit/mirrors-mypy
 #     rev: v0.991
 #     hooks:
 #       - id: mypy
```

### Comparing `matchmaps-0.1.3/setup.py` & `matchmaps-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.3/tox.ini` & `matchmaps-0.1.4/tox.ini`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.3/.github/workflows/build_docs.yml` & `matchmaps-0.1.4/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.3/.github/workflows/ci.yml` & `matchmaps-0.1.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.3/.github/workflows/cron.yml` & `matchmaps-0.1.4/.github/workflows/cron.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 name: --pre Test
 # An "early warning" cron job that will install dependencies
 # with `pip install --pre` periodically to test for breakage
 # (and open an issue if a test fails)
 
 on:
-  schedule:
-    - cron: "0 16 * * 1" # monday at noon est
+#  schedule:
+#    - cron: "0 16 * * 1" # monday at noon est
   workflow_dispatch:
 
 jobs:
 
   test:
     name: ${{ matrix.platform }} (${{ matrix.python-version }})
     runs-on: ${{ matrix.platform }}
```

### Comparing `matchmaps-0.1.3/docs/Makefile` & `matchmaps-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.3/docs/conf.py` & `matchmaps-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.3/docs/index.md` & `matchmaps-0.1.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.3/docs/make.bat` & `matchmaps-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.3/src/matchmaps/_compute_nonisomorphous_diff.py` & `matchmaps-0.1.4/src/matchmaps/_compute_realspace_diff.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,46 @@
-"""Compute unbiased nonisomorphous difference map."""
+"""Compute unbiased real space difference map."""
 
 import argparse
 import os
 import subprocess
 import time
 from functools import partial
 
 import gemmi
 import numpy as np
 import reciprocalspaceship as rs
 
 from matchmaps._utils import (
     _handle_special_positions,
-    align_grids_from_model_transform,
+    # align_grids_from_model_transform,
     make_floatgrid_from_mtz,
     rigid_body_refinement_wrapper,
+    _realspace_align_and_subtract,
+    _rbr_selection_parser,
+    _renumber_waters,
 )
 
 
-def compute_nonisomorphous_difference_map(
+def compute_realspace_difference_map(
     pdboff,
     mtzoff,
     mtzon,
     Foff,
     SigFoff,
     Fon,
     SigFon,
     ligands=None,
     dmin=None,
     spacing=0.5,
     on_as_stationary=False,
     input_dir="./",
     output_dir="./",
     verbose=False,
-    selection=None,
+    rbr_selections=None,
     eff=None,
 ):
     """
     _summary_.
 
     Parameters
     ----------
@@ -67,18 +70,17 @@
         _description_, by default False
     input_dir : str, optional
         Path to directory containing input files, by default "./" (current directory)
     output_dir : str, optional
         Path to directory to which output files should be written, by default "./" (current directory)
     verbose : bool, optional
         If True, print outputs of scaleit and phenix.refine, by default False
-    selection : str, optional
-        Custom selection to provide to refinement.refine.sites.rigid_body=
-        If omitted, then refinement.refine.sites.rigid_body=all
-        Custom selection is only necessary if special-position atoms need to be excluded from refinement
+    rbr_selections : list of strings, optional
+        Custom selections to provide to refinement.refine.sites.rigid_body=
+        If omitted, then refinement.refine.sites.rigid_body=all, and the entire structure is refined as a single rigid body.
     eff : str, optional
         Name of a file containing a template .eff parameter file for phenix.refine.
         If omitted, the sensible built-in .eff template is used. If you need to change something,
         I recommend copying the template from the source code and editing that.
     """
     off_name = str(mtzoff.removesuffix(".mtz"))
     on_name = str(mtzon.removesuffix(".mtz"))
@@ -86,59 +88,63 @@
     # make sure directories have a trailing slash!
     if input_dir[-1] != "/":
         input_dir = input_dir + "/"
 
     if output_dir[-1] != "/":
         output_dir = output_dir + "/"
 
+    # take in the list of rbr selections and parse them into phenix and gemmi selection formats
+    # if rbr_groups = None, just returns (None, None)
+    rbr_phenix, rbr_gemmi = _rbr_selection_parser(rbr_selections)
+
     mtzon_scaled = mtzon.removesuffix(".mtz") + "_scaled" + ".mtz"
 
     print(
         f"{time.strftime('%H:%M:%S')}: Running scaleit to scale 'on' data to 'off' data..."
     )
 
     subprocess.run(
         f"rs.scaleit -r {input_dir}/{mtzoff} {Foff} {SigFoff} -i {input_dir}/{mtzon} {Fon} {SigFon} -o {output_dir}/{mtzon_scaled}",
         shell=True,
         capture_output=(not verbose),
     )
 
     pdboff = _handle_special_positions(pdboff, input_dir, output_dir)
 
+    pdboff = _renumber_waters(pdboff, output_dir)
+
     mtzon = mtzon_scaled
 
     print(f"{time.strftime('%H:%M:%S')}: Running phenix.refine for the 'on' data...")
 
     nickname_on = rigid_body_refinement_wrapper(
         mtzon=mtzon,
         pdboff=pdboff,
         input_dir=input_dir,
         output_dir=output_dir,
         ligands=ligands,
         eff=eff,
         verbose=verbose,
-        selection=selection,
+        rbr_selections=rbr_phenix,
     )
 
     print(f"{time.strftime('%H:%M:%S')}: Running phenix.refine for the 'off' data...")
 
     nickname_off = rigid_body_refinement_wrapper(
         mtzon=mtzoff,
         pdboff=pdboff,
         input_dir=input_dir,
         output_dir=output_dir,
         ligands=ligands,
         eff=eff,
         verbose=verbose,
-        selection=selection,
+        rbr_selections=rbr_phenix,
         off_labels=f"{Foff},{SigFoff}",
     )
 
-    # done with reciprocal space; transitioning to real space
-
     # read back in the files created by phenix
     # these have knowable names
     mtzon = rs.read_mtz(f"{output_dir}/{nickname_on}_1.mtz")
     mtzoff = rs.read_mtz(f"{output_dir}/{nickname_off}_1.mtz")
 
     pdbon = gemmi.read_structure(f"{output_dir}/{nickname_on}_1.pdb")
     pdboff = gemmi.read_structure(f"{output_dir}/{nickname_off}_1.pdb")
@@ -156,107 +162,59 @@
     fg_off = make_floatgrid_from_mtz(
         mtzoff, spacing, F="F-obs-filtered", Phi="PH2FOFCWT", spacegroup="P1", dmin=dmin
     )
     fg_on = make_floatgrid_from_mtz(
         mtzon, spacing, F="F-obs-filtered", Phi="PH2FOFCWT", spacegroup="P1", dmin=dmin
     )
 
-    # TO-DO: think more about scaling!
-
-    print(f"{time.strftime('%H:%M:%S')}: Using models to rigid-body align maps...")
-    if on_as_stationary:
-        # rs.io.write_ccp4_map(fg_off.array, f'{output_dir}/off_before_transforming.map',
-        #                      fg_off.unit_cell, fg_off.spacegroup)
-        fg_off = align_grids_from_model_transform(fg_on, fg_off, pdbon, pdboff)
-        fg_on = align_grids_from_model_transform(fg_on, fg_on, pdbon, pdbon)
-        pdb = pdbon
-        fg_ref = fg_on
-    else:
-        # rs.io.write_ccp4_map(fg_on.array, f'{output_dir}/on_before_transforming.map',
-        #                      fg_on.unit_cell, fg_on.spacegroup)
-        fg_on = align_grids_from_model_transform(fg_off, fg_on, pdboff, pdbon)
-        fg_off = align_grids_from_model_transform(
-            fg_off, fg_off, pdboff, pdboff
-        )  # apply same masking sitch to both grids?
-        pdb = pdboff
-        fg_ref = fg_off
-
-    print(f"{fg_off.array.mean()=}, {fg_on.array.mean()=}")
-
-    # do this again, because transformation + carving can mess up scales:
-    fg_on.normalize()
-    fg_off.normalize()
-
-    print(f"{fg_off.array.mean()=}, {fg_on.array.mean()=}")
-
-    print(f"{time.strftime('%H:%M:%S')}: Writing files...")
-
-    difference_array = fg_on.array - fg_off.array
-
-    # all that's left is to mask out voxels that aren't near the model!
-    # we can do this in gemmi
-    fg_mask_only = fg_ref.clone()
-    masker = gemmi.SolventMasker(gemmi.AtomicRadiiSet.Cctbx)
-    masker.rprobe = 2  # this should do it, idk, no need to make this a user parameter
-
-    masker.put_mask_on_float_grid(fg_mask_only, pdb[0])
-    masked_difference_array = np.logical_not(fg_mask_only.array) * difference_array
-
-    # and finally, write stuff out
-    # use partial function to guarantee I'm always using the same and correct cell
-
-    # coot refuses to render periodic boundaries for P1 maps with alpha=beta=gamma=90, sooooo
-    if all(
-        [
-            angle == 90
-            for angle in (
-                fg_ref.unit_cell.alpha,
-                fg_ref.unit_cell.beta,
-                fg_ref.unit_cell.gamma,
-            )
-        ]
-    ):
-        fg_ref.unit_cell = gemmi.UnitCell(
-            fg_ref.unit_cell.a,
-            fg_ref.unit_cell.b,
-            fg_ref.unit_cell.c,
-            90.006,
-            fg_ref.unit_cell.beta,
-            fg_ref.unit_cell.gamma,
+    if rbr_gemmi is None:
+        _realspace_align_and_subtract(
+            fg_off=fg_off,
+            fg_on=fg_on,
+            pdboff=pdboff,
+            pdbon=pdbon,
+            output_dir=output_dir,
+            on_name=on_name,
+            off_name=off_name,
+            on_as_stationary=on_as_stationary,
+            selection=rbr_gemmi,
         )
-        print("did silly angle thing")
-
-    write_maps = partial(
-        rs.io.write_ccp4_map, cell=fg_ref.unit_cell, spacegroup=fg_ref.spacegroup
-    )
-
-    write_maps(fg_on.array, f"{output_dir}/{on_name}.map")
-
-    write_maps(fg_off.array, f"{output_dir}/{off_name}.map")
 
-    write_maps(masked_difference_array, f"{output_dir}/{on_name}_minus_{off_name}.map")
-    write_maps(
-        difference_array, f"{output_dir}/{on_name}_minus_{off_name}_unmasked.map"
-    )
+    else:  # run helper function separately for each selection
+        for n, selection in enumerate(rbr_gemmi, start=1):
+            on_name_rbr = on_name + "_rbrgroup" + str(n)
+            off_name_rbr = off_name + "_rbrgroup" + str(n)
+
+            _realspace_align_and_subtract(
+                fg_off=fg_off.clone(),
+                fg_on=fg_on.clone(),
+                pdboff=pdboff,
+                pdbon=pdbon,
+                output_dir=output_dir,
+                on_name=on_name_rbr,
+                off_name=off_name_rbr,
+                on_as_stationary=on_as_stationary,
+                selection=selection,
+            )
 
     print(f"{time.strftime('%H:%M:%S')}: Done!")
 
     return
 
 
 def parse_arguments():
     """Parse commandline arguments."""
     parser = argparse.ArgumentParser(
         description=(
-            "Compute a difference map using non-isomorphous inputs. "
+            "Compute a real-space difference map. "
             "You will need two MTZ files, which will be referred to throughout as 'on' and 'off', "
             "though they could also be light/dark, bound/apo, mutant/WT, hot/cold, etc. "
             "Each mtz will need to contain structure factor amplitudes and uncertainties; you will not need any phases. "
             "You will, however, need an input model (assumed to correspond with the 'off' state) which will be used to determine phases. "
-            "Please note that both ccp4 and phenix must be installed and active in your environment for this function to work. "
+            "Please note that both ccp4 and phenix must be installed and active in your environment for this function to run. "
         )
     )
 
     parser.add_argument(
         "--mtzoff",
         "-f",
         nargs=3,
@@ -340,34 +298,35 @@
     parser.add_argument(
         "--dmin",
         required=False,
         type=float,
         default=None,
         help=(
             "Highest-resolution (in Angstroms) reflections to include in Fourier transform for FloatGrid creation. "
-            "By default, cutoff is the resolution of the lower-resolution input MTZ. "
+            "By default, cutoff is the resolution limit of the lower-resolution input MTZ. "
         ),
     )
 
     parser.add_argument(
         "--verbose",
         "-v",
         required=False,
         action="store_true",
         default=False,
         help="Include this flag to print out scaleit and phenix.refine outputs to the terminal. Useful for troubleshooting, but annoying; defaults to False.",
     )
 
     parser.add_argument(
-        "--selection",
+        "--rbr-selections",
+        "-r",
         required=False,
         default=None,
+        nargs="*",
         help=(
-            "Argument to phenix.refine's refinement.refine.sites.rigid_body. "
-            "Use this flag if atoms on special positions need to be omitted from the atom selection. "
+            "Specification of multiple rigid-body groups for refinement. By default, everything is refined as one rigid-body group. "
         ),
     )
 
     parser.add_argument(
         "--eff",
         required=False,
         default=None,
@@ -380,27 +339,27 @@
 def main():
     parser = parse_arguments()
     args = parser.parse_args()
 
     if not os.path.exists(args.output_dir):
         os.makedirs(args.output_dir)
 
-    compute_nonisomorphous_difference_map(
+    compute_realspace_difference_map(
         pdboff=args.pdboff,
         ligands=args.ligands,
         mtzoff=args.mtzoff[0],
         mtzon=args.mtzon[0],
         Foff=args.mtzoff[1],
         SigFoff=args.mtzoff[2],
         Fon=args.mtzon[1],
         SigFon=args.mtzon[2],
         input_dir=args.input_dir,
         output_dir=args.output_dir,
         verbose=args.verbose,
-        selection=args.selection,
+        rbr_selections=args.rbr_selections,
         eff=args.eff,
         dmin=args.dmin,
         spacing=args.spacing,
         on_as_stationary=args.on_as_stationary,
     )
 
     return
```

### Comparing `matchmaps-0.1.3/.gitignore` & `matchmaps-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.3/LICENSE` & `matchmaps-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.3/README.md` & `matchmaps-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `matchmaps-0.1.3/pyproject.toml` & `matchmaps-0.1.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 [project.urls]
 homepage = "https://dennisbrookner.github.io/matchmaps/"
 repository = "https://github.com/dennisbrookner/matchmaps"
 
 # same as console_scripts entry point
 [project.scripts]
-matchmaps = "matchmaps._compute_nonisomorphous_diff:main"
+matchmaps = "matchmaps._compute_realspace_diff:main"
 
 # Entry points
 # https://peps.python.org/pep-0621/#entry-points
 # [project.entry-points."spam.magical"]
 # tomatoes = "spam:main_tomatoes"
 
 # https://hatch.pypa.io/latest/config/metadata/
@@ -78,101 +78,101 @@
 # include = ["/src", "/tests"]
 
 # [tool.hatch.build.targets.wheel]
 # only-include = ["src"]
 # sources = ["src"]
 
 # https://github.com/charliermarsh/ruff
-[tool.ruff]
-line-length = 88
-target-version = "py38"
-# https://beta.ruff.rs/docs/rules/
-extend-select = [
-    "E",    # style errors
-    "W",    # style warnings
-    "F",    # flakes
-    "D",    # pydocstyle
-    "I",    # isort
-    "U",    # pyupgrade
-    # "S",    # bandit
-    "C",    # flake8-comprehensions
-    "B",    # flake8-bugbear
-    "A001", # flake8-builtins
-    "RUF",  # ruff-specific rules
-]
+# [tool.ruff]
+# line-length = 88
+# target-version = "py38"
+# # https://beta.ruff.rs/docs/rules/
+# extend-select = [
+#     "E",    # style errors
+#     "W",    # style warnings
+#     "F",    # flakes
+#     "D",    # pydocstyle
+#     "I",    # isort
+#     "U",    # pyupgrade
+#     # "S",    # bandit
+#     "C",    # flake8-comprehensions
+#     "B",    # flake8-bugbear
+#     "A001", # flake8-builtins
+#     "RUF",  # ruff-specific rules
+# ]
 # I do this to get numpy-style docstrings AND retain
 # D417 (Missing argument descriptions in the docstring)
 # otherwise, see:
 # https://beta.ruff.rs/docs/faq/#does-ruff-support-numpy-or-google-style-docstrings
 # https://github.com/charliermarsh/ruff/issues/2606
-extend-ignore = [
-    "D100", # Missing docstring in public module
-    "D107", # Missing docstring in __init__
-    "D203", # 1 blank line required before class docstring
-    "D212", # Multi-line docstring summary should start at the first line
-    "D213", # Multi-line docstring summary should start at the second line
-    "D401", # First line should be in imperative mood
-    "D413", # Missing blank line after last section
-    "D416", # Section name should end with a colon
-]
-
-[tool.ruff.per-file-ignores]
-"tests/*.py" = ["D", "S"]
-"setup.py" = ["D"]
-"docs/conf.py" = [
-    "A001",
-    "C901",
-    "D200",
-    "D400",
-    "D415",
-]
+# extend-ignore = [
+#     "D100", # Missing docstring in public module
+#     "D107", # Missing docstring in __init__
+#     "D203", # 1 blank line required before class docstring
+#     "D212", # Multi-line docstring summary should start at the first line
+#     "D213", # Multi-line docstring summary should start at the second line
+#     "D401", # First line should be in imperative mood
+#     "D413", # Missing blank line after last section
+#     "D416", # Section name should end with a colon
+# ]
+
+# [tool.ruff.per-file-ignores]
+# "tests/*.py" = ["D", "S"]
+# "setup.py" = ["D"]
+# "docs/conf.py" = [
+#     "A001",
+#     "C901",
+#     "D200",
+#     "D400",
+#     "D415",
+# ]
 
 # https://docs.pytest.org/en/6.2.x/customize.html
-[tool.pytest.ini_options]
-minversion = "6.0"
-testpaths = ["tests"]
-filterwarnings = ["error"]
+# [tool.pytest.ini_options]
+# minversion = "6.0"
+# testpaths = ["tests"]
+# filterwarnings = ["error"]
 
 # https://mypy.readthedocs.io/en/stable/config_file.html
-[tool.mypy]
-files = "src/**/"
-strict = true
-disallow_any_generics = false
-disallow_subclassing_any = false
-show_error_codes = true
-pretty = true
+# [tool.mypy]
+# files = "src/**/"
+# strict = true
+# disallow_any_generics = false
+# disallow_subclassing_any = false
+# show_error_codes = true
+# pretty = true
 
 # # module specific overrides
 # [[tool.mypy.overrides]]
 # module = ["numpy.*",]
 # ignore_errors = true
 
 
 # https://coverage.readthedocs.io/en/6.4/config.html
-[tool.coverage.report]
-exclude_lines = [
-    "pragma: no cover",
-    "if TYPE_CHECKING:",
-    "@overload",
-    "except ImportError",
-    "\\.\\.\\.",
-    "raise NotImplementedError()",
-]
-[tool.coverage.run]
-source = ["src"]
+# [tool.coverage.report]
+# exclude_lines = [
+#     "pragma: no cover",
+#     "if TYPE_CHECKING:",
+#     "@overload",
+#     "except ImportError",
+#     "\\.\\.\\.",
+#     "raise NotImplementedError()",
+# ]
+# [tool.coverage.run]
+# source = ["src"]
 
 # https://github.com/mgedmin/check-manifest#configuration
-[tool.check-manifest]
-ignore = [
-    ".github_changelog_generator",
-    ".pre-commit-config.yaml",
-    ".ruff_cache/**/*",
-    "setup.py",
-    "tests/**/*",
-]
+# [tool.check-manifest]
+# ignore = [
+#     ".github_changelog_generator",
+#     ".pre-commit-config.yaml",
+#     ".ruff_cache/**/*",
+#     "setup.py",
+#     "tests/**/*",
+# ]
 
 # # https://python-semantic-release.readthedocs.io/en/latest/configuration.html
 # [tool.semantic_release]
 # version_source = "tag_only"
 # branch = "main"
 # changelog_sections = "feature,fix,breaking,documentation,performance,chore,:boom:,:sparkles:,:children_crossing:,:lipstick:,:iphone:,:egg:,:chart_with_upwards_trend:,:ambulance:,:lock:,:bug:,:zap:,:goal_net:,:alien:,:wheelchair:,:speech_balloon:,:mag:,:apple:,:penguin:,:checkered_flag:,:robot:,:green_apple:,Other"
 # # commit_parser=semantic_release.history.angular_parser
```

### Comparing `matchmaps-0.1.3/PKG-INFO` & `matchmaps-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchmaps
-Version: 0.1.3
+Version: 0.1.4
 Summary: Make unbiased difference maps even for non-isomorphous inputs
 Project-URL: homepage, https://dennisbrookner.github.io/matchmaps/
 Project-URL: repository, https://github.com/dennisbrookner/matchmaps
 Author-email: Dennis Brookner <debrookner@gmail.com>
 License: BSD 3-Clause License
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
```

