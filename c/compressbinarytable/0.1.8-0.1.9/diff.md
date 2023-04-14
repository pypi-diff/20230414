# Comparing `tmp/compressbinarytable-0.1.8.tar.gz` & `tmp/compressbinarytable-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compressbinarytable-0.1.8.tar", max compression
+gzip compressed data, was "compressbinarytable-0.1.9.tar", max compression
```

## Comparing `compressbinarytable-0.1.8.tar` & `compressbinarytable-0.1.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1125 2023-04-14 12:56:55.183428 compressbinarytable-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-04-14 10:19:30.058694 compressbinarytable-0.1.8/compressbinarytable/__init__.py
--rw-r--r--   0        0        0     7810 2023-04-14 12:41:35.548262 compressbinarytable-0.1.8/compressbinarytable/compressbinarytable.py
--rw-r--r--   0        0        0      625 2023-04-14 12:58:44.122244 compressbinarytable-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1786 1970-01-01 00:00:00.000000 compressbinarytable-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1113 2023-04-14 14:14:27.887908 compressbinarytable-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-04-14 10:19:30.058694 compressbinarytable-0.1.9/compressbinarytable/__init__.py
+-rw-r--r--   0        0        0     7780 2023-04-14 14:16:55.244395 compressbinarytable-0.1.9/compressbinarytable/compressbinarytable.py
+-rw-r--r--   0        0        0      675 2023-04-14 14:17:50.925130 compressbinarytable-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 compressbinarytable-0.1.9/PKG-INFO
```

### Comparing `compressbinarytable-0.1.8/README.md` & `compressbinarytable-0.1.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,63 @@
 # CompressBinaryTable
  
 ## Basic Usage:
 
 ```console
-
 cbt -i input_file -o output_file -c 
-
 ```
 
 ## Options:
 
 ```console
-
 -i = input, required 
 -o = output, required 
 -c = compression 
 -d = decompression 
 -t = output type, either csv or tsv 
 --override = to override output file if it exist 
-
 ```
 
 ## Available Python functions:
 
 ```
-
 # Returns numpy array of file as uncompressed, useful for ML (same as load as pandas df, and to_numpy())
 cbt_to_array(compressed_file)
 
 # Returns numpy array of name of the mutations as uncompressed, useful for ML, (same as load pandas df and use df.colums)
 cbt_columns(compressed_file)
-
 ```
 
 ## Required file example:
 
 ### CSV:
 
 ```
-
 strain_name,mut1,mut2,mut3,mut4,outcome
 strain1,0,1,1,1,1,1
 strain2,0,0,1,1,1,0
 strain3,0,1,0,1,1,0
 strain4,1,1,1,1,1,1
-
 ```
 
 ### TSV:
 
 ```
-
 strain_name mut1    mut2    mut3    mut4    outcome
 strain1 0   1   1   1   1   1
 strain2 0   0   1   1   1   0
 strain3 0   1   0   1   1   0
 strain4 1   1   1   1   1   1
-
 ```
 
 ### CBT:
 
 ```
-
 1;mut1;mut2;mut3;mut4;outcome
 strain1;6;43;87;102
 strain2;16;43;87;102
 strain3;6;53;78;112
 strain4;61;413;824;942
-
 ```
```

### Comparing `compressbinarytable-0.1.8/compressbinarytable/compressbinarytable.py` & `compressbinarytable-0.1.9/compressbinarytable/compressbinarytable.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
     
     return dictionary_of_strains_data, columns, selection
 
 
 # Writes compressed file into outfile 
 def compressed_file_writer(outfile, dictionary_of_strains_data, columns, selection):
 
-    if outfile_name.endswith(".cbt"):
-        outfile_name = outfile_name[:-4]
+    if outfile.endswith(".cbt"):
+        outfile = outfile[:-4]
 
     with open(outfile + ".cbt", "w") as compressed_file:
         compressed_file.write(str(selection))
         for col in columns[1:]:
             compressed_file.write(";" + str(col))
         compressed_file.write("\n")
 
@@ -224,15 +224,15 @@
     return return_array 
 
 
 def main():
 
     # Main function to call from command line
 
-    parser = argparse.ArgumentParser(description='Compression of Binary Mutation Tables')
+    parser = argparse.ArgumentParser(description='Compression of Binary Tables')
 
     parser.add_argument("-c", help="Compression flag", action="store_true")
 
     parser.add_argument("-d", help="Decompression flag", action="store_true")
 
     parser.add_argument("-i", help="Path of input file", required=True)
 
@@ -286,13 +286,11 @@
 
         exit()
     
     else:
         print("You need to select either Compression -c or Decompression -d")
         exit()
 
-    
-
  
 if __name__ == "__main__":
     main()
```

### Comparing `compressbinarytable-0.1.8/pyproject.toml` & `compressbinarytable-0.1.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "compressbinarytable"
-version = "0.1.8"
-repository = ""
+version = "0.1.9"
+repository = "https://github.com/kalininalab/CompressBinaryTable"
 readme = "README.md"
 description = "Compression of binary table"
 authors = ["Alper Yurtseven <alper.yurtseven@helmholtz-hips.de>"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Operating System :: OS Independent"
 ]
```

### Comparing `compressbinarytable-0.1.8/PKG-INFO` & `compressbinarytable-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,94 +1,84 @@
 Metadata-Version: 2.1
 Name: compressbinarytable
-Version: 0.1.8
+Version: 0.1.9
 Summary: Compression of binary table
+Home-page: https://github.com/kalininalab/CompressBinaryTable
 Author: Alper Yurtseven
 Author-email: alper.yurtseven@helmholtz-hips.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.21.4,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Project-URL: Repository, https://github.com/kalininalab/CompressBinaryTable
 Description-Content-Type: text/markdown
 
 # CompressBinaryTable
  
 ## Basic Usage:
 
 ```console
-
 cbt -i input_file -o output_file -c 
-
 ```
 
 ## Options:
 
 ```console
-
 -i = input, required 
 -o = output, required 
 -c = compression 
 -d = decompression 
 -t = output type, either csv or tsv 
 --override = to override output file if it exist 
-
 ```
 
 ## Available Python functions:
 
 ```
-
 # Returns numpy array of file as uncompressed, useful for ML (same as load as pandas df, and to_numpy())
 cbt_to_array(compressed_file)
 
 # Returns numpy array of name of the mutations as uncompressed, useful for ML, (same as load pandas df and use df.colums)
 cbt_columns(compressed_file)
-
 ```
 
 ## Required file example:
 
 ### CSV:
 
 ```
-
 strain_name,mut1,mut2,mut3,mut4,outcome
 strain1,0,1,1,1,1,1
 strain2,0,0,1,1,1,0
 strain3,0,1,0,1,1,0
 strain4,1,1,1,1,1,1
-
 ```
 
 ### TSV:
 
 ```
-
 strain_name mut1    mut2    mut3    mut4    outcome
 strain1 0   1   1   1   1   1
 strain2 0   0   1   1   1   0
 strain3 0   1   0   1   1   0
 strain4 1   1   1   1   1   1
-
 ```
 
 ### CBT:
 
 ```
-
 1;mut1;mut2;mut3;mut4;outcome
 strain1;6;43;87;102
 strain2;16;43;87;102
 strain3;6;53;78;112
 strain4;61;413;824;942
-
 ```
```

