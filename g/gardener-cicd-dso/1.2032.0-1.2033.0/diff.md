# Comparing `tmp/gardener-cicd-dso-1.2032.0.tar.gz` & `tmp/gardener-cicd-dso-1.2033.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-dso-1.2032.0.tar", last modified: Wed Apr 12 12:34:12 2023, max compression
+gzip compressed data, was "gardener-cicd-dso-1.2033.0.tar", last modified: Fri Apr 14 08:39:48 2023, max compression
```

## Comparing `gardener-cicd-dso-1.2032.0.tar` & `gardener-cicd-dso-1.2033.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:34:12.976354 gardener-cicd-dso-1.2032.0/
--rw-r--r--   0 root         (0) root         (0)    16830 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/NOTICE.md
--rw-r--r--   0 root         (0) root         (0)      171 2023-04-12 12:34:12.976354 gardener-cicd-dso-1.2032.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:34:12.972353 gardener-cicd-dso-1.2032.0/checkmarx/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/checkmarx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7623 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/checkmarx/client.py
--rw-r--r--   0 root         (0) root         (0)     3746 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/checkmarx/model.py
--rw-r--r--   0 root         (0) root         (0)     7006 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/checkmarx/project.py
--rw-r--r--   0 root         (0) root         (0)     5790 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/checkmarx/tablefmt.py
--rw-r--r--   0 root         (0) root         (0)    17856 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/checkmarx/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:34:12.972353 gardener-cicd-dso-1.2032.0/clamav/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/clamav/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5287 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/clamav/client.py
--rw-r--r--   0 root         (0) root         (0)     5266 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/clamav/cnudie.py
--rw-r--r--   0 root         (0) root         (0)     2417 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/clamav/model.py
--rw-r--r--   0 root         (0) root         (0)     1339 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/clamav/report.py
--rw-r--r--   0 root         (0) root         (0)     1690 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/clamav/routes.py
--rw-r--r--   0 root         (0) root         (0)     7689 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/clamav/scan.py
--rw-r--r--   0 root         (0) root         (0)     6135 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/clamav/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:34:12.972353 gardener-cicd-dso-1.2032.0/gardener_cicd_dso.egg-info/
--rw-r--r--   0 root         (0) root         (0)      171 2023-04-12 12:34:12.000000 gardener-cicd-dso-1.2032.0/gardener_cicd_dso.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      688 2023-04-12 12:34:12.000000 gardener-cicd-dso-1.2032.0/gardener_cicd_dso.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-12 12:34:12.000000 gardener-cicd-dso-1.2032.0/gardener_cicd_dso.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-12 12:34:12.000000 gardener-cicd-dso-1.2032.0/gardener_cicd_dso.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-04-12 12:34:12.000000 gardener-cicd-dso-1.2032.0/gardener_cicd_dso.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-12 12:34:12.976354 gardener-cicd-dso-1.2032.0/protecode/
--rw-r--r--   0 root         (0) root         (0)      740 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/protecode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5756 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/protecode/assessments.py
--rw-r--r--   0 root         (0) root         (0)    17050 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/protecode/client.py
--rw-r--r--   0 root         (0) root         (0)    11985 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/protecode/model.py
--rw-r--r--   0 root         (0) root         (0)     3645 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/protecode/report.py
--rw-r--r--   0 root         (0) root         (0)     3563 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/protecode/rescore.py
--rw-r--r--   0 root         (0) root         (0)    24660 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/protecode/scanning.py
--rw-r--r--   0 root         (0) root         (0)     8437 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/protecode/util.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-04-12 12:34:12.976354 gardener-cicd-dso-1.2032.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      673 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/setup.dso.py
--rw-r--r--   0 root         (0) root         (0)     2096 2023-04-12 12:33:14.000000 gardener-cicd-dso-1.2032.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:39:48.925402 gardener-cicd-dso-1.2033.0/
+-rw-r--r--   0 root         (0) root         (0)    16830 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/NOTICE.md
+-rw-r--r--   0 root         (0) root         (0)      171 2023-04-14 08:39:48.925402 gardener-cicd-dso-1.2033.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:39:48.921403 gardener-cicd-dso-1.2033.0/checkmarx/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/checkmarx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7623 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/checkmarx/client.py
+-rw-r--r--   0 root         (0) root         (0)     3746 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/checkmarx/model.py
+-rw-r--r--   0 root         (0) root         (0)     7006 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/checkmarx/project.py
+-rw-r--r--   0 root         (0) root         (0)     5790 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/checkmarx/tablefmt.py
+-rw-r--r--   0 root         (0) root         (0)    17856 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/checkmarx/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:39:48.921403 gardener-cicd-dso-1.2033.0/clamav/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/clamav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5287 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/clamav/client.py
+-rw-r--r--   0 root         (0) root         (0)     8057 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/clamav/cnudie.py
+-rw-r--r--   0 root         (0) root         (0)     2417 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/clamav/model.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/clamav/report.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/clamav/routes.py
+-rw-r--r--   0 root         (0) root         (0)     7469 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/clamav/scan.py
+-rw-r--r--   0 root         (0) root         (0)     6604 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/clamav/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:39:48.921403 gardener-cicd-dso-1.2033.0/gardener_cicd_dso.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-04-14 08:39:48.000000 gardener-cicd-dso-1.2033.0/gardener_cicd_dso.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      688 2023-04-14 08:39:48.000000 gardener-cicd-dso-1.2033.0/gardener_cicd_dso.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-14 08:39:48.000000 gardener-cicd-dso-1.2033.0/gardener_cicd_dso.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-04-14 08:39:48.000000 gardener-cicd-dso-1.2033.0/gardener_cicd_dso.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-14 08:39:48.000000 gardener-cicd-dso-1.2033.0/gardener_cicd_dso.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-14 08:39:48.925402 gardener-cicd-dso-1.2033.0/protecode/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/protecode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5756 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/protecode/assessments.py
+-rw-r--r--   0 root         (0) root         (0)    17050 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/protecode/client.py
+-rw-r--r--   0 root         (0) root         (0)    11985 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/protecode/model.py
+-rw-r--r--   0 root         (0) root         (0)     3645 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/protecode/report.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/protecode/rescore.py
+-rw-r--r--   0 root         (0) root         (0)    24660 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/protecode/scanning.py
+-rw-r--r--   0 root         (0) root         (0)     8437 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/protecode/util.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-04-14 08:39:48.925402 gardener-cicd-dso-1.2033.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      673 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/setup.dso.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-04-14 08:09:43.000000 gardener-cicd-dso-1.2033.0/setup.py
```

### Comparing `gardener-cicd-dso-1.2032.0/LICENSE.md` & `gardener-cicd-dso-1.2033.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/README.md` & `gardener-cicd-dso-1.2033.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/checkmarx/__init__.py` & `gardener-cicd-dso-1.2033.0/checkmarx/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/checkmarx/client.py` & `gardener-cicd-dso-1.2033.0/checkmarx/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/checkmarx/model.py` & `gardener-cicd-dso-1.2033.0/checkmarx/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/checkmarx/project.py` & `gardener-cicd-dso-1.2033.0/checkmarx/project.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/checkmarx/tablefmt.py` & `gardener-cicd-dso-1.2033.0/checkmarx/tablefmt.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/checkmarx/util.py` & `gardener-cicd-dso-1.2033.0/checkmarx/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/clamav/__init__.py` & `gardener-cicd-dso-1.2033.0/clamav/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/clamav/client.py` & `gardener-cicd-dso-1.2033.0/clamav/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/clamav/cnudie.py` & `gardener-cicd-dso-1.2033.0/clamav/cnudie.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,47 +8,117 @@
 import gci.componentmodel as cm
 
 import ci.log
 import ci.util
 import clamav.client
 import clamav.model
 import clamav.scan
