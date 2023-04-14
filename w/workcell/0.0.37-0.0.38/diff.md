# Comparing `tmp/workcell-0.0.37.tar.gz` & `tmp/workcell-0.0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workcell-0.0.37.tar", max compression
+gzip compressed data, was "workcell-0.0.38.tar", max compression
```

## Comparing `workcell-0.0.37.tar` & `workcell-0.0.38.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0    11306 2023-04-01 15:38:31.016743 workcell-0.0.37/LICENSE
--rw-r--r--   0        0        0     6912 2023-04-01 15:38:31.016743 workcell-0.0.37/README.md
--rw-r--r--   0        0        0      931 2023-04-01 15:38:31.024743 workcell-0.0.37/pyproject.toml
--rw-r--r--   0        0        0      227 2023-04-01 15:38:31.024743 workcell-0.0.37/workcell/__init__.py
--rw-r--r--   0        0        0      140 2023-04-01 15:38:31.024743 workcell-0.0.37/workcell/cli/__init__.py
--rw-r--r--   0        0        0     5136 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/cli/builder.py
--rw-r--r--   0        0        0    16721 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/cli/cli.py
--rw-r--r--   0        0        0      178 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/cli/export.py
--rw-r--r--   0        0        0      546 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/cli/utils.py
--rw-r--r--   0        0        0      105 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/core/__init__.py
--rw-r--r--   0        0        0     1384 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/core/components.py
--rw-r--r--   0        0        0      737 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/core/constants.py
--rw-r--r--   0        0        0     3884 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/core/errors.py
--rw-r--r--   0        0        0     6040 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/core/networking.py
--rw-r--r--   0        0        0     6850 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/core/routes.py
--rw-r--r--   0        0        0     2261 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/core/serialization.py
--rw-r--r--   0        0        0     9642 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/core/spec.py
--rw-r--r--   0        0        0    11375 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/core/utils.py
--rw-r--r--   0        0        0     9837 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/core/workcell.py
--rw-r--r--   0        0        0        0 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/deploy/__init__.py
--rw-r--r--   0        0        0       40 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/deploy/huggingface/__init__.py
--rw-r--r--   0        0        0      875 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/deploy/huggingface/utils.py
--rw-r--r--   0        0        0     4166 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/deploy/huggingface/wrapper.py
--rw-r--r--   0        0        0      270 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/integrations/types/__init__.py
--rw-r--r--   0        0        0      670 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/integrations/types/altair.py
--rw-r--r--   0        0        0      218 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/integrations/types/dummy.py
--rw-r--r--   0        0        0      855 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/integrations/types/file.py
--rw-r--r--   0        0        0      288 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/integrations/types/markdown.py
--rw-r--r--   0        0        0      605 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/integrations/types/pandas.py
--rw-r--r--   0        0        0     1117 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/integrations/types/perspective.py
--rw-r--r--   0        0        0      483 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/integrations/types/plotly.py
--rw-r--r--   0        0        0        0 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/integrations/types/s3.py
--rw-r--r--   0        0        0      320 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/integrations/types/svg.py
--rw-r--r--   0        0        0     1495 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/templates/frontend/index.html
--rw-r--r--   0        0        0      734 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/templates/runtime/huggingface/python3.8/Dockerfile
--rw-r--r--   0        0        0        8 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/templates/runtime/huggingface/python3.8/requirements.txt
--rw-r--r--   0        0        0      734 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/templates/runtime/huggingface/python3.9/Dockerfile
--rw-r--r--   0        0        0        8 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/templates/runtime/huggingface/python3.9/requirements.txt
--rw-r--r--   0        0        0      734 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/templates/scaffold/huggingface/python3.8/Dockerfile
--rw-r--r--   0        0        0      256 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/templates/scaffold/huggingface/python3.8/app.py
--rw-r--r--   0        0        0        8 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/templates/scaffold/huggingface/python3.8/requirements.txt
--rw-r--r--   0        0        0      194 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/templates/scaffold/huggingface/python3.8/workcell.yaml
--rw-r--r--   0        0        0      734 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/templates/scaffold/huggingface/python3.9/Dockerfile
--rw-r--r--   0        0        0      256 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/templates/scaffold/huggingface/python3.9/app.py
--rw-r--r--   0        0        0        8 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/templates/scaffold/huggingface/python3.9/requirements.txt
--rw-r--r--   0        0        0      194 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/templates/scaffold/huggingface/python3.9/workcell.yaml
--rw-r--r--   0        0        0        0 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/utils/__init__.py
--rw-r--r--   0        0        0     1387 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/utils/encryptor.py
--rw-r--r--   0        0        0    27159 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/utils/processing_utils.py
--rw-r--r--   0        0        0     1034 2023-04-01 15:38:31.028743 workcell-0.0.37/workcell/utils/serve.py
--rw-r--r--   0        0        0     8059 1970-01-01 00:00:00.000000 workcell-0.0.37/PKG-INFO
+-rw-r--r--   0        0        0    11306 2023-04-14 08:12:44.963596 workcell-0.0.38/LICENSE
+-rw-r--r--   0        0        0     6912 2023-04-14 08:12:44.963596 workcell-0.0.38/README.md
+-rw-r--r--   0        0        0      931 2023-04-14 08:12:44.975596 workcell-0.0.38/pyproject.toml
+-rw-r--r--   0        0        0      227 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/__init__.py
+-rw-r--r--   0        0        0      140 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/cli/__init__.py
+-rw-r--r--   0        0        0     5136 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/cli/builder.py
+-rw-r--r--   0        0        0    16876 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/cli/cli.py
+-rw-r--r--   0        0        0      178 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/cli/export.py
+-rw-r--r--   0        0        0      546 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/cli/utils.py
+-rw-r--r--   0        0        0      105 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/core/__init__.py
+-rw-r--r--   0        0        0     1384 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/core/components.py
+-rw-r--r--   0        0        0      737 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/core/constants.py
+-rw-r--r--   0        0        0     3884 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/core/errors.py
+-rw-r--r--   0        0        0     6040 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/core/networking.py
+-rw-r--r--   0        0        0     6850 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/core/routes.py
+-rw-r--r--   0        0        0     2261 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/core/serialization.py
+-rw-r--r--   0        0        0     9642 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/core/spec.py
+-rw-r--r--   0        0        0    11375 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/core/utils.py
+-rw-r--r--   0        0        0     9837 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/core/workcell.py
+-rw-r--r--   0        0        0        0 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/deploy/__init__.py
+-rw-r--r--   0        0        0       40 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/deploy/huggingface/__init__.py
+-rw-r--r--   0        0        0      875 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/deploy/huggingface/utils.py
+-rw-r--r--   0        0        0     4166 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/deploy/huggingface/wrapper.py
+-rw-r--r--   0        0        0      270 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/integrations/types/__init__.py
+-rw-r--r--   0        0        0      670 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/integrations/types/altair.py
+-rw-r--r--   0        0        0      218 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/integrations/types/dummy.py
+-rw-r--r--   0        0        0      855 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/integrations/types/file.py
+-rw-r--r--   0        0        0      288 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/integrations/types/markdown.py
+-rw-r--r--   0        0        0      605 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/integrations/types/pandas.py
+-rw-r--r--   0        0        0     1117 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/integrations/types/perspective.py
+-rw-r--r--   0        0        0      483 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/integrations/types/plotly.py
+-rw-r--r--   0        0        0        0 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/integrations/types/s3.py
+-rw-r--r--   0        0        0      320 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/integrations/types/svg.py
+-rw-r--r--   0        0        0     1495 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/templates/frontend/index.html
+-rw-r--r--   0        0        0      734 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/templates/runtime/huggingface/python3.8/Dockerfile
+-rw-r--r--   0        0        0        8 2023-04-14 08:12:44.975596 workcell-0.0.38/workcell/templates/runtime/huggingface/python3.8/requirements.txt
+-rw-r--r--   0        0        0      734 2023-04-14 08:12:44.979596 workcell-0.0.38/workcell/templates/runtime/huggingface/python3.9/Dockerfile
+-rw-r--r--   0        0        0        8 2023-04-14 08:12:44.979596 workcell-0.0.38/workcell/templates/runtime/huggingface/python3.9/requirements.txt
+-rw-r--r--   0        0        0      734 2023-04-14 08:12:44.979596 workcell-0.0.38/workcell/templates/scaffold/huggingface/python3.8/Dockerfile
+-rw-r--r--   0        0        0      256 2023-04-14 08:12:44.979596 workcell-0.0.38/workcell/templates/scaffold/huggingface/python3.8/app.py
+-rw-r--r--   0        0        0        8 2023-04-14 08:12:44.979596 workcell-0.0.38/workcell/templates/scaffold/huggingface/python3.8/requirements.txt
+-rw-r--r--   0        0        0      194 2023-04-14 08:12:44.979596 workcell-0.0.38/workcell/templates/scaffold/huggingface/python3.8/workcell.yaml
+-rw-r--r--   0        0        0      734 2023-04-14 08:12:44.979596 workcell-0.0.38/workcell/templates/scaffold/huggingface/python3.9/Dockerfile
+-rw-r--r--   0        0        0      256 2023-04-14 08:12:44.979596 workcell-0.0.38/workcell/templates/scaffold/huggingface/python3.9/app.py
+-rw-r--r--   0        0        0        8 2023-04-14 08:12:44.979596 workcell-0.0.38/workcell/templates/scaffold/huggingface/python3.9/requirements.txt
+-rw-r--r--   0        0        0      194 2023-04-14 08:12:44.979596 workcell-0.0.38/workcell/templates/scaffold/huggingface/python3.9/workcell.yaml
+-rw-r--r--   0        0        0        0 2023-04-14 08:12:44.979596 workcell-0.0.38/workcell/utils/__init__.py
+-rw-r--r--   0        0        0     1387 2023-04-14 08:12:44.979596 workcell-0.0.38/workcell/utils/encryptor.py
+-rw-r--r--   0        0        0    27159 2023-04-14 08:12:44.979596 workcell-0.0.38/workcell/utils/processing_utils.py
+-rw-r--r--   0        0        0     1034 2023-04-14 08:12:44.979596 workcell-0.0.38/workcell/utils/serve.py
+-rw-r--r--   0        0        0     7133 2023-04-14 08:12:44.979596 workcell-0.0.38/workcell/utils/strings.py
+-rw-r--r--   0        0        0     8059 1970-01-01 00:00:00.000000 workcell-0.0.38/PKG-INFO
```

### Comparing `workcell-0.0.37/LICENSE` & `workcell-0.0.38/LICENSE`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/README.md` & `workcell-0.0.38/README.md`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/pyproject.toml` & `workcell-0.0.38/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "workcell"
-version = "0.0.37"
+version = "0.0.38"
 description = "Turn python function into microservice."
 authors = ["jiandong <jiandong@weanalyze.co>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
```

### Comparing `workcell-0.0.37/workcell/cli/builder.py` & `workcell-0.0.38/workcell/cli/builder.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/cli/cli.py` & `workcell-0.0.38/workcell/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,29 +104,34 @@
         )
         raise
     return None
 
 
 @cli.command()
 def serve(
-    workcell_entrypoint: str,
+    entrypoint: str,
     config_path: Path = typer.Option(
         None, "--config", "-c", callback=conf_callback, is_eager=True
     ),
     port: int = typer.Option(int(WORKCELL_SERVER_PORT), "--port", "-p"),
     host: str = typer.Option(str(WORKCELL_SERVER_NAME), "--host", "-h"),
 ) -> None:
     """Start a HTTP API server for the workcell.
     This will launch a FastAPI server based on the OpenAPI standard and with a automatic interactive documentation.
     """
     if config_path:
         workcell_config = yaml.load(config_path.read_text(), Loader=yaml.Loader)
         launch_app(fn=workcell_config, host=host, port=port)
