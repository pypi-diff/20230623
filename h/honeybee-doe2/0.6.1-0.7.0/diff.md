# Comparing `tmp/honeybee-doe2-0.6.1.tar.gz` & `tmp/honeybee-doe2-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-doe2-0.6.1.tar", last modified: Tue Jun 13 23:52:13 2023, max compression
+gzip compressed data, was "dist/honeybee-doe2-0.7.0.tar", last modified: Fri Jun 23 16:05:47 2023, max compression
```

## Comparing `honeybee-doe2-0.6.1.tar` & `honeybee-doe2-0.7.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/_extend_honeybee_doe2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/cli/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/geometry/polygon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/aperture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/constructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/exposedfloor.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/groundcontact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/hvac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/glass_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/run_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/sitebldg.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/title.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/interiorfloor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/roof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/shades.py
--rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/story.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/properties/wall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/utils/doe_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/utils/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/honeybee_doe2/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-13 23:52:12.000000 honeybee-doe2-0.6.1/honeybee_doe2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/honeybee_doe2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 23:52:12.000000 honeybee-doe2-0.6.1/honeybee_doe2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-13 23:52:12.000000 honeybee-doe2-0.6.1/honeybee_doe2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 23:52:12.000000 honeybee-doe2-0.6.1/honeybee_doe2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 23:52:12.000000 honeybee-doe2-0.6.1/honeybee_doe2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 23:52:13.000000 honeybee-doe2-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-13 23:51:09.000000 honeybee-doe2-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/_extend_honeybee_doe2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/cli/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/geometry/polygon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/constructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/exposedfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/groundcontact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/hvac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/glass_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/run_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/sitebldg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/interiorfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/roof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/shades.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/properties/wall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/utils/doe_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/utils/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/honeybee_doe2/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-23 16:05:46.000000 honeybee-doe2-0.7.0/honeybee_doe2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/honeybee_doe2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:05:46.000000 honeybee-doe2-0.7.0/honeybee_doe2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 16:05:46.000000 honeybee-doe2-0.7.0/honeybee_doe2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 16:05:46.000000 honeybee-doe2-0.7.0/honeybee_doe2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 16:05:46.000000 honeybee-doe2-0.7.0/honeybee_doe2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-23 16:05:47.000000 honeybee-doe2-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-23 16:04:45.000000 honeybee-doe2-0.7.0/setup.py
```

### Comparing `honeybee-doe2-0.6.1/LICENSE` & `honeybee-doe2-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/PKG-INFO` & `honeybee-doe2-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.6.1
+Version: 0.7.0
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.6.1/README.md` & `honeybee-doe2-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/_extend_honeybee_doe2.py` & `honeybee-doe2-0.7.0/honeybee_doe2/_extend_honeybee_doe2.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/cli/translate.py` & `honeybee-doe2-0.7.0/honeybee_doe2/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/geometry/polygon.py` & `honeybee-doe2-0.7.0/honeybee_doe2/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/aperture.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/aperture.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/constructions.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/constructions.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/exposedfloor.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/exposedfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/face.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/groundcontact.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/groundcontact.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/hvac.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/hvac.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/blocks.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/blocks.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/compliance.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/compliance.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/glass_types.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/glass_types.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/run_period.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/run_period.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/inputils/sitebldg.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/inputils/sitebldg.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/interiorfloor.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/interiorfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/materials.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/materials.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/model.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/model.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/roof.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/roof.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,19 +19,19 @@
         spc = ''
         obj_lines = []
 
         obj_lines.append('"{}" = ROOF'.format(p_name))
         obj_lines.append('\n   POLYGON           = "{}"'.format(p_name+' Plg'))
         obj_lines.append('\n   CONSTRUCTION      = "{}_c"'.format(
             short_name(constr, 30)))
