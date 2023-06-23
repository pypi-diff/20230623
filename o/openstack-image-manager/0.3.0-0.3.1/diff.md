# Comparing `tmp/openstack-image-manager-0.3.0.tar.gz` & `tmp/openstack-image-manager-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstack-image-manager-0.3.0.tar", last modified: Mon Jun 12 17:22:08 2023, max compression
+gzip compressed data, was "openstack-image-manager-0.3.1.tar", last modified: Fri Jun 23 21:33:32 2023, max compression
```

## Comparing `openstack-image-manager-0.3.0.tar` & `openstack-image-manager-0.3.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.clouds.yml
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.660799 openstack-image-manager-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/renovate.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.660799 openstack-image-manager-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/build-container-image.yml
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/mirror-images-dry-run.yml
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/mirror-images.yml
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/run-unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/test-python-setup.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/update-images.yml
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.github/workflows/validate-configuration.yml
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.yamllint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/.zuul.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/Containerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    40761 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/clouds.yml.sample
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.664799 openstack-image-manager-0.3.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/configuration.md
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/getting_started.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.664799 openstack-image-manager-0.3.0/doc/images/
--rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/overview.md
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/requirements.md
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/doc/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.664799 openstack-image-manager-0.3.0/etc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.664799 openstack-image-manager-0.3.0/etc/images/
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/almalinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/centos.yml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/cirros.yml
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/clearlinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/debian.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/fedora.yml
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/flatcar.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/gardenlinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/kubernetes.yml
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/octavia.yml
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/opensuse.yml
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/opnsense.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/rockylinux.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/talos.yml
--rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/images/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/etc/schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.664799 openstack-image-manager-0.3.0/openstack_image_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/openstack_image_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47634 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/openstack_image_manager/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/openstack_image_manager/mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/openstack_image_manager/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/openstack_image_manager/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.664799 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-12 17:22:08.000000 openstack-image-manager-0.3.0/openstack_image_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/playbooks/integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/playbooks/pre-integration-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/playbooks/pre-real-world.yml
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/playbooks/real-world.yml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      723 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/scripts/build.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      477 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/scripts/push.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/secure.yml.sample
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/test/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/test/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/test/integration/fixtures/test_image.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/test/integration/test_manage_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 17:22:08.668799 openstack-image-manager-0.3.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/test/unit/test_manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-12 17:21:58.000000 openstack-image-manager-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.723476 openstack-image-manager-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.clouds.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.711475 openstack-image-manager-0.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/renovate.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.715475 openstack-image-manager-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/build-container-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/mirror-images-dry-run.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/mirror-images.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/run-unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/test-python-setup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/update-images.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.github/workflows/validate-configuration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.yamllint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/.zuul.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/Containerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-23 21:33:32.723476 openstack-image-manager-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    40597 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/clouds.yml.sample
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.715475 openstack-image-manager-0.3.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/configuration.md
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/getting_started.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.715475 openstack-image-manager-0.3.1/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/overview.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/requirements.md
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/doc/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.715475 openstack-image-manager-0.3.1/etc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/etc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/almalinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/centos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/cirros.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/clearlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/debian.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/fedora.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/flatcar.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/gardenlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/kubernetes.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/octavia.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/opensuse.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/opnsense.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/rockylinux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/talos.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     9047 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/images/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/etc/schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/openstack_image_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/openstack_image_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47634 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/openstack_image_manager/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/openstack_image_manager/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/openstack_image_manager/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8434 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/openstack_image_manager/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 21:33:32.000000 openstack-image-manager-0.3.1/openstack_image_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/playbooks/integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/playbooks/pre-integration-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/playbooks/pre-real-world.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/playbooks/real-world.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      723 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/scripts/build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      477 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/scripts/push.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/secure.yml.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-06-23 21:33:32.723476 openstack-image-manager-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/test/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/test/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/test/integration/fixtures/test_image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/test/integration/test_manage_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:32.719475 openstack-image-manager-0.3.1/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/test/unit/test_manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-23 21:33:21.000000 openstack-image-manager-0.3.1/tox.ini
```

### Comparing `openstack-image-manager-0.3.0/.github/workflows/build-container-image.yml` & `openstack-image-manager-0.3.1/.github/workflows/build-container-image.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/.github/workflows/mirror-images-dry-run.yml` & `openstack-image-manager-0.3.1/.github/workflows/mirror-images-dry-run.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/.github/workflows/mirror-images.yml` & `openstack-image-manager-0.3.1/.github/workflows/mirror-images.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/.github/workflows/publish.yml` & `openstack-image-manager-0.3.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/.github/workflows/run-unit-tests.yml` & `openstack-image-manager-0.3.1/.github/workflows/run-unit-tests.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/.github/workflows/test-python-setup.yml` & `openstack-image-manager-0.3.1/.github/workflows/test-python-setup.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/.github/workflows/update-images.yml` & `openstack-image-manager-0.3.1/.github/workflows/update-images.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/.github/workflows/validate-configuration.yml` & `openstack-image-manager-0.3.1/.github/workflows/validate-configuration.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/.zuul.yaml` & `openstack-image-manager-0.3.1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/Containerfile` & `openstack-image-manager-0.3.1/Containerfile`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/Dockerfile` & `openstack-image-manager-0.3.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/LICENSE` & `openstack-image-manager-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/PKG-INFO` & `openstack-image-manager-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstack-image-manager
-Version: 0.3.0
+Version: 0.3.1
 Summary: OpenStack image manager
 Home-page: https://github.com/osism/openstack-image-manager
 Author: OSISM community
 Author-email: info@osism.tech
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `openstack-image-manager-0.3.0/Pipfile.lock` & `openstack-image-manager-0.3.1/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9806327160493827%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'a979a09d5096c774f26ccb5c6f299ee4dccab28428a004599c5938cda1afc17b'}}",*

 * * "'default'": "{'cryptography': {'hashes': "*

 * *              "['sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db', "*

 * *              "'sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a', "*

 * *              "'sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039', "*

 * *              "'sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "5815d8516002d1097aa337a720f60a3ed7025e766d2111f9c163db86f84da742"
