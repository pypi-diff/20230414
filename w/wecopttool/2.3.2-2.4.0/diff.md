# Comparing `tmp/wecopttool-2.3.2.tar.gz` & `tmp/wecopttool-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wecopttool-2.3.2.tar", last modified: Wed Apr 12 17:16:57 2023, max compression
+gzip compressed data, was "wecopttool-2.4.0.tar", last modified: Fri Apr 14 16:11:47 2023, max compression
```

## Comparing `wecopttool-2.3.2.tar` & `wecopttool-2.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:16:57.304774 wecopttool-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 17:16:45.000000 wecopttool-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-12 17:16:45.000000 wecopttool-2.3.2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-12 17:16:57.304774 wecopttool-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-12 17:16:45.000000 wecopttool-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-12 17:16:45.000000 wecopttool-2.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 17:16:57.304774 wecopttool-2.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:16:57.300774 wecopttool-2.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    50582 2023-04-12 17:16:45.000000 wecopttool-2.3.2/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-12 17:16:45.000000 wecopttool-2.3.2/tests/test_hydrostatics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-04-12 17:16:45.000000 wecopttool-2.3.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-04-12 17:16:45.000000 wecopttool-2.3.2/tests/test_pto.py
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-04-12 17:16:45.000000 wecopttool-2.3.2/tests/test_waves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:16:57.300774 wecopttool-2.3.2/wecopttool/
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-12 17:16:45.000000 wecopttool-2.3.2/wecopttool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    82645 2023-04-12 17:16:45.000000 wecopttool-2.3.2/wecopttool/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-12 17:16:45.000000 wecopttool-2.3.2/wecopttool/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-12 17:16:45.000000 wecopttool-2.3.2/wecopttool/hydrostatics.py
--rw-r--r--   0 runner    (1001) docker     (123)    33435 2023-04-12 17:16:45.000000 wecopttool-2.3.2/wecopttool/pto.py
--rw-r--r--   0 runner    (1001) docker     (123)    17475 2023-04-12 17:16:45.000000 wecopttool-2.3.2/wecopttool/waves.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 17:16:57.304774 wecopttool-2.3.2/wecopttool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-12 17:16:57.000000 wecopttool-2.3.2/wecopttool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-12 17:16:57.000000 wecopttool-2.3.2/wecopttool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 17:16:57.000000 wecopttool-2.3.2/wecopttool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-12 17:16:57.000000 wecopttool-2.3.2/wecopttool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 17:16:57.000000 wecopttool-2.3.2/wecopttool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:47.452280 wecopttool-2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-14 16:11:36.000000 wecopttool-2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-14 16:11:36.000000 wecopttool-2.4.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-14 16:11:47.452280 wecopttool-2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2738 2023-04-14 16:11:36.000000 wecopttool-2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-14 16:11:36.000000 wecopttool-2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 16:11:47.452280 wecopttool-2.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:47.448280 wecopttool-2.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    50582 2023-04-14 16:11:36.000000 wecopttool-2.4.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-04-14 16:11:36.000000 wecopttool-2.4.0/tests/test_hydrostatics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12231 2023-04-14 16:11:36.000000 wecopttool-2.4.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-04-14 16:11:36.000000 wecopttool-2.4.0/tests/test_pto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-04-14 16:11:36.000000 wecopttool-2.4.0/tests/test_waves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:47.452280 wecopttool-2.4.0/wecopttool/
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-14 16:11:36.000000 wecopttool-2.4.0/wecopttool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    82645 2023-04-14 16:11:36.000000 wecopttool-2.4.0/wecopttool/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-04-14 16:11:36.000000 wecopttool-2.4.0/wecopttool/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-04-14 16:11:36.000000 wecopttool-2.4.0/wecopttool/hydrostatics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34521 2023-04-14 16:11:36.000000 wecopttool-2.4.0/wecopttool/pto.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17475 2023-04-14 16:11:36.000000 wecopttool-2.4.0/wecopttool/waves.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:47.452280 wecopttool-2.4.0/wecopttool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-04-14 16:11:47.000000 wecopttool-2.4.0/wecopttool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-14 16:11:47.000000 wecopttool-2.4.0/wecopttool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:11:47.000000 wecopttool-2.4.0/wecopttool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-14 16:11:47.000000 wecopttool-2.4.0/wecopttool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 16:11:47.000000 wecopttool-2.4.0/wecopttool.egg-info/top_level.txt
```

### Comparing `wecopttool-2.3.2/LICENSE` & `wecopttool-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.2/NOTICE` & `wecopttool-2.4.0/NOTICE`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.2/PKG-INFO` & `wecopttool-2.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wecopttool
-Version: 2.3.2
+Version: 2.4.0
 Summary: WEC Design Optimization Toolbox
 Author: Sandia National Laboratories
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Documentation, https://snl-waterpower.github.io/WecOptTool/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `wecopttool-2.3.2/README.md` & `wecopttool-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.2/pyproject.toml` & `wecopttool-2.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "wecopttool"
-version = "2.3.2"
+version = "2.4.0"
 description = "WEC Design Optimization Toolbox"
 readme = "README.md"
 authors = [
     {name = "Sandia National Laboratories"},
 ]
 urls = {Documentation = "https://snl-waterpower.github.io/WecOptTool/"}
 requires-python = ">=3.8"
