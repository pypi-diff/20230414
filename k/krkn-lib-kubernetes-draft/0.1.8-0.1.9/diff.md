# Comparing `tmp/krkn_lib_kubernetes_draft-0.1.8.tar.gz` & `tmp/krkn_lib_kubernetes_draft-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krkn_lib_kubernetes_draft-0.1.8.tar", max compression
+gzip compressed data, was "krkn_lib_kubernetes_draft-0.1.9.tar", max compression
```

## Comparing `krkn_lib_kubernetes_draft-0.1.8.tar` & `krkn_lib_kubernetes_draft-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    10173 2023-04-12 08:14:10.838229 krkn_lib_kubernetes_draft-0.1.8/LICENSE
--rw-r--r--   0        0        0       22 2023-04-12 08:14:10.838229 krkn_lib_kubernetes_draft-0.1.8/README.md
--rw-r--r--   0        0        0      539 2023-04-12 08:14:10.906230 krkn_lib_kubernetes_draft-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       63 2023-04-12 08:14:10.838229 krkn_lib_kubernetes_draft-0.1.8/src/krkn_lib_kubernetes_draft/__init__.py
--rw-r--r--   0        0        0    39728 2023-04-12 08:14:22.166372 krkn_lib_kubernetes_draft-0.1.8/src/krkn_lib_kubernetes_draft/client.py
--rw-r--r--   0        0        0     1690 2023-04-12 08:14:10.838229 krkn_lib_kubernetes_draft-0.1.8/src/krkn_lib_kubernetes_draft/resources.py
--rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 krkn_lib_kubernetes_draft-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    10173 2023-04-12 09:36:48.060853 krkn_lib_kubernetes_draft-0.1.9/LICENSE
+-rw-r--r--   0        0        0       22 2023-04-12 09:36:48.064852 krkn_lib_kubernetes_draft-0.1.9/README.md
+-rw-r--r--   0        0        0      539 2023-04-12 09:36:48.128837 krkn_lib_kubernetes_draft-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       63 2023-04-12 09:36:48.064852 krkn_lib_kubernetes_draft-0.1.9/src/krkn_lib_kubernetes_draft/__init__.py
+-rw-r--r--   0        0        0    42541 2023-04-12 09:36:57.404748 krkn_lib_kubernetes_draft-0.1.9/src/krkn_lib_kubernetes_draft/client.py
+-rw-r--r--   0        0        0     1690 2023-04-12 09:36:48.064852 krkn_lib_kubernetes_draft-0.1.9/src/krkn_lib_kubernetes_draft/resources.py
+-rw-r--r--   0        0        0      732 1970-01-01 00:00:00.000000 krkn_lib_kubernetes_draft-0.1.9/PKG-INFO
```

### Comparing `krkn_lib_kubernetes_draft-0.1.8/LICENSE` & `krkn_lib_kubernetes_draft-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `krkn_lib_kubernetes_draft-0.1.8/pyproject.toml` & `krkn_lib_kubernetes_draft-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "krkn-lib-kubernetes-draft"
-version = "v0.1.8"
+version = "v0.1.9"
 description = "Kubernetes library for Kraken"
 authors = ["Red Hat Chaos Engineering Team"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/redhat-chaos/krkn"
 #packages = [{include= "src/krkn_lib_kubernetes_draft"}]
```

### Comparing `krkn_lib_kubernetes_draft-0.1.8/src/krkn_lib_kubernetes_draft/client.py` & `krkn_lib_kubernetes_draft-0.1.9/src/krkn_lib_kubernetes_draft/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import random
 import re
 import time
 
 import arcaflow_lib_kubernetes
 import kubernetes
 from kubernetes import client, config, utils, watch
 from kubernetes.client.rest import ApiException
