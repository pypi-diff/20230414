# Comparing `tmp/pyees-1.1.4.tar.gz` & `tmp/pyees-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyees-1.1.4.tar", last modified: Fri Apr 14 07:49:40 2023, max compression
+gzip compressed data, was "pyees-1.1.5.tar", last modified: Fri Apr 14 08:24:40 2023, max compression
```

## Comparing `pyees-1.1.4.tar` & `pyees-1.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 07:49:21.165818 pyees-1.1.4/
--rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0      616 2023-04-14 07:49:21.181443 pyees-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 07:49:20.931442 pyees-1.1.4/pyees/
--rw-rw-rw-   0        0        0      619 2023-03-30 05:48:48.000000 pyees-1.1.4/pyees/__init__.py
--rw-rw-rw-   0        0        0    15688 2023-03-11 13:10:44.000000 pyees-1.1.4/pyees/fit.py
--rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.1.4/pyees/profilePyees.py
--rw-rw-rw-   0        0        0     8922 2023-04-03 12:12:15.000000 pyees-1.1.4/pyees/prop.py
--rw-rw-rw-   0        0        0    14265 2023-04-14 07:44:37.000000 pyees-1.1.4/pyees/readData.py
--rw-rw-rw-   0        0        0    10138 2023-04-05 08:09:23.000000 pyees-1.1.4/pyees/solve.py
--rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.1.4/pyees/stackOverflowODR.py
--rw-rw-rw-   0        0        0     3249 2023-03-13 12:35:20.000000 pyees-1.1.4/pyees/testFit.py
--rw-rw-rw-   0        0        0     1671 2023-03-07 14:26:33.000000 pyees-1.1.4/pyees/testProp.py
--rw-rw-rw-   0        0        0     1059 2023-04-14 07:48:34.000000 pyees-1.1.4/pyees/testPyees.py
--rw-rw-rw-   0        0        0     9133 2023-04-03 11:24:36.000000 pyees-1.1.4/pyees/testReadData.py
--rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.1.4/pyees/testSolve.py
--rw-rw-rw-   0        0        0     8044 2023-04-14 07:44:27.000000 pyees-1.1.4/pyees/testUnit.py
--rw-rw-rw-   0        0        0    80327 2023-04-03 13:10:52.000000 pyees-1.1.4/pyees/testVariable.py
--rw-rw-rw-   0        0        0    43305 2023-04-14 07:48:22.000000 pyees-1.1.4/pyees/unit.py
--rw-rw-rw-   0        0        0    34501 2023-04-14 06:49:23.000000 pyees-1.1.4/pyees/variable.py
-drwxrwxrwx   0        0        0        0 2023-04-14 07:49:21.118943 pyees-1.1.4/pyees.egg-info/
--rw-rw-rw-   0        0        0      616 2023-04-14 07:49:19.000000 pyees-1.1.4/pyees.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      477 2023-04-14 07:49:19.000000 pyees-1.1.4/pyees.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 07:49:19.000000 pyees-1.1.4/pyees.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-14 07:49:19.000000 pyees-1.1.4/pyees.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-14 07:49:19.000000 pyees-1.1.4/pyees.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-14 07:49:21.212694 pyees-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1064 2023-04-14 07:49:13.000000 pyees-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:24:20.703124 pyees-1.1.5/
+-rw-rw-rw-   0        0        0     1085 2022-02-05 11:46:00.000000 pyees-1.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      616 2023-04-14 08:24:20.718749 pyees-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2023-03-10 10:19:19.000000 pyees-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-14 08:24:20.468747 pyees-1.1.5/pyees/
+-rw-rw-rw-   0        0        0      619 2023-03-30 05:48:48.000000 pyees-1.1.5/pyees/__init__.py
+-rw-rw-rw-   0        0        0    15688 2023-03-11 13:10:44.000000 pyees-1.1.5/pyees/fit.py
+-rw-rw-rw-   0        0        0      811 2023-04-03 12:11:18.000000 pyees-1.1.5/pyees/profilePyees.py
+-rw-rw-rw-   0        0        0     8922 2023-04-03 12:12:15.000000 pyees-1.1.5/pyees/prop.py
+-rw-rw-rw-   0        0        0    14265 2023-04-14 07:44:37.000000 pyees-1.1.5/pyees/readData.py
+-rw-rw-rw-   0        0        0    10138 2023-04-05 08:09:23.000000 pyees-1.1.5/pyees/solve.py
+-rw-rw-rw-   0        0        0     1406 2022-03-24 20:23:42.000000 pyees-1.1.5/pyees/stackOverflowODR.py
+-rw-rw-rw-   0        0        0     3249 2023-03-13 12:35:20.000000 pyees-1.1.5/pyees/testFit.py
+-rw-rw-rw-   0        0        0     1671 2023-03-07 14:26:33.000000 pyees-1.1.5/pyees/testProp.py
+-rw-rw-rw-   0        0        0     1059 2023-04-14 07:48:34.000000 pyees-1.1.5/pyees/testPyees.py
+-rw-rw-rw-   0        0        0     9133 2023-04-03 11:24:36.000000 pyees-1.1.5/pyees/testReadData.py
+-rw-rw-rw-   0        0        0    20218 2023-04-05 08:10:48.000000 pyees-1.1.5/pyees/testSolve.py
+-rw-rw-rw-   0        0        0     8532 2023-04-14 08:02:12.000000 pyees-1.1.5/pyees/testUnit.py
+-rw-rw-rw-   0        0        0    81154 2023-04-14 08:23:21.000000 pyees-1.1.5/pyees/testVariable.py
+-rw-rw-rw-   0        0        0    43260 2023-04-14 07:59:45.000000 pyees-1.1.5/pyees/unit.py
+-rw-rw-rw-   0        0        0    34872 2023-04-14 08:21:49.000000 pyees-1.1.5/pyees/variable.py
+drwxrwxrwx   0        0        0        0 2023-04-14 08:24:20.656248 pyees-1.1.5/pyees.egg-info/
+-rw-rw-rw-   0        0        0      616 2023-04-14 08:24:18.000000 pyees-1.1.5/pyees.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      477 2023-04-14 08:24:19.000000 pyees-1.1.5/pyees.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-14 08:24:18.000000 pyees-1.1.5/pyees.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-04-14 08:24:18.000000 pyees-1.1.5/pyees.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-14 08:24:19.000000 pyees-1.1.5/pyees.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-14 08:24:20.749999 pyees-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1064 2023-04-14 08:24:09.000000 pyees-1.1.5/setup.py
```

### Comparing `pyees-1.1.4/LICENSE.txt` & `pyees-1.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyees-1.1.4/PKG-INFO` & `pyees-1.1.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.1.4
+Version: 1.1.5
 Summary: EES but for python
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.1.4/README.md` & `pyees-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pyees-1.1.4/pyees/__init__.py` & `pyees-1.1.5/pyees/__init__.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.4/pyees/fit.py` & `pyees-1.1.5/pyees/fit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.4/pyees/profilePyees.py` & `pyees-1.1.5/pyees/profilePyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.4/pyees/prop.py` & `pyees-1.1.5/pyees/prop.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.4/pyees/readData.py` & `pyees-1.1.5/pyees/readData.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.4/pyees/solve.py` & `pyees-1.1.5/pyees/solve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.4/pyees/stackOverflowODR.py` & `pyees-1.1.5/pyees/stackOverflowODR.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.4/pyees/testFit.py` & `pyees-1.1.5/pyees/testFit.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.4/pyees/testProp.py` & `pyees-1.1.5/pyees/testProp.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.4/pyees/testPyees.py` & `pyees-1.1.5/pyees/testPyees.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.4/pyees/testReadData.py` & `pyees-1.1.5/pyees/testReadData.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.4/pyees/testSolve.py` & `pyees-1.1.5/pyees/testSolve.py`

 * *Files identical despite different names*

### Comparing `pyees-1.1.4/pyees/testUnit.py` & `pyees-1.1.5/pyees/testUnit.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,14 +178,25 @@
             a = unit('m!/s')
         self.assertEqual('The character ! is not used within the unitsystem', str(context.exception))
 
         with self.assertRaises(Exception) as context:
             a = unit('m/s/bar')
         self.assertEqual('A unit can only have a single slash (/)', str(context.exception))
 