```

### Comparing `wecopttool-2.3.2/tests/test_core.py` & `wecopttool-2.4.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.2/tests/test_hydrostatics.py` & `wecopttool-2.4.0/tests/test_hydrostatics.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.2/tests/test_integration.py` & `wecopttool-2.4.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.2/tests/test_pto.py` & `wecopttool-2.4.0/tests/test_pto.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.2/tests/test_waves.py` & `wecopttool-2.4.0/tests/test_waves.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.2/wecopttool/__init__.py` & `wecopttool-2.4.0/wecopttool/__init__.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.2/wecopttool/core.py` & `wecopttool-2.4.0/wecopttool/core.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.2/wecopttool/geom.py` & `wecopttool-2.4.0/wecopttool/geom.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.2/wecopttool/hydrostatics.py` & `wecopttool-2.4.0/wecopttool/hydrostatics.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.2/wecopttool/pto.py` & `wecopttool-2.4.0/wecopttool/pto.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,21 +122,36 @@
 
         def force(wec, x_wec, x_opt, waves, nsubsteps=1):
             return controller(self, wec, x_wec, x_opt, waves, nsubsteps)
 
         self._force = force
 
         # power
-        self._impedance = impedance
-        self._loss = loss
         if impedance is not None:
+            check_1 = impedance.shape[0] == impedance.shape[1] == 2*self.ndof
+            check_2 = len(impedance.shape) == 3
+            if not (check_1 and check_2):
+                raise TypeError(
+                    "Impedance should have size [2*ndof, 2*ndof, nfreq]"
+                )
+            for i in range(impedance.shape[2]-1):
+                check_3 = (
+                    np.allclose(np.real(impedance[:, :, i+1]), np.real(impedance[:, :, 0]))
+                )
+                if not check_3:
+                    raise ValueError(
+                        "Real component of impedance must be constant for " +
+                        "all frequencies."
+                    )
             impedance_abcd = _make_abcd(impedance, ndof)
             self._transfer_mat = _make_mimo_transfer_mat(impedance_abcd, ndof)
         else:
             self._transfer_mat = None
+        self._impedance = impedance
+        self._loss = loss
 
     @property
     def ndof(self) -> int:
         """Number of degrees of freedom."""
         return self._ndof
 
     @property
@@ -423,15 +438,15 @@
     def power_variables(self,
         wec: TWEC,
         x_wec: ndarray,
         x_opt: ndarray,
         waves: Optional[Dataset] = None,
         nsubsteps: Optional[int] = 1,
     ) -> tuple[ndarray, ndarray]:
-        """Calculate the power variables (flow q and effort e) time-series 
+        """Calculate the power variables (flow q and effort e) time-series
         in each PTO DOF for a given system state.
 
         Parameters
         ----------
         wec
             :py:class:`wecopttool.WEC` object.
         x_wec
