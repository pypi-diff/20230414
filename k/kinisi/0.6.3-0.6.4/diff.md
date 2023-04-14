# Comparing `tmp/kinisi-0.6.3.tar.gz` & `tmp/kinisi-0.6.4.tar.gz`

## Comparing `kinisi-0.6.3.tar` & `kinisi-0.6.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/__init__.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/analyze.py
--rw-r--r--   0        0        0    17218 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/analyzer.py
--rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/arrhenius.py
--rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/conductivity_analyzer.py
--rw-r--r--   0        0        0    34673 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/diffusion.py
--rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/diffusion_analyzer.py
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/jump_diffusion_analyzer.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/matrix.py
--rw-r--r--   0        0        0    23518 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/__init__.py
--rw-r--r--   0        0        0    14904 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/test_analyze.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/test_arrhenius.py
--rw-r--r--   0        0        0    38583 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/test_diffusion.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/test_matrix.py
--rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/test_parser.py
--rw-r--r--   0        0        0    46919 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/inputs/example_LAMMPS.data
--rw-r--r--   0        0        0   630756 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/inputs/example_LAMMPS.dcd
--rw-r--r--   0        0        0   842426 2020-02-02 00:00:00.000000 kinisi-0.6.3/kinisi/tests/inputs/example_XDATCAR.gz
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 kinisi-0.6.3/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 kinisi-0.6.3/LICENSE
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 kinisi-0.6.3/README.md
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 kinisi-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 kinisi-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/__init__.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/analyze.py
+-rw-r--r--   0        0        0    17218 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/analyzer.py
+-rw-r--r--   0        0        0     7609 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/arrhenius.py
+-rw-r--r--   0        0        0    12707 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/conductivity_analyzer.py
+-rw-r--r--   0        0        0    34775 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/diffusion.py
+-rw-r--r--   0        0        0    11039 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/diffusion_analyzer.py
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/jump_diffusion_analyzer.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/matrix.py
+-rw-r--r--   0        0        0    23518 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/__init__.py
+-rw-r--r--   0        0        0    14904 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/test_analyze.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/test_arrhenius.py
+-rw-r--r--   0        0        0    38583 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/test_diffusion.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/test_matrix.py
+-rw-r--r--   0        0        0     4815 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/test_parser.py
+-rw-r--r--   0        0        0    46919 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/inputs/example_LAMMPS.data
+-rw-r--r--   0        0        0   630756 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/inputs/example_LAMMPS.dcd
+-rw-r--r--   0        0        0   842426 2020-02-02 00:00:00.000000 kinisi-0.6.4/kinisi/tests/inputs/example_XDATCAR.gz
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 kinisi-0.6.4/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 kinisi-0.6.4/LICENSE
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 kinisi-0.6.4/README.md
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 kinisi-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 kinisi-0.6.4/PKG-INFO
```

### Comparing `kinisi-0.6.3/kinisi/analyze.py` & `kinisi-0.6.4/kinisi/analyze.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 This module contains the API classes for :py:mod:`kinisi`.
 It is anticipated that this is where the majority of interaction with the package will occur.
 This module includes:
 
 * the :py:class:`kinisi.analyze.DiffusionAnalyzer` class for MSD and diffusion analysis;