+        self.assertEqual(str(unit(' ')), '1')
+        self.assertEqual(str(unit('-')), '1')
+        self.assertEqual(str(unit('')), '1')
+        self.assertEqual(str(unit('--')), '1')
+        self.assertEqual(str(unit('()')), '1')
+        self.assertEqual(str(unit('( )')), '1')
+        self.assertEqual(str(unit('(  )')), '1')  
+        self.assertEqual(str(unit('(-)')), '1')
+        self.assertEqual(str(unit('(--)')), '1')
+        self.assertEqual(str(unit('( -)')), '1')
+
     def testAddNewUnit(self):
         addNewUnit('gnA', 9.81, 'm/s2')
         converter = unit('gnA').getConverter('m/s2')
         self.assertEqual(converter.convert(1), 9.81)
         
         addNewUnit('gnB', 9.81, 'm/s2', 0)
         converter = unit('gnB').getConverter('m/s2')
```

### Comparing `pyees-1.1.4/pyees/testVariable.py` & `pyees-1.1.5/pyees/testVariable.py`

 * *Files 1% similar despite different names*

```diff
@@ -486,14 +486,34 @@
         with self.assertRaises(Exception) as context:
             A[1]
         self.assertTrue("'scalarVariable' object is not subscriptable" in str(context.exception))
 
         with self.assertRaises(Exception) as context:
             A_vec[23]
         self.assertTrue('list index out of range' in str(context.exception))