@@ -82,16 +83,16 @@
             f = open(kubeconfig_path)
             with f:
                 kubeconfig_str = f.read()
                 self.initialize_clients_from_kconfig_string(kubeconfig_str)
 
         except OSError:
             raise Exception(
-                f"Invalid kube-config file: {kubeconfig_path}. "
-                "No configuration found."
+                "Invalid kube-config file: {0}. "
+                "No configuration found.".format(kubeconfig_path)
             )
 
     def __initialize_clients_from_kconfig_string(
         self,
         kubeconfig_str: str,
     ):
         """
@@ -112,18 +113,20 @@
             self.batch_cli = client.BatchV1Api(self.api_client)
             self.watch_resource = watch.Watch()
             self.custom_object_client = client.CustomObjectsApi(
                 self.api_client
             )
             self.dyn_client = DynamicClient(self.api_client)
         except ApiException as e:
-            logging.error(f"Failed to initialize kubernetes client: {e}\n")
+            logging.error(
+                "Failed to initialize kubernetes client: %s\n", str(e)
+            )
             raise e
         except Exception as e:
-            logging.error(f"failed to validate kubeconfig: {e}\n")
+            logging.error("failed to validate kubeconfig: %s\n", str(e))
             raise e
 
     def get_host(self) -> str:
         """
         Returns the Kubernetes server URL
         :return: kubernetes server URL
         """
@@ -171,15 +174,16 @@
                 ret = self.cli.list_namespace(
                     pretty=True, label_selector=label_selector
                 )
             else:
                 ret = self.cli.list_namespace(pretty=True)
         except ApiException as e:
             logging.error(
-                f"Exception when calling CoreV1Api->list_namespaced_pod: {e}\n"
+                "Exception when calling CoreV1Api->list_namespaced_pod: %s\n",
+                str(e),
             )
             raise e
         for namespace in ret.items:
             namespaces.append(namespace.metadata.name)
         return namespaces
 
     def get_namespace_status(self, namespace_name: str) -> str:
@@ -191,16 +195,17 @@
         """
 
         ret = ""
         try:
             ret = self.cli.read_namespace_status(namespace_name)
         except ApiException as e:
             logging.error(
-                f"Exception when calling "
-                f"CoreV1Api->read_namespace_status: {e}\n"
+                "Exception when calling "
+                "CoreV1Api->read_namespace_status: %s\n",
+                str(e),
             )
         return ret.status.phase
 
     def delete_namespace(self, namespace: str) -> client.V1Status:
         """
         Delete a given namespace
         using kubernetes python client
@@ -208,21 +213,22 @@
         :param namespace: namespace name
         :return: V1Status API object
         """
 
         try:
             api_response = self.cli.delete_namespace(namespace)
             logging.debug(
-                f"Namespace deleted. status='{str(api_response.status)}'"
+                "Namespace deleted. status='%s'", str(api_response.status)
             )
             return api_response
 
         except Exception as e:
             logging.error(
-                "Exception when calling CoreV1Api->delete_namespace: {e}\n"
+                "Exception when calling CoreV1Api->delete_namespace: %s\n",
+                str(e),
             )
             raise e
 
     def check_namespaces(
         self, namespaces: list[str], label_selector: str = None
     ) -> list[str]:
         """
@@ -245,20 +251,21 @@
                         if re.search(regex_namespace, namespace):
                             final_namespaces.add(namespace)
                             valid_regex.add(regex_namespace)
                             break
             invalid_namespaces = regex_namespaces - valid_regex
             if invalid_namespaces:
                 raise Exception(
-                    f"There exists no namespaces"
-                    f" matching: {invalid_namespaces}"
+                    "There exists no namespaces matching: {0}".format(
+                        invalid_namespaces
+                    )
                 )
             return list(final_namespaces)
         except Exception as e:
-            logging.error(f"{e}")
+            logging.error("%s", str(e))
             raise e
 
     #
     def list_nodes(self, label_selector: str = None) -> list[str]:
         """
         List nodes in the cluster
 
@@ -272,15 +279,15 @@
                 ret = self.cli.list_node(
                     pretty=True, label_selector=label_selector
                 )
             else:
                 ret = self.cli.list_node(pretty=True)
         except ApiException as e:
             logging.error(
-                f"Exception when calling CoreV1Api->list_node: {e}\n"
+                "Exception when calling CoreV1Api->list_node: %s\n", str(e)
             )
             raise e
         for node in ret.items:
             nodes.append(node.metadata.name)
         return nodes
 
     #
