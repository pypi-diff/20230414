# Comparing `tmp/repository_service_tuf-0.1.0a1.tar.gz` & `tmp/repository_service_tuf-0.1.1a2.tar.gz`

## Comparing `repository_service_tuf-0.1.0a1.tar` & `repository_service_tuf-0.1.1a2.tar`

### file list

```diff
@@ -1,91 +1,93 @@
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/.gitignore
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/.readthedocs.yaml
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/CODE_OF_CONDUCT.rst
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/LICENSE
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/MAINTAINERS.rst
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/Makefile
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/Pipfile
--rw-r--r--   0        0        0    81107 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/Pipfile.lock
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/README.rst
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/id_ed25519
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/id_ed25519.pub
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/requirements-dev.txt
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/requirements.txt
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tox.ini
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/.github/dependabot.yml
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/.github/ISSUE_TEMPLATE/other.yml
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/.github/ISSUE_TEMPLATE/task.yml
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/.github/PULL_REQUEST_TEMPLATE/pr.yml
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/.github/workflows/cd.yml
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/.github/workflows/update-python-deps.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/make.bat
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/requirements.txt
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/diagrams/repository-service-tuf-cli-C1.puml
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/diagrams/repository-service-tuf-cli-C2.puml
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/diagrams/repository-service-tuf-cli-C3.puml
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/source/conf.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/source/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/source/_static/INFO
--rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/source/_static/repository-service-tuf-cli-C1.png
--rw-r--r--   0        0        0    41916 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/source/_static/repository-service-tuf-cli-C2.png
--rw-r--r--   0        0        0    94852 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/source/_static/repository-service-tuf-cli-C3.png
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/source/devel/design.rst
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/source/devel/index.rst
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/source/devel/modules.rst
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/source/devel/repository_service_tuf.cli.admin.rst
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/source/devel/repository_service_tuf.cli.key.rst
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/source/devel/repository_service_tuf.cli.rst
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/source/devel/repository_service_tuf.helpers.rst
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/source/devel/repository_service_tuf.rst
--rw-r--r--   0        0        0    45268 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/docs/source/guide/index.rst
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/repository_service_tuf/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/repository_service_tuf/__version__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/repository_service_tuf/constants.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/repository_service_tuf/cli/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/repository_service_tuf/cli/admin/__init__.py
--rw-r--r--   0        0        0    24520 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/repository_service_tuf/cli/admin/ceremony.py
--rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/repository_service_tuf/cli/admin/import_targets.py
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/repository_service_tuf/cli/admin/login.py
--rw-r--r--   0        0        0     2552 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/repository_service_tuf/cli/admin/token.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/repository_service_tuf/cli/key/__init__.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/repository_service_tuf/cli/key/generate_key.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/repository_service_tuf/helpers/__init__.py
--rw-r--r--   0        0        0     5793 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/repository_service_tuf/helpers/api_client.py
--rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/repository_service_tuf/helpers/tuf.py
--rwxr-xr-x   0        0        0      861 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/2.targets.json
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/conftest.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/test_tuf_repository_service.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/JanisJoplin.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/JanisJoplin.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/JimiHendrix.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/JimiHendrix.pub
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/README.md
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/online-rsa.key
--rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/online-rsa.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/online.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/online.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/keystorage/JanisJoplin.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/keystorage/JanisJoplin.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/keystorage/JimiHendrix.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/keystorage/JimiHendrix.pub
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/keystorage/README.md
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/keystorage/online-rsa.key
--rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/keystorage/online-rsa.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/keystorage/online.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/files/keystorage/online.pub
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/unit/cli/admin/__init__.py
--rw-r--r--   0        0        0    27843 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/unit/cli/admin/test_ceremony.py
--rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/unit/cli/admin/test_import_targets.py
--rw-r--r--   0        0        0    11219 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/unit/cli/admin/test_login.py
--rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/unit/cli/key/test_generate_key.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/unit/helpers/__init__.py
--rw-r--r--   0        0        0    20035 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/unit/helpers/test_api_client.py
--rw-r--r--   0        0        0    12210 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/tests/unit/helpers/test_tuf.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.gitignore
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.readthedocs.yaml
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/CODE_OF_CONDUCT.rst
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/LICENSE
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/MAINTAINERS.rst
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/Makefile
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/Pipfile
+-rw-r--r--   0        0        0    80773 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/Pipfile.lock
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/README.rst
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/id_ed25519
+-rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/id_ed25519.pub
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/pyproject.toml
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/requirements-dev.txt
+-rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/requirements.txt
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/rstuf.ini
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tox.ini
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/ISSUE_TEMPLATE/other.yml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/ISSUE_TEMPLATE/task.yml
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/PULL_REQUEST_TEMPLATE/pr.yml
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/.github/workflows/update-python-deps.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/make.bat
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/requirements.txt
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/diagrams/repository-service-tuf-cli-C1.puml
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/diagrams/repository-service-tuf-cli-C2.puml
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/diagrams/repository-service-tuf-cli-C3.puml
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/conf.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/_static/INFO
+-rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/_static/repository-service-tuf-cli-C1.png
+-rw-r--r--   0        0        0    41916 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/_static/repository-service-tuf-cli-C2.png
+-rw-r--r--   0        0        0    94852 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/_static/repository-service-tuf-cli-C3.png
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/design.rst
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/index.rst
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/modules.rst
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/repository_service_tuf.cli.admin.rst
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/repository_service_tuf.cli.key.rst
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/repository_service_tuf.cli.rst
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/repository_service_tuf.helpers.rst
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/devel/repository_service_tuf.rst
+-rw-r--r--   0        0        0    45409 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/docs/source/guide/index.rst
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/__version__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/constants.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/__init__.py
+-rw-r--r--   0        0        0    24979 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/ceremony.py
+-rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/import_targets.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/login.py
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/token.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/key/__init__.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/cli/key/generate_key.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/helpers/__init__.py
+-rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/helpers/api_client.py
+-rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/repository_service_tuf/helpers/tuf.py
+-rwxr-xr-x   0        0        0      861 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/2.targets.json
+-rw-r--r--   0        0        0     3656 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/conftest.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/test_tuf_repository_service.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/JanisJoplin.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/JanisJoplin.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/JimiHendrix.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/JimiHendrix.pub
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/README.md
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/online-rsa.key
+-rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/online-rsa.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/online.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/online.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/JanisJoplin.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/JanisJoplin.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/JimiHendrix.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/JimiHendrix.pub
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/README.md
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/online-rsa.key
+-rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/online-rsa.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/online.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/files/keystorage/online.pub
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/cli/test__init__.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/cli/admin/__init__.py
+-rw-r--r--   0        0        0    30060 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/cli/admin/test_ceremony.py
+-rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/cli/admin/test_import_targets.py
+-rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/cli/admin/test_login.py
+-rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/cli/key/test_generate_key.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/helpers/__init__.py
+-rw-r--r--   0        0        0    21182 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/helpers/test_api_client.py
+-rw-r--r--   0        0        0    12210 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/tests/unit/helpers/test_tuf.py
+-rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a2/PKG-INFO
```

