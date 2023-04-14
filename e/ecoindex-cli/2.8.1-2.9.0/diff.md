# Comparing `tmp/ecoindex-cli-2.8.1.tar.gz` & `tmp/ecoindex-cli-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoindex-cli-2.8.1.tar", max compression
+gzip compressed data, was "ecoindex-cli-2.9.0.tar", max compression
```

## Comparing `ecoindex-cli-2.8.1.tar` & `ecoindex-cli-2.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1069 2022-04-28 12:46:26.809137 ecoindex-cli-2.8.1/LICENSE
--rw-r--r--   0        0        0     8880 2022-04-28 12:46:26.809137 ecoindex-cli-2.8.1/README.md
--rw-r--r--   0        0        0       22 2022-04-28 12:46:26.809137 ecoindex-cli-2.8.1/ecoindex_cli/__init__.py
--rw-r--r--   0        0        0        0 2022-04-28 12:46:26.813137 ecoindex-cli-2.8.1/ecoindex_cli/cli/__init__.py
--rw-r--r--   0        0        0     6896 2022-04-28 12:46:26.813137 ecoindex-cli-2.8.1/ecoindex_cli/cli/app.py
--rw-r--r--   0        0        0     3147 2022-04-28 12:46:26.813137 ecoindex-cli-2.8.1/ecoindex_cli/cli/arguments_handler.py
--rw-r--r--   0        0        0      781 2022-04-28 12:46:26.813137 ecoindex-cli-2.8.1/ecoindex_cli/crawl.py
--rw-r--r--   0        0        0      871 2022-04-28 12:46:26.813137 ecoindex-cli-2.8.1/ecoindex_cli/files.py
--rw-r--r--   0        0        0      470 2022-04-28 12:46:26.813137 ecoindex-cli-2.8.1/ecoindex_cli/logger.py
--rw-r--r--   0        0        0        0 2022-04-28 12:46:26.813137 ecoindex-cli-2.8.1/ecoindex_cli/report/__init__.py
--rw-r--r--   0        0        0     3820 2022-04-28 12:46:26.813137 ecoindex-cli-2.8.1/ecoindex_cli/report/report.py
--rw-r--r--   0        0        0     7978 2022-04-28 12:46:26.813137 ecoindex-cli-2.8.1/ecoindex_cli/report/template.html
--rw-r--r--   0        0        0      888 2022-04-28 12:46:26.813137 ecoindex-cli-2.8.1/pyproject.toml
--rw-r--r--   0        0        0    10204 2022-04-28 12:47:33.416463 ecoindex-cli-2.8.1/setup.py
--rw-r--r--   0        0        0     9840 2022-04-28 12:47:33.417291 ecoindex-cli-2.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2022-05-02 08:56:10.790886 ecoindex-cli-2.9.0/LICENSE
+-rw-r--r--   0        0        0     8880 2022-05-02 08:56:10.790886 ecoindex-cli-2.9.0/README.md
+-rw-r--r--   0        0        0       22 2022-05-02 08:56:10.794887 ecoindex-cli-2.9.0/ecoindex_cli/__init__.py
+-rw-r--r--   0        0        0        0 2022-05-02 08:56:10.794887 ecoindex-cli-2.9.0/ecoindex_cli/cli/__init__.py
+-rw-r--r--   0        0        0     6896 2022-05-02 08:56:10.794887 ecoindex-cli-2.9.0/ecoindex_cli/cli/app.py
+-rw-r--r--   0        0        0     3155 2022-05-02 08:56:10.794887 ecoindex-cli-2.9.0/ecoindex_cli/cli/arguments_handler.py
+-rw-r--r--   0        0        0      781 2022-05-02 08:56:10.794887 ecoindex-cli-2.9.0/ecoindex_cli/crawl.py
+-rw-r--r--   0        0        0      879 2022-05-02 08:56:10.794887 ecoindex-cli-2.9.0/ecoindex_cli/files.py
+-rw-r--r--   0        0        0      470 2022-05-02 08:56:10.794887 ecoindex-cli-2.9.0/ecoindex_cli/logger.py
+-rw-r--r--   0        0        0        0 2022-05-02 08:56:10.794887 ecoindex-cli-2.9.0/ecoindex_cli/report/__init__.py
+-rw-r--r--   0        0        0     3820 2022-05-02 08:56:10.794887 ecoindex-cli-2.9.0/ecoindex_cli/report/report.py
+-rw-r--r--   0        0        0     7978 2022-05-02 08:56:10.794887 ecoindex-cli-2.9.0/ecoindex_cli/report/template.html
+-rw-r--r--   0        0        0      857 2022-05-02 08:56:10.794887 ecoindex-cli-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0    10211 2022-05-02 08:57:03.872462 ecoindex-cli-2.9.0/setup.py
+-rw-r--r--   0        0        0     9847 2022-05-02 08:57:03.873217 ecoindex-cli-2.9.0/PKG-INFO
```

### Comparing `ecoindex-cli-2.8.1/LICENSE` & `ecoindex-cli-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoindex-cli-2.8.1/README.md` & `ecoindex-cli-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `ecoindex-cli-2.8.1/ecoindex_cli/cli/app.py` & `ecoindex-cli-2.9.0/ecoindex_cli/cli/app.py`

 * *Files identical despite different names*

