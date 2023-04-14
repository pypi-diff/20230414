# Comparing `tmp/vmware_aria_operations_integration_sdk-0.5.0rc2.tar.gz` & `tmp/vmware_aria_operations_integration_sdk-0.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmware_aria_operations_integration_sdk-0.5.0rc2.tar", max compression
+gzip compressed data, was "vmware_aria_operations_integration_sdk-0.5.0rc3.tar", max compression
```

## Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2.tar` & `vmware_aria_operations_integration_sdk-0.5.0rc3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    10449 2022-10-27 15:46:24.345895 vmware_aria_operations_integration_sdk-0.5.0rc2/LICENSE
--rw-r--r--   0        0        0    12154 2022-11-22 16:59:16.854261 vmware_aria_operations_integration_sdk-0.5.0rc2/README.md
--rw-r--r--   0        0        0     1992 2023-03-31 19:01:54.687489 vmware_aria_operations_integration_sdk-0.5.0rc2/pyproject.toml
--rw-r--r--   0        0        0       70 2022-11-22 16:59:16.872140 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/__init__.py
--rw-r--r--   0        0        0     4039 2023-02-24 14:06:04.218957 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/adapter_container.py
--rw-r--r--   0        0        0       70 2022-11-30 20:30:20.187730 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/adapter_template/__init__.py
--rw-r--r--   0        0        0    10899 2023-01-27 15:59:03.422897 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/adapter_template/adapter.py
--rw-r--r--   0        0        0    38857 2023-01-11 16:15:44.602229 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/adapter_template/alertDefinitionSchema.xsd
--rw-r--r--   0        0        0   115627 2022-11-22 16:59:16.875203 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/adapter_template/describeSchema.xsd
--rw-r--r--   0        0        0      877 2022-11-30 20:30:20.188151 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/adapter_template/java.py
--rw-r--r--   0        0        0      504 2023-02-02 21:38:57.354182 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/adapter_template/powershell.py
--rw-r--r--   0        0        0    12694 2022-11-22 16:59:16.876825 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/adapter_template/traversalSpecsSchema.xsd
--rw-r--r--   0        0        0       70 2022-11-22 16:59:16.877055 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/api/__init__.py
--rw-r--r--   0        0        0     8537 2022-11-22 16:59:16.877842 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/api/integration-sdk-definition-endpoint.json
--rw-r--r--   0        0        0    22318 2023-03-31 18:20:30.853497 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/api/vmware-aria-operations-collector-fwk2.json
--rw-r--r--   0        0        0    17880 2023-03-28 19:28:30.435791 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/collection_statistics.py
--rw-r--r--   0        0        0     2864 2023-01-11 16:15:44.604632 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/config.py
--rw-r--r--   0        0        0     1245 2022-11-30 20:30:20.188889 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/constant.py
--rw-r--r--   0        0        0      501 2023-03-31 18:48:42.334870 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/container_versions.json
--rw-r--r--   0        0        0     6522 2023-03-31 18:20:30.854391 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/containerized_adapter_rest_api.py
--rw-r--r--   0        0        0    18841 2023-03-30 20:55:20.203300 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/describe.py
--rw-r--r--   0        0        0    14164 2023-03-30 20:55:20.204815 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/docker_wrapper.py
--rw-r--r--   0        0        0     2018 2023-03-31 18:20:30.857197 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/filesystem.py
--rw-r--r--   0        0        0     1737 2023-01-11 16:15:44.610687 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/logging_format.py
--rw-r--r--   0        0        0     2194 2023-01-11 16:15:44.611683 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/model.py
--rw-r--r--   0        0        0    22646 2023-03-31 18:20:30.858558 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/mp_build.py
--rw-r--r--   0        0        0    19741 2023-03-31 18:39:47.668749 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/mp_init.py
--rw-r--r--   0        0        0    33436 2023-03-31 18:20:30.859579 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/mp_test.py
--rw-r--r--   0        0        0     6888 2023-03-31 18:20:30.860710 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/project.py
--rw-r--r--   0        0        0      834 2023-01-11 16:15:44.618210 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/propertiesfile.py
--rw-r--r--   0        0        0    13100 2023-03-31 18:20:30.861565 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/serialization.py
--rw-r--r--   0        0        0     2822 2023-01-11 16:15:44.620174 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/stats.py
--rw-r--r--   0        0        0      634 2023-01-11 16:15:44.621124 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/threading.py
--rw-r--r--   0        0        0     1590 2023-01-11 16:15:44.622057 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/timer.py
--rw-r--r--   0        0        0    17620 2023-02-24 14:06:04.222246 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/ui.py
--rw-r--r--   0        0        0      762 2023-01-11 16:15:44.624427 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/util.py
--rw-r--r--   0        0        0       70 2022-11-30 20:30:20.193055 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/__init__.py
--rw-r--r--   0        0        0     2262 2023-03-31 18:20:30.862856 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/adapter_definition_validator.py
--rw-r--r--   0        0        0     3136 2023-03-31 18:20:30.863841 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/api_response_validation.py
--rw-r--r--   0        0        0    11224 2023-03-31 18:20:30.864980 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/describe_checks.py
--rw-r--r--   0        0        0     1961 2023-03-31 18:20:30.865956 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/endpoint_url_validator.py
--rw-r--r--   0        0        0     6874 2023-03-31 18:20:30.866991 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/highlights.py
--rw-r--r--   0        0        0     6923 2023-03-31 18:20:30.867726 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/input_validators.py
--rw-r--r--   0        0        0     5191 2023-03-31 18:20:30.868584 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/relationship_validator.py
--rw-r--r--   0        0        0     1311 2023-03-31 18:20:30.869895 vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/result.py
--rw-r--r--   0        0        0    14222 1970-01-01 00:00:00.000000 vmware_aria_operations_integration_sdk-0.5.0rc2/setup.py
--rw-r--r--   0        0        0    13653 1970-01-01 00:00:00.000000 vmware_aria_operations_integration_sdk-0.5.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    10449 2022-10-27 15:46:24.345895 vmware_aria_operations_integration_sdk-0.5.0rc3/LICENSE
+-rw-r--r--   0        0        0    14832 2023-04-14 19:48:56.128849 vmware_aria_operations_integration_sdk-0.5.0rc3/README.md
+-rw-r--r--   0        0        0     1992 2023-04-14 20:07:29.284449 vmware_aria_operations_integration_sdk-0.5.0rc3/pyproject.toml
+-rw-r--r--   0        0        0       70 2022-11-22 16:59:16.872140 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/__init__.py
+-rw-r--r--   0        0        0     4039 2023-02-24 14:06:04.218957 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_container.py
+-rw-r--r--   0        0        0       70 2022-11-30 20:30:20.187730 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/__init__.py
+-rw-r--r--   0        0        0    10899 2023-01-27 15:59:03.422897 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/adapter.py
+-rw-r--r--   0        0        0    38857 2023-01-11 16:15:44.602229 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/alertDefinitionSchema.xsd
+-rw-r--r--   0        0        0   115627 2022-11-22 16:59:16.875203 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/describeSchema.xsd
+-rw-r--r--   0        0        0      877 2022-11-30 20:30:20.188151 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/java.py
+-rw-r--r--   0        0        0      504 2023-02-02 21:38:57.354182 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/powershell.py
+-rw-r--r--   0        0        0    12694 2022-11-22 16:59:16.876825 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/traversalSpecsSchema.xsd
+-rw-r--r--   0        0        0       70 2022-11-22 16:59:16.877055 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/api/__init__.py
+-rw-r--r--   0        0        0     8537 2022-11-22 16:59:16.877842 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/api/integration-sdk-definition-endpoint.json
+-rw-r--r--   0        0        0    22318 2023-03-31 18:20:30.853497 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/api/vmware-aria-operations-collector-fwk2.json
+-rw-r--r--   0        0        0    17880 2023-03-28 19:28:30.435791 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/collection_statistics.py
+-rw-r--r--   0        0        0     2864 2023-01-11 16:15:44.604632 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/config.py
+-rw-r--r--   0        0        0     1298 2023-04-14 19:48:56.132533 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/constant.py
+-rw-r--r--   0        0        0      501 2023-03-31 18:48:42.334870 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/container_versions.json
+-rw-r--r--   0        0        0     6522 2023-03-31 18:20:30.854391 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/containerized_adapter_rest_api.py
+-rw-r--r--   0        0        0    18841 2023-03-30 20:55:20.203300 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/describe.py
+-rw-r--r--   0        0        0    14164 2023-03-30 20:55:20.204815 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/docker_wrapper.py
+-rw-r--r--   0        0        0     2018 2023-03-31 18:20:30.857197 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/filesystem.py
+-rw-r--r--   0        0        0     1737 2023-01-11 16:15:44.610687 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/logging_format.py
+-rw-r--r--   0        0        0     2194 2023-01-11 16:15:44.611683 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/model.py
+-rw-r--r--   0        0        0    22850 2023-04-14 19:48:56.134212 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/mp_build.py
+-rw-r--r--   0        0        0    19790 2023-04-14 19:48:56.135094 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/mp_init.py
+-rw-r--r--   0        0        0    33436 2023-03-31 18:20:30.859579 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/mp_test.py
+-rw-r--r--   0        0        0     6888 2023-03-31 18:20:30.860710 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/project.py
+-rw-r--r--   0        0        0      852 2023-04-07 21:23:08.899171 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/propertiesfile.py
+-rw-r--r--   0        0        0    13100 2023-03-31 18:20:30.861565 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/serialization.py
+-rw-r--r--   0        0        0     2822 2023-01-11 16:15:44.620174 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/stats.py
+-rw-r--r--   0        0        0      634 2023-01-11 16:15:44.621124 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/threading.py
+-rw-r--r--   0        0        0     1590 2023-01-11 16:15:44.622057 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/timer.py
+-rw-r--r--   0        0        0    17620 2023-02-24 14:06:04.222246 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/ui.py
+-rw-r--r--   0        0        0      762 2023-01-11 16:15:44.624427 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/util.py
+-rw-r--r--   0        0        0       70 2022-11-30 20:30:20.193055 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/__init__.py
+-rw-r--r--   0        0        0     2262 2023-03-31 18:20:30.862856 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/adapter_definition_validator.py
+-rw-r--r--   0        0        0     3136 2023-03-31 18:20:30.863841 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/api_response_validation.py
+-rw-r--r--   0        0        0    11224 2023-03-31 18:20:30.864980 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/describe_checks.py
+-rw-r--r--   0        0        0     1961 2023-03-31 18:20:30.865956 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/endpoint_url_validator.py
+-rw-r--r--   0        0        0     6874 2023-03-31 18:20:30.866991 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/highlights.py
+-rw-r--r--   0        0        0     6923 2023-03-31 18:20:30.867726 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/input_validators.py
+-rw-r--r--   0        0        0     5191 2023-03-31 18:20:30.868584 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/relationship_validator.py
+-rw-r--r--   0        0        0     1311 2023-03-31 18:20:30.869895 vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/result.py
+-rw-r--r--   0        0        0    16957 1970-01-01 00:00:00.000000 vmware_aria_operations_integration_sdk-0.5.0rc3/setup.py
+-rw-r--r--   0        0        0    16331 1970-01-01 00:00:00.000000 vmware_aria_operations_integration_sdk-0.5.0rc3/PKG-INFO
```

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/LICENSE` & `vmware_aria_operations_integration_sdk-0.5.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/README.md` & `vmware_aria_operations_integration_sdk-0.5.0rc3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,59 @@
 VMware Aria Operations Integration SDK
 =====================
 
 Welcome to the VMware Aria Operations Integration SDK. 
 
