# Comparing `tmp/NewareNDA-2023.2.1.post1-py3-none-any.whl.zip` & `tmp/NewareNDA-2023.4.14-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6297 bytes, number of entries: 9
--rw-rw-r--  2.0 unx     7671 b- defN 23-Feb-02 18:25 NewareNDA/NewareNDA.py
+Zip file size: 6276 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx     7403 b- defN 23-Apr-14 13:45 NewareNDA/NewareNDA.py
 -rw-rw-r--  2.0 unx       61 b- defN 22-Sep-06 14:02 NewareNDA/__init__.py
--rw-rw-r--  2.0 unx       34 b- defN 23-Feb-07 17:13 NewareNDA/version.py
--rwxrwxr-x  2.0 unx     1189 b- defN 23-Feb-07 17:13 NewareNDA-2023.2.1.post1.data/scripts/NewareNDA-cli.py
--rw-rw-r--  2.0 unx     1488 b- defN 23-Feb-07 17:13 NewareNDA-2023.2.1.post1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      852 b- defN 23-Feb-07 17:13 NewareNDA-2023.2.1.post1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Feb-07 17:13 NewareNDA-2023.2.1.post1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Feb-07 17:13 NewareNDA-2023.2.1.post1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      781 b- defN 23-Feb-07 17:13 NewareNDA-2023.2.1.post1.dist-info/RECORD
-9 files, 12178 bytes uncompressed, 4929 bytes compressed:  59.5%
+-rw-rw-r--  2.0 unx       28 b- defN 23-Apr-14 13:47 NewareNDA/version.py
+-rwxrwxr-x  2.0 unx     1189 b- defN 23-Apr-14 14:03 NewareNDA-2023.4.14.data/scripts/NewareNDA-cli.py
+-rw-rw-r--  2.0 unx     1488 b- defN 23-Apr-14 14:03 NewareNDA-2023.4.14.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      919 b- defN 23-Apr-14 14:03 NewareNDA-2023.4.14.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-14 14:03 NewareNDA-2023.4.14.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Apr-14 14:03 NewareNDA-2023.4.14.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      751 b- defN 23-Apr-14 14:03 NewareNDA-2023.4.14.dist-info/RECORD
+9 files, 11941 bytes uncompressed, 4968 bytes compressed:  58.4%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: NewareNDA/__init__.py
 Comment: 
 
 Filename: NewareNDA/version.py
 Comment: 
 
-Filename: NewareNDA-2023.2.1.post1.data/scripts/NewareNDA-cli.py
+Filename: NewareNDA-2023.4.14.data/scripts/NewareNDA-cli.py
 Comment: 
 
-Filename: NewareNDA-2023.2.1.post1.dist-info/LICENSE
+Filename: NewareNDA-2023.4.14.dist-info/LICENSE
 Comment: 
 
-Filename: NewareNDA-2023.2.1.post1.dist-info/METADATA
+Filename: NewareNDA-2023.4.14.dist-info/METADATA
 Comment: 
 
-Filename: NewareNDA-2023.2.1.post1.dist-info/WHEEL
+Filename: NewareNDA-2023.4.14.dist-info/WHEEL
 Comment: 
 
-Filename: NewareNDA-2023.2.1.post1.dist-info/top_level.txt
+Filename: NewareNDA-2023.4.14.dist-info/top_level.txt
 Comment: 
 
-Filename: NewareNDA-2023.2.1.post1.dist-info/RECORD
+Filename: NewareNDA-2023.4.14.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## NewareNDA/NewareNDA.py

