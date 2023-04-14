# Comparing `tmp/decanter-ai-sdk-0.1.7.tar.gz` & `tmp/decanter-ai-sdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decanter-ai-sdk-0.1.7.tar", max compression
+gzip compressed data, was "decanter-ai-sdk-0.1.8.tar", max compression
```

## Comparing `decanter-ai-sdk-0.1.7.tar` & `decanter-ai-sdk-0.1.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1069 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/LICENSE
--rw-r--r--   0        0        0     4508 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/README.md
--rw-r--r--   0        0        0       22 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/__init__.py
--rw-r--r--   0        0        0    21752 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/client.py
--rw-r--r--   0        0        0      696 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/enums/algorithms.py
--rw-r--r--   0        0        0      132 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/enums/data_types.py
--rw-r--r--   0        0        0     1018 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/enums/evaluators.py
--rw-r--r--   0        0        0      372 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/enums/missing_value_handling.py
--rw-r--r--   0        0        0      152 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/enums/status.py
--rw-r--r--   0        0        0      118 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/enums/time_units.py
--rw-r--r--   0        0        0     5382 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/experiment.py
--rw-r--r--   0        0        0      285 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/model.py
--rw-r--r--   0        0        0    24678 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/non_blocking_client.py
--rw-r--r--   0        0        0      669 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/prediction.py
--rw-r--r--   0        0        0     1189 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/api.py
--rw-r--r--   0        0        0    15145 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/iid_exp.json
--rw-r--r--   0        0        0      897 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/iid_predict.json
--rw-r--r--   0        0        0     1914 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/iid_test_table.json
--rw-r--r--   0        0        0     1914 2023-04-10 09:46:38.541767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/iid_train_table.json
--rw-r--r--   0        0        0    80346 2023-04-10 09:46:38.545767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/model_list.json
--rw-r--r--   0        0        0      365 2023-04-10 09:46:38.545767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/table_info.json
--rw-r--r--   0        0        0     4128 2023-04-10 09:46:38.545767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/table_list.json
--rw-r--r--   0        0        0    39974 2023-04-10 09:46:38.545767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/ts_exp.json
--rw-r--r--   0        0        0      897 2023-04-10 09:46:38.545767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/ts_predict.json
--rw-r--r--   0        0        0     1914 2023-04-10 09:46:38.545767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/ts_test_table.json
--rw-r--r--   0        0        0     1914 2023-04-10 09:46:38.545767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/ts_train_table.json
--rw-r--r--   0        0        0     6441 2023-04-10 09:46:38.545767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/decanter_api.py
--rw-r--r--   0        0        0     2618 2023-04-10 09:46:38.545767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/iid_testing_api.py
--rw-r--r--   0        0        0     2645 2023-04-10 09:46:38.545767 decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/ts_testing_api.py
--rw-r--r--   0        0        0     1563 2023-04-10 09:46:38.545767 decanter-ai-sdk-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     5794 2023-04-10 09:46:51.110422 decanter-ai-sdk-0.1.7/setup.py
--rw-r--r--   0        0        0     5475 2023-04-10 09:46:51.110876 decanter-ai-sdk-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/LICENSE
+-rw-r--r--   0        0        0     4508 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/README.md
+-rw-r--r--   0        0        0       22 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/__init__.py
+-rw-r--r--   0        0        0    22632 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/client.py
+-rw-r--r--   0        0        0      696 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/algorithms.py
+-rw-r--r--   0        0        0      132 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/data_types.py
+-rw-r--r--   0        0        0     1018 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/evaluators.py
+-rw-r--r--   0        0        0      372 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/missing_value_handling.py
+-rw-r--r--   0        0        0      152 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/status.py
+-rw-r--r--   0        0        0      118 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/time_units.py
+-rw-r--r--   0        0        0     5382 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/experiment.py
+-rw-r--r--   0        0        0      285 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/model.py
+-rw-r--r--   0        0        0    24678 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/non_blocking_client.py
+-rw-r--r--   0        0        0      669 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/prediction.py
+-rw-r--r--   0        0        0     1189 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/api.py
+-rw-r--r--   0        0        0    15145 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_exp.json
+-rw-r--r--   0        0        0      897 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_predict.json
+-rw-r--r--   0        0        0     1914 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_test_table.json
+-rw-r--r--   0        0        0     1914 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_train_table.json
+-rw-r--r--   0        0        0    80346 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/model_list.json
+-rw-r--r--   0        0        0      365 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/table_info.json
+-rw-r--r--   0        0        0     4128 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/table_list.json
+-rw-r--r--   0        0        0    39974 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_exp.json
+-rw-r--r--   0        0        0      897 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_predict.json
+-rw-r--r--   0        0        0     1914 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_test_table.json
+-rw-r--r--   0        0        0     1914 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_train_table.json
+-rw-r--r--   0        0        0     7513 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/decanter_api.py
+-rw-r--r--   0        0        0     2618 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/iid_testing_api.py
+-rw-r--r--   0        0        0     2645 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/ts_testing_api.py
+-rw-r--r--   0        0        0     1563 2023-04-14 02:25:34.989975 decanter-ai-sdk-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     5794 2023-04-14 02:25:48.049560 decanter-ai-sdk-0.1.8/setup.py
+-rw-r--r--   0        0        0     5475 2023-04-14 02:25:48.050036 decanter-ai-sdk-0.1.8/PKG-INFO
```

### Comparing `decanter-ai-sdk-0.1.7/LICENSE` & `decanter-ai-sdk-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/README.md` & `decanter-ai-sdk-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/client.py` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -594,7 +594,39 @@
 
         Returns:
         ----------
             (float)
                 threshold
         """
         return self.api.get_model_threshold(experiment_id, model_id)
+
+    def get_performance_metrics(self, model_id, table_id) -> List:
+        """
+        Return metrics and threshold in specific model and table.
+
+        Classification problem returns numeric value to be threshold, and regression problem returns np.nan
+
+        Args:
+            model_id
+            table_id
+
+        Returns:
+        ----------
+            (List)
+                List of dictionary including all metrics and threshold for specific model.
+
+        """
+        return self.api.get_performance_metrics(model_id, table_id)
+
+    def delete_experiment(self, experiment_id) -> str:
+        """
+        Return "Experiment delete successful" or "Experiment does not exist"
+
+        Args:
+            experiment_id
+
+        Returns:
+        ----------
+            (str)
+                API's message
+        """
+        return self.api.delete_experiment(experiment_id)
```

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/enums/algorithms.py` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/algorithms.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/enums/evaluators.py` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/enums/evaluators.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/experiment.py` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/experiment.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/non_blocking_client.py` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/non_blocking_client.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/prediction.py` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/prediction.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/api.py` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/api.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/iid_exp.json` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_exp.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/iid_predict.json` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_predict.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/iid_test_table.json` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_test_table.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/iid_train_table.json` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/iid_train_table.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/model_list.json` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/model_list.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/table_list.json` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/table_list.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/ts_exp.json` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_exp.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/ts_predict.json` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_predict.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/ts_test_table.json` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_test_table.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/data/ts_train_table.json` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/data/ts_train_table.json`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/decanter_api.py` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/decanter_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-from typing import Dict
+from typing import Dict, List
 from io import StringIO
 import json
 import requests
 import pandas as pd
