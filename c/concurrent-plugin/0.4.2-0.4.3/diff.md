# Comparing `tmp/concurrent_plugin-0.4.2-py3-none-any.whl.zip` & `tmp/concurrent_plugin-0.4.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 30813 bytes, number of entries: 18
+Zip file size: 30856 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx        2 b- defN 22-Nov-27 22:37 concurrent_plugin/__init__.py
--rw-rw-r--  2.0 unx    31658 b- defN 23-Apr-13 18:25 concurrent_plugin/concurrent_backend.py
+-rw-rw-r--  2.0 unx    31831 b- defN 23-Apr-14 15:37 concurrent_plugin/concurrent_backend.py
 -rw-rw-r--  2.0 unx    16820 b- defN 22-Dec-17 04:51 concurrent_plugin/concurrent_core.py
 -rw-rw-r--  2.0 unx    15759 b- defN 23-Feb-15 23:54 concurrent_plugin/login.py
 -rw-rw-r--  2.0 unx     3994 b- defN 22-Dec-20 19:35 concurrent_plugin/periodic_run.py
 -rw-rw-r--  2.0 unx     1298 b- defN 23-Jan-19 23:36 concurrent_plugin/periodic_run_utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/__init__.py
 -rw-rw-r--  2.0 unx      990 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infin_download.py
 -rw-rw-r--  2.0 unx     1339 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infin_prefetch.py
 -rw-rw-r--  2.0 unx    10783 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infinfs.py
 -rw-rw-r--  2.0 unx     5326 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/infinmount.py
 -rw-rw-r--  2.0 unx     1140 b- defN 22-Nov-27 22:37 concurrent_plugin/infinfs/mount_main.py
 -rw-rw-r--  2.0 unx    15276 b- defN 23-Apr-09 17:20 concurrent_plugin/infinfs/mount_service.py
--rw-rw-r--  2.0 unx      205 b- defN 23-Apr-13 18:27 concurrent_plugin-0.4.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-13 18:27 concurrent_plugin-0.4.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx      182 b- defN 23-Apr-13 18:27 concurrent_plugin-0.4.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       18 b- defN 23-Apr-13 18:27 concurrent_plugin-0.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1663 b- defN 23-Apr-13 18:27 concurrent_plugin-0.4.2.dist-info/RECORD
-18 files, 106545 bytes uncompressed, 28025 bytes compressed:  73.7%
+-rw-rw-r--  2.0 unx      205 b- defN 23-Apr-14 16:33 concurrent_plugin-0.4.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Apr-14 16:33 concurrent_plugin-0.4.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      182 b- defN 23-Apr-14 16:33 concurrent_plugin-0.4.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       18 b- defN 23-Apr-14 16:33 concurrent_plugin-0.4.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1663 b- defN 23-Apr-14 16:33 concurrent_plugin-0.4.3.dist-info/RECORD
+18 files, 106718 bytes uncompressed, 28068 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -33,23 +33,23 @@
 
 Filename: concurrent_plugin/infinfs/mount_main.py
 Comment: 
 
 Filename: concurrent_plugin/infinfs/mount_service.py
 Comment: 
 
-Filename: concurrent_plugin-0.4.2.dist-info/METADATA
+Filename: concurrent_plugin-0.4.3.dist-info/METADATA
 Comment: 
 
-Filename: concurrent_plugin-0.4.2.dist-info/WHEEL
+Filename: concurrent_plugin-0.4.3.dist-info/WHEEL
 Comment: 
 
-Filename: concurrent_plugin-0.4.2.dist-info/entry_points.txt
+Filename: concurrent_plugin-0.4.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: concurrent_plugin-0.4.2.dist-info/top_level.txt
+Filename: concurrent_plugin-0.4.3.dist-info/top_level.txt
 Comment: 
 
-Filename: concurrent_plugin-0.4.2.dist-info/RECORD
+Filename: concurrent_plugin-0.4.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## concurrent_plugin/concurrent_backend.py

