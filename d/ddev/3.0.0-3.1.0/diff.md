# Comparing `tmp/ddev-3.0.0.tar.gz` & `tmp/ddev-3.1.0.tar.gz`

## Comparing `ddev-3.0.0.tar` & `ddev-3.1.0.tar`

### file list

```diff
@@ -1,111 +1,111 @@
--rw-r--r--   0        0        0     4533 2020-02-02 00:00:00.000000 ddev-3.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     2893 2020-02-02 00:00:00.000000 ddev-3.0.0/pyoxidizer.bzl
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/py.typed
--rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/__init__.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/application.py
--rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/terminal.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/ci/__init__.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/clean/__init__.py
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/config/__init__.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/docs/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/env/__init__.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/meta/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/meta/scripts/__init__.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/meta/scripts/upgrade_python.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/release/__init__.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/release/agent/__init__.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/release/list_versions/__init__.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/release/show/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/release/stats/__init__.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/status/__init__.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/validate/__init__.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/validate/ci.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/validate/licenses.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/validate/manifest.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/cli/validate/openmetrics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/config/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/config/constants.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/config/file.py
--rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/config/model.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/config/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/integration/__init__.py
--rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/integration/core.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/integration/manifest.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/plugin/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/plugin/api.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/plugin/specs.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/plugin/external/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/plugin/external/starship/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/plugin/external/starship/__main__.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/plugin/external/starship/prompt.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/repo/__init__.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/repo/config.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/repo/constants.py
--rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/repo/core.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/ci.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/fs.py
--rw-r--r--   0        0        0     2601 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/git.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/json.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/network.py
--rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/platform.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/structures.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/toml.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/scripts/__init__.py
--rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/utils/scripts/ci_matrix.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/validation/__init__.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ddev-3.0.0/src/ddev/validation/tracker.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/__init__.py
--rw-r--r--   0        0        0     5865 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/conftest.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/test__utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/clean/__init__.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/clean/test_clean.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/config/__init__.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/config/test_edit.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/config/test_explore.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/config/test_find.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/config/test_restore.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/config/test_set.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/config/test_show.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/meta/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/meta/scripts/__init__.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/meta/scripts/test_upgrade_python.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/release/__init__.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/release/test_list_versions.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/status/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/status/test_status.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/validate/__init__.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/validate/test_licenses.py
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/validate/test_manifest.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/cli/validate/test_openmetrics.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/config/__init__.py
--rw-r--r--   0        0        0    40933 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/config/test_model.py
--rw-r--r--   0        0        0    23688 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/fixtures/network/list_versions/success_datadog_checks_base.yaml
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/fixtures/network/list_versions/success_disk.yaml
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/fixtures/network/manifest/missing_app_uuid.yaml
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/fixtures/network/manifest/success.yaml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/helpers/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/helpers/api.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/integration/test_core.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/integration/test_manifest.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/repo/__init__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/repo/test_config.py
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/repo/test_core.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/utils/__init__.py
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/utils/test_fs.py
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/utils/test_git.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/utils/test_json.py
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/utils/test_platform.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/utils/test_structures.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/validation/__init__.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 ddev-3.0.0/tests/validation/test_tracker.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 ddev-3.0.0/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ddev-3.0.0/README.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ddev-3.0.0/hatch.toml
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 ddev-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 ddev-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 ddev-3.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 ddev-3.1.0/pyoxidizer.bzl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/py.typed
+-rw-r--r--   0        0        0     5416 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/__init__.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/application.py
+-rw-r--r--   0        0        0     7052 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/terminal.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/ci/__init__.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/clean/__init__.py
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/config/__init__.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/docs/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/env/__init__.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/meta/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/meta/scripts/__init__.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/meta/scripts/upgrade_python.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/release/__init__.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/release/agent/__init__.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/release/list_versions/__init__.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/release/show/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/release/stats/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/status/__init__.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/validate/__init__.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/validate/ci.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/validate/licenses.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/validate/manifest.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/cli/validate/openmetrics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/config/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/config/constants.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/config/file.py
+-rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/config/model.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/config/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/integration/__init__.py
+-rw-r--r--   0        0        0     3629 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/integration/core.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/integration/manifest.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/plugin/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/plugin/api.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/plugin/specs.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/plugin/external/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/plugin/external/starship/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/plugin/external/starship/__main__.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/plugin/external/starship/prompt.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/repo/__init__.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/repo/config.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/repo/constants.py
+-rw-r--r--   0        0        0     5191 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/repo/core.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/ci.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/fs.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/git.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/json.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/network.py
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/platform.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/structures.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/toml.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/scripts/__init__.py
+-rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/utils/scripts/ci_matrix.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/validation/__init__.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ddev-3.1.0/src/ddev/validation/tracker.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     6051 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/test__utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/clean/__init__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/clean/test_clean.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/config/__init__.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/config/test_edit.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/config/test_explore.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/config/test_find.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/config/test_restore.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/config/test_set.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/config/test_show.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/meta/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/meta/scripts/__init__.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/meta/scripts/test_upgrade_python.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/release/__init__.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/release/test_list_versions.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/status/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/status/test_status.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/validate/__init__.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/validate/test_licenses.py
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/validate/test_manifest.py
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/cli/validate/test_openmetrics.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/config/__init__.py
+-rw-r--r--   0        0        0    40933 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/config/test_model.py
+-rw-r--r--   0        0        0    23688 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/fixtures/network/list_versions/success_datadog_checks_base.yaml
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/fixtures/network/list_versions/success_disk.yaml
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/fixtures/network/manifest/missing_app_uuid.yaml
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/fixtures/network/manifest/success.yaml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/helpers/api.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     6581 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/integration/test_core.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/integration/test_manifest.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/repo/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/repo/test_config.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/repo/test_core.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/utils/test_fs.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/utils/test_json.py
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/utils/test_platform.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/utils/test_structures.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/validation/__init__.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 ddev-3.1.0/tests/validation/test_tracker.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 ddev-3.1.0/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ddev-3.1.0/README.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 ddev-3.1.0/hatch.toml
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 ddev-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 ddev-3.1.0/PKG-INFO
```