### Comparing `ecoindex-cli-2.8.1/ecoindex_cli/cli/arguments_handler.py` & `ecoindex-cli-2.9.0/ecoindex_cli/cli/arguments_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from tempfile import NamedTemporaryFile
 from typing import List, Optional, Set, Tuple
 from urllib.parse import urlparse
 
 from click.exceptions import BadParameter
-from ecoindex.models import WindowSize
 from ecoindex_cli.crawl import EcoindexSpider
+from ecoindex_scraper.models import WindowSize
 from pydantic import validate_arguments
 from pydantic.error_wrappers import ErrorWrapper, ValidationError
 from pydantic.networks import HttpUrl
 from pydantic.types import FilePath
 from scrapy.crawler import CrawlerProcess
```

### Comparing `ecoindex-cli-2.8.1/ecoindex_cli/crawl.py` & `ecoindex-cli-2.9.0/ecoindex_cli/crawl.py`

 * *Files identical despite different names*

### Comparing `ecoindex-cli-2.8.1/ecoindex_cli/files.py` & `ecoindex-cli-2.9.0/ecoindex_cli/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from csv import DictWriter
 from os import makedirs
 from os.path import exists
 from typing import List
 
-from ecoindex.models import Result
+from ecoindex_scraper.models import Result
 
 
 def create_folder(path: str) -> None:
     if not exists(path):
         makedirs(path)