```diff
@@ -11,14 +11,70 @@
 # Names for data fields
 rec_columns = [
     'Index', 'Cycle', 'Step', 'Status', 'Time', 'Voltage',
     'Current(mA)', 'Charge_Capacity(mAh)', 'Discharge_Capacity(mAh)',
     'Charge_Energy(mWh)', 'Discharge_Energy(mWh)', 'Timestamp']
 aux_columns = ['Index', 'Aux', 'T']
 
+# Define precision of fields
+dtype_dict = {
+    'Index': 'uint32',
+    'Cycle': 'uint16',
+    'Step': 'uint32',
+    'Status': 'category',
+    'Time': 'float32',
+    'Voltage': 'float32',
+    'Current(mA)': 'float32',
+    'Charge_Capacity(mAh)': 'float32',
+    'Discharge_Capacity(mAh)': 'float32',
+    'Charge_Energy(mWh)': 'float32',
+    'Discharge_Energy(mWh)': 'float32'
+}
+
+# Dictionary mapping Status integer to string
+state_dict = {
+    1: 'CC_Chg',
+    2: 'CC_DChg',
+    3: 'CV_Chg',
+    4: 'Rest',
+    5: 'Cycle',
+    7: 'CCCV_Chg',
+    10: 'CR_DChg',
+    13: 'Pause',
+    17: 'SIM',
+    19: 'CV_DChg',
+    20: 'CCCV_DChg'
+}
+
+# Define field scaling based on instrument Range setting
+multiplier_dict = {
+    -200000: 1e-2,
+    -100000: 1e-2,
+    -60000: 1e-2,
+    -30000: 1e-2,
+    -50000: 1e-2,
+    -20000: 1e-2,
+    -10000: 1e-2,
+    -6000: 1e-2,
+    -5000: 1e-2,
+    -3000: 1e-2,
+    -1000: 1e-2,
+    -500: 1e-3,
+    -100: 1e-3,
+    0: 0,
+    10: 1e-3,
+    100: 1e-2,
+    200: 1e-2,
+    1000: 1e-1,
+    6000: 1e-1,
+    12000: 1e-1,
+    50000: 1e-1,
+    60000: 1e-1,
+}
+
 
 def read(file):
     """
     Function read electrochemical data from a Neware nda binary file.
 
     Args:
         file (str): Name of a .nda file to read
@@ -84,111 +140,58 @@
 
     df.reset_index(drop=True, inplace=True)
 
     # Join temperature data
     aux_df = pd.DataFrame(aux, columns=aux_columns)
     aux_df.drop_duplicates(inplace=True)
     if not aux_df.empty:
-        for Aux in aux_df.Aux.unique():
-            df = df.join(aux_df.loc[aux_df.Aux == Aux, 'T'])
-            df.rename(columns={'T': f"T{Aux}"}, inplace=True)
+        pvt_df = aux_df.pivot(index='Index', columns='Aux', values='T')
+        for k in pvt_df.keys():
+            pvt_df.rename(columns={k: f"T{k}"}, inplace=True)
+        df = df.join(pvt_df, on='Index')
 
     # Postprocessing
     df.Step = _count_changes(df.Step)
     df.Cycle = _generate_cycle_number(df)
-
-    # Define precision of fields
-    dtype_dict = {
-        'Index': 'uint32',
-        'Cycle': 'uint16',
-        'Step': 'uint32',
-        'Status': 'category',
-        'Time': 'float32',
-        'Voltage': 'float32',
-        'Current(mA)': 'float32',
-        'Charge_Capacity(mAh)': 'float32',
-        'Discharge_Capacity(mAh)': 'float32',
-        'Charge_Energy(mWh)': 'float32',
-        'Discharge_Energy(mWh)': 'float32'
-    }
     df = df.astype(dtype=dtype_dict)
 
-    return(df)
+    return df
 
 
 def _valid_record(bytes):
     """Helper function to identify a valid record"""
     # Check for a non-zero Status
     [Status] = struct.unpack('<B', bytes[12:13])
-    return(Status != 0)
+    return (Status != 0)
 
 
 def _bytes_to_list(bytes):
     """Helper function for interpreting a byte string"""
-    # Dictionary mapping Status integer to string
-    state_dict = {
-        1: 'CC_Chg',
-        2: 'CC_DChg',
-        3: 'CV_Chg',
-        4: 'Rest',
-        5: 'Cycle',
-        7: 'CCCV_Chg',
-        10: 'CR_DChg',
-        13: 'Pause',
-        17: 'SIM',
-        19: 'CV_DChg',
-        20: 'CCCV_DChg'
-    }
 
     # Extract fields from byte string
     [Index, Cycle] = struct.unpack('<IB', bytes[2:7])
     [Step] = struct.unpack('<I', bytes[10:14])
     [Status, Jump, Time] = struct.unpack('<BBQ', bytes[12:22])
     [Voltage, Current] = struct.unpack('<ii', bytes[22:30])
     [Charge_capacity, Discharge_capacity] = struct.unpack('<qq', bytes[38:54])
     [Charge_energy, Discharge_energy] = struct.unpack('<qq', bytes[54:70])
     [Y, M, D, h, m, s] = struct.unpack('<HBBBBB', bytes[70:77])
     [Range] = struct.unpack('<i', bytes[78:82])
 
     # Index should not be zero
     if Index == 0:
-        return([])
+        return []
 
     # Convert date to datetime. Try Unix timestamp on failure.
     try:
         Date = datetime(Y, M, D, h, m, s)
     except ValueError:
         [Timestamp] = struct.unpack('<Q', bytes[70:78])
         Date = datetime.fromtimestamp(Timestamp)
 
-    # Define field scaling based on instrument Range setting
-    multiplier_dict = {
-        -200000: 1e-2,
-        -100000: 1e-2,
-        -60000: 1e-2,
-        -30000: 1e-2,
-        -50000: 1e-2,
-        -20000: 1e-2,
-        -10000: 1e-2,
-        -6000: 1e-2,
-        -5000: 1e-2,
-        -3000: 1e-2,
-        -1000: 1e-2,
-        -500: 1e-3,
-        -100: 1e-3,
-        0: 0,
-        10: 1e-3,
-        100: 1e-2,
-        200: 1e-2,
-        1000: 1e-1,
-        6000: 1e-1,
-        12000: 1e-1,
-        50000: 1e-1,
-        60000: 1e-1,
-    }
     multiplier = multiplier_dict[Range]
 
     # Create a dictionary for the record
     list = [
         Index,
         Cycle + 1,
         Step,
@@ -198,30 +201,23 @@
         Current*multiplier,
         Charge_capacity*multiplier/3600,
         Discharge_capacity*multiplier/3600,
         Charge_energy*multiplier/3600,
         Discharge_energy*multiplier/3600,
         Date
     ]
-    return(list)
+    return list
 
 
 def _aux_bytes_to_list(bytes):
     """Helper function for intepreting auxiliary records"""
-    [Aux] = struct.unpack('<B', bytes[1:2])
-    [Index, Cycle] = struct.unpack('<IB', bytes[2:7])
+    [Aux, Index] = struct.unpack('<BI', bytes[1:6])
     [T] = struct.unpack('<h', bytes[34:36])
 
-    list = [
-        Index,
-        Aux,
-        T/10
-    ]
-
-    return(list)
+    return [Index, Aux, T/10]
 
 
 def _generate_cycle_number(df):
     """
     Generate a cycle number to match Neware. A new cycle starts with a charge
     step after there has previously been a discharge.
     """
@@ -242,16 +238,16 @@
         if chg[n] & dchg:
             cyc += 1
             dchg = False
         elif 'DChg' in status[n] or status[n] == 'SIM':
             dchg = True
         chg[n] = cyc
 
-    return(chg)
+    return chg
 
 
 def _count_changes(series):
     """Enumerate the number of value changes in a series"""
     a = series.diff()
     a.iloc[0] = 1
     a.iloc[-1] = 0
-    return((abs(a) > 0).cumsum())
+    return (abs(a) > 0).cumsum()
```

