# Comparing `tmp/orion_nais-0.1.0.tar.gz` & `tmp/orion_nais-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orion_nais-0.1.0.tar", max compression
+gzip compressed data, was "orion_nais-0.1.1.tar", max compression
```

## Comparing `orion_nais-0.1.0.tar` & `orion_nais-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-02-10 13:07:27.340638 orion_nais-0.1.0/LICENSE
--rw-r--r--   0        0        0     5661 2023-02-10 12:35:25.307477 orion_nais-0.1.0/README.md
--rw-r--r--   0        0        0       39 2023-01-26 14:12:33.833384 orion_nais-0.1.0/orion/__init__.py
--rw-r--r--   0        0        0    15699 2023-02-10 12:10:19.249738 orion_nais-0.1.0/orion/client.py
--rw-r--r--   0        0        0    17303 2023-02-10 12:06:31.153714 orion_nais-0.1.0/orion/mmsi.py
--rw-r--r--   0        0        0        0 2023-02-03 22:04:07.481203 orion_nais-0.1.0/orion/types/__init__.py
--rw-r--r--   0        0        0      296 2023-02-03 09:47:58.249080 orion_nais-0.1.0/orion/types/ais.py
--rw-r--r--   0        0        0      136 2023-01-27 13:52:51.653087 orion_nais-0.1.0/orion/urls.py
--rw-r--r--   0        0        0        0 2023-02-04 00:21:05.300372 orion_nais-0.1.0/orion/utils/__init__.py
--rw-r--r--   0        0        0     1100 2023-02-10 10:06:30.752969 orion_nais-0.1.0/orion/utils/get_data.py
--rw-r--r--   0        0        0    16329 2023-02-10 12:07:42.453458 orion_nais-0.1.0/orion/vessel_codes.py
--rw-r--r--   0        0        0     1378 2023-02-10 14:19:47.073577 orion_nais-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6715 1970-01-01 00:00:00.000000 orion_nais-0.1.0/setup.py
--rw-r--r--   0        0        0     6332 1970-01-01 00:00:00.000000 orion_nais-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-10 13:07:27.340638 orion_nais-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6081 2023-04-14 11:14:29.054669 orion_nais-0.1.1/README.md
+-rw-r--r--   0        0        0       39 2023-01-26 14:12:33.833384 orion_nais-0.1.1/orion/__init__.py
+-rw-r--r--   0        0        0    16061 2023-04-14 10:54:20.572049 orion_nais-0.1.1/orion/client.py
+-rw-r--r--   0        0        0    17303 2023-02-10 12:06:31.153714 orion_nais-0.1.1/orion/mmsi.py
+-rw-r--r--   0        0        0        0 2023-02-03 22:04:07.481203 orion_nais-0.1.1/orion/types/__init__.py
+-rw-r--r--   0        0        0      296 2023-02-03 09:47:58.249080 orion_nais-0.1.1/orion/types/ais.py
+-rw-r--r--   0        0        0      136 2023-01-27 13:52:51.653087 orion_nais-0.1.1/orion/urls.py
+-rw-r--r--   0        0        0        0 2023-02-04 00:21:05.300372 orion_nais-0.1.1/orion/utils/__init__.py
+-rw-r--r--   0        0        0     1100 2023-02-10 10:06:30.752969 orion_nais-0.1.1/orion/utils/get_data.py
+-rw-r--r--   0        0        0    16329 2023-02-10 12:07:42.453458 orion_nais-0.1.1/orion/vessel_codes.py
+-rw-r--r--   0        0        0     1378 2023-04-14 11:15:41.046256 orion_nais-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7146 1970-01-01 00:00:00.000000 orion_nais-0.1.1/setup.py
+-rw-r--r--   0        0        0     6752 1970-01-01 00:00:00.000000 orion_nais-0.1.1/PKG-INFO
```

### Comparing `orion_nais-0.1.0/LICENSE` & `orion_nais-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `orion_nais-0.1.0/README.md` & `orion_nais-0.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -85,14 +85,25 @@
 
 ### Makefile commands
 
 - `make lint`
   - lint the code in the src folder with black, isort and flake8. Mypy will check for correct typing.
 - `make format`
   - format the code in the src folder with black and isort.
+- `make test`
+  - run the tests in the tests folder.
+- `make bump-patch`
+  - bump the patch version of the package. Example: 0.1.0 -> 0.1.1
+- `make bump-minor`
+  - bump the minor version of the package. Example: 0.1.0 -> 0.2.0
+- `make bump-major`
+  - bump the major version of the package. Example: 0.1.0 -> 1.0.0 
+- `make release`
+  - publish the package to pypi. You need to have an account and be logged in to pypi.
+
 
 ### Structure
 
 ```
 .
 ├── .bumpversion.cfg
 ├── .editorconfig