-* the :py:class:`kinisi.analyze.JumpDiffusionAnalyzer` class for TMSD and collective diffusion analysis; and
+* the :py:class:`kinisi.analyze.JumpDiffusionAnalyzer` class for MSTD and collective diffusion analysis; and
 * the :py:class:`kinisi.analyze.ConductivityAnalyzer` class for MSCD and conductivity analysis.
 
 These are all compatible with VASP Xdatcar output files, pymatgen structures and any MD trajectory that the
 :py:mod:`MDAnalysis` package can handle.
 """
 
 # Copyright (c) Andrew R. McCluskey and Benjamin J. Morgan
```

### Comparing `kinisi-0.6.3/kinisi/analyzer.py` & `kinisi-0.6.4/kinisi/analyzer.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.3/kinisi/arrhenius.py` & `kinisi-0.6.4/kinisi/arrhenius.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.3/kinisi/conductivity_analyzer.py` & `kinisi-0.6.4/kinisi/conductivity_analyzer.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.3/kinisi/diffusion.py` & `kinisi-0.6.4/kinisi/diffusion.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,30 +173,30 @@
         :return: Timestep values that were resampled.
         """
         return self._dt
 
     @property
     def n(self) -> np.ndarray:
         """
-        :return: The mean MSD/TMSD/MSCD, as determined from the bootstrap resampling process, in units Å:sup:`2`.
+        :return: The mean MSD/MSTD/MSCD, as determined from the bootstrap resampling process, in units Å:sup:`2`.
         """
         return self._n
 
     @property
     def s(self) -> np.ndarray:
         """
-        :return: The MSD/TMSD/MSCD standard deviation, as determined from the bootstrap resampling process, in
+        :return: The MSD/MSTD/MSCD standard deviation, as determined from the bootstrap resampling process, in
             units Å:sup:`2`.
         """
         return self._s
 
     @property
     def v(self) -> np.ndarray:
         """
-        :return: The MSD/TMSD/MSCD variance as determined from the bootstrap resampling process, in units Å:sup:`4`.
+        :return: The MSD/MSTD/MSCD variance as determined from the bootstrap resampling process, in units Å:sup:`4`.
         """
         return self._v
 
     @property
     def euclidian_displacements(self) -> List[Distribution]:
         """
         :return: Displacements between particles at each dt.
@@ -521,15 +521,15 @@
             self._v = np.append(self._v, np.var(d_squared, ddof=1) / n_o[i])
             self._s = np.append(self._s, np.sqrt(self._v[i]))
             self._ngp = np.append(self._ngp, self.ngp_calculation(d_squared))
             self._dt = np.append(self._dt, self._delta_t[i])
         self._n_o = self._n_o[:self._n.size]
 
 
-class TMSDBootstrap(Bootstrap):
+class MSTDBootstrap(Bootstrap):
     """
     Perform a bootstrap resampling to obtain accurate estimates for the mean and uncertainty for the total
     mean squared displacements.
 
     :param delta_t: An array of the timestep values.
     :param disp_3d: A list of arrays, where each array has the axes
         :code:`[atom, displacement observation, dimension]`. There is one array in the list for each
@@ -573,21 +573,21 @@
                                                                            self._displacements[i].shape[1], self.dims)
             d_squared = np.sum(disp_slice**2, axis=-1)
             coll_motion = np.sum(np.sum(disp_slice, axis=0)**2, axis=-1)
             if coll_motion.size <= 1:
                 continue
             self._euclidian_displacements.append(Distribution(np.sqrt(d_squared.flatten())))
             if bootstrap:
-                distro = self.sample_until_normal(d_squared, n_o[i], n_resamples, max_resamples, alpha, random_state)
+                distro = self.sample_until_normal(coll_motion, n_o[i] / d_squared.shape[0], n_resamples, max_resamples, alpha, random_state)
                 self._distributions.append(distro)
                 self._n_bootstrap = np.append(self._n_bootstrap, np.mean(distro.samples))
                 self._v_bootstrap = np.append(self._v_bootstrap, np.var(distro.samples, ddof=1))
                 self._s_bootstrap = np.append(self._s_bootstrap, np.std(distro.samples, ddof=1))
-            self._n = np.append(self._n, d_squared.mean())
-            self._v = np.append(self._v, np.var(d_squared, ddof=1) / n_o[i])
+            self._n = np.append(self._n, coll_motion.mean())
+            self._v = np.append(self._v, np.var(coll_motion, ddof=1) / n_o[i] / d_squared.shape[0])
             self._s = np.append(self._s, np.sqrt(self._v[i]))
             self._ngp = np.append(self._ngp, self.ngp_calculation(d_squared.flatten()))
             self._dt = np.append(self._dt, self._delta_t[i])
         self._n_o = self._n_o[:self._n.size]
 
 
 class MSCDBootstrap(Bootstrap):