## NewareNDA/version.py

```diff
@@ -1 +1 @@
-__version__ = 'v2023.02.01.post1'
+__version__ = 'v2023.04.14'
```

## Comparing `NewareNDA-2023.2.1.post1.data/scripts/NewareNDA-cli.py` & `NewareNDA-2023.4.14.data/scripts/NewareNDA-cli.py`

 * *Files identical despite different names*

## Comparing `NewareNDA-2023.2.1.post1.dist-info/LICENSE` & `NewareNDA-2023.4.14.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `NewareNDA-2023.2.1.post1.dist-info/METADATA` & `NewareNDA-2023.4.14.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NewareNDA
-Version: 2023.2.1.post1
+Version: 2023.4.14
 Summary: Neware nda binary file reader.
 Home-page: https://github.com/Solid-Energy-Systems/NewareNDA
 Author: Daniel Cogswell
 Author-email: danielcogswell@ses.ai
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
@@ -14,15 +14,15 @@
 
 # NewareNDA
 
 © 2023 Copyright SES AI
 <br>Author: Daniel Cogswell
 <br>Email: danielcogswell@ses.ai
 
-Neware NDA binary file reader.
+Python module and Bash command line tool for reading and converting Neware .nda battery cycling files.
 
 # Installation
 ```
 cd NewareNDA
 pip install .
 ```