@@ -442,15 +457,15 @@
             :py:class:`xarray.Dataset` with the structure and elements
             shown by :py:mod:`wecopttool.waves`.
         nsubsteps
             Number of steps between the default (implied) time steps.
             A value of :python:`1` corresponds to the default step
             length.
         """
-        # convert q1 (PTO velocity), e1 (PTO force) 
+        # convert q1 (PTO velocity), e1 (PTO force)
         # to q2 (flow variable), e2 (effort variable)
         if self.impedance is not None:
             q1_td = self.velocity(wec, x_wec, x_opt, waves)
             e1_td = self.force(wec, x_wec, x_opt, waves)
             q1 = complex_to_real(td_to_fd(q1_td, False))
             e1 = complex_to_real(td_to_fd(e1_td, False))
             vars_1 = np.hstack([q1, e1])
@@ -489,18 +504,25 @@
             :py:class:`xarray.Dataset` with the structure and elements
             shown by :py:mod:`wecopttool.waves`.
         nsubsteps
             Number of steps between the default (implied) time steps.
             A value of :python:`1` corresponds to the default step
             length.
         """
-        q2_td, e2_td = self.power_variables(wec, x_wec, 
+        q2_td, e2_td = self.power_variables(wec, x_wec,
                                             x_opt, waves, nsubsteps)
         # power
         power_out = q2_td * e2_td
+        if self.impedance is not None:
+            z_12 = self.impedance[:self.ndof, self.ndof:, 0] # Fi
+            z_22 = self.impedance[self.ndof:, self.ndof:, 0] # Vi
+            z_12_inv = np.linalg.inv(z_12.T).T
+            x_opt_0 = vec_to_dofmat(x_opt, self.ndof)[0:1, :]
+            transduced_flow = np.dot(np.real(z_12_inv), x_opt_0.T)
+            power_out = power_out + (np.dot(np.real(z_22), transduced_flow**2)).T
         if self.loss is not None:
             power_out = power_out + self.loss(q2_td, e2_td)
         return power_out
 
     def energy(self,
         wec: TWEC,
         x_wec: ndarray,
@@ -562,28 +584,28 @@
     def transduced_flow(self,
         wec: TWEC,
         x_wec: ndarray,
         x_opt: ndarray,
         waves: Optional[Dataset] = None,
         nsubsteps: Optional[int] = 1,
     ) -> float:
-        """Calculate the transduced flow variable time-series in each PTO DOF 
-        for a given system state. Equals the PTO velocity if no impedance 
+        """Calculate the transduced flow variable time-series in each PTO DOF
+        for a given system state. Equals the PTO velocity if no impedance
         is defined.
 
         Examples for PTO impedance and corresponding flow variables:
 
         - OWC: (pneumatic admittance)^-1 : flow = volumetric air flow
 
         - Drive-train: rotational impedance : flow = rotational velocity
 
         - Generator: winding impedance: flow = electric current
 
         - Drive-train and Generator combined: flow = electric current
-        
+
         Parameters
         ----------
         wec
             :py:class:`wecopttool.WEC` object.
         x_wec
             WEC dynamic state.
         x_opt
@@ -592,27 +614,27 @@
             :py:class:`xarray.Dataset` with the structure and elements
             shown by :py:mod:`wecopttool.waves`.
         nsubsteps
             Number of steps between the default (implied) time steps.
             A value of :python:`1` corresponds to the default step
             length.
         """
-        q2_td, _ = self.power_variables(wec, x_wec, 
+        q2_td, _ = self.power_variables(wec, x_wec,
                                         x_opt, waves, nsubsteps)
-        return q2_td   
+        return q2_td
 
     def transduced_effort(self,
         wec: TWEC,
         x_wec: ndarray,
         x_opt: ndarray,
         waves: Optional[Dataset] = None,
         nsubsteps: Optional[int] = 1,
     ) -> float:
-        """Calculate the transduced flow variable time-series in each PTO DOF 
-        for a given system state. Equals the PTO force if no impedance 
+        """Calculate the transduced flow variable time-series in each PTO DOF
+        for a given system state. Equals the PTO force if no impedance
         is defined.
 
         Examples for PTO impedance and corresponding effort variables:
 
         - OWC: (pneumatic admittance)^-1 : effort =  air pressure
 
         - Drive-train: rotational impedance : effort = torque
@@ -634,15 +656,15 @@
             shown by :py:mod:`wecopttool.waves`.
         nsubsteps
             Number of steps between the default (implied) time steps.
             A value of :python:`1` corresponds to the default step
             length.
         """
         _, e2_td = self.power_variables(wec, x_wec, x_opt, waves, nsubsteps)
-        return e2_td  
+        return e2_td
 
     def post_process(self,
         wec: TWEC,
         res: OptimizeResult,
         waves: Optional[DataArray] = None,
         nsubsteps: Optional[int] = 1,
     ) -> tuple[Dataset, Dataset]:
@@ -715,15 +737,15 @@
         # power
         power_td = self.power(wec, x_wec, x_opt, waves, nsubsteps)
         power_fd = wec.td_to_fd(power_td[::nsubsteps])
 
         # mechanical power
         mech_power_td = self.mechanical_power(wec, x_wec, x_opt, waves,
                                               nsubsteps)
-        mech_power_fd = wec.td_to_fd(mech_power_td[::nsubsteps])    
+        mech_power_fd = wec.td_to_fd(mech_power_td[::nsubsteps])
 
         pos_attr = {'long_name': 'Position', 'units': 'm or rad'}
         vel_attr = {'long_name': 'Velocity', 'units': 'm/s or rad/s'}
         acc_attr = {'long_name': 'Acceleration',
                     'units': 'm/s^2 or rad/s^2'}
         force_attr = {'long_name': 'Force or moment on WEC',
                       'units': 'N or Nm'}
@@ -740,15 +762,15 @@
         results_fd = Dataset(
             data_vars={
                 'pos': (['omega','dof'], pos_fd, pos_attr),
                 'vel': (['omega','dof'], vel_fd, vel_attr),
                 'acc': (['omega','dof'], acc_fd, acc_attr),
                 'force': (['omega','dof'], force_fd, force_attr),
                 'power': (['omega','dof'], power_fd, power_attr),
-                'mech_power': (['omega','dof'], 
+                'mech_power': (['omega','dof'],
                                 mech_power_fd, mech_power_attr)
             },
             coords={
                 'omega':('omega', wec.omega, omega_attr),
                 'freq':('omega', wec.frequency, freq_attr),
                 'period':('omega', wec.period, period_attr),
                 'dof':('dof', self.names, dof_attr)},
@@ -766,25 +788,25 @@
                                  mech_power_td, mech_power_attr)
             },
             coords={
                 'time':('time', t_dat, time_attr),
                 'dof':('dof', self.names, dof_attr)},
             attrs={"time_created_utc": create_time}
             )
-        
+
         if self.impedance is not None:
         #transduced flow and effort variables
             q2_td, e2_td = self.power_variables(wec, x_wec, x_opt,
                                                 waves, nsubsteps)
             q2_fd = wec.td_to_fd(q2_td[::nsubsteps])
             e2_fd = wec.td_to_fd(e2_td[::nsubsteps])
 
-            q2_attr = {'long_name': 'Transduced Flow', 
+            q2_attr = {'long_name': 'Transduced Flow',
                        'units': 'A or m^3/s or rad/s or m/s'}
-            e2_attr = {'long_name': 'Transduced Effort', 
+            e2_attr = {'long_name': 'Transduced Effort',
                        'units': 'V or N/m^2 or Nm or Ns'}
 
             results_td = results_td.assign({
                         'trans_flo': (['time','dof'], q2_td, q2_attr),
                         'trans_eff': (['time','dof'], e2_td, e2_attr),
                     })
             results_fd = results_fd.assign({
```

### Comparing `wecopttool-2.3.2/wecopttool/waves.py` & `wecopttool-2.4.0/wecopttool/waves.py`

 * *Files identical despite different names*

### Comparing `wecopttool-2.3.2/wecopttool.egg-info/PKG-INFO` & `wecopttool-2.4.0/wecopttool.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wecopttool
-Version: 2.3.2
+Version: 2.4.0
 Summary: WEC Design Optimization Toolbox
 Author: Sandia National Laboratories
 License: GNU General Public License v3 (GPLv3)
 Project-URL: Documentation, https://snl-waterpower.github.io/WecOptTool/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