```

### Comparing `ecoindex-cli-2.8.1/ecoindex_cli/report/report.py` & `ecoindex-cli-2.9.0/ecoindex_cli/report/report.py`

 * *Files identical despite different names*

### Comparing `ecoindex-cli-2.8.1/ecoindex_cli/report/template.html` & `ecoindex-cli-2.9.0/ecoindex_cli/report/template.html`

 * *Files identical despite different names*

### Comparing `ecoindex-cli-2.8.1/pyproject.toml` & `ecoindex-cli-2.9.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecoindex-cli"
-version = "v2.8.1"
+version = "v2.9.0"
 description = "`ecoindex-cli` is a CLI tool that let you make ecoindex tests on given pages"
 authors = ["Vincent Vatelot <vincent.vatelot@ik.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "http://www.ecoindex.fr"
 repository = "https://github.com/cnumr/ecoindex_cli"
 include = [
@@ -12,22 +12,22 @@
 ]
 
 [tool.poetry.scripts]
 ecoindex-cli = "ecoindex_cli.cli.app:app"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-ecoindex = {version = "^2.11.0", allow-prereleases = true}
 typer = ">=0.3.2,<0.5.0"
 pandas = "^1.3.3"
 Jinja2 = "^3.0.1"
 matplotlib = "^3.4.3"
 click-spinner = "^0.1.10"
 pydantic = "^1.8.2"
 Scrapy = "^2.5.0"
+ecoindex-scraper = "^1.2.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1"
 black = {version = "^22.3", allow-prereleases = true}
 pytest-cov = "^3.0.0"
 
 [build-system]
```

### Comparing `ecoindex-cli-2.8.1/setup.py` & `ecoindex-cli-2.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['Jinja2>=3.0.1,<4.0.0',
  'Scrapy>=2.5.0,<3.0.0',
  'click-spinner>=0.1.10,<0.2.0',
- 'ecoindex>=2.11.0,<3.0.0',
+ 'ecoindex-scraper>=1.2.0,<2.0.0',
  'matplotlib>=3.4.3,<4.0.0',
  'pandas>=1.3.3,<2.0.0',
  'pydantic>=1.8.2,<2.0.0',
  'typer>=0.3.2,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['ecoindex-cli = ecoindex_cli.cli.app:app']}
 
 setup_kwargs = {
     'name': 'ecoindex-cli',
-    'version': '2.8.1',
+    'version': '2.9.0',
     'description': '`ecoindex-cli` is a CLI tool that let you make ecoindex tests on given pages',
     'long_description': '# Ecoindex-Cli\n\n[![Quality check](https://github.com/cnumr/ecoindex_cli/workflows/Quality%20checks/badge.svg)](https://github.com/cnumr/ecoindex_cli/actions/workflows/quality.yml)\n[![PyPI version](https://badge.fury.io/py/ecoindex-cli.svg)](https://badge.fury.io/py/ecoindex-cli)\n\nThis tool provides an easy way to analyze websites with [Ecoindex](http://www.ecoindex.fr) from your local computer. You have the ability to:\n\n- Make the analysis on multiple pages\n- Define multiple screen resolution\n- Make a recursive analysis from a given website\n\nThis CLI is built on top of [ecoindex-python](https://pypi.org/project/ecoindex/) with [Typer](https://typer.tiangolo.com/)\n\nThe output is always a CSV file with the results of the analysis.\n\n> **Current limitation:** This does not work well with SPA.\n\n## Requirements\n\n- Python ^3.8\n- [pip](https://pip.pypa.io/en/stable/)\n\n## Setup\n\n```bash\npip install --user -U ecoindex-cli\n```\n\n## Use case\n\nThe cli gets 2 commands: `analyze` and `report` which can be used separately:\n\n```bash\necoindex-cli --help                                \n```\n\n```bash\nUsage: ecoindex-cli [OPTIONS] COMMAND [ARGS]...\n\n  Ecoindex cli to make analysis of webpages\n\nOptions:\n  --install-completion [bash|zsh|fish|powershell|pwsh]\n                                  Install completion for the specified shell.\n  --show-completion [bash|zsh|fish|powershell|pwsh]\n                                  Show completion for the specified shell, to\n                                  copy it or customize the installation.\n\n  --help                          Show this message and exit.\n\nCommands:\n  analyze  Make an ecoindex analysis of given webpages or website.\n  report   If you already performed an ecoindex analysis and have your...\n```\n\n### Make a simple analysis\n\nYou give just one web url\n\n```bash\necoindex-cli analyze --url http://www.ecoindex.fr\n```\n\n<details><summary>Result</summary>\n\n```bash\nThere are 1 url(s), do you want to process? [Y/n]:\n1 urls for 1 window size\nProcessing  [####################################]  100%\n🙌️ File /tmp/ecoindex-cli/output/www.ecoindex.fr/2021-04-20_164433/results.csv written !\n```\n\n</details>\n\n> This makes an analysis with a screen resolution of 1920x1080px by default\n\n### Set the output file\n\nYou can define the csv output file\n\n```bash\necoindex-cli analyze --url http://www.ecoindex.fr --output-file ~/ecoindex-results/ecoindex.csv\n```\n\n<details><summary>Result</summary>\n\n```bash\n📁️ Urls recorded in file `input/www.ecoindex.fr.csv`\nThere are 1 url(s), do you want to process? [Y/n]:\n1 urls for 1 window size\nProcessing  [####################################]  100%\n🙌️ File /home/vvatelot/ecoindex-results/ecoindex.csv written !\n```\n\n</details>\n\n### Multiple url analysis\n\n```bash\necoindex-cli analyze --url http://www.ecoindex.fr --url https://www.greenit.fr/\n```\n\n<details><summary>Result</summary>\n\n```bash\nThere are 2 url(s), do you want to process? [Y/n]:\n2 urls for 1 window size\nProcessing  [####################################]  100%\n🙌️ File /tmp/ecoindex-cli/output/www.ecoindex.fr/2021-04-20_164524/results.csv written !\n```\n\n</details>\n\n### Provide urls from a file\n\nYou can use a file with given urls that you want to analyze: One url per line. This is helpful if you want to play the same scenario recurrently.\n\n```bash\necoindex-cli analyze --urls-file input/ecoindex.csv\n```\n\n<details><summary>Result</summary>\n\n```bash\nThere are 2 url(s), do you want to process? [Y/n]:\n2 urls for 1 window size\nProcessing  [####################################]  100%\n🙌️ File /tmp/ecoindex-cli/output/www.ecoindex.fr/2021-04-20_164524/results.csv written !\n```\n\n</details>\n\n### Make a recursive analysis\n\nYou can make a recursive analysis of a given webiste. This means that the app will try to find out all the pages into your website and launch an analysis on all those web pages. ⚠️ This can process for a very long time! **Use it at your own risks!**\n\n```bash\necoindex-cli analyze --url http://www.ecoindex.fr --recursive\n```\n\n<details><summary>Result</summary>\n\n```bash\n⏲️ Crawling root url http://www.ecoindex.fr -> Wait a minute !\n📁️ Urls recorded in file `/tmp/ecoindex-cli/input/www.ecoindex.fr.csv`\nThere are 3 url(s), do you want to process? [Y/n]:\n3 urls for 1 window size\nProcessing  [####################################]  100%\n🙌️ File /tmp/ecoindex-cli/output/www.ecoindex.fr/2021-04-20_164729/results.csv written !\n```\n\n</details>\n\n### Disable console interaction\n\nYou can disable confirmations, and force the app to answer yes to all of them. It can be useful if you need to start the app from another script, or if you have no time to wait it to finish.\n\n```bash\necoindex-cli analyze --url http://www.ecoindex.fr --recursive --no-interaction\n```\n\n<details><summary>Result</summary>\n\n```bash\n⏲️ Crawling root url http://www.ecoindex.fr -> Wait a minute !\n📁️ Urls recorded in file `/tmp/ecoindex-cli/input/www.ecoindex.fr.csv`\n3 urls for 1 window size\nProcessing  [####################################]  100%\n🙌️ File /tmp/ecoindex-cli/output/www.ecoindex.fr/2021-11-04_081913/results.csv written !\n```\n\n</details>\n\n### Set other screen resolutions\n\nYou can provide other screen resolutions. By default, the screen resolution is `1920x1080px` but you can provide other resolution for example if you want to test ecoindex for mobile.\n\n```bash\necoindex-cli analyze --url http://www.ecoindex.fr --window-size 1920,1080 --window-size 386,540\n```\n\n<details><summary>Result</summary>\n\n```bash\nThere are 1 url(s), do you want to process? [Y/n]:\n1 urls for 2 window size\nProcessing  [####################################]  100%\n🙌️ File /tmp/ecoindex-cli/output/www.ecoindex.fr/2021-04-21_212244/results.csv written !\n```\n\n</details>\n\n### Generate a html report\n\nYou can generate a html report easily at the end of the analysis. You just have to add the option `--html-report`.\n\n```bash\necoindex-cli analyze --url http://www.ecoindex.fr --recursive --html-report\n```\n\n<details><summary>Result</summary>\n\n```bash\n⏲️ Crawling root url http://www.ecoindex.fr -> Wait a minute !\n📁️ Urls recorded in file `input/www.ecoindex.fr.csv`\nThere are 3 url(s), do you want to process? [Y/n]:\n3 urls for 1 window size\nProcessing  [####################################]  100%\n🙌️ File output/www.ecoindex.fr/2021-04-21_212127/results.csv written !\n🦄️ Amazing! A report has been generated to `/tmp/ecoindex-cli/output/www.ecoindex.fr/2021-04-21_212127/report.html`\n```\n\n</details>\n\nHere is a sample result:\n![Sample report](doc/report.png)\n\n### Only generate a report from existing result file\n\nIf you already performed an anlayzis and (for example), forgot to generate the html report, you do not need to re-run a full analyzis, you can simply request a report from your result file :\n\n```bash\necoindex-cli report "/tmp/ecoindex-cli/output/www.ecoindex.fr/2021-05-06_191355/results.csv" "www.synchrone.fr"\n```\n\n<details><summary>Result</summary>\n\n```bash\n🦄️ Amazing! A report has been generated to `/tmp/ecoindex-cli/output/www.ecoindex.fr/2021-05-06_191355/report.html`\n```\n\n</details>\n\n\n## Results example\n\nThe result of the analysis is a CSV file which can be easily used for further analysis:\n\n```csv\nsize,nodes,requests,grade,score,ges,water,url,date,resolution,page_type\n119.095,45,8,A,89,1.22,1.83,http://www.ecoindex.fr,2021-04-20 16:45:28.570179,"1920,1080",\n769.252,730,94,D,41,2.18,3.27,https://www.greenit.fr/,2021-04-20 16:45:32.199242,"1920,1080",website\n```\n\nWhere:\n\n- `size` is the size of the page and of the downloaded elements of the page in KB\n- `nodes` is the number of the DOM elements in the page\n- `requests` is the number of external requests made by the page\n- `grade` is the corresponding ecoindex grade of the page (from A to G)\n- `score`\xa0is the corresponding ecoindex score of the page (0 to 100)\n- `ges` is the equivalent of greenhouse gases emission (in `gCO2e`) of the page\n- `water`is the equivalent water consumption (in `cl`) of the page\n- `url` is the analysed page url\n- `date` is the datetime of the page analysis\n- `resolution` is the screen resolution used for the page analysis (`width,height`)\n- `page_type` is the type of the page, based ton the [opengraph type tag](https://ogp.me/#types)\n\n## Testing\n\nIn order to develop or test, you have to use [Poetry](https://python-poetry.org/), install the dependencies and execute a poetry shell:\n\n```bash\npoetry install && \\\npoetry shell\n```\n\nWe use Pytest to run unit tests for this project. The test suite are in the `tests` folder. Just execute :\n\n```bash\npytest --cov-report term-missing:skip-covered --cov=. --cov-config=.coveragerc tests\n```\n\n> This runs pytest and also generate a [coverage report](https://pytest-cov.readthedocs.io/en/latest/) (terminal and html)\n\n## [Contributing](CONTRIBUTING.md)\n\n## [Code of conduct](CODE_OF_CONDUCT.md)\n',
     'author': 'Vincent Vatelot',
     'author_email': 'vincent.vatelot@ik.me',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'http://www.ecoindex.fr',
```

### Comparing `ecoindex-cli-2.8.1/PKG-INFO` & `ecoindex-cli-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ecoindex-cli
-Version: 2.8.1
+Version: 2.9.0
 Summary: `ecoindex-cli` is a CLI tool that let you make ecoindex tests on given pages
 Home-page: http://www.ecoindex.fr
 License: MIT
 Author: Vincent Vatelot
 Author-email: vincent.vatelot@ik.me
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Jinja2 (>=3.0.1,<4.0.0)
 Requires-Dist: Scrapy (>=2.5.0,<3.0.0)
 Requires-Dist: click-spinner (>=0.1.10,<0.2.0)
-Requires-Dist: ecoindex (>=2.11.0,<3.0.0)
+Requires-Dist: ecoindex-scraper (>=1.2.0,<2.0.0)
 Requires-Dist: matplotlib (>=3.4.3,<4.0.0)
 Requires-Dist: pandas (>=1.3.3,<2.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: typer (>=0.3.2,<0.5.0)
 Project-URL: Repository, https://github.com/cnumr/ecoindex_cli
 Description-Content-Type: text/markdown
```

