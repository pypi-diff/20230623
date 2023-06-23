# Comparing `tmp/geomapi-0.3.1.tar.gz` & `tmp/geomapi-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapi-0.3.1.tar", last modified: Tue May 16 14:34:17 2023, max compression
+gzip compressed data, was "geomapi-0.3.2.tar", last modified: Fri Jun 23 07:59:17 2023, max compression
```

## Comparing `geomapi-0.3.1.tar` & `geomapi-0.3.2.tar`

### file list

```diff
@@ -1,70 +1,71 @@
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.636665 geomapi-0.3.1/
--rw-rw-rw-   0 root         (0) daemon       (1)     1133 2023-05-16 14:32:42.000000 geomapi-0.3.1/LICENSE
--rw-r--r--   0 root         (0) daemon       (1)     1508 2023-05-16 14:34:17.636665 geomapi-0.3.1/PKG-INFO
--rw-rw-rw-   0 root         (0) daemon       (1)      890 2023-05-16 14:32:42.000000 geomapi-0.3.1/README.md
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.628665 geomapi-0.3.1/developmenttests/
--rw-rw-rw-   0 root         (0) daemon       (1)    42245 2023-05-16 14:32:42.000000 geomapi-0.3.1/developmenttests/QualityCompare.py
--rw-rw-rw-   0 root         (0) daemon       (1)     5108 2023-05-16 14:32:42.000000 geomapi-0.3.1/developmenttests/QualityCompare_gui.py
--rw-rw-rw-   0 root         (0) daemon       (1)        0 2023-05-16 14:32:53.000000 geomapi-0.3.1/developmenttests/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)      119 2023-05-16 14:32:43.000000 geomapi-0.3.1/developmenttests/context.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2241 2023-05-16 14:32:43.000000 geomapi-0.3.1/developmenttests/ifc_to_nodes.py
--rw-rw-rw-   0 root         (0) daemon       (1)     4911 2023-05-16 14:32:43.000000 geomapi-0.3.1/developmenttests/import_e57.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.628665 geomapi-0.3.1/geomapi/
--rw-rw-rw-   0 root         (0) daemon       (1)       64 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/nodes/
--rw-rw-rw-   0 root         (0) daemon       (1)      372 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)    12147 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/bimnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    16209 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/geometrynode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    35014 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/imagenode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     9033 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/linesetnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     7742 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/meshnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    22483 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/node.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2101 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/orthonode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    17538 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/pointcloudnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    27142 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/sessionnode.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/tools/
--rw-rw-rw-   0 root         (0) daemon       (1)    45777 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/tools/alignmenttools/
--rw-rw-rw-   0 root         (0) daemon       (1)     2975 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/alignmenttools/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)    17867 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/alignmenttools/match.py
--rw-rw-rw-   0 root         (0) daemon       (1)      604 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/alignmenttools/params.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/tools/completiontools/
--rw-rw-rw-   0 root         (0) daemon       (1)     5455 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/completiontools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/tools/inspectiontools/
--rw-rw-rw-   0 root         (0) daemon       (1)      306 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/inspectiontools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/tools/machinelearningtools/
--rw-rw-rw-   0 root         (0) daemon       (1)    13233 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/machinelearningtools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/tools/progresstools/
--rw-rw-rw-   0 root         (0) daemon       (1)    41267 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/progresstools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/tools/validationtools/
--rw-rw-rw-   0 root         (0) daemon       (1)    30354 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/validationtools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/utils/
--rw-rw-rw-   0 root         (0) daemon       (1)    38758 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/utils/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)   119403 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/utils/geometryutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)     6335 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/utils/geospatialutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)    26061 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/utils/imageutils.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.628665 geomapi-0.3.1/geomapi.egg-info/
--rw-r--r--   0 root         (0) daemon       (1)     1508 2023-05-16 14:34:17.000000 geomapi-0.3.1/geomapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) daemon       (1)     1539 2023-05-16 14:34:17.000000 geomapi-0.3.1/geomapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) daemon       (1)        1 2023-05-16 14:34:17.000000 geomapi-0.3.1/geomapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) daemon       (1)      194 2023-05-16 14:34:17.000000 geomapi-0.3.1/geomapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) daemon       (1)       30 2023-05-16 14:34:17.000000 geomapi-0.3.1/geomapi.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) daemon       (1)       80 2023-05-16 14:32:43.000000 geomapi-0.3.1/pyproject.toml
--rw-rw-rw-   0 root         (0) daemon       (1)      921 2023-05-16 14:34:17.636665 geomapi-0.3.1/setup.cfg
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.636665 geomapi-0.3.1/test/
--rw-rw-rw-   0 root         (0) daemon       (1)      128 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)     1787 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_alignmenttools.py
--rw-rw-rw-   0 root         (0) daemon       (1)    18912 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_bimnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2023 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_completiontools.py
--rw-rw-rw-   0 root         (0) daemon       (1)    14578 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_geometrynode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    24158 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_geometryutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)     1112 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_geospatialutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2392 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_imageutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)    13030 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_imgnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    12504 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_meshnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    15672 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_node.py
--rw-rw-rw-   0 root         (0) daemon       (1)    12842 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_pointcloudnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     4270 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_progresstools.py
--rw-rw-rw-   0 root         (0) daemon       (1)     9408 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_sessionnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    15091 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_tools.py
--rw-rw-rw-   0 root         (0) daemon       (1)    27056 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_utils.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-06-23 07:59:17.617733 geomapi-0.3.2/
+-rw-rw-rw-   0 root         (0) daemon       (1)     1133 2023-06-23 07:57:45.000000 geomapi-0.3.2/LICENSE
+-rw-r--r--   0 root         (0) daemon       (1)     1508 2023-06-23 07:59:17.621734 geomapi-0.3.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) daemon       (1)      890 2023-06-23 07:57:45.000000 geomapi-0.3.2/README.md
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-06-23 07:59:17.613733 geomapi-0.3.2/developmenttests/
+-rw-rw-rw-   0 root         (0) daemon       (1)    42245 2023-06-23 07:57:45.000000 geomapi-0.3.2/developmenttests/QualityCompare.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     5108 2023-06-23 07:57:45.000000 geomapi-0.3.2/developmenttests/QualityCompare_gui.py
+-rw-rw-rw-   0 root         (0) daemon       (1)        0 2023-06-23 07:57:56.000000 geomapi-0.3.2/developmenttests/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)      119 2023-06-23 07:57:46.000000 geomapi-0.3.2/developmenttests/context.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2241 2023-06-23 07:57:46.000000 geomapi-0.3.2/developmenttests/ifc_to_nodes.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     4911 2023-06-23 07:57:46.000000 geomapi-0.3.2/developmenttests/import_e57.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-06-23 07:59:17.613733 geomapi-0.3.2/geomapi/
+-rw-rw-rw-   0 root         (0) daemon       (1)       64 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-06-23 07:59:17.613733 geomapi-0.3.2/geomapi/nodes/
+-rw-rw-rw-   0 root         (0) daemon       (1)      372 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/nodes/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    12147 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/nodes/bimnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    16209 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/nodes/geometrynode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    35016 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/nodes/imagenode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     9033 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/nodes/linesetnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     7688 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/nodes/meshnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    22483 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/nodes/node.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2101 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/nodes/orthonode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    17538 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/nodes/pointcloudnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    27142 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/nodes/sessionnode.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-06-23 07:59:17.613733 geomapi-0.3.2/geomapi/tools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    47786 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/tools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-06-23 07:59:17.617733 geomapi-0.3.2/geomapi/tools/alignmenttools/
+-rw-rw-rw-   0 root         (0) daemon       (1)     2975 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/tools/alignmenttools/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    17867 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/tools/alignmenttools/match.py
+-rw-rw-rw-   0 root         (0) daemon       (1)      604 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/tools/alignmenttools/params.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-06-23 07:59:17.617733 geomapi-0.3.2/geomapi/tools/completiontools/
+-rw-rw-rw-   0 root         (0) daemon       (1)     5455 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/tools/completiontools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-06-23 07:59:17.617733 geomapi-0.3.2/geomapi/tools/inspectiontools/
+-rw-rw-rw-   0 root         (0) daemon       (1)      306 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/tools/inspectiontools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-06-23 07:59:17.617733 geomapi-0.3.2/geomapi/tools/machinelearningtools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    13233 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/tools/machinelearningtools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-06-23 07:59:17.617733 geomapi-0.3.2/geomapi/tools/progresstools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    41295 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/tools/progresstools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-06-23 07:59:17.617733 geomapi-0.3.2/geomapi/tools/validationtools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    33519 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/tools/validationtools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-06-23 07:59:17.617733 geomapi-0.3.2/geomapi/utils/
+-rw-rw-rw-   0 root         (0) daemon       (1)    38758 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/utils/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    33790 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/utils/cadutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)   128098 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/utils/geometryutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     8161 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/utils/geospatialutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    26061 2023-06-23 07:57:46.000000 geomapi-0.3.2/geomapi/utils/imageutils.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-06-23 07:59:17.613733 geomapi-0.3.2/geomapi.egg-info/
+-rw-r--r--   0 root         (0) daemon       (1)     1508 2023-06-23 07:59:17.000000 geomapi-0.3.2/geomapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) daemon       (1)     1565 2023-06-23 07:59:17.000000 geomapi-0.3.2/geomapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) daemon       (1)        1 2023-06-23 07:59:17.000000 geomapi-0.3.2/geomapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) daemon       (1)      194 2023-06-23 07:59:17.000000 geomapi-0.3.2/geomapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) daemon       (1)       30 2023-06-23 07:59:17.000000 geomapi-0.3.2/geomapi.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) daemon       (1)       80 2023-06-23 07:57:46.000000 geomapi-0.3.2/pyproject.toml
+-rw-rw-rw-   0 root         (0) daemon       (1)      921 2023-06-23 07:59:17.621734 geomapi-0.3.2/setup.cfg
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-06-23 07:59:17.617733 geomapi-0.3.2/test/
+-rw-rw-rw-   0 root         (0) daemon       (1)      128 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     1787 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/test_alignmenttools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    18912 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/test_bimnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2023 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/test_completiontools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    14578 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/test_geometrynode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    24158 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/test_geometryutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     1112 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/test_geospatialutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2392 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/test_imageutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    13030 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/test_imgnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    12504 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/test_meshnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    15672 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/test_node.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    12842 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/test_pointcloudnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     4270 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/test_progresstools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     9408 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/test_sessionnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    15121 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/test_tools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    27056 2023-06-23 07:57:46.000000 geomapi-0.3.2/test/test_utils.py
```

### Comparing `geomapi-0.3.1/LICENSE` & `geomapi-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/PKG-INFO` & `geomapi-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapi
-Version: 0.3.1
+Version: 0.3.2
 Summary: A standard library to manage geomatic data
 Home-page: https://geomatics.pages.gitlab.kuleuven.be/research-projects/geomapi/
 Author: Bassier M., De Geyter S., De Winter H., Vermandere J. @ Geomatics KU Leuven
 License: MIT
 Keywords: Geomatics,alignment,monitoring,validation,progress,point clouds,computer vision,deep learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geomapi-0.3.1/README.md` & `geomapi-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/developmenttests/QualityCompare.py` & `geomapi-0.3.2/developmenttests/QualityCompare.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/developmenttests/QualityCompare_gui.py` & `geomapi-0.3.2/developmenttests/QualityCompare_gui.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/developmenttests/ifc_to_nodes.py` & `geomapi-0.3.2/developmenttests/ifc_to_nodes.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/developmenttests/import_e57.py` & `geomapi-0.3.2/developmenttests/import_e57.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/geomapi/nodes/bimnode.py` & `geomapi-0.3.2/geomapi/nodes/bimnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/geomapi/nodes/geometrynode.py` & `geomapi-0.3.2/geomapi/nodes/geometrynode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/geomapi/nodes/imagenode.py` & `geomapi-0.3.2/geomapi/nodes/imagenode.py`

 * *Files 0% similar despite different names*

```diff
@@ -622,15 +622,15 @@
 
         Features:
             1. cartesianTransform (np.array(4x4))\n
             2. sxy: accuracy in XY (m)\n
             3. sz: accuracy in Z (m) \n
 
         Returns:
