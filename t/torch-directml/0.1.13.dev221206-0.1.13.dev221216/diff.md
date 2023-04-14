# Comparing `tmp/torch_directml-0.1.13.dev221206-cp39-cp39-win_amd64.whl.zip` & `tmp/torch_directml-0.1.13.dev221216-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7494024 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat  1927168 b- defN 22-Dec-06 21:55 torch_directml_native.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat  9677208 b- defN 22-Dec-06 21:54 torch_directml/DirectML.dll
--rw-rw-rw-  2.0 fat      488 b- defN 22-Dec-06 21:46 torch_directml/__init__.py
--rw-rw-rw-  2.0 fat     1695 b- defN 22-Dec-06 21:46 torch_directml/device.py
--rw-rw-rw-  2.0 fat     6361 b- defN 22-Dec-06 21:46 torch_directml/csrc/auto_gen_yaml.py
--rw-rw-rw-  2.0 fat     1183 b- defN 22-Dec-06 21:55 torch_directml-0.1.13.dev221206.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4487 b- defN 22-Dec-06 21:55 torch_directml-0.1.13.dev221206.dist-info/METADATA
--rw-rw-rw-  2.0 fat    52853 b- defN 22-Dec-06 21:55 torch_directml-0.1.13.dev221206.dist-info/NOTICE
--rw-rw-rw-  2.0 fat      100 b- defN 22-Dec-06 21:55 torch_directml-0.1.13.dev221206.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       68 b- defN 22-Dec-06 21:55 torch_directml-0.1.13.dev221206.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1026 b- defN 22-Dec-06 21:55 torch_directml-0.1.13.dev221206.dist-info/RECORD
-11 files, 11672637 bytes uncompressed, 7492266 bytes compressed:  35.8%
+Zip file size: 7500654 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat  1939968 b- defN 22-Dec-16 16:27 torch_directml_native.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  9677208 b- defN 22-Dec-16 16:25 torch_directml/DirectML.dll
+-rw-rw-rw-  2.0 fat      488 b- defN 22-Dec-16 16:20 torch_directml/__init__.py
+-rw-rw-rw-  2.0 fat     1803 b- defN 22-Dec-16 16:20 torch_directml/device.py
+-rw-rw-rw-  2.0 fat     6361 b- defN 22-Dec-16 16:20 torch_directml/csrc/auto_gen_yaml.py
+-rw-rw-rw-  2.0 fat     1183 b- defN 22-Dec-16 16:27 torch_directml-0.1.13.dev221216.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4481 b- defN 22-Dec-16 16:27 torch_directml-0.1.13.dev221216.dist-info/METADATA
+-rw-rw-rw-  2.0 fat    52853 b- defN 22-Dec-16 16:27 torch_directml-0.1.13.dev221216.dist-info/NOTICE
+-rw-rw-rw-  2.0 fat      100 b- defN 22-Dec-16 16:27 torch_directml-0.1.13.dev221216.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       68 b- defN 22-Dec-16 16:27 torch_directml-0.1.13.dev221216.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1026 b- defN 22-Dec-16 16:27 torch_directml-0.1.13.dev221216.dist-info/RECORD
+11 files, 11685539 bytes uncompressed, 7498896 bytes compressed:  35.8%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: torch_directml/device.py
 Comment: 
 
 Filename: torch_directml/csrc/auto_gen_yaml.py
 Comment: 
 
-Filename: torch_directml-0.1.13.dev221206.dist-info/LICENSE
+Filename: torch_directml-0.1.13.dev221216.dist-info/LICENSE
 Comment: 
 
-Filename: torch_directml-0.1.13.dev221206.dist-info/METADATA
+Filename: torch_directml-0.1.13.dev221216.dist-info/METADATA
 Comment: 
 
-Filename: torch_directml-0.1.13.dev221206.dist-info/NOTICE
+Filename: torch_directml-0.1.13.dev221216.dist-info/NOTICE
 Comment: 
 
-Filename: torch_directml-0.1.13.dev221206.dist-info/WHEEL
+Filename: torch_directml-0.1.13.dev221216.dist-info/WHEEL
 Comment: 
 
-Filename: torch_directml-0.1.13.dev221206.dist-info/top_level.txt
+Filename: torch_directml-0.1.13.dev221216.dist-info/top_level.txt
 Comment: 
 
-Filename: torch_directml-0.1.13.dev221206.dist-info/RECORD
+Filename: torch_directml-0.1.13.dev221216.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torch_directml/device.py

```diff
@@ -36,9 +36,12 @@
         return torch_directml_native.custom_device(device_id)
     else:
         raise Exception(f"Invalid device_id argument supplied {device_id}. device_id must be in range [0, {num_devices}).")
 
 def disable_tiled_resources(is_disabled):
     torch_directml_native.disable_tiled_resources(is_disabled)
 
+def has_float64_support(is_disabled):
+    return torch_directml_native.has_float64_support(is_disabled)
+
 def gpu_memory(device_id = default_device(), mb_per_tile = 1):
     return torch_directml_native.get_gpu_memory(device_id, mb_per_tile)
```