@@ -299,15 +306,15 @@
                 ret = self.cli.list_node(
                     pretty=True, label_selector=label_selector
                 )
             else:
                 ret = self.cli.list_node(pretty=True)
         except ApiException as e:
             logging.error(
-                f"Exception when calling CoreV1Api->list_node: {e}\n"
+                "Exception when calling CoreV1Api->list_node: %s\n", str(e)
             )
             raise e
         for node in ret.items:
             if kraken_node_name != node.metadata.name:
                 for cond in node.status.conditions:
                     if (
                         str(cond.type) == "Ready"
@@ -332,16 +339,17 @@
                 group="cluster.open-cluster-management.io",
                 version="v1",
                 plural="managedclusters",
                 label_selector=label_selector,
             )
         except ApiException as e:
             logging.error(
-                f"Exception when calling "
-                f"CustomObjectsApi->list_cluster_custom_object: {e}\n"
+                "Exception when calling "
+                "CustomObjectsApi->list_cluster_custom_object: %s\n",
+                str(e),
             )
             raise e
         for managedcluster in ret["items"]:
             conditions = managedcluster["status"]["conditions"]
             available = list(
                 filter(
                     lambda condition: condition["reason"]
@@ -371,15 +379,16 @@
                 ret = self.cli.list_namespaced_pod(
                     namespace, pretty=True, label_selector=label_selector
                 )
             else:
                 ret = self.cli.list_namespaced_pod(namespace, pretty=True)
         except ApiException as e:
             logging.error(
-                f"Exception when calling CoreV1Api->list_namespaced_pod: {e}\n"
+                "Exception when calling CoreV1Api->list_namespaced_pod: %s\n",
+                str(e),
             )
             raise e
         for pod in ret.items:
             pods.append(pod.metadata.name)
         return pods
 
     def get_all_pods(self, label_selector: str = None) -> list[[str, str]]:
@@ -444,15 +453,15 @@
                     command=exec_command,
                     stderr=True,
                     stdin=False,
                     stdout=True,
                     tty=False,
                 )
         except Exception as e:
-            logging.error(f"failed to exec command on pod {e}")
+            logging.error("failed to exec command on pod %s", str(e))
             raise e
         return ret
 
     def delete_pod(self, name: str, namespace: str = "default"):
         """
         Delete a pod in a namespace
 
@@ -463,15 +472,15 @@
             self.cli.delete_namespaced_pod(name=name, namespace=namespace)
             while self.cli.read_namespaced_pod(name=name, namespace=namespace):
                 time.sleep(1)
         except ApiException as e:
             if e.status == 404:
                 logging.info("Pod already deleted")
             else:
-                logging.error(f"Failed to delete pod {e}")
+                logging.error("Failed to delete pod %s", str(e))
                 raise e
 
     def create_pod(self, body: any, namespace: str, timeout: int = 120):
         """
         Create a pod in a namespace
 
         :param body: an object representation of a valid pod yaml manifest
@@ -490,15 +499,15 @@
                 )
                 if pod_stat.status.phase == "Running":
                     break
                 if time.time() > end_time:
                     raise Exception("Starting pod failed")
                 time.sleep(1)
         except Exception as e:
-            logging.error(f"Pod creation failed {e}")
+            logging.error("Pod creation failed %s", str(e))
             if pod_stat:
                 logging.error(pod_stat.status.container_statuses)
             self.delete_pod(body["metadata"]["name"], namespace)
             raise e
 
     def read_pod(self, name: str, namespace: str = "default") -> client.V1Pod:
         """
@@ -556,28 +565,28 @@
             api_response = self.batch_cli.delete_namespaced_job(
                 name=name,
                 namespace=namespace,
                 body=client.V1DeleteOptions(
                     propagation_policy="Foreground", grace_period_seconds=0
                 ),
             )
-            logging.debug(
-                "Job deleted. status='%s'" % str(api_response.status)
-            )
+            logging.debug("Job deleted. status='%s'", str(api_response.status))
             return api_response
         except ApiException as api:
             logging.warning(
-                f"Exception when calling "
-                f"BatchV1Api->create_namespaced_job: {api}"
+                "Exception when calling "
+                "BatchV1Api->create_namespaced_job: %s",
+                api,
             )
             logging.warning("Job already deleted\n")
         except Exception as e:
             logging.error(
-                f"Exception when calling "
-                f"BatchV1Api->delete_namespaced_job: {e}\n"
+                "Exception when calling "
+                "BatchV1Api->delete_namespaced_job: %s\n",
+                str(e),
             )
             raise e
 
     def create_job(
         self, body: any, namespace: str = "default"
     ) -> client.V1Job:
         """
