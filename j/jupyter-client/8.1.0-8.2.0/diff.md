# Comparing `tmp/jupyter_client-8.1.0.tar.gz` & `tmp/jupyter_client-8.2.0.tar.gz`

## Comparing `jupyter_client-8.1.0.tar` & `jupyter_client-8.2.0.tar`

### file list

```diff
@@ -1,98 +1,97 @@
--rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/.mailmap
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/.readthedocs.yaml
--rw-r--r--   0        0        0    75321 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/RELEASING.md
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/codecov.yml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/.github/workflows/downstream.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/Makefile
--rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/conf.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/index.rst
--rw-r--r--   0        0        0     8611 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/kernels.rst
--rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/make.bat
--rw-r--r--   0        0        0    64020 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/messaging.rst
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/migration.md
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/pending-kernels.rst
--rw-r--r--   0        0        0    15197 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/provisioning.rst
--rw-r--r--   0        0        0     7302 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/wrapperkernels.rst
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/api/jupyter_client.asynchronous.rst
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/api/jupyter_client.blocking.rst
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/api/jupyter_client.ioloop.rst
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/api/jupyter_client.provisioning.rst
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/api/jupyter_client.rst
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/api/jupyter_client.ssh.rst
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/api/modules.rst
--rw-r--r--   0        0        0   153577 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/figs/frontend-kernel.png
--rw-r--r--   0        0        0   283952 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/docs/figs/frontend-kernel.svg
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/__init__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/_version.py
--rw-r--r--   0        0        0    14381 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/adapter.py
--rw-r--r--   0        0        0    10745 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/channels.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/channelsabc.py
--rw-r--r--   0        0        0    30383 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/client.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/clientabc.py
--rw-r--r--   0        0        0    25052 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/connect.py
--rw-r--r--   0        0        0    13827 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/consoleapp.py
--rw-r--r--   0        0        0     5956 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/jsonutil.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/kernelapp.py
--rw-r--r--   0        0        0    15109 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/kernelspec.py
--rw-r--r--   0        0        0    11904 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/kernelspecapp.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/launcher.py
--rw-r--r--   0        0        0     8004 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/localinterfaces.py
--rw-r--r--   0        0        0    28678 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/manager.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/managerabc.py
--rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/multikernelmanager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/py.typed
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/restarter.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/runapp.py
--rw-r--r--   0        0        0    37594 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/session.py
--rw-r--r--   0        0        0     9810 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/threaded.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/utils.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/win_interrupt.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/asynchronous/__init__.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/asynchronous/client.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/blocking/__init__.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/blocking/client.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/ioloop/__init__.py
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/ioloop/manager.py
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/ioloop/restarter.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/provisioning/__init__.py
--rw-r--r--   0        0        0     9611 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/provisioning/factory.py
--rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/provisioning/local_provisioner.py
--rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/provisioning/provisioner_base.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/ssh/__init__.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/ssh/forward.py
--rw-r--r--   0        0        0    12948 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/jupyter_client/ssh/tunnel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/conftest.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/problemkernel.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/signalkernel.py
--rw-r--r--   0        0        0    14436 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_adapter.py
--rw-r--r--   0        0        0     9886 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_client.py
--rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_connect.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_consoleapp.py
--rw-r--r--   0        0        0     5926 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_jsonutil.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_kernelapp.py
--rw-r--r--   0        0        0    19981 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_kernelmanager.py
--rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_kernelspec.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_kernelspecapp.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_localinterfaces.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_manager.py
--rw-r--r--   0        0        0    23126 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_multikernelmanager.py
--rw-r--r--   0        0        0    11892 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_provisioning.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_public_api.py
--rw-r--r--   0        0        0     8408 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_restarter.py
--rw-r--r--   0        0        0    19845 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_session.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/test_ssh.py
--rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/tests/utils.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/.gitignore
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/LICENSE
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/README.md
--rw-r--r--   0        0        0     6542 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/pyproject.toml
--rw-r--r--   0        0        0     8565 2020-02-02 00:00:00.000000 jupyter_client-8.1.0/PKG-INFO
+-rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.mailmap
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0    76659 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/RELEASING.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.github/workflows/downstream.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/Makefile
+-rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/conf.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/index.rst
+-rw-r--r--   0        0        0     8611 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/kernels.rst
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/make.bat
+-rw-r--r--   0        0        0    64020 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/messaging.rst
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/migration.md
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/pending-kernels.rst
+-rw-r--r--   0        0        0    15197 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/provisioning.rst
+-rw-r--r--   0        0        0     7302 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/wrapperkernels.rst
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/api/jupyter_client.asynchronous.rst
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/api/jupyter_client.blocking.rst
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/api/jupyter_client.ioloop.rst
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/api/jupyter_client.provisioning.rst
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/api/jupyter_client.rst
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/api/jupyter_client.ssh.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/api/modules.rst
+-rw-r--r--   0        0        0   153577 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/figs/frontend-kernel.png
+-rw-r--r--   0        0        0   283952 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/figs/frontend-kernel.svg
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/__init__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/_version.py
+-rw-r--r--   0        0        0    14381 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/adapter.py
+-rw-r--r--   0        0        0    10745 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/channels.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/channelsabc.py
+-rw-r--r--   0        0        0    30383 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/client.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/clientabc.py
+-rw-r--r--   0        0        0    25088 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/connect.py
+-rw-r--r--   0        0        0    13841 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/consoleapp.py
+-rw-r--r--   0        0        0     5956 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/jsonutil.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/kernelapp.py
+-rw-r--r--   0        0        0    15109 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/kernelspec.py
+-rw-r--r--   0        0        0    11904 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/kernelspecapp.py
+-rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/launcher.py
+-rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/localinterfaces.py
+-rw-r--r--   0        0        0    28686 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/manager.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/managerabc.py
+-rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/multikernelmanager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/py.typed
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/restarter.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/runapp.py
+-rw-r--r--   0        0        0    37674 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/session.py
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/threaded.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/utils.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/win_interrupt.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/asynchronous/__init__.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/asynchronous/client.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/blocking/__init__.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/blocking/client.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/ioloop/__init__.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/ioloop/manager.py
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/ioloop/restarter.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/provisioning/__init__.py
+-rw-r--r--   0        0        0     9611 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/provisioning/factory.py
+-rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/provisioning/local_provisioner.py
+-rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/provisioning/provisioner_base.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/ssh/__init__.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/ssh/forward.py
+-rw-r--r--   0        0        0    13004 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/ssh/tunnel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/problemkernel.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/signalkernel.py
+-rw-r--r--   0        0        0    14444 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_adapter.py
+-rw-r--r--   0        0        0     9886 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_client.py
+-rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_connect.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_consoleapp.py
+-rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_jsonutil.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_kernelapp.py
+-rw-r--r--   0        0        0    19981 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_kernelmanager.py
+-rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_kernelspec.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_kernelspecapp.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_localinterfaces.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_manager.py
+-rw-r--r--   0        0        0    23126 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_multikernelmanager.py
+-rw-r--r--   0        0        0    11892 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_provisioning.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_public_api.py
+-rw-r--r--   0        0        0     8408 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_restarter.py
+-rw-r--r--   0        0        0    19845 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_session.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_ssh.py
+-rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/utils.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.gitignore
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/LICENSE
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/README.md
+-rw-r--r--   0        0        0     6833 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/PKG-INFO
```