-            bool: True if metadata is sucesfully parsed
+            bool: True if metadata is successfully parsed
         """
         if self.xmlPath is None or not os.path.exists(self.xmlPath):
             return False
 
         if (getattr(self,'cartesianTransform',None) is not None and
             getattr(self,'sxy',None) is not None and
             getattr(self,'sz',None) is not None ):
```

### Comparing `geomapi-0.3.1/geomapi/nodes/linesetnode.py` & `geomapi-0.3.2/geomapi/nodes/linesetnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/geomapi/nodes/meshnode.py` & `geomapi-0.3.2/geomapi/nodes/meshnode.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         Args:
             1. open3d.geometry.TriangleMesh
             2. trimesh.Trimesh
 
         Raises:
             ValueError: Resource must be an o3d.geometry.TriangleMesh with len(resource.triangles) >=2 or an trimesh.Trimesh instance.
         """
-        if 'TriangleMesh' in str(type(value)) and len(value.triangles) >=2:
+        if 'TriangleMesh' in str(type(value)) and len(value.triangles) >=1:
             self._resource = value
         elif 'Trimesh' in str(type(value)):
             self._resource=value.as_open3d
         else:
             raise ValueError('Resource must be an o3d.geometry.TriangleMesh with len(resource.triangles) >=2 or an trimesh.Trimesh instance.')
 
     def get_resource(self)->o3d.geometry.TriangleMesh: 
@@ -162,33 +162,37 @@
         Returns:
             bool: True if exif data is successfully parsed
         """
         if (not self.resource or
             len(self.resource.triangles) <2):
             return False    
 
-        try:
-            if getattr(self,'pointCount',None) is None:
-                self.pointCount=len(self.resource.vertices)
-
-            if getattr(self,'faceCount',None) is None:
-                self.faceCount=len(self.resource.triangles)
-
-            if  getattr(self,'cartesianTransform',None) is None:
-                center=self.resource.get_center()  
-                self.cartesianTransform= np.array([[1,0,0,center[0]],
-                                                    [0,1,0,center[1]],
-                                                    [0,0,1,center[2]],
-                                                    [0,0,0,1]])
-
-            if getattr(self,'cartesianBounds',None) is  None:
-                self.cartesianBounds=gmu.get_cartesian_bounds(self.resource)
-            if getattr(self,'orientedBoundingBox',None) is  None:
+        if getattr(self,'pointCount',None) is None:
+            self.pointCount=len(self.resource.vertices)
+
+        if getattr(self,'faceCount',None) is None:
+            self.faceCount=len(self.resource.triangles)
+
+        if  getattr(self,'cartesianTransform',None) is None:
+            center=self.resource.get_center()  
+            self.cartesianTransform= np.array([[1,0,0,center[0]],
+                                                [0,1,0,center[1]],
+                                                [0,0,1,center[2]],
+                                                [0,0,0,1]])
+
+        if getattr(self,'cartesianBounds',None) is None:
+            self.cartesianBounds=gmu.get_cartesian_bounds(self.resource)
+        if getattr(self,'orientedBoundingBox',None) is  None:
+            try:
                 self.orientedBoundingBox=self.resource.get_oriented_bounding_box()
-            if getattr(self,'orientedBounds',None) is  None:
+            except:
+                pass
+        if getattr(self,'orientedBounds',None) is None:
+            try:
                 box=self.resource.get_oriented_bounding_box()
                 self.orientedBounds= np.asarray(box.get_box_points())
-            return True
-        except:
-            raise ValueError('Metadata extraction from resource failed')
+            except:
+                pass
+            
+
```

### Comparing `geomapi-0.3.1/geomapi/nodes/node.py` & `geomapi-0.3.2/geomapi/nodes/node.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/geomapi/nodes/orthonode.py` & `geomapi-0.3.2/geomapi/nodes/orthonode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/geomapi/nodes/pointcloudnode.py` & `geomapi-0.3.2/geomapi/nodes/pointcloudnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/geomapi/nodes/sessionnode.py` & `geomapi-0.3.2/geomapi/nodes/sessionnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/geomapi/tools/__init__.py` & `geomapi-0.3.2/geomapi/tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     Args:
         1.xmlPath (string): xml file path e.g. "D:/Data/cameras.xml"
         2.skip (int, Optional): select every nth image from the xml. Defaults to None.
         3.filterByFolder (bool, Optional): Filter imgNodes based on the images in the folder or not. Defaults to False.
             
     Returns:
-        A list of pointcloudnodes with the xml metadata 
+        A list of ImageNodes with the xml metadata 
     """
     assert skip == None or skip >0, f'skip == None or skip '
     assert os.path.exists(xmlPath), f'File does not exist.'
     assert xmlPath.endswith('.xml'), f'File does not end with xml.' 
     
     #open xml
     mytree = ET.parse(xmlPath)
