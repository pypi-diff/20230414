# Comparing `tmp/nonebot-plugin-sentry-0.2.2.tar.gz` & `tmp/nonebot_plugin_sentry-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-sentry-0.2.2.tar", max compression
+gzip compressed data, was "nonebot_plugin_sentry-0.3.0.tar", max compression
```

## Comparing `nonebot-plugin-sentry-0.2.2.tar` & `nonebot_plugin_sentry-0.3.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rwxr-xr-x   0        0        0     2341 2020-11-23 14:15:55.010344 nonebot-plugin-sentry-0.2.2/README.md
--rwxr-xr-x   0        0        0     1267 2021-06-18 12:03:08.004715 nonebot-plugin-sentry-0.2.2/__init__.py
--rwxr-xr-x   0        0        0     1658 2021-06-10 15:48:15.220927 nonebot-plugin-sentry-0.2.2/config.py
--rwxr-xr-x   0        0        0      848 2021-06-18 12:03:52.280053 nonebot-plugin-sentry-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3264 2021-06-18 12:04:03.318580 nonebot-plugin-sentry-0.2.2/setup.py
--rw-r--r--   0        0        0     3291 2021-06-18 12:04:03.318836 nonebot-plugin-sentry-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1413 2023-04-14 09:29:05.547658 nonebot_plugin_sentry-0.3.0/README.md
+-rw-r--r--   0        0        0     1131 2023-04-14 09:29:05.547658 nonebot_plugin_sentry-0.3.0/__init__.py
+-rw-r--r--   0        0        0     1071 2023-04-14 09:29:05.547658 nonebot_plugin_sentry-0.3.0/config.py
+-rw-r--r--   0        0        0      844 2023-04-14 09:29:05.547658 nonebot_plugin_sentry-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 nonebot_plugin_sentry-0.3.0/PKG-INFO
```

### Comparing `nonebot-plugin-sentry-0.2.2/__init__.py` & `nonebot_plugin_sentry-0.3.0/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 @Author         : yanyongyu
 @Date           : 2020-11-23 18:44:25
 @LastEditors    : yanyongyu
