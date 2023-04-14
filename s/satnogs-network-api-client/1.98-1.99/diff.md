# Comparing `tmp/satnogs-network-api-client-1.98.tar.gz` & `tmp/satnogs-network-api-client-1.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satnogs-network-api-client-1.98.tar", last modified: Thu Dec 15 10:13:58 2022, max compression
+gzip compressed data, was "satnogs-network-api-client-1.99.tar", last modified: Thu Dec 15 12:07:32 2022, max compression
```

## Comparing `satnogs-network-api-client-1.98.tar` & `satnogs-network-api-client-1.99.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:58.408345 satnogs-network-api-client-1.98/
--rw-rw-rw-   0 root         (0) root         (0)    34521 2022-12-15 10:01:55.000000 satnogs-network-api-client-1.98/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-15 10:01:55.000000 satnogs-network-api-client-1.98/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      867 2022-12-15 10:13:58.408345 satnogs-network-api-client-1.98/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      426 2022-12-15 10:01:55.000000 satnogs-network-api-client-1.98/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:58.389343 satnogs-network-api-client-1.98/satnogs_network_api_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      867 2022-12-15 10:13:58.000000 satnogs-network-api-client-1.98/satnogs_network_api_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2714 2022-12-15 10:13:58.000000 satnogs-network-api-client-1.98/satnogs_network_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-15 10:13:58.000000 satnogs-network-api-client-1.98/satnogs_network_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2022-12-15 10:13:58.000000 satnogs-network-api-client-1.98/satnogs_network_api_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2022-12-15 10:13:58.000000 satnogs-network-api-client-1.98/satnogs_network_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:58.409345 satnogs-network-api-client-1.98/satnogsnetworkapiclient/
--rw-r--r--   0 root         (0) root         (0)      826 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/__init__.py
--rw-r--r--   0 root         (0) root         (0)      496 2022-12-15 10:13:58.409345 satnogs-network-api-client-1.98/satnogsnetworkapiclient/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:58.394343 satnogs-network-api-client-1.98/satnogsnetworkapiclient/api/
--rw-r--r--   0 root         (0) root         (0)      233 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8649 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/api/configuration_api.py
--rw-r--r--   0 root         (0) root         (0)    13188 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/api/jobs_api.py
--rw-r--r--   0 root         (0) root         (0)    27128 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/api/observations_api.py
--rw-r--r--   0 root         (0) root         (0)     4594 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/api/station_api.py
--rw-r--r--   0 root         (0) root         (0)     9945 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/api/stations_api.py
--rw-r--r--   0 root         (0) root         (0)     9332 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/api/transmitters_api.py
--rw-r--r--   0 root         (0) root         (0)    36938 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:58.394343 satnogs-network-api-client-1.98/satnogsnetworkapiclient/apis/
--rw-r--r--   0 root         (0) root         (0)      831 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17019 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5076 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:58.400344 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/
--rw-r--r--   0 root         (0) root         (0)      348 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11126 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/demod_data.py
--rw-r--r--   0 root         (0) root         (0)    12942 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/job.py
--rw-r--r--   0 root         (0) root         (0)    12377 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/new_observation.py
--rw-r--r--   0 root         (0) root         (0)    22490 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/observation.py
--rw-r--r--   0 root         (0) root         (0)    11944 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/paginated_observation_list.py
--rw-r--r--   0 root         (0) root         (0)    11904 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/paginated_station_list.py
--rw-r--r--   0 root         (0) root         (0)    11944 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/paginated_transmitter_list.py
--rw-r--r--   0 root         (0) root         (0)    23739 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/patched_observation.py
--rw-r--r--   0 root         (0) root         (0)    14939 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/station.py
--rw-r--r--   0 root         (0) root         (0)    13780 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/station_configuration.py
--rw-r--r--   0 root         (0) root         (0)    11233 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/transmitter.py
--rw-r--r--   0 root         (0) root         (0)    11762 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/transmitter_type_enum.py
--rw-r--r--   0 root         (0) root         (0)    11992 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/update_observation.py
--rw-r--r--   0 root         (0) root         (0)    81907 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:58.400344 satnogs-network-api-client-1.98/satnogsnetworkapiclient/models/
--rw-r--r--   0 root         (0) root         (0)     1364 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12689 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 10:13:58.408345 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      851 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_configuration_api.py
--rw-r--r--   0 root         (0) root         (0)      751 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_demod_data.py
--rw-r--r--   0 root         (0) root         (0)      708 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_job.py
--rw-r--r--   0 root         (0) root         (0)      770 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_jobs_api.py
--rw-r--r--   0 root         (0) root         (0)      786 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_new_observation.py
--rw-r--r--   0 root         (0) root         (0)      862 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_observation.py
--rw-r--r--   0 root         (0) root         (0)     1194 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_observations_api.py
--rw-r--r--   0 root         (0) root         (0)      962 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_paginated_observation_list.py
--rw-r--r--   0 root         (0) root         (0)      918 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_paginated_station_list.py
--rw-r--r--   0 root         (0) root         (0)      962 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_paginated_transmitter_list.py
--rw-r--r--   0 root         (0) root         (0)      912 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_patched_observation.py
--rw-r--r--   0 root         (0) root         (0)      736 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_station.py
--rw-r--r--   0 root         (0) root         (0)      713 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_station_api.py
--rw-r--r--   0 root         (0) root         (0)      828 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_station_configuration.py
--rw-r--r--   0 root         (0) root         (0)      806 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_stations_api.py
--rw-r--r--   0 root         (0) root         (0)      764 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_transmitter.py
--rw-r--r--   0 root         (0) root         (0)      822 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_transmitter_type_enum.py
--rw-r--r--   0 root         (0) root         (0)      842 2022-12-15 10:03:05.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_transmitters_api.py
--rw-r--r--   0 root         (0) root         (0)      807 2022-12-15 10:03:04.000000 satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_update_observation.py
--rw-rw-rw-   0 root         (0) root         (0)     1071 2022-12-15 10:13:58.408345 satnogs-network-api-client-1.98/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      136 2022-12-15 10:01:55.000000 satnogs-network-api-client-1.98/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    68573 2022-12-15 10:01:55.000000 satnogs-network-api-client-1.98/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:32.620183 satnogs-network-api-client-1.99/
+-rw-rw-rw-   0 root         (0) root         (0)    34521 2022-12-15 11:55:31.000000 satnogs-network-api-client-1.99/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-15 11:55:31.000000 satnogs-network-api-client-1.99/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      867 2022-12-15 12:07:32.621183 satnogs-network-api-client-1.99/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      426 2022-12-15 11:55:31.000000 satnogs-network-api-client-1.99/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:32.601181 satnogs-network-api-client-1.99/satnogs_network_api_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      867 2022-12-15 12:07:32.000000 satnogs-network-api-client-1.99/satnogs_network_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2714 2022-12-15 12:07:32.000000 satnogs-network-api-client-1.99/satnogs_network_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-12-15 12:07:32.000000 satnogs-network-api-client-1.99/satnogs_network_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2022-12-15 12:07:32.000000 satnogs-network-api-client-1.99/satnogs_network_api_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2022-12-15 12:07:32.000000 satnogs-network-api-client-1.99/satnogs_network_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:32.622183 satnogs-network-api-client-1.99/satnogsnetworkapiclient/
+-rw-r--r--   0 root         (0) root         (0)      826 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      496 2022-12-15 12:07:32.622183 satnogs-network-api-client-1.99/satnogsnetworkapiclient/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:32.606181 satnogs-network-api-client-1.99/satnogsnetworkapiclient/api/
+-rw-r--r--   0 root         (0) root         (0)      233 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8649 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/api/configuration_api.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/api/jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)    27128 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/api/observations_api.py
+-rw-r--r--   0 root         (0) root         (0)     4594 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/api/station_api.py
+-rw-r--r--   0 root         (0) root         (0)     9945 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/api/stations_api.py
+-rw-r--r--   0 root         (0) root         (0)     9332 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/api/transmitters_api.py
+-rw-r--r--   0 root         (0) root         (0)    36938 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:32.607181 satnogs-network-api-client-1.99/satnogsnetworkapiclient/apis/
+-rw-r--r--   0 root         (0) root         (0)      831 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17019 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5076 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:32.612182 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/
+-rw-r--r--   0 root         (0) root         (0)      348 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11126 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/demod_data.py
+-rw-r--r--   0 root         (0) root         (0)    12942 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/job.py
+-rw-r--r--   0 root         (0) root         (0)    12377 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/new_observation.py
+-rw-r--r--   0 root         (0) root         (0)    22490 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/observation.py
+-rw-r--r--   0 root         (0) root         (0)    11944 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/paginated_observation_list.py
+-rw-r--r--   0 root         (0) root         (0)    11904 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/paginated_station_list.py
+-rw-r--r--   0 root         (0) root         (0)    11944 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/paginated_transmitter_list.py
+-rw-r--r--   0 root         (0) root         (0)    23739 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/patched_observation.py
+-rw-r--r--   0 root         (0) root         (0)    14939 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/station.py
+-rw-r--r--   0 root         (0) root         (0)    13780 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/station_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    11233 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/transmitter.py
+-rw-r--r--   0 root         (0) root         (0)    11762 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/transmitter_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)    11992 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/update_observation.py
+-rw-r--r--   0 root         (0) root         (0)    81907 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:32.613182 satnogs-network-api-client-1.99/satnogsnetworkapiclient/models/
+-rw-r--r--   0 root         (0) root         (0)     1364 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12689 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-15 12:07:32.620183 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      851 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_configuration_api.py
+-rw-r--r--   0 root         (0) root         (0)      751 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_demod_data.py
+-rw-r--r--   0 root         (0) root         (0)      708 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_job.py
+-rw-r--r--   0 root         (0) root         (0)      770 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_jobs_api.py
+-rw-r--r--   0 root         (0) root         (0)      786 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_new_observation.py
+-rw-r--r--   0 root         (0) root         (0)      862 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_observation.py
+-rw-r--r--   0 root         (0) root         (0)     1194 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_observations_api.py
+-rw-r--r--   0 root         (0) root         (0)      962 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_paginated_observation_list.py
+-rw-r--r--   0 root         (0) root         (0)      918 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_paginated_station_list.py
+-rw-r--r--   0 root         (0) root         (0)      962 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_paginated_transmitter_list.py
+-rw-r--r--   0 root         (0) root         (0)      912 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_patched_observation.py
+-rw-r--r--   0 root         (0) root         (0)      736 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_station.py
+-rw-r--r--   0 root         (0) root         (0)      713 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_station_api.py
+-rw-r--r--   0 root         (0) root         (0)      828 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_station_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      806 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_stations_api.py
+-rw-r--r--   0 root         (0) root         (0)      764 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_transmitter.py
+-rw-r--r--   0 root         (0) root         (0)      822 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_transmitter_type_enum.py
+-rw-r--r--   0 root         (0) root         (0)      842 2022-12-15 11:56:42.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_transmitters_api.py
+-rw-r--r--   0 root         (0) root         (0)      807 2022-12-15 11:56:41.000000 satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_update_observation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2022-12-15 12:07:32.621183 satnogs-network-api-client-1.99/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      136 2022-12-15 11:55:31.000000 satnogs-network-api-client-1.99/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    68573 2022-12-15 11:55:31.000000 satnogs-network-api-client-1.99/versioneer.py
```

### Comparing `satnogs-network-api-client-1.98/LICENSE` & `satnogs-network-api-client-1.99/LICENSE`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/PKG-INFO` & `satnogs-network-api-client-1.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satnogs-network-api-client
-Version: 1.98
+Version: 1.99
 Summary: SatNOGS Network API Client
 Home-page: https://gitlab.com/librespacefoundation/satnogs/satnogs-network
 Author: SatNOGS project
 Author-email: dev@satnogs.org
 License: AGPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `satnogs-network-api-client-1.98/satnogs_network_api_client.egg-info/PKG-INFO` & `satnogs-network-api-client-1.99/satnogs_network_api_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: satnogs-network-api-client