### Comparing `ddev-3.0.0/CHANGELOG.md` & `ddev-3.1.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # CHANGELOG - ddev
 
+## 3.1.0 / 2023-06-23
+
+***Added***:
+
+* Update version of datadog-checks-dev. See [#14865](https://github.com/DataDog/integrations-core/pull/14865).
+* Add Git utilities. See [#14838](https://github.com/DataDog/integrations-core/pull/14838).
+* Add pluggy to ddev dependencies. See [#14821](https://github.com/DataDog/integrations-core/pull/14821).
+
 ## 3.0.0 / 2023-06-20
 
 * [Added] Bump the minimum version of datadog-checks-dev. See [#14785](https://github.com/DataDog/integrations-core/pull/14785).
 * [Added] Upgrade Pydantic model code generator. See [#14779](https://github.com/DataDog/integrations-core/pull/14779).
 * [Added] Use Git for versioning. See [#14778](https://github.com/DataDog/integrations-core/pull/14778).
 * [Added] Add validations for removed dependencies. See [#14556](https://github.com/DataDog/integrations-core/pull/14556).
 * [Added] Migrate `clean` command. See [#14726](https://github.com/DataDog/integrations-core/pull/14726).
```

### Comparing `ddev-3.0.0/pyoxidizer.bzl` & `ddev-3.1.0/pyoxidizer.bzl`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2023-present Datadog, Inc. <dev@datadoghq.com>
 #
 # SPDX-License-Identifier: MIT
 VERSION = VARS["version"]
 APP_NAME = "ddev"
-DISPLAY_NAME = "Datadog Agent integration developer tool"
+DISPLAY_NAME = "ddev"
 AUTHOR = "Datadog, Inc."
 
 
 def make_msi(target):
     if target == "x86_64-pc-windows-msvc":
         arch = "x64"
     elif target == "i686-pc-windows-msvc":
@@ -68,15 +68,15 @@
 
 
 def make_macos_app_bundle():
     # https://gregoryszorc.com/docs/pyoxidizer/main/tugger_starlark_type_macos_application_bundle_builder.html
     bundle = MacOsApplicationBundleBuilder(DISPLAY_NAME)
     bundle.set_info_plist_required_keys(
         display_name=DISPLAY_NAME,
-        identifier="com.datadoghq." + APP_NAME,         
+        identifier="com.datadoghq." + APP_NAME,
         version=VERSION,
         signature=APP_NAME,
         executable=APP_NAME,
     )
 
     # https://gregoryszorc.com/docs/pyoxidizer/main/tugger_starlark_type_apple_universal_binary.html
     universal = AppleUniversalBinary(APP_NAME)
```

### Comparing `ddev-3.0.0/src/ddev/cli/__init__.py` & `ddev-3.1.0/src/ddev/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/application.py` & `ddev-3.1.0/src/ddev/cli/application.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/terminal.py` & `ddev-3.1.0/src/ddev/cli/terminal.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/clean/__init__.py` & `ddev-3.1.0/src/ddev/cli/clean/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/config/__init__.py` & `ddev-3.1.0/src/ddev/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/env/__init__.py` & `ddev-3.1.0/src/ddev/cli/env/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/meta/__init__.py` & `ddev-3.1.0/src/ddev/cli/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/meta/scripts/__init__.py` & `ddev-3.1.0/src/ddev/cli/meta/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/meta/scripts/upgrade_python.py` & `ddev-3.1.0/src/ddev/cli/meta/scripts/upgrade_python.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/release/__init__.py` & `ddev-3.1.0/src/ddev/cli/release/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/release/agent/__init__.py` & `ddev-3.1.0/src/ddev/cli/release/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/release/list_versions/__init__.py` & `ddev-3.1.0/src/ddev/cli/release/list_versions/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/release/show/__init__.py` & `ddev-3.1.0/src/ddev/cli/release/show/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/status/__init__.py` & `ddev-3.1.0/src/ddev/cli/status/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/validate/__init__.py` & `ddev-3.1.0/src/ddev/cli/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/validate/ci.py` & `ddev-3.1.0/src/ddev/cli/validate/ci.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/validate/licenses.py` & `ddev-3.1.0/src/ddev/cli/validate/licenses.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/validate/manifest.py` & `ddev-3.1.0/src/ddev/cli/validate/manifest.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/cli/validate/openmetrics.py` & `ddev-3.1.0/src/ddev/cli/validate/openmetrics.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/config/file.py` & `ddev-3.1.0/src/ddev/config/file.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/config/model.py` & `ddev-3.1.0/src/ddev/config/model.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/config/utils.py` & `ddev-3.1.0/src/ddev/config/utils.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/integration/core.py` & `ddev-3.1.0/src/ddev/integration/core.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/repo/core.py` & `ddev-3.1.0/src/ddev/repo/core.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/utils/fs.py` & `ddev-3.1.0/src/ddev/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/utils/git.py` & `ddev-3.1.0/src/ddev/utils/git.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,18 +7,34 @@
 from functools import cached_property
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from ddev.utils.fs import Path
 
 
+class GitCommit:
+    def __init__(self, sha: str, *, subject: str = ''):
+        self.__sha = sha
+        self.__subject = subject
+
+    @property
+    def sha(self) -> str:
+        return self.__sha
+
+    @property
+    def subject(self) -> str:
+        return self.__subject
+
+
 class GitManager:
     def __init__(self, repo_root: Path):
         self.__repo_root = repo_root
 
+        self.__filtered_tags: dict[str, list[str]] = {}
+
     @property
     def repo_root(self) -> Path:
         return self.__repo_root
 
     @cached_property
     def current_branch(self) -> str:
         return self.capture('rev-parse', '--abbrev-ref', 'HEAD').strip()
@@ -26,14 +42,34 @@
     def get_current_branch(self) -> str:
         with suppress(AttributeError):
             del self.current_branch
 
         return self.current_branch
 
     @cached_property
+    def latest_commit(self) -> GitCommit:
+        return GitCommit(self.capture('rev-parse', 'HEAD').strip())
+
+    def get_latest_commit(self) -> GitCommit:
+        with suppress(AttributeError):
+            del self.latest_commit
+
+        return self.latest_commit
+
+    @cached_property
+    def tags(self) -> list[str]:
+        return sorted(set(self.capture('tag', '--list').splitlines()))
+
+    def get_tags(self) -> list[str]:
+        with suppress(AttributeError):
+            del self.tags
+
+        return self.tags
+
+    @cached_property
     def changed_files(self) -> list[str]:
         changed_files = set()
 
         # Committed e.g.:
         # A   relative/path/to/file.added
         # M   relative/path/to/file.modified
         for line in self.capture('diff', '--name-status', 'origin/master...').splitlines():
@@ -52,14 +88,23 @@
 
     def get_changed_files(self) -> list[str]:
         with suppress(AttributeError):
             del self.changed_files
 
         return self.changed_files
 
+    def filter_tags(self, pattern: str) -> list[str]:
+        import re
+
+        if pattern in self.__filtered_tags:
+            return self.__filtered_tags[pattern]
+
+        tags = self.__filtered_tags[pattern] = [tag for tag in self.tags if re.search(pattern, tag)]
+        return tags
+
     def run(self, *args):
         import subprocess
 
         with self.repo_root.as_cwd():
             try:
                 subprocess.run(['git', *args], check=True)
             except subprocess.CalledProcessError as e:
```

### Comparing `ddev-3.0.0/src/ddev/utils/json.py` & `ddev-3.1.0/src/ddev/utils/json.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/utils/platform.py` & `ddev-3.1.0/src/ddev/utils/platform.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/utils/structures.py` & `ddev-3.1.0/src/ddev/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/utils/scripts/ci_matrix.py` & `ddev-3.1.0/src/ddev/utils/scripts/ci_matrix.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/src/ddev/validation/tracker.py` & `ddev-3.1.0/src/ddev/validation/tracker.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/conftest.py` & `ddev-3.1.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,19 @@
         with self.path.as_cwd():
             # Hard reset
             PLATFORM.check_command_output(['git', 'checkout', '-fB', self.testing_branch, self.original_branch])
 
             # Remove untracked files
             PLATFORM.check_command_output(['git', 'clean', '-fd'])
 
+            # Remove all tags
+            tags_dir = self.path / '.git' / 'refs' / 'tags'
+            if tags_dir.is_dir():
+                tags_dir.remove()
+
     @staticmethod
     def new_branch():
         return os.urandom(10).hex()
 
 
 class CliRunner(__CliRunner):
     def __init__(self, command):
@@ -114,15 +119,17 @@
             yield d
 
 
 @pytest.fixture(scope='session')
 def local_clone(isolation, local_repo) -> Generator[ClonedRepo, None, None]:
     cloned_repo_path = isolation / local_repo.name
 
-    PLATFORM.check_command_output(['git', 'clone', '--local', '--shared', str(local_repo), str(cloned_repo_path)])
+    PLATFORM.check_command_output(
+        ['git', 'clone', '--local', '--shared', '--no-tags', str(local_repo), str(cloned_repo_path)]
+    )
     with cloned_repo_path.as_cwd():
         PLATFORM.check_command_output(['git', 'config', 'user.name', 'Foo Bar'])
         PLATFORM.check_command_output(['git', 'config', 'user.email', 'foo@bar.baz'])
         PLATFORM.check_command_output(['git', 'config', 'commit.gpgsign', 'false'])
 
     cloned_repo = ClonedRepo(cloned_repo_path, 'origin/master', 'ddev-testing')
     cloned_repo.reset_branch()
```

### Comparing `ddev-3.0.0/tests/test__utils.py` & `ddev-3.1.0/tests/test__utils.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/cli/clean/test_clean.py` & `ddev-3.1.0/tests/cli/clean/test_clean.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/cli/config/test_restore.py` & `ddev-3.1.0/tests/cli/config/test_restore.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/cli/config/test_set.py` & `ddev-3.1.0/tests/cli/config/test_set.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/cli/config/test_show.py` & `ddev-3.1.0/tests/cli/config/test_show.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/cli/meta/scripts/test_upgrade_python.py` & `ddev-3.1.0/tests/cli/meta/scripts/test_upgrade_python.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/cli/release/test_list_versions.py` & `ddev-3.1.0/tests/cli/release/test_list_versions.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/cli/status/test_status.py` & `ddev-3.1.0/tests/cli/status/test_status.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/cli/validate/test_licenses.py` & `ddev-3.1.0/tests/cli/validate/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/cli/validate/test_manifest.py` & `ddev-3.1.0/tests/cli/validate/test_manifest.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/cli/validate/test_openmetrics.py` & `ddev-3.1.0/tests/cli/validate/test_openmetrics.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/config/test_model.py` & `ddev-3.1.0/tests/config/test_model.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/fixtures/network/list_versions/success_datadog_checks_base.yaml` & `ddev-3.1.0/tests/fixtures/network/list_versions/success_datadog_checks_base.yaml`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/fixtures/network/list_versions/success_disk.yaml` & `ddev-3.1.0/tests/fixtures/network/list_versions/success_disk.yaml`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/fixtures/network/manifest/missing_app_uuid.yaml` & `ddev-3.1.0/tests/fixtures/network/manifest/missing_app_uuid.yaml`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/fixtures/network/manifest/success.yaml` & `ddev-3.1.0/tests/fixtures/network/manifest/success.yaml`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/helpers/api.py` & `ddev-3.1.0/tests/helpers/api.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/integration/test_core.py` & `ddev-3.1.0/tests/integration/test_core.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/repo/test_core.py` & `ddev-3.1.0/tests/repo/test_core.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/utils/test_fs.py` & `ddev-3.1.0/tests/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/utils/test_git.py` & `ddev-3.1.0/tests/utils/test_git.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,14 +13,51 @@
     repo.git.capture('checkout', '-b', new_branch)
     assert repo.git.current_branch == repository.testing_branch
 
     assert repo.git.get_current_branch() == new_branch
     assert repo.git.current_branch == new_branch
 
 
+def test_get_latest_commit(repository):
+    repo = Repository(repository.path.name, str(repository.path))
+
+    (repo.path / 'test1.txt').touch()
+    repo.git.capture('add', '.')
+    commit_status1 = repo.git.capture('commit', '-m', 'test1')
+    commit1 = repo.git.get_latest_commit()
+    assert len(commit1.sha) == 40
+
+    (repo.path / 'test2.txt').touch()
+    repo.git.capture('add', '.')
+    commit_status2 = repo.git.capture('commit', '-m', 'test2')
+    commit2 = repo.git.get_latest_commit()
+    assert len(commit2.sha) == 40
+
+    short_sha1 = commit1.sha[:7]
+    short_sha2 = commit2.sha[:7]
+
+    assert short_sha1 in commit_status1
+    assert short_sha1 not in commit_status2
+    assert short_sha2 in commit_status2
+    assert short_sha2 not in commit_status1
+
+
+def test_tags(repository):
+    repo = Repository(repository.path.name, str(repository.path))
+
+    assert repo.git.tags == []
+
+    repo.git.capture('tag', 'foo')
+    repo.git.capture('tag', 'bar')
+
+    assert repo.git.tags == []
+    assert repo.git.get_tags() == ['bar', 'foo']
+    assert repo.git.tags == ['bar', 'foo']
+
+
 def test_changed_files(repository):
     repo = Repository(repository.path.name, str(repository.path))
 
     # Committed
     with (repo.path / 'pyproject.toml').open(mode='a') as f:
         f.write('\n')
 
@@ -43,7 +80,17 @@
 
     (zoo_subdir / 'baz.txt').touch()
     assert repo.git.changed_files == changed_files
 
     changed_files.insert(0, 'zoo/sub/baz.txt')
     assert repo.git.get_changed_files() == changed_files
     assert repo.git.changed_files == changed_files
+
+
+def test_filtered_tags(repository):
+    repo = Repository(repository.path.name, str(repository.path))
+
+    repo.git.capture('tag', 'foo')
+    repo.git.capture('tag', 'bar')
+    repo.git.capture('tag', 'baz')
+
+    assert repo.git.filter_tags('^ba') == ['bar', 'baz']
```

### Comparing `ddev-3.0.0/tests/utils/test_json.py` & `ddev-3.1.0/tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/utils/test_platform.py` & `ddev-3.1.0/tests/utils/test_platform.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/utils/test_structures.py` & `ddev-3.1.0/tests/utils/test_structures.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/tests/validation/test_tracker.py` & `ddev-3.1.0/tests/validation/test_tracker.py`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/.gitignore` & `ddev-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/README.md` & `ddev-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ddev-3.0.0/pyproject.toml` & `ddev-3.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,18 +22,19 @@
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
-    "datadog-checks-dev[cli]~=20.0",
+    "datadog-checks-dev[cli]~=21.0",
     "hatch>=1.6.3",
     "httpx",
     "jsonpointer",
+    "pluggy",
     "rich>=12.5.1",
     "tomli; python_version < '3.11'",
     "tomli-w",
     "tomlkit",
 ]
 dynamic = ["version"]
```

### Comparing `ddev-3.0.0/PKG-INFO` & `ddev-3.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: ddev
-Version: 3.0.0
+Version: 3.1.0
 Summary: The Datadog Agent integration developer tool
 Project-URL: Source, https://github.com/DataDog/integrations-core
 Author-email: Datadog <packages@datadoghq.com>
 License-Expression: BSD-3-Clause
 Keywords: agent,datadog,integration
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
-Requires-Dist: datadog-checks-dev[cli]~=20.0
+Requires-Dist: datadog-checks-dev[cli]~=21.0
 Requires-Dist: hatch>=1.6.3
 Requires-Dist: httpx
 Requires-Dist: jsonpointer
+Requires-Dist: pluggy
 Requires-Dist: rich>=12.5.1
 Requires-Dist: tomli-w
 Requires-Dist: tomli; python_version < '3.11'
 Requires-Dist: tomlkit
 Description-Content-Type: text/markdown
 
 # ddev
```

