# Comparing `tmp/open-prime-rando-0.6.1.tar.gz` & `tmp/open-prime-rando-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-prime-rando-0.6.1.tar", last modified: Wed Jun 21 09:32:21 2023, max compression
+gzip compressed data, was "open-prime-rando-0.6.2.tar", last modified: Fri Jun 23 10:28:44 2023, max compression
```

## Comparing `open-prime-rando-0.6.1.tar` & `open-prime-rando-0.6.2.tar`

### file list

```diff
@@ -1,88 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.479787 open-prime-rando-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.471787 open-prime-rando-0.6.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.471787 open-prime-rando-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/.github/workflows/python.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 09:32:21.479787 open-prime-rando-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.475787 open-prime-rando-0.6.1/open_prime_rando/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.475787 open-prime-rando-0.6.1/open_prime_rando/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/__pyinstaller/hook-open_prime_rando.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/dynamic_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.475787 open-prime-rando-0.6.1/open_prime_rando/echoes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.479787 open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/agon_wastes.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/great_temple.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/m01_sidehopperstation.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/m02_spires.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/m03_crossfirechaos.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/m04_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/m05_spidercomplex.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/m06_shootinggallery.py
--rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py
--rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/temple_grounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/torvus_bog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/world.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.467787 open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.479787 open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/doors/
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.479787 open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/rubiks/
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
--rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.479787 open-prime-rando-0.6.1/open_prime_rando/echoes/dock_lock_rando/
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/dock_lock_rando/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20936 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/dock_lock_rando/dock_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/dock_lock_rando/map_icons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.479787 open-prime-rando-0.6.1/open_prime_rando/echoes/elevators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/elevators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/elevators/elevator_rando.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.479787 open-prime-rando-0.6.1/open_prime_rando/echoes/inverted/
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/inverted/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/inverted/area_pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.479787 open-prime-rando-0.6.1/open_prime_rando/echoes/small_randomizations/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/small_randomizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/small_randomizations/echo_locks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/small_randomizations/rubiks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/specific_area_patches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes/vulnerabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/echoes_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/p1r_patcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3256 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/patcher_editor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.479787 open-prime-rando-0.6.1/open_prime_rando/prime_remastered/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/prime_remastered/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/unique_area_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/open_prime_rando/validator_with_default.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-21 09:32:21.000000 open-prime-rando-0.6.1/open_prime_rando/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.475787 open-prime-rando-0.6.1/open_prime_rando.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-21 09:32:21.000000 open-prime-rando-0.6.1/open_prime_rando.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-21 09:32:21.000000 open-prime-rando-0.6.1/open_prime_rando.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:32:21.000000 open-prime-rando-0.6.1/open_prime_rando.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-21 09:32:21.000000 open-prime-rando-0.6.1/open_prime_rando.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 09:32:21.000000 open-prime-rando-0.6.1/open_prime_rando.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 09:32:21.000000 open-prime-rando-0.6.1/open_prime_rando.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-21 09:32:21.000000 open-prime-rando-0.6.1/open_prime_rando.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-21 09:32:21.483787 open-prime-rando-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.479787 open-prime-rando-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/tests/test_echoes_custom_Assets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 09:32:21.479787 open-prime-rando-0.6.1/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-06-21 09:32:07.000000 open-prime-rando-0.6.1/tools/asset_id_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.423196 open-prime-rando-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.411196 open-prime-rando-0.6.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.411196 open-prime-rando-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/.github/workflows/python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-23 10:28:44.423196 open-prime-rando-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-23 10:28:44.423196 open-prime-rando-0.6.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.407195 open-prime-rando-0.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.411196 open-prime-rando-0.6.2/src/open_prime_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.415196 open-prime-rando-0.6.2/src/open_prime_rando/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/__pyinstaller/hook-open_prime_rando.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.415196 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/all_prime_dol_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.415196 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/corruption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/corruption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/corruption/dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/corruption/doll_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/dol_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.415196 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/echoes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/echoes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/echoes/beam_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/echoes/dol_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16534 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/echoes/dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/echoes/dol_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/echoes/user_preferences.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.415196 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/prime1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/prime1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/prime1/dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dol_patching/prime1/dol_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/dynamic_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.415196 open-prime-rando-0.6.2/src/open_prime_rando/echoes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.419196 open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/agon_wastes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/great_temple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/m01_sidehopperstation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/m02_spires.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/m03_crossfirechaos.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/m04_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/m05_spidercomplex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/m06_shootinggallery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16279 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14819 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/temple_grounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/torvus_bog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.411196 open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.419196 open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/doors/
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    32780 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    66717 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_template.pdn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.419196 open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/rubiks/
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.419196 open-prime-rando-0.6.2/src/open_prime_rando/echoes/dock_lock_rando/
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/dock_lock_rando/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20626 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/dock_lock_rando/dock_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10917 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/dock_lock_rando/map_icons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.419196 open-prime-rando-0.6.2/src/open_prime_rando/echoes/elevators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/elevators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/elevators/elevator_rando.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.419196 open-prime-rando-0.6.2/src/open_prime_rando/echoes/inverted/
+-rw-r--r--   0 runner    (1001) docker     (123)     7656 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/inverted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/inverted/area_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.419196 open-prime-rando-0.6.2/src/open_prime_rando/echoes/small_randomizations/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/small_randomizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/small_randomizations/echo_locks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/small_randomizations/rubiks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/specific_area_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes/vulnerabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5549 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/echoes_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/p1r_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/patcher_editor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.419196 open-prime-rando-0.6.2/src/open_prime_rando/prime_remastered/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/prime_remastered/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/unique_area_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/src/open_prime_rando/validator_with_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 10:28:44.000000 open-prime-rando-0.6.2/src/open_prime_rando/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.415196 open-prime-rando-0.6.2/src/open_prime_rando.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-23 10:28:44.000000 open-prime-rando-0.6.2/src/open_prime_rando.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4371 2023-06-23 10:28:44.000000 open-prime-rando-0.6.2/src/open_prime_rando.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:28:44.000000 open-prime-rando-0.6.2/src/open_prime_rando.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-23 10:28:44.000000 open-prime-rando-0.6.2/src/open_prime_rando.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-23 10:28:44.000000 open-prime-rando-0.6.2/src/open_prime_rando.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 10:28:44.000000 open-prime-rando-0.6.2/src/open_prime_rando.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.419196 open-prime-rando-0.6.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.423196 open-prime-rando-0.6.2/tests/dol_patching/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/tests/dol_patching/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18392 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/tests/dol_patching/test_all_prime_dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/tests/dol_patching/test_dol_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/tests/dol_patching/test_echoes_dol_patcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17803 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/tests/dol_patching/test_echoes_dol_patches.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/tests/test_echoes_custom_Assets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:28:44.423196 open-prime-rando-0.6.2/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-06-23 10:28:32.000000 open-prime-rando-0.6.2/tools/asset_id_files.py
```

### Comparing `open-prime-rando-0.6.1/.github/dependabot.yml` & `open-prime-rando-0.6.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/.github/workflows/python.yml` & `open-prime-rando-0.6.2/.github/workflows/python.yml`

 * *Files 15% similar despite different names*

```diff
@@ -48,36 +48,92 @@
       matrix:
         python:
           - {version: '3.10', wheel: 'cp310-cp310'}
           - {version: '3.11', wheel: 'cp311-cp311'}
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
+
+      - name: remove code outside of wheel
+        run: rm -rf src
+        shell: bash
 
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python.version }}
 
       - name: Download all the dists
-        uses: actions/download-artifact@v2
+        uses: actions/download-artifact@v3
         with:
           name: python-package-distributions
           path: dist/
 
       - name: Install Python packages
-        run: python -m pip install --upgrade pip pytest
+        run: python -m pip install --upgrade pip
 
       - name: install built wheel