## Comparing `torch_directml-0.1.13.dev221206.dist-info/LICENSE` & `torch_directml-0.1.13.dev221216.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torch_directml-0.1.13.dev221206.dist-info/METADATA` & `torch_directml-0.1.13.dev221216.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: torch-directml
-Version: 0.1.13.dev221206
-Summary: Torch DirectML extension backend.
+Version: 0.1.13.dev221216
+Summary: A DirectML backend for hardware acceleration in PyTorch.
 Home-page: https://github.com/microsoft/directml
 Author: Microsoft Corporation
 Author-email: askdirectml@microsoft.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/microsoft/directml/issues
 Keywords: pytorch,plugin,machine learning,directml,directx,d3d12
 Platform: UNKNOWN
@@ -36,18 +36,17 @@
 
 DirectML is a high-performance, hardware-accelerated DirectX 12 library for machine learning. DirectML provides GPU acceleration for common machine learning tasks across a broad range of supported hardware and drivers, including all DirectX 12-capable GPUs from vendors such as AMD, Intel, NVIDIA, and Qualcomm.
 
 More information about DirectML can be found in [Introduction to DirectML](https://docs.microsoft.com/windows/win32/direct3d12/dml-intro).
 
 PyTorch on DirectML is supported on both the latest versions of Windows 10 and the [Windows Subsystem for Linux](https://docs.microsoft.com/windows/wsl/about), and is available for download as a PyPI package. For more information about getting started, see [GPU accelerated ML training (docs.microsoft.com)](http://aka.ms/gpuinwsldocs)
 
-* [Samples](https://github.com/microsoft/DirectML/tree/master/PyTorch)
-* [Feedback](#feedback)
-* [Contributing](#contributing)
-* [External Links](#external-links)
+
+## Samples
+Refer to the [Pytorch with DirectML Samples Repo](https://github.com/microsoft/DirectML/tree/master/PyTorch) for samples. 
 
 ## Feedback
 
 We look forward to hearing from you!
 
 * For TensorFlow with DirectML issues, bugs, and feedback; or for general DirectML issues and feedback, please [file an issue](https://github.com/microsoft/DirectML-Samples/issues) or contact us directly at askdirectml@microsoft.com.
```

## Comparing `torch_directml-0.1.13.dev221206.dist-info/NOTICE` & `torch_directml-0.1.13.dev221216.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `torch_directml-0.1.13.dev221206.dist-info/RECORD` & `torch_directml-0.1.13.dev221216.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-torch_directml_native.cp39-win_amd64.pyd,sha256=CmwxPeT03BeqUT9rmN5GaBsFIpJIhqhQ2I9omUCCTr0,1927168
+torch_directml_native.cp39-win_amd64.pyd,sha256=9nIKCEKIOy47IUll-iohS2dziWKXuw0Z0OVGT5iDK10,1939968
 torch_directml/DirectML.dll,sha256=vDRFEq8PI6vrxiipnWAZ3AIcaLeLzBsuqpEpVs9-hYU,9677208
 torch_directml/__init__.py,sha256=4Os9AFoEAHfHNaKGgPy-ENnReRjCYQezn-msfKzYSAE,488
-torch_directml/device.py,sha256=mLBqRaWnTnNolo4aT724dnhAFaUwdvx8zaqdikfwT0Q,1695
+torch_directml/device.py,sha256=vScHJtGXmBJ7FReLP01zuvC4yvi_0kt8oxKH-PZ1s4c,1803
 torch_directml/csrc/auto_gen_yaml.py,sha256=fknASwduV7qdgQqp1zJFAz3v_UF0TsuEKLQSIg8wT1Y,6361
-torch_directml-0.1.13.dev221206.dist-info/LICENSE,sha256=3qkmU0GCkALiwjpzcjk-su1uJghftiPzikugr4M_MKY,1183
-torch_directml-0.1.13.dev221206.dist-info/METADATA,sha256=vFNS6WmCI74nvpv03-tdksOoqd_HpkI_FeFhZgNvmQE,4487
-torch_directml-0.1.13.dev221206.dist-info/NOTICE,sha256=4uO665QNJMTrFu7L4zL6lMvFQtAMTDbS9GYOal1F3mY,52853
-torch_directml-0.1.13.dev221206.dist-info/WHEEL,sha256=J_4V_gB-O6Y7Pn6lk91K27JaIhI-q07YM5J8Ufzqla4,100
-torch_directml-0.1.13.dev221206.dist-info/top_level.txt,sha256=fh-ZIpP9HQt22AqW8TqQNRlz9mx43devjQy7IV9tGEw,68
-torch_directml-0.1.13.dev221206.dist-info/RECORD,,
+torch_directml-0.1.13.dev221216.dist-info/LICENSE,sha256=3qkmU0GCkALiwjpzcjk-su1uJghftiPzikugr4M_MKY,1183
+torch_directml-0.1.13.dev221216.dist-info/METADATA,sha256=Eq53rwMONR4x4aTkCDUp4oqglhoPd44X1ohhrCS2jZo,4481
+torch_directml-0.1.13.dev221216.dist-info/NOTICE,sha256=4uO665QNJMTrFu7L4zL6lMvFQtAMTDbS9GYOal1F3mY,52853
+torch_directml-0.1.13.dev221216.dist-info/WHEEL,sha256=J_4V_gB-O6Y7Pn6lk91K27JaIhI-q07YM5J8Ufzqla4,100
+torch_directml-0.1.13.dev221216.dist-info/top_level.txt,sha256=fh-ZIpP9HQt22AqW8TqQNRlz9mx43devjQy7IV9tGEw,68
+torch_directml-0.1.13.dev221216.dist-info/RECORD,,
```