+import clamav.util
+import github.compliance.model as gcm
 import cnudie.iter
+import delivery.client
+import delivery.model
 import dso.model
 import github.compliance.model
 import oci.client
 
 logger = logging.getLogger(__name__)
 ci.log.configure_default_logging()
 
 
+def _may_reuse_existing_scan_result(
+        resource_node: cnudie.iter.ResourceNode,
+        virus_db_max_age_days: int,
+        delivery_client: delivery.client.DeliveryServiceClient,
+        current_version_info: clamav.model.ClamAVVersionInfo = None,
+) -> bool:
+
+    previous_findings = delivery_client.artefact_metadata_for_resource_node(
+        resource_node=resource_node,
+        types=[dso.model.Datatype.MALWARE],
+    )
+
+    if not (latest_finding := max(
+        previous_findings,
+        default=None,
+        key=lambda f: f.meta.creation_date.astimezone(),
+    )):
+        return False
+
+    if isinstance(latest_finding.data, dict):
+        # In this case the previous scan we have available predates the current dataclasses.
+        # Returning False here results in a rescan which will put a new scan result into
+        # the database if there are any findings.
+        # Also, as an additional safeguard against future errors, we check that no such
+        # supposedly structurally outdated finding was put into the database after this
+        # change was added.
+        cutoff_date = datetime.datetime(year=2023, month=4, day=17)
+        if latest_finding.meta.creation_date > cutoff_date:
+            raise RuntimeError(
+                'Encountered a malware scan result with outdated schema that was created '
+                'after introduction of the new schema.'
+            )
+        return False
+
+    finding_clamav_metadata = latest_finding.data.metadata
+
+    if finding_clamav_metadata.signature_version == current_version_info.signature_version:
+        # No changes to virus signature database version. Safe to skip, as scan would not
+        # discover anything new.
+        return True
+
+    if (
+        current_version_info.signature_date
+        - finding_clamav_metadata.virus_definition_timestamp
+    ).days < virus_db_max_age_days:
+        return True
+
+    return False
+
+
 def scan_resources(
     resource_nodes: typing.Iterable[cnudie.iter.ResourceNode],
+    clamav_version_info: clamav.model.ClamAVVersionInfo,
+    virus_db_max_age_days: int,
     oci_client: oci.client.Client,
     clamav_client: clamav.client.ClamAVClient,
-    clamav_version_info: clamav.model.ClamAVVersionInfo,
+    delivery_client: delivery.client.DeliveryServiceClient = None,
     s3_client=None,
     max_workers:int = 16,
 ) -> typing.Generator[clamav.model.ClamAVResourceScanResult, None, None]:
-    executor = concurrent.futures.ThreadPoolExecutor(max_workers=max_workers)
 
     def scan_resource(
         resource_node: cnudie.iter.ResourceNode,
-    ):
+    ) -> clamav.model.ClamAVResourceScanResult:
         component = resource_node.component
         resource = resource_node.resource
 
+        if delivery_client and _may_reuse_existing_scan_result(
+            resource_node=resource_node,
+            delivery_client=delivery_client,
+            current_version_info=clamav_version_info,
+            virus_db_max_age_days=virus_db_max_age_days,
+        ):
+            resource_name = f'{component.name}/{resource.name}'
+            logger.info(f'Skipping scan of {resource_name}.')
+            return clamav.model.ClamAVResourceScanResult(
+                scan_result=None,
+                state=gcm.ScanState.SKIPPED,
+                scanned_element=resource_node,
+            )
+
         if isinstance(resource.access, cm.OciAccess):
             access: cm.OciAccess = resource.access
             image_reference = access.imageReference
             results = clamav.scan.scan_oci_image(
                 image_reference=image_reference,
                 oci_client=oci_client,
                 clamav_client=clamav_client,
             )
+
         elif isinstance(resource.access, cm.S3Access):
             access: cm.S3Access = resource.access
             if isinstance(resource.type, enum.Enum):
                 rtype = resource.type.value
             else:
                 rtype = resource.type
             if not rtype.startswith('application/tar'):
@@ -61,52 +131,76 @@
 
             tf = tarfile.open(fileobj=fileobj, mode='r|*')
 
             results = clamav.scan.scan_tarfile(
                 clamav_client=clamav_client,
                 tf=tf,
             )
+
         else:
             raise NotImplementedError(type(resource.access))
 
         scan_result = clamav.scan.aggregate_scan_result(
             resource=resource,
             results=results,
             name=f'{component.name}/{resource.name}',
             clamav_version_info=clamav_version_info,
         )
 
         # pylint: disable=E1123
         return clamav.model.ClamAVResourceScanResult(
             scan_result=scan_result,
-            scanned_element=cnudie.iter.ResourceNode(
-                path=(component,),
-                resource=resource,
-            ),
+            scanned_element=resource_node,
         )
 
