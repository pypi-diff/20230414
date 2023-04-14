# Comparing `tmp/pyees-1.1.3.tar.gz` & `tmp/pyees-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.1.3.tar", last modified: Mon Mar 13 13:35:18 2023, max compression
+gzip compressed data, was "pyees-1.1.4.tar", last modified: Fri Apr 14 07:49:40 2023, max compression
```

## Comparing `pyees-1.1.3.tar` & `pyees-1.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-03-13 13:35:18.606860 pyees-1.1.3/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0      616 2023-03-13 13:35:18.618829 pyees-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-03-13 13:35:18.412380 pyees-1.1.3/pyees/
--rw-rw-rw-   0        0        0      308 2023-03-09 12:26:40.000000 pyees-1.1.3/pyees/__init__.py
--rw-rw-rw-   0        0        0    15688 2023-03-11 13:10:44.000000 pyees-1.1.3/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-03-07 14:27:06.000000 pyees-1.1.3/pyees/profilePyees.py
--rw-rw-rw-   0        0        0     8963 2023-03-13 12:20:12.000000 pyees-1.1.3/pyees/prop.py
--rw-rw-rw-   0        0        0    16020 2023-03-07 14:33:13.000000 pyees-1.1.3/pyees/readData.py
--rw-rw-rw-   0        0        0     7175 2023-03-07 14:26:45.000000 pyees-1.1.3/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.1.3/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     3249 2023-03-13 12:35:20.000000 pyees-1.1.3/pyees/testFit.py
--rw-rw-rw-   0        0        0     1671 2023-03-07 14:26:33.000000 pyees-1.1.3/pyees/testProp.py
--rw-rw-rw-   0        0        0     1059 2023-03-09 12:40:27.000000 pyees-1.1.3/pyees/testPyees.py
--rw-rw-rw-   0        0        0     8615 2023-03-07 14:25:53.000000 pyees-1.1.3/pyees/testReadData.py
--rw-rw-rw-   0        0        0    12271 2023-03-07 14:25:05.000000 pyees-1.1.3/pyees/testSolve.py
--rw-rw-rw-   0        0        0     7326 2023-03-13 12:56:04.000000 pyees-1.1.3/pyees/testUnit.py
--rw-rw-rw-   0        0        0    75387 2023-03-13 13:34:08.000000 pyees-1.1.3/pyees/testVariable.py
--rw-rw-rw-   0        0        0    41289 2023-03-13 13:25:22.000000 pyees-1.1.3/pyees/unit.py
--rw-rw-rw-   0        0        0    31530 2023-03-13 13:23:17.000000 pyees-1.1.3/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-03-13 13:35:18.581925 pyees-1.1.3/pyees.egg-info/
--rw-rw-rw-   0        0        0      616 2023-03-13 13:35:17.000000 pyees-1.1.3/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-03-13 13:35:17.000000 pyees-1.1.3/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-13 13:35:17.000000 pyees-1.1.3/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-03-13 13:35:18.562977 pyees-1.1.3/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-03-13 13:35:17.000000 pyees-1.1.3/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-03-13 13:35:18.636781 pyees-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-03-13 13:34:41.000000 pyees-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:49:21.165818 pyees-1.1.4/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      616 2023-04-14 07:49:21.181443 pyees-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 07:49:20.931442 pyees-1.1.4/pyees/
+-rw-rw-rw-   0        0        0      619 2023-03-30 05:48:48.000000 pyees-1.1.4/pyees/__init__.py
+-rw-rw-rw-   0        0        0    15688 2023-03-11 13:10:44.000000 pyees-1.1.4/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.1.4/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0     8922 2023-04-03 12:12:15.000000 pyees-1.1.4/pyees/prop.py
+-rw-rw-rw-   0        0        0    14265 2023-04-14 07:44:37.000000 pyees-1.1.4/pyees/readData.py
+-rw-rw-rw-   0        0        0    10138 2023-04-05 08:09:23.000000 pyees-1.1.4/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.1.4/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     3249 2023-03-13 12:35:20.000000 pyees-1.1.4/pyees/testFit.py
+-rw-rw-rw-   0        0        0     1671 2023-03-07 14:26:33.000000 pyees-1.1.4/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1059 2023-04-14 07:48:34.000000 pyees-1.1.4/pyees/testPyees.py
+-rw-rw-rw-   0        0        0     9133 2023-04-03 11:24:36.000000 pyees-1.1.4/pyees/testReadData.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.1.4/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     8044 2023-04-14 07:44:27.000000 pyees-1.1.4/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    80327 2023-04-03 13:10:52.000000 pyees-1.1.4/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    43305 2023-04-14 07:48:22.000000 pyees-1.1.4/pyees/unit.py
+-rw-rw-rw-   0        0        0    34501 2023-04-14 06:49:23.000000 pyees-1.1.4/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-04-14 07:49:21.118943 pyees-1.1.4/pyees.egg-info/
+-rw-rw-rw-   0        0        0      616 2023-04-14 07:49:19.000000 pyees-1.1.4/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-04-14 07:49:19.000000 pyees-1.1.4/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 07:49:19.000000 pyees-1.1.4/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-14 07:49:19.000000 pyees-1.1.4/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-14 07:49:19.000000 pyees-1.1.4/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-14 07:49:21.212694 pyees-1.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2023-04-14 07:49:13.000000 pyees-1.1.4/setup.py
```

### Comparing `pyees-1.1.3/LICENSE.txt` & `pyees-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.1.3/PKG-INFO` & `pyees-1.1.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.1.3
+Version: 1.1.4
 Summary: EES but for python
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.1.3/README.md` & `pyees-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.1.3/pyees/fit.py` & `pyees-1.1.4/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.3/pyees/profilePyees.py` & `pyees-1.1.4/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.3/pyees/prop.py` & `pyees-1.1.4/pyees/prop.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,16 @@
     fluid = Fluid(FluidsList.Water)
     fluid = fluid.with_state(Input.temperature(T.value), Input.pressure(P.value))
     
     ## create a variable from the fluid
     var = getattr(fluid, property)
     var = variable(var, propertyUnits[property])
     vars, grads = differentials(fluid, property, [T, P])
-    var._addDependents(vars, grads)
+    for v, g in zip(vars, grads):
+        var._addDependent(v,g)
     var._calculateUncertanty()
     
     ## return the variable
     return var
    
     
 def propMEG(property, arguments):
@@ -199,15 +200,16 @@
     ## update the fluid state
     fluid = fluid.with_state(Input.temperature(T.value), Input.pressure(P.value))
     
     ## create a variable from the fluid
     var = getattr(fluid, property)
     var = variable(var, propertyUnits[property])
     vars, grads = differentialsBrine(fluid, FluidsList.MEG, property, C, [T, P])
-    var._addDependents(vars, grads)
+    for v, g in zip(vars, grads):
+        var._addDependent(v,g)
     var._calculateUncertanty()
     
     ## convert the arguments back in to the original units
     T.convert(Tunit)
     P.convert(Punit)
     
     ## return the variable
@@ -272,16 +274,17 @@
         
     fluid = HumidAir()    
     fluid = fluid.with_state(*inputs)
     
     ## create a variable from the fluid
     var = getattr(fluid, property)
     var = variable(var, propertyUnits[property])