-        obj_lines.append('\n  TILT              =  {}'.format(tilt))
-        obj_lines.append('\n  AZIMUTH           =  {}'.format(azimuth))
-        obj_lines.append('\n  X                 =  {}'.format(origin_pt.x))
-        obj_lines.append('\n  Y                 =  {}'.format(origin_pt.y))
-        obj_lines.append('\n  Z                 =  {}\n  ..\n'.format(origin_pt.z))
+        obj_lines.append('\n   TILT              =  {}'.format(tilt))
+        obj_lines.append('\n   AZIMUTH           =  {}'.format(azimuth))
+        obj_lines.append('\n   X                 =  {}'.format(origin_pt.x))
+        obj_lines.append('\n   Y                 =  {}'.format(origin_pt.y))
+        obj_lines.append('\n   Z                 =  {}\n  ..\n'.format(origin_pt.z))
         temp_str = spc.join([line for line in obj_lines])
 
         doe_windows = [
             Window(ap, self.face) for ap in self.face.apertures
         ]
 
         nl = '\n'
```

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/room.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/room.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/shades.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/shades.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/story.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/story.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/properties/wall.py` & `honeybee-doe2-0.7.0/honeybee_doe2/properties/wall.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,16 @@
         if b_c is not None:
             if str(b_c) == 'Outdoors':
                 return 'EXTERIOR-WALL'
             elif str(b_c) == 'Ground':
                 return 'UNDERGROUND-WALL'
             elif str(b_c) == 'Surface':
                 return 'INTERIOR-WALL'
+            elif str(b_c) == 'Adiabatic':
+                return 'INTERIOR-WALL'
 
 
 class DoeWall:
     def __init__(self, face):
         self.face = face
 
     def to_inp(self, space_origin):
@@ -42,23 +44,30 @@
         obj_lines.append('\n  POLYGON           = "{}"'.format(f'{p_name} Plg'))
         obj_lines.append('\n  CONSTRUCTION      = "{}_c"'.format(short_name(constr, 30)))
         obj_lines.append('\n  TILT              =  {}'.format(tilt))
         obj_lines.append('\n  AZIMUTH           =  {}'.format(azimuth))
         obj_lines.append('\n  X                 =  {}'.format(origin_pt.x))
         obj_lines.append('\n  Y                 =  {}'.format(origin_pt.y))
         obj_lines.append('\n  Z                 =  {}'.format(origin_pt.z))
-        if wall_typology == 'INTERIOR-WALL':
+        if wall_typology == 'INTERIOR-WALL' and str(
+                self.face.boundary_condition) == 'Surface':
             if self.face.user_data:
                 next_to = self.face.user_data['adjacent_room']
                 obj_lines.append('\n  NEXT-TO           =  "{}"'.format(next_to))
             else:
                 print(
                     f'{self.face.display_name} is an interior face but is missing '
                     'adjacent room info in user data.'
                 )
+        if wall_typology == 'INTERIOR-WALL' and str(
+                self.face.boundary_condition) == 'Adiabatic':
+            obj_lines.append('\n  INT-WALL-TYPE = ADIABATIC')
+            next_to = self.face.parent.display_name
+            obj_lines.append('\n  NEXT-TO           =  "{}"'.format(next_to))
+
         obj_lines.append('\n  ..\n')
 
         temp_str = spc.join([line for line in obj_lines])
 
         doe_windows = [
             Window(ap, self.face) for ap in self.face.apertures
         ]
```

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/utils/doe_formatters.py` & `honeybee-doe2-0.7.0/honeybee_doe2/utils/doe_formatters.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/utils/geometry.py` & `honeybee-doe2-0.7.0/honeybee_doe2/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2/writer.py` & `honeybee-doe2-0.7.0/honeybee_doe2/writer.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2.egg-info/PKG-INFO` & `honeybee-doe2-0.7.0/honeybee_doe2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.6.1
+Version: 0.7.0
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.6.1/honeybee_doe2.egg-info/SOURCES.txt` & `honeybee-doe2-0.7.0/honeybee_doe2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.6.1/setup.py` & `honeybee-doe2-0.7.0/setup.py`

 * *Files identical despite different names*