+            "sha256": "a979a09d5096c774f26ccb5c6f299ee4dccab28428a004599c5938cda1afc17b"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.9"
         },
         "sources": [
             {
@@ -221,36 +221,36 @@
                 "sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44",
                 "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
             "version": "==0.4.6"
         },
         "cryptography": {
             "hashes": [
-                "sha256:0ddaee209d1cf1f180f1efa338a68c4621154de0afaef92b89486f5f96047c55",
-                "sha256:14754bcdae909d66ff24b7b5f166d69340ccc6cb15731670435efd5719294895",
-                "sha256:344c6de9f8bda3c425b3a41b319522ba3208551b70c2ae00099c205f0d9fd3be",
-                "sha256:34d405ea69a8b34566ba3dfb0521379b210ea5d560fafedf9f800a9a94a41928",
-                "sha256:3680248309d340fda9611498a5319b0193a8dbdb73586a1acf8109d06f25b92d",
-                "sha256:3c5ef25d060c80d6d9f7f9892e1d41bb1c79b78ce74805b8cb4aa373cb7d5ec8",
-                "sha256:4ab14d567f7bbe7f1cdff1c53d5324ed4d3fc8bd17c481b395db224fb405c237",
-                "sha256:5c1f7293c31ebc72163a9a0df246f890d65f66b4a40d9ec80081969ba8c78cc9",
-                "sha256:6b71f64beeea341c9b4f963b48ee3b62d62d57ba93eb120e1196b31dc1025e78",
-                "sha256:7d92f0248d38faa411d17f4107fc0bce0c42cae0b0ba5415505df72d751bf62d",
-                "sha256:8362565b3835ceacf4dc8f3b56471a2289cf51ac80946f9087e66dc283a810e0",
-                "sha256:84a165379cb9d411d58ed739e4af3396e544eac190805a54ba2e0322feb55c46",
-                "sha256:88ff107f211ea696455ea8d911389f6d2b276aabf3231bf72c8853d22db755c5",
-                "sha256:9f65e842cb02550fac96536edb1d17f24c0a338fd84eaf582be25926e993dde4",
-                "sha256:a4fc68d1c5b951cfb72dfd54702afdbbf0fb7acdc9b7dc4301bbf2225a27714d",
-                "sha256:b7f2f5c525a642cecad24ee8670443ba27ac1fab81bba4cc24c7b6b41f2d0c75",
-                "sha256:b846d59a8d5a9ba87e2c3d757ca019fa576793e8758174d3868aecb88d6fc8eb",
-                "sha256:bf8fc66012ca857d62f6a347007e166ed59c0bc150cefa49f28376ebe7d992a2",
-                "sha256:f5d0bf9b252f30a31664b6f64432b4730bb7038339bd18b1fafe129cfc2be9be"
+                "sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db",
+                "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a",
+                "sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039",
+                "sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c",
+                "sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3",
+                "sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485",
+                "sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c",
+                "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca",
+                "sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5",
+                "sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5",
+                "sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3",
+                "sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb",
+                "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43",
+                "sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31",
+                "sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc",
+                "sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b",
+                "sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006",
+                "sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a",
+                "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==41.0.0"
+            "version": "==41.0.1"
         },
         "decorator": {
             "hashes": [
                 "sha256:637996211036b6385ef91435e4fae22989472f9d571faba8927ba8253acbc330",
                 "sha256:b8c3f85900b9dc423225913c5aace94729fe1fa9763b38939a95226f02d37186"
             ],
             "markers": "python_version >= '3.5'",
@@ -270,67 +270,65 @@
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
         "iso8601": {
             "hashes": [
-                "sha256:32811e7b81deee2063ea6d2e94f8819a86d1f3811e49d23623a41fa832bef03f",
-                "sha256:8400e90141bf792bce2634df533dc57e3bee19ea120a87bebcd3da89a58ad73f"
+                "sha256:739960d37c74c77bd9bd546a76562ccb581fe3d4820ff5c3141eb49c839fda8f",
+                "sha256:ebe10061b932edb8a8e33cc635d661926c59b9c3bed7a4f4edca8c62d400af10"
             ],
-            "markers": "python_version < '4.0' and python_full_version >= '3.6.2'",
-            "version": "==1.1.0"
+            "markers": "python_version >= '3.7' and python_version < '4.0'",
+            "version": "==2.0.0"
         },
         "jmespath": {
             "hashes": [
                 "sha256:02e2e4cc71b5bcab88332eebf907519190dd9e6e82107fa7f83b1003a6252980",
                 "sha256:90261b206d6defd58fdd5e85f478bf633a2901798906be2ad389150c5c60edbe"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.1"
         },
         "jsonpatch": {
             "hashes": [
-                "sha256:26ac385719ac9f54df8a2f0827bb8253aa3ea8ab7b3368457bcdb8c14595a397",
-                "sha256:b6ddfe6c3db30d81a96aaeceb6baf916094ffa23d7dd5fa2c13e13f8b6e600c2"
+                "sha256:0ae28c0cd062bbd8b8ecc26d7d164fbbea9652a1a3693f3b956c1eae5145dade"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'",
-            "version": "==1.32"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
+            "version": "==1.33"
         },
         "jsonpointer": {
             "hashes": [
-                "sha256:51801e558539b4e9cd268638c078c6c5746c9ac96bc38152d443400e4f3793e9",
-                "sha256:97cba51526c829282218feb99dab1b1e6bdf8efd1c43dc9d57be093c0d69c99a"
+                "sha256:15d51bba20eea3165644553647711d150376234112651b4f1811022aecad7d7a"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==2.3"
+            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
+            "version": "==2.4"
         },
         "keystoneauth1": {
             "hashes": [
-                "sha256:84feba003301c2042693eb9366b0008eabd47b221c65f8106f0049f54eba989d",
-                "sha256:af54bcb9cf3b5d8492894ff8b6680447c8ef1fb880734a5d3ce3a78ed8459844"
+                "sha256:d2fcfdcfe347df8d92390e0806b4969289d884cd9ec3519e4c5aec53e66d0767",
+                "sha256:f79b1c27ed5a69be4d03a5bc4967df3dfab0c5d76e85226fa2060cffadff74a1"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==5.2.0"
+            "version": "==5.2.1"
         },
         "loguru": {
             "hashes": [
                 "sha256:1612053ced6ae84d7959dd7d5e431a0532642237ec21f7fd83ac73fe539e03e1",
                 "sha256:b93aa30099fa6860d4727f1b81f8718e965bb96253fa190fab2077aaad6d15d3"
             ],
             "index": "pypi",
             "version": "==0.7.0"
         },
         "markdown-it-py": {
             "hashes": [
-                "sha256:5a35f8d1870171d9acc47b99612dc146129b631baf04970128b568f190d0cc30",
-                "sha256:7c9a5e412688bc771c67432cbfebcdd686c93ce6484913dccf06cb5a0bea35a1"
+                "sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1",
+                "sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb"
             ],
-            "markers": "python_version >= '3.7'",
-            "version": "==2.2.0"
+            "markers": "python_version >= '3.8'",
+            "version": "==3.0.0"
         },
         "mdurl": {
             "hashes": [
                 "sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8",
                 "sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba"
             ],
             "markers": "python_version >= '3.7'",
@@ -350,19 +348,19 @@
                 "sha256:5284603030c00906d9d64d8108728c004fbeb91fc1c1e4caca342bc48f2a6dfd"
             ],
             "index": "pypi",
             "version": "==3.0.0"
         },
         "natsort": {
             "hashes": [
-                "sha256:517595492dde570a4fd6b6a76f644440c1ba51e2338c8a671d7f0475fda8f9fd",
-                "sha256:d583bc9050dd10538de36297c960b93f873f0cd01671a3c50df5bd86dd391dcb"
+                "sha256:45312c4a0e5507593da193dedd04abb1469253b601ecaf63445ad80f0a1ea581",
+                "sha256:4732914fb471f56b5cce04d7bae6f164a592c7712e1c85f9ef585e197299521c"
             ],
             "index": "pypi",
-            "version": "==8.3.1"
+            "version": "==8.4.0"
         },
         "netifaces": {
             "hashes": [
                 "sha256:043a79146eb2907edf439899f262b3dfe41717d34124298ed281139a8b93ca32",
                 "sha256:08e3f102a59f9eaef70948340aeb6c89bd09734e0dca0f3b82720305729f63ea",
                 "sha256:0f6133ac02521270d9f7c490f0c8c60638ff4aec8338efeff10a1b51506abe85",
                 "sha256:18917fbbdcb2d4f897153c5ddbb56b31fa6dd7c3fa9608b7e3c3a663df8206b5",
@@ -393,19 +391,19 @@
                 "sha256:e76c7f351e0444721e85f975ae92718e21c1f361bda946d60a214061de1f00a1",
                 "sha256:eb4813b77d5df99903af4757ce980a98c4d702bbcb81f32a0b305a1537bdf0b1"
             ],
             "version": "==0.11.0"
         },
         "openstacksdk": {
             "hashes": [
-                "sha256:bc4b340fde80503b839bda72a32eb7d630ccde5c2c1ff4952840d79fca5bce7f",
-                "sha256:d73b5b9825b14230d8faca0acc9dbbfacf1299eb8eceae1f0f6900ed17aede6e"
+                "sha256:207a75e5a81e1173bf251e9976965a66ff2ff379d0a0ba55a4903dcf2b5c1974",
+                "sha256:42afb8435b137905f7733f89a6627b7604f92adea7d49b3e22826c66e6062859"
             ],
             "index": "pypi",
-            "version": "==1.2.0"
+            "version": "==1.3.0"
         },
         "os-service-types": {
             "hashes": [
                 "sha256:0505c72205690910077fb72b88f2a1f07533c8d39f2fe75b29583481764965d6",
                 "sha256:31800299a82239363995b91f1ebf9106ac7758542a1e4ef6dc737a5932878c6c"
             ],
             "version": "==1.7.0"
@@ -524,26 +522,26 @@
                 "sha256:3083d872b6e07dc5c323563ef37671d992214ad9a32b0ca4a3d7f5500bf38ce3",
                 "sha256:b095cbc77618f066d459a02b137b020c37da9f46d9b057704019c9f77dba3065"
             ],
             "version": "==1.4.0"
         },
         "rich": {
             "hashes": [
-                "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
-                "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
+                "sha256:8f87bc7ee54675732fa66a05ebfe489e27264caeeff3728c945d25971b6485ec",
+                "sha256:d653d6bccede5844304c605d5aac802c7cf9621efd700b46c7ec2b51ea914898"
             ],
-            "version": "==13.3.5"
+            "version": "==13.4.2"
         },
         "ruamel.yaml": {
             "hashes": [
-                "sha256:098ed1eb6d338a684891a72380277c1e6fc4d4ae0e120de9a447275056dda335",
-                "sha256:3cf153f0047ced526e723097ac615d3009371779432e304dbd5596b6f3a4c777"
+                "sha256:23cd2ed620231677564646b0c6a89d138b6822a0d78656df7abda5879ec4f447",
+                "sha256:ec939063761914e14542972a5cba6d33c23b0859ab6342f61cf070cfc600efc2"
             ],
             "index": "pypi",
-            "version": "==0.17.31"
+            "version": "==0.17.32"
         },
         "ruamel.yaml.clib": {
             "hashes": [
                 "sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e",
                 "sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3",
                 "sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5",
                 "sha256:1a6391a7cabb7641c32517539ca42cf84b87b667bad38b78d4d42dd23e957c81",
@@ -625,27 +623,27 @@
                 "sha256:5d96d986a21493606a358cae4461bd8cdf83cbf33a5aa950ae629ca3b51467ee"
             ],
             "index": "pypi",
             "version": "==0.9.0"
         },
         "typing-extensions": {
             "hashes": [
-                "sha256:06006244c70ac8ee83fa8282cb188f697b8db25bc8b4df07be1873c43897060c",
-                "sha256:3a8b36f13dd5fdc5d1b16fe317f5668545de77fa0b8e02006381fd49d731ab98"
+                "sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26",
+                "sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==4.6.2"
+            "version": "==4.6.3"
         },
         "urllib3": {
             "hashes": [
-                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
-                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
+                "sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1",
+                "sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.0.2"
+            "version": "==2.0.3"
         },
         "yamale": {
             "hashes": [
                 "sha256:04f914c0886bda03ac20f8468272cfd9374a634a062549490eff2beedeb30497",
                 "sha256:e524caf71cbbbd15aa295e8bdda01688ac4b5edaf38dd60851ddff6baef383ba"
             ],
             "index": "pypi",
```

### Comparing `openstack-image-manager-0.3.0/doc/conf.py` & `openstack-image-manager-0.3.1/doc/conf.py`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/doc/configuration.md` & `openstack-image-manager-0.3.1/doc/configuration.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/doc/contribute.md` & `openstack-image-manager-0.3.1/doc/contribute.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/doc/getting_started.md` & `openstack-image-manager-0.3.1/doc/getting_started.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/doc/images/logo.png` & `openstack-image-manager-0.3.1/doc/images/logo.png`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/doc/overview.md` & `openstack-image-manager-0.3.1/doc/overview.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/doc/quickstart.md` & `openstack-image-manager-0.3.1/doc/quickstart.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/doc/requirements.md` & `openstack-image-manager-0.3.1/doc/requirements.md`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/images/almalinux.yml` & `openstack-image-manager-0.3.1/etc/images/almalinux.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/images/centos.yml` & `openstack-image-manager-0.3.1/etc/images/centos.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/images/cirros.yml` & `openstack-image-manager-0.3.1/etc/images/cirros.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/images/clearlinux.yml` & `openstack-image-manager-0.3.1/etc/images/clearlinux.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/images/debian.yml` & `openstack-image-manager-0.3.1/etc/images/debian.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/images/fedora.yml` & `openstack-image-manager-0.3.1/etc/images/fedora.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/images/flatcar.yml` & `openstack-image-manager-0.3.1/etc/images/flatcar.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/images/gardenlinux.yml` & `openstack-image-manager-0.3.1/etc/images/gardenlinux.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/images/kubernetes.yml` & `openstack-image-manager-0.3.1/etc/images/kubernetes.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/images/octavia.yml` & `openstack-image-manager-0.3.1/etc/images/octavia.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/images/opensuse.yml` & `openstack-image-manager-0.3.1/etc/images/opensuse.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/images/opnsense.yml` & `openstack-image-manager-0.3.1/etc/images/opnsense.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/images/rockylinux.yml` & `openstack-image-manager-0.3.1/etc/images/rockylinux.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/images/talos.yml` & `openstack-image-manager-0.3.1/etc/images/talos.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/images/ubuntu.yml` & `openstack-image-manager-0.3.1/etc/images/ubuntu.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/etc/schema.yaml` & `openstack-image-manager-0.3.1/etc/schema.yaml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/openstack_image_manager/manage.py` & `openstack-image-manager-0.3.1/openstack_image_manager/manage.py`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/openstack_image_manager/mirror.py` & `openstack-image-manager-0.3.1/openstack_image_manager/mirror.py`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/openstack_image_manager/table.py` & `openstack-image-manager-0.3.1/openstack_image_manager/table.py`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/openstack_image_manager/update.py` & `openstack-image-manager-0.3.1/openstack_image_manager/update.py`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/openstack_image_manager.egg-info/PKG-INFO` & `openstack-image-manager-0.3.1/openstack_image_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstack-image-manager
-Version: 0.3.0
+Version: 0.3.1
 Summary: OpenStack image manager
 Home-page: https://github.com/osism/openstack-image-manager
 Author: OSISM community
 Author-email: info@osism.tech
 License: Apache-2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `openstack-image-manager-0.3.0/openstack_image_manager.egg-info/SOURCES.txt` & `openstack-image-manager-0.3.1/openstack_image_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/playbooks/real-world.yml` & `openstack-image-manager-0.3.1/playbooks/real-world.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/scripts/build.sh` & `openstack-image-manager-0.3.1/scripts/build.sh`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/setup.cfg` & `openstack-image-manager-0.3.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/test/integration/fixtures/test_image.yml` & `openstack-image-manager-0.3.1/test/integration/fixtures/test_image.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/test/integration/test_manage_api.py` & `openstack-image-manager-0.3.1/test/integration/test_manage_api.py`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/test/unit/test_manage.py` & `openstack-image-manager-0.3.1/test/unit/test_manage.py`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.3.0/tox.ini` & `openstack-image-manager-0.3.1/tox.ini`

 * *Files identical despite different names*