@@ -710,29 +710,28 @@
             return nodelist
     else:
         raise ValueError('No valid ifcPath.') 
 
 
 ##### NODE SELECTION #####
 
-def select_k_nearest_nodes(node:Node,nodelist:List[Node],k:int=10) -> Tuple[List [Node], o3d.utility.DoubleVector]:
+def select_nodes_k_nearest_neighbors(node:Node,nodelist:List[Node],k:int=10) -> Tuple[List [Node], o3d.utility.DoubleVector]:
     """ Select k nearest nodes based on Euclidean distance between centroids.\n
 
     .. image:: ../docs/pics/selection_k_nearest.PNG
 
     Args:
         0. node (Node): node to search from\n
         1. nodelist (List[Node])\n
         2. k (int, optional): number of neighbors. Defaults to 10.\n
 
     Returns:
         List of Nodes
     """
-    if k <=0:
-        raise ValueError('k must be positive and non-negative.')
+    assert k>0, f'k is {k}, but k should be >0.'
 
     #get node center
     if node.get_cartesian_transform() is not None:
         point=gmu.get_translation(node.cartesianTransform)
         #create pcd from nodelist centers
         pcd = o3d.geometry.PointCloud()
         array=np.empty(shape=(len(nodelist),3))
@@ -751,30 +750,72 @@
         selectedNodeList=[node for idx,node in enumerate(nodelist) if idx in idxList]
 
         if any(selectedNodeList):        
             return selectedNodeList, distances
     else:
         return None,None
 
+
+def create_selection_box_from_image_boundary_points(n:ImageNode,roi:Tuple[int,int,int,int],mesh:o3d.geometry.TriangleMesh,z:float=5)->o3d.geometry.OrientedBoundingBox:
+    """Create a selection box from an ImageNode, a region of interest (roi) and a mesh to raycast.
+    A o3d.geometry.OrientedBoundingBox will be created on the location of the intersection of the rays with the mesh.
+    The height of the box is determined by the offset of z in both positive and negative Z-direction
+
+    Args:
+        n (ImageNode): Imagenode used for the raycasting (internal and external camera paramters)
+        roi (Tuple[int,int,int,int]): region of interest (rowMin,rowMax,columnMin,columnMax)
+        mesh (o3d.geometry.TriangleMesh): mesh used for the raycasting
+        z (float, optional): offset in height of the bounding box. Defaults to [-5m:5m].
+
+    Returns:
+        o3d.geometry.OrientedBoundingBox or None (if not all rays hit the mesh)
+    """
+    box=None
+    
+    #create rays for boundaries
+    uvCoordinates=np.array([[roi[0],roi[2]], # top left
+                            [roi[0],roi[3]], # top right
+                            [roi[1],roi[2]], # bottom left
+                            [roi[1],roi[3]] # bottom right
+                            ])
+    # transform uvcoordinates  to world coordinates to rays   
+    rays=n.create_rays(uvCoordinates)
+    
+    # cast rays to 3D mesh 
+    distances,_=gmu.compute_raycasting_collisions(mesh,rays)
+    
+    if all(np.isnan(distances)==False): #if all rays hit
+        #compute endpoints 
+        _,endpoints=gmu.rays_to_points(rays,distances)
+        
+        #create box of projected points
+        points=np.vstack((gmu.transform_points(endpoints,transform=np.array([[1,0,0,0],[0,1,0,0],[0,0,1,z],[0,0,0,1]])),
+                        gmu.transform_points(endpoints,transform=np.array([[1,0,0,0],[0,1,0,0],[0,0,1,-z],[0,0,0,1]]))))
+        box=o3d.geometry.OrientedBoundingBox.create_from_points(o3d.cpu.pybind.utility.Vector3dVector(points))
+        box.color=[1,0,0]     
+    return box 
+
+
+
 def select_nodes_with_centers_in_radius(node:Node,nodelist:List[Node],r:float=0.5) -> Tuple[List [Node] ,List[float]]:
     """Select nodes within radius of the node centroid based on Euclidean distance between node centroids.\n
 
     .. image:: ../docs/pics/selection_radius_nearest.PNG
     
     Args:
         0. node (Node): node to search from\n
         1. nodelist (List[Node])\n
         2. r (float, optional): radius to search. Defaults to 0.5m.\n
 
     Returns:
         List of Nodes, List of Distances
     """
     
-    if r <=0:
-        raise ValueError('r must be positive and non-negative.')
+    assert r >0, f'r is {r}, while it should be >0.'
+    
     #get node center
     if node.get_cartesian_transform() is not None:
         point=gmu.get_translation(node.cartesianTransform)
         #create pcd from nodelist centers
         pcd = o3d.geometry.PointCloud()
         array=np.empty(shape=(len(nodelist),3))
         for idx,node in enumerate(nodelist):
```

### Comparing `geomapi-0.3.1/geomapi/tools/alignmenttools/__init__.py` & `geomapi-0.3.2/geomapi/tools/alignmenttools/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/geomapi/tools/alignmenttools/match.py` & `geomapi-0.3.2/geomapi/tools/alignmenttools/match.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/geomapi/tools/alignmenttools/params.py` & `geomapi-0.3.2/geomapi/tools/alignmenttools/params.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/geomapi/tools/completiontools/__init__.py` & `geomapi-0.3.2/geomapi/tools/completiontools/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/geomapi/tools/machinelearningtools/__init__.py` & `geomapi-0.3.2/geomapi/tools/machinelearningtools/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/geomapi/tools/progresstools/__init__.py` & `geomapi-0.3.2/geomapi/tools/progresstools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
 def subdivide_pcd_per_octree(pcd,maxDepth:int=4,lowEnd=0,highEnd=2000000)-> Tuple[List[int],List[int]]:
     """Create an octree of various point clouds and subdivide it according to a voxel octree. For each depth level, the data is divided 8-fold.
     This function returns the indices per voxel if that node has a number of points between lowEnd and highEnd.
 
     Args:
         pcd (las,dataframe or open3d): Point Cloud (only points are used)
-        maxDepth (int, optional): depth of the octree. Defaults to 4.
+        maxDepth (int, optional): depth of the octree. Defaults to 4 (this is also the maxDepth).
         lowEnd (int, optional): minimum number of points in a node for it to be added to the export. Defaults to 0.
         highEnd (int, optional): maximum number of points in a node for it to be added to the export. If this is surpassed, its children will be assessed. Defaults to 2000000.
 
     Returns:
         Tuple[List[int],List[int]]: pathLists with names formatted as 'pcd_{a}_{b}_{c}_{d}' that correspond to the depth ,idxLists with indices per valid node
     """
     #validate inputs
```

### Comparing `geomapi-0.3.1/geomapi/tools/validationtools/__init__.py` & `geomapi-0.3.2/geomapi/tools/validationtools/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -535,32 +535,14 @@
                 if LOA[2] == 'LOA10':
                     BIMNode.resource.paint_uniform_color([1,0.76,0])
                 if LOA[2] == 'LOA20':
                     BIMNode.resource.paint_uniform_color([1,1,0])
                 if LOA[2] == 'LOA30':
                     BIMNode.resource.paint_uniform_color([0,1,0])
 
