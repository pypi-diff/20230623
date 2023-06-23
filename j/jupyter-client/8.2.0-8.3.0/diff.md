# Comparing `tmp/jupyter_client-8.2.0.tar.gz` & `tmp/jupyter_client-8.3.0.tar.gz`

## Comparing `jupyter_client-8.2.0.tar` & `jupyter_client-8.3.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
--rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.mailmap
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.readthedocs.yaml
--rw-r--r--   0        0        0    76659 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/RELEASING.md
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.github/workflows/downstream.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.github/workflows/main.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/Makefile
--rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/conf.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/index.rst
--rw-r--r--   0        0        0     8611 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/kernels.rst
--rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/make.bat
--rw-r--r--   0        0        0    64020 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/messaging.rst
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/migration.md
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/pending-kernels.rst
--rw-r--r--   0        0        0    15197 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/provisioning.rst
--rw-r--r--   0        0        0     7302 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/wrapperkernels.rst
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/api/jupyter_client.asynchronous.rst
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/api/jupyter_client.blocking.rst
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/api/jupyter_client.ioloop.rst
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/api/jupyter_client.provisioning.rst
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/api/jupyter_client.rst
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/api/jupyter_client.ssh.rst
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/api/modules.rst
--rw-r--r--   0        0        0   153577 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/figs/frontend-kernel.png
--rw-r--r--   0        0        0   283952 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/docs/figs/frontend-kernel.svg
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/__init__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/_version.py
--rw-r--r--   0        0        0    14381 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/adapter.py
--rw-r--r--   0        0        0    10745 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/channels.py
--rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/channelsabc.py
--rw-r--r--   0        0        0    30383 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/client.py
--rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/clientabc.py
--rw-r--r--   0        0        0    25088 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/connect.py
--rw-r--r--   0        0        0    13841 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/consoleapp.py
--rw-r--r--   0        0        0     5956 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/jsonutil.py
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/kernelapp.py
--rw-r--r--   0        0        0    15109 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/kernelspec.py
--rw-r--r--   0        0        0    11904 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/kernelspecapp.py
--rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/launcher.py
--rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/localinterfaces.py
--rw-r--r--   0        0        0    28686 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/manager.py
--rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/managerabc.py
--rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/multikernelmanager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/py.typed
--rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/restarter.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/runapp.py
--rw-r--r--   0        0        0    37674 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/session.py
--rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/threaded.py
--rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/utils.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/win_interrupt.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/asynchronous/__init__.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/asynchronous/client.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/blocking/__init__.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/blocking/client.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/ioloop/__init__.py
--rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/ioloop/manager.py
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/ioloop/restarter.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/provisioning/__init__.py
--rw-r--r--   0        0        0     9611 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/provisioning/factory.py
--rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/provisioning/local_provisioner.py
--rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/provisioning/provisioner_base.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/ssh/__init__.py
--rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/ssh/forward.py
--rw-r--r--   0        0        0    13004 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/jupyter_client/ssh/tunnel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/__init__.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/conftest.py
--rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/problemkernel.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/signalkernel.py
--rw-r--r--   0        0        0    14444 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_adapter.py
--rw-r--r--   0        0        0     9886 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_client.py
--rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_connect.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_consoleapp.py
--rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_jsonutil.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_kernelapp.py
--rw-r--r--   0        0        0    19981 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_kernelmanager.py
--rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_kernelspec.py
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_kernelspecapp.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_localinterfaces.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_manager.py
--rw-r--r--   0        0        0    23126 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_multikernelmanager.py
--rw-r--r--   0        0        0    11892 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_provisioning.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_public_api.py
--rw-r--r--   0        0        0     8408 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_restarter.py
--rw-r--r--   0        0        0    19845 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_session.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/test_ssh.py
--rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/tests/utils.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/.gitignore
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/LICENSE
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/README.md
--rw-r--r--   0        0        0     6833 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/pyproject.toml
--rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 jupyter_client-8.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/.mailmap
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0    77460 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/RELEASING.md
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/.github/workflows/downstream.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     4930 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/Makefile
+-rw-r--r--   0        0        0    10472 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/conf.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/index.rst
+-rw-r--r--   0        0        0     8611 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/kernels.rst
+-rw-r--r--   0        0        0     7260 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/make.bat
+-rw-r--r--   0        0        0    64020 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/messaging.rst
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/migration.md
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/pending-kernels.rst
+-rw-r--r--   0        0        0    15197 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/provisioning.rst
+-rw-r--r--   0        0        0     7302 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/wrapperkernels.rst
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/api/jupyter_client.asynchronous.rst
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/api/jupyter_client.blocking.rst
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/api/jupyter_client.ioloop.rst
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/api/jupyter_client.provisioning.rst
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/api/jupyter_client.rst
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/api/jupyter_client.ssh.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/api/modules.rst
+-rw-r--r--   0        0        0   153577 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/figs/frontend-kernel.png
+-rw-r--r--   0        0        0   283952 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/docs/figs/frontend-kernel.svg
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/__init__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/_version.py
+-rw-r--r--   0        0        0    14381 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/adapter.py
+-rw-r--r--   0        0        0    10745 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/channels.py
+-rw-r--r--   0        0        0     1120 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/channelsabc.py
+-rw-r--r--   0        0        0    30383 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/client.py
+-rw-r--r--   0        0        0     2347 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/clientabc.py
+-rw-r--r--   0        0        0    25167 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/connect.py
+-rw-r--r--   0        0        0    13841 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/consoleapp.py
+-rw-r--r--   0        0        0     5956 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/jsonutil.py
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/kernelapp.py
+-rw-r--r--   0        0        0    15109 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/kernelspec.py
+-rw-r--r--   0        0        0    11904 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/kernelspecapp.py
+-rw-r--r--   0        0        0     6442 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/launcher.py
+-rw-r--r--   0        0        0     8026 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/localinterfaces.py
+-rw-r--r--   0        0        0    28686 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/manager.py
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/managerabc.py
+-rw-r--r--   0        0        0    19634 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/multikernelmanager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/py.typed
+-rw-r--r--   0        0        0     5652 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/restarter.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/runapp.py
+-rw-r--r--   0        0        0    37674 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/session.py
+-rw-r--r--   0        0        0    10938 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/threaded.py
+-rw-r--r--   0        0        0     3022 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/utils.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/win_interrupt.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/asynchronous/__init__.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/asynchronous/client.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/blocking/__init__.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/blocking/client.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/ioloop/__init__.py
+-rw-r--r--   0        0        0     4045 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/ioloop/manager.py
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/ioloop/restarter.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/provisioning/__init__.py
+-rw-r--r--   0        0        0     9611 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/provisioning/factory.py
+-rw-r--r--   0        0        0     9826 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/provisioning/local_provisioner.py
+-rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/provisioning/provisioner_base.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/ssh/__init__.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/ssh/forward.py
+-rw-r--r--   0        0        0    13004 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/jupyter_client/ssh/tunnel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/__init__.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/conftest.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/problemkernel.py
+-rw-r--r--   0        0        0     2523 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/signalkernel.py
+-rw-r--r--   0        0        0    14444 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_adapter.py
+-rw-r--r--   0        0        0     9886 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_client.py
+-rw-r--r--   0        0        0     9386 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_connect.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_consoleapp.py
+-rw-r--r--   0        0        0     5934 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_jsonutil.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_kernelapp.py
+-rw-r--r--   0        0        0    19981 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_kernelmanager.py
+-rw-r--r--   0        0        0     6808 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_kernelspec.py
+-rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_kernelspecapp.py
+-rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_localinterfaces.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_manager.py
+-rw-r--r--   0        0        0    23126 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_multikernelmanager.py
+-rw-r--r--   0        0        0    11892 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_provisioning.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_public_api.py
+-rw-r--r--   0        0        0     8408 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_restarter.py
+-rw-r--r--   0        0        0    19845 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_session.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/test_ssh.py
+-rw-r--r--   0        0        0     6677 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/tests/utils.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/.gitignore
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/LICENSE
+-rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/README.md
+-rw-r--r--   0        0        0     6906 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/pyproject.toml
+-rw-r--r--   0        0        0     8505 2020-02-02 00:00:00.000000 jupyter_client-8.3.0/PKG-INFO
```

### Comparing `jupyter_client-8.2.0/.mailmap` & `jupyter_client-8.3.0/.mailmap`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/.pre-commit-config.yaml` & `jupyter_client-8.3.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,26 @@
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.22.0
+    rev: 0.23.1
     hooks:
       - id: check-github-workflows
 
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
 
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.260
+    rev: v0.0.270
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `jupyter_client-8.2.0/CHANGELOG.md` & `jupyter_client-8.3.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,29 @@
 # Changes in Jupyter Client {#changelog}
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 8.3.0
+
+([Full Changelog](https://github.com/jupyter/jupyter_client/compare/v8.2.0...bddb8854a4aa3324e128e0497539e17246fbf630))
+
+### Enhancements made
+
+- Allow kwargs when writting connection_file [#953](https://github.com/jupyter/jupyter_client/pull/953) ([@fecet](https://github.com/fecet))
+
+### Maintenance and upkeep improvements
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter/jupyter_client/graphs/contributors?from=2023-04-13&to=2023-06-23&type=c))
+
+[@fecet](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_client+involves%3Afecet+updated%3A2023-04-13..2023-06-23&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_client+involves%3Apre-commit-ci+updated%3A2023-04-13..2023-06-23&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 8.2.0
 
 ([Full Changelog](https://github.com/jupyter/jupyter_client/compare/v8.1.0...dbf6b81fa5ab606eaedc5e8d0843debce18e8746))
 
 ### Enhancements made
 
 - use c.f.Future to wait across threads [#940](https://github.com/jupyter/jupyter_client/pull/940) ([@minrk](https://github.com/minrk))
@@ -17,16 +35,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter/jupyter_client/graphs/contributors?from=2023-03-20&to=2023-04-13&type=c))
 
 [@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_client+involves%3Ablink1073+updated%3A2023-03-20..2023-04-13&type=Issues) | [@fcollonval](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_client+involves%3Afcollonval+updated%3A2023-03-20..2023-04-13&type=Issues) | [@minrk](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_client+involves%3Aminrk+updated%3A2023-03-20..2023-04-13&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fjupyter_client+involves%3Apre-commit-ci+updated%3A2023-03-20..2023-04-13&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 8.1.0
 
 ([Full Changelog](https://github.com/jupyter/jupyter_client/compare/v8.0.3...e3ac7a69355dd1af66038eda767e51e92ef034fb))
 
 ### Bugs fixed
 
 - ThreadedZMQStream: close stream before socket [#936](https://github.com/jupyter/jupyter_client/pull/936) ([@minrk](https://github.com/minrk))
```

### Comparing `jupyter_client-8.2.0/RELEASING.md` & `jupyter_client-8.3.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/.github/workflows/downstream.yml` & `jupyter_client-8.3.0/.github/workflows/downstream.yml`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/.github/workflows/main.yml` & `jupyter_client-8.3.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/.github/workflows/prep-release.yml` & `jupyter_client-8.3.0/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/.github/workflows/publish-release.yml` & `jupyter_client-8.3.0/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/docs/Makefile` & `jupyter_client-8.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/docs/conf.py` & `jupyter_client-8.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/docs/index.rst` & `jupyter_client-8.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/docs/kernels.rst` & `jupyter_client-8.3.0/docs/kernels.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/docs/make.bat` & `jupyter_client-8.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/docs/messaging.rst` & `jupyter_client-8.3.0/docs/messaging.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/docs/migration.md` & `jupyter_client-8.3.0/docs/migration.md`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/docs/pending-kernels.rst` & `jupyter_client-8.3.0/docs/pending-kernels.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/docs/provisioning.rst` & `jupyter_client-8.3.0/docs/provisioning.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/docs/wrapperkernels.rst` & `jupyter_client-8.3.0/docs/wrapperkernels.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/docs/api/jupyter_client.provisioning.rst` & `jupyter_client-8.3.0/docs/api/jupyter_client.provisioning.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/docs/api/jupyter_client.rst` & `jupyter_client-8.3.0/docs/api/jupyter_client.rst`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/docs/figs/frontend-kernel.png` & `jupyter_client-8.3.0/docs/figs/frontend-kernel.png`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/docs/figs/frontend-kernel.svg` & `jupyter_client-8.3.0/docs/figs/frontend-kernel.svg`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/__init__.py` & `jupyter_client-8.3.0/jupyter_client/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/_version.py` & `jupyter_client-8.3.0/jupyter_client/_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """The version information for jupyter client."""
 import re
 from typing import List, Union
 
-__version__ = "8.2.0"
+__version__ = "8.3.0"
 
 # Build up version_info tuple for backwards compatibility
 pattern = r'(?P<major>\d+).(?P<minor>\d+).(?P<patch>\d+)(?P<rest>.*)'
 match = re.match(pattern, __version__)
 if match:
     parts: List[Union[int, str]] = [int(match[part]) for part in ['major', 'minor', 'patch']]
     if match['rest']:
```

### Comparing `jupyter_client-8.2.0/jupyter_client/adapter.py` & `jupyter_client-8.3.0/jupyter_client/adapter.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/channels.py` & `jupyter_client-8.3.0/jupyter_client/channels.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/channelsabc.py` & `jupyter_client-8.3.0/jupyter_client/channelsabc.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/client.py` & `jupyter_client-8.3.0/jupyter_client/client.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/clientabc.py` & `jupyter_client-8.3.0/jupyter_client/clientabc.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/connect.py` & `jupyter_client-8.3.0/jupyter_client/connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     hb_port: int = 0,
     control_port: int = 0,
     ip: str = "",
     key: bytes = b"",
     transport: str = "tcp",
     signature_scheme: str = "hmac-sha256",
     kernel_name: str = "",
+    **kwargs: Any,
 ) -> Tuple[str, KernelConnectionInfo]:
     """Generates a JSON config file, including the selection of random ports.
 
     Parameters
     ----------
 
     fname : unicode
@@ -136,14 +137,15 @@
         "hb_port": hb_port,
     }
     cfg["ip"] = ip
     cfg["key"] = key.decode()
     cfg["transport"] = transport
     cfg["signature_scheme"] = signature_scheme
     cfg["kernel_name"] = kernel_name
+    cfg.update(kwargs)
 
     # Only ever write this file as user read/writeable
     # This would otherwise introduce a vulnerability as a file has secrets
     # which would let others execute arbitrary code as you
     with secure_write(fname) as f:
         f.write(json.dumps(cfg, indent=2))
 
@@ -479,15 +481,15 @@
             return
 
         for name in self._random_port_names:
             setattr(self, name, 0)
 
         self.cleanup_connection_file()
 
-    def write_connection_file(self) -> None:
+    def write_connection_file(self, **kwargs: Any) -> None:
         """Write connection info to JSON dict in self.connection_file."""
         if self._connection_file_written and os.path.exists(self.connection_file):
             return
 
         self.connection_file, cfg = write_connection_file(
             self.connection_file,
             transport=self.transport,
@@ -496,14 +498,15 @@
             stdin_port=self.stdin_port,
             iopub_port=self.iopub_port,
             shell_port=self.shell_port,
             hb_port=self.hb_port,
             control_port=self.control_port,
             signature_scheme=self.session.signature_scheme,
             kernel_name=self.kernel_name,
+            **kwargs,
         )
         # write_connection_file also sets default ports:
         self._record_random_port_names()
         for name in port_names:
             setattr(self, name, cfg[name])
 
         self._connection_file_written = True
```

### Comparing `jupyter_client-8.2.0/jupyter_client/consoleapp.py` & `jupyter_client-8.3.0/jupyter_client/consoleapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/jsonutil.py` & `jupyter_client-8.3.0/jupyter_client/jsonutil.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/kernelapp.py` & `jupyter_client-8.3.0/jupyter_client/kernelapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/kernelspec.py` & `jupyter_client-8.3.0/jupyter_client/kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/kernelspecapp.py` & `jupyter_client-8.3.0/jupyter_client/kernelspecapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/launcher.py` & `jupyter_client-8.3.0/jupyter_client/launcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         kwargs["start_new_session"] = True
         if not independent:
             env["JPY_PARENT_PID"] = str(os.getpid())
 
     try:
         # Allow to use ~/ in the command or its arguments
         cmd = [os.path.expanduser(s) for s in cmd]
-        proc = Popen(cmd, **kwargs)
+        proc = Popen(cmd, **kwargs)  # noqa
     except Exception as ex:
         try:
             msg = "Failed to run command:\n{}\n    PATH={!r}\n    with kwargs:\n{!r}\n"
             # exclude environment variables,
             # which may contain access tokens and the like.
             without_env = {key: value for key, value in kwargs.items() if key != "env"}
             msg = msg.format(cmd, env.get("PATH", os.defpath), without_env)
```

### Comparing `jupyter_client-8.2.0/jupyter_client/localinterfaces.py` & `jupyter_client-8.3.0/jupyter_client/localinterfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 def _get_output(cmd):
     """Get output of a command, raising IOError if it fails"""
     startupinfo = None
     if os.name == "nt":
         startupinfo = subprocess.STARTUPINFO()  # type:ignore[attr-defined]
         startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW  # type:ignore[attr-defined]
-    p = Popen(cmd, stdout=PIPE, stderr=PIPE, startupinfo=startupinfo)
+    p = Popen(cmd, stdout=PIPE, stderr=PIPE, startupinfo=startupinfo)  # noqa
     stdout, stderr = p.communicate()
     if p.returncode:
         msg = "Failed to run {}: {}".format(cmd, stderr.decode("utf8", "replace"))
         raise OSError(msg)
     return stdout.decode("utf8", "replace")
```

### Comparing `jupyter_client-8.2.0/jupyter_client/manager.py` & `jupyter_client-8.3.0/jupyter_client/manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/managerabc.py` & `jupyter_client-8.3.0/jupyter_client/managerabc.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/multikernelmanager.py` & `jupyter_client-8.3.0/jupyter_client/multikernelmanager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/restarter.py` & `jupyter_client-8.3.0/jupyter_client/restarter.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/runapp.py` & `jupyter_client-8.3.0/jupyter_client/runapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/session.py` & `jupyter_client-8.3.0/jupyter_client/session.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/threaded.py` & `jupyter_client-8.3.0/jupyter_client/threaded.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/utils.py` & `jupyter_client-8.3.0/jupyter_client/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/win_interrupt.py` & `jupyter_client-8.3.0/jupyter_client/win_interrupt.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/asynchronous/client.py` & `jupyter_client-8.3.0/jupyter_client/asynchronous/client.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/blocking/client.py` & `jupyter_client-8.3.0/jupyter_client/blocking/client.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/ioloop/manager.py` & `jupyter_client-8.3.0/jupyter_client/ioloop/manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/ioloop/restarter.py` & `jupyter_client-8.3.0/jupyter_client/ioloop/restarter.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/provisioning/factory.py` & `jupyter_client-8.3.0/jupyter_client/provisioning/factory.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/provisioning/local_provisioner.py` & `jupyter_client-8.3.0/jupyter_client/provisioning/local_provisioner.py`

 * *Files 3% similar despite different names*

```diff
@@ -182,16 +182,19 @@
                 lpc = LocalPortCache.instance()
                 km.shell_port = lpc.find_available_port(km.ip)
                 km.iopub_port = lpc.find_available_port(km.ip)
                 km.stdin_port = lpc.find_available_port(km.ip)
                 km.hb_port = lpc.find_available_port(km.ip)
                 km.control_port = lpc.find_available_port(km.ip)
                 self.ports_cached = True
-
-            km.write_connection_file()
+            if 'env' in kwargs:
+                jupyter_session = kwargs['env'].get("JPY_SESSION_NAME", "")
+                km.write_connection_file(jupyter_session=jupyter_session)
+            else:
+                km.write_connection_file()
             self.connection_info = km.get_connection_info()
 
             kernel_cmd = km.format_kernel_cmd(
                 extra_arguments=extra_arguments
             )  # This needs to remain here for b/c
         else:
             extra_arguments = kwargs.pop('extra_arguments', [])
```

### Comparing `jupyter_client-8.2.0/jupyter_client/provisioning/provisioner_base.py` & `jupyter_client-8.3.0/jupyter_client/provisioning/provisioner_base.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/jupyter_client/ssh/forward.py` & `jupyter_client-8.3.0/jupyter_client/ssh/forward.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,16 +58,15 @@
             logger.debug(
                 "Incoming request to %s:%d was rejected by the SSH server."
                 % (self.chain_host, self.chain_port)
             )
             return
 
         logger.debug(
-            "Connected!  Tunnel open %r -> %r -> %r"
-            % (
+            "Connected!  Tunnel open {!r} -> {!r} -> {!r}".format(
                 self.request.getpeername(),
                 chan.getpeername(),
                 (self.chain_host, self.chain_port),
             )
         )
         while True:
             r, w, x = select.select([self.request, chan], [], [])
```

### Comparing `jupyter_client-8.2.0/jupyter_client/ssh/tunnel.py` & `jupyter_client-8.3.0/jupyter_client/ssh/tunnel.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/problemkernel.py` & `jupyter_client-8.3.0/tests/problemkernel.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/signalkernel.py` & `jupyter_client-8.3.0/tests/signalkernel.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     ):
         code = code.strip()
         reply: dict = {
             "status": "ok",
             "user_expressions": {},
         }
         if code == "start":
-            child = Popen(["bash", "-i", "-c", "sleep 30"], stderr=PIPE)
+            child = Popen(["bash", "-i", "-c", "sleep 30"], stderr=PIPE)  # noqa
             self.children.append(child)
             reply["user_expressions"]["pid"] = self.children[-1].pid
         elif code == "check":
             reply["user_expressions"]["poll"] = [child.poll() for child in self.children]
         elif code == "env":
             reply["user_expressions"]["env"] = os.getenv("TEST_VARS", "")
         elif code == "sleep":
```

### Comparing `jupyter_client-8.2.0/tests/test_adapter.py` & `jupyter_client-8.3.0/tests/test_adapter.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/test_client.py` & `jupyter_client-8.3.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/test_connect.py` & `jupyter_client-8.3.0/tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/test_consoleapp.py` & `jupyter_client-8.3.0/tests/test_consoleapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/test_jsonutil.py` & `jupyter_client-8.3.0/tests/test_jsonutil.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/test_kernelapp.py` & `jupyter_client-8.3.0/tests/test_kernelapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/test_kernelmanager.py` & `jupyter_client-8.3.0/tests/test_kernelmanager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/test_kernelspec.py` & `jupyter_client-8.3.0/tests/test_kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/test_kernelspecapp.py` & `jupyter_client-8.3.0/tests/test_kernelspecapp.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/test_localinterfaces.py` & `jupyter_client-8.3.0/tests/test_localinterfaces.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/test_manager.py` & `jupyter_client-8.3.0/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/test_multikernelmanager.py` & `jupyter_client-8.3.0/tests/test_multikernelmanager.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/test_provisioning.py` & `jupyter_client-8.3.0/tests/test_provisioning.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/test_public_api.py` & `jupyter_client-8.3.0/tests/test_public_api.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/test_restarter.py` & `jupyter_client-8.3.0/tests/test_restarter.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/test_session.py` & `jupyter_client-8.3.0/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/tests/utils.py` & `jupyter_client-8.3.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/LICENSE` & `jupyter_client-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/README.md` & `jupyter_client-8.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_client-8.2.0/pyproject.toml` & `jupyter_client-8.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -107,15 +107,15 @@
 [tool.hatch.envs.typing.scripts]
 test = "mypy --install-types --non-interactive {args:.}"
 
 [tool.hatch.envs.lint]
 dependencies = [
   "black[jupyter]==23.3.0",
   "mdformat>0.7",
-  "ruff==0.0.260",
+  "ruff==0.0.270",
 ]
 [tool.hatch.envs.lint.scripts]
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
   "mdformat --check {args:docs *.md}"
 ]
@@ -265,15 +265,16 @@
 # C408 Unnecessary `dict` call
 # E402 Module level import not at top of file
 # T201 `print` found
 # B007 Loop control variable `i` not used within the loop body.
 # N802 Function name `assertIn` should be lowercase
 # EM101 Exception must not use a string literal, assign to variable first
 # PLR2004 Magic value used in comparison
-"tests/*" = ["B011", "F841", "C408", "E402", "T201", "B007", "N802", "EM101", "EM102", "PLR2004"]
+# S603 `subprocess` call: check for execution of untrusted input
+"tests/*" = ["B011", "F841", "C408", "E402", "T201", "B007", "N802", "EM101", "EM102", "PLR2004", "S603"]
 # T201 `print` found
 "*app.py" = ["T201"]
 # F401 `._version.__version__` imported but unused
 "jupyter_client/__init__.py" = ["F401"]
 
 [tool.interrogate]
 ignore-init-module=true
```

### Comparing `jupyter_client-8.2.0/PKG-INFO` & `jupyter_client-8.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_client
-Version: 8.2.0
+Version: 8.3.0
 Summary: Jupyter protocol implementation and client libraries
 Project-URL: Homepage, https://jupyter.org
 Project-URL: Documentation, https://jupyter-client.readthedocs.io/
 Project-URL: Source, https://github.com/jupyter/jupyter_client
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
```

