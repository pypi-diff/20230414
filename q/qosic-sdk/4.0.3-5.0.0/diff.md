# Comparing `tmp/qosic_sdk-4.0.3.tar.gz` & `tmp/qosic_sdk-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qosic_sdk-4.0.3.tar", max compression
+gzip compressed data, was "qosic_sdk-5.0.0.tar", max compression
```

## Comparing `qosic_sdk-4.0.3.tar` & `qosic_sdk-5.0.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-03-12 21:28:03.303354 qosic_sdk-4.0.3/LICENSE
--rw-r--r--   0        0        0     2637 2023-03-12 21:59:35.242782 qosic_sdk-4.0.3/README.rst
--rw-r--r--   0        0        0     1297 2023-03-12 22:12:11.303068 qosic_sdk-4.0.3/pyproject.toml
--rw-r--r--   0        0        0      245 2023-03-12 21:28:03.304354 qosic_sdk-4.0.3/qosic/__init__.py
--rw-r--r--   0        0        0     2339 2023-03-12 21:28:03.304354 qosic_sdk-4.0.3/qosic/api.py
--rw-r--r--   0        0        0      443 2023-03-12 21:28:03.304354 qosic_sdk-4.0.3/qosic/constants.py
--rw-r--r--   0        0        0      302 2023-03-12 21:28:03.304354 qosic_sdk-4.0.3/qosic/errors.py
--rw-r--r--   0        0        0      320 2023-03-12 21:28:03.304354 qosic_sdk-4.0.3/qosic/logger.py
--rw-r--r--   0        0        0      407 2023-03-12 21:28:03.304354 qosic_sdk-4.0.3/qosic/protocols.py
--rw-r--r--   0        0        0     6102 2023-03-12 21:28:03.304354 qosic_sdk-4.0.3/qosic/providers.py
--rw-r--r--   0        0        0        0 2023-03-12 21:28:03.304354 qosic_sdk-4.0.3/qosic/py.typed
--rw-r--r--   0        0        0     1937 2023-03-12 21:28:03.304354 qosic_sdk-4.0.3/qosic/utils.py
--rw-r--r--   0        0        0     3424 1970-01-01 00:00:00.000000 qosic_sdk-4.0.3/setup.py
--rw-r--r--   0        0        0     3635 1970-01-01 00:00:00.000000 qosic_sdk-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-12 21:28:03.303354 qosic_sdk-5.0.0/LICENSE
+-rw-r--r--   0        0        0     2689 2023-04-14 01:28:48.893584 qosic_sdk-5.0.0/README.rst
+-rw-r--r--   0        0        0     1455 2023-04-14 01:32:48.475923 qosic_sdk-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0      239 2023-04-14 01:14:33.379707 qosic_sdk-5.0.0/qosic/__init__.py
+-rw-r--r--   0        0        0     2324 2023-04-14 01:31:39.956112 qosic_sdk-5.0.0/qosic/client.py
+-rw-r--r--   0        0        0      373 2023-04-14 00:58:28.576720 qosic_sdk-5.0.0/qosic/errors.py
+-rw-r--r--   0        0        0      320 2023-03-12 21:28:03.304354 qosic_sdk-5.0.0/qosic/logger.py
+-rw-r--r--   0        0        0        0 2023-04-14 01:15:19.899605 qosic_sdk-5.0.0/qosic/mobile_carriers/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-14 01:16:57.383390 qosic_sdk-5.0.0/qosic/mobile_carriers/bj/__init__.py
+-rw-r--r--   0        0        0     1605 2023-04-14 01:27:02.658877 qosic_sdk-5.0.0/qosic/mobile_carriers/bj/moov.py
+-rw-r--r--   0        0        0     3639 2023-04-14 01:26:12.206016 qosic_sdk-5.0.0/qosic/mobile_carriers/bj/mtn.py
+-rw-r--r--   0        0        0     2103 2023-04-14 01:30:49.059252 qosic_sdk-5.0.0/qosic/mobile_carriers/utils.py
+-rw-r--r--   0        0        0      424 2023-04-14 01:11:42.396009 qosic_sdk-5.0.0/qosic/protocols.py
+-rw-r--r--   0        0        0        0 2023-03-12 21:28:03.304354 qosic_sdk-5.0.0/qosic/py.typed
+-rw-r--r--   0        0        0     2036 2023-04-14 01:30:29.259307 qosic_sdk-5.0.0/qosic/utils.py
+-rw-r--r--   0        0        0     3734 1970-01-01 00:00:00.000000 qosic_sdk-5.0.0/PKG-INFO
```

### Comparing `qosic_sdk-4.0.3/LICENSE` & `qosic_sdk-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qosic_sdk-4.0.3/README.rst` & `qosic_sdk-5.0.0/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -48,15 +48,16 @@
 
        pip install qosic-sdk
 
 .. code:: python3
 
 
        from dotenv import dotenv_values