```

#### html2text {}

```diff
@@ -24,20 +24,25 @@
 functions for you to use. Enjoy. ## Local development ### Requirements --- -
 pyenv - manage python versions - poetry - manage python dependencies To install
 on mac you can use homebrew: ```bash brew upgrade brew install pyenv ``` You
 can either install poetry with homebrew or the way described in the
 [documentation](https://python-poetry.org/docs/#installation) ### Makefile
 commands - `make lint` - lint the code in the src folder with black, isort and
 flake8. Mypy will check for correct typing. - `make format` - format the code
-in the src folder with black and isort. ### Structure ``` . âââ
-.bumpversion.cfg âââ .editorconfig âââ .flake8 âââ .gitignore
-âââ Makefile âââ README.md âââ orion â âââ client.py
-â âââ mmsi.py â âââ types â â âââ ais.py â
-âââ urls.py â âââ utils â â âââ get_data.py â
-âââ vessel_codes.py âââ poetry.lock âââ pyproject.toml
+in the src folder with black and isort. - `make test` - run the tests in the
+tests folder. - `make bump-patch` - bump the patch version of the package.
+Example: 0.1.0 -> 0.1.1 - `make bump-minor` - bump the minor version of the
+package. Example: 0.1.0 -> 0.2.0 - `make bump-major` - bump the major version
+of the package. Example: 0.1.0 -> 1.0.0 - `make release` - publish the package
+to pypi. You need to have an account and be logged in to pypi. ### Structure
+``` . âââ .bumpversion.cfg âââ .editorconfig âââ .flake8
+âââ .gitignore âââ Makefile âââ README.md âââ orion â
+âââ client.py â âââ mmsi.py â âââ types â â âââ
+ais.py â âââ urls.py â âââ utils â â âââ get_data.py
+â âââ vessel_codes.py âââ poetry.lock âââ pyproject.toml
 âââ tests âââ make_mock_data.py âââ mocks âââ
 test_orion.py ``` - `.bumpversion.cfg` - Configuration file for bumpversion. -
 `.editorconfig` - Configuration file for editorconfig. - `.flake8` -
 Configuration file for flake8. - `.gitignore` - Configuration file for git. -
 `pyproject.toml` - Configuration file for poetry. Mypy and isort is configured
 here. - `poetry.lock` - Lock file for poetry. - `Makefile` - Makefile for the
 project. Here you can find commands for linting and formatting. - `README.md` -
```

### Comparing `orion_nais-0.1.0/orion/client.py` & `orion_nais-0.1.1/orion/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 """
 import json
 import logging
 import math
 import os
+import urllib.parse
 from datetime import datetime, timedelta
 from typing import Dict, List, Optional, Union
 
 import dotenv
 import geopandas
 import pandas as pd
 import pytz
@@ -64,22 +65,29 @@
             client_secret (str): secret for your user at Barentswatch.
             skip_auth (Optional[bool]): skip authentication. Useful for testing.
         """
         if not skip_auth:
             self.client_id = client_id or CLIENT_ID
             self.client_secret = client_secret or CLIENT_SECRET
 
-            if (not CLIENT_ID) | (not CLIENT_SECRET):  # pragma: no cover
+            if (not self.client_id) | (
+                not self.client_secret
+            ):  # pragma: no cover # noqa
                 raise ValueError(
                     """
-                    Please set CLIENT_ID and CLIENT_SECRET in .env file
+                    Please either set CLIENT_ID and CLIENT_SECRET in .env file
                     or provide them when creating an instance of the class
                     """
                 )
 
+            if type(self.client_id) == str:  # pragma: no cover
+                self.client_id = urllib.parse.quote_plus(self.client_id)
+            if type(self.client_secret) == str:  # pragma: no cover
+                self.client_secret = urllib.parse.quote_plus(self.client_secret)
+
             self.authenticate_session = requests.Session()  # Session for tokens
             self.authenticate()
             self.access = ""
 
             self.session = requests.Session()
             self.session.auth = self.auth  # type: ignore
             self.session.hooks["response"].append(self.reauth)
@@ -378,15 +386,15 @@
 
         _gdf = _gdf.sort_values(by="msgtime")
 
         return _gdf
 
     def explore(  # type: ignore[no-any-unimported]
         self, _gdf: geopandas.GeoDataFrame
-    ) -> str: # pragma: no cover
+    ) -> str:  # pragma: no cover
         """helper function to geopandas explore
 
         Args:
             _gdf (GeoDataFrame): the geodataframe to explore
 
         Returns:
             html: an interactive map of our data
```

### Comparing `orion_nais-0.1.0/orion/mmsi.py` & `orion_nais-0.1.1/orion/mmsi.py`

 * *Files identical despite different names*

### Comparing `orion_nais-0.1.0/orion/utils/get_data.py` & `orion_nais-0.1.1/orion/utils/get_data.py`

 * *Files identical despite different names*

### Comparing `orion_nais-0.1.0/orion/vessel_codes.py` & `orion_nais-0.1.1/orion/vessel_codes.py`

 * *Files identical despite different names*

### Comparing `orion_nais-0.1.0/pyproject.toml` & `orion_nais-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "orion-nais"
-version = "0.1.0"
+version = "0.1.1"
 description = "A client for the NAIS API from FThe Norwegian Coastal Administration"
 authors = ["Lasse Lambrechts <lasse.lambrechts@bt.no>"]
 readme = "README.md"
 packages = [{include = "orion"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `orion_nais-0.1.0/setup.py` & `orion_nais-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
  'python-dotenv>=0.21.0,<0.22.0',
  'pytz>=2022.7.1,<2023.0.0',
  'requests>=2.28.0,<3.0.0',
  'shapely>=2.0.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'orion-nais',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'A client for the NAIS API from FThe Norwegian Coastal Administration',
-    'long_description': '# Orion-NAIS\n\n\n<!-- TABLE OF CONTENTS -->\n<details open="open">\n  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>\n  <ol>\n    <li>\n      <a href="#about-the-project">About The Project</a>\n      <ul>\n        <li><a href="#requirements">Requirements</a></li>\n        <li><a href="#structure">Structure</a></li>\n      </ul>\n    </li>\n    <li>\n      <a href="#getting-started">Getting Started</a>\n      <ul>\n        <li><a href="#prerequisites">Prerequisites</a></li>\n        <li><a href="#installation">Installation</a></li>\n      </ul>\n    </li>\n    <li><a href="#usage">Usage</a></li>\n    <li><a href="#contributing">Contributing</a></li>\n    <li><a href="#contact">Contact</a></li>\n  </ol>\n</details>\n\n<!-- ABOUT THE PROJECT -->\n\n## About The Project\n\nOrion-NAIS is a client to work with the NAIS API. It helps with authentication and provides a simple interface to work with the API.\n\nWhen working with the API you need to have a valid token. The token is valid for a set period of time. The client will automatically refresh the token when it expires.\n\n### Why the name Orion?\n\nThe NAIS Api is provided through BarentsWatch. BarentsWatch is a Norwegian information portal that provides overview of activity and knowledge in coastal and sea areas. The Norwegian movie "Orion\'s Belt" from 1985 is an action movie set in the Barents region. About three men, a bulldozer, a Russian helicopter and a ship. Thus the name Orion.\n\n## Installation\n\nRequires Python 3.10 or later.\n\n```bash\n\npip install orion-nais\n\n```\n\nor using pipenv:\n\n```bash\n\npipenv install orion-nais\n\n```\n\nor using poetry:\n\n```bash\npoetry add orion-nais\n```\n\n## Usage\n\nThere are a heap of functions for you to use. Enjoy.\n\n## Local development\n\n### Requirements\n---\n\n- pyenv - manage python versions\n- poetry - manage python dependencies\n\nTo install on mac you can use homebrew:\n\n```bash\nbrew upgrade\nbrew install pyenv\n```\n\nYou can either install poetry with homebrew or the way described in the [documentation](https://python-poetry.org/docs/#installation)\n\n\n### Makefile commands\n\n- `make lint`\n  - lint the code in the src folder with black, isort and flake8. Mypy will check for correct typing.\n- `make format`\n  - format the code in the src folder with black and isort.\n\n### Structure\n\n```\n.\n├── .bumpversion.cfg\n├── .editorconfig\n├── .flake8\n├── .gitignore\n├── Makefile\n├── README.md\n├── orion\n│   ├── client.py\n│   ├── mmsi.py\n│   ├── types\n│   │   └── ais.py\n│   ├── urls.py\n│   ├── utils\n│   │   └── get_data.py\n│   └── vessel_codes.py\n├── poetry.lock\n├── pyproject.toml\n└── tests\n    ├── make_mock_data.py\n    ├── mocks\n    └── test_orion.py\n    \n```\n\n- `.bumpversion.cfg`\n  - Configuration file for bumpversion.\n- `.editorconfig`\n  - Configuration file for editorconfig.\n- `.flake8`\n  - Configuration file for flake8.\n- `.gitignore`\n  - Configuration file for git.\n- `pyproject.toml`\n  - Configuration file for poetry. Mypy and isort is configured here.\n- `poetry.lock`\n  - Lock file for poetry.\n- `Makefile`\n  - Makefile for the project. Here you can find commands for linting and formatting.\n- `README.md`\n  - This file.\n- `orion`\n  - The source code for the package.\n  - `client.py`\n    - The client class.\n  - `mmsi.py`\n    - A dataclass for handling MMSI numbers and MID-codes (jurisdiction).\n  - `types`\n    - A folder for types.\n    - `ais.py`\n      - A class for handling AIS messages.\n  - `urls.py`\n    - A file with urls for the API.\n  - `utils`\n    - A folder for utility functions.\n    - `get_data.py`\n      - A function for getting data from other sources. Not used by the Orion client. Contains code for getting data from the Norwegian Petroleum Directorate.\n  - `vessel_codes.py`\n    - A dataclass for looking up vessel codes.\n- `tests`\n  - Tests for the package.\n\n## Usage\n\nTo install the package in your project run\n\n```bash\n\npoetry add orion-nais\n```\n\n## Contributing\n\nDo you have write permissions to the repo? Then you can clone this project to a folder on your computer.\n\n```bash\ngit clone https://github.com/BergensTidende/orion-nais.git\n```\n\nIf not do the following:\n\n- Create a personal fork of the project on Github.\n- Clone the fork on your local machine. Your remote repo on Github is called `origin`.\n- Add the original repository as a remote called `upstream`.\n- If you created your fork a while ago be sure to pull upstream changes into your local repository.\n\nThis will clone the repo into `pakkenellik`. \n\nCreate a branch for your changes\n\n```bash\ngit checkout -b name-of-branch\n```\n\nMake your changes, rememeber to commit. And always write your commit messages in the present tense. Your commit message should describe what the commit, when applied, does to the code – not what you did to the code.\n\nIf you\'re working on a clone push the branch to github and make PR.\n\nIf your\'re working a fork:\n\n- Squash your commits into a single commit with git\'s [interactive rebase](https://help.github.com/articles/interactive-rebase). Create a new branch if necessary.\n- Push your branch to your fork on Github, the remote `origin`.\n- From your fork open a pull request in the correct branch. Target the project\'s `develop` branch if there is one, else go for `master`!\n- …\n- If the maintainer requests further changes just push them to your branch. The PR will be updated automatically.\n- Once the pull request is approved and merged you can pull the changes from `upstream` to your local repo and delete\n  your extra branch(es).\n\n <!-- CONTACT -->\n\n## Contact\n\nBord4 - bord4@bt.no\n',
+    'long_description': '# Orion-NAIS\n\n\n<!-- TABLE OF CONTENTS -->\n<details open="open">\n  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>\n  <ol>\n    <li>\n      <a href="#about-the-project">About The Project</a>\n      <ul>\n        <li><a href="#requirements">Requirements</a></li>\n        <li><a href="#structure">Structure</a></li>\n      </ul>\n    </li>\n    <li>\n      <a href="#getting-started">Getting Started</a>\n      <ul>\n        <li><a href="#prerequisites">Prerequisites</a></li>\n        <li><a href="#installation">Installation</a></li>\n      </ul>\n    </li>\n    <li><a href="#usage">Usage</a></li>\n    <li><a href="#contributing">Contributing</a></li>\n    <li><a href="#contact">Contact</a></li>\n  </ol>\n</details>\n\n<!-- ABOUT THE PROJECT -->\n\n## About The Project\n\nOrion-NAIS is a client to work with the NAIS API. It helps with authentication and provides a simple interface to work with the API.\n\nWhen working with the API you need to have a valid token. The token is valid for a set period of time. The client will automatically refresh the token when it expires.\n\n### Why the name Orion?\n\nThe NAIS Api is provided through BarentsWatch. BarentsWatch is a Norwegian information portal that provides overview of activity and knowledge in coastal and sea areas. The Norwegian movie "Orion\'s Belt" from 1985 is an action movie set in the Barents region. About three men, a bulldozer, a Russian helicopter and a ship. Thus the name Orion.\n\n## Installation\n\nRequires Python 3.10 or later.\n\n```bash\n\npip install orion-nais\n\n```\n\nor using pipenv:\n\n```bash\n\npipenv install orion-nais\n\n```\n\nor using poetry:\n\n```bash\npoetry add orion-nais\n```\n\n## Usage\n\nThere are a heap of functions for you to use. Enjoy.\n\n## Local development\n\n### Requirements\n---\n\n- pyenv - manage python versions\n- poetry - manage python dependencies\n\nTo install on mac you can use homebrew:\n\n```bash\nbrew upgrade\nbrew install pyenv\n```\n\nYou can either install poetry with homebrew or the way described in the [documentation](https://python-poetry.org/docs/#installation)\n\n\n### Makefile commands\n\n- `make lint`\n  - lint the code in the src folder with black, isort and flake8. Mypy will check for correct typing.\n- `make format`\n  - format the code in the src folder with black and isort.\n- `make test`\n  - run the tests in the tests folder.\n- `make bump-patch`\n  - bump the patch version of the package. Example: 0.1.0 -> 0.1.1\n- `make bump-minor`\n  - bump the minor version of the package. Example: 0.1.0 -> 0.2.0\n- `make bump-major`\n  - bump the major version of the package. Example: 0.1.0 -> 1.0.0 \n- `make release`\n  - publish the package to pypi. You need to have an account and be logged in to pypi.\n\n\n### Structure\n\n```\n.\n├── .bumpversion.cfg\n├── .editorconfig\n├── .flake8\n├── .gitignore\n├── Makefile\n├── README.md\n├── orion\n│   ├── client.py\n│   ├── mmsi.py\n│   ├── types\n│   │   └── ais.py\n│   ├── urls.py\n│   ├── utils\n│   │   └── get_data.py\n│   └── vessel_codes.py\n├── poetry.lock\n├── pyproject.toml\n└── tests\n    ├── make_mock_data.py\n    ├── mocks\n    └── test_orion.py\n    \n```\n\n- `.bumpversion.cfg`\n  - Configuration file for bumpversion.\n- `.editorconfig`\n  - Configuration file for editorconfig.\n- `.flake8`\n  - Configuration file for flake8.\n- `.gitignore`\n  - Configuration file for git.\n- `pyproject.toml`\n  - Configuration file for poetry. Mypy and isort is configured here.\n- `poetry.lock`\n  - Lock file for poetry.\n- `Makefile`\n  - Makefile for the project. Here you can find commands for linting and formatting.\n- `README.md`\n  - This file.\n- `orion`\n  - The source code for the package.\n  - `client.py`\n    - The client class.\n  - `mmsi.py`\n    - A dataclass for handling MMSI numbers and MID-codes (jurisdiction).\n  - `types`\n    - A folder for types.\n    - `ais.py`\n      - A class for handling AIS messages.\n  - `urls.py`\n    - A file with urls for the API.\n  - `utils`\n    - A folder for utility functions.\n    - `get_data.py`\n      - A function for getting data from other sources. Not used by the Orion client. Contains code for getting data from the Norwegian Petroleum Directorate.\n  - `vessel_codes.py`\n    - A dataclass for looking up vessel codes.\n- `tests`\n  - Tests for the package.\n\n## Usage\n\nTo install the package in your project run\n\n```bash\n\npoetry add orion-nais\n```\n\n## Contributing\n\nDo you have write permissions to the repo? Then you can clone this project to a folder on your computer.\n\n```bash\ngit clone https://github.com/BergensTidende/orion-nais.git\n```\n\nIf not do the following:\n\n- Create a personal fork of the project on Github.\n- Clone the fork on your local machine. Your remote repo on Github is called `origin`.\n- Add the original repository as a remote called `upstream`.\n- If you created your fork a while ago be sure to pull upstream changes into your local repository.\n\nThis will clone the repo into `pakkenellik`. \n\nCreate a branch for your changes\n\n```bash\ngit checkout -b name-of-branch\n```\n\nMake your changes, rememeber to commit. And always write your commit messages in the present tense. Your commit message should describe what the commit, when applied, does to the code – not what you did to the code.\n\nIf you\'re working on a clone push the branch to github and make PR.\n\nIf your\'re working a fork:\n\n- Squash your commits into a single commit with git\'s [interactive rebase](https://help.github.com/articles/interactive-rebase). Create a new branch if necessary.\n- Push your branch to your fork on Github, the remote `origin`.\n- From your fork open a pull request in the correct branch. Target the project\'s `develop` branch if there is one, else go for `master`!\n- …\n- If the maintainer requests further changes just push them to your branch. The PR will be updated automatically.\n- Once the pull request is approved and merged you can pull the changes from `upstream` to your local repo and delete\n  your extra branch(es).\n\n <!-- CONTACT -->\n\n## Contact\n\nBord4 - bord4@bt.no\n',
     'author': 'Lasse Lambrechts',
     'author_email': 'lasse.lambrechts@bt.no',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['orion',
 'orion.types', 'orion.utils'] package_data = \ {'': ['*']} install_requires = \
 ['geopandas>=0.12.2,<0.13.0', 'pandas>=1.5.2,<2.0.0', 'python-
 dotenv>=0.21.0,<0.22.0', 'pytz>=2022.7.1,<2023.0.0', 'requests>=2.28.0,<3.0.0',
 'shapely>=2.0.0,<3.0.0'] setup_kwargs = { 'name': 'orion-nais', 'version':
-'0.1.0', 'description': 'A client for the NAIS API from FThe Norwegian Coastal
+'0.1.1', 'description': 'A client for the NAIS API from FThe Norwegian Coastal
 Administration', 'long_description': '# Orion-NAIS\n\n\n\n\n
 ***** Table of Contents *****
 \n
    1. \n
    2. \n About_The_Project\n
           o \n
           o Requirements
@@ -47,15 +47,21 @@
 --\n\n- pyenv - manage python versions\n- poetry - manage python
 dependencies\n\nTo install on mac you can use homebrew:\n\n```bash\nbrew
 upgrade\nbrew install pyenv\n```\n\nYou can either install poetry with homebrew
 or the way described in the [documentation](https://python-poetry.org/docs/
 #installation)\n\n\n### Makefile commands\n\n- `make lint`\n - lint the code in
 the src folder with black, isort and flake8. Mypy will check for correct
 typing.\n- `make format`\n - format the code in the src folder with black and
-isort.\n\n### Structure\n\n```\n.\nâââ .bumpversion.cfg\nâââ
+isort.\n- `make test`\n - run the tests in the tests folder.\n- `make bump-
+patch`\n - bump the patch version of the package. Example: 0.1.0 -> 0.1.1\n-
+`make bump-minor`\n - bump the minor version of the package. Example: 0.1.0 -
+> 0.2.0\n- `make bump-major`\n - bump the major version of the package.
+Example: 0.1.0 -> 1.0.0 \n- `make release`\n - publish the package to pypi. You
+need to have an account and be logged in to pypi.\n\n\n###
+Structure\n\n```\n.\nâââ .bumpversion.cfg\nâââ
 .editorconfig\nâââ .flake8\nâââ .gitignore\nâââ
 Makefile\nâââ README.md\nâââ orion\nâ âââ client.py\nâ
 âââ mmsi.py\nâ âââ types\nâ â âââ ais.py\nâ âââ
 urls.py\nâ âââ utils\nâ â âââ get_data.py\nâ âââ
 vessel_codes.py\nâââ poetry.lock\nâââ pyproject.toml\nâââ
 tests\n âââ make_mock_data.py\n âââ mocks\n âââ
 test_orion.py\n \n```\n\n- `.bumpversion.cfg`\n - Configuration file for
```

### Comparing `orion_nais-0.1.0/PKG-INFO` & `orion_nais-0.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orion-nais
-Version: 0.1.0
+Version: 0.1.1
 Summary: A client for the NAIS API from FThe Norwegian Coastal Administration
 Author: Lasse Lambrechts
 Author-email: lasse.lambrechts@bt.no
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -103,14 +103,25 @@
 
 ### Makefile commands
 
 - `make lint`
   - lint the code in the src folder with black, isort and flake8. Mypy will check for correct typing.
 - `make format`
   - format the code in the src folder with black and isort.
+- `make test`
+  - run the tests in the tests folder.
+- `make bump-patch`
+  - bump the patch version of the package. Example: 0.1.0 -> 0.1.1
+- `make bump-minor`
+  - bump the minor version of the package. Example: 0.1.0 -> 0.2.0
+- `make bump-major`
+  - bump the major version of the package. Example: 0.1.0 -> 1.0.0 
+- `make release`
+  - publish the package to pypi. You need to have an account and be logged in to pypi.
+
 
 ### Structure
 
 ```
 .
 ├── .bumpversion.cfg
 ├── .editorconfig
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: orion-nais Version: 0.1.0 Summary: A client for the
+Metadata-Version: 2.1 Name: orion-nais Version: 0.1.1 Summary: A client for the
 NAIS API from FThe Norwegian Coastal Administration Author: Lasse Lambrechts
 Author-email: lasse.lambrechts@bt.no Requires-Python: >=3.10,<4.0 Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-Dist:
 geopandas (>=0.12.2,<0.13.0) Requires-Dist: pandas (>=1.5.2,<2.0.0) Requires-
 Dist: python-dotenv (>=0.21.0,<0.22.0) Requires-Dist: pytz
 (>=2022.7.1,<2023.0.0) Requires-Dist: requests (>=2.28.0,<3.0.0) Requires-Dist:
@@ -32,20 +32,25 @@
 functions for you to use. Enjoy. ## Local development ### Requirements --- -
 pyenv - manage python versions - poetry - manage python dependencies To install
 on mac you can use homebrew: ```bash brew upgrade brew install pyenv ``` You
 can either install poetry with homebrew or the way described in the
 [documentation](https://python-poetry.org/docs/#installation) ### Makefile
 commands - `make lint` - lint the code in the src folder with black, isort and
 flake8. Mypy will check for correct typing. - `make format` - format the code
-in the src folder with black and isort. ### Structure ``` . âââ
-.bumpversion.cfg âââ .editorconfig âââ .flake8 âââ .gitignore
-âââ Makefile âââ README.md âââ orion â âââ client.py
-â âââ mmsi.py â âââ types â â âââ ais.py â
-âââ urls.py â âââ utils â â âââ get_data.py â
-âââ vessel_codes.py âââ poetry.lock âââ pyproject.toml
+in the src folder with black and isort. - `make test` - run the tests in the
+tests folder. - `make bump-patch` - bump the patch version of the package.
+Example: 0.1.0 -> 0.1.1 - `make bump-minor` - bump the minor version of the
+package. Example: 0.1.0 -> 0.2.0 - `make bump-major` - bump the major version
+of the package. Example: 0.1.0 -> 1.0.0 - `make release` - publish the package
+to pypi. You need to have an account and be logged in to pypi. ### Structure
+``` . âââ .bumpversion.cfg âââ .editorconfig âââ .flake8
+âââ .gitignore âââ Makefile âââ README.md âââ orion â
+âââ client.py â âââ mmsi.py â âââ types â â âââ
+ais.py â âââ urls.py â âââ utils â â âââ get_data.py
+â âââ vessel_codes.py âââ poetry.lock âââ pyproject.toml
 âââ tests âââ make_mock_data.py âââ mocks âââ
 test_orion.py ``` - `.bumpversion.cfg` - Configuration file for bumpversion. -
 `.editorconfig` - Configuration file for editorconfig. - `.flake8` -
 Configuration file for flake8. - `.gitignore` - Configuration file for git. -
 `pyproject.toml` - Configuration file for poetry. Mypy and isort is configured
 here. - `poetry.lock` - Lock file for poetry. - `Makefile` - Makefile for the
 project. Here you can find commands for linting and formatting. - `README.md` -
```