+    elif entrypoint:
+        launch_app(fn=entrypoint, host=host, port=port)
     else:
-        launch_app(fn=workcell_entrypoint, host=host, port=port)
+        typer.secho(
+            f"One of `entrypoint` and `config_path` arg must be set! ", fg=typer.colors.RED, err=True
+        )
+        return None
 
 
 @cli.command()
 def hello() -> None:
     """Say hello to workcell.
     This will create a `hello_workcell` project dir and serve it.
     """
@@ -214,15 +219,14 @@
     if not valid_workcell_import_string(import_string):
         typer.secho(
             f"Import function: {function_name} from app.py failed, check spelling or dependencies.",
             fg=typer.colors.RED,
             err=True,
         )
         return None
-
     # generate workcell_config
     workcell_config = gen_workcell_config(
         import_string=import_string,
         provider_name=provider_name,  # workcell provider name
         version=version,
         runtime=runtime,  # workcell runtime in [ "python3.8", ...]
         tags=tags,
```

### Comparing `workcell-0.0.37/workcell/cli/utils.py` & `workcell-0.0.38/workcell/cli/utils.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/core/components.py` & `workcell-0.0.38/workcell/core/components.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/core/constants.py` & `workcell-0.0.38/workcell/core/constants.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/core/errors.py` & `workcell-0.0.38/workcell/core/errors.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/core/networking.py` & `workcell-0.0.38/workcell/core/networking.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/core/routes.py` & `workcell-0.0.38/workcell/core/routes.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/core/serialization.py` & `workcell-0.0.38/workcell/core/serialization.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/core/spec.py` & `workcell-0.0.38/workcell/core/spec.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/core/utils.py` & `workcell-0.0.38/workcell/core/utils.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/core/workcell.py` & `workcell-0.0.38/workcell/core/workcell.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/deploy/huggingface/utils.py` & `workcell-0.0.38/workcell/deploy/huggingface/utils.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/deploy/huggingface/wrapper.py` & `workcell-0.0.38/workcell/deploy/huggingface/wrapper.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/integrations/types/altair.py` & `workcell-0.0.38/workcell/integrations/types/altair.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/integrations/types/file.py` & `workcell-0.0.38/workcell/integrations/types/file.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/integrations/types/pandas.py` & `workcell-0.0.38/workcell/integrations/types/pandas.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/integrations/types/perspective.py` & `workcell-0.0.38/workcell/integrations/types/perspective.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/templates/frontend/index.html` & `workcell-0.0.38/workcell/templates/frontend/index.html`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/templates/runtime/huggingface/python3.8/Dockerfile` & `workcell-0.0.38/workcell/templates/runtime/huggingface/python3.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/templates/runtime/huggingface/python3.9/Dockerfile` & `workcell-0.0.38/workcell/templates/runtime/huggingface/python3.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/templates/scaffold/huggingface/python3.8/Dockerfile` & `workcell-0.0.38/workcell/templates/scaffold/huggingface/python3.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/templates/scaffold/huggingface/python3.9/Dockerfile` & `workcell-0.0.38/workcell/templates/scaffold/huggingface/python3.9/Dockerfile`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/utils/encryptor.py` & `workcell-0.0.38/workcell/utils/encryptor.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/utils/processing_utils.py` & `workcell-0.0.38/workcell/utils/processing_utils.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/workcell/utils/serve.py` & `workcell-0.0.38/workcell/utils/serve.py`

 * *Files identical despite different names*

### Comparing `workcell-0.0.37/PKG-INFO` & `workcell-0.0.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: workcell
-Version: 0.0.37
+Version: 0.0.38
 Summary: Turn python function into microservice.
 License: Apache-2.0
 Author: jiandong
 Author-email: jiandong@weanalyze.co
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: workcell Version: 0.0.37 Summary: Turn python
+Metadata-Version: 2.1 Name: workcell Version: 0.0.38 Summary: Turn python
 function into microservice. License: Apache-2.0 Author: jiandong Author-email:
 jiandong@weanalyze.co Requires-Python: >=3.8 Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: altair
 (>=4.2.2,<5.0.0) Requires-Dist: fastapi (>=0.85.1,<0.86.0) Requires-Dist:
```