@@ -589,22 +598,23 @@
         try:
             api_response = self.batch_cli.create_namespaced_job(
                 body=body, namespace=namespace
             )
             return api_response
         except ApiException as api:
             logging.warning(
-                f"Exception when calling BatchV1Api->create_job: {api}"
+                "Exception when calling BatchV1Api->create_job: %s", api
             )
             if api.status == 409:
                 logging.warning("Job already present")
         except Exception as e:
             logging.error(
-                f"Exception when calling "
-                f"BatchV1Api->create_namespaced_job: {e}"
+                "Exception when calling "
+                "BatchV1Api->create_namespaced_job: %s",
+                str(e),
             )
             raise e
 
     def create_manifestwork(
         self, body: any, namespace: str = "default"
     ) -> object:
         """
@@ -627,16 +637,17 @@
                     body=body,
                     namespace=namespace,
                 )
             )
             return api_response
         except ApiException as e:
             print(
-                f"Exception when calling "
-                f"CustomObjectsApi->create_namespaced_custom_object: {e}\n"
+                "Exception when calling "
+                "CustomObjectsApi->create_namespaced_custom_object: %s\n",
+                str(e),
             )
 
     def delete_manifestwork(self, namespace: str):
         """
         Delete a manifestwork from a namespace
 
         :param namespace: namespace from where the manifestwork must be deleted
@@ -652,16 +663,17 @@
                     name="managedcluster-scenarios-template",
                     namespace=namespace,
                 )
             )
             return api_response
         except ApiException as e:
             print(
-                f"Exception when calling "
-                f"CustomObjectsApi->delete_namespaced_custom_object: {e}\n"
+                "Exception when calling "
+                "CustomObjectsApi->delete_namespaced_custom_object: %s\n",
+                str(e),
             )
 
     def get_job_status(
         self, name: str, namespace: str = "default"
     ) -> client.V1Job:
         """
         Get a job status
@@ -672,16 +684,17 @@
         """
         try:
             return self.batch_cli.read_namespaced_job_status(
                 name=name, namespace=namespace
             )
         except Exception as e:
             logging.error(
-                f"Exception when calling "
-                f"BatchV1Api->read_namespaced_job_status: {e}\n"
+                "Exception when calling "
+                "BatchV1Api->read_namespaced_job_status: %s\n",
+                str(e),
             )
             raise
 
     def monitor_nodes(
         self,
     ) -> (bool, list[str]):
         """
@@ -694,16 +707,17 @@
         notready_nodes = []
         node_kerneldeadlock_status = "False"
         for node in nodes:
             try:
                 node_info = self.cli.read_node_status(node, pretty=True)
             except ApiException as e:
                 logging.error(
-                    f"Exception when calling "
-                    f"CoreV1Api->read_node_status: {e}\n"
+                    "Exception when calling "
+                    "CoreV1Api->read_node_status: %s\n",
+                    str(e),
                 )
                 raise e
             for condition in node_info.status.conditions:
                 if condition.type == "KernelDeadlock":
                     node_kerneldeadlock_status = condition.status
                 elif condition.type == "Ready":
                     node_ready_status = condition.status
@@ -733,16 +747,17 @@
         for pod in pods:
             try:
                 pod_info = self.cli.read_namespaced_pod_status(
                     pod, namespace, pretty=True
                 )
             except ApiException as e:
                 logging.error(
-                    f"Exception when calling "
-                    f"CoreV1Api->read_namespaced_pod_status: {e}\n"
+                    "Exception when calling "
+                    "CoreV1Api->read_namespaced_pod_status: %s\n",
+                    str(e),
                 )
                 raise e
             pod_status = pod_info.status.phase
             if (
                 pod_status != "Running"
                 and pod_status != "Completed"
                 and pod_status != "Succeeded"
@@ -765,16 +780,18 @@
         :return: the status of the component namespace
         """
 
         watch_component_status, failed_component_pods = self.monitor_namespace(
             component_namespace
         )
         logging.info(
-            f"Iteration {iteration}: "
-            f"{component_namespace}: {watch_component_status}"
+            "Iteration %s: %s: %s",
+            iteration,
+            component_namespace,
+            watch_component_status,
         )
         return watch_component_status, failed_component_pods
 
     def apply_yaml(self, path, namespace="default") -> list[str]:
         """
         Apply yaml config to create Kubernetes resources
 
@@ -845,16 +862,15 @@
                 containers=container_list,
                 nodeName=response.spec.node_name,
                 volumes=volume_list,
             )
             return pod_info
         else:
             logging.error(
-                f"Pod '{str(name)}' doesn't "
-                f"exist in namespace '{str(namespace)}'"
+                "Pod '%s' doesn't exist in namespace '%s'", name, namespace
             )
             return None
 
     def get_litmus_chaos_object(
         self, kind: str, name: str, namespace: str = "default"
     ) -> LitmusChaosObject:
         """
