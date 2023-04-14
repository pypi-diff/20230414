# Comparing `tmp/pyroll_hensel_power_and_labour-2.0.0a0.post1.tar.gz` & `tmp/pyroll_hensel_power_and_labour-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroll_hensel_power_and_labour-2.0.0a0.post1.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pyroll_hensel_power_and_labour-2.0.0a0.post1.tar` & `pyroll_hensel_power_and_labour-2.0.1.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1473 2022-06-07 15:10:43.877495 pyroll_hensel_power_and_labour-2.0.0a0.post1/LICENSE
--rw-r--r--   0        0        0      105 2022-06-07 15:10:43.877495 pyroll_hensel_power_and_labour-2.0.0a0.post1/README.md
--rw-r--r--   0        0        0      956 2022-12-21 09:52:33.531396 pyroll_hensel_power_and_labour-2.0.0a0.post1/pyproject.toml
--rw-r--r--   0        0        0     2007 2022-12-21 09:49:36.893249 pyroll_hensel_power_and_labour-2.0.0a0.post1/pyroll/hensel_power_and_labour/__init__.py
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 pyroll_hensel_power_and_labour-2.0.0a0.post1/setup.py
--rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 pyroll_hensel_power_and_labour-2.0.0a0.post1/PKG-INFO
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 pyroll_hensel_power_and_labour-2.0.1/pyroll/hensel_power_and_labour.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 pyroll_hensel_power_and_labour-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 pyroll_hensel_power_and_labour-2.0.1/LICENSE
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 pyroll_hensel_power_and_labour-2.0.1/README.md
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pyroll_hensel_power_and_labour-2.0.1/hatch.toml
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 pyroll_hensel_power_and_labour-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1502 2020-02-02 00:00:00.000000 pyroll_hensel_power_and_labour-2.0.1/PKG-INFO
```

### Comparing `pyroll_hensel_power_and_labour-2.0.0a0.post1/LICENSE` & `pyroll_hensel_power_and_labour-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyroll_hensel_power_and_labour-2.0.0a0.post1/pyroll/hensel_power_and_labour/__init__.py` & `pyroll_hensel_power_and_labour-2.0.1/pyroll/hensel_power_and_labour.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import numpy as np
 from pyroll.core import RollPass, Hook
 
+VERSION = "2.0.1"
+
 RollPass.roll_gap_ratio = Hook[float]()
 """Calculate cross-section ratio used in Hensel-Poluchin master curves."""
 
 RollPass.rolling_efficiency = Hook[float]()
 """Calculate rolling efficiency according to Hensel-Poluchin master curve."""
 
-RollPass.deformation_resistance = Hook[float]()
-"""Calculate deformation resistance according to Hensel-Poluchin master curve."""
-
 RollPass.lever_arm_coefficient = Hook[float]()
 """Calculate lever coefficient according to Hensel-Poluchin master curve."""
 
 
 @RollPass.roll_gap_ratio
 def roll_gap_ratio(self: RollPass):
     mean_cross_section = (self.in_profile.cross_section.area + 2 * self.out_profile.cross_section.area) / 3
@@ -24,14 +23,20 @@
 def rolling_efficiency(self: RollPass):
     inverse_efficiency = (0.9901 + 0.106 * self.roll_gap_ratio + 0.0283 * self.roll_gap_ratio ** 2
                           + 1.5718 * np.exp(-2.4609 * self.roll_gap_ratio)
                           + 0.3117 * np.exp(-15.625 * self.roll_gap_ratio ** 2))
     return inverse_efficiency ** -1
 
 
+@RollPass.DiskElement.deformation_resistance
+def deformation_resistance(self: RollPass.DiskElement):
+    mean_flow_stress = (self.in_profile.flow_stress + self.out_profile.flow_stress) / 2
+    return mean_flow_stress / self.roll_pass.rolling_efficiency
+
+
 @RollPass.deformation_resistance
 def deformation_resistance(self: RollPass):
     mean_flow_stress = (self.in_profile.flow_stress + 2 * self.out_profile.flow_stress) / 3
     return mean_flow_stress / self.rolling_efficiency
 
 
 @RollPass.lever_arm_coefficient
@@ -45,8 +50,8 @@
 @RollPass.roll_force
 def roll_force(self: RollPass):
     return self.deformation_resistance * self.roll.contact_area
 
 
 @RollPass.Roll.roll_torque
 def roll_torque(self: RollPass.Roll):
-    return self.roll_pass().roll_force * self.contact_length * self.roll_pass().lever_arm_coefficient
+    return self.roll_pass.roll_force * self.contact_length * self.roll_pass.lever_arm_coefficient
```

### Comparing `pyroll_hensel_power_and_labour-2.0.0a0.post1/PKG-INFO` & `pyroll_hensel_power_and_labour-2.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,33 @@
 Metadata-Version: 2.1
 Name: pyroll-hensel-power-and-labour
-Version: 2.0.0a0.post1
+Version: 2.0.1
 Summary: PyRoll plugin providing roll force and roll torque empirical approach by A. Hensel.
-Home-page: https://pyroll-project.github.io/
-License: BSD-3-Clause
-Requires-Python: >=3.9,<4.0
+Project-URL: Homepage, https://pyroll.readthedocs.io
+Project-URL: Repository, https://github.com/pyroll-project/pyroll-hensel-power-and-labour
+Project-URL: Documentation, https://github.com/pyroll-project/pyroll-hensel-power-and-labour/blob/main/docs/docs.pdf
+Author-email: Christoph Renzing <christoph.renzing@imf.tu-freiberg.de>, Max Weiner <max.weiner@imf.tu-freiberg.de>
+License-Expression: BSD-3-Clause
+License-File: LICENSE
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Framework :: Hatch
+Classifier: Framework :: IPython
+Classifier: Framework :: Jupyter
+Classifier: Framework :: Pytest
+Classifier: Framework :: Sphinx
 Classifier: Intended Audience :: Manufacturing
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
-Requires-Dist: pyroll-core (>=2.0.0a,<3.0.0)
-Project-URL: Documentation, https://github.com/pyroll-project/pyroll-hensel-power-and-labour/blob/main/docs/docs.pdf
-Project-URL: Repository, https://github.com/pyroll-project/pyroll-hensel-power-and-labour
+Requires-Python: >=3.9
+Requires-Dist: pyroll-core>=2.0.2,~=2.0
 Description-Content-Type: text/markdown
 
 # PyRoll Hensel Force
 
-PyRoll plugin providing roll force and roll torque empirical approach by A. Hensel
+PyRoll plugin providing roll force and roll torque empirical approach by A. Hensel
```

