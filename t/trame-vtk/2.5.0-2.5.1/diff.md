# Comparing `tmp/trame-vtk-2.5.0.tar.gz` & `tmp/trame-vtk-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-vtk-2.5.0.tar", last modified: Fri Jun 16 22:29:27 2023, max compression
+gzip compressed data, was "trame-vtk-2.5.1.tar", last modified: Fri Jun 23 21:12:15 2023, max compression
```

## Comparing `trame-vtk-2.5.0.tar` & `trame-vtk-2.5.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.389058 trame-vtk-2.5.0/
--rw-r--r--   0 root         (0) root         (0)     1504 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    13038 2023-06-16 22:29:27.389058 trame-vtk-2.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12303 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/README.rst
--rw-r--r--   0 root         (0) root         (0)      878 2023-06-16 22:29:27.389058 trame-vtk-2.5.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.373057 trame-vtk-2.5.0/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.373057 trame-vtk-2.5.0/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame/modules/paraview.py
--rw-r--r--   0 root         (0) root         (0)       39 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame/modules/vtk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.373057 trame-vtk-2.5.0/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame/widgets/paraview.py
--rw-r--r--   0 root         (0) root         (0)      172 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame/widgets/vtk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.373057 trame-vtk-2.5.0/trame_vtk/
--rw-r--r--   0 root         (0) root         (0)     1504 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/LICENSE
--rw-r--r--   0 root         (0) root         (0)       91 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.377057 trame-vtk-2.5.0/trame_vtk/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.377057 trame-vtk-2.5.0/trame_vtk/modules/common/
--rw-r--r--   0 root         (0) root         (0)      354 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.377057 trame-vtk-2.5.0/trame_vtk/modules/common/serve/
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/common/serve/.gitignore
--rw-r--r--   0 root         (0) root         (0)  1693943 2023-06-16 22:29:24.000000 trame-vtk-2.5.0/trame_vtk/modules/common/serve/trame-vtk.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.381058 trame-vtk-2.5.0/trame_vtk/modules/paraview/
--rw-r--r--   0 root         (0) root         (0)     7755 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/paraview/__init__.py
--rw-r--r--   0 root         (0) root         (0)      627 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/paraview/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.381058 trame-vtk-2.5.0/trame_vtk/modules/paraview/protocols/
--rw-r--r--   0 root         (0) root         (0)      363 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/paraview/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5356 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/paraview/protocols/local_rendering.py
--rw-r--r--   0 root         (0) root         (0)     2233 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/paraview/protocols/mouse_handler.py
--rw-r--r--   0 root         (0) root         (0)    23952 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/paraview/protocols/publish_image_delivery.py
--rw-r--r--   0 root         (0) root         (0)     3565 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/paraview/protocols/view_port.py
--rw-r--r--   0 root         (0) root         (0)     4170 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/paraview/protocols/web_protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.381058 trame-vtk-2.5.0/trame_vtk/modules/vtk/
--rw-r--r--   0 root         (0) root         (0)     7518 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2624 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.385058 trame-vtk-2.5.0/trame_vtk/modules/vtk/protocols/
--rw-r--r--   0 root         (0) root         (0)      322 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/protocols/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5574 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/protocols/local_rendering.py
--rw-r--r--   0 root         (0) root         (0)     3981 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/protocols/mouse_handler.py
--rw-r--r--   0 root         (0) root         (0)    12797 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/protocols/publish_image_delivery.py
--rw-r--r--   0 root         (0) root         (0)     1973 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/protocols/view_port.py
--rw-r--r--   0 root         (0) root         (0)     1787 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/protocols/web_protocol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.389058 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/
--rw-r--r--   0 root         (0) root         (0)      726 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12646 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/actors.py
--rw-r--r--   0 root         (0) root         (0)      463 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/cache.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/data.py
--rw-r--r--   0 root         (0) root         (0)      926 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/export.py
--rw-r--r--   0 root         (0) root         (0)     5785 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/helpers.py
--rw-r--r--   0 root         (0) root         (0)     4664 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/lights.py
--rw-r--r--   0 root         (0) root         (0)     6115 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/lookup_tables.py
--rw-r--r--   0 root         (0) root         (0)     5431 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/mappers.py
--rw-r--r--   0 root         (0) root         (0)     6041 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/mesh.py
--rw-r--r--   0 root         (0) root         (0)     3471 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/properties.py
--rw-r--r--   0 root         (0) root         (0)      378 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/registry.py
--rw-r--r--   0 root         (0) root         (0)     4978 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/render_windows.py
--rw-r--r--   0 root         (0) root         (0)      914 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/serialize.py
--rw-r--r--   0 root         (0) root         (0)     3541 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/synchronization_context.py
--rw-r--r--   0 root         (0) root         (0)     1337 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/textures.py
--rw-r--r--   0 root         (0) root         (0)     1946 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/utils.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/widgets.py
--rw-r--r--   0 root         (0) root         (0)     4551 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/modules/vtk/widget.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.389058 trame-vtk-2.5.0/trame_vtk/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/widgets/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.389058 trame-vtk-2.5.0/trame_vtk/widgets/vtk/
--rw-r--r--   0 root         (0) root         (0)      645 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/widgets/vtk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32816 2023-06-16 22:29:23.000000 trame-vtk-2.5.0/trame_vtk/widgets/vtk/common.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 22:29:27.377057 trame-vtk-2.5.0/trame_vtk.egg-info/
--rw-r--r--   0 root         (0) root         (0)    13038 2023-06-16 22:29:27.000000 trame-vtk-2.5.0/trame_vtk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2338 2023-06-16 22:29:27.000000 trame-vtk-2.5.0/trame_vtk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 22:29:27.000000 trame-vtk-2.5.0/trame_vtk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-06-16 22:29:27.000000 trame-vtk-2.5.0/trame_vtk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-16 22:29:27.000000 trame-vtk-2.5.0/trame_vtk.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.928688 trame-vtk-2.5.1/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    13038 2023-06-23 21:12:15.928688 trame-vtk-2.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12303 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)      878 2023-06-23 21:12:15.928688 trame-vtk-2.5.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame/modules/paraview.py
+-rw-r--r--   0 root         (0) root         (0)       39 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame/modules/vtk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame/widgets/paraview.py
+-rw-r--r--   0 root         (0) root         (0)      172 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame/widgets/vtk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame_vtk/
+-rw-r--r--   0 root         (0) root         (0)     1504 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       91 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame_vtk/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame_vtk/modules/common/
+-rw-r--r--   0 root         (0) root         (0)      354 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame_vtk/modules/common/serve/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/common/serve/.gitignore
+-rw-r--r--   0 root         (0) root         (0)  1693943 2023-06-23 21:12:13.000000 trame-vtk-2.5.1/trame_vtk/modules/common/serve/trame-vtk.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame_vtk/modules/paraview/
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      627 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.924688 trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/
+-rw-r--r--   0 root         (0) root         (0)      363 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5356 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/local_rendering.py
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/mouse_handler.py
+-rw-r--r--   0 root         (0) root         (0)    23952 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/publish_image_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     3565 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/view_port.py
+-rw-r--r--   0 root         (0) root         (0)     4170 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/web_protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.924688 trame-vtk-2.5.1/trame_vtk/modules/vtk/
+-rw-r--r--   0 root         (0) root         (0)     7518 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.924688 trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/
+-rw-r--r--   0 root         (0) root         (0)      322 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5574 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/local_rendering.py
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/mouse_handler.py
+-rw-r--r--   0 root         (0) root         (0)    12797 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/publish_image_delivery.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/view_port.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/web_protocol.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.924688 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/
+-rw-r--r--   0 root         (0) root         (0)      726 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12646 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/actors.py
+-rw-r--r--   0 root         (0) root         (0)      463 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/cache.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/data.py
+-rw-r--r--   0 root         (0) root         (0)      926 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/export.py
+-rw-r--r--   0 root         (0) root         (0)     5785 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/helpers.py
+-rw-r--r--   0 root         (0) root         (0)     4664 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/lights.py
+-rw-r--r--   0 root         (0) root         (0)     6059 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/lookup_tables.py
+-rw-r--r--   0 root         (0) root         (0)     5431 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/mappers.py
+-rw-r--r--   0 root         (0) root         (0)     6041 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/mesh.py
+-rw-r--r--   0 root         (0) root         (0)     3471 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/properties.py
+-rw-r--r--   0 root         (0) root         (0)      378 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/registry.py
+-rw-r--r--   0 root         (0) root         (0)     4978 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/render_windows.py
+-rw-r--r--   0 root         (0) root         (0)      914 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     3541 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/synchronization_context.py
+-rw-r--r--   0 root         (0) root         (0)     1337 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/textures.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/widgets.py
+-rw-r--r--   0 root         (0) root         (0)     4551 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/modules/vtk/widget.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.924688 trame-vtk-2.5.1/trame_vtk/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/widgets/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.924688 trame-vtk-2.5.1/trame_vtk/widgets/vtk/
+-rw-r--r--   0 root         (0) root         (0)      645 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/widgets/vtk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32816 2023-06-23 21:12:10.000000 trame-vtk-2.5.1/trame_vtk/widgets/vtk/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 21:12:15.920688 trame-vtk-2.5.1/trame_vtk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13038 2023-06-23 21:12:15.000000 trame-vtk-2.5.1/trame_vtk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2338 2023-06-23 21:12:15.000000 trame-vtk-2.5.1/trame_vtk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 21:12:15.000000 trame-vtk-2.5.1/trame_vtk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-23 21:12:15.000000 trame-vtk-2.5.1/trame_vtk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-23 21:12:15.000000 trame-vtk-2.5.1/trame_vtk.egg-info/top_level.txt
```

### Comparing `trame-vtk-2.5.0/LICENSE` & `trame-vtk-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/PKG-INFO` & `trame-vtk-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtk
-Version: 2.5.0
+Version: 2.5.1
 Summary: VTK widgets for trame
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `trame-vtk-2.5.0/README.rst` & `trame-vtk-2.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/setup.cfg` & `trame-vtk-2.5.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-vtk
-version = 2.5.0
+version = 2.5.1
 description = VTK widgets for trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = BSD License
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-vtk-2.5.0/trame_vtk/LICENSE` & `trame-vtk-2.5.1/trame_vtk/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/common/serve/trame-vtk.js` & `trame-vtk-2.5.1/trame_vtk/modules/common/serve/trame-vtk.js`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/paraview/__init__.py` & `trame-vtk-2.5.1/trame_vtk/modules/paraview/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/paraview/core.py` & `trame-vtk-2.5.1/trame_vtk/modules/paraview/core.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/paraview/protocols/local_rendering.py` & `trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/local_rendering.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/paraview/protocols/mouse_handler.py` & `trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/mouse_handler.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/paraview/protocols/publish_image_delivery.py` & `trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/publish_image_delivery.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/paraview/protocols/view_port.py` & `trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/view_port.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/paraview/protocols/web_protocol.py` & `trame-vtk-2.5.1/trame_vtk/modules/paraview/protocols/web_protocol.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/__init__.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/core.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/core.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/protocols/local_rendering.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/local_rendering.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/protocols/mouse_handler.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/mouse_handler.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/protocols/publish_image_delivery.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/publish_image_delivery.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/protocols/view_port.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/view_port.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/protocols/web_protocol.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/protocols/web_protocol.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/__init__.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/actors.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/actors.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/data.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/data.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/export.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/export.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/helpers.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/helpers.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/initialize.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/initialize.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/lights.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/lights.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/lookup_tables.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/lookup_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,16 +100,14 @@
             instance.GetDiscretize() if hasattr(instance, "GetDiscretize") else 0
         )
         number_of_values = (
             instance.GetNumberOfValues()
             if hasattr(instance, "GetNumberOfValues")
             else 256
         )