@@ -644,21 +644,21 @@
                                                                            self._displacements[i].shape[1], self.dims)
             d_squared = np.sum(disp_slice**2, axis=-1)
             sq_chg_motion = np.sum(np.sum((ionic_charge * self._displacements[i].T).T, axis=0)**2, axis=-1)
             if sq_chg_motion.size <= 1:
                 continue
             self._euclidian_displacements.append(Distribution(np.sqrt(d_squared.flatten())))
             if bootstrap:
-                distro = self.sample_until_normal(d_squared, n_o[i], n_resamples, max_resamples, alpha, random_state)
+                distro = self.sample_until_normal(sq_chg_motion, n_o[i] / d_squared.shape[0], n_resamples, max_resamples, alpha, random_state)
                 self._distributions.append(distro)
                 self._n_bootstrap = np.append(self._n_bootstrap, np.mean(distro.samples))
                 self._v_bootstrap = np.append(self._v_bootstrap, np.var(distro.samples, ddof=1))
                 self._s_bootstrap = np.append(self._s_bootstrap, np.std(distro.samples, ddof=1))
-            self._n = np.append(self._n, d_squared.mean())
-            self._v = np.append(self._v, np.var(d_squared, ddof=1) / n_o[i])
+            self._n = np.append(self._n, sq_chg_motion.mean())
+            self._v = np.append(self._v, np.var(sq_chg_motion, ddof=1) / n_o[i] / d_squared.shape[0])
             self._s = np.append(self._s, np.sqrt(self._v[i]))
             self._ngp = np.append(self._ngp, self.ngp_calculation(d_squared.flatten()))
             self._dt = np.append(self._dt, self._delta_t[i])
         self._n_o = self._n_o[:self._n.size]
 
 
 def _bootstrap(array: np.ndarray,
```

### Comparing `kinisi-0.6.3/kinisi/diffusion_analyzer.py` & `kinisi-0.6.4/kinisi/diffusion_analyzer.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.3/kinisi/jump_diffusion_analyzer.py` & `kinisi-0.6.4/kinisi/jump_diffusion_analyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 class JumpDiffusionAnalyzer(Analyzer):
     """
     The :py:class:`kinisi.analyze.JumpDiffusionAnalyzer` class performs analysis of collective diffusion
     relationships in materials.
     This is achieved through the application of a bootstrapping methodology to obtain the most statistically
     accurate values for total mean squared displacement uncertainty and covariance.
-    The time-dependence of the TMSD is then modelled in a generalised least squares fashion to obtain the jump
+    The time-dependence of the MSTD is then modelled in a generalised least squares fashion to obtain the jump
     diffusion coefficient and offset using Markov chain Monte Carlo maximum likelihood sampling.
 
     :param delta_t: An array of the timestep values.
     :param disp_3d: A list of arrays, where each array has the axes [atom, displacement observation, dimension].
         There is one array in the list for each delta_t value. Note: it is necessary to use a list of arrays as
         the number of observations is not necessary the same at each data point.
     :param volume: The volume of the simulation cell.
@@ -79,15 +79,15 @@
             appropriate documentation for more guidance on this. Optional, default is the default bootstrap parameters.
 
         :return: Relevant :py:class:`JumpDiffusionAnalyzer` object.
         """
         if bootstrap_params is None:
             bootstrap_params = {}
         jdiff_anal = super()._from_pymatgen(trajectory, parser_params, dtype=dtype)
-        jdiff_anal._diff = diffusion.TMSDBootstrap(jdiff_anal._delta_t, jdiff_anal._disp_3d, jdiff_anal._n_o,
+        jdiff_anal._diff = diffusion.MSTDBootstrap(jdiff_anal._delta_t, jdiff_anal._disp_3d, jdiff_anal._n_o,
                                                    **bootstrap_params)
         return jdiff_anal
 
     @classmethod
     def from_Xdatcar(cls,
                      trajectory: Union['pymatgen.io.vasp.outputs.Xdatcar', List['pymatgen.io.vasp.outputs.Xdatcar']],
                      parser_params: dict,
@@ -109,15 +109,15 @@
             appropriate documentation for more guidance on this. Optional, default is the default bootstrap parameters.
 
         :return: Relevant :py:class:`JumpDiffusionAnalyzer` object.
         """
         if bootstrap_params is None:
             bootstrap_params = {}
         jdiff_anal = super()._from_Xdatcar(trajectory, parser_params, dtype=dtype)
-        jdiff_anal._diff = diffusion.TMSDBootstrap(jdiff_anal._delta_t, jdiff_anal._disp_3d, jdiff_anal._n_o,
+        jdiff_anal._diff = diffusion.MSTDBootstrap(jdiff_anal._delta_t, jdiff_anal._disp_3d, jdiff_anal._n_o,
                                                    **bootstrap_params)
         return jdiff_anal
 
     @classmethod
     def from_file(cls,
                   trajectory: Union[str, List[str]],
                   parser_params: dict,
@@ -137,15 +137,15 @@
             appropriate documentation for more guidance on this. Optional, default is the default bootstrap parameters.
 
         :return: Relevant :py:class:`JumpDiffusionAnalyzer` object.
         """
         if bootstrap_params is None:
             bootstrap_params = {}
         jdiff_anal = super()._from_file(trajectory, parser_params, dtype=dtype)
-        jdiff_anal._diff = diffusion.TMSDBootstrap(jdiff_anal._delta_t, jdiff_anal._disp_3d, jdiff_anal._n_o,
+        jdiff_anal._diff = diffusion.MSTDBootstrap(jdiff_anal._delta_t, jdiff_anal._disp_3d, jdiff_anal._n_o,
                                                    **bootstrap_params)
         return jdiff_anal
 
     @classmethod
     def from_universe(cls,
                       trajectory: 'MDAnalysis.core.universe.Universe',
                       parser_params: dict,
@@ -166,40 +166,40 @@
             appropriate documentation for more guidance on this. Optional, default is the default bootstrap parameters.
 
         :return: Relevant :py:class:`JumpDiffusionAnalyzer` object.
         """
         if bootstrap_params is None:
             bootstrap_params = {}
         jdiff_anal = super()._from_universe(trajectory, parser_params, dtype=dtype)
-        jdiff_anal._diff = diffusion.TMSDBootstrap(jdiff_anal._delta_t, jdiff_anal._disp_3d, jdiff_anal._n_o,
+        jdiff_anal._diff = diffusion.MSTDBootstrap(jdiff_anal._delta_t, jdiff_anal._disp_3d, jdiff_anal._n_o,
                                                    **bootstrap_params)
         return jdiff_anal
 
     def jump_diffusion(self, jump_diffusion_params: Union[dict, None] = None):
         """
         Calculate the jump diffusion coefficicent using the bootstrap-GLS methodology.
 
-        :param ump_diffusion_params: The parameters for the :py:class:`kinisi.diffusion.TMSDBootstrap`
+        :param ump_diffusion_params: The parameters for the :py:class:`kinisi.diffusion.MSTDBootstrap`
             object. See the appropriate documentation for more guidance on this. Optional, default is the
             default bootstrap parameters.
         """
         if jump_diffusion_params is None:
             jump_diffusion_params = {}
         self._diff.jump_diffusion(**jump_diffusion_params)
 
     @property
-    def tmsd(self) -> np.ndarray:
+    def mstd(self) -> np.ndarray:
         """
-        :return: TMSD for the input trajectories. Note that this is the bootstrap sampled MSD, not the numerical
+        :return: MSTD for the input trajectories. Note that this is the bootstrap sampled MSD, not the numerical
             average from the data.
         """
         return self._diff.n
 
     @property
-    def tmsd_std(self) -> np.ndarray:
+    def mstd_std(self) -> np.ndarray:
         """
         :return: MSD standard deviation values for the input trajectories (a single standard deviation).
         """
         return self._diff.s
 
     @property
     def D_J(self) -> 'uravu.distribution.Distribution':
```

### Comparing `kinisi-0.6.3/kinisi/matrix.py` & `kinisi-0.6.4/kinisi/matrix.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.3/kinisi/parser.py` & `kinisi-0.6.4/kinisi/parser.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.3/kinisi/tests/test_analyze.py` & `kinisi-0.6.4/kinisi/tests/test_analyze.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,53 +204,53 @@
 
     def test_properties(self):
         with warnings.catch_warnings(record=True) as w:
             a = JumpDiffusionAnalyzer.from_pymatgen(xd.structures,
                                                     parser_params=da_params,
                                                     bootstrap_params={'random_state': np.random.RandomState(0)})
             assert_almost_equal(a.dt, a._diff.dt)
-            assert_almost_equal(a.tmsd, a._diff.n)
-            assert_almost_equal(a.tmsd_std, a._diff.s)
+            assert_almost_equal(a.mstd, a._diff.n)
+            assert_almost_equal(a.mstd_std, a._diff.s)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, a._diff.euclidian_displacements[i].samples)
             assert a.ngp_max == a._diff.dt[a._diff.ngp.argmax()]
 
     def test_diffusion(self):
         with warnings.catch_warnings(record=True) as w:
             a = JumpDiffusionAnalyzer.from_pymatgen(xd.structures,
                                                     parser_params=da_params,
                                                     bootstrap_params={'random_state': np.random.RandomState(0)})
             assert_almost_equal(a.dt, a._diff.dt)
-            assert_almost_equal(a.tmsd, a._diff.n)
-            assert_almost_equal(a.tmsd_std, a._diff.s)
+            assert_almost_equal(a.mstd, a._diff.n)
+            assert_almost_equal(a.mstd_std, a._diff.s)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, a._diff.euclidian_displacements[i].samples)
             a.jump_diffusion()
             assert a.ngp_max == a._diff.dt[a._diff.ngp.argmax()]
             assert isinstance(a.D_J, Distribution)
             assert a.flatchain.shape == (3200, 2)
 
     def test_dictionary_roundtrip(self):
         with warnings.catch_warnings(record=True) as w:
             a = JumpDiffusionAnalyzer.from_pymatgen(xd.structures,
                                                     parser_params=da_params,
                                                     bootstrap_params={'random_state': np.random.RandomState(0)})
             assert_almost_equal(a.dt, a._diff.dt)
-            assert_almost_equal(a.tmsd, a._diff.n)
-            assert_almost_equal(a.tmsd_std, a._diff.s)
+            assert_almost_equal(a.mstd, a._diff.n)
+            assert_almost_equal(a.mstd_std, a._diff.s)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, a._diff.euclidian_displacements[i].samples)
             a.jump_diffusion()
             assert a.ngp_max == a._diff.dt[a._diff.ngp.argmax()]
             assert isinstance(a.D_J, Distribution)
             assert a.flatchain.shape == (3200, 2)
             b = JumpDiffusionAnalyzer.from_dict(a.to_dict())
             assert_equal(a.dt, b.dt)
-            assert_equal(a.tmsd, b.tmsd)
-            assert_equal(a.tmsd_std, b.tmsd_std)
+            assert_equal(a.mstd, b.mstd)
+            assert_equal(a.mstd_std, b.mstd_std)
             for i in range(len(a.dr)):
                 assert_almost_equal(a.dr[i].samples, b.dr[i].samples)
             assert a.ngp_max == b.ngp_max
             assert_equal(a.D_J.samples, b.D_J.samples)
             assert_equal(a.flatchain, b.flatchain)
```

### Comparing `kinisi-0.6.3/kinisi/tests/test_arrhenius.py` & `kinisi-0.6.4/kinisi/tests/test_arrhenius.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.3/kinisi/tests/test_diffusion.py` & `kinisi-0.6.4/kinisi/tests/test_diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # pylint: disable=R0201
 
 import unittest
 import warnings
 import numpy as np
 from tqdm import tqdm
 from numpy.testing import assert_almost_equal, assert_equal
-from kinisi.diffusion import Bootstrap, MSDBootstrap, TMSDBootstrap, MSCDBootstrap, _bootstrap
+from kinisi.diffusion import Bootstrap, MSDBootstrap, MSTDBootstrap, MSCDBootstrap, _bootstrap
 from uravu.distribution import Distribution
 
 RNG = np.random.RandomState(43)
 
 
 class TestBootstrap(unittest.TestCase):
     """
@@ -103,15 +103,15 @@
             assert_almost_equal(distro1.samples, distro2.samples)
 
     def test_ngp_calculation(self):
         result = Bootstrap.ngp_calculation(np.array([1, 2, 3]))
         assert_almost_equal(result, -0.3)
 
 
-class TestMSDBootstrap(unittest.TestCase):
+class TesMSTDBootstrap(unittest.TestCase):
     """
     Tests for the diffusion.MSDBootstrap class.
     """
 
     def test_dictionary_roundtrip(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
@@ -369,25 +369,25 @@
     #     assert bs1.intercept.size == 500
     #     bs2 = DiffBootstrap(dt, disp_3d, n_walkers=5, n_samples=100, random_state=np.random.RandomState(0))
     #     assert_almost_equal(bs1.v, bs2.v)
     #     assert_almost_equal(bs1.covariance_matrix, bs2.covariance_matrix)
     #     assert_almost_equal(bs1.diffusion_coefficient.samples, bs2.diffusion_coefficient.samples)
 
 
-class TestTMSDBootstrap(unittest.TestCase):
+class TestMSTDBootstrap(unittest.TestCase):
     """
-    Tests for the diffusion.TMSDBootstrap class.
+    Tests for the diffusion.MSTDBootstrap class.
     """
 
     def test_initialisation(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
-            bs = TMSDBootstrap(dt, disp_3d, n_o, random_state=np.random.RandomState(0))
+            bs = MSTDBootstrap(dt, disp_3d, n_o, random_state=np.random.RandomState(0))
             assert bs.n.shape == (5, )
             assert bs.s.shape == (5, )
             assert_almost_equal(bs.v, np.square(bs.s))
             assert bs.ngp.shape == (5, )
             assert len(bs.euclidian_displacements) == 5
             for i in bs.euclidian_displacements:
                 assert isinstance(i, Distribution)
@@ -395,15 +395,15 @@
                 assert i.samples.size >= 1000
 
     def test_initialisation_n_resamples(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
-            bs = TMSDBootstrap(dt, disp_3d, n_o, n_resamples=10, random_state=np.random.RandomState(0))
+            bs = MSTDBootstrap(dt, disp_3d, n_o, n_resamples=10, random_state=np.random.RandomState(0))
             assert bs.n.shape == (5, )
             assert bs.s.shape == (5, )
             assert_almost_equal(bs.v, np.square(bs.s))
             assert bs.ngp.shape == (5, )
             assert len(bs.euclidian_displacements) == 5
             for i in bs.euclidian_displacements:
                 assert isinstance(i, Distribution)
@@ -411,15 +411,15 @@
                 assert i.samples.size >= 10
 
     def test_initialisation_max_resamples(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
-            bs = TMSDBootstrap(dt,
+            bs = MSTDBootstrap(dt,
                                disp_3d,
                                n_o,
                                n_resamples=10,
                                max_resamples=100,
                                random_state=np.random.RandomState(0))
             assert bs.n.shape == (5, )
             assert bs.s.shape == (5, )
@@ -432,34 +432,34 @@
                 assert i.samples.size <= 110
 
     def test_initialisation_random_state(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
-            bs1 = TMSDBootstrap(dt, disp_3d, n_o, bootstrap=True, random_state=np.random.RandomState(0))
+            bs1 = MSTDBootstrap(dt, disp_3d, n_o, bootstrap=True, random_state=np.random.RandomState(0))
             assert bs1.n.shape == (5, )
             assert bs1.s.shape == (5, )
             assert_almost_equal(bs1.v, np.square(bs1.s))
             assert bs1.ngp.shape == (5, )
             assert len(bs1.euclidian_displacements) == 5
             for i in bs1.euclidian_displacements:
                 assert isinstance(i, Distribution)
             for i in bs1._distributions:
                 assert i.samples.size >= 1000
-            bs2 = TMSDBootstrap(dt, disp_3d, n_o, bootstrap=True, random_state=np.random.RandomState(0))
+            bs2 = MSTDBootstrap(dt, disp_3d, n_o, bootstrap=True, random_state=np.random.RandomState(0))
             assert bs1._distributions[-1].size == bs2._distributions[-1].size
             assert_almost_equal(bs1._distributions[-1].samples, bs2._distributions[-1].samples)
 
     def test_initialisation_progress(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
-            bs = TMSDBootstrap(dt, disp_3d, n_o, progress=False, random_state=np.random.RandomState(0))
+            bs = MSTDBootstrap(dt, disp_3d, n_o, progress=False, random_state=np.random.RandomState(0))
             assert bs.n.shape == (5, )
             assert bs.s.shape == (5, )
             assert_almost_equal(bs.v, np.square(bs.s))
             assert bs.ngp.shape == (5, )
             assert len(bs.euclidian_displacements) == 5
             for i in bs.euclidian_displacements:
                 assert isinstance(i, Distribution)
@@ -468,15 +468,15 @@
             assert isinstance(bs._iterator, range)
 
     def test_initialisation_skip_where_low_samples(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(1, i, 3) for i in range(10, 1, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
-            bs = TMSDBootstrap(dt, disp_3d, n_o, progress=False, random_state=np.random.RandomState(0))
+            bs = MSTDBootstrap(dt, disp_3d, n_o, progress=False, random_state=np.random.RandomState(0))
             assert bs.n.shape == (4, )
             assert bs.s.shape == (4, )
             assert_almost_equal(bs.v, np.square(bs.s))
             assert bs.ngp.shape == (4, )
             assert len(bs.euclidian_displacements) == 4
             for i in bs.euclidian_displacements:
                 assert isinstance(i, Distribution)
@@ -485,98 +485,98 @@
             assert isinstance(bs._iterator, range)
 
     def test_bootstrap(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
-            bs = TMSDBootstrap(dt, disp_3d, n_o, random_state=RNG)
+            bs = MSTDBootstrap(dt, disp_3d, n_o, random_state=RNG)
             bs.jump_diffusion()
             assert bs.covariance_matrix.shape == (5, 5)
             assert isinstance(bs._jump_diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs._jump_diffusion_coefficient.size == 3200
             assert bs.intercept.size == 3200
 
     def test_bootstrap_use_ngp(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
-            bs = TMSDBootstrap(dt, disp_3d, n_o, random_state=RNG)
+            bs = MSTDBootstrap(dt, disp_3d, n_o, random_state=RNG)
             bs.jump_diffusion(use_ngp=True)
             assert bs.covariance_matrix.shape == (5 - np.argmax(bs.ngp), 5 - np.argmax(bs.ngp))
             assert isinstance(bs._jump_diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs._jump_diffusion_coefficient.size == 3200
             assert bs.intercept.size == 3200
 
     def test_bootstrap_fit_intercept(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
-            bs = TMSDBootstrap(dt, disp_3d, n_o, random_state=RNG)
+            bs = MSTDBootstrap(dt, disp_3d, n_o, random_state=RNG)
             bs.jump_diffusion(n_samples=500, fit_intercept=False)
             assert bs.covariance_matrix.shape == (5, 5)
             assert isinstance(bs._jump_diffusion_coefficient, Distribution)
             assert bs._jump_diffusion_coefficient.size == 1600
             assert bs.intercept is None
 
     def test_bootstrap_n_samples(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
-            bs = TMSDBootstrap(dt, disp_3d, n_o, random_state=RNG)
+            bs = MSTDBootstrap(dt, disp_3d, n_o, random_state=RNG)
             bs.jump_diffusion(n_samples=100)
             assert bs.covariance_matrix.shape == (5, 5)
             assert isinstance(bs._jump_diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs._jump_diffusion_coefficient.size == 320
             assert bs.intercept.size == 320
 
     def test_bootstrap_D(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(20, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 10)
-            bs = TMSDBootstrap(dt, disp_3d, n_o, random_state=RNG)
+            bs = MSTDBootstrap(dt, disp_3d, n_o, random_state=RNG)
             bs.jump_diffusion(n_samples=100)
             assert bs.covariance_matrix.shape == (5, 5)
             assert isinstance(bs._jump_diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs._jump_diffusion_coefficient.size == 320
             assert bs.intercept.size == 320
 
     def test_bootstrap_thin(self):
         with warnings.catch_warnings(record=True) as _:
             disp_3d = [RNG.randn(100, i, 3) for i in range(200, 10, -1)]
             n_o = np.ones(len(disp_3d)) * 100
             dt = np.linspace(100, 1000, 190)
-            bs = TMSDBootstrap(dt, disp_3d, n_o, random_state=RNG)
+            bs = MSTDBootstrap(dt, disp_3d, n_o, random_state=RNG)
             bs.jump_diffusion(use_ngp=True, thin=1)
             assert bs.covariance_matrix.shape == (95 - np.argmax(bs.ngp), 95 - np.argmax(bs.ngp))
             assert isinstance(bs._jump_diffusion_coefficient, Distribution)
             assert isinstance(bs.intercept, Distribution)
             assert bs._jump_diffusion_coefficient.size == 32000
             assert bs.intercept.size == 32000
 
     # Waiting on https://github.com/dfm/emcee/pull/376
     # def test_initialisation_random_state(self):
     #     disp_3d = [RNG.randn(100, i, 3) + 1000 for i in range(20, 10, -1)]
     #     dt = np.linspace(100, 1000, 10)
-    #     bs1 = TMSDBootstrap(dt, disp_3d, random_state=np.random.RandomState(0))
+    #     bs1 = MSTDBootstrap(dt, disp_3d, random_state=np.random.RandomState(0))
     #     bs1.jump_diffusion( n_walkers=5, n_samples=100, random_state=np.random.RandomState(0))
     #     assert bs1.covariance_matrix.shape == (10, 10)
     #     assert isinstance(bs1.diffusion_coefficient, Distribution)
     #     assert isinstance(bs1.intercept, Distribution)
     #     assert bs1.diffusion_coefficient.size == 500
     #     assert bs1.intercept.size == 500
-    #     bs2 = TMSDBootstrap(dt, disp_3d, random_state=np.random.RandomState(0))
+    #     bs2 = MSTDBootstrap(dt, disp_3d, random_state=np.random.RandomState(0))
     #     bs2.jump_diffusion( n_walkers=5, n_samples=100, random_state=np.random.RandomState(0))
     #     assert_almost_equal(bs1.v, bs2.v)
     #     assert_almost_equal(bs1.covariance_matrix, bs2.covariance_matrix)
     #     assert_almost_equal(bs1.diffusion_coefficient.samples, bs2.diffusion_coefficient.samples)
 
 
 class TestMSCDBootstrap(unittest.TestCase):
```

### Comparing `kinisi-0.6.3/kinisi/tests/test_matrix.py` & `kinisi-0.6.4/kinisi/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.3/kinisi/tests/test_parser.py` & `kinisi-0.6.4/kinisi/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.3/kinisi/tests/inputs/example_LAMMPS.data` & `kinisi-0.6.4/kinisi/tests/inputs/example_LAMMPS.data`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.3/kinisi/tests/inputs/example_LAMMPS.dcd` & `kinisi-0.6.4/kinisi/tests/inputs/example_LAMMPS.dcd`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.3/kinisi/tests/inputs/example_XDATCAR.gz` & `kinisi-0.6.4/kinisi/tests/inputs/example_XDATCAR.gz`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.3/LICENSE` & `kinisi-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.3/README.md` & `kinisi-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.3/pyproject.toml` & `kinisi-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kinisi-0.6.3/PKG-INFO` & `kinisi-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kinisi
-Version: 0.6.3
+Version: 0.6.4
 Summary: Efficient estimation of diffusion processes from molecular dynamics.
 Project-URL: homepage, https://github.com/bjmorgan/kinisi
 Project-URL: documentation, https://kinisi.rtfd.io
 Author-email: "Andrew R. McCluskey" <andrew.mccluskey@ess.eu>, "Benjamin J. Morgan" <b.j.morgan@bath.ac.uk>
 Maintainer-email: "Andrew R. McCluskey" <andrew.mccluskey@ess.eu>, "Benjamin J. Morgan" <b.j.morgan@bath.ac.uk>
 License-Expression: MIT
 License-File: LICENSE
```

