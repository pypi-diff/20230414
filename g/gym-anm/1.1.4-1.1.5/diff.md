# Comparing `tmp/gym-anm-1.1.4.tar.gz` & `tmp/gym_anm-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym-anm-1.1.4.tar", max compression
+gzip compressed data, was "gym_anm-1.1.5.tar", max compression
```

## Comparing `gym-anm-1.1.4.tar` & `gym_anm-1.1.5.tar`

### file list

```diff
@@ -1,45 +1,44 @@
--rw-r--r--   0        0        0     1068 2022-11-27 02:32:11.794005 gym-anm-1.1.4/LICENSE.md
--rw-r--r--   0        0        0     5269 2022-11-27 02:32:11.794005 gym-anm-1.1.4/README.md
--rw-r--r--   0        0        0      259 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/__init__.py
--rw-r--r--   0        0        0      167 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/agents/__init__.py
--rw-r--r--   0        0        0    18100 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/agents/mpc.py
--rw-r--r--   0        0        0     1380 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/agents/mpc_constant.py
--rw-r--r--   0        0        0     1529 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/agents/mpc_perfect.py
--rw-r--r--   0        0        0      165 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/__init__.py
--rw-r--r--   0        0        0       24 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/__init__.py
--rw-r--r--   0        0        0     8708 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/anm6.py
--rw-r--r--   0        0        0     4536 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/anm6_easy.py
--rw-r--r--   0        0        0     2975 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/network.py
--rw-r--r--   0        0        0        0 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/__init__.py
--rw-r--r--   0        0        0       57 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/css/styles.css
--rw-r--r--   0        0        0   223788 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/envs/anm6/network.svg
--rw-r--r--   0        0        0     4644 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/envs/anm6/svgLabels.js
--rw-r--r--   0        0        0      675 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/index.html
--rw-r--r--   0        0        0      775 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/js/dateTime.js
--rw-r--r--   0        0        0    14008 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/js/devices.js
--rw-r--r--   0        0        0     4387 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/js/graph.js
--rw-r--r--   0        0        0     2851 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/js/init.js
--rw-r--r--   0        0        0     1940 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/js/reward.js
--rw-r--r--   0        0        0      715 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/js/text.js
--rw-r--r--   0        0        0        0 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/py/__init__.py
--rw-r--r--   0        0        0      296 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/py/constants.py
--rw-r--r--   0        0        0     6765 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/py/rendering.py
--rw-r--r--   0        0        0     5960 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/py/servers.py
--rw-r--r--   0        0        0      581 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm6_env/utils.py
--rw-r--r--   0        0        0    22764 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/anm_env.py
--rw-r--r--   0        0        0     4800 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/envs/utils.py
--rw-r--r--   0        0        0     1359 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/errors.py
--rw-r--r--   0        0        0       89 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/simulator/__init__.py
--rw-r--r--   0        0        0     2564 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/simulator/check_network.py
--rw-r--r--   0        0        0      144 2022-11-27 02:32:11.814005 gym-anm-1.1.4/gym_anm/simulator/components/__init__.py
--rw-r--r--   0        0        0     7201 2022-11-27 02:32:11.818005 gym-anm-1.1.4/gym_anm/simulator/components/branch.py
--rw-r--r--   0        0        0     3151 2022-11-27 02:32:11.818005 gym-anm-1.1.4/gym_anm/simulator/components/bus.py
--rw-r--r--   0        0        0     1364 2022-11-27 02:32:11.818005 gym-anm-1.1.4/gym_anm/simulator/components/constants.py
--rw-r--r--   0        0        0    18890 2022-11-27 02:32:11.818005 gym-anm-1.1.4/gym_anm/simulator/components/devices.py
--rw-r--r--   0        0        0     1510 2022-11-27 02:32:11.818005 gym-anm-1.1.4/gym_anm/simulator/components/errors.py
--rw-r--r--   0        0        0    27689 2022-11-27 02:32:11.818005 gym-anm-1.1.4/gym_anm/simulator/simulator.py
--rw-r--r--   0        0        0     7180 2022-11-27 02:32:11.818005 gym-anm-1.1.4/gym_anm/simulator/solve_load_flow.py
--rw-r--r--   0        0        0      168 2022-11-27 02:32:11.818005 gym-anm-1.1.4/gym_anm/utils.py
--rw-r--r--   0        0        0      971 2022-11-27 02:32:11.818005 gym-anm-1.1.4/pyproject.toml
--rw-r--r--   0        0        0     6547 1970-01-01 00:00:00.000000 gym-anm-1.1.4/setup.py
--rw-r--r--   0        0        0     6297 1970-01-01 00:00:00.000000 gym-anm-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-14 19:14:10.017700 gym_anm-1.1.5/LICENSE.md
+-rw-r--r--   0        0        0     5269 2023-04-14 19:14:10.017700 gym_anm-1.1.5/README.md
+-rw-r--r--   0        0        0      259 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/__init__.py
+-rw-r--r--   0        0        0      167 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/agents/__init__.py
+-rw-r--r--   0        0        0    18100 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/agents/mpc.py
+-rw-r--r--   0        0        0     1380 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/agents/mpc_constant.py
+-rw-r--r--   0        0        0     1529 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/agents/mpc_perfect.py
+-rw-r--r--   0        0        0      165 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/__init__.py
+-rw-r--r--   0        0        0     8708 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/anm6.py
+-rw-r--r--   0        0        0     4536 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/anm6_easy.py
+-rw-r--r--   0        0        0     2975 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/network.py
+-rw-r--r--   0        0        0        0 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/__init__.py
+-rw-r--r--   0        0        0       57 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/css/styles.css
+-rw-r--r--   0        0        0   223788 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/envs/anm6/network.svg
+-rw-r--r--   0        0        0     4644 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/envs/anm6/svgLabels.js
+-rw-r--r--   0        0        0      675 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/index.html
+-rw-r--r--   0        0        0      775 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/js/dateTime.js
+-rw-r--r--   0        0        0    14008 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/js/devices.js
+-rw-r--r--   0        0        0     4387 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/js/graph.js
+-rw-r--r--   0        0        0     2851 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/js/init.js
+-rw-r--r--   0        0        0     1940 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/js/reward.js
+-rw-r--r--   0        0        0      715 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/js/text.js
+-rw-r--r--   0        0        0        0 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/py/__init__.py
+-rw-r--r--   0        0        0      296 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/py/constants.py
+-rw-r--r--   0        0        0     6765 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/py/rendering.py
+-rw-r--r--   0        0        0     5960 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/py/servers.py
+-rw-r--r--   0        0        0      581 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm6_env/utils.py
+-rw-r--r--   0        0        0    22764 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/anm_env.py
+-rw-r--r--   0        0        0     4800 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/envs/utils.py
+-rw-r--r--   0        0        0     1359 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/errors.py
+-rw-r--r--   0        0        0       89 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/simulator/__init__.py
+-rw-r--r--   0        0        0     2564 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/simulator/check_network.py
+-rw-r--r--   0        0        0      144 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/simulator/components/__init__.py
+-rw-r--r--   0        0        0     7201 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/simulator/components/branch.py
+-rw-r--r--   0        0        0     3151 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/simulator/components/bus.py
+-rw-r--r--   0        0        0     1364 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/simulator/components/constants.py
+-rw-r--r--   0        0        0    18890 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/simulator/components/devices.py
+-rw-r--r--   0        0        0     1510 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/simulator/components/errors.py
+-rw-r--r--   0        0        0    27692 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/simulator/simulator.py
+-rw-r--r--   0        0        0     7180 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/simulator/solve_load_flow.py
+-rw-r--r--   0        0        0      168 2023-04-14 19:14:10.037681 gym_anm-1.1.5/gym_anm/utils.py
+-rw-r--r--   0        0        0      971 2023-04-14 19:14:10.037681 gym_anm-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0     6348 1970-01-01 00:00:00.000000 gym_anm-1.1.5/PKG-INFO
```

### Comparing `gym-anm-1.1.4/LICENSE.md` & `gym_anm-1.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/README.md` & `gym_anm-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/agents/mpc.py` & `gym_anm-1.1.5/gym_anm/agents/mpc.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/agents/mpc_constant.py` & `gym_anm-1.1.5/gym_anm/agents/mpc_constant.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/agents/mpc_perfect.py` & `gym_anm-1.1.5/gym_anm/agents/mpc_perfect.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm6_env/anm6.py` & `gym_anm-1.1.5/gym_anm/envs/anm6_env/anm6.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm6_env/anm6_easy.py` & `gym_anm-1.1.5/gym_anm/envs/anm6_env/anm6_easy.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm6_env/network.py` & `gym_anm-1.1.5/gym_anm/envs/anm6_env/network.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/envs/anm6/network.svg` & `gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/envs/anm6/network.svg`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/envs/anm6/svgLabels.js` & `gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/envs/anm6/svgLabels.js`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/index.html` & `gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/index.html`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/js/dateTime.js` & `gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/js/dateTime.js`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/js/devices.js` & `gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/js/devices.js`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/js/graph.js` & `gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/js/graph.js`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/js/init.js` & `gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/js/init.js`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/js/reward.js` & `gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/js/reward.js`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/js/text.js` & `gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/js/text.js`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/py/rendering.py` & `gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/py/rendering.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm6_env/rendering/py/servers.py` & `gym_anm-1.1.5/gym_anm/envs/anm6_env/rendering/py/servers.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm6_env/utils.py` & `gym_anm-1.1.5/gym_anm/envs/anm6_env/utils.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/anm_env.py` & `gym_anm-1.1.5/gym_anm/envs/anm_env.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/envs/utils.py` & `gym_anm-1.1.5/gym_anm/envs/utils.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/errors.py` & `gym_anm-1.1.5/gym_anm/errors.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/simulator/check_network.py` & `gym_anm-1.1.5/gym_anm/simulator/check_network.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/simulator/components/branch.py` & `gym_anm-1.1.5/gym_anm/simulator/components/branch.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/simulator/components/bus.py` & `gym_anm-1.1.5/gym_anm/simulator/components/bus.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/simulator/components/constants.py` & `gym_anm-1.1.5/gym_anm/simulator/components/constants.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/simulator/components/devices.py` & `gym_anm-1.1.5/gym_anm/simulator/components/devices.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/simulator/components/errors.py` & `gym_anm-1.1.5/gym_anm/simulator/components/errors.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/gym_anm/simulator/simulator.py` & `gym_anm-1.1.5/gym_anm/simulator/simulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         return baseMVA, buses, branches, devices
 
     def _build_admittance_matrix(self):
         """
         Build the nodal admittance matrix of the network (in p.u.).
         """
         n = max([i for i in self.buses.keys()])
-        Y_bus = np.zeros((n + 1, n + 1), dtype=np.complex)
+        Y_bus = np.zeros((n + 1, n + 1), dtype=np.complex128)
 
         for (f, t), br in self.branches.items():
             # Fill an off-diagonal elements of the admittance matrix Y_bus.
             Y_bus[f, t] = -br.series / np.conjugate(br.tap)
             Y_bus[t, f] = -br.series / br.tap
 
             # Increment diagonal element of the admittance matrix Y_bus.
```

