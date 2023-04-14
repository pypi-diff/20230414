# Comparing `tmp/zen_dash-0.5.3.tar.gz` & `tmp/zen_dash-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zen_dash-0.5.3.tar", max compression
+gzip compressed data, was "zen_dash-0.5.4.tar", max compression
```

## Comparing `zen_dash-0.5.3.tar` & `zen_dash-0.5.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1070 2023-02-09 14:33:40.121808 zen_dash-0.5.3/LICENSE
--rw-r--r--   0        0        0     7635 2023-02-17 15:04:08.036446 zen_dash-0.5.3/README.md
--rw-r--r--   0        0        0     1289 2023-04-12 05:50:21.332964 zen_dash-0.5.3/pyproject.toml
--rw-r--r--   0        0        0       41 2023-04-12 05:50:21.332964 zen_dash-0.5.3/zen_dash/__init__.py
--rw-r--r--   0        0        0        0 2023-01-07 16:56:11.285785 zen_dash-0.5.3/zen_dash/cli/__init__.py
--rw-r--r--   0        0        0      227 2023-04-12 05:50:21.336964 zen_dash-0.5.3/zen_dash/cli/main.py
--rw-r--r--   0        0        0     5073 2023-04-12 05:50:21.336964 zen_dash-0.5.3/zen_dash/cli/project_management.py
--rw-r--r--   0        0        0      203 2023-04-12 05:50:21.336964 zen_dash-0.5.3/zen_dash/flex_data.py
--rw-r--r--   0        0        0      196 2023-04-12 05:50:21.336964 zen_dash-0.5.3/zen_dash/instances.py
--rw-r--r--   0        0        0     1079 2023-04-12 05:50:21.336964 zen_dash-0.5.3/zen_dash/objects/__init__.py
--rw-r--r--   0        0        0      291 2023-04-12 05:50:21.336964 zen_dash-0.5.3/zen_dash/objects/flex_data.py
--rw-r--r--   0        0        0    12356 2023-04-12 05:50:21.336964 zen_dash-0.5.3/zen_dash/objects/instances.py
--rw-r--r--   0        0        0      255 2023-04-12 05:50:21.336964 zen_dash-0.5.3/zen_dash/objects/page.py
--rw-r--r--   0        0        0      768 2023-04-12 05:50:21.336964 zen_dash-0.5.3/zen_dash/objects/scripts.py
--rw-r--r--   0        0        0      720 2023-04-12 05:50:21.336964 zen_dash-0.5.3/zen_dash/objects/sidebar.py
--rw-r--r--   0        0        0      919 2023-04-12 05:50:21.336964 zen_dash-0.5.3/zen_dash/page.py
--rw-r--r--   0        0        0        0 2023-04-12 05:50:21.336964 zen_dash-0.5.3/zen_dash/route.py
--rw-r--r--   0        0        0      191 2023-04-12 05:50:21.336964 zen_dash-0.5.3/zen_dash/scripts.py
--rw-r--r--   0        0        0      195 2023-04-12 05:50:21.336964 zen_dash-0.5.3/zen_dash/sidebar.py
--rw-r--r--   0        0        0  1017713 2023-04-12 05:52:55.071166 zen_dash-0.5.3/zen_dash/static/275.07215382ec6b3916.js
--rw-r--r--   0        0        0    57081 2023-04-12 05:52:55.071166 zen_dash-0.5.3/zen_dash/static/3rdpartylicenses.txt
--rw-r--r--   0        0        0   128180 2023-04-12 05:52:55.071166 zen_dash-0.5.3/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf
--rw-r--r--   0        0        0   143258 2023-04-12 05:52:55.071166 zen_dash-0.5.3/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot
--rw-r--r--   0        0        0    44300 2023-04-12 05:52:55.071166 zen_dash-0.5.3/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2
--rw-r--r--   0        0        0    57620 2023-04-12 05:52:55.071166 zen_dash-0.5.3/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff
--rw-r--r--   0        0        0      948 2023-04-12 05:52:55.071166 zen_dash-0.5.3/zen_dash/static/favicon.ico
--rw-r--r--   0        0        0     2073 2023-04-12 05:52:56.027180 zen_dash-0.5.3/zen_dash/static/index.html
--rw-r--r--   0        0        0  3105118 2023-04-12 05:52:55.071166 zen_dash-0.5.3/zen_dash/static/main.03cfb17449f365e9.js
--rw-r--r--   0        0        0    33759 2023-04-12 05:52:55.071166 zen_dash-0.5.3/zen_dash/static/polyfills.0a8881ff36766b1e.js
--rw-r--r--   0        0        0     3285 2023-04-12 05:52:55.071166 zen_dash-0.5.3/zen_dash/static/runtime.5615a939e3c41241.js
--rw-r--r--   0        0        0   152653 2023-04-12 05:52:55.071166 zen_dash-0.5.3/zen_dash/static/styles.362a8260c32d36d9.css
--rw-r--r--   0        0        0      621 2022-10-23 00:15:15.909625 zen_dash-0.5.3/zen_dash/support/__init__.py
--rw-r--r--   0        0        0      217 2023-04-12 05:50:21.352964 zen_dash-0.5.3/zen_dash/support/encoder.py
--rw-r--r--   0        0        0     6971 2023-04-10 07:23:01.329101 zen_dash-0.5.3/zen_dash/tag/__init__.py
--rw-r--r--   0        0        0     1513 2023-04-12 05:50:21.352964 zen_dash-0.5.3/zen_dash/websocket/__init__.py
--rw-r--r--   0        0        0     8869 2023-04-12 05:55:22.968384 zen_dash-0.5.3/setup.py
--rw-r--r--   0        0        0     8606 2023-04-12 05:55:22.968690 zen_dash-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-02-09 14:33:40.121808 zen_dash-0.5.4/LICENSE
+-rw-r--r--   0        0        0     7635 2023-02-17 15:04:08.036446 zen_dash-0.5.4/README.md
+-rw-r--r--   0        0        0     1281 2023-04-14 03:33:20.214857 zen_dash-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-04-12 05:50:21.332964 zen_dash-0.5.4/zen_dash/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-07 16:56:11.285785 zen_dash-0.5.4/zen_dash/cli/__init__.py
+-rw-r--r--   0        0        0      219 2023-04-14 03:33:36.095076 zen_dash-0.5.4/zen_dash/cli/main.py
+-rw-r--r--   0        0        0     5879 2023-04-14 03:33:25.986936 zen_dash-0.5.4/zen_dash/cli/project_management.py
+-rw-r--r--   0        0        0      203 2023-04-12 05:50:21.336964 zen_dash-0.5.4/zen_dash/flex_data.py
+-rw-r--r--   0        0        0      196 2023-04-12 05:50:21.336964 zen_dash-0.5.4/zen_dash/instances.py
+-rw-r--r--   0        0        0     1079 2023-04-12 05:50:21.336964 zen_dash-0.5.4/zen_dash/objects/__init__.py
+-rw-r--r--   0        0        0      291 2023-04-12 05:50:21.336964 zen_dash-0.5.4/zen_dash/objects/flex_data.py
+-rw-r--r--   0        0        0    12356 2023-04-12 05:50:21.336964 zen_dash-0.5.4/zen_dash/objects/instances.py
+-rw-r--r--   0        0        0      255 2023-04-12 05:50:21.336964 zen_dash-0.5.4/zen_dash/objects/page.py
+-rw-r--r--   0        0        0      768 2023-04-12 05:50:21.336964 zen_dash-0.5.4/zen_dash/objects/scripts.py
+-rw-r--r--   0        0        0      720 2023-04-12 05:50:21.336964 zen_dash-0.5.4/zen_dash/objects/sidebar.py
+-rw-r--r--   0        0        0      919 2023-04-12 05:50:21.336964 zen_dash-0.5.4/zen_dash/page.py
+-rw-r--r--   0        0        0        0 2023-04-12 05:50:21.336964 zen_dash-0.5.4/zen_dash/route.py
+-rw-r--r--   0        0        0      191 2023-04-12 05:50:21.336964 zen_dash-0.5.4/zen_dash/scripts.py
+-rw-r--r--   0        0        0      195 2023-04-12 05:50:21.336964 zen_dash-0.5.4/zen_dash/sidebar.py
+-rw-r--r--   0        0        0  1017713 2023-04-12 05:52:55.071166 zen_dash-0.5.4/zen_dash/static/275.07215382ec6b3916.js
+-rw-r--r--   0        0        0    57081 2023-04-12 05:52:55.071166 zen_dash-0.5.4/zen_dash/static/3rdpartylicenses.txt
+-rw-r--r--   0        0        0   128180 2023-04-12 05:52:55.071166 zen_dash-0.5.4/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf
+-rw-r--r--   0        0        0   143258 2023-04-12 05:52:55.071166 zen_dash-0.5.4/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot
+-rw-r--r--   0        0        0    44300 2023-04-12 05:52:55.071166 zen_dash-0.5.4/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2
+-rw-r--r--   0        0        0    57620 2023-04-12 05:52:55.071166 zen_dash-0.5.4/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff
+-rw-r--r--   0        0        0      948 2023-04-12 05:52:55.071166 zen_dash-0.5.4/zen_dash/static/favicon.ico
+-rw-r--r--   0        0        0     2073 2023-04-12 05:52:56.027180 zen_dash-0.5.4/zen_dash/static/index.html
+-rw-r--r--   0        0        0  3105118 2023-04-12 05:52:55.071166 zen_dash-0.5.4/zen_dash/static/main.03cfb17449f365e9.js
+-rw-r--r--   0        0        0    33759 2023-04-12 05:52:55.071166 zen_dash-0.5.4/zen_dash/static/polyfills.0a8881ff36766b1e.js
+-rw-r--r--   0        0        0     3285 2023-04-12 05:52:55.071166 zen_dash-0.5.4/zen_dash/static/runtime.5615a939e3c41241.js
+-rw-r--r--   0        0        0   152653 2023-04-12 05:52:55.071166 zen_dash-0.5.4/zen_dash/static/styles.362a8260c32d36d9.css
+-rw-r--r--   0        0        0      621 2022-10-23 00:15:15.909625 zen_dash-0.5.4/zen_dash/support/__init__.py
+-rw-r--r--   0        0        0      217 2023-04-12 05:50:21.352964 zen_dash-0.5.4/zen_dash/support/encoder.py
+-rw-r--r--   0        0        0     6971 2023-04-10 07:23:01.329101 zen_dash-0.5.4/zen_dash/tag/__init__.py
+-rw-r--r--   0        0        0     1513 2023-04-12 05:50:21.352964 zen_dash-0.5.4/zen_dash/websocket/__init__.py
+-rw-r--r--   0        0        0     8861 2023-04-14 03:43:21.384414 zen_dash-0.5.4/setup.py
+-rw-r--r--   0        0        0     8606 2023-04-14 03:43:21.384727 zen_dash-0.5.4/PKG-INFO
```

### Comparing `zen_dash-0.5.3/LICENSE` & `zen_dash-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/README.md` & `zen_dash-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/pyproject.toml` & `zen_dash-0.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zen_dash"
-version = "0.5.3"
+version = "0.5.4"
 license = "MIT"
 description = "Simple yet scable and production ready python dashboard that is better than shiny application for business."
 readme = "README.md"
 authors = ["Zen <zenreportz@pm.me>"]
 homepage = "https://zen-reportz.github.io/zen_dash/index.html"
 repository = "https://github.com/Zen-Reportz/zen_dash"
 include = [
@@ -35,8 +35,8 @@
 Sphinx = "^5.0.2"
 
 [build-system]
 requires = ["poetry-core @ git+https://github.com/python-poetry/poetry-core.git@master"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-create_project = 'zen_dash.cli.main:create_project'
+create_zen = 'zen_dash.cli.main:create_zen'
```

### Comparing `zen_dash-0.5.3/zen_dash/objects/__init__.py` & `zen_dash-0.5.4/zen_dash/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/objects/instances.py` & `zen_dash-0.5.4/zen_dash/objects/instances.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/objects/scripts.py` & `zen_dash-0.5.4/zen_dash/objects/scripts.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/objects/sidebar.py` & `zen_dash-0.5.4/zen_dash/objects/sidebar.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/page.py` & `zen_dash-0.5.4/zen_dash/page.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/static/275.07215382ec6b3916.js` & `zen_dash-0.5.4/zen_dash/static/275.07215382ec6b3916.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/static/3rdpartylicenses.txt` & `zen_dash-0.5.4/zen_dash/static/3rdpartylicenses.txt`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf` & `zen_dash-0.5.4/zen_dash/static/MaterialIcons-Regular.196fa4a92dd6fa73.ttf`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot` & `zen_dash-0.5.4/zen_dash/static/MaterialIcons-Regular.1e50f5c2ffa6aba4.eot`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2` & `zen_dash-0.5.4/zen_dash/static/MaterialIcons-Regular.7ea2023eeca07427.woff2`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff` & `zen_dash-0.5.4/zen_dash/static/MaterialIcons-Regular.db852539204b1a34.woff`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/static/favicon.ico` & `zen_dash-0.5.4/zen_dash/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/static/index.html` & `zen_dash-0.5.4/zen_dash/static/index.html`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/static/main.03cfb17449f365e9.js` & `zen_dash-0.5.4/zen_dash/static/main.03cfb17449f365e9.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/static/polyfills.0a8881ff36766b1e.js` & `zen_dash-0.5.4/zen_dash/static/polyfills.0a8881ff36766b1e.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/static/runtime.5615a939e3c41241.js` & `zen_dash-0.5.4/zen_dash/static/runtime.5615a939e3c41241.js`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/static/styles.362a8260c32d36d9.css` & `zen_dash-0.5.4/zen_dash/static/styles.362a8260c32d36d9.css`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/support/__init__.py` & `zen_dash-0.5.4/zen_dash/support/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/tag/__init__.py` & `zen_dash-0.5.4/zen_dash/tag/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/zen_dash/websocket/__init__.py` & `zen_dash-0.5.4/zen_dash/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `zen_dash-0.5.3/setup.py` & `zen_dash-0.5.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
  'fastapi>=0.92.0,<0.93.0',
  'python-multipart>=0.0.5,<0.0.6',
  'sphinx-rtd-theme>=1.0.0,<2.0.0',
  'websocket>=0.2.1,<0.3.0',
  'websockets>=10.4,<11.0']
 
 entry_points = \
-{'console_scripts': ['create_project = zen_dash.cli.main:create_project']}
+{'console_scripts': ['create_zen = zen_dash.cli.main:create_zen']}
 
 setup_kwargs = {
     'name': 'zen-dash',
-    'version': '0.5.3',
+    'version': '0.5.4',
     'description': 'Simple yet scable and production ready python dashboard that is better than shiny application for business.',
     'long_description': "# What is Zen Dash?\nZen Dash, a python package, simplifies the building analytics/BI dashboard process while providing enterprise-level scalability, stability, and performance. You can use FastAPI and Flask to host the application. \n\n\n[![Downloads](https://static.pepy.tech/badge/zen-dash)](https://pepy.tech/project/zen-dash)\n[![python](https://img.shields.io/pypi/pyversions/zen-dash.svg?color=green)](https://img.shields.io/pypi/pyversions/zen-dash.svg?color=green)\n[![license](https://img.shields.io/github/license/Zen-Reportz/zen_dash?color=green)](https://img.shields.io/github/license/Zen-Reportz/zen_dash?color=green)\n[![version](https://img.shields.io/pypi/v/zen-dash?color=green&label=pypi%20package)](https://img.shields.io/pypi/v/zen-dash?color=green&label=pypi%20package)\n\n# How to run demo\nLearn more about how to run demo here: [Link](https://github.com/Zen-Reportz/zen_dash/wiki/How-can-I-run-demo-%3F)\n\n# How to Contribute\nPlease visit this page to learn how to contribute: [Link](https://github.com/Zen-Reportz/zen_dash/blob/main/how_to_contribute.md)\n\n# Why did I build Zen Dash?\n\nThere are many dashboarding solutions, like shiny (R, python), Streamlit, and others. I have used all of these solutions. I enjoy building solutions. However, all of these tools and libraries lack one vital point. They are not enterprise-ready solutions. They are fragile and not scalable solutions. So, whenever I built analytics/ BI Dashboards, Even after many bandages, dashboards were delicate and unstable. \n\nBefore explaining the problem and its reasons, I like to describe the issues we are trying to solve. \n\n* Some of our dashboards need to be used by more than 200 people simultaneously and require a sub-second response to be practical. They will use more than 8 hours straight for work. The dashboard should not crash during usage.\n\n* more than a hundred field team members are using our other dashboard, which is spread across multiple countries. Their internet speed is not ideal like office, so the analytics dashboard needs to be anti-fragile. They should be able to share their data with our customers on the ground without worrying about the dashboard crashing or refreshing data. \n\n* the Third group of the dashboard is far more complex and sensitive since we integrated it into one of our company production environments. This dashboard needs to better code isolation for testing, so they deployed it, so we can be sure it is not breaking the company production environment. \n\nSo, I invested time in the zen-dash, which addresses these problems. Before jumping into the zen-dash, I want to show you what we have done to make anti-fragile systems using other analytics solutions. I will also explain why it is failing. You might want to try a zen dash to elevate pains in these stages. \n\n\n* Building plumber or fastapi/flask to offload computation. \nGood thing: application becomes somewhat better at responding\nBad thing: now, code is in multiple locations, which makes it difficult to onboard and debug. If we use shiny with python, it is difficult for some team members to understand what they are doing.\n\n* Rather than dashboards, we started to provide more reports. However, this, in turn, created more work to report on building and maintenance.\n\n* Building simpler dashboards with limited functionality or exploration. We also get pushed back on this type of dashboard because people want to know more than what limited functionality dashboard what returns\n\n* Using Tableau to deliver data to field or high requirements teams. Tableau is not a perfect solution, either. It limits what analytics tools we can use.\n\n\nIf you see these signs in your analytics dashboarding solutions, you face a similar and painful situation.\n\n\n# Why are other tools creating such issues?\n\nLet me explain in technical detail. Here I am focusing on specifically Shiny and Streamlit because both face similar situations. After all, they are using the same architecture and software design. In a single word, it is due to incompatible architecture and software design. \n\nThey are facing two main issues.\n\n* Websocket\n* Lack of separation between UI and backend (specifically with shiny).\n\n\nWebsocket is one great tool where you can connect the front and back end once and send as much data as you want between them. \n\nThe chat system uses Websocket. Websocket simplifies your communication architecture when you use WebSocket over the rest API. It is an effective tool for communicating real-time data with lower overhead. Websocket keeps the connection open to the backend server so that new data transfers don't require creating a new link and overhead related to it. \n\nHowever, this constant connection makes a delicate system. It can break for any reason. So, when shiny apps WebSocket crashes, it grays out the screen, and you must start again from scratch. You will lose all filter selections you have made. I believe this is done to reduce overhead to the complexity of code on the shiny side. Because of it, it is not an enterprise-grade solution. Due to these design selections, we are facing problems 1 and 2.\n\nAnother issue with the WebSocket will create an artificial choke point at the backend level since R is a single thread with poor async support. In R, code usually runs sequentially. You have to use the API pool to redistribute the load on other machines. However, R is choking data push even when an API pool is used. So if we offload work on other services using the rest API pool, it has to wait until all processes are finished. Even if threading support is in python, we are not thinking about additional processing we need where threading is not a good option. The best option is to do multiprocessing. To do that, you need a different type of software design. I have seen situations regularly where shiny renders time well over 1 min when you have too many things to render on the page. These limitations are attributing problems 2 and 3\n\nIf WebSocket is used, you select only one machine/service to respond. So single service needs to process all requests and respond to them. Because of it, we had to create situation one to address this. These design is attributing problem 1\n\nThe second biggest issue with shiny is not separating UI from the backend. This design is excellent for rapid development, but if misused, it can slow down your application. It creates problems precisely when you want to render a large data example table. Shiny, rather than sending data for the table, the backend converts to HTML code and pushes HTML code as a string through WebSocket. This process becomes cumbersome very quickly because sending just data will be light, but sending HTML as a string adds quite a bit of load. In addition, you have to use eval or similar code to evaluate the code base, which adds security venerability and other overhead processes. It also slowdowns applications.\n\n\n# How much does zen dash make a difference?\nA dashboard that regularly took more than 60 seconds to load response data within ten or fewer seconds. \n\nOur dashboard has become more stable. If the internet connection is slow or fast, it doesn't impact the entire application.\n\nThe dashboard can run for days at a time without stability issues.\n\nHow do we achieve it? After understanding the limitation of the WebSocket, I decided to remove the WebSocket for communicating information. Instead, it will send data using a traditional HTTP request. \n\nUI is prebuilt in angular and complies, where you can provide what to render using angular flex and material design. \n\n# Docs\nhttps://zen-reportz.github.io/zen_dash/index.html\n",
     'author': 'Zen',
     'author_email': 'zenreportz@pm.me',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://zen-reportz.github.io/zen_dash/index.html',
```

### Comparing `zen_dash-0.5.3/PKG-INFO` & `zen_dash-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zen-dash
-Version: 0.5.3
+Version: 0.5.4
 Summary: Simple yet scable and production ready python dashboard that is better than shiny application for business.
 Home-page: https://zen-reportz.github.io/zen_dash/index.html
 License: MIT
 Author: Zen
 Author-email: zenreportz@pm.me
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