```diff
@@ -613,16 +613,18 @@
         volume_mounts.append(kubernetes.client.V1VolumeMount(mount_path=CONCURRENT_FUSE_MOUNT_BASE,
                                                              name='sharedmount',
                                                              mount_propagation='HostToContainer'))
         side_car_volume_mounts.append(kubernetes.client.V1VolumeMount(mount_path=CONCURRENT_FUSE_MOUNT_BASE,
                                                     name='sharedmount',
                                                     mount_propagation='Bidirectional'))
 
+        job_template["spec"]["ttlSecondsAfterFinished"] = 600
         job_template["spec"]["template"]["spec"]["containers"][0]["volumeMounts"] = volume_mounts
-        job_template["spec"]["template"]["spec"]["containers"][1]["volumeMounts"] = side_car_volume_mounts
+        if len(job_template["spec"]["template"]["spec"]["containers"]) > 1: # sidecar container is present
+            job_template["spec"]["template"]["spec"]["containers"][1]["volumeMounts"] = side_car_volume_mounts
 
         job_template["spec"]["template"]["spec"]["serviceAccountName"] = 'k8s-serviceaccount-for-users-' + job_namespace
 
         job_template["spec"]["template"]["spec"]["volumes"] = [
                     kubernetes.client.V1Volume(name="parallels-token-file", secret=kubernetes.client.V1SecretVolumeSource(secret_name=token_secret_name)),
                     kubernetes.client.V1Volume(name="aws-creds-file", secret=kubernetes.client.V1SecretVolumeSource(secret_name=awscreds_secret_name)),
                     kubernetes.client.V1Volume(name='sharedmount', empty_dir=kubernetes.client.V1EmptyDirVolumeSource())
```

## Comparing `concurrent_plugin-0.4.2.dist-info/RECORD` & `concurrent_plugin-0.4.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 concurrent_plugin/__init__.py,sha256=4W8VliAYUP1KY2gLJ_YDy2TmcXYVm-PY7XikQD_bFwA,2
-concurrent_plugin/concurrent_backend.py,sha256=u8iTg8RKtpvkoZPPXtvFyQRST4PzetQsfMJjT1CrI6M,31658
+concurrent_plugin/concurrent_backend.py,sha256=tMviGg7scbSSVnVcCj3F_2Pby8f7TxZBmYT77J7u7B0,31831
 concurrent_plugin/concurrent_core.py,sha256=ECXT0b11j8L5kgWAxxyW6gg6gUK9d_TGOf_AibCb27k,16820
 concurrent_plugin/login.py,sha256=yBdoKr_9Uiq4DFPHmQjJEBGS61F2fw79QIL8c3hy5Vg,15759
 concurrent_plugin/periodic_run.py,sha256=Ud66-3AtnonAO6oOhcn2EwJQPfbljcrlCQeR23ELH1c,3994
 concurrent_plugin/periodic_run_utils.py,sha256=MZuX9uSFEuA7B8UFDAchsrWhidXT5QyuOA-GDtzIPOo,1298
 concurrent_plugin/infinfs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 concurrent_plugin/infinfs/infin_download.py,sha256=6yILg2brDNDNMFGqayFHIshB4cl25byn5dal0QI7JKQ,990
 concurrent_plugin/infinfs/infin_prefetch.py,sha256=ICqCHaiugg0z_gm4cMpQGJHozSXuf54kAw97g4yAhGU,1339
 concurrent_plugin/infinfs/infinfs.py,sha256=3xId2Ocp7UJv7ntBgpr-KCFv5wGJQFw2m8csamIHiYY,10783
 concurrent_plugin/infinfs/infinmount.py,sha256=Y9BPuggy0P9gz-kYH2ZhLy24Z1WTsw7GgU3rgH7JSsY,5326
 concurrent_plugin/infinfs/mount_main.py,sha256=ehL8zXZ1HRviaukp753TjJ6pFCtO9uUfUIjx8yfUHVE,1140
 concurrent_plugin/infinfs/mount_service.py,sha256=y2vNoDpEXLm95ch_GDhnVNF7oXf8I9fvQZhjc_JNcX4,15276
-concurrent_plugin-0.4.2.dist-info/METADATA,sha256=bwxXwlbkanwtMdpB9j0ofqdOwYaFiwTw1JO0_ArJ1jc,205
-concurrent_plugin-0.4.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-concurrent_plugin-0.4.2.dist-info/entry_points.txt,sha256=5bYsI3RSqBvAjlcOeCbKKIRorBotB8wvo1p4Xfn3tXY,182
-concurrent_plugin-0.4.2.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
-concurrent_plugin-0.4.2.dist-info/RECORD,,
+concurrent_plugin-0.4.3.dist-info/METADATA,sha256=A8pr78vzCnrcnu8NArR-v0oa68Wejq6FFXI33d3P_uQ,205
+concurrent_plugin-0.4.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+concurrent_plugin-0.4.3.dist-info/entry_points.txt,sha256=5bYsI3RSqBvAjlcOeCbKKIRorBotB8wvo1p4Xfn3tXY,182
+concurrent_plugin-0.4.3.dist-info/top_level.txt,sha256=rMkubPHW5GESfE5gDfsycyj3TWUOusZRYPD2lwoggcg,18
+concurrent_plugin-0.4.3.dist-info/RECORD,,
```