### Comparing `gym-anm-1.1.4/gym_anm/simulator/solve_load_flow.py` & `gym_anm-1.1.5/gym_anm/simulator/solve_load_flow.py`

 * *Files identical despite different names*

### Comparing `gym-anm-1.1.4/pyproject.toml` & `gym_anm-1.1.5/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gym-anm"
-version = "1.1.4"
+version = "1.1.5"
 description = "A framework to build Reinforcement Learning environments for Active Network Management tasks in electricity networks."
 authors = [
     "Robin Henry <robin@robinxhenry.com>",
 ]
 license = "MIT"
 readme = "README.md"
 documentation = "https://gym-anm.readthedocs.io/en/latest/"
```

### Comparing `gym-anm-1.1.4/setup.py` & `gym_anm-1.1.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,43 +1,150 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['gym_anm',
- 'gym_anm.agents',
- 'gym_anm.envs',
- 'gym_anm.envs.anm6_env',
- 'gym_anm.envs.anm6_env.rendering',
- 'gym_anm.envs.anm6_env.rendering.py',
- 'gym_anm.simulator',
- 'gym_anm.simulator.components']
-
-package_data = \
-{'': ['*'], 'gym_anm.envs.anm6_env.rendering': ['css/*', 'envs/anm6/*', 'js/*']}
-
-install_requires = \
-['cvxpy>=1.2.2,<2.0.0',
- 'gym>=0.26.2,<0.27.0',
- 'numpy>=1.23.5,<2.0.0',
- 'pandas>=1.5.2,<2.0.0',
- 'requests>=2.28.1,<3.0.0',
- 'websocket-client==0.56.0',
- 'websocket-server==0.4']
-
-setup_kwargs = {
-    'name': 'gym-anm',
-    'version': '1.1.4',
-    'description': 'A framework to build Reinforcement Learning environments for Active Network Management tasks in electricity networks.',
-    'long_description': "# Gym-ANM\n[![Downloads](https://pepy.tech/badge/gym-anm)](https://pepy.tech/project/gym-anm)\n[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://gym-anm.readthedocs.io/en/latest/)\n[![codecov](https://codecov.io/gh/robinhenry/gym-anm/branch/master/graph/badge.svg?token=7JSMJPPIQ7)](https://codecov.io/gh/robinhenry/gym-anm)\n[![Checks](https://github.com/robinhenry/gym-anm/actions/workflows/ci_checks.yml/badge.svg)](https://github.com/robinhenry/gym-anm/actions/workflows/ci_checks.yml)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n\n`gym-anm` is a framework for designing reinforcement learning (RL) environments that model Active Network\nManagement (ANM) tasks in electricity distribution networks. It is built on top of the\n[OpenAI Gym](https://github.com/openai/gym) toolkit.\n\nThe `gym-anm` framework was designed with one goal in mind: **bridge the gap between research in RL and in\nthe management of power systems**. We attempt to do this by providing RL researchers with an easy-to-work-with\nlibrary of environments that model decision-making tasks in power grids.\n\n**Papers:**\n*  [Gym-ANM: Reinforcement Learning Environments for Active Network Management Tasks in Electricity Distribution Systems](https://doi.org/10.1016/j.egyai.2021.100092)\n*  [Gym-ANM: Open-source software to leverage reinforcement learning for power system management in research and education](https://doi.org/10.1016/j.simpa.2021.100092)\n\n## Key features\n*  Very little background in electricity systems modelling it required. This makes `gym-anm` an ideal starting point\n   for RL students and researchers looking to enter the field.\n*  The environments (tasks) generated by `gym-anm` follow the [OpenAI Gym](https://github.com/openai/gym)\n   framework, with which a large part of the RL community is already familiar.\n*  The flexibility of `gym-anm`, with its different customizable components, makes it a suitable framework\n   to model a wide range of ANM tasks, from simple ones that can be used for educational purposes, to complex ones\n   designed to conduct advanced research.\n\n## Documentation\nDocumentation is provided online at [https://gym-anm.readthedocs.io/en/latest/](https://gym-anm.readthedocs.io/en/latest/).\n\n## Installation\n\n### Requirements\n`gym-anm` requires Python 3.8+ and can run on Linux, MaxOS, and Windows. Some rendering features may not work properly\non Windows (not tested).\n\nWe recommend installing `gym-anm` in a Python environment (e.g., [virtualenv](https://virtualenv.pypa.io/en/latest/)\nor [conda](https://conda.io/en/latest/#)).\n\n### Using pip\nUsing pip (preferably after activating your virtual environment):\n```\npip install gym-anm\n```\n\n### Building from source\nAlternatively, you can build `gym-anm` directly from source:\n```\ngit clone https://github.com/robinhenry/gym-anm.git\ncd gym-anm\npip install -e .\n```\n\n## Example\nThe following code snippet illustrates how `gym-anm` environments can be used. In this example,\nactions are randomly sampled from the action space of the environment `ANM6Easy-v0`. For more information\nabout the agent-environment interface, see the official [OpenAI Gym documentation](https://github.com/openai/gym).\n```\nimport gym\nimport time\n\ndef run():\n   env = gym.make('gym_anm:ANM6Easy-v0')\n   o = env.reset()\n\n   for i in range(100):\n       a = env.action_space.sample()\n       o, r, done, info = env.step(a)\n       env.render()\n       time.sleep(0.5)  # otherwise the rendering is too fast for the human eye.\n\n   env.close()\n\nif __name__ == '__main__':\n    run()\n```\nThe above code would render the environment in your default web browser as shown in the image below:\n![alt text](https://github.com/robinhenry/gym-anm/blob/master/docs/source/images/anm6-easy-example.png?raw=true)\n\nAdditional example scripts can be found in [examples/](examples).\n\n## Testing the installation\nAll unit tests in `gym-anm` can be ran from the project root directory with:\n```\npython -m pytest tests\n```\n\n## Contributing\nContributions are always welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.\n\n## Citing the project\nAll publications derived from the use of `gym-anm` should cite the following two 2021 papers:\n```\n@article{HENRY2021100092,\n    title = {Gym-ANM: Reinforcement learning environments for active network management tasks in electricity distribution systems},\n    journal = {Energy and AI},\n    volume = {5},\n    pages = {100092},\n    year = {2021},\n    issn = {2666-5468},\n    doi = {https://doi.org/10.1016/j.egyai.2021.100092},\n    author = {Robin Henry and Damien Ernst},\n}\n```\n```\n@article{HENRY2021100092,\n    title = {Gym-ANM: Open-source software to leverage reinforcement learning for power system management in research and education},\n    journal = {Software Impacts},\n    volume = {9},\n    pages = {100092},\n    year = {2021},\n    issn = {2665-9638},\n    doi = {https://doi.org/10.1016/j.simpa.2021.100092},\n    author = {Robin Henry and Damien Ernst}\n}\n```\n\n## Maintainers\n`gym-anm` is currently maintained by [Robin Henry](https://www.robinxhenry.com/).\n\n## License\nThis project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.\n",
-    'author': 'Robin Henry',
-    'author_email': 'robin@robinxhenry.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/robinhenry/gym-anm',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
+Metadata-Version: 2.1
+Name: gym-anm
+Version: 1.1.5
+Summary: A framework to build Reinforcement Learning environments for Active Network Management tasks in electricity networks.
+Home-page: https://github.com/robinhenry/gym-anm
+License: MIT
+Author: Robin Henry
+Author-email: robin@robinxhenry.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cvxpy (>=1.2.2,<2.0.0)
+Requires-Dist: gym (>=0.26.2,<0.27.0)
+Requires-Dist: numpy (>=1.23.5,<2.0.0)
+Requires-Dist: pandas (>=1.5.2,<2.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: websocket-client (==0.56.0)
+Requires-Dist: websocket-server (==0.4)
+Project-URL: Documentation, https://gym-anm.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/robinhenry/gym-anm
+Description-Content-Type: text/markdown
+
+# Gym-ANM
+[![Downloads](https://pepy.tech/badge/gym-anm)](https://pepy.tech/project/gym-anm)
+[![Documentation Status](https://readthedocs.org/projects/ansicolortags/badge/?version=latest)](https://gym-anm.readthedocs.io/en/latest/)
+[![codecov](https://codecov.io/gh/robinhenry/gym-anm/branch/master/graph/badge.svg?token=7JSMJPPIQ7)](https://codecov.io/gh/robinhenry/gym-anm)
+[![Checks](https://github.com/robinhenry/gym-anm/actions/workflows/ci_checks.yml/badge.svg)](https://github.com/robinhenry/gym-anm/actions/workflows/ci_checks.yml)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+
+`gym-anm` is a framework for designing reinforcement learning (RL) environments that model Active Network
+Management (ANM) tasks in electricity distribution networks. It is built on top of the
+[OpenAI Gym](https://github.com/openai/gym) toolkit.
+
+The `gym-anm` framework was designed with one goal in mind: **bridge the gap between research in RL and in
+the management of power systems**. We attempt to do this by providing RL researchers with an easy-to-work-with
+library of environments that model decision-making tasks in power grids.
+
+**Papers:**
+*  [Gym-ANM: Reinforcement Learning Environments for Active Network Management Tasks in Electricity Distribution Systems](https://doi.org/10.1016/j.egyai.2021.100092)
+*  [Gym-ANM: Open-source software to leverage reinforcement learning for power system management in research and education](https://doi.org/10.1016/j.simpa.2021.100092)
+
+## Key features
+*  Very little background in electricity systems modelling it required. This makes `gym-anm` an ideal starting point
+   for RL students and researchers looking to enter the field.
+*  The environments (tasks) generated by `gym-anm` follow the [OpenAI Gym](https://github.com/openai/gym)
+   framework, with which a large part of the RL community is already familiar.
+*  The flexibility of `gym-anm`, with its different customizable components, makes it a suitable framework
+   to model a wide range of ANM tasks, from simple ones that can be used for educational purposes, to complex ones
+   designed to conduct advanced research.
+
+## Documentation
+Documentation is provided online at [https://gym-anm.readthedocs.io/en/latest/](https://gym-anm.readthedocs.io/en/latest/).
+
+## Installation
+
+### Requirements
+`gym-anm` requires Python 3.8+ and can run on Linux, MaxOS, and Windows. Some rendering features may not work properly
+on Windows (not tested).
+
+We recommend installing `gym-anm` in a Python environment (e.g., [virtualenv](https://virtualenv.pypa.io/en/latest/)
+or [conda](https://conda.io/en/latest/#)).
+
+### Using pip
+Using pip (preferably after activating your virtual environment):
+```
+pip install gym-anm
+```
+
+### Building from source
+Alternatively, you can build `gym-anm` directly from source:
+```
+git clone https://github.com/robinhenry/gym-anm.git
+cd gym-anm
+pip install -e .
+```
+
+## Example
+The following code snippet illustrates how `gym-anm` environments can be used. In this example,
+actions are randomly sampled from the action space of the environment `ANM6Easy-v0`. For more information
+about the agent-environment interface, see the official [OpenAI Gym documentation](https://github.com/openai/gym).
+```
+import gym
+import time
+
+def run():
+   env = gym.make('gym_anm:ANM6Easy-v0')
+   o = env.reset()
+
+   for i in range(100):
+       a = env.action_space.sample()
+       o, r, done, info = env.step(a)
+       env.render()
+       time.sleep(0.5)  # otherwise the rendering is too fast for the human eye.
+
+   env.close()
+
+if __name__ == '__main__':
+    run()
+```
+The above code would render the environment in your default web browser as shown in the image below:
+![alt text](https://github.com/robinhenry/gym-anm/blob/master/docs/source/images/anm6-easy-example.png?raw=true)
+
+Additional example scripts can be found in [examples/](examples).
+
+## Testing the installation
+All unit tests in `gym-anm` can be ran from the project root directory with:
+```
+python -m pytest tests
+```
+
+## Contributing
+Contributions are always welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first.
+
+## Citing the project
+All publications derived from the use of `gym-anm` should cite the following two 2021 papers:
+```
+@article{HENRY2021100092,
+    title = {Gym-ANM: Reinforcement learning environments for active network management tasks in electricity distribution systems},
+    journal = {Energy and AI},
+    volume = {5},
+    pages = {100092},
+    year = {2021},
+    issn = {2666-5468},
+    doi = {https://doi.org/10.1016/j.egyai.2021.100092},
+    author = {Robin Henry and Damien Ernst},
+}
+```
+```
+@article{HENRY2021100092,
+    title = {Gym-ANM: Open-source software to leverage reinforcement learning for power system management in research and education},
+    journal = {Software Impacts},
+    volume = {9},
+    pages = {100092},
+    year = {2021},
+    issn = {2665-9638},
+    doi = {https://doi.org/10.1016/j.simpa.2021.100092},
+    author = {Robin Henry and Damien Ernst}
 }
+```
+
+## Maintainers
+`gym-anm` is currently maintained by [Robin Henry](https://www.robinxhenry.com/).
 
+## License
+This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
 
-setup(**setup_kwargs)
```