-def divide_line_in_sections(linesets,resolution:float=0.1)->np.ndarray:
-
-    #convert to list
-    linesets=ut.item_to_list(linesets)
-
-    for lineset in linesets:
-        #sample every line
-        for line in lineset.lines:
-            start=lineset.points(line.points[0])
-            end=lineset.points(line.points[1])
-            vector=end-start #create line function using start end
-            length=0
-            #compute points on the vector at fixed intervals given the resolution on 
-    
-    return points
-
-
-
 
 def cad_show_lines(dxf_path:str):
 
     doc = ezdxf.readfile(dxf_path)
 
     # Extract all line entities from the DXF file
     msp = doc.modelspace()
@@ -570,173 +552,227 @@
     for line in lines:
         x1, y1, _ = line.dxf.start
         x2, y2, _ = line.dxf.end
         plt.plot([x1, x2], [y1, y2])
 
     plt.show()
 
-def dxf_extract_ezdxf_lines(dxf_path:str) -> List[Tuple[ezdxf.math.vector.Vector,ezdxf.math.vector.Vector,int,str,float]]:
-    """Import a DXF and extract all line assets.  
-
-    Args:
-        dxf_path (str): path to dxf
-
-    Returns:
-        List[Tuple[ezdxf.math.vector.Vector,ezdxf.math.vector.Vector,int,str,float]]: (start, end, color, layer, thickness)
-
-    """
-    #open dxf file
-    dwg = ezdxf.readfile(dxf_path)
-    modelspace = dwg.modelspace()
-    
-    #parse lines
-    lines = []
-    for entity in modelspace:
-        if entity.dxftype() == 'LINE': #! make bigger linesets
-            start = entity.dxf.start
-            end = entity.dxf.end
-            color = entity.dxf.color
-            layer = entity.dxf.layer
-            thickness = entity.dxf.lineweight
-            lines.append((start, end, color, layer, thickness))
-    
-    return lines
-
-def create_lineset(line, points:np.ndarray):
-    pcd = o3d.geometry.PointCloud()
-    pcd.points = o3d.utility.Vector3dVector(np.array(points))
-    colors = [line[2]] * len(points) #! this is sketchy
-    pcd.colors = o3d.utility.Vector3dVector(np.array(colors) / 255.0)
-    
-    lineset = o3d.geometry.LineSet.create_from_point_cloud_correspondences(pcd, pcd, [(i, i+1) for i in range(len(points)-1)])
-    lineset.paint_uniform_color(np.array(line[2]) / 255.0)
-    lineset.line_width = line[4]
+# def create_lineset(line, points:np.ndarray):
+#     pcd = o3d.geometry.PointCloud()
+#     pcd.points = o3d.utility.Vector3dVector(np.array(points))
+#     colors = [line[2]] * len(points) #! this is sketchy
+#     pcd.colors = o3d.utility.Vector3dVector(np.array(colors) / 255.0)
+    
+#     lineset = o3d.geometry.LineSet.create_from_point_cloud_correspondences(pcd, pcd, [(i, i+1) for i in range(len(points)-1)])
+#     lineset.paint_uniform_color(np.array(line[2]) / 255.0)
+#     lineset.line_width = line[4]
     
-    return lineset
+#     return lineset
 
-def sample_pcd_from_linesets(linesets:List[o3d.geometry.LineSet],step_size:float=0.1)-> List[o3d.geometry.PointCloud]:
+def sample_pcd_from_linesets(linesets:List[o3d.geometry.LineSet],step_size:float=0.1)-> Tuple[o3d.geometry.PointCloud,np.ndarray]:
     """Sample a point cloud from a set of o3d.geometry.LineSet elements (color is inherited)
 
     Args:
         linesets (List[o3d.geometry.LineSet]): linesets to sample. 
         step_size(float,optional):spacing between points. Defaults to 0.1m.
 
     Returns:
-        List[o3d.geometry.PointCloud]: point_clouds
+        Tuple[List[o3d.geometry.PointCloud],np.ndarray]: point_clouds, identityarray with integers of the origin of the points
     """
-    point_clouds=[]
-    for lineset in linesets:
+    point_clouds=o3d.geometry.PointCloud()
+    ilist=[]
+    jlist=[]
+    
+    for i,lineset in enumerate(linesets):
 
         # Get line segments from the LineSet
         pointArray=np.asarray(lineset.points)
         points = []
 
-        for line in np.asarray(lineset.lines):
+        for j,line in enumerate(np.asarray(lineset.lines)):
             #get start and end
             start_point = pointArray[line[0]]
             end_point = pointArray[line[1]]
             #get direction and length
             direction = end_point - start_point
             length = np.linalg.norm(direction)
             #compute number of points
             num_points = int(length / step_size)
             if num_points > 0:
                 step = direction / num_points
-                points.extend([start_point + i * step for i in range(num_points + 1)])
-
+                p=[start_point + r * step for r in range(num_points + 1)]
+                points.extend(p)
+                
+                #keep track of identity of the points
+                ilist.extend(np.full((len(p), 1), i))
+                jlist.extend(np.full((len(p), 1), j))
+                
         # Convert the sampled points to an o3d PointCloud
         point_cloud = o3d.geometry.PointCloud()
         point_cloud.points = o3d.utility.Vector3dVector(points)
         color=lineset.colors[0]
         point_cloud.paint_uniform_color(color)
-        point_clouds.append(point_cloud)
+        point_clouds+=point_cloud
         
-    return point_clouds
+    #compile identidyarray & point cloud
+    indentityArray=np.column_stack((np.array(ilist),np.array(jlist)))
 
-def create_unique_mapping(array:np.ndarray)->Tuple[np.ndarray,np.ndarray]:
-    """Create a unique mapping of an array
+    return point_clouds,indentityArray
 
-    Args:
-        array (np.ndarray): first column of the array will be used for the sorting.
+# def select_lineset_inliers(linesets,points)->o3d.geometry.LineSet:
+#     linesetselection=np.empty((points.shape[0],2))
 
-    Returns:
-        Tuple[np.ndarray,np.ndarray]: unique_values, mapping (shape of input array)
-    """
-    #get first array #! this is a bit flawed and supposes that every x-value is unique
-    a=array[:,0]
-    unique_values=np.unique(array,axis=0)
-    
-    # build dictionary
-    fwd = np.argsort(a)
-    asorted = a[fwd]
-    keys = np.unique(asorted) 
-    lower = np.searchsorted(asorted, keys)
-    higher = np.append(lower[1:], len(asorted))
-
-    inv = {key: fwd[lower_i:higher_i]
-            for key, lower_i, higher_i
-            in zip(keys, lower, higher)}
-    
-    # remap values to 0,1,2,....
-    mapping=np.zeros(array.shape[0])
-    i=0
-    for _,value in inv.items():
-            for v in value:
-                    mapping[v]=i
-            i+=1
-    
-    return unique_values,mapping
+#     #iterate through linesets
+#     for i,p in enumerate(points):
+        
+#         for linesetidx,lineset in enumerate(sublinesets):
+            
+#             #iterate through line
+#             for lineidx,line in enumerate(lineset.lines):
+#                 # # get p0 and p1 in the size of the input points
+#                 # p0=np.tile(lineset.points[line[0]], (points.shape[0], 1)) 
+#                 # p1=np.tile(lineset.points[line[1]], (points.shape[0], 1))
+#                 p0=lineset.points[line[0]]
+#                 p1=lineset.points[line[1]]
+                
+#                 #test if any point is on the line  -> # 0.0 <= dot(p1-p0,p-p0)/|p-p0| <= 1.0
+#                 # print(np.sum((p-p0)**2))
+#                 dot=np.dot(p1-p0,p-p0)/np.sum((p-p0)**2)
+                
+#                 if (dot>=0) & (dot <=1 ):
+#                     linesetselection[i,0]=linesetidx
+#                     linesetselection[i,1]=lineidx
+#     return(linesetselection)               
+#             # print('line')
+#             # dot=np.sum(np.dot(p1-p0,(points-p0).T),axis=1) /np.sum((points-p0)**2,axis=1)
+        
+# #         # create tuple 
+# #         np.where((dot>=0) & (dot <=1 ),
+# #                  (linesetidx,lineidx,dot),
+# #                  (np.nan,np.nan,dot))
+            
+        
+# # return linesetselection.append((linesetidx,lineidx,distance))
+        
+# # return True if (dot>=0 or dot <=1 ) else False
+
+
+# def create_unique_mapping(array:np.ndarray)->Tuple[np.ndarray,np.ndarray]:
+#     """Create a unique mapping of an array
+
+#     Args:
+#         array (np.ndarray): first column of the array will be used for the sorting.
 