+    executor = concurrent.futures.ThreadPoolExecutor(max_workers=max_workers)
     tasks = [
         executor.submit(scan_resource, resource_node)
        for resource_node in resource_nodes
     ]
 
     logger.info(f'will scan {len(tasks)=} with {max_workers=}')
 
+    if not delivery_client:
+        logger.info(
+            'Unable to compare with previous findings in delivery-service, no client available. '
+            'All files will be scanned.'
+        )
+
     while True:
         done, not_done = concurrent.futures.wait(
             tasks,
             return_when=concurrent.futures.FIRST_COMPLETED,
         )
         logger.info(f'{len(done)} scans finished - {len(not_done)=}')
         yield from (f.result() for f in done)
         if not not_done:
             break
         tasks = not_done
 
 
+def _scan_result_to_malware_finding(
+        scan_result: clamav.model.ScanResult,
+) -> dso.model.MalwareFinding:
+    if (meta := scan_result.meta):
+        meta = dso.model.MalwareFindingMeta(
+            receive_duration_seconds=meta.receive_duration_seconds,
+            scanned_octets=meta.scanned_octets,
+            scanned_content_digest=meta.scanned_content_digest,
+            scan_duration_seconds=meta.scan_duration_seconds,
+        )
+    return dso.model.MalwareFinding(
+        status=scan_result.status.value,
+        details=scan_result.details,
+        meta=meta,
+        name=scan_result.name,
+        malware_status=scan_result.malware_status.name,
+    )
+
+
 def resource_scan_result_to_artefact_metadata(
     resource_scan_result: clamav.model.ClamAVResourceScanResult,
     datasource: str = dso.model.Datasource.CLAMAV,
     datatype: str = dso.model.Datatype.MALWARE,
     creation_date: datetime.datetime = datetime.datetime.now(),
 ) -> dso.model.ArtefactMetadata:
 
@@ -118,32 +212,14 @@
 
     meta = dso.model.Metadata(
         datasource=datasource,
         type=datatype,
         creation_date=creation_date,
     )
 