-@LastEditTime   : 2021-06-18 20:03:07
-@Description    : None
+@LastEditTime   : 2023-03-30 19:58:06
+@Description    : Sentry plugin
 @GitHub         : https://github.com/yanyongyu
 """
 __author__ = "yanyongyu"
 
 import sentry_sdk
 from nonebot import get_driver
 from nonebot.log import logger
@@ -18,33 +18,28 @@
 from .config import Config
 
 driver = get_driver()
 global_config = driver.config
 config = Config(**global_config.dict())
 
 
-class Filter:
-
-    def __init__(self, level="INFO") -> None:
-        self.level = level
-
-    def __call__(self, record):
-        levelno = logger.level(self.level).no
-        return record["level"].no >= levelno
-
-
-def init(config: Config):
+def init_sentry(config: Config):
     sentry_config = {
         key[7:]: value
-        for key, value in config.dict().items()
-        if key != "sentry_environment"
+        for key, value in config.dict(exclude={"sentry_environment"}).items()
     }
-    sentry_sdk.init(**sentry_config,
-                    environment=config.sentry_environment or driver.env,
-                    default_integrations=False)
-
-    logger.add(EventHandler("ERROR"), filter=Filter("ERROR"))
-    logger.add(BreadcrumbHandler("INFO"), filter=Filter("INFO"))
+    sentry_sdk.init(
+        **sentry_config, environment=config.sentry_environment or driver.env
+    )
+
+    logger.add(
+        EventHandler("ERROR"),
+        filter=lambda r: r["level"].no >= logger.level("ERROR").no,
+    )
+    logger.add(
+        BreadcrumbHandler("INFO"),
+        filter=lambda r: r["level"].no >= logger.level("INFO").no,
+    )
 
 
 if config.sentry_dsn:
-    init(config)
+    init_sentry(config)
```

### Comparing `nonebot-plugin-sentry-0.2.2/pyproject.toml` & `nonebot_plugin_sentry-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "nonebot-plugin-sentry"
-version = "0.2.2"
+version = "0.3.0"
 description = "Push your bot errors to Sentry.io"
 license = "MIT"
-authors = ["yanyongyu <yanyongyu_1@126.com>"]
+authors = ["yanyongyu <yyy@nonebot.dev>"]
 readme = "README.md"
 homepage = "https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry"
 repository = "https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry"
 documentation = "https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry#readme"
 keywords = ["nonebot", "nonebot2", "sentry"]
 packages = [
     { include = "nonebot_plugin_sentry/*.py", from = ".." }
```

### Comparing `nonebot-plugin-sentry-0.2.2/PKG-INFO` & `nonebot_plugin_sentry-0.3.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-sentry
-Version: 0.2.2
+Version: 0.3.0
 Summary: Push your bot errors to Sentry.io
 Home-page: https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry
 License: MIT
 Keywords: nonebot,nonebot2,sentry
 Author: yanyongyu
-Author-email: yanyongyu_1@126.com
+Author-email: yyy@nonebot.dev
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: nonebot2 (>=2.0.0-alpha.6,<3.0.0)
 Requires-Dist: sentry-sdk (>=1.0.0,<2.0.0)
 Project-URL: Documentation, https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry#readme
 Project-URL: Repository, https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry
 Description-Content-Type: text/markdown
 
 <!--
  * @Author         : yanyongyu
  * @Date           : 2020-11-23 20:23:12
  * @LastEditors    : yanyongyu
- * @LastEditTime   : 2020-11-23 22:15:54
+ * @LastEditTime   : 2023-04-14 17:04:28
  * @Description    : None
  * @GitHub         : https://github.com/yanyongyu
 -->
 
 <p align="center">
   <a href="https://v2.nonebot.dev/">
-    <img src="https://raw.githubusercontent.com/nonebot/nonebot2/master/docs/.vuepress/public/logo.png" height="100" alt="nonebot">
+    <img src="https://v2.nonebot.dev/logo.png" height="100" alt="nonebot">
   </a>
   <a href="https://sentry.io">
     <img src="https://sentry-brand.storage.googleapis.com/sentry-logo-black.png" height="100" alt="sentry">
   </a>
 </p>
 
 <div align="center">
@@ -57,31 +59,11 @@
 
 ## 使用方式
 
 填写必须配置项 `SENTRY_DSN` ，即刻开始 sentry 之旅！
 
 ## 配置项
 
-配置项具体含义参考: [Sentry Docs](https://docs.sentry.io/platforms/python/configuration/options/)
+配置项需要添加前缀 `sentry_`，所有参数以及具体含义参考: [Sentry Docs](https://docs.sentry.io/platforms/python/configuration/options/)
 
-- `sentry_dsn: str`
-- `sentry_debug: bool = False`
-- `sentry_release: Optional[str] = None`
-- `sentry_release: Optional[str] = None`
-- `sentry_environment: Optional[str] = nonebot env`
-- `sentry_server_name: Optional[str] = None`
-- `sentry_sample_rate: float = 1.`
-- `sentry_max_breadcrumbs: int = 100`
-- `sentry_attach_stacktrace: bool = False`
-- `sentry_send_default_pii: bool = False`
-- `sentry_in_app_include: List[str] = Field(default_factory=lambda: [])`
-- `sentry_in_app_exclude: List[str] = Field(default_factory=lambda: [])`
-- `sentry_request_bodies: str = "medium"`
-- `sentry_with_locals: bool = True`
-- `sentry_ca_certs: Optional[str] = None`
-- `sentry_before_send: Optional[Callable[[Any, Any], Optional[Any]]] = None`
-- `sentry_before_breadcrumb: Optional[Callable[[Any, Any], Optional[Any]]] = None`
-- `sentry_transport: Optional[Any] = None`
-- `sentry_http_proxy: Optional[str] = None`
-- `sentry_https_proxy: Optional[str] = None`
-- `sentry_shutdown_timeout: int = 2`
+所有以 `sentry_` 开头的配置项将会被自动读取。
```

#### html2text {}

```diff
@@ -1,33 +1,23 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-sentry Version: 0.2.2 Summary: Push
+Metadata-Version: 2.1 Name: nonebot-plugin-sentry Version: 0.3.0 Summary: Push
 your bot errors to Sentry.io Home-page: https://github.com/cscs181/QQ-GitHub-
 Bot/tree/master/src/plugins/nonebot_plugin_sentry License: MIT Keywords:
-nonebot,nonebot2,sentry Author: yanyongyu Author-email: yanyongyu_1@126.com
+nonebot,nonebot2,sentry Author: yanyongyu Author-email: yyy@nonebot.dev
 Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Requires-Dist: nonebot2
-(>=2.0.0-alpha.6,<3.0.0) Requires-Dist: sentry-sdk (>=1.0.0,<2.0.0) Project-
-URL: Documentation, https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/
-plugins/nonebot_plugin_sentry#readme Project-URL: Repository, https://
-github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry
-Description-Content-Type: text/markdown
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nonebot2 (>=2.0.0-alpha.6,<3.0.0) Requires-Dist: sentry-sdk
+(>=1.0.0,<2.0.0) Project-URL: Documentation, https://github.com/cscs181/QQ-
+GitHub-Bot/tree/master/src/plugins/nonebot_plugin_sentry#readme Project-URL:
+Repository, https://github.com/cscs181/QQ-GitHub-Bot/tree/master/src/plugins/
+nonebot_plugin_sentry Description-Content-Type: text/markdown
                               [nonebot] [sentry]
          # nonebot-plugin-sentry _â¨ å¨ Sentry.io ä¸è¿è¡ NoneBot
                     æå¡æ¥å¿æ¥çãéè¯¯å¤ç â¨_
                            [license] [pypi] [python]
 ## ä½¿ç¨æ¹å¼ å¡«åå¿é¡»éç½®é¡¹ `SENTRY_DSN` ï¼å³å»å¼å§ sentry
-ä¹æï¼ ## éç½®é¡¹ éç½®é¡¹å·ä½å«ä¹åè: [Sentry Docs](https://
-docs.sentry.io/platforms/python/configuration/options/) - `sentry_dsn: str` -
-`sentry_debug: bool = False` - `sentry_release: Optional[str] = None` -
-`sentry_release: Optional[str] = None` - `sentry_environment: Optional[str] =
-nonebot env` - `sentry_server_name: Optional[str] = None` -
-`sentry_sample_rate: float = 1.` - `sentry_max_breadcrumbs: int = 100` -
-`sentry_attach_stacktrace: bool = False` - `sentry_send_default_pii: bool =
-False` - `sentry_in_app_include: List[str] = Field(default_factory=lambda: [])`
-- `sentry_in_app_exclude: List[str] = Field(default_factory=lambda: [])` -
-`sentry_request_bodies: str = "medium"` - `sentry_with_locals: bool = True` -
-`sentry_ca_certs: Optional[str] = None` - `sentry_before_send: Optional
-[Callable[[Any, Any], Optional[Any]]] = None` - `sentry_before_breadcrumb:
-Optional[Callable[[Any, Any], Optional[Any]]] = None` - `sentry_transport:
-Optional[Any] = None` - `sentry_http_proxy: Optional[str] = None` -
-`sentry_https_proxy: Optional[str] = None` - `sentry_shutdown_timeout: int = 2`
+ä¹æï¼ ## éç½®é¡¹ éç½®é¡¹éè¦æ·»å åç¼
+`sentry_`ï¼ææåæ°ä»¥åå·ä½å«ä¹åè: [Sentry Docs](https://
+docs.sentry.io/platforms/python/configuration/options/) ææä»¥ `sentry_`
+å¼å¤´çéç½®é¡¹å°ä¼è¢«èªå¨è¯»åã
```