### Comparing `jupyter_client-8.1.0/.mailmap` & `jupyter_client-8.2.0/.mailmap`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/.pre-commit-config.yaml` & `jupyter_client-8.2.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,26 @@
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.21.0
+    rev: 0.22.0
     hooks:
       - id: check-github-workflows
 
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.254
+    rev: v0.0.260
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `jupyter_client-8.1.0/CHANGELOG.md` & `jupyter_client-8.2.0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,32 @@
 # Changes in Jupyter Client {#changelog}
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 8.2.0
+
+([Full Changelog](https://github.com/jupyter/jupyter_client/compare/v8.1.0...dbf6b81fa5ab606eaedc5e8d0843debce18e8746))
+
+### Enhancements made
+
+- use c.f.Future to wait across threads [#940](https://github.com/jupyter/jupyter_client/pull/940) ([@minrk](https://github.com/minrk))
+
+### Maintenance and upkeep improvements
+
+- Use local coverage [#945](https://github.com/jupyter/jupyter_client/pull/945) ([@blink1073](https://github.com/blink1073))
+- Add more project URLs [#944](https://github.com/jupyter/jupyter_client/pull/944) ([@fcollonval](https://github.com/fcollonval))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter/jupyter_client/graphs/contributors?from=2023-03-20&to=2023-04-13&type=c))
+
+[@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_client+involves%3Ablink1073+updated%3A2023-03-20..2023-04-13&type=Issues) | [@fcollonval](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_client+involves%3Afcollonval+updated%3A2023-03-20..2023-04-13&type=Issues) | [@minrk](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_client+involves%3Aminrk+updated%3A2023-03-20..2023-04-13&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_client+involves%3Apre-commit-ci+updated%3A2023-03-20..2023-04-13&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 8.1.0
 
 ([Full Changelog](https://github.com/jupyter/jupyter_client/compare/v8.0.3...e3ac7a69355dd1af66038eda767e51e92ef034fb))
 
 ### Bugs fixed
 
 - ThreadedZMQStream: close stream before socket [#936](https://github.com/jupyter/jupyter_client/pull/936) ([@minrk](https://github.com/minrk))
@@ -18,16 +39,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter/jupyter_client/graphs/contributors?from=2023-02-16&to=2023-03-20&type=c))
 
 [@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_client+involves%3Ablink1073+updated%3A2023-02-16..2023-03-20&type=Issues) | [@brichet](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_client+involves%3Abrichet+updated%3A2023-02-16..2023-03-20&type=Issues) | [@minrk](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_client+involves%3Aminrk+updated%3A2023-02-16..2023-03-20&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_client+involves%3Apre-commit-ci+updated%3A2023-02-16..2023-03-20&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 8.0.3
 
 ([Full Changelog](https://github.com/jupyter/jupyter_client/compare/v8.0.2...dc0eaba1f609079672ec739fcd977dc44431da92))
 
 ### Bugs fixed
 
 - Fix kernelspec print output [#933](https://github.com/jupyter/jupyter_client/pull/933) ([@minrk](https://github.com/minrk))
```