```

## Comparing `NewareNDA-2023.2.1.post1.dist-info/RECORD` & `NewareNDA-2023.4.14.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-NewareNDA/NewareNDA.py,sha256=3sbU7KG9Ixl12f7Jy6UqBSnwVHR5f3rDJ-7rlXBP4ec,7671
+NewareNDA/NewareNDA.py,sha256=ROuoZ2hcHEAKBpueQhRTcsSYpeR0oA9jVoBCfgYv5xk,7403
 NewareNDA/__init__.py,sha256=HcIL21PU-NmBDfuzsk6zzOsoq_GIgFwU86JYhHUUxVY,61
-NewareNDA/version.py,sha256=EpTENsFC8lWPnAL2cfJMZuYJVt-cqUMlskJLW0Xcoas,34
-NewareNDA-2023.2.1.post1.data/scripts/NewareNDA-cli.py,sha256=lKzHAUSqfmxorAo-qRKZikdgW6B-kJ-ePq3YVdR5qno,1189
-NewareNDA-2023.2.1.post1.dist-info/LICENSE,sha256=AGY-bfMClgUyCBsA_w4IMlP5G018QfjCPfSGgHOrF3Y,1488
-NewareNDA-2023.2.1.post1.dist-info/METADATA,sha256=5N50LzCd6lE2DHnCcO92tpNHf52GtPSKYQVpg-hLIQs,852
-NewareNDA-2023.2.1.post1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-NewareNDA-2023.2.1.post1.dist-info/top_level.txt,sha256=TrIpR_dGmBO9hgO5ZtJ2_09-dx4Q1x3iieFIJ2ZbIa4,10
-NewareNDA-2023.2.1.post1.dist-info/RECORD,,
+NewareNDA/version.py,sha256=LrufNtHNcWr2xPkf2tZ2uoA4oWKI-847_Z2cSdiIz0Q,28
+NewareNDA-2023.4.14.data/scripts/NewareNDA-cli.py,sha256=lKzHAUSqfmxorAo-qRKZikdgW6B-kJ-ePq3YVdR5qno,1189
+NewareNDA-2023.4.14.dist-info/LICENSE,sha256=AGY-bfMClgUyCBsA_w4IMlP5G018QfjCPfSGgHOrF3Y,1488
+NewareNDA-2023.4.14.dist-info/METADATA,sha256=M4xT88AaEa2C4lD0j8nyiNi-RAKjtCvtgZ9NlaLGueE,919
+NewareNDA-2023.4.14.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+NewareNDA-2023.4.14.dist-info/top_level.txt,sha256=TrIpR_dGmBO9hgO5ZtJ2_09-dx4Q1x3iieFIJ2ZbIa4,10
+NewareNDA-2023.4.14.dist-info/RECORD,,
```