-def ezdxf_lines_to_open3d_linesets(ezdxf_lines:List[Tuple[ezdxf.math.vector.Vector,ezdxf.math.vector.Vector,int,str,float]]) -> List[o3d.geometry.LineSet]: #
-    """Convert ezdxf lines to open3D linesets. Create 1 lineset per layer.
+#     Returns:
+#         Tuple[np.ndarray,np.ndarray]: unique_values, mapping (shape of input array)
+#     """
+#     #get first array #! this is a bit flawed and supposes that every x-value is unique
+#     a=array[:,0]
+#     unique_values=np.unique(array,axis=0)
+    
+#     # build dictionary
+#     fwd = np.argsort(a)
+#     asorted = a[fwd]
+#     keys = np.unique(asorted) 
+#     lower = np.searchsorted(asorted, keys)
+#     higher = np.append(lower[1:], len(asorted))
+
+#     inv = {key: fwd[lower_i:higher_i]
+#             for key, lower_i, higher_i
+#             in zip(keys, lower, higher)}
+    
+#     # remap values to 0,1,2,....
+#     mapping=np.zeros(array.shape[0])
+#     i=0
+#     for _,value in inv.items():
+#             for v in value:
+#                     mapping[v]=i
+#             i+=1
+    
+#     return unique_values,mapping
+
+def get_linesets_inliers_in_box(linesets:List[o3d.geometry.LineSet],box:o3d.geometry.OrientedBoundingBox,point_cloud:o3d.geometry.PointCloud,identityArray:np.ndarray) -> List[o3d.geometry.LineSet]:
+    """Returns the segments of the linesets that have sampled pointcloud points falling within a certain bounding box.
+    This function should be used together with:\\
+        1. vt.sample_pcd_from_linesets(linesets,step_size=0.1)\\
+        2.vt.create_selection_box_from_image_boundary_points(n,roi,meshNode.resource,z=5) \\
 
     Args:
-        ezdxf_lines (List[Tuple[ezdxf.math.vector.Vector,ezdxf.math.vector.Vector,int,str,float]]): (start, end, color, layer, thickness)
+        linesets (List[o3d.geometry.LineSet]): linesets from which the segments will be selected
+        box (o3d.geometry.OrientedBoundingBox): bounding box that is used to filter the point cloud points
+        point_cloud (o3d.geometry.PointCloud): sampled points on the linesets
+        identityArray (np.ndarray): array with integers that reflect which point cloud point belongs to which lineset
 
     Returns:
-        List[o3d.geometry.LineSet]
-    """  
-    # get layers (str)
-    layers=list(set([line[3] for line in ezdxf_lines]))
-
-    #Convert linesets
-    linesets = []  
-    for layer in layers:
-
-        # get lines in layer
-        lines=[line for line in ezdxf_lines if line[3]==layer]
-        
-        # get start and endpoints       
-        array=np.empty((len(lines)*2,3))
-        for i,line in enumerate(lines): 
-            array[2*i,:]= np.array(line[0])
-            array[2*i+1,:]= np.array(line[1])
+        List[o3d.geometry.LineSet]: _description_
+    """
+    assert len(np.asarray(point_cloud.points))==identityArray.shape[0], f'length of point cloud and identityarray are not equal'
         
-        #get mapping    
-        unique_values,mapping = create_unique_mapping(array)
-
-        #get points and lines and create lineset
+    #compute point_cloud inliers in box
+    idxList=box.get_point_indices_within_bounding_box(point_cloud.points)
+    if len(idxList)==0:
+        return []    
+        
+    #retrieve which linesets are visible in the box
+    idx=identityArray[idxList]
+    unique_rows, _ = np.unique(idx, axis=0, return_inverse=True)
+    
+    #split lists per lineset -> create split_rows dictionary of mapping
+    split_rows = {}
+    for row in unique_rows:
+        key = row[0]
+        if key not in split_rows:
+            split_rows[key] = []
+        split_rows[key].append(row)
+    
+    #get linesegments and build new linesets
+    sublinesets=[]
+    for key,value in split_rows.items():
+        #get lineset
+        lineset=linesets[key]
+        #get linesegments
+        linesegments=[linesets[key].lines[v[1]] for v in value]
+        #create new linesets -> currently still has all redundant points
         line_set = o3d.geometry.LineSet() 
-        lineArray=np.reshape(mapping,(len(lines),2))
-        line_set.points = o3d.utility.Vector3dVector(unique_values)  
-        line_set.lines = o3d.utility.Vector2iVector(lineArray)
-        
-        #colorize per color 
-        color=next(line[2] for line in ezdxf_lines if line[3]==layer)/256
-        line_set.paint_uniform_color(np.repeat(color,3))
-        linesets.append(line_set)
-
-    return linesets
-
-def compute_distance_between_open3d_lines(lines:List[o3d.geometry.LineSet],resolution:float=0.1) -> List[float]:
-    """Compute distance between lines at periodic intervals
+        line_set.points = o3d.utility.Vector3dVector(lineset.points)  
+        line_set.lines = o3d.utility.Vector2iVector(linesegments)
+        sublinesets.append(line_set)
+    return sublinesets
+
+def create_selection_box_from_image_boundary_points(n:ImageNode,roi:Tuple[int,int,int,int],mesh:o3d.geometry.TriangleMesh,z:float=5)->o3d.geometry.OrientedBoundingBox:
+    """Create a selection box from an ImageNode, a region of interest (roi) and a mesh to raycast.
+    A o3d.geometry.OrientedBoundingBox will be created on the location of the intersection of the rays with the mesh.
+    The height of the box is determined by the offset of z in both positive and negative Z-direction
 
     Args:
-        lines (List[o3d.geometry.LineSet]): _description_
-        resolution (float, optional): _description_. Defaults to 0.1.
+        n (ImageNode): Imagenode used for the raycasting (internal and external camera paramters)
+        roi (Tuple[int,int,int,int]): region of interest (rowMin,rowMax,columnMin,columnMax)
+        mesh (o3d.geometry.TriangleMesh): mesh used for the raycasting
+        z (float, optional): offset in height of the bounding box. Defaults to [-5m:5m].
 
     Returns:
-        List[float]: _description_
+        o3d.geometry.OrientedBoundingBox or None (if not all rays hit the mesh)
     """
-    distances=[0]
-    return distances
-
+    box=None
+    
+    #create rays for boundaries
+    uvCoordinates=np.array([[roi[0],roi[2]], # top left
+                            [roi[0],roi[3]], # top right
+                            [roi[1],roi[2]], # bottom left
+                            [roi[1],roi[3]] # bottom right
+                            ])
+    # transform uvcoordinates  to world coordinates to rays   
+    rays=n.create_rays(uvCoordinates)
+    
+    # cast rays to 3D mesh 
+    distances,_=gmu.compute_raycasting_collisions(mesh,rays)
+    
+    if all(np.isnan(distances)==False): #if all rays hit
+        #compute endpoints 
+        _,endpoints=gmu.rays_to_points(rays,distances)
+        
+        #create box of projected points
+        points=np.vstack((gmu.transform_points(endpoints,transform=np.array([[1,0,0,0],[0,1,0,0],[0,0,1,z],[0,0,0,1]])),
+                        gmu.transform_points(endpoints,transform=np.array([[1,0,0,0],[0,1,0,0],[0,0,1,-z],[0,0,0,1]]))))
+        box=o3d.geometry.OrientedBoundingBox.create_from_points(o3d.cpu.pybind.utility.Vector3dVector(points))
+        box.color=[1,0,0]     
+    return box
```

### Comparing `geomapi-0.3.1/geomapi/utils/__init__.py` & `geomapi-0.3.2/geomapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/geomapi/utils/geometryutils.py` & `geomapi-0.3.2/geomapi/utils/geometryutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,23 @@
 import copy
 import math
 import os
 from typing import List, Tuple
 # from xmlrpc.client import bool
 import pandas as pd
 import sys