-       from qosic import Client, MTN, MOOV
+       from qosic import Client
+       from qosic.mobile_carriers import bj
 
        config = dotenv_values(".env")
 
        moov_client_id = config.get("MOOV_CLIENT_ID")
        mtn_client_id = config.get("MTN_CLIENT_ID")
        server_login = config.get("SERVER_LOGIN")
        server_pass = config.get("SERVER_PASSWORD")
@@ -64,22 +65,22 @@
        phone = config.get("PHONE_NUMBER")
 
 
        def main():
            client = Client(
                login=server_login,
                password=server_pass,
-               providers=[MTN(id=mtn_client_id), MOOV(id=moov_client_id)],
+               providers=[bj.MTN(id=mtn_client_id), bj.MOOV(id=moov_client_id)],
            )
            result = client.pay(phone=phone, amount=500, first_name="User", last_name="TEST")
            print(result)
            if result.success:
                print(f"Everything went fine")
 
-           result = client.refund(reference=result.reference)
+           result = client.refund(reference=result.reference, phone=phone)
            print(result)
 
 
        if __name__ == "__main__":
            main()
 
 Credits
```

### Comparing `qosic_sdk-4.0.3/pyproject.toml` & `qosic_sdk-5.0.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qosic-sdk"
-version = "4.0.3"
+version = "5.0.0"
 description = "An unofficial python sdk for the QosIc platform."
 authors = ["Tobi-De <tobidegnon@protonmail.com>"]
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/Tobi-De/qosic-sdk"
 homepage = "https://github.com/Tobi-De/qosic-sdk"
 keywords = ["python", "qosic-sdk", "qosic", "qos", "payment", "momo", "mobile money"]
@@ -17,27 +17,33 @@
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "License :: OSI Approved :: MIT License",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-httpx = "^0.23.3"
+httpx = "^0.24.0"
 polling2 = "^0.5.0"
+shibuya = "^2023.3.19"
 
-[tool.poetry.dev-dependencies]
-black = "^23.1.0"
-mypy = "^1.1.1"
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+mypy = "^1.2.0"
 python-dotenv = "^1.0.0"
-coverage = "^7.2.1"
-furo = "^2022.12.7"
+coverage = "^7.2.3"
+furo = "^2023.3.27"
 types-dataclasses = "^0.6.6"
-pytest = "^7.2.2"
-pytest-httpx = "^0.21.3"
+pytest = "^7.3.0"
+pytest-httpx = "^0.22.0"
 myst-parser = "^1.0.0"
+sphinx-watch = "^0.1.2"
+poethepoet = "^0.19.0"
+
+[tool.poe.tasks]
+docs = "sphinx-watch docs docs/_build html --httpd --port 8080"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     "error",
     "ignore::UserWarning",
     # note the use of single quote below to denote "raw" strings in TOML
     'ignore:function ham\(\) is deprecated:DeprecationWarning',
```

### Comparing `qosic_sdk-4.0.3/qosic/utils.py` & `qosic_sdk-5.0.0/qosic/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 from logging import Logger
 from string import ascii_letters, digits
 from typing import TYPE_CHECKING
 
 import httpx
 from dataclasses import dataclass
 
-from .errors import ProviderNotFoundError, InvalidPhoneNumberError
+from .errors import MobileCarrierNotFoundError, InvalidPhoneNumberError
 
 if TYPE_CHECKING:
-    from .protocols import Provider
+    from .protocols import MobileCarrier
 
 
 def log_request(request: httpx.Request, /, *, logger: Logger):
     logger.info(f"REQUEST: {request.method} {request.url} - Waiting for response")
     logger.info(request.read())
 
 
@@ -29,47 +29,50 @@
     logger.info(f"{response.read()}")
 
 
 def get_random_string(length: int = 12) -> str:
     return "".join(secrets.choice(ascii_letters + digits) for _ in range(length))
 
 