@@ -950,15 +966,15 @@
 
         namespace_exists = self.check_if_namespace_exists(namespace)
         if namespace_exists:
             pod_list = self.list_pods(namespace=namespace)
             if name in pod_list:
                 return True
         else:
-            logging.error(f"Namespace '{str(namespace)}' doesn't exist")
+            logging.error("Namespace '%s' doesn't exist", str(namespace))
         return False
 
     def check_if_pvc_exists(
         self, name: str, namespace: str = "default"
     ) -> bool:
         """
         Check if a PVC exists by parsing through the list of projects.
@@ -973,15 +989,15 @@
             response = self.cli.list_namespaced_persistent_volume_claim(
                 namespace=namespace
             )
             pvc_list = [pvc.metadata.name for pvc in response.items]
             if name in pvc_list:
                 return True
         else:
-            logging.error(f"Namespace '{str(namespace)}' doesn't exist")
+            logging.error("Namespace '%s' doesn't exist", str(namespace))
         return False
 
     def get_pvc_info(self, name: str, namespace: str) -> PVC:
         """
         Retrieve information about a Persistent Volume Claim in a
         given namespace
 
@@ -1023,16 +1039,17 @@
                 volumeName=volume_name,
                 podNames=pvc_pod_list,
                 namespace=namespace,
             )
             return pvc_info
         else:
             logging.error(
-                f"PVC '{str(name)}' doesn't exist "
-                f"in namespace '{str(namespace)}'"
+                "PVC '%s' doesn't exist in namespace '%s'",
+                str(name),
+                str(namespace),
             )
             return None
 
     def find_kraken_node(self) -> str:
         """
         Find the node kraken is deployed on
         Set global kraken node to not delete
@@ -1054,15 +1071,15 @@
         if kraken_pod_name:
             # get kraken-deployment pod, find node name
             try:
                 node_name = self.get_pod_info(
                     kraken_pod_name, kraken_project
                 ).nodeName
             except Exception as e:
-                logging.info(f"{e}")
+                logging.info("%s", str(e))
                 raise e
         return node_name
 
     def watch_node_status(
         self, node: str, status: str, timeout: int, resource_version: str
     ):
         """