-    elif number_of_values < 256:
-        discretize = 1
 
     return {
         "parent": reference_id(parent),
         "id": obj_id,
         "type": class_name(instance),
         "properties": cache_properties(
             obj_id,
```

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/mappers.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/mappers.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/mesh.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/mesh.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/properties.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/properties.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/render_windows.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/render_windows.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/serialize.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/serialize.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/synchronization_context.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/synchronization_context.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/textures.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/textures.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/utils.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/utils.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/serializers/widgets.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/serializers/widgets.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/modules/vtk/widget.py` & `trame-vtk-2.5.1/trame_vtk/modules/vtk/widget.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/widgets/vtk/__init__.py` & `trame-vtk-2.5.1/trame_vtk/widgets/vtk/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk/widgets/vtk/common.py` & `trame-vtk-2.5.1/trame_vtk/widgets/vtk/common.py`

 * *Files identical despite different names*

### Comparing `trame-vtk-2.5.0/trame_vtk.egg-info/PKG-INFO` & `trame-vtk-2.5.1/trame_vtk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame-vtk
-Version: 2.5.0
+Version: 2.5.1
 Summary: VTK widgets for trame
 Author: Kitware Inc.
 License: BSD License
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `trame-vtk-2.5.0/trame_vtk.egg-info/SOURCES.txt` & `trame-vtk-2.5.1/trame_vtk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