+import itertools
 
 from sklearn.neighbors import NearestNeighbors # to compute nearest neighbors
 import laspy # this is to process las point clouds
 import cv2
 import geomapi.utils as ut
+
+import geomapi.utils.imageutils as iu #! this might be a problem
+
 import ifcopenshell
 import ifcopenshell.geom as geom
 import ifcopenshell.util
 # import matplotlib
 import numpy as np
 import open3d as o3d
 import pye57
@@ -155,17 +159,72 @@
                 combined = trimesh.util.concatenate( [ meshes ] )
                 combined.merge_vertices(merge_tex =True,merge_norm =True )
                 combined.remove_duplicate_faces()
                 submesh=combined
                 submeshes.append(submesh)
     return submeshes
 
+def sample_geometry(geometries:List[o3d.geometry.Geometry],resolution:float=0.1)->List[o3d.geometry.PointCloud]:
+    """Sample the surface, line or point cloud of an open3d object given a resolution.
+
+    Args:
+        geometries (List[o3d.geometry.Geometry]): o3d.Geometry.LineSet,o3d.Geometry.TriangleMesh or o3d.Geometry.PointCloud
+        resolution (float, optional): spacing between sampled points. Defaults to 0.1m.
+
+    Returns:
+        List[o3d.geometry.PointCloud]
+    """
+    geometries=ut.item_to_list(geometries)
+        
+    point_clouds=[]
+    for g in geometries:
+        pcd=o3d.geometry.PointCloud()
+        
+        if 'TriangleMesh' in str(type(g)) and len(g.vertices) != 0:
+            area=g.get_surface_area()
+            count=int(area/(resolution*resolution))
+            pcd=g.sample_points_uniformly(number_of_points=count)
+            
+        elif 'PointCloud' in str(type(g)) and len(g.points) != 0: 
+            pcd=g.voxel_down_sample(resolution)
+            
+        elif 'ndarray' in str(type(g)):
+            pcd.points=o3d.utility.Vector3dVector(g)
+            pcd=pcd.voxel_down_sample(resolution)
+            
+        elif 'LineSet' in str(type(g)):    
+            # Get line segments from the LineSet
+            pointArray=np.asarray(g.points)
+            points = []
+
+            for line in np.asarray(g.lines): #! this is not efficient
+                #get start and end
+                start_point = pointArray[line[0]]
+                end_point = pointArray[line[1]]
+                #get direction and length
+                direction = end_point - start_point
+                length = np.linalg.norm(direction)
+                #compute number of points
+                num_points = int(length / resolution)
+                if num_points > 0:
+                    step = direction / num_points
+                    p=[start_point + r * step for r in range(num_points + 1)]
+                    points.extend(p)
+            pcd.points=o3d.utility.Vector3dVector(points)  
+                  
+        point_clouds.append(pcd)
+        
+    return point_clouds
+
+
 def mesh_sample_points_uniformly(meshes:List[o3d.geometry.TriangleMesh],resolution:float=0.1)->List[o3d.geometry.PointCloud]:
     """Sample the surface of a open3d mesh with a fixed resolution.\n
 
+    **NOTE** DEPRECIATED, use sample_geometry instead
+    
     Args:
         1.meshes (List[o3d.geometry.TriangleMesh])\n
         2.resolution (float, optional): spatial resolution of the generated point cloud. Defaults to 0.1m.\n
 
     Returns:
         o3d.geometry.PointCloud
     """
@@ -286,14 +345,88 @@
     Returns:
         Tuple(o3d.geometry.PointCloud,o3d.geometry.PointCloud): The points close enough and the points too far away.
     """
     dists = sourcePcd.compute_point_cloud_distance(testPcd)
     ind = np.where(np.asarray(dists) < maxDistance)[0]
     return (sourcePcd.select_by_index(ind), sourcePcd.select_by_index(ind, True))
 
+def filter_geometry_by_distance(geometries: List[o3d.geometry.Geometry], querry_point:np.ndarray, distance_threshold : float =500) -> List[o3d.geometry.Geometry]:
+    """Filter out the parts of geometries that lie to far from a querry point.
+
+    Args:
+        geometries (List[o3d.geometry.Geometry]): list of geometries (point clouds, trianglemesh or lineset)
+        querry_point (np.ndarray[1x3]): center point of the search
+        distance_threshold (float, optional): search distance. Defaults to 500m.
+
+    Returns:
+        List[o3d.geometry.Geometry]
+    """
+    geometry_groups=copy.deepcopy(geometries)
+    geometryArray=[]
+
+    for i,g in enumerate(list(itertools.chain(*geometry_groups))):
+    
+        if type(g)==o3d.geometry.LineSet:
+            #get indices outside range
+            points=np.asarray(g.points)            
+            dist = np.linalg.norm(points-querry_point,axis=1)         
+            indices=(dist>distance_threshold).nonzero()[0]
+            
+            if indices.size >0 and indices.size < points.shape[0]:            
+                # Remove points
+                g.points = o3d.utility.Vector3dVector(np.delete(points, indices, axis=0))  
+                # get linesindices to remove          
+                lineindices = np.where(np.any(np.isin(np.asarray(g.lines), indices), axis=1))[0]
+                if  lineindices.size==0:
+                    #add in its totality
+                    geometryArray.append(g)   
+                else:
+                    # Remove lines
+                    g.lines = o3d.utility.Vector2iVector(np.delete(np.asarray(g.lines), lineindices, axis=0))
+                    geometryArray.append(g)
+        
+        elif type(g)==o3d.geometry.PointCloud:
+            #get indices outside range
+            kd= o3d.geometry.KDTreeFlann(g)
+            _, idx, _=kd.search_radius_vector_3d(querry_point,distance_threshold)
+            indices=np.asarray(idx)
+            
+            if  indices.size == 0:
+                #ignore this geometry
+                continue
+            elif  indices.size == np.asarray(g.points).shape[0]:
+                #add in its totality
+                geometryArray.append(g)
+            else:
+                #select some points
+                g=g.select_by_index(indices)       
+                geometryArray.append(g)
+            
+        elif type(g)==o3d.geometry.TriangleMesh:
+            #get indices outside range
+            points=np.asarray(g.vertices)            
+            dist = np.linalg.norm(points-querry_point,axis=1) 
+            indices=(dist>distance_threshold).nonzero()[0]
+            
+            if indices.size >0 and indices.size < points.shape[0]:
+                # Remove points
+                # g.vertices = o3d.utility.Vector3dVector(np.delete(points, indices, axis=0))
+                # Remove triangles
+                triangleindices = np.where(np.any(np.isin(np.asarray(g.triangles), indices), axis=1))[0]
+                if  triangleindices.size==0:
+                    #add in its totality
+                    geometryArray.append(g)
+                else:
+                    #remove some triangles
+                    g.remove_triangles_by_index(triangleindices) 
+                    g.remove_unreferenced_vertices()    
+                    geometryArray.append(g)           
+
+    return geometryArray
+
 def get_indices_in_hull(points : np.ndarray, hull :np.ndarray) -> List[int]:
     """Get the indices of all the points that are inside the hull.\n
 
     Args:
         1. points (numpy.array): should be a `NxK` coordinates of `N` points in `K` dimensions.\n
         2. hull (np.array): is either a scipy.spatial.Delaunay object or the `MxK` array of the 
         coordinates of `M` points in `K`dimensions for which Delaunay triangulation will be computed
@@ -907,15 +1040,15 @@
     if rgb:
         rgb=dataframe.iloc[:,rgb].to_numpy()
         las.red=rgb[:, 0]
         las.green=rgb[:, 1]
         las.blue=rgb[:, 2]
         
     # 4. Create extra dims for scalar fields