@@ -1087,15 +1104,17 @@
             ]
             if conditions[0].status == status:
                 self.watch_resource.stop()
                 break
             else:
                 count -= 1
                 logging.info(
-                    f"Status of node {node}: {str(conditions[0].status)}"
+                    "Status of node %s: %s",
+                    node,
+                    str(conditions[0].status),
                 )
             if not count:
                 self.watch_resource.stop()
 
     #
     # TODO: Implement this with a watcher instead of polling
     def watch_managedcluster_status(
@@ -1123,34 +1142,103 @@
                     == "ManagedClusterAvailable",
                     conditions,
                 )
             )
             if status == "True":
                 if available and available[0]["status"] == "True":
                     logging.info(
-                        f"Status of managedcluster "
-                        f"{managedcluster}: Available"
+                        "Status of managedcluster %s: Available",
+                        managedcluster,
                     )
                     return True
             else:
                 if not available:
                     logging.info(
-                        f"Status of managedcluster "
-                        f"{managedcluster}: Unavailable"
+                        "Status of managedcluster %s: Unavailable",
+                        managedcluster,
                     )
                     return True
             time.sleep(2)
             elapsed_time += 2
             if elapsed_time >= timeout:
                 logging.info(
-                    f"Timeout waiting for managedcluster "
-                    f"{managedcluster}  to become: {status}"
+                    "Timeout waiting for managedcluster %s to become: %s",
+                    managedcluster,
+                    status,
                 )
                 return False
 
     def get_node_resource_version(self, node: str) -> str:
         """
         Get the resource version for the specified node
         :param node: node name
         :return: resource version
         """
         return self.cli.read_node(name=node).metadata.resource_version
+
+    def list_ready_nodes(self, label_selector: str = None) -> list[str]:
+        """
+        Returns a list of ready nodes
+
+        :param label_selector: filter by label
+                               selector (optional default `None`)
+        :return: a list of node names
+        """
+
+        nodes = []
+        try:
+            if label_selector:
+                ret = self.cli.list_node(
+                    pretty=True, label_selector=label_selector
+                )
+            else:
+                ret = self.cli.list_node(pretty=True)
+        except ApiException as e:
+            logging.error(
+                "Exception when calling CoreV1Api->list_node: %s\n", str(e)
+            )
+            raise e
+        for node in ret.items:
+            for cond in node.status.conditions:
+                if str(cond.type) == "Ready" and str(cond.status) == "True":
+                    nodes.append(node.metadata.name)
+
+        return nodes
+
+    # TODO: is the signature correct? the method
+    #  returns a list of nodes and the signature name is `get_node`
+    def get_node(
+        self, node_name: str, label_selector: str, instance_kill_count: int
+    ) -> list[str]:
+        """
+        Returns active node(s)
+
+        :param node_name: node name
+        :param label_selector: filter by label
+        :param instance_kill_count:
+        :return:
+        """
+        if node_name in self.list_ready_nodes():
+            return [node_name]
+        elif node_name:
+            logging.info(
+                "Node with provided node_name "
+                "does not exist or the node might "
+                "be in NotReady state."
+            )
+        nodes = self.list_ready_nodes(label_selector)
+        if not nodes:
+            raise Exception(
+                "Ready nodes with the provided label selector do not exist"
+            )
+        logging.info(
+            "Ready nodes with the label selector %s: %s", label_selector, nodes
+        )
+        number_of_nodes = len(nodes)
+        if instance_kill_count == number_of_nodes:
+            return nodes
+        nodes_to_return = []
+        for i in range(instance_kill_count):
+            node_to_add = nodes[random.randint(0, len(nodes) - 1)]
+            nodes_to_return.append(node_to_add)
+            nodes.remove(node_to_add)
+        return nodes_to_return
```

### Comparing `krkn_lib_kubernetes_draft-0.1.8/src/krkn_lib_kubernetes_draft/resources.py` & `krkn_lib_kubernetes_draft-0.1.9/src/krkn_lib_kubernetes_draft/resources.py`

 * *Files identical despite different names*

### Comparing `krkn_lib_kubernetes_draft-0.1.8/PKG-INFO` & `krkn_lib_kubernetes_draft-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krkn-lib-kubernetes-draft
-Version: 0.1.8
+Version: 0.1.9
 Summary: Kubernetes library for Kraken
 Home-page: https://github.com/redhat-chaos/krkn
 License: Apache-2.0
 Author: Red Hat Chaos Engineering Team
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