-    def _scan_result_to_malware_finding(
-            scan_result: clamav.model.ScanResult,
-    ) -> dso.model.MalwareFinding:
-        if (meta := scan_result.meta):
-            meta = dso.model.MalwareFindingMeta(
-                receive_duration_seconds=meta.receive_duration_seconds,
-                scanned_octets=meta.scanned_octets,
-                scanned_content_digest=meta.scanned_content_digest,
-                scan_duration_seconds=meta.scan_duration_seconds,
-            )
-        return dso.model.MalwareFinding(
-            status=scan_result.status.value,
-            details=scan_result.details,
-            meta=meta,
-            name=scan_result.name,
-            malware_status=scan_result.malware_status.name,
-        )
-
     aggregated_scan_result = resource_scan_result.scan_result
     clamav_version_info = aggregated_scan_result.clamav_version_info
 
     finding = dso.model.MalwareSummary(
         findings=tuple(
             _scan_result_to_malware_finding(r)
             for r in aggregated_scan_result.findings
```

### Comparing `gardener-cicd-dso-1.2032.0/clamav/model.py` & `gardener-cicd-dso-1.2033.0/clamav/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/clamav/report.py` & `gardener-cicd-dso-1.2033.0/clamav/report.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,30 +12,33 @@
 ):
     headers = ('resource', 'status', 'details')
 
     def row_from_result(scan_result: clamav.model.ClamAVResourceScanResult):
         c = scan_result.scanned_element.component
         a = github.compliance.model.artifact_from_node(scan_result.scanned_element)
         resource = f'{c.name}:{c.version}/{a.name}:{a.version}'
-        res = scan_result.scan_result
 
-        status = res.malware_status
-
-        if status is clamav.model.MalwareStatus.OK:
-            details = 'no malware found'
-        elif status is clamav.model.MalwareStatus.UNKNOWN:
-            details = 'failed to scan'
-        elif status is clamav.model.MalwareStatus.FOUND_MALWARE:
-            details = '\n'.join((
-                f'{finding.name}: {finding.details}' for finding in res.findings
-            ))
+        if scan_result.state is github.compliance.model.ScanState.SKIPPED:
+            return resource, 'scan skipped', ''
         else:
-            raise NotImplementedError(status)
+            res = scan_result.scan_result
+            status = res.malware_status
+
+            if status is clamav.model.MalwareStatus.OK:
+                details = 'no malware found'
+            elif status is clamav.model.MalwareStatus.UNKNOWN:
+                details = 'failed to scan'
+            elif status is clamav.model.MalwareStatus.FOUND_MALWARE:
+                details = '\n'.join((
+                    f'{finding.name}: {finding.details}' for finding in res.findings
+                ))
+            else:
+                raise NotImplementedError(status)
 
-        return resource, status, details
+            return resource, status, details
 
     def rows():
         for result in scan_results:
             yield row_from_result(scan_result=result)
 
     return tabulate.tabulate(
         tabular_data=rows(),
```

### Comparing `gardener-cicd-dso-1.2032.0/clamav/routes.py` & `gardener-cicd-dso-1.2033.0/clamav/routes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/clamav/scan.py` & `gardener-cicd-dso-1.2033.0/clamav/scan.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import typing
 
 import gci.componentmodel as cm
 
 import ci.log
 import clamav.client
 import clamav.model
+import clamav.util
 import oci.client
 import oci.model
 
 
 logger = logging.getLogger(__name__)
 ci.log.configure_default_logging()
 
@@ -57,24 +58,16 @@
         if len(findings) < 1:
             malware_status = clamav.model.MalwareStatus.OK
         else:
             malware_status = clamav.model.MalwareStatus.FOUND_MALWARE
     else:
         malware_status = clamav.model.MalwareStatus.UNKNOWN
 
-    if isinstance(resource.access, cm.OciAccess):
-        resource_url = resource.access.imageReference
-    elif isinstance(resource.access, cm.S3Access):
-        a = resource.access
-        resource_url = f's3://{a.bucketName}/{a.objectKey}'
-    else:
-        resource_url = '<unknown>'
-
     return clamav.model.AggregatedScanResult(
-        resource_url=resource_url,
+        resource_url=clamav.util.resource_url_from_resource_access(resource.access),
         name=name,
         malware_status=malware_status,
         findings=findings,
         scan_count=count,
         scanned_octets=scanned_octets,
         scan_duration_seconds=scan_duration_seconds,
         upload_duration_seconds=upload_duration_seconds,
```

### Comparing `gardener-cicd-dso-1.2032.0/clamav/util.py` & `gardener-cicd-dso-1.2033.0/clamav/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -180,7 +180,18 @@
 
     results = executor.map(
         try_scan_func,
         resources,
     )
 
     yield from results
+
+def resource_url_from_resource_access(
+    access: gci.componentmodel.ResourceAccess,
+) -> str:
+        # TODO: replace once a more fitting method exists in component-model
+        if isinstance(access, gci.componentmodel.OciAccess):
+            return access.imageReference
+        elif isinstance(access, gci.componentmodel.S3Access):
+            return f's3://{access.bucketName}/{access.objectKey}'
+        else:
+            raise NotImplementedError(access.type)
```

### Comparing `gardener-cicd-dso-1.2032.0/gardener_cicd_dso.egg-info/SOURCES.txt` & `gardener-cicd-dso-1.2033.0/gardener_cicd_dso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/protecode/__init__.py` & `gardener-cicd-dso-1.2033.0/protecode/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/protecode/assessments.py` & `gardener-cicd-dso-1.2033.0/protecode/assessments.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/protecode/client.py` & `gardener-cicd-dso-1.2033.0/protecode/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/protecode/model.py` & `gardener-cicd-dso-1.2033.0/protecode/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/protecode/report.py` & `gardener-cicd-dso-1.2033.0/protecode/report.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/protecode/rescore.py` & `gardener-cicd-dso-1.2033.0/protecode/rescore.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/protecode/scanning.py` & `gardener-cicd-dso-1.2033.0/protecode/scanning.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/protecode/util.py` & `gardener-cicd-dso-1.2033.0/protecode/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/setup.dso.py` & `gardener-cicd-dso-1.2033.0/setup.dso.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2032.0/setup.py` & `gardener-cicd-dso-1.2033.0/setup.py`

 * *Files identical despite different names*