### Comparing `jupyter_client-8.1.0/RELEASING.md` & `jupyter_client-8.2.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/.github/workflows/downstream.yml` & `jupyter_client-8.2.0/.github/workflows/downstream.yml`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/.github/workflows/main.yml` & `jupyter_client-8.2.0/.github/workflows/main.yml`

 * *Files 3% similar despite different names*

```diff
@@ -61,18 +61,25 @@
         if: ${{ startsWith(matrix.python-version, 'pypy') }}
         run: |
           hatch run test:nowarn || hatch run test:nowarn --lf
       - name: Run the tests on windows
         if: ${{ startsWith(matrix.os, 'windows') }}
         run: |
           hatch run cov:nowarn || hatch run test:nowarn --lf
-      - name: Code coverage
-        run: |
-          pip install codecov coverage[toml]
-          codecov
+      - uses: jupyterlab/maintainer-tools/.github/actions/upload-coverage@v1
+
+  coverage:
+    runs-on: ubuntu-latest
+    needs:
+      - test
+    steps:
+      - uses: actions/checkout@v3
+      - uses: jupyterlab/maintainer-tools/.github/actions/report-coverage@v1
+        with:
+          fail_under: 78
 
   docs:
     runs-on: windows-latest
     steps:
       - uses: actions/checkout@v3
       - uses: jupyterlab/maintainer-tools/.github/actions/base-setup@v1
       - name: Build API docs
@@ -144,15 +151,15 @@
       - uses: jupyterlab/maintainer-tools/.github/actions/test-sdist@v1
         with:
           test_command: pytest -vv || pytest -vv --lf
 
   tests_check: # This job does nothing and is only used for the branch protection
     if: always()
     needs:
-      - test
+      - coverage
       - docs
       - lint
       - check_links
       - test_minimum_verisons
       - test_prereleases
       - test_sdist
     runs-on: ubuntu-latest
```

### Comparing `jupyter_client-8.1.0/.github/workflows/prep-release.yml` & `jupyter_client-8.2.0/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/.github/workflows/publish-release.yml` & `jupyter_client-8.2.0/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/docs/Makefile` & `jupyter_client-8.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/docs/conf.py` & `jupyter_client-8.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/docs/index.rst` & `jupyter_client-8.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/docs/kernels.rst` & `jupyter_client-8.2.0/docs/kernels.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/docs/make.bat` & `jupyter_client-8.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/docs/messaging.rst` & `jupyter_client-8.2.0/docs/messaging.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/docs/migration.md` & `jupyter_client-8.2.0/docs/migration.md`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/docs/pending-kernels.rst` & `jupyter_client-8.2.0/docs/pending-kernels.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/docs/provisioning.rst` & `jupyter_client-8.2.0/docs/provisioning.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/docs/wrapperkernels.rst` & `jupyter_client-8.2.0/docs/wrapperkernels.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/docs/api/jupyter_client.provisioning.rst` & `jupyter_client-8.2.0/docs/api/jupyter_client.provisioning.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/docs/api/jupyter_client.rst` & `jupyter_client-8.2.0/docs/api/jupyter_client.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/docs/figs/frontend-kernel.png` & `jupyter_client-8.2.0/docs/figs/frontend-kernel.png`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/docs/figs/frontend-kernel.svg` & `jupyter_client-8.2.0/docs/figs/frontend-kernel.svg`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/_version.py` & `jupyter_client-8.2.0/jupyter_client/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """The version information for jupyter client."""
 import re
 from typing import List, Union
 
-__version__ = "8.1.0"
+__version__ = "8.2.0"
 
 # Build up version_info tuple for backwards compatibility
 pattern = r'(?P<major>\d+).(?P<minor>\d+).(?P<patch>\d+)(?P<rest>.*)'
 match = re.match(pattern, __version__)
 if match:
     parts: List[Union[int, str]] = [int(match[part]) for part in ['major', 'minor', 'patch']]
     if match['rest']:
```

### Comparing `jupyter_client-8.1.0/jupyter_client/adapter.py` & `jupyter_client-8.2.0/jupyter_client/adapter.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/channels.py` & `jupyter_client-8.2.0/jupyter_client/channels.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/channelsabc.py` & `jupyter_client-8.2.0/jupyter_client/channelsabc.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/client.py` & `jupyter_client-8.2.0/jupyter_client/client.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/clientabc.py` & `jupyter_client-8.2.0/jupyter_client/clientabc.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/connect.py` & `jupyter_client-8.2.0/jupyter_client/connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,17 @@
         Paths in which to search for connection files.
 
     Returns
     -------
     str : The absolute path of the connection file.
     """
     if profile is not None:
-        warnings.warn("Jupyter has no profiles. profile=%s has been ignored." % profile)
+        warnings.warn(
+            "Jupyter has no profiles. profile=%s has been ignored." % profile, stacklevel=2
+        )
     if path is None:
         path = [".", jupyter_runtime_dir()]
     if isinstance(path, str):
         path = [path]
 
     try:
         # first, try explicit name
```

### Comparing `jupyter_client-8.1.0/jupyter_client/consoleapp.py` & `jupyter_client-8.2.0/jupyter_client/consoleapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,9 +367,9 @@
 
 
 class IPythonConsoleApp(JupyterConsoleApp):
     """An app to manage an ipython console."""
 
     def __init__(self, *args, **kwargs):
         """Initialize the app."""
-        warnings.warn("IPythonConsoleApp is deprecated. Use JupyterConsoleApp")
+        warnings.warn("IPythonConsoleApp is deprecated. Use JupyterConsoleApp", stacklevel=2)
         super().__init__(*args, **kwargs)
```

### Comparing `jupyter_client-8.1.0/jupyter_client/jsonutil.py` & `jupyter_client-8.2.0/jupyter_client/jsonutil.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/kernelapp.py` & `jupyter_client-8.2.0/jupyter_client/kernelapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/kernelspec.py` & `jupyter_client-8.2.0/jupyter_client/kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/kernelspecapp.py` & `jupyter_client-8.2.0/jupyter_client/kernelspecapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/launcher.py` & `jupyter_client-8.2.0/jupyter_client/launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,16 +158,19 @@
             msg = "Failed to run command:\n{}\n    PATH={!r}\n    with kwargs:\n{!r}\n"
             # exclude environment variables,
             # which may contain access tokens and the like.
             without_env = {key: value for key, value in kwargs.items() if key != "env"}
             msg = msg.format(cmd, env.get("PATH", os.defpath), without_env)
             get_logger().error(msg)
         except Exception as ex2:  # Don't let a formatting/logger issue lead to the wrong exception
-            warnings.warn(f"Failed to run command: '{cmd}' due to exception: {ex}")
-            warnings.warn(f"The following exception occurred handling the previous failure: {ex2}")
+            warnings.warn(f"Failed to run command: '{cmd}' due to exception: {ex}", stacklevel=2)
+            warnings.warn(
+                f"The following exception occurred handling the previous failure: {ex2}",
+                stacklevel=2,
+            )
         raise ex
 
     if sys.platform == "win32":
         # Attach the interrupt event to the Popen objet so it can be used later.
         proc.win32_interrupt_event = interrupt_event
 
     # Clean up pipes created to work around Popen bug.
```

### Comparing `jupyter_client-8.1.0/jupyter_client/localinterfaces.py` & `jupyter_client-8.2.0/jupyter_client/localinterfaces.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
         # lowest priority, use gethostbyname
 
         return _load_ips_gethostbyname()
     except Exception as e:
         if not suppress_exceptions:
             raise
         # unexpected error shouldn't crash, load dumb default values instead.
-        warn("Unexpected error discovering local network interfaces: %s" % e)
+        warn("Unexpected error discovering local network interfaces: %s" % e, stacklevel=2)
     _load_ips_dumb()
 
 
 @_requires_ips
 def local_ips():
     """return the IP addresses that point to this machine"""
     return LOCAL_IPS
```

### Comparing `jupyter_client-8.1.0/jupyter_client/manager.py` & `jupyter_client-8.2.0/jupyter_client/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,15 @@
         if change["new"] == "python":
             self.kernel_name = kernelspec.NATIVE_KERNEL_NAME
 
     _kernel_spec: t.Optional[kernelspec.KernelSpec] = None
 
     @property
     def kernel_spec(self) -> t.Optional[kernelspec.KernelSpec]:
-        if self._kernel_spec is None and self.kernel_name != "":
+        if self._kernel_spec is None and self.kernel_name != "":  # noqa
             self._kernel_spec = self.kernel_spec_manager.get_kernel_spec(self.kernel_name)
         return self._kernel_spec
 
     cache_ports: Bool = Bool(
         help="True if the MultiKernelManager should cache ports for this KernelManager instance"
     )
```

### Comparing `jupyter_client-8.1.0/jupyter_client/managerabc.py` & `jupyter_client-8.2.0/jupyter_client/managerabc.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/multikernelmanager.py` & `jupyter_client-8.2.0/jupyter_client/multikernelmanager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/restarter.py` & `jupyter_client-8.2.0/jupyter_client/restarter.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/runapp.py` & `jupyter_client-8.2.0/jupyter_client/runapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/session.py` & `jupyter_client-8.2.0/jupyter_client/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
 
 def default_secure(cfg: t.Any) -> None:  # pragma: no cover
     """Set the default behavior for a config environment to be secure.
 
     If Session.key/keyfile have not been set, set Session.key to
     a new random UUID.
     """
-    warnings.warn("default_secure is deprecated", DeprecationWarning)
+    warnings.warn("default_secure is deprecated", DeprecationWarning, stacklevel=2)
     if "Session" in cfg and ("key" in cfg.Session or "keyfile" in cfg.Session):
         return
     # key/keyfile not specified, generate new UUID:
     cfg.Session.key = new_id_bytes()
 
 
 def utcnow() -> datetime:
@@ -563,15 +563,15 @@
             The file containing a key.  If this is set, `key` will be
             initialized to the contents of the file.
         """
         super().__init__(**kwargs)
         self._check_packers()
         self.none = self.pack({})
         # ensure self._session_default() if necessary, so bsession is defined:
-        self.session
+        self.session  # noqa
         self.pid = os.getpid()
         self._new_auth()
         if not self.key:
             get_logger().warning(
                 "Message signing is disabled.  This is insecure and not recommended!"
             )
 
@@ -857,17 +857,17 @@
             tracker = stream.send_multipart(to_send, copy=False, track=True)
         elif stream:
             # use dummy tracker, which will be done immediately
             tracker = DONE
             stream.send_multipart(to_send, copy=copy)
 
         if self.debug:
-            pprint.pprint(msg)
-            pprint.pprint(to_send)
-            pprint.pprint(buffers)
+            pprint.pprint(msg)  # noqa
+            pprint.pprint(to_send)  # noqa
+            pprint.pprint(buffers)  # noqa
 
         msg["tracker"] = tracker
 
         return msg
 
     def send_raw(
         self,
@@ -1084,19 +1084,20 @@
         buffers = [memoryview(b) for b in msg_list[5:]]
         if buffers and buffers[0].shape is None:
             # force copy to workaround pyzmq #646
             msg_list = t.cast(t.List[zmq.Message], msg_list)
             buffers = [memoryview(bytes(b.bytes)) for b in msg_list[5:]]
         message["buffers"] = buffers
         if self.debug:
-            pprint.pprint(message)
+            pprint.pprint(message)  # noqa
         # adapt to the current version
         return adapt(message)
 
     def unserialize(self, *args: t.Any, **kwargs: t.Any) -> t.Dict[str, t.Any]:
         """**DEPRECATED** Use deserialize instead."""
         # pragma: no cover
         warnings.warn(
             "Session.unserialize is deprecated. Use Session.deserialize.",
             DeprecationWarning,
+            stacklevel=2,
         )
         return self.deserialize(*args, **kwargs)
```

### Comparing `jupyter_client-8.1.0/jupyter_client/threaded.py` & `jupyter_client-8.2.0/jupyter_client/threaded.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """ Defines a KernelClient that provides thread-safe sockets with async callbacks on message
 replies.
 """
 import asyncio
 import atexit
 import time
 from concurrent.futures import Future
-from threading import Event, Thread
+from functools import partial
+from threading import Thread
 from typing import Any, Dict, List, Optional
 
 import zmq
 from tornado.ioloop import IOLoop
 from traitlets import Instance, Type
 from traitlets.log import get_logger
 from zmq.eventloop import zmqstream
@@ -50,25 +51,30 @@
             A tornado ioloop to connect the socket to using a ZMQStream
         """
         super().__init__()
 
         self.socket = socket
         self.session = session
         self.ioloop = loop
-        evt = Event()
+        f: Future = Future()
 
         def setup_stream():
-            assert self.socket is not None
-            self.stream = zmqstream.ZMQStream(self.socket, self.ioloop)
-            self.stream.on_recv(self._handle_recv)
-            evt.set()
+            try:
+                assert self.socket is not None
+                self.stream = zmqstream.ZMQStream(self.socket, self.ioloop)
+                self.stream.on_recv(self._handle_recv)
+            except Exception as e:
+                f.set_exception(e)
+            else:
+                f.set_result(None)
 
         assert self.ioloop is not None
         self.ioloop.add_callback(setup_stream)
-        evt.wait()
+        # don't wait forever, raise any errors
+        f.result(timeout=10)
 
     _is_alive = False
 
     def is_alive(self) -> bool:
         """Whether the channel is alive."""
         return self._is_alive
 
@@ -175,21 +181,39 @@
         ----------
         timeout : float, optional
             The maximum amount of time to spend flushing, in seconds. The
             default is one second.
         """
         # We do the IOLoop callback process twice to ensure that the IOLoop
         # gets to perform at least one full poll.
-        stop_time = time.time() + timeout
+        stop_time = time.monotonic() + timeout
         assert self.ioloop is not None
+        if self.stream is None or self.stream.closed():
+            # don't bother scheduling flush on a thread if we're closed
+            _msg = "Attempt to flush closed stream"
+            raise OSError(_msg)
+
+        def flush(f):
+            try:
+                self._flush()
+            except Exception as e:
+                f.set_exception(e)
+            else:
+                f.set_result(None)
+
         for _ in range(2):
-            self._flushed = False
-            self.ioloop.add_callback(self._flush)
-            while not self._flushed and time.time() < stop_time:
-                time.sleep(0.01)
+            f: Future = Future()
+            self.ioloop.add_callback(partial(flush, f))
+            # wait for async flush, re-raise any errors
+            timeout = max(stop_time - time.monotonic(), 0)
+            try:
+                f.result(max(stop_time - time.monotonic(), 0))
+            except TimeoutError:
+                # flush with a timeout means stop waiting, not raise
+                return
 
     def _flush(self) -> None:
         """Callback for :method:`self.flush`."""
         assert self.stream is not None
         self.stream.flush()
         self._flushed = True
 
@@ -215,32 +239,40 @@
 
     def start(self) -> None:
         """Start the IOLoop thread
 
         Don't return until self.ioloop is defined,
         which is created in the thread
         """
-        self._start_event = Event()
+        self._start_future: Future = Future()
         Thread.start(self)
-        self._start_event.wait()
+        # wait for start, re-raise any errors
+        self._start_future.result(timeout=10)
 
     def run(self) -> None:
         """Run my loop, ignoring EINTR events in the poller"""
-        loop = asyncio.new_event_loop()
-        asyncio.set_event_loop(loop)
+        try:
+            loop = asyncio.new_event_loop()
+            asyncio.set_event_loop(loop)
+
+            async def assign_ioloop():
+                self.ioloop = IOLoop.current()
+
+            loop.run_until_complete(assign_ioloop())
+        except Exception as e:
+            self._start_future.set_exception(e)
+        else:
+            self._start_future.set_result(None)
+
         loop.run_until_complete(self._async_run())
 
     async def _async_run(self):
-        self.ioloop = IOLoop.current()
-        # signal that self.ioloop is defined
-        self._start_event.set()
-        while True:
+        """Run forever (until self._exiting is set)"""
+        while not self._exiting:
             await asyncio.sleep(1)
-            if self._exiting:
-                break
 
     def stop(self) -> None:
         """Stop the channel's event loop and join its thread.
 
         This calls :meth:`~threading.Thread.join` and returns when the thread
         terminates. :class:`RuntimeError` will be raised if
         :meth:`~threading.Thread.start` is called again.
```

### Comparing `jupyter_client-8.1.0/jupyter_client/utils.py` & `jupyter_client-8.2.0/jupyter_client/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/win_interrupt.py` & `jupyter_client-8.2.0/jupyter_client/win_interrupt.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/asynchronous/client.py` & `jupyter_client-8.2.0/jupyter_client/asynchronous/client.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/blocking/client.py` & `jupyter_client-8.2.0/jupyter_client/blocking/client.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/ioloop/manager.py` & `jupyter_client-8.2.0/jupyter_client/ioloop/manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/ioloop/restarter.py` & `jupyter_client-8.2.0/jupyter_client/ioloop/restarter.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/provisioning/factory.py` & `jupyter_client-8.2.0/jupyter_client/provisioning/factory.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/provisioning/local_provisioner.py` & `jupyter_client-8.2.0/jupyter_client/provisioning/local_provisioner.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/provisioning/provisioner_base.py` & `jupyter_client-8.2.0/jupyter_client/provisioning/provisioner_base.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/ssh/forward.py` & `jupyter_client-8.2.0/jupyter_client/ssh/forward.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/jupyter_client/ssh/tunnel.py` & `jupyter_client-8.2.0/jupyter_client/ssh/tunnel.py`

 * *Files 3% similar despite different names*

```diff
@@ -265,15 +265,15 @@
             tunnel.wait()
             if tunnel.exitstatus:
                 raise RuntimeError("tunnel '%s' failed to start" % (cmd)) from e
             else:
                 return tunnel.pid
         else:
             if failed:
-                warnings.warn("Password rejected, try again")
+                warnings.warn("Password rejected, try again", stacklevel=2)
                 password = None
             if password is None:
                 password = getpass("%s's password: " % (server))
             tunnel.sendline(password)
             failed = True
 
 
@@ -374,27 +374,27 @@
     #    except paramiko.AuthenticationException:
     #        if password is None:
     #            password = getpass("%s@%s's password: "%(username, server))
     #            client.connect(server, port, username=username, password=password)
     #        else:
     #            raise
     except Exception as e:
-        warnings.warn("*** Failed to connect to %s:%d: %r" % (server, port, e))
+        warnings.warn("*** Failed to connect to %s:%d: %r" % (server, port, e), stacklevel=2)
         sys.exit(1)
 
     # Don't let SIGINT kill the tunnel subprocess
     signal.signal(signal.SIGINT, signal.SIG_IGN)
 
     try:
         forward_tunnel(lport, remoteip, rport, client.get_transport())
     except KeyboardInterrupt:
-        warnings.warn("SIGINT: Port forwarding stopped cleanly")
+        warnings.warn("SIGINT: Port forwarding stopped cleanly", stacklevel=2)
         sys.exit(0)
     except Exception as e:
-        warnings.warn("Port forwarding stopped uncleanly: %s" % e)
+        warnings.warn("Port forwarding stopped uncleanly: %s" % e, stacklevel=2)
         sys.exit(255)
 
 
 if sys.platform == "win32":
     ssh_tunnel = paramiko_tunnel
 else:
     ssh_tunnel = openssh_tunnel
```

### Comparing `jupyter_client-8.1.0/tests/problemkernel.py` & `jupyter_client-8.2.0/tests/problemkernel.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/signalkernel.py` & `jupyter_client-8.2.0/tests/signalkernel.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/test_adapter.py` & `jupyter_client-8.2.0/tests/test_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     original = copy.deepcopy(msg)
     adapted = adapt(original)
     assert adapted["header"]["version"] == V4toV5.version
 
 
 def test_code_to_line_no_code():
     line, pos = code_to_line("", 0)
-    assert line == ""
+    assert line == ""  # noqa
     assert pos == 0
 
 
 class AdapterTest(TestCase):
     def setUp(self):
         self.session = Session()
```

### Comparing `jupyter_client-8.1.0/tests/test_client.py` & `jupyter_client-8.2.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/test_connect.py` & `jupyter_client-8.2.0/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/test_consoleapp.py` & `jupyter_client-8.2.0/tests/test_consoleapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/test_jsonutil.py` & `jupyter_client-8.2.0/tests/test_jsonutil.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 numbers.Real.register(MyFloat)
 
 
 def test_parse_date_invalid():
     assert jsonutil.parse_date(None) is None
-    assert jsonutil.parse_date("") == ""
+    assert jsonutil.parse_date("") == ""  # noqa
     assert jsonutil.parse_date("invalid-date") == "invalid-date"
 
 
 def test_parse_date_valid():
     ref = REFERENCE_DATETIME
     timestamp = "2013-07-03T16:34:52.249482Z"
     parsed = jsonutil.parse_date(timestamp)
```

### Comparing `jupyter_client-8.1.0/tests/test_kernelapp.py` & `jupyter_client-8.2.0/tests/test_kernelapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/test_kernelmanager.py` & `jupyter_client-8.2.0/tests/test_kernelmanager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/test_kernelspec.py` & `jupyter_client-8.2.0/tests/test_kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/test_kernelspecapp.py` & `jupyter_client-8.2.0/tests/test_kernelspecapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/test_localinterfaces.py` & `jupyter_client-8.2.0/tests/test_localinterfaces.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/test_manager.py` & `jupyter_client-8.2.0/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/test_multikernelmanager.py` & `jupyter_client-8.2.0/tests/test_multikernelmanager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/test_provisioning.py` & `jupyter_client-8.2.0/tests/test_provisioning.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/test_public_api.py` & `jupyter_client-8.2.0/tests/test_public_api.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/test_restarter.py` & `jupyter_client-8.2.0/tests/test_restarter.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/test_session.py` & `jupyter_client-8.2.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/tests/utils.py` & `jupyter_client-8.2.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/LICENSE` & `jupyter_client-8.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.1.0/README.md` & `jupyter_client-8.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Jupyter Client
 
 [![Build Status](https://github.com/jupyter/jupyter_client/workflows/CI/badge.svg)](https://github.com/jupyter/jupyter_client/actions)
-[![codecov](https://codecov.io/gh/jupyter/jupyter_client/branch/main/graph/badge.svg?token=kxoFu4KnhT)](https://codecov.io/gh/jupyter/jupyter_client)
 [![Documentation Status](https://readthedocs.org/projects/jupyter-client/badge/?version=latest)](http://jupyter-client.readthedocs.io/en/latest/?badge=latest)
 
 `jupyter_client` contains the reference implementation of the [Jupyter protocol].
 It also provides client and kernel management APIs for working with kernels.
 
 It also provides the `jupyter kernelspec` entrypoint
 for installing kernelspecs for use with Jupyter frontends.
```

### Comparing `jupyter_client-8.1.0/pyproject.toml` & `jupyter_client-8.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -41,18 +41,19 @@
 content-type = "text/markdown"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://jupyter.org"
+Documentation = "https://jupyter-client.readthedocs.io/"
+Source = "https://github.com/jupyter/jupyter_client"
 
 [project.optional-dependencies]
 test = [
-    "codecov",
     "coverage",
     "ipykernel>=6.14",
     "mypy",
     "paramiko; sys_platform == 'win32'",
     "pre-commit",
     "pytest",
     "pytest-jupyter[client]>=0.4.1",
@@ -104,17 +105,17 @@
 features = ["test"]
 dependencies = ["mypy>=0.990"]
 [tool.hatch.envs.typing.scripts]
 test = "mypy --install-types --non-interactive {args:.}"
 
 [tool.hatch.envs.lint]
 dependencies = [
-  "black[jupyter]==23.1.0",
+  "black[jupyter]==23.3.0",
   "mdformat>0.7",
-  "ruff==0.0.254",
+  "ruff==0.0.260",
 ]
 [tool.hatch.envs.lint.scripts]
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
   "mdformat --check {args:docs *.md}"
 ]
@@ -151,14 +152,18 @@
   "class .*\bProtocol\\):",
 "@(abc\\.)?abstractmethod",
 ]
 omit = [
     "jupyter_client/ssh/forward.py"
 ]
 
+[tool.coverage.run]
+relative_files = true
+source = ["jupyter_client"]
+
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = false
 disallow_incomplete_defs = true
 disallow_untyped_decorators = true
 no_implicit_optional = true
 no_implicit_reexport = false
@@ -246,14 +251,16 @@
   "PLW0603",
 ]
 unfixable = [
   # Don't touch print statements
   "T201",
   # Don't touch noqa lines
   "RUF100",
+  # Imported but unused
+  "F401",
 ]
 
 [tool.ruff.per-file-ignores]
 # B011 Do not call assert False since python -O removes these calls
 # F841 local variable 'foo' is assigned to but never used
 # C408 Unnecessary `dict` call
 # E402 Module level import not at top of file
@@ -261,14 +268,16 @@
 # B007 Loop control variable `i` not used within the loop body.
 # N802 Function name `assertIn` should be lowercase
 # EM101 Exception must not use a string literal, assign to variable first
 # PLR2004 Magic value used in comparison
 "tests/*" = ["B011", "F841", "C408", "E402", "T201", "B007", "N802", "EM101", "EM102", "PLR2004"]
 # T201 `print` found
 "*app.py" = ["T201"]
+# F401 `._version.__version__` imported but unused
+"jupyter_client/__init__.py" = ["F401"]
 
 [tool.interrogate]
 ignore-init-module=true
 ignore-private=true
 ignore-semiprivate=true
 ignore-property-decorators=true
 ignore-nested-functions=true
```

### Comparing `jupyter_client-8.1.0/PKG-INFO` & `jupyter_client-8.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: jupyter_client
-Version: 8.1.0
+Version: 8.2.0
 Summary: Jupyter protocol implementation and client libraries
 Project-URL: Homepage, https://jupyter.org
+Project-URL: Documentation, https://jupyter-client.readthedocs.io/
+Project-URL: Source, https://github.com/jupyter/jupyter_client
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
         - Copyright (c) 2001-2015, IPython Development Team
         - Copyright (c) 2015-, Jupyter Development Team
         
         All rights reserved.
@@ -62,30 +64,28 @@
 Requires-Dist: myst-parser; extra == 'docs'
 Requires-Dist: pydata-sphinx-theme; extra == 'docs'
 Requires-Dist: sphinx-autodoc-typehints; extra == 'docs'
 Requires-Dist: sphinx>=4; extra == 'docs'
 Requires-Dist: sphinxcontrib-github-alt; extra == 'docs'
 Requires-Dist: sphinxcontrib-spelling; extra == 'docs'
 Provides-Extra: test
-Requires-Dist: codecov; extra == 'test'
 Requires-Dist: coverage; extra == 'test'
 Requires-Dist: ipykernel>=6.14; extra == 'test'
 Requires-Dist: mypy; extra == 'test'
 Requires-Dist: paramiko; sys_platform == 'win32' and extra == 'test'
 Requires-Dist: pre-commit; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-cov; extra == 'test'
 Requires-Dist: pytest-jupyter[client]>=0.4.1; extra == 'test'
 Requires-Dist: pytest-timeout; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Jupyter Client
 
 [![Build Status](https://github.com/jupyter/jupyter_client/workflows/CI/badge.svg)](https://github.com/jupyter/jupyter_client/actions)
-[![codecov](https://codecov.io/gh/jupyter/jupyter_client/branch/main/graph/badge.svg?token=kxoFu4KnhT)](https://codecov.io/gh/jupyter/jupyter_client)
 [![Documentation Status](https://readthedocs.org/projects/jupyter-client/badge/?version=latest)](http://jupyter-client.readthedocs.io/en/latest/?badge=latest)
 
 `jupyter_client` contains the reference implementation of the [Jupyter protocol].
 It also provides client and kernel management APIs for working with kernels.
 
 It also provides the `jupyter kernelspec` entrypoint
 for installing kernelspecs for use with Jupyter frontends.
```

