# Comparing `tmp/economic-complexity-0.1.2.tar.gz` & `tmp/economic_complexity-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "economic-complexity-0.1.2.tar", max compression
+gzip compressed data, was "economic_complexity-0.1.3.tar", max compression
```

## Comparing `economic-complexity-0.1.2.tar` & `economic_complexity-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      618 2022-11-15 21:11:28.673575 economic-complexity-0.1.2/economic_complexity/__init__.py
--rw-r--r--   0        0        0     2248 2022-11-15 21:13:07.101014 economic-complexity-0.1.2/economic_complexity/complexity.py
--rw-r--r--   0        0        0     3774 2022-05-04 21:01:08.480474 economic-complexity-0.1.2/economic_complexity/cross_space.py
--rw-r--r--   0        0        0    10822 2022-11-15 21:12:15.198854 economic-complexity-0.1.2/economic_complexity/product_space.py
--rw-r--r--   0        0        0     1431 2022-11-15 21:12:43.234320 economic-complexity-0.1.2/economic_complexity/rca.py
--rw-r--r--   0        0        0     1071 2022-05-06 03:32:39.758645 economic-complexity-0.1.2/LICENSE
--rw-r--r--   0        0        0     3032 2022-11-15 21:09:40.964713 economic-complexity-0.1.2/PACKAGE.md
--rw-r--r--   0        0        0      729 2022-11-15 21:14:57.006938 economic-complexity-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     3802 1970-01-01 00:00:00.000000 economic-complexity-0.1.2/setup.py
--rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 economic-complexity-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      695 2023-04-14 20:01:48.594569 economic_complexity-0.1.3/economic_complexity/__init__.py
+-rw-r--r--   0        0        0     2248 2022-11-15 21:13:07.101014 economic_complexity-0.1.3/economic_complexity/complexity.py
+-rw-r--r--   0        0        0     3774 2022-05-04 21:01:08.480474 economic_complexity-0.1.3/economic_complexity/cross_space.py
+-rw-r--r--   0        0        0    11108 2023-04-14 19:59:47.028046 economic_complexity-0.1.3/economic_complexity/product_space.py
+-rw-r--r--   0        0        0     1431 2022-11-15 21:12:43.234320 economic_complexity-0.1.3/economic_complexity/rca.py
+-rw-r--r--   0        0        0     2246 2023-04-14 19:59:47.029052 economic_complexity-0.1.3/economic_complexity/subnational.py
+-rw-r--r--   0        0        0     1071 2022-05-06 03:32:39.758645 economic_complexity-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3032 2022-11-15 21:09:40.964713 economic_complexity-0.1.3/PACKAGE.md
+-rw-r--r--   0        0        0      740 2023-04-14 20:01:42.840008 economic_complexity-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3848 1970-01-01 00:00:00.000000 economic_complexity-0.1.3/PKG-INFO
```

### Comparing `economic-complexity-0.1.2/economic_complexity/__init__.py` & `economic_complexity-0.1.3/economic_complexity/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 This module contains functions to ease the calculation of Economic Complexity values.
 """
 
 from .rca import rca
 from .complexity import complexity
 from .product_space import distance, opportunity_gain, proximity, relatedness, similarity, pgi, peii
 from .cross_space import cross_proximity, cross_relatedness
+from .subnational import complexity_subnational
 
-__version_info__ = ('0', '1', '2')
+__version_info__ = ('0', '1', '3')
 __version__ = '.'.join(__version_info__)
 
 __all__ = (
     "rca",
     "complexity",
     "distance",
     "opportunity_gain",
     "proximity",
     "relatedness",
     "cross_proximity",
     "cross_relatedness",
     "similarity",
     "pgi",
     "peii",
+    "complexity_subnational"
 )
```

### Comparing `economic-complexity-0.1.2/economic_complexity/complexity.py` & `economic_complexity-0.1.3/economic_complexity/complexity.py`

 * *Files identical despite different names*

### Comparing `economic-complexity-0.1.2/economic_complexity/cross_space.py` & `economic_complexity-0.1.3/economic_complexity/cross_space.py`

 * *Files identical despite different names*

### Comparing `economic-complexity-0.1.2/economic_complexity/product_space.py` & `economic_complexity-0.1.3/economic_complexity/product_space.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,283 +1,283 @@
-"""Product Space module
-"""
-
-import pandas as pd
-import numpy as np
-
-
-def proximity(rcas: pd.DataFrame, procedure="max"):
-    """Calculates the Proximity index for a matrix of RCAs.
-
-    Hidalgo et al. (2007), introduces the Proximity index which measures the
-    minimum probability that a country has comparative advantages in the export
-    of a product `i`, given that it has comparative advantages in a product `j`.
-
-    This function only needs the pivot table obtained from the RCA function,
-    and returns a square matrix with the proximity between the elements.
-
-    Args:
-        rcas (pd.DataFrame) -- A RCA matrix of pivotted values.
-        procedure (str, optional) -- Determines how to calcule the denominator.
-            Available options are "sqrt" and "max", defaults to "max".
-
-    Returns:
-        (pd.DataFrame) -- A square matrix with the proximity between the elements.
-    """
-    rcas = rcas.copy()
-    rcas[rcas >= 1] = 1
-    rcas[rcas < 1] = 0
-
-    # transpose the matrix so that it is now industries as rows
-    # and munics as columns
-    rcas_t = rcas.T.fillna(0)
-
-    # Matrix multiplication on M_mi matrix and transposed version,
-    # number of products = number of rows and vice versa on transposed
-    # version, thus the shape of this result will be length of products
-    # by the length of products (symetric)
-    numerator_intersection = rcas_t.dot(rcas_t.T)
-
-    # kp0 is a vector of the number of munics with RCA in the given product
-    kp0 = rcas.sum(axis=0)
-    kp0 = kp0.to_numpy().reshape((1, len(kp0)))
-
-    # transpose this to get the unions
-    kp0_trans = kp0.T
-
-    # multiply these two vectors, take the squre root
-    # and then we have the denominator
-    if procedure == "sqrt":
-        # get square root for geometric mean
-        denominator_union = kp0_trans.dot(kp0)
-        denominator_union = np.power(denominator_union, .5)
-    else:
-        denominator_union = np.maximum(kp0, kp0_trans)
-
-    # to get the proximities it is now a simple division of the untion sqrt
-    # with the numerator intersections
-    phi = np.divide(numerator_intersection, denominator_union)
-    np.fill_diagonal(phi.values, 0)
-
-    return phi
-
-
-def relatedness(rcas: pd.DataFrame, proximities: pd.DataFrame):
-    """Calculates the Relatedness, given a matrix of RCAs for the economic
-    activities of a location, and a matrix of Proximities.
-
-    The fact that the growth of an activity in a location is correlated with
-    relatedness is known as The Principle of Relatedness, introduced by
-    Hidalgo et al. (2018), which consists of a statistical law that tells us
-    that the probability a location (a country, city, or region) enters an
-    economic activity (e.g. a product, industry, technology), grows with the
-    number of related activities present in that location.
-
-    Scholars measure Relatedness between a location and an economic activity
-    to predict the probability that a region will enter or exit that activity
-    in the future.
-
-    Args:
-        rcas (pd.DataFrame) -- Matrix of RCAs for a certain location.
-        proximities (pd.DataFrame) -- Matrix with the proximity between the elements.
-
-    Returns:
-        (pd.DataFrame) -- A matrix with the probability that a location
-            generates comparative advantages in a economic activity.
-    """
-    rcas = rcas.copy()
-    rcas[rcas >= 1] = 1
-    rcas[rcas < 1] = 0
-
-    # Get numerator by matrix multiplication of proximities with M_im
-    density_numerator = rcas.dot(proximities)
-
-    # Get denominator by multiplying proximities by all ones vector thus
-    # getting the sum of all proximities
-    # rcas_ones = pd.DataFrame(np.ones_like(rcas))
-    rcas_ones = rcas * 0
-    rcas_ones = rcas_ones + 1
-    # print rcas_ones.shape, proximities.shape
-    density_denominator = rcas_ones.dot(proximities)
-
-    # We now have our densities matrix by dividing numerator by denomiator
-    densities = density_numerator / density_denominator
-
-    return densities
-
-
-def distance(rcas: pd.DataFrame, proximities: pd.DataFrame):
-    """Calculates the distance.
-
-    In this context, the Distance for a Country and a certain Product is defined
-    as the
-
-    Args:
-        rcas (pd.DataFrame) -- Matrix of RCAs for a certain location.
-        proximities (pd.DataFrame) -- Matrix with the proximity between the elements.
-
-    Returns:
-        (pd.DataFrame) --
-    """
-    return 1 - relatedness(rcas, proximities)
-
-
-def opportunity_gain(rcas: pd.DataFrame, proximities: pd.DataFrame, pci: pd.DataFrame):
-    """Calculates the opportunity gain caused by the contribution of a certain
-    characteristic, relative to how this affects other characteristics.
-
-    Args:
-        rcas (pd.DataFrame) -- Matrix of RCAs considering a
-        proximities (pd.DataFrame) -- [description]
-        pci (pd.DataFrame) -- [description]
-
-    Returns:
-        (pd.DataFrame) --
-    """
-    rcas = rcas.copy()
-    rcas[rcas >= 1] = 1
-    rcas[rcas < 1] = 0
-
-    # turn proximities in to ratios out of total
-    prox_ratio = proximities / proximities.sum()
-
-    # get the inverse of the RCAs matrix. Since they are in the form of 1's and
-    # 0's this will flip all of them i.e. 1 = 0 and 0 = 1
-    inverse_rcas = 1 - rcas
-
-    # here we now have the middle part of the equation
-    middle = inverse_rcas.multiply(pci)
-
-    # get the relatedness with the backwards bizzaro RCAs
-    dcp = relatedness(inverse_rcas, proximities)
-    # now get the inverse
-    dcp = 1 - dcp
-    # we now have the right-half of the equation
-    right = dcp.multiply(pci)
-
-    # matrix multiplication with proximities ratio
-    opp_gain = middle.dot(prox_ratio) - right
-
-    return opp_gain
-
-
-def similarity(rcas: pd.DataFrame):
-    """
-    Calculates the Export Similarity Index for a matrix of RCAs.
-
-    Bahar et al. (2014) introduces this measure of similarity in the export structure of a pair of countries c and c'. It's defined as the Pearson correlation between the logarithm of the RCA vectors of the two countries.
-
-    This function only needs the pivot table obtained from the RCA function,
-    and returns a square matrix with the Export Similarity Index between the elements.
-
-    Args:
-        rcas (pd.DataFrame) -- A RCA matrix of pivotted values.
-
-    Returns:
-        (pd.DataFrame) -- A square matrix with the Export Similarity Index between the elements.
-    """
-
-    # Take the log of rcas (add 0.1 as \epsilon)
-    rcas = np.log(rcas + 0.1)
-
-    # calculate the matrix through the pearson correlation
-    scc = pd.DataFrame(np.corrcoef(rcas), columns=rcas.index, index = rcas.index)
-
-    return scc
-
-
-def pmi(tbl: pd.DataFrame, rcas: pd.DataFrame, measure: pd.DataFrame, measure_name: str) -> pd.DataFrame:
-    """
-    Calculates the Product 'measure' Index, where measure corresponds to a dataframe with the measure values for each geography.
-    For example, in the literature this method has been applied to calculate the Product Gini Index (PGI) and the Product Emission Intensity Index.
-
-    Args:
-        tbl (pd.DataFrame) -- A pivoted table using a geographic index,
-            columns with the categories to be evaluated and the measurement of
-            the data as values.
-        measure (pd.DataFrame) -- A table using a geographic index, with a single column with the measure values.
-        measure_name (str) -- A string with the name of the measure
-
-    Returns:
-        (pd.DataFrame) -- A square matrix with the Export Similarity Index between the elements.
-
-    """
-    # drop product with no exports and fill missing values with zeros
-    tbl = tbl.dropna(how="all", axis=1).fillna(value=0)
-    measure = measure.fillna(value=0)
-
-    # get Mcp matrix
-    m = rcas.copy()
-    m[rcas >= 1] = 1
-    m[rcas < 1] = 0
-
-    # Ensures that the matrices are aligned by removing geographies that don't exist in both matrices
-    tbl_geo = tbl.index
-    measure_geo = measure.index
-    intersection_geo = list(set(tbl_geo) & set(measure_geo))
-    tbl = tbl.filter(items=intersection_geo, axis=0)
-    measure = measure.filter(items=intersection_geo, axis=0)
-    m = m.filter(items=intersection_geo, axis=0)
-
-    tbl = tbl.sort_index(ascending=True)
-    measure = measure.sort_index(ascending=True)
-    m = m.sort_index(ascending=True)
-
-    # get Scp matrix
-    col_sums = tbl.sum(axis=1)
-    col_sums = col_sums.to_numpy().reshape((len(col_sums), 1))
-    scp = np.divide(tbl, col_sums)
-
-    # get Np array
-    normp = m.multiply(scp).sum(axis=0)
-    normp = pd.DataFrame(normp)
-
-    num = m.multiply(scp).T.dot(measure)
-
-    pmi = np.divide(num, normp)
-    pmi.rename(columns={pmi.columns[0]: measure_name}, inplace=True)
-
-    return pmi
-
-def pgi(tbl: pd.DataFrame, rcas: pd.DataFrame, gini: pd.DataFrame) -> pd.DataFrame:
-
-    """Calculates the Product Gini Index (PGI) for a pivoted matrix.
-    It is important to note that even though the functions do not use a
-    parameter in relation to time, the data used for the calculations must
-    be per period; for example working with World Exports for the year 2020.
-    Also, the index always has to be a geographic level.
-    It is also important to make sure that the input matrices are aligned,
-    that is, that both matrices consider the same geographic units.
-    Arguments:
-        tbl (pandas.DataFrame) -- A pivoted table using a geographic index,
-            columns with the categories to be evaluated and the measurement of
-            the data as values.
-        gini (pandas.DataFrame) -- A matrix of GINI indices using a geographic index.
-    Returns:
-        (pandas.DataFrame) -- PGI matrix with categories evaluated as an index.
-    """
-
-    pgip = pmi(tbl = tbl, rcas = rcas, measure = gini, measure_name='pgi')
-
-    return pgip
-
-def peii(tbl: pd.DataFrame, rcas: pd.DataFrame, emissions: pd.DataFrame) -> pd.DataFrame:
-
-    """
-    Calculates the Product Emissions Intensity Index (PEII) for a pivoted matrix.
-    It is important to note that even though the functions do not use a
-    parameter in relation to time, the data used for the calculations must
-    be per period; for example working with World Exports for the year 2020.
-    Also, the index always has to be a geographic level.
-    It is also important to make sure that the input matrices are aligned,
-    that is, that both matrices consider the same geographic units.
-    Arguments:
-        tbl (pandas.DataFrame) -- A pivoted table using a geographic index,
-            columns with the categories to be evaluated and the measurement of
-            the data as values.
-        emissions (pandas.DataFrame) -- A matrix of emissions intensity using a geographic index.
-    Returns:
-        (pandas.DataFrame) -- PEII matrix with categories evaluated as an index.
-    """
-
-    peii = pmi(tbl = tbl, rcas = rcas, measure=emissions, measure_name='peii')
-    return peii
+"""Product Space module
+"""
+
+import pandas as pd
+import numpy as np
+
+
+def proximity(rcas: pd.DataFrame, procedure="max"):
+    """Calculates the Proximity index for a matrix of RCAs.
+
+    Hidalgo et al. (2007), introduces the Proximity index which measures the
+    minimum probability that a country has comparative advantages in the export
+    of a product `i`, given that it has comparative advantages in a product `j`.
+
+    This function only needs the pivot table obtained from the RCA function,
+    and returns a square matrix with the proximity between the elements.
+
+    Args:
+        rcas (pd.DataFrame) -- A RCA matrix of pivotted values.
+        procedure (str, optional) -- Determines how to calcule the denominator.
+            Available options are "sqrt" and "max", defaults to "max".
+
+    Returns:
+        (pd.DataFrame) -- A square matrix with the proximity between the elements.
+    """
+    rcas = rcas.copy()
+    rcas[rcas >= 1] = 1
+    rcas[rcas < 1] = 0
+
+    # transpose the matrix so that it is now industries as rows
+    # and munics as columns
+    rcas_t = rcas.T.fillna(0)
+
+    # Matrix multiplication on M_mi matrix and transposed version,
+    # number of products = number of rows and vice versa on transposed
+    # version, thus the shape of this result will be length of products
+    # by the length of products (symetric)
+    numerator_intersection = rcas_t.dot(rcas_t.T)
+
+    # kp0 is a vector of the number of munics with RCA in the given product
+    kp0 = rcas.sum(axis=0)
+    kp0 = kp0.to_numpy().reshape((1, len(kp0)))
+
+    # transpose this to get the unions
+    kp0_trans = kp0.T
+
+    # multiply these two vectors, take the squre root
+    # and then we have the denominator
+    if procedure == "sqrt":
+        # get square root for geometric mean
+        denominator_union = kp0_trans.dot(kp0)
+        denominator_union = np.power(denominator_union, .5)
+    else:
+        denominator_union = np.maximum(kp0, kp0_trans)
+
+    # to get the proximities it is now a simple division of the untion sqrt
+    # with the numerator intersections
+    phi = np.divide(numerator_intersection, denominator_union)
+    np.fill_diagonal(phi.values, 0)
+
+    return phi
+
+
+def relatedness(rcas: pd.DataFrame, proximities: pd.DataFrame):
+    """Calculates the Relatedness, given a matrix of RCAs for the economic
+    activities of a location, and a matrix of Proximities.
+
+    The fact that the growth of an activity in a location is correlated with
+    relatedness is known as The Principle of Relatedness, introduced by
+    Hidalgo et al. (2018), which consists of a statistical law that tells us
+    that the probability a location (a country, city, or region) enters an
+    economic activity (e.g. a product, industry, technology), grows with the
+    number of related activities present in that location.
+
+    Scholars measure Relatedness between a location and an economic activity
+    to predict the probability that a region will enter or exit that activity
+    in the future.
+
+    Args:
+        rcas (pd.DataFrame) -- Matrix of RCAs for a certain location.
+        proximities (pd.DataFrame) -- Matrix with the proximity between the elements.
+
+    Returns:
+        (pd.DataFrame) -- A matrix with the probability that a location
+            generates comparative advantages in a economic activity.
+    """
+    rcas = rcas.copy()
+    rcas[rcas >= 1] = 1
+    rcas[rcas < 1] = 0
+
+    # Get numerator by matrix multiplication of proximities with M_im
+    density_numerator = rcas.dot(proximities)
+
+    # Get denominator by multiplying proximities by all ones vector thus
+    # getting the sum of all proximities
+    # rcas_ones = pd.DataFrame(np.ones_like(rcas))
+    rcas_ones = rcas * 0
+    rcas_ones = rcas_ones + 1
+    # print rcas_ones.shape, proximities.shape
+    density_denominator = rcas_ones.dot(proximities)
+
+    # We now have our densities matrix by dividing numerator by denomiator
+    densities = density_numerator / density_denominator
+
+    return densities
+
+
+def distance(rcas: pd.DataFrame, proximities: pd.DataFrame):
+    """Calculates the distance.
+
+    In this context, the Distance for a Country and a certain Product is defined
+    as the
+
+    Args:
+        rcas (pd.DataFrame) -- Matrix of RCAs for a certain location.
+        proximities (pd.DataFrame) -- Matrix with the proximity between the elements.
+
+    Returns:
+        (pd.DataFrame) --
+    """
+    return 1 - relatedness(rcas, proximities)
+
+
+def opportunity_gain(rcas: pd.DataFrame, proximities: pd.DataFrame, pci: pd.DataFrame):
+    """Calculates the opportunity gain caused by the contribution of a certain
+    characteristic, relative to how this affects other characteristics.
+
+    Args:
+        rcas (pd.DataFrame) -- Matrix of RCAs considering a
+        proximities (pd.DataFrame) -- [description]
+        pci (pd.DataFrame) -- [description]
+
+    Returns:
+        (pd.DataFrame) --
+    """
+    rcas = rcas.copy()
+    rcas[rcas >= 1] = 1
+    rcas[rcas < 1] = 0
+
+    # turn proximities in to ratios out of total
+    prox_ratio = proximities / proximities.sum()
+
+    # get the inverse of the RCAs matrix. Since they are in the form of 1's and
+    # 0's this will flip all of them i.e. 1 = 0 and 0 = 1
+    inverse_rcas = 1 - rcas
+
+    # here we now have the middle part of the equation
+    middle = inverse_rcas.multiply(pci)
+
+    # get the relatedness with the backwards bizzaro RCAs
+    dcp = relatedness(inverse_rcas, proximities)
+    # now get the inverse
+    dcp = 1 - dcp
+    # we now have the right-half of the equation
+    right = dcp.multiply(pci)
+
+    # matrix multiplication with proximities ratio
+    opp_gain = middle.dot(prox_ratio) - right
+
+    return opp_gain
+
+
+def similarity(rcas: pd.DataFrame):
+    """
+    Calculates the Export Similarity Index for a matrix of RCAs.
+
+    Bahar et al. (2014) introduces this measure of similarity in the export structure of a pair of countries c and c'. It's defined as the Pearson correlation between the logarithm of the RCA vectors of the two countries.
+
+    This function only needs the pivot table obtained from the RCA function,
+    and returns a square matrix with the Export Similarity Index between the elements.
+
+    Args:
+        rcas (pd.DataFrame) -- A RCA matrix of pivotted values.
+
+    Returns:
+        (pd.DataFrame) -- A square matrix with the Export Similarity Index between the elements.
+    """
+
+    # Take the log of rcas (add 0.1 as \epsilon)
+    rcas = np.log(rcas + 0.1)
+
+    # calculate the matrix through the pearson correlation
+    scc = pd.DataFrame(np.corrcoef(rcas), columns=rcas.index, index = rcas.index)
+
+    return scc
+
+
+def _pmi(tbl: pd.DataFrame, rcas: pd.DataFrame, measure: pd.DataFrame, measure_name: str) -> pd.DataFrame:
+    """
+    Calculates the Product 'measure' Index, where measure corresponds to a dataframe with the measure values for each geography.
+    For example, in the literature this method has been applied to calculate the Product Gini Index (PGI) and the Product Emission Intensity Index.
+
+    Args:
+        tbl (pd.DataFrame) -- A pivoted table using a geographic index,
+            columns with the categories to be evaluated and the measurement of
+            the data as values.
+        measure (pd.DataFrame) -- A table using a geographic index, with a single column with the measure values.
+        measure_name (str) -- A string with the name of the measure
+
+    Returns:
+        (pd.DataFrame) -- A square matrix with the Export Similarity Index between the elements.
+
+    """
+    # drop product with no exports and fill missing values with zeros
+    tbl = tbl.dropna(how="all", axis=1).fillna(value=0)
+    measure = measure.fillna(value=0)
+
+    # get Mcp matrix
+    m = rcas.copy()
+    m[rcas >= 1] = 1
+    m[rcas < 1] = 0
+
+    # Ensures that the matrices are aligned by removing geographies that don't exist in both matrices
+    tbl_geo = tbl.index
+    measure_geo = measure.index
+    intersection_geo = list(set(tbl_geo) & set(measure_geo))
+    tbl = tbl.filter(items=intersection_geo, axis=0)
+    measure = measure.filter(items=intersection_geo, axis=0)
+    m = m.filter(items=intersection_geo, axis=0)
+
+    tbl = tbl.sort_index(ascending=True)
+    measure = measure.sort_index(ascending=True)
+    m = m.sort_index(ascending=True)
+
+    # get Scp matrix
+    col_sums = tbl.sum(axis=1)
+    col_sums = col_sums.to_numpy().reshape((len(col_sums), 1))
+    scp = np.divide(tbl, col_sums)
+
+    # get Np array
+    normp = m.multiply(scp).sum(axis=0)
+    normp = pd.DataFrame(normp)
+
+    num = m.multiply(scp).T.dot(measure)
+
+    pmi = np.divide(num, normp)
+    pmi.rename(columns={pmi.columns[0]: measure_name}, inplace=True)
+
+    return pmi
+
+def pgi(tbl: pd.DataFrame, rcas: pd.DataFrame, gini: pd.DataFrame) -> pd.DataFrame:
+
+    """Calculates the Product Gini Index (PGI) for a pivoted matrix.
+    It is important to note that even though the functions do not use a
+    parameter in relation to time, the data used for the calculations must
+    be per period; for example working with World Exports for the year 2020.
+    Also, the index always has to be a geographic level.
+    It is also important to make sure that the input matrices are aligned,
+    that is, that both matrices consider the same geographic units.
+    Arguments:
+        tbl (pandas.DataFrame) -- A pivoted table using a geographic index,
+            columns with the categories to be evaluated and the measurement of
+            the data as values.
+        gini (pandas.DataFrame) -- A matrix of GINI indices using a geographic index.
+    Returns:
+        (pandas.DataFrame) -- PGI matrix with categories evaluated as an index.
+    """
+
+    pgip = _pmi(tbl = tbl, rcas = rcas, measure = gini, measure_name='pgi')
+
+    return pgip
+
+def peii(tbl: pd.DataFrame, rcas: pd.DataFrame, emissions: pd.DataFrame) -> pd.DataFrame:
+
+    """
+    Calculates the Product Emissions Intensity Index (PEII) for a pivoted matrix.
+    It is important to note that even though the functions do not use a
+    parameter in relation to time, the data used for the calculations must
+    be per period; for example working with World Exports for the year 2020.
+    Also, the index always has to be a geographic level.
+    It is also important to make sure that the input matrices are aligned,
+    that is, that both matrices consider the same geographic units.
+    Arguments:
+        tbl (pandas.DataFrame) -- A pivoted table using a geographic index,
+            columns with the categories to be evaluated and the measurement of
+            the data as values.
+        emissions (pandas.DataFrame) -- A matrix of emissions intensity using a geographic index.
+    Returns:
+        (pandas.DataFrame) -- PEII matrix with categories evaluated as an index.
+    """
+
+    peii = _pmi(tbl = tbl, rcas = rcas, measure=emissions, measure_name='peii')
+    return peii
```

### Comparing `economic-complexity-0.1.2/economic_complexity/rca.py` & `economic_complexity-0.1.3/economic_complexity/rca.py`

 * *Files identical despite different names*

### Comparing `economic-complexity-0.1.2/LICENSE` & `economic_complexity-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `economic-complexity-0.1.2/PACKAGE.md` & `economic_complexity-0.1.3/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `economic-complexity-0.1.2/setup.py` & `economic_complexity-0.1.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,65 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: economic-complexity
+Version: 0.1.3
+Summary: Functions to calculate Economic Complexity indicators.
+Home-page: https://github.com/Datawheel/py-economic-complexity
+License: MIT
+Author: Jelmy Hermosilla
+Author-email: jelmy@datawheel.us
+Maintainer: Francisco Abarzua
+Maintainer-email: francisco@datawheel.us
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.24.0,<2.0.0)
+Requires-Dist: pandas (>=1.1.0,<2.0.0)
+Project-URL: Repository, https://github.com/Datawheel/py-economic-complexity
+Description-Content-Type: text/markdown
+
+This package contains functions to calculate Economic Complexity indicators.  
+The functions handle the data through `pandas.DataFrame` objects.
+
+<p>
+<a href="https://github.com/Datawheel/py-economic-complexity"><img src="https://flat.badgen.net/github/release/Datawheel/py-economic-complexity" /></a>
+<a href="https://github.com/Datawheel/py-economic-complexity/blob/master/LICENSE"><img src="https://flat.badgen.net/github/license/Datawheel/py-economic-complexity" /></a>
+<a href="https://github.com/Datawheel/py-economic-complexity/"><img src="https://flat.badgen.net/github/checks/Datawheel/py-economic-complexity" /></a>
+<a href="https://github.com/Datawheel/py-economic-complexity/issues"><img src="https://flat.badgen.net/github/issues/Datawheel/py-economic-complexity" /></a>
+</p>
+
+## Installation
+
+We recommend the use of `poetry`, to resolve the best version of the dependencies that works with your current project.
+
+```bash
+$ poetry add economic-complexity
+```
+
+## Tutorial
+
+We have [a brief Tutorial](https://github.com/Datawheel/py-economic-complexity/blob/main/docs/TUTORIAL.ipynb), using data from the Observatory of Economic Complexity, to get started on how to use the basic functions of this package.  
+More complex functions use the resulting dataframes of the basic functions as arguments.
+
+## References
+
+* Hidalgo, César A. (2021). Economic complexity theory and applications. _Nature Reviews Physics, 3_(2), 92–113. https://doi.org/10.1038/s42254-020-00275-1
+
+* Catalán, P., Navarrete, C., & Figueroa, F. (2020). The scientific and technological cross-space: Is technological diversification driven by scientific endogenous capacity? _Research Policy, 104016_, 104016. https://doi.org/10.1016/j.respol.2020.104016
+
+* Hidalgo, César A., & Hausmann, R. (2009). The building blocks of economic complexity. _Proceedings of the National Academy of Sciences of the United States of America, 106_(26), 10570–10575. https://doi.org/10.1073/pnas.0900943106
+
+* Hidalgo, C. A., Klinger, B., Barabási, A.-L., & Hausmann, R. (2007). The product space conditions the development of nations. _Science (New York, N.Y.), 317_(5837), 482–487. https://doi.org/10.1126/science.1144581
+
+* Hartmann, D., Guevara, M. R., Jara-Figueroa, C., Aristarán, M., & Hidalgo, C. A. (2017). Linking Economic Complexity, Institutions, and Income Inequality. _World Development_, 93, 75–93. https://doi.org/10.1016/j.worlddev.2016.12.020
+
+* Romero, J. P., & Gramkow, C. (2021). Economic complexity and greenhouse gas emissions. _World Development_, 139, 105317. https://doi.org/10.1016/j.worlddev.2020.105317
+
+* Bahar, D., Hausmann, R., Hidalgo, C. A. (2014). Neighbors and the evolution of the comparative advantage of nations: Evidence of international knowledge diffusion?. _Journal of International Economics_, 92, 111-123. http://dx.doi.org/10.1016/j.jinteco.2013.11.001
+
+---
+&copy; 2022 [Datawheel, LLC.](https://www.datawheel.us/)  
+This project is licensed under [MIT](./LICENSE).
 
-packages = \
-['economic_complexity']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['numpy>=1.18.0,<2.0.0', 'pandas>=1.1.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'economic-complexity',
-    'version': '0.1.2',
-    'description': 'Functions to calculate Economic Complexity indicators.',
-    'long_description': 'This package contains functions to calculate Economic Complexity indicators.  \nThe functions handle the data through `pandas.DataFrame` objects.\n\n<p>\n<a href="https://github.com/Datawheel/py-economic-complexity"><img src="https://flat.badgen.net/github/release/Datawheel/py-economic-complexity" /></a>\n<a href="https://github.com/Datawheel/py-economic-complexity/blob/master/LICENSE"><img src="https://flat.badgen.net/github/license/Datawheel/py-economic-complexity" /></a>\n<a href="https://github.com/Datawheel/py-economic-complexity/"><img src="https://flat.badgen.net/github/checks/Datawheel/py-economic-complexity" /></a>\n<a href="https://github.com/Datawheel/py-economic-complexity/issues"><img src="https://flat.badgen.net/github/issues/Datawheel/py-economic-complexity" /></a>\n</p>\n\n## Installation\n\nWe recommend the use of `poetry`, to resolve the best version of the dependencies that works with your current project.\n\n```bash\n$ poetry add economic-complexity\n```\n\n## Tutorial\n\nWe have [a brief Tutorial](https://github.com/Datawheel/py-economic-complexity/blob/main/docs/TUTORIAL.ipynb), using data from the Observatory of Economic Complexity, to get started on how to use the basic functions of this package.  \nMore complex functions use the resulting dataframes of the basic functions as arguments.\n\n## References\n\n* Hidalgo, César A. (2021). Economic complexity theory and applications. _Nature Reviews Physics, 3_(2), 92–113. https://doi.org/10.1038/s42254-020-00275-1\n\n* Catalán, P., Navarrete, C., & Figueroa, F. (2020). The scientific and technological cross-space: Is technological diversification driven by scientific endogenous capacity? _Research Policy, 104016_, 104016. https://doi.org/10.1016/j.respol.2020.104016\n\n* Hidalgo, César A., & Hausmann, R. (2009). The building blocks of economic complexity. _Proceedings of the National Academy of Sciences of the United States of America, 106_(26), 10570–10575. https://doi.org/10.1073/pnas.0900943106\n\n* Hidalgo, C. A., Klinger, B., Barabási, A.-L., & Hausmann, R. (2007). The product space conditions the development of nations. _Science (New York, N.Y.), 317_(5837), 482–487. https://doi.org/10.1126/science.1144581\n\n* Hartmann, D., Guevara, M. R., Jara-Figueroa, C., Aristarán, M., & Hidalgo, C. A. (2017). Linking Economic Complexity, Institutions, and Income Inequality. _World Development_, 93, 75–93. https://doi.org/10.1016/j.worlddev.2016.12.020\n\n* Romero, J. P., & Gramkow, C. (2021). Economic complexity and greenhouse gas emissions. _World Development_, 139, 105317. https://doi.org/10.1016/j.worlddev.2020.105317\n\n* Bahar, D., Hausmann, R., Hidalgo, C. A. (2014). Neighbors and the evolution of the comparative advantage of nations: Evidence of international knowledge diffusion?. _Journal of International Economics_, 92, 111-123. http://dx.doi.org/10.1016/j.jinteco.2013.11.001\n\n---\n&copy; 2022 [Datawheel, LLC.](https://www.datawheel.us/)  \nThis project is licensed under [MIT](./LICENSE).\n',
-    'author': 'Jelmy Hermosilla',
-    'author_email': 'jelmy@datawheel.us',
-    'maintainer': 'Francisco Abarzua',
-    'maintainer_email': 'francisco@datawheel.us',
-    'url': 'https://github.com/Datawheel/py-economic-complexity',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,47 +1,47 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \
-['economic_complexity'] package_data = \ {'': ['*']} install_requires = \
-['numpy>=1.18.0,<2.0.0', 'pandas>=1.1.0,<2.0.0'] setup_kwargs = { 'name':
-'economic-complexity', 'version': '0.1.2', 'description': 'Functions to
-calculate Economic Complexity indicators.', 'long_description': 'This package
-contains functions to calculate Economic Complexity indicators. \nThe functions
-handle the data through `pandas.DataFrame` objects.\n\n
-\n[https://flat.badgen.net/github/release/Datawheel/py-economic-complexity]\n
-[https://flat.badgen.net/github/license/Datawheel/py-economic-complexity]\n
-[https://flat.badgen.net/github/checks/Datawheel/py-economic-complexity]\n
-[https://flat.badgen.net/github/issues/Datawheel/py-economic-complexity]\n
-\n\n## Installation\n\nWe recommend the use of `poetry`, to resolve the best
-version of the dependencies that works with your current project.\n\n```bash\n$
-poetry add economic-complexity\n```\n\n## Tutorial\n\nWe have [a brief
-Tutorial](https://github.com/Datawheel/py-economic-complexity/blob/main/docs/
-TUTORIAL.ipynb), using data from the Observatory of Economic Complexity, to get
-started on how to use the basic functions of this package. \nMore complex
-functions use the resulting dataframes of the basic functions as
-arguments.\n\n## References\n\n* Hidalgo, CÃ©sar A. (2021). Economic complexity
-theory and applications. _Nature Reviews Physics, 3_(2), 92â113. https://
-doi.org/10.1038/s42254-020-00275-1\n\n* CatalÃ¡n, P., Navarrete, C., &
-Figueroa, F. (2020). The scientific and technological cross-space: Is
-technological diversification driven by scientific endogenous capacity?
-_Research Policy, 104016_, 104016. https://doi.org/10.1016/
-j.respol.2020.104016\n\n* Hidalgo, CÃ©sar A., & Hausmann, R. (2009). The
-building blocks of economic complexity. _Proceedings of the National Academy of
-Sciences of the United States of America, 106_(26), 10570â10575. https://
-doi.org/10.1073/pnas.0900943106\n\n* Hidalgo, C. A., Klinger, B., BarabÃ¡si,
-A.-L., & Hausmann, R. (2007). The product space conditions the development of
-nations. _Science (New York, N.Y.), 317_(5837), 482â487. https://doi.org/
-10.1126/science.1144581\n\n* Hartmann, D., Guevara, M. R., Jara-Figueroa, C.,
-AristarÃ¡n, M., & Hidalgo, C. A. (2017). Linking Economic Complexity,
-Institutions, and Income Inequality. _World Development_, 93, 75â93. https://
-doi.org/10.1016/j.worlddev.2016.12.020\n\n* Romero, J. P., & Gramkow, C.
-(2021). Economic complexity and greenhouse gas emissions. _World Development_,
-139, 105317. https://doi.org/10.1016/j.worlddev.2020.105317\n\n* Bahar, D.,
-Hausmann, R., Hidalgo, C. A. (2014). Neighbors and the evolution of the
-comparative advantage of nations: Evidence of international knowledge
+Metadata-Version: 2.1 Name: economic-complexity Version: 0.1.3 Summary:
+Functions to calculate Economic Complexity indicators. Home-page: https://
+github.com/Datawheel/py-economic-complexity License: MIT Author: Jelmy
+Hermosilla Author-email: jelmy@datawheel.us Maintainer: Francisco Abarzua
+Maintainer-email: francisco@datawheel.us Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.24.0,<2.0.0) Requires-Dist: pandas (>=1.1.0,<2.0.0)
+Project-URL: Repository, https://github.com/Datawheel/py-economic-complexity
+Description-Content-Type: text/markdown This package contains functions to
+calculate Economic Complexity indicators. The functions handle the data through
+`pandas.DataFrame` objects.
+[https://flat.badgen.net/github/release/Datawheel/py-economic-complexity]
+[https://flat.badgen.net/github/license/Datawheel/py-economic-complexity]
+[https://flat.badgen.net/github/checks/Datawheel/py-economic-complexity]
+[https://flat.badgen.net/github/issues/Datawheel/py-economic-complexity]
+## Installation We recommend the use of `poetry`, to resolve the best version
+of the dependencies that works with your current project. ```bash $ poetry add
+economic-complexity ``` ## Tutorial We have [a brief Tutorial](https://
+github.com/Datawheel/py-economic-complexity/blob/main/docs/TUTORIAL.ipynb),
+using data from the Observatory of Economic Complexity, to get started on how
+to use the basic functions of this package. More complex functions use the
+resulting dataframes of the basic functions as arguments. ## References *
+Hidalgo, CÃ©sar A. (2021). Economic complexity theory and applications. _Nature
+Reviews Physics, 3_(2), 92â113. https://doi.org/10.1038/s42254-020-00275-1 *
+CatalÃ¡n, P., Navarrete, C., & Figueroa, F. (2020). The scientific and
+technological cross-space: Is technological diversification driven by
+scientific endogenous capacity? _Research Policy, 104016_, 104016. https://
+doi.org/10.1016/j.respol.2020.104016 * Hidalgo, CÃ©sar A., & Hausmann, R.
+(2009). The building blocks of economic complexity. _Proceedings of the
+National Academy of Sciences of the United States of America, 106_(26),
+10570â10575. https://doi.org/10.1073/pnas.0900943106 * Hidalgo, C. A.,
+Klinger, B., BarabÃ¡si, A.-L., & Hausmann, R. (2007). The product space
+conditions the development of nations. _Science (New York, N.Y.), 317_(5837),
+482â487. https://doi.org/10.1126/science.1144581 * Hartmann, D., Guevara, M.
+R., Jara-Figueroa, C., AristarÃ¡n, M., & Hidalgo, C. A. (2017). Linking
+Economic Complexity, Institutions, and Income Inequality. _World Development_,
+93, 75â93. https://doi.org/10.1016/j.worlddev.2016.12.020 * Romero, J. P., &
+Gramkow, C. (2021). Economic complexity and greenhouse gas emissions. _World
+Development_, 139, 105317. https://doi.org/10.1016/j.worlddev.2020.105317 *
+Bahar, D., Hausmann, R., Hidalgo, C. A. (2014). Neighbors and the evolution of
+the comparative advantage of nations: Evidence of international knowledge
 diffusion?. _Journal of International Economics_, 92, 111-123. http://
-dx.doi.org/10.1016/j.jinteco.2013.11.001\n\n---\n© 2022 [Datawheel, LLC.]
-(https://www.datawheel.us/) \nThis project is licensed under [MIT](./
-LICENSE).\n', 'author': 'Jelmy Hermosilla', 'author_email':
-'jelmy@datawheel.us', 'maintainer': 'Francisco Abarzua', 'maintainer_email':
-'francisco@datawheel.us', 'url': 'https://github.com/Datawheel/py-economic-
-complexity', 'packages': packages, 'package_data': package_data,
-'install_requires': install_requires, 'python_requires': '>=3.7,<4.0', } setup
-(**setup_kwargs)
+dx.doi.org/10.1016/j.jinteco.2013.11.001 --- © 2022 [Datawheel, LLC.](https://
+www.datawheel.us/) This project is licensed under [MIT](./LICENSE).
```