+        
+        a_vec = A_vec[0]
+        self.assertEqual(a_vec.value, 12.3)
+        self.assertEqual(a_vec.unit, 'L/min')
+        self.assertEqual(a_vec.uncert, 2.6)
+        
+        a_vec = A_vec[0:2]
+        np.testing.assert_array_equal(a_vec.value, [12.3, 54.3])
+        self.assertEqual(a_vec.unit, 'L/min')
+        np.testing.assert_array_equal(a_vec.uncert, [2.6, 5.4])
+        
+        a_vec = A_vec[1:3]
+        np.testing.assert_array_equal(a_vec.value, [54.3, 91.3])
+        self.assertEqual(a_vec.unit, 'L/min')
+        np.testing.assert_array_equal(a_vec.uncert, [5.4, 10.56])
+        
+        a_vec = A_vec[[0,2]]
+        np.testing.assert_array_equal(a_vec.value, [12.3, 91.3])
+        self.assertEqual(a_vec.unit, 'L/min')
+        np.testing.assert_array_equal(a_vec.uncert, [2.6, 10.56])
 
     def testAddEqual(self):
         A = variable(12.3, 'L/min', uncert=2.6)
         B = variable(745.1, 'L/min', uncert=53.9)
 
         A += B
         self.assertAlmostEqual(A.value, 12.3 + 745.1)
```

### Comparing `pyees-1.1.4/pyees/unit.py` & `pyees-1.1.5/pyees/unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -507,14 +507,16 @@
             upper = ['DELTA' + elem if elem in temperature else elem for elem in upper]
             lower = ['DELTA' + elem if elem in temperature else elem for elem in lower]
 
         return upper, upperPrefix, upperExp, lower, lowerPrefix, lowerExp
 
     @ staticmethod
     def _formatUnit(unitStr):
+        ## TODO this is a mess - remake this
+
         # Removing any spaces
         unitStr = unitStr.replace(' ', '')
 
         # Removing any illegal symbols
         for s in unitStr:
             if s not in knownCharacters:
                 raise ValueError(f'The character {s} is not used within the unitsystem')
@@ -620,15 +622,14 @@
                     upper[i] = u + str(e * exponent)
                 for i, low in enumerate(lower):
                     u, e = unit._removeExponentFromUnit(low)
                     lower[i] = u + str(e * exponent)
                 out = '-'.join(upper)
                 if lower:
                     out += '/' + '-'.join(lower)
-                return out
             except TypeError:
                 raise TypeError()
         return parts
     
     @ staticmethod
     def _splitCompositeUnit(compositeUnit):
         lower = []
@@ -1096,16 +1097,15 @@
 
         self._SIBaseUnit = self._getSIBaseUnit(self.upper, self.upperExp, self.lower, self.lowerExp)
         otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp = self._getLists(self._SIBaseUnit)
         self._converterToSI = self._getConverter(otherUpper, otherUpperPrefix, otherUpperExp, otherLower, otherLowerPrefix, otherLowerExp)
 
 
 if __name__ == "__main__":
-    a = unit('C')
-    b = unit('C')
-    print(a - b, 'DELTAC')
-    
-    a = unit('J/kg-DELTAK')
-    b = unit('J/kg-DELTAK')
-    print(a - b, 'J/kg-DELTAK')
+    a = unit(' ')
+    print(a)
+    a = unit('-')
+    print(a)
+    a = unit('')
+    print(a)
```

### Comparing `pyees-1.1.4/pyees/variable.py` & `pyees-1.1.5/pyees/variable.py`

 * *Files 2% similar despite different names*

```diff
@@ -711,25 +711,34 @@
 
     def __hash__(self):
         return id(self)
 
 
 class arrayVariable(scalarVariable):
     
-    def __init__(self, value, unitStr, uncert, nDigits) -> None:
-        self.nDigits = nDigits
+    def __init__(self, value = None, unitStr = None, uncert= None, nDigits= None, scalarVariables = None) -> None:
         