-Version: 1.98
+Version: 1.99
 Summary: SatNOGS Network API Client
 Home-page: https://gitlab.com/librespacefoundation/satnogs/satnogs-network
 Author: SatNOGS project
 Author-email: dev@satnogs.org
 License: AGPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `satnogs-network-api-client-1.98/satnogs_network_api_client.egg-info/SOURCES.txt` & `satnogs-network-api-client-1.99/satnogs_network_api_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/__init__.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/api/configuration_api.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/api/configuration_api.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/api/jobs_api.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/api/jobs_api.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/api/observations_api.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/api/observations_api.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/api/station_api.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/api/station_api.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/api/stations_api.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/api/stations_api.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/api/transmitters_api.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/api/transmitters_api.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/api_client.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/api_client.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/apis/__init__.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/configuration.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/configuration.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/exceptions.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/demod_data.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/demod_data.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/job.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/job.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/new_observation.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/new_observation.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/observation.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/observation.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/paginated_observation_list.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/paginated_observation_list.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/paginated_station_list.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/paginated_station_list.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/paginated_transmitter_list.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/paginated_transmitter_list.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/patched_observation.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/patched_observation.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/station.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/station.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/station_configuration.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/station_configuration.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/transmitter.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/transmitter.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/transmitter_type_enum.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/transmitter_type_enum.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/model/update_observation.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/model/update_observation.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/model_utils.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/model_utils.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/models/__init__.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/models/__init__.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/rest.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/rest.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_configuration_api.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_configuration_api.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_demod_data.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_demod_data.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_job.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_job.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_jobs_api.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_jobs_api.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_new_observation.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_new_observation.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_observation.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_observation.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_observations_api.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_observations_api.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_paginated_observation_list.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_paginated_observation_list.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_paginated_station_list.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_paginated_station_list.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_paginated_transmitter_list.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_paginated_transmitter_list.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_patched_observation.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_patched_observation.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_station.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_station.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_station_api.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_station_api.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_station_configuration.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_station_configuration.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_stations_api.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_stations_api.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_transmitter.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_transmitter.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_transmitter_type_enum.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_transmitter_type_enum.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_transmitters_api.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_transmitters_api.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/satnogsnetworkapiclient/test/test_update_observation.py` & `satnogs-network-api-client-1.99/satnogsnetworkapiclient/test/test_update_observation.py`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/setup.cfg` & `satnogs-network-api-client-1.99/setup.cfg`

 * *Files identical despite different names*

### Comparing `satnogs-network-api-client-1.98/versioneer.py` & `satnogs-network-api-client-1.99/versioneer.py`

 * *Files identical despite different names*