### Comparing `repository_service_tuf-0.1.0a1/.gitignore` & `repository_service_tuf-0.1.1a2/.gitignore`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/.pre-commit-config.yaml` & `repository_service_tuf-0.1.1a2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/.readthedocs.yaml` & `repository_service_tuf-0.1.1a2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/CODE_OF_CONDUCT.rst` & `repository_service_tuf-0.1.1a2/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/CONTRIBUTING.rst` & `repository_service_tuf-0.1.1a2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/LICENSE` & `repository_service_tuf-0.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/Pipfile` & `repository_service_tuf-0.1.1a2/Pipfile`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/Pipfile.lock` & `repository_service_tuf-0.1.1a2/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9917792792792793%*

 * *Differences: {"'default'": "{'pygments': {'hashes': "*

 * *              "['sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094', "*

 * *              "'sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500'], "*

 * *              '\'markers\': "python_version >= \'3.7\'", \'version\': \'==2.15.0\'}, \'rich\': '*

 * *              "{'hashes': "*

 * *              "['sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a', "*

 * *              "'sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13 […]*

```diff
@@ -347,19 +347,19 @@
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
             "version": "==2.21"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094",
+                "sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.0"
         },
         "pynacl": {
             "hashes": [
                 "sha256:06b8f6fa7f5de8d5d2f7573fe8c863c051225a27b61e6860fd047b1775807858",
                 "sha256:0c84947a22519e013607c9be43706dd42513f9e6ae5d39d3613ca1e142fba44d",
                 "sha256:20f42270d27e1b6a29f54032090b972d97f0a1b0948cc52392041ef7831fee93",
                 "sha256:401002a4aaa07c9414132aaed7f6836ff98f59277a234704ff66878c2ee4a0d1",
@@ -379,19 +379,19 @@
                 "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
             ],
             "index": "pypi",
             "version": "==2.28.2"
         },
         "rich": {
             "hashes": [
-                "sha256:540c7d6d26a1178e8e8b37e9ba44573a3cd1464ff6348b99ee7061b95d1c6333",
-                "sha256:dc84400a9d842b3a9c5ff74addd8eb798d155f36c1c91303888e0a66850d2a15"
+                "sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a",
+                "sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13f74cf454ccb2f490708b"
             ],
             "index": "pypi",
-            "version": "==13.3.3"
+            "version": "==13.3.4"
         },
         "rich-click": {
             "hashes": [
                 "sha256:0fcf4d1a09029d79322dd814ab0b2e66ac183633037561881d45abae8a161d95",
                 "sha256:f8ff96693ec6e261d1544e9f7d9a5811c5ef5d74c8adb4978430fc0dac16777e"
             ],
             "index": "pypi",
@@ -493,22 +493,14 @@
             "hashes": [
                 "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==0.7.13"
         },
-        "attrs": {
-            "hashes": [
-                "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
-                "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
-            ],
-            "markers": "python_version >= '3.6'",
-            "version": "==22.2.0"
-        },
         "babel": {
             "hashes": [
                 "sha256:b4246fb7677d3b98f501a39d43396d3cafdc8eadb045f4a31be01863f655c610",
                 "sha256:cc2d99999cd01d44420ae725a21c9e3711b3aadc7976d6147f622d8581963455"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.12.1"
@@ -687,68 +679,68 @@
                 "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
             "version": "==0.4.6"
         },
         "coverage": {
             "hashes": [
-                "sha256:006ed5582e9cbc8115d2e22d6d2144a0725db542f654d9d4fda86793832f873d",
-                "sha256:046936ab032a2810dcaafd39cc4ef6dd295df1a7cbead08fe996d4765fca9fe4",
-                "sha256:0484d9dd1e6f481b24070c87561c8d7151bdd8b044c93ac99faafd01f695c78e",
-                "sha256:0ce383d5f56d0729d2dd40e53fe3afeb8f2237244b0975e1427bfb2cf0d32bab",
-                "sha256:186e0fc9cf497365036d51d4d2ab76113fb74f729bd25da0975daab2e107fd90",
-                "sha256:2199988e0bc8325d941b209f4fd1c6fa007024b1442c5576f1a32ca2e48941e6",
-                "sha256:299bc75cb2a41e6741b5e470b8c9fb78d931edbd0cd009c58e5c84de57c06731",
-                "sha256:3668291b50b69a0c1ef9f462c7df2c235da3c4073f49543b01e7eb1dee7dd540",
-                "sha256:36dd42da34fe94ed98c39887b86db9d06777b1c8f860520e21126a75507024f2",
-                "sha256:38004671848b5745bb05d4d621526fca30cee164db42a1f185615f39dc997292",
-                "sha256:387fb46cb8e53ba7304d80aadca5dca84a2fbf6fe3faf6951d8cf2d46485d1e5",
-                "sha256:3eb55b7b26389dd4f8ae911ba9bc8c027411163839dea4c8b8be54c4ee9ae10b",
-                "sha256:420f94a35e3e00a2b43ad5740f935358e24478354ce41c99407cddd283be00d2",
-                "sha256:4ac0f522c3b6109c4b764ffec71bf04ebc0523e926ca7cbe6c5ac88f84faced0",
-                "sha256:4c752d5264053a7cf2fe81c9e14f8a4fb261370a7bb344c2a011836a96fb3f57",
-                "sha256:4f01911c010122f49a3e9bdc730eccc66f9b72bd410a3a9d3cb8448bb50d65d3",
-                "sha256:4f68ee32d7c4164f1e2c8797535a6d0a3733355f5861e0f667e37df2d4b07140",
-                "sha256:4fa54fb483decc45f94011898727802309a109d89446a3c76387d016057d2c84",
-                "sha256:507e4720791977934bba016101579b8c500fb21c5fa3cd4cf256477331ddd988",
-                "sha256:53d0fd4c17175aded9c633e319360d41a1f3c6e352ba94edcb0fa5167e2bad67",
-                "sha256:55272f33da9a5d7cccd3774aeca7a01e500a614eaea2a77091e9be000ecd401d",
-                "sha256:5764e1f7471cb8f64b8cda0554f3d4c4085ae4b417bfeab236799863703e5de2",
-                "sha256:57b77b9099f172804e695a40ebaa374f79e4fb8b92f3e167f66facbf92e8e7f5",
-                "sha256:5afdad4cc4cc199fdf3e18088812edcf8f4c5a3c8e6cb69127513ad4cb7471a9",
-                "sha256:5cc0783844c84af2522e3a99b9b761a979a3ef10fb87fc4048d1ee174e18a7d8",
-                "sha256:5e1df45c23d4230e3d56d04414f9057eba501f78db60d4eeecfcb940501b08fd",
-                "sha256:6146910231ece63facfc5984234ad1b06a36cecc9fd0c028e59ac7c9b18c38c6",
-                "sha256:797aad79e7b6182cb49c08cc5d2f7aa7b2128133b0926060d0a8889ac43843be",
-                "sha256:7c20b731211261dc9739bbe080c579a1835b0c2d9b274e5fcd903c3a7821cf88",
-                "sha256:817295f06eacdc8623dc4df7d8b49cea65925030d4e1e2a7c7218380c0072c25",
-                "sha256:81f63e0fb74effd5be736cfe07d710307cc0a3ccb8f4741f7f053c057615a137",
-                "sha256:872d6ce1f5be73f05bea4df498c140b9e7ee5418bfa2cc8204e7f9b817caa968",
-                "sha256:8c99cb7c26a3039a8a4ee3ca1efdde471e61b4837108847fb7d5be7789ed8fd9",
-                "sha256:8dbe2647bf58d2c5a6c5bcc685f23b5f371909a5624e9f5cd51436d6a9f6c6ef",
-                "sha256:8efb48fa743d1c1a65ee8787b5b552681610f06c40a40b7ef94a5b517d885c54",
-                "sha256:92ebc1619650409da324d001b3a36f14f63644c7f0a588e331f3b0f67491f512",
-                "sha256:9d22e94e6dc86de981b1b684b342bec5e331401599ce652900ec59db52940005",
-                "sha256:ba279aae162b20444881fc3ed4e4f934c1cf8620f3dab3b531480cf602c76b7f",
-                "sha256:bc4803779f0e4b06a2361f666e76f5c2e3715e8e379889d02251ec911befd149",
-                "sha256:bfe7085783cda55e53510482fa7b5efc761fad1abe4d653b32710eb548ebdd2d",
-                "sha256:c448b5c9e3df5448a362208b8d4b9ed85305528313fca1b479f14f9fe0d873b8",
-                "sha256:c90e73bdecb7b0d1cea65a08cb41e9d672ac6d7995603d6465ed4914b98b9ad7",
-                "sha256:d2b96123a453a2d7f3995ddb9f28d01fd112319a7a4d5ca99796a7ff43f02af5",
-                "sha256:d52f0a114b6a58305b11a5cdecd42b2e7f1ec77eb20e2b33969d702feafdd016",
-                "sha256:d530191aa9c66ab4f190be8ac8cc7cfd8f4f3217da379606f3dd4e3d83feba69",
-                "sha256:d683d230b5774816e7d784d7ed8444f2a40e7a450e5720d58af593cb0b94a212",
-                "sha256:db45eec1dfccdadb179b0f9ca616872c6f700d23945ecc8f21bb105d74b1c5fc",
-                "sha256:db8c2c5ace167fd25ab5dd732714c51d4633f58bac21fb0ff63b0349f62755a8",
-                "sha256:e2926b8abedf750c2ecf5035c07515770944acf02e1c46ab08f6348d24c5f94d",
-                "sha256:e627dee428a176ffb13697a2c4318d3f60b2ccdde3acdc9b3f304206ec130ccd",
-                "sha256:efe1c0adad110bf0ad7fb59f833880e489a61e39d699d37249bdf42f80590169"
+                "sha256:06ddd9c0249a0546997fdda5a30fbcb40f23926df0a874a60a8a185bc3a87d93",
+                "sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013",
+                "sha256:0f3736a5d34e091b0a611964c6262fd68ca4363df56185902528f0b75dbb9c1f",
+                "sha256:1127b16220f7bfb3f1049ed4a62d26d81970a723544e8252db0efde853268e21",
+                "sha256:172db976ae6327ed4728e2507daf8a4de73c7cc89796483e0a9198fd2e47b462",
+                "sha256:182eb9ac3f2b4874a1f41b78b87db20b66da6b9cdc32737fbbf4fea0c35b23fc",
+                "sha256:1bb1e77a9a311346294621be905ea8a2c30d3ad371fc15bb72e98bfcfae532df",
+                "sha256:1fd78b911aea9cec3b7e1e2622c8018d51c0d2bbcf8faaf53c2497eb114911c1",
+                "sha256:20d1a2a76bb4eb00e4d36b9699f9b7aba93271c9c29220ad4c6a9581a0320235",
+                "sha256:21b154aba06df42e4b96fc915512ab39595105f6c483991287021ed95776d934",
+                "sha256:2c2e58e45fe53fab81f85474e5d4d226eeab0f27b45aa062856c89389da2f0d9",
+                "sha256:2c3b2803e730dc2797a017335827e9da6da0e84c745ce0f552e66400abdfb9a1",
+                "sha256:3146b8e16fa60427e03884301bf8209221f5761ac754ee6b267642a2fd354c48",
+                "sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4",
+                "sha256:387065e420aed3c71b61af7e82c7b6bc1c592f7e3c7a66e9f78dd178699da4fe",
+                "sha256:3f04becd4fcda03c0160d0da9c8f0c246bc78f2f7af0feea1ec0930e7c93fa4a",
+                "sha256:4a42e1eff0ca9a7cb7dc9ecda41dfc7cbc17cb1d02117214be0561bd1134772b",
+                "sha256:4ea748802cc0de4de92ef8244dd84ffd793bd2e7be784cd8394d557a3c751e21",
+                "sha256:55416d7385774285b6e2a5feca0af9652f7f444a4fa3d29d8ab052fafef9d00d",
+                "sha256:5d0391fb4cfc171ce40437f67eb050a340fdbd0f9f49d6353a387f1b7f9dd4fa",
+                "sha256:63cdeaac4ae85a179a8d6bc09b77b564c096250d759eed343a89d91bce8b6367",
+                "sha256:72fcae5bcac3333a4cf3b8f34eec99cea1187acd55af723bcbd559adfdcb5535",
+                "sha256:7c4ed4e9f3b123aa403ab424430b426a1992e6f4c8fd3cb56ea520446e04d152",
+                "sha256:83957d349838a636e768251c7e9979e899a569794b44c3728eaebd11d848e58e",
+                "sha256:87ecc7c9a1a9f912e306997ffee020297ccb5ea388421fe62a2a02747e4d5539",
+                "sha256:8f69770f5ca1994cb32c38965e95f57504d3aea96b6c024624fdd5bb1aa494a1",
+                "sha256:8f6c930fd70d91ddee53194e93029e3ef2aabe26725aa3c2753df057e296b925",
+                "sha256:965ee3e782c7892befc25575fa171b521d33798132692df428a09efacaffe8d0",
+                "sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2",
+                "sha256:981b4df72c93e3bc04478153df516d385317628bd9c10be699c93c26ddcca8ab",
+                "sha256:aa784405f0c640940595fa0f14064d8e84aff0b0f762fa18393e2760a2cf5841",
+                "sha256:ae7863a1d8db6a014b6f2ff9c1582ab1aad55a6d25bac19710a8df68921b6e30",
+                "sha256:aeae2aa38395b18106e552833f2a50c27ea0000122bde421c31d11ed7e6f9c91",
+                "sha256:b2317d5ed777bf5a033e83d4f1389fd4ef045763141d8f10eb09a7035cee774c",
+                "sha256:be19931a8dcbe6ab464f3339966856996b12a00f9fe53f346ab3be872d03e257",
+                "sha256:be9824c1c874b73b96288c6d3de793bf7f3a597770205068c6163ea1f326e8b9",
+                "sha256:c0045f8f23a5fb30b2eb3b8a83664d8dc4fb58faddf8155d7109166adb9f2040",
+                "sha256:c86bd45d1659b1ae3d0ba1909326b03598affbc9ed71520e0ff8c31a993ad911",
+                "sha256:ca0f34363e2634deffd390a0fef1aa99168ae9ed2af01af4a1f5865e362f8623",
+                "sha256:d298c2815fa4891edd9abe5ad6e6cb4207104c7dd9fd13aea3fdebf6f9b91259",
+                "sha256:d2a3a6146fe9319926e1d477842ca2a63fe99af5ae690b1f5c11e6af074a6b5c",
+                "sha256:dfd393094cd82ceb9b40df4c77976015a314b267d498268a076e940fe7be6b79",
+                "sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5",
+                "sha256:ea3f5bc91d7d457da7d48c7a732beaf79d0c8131df3ab278e6bba6297e23c6c4",
+                "sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4",
+                "sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22",
+                "sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd",
+                "sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1",
+                "sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910",
+                "sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859",
+                "sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312"
             ],
             "index": "pypi",
-            "version": "==7.2.2"
+            "version": "==7.2.3"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
@@ -775,19 +767,19 @@
                 "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
             "version": "==1.1.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:892be14aa8efc01673b5ed6589dbccb95f9a8596f0507e232626155495c18105",
-                "sha256:bde48477b15fde2c7e5a0713cbe72721cb5a5ad32ee0b8f419907960b9d75536"
+                "sha256:3618c0da67adcc0506b015fd11ef7faf1b493f0b40d87728e19986b536890c37",
+                "sha256:f08a52314748335c6460fc8fe40cd5638b85001225db78c2aa01c8c0db83b318"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.10.7"
+            "version": "==3.11.0"
         },
         "flake8": {
             "hashes": [
                 "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
                 "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
             "index": "pypi",
@@ -943,43 +935,43 @@
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.1.2"
         },
         "mypy": {
             "hashes": [
-                "sha256:0a28a76785bf57655a8ea5eb0540a15b0e781c807b5aa798bd463779988fa1d5",
-                "sha256:19ba15f9627a5723e522d007fe708007bae52b93faab00f95d72f03e1afa9598",
-                "sha256:21b437be1c02712a605591e1ed1d858aba681757a1e55fe678a15c2244cd68a5",
-                "sha256:26cdd6a22b9b40b2fd71881a8a4f34b4d7914c679f154f43385ca878a8297389",
-                "sha256:2888ce4fe5aae5a673386fa232473014056967f3904f5abfcf6367b5af1f612a",
-                "sha256:2b0c373d071593deefbcdd87ec8db91ea13bd8f1328d44947e88beae21e8d5e9",
-                "sha256:315ac73cc1cce4771c27d426b7ea558fb4e2836f89cb0296cbe056894e3a1f78",
-                "sha256:39c7119335be05630611ee798cc982623b9e8f0cff04a0b48dfc26100e0b97af",
-                "sha256:4b398d8b1f4fba0e3c6463e02f8ad3346f71956b92287af22c9b12c3ec965a9f",
-                "sha256:4e4e8b362cdf99ba00c2b218036002bdcdf1e0de085cdb296a49df03fb31dfc4",
-                "sha256:59bbd71e5c58eed2e992ce6523180e03c221dcd92b52f0e792f291d67b15a71c",
-                "sha256:5b5f81b40d94c785f288948c16e1f2da37203c6006546c5d947aab6f90aefef2",
-                "sha256:5cb14ff9919b7df3538590fc4d4c49a0f84392237cbf5f7a816b4161c061829e",
-                "sha256:61bf08362e93b6b12fad3eab68c4ea903a077b87c90ac06c11e3d7a09b56b9c1",
-                "sha256:64cc3afb3e9e71a79d06e3ed24bb508a6d66f782aff7e56f628bf35ba2e0ba51",
-                "sha256:69b35d1dcb5707382810765ed34da9db47e7f95b3528334a3c999b0c90fe523f",
-                "sha256:9401e33814cec6aec8c03a9548e9385e0e228fc1b8b0a37b9ea21038e64cdd8a",
-                "sha256:a380c041db500e1410bb5b16b3c1c35e61e773a5c3517926b81dfdab7582be54",
-                "sha256:ae9ceae0f5b9059f33dbc62dea087e942c0ccab4b7a003719cb70f9b8abfa32f",
-                "sha256:b7c7b708fe9a871a96626d61912e3f4ddd365bf7f39128362bc50cbd74a634d5",
-                "sha256:c1c10fa12df1232c936830839e2e935d090fc9ee315744ac33b8a32216b93707",
-                "sha256:ce61663faf7a8e5ec6f456857bfbcec2901fbdb3ad958b778403f63b9e606a1b",
-                "sha256:d64c28e03ce40d5303450f547e07418c64c241669ab20610f273c9e6290b4b0b",
-                "sha256:d809f88734f44a0d44959d795b1e6f64b2bbe0ea4d9cc4776aa588bb4229fc1c",
-                "sha256:dbb19c9f662e41e474e0cff502b7064a7edc6764f5262b6cd91d698163196799",
-                "sha256:ef6a01e563ec6a4940784c574d33f6ac1943864634517984471642908b30b6f7"
+                "sha256:023fe9e618182ca6317ae89833ba422c411469156b690fde6a315ad10695a521",
+                "sha256:031fc69c9a7e12bcc5660b74122ed84b3f1c505e762cc4296884096c6d8ee140",
+                "sha256:2de7babe398cb7a85ac7f1fd5c42f396c215ab3eff731b4d761d68d0f6a80f48",
+                "sha256:2e93a8a553e0394b26c4ca683923b85a69f7ccdc0139e6acd1354cc884fe0128",
+                "sha256:390bc685ec209ada4e9d35068ac6988c60160b2b703072d2850457b62499e336",
+                "sha256:3a2d219775a120581a0ae8ca392b31f238d452729adbcb6892fa89688cb8306a",
+                "sha256:3efde4af6f2d3ccf58ae825495dbb8d74abd6d176ee686ce2ab19bd025273f41",
+                "sha256:4a99fe1768925e4a139aace8f3fb66db3576ee1c30b9c0f70f744ead7e329c9f",
+                "sha256:4b41412df69ec06ab141808d12e0bf2823717b1c363bd77b4c0820feaa37249e",
+                "sha256:4c8d8c6b80aa4a1689f2a179d31d86ae1367ea4a12855cc13aa3ba24bb36b2d8",
+                "sha256:4d19f1a239d59f10fdc31263d48b7937c585810288376671eaf75380b074f238",
+                "sha256:4e4a682b3f2489d218751981639cffc4e281d548f9d517addfd5a2917ac78119",
+                "sha256:695c45cea7e8abb6f088a34a6034b1d273122e5530aeebb9c09626cea6dca4cb",
+                "sha256:701189408b460a2ff42b984e6bd45c3f41f0ac9f5f58b8873bbedc511900086d",
+                "sha256:70894c5345bea98321a2fe84df35f43ee7bb0feec117a71420c60459fc3e1eed",
+                "sha256:8293a216e902ac12779eb7a08f2bc39ec6c878d7c6025aa59464e0c4c16f7eb9",
+                "sha256:8d26b513225ffd3eacece727f4387bdce6469192ef029ca9dd469940158bc89e",
+                "sha256:a197ad3a774f8e74f21e428f0de7f60ad26a8d23437b69638aac2764d1e06a6a",
+                "sha256:bea55fc25b96c53affab852ad94bf111a3083bc1d8b0c76a61dd101d8a388cf5",
+                "sha256:c9a084bce1061e55cdc0493a2ad890375af359c766b8ac311ac8120d3a472950",
+                "sha256:d0e9464a0af6715852267bf29c9553e4555b61f5904a4fc538547a4d67617937",
+                "sha256:d8e9187bfcd5ffedbe87403195e1fc340189a68463903c39e2b63307c9fa0394",
+                "sha256:eaeaa0888b7f3ccb7bcd40b50497ca30923dba14f385bde4af78fac713d6d6f6",
+                "sha256:f46af8d162f3d470d8ffc997aaf7a269996d205f9d746124a179d3abe05ac602",
+                "sha256:f70a40410d774ae23fcb4afbbeca652905a04de7948eaf0b1789c8d1426b72d1",
+                "sha256:fe91be1c51c90e2afe6827601ca14353bbf3953f343c2129fa1e247d55fd95ba"
             ],
             "index": "pypi",
-            "version": "==1.1.1"
+            "version": "==1.2.0"
         },
         "mypy-extensions": {
             "hashes": [
                 "sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d",
                 "sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782"
             ],
             "markers": "python_version >= '3.5'",
@@ -991,19 +983,19 @@
                 "sha256:e0e7f7dfb85fc5394c6fe1e8fa98131a2473e04311a45afb6508f7cf1836fa2b"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
             "version": "==1.7.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.1'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "pathspec": {
             "hashes": [
                 "sha256:2798de800fa92780e33acca925945e9a19a133b715067cf165b8866c15a31687",
                 "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
             ],
             "markers": "python_version >= '3.7'",
@@ -1071,19 +1063,19 @@
                 "sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==3.0.1"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094",
+                "sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.0"
         },
         "pyproject-api": {
             "hashes": [
                 "sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9",
                 "sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43"
             ],
             "markers": "python_version >= '3.7'",
@@ -1095,19 +1087,19 @@
                 "sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
         "pytest": {
             "hashes": [
-                "sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e",
-                "sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4"
+                "sha256:58ecc27ebf0ea643ebfdf7fb1249335da761a00c9f955bcd922349bcb68ee57d",
+                "sha256:933051fa1bfbd38a21e73c3960cebdad4cf59483ddba7696c48509727e17f201"
             ],
             "index": "pypi",
-            "version": "==7.2.2"
+            "version": "==7.3.0"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
@@ -1157,19 +1149,19 @@
                 "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
             ],
             "index": "pypi",
             "version": "==2.28.2"
         },
         "rich": {
             "hashes": [
-                "sha256:540c7d6d26a1178e8e8b37e9ba44573a3cd1464ff6348b99ee7061b95d1c6333",
-                "sha256:dc84400a9d842b3a9c5ff74addd8eb798d155f36c1c91303888e0a66850d2a15"
+                "sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a",
+                "sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13f74cf454ccb2f490708b"
             ],
             "index": "pypi",
-            "version": "==13.3.3"
+            "version": "==13.3.4"
         },
         "setuptools": {
             "hashes": [
                 "sha256:257de92a9d50a60b8e22abfcbb771571fde0dbf3ec234463212027a4eeecbe9a",
                 "sha256:e728ca814a823bf7bf60162daf9db95b93d532948c4c0bea762ce62f60189078"
             ],
             "markers": "python_version >= '3.7'",
@@ -1283,19 +1275,19 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version >= '3.1'",
             "version": "==2.0.1"
         },
         "tox": {
             "hashes": [
-                "sha256:6fa4dbd933d0e335b5392c81e9cd467630119b3669705dbad47814a93b6c9586",
-                "sha256:cd88e41aef9c71f0ba02b6d7939f102760b192b63458fbe04dbbaed82f7bf5f5"
+                "sha256:740f5209d0dec19451b951ee5b1cce4a207acdc7357af84dbc8ec35bcf2c454e",
+                "sha256:d4be558809d86fad13f4553976b0500352630a8fbfa39ea4b1ce3bd945ba680b"
             ],
             "index": "pypi",
-            "version": "==4.4.11"
+            "version": "==4.4.12"
         },
         "types-requests": {
             "hashes": [
                 "sha256:0d580652ce903f643f8c3b494dd01d29367ea57cea0c7ad7f65cf3169092edb0",
                 "sha256:cc1aba862575019306b2ed134eb1ea994cab1c887a22e18d3383e6dd42e9789b"
             ],
             "index": "pypi",
```

### Comparing `repository_service_tuf-0.1.0a1/README.rst` & `repository_service_tuf-0.1.1a2/README.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/id_ed25519` & `repository_service_tuf-0.1.1a2/id_ed25519`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/pyproject.toml` & `repository_service_tuf-0.1.1a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/requirements-dev.txt` & `repository_service_tuf-0.1.1a2/requirements-dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,61 +1,60 @@
 -i https://pypi.org/simple
 alabaster==0.7.13 ; python_version >= '3.6'
-attrs==22.2.0 ; python_version >= '3.6'
 babel==2.12.1 ; python_version >= '3.7'
 bandit==1.7.5
 black==23.3.0
 build==0.10.0
 cachetools==5.3.0 ; python_version ~= '3.7'
 certifi==2022.12.7 ; python_version >= '3.6'
 cfgv==3.3.1 ; python_full_version >= '3.6.1'
 chardet==5.1.0 ; python_version >= '3.7'
 charset-normalizer==3.1.0 ; python_full_version >= '3.7.0'
 click==8.1.3
 colorama==0.4.6 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
-coverage==7.2.2
+coverage==7.2.3
 distlib==0.3.6
 docutils==0.18.1 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
 editables==0.3 ; python_version >= '3.1'
 exceptiongroup==1.1.1 ; python_version < '3.11'
-filelock==3.10.7 ; python_version >= '3.7'
+filelock==3.11.0 ; python_version >= '3.7'
 flake8==6.0.0
 gitdb==4.0.10 ; python_version >= '3.7'
 gitpython==3.1.31 ; python_version >= '3.7'
 hatchling==0.22.0
 identify==2.5.22 ; python_version >= '3.7'
 idna==3.4 ; python_version >= '3.5'
 imagesize==1.4.1 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 iniconfig==2.0.0 ; python_version >= '3.7'
 isort==5.12.0
 jinja2==3.1.2 ; python_version >= '3.7'
 markdown-it-py==2.2.0 ; python_version >= '3.7'
 markupsafe==2.1.2 ; python_version >= '3.7'
 mccabe==0.7.0 ; python_version >= '3.6'
 mdurl==0.1.2 ; python_version >= '3.7'
-mypy==1.1.1
+mypy==1.2.0
 mypy-extensions==1.0.0 ; python_version >= '3.5'
 nodeenv==1.7.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
-packaging==23.0 ; python_version >= '3.1'
+packaging==23.1 ; python_version >= '3.1'
 pathspec==0.11.1 ; python_version >= '3.7'
 pbr==5.11.1 ; python_version >= '2.6'
 pip==23.0.1
 platformdirs==3.2.0 ; python_version >= '3.7'
 pluggy==1.0.0 ; python_version >= '3.1'
 pre-commit==3.2.2
 pretend==1.0.9
 pycodestyle==2.10.0 ; python_version >= '3.6'
 pyflakes==3.0.1 ; python_version >= '3.6'
-pygments==2.14.0 ; python_version >= '3.6'
+pygments==2.15.0 ; python_version >= '3.7'
 pyproject-api==1.5.1 ; python_version >= '3.7'
 pyproject-hooks==1.0.0 ; python_version >= '3.7'
-pytest==7.2.2
+pytest==7.3.0
 pyyaml==6.0 ; python_version >= '3.6'
 requests==2.28.2
-rich==13.3.3
+rich==13.3.4
 setuptools==67.6.1 ; python_version >= '3.7'
 smmap==5.0.0 ; python_version >= '3.6'
 snowballstemmer==2.2.0
 sphinx==6.1.3
 sphinx-rtd-theme==1.2.0
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
@@ -63,15 +62,15 @@
 sphinxcontrib-jquery==4.1 ; python_version >= '3.1'
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-plantuml==0.25
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 stevedore==5.0.0 ; python_version >= '3.8'
 tomli==2.0.1 ; python_version >= '3.1'
-tox==4.4.11
+tox==4.4.12
 types-requests==2.28.11.17
 types-urllib3==1.26.25.10
 typing-extensions==4.5.0 ; python_version >= '3.7'
 urllib3==1.26.15 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
 virtualenv==20.21.0 ; python_version >= '3.7'
 cffi==1.15.1
 configobj==5.0.8
```

### Comparing `repository_service_tuf-0.1.0a1/requirements.txt` & `repository_service_tuf-0.1.1a2/requirements.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 greenlet==2.0.2 ; platform_machine == 'aarch64' or (platform_machine == 'ppc64le' or (platform_machine == 'x86_64' or (platform_machine == 'amd64' or (platform_machine == 'AMD64' or (platform_machine == 'win32' or platform_machine == 'WIN32')))))
 idna==3.4 ; python_version >= '3.5'
 isort==5.12.0
 markdown-it-py==2.2.0 ; python_version >= '3.7'
 mdurl==0.1.2 ; python_version >= '3.7'
 psycopg2==2.9.6
 pycparser==2.21
-pygments==2.14.0 ; python_version >= '3.6'
+pygments==2.15.0 ; python_version >= '3.7'
 pynacl==1.5.0
 requests==2.28.2
-rich==13.3.3
+rich==13.3.4
 rich-click==1.6.1
 securesystemslib[crypto]==0.27.0
 six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 sqlalchemy==2.0.9
 tuf==2.0.0
 typing-extensions==4.5.0 ; python_version >= '3.7'
 urllib3==1.26.15 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
```

### Comparing `repository_service_tuf-0.1.0a1/tox.ini` & `repository_service_tuf-0.1.1a2/tox.ini`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/.github/ISSUE_TEMPLATE/bug.yml` & `repository_service_tuf-0.1.1a2/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/.github/ISSUE_TEMPLATE/other.yml` & `repository_service_tuf-0.1.1a2/.github/ISSUE_TEMPLATE/other.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/.github/ISSUE_TEMPLATE/task.yml` & `repository_service_tuf-0.1.1a2/.github/ISSUE_TEMPLATE/task.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/.github/PULL_REQUEST_TEMPLATE/pr.yml` & `repository_service_tuf-0.1.1a2/.github/PULL_REQUEST_TEMPLATE/pr.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/.github/workflows/cd.yml` & `repository_service_tuf-0.1.1a2/.github/workflows/cd.yml`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     name: Build
     runs-on: ubuntu-latest
     needs: functional-latest
     outputs:
       release_id: ${{ steps.gh-release.outputs.id }}
     steps:
       - name: Checkout release tag
-        uses: actions/checkout@8f4b7f84864484a7bf31766abe9204da3cbe65b3
+        uses: actions/checkout@8e5e7e5ab8b370d6c329ec480221332ada57f0ab
         with:
           ref: ${{ github.event.workflow_run.head_branch }}
 
       - name: Set up Python
         uses: actions/setup-python@d27e3f3d7c64b4bbf8e4abfb9b63b83e846e0435
         with:
           python-version: '3.x'
@@ -67,15 +67,15 @@
       - name: Fetch build artifacts
         uses: actions/download-artifact@9bc31d5ccc31df68ecc42ccf4149144866c47d8a
         with:
           name: build-artifacts
           path: dist
 
       - name: Finalize GitHub release
-        uses: actions/github-script@98814c53be79b1d30f795b907e553d8679345975
+        uses: actions/github-script@d7906e4ad0b1822421a7e6a35d5ca353c962f410
         with:
           script: |
             await github.rest.repos.updateRelease({
               owner: context.repo.owner,
               repo: context.repo.repo,
               release_id: '${{ needs.build.outputs.release_id }}',
               name: '${{ github.ref_name }}',
```

### Comparing `repository_service_tuf-0.1.0a1/.github/workflows/update-python-deps.yml` & `repository_service_tuf-0.1.1a2/.github/workflows/update-python-deps.yml`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 jobs:
   update-dep:
     runs-on: ubuntu-latest
     strategy:
       matrix:
         python-versions: ["3.10"]
     steps:
-      - uses: actions/checkout@8f4b7f84864484a7bf31766abe9204da3cbe65b3
+      - uses: actions/checkout@8e5e7e5ab8b370d6c329ec480221332ada57f0ab
       - uses: actions/setup-python@d27e3f3d7c64b4bbf8e4abfb9b63b83e846e0435
         with:
           python-version: ${{ matrix.python-versions }}
       - name: Install prerequisites
         run: |
           pip install tox pipenv
       - name: Update dependencies
```

### Comparing `repository_service_tuf-0.1.0a1/docs/Makefile` & `repository_service_tuf-0.1.1a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/docs/make.bat` & `repository_service_tuf-0.1.1a2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/docs/diagrams/repository-service-tuf-cli-C1.puml` & `repository_service_tuf-0.1.1a2/docs/diagrams/repository-service-tuf-cli-C1.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/docs/diagrams/repository-service-tuf-cli-C2.puml` & `repository_service_tuf-0.1.1a2/docs/diagrams/repository-service-tuf-cli-C2.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/docs/diagrams/repository-service-tuf-cli-C3.puml` & `repository_service_tuf-0.1.1a2/docs/diagrams/repository-service-tuf-cli-C3.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/docs/source/conf.py` & `repository_service_tuf-0.1.1a2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/docs/source/_static/repository-service-tuf-cli-C1.png` & `repository_service_tuf-0.1.1a2/docs/source/_static/repository-service-tuf-cli-C1.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/docs/source/_static/repository-service-tuf-cli-C2.png` & `repository_service_tuf-0.1.1a2/docs/source/_static/repository-service-tuf-cli-C2.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/docs/source/_static/repository-service-tuf-cli-C3.png` & `repository_service_tuf-0.1.1a2/docs/source/_static/repository-service-tuf-cli-C3.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/docs/source/devel/design.rst` & `repository_service_tuf-0.1.1a2/docs/source/devel/design.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/docs/source/devel/repository_service_tuf.cli.admin.rst` & `repository_service_tuf-0.1.1a2/docs/source/devel/repository_service_tuf.cli.admin.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/docs/source/devel/repository_service_tuf.helpers.rst` & `repository_service_tuf-0.1.1a2/docs/source/devel/repository_service_tuf.helpers.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/docs/source/guide/index.rst` & `repository_service_tuf-0.1.1a2/docs/source/guide/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 
     Usage: rstuf [OPTIONS] COMMAND [ARGS]...
 
     Repository Service for TUF Command Line Interface (CLI).
 
     ╭─ Options ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ --config   -c  TEXT  Repository Service for TUF config file                                                                      │
+    │ --no-auth            Skips the use of RSTUF built-in authentication.                                                             │
     │ --version            Show the version and exit.                                                                                  │
     │ --help     -h        Show this message and exit.                                                                                 │
     ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
     ╭─ Commands ───────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
     │ admin                      Administrative Commands                                                                               │
     │ key                        Cryptographic Key Commands                                                                            │
     ╰──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
```

### Comparing `repository_service_tuf-0.1.0a1/repository_service_tuf/constants.py` & `repository_service_tuf-0.1.1a2/repository_service_tuf/constants.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/repository_service_tuf/cli/admin/ceremony.py` & `repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/ceremony.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,25 @@
 # Ceremony
 #
 import json
 import os
 from typing import Any, Dict, Generator, Optional
 
 from rich import box, markdown, prompt, table  # type: ignore
-from rich.console import Console  # type: ignore
 from securesystemslib.exceptions import (  # type: ignore
     CryptoError,
     Error,
     FormatError,
     StorageError,
 )
 from securesystemslib.interface import (  # type: ignore
     import_privatekey_from_file,
 )
 
-from repository_service_tuf.cli import click
+from repository_service_tuf.cli import click, console
 from repository_service_tuf.cli.admin import admin
 from repository_service_tuf.constants import KeyType
 from repository_service_tuf.helpers.api_client import (
     URL,
     LazySettings,
     Methods,
     bootstrap_status,
@@ -229,16 +228,14 @@
  https://example.com/downloads/productA/productA-v1.0.tar
 - "1.bins-1.json" will be responsible for file:
  https://example.com/downloads/productB/productB-v1.0.tar
 - "1.bins-5.json" will be responsible for file:
  https://example.com/downloads/productB/updates/servicepack-1.tar
 """
 
-console = Console()
-
 
 # Define all initial settings
 setup = BootstrapSetup(
     expiration={
         Roles.ROOT: 365,
         Roles.TARGETS: 365,
         Roles.SNAPSHOT: 1,
@@ -686,27 +683,38 @@
         "Upload existent payload 'file'. Requires '-b/--bootstrap'. "
         "Optional '-f/--file' to use non default file."
     ),
     required=False,
     is_flag=True,
 )
 @click.option(
+    "--upload-server",
+    help="[when using '--no-auth'] Upload RSTUF API Server address. ",
+    required=False,
+    hidden=True,
+)
+@click.option(
     "-s",
     "--save",
     help=(
         "Save a copy of the metadata locally. This option saves the JSON "
         "metadata files in the 'metadata' folder in the current directory."
     ),
     default=False,
     show_default=True,
     is_flag=True,
 )
 @click.pass_context
 def ceremony(
-    context: Any, bootstrap: bool, file: str, upload: bool, save: bool
+    context: Any,
+    bootstrap: bool,
+    file: str,
+    upload: bool,
+    save: bool,
+    upload_server: str,
 ) -> None:
     """
     Start a new Metadata Ceremony.
     """
     settings = context.obj["settings"]
     # option save: creates the folder
     if save is True:
@@ -717,14 +725,22 @@
 
     # option upload: it requires -b/--bootstrap
     if upload is True and bootstrap is False:
         raise click.ClickException("Requires '-b/--bootstrap' option.")
 
     # option bootstrap: checks if the server accepts it beforehand
     if bootstrap:
+        if settings.AUTH is False and upload_server is None:
+            raise click.ClickException(
+                "Requires '--upload-server' when using '--no-auth'. "
+                "Example: --upload-server https://rstuf-api.example.com"
+            )
+        elif upload_server:
+            settings.SERVER = upload_server
+
         bs_status = bootstrap_status(settings)
         if bs_status.get("data", {}).get("bootstrap") is True:
             raise click.ClickException(f"{bs_status.get('message')}")
 
     # option bootstrap + upload: bootstrap payload is available, skips ceremony
     if bootstrap is True and upload is True:
         bootstrap_payload = _load_bootstrap_payload(file)
```

### Comparing `repository_service_tuf-0.1.0a1/repository_service_tuf/cli/admin/import_targets.py` & `repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/import_targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import json
 import os
 from datetime import datetime
 from typing import Any, Dict, List
 
-from rich.console import Console
 from tuf.api.metadata import Delegations, SuccinctRoles, Targets
 
-from repository_service_tuf.cli import click
+from repository_service_tuf.cli import click, console
 from repository_service_tuf.cli.admin import admin
 from repository_service_tuf.helpers.api_client import (
     Methods,
     bootstrap_status,
     publish_targets,
     request_server,
     task_status,
 )
 from repository_service_tuf.helpers.tuf import Metadata
 
-console = Console()
-
 
 def _check_csv_files(csv_files: List[str]):
     not_found_csv_files: List[str] = []
     for csv_file in csv_files:
         if not os.path.isfile(csv_file):
             not_found_csv_files.append(csv_file)
```

### Comparing `repository_service_tuf-0.1.0a1/repository_service_tuf/cli/admin/login.py` & `repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/login.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,24 @@
 #
 # SPDX-License-Identifier: MIT
 
 from typing import Dict
 
 from dynaconf import loaders
 from rich import markdown, prompt  # type: ignore
-from rich.console import Console  # type: ignore
 
-from repository_service_tuf.cli import click
+from repository_service_tuf.cli import click, console
 from repository_service_tuf.cli.admin import admin
 from repository_service_tuf.helpers.api_client import (
     URL,
     Methods,
     is_logged,
     request_server,
 )
 
-console = Console()
-
 
 def _login(server: str, data: Dict[str, str]):
     token_response = request_server(
         server, URL.token.value, Methods.post, data=data
     )
     if token_response.status_code != 200:
         raise click.ClickException(token_response.json()["detail"])
@@ -113,25 +110,30 @@
 )
 @click.pass_context
 def login(context, force, server_, user_, password_, expires_):
     """
     Login to Repository Service for TUF (API).
     """
     settings = context.obj.get("settings")
-    server = settings.get("SERVER")
-    token = settings.get("TOKEN")
 
-    if force is False and server is not None and token is not None:
-        response = is_logged(server, token)
+    if settings.get("AUTH") is False:
+        return None
+
+    elif (
+        force is False
+        and settings.get("SERVER") is not None
+        and settings.get("TOKEN") is not None
+    ):
+        response = is_logged(settings)
         if response.state is False:
             _run_login(context, server_, user_, password_, expires_)
 
         else:
             data = response.data
             if response.data.get("expired") is False:
                 console.print(
-                    f"Already logged to {server}. "
+                    f"Already logged to {settings.get('SERVER')}. "
                     f"Valid until '{data['expiration']}'"
                 )
 
     else:
         _run_login(context, server_, user_, password_, expires_)
```

### Comparing `repository_service_tuf-0.1.0a1/repository_service_tuf/cli/admin/token.py` & `repository_service_tuf-0.1.1a2/repository_service_tuf/cli/admin/token.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 # SPDX-FileCopyrightText: 2022-2023 VMware Inc
 #
 # SPDX-License-Identifier: MIT
-
-import click
-from rich.console import Console  # type: ignore
-
+from repository_service_tuf.cli import click, console
 from repository_service_tuf.cli.admin import admin
 from repository_service_tuf.helpers.api_client import (
     URL,
     Methods,
     is_logged,
     request_server,
 )
 
-console = Console()
-
 
 @admin.group()
 @click.pass_context
 def token(context):
     """
     Token Management.
     """
+    settings = context.obj.get("settings")
+    if settings.get("AUTH") is False:
+        console.print("[INFO] admin token is disabled with `--no-auth`")
+        raise click.Abort()
 
 
 @token.command()
 @click.option(
     "-e",
     "--expires",
     "expires",
```

### Comparing `repository_service_tuf-0.1.0a1/repository_service_tuf/cli/key/generate_key.py` & `repository_service_tuf-0.1.1a2/repository_service_tuf/cli/key/generate_key.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/repository_service_tuf/helpers/api_client.py` & `repository_service_tuf-0.1.1a2/repository_service_tuf/helpers/api_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,19 +5,16 @@
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Dict, Optional
 
 import requests
 from dynaconf import LazySettings
 from requests.exceptions import ConnectionError
-from rich.console import Console
 
-from repository_service_tuf.cli import click
-
-console = Console()
+from repository_service_tuf.cli import click, console
 
 
 class URL(Enum):
     token = "api/v1/token/"  # nosec bandit: not hard coded password.
     bootstrap = "api/v1/bootstrap/"
     task = "api/v1/task/?task_id="
     publish_targets = "api/v1/targets/publish/"
@@ -58,15 +55,20 @@
 
     except ConnectionError:
         raise click.ClickException(f"Failed to connect to {server}")
 
     return response
 
 
-def is_logged(server: str, token: str):
+def is_logged(settings: LazySettings):
+    if settings.get("AUTH") is False:
+        return None
+
+    token = settings.get("TOKEN")
+    server = settings.get("SERVER")
     headers = {"Authorization": f"Bearer {token}"}
     url = f"{URL.token.value}?token={token}"
     response = request_server(server, url, Methods.get, headers=headers)
     if response.status_code == 401 or response.status_code == 403:
         return Login(state=False)
 
     elif response.status_code == 200:
@@ -77,18 +79,21 @@
     else:
         raise click.ClickException(
             f"Error {response.status_code} {response.text}"
         )
 
 
 def get_headers(settings: LazySettings) -> Dict[str, str]:
+    if settings.get("AUTH") is False:
+        return {}
+
     server = settings.get("SERVER")
     token = settings.get("TOKEN")
     if server and token:
-        token_access_check = is_logged(server, token)
+        token_access_check = is_logged(settings)
         if token_access_check.state is False:
             raise click.ClickException(
                 f"{str(token_access_check.data)}"
                 "\n\nTry re-login: 'rstuf admin login'"
             )
 
         expired_admin = token_access_check.data.get("expired")
```

### Comparing `repository_service_tuf-0.1.0a1/repository_service_tuf/helpers/tuf.py` & `repository_service_tuf-0.1.1a2/repository_service_tuf/helpers/tuf.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/tests/2.targets.json` & `repository_service_tuf-0.1.1a2/tests/2.targets.json`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/tests/conftest.py` & `repository_service_tuf-0.1.1a2/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 )
 
 
 @pytest.fixture
 def test_context() -> Dict[str, Any]:
     setting_file = os.path.join(TemporaryDirectory().name, "test_settings.ini")
     test_settings = Dynaconf(settings_files=[setting_file])
+    test_settings.AUTH = True
     return {"settings": test_settings, "config": setting_file}
 
 
 @pytest.fixture
 def client() -> CliRunner:
     runner = CliRunner()
     return runner
```

### Comparing `repository_service_tuf-0.1.0a1/tests/test_tuf_repository_service.py` & `repository_service_tuf-0.1.1a2/tests/test_tuf_repository_service.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/tests/files/JanisJoplin.key` & `repository_service_tuf-0.1.1a2/tests/files/JanisJoplin.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/tests/files/JimiHendrix.key` & `repository_service_tuf-0.1.1a2/tests/files/JimiHendrix.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/tests/files/online-rsa.key` & `repository_service_tuf-0.1.1a2/tests/files/online-rsa.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/tests/files/online-rsa.pub` & `repository_service_tuf-0.1.1a2/tests/files/online-rsa.pub`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/tests/files/online.key` & `repository_service_tuf-0.1.1a2/tests/files/online.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/tests/files/keystorage/JanisJoplin.key` & `repository_service_tuf-0.1.1a2/tests/files/keystorage/JanisJoplin.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/tests/files/keystorage/JimiHendrix.key` & `repository_service_tuf-0.1.1a2/tests/files/keystorage/JimiHendrix.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/tests/files/keystorage/online-rsa.key` & `repository_service_tuf-0.1.1a2/tests/files/keystorage/online-rsa.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/tests/files/keystorage/online-rsa.pub` & `repository_service_tuf-0.1.1a2/tests/files/keystorage/online-rsa.pub`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/tests/files/keystorage/online.key` & `repository_service_tuf-0.1.1a2/tests/files/keystorage/online.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/tests/unit/cli/admin/test_ceremony.py` & `repository_service_tuf-0.1.1a2/tests/unit/cli/admin/test_ceremony.py`

 * *Files 3% similar despite different names*

```diff
@@ -704,14 +704,15 @@
             lambda *a: {"k": "v"}
         )
         ceremony._send_bootstrap = pretend.call_recorder(
             lambda *a: "fake_task_id"
         )
         ceremony.task_status = pretend.call_recorder(lambda *a: None)
 
+        test_context["settings"].SERVER = "http://server"
         test_result = client.invoke(
             ceremony.ceremony,
             ["--bootstrap", "--upload"],
             input=None,
             obj=test_context,
         )
 
@@ -730,14 +731,77 @@
             pretend.call(test_context["settings"], {"k": "v"})
         ]
         assert ceremony.task_status.calls == [
             pretend.call(
                 "fake_task_id", test_context["settings"], "Bootstrap status: "
             )
         ]
+        # test regression https://github.com/vmware/repository-service-tuf-cli/pull/259  # noqa
+        assert test_context["settings"].SERVER is not None
+
+    def test_ceremony_option_bootstrap_upload_no_auth(
+        self, client, test_context
+    ):
+        ceremony.bootstrap_status = pretend.call_recorder(
+            lambda *a: {"data": {"bootstrap": False}}
+        )
+        ceremony._load_bootstrap_payload = pretend.call_recorder(
+            lambda *a: {"k": "v"}
+        )
+        ceremony._send_bootstrap = pretend.call_recorder(
+            lambda *a: "fake_task_id"
+        )
+        ceremony.task_status = pretend.call_recorder(lambda *a: None)
+
+        test_context["settings"].AUTH = False
+
+        test_result = client.invoke(
+            ceremony.ceremony,
+            ["--bootstrap", "--upload", "--upload-server", "http://rstuf"],
+            input=None,
+            obj=test_context,
+        )
+
+        assert test_result.exit_code == 0, test_result.output
+        assert (
+            "Bootstrap completed using `payload.json`. 🔐 🎉"
+            in test_result.output
+        )
+        assert ceremony.bootstrap_status.calls == [
+            pretend.call(test_context["settings"])
+        ]
+        assert ceremony._load_bootstrap_payload.calls == [
+            pretend.call("payload.json")
+        ]
+        assert ceremony._send_bootstrap.calls == [
+            pretend.call(test_context["settings"], {"k": "v"})
+        ]
+        assert ceremony.task_status.calls == [
+            pretend.call(
+                "fake_task_id", test_context["settings"], "Bootstrap status: "
+            )
+        ]
+
+    def test_ceremony_option_bootstrap_upload_no_auth_missing_upload_server(
+        self, client, test_context
+    ):
+        test_context["settings"].AUTH = False
+
+        test_result = client.invoke(
+            ceremony.ceremony,
+            ["--bootstrap", "--upload"],
+            input=None,
+            obj=test_context,
+        )
+
+        assert test_result.exit_code == 1, test_result.output
+        assert (
+            "Requires '--upload-server' when using '--no-auth'"
+            in test_result.output
+        )
 
     def test_ceremony_option_upload_missing_bootstrap(
         self, client, test_context, test_inputs, test_setup
     ):
         ceremony.setup = test_setup
         input_step1, input_step2, input_step3, input_step4 = test_inputs
```

### Comparing `repository_service_tuf-0.1.0a1/tests/unit/cli/admin/test_import_targets.py` & `repository_service_tuf-0.1.1a2/tests/unit/cli/admin/test_import_targets.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/tests/unit/cli/admin/test_login.py` & `repository_service_tuf-0.1.1a2/tests/unit/cli/admin/test_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,35 @@
         assert "Login successful." in test_result.output
         assert login.loaders.write.calls == [
             pretend.call(
                 test_context["config"], test_context["settings"].to_dict()
             )
         ]
 
+    def test_login_no_auth(self, client, test_context):
+        steps = [
+            "http://test-rstuf",
+            "admin",
+            "pass",
+            "1",
+        ]
+        login._login = pretend.call_recorder(
+            lambda *a: {"access_token": "fake-token"}
+        )
+        test_context["settings"].AUTH = False
+        login.loaders = pretend.stub(
+            write=pretend.call_recorder(lambda *a: None)
+        )
+        test_result = client.invoke(
+            login.login, input="\n".join(steps), obj=test_context
+        )
+
+        assert test_result.exit_code == 0
+        assert login.loaders.write.calls == []
+
     def test_login_force(self, client, test_context):
         # simulate the settings file
         test_context["settings"].SERVER = "fake-server"
         test_context["settings"].TOKEN = "test-token"
 
         steps = [
             "http://test-rstuf",
@@ -138,15 +159,15 @@
         assert "Login successful." in test_result.output
         assert login.loaders.write.calls == [
             pretend.call(
                 test_context["config"], test_context["settings"].to_dict()
             )
         ]
         assert login.is_logged.calls == [
-            pretend.call(test_context["settings"].SERVER, "fake-token")
+            pretend.call(test_context["settings"])
         ]
 
     def test_login_already_logged(self, client, test_context):
         # simulate the settings file with invalid/expired token
         test_context["settings"].SERVER = "http://test-rstuf"
         test_context["settings"].TOKEN = "fake-token"
 
@@ -176,15 +197,15 @@
 
         assert test_result.exit_code == 0
         assert (
             "Already logged to http://test-rstuf."
             " Valid until '2022-08-23T09:10:14'" in test_result.output
         )
         assert login.is_logged.calls == [
-            pretend.call(test_context["settings"].SERVER, "fake-token")
+            pretend.call(test_context["settings"])
         ]
 
     def test_login_missing_http_protocol(self, client, test_context):
         steps = [
             "test-rstuf",
             "http://test-rstuf",
             "admin",
```

### Comparing `repository_service_tuf-0.1.0a1/tests/unit/cli/key/test_generate_key.py` & `repository_service_tuf-0.1.1a2/tests/unit/cli/key/test_generate_key.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/tests/unit/helpers/test_api_client.py` & `repository_service_tuf-0.1.1a2/tests/unit/helpers/test_api_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -65,153 +65,175 @@
         with pytest.raises(api_client.click.exceptions.ClickException) as err:
             api_client.request_server(
                 "http://server", "url", api_client.Methods.post, {"k": "v"}
             )
 
         assert "Failed to connect to http://server" in str(err.value)
 
-    def test_is_logged(self):
+    def test_is_logged(self, test_context):
         fake_response = pretend.stub(
             status_code=200,
             json=pretend.call_recorder(lambda: {"data": {"expired": False}}),
         )
         api_client.request_server = pretend.call_recorder(
             lambda *a, **kw: fake_response
         )
 
-        result = api_client.is_logged("http://server", "fake_token")
+        test_context["settings"].SERVER = "http://server"
+        test_context["settings"].TOKEN = "fake_token"
+        result = api_client.is_logged(test_context["settings"])
         assert result == api_client.Login(state=True, data={"expired": False})
         assert api_client.request_server.calls == [
             pretend.call(
                 "http://server",
                 "api/v1/token/?token=fake_token",
                 api_client.Methods.get,
                 headers={"Authorization": "Bearer fake_token"},
             )
         ]
 
-    def test_is_logged_401(self):
+    def test_is_logged_no_auth(self, test_context):
+        test_context["settings"].SERVER = "http://server"
+        test_context["settings"].TOKEN = "fake_token"
+        test_context["settings"].AUTH = False
+        result = api_client.is_logged(test_context["settings"])
+        assert result is None
+
+    def test_is_logged_401(self, test_context):
         fake_response = pretend.stub(
             status_code=401,
         )
         api_client.request_server = pretend.call_recorder(
             lambda *a, **kw: fake_response
         )
 
-        result = api_client.is_logged("http://server", "fake_token")
+        test_context["settings"].SERVER = "http://server"
+        test_context["settings"].TOKEN = "fake_token"
+        result = api_client.is_logged(test_context["settings"])
         assert result == api_client.Login(state=False, data=None)
         assert api_client.request_server.calls == [
             pretend.call(
                 "http://server",
                 "api/v1/token/?token=fake_token",
                 api_client.Methods.get,
                 headers={"Authorization": "Bearer fake_token"},
             )
         ]
 
-    def test_is_logged_500(self):
+    def test_is_logged_500(self, test_context):
         fake_response = pretend.stub(
             status_code=500,
             text="body",
         )
         api_client.request_server = pretend.call_recorder(
             lambda *a, **kw: fake_response
         )
 
+        test_context["settings"].SERVER = "http://server"
+        test_context["settings"].TOKEN = "fake_token"
         with pytest.raises(api_client.click.ClickException) as err:
-            api_client.is_logged("http://server", "fake_token")
+            api_client.is_logged(test_context["settings"])
 
         assert "Error 500 body" in str(err)
         assert api_client.request_server.calls == [
             pretend.call(
                 "http://server",
                 "api/v1/token/?token=fake_token",
                 api_client.Methods.get,
                 headers={"Authorization": "Bearer fake_token"},
             )
         ]
 
-    def test_get_headers(self):
+    def test_get_headers(self, test_context):
         api_client.is_logged = pretend.call_recorder(
             lambda *a: api_client.Login(
                 state=True, data={"data": {"expired": False}}
             )
         )
         api_client.request_server = pretend.call_recorder(
             lambda *a, **kw: pretend.stub(status_code=200)
         )
 
-        result = api_client.get_headers(
-            {"SERVER": "http://server", "TOKEN": "fake_token"}
-        )
+        test_context["settings"].SERVER = "http://server"
+        test_context["settings"].TOKEN = "fake_token"
+        result = api_client.get_headers(test_context["settings"])
 
         assert result == {"Authorization": "Bearer fake_token"}
         assert api_client.is_logged.calls == [
-            pretend.call("http://server", "fake_token")
+            pretend.call(test_context["settings"])
         ]
         assert api_client.request_server.calls == [
             pretend.call(
                 "http://server",
                 api_client.URL.bootstrap.value,
                 api_client.Methods.get,
                 headers={"Authorization": "Bearer fake_token"},
             )
         ]
 
+    def test_get_headers_no_auth(self, test_context):
+        test_context["settings"].AUTH = False
+        result = api_client.get_headers(test_context["settings"])
+
+        assert result == {}
+
     def test_get_headers_never_logged(self):
         with pytest.raises(api_client.click.ClickException) as err:
             api_client.get_headers({})
 
         assert "Login first. Run 'rstuf admin login'" in str(err)
 
-    def test_get_headers_is_logged_state_false(self):
+    def test_get_headers_is_logged_state_false(self, test_context):
         api_client.is_logged = pretend.call_recorder(
             lambda *a: api_client.Login(state=False, data={"expired": False})
         )
 
+        test_context["settings"].SERVER = "http://server"
+        test_context["settings"].TOKEN = "fake_token"
         with pytest.raises(api_client.click.ClickException) as err:
-            api_client.get_headers(
-                {"SERVER": "http://server", "TOKEN": "fake_token"}
-            )
+            api_client.get_headers(test_context["settings"])
 
         assert "re-login" in str(err)
         assert api_client.is_logged.calls == [
-            pretend.call("http://server", "fake_token")
+            pretend.call(test_context["settings"])
         ]
 
-    def test_get_headers_is_logged_state_true_expired_token(self):
+    def test_get_headers_is_logged_state_true_expired_token(
+        self, test_context
+    ):
         api_client.is_logged = pretend.call_recorder(
             lambda *a: api_client.Login(state=True, data={"expired": True})
         )
 
+        test_context["settings"].SERVER = "http://server"
+        test_context["settings"].TOKEN = "fake_token"
         with pytest.raises(api_client.click.ClickException) as err:
-            api_client.get_headers(
-                {"SERVER": "http://server", "TOKEN": "fake_token"}
-            )
+            api_client.get_headers(test_context["settings"])
 
         assert "The token has expired" in str(err)
         assert api_client.is_logged.calls == [
-            pretend.call("http://server", "fake_token")
+            pretend.call(test_context["settings"])
         ]
 
-    def test_get_headers_unexpected_error(self):
+    def test_get_headers_unexpected_error(self, test_context):
         api_client.is_logged = pretend.call_recorder(
             lambda *a: api_client.Login(state=True, data={"expired": False})
         )
         api_client.request_server = pretend.call_recorder(
             lambda *a, **kw: pretend.stub(status_code=500, text="error body")
         )
+
+        test_context["settings"].SERVER = "http://server"
+        test_context["settings"].TOKEN = "fake_token"
         with pytest.raises(api_client.click.ClickException) as err:
-            api_client.get_headers(
-                {"SERVER": "http://server", "TOKEN": "fake_token"}
-            )
+            api_client.get_headers(test_context["settings"])
 
         assert "Unexpected error" in str(err)
         assert api_client.is_logged.calls == [
-            pretend.call("http://server", "fake_token")
+            pretend.call(test_context["settings"])
         ]
 
     def test_bootstrap_status(self, test_context):
         test_context["settings"].SERVER = "http://server"
         api_client.get_headers = pretend.call_recorder(
             lambda *a: {"auth": "token"}
         )
```

### Comparing `repository_service_tuf-0.1.0a1/tests/unit/helpers/test_tuf.py` & `repository_service_tuf-0.1.1a2/tests/unit/helpers/test_tuf.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.0a1/PKG-INFO` & `repository_service_tuf-0.1.1a2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repository-service-tuf
-Version: 0.1.0a1
+Version: 0.1.1a2
 Summary: Repository Service for TUF Command Line Interface
 Author-email: Kairo de Araujo <kairo@dearaujo.nl>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