-    names=arr.columns[3:] if rgb is None else arr.columns[[t for t in np.arange(3,len(arr.columns)) if t not in rgb]] 
+    names=dataframe.columns[3:] if rgb is None else dataframe.columns[[t for t in np.arange(3,len(dataframe.columns)) if t not in rgb]] #! there might be a problem here
     dtypes=dtypes if dtypes else ['float32' for n in names]
     extraBytesParams=[laspy.ExtraBytesParams(name=name, type=dtype) for name,dtype in zip(names,dtypes)]
     las.add_extra_dims(extraBytesParams)   
     [setattr(las,name,dataframe[name].to_numpy()) for i,name in enumerate(names)]
     
     return las
 
@@ -1993,41 +2126,103 @@
         # assert ((abs(u)<= box.get_extent()[0]) and (abs(v)<=box.get_extent()[1]) and (abs(w)<=box.get_extent()[2])), f'cannot schrink more than the extent of the box.'
         minBound=box.get_min_bound()
         maxBound=box.get_max_bound()
         new_minBound=minBound-np.array([u,v,w])/2
         new_maxBound=maxBound+np.array([u,v,w])/2        
         return o3d.geometry.AxisAlignedBoundingBox(new_minBound,new_maxBound) 
 
-def join_geometries(geometries)->o3d.geometry:
-    """Join a number of o3d.PointCloud or o3d.TriangleMesh instances.\n
+# def join_geometries(geometries)->o3d.geometry:
+#     """Join a number of o3d.PointCloud or o3d.TriangleMesh instances.\n
+
+#     **NOTE**: Only members of the same geometryType can be merged.\n
+
+#     Args:
+#         geometries (o3d.PointCloud or TriangleMesh)
+
+#     Returns:
+#         merged o3d.geometry (o3d.PointCloud or TriangleMesh)
+#     """
+#     geometries=ut.item_to_list(geometries)
+#     if any('TriangleMesh' in str(type(g)) for g in geometries ):
+#         joined=o3d.geometry.TriangleMesh()
+#         for geometry in geometries:
+#             if geometry is not None and len(geometry.vertices) != 0:
+#                 joined +=geometry
+#         return joined
+#     if any('PointCloud' in str(type(g)) for g in geometries ):
+#         joined=o3d.geometry.PointCloud()
+#         for geometry in geometries:
+#             if geometry is not None and len(geometry.points) != 0:
+#                 joined +=geometry
+#         return joined
+#     else:
+#         raise ValueError('Only submit o3d.geometry.TriangleMesh or o3d.geometry.PointCloud objects') 
+
+def split_pcd_by_labels(point_cloud:o3d.geometry.PointCloud,labels:np.ndarray)-> Tuple[List[o3d.geometry.PointCloud],np.ndarray]:
+    """Split a point cloud in parts to match a list of labels. The result is a set of point clouds, one for each unique label.
+
+    Args:
+        point_cloud (o3d.geometry.PointCloud):
+        labels (np.ndarray): integer array with the same length as the point clouds 
+
+    Returns:
+        Tuple[List[o3d.geometry.PointCloud],np.ndarray]: point clouds, unique labels
+    """
+    pcdList=[]
+    unique=np.unique(labels)
+    for i in unique:    
+        ind = np.where(labels==i)[0]
+        pcdList.append(point_cloud.select_by_index(ind))
+    return pcdList,unique
+
+def join_geometries(geometries:List[o3d.geometry.Geometry])->List[o3d.geometry.Geometry]:
+    """Join together a number of o3d geometries e.g. LineSet, PointCloud or o3d.TriangleMesh instances.\n
 
     **NOTE**: Only members of the same geometryType can be merged.\n
+    
+    **NOTE**: np.arrays can also be processed (these are added to the point cloud)
 
     Args:
-        geometries (o3d.PointCloud or TriangleMesh)
+        geometries (List[o3d.geometry.Geometry]): LineSet, PointCloud or o3d.TriangleMesh or np.array[nx3]
 
     Returns:
-        merged o3d.geometry (o3d.PointCloud or TriangleMesh)
+        merged o3d.geometries
     """
     geometries=ut.item_to_list(geometries)
-    if any('TriangleMesh' in str(type(g)) for g in geometries ):
-        joined=o3d.geometry.TriangleMesh()
-        for geometry in geometries:
-            if geometry is not None and len(geometry.vertices) != 0:
-                joined +=geometry
-        return joined
-    if any('PointCloud' in str(type(g)) for g in geometries ):
-        joined=o3d.geometry.PointCloud()
-        for geometry in geometries:
-            if geometry is not None and len(geometry.points) != 0:
-                joined +=geometry
-        return joined
-    else:
-        raise ValueError('Only submit o3d.geometry.TriangleMesh or o3d.geometry.PointCloud objects') 
-
+    
+    #group per geometrytype
+    line_set=o3d.geometry.LineSet()
+    point_cloud=o3d.geometry.PointCloud()
+    mesh=o3d.geometry.TriangleMesh()
+    points=[]
+    for g in geometries:
+        if 'TriangleMesh' in str(type(g)) and len(g.vertices) != 0:
+            mesh+=g
+        elif 'PointCloud' in str(type(g)) and len(g.points) != 0: 
+            point_cloud+=g
+        elif 'ndarray' in str(type(g)):
+            [points.append(p) for p in g]
+        elif 'LineSet' in str(type(g)):    
+            line_set+=g
+    
+    #add points to point_cloud
+    points=np.array(points)
+    if points.shape[0]>0:
+        pcd=o3d.geometry.PointCloud()
+        pcd.points=o3d.utility.Vector3dVector(points)
+        point_cloud+=pcd
+    
+    #return geometries
+    geometries=[]
+    geometries.append(line_set) if np.asarray(line_set.points).shape[0]>0 else None
+    geometries.append(point_cloud) if np.asarray(point_cloud.points).shape[0]>0 else None
+    geometries.append(mesh) if np.asarray(mesh.vertices).shape[0]>0 else None
+    
+    return geometries if len(geometries)!=1 else geometries[0]
+        
 def crop_dataframe_from_meshes(df: pd.DataFrame,meshes:List[o3d.geometry.TriangleMesh]) -> List[pd.DataFrame]:
     """Crop point cloud and divide the inliers per waterthight mesh. \n
 
     Args:
         1. dataFrame (pd.DataFrame): Pandas dataframe with first three columns as [X,Y,Z].\n
         2. meshes (o3d.geometry.TriangleMesh): meshes to test the inliers.\n
 
@@ -2154,27 +2349,48 @@
             indentityArray=np.vstack((indentityArray,np.full((len(pcd.points), 1), i)))
             pcd.paint_uniform_color(colorArray[i])
             identityPointCloud +=pcd
             # np.concatenate((np.asarray(identityPointCloud.points),np.asarray(identityPointCloud.points)),axis=0)
         elif 'TriangleMesh' in str(type(geometry)):
             area=geometry.get_surface_area()
             count=int(area/(resolution*resolution))
-            pcd=geometry.sample_points_uniformly(number_of_points=count, use_triangle_normal=getNormals)
-            # pcd=pcd.voxel_down_sample(resolution) #! why 10*count and downsample?
+            if count>0:
+                count=count if count>0 else len(np.asarray(geometry.vertices))
+                pcd=geometry.sample_points_uniformly(number_of_points=count, use_triangle_normal=getNormals)
+            else:
+                pcd=o3d.geometry.PointCloud()
+                pcd.points=o3d.utility.Vector3dVector(np.array([geometry.get_center()]))
+                
             indentityArray=np.vstack((indentityArray,np.full((len(pcd.points), 1), i)))
             pcd.paint_uniform_color(colorArray[i])
             identityPointCloud +=pcd
         else:
             print(f'{geometry} is invalid')
             continue
-            # raise ValueError('Geometries must be o3d.geometry (PointCloud or TriangleMesh)')    
     indentityArray=indentityArray.flatten()
     indentityArray=np.delete(indentityArray,0)
     return identityPointCloud, indentityArray
 
+def split_quad_faces(faces:np.ndarray) ->np.ndarray:
+    """Split an array of quad faces e.g. [[0,1,2,3]] into triangle faces e.g. [[0,1,2],[0,2,3]]
+
+    Args:
+        faces (np.ndarray[nx4]) 
+
+    Returns:
+        np.ndarray[2nx3]
+    """
+    newFaces=np.zeros((1,3),dtype=np.uint16)
+    for f in faces:
+        f=np.array(f)       
+        newFaces=np.vstack((newFaces,np.array([f[0:3]]),np.array([f[0],f[2],f[3]]))) if f.shape[0]==4 else np.vstack((newFaces,f))
+    newFaces=np.delete(newFaces,0,axis=0)
+        
+    return newFaces
+
 def transform_dataframe(df:pd.DataFrame,transform:np.array,pointFields:List[str]=['x', 'y', 'z','Nx', 'Ny', 'Nz'])->pd.DataFrame:
     """apply rigid body transformation to the 3D point coordinates[x,y,z] in a pandas dataFrame.\n
 
     Args:
         1. df (pd.DataFrame)\n
         2. transform (np.array[4x4]): Rigid body transformation.\n
         3. pointFields (List[str], optional): names of the dataFrame columns. Defaults to ['x', 'y', 'z','Nx', 'Ny', 'Nz'].\n