-def provider_by_phone(*, phone: str, providers: list[Provider]) -> Provider:
+def guess_mobile_carrier_from(
+    *, phone: str, mobile_carriers: list[MobileCarrier]
+) -> MobileCarrier:
     prefix = phone[3:5]
-    for provider in providers:
-        if prefix in provider.allowed_prefixes:
-            return provider
-    raise ProviderNotFoundError(
+    for carrier in mobile_carriers:
+        if prefix in carrier.allowed_prefixes:
+            return carrier
+    raise MobileCarrierNotFoundError(
         f"A provider was not found for the given phone number: {phone}"
     )
 
 
 @dataclass(frozen=True)
 class Result:
     """A helper class to summarize the responses from the server."""
 
     class Status(str, Enum):
         CONFIRMED = "CONFIRMED"
         FAILED = "FAILED"
 
     status: Status
     reference: str
-    provider: Provider
+    phone: str
+    mobile_carrier: MobileCarrier
     response: httpx.Response
 
     @property
     def success(self) -> bool:
         return self.status == self.Status.CONFIRMED
 
 
 @dataclass(frozen=True)
 class Payer:
     phone: str
     amount: int
-    first_name: str
-    last_name: str
+    first_name: str | None = None
+    last_name: str | None = None
 
     def __post_init__(self):
-        if not re.fullmatch(r"[0-9]{11}", self.phone):
+        if not re.fullmatch(r"\d{11}", self.phone):
             raise InvalidPhoneNumberError(
                 f"Invalid format for {self.phone}, ex: 229XXXXXXXX"
             )
```

### Comparing `qosic_sdk-4.0.3/setup.py` & `qosic_sdk-5.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,120 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: qosic-sdk
+Version: 5.0.0
+Summary: An unofficial python sdk for the QosIc platform.
+Home-page: https://github.com/Tobi-De/qosic-sdk
+License: MIT
+Keywords: python,qosic-sdk,qosic,qos,payment,momo,mobile money
+Author: Tobi-De
+Author-email: tobidegnon@protonmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: polling2 (>=0.5.0,<0.6.0)
+Requires-Dist: shibuya (>=2023.3.19,<2024.0.0)
+Project-URL: Repository, https://github.com/Tobi-De/qosic-sdk
+Description-Content-Type: text/x-rst
+
+qosic-sdk
+=========
+
+An unofficial python sdk for the `QosIC <https://www.qosic.com/>`__
+platform. This platform provides an api to enable mobile money payments
+for businesses in Africa.
+
+
+.. image:: https://img.shields.io/pypi/v/qosic-sdk.svg
+        :target: https://pypi.python.org/pypi/qosic-sdk
+
+.. image:: https://img.shields.io/pypi/pyversions/qosic-sdk
+        :target: https://github.com/Tobi-De/qosic-sdk
+
+.. image:: https://api.travis-ci.com/Tobi-De/qosic-sdk.svg
+        :target: https://travis-ci.com/Tobi-De/qosic-sdk
+
+.. image:: https://readthedocs.org/projects/qosic-sdk/badge/?version=latest
+        :target: https://qosic-sdk.readthedocs.io/en/latest/?version=latest
+        :alt: Documentation Status
+
+.. image:: https://img.shields.io/badge/license-MIT-blue.svg
+        :target: https://github.com/Tobi-De/qosic-sdk/blob/main/LICENSE
+
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+        :target: https://github.com/psf/black
+
+----
+
+-  Free software: MIT license
+-  Documentation: https://qosic-sdk.readthedocs.io.
+
+Features
+--------
+
+-  Simple synchronous client to make your payment requests
+-  Cover 100% of Qosic public api
+-  Clean and meaningful exceptions
+-  100 % test coverage
+-  Configurable timeouts
+
+Quickstart
+----------
+
+For those of you in a hurry, here’s a sample code to get you started.
+
+.. code:: shell
+
+       pip install qosic-sdk
+
+.. code:: python3
+
+
+       from dotenv import dotenv_values
+       from qosic import Client
+       from qosic.mobile_carriers import bj
+
+       config = dotenv_values(".env")
+
+       moov_client_id = config.get("MOOV_CLIENT_ID")
+       mtn_client_id = config.get("MTN_CLIENT_ID")
+       server_login = config.get("SERVER_LOGIN")
+       server_pass = config.get("SERVER_PASSWORD")
+       # This is just for test purpose, you should directly pass the phone number
+       phone = config.get("PHONE_NUMBER")
+
+
+       def main():
+           client = Client(
+               login=server_login,
+               password=server_pass,
+               providers=[bj.MTN(id=mtn_client_id), bj.MOOV(id=moov_client_id)],
+           )
+           result = client.pay(phone=phone, amount=500, first_name="User", last_name="TEST")
+           print(result)
+           if result.success:
+               print(f"Everything went fine")
+
+           result = client.refund(reference=result.reference, phone=phone)
+           print(result)
+
+
+       if __name__ == "__main__":
+           main()
+
+Credits
+-------
+
+This package was created with
+`Cookiecutter <https://github.com/audreyr/cookiecutter>`__ and the
+`audreyr/cookiecutter-pypackage <https://github.com/audreyr/cookiecutter-pypackage>`__
+project template.
 
-packages = \
-['qosic']
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['httpx>=0.23.3,<0.24.0', 'polling2>=0.5.0,<0.6.0']
-
-setup_kwargs = {
-    'name': 'qosic-sdk',
-    'version': '4.0.3',
-    'description': 'An unofficial python sdk for the QosIc platform.',
-    'long_description': 'qosic-sdk\n=========\n\nAn unofficial python sdk for the `QosIC <https://www.qosic.com/>`__\nplatform. This platform provides an api to enable mobile money payments\nfor businesses in Africa.\n\n\n.. image:: https://img.shields.io/pypi/v/qosic-sdk.svg\n        :target: https://pypi.python.org/pypi/qosic-sdk\n\n.. image:: https://img.shields.io/pypi/pyversions/qosic-sdk\n        :target: https://github.com/Tobi-De/qosic-sdk\n\n.. image:: https://api.travis-ci.com/Tobi-De/qosic-sdk.svg\n        :target: https://travis-ci.com/Tobi-De/qosic-sdk\n\n.. image:: https://readthedocs.org/projects/qosic-sdk/badge/?version=latest\n        :target: https://qosic-sdk.readthedocs.io/en/latest/?version=latest\n        :alt: Documentation Status\n\n.. image:: https://img.shields.io/badge/license-MIT-blue.svg\n        :target: https://github.com/Tobi-De/qosic-sdk/blob/main/LICENSE\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n        :target: https://github.com/psf/black\n\n----\n\n-  Free software: MIT license\n-  Documentation: https://qosic-sdk.readthedocs.io.\n\nFeatures\n--------\n\n-  Simple synchronous client to make your payment requests\n-  Cover 100% of Qosic public api\n-  Clean and meaningful exceptions\n-  100 % test coverage\n-  Configurable timeouts\n\nQuickstart\n----------\n\nFor those of you in a hurry, here’s a sample code to get you started.\n\n.. code:: shell\n\n       pip install qosic-sdk\n\n.. code:: python3\n\n\n       from dotenv import dotenv_values\n       from qosic import Client, MTN, MOOV\n\n       config = dotenv_values(".env")\n\n       moov_client_id = config.get("MOOV_CLIENT_ID")\n       mtn_client_id = config.get("MTN_CLIENT_ID")\n       server_login = config.get("SERVER_LOGIN")\n       server_pass = config.get("SERVER_PASSWORD")\n       # This is just for test purpose, you should directly pass the phone number\n       phone = config.get("PHONE_NUMBER")\n\n\n       def main():\n           client = Client(\n               login=server_login,\n               password=server_pass,\n               providers=[MTN(id=mtn_client_id), MOOV(id=moov_client_id)],\n           )\n           result = client.pay(phone=phone, amount=500, first_name="User", last_name="TEST")\n           print(result)\n           if result.success:\n               print(f"Everything went fine")\n\n           result = client.refund(reference=result.reference)\n           print(result)\n\n\n       if __name__ == "__main__":\n           main()\n\nCredits\n-------\n\nThis package was created with\n`Cookiecutter <https://github.com/audreyr/cookiecutter>`__ and the\n`audreyr/cookiecutter-pypackage <https://github.com/audreyr/cookiecutter-pypackage>`__\nproject template.\n\n',
-    'author': 'Tobi-De',
-    'author_email': 'tobidegnon@protonmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Tobi-De/qosic-sdk',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