-        # create a unit object
-        self._unitObject = unitStr if isinstance(unitStr, unit) else unit(unitStr)        
+        if not (value is None) and not (scalarVariables is None):
+            raise ValueError('You cannot supply both values and scalarVariables')
         
-        self.scalarVariables = []
         if not value is None:
-            for v, u in zip(value, uncert):
-                self.scalarVariables.append(scalarVariable(v, self._unitObject, u, nDigits))
-    
+            self.nDigits = nDigits
+            
+            # create a unit object
+            self._unitObject = unitStr if isinstance(unitStr, unit) else unit(unitStr)        
+            
+            self.scalarVariables = []
+            if not value is None:
+                for v, u in zip(value, uncert):
+                    self.scalarVariables.append(scalarVariable(v, self._unitObject, u, nDigits))
+        else:
+            self.scalarVariables = scalarVariables
+            self._unitObject = self.scalarVariables[0]._unitObject
+            self.nDigits = self.scalarVariables[0].nDigits
+            
     def _calculateUncertanty(self):
         for elem in self.scalarVariables:
             elem._calculateUncertanty()
     
     def addCovariance(self, var, grad: np.ndarray, unitStr: str):
         for elem, varElem, gradElem in zip(self.scalarVariables, var, grad):
             elem.addCovariance(varElem, gradElem, unitStr)
@@ -747,17 +756,17 @@
         return len(self.scalarVariables)
 
     def __getitem__(self, index):
         
         if isinstance(index, int):
             return self.scalarVariables[index]
         elif isinstance(index, slice):
-            vals = [elem.value for elem in self.scalarVariables[index]]
-            unc = [elem.uncert for elem in self.scalarVariables[index]]
-            return variable(vals, self._unitObject, unc, self.nDigits)
+            return arrayVariable(scalarVariables = self.scalarVariables[index])
+        if isinstance(index, list):
+            return arrayVariable(scalarVariables = [self.scalarVariables[elem] for elem in index])
         else:
             raise NotImplementedError()
  
     @property
     def value(self):
         return np.array([elem.value for elem in self.scalarVariables])       
  
@@ -883,18 +892,15 @@
             if len(self) != len(other):
                 raise ValueError(f'operands could not be broadcast together with shapes {self.value.shape} {other.value.shape}')
             out = [a**b for a,b in zip(self, other)]
         else:
             out = [a**other for a in self]
 
         if all([out[0].unit == elem.unit for elem in out]):
-            oout = arrayVariable(None, out[0].unit, None, out[0].nDigits)
-            for o in out:
-                oout.append(o)
-            return oout
+            return arrayVariable(scalarVariables=out)
         
         return out
      
     def __rpow__(self,other):
         if not (isinstance(other, scalarVariable) or isinstance(other, arrayVariable)):
             return variable(other) ** self
     
@@ -985,19 +991,17 @@
             if len(uncert) != len(value):
                 raise ValueError('The lenght of the value has to be equal to the lenght of the uncertanty')
         else:
             if isinstance(uncert, np.ndarray):
                 raise ValueError('The lenght of the value has to be equal to the lenght of the uncertanty')      
     
     if isinstance(value, np.ndarray):
-        return arrayVariable(value, unit, uncert, nDigits)
+        return arrayVariable(value = value, unitStr = unit, uncert = uncert, nDigits = nDigits)
     else:
         return scalarVariable(value, unit, uncert, nDigits)
 
 
 if __name__ == "__main__":
-    a = variable(1,'J/kg-DELTAK')
-    b = variable(1,'J/kg-DELTAK')
-    c = a + b
-    
+    a = variable(1)
+    print(a)
```

### Comparing `pyees-1.1.4/pyees.egg-info/PKG-INFO` & `pyees-1.1.5/pyees.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyees
-Version: 1.1.4
+Version: 1.1.5
 Summary: EES but for python
 Home-page: https://github.com/jacobv95/pyees
 Download-URL: https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz
 Author: Jacob Vestergaard
 Author-email: jacobvestergaard95@gmail.com
 License: MIT
 Keywords: python,data processing,uncertanty,EES
```

### Comparing `pyees-1.1.4/setup.py` & `pyees-1.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
     name='pyees',
     packages=['pyees'],
-    version='1.1.4',
+    version='1.1.5',
     license='MIT',
     description='EES but for python',
     author='Jacob Vestergaard',
     author_email='jacobvestergaard95@gmail.com',
     url='https://github.com/jacobv95/pyees',
     download_url='https://github.com/jacobv95/pyees/archive/refs/tags/v1.0.tar.gz',
     keywords=['python', 'data processing', 'uncertanty', 'EES'],
```