@@ -2269,14 +2485,15 @@
             bounds[2*i+1]+=1
             res+=1
         #generate values       
         values.append( np.arange(bounds[2*i], bounds[2*i+1], res )) 
     grid  = np.meshgrid(values[0],values[1],values[2])
     return np.stack(grid)
 
+
 def crop_geometry_by_distance(source: o3d.geometry.Geometry, reference:List[o3d.geometry.Geometry], threshold : float =0.1) -> o3d.geometry.PointCloud:
     """Returns the portion of a pointcloud that lies within a range of another mesh/point cloud.\n
     
     .. image:: ../../../docs/pics/crop_by_distance2.PNG
 
     Args:
         1. source (o3d.geometry.TriangleMesh or o3d.geometry.PointCloud) : point cloud to filter \n
```

### Comparing `geomapi-0.3.1/geomapi/utils/imageutils.py` & `geomapi-0.3.2/geomapi/utils/imageutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/geomapi.egg-info/PKG-INFO` & `geomapi-0.3.2/geomapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapi
-Version: 0.3.1
+Version: 0.3.2
 Summary: A standard library to manage geomatic data
 Home-page: https://geomatics.pages.gitlab.kuleuven.be/research-projects/geomapi/
 Author: Bassier M., De Geyter S., De Winter H., Vermandere J. @ Geomatics KU Leuven
 License: MIT
 Keywords: Geomatics,alignment,monitoring,validation,progress,point clouds,computer vision,deep learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geomapi-0.3.1/geomapi.egg-info/SOURCES.txt` & `geomapi-0.3.2/geomapi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 geomapi/tools/alignmenttools/params.py
 geomapi/tools/completiontools/__init__.py
 geomapi/tools/inspectiontools/__init__.py
 geomapi/tools/machinelearningtools/__init__.py
 geomapi/tools/progresstools/__init__.py
 geomapi/tools/validationtools/__init__.py
 geomapi/utils/__init__.py
+geomapi/utils/cadutils.py
 geomapi/utils/geometryutils.py
 geomapi/utils/geospatialutils.py
 geomapi/utils/imageutils.py
 test/__init__.py
 test/test_alignmenttools.py
 test/test_bimnode.py
 test/test_completiontools.py
```

### Comparing `geomapi-0.3.1/setup.cfg` & `geomapi-0.3.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = geomapi
-version = 0.3.1
+version = 0.3.2
 author = Bassier M., De Geyter S., De Winter H., Vermandere J. @ Geomatics KU Leuven
 description = A standard library to manage geomatic data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://geomatics.pages.gitlab.kuleuven.be/research-projects/geomapi/
 keywords = Geomatics, alignment, monitoring, validation, progress, point clouds, computer vision, deep learning
 License = MIT
```

### Comparing `geomapi-0.3.1/test/test_alignmenttools.py` & `geomapi-0.3.2/test/test_alignmenttools.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/test/test_bimnode.py` & `geomapi-0.3.2/test/test_bimnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/test/test_completiontools.py` & `geomapi-0.3.2/test/test_completiontools.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/test/test_geometrynode.py` & `geomapi-0.3.2/test/test_geometrynode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/test/test_geometryutils.py` & `geomapi-0.3.2/test/test_geometryutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/test/test_geospatialutils.py` & `geomapi-0.3.2/test/test_geospatialutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/test/test_imageutils.py` & `geomapi-0.3.2/test/test_imageutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/test/test_imgnode.py` & `geomapi-0.3.2/test/test_imgnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/test/test_meshnode.py` & `geomapi-0.3.2/test/test_meshnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/test/test_node.py` & `geomapi-0.3.2/test/test_node.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/test/test_pointcloudnode.py` & `geomapi-0.3.2/test/test_pointcloudnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/test/test_progresstools.py` & `geomapi-0.3.2/test/test_progresstools.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/test/test_sessionnode.py` & `geomapi-0.3.2/test/test_sessionnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.1/test/test_tools.py` & `geomapi-0.3.2/test/test_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,32 +288,32 @@
         self.assertEqual(len(nodes),len(subjects))
 
         #with getResource
         nodes=tl.graph_path_to_nodes(graphPath=self.resourceGraphPath,getResource=True)
         geometries=[n.resource for n in nodes]
         self.assertEqual(len(nodes),len(geometries))
 
-    def test_select_k_nearest_nodes(self):
-        nodes=tl.graph_path_to_nodes(graphPath=self.bimGraphPath1,getResource=True)
-        list,distances=tl.select_k_nearest_nodes(nodes[0],nodes)
-        self.assertEqual(len(list),4)
-
-        #error k<=0
-        self.assertRaises(ValueError,tl.select_k_nearest_nodes,node=nodes[0],nodelist=nodes,k=-5 )
-
-    def test_select_nodes_with_centers_in_radius(self):
-        nodes=tl.graph_path_to_nodes(graphPath=self.bimGraphPath2,getResource=True)
-        list,distances=tl.select_nodes_with_centers_in_radius(nodes[0],nodes,r=10)
-        self.assertEqual(len(list),1)
-        for d in distances:
-            self.assertLess(d,10)
-
-        #error r<=0
-        self.assertRaises(ValueError,tl.select_nodes_with_centers_in_radius,nodes[0],nodes,r=0 )
-        self.assertRaises(ValueError,tl.select_nodes_with_centers_in_radius,nodes[0],nodes,r=-5 )
+    # def test_select_k_nearest_nodes(self):
+    #     nodes=tl.graph_path_to_nodes(graphPath=self.bimGraphPath1,getResource=True)
+    #     list,distances=tl.select_k_nearest_nodes(nodes[0],nodes)
+    #     self.assertEqual(len(list),4)
+
+    #     #error k<=0
+    #     self.assertRaises(ValueError,tl.select_k_nearest_nodes,node=nodes[0],nodelist=nodes,k=-5 )
+
+    # def test_select_nodes_with_centers_in_radius(self):
+    #     nodes=tl.graph_path_to_nodes(graphPath=self.bimGraphPath2,getResource=True)
+    #     list,distances=tl.select_nodes_with_centers_in_radius(nodes[0],nodes,r=10)
+    #     self.assertEqual(len(list),1)
+    #     for d in distances:
+    #         self.assertLess(d,10)
+
+    #     #error r<=0
+    #     self.assertRaises(ValueError,tl.select_nodes_with_centers_in_radius,nodes[0],nodes,r=0 )
+    #     self.assertRaises(ValueError,tl.select_nodes_with_centers_in_radius,nodes[0],nodes,r=-5 )
 
     def test_select_nodes_with_centers_in_bounding_box(self): 
         nodes=tl.graph_path_to_nodes(graphPath=self.bimGraphPath3,getResource=True)
         list=tl.select_nodes_with_centers_in_bounding_box(nodes[0],nodes,u=5,v=5,w=5)
         self.assertEqual(len(list),1)
 
         # no nodes
```

### Comparing `geomapi-0.3.1/test/test_utils.py` & `geomapi-0.3.2/test/test_utils.py`

 * *Files identical despite different names*