-        run: python -m pip install dist/*.whl
+        run: python -m pip install "$(ls dist/*.whl)[test]"
         shell: bash
 
-      - name: test
-        run: python -m pytest tests
+      - name: run pytest
+        run: python -m pytest
+
+  full_test:
+    runs-on: self-hosted
+    needs:
+      - build
+
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+          submodules: 'recursive'
+
+      - name: Create venv
+        run: python -m venv venv
+
+      - name: Install Python packages
+        run: venv/bin/python -m pip install --upgrade pip
+
+      - name: install built wheel
+        run: venv/bin/python -m pip install -e .[test]
+
+      - name: Run Tests
+        run:
+          venv/bin/python -m pytest --cov --durations=100
+
+      - name: codecov
+        uses: codecov/codecov-action@v3
+        with:
+          fail_ci_if_error: true
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
+
+  ruff:
+    runs-on: 'ubuntu-latest'
+
+    steps:
+      - name: Checkout
+        uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+
+      - name: Set up Python
+        uses: actions/setup-python@v4
+        with:
+          python-version: "3.10"
+
+      - name: Install Python packages
+        run: python -m pip install ruff==0.0.272
+
+      - name: Run ruff
+        run: ruff check --format=github .
 
   pypi:
     runs-on: 'ubuntu-latest'
     needs:
       - test
 
     steps:
```

### Comparing `open-prime-rando-0.6.1/.gitignore` & `open-prime-rando-0.6.2/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -128,8 +128,8 @@
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
 # Project
-open_prime_rando/version.py
+src/open_prime_rando/version.py
```

### Comparing `open-prime-rando-0.6.1/LICENSE` & `open-prime-rando-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/PKG-INFO` & `open-prime-rando-0.6.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: open-prime-rando
-Version: 0.6.1
+Version: 0.6.2
 Summary: An open source randomizer patcher for Metroid Prime 2 and 3.
-Home-page: https://github.com/randovania/open-prime-rando
 Author: Henrique Gemignani
+Project-URL: Homepage, https://github.com/randovania/open-prime-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # Open Prime Rando
 Open Source randomizer patcher for Prime 2 and eventually 3.
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/cli.py` & `open-prime-rando-0.6.2/src/open_prime_rando/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import importlib
 import json
 import logging
 import logging.config
 from pathlib import Path
 
-from retro_data_structures.asset_manager import PathFileProvider, IsoFileProvider
+from retro_data_structures.asset_manager import IsoFileProvider, PathFileProvider
 
 _game_to_patcher = {
     "echoes": "open_prime_rando.echoes_patcher",
     "prime_remastered": "open_prime_rando.p1r_patcher",
 }
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/dynamic_schema.py` & `open-prime-rando-0.6.2/src/open_prime_rando/dynamic_schema.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/agon_wastes.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/agon_wastes.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/great_temple.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/great_temple.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/sanctuary_fortress.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/temple_grounds.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/temple_grounds.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/torvus_bog.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/torvus_bog.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/asset_ids/world.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/asset_ids/world.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_darkburst.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_greyscale_emissive.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sonicboom.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/doors/custom_door_lock_sunburst.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_blue.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_green.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets/rubiks/rubiks_red.TXTR`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/custom_assets.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/custom_assets.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/dock_lock_rando/__init__.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/dock_lock_rando/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from pathlib import Path
 
-from construct import Construct, Container
-from open_prime_rando.echoes.dock_lock_rando.dock_type import *
+from construct import Container
+from open_prime_rando.echoes.dock_lock_rando import dock_type
 from open_prime_rando.echoes.dock_lock_rando.dock_type_database import DOCK_TYPES
 from open_prime_rando.patcher_editor import PatcherEditor
-
-from retro_data_structures.base_resource import RawResource
+from retro_data_structures.base_resource import AssetId, RawResource
 from retro_data_structures.formats.cmdl import Cmdl
 from retro_data_structures.game_check import Game
 
 
 def add_custom_models(editor: PatcherEditor):
     assets = Path(__file__).parent.parent.joinpath("custom_assets", "doors")
     def get_txtr(n: str) -> AssetId:
         res = RawResource(
             type="TXTR",
             data=assets.joinpath(f"{n}.TXTR").read_bytes()
         )
         return editor.add_file(f"{n}.TXTR", res, [])
-    
+
     emissive = get_txtr("custom_door_lock_greyscale_emissive")
     template = editor.get_parsed_asset(0xF115F575, type_hint=Cmdl)
 
     for name in ("darkburst", "sunburst", "sonicboom"):
         txtr = get_txtr(f"custom_door_lock_{name}")
         cmdl = Container(template.raw)
         cmdl.material_sets[0].texture_file_ids[0] = txtr
         cmdl.material_sets[0].texture_file_ids[1] = emissive
         editor.add_file(f"custom_door_lock_{name}.CMDL", Cmdl(cmdl, Game.ECHOES, editor), [])
 
 
-def apply_door_rando(editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, new_door_type: str, old_door_type: str | None, low_memory: bool):
+def apply_door_rando(editor: PatcherEditor, world_name: str, area_name: str, dock_name: str,
+                     new_door_type: str, old_door_type: str | None, low_memory: bool):
     if old_door_type is not None:
         old_door = DOCK_TYPES[old_door_type]
 
-        if isinstance(old_door, VanillaBlastShieldDoorType):
+        if isinstance(old_door, dock_type.VanillaBlastShieldDoorType):
             old_door.remove_blast_shield(editor, world_name, area_name, dock_name)
-    
+
     new_door = DOCK_TYPES[new_door_type]
     new_door.patch_door(editor, world_name, area_name, dock_name, low_memory)
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/dock_lock_rando/dock_type.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/dock_lock_rando/dock_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,103 +1,100 @@
 import dataclasses
-import functools
-import logging
-from typing import NamedTuple, Type
+from typing import NamedTuple
+
+from open_prime_rando.echoes.asset_ids import world
 from open_prime_rando.echoes.dock_lock_rando.map_icons import DoorMapIcon
-from open_prime_rando.patcher_editor import PatcherEditor
-from open_prime_rando.echoes.asset_ids import *
 from open_prime_rando.echoes.vulnerabilities import resist_all_vuln
-
-from retro_data_structures.base_resource import AssetId
+from open_prime_rando.patcher_editor import PatcherEditor
 from retro_data_structures.asset_manager import NameOrAssetId
+from retro_data_structures.base_resource import AssetId
+from retro_data_structures.enums.echoes import Message, State, VisorFlags
+from retro_data_structures.formats.mapa import Mapa
+from retro_data_structures.formats.mrea import Area
+from retro_data_structures.formats.scan import Scan
+from retro_data_structures.formats.script_object import ScriptInstance
+from retro_data_structures.formats.strg import Strg
 from retro_data_structures.properties.base_property import BaseObjectType
+from retro_data_structures.properties.echoes.archetypes.ActorParameters import ActorParameters
 from retro_data_structures.properties.echoes.archetypes.DamageVulnerability import DamageVulnerability
-from retro_data_structures.properties.echoes.archetypes.WeaponVulnerability import WeaponVulnerability
-from retro_data_structures.properties.echoes.core.Color import Color
-from retro_data_structures.properties.echoes.core.Vector import Vector
 from retro_data_structures.properties.echoes.archetypes.EditorProperties import EditorProperties
+from retro_data_structures.properties.echoes.archetypes.HealthInfo import HealthInfo
 from retro_data_structures.properties.echoes.archetypes.ScannableParameters import ScannableParameters
 from retro_data_structures.properties.echoes.archetypes.SurroundPan import SurroundPan
-from retro_data_structures.properties.echoes.archetypes.ActorParameters import ActorParameters
-from retro_data_structures.properties.echoes.archetypes.HealthInfo import HealthInfo
-from retro_data_structures.properties.echoes.archetypes.VisorParameters import VisorParameters
 from retro_data_structures.properties.echoes.archetypes.Transform import Transform
+from retro_data_structures.properties.echoes.archetypes.VisorParameters import VisorParameters
+from retro_data_structures.properties.echoes.archetypes.WeaponVulnerability import WeaponVulnerability
+from retro_data_structures.properties.echoes.core.Color import Color
+from retro_data_structures.properties.echoes.core.Spline import Spline
+from retro_data_structures.properties.echoes.core.Vector import Vector
+from retro_data_structures.properties.echoes.objects.Actor import Actor
+from retro_data_structures.properties.echoes.objects.CameraShaker import CameraShaker
+from retro_data_structures.properties.echoes.objects.Counter import Counter
+from retro_data_structures.properties.echoes.objects.DamageableTrigger import DamageableTrigger
+from retro_data_structures.properties.echoes.objects.DamageableTriggerOrientated import DamageableTriggerOrientated
 from retro_data_structures.properties.echoes.objects.Dock import Dock
 from retro_data_structures.properties.echoes.objects.Door import Door
-from retro_data_structures.properties.echoes.objects.Actor import Actor
+from retro_data_structures.properties.echoes.objects.Effect import Effect
 from retro_data_structures.properties.echoes.objects.MemoryRelay import MemoryRelay
+from retro_data_structures.properties.echoes.objects.Relay import Relay
 from retro_data_structures.properties.echoes.objects.ScannableObjectInfo import ScannableObjectInfo
 from retro_data_structures.properties.echoes.objects.Sound import Sound
 from retro_data_structures.properties.echoes.objects.StreamedAudio import StreamedAudio
-from retro_data_structures.properties.echoes.objects.MemoryRelay import MemoryRelay
-from retro_data_structures.properties.echoes.objects.Effect import Effect
-from retro_data_structures.properties.echoes.objects.DamageableTrigger import DamageableTrigger
-from retro_data_structures.properties.echoes.objects.DamageableTriggerOrientated import DamageableTriggerOrientated
 from retro_data_structures.properties.echoes.objects.Timer import Timer
-from retro_data_structures.properties.echoes.objects.CameraShaker import CameraShaker
-from retro_data_structures.properties.echoes.objects.Counter import Counter
-from retro_data_structures.properties.echoes.objects.Relay import Relay
-from retro_data_structures.properties.echoes.core.Spline import Spline
-from retro_data_structures.formats.mapa import Mapa
-from retro_data_structures.formats.mlvl import AreaWrapper
-from retro_data_structures.formats.scan import Scan
-from retro_data_structures.formats.strg import Strg
-from retro_data_structures.formats.script_object import ScriptInstanceHelper
-from retro_data_structures.enums.echoes import State, Message, VisorFlags
 
 
 @dataclasses.dataclass(kw_only=True)
 class DoorType:
     name: str
 
     vulnerability: DamageVulnerability
 
-    shell_model: NameOrAssetId = 0x6B78FD92 # normal door model
+    shell_model: NameOrAssetId = 0x6B78FD92  # normal door model
     shell_color: Color
 
     scan_text: tuple[str, ...] | None = None
 
     map_icon: DoorMapIcon
 
     patched_scan: AssetId | None = None
 
     def get_paks(self, editor: PatcherEditor, world_name: str, area_name: str):
         world_file = world.load_dedicated_file(world_name)
         return editor.find_paks(world_file.NAME_TO_ID_MREA[area_name])
 
-    def get_files(self, editor: PatcherEditor, world_name: str, area_name: str) -> tuple[AreaWrapper, Mapa]:
+    def get_files(self, editor: PatcherEditor, world_name: str, area_name: str) -> tuple[Area, Mapa]:
         world_file = world.load_dedicated_file(world_name)
-        mrea = editor.get_area_helper(world.NAME_TO_ID_MLVL[world_name], world_file.NAME_TO_ID_MREA[area_name])
+        area = editor.get_area(world.NAME_TO_ID_MLVL[world_name], world_file.NAME_TO_ID_MREA[area_name])
         mapa = editor.get_file(world_file.NAME_TO_ID_MAPA[area_name], type_hint=Mapa)
-        return mrea, mapa
+        return area, mapa
 
     def get_dock_index(self, world_name: str, area_name: str, dock_name: str) -> int:
         world_file = world.load_dedicated_file(world_name)
         return world_file.DOCK_NAMES[area_name][dock_name]
 
-    def get_mrea(self, editor: PatcherEditor, world_name: str, area_name: str) -> AreaWrapper:
+    def get_area(self, editor: PatcherEditor, world_name: str, area_name: str) -> Area:
         return self.get_files(editor, world_name, area_name)[0]
 
-    def get_door_from_dock_index(self, mrea: AreaWrapper, dock_index: int) -> ScriptInstanceHelper:
+    def get_door_from_dock_index(self, area: Area, dock_index: int) -> ScriptInstance:
         dock = next(
-            inst for inst in mrea.mrea.all_instances
+            inst for inst in area.all_instances
             if (
-                inst.type == Dock and
-                inst.get_properties_as(Dock).dock_number == dock_index
+                    inst.type == Dock and
+                    inst.get_properties_as(Dock).dock_number == dock_index
             )
         )
-        for instance in mrea.mrea.all_instances:
+        for instance in area.all_instances:
             if instance.type != Door:
                 continue
             for connection in instance.connections:
                 if dock.id_matches(connection.target):
                     return instance
-        raise KeyError(f"no door found with a connection to {dock} in {mrea.name}")
+        raise KeyError(f"no door found with a connection to {dock} in {area.name}")
 
-    def patch_map_icon(self, mapa: Mapa, door: ScriptInstanceHelper):
+    def patch_map_icon(self, mapa: Mapa, door: ScriptInstance):
         for obj in mapa.raw.mappable_objects:
             if door.id_matches(obj.editor_id):
                 obj.type = self.map_icon.value
                 return
 
     @staticmethod
     def get_scan_templates(editor: PatcherEditor) -> tuple[Scan, Strg]:
@@ -123,67 +120,75 @@
             self.patched_scan = scan_id
 
         for pak in paks:
             editor.ensure_present(pak, self.patched_scan)
         return self.patched_scan
 
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
-        mrea, mapa = self.get_files(editor, world_name, area_name)
-        door = self.get_door_from_dock_index(mrea, self.get_dock_index(world_name, area_name, dock_name))
+        area, mapa = self.get_files(editor, world_name, area_name)
+        door = self.get_door_from_dock_index(area, self.get_dock_index(world_name, area_name, dock_name))
         self.patch_map_icon(mapa, door)
 
         shell_model = editor._resolve_asset_id(self.shell_model)
 
         with door.edit_properties(Door) as door_props:
             door_props.shell_model = shell_model
             door_props.shell_color = self.shell_color
+            if self.scan_text is not None:
+                door_props.alt_scannable.scannable_info0 = self.get_patched_scan(editor, world_name, area_name)
+            else:
+                door_props.alt_scannable.scannable_info0 = 0xFFFFFFFF
 
         for pak in self.get_paks(editor, world_name, area_name):
             editor.ensure_present(pak, shell_model)
 
 
 @dataclasses.dataclass(kw_only=True)
 class NormalDoorType(DoorType):
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
         super().patch_door(editor, world_name, area_name, dock_name, low_memory)
-        mrea = self.get_mrea(editor, world_name, area_name)
-        door = self.get_door_from_dock_index(mrea, self.get_dock_index(world_name, area_name, dock_name))
+        area = self.get_area(editor, world_name, area_name)
+        door = self.get_door_from_dock_index(area, self.get_dock_index(world_name, area_name, dock_name))
 
         with door.edit_properties(Door) as door_props:
             door_props.vulnerability = self.vulnerability
-            if self.scan_text is not None:
-                door_props.alt_scannable.scannable_info0 = self.get_patched_scan(editor, world_name, area_name)
 
 
 class BlastShieldActors(NamedTuple):
-    door: ScriptInstanceHelper
-    sound: ScriptInstanceHelper
-    streamed: ScriptInstanceHelper
-    lock: ScriptInstanceHelper
-    relay: ScriptInstanceHelper
-    gibs: ScriptInstanceHelper | None
+    door: ScriptInstance
+    sound: ScriptInstance
+    streamed: ScriptInstance
+    lock: ScriptInstance
+    relay: ScriptInstance
+    gibs: ScriptInstance | None
 
 
 @dataclasses.dataclass(kw_only=True)
 class BlastShieldDoorType(DoorType):
     shield_model: NameOrAssetId
     shield_collision_box: Vector = dataclasses.field(default_factory=lambda: Vector(0.35, 5.0, 4.0))
-    shield_collision_offset: Vector = dataclasses.field(default_factory=lambda: Vector(-2/3, 0, 2.0))
+    shield_collision_offset: Vector = dataclasses.field(default_factory=lambda: Vector(-2 / 3, 0, 2.0))
 
-    def find_attached_instance(self, area: AreaWrapper, source: ScriptInstanceHelper, state: State, message: Message, target_type: Type[BaseObjectType], target_name: str | None = None) -> ScriptInstanceHelper:
+    def find_attached_instance(
+            self, area: Area, source: ScriptInstance, state: State, message: Message,
+            target_type: type[BaseObjectType], target_name: str | None = None
+    ) -> ScriptInstance:
         for connection in source.connections:
             if connection.state == state and connection.message == message:
                 target = area.get_instance(connection.target)
                 if target.type == target_type and (target_name is None or target.name == target_name):
                     return target
         name = f"{target_type} named {target_name}" if target_name is not None else str(target_type)
         raise TypeError(f"No {name} connected to {source}")
 
     def get_spline(self) -> Spline:
-        return Spline(data=b'\x00\x00\x00\x00\x00\x02\x00\x00\x00\x00\x00\x00\x00\x00\x02\x02A \x00\x00?\x80\x00\x00\x02\x02\x01\x00\x00\x00\x00?\x80\x00\x00')
+        return Spline(
+            data=b'\x00\x00\x00\x00\x00\x02\x00\x00\x00\x00\x00\x00\x00\x00\x02'
+                 b'\x02A \x00\x00?\x80\x00\x00\x02\x02\x01\x00\x00\x00\x00?\x80\x00\x00'
+        )
 
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
         """
         blast shield connections:
             DEAD -> lock cleared MemoryRelay, ACTV
             DEAD -> lock breaking SoundEffect, PLAY
             DEAD -> lock explosion gibs, ACTV
@@ -193,19 +198,19 @@
             OPEN -> lock cleared MemoryRelay, ACTV
 
         memory relay connections:
             ACTV -> door, RSET
             ACTV -> blast shield, DCTV
         """
         super().patch_door(editor, world_name, area_name, dock_name, low_memory)
-        mrea = self.get_mrea(editor, world_name, area_name)
-        door = self.get_door_from_dock_index(mrea, self.get_dock_index(world_name, area_name, dock_name))
+        area = self.get_area(editor, world_name, area_name)
+        door = self.get_door_from_dock_index(area, self.get_dock_index(world_name, area_name, dock_name))
         door_transform = door.get_properties_as(Door).editor_properties.transform
 
-        default = mrea.get_layer("Default")
+        default = area.get_layer("Default")
 
         sound = default.add_instance_with(Sound(
             editor_properties=EditorProperties(
                 name="Metal Door Lock Breaking",
                 transform=door_transform
             ),
             sound=948,
@@ -254,15 +259,15 @@
         relay.add_connection(State.Active, Message.Deactivate, lock)
         relay.add_connection(State.Active, Message.Reset, door)
 
         door.add_connection(State.Open, Message.Activate, relay)
 
         dependencies = [
             model,
-            0x8B4CD966, # MetalDoorLockBreak AGSC
+            0x8B4CD966,  # MetalDoorLockBreak AGSC
         ]
 
         gibs = None
         if not low_memory:
             particle = 0xCDCBDF04
 
             gibs = default.add_instance_with(Effect(
@@ -284,42 +289,42 @@
 
         return BlastShieldActors(door, sound, streamed, lock, relay, gibs)
 
 
 @dataclasses.dataclass(kw_only=True)
 class VanillaBlastShieldDoorType(BlastShieldDoorType):
     def remove_blast_shield(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str):
-        mrea = self.get_mrea(editor, world_name, area_name)
-        door = self.get_door_from_dock_index(mrea, self.get_dock_index(world_name, area_name, dock_name))
+        area = self.get_area(editor, world_name, area_name)
+        door = self.get_door_from_dock_index(area, self.get_dock_index(world_name, area_name, dock_name))
 
-        relay = self.find_attached_instance(mrea, door, State.Open, Message.Activate, MemoryRelay)
-        lock = self.find_attached_instance(mrea, relay, State.Active, Message.Deactivate, Actor)
+        relay = self.find_attached_instance(area, door, State.Open, Message.Activate, MemoryRelay)
+        lock = self.find_attached_instance(area, relay, State.Active, Message.Deactivate, Actor)
 
         for connection in lock.connections:
-            mrea.mrea.remove_instance(connection.target)
-        mrea.mrea.remove_instance(lock)
+            area.remove_instance(connection.target)
+        area.remove_instance(lock)
 
 
 @dataclasses.dataclass(kw_only=True)
 class SeekerBlastShieldDoorType(VanillaBlastShieldDoorType):
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
         actors = super().patch_door(editor, world_name, area_name, dock_name, low_memory)
-        mrea = self.get_mrea(editor, world_name, area_name)
-        default = mrea.get_layer("Default")
+        area = self.get_area(editor, world_name, area_name)
+        default = area.get_layer("Default")
 
         # immune instead of reflect so that it explodes on the lock
         missile_immune = dataclasses.replace(resist_all_vuln, missile=WeaponVulnerability(damage_multiplier=0.0))
         with actors.lock.edit_properties(Actor) as lock:
             lock.vulnerability = missile_immune
         with actors.door.edit_properties(Door) as door:
             door.vulnerability = missile_immune
 
         door_transform = actors.door.get_properties_as(Door).editor_properties.transform
 
-        def create_trigger(name: str, health: float, lock_on: bool = True) -> ScriptInstanceHelper:
+        def create_trigger(name: str, health: float, lock_on: bool = True) -> ScriptInstance:
             pos = Vector(
                 door_transform.position.x,
                 door_transform.position.y,
                 door_transform.position.z + 1.8
             )
 
             return default.add_instance_with(DamageableTriggerOrientated(
@@ -385,36 +390,29 @@
 
         for trigger in triggers:
             actors.relay.add_connection(State.Active, Message.Deactivate, trigger)
         actors.relay.add_connection(State.Active, Message.Deactivate, mini_trigger)
         actors.relay.add_connection(State.Active, Message.Deactivate, timer)
         actors.relay.add_connection(State.Active, Message.Deactivate, timer_reset)
 
-
     def remove_blast_shield(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str):
-        mrea = self.get_mrea(editor, world_name, area_name)
-        door = self.get_door_from_dock_index(mrea, self.get_dock_index(world_name, area_name, dock_name))
-
-        default = mrea.get_layer("Default")
+        area = self.get_area(editor, world_name, area_name)
+        door = self.get_door_from_dock_index(area, self.get_dock_index(world_name, area_name, dock_name))
 
-        memory_relay = self.find_attached_instance(mrea, door, State.Open, Message.Activate, MemoryRelay)
-        trigger = self.find_attached_instance(mrea, memory_relay, State.Active, Message.Deactivate, DamageableTrigger)
-        shaker = self.find_attached_instance(mrea, trigger, State.Dead, Message.Action, CameraShaker)
-        counter = self.find_attached_instance(mrea, trigger, State.Dead, Message.Increment, Counter)
-        complete_relay = self.find_attached_instance(mrea, counter, State.MaxReached, Message.SetToZero, Relay)
+        memory_relay = self.find_attached_instance(area, door, State.Open, Message.Activate, MemoryRelay)
+        trigger = self.find_attached_instance(area, memory_relay, State.Active, Message.Deactivate, DamageableTrigger)
+        shaker = self.find_attached_instance(area, trigger, State.Dead, Message.Action, CameraShaker)
+        counter = self.find_attached_instance(area, trigger, State.Dead, Message.Increment, Counter)
+        complete_relay = self.find_attached_instance(area, counter, State.MaxReached, Message.SetToZero, Relay)
 
-        default.remove_instance(shaker)
+        area.remove_instance(shaker)
         for connection in complete_relay.connections:
-            try:
-                default.remove_instance(connection.target)
-            except KeyError:
-                # I guess claris already removed it probably?
-                complete_relay.remove_connection(connection)
-        default.remove_instance(complete_relay)
-        default.remove_instance(counter)
+            area.remove_instance(connection.target)
+        area.remove_instance(complete_relay)
+        area.remove_instance(counter)
 
 
 @dataclasses.dataclass(kw_only=True)
 class PlanetaryEnergyDoorType(DoorType):
     planetary_energy_item_id: int
 
     def patch_door(self, editor: PatcherEditor, world_name: str, area_name: str, dock_name: str, low_memory: bool):
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/dock_lock_rando/dock_type_database.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,237 +1,247 @@
 import dataclasses
 
+from open_prime_rando.echoes.dock_lock_rando import dock_type
+from open_prime_rando.echoes.dock_lock_rando.map_icons import DoorMapIcon
+from open_prime_rando.echoes.vulnerabilities import resist_all_vuln, vulnerable
 from retro_data_structures.properties.echoes.core.Color import Color
 from retro_data_structures.properties.echoes.core.Vector import Vector
 
-from open_prime_rando.echoes.dock_lock_rando.dock_type import *
-from open_prime_rando.echoes.dock_lock_rando.map_icons import DoorMapIcon
-from open_prime_rando.echoes.vulnerabilities import vulnerable, resist_all_vuln
-
-
 normal_door_model = 0x6B78FD92
 dark_door_model = 0xbbcf134d
 annihilator_door_model = 0xa50c7238
 
 blast_collision_box = Vector(0.35, 5.0, 4.0)
-blast_collision_offset = Vector(-2/3, 0, 2.0)
-
+blast_collision_offset = Vector(-2 / 3, 0, 2.0)
 
-DOCK_TYPES: dict[str, DoorType] = {
-    "Normal": NormalDoorType(
+DOCK_TYPES: dict[str, dock_type.DoorType] = {
+    "Normal": dock_type.NormalDoorType(
         name="Normal",
         vulnerability=dataclasses.replace(
             resist_all_vuln,
             power=vulnerable, dark=vulnerable, light=vulnerable, annihilator=vulnerable,
             power_charge=vulnerable, entangler=vulnerable, light_blast=vulnerable, sonic_boom=vulnerable,
             super_missle=vulnerable, black_hole=vulnerable, sunburst=vulnerable, imploder=vulnerable,
 
             missile=vulnerable, bomb=vulnerable, power_bomb=vulnerable,
 
         ),
         shell_color=Color(r=0, g=1, b=1, a=1),
         map_icon=DoorMapIcon.Normal,
     ),
-    "Dark": NormalDoorType(
+    "Dark": dock_type.NormalDoorType(
         name="Dark",
-        vulnerability=dataclasses.replace(resist_all_vuln, dark=vulnerable, entangler=vulnerable, black_hole=vulnerable),
+        vulnerability=dataclasses.replace(resist_all_vuln, dark=vulnerable, entangler=vulnerable,
+                                          black_hole=vulnerable),
         shell_model=dark_door_model,
         shell_color=Color(r=1, g=1, b=1, a=1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. Dark energy may damage it."
         ),
         map_icon=DoorMapIcon.Dark
     ),
-    "Light": NormalDoorType(
+    "Light": dock_type.NormalDoorType(
         name="Light",
-        vulnerability=dataclasses.replace(resist_all_vuln, light=vulnerable, light_blast=vulnerable, sunburst=vulnerable),
+        vulnerability=dataclasses.replace(resist_all_vuln, light=vulnerable, light_blast=vulnerable,
+                                          sunburst=vulnerable),
         shell_color=Color(r=1, g=1, b=1, a=1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. Light energy may damage it."
         ),
         map_icon=DoorMapIcon.Light
     ),
-    "Annihilator": NormalDoorType(
+    "Annihilator": dock_type.NormalDoorType(
         name="Annihilator",
-        vulnerability=dataclasses.replace(resist_all_vuln, annihilator=vulnerable, sonic_boom=vulnerable, imploder=vulnerable),
+        vulnerability=dataclasses.replace(resist_all_vuln, annihilator=vulnerable, sonic_boom=vulnerable,
+                                          imploder=vulnerable),
         shell_model=annihilator_door_model,
         shell_color=Color(r=1, g=1, b=1, a=1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
-            "Analysis indicates that the Blast Shield is invulnerable to most weapons. A mix of light and dark energy may damage it."
+            "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
+            "A mix of light and dark energy may damage it."
         ),
         map_icon=DoorMapIcon.Annihilator
     ),
-    "Disabled": NormalDoorType(
+    "Disabled": dock_type.NormalDoorType(
         name="Disabled",
         vulnerability=resist_all_vuln,
         shell_color=Color(r=0, g=0, b=0, a=0),
         scan_text=(
             "Door system access denied.",
             "Unable to bypass security codes. Seek an alternate exit."
         ),
         map_icon=DoorMapIcon.Disabled
     ),
-    "Missile": VanillaBlastShieldDoorType(
+    "Missile": dock_type.VanillaBlastShieldDoorType(
         name="Missile",
         vulnerability=dataclasses.replace(resist_all_vuln, missile=vulnerable),
         shell_color=Color(r=1, g=0, b=0, a=1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. A Missile blast may damage it."
         ),
         map_icon=DoorMapIcon.Missile,
         shield_model=0xBFB4A8EE,
     ),
-    "SuperMissile": VanillaBlastShieldDoorType(
+    "SuperMissile": dock_type.VanillaBlastShieldDoorType(
         name="SuperMissile",
         vulnerability=dataclasses.replace(resist_all_vuln, super_missle=vulnerable),
         shell_color=Color(r=0, g=1, b=0, a=1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
-            "Analysis indicates that the Blast Shield is invulnerable to most weapons. A Super Missile blast may damage it."
+            "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
+            "A Super Missile blast may damage it."
         ),
         map_icon=DoorMapIcon.SuperMissile,
         shield_model=0xF115F575,
     ),
-    "PowerBomb": VanillaBlastShieldDoorType(
+    "PowerBomb": dock_type.VanillaBlastShieldDoorType(
         name="PowerBomb",
         vulnerability=dataclasses.replace(resist_all_vuln, power_bomb=vulnerable),
         shell_color=Color(r=1, g=0.94, b=0, a=1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. A Power Bomb may damage it."
         ),
         map_icon=DoorMapIcon.PowerBomb,
         shield_model=0xC2E4F075,
     ),
-    "SeekerMissile": SeekerBlastShieldDoorType(
+    "SeekerMissile": dock_type.SeekerBlastShieldDoorType(
         name="SeekerMissile",
         vulnerability=dataclasses.replace(resist_all_vuln, missile=vulnerable),
         shell_color=Color(r=0.5, g=0, b=0.64, a=1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
-            "Analysis indicates that the Blast Shield is invulnerable to most weapons. Five simultaneous Missile blasts may damage it."
+            "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
+            "Five simultaneous Missile blasts may damage it."
         ),
         map_icon=DoorMapIcon.SeekerMissile,
         shield_model=0x56F4208B,
     ),
-    "ScrewAttack": BlastShieldDoorType(
+    "ScrewAttack": dock_type.BlastShieldDoorType(
         name="ScrewAttack",
         vulnerability=dataclasses.replace(resist_all_vuln, screw_attack=vulnerable),
         shell_model=annihilator_door_model,
         shell_color=Color(r=0, g=0, b=1, a=1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. The Screw Attack may damage it."
         ),
         map_icon=DoorMapIcon.ScrewAttack,
         shield_model=0x56F4208B,
     ),
-    "Bomb": BlastShieldDoorType(
+    "Bomb": dock_type.BlastShieldDoorType(
         name="Bomb",
         vulnerability=dataclasses.replace(resist_all_vuln, bomb=vulnerable),
         shell_model=annihilator_door_model,
         shell_color=Color(r=0, g=1, b=1, a=1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
-            "Analysis indicates that the Blast Shield is invulnerable to most weapons. A Morph Ball Bomb blast may damage it."
+            "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
+            "A Morph Ball Bomb blast may damage it."
         ),
         map_icon=DoorMapIcon.Bomb,
         shield_model=0x56F4208B,
     ),
-    "Boost": BlastShieldDoorType(
+    "Boost": dock_type.BlastShieldDoorType(
         name="Boost",
         vulnerability=dataclasses.replace(resist_all_vuln, boost_ball=vulnerable, cannon_ball=vulnerable),
         shell_model=annihilator_door_model,
         shell_color=Color(r=1, g=1, b=0, a=1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
             "Analysis indicates that the Blast Shield is invulnerable to most weapons. The Boost Ball may damage it."
         ),
         map_icon=DoorMapIcon.Boost,
         shield_model=0x56F4208B,
     ),
-    "Grapple": GrappleDoorType(
+    "Grapple": dock_type.GrappleDoorType(
         name="Grapple",
         vulnerability=resist_all_vuln,
         shell_model=annihilator_door_model,
         shell_color=Color(r=1, g=0, b=0, a=1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
-            "Analysis indicates that the Blast Shield is invulnerable to weapon fire, but is weakly secured. The Grapple Beam may be able to remove it."
+            "Analysis indicates that the Blast Shield is invulnerable to weapon fire, but is weakly secured. "
+            "The Grapple Beam may be able to remove it."
         ),
         map_icon=DoorMapIcon.Grapple,
         shield_model=0x56F4208B,
     ),
-    "Darkburst": BlastShieldDoorType(
+    "Darkburst": dock_type.BlastShieldDoorType(
         name="Darkburst",
         vulnerability=dataclasses.replace(resist_all_vuln, black_hole=vulnerable),
         shell_model=dark_door_model,
         shell_color=Color(r=1, g=1, b=1, a=1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
-            "Analysis indicates that the Blast Shield is invulnerable to most weapons. A massive burst of dark energy may damage it."
+            "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
+            "A massive burst of dark energy may damage it."
         ),
         map_icon=DoorMapIcon.Dark,
         shield_model="custom_door_lock_darkburst.CMDL",
     ),
-    "Sunburst": BlastShieldDoorType(
+    "Sunburst": dock_type.BlastShieldDoorType(
         name="Sunburst",
         vulnerability=dataclasses.replace(resist_all_vuln, sunburst=vulnerable),
         shell_model=normal_door_model,
         shell_color=Color(r=1, g=1, b=1, a=1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
-            "Analysis indicates that the Blast Shield is invulnerable to most weapons. A massive burst of light energy may damage it."
+            "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
+            "A massive burst of light energy may damage it."
         ),
         map_icon=DoorMapIcon.Light,
         shield_model="custom_door_lock_sunburst.CMDL",
     ),
-    "SonicBoom": BlastShieldDoorType(
+    "SonicBoom": dock_type.BlastShieldDoorType(
         name="SonicBoom",
         vulnerability=dataclasses.replace(resist_all_vuln, imploder=vulnerable),
         shell_model=annihilator_door_model,
         shell_color=Color(r=1, g=1, b=1, a=1),
         scan_text=(
             "There is a Blast Shield on the door blocking access. ",
-            "Analysis indicates that the Blast Shield is invulnerable to most weapons. A massive burst of light and dark energy may damage it."
+            "Analysis indicates that the Blast Shield is invulnerable to most weapons. "
+            "A massive burst of light and dark energy may damage it."
         ),
         map_icon=DoorMapIcon.Annihilator,
         shield_model="custom_door_lock_sonicboom.CMDL",
     ),
-    "AgonEnergy": PlanetaryEnergyDoorType(
+    "AgonEnergy": dock_type.PlanetaryEnergyDoorType(
         name="AgonEnergy",
         vulnerability=resist_all_vuln,
         shell_color=Color(r=0.64, g=0.34, b=0, a=1),
         scan_text=(
             "There is a Luminoth barrier on the door blocking access. ",
             "Analysis indicates that the barrier is linked to the energy of Agon. Return the energy to the Agon Temple."
         ),
         map_icon=DoorMapIcon.AgonEnergy,
-        planetary_energy_item_id=-1 # TODO
+        planetary_energy_item_id=-1  # TODO
     ),
-    "TorvusEnergy": PlanetaryEnergyDoorType(
+    "TorvusEnergy": dock_type.PlanetaryEnergyDoorType(
         name="TorvusEnergy",
         vulnerability=resist_all_vuln,
         shell_color=Color(r=0.31, g=0.59, b=38, a=1),
         scan_text=(
             "There is a Luminoth barrier on the door blocking access. ",
-            "Analysis indicates that the barrier is linked to the energy of Torvus. Return the energy to the Torvus Temple."
+            "Analysis indicates that the barrier is linked to the energy of Torvus. "
+            "Return the energy to the Torvus Temple."
         ),
         map_icon=DoorMapIcon.TorvusEnergy,
-        planetary_energy_item_id=-1 # TODO
+        planetary_energy_item_id=-1  # TODO
     ),
-    "SanctuaryEnergy": PlanetaryEnergyDoorType(
+    "SanctuaryEnergy": dock_type.PlanetaryEnergyDoorType(
         name="SanctuaryEnergy",
         vulnerability=resist_all_vuln,
         shell_color=Color(r=0.64, g=0.34, b=0, a=1),
         scan_text=(
             "There is a Luminoth barrier on the door blocking access. ",
-            "Analysis indicates that the barrier is linked to the energy of Sanctuary. Return the energy to the Sanctuary Temple."
+            "Analysis indicates that the barrier is linked to the energy of Sanctuary. "
+            "Return the energy to the Sanctuary Temple."
         ),
         map_icon=DoorMapIcon.AgonEnergy,
-        planetary_energy_item_id=-1 # TODO
+        planetary_energy_item_id=-1  # TODO
     ),
 }
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/elevators/auto_enabled_elevator_patches.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import open_prime_rando.echoes.asset_ids.agon_wastes as agon_wastes
 import open_prime_rando.echoes.asset_ids.great_temple as great_temple
 import open_prime_rando.echoes.asset_ids.sanctuary_fortress as sanctuary_fortress
 import open_prime_rando.echoes.asset_ids.temple_grounds as temple_grounds
 import open_prime_rando.echoes.asset_ids.torvus_bog as torvus_bog
 import open_prime_rando.echoes.asset_ids.world as world
 from open_prime_rando.patcher_editor import PatcherEditor
-
-from retro_data_structures.formats.script_object import ScriptInstanceHelper
-from retro_data_structures.game_check import Game
-from retro_data_structures.properties.echoes.objects.Timer import Timer
+from retro_data_structures.enums.echoes import Message, State
 from retro_data_structures.properties.echoes.archetypes.EditorProperties import EditorProperties
-from retro_data_structures.enums.echoes import State, Message
-
+from retro_data_structures.properties.echoes.objects.Timer import Timer
 
 ELEVATOR_MEMORY_RELAY_PER_MREA = {
     world.GREAT_TEMPLE_MLVL: {
         great_temple.TEMPLE_TRANSPORT_A_MREA: 0x00000107,
         great_temple.TEMPLE_TRANSPORT_B_MREA: 0x0008002f,
         great_temple.TEMPLE_TRANSPORT_C_MREA: 0x00060046,
     },
@@ -48,15 +44,15 @@
 
 def apply_auto_enabled_elevators_patch(editor: PatcherEditor):
     """
     Patches that activates every elevator on room load
     """
     for mlvl_id, areas in ELEVATOR_MEMORY_RELAY_PER_MREA.items():
         for mrea_id, memory_relay_id in areas.items():
-            area = editor.get_area_helper(mlvl_id, mrea_id)
+            area = editor.get_area(mlvl_id, mrea_id)
             timer = area.get_layer("Default").add_instance_with(Timer(
                 editor_properties=EditorProperties(
                     name="Timer - Auto enable elevator",
                     active=False
                 ),
                 time=0.001,
                 auto_start=True
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/elevators/elevator_rando.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/elevators/elevator_rando.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from open_prime_rando.patcher_editor import PatcherEditor
-from retro_data_structures.formats.mlvl import AreaWrapper
-from retro_data_structures.properties.echoes.objects.WorldTeleporter import WorldTeleporter
+from retro_data_structures.formats.mrea import Area
 from retro_data_structures.formats.strg import Strg
+from retro_data_structures.properties.echoes.objects.WorldTeleporter import WorldTeleporter
+
 
+def patch_elevator(editor: PatcherEditor, area: Area, elevator_id: int,
+                   target_mlvl: int, target_mrea: int, target_strg: int, target_name: str):
 
-def patch_elevator(editor: PatcherEditor, area: AreaWrapper, elevator_id: int, target_mlvl: int, target_mrea: int, target_strg: int, target_name: str):
     elevator = area.get_instance(elevator_id)
     with elevator.edit_properties(WorldTeleporter) as props:
         props.world = target_mlvl
         props.area = target_mrea
 
     if target_strg is not None:
         strg = editor.get_file(target_strg, Strg)
-        strg.set_string(1, f"Access to &push;&main-color=#FF3333;{target_name} &pop;granted. Step into the hologram to activate elevator.")
+        strg.set_string(1, f"Access to &push;&main-color=#FF3333;{target_name} &pop;granted. "
+                           f"Step into the hologram to activate elevator.")
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/inverted/__init__.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/inverted/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import dataclasses
 
 import construct
+from open_prime_rando.echoes.asset_ids import world as world_ids
+from open_prime_rando.echoes.inverted import area_pairs
+from open_prime_rando.patcher_editor import PatcherEditor
 from retro_data_structures.base_resource import Dependency, RawResource
 from retro_data_structures.dependencies import recursive_dependencies_for_editor
 from retro_data_structures.formats import Mlvl
+from retro_data_structures.formats.mrea import Area
+from retro_data_structures.formats.script_layer import ScriptLayer
+from retro_data_structures.formats.script_object import InstanceId, ScriptInstance
 from retro_data_structures.properties.echoes.objects.AreaAttributes import AreaAttributes
 from retro_data_structures.properties.echoes.objects.SafeZone import SafeZone
 from retro_data_structures.properties.echoes.objects.SafeZoneCrystal import SafeZoneCrystal
 
-from open_prime_rando.echoes.asset_ids import world as world_ids
-from open_prime_rando.echoes.inverted.area_pairs import TG_PAIRS, AGON_PAIRS
-from open_prime_rando.patcher_editor import PatcherEditor
-
 _WORLDS = [
     world_ids.TEMPLE_GROUNDS_MLVL, world_ids.AGON_WASTES_MLVL, world_ids.TORVUS_BOG_MLVL,
     world_ids.SANCTUARY_FORTRESS_MLVL, world_ids.GREAT_TEMPLE_MLVL,
 ]
 _AREAS_TO_SKIP = {
     0x775664a5,  # 00_scandummy
     0x752b2850,  # game_end_part1
@@ -61,98 +63,120 @@
             mapa[8:12] = construct.Int32ub.build(not is_dark_world)
             editor.replace_asset(
                 mapa_id,
                 RawResource("MAPA", bytes(mapa))
             )
 
 
+def _copy_safe_zones(dark: Area, dark_layer: ScriptLayer, light_layer: ScriptLayer,
+                     new_dependencies: set[int], special_ids: set):
+    copied_safe_zones = {}
+
+    for instance in list(dark_layer.instances):
+        if instance.type == SafeZone:
+            copied_safe_zones[instance.id] = light_layer.add_instance_with(props := instance.get_properties())
+            assert isinstance(props, SafeZone)
+            new_dependencies.add(props.impact_effect)
+
+            ids = {conn.target for conn in instance.connections}
+            for target in ids:
+                target_name = dark.get_instance(target).name
+                if "ENTERED Safezone" not in target_name and "EXITED Safezone" not in target_name:
+                    special_ids.add(instance.id)
+
+            if instance.id not in special_ids:
+                dark_layer.remove_instance(instance)
+
+    return copied_safe_zones
+
+
+def _copy_safe_zone_crystal(copied_crystal: ScriptInstance,
+                            instance: ScriptInstance,
+                            copied_safe_zones: dict[InstanceId, ScriptInstance],
+                            dark: Area, special_ids: set[int],
+                            ):
+    targets_special = False
+
+    for conn in instance.connections:
+        if conn.target == instance.id:
+            target = copied_crystal
+        elif conn.target in copied_safe_zones:
+            targets_special = targets_special or conn.target in special_ids
+            target = copied_safe_zones[conn.target]
+        else:
+            targets_special = True
+            weird_target = dark.get_instance(conn.target)
+            print(
+                f"Crystal {instance.name} at {dark.name} has unexpected connections "
+                f"to {weird_target} ({weird_target.name})")
+            continue
+        copied_crystal.add_connection(conn.state, conn.message, target)
+
+    return targets_special
+
+
+def _update_dependencies(world: Mlvl, light: Area, new_dependencies: set[int]):
+    # Add assets used by safe zones
+    new_dependencies = frozenset(new_dependencies)
+    if new_dependencies not in _all_deps_cache:
+        _all_deps_cache[new_dependencies] = recursive_dependencies_for_editor(
+            world.asset_manager, list(new_dependencies)
+        )
+
+    dependencies = light._raw.dependencies
+    assert isinstance(dependencies.dependencies_b, list)
+    for dep in _all_deps_cache[new_dependencies]:
+        dependencies.dependencies_b.append(construct.Container(
+            asset_id=dep.id,
+            asset_type=dep.type,
+        ))
+
+    for i in range(1, len(dependencies.dependencies_offset)):
+        dependencies.dependencies_offset[i] += len(new_dependencies)
+
+    # Add Safe Zone's module dep
+    module_dependencies = light._raw.module_dependencies
+    for module_dep in set(SafeZone.modules() + SafeZoneCrystal.modules()):
+        if module_dep not in module_dependencies.rel_module:
+            module_dependencies.rel_module.insert(0, module_dep)
+            for i in range(1, len(module_dependencies.rel_offset)):
+                module_dependencies.rel_offset[i] += 1
+
+
 def _move_safe_zones(world: Mlvl, pairs: list[tuple[int, int]]):
     for pair in pairs:
         light = world.get_area(pair[0])
         dark = world.get_area(pair[1])
 
         light_layer = light.get_layer("Default")
         dark_layer = dark.get_layer("Default")
 
         assert light_layer.index == 0
 
-        new_dependencies = set()  # asset ids that must be added to the mlvl dependency list
+        new_dependencies: set[int] = set()  # asset ids that must be added to the mlvl dependency list
         special_ids = set()  # ids for objects that have extra functionality and we want to keep
-        copied_safe_zones = {}
 
         # Copy the safe zones
-        for instance in list(dark_layer.instances):
-            if instance.type == SafeZone:
-                copied_safe_zones[instance.id] = light_layer.add_instance_with(props := instance.get_properties())
-                assert isinstance(props, SafeZone)
-                new_dependencies.add(props.impact_effect)
-
-                ids = {conn.target for conn in instance.connections}
-                for target in ids:
-                    target_name = dark.get_instance(target).name
-                    if "ENTERED Safezone" not in target_name and "EXITED Safezone" not in target_name:
-                        special_ids.add(instance.id)
-
-                if instance.id not in special_ids:
-                    dark_layer.remove_instance(instance)
+        copied_safe_zones = _copy_safe_zones(dark, dark_layer, light_layer, new_dependencies, special_ids)
 
         # Copy the safe zone crystals
         for instance in list(dark_layer.instances):
             if instance.type == SafeZoneCrystal:
                 copied_crystal = light_layer.add_instance_with(props := instance.get_properties())
                 new_dependencies.update(collect_dependencies(props))
 
-                targets_special = False
-
-                for conn in instance.connections:
-                    if conn.target == instance.id:
-                        target = copied_crystal
-                    elif conn.target in copied_safe_zones:
-                        targets_special = targets_special or conn.target in special_ids
-                        target = copied_safe_zones[conn.target]
-                    else:
-                        targets_special = True
-                        weird_target = dark.get_instance(conn.target)
-                        print(
-                            f"Crystal {instance.name} at {dark.name} has unexpected connections to {weird_target} ({weird_target.name})")
-                        continue
-                    copied_crystal.add_connection(conn.state, conn.message, target)
-
+                targets_special = _copy_safe_zone_crystal(
+                    copied_crystal, instance, copied_safe_zones, dark, special_ids
+                )
                 if not targets_special:
                     dark_layer.remove_instance(instance)
 
         assert 0xffffffff not in new_dependencies
-
         # Update dependencies
-
-        # Add assets used by safe zones
-        new_dependencies = frozenset(new_dependencies)
-        if new_dependencies not in _all_deps_cache:
-            _all_deps_cache[new_dependencies] = recursive_dependencies_for_editor(
-                world.asset_manager, list(new_dependencies)
-            )
-
-        dependencies = light._raw.dependencies
-        assert isinstance(dependencies.dependencies_b, list)
-        for dep in _all_deps_cache[new_dependencies]:
-            dependencies.dependencies_b.append(construct.Container(
-                asset_id=dep.id,
-                asset_type=dep.type,
-            ))
-
-        for i in range(1, len(dependencies.dependencies_offset)):
-            dependencies.dependencies_offset[i] += len(new_dependencies)
-
-        # Add Safe Zone's module dep
-        module_dependencies = light._raw.module_dependencies
-        for module_dep in set(SafeZone.modules() + SafeZoneCrystal.modules()):
-            if module_dep not in module_dependencies.rel_module:
-                module_dependencies.rel_module.insert(0, module_dep)
-                for i in range(1, len(module_dependencies.rel_offset)):
-                    module_dependencies.rel_offset[i] += 1
+        _update_dependencies(world, light, new_dependencies)
 
 
 def apply_inverted(editor: PatcherEditor):
     _swap_dark_world(editor)
 
     _move_safe_zones(editor.get_mlvl(world_ids.TEMPLE_GROUNDS_MLVL), area_pairs.TG_PAIRS)
     _move_safe_zones(editor.get_mlvl(world_ids.AGON_WASTES_MLVL), area_pairs.AGON_PAIRS)
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/inverted/area_pairs.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/inverted/area_pairs.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/schema.json` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/schema.json`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/small_randomizations/__init__.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/small_randomizations/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from random import Random
+
 from open_prime_rando.echoes.small_randomizations.echo_locks import randomize_echo_locks
 from open_prime_rando.echoes.small_randomizations.minigyro_chamber import randomize_minigyro_chamber
 from open_prime_rando.echoes.small_randomizations.rubiks import randomize_rubiks_puzzles
-
 from open_prime_rando.patcher_editor import PatcherEditor
 
 
 def apply_small_randomizations(editor: PatcherEditor, configuration: dict):
     rng = Random(configuration["seed"])
-    
+
     if configuration["echo_locks"]:
         randomize_echo_locks(editor, rng)
-    
+
     if configuration["minigyro_chamber"]:
         randomize_minigyro_chamber(editor, rng)
-    
+
     if configuration["rubiks"]:
         randomize_rubiks_puzzles(editor, rng)
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/small_randomizations/echo_locks.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/small_randomizations/echo_locks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 import random
 
 from open_prime_rando.echoes.asset_ids.sanctuary_fortress import MAIN_GYRO_CHAMBER_MREA, SENTINELS_PATH_MREA
 from open_prime_rando.echoes.asset_ids.temple_grounds import PROFANE_PATH_MREA
+from open_prime_rando.echoes.asset_ids.world import SANCTUARY_FORTRESS_MLVL, TEMPLE_GROUNDS_MLVL
 from open_prime_rando.patcher_editor import PatcherEditor
-from retro_data_structures.enums.echoes import ScanSpeed
+from retro_data_structures.enums.echoes import Message, ScanSpeed, State
 from retro_data_structures.formats.scan import Scan
 from retro_data_structures.formats.strg import Strg
 from retro_data_structures.properties.echoes.objects.PointOfInterest import PointOfInterest
 from retro_data_structures.properties.echoes.objects.ScannableObjectInfo import ScannableObjectInfo
 from retro_data_structures.properties.echoes.objects.Sound import Sound
 from retro_data_structures.properties.echoes.objects.Switch import Switch
-from retro_data_structures.enums.echoes import State, Message
 
-ECHO_LOCK_MREAS = [MAIN_GYRO_CHAMBER_MREA, SENTINELS_PATH_MREA, PROFANE_PATH_MREA]
+ECHO_LOCK_MREAS = [
+    (SANCTUARY_FORTRESS_MLVL, MAIN_GYRO_CHAMBER_MREA),
+    (SANCTUARY_FORTRESS_MLVL, SENTINELS_PATH_MREA),
+    (TEMPLE_GROUNDS_MLVL, PROFANE_PATH_MREA)
+]
 ECHO_LOCK_STATES = [State.Zero, State.InternalState00, State.InternalState01, State.InternalState02]
 ECHO_LOCK_SOUNDS = [1005, 1006, 1007]
 
 
 def randomize_echo_locks(editor: PatcherEditor, rng: random.Random):
     # create key scan assets
     key_scan = editor.get_parsed_asset(0x2E7C4349, type_hint=Scan)
     scan_info = key_scan.scannable_object_info.get_properties_as(ScannableObjectInfo)
     key_strg = editor.get_parsed_asset(0x43894960, type_hint=Strg)
 
     all_paks = set()
-    for mrea in ECHO_LOCK_MREAS:
+    for _, mrea in ECHO_LOCK_MREAS:
         all_paks.update(editor.find_paks(mrea))
 
     key_scans = []
     for pitch in ["low", "medium", "high"]:
         key_strg.set_string(
             1,
             "Sonic detection gear needed to interface with this system."
@@ -44,27 +48,27 @@
         key_scans.append(scan_id)
 
     gate_scan = editor.get_parsed_asset(0x80A987AA, type_hint=Scan)
     gate_scan_info = gate_scan.scannable_object_info.get_properties_as(ScannableObjectInfo)
     gate_scan_info.scan_speed = ScanSpeed.Slow
     gate_strg = editor.get_parsed_asset(0x2820CC3D, type_hint=Strg)
 
-    for asset_id in ECHO_LOCK_MREAS:
-        mrea = editor.get_mrea(asset_id)
+    for mlvl_id, mrea_id in ECHO_LOCK_MREAS:
+        area = editor.get_area(mlvl_id, mrea_id)
         solution = [rng.randint(0, 2) for _ in range(4)]
 
-        counter = mrea.get_instance_by_name("Lock Solution Counter")
-        gate_poi = mrea.get_instance_by_name("(Gate) Echo Gate Scan Point")
-        correct_key_relays = [mrea.get_instance_by_name(f"[IN] Set Key {i} As Correct Choice") for i in range(3)]
-        lock_tone_players = [mrea.get_instance_by_name(f"(Gate) Lock {i} Tone") for i in range(4)]
-        key_switches = [mrea.get_instance_by_name(f"(Key {i}) Check Echo Key") for i in range(3)]
-        key_scan_points = [mrea.get_instance_by_name(f"(Key {i}) Scan Point") for i in range(3)]
+        counter = area.get_instance("Lock Solution Counter")
+        gate_poi = area.get_instance("(Gate) Echo Gate Scan Point")
+        correct_key_relays = [area.get_instance(f"[IN] Set Key {i} As Correct Choice") for i in range(3)]
+        lock_tone_players = [area.get_instance(f"(Gate) Lock {i} Tone") for i in range(4)]
+        key_switches = [area.get_instance(f"(Key {i}) Check Echo Key") for i in range(3)]
+        key_scan_points = [area.get_instance(f"(Key {i}) Scan Point") for i in range(3)]
 
         for relay in correct_key_relays:
-            counter.remove_connections(relay)
+            counter.remove_connections_from(relay)
 
         # Update all scan posts to have the updated scan text
         for scan_point, key_scan in zip(key_scan_points, key_scans):
             with scan_point.edit_properties(PointOfInterest) as scan:
                 scan.scan_info.scannable_info0 = key_scan
 
         for i, key in enumerate(solution):
@@ -74,19 +78,20 @@
                 tone.sound = ECHO_LOCK_SOUNDS[key]
 
         for i, switch in enumerate(key_switches):
             with switch.edit_properties(Switch) as props:
                 props.is_open = i == solution[0]
 
         # edit scan to indicate the solution
-        solution_text = "Sonic detection gear needed to interface with this system. The combination of its sonic locks is:\n"
-        solution_text += ", ".join((["Low", "Medium", "High"][key] for key in solution))
+        solution_text = ("Sonic detection gear needed to interface with this system. "
+                         "The combination of its sonic locks is:\n")
+        solution_text += ", ".join(["Low", "Medium", "High"][key] for key in solution)
         gate_strg.set_string(1, solution_text)
-        strg_id = editor.add_file(f"accessible_echo_gate_{asset_id}.STRG", gate_strg, all_paks)
+        strg_id = editor.add_file(f"accessible_echo_gate_{mrea_id}.STRG", gate_strg, all_paks)
 
         gate_scan_info.string = strg_id
         gate_scan.scannable_object_info.set_properties(gate_scan_info)
-        scan_id = editor.add_file(f"accessible_echo_gate_{asset_id}.SCAN", gate_scan, all_paks)
+        scan_id = editor.add_file(f"accessible_echo_gate_{mrea_id}.SCAN", gate_scan, all_paks)
 
         with gate_poi.edit_properties(PointOfInterest) as poi:
             poi.scan_info.scannable_info0 = scan_id
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/small_randomizations/minigyro_chamber.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from enum import Enum
 import random
+from enum import Enum
+
 from open_prime_rando.echoes.asset_ids.sanctuary_fortress import MINIGYRO_CHAMBER_MREA
+from open_prime_rando.echoes.asset_ids.world import SANCTUARY_FORTRESS_MLVL
 from open_prime_rando.patcher_editor import PatcherEditor
-
+from retro_data_structures.enums.echoes import Message, State
 from retro_data_structures.formats.strg import Strg
-from retro_data_structures.enums.echoes import State, Message
 
 
 class GyroColor(Enum):
     AMBER = 0
     COBALT = 1
     CRIMSON = 2
     EMERALD = 3
@@ -33,32 +34,30 @@
     State.InternalState01,
     State.InternalState02,
     State.InternalState03,
 ]
 
 
 def randomize_minigyro_chamber(editor: PatcherEditor, rng: random.Random):
-    mrea = editor.get_mrea(MINIGYRO_CHAMBER_MREA)
+    area = editor.get_area(SANCTUARY_FORTRESS_MLVL, MINIGYRO_CHAMBER_MREA)
     solution = [GyroColor.AMBER, GyroColor.COBALT, GyroColor.CRIMSON, GyroColor.EMERALD]
     rng.shuffle(solution)
 
-    counter = mrea.get_instance_by_name("Stage gate activator")
-    stage_gates = [mrea.get_instance_by_name(f"Stage gate {i+1}") for i in range(4)]
+    counter = area.get_instance("Stage gate activator")
+    stage_gates = [area.get_instance(f"Stage gate {i+1}") for i in range(4)]
 
     for i, gate in enumerate(stage_gates):
-        counter.remove_connections(gate)
+        counter.remove_connections_from(gate)
         for j, gyro in enumerate(solution):
             message = Message.Activate if i == gyro.value else Message.Deactivate
             counter.add_connection(GYRO_STATES[j], message, gate)
 
     # play jingle on the final gyro
-    stop_gyros = [mrea.get_instance_by_name(f"[IN/OUT] Stop gyroscope {i+1}") for i in range(4)]
-    jingle = mrea.get_instance_by_name(f"StreamedAudio - Event Jingle")
+    stop_gyros = [area.get_instance(f"[IN/OUT] Stop gyroscope {i+1}") for i in range(4)]
+    jingle = area.get_instance("StreamedAudio - Event Jingle")
 
-    stop_gyros[3].remove_connections(jingle)
+    stop_gyros[3].remove_connections_from(jingle)
     stop_gyros[solution[3].value].add_connection(State.Zero, Message.Play, jingle)
 
-    # print([f"{mrea.get_instance(c.target).name} - {c.state}: {c.message}" for c in counter.connections])
-
     scan = editor.get_file(0xFBFF349D, Strg)
-    solution_text = '\n'.join((gyro.text for gyro in solution))
+    solution_text = '\n'.join(gyro.text for gyro in solution)
     scan.set_string(1, f"Safety lockdown code is as follows:\n\n\n{solution_text}")
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/small_randomizations/rubiks.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/small_randomizations/rubiks.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,18 @@
+import random
 from dataclasses import dataclass
-from enum import Enum
 from pathlib import Path
-import random
 
-from retro_data_structures.properties.echoes.objects.Actor import Actor
-from retro_data_structures.crc import crc32
-from retro_data_structures.formats.cmdl import Cmdl
-from retro_data_structures.base_resource import RawResource
 from open_prime_rando.echoes.asset_ids.sanctuary_fortress import MAIN_GYRO_CHAMBER_MREA
-from retro_data_structures.enums.echoes import State, Message
-
+from open_prime_rando.echoes.asset_ids.world import SANCTUARY_FORTRESS_MLVL
 from open_prime_rando.patcher_editor import PatcherEditor
-
+from retro_data_structures.base_resource import RawResource
+from retro_data_structures.enums.echoes import Message, State
+from retro_data_structures.formats.cmdl import Cmdl
+from retro_data_structures.properties.echoes.objects.Actor import Actor
 
 RUBIKS_CUBES = {
     "Puzzle 1": [
         0x240013, 0x2401A4, 0x240145,
         0x24010A, 0x24000E, 0x240192,
         0x240139, 0x24013A, 0x240148,
     ],
@@ -65,15 +62,15 @@
         cmdl=0x8F25F715,
         old_txtr=0xFED23B81,
     )
 }
 
 
 def randomize_rubiks_puzzles(editor: PatcherEditor, rng: random.Random):
-    mrea = editor.get_mrea(MAIN_GYRO_CHAMBER_MREA)
+    area = editor.get_area(SANCTUARY_FORTRESS_MLVL, MAIN_GYRO_CHAMBER_MREA)
 
     # Add custom textures so colorblind players can distinguish the cubes
     for color in COLORS.values():
         txtr_id = editor.add_file(color.txtr_name, color.txtr, editor.find_paks(MAIN_GYRO_CHAMBER_MREA))
 
         cmdl = editor.get_file(color.cmdl, Cmdl)
         file_ids = cmdl.raw.material_sets[0].texture_file_ids
@@ -84,18 +81,17 @@
         solution = [
             COLORS["RED"], COLORS["RED"], COLORS["RED"],
             COLORS["GREEN"], COLORS["GREEN"], COLORS["GREEN"],
             COLORS["BLUE"], COLORS["BLUE"], COLORS["BLUE"],
         ]
         rng.shuffle(solution)
 
-        puzzle = mrea.get_instance_by_name(puzzle_name)
+        puzzle = area.get_instance(puzzle_name)
         for color, cube_id in zip(solution, cubes):
-            cube = mrea.get_instance(cube_id)
-            assert cube is not None
+            cube = area.get_instance(cube_id)
 
-            puzzle.remove_connections(cube)
+            puzzle.remove_connections_from(cube)
             puzzle.add_connection(color.state, Message.Attach, cube)
 
             with cube.edit_properties(Actor) as props:
                 props.model = color.cmdl
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/specific_area_patches.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/specific_area_patches.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import logging
 
 from construct import Container
-
 from open_prime_rando.echoes.asset_ids.agon_wastes import MINING_STATION_B_MREA, PORTAL_TERMINAL_MREA
 from open_prime_rando.echoes.asset_ids.torvus_bog import TORVUS_ENERGY_CONTROLLER_MREA, TORVUS_TEMPLE_MREA
 from open_prime_rando.echoes.asset_ids.world import TORVUS_BOG_MLVL
 from open_prime_rando.patcher_editor import PatcherEditor
-from retro_data_structures.formats.script_object import ScriptInstanceHelper
+from retro_data_structures.enums.echoes import Message, State
+from retro_data_structures.formats.script_object import ScriptInstance
 from retro_data_structures.game_check import Game
 from retro_data_structures.properties.echoes.objects.Counter import Counter
 from retro_data_structures.properties.echoes.objects.Relay import Relay
 from retro_data_structures.properties.echoes.objects.ScriptLayerController import ScriptLayerController
-from retro_data_structures.enums.echoes import State, Message
 
 LOG = logging.getLogger("echoes_patcher")
 
 
 def specific_patches(editor: PatcherEditor, area_patches: dict):
     # sand_mining(editor)
     # torvus_generator(editor)
@@ -29,16 +28,16 @@
 
     properties = post_pickup_relay.get_properties()
     assert isinstance(properties, Relay)
     properties.editor_properties.active = True
     post_pickup_relay.set_properties(properties)
 
 
-def create_layer_controller(area_id: int, layer: int, dynamic: bool = False) -> ScriptInstanceHelper:
-    layer_controller = ScriptInstanceHelper.new_instance(Game.ECHOES, "SLCT")
+def create_layer_controller(area_id: int, layer: int, dynamic: bool = False) -> ScriptInstance:
+    layer_controller = ScriptInstance.new_instance(Game.ECHOES, "SLCT")
     props = layer_controller.get_properties()
     assert isinstance(props, ScriptLayerController)
 
     props.editor_properties.name = "Layer Controller"
     props.editor_properties.transform.Scale = Container({"X": 1.0, "Y": 1.0, "Z": 1.0})
     props.editor_properties.active = True
     props.editor_properties.unknown = 3
@@ -74,32 +73,29 @@
     obj.add_connection(State.Zero, Message.Increment, layer_cont2)
 
 
 def torvus_temple_crash(editor: PatcherEditor):
     """
     Remove cosmetic objects from Torvus Temple to minimize the chance of chance via alloc failure
     """
-    world = editor.get_mlvl(TORVUS_BOG_MLVL)
-    area = world.get_area(TORVUS_TEMPLE_MREA)
+    area = editor.get_area(TORVUS_BOG_MLVL, TORVUS_TEMPLE_MREA)
+
+    to_remove = [
+        "Thrust1",
+        "Thrust1",
+        "Thrust2",
+        "Thrust2",
+        "Looping Thrust w/Doppler",
+        "Looping Thrust w/Doppler",
+        "GENERATE GIBS",
+    ]
+    to_remove.extend(["SwampCrateDebris"] * 7)
 
-    default = area.get_layer("Default")
-    first_pass = area.get_layer("1st Pass")
-    second_pass = area.get_layer("2nd PAss")
-
-    for obj in ["Thrust1", "Thrust1", "Thrust2", "Thrust2", "Looping Thrust w/Doppler", "Looping Thrust w/Doppler"]:
-        first_pass.remove_instance(obj)
-
-    for obj in ["GENERATE GIBS"]:
-        second_pass.remove_instance(obj)
-
-    # These are generated objects, so to remove these we need to change the generated objects layer
-    # Since that isn't properly exposed by RDS, let's skip for now
-    # debris = ["SwampCrateDebris"] * 7
-    # for obj in ["GibFlash", "Sound - Swamp Crate Gib"] + debris:
-    #     default.remove_instance(obj)
+    for obj in to_remove:
+        area.remove_instance(obj)
 
 
 def agon_wastes_portal_terminal_puzzle_patch(editor: PatcherEditor):
     """
     Patches Agon Wastes - Portal Terminal to behave like in GC NTSC-U/PAL
     In GC NTSC-J version a counter was added to check for each cork to be broken
     """
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes/vulnerabilities.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes/vulnerabilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from retro_data_structures.enums import echoes
-
 from retro_data_structures.properties.echoes.archetypes.DamageVulnerability import DamageVulnerability
 from retro_data_structures.properties.echoes.archetypes.WeaponVulnerability import WeaponVulnerability
 
-
 reflect = WeaponVulnerability(damage_multiplier=0, effect=echoes.Effect.Reflect)
 vulnerable = WeaponVulnerability(damage_multiplier=100, effect=echoes.Effect.Normal)
 immune = WeaponVulnerability(damage_multiplier=0, effect=echoes.Effect.Normal, ignore_radius=True)
 
 
 resist_all_vuln = DamageVulnerability(
     power=reflect, dark=reflect, light=reflect, annihilator=reflect,
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/echoes_patcher.py` & `open-prime-rando-0.6.2/src/open_prime_rando/echoes_patcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,45 @@
 import json
 import logging
+from collections.abc import Callable
 from pathlib import Path
-from typing import Callable
+
+from retro_data_structures.asset_manager import FileProvider
+from retro_data_structures.formats.mrea import Area
+from retro_data_structures.formats.strg import Strg
+from retro_data_structures.game_check import Game
 
 from open_prime_rando import dynamic_schema
-from open_prime_rando.echoes import specific_area_patches, asset_ids, dock_lock_rando
+from open_prime_rando.echoes import asset_ids, dock_lock_rando, specific_area_patches
 from open_prime_rando.echoes.elevators import auto_enabled_elevator_patches
 from open_prime_rando.echoes.elevators.elevator_rando import patch_elevator
 from open_prime_rando.echoes.inverted import apply_inverted
 from open_prime_rando.echoes.small_randomizations import apply_small_randomizations
 from open_prime_rando.patcher_editor import PatcherEditor
 from open_prime_rando.unique_area_name import get_name_for_area
 from open_prime_rando.validator_with_default import DefaultValidatingDraft7Validator
-from retro_data_structures.asset_manager import FileProvider
-from retro_data_structures.formats.mlvl import AreaWrapper
-from retro_data_structures.game_check import Game
-from retro_data_structures.formats.strg import Strg
 
 LOG = logging.getLogger("echoes_patcher")
 
 
 def _read_schema():
     with Path(__file__).parent.joinpath("echoes", "schema.json").open() as f:
         return json.load(f)
 
 
-def apply_area_modifications(editor: PatcherEditor, configuration: dict[str, dict], status_update: Callable[[str, float], None]):
+def apply_area_modifications(editor: PatcherEditor, configuration: dict[str, dict],
+                             status_update: Callable[[str, float], None]):
     num_areas = sum(len(world_config["areas"]) for world_config in configuration.values())
     areas_processed = 0.0
 
     for world_name, world_config in configuration.items():
         world_meta = asset_ids.world.load_dedicated_file(world_name)
         mlvl = editor.get_mlvl(asset_ids.world.NAME_TO_ID_MLVL[world_name])
 
-        areas_by_name: dict[str, AreaWrapper] = {
+        areas_by_name: dict[str, Area] = {
             get_name_for_area(area): area
             for area in mlvl.areas
         }
 
         for i, (area_name, area) in enumerate(areas_by_name.items()):
             if area_name not in world_config["areas"]:
                 continue
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/p1r_patcher.py` & `open-prime-rando-0.6.2/src/open_prime_rando/p1r_patcher.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import json
 import logging
 from pathlib import Path
 
-from open_prime_rando.patcher_editor import PatcherEditor
-from open_prime_rando.validator_with_default import DefaultValidatingDraft7Validator
 from retro_data_structures.asset_manager import FileProvider
 from retro_data_structures.game_check import Game
 
+from open_prime_rando.patcher_editor import PatcherEditor
+from open_prime_rando.validator_with_default import DefaultValidatingDraft7Validator
+
 LOG = logging.getLogger("p1r_patcher")
 
 
 def _read_schema():
     with Path(__file__).parent.joinpath("prime_remastered", "schema.json").open() as f:
         return json.load(f)
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/patcher_editor.py` & `open-prime-rando-0.6.2/src/open_prime_rando/patcher_editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import io
 import typing
 from concurrent.futures import ThreadPoolExecutor
 from pathlib import Path
 
 from ppc_asm.dol_file import DolEditor, DolHeader
 from retro_data_structures.asset_manager import AssetManager, FileProvider
-from retro_data_structures.base_resource import Resource, BaseResource, NameOrAssetId, RawResource, AssetId
+from retro_data_structures.base_resource import AssetId, BaseResource, NameOrAssetId, RawResource, Resource
 from retro_data_structures.crc import crc32
-from retro_data_structures.formats.mlvl import Mlvl, AreaWrapper
-from retro_data_structures.formats.mrea import Mrea
+from retro_data_structures.formats.mlvl import Mlvl
+from retro_data_structures.formats.mrea import Area
 from retro_data_structures.game_check import Game
 
 T = typing.TypeVar("T")
 
 
 class MemoryDol(DolEditor):
     def __init__(self, dol: bytes):
@@ -36,38 +36,35 @@
         self.memory_files = {}
 
         if game in [Game.PRIME, Game.ECHOES]:
             self.dol = MemoryDol(provider.get_dol())
         else:
             self.dol = None
 
-    def get_file(self, path: NameOrAssetId, type_hint: typing.Type[T] = BaseResource) -> T:
+    def get_file(self, path: NameOrAssetId, type_hint: type[T] = BaseResource) -> T:
         if path not in self.memory_files:
             self.memory_files[path] = self.get_parsed_asset(path, type_hint=type_hint)
         return self.memory_files[path]
 
     def get_mlvl(self, name: NameOrAssetId) -> Mlvl:
         return self.get_file(name, Mlvl)
 
-    def get_mrea(self, name: NameOrAssetId) -> Mrea:
-        return self.get_file(name, Mrea)
-
-    def get_area_helper(self, mlvl: NameOrAssetId, mrea: NameOrAssetId) -> AreaWrapper:
+    def get_area(self, mlvl: NameOrAssetId, mrea: NameOrAssetId) -> Area:
         return self.get_mlvl(mlvl).get_area(mrea)
 
     def flush_modified_assets(self):
         with ThreadPoolExecutor() as executor:
             for name, resource in self.memory_files.items():
                 executor.submit(self.replace_asset, name, resource)
         self.memory_files = {}
 
     def add_file(self,
                  name: str,
-                 asset: typing.Union[RawResource, BaseResource],
-                 paks: typing.Iterable[str]
+                 asset: RawResource | BaseResource,
+                 paks: typing.Iterable[str] = ()
                  ) -> AssetId:
         asset_id = crc32(name)
         self.register_custom_asset_name(name, asset_id)
         self.add_new_asset(name, asset, paks)
         return asset_id
 
     def save_modifications(self, output_path: Path):
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando/validator_with_default.py` & `open-prime-rando-0.6.2/src/open_prime_rando/validator_with_default.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,18 +5,17 @@
     validate_properties = validator_class.VALIDATORS["properties"]
 
     def set_defaults(validator, properties, instance, schema):
         for prop, subschema in properties.items():
             if "default" in subschema:
                 instance.setdefault(prop, subschema["default"])
 
-        for error in validate_properties(
+        yield from validate_properties(
                 validator, properties, instance, schema,
-        ):
-            yield error
+        )
 
     return validators.extend(
         validator_class, {"properties": set_defaults},
     )
 
 
 DefaultValidatingDraft7Validator = extend_with_default(Draft7Validator)
```

### Comparing `open-prime-rando-0.6.1/open_prime_rando.egg-info/PKG-INFO` & `open-prime-rando-0.6.2/src/open_prime_rando.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: open-prime-rando
-Version: 0.6.1
+Version: 0.6.2
 Summary: An open source randomizer patcher for Metroid Prime 2 and 3.
-Home-page: https://github.com/randovania/open-prime-rando
 Author: Henrique Gemignani
+Project-URL: Homepage, https://github.com/randovania/open-prime-rando
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 
 # Open Prime Rando
 Open Source randomizer patcher for Prime 2 and eventually 3.
```

### Comparing `open-prime-rando-0.6.1/tests/test_echoes_custom_Assets.py` & `open-prime-rando-0.6.2/tests/test_echoes_custom_Assets.py`

 * *Files identical despite different names*

### Comparing `open-prime-rando-0.6.1/tools/asset_id_files.py` & `open-prime-rando-0.6.2/tools/asset_id_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import argparse
 import os.path
 from pathlib import Path
 
-from retro_data_structures.asset_manager import IsoFileProvider
-from retro_data_structures.formats import Strg, Mrea
-from retro_data_structures.game_check import Game
-from retro_data_structures.properties.shared_objects import Dock
 import retro_data_structures.exceptions
-
 from open_prime_rando.patcher_editor import PatcherEditor
 from open_prime_rando.unique_area_name import CUSTOM_AREA_NAMES
+from retro_data_structures.asset_manager import IsoFileProvider
+from retro_data_structures.formats import Mrea, Strg
+from retro_data_structures.game_check import Game
+from retro_data_structures.properties.shared_objects import Dock
 
 _CUSTOM_WORLD_NAMES = {
     Game.ECHOES: {
         0x69802220: "FrontEnd",
         0xA50A80CC: "M01_SidehopperStation",
         0xAE171602: "M02_Spires",
         0xE3B0C703: "M03_CrossfireChaos",
@@ -23,14 +22,17 @@
     }
 }
 _CUSTOM_AREA_NAMES = {
     Game.ECHOES: CUSTOM_AREA_NAMES,
 }
 
 
+# Complexity
+# ruff: noqa: C901
+
 def filter_name(s: str) -> str:
     result = s.replace("!", "").replace(" ", "_").replace("'", "").replace(
         '"', "").replace("(", "").replace(")", "").upper()
     while result and not result[0].isalpha():
         result = result[1:]
     return result
 
@@ -73,15 +75,15 @@
     for value in editor.all_asset_ids():
         if editor.get_asset_type(value).lower() != "mlvl":
             continue
 
         mlvl = editor.get_mlvl(value)
 
         try:
-            strg = editor.get_parsed_asset(mlvl.raw.world_name_id, type_hint=Strg)
+            strg = editor.get_file(mlvl.raw.world_name_id, type_hint=Strg)
             world_name = strg.raw.string_tables[0].strings[0].string
         except retro_data_structures.exceptions.UnknownAssetId:
             if value not in custom_world_names:
                 print(f"Skipping MLVL {value}: no name found")
                 continue
             world_name = custom_world_names[value]
 
@@ -90,24 +92,24 @@
 
         area_names = {}
         mapa_names = {}
         dock_names = {}
 
         for area, mapa in zip(mlvl.raw.areas, mlvl.mapw.mapa_ids):
             try:
-                strg = editor.get_parsed_asset(area.area_name_id, type_hint=Strg)
+                strg = editor.get_file(area.area_name_id, type_hint=Strg)
                 area_name = strg.raw.string_tables[0].strings[0].string
             except retro_data_structures.exceptions.UnknownAssetId:
                 area_name = area.internal_area_name
             area_name = _CUSTOM_AREA_NAMES[editor.target_game].get(area.area_mrea_id, area_name)
 
             assert area_name not in area_names, area_name
             area_names[area_name] = area.area_mrea_id
             mapa_names[area_name] = mapa
-            mrea = editor.get_parsed_asset(area_names[area_name], type_hint=Mrea)
+            mrea = editor.get_file(area_names[area_name], type_hint=Mrea)
 
             docks = {}
             for layer in mrea.script_layers:
                 for obj in layer.instances:
                     if obj.type_name == "DOCK":
                         dock: Dock = obj.get_properties_as(Dock)
                         assert dock.get_name() not in docks
```