-Where should I start?
-* If you want to get started creating your first Management Pack, or don't know where to start, read the 'Get Started' tutorial below.
-* If you'd like an introduction to VMware Aria Operations, Management Packs, and this SDK, [read the introduction](doc/introduction.md).
+## What is the Integration SDK?
+
+The Integration SDK creates Management Packs to add custom objects, data, and 
+relationships from a endpoint into VMware Aria Operations. 
+
+Using this SDK to create a Management Pack requires some Python 
+knowledge (more languages are planned), and an understanding of how to get 
+data from the endpoint using an API. For example, to create a Management Pack for 
+Cassandra DB, an understanding of how to write an SQL query, execute it, and read the 
+results is required.
+
+Currently, installing a Management Pack built with the integration SDK is supported for 
+On-Prem versions of VMware Aria Operations only, but we are working to bring support to 
+VMware Aria Operations Cloud in a future release.
+
+For a high-level overview of VMware Aria Operations, Management Packs, and this SDK, 
+see [the introduction](doc/introduction.md).
+
+## What can the Integration SDK be used for?
+The Integration SDK can be used to add any endpoint that supports remote monitoring to 
+VMware Aria Operations. Adding the endpoint involves creating objects that 
+represent the endpoint, which may include properties, metrics, and events, as well as
+relationships between objects.
+
+**Remote monitoring** uses an API (such as REST, SNMP, SQL, etc) to retrieve the data (as
+opposed to agent-based monitoring, where the monitoring code runs in the same location
+as the endpoint).
+
+For an example walkthrough of creating a new Management Pack monitoring an endpoint, see
+[Creating a new Management Pack for Cassandra DB](#creating-a-new-management-pack--cassandra-db-)
+
+The Integration SDK can also be used to extend objects created by another Management
+Pack with additional metrics, properties, events, or relationships. This can be useful
+to ensure access to custom data without having to re-implement already existing data.
+
+For an example walkthrough of the steps required to extend another management pack, see 
+[Extending the Existing Management Pack for MySQL](#extending-an-existing-management-pack--mysql-)
+
+## Where should I start?
+* If you want to get started creating your first Management Pack, or don't know where to start, read the [Get Started](#get-started) tutorial.
+* If you have completed the Get Started tutorial, the [walkthroughs](#walkthroughs) are guides for modifying your adapter.
 * All documentation is available from the [contents](doc/contents.md) page.
 
 ## Get Started
-
-This guide will walk through setting up the SDK and using the SDK
-to create, test, and install a simple Management Pack (integration) onto VMware Aria Operations.
+<details>
+<summary>This guide will walk through setting up the SDK and using the SDK
+to create, test, and install a simple Management Pack (integration) onto VMware Aria Operations.</summary>
 
 Contents
 * [Requirements](#requirements)
 * [Installation](#installation)
 * [Creating a Management Pack](#creating-a-management-pack)
 * [Testing a Management Pack](#testing-a-management-pack)
 * [Building and Installing a Management Pack](#building-and-installing-a-management-pack)
@@ -36,16 +74,15 @@
 The Management Packs generated by the VMware Aria Operations Integration SDK will only run on versions that supports containerized Management Packs. Currently, this is limited to on-prem installs, version 8.10 or later.
 In addition, at least one Cloud Proxy (also version 8.10 or later) must be set up in VMware Aria Operations, as containerized Management Packs must be run on a Cloud Proxy collector.
 
 #### Dependencies
 * Docker 20.10.0 or later. Updating to the latest stable version is recommended. For instructions on installing Docker,
   go to [Docker's installation documentation](https://docs.docker.com/engine/install/), choose the OS you need and
   follow the instructions provided.
-* Python3 3.9.0 or later. Earlier versions of Python3 may also work, but updating to the latest stable version is
-  recommended. Python 3.8 and earlier (including Python2) are not supported. For instructions on installing Python, go
+* Python3 3.9.0 or later. Updating to the latest stable version is recommended. Python 3.8 and earlier (including Python2) are not supported. For instructions on installing Python, go
   to [Python's installation documentation](https://wiki.python.org/moin/BeginnersGuide/Download), choose the OS you need
   and follow the instructions provided.
 * Pip. If Python3 is installed, pip is most likely also installed. For instructions on installing Pip, go
   to [Pip's installation documentation](https://pip.pypa.io/en/stable/installation/), and follow the instructions
   provided.
 * Git 2.35.0 or later. Updating to the latest stable version is recommended. 
   For instructions in installing git, go to [Git's installation documentation](https://git-scm.com/downloads),
@@ -195,14 +232,37 @@
 minutes later, the objects' metrics, properties, and events should appear. These can be checked by navigating to **
 Environment &rarr; Object Browser &rarr; All Objects** and expanding the Adapter and associated object types and object.
 
 ![CPU Idle Time](doc/test-adapter-cpu-idle-time.png)
 *The CPU object's `idle-time` metric in a Management Pack named `QAAdapterName`.*
 
 For complete documentation of the `mp-build` tool see the [MP Build Tool Documentation](doc/mp-build.md).
+</details>
+
+## Walkthroughs
+
+### Creating a New Management Pack (Cassandra-DB)
+<details><summary>
+This guide assumes you have already set up the SDK and know how to create a new project. 
+It walks you through the steps necessary to monitor an endpoint, using Cassandra DB as 
+an example.</summary>
+TODO
+</details>
+
+### Extending an Existing Management Pack (MySQL)
+<details><summary>
+This guide assumes you have already set up the SDK and know how to create a new project. 
+It walks you through the steps necessary to extend an existing Management Pact to add
+additional data, using the MySQL Management Pack as an example.</summary>
+TODO
+</details>
+
+
+## Troubleshooting
+TODO
 
 ## Contributing
 
 The vmware-aria-operations-integration-sdk project team welcomes contributions from the community. Before you start
 working with this project please read and sign our Contributor License Agreement (https://cla.vmware.com/cla/1/preview).
 If you wish to contribute code and you have not signed our Contributor Licence Agreement (CLA), our bot will prompt you
 to do so when you open a Pull Request. For any questions about the CLA process, please refer to our
```

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/pyproject.toml` & `vmware_aria_operations_integration_sdk-0.5.0rc3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.bandit]
 exclude_dirs = ["tests", "lib/python/tests"]
 
 [tool.poetry]
 name = "vmware_aria_operations_integration_sdk"
-version = "0.5.0rc2"
+version = "0.5.0rc3"
 description = "A set of tools to help users create, test, and build containerized management packs for VMware Aria Operations"
 authors = ["Kyle Rokos <krokos@vmware.com>", "Santiago Quiroga Cubillos <squirogacubi@vmware.com>"]
 license = "APACHE-2.0"
 readme = "README.md"
 packages = [{include = "vmware_aria_operations_integration_sdk"}]
 include = [
     "vmware_aria_operations_integration_sdk/adapter_template/describeSchema.xsd",
```

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/adapter_container.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_container.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/adapter_template/adapter.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/adapter.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/adapter_template/alertDefinitionSchema.xsd` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/alertDefinitionSchema.xsd`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/adapter_template/describeSchema.xsd` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/describeSchema.xsd`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/adapter_template/java.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/java.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/adapter_template/traversalSpecsSchema.xsd` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/adapter_template/traversalSpecsSchema.xsd`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/api/integration-sdk-definition-endpoint.json` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/api/integration-sdk-definition-endpoint.json`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/api/vmware-aria-operations-collector-fwk2.json` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/api/vmware-aria-operations-collector-fwk2.json`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/collection_statistics.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/collection_statistics.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/config.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/config.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/constant.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/constant.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 VERSION_FILE = "container_versions.json"
 CONTAINER_BASE_NAME = "base-adapter"
 CONTAINER_REGISTRY_PATH = "vmware_aria_operations_integration_sdk"
 CONTAINER_REGISTRY_HOST = "projects.registry.vmware.com"
 
 if platform == "win32":
     CONFIG_DIRECTORY = path.join(
-        environ.get("LocalAppData", ""), "VMware", "vROps Integration SDK"
+        environ.get("LocalAppData", ""), "VMware", "Aria Operations Integration SDK"
     )
 else:
-    CONFIG_DIRECTORY = path.join(environ.get("HOME", ""), ".vrops-sdk")
+    CONFIG_DIRECTORY = path.join(
+        environ.get("HOME", ""), ".vmware-aria-operations-integration-sdk"
+    )
 
 try:
     os.makedirs(CONFIG_DIRECTORY, exist_ok=True)
 except OSError as e:
     # This should rarely if ever happen
     print(
         f"Could not create config directory '{CONFIG_DIRECTORY}'. Please manually create and rerun this command."
```

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/containerized_adapter_rest_api.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/containerized_adapter_rest_api.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/describe.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/describe.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/docker_wrapper.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/filesystem.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/filesystem.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/logging_format.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/logging_format.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/model.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/model.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/mp_build.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/mp_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,35 +131,41 @@
         validator=NotEmptyValidator("Host"),
         description="The tag of a container registry is used to login into the container registry. the tag is composed of\n"
         "three parts: domain, port, and path. For example:\n"
         "projects.registry.vmware.com:443/vmware_aria_operations_integration_sdk_mps/base-adapter breaks into\n"
         "domain: projects.registry.vmware.com\n"
         "port: 443\n"
         "path: vmware_aria_operations_integration_sdk_mps/base-adapter\n"
-        "Domain is optional, and defaults to Docker Hub (docker.io)\n"
         "Port number is optional, and defaults to 443.",
     )
 
 
 def get_docker_registry(
     adapter_kind_key: str,
     config_file: str,
     docker_registry_arg: Optional[str],
     **kwargs: Any,
 ) -> str:
     docker_registry = get_config_value("docker_registry", config_file=config_file)
-    default_registry_value = f"harbor-repo.vmware.com/vmware_aria_operations_integration_sdk_mps/{adapter_kind_key.lower()}"
+    default_registry_value = get_config_value("default_container_registry_path")
 
     original_value = docker_registry
     if docker_registry is None and docker_registry_arg is None:
         print(
             "mp-build needs to configure a container registry to store the adapter container image.",
             "class:information",
         )
-        docker_registry = registry_prompt(default=default_registry_value)
+        if default_registry_value is not None:
+            # The default registry should have a trailing fordward slash
+            default_registry_value = (
+                f"{default_registry_value}{adapter_kind_key.lower()}"
+            )
+            docker_registry = registry_prompt(default=default_registry_value)
+        else:
+            docker_registry = registry_prompt(default="")
 
         first_time = True
         while not is_valid_registry(docker_registry):
             if first_time:
                 print("Press Ctrl + C to cancel build", "class:information")
                 first_time = False
             docker_registry = registry_prompt(default=docker_registry)
```

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/mp_init.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/mp_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,25 +300,27 @@
         if icon_file == "":
             print(
                 "An icon can be added later by setting the 'pak_icon' key in 'manifest.txt' to the \n"
                 "icon file name and adding the icon file to the root project directory.",
                 "class:information",
             )
 
-        language = selection_prompt(
-            "Select a language for the adapter.",
-            items=[
-                ("python", "Python"),
-                ("java", "Java", "Unavailable for beta release"),
-                ("powershell", "PowerShell", "Unavailable for beta release"),
-            ],
-            description="The language for the Management Pack determines the language for the template\n"
-            "source and build files.",
-        )
+        language = "python"
+        # language = selection_prompt(
+        #     "Select a language for the adapter.",
+        #     items=[
+        #         ("python", "Python"),
+        #         ("java", "Java", "Unavailable for beta release"),
+        #         ("powershell", "PowerShell", "Unavailable for beta release"),
+        #     ],
+        #     description="The language for the Management Pack determines the language for the template\n"
+        #     "source and build files.",
+        # )
         # create project_directory
+
         with Spinner("Creating Project"):
             create_project(
                 path,
                 name,
                 adapter_key,
                 description,
                 vendor,
@@ -423,15 +425,15 @@
     if language == "python":
         project_directory = "app"
         mkdir(path, project_directory)
 
         # create template requirements.txt
         requirements_file = os.path.join(path, "adapter_requirements.txt")
         with open(requirements_file, "w") as requirements:
-            requirements.write("psutil==5.9.0\n")
+            requirements.write("psutil==5.9.4\n")
             requirements.write("vmware-aria-operations-integration-sdk-lib==0.7.*\n")
 
         # create development requirements file
         requirements_file = os.path.join(path, "requirements.txt")
         with open(requirements_file, "w") as requirements:
             package = "vmware-aria-operations-integration-sdk"
             version = pkg_resources.get_distribution(package).version
```

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/mp_test.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/mp_test.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/project.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/project.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/propertiesfile.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/propertiesfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,11 +15,11 @@
     except FileNotFoundError as e:
         # resources.properties file is not required to exist
         pass
     return properties
 
 
 def write_properties(properties: dict, filename: str) -> bool:
-    with open(filename, "w") as f:
+    with open(filename, "w", encoding="utf-8") as f:
         for _property in properties.keys():
             f.write(str(_property) + " = " + str(properties[_property]) + "\n")
     return True
```

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/serialization.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/serialization.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/stats.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/stats.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/threading.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/threading.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/timer.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/timer.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/ui.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/ui.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/util.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/util.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/adapter_definition_validator.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/adapter_definition_validator.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/api_response_validation.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/api_response_validation.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/describe_checks.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/describe_checks.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/endpoint_url_validator.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/endpoint_url_validator.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/highlights.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/highlights.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/input_validators.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/input_validators.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/relationship_validator.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/relationship_validator.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/vmware_aria_operations_integration_sdk/validation/result.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/vmware_aria_operations_integration_sdk/validation/result.py`

 * *Files identical despite different names*

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/setup.py` & `vmware_aria_operations_integration_sdk-0.5.0rc3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -35,17 +35,17 @@
                      'mp-init = '
                      'vmware_aria_operations_integration_sdk.mp_init:main',
                      'mp-test = '
                      'vmware_aria_operations_integration_sdk.mp_test:main']}
 
 setup_kwargs = {
     'name': 'vmware-aria-operations-integration-sdk',
-    'version': '0.5.0rc2',
+    'version': '0.5.0rc3',
     'description': 'A set of tools to help users create, test, and build containerized management packs for VMware Aria Operations',
-    'long_description': 'VMware Aria Operations Integration SDK\n=====================\n\nWelcome to the VMware Aria Operations Integration SDK. \n\nWhere should I start?\n* If you want to get started creating your first Management Pack, or don\'t know where to start, read the \'Get Started\' tutorial below.\n* If you\'d like an introduction to VMware Aria Operations, Management Packs, and this SDK, [read the introduction](doc/introduction.md).\n* All documentation is available from the [contents](doc/contents.md) page.\n\n## Get Started\n\nThis guide will walk through setting up the SDK and using the SDK\nto create, test, and install a simple Management Pack (integration) onto VMware Aria Operations.\n\nContents\n* [Requirements](#requirements)\n* [Installation](#installation)\n* [Creating a Management Pack](#creating-a-management-pack)\n* [Testing a Management Pack](#testing-a-management-pack)\n* [Building and Installing a Management Pack](#building-and-installing-a-management-pack)\n\n### Requirements\n\n#### Operating System:\nThe VMware Aria Operations Integration SDK has been tested in the following OSes:\n* Windows 10\n* Windows 11\n* macOS Monterey\n* Debian Linux\n* Fedora Linux\n    \nOther operating systems may be compatible.\n\n#### VMware Aria Operations\nThe Management Packs generated by the VMware Aria Operations Integration SDK will only run on versions that supports containerized Management Packs. Currently, this is limited to on-prem installs, version 8.10 or later.\nIn addition, at least one Cloud Proxy (also version 8.10 or later) must be set up in VMware Aria Operations, as containerized Management Packs must be run on a Cloud Proxy collector.\n\n#### Dependencies\n* Docker 20.10.0 or later. Updating to the latest stable version is recommended. For instructions on installing Docker,\n  go to [Docker\'s installation documentation](https://docs.docker.com/engine/install/), choose the OS you need and\n  follow the instructions provided.\n* Python3 3.9.0 or later. Earlier versions of Python3 may also work, but updating to the latest stable version is\n  recommended. Python 3.8 and earlier (including Python2) are not supported. For instructions on installing Python, go\n  to [Python\'s installation documentation](https://wiki.python.org/moin/BeginnersGuide/Download), choose the OS you need\n  and follow the instructions provided.\n* Pip. If Python3 is installed, pip is most likely also installed. For instructions on installing Pip, go\n  to [Pip\'s installation documentation](https://pip.pypa.io/en/stable/installation/), and follow the instructions\n  provided.\n* Git 2.35.0 or later. Updating to the latest stable version is recommended. \n  For instructions in installing git, go to [Git\'s installation documentation](https://git-scm.com/downloads),\n  choose the OS you need and follow the instructions provided.\n\n[//]: # (TODO: Add this section back in once we support them)\n[//]: # (#### Optional Prerequisites)\n[//]: # (* Java. Java is only required for building Java Management Packs. We recommend the latest version of the [Azul Zulu SDK]&#40;https://www.azul.com/downloads/?package=jdk#download-openjdk&#41;.)\n[//]: # (* Powershell. Powershell is only required for building Powershell Management Packs. See [Microsoft\'s installation instructions for PowerShell]&#40;https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell?view=powershell-7.2&#41;.)\n[//]: # (> Note: Creating Java and Powershell Management Packs is disabled for the Beta)\n\n### Installation\n\nTo install the SDK, use `pip` to install into the global Python environment, or `pipx` to install into a isolated environment.\n```sh\npython3 -m pip install vmware-aria-operations-integration-sdk\n```\n\n### Creating a Management Pack\nAfter the SDK is installed, create a new project, by running `mp-init`. This tool asks a series of questions that guides\nthe creation of a new management pack project. \n\n\n1. `Enter a path for the project (where code for collection, metadata, and content reside). Path:`\n\n    The path can be an absolute path, or a path relative to the directory `mp-init` was run from. The path should end in an empty\n    or non-existing directory. If the directory does not exist, it will be created. This directory will contain a new Management\n    Pack project.\n\n2. `Management Pack display name`\n\n    The Management Pack display name will show up in VMware Aria Operations (**Data Sources &rarr; Integrations &rarr;\n    Repository**), or when adding an account.\n\n    ![Integration Card for the \'TestAdapter\' Management Pack](doc/test-adapter-integration-card.png)\n\n    *This Management Pack\'s display name is \'TestAdapter\', and uses the default icon*\n\n3. `Management Pack adapter key`\n\n    This field is used internally to identify the Management Pack and Adapter Kind. By default, it is set to the \n    Management Pack display name with special characters and whitespace stripped from it.\n\n4. `Management Pack description`\n\n    This field should describe what the Management Pack will do or monitor.\n\n5. `Management Pack vendor`\n\n   The vendor field shows up in the UI under \'About\' on the Integration Card.\n\n   ![About popup for the \'TestAdapter\' Management Pack](doc/test-adapter-about.png)\n\n   *This Management Pack\'s vendor is \'VMware\'*\n\n6. `Enter a path to a EULA text file, or leave blank for no EULA`\n\n   VMware Aria Operations requires a EULA file to be present in a Management Pack. If one isn\'t provided, a stub EULA file (`eula.txt` in\n   the root project directory) will be added to the project which reads:\n    ```\n    There is no EULA associated with this Management Pack.\n    ```\n\n7. `Enter a path to the Management Pack icon file, or leave blank for no icon`\n\n   The icon is used in the VMware Aria Operations UI if present. If it is not present, a default icon will be used. The icon file must be\n   png format and 256x256 px. An icon file can be added later by copying the icon to the root project directory and\n   setting the value of the `"pak_icon"` key to the icon\'s file name in the `manifest.txt` file.\n\n8. `Select a language for the adapter. Supported languages are [...]`\n\n   Supported languages are listed. Once selected, the project will be generated, including a template adapter in the\n   selected language. The template adapter collects several objects and metrics from the container that the adapter \n   is running in, and can be used as a starting point for creating a new adapter.\n\nFor complete documentation of the `mp-init` tool see the [MP Initialization Tool Documentation](doc/mp-init.md).\n\n### Testing a Management Pack\n\nIn the Management Pack directory, the installation script writes a `requirements.txt` file containing the version of the\nSDK used to generate the project, and installs the SDK into a virtual environment named `venv`. Note that the packages\nin `requirements.txt` are _not_ installed into the adapter. To add a package to the adapter, specify it in the file\n`adapter_requirements.txt`. \n\nTo use the SDK, navigate to the newly-generated project directory and activate the virtual environment:\n\nFor Mac and Linux:\n```sh\nsource venv/bin/activate\n```\n(This script is written for the bash shell. If you use the csh or fish shells, there are alternate activate.csh and activate.fish scripts you should use instead.)\nFor Windows:\n```cmd\nvenv\\Scripts\\activate.bat\n```\nTo exit the virtual environment, run `deactivate` in the virtual environment.\n\nTo test a project, run `mp-test`  in the virtual environment.\n\nIf `mp-test` is run from anywhere outside of a root project directory, the tool will prompt to choose a project, and will\ntest the selected project. If the tool is run from a project directory, the tool will automatically test that project.\n\n`mp-test` will ask for a _connection_. No connections should exist, so choose **New Connection**. The test tool then\nreads the `conf/describe.xml` file to find the connection parameters and credentials required for a connection, and\nprompts for each. This is similar to creating a new _Adapter Instance_ in the VMware Aria Operations UI. Connections are automatically\nsaved per project, and can be reused when re-running the `mp-test` tool.\n\n> Note: In the template project, the only connection parameter is `ID`, and because it connects to the container it is running on, this parameter is not necessary; it is only there as an example, and can be set to any value. The template also implements an example Test Connection. If a Test Connection is run (see below), with the `ID` set to the text `bad`, then the Test Connection will fail.\n\nThe test tool also asks for the method to test. There are four options:\n\n* Test Connection - This call tests the connection and returns either an error message if the connection failed, or an\n  empty json object if the connection succeeded.\n* Collect - This call test the collection, and returns objects, metrics, properties, events, and relationships.\n* Endpoint URLs - This returns a list (possibly empty) of URLs that have distinct SSL certificates that VMware Aria Operations can ask\n  the end user to import into the TrustStore.\n* Version - This returns\n  the [VMware Aria Operations Collector API](vmware_aria_operations_integration_sdk/api/vmware-aria-operations-collector-fwk2.json) version the\n  adapter implements. The implementation of this method is not generally handled by the developer.\n\nFor more information on these endpoints, see\nthe [Swagger API documentation](vmware_aria_operations_integration_sdk/api/vmware-aria-operations-collector-fwk2.json). Each\nresponse is validated against the API.\n\nFor complete documentation of the `mp-test` tool see the [MP Test Tool Documentation](doc/mp-test.md).\n\n### Building and Installing a Management Pack\nTo build a project, run `mp-build`  in the virtual environment.\n\nIf `mp-build` is run from anywhere outside of a root project directory, the tool will prompt to choose a project, and will\nbuild the selected project. If the tool is run from a project directory, the tool will automatically build that\nproject.\n\nOnce the project is selected (if necessary), the tool will build the management pack and emit a `pak` file which can be \ninstalled on VMware Aria Operations. The `pak` file will be located in the project directory.\n\nTo install the `pak` file, in VMware Aria Operations navigate to **Data Sources &rarr; Integrations &rarr;\nRepository** and click `ADD`. Select and upload the generated `pak` file, accept the README, and install the management pack.\n\nTo configure the management pack, VMware Aria Operations navigate to **Data Sources &rarr; Integrations &rarr;\nAccounts** and click `ADD ACCOUNT`. Select the newly-installed management pack and configure the required fields. For \n`Collector/Group`, make sure that a cloud proxy collector is selected. Click `VALIDATE CONNECTION` to test the connection. \nIt should return successfully, then click `ADD`.\n\nBy default, a collection will run every 5 minutes. The first collection should happen immediately, however newly-created\nobjects cannot have metrics, properties, and events added to them. After the second collection, approximately five\nminutes later, the objects\' metrics, properties, and events should appear. These can be checked by navigating to **\nEnvironment &rarr; Object Browser &rarr; All Objects** and expanding the Adapter and associated object types and object.\n\n![CPU Idle Time](doc/test-adapter-cpu-idle-time.png)\n*The CPU object\'s `idle-time` metric in a Management Pack named `QAAdapterName`.*\n\nFor complete documentation of the `mp-build` tool see the [MP Build Tool Documentation](doc/mp-build.md).\n\n## Contributing\n\nThe vmware-aria-operations-integration-sdk project team welcomes contributions from the community. Before you start\nworking with this project please read and sign our Contributor License Agreement (https://cla.vmware.com/cla/1/preview).\nIf you wish to contribute code and you have not signed our Contributor Licence Agreement (CLA), our bot will prompt you\nto do so when you open a Pull Request. For any questions about the CLA process, please refer to our\n[FAQ](https://cla.vmware.com/faq).\n\n## License\n\nThis project is licensed under the APACHE-2 License.\n',
+    'long_description': 'VMware Aria Operations Integration SDK\n=====================\n\nWelcome to the VMware Aria Operations Integration SDK. \n\n## What is the Integration SDK?\n\nThe Integration SDK creates Management Packs to add custom objects, data, and \nrelationships from a endpoint into VMware Aria Operations. \n\nUsing this SDK to create a Management Pack requires some Python \nknowledge (more languages are planned), and an understanding of how to get \ndata from the endpoint using an API. For example, to create a Management Pack for \nCassandra DB, an understanding of how to write an SQL query, execute it, and read the \nresults is required.\n\nCurrently, installing a Management Pack built with the integration SDK is supported for \nOn-Prem versions of VMware Aria Operations only, but we are working to bring support to \nVMware Aria Operations Cloud in a future release.\n\nFor a high-level overview of VMware Aria Operations, Management Packs, and this SDK, \nsee [the introduction](doc/introduction.md).\n\n## What can the Integration SDK be used for?\nThe Integration SDK can be used to add any endpoint that supports remote monitoring to \nVMware Aria Operations. Adding the endpoint involves creating objects that \nrepresent the endpoint, which may include properties, metrics, and events, as well as\nrelationships between objects.\n\n**Remote monitoring** uses an API (such as REST, SNMP, SQL, etc) to retrieve the data (as\nopposed to agent-based monitoring, where the monitoring code runs in the same location\nas the endpoint).\n\nFor an example walkthrough of creating a new Management Pack monitoring an endpoint, see\n[Creating a new Management Pack for Cassandra DB](#creating-a-new-management-pack--cassandra-db-)\n\nThe Integration SDK can also be used to extend objects created by another Management\nPack with additional metrics, properties, events, or relationships. This can be useful\nto ensure access to custom data without having to re-implement already existing data.\n\nFor an example walkthrough of the steps required to extend another management pack, see \n[Extending the Existing Management Pack for MySQL](#extending-an-existing-management-pack--mysql-)\n\n## Where should I start?\n* If you want to get started creating your first Management Pack, or don\'t know where to start, read the [Get Started](#get-started) tutorial.\n* If you have completed the Get Started tutorial, the [walkthroughs](#walkthroughs) are guides for modifying your adapter.\n* All documentation is available from the [contents](doc/contents.md) page.\n\n## Get Started\n<details>\n<summary>This guide will walk through setting up the SDK and using the SDK\nto create, test, and install a simple Management Pack (integration) onto VMware Aria Operations.</summary>\n\nContents\n* [Requirements](#requirements)\n* [Installation](#installation)\n* [Creating a Management Pack](#creating-a-management-pack)\n* [Testing a Management Pack](#testing-a-management-pack)\n* [Building and Installing a Management Pack](#building-and-installing-a-management-pack)\n\n### Requirements\n\n#### Operating System:\nThe VMware Aria Operations Integration SDK has been tested in the following OSes:\n* Windows 10\n* Windows 11\n* macOS Monterey\n* Debian Linux\n* Fedora Linux\n    \nOther operating systems may be compatible.\n\n#### VMware Aria Operations\nThe Management Packs generated by the VMware Aria Operations Integration SDK will only run on versions that supports containerized Management Packs. Currently, this is limited to on-prem installs, version 8.10 or later.\nIn addition, at least one Cloud Proxy (also version 8.10 or later) must be set up in VMware Aria Operations, as containerized Management Packs must be run on a Cloud Proxy collector.\n\n#### Dependencies\n* Docker 20.10.0 or later. Updating to the latest stable version is recommended. For instructions on installing Docker,\n  go to [Docker\'s installation documentation](https://docs.docker.com/engine/install/), choose the OS you need and\n  follow the instructions provided.\n* Python3 3.9.0 or later. Updating to the latest stable version is recommended. Python 3.8 and earlier (including Python2) are not supported. For instructions on installing Python, go\n  to [Python\'s installation documentation](https://wiki.python.org/moin/BeginnersGuide/Download), choose the OS you need\n  and follow the instructions provided.\n* Pip. If Python3 is installed, pip is most likely also installed. For instructions on installing Pip, go\n  to [Pip\'s installation documentation](https://pip.pypa.io/en/stable/installation/), and follow the instructions\n  provided.\n* Git 2.35.0 or later. Updating to the latest stable version is recommended. \n  For instructions in installing git, go to [Git\'s installation documentation](https://git-scm.com/downloads),\n  choose the OS you need and follow the instructions provided.\n\n[//]: # (TODO: Add this section back in once we support them)\n[//]: # (#### Optional Prerequisites)\n[//]: # (* Java. Java is only required for building Java Management Packs. We recommend the latest version of the [Azul Zulu SDK]&#40;https://www.azul.com/downloads/?package=jdk#download-openjdk&#41;.)\n[//]: # (* Powershell. Powershell is only required for building Powershell Management Packs. See [Microsoft\'s installation instructions for PowerShell]&#40;https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell?view=powershell-7.2&#41;.)\n[//]: # (> Note: Creating Java and Powershell Management Packs is disabled for the Beta)\n\n### Installation\n\nTo install the SDK, use `pip` to install into the global Python environment, or `pipx` to install into a isolated environment.\n```sh\npython3 -m pip install vmware-aria-operations-integration-sdk\n```\n\n### Creating a Management Pack\nAfter the SDK is installed, create a new project, by running `mp-init`. This tool asks a series of questions that guides\nthe creation of a new management pack project. \n\n\n1. `Enter a path for the project (where code for collection, metadata, and content reside). Path:`\n\n    The path can be an absolute path, or a path relative to the directory `mp-init` was run from. The path should end in an empty\n    or non-existing directory. If the directory does not exist, it will be created. This directory will contain a new Management\n    Pack project.\n\n2. `Management Pack display name`\n\n    The Management Pack display name will show up in VMware Aria Operations (**Data Sources &rarr; Integrations &rarr;\n    Repository**), or when adding an account.\n\n    ![Integration Card for the \'TestAdapter\' Management Pack](doc/test-adapter-integration-card.png)\n\n    *This Management Pack\'s display name is \'TestAdapter\', and uses the default icon*\n\n3. `Management Pack adapter key`\n\n    This field is used internally to identify the Management Pack and Adapter Kind. By default, it is set to the \n    Management Pack display name with special characters and whitespace stripped from it.\n\n4. `Management Pack description`\n\n    This field should describe what the Management Pack will do or monitor.\n\n5. `Management Pack vendor`\n\n   The vendor field shows up in the UI under \'About\' on the Integration Card.\n\n   ![About popup for the \'TestAdapter\' Management Pack](doc/test-adapter-about.png)\n\n   *This Management Pack\'s vendor is \'VMware\'*\n\n6. `Enter a path to a EULA text file, or leave blank for no EULA`\n\n   VMware Aria Operations requires a EULA file to be present in a Management Pack. If one isn\'t provided, a stub EULA file (`eula.txt` in\n   the root project directory) will be added to the project which reads:\n    ```\n    There is no EULA associated with this Management Pack.\n    ```\n\n7. `Enter a path to the Management Pack icon file, or leave blank for no icon`\n\n   The icon is used in the VMware Aria Operations UI if present. If it is not present, a default icon will be used. The icon file must be\n   png format and 256x256 px. An icon file can be added later by copying the icon to the root project directory and\n   setting the value of the `"pak_icon"` key to the icon\'s file name in the `manifest.txt` file.\n\n8. `Select a language for the adapter. Supported languages are [...]`\n\n   Supported languages are listed. Once selected, the project will be generated, including a template adapter in the\n   selected language. The template adapter collects several objects and metrics from the container that the adapter \n   is running in, and can be used as a starting point for creating a new adapter.\n\nFor complete documentation of the `mp-init` tool see the [MP Initialization Tool Documentation](doc/mp-init.md).\n\n### Testing a Management Pack\n\nIn the Management Pack directory, the installation script writes a `requirements.txt` file containing the version of the\nSDK used to generate the project, and installs the SDK into a virtual environment named `venv`. Note that the packages\nin `requirements.txt` are _not_ installed into the adapter. To add a package to the adapter, specify it in the file\n`adapter_requirements.txt`. \n\nTo use the SDK, navigate to the newly-generated project directory and activate the virtual environment:\n\nFor Mac and Linux:\n```sh\nsource venv/bin/activate\n```\n(This script is written for the bash shell. If you use the csh or fish shells, there are alternate activate.csh and activate.fish scripts you should use instead.)\nFor Windows:\n```cmd\nvenv\\Scripts\\activate.bat\n```\nTo exit the virtual environment, run `deactivate` in the virtual environment.\n\nTo test a project, run `mp-test`  in the virtual environment.\n\nIf `mp-test` is run from anywhere outside of a root project directory, the tool will prompt to choose a project, and will\ntest the selected project. If the tool is run from a project directory, the tool will automatically test that project.\n\n`mp-test` will ask for a _connection_. No connections should exist, so choose **New Connection**. The test tool then\nreads the `conf/describe.xml` file to find the connection parameters and credentials required for a connection, and\nprompts for each. This is similar to creating a new _Adapter Instance_ in the VMware Aria Operations UI. Connections are automatically\nsaved per project, and can be reused when re-running the `mp-test` tool.\n\n> Note: In the template project, the only connection parameter is `ID`, and because it connects to the container it is running on, this parameter is not necessary; it is only there as an example, and can be set to any value. The template also implements an example Test Connection. If a Test Connection is run (see below), with the `ID` set to the text `bad`, then the Test Connection will fail.\n\nThe test tool also asks for the method to test. There are four options:\n\n* Test Connection - This call tests the connection and returns either an error message if the connection failed, or an\n  empty json object if the connection succeeded.\n* Collect - This call test the collection, and returns objects, metrics, properties, events, and relationships.\n* Endpoint URLs - This returns a list (possibly empty) of URLs that have distinct SSL certificates that VMware Aria Operations can ask\n  the end user to import into the TrustStore.\n* Version - This returns\n  the [VMware Aria Operations Collector API](vmware_aria_operations_integration_sdk/api/vmware-aria-operations-collector-fwk2.json) version the\n  adapter implements. The implementation of this method is not generally handled by the developer.\n\nFor more information on these endpoints, see\nthe [Swagger API documentation](vmware_aria_operations_integration_sdk/api/vmware-aria-operations-collector-fwk2.json). Each\nresponse is validated against the API.\n\nFor complete documentation of the `mp-test` tool see the [MP Test Tool Documentation](doc/mp-test.md).\n\n### Building and Installing a Management Pack\nTo build a project, run `mp-build`  in the virtual environment.\n\nIf `mp-build` is run from anywhere outside of a root project directory, the tool will prompt to choose a project, and will\nbuild the selected project. If the tool is run from a project directory, the tool will automatically build that\nproject.\n\nOnce the project is selected (if necessary), the tool will build the management pack and emit a `pak` file which can be \ninstalled on VMware Aria Operations. The `pak` file will be located in the project directory.\n\nTo install the `pak` file, in VMware Aria Operations navigate to **Data Sources &rarr; Integrations &rarr;\nRepository** and click `ADD`. Select and upload the generated `pak` file, accept the README, and install the management pack.\n\nTo configure the management pack, VMware Aria Operations navigate to **Data Sources &rarr; Integrations &rarr;\nAccounts** and click `ADD ACCOUNT`. Select the newly-installed management pack and configure the required fields. For \n`Collector/Group`, make sure that a cloud proxy collector is selected. Click `VALIDATE CONNECTION` to test the connection. \nIt should return successfully, then click `ADD`.\n\nBy default, a collection will run every 5 minutes. The first collection should happen immediately, however newly-created\nobjects cannot have metrics, properties, and events added to them. After the second collection, approximately five\nminutes later, the objects\' metrics, properties, and events should appear. These can be checked by navigating to **\nEnvironment &rarr; Object Browser &rarr; All Objects** and expanding the Adapter and associated object types and object.\n\n![CPU Idle Time](doc/test-adapter-cpu-idle-time.png)\n*The CPU object\'s `idle-time` metric in a Management Pack named `QAAdapterName`.*\n\nFor complete documentation of the `mp-build` tool see the [MP Build Tool Documentation](doc/mp-build.md).\n</details>\n\n## Walkthroughs\n\n### Creating a New Management Pack (Cassandra-DB)\n<details><summary>\nThis guide assumes you have already set up the SDK and know how to create a new project. \nIt walks you through the steps necessary to monitor an endpoint, using Cassandra DB as \nan example.</summary>\nTODO\n</details>\n\n### Extending an Existing Management Pack (MySQL)\n<details><summary>\nThis guide assumes you have already set up the SDK and know how to create a new project. \nIt walks you through the steps necessary to extend an existing Management Pact to add\nadditional data, using the MySQL Management Pack as an example.</summary>\nTODO\n</details>\n\n\n## Troubleshooting\nTODO\n\n## Contributing\n\nThe vmware-aria-operations-integration-sdk project team welcomes contributions from the community. Before you start\nworking with this project please read and sign our Contributor License Agreement (https://cla.vmware.com/cla/1/preview).\nIf you wish to contribute code and you have not signed our Contributor Licence Agreement (CLA), our bot will prompt you\nto do so when you open a Pull Request. For any questions about the CLA process, please refer to our\n[FAQ](https://cla.vmware.com/faq).\n\n## License\n\nThis project is licensed under the APACHE-2 License.\n',
     'author': 'Kyle Rokos',
     'author_email': 'krokos@vmware.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/vmware/vrealize-operations-integration-sdk',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `vmware_aria_operations_integration_sdk-0.5.0rc2/PKG-INFO` & `vmware_aria_operations_integration_sdk-0.5.0rc3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmware-aria-operations-integration-sdk
-Version: 0.5.0rc2
+Version: 0.5.0rc3
 Summary: A set of tools to help users create, test, and build containerized management packs for VMware Aria Operations
 Home-page: https://github.com/vmware/vrealize-operations-integration-sdk
 License: Apache-2.0
 Author: Kyle Rokos
 Author-email: krokos@vmware.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -33,23 +33,61 @@
 Description-Content-Type: text/markdown
 
 VMware Aria Operations Integration SDK
 =====================
 
 Welcome to the VMware Aria Operations Integration SDK. 
 
-Where should I start?
-* If you want to get started creating your first Management Pack, or don't know where to start, read the 'Get Started' tutorial below.
-* If you'd like an introduction to VMware Aria Operations, Management Packs, and this SDK, [read the introduction](doc/introduction.md).
+## What is the Integration SDK?
+
+The Integration SDK creates Management Packs to add custom objects, data, and 
+relationships from a endpoint into VMware Aria Operations. 
+
+Using this SDK to create a Management Pack requires some Python 
+knowledge (more languages are planned), and an understanding of how to get 
+data from the endpoint using an API. For example, to create a Management Pack for 
+Cassandra DB, an understanding of how to write an SQL query, execute it, and read the 
+results is required.
+
+Currently, installing a Management Pack built with the integration SDK is supported for 
+On-Prem versions of VMware Aria Operations only, but we are working to bring support to 
+VMware Aria Operations Cloud in a future release.
+
+For a high-level overview of VMware Aria Operations, Management Packs, and this SDK, 
+see [the introduction](doc/introduction.md).
+
+## What can the Integration SDK be used for?
+The Integration SDK can be used to add any endpoint that supports remote monitoring to 
+VMware Aria Operations. Adding the endpoint involves creating objects that 
+represent the endpoint, which may include properties, metrics, and events, as well as
+relationships between objects.
+
+**Remote monitoring** uses an API (such as REST, SNMP, SQL, etc) to retrieve the data (as
+opposed to agent-based monitoring, where the monitoring code runs in the same location
+as the endpoint).
+
+For an example walkthrough of creating a new Management Pack monitoring an endpoint, see
+[Creating a new Management Pack for Cassandra DB](#creating-a-new-management-pack--cassandra-db-)
+
+The Integration SDK can also be used to extend objects created by another Management
+Pack with additional metrics, properties, events, or relationships. This can be useful
+to ensure access to custom data without having to re-implement already existing data.
+
+For an example walkthrough of the steps required to extend another management pack, see 
+[Extending the Existing Management Pack for MySQL](#extending-an-existing-management-pack--mysql-)
+
+## Where should I start?
+* If you want to get started creating your first Management Pack, or don't know where to start, read the [Get Started](#get-started) tutorial.
+* If you have completed the Get Started tutorial, the [walkthroughs](#walkthroughs) are guides for modifying your adapter.
 * All documentation is available from the [contents](doc/contents.md) page.
 
 ## Get Started
-
-This guide will walk through setting up the SDK and using the SDK
-to create, test, and install a simple Management Pack (integration) onto VMware Aria Operations.
+<details>
+<summary>This guide will walk through setting up the SDK and using the SDK
+to create, test, and install a simple Management Pack (integration) onto VMware Aria Operations.</summary>
 
 Contents
 * [Requirements](#requirements)
 * [Installation](#installation)
 * [Creating a Management Pack](#creating-a-management-pack)
 * [Testing a Management Pack](#testing-a-management-pack)
 * [Building and Installing a Management Pack](#building-and-installing-a-management-pack)
@@ -70,16 +108,15 @@
 The Management Packs generated by the VMware Aria Operations Integration SDK will only run on versions that supports containerized Management Packs. Currently, this is limited to on-prem installs, version 8.10 or later.
 In addition, at least one Cloud Proxy (also version 8.10 or later) must be set up in VMware Aria Operations, as containerized Management Packs must be run on a Cloud Proxy collector.
 
 #### Dependencies
 * Docker 20.10.0 or later. Updating to the latest stable version is recommended. For instructions on installing Docker,
   go to [Docker's installation documentation](https://docs.docker.com/engine/install/), choose the OS you need and
   follow the instructions provided.
-* Python3 3.9.0 or later. Earlier versions of Python3 may also work, but updating to the latest stable version is
-  recommended. Python 3.8 and earlier (including Python2) are not supported. For instructions on installing Python, go
+* Python3 3.9.0 or later. Updating to the latest stable version is recommended. Python 3.8 and earlier (including Python2) are not supported. For instructions on installing Python, go
   to [Python's installation documentation](https://wiki.python.org/moin/BeginnersGuide/Download), choose the OS you need
   and follow the instructions provided.
 * Pip. If Python3 is installed, pip is most likely also installed. For instructions on installing Pip, go
   to [Pip's installation documentation](https://pip.pypa.io/en/stable/installation/), and follow the instructions
   provided.
 * Git 2.35.0 or later. Updating to the latest stable version is recommended. 
   For instructions in installing git, go to [Git's installation documentation](https://git-scm.com/downloads),
@@ -229,14 +266,37 @@
 minutes later, the objects' metrics, properties, and events should appear. These can be checked by navigating to **
 Environment &rarr; Object Browser &rarr; All Objects** and expanding the Adapter and associated object types and object.
 
 ![CPU Idle Time](doc/test-adapter-cpu-idle-time.png)
 *The CPU object's `idle-time` metric in a Management Pack named `QAAdapterName`.*
 
 For complete documentation of the `mp-build` tool see the [MP Build Tool Documentation](doc/mp-build.md).
+</details>
+
+## Walkthroughs
+
+### Creating a New Management Pack (Cassandra-DB)
+<details><summary>
+This guide assumes you have already set up the SDK and know how to create a new project. 
+It walks you through the steps necessary to monitor an endpoint, using Cassandra DB as 
+an example.</summary>
+TODO
+</details>
+
+### Extending an Existing Management Pack (MySQL)
+<details><summary>
+This guide assumes you have already set up the SDK and know how to create a new project. 
+It walks you through the steps necessary to extend an existing Management Pact to add
+additional data, using the MySQL Management Pack as an example.</summary>
+TODO
+</details>
+
+
+## Troubleshooting
+TODO
 
 ## Contributing
 
 The vmware-aria-operations-integration-sdk project team welcomes contributions from the community. Before you start
 working with this project please read and sign our Contributor License Agreement (https://cla.vmware.com/cla/1/preview).
 If you wish to contribute code and you have not signed our Contributor Licence Agreement (CLA), our bot will prompt you
 to do so when you open a Pull Request. For any questions about the CLA process, please refer to our
```