-    Vars, grads = differentials(fluid, property, vars)
-    var._addDependents(Vars, grads)
+    vars, grads = differentials(fluid, property, vars)
+    for v, g in zip(vars, grads):
+        var._addDependent(v,g)
     var._calculateUncertanty()
     
     return var 
 
 propertyUnits = {
     'density': 'kg/m3',
     'specific_heat': 'J/kg-K',
@@ -296,12 +299,7 @@
 
 knownFluids = {
     'water': [propWater],
     'MEG': [propMEG],
     'air': [propHumidAir]
 }
 
-
-if __name__ == '__main__':
-    rho = prop('density', 'water', P = variable(1,'bar'), T = variable(30,'C'))
-    print(rho)
-
```

### Comparing `pyees-1.1.3/pyees/readData.py` & `pyees-1.1.4/pyees/readData.py`

 * *Files 14% similar despite different names*

```diff
@@ -135,24 +135,26 @@
                 head = '_' + head
 
             # remove "_" if the last letter is "_"
             if head[-1] == "_" and len(head) != 1:
                 head = head[0:-1]
 
             # add a number to the end of the unit if the unit exists
-            i, imax, done = 0, 100, False
-            while not done and i <= imax:
-                if i > 0:
-                    h = head + f'_{i+2}'
-                else:
-                    h = head
-                if h not in out:
-                    out.append(h)
-                    done = True
-
+            if head not in out:
+                out.append(head)
+            else:
+                i, imax, done = 1, 100, False
+                while not done and i <= imax:
+                    h = head + f'_{i+1}'
+                    if h not in out:
+                        out.append(h)
+                        done = True
+                    i += 1
+                if not done:
+                    raise ValueError(f'The header {head} could not be added to the sheet')
         return out
 
     def readData(self):
         self.dat = _Data()
 
         # Looping over the sheets in the data file
         for i, sheet in enumerate(self.sheets):
@@ -242,15 +244,15 @@
                         vars.append(var)
 
                     for i in range(self.nCols):
                         covariance = [elem[:, i] for elem in uncert]
                         for j in range(self.nCols):
                             if i != j:
                                 cov = [elem[j] for elem in covariance]
-                                vars[i]._addCovariance(vars[j], cov)
+                                vars[i].addCovariance(vars[j], cov, str(vars[i]._unitObject * vars[j]._unitObject))
 
                     for head, var in zip(headers, vars):
                         sheetData._addMeasurement(head, var)
             else:
                 # There are no uncertaty data in the sheet
 
                 # create the measurements without uncertanties
@@ -320,73 +322,39 @@
 
         for measurement, measurementName in zip(measurements, self.measurementNames):
             sheet._addMeasurement(measurementName, measurement)
 
         return sheet
 
     def append(self, other):
-
         if not isinstance(other, _Sheet):
             raise ValueError('You can only append two sheets together')
 
         # Test if all names are the same
         for elem in self.measurementNames:
             if elem not in other.measurementNames:
                 raise ValueError('You can only append sheets with the excact same measurements. The names did not match')
 
-        # get the measurements in the same order
-        measA = self.measurements
-        measB = []
-        for elem in self.measurementNames:
-            index = other.measurementNames.index(elem)
-            measB.append(other.measurements[index])
-
-        # test if all units are the same
-        for elemA, elemB in zip(measA, measB):
-            if str(elemA.unit) != str(elemB.unit):
-                raise ValueError('You can only append sheets with the excact same measurements. The units did not match')
-
-        # append the data
-        for i in range(len(self.measurements)):
-            meas_i = measB[i]
-            self.measurements[i]._value = np.append(self.measurements[i].value, meas_i.value)
-            self.measurements[i]._uncert = np.append(self.measurements[i].uncert, meas_i.uncert)
-            if len(self.measurements[i].covariance) == 0:
-                if len(meas_i.covariance) == 0:
-                    # do nothing
-                    pass
-                else:
-                    # create covarinace for self.measurements[i] and fill it with zeros
-                    nData = int(len(self.measurements[i].value) / 2)
-                    for j in range(len(self.measurements)):
-                        if i != j:
-                            self.measurements[i].covariance[self.measurements[j]] = [0] * nData
-
-                    # append the covariance from meas_i
-                    keys = list(self.measurements[i].covariance.keys())
-                    keys_i = list(meas_i.covariance.keys())
-                    for key_i, name in zip(keys_i, other.measurementNames):
-                        index = self.measurementNames.index(name)
-                        self.measurements[i].covariance[keys[index]] = np.append(self.measurements[i].covariance[keys[index]], meas_i.covariance[key_i])
-            else:
-                if len(meas_i.covariance) == 0:
-                    # append zeros to the covariance of self.measurements[i]
-                    nData = int(len(self.measurements[i].value) / 2)
-                    for key in self.measurements[i].covariance.keys():
-                        self.measurements[i].covariance[key] = np.append(self.measurements[i].covariance[key], [0] * nData)
-                else:
-                    # append the covariance of meas_i to the covariance of self.measurements[i]
-                    keys = list(self.measurements[i].covariance.keys())
-                    keys_i = list(meas_i.covariance.keys())
-                    for key_i, name in zip(keys_i, other.measurementNames):
-                        index = self.measurementNames.index(name)
-                        self.measurements[i].covariance[keys[index]] = np.append(self.measurements[i].covariance[keys[index]], meas_i.covariance[key_i])
+        for elem in other.measurementNames:
+            if elem not in self.measurementNames:
+                raise ValueError('You can only append sheets with the excact same measurements. The names did not match')
 
+        # append the measurements from other to self
+        for elem, elemNames in zip(self.measurements, self.measurementNames):
+            index = other.measurementNames.index(elemNames)
+            elem.append(other.measurements[index])    
+        
     def __iter__(self):
         return iter(self.measurements)
 
 
+## TODO change the name of "import data.md" to "sheet.md"
+## TODO remove the _Data class. instead return a list of Sheets
+## TODO change the name of "_Sheet" to "Sheet"
+## TODO change the name of "readData" to "sheetFromFile"
+## TODO read data vælg ark
+## TODO the inputs of "sheetFromFile" has to be able to take list-list inputs and return a list of Sheets
+## TODO save Sheet as xlFile
+
+## TODO error when reading from multiple sheets with different number of rows
 
 
-## TODOread data vælg ark
-## TODO vælg område for hvert ark seperat
-## TODO save sheet as new file
```

### Comparing `pyees-1.1.3/pyees/stackOverflowODR.py` & `pyees-1.1.4/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.3/pyees/testFit.py` & `pyees-1.1.4/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.3/pyees/testProp.py` & `pyees-1.1.4/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.3/pyees/testPyees.py` & `pyees-1.1.4/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.3/pyees/testReadData.py` & `pyees-1.1.4/pyees/testReadData.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,22 +40,22 @@
         self.assertEqual(str(dat.s1.b.unit), 'mA')
         np.testing.assert_array_equal(dat.s1.b.uncert, [0.5, 0.6, 0.7, 0.8, 0.9])
 
         dat = readData('testData/data4.xlsx', 'A-B', 'C-D')
         np.testing.assert_array_equal(dat.s1.a.value, [1, 2, 3, 4, 5])
         self.assertEqual(str(dat.s1.a.unit), 'L/min')
         np.testing.assert_array_equal(dat.s1.a.uncert, [0.05, 0.1, 0.15, 0.2, 0.25])
-        np.testing.assert_almost_equal(dat.s1.a.covariance[dat.s1.b], [0.025, 0.06, 0.105, 0.16, 0.225])
+        np.testing.assert_almost_equal([elemA.covariance[elemB] for elemA, elemB in zip(dat.s1.a, dat.s1.b)], np.array([0.025, 0.06, 0.105, 0.16, 0.225])/1000 / 60 / 1000)
         np.testing.assert_array_equal(dat.s1.b.value, [5, 6, 7, 8, 9])
         self.assertEqual(str(dat.s1.b.unit), 'mA')
         np.testing.assert_array_equal(dat.s1.b.uncert, [0.5, 0.6, 0.7, 0.8, 0.9])
-        np.testing.assert_almost_equal(dat.s1.b.covariance[dat.s1.a], [0.025, 0.06, 0.105, 0.16, 0.225])
+        np.testing.assert_almost_equal([elemB.covariance[elemA] for elemA, elemB in zip(dat.s1.a, dat.s1.b)], np.array([0.025, 0.06, 0.105, 0.16, 0.225])/1000 / 60 / 1000)
 
         with self.assertRaises(Exception) as context:
-            dat6 = readData('testData/data6.xlsx', 'A-B', 'C-D')
+            readData('testData/data6.xlsx', 'A-B', 'C-D')
         self.assertTrue("The covariances has to be symmetric" in str(context.exception))
 
     def testAppend(self):
         dat1 = readData('testData/data1.xlsx', 'A-B')
         dat2 = readData('testData/data2.xlsx', 'A-B')
         dat1.s1.append(dat2.s1)
         np.testing.assert_array_equal(dat1.s1.a.value, [1, 2, 3, 4, 5, 1, 2, 3, 4, 5])
@@ -71,50 +71,58 @@
             dat4.s1.append(dat5.s1)
         self.assertTrue("You can only append sheets with the excact same measurements. The names did not match" in str(context.exception))
 
         dat3 = readData('testData/data3.xlsx', 'A-B')
         dat4 = readData('testData/data4.xlsx', 'A-B')
         with self.assertRaises(Exception) as context:
             dat3.s1.append(dat4.s1)
-        self.assertTrue("You can only append sheets with the excact same measurements. The units did not match" in str(context.exception))
+        self.assertTrue("You can not set an element of [1, 2, 3, 4, 5] [m] with [1, 2, 3, 4, 5] [L/min] as they do not have the same unit" in str(context.exception))
 
         dat2 = readData('testData/data2.xlsx', 'A-B', 'C-D')
         dat4 = readData('testData/data4.xlsx', 'A-B', 'C-D')
         dat2.s1.append(dat4.s1)
         np.testing.assert_array_equal(dat2.s1.a.value, [1, 2, 3, 4, 5, 1, 2, 3, 4, 5])
         self.assertEqual(str(dat2.s1.a.unit), 'L/min')
         np.testing.assert_array_equal(dat2.s1.a.uncert, [0.05, 0.1, 0.15, 0.2, 0.25, 0.05, 0.1, 0.15, 0.2, 0.25])
         np.testing.assert_array_equal(dat2.s1.b.value, [5, 6, 7, 8, 9, 5, 6, 7, 8, 9])
         self.assertEqual(str(dat2.s1.b.unit), 'mA')
         np.testing.assert_array_equal(dat2.s1.b.uncert, [0.5, 0.6, 0.7, 0.8, 0.9, 0.5, 0.6, 0.7, 0.8, 0.9])
-        np.testing.assert_almost_equal(dat2.s1.a.covariance[dat2.s1.b], [0, 0, 0, 0, 0, 0.025, 0.06, 0.105, 0.16, 0.225])
-        np.testing.assert_almost_equal(dat2.s1.b.covariance[dat2.s1.a], [0, 0, 0, 0, 0, 0.025, 0.06, 0.105, 0.16, 0.225])
-
+        cov = np.array([0, 0, 0, 0, 0, 0.025, 0.06, 0.105, 0.16, 0.225]) / 1000 / 60 / 1000
+        for i, (elemA, elemB) in enumerate(zip(dat2.s1.a, dat2.s1.b)):
+            if elemB in elemA.covariance:
+                self.assertAlmostEqual(elemA.covariance[elemB], cov[i])
+                self.assertAlmostEqual(elemB.covariance[elemA], cov[i])
+                
+            
         dat2 = readData('testData/data2.xlsx', 'A-B', 'C-D')
         dat4 = readData('testData/data4.xlsx', 'A-B', 'C-D')
         dat4.s1.append(dat2.s1)
         np.testing.assert_array_equal(dat4.s1.a.value, [1, 2, 3, 4, 5, 1, 2, 3, 4, 5])
         self.assertEqual(str(dat4.s1.a.unit), 'L/min')
         np.testing.assert_array_equal(dat4.s1.a.uncert, [0.05, 0.1, 0.15, 0.2, 0.25, 0.05, 0.1, 0.15, 0.2, 0.25])
         np.testing.assert_array_equal(dat4.s1.b.value, [5, 6, 7, 8, 9, 5, 6, 7, 8, 9])
         self.assertEqual(str(dat4.s1.b.unit), 'mA')
         np.testing.assert_array_equal(dat4.s1.b.uncert, [0.5, 0.6, 0.7, 0.8, 0.9, 0.5, 0.6, 0.7, 0.8, 0.9])
-        np.testing.assert_almost_equal(dat4.s1.a.covariance[dat4.s1.b], [0.025, 0.06, 0.105, 0.16, 0.225, 0, 0, 0, 0, 0])
-        np.testing.assert_almost_equal(dat4.s1.b.covariance[dat4.s1.a], [0.025, 0.06, 0.105, 0.16, 0.225, 0, 0, 0, 0, 0])
-
+        cov = np.array([0.025, 0.06, 0.105, 0.16, 0.225, 0, 0, 0, 0, 0]) / 1000 / 60 / 1000
+        for i, (elemA, elemB) in enumerate(zip(dat4.s1.a, dat4.s1.b)):
+            if elemB in elemA.covariance:
+                self.assertAlmostEqual(elemA.covariance[elemB], cov[i])
+                self.assertAlmostEqual(elemB.covariance[elemA], cov[i])
+       
+        dat4_1 = readData('testData/data4.xlsx', 'A-B', 'C-D')
         dat4_2 = readData('testData/data4.xlsx', 'A-B', 'C-D')
-        dat4.s1.append(dat4_2.s1)
-        np.testing.assert_array_equal(dat4.s1.a.value, [1, 2, 3, 4, 5, 1, 2, 3, 4, 5, 1, 2, 3, 4, 5])
-        self.assertEqual(str(dat4.s1.a.unit), 'L/min')
-        np.testing.assert_array_equal(dat4.s1.a.uncert, [0.05, 0.1, 0.15, 0.2, 0.25, 0.05, 0.1, 0.15, 0.2, 0.25, 0.05, 0.1, 0.15, 0.2, 0.25])
-        np.testing.assert_array_equal(dat4.s1.b.value, [5, 6, 7, 8, 9, 5, 6, 7, 8, 9, 5, 6, 7, 8, 9])
-        self.assertEqual(str(dat4.s1.b.unit), 'mA')
-        np.testing.assert_array_equal(dat4.s1.b.uncert, [0.5, 0.6, 0.7, 0.8, 0.9, 0.5, 0.6, 0.7, 0.8, 0.9, 0.5, 0.6, 0.7, 0.8, 0.9])
-        np.testing.assert_almost_equal(dat4.s1.a.covariance[dat4.s1.b], [0.025, 0.06, 0.105, 0.16, 0.225, 0, 0, 0, 0, 0, 0.025, 0.06, 0.105, 0.16, 0.225])
-        np.testing.assert_almost_equal(dat4.s1.b.covariance[dat4.s1.a], [0.025, 0.06, 0.105, 0.16, 0.225, 0, 0, 0, 0, 0, 0.025, 0.06, 0.105, 0.16, 0.225])
+        dat4_1.s1.append(dat4_2.s1)
+        np.testing.assert_array_equal(dat4_1.s1.a.value, [1, 2, 3, 4, 5, 1, 2, 3, 4, 5])
+        self.assertEqual(str(dat4_1.s1.a.unit), 'L/min')
+        np.testing.assert_array_equal(dat4_1.s1.a.uncert, [0.05, 0.1, 0.15, 0.2, 0.25, 0.05, 0.1, 0.15, 0.2, 0.25])
+        np.testing.assert_array_equal(dat4_1.s1.b.value, [5, 6, 7, 8, 9, 5, 6, 7, 8, 9])
+        self.assertEqual(str(dat4_1.s1.b.unit), 'mA')
+        np.testing.assert_array_equal(dat4_1.s1.b.uncert, [0.5, 0.6, 0.7, 0.8, 0.9, 0.5, 0.6, 0.7, 0.8, 0.9])
+        np.testing.assert_almost_equal([elemA.covariance[elemB] for elemA, elemB in zip(dat4_1.s1.a, dat4_1.s1.b)], np.array([0.025, 0.06, 0.105, 0.16, 0.225, 0.025, 0.06, 0.105, 0.16, 0.225]) / 1000 / 60 / 6000)
+        np.testing.assert_almost_equal([elemB.covariance[elemA] for elemA, elemB in zip(dat4_1.s1.a, dat4_1.s1.b)], np.array([0.025, 0.06, 0.105, 0.16, 0.225, 0.025, 0.06, 0.105, 0.16, 0.225]) / 1000 / 60 / 6000)
 
     def testIndex(self):
         dat = readData('testData/data1.xlsx', 'A-B')
         np.testing.assert_array_equal(dat.s1.a.value, [1, 2, 3, 4, 5])
         self.assertEqual(str(dat.s1.a.unit), 'L/min')
         np.testing.assert_array_equal(dat.s1.a.uncert, [0, 0, 0, 0, 0])
         np.testing.assert_array_equal(dat.s1.b.value, [5, 6, 7, 8, 9])
```

### Comparing `pyees-1.1.3/pyees/testUnit.py` & `pyees-1.1.4/pyees/testUnit.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,28 +75,47 @@
         _,cUnit,_,_,_ = a + b
         self.assertEqual(cUnit, 'L/min')
 
         a = unit('m-K/L-bar')
         b = unit('K-m/bar-L')
         _,cUnit,_,_,_ = a + b
         self.assertTrue(unit._assertEqualStatic(cUnit, 'DELTAK-m/bar-L'))
-
+        
+        a = unit('J/kg-DELTAK')
+        b = unit('J/kg-DELTAK')
+        _,cUnit,_,_,_ = a + b
+        self.assertTrue(unit._assertEqualStatic(cUnit, 'J/kg-DELTAK'))
+        
+        a = unit('J/g-DELTAK')
+        b = unit('J/kg-DELTAK')
+        _,cUnit,_,_,_ = a + b
+        self.assertTrue(unit._assertEqualStatic(cUnit, 'J/g-DELTAK'))
+        
     def testSub(self):
         a = unit('L/min')
         b = unit('kg-m/L')
         
         with self.assertRaises(Exception) as context:
             a-b
         self.assertTrue('You tried to subtract a variable in [kg-m/L] from a variable in [L/min], but the units do not have the same SI base unit' in str(context.exception))
-
         
         a = unit('L/min')
         b = unit('L/min')
         _,cUnit,_,_,_ = a - b
         self.assertEqual(str(cUnit), 'L/min')
+        
+        a = unit('J/kg-DELTAK')
+        b = unit('J/kg-DELTAK')
+        _,cUnit,_,_,_ = a - b
+        self.assertTrue(unit._assertEqualStatic(cUnit, 'J/kg-DELTAK'))
+        
+        a = unit('J/g-DELTAK')
+        b = unit('J/kg-DELTAK')
+        _,cUnit,_,_,_ = a - b
+        self.assertTrue(unit._assertEqualStatic(cUnit, 'J/g-DELTAK'))
 
     def testConvert(self):
         a = unit('L/min')
         converter = a.getConverter('m3/h')
         self.assertAlmostEqual(converter.convert(1), 0.06)
 
         a = unit('K')
```

### Comparing `pyees-1.1.3/pyees/testVariable.py` & `pyees-1.1.4/pyees/testVariable.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,14 +146,29 @@
             A + B
         self.assertTrue('You tried to add a variable in [L/min] to a variable in [m], but the units do not have the same SI base unit' in str(context.exception))
 
         with self.assertRaises(Exception) as context:
             A_vec + B_vec
         self.assertTrue('You tried to add a variable in [L/min] to a variable in [m], but the units do not have the same SI base unit' in str(context.exception))
 
+        a = variable(10, 'L', 1.2)
+        b = variable(100, 'mL', 3.9)
+        c = a + b
+        self.assertEqual(c.value, 10.1)
+        self.assertEqual(c.unit, 'L')
+        self.assertEqual(c.uncert, np.sqrt((1 * 1.2)**2 + (1 * 3.9/1000)**2))
+        
+        
+        a = variable(10, 'C', 1.2)
+        b = variable(100, 'muC', 3.9)
+        c = a + b
+        self.assertEqual(c.value, 10 + 100 * 1e-6)
+        self.assertEqual(c.unit, 'C')
+        self.assertEqual(c.uncert, np.sqrt((1 * 1.2)**2 + (1 * 3.9*1e-6)**2))
+
     def test_sub_with_different_units(self):
         A = variable(12.3, 'm3/s', uncert=2.6)
         B = variable(745.1, 'L/min', uncert=53.9)
         C = A - B
         self.assertAlmostEqual(C.value, 12.3 - 745.1 / 1000 / 60)
         self.assertEqual(C.unit, 'm3/s')
         self.assertAlmostEqual(C.uncert, np.sqrt(2.6**2 + (53.9 / 1000 / 60)**2))
@@ -189,14 +204,28 @@
             A - B
         self.assertTrue('You tried to subtract a variable in [m] from a variable in [L/min], but the units do not have the same SI base unit' in str(context.exception))
 
         with self.assertRaises(Exception) as context:
             A_vec - B_vec
         self.assertTrue('You tried to subtract a variable in [m] from a variable in [L/min], but the units do not have the same SI base unit' in str(context.exception))
 
+        a = variable(10, 'L', 1.2)
+        b = variable(100, 'mL', 3.9)
+        c = a - b
+        self.assertEqual(c.value, 10 - 100 / 1000)
+        self.assertEqual(c.unit, 'L')
+        self.assertEqual(c.uncert, np.sqrt((1 * 1.2)**2 + (1 * 3.9/1000)**2))
+        
+        a = variable(10, 'C', 1.2)
+        b = variable(100, 'muC', 3.9)
+        c = a - b
+        self.assertAlmostEqual(c.value, 10 - 100 * 1e-6)
+        self.assertEqual(c.unit, 'DELTAC')
+        self.assertEqual(c.uncert, np.sqrt((1 * 1.2)**2 + (1 * 3.9*1e-6)**2))
+
     def test_multiply(self):
         A = variable(12.3, 'L/min', uncert=2.6)
         B = variable(745.1, 'm', uncert=53.9)
         A_vec = variable([12.3, 54.3, 91.3], 'L/min', uncert=[2.6, 5.4, 10.56])
         B_vec = variable([745.1, 496.13, 120.54], 'm', uncert=[53.9, 24.75, 6.4])
 
         C = A * B
@@ -204,15 +233,15 @@
         self.assertAlmostEqual(C.value, 12.3 * 745.1)
         self.assertTrue(C._unitObject._assertEqual('L-m/min'))
         self.assertAlmostEqual(C.uncert, np.sqrt((745.1 * 2.6)**2 + (12.3 * 53.9)**2))
 
         C_vec = A_vec * B_vec
         np.testing.assert_array_equal(C_vec.value, np.array([12.3 * 745.1, 54.3 * 496.13, 91.3 * 120.54]))
         self.assertTrue(C._unitObject._assertEqual('L-m/min'))
-        np.testing.assert_array_equal(
+        np.testing.assert_array_almost_equal(
             C_vec.uncert,
             np.array([
                 np.sqrt((745.1 * 2.6)**2 + (12.3 * 53.9)**2),
                 np.sqrt((496.13 * 5.4)**2 + (54.3 * 24.75)**2),
                 np.sqrt((120.54 * 10.56)**2 + (91.3 * 6.4)**2),
             ]))
 
@@ -249,15 +278,15 @@
         self.assertAlmostEqual(C.value, 12.3 / 745.1 / 1000 * 60 / 1000)
         self.assertEqual(C.unit, 'm3/h-mm')
         self.assertAlmostEqual(C.uncert, np.sqrt((1 / (745.1 * 1000) * 2.6 / 1000 * 60)**2 + (12.3 / ((745.1)**2) * 53.9 / 1000 * 60 / 1000)**2))
 
         C_vec = A_vec / B_vec
         np.testing.assert_array_equal(C_vec.value, np.array([12.3 / 745.1, 54.3 / 496.13, 91.3 / 120.54]))
         self.assertTrue(C_vec._unitObject._assertEqual('L/min-m'))
-        np.testing.assert_array_equal(
+        np.testing.assert_array_almost_equal(
             C_vec.uncert,
             np.array([
                 np.sqrt((1 / 745.1 * 2.6)**2 + (12.3 / (745.1)**2 * 53.9)**2),
                 np.sqrt((1 / 496.13 * 5.4)**2 + (54.3 / (496.13)**2 * 24.75)**2),
                 np.sqrt((1 / 120.54 * 10.56)**2 + (91.3 / (120.54)**2 * 6.4)**2),
             ]))
 
@@ -447,39 +476,24 @@
         self.assertTrue('The exponent can not have a unit' in str(context.exception))
 
     def testIndex(self):
         A = variable(12.3, 'L/min', uncert=2.6)
         A_vec = variable([12.3, 54.3, 91.3], 'L/min', uncert=[2.6, 5.4, 10.56])
 
         with self.assertRaises(Exception) as context:
-            a = A[0]
+            A[0]
         self.assertTrue("'scalarVariable' object is not subscriptable" in str(context.exception))
-        
-        a_vec = A_vec[0, 1]
-        np.testing.assert_equal(a_vec.value, [12.3, 54.3])
-        self.assertEqual(a_vec.unit, 'L/min')
-        np.testing.assert_equal(a_vec.uncert, [2.6, 5.4])
-
-        a_vec = A_vec[0, 2]
-        np.testing.assert_equal(a_vec.value, [12.3, 91.3])
-        self.assertEqual(a_vec.unit, 'L/min')
-        np.testing.assert_equal(a_vec.uncert, [2.6, 10.56])
-
-        a_vec = A_vec[2, 0]
-        np.testing.assert_equal(a_vec.value, [91.3, 12.3])
-        self.assertEqual(a_vec.unit, 'L/min')
-        np.testing.assert_equal(a_vec.uncert, [10.56, 2.6])
 
         with self.assertRaises(Exception) as context:
-            a = A[1]
+            A[1]
         self.assertTrue("'scalarVariable' object is not subscriptable" in str(context.exception))
 
         with self.assertRaises(Exception) as context:
-            a = A_vec[23]
-        self.assertTrue('Index out of bounds' in str(context.exception))
+            A_vec[23]
+        self.assertTrue('list index out of range' in str(context.exception))
 
     def testAddEqual(self):
         A = variable(12.3, 'L/min', uncert=2.6)
         B = variable(745.1, 'L/min', uncert=53.9)
 
         A += B
         self.assertAlmostEqual(A.value, 12.3 + 745.1)
@@ -857,15 +871,14 @@
         self.assertEqual(v.value, np.sqrt(2 * 10 / 2.5))
         
         dP = variable(1, 'bar')
         rho = variable(2.5, 'kg/L')
         v = np.sqrt(2 * dP / rho)
         self.assertEqual(v.value, 8.9442719099991585541)
 
-
     def testLargerUncertThenValue(self):
 
         A = variable(0.003, 'L/min', 0.2)
         self.assertEqual(str(A), '0.0 +/- 0.2 [L/min]')
 
         A = variable(1, 'L/min', 10)
         self.assertEqual(str(A), '0 +/- 10 [L/min]')
@@ -937,15 +950,14 @@
             2**B_vec
         self.assertTrue('The exponent can not have a unit' in str(context.exception))
      
         d_vec = 2**D_vec
         np.testing.assert_equal(d_vec.value, [2**0.34, 2**0.64, 2**0.87])
         self.assertEqual(d_vec.unit, '1')
         self.assertEqual(d_vec.uncert[0], np.sqrt((2**0.34 * np.log(2) * 0.01)**2 + (0.34 * 2**(0.34 - 1) * 0)**2))
-
         
     def testPrettyPrint(self):
         a = variable(12.3, 'm')
         b = variable(12.3, 'm', 2.5)
         c = variable([12.3, 56.2], 'm')
         d = variable([12.3, 56.2], 'm', [2.5, 7.3])
 
@@ -1087,15 +1099,15 @@
         a = variable(23, 'deg', 2)
         b = np.sin(a)
         c = a * b
         val = 23
         unc = 2
         self.assertEqual(c.value, val * np.sin(np.pi / 180 * val))
         self.assertEqual(c.unit, 'deg')
-        self.assertEqual(c.uncert, np.sqrt((unc * (np.sin(np.pi / 180 * val) + (np.pi / 180 * val) * np.cos(np.pi / 180 * val)))**2))
+        self.assertAlmostEqual(c.uncert, np.sqrt((unc * (np.sin(np.pi / 180 * val) + (np.pi / 180 * val) * np.cos(np.pi / 180 * val)))**2))
 
         a = variable(23, 'deg', 2)
         a.convert('rad')
         b = np.sin(a)
         c = a * b
         val = np.pi / 180 * 23
         unc = np.pi / 180 * 2
@@ -1117,15 +1129,15 @@
         b = np.sin(a)
         a.convert('deg')
         c = a * b
         val = 23
         unc = 2
         self.assertEqual(c.value, val * np.sin(np.pi / 180 * val))
         self.assertEqual(c.unit, 'deg')
-        self.assertEqual(c.uncert, np.sqrt((unc * (np.sin(np.pi / 180 * val) + (np.pi / 180 * val) * np.cos(np.pi / 180 * val)))**2))
+        self.assertAlmostEqual(c.uncert, np.sqrt((unc * (np.sin(np.pi / 180 * val) + (np.pi / 180 * val) * np.cos(np.pi / 180 * val)))**2))
 
         a = variable(200, 'L/min', 1.5)
         b = a**2
         self.assertAlmostEqual(b.value, 200 ** 2)
         self.assertEqual(b.unit, 'L2/min2')
         self.assertAlmostEqual(b.uncert, np.sqrt((1.5 * 2 * 200)**2))
 
@@ -1188,38 +1200,60 @@
         e = \sum^{\infty}_{n=0} 1/(n!)
         b = \sum^{\infty}_{n=0} 1/(n!) * a = e*a
         \frac{\partial b}{\partial a} = e
         """
         a = variable(2.3, 'L/min', 0.0237)
         b = variable(0, 'L/min')
         for i in range(15):
-            b += 1 / variable(np.math.factorial(i)) * a
+            b += 1 / np.math.factorial(i) * a
         self.assertAlmostEqual(b.value, np.e * 2.3)
         self.assertEqual(b.unit, 'L/min')
         self.assertAlmostEqual(b.uncert, np.sqrt((np.e * 0.0237)**2))
 
     def testCovariance(self):
         a = variable(123, 'L/min', 9.7)
         b = variable(93, 'Pa', 1.2)
-        a._addCovariance(b, [23])
-        b._addCovariance(a, [23])
+        a.addCovariance(b, 23, 'L-Pa/min')
         c = a * b
         self.assertEqual(c.value, 123 * 93)
         self.assertTrue(c._unitObject._assertEqual('L-Pa/min'))
-        self.assertEqual(c.uncert, np.sqrt((123 * 1.2)**2 + (93 * 9.7)**2 + 2 * 93 * 123 * 23))
+        self.assertAlmostEqual(c.uncert, np.sqrt((123 * 1.2)**2 + (93 * 9.7)**2 + 2 * 93 * 123 * 23))
 
         a = variable(123, 'L/min', 9.7)
         b = variable(93, 'Pa', 1.2)
-        a._addCovariance(b, [23])
-        b._addCovariance(a, [23])
+        a.addCovariance(b, 23, 'L-Pa/min')
+        a.convert('m3/s')
+        c = a * b
+        self.assertEqual(c.value, 123 * 93 / 1000 / 60)
+        self.assertTrue(c._unitObject._assertEqual('m3-Pa/s'))
+        self.assertEqual(c.uncert, np.sqrt((123 / 1000 / 60 * 1.2)**2 + (93 * 9.7 / 1000 / 60)**2 + 2 * 93 * 123 / 1000 / 60 * 23 / 1000 / 60))
+        
+        a = variable(123, 'L/min', 9.7)
+        b = variable(93, 'Pa', 1.2)
+        a.addCovariance(b, 23, 'm3-Pa/s')
         a.convert('m3/s')
         c = a * b
         self.assertEqual(c.value, 123 * 93 / 1000 / 60)
         self.assertTrue(c._unitObject._assertEqual('m3-Pa/s'))
         self.assertEqual(c.uncert, np.sqrt((123 / 1000 / 60 * 1.2)**2 + (93 * 9.7 / 1000 / 60)**2 + 2 * 93 * 123 / 1000 / 60 * 23))
+        
+        a = variable([1, 2, 3], 'L/min', [0.1, 0.2 ,0.3])
+        b = variable([93, 97, 102], 'Pa', [1.2, 2.4, 4.7])
+        a.addCovariance(b, [2, 3, 4], 'L-Pa/min')
+        c = a * b
+        np.testing.assert_equal(c.value, [1*93, 2*97, 3*102])
+        self.assertTrue(c._unitObject._assertEqual('L-Pa/min'))
+        dcda = np.array([93, 97, 102], dtype = float)
+        dcdb = np.array([1, 2, 3], dtype = float)
+        ua = np.array([0.1, 0.2, 0.3], dtype = float)
+        ub = np.array([1.2, 2.4, 4.7], dtype = float)
+        uab = np.array([2, 3, 4], dtype = float)
+
+        uc = np.sqrt((dcda * ua)**2 + (dcdb * ub)**2 + 2 * dcda * dcdb * uab)
+        np.testing.assert_equal(c.uncert, uc)
 
     def testConvert(self):
         a = variable(1, 'km')
         b = variable(1, 'm')
         c = a * b
         c.convert('mm2')
 
@@ -1331,15 +1365,79 @@
         with self.assertRaises(Exception) as context:
             A_vec[0] = A_vec
         self.assertTrue("You can only set an element with a scalar variable" in str(context.exception))
 
         with self.assertRaises(Exception) as context:
             A[0] = B
         self.assertTrue("'scalarVariable' object does not support item assignment" in str(context.exception))
-           
+          
+        a = variable([1,2,3], 'm', [0.1, 0.2, 0.3])
+        b = a**2
+        a[1] = variable(5,'m',0.5)
+        c = b * a
+        
+        a0 = variable(1, 'm', 0.1)
+        a1 = variable(2, 'm', 0.2)
+        a2 = variable(3, 'm', 0.3)
+        b0 = a0**2
+        b1 = a1**2
+        b2 = a2**2
+        a1 = variable(5,'m', 0.5)
+        c0 = b0 * a0
+        c1 = b1 * a1
+        c2 = b2 * a2
+        
+        self.assertEqual(c[0].value, c0.value)
+        self.assertEqual(c[1].value, c1.value)
+        self.assertEqual(c[2].value, c2.value)
+        self.assertEqual(c.unit, c0.unit)
+        self.assertEqual(c[0].uncert, c0.uncert)
+        self.assertEqual(c[1].uncert, c1.uncert)
+        self.assertEqual(c[2].uncert, c2.uncert)
+        
+        
+        A = variable([1, 2, 3], 'L/min', [0.1, 0.2 ,0.3])
+        B = variable([93, 97, 102], 'Pa', [1.2, 2.4, 4.7])
+        A.addCovariance(B, [2, 3, 4], 'L-Pa/min')
+        C = A * B
+        A[1] = variable(2.5, 'L/min', 0.25)
+        C *= A
+                
+        a0 = variable(1, 'L/min', 0.1)
+        b0 = variable(93, 'Pa', 1.2)
+        a0.addCovariance(b0, 2, 'L-Pa/min')
+        c0 = a0 * b0
+        c0 *= a0
+        
+        a1 = variable(2, 'L/min', 0.2)
+        b1 = variable(97, 'Pa', 2.4)
+        a1.addCovariance(b1, 3, 'L-Pa/min')
+        c1 = a1 * b1
+        a11 = variable(2.5, 'L/min', 0.25)
+        c1 *= a11
+        
+        a2 = variable(3, 'L/min', 0.3)
+        b2 = variable(102, 'Pa', 4.7)
+        a2.addCovariance(b2, 4, 'L-Pa/min')
+        c2 = a2 * b2
+        c2 *= a2
+        
+        np.testing.assert_equal(C[0].value, c0.value)
+        self.assertTrue(C._unitObject._assertEqual(c0.unit))
+        np.testing.assert_equal(C[0].uncert, c0.uncert)
+        
+        np.testing.assert_equal(C[1].value, c1.value)
+        self.assertTrue(C._unitObject._assertEqual(c0.unit))
+        np.testing.assert_equal(C[1].uncert, c1.uncert)
+        
+        np.testing.assert_equal(C[2].value, c2.value)
+        self.assertTrue(C._unitObject._assertEqual(c0.unit))
+        np.testing.assert_equal(C[2].uncert, c2.uncert)
+
+              
     def testAppend(self):
         A = variable(12.3, 'L/min', uncert=2.6)
         B = variable(45, 'Pa', 1.2)
         A_vec = variable([12.3, 54.3, 91.3], 'L/min', uncert=[2.6, 5.4, 10.56])
 
         A_vec.append(A)
         np.testing.assert_equal(A_vec.value, [12.3, 54.3, 91.3, 12.3])
@@ -1355,14 +1453,41 @@
         self.assertEqual(A_vec.unit, 'L/min')
         np.testing.assert_equal(A_vec.uncert, [2.6, 5.4, 10.56, 2.6] * 2)
         
         with self.assertRaises(Exception) as context:
             A.append(B)
         self.assertTrue("'scalarVariable' object has no attribute 'append'" in str(context.exception))
         
+        a = variable([1, 2, 3], 'm')
+        b = variable([4, 5, 6], 'm')
+        c = variable([10, 11, 12], 'Pa')
+        d = variable([13, 14, 15], 'Pa')
+        b.addCovariance(d, [0.1, 0.2, 0.3], 'm-Pa')
+        a.append(b)
+        c.append(d) 
+        d = a * c
+
+        np.testing.assert_equal(d.value, np.array([1,2,3,4,5,6]) * np.array([10,11,12,13,14,15]))
+        self.assertTrue(d._unitObject._assertEqualStatic(d.unit, 'm-Pa'))        
+        np.testing.assert_equal(d.uncert, np.sqrt(2 * np.array([1,2,3,4,5,6]) * np.array([10,11,12,13,14,15]) * np.array([0,0,0,0.1,0.2,0.3])))
+        
+        
+        a = variable([1, 2, 3], 'm')
+        b = variable([4, 5, 6], 'm')
+        c = variable([10, 11, 12], 'Pa')
+        d = variable([13, 14, 15], 'Pa')
+        b.addCovariance(c, [0.1, 0.2, 0.3], 'm-Pa')
+        a.append(b)
+        c.append(d) 
+        d = a * c
+        np.testing.assert_equal(d.value, np.array([1,2,3,4,5,6]) * np.array([10,11,12,13,14,15]))
+        self.assertTrue(d._unitObject._assertEqualStatic(d.unit, 'm-Pa'))        
+        np.testing.assert_equal(d.uncert, np.array([0,0,0,0,0,0]))
+        
+        
     def testAddBel(self):
         a = variable(11,'dB', 0.1)
         b = variable(19,'dB',1.2)
         c = a + b
         self.assertEqual(c.value, 19.638920341433795986775635083534144311728776386508569289294)
         self.assertEqual(c.unit, 'dB')
         gradA = (10**(11/10)) / (10**(19/10) + 10**(11/10))
```

### Comparing `pyees-1.1.3/pyees/unit.py` & `pyees-1.1.4/pyees/unit.py`

 * *Files 3% similar despite different names*

```diff
@@ -285,17 +285,14 @@
                 unitType2 = [key for key, a in locals().items() if a == item][0]
         if unitType2 == '':
             raise ValueError(f'The unit {unit} was not found.')
 
         raise ValueError(f'The unit {elem} can be interpreted as a {unitType1} or a {unitType2} with the prefix {prefix}. The cannot be distiguished.')
 
 
-
-
-
 def addNewUnit(newUnit: str, scale: float, existingUnit: str, offset : float = 0):
         
     if newUnit in unitPrefixCombinations:
         raise ValueError(f'The unit {newUnit} is already known within the unit system')
     unitPrefixCombinations.append(newUnit)
     for p in knownPrefixes:
         if p+newUnit in unitPrefixCombinations:
@@ -335,17 +332,14 @@
     knownUnits[newUnit] = [SIBaseUnit, conversion]
         
     global knownCharacters
     for s in newUnit:
         knownCharacters.add(s)
 
     
-    
-    
-    
 hyphen = '-'
 slash = '/'
 integers = ['0', '1', '2', '3', '4', '5', '6', '7', '8', '9']
 
 
 class unit():
 
@@ -829,40 +823,49 @@
         
         ## output 1: are the units a logarithmic unit
         ## output 2: outputUnit
         ## output 3: scaleToSI. If true, then scale both self and other to SI and neglect output 2 and 3
         ## output 4: scaleSelf. If true then scale self to remove the prefix
         ## output 5: scaleOther. If true then scale other to remove the prefix
         
-        
+        ## determine the units of self without any prefixes and convert this to a string
         selfWithoutPrefixes = unit(unit._combineUpperAndLower(self.upper, [None] * len(self.upperPrefix), self.upperExp, self.lower, [None] * len(self.lowerPrefix), self.lowerExp))
+        selfWithoutPrefixesString = str(selfWithoutPrefixes)
+        
+        ## determine if self is a part of the logarithmic units
+        isLogarithmicUnit = selfWithoutPrefixesString in logrithmicUnits.keys()
+        
+        ## determine if self is the same as other - then no conversions are necessary
+        if unit._assertEqualStatic(str(self), str(other)):
+            return isLogarithmicUnit, str(self), False, False, False   
+        
+        ## determine the units of other without any prefixes and convert this to a string
         otherWithoutPrefixes = unit(unit._combineUpperAndLower(other.upper, [None] * len(other.upperPrefix), other.upperExp, other.lower, [None] * len(other.lowerPrefix), other.lowerExp))
-        aStr = str(selfWithoutPrefixes)
-        bStr = str(otherWithoutPrefixes)
+        otherWithoutPrefixesString = str(otherWithoutPrefixes)
         
-        isLogarithmicUnit = aStr in logrithmicUnits.keys()
-                
-        scaleSelf = str(self) != aStr
-        scaleOther = str(other) != bStr
+        ## determine if self and/or other has to be scaled in order to remove any prefixes
+        scaleSelf = str(self) != selfWithoutPrefixesString
+        scaleOther = str(other) != otherWithoutPrefixesString
         
-        if unit._assertEqualStatic(aStr, bStr):
-            return isLogarithmicUnit, aStr, False, scaleSelf, scaleOther
+        ## determine if the self and other are identical once any prefixes has been removed
+        if unit._assertEqualStatic(selfWithoutPrefixesString, otherWithoutPrefixesString):
+            return isLogarithmicUnit, selfWithoutPrefixesString, False, scaleSelf, scaleOther
         
-        # test if the SI base units are identical
+        # determine if the SI base units of self and other are equal
         if self._SIBaseUnit == other._SIBaseUnit:
             return isLogarithmicUnit, self._SIBaseUnit, True, False, False
         
-        
+        ## determine if "DELTAK" and "K" are the SI Baseunits of self and other
         SIBaseUnits = [selfWithoutPrefixes._SIBaseUnit,  otherWithoutPrefixes._SIBaseUnit]        
         if 'DELTAK' in SIBaseUnits and 'K' in SIBaseUnits:
             
             indexTemp = SIBaseUnits.index('K')
             indexDiff = 0 if indexTemp == 1 else 1
             
-            units = [aStr, bStr]
+            units = [selfWithoutPrefixesString, otherWithoutPrefixesString]
 
             if units[indexTemp] == units[indexDiff][-1]:        
                 return isLogarithmicUnit, units[indexTemp], False, scaleSelf, scaleOther
             
             return isLogarithmicUnit, 'K', True, False, False
 
         raise ValueError(f'You tried to add a variable in [{self}] to a variable in [{other}], but the units do not have the same SI base unit')
@@ -870,49 +873,59 @@
     def __sub__(self, other):
         ## output 1: are the units a logarithmic unit
         ## output 2: outputUnit
         ## output 3: scaleToSI. If true, then scale both self and other to SI and neglect output 2 and 3
         ## output 4: scaleSelf. If true then scale self to remove the prefix
         ## output 5: scaleOther. If true then scale other to remove the prefix
         
-        
+        ## determine the units of self without any prefixes and convert this to a string
         selfWithoutPrefixes = unit(unit._combineUpperAndLower(self.upper, [None] * len(self.upperPrefix), self.upperExp, self.lower, [None] * len(self.lowerPrefix), self.lowerExp))
+        selfWithoutPrefixesString = str(selfWithoutPrefixes)
+        
+        ## determine if self is a part of the logarithmic units
+        isLogarithmicUnit = selfWithoutPrefixesString in logrithmicUnits.keys()
+        
+        ## determine the units of other without any prefixes and convert this to a string
         otherWithoutPrefixes = unit(unit._combineUpperAndLower(other.upper, [None] * len(other.upperPrefix), other.upperExp, other.lower, [None] * len(other.lowerPrefix), other.lowerExp))
-        aStr = str(selfWithoutPrefixes)
-        bStr = str(otherWithoutPrefixes)
+        otherWithoutPrefixesString = str(otherWithoutPrefixes)
         
-        isLogarithmicUnit = aStr in logrithmicUnits.keys()
-                
-        scaleSelf = str(self) != aStr
-        scaleOther = str(other) != bStr
+        ## determine if self and/or other has to be scaled in order to remove any prefixes
+        scaleSelf = str(self) != selfWithoutPrefixesString
+        scaleOther = str(other) != otherWithoutPrefixesString
 
+        ## determine if "DELTAK" and "K" are the SI Baseunits of self and other
         SIBaseUnits = [self._SIBaseUnit, other._SIBaseUnit]
         if SIBaseUnits[0] == 'K' and SIBaseUnits[1] == 'K':
-            if self._assertEqual(other):
+            if selfWithoutPrefixesString == otherWithoutPrefixesString:
                 return isLogarithmicUnit, 'DELTA' + str(self), False, scaleSelf, scaleOther
             return isLogarithmicUnit,'DELTAK', True, False, False
 
         if 'DELTAK' in SIBaseUnits and 'K' in SIBaseUnits:
-
             
             indexTemp = SIBaseUnits.index('K')
             if indexTemp != 0:
                 raise ValueError('You tried to subtract a temperature from a temperature differnce. This is not possible.')
             indexDiff = 0 if indexTemp == 1 else 1
             
-            units = [aStr, bStr]
+            units = [selfWithoutPrefixesString, otherWithoutPrefixesString]
 
 
             if units[indexTemp] == units[indexDiff][-1]:        
                 return isLogarithmicUnit, units[indexTemp], False, scaleSelf, scaleOther
             
             return isLogarithmicUnit, 'K', True, False, False
         
-        if unit._assertEqualStatic(aStr, bStr):
-            return isLogarithmicUnit, aStr, False, scaleSelf, scaleOther
+                
+        ## determine if self is the same as other - then no conversions are necessary
+        if unit._assertEqualStatic(str(self), str(other)):
+            return isLogarithmicUnit, str(self), False, False, False
+           
+        ## determine if the self and other are identical once any prefixes has been removed
+        if unit._assertEqualStatic(selfWithoutPrefixesString, otherWithoutPrefixesString):
+            return isLogarithmicUnit, selfWithoutPrefixesString, False, scaleSelf, scaleOther
         
         # test if the SI base units are identical
         if self._SIBaseUnit == other._SIBaseUnit:
             return isLogarithmicUnit, self._SIBaseUnit, True, False, False
         
         
         
@@ -1081,13 +1094,18 @@
         # create the unit string
         self.unitStr = self._createUnitString()
 
         self._SIBaseUnit = self._getSIBaseUnit(self.upper, self.upperExp, self.lower, self.lowerExp)
         otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp = self._getLists(self._SIBaseUnit)
         self._converterToSI = self._getConverter(otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
+    a = unit('C')
+    b = unit('C')
+    print(a - b, 'DELTAC')
+    
+    a = unit('J/kg-DELTAK')
+    b = unit('J/kg-DELTAK')
+    print(a - b, 'J/kg-DELTAK')
     
-    a = unit('J-L-DELTAC/K-m3-min')
-    a.getConverter('kW')
-    print(a)
```

### Comparing `pyees-1.1.3/pyees/variable.py` & `pyees-1.1.4/pyees/variable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from copy import deepcopy
+from copy import copy
 import numpy as np
 try:
     from unit import unit
     from unit import logrithmicUnits
 except ImportError:
     from pyees.unit import unit
     from pyees.unit import logrithmicUnits
@@ -90,34 +90,32 @@
         c._unitStr = aUnitWithoutPrefix
         c._unitObject = unit(aUnitWithoutPrefix)
         c.convert(aUnit)
 
         return c
    
 class scalarVariable():
-    def __init__(self, value, unitStr, uncert, nDigits) -> None:
+    def __init__(self, value, unitObject : str | unit, uncert, nDigits) -> None:
         
         self._value = value
         self._uncert = uncert
 
         # create a unit object
-        self._unitObject = unitStr if isinstance(unitStr, unit) else unit(unitStr)
+        self._unitObject = unitObject if isinstance(unitObject, unit) else unit(unitObject)
 
         # number of digits to show
         self.nDigits = nDigits
 
-        # value and unit in SI. This is used when determining the gradient in the uncertanty expression
-        self._getConverterToSI()
-
         # uncertanty
         self.dependsOn = {}
         self.covariance = {}
 
-    def _getConverterToSI(self):
-        self._converterToSI = self._unitObject._converterToSI
+    @property
+    def _converterToSI(self):
+        return self._unitObject._converterToSI
 
     @property
     def value(self):
         return self._value
 
     @property
     def unit(self):
@@ -128,17 +126,14 @@
         return self._uncert
 
     def convert(self, newUnit):
         converter = self._unitObject.getConverter(newUnit)
         self._value = converter.convert(self._value, useOffset=not self._unitObject.isCombinationUnit())
         self._uncert = converter.convert(self._uncert, useOffset=False)
         self._unitObject.convert(newUnit)
-
-        # update the converter to SI
-        self._getConverterToSI()
  
     def printUncertanty(self, value, uncert):
         # function to print number
         if uncert == 0 or uncert is None or np.isnan(uncert):
             return f'{value:.{self.nDigits}g}', None
 
         digitsUncert = -int(np.floor(np.log10(np.abs(uncert))))
@@ -199,72 +194,95 @@
 
         value, uncert = self.printUncertanty(value, uncert)
         if uncert is None:
             return rf'{value}{space}{unitStr}'
         else:
                 return rf'{value} {pm} {uncert}{space}{unitStr}'
 
-    def _addDependents(self, vars, grads):
-        # copy the gradients
-        # this prevents a pointer error as the gradients often are set to the value of a variable
-        # when the gradients are scaled this causes problems
-        grads = [deepcopy(elem) for elem in grads]
-
-        # loop over the variables and their gradients
-        for var, grad in zip(vars, grads):
-            # scale the gradient to SI units. This is necessary if one of the variables are converted after the dependency has been noted
-            scale = self._converterToSI.convert(1, useOffset=False) / var._converterToSI.convert(1, useOffset=False)
-            grad *= scale
-
-            # check if the variable depends on other variables
-            if var.dependsOn:
-
-                # loop over the dependencies of the variables and add them to the dependencies of self.
-                # this ensures that the product rule is used
-                for key, item in var.dependsOn.items():
-                    if key in self.dependsOn:
-                        self.dependsOn[key] += item * grad
-                    else:
-                        self.dependsOn[key] = item * grad
-            else:
-
-                # the variable did not have any dependecies. Therefore the the varaible is added to the dependencies of self
-                if var in self.dependsOn:
-                    self.dependsOn[var] += grad
+    def _addDependent(self, var, grad):
+        # scale the gradient to SI units. This is necessary if one of the variables are converted after the dependency has been noted
+        grad *= self._converterToSI.convert(1, useOffset=False) / var._converterToSI.convert(1, useOffset=False)
+        
+        if var.dependsOn:
+            # the variable depends on other variables
+            # loop over the dependencies of the variables and add them to the dependencies of self.
+            # this ensures that the product rule is used
+            for vvar, dependency in var.dependsOn.items():
+                if not vvar in self.dependsOn:
+                    unc = vvar._converterToSI.convert(vvar.uncert, useOffset = False)
+                    self.dependsOn[vvar] = [unc, grad * dependency[1]]
                 else:
-                    self.dependsOn[var] = grad
+                    self.dependsOn[vvar][1] += grad * dependency[1]
+        else:    
+            ## the variable does not depend on other variables
+            ## add the variable to the dependencies of self
+            if not var in self.dependsOn:
+                unc = var._converterToSI.convert(var.uncert, useOffset = False)
+                self.dependsOn[var] = [unc, grad]
+            else:
+                self.dependsOn[var][1] += grad
 
-    def _addCovariance(self, var, covariance):
-        self.covariance[var] = covariance
+    def __iter__(self):
+        self.n = 0
+        return self
 
+    def __next__(self):
+        if self.n == 0:
+            self.n += 1
+            return self
+        raise StopIteration           
+   
+    def addCovariance(self, var, covariance: float, unitStr: str):
+        try:
+            float(covariance)
+        except TypeError:
+            raise ValueError(f'You tried to set the covariance between {self} and {var} with a non scalar value')
+        
+        covUnit = unit(unitStr)
+        selfVarUnit = unit(self._unitObject * var._unitObject)
+        if not unit._assertEqualStatic(covUnit._SIBaseUnit, selfVarUnit._SIBaseUnit):
+            raise ValueError(f'The covariance of {covariance} [{unitStr}] does not match the units of {self} and {var}')
+        
+        covariance = covUnit._converterToSI.convert(covariance, useOffset=False)
+        
+        self.covariance[var] = covariance        
+        var.covariance[self] = covariance
+        
     def _calculateUncertanty(self):
-
+ 
         # variance from each measurement
         variance = 0
-        selfScaleToSI = self._converterToSI.convert(1, useOffset=False)
-        for var, grad in self.dependsOn.items():
-            # the gradient is scaled with the inverse of the conversion of the unit to SI units.
-            # This is necessary if the variable "var" has been converted after the dependency has been noted
-            scale = var._converterToSI.convert(1, useOffset=False) / selfScaleToSI           
-            variance += (grad * scale * var.uncert)**2
 
+        # loop over each different variable object in the dependency dict
+        for dependency in self.dependsOn.values():
+            
+            ## loop over each "instance" of the variable
+            ## an instance occurs when the variable has been changed using methods as __setitem__
+            ## this affectively makes the variable a "new" variable in the eyes of other variables
+    
+            ## add the variance constribution to the variance
+            unc, grad = dependency[0], dependency[1]
+            variance += (unc * grad) ** 2
+        
+        ## scale the variance back in to the currenct unit
+        ## the scaling is raised to a power of 2, as the above line should be
+        ## variance += (scale * unc * grad) ** 2
+        scale = 1 / self._converterToSI.convert(1, useOffset=False)
+        variance *= scale ** 2
+        
         # variance from the corralation between measurements
-        n = len(self.dependsOn.keys())
-        for i in range(n):
-            var_i = list(self.dependsOn.keys())[i]
-            for j in range(i + 1, n):
-                var_j = list(self.dependsOn.keys())[j]
-                if var_j in var_i.covariance.keys():
-                    if not var_i in var_j.covariance.keys():
-                        raise ValueError(
-                            f'The variable {var_i} is correlated with the varaible {var_j}. However the variable {var_j} not not correlated with the variable {var_i}. Something is wrong.')
-                    scale_i = var_i._converterToSI.convert(1, useOffset=False) / selfScaleToSI
-                    scale_j = var_j._converterToSI.convert(1, useOffset=False) / selfScaleToSI
-                    varianceContribution = 2 * scale_i * self.dependsOn[var_i] * scale_j * self.dependsOn[var_j] * var_i.covariance[var_j][0]
-                    variance += varianceContribution
+        ## covariance = list(vari, vari.currentValue, vari.currentUncert, varj, varj.currentValue, varj.currenctUncert, cov)
+        ## from the above the gradients can be found from self.dependsOn
+        
+        for var1 in self.dependsOn.keys():
+            for var2 in var1.covariance.keys():
+                if var2 in self.dependsOn:
+                    grad1 = self.dependsOn[var1][1]
+                    grad2 = self.dependsOn[var2][1]
+                    variance += scale**2 * grad1 * grad2 * var1.covariance[var2]
 
         self._uncert = np.sqrt(variance)
         
     def __add__(self, other):
         
         if not isinstance(other, scalarVariable):
             return self + variable(other, self.unit)
@@ -272,37 +290,36 @@
         # determine if the two variable can be added
         isLogarithmicUnit, outputUnit, scaleToSI, scaleSelf, scaleOther = self._unitObject + other._unitObject
 
         if isLogarithmicUnit:
             return logarithmicVariables.__add__(self, other)
 
         # convert self and other to the SI unit system
-        selfUnit = deepcopy(self.unit)
-        otherUnit = deepcopy(other.unit)
+        selfUnit = copy(self.unit)
+        otherUnit = copy(other.unit)
         
         if scaleToSI:
             self.convert(self._unitObject._SIBaseUnit)
             other.convert(other._unitObject._SIBaseUnit)
         else:
             if scaleSelf:
                 a, _ = self._unitObject._removePrefixFromUnit(self.unit)
                 self.convert(a)
             if scaleOther:
                 a, _ = other._unitObject._removePrefixFromUnit(other.unit)
                 other.convert(a)
         
 
         # determine the value and gradients
-        val = self._value + other._value
-        grad = [1, 1]
-        vars = [self, other]
+        val = self.value + other.value
         
         # create the new variable
         var = variable(val, outputUnit)
-        var._addDependents(vars, grad)
+        var._addDependent(self, 1)
+        var._addDependent(other, 1)
         var._calculateUncertanty()
 
         # convert all units back to their original units
         self.convert(selfUnit)
         other.convert(otherUnit)
         
         ## convert the variable in to the original unit if self and other has the same original unit
@@ -326,35 +343,35 @@
         # determine if the variables can be subtracted
         isLogarithmicUnit, outputUnit, scaleToSI, scaleSelf, scaleOther = self._unitObject - other._unitObject
 
         if isLogarithmicUnit:
             return logarithmicVariables.__sub__(self, other)
 
         # convert self and other to the SI unit system
-        selfUnit = deepcopy(self.unit)
-        otherUnit = deepcopy(other.unit)
+        selfUnit = copy(self.unit)
+        otherUnit = copy(other.unit)
  
         if scaleToSI:
             self.convert(self._unitObject._SIBaseUnit)
             other.convert(other._unitObject._SIBaseUnit)
         else:
             if scaleSelf:
                 a, _ = self._unitObject._removePrefixFromUnit(self.unit)
                 self.convert(a)
             if scaleOther:
                 a, _ = other._unitObject._removePrefixFromUnit(other.unit)
                 other.convert(a)
 
         # determine the value and gradients
         val = self.value - other.value
-        grad = [1, -1]
-        vars = [self, other]
+
         # create the new variable
         var = variable(val, outputUnit)
-        var._addDependents(vars, grad)
+        var._addDependent(self, 1)
+        var._addDependent(other, -1)
         var._calculateUncertanty()
 
 
         # convert self and other back
         self.convert(selfUnit)
         other.convert(otherUnit)
 
@@ -366,26 +383,24 @@
                 var.convert([selfUnit, otherUnit][SIBaseUnits.index('K')]) 
         return var
 
     def __rsub__(self, other):
         return - self + other
 
     def __mul__(self, other):
-
+    
         if not isinstance(other, scalarVariable):
             return self * variable(other)
 
         val = self.value * other.value
         outputUnit = self._unitObject * other._unitObject
 
-        grad = [other._value, self._value]
-        vars = [self, other]
-
         var = variable(val, outputUnit)
-        var._addDependents(vars, grad)
+        var._addDependent(self, other.value)
+        var._addDependent(other, self.value)
         var._calculateUncertanty()
 
         if var._unitObject._SIBaseUnit == '1' and var._unitObject != '1':
             var.convert('1')
 
         return var
 
@@ -395,80 +410,75 @@
     def __pow__(self, other):
         if not isinstance(other, scalarVariable):
             return self ** variable(other, '')
 
         if str(other.unit) != '1':
             raise ValueError('The exponent can not have a unit')
 
-        selfUnit = deepcopy(self.unit)
+        selfUnit = copy(self.unit)
         outputUnit, hasToBeScaledToSI = self._unitObject ** other.value
 
         if hasToBeScaledToSI:
             self.convert(self._unitObject._SIBaseUnit)
         
-        val = self._value ** other.value
+        val = self.value ** other.value
 
         def gradSelf(valSelf, valOTher):
             if valSelf != 0:
                 return  valOTher * valSelf ** (valOTher - 1)
             return 0
         
         def gradOther(valSelf, valOther, uncertOther):
             if uncertOther != 0:
                 return valSelf ** valOther * np.log(valSelf)
             return 0
         
-        gradOther = np.vectorize(gradOther, otypes=[float])(self._value, other._value, other._uncert)
-        gradSelf = np.vectorize(gradSelf, otypes=[float])(self._value, other._value)
-        grad = [gradSelf, gradOther]
-        vars = [self, other]
-                
+        gradOther = np.vectorize(gradOther, otypes=[float])(self.value, other.value, other._uncert)
+        gradSelf = np.vectorize(gradSelf, otypes=[float])(self.value, other.value)
+        
         var = variable(val, outputUnit)
-        var._addDependents(vars, grad)
+        var._addDependent(self, gradSelf)
+        var._addDependent(other, gradOther)
         var._calculateUncertanty()
         
         if hasToBeScaledToSI:
             self.convert(selfUnit)
         
         return var
 
     def __rpow__(self, other):
         return variable(other, '1') ** self
 
     def __truediv__(self, other):
         if not isinstance(other, scalarVariable):
             return self / variable(other)
 
-        val = self._value / other._value
+        val = self.value / other.value
         outputUnit = self._unitObject / other._unitObject
 
-        grad = [1 / other._value, -self._value / (other._value**2)]
-        vars = [self, other]
-        
         var = variable(val, outputUnit)
-        var._addDependents(vars, grad)
+        var._addDependent(self, 1 / other.value)
+        var._addDependent(other, -self.value / (other.value**2))
         var._calculateUncertanty()
 
         if var._unitObject._SIBaseUnit == '1' and var._unitObject != '1':
             var.convert('1')
 
         return var
 
     def __rtruediv__(self, other):
         if not isinstance(other, scalarVariable):
             return variable(other) / self
 
-        val = other._value / self._value
+        val = other.value / self.value
         outputUnit = other._unitObject / self._unitObject
-
-        grad = [-other._value / (self._value**2), 1 / (self._value)]
-        vars = [self, other]
-
+        
         var = variable(val, outputUnit)
-        var._addDependents(vars, grad)
+        var._addDependent(self, -other.value / (self.value**2))
+        var._addDependent(other, 1 / (self.value))
         var._calculateUncertanty()
 
         if var._unitObject._SIBaseUnit == '1' and var._unitObject != '1':
             var.convert('1')
 
         return var
 
@@ -477,33 +487,27 @@
 
     def log(self):
         if self.unit != '1':
             raise ValueError('You can only take the natural log of a variable if it has no unit')
 
         val = np.log(self.value)
 
-        vars = [self]
-        grad = [1 / self.value]
-
         var = variable(val, '1')
-        var._addDependents(vars, grad)
+        var._addDependent(self, 1 / self.value)
         var._calculateUncertanty()
 
         return var
 
     def log10(self):
         if self.unit != '1':
             raise ValueError('You can only take the base 10 log of a variable if it has no unit')
         val = np.log10(self.value)
 
-        vars = [self]
-        grad = [1 / (self.value * np.log10(self.value))]
-
         var = variable(val, '1')
-        var._addDependents(vars, grad)
+        var._addDependent(self, 1 / (self.value * np.log10(self.value)))
         var._calculateUncertanty()
 
         return var
 
     def exp(self):
         return np.e**self
 
@@ -513,63 +517,57 @@
     def sin(self):
         if str(self._unitObject._SIBaseUnit) != 'rad':
             raise ValueError('You can only take sin of an angle')
         
         outputUnit = '1'
         if self._unitObject._assertEqual('rad'):
             val = np.sin(self.value)
-            grad = [np.cos(self.value)]
+            grad = np.cos(self.value)
         else:
             val = np.sin(np.pi / 180 * self.value)
-            grad = [np.pi / 180 * np.cos(np.pi / 180 * self.value)]
+            grad = np.pi / 180 * np.cos(np.pi / 180 * self.value)
         
-        vars = [self]
-
         var = variable(val, outputUnit)
-        var._addDependents(vars, grad)
+        var._addDependent(self, grad)
         var._calculateUncertanty()
 
         return var
 
     def cos(self):
         if str(self._unitObject._SIBaseUnit) != 'rad':
             raise ValueError('You can only take cos of an angle')
 
         outputUnit = '1'
         if self.unit == 'rad':
             val = np.cos(self.value)
-            grad = [-np.sin(self.value)]
+            grad = -np.sin(self.value)
         else:
             val = np.cos(np.pi / 180 * self.value)
-            grad = [-np.pi / 180 * np.sin(np.pi / 180 * self.value)]
-
-        vars = [self]
-
+            grad = -np.pi / 180 * np.sin(np.pi / 180 * self.value)
+            
         var = variable(val, outputUnit)
-        var._addDependents(vars, grad)
+        var._addDependent(self, grad)
         var._calculateUncertanty()
 
         return var
 
     def tan(self):
         if str(self._unitObject._SIBaseUnit) != 'rad':
             raise ValueError('You can only take tan of an angle')
 
         outputUnit = '1'
         if self.unit == 'rad':
             val = np.tan(self.value)
-            grad = [2 / (np.cos(2 * self.value) + 1)]
+            grad = 2 / (np.cos(2 * self.value) + 1)
         else:
             val = np.tan(np.pi / 180 * self.value)
-            grad = [np.pi / (90 * (np.cos(np.pi / 90 * self.value) + 1))]
-
-        vars = [self]
+            grad = np.pi / (90 * (np.cos(np.pi / 90 * self.value) + 1))
 
         var = variable(val, outputUnit)
-        var._addDependents(vars, grad)
+        var._addDependent(self, grad)
         var._calculateUncertanty()
 
         return var
 
     def __abs__(self):
         return variable(np.abs(self.value), self.unit, self.uncert)
 
@@ -581,28 +579,30 @@
                 return self.min()
             case np.mean:
                 return self.mean()
         raise NotImplementedError()
     
     def max(self):
         return self
+    
     def min(self):
         return self
+    
     def mean(self):
         return self
 
     def __lt__(self, other):
         if not isinstance(other, scalarVariable):
             return self < variable(other, self.unit)
 
         if not self._unitObject._SIBaseUnit == other._unitObject._SIBaseUnit:
             raise ValueError(f'You cannot compare {self} and {other} as they do not have the same SI base unit')
         
-        selfUnit = deepcopy(self.unit)
-        otherUnit = deepcopy(other.unit)
+        selfUnit = copy(self.unit)
+        otherUnit = copy(other.unit)
         
         self.convert(self._unitObject._SIBaseUnit)
         other.convert(self._unitObject._SIBaseUnit)
 
         out = self.value < other.value
         
         self.convert(selfUnit)
@@ -611,16 +611,16 @@
 
     def __le__(self, other):
         if not isinstance(other, scalarVariable):
             return self <= variable(other, self.unit)
         if not self._unitObject._SIBaseUnit == other._unitObject._SIBaseUnit:
             raise ValueError(f'You cannot compare {self} and {other} as they do not have the same SI base unit')
         
-        selfUnit = deepcopy(self.unit)
-        otherUnit = deepcopy(other.unit)
+        selfUnit = copy(self.unit)
+        otherUnit = copy(other.unit)
         
         self.convert(self._unitObject._SIBaseUnit)
         other.convert(self._unitObject._SIBaseUnit)
         
         out = self.value <= other.value
         
         self.convert(selfUnit)
@@ -630,16 +630,16 @@
     def __gt__(self, other):
         if not isinstance(other, scalarVariable):
             return self > variable(other, self.unit)
 
         if not self._unitObject._SIBaseUnit == other._unitObject._SIBaseUnit:
             raise ValueError(f'You cannot compare {self} and {other} as they do not have the same SI base unit')
         
-        selfUnit = deepcopy(self.unit)
-        otherUnit = deepcopy(other.unit)
+        selfUnit = copy(self.unit)
+        otherUnit = copy(other.unit)
         
         self.convert(self._unitObject._SIBaseUnit)
         other.convert(self._unitObject._SIBaseUnit)
 
         out = self.value > other.value
            
         self.convert(selfUnit)
@@ -649,16 +649,16 @@
     def __ge__(self, other):
         if not isinstance(other, scalarVariable):
             return self >= variable(other, self.unit)
 
         if not self._unitObject._SIBaseUnit == other._unitObject._SIBaseUnit:
             raise ValueError(f'You cannot compare {self} and {other} as they do not have the same SI base unit')
         
-        selfUnit = deepcopy(self.unit)
-        otherUnit = deepcopy(other.unit)
+        selfUnit = copy(self.unit)
+        otherUnit = copy(other.unit)
         
         self.convert(self._unitObject._SIBaseUnit)
         other.convert(self._unitObject._SIBaseUnit)
 
         out = self.value >= other.value
         
         self.convert(selfUnit)
@@ -668,16 +668,16 @@
     def __eq__(self, other):
         if not isinstance(other, scalarVariable):
             return self == variable(other, self.unit)
 
         if not self._unitObject._SIBaseUnit == other._unitObject._SIBaseUnit:
             raise ValueError(f'You cannot compare {self} and {other} as they do not have the same SI base unit')
         
-        selfUnit = deepcopy(self.unit)
-        otherUnit = deepcopy(other.unit)
+        selfUnit = copy(self.unit)
+        otherUnit = copy(other.unit)
         
         self.convert(self._unitObject._SIBaseUnit)
         other.convert(self._unitObject._SIBaseUnit)
         
         if isinstance(self, arrayVariable) and isinstance(other, arrayVariable):
             if len(self) != len(other):
                 raise ValueError(f"operands could not be broadcast together with shapes {self.value.shape} {other.value.shape}")    
@@ -690,16 +690,16 @@
     def __ne__(self, other):
         if not isinstance(other, scalarVariable):
             return self != variable(other, self.unit)
 
         if not self._unitObject._SIBaseUnit == other._unitObject._SIBaseUnit:
             raise ValueError(f'You cannot compare {self} and {other} as they do not have the same SI base unit')
         
-        selfUnit = deepcopy(self.unit)
-        otherUnit = deepcopy(other.unit)
+        selfUnit = copy(self.unit)
+        otherUnit = copy(other.unit)
         
         self.convert(self._unitObject._SIBaseUnit)
         other.convert(self._unitObject._SIBaseUnit)
 
         if isinstance(self, arrayVariable) and isinstance(other, arrayVariable):
             if len(self) != len(other):
                 raise ValueError(f"operands could not be broadcast together with shapes {self.value.shape} {other.value.shape}")    
@@ -708,52 +708,119 @@
         self.convert(selfUnit)
         other.convert(otherUnit)
         return out
 
     def __hash__(self):
         return id(self)
 
-   
+
 class arrayVariable(scalarVariable):
-   
+    
+    def __init__(self, value, unitStr, uncert, nDigits) -> None:
+        self.nDigits = nDigits
+        
+        # create a unit object
+        self._unitObject = unitStr if isinstance(unitStr, unit) else unit(unitStr)        
+        
+        self.scalarVariables = []
+        if not value is None:
+            for v, u in zip(value, uncert):
+                self.scalarVariables.append(scalarVariable(v, self._unitObject, u, nDigits))
+    
+    def _calculateUncertanty(self):
+        for elem in self.scalarVariables:
+            elem._calculateUncertanty()
+    
+    def addCovariance(self, var, grad: np.ndarray, unitStr: str):
+        for elem, varElem, gradElem in zip(self.scalarVariables, var, grad):
+            elem.addCovariance(varElem, gradElem, unitStr)
+    
+    def _addDependent(self, var, grad):
+        isArrayVariable = isinstance(var, arrayVariable)
+        isArrayGradient = isinstance(grad, list) or isinstance(grad, np.ndarray)
+        
+        for i, elem in enumerate(self.scalarVariables):
+            v = var[i] if isArrayVariable else var
+            g = grad[i] if isArrayGradient else grad
+            elem._addDependent(v, g)
+                        
     def __len__(self):
-        return len(self._value)
+        return len(self.scalarVariables)
 
     def __getitem__(self, index):
-        if isinstance(index, int) or isinstance(index, slice):
-            if index >= len(self):
-                raise IndexError('Index out of bounds')
-            if len(self) == 1:
-                if index != 0:
-                    raise IndexError('Index out of bound')
-                return variable(self.value, self._unitObject, self.uncert)
-            return variable(self.value[index], self._unitObject, self.uncert[index])
-        else:
-            val = [self.value[elem]for elem in index]
-            unc = [self.uncert[elem]for elem in index]
-            return variable(val, self._unitObject, unc)
+        
+        if isinstance(index, int):
+            return self.scalarVariables[index]
+        elif isinstance(index, slice):
+            vals = [elem.value for elem in self.scalarVariables[index]]
+            unc = [elem.uncert for elem in self.scalarVariables[index]]
+            return variable(vals, self._unitObject, unc, self.nDigits)
+        else:
+            raise NotImplementedError()
+ 
+    @property
+    def value(self):
+        return np.array([elem.value for elem in self.scalarVariables])       
+ 
+    @property
+    def uncert(self):
+        return np.array([elem.uncert for elem in self.scalarVariables])       
  
     def __setitem__(self, i, elem):
         if (type(elem) != scalarVariable):
             raise ValueError(f'You can only set an element with a scalar variable')
         if (elem.unit != self.unit):
             raise ValueError(f'You can not set an element of {self} with {elem} as they do not have the same unit')
-        self._value[i] = elem.value
-        self._uncert[i] = elem.uncert
-    
+        
+        self.scalarVariables[i] = elem
+   
     def append(self, elem):
-        if not (isinstance(elem, scalarVariable)):
-            raise ValueError(f'You can only set an element with a variable')
+        
         if (elem.unit != self.unit):
             raise ValueError(f'You can not set an element of {self} with {elem} as they do not have the same unit')
-        
-        self._value = np.append(self._value, elem.value)
-        self._uncert = np.append(self._uncert, elem.uncert)
-    
+
+        if isinstance(elem, arrayVariable):
+            elemsToAppend = [e for e in elem]
+            for e in elemsToAppend:
+                self.scalarVariables.append(e)
+        else:
+            self.scalarVariables.append(elem) 
        
+    def printUncertanty(self, value, uncert):
+        # function to print number
+        if uncert == 0 or uncert is None or np.isnan(uncert):
+            return f'{value:.{self.nDigits}g}', 0
+
+        digitsUncert = -int(np.floor(np.log10(np.abs(uncert))))
+
+        if value != 0:
+            digitsValue = -int(np.floor(np.log10(np.abs(value))))
+        else:
+            digitsValue = 0
+
+        # uncertanty
+        if digitsUncert > 0:
+            uncert = f'{uncert:.{1}g}'
+        else:
+            nDecimals = len(str(int(uncert)))
+            uncert = int(np.around(uncert, -nDecimals + 1))
+
+        # value
+        if digitsValue <= digitsUncert:
+            if digitsUncert > 0:
+                value = f'{value:.{digitsUncert}f}'
+            else:
+                value = int(np.around(value, - nDecimals + 1))
+        else:
+            value = '0'
+            if digitsUncert > 0:
+                value += '.' + ''.join(['0'] * digitsUncert)
+
+        return value, uncert 
+    
     def __str__(self, pretty=None) -> str:
         unitStr = self._unitObject.__str__(pretty=pretty)
 
         if pretty:
             pm = r'\pm'
             space = r'\ '
             squareBracketLeft = r'\left ['
@@ -774,15 +841,15 @@
         valStr = []
         uncStr = []
         for v, u in zip(self.value, self.uncert):
             v, u = self.printUncertanty(v, u)
             valStr.append(v)
             uncStr.append(u)
 
-        if all(self._uncert == 0) or all(elem is None for elem in self._uncert):
+        if all(self.uncert == 0) or all(elem is None for elem in self.uncert):
             out = rf''
             out += rf'['
             for i, elem in enumerate(valStr):
                 out += rf'{elem}'
                 if i != len(valStr) - 1:
                     out += rf', '
             out += rf']'
@@ -816,15 +883,18 @@
             if len(self) != len(other):
                 raise ValueError(f'operands could not be broadcast together with shapes {self.value.shape} {other.value.shape}')
             out = [a**b for a,b in zip(self, other)]
         else:
             out = [a**other for a in self]
 
         if all([out[0].unit == elem.unit for elem in out]):
-            return variable([elem.value for elem in out], out[0].unit, [elem.uncert for elem in out])
+            oout = arrayVariable(None, out[0].unit, None, out[0].nDigits)
+            for o in out:
+                oout.append(o)
+            return oout
         
         return out
      
     def __rpow__(self,other):
         if not (isinstance(other, scalarVariable) or isinstance(other, arrayVariable)):
             return variable(other) ** self
     
@@ -863,31 +933,43 @@
 
     def max(self):
         index = np.argmax(self.value)
         return variable(self.value[index], self.unit, self.uncert[index])
     
     def mean(self):
         return sum(self) / len(self)
+    
+    def convert(self, newUnit):
+        converter = self._unitObject.getConverter(newUnit)
+        for elem in self.scalarVariables:
+            elem._value = converter.convert(elem._value, useOffset=not self._unitObject.isCombinationUnit())
+            elem._uncert = converter.convert(elem._uncert, useOffset=False)
+        self._unitObject.convert(newUnit)
 
+    def __iter__(self):
+        self.n = 0
+        return self
 
+    def __next__(self):
+        if self.n < len(self):
+            out = self.scalarVariables[self.n]
+            self.n += 1
+            return out
 
+        raise StopIteration
 
 def variable(value, unit = '', uncert = None, nDigits = 3):
     # store the value and the uncertaty
     def evaluateInput(input):
         if input is None:
             return input
         if isinstance(input, np.ndarray):
-            if len(input) == 1:
-                return input[0]
             return input
         else:
             if isinstance(input, list):
-                if len(input) == 1:
-                    return input[0]
                 return np.array(input, dtype=float)
             else:
                 return float(input)
                 
     value = evaluateInput(value)
     uncert = evaluateInput(uncert)
     
@@ -907,7 +989,15 @@
                 raise ValueError('The lenght of the value has to be equal to the lenght of the uncertanty')      
     
     if isinstance(value, np.ndarray):
         return arrayVariable(value, unit, uncert, nDigits)
     else:
         return scalarVariable(value, unit, uncert, nDigits)
 
+
+if __name__ == "__main__":
+    a = variable(1,'J/kg-DELTAK')
+    b = variable(1,'J/kg-DELTAK')
+    c = a + b
+    
+    
+
```

### Comparing `pyees-1.1.3/pyees.egg-info/PKG-INFO` & `pyees-1.1.4/pyees.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.1.3
+Version: 1.1.4
 Summary: EES but for python
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.1.3/setup.py` & `pyees-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.1.3',
+    version='1.1.4',
     license='MIT',
     description='EES but for python',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