+import numpy as np
 
 from decanter_ai_sdk.web_api.api import ApiClient
 
 
 class DecanterApiClient(ApiClient):
     def __init__(self, host, headers, auth_headers, project_id):  # pragma: no cover
         self.url = host + "/v1/"
@@ -176,24 +177,43 @@
         res = requests.get(
             f"{self.url}experiment/{experiment_id}/model/getlist?projectId={self.project_id}",
             headers=self.auth_headers,
             verify=False,
         )
         return res.json()["model_list"]
 
-    def get_model_threshold(self, experiment_id, model_id):  # pragma: no cover
+    def get_model_threshold(self, experiment_id, model_id) -> float:
 
         res = requests.get(
-            f"{self.url}experiment/{experiment_id}/model/{model_id}",
+            f"{self.url}experiment/{experiment_id}/model/{model_id}/predict_threshold",
             headers=self.headers,
+            params={"project_id": self.project_id},
+            verify=False,
+        )
+        return res.json()["threshold"]
+
+    def get_performance_metrics(self, model_id, table_id) -> List:
+        res = requests.get(
+            f"{self.url}prediction/getlist/{model_id}",
             verify=False,
+            params={"project_id": self.project_id},
+            headers=self.headers,
         )
-        return res.json()["model"]["attributes"]["auc"]["cv_average"]["th_max_by"][
-            "evaluator"
+        res_pred = res.json()["predictions"]
+        perf_list = [
+            {
+                "metrics": res_pred[x]["performance"]["metrics"],
+                "threshold": res_pred[x]["threshold"]
+                if "threshold" in list(res_pred[0].keys())
+                else np.nan,
+            }
+            for x in range(len(res_pred))
+            if res_pred[x]["table_id"] == table_id
         ]
+        return perf_list
 
     def stop_uploading(self, id) -> bool:  # pragma: no cover
         res = requests.post(
             f"{self.url}table/stop",
             headers=self.auth_headers,
             verify=False,
             data={"table_id": id, "project_id": self.project_id},
@@ -204,7 +224,20 @@
         res = requests.post(
             f"{self.url}experiment/stop",
             headers=self.auth_headers,
             verify=False,
             data={"experiment_id": id, "project_id": self.project_id},
         )
         return res.ok
+
+    def delete_experiment(self, experiment_id) -> str:
+
+        res = requests.post(
+            f"{self.url}experiment/delete",
+            headers=self.headers,
+            data=json.dumps(
+                {"project_id": self.project_id, "experiment_id": experiment_id}
+            ),
+            verify=False,
+        )
+
+        return res.json()["message"]
```

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/iid_testing_api.py` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/iid_testing_api.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/decanter_ai_sdk/web_api/ts_testing_api.py` & `decanter-ai-sdk-0.1.8/decanter_ai_sdk/web_api/ts_testing_api.py`

 * *Files identical despite different names*

### Comparing `decanter-ai-sdk-0.1.7/pyproject.toml` & `decanter-ai-sdk-0.1.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "decanter-ai-sdk"
-version = "0.1.7"
+version = "0.1.8"
 description = "Decanter AI is a powerful AutoML tool which enables everyone to build ML models and make predictions without data science background. With Decanter AI SDK, you can integrate Decanter AI into your application more easily with Python."
 homepage = "https://github.com/MoBagel/decanter-ai-sdk"
 authors = ["senchao <senchao@mobagel.com>"]
 readme = "README.md"
 include = [
   "README.md"
 ]
```

### Comparing `decanter-ai-sdk-0.1.7/setup.py` & `decanter-ai-sdk-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pydantic>=1.9.2,<2.0.0',
  'pytest>=7.1.2,<8.0.0',
  'requests-toolbelt>=0.9.1,<0.10.0',
  'tqdm>=4.64.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'decanter-ai-sdk',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Decanter AI is a powerful AutoML tool which enables everyone to build ML models and make predictions without data science background. With Decanter AI SDK, you can integrate Decanter AI into your application more easily with Python.',
     'long_description': '[![Coverage Status](https://coveralls.io/repos/github/MoBagel/decanter-ai-sdk/badge.svg?branch=coveralls)](https://coveralls.io/github/MoBagel/decanter-ai-sdk?branch=coveralls)\n[![tests](https://github.com/MoBagel/decanter-ai-sdk/workflows/main/badge.svg)](https://github.com/MoBagel/decanter-ai-sdk)\n[![PyPI version](https://badge.fury.io/py/decanter-ai-sdk.svg)](https://badge.fury.io/py/decanter-ai-sdk)\n# Mobagel decanter ai sdk\n\nDecanter AI is a powerful AutoML tool which enables everyone to build ML models and make predictions without data science background. With Decanter AI SDK, you can integrate Decanter AI into your application more easily with Python.\n\nIt supports actions such as data uploading, model training, and prediction to run in a more efficient way and access results more easily.\n\nTo know more about Decanter AI and how you can be benefited with AutoML, visit [MoBagel website](https://mobagel.com/tw/) and contact us to try it out!\n\n## How it works\n\n- Upload train and test files in both csv and pandas dataframe.\n- Setup different standards and conduct customized experiments on uploaded data.\n- Use different models to run predictions\n- Get predict data in pandas dataframe form.\n\n## Requirements\n\n- [Python >= 3.8](https://www.python.org/downloads/release/python-380/)\n- [poetry](https://python-poetry.org/)\n\n## Usage\n\n### Installation\n\n`pip install decanter-ai-sdk`\n### Constructor\nTo use this sdk, you must first construct a client object.\n```python\nfrom decanter_ai_sdk.client import Client\n    client = Client(\n        auth_key="auth_API_key",\n        project_id="project_id",\n        host="host_url",\n    )\n```\n\n### Upload\nAfter the client is constructed, now you can use it to upload your training and testing files in both csv and pandas dataframe. This function will return uploaded data id in Decanter server.\n```python\nimport os\nsys.path.append("..")\n\ncurrent_path = os.path.dirname(os.path.abspath(__file__))\ntrain_file_path = os.path.join(current_path, "ts_train.csv")\ntrain_file = open(train_file_path, "rb")\ntrain_id = client.upload(train_file, "train_file")\n```\n\n### Experiment\nTo conduct an experiment, you need to first specify which type of data you are going to use , i.e., iid or ts, then you can input parameters by following our pyhint to customize your experiment.\nAfter the experiment, the function will return an object which you can get experiment attributes from it.\n```python\n# Training iid data\nexperiment = client.train_iid(\n    experiment_name=exp_name,\n    experiment_table_id=train_id,\n    target="Survived",\n    evaluator=ClassificationMetric.AUC,\n    custom_feature_types={\n        "Pclass": DataType.categorical,\n        "Parch": DataType.categorical,\n    },\n)\n```\n\n```python\n# Training ts data\nexperiment = client.train_ts(\n    experiment_name=exp_name,\n    experiment_table_id=train_id,\n    target="Passengers",\n    datetime="Month",\n    time_groups=[],\n    timeunit=TimeUnit.month,\n    groupby_method="sum",\n    max_model=5,\n    evaluator=RegressionMetric.MAPE,\n    custom_feature_types={"Pclass": DataType.numerical},\n)\n```\nTo get its attributes, you can either extract them by simply using dot or its functions.\n```python\n# Experiment object usage\nbest_model = experiment.get_best_model()\nmodel_list = experiment.get_model_list()\nbest_auc_model = experiment.get_best_model_by_metric(ClassificationMetric.AUC)\n```\n### Prediction\nNow you can use model data to run prediction.\n```python\n# Predicting iid data\npredict = client.predict_iid(\n    keep_columns=[], \n    non_negative=False, \n    test_table_id=test_id, \n    model=best_model\n)\n```\n\n```python\n# Predicting ts data\npredict = client.predict_ts(\n    keep_columns=[], \n    non_negative=False, \n    test_table_id=test_id, \n    model=best_model\n)\n```\nTo get prediction result, do\n```python\npredict_data = predict.get_predict_df()\n```\n## Development\n\n### Installing poetry\n\n1. `pip install poetry poethepoet`\n2. `poetry install` #Project setup.\n3. `poetry shell` #Start your project in poetry env.\n\nNow you can create your own branch to start developing new feature.\n\n### Testing\nTo run test, do:\n```\npoe test\n```\n\n### Lint and format\nTo lint, do:\n```\npoe lint\n```\n\nTo reformat, do:\n```\npoe format\n```\n\n## Releasing\n1. poetry version [new_version]\n2. git commit -m"Bump version"\n3. git push origin main\n4. create new release on github.\n5. Create release off main branch, auto generate notes, and review release note.\n6. Publish release\n\n## Enums\n#TODO\n\n## License\n#TODO\n\n## TODO\n#TODO\n\n\n\n',
     'author': 'senchao',
     'author_email': 'senchao@mobagel.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/MoBagel/decanter-ai-sdk',
```

### Comparing `decanter-ai-sdk-0.1.7/PKG-INFO` & `decanter-ai-sdk-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decanter-ai-sdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: Decanter AI is a powerful AutoML tool which enables everyone to build ML models and make predictions without data science background. With Decanter AI SDK, you can integrate Decanter AI into your application more easily with Python.
 Home-page: https://github.com/MoBagel/decanter-ai-sdk
 Author: senchao
 Author-email: senchao@mobagel.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

