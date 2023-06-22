# Comparing `tmp/sage_flatsurf-0.4.7.tar.gz` & `tmp/sage_flatsurf-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sage_flatsurf-0.4.7.tar", last modified: Fri Jul  8 11:26:46 2022, max compression
+gzip compressed data, was "sage_flatsurf-0.5.0.tar", last modified: Thu Jun 22 23:26:14 2023, max compression
```

## Comparing `sage_flatsurf-0.4.7.tar` & `sage_flatsurf-0.5.0.tar`

### file list

```diff
@@ -1,58 +1,69 @@
-drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2022-07-08 11:26:46.876907 sage_flatsurf-0.4.7/
--rw-r--r--   0 jule      (1000) jule      (1000)    15170 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/COPYING
--rw-r--r--   0 jule      (1000) jule      (1000)       50 2022-06-17 08:44:17.000000 sage_flatsurf-0.4.7/MANIFEST.in
--rw-r--r--   0 jule      (1000) jule      (1000)     5926 2022-07-08 11:26:46.876907 sage_flatsurf-0.4.7/PKG-INFO
--rw-r--r--   0 jule      (1000) jule      (1000)     5149 2022-06-17 08:44:17.000000 sage_flatsurf-0.4.7/README.rst
-drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2022-07-08 11:26:46.866907 sage_flatsurf-0.4.7/flatsurf/
--rw-r--r--   0 jule      (1000) jule      (1000)     1005 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/__init__.py
--rw-r--r--   0 jule      (1000) jule      (1000)     1188 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/features.py
-drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2022-07-08 11:26:46.876907 sage_flatsurf-0.4.7/flatsurf/geometry/
--rw-r--r--   0 jule      (1000) jule      (1000)      709 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/__init__.py
--rw-r--r--   0 jule      (1000) jule      (1000)     4686 2022-03-01 05:26:59.000000 sage_flatsurf-0.4.7/flatsurf/geometry/chamanara.py
--rw-r--r--   0 jule      (1000) jule      (1000)     8366 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/circle.py
--rw-r--r--   0 jule      (1000) jule      (1000)     3596 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/cone_surface.py
--rw-r--r--   0 jule      (1000) jule      (1000)    16639 2022-03-01 05:26:59.000000 sage_flatsurf-0.4.7/flatsurf/geometry/delaunay.py
--rw-r--r--   0 jule      (1000) jule      (1000)      976 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/dilation_surface.py
--rw-r--r--   0 jule      (1000) jule      (1000)    12334 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/finitely_generated_matrix_group.py
--rw-r--r--   0 jule      (1000) jule      (1000)    12288 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/fundamental_group.py
--rw-r--r--   0 jule      (1000) jule      (1000)    51542 2022-07-08 11:22:45.000000 sage_flatsurf-0.4.7/flatsurf/geometry/gl2r_orbit_closure.py
--rw-r--r--   0 jule      (1000) jule      (1000)    15518 2022-03-01 05:26:59.000000 sage_flatsurf-0.4.7/flatsurf/geometry/half_dilation_surface.py
--rw-r--r--   0 jule      (1000) jule      (1000)    11563 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/half_translation_surface.py
--rw-r--r--   0 jule      (1000) jule      (1000)     7249 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/interval_exchange_transformation.py
--rw-r--r--   0 jule      (1000) jule      (1000)    12145 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/l_infinity_delaunay_cells.py
--rw-r--r--   0 jule      (1000) jule      (1000)    34655 2022-03-01 05:26:59.000000 sage_flatsurf-0.4.7/flatsurf/geometry/mappings.py
--rw-r--r--   0 jule      (1000) jule      (1000)     8378 2022-06-01 08:14:33.000000 sage_flatsurf-0.4.7/flatsurf/geometry/matrix_2x2.py
--rw-r--r--   0 jule      (1000) jule      (1000)     4480 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/mega_wollmilchsau.py
--rw-r--r--   0 jule      (1000) jule      (1000)     8858 2022-06-01 08:14:33.000000 sage_flatsurf-0.4.7/flatsurf/geometry/minimal_cover.py
--rw-r--r--   0 jule      (1000) jule      (1000)   110772 2022-06-10 11:19:45.000000 sage_flatsurf-0.4.7/flatsurf/geometry/polygon.py
--rw-r--r--   0 jule      (1000) jule      (1000)    15073 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/polyhedra.py
--rw-r--r--   0 jule      (1000) jule      (1000)    10843 2022-07-08 11:22:45.000000 sage_flatsurf-0.4.7/flatsurf/geometry/pyflatsurf_conversion.py
--rw-r--r--   0 jule      (1000) jule      (1000)     1149 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/rational_cone_surface.py
--rw-r--r--   0 jule      (1000) jule      (1000)     2735 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/rational_similarity_surface.py
--rw-r--r--   0 jule      (1000) jule      (1000)     6502 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/relative_homology.py
--rw-r--r--   0 jule      (1000) jule      (1000)    18809 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/similarity.py
--rw-r--r--   0 jule      (1000) jule      (1000)   101335 2022-06-01 08:14:33.000000 sage_flatsurf-0.4.7/flatsurf/geometry/similarity_surface.py
--rw-r--r--   0 jule      (1000) jule      (1000)    53425 2022-06-10 11:19:45.000000 sage_flatsurf-0.4.7/flatsurf/geometry/similarity_surface_generators.py
--rw-r--r--   0 jule      (1000) jule      (1000)    31149 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/straight_line_trajectory.py
--rw-r--r--   0 jule      (1000) jule      (1000)    13641 2022-03-01 05:06:10.000000 sage_flatsurf-0.4.7/flatsurf/geometry/subfield.py
--rw-r--r--   0 jule      (1000) jule      (1000)    60090 2022-03-01 05:26:59.000000 sage_flatsurf-0.4.7/flatsurf/geometry/surface.py
--rw-r--r--   0 jule      (1000) jule      (1000)    39877 2022-03-01 05:26:59.000000 sage_flatsurf-0.4.7/flatsurf/geometry/surface_objects.py
--rw-r--r--   0 jule      (1000) jule      (1000)    24059 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/tangent_bundle.py
--rw-r--r--   0 jule      (1000) jule      (1000)     6405 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/thurston_veech.py
--rw-r--r--   0 jule      (1000) jule      (1000)    29508 2022-03-21 01:22:00.000000 sage_flatsurf-0.4.7/flatsurf/geometry/translation_surface.py
--rw-r--r--   0 jule      (1000) jule      (1000)     8523 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/geometry/xml.py
-drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2022-07-08 11:26:46.876907 sage_flatsurf-0.4.7/flatsurf/graphical/
--rw-r--r--   0 jule      (1000) jule      (1000)      728 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/graphical/__init__.py
--rw-r--r--   0 jule      (1000) jule      (1000)    11919 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/graphical/polygon.py
--rw-r--r--   0 jule      (1000) jule      (1000)     4338 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/graphical/straight_line_trajectory.py
--rw-r--r--   0 jule      (1000) jule      (1000)    42816 2022-03-01 05:26:59.000000 sage_flatsurf-0.4.7/flatsurf/graphical/surface.py
--rw-r--r--   0 jule      (1000) jule      (1000)     2293 2022-01-18 01:36:32.000000 sage_flatsurf-0.4.7/flatsurf/graphical/surface_point.py
--rw-r--r--   0 jule      (1000) jule      (1000)       18 2022-07-08 11:26:43.000000 sage_flatsurf-0.4.7/flatsurf/version.py
-drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2022-07-08 11:26:46.876907 sage_flatsurf-0.4.7/sage_flatsurf.egg-info/
--rw-r--r--   0 jule      (1000) jule      (1000)     5926 2022-07-08 11:26:46.000000 sage_flatsurf-0.4.7/sage_flatsurf.egg-info/PKG-INFO
--rw-r--r--   0 jule      (1000) jule      (1000)     1745 2022-07-08 11:26:46.000000 sage_flatsurf-0.4.7/sage_flatsurf.egg-info/SOURCES.txt
--rw-r--r--   0 jule      (1000) jule      (1000)        1 2022-07-08 11:26:46.000000 sage_flatsurf-0.4.7/sage_flatsurf.egg-info/dependency_links.txt
--rw-r--r--   0 jule      (1000) jule      (1000)       17 2022-07-08 11:26:46.000000 sage_flatsurf-0.4.7/sage_flatsurf.egg-info/requires.txt
--rw-r--r--   0 jule      (1000) jule      (1000)        9 2022-07-08 11:26:46.000000 sage_flatsurf-0.4.7/sage_flatsurf.egg-info/top_level.txt
--rw-r--r--   0 jule      (1000) jule      (1000)       38 2022-07-08 11:26:46.876907 sage_flatsurf-0.4.7/setup.cfg
--rw-r--r--   0 jule      (1000) jule      (1000)     1158 2022-07-08 11:26:43.000000 sage_flatsurf-0.4.7/setup.py
+drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-06-22 23:26:14.179195 sage_flatsurf-0.5.0/
+-rw-r--r--   0 jule      (1000) jule      (1000)    15170 2022-01-18 01:36:32.000000 sage_flatsurf-0.5.0/COPYING
+-rw-r--r--   0 jule      (1000) jule      (1000)       34 2023-03-22 01:49:20.000000 sage_flatsurf-0.5.0/MANIFEST.in
+-rw-r--r--   0 jule      (1000) jule      (1000)     3760 2023-06-22 23:26:14.179195 sage_flatsurf-0.5.0/PKG-INFO
+-rw-r--r--   0 jule      (1000) jule      (1000)     2964 2023-06-22 23:25:20.000000 sage_flatsurf-0.5.0/README.md
+drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-06-22 23:26:14.172528 sage_flatsurf-0.5.0/flatsurf/
+-rw-r--r--   0 jule      (1000) jule      (1000)      886 2023-06-22 23:01:04.000000 sage_flatsurf-0.5.0/flatsurf/__init__.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     1200 2023-06-05 21:37:59.000000 sage_flatsurf-0.5.0/flatsurf/features.py
+drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-06-22 23:26:14.175862 sage_flatsurf-0.5.0/flatsurf/geometry/
+-rw-r--r--   0 jule      (1000) jule      (1000)     1104 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/__init__.py
+drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-06-22 23:26:14.175862 sage_flatsurf-0.5.0/flatsurf/geometry/categories/
+-rw-r--r--   0 jule      (1000) jule      (1000)     8327 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/__init__.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    17139 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/cone_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    23407 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/dilation_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     9836 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/euclidean_polygonal_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    89332 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/euclidean_polygons.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    46720 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/euclidean_polygons_with_angles.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    25307 2023-06-22 23:01:20.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/half_translation_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     2344 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/hyperbolic_polygons.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    49604 2023-06-22 23:24:45.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/polygonal_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    19633 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/polygons.py
+-rw-r--r--   0 jule      (1000) jule      (1000)   112904 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/similarity_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     2588 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/surface_category.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    19608 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/topological_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    28889 2023-06-22 23:01:04.000000 sage_flatsurf-0.5.0/flatsurf/geometry/categories/translation_surfaces.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    10135 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/chamanara.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     8896 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/circle.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    46514 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/delaunay.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    18517 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/euclidean.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    13583 2023-06-22 23:24:45.000000 sage_flatsurf-0.5.0/flatsurf/geometry/finitely_generated_matrix_group.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    12790 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/fundamental_group.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    54160 2023-06-22 23:24:45.000000 sage_flatsurf-0.5.0/flatsurf/geometry/gl2r_orbit_closure.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    11740 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/half_dilation_surface.py
+-rw-r--r--   0 jule      (1000) jule      (1000)   459593 2023-06-22 23:24:45.000000 sage_flatsurf-0.5.0/flatsurf/geometry/hyperbolic.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     7303 2023-06-22 22:50:10.000000 sage_flatsurf-0.5.0/flatsurf/geometry/interval_exchange_transformation.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    13586 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/l_infinity_delaunay_cells.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    31194 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/mappings.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     5693 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/mega_wollmilchsau.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    26845 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/minimal_cover.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     5674 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/origami.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    59727 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/polygon.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    18571 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/polyhedra.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    11077 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/pyflatsurf_conversion.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     7658 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/relative_homology.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    21216 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/similarity.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    76748 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/similarity_surface_generators.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    32811 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/straight_line_trajectory.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    14681 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/subfield.py
+-rw-r--r--   0 jule      (1000) jule      (1000)   105338 2023-06-22 23:24:45.000000 sage_flatsurf-0.5.0/flatsurf/geometry/surface.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    89410 2023-06-22 23:24:45.000000 sage_flatsurf-0.5.0/flatsurf/geometry/surface_legacy.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    52257 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/surface_objects.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    26371 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/tangent_bundle.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     6402 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/geometry/thurston_veech.py
+drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-06-22 23:26:14.179195 sage_flatsurf-0.5.0/flatsurf/graphical/
+-rw-r--r--   0 jule      (1000) jule      (1000)     1122 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/graphical/__init__.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    48132 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/graphical/hyperbolic.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    12346 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/graphical/polygon.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     4456 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/graphical/straight_line_trajectory.py
+-rw-r--r--   0 jule      (1000) jule      (1000)    44815 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/graphical/surface.py
+-rw-r--r--   0 jule      (1000) jule      (1000)     2557 2023-06-22 22:55:37.000000 sage_flatsurf-0.5.0/flatsurf/graphical/surface_point.py
+-rw-r--r--   0 jule      (1000) jule      (1000)       18 2023-06-22 23:25:20.000000 sage_flatsurf-0.5.0/flatsurf/version.py
+drwxr-xr-x   0 jule      (1000) jule      (1000)        0 2023-06-22 23:26:14.179195 sage_flatsurf-0.5.0/sage_flatsurf.egg-info/
+-rw-r--r--   0 jule      (1000) jule      (1000)     3760 2023-06-22 23:26:14.000000 sage_flatsurf-0.5.0/sage_flatsurf.egg-info/PKG-INFO
+-rw-r--r--   0 jule      (1000) jule      (1000)     2278 2023-06-22 23:26:14.000000 sage_flatsurf-0.5.0/sage_flatsurf.egg-info/SOURCES.txt
+-rw-r--r--   0 jule      (1000) jule      (1000)        1 2023-06-22 23:26:14.000000 sage_flatsurf-0.5.0/sage_flatsurf.egg-info/dependency_links.txt
+-rw-r--r--   0 jule      (1000) jule      (1000)       17 2023-06-22 23:26:14.000000 sage_flatsurf-0.5.0/sage_flatsurf.egg-info/requires.txt
+-rw-r--r--   0 jule      (1000) jule      (1000)        9 2023-06-22 23:26:14.000000 sage_flatsurf-0.5.0/sage_flatsurf.egg-info/top_level.txt
+-rw-r--r--   0 jule      (1000) jule      (1000)       38 2023-06-22 23:26:14.179195 sage_flatsurf-0.5.0/setup.cfg
+-rw-r--r--   0 jule      (1000) jule      (1000)     2161 2023-06-22 23:25:20.000000 sage_flatsurf-0.5.0/setup.py
```

### Comparing `sage_flatsurf-0.4.7/COPYING` & `sage_flatsurf-0.5.0/COPYING`

 * *Files identical despite different names*

### Comparing `sage_flatsurf-0.4.7/flatsurf/features.py` & `sage_flatsurf-0.5.0/flatsurf/features.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,9 +18,13 @@
 #
 #  You should have received a copy of the GNU General Public License
 #  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
 # ####################################################################
 
 from sage.features import PythonModule
 
-cppyy_feature = PythonModule("cppyy", url="https://cppyy.readthedocs.io/en/latest/installation.html")
-pyflatsurf_feature = PythonModule("pyflatsurf", url="https://github.com/flatsurf/flatsurf/#install-with-conda")
+cppyy_feature = PythonModule(
+    "cppyy", url="https://cppyy.readthedocs.io/en/latest/installation.html"
+)
+pyflatsurf_feature = PythonModule(
+    "pyflatsurf", url="https://github.com/flatsurf/flatsurf/#install-with-conda"
+)
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/circle.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/circle.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,146 +1,167 @@
 r"""
-This class contains methods useful for working with circles. 
+This class contains methods useful for working with circles.
 
 This will be used to build a LazyDelaunayTriangulation class which will compute the
 Delaunay decomposition for infinite surfaces.
 """
-#*****************************************************************************
-#       Copyright (C) 2013-2019 Vincent Delecroix <20100.delecroix@gmail.com>
-#                     2013-2019 W. Patrick Hooper <wphooper@gmail.com>
+# ****************************************************************************
+#  This file is part of sage-flatsurf.
 #
-#  Distributed under the terms of the GNU General Public License (GPL)
-#  as published by the Free Software Foundation; either version 2 of
-#  the License, or (at your option) any later version.
-#                  https://www.gnu.org/licenses/
-#*****************************************************************************
-
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
+#       Copyright (C) 2013-2019 Vincent Delecroix
+#                     2013-2019 W. Patrick Hooper
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+# ****************************************************************************
 
 from sage.modules.free_module import VectorSpace
 from sage.modules.free_module_element import vector
 
-def circle_from_three_points(p,q,r,base_ring=None):
+
+def circle_from_three_points(p, q, r, base_ring=None):
     r"""
     Construct a circle from three points on the circle.
     """
     if base_ring is None:
-        base_ring=p.base_ring()
+        base_ring = p.base_ring()
     V2 = VectorSpace(base_ring.fraction_field(), 2)
     V3 = VectorSpace(base_ring.fraction_field(), 3)
-    
-    v1=V3((p[0]+q[0],p[1]+q[1],2))
-    v2=V3((p[1]-q[1],q[0]-p[0],0))
-    line1=v1.cross_product(v2)
-    v1=V3((p[0]+r[0],p[1]+r[1],2))
-    v2=V3((p[1]-r[1],r[0]-p[0],0))
-    line2=v1.cross_product(v2)
+
+    v1 = V3((p[0] + q[0], p[1] + q[1], 2))
+    v2 = V3((p[1] - q[1], q[0] - p[0], 0))
+    line1 = v1.cross_product(v2)
+    v1 = V3((p[0] + r[0], p[1] + r[1], 2))
+    v2 = V3((p[1] - r[1], r[0] - p[0], 0))
+    line2 = v1.cross_product(v2)
     center_3 = line1.cross_product(line2)
     if center_3[2].is_zero():
         raise ValueError("The three points lie on a line.")
-    center = V2( (center_3[0]/center_3[2], center_3[1]/center_3[2]) )
-    return Circle(center, (p[0]-center[0])**2+(p[1]-center[1])**2 )
+    center = V2((center_3[0] / center_3[2], center_3[1] / center_3[2]))
+    return Circle(center, (p[0] - center[0]) ** 2 + (p[1] - center[1]) ** 2)
+
 
 class Circle:
     def __init__(self, center, radius_squared, base_ring=None):
         r"""
         Construct a circle from a Vector representing the center, and the
         radius squared.
         """
         if base_ring is None:
             self._base_ring = radius_squared.parent()
         else:
             self._base_ring = base_ring
 
         # for calculations:
-        self._V2 = VectorSpace(self._base_ring,2)
-        self._V3 = VectorSpace(self._base_ring,3)
+        self._V2 = VectorSpace(self._base_ring, 2)
+        self._V3 = VectorSpace(self._base_ring, 3)
 
         self._center = self._V2(center)
         self._radius_squared = self._base_ring(radius_squared)
-        
+
     def center(self):
         r"""
         Return the center of the circle as a vector.
         """
         return self._center
-        
+
     def radius_squared(self):
         r"""
         Return the square of the radius of the circle.
         """
         return self._radius_squared
-    
+
     def point_position(self, point):
         r"""
         Return 1 if point lies in the circle, 0 if the point lies on the circle,
         and -1 if the point lies outide the circle.
         """
-        value = (point[0]-self._center[0])**2 + (point[1]-self._center[1])**2 - \
-            self._radius_squared
+        value = (
+            (point[0] - self._center[0]) ** 2
+            + (point[1] - self._center[1]) ** 2
+            - self._radius_squared
+        )
         if value > self._base_ring.zero():
             return -1
         if value < self._base_ring.zero():
             return 1
         return 0
-    
+
     def closest_point_on_line(self, point, direction_vector):
         r"""
         Consider the line through the provided point in the given direction.
         Return the closest point on this line to the center of the circle.
         """
-        cc = self._V3((self._center[0],self._center[1], self._base_ring.one()))
+        cc = self._V3((self._center[0], self._center[1], self._base_ring.one()))
         # point at infinite orthogonal to direction_vector:
-        dd = self._V3((direction_vector[1],-direction_vector[0], self._base_ring.zero()))
+        dd = self._V3(
+            (direction_vector[1], -direction_vector[0], self._base_ring.zero())
+        )
         l1 = cc.cross_product(dd)
-        
-        pp = self._V3((point[0],point[1], self._base_ring.one()))
+
+        pp = self._V3((point[0], point[1], self._base_ring.one()))
         # direction_vector pushed to infinity
-        ee = self._V3((direction_vector[0],direction_vector[1], self._base_ring.zero()))
+        ee = self._V3(
+            (direction_vector[0], direction_vector[1], self._base_ring.zero())
+        )
         l2 = pp.cross_product(ee)
-        
+
         # This is the point we want to return
         rr = l1.cross_product(l2)
         try:
-            return self._V2((rr[0]/rr[2], rr[1]/rr[2]))
+            return self._V2((rr[0] / rr[2], rr[1] / rr[2]))
         except ZeroDivisionError:
-            raise ValueError("Division by zero error. Perhaps direction is zero. "+\
-                "point="+str(point)+" direction="+str(direction_vector)+" circle="+\
-                str(self))
-
+            raise ValueError(
+                "Division by zero error. Perhaps direction is zero. "
+                + "point="
+                + str(point)
+                + " direction="
+                + str(direction_vector)
+                + " circle="
+                + str(self)
+            )
 
     def line_position(self, point, direction_vector):
         r"""
         Consider the line through the provided point in the given direction.
         We return 1 if the line passes through the circle, 0 if it is tangent
         to the circle and -1 if the line does not intersect the circle.
         """
-        return self.point_position(self.closest_point_on_line(point,direction_vector))
+        return self.point_position(self.closest_point_on_line(point, direction_vector))
 
     def line_segment_position(self, p, q):
         r"""
         Consider the open line segment pq.We return 1 if the line segment
-        enters the interior of the circle, zero if it touches the circle 
+        enters the interior of the circle, zero if it touches the circle
         tangentially (at a point in the interior of the segment) and
         and -1 if it does not touch the circle or its interior.
         """
-        if self.point_position(p)==1:
+        if self.point_position(p) == 1:
             return 1
-        if self.point_position(q)==1:
+        if self.point_position(q) == 1:
             return 1
-        r=self.closest_point_on_line(p,q-p)
+        r = self.closest_point_on_line(p, q - p)
         pos = self.point_position(r)
-        if pos ==-1:
+        if pos == -1:
             return -1
         # This checks if r lies in the interior of pq
-        if p[0]==q[0]:
-            if (p[1]<r[1] and r[1]<q[1]) or (p[1]>r[1] and r[1]>q[1]):
+        if p[0] == q[0]:
+            if (p[1] < r[1] and r[1] < q[1]) or (p[1] > r[1] and r[1] > q[1]):
                 return pos
-        elif (p[0]<r[0] and r[0]<q[0]) or (p[0]>r[0] and r[0]>q[0]):
+        elif (p[0] < r[0] and r[0] < q[0]) or (p[0] > r[0] and r[0] > q[0]):
             return pos
         # It does not lie in the interior.
         return -1
 
     def tangent_vector(self, point):
         r"""
         Return a vector based at the provided point (which must lie on the circle)
@@ -152,68 +173,71 @@
             sage: from flatsurf.geometry.circle import Circle
             sage: c=Circle(vector((0,0)), 2, base_ring=QQ)
             sage: c.tangent_vector(vector((1,1)))
             (-1, 1)
         """
         if not self.point_position(point) == 0:
             raise ValueError("point not on circle.")
-        return vector((self._center[1]-point[1], point[0]-self._center[0]))
-    
+        return vector((self._center[1] - point[1], point[0] - self._center[0]))
+
     def other_intersection(self, p, v):
         r"""
         Consider a point p on the circle and a vector v. Let L be the line
         through p in direction v. Then L intersects the circle at another
         point q. This method returns q.
-        
+
         Note that if p and v are both in the field of the circle,
         then so is q.
-        
+
         EXAMPLES::
 
             sage: from flatsurf.geometry.circle import Circle
             sage: c=Circle(vector((0,0)), 25, base_ring=QQ)
             sage: c.other_intersection(vector((3,4)),vector((1,2)))
             (-7/5, -24/5)
         """
-        pp=self._V3((p[0],p[1],self._base_ring.one()))
-        vv=self._V3((v[0],v[1],self._base_ring.zero()))
+        pp = self._V3((p[0], p[1], self._base_ring.one()))
+        vv = self._V3((v[0], v[1], self._base_ring.zero()))
         L = pp.cross_product(vv)
-        cc=self._V3((self._center[0],self._center[1],self._base_ring.one()))
-        vvperp=self._V3((-v[1],v[0],self._base_ring.zero()))
+        cc = self._V3((self._center[0], self._center[1], self._base_ring.one()))
+        vvperp = self._V3((-v[1], v[0], self._base_ring.zero()))
         # line perpendicular to L through center:
         Lperp = cc.cross_product(vvperp)
         # intersection of L and Lperp:
         rr = L.cross_product(Lperp)
-        r = self._V2((rr[0]/rr[2],rr[1]/rr[2]))
-        return self._V2((2*r[0]-p[0], 2*r[1]-p[1]))
+        r = self._V2((rr[0] / rr[2], rr[1] / rr[2]))
+        return self._V2((2 * r[0] - p[0], 2 * r[1] - p[1]))
 
     def __rmul__(self, similarity):
         r"""
         Apply a similarity to the circle.
-        
+
         EXAMPLES::
 
-            sage: from flatsurf import *
-            sage: from flatsurf.geometry.circle import *
+            sage: from flatsurf import translation_surfaces
             sage: s = translation_surfaces.square_torus()
             sage: c = s.polygon(0).circumscribing_circle()
             sage: c
             Circle((1/2, 1/2), 1/2)
             sage: s.edge_transformation(0,2)
             (x, y) |-> (x, y - 1)
             sage: s.edge_transformation(0,2) * c
             Circle((1/2, -1/2), 1/2)
         """
         from .similarity import SimilarityGroup
+
         SG = SimilarityGroup(self._base_ring)
         s = SG(similarity)
-        return Circle(s(self._center), \
-            s.det()*self._radius_squared, \
-            base_ring=self._base_ring)
+        return Circle(
+            s(self._center), s.det() * self._radius_squared, base_ring=self._base_ring
+        )
 
     def __str__(self):
-        return "circle with center "+str(self._center)+" and radius squared " + \
-            str(self._radius_squared)
-    
+        return (
+            "circle with center "
+            + str(self._center)
+            + " and radius squared "
+            + str(self._radius_squared)
+        )
+
     def __repr__(self):
-        return "Circle("+repr(self._center)+", "+repr(self._radius_squared)+")"
-    
+        return "Circle(" + repr(self._center) + ", " + repr(self._radius_squared) + ")"
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/finitely_generated_matrix_group.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/finitely_generated_matrix_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,10 @@
 r"""
 Class for matrix groups generated by a finite number of elements.
 
-.. TODO::
-
-    - The stupid test ``_test_change_ring`` fails because if a matrix ``m`` is
-      immutable then ``m.change_ring(m.base_ring())`` returns ``m`` and not a
-      copy.
-
-    - ``m.multiplicative_order()``
-
 EXAMPLES::
 
     sage: from flatsurf.geometry.finitely_generated_matrix_group import  FinitelyGenerated2x2MatrixGroup
 
     sage: m1 = matrix([[1,1],[0,1]])
     sage: m2 = matrix([[1,0],[1,1]])
     sage: G = FinitelyGenerated2x2MatrixGroup([m1,m2])
@@ -25,26 +17,34 @@
     [
     [1 0]  [1 1]  [1 2]  [2 1]  [ 0  1]
     [0 1], [0 1], [0 1], [1 1], [-1  1]
     ]
 
     sage: G = FinitelyGenerated2x2MatrixGroup([identity_matrix(2)])
 """
-#*****************************************************************************
-#       Copyright (C) 2013-2019 Vincent Delecroix <20100.delecroix@gmail.com>
-#                     2013-2019 W. Patrick Hooper <wphooper@gmail.com>
+# ****************************************************************************
+#  This file is part of sage-flatsurf.
 #
-#  Distributed under the terms of the GNU General Public License (GPL)
-#  as published by the Free Software Foundation; either version 2 of
-#  the License, or (at your option) any later version.
-#                  https://www.gnu.org/licenses/
-#*****************************************************************************
-
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
+#       Copyright (C) 2013-2019 Vincent Delecroix
+#                     2013-2019 W. Patrick Hooper
+#                          2023 Julian Rüth <julian.rueth@fsfe.org>
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+# ****************************************************************************
 
 from sage.rings.integer import Integer
 from sage.structure.parent import Parent
 from sage.groups.group import Group
 from sage.structure.sequence import Sequence
 from sage.rings.infinity import Infinity
 from sage.matrix.constructor import matrix
@@ -113,23 +113,37 @@
         ....:     assert r.transpose() * m * r == m
     """
     if m.is_scalar():
         raise ValueError("m must be non scalar")
     s = m.det()
     if not s.is_unit():
         raise ValueError("determinant must be +1 or -1")
-    a,b,c,d = m.list()
-    V = matrix(m.base_ring(), 4, 3,
-              [a-s*d,     0, (1+s)*c,
-                 s*b,     c,  (1-s)*a,
-                   b,   s*c,  (1-s)*d,
-                   0,   d-s*a, (1+s)*b]
-              ).right_kernel()
+    a, b, c, d = m.list()
+    V = matrix(
+        m.base_ring(),
+        4,
+        3,
+        [
+            a - s * d,
+            0,
+            (1 + s) * c,
+            s * b,
+            c,
+            (1 - s) * a,
+            b,
+            s * c,
+            (1 - s) * d,
+            0,
+            d - s * a,
+            (1 + s) * b,
+        ],
+    ).right_kernel()
     return V
 
+
 def contains_definite_form(V):
     r"""
     Check whether a given a subspace of the 3 dimensional space (a,b,c) contains
     a definitive positive quadratic form ax^2 + 2bxy + by^2.
 
     TESTS::
 
@@ -149,78 +163,97 @@
         sage: contains_definite_form(V.submodule([(-1,0,0),(0,1,3)]))
         True
     """
     dim = V.dimension()
     if dim == 0:
         return False
     elif dim == 1:
-        a,c,b = V.gen(0)
-        return b**2 < a*c
+        a, c, b = V.gen(0)
+        return b**2 < a * c
     elif dim == 2:
-        a1,c1,b1 = V.gen(0)
-        a2,c2,b2 = V.gen(1)
-        if b1**2 < a1*c1 or b2**2 < a2*c2:
+        a1, c1, b1 = V.gen(0)
+        a2, c2, b2 = V.gen(1)
+        if b1**2 < a1 * c1 or b2**2 < a2 * c2:
             return True
-        return (2*b1*b2 - a2*c1 - a1*c2)**2 - 4 * (b1**2 - a1*c1) * (b2**2 - a2*c2) > 0
+        return (2 * b1 * b2 - a2 * c1 - a1 * c2) ** 2 - 4 * (b1**2 - a1 * c1) * (
+            b2**2 - a2 * c2
+        ) > 0
     elif dim == 3:
         return True
     else:
         raise RuntimeError
 
+
 def matrix_multiplicative_order(m):
     r"""
     Return the order of the 2x2 matrix ``m``.
     """
     if m.is_one():
         return Integer(1)
     elif m.det() != 1 and m.det() != -1:
         return Infinity
 
     # now we compute the potentially preserved quadratic form
     # i.e. looking for A such that m^t A m = A
-    m00 = m[0,0]
-    m01 = m[0,1]
-    m10 = m[1,0]
-    m11 = m[1,1]
-    M = matrix(m.base_ring(),
-        [[m00**2, m00*m10, m10**2],
-         [m00*m01, m00*m11, m10*m11],
-         [m01**2, m01*m11, m11**2]])
+    m00 = m[0, 0]
+    m01 = m[0, 1]
+    m10 = m[1, 0]
+    m11 = m[1, 1]
+    M = matrix(
+        m.base_ring(),
+        [
+            [m00**2, m00 * m10, m10**2],
+            [m00 * m01, m00 * m11, m10 * m11],
+            [m01**2, m01 * m11, m11**2],
+        ],
+    )
 
     # might there be several solutions ? (other than scaling)... should not
     try:
-        v = (M-identity_matrix(3)).solve_right()
-    except ValueError: # no solution
+        from sage.all import identity_matrix
+
+        v = (M - identity_matrix(3)).solve_right()
+    except ValueError:  # no solution
         return False
 
-    raise NotImplementedError("your matrix is conjugate to an orthogonal matrix but the angle might not be rational.. to be terminated.")
+    raise NotImplementedError(
+        "your matrix is conjugate to an orthogonal matrix but the angle might not be rational.. to be terminated."
+    )
 
     # then we conjugate and check if the angles are rational
     # we need to take a square root of a symmetric matrix... this is not implemented!
-    A = matrix(m.base_ring(), [[v[0],v[1]],[v[1],v[2]]])
-
+    # A = matrix(m.base_ring(), [[v[0], v[1]], [v[1], v[2]]])
 
 
 class FinitelyGenerated2x2MatrixGroup(Group):
     r"""
     Finitely generated group of 2x2 matrices with real coefficients
+
+    .. SEEALSO::
+
+        :py:mod:`sage.groups.group` for the general interface of groups
+        like this in SageMath
+
     """
+
     def __init__(self, matrices, matrix_space=None, category=None):
         if matrix_space is None:
             from sage.matrix.matrix_space import MatrixSpace
+
             ring = Sequence(matrices).universe().base_ring()
-            matrix_space = MatrixSpace(ring,2)
+            matrix_space = MatrixSpace(ring, 2)
 
-        self._generators = list(map(matrix_space,matrices))
+        self._generators = list(map(matrix_space, matrices))
         for m in self._generators:
             m.set_immutable()
         self._matrix_space = matrix_space
 
         if category is None:
             from sage.categories.groups import Groups
+
             category = Groups()
 
         Parent.__init__(self, category=category, facade=matrix_space)
 
     def is_abelian(self):
         r"""
         Check whether this group is abelian.
@@ -241,23 +274,26 @@
 
             sage: G = FinitelyGenerated2x2MatrixGroup([m1])
             sage: G.is_abelian()
             True
         """
         for a in self._generators:
             for b in self._generators:
-                if a*b != b*a:
+                if a * b != b * a:
                     return False
         return True
 
     def _repr_(self):
-        mat_string = [g.str().split('\n') for g in self._generators]
-        return ("Matrix group generated by:\n" +
-                "  ".join(x[0] for x in mat_string) + "\n" +
-                ", ".join(x[1] for x in mat_string))
+        mat_string = [g.str().split("\n") for g in self._generators]
+        return (
+            "Matrix group generated by:\n"
+            + "  ".join(x[0] for x in mat_string)
+            + "\n"
+            + ", ".join(x[1] for x in mat_string)
+        )
 
     def is_finite(self):
         r"""
         Check whether the group is finite.
 
         A group is finite if and only if it is conjugate to a (finite) subgroup
         of O(2). This is actually also true in higher dimensions.
@@ -297,26 +333,29 @@
             False
             sage: FinitelyGenerated2x2MatrixGroup([t*m2*~t, t*r*~t]).is_finite()
             False
         """
         # determinant and trace tests
         # (the code actually check that each generator is of finite order)
         for m in self._generators:
-            if (m.det() != 1 and m.det() != -1) or \
-               m.trace().abs() > 2 or \
-               (m.trace().abs() == 2 and (m[0,1] or m[1,0])):
-                   return False
+            if (
+                (m.det() != 1 and m.det() != -1)
+                or m.trace().abs() > 2
+                or (m.trace().abs() == 2 and (m[0, 1] or m[1, 0]))
+            ):
+                return False
 
         gens = [g for g in self._generators if not g.is_scalar()]
 
         if len(gens) <= 1:
             return True
 
         # now we try to find a non-trivial invariant quadratic form
         from sage.modules.free_module import FreeModule
+
         V = FreeModule(self._matrix_space.base_ring(), 3)
         for g in gens:
             V = V.intersection(invariant_quadratic_forms(g))
             if not contains_definite_form(V):
                 return False
 
         return True
@@ -334,36 +373,61 @@
         wait = self._generators[:]
         while wait:
             p = wait.pop(0)
             if p not in s:
                 yield p
                 s.add(p)
             for g in self._generators:
-                for m in [p*g, p*g.inverse(), g*p, g.inverse()*p]:
+                for m in [p * g, p * g.inverse(), g * p, g.inverse() * p]:
                     m.set_immutable()
                     if m not in s:
                         yield m
                         s.add(m)
                         wait.append(m)
 
     def __eq__(self, other):
-        return (isinstance(other, FinitelyGenerated2x2MatrixGroup) and
-                self._generators == other._generators)
+        return (
+            isinstance(other, FinitelyGenerated2x2MatrixGroup)
+            and self._generators == other._generators
+        )
 
     def some_elements(self):
         from itertools import islice
+
         return list(islice(self, 5))
 
     def __ne__(self, other):
         return not self == other
 
     def __reduce__(self):
         return FinitelyGenerated2x2MatrixGroup, (self._generators, self._matrix_space)
 
     def one(self):
         return self._matrix_space.identity_matrix()
 
-    def an_element(self):
+    def _an_element_(self):
+        r"""
+        Return a typical element of this group, namely a generator.
+
+        EXAMPLES:
+
+            sage: from flatsurf.geometry.finitely_generated_matrix_group import FinitelyGenerated2x2MatrixGroup
+            sage: G = FinitelyGenerated2x2MatrixGroup([identity_matrix(2)])
+
+            sage: G._an_element_()
+            [1 0]
+            [0 1]
+
+            sage: G.an_element()
+            [1 0]
+            [0 1]
+
+        .. SEEALSO::
+
+            :meth:`sage.structure.parent.Parent.an_element` which relies on
+            this method and should be called instead
+
+        """
         return self._generators[0]
 
     def gen(self, i):
         return self._generators[i]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/fundamental_group.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/fundamental_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-#*****************************************************************************
-#       Copyright (C) 2013-2019 Vincent Delecroix <20100.delecroix@gmail.com>
-#                     2013-2019 W. Patrick Hooper <wphooper@gmail.com>
+# ****************************************************************************
+#  This file is part of sage-flatsurf.
 #
-#  Distributed under the terms of the GNU General Public License (GPL)
-#  as published by the Free Software Foundation; either version 2 of
-#  the License, or (at your option) any later version.
-#                  https://www.gnu.org/licenses/
-#*****************************************************************************
-
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
+#       Copyright (C) 2013-2019 Vincent Delecroix
+#                     2013-2019 W. Patrick Hooper
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+# ****************************************************************************
 
 from sage.misc.cachefunc import cached_method
 
 from sage.structure.element import parent
 
 from sage.categories.groups import Groups
 from sage.groups.group import Group
 from sage.structure.element import MultiplicativeGroupElement
 from sage.structure.unique_representation import UniqueRepresentation
 
+
 def intersection(i0, j0, i1, j1):
     r"""
     Intersection inside a polygon.
 
     In case of equality we consider that i0 < i1 < j1 < j0
 
     INPUT:
@@ -55,18 +63,19 @@
         0
     """
     if i0 <= j0:  # that is i0 < j0 or i0 == j0
         return (i0 <= i1 <= j0) - (i0 <= j1 <= j0)
     else:
         return (j0 < j1 < i0) - (j0 < i1 < i0)
 
+
 class Path(MultiplicativeGroupElement):
-# activating the following somehow break the discovery of the Python _mul_
-# method below...
-#    __slots__ = ['_polys', '_edges', '_edges_rev']
+    # activating the following somehow break the discovery of the Python _mul_
+    # method below...
+    #    __slots__ = ['_polys', '_edges', '_edges_rev']
 
     def __init__(self, parent, polys, edge, edge_rev, check=True, reduced=False):
         self._polys = tuple(polys)
         self._edges = tuple(edge)
         self._edges_rev = tuple(edge_rev)
         MultiplicativeGroupElement.__init__(self, parent)
 
@@ -78,137 +87,143 @@
     def _reduce(self):
         r"""
         Remove
         """
         pass
 
     def _poly_cross_dict(self):
-        d = {p: [] for p in self.parent()._s.label_iterator()}
+        d = {p: [] for p in self.parent()._s.labels()}
         d[self._polys[0]].append((self._edges_rev[-1], self._edges[0]))
-        for i in range(1, len(self._polys)-1):
+        for i in range(1, len(self._polys) - 1):
             p = self._polys[i]
-            e0 = self._edges_rev[i-1]
+            e0 = self._edges_rev[i - 1]
             e1 = self._edges[i]
-            d[p].append((e0,e1))
+            d[p].append((e0, e1))
         return d
 
     def __hash__(self):
-        return hash(self._polys) ^ hash(self._edges)
+        return hash((self._polys, self._edges))
 
     def __eq__(self, other):
         r"""
         TESTS::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: t = translation_surfaces.square_torus()
             sage: F = t.fundamental_group()
             sage: a,b = F.gens()
             sage: a == b
             False
             sage: a*b == b*a
             False
             sage: a*b == a*b
             True
         """
-        return parent(self) is parent(other) and \
-               self._polys == other._polys and  \
-               self._edges == other._edges 
+        return (
+            parent(self) is parent(other)
+            and self._polys == other._polys
+            and self._edges == other._edges
+        )
 
     def __ne__(self, other):
         r"""
         TESTS::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: t = translation_surfaces.square_torus()
             sage: F = t.fundamental_group()
             sage: a,b = F.gens()
             sage: a != b
             True
             sage: a*b != b*a
             True
             sage: a*b != a*b
             False
         """
-        return parent(self) is not parent(other) or \
-               self._polys != other._polys or \
-               self._edges != other._edges
+        return (
+            parent(self) is not parent(other)
+            or self._polys != other._polys
+            or self._edges != other._edges
+        )
 
     def _check(self):
-        if not(len(self._polys)-1 == len(self._edges) == len(self._edges_rev)):
-            raise ValueError("polys = {}\nedges = {}\nedges_rev={}".format(
-                self._polys, self._edges, self._edges_rev))
+        if not (len(self._polys) - 1 == len(self._edges) == len(self._edges_rev)):
+            raise ValueError(
+                "polys = {}\nedges = {}\nedges_rev={}".format(
+                    self._polys, self._edges, self._edges_rev
+                )
+            )
         assert self._polys[0] == self.parent()._b == self._polys[-1]
 
     def is_one(self):
         return not self._edges
 
     def _repr_(self):
-        return "".join("{} --{}-- ".format(p,e)
-              for p,e in zip(self._polys, self._edges)) + \
-               "{}".format(self._polys[-1]) 
+        return "".join(
+            "{} --{}-- ".format(p, e) for p, e in zip(self._polys, self._edges)
+        ) + "{}".format(self._polys[-1])
 
     def _mul_(self, other):
         r"""
         TESTS::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: t = translation_surfaces.square_torus()
             sage: a,b = t.fundamental_group().gens()
             sage: a*b
             0 --0-- 0 --1-- 0
         """
         sp = self._polys[:]
         se = self._edges[:]
-        ser = self._edges_rev[:]
+        se_r = self._edges_rev[:]
 
         op = other._polys[:]
         oe = other._edges[:]
-        oer = other._edges_rev[:]
+        oe_r = other._edges_rev[:]
 
         if sp[-1] != op[0]:
             return None
 
         i = 0
-        while i < len(se) and i < len(oe) and se[-i-1] == oer[i]:
+        while i < len(se) and i < len(oe) and se[-i - 1] == oe_r[i]:
             i += 1
 
         P = self.parent()
         return P.element_class(
-                P,
-                sp[:len(sp)-i] + op[i+1:],
-                se[:len(se)-i]+ oe[i:],
-                ser[:len(ser)-i] + oer[i:])
+            P,
+            sp[: len(sp) - i] + op[i + 1 :],
+            se[: len(se) - i] + oe[i:],
+            se_r[: len(se_r) - i] + oe_r[i:],
+        )
 
     def __invert__(self):
         r"""
         TESTS::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: o = translation_surfaces.octagon_and_squares()
             sage: F = o.fundamental_group()
             sage: a1,a2,a3,a4,a5,a6 = F.gens()
             sage: (a1 * a2 * ~a2 * ~a1).is_one()
             True
             sage: (a1 * ~a2 * a2 * a1) == a1 * a1
             True
         """
         P = self.parent()
         return P.element_class(
-                P,
-                self._polys[::-1],
-                self._edges_rev[::-1],
-                self._edges[::-1])
+            P, self._polys[::-1], self._edges_rev[::-1], self._edges[::-1]
+        )
 
     def intersection(self, other):
         r"""
         The intersection number of this element with ``other``.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: t = translation_surfaces.square_torus()
             sage: a,b = t.fundamental_group().gens()
             sage: a.intersection(b)
             1
             sage: b.intersection(a)
             -1
 
@@ -260,46 +275,46 @@
             [ 1  1  0  0  0  0  0  1 -1]
             [ 1  1  0  0  0  0 -1  0 -1]
             [-1 -1  0  0  0  0  1  1  0]
         """
         si = self._poly_cross_dict()
         oi = other._poly_cross_dict()
         n = 0
-        for p in self.parent()._s.label_iterator():
-            for e0,e1 in si[p]:
-                for f0,f1 in oi[p]:
-                    n += intersection(e0,e1,f0,f1)
+        for p in self.parent()._s.labels():
+            for e0, e1 in si[p]:
+                for f0, f1 in oi[p]:
+                    n += intersection(e0, e1, f0, f1)
         return n
 
 
 class FundamentalGroup(UniqueRepresentation, Group):
     r"""
     The fundamental group of a punctured surface
 
     EXAMPLES::
 
-        sage: from flatsurf import *
+        sage: from flatsurf import translation_surfaces
         sage: t = translation_surfaces.square_torus()
         sage: TestSuite(t.fundamental_group()).run()
     """
     Element = Path
 
     def __init__(self, surface, base):
-        if not surface.is_finite():
+        if not surface.is_finite_type():
             raise ValueError("the method only work for finite surfaces")
         self._s = surface
         self._b = base
 
         Group.__init__(self, category=Groups().Infinite())
 
     def _element_constructor_(self, *args):
         r"""
         TESTS::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: S = SymmetricGroup(4)
             sage: r = S('(1,2)(3,4)')
             sage: u = S('(2,3)')
             sage: o = translation_surfaces.origami(r,u)
             sage: F = o.fundamental_group()
             sage: F([1,1])
             1 --1-- 2 --1-- 1
@@ -307,99 +322,96 @@
             1 --1-- 2 --2-- 3 --2-- 2 --3-- 1
 
             sage: F([1,2,3])
             Traceback (most recent call last):
             ...
             AssertionError
         """
-        if len(args) == 1 and isinstance(args[0], (tuple,list)):
+        if len(args) == 1 and isinstance(args[0], (tuple, list)):
             args = args[0]
         s = self._s
         p = [self._b]
         e = []
         er = []
         for i in args:
-            i = int(i) % s.polygon(p[-1]).num_edges()
-            q,j = s.opposite_edge(p[-1],i)
+            i = int(i) % len(s.polygon(p[-1]).vertices())
+            q, j = s.opposite_edge(p[-1], i)
             p.append(q)
             e.append(i)
             er.append(j)
         return self.element_class(self, p, e, er)
 
     def _repr_(self):
-        return "Fundamental group of {} based at polygon {}".format(
-                self._s,
-                self._b)
+        return "Fundamental group of {} based at polygon {}".format(self._s, self._b)
 
     @cached_method
     def one(self):
         return self.element_class(self, [self._b], [], [])
 
     @cached_method
     def gens(self):
         r"""
         Return a generating set
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: S = SymmetricGroup(8)
             sage: r = S('(1,2,3,4,5,6,7,8)')
             sage: u = S('(1,8,5,4)(2,3)(6,7)')
             sage: o = translation_surfaces.origami(r,u)
             sage: len(o.fundamental_group().gens())
             9
         """
         p = self._b
         s = self._s
-        tree = {}   # a tree whose root is base_label
+        tree = {}  # a tree whose root is base_label
         basis = []
 
-        tree[p] = (None,None,None)
+        tree[p] = (None, None, None)
 
-        wait = [] # list of edges of the dual graph, ie p1 -- (e1,e2) --> p2
-        for e in range(s.polygon(p).num_edges()):
-            pp,ee = s.opposite_edge(p,e)
-            wait.append((pp,ee,p,e))
+        wait = []  # list of edges of the dual graph, ie p1 -- (e1,e2) --> p2
+        for e in range(len(s.polygon(p).vertices())):
+            pp, ee = s.opposite_edge(p, e)
+            wait.append((pp, ee, p, e))
         while wait:
-            p1,e1,p2,e2 = wait.pop()
+            p1, e1, p2, e2 = wait.pop()
             assert p2 in tree
-            if p1 in tree: # new cycle?
-                if (p1,e1) > (p2,e2):
+            if p1 in tree:  # new cycle?
+                if (p1, e1) > (p2, e2):
                     continue
                 polys = [p1]
                 edges = []
                 edges_rev = []
 
-                p1,e,e_back = tree[p1]
+                p1, e, e_back = tree[p1]
                 while p1 is not None:
                     edges.append(e_back)
                     edges_rev.append(e)
                     polys.append(p1)
-                    p1,e,e_back = tree[p1]
+                    p1, e, e_back = tree[p1]
                 polys.reverse()
                 edges.reverse()
                 edges_rev.reverse()
 
                 polys.append(p2)
                 edges.append(e1)
                 edges_rev.append(e2)
 
-                p2,e,e_back = tree[p2]
+                p2, e, e_back = tree[p2]
                 while p2 is not None:
                     edges.append(e)
                     edges_rev.append(e_back)
                     polys.append(p2)
-                    p2,e,e_back = tree[p2]
+                    p2, e, e_back = tree[p2]
 
                 basis.append((polys, edges, edges_rev))
 
-            else: # new branch
-                tree[p1] = (p2,e1,e2)
-                for e in range(s.polygon(p1).num_edges()):
+            else:  # new branch
+                tree[p1] = (p2, e1, e2)
+                for e in range(len(s.polygon(p1).vertices())):
                     if e != e1:
-                        pp,ee = s.opposite_edge(p1,e)
-                        wait.append((pp,ee,p1,e))
+                        pp, ee = s.opposite_edge(p1, e)
+                        wait.append((pp, ee, p1, e))
 
         basis.sort()
-        return tuple([self.element_class(self,p,e,er) for p,e,er in basis])
-
+        return tuple([self.element_class(self, p, e, er) for p, e, er in basis])
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/gl2r_orbit_closure.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/gl2r_orbit_closure.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 r"""
 GL(2,R)-orbit closure of translation surfaces
 
 .. TODO::
 
     - Theorem 1.9 of Alex Wright: the field of definition is contained in the field generated by
       the ratio of circumferences. We should provide a method, .reset_field_of_definition or
@@ -11,20 +10,20 @@
     - flow decompositions should be accessible on surfaces rather than on ``GL2ROrbitClosure``
 
 EXAMPLES:
 
 Let us first construct a Veech surface in the stratum H(2)::
 
     sage: from flatsurf import translation_surfaces
-    sage: from flatsurf import GL2ROrbitClosure # optional: pyflatsurf
+    sage: from flatsurf import GL2ROrbitClosure
 
     sage: x = polygen(QQ)
     sage: K.<a> = NumberField(x^3 - 2, embedding=AA(2)**(1/3))
     sage: S = translation_surfaces.mcmullen_L(1,1,1,a)
-    sage: O = GL2ROrbitClosure(S) # optional: pyflatsurf
+    sage: O = GL2ROrbitClosure(S) # optional: pyflatsurf  # random output due to matplotlib warnings with some combinations of setuptools and matplotlib
     sage: O.decomposition((1,2)).cylinders() # optional: pyflatsurf
     [Cylinder with perimeter [...]]
 
 The following is also a Veech surface. However the flow decomposition
 in directions with long cylinders might not discover them if a limit
 is set::
 
@@ -57,15 +56,15 @@
     sage: S = translation_surfaces.mcmullen_genus2_prototype(4,2,1,1,1/4)
     sage: O = GL2ROrbitClosure(S)  # optional: pyflatsurf
     sage: all((d.hasCylinder() == False) or d.parabolic() for d in O.decompositions(6))  # optional: pyflatsurf
     False
     sage: all((d.completelyPeriodic() == True) or (d.hasCylinder() == False) for d in O.decompositions(6))  # optional: pyflatsurf
     True
 """
-######################################################################
+# ****************************************************************************
 #  This file is part of sage-flatsurf.
 #
 #        Copyright (C) 2019-2022 Julian Rüth
 #                      2020      Vincent Delecroix
 #
 #  sage-flatsurf is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
@@ -75,17 +74,18 @@
 #  sage-flatsurf is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
-######################################################################
+# ****************************************************************************
+
+from sage.all import FreeModule, matrix, identity_matrix, ZZ, QQ, Unknown, vector, prod
 
-from sage.all import VectorSpace, FreeModule, matrix, identity_matrix, ZZ, QQ, Unknown, vector, prod
 
 class GL2ROrbitClosure:
     r"""
     Lower bound approximation to the tangent space of a GL(2,R)-orbit closure of a
     linear family of translation surfaces.
 
     EXAMPLES::
@@ -97,29 +97,30 @@
         sage: S = similarity_surfaces.billiard(T)
         sage: S = S.minimal_cover(cover_type="translation")
         sage: GL2ROrbitClosure(S)  # optional: pyflatsurf
         GL(2,R)-orbit closure of dimension at least 2 in H_5(4, 2^2) (ambient dimension 12)
 
     Computing an orbit closure over an exact real ring with transcendental elements::
 
-        sage: from flatsurf import EquiangularPolygons
-        sage: from pyexactreal import ExactReals  # optional: exactreal
+        sage: from flatsurf import Polygon, EuclideanPolygonsWithAngles
+        sage: from pyexactreal import ExactReals  # optional: exactreal  # random output due to matplotlib warnings with some combinations of setuptools and matplotlib
 
-        sage: E = EquiangularPolygons(1, 5, 5, 5)
+        sage: E = EuclideanPolygonsWithAngles((1, 5, 5, 5))
         sage: R = ExactReals(E.base_ring())  # optional: exactreal
-        sage: T = E(R(1), R.random_element(1/4))  # optional: exactreal
+        sage: slopes = E.slopes()
+        sage: T = Polygon(angles=(1, 5, 5, 5), edges=[slopes[0], R.random_element(1/4) * slopes[1]])  # optional: exactreal
         sage: S = similarity_surfaces.billiard(T)  # optional: exactreal
         sage: S = S.minimal_cover(cover_type="translation")  # optional: exactreal
-        sage: O = GL2ROrbitClosure(S); O  # optional: pyflatsurf
+        sage: O = GL2ROrbitClosure(S); O  # optional: pyflatsurf, optional: exactreal
         GL(2,R)-orbit closure of dimension at least 4 in H_7(4^3, 0) (ambient dimension 17)
         sage: bound = E.billiard_unfolding_stratum('half-translation', marked_points=True).dimension()
-        sage: for decomposition in O.decompositions(1):  # long time, optional: pyflatsurf
+        sage: for decomposition in O.decompositions(1):  # long time, optional: pyflatsurf, optional: exactreal
         ....:     O.update_tangent_space_from_flow_decomposition(decomposition)
         ....:     if O.dimension() == bound: break
-        sage: O  # long time, optional: pyflatsurf
+        sage: O  # long time, optional: pyflatsurf, optional: exactreal
         GL(2,R)-orbit closure of dimension at least 8 in H_7(4^3, 0) (ambient dimension 17)
 
     TESTS::
 
         sage: from flatsurf import translation_surfaces
         sage: x = polygen(QQ)
         sage: K = NumberField(x**3 - 2, 'a', embedding=AA(2)**QQ((1,3)))
@@ -129,36 +130,53 @@
         sage: from flatsurf import GL2ROrbitClosure  # optional: pyflatsurf
         sage: O = GL2ROrbitClosure(S) # optional: pyflatsurf
         sage: O._U.base_ring() # optional: pyflatsurf
         Number Field in a with defining polynomial x^3 - 2 with a = 1.259921049894873?
 
     We now illustrate the projection::
 
-        sage: V = O.proj._row_ambient_module() # optional: pyflatsurf
-        sage: H = O.proj._column_ambient_module() # optional: pyflatsurf
+        sage: try: # optional: pyflatsurf
+        ....:     V = O.proj.row_ambient_module()
+        ....: except AttributeError:
+        ....:     V = O.proj._row_ambient_module()
+        sage: try: # optional: pyflatsurf
+        ....:     H = O.proj.column_ambient_module()
+        ....: except AttributeError:
+        ....:     H = O.proj._column_ambient_module()
         sage: assert O.proj.rank() == H.dimension() # optional: pyflatsurf
         sage: for b in O.boundaries(): # optional: pyflatsurf
         ....:    assert (O.proj * b).is_zero()
         sage: for i, e in enumerate(O.spanning_set): # optional: pyflatsurf
         ....:     assert (O.proj * V.gen(e.index())) == H.gen(i)
     """
+
     def __init__(self, surface):
-        from flatsurf.geometry.translation_surface import TranslationSurface
-        if isinstance(surface, TranslationSurface):
+        from flatsurf.geometry.categories import TranslationSurfaces
+        from flatsurf.geometry.surface import Surface_base
+
+        if isinstance(surface, Surface_base):
+            if surface not in TranslationSurfaces():
+                raise NotImplementedError(
+                    "cannot compute orbit closure of a non-translation surface"
+                )
+
             base_ring = surface.base_ring()
             from flatsurf.geometry.pyflatsurf_conversion import to_pyflatsurf
+
             self._surface = to_pyflatsurf(surface)
         else:
             from flatsurf.geometry.pyflatsurf_conversion import sage_ring
+
             base_ring = sage_ring(surface)
             self._surface = surface
 
         # A model of the vector space R² in libflatsurf, e.g., to represent the
         # vector associated to a saddle connection.
         from flatsurf.features import pyflatsurf_feature
+
         pyflatsurf_feature.require()
         import pyflatsurf.vector
 
         self.V2 = pyflatsurf.vector.Vectors(base_ring)
 
         # We construct a spanning set of edges, that is a subset of the
         # edges that form a basis of H_1(S, Sigma; Z)
@@ -167,15 +185,15 @@
         assert set(t.keys()) == set(f[2] for f in self._surface.faces())
         self.spanning_set = []
         v = set(t.values())
         for e in self._surface.edges():
             if e.positive() not in v and e.negative() not in v:
                 self.spanning_set.append(e)
         self.d = len(self.spanning_set)
-        assert 3*self.d - 3 == self._surface.size()
+        assert 3 * self.d - 3 == self._surface.size()
         assert m.rank() == self.d
         m = m.transpose()
         # projection matrix from Z^E to H_1(S, Sigma; Z) in the basis
         # of spanning edges
         self.proj = matrix(ZZ, [r for r in m.rows() if not r.is_zero()])
 
         self.Omega = self._intersection_matrix(t, self.spanning_set)
@@ -201,28 +219,32 @@
         self._U_rank = 0
 
         self.update_tangent_space_from_vector(self.H.transpose()[0])
         self.update_tangent_space_from_vector(self.H.transpose()[1])
 
     def dimension(self):
         r"""
-        Return the current real dimension of the GL(2,R)-orbit closure.
+        Return the current complex dimension of the GL(2,R)-orbit closure.
+
+        Note that this is not the dimension of the orbit closure but only a
+        lower bound. It is always at least 2 (coming from a GL(2,R)-orbit).
+        The current tangent space could be refined via
+        :meth:`update_tangent_space_from_flow_decomposition`.
 
         EXAMPLES::
 
-            sage: from flatsurf import EquiangularPolygons, similarity_surfaces
+            sage: from flatsurf import Polygon, similarity_surfaces
             sage: from flatsurf import GL2ROrbitClosure # optional: pyflatsurf
-            sage: E = EquiangularPolygons(1, 3, 5)
-            sage: T = E(1)
+            sage: T = Polygon(angles=(1, 3, 5))
             sage: S = similarity_surfaces.billiard(T)
             sage: S = S.minimal_cover(cover_type="translation")
             sage: O = GL2ROrbitClosure(S) # optional: pyflatsurf
             sage: O.dimension() # optional: pyflatsurf
             2
-            sage: bound = E.billiard_unfolding_stratum('half-translation', marked_points=True).dimension()
+            sage: bound = T.category().billiard_unfolding_stratum('half-translation', marked_points=True).dimension()
             sage: for decomposition in O.decompositions(1):  # long time, optional: pyflatsurf
             ....:     if O.dimension() == bound: break
             ....:     O.update_tangent_space_from_flow_decomposition(decomposition)
             ....:     print(O.dimension())
             3
             5
             5
@@ -234,28 +256,28 @@
 
     def ambient_stratum(self):
         r"""
         Return the stratum of Abelian differentials this surface belongs to.
 
         EXAMPLES::
 
-            sage: from flatsurf import EquiangularPolygons, similarity_surfaces
+            sage: from flatsurf import Polygon, similarity_surfaces
             sage: from flatsurf import GL2ROrbitClosure # optional: pyflatsurf
-            sage: E = EquiangularPolygons(1, 3, 5)
-            sage: T = E(1)
+            sage: T = Polygon(angles=(1, 3, 5))
             sage: S = similarity_surfaces.billiard(T)
             sage: S = S.minimal_cover(cover_type="translation")
             sage: O = GL2ROrbitClosure(S) # optional: pyflatsurf
             sage: O.ambient_stratum() # optional: pyflatsurf
             H_3(4, 0^4)
         """
         from surface_dynamics import AbelianStratum
+
         surface = self._surface
         angles = [surface.angle(v) for v in surface.vertices()]
-        return AbelianStratum([a-1 for a in angles])
+        return AbelianStratum([a - 1 for a in angles])
 
     def base_ring(self):
         r"""
         Return the underlying base ring
         """
         return self._U.base_ring()
 
@@ -267,66 +289,70 @@
 
             This involves the computation of the echelon form of the matrix. It
             might be rather expensive if the computation of the tangent space is
             not terminated.
 
         EXAMPLES::
 
-            sage: from flatsurf import polygons, similarity_surfaces, EquiangularPolygons
+            sage: from flatsurf import Polygon, similarity_surfaces, EuclideanPolygonsWithAngles
             sage: from flatsurf import GL2ROrbitClosure  # optional: pyflatsurf
             sage: from pyexactreal import ExactReals  # optional: exactreal
-            sage: E = EquiangularPolygons(1, 5, 5, 5)
+            sage: E = EuclideanPolygonsWithAngles((1, 5, 5, 5))
             sage: R = ExactReals(E.base_ring())  # optional: exactreal
-            sage: T = E(R(1), R.random_element(1/4))  # optional: exactreal
+            sage: slopes = E.slopes()
+            sage: T = Polygon(angles=(1, 5, 5, 5), edges=[slopes[0], R.random_element(1/4) * slopes[1]])  # optional: exactreal
             sage: S = similarity_surfaces.billiard(T)  # optional: exactreal
             sage: S = S.minimal_cover(cover_type="translation")  # optional: exactreal
-            sage: O = GL2ROrbitClosure(S); O  # optional: pyflatsurf
+            sage: O = GL2ROrbitClosure(S); O  # optional: pyflatsurf, optional: exactreal
             GL(2,R)-orbit closure of dimension at least 4 in H_7(4^3, 0) (ambient dimension 17)
-            sage: O.field_of_definition() # optional: pyflatsurf
+            sage: O.field_of_definition() # optional: pyflatsurf, optional: exactreal
             Number Field in c0 with defining polynomial x^2 - 2 with c0 = 1.414213562373095?
             sage: bound = E.billiard_unfolding_stratum('half-translation', marked_points=True).dimension()
-            sage: for decomposition in O.decompositions(1):  # long time, optional: pyflatsurf
+            sage: for decomposition in O.decompositions(1):  # long time, optional: pyflatsurf, optional: exactreal
             ....:     if O.dimension() == bound: break
             ....:     O.update_tangent_space_from_flow_decomposition(decomposition)
-            sage: O.field_of_definition()  # long time, optional: pyflatsurf
+            sage: O.field_of_definition()  # long time, optional: pyflatsurf, optional: exactreal
             Rational Field
 
-            sage: E = EquiangularPolygons(1, 3, 5)
-            sage: T = E(1)
+            sage: T = Polygon(angles=(1, 3, 5))
             sage: S = similarity_surfaces.billiard(T)
             sage: S = S.minimal_cover(cover_type="translation")
             sage: O = GL2ROrbitClosure(S) # optional: pyflatsurf
             sage: O.field_of_definition() # optional: pyflatsurf
             Number Field in c0 with defining polynomial x^3 - 3*x - 1 with c0 = 1.879385241571817?
-            sage: bound = E.billiard_unfolding_stratum('half-translation', marked_points=True).dimension()
+            sage: bound = T.category().billiard_unfolding_stratum('half-translation', marked_points=True).dimension()
             sage: for decomposition in O.decompositions(1):  # long time, optional: pyflatsurf
             ....:     if O.dimension() == bound: break
             ....:     O.update_tangent_space_from_flow_decomposition(decomposition)
             sage: O.field_of_definition()  # long time, optional: pyflatsurf
             Rational Field
         """
         M = self._U.echelon_form()
 
         from flatsurf.geometry.subfield import subfield_from_elements
-        L, elts, phi = subfield_from_elements(M.base_ring(), M[:self._U_rank].list())
+
+        L, elts, phi = subfield_from_elements(M.base_ring(), M[: self._U_rank].list())
 
         return L
 
     def _half_edge_to_face(self, h):
         r"""
         Return a canonical half-edge encoding the face bounded by ``h``.
         """
         surface = self._surface
         h1 = h
         h2 = surface.nextInFace(h1)
         h3 = surface.nextInFace(h2)
         return min([h1, h2, h3], key=lambda x: x.index())
 
     def __repr__(self):
-        return "GL(2,R)-orbit closure of dimension at least %d in %s (ambient dimension %d)" % (self._U_rank, self.ambient_stratum(), self.d)
+        return (
+            "GL(2,R)-orbit closure of dimension at least %d in %s (ambient dimension %d)"
+            % (self._U_rank, self.ambient_stratum(), self.d)
+        )
 
     def holonomy(self, v):
         r"""
         Return the holonomy of ``v`` (with respect to the chosen homology basis)
 
         EXAMPLES::
 
@@ -346,15 +372,15 @@
     def holonomy_dual(self, v):
         r"""
         Return the holonomy of the dual of ``v``
         """
         return self.V(v) * self.Hdual
 
     def tangent_space_basis(self):
-        return self._U[:self._U_rank].rows()
+        return self._U[: self._U_rank].rows()
 
     def lift(self, v):
         r"""
         Given a vector in the "spanning set basis" return a vector on the full basis of
         edges.
 
         EXAMPLES::
@@ -366,16 +392,16 @@
             sage: O = GL2ROrbitClosure(S)  # optional: pyflatsurf
             sage: u0,u1 = O.tangent_space_basis()  # optional: pyflatsurf
             sage: v0 = O.lift(u0)  # optional: pyflatsurf
             sage: v1 = O.lift(u1)  # optional: pyflatsurf
             sage: span([v0, v1])  # optional: pyflatsurf
             Vector space of degree 9 and dimension 2 over Real Embedded Number Field in l with defining polynomial x^2 - x - 8 with l = 3.372281323269015?
             Basis matrix:
-            [                         1                          0                         -1   (1/4*l-1/4 ~ 0.59307033) (-1/4*l+1/4 ~ -0.59307033)                          0 (-1/4*l+1/4 ~ -0.59307033)                          0 (-1/4*l+1/4 ~ -0.59307033)]
-            [                         0                          1                         -1    (1/8*l+7/8 ~ 1.2965352) (-1/8*l+1/8 ~ -0.29653517)                         -1 (3/8*l-11/8 ~ -0.11039450) (-1/2*l+3/2 ~ -0.18614066) (-1/8*l+1/8 ~ -0.29653517)]
+            [                         1                          0                         -1                          0   (1/4*l-1/4 ~ 0.59307033) (-1/4*l+1/4 ~ -0.59307033)   (1/4*l-1/4 ~ 0.59307033) (-1/4*l+1/4 ~ -0.59307033)                          0]
+            [                         0                          1                         -1                         -1    (1/8*l+7/8 ~ 1.2965352) (-1/8*l+1/8 ~ -0.29653517)   (1/8*l-1/8 ~ 0.29653517) (3/8*l-11/8 ~ -0.11039450) (-1/2*l+3/2 ~ -0.18614066)]
 
         This can be used to deform the surface::
 
             sage: T = polygons.triangle(3,4,13)
             sage: S = similarity_surfaces.billiard(T)
             sage: S = S.minimal_cover("translation").erase_marked_points() # long time (3s, #122), optional: pyflatsurf
             sage: O = GL2ROrbitClosure(S)  # long time (above), optional: pyflatsurf
@@ -396,42 +422,54 @@
         """
         # given the values on the spanning edges we reconstruct the unique vector that
         # vanishes on the boundary
         bdry = self.boundaries()
         n = self._surface.edges().size()
         k = len(self.spanning_set)
         assert k + len(bdry) == n + 1
-        A = matrix(QQ, n+1, n)
-        for i,e in enumerate(self.spanning_set):
-            A[i,e.index()] = 1
-        for i,b in enumerate(bdry):
-            A[k+i,:] = b
+        A = matrix(QQ, n + 1, n)
+        for i, e in enumerate(self.spanning_set):
+            A[i, e.index()] = 1
+        for i, b in enumerate(bdry):
+            A[k + i, :] = b
         u = vector(self.V2.base_ring(), n + 1)
         u[:k] = v
         from sage.all import Fields
+
         if not self.V2.base_ring() in Fields():
             assert all(uu._backend.coefficients().size() == 1 for uu in u)
-            u = u.parent().change_ring(self.V2.base_ring().base_ring())([uu._backend.coefficients()[0] for uu in u])
+            u = u.parent().change_ring(self.V2.base_ring().base_ring())(
+                [uu._backend.coefficients()[0] for uu in u]
+            )
         return A.solve_right(u)
 
     def absolute_homology(self):
-        vert_index = {v:i for i,v in enumerate(self._surface.vertices())}
+        vert_index = {v: i for i, v in enumerate(self._surface.vertices())}
         m = len(vert_index)
         if m == 1:
             return self.V
         rows = []
 
         from flatsurf.features import pyflatsurf_feature
+
         pyflatsurf_feature.require()
         import pyflatsurf
 
         for e in self.spanning_set:
             r = [0] * m
-            i = vert_index[pyflatsurf.flatsurf.Vertex.target(e.positive(), self._surface.combinatorial())]
-            j = vert_index[pyflatsurf.flatsurf.Vertex.source(e.positive(), self._surface.combinatorial())]
+            i = vert_index[
+                pyflatsurf.flatsurf.Vertex.target(
+                    e.positive(), self._surface.combinatorial()
+                )
+            ]
+            j = vert_index[
+                pyflatsurf.flatsurf.Vertex.source(
+                    e.positive(), self._surface.combinatorial()
+                )
+            ]
             if i != j:
                 r[i] = 1
                 r[j] = -1
             rows.append(r)
         return matrix(rows).left_kernel()
 
     def absolute_dimension(self):
@@ -458,21 +496,23 @@
             sage: for d in O.decompositions(5, 100):  # long time (3s) optional: pyflatsurf
             ....:     O.update_tangent_space_from_flow_decomposition(d)
             ....:     if O.dimension() == 9:
             ....:         break
             sage: O.absolute_dimension()  # long time (above), optional: pyflatsurf
             6
         """
-        return (self.absolute_homology().matrix() * self._U[:self._U_rank].transpose()).rank()
+        return (
+            self.absolute_homology().matrix() * self._U[: self._U_rank].transpose()
+        ).rank()
 
     def _spanning_tree(self, root=None):
         r"""
         Return a pair ``(tree, proj)`` where
 
-        - ``tree`` is a tree encoded in a dictionnary. Its keys are the faces
+        - ``tree`` is a tree encoded in a dictionary. Its keys are the faces
           (coded by their minimal adjacent half-edge) and the corresponding
           value is the half-edge to cross to go toward the root face.
 
         - ``proj`` a projection matrix : for a vector ``v``, the vector
           ``v * proj`` is cohomologous to ``v`` and only takes values on the
           spanning set.
 
@@ -509,15 +549,15 @@
             ....:     else:
             ....:         assert (proj * v).is_zero()
         """
         if root is None:
             root = next(iter(self._surface.edges())).positive()
 
         root = self._half_edge_to_face(root)
-        t = {root: None} # face -> half edge to take to go to the root
+        t = {root: None}  # face -> half edge to take to go to the root
         todo = [root]
         edges = []  # store edges in topological order to perform Gauss reduction
         while todo:
             f = todo.pop()
             for _ in range(3):
                 f1 = -f
                 g = self._half_edge_to_face(f1)
@@ -529,46 +569,45 @@
                 f = self._surface.nextInFace(f)
 
         # gauss reduction
         n = self._surface.size()
         proj = identity_matrix(ZZ, n)
         edges.reverse()
         for f1 in edges:
-            v = [0] * n
             f2 = self._surface.nextInFace(f1)
             f3 = self._surface.nextInFace(f2)
             assert self._surface.nextInFace(f3) == f1
 
             i1 = f1.index()
-            s1 = -1 if i1%2 else 1
+            s1 = -1 if i1 % 2 else 1
             i2 = f2.index()
-            s2 = -1 if i2%2 else 1
+            s2 = -1 if i2 % 2 else 1
             i3 = f3.index()
-            s3 = -1 if i3%2 else 1
+            s3 = -1 if i3 % 2 else 1
             i1 = f1.edge().index()
             i2 = f2.edge().index()
             i3 = f3.edge().index()
-            proj[i1] = -s1*(s2*proj[i2] + s3*proj[i3])
+            proj[i1] = -s1 * (s2 * proj[i2] + s3 * proj[i3])
             for j in range(n):
-                assert proj[j,i1] == 0
+                assert proj[j, i1] == 0
 
         return (t, proj)
 
     def _intersection_matrix(self, t, spanning_set):
         r"""
         Given a spanning tree, compute the associated intersection matrix.
 
         It can be used to compute holonomies. (we can be off by a - sign)
         """
         d = len(spanning_set)
         h = spanning_set[0].positive()
         all_edges = set([e.positive() for e in spanning_set])
         all_edges.update([e.negative() for e in spanning_set])
         contour = []
-        contour_inv = {}   # half edge -> position in contour
+        contour_inv = {}  # half edge -> position in contour
         while h not in contour_inv:
             contour_inv[h] = len(contour)
             contour.append(h)
             h = self._surface.nextAtVertex(-h)
             while h not in all_edges:
                 h = self._surface.nextAtVertex(h)
 
@@ -582,42 +621,45 @@
             pi1 = contour_inv[ei.positive()]
             pi2 = contour_inv[ei.negative()]
             if pi1 > pi2:
                 si = -1
                 pi1, pi2 = pi2, pi1
             else:
                 si = 1
-            for j in range(i+1, len(spanning_set)):
+            for j in range(i + 1, len(spanning_set)):
                 ej = spanning_set[j]
                 pj1 = contour_inv[ej.positive()]
                 pj2 = contour_inv[ej.negative()]
                 if pj1 > pj2:
                     sj = -1
                     pj1, pj2 = pj2, pj1
                 else:
                     sj = 1
 
                 # pj1 pj2 pi1 pi2: pj2 < pi1
                 # pi1 pi2 pj1 pj2: pi2 < pj1
                 # pi1 pj1 pj2 pi2: pi1 < pj1 and pj2 < pi2
                 # pj1 pi1 pi2 pj2: pj1 < pi1 and pi2 < pj2
-                if (pj2 < pi1) or (pi2 < pj1) or \
-                   (pj1 > pi1 and pj2 < pi2) or \
-                   (pj1 < pi1 and pj2 > pi2):
+                if (
+                    (pj2 < pi1)
+                    or (pi2 < pj1)
+                    or (pj1 > pi1 and pj2 < pi2)
+                    or (pj1 < pi1 and pj2 > pi2)
+                ):
                     # no intersection
                     continue
 
                 if pi1 < pj1 < pi2:
                     # one sign
-                    Omega[i,j] = si * sj
+                    Omega[i, j] = si * sj
                 else:
                     # other sign
                     assert pi1 < pj2 < pi2, (pi1, pi2, pj1, pj2)
-                    Omega[i,j] = -si*sj
-                Omega[j,i] = - Omega[i,j]
+                    Omega[i, j] = -si * sj
+                Omega[j, i] = -Omega[i, j]
         return Omega
 
     def boundaries(self):
         r"""
         Return the list of boundaries (ie sum of edges around a triangular face).
 
         These are elements of H_1(S, Sigma; Z).
@@ -639,21 +681,21 @@
             ....:             O = GL2ROrbitClosure(S)
             ....:             for b in O.boundaries():
             ....:                 assert (O.proj * b).is_zero()
         """
         n = self._surface.size()
         V = FreeModule(ZZ, n)
         B = []
-        for (f1,f2,f3) in self._surface.faces():
+        for f1, f2, f3 in self._surface.faces():
             i1 = f1.index()
-            s1 = -1 if i1%2 else 1
+            s1 = -1 if i1 % 2 else 1
             i2 = f2.index()
-            s2 = -1 if i2%2 else 1
+            s2 = -1 if i2 % 2 else 1
             i3 = f3.index()
-            s3 = -1 if i3%2 else 1
+            s3 = -1 if i3 % 2 else 1
             i1 = f1.edge().index()
             i2 = f2.edge().index()
             i3 = f3.edge().index()
             v = [0] * n
             v[i1] = 1
             v[i2] = s1 * s2
             v[i3] = s1 * s3
@@ -662,41 +704,46 @@
 
         return B
 
     def decomposition(self, v, limit=-1):
         v = self.V2(v)
 
         from flatsurf.features import pyflatsurf_feature
+
         pyflatsurf_feature.require()
         import pyflatsurf
 
-        decomposition = pyflatsurf.flatsurf.makeFlowDecomposition(self._surface, v.vector)
+        decomposition = pyflatsurf.flatsurf.makeFlowDecomposition(
+            self._surface, v.vector
+        )
 
-        u = self.V2._isomorphic_vector_space(v)
         if limit != 0:
             decomposition.decompose(int(limit))
         return decomposition
 
     def decompositions(self, bound, limit=-1, bfs=False):
         limit = int(limit)
 
         connections = self._surface.connections().bound(int(bound))
         if bfs:
             connections = connections.byLength()
 
         slopes = None
 
         from flatsurf.features import cppyy_feature
+
         cppyy_feature.require()
         import cppyy
 
         for connection in connections:
             direction = connection.vector()
             if slopes is None:
-                slopes = cppyy.gbl.std.set[type(direction), type(direction).CompareSlope]()
+                slopes = cppyy.gbl.std.set[
+                    type(direction), type(direction).CompareSlope
+                ]()
             if slopes.find(direction) != slopes.end():
                 continue
             slopes.insert(direction)
             yield self.decomposition(direction, limit)
 
     def decompositions_depth_first(self, bound, limit=-1):
         return self.decompositions(bound, bfs=False, limit=limit)
@@ -749,27 +796,29 @@
         ne = len(self._surface.edges())
         nf = len(self._surface.faces())
         genus = (ne - nv - nf) // 2 + 1
         if k.degree() > genus or not k.is_totally_real():
             return False
 
         for decomposition in self.decompositions_depth_first(bound, limit):
-            if decomposition.parabolic() == False:
+            if (
+                decomposition.parabolic() == False
+            ):  # noqa, we are comparing to a boost tribool so this cannot be replaced by "is False"
                 return False
 
         return Unknown
 
     def cylinder_circumference(self, component, A, sc_index, proj):
         r"""
-        Return the circumference of the cylindre ``component`` in the homology
+        Return the circumference of the cylinder ``component`` in the homology
         of the underlying surface.
 
         INPUT:
 
-        - ``component`` - a cylinder
+        - ``component`` -- a cylinder
 
         - ``A``, ``sc_index``, ``proj`` -- the output of
           ``flow_decomposition_kontsevich_zorich_cocycle``
 
         EXAMPLES::
 
             sage: from flatsurf import translation_surfaces
@@ -778,29 +827,31 @@
             sage: S = translation_surfaces.veech_double_n_gon(5)
             sage: O = GL2ROrbitClosure(S)  # optional: pyflatsurf
             sage: for dec in O.decompositions_depth_first(1):  # optional: pyflatsurf
             ....:     break
             sage: c0, c1 = dec.components() # optional: pyflatsurf
             sage: kz = O.flow_decomposition_kontsevich_zorich_cocycle(dec) # optional: pyflatsurf
             sage: O.cylinder_circumference(c0, *kz) # optional: pyflatsurf
-            (1, 0, 0, -1)
+            (1, 0, -1, 0)
             sage: O.cylinder_circumference(c1, *kz) # optional: pyflatsurf
-            (0, 0, -1, 0)
+            (0, 0, 0, -1)
         """
-        if component.cylinder() != True:
+        if (
+            component.cylinder() != True
+        ):  # noqa, we are comparing to a boost tribool so this cannot be replaced by "is not True"
             raise ValueError
 
-        perimeters = [p for p in component.perimeter()]
+        perimeters = list(component.perimeter())
         per = perimeters[0]
         assert not per.vertical()
         sc = per.saddleConnection()
         i = sc_index[sc]
         if i < 0:
             s = -1
-            i = -i-1
+            i = -i - 1
         else:
             s = 1
         v = s * proj.column(i)
         circumference = -A.solve_right(v)
 
         # check
         hol = self.holonomy_dual(circumference)
@@ -813,88 +864,131 @@
     def cylinder_deformation_subspace(self, decomposition):
         r"""
         Return a subspace included in the tangent space to the GL(2,R)-orbit
         closure computed from the flow decomposition ``decomposition``.
 
         From A. Wright cylinder deformation Theorem.
         """
+
         def eliminate_denominators(fractions):
             r"""
             Given a list of ``fractions``, pairs of numerators `n_i` and
             denominators `d_i`, return a list of fractions `c n_i/d_i` scaled
             uniformly such that the value can be represented in the underlying
             ring.
             """
             fractions = list(fractions)
             try:
                 return [x.parent()(x / y) for x, y in fractions]
             except (ValueError, ArithmeticError, NotImplementedError):
-                denominators = set([denominator for numerator, denominator in fractions])
-                return [numerator * prod(
-                    [d for d in denominators if denominator != d]
-                ) for (numerator, denominator) in fractions]
+                denominators = set(
+                    [denominator for numerator, denominator in fractions]
+                )
+                return [
+                    numerator * prod([d for d in denominators if denominator != d])
+                    for (numerator, denominator) in fractions
+                ]
 
-        v = self.V()
         module_fractions = []
         vcyls = []
         kz = self.flow_decomposition_kontsevich_zorich_cocycle(decomposition)
         for component in decomposition.components():
-            if component.cylinder() == False:
+            if (
+                component.cylinder() == False
+            ):  # noqa, we are comparing to a boost tribool so this cannot be replaced by "is False"
                 continue
-            elif component.cylinder() == True:
+            elif (
+                component.cylinder() == True
+            ):  # noqa, we are comparing to a boost tribool so this cannot be replaced with "is True"
                 vcyls.append(self.cylinder_circumference(component, *kz))
 
-                vertical = component.vertical()
-                width = self.V2._isomorphic_vector_space.base_ring()(self.V2.base_ring()(component.width()))
-                height = self.V2._isomorphic_vector_space.base_ring()(self.V2.base_ring()(component.vertical().project(component.circumferenceHolonomy())))
+                width = self.V2._isomorphic_vector_space.base_ring()(
+                    self.V2.base_ring()(component.width())
+                )
+                height = self.V2._isomorphic_vector_space.base_ring()(
+                    self.V2.base_ring()(
+                        component.vertical().project(component.circumferenceHolonomy())
+                    )
+                )
                 module_fractions.append((width, height))
             else:
                 return []
 
         if not module_fractions:
             return []
 
         modules = eliminate_denominators(module_fractions)
 
-        if hasattr(modules[0], '_backend'):
+        if hasattr(modules[0], "_backend"):
             # Make sure all modules live in the same K-Module so that .coefficients() below produces coefficient lists of the same length.
             from functools import reduce
-            parent = reduce(lambda m, n: m.span(m, n), [module._backend.module() for module in modules], modules[0]._backend.module())
-            modules = [module.parent()(module._backend.promote(parent)) for module in modules]
+
+            parent = reduce(
+                lambda m, n: m.span(m, n),
+                [module._backend.module() for module in modules],
+                modules[0]._backend.module(),
+            )
+            modules = [
+                module.parent()(module._backend.promote(parent)) for module in modules
+            ]
 
         def to_rational_vector(x):
             r"""
             Return the rational coefficients of `x` over its implicit basis,
             e.g., if `x` is in a number field K, return the coefficients of x
             in `K` as a vector space over the rationals.
             """
             if x.parent() in [ZZ, QQ]:
                 ret = [QQ(x)]
-            elif hasattr(x, 'vector'):
+            elif hasattr(x, "vector"):
                 ret = x.vector()
-            elif hasattr(x, 'renf_elem'):
+            elif hasattr(x, "renf_elem"):
                 ret = x.parent().number_field(x).vector()
-            elif hasattr(x, '_backend'):
+            elif hasattr(x, "_backend"):
                 from itertools import chain
-                ret = list(chain(*[to_rational_vector(self.V2.base_ring().base_ring()(self.V2.base_ring().base_ring()(c))) for c in x._backend.coefficients()]))
+
+                ret = list(
+                    chain(
+                        *[
+                            to_rational_vector(
+                                self.V2.base_ring().base_ring()(
+                                    self.V2.base_ring().base_ring()(c)
+                                )
+                            )
+                            for c in x._backend.coefficients()
+                        ]
+                    )
+                )
             else:
-                raise NotImplementedError("cannot turn %s, i.e., a %s, into a rational vector yet"%(x,type(x)))
+                raise NotImplementedError(
+                    "cannot turn %s, i.e., a %s, into a rational vector yet"
+                    % (x, type(x))
+                )
 
             assert all(y in QQ for y in ret)
             return ret
 
         assert all(module.parent() is modules[0].parent() for module in modules)
         M = matrix([to_rational_vector(module) for module in modules])
         assert M.base_ring() is QQ
         relations = self._left_kernel_matrix(M)
         assert len(vcyls) == len(module_fractions) == relations.ncols()
 
-        vectors = [sum(t * vcyl * module[1] for (t, vcyl, module) in zip(relation, vcyls, module_fractions)) for relation in self._right_kernel_matrix(relations).rows()]
-
-        assert all(v.base_ring() is self.V2._isomorphic_vector_space.base_ring() for v in vectors)
+        vectors = [
+            sum(
+                t * vcyl * module[1]
+                for (t, vcyl, module) in zip(relation, vcyls, module_fractions)
+            )
+            for relation in self._right_kernel_matrix(relations).rows()
+        ]
+
+        assert all(
+            v.base_ring() is self.V2._isomorphic_vector_space.base_ring()
+            for v in vectors
+        )
 
         return vectors
 
     def _flow_decomposition_spanning_tree(self, decomposition, sc_index, sc_comp):
         r"""
         Helper for :meth:`flow_decomposition_kontsevich_zorich_cocycle`.
 
@@ -911,24 +1005,23 @@
           boundary of ``decomposition`` and the corresponding values are the indices
           used in the matrix
 
         - ``sc_comp`` -- a dictionary whose keys are the saddle connections on the
           boundary of ``decomposition`` and the corresponding values are the indices
           of the components of ``decomposition``
         """
-        components = [c for c in decomposition.components()]
+        components = list(decomposition.components())
 
         n = len(sc_index)
         assert n % 2 == 0
         n //= 2
 
         for p in components[0].perimeter():
             break
-        root = p.saddleConnection()
-        t = {0: None} # face -> half edge to take to go to the root
+        t = {0: None}  # face -> half edge to take to go to the root
         todo = [0]
         edges = []  # store edges in topological order to perform Gauss reduction
         while todo:
             i = todo.pop()
             c = components[i]
             for sc in c.perimeter():
                 sc1 = -sc.saddleConnection()
@@ -942,34 +1035,34 @@
         spanning_set = set(range(n))
         proj = identity_matrix(ZZ, n)
         edges.reverse()
         for sc1 in edges:
             i1 = sc_index[sc1]
             if i1 < 0:
                 s1 = -1
-                i1 = -i1-1
+                i1 = -i1 - 1
             else:
                 s1 = 1
             comp = components[sc_comp[sc1]]
             proj[i1] = 0
             for p in comp.perimeter():
                 sc = p.saddleConnection()
                 if sc == sc1:
                     continue
                 j = sc_index[sc]
                 if j < 0:
                     s = -1
-                    j = -j-1
+                    j = -j - 1
                 else:
                     s = 1
-                proj[i1] = - s1 * s * proj[j]
+                proj[i1] = -s1 * s * proj[j]
 
             spanning_set.remove(i1)
             for j in range(n):
-                assert proj[j,i1] == 0
+                assert proj[j, i1] == 0
 
         return (t, sorted(spanning_set), proj)
 
     def flow_decomposition_kontsevich_zorich_cocycle(self, decomposition):
         r"""
         Base change from the homology of ``decomposition`` to the underlying surface.
 
@@ -1009,43 +1102,47 @@
             [ 1  0]
             [-1  1]
             [ 1 -1]
             [-1  2]
             [ 1  0]
             [-2  1]
         """
-        sc_pos = []   # list of positive boundary saddle connections
-                      # (store only one orientation for each)
-        sc_index = {} # inverse of sc_pos (and also reverse orientation with negative index)
+        sc_pos = (
+            []
+        )  # list of positive boundary saddle connections (store only one orientation for each)
+        sc_index = (
+            {}
+        )  # inverse of sc_pos (and also reverse orientation with negative index)
         sc_comp = {}
         n_saddles = 0
         components = list(decomposition.components())
         n_components = len(components)
-        for i,comp in enumerate(components):
+        for i, comp in enumerate(components):
             for p in comp.perimeter():
                 sc = p.saddleConnection()
                 sc_comp[sc] = i
                 if sc not in sc_index:
                     sc_index[sc] = n_saddles
                     sc_pos.append(sc)
-                    sc_index[-sc] = -n_saddles-1
+                    sc_index[-sc] = -n_saddles - 1
                     n_saddles += 1
 
-        t, spanning_set, proj = self._flow_decomposition_spanning_tree(decomposition, sc_index, sc_comp)
+        t, spanning_set, proj = self._flow_decomposition_spanning_tree(
+            decomposition, sc_index, sc_comp
+        )
         assert proj.rank() == len(spanning_set) == n_saddles - n_components + 1
         proj = proj.transpose()
         proj = matrix(ZZ, [r for r in proj.rows() if not r.is_zero()])
         assert proj.nrows() == self.proj.nrows()
 
         # Write the base change V^*(T') -> V^*(T) relative to our bases
         A = matrix(ZZ, self.d)
         for i, sc in enumerate(spanning_set):
             sc = sc_pos[sc]
             c = sc.chain()
-            v = [0] * self.d
             for edge in self._surface.edges():
                 A[i] += ZZ(str(c[edge])) * self.proj.column(edge.index())
         assert A.det().is_unit()
         return A, sc_index, proj
 
     def update_tangent_space_from_flow_decomposition(self, decomposition):
         r"""
@@ -1087,35 +1184,40 @@
             (3, 2, 2): 5
             (4, 2, 1): 4
             (4, 4, 3): 4
             (5, 3, 3): 4
             (5, 4, 4): 7
             (5, 5, 3): 4
         """
-        if self._U_rank == self._U.nrows(): return
+        if self._U_rank == self._U.nrows():
+            return
         for v in self.cylinder_deformation_subspace(decomposition):
             self.update_tangent_space_from_vector(v)
-            if self._U_rank == self._U.nrows(): return
+            if self._U_rank == self._U.nrows():
+                return
 
     def _rank(self):
         r"""
         Return a lower bound for the rank of the matrix _U.
         """
         while True:
             if self._p is not None:
                 try:
-                    self._Ubar = self._U.apply_map(phi=self._p.reduce, R=self._p.residue_field())
+                    self._Ubar = self._U.apply_map(
+                        phi=self._p.reduce, R=self._p.residue_field()
+                    )
                     break
                 except ValueError:
                     # The matrix _U cannot be reduced mod p because some entries have negative valuation.
                     pass
 
             p = 2**30 if self._p is None else self._p.p()
-            
+
             from sage.all import next_prime
+
             self._p = ZZ.valuation(next_prime(p)).extensions(self._U.base_ring())[0]
 
         return self._Ubar.rank()
 
     def update_tangent_space_from_vector(self, v):
         if self._U_rank == self._U.nrows():
             return
@@ -1144,15 +1246,15 @@
             sage: from flatsurf import GL2ROrbitClosure  # optional: pyflatsurf
 
             sage: T = polygons.triangle(1, 2, 5)
             sage: S = similarity_surfaces.billiard(T)
             sage: S = S.minimal_cover(cover_type="translation")
             sage: GL2ROrbitClosure(S) == GL2ROrbitClosure(S) # optional: pyflatsurf
             True
-            
+
         """
         return self._surface == other._surface
 
     def __ne__(self, other):
         r"""
         Return whether ``other`` was not built starting from the same surface
         than this orbit closure.
@@ -1163,15 +1265,15 @@
             sage: from flatsurf import GL2ROrbitClosure  # optional: pyflatsurf
 
             sage: T = polygons.triangle(1, 2, 5)
             sage: S = similarity_surfaces.billiard(T)
             sage: S = S.minimal_cover(cover_type="translation")
             sage: GL2ROrbitClosure(S) != GL2ROrbitClosure(S) # optional: pyflatsurf
             False
-            
+
         """
         return not (self == other)
 
     def __hash__(self):
         r"""
         Return a hash value of this object compatible with equality operators.
 
@@ -1201,18 +1303,20 @@
 
             sage: T = polygons.triangle(1, 2, 5)
             sage: S = similarity_surfaces.billiard(T)
             sage: S = S.minimal_cover(cover_type="translation")
             sage: O = GL2ROrbitClosure(S)  # optional: pyflatsurf
             sage: loads(dumps(O)) == O  # long time (6s, #123)
             True
-
         """
-        from flatsurf.geometry.pyflatsurf_conversion import from_pyflatsurf
-        return (GL2ROrbitClosure, (self._surface,), {'_U': self._U, '_U_rank': self._U_rank})
+        return (
+            GL2ROrbitClosure,
+            (self._surface,),
+            {"_U": self._U, "_U_rank": self._U_rank},
+        )
 
     @classmethod
     def _right_kernel_matrix(cls, M):
         r"""
         Compute the right kernel of the rational matrix `M`.
 
         See https://github.com/flatsurf/sage-flatsurf/issues/100.
@@ -1227,25 +1331,25 @@
             return M.new_matrix(nrows=0, ncols=M.ncols())
         if M.nrows() == 0:
             return M.matrix_space(M.ncols(), M.ncols()).identity_matrix()
 
         height = M.height()
 
         if height >= 2**256:
-            algorithm = 'flint'
+            algorithm = "flint"
         elif columns >= 64 and rows >= 64:
-            algorithm = 'padic'
+            algorithm = "padic"
         elif rows * columns <= 32:
-            algorithm = 'flint'
+            algorithm = "flint"
         else:
-            algorithm = 'pari'
+            algorithm = "pari"
 
-        if algorithm == 'pari':
+        if algorithm == "pari":
             ker = M.__pari__().matker().mattranspose().sage()
-        elif algorithm == 'flint':
+        elif algorithm == "flint":
             ker = M._rational_kernel_flint().transpose()
         else:
             ker = M._rational_kernel_iml().transpose()
 
         if ker.nrows() == 0 and ker.ncols() != M.ncols():
             ker = ker.new_matrix(nrows=0, ncols=M.ncols())
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/half_dilation_surface.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/l_infinity_delaunay_cells.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,390 +1,397 @@
-#*****************************************************************************
-#       Copyright (C) 2013-2019 Vincent Delecroix <20100.delecroix@gmail.com>
-#                     2013-2019 W. Patrick Hooper <wphooper@gmail.com>
+r"""
+Cells for the L-infinity Delaunay triangulation.
+
+Each cell of the L-infinity Delaunay triangulation can be identified with a
+marked triangulation. The marking corresponds to the position of the horizontal
+and vertical separatrices. Each triangle hence get one of the following types:
+bottom-left, bottom-right, top-left, top-right.
+"""
+# ****************************************************************************
+#  This file is part of sage-flatsurf.
+#
+#       Copyright (C) 2016-2019 Vincent Delecroix
+#                     2016-2019 W. Patrick Hooper
+#                          2023 Julian Rüth
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
 #
-#  Distributed under the terms of the GNU General Public License (GPL)
-#  as published by the Free Software Foundation; either version 2 of
-#  the License, or (at your option) any later version.
-#                  https://www.gnu.org/licenses/
-#*****************************************************************************
-
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
-from six import iteritems
-
-from flatsurf.geometry.surface import Surface
-from flatsurf.geometry.similarity_surface import SimilaritySurface
-from flatsurf.geometry.mappings import SurfaceMapping, IdentityMapping, SurfaceMappingComposition
-from flatsurf.geometry.polygon import ConvexPolygons
-
-from sage.env import SAGE_VERSION
-if SAGE_VERSION >= '8.2':
-    from sage.structure.element import is_Matrix
-else:
-    from sage.matrix.matrix import is_Matrix
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+# ****************************************************************************
+from sage.misc.cachefunc import cached_method
+
+# the types of edges
+V_NONE = 0  # start vertex has no horizontal/vertical separatrix
+V_LEFT = 1  # horizontal separatrix going right
+V_RIGHT = 2  # horizontal separatrix going left
+V_BOT = 3  # vertical separatrix going up
+V_TOP = 4  # vertical separatrix going down
+
 
-class HalfDilationSurface(SimilaritySurface):
+def sign_and_norm_conditions(dim, i, s):
     r"""
-    Half dilation surface.
+    Inequalities:
 
-    A half-dilation surface is a (G,X) structure for the group of dilatations
-    `G = \RR^*` acting on the plane `X = \RR^2`. If you want to consider only
-    the oriented case, have a look at
-    :meth:`flatsurf.dilation_surface.DilationSurface`.
+    if `s=+1`, encode the inequalities `+1 >= x_i >= 0`
+    if `s=-1`, encode the inequalities `-1 <= x_i <= 0`
+
+    EXAMPLES::
+
+        sage: from flatsurf.geometry.l_infinity_delaunay_cells import sign_and_norm_conditions
+
+        sage: sorted(Polyhedron(ieqs=sign_and_norm_conditions(1, 0, 1)).vertices_list())
+        [[0], [1]]
+        sage: sorted(Polyhedron(ieqs=sign_and_norm_conditions(1, 0, -1)).vertices_list())
+        [[-1], [0]]
+
+        sage: ieqs = []
+        sage: ieqs.extend(sign_and_norm_conditions(2, 0, 1))
+        sage: ieqs.extend(sign_and_norm_conditions(2, 1, -1))
+        sage: sorted(Polyhedron(ieqs=ieqs).vertices_list())
+        [[0, -1], [0, 0], [1, -1], [1, 0]]
     """
-    def GL2R_mapping(self, matrix):
-        r"""
-        Deprecated. Use apply_matrix instead.
-        
-        Apply a 2x2 matrix to the polygons making up this surface. 
-        Returns the flatsurf.geometry.SurfaceMapping from this surface to its image.
-        """
-        deprecation(13109, "GL2R_mapping is deprecated. Use apply_matrix(mapping=True) instead.")
-        return GL2RMapping(self, matrix)
-        
-    def __rmul__(self,matrix):
+    l_sign = [0] * (dim + 1)
+    l_sign[i + 1] = s
+
+    l_norm = [0] * (dim + 1)
+    l_norm[i + 1] = -s
+    l_norm[0] = 1
+
+    return (l_sign, l_norm)
+
+
+def opposite_condition(dim, i, j):
+    r"""
+    encode the equality `x_i = -x_j`
+
+    EXAMPLES::
+
+        sage: from flatsurf.geometry.l_infinity_delaunay_cells import \
+        ....:     opposite_condition, sign_and_norm_conditions
+
+        sage: eq1 = opposite_condition(2, 0, 1)
+        sage: eq2 = opposite_condition(2, 1, 0)
+
+        sage: ieqs1 = sign_and_norm_conditions(2, 0, 1)
+        sage: ieqs2 = sign_and_norm_conditions(2, 1, -1)
+
+        sage: sorted(Polyhedron(eqns=[eq1], ieqs=ieqs1).vertices_list())
+        [[0, 0], [1, -1]]
+        sage: sorted(Polyhedron(eqns=[eq1,eq2], ieqs=ieqs1).vertices_list())
+        [[0, 0], [1, -1]]
+        sage: sorted(Polyhedron(eqns=[eq1,eq2], ieqs=ieqs1+ieqs2).vertices_list())
+        [[0, 0], [1, -1]]
+    """
+    linear = [0] * (dim + 1)
+    linear[i + 1] = 1
+    linear[j + 1] = 1
+
+    return linear
+
+
+def bottom_top_delaunay_condition(dim, p1, e1, p2, e2):
+    r"""
+    Delaunay condition for bottom-top pairs of triangles
+    """
+    # re(e2p1) <= im(e1) + im(e2m1)
+    e2m1 = (e2 + 2) % 3
+    e2p1 = (e2 + 1) % 3
+
+    im_e2m1 = 2 * (3 * p2 + e2m1) + 1
+    re_e2p1 = 2 * (3 * p2 + e2p1)
+    im_e1 = 2 * (3 * p1 + e1) + 1
+
+    linear = [0] * (dim + 1)
+    linear[im_e1 + 1] = 1
+    linear[im_e2m1 + 1] = 1
+    linear[re_e2p1 + 1] = -1
+
+    return linear
+
+
+def right_left_delaunay_condition(dim, p1, e1, p2, e2):
+    r"""
+    Delaunay condition for right-left pairs of triangles
+    """
+    # im(e2p1) <= re(e2) + re(e1m1)
+    e1m1 = (e1 + 2) % 3
+    e2p1 = (e2 + 1) % 3
+
+    im_e2p1 = 3 * (p2 + e2p1) + 1
+    re_e2 = 3 * (p2 + e2)
+    re_e1m1 = 3 * (p1 + e1m1)
+
+    linear = [0] * (dim + 1)
+    linear[re_e2 + 1] = 1
+    linear[re_e1m1 + 1] = 1
+    linear[im_e2p1 + 1] = -1
+
+    return linear
+
+
+class LInfinityMarkedTriangulation:
+    r"""
+    EXAMPLES::
+
+        sage: from flatsurf.geometry.l_infinity_delaunay_cells import \
+        ....:     V_NONE, V_BOT, V_TOP, V_RIGHT, V_LEFT, LInfinityMarkedTriangulation
+
+        sage: gluings = {(0,0):(1,2), (1,2):(0,0), (0,1):(1,0), (1,0):(0,1),
+        ....:            (0,2):(1,1), (1,1):(0,2)}
+        sage: types = [(V_BOT, V_NONE, V_RIGHT), (V_NONE, V_LEFT, V_TOP)]
+        sage: T = LInfinityMarkedTriangulation(2, gluings, types)
+    """
+
+    def __init__(self, num_faces, edge_identifications, edge_types, check=True):
+        from sage.rings.integer_ring import ZZ
+
+        self._n = ZZ(num_faces)
+        self._edge_identifications = edge_identifications
+        self._edge_types = edge_types
+        if check:
+            self._check()
+
+    def _check(self):
+        if self._n % 2:
+            raise ValueError("the number of faces must be even")
+
+        if sorted(self._edge_identifications.keys()) != [
+            (i, j) for i in range(self._n) for j in range(3)
+        ]:
+            raise ValueError("should be a triangulation")
+
+        if (
+            not isinstance(self._edge_types, list)
+            or len(self._edge_types) != self.num_faces()
+        ):
+            raise ValueError("edge_types invalid")
+
+        for i in range(self.num_faces()):
+            if len(self._edge_types[i]) != 3:
+                raise ValueError("edge_types invalid")
+            for j in range(3):
+                if self._edge_types[i][j] not in [
+                    V_NONE,
+                    V_LEFT,
+                    V_RIGHT,
+                    V_BOT,
+                    V_TOP,
+                ]:
+                    raise ValueError("types[{}] = {} invalid", i, self._edge_types[i])
+
+        seen = [False] * self._n
+        for p in range(self._n):
+            if seen[p]:
+                continue
+            sh = sum(
+                self._edge_types[p][r] == V_LEFT or self._edge_types[p][r] == V_RIGHT
+                for r in (0, 1, 2)
+            )
+            sv = sum(
+                self._edge_types[p][r] == V_BOT or self._edge_types[p][r] == V_TOP
+                for r in (0, 1, 2)
+            )
+            if sh != 1 or sv != 1:
+                raise ValueError(
+                    "triangle {} has invalid types {}".format(p, self._edge_types[p])
+                )
+
+    def num_faces(self):
+        return self._n
+
+    def num_edges(self):
+        return 3 * self._n // 2
+
+    def opposite_edge(self, p, e):
+        return self._edge_identifications[(p, e)]
+
+    def __repr__(self):
+        return "Marked triangulation made of {} triangles".format(self.num_faces())
+
+    def bottom_top_pairs(self):
         r"""
+        Return a list ``(p1,e1,p2,e2)``.
+
         EXAMPLES::
 
-            sage: from flatsurf import *
-            sage: s=translation_surfaces.infinite_staircase()
-            sage: s.underlying_surface()
-            The infinite staircase
-            sage: m=Matrix([[1,2],[0,1]])
-            sage: s2=m*s
-            sage: TestSuite(s2).run(skip='_test_pickling')
-            sage: s2.polygon(0)
-            Polygon: (0, 0), (1, 0), (3, 1), (2, 1)
-
-        Testing multiplication by a matrix with negative determinant::
-
-            sage: from flatsurf import *
-            sage: ds1 = dilation_surfaces.genus_two_square(1/2, 1/3, 1/4, 1/5)
-            sage: ds1.polygon(0)
-            Polygon: (0, 0), (1/2, 0), (1, 1/3), (1, 1), (3/4, 1), (0, 4/5)
-            sage: m = matrix(QQ, [[0, 1], [1, 0]]) # maps (x,y) to (y, x)
-            sage: ds2 = m*ds1
-            sage: ds2.polygon(0)
-            Polygon: (0, 0), (4/5, 0), (1, 3/4), (1, 1), (1/3, 1), (0, 1/2)
+            sage: from flatsurf.geometry.l_infinity_delaunay_cells import \
+            ....:     V_NONE, V_BOT, V_TOP, V_RIGHT, V_LEFT, LInfinityMarkedTriangulation
+
+            sage: gluings = {(0,0):(1,2), (1,2):(0,0), (0,1):(1,0), (1,0):(0,1),
+            ....:            (0,2):(1,1), (1,1):(0,2)}
+            sage: types = [(V_BOT, V_NONE, V_RIGHT), (V_NONE, V_LEFT, V_TOP)]
+            sage: T = LInfinityMarkedTriangulation(2, gluings, types)
+            sage: T.bottom_top_pairs()
+            [(0, 0, 1, 2)]
         """
-        if not is_Matrix(matrix):
-            raise NotImplementedError("Only implemented for matrices.")
-        if not matrix.dimensions!=(2,2):
-            raise NotImplementedError("Only implemented for 2x2 matrices.")
-        return self.__class__(GL2RImageSurface(self,matrix)).copy()
+        pairs = []
+        for p1 in range(self._n):
+            for e1 in range(3):
+                if self._edge_types[p1][e1] == V_BOT:
+                    e1p1 = (e1 + 1) % 3
+                    p2, e2 = self.opposite_edge(p1, e1p1)
+                    e2m1 = (e2 - 1) % 3
+                    if self._edge_types[p2][e2m1] == V_TOP:
+                        pairs.append((p1, e1, p2, e2m1))
+        return pairs
 
-    def apply_matrix(self,m,in_place=True, mapping=False):
+    def right_left_pairs(self):
         r"""
-        Carry out the GL(2,R) action of m on this surface and return the result.
-        
-        If in_place=True, then this is done in place and changes the surface. 
-        This can only be carried out if the surface is finite and mutable.
-        
-        If mapping=True, then we return a GL2RMapping between this surface and its image. 
-        In this case in_place must be False.
-        
-        If in_place=False, then a copy is made before the deformation.
+        Return a list ``(p1,e1,p2,e2)``
+
+        EXAMPLES::
+
+            sage: from flatsurf.geometry.l_infinity_delaunay_cells import \
+            ....:     V_NONE, V_BOT, V_TOP, V_RIGHT, V_LEFT, LInfinityMarkedTriangulation
+
+            sage: gluings = {(0,0):(1,2), (1,2):(0,0), (0,1):(1,0), (1,0):(0,1),
+            ....:            (0,2):(1,1), (1,1):(0,2)}
+            sage: types = [(V_BOT, V_NONE, V_LEFT), (V_NONE, V_RIGHT, V_TOP)]
+            sage: T = LInfinityMarkedTriangulation(2, gluings, types)
+            sage: T.right_left_pairs()
+            [(1, 1, 0, 2)]
         """
-        if mapping==True:
-            assert in_place==False, "Can not modify in place and return a mapping."
-            return GL2RMapping(self, m)
-        if not in_place:
-            if self.is_finite():
-                from sage.structure.element import get_coercion_model
-                cm = get_coercion_model()
-                field = cm.common_parent(self.base_ring(), m.base_ring())
-                s=self.copy(mutable=True, new_field=field)
-                return s.apply_matrix(m)
-            else:
-                return m*self
-        else:
-            # Make sure m is in the right state
-            from sage.matrix.constructor import Matrix
-            m=Matrix(self.base_ring(), 2, 2, m)
-            assert m.det()!=self.base_ring().zero(), "Can not deform by degenerate matrix."
-            assert self.is_finite(), "In place GL(2,R) action only works for finite surfaces."
-            us=self.underlying_surface()
-            assert us.is_mutable(), "In place changes only work for mutable surfaces."
-            for label in self.label_iterator():
-                us.change_polygon(label,m*self.polygon(label))
-            if m.det()<self.base_ring().zero():
-                # Polygons were all reversed orientation. Need to redo gluings.
-                
-                # First pass record new gluings in a dictionary.
-                new_glue={}
-                seen_labels=set()
-                for p1 in self.label_iterator():
-                    n1=self.polygon(p1).num_edges()
-                    for e1 in range(n1):
-                        p2,e2=self.opposite_edge(p1,e1)
-                        n2=self.polygon(p2).num_edges()
-                        if p2 in seen_labels:
-                            pass
-                        elif p1==p2 and e1>e2:
-                            pass
-                        else:
-                            new_glue[(p1, n1-1-e1)]=(p2, n2-1-e2)
-                    seen_labels.add(p1)
-                # Second pass: reassign gluings
-                for (p1,e1),(p2,e2) in iteritems(new_glue):
-                    us.change_edge_gluing(p1,e1,p2,e2)
-            return self
-                
-    def _edge_needs_flip_Linfinity(self, p1, e1, p2, e2):
+        pairs = []
+        for p1 in range(self._n):
+            for e1 in range(3):
+                if self._edge_types[p1][e1] == V_RIGHT:
+                    e1p1 = (e1 + 1) % 3
+                    p2, e2 = self.opposite_edge(p1, e1p1)
+                    e2m1 = (e2 - 1) % 3
+                    if self._edge_types[p2][e2m1] == V_LEFT:
+                        pairs.append((p1, e1, p2, e2m1))
+        return pairs
+
+    @cached_method
+    def polytope(self):
         r"""
-        Check whether the provided edge which bounds two triangles should be flipped
-        to get closer to the L-infinity Delaunay decomposition.
+        Each edge correspond to a vector in RR^2 (identified to CC)
 
-        TESTS::
+        We assign the following coordinates
 
-            sage: from flatsurf import *
-            sage: s = Surface_list(base_ring=QQ)
-            sage: t1 = polygons((1,0),(-1,1),(0,-1))
-            sage: t2 = polygons((0,1),(-1,0),(1,-1))
-            sage: s.add_polygon(polygons(vertices=[(0,0), (1,0), (0,1)]))
-            0
-            sage: s.add_polygon(polygons(vertices=[(1,1), (0,1), (1,0)]))
-            1
-            sage: s.change_polygon_gluings(0, [(1,0), (1,1), (1,2)])
-            sage: s = TranslationSurface(s)
-            sage: [s._edge_needs_flip_Linfinity(0, i, 1, i) for i in range(3)]
-            [False, False, False]
-
-            sage: ss = matrix(2, [1,1,0,1]) * s
-            sage: [ss._edge_needs_flip_Linfinity(0, i, 1, i) for i in range(3)]
-            [False, False, False]
-            sage: ss = matrix(2, [1,0,1,1]) * s
-            sage: [ss._edge_needs_flip_Linfinity(0, i, 1, i) for i in range(3)]
-            [False, False, False]
-
-            sage: ss = matrix(2, [1,2,0,1]) * s
-            sage: [ss._edge_needs_flip_Linfinity(0, i, 1, i) for i in range(3)]
-            [False, False, True]
-
-            sage: ss = matrix(2, [1,0,2,1]) * s
-            sage: [ss._edge_needs_flip_Linfinity(0, i, 1, i) for i in range(3)]
-            [True, False, False]
+        (p,e) -> real part at 2*(3*p + e) and imag part at 2*(3*p + e) + 1
+
+        The return polyhedron is compact as we fix each side to be of L-infinity
+        length less than 1.
         """
-        # safety check for now
-        assert self.opposite_edge(p1, e1) == (p2, e2), "not opposite edges"
+        dim = 4 * self.num_edges()
+        eqns = []
+        ieqs = []
+
+        signs = [None] * dim
+
+        # edges should sum up to zero
+        for p in range(self._n):
+            linear = [0] * (dim + 1)
+            linear[6 * p + 1] = 1
+            linear[6 * p + 3] = 1
+            linear[6 * p + 5] = 1
+            eqns.append(linear)
+
+            linear = [0] * (dim + 1)
+            linear[6 * p + 2] = 1
+            linear[6 * p + 4] = 1
+            linear[6 * p + 6] = 1
+            eqns.append(linear)
 
-        # triangles
-        poly1 = self.polygon(p1)
-        poly2 = self.polygon(p2)
-        if poly1.num_edges() != 3 or poly2.num_edges() != 3:
-            raise ValueError("edge must be adjacent to two triangles")
-
-        edge1 = poly1.edge(e1)
-        edge1L = poly1.edge(e1 - 1)
-        edge1R = poly1.edge(e1 + 1)
-        edge2 = poly2.edge(e2)
-        edge2L = poly2.edge(e2 - 1)
-        edge2R = poly2.edge(e2 + 1)
-
-        sim = self.edge_transformation(p2, e2)
-        m = sim.derivative()   # matrix carrying p2 to p1
-        if not m.is_one():
-            edge2 = m * edge2
-            edge2L = m * edge2L
-            edge2R = m * edge2R
-
-        # convexity check of the quadrilateral
-        from flatsurf.geometry.polygon import wedge_product
-        if wedge_product(edge2L, edge1R) <= 0 or \
-           wedge_product(edge1L, edge2R) <=0:
-            return False
-
-        # compare the norms
-        new_edge = edge2L + edge1R
-        n1 = max(abs(edge1[0]), abs(edge1[1]))
-        n = max(abs(new_edge[0]), abs(new_edge[1]))
-        return n < n1
+        # opposite edges are opposite vectors
+        for p1 in range(self._n):
+            for e1 in range(3):
+                p2, e2 = self.opposite_edge(p1, e1)
+                re1 = 2 * (3 * p1 + e1)
+                im1 = 2 * (3 * p1 + e1) + 1
+                re2 = 2 * (3 * p2 + e2)
+                im2 = 2 * (3 * p2 + e2) + 1
+                if re1 < re2:
+                    eqns.append(opposite_condition(dim, re1, re2))
+                    eqns.append(opposite_condition(dim, im1, im2))
+
+        # Compute the signs depending on edge types
+        for p in range(self._n):
+            for e1, e2 in ((2, 0), (0, 1), (1, 2)):
+                t = self._edge_types[p][e2]
+                re1 = 2 * (3 * p + e1)
+                im1 = 2 * (3 * p + e1) + 1
+                re2 = 2 * (3 * p + e2)
+                im2 = 2 * (3 * p + e2) + 1
+                if t == V_BOT:
+                    signs[re1] = signs[re2] = +1
+                    signs[im1] = -1
+                    signs[im2] = +1
+                elif t == V_TOP:
+                    signs[re1] = signs[re2] = -1
+                    signs[im1] = +1
+                    signs[im2] = -1
+                elif t == V_RIGHT:
+                    signs[re1] = +1
+                    signs[re2] = -1
+                    signs[im1] = signs[im2] = +1
+                elif t == V_LEFT:
+                    signs[re1] = -1
+                    signs[re2] = +1
+                    signs[im1] = signs[im2] = -1
+
+        # adding sign conditions
+        for i in range(dim):
+            ieqs.extend(sign_and_norm_conditions(dim, i, signs[i]))
+
+        # Delaunay conditions
+        for p1, e1, p2, e2 in self.bottom_top_pairs():
+            ieqs.append(bottom_top_delaunay_condition(dim, p1, e1, p2, e2))
+        for p1, e1, p2, e2 in self.right_left_pairs():
+            ieqs.append(right_left_delaunay_condition(dim, p1, e1, p2, e2))
 
-    def l_infinity_delaunay_triangulation(self, triangulated=False, in_place=False, limit=None, direction=None):
-        r"""
-        Returns a L-infinity Delaunay triangulation of a surface, or make some
-        triangle flips to get closer to the Delaunay decomposition.
+        #        return eqns, ieqs
 
-        INPUT:
+        from sage.geometry.polyhedron.constructor import Polyhedron
+        from sage.rings.rational_field import QQ
 
-        - ``triangulated`` -- optional (boolean, default ``False``) If true, the
-          algorithm assumes the surface is already triangulated. It does this
-          without verification.
-
-        - ``in_place`` -- optional (boolean, default ``False``) If true, the
-          triangulating and the triangle flips are done in place. Otherwise, a
-          mutable copy of the surface is made.
-
-        - ``limit`` -- optional (positive integer) If provided, then at most ``limit``
-            many diagonal flips will be done.
-
-        - ``direction`` -- optional (vector). Used to determine labels when a
-          pair of triangles is flipped. Each triangle has a unique separatrix
-          which points in the provided direction or its negation. As such a
-          vector determines a sign for each triangle.  A pair of adjacent
-          triangles have opposite signs. Labels are chosen so that this sign is
-          preserved (as a function of labels).
+        return Polyhedron(ieqs=ieqs, eqns=eqns, base_ring=QQ)
 
-        EXAMPLES::
+    def barycenter(self):
+        r"""
+        Return the translation surface in the barycenter of this polytope.
 
-            sage: from flatsurf import *
-            sage: s0 = translation_surfaces.veech_double_n_gon(5)
-            sage: field = s0.base_ring()
-            sage: a = field.gen()
-            sage: m = matrix(field, 2, [2,a,1,1])
-
-            sage: s = m*s0
-            sage: s = s.l_infinity_delaunay_triangulation()
-            sage: TestSuite(s).run()
-
-            sage: s = (m**2)*s0
-            sage: s = s.l_infinity_delaunay_triangulation()
-            sage: TestSuite(s).run()
-
-            sage: s = (m**3)*s0
-            sage: s = s.l_infinity_delaunay_triangulation()
-            sage: TestSuite(s).run()
-        """
-        if not self.is_finite():
-            raise NotImplementedError("no L-infinity Delaunay implemented for infinite surfaces")
-        if triangulated:
-            if in_place:
-                s = self
-            else:
-                from flatsurf.geometry.surface import Surface_dict
-                s = self.__class__(Surface_dict(surface=self,mutable=True))
-        else:
-            from flatsurf.geometry.surface import Surface_list
-            s = self.__class__(Surface_list(surface=self.triangulate(in_place=in_place),mutable=True))
-
-        if direction is None:
-            base_ring = self.base_ring()
-            direction = self.vector_space()( (base_ring.zero(), base_ring.one()) )
-        else:
-            assert not direction.is_zero()
-
-        triangles = set(s.label_iterator())
-        if limit is None:
-            limit = -1
-        else:
-            limit = int(limit)
-        while triangles and limit:
-            p1 = triangles.pop()
-            for e1 in range(3):
-                p2, e2 = s.opposite_edge(p1, e1)
-                if s._edge_needs_flip_Linfinity(p1, e1, p2, e2):
-                    s.triangle_flip(p1, e1, in_place=True, direction=direction)
-                    triangles.add(p1)
-                    triangles.add(p2)
-                    limit -= 1
-        return s
+        EXAMPLES::
 
-class GL2RImageSurface(Surface):
-    r"""
-    This is a lazy implementation of the SL(2,R) image of a translation surface.
+            sage: from flatsurf.geometry.l_infinity_delaunay_cells import \
+            ....:     V_NONE, V_BOT, V_TOP, V_RIGHT, V_LEFT, LInfinityMarkedTriangulation
 
-    EXAMPLE::
+            sage: gluings = {(0,0):(1,2), (1,2):(0,0), (0,1):(1,0), (1,0):(0,1),
+            ....:            (0,2):(1,1), (1,1):(0,2)}
+            sage: types = [(V_BOT, V_NONE, V_LEFT), (V_NONE, V_RIGHT, V_TOP)]
+            sage: T = LInfinityMarkedTriangulation(2, gluings, types)
+            sage: S = T.barycenter()
+            sage: S.polygon(0)
+            Polygon(vertices=[(0, 0), (3/7, 13/21), (-3/7, 11/21)])
+            sage: S.polygon(1)
+            Polygon(vertices=[(0, 0), (6/7, 2/21), (3/7, 13/21)])
+        """
+        verts = [v.vector() for v in self.polytope().vertices()]
+        b = sum(verts) / len(verts)
 
-        sage: import flatsurf
-        sage: s=flatsurf.translation_surfaces.octagon_and_squares()
-        sage: r=matrix(ZZ,[[0,1],[1,0]])
-        sage: ss=r*s
-        sage: TestSuite(ss).run()
-        sage: s.canonicalize()==ss.canonicalize()
-        True
+        from flatsurf import Polygon
+        from sage.rings.rational_field import QQ
 
-    """
+        from flatsurf import MutableOrientedSimilaritySurface
 
-    def __init__(self, surface, m, ring=None):
+        barycenter = MutableOrientedSimilaritySurface(QQ)
 
-        if surface.is_mutable():
-            if surface.is_finite():
-                self._s=surface.copy()
-            else:
-                raise ValueError("Can not apply matrix to mutable infinite surface.")
-        else:
-            self._s=surface
-
-        det = m.determinant()
-
-        if det>0:
-            self._det_sign=1
-        elif det<0:
-            self._det_sign=-1
-        else:
-            raise ValueError("Can not apply matrix with zero determinant to surface.")
-
-        self._m=m
-
-        if ring is None:
-            if m.base_ring() == self._s.base_ring():
-                base_ring = self._s.base_ring()
-            else:
-                from sage.structure.element import get_coercion_model
-                cm = get_coercion_model()
-                base_ring = cm.common_parent(m.base_ring(), self._s.base_ring())
-        else:
-            base_ring=ring
-
-        self._P = ConvexPolygons(base_ring)
-
-        super().__init__(base_ring, self._s.base_label(), finite=self._s.is_finite(), mutable=False)
-
-    def polygon(self, lab):
-        if self._det_sign==1:
-            p = self._s.polygon(lab)
-            edges = [ self._m * p.edge(e) for e in range(p.num_edges())]
-            return self._P(edges)
-        else:
-            p = self._s.polygon(lab)
-            edges = [ self._m * (-p.edge(e)) for e in range(p.num_edges()-1,-1,-1)]
-            return self._P(edges)
+        for p in range(self._n):
+            e1 = (b[6 * p], b[6 * p + 1])
+            e2 = (b[6 * p + 2], b[6 * p + 3])
+            e3 = (b[6 * p + 4], b[6 * p + 5])
+            barycenter.add_polygon(Polygon(edges=[e1, e2, e3], base_ring=QQ))
 
-    def opposite_edge(self, p, e):
-        if self._det_sign==1:
-            return self._s.opposite_edge(p,e)
-        else:
-            polygon = self._s.polygon(p)
-            pp,ee = self._s.opposite_edge(p,polygon.num_edges()-1-e)
-            polygon2 = self._s.polygon(pp)
-            return pp,polygon2.num_edges()-1-ee
+        for gluing in self._edge_identifications.items():
+            barycenter.glue(*gluing)
 
-class GL2RMapping(SurfaceMapping):
-    r"""
-    This class pushes a surface forward under a matrix.
-    
-    Note that for matrices of negative determinant we need to relabel edges (because
-    edges must have a counterclockwise cyclic order). For each n-gon in the surface,
-    we relabel edges according to the involution e mapsto n-1-e.
-
-    EXAMPLE::
-
-        sage: from flatsurf import *
-        sage: s=translation_surfaces.veech_2n_gon(4)
-        sage: from flatsurf.geometry.half_dilation_surface import GL2RMapping
-        sage: mat=Matrix([[2,1],[1,1]])
-        sage: m=GL2RMapping(s,mat)
-        sage: TestSuite(m.codomain()).run()
-    """
-    def __init__(self, s, m, ring=None):
-        r"""
-        Hit the surface s with the 2x2 matrix m which should have positive determinant.
-        """
-        codomain = s.__class__(GL2RImageSurface(s,m,ring = ring))
-        self._m=m
-        self._im=~m
-        SurfaceMapping.__init__(self, s, codomain)
-
-    def push_vector_forward(self,tangent_vector):
-        r"""Applies the mapping to the provided vector."""
-        return self.codomain().tangent_vector(
-                tangent_vector.polygon_label(), \
-                self._m*tangent_vector.point(), \
-                self._m*tangent_vector.vector())
-
-    def pull_vector_back(self,tangent_vector):
-        r"""Applies the inverse of the mapping to the provided vector."""
-        return self.domain().tangent_vector(
-                tangent_vector.polygon_label(), \
-                self._im*tangent_vector.point(), \
-                self._im*tangent_vector.vector())
+        return barycenter
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/half_translation_surface.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/half_dilation_surface.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,281 +1,367 @@
-#*****************************************************************************
-#       Copyright (C) 2013-2019 Vincent Delecroix <20100.delecroix@gmail.com>
-#                     2013-2019 W. Patrick Hooper <wphooper@gmail.com>
+# ****************************************************************************
+#  This file is part of sage-flatsurf.
 #
-#  Distributed under the terms of the GNU General Public License (GPL)
-#  as published by the Free Software Foundation; either version 2 of
-#  the License, or (at your option) any later version.
-#                  https://www.gnu.org/licenses/
-#*****************************************************************************
+#       Copyright (C) 2013-2019 Vincent Delecroix
+#                     2013-2019 W. Patrick Hooper
+#                          2023 Julian Rüth
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+# ****************************************************************************
 
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
+from flatsurf.geometry.surface import OrientedSimilaritySurface
+from flatsurf.geometry.mappings import SurfaceMapping
 
-import itertools
+from sage.misc.cachefunc import cached_method
 
-from .polygon import wedge_product
-from .surface import Surface
-from .half_dilation_surface import HalfDilationSurface
-from .rational_cone_surface import RationalConeSurface
 
-from sage.rings.all import QQ, AA
-from sage.matrix.constructor import matrix
+class GL2RImageSurface(OrientedSimilaritySurface):
+    r"""
+    The GL(2,R) image of an oriented similarity surface.
 
+    EXAMPLE::
+
+        sage: from flatsurf import translation_surfaces
+        sage: S = translation_surfaces.octagon_and_squares()
+        sage: r = matrix(ZZ,[[0, 1], [1, 0]])
+        sage: SS = r * S
+
+        sage: S.canonicalize() == SS.canonicalize()
+        True
+
+    TESTS::
+
+        sage: TestSuite(SS).run()
+
+        sage: from flatsurf.geometry.half_dilation_surface import GL2RImageSurface
+        sage: isinstance(SS, GL2RImageSurface)
+        True
 
-class HalfTranslationSurface(HalfDilationSurface, RationalConeSurface):
-    r"""
-    A half translation surface has gluings between polygons whose monodromy is +I or -I.
     """
-    def angles(self, numerical=False, return_adjacent_edges=False):
+
+    def __init__(self, surface, m, ring=None, category=None):
+        if surface.is_mutable():
+            if surface.is_finite_type():
+                from flatsurf.geometry.surface import MutableOrientedSimilaritySurface
+
+                self._s = MutableOrientedSimilaritySurface.from_surface(surface)
+            else:
+                raise ValueError("Can not apply matrix to mutable infinite surface.")
+        else:
+            self._s = surface
+
+        det = m.determinant()
+
+        if det > 0:
+            self._det_sign = 1
+        elif det < 0:
+            self._det_sign = -1
+        else:
+            raise ValueError("Can not apply matrix with zero determinant to surface.")
+
+        if m.is_mutable():
+            from sage.all import matrix
+
+            m = matrix(m, immutable=True)
+
+        self._m = m
+
+        if ring is None:
+            if m.base_ring() == self._s.base_ring():
+                base_ring = self._s.base_ring()
+            else:
+                from sage.structure.element import get_coercion_model
+
+                cm = get_coercion_model()
+                base_ring = cm.common_parent(m.base_ring(), self._s.base_ring())
+        else:
+            base_ring = ring
+
+        if category is None:
+            category = surface.category()
+
+        super().__init__(base_ring, category=category)
+
+    def roots(self):
         r"""
-        Return the set of angles around the vertices of the surface.
+        Return root labels for the polygons forming the connected
+        components of this surface.
 
-        These are given as multiple of `2 \pi`.
+        This implements
+        :meth:`flatsurf.geometry.categories.polygonal_surfaces.PolygonalSurfaces.ParentMethods.roots`.
 
         EXAMPLES::
 
-            sage: import flatsurf.geometry.similarity_surface_generators as sfg
-            sage: sfg.translation_surfaces.regular_octagon().angles()
-            [3]
-            sage: S = sfg.translation_surfaces.veech_2n_gon(5)
-            sage: S.angles()
-            [2, 2]
-            sage: S.angles(numerical=True)
-            [2.0, 2.0]
-            sage: S.angles(return_adjacent_edges=True) # random output
-            [(2, [(0, 1), (0, 5), (0, 9), (0, 3), (0, 7)]),
-             (2, [(0, 0), (0, 4), (0, 8), (0, 2), (0, 6)])]
-            sage: S.angles(numerical=True, return_adjacent_edges=True) # random output
-            [(2.0, [(0, 1), (0, 5), (0, 9), (0, 3), (0, 7)]),
-             (2.0, [(0, 0), (0, 4), (0, 8), (0, 2), (0, 6)])]
-
-            sage: sfg.translation_surfaces.veech_2n_gon(6).angles()
-            [5]
-            sage: sfg.translation_surfaces.veech_double_n_gon(5).angles()
-            [3]
-            sage: sfg.translation_surfaces.cathedral(1, 1).angles()
-            [3, 3, 3]
-
-            sage: from flatsurf import polygons, similarity_surfaces
-            sage: B = similarity_surfaces.billiard(polygons.triangle(1, 2, 5))
-            sage: H = B.minimal_cover(cover_type="half-translation")
-            sage: S = B.minimal_cover(cover_type="translation")
-            sage: H.angles()
-            [1/2, 5/2, 1/2, 1/2]
-            sage: S.angles()
-            [1, 5, 1, 1]
-
-            sage: H.angles(return_adjacent_edges=True)
-             [(1/2, [...]), (5/2, [...]), (1/2, [...]), (1/2, [...])]
-            sage: S.angles(return_adjacent_edges=True)
-             [(1, [...]), (5, [...]), (1, [...]), (1, [...])]
-        """
-        if not self.is_finite():
-            raise NotImplementedError("the set of edges is infinite!")
-
-        edges = set(self.edge_iterator())
-        angles = []
-
-        if return_adjacent_edges:
-            while edges:
-                # Note that iteration order here is different for different
-                # versions of Python. Therefore, the output in the doctest
-                # above is random.
-                pair = p,e = next(iter(edges))
-                ve = self.polygon(p).edge(e)
-                angle = 0
-                adjacent_edges = []
-                while pair in edges:
-                    adjacent_edges.append(pair)
-                    edges.remove(pair)
-                    f = (e-1) % self.polygon(p).num_edges()
-                    ve = self.polygon(p).edge(e)
-                    vf = -self.polygon(p).edge(f)
-                    ppair = pp,ff = self.opposite_edge(p, f)
-                    angle += (ve[0] > 0 and vf[0] <= 0) or (ve[0] < 0 and vf[0] >= 0) or (ve[0] == vf[0] == 0)
-                    pair, p, e = ppair, pp, ff
-                if numerical:
-                    angles.append((float(angle) / 2, adjacent_edges))
-                else:
-                    angles.append((QQ((angle, 2)), adjacent_edges))
-        else:
-            while edges:
-                pair = p,e = next(iter(edges))
-                angle = 0
-                while pair in edges:
-                    edges.remove(pair)
-                    f = (e-1) % self.polygon(p).num_edges()
-                    ve = self.polygon(p).edge(e)
-                    vf = -self.polygon(p).edge(f)
-                    ppair = pp,ff = self.opposite_edge(p, f)
-                    angle += (ve[0] > 0 and vf[0] <= 0) or (ve[0] < 0 and vf[0] >= 0) or (ve[0] == vf[0] == 0)
-                    pair, p, e = ppair, pp, ff
-                if numerical:
-                    angles.append(float(angle) / 2)
-                else:
-                    angles.append(QQ((angle,2)))
+            sage: from flatsurf import translation_surfaces
+            sage: S = translation_surfaces.octagon_and_squares()
+            sage: r = matrix(ZZ,[[0, 1], [1, 0]])
+            sage: S = r * S
+
+            sage: S.roots()
+            (0,)
 
-        return angles
+        """
+        return self._s.roots()
 
-    def stratum(self):
+    def is_compact(self):
         r"""
+        Return whether this surface is compact as a topological space.
+
+        This implements
+        :meth:`flatsurf.geometry.categories.topological_surfaces.TopologicalSurfaces.ParentMethods.is_compact`.
+
         EXAMPLES::
 
-            sage: from flatsurf import polygons, similarity_surfaces
-            sage: B = similarity_surfaces.billiard(polygons.triangle(1, 2, 5))
-            sage: H = B.minimal_cover(cover_type="half-translation")
-            sage: H.stratum()
-            Q_1(3, -1^3)
-        """
-        angles = self.angles()
-        if all(x.denominator() == 1 for x in angles):
-            raise NotImplementedError
-        from surface_dynamics import QuadraticStratum
-        return QuadraticStratum(*[2*a-2 for a in angles])
-
-    def _test_edge_matrix(self, **options):
-        r"""
-        Check the compatibility condition
-        """
-        tester = self._tester(**options)
-        from flatsurf.geometry.similarity_surface import SimilaritySurface
-        if self.is_finite():
-            it = self.label_iterator()
-        else:
-            it = islice(self.label_iterator(), 30)
+            sage: from flatsurf import translation_surfaces
+            sage: S = translation_surfaces.octagon_and_squares()
+            sage: r = matrix(ZZ,[[0, 1], [1, 0]])
+            sage: S = r * S
 
-        for lab in it:
-            p = self.polygon(lab)
-            for e in range(p.num_edges()):
-                # Warning: check the matrices computed from the edges,
-                # rather the ones overriden by TranslationSurface.
-                m = SimilaritySurface.edge_matrix(self,lab,e)
-                tester.assertTrue(m.is_one() or (-m).is_one(),
-                    "edge_matrix between edge e={} and e'={} has matrix\n{}\nwhich is neither a translation nor a rotation by pi".format((lab,e), self.opposite_edge((lab,e)), m))
+            sage: S.is_compact()
+            True
 
-    def holonomy_field(self):
+        """
+        return self._s.is_compact()
+
+    def is_mutable(self):
         r"""
-        Return the relative holonomy field of this translation or half-translation surface.
+        Return whether this surface is mutable, i.e., return ``False``.
+
+        This implements
+        :meth:`flatsurf.geometry.categories.topological_surfaces.TopologicalSurfaces.ParentMethods.is_mutable`.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
+            sage: S = translation_surfaces.octagon_and_squares()
+            sage: r = matrix(ZZ,[[0, 1], [1, 0]])
+            sage: S = r * S
 
-            sage: S = translation_surfaces.veech_2n_gon(5)
-            sage: S.holonomy_field()
-            Number Field in a0 with defining polynomial x^2 - x - 1 with a0 = 1.618033988749895?
-            sage: S.base_ring()
-            Number Field in a with defining polynomial y^4 - 5*y^2 + 5 with a = 1.175570504584947?
-
-            sage: T = translation_surfaces.torus((1, AA(2).sqrt()), (AA(3).sqrt(), 3))
-            sage: T.holonomy_field()
-            Rational Field
-
-            sage: T = polygons.triangle(1,6,11)
-            sage: S = similarity_surfaces.billiard(T)
-            sage: S = S.minimal_cover("translation")
-            sage: S.base_ring()
-            Number Field in c with defining polynomial x^6 - 6*x^4 + 9*x^2 - 3 with c = 1.969615506024417?
-            sage: S.holonomy_field()
-            Number Field in c0 with defining polynomial x^3 - 3*x - 1 with c0 = 1.879385241571817?
-        """
-        return self.normalized_coordinates()[0].base_ring()
-
-    def normalized_coordinates(self):
-        r"""
-        Return a pair ``(new_surface, matrix)`` where ``new_surface`` is defined over the
-        holonomy field and ``matrix`` is the transition matrix that maps this surface to
-        ``new_surface``.
+            sage: S.is_mutable()
+            False
+
+        """
+        return False
+
+    def is_translation_surface(self, positive=True):
+        r"""
+        Return whether this surface is a translation surface, i.e., glued
+        edges can be transformed into each other by translations.
+
+        This implements
+        :meth:`flatsurf.geometry.categories.similarity_surfaces.SimilaritySurfaces.ParentMethods.is_translation_surface`.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
+            sage: S = translation_surfaces.octagon_and_squares()
+            sage: r = matrix(ZZ,[[0, 1], [1, 0]])
+            sage: S = r * S
 
-            sage: S = translation_surfaces.veech_2n_gon(5)
-            sage: U, mat = S.normalized_coordinates()
-            sage: U.base_ring()
-            Number Field in a0 with defining polynomial x^2 - x - 1 with a0 = 1.618033988749895?
-            sage: mat
-            [             0 -2/5*a^3 + 2*a]
-            [            -1 -3/5*a^3 + 2*a]
-
-            sage: T = translation_surfaces.torus((1, AA(2).sqrt()), (AA(3).sqrt(), 3))
-            sage: U, mat = T.normalized_coordinates()
-            sage: U.base_ring()
-            Rational Field
-            sage: U.holonomy_field()
-            Rational Field
-            sage: mat
-            [-2.568914100752347?  1.816496580927726?]
-            [-5.449489742783178?  3.146264369941973?]
-            sage: TestSuite(U).run()
-
-            sage: T = polygons.triangle(1,6,11)
-            sage: S = similarity_surfaces.billiard(T)
-            sage: S = S.minimal_cover("translation")
-            sage: U, _ = S.normalized_coordinates()
-            sage: U.base_ring()
-            Number Field in c0 with defining polynomial x^3 - 3*x - 1 with c0 = 1.879385241571817?
-            sage: U.holonomy_field() == U.base_ring()
+            sage: S.is_translation_surface()
             True
-            sage: S.base_ring()
-            Number Field in c with defining polynomial x^6 - 6*x^4 + 9*x^2 - 3 with c = 1.969615506024417?
-            sage: TestSuite(U).run()
-
-            sage: from flatsurf import EquiangularPolygons
-            sage: E = EquiangularPolygons(1, 3, 1, 1)
-            sage: r1, r2 = [r.vector() for r in E.lengths_polytope().rays()]
-            sage: p = E(r1 + r2)
-            sage: B = similarity_surfaces.billiard(p)
-            sage: B.minimal_cover("translation")
-            TranslationSurface built from 6 polygons
-            sage: S = B.minimal_cover("translation")
-            sage: S, _ = S.normalized_coordinates()
-            sage: S
-            TranslationSurface built from 6 polygons
-        """
-        if not self.is_finite():
-            raise ValueError('the surface must be finite')
-        if self.base_ring() is QQ:
-            return (self, matrix(QQ, 2, 2, 1))
-
-        lab = next(self.label_iterator())
-        p = self.polygon(lab)
-        u = p.edge(1)
-        v = -p.edge(0)
-        i = 1
-        while wedge_product(u, v) == 0:
-            i += 1
-            u = p.edge(i)
-            v = -p.edge(i-1)
-        M = matrix(2, [u,v]).transpose().inverse()
-        assert M.det() > 0
-        hols = []
-        for lab in self.label_iterator():
-            p = self.polygon(lab)
-            for e in range(p.num_edges()):
-                w = M * p.edge(e)
-                hols.append(w[0])
-                hols.append(w[1])
-        if self.base_ring() is AA:
-            from .subfield import number_field_elements_from_algebraics
-            K, new_hols = number_field_elements_from_algebraics(hols)
+
+        """
+        return self._s.is_translation_surface(positive=positive)
+
+    @cached_method
+    def polygon(self, lab):
+        r"""
+        Return the polygon with ``label``.
+
+        This implements
+        :meth:`flatsurf.geometry.categories.polygonal_surfaces.PolygonalSurfaces.ParentMethods.polygon`.
+
+        EXAMPLES::
+
+            sage: from flatsurf import translation_surfaces
+            sage: S = translation_surfaces.octagon_and_squares()
+            sage: r = matrix(ZZ,[[0, 1], [1, 0]])
+            sage: S = r * S
+
+            sage: S.polygon(0)
+            Polygon(vertices=[(0, 0), (a, -a), (a + 2, -a), (2*a + 2, 0), (2*a + 2, 2), (a + 2, a + 2), (a, a + 2), (0, 2)])
+
+        """
+        if self._det_sign == 1:
+            p = self._s.polygon(lab)
+            edges = [self._m * p.edge(e) for e in range(len(p.vertices()))]
+
+            from flatsurf import Polygon
+
+            return Polygon(edges=edges, base_ring=self.base_ring())
+        else:
+            p = self._s.polygon(lab)
+            edges = [
+                self._m * (-p.edge(e)) for e in range(len(p.vertices()) - 1, -1, -1)
+            ]
+
+            from flatsurf import Polygon
+
+            return Polygon(edges=edges, base_ring=self.base_ring())
+
+    def labels(self):
+        r"""
+        Return the labels of this surface.
+
+        This implements
+        :meth:`flatsurf.geometry.categories.polygonal_surfaces.PolygonalSurfaces.ParentMethods.labels`.
+
+        EXAMPLES::
+
+            sage: from flatsurf import translation_surfaces
+            sage: S = translation_surfaces.octagon_and_squares()
+            sage: r = matrix(ZZ,[[0, 1], [1, 0]])
+            sage: S = r * S
+
+            sage: S.labels()
+            (0, 1, 2)
+
+        """
+        return self._s.labels()
+
+    def opposite_edge(self, p, e):
+        r"""
+        Return the polygon label and edge index when crossing over the ``edge``
+        of the polygon ``label``.
+
+        This implements
+        :meth:`flatsurf.geometry.categories.polygonal_surfaces.PolygonalSurfaces.ParentMethods.opposite_edge`.
+
+        EXAMPLES::
+
+            sage: from flatsurf import translation_surfaces
+            sage: S = translation_surfaces.octagon_and_squares()
+            sage: r = matrix(ZZ,[[0, 1], [1, 0]])
+            sage: S = r * S
+
+            sage: S.opposite_edge(0, 0)
+            (2, 0)
+
+        """
+        if self._det_sign == 1:
+            return self._s.opposite_edge(p, e)
         else:
-            from .subfield import subfield_from_elements
-            K, new_hols, _ = subfield_from_elements(self.base_ring(), hols)
+            polygon = self._s.polygon(p)
+            pp, ee = self._s.opposite_edge(p, len(polygon.vertices()) - 1 - e)
+            polygon2 = self._s.polygon(pp)
+            return pp, len(polygon2.vertices()) - 1 - ee
+
+    def __repr__(self):
+        r"""
+        Return a printable representation of this surface.
+
+        EXAMPLES::
+
+            sage: from flatsurf import translation_surfaces
+            sage: S = translation_surfaces.octagon_and_squares()
+            sage: matrix([[0, 1], [1, 0]]) * S
+            Translation Surface in H_3(4) built from 2 squares and a regular octagon
+            sage: matrix([[0, 2], [1, 0]]) * S
+            Translation Surface in H_3(4) built from a rhombus, a rectangle and an octagon
+
+        """
+        if self.is_finite_type():
+            from flatsurf.geometry.surface import MutableOrientedSimilaritySurface
 
-        from .polygon import ConvexPolygons
-        from .surface import Surface_list
-        S = Surface_list(K)
-        C = ConvexPolygons(K)
-        relabelling = {}
-        k = 0
-        for lab in self.label_iterator():
-            m = self.polygon(lab).num_edges()
-            relabelling[lab] = S.add_polygon(C(edges=[(new_hols[k + 2*i], new_hols[k + 2*i+1]) for i in range(m)]))
-            k += 2 * m
+            S = MutableOrientedSimilaritySurface.from_surface(self)
+            S.set_immutable()
+            return repr(S)
 
-        for (p1,e1),(p2,e2) in self.edge_iterator(gluings=True):
-            S.set_edge_pairing(relabelling[p1], e1, relabelling[p2], e2)
+        return f"GL2RImageSurface of {self._s!r}"
 
-        return (type(self)(S), M)
+    def __hash__(self):
+        r"""
+        Return a hash value for this surface that is compatible with
+        :meth:`__eq__`.
+
+        EXAMPLES::
+
+            sage: from flatsurf import translation_surfaces
+            sage: S = translation_surfaces.octagon_and_squares()
+            sage: r = matrix(ZZ,[[0, 1], [1, 0]])
+
+            sage: hash(r * S) == hash(r * S)
+            True
+
+        """
+        return hash((self._s, self._m))
+
+    def __eq__(self, other):
+        r"""
+        Return whether this image is indistinguishable from ``other``.
+
+        See :meth:`SimilaritySurfaces.FiniteType._test_eq_surface` for details
+        on this notion of equality.
+
+        EXAMPLES::
+
+            sage: from flatsurf import translation_surfaces
+            sage: S = translation_surfaces.octagon_and_squares()
+            sage: m = matrix(ZZ,[[0, 1], [1, 0]])
+            sage: m * S == m * S
+            True
+
+        """
+        if not isinstance(other, GL2RImageSurface):
+            return False
+
+        return (
+            self._s == other._s
+            and self._m == other._m
+            and self.base_ring() == other.base_ring()
+        )
+
+
+class GL2RMapping(SurfaceMapping):
+    r"""
+    This class pushes a surface forward under a matrix.
+
+    Note that for matrices of negative determinant we need to relabel edges (because
+    edges must have a counterclockwise cyclic order). For each n-gon in the surface,
+    we relabel edges according to the involution `e \mapsto n-1-e`.
+
+    EXAMPLE::
+
+        sage: from flatsurf import translation_surfaces
+        sage: s=translation_surfaces.veech_2n_gon(4)
+        sage: from flatsurf.geometry.half_dilation_surface import GL2RMapping
+        sage: mat=Matrix([[2,1],[1,1]])
+        sage: m=GL2RMapping(s,mat)
+        sage: TestSuite(m.codomain()).run()
+    """
+
+    def __init__(self, s, m, ring=None, category=None):
+        r"""
+        Hit the surface s with the 2x2 matrix m which should have positive determinant.
+        """
+        codomain = GL2RImageSurface(s, m, ring=ring, category=category or s.category())
+        self._m = m
+        self._im = ~m
+        SurfaceMapping.__init__(self, s, codomain)
+
+    def push_vector_forward(self, tangent_vector):
+        r"""Applies the mapping to the provided vector."""
+        return self.codomain().tangent_vector(
+            tangent_vector.polygon_label(),
+            self._m * tangent_vector.point(),
+            self._m * tangent_vector.vector(),
+        )
+
+    def pull_vector_back(self, tangent_vector):
+        r"""Applies the inverse of the mapping to the provided vector."""
+        return self.domain().tangent_vector(
+            tangent_vector.polygon_label(),
+            self._im * tangent_vector.point(),
+            self._im * tangent_vector.vector(),
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/interval_exchange_transformation.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/interval_exchange_transformation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,10 @@
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
-
 from sage.structure.sage_object import SageObject
 
+
 class FlowPolygonMap(SageObject):
     r"""
     The map obtained as the return map of the flow on the sides of a (convex)
     polygon.
 
     Formally, this can be defined as follows: one start with two partition into
     (finitely many) intervals of a given interval. The map corresponds to
@@ -27,56 +25,61 @@
         sage: [T.forward_image(0,x) for x in range(3)]
         [(2, 0), (1, 0), (1, 1)]
         sage: [T.forward_image(1,x) for x in range(4)]
         [(1, 1), (1, 2), (0, 0), (0, 1)]
         sage: [T.forward_image(2,x) for x in range(1)]
         [(0, 1)]
     """
+
     def __init__(self, ring, bot_labels, bot_lengths, top_labels, top_lengths):
         r"""
         INPUT:
 
         - ``ring`` -- the base ring for the lengths of the interval
 
         - ``bot_labels`` -- labels for the bottom partition
 
         - ``bot_lengths`` -- lengths for the bottom partition
 
         - ``top_labels`` -- labels for the top partition
 
         - ``top_lengths`` -- lengths for top partition
         """
-        assert all(x > ring.zero() for x in bot_lengths)
-        assert all(x > ring.zero() for x in top_lengths)
-        assert len(bot_labels) == len(bot_lengths)
-        assert len(top_labels) == len(top_lengths)
-        assert sum(top_lengths)  == sum(bot_lengths)
+        if not all(x > ring.zero() for x in bot_lengths):
+            raise ValueError
+        if not all(x > ring.zero() for x in top_lengths):
+            raise ValueError
+        if len(bot_labels) != len(bot_lengths):
+            raise ValueError
+        if len(top_labels) != len(top_lengths):
+            raise ValueError
+        if sum(top_lengths) != sum(bot_lengths):
+            raise ValueError
 
         self._ring = ring
 
         self._bot_labels = bot_labels
         self._top_labels = top_labels
-        self._bot_labels_to_index = {j:i for i,j in enumerate(bot_labels)}
-        self._top_labels_to_index = {j:i for i,j in enumerate(top_labels)}
+        self._bot_labels_to_index = {j: i for i, j in enumerate(bot_labels)}
+        self._top_labels_to_index = {j: i for i, j in enumerate(top_labels)}
         if len(self._bot_labels) != len(self._bot_labels_to_index):
             raise ValueError("non unique labels for bot: {}".format(bot_labels))
         if len(self._top_labels) != len(self._top_labels_to_index):
             raise ValueError("non unique labels in top: {}".format(top_labels))
 
-        self._bot_lengths = list(map(ring,bot_lengths))
-        self._top_lengths = list(map(ring,top_lengths))
-
+        self._bot_lengths = list(map(ring, bot_lengths))
+        self._top_lengths = list(map(ring, top_lengths))
 
         # forward image of intervals
         it = 0
         lt = x1 = top_lengths[it]
         self._forward_images = []
         for ib in range(len(bot_lengths)):
             lenb = bot_lengths[ib]
-            self._forward_images.append((it,lt-x1))
+            self._forward_images.append((it, lt - x1))
 
             while lenb and lenb >= x1:
                 lenb -= x1
                 it += 1
                 if it < len(top_lengths):
                     lt = x1 = top_lengths[it]
                 else:
@@ -86,15 +89,15 @@
 
         # backward image of intervals
         ib = 0
         lb = x1 = bot_lengths[ib]
         self._backward_images = []
         for it in range(len(top_lengths)):
             lent = top_lengths[it]
-            self._backward_images.append((ib,lb-x1))
+            self._backward_images.append((ib, lb - x1))
 
             while lent and lent >= x1:
                 lent -= x1
                 ib += 1
                 if ib < len(bot_lengths):
                     lb = x1 = bot_lengths[ib]
                 else:
@@ -133,23 +136,23 @@
             (2, 0)
             sage: T.forward_image(0, 1)  # could have equally been (2, 1)
             (3, 0)
         """
         i = self._bot_labels_to_index[i]
         if x < self._ring.zero() or x > self._bot_lengths[i]:
             raise ValueError("x = {} is out of the interval".format(x))
-        j,y = self._forward_images[i]
-        if x+y < self._top_lengths[j]:
-            return (self._top_labels[j], x+y)
-        x -= self._top_lengths[j]-y
+        j, y = self._forward_images[i]
+        if x + y < self._top_lengths[j]:
+            return (self._top_labels[j], x + y)
+        x -= self._top_lengths[j] - y
         j += 1
         while x > self._top_lengths[j]:
             x -= self._top_lengths[j]
             j += 1
-        return (self._top_labels[j],x)
+        return (self._top_labels[j], x)
 
     def backward_image(self, i, x):
         r"""
         EXAMPLES::
 
             sage: from flatsurf.geometry.interval_exchange_transformation import \
             ....:     FlowPolygonMap
@@ -187,16 +190,16 @@
             ....:         assert T.backward_image(*p1) == p0, "p0 = {}, p1 = {}".format(p0,p1)
             ....:         p0 = p1
 
         """
         i = self._top_labels_to_index[i]
         if x < self._ring.zero() or x > self._top_lengths[i]:
             raise ValueError("x = {} is out of the interval".format(x))
-        j,y = self._backward_images[i]
-        if x+y < self._bot_lengths[j]:
-            return (self._bot_labels[j], x+y)
-        x -= self._bot_lengths[j]-y
+        j, y = self._backward_images[i]
+        if x + y < self._bot_lengths[j]:
+            return (self._bot_labels[j], x + y)
+        x -= self._bot_lengths[j] - y
         j += 1
         while x > self._bot_lengths[j]:
             x -= self._bot_lengths[j]
             j += 1
-        return (self._bot_labels[j],x)
+        return (self._bot_labels[j], x)
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/mappings.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/mappings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,947 +1,898 @@
 r"""Mappings between translation surfaces."""
+# *********************************************************************
+#  This file is part of sage-flatsurf.
+#
+#        Copyright (C) 2016-2022 W. Patrick Hooper
+#                      2016-2022 Vincent Delecroix
+#                           2023 Julian Rüth
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+# *********************************************************************
 
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
-from six import iteritems
-
-from flatsurf.geometry.polygon import ConvexPolygons, wedge_product
-from flatsurf.geometry.surface import Surface, Surface_list, Surface_dict, ExtraLabel
-from flatsurf.geometry.similarity_surface import SimilaritySurface
-
-from sage.rings.infinity import Infinity
-from sage.structure.sage_object import SageObject
 
 class SurfaceMapping:
     r"""Abstract class for any mapping between surfaces."""
-    
+
     def __init__(self, domain, codomain):
-        self._domain=domain
-        self._codomain=codomain
-    
+        self._domain = domain
+        self._codomain = codomain
+
     def domain(self):
         r"""
         Return the domain of the mapping.
         """
         return self._domain
 
     def codomain(self):
         r"""
         Return the range of the mapping.
         """
         return self._codomain
 
-    def push_vector_forward(self,tangent_vector):
+    def push_vector_forward(self, tangent_vector):
         r"""Applies the mapping to the provided vector."""
         raise NotImplementedError
 
-    def pull_vector_back(self,tangent_vector):
+    def pull_vector_back(self, tangent_vector):
         r"""Applies the inverse of the mapping to the provided vector."""
         raise NotImplementedError
-        
-    def __mul__(self,other):
+
+    def __mul__(self, other):
         # Compose SurfaceMappings
-        return SurfaceMappingComposition(other,self)
-    
-    def __rmul__(self,other):
-        return SurfaceMappingComposition(self,other)
-
-
-#class FinitelyPerturbedSurface(Surface):
-#    def __init__(self, surface, polygon_dictionary=None, glue_dictionary=None, base_label=None, ring=None):
-#        r"""
-#        
-#        Warning: No checks are made to make sure the surface is reasonable.
-#        
-#        PARAMETERS::
-#            surface: The surface this is based on.
-#            polygon_dictionary: A dictionary mapping labels to polygons which will override whatever was on the original surface.
-#            glue_dictionary: A dictionary mapping edges to edges, which will override whatever was on the original surface. It will automatically be made symmetric.
-#            base_label: A label representing the base_label on the new surface.
-#            ring: A new ring containing the vertices.
-#        """
-#        self._s=surface
-#        if polygon_dictionary is None:
-#            self._pdict={}
-#        else:
-#            self._pdict=dict(polygon_dictionary)
-#        self._gdict={}
-#        if not glue_dictionary is None:
-#            for edge1,edge2 in iteritems(glue_dictionary):
-#                self._gdict[edge1]=edge2
-#                self._gdict[edge2]=edge1
-#        if base_label is None:
-#            self._base_label = surface.base_label()
-#        else:
-#            self._base_label = base_label
-#        if ring is None:
-#            self._ring = surface.base_ring()
-#        else:
-#            self._ring = ring
-#        self._is_finite = surface.is_finite()
-#        Surface.__init__(self, )
-
-#    def base_ring(self):
-#        return self._ring
-
-#    def base_label(self):
-#        return self._base_label
-
-#    def polygon(self, lab):
-#        p = self._pdict.get(lab)
-#        if p is None:
-#            return self._s.polygon(lab)
-#        return p
-
-#    def opposite_edge(self, p, e):
-#        edge = self._gdict.get((p,e))
-#        if edge is None:
-#            return self._s.opposite_edge(p,e)
-#        return edge
+        return SurfaceMappingComposition(other, self)
+
+    def __rmul__(self, other):
+        return SurfaceMappingComposition(self, other)
 
-#    def is_finite(self):
-#        return self._is_finite
 
 class SurfaceMappingComposition(SurfaceMapping):
     r"""
     Composition of two mappings between surfaces.
     """
-    
+
     def __init__(self, mapping1, mapping2):
         r"""
         Represent the mapping of mapping1 followed by mapping2.
         """
         if mapping1.codomain() != mapping2.domain():
-            raise ValueError("Codomain of mapping1 must be equal to the domain of mapping2")
+            raise ValueError(
+                "Codomain of mapping1 must be equal to the domain of mapping2"
+            )
         self._m1 = mapping1
         self._m2 = mapping2
         SurfaceMapping.__init__(self, self._m1.domain(), self._m2.codomain())
 
-    def push_vector_forward(self,tangent_vector):
+    def push_vector_forward(self, tangent_vector):
         r"""Applies the mapping to the provided vector."""
-        return self._m2.push_vector_forward(self._m1.push_vector_forward(tangent_vector))
+        return self._m2.push_vector_forward(
+            self._m1.push_vector_forward(tangent_vector)
+        )
 
-    def pull_vector_back(self,tangent_vector):
+    def pull_vector_back(self, tangent_vector):
         r"""Applies the inverse of the mapping to the provided vector."""
         return self._m1.pull_vector_back(self._m2.pull_vector_back(tangent_vector))
 
     def factors(self):
         r"""
         Return the two factors of this surface mapping as a pair (f,g),
         where the original map is f o g.
         """
         return self._m2, self._m1
 
+
 class IdentityMapping(SurfaceMapping):
     r"""
     Construct an identity map between two "equal" surfaces.
     """
+
     def __init__(self, domain, codomain):
         SurfaceMapping.__init__(self, domain, codomain)
 
-    def push_vector_forward(self,tangent_vector):
+    def push_vector_forward(self, tangent_vector):
         r"""Applies the mapping to the provided vector."""
         ring = tangent_vector.bundle().base_ring()
-        return self._codomain.tangent_vector( \
-            tangent_vector.polygon_label(), \
-            tangent_vector.point(), \
-            tangent_vector.vector(), \
-            ring = ring)
+        return self._codomain.tangent_vector(
+            tangent_vector.polygon_label(),
+            tangent_vector.point(),
+            tangent_vector.vector(),
+            ring=ring,
+        )
 
-    def pull_vector_back(self,tangent_vector):
+    def pull_vector_back(self, tangent_vector):
         r"""Applies the pullback mapping to the provided vector."""
         ring = tangent_vector.bundle().base_ring()
-        return self._domain.tangent_vector( \
-            tangent_vector.polygon_label(), \
-            tangent_vector.point(), \
-            tangent_vector.vector(), \
-            ring = ring)
-
-class MatrixListDeformedSurface(Surface):
-    r"""
-    Apply a different matrix to each polygon in the surface. 
-    Here matrix_function is a python function mapping labels to 2x2 matrices with positive determinant.
-    """
-    def __init__(self, surface, matrix_function, ring=None):
-        self._s=surface
-        self._m=matrix_function
-        if ring is None:
-            self._base_ring = self._s.base_ring()
-        else:
-            self._base_ring=ring
-        self._P = ConvexPolygons(self._base_ring)
-        Surface.__init__(self)
-
-    def base_ring(self):
-        return self._base_ring
-
-    def base_label(self):
-        return self._s.base_label()
-
-    def polygon(self, lab):
-        p = self._s.polygon(lab)
-        edges = [ self._m(lab) * p.edge(e) for e in range(p.num_edges())]
-        return self._P(edges)
+        return self._domain.tangent_vector(
+            tangent_vector.polygon_label(),
+            tangent_vector.point(),
+            tangent_vector.vector(),
+            ring=ring,
+        )
 
-    def opposite_edge(self, p, e):
-        return self._s.opposite_edge(p,e)
-
-    def is_finite(self):
-        return self._s.is_finite()
-
-class MatrixListDeformedSurfaceMapping(SurfaceMapping):
-    r"""
-    This mapping applies a possibly different linear matrix to each polygon.
-    The matrix is determined by the matrix_function which should be a python
-    object.
-    """
-    def __init__(self, s, matrix_function, ring=None):
-        codomain = MatrixListDeformedSurface(s,matrix_function,ring = ring)
-        self._m=matrix_function
-        SurfaceMapping.__init__(self, s, codomain)
-
-    def push_vector_forward(self,tangent_vector):
-        label = tangent_vector.polygon_label()
-        m = self._m(label)
-        return self.codomain().tangent_vector(
-                label, \
-                m*tangent_vector.point(), \
-                m*tangent_vector.vector())
-
-    def pull_vector_back(self,tangent_vector):
-        label = tangent_vector.polygon_label()
-        im = ~self._m(label)
-        return self.domain().tangent_vector(
-                label, \
-                im*tangent_vector.point(), \
-                im*tangent_vector.vector())
 
 class SimilarityJoinPolygonsMapping(SurfaceMapping):
     r"""
     Return a SurfaceMapping joining two polygons together along the edge provided to the constructor.
 
     EXAMPLES::
 
-        sage: from flatsurf.geometry.surface import Surface_list
-        sage: from flatsurf.geometry.translation_surface import TranslationSurface
-        sage: from flatsurf.geometry.polygon import ConvexPolygons
-        sage: P = ConvexPolygons(QQ)
-        sage: s0=Surface_list(base_ring=QQ)
-        sage: s0.add_polygon(P([(1,0),(0,1),(-1,-1)])) # gets label=0
+        sage: from flatsurf import MutableOrientedSimilaritySurface, Polygon
+        sage: s = MutableOrientedSimilaritySurface(QQ)
+        sage: s.add_polygon(Polygon(edges=[(1,0),(0,1),(-1,-1)]))
         0
-        sage: s0.add_polygon(P([(-1,0),(0,-1),(1,1)])) # gets label=1
+        sage: s.add_polygon(Polygon(edges=[(-1,0),(0,-1),(1,1)]))
         1
-        sage: s0.change_polygon_gluings(0,[(1,0),(1,1),(1,2)])
-        sage: s0.set_immutable()
-        sage: s=TranslationSurface(s0)
-        sage: from flatsurf.geometry.mappings import *
-        sage: m=SimilarityJoinPolygonsMapping(s,0,2)
+        sage: s.glue((0, 0), (1, 0))
+        sage: s.glue((0, 1), (1, 1))
+        sage: s.glue((0, 2), (1, 2))
+        sage: s.set_immutable()
+
+        sage: from flatsurf.geometry.mappings import SimilarityJoinPolygonsMapping
+        sage: m=SimilarityJoinPolygonsMapping(s, 0, 2)
         sage: s2=m.codomain()
-        sage: for label,polygon in s2.label_iterator(polygons=True):
-        ....:     print("Polygon "+str(label)+" is "+str(polygon)+".")
-        Polygon 0 is Polygon: (0, 0), (1, 0), (1, 1), (0, 1).
-        sage: for label,edge in s2.edge_iterator():
-        ....:     print(str((label,edge))+" is glued to "+str(s2.opposite_edge(label,edge))+".")
-        (0, 0) is glued to (0, 2).
-        (0, 1) is glued to (0, 3).
-        (0, 2) is glued to (0, 0).
-        (0, 3) is glued to (0, 1).
+        sage: s2.labels()
+        (0,)
+        sage: s2.polygons()
+        (Polygon(vertices=[(0, 0), (1, 0), (1, 1), (0, 1)]),)
+        sage: s2.gluings()
+        (((0, 0), (0, 2)), ((0, 1), (0, 3)), ((0, 2), (0, 0)), ((0, 3), (0, 1)))
+
     """
+
     def __init__(self, s, p1, e1):
         r"""
         Join polygon with label p1 of s to polygon sharing edge e1.
         """
         if s.is_mutable():
-            raise ValueError("Can only construct SimilarityJoinPolygonsMapping for immutable surfaces.")
-
-        ss2=s.copy(lazy=True,mutable=True)
-        s2=ss2.underlying_surface()
-
-        poly1=s.polygon(p1)
-        p2,e2 = s.opposite_edge(p1,e1)
-        poly2=s.polygon(p2)
-        t=s.edge_transformation(p2, e2)
-        dt=t.derivative()
+            raise ValueError(
+                "Can only construct SimilarityJoinPolygonsMapping for immutable surfaces."
+            )
+
+        from flatsurf.geometry.surface import MutableOrientedSimilaritySurface
+
+        ss2 = MutableOrientedSimilaritySurface.from_surface(s)
+        s2 = ss2
+
+        poly1 = s.polygon(p1)
+        p2, e2 = s.opposite_edge(p1, e1)
+        poly2 = s.polygon(p2)
+        t = s.edge_transformation(p2, e2)
+        dt = t.derivative()
         vs = []  # actually stores new edges...
-        edge_map={} # Store the pairs for the old edges.
+        edge_map = {}  # Store the pairs for the old edges.
         for i in range(e1):
-            edge_map[len(vs)]=(p1,i)
+            edge_map[len(vs)] = (p1, i)
             vs.append(poly1.edge(i))
-        ne=poly2.num_edges()
-        for i in range(1,ne):
-            ee=(e2+i)%ne
-            edge_map[len(vs)]=(p2,ee)
-            vs.append(dt * poly2.edge( ee ))
-        for i in range(e1+1, poly1.num_edges()):
-            edge_map[len(vs)]=(p1,i)
+        ne = len(poly2.vertices())
+        for i in range(1, ne):
+            ee = (e2 + i) % ne
+            edge_map[len(vs)] = (p2, ee)
+            vs.append(dt * poly2.edge(ee))
+        for i in range(e1 + 1, len(poly1.vertices())):
+            edge_map[len(vs)] = (p1, i)
             vs.append(poly1.edge(i))
 
-        inv_edge_map={}
-        for key, value in iteritems(edge_map):
-            inv_edge_map[value]=(p1,key)
+        inv_edge_map = {}
+        for key, value in edge_map.items():
+            inv_edge_map[value] = (p1, key)
 
-        if s.base_label()==p2:
+        if p2 in s.roots():
             # The polygon with the base label is being removed.
-            s2.change_base_label(p1)
-        
-        s2.change_polygon(p1, ConvexPolygons(s.base_ring())(vs))
-        
+            s2.set_roots(tuple(p1 if label == p2 else label for label in s.roots()))
+
+        s2.remove_polygon(p1)
+        from flatsurf import Polygon
+
+        s2.add_polygon(Polygon(edges=vs, base_ring=s.base_ring()), label=p1)
+
         for i in range(len(vs)):
-            p3,e3 = edge_map[i]
-            p4,e4 = s.opposite_edge(p3,e3)
-            if p4 == p1 or p4 == p2: 
-                pp,ee = inv_edge_map[(p4,e4)]
-                s2.change_edge_gluing(p1,i,pp,ee)
+            p3, e3 = edge_map[i]
+            p4, e4 = s.opposite_edge(p3, e3)
+            if p4 == p1 or p4 == p2:
+                pp, ee = inv_edge_map[(p4, e4)]
+                s2.glue((p1, i), (pp, ee))
             else:
-                s2.change_edge_gluing(p1,i,p4,e4)
+                s2.glue((p1, i), (p4, e4))
 
+        s2.remove_polygon(p2)
         s2.set_immutable()
-        
-        self._saved_label=p1
-        self._removed_label=p2
+
+        self._saved_label = p1
+        self._removed_label = p2
         self._remove_map = t
         self._remove_map_derivative = dt
-        self._glued_edge=e1
+        self._glued_edge = e1
         SurfaceMapping.__init__(self, s, ss2)
 
     def removed_label(self):
         r"""
         Return the label that was removed in the joining process.
         """
         return self._removed_label
 
     def glued_vertices(self):
         r"""
         Return the vertices of the newly glued polygon which bound the diagonal formed by the glue.
         """
-        return (self._glued_edge,self._glued_edge+self._domain.polygon(self._removed_label).num_edges())
+        return (
+            self._glued_edge,
+            self._glued_edge
+            + len(self._domain.polygon(self._removed_label).vertices()),
+        )
 
-    def push_vector_forward(self,tangent_vector):
+    def push_vector_forward(self, tangent_vector):
         r"""Applies the mapping to the provided vector."""
         ring = tangent_vector.bundle().base_ring()
         if tangent_vector.polygon_label() == self._removed_label:
-            return self._codomain.tangent_vector( \
-                self._saved_label, \
-                self._remove_map(tangent_vector.point()), \
-                self._remove_map_derivative*tangent_vector.vector(), \
-                ring = ring)
+            return self._codomain.tangent_vector(
+                self._saved_label,
+                self._remove_map(tangent_vector.point()),
+                self._remove_map_derivative * tangent_vector.vector(),
+                ring=ring,
+            )
         else:
-            return self._codomain.tangent_vector( \
-                tangent_vector.polygon_label(), \
-                tangent_vector.point(), \
-                tangent_vector.vector(), \
-                ring = ring)
+            return self._codomain.tangent_vector(
+                tangent_vector.polygon_label(),
+                tangent_vector.point(),
+                tangent_vector.vector(),
+                ring=ring,
+            )
 
-    def pull_vector_back(self,tangent_vector):
+    def pull_vector_back(self, tangent_vector):
         r"""
         Applies the inverse of the mapping to the provided vector.
         """
         ring = tangent_vector.bundle().base_ring()
         if tangent_vector.polygon_label() == self._saved_label:
-            p=tangent_vector.point()
-            v=self._domain.polygon(self._saved_label).vertex(self._glued_edge)
-            e=self._domain.polygon(self._saved_label).edge(self._glued_edge)
-            from flatsurf.geometry.polygon import wedge_product
-            wp = wedge_product(p-v,e)
+            p = tangent_vector.point()
+            v = self._domain.polygon(self._saved_label).vertex(self._glued_edge)
+            e = self._domain.polygon(self._saved_label).edge(self._glued_edge)
+            from flatsurf.geometry.euclidean import ccw
+
+            wp = ccw(p - v, e)
             if wp > 0:
                 # in polygon with the removed label
-                return self.domain().tangent_vector( \
-                    self._removed_label, \
-                    (~ self._remove_map)(tangent_vector.point()), \
-                    (~ self._remove_map_derivative)*tangent_vector.vector(), \
-                    ring = ring)
+                return self.domain().tangent_vector(
+                    self._removed_label,
+                    (~self._remove_map)(tangent_vector.point()),
+                    (~self._remove_map_derivative) * tangent_vector.vector(),
+                    ring=ring,
+                )
             if wp < 0:
                 # in polygon with the removed label
-                return self.domain().tangent_vector( \
-                    self._saved_label, \
-                    tangent_vector.point(), \
-                    tangent_vector.vector(), \
-                    ring = ring)
+                return self.domain().tangent_vector(
+                    self._saved_label,
+                    tangent_vector.point(),
+                    tangent_vector.vector(),
+                    ring=ring,
+                )
             # Otherwise wp==0
             w = tangent_vector.vector()
-            wp = wedge_product(w,e)
+            wp = ccw(w, e)
             if wp > 0:
                 # in polygon with the removed label
-                return self.domain().tangent_vector( \
-                    self._removed_label, \
-                    (~ self._remove_map)(tangent_vector.point()), \
-                    (~ self._remove_map_derivative)*tangent_vector.vector(), \
-                    ring = ring)
-            return self.domain().tangent_vector( \
-                self._saved_label, \
-                tangent_vector.point(), \
-                tangent_vector.vector(), \
-                ring = ring)
+                return self.domain().tangent_vector(
+                    self._removed_label,
+                    (~self._remove_map)(tangent_vector.point()),
+                    (~self._remove_map_derivative) * tangent_vector.vector(),
+                    ring=ring,
+                )
+            return self.domain().tangent_vector(
+                self._saved_label,
+                tangent_vector.point(),
+                tangent_vector.vector(),
+                ring=ring,
+            )
         else:
-            return self._domain.tangent_vector( \
-                tangent_vector.polygon_label(), \
-                tangent_vector.point(), \
-                tangent_vector.vector(), \
-                ring = ring)
+            return self._domain.tangent_vector(
+                tangent_vector.polygon_label(),
+                tangent_vector.point(),
+                tangent_vector.vector(),
+                ring=ring,
+            )
+
 
 class SplitPolygonsMapping(SurfaceMapping):
     r"""
     Class for cutting a polygon along a diagonal.
-    
+
     EXAMPLES::
 
-        sage: from flatsurf import *
+        sage: from flatsurf import translation_surfaces
         sage: s=translation_surfaces.veech_2n_gon(4)
         sage: from flatsurf.geometry.mappings import SplitPolygonsMapping
         sage: m = SplitPolygonsMapping(s,0,0,2)
         sage: s2=m.codomain()
         sage: TestSuite(s2).run()
-        sage: for pair in s2.label_iterator(polygons=True):
-        ....:     print(pair)
-        (0, Polygon: (0, 0), (1/2*a + 1, 1/2*a), (1/2*a + 1, 1/2*a + 1), (1, a + 1), (0, a + 1), (-1/2*a, 1/2*a + 1), (-1/2*a, 1/2*a))
-        (ExtraLabel(0), Polygon: (0, 0), (-1/2*a - 1, -1/2*a), (-1/2*a, -1/2*a))
-        sage: for glue in s2.edge_iterator(gluings=True):
-        ....:     print(glue)
-        ((0, 0), (ExtraLabel(0), 0))
-        ((0, 1), (0, 5))
-        ((0, 2), (0, 6))
-        ((0, 3), (ExtraLabel(0), 1))
-        ((0, 4), (ExtraLabel(0), 2))
-        ((0, 5), (0, 1))
-        ((0, 6), (0, 2))
-        ((ExtraLabel(0), 0), (0, 0))
-        ((ExtraLabel(0), 1), (0, 3))
-        ((ExtraLabel(0), 2), (0, 4))
+        sage: s2.labels()
+        (0, 1)
+        sage: s2.polygons()
+        (Polygon(vertices=[(0, 0), (1/2*a + 1, 1/2*a), (1/2*a + 1, 1/2*a + 1), (1, a + 1), (0, a + 1), (-1/2*a, 1/2*a + 1), (-1/2*a, 1/2*a)]), Polygon(vertices=[(0, 0), (-1/2*a - 1, -1/2*a), (-1/2*a, -1/2*a)]))
+        sage: s2.gluings()
+        (((0, 0), (1, 0)), ((0, 1), (0, 5)), ((0, 2), (0, 6)), ((0, 3), (1, 1)), ((0, 4), (1, 2)), ((0, 5), (0, 1)), ((0, 6), (0, 2)), ((1, 0), (0, 0)), ((1, 1), (0, 3)), ((1, 2), (0, 4)))
+
     """
-    
-    def __init__(self, s, p, v1, v2, new_label = None):
+
+    def __init__(self, s, p, v1, v2, new_label=None):
         r"""
         Split the polygon with label p of surface s along the diagonal joining vertex v1 to vertex v2.
-        
+
         Warning: We do not ensure that new_label is not already in the list of labels unless it is None (as by default).
         """
         if s.is_mutable():
             raise ValueError("The surface should be immutable.")
 
-        poly=s.polygon(p)
-        ne=poly.num_edges()
-        if v1<0 or v2<0 or v1>=ne or v2>=ne:
-            raise ValueError('Provided vertices out of bounds.')
-        if abs(v1-v2)<=1 or abs(v1-v2)>=ne-1:
-            raise ValueError('Provided diagonal is not a diagonal.')
-        if v2<v1:
-            temp=v1
-            v1=v2
-            v2=temp
-            
-        newvertices1=[poly.vertex(v2)-poly.vertex(v1)]
-        for i in range(v2, v1+ne):
-            newvertices1.append(poly.edge(i))
-        newpoly1 = ConvexPolygons(s.base_ring())(newvertices1)
-        
-        newvertices2=[poly.vertex(v1)-poly.vertex(v2)]
-        for i in range(v1,v2):
-            newvertices2.append(poly.edge(i))
-        newpoly2 = ConvexPolygons(s.base_ring())(newvertices2)
-
-        ss2 = s.copy(mutable=True,lazy=True)
-        s2 = ss2.underlying_surface()
-        s2.change_polygon(p,newpoly1)
+        poly = s.polygon(p)
+        ne = len(poly.vertices())
+        if v1 < 0 or v2 < 0 or v1 >= ne or v2 >= ne:
+            raise ValueError("Provided vertices out of bounds.")
+        if abs(v1 - v2) <= 1 or abs(v1 - v2) >= ne - 1:
+            raise ValueError("Provided diagonal is not a diagonal.")
+        if v2 < v1:
+            temp = v1
+            v1 = v2
+            v2 = temp
+
+        newedges1 = [poly.vertex(v2) - poly.vertex(v1)]
+        for i in range(v2, v1 + ne):
+            newedges1.append(poly.edge(i))
+
+        from flatsurf import Polygon
+
+        newpoly1 = Polygon(edges=newedges1, base_ring=s.base_ring())
+
+        newedges2 = [poly.vertex(v1) - poly.vertex(v2)]
+        for i in range(v1, v2):
+            newedges2.append(poly.edge(i))
+        newpoly2 = Polygon(edges=newedges2, base_ring=s.base_ring())
+
+        from flatsurf.geometry.surface import MutableOrientedSimilaritySurface
+
+        ss2 = MutableOrientedSimilaritySurface.from_surface(s)
+        s2 = ss2
+        s2.remove_polygon(p)
+        s2.add_polygon(newpoly1, label=p)
         new_label = s2.add_polygon(newpoly2, label=new_label)
 
-        old_to_new_labels={}
+        old_to_new_labels = {}
         for i in range(ne):
-            if i<v1:
-                old_to_new_labels[i]=(p,i+ne-v2+1)
-            elif i<v2:
-                old_to_new_labels[i]=(new_label,i-v1+1)
-            else: # i>=v2
-                old_to_new_labels[i]=(p,i-v2+1)
-        new_to_old_labels={}
-        for i,pair in iteritems(old_to_new_labels):
-            new_to_old_labels[pair]=i
+            if i < v1:
+                old_to_new_labels[i] = (p, i + ne - v2 + 1)
+            elif i < v2:
+                old_to_new_labels[i] = (new_label, i - v1 + 1)
+            else:  # i>=v2
+                old_to_new_labels[i] = (p, i - v2 + 1)
+        new_to_old_labels = {}
+        for i, pair in old_to_new_labels.items():
+            new_to_old_labels[pair] = i
 
         # This glues the split polygons together.
-        s2.change_edge_gluing(p,0,new_label,0)
+        s2.glue((p, 0), (new_label, 0))
         for e in range(ne):
-            ll,ee = old_to_new_labels[e]
-            lll,eee = s.opposite_edge(p,e)
+            ll, ee = old_to_new_labels[e]
+            lll, eee = s.opposite_edge(p, e)
             if lll == p:
-                gl,ge = old_to_new_labels[eee]
-                s2.change_edge_gluing(ll,ee,gl,ge)
+                gl, ge = old_to_new_labels[eee]
+                s2.glue((ll, ee), (gl, ge))
             else:
-                s2.change_edge_gluing(ll,ee,lll,eee)
-        
+                s2.glue((ll, ee), (lll, eee))
+
         s2.set_immutable()
-        
-        self._p=p
-        self._v1=v1
-        self._v2=v2
-        self._new_label=new_label
+
+        self._p = p
+        self._v1 = v1
+        self._v2 = v2
+        self._new_label = new_label
         from flatsurf.geometry.similarity import SimilarityGroup
+
         TG = SimilarityGroup(s.base_ring())
         self._tp = TG(-s.polygon(p).vertex(v1))
         self._tnew_label = TG(-s.polygon(p).vertex(v2))
         SurfaceMapping.__init__(self, s, ss2)
 
-    def push_vector_forward(self,tangent_vector):
+    def push_vector_forward(self, tangent_vector):
         r"""Applies the mapping to the provided vector."""
         ring = tangent_vector.bundle().base_ring()
         if tangent_vector.polygon_label() == self._p:
-            point=tangent_vector.point()
-            vertex1=self._domain.polygon(self._p).vertex(self._v1)
-            vertex2=self._domain.polygon(self._p).vertex(self._v2)
+            point = tangent_vector.point()
+            vertex1 = self._domain.polygon(self._p).vertex(self._v1)
+            vertex2 = self._domain.polygon(self._p).vertex(self._v2)
+
+            from flatsurf.geometry.euclidean import ccw
 
-            wp = wedge_product(vertex2-vertex1,point-vertex1)
+            wp = ccw(vertex2 - vertex1, point - vertex1)
 
             if wp > 0:
                 # in new polygon 1
-                return self.codomain().tangent_vector( \
-                    self._p, \
-                    self._tp(tangent_vector.point()), \
-                    tangent_vector.vector(), \
-                    ring = ring)
+                return self.codomain().tangent_vector(
+                    self._p,
+                    self._tp(tangent_vector.point()),
+                    tangent_vector.vector(),
+                    ring=ring,
+                )
             if wp < 0:
                 # in new polygon 2
-                return self.codomain().tangent_vector( \
-                    self._new_label, \
-                    self._tnew_label(tangent_vector.point()), \
-                    tangent_vector.vector(), \
-                    ring = ring)
+                return self.codomain().tangent_vector(
+                    self._new_label,
+                    self._tnew_label(tangent_vector.point()),
+                    tangent_vector.vector(),
+                    ring=ring,
+                )
 
             # Otherwise wp==0
             w = tangent_vector.vector()
-            wp = wedge_product(vertex2-vertex1,w)
+            wp = ccw(vertex2 - vertex1, w)
             if wp > 0:
                 # in new polygon 1
-                return self.codomain().tangent_vector( \
-                    self._p, \
-                    self._tp(tangent_vector.point()), \
-                    tangent_vector.vector(), \
-                    ring = ring)
+                return self.codomain().tangent_vector(
+                    self._p,
+                    self._tp(tangent_vector.point()),
+                    tangent_vector.vector(),
+                    ring=ring,
+                )
             # in new polygon 2
-            return self.codomain().tangent_vector( \
-                self._new_label, \
-                self._tnew_label(tangent_vector.point()), \
-                tangent_vector.vector(), \
-                ring = ring)
+            return self.codomain().tangent_vector(
+                self._new_label,
+                self._tnew_label(tangent_vector.point()),
+                tangent_vector.vector(),
+                ring=ring,
+            )
         else:
             # Not in a polygon that was changed. Just copy the data.
-            return self._codomain.tangent_vector( \
-                tangent_vector.polygon_label(), \
-                tangent_vector.point(), \
-                tangent_vector.vector(), \
-                ring = ring)
-
+            return self._codomain.tangent_vector(
+                tangent_vector.polygon_label(),
+                tangent_vector.point(),
+                tangent_vector.vector(),
+                ring=ring,
+            )
 
-    def pull_vector_back(self,tangent_vector):
+    def pull_vector_back(self, tangent_vector):
         r"""Applies the pullback mapping to the provided vector."""
         ring = tangent_vector.bundle().base_ring()
         if tangent_vector.polygon_label() == self._p:
-            return self._domain.tangent_vector( \
-                self._p, \
-                (~ self._tp)(tangent_vector.point()), \
-                tangent_vector.vector(), \
-                ring = ring)
+            return self._domain.tangent_vector(
+                self._p,
+                (~self._tp)(tangent_vector.point()),
+                tangent_vector.vector(),
+                ring=ring,
+            )
         elif tangent_vector.polygon_label() == self._new_label:
-            return self._domain.tangent_vector( \
-                self._p, \
-                (~ self._tnew_label)(tangent_vector.point()), \
-                tangent_vector.vector(), \
-                ring = ring)
+            return self._domain.tangent_vector(
+                self._p,
+                (~self._tnew_label)(tangent_vector.point()),
+                tangent_vector.vector(),
+                ring=ring,
+            )
         else:
             # Not in a polygon that was changed. Just copy the data.
-            return self._domain.tangent_vector( \
-                tangent_vector.polygon_label(), \
-                tangent_vector.point(), \
-                tangent_vector.vector(), \
-                ring = ring)
+            return self._domain.tangent_vector(
+                tangent_vector.polygon_label(),
+                tangent_vector.point(),
+                tangent_vector.vector(),
+                ring=ring,
+            )
+
 
 def subdivide_a_polygon(s):
     r"""
     Return a SurfaceMapping which cuts one polygon along a diagonal or None if the surface is triangulated.
     """
-    from flatsurf.geometry.polygon import wedge_product
-    for l,poly in s.label_iterator(polygons=True):
-        n = poly.num_edges() 
-        if n>3:
+    from flatsurf.geometry.euclidean import ccw
+
+    for label, poly in zip(s.labels(), s.polygons()):
+        n = len(poly.vertices())
+        if n > 3:
             for i in range(n):
-                e1=poly.edge(i)
-                e2=poly.edge((i+1)%n)
-                if wedge_product(e1,e2) != 0:
-                    return SplitPolygonsMapping(s,l,i, (i+2)%n)
-            raise ValueError("Unable to triangulate polygon with label "+str(l)+\
-                ": "+str(poly))
+                e1 = poly.edge(i)
+                e2 = poly.edge((i + 1) % n)
+                if ccw(e1, e2) != 0:
+                    return SplitPolygonsMapping(s, label, i, (i + 2) % n)
+            raise ValueError(
+                "Unable to triangulate polygon with label "
+                + str(label)
+                + ": "
+                + str(poly)
+            )
     return None
 
 
 def triangulation_mapping(s):
-    r"""Return a  SurfaceMapping triangulating the provided surface.
-    
+    r"""
+    Return a SurfaceMapping triangulating ``s``.
+
     EXAMPLES::
 
-        sage: from flatsurf import *
+        sage: from flatsurf import translation_surfaces
         sage: s=translation_surfaces.veech_2n_gon(4)
-        sage: from flatsurf.geometry.mappings import *
+        sage: from flatsurf.geometry.mappings import triangulation_mapping
         sage: m=triangulation_mapping(s)
         sage: s2=m.codomain()
         sage: TestSuite(s2).run()
-        sage: for label,polygon in s2.label_iterator(polygons=True):
-        ....:     print(str(polygon))
-        Polygon: (0, 0), (-1/2*a, 1/2*a + 1), (-1/2*a, 1/2*a)
-        Polygon: (0, 0), (1/2*a, -1/2*a - 1), (1/2*a, 1/2*a)
-        Polygon: (0, 0), (-1/2*a - 1, -1/2*a - 1), (0, -1)
-        Polygon: (0, 0), (-1, -a - 1), (1/2*a, -1/2*a)
-        Polygon: (0, 0), (0, -a - 1), (1, 0)
-        Polygon: (0, 0), (-1/2*a - 1, -1/2*a), (-1/2*a, -1/2*a)
+        sage: s2.polygons()
+        (Polygon(vertices=[(0, 0), (-1/2*a, 1/2*a + 1), (-1/2*a, 1/2*a)]),
+         Polygon(vertices=[(0, 0), (1/2*a, -1/2*a - 1), (1/2*a, 1/2*a)]),
+         Polygon(vertices=[(0, 0), (-1/2*a - 1, -1/2*a - 1), (0, -1)]),
+         Polygon(vertices=[(0, 0), (-1, -a - 1), (1/2*a, -1/2*a)]),
+         Polygon(vertices=[(0, 0), (0, -a - 1), (1, 0)]),
+         Polygon(vertices=[(0, 0), (-1/2*a - 1, -1/2*a), (-1/2*a, -1/2*a)]))
+
     """
-    assert(s.is_finite())
-    m=subdivide_a_polygon(s)
+    if not s.is_finite_type():
+        raise NotImplementedError
+
+    m = subdivide_a_polygon(s)
     if m is None:
         return None
-    s1=m.codomain()
+    s1 = m.codomain()
     while True:
-        m2=subdivide_a_polygon(s1)
+        m2 = subdivide_a_polygon(s1)
         if m2 is None:
             return m
-        s1=m2.codomain()
-        m=SurfaceMappingComposition(m,m2)
+        s1 = m2.codomain()
+        m = SurfaceMappingComposition(m, m2)
     return m
 
-def flip_edge_mapping(s,p1,e1):
+
+def flip_edge_mapping(s, p1, e1):
     r"""
     Return a mapping whose domain is s which flips the provided edge.
     """
-    m1=SimilarityJoinPolygonsMapping(s,p1,e1)
-    v1,v2=m1.glued_vertices()
+    m1 = SimilarityJoinPolygonsMapping(s, p1, e1)
+    v1, v2 = m1.glued_vertices()
     removed_label = m1.removed_label()
-    m2=SplitPolygonsMapping(m1.codomain(), p1, (v1+1)%4, (v1+3)%4, new_label = removed_label)
-    return SurfaceMappingComposition(m1,m2)
+    m2 = SplitPolygonsMapping(
+        m1.codomain(), p1, (v1 + 1) % 4, (v1 + 3) % 4, new_label=removed_label
+    )
+    return SurfaceMappingComposition(m1, m2)
+
 
 def one_delaunay_flip_mapping(s):
     r"""
     Returns one delaunay flip, or none if no flips are needed.
     """
-    for p,poly in s.label_iterator(polygons=True):
-        for e in range(poly.num_edges()):
-            if s._edge_needs_flip(p,e):
-                return flip_edge_mapping(s,p,e)
+    for p, poly in zip(s.labels(), s.polygons()):
+        for e in range(len(poly.vertices())):
+            if s._delaunay_edge_needs_flip(p, e):
+                return flip_edge_mapping(s, p, e)
     return None
 
+
 def delaunay_triangulation_mapping(s):
     r"""
     Returns a mapping to a Delaunay triangulation or None if the surface already is Delaunay triangulated.
     """
-    assert(s.is_finite())
-    m=triangulation_mapping(s)
+    if not s.is_finite_type():
+        raise NotImplementedError
+
+    m = triangulation_mapping(s)
     if m is None:
-        s1=s
-    else: 
-        s1=m.codomain()
-    m1=one_delaunay_flip_mapping(s1)
+        s1 = s
+    else:
+        s1 = m.codomain()
+    m1 = one_delaunay_flip_mapping(s1)
     if m1 is None:
         return m
     if m is None:
-        m=m1
+        m = m1
     else:
-        m=SurfaceMappingComposition(m,m1)
-    s1=m1.codomain()
+        m = SurfaceMappingComposition(m, m1)
+    s1 = m1.codomain()
     while True:
-        m1=one_delaunay_flip_mapping(s1)
+        m1 = one_delaunay_flip_mapping(s1)
         if m1 is None:
             return m
-        s1=m1.codomain()
-        m=SurfaceMappingComposition(m,m1)
+        s1 = m1.codomain()
+        m = SurfaceMappingComposition(m, m1)
+
 
 def delaunay_decomposition_mapping(s):
     r"""
     Returns a mapping to a Delaunay decomposition or possibly None if the surface already is Delaunay.
     """
-    m=delaunay_triangulation_mapping(s)
+    m = delaunay_triangulation_mapping(s)
     if m is None:
-        s1=s
+        s1 = s
     else:
-        s1=m.codomain()
-    edge_vectors=[]
-    lc = s._label_comparator()
-    for p,poly in s1.label_iterator(polygons=True):
-        for e in range(poly.num_edges()):
-            pp,ee=s1.opposite_edge(p,e)
-            if (lc.lt(p,pp) or (p==pp and e<ee)) and s1._edge_needs_join(p,e):
-                edge_vectors.append( s1.tangent_vector(p,poly.vertex(e),poly.edge(e)) )
-    if len(edge_vectors)>0:
-        ev=edge_vectors.pop()
-        p,e=ev.edge_pointing_along()
-        m1=SimilarityJoinPolygonsMapping(s1,p,e)
-        s2=m1.codomain()
-        while len(edge_vectors)>0:
-            ev=edge_vectors.pop()
-            ev2=m1.push_vector_forward(ev)
-            p,e=ev2.edge_pointing_along()
-            mtemp=SimilarityJoinPolygonsMapping(s2,p,e)
-            m1=SurfaceMappingComposition(m1,mtemp)
-            s2=m1.codomain()
+        s1 = m.codomain()
+
+    joins = set()
+    edge_vectors = []
+
+    for p, poly in zip(s1.labels(), s1.polygons()):
+        for e in range(len(poly.vertices())):
+            pp, ee = s1.opposite_edge(p, e)
+            if (pp, ee) in joins:
+                continue
+            if s1._delaunay_edge_needs_join(p, e):
+                joins.add((p, e))
+                edge_vectors.append(s1.tangent_vector(p, poly.vertex(e), poly.edge(e)))
+
+    if len(edge_vectors) > 0:
+        ev = edge_vectors.pop()
+        p, e = ev.edge_pointing_along()
+        m1 = SimilarityJoinPolygonsMapping(s1, p, e)
+        s2 = m1.codomain()
+        while len(edge_vectors) > 0:
+            ev = edge_vectors.pop()
+            ev2 = m1.push_vector_forward(ev)
+            p, e = ev2.edge_pointing_along()
+            mtemp = SimilarityJoinPolygonsMapping(s2, p, e)
+            m1 = SurfaceMappingComposition(m1, mtemp)
+            s2 = m1.codomain()
         if m is None:
             return m1
         else:
-            return SurfaceMappingComposition(m,m1)
+            return SurfaceMappingComposition(m, m1)
     return m
-    
+
+
 def canonical_first_vertex(polygon):
     r"""
     Return the index of the vertex with smallest y-coordinate.
     If two vertices have the same y-coordinate, then the one with least x-coordinate is returned.
     """
-    best=0
-    best_pt=polygon.vertex(best)
-    for v in range(1,polygon.num_edges()):
-        pt=polygon.vertex(v)
-        if pt[1]<best_pt[1]:
-            best=v
-            best_pt=pt
-    if best==0:
-        if pt[1]==best_pt[1]:
+    best = 0
+    best_pt = polygon.vertex(best)
+    for v in range(1, len(polygon.vertices())):
+        pt = polygon.vertex(v)
+        if pt[1] < best_pt[1]:
+            best = v
+            best_pt = pt
+    if best == 0:
+        if pt[1] == best_pt[1]:
             return v
     return best
-   
+
+
 class CanonicalizePolygonsMapping(SurfaceMapping):
     r"""
     This is a mapping to a surface with the polygon vertices canonically determined.
     A canonical labeling is when the canonocal_first_vertex is the zero vertex.
     """
+
     def __init__(self, s):
         r"""
         Split the polygon with label p of surface s along the diagonal joining vertex v1 to vertex v2.
         """
-        if not s.is_finite():
+        if not s.is_finite_type():
             raise ValueError("Currently only works with finite surfaces.")
-        ring=s.base_ring()
+        ring = s.base_ring()
         from flatsurf.geometry.similarity import SimilarityGroup
+
         T = SimilarityGroup(ring)
-        P = ConvexPolygons(ring)
-        cv = {} # dictionary for canonical vertices
-        translations={} # translations bringing the canonical vertex to the origin.
-        s2 = Surface_dict(base_ring=ring)
-        for l,polygon in s.label_iterator(polygons=True):
-            cv[l]=cvcur=canonical_first_vertex(polygon)
-            newedges=[]
-            for i in range(polygon.num_edges()):
-                newedges.append(polygon.edge( (i+cvcur) % polygon.num_edges() ))
-            s2.add_polygon(P(newedges), label=l)
-            translations[l]=T( -polygon.vertex(cvcur) )
-        for l1,polygon in s.label_iterator(polygons=True):
-            for e1 in range(polygon.num_edges()):
-                l2,e2=s.opposite_edge(l1,e1)
-                ee1= (e1-cv[l1]+polygon.num_edges())%polygon.num_edges()
-                polygon2=s.polygon(l2)
-                ee2= (e2-cv[l2]+polygon2.num_edges())%polygon2.num_edges()
+        cv = {}  # dictionary for canonical vertices
+        translations = {}  # translations bringing the canonical vertex to the origin.
+        from flatsurf.geometry.surface import MutableOrientedSimilaritySurface
+
+        s2 = MutableOrientedSimilaritySurface(ring)
+        for label, polygon in zip(s.labels(), s.polygons()):
+            cv[label] = cvcur = canonical_first_vertex(polygon)
+            newedges = []
+            for i in range(len(polygon.vertices())):
+                newedges.append(polygon.edge((i + cvcur) % len(polygon.vertices())))
+
+            from flatsurf import Polygon
+
+            s2.add_polygon(Polygon(edges=newedges, base_ring=ring), label=label)
+            translations[label] = T(-polygon.vertex(cvcur))
+        for l1, polygon in zip(s.labels(), s.polygons()):
+            for e1 in range(len(polygon.vertices())):
+                l2, e2 = s.opposite_edge(l1, e1)
+                ee1 = (e1 - cv[l1] + len(polygon.vertices())) % len(polygon.vertices())
+                polygon2 = s.polygon(l2)
+                ee2 = (e2 - cv[l2] + len(polygon2.vertices())) % len(
+                    polygon2.vertices()
+                )
                 # newgluing.append( ( (l1,ee1),(l2,ee2) ) )
-                s2.change_edge_gluing(l1,ee1,l2,ee2)
-        s2.change_base_label(s.base_label())
+                s2.glue((l1, ee1), (l2, ee2))
+        s2.set_roots(s.roots())
         s2.set_immutable()
-        ss2=s.__class__(s2)
-        
-        self._cv=cv
-        self._translations=translations
+        ss2 = s2
+
+        self._cv = cv
+        self._translations = translations
 
         SurfaceMapping.__init__(self, s, ss2)
 
-    def push_vector_forward(self,tangent_vector):
+    def push_vector_forward(self, tangent_vector):
         r"""Applies the mapping to the provided vector."""
         ring = tangent_vector.bundle().base_ring()
-        l=tangent_vector.polygon_label()
-        return self.codomain().tangent_vector(l, \
-            self._translations[l](tangent_vector.point()), \
-            tangent_vector.vector(), \
-            ring = ring)
+        label = tangent_vector.polygon_label()
+        return self.codomain().tangent_vector(
+            label,
+            self._translations[label](tangent_vector.point()),
+            tangent_vector.vector(),
+            ring=ring,
+        )
 
-    def pull_vector_back(self,tangent_vector):
+    def pull_vector_back(self, tangent_vector):
         r"""Applies the pullback mapping to the provided vector."""
         ring = tangent_vector.bundle().base_ring()
-        l=tangent_vector.polygon_label()
-        return self.domain().tangent_vector(l, \
-            (~self._translations[l])(tangent_vector.point()), \
-            tangent_vector.vector(), \
-            ring = ring)
+        label = tangent_vector.polygon_label()
+        return self.domain().tangent_vector(
+            label,
+            (~self._translations[label])(tangent_vector.point()),
+            tangent_vector.vector(),
+            ring=ring,
+        )
+
 
 class ReindexMapping(SurfaceMapping):
     r"""
     Apply a dictionary to relabel the polygons.
     """
-    def __init__(self,s,relabler,new_base_label=None):
+
+    def __init__(self, s, relabler, new_base_label=None):
         r"""
         The parameters should be a surface and a dictionary which takes as input a label and produces a new label.
         """
-        if not s.is_finite():
-            raise ValueError("Currently only works with finite surfaces.""")
-        f = {} # map for labels going forward.
-        b = {} # map for labels going backward.
-        for l in s.label_iterator():
-            if l in relabler:
-                l2=relabler[l]
-                f[l]=l2
+        if not s.is_finite_type():
+            raise ValueError("Currently only works with finite surfaces." "")
+        f = {}  # map for labels going forward.
+        b = {}  # map for labels going backward.
+        for label in s.labels():
+            if label in relabler:
+                l2 = relabler[label]
+                f[label] = l2
                 if l2 in b:
-                    raise ValueError("Provided dictionary has two keys mapping to the same value. Or you are mapping to a label you didn't change.")
-                b[l2]=l
+                    raise ValueError(
+                        "Provided dictionary has two keys mapping to the same value. Or you are mapping to a label you didn't change."
+                    )
+                b[l2] = label
             else:
                 # If no key then don't change the label
-                f[l]=l
-                if l in b:
-                    raise ValueError("Provided dictionary has two keys mapping to the same value. Or you are mapping to a label you didn't change.")
-                b[l]=l
-
-        self._f=f
-        self._b=b
-        
-        if new_base_label==None:
-            if s.base_label() in f:                
-                new_base_label = f[s.base_label()]
+                f[label] = label
+                if label in b:
+                    raise ValueError(
+                        "Provided dictionary has two keys mapping to the same value. Or you are mapping to a label you didn't change."
+                    )
+                b[label] = label
+
+        self._f = f
+        self._b = b
+
+        if new_base_label is None:
+            if s.root() in f:
+                new_base_label = f[s.root()]
             else:
-                new_base_label = s.base_label()
-        s2=s.copy(mutable=True,lazy=True)
+                new_base_label = s.root()
+        from flatsurf.geometry.surface import MutableOrientedSimilaritySurface
+
+        s2 = MutableOrientedSimilaritySurface.from_surface(s)
         s2.relabel(relabler, in_place=True)
-        s2.underlying_surface().change_base_label(new_base_label)
-        
+        s2.set_roots([new_base_label])
+        s2.set_immutable()
+
         SurfaceMapping.__init__(self, s, s2)
-            
-    def push_vector_forward(self,tangent_vector):
+
+    def push_vector_forward(self, tangent_vector):
         r"""Applies the mapping to the provided vector."""
         # There is no change- we just move it to the new surface.
         ring = tangent_vector.bundle().base_ring()
-        return self.codomain().tangent_vector( \
-            self._f[tangent_vector.polygon_label()], \
-            tangent_vector.point(), \
-            tangent_vector.vector(), \
-            ring = ring)
+        return self.codomain().tangent_vector(
+            self._f[tangent_vector.polygon_label()],
+            tangent_vector.point(),
+            tangent_vector.vector(),
+            ring=ring,
+        )
 
-    def pull_vector_back(self,tangent_vector):
+    def pull_vector_back(self, tangent_vector):
         r"""Applies the pullback mapping to the provided vector."""
         ring = tangent_vector.bundle().base_ring()
-        return self.domain().tangent_vector( \
-            self._b[tangent_vector.polygon_label()], \
-            tangent_vector.point(), \
-            tangent_vector.vector(), \
-            ring = ring)
+        return self.domain().tangent_vector(
+            self._b[tangent_vector.polygon_label()],
+            tangent_vector.point(),
+            tangent_vector.vector(),
+            ring=ring,
+        )
+
 
 def my_sgn(val):
-    if val>0:
+    if val > 0:
         return 1
-    elif val<0:
+    elif val < 0:
         return -1
     else:
         return 0
 
-def polygon_compare(poly1,poly2):
+
+def polygon_compare(poly1, poly2):
     r"""
     Compare two polygons first by area, then by number of sides,
-    then by lexigraphical ording on edge vectors."""
+    then by lexicographical ordering on edge vectors."""
     # This should not be used is broken!!
-    #from sage.functions.generalized import sgn
-    res = my_sgn(-poly1.area()+poly2.area())
-    if res!=0:
+    # from sage.functions.generalized import sgn
+    res = my_sgn(-poly1.area() + poly2.area())
+    if res != 0:
         return res
-    res = my_sgn(poly1.num_edges()-poly2.num_edges())
-    if res!=0:
+    res = my_sgn(len(poly1.vertices()) - len(poly2.vertices()))
+    if res != 0:
         return res
-    ne=poly1.num_edges()
-    for i in range(0,ne-1):
+    ne = len(poly1.vertices())
+    for i in range(0, ne - 1):
         edge_diff = poly1.edge(i) - poly2.edge(i)
         res = my_sgn(edge_diff[0])
-        if res!=0:
+        if res != 0:
             return res
         res = my_sgn(edge_diff[1])
-        if res!=0:
+        if res != 0:
             return res
     return 0
-    
-def translation_surface_cmp(s1, s2):
-    r"""
-    Compare two finite surfaces. 
-    The surfaces will be considered equal if and only if there is a translation automorphism
-    respecting the polygons and the base_labels.
-    """
-    if not s1.is_finite() or not s2.is_finite():
-        raise NotImplementedError
-    lw1=s1.walker()
-    lw2=s2.walker()
-    try:
-        from itertools import zip_longest
-    except ImportError:
-        from itertools import izip_longest as zip_longest
-    for p1,p2 in zip_longest(lw1.polygon_iterator(), lw2.polygon_iterator()):
-        if p1 is None:
-            # s2 has more polygons
-            return -1
-        if p2 is None:
-            # s1 has more polygons
-            return 1
-        ret = polygon_compare(p1,p2)
-        if ret != 0:
-            return ret
-    # Polygons are identical. Compare edge gluings.
-    for pair1,pair2 in zip_longest(lw1.edge_iterator(), lw2.edge_iterator()):
-        l1,e1 = s1.opposite_edge(pair1)
-        l2,e2 = s2.opposite_edge(pair2)
-        num1 = lw1.label_to_number(l1)
-        num2 = lw2.label_to_number(l2)
-        ret = (num1 > num2) - (num1 < num2)
-        if ret!=0:
-            return ret
-        ret = (e1 > e2) - (e1 < e2)
-        if ret!=0:
-            return ret
-    return 0
+
 
 def canonicalize_translation_surface_mapping(s):
     r"""
     Return the translation surface in a canonical form.
-    
+
     EXAMPLES::
 
-        sage: from flatsurf import *
-        sage: s=translation_surfaces.octagon_and_squares().canonicalize()
+        sage: from flatsurf import translation_surfaces
+        sage: s = translation_surfaces.octagon_and_squares().canonicalize()
+
         sage: TestSuite(s).run()
+
         sage: a = s.base_ring().gen()  # a is the square root of 2.
 
-        sage: from flatsurf.geometry.mappings import *
+        sage: from flatsurf.geometry.half_dilation_surface import GL2RMapping
+        sage: from flatsurf.geometry.mappings import canonicalize_translation_surface_mapping
         sage: mat=Matrix([[1,2+a],[0,1]])
         sage: from flatsurf.geometry.half_dilation_surface import GL2RMapping
-        sage: m1=GL2RMapping(s,mat)
+        sage: m1=GL2RMapping(s, mat)
         sage: m2=canonicalize_translation_surface_mapping(m1.codomain())
         sage: m=m2*m1
-        sage: translation_surface_cmp(m.domain(),m.codomain())==0
-        True
+        sage: m.domain().cmp(m.codomain())
+        0
         sage: TestSuite(m.codomain()).run()
         sage: s=m.domain()
         sage: v=s.tangent_vector(0,(0,0),(1,1))
         sage: w=m.push_vector_forward(v)
         sage: print(w)
         SimilaritySurfaceTangentVector in polygon 0 based at (0, 0) with vector (a + 3, 1)
     """
-    from flatsurf.geometry.translation_surface import TranslationSurface
-    if not s.is_finite():
+    from flatsurf.geometry.categories import TranslationSurfaces
+
+    if not s.is_finite_type():
         raise NotImplementedError
-    if not isinstance(s,TranslationSurface):
+    if s not in TranslationSurfaces():
         raise ValueError("Only defined for TranslationSurfaces")
-    m1=delaunay_decomposition_mapping(s)
+    m1 = delaunay_decomposition_mapping(s)
     if m1 is None:
-        s2=s
+        s2 = s
     else:
-        s2=m1.codomain()
-    m2=CanonicalizePolygonsMapping(s2)
+        s2 = m1.codomain()
+    m2 = CanonicalizePolygonsMapping(s2)
     if m1 is None:
-        m=m2
+        m = m2
     else:
-        m=SurfaceMappingComposition(m1,m2)
-    s2=m.codomain()
+        m = SurfaceMappingComposition(m1, m2)
+    s2 = m.codomain()
+
+    # This is essentially copy & paste from canonicalize() from TranslationSurfaces()
+    from flatsurf.geometry.surface import MutableOrientedSimilaritySurface
 
-    s2copy=s2.copy(mutable=True)
-    ss=s2.copy(mutable=True)
-    labels={label for label in s2.label_iterator()}
-    labels.remove(s2.base_label())
+    s2copy = MutableOrientedSimilaritySurface.from_surface(s2)
+    ss = MutableOrientedSimilaritySurface.from_surface(s2)
+    labels = {label for label in s2.labels()}
     for label in labels:
-        ss.underlying_surface().change_base_label(label)
-        if ss.cmp(s2copy)>0:
-            s2copy.underlying_surface().change_base_label(label)
+        ss.set_roots([label])
+        if ss.cmp(s2copy) > 0:
+            s2copy.set_roots([label])
+
+    s2copy.set_immutable()
+
     # We now have the base_label correct.
-    # We will use the label walker to generate the canonical labeling of polygons.
-    w=s2copy.walker()
-    w.find_all_labels()
-
-    m3=ReindexMapping(s2,w.label_dictionary(),0)
-    return SurfaceMappingComposition(m,m3)
-    
+    # We will use the label walk to generate the canonical labeling of polygons.
+    labels = {label: i for (i, label) in enumerate(s2copy.labels())}
+
+    m3 = ReindexMapping(s2, labels, 0)
+    return SurfaceMappingComposition(m, m3)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/mega_wollmilchsau.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/mega_wollmilchsau.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,150 +1,174 @@
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
-
+# ****************************************************************************
+#  This file is part of sage-flatsurf.
+#
+#       Copyright (C) 2016-2019 Vincent Delecroix
+#                     2016-2019 W. Patrick Hooper
+#                          2023 Julian Rüth
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+# ****************************************************************************
 from sage.groups.group import Group
 from sage.categories.groups import Groups
 from sage.structure.unique_representation import UniqueRepresentation
 from sage.structure.element import MultiplicativeGroupElement
 from sage.algebras.quatalg.quaternion_algebra import QuaternionAlgebra
-from sage.rings.infinity import infinity
 from sage.rings.integer_ring import ZZ
 
-from .translation_surface import AbstractOrigami
+from flatsurf.geometry.origami import AbstractOrigami
+
+_Q = QuaternionAlgebra(-1, -1)
+_i, _j, _k = _Q.gens()
 
-_Q=QuaternionAlgebra(-1, -1)
-_i,_j,_k=_Q.gens()
 
 class MegaWollmilchsauGroupElement(MultiplicativeGroupElement):
-    
     @staticmethod
     def quat_to_tuple(r):
         r"""Convert an element in the quaternion algebra to a quadruple"""
-        if type(r)==type(1):
-            return (r,0,0,0)
+        if isinstance(r, int):
+            return (r, 0, 0, 0)
         else:
-            return (r[0],r[1],r[2],r[3])
-            
+            return (r[0], r[1], r[2], r[3])
+
     @staticmethod
-    def wedge(r1,r2):
+    def wedge(r1, r2):
         r"""Wedge two quaterions. Returns an integer."""
         x = MegaWollmilchsauGroupElement.quat_to_tuple(r1)
         y = MegaWollmilchsauGroupElement.quat_to_tuple(r2)
-        return -x[0]*y[3]+x[1]*y[2]-x[2]*y[1]+x[3]*y[0]
-    
+        return -x[0] * y[3] + x[1] * y[2] - x[2] * y[1] + x[3] * y[0]
+
     def __init__(self, parent, i, r, q):
         if parent is None:
             raise ValueError("The parent must be provided")
         # I should assert that the element lives in the domain of the group.
-        assert i in ZZ
-        assert r in _Q
+        if i not in ZZ:
+            raise ValueError
+        if r not in _Q:
+            raise ValueError
         # Actually q should be in {1,-1,-i,i,j,-j,k,-k}. I'm not testing for that.
-        assert q in _Q
+        if q not in _Q:
+            raise ValueError
         # There is one more condition. The group doesn't have full image...
-        self._i=i
-        self._r=r
-        self._q=q
-        self._parent=parent
-        MultiplicativeGroupElement.__init__(self,parent)
-        
+        self._i = i
+        self._r = r
+        self._q = q
+        self._parent = parent
+        MultiplicativeGroupElement.__init__(self, parent)
+
     def _repr_(self):
-        return "["+str(self._i)+", "+str(self._r)+", "+str(self._q)+"]"
+        return "[" + str(self._i) + ", " + str(self._r) + ", " + str(self._q) + "]"
 
     def _cmp_(self, other):
-        return (self._i > other._i - self._i < other._i) or \
-               (self._r > other._r - self._r < other._r) or \
-               (self._q > other._q - self._q < other._q)
-
-    def _mul_(self,m):
-        return MegaWollmilchsauGroupElement(self._parent,
-            self._i+m._i+MegaWollmilchsauGroupElement.wedge(self._r,self._q*m._r),
-            self._r+self._q*m._r, self._q*m._q)
+        return (
+            (self._i > other._i - self._i < other._i)
+            or (self._r > other._r - self._r < other._r)
+            or (self._q > other._q - self._q < other._q)
+        )
+
+    def _mul_(self, m):
+        return MegaWollmilchsauGroupElement(
+            self._parent,
+            self._i
+            + m._i
+            + MegaWollmilchsauGroupElement.wedge(self._r, self._q * m._r),
+            self._r + self._q * m._r,
+            self._q * m._q,
+        )
 
     def __invert__(self):
-        q1=~self._q
-        r1=-(q1 * self._r)
-        i1=-(self._i+MegaWollmilchsauGroupElement.wedge(r1,q1*self._r))
-        return MegaWollmilchsauGroupElement(self._parent,i1,r1,q1)
+        q1 = ~self._q
+        r1 = -(q1 * self._r)
+        i1 = -(self._i + MegaWollmilchsauGroupElement.wedge(r1, q1 * self._r))
+        return MegaWollmilchsauGroupElement(self._parent, i1, r1, q1)
 
-    def _div_(self,m):
+    def _div_(self, m):
         return self._mul_(m.__invert__())
 
     def __hash__(self):
-        return 67*hash(self._i)+23*hash(MegaWollmilchsauGroupElement.quat_to_tuple(self._r))-17*hash(MegaWollmilchsauGroupElement.quat_to_tuple(self._q))
+        return (
+            67 * hash(self._i)
+            + 23 * hash(MegaWollmilchsauGroupElement.quat_to_tuple(self._r))
+            - 17 * hash(MegaWollmilchsauGroupElement.quat_to_tuple(self._q))
+        )
+
 
 class MegaWollmilchsauGroup(UniqueRepresentation, Group):
     Element = MegaWollmilchsauGroupElement
 
     def _element_constructor_(self, *args, **kwds):
-        if len(args)!=1:
+        if len(args) != 1:
             return self.element_class(self, *args, **kwds)
         x = args[0]
         return self.element_class(self, x, **kwds)
 
     def __init__(self):
         Group.__init__(self, category=Groups().Infinite())
 
     def _repr_(self):
         return "MegaWollmilchsauGroup"
 
     def a(self):
-        return self.element_class(self,0,1,_i)
+        return self.element_class(self, 0, 1, _i)
 
     def b(self):
-        return self.element_class(self,0,1,_j)
+        return self.element_class(self, 0, 1, _j)
 
     def one(self):
-        return self.element_class(self,0,0,1)
+        return self.element_class(self, 0, 0, 1)
 
     def gens(self):
         return (self.a(), self.b())
 
     def is_abelian(self):
         return False
 
-    #def order(self):
-    #    return infinity
-
     def _an_element_(self):
         return self.a()
 
     def some_elements(self):
         return [self.a(), self.b()]
 
-    def _test_relations(self,**options):
-        a,b=self.gens()
-        e=self.one()
-        assert a**4==e
-        assert b**4==e
-        assert (a*b)**4==e
-        assert (a/b)**4==e
-        assert (a*a*b)**4==e
-        assert (a*a/b)**4==e
-        assert (a*b/a/b)**2!=e
-
-    #def cardinality(self):
-    #    return infinity
+    def _test_relations(self, **options):
+        tester = self._tester(**options)
+        a, b = self.gens()
+        e = self.one()
+        tester.assertEqual(a**4, e)
+        tester.assertEqual(b**4, e)
+        tester.assertEqual((a * b) ** 4, e)
+        tester.assertEqual((a / b) ** 4, e)
+        tester.assertEqual((a * a * b) ** 4, e)
+        tester.assertEqual((a * a / b) ** 4, e)
+        tester.assertNotEqual((a * b / a / b) ** 2, e)
 
 
 class MegaWollmilchsau(AbstractOrigami):
-
     def __init__(self):
-        self._G=self._domain=MegaWollmilchsauGroup()
-        self._a,self._b=self._G.gens()
-        self._ai=~self._a
-        self._bi=~self._b
+        self._G = self._domain = MegaWollmilchsauGroup()
+        self._a, self._b = self._G.gens()
+        self._ai = ~self._a
+        self._bi = ~self._b
 
     def up(self, label):
-        return self._b*label
+        return self._b * label
 
     def down(self, label):
-        return self._bi*label
+        return self._bi * label
 
     def right(self, label):
-        return self._a*label
+        return self._a * label
 
     def left(self, label):
-        return self._ai*label
+        return self._ai * label
 
     def _repr_(self):
         return "MegaWollmilchsau Origami"
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/polyhedra.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/polyhedra.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,395 +1,481 @@
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
-
+# ********************************************************************
+#  This file is part of sage-flatsurf.
+#
+#        Copyright (C) 2017-2020 W. Patrick Hooper
+#                      2017-2020 Vincent Delecroix
+#                           2023 Julian Rüth
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+# ********************************************************************
 from sage.rings.integer_ring import ZZ
 from sage.rings.rational_field import QQ
 from sage.rings.number_field.number_field import NumberField
 from sage.rings.qqbar import AA, number_field_elements_from_algebraics
 from sage.structure.sage_object import SageObject
 from sage.matrix.constructor import matrix
 from sage.modules.free_module_element import vector
 from sage.geometry.polyhedron.constructor import Polyhedron
 from sage.functions.other import sqrt
 
-from flatsurf.geometry.polygon import ConvexPolygons
-from flatsurf.geometry.surface import surface_list_from_polygons_and_gluings
-from flatsurf.geometry.cone_surface import ConeSurface
-from flatsurf.geometry.straight_line_trajectory import StraightLineTrajectory, SegmentInPolygon 
+from flatsurf.geometry.straight_line_trajectory import (
+    StraightLineTrajectory,
+    SegmentInPolygon,
+)
 from flatsurf.geometry.tangent_bundle import SimilaritySurfaceTangentVector
 
+
 class ConeSurfaceToPolyhedronMap(SageObject):
     r"""
-    A map sending objects defined on a ConeSurface built from a polyhedron to the polyhedron. Currently, this 
+    A map sending objects defined on a ConeSurface built from a polyhedron to the polyhedron. Currently, this
     works to send a trajectory to a list of points.
-    
+
     This class should not be called directly. You get an object of this type from polyhedron_to_cone_surface.
     """
+
     def __init__(self, cone_surface, polyhedron, mapping_data):
-        self._s=cone_surface
-        self._p=polyhedron
-        self._md=mapping_data
-    
-    def __call__(self,o):
+        self._s = cone_surface
+        self._p = polyhedron
+        self._md = mapping_data
+
+    def __call__(self, o):
         r"""
         This method is used to convert from an object on the cone surface to an object on the polyhedron.
-        
-        Currently works with 
+
+        Currently works with
         - StraightLineTrajectory -- returns the corresponding list of points on the polyhedron
         - SegmentInPolygon -- returns the corresponding pair of points on the polyhedron
         - SimilaritySurfaceTangentVector -- returns a pair of points corresponding to the image point and image of the tangent vector.
         """
         if isinstance(o, StraightLineTrajectory):
-            points=[]
+            points = []
             it = iter(o.segments())
             s = next(it)
             label = s.polygon_label()
-            points.append(self._md[label][0]+self._md[label][1]*s.start().point())
-            points.append(self._md[label][0]+self._md[label][1]*s.end().point())
+            points.append(self._md[label][0] + self._md[label][1] * s.start().point())
+            points.append(self._md[label][0] + self._md[label][1] * s.end().point())
             for s in it:
                 label = s.polygon_label()
-                points.append(self._md[label][0]+self._md[label][1]*s.end().point())
-            return points    
+                points.append(self._md[label][0] + self._md[label][1] * s.end().point())
+            return points
         if isinstance(o, SegmentInPolygon):
             # Return the pair of images of the endpoints.
             label = o.polygon_label()
-            return ( self._md[label][0]+self._md[label][1]*o.start().point(), \
-                     self._md[label][0]+self._md[label][1]*o.end().point() )
-        if isinstance(o,SimilaritySurfaceTangentVector):
+            return (
+                self._md[label][0] + self._md[label][1] * o.start().point(),
+                self._md[label][0] + self._md[label][1] * o.end().point(),
+            )
+        if isinstance(o, SimilaritySurfaceTangentVector):
             # Map to a pair of vectors conisting of the image of the basepoint and the image of the vector.
             label = o.polygon_label()
             point = o.point()
             vector = o.vector()
-            return (self._md[label][0]+self._md[label][1]*point, \
-                    self._md[label][1]*vector)
+            return (
+                self._md[label][0] + self._md[label][1] * point,
+                self._md[label][1] * vector,
+            )
         raise ValueError("Failed to recognize type of passed object")
-        
+
+    def __eq__(self, other):
+        r"""
+        Return whether this map is indistinguishable from ``other``.
+
+        EXAMPLES::
+
+            sage: from flatsurf.geometry.polyhedra import Polyhedron, polyhedron_to_cone_surface
+            sage: vertices=[]
+            sage: for i in range(3):
+            ....:     temp=vector([1 if k==i else 0 for k in range(3)])
+            ....:     for j in range(-1,3,2):
+            ....:         vertices.append(j*temp)
+            sage: octahedron=Polyhedron(vertices=vertices)
+            sage: surface, surface_to_octahedron = polyhedron_to_cone_surface(octahedron,scaling_factor=AA(1/sqrt(2)))  # long time (.5s)
+
+            sage: surface_to_octahedron == surface_to_octahedron  # long time (see above)
+            True
+
+        """
+        if not isinstance(other, ConeSurfaceToPolyhedronMap):
+            return False
+        return self._s == other._s and self._p == other._p and self._md == other._md
+
+    def __ne__(self, other):
+        r"""
+        Return whether this map is distinguishable from ``other``.
+
+        EXAMPLES::
+
+            sage: from flatsurf.geometry.polyhedra import Polyhedron, polyhedron_to_cone_surface
+            sage: vertices=[]
+            sage: for i in range(3):
+            ....:     temp=vector([1 if k==i else 0 for k in range(3)])
+            ....:     for j in range(-1,3,2):
+            ....:         vertices.append(j*temp)
+            sage: octahedron=Polyhedron(vertices=vertices)
+            sage: surface, surface_to_octahedron = polyhedron_to_cone_surface(octahedron,scaling_factor=AA(1/sqrt(2)))  # long time (.3s)
+
+            sage: surface_to_octahedron != surface_to_octahedron  # long time (see above)
+            False
+
+        """
+        return not (self == other)
+
 
 def polyhedron_to_cone_surface(polyhedron, use_AA=False, scaling_factor=ZZ(1)):
-    r"""Construct the Euclidean Cone Surface associated to the surface of a polyhedron and a map
+    r"""
+    Construct the Euclidean Cone Surface associated to the surface of a polyhedron and a map
     from the cone surface to the polyhedron.
-    
+
     INPUT:
 
-    - ``polyhedron`` -- A 3-dimensional polyhedron, which should be define over something that coerces into AA
+    - ``polyhedron`` -- A 3-dimensional polyhedron, which should be defined over something that coerces into AA
 
     - ``use_AA`` -- If True, the surface returned will be defined over AA. If false, the algorithm will find the smallest NumberField and write the field there.
-    
+
     - ``scaling_factor`` -- The surface returned will have a metric scaled by multiplication by this factor (compared with the original polyhendron). This can be used to produce a surface defined over a smaller NumberField.
-    
+
     OUTPUT:
-    
+
     A pair consisting of a ConeSurface and a ConeSurfaceToPolyhedronMap.
 
     EXAMPLES::
 
-    sage: from flatsurf.geometry.polyhedra import *
-    sage: vertices=[]
-    sage: for i in range(3):
-    ....:     temp=vector([1 if k==i else 0 for k in range(3)])
-    ....:     for j in range(-1,3,2):
-    ....:         vertices.append(j*temp)
-    sage: octahedron=Polyhedron(vertices=vertices)
-    sage: surface,surface_to_octahedron = \
-    ....:     polyhedron_to_cone_surface(octahedron,scaling_factor=AA(1/sqrt(2)))
-    sage: TestSuite(surface).run()
-    sage: TestSuite(surface_to_octahedron).run(skip="_test_pickling")
-    sage: surface.num_polygons()
-    8
-    sage: surface.base_ring()
-    Number Field in a with defining polynomial y^2 - 3 with a = 1.732050807568878?
-    sage: sqrt3=surface.base_ring().gen()
-    sage: tangent_bundle=surface.tangent_bundle()
-    sage: v=tangent_bundle(0,(0,0),(sqrt3,2))
-    sage: traj=v.straight_line_trajectory()
-    sage: traj.flow(10)
-    sage: traj.is_saddle_connection()
-    True
-    sage: traj.combinatorial_length()
-    8
-    sage: path3d = surface_to_octahedron(traj)
-    sage: len(path3d)
-    9
-    sage: # We will show that the length of the path is sqrt(42):
-    sage: total_length = 0
-    sage: for i in range(8):
-    ....:     start = path3d[i]
-    ....:     end = path3d[i+1]
-    ....:     total_length += (vector(end)-vector(start)).norm()
-    sage: ZZ(total_length**2)
-    42
+        sage: from flatsurf.geometry.polyhedra import Polyhedron, polyhedron_to_cone_surface
+        sage: vertices=[]
+        sage: for i in range(3):
+        ....:     temp=vector([1 if k==i else 0 for k in range(3)])
+        ....:     for j in range(-1,3,2):
+        ....:         vertices.append(j*temp)
+        sage: octahedron=Polyhedron(vertices=vertices)
+        sage: surface,surface_to_octahedron = \
+        ....:     polyhedron_to_cone_surface(octahedron,scaling_factor=AA(1/sqrt(2)))
+        sage: TestSuite(surface).run()
+        sage: TestSuite(surface_to_octahedron).run()  # long time (.4s)
+        sage: len(surface.polygons())
+        8
+        sage: surface.base_ring()
+        Number Field in a with defining polynomial y^2 - 3 with a = 1.732050807568878?
+        sage: sqrt3=surface.base_ring().gen()
+        sage: tangent_bundle=surface.tangent_bundle()
+        sage: v=tangent_bundle(0,(0,0),(sqrt3,2))
+        sage: traj=v.straight_line_trajectory()
+        sage: traj.flow(10)
+        sage: traj.is_saddle_connection()
+        True
+        sage: traj.combinatorial_length()
+        8
+        sage: path3d = surface_to_octahedron(traj)
+        sage: len(path3d)
+        9
+        sage: # We will show that the length of the path is sqrt(42):
+        sage: total_length = 0
+        sage: for i in range(8):
+        ....:     start = path3d[i]
+        ....:     end = path3d[i+1]
+        ....:     total_length += (vector(end)-vector(start)).norm()
+        sage: ZZ(total_length**2)
+        42
     """
-    assert polyhedron.dim()==3
-    c=polyhedron.center()
-    vertices=polyhedron.vertices()
-    vertex_order={}
-    for i,v in enumerate(vertices):
-        vertex_order[v]=i
-    faces=polyhedron.faces(2)
-    face_order={}
-    face_edges=[]
-    face_vertices=[]
-    face_map_data=[]
-    for i,f in enumerate(faces):
-        face_order[f]=i
-        edges=f.as_polyhedron().faces(1)
+    if polyhedron.dim() != 3:
+        raise ValueError
+
+    c = polyhedron.center()
+    vertices = polyhedron.vertices()
+    vertex_order = {}
+    for i, v in enumerate(vertices):
+        vertex_order[v] = i
+    faces = polyhedron.faces(2)
+    face_order = {}
+    face_edges = []
+    face_vertices = []
+    face_map_data = []
+    for i, f in enumerate(faces):
+        face_order[f] = i
+        edges = f.as_polyhedron().faces(1)
         face_edges_temp = set()
         for edge in edges:
-            edge_temp=set()
+            edge_temp = set()
             for vertex in edge.vertices():
-                v=vertex.vector()
+                v = vertex.vector()
                 v.set_immutable()
                 edge_temp.add(v)
             face_edges_temp.add(frozenset(edge_temp))
 
-            
         last_edge = next(iter(face_edges_temp))
         v = next(iter(last_edge))
-        face_vertices_temp=[v]
-        for j in range(len(face_edges_temp)-1):
+        face_vertices_temp = [v]
+        for j in range(len(face_edges_temp) - 1):
             for edge in face_edges_temp:
-                if v in edge and edge!=last_edge:
+                if v in edge and edge != last_edge:
                     # bingo
-                    last_edge=edge
+                    last_edge = edge
                     for vv in edge:
-                        if vv!=v:
-                            v=vv
+                        if vv != v:
+                            v = vv
                             face_vertices_temp.append(vv)
                             break
                     break
 
-
-        v0=face_vertices_temp[0]
-        v1=face_vertices_temp[1]
-        v2=face_vertices_temp[2]
-        n=(v1-v0).cross_product(v2-v0)
-        if (v0-c).dot_product(n)<0:
-            n=-n
+        v0 = face_vertices_temp[0]
+        v1 = face_vertices_temp[1]
+        v2 = face_vertices_temp[2]
+        n = (v1 - v0).cross_product(v2 - v0)
+        if (v0 - c).dot_product(n) < 0:
+            n = -n
             face_vertices_temp.reverse()
-            v0=face_vertices_temp[0]
-            v1=face_vertices_temp[1]
-            v2=face_vertices_temp[2]
-
-        face_vertices.append(face_vertices_temp)    
-        n=n/AA(n.norm())
-        w=v1-v0
-        w=w/AA(w.norm())
-        m=1/scaling_factor*matrix(AA,[w,n.cross_product(w),n]).transpose()
-        mi=~m
-        mis=mi.submatrix(0,0,2,3)
-        face_map_data.append((
-            v0, # translation to bring origin in plane to v0
-            m.submatrix(0,0,3,2),
-            -mis*v0,
-            mis
-        ))
-
-        it=iter(face_vertices_temp)    
-        v_last=next(it)
-        face_edge_dict={}
-        j=0
+            v0 = face_vertices_temp[0]
+            v1 = face_vertices_temp[1]
+            v2 = face_vertices_temp[2]
+
+        face_vertices.append(face_vertices_temp)
+        n = n / AA(n.norm())
+        w = v1 - v0
+        w = w / AA(w.norm())
+        m = 1 / scaling_factor * matrix(AA, [w, n.cross_product(w), n]).transpose()
+        mi = ~m
+        mi_submatrix = mi.submatrix(0, 0, 2, 3)
+        face_map_data.append(
+            (
+                v0,  # translation to bring origin in plane to v0
+                m.submatrix(0, 0, 3, 2),
+                -mi_submatrix * v0,
+                mi_submatrix,
+            )
+        )
+
+        it = iter(face_vertices_temp)
+        v_last = next(it)
+        face_edge_dict = {}
+        j = 0
         for v in it:
-            edge=frozenset([v_last,v])
-            face_edge_dict[edge]=j
-            j+=1
-            v_last=v
-        v=next(iter(face_vertices_temp))
-        edge=frozenset([v_last,v])
-        face_edge_dict[edge]=j
+            edge = frozenset([v_last, v])
+            face_edge_dict[edge] = j
+            j += 1
+            v_last = v
+        v = next(iter(face_vertices_temp))
+        edge = frozenset([v_last, v])
+        face_edge_dict[edge] = j
         face_edges.append(face_edge_dict)
-        
-    gluings={}
-    for p1,face_edge_dict1 in enumerate(face_edges):
+
+    gluings = {}
+    for p1, face_edge_dict1 in enumerate(face_edges):
         for edge, e1 in face_edge_dict1.items():
-            found=False
+            found = False
             for p2, face_edge_dict2 in enumerate(face_edges):
-                if p1!=p2 and edge in face_edge_dict2:
-                    e2=face_edge_dict2[edge]
-                    gluings[(p1,e1)]=(p2,e2)
-                    found=True
+                if p1 != p2 and edge in face_edge_dict2:
+                    e2 = face_edge_dict2[edge]
+                    gluings[(p1, e1)] = (p2, e2)
+                    found = True
                     break
             if not found:
                 print(p1)
                 print(e1)
                 print(edge)
                 raise RuntimeError("Failed to find glued edge")
-    polygon_vertices_AA=[]
-    for p,vs in enumerate(face_vertices):
-        trans=face_map_data[p][2]
-        m=face_map_data[p][3]
-        polygon_vertices_AA.append([trans+m*v for v in vs])
-        
-    
-    if use_AA==True:
-        Polys=ConvexPolygons(AA)
-        polygons=[]
+
+    polygon_vertices_AA = []
+    for p, vs in enumerate(face_vertices):
+        trans = face_map_data[p][2]
+        m = face_map_data[p][3]
+        polygon_vertices_AA.append([trans + m * v for v in vs])
+
+    from flatsurf import MutableOrientedSimilaritySurface
+
+    if use_AA is True:
+        from flatsurf import Polygon
+
+        S = MutableOrientedSimilaritySurface(AA)
         for vs in polygon_vertices_AA:
-            polygons.append(Polys(vertices=vs))
-        S=ConeSurface(surface_list_from_polygons_and_gluings(polygons,gluings))
-        return S, \
-            ConeSurfaceToPolyhedronMap(S,polyhedron,face_map_data)
+            S.add_polygon(Polygon(vertices=vs, base_ring=AA))
+        for x, y in gluings.items():
+            S.glue(x, y)
+        S.set_immutable()
+        return S, ConeSurfaceToPolyhedronMap(S, polyhedron, face_map_data)
     else:
-        elts=[]
+        elts = []
         for vs in polygon_vertices_AA:
             for v in vs:
                 elts.append(v[0])
                 elts.append(v[1])
-                
+
         # Find the best number field:
-        field,elts2,hom = number_field_elements_from_algebraics(elts,minimal=True)
-        if field==QQ:
+        field, elts2, hom = number_field_elements_from_algebraics(elts, minimal=True)
+        if field == QQ:
             # Defined over the rationals!
-            polygon_vertices_field2=[]
-            j=0
+            polygon_vertices_field2 = []
+            j = 0
             for vs in polygon_vertices_AA:
-                vs2=[]
+                vs2 = []
                 for v in vs:
-                    vs2.append(vector(field,[elts2[j],elts2[j+1]]))
-                    j=j+2
+                    vs2.append(vector(field, [elts2[j], elts2[j + 1]]))
+                    j = j + 2
                 polygon_vertices_field2.append(vs2)
-            Polys=ConvexPolygons(field)
-            polygons=[]
+            S = MutableOrientedSimilaritySurface(field)
+            from flatsurf import Polygon
+
             for vs in polygon_vertices_field2:
-                polygons.append(Polys(vertices=vs))
-            S=ConeSurface(surface_list_from_polygons_and_gluings(polygons,gluings))
-            return S, \
-                ConeSurfaceToPolyhedronMap(S,polyhedron,face_map_data)
+                S.add_polygon(Polygon(vertices=vs, base_ring=field))
+            for x, y in gluings.items():
+                S.glue(x, y)
+            S.set_immutable()
+            return S, ConeSurfaceToPolyhedronMap(S, polyhedron, face_map_data)
 
-        else:        
+        else:
             # Unfortunately field doesn't come with an real embedding (which is given by hom!)
             # So, we make a copy of the field, and add the embedding.
-            field2=NumberField(field.polynomial(),name="a",embedding=hom(field.gen()))
+            field2 = NumberField(
+                field.polynomial(), name="a", embedding=hom(field.gen())
+            )
             # The following converts from field to field2:
-            hom2=field.hom(im_gens=[field2.gen()])
+            hom2 = field.hom(im_gens=[field2.gen()])
 
-            polygon_vertices_field2=[]
-            j=0
+            polygon_vertices_field2 = []
+            j = 0
             for vs in polygon_vertices_AA:
-                vs2=[]
+                vs2 = []
                 for v in vs:
-                    vs2.append(vector(field2,[hom2(elts2[j]),hom2(elts2[j+1])]))
-                    j=j+2
+                    vs2.append(vector(field2, [hom2(elts2[j]), hom2(elts2[j + 1])]))
+                    j = j + 2
                 polygon_vertices_field2.append(vs2)
-            Polys=ConvexPolygons(field2)
-            polygons=[]
+            S = MutableOrientedSimilaritySurface(field2)
+            from flatsurf import Polygon
+
             for vs in polygon_vertices_field2:
-                polygons.append(Polys(vertices=vs))
-            S=ConeSurface(surface_list_from_polygons_and_gluings(polygons,gluings))
-            return S, \
-                ConeSurfaceToPolyhedronMap(S,polyhedron,face_map_data)
+                S.add_polygon(Polygon(vertices=vs, base_ring=field2))
+            for x, y in gluings.items():
+                S.glue(x, y)
+            S.set_immutable()
+            return S, ConeSurfaceToPolyhedronMap(S, polyhedron, face_map_data)
+
 
 def platonic_tetrahedron():
     r"""Produce a triple consisting of a polyhedral version of the platonic tetrahedron,
     the associated cone surface, and a ConeSurfaceToPolyhedronMap from the surface
     to the polyhedron.
 
     EXAMPLES::
 
-    sage: from flatsurf.geometry.polyhedra import platonic_tetrahedron
-    sage: polyhedron,surface,surface_to_polyhedron = platonic_tetrahedron()
-    sage: TestSuite(surface).run()
-    r"""
-    vertices=[]
-    for x in range(-1,3,2):
-        for y in range(-1,3,2):
-                vertices.append(vector(QQ,(x,y,x*y)))
-    p=Polyhedron(vertices=vertices)
-    s,m = polyhedron_to_cone_surface(p,scaling_factor=AA(1/sqrt(2)))
-    return p,s,m
+        sage: from flatsurf.geometry.polyhedra import platonic_tetrahedron
+        sage: polyhedron,surface,surface_to_polyhedron = platonic_tetrahedron()
+        sage: TestSuite(surface).run()
+    """
+    vertices = []
+    for x in range(-1, 3, 2):
+        for y in range(-1, 3, 2):
+            vertices.append(vector(QQ, (x, y, x * y)))
+    p = Polyhedron(vertices=vertices)
+    s, m = polyhedron_to_cone_surface(p, scaling_factor=AA(1 / sqrt(2)))
+    return p, s, m
+
 
 def platonic_cube():
     r"""Produce a triple consisting of a polyhedral version of the platonic cube,
     the associated cone surface, and a ConeSurfaceToPolyhedronMap from the surface
     to the polyhedron.
 
     EXAMPLES::
 
-    sage: from flatsurf.geometry.polyhedra import platonic_cube
-    sage: polyhedron,surface,surface_to_polyhedron = platonic_cube()
-    sage: TestSuite(surface).run()
-    r"""
-    vertices=[]
-    for x in range(-1,3,2):
-        for y in range(-1,3,2):
-            for z in range(-1,3,2):
-                vertices.append(vector(QQ,(x,y,z)))
-    p=Polyhedron(vertices=vertices)
-    s,m = polyhedron_to_cone_surface(p,scaling_factor=QQ(1)/2)
-    return p,s,m
+        sage: from flatsurf.geometry.polyhedra import platonic_cube
+        sage: polyhedron,surface,surface_to_polyhedron = platonic_cube()
+        sage: TestSuite(surface).run()
+    """
+    vertices = []
+    for x in range(-1, 3, 2):
+        for y in range(-1, 3, 2):
+            for z in range(-1, 3, 2):
+                vertices.append(vector(QQ, (x, y, z)))
+    p = Polyhedron(vertices=vertices)
+    s, m = polyhedron_to_cone_surface(p, scaling_factor=QQ(1) / 2)
+    return p, s, m
+
 
 def platonic_octahedron():
     r"""Produce a triple consisting of a polyhedral version of the platonic octahedron,
     the associated cone surface, and a ConeSurfaceToPolyhedronMap from the surface
     to the polyhedron.
 
     EXAMPLES::
 
-    sage: from flatsurf.geometry.polyhedra import platonic_octahedron
-    sage: polyhedron,surface,surface_to_polyhedron = platonic_octahedron()
-    sage: TestSuite(surface).run()
-    r"""
-    vertices=[]
+        sage: from flatsurf.geometry.polyhedra import platonic_octahedron
+        sage: polyhedron,surface,surface_to_polyhedron = platonic_octahedron()  # long time (.3s)
+        sage: TestSuite(surface).run()  # long time (see above)
+    """
+    vertices = []
     for i in range(3):
-        temp=vector(QQ,[1 if k==i else 0 for k in range(3)])
-        for j in range(-1,3,2):
-            vertices.append(j*temp)
-    octahedron=Polyhedron(vertices=vertices)
-    surface,surface_to_octahedron = \
-        polyhedron_to_cone_surface(octahedron,scaling_factor=AA(sqrt(2)))
-    return octahedron,surface,surface_to_octahedron
+        temp = vector(QQ, [1 if k == i else 0 for k in range(3)])
+        for j in range(-1, 3, 2):
+            vertices.append(j * temp)
+    octahedron = Polyhedron(vertices=vertices)
+    surface, surface_to_octahedron = polyhedron_to_cone_surface(
+        octahedron, scaling_factor=AA(sqrt(2))
+    )
+    return octahedron, surface, surface_to_octahedron
+
 
 def platonic_dodecahedron():
     r"""Produce a triple consisting of a polyhedral version of the platonic dodecahedron,
     the associated cone surface, and a ConeSurfaceToPolyhedronMap from the surface
     to the polyhedron.
 
     EXAMPLES::
 
-    sage: from flatsurf.geometry.polyhedra import platonic_dodecahedron
-    sage: polyhedron,surface,surface_to_polyhedron = platonic_dodecahedron()
-    sage: TestSuite(surface).run()
-    r"""
-    vertices=[]
-    phi=AA(1+sqrt(5))/2
-    F=NumberField(phi.minpoly(),"phi",embedding=phi)
-    phi=F.gen()
-    for x in range(-1,3,2):
-        for y in range(-1,3,2):
-            for z in range(-1,3,2):
-                vertices.append(vector(F,(x,y,z)))
-    for x in range(-1,3,2):
-        for y in range(-1,3,2):
-            vertices.append(vector(F,(0,x*phi,y/phi)))
-            vertices.append(vector(F,(y/phi,0,x*phi)))
-            vertices.append(vector(F,(x*phi,y/phi,0)))
-    scale=AA(2/sqrt(1+(phi-1)**2+(1/phi-1)**2))
-    p=Polyhedron(vertices=vertices)
-    s,m = polyhedron_to_cone_surface(p,scaling_factor=scale)
-    return p,s,m
+        sage: from flatsurf.geometry.polyhedra import platonic_dodecahedron
+        sage: polyhedron, surface, surface_to_polyhedron = platonic_dodecahedron()  # long time (1s)
+        sage: TestSuite(surface).run()  # long time (.8s)
+    """
+    vertices = []
+    phi = AA(1 + sqrt(5)) / 2
+    F = NumberField(phi.minpoly(), "phi", embedding=phi)
+    phi = F.gen()
+    for x in range(-1, 3, 2):
+        for y in range(-1, 3, 2):
+            for z in range(-1, 3, 2):
+                vertices.append(vector(F, (x, y, z)))
+    for x in range(-1, 3, 2):
+        for y in range(-1, 3, 2):
+            vertices.append(vector(F, (0, x * phi, y / phi)))
+            vertices.append(vector(F, (y / phi, 0, x * phi)))
+            vertices.append(vector(F, (x * phi, y / phi, 0)))
+    scale = AA(2 / sqrt(1 + (phi - 1) ** 2 + (1 / phi - 1) ** 2))
+    p = Polyhedron(vertices=vertices)
+    s, m = polyhedron_to_cone_surface(p, scaling_factor=scale)
+    return p, s, m
+
 
 def platonic_icosahedron():
     r"""Produce a triple consisting of a polyhedral version of the platonic icosahedron,
     the associated cone surface, and a ConeSurfaceToPolyhedronMap from the surface
     to the polyhedron.
 
     EXAMPLES::
 
-    sage: from flatsurf.geometry.polyhedra import platonic_icosahedron
-    sage: polyhedron,surface,surface_to_polyhedron = platonic_icosahedron()
-    sage: TestSuite(surface).run()
-    r"""
-    vertices=[]
-    phi=AA(1+sqrt(5))/2
-    F=NumberField(phi.minpoly(),"phi",embedding=phi)
-    phi=F.gen()
+        sage: from flatsurf.geometry.polyhedra import platonic_icosahedron
+        sage: polyhedron,surface,surface_to_polyhedron = platonic_icosahedron()  # long time (.9s)
+        sage: TestSuite(surface).run()  # long time (see above)
+    """
+    vertices = []
+    phi = AA(1 + sqrt(5)) / 2
+    F = NumberField(phi.minpoly(), "phi", embedding=phi)
+    phi = F.gen()
     for i in range(3):
-        for s1 in range(-1,3,2):
-            for s2 in range(-1,3,2):
-                p=3*[None]
-                p[i]=s1*phi
-                p[(i+1)%3]=s2
-                p[(i+2)%3]=0
-                vertices.append(vector(F,p))
-    p=Polyhedron(vertices=vertices)
-    
-    s,m = polyhedron_to_cone_surface(p)
-    return p,s,m
+        for s1 in range(-1, 3, 2):
+            for s2 in range(-1, 3, 2):
+                p = 3 * [None]
+                p[i] = s1 * phi
+                p[(i + 1) % 3] = s2
+                p[(i + 2) % 3] = 0
+                vertices.append(vector(F, p))
+    p = Polyhedron(vertices=vertices)
+
+    s, m = polyhedron_to_cone_surface(p)
+    return p, s, m
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/pyflatsurf_conversion.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/pyflatsurf_conversion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 r"""
 Interface with pyflatsurf
 """
 # ********************************************************************
 #  This file is part of sage-flatsurf.
 #
 #        Copyright (C) 2019      Vincent Delecroix
@@ -36,42 +35,42 @@
     assert isinstance(vp, list)
     assert isinstance(fp, list)
     assert isinstance(vec, list)
 
     n = len(vp) - 1
 
     assert n % 2 == 0, n
-    assert len(fp) == n+1
-    assert len(vec) == n//2
+    assert len(fp) == n + 1
+    assert len(vec) == n // 2
 
     assert vp[0] is None
     assert fp[0] is None
 
-    for i in range(1, n//2+1):
+    for i in range(1, n // 2 + 1):
         # check fp/vp consistency
         assert fp[-vp[i]] == i, i
 
         # check that each face is a triangle and that vectors sum up to zero
         j = fp[i]
         k = fp[j]
         assert i != j and i != k and fp[k] == i, (i, j, k)
-        vi = vec[i-1] if i >= 1 else -vec[-i-1]
-        vj = vec[j-1] if j >= 1 else -vec[-j-1]
-        vk = vec[k-1] if k >= 1 else -vec[-k-1]
+        vi = vec[i - 1] if i >= 1 else -vec[-i - 1]
+        vj = vec[j - 1] if j >= 1 else -vec[-j - 1]
+        vk = vec[k - 1] if k >= 1 else -vec[-k - 1]
         v = vi + vj + vk
         assert v.x() == 0, v.x()
         assert v.y() == 0, v.y()
 
 
 def _cycle_decomposition(p):
     n = len(p) - 1
     assert n % 2 == 0
     cycles = []
-    unseen = [True] * (n+1)
-    for i in list(range(-n//2+1, 0)) + list(range(1, n//2)):
+    unseen = [True] * (n + 1)
+    for i in list(range(-n // 2 + 1, 0)) + list(range(1, n // 2)):
         if unseen[i]:
             j = i
             cycle = []
             while unseen[j]:
                 unseen[j] = False
                 cycle.append(j)
                 j = p[j]
@@ -80,89 +79,98 @@
 
 
 def to_pyflatsurf(S):
     r"""
     Given S a translation surface from sage-flatsurf return a
     flatsurf::FlatTriangulation from libflatsurf/pyflatsurf.
     """
-    from flatsurf.geometry.translation_surface import TranslationSurface
-    if not isinstance(S, TranslationSurface):
+    from flatsurf.geometry.categories import TranslationSurfaces
+
+    if S not in TranslationSurfaces():
         raise TypeError("S must be a translation surface")
-    if not S.is_finite():
+    if not S.is_finite_type():
         raise ValueError("the surface S must be finite")
 
     S = S.triangulate()
 
     # populate half edges and vectors
-    n = sum(S.polygon(lab).num_edges() for lab in S.label_iterator())
-    half_edge_labels = {}   # map: (face lab, edge num) in faltsurf -> integer
-    vec = []                # vectors
-    k = 1                   # half edge label in {1, ..., n}
-    for t0, t1 in S.edge_iterator(gluings=True):
+    n = sum(len(S.polygon(lab).vertices()) for lab in S.labels())
+    half_edge_labels = {}  # map: (face lab, edge num) in faltsurf -> integer
+    vec = []  # vectors
+    k = 1  # half edge label in {1, ..., n}
+    for t0, t1 in S.gluings():
         if t0 in half_edge_labels:
             continue
 
         half_edge_labels[t0] = k
         half_edge_labels[t1] = -k
 
         f0, e0 = t0
         p = S.polygon(f0)
         vec.append(p.edge(e0))
 
         k += 1
 
     # compute vertex and face permutations
-    vp = [None] * (n+1)  # vertex permutation
-    fp = [None] * (n+1)  # face permutation
-    for t in S.edge_iterator(gluings=False):
+    vp = [None] * (n + 1)  # vertex permutation
+    fp = [None] * (n + 1)  # face permutation
+    for t in S.edges():
         e = half_edge_labels[t]
-        j = (t[1] + 1) % S.polygon(t[0]).num_edges()
+        j = (t[1] + 1) % len(S.polygon(t[0]).vertices())
         fp[e] = half_edge_labels[(t[0], j)]
         vp[fp[e]] = -e
 
     # convert the vp permutation into cycles
     verts = _cycle_decomposition(vp)
 
     # find a finite SageMath base ring that contains all the coordinates
     base_ring = S.base_ring()
     if base_ring is AA:
         from sage.rings.qqbar import number_field_elements_from_algebraics
         from itertools import chain
-        base_ring = number_field_elements_from_algebraics(list(chain(*[list(v) for v in vec])), embedded=True)[0]
+
+        base_ring = number_field_elements_from_algebraics(
+            list(chain(*[list(v) for v in vec])), embedded=True
+        )[0]
 
     from flatsurf.features import pyflatsurf_feature
+
     pyflatsurf_feature.require()
     from pyflatsurf.vector import Vectors
 
     V = Vectors(base_ring)
     vec = [V(v).vector for v in vec]
 
     _check_data(vp, fp, vec)
 
     from pyflatsurf.factory import make_surface
+
     return make_surface(verts, vec)
 
 
 def sage_ring(surface):
     r"""
     Return the SageMath ring over which the pyflatsurf surface ``surface`` can
     be constructed in sage-flatsurf.
 
     EXAMPLES::
 
         sage: from flatsurf import translation_surfaces
         sage: from flatsurf.geometry.pyflatsurf_conversion import to_pyflatsurf, sage_ring # optional: pyflatsurf
-        sage: S = to_pyflatsurf(translation_surfaces.veech_double_n_gon(5)) # optional: pyflatsurf
+        sage: S = to_pyflatsurf(translation_surfaces.veech_double_n_gon(5)) # optional: pyflatsurf  # random output due to matplotlib warnings with some combinations of setuptools and matplotlib
         sage: sage_ring(S) # optional: pyflatsurf
         Number Field in a with defining polynomial x^4 - 5*x^2 + 5 with a = 1.902113032590308?
 
     """
     from sage.all import Sequence
+
     vectors = [surface.fromHalfEdge(e.positive()) for e in surface.edges()]
-    return Sequence([to_sage_ring(v.x()) for v in vectors] + [to_sage_ring(v.y()) for v in vectors]).universe()
+    return Sequence(
+        [to_sage_ring(v.x()) for v in vectors] + [to_sage_ring(v.y()) for v in vectors]
+    ).universe()
 
 
 def to_sage_ring(x):
     r"""
     Given a coordinate of a flatsurf::Vector, return a SageMath element from
     which :meth:`from_pyflatsurf` can eventually construct a translation surface.
 
@@ -193,14 +201,15 @@
         sage: from pyexactreal import QQModule, RealNumber  # optional: pyflatsurf
         sage: M = QQModule(RealNumber.random())   # optional: pyflatsurf
         sage: to_sage_ring(M.gen(0R)).parent()  # optional: pyflatsurf
         Real Numbers as (Rational Field)-Module
 
     """
     from flatsurf.features import cppyy_feature
+
     cppyy_feature.require()
     import cppyy
 
     def maybe_type(t):
         try:
             return t()
         except AttributeError:
@@ -211,96 +220,113 @@
         return ZZ(x)
     elif type(x) is maybe_type(lambda: cppyy.gbl.mpz_class):
         return ZZ(str(x))
     elif type(x) is maybe_type(lambda: cppyy.gbl.mpq_class):
         return QQ(str(x))
     elif type(x) is maybe_type(lambda: cppyy.gbl.eantic.renf_elem_class):
         from pyeantic import RealEmbeddedNumberField
+
         real_embedded_number_field = RealEmbeddedNumberField(x.parent())
         return real_embedded_number_field.number_field(real_embedded_number_field(x))
-    elif type(x) is maybe_type(lambda: cppyy.gbl.exactreal.Element[cppyy.gbl.exactreal.IntegerRing]):
+    elif type(x) is maybe_type(
+        lambda: cppyy.gbl.exactreal.Element[cppyy.gbl.exactreal.IntegerRing]
+    ):
         from pyexactreal import ExactReals
+
         return ExactReals(ZZ)(x)
-    elif type(x) is maybe_type(lambda: cppyy.gbl.exactreal.Element[cppyy.gbl.exactreal.RationalField]):
+    elif type(x) is maybe_type(
+        lambda: cppyy.gbl.exactreal.Element[cppyy.gbl.exactreal.RationalField]
+    ):
         from pyexactreal import ExactReals
+
         return ExactReals(QQ)(x)
-    elif type(x) is maybe_type(lambda: cppyy.gbl.exactreal.Element[cppyy.gbl.exactreal.NumberField]):
+    elif type(x) is maybe_type(
+        lambda: cppyy.gbl.exactreal.Element[cppyy.gbl.exactreal.NumberField]
+    ):
         from pyexactreal import ExactReals
+
         return ExactReals(x.module().ring().parameters)(x)
     else:
-        raise NotImplementedError(f"unknown coordinate ring for element {x} which is a {type(x)}")
+        raise NotImplementedError(
+            f"unknown coordinate ring for element {x} which is a {type(x)}"
+        )
 
 
 def from_pyflatsurf(T):
     r"""
     Given T a flatsurf::FlatTriangulation from libflatsurf/pyflatsurf, return a
     sage-flatsurf translation surface.
 
     EXAMPLES::
 
         sage: from flatsurf import translation_surfaces
         sage: from flatsurf.geometry.pyflatsurf_conversion import to_pyflatsurf, from_pyflatsurf # optional: pyflatsurf
         sage: S = translation_surfaces.veech_double_n_gon(5) # optional: pyflatsurf
-        sage: from_pyflatsurf(to_pyflatsurf(S)) # optional: pyflatsurf
-        TranslationSurface built from 6 polygons
-
-    TESTS:
+        sage: T = from_pyflatsurf(to_pyflatsurf(S)) # optional: pyflatsurf
+        sage: T  # optional: pyflatsurf
+        Translation Surface in H_2(2) built from 6 isosceles triangles
+
+    TESTS::
+
+        sage: from flatsurf.geometry.categories import TranslationSurfaces
+        sage: T in TranslationSurfaces()  # optional: pyflatsurf
+        True
 
     Verify that #137 has been resolved::
 
-        sage: from flatsurf import polygons
-        sage: from flatsurf.geometry.surface import Surface_list
-        sage: from flatsurf.geometry.translation_surface import TranslationSurface
+        sage: from flatsurf import polygons, MutableOrientedSimilaritySurface
         sage: from flatsurf.geometry.gl2r_orbit_closure import GL2ROrbitClosure
         sage: from flatsurf.geometry.pyflatsurf_conversion import from_pyflatsurf
         sage: P = polygons.regular_ngon(10)
-        sage: S = Surface_list(P.base_ring())
+        sage: S = MutableOrientedSimilaritySurface(P.base_ring())
         sage: S.add_polygon(P)
         0
-        sage: for i in range(5): S.set_edge_pairing(0, i, 0, 5+i)
-        sage: M = TranslationSurface(S)
+        sage: for i in range(5): S.glue((0, i), (0, 5+i))
+        sage: S.set_immutable()
+        sage: M = S
         sage: X = GL2ROrbitClosure(M)  # optional: pyflatsurf
         sage: D0 = list(X.decompositions(2))[2]  # optional: pyflatsurf
         sage: T0 = D0.triangulation()  # optional: pyflatsurf
         sage: from_pyflatsurf(T0)  # optional: pyflatsurf
-        TranslationSurface built from 8 polygons
+        Translation Surface in H_2(1^2) built from 2 isosceles triangles and 6 triangles
 
     """
     from flatsurf.features import pyflatsurf_feature
+
     pyflatsurf_feature.require()
     import pyflatsurf
 
     ring = sage_ring(T)
 
-    from flatsurf.geometry.surface import Surface_list
-    S = Surface_list(ring)
+    from flatsurf.geometry.surface import MutableOrientedSimilaritySurface
+
+    S = MutableOrientedSimilaritySurface(ring)
 
-    from flatsurf.geometry.polygon import ConvexPolygons
-    P = ConvexPolygons(ring)
+    from flatsurf.geometry.polygon import Polygon
 
-    V = P.module()
+    V = ring**2
 
     half_edges = {}
 
     for face in T.faces():
         a, b, c = map(pyflatsurf.flatsurf.HalfEdge, face)
 
         vectors = [T.fromHalfEdge(he) for he in face]
-        vectors = [V([ring(to_sage_ring(v.x())), ring(to_sage_ring(v.y()))]) for v in vectors]
-        triangle = P(vectors)
+        vectors = [
+            V([ring(to_sage_ring(v.x())), ring(to_sage_ring(v.y()))]) for v in vectors
+        ]
+        triangle = Polygon(edges=vectors)
         face_id = S.add_polygon(triangle)
 
-        assert(a not in half_edges)
+        assert a not in half_edges
         half_edges[a] = (face_id, 0)
-        assert(b not in half_edges)
+        assert b not in half_edges
         half_edges[b] = (face_id, 1)
-        assert(c not in half_edges)
+        assert c not in half_edges
         half_edges[c] = (face_id, 2)
 
     for half_edge, (face, id) in half_edges.items():
         _face, _id = half_edges[-half_edge]
-        S.change_edge_gluing(face, id, _face, _id)
+        S.glue((face, id), (_face, _id))
 
     S.set_immutable()
-
-    from flatsurf.geometry.translation_surface import TranslationSurface
-    return TranslationSurface(S)
+    return S
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/similarity.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/similarity.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,26 @@
-# -*- coding: utf-8 -*-
-#*********************************************************************
+# ****************************************************************************
 #  This file is part of sage-flatsurf.
 #
 #        Copyright (C) 2016-2020 Vincent Delecroix
-#                      2020      Julian Rüth
+#                      2020-2023 Julian Rüth
 #
 #  sage-flatsurf is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 2 of the License, or
 #  (at your option) any later version.
 #
 #  sage-flatsurf is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
-#*********************************************************************
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
-
+# *********************************************************************
 from sage.misc.cachefunc import cached_method
 
 from sage.structure.element import MultiplicativeGroupElement, parent
 from sage.structure.unique_representation import UniqueRepresentation
 
 from sage.categories.groups import Groups
 
@@ -32,33 +28,29 @@
 
 from sage.modules.free_module_element import vector
 from sage.groups.group import Group
 from sage.rings.integer import Integer
 from sage.rings.integer_ring import ZZ
 from sage.modules.free_module_element import FreeModuleElement
 
-from sage.env import SAGE_VERSION
-if SAGE_VERSION >= '8.2':
-    from sage.structure.element import is_Matrix
-else:
-    from sage.matrix.matrix import is_Matrix
-
-from flatsurf.geometry.polygon import ConvexPolygon, ConvexPolygons
+from sage.structure.element import is_Matrix
 
 ZZ_0 = Integer(0)
 ZZ_1 = Integer(1)
 ZZ_m1 = -ZZ_1
 
+
 class Similarity(MultiplicativeGroupElement):
     r"""
     Class for a similarity of the plane with possible reflection.
 
     Construct the similarity (x,y) mapsto (ax-by+s,bx+ay+t) if sign=1,
     and (ax+by+s,bx-ay+t) if sign=-1
     """
+
     def __init__(self, p, a, b, s, t, sign):
         r"""
         Construct the similarity (x,y) mapsto (ax-by+s,bx+ay+t) if sign=1,
         and (ax+by+s,bx-ay+t) if sign=-1
         """
         if p is None:
             raise ValueError("The parent must be provided")
@@ -113,15 +105,19 @@
             sage: S((1,2)).is_half_translation()
             True
             sage: S((-1, 0, 0, 2)).is_half_translation()
             True
             sage: S((0,1,0,0)).is_half_translation()
             False
         """
-        return self._sign.is_one() and (self._a.is_one() or ((-self._a).is_one())) and self._b.is_zero()
+        return (
+            self._sign.is_one()
+            and (self._a.is_one() or ((-self._a).is_one()))
+            and self._b.is_zero()
+        )
 
     def is_orientable(self):
         return self._sign.is_one()
 
     def is_rotation(self):
         r"""
         Check whether this element is a rotation
@@ -161,17 +157,17 @@
         det = self.det()
         return det.is_one() or (-det).is_one()
 
     def det(self):
         r"""
         Return the determinant of this element
         """
-        return self._sign * (self._a*self._a + self._b*self._b)
+        return self._sign * (self._a * self._a + self._b * self._b)
 
-    def _mul_(left, right):
+    def _mul_(self, right):
         r"""
         Composition
 
         EXAMPLES::
 
             sage: from flatsurf.geometry.similarity import SimilarityGroup
             sage: S = SimilarityGroup(QQ)
@@ -184,20 +180,20 @@
             sage: a3 = S((1,1,0,0))
             sage: a4 = S((1,0,-1,1))
             sage: a5 = S((2,-1,3/5,2/3,-1))
             sage: for g1,g2,g3 in product([a1,a2,a3,a4,a5], repeat=3):
             ....:     assert g1.matrix()*g2.matrix() == (g1*g2).matrix()
             ....:     assert (g1*g2).matrix()*g3.matrix() == (g1*g2*g3).matrix()
         """
-        a = left._a * right._a - left._sign * left._b * right._b
-        b = left._b * right._a + left._sign * left._a * right._b
-        s = left._a * right._s - left._sign * left._b * right._t + left._s
-        t = left._b * right._s + left._sign * left._a * right._t + left._t
-        sign = left._sign * right._sign
-        P = left.parent()
+        a = self._a * right._a - self._sign * self._b * right._b
+        b = self._b * right._a + self._sign * self._a * right._b
+        s = self._a * right._s - self._sign * self._b * right._t + self._s
+        t = self._b * right._s + self._sign * self._a * right._t + self._t
+        sign = self._sign * right._sign
+        P = self.parent()
         return P.element_class(P, a, b, s, t, sign)
 
     def __invert__(self):
         r"""
         Invert a similarity.
 
         TESTS::
@@ -208,110 +204,138 @@
             sage: for a in [S((0,2,0,0,1)), S((1,0,0,0,-1)), S((1,1,0,0)),
             ....:           S((1,0,-1,1)), S((2,-1,3/5,2/3,-1))]:
             ....:     assert (a*~a).is_one() and (~a*a).is_one()
         """
         P = self.parent()
         sign = self._sign
         det = self.det()
-        a = sign*self._a/det
-        b = -self._b/det
-        return P.element_class(P,a,b,
-            -a*self._s + sign*b*self._t,
-            -b*self._s - sign*a*self._t,
-            sign)
+        a = sign * self._a / det
+        b = -self._b / det
+        return P.element_class(
+            P,
+            a,
+            b,
+            -a * self._s + sign * b * self._t,
+            -b * self._s - sign * a * self._t,
+            sign,
+        )
 
-    def _div_(left, right):
+    def _div_(self, right):
         det = right.det()
 
         inv_a = right._sign * right._a
         inv_b = -right._b
         inv_s = -right._sign * right._a * right._s - right._sign * right._b * right._t
         inv_t = right._b * right._s - right._a * right._t
 
-        a = (left._a * inv_a - left._sign * left._b * inv_b) / det
-        b = (left._b * inv_a + left._sign * left._a * inv_b) / det
-        s = (left._a * inv_s - left._sign * left._b * inv_t) / det + left._s
-        t = (left._b * inv_s + left._sign * left._a * inv_t) / det + left._t
-
-        return left.parent().element_class(left.parent(),
-            left.base_ring()(a),
-            left.base_ring()(b),
-            left.base_ring()(s),
-            left.base_ring()(t),
-            left._sign * right._sign)
+        a = (self._a * inv_a - self._sign * self._b * inv_b) / det
+        b = (self._b * inv_a + self._sign * self._a * inv_b) / det
+        s = (self._a * inv_s - self._sign * self._b * inv_t) / det + self._s
+        t = (self._b * inv_s + self._sign * self._a * inv_t) / det + self._t
+
+        return self.parent().element_class(
+            self.parent(),
+            self.base_ring()(a),
+            self.base_ring()(b),
+            self.base_ring()(s),
+            self.base_ring()(t),
+            self._sign * right._sign,
+        )
 
     def __hash__(self):
-        return 73*hash(self._a)-19*hash(self._b)+13*hash(self._s)+53*hash(self._t)+67*hash(self._sign)
-
-    def __call__(self, w, ring = None):
-        r"""
-        Return the image of ``w`` under the similarity. Here ``w`` may be a ConvexPolygon or a vector
-        (or something that can be indexed in the same way as a vector). If a ring is provided,
-        the objects returned will be defined over this ring.
+        return (
+            73 * hash(self._a)
+            - 19 * hash(self._b)
+            + 13 * hash(self._s)
+            + 53 * hash(self._t)
+            + 67 * hash(self._sign)
+        )
+
+    def __call__(self, w, ring=None):
+        r"""
+        Return the image of ``w`` under the similarity. Here ``w`` may be a
+        convex polygon or a vector (or something that can be indexed in the
+        same way as a vector). If a ring is provided, the objects returned will
+        be defined over this ring.
 
         TESTS::
 
             sage: from flatsurf.geometry.similarity import SimilarityGroup
             sage: S = SimilarityGroup(AA)
             sage: a = S((1,-1,AA(2).sqrt(),0))
             sage: a((1,2))
             (4.414213562373095?, 1)
             sage: a.matrix()*vector((1,2,1))
             (4.414213562373095?, 1, 1)
 
             sage: from flatsurf.geometry.similarity import SimilarityGroup
             sage: SG = SimilarityGroup(QQ)
-            sage: from flatsurf import ConvexPolygons
-            sage: P = ConvexPolygons(QQ)
-            sage: p = P.an_element()
-            sage: p
-            Polygon: (0, 0), (1, 0), (1, 1), (0, 1)
+            sage: from flatsurf import Polygon
+            sage: p = Polygon(vertices=[(0, 0), (1, 0), (1, 1), (0, 1)])
             sage: g = SG.an_element()**2
             sage: g
             (x, y) |-> (25*x + 4, 25*y + 10)
             sage: g(p)
-            Polygon: (4, 10), (29, 10), (29, 35), (4, 35)
-            sage: g(p, ring=AA).parent()
-            ConvexPolygons(Algebraic Real Field)
+            Polygon(vertices=[(4, 10), (29, 10), (29, 35), (4, 35)])
+            sage: g(p, ring=AA).category()
+            Category of convex simple euclidean polygons over Algebraic Real Field
+
         """
         if ring is not None and ring not in Rings():
             raise TypeError("ring must be a ring")
 
-        if isinstance(w, ConvexPolygon):
+        from flatsurf.geometry.polygon import EuclideanPolygon
+
+        if isinstance(w, EuclideanPolygon) and w.is_convex():
             if ring is None:
                 ring = self.parent().base_ring()
-            P = ConvexPolygons(ring)
+
+            from flatsurf import Polygon
 
             try:
-                return P(vertices=[self(v) for v in w.vertices()])
-            except ValueError as e:
+                return Polygon(vertices=[self(v) for v in w.vertices()], base_ring=ring)
+            except ValueError:
                 if not self._sign.is_one():
                     raise ValueError("Similarity must be orientation preserving.")
-                else:
-                    # Not sure why this would happen:
-                    raise
+
+                # Not sure why this would happen:
+                raise
 
         if ring is None:
             if self._sign.is_one():
-                return vector([
-                    self._a * w[0] - self._b*w[1] + self._s,
-                    self._b * w[0] + self._a * w[1] + self._t])
+                return vector(
+                    [
+                        self._a * w[0] - self._b * w[1] + self._s,
+                        self._b * w[0] + self._a * w[1] + self._t,
+                    ]
+                )
             else:
-                return vector([
-                    self._a * w[0] + self._b * w[1] + self._s,
-                    self._b * w[0] - self._a * w[1] + self._t])
+                return vector(
+                    [
+                        self._a * w[0] + self._b * w[1] + self._s,
+                        self._b * w[0] - self._a * w[1] + self._t,
+                    ]
+                )
         else:
             if self._sign.is_one():
-                return vector(ring, [
-                    self._a * w[0] - self._b * w[1] + self._s,
-                    self._b * w[0] + self._a * w[1] + self._t])
+                return vector(
+                    ring,
+                    [
+                        self._a * w[0] - self._b * w[1] + self._s,
+                        self._b * w[0] + self._a * w[1] + self._t,
+                    ],
+                )
             else:
-                return vector(ring, [
-                    self._a * w[0] + self._b * w[1] + self._s,
-                    self._b * w[0] - self._a * w[1] + self._t])
+                return vector(
+                    ring,
+                    [
+                        self._a * w[0] + self._b * w[1] + self._s,
+                        self._b * w[0] - self._a * w[1] + self._t,
+                    ],
+                )
 
     def _repr_(self):
         r"""
         TESTS::
 
             sage: from flatsurf.geometry.similarity import SimilarityGroup
             sage: S = SimilarityGroup(QQ)
@@ -320,19 +344,20 @@
             sage: S((1,-2/3))
             (x, y) |-> (x + 1, y - 2/3)
             sage: S((-1,0,2/3,3))
             (x, y) |-> (-x + 2/3, -y + 3)
             sage: S((-1,0,2/3,3,-1))
             (x, y) |-> (-x + 2/3, y + 3)
         """
-        R = self.parent().base_ring()['x','y']
-        x,y = R.gens()
+        R = self.parent().base_ring()["x", "y"]
+        x, y = R.gens()
         return "(x, y) |-> ({}, {})".format(
-                    self._a*x - self._sign*self._b*y + self._s,
-                    self._b*x + self._sign*self._a*y + self._t)
+            self._a * x - self._sign * self._b * y + self._s,
+            self._b * x + self._sign * self._a * y + self._t,
+        )
 
     def __eq__(self, other):
         r"""
         TESTS::
 
             sage: from flatsurf.geometry.similarity import SimilarityGroup
             sage: S = SimilarityGroup(QQ)
@@ -343,23 +368,25 @@
             sage: S((1,0,0,0)) == S((0,1,0,0))
             False
             sage: S((1,0,0,0,1)) == S((1,0,0,0,-1))
             False
         """
         if other is None:
             return False
-        if type(other)==int:
+        if type(other) == int:
             return False
         if self.parent() != other.parent():
             return False
-        return self._a == other._a and \
-               self._b == other._b and \
-               self._s == other._s and \
-               self._t == other._t and \
-               self._sign == other._sign
+        return (
+            self._a == other._a
+            and self._b == other._b
+            and self._s == other._s
+            and self._t == other._t
+            and self._sign == other._sign
+        )
 
     def __ne__(self, other):
         return not (self == other)
 
     def matrix(self):
         r"""
         Return the 3x3 matrix representative of this element
@@ -375,17 +402,26 @@
             [   0    0    1]
         """
         P = self.parent()
         M = P._matrix_space_3x3()
         z = P._ring.zero()
         o = P._ring.one()
         return M(
-            [self._a, -self._sign*self._b, self._s,
-             self._b, +self._sign*self._a, self._t,
-            z, z, o])
+            [
+                self._a,
+                -self._sign * self._b,
+                self._s,
+                self._b,
+                +self._sign * self._a,
+                self._t,
+                z,
+                z,
+                o,
+            ]
+        )
 
     def derivative(self):
         r"""
         Return the 2x2 matrix corresponding to the derivative of this element
 
         EXAMPLES::
 
@@ -393,37 +429,16 @@
             sage: S = SimilarityGroup(QQ)
 
             sage: S((1,-2/3,1,1,-1)).derivative()
             [   1 -2/3]
             [-2/3   -1]
         """
         M = self.parent()._matrix_space_2x2()
-        return M([self._a, -self._sign*self._b, self._b,  self._sign*self._a])
-
-    # OLD AND DEPRECATED
+        return M([self._a, -self._sign * self._b, self._b, self._sign * self._a])
 
-    def a(self):
-        from sage.misc.superseded import deprecation
-        deprecation(42, "Do not use .a()")
-        return self._a
-
-    def b(self):
-        from sage.misc.superseded import deprecation
-        deprecation(42, "Do not use .b()")
-        return self._b
-
-    def s(self):
-        from sage.misc.superseded import deprecation
-        deprecation(42, "Do not use .s()")
-        return self._s
-
-    def t(self):
-        from sage.misc.superseded import deprecation
-        deprecation(42, "Do not use .t()")
-        return self._t
 
 class SimilarityGroup(UniqueRepresentation, Group):
     r"""
     The group of possibly orientation reversing similarities in the plane.
 
     This is the group generated by rotations, translations and dilations.
     """
@@ -439,24 +454,27 @@
         """
         self._ring = base_ring
         Group.__init__(self, category=Groups().Infinite())
 
     @cached_method
     def _matrix_space_2x2(self):
         from sage.matrix.matrix_space import MatrixSpace
+
         return MatrixSpace(self._ring, 2)
 
     @cached_method
     def _matrix_space_3x3(self):
         from sage.matrix.matrix_space import MatrixSpace
+
         return MatrixSpace(self._ring, 3)
 
     @cached_method
     def _vector_space(self):
         from sage.modules.free_module import VectorSpace
+
         return VectorSpace(self._ring, 2)
 
     def _element_constructor_(self, *args, **kwds):
         r"""
         TESTS::
 
             sage: from flatsurf.geometry.similarity import SimilarityGroup
@@ -478,55 +496,61 @@
 
         a = self._ring.one()
         b = s = t = self._ring.zero()
         sign = ZZ_1
 
         # TODO: 2x2 and 3x3 matrix input
 
-        if isinstance(x, (tuple,list)):
+        if isinstance(x, (tuple, list)):
             if len(x) == 2:
-                s,t = map(self._ring, x)
+                s, t = map(self._ring, x)
             elif len(x) == 4:
-                a,b,s,t = map(self._ring, x)
+                a, b, s, t = map(self._ring, x)
             elif len(x) == 5:
-                a,b,s,t = map(self._ring, x[:4])
+                a, b, s, t = map(self._ring, x[:4])
                 sign = ZZ(x[4])
             else:
-                raise ValueError("can not construct a similarity from a list of length {}".format(len(x)))
+                raise ValueError(
+                    "can not construct a similarity from a list of length {}".format(
+                        len(x)
+                    )
+                )
         elif is_Matrix(x):
             #   a -sb
             #   b sa
             if x.nrows() == x.ncols() == 2:
-                a,c,b,d = x.list()
+                a, c, b, d = x.list()
                 if a == d and b == -c:
                     sign = ZZ_1
                 elif a == -d and b == c:
                     sign = ZZ_m1
                 else:
                     raise ValueError("not a similarity matrix")
             elif x.nrows() == x.ncols() == 3:
                 raise NotImplementedError
             else:
                 raise ValueError("invalid dimension for matrix input")
         elif isinstance(x, FreeModuleElement):
             if len(x) == 2:
                 if x.base_ring() is self._ring:
-                    s,t = x
+                    s, t = x
                 else:
-                    s,t = map(self._ring, x)
+                    s, t = map(self._ring, x)
             else:
                 raise ValueError("invalid dimension for vector input")
         else:
             p = parent(x)
             if self._ring.has_coerce_map_from(p):
                 a = self._ring(x)
             else:
-                raise ValueError("element in %s cannot be used to create element in %s"%(p, self))
+                raise ValueError(
+                    "element in %s cannot be used to create element in %s" % (p, self)
+                )
 
-        if (a*a + b*b).is_zero():
+        if (a * a + b * b).is_zero():
             raise ValueError("not invertible")
 
         return self.element_class(self, a, b, s, t, sign)
 
     def _coerce_map_from_(self, S):
         if self._ring.has_coerce_map_from(S):
             return True
@@ -549,22 +573,117 @@
 
             sage: from flatsurf.geometry.similarity import SimilarityGroup
             sage: SimilarityGroup(QQ).one()
             (x, y) |-> (x, y)
             sage: SimilarityGroup(QQ).one().is_one()
             True
         """
-        return self.element_class(self,
-                self._ring.one(),  # a
-                self._ring.zero(), # b
-                self._ring.zero(), # s
-                self._ring.zero(), # t
-                ZZ_1)              # sign
+        return self.element_class(
+            self,
+            self._ring.one(),  # a
+            self._ring.zero(),  # b
+            self._ring.zero(),  # s
+            self._ring.zero(),  # t
+            ZZ_1,
+        )  # sign
+
+    def _an_element_(self):
+        r"""
+        Return a typical element of this group.
 
-    def an_element(self):
+        EXAMPLES:
+
+            sage: from flatsurf.geometry.similarity import SimilarityGroup
+
+            sage: SimilarityGroup(QQ)._an_element_()
+            (x, y) |-> (3*x + 4*y + 2, 4*x - 3*y - 1)
+
+            sage: SimilarityGroup(QQ).an_element()
+            (x, y) |-> (3*x + 4*y + 2, 4*x - 3*y - 1)
+
+        .. SEEALSO::
+
+            :meth:`sage.structure.parent.Parent.an_element` which relies on
+            this method and should be called instead
+
+        """
         return self(3, 4, 2, -1, -1)
 
     def is_abelian(self):
         return False
 
     def base_ring(self):
         return self._ring
+
+
+def similarity_from_vectors(u, v, matrix_space=None):
+    r"""
+    Return the unique similarity matrix that maps ``u`` to ``v``.
+
+    EXAMPLES::
+
+        sage: from flatsurf.geometry.similarity import similarity_from_vectors
+
+        sage: V = VectorSpace(QQ,2)
+        sage: u = V((1,0))
+        sage: v = V((0,1))
+        sage: m = similarity_from_vectors(u,v); m
+        [ 0 -1]
+        [ 1  0]
+        sage: m*u == v
+        True
+
+        sage: u = V((2,1))
+        sage: v = V((1,-2))
+        sage: m = similarity_from_vectors(u,v); m
+        [ 0  1]
+        [-1  0]
+        sage: m * u == v
+        True
+
+    An example built from the Pythagorean triple 3^2 + 4^2 = 5^2::
+
+        sage: u2 = V((5,0))
+        sage: v2 = V((3,4))
+        sage: m = similarity_from_vectors(u2,v2); m
+        [ 3/5 -4/5]
+        [ 4/5  3/5]
+        sage: m * u2 == v2
+        True
+
+    Some test over number fields::
+
+        sage: K.<sqrt2> = NumberField(x^2-2, embedding=1.4142)
+        sage: V = VectorSpace(K,2)
+        sage: u = V((sqrt2,0))
+        sage: v = V((1, 1))
+        sage: m = similarity_from_vectors(u,v); m
+        [ 1/2*sqrt2 -1/2*sqrt2]
+        [ 1/2*sqrt2  1/2*sqrt2]
+        sage: m*u == v
+        True
+
+        sage: m = similarity_from_vectors(u, 2*v); m
+        [ sqrt2 -sqrt2]
+        [ sqrt2  sqrt2]
+        sage: m*u == 2*v
+        True
+
+    """
+    if u.parent() is not v.parent():
+        raise ValueError
+
+    if matrix_space is None:
+        from sage.matrix.matrix_space import MatrixSpace
+
+        matrix_space = MatrixSpace(u.base_ring(), 2)
+
+    if u == v:
+        return matrix_space.one()
+
+    sqnorm_u = u[0] * u[0] + u[1] * u[1]
+    cos_uv = (u[0] * v[0] + u[1] * v[1]) / sqnorm_u
+    sin_uv = (u[0] * v[1] - u[1] * v[0]) / sqnorm_u
+
+    m = matrix_space([cos_uv, -sin_uv, sin_uv, cos_uv])
+    m.set_immutable()
+    return m
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/similarity_surface.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/categories/similarity_surfaces.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,2363 +1,2615 @@
-# -*- coding: utf-8 -*-
 r"""
-Similarity surfaces.
+The category of similarity surfaces.
+
+This module provides shared functionality for all surfaces in sage-flatsurf
+that are built from Euclidean polygons that are glued by similarities, i.e.,
+identified edges can be transformed into each other by application of rotation
+and homothety (dilation) and translation.
+
+See :mod:`flatsurf.geometry.categories` for a general description of the
+category framework in sage-flatsurf.
+
+Normally, you won't create this (or any other) category directly. The correct
+category is automatically determined for immutable surfaces.
+
+EXAMPLES::
+
+    sage: from flatsurf import MutableOrientedSimilaritySurface
+    sage: C = MutableOrientedSimilaritySurface(QQ).category()
+
+    sage: from flatsurf.geometry.categories import SimilaritySurfaces
+    sage: C.is_subcategory(SimilaritySurfaces())
+    True
+
+The easiest way to construct a similarity surface is to use the constructions
+from
+:class:`flatsurf.geometry.similarity_surface_generators.SimilaritySurfaceGenerators`::
+
+    sage: from flatsurf import Polygon, similarity_surfaces
+    sage: P = Polygon(vertices=[(0,0), (2,0), (1,4), (0,5)])
+    sage: similarity_surfaces.self_glued_polygon(P)
+    Half-Translation Surface in Q_0(0, -1^4) built from a quadrilateral
+
+Another way is to build a surface from scratch (using e.g.
+:class:`flatsurf.geometry.surface.MutableOrientedSimilaritySurface`)::
+
+    sage: P = Polygon(vertices=[(0,0), (1,0), (1,1), (0,1)])
+    sage: S = MutableOrientedSimilaritySurface(QQ)
+    sage: S.add_polygon(P)
+    0
+    sage: S.add_polygon(2*P)
+    1
+    sage: S.add_polygon(3*P)
+    2
+    sage: S.glue((0, 1), (1, 3))
+    sage: S.glue((0, 0), (2, 2))
+    sage: S.glue((0, 2), (2, 0))
+    sage: S.glue((0, 3), (1, 1))
+    sage: S.glue((1, 2), (2, 1))
+    sage: S.glue((1, 0), (2, 3))
+    sage: S
+    Surface built from 3 squares
+
+To perform a sanity check on the obtained surface, you can run its test
+suite::
+
+    sage: TestSuite(S).run()
+
+If there are no errors reported, no consistency problems could be detected in
+your surface.
+
+Once you mark the surface as immutable, it gets more functionality, e.g.,
+coming from its structure as a translation surface. This also adds more tests
+to its test suite::
+
+    sage: S.category()
+    Category of finite type oriented similarity surfaces
+    sage: S.set_immutable()
+    sage: S.category()
+    Category of connected without boundary finite type oriented rational similarity surfaces
+
+    sage: TestSuite(S).run()
+
+In the following example, we attempt to build a broken surface by gluing more
+than two edges to each other; however, edges get unglued automatically::
+
+    sage: S = MutableOrientedSimilaritySurface.from_surface(S)
+    sage: S.glue((0, 0), (0, 3))
+    sage: S.glue((0, 1), (0, 3))
+    sage: S.glue((0, 2), (0, 3))
+
+    sage: S.gluings()
+    (((0, 2), (0, 3)), ((0, 3), (0, 2)), ((1, 0), (2, 3)), ((1, 2), (2, 1)), ((2, 1), (1, 2)), ((2, 3), (1, 0)))
+
+    sage: S.set_immutable()
+    sage: S.category()
+    Category of with boundary finite type oriented rational similarity surfaces
+    sage: TestSuite(S).run()
+
+If we don't glue all the edges, we get a surface with boundary::
+
+    sage: P = Polygon(vertices=[(0,0), (1,0), (1,1), (0,1)])
+    sage: S = MutableOrientedSimilaritySurface(QQ)
+    sage: S.add_polygon(P)
+    0
+    sage: TestSuite(S).run()
+
 """
-#*********************************************************************
+# ****************************************************************************
 #  This file is part of sage-flatsurf.
 #
 #        Copyright (C) 2016-2020 Vincent Delecroix
-#                      2020-2022 Julian Rüth
+#                           2023 Julian Rüth
 #
 #  sage-flatsurf is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 2 of the License, or
 #  (at your option) any later version.
 #
 #  sage-flatsurf is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
-#*********************************************************************
-
-from __future__ import absolute_import, print_function, division
-from six.moves import range
-from six import iteritems
+# ****************************************************************************
 
+from flatsurf.geometry.categories.surface_category import (
+    SurfaceCategory,
+    SurfaceCategoryWithAxiom,
+)
+from sage.categories.category_with_axiom import all_axioms
 from sage.misc.cachefunc import cached_method
-from sage.misc.sage_unittest import TestSuite
-
-from sage.structure.sage_object import SageObject
-
-from sage.rings.infinity import Infinity
-
-from sage.rings.all import ZZ, QQ, AA, NumberField
-
-from sage.modules.free_module_element import vector
-
-from .similarity import SimilarityGroup
-from .polygon import ConvexPolygons, wedge_product
+from sage.all import QQ, AA
 
-from .surface import Surface, Surface_dict, Surface_list, LabelComparator
-from .surface_objects import Singularity, SaddleConnection, SurfacePoint
-from .circle import Circle
-from .matrix_2x2 import similarity_from_vectors
 
-ZZ_1 = ZZ.one()
-ZZ_2 = ZZ_1 + ZZ_1
-
-
-class SimilaritySurface(SageObject):
+class SimilaritySurfaces(SurfaceCategory):
     r"""
-    An oriented surface built from a set of polygons and edges identified with
-    similarities (i.e. composition of homothety, rotations and translations).
-
-    Each polygon is identified with a unique key (its label). The choice of the
-    label of the polygons is done at startup. If the set is finite then by
-    default the labels are the first non-negative integers 0,1,...
-
-    The edges are labeled by a pair ``(polygon label, edge number)``.
-
-    EXAMPLES:
-
-    The easiest way to construct a similarity surface is to use the pre-built
-    constructions from
-    :class:`flatsurf.geometry.similarity_surface_generators.SimilaritySurfaceGenerators`::
-
-        sage: from flatsurf import polygons, similarity_surfaces
-        sage: P = polygons(vertices=[(0,0), (2,0), (1,4), (0,5)])
-        sage: similarity_surfaces.self_glued_polygon(P)
-        HalfTranslationSurface built from 1 polygon
-
-    The second way is to build a surface (using e.g. :class:`flatsurf.geometry.surface.Surface_list`)
-    and then use this surface as an argument for class:`SimilaritySurface`)::
-
-        sage: from flatsurf.geometry.similarity_surface import SimilaritySurface
-        sage: from flatsurf.geometry.surface import Surface_list
-        sage: P = polygons(vertices=[(0,0), (1,0), (1,1), (0,1)])
-        sage: Stop = Surface_list(QQ)
-        sage: Stop.add_polygon(P)
-        0
-        sage: Stop.add_polygon(2*P)
-        1
-        sage: Stop.add_polygon(3*P)
-        2
-        sage: Stop.set_edge_pairing(0, 1, 1, 3)
-        sage: Stop.set_edge_pairing(0, 0, 2, 2)
-        sage: Stop.set_edge_pairing(0, 2, 2, 0)
-        sage: Stop.set_edge_pairing(0, 3, 1, 1)
-        sage: Stop.set_edge_pairing(1, 2, 2, 1)
-        sage: Stop.set_edge_pairing(1, 0, 2, 3)
-        sage: S = SimilaritySurface(Stop)
-        sage: S
-        SimilaritySurface built from 3 polygons
-
-    To perform a sanity check on the obtained surface, you can run its test
-    suite::
-
-        sage: TestSuite(S).run()
-
-    In the following example, we build two broken surfaces and
-    check that the test suite fails as expected::
-
-        sage: P = polygons(vertices=[(0,0), (1,0), (1,1), (0,1)])
-        sage: Stop = Surface_list(QQ)
-        sage: Stop.add_polygon(P)
-        0
-        sage: S = SimilaritySurface(Stop)
-        sage: TestSuite(S).run()
-        ...
-          AssertionError: edge (0, 0) is not glued
-          ------------------------------------------------------------
-          The following tests failed: _test_gluings
-        Failure in _test_underlying_surface
-        The following tests failed: _test_underlying_surface
-
-        sage: Stop.set_edge_pairing(0, 0, 0, 3)
-        sage: Stop.set_edge_pairing(0, 1, 0, 3)
-        sage: Stop.set_edge_pairing(0, 2, 0, 3)
-        sage: S = SimilaritySurface(Stop)
-        sage: TestSuite(S).run()
-        ...
-          AssertionError: edge gluing is not a pairing:
-          (0, 0) -> (0, 3) -> (0, 2)
-          ------------------------------------------------------------
-          The following tests failed: _test_gluings
-        Failure in _test_underlying_surface
-        The following tests failed: _test_underlying_surface
-
-    Finally, you can also implement a similarity surface by inheriting from
-    :class:`SimilaritySurface` and implement the methods:
-
-    - ``base_ring(self)``: the base ring in which coordinates lives
-
-    - ``polygon(self, lab)``: the polygon associated to the label ``lab``
+    The category of surfaces built from polygons with edges identified by
+    similarities.
 
-    - ``base_label(self)``: which label to use as the base one
+    EXAMPLES::
 
-    - ``opposite_edge(self, lab, edge)``: a pair (``other_label``,
-      ``other_edge``) representing the edge being glued
+        sage: from flatsurf.geometry.categories import SimilaritySurfaces
+        sage: SimilaritySurfaces()
+        Category of similarity surfaces
 
-    - ``is_finite(self)``: whether the surface is built from finitely many polygons
     """
-    def __init__(self, surface):
-        r"""
-        TESTS::
-
-            sage: from flatsurf.geometry.similarity_surface import SimilaritySurface
-            sage: SimilaritySurface(3)
-            Traceback (most recent call last):
-            ...
-            TypeError: invalid argument surface=3 to build a similarity surface
-        """
-        if isinstance(surface, SimilaritySurface):
-            self._s = surface.underlying_surface()
-        elif isinstance(surface, Surface):
-            self._s = surface
-        else:
-            raise TypeError("invalid argument surface={} to build a similarity surface".format(surface))
-
-    @cached_method
-    def _matrix_space(self):
-        from sage.matrix.matrix_space import MatrixSpace
-        return MatrixSpace(self.base_ring(), 2)
 
-    def underlying_surface(self):
+    def super_categories(self):
         r"""
-        Return the surface underlying this SimilaritySurface.
-        """
-        return self._s
+        Return the categories that a similarity surface is also a member of,
+        namely the surfaces formed by Euclidean polygons.
 
-    def _test_underlying_surface(self, **options):
-        is_sub_testsuite = 'tester' in options
-        tester = self._tester(**options)
-        tester.info("")
-
-        # TODO: this nested subsuite is very fragile since we have no
-        #       way of forwarding the doctests to be skipped... Since
-        #       for now, the unique usage of this is for pickling of
-        #       infinite surface we provide that manually
-        if not self._s.is_finite():
-            skip = ['_test_pickling']
-        else:
-            skip = []
-
-        TestSuite(self._s).run(verbose = tester._verbose,
-                                prefix = tester._prefix + "  ",
-                                raise_on_failure=is_sub_testsuite,
-                                skip=skip)
-        tester.info(tester._prefix + " ", newline=False)
-
-    def base_ring(self):
-        r"""
-        The field on which the coordinates of ``self`` live.
+        EXAMPLES::
 
-        This method must be overriden in subclasses!
-        """
-        return self._s.base_ring()
+            sage: from flatsurf.geometry.categories import SimilaritySurfaces
+            sage: SimilaritySurfaces().super_categories()
+            [Category of euclidean polygonal surfaces]
 
-    def polygon(self, lab):
-        r"""
-        Return the polygon with label ``lab``.
         """
-        return self._s.polygon(lab)
+        from flatsurf.geometry.categories.euclidean_polygonal_surfaces import (
+            EuclideanPolygonalSurfaces,
+        )
 
-    def base_label(self):
-        r"""
-        Always returns the same label.
-        """
-        return self._s.base_label()
+        return [EuclideanPolygonalSurfaces()]
 
-    def opposite_edge(self, l, e=None):
+    class ParentMethods:
         r"""
-        Given the label ``l`` of a polygon and an edge ``e`` in that polygon
-        returns the pair (``ll``, ``ee``) to which this edge is glued.
-        If e is not provided, then it expects the only parameter to be
-        the pair (``l``,``e``) and will again return a the pair (``ll``,``ee``).
-        """
-        if e is None:
-            return self._s.opposite_edge(l[0],l[1])
-        return self._s.opposite_edge(l,e)
+        Provides methods available to all surfaces that are built from
+        Euclidean polygons that are glued by similarities.
 
-    def is_finite(self):
-        r"""
-        Return whether or not the surface is finite.
-        """
-        return self._s.is_finite()
-
-    def is_mutable(self):
-        r"""
-        Return if the surface is mutable.
-        """
-        return self._s.is_mutable()
-
-    def set_immutable(self):
-        r"""
-        Mark the surface as immutable.
+        If you want to add functionality for such surfaces you most likely
+        want to put it here.
         """
-        self._s.set_immutable()
 
-    def is_triangulated(self, limit=None):
-        return self._s.is_triangulated(limit=limit)
+        def refined_category(self):
+            r"""
+            Return the smallest subcategory that this surface is in by consulting
+            how its edges are glued.
 
-    #
-    # generic methods
-    #
-
-    #def compute_surface_type_from_gluings(self,limit=None):
-    #    r"""
-    #    Compute the surface type by looking at the edge gluings.
-    #    If limit is defined, we try to guess the type by looking at limit many edges.
-    #    """
-    #    if limit is None:
-    #        if not self.is_finite():
-    #            raise ValueError("Need a limit when working with an infinite surface.")
-    #        it = self.edge_iterator()
-    #        label,edge = it.next()
-    #        # Use honest matrices!
-    #        m = SimilaritySurface_generic.edge_matrix(self,label,edge)
-    #        surface_type = surface_type_from_matrix(m)
-    #        for label,edge in it:
-    #            # Use honest matrices!
-    #            m = SimilaritySurface_generic.edge_matrix(self,label,edge)
-    #            surface_type = combine_surface_types(surface_type, surface_type_from_matrix(m))
-    #        return surface_type
-    #    else:
-    #        count=0
-    #        it = self.edge_iterator()
-    #        label,edge = it.next()
-    #        # Use honest matrices!
-    #        m = SimilaritySurface_generic.edge_matrix(self,label,edge)
-    #        surface_type = surface_type_from_matrix(m)
-    #        for label,edge in it:
-    #            # Use honest matrices!
-    #            m = SimilaritySurface_generic.edge_matrix(self,label,edge)
-    #            surface_type = combine_surface_types(surface_type, surface_type_from_matrix(m))
-    #            count=count+1
-    #            if count >= limit:
-    #                return surface_type
-    #        return surface_type
+            The result of this method can be fed to ``_refine_category_`` to
+            change the category of the surface (and enable functionality
+            specific to the smaller classes of surfaces.)
 
-    def walker(self):
-        return self._s.walker()
 
-    def label_iterator(self, polygons=False):
-        r"""
-        Iterator over all polygon labels.
+            .. NOTE::
 
-        If the keyword polygons is True then we return pairs (label, polygon)
-        instead of just labels.
-        """
-        if polygons:
-            return self._s.label_polygon_iterator()
-        else:
-            return self._s.label_iterator()
+                If a surface cannot implement the various ``is_`` methods used in
+                the implementation of this method (i.e., if any of them throws a
+                ``NotImplementedError``,) then this method ``refined_category``
+                must be overridden to skip that check. We don't want to actively
+                catch a ``NotImplementedError`` and instead encourage authors
+                to explicitly select the category their surfaces lives in.
 
-    def edge_iterator(self, gluings=False):
-        r"""
-        Iterate over the edges of polygons, which are pairs (l,e) where l is a polygon label, 0 <= e < N and N is the number of edges of the polygon with label l.
+            EXAMPLES::
 
-        If the keyword gluings is set to true, then we iterate over ordered
-        pairs of edges ((l,e),(ll,ee)) where edge (l,e) is glued to (ll,ee).
+                sage: from flatsurf import MutableOrientedSimilaritySurface
+                sage: S = MutableOrientedSimilaritySurface(QQ)
 
-        EXAMPLES::
+                sage: from flatsurf import polygons
+                sage: S.add_polygon(polygons.square(), label=0)
+                0
+                sage: S.refined_category()
+                Category of connected with boundary finite type translation surfaces
 
-            sage: from flatsurf import ConvexPolygons
-            sage: P = ConvexPolygons(QQ)
-            sage: tri0=P([(1,0),(0,1),(-1,-1)])
-            sage: tri1=P([(-1,0),(0,-1),(1,1)])
-            sage: gluings=[((0,0),(1,0)),((0,1),(1,1)),((0,2),(1,2))]
-            sage: from flatsurf.geometry.surface import surface_list_from_polygons_and_gluings
-            sage: from flatsurf.geometry.translation_surface import TranslationSurface
-            sage: s=TranslationSurface(surface_list_from_polygons_and_gluings([tri0,tri1], gluings))
-            sage: for edge in s.edge_iterator():
-            ....:     print(edge)
-            (0, 0)
-            (0, 1)
-            (0, 2)
-            (1, 0)
-            (1, 1)
-            (1, 2)
-        """
-        if gluings:
-            return self._s.edge_gluing_iterator()
-        else:
-            return self._s.edge_iterator()
+                sage: S.glue((0, 0), (0, 2))
+                sage: S.glue((0, 1), (0, 3))
+                sage: S.refined_category()
+                Category of connected without boundary finite type translation surfaces
 
-    def num_polygons(self):
-        r"""
-        Return the number of polygons.
-        """
-        return self._s.num_polygons()
+            """
+            from flatsurf.geometry.categories.polygonal_surfaces import (
+                PolygonalSurfaces,
+            )
 
-    def num_edges(self):
-        r"""
-        Return the total number of edges of all polygons used.
-        """
-        return self._s.num_edges()
+            category = PolygonalSurfaces.ParentMethods.refined_category(self)
 
-    def num_singularities(self):
-        r"""
-        EXAMPLES::
+            if self.is_cone_surface():
+                from flatsurf.geometry.categories.cone_surfaces import ConeSurfaces
 
-            sage: from flatsurf import *
+                category &= ConeSurfaces()
 
-            sage: translation_surfaces.regular_octagon().num_singularities()
-            1
+            if self.is_dilation_surface():
+                from flatsurf.geometry.categories.dilation_surfaces import (
+                    DilationSurfaces,
+                )
 
-            sage: S = SymmetricGroup(4)
-            sage: r = S('(1,2)(3,4)')
-            sage: u = S('(2,3)')
-            sage: translation_surfaces.origami(r,u).num_singularities()
-            2
-
-            sage: S = SymmetricGroup(8)
-            sage: r = S('(1,2,3,4,5,6,7,8)')
-            sage: u = S('(1,8,5,4)(2,3)(6,7)')
-            sage: translation_surfaces.origami(r,u).num_singularities()
-            4
-        """
-        if not self.is_finite():
-            raise ValueError("the method only work for finite surfaces")
+                category &= DilationSurfaces()
 
-        # NOTE:
-        # the very same code is implemented in the method angles (translation
-        # surfaces). we should factor out the code
-        edges = set((p,e) for p in self.label_iterator() for e in range(self.polygon(p).num_edges()))
-
-        n = ZZ(0)
-        while edges:
-            p,e = edges.pop()
-            n += 1
-            ee = (e-1) % self.polygon(p).num_edges()
-            p,e = self.opposite_edge(p,ee)
-            while (p,e) in edges:
-                edges.remove((p,e))
-                ee = (e-1) % self.polygon(p).num_edges()
-                p,e = self.opposite_edge(p,ee)
-        return n
-
-    def _repr_(self):
-        if self.num_polygons() == Infinity:
-            num = 'infinitely many'
-        else:
-            num = str(self.num_polygons())
-
-        if self.num_polygons() == 1:
-            end = ""
-        else:
-            end = "s"
+                if self.is_dilation_surface(positive=True):
+                    category &= DilationSurfaces().Positive()
 
-        return "{} built from {} polygon{}".format(self.__class__.__name__, num, end)
+                    if self.is_translation_surface():
+                        from flatsurf.geometry.categories.translation_surfaces import (
+                            TranslationSurfaces,
+                        )
 
-    @cached_method
-    def edge_matrix(self, p, e=None):
-        r"""
-        Returns the 2x2 matrix representing a similarity which when applied to the polygon with label `p`
-        makes it so the edge `e` can be glued to its opposite edge by translation.
+                        category &= TranslationSurfaces()
+                elif self.is_translation_surface(positive=False):
+                    from flatsurf.geometry.categories.half_translation_surfaces import (
+                        HalfTranslationSurfaces,
+                    )
 
-        If `e` is not provided, then `p` should be a pair consisting of a polygon label and an edge.
+                    category &= HalfTranslationSurfaces()
 
-        EXAMPLES::
+            if "Rational" not in category.axioms():
+                if self.is_rational_surface():
+                    category = category.Rational()
 
-            sage: from flatsurf.geometry.similarity_surface_generators import SimilaritySurfaceGenerators
-            sage: s = SimilaritySurfaceGenerators.example()
-            sage: print(s.polygon(0))
-            Polygon: (0, 0), (2, -2), (2, 0)
-            sage: print(s.polygon(1))
-            Polygon: (0, 0), (2, 0), (1, 3)
-            sage: s.opposite_edge(0,0)
-            (1, 1)
-            sage: m = s.edge_matrix(0, 0)
-            sage: m
-            [   1  1/2]
-            [-1/2    1]
-            sage: m * vector((2,-2)) == -vector((-1, 3))
-            True
-        """
-        if e is None:
-            import warning
-            warning.warn('edge_matrix will now only take two arguments')
-            p, e = p
-        u = self.polygon(p).edge(e)
-        pp, ee = self.opposite_edge(p, e)
-        v = self.polygon(pp).edge(ee)
+            return category
 
-        # be careful, because of the orientation, it is -v and not v
-        return similarity_from_vectors(u, -v, self._matrix_space())
+        def is_cone_surface(self):
+            r"""
+            Return whether this surface is a cone surface, i.e., glued edges
+            can be transformed into each other with isometries.
 
-    def edge_transformation(self, p, e):
-        r"""
-        Return the similarity bringing the provided edge to the opposite edge.
+            .. NOTE::
 
-        EXAMPLES::
+                This is a stronger requirement than the usual
+                definition of a cone surface, see :mod:`.cone_surfaces` for
+                details.
 
-            sage: from flatsurf.geometry.similarity_surface_generators import SimilaritySurfaceGenerators
-            sage: s = SimilaritySurfaceGenerators.example()
-            sage: print(s.polygon(0))
-            Polygon: (0, 0), (2, -2), (2, 0)
-            sage: print(s.polygon(1))
-            Polygon: (0, 0), (2, 0), (1, 3)
-            sage: print(s.opposite_edge(0,0))
-            (1, 1)
-            sage: g = s.edge_transformation(0,0)
-            sage: g((0,0))
-            (1, 3)
-            sage: g((2,-2))
-            (2, 0)
-        """
-        G = SimilarityGroup(self.base_ring())
-        q = self.polygon(p)
-        a = q.vertex(e)
-        b = q.vertex(e+1)
-        # This is the similarity carrying the origin to a and (1,0) to b:
-        g = G(b[0] - a[0], b[1] - a[1], a[0], a[1])
-
-        pp, ee = self.opposite_edge(p, e)
-        qq = self.polygon(pp)
-        # Be careful here: opposite vertices are identified
-        aa = qq.vertex(ee+1)
-        bb = qq.vertex(ee)
-        # This is the similarity carrying the origin to aa and (1,0) to bb:
-        gg = G(bb[0] - aa[0], bb[1] - aa[1], aa[0], aa[1])
+            .. NOTE::
 
-        # This is the similarity carrying (a,b) to (aa,bb):
-        return gg / g
+                This method is used to determine whether this surface is in the
+                category of :class:`~.cone_surfaces.ConeSurfaces`. Surfaces can
+                override this method to perform specialized logic, see the note
+                in :mod:`flatsurf.geometry.categories` for performance
+                considerations.
 
-    def set_vertex_zero(self, label, v, in_place=False):
-        r"""
-        Applies a combinatorial rotation to the polygon with the provided label.
+            EXAMPLES::
 
-        This makes what is currently vertex v of this polygon vertex 0. In other words,
-        what is currently vertex (or edge) e will now become vertex (e-v)%n where
-        n is the number of sides of the polygon.
-
-        For the updated polygons, the polygons will be translated so that vertex
-        0 is the origin.
-
-        EXAMPLES:
-
-        Example with polygon glued to another polygon::
-
-            sage: from flatsurf import *
-            sage: s = translation_surfaces.veech_double_n_gon(4)
-            sage: s.polygon(0)
-            Polygon: (0, 0), (1, 0), (1, 1), (0, 1)
-            sage: [s.opposite_edge(0,i) for i in range(4)]
-            [(1, 0), (1, 1), (1, 2), (1, 3)]
-            sage: ss = s.set_vertex_zero(0,1)
-            sage: ss.polygon(0)
-            Polygon: (0, 0), (0, 1), (-1, 1), (-1, 0)
-            sage: [ss.opposite_edge(0,i) for i in range(4)]
-            [(1, 1), (1, 2), (1, 3), (1, 0)]
-            sage: TestSuite(ss).run()
-
-        Example with polygon glued to self::
-
-            sage: s = translation_surfaces.veech_2n_gon(2)
-            sage: s.polygon(0)
-            Polygon: (0, 0), (1, 0), (1, 1), (0, 1)
-            sage: [s.opposite_edge(0,i) for i in range(4)]
-            [(0, 2), (0, 3), (0, 0), (0, 1)]
-            sage: ss = s.set_vertex_zero(0,3)
-            sage: ss.polygon(0)
-            Polygon: (0, 0), (0, -1), (1, -1), (1, 0)
-            sage: [ss.opposite_edge(0,i) for i in range(4)]
-            [(0, 2), (0, 3), (0, 0), (0, 1)]
-            sage: TestSuite(ss).run()
-        """
-        if in_place:
-            us = self.underlying_surface()
-            if not us.is_mutable():
-                raise ValueError("set_vertex_zero can only be done in_place for a mutable surface.")
-            p = us.polygon(label)
-            n=p.num_edges()
-            assert 0<=v and v<n
-            glue=[]
-            P = ConvexPolygons(us.base_ring())
-            pp = P(edges=[p.edge((i+v)%n) for i in range(n)])
-
-            for i in range(n):
-                e=(v+i)%n
-                ll,ee = us.opposite_edge(label,e)
-                if ll==label:
-                    ee = (ee+n-v)%n
-                glue.append((ll,ee))
-
-            us.change_polygon(label,pp,gluing_list=glue)
-            return self
-        else:
-            return self.copy(mutable=True).set_vertex_zero(label,v,in_place=True)
+                sage: from flatsurf import Polygon, similarity_surfaces
+                sage: P = Polygon(vertices=[(0,0), (1,0), (1,1), (0,1)])
+                sage: S = similarity_surfaces.self_glued_polygon(P)
+                sage: S.is_cone_surface()
+                True
 
-    def _label_comparator(self):
-        r"""
-        Return a LabelComparator, which provides a fixed total ordering on the polygon labels.
-        """
-        try:
-            return self._lc
-        except AttributeError:
-            self._lc = LabelComparator()
-            return self._lc
+            """
+            if self.is_translation_surface():
+                return True
 
-    def relabel(self, relabeling_map, in_place=False):
-        r"""
-        Attempt to relabel the polygons according to a relabeling_map, which takes as input
-        a current label and outputs a new label for the same polygon. The method returns a pair
-        (surface,success) where surface is the relabeled surface, and success is a boolean value
-        indicating the success of the operation. The operation will fail if the implementation of the
-        underlying surface does not support labels used in the image of the relabeling map. In this case,
-        other (arbitrary) labels will be used to replace the labels of the surface, and the resulting
-        surface should still be okay.
-
-        Currently, the relabeling_map must be a dictionary.
-
-        If in_place is True then the relabeling is done to the current surface, otherwise a
-        mutable copy is made before relabeling.
-
-        ToDo:
-          - Allow relabeling_map to be a function rather than just a dictionary.
-            This will allow it to work for infinite surfaces.
+            from flatsurf.geometry.categories import ConeSurfaces
 
-        EXAMPLES::
+            return ConeSurfaces.ParentMethods._is_cone_surface(self)
 
-            sage: from flatsurf import *
-            sage: s=translation_surfaces.veech_double_n_gon(5)
-            sage: ss,valid=s.relabel({0:1,1:2})
-            sage: valid
-            True
-            sage: ss.base_label()
-            1
-            sage: ss.opposite_edge(1,0)
-            (2, 0)
-            sage: ss.num_polygons()
-            2
-            sage: TestSuite(ss).run()
-        """
-        if in_place:
-            us = self.underlying_surface()
-            if not us.is_mutable():
-                raise ValueError("Your surface is not mutable, so can not be relabeled in place.")
-            if not isinstance(relabeling_map,dict):
-                raise NotImplementedError("Currently relabeling is only implemented via a dictionary.")
-            domain=set()
-            codomain=set()
-            data={}
-            for l1,l2 in iteritems(relabeling_map):
-                p=us.polygon(l1)
-                glue = []
-                for e in range(p.num_edges()):
-                    ll,ee = us.opposite_edge(l1,e)
-                    try:
-                        lll=relabeling_map[ll]
-                    except KeyError:
-                        lll=ll
-                    glue.append((lll,ee))
-                data[l2]=(p,glue)
-                domain.add(l1)
-                codomain.add(l2)
-            if len(domain)!=len(codomain):
-                raise ValueError("The relabeling_map must be injective. Received "+str(relabeling_map))
-            changed_labels = domain.intersection(codomain)
-            added_labels=codomain.difference(domain)
-            removed_labels=domain.difference(codomain)
-            # Pass to add_polygons
-            relabel_errors={}
-            for l2 in added_labels:
-                p,glue=data[l2]
-                l3 = us.add_polygon(p, label=l2)
-                if not l2==l3:
-                    # This means the label l2 could not be added for some reason.
-                    # Perhaps the implementation does not support this type of label.
-                    # Or perhaps there is already a polygon with this label.
-                    relabel_errors[l2]=l3
-            # Pass to change polygons
-            for l2 in changed_labels:
-                p,glue=data[l2]
-                # This should always work since the domain of the relabeling map should be labels for polygons.
-                us.change_polygon(l2,p)
-            # Deal with the base_label
-            base_label = us.base_label()
-            if base_label in relabeling_map:
-                base_label = relabeling_map[base_label]
-                if base_label in relabel_errors:
-                    base_label = relabel_errors[base_label]
-                us.change_base_label(base_label)
-            # Pass to remove polygons:
-            for l1 in removed_labels:
-                us.remove_polygon(l1)
-            # Pass to update the edge gluings
-            if len(relabel_errors)==0:
-                # No problems. Update the gluings.
-                for l2 in codomain:
-                    p,glue=data[l2]
-                    us.change_polygon_gluings(l2, glue)
-            else:
-                # Use the gluings provided by relabel_errors when necessary
-                for l2 in codomain:
-                    p,glue=data[l2]
-                    for e in range(p.num_edges()):
-                        ll,ee=glue[e]
-                        try:
-                            # First try the error dictionary
-                            us.change_edge_gluing(l2, e, relabel_errors[ll],ee)
-                        except KeyError:
-                            us.change_edge_gluing(l2, e, ll,ee)
-            return self, len(relabel_errors)==0
-        else:
-            return self.copy(mutable=True).relabel(relabeling_map, in_place=True)
+        def is_dilation_surface(self, positive=False):
+            r"""
+            Return whether this surface is a dilation surface, i.e., whether
+            glued edges can be transformed into each other by translation
+            followed by a dilation (multiplication by a diagonal matrix.)
+
+            .. NOTE::
+
+                This method is used to determine whether this surface is in the
+                category of :class:`~.dilation_surfaces.DilationSurfaces` or
+                :class:`~.dilation_surfaces.DilationSurfaces.Positive`.
+                Surfaces can override this method to perform specialized logic,
+                see the note in :mod:`~flatsurf.geometry.categories` for
+                performance considerations.
+
+            INPUT:
+
+            - ``positive`` -- a boolean (default: ``False``); whether the
+              entries of the diagonal matrix must be positive or are allowed to
+              be negative.
+
+            EXAMPLES::
+
+                sage: from flatsurf import Polygon, similarity_surfaces
+                sage: P = Polygon(vertices=[(0,0), (2,0), (1,4), (0,5)])
+                sage: S = similarity_surfaces.self_glued_polygon(P)
+                sage: S.is_dilation_surface()
+                True
+                sage: S.is_dilation_surface(positive=True)
+                False
 
-    def copy(self, relabel=False, mutable=False, lazy=None, new_field=None, optimal_number_field=False):
-        r"""
-        Returns a copy of this surface. The method takes several flags to modify how the copy is taken.
+            """
+            if self.is_translation_surface(positive=positive):
+                return True
 
-        If relabel is True, then instead of returning an exact copy, it returns a copy indexed by the
-        non-negative integers. This uses the Surface_list implementation. If relabel is False (default),
-        then we return an exact copy. The returned surface uses the Surface_dict implementation.
+            from flatsurf.geometry.categories import DilationSurfaces
 
-        The mutability flag returns if the resulting surface should be mutable or not. By default, the
-        resulting surface will not be mutable.
+            return DilationSurfaces.ParentMethods._is_dilation_surface(
+                self, positive=positive
+            )
+
+        def is_translation_surface(self, positive=True):
+            r"""
+            Return whether this surface is a translation surface, i.e., glued
+            edges can be transformed into each other by translations.
+
+            This method must be implemented if this surface is a dilation surface.
+
+            .. NOTE::
+
+                This method is used to determine whether this surface is in the
+                category of
+                :class:`~.half_translation_surfaces.HalfTranslationSurfaces` or
+                :class:`~.translation_surfaces.TranslationSurfaces`. Surfaces
+                can override this method to perform specialized logic, see the
+                note in :mod:`~flatsurf.geometry.categories` for performance
+                considerations.
+
+            INPUT:
+
+            - ``positive`` -- a boolean (default: ``True``); whether the
+              transformation must be a translation or is allowed to be a
+              half-translation, i.e., a translation followed by a reflection in
+              a point (equivalently, a rotation by π.)
+
+            EXAMPLES::
+
+                sage: from flatsurf import Polygon, similarity_surfaces
+                sage: P = Polygon(vertices=[(0,0), (1,0), (1,1), (0,1)])
+                sage: S = similarity_surfaces.self_glued_polygon(P)
+                sage: S.is_translation_surface()
+                False
+                sage: S.is_translation_surface(False)
+                True
+
+            ::
+
+                sage: from flatsurf import translation_surfaces
+                sage: S = translation_surfaces.square_torus()
+                sage: S.is_translation_surface()
+                True
+
+            """
+            from flatsurf.geometry.categories import TranslationSurfaces
+
+            return TranslationSurfaces.ParentMethods._is_translation_surface(
+                self, positive=positive
+            )
+
+        def is_rational_surface(self):
+            r"""
+            Return whether this surface is a rational surface, i.e., the
+            rotational part of all gluings is a rational multiple of π.
+
+            .. NOTE::
+
+                This method is used to determine whether this surface satisfies
+                the :class:`~.SimilaritySurfaces.Rational` axiom. Surfaces can
+                override this method to perform specialized logic, see the note
+                in :mod:`flatsurf.geometry.categories` for performance
+                considerations.
+
+            EXAMPLES::
+
+                sage: from flatsurf import Polygon, similarity_surfaces
+                sage: P = Polygon(vertices=[(0,0), (1,0), (1,1), (0,1)])
+                sage: S = similarity_surfaces.self_glued_polygon(P)
+                sage: S.is_rational_surface()
+                True
 
-        If lazy is True, then the surface is copied by reference. This is the only type of copy
-        possible for infinite surfaces. The parameter defaults to False for finite surfaces, and
-        defaults to True for infinite surfaces.
+            """
+            if self.is_dilation_surface(positive=False):
+                return True
 
-        The new_field parameter can be used to place the vertices in a larger field than the basefield
-        for the original surface.
+            return SimilaritySurfaces.Rational.ParentMethods._is_rational_surface(self)
 
-        The optimal_number_field option can be used to find a best NumberField containing the
-        (necessarily finite) surface.
+        def _mul_(self, matrix, switch_sides=True):
+            r"""
+            EXAMPLES::
+
+                sage: from flatsurf import translation_surfaces
+                sage: s = translation_surfaces.infinite_staircase()
+                sage: s
+                The infinite staircase
+                sage: m=Matrix([[1,2],[0,1]])
+                sage: s2=m*s
+                sage: TestSuite(s2).run()
+                sage: s2.polygon(0)
+                Polygon(vertices=[(0, 0), (1, 0), (3, 1), (2, 1)])
+
+            Testing multiplication by a matrix with negative determinant::
+
+                sage: from flatsurf import dilation_surfaces
+                sage: ds1 = dilation_surfaces.genus_two_square(1/2, 1/3, 1/4, 1/5)
+                sage: ds1.polygon(0)
+                Polygon(vertices=[(0, 0), (1/2, 0), (1, 1/3), (1, 1), (3/4, 1), (0, 4/5)])
+                sage: m = matrix(QQ, [[0, 1], [1, 0]]) # maps (x,y) to (y, x)
+                sage: ds2 = m*ds1
+                sage: ds2.polygon(0)
+                Polygon(vertices=[(0, 0), (4/5, 0), (1, 3/4), (1, 1), (1/3, 1), (0, 1/2)])
+            """
+            if not switch_sides:
+                raise NotImplementedError
+
+            from sage.structure.element import is_Matrix
+
+            if not is_Matrix(matrix):
+                raise NotImplementedError("only implemented for matrices")
+            if not matrix.dimensions != (2, 2):
+                raise NotImplementedError("only implemented for 2x2 matrices")
+
+            from flatsurf.geometry.half_dilation_surface import GL2RImageSurface
+
+            return GL2RImageSurface(self, matrix)
+
+    class Oriented(SurfaceCategoryWithAxiom):
+        r"""
+        The category of oriented surfaces built from Euclidean polygons that
+        are glued by similarities with the orientation compatible with the
+        orientation of the real plane that polygons are defined in.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
-            sage: ss=translation_surfaces.ward(3)
-            sage: print(ss.is_mutable())
-            False
-            sage: s=ss.copy(mutable=True)
-            sage: print(s.is_mutable())
-            True
-            sage: TestSuite(s).run()
-            sage: print(s==ss)
-            True
+            sage: from flatsurf.geometry.categories import SimilaritySurfaces
+            sage: SimilaritySurfaces().Oriented()
+            Category of oriented similarity surfaces
+
+        """
+
+        class ParentMethods:
+            r"""
+            Provides methods available to all oriented surfaces that are built
+            from Euclidean polygons that are glued by similarities.
+
+            If you want to add functionality for such surfaces you most likely
+            want to put it here.
+            """
+
+            @cached_method
+            def edge_matrix(self, p, e=None):
+                r"""
+                Returns the 2x2 matrix representing a similarity which when
+                applied to the polygon with label `p` makes it so the edge `e`
+                can be glued to its opposite edge by translation.
+
+                If `e` is not provided, then `p` should be a pair consisting of
+                a polygon label and an edge.
+
+                EXAMPLES::
+
+                    sage: from flatsurf.geometry.similarity_surface_generators import SimilaritySurfaceGenerators
+                    sage: s = SimilaritySurfaceGenerators.example()
+                    sage: s.polygon(0)
+                    Polygon(vertices=[(0, 0), (2, -2), (2, 0)])
+                    sage: s.polygon(1)
+                    Polygon(vertices=[(0, 0), (2, 0), (1, 3)])
+                    sage: s.opposite_edge(0,0)
+                    (1, 1)
+                    sage: m = s.edge_matrix(0, 0)
+                    sage: m
+                    [   1  1/2]
+                    [-1/2    1]
+                    sage: m * vector((2,-2)) == -vector((-1, 3))
+                    True
+
+                """
+                if e is None:
+                    import warnings
+
+                    warnings.warn(
+                        "passing only a single tuple argument to edge_matrix() has been deprecated and will be deprecated in a future version of sage-flatsurf; pass the label and edge index as separate arguments instead"
+                    )
+                    p, e = p
+
+                u = self.polygon(p).edge(e)
+                pp, ee = self.opposite_edge(p, e)
+                v = self.polygon(pp).edge(ee)
+
+                # note the orientation, it is -v and not v
+                from flatsurf.geometry.similarity import similarity_from_vectors
+                from sage.matrix.matrix_space import MatrixSpace
+
+                return similarity_from_vectors(u, -v, MatrixSpace(self.base_ring(), 2))
+
+            def _an_element_(self):
+                r"""
+                Return a point on this surface.
+
+                EXAMPLES::
+
+                    sage: from flatsurf.geometry.similarity_surface_generators import SimilaritySurfaceGenerators
+                    sage: s = SimilaritySurfaceGenerators.example()
+                    sage: s.an_element()
+                    Point (4/3, -2/3) of polygon 0
+
+                ::
+
+                    sage: from flatsurf import Polygon, MutableOrientedSimilaritySurface
+
+                    sage: S = MutableOrientedSimilaritySurface(QQ)
+                    sage: S.add_polygon(Polygon(vertices=[(0, 0), (1, 0), (1, 1), (0, 1)]))
+                    0
+                    sage: S.glue((0, 0), (0, 2))
+                    sage: S.glue((0, 1), (0, 3))
+
+                    sage: S.an_element()
+                    Point (1/2, 1/2) of polygon 0
+
+                TESTS:
+
+                Verify that this method works over non-fields (if 2 is
+                invertible)::
+
+                  sage: from flatsurf import similarity_surfaces
+                  sage: from flatsurf import EuclideanPolygonsWithAngles
+                  sage: E = EuclideanPolygonsWithAngles((3, 3, 5))
+                  sage: from pyexactreal import ExactReals # optional: exactreal  # random output due to pkg_resources deprecation warnings in some contexts
+                  sage: R = ExactReals(E.base_ring()) # optional: exactreal
+                  sage: angles = (3, 3, 5)
+                  sage: slopes = EuclideanPolygonsWithAngles(*angles).slopes()
+                  sage: P = Polygon(angles=angles, edges=[R.random_element() * slopes[0]])  # optional: exactreal
+                  sage: S = similarity_surfaces.billiard(P) # optional: exactreal
+                  sage: S.an_element()  # optional: exactreal
+                  Point ((1/2 ~ 0.50000000)*ℝ(0.303644…), 0) of polygon 0
+
+                """
+                label = next(iter(self.labels()))
+                polygon = self.polygon(label)
+
+                from sage.categories.all import Fields
+
+                # We use a point that can be constructed without problems on an
+                # infinite surface.
+                if polygon.is_convex() and self.base_ring() in Fields():
+                    coordinates = polygon.centroid()
+                else:
+                    # Sometimes, this is not implemented because it requires the edge
+                    # transformation to be known, so we prefer the centroid.
+                    coordinates = polygon.edge(0) / 2
+                return self(label, coordinates)  # pylint: disable=not-callable
+
+            def underlying_surface(self):
+                r"""
+                Return this surface.
+
+                EXAMPLES::
+
+                    sage: from flatsurf import MutableOrientedSimilaritySurface
+                    sage: S = MutableOrientedSimilaritySurface(QQ)
+                    sage: S.underlying_surface() is S
+                    doctest:warning
+                    ...
+                    UserWarning: underlying_surface() has been deprecated and will be removed in a future version of sage-flatsurf; this function has no effect anymore since there is no distinction between a surface and its underlying surface anymore
+                    True
+
+                """
+                import warnings
+
+                warnings.warn(
+                    "underlying_surface() has been deprecated and will be removed in a future version of sage-flatsurf; this function has no effect anymore since there is no distinction between a surface and its underlying surface anymore"
+                )
 
-            sage: # Changing the base field
-            sage: from flatsurf import *
-            sage: s=translation_surfaces.veech_double_n_gon(5)
-            sage: ss=s.copy(mutable=False,new_field=AA)
-            sage: TestSuite(ss).run()
-            sage: ss.base_ring()
-            Algebraic Real Field
-
-            sage: # Optimization of number field
-            sage: from flatsurf import *
-            sage: s = translation_surfaces.arnoux_yoccoz(3)
-            sage: ss = s.copy(new_field=AA).copy(optimal_number_field=True)
-            sage: TestSuite(ss).run()
-            sage: ss.base_ring().discriminant()
-            -44
-        """
-        s = None  # This will be the surface we copy. (Likely we will set s=self below.)
-        if new_field is not None and optimal_number_field:
-            raise ValueError("You can not set a new_field and also set optimal_number_field=True.")
-        if optimal_number_field == True:
-            assert self.is_finite(), "Can only optimize_number_field for a finite surface."
-            assert not lazy, "Lazy copying is unavailable when optimize_number_field=True."
-            coordinates_AA = []
-            for l,p in self.label_iterator(polygons = True):
-                for e in p.edges():
-                    coordinates_AA.append(AA(e[0]))
-                    coordinates_AA.append(AA(e[1]))
-            from sage.rings.qqbar import number_field_elements_from_algebraics
-            field,coordinates_NF,hom = number_field_elements_from_algebraics(coordinates_AA, minimal = True)
-            if field is QQ:
-                new_field = QQ
-                # We pretend new_field = QQ was passed as a parameter.
-                # It will now get picked up by the "if new_field is not None:" line below.
-            else:
-                # Unfortunately field doesn't come with an real embedding (which is given by hom!)
-                # So, we make a copy of the field, and add the embedding.
-                field2 = NumberField(field.polynomial(), name = "a", embedding = hom(field.gen()))
-                # The following converts from field to field2:
-                hom2 = field.hom(im_gens = [field2.gen()])
-
-                ss = Surface_dict(base_ring = field2)
-                index = 0
-                P = ConvexPolygons(field2)
-                for l,p in self.label_iterator(polygons = True):
-                    new_edges = []
-                    for i in range(p.num_edges()):
-                        new_edges.append( (hom2(coordinates_NF[index]), hom2(coordinates_NF[index+1]) ) )
-                        index += 2
-                    pp = P(edges = new_edges)
-                    ss.add_polygon(pp, label = l)
-                ss.change_base_label(self.base_label())
-                for (l1,e1),(l2,e2) in self.edge_iterator(gluings = True):
-                    ss.change_edge_gluing(l1, e1, l2, e2)
-                s = self.__class__(ss)
-                if not relabel:
-                    if not mutable:
-                        s.set_immutable()
-                    return s
-                # Otherwise we are supposed to relabel. We will make a relabeled copy of s below.
-        if new_field is not None:
-            from flatsurf.geometry.surface import BaseRingChangedSurface
-            s = BaseRingChangedSurface(self,new_field)
-        if s is None:
-            s = self
-        if s.is_finite():
-            if relabel:
-                return self.__class__(Surface_list(surface=s, copy=not lazy, mutable=mutable))
-            else:
-                return self.__class__(Surface_dict(surface=s, copy=not lazy, mutable=mutable))
-        else:
-            if lazy==False:
-                raise ValueError("Only lazy copying available for infinite surfaces.")
-            if self.underlying_surface().is_mutable():
-                raise ValueError("An infinite surface can only be copied if it is immutable.")
-            if relabel:
-                return self.__class__(Surface_list(surface=s, copy=False, mutable=mutable))
-            else:
-                return self.__class__(Surface_dict(surface=s, copy=False, mutable=mutable))
+                return self
 
-    def triangle_flip(self, l1, e1, in_place=False, test=False, direction=None):
-        r"""
-        Flips the diagonal of the quadrilateral formed by two triangles
-        glued together along the provided edge (l1,e1). This can be broken
-        into two steps: join along the edge to form a convex quadilateral,
-        then cut along the other diagonal. Raises a ValueError if this
-        quadrilateral would be non-convex. In this case no changes to the
-        surface are made.
-
-        The direction parameter defaults to (0,1). This is used to decide how
-        the triangles being glued in are labeled. Let p1 be the triangle
-        associated to label l1, and p2 be the triangle associated to l2
-        but moved by a similarity to share the edge (l1,e1). Each triangle
-        has a exactly one separatrix leaving a vertex which travels in the
-        provided direction or its opposite. (For edges we only count as sepatrices
-        traveling counter-clockwise around the triangle.) This holds for p1
-        and p2 and the separatrices must point in opposite directions.
-
-        The above description gives two new triangles t1 and t2 which must be
-        glued in (obtained by flipping the diagonal of the quadrilateral).
-        Up to swapping t1 and t2 we can assume the separatrix in t1 in the
-        provided direction (or its opposite) points in the same direction as
-        that of p1. Further up to cyclic permutation of vertex labels we can
-        assume that the separatrices in p1 and t1 start at the vertex with the
-        same index (an element of {0,1,2}). The same can be done for p2 and t2.
-        We apply the label l1 to t1 and the label l2 to t2. This precisely
-        determines how t1 and t2 should be used to replace p1 and p2.
-
-        INPUT:
-
-        - ``l1`` - label of polygon
-
-        - ``e1`` - (integer) edge of the polygon
-
-        - ``in_place`` (boolean) - If True do the flip to the current surface
-          which must be mutable. In this case the updated surface will be
-          returned.  Otherwise a mutable copy is made and then an edge is
-          flipped, which is then returned.
-
-        - ``test`` (boolean) - If True we don't actually flip, and we return
-          True or False depending on whether or not the flip would be
-          successful.
+            def edge_transformation(self, p, e):
+                r"""
+                Return the similarity bringing the provided edge to the opposite edge.
+
+                EXAMPLES::
+
+                    sage: from flatsurf.geometry.similarity_surface_generators import SimilaritySurfaceGenerators
+                    sage: s = SimilaritySurfaceGenerators.example()
+                    sage: s.polygon(0)
+                    Polygon(vertices=[(0, 0), (2, -2), (2, 0)])
+                    sage: s.polygon(1)
+                    Polygon(vertices=[(0, 0), (2, 0), (1, 3)])
+                    sage: s.opposite_edge(0,0)
+                    (1, 1)
+                    sage: g = s.edge_transformation(0,0)
+                    sage: g((0,0))
+                    (1, 3)
+                    sage: g((2,-2))
+                    (2, 0)
+
+                """
+                from flatsurf.geometry.similarity import SimilarityGroup
+
+                G = SimilarityGroup(self.base_ring())
+                q = self.polygon(p)
+                a = q.vertex(e)
+                b = q.vertex(e + 1)
+                # This is the similarity carrying the origin to a and (1,0) to b:
+                g = G(b[0] - a[0], b[1] - a[1], a[0], a[1])
+
+                pp, ee = self.opposite_edge(p, e)
+                qq = self.polygon(pp)
+                # Be careful here: opposite vertices are identified
+                aa = qq.vertex(ee + 1)
+                bb = qq.vertex(ee)
+                # This is the similarity carrying the origin to aa and (1,0) to bb:
+                gg = G(bb[0] - aa[0], bb[1] - aa[1], aa[0], aa[1])
+
+                # This is the similarity carrying (a,b) to (aa,bb):
+                return gg / g
+
+            def set_vertex_zero(self, label, v, in_place=False):
+                r"""
+                Applies a combinatorial rotation to the polygon with the provided label.
+
+                This makes what is currently vertex v of this polygon vertex 0. In other words,
+                what is currently vertex (or edge) e will now become vertex (e-v)%n where
+                n is the number of sides of the polygon.
+
+                For the updated polygons, the polygons will be translated so that vertex
+                0 is the origin.
+
+                EXAMPLES:
+
+                Example with polygon glued to another polygon::
+
+                    sage: from flatsurf import translation_surfaces
+                    sage: s = translation_surfaces.veech_double_n_gon(4)
+                    sage: s.polygon(0)
+                    Polygon(vertices=[(0, 0), (1, 0), (1, 1), (0, 1)])
+                    sage: [s.opposite_edge(0,i) for i in range(4)]
+                    [(1, 0), (1, 1), (1, 2), (1, 3)]
+                    sage: ss = s.set_vertex_zero(0,1)
+                    sage: ss.polygon(0)
+                    Polygon(vertices=[(0, 0), (0, 1), (-1, 1), (-1, 0)])
+                    sage: [ss.opposite_edge(0,i) for i in range(4)]
+                    [(1, 1), (1, 2), (1, 3), (1, 0)]
+                    sage: TestSuite(ss).run()
+
+                Example with polygon glued to self::
+
+                    sage: s = translation_surfaces.veech_2n_gon(2)
+                    sage: s.polygon(0)
+                    Polygon(vertices=[(0, 0), (1, 0), (1, 1), (0, 1)])
+                    sage: [s.opposite_edge(0,i) for i in range(4)]
+                    [(0, 2), (0, 3), (0, 0), (0, 1)]
+                    sage: ss = s.set_vertex_zero(0,3)
+                    sage: ss.polygon(0)
+                    Polygon(vertices=[(0, 0), (0, -1), (1, -1), (1, 0)])
+                    sage: [ss.opposite_edge(0,i) for i in range(4)]
+                    [(0, 2), (0, 3), (0, 0), (0, 1)]
+                    sage: TestSuite(ss).run()
 
-        - ``direction`` (2-dimensional vector) - Defaults to (0,1). The choice
-          of this vector determines how the newly added triangles are labeled.
+                """
+                if in_place:
+                    raise NotImplementedError(
+                        "this surface does not support set_vertex_zero(mutable=True)"
+                    )
+
+                from flatsurf.geometry.surface import (
+                    MutableOrientedSimilaritySurface,
+                )
+
+                s = MutableOrientedSimilaritySurface.from_surface(self)
+                s.set_vertex_zero(label, v, in_place=True)
+                s.set_immutable()
+                return s
 
-        EXAMPLES::
+            def relabel(self, relabeling_map, in_place=False):
+                r"""
+                Attempt to relabel the polygons according to a relabeling_map, which takes as input
+                a current label and outputs a new label for the same polygon. The method returns a pair
+                (surface,success) where surface is the relabeled surface, and success is a boolean value
+                indicating the success of the operation. The operation will fail if the implementation of the
+                underlying surface does not support labels used in the image of the relabeling map. In this case,
+                other (arbitrary) labels will be used to replace the labels of the surface, and the resulting
+                surface should still be okay.
+
+                Currently, the relabeling_map must be a dictionary.
+
+                If in_place is True then the relabeling is done to the current surface, otherwise a
+                mutable copy is made before relabeling.
+
+                ToDo:
+                  - Allow relabeling_map to be a function rather than just a dictionary.
+                    This will allow it to work for infinite surfaces.
+
+                EXAMPLES::
+
+                    sage: from flatsurf import translation_surfaces
+                    sage: s=translation_surfaces.veech_double_n_gon(5)
+                    sage: ss,valid=s.relabel({0:1, 1:2})
+                    sage: valid
+                    True
+                    sage: ss.root()
+                    1
+                    sage: ss.opposite_edge(1,0)
+                    (2, 0)
+                    sage: len(ss.polygons())
+                    2
+                    sage: TestSuite(ss).run()
 
-            sage: from flatsurf import *
+                """
+                if in_place:
+                    raise NotImplementedError(
+                        "this surface does not implement relabel(in_place=True) yet"
+                    )
+
+                from flatsurf.geometry.surface import (
+                    MutableOrientedSimilaritySurface,
+                )
+
+                s = MutableOrientedSimilaritySurface.from_surface(self)
+                s, valid = s.relabel(relabeling_map=relabeling_map, in_place=True)
+                s.set_immutable()
+                return s, valid
+
+            def copy(
+                self,
+                relabel=False,
+                mutable=False,
+                lazy=None,
+                new_field=None,
+                optimal_number_field=False,
+            ):
+                r"""
+                Returns a copy of this surface. The method takes several flags to modify how the copy is taken.
+
+                If relabel is True, then instead of returning an exact copy, it returns a copy indexed by the
+                non-negative integers. This uses the Surface_list implementation. If relabel is False (default),
+                then we return an exact copy. The returned surface uses the Surface_dict implementation.
+
+                The mutability flag returns if the resulting surface should be mutable or not. By default, the
+                resulting surface will not be mutable.
+
+                If lazy is True, then the surface is copied by reference. This is the only type of copy
+                possible for infinite surfaces. The parameter defaults to False for finite surfaces, and
+                defaults to True for infinite surfaces.
+
+                The new_field parameter can be used to place the vertices in a larger field than the basefield
+                for the original surface.
+
+                The optimal_number_field option can be used to find a best NumberField containing the
+                (necessarily finite) surface.
+
+                EXAMPLES::
+
+                    sage: from flatsurf import translation_surfaces
+                    sage: ss=translation_surfaces.ward(3)
+                    sage: ss.is_mutable()
+                    False
+                    sage: s=ss.copy(mutable=True)
+                    doctest:warning
+                    ...
+                    UserWarning: copy() has been deprecated and will be removed from a future version of sage-flatsurf; for surfaces of finite type use MutableOrientedSimilaritySurface.from_surface() instead.
+                    sage: s.is_mutable()
+                    True
+                    sage: TestSuite(s).run()
+                    sage: s == ss
+                    False
+
+                Changing the base field::
+
+                    sage: s=translation_surfaces.veech_double_n_gon(5)
+                    sage: ss=s.copy(mutable=False,new_field=AA)
+                    doctest:warning
+                    ...
+                    UserWarning: copy() has been deprecated and will be removed from a future version of sage-flatsurf; for surfaces of finite type use MutableOrientedSimilaritySurface.from_surface() instead.
+                    Use set_immutable() to make the resulting surface immutable. Use change_ring() to change the field over which the surface is defined.
+                    sage: TestSuite(ss).run()
+                    sage: ss.base_ring()
+                    Algebraic Real Field
+
+                Optimization of number field::
+
+                    sage: s = translation_surfaces.arnoux_yoccoz(3)
+                    sage: ss = s.copy(new_field=AA).copy(optimal_number_field=True)
+                    doctest:warning
+                    ...
+                    UserWarning: copy() has been deprecated and will be removed from a future version of sage-flatsurf; for surfaces of finite type use MutableOrientedSimilaritySurface.from_surface() instead.
+                    Use set_immutable() to make the resulting surface immutable. Use change_ring() to change the field over which the surface is defined.
+                    doctest:warning
+                    ...
+                    UserWarning: copy() has been deprecated and will be removed from a future version of sage-flatsurf; for surfaces of finite type use MutableOrientedSimilaritySurface.from_surface() instead.
+                    Use set_immutable() to make the resulting surface immutable. There is currently no replacement for optimal number field.
+                    If you are relying on this features, let the authors of sage-flatsurf know and we will try to make it available again.
+                    sage: TestSuite(ss).run()
+                    sage: ss.base_ring().discriminant()
+                    -44
+                """
+                message = "copy() has been deprecated and will be removed from a future version of sage-flatsurf; for surfaces of finite type use MutableOrientedSimilaritySurface.from_surface() instead."
+
+                if not mutable:
+                    message += (
+                        " Use set_immutable() to make the resulting surface immutable."
+                    )
+
+                if relabel:
+                    message += " Use relabel({old: new for (new, old) in enumerate(surface.labels())}) for integer labels."
+
+                if not self.is_finite_type():
+                    message += " However, there is no immediate replacement for lazy copying of infinite surfaces. Have a look at the implementation of flatsurf.geometry.delaunay.LazyMutableSurface and adapt it to your needs."
+
+                if new_field is not None:
+                    message += " Use change_ring() to change the field over which the surface is defined."
+
+                if optimal_number_field:
+                    message += " There is currently no replacement for optimal number field. If you are relying on this features, let the authors of sage-flatsurf know and we will try to make it available again."
+
+                import warnings
+
+                warnings.warn(message)
+
+                category = self.category()
+                s = None  # This will be the surface we copy. (Likely we will set s=self below.)
+                if new_field is not None and optimal_number_field:
+                    raise ValueError(
+                        "You can not set a new_field and also set optimal_number_field=True."
+                    )
+                if optimal_number_field is True:
+                    if not self.is_finite_type():
+                        raise NotImplementedError(
+                            "can only optimize_number_field for a finite surface"
+                        )
+                    if lazy:
+                        raise NotImplementedError(
+                            "lazy copying is unavailable when optimize_number_field=True"
+                        )
+                    coordinates_AA = []
+                    for label, p in zip(self.labels(), self.polygons()):
+                        for e in p.edges():
+                            coordinates_AA.append(AA(e[0]))
+                            coordinates_AA.append(AA(e[1]))
+                    from sage.rings.qqbar import number_field_elements_from_algebraics
+
+                    field, coordinates_NF, hom = number_field_elements_from_algebraics(
+                        coordinates_AA, minimal=True
+                    )
+                    if field is QQ:
+                        new_field = QQ
+                        # We pretend new_field = QQ was passed as a parameter.
+                        # It will now get picked up by the "if new_field is not None:" line below.
+                    else:
+                        # Unfortunately field doesn't come with an real embedding (which is given by hom!)
+                        # So, we make a copy of the field, and add the embedding.
+                        from sage.all import NumberField
+
+                        field2 = NumberField(
+                            field.polynomial(), name="a", embedding=hom(field.gen())
+                        )
+                        # The following converts from field to field2:
+                        hom2 = field.hom(im_gens=[field2.gen()])
+
+                        from flatsurf.geometry.surface import (
+                            MutableOrientedSimilaritySurface,
+                        )
+
+                        ss = MutableOrientedSimilaritySurface(field2)
+                        index = 0
+
+                        from flatsurf import Polygon
+
+                        for label, p in zip(self.labels(), self.polygons()):
+                            new_edges = []
+                            for i in range(len(p.vertices())):
+                                new_edges.append(
+                                    (
+                                        hom2(coordinates_NF[index]),
+                                        hom2(coordinates_NF[index + 1]),
+                                    )
+                                )
+                                index += 2
+                            pp = Polygon(edges=new_edges, base_ring=field2)
+                            ss.add_polygon(pp, label=label)
+                        ss.set_roots(self.roots())
+                        for (l1, e1), (l2, e2) in self.gluings():
+                            ss.glue((l1, e1), (l2, e2))
+                        s = ss
+                        if not relabel:
+                            if not mutable:
+                                s.set_immutable()
+                            return s
+                        # Otherwise we are supposed to relabel. We will make a relabeled copy of s below.
+                if new_field is not None:
+                    s = self.change_ring(new_field)
+                if s is None:
+                    s = self
+                if s.is_finite_type():
+                    if relabel:
+                        from flatsurf.geometry.surface import Surface_list
+
+                        return Surface_list(
+                            surface=s,
+                            copy=not lazy,
+                            mutable=mutable,
+                            category=category,
+                            deprecation_warning=False,
+                        )
+                    else:
+                        from flatsurf.geometry.surface import Surface_dict
 
-            sage: s = similarity_surfaces.right_angle_triangle(ZZ(1),ZZ(1))
-            sage: print(s.polygon(0))
-            Polygon: (0, 0), (1, 0), (0, 1)
-            sage: s.triangle_flip(0, 0, test=True)
-            False
-            sage: s.triangle_flip(0, 1, test=True)
-            True
-            sage: s.triangle_flip(0, 2, test=True)
-            False
+                        return Surface_dict(
+                            surface=s,
+                            copy=not lazy,
+                            mutable=mutable,
+                            category=category,
+                            deprecation_warning=False,
+                        )
+                else:
+                    if lazy is False:
+                        raise ValueError(
+                            "Only lazy copying available for infinite surfaces."
+                        )
+                    if self.is_mutable():
+                        raise ValueError(
+                            "An infinite surface can only be copied if it is immutable."
+                        )
+                    if relabel:
+                        from flatsurf.geometry.surface import Surface_list
+
+                        return Surface_list(
+                            surface=s,
+                            copy=False,
+                            mutable=mutable,
+                            category=category,
+                            deprecation_warning=False,
+                        )
+                    else:
+                        from flatsurf.geometry.surface import Surface_dict
 
-            sage: s = similarity_surfaces.right_angle_triangle(ZZ(1),ZZ(1))
-            sage: from flatsurf.geometry.surface import Surface_list
-            sage: s = s.__class__(Surface_list(surface=s, mutable=True))
-            sage: try:
-            ....:     s.triangle_flip(0,0,in_place=True)
-            ....: except ValueError as e:
-            ....:     print(e)
-            Gluing triangles along this edge yields a non-convex quadrilateral.
-            sage: s.triangle_flip(0,1,in_place=True)
-            ConeSurface built from 2 polygons
-            sage: s.polygon(0)
-            Polygon: (0, 0), (1, 1), (0, 1)
-            sage: s.polygon(1)
-            Polygon: (0, 0), (-1, -1), (0, -1)
-            sage: for p in s.edge_iterator(gluings=True):
-            ....:     print(p)
-            ((0, 0), (1, 0))
-            ((0, 1), (0, 2))
-            ((0, 2), (0, 1))
-            ((1, 0), (0, 0))
-            ((1, 1), (1, 2))
-            ((1, 2), (1, 1))
-            sage: try:
-            ....:     s.triangle_flip(0,2,in_place=True)
-            ....: except ValueError as e:
-            ....:     print(e)
-            ....:
-            Gluing triangles along this edge yields a non-convex quadrilateral.
-
-            sage: p = polygons((2,0),(-1,3),(-1,-3))
-            sage: s = similarity_surfaces.self_glued_polygon(p)
-            sage: from flatsurf.geometry.surface import Surface_list
-            sage: s = s.__class__(Surface_list(surface=s,mutable=True))
-            sage: s.triangle_flip(0,1,in_place=True)
-            HalfTranslationSurface built from 1 polygon
-            sage: for x in s.label_iterator(polygons=True):
-            ....:     print(x)
-            (0, Polygon: (0, 0), (-3, -3), (-1, -3))
-            sage: for x in s.edge_iterator(gluings=True):
-            ....:     print(x)
-            ((0, 0), (0, 0))
-            ((0, 1), (0, 1))
-            ((0, 2), (0, 2))
-            sage: TestSuite(s).run()
-        """
-        if test:
-            # Just test if the flip would be successful
-            p1=self.polygon(l1)
-            if not p1.num_edges()==3:
-                return False
-            l2,e2 = self.opposite_edge(l1,e1)
-            p2 = self.polygon(l2)
-            if not p2.num_edges()==3:
-                return False
-            sim = self.edge_transformation(l2,e2)
-            hol = sim( p2.vertex( (e2+2)%3 ) - p1.vertex((e1+2)%3) )
-            from flatsurf.geometry.polygon import wedge_product
-            return wedge_product(p1.edge((e1+2)%3), hol) > 0 and \
-                wedge_product(p1.edge((e1+1)%3), hol) > 0
-
-        if in_place:
-            s=self
-            assert s.is_mutable(), "Surface must be mutable for in place triangle_flip."
-        else:
-            s=self.copy(mutable=True)
-
-        p1=s.polygon(l1)
-        if not p1.num_edges()==3:
-            raise ValueError("The polygon with the provided label is not a triangle.")
-        l2,e2 = s.opposite_edge(l1,e1)
-
-        sim = s.edge_transformation(l2,e2)
-        m = sim.derivative()
-        p2=s.polygon(l2)
-        if not p2.num_edges()==3:
-            raise ValueError("The polygon opposite the provided edge is not a triangle.")
-        P=p1.parent()
-        p2=P(vertices=[sim(v) for v in p2.vertices()])
-
-        if direction is None:
-            direction=s.vector_space()((0,1))
-        # Get vertices corresponding to separatices in the provided direction.
-        v1=p1.find_separatrix(direction=direction)[0]
-        v2=p2.find_separatrix(direction=direction)[0]
-        # Our quadrilateral has vertices labeled:
-        # * 0=p1.vertex(e1+1)=p2.vertex(e2)
-        # * 1=p1.vertex(e1+2)
-        # * 2=p1.vertex(e1)=p2.vertex(e2+1)
-        # * 3=p2.vertex(e2+2)
-        # Record the corresponding vertices of this quadrilateral.
-        q1 = (3+v1-e1-1)%3
-        q2 = (2+(3+v2-e2-1)%3)%4
-
-        new_diagonal=p2.vertex((e2+2)%3)-p1.vertex((e1+2)%3)
-        # This list will store the new triangles which are being glued in.
-        # (Unfortunately, they may not be cyclically labeled in the correct way.)
-        new_triangle=[]
-        try:
-            new_triangle.append(P(edges=[p1.edge((e1+2)%3),p2.edge((e2+1)%3),-new_diagonal]))
-            new_triangle.append(P(edges=[p2.edge((e2+2)%3),p1.edge((e1+1)%3),new_diagonal]))
-            # The above triangles would be glued along edge 2 to form the diagonal of the quadrilateral being removed.
-        except ValueError:
-            raise ValueError("Gluing triangles along this edge yields a non-convex quadrilateral.")
-
-        # Find the separatrices of the two new triangles, and in particular which way they point.
-        new_sep=[]
-        new_sep.append(new_triangle[0].find_separatrix(direction=direction)[0])
-        new_sep.append(new_triangle[1].find_separatrix(direction=direction)[0])
-        # The quadrilateral vertices corresponding to these separatrices are
-        # new_sep[0]+1 and (new_sep[1]+3)%4 respectively.
-
-        # i=0 if the new_triangle[0] should be labeled l1 and new_triangle[1] should be labeled l2.
-        # i=1 indicates the opposite labeling.
-        if new_sep[0]+1==q1:
-            # For debugging:
-            assert (new_sep[1]+3)%4==q2, \
-                "Bug: new_sep[1]="+str(new_sep[1])+" and q2="+str(q2)
-            i=0
-        else:
-            # For debugging:
-            assert (new_sep[1]+3)%4==q1
-            assert new_sep[0]+1==q2
-            i=1
-
-        # These quantities represent the cyclic relabeling of triangles needed.
-        cycle1 = (new_sep[i]-v1+3)%3
-        cycle2 = (new_sep[1-i]-v2+3)%3
-
-        # This will be the new triangle with label l1:
-        tri1=P(edges=[new_triangle[i].edge(cycle1), \
-                      new_triangle[i].edge((cycle1+1)%3), \
-                      new_triangle[i].edge((cycle1+2)%3)])
-        # This will be the new triangle with label l2:
-        tri2=P(edges=[new_triangle[1-i].edge(cycle2), \
-                      new_triangle[1-i].edge((cycle2+1)%3), \
-                      new_triangle[1-i].edge((cycle2+2)%3)])
-        # In the above, edge 2-cycle1 of tri1 would be glued to edge 2-cycle2 of tri2
-        diagonal_glue_e1=2-cycle1
-        diagonal_glue_e2=2-cycle2
-
-        # FOR CATCHING BUGS:
-        assert p1.find_separatrix(direction=direction)==tri1.find_separatrix(direction=direction)
-        assert p2.find_separatrix(direction=direction)==tri2.find_separatrix(direction=direction)
-
-        # Two opposite edges will not change their labels (label,edge) under our regluing operation.
-        # The other two opposite ones will change and in fact they change labels.
-        # The following finds them (there are two cases).
-        # At the end of the if statement, the following will be true:
-        # * new_glue_e1 and new_glue_e2 will be the edges of the new triangle with label l1 and l2 which need regluing.
-        # * old_e1 and old_e2 will be the corresponding edges of the old triangles.
-        # (Note that labels are swapped between the pair. The appending 1 or 2 refers to the label used for the triangle.)
-        if p1.edge(v1)==tri1.edge(v1):
-            # We don't have to worry about changing gluings on edge v1 of the triangles with label l1
-            # We do have to worry about the following edge:
-            new_glue_e1=3-diagonal_glue_e1-v1 # returns the edge which is neither diagonal_glue_e1 nor v1.
-            # This corresponded to the following old edge:
-            old_e1 = 3 - e1 - v1 # Again this finds the edge which is neither e1 nor v1
-        else:
-            temp = (v1+2)%3
-            # FOR CATCHING BUGS:
-            assert p1.edge(temp)==tri1.edge(temp)
-            # We don't have to worry about changing gluings on edge (v1+2)%3 of the triangles with label l1
-            # We do have to worry about the following edge:
-            new_glue_e1=3-diagonal_glue_e1-temp # returns the edge which is neither diagonal_glue_e1 nor temp.
-            # This corresponded to the following old edge:
-            old_e1 = 3 - e1 - temp # Again this finds the edge which is neither e1 nor temp
-        if p2.edge(v2)==tri2.edge(v2):
-            # We don't have to worry about changing gluings on edge v2 of the triangles with label l2
-            # We do have to worry about the following edge:
-            new_glue_e2=3-diagonal_glue_e2-v2 # returns the edge which is neither diagonal_glue_e2 nor v2.
-            # This corresponded to the following old edge:
-            old_e2 = 3 - e2 - v2 # Again this finds the edge which is neither e2 nor v2
-        else:
-            temp = (v2+2)%3
-            # FOR CATCHING BUGS:
-            assert p2.edge(temp)==tri2.edge(temp)
-            # We don't have to worry about changing gluings on edge (v2+2)%3 of the triangles with label l2
-            # We do have to worry about the following edge:
-            new_glue_e2=3-diagonal_glue_e2-temp # returns the edge which is neither diagonal_glue_e2 nor temp.
-            # This corresponded to the following old edge:
-            old_e2 = 3 - e2 - temp # Again this finds the edge which is neither e2 nor temp
-
-        # remember the old gluings.
-        old_opposite1 = s.opposite_edge(l1, old_e1)
-        old_opposite2 = s.opposite_edge(l2, old_e2)
-
-        # We make changes to the underlying surface
-        us=s.underlying_surface()
-
-        # Replace the triangles.
-        us.change_polygon(l1,tri1)
-        us.change_polygon(l2,tri2)
-        # Glue along the new diagonal of the quadrilateral
-        us.change_edge_gluing(l1,diagonal_glue_e1,
-                             l2,diagonal_glue_e2)
-        # Now we deal with that pair of opposite edges of the quadrilateral that need regluing.
-        # There are some special cases:
-        if old_opposite1==(l2,old_e2):
-            # These opposite edges were glued to each other.
-            # Do the same in the new surface:
-            us.change_edge_gluing(l1,new_glue_e1,
-                                 l2,new_glue_e2)
-        else:
-            if old_opposite1==(l1,old_e1):
-                # That edge was "self-glued".
-                us.change_edge_gluing(l2,new_glue_e2,
-                                     l2,new_glue_e2)
-            else:
-                # The edge (l1,old_e1) was glued in a standard way.
-                # That edge now corresponds to (l2,new_glue_e2):
-                us.change_edge_gluing(l2,new_glue_e2,
-                                     old_opposite1[0],old_opposite1[1])
-            if old_opposite2==(l2,old_e2):
-                # That edge was "self-glued".
-                us.change_edge_gluing(l1,new_glue_e1,
-                                     l1,new_glue_e1)
-            else:
-                # The edge (l2,old_e2) was glued in a standard way.
-                # That edge now corresponds to (l1,new_glue_e1):
-                us.change_edge_gluing(l1,new_glue_e1,
-                                     old_opposite2[0],old_opposite2[1])
-        return s
+                        return Surface_dict(
+                            surface=s,
+                            copy=False,
+                            mutable=mutable,
+                            category=category,
+                            deprecation_warning=False,
+                        )
+
+            def change_ring(self, ring):
+                r"""
+                Return a copy of this surface whose polygons are defined over
+                ``ring``.
+
+                EXAMPLES::
+
+                    sage: from flatsurf import translation_surfaces
+                    sage: S = translation_surfaces.veech_2n_gon(4)
+                    sage: T = S.change_ring(AA)
+                    sage: T.base_ring()
+                    Algebraic Real Field
+
+                """
+                from flatsurf.geometry.surface import BaseRingChangedSurface
+
+                return BaseRingChangedSurface(self, ring)
+
+            def triangle_flip(self, l1, e1, in_place=False, test=False, direction=None):
+                r"""
+                Flips the diagonal of the quadrilateral formed by two triangles
+                glued together along the provided edge (l1,e1). This can be broken
+                into two steps: join along the edge to form a convex quadilateral,
+                then cut along the other diagonal. Raises a ValueError if this
+                quadrilateral would be non-convex. In this case no changes to the
+                surface are made.
+
+                The direction parameter defaults to (0,1). This is used to decide how
+                the triangles being glued in are labeled. Let p1 be the triangle
+                associated to label l1, and p2 be the triangle associated to l2
+                but moved by a similarity to share the edge (l1,e1). Each triangle
+                has a exactly one separatrix leaving a vertex which travels in the
+                provided direction or its opposite. (For edges we only count as sepatrices
+                traveling counter-clockwise around the triangle.) This holds for p1
+                and p2 and the separatrices must point in opposite directions.
+
+                The above description gives two new triangles t1 and t2 which must be
+                glued in (obtained by flipping the diagonal of the quadrilateral).
+                Up to swapping t1 and t2 we can assume the separatrix in t1 in the
+                provided direction (or its opposite) points in the same direction as
+                that of p1. Further up to cyclic permutation of vertex labels we can
+                assume that the separatrices in p1 and t1 start at the vertex with the
+                same index (an element of {0,1,2}). The same can be done for p2 and t2.
+                We apply the label l1 to t1 and the label l2 to t2. This precisely
+                determines how t1 and t2 should be used to replace p1 and p2.
+
+                INPUT:
+
+                - ``l1`` - label of polygon
+
+                - ``e1`` - (integer) edge of the polygon
+
+                - ``in_place`` (boolean) - If True do the flip to the current surface
+                  which must be mutable. In this case the updated surface will be
+                  returned.  Otherwise a mutable copy is made and then an edge is
+                  flipped, which is then returned.
+
+                - ``test`` (boolean) - If True we don't actually flip, and we return
+                  True or False depending on whether or not the flip would be
+                  successful.
+
+                - ``direction`` (2-dimensional vector) - Defaults to (0,1). The choice
+                  of this vector determines how the newly added triangles are labeled.
+
+                EXAMPLES::
+
+                    sage: from flatsurf import similarity_surfaces, MutableOrientedSimilaritySurface, Polygon
+
+                    sage: s = similarity_surfaces.right_angle_triangle(ZZ(1),ZZ(1))
+                    sage: s.polygon(0)
+                    Polygon(vertices=[(0, 0), (1, 0), (0, 1)])
+                    sage: s.triangle_flip(0, 0, test=True)
+                    False
+                    sage: s.triangle_flip(0, 1, test=True)
+                    True
+                    sage: s.triangle_flip(0, 2, test=True)
+                    False
+
+                    sage: s = similarity_surfaces.right_angle_triangle(ZZ(1),ZZ(1))
+                    sage: s = MutableOrientedSimilaritySurface.from_surface(s)
+                    sage: s.triangle_flip(0, 0, in_place=True)
+                    Traceback (most recent call last):
+                    ...
+                    ValueError: Gluing triangles along this edge yields a non-convex quadrilateral.
+                    sage: s.triangle_flip(0,1,in_place=True)
+                    Rational Cone Surface built from 2 isosceles triangles
+                    sage: s.polygon(0)
+                    Polygon(vertices=[(0, 0), (1, 1), (0, 1)])
+                    sage: s.polygon(1)
+                    Polygon(vertices=[(0, 0), (-1, -1), (0, -1)])
+                    sage: s.gluings()
+                    (((0, 0), (1, 0)), ((0, 1), (0, 2)), ((0, 2), (0, 1)), ((1, 0), (0, 0)), ((1, 1), (1, 2)), ((1, 2), (1, 1)))
+                    sage: s.triangle_flip(0,2,in_place=True)
+                    Traceback (most recent call last):
+                    ...
+                    ValueError: Gluing triangles along this edge yields a non-convex quadrilateral.
+
+                    sage: p = Polygon(edges=[(2,0),(-1,3),(-1,-3)])
+                    sage: s = similarity_surfaces.self_glued_polygon(p)
+                    sage: s = MutableOrientedSimilaritySurface.from_surface(s)
+                    sage: s.triangle_flip(0,1,in_place=True)
+                    Half-Translation Surface built from a triangle
+
+                    sage: s.set_immutable()
+
+                    sage: from flatsurf.geometry.categories import DilationSurfaces
+                    sage: s in DilationSurfaces()
+                    True
+                    sage: s.labels()
+                    (0,)
+                    sage: s.polygons()
+                    (Polygon(vertices=[(0, 0), (-3, -3), (-1, -3)]),)
+                    sage: s.gluings()
+                    (((0, 0), (0, 0)), ((0, 1), (0, 1)), ((0, 2), (0, 2)))
+                    sage: TestSuite(s).run()
+
+                """
+                if test:
+                    # Just test if the flip would be successful
+                    p1 = self.polygon(l1)
+                    if not len(p1.vertices()) == 3:
+                        return False
+                    l2, e2 = self.opposite_edge(l1, e1)
+                    p2 = self.polygon(l2)
+                    if not len(p2.vertices()) == 3:
+                        return False
+                    sim = self.edge_transformation(l2, e2)
+                    hol = sim(p2.vertex((e2 + 2) % 3) - p1.vertex((e1 + 2) % 3))
+                    from flatsurf.geometry.euclidean import ccw
+
+                    return (
+                        ccw(p1.edge((e1 + 2) % 3), hol) > 0
+                        and ccw(p1.edge((e1 + 1) % 3), hol) > 0
+                    )
 
-    def join_polygons(self, p1, e1, test=False, in_place=False):
-        r"""
-        Join polygons across the provided edge (p1,e1). By default,
-        it returns the surface obtained by joining the two polygons
-        together. It raises a ValueError if gluing the two polygons
-        together results in a non-convex polygon. This is done to the
-        current surface if in_place is True, and otherwise a mutable
-        copy is made and then modified.
-
-        If test is True then instead of changing the surface, it just
-        checks to see if the change would be successful and returns
-        True if successful or False if not.
+                if in_place:
+                    raise NotImplementedError(
+                        "this surface does not support triangle_flip(in_place=True) yet"
+                    )
+
+                from flatsurf.geometry.surface import (
+                    MutableOrientedSimilaritySurface,
+                )
+
+                s = MutableOrientedSimilaritySurface.from_surface(self)
+                s.triangle_flip(
+                    l1=l1, e1=e1, in_place=True, test=test, direction=direction
+                )
+                s.set_immutable()
+                return s
 
-        EXAMPLES::
+            def join_polygons(self, p1, e1, test=False, in_place=False):
+                r"""
+                Join polygons across the provided edge (p1,e1). By default,
+                it returns the surface obtained by joining the two polygons
+                together. It raises a ValueError if gluing the two polygons
+                together results in a non-convex polygon. This is done to the
+                current surface if in_place is True, and otherwise a mutable
+                copy is made and then modified.
+
+                If test is True then instead of changing the surface, it just
+                checks to see if the change would be successful and returns
+                True if successful or False if not.
+
+                EXAMPLES::
+
+                    sage: from flatsurf import translation_surfaces, MutableOrientedSimilaritySurface
+                    sage: ss = translation_surfaces.ward(3)
+                    sage: s = MutableOrientedSimilaritySurface.from_surface(ss)
+                    sage: s.join_polygons(0,0, in_place=True)
+                    Translation Surface built from an equilateral triangle and a pentagon with 2 marked vertices
+                    sage: s.polygon(0)
+                    Polygon(vertices=[(0, 0), (1, -a), (2, 0), (3, a), (2, 2*a), (0, 2*a), (-1, a)])
+                    sage: s.join_polygons(0,4, in_place=True)
+                    Translation Surface built from a rhombus
+                    sage: s.polygon(0)
+                    Polygon(vertices=[(0, 0), (1, -a), (2, 0), (3, a), (2, 2*a), (1, 3*a), (0, 2*a), (-1, a)])
+
+                TESTS::
+
+                    sage: from flatsurf.geometry.categories import TranslationSurfaces
+                    sage: s.set_immutable()
+                    sage: s in TranslationSurfaces()
+                    True
+
+                """
+                if test:
+                    in_place = False
 
-            sage: from flatsurf import *
-            sage: ss=translation_surfaces.ward(3)
-            sage: s=ss.copy(mutable=True)
-            sage: s.join_polygons(0,0, in_place=True)
-            TranslationSurface built from 2 polygons
-            sage: print(s.polygon(0))
-            Polygon: (0, 0), (1, -a), (2, 0), (3, a), (2, 2*a), (0, 2*a), (-1, a)
-            sage: s.join_polygons(0,4, in_place=True)
-            TranslationSurface built from 1 polygon
-            sage: print(s.polygon(0))
-            Polygon: (0, 0), (1, -a), (2, 0), (3, a), (2, 2*a), (1, 3*a), (0, 2*a), (-1, a)
-        """
-        poly1=self.polygon(p1)
-        p2,e2 = self.opposite_edge(p1,e1)
-        poly2=self.polygon(p2)
-        if p1==p2:
-            if test:
-                return False
-            else:
-                raise ValueError("Can't glue polygon to itself.")
-        t=self.edge_transformation(p2, e2)
-        dt=t.derivative()
-        vs = []
-        edge_map={} # Store the pairs for the old edges.
-        for i in range(e1):
-            edge_map[len(vs)]=(p1,i)
-            vs.append(poly1.edge(i))
-        ne=poly2.num_edges()
-        for i in range(1,ne):
-            ee=(e2+i)%ne
-            edge_map[len(vs)]=(p2,ee)
-            vs.append(dt * poly2.edge( ee ))
-        for i in range(e1+1, poly1.num_edges()):
-            edge_map[len(vs)]=(p1,i)
-            vs.append(poly1.edge(i))
-
-        try:
-            new_polygon = ConvexPolygons(self.base_ring())(vs)
-        except (ValueError, TypeError):
-            if test:
-                return False
-            else:
-                raise ValueError("Joining polygons along this edge results in a non-convex polygon.")
-
-        if test:
-            # Gluing would be successful
-            return True
-
-        # Now no longer testing. Do the gluing.
-        if in_place:
-            ss=self
-        else:
-            ss=self.copy(mutable=True)
-        s=ss.underlying_surface()
-
-        inv_edge_map={}
-        for key, value in iteritems(edge_map):
-            inv_edge_map[value]=(p1,key)
-
-        glue_list=[]
-        for i in range(len(vs)):
-            p3,e3 = edge_map[i]
-            p4,e4 = self.opposite_edge(p3,e3)
-            if p4 == p1 or p4 == p2:
-                glue_list.append(inv_edge_map[(p4,e4)])
-            else:
-                glue_list.append((p4,e4))
-
-        if s.base_label()==p2:
-             s.change_base_label(p1)
+                if in_place:
+                    raise NotImplementedError(
+                        "this surface does not implement join_polygons(in_place=True) yet"
+                    )
+
+                if not test:
+                    from flatsurf.geometry.surface import (
+                        MutableOrientedSimilaritySurface,
+                    )
+
+                    s = MutableOrientedSimilaritySurface.from_surface(self)
+                    s.join_polygons(p1=p1, e1=e1, test=False, in_place=True)
+                    s.set_immutable()
+                    return s
 
-        s.remove_polygon(p2)
+                poly1 = self.polygon(p1)
+                p2, e2 = self.opposite_edge(p1, e1)
+                poly2 = self.polygon(p2)
 
-        s.change_polygon(p1, new_polygon, glue_list)
+                if p1 == p2:
+                    return False
 
-        return ss
+                t = self.edge_transformation(p2, e2)
+                dt = t.derivative()
+                es = []
+                for i in range(e1):
+                    es.append(poly1.edge(i))
+                ne = len(poly2.vertices())
+                for i in range(1, ne):
+                    ee = (e2 + i) % ne
+                    es.append(dt * poly2.edge(ee))
+                for i in range(e1 + 1, len(poly1.vertices())):
+                    es.append(poly1.edge(i))
 
-    def subdivide_polygon(self, p, v1, v2, test=False, new_label=None):
-        r"""
-        Cut the polygon with label p along the diagonal joining vertex
-        v1 to vertex v2. This cuts p into two polygons, one will keep the same
-        label. The other will get a new label, which can be provided
-        via new_label. Otherwise a default new label will be provided.
-        If test=False, then the surface will be changed (in place). If
-        test=True, then it just checks to see if the change would be successful
-
-        The convention is that the resulting subdivided polygon which has an oriented
-        edge going from the original vertex v1 to vertex v2 will keep the label p.
-        The other polygon will get a new label.
+                try:
+                    from flatsurf import Polygon
 
-        The change will be done in place.
-        """
-        poly=self.polygon(p)
-        ne=poly.num_edges()
-        if v1<0 or v2<0 or v1>=ne or v2>=ne:
-            if test:
-                return False
-            else:
-                raise ValueError('Provided vertices out of bounds.')
-        if abs(v1-v2)<=1 or abs(v1-v2)>=ne-1:
-            if test:
-                return False
-            else:
-                raise ValueError('Provided diagonal is not actually a diagonal.')
-
-        if v2<v1:
-            v2=v2+ne
-
-        newedges1=[poly.vertex(v2)-poly.vertex(v1)]
-        for i in range(v2, v1+ne):
-            newedges1.append(poly.edge(i))
-        newpoly1 = ConvexPolygons(self.base_ring())(newedges1)
-
-        newedges2=[poly.vertex(v1)-poly.vertex(v2)]
-        for i in range(v1,v2):
-            newedges2.append(poly.edge(i))
-        newpoly2 = ConvexPolygons(self.base_ring())(newedges2)
-
-        # Store the old gluings
-        old_gluings = {(p,i): self.opposite_edge(p,i) for i in range(ne)}
-
-        # Update the polygon with label p, add a new polygon.
-        self.underlying_surface().change_polygon(p, newpoly1)
-        if new_label is None:
-            new_label = self.underlying_surface().add_polygon(newpoly2)
-        else:
-            new_label = self.underlying_surface().add_polygon(newpoly2, label=new_label)
-        # This gluing is the diagonal we used.
-        self.underlying_surface().change_edge_gluing(p, 0, new_label, 0)
-
-        # Setup conversion from old to new labels.
-        old_to_new_labels={}
-        for i in range(v1, v2):
-            old_to_new_labels[(p,i%ne)]=(new_label,i-v1+1)
-        for i in range(v2, ne+v1):
-            old_to_new_labels[(p,i%ne)]=(p,i-v2+1)
-
-        for e in range(1, newpoly1.num_edges()):
-            pair = old_gluings[(p,(v2+e-1)%ne)]
-            if pair in old_to_new_labels:
-                pair = old_to_new_labels[pair]
-            self.underlying_surface().change_edge_gluing(p, e, pair[0], pair[1])
-
-        for e in range(1, newpoly2.num_edges()):
-            pair = old_gluings[(p,(v1+e-1)%ne)]
-            if pair in old_to_new_labels:
-                pair = old_to_new_labels[pair]
-            self.underlying_surface().change_edge_gluing(new_label, e, pair[0], pair[1])
+                    Polygon(edges=es, base_ring=self.base_ring())
+                except (ValueError, TypeError):
+                    return False
 
-    def singularity(self, l, v, limit=None):
-        r"""
-        Represents the Singularity associated to the v-th vertex of the polygon with
-        label l.
+                # Gluing would be successful
+                return True
 
-        If the surface is infinite, the limit needs to be set. In this case the construction
-        of the singularity is successful if the sequence of vertices hit by passing through
-        edges closes up in limit or less steps.
+            def subdivide_polygon(self, p, v1, v2, test=False, new_label=None):
+                r"""
+                Cut the polygon with label p along the diagonal joining vertex
+                v1 to vertex v2. This cuts p into two polygons, one will keep the same
+                label. The other will get a new label, which can be provided
+                via new_label. Otherwise a default new label will be provided.
+                If test=False, then the surface will be changed (in place). If
+                test=True, then it just checks to see if the change would be successful
+
+                The convention is that the resulting subdivided polygon which has an oriented
+                edge going from the original vertex v1 to vertex v2 will keep the label p.
+                The other polygon will get a new label.
+
+                The change will be done in place.
+                """
+                if not test:
+                    raise NotImplementedError(
+                        "this surface does not implement subdivide_polygon(test=False) yet"
+                    )
+
+                poly = self.polygon(p)
+                ne = len(poly.vertices())
+                if v1 < 0 or v2 < 0 or v1 >= ne or v2 >= ne:
+                    return False
+                if abs(v1 - v2) <= 1 or abs(v1 - v2) >= ne - 1:
+                    return False
 
-        EXAMPLES::
+                return True
 
-            sage: from flatsurf import *
-            sage: s = translation_surfaces.square_torus()
-            sage: pc = s.minimal_cover(cover_type="planar")
-            sage: pc.singularity(pc.base_label(),0)
-            Traceback (most recent call last):
-            ...
-            ValueError: need a limit when working with an infinite surface
-            sage: pc.singularity(pc.base_label(),0,limit=4)
-            singularity with vertex equivalence class frozenset(...)
-        """
-        return Singularity(self,l,v,limit)
+            def singularity(self, label, v, limit=None):
+                r"""
+                Represents the Singularity associated to the v-th vertex of the polygon
+                with label ``label``.
+
+                If the surface is infinite, the limit can be set. In this case the
+                construction of the singularity is successful if the sequence of
+                vertices hit by passing through edges closes up in limit or less steps.
+
+                EXAMPLES::
+
+                    sage: from flatsurf import translation_surfaces
+                    sage: s = translation_surfaces.square_torus()
+                    sage: pc = s.minimal_cover(cover_type="planar")
+                    sage: pc.singularity(pc.root(), 0)
+                    doctest:warning
+                    ...
+                    UserWarning: Singularity() is deprecated and will be removed in a future version of sage-flatsurf. Use surface.point() instead.
+                    Vertex 0 of polygon (0, (x, y) |-> (x, y))
+                    sage: pc.singularity(pc.root(), 0, limit=1)
+                    Traceback (most recent call last):
+                    ...
+                    ValueError: number of edges at singularity exceeds limit
+
+                """
+                from flatsurf.geometry.surface_objects import Singularity
+
+                return Singularity(self, label, v, limit)
+
+            def point(self, label, point, ring=None, limit=None):
+                r"""
+                Return a point in this surface.
+
+                INPUT:
+
+                - ``label`` - label of the polygon
+
+                - ``point`` - coordinates of the point inside the polygon or
+                  the index of the vertex of the polygon.
+
+                - ``ring`` (optional) - a ring for the coordinates
+
+                - ``limit`` (optional) - undocumented (only relevant if the point
+                  corresponds to a singularity in an infinite surface)
+
+                EXAMPLES::
+
+                    sage: from flatsurf import translation_surfaces
+                    sage: s = translation_surfaces.square_torus()
+                    sage: pc = s.minimal_cover(cover_type="planar")
+                    sage: pc.point(pc.root(), (0, 0))
+                    Vertex 0 of polygon (0, (x, y) |-> (x, y))
+                    sage: pc.point(pc.root(), 0)
+                    Vertex 0 of polygon (0, (x, y) |-> (x, y))
+                    sage: pc.point(pc.root(), 1)
+                    Vertex 0 of polygon (0, (x, y) |-> (x + 1, y))
+                    sage: pc.point(pc.root(), (1, 1))
+                    Vertex 0 of polygon (0, (x, y) |-> (x + 1, y + 1))
+                    sage: z = pc.point(pc.root(),(sqrt(2)-1,sqrt(3)-1),ring=AA)
+                    doctest:warning
+                    ...
+                    UserWarning: the ring parameter is deprecated and will be removed in a future version of sage-flatsurf; define the surface over a larger ring instead so that this points' coordinates live in the base ring
+                    sage: next(iter(z.coordinates(next(iter(z.labels()))))).parent()
+                    Vector space of dimension 2 over Algebraic Real Field
+
+                ::
+
+                    sage: s = translation_surfaces.cathedral(2, 3)
+                    sage: s.point(0, 0)
+                    Vertex 0 of polygon 0
+                    sage: s.point(0, (0, 0))
+                    Vertex 0 of polygon 0
+                    sage: s.point(0, (1, 1))
+                    Point (1, 0) of polygon 0
+                    sage: s.point(0, 1)
+                    Vertex 0 of polygon 1
+
+                """
+                # pylint: disable-next=not-callable
+                return self(label, point, limit=limit, ring=ring)
+
+            def surface_point(self, *args, **kwargs):
+                r"""
+                Return a point in this surface.
+
+                This is an alias for :meth:`point`.
+                """
+                import warnings
+
+                warnings.warn(
+                    "surface_point() has been deprecated and will be removed in a future version of sage-flatsurf; use point() instead"
+                )
+
+                return self.point(*args, **kwargs)
+
+            def minimal_cover(self, cover_type="translation"):
+                r"""
+                Return the minimal translation or half-translation cover of the surface.
+
+                Cover type may be either "translation", "half-translation" or "planar".
+
+                The minimal planar cover of a surface S is the smallest cover C so that
+                the developing map from the universal cover U to the plane induces a
+                well defined map from C to the plane. This is an infinite translation
+                surface that is naturally a branched cover of the plane.
+
+                EXAMPLES::
+
+                    sage: from flatsurf import polygons, MutableOrientedSimilaritySurface
+                    sage: s = MutableOrientedSimilaritySurface(QQ)
+                    sage: square = polygons.square(base_ring=QQ)
+                    sage: s.add_polygon(square)
+                    0
+                    sage: s.glue((0,0), (0,1))
+                    sage: s.glue((0,2) ,(0,3))
+                    sage: cs = s
+                    sage: ts = cs.minimal_cover(cover_type="translation")
+                    sage: ts
+                    Minimal Translation Cover of Rational Cone Surface built from a square
+                    sage: from flatsurf.geometry.categories import TranslationSurfaces
+                    sage: ts in TranslationSurfaces()
+                    True
+                    sage: hts = cs.minimal_cover(cover_type="half-translation")
+                    sage: hts
+                    Minimal Half-Translation Cover of Genus 0 Rational Cone Surface built from a square
+                    sage: from flatsurf.geometry.categories import HalfTranslationSurfaces
+                    sage: hts in HalfTranslationSurfaces()
+                    True
+                    sage: TestSuite(hts).run()
+                    sage: ps = cs.minimal_cover(cover_type="planar")
+                    sage: ps
+                    Minimal Planar Cover of Genus 0 Rational Cone Surface built from a square
+                    sage: ps in TranslationSurfaces()
+                    True
+                    sage: TestSuite(ps).run()
+
+                    sage: from flatsurf import similarity_surfaces
+                    sage: S = similarity_surfaces.example()
+                    sage: T = S.minimal_cover(cover_type="translation")
+                    sage: T
+                    Minimal Translation Cover of Genus 1 Surface built from 2 isosceles triangles
+                    sage: T in TranslationSurfaces()
+                    True
+                    sage: T.polygon(T.root())
+                    Polygon(vertices=[(0, 0), (2, -2), (2, 0)])
+
+                """
+                if cover_type == "translation":
+                    from flatsurf.geometry.minimal_cover import MinimalTranslationCover
+
+                    return MinimalTranslationCover(self)
+
+                if cover_type == "half-translation":
+                    from flatsurf.geometry.minimal_cover import (
+                        MinimalHalfTranslationCover,
+                    )
+
+                    return MinimalHalfTranslationCover(self)
+
+                if cover_type == "planar":
+                    from flatsurf.geometry.minimal_cover import MinimalPlanarCover
+
+                    return MinimalPlanarCover(self)
+
+                raise ValueError("Provided cover_type is not supported.")
+
+            def vector_space(self):
+                r"""
+                Return the vector space in which self naturally embeds.
+
+                EXAMPLES::
+
+                    sage: from flatsurf import translation_surfaces
+                    sage: S = translation_surfaces.square_torus()
+                    sage: S.vector_space()
+                    doctest:warning
+                    ...
+                    UserWarning: vector_space() has been deprecated and will be removed in a future version of sage-flatsurf; use base_ring()**2 or base_ring().fraction_field()**2 instead
+                    Vector space of dimension 2 over Rational Field
+
+                    sage: S.base_ring()**2
+                    Vector space of dimension 2 over Rational Field
+
+                """
+                import warnings
+
+                warnings.warn(
+                    "vector_space() has been deprecated and will be removed in a future version of sage-flatsurf; use base_ring()**2 or base_ring().fraction_field()**2 instead"
+                )
+
+                from sage.modules.free_module import VectorSpace
+
+                return VectorSpace(self.base_ring(), 2)
+
+            @cached_method(key=lambda self, ring: ring or self.base_ring())
+            def tangent_bundle(self, ring=None):
+                r"""
+                Return the tangent bundle
+
+                INPUT:
+
+                - ``ring`` -- an optional field (defaults to the coordinate field of the
+                  surface)
+                """
+                if ring is None:
+                    ring = self.base_ring()
+
+                if self.is_mutable():
+                    raise NotImplementedError(
+                        "cannot compute the tangent bundle of a mutable surface"
+                    )
+
+                from flatsurf.geometry.tangent_bundle import (
+                    SimilaritySurfaceTangentBundle,
+                )
+
+                return SimilaritySurfaceTangentBundle(self, ring)
+
+            def tangent_vector(self, lab, p, v, ring=None):
+                r"""
+                Return a tangent vector.
+
+                INPUT:
+
+                - ``lab`` -- label of a polygon
+
+                - ``p`` -- coordinates of a point in the polygon
+
+                - ``v`` -- coordinates of a vector in R^2
+
+                EXAMPLES::
+
+                    sage: from flatsurf.geometry.chamanara import chamanara_surface
+                    sage: S = chamanara_surface(1/2)
+                    sage: S.tangent_vector(S.root(), (1/2,1/2), (1,1))
+                    SimilaritySurfaceTangentVector in polygon (1, -1, 0) based at (1/2, -3/2) with vector (1, 1)
+                    sage: K.<sqrt2> = QuadraticField(2)
+                    sage: S.tangent_vector(S.root(), (1/2,1/2), (1,sqrt2), ring=K)
+                    SimilaritySurfaceTangentVector in polygon (1, -1, 0) based at (1/2, -3/2) with vector (1, sqrt2)
+                """
+                from sage.all import vector
+
+                p = vector(p)
+                v = vector(v)
+
+                if p.parent().dimension() != 2 or v.parent().dimension() != 2:
+                    raise ValueError(
+                        "p (={!r}) and v (={!v}) should have two coordinates"
+                    )
+
+                return self.tangent_bundle(ring=ring)(lab, p, v)
+
+            def triangulation_mapping(self):
+                r"""
+                Return a ``SurfaceMapping`` triangulating the surface
+                or ``None`` if the surface is already triangulated.
+                """
+                from flatsurf.geometry.mappings import triangulation_mapping
+
+                return triangulation_mapping(self)
+
+            def triangulate(self, in_place=False, label=None, relabel=None):
+                r"""
+                Return a triangulated version of this surface. (This may be mutable
+                or not depending on the input.)
+
+                If label=None (as default) all polygons are triangulated. Otherwise,
+                label should be a polygon label. In this case, just this polygon
+                is split into triangles.
+
+                This is done in place if in_place is True (defaults to False).
+
+                EXAMPLES::
+
+                    sage: from flatsurf import translation_surfaces
+                    sage: s=translation_surfaces.mcmullen_L(1,1,1,1)
+                    sage: ss=s.triangulate()
+                    sage: gs=ss.graphical_surface()
+                    sage: gs.make_all_visible()
+                    sage: gs
+                    Graphical representation of Translation Surface in H_2(2) built from 6 isosceles triangles
+
+                A non-strictly convex example that caused trouble:
+
+                    sage: from flatsurf import similarity_surfaces, Polygon
+                    sage: s=similarity_surfaces.self_glued_polygon(Polygon(edges=[(1,1),(-3,-1),(1,0),(1,0)]))
+                    sage: s=s.triangulate()
+                    sage: len(s.polygon(0).vertices())
+                    3
+                """
+                if relabel is not None:
+                    import warnings
+
+                    warnings.warn(
+                        "the relabel keyword argument of triangulate() is ignored, it has been deprecated and will be removed in a future version of sage-flatsurf"
+                    )
 
-    def point(self, label, point, ring=None, limit=None):
-        r"""
-        Return a point in this surface.
+                if in_place:
+                    raise NotImplementedError(
+                        "this surface does not implement triangulate(in_place=True) yet"
+                    )
+
+                if self.is_finite_type():
+                    from flatsurf.geometry.surface import (
+                        MutableOrientedSimilaritySurface,
+                    )
+
+                    s = MutableOrientedSimilaritySurface.from_surface(self)
+                    s.triangulate(in_place=True, label=label, relabel=relabel)
+                    s.set_immutable()
+                    return s
 
-        INPUT:
+                if label is not None:
+                    raise NotImplementedError(
+                        "triangulate(label=) not implemented for infinite type surfaces"
+                    )
 
-        - ``label`` - label of the polygon
+                from flatsurf.geometry.delaunay import LazyTriangulatedSurface
 
-        - ``point`` - coordinates of the point inside the polygon
+                return LazyTriangulatedSurface(self)
 
-        - ``ring`` (optional) - a ring for the coordinates
+            def _delaunay_edge_needs_flip(self, p1, e1):
+                r"""
+                Return whether edge ``e1`` of polygon ``p1`` should be flipped
+                to get closer to a Delaunay triangulated surface.
+                """
+                p2, e2 = self.opposite_edge(p1, e1)
+                poly1 = self.polygon(p1)
+                poly2 = self.polygon(p2)
+                if len(poly1.vertices()) != 3 or len(poly2.vertices()) != 3:
+                    raise ValueError("Edge must be adjacent to two triangles.")
+                from flatsurf.geometry.similarity import similarity_from_vectors
+
+                sim1 = similarity_from_vectors(poly1.edge(e1 + 2), -poly1.edge(e1 + 1))
+                sim2 = similarity_from_vectors(poly2.edge(e2 + 2), -poly2.edge(e2 + 1))
+                sim = sim1 * sim2
+                return sim[1][0] < 0
+
+            def _delaunay_edge_needs_join(self, p1, e1):
+                r"""
+                Return whether edge ``e1`` of polygon ``p1`` should be
+                eliminated and the polygons attached to it joined to get closer
+                to a Delaunay cell decomposition.
+                """
+                p2, e2 = self.opposite_edge(p1, e1)
+                poly1 = self.polygon(p1)
+                poly2 = self.polygon(p2)
+                from flatsurf.geometry.similarity import similarity_from_vectors
+
+                sim1 = similarity_from_vectors(
+                    poly1.vertex(e1) - poly1.vertex(e1 + 2), -poly1.edge(e1 + 1)
+                )
+                sim2 = similarity_from_vectors(
+                    poly2.vertex(e2) - poly2.vertex(e2 + 2), -poly2.edge(e2 + 1)
+                )
+                sim = sim1 * sim2
+
+                return sim[1][0] == 0
+
+            def is_delaunay_triangulated(self, limit=None):
+                r"""
+                Return whether the surface is triangulated and the
+                triangulation is Delaunay.
+
+                INPUT:
+
+                - ``limit`` -- an integer or ``None`` (default: ``None``);
+                  check only ``limit`` many edges if set
+
+                """
+                if not self.is_finite_type() and limit is None:
+                    raise NotImplementedError(
+                        "a limit must be set for infinite surfaces."
+                    )
 
-        - ``limit`` (optional) - undocumented (only necessary if the point corresponds
-          to a singularity in an infinite surface)
+                count = 0
 
-        EXAMPLES::
+                for (l1, e1), (l2, e2) in self.gluings():
+                    if limit is not None and count >= limit:
+                        break
+                    count += 1
+                    if len(self.polygon(l1).vertices()) != 3:
+                        return False
+                    if len(self.polygon(l2).vertices()) != 3:
+                        return False
+                    if self._delaunay_edge_needs_flip(l1, e1):
+                        return False
 
-            sage: from flatsurf import *
-            sage: s = translation_surfaces.square_torus()
-            sage: pc = s.minimal_cover(cover_type="planar")
-            sage: pc.surface_point(pc.base_label(),(0,0))
-            Traceback (most recent call last):
-            ...
-            ValueError: need a limit when working with an infinite surface
-            sage: pc.surface_point(pc.base_label(),(1,0),limit=4)
-            Surface point with 4 coordinate representations
-            sage: z = pc.surface_point(pc.base_label(),(sqrt(2)-1,sqrt(3)-1),ring=AA)
-            sage: next(iter(z.coordinates(z.labels()[0]))).parent()
-            Vector space of dimension 2 over Algebraic Real Field
-        """
-        return SurfacePoint(self, label, point, ring=ring, limit=limit)
+                return True
 
-    # TODO: deprecate
-    surface_point = point
+            def is_delaunay_decomposed(self, limit=None):
+                r"""
+                Return if the decomposition of the surface into polygons is Delaunay.
 
-    def ramified_cover(self, degree, data):
-        r"""
-        Build a ramified cover of this surface with given ``degree`` and ramification ``data``.
+                INPUT:
 
-        INPUT:
+                - ``limit`` -- an integer or ``None`` (default: ``None``);
+                  check only ``limit`` many polygons if set
 
-        - ``degree`` (integer) -- the degree of the cover
+                """
+                if not self.is_finite_type() and limit is None:
+                    raise NotImplementedError(
+                        "a limit must be set for infinite surfaces."
+                    )
 
-        - ``data`` -- dictionary that associates a pair ``(polygon_label, edge_number)`` a permutation
-          of ``{1, 2, ..., d}``
+                count = 0
 
-        EXAMPLES:
+                for l1, p1 in zip(self.labels(), self.polygons()):
+                    if limit is not None and count >= limit:
+                        break
 
-        The L-shape origami::
+                    count += 1
 
-            sage: import flatsurf
-            sage: T = flatsurf.translation_surfaces.square_torus()
-            sage: T.ramified_cover(3, {(0,0): '(1,2)', (0,1): '(1,3)'})
-            TranslationSurface built from 3 polygons
-            sage: O = T.ramified_cover(3, {(0,0): '(1,2)', (0,1): '(1,3)'})
-            sage: O.stratum()
-            H_2(2)
+                    try:
+                        c1 = p1.circumscribing_circle()
+                    except ValueError:
+                        # p1 is not circumscribed
+                        return False
+
+                    for e1 in range(len(p1.vertices())):
+                        c2 = self.edge_transformation(l1, e1) * c1
+                        l2, e2 = self.opposite_edge(l1, e1)
+                        if c2.point_position(self.polygon(l2).vertex(e2 + 2)) != -1:
+                            # The circumscribed circle developed into the adjacent polygon
+                            # contains a vertex in its interior or boundary.
+                            return False
 
-        TESTS::
+                return True
 
-            sage: import flatsurf
-            sage: T = flatsurf.translation_surfaces.square_torus()
-            sage: T.ramified_cover(3, {(0,0): '(1,2)', (0,2): '(1,3)'})
-            Traceback (most recent call last):
-            ...
-            ValueError: inconsistent covering data
-        """
-        if not self.is_finite():
-            raise ValueError("this method is only available for finite surfaces")
-        return type(self)(self._s.ramified_cover(degree, data))
+            def delaunay_triangulation(
+                self,
+                triangulated=False,
+                in_place=False,
+                direction=None,
+                relabel=None,
+            ):
+                r"""
+                Returns a Delaunay triangulation of a surface, or make some
+                triangle flips to get closer to the Delaunay decomposition.
+
+                INPUT:
+
+                - ``triangulated`` (boolean) - If true, the algorithm assumes the
+                  surface is already triangulated. It does this without verification.
+
+                - ``in_place`` (boolean) - If true, the triangulating and the
+                  triangle flips are done in place.  Otherwise, a mutable copy of the
+                  surface is made.
+
+                - ``direction`` (None or Vector) - with two entries in the base field
+                    Used to determine labels when a pair of triangles is flipped. Each triangle
+                    has a unique separatrix which points in the provided direction or its
+                    negation. As such a vector determines a sign for each triangle.
+                    A pair of adjacent triangles have opposite signs. Labels are chosen
+                    so that this sign is preserved (as a function of labels).
+
+                EXAMPLES::
+
+                    sage: from flatsurf import translation_surfaces
+
+                    sage: m = matrix([[2,1],[1,1]])
+                    sage: s = m*translation_surfaces.infinite_staircase()
+                    sage: ss = s.delaunay_triangulation()
+                    sage: ss.root()
+                    (0, (0, 1, 2))
+                    sage: ss.polygon((0, (0, 1, 2)))
+                    Polygon(vertices=[(0, 0), (1, 0), (1, 1)])
+                    sage: TestSuite(ss).run()
+                    sage: ss.is_delaunay_triangulated(limit=10)
+                    True
+                """
+                if in_place:
+                    raise NotImplementedError(
+                        "this surface does not implement delaunay_triangulation(in_place=True) yet"
+                    )
+
+                if relabel is not None:
+                    if relabel:
+                        raise NotImplementedError(
+                            "the relabel keyword has been removed from delaunay_triangulation(); use relabel({old: new for (new, old) in enumerate(surface.labels())}) to use integer labels instead"
+                        )
+                    else:
+                        import warnings
 
-    def minimal_cover(self, cover_type = "translation"):
-        r"""
-        Return the minimal translation or half-translation cover of the surface.
+                        warnings.warn(
+                            "the relabel keyword will be removed in a future version of sage-flatsurf; do not pass it explicitly anymore to delaunay_triangulation()"
+                        )
+
+                if self.is_finite_type():
+                    from flatsurf.geometry.surface import (
+                        MutableOrientedSimilaritySurface,
+                    )
+
+                    s = MutableOrientedSimilaritySurface.from_surface(self)
+                    s.delaunay_triangulation(
+                        triangulated=triangulated,
+                        in_place=True,
+                        direction=direction,
+                        relabel=relabel,
+                    )
+                    s.set_immutable()
+                    return s
 
-        Cover type may be either "translation", "half-translation" or "planar".
+                from flatsurf.geometry.delaunay import (
+                    LazyDelaunayTriangulatedSurface,
+                )
+
+                return LazyDelaunayTriangulatedSurface(
+                    self, direction=direction, category=self.category()
+                )
+
+            def delaunay_decomposition(
+                self,
+                triangulated=False,
+                delaunay_triangulated=False,
+                in_place=False,
+                direction=None,
+                relabel=None,
+            ):
+                r"""
+                Return the Delaunay Decomposition of this surface.
+
+                INPUT:
+
+                - ``triangulated`` (boolean) - If true, the algorithm assumes the
+                  surface is already triangulated. It does this without verification.
+
+                - ``delaunay_triangulated`` (boolean) - If true, the algorithm assumes
+                  the surface is already delaunay_triangulated. It does this without
+                  verification.
+
+                - ``in_place`` (boolean) - If true, the triangulating and the triangle
+                  flips are done in place. Otherwise, a mutable copy of the surface is
+                  made.
+
+                - ``direction`` - (None or Vector with two entries in the base field) -
+                  Used to determine labels when a pair of triangles is flipped. Each triangle
+                  has a unique separatrix which points in the provided direction or its
+                  negation. As such a vector determines a sign for each triangle.
+                  A pair of adjacent triangles have opposite signs. Labels are chosen
+                  so that this sign is preserved (as a function of labels).
+
+                EXAMPLES::
+
+                    sage: from flatsurf import translation_surfaces, Polygon, similarity_surfaces
+                    sage: s0 = translation_surfaces.octagon_and_squares()
+                    sage: a = s0.base_ring().gens()[0]
+                    sage: m = Matrix([[1,2+a],[0,1]])
+                    sage: s = m*s0
+                    sage: s = s.triangulate()
+                    sage: ss = s.delaunay_decomposition(triangulated=True)
+                    sage: len(ss.polygons())
+                    3
+
+                    sage: p = Polygon(edges=[(4,0),(-2,1),(-2,-1)])
+                    sage: s0 = similarity_surfaces.self_glued_polygon(p)
+                    sage: s = s0.delaunay_decomposition()
+                    sage: TestSuite(s).run()
+
+                    sage: m = matrix([[2,1],[1,1]])
+                    sage: s = m*translation_surfaces.infinite_staircase()
+                    sage: ss = s.delaunay_decomposition()
+                    sage: ss.root()
+                    (0, (0, 1, 2))
+                    sage: ss.polygon(ss.root())
+                    Polygon(vertices=[(0, 0), (1, 0), (1, 1), (0, 1)])
+                    sage: TestSuite(ss).run()
+                    sage: ss.is_delaunay_decomposed(limit=10)
+                    True
 
-        The minimal planar cover of a surface S is the smallest cover C so that
-        the developing map from the universal cover U to the plane induces a
-        well defined map from C to the plane. This is an infinite translation
-        surface that is naturally a branched cover of the plane.
+                """
+                if in_place:
+                    raise NotImplementedError(
+                        "this surface does not implement delaunay_decomposition(in_place=True) yet"
+                    )
+
+                if relabel is not None:
+                    if relabel:
+                        raise NotImplementedError(
+                            "the relabel keyword has been removed from delaunay_decomposition(); use relabel({old: new for (new, old) in enumerate(surface.labels())}) to use integer labels instead"
+                        )
+                    else:
+                        import warnings
 
-        EXAMPLES::
+                        warnings.warn(
+                            "the relabel keyword will be removed in a future version of sage-flatsurf; do not pass it explicitly anymore to delaunay_decomposition()"
+                        )
+
+                if not self.is_finite_type():
+                    from flatsurf.geometry.delaunay import LazyDelaunaySurface
+
+                    return LazyDelaunaySurface(
+                        self, direction=direction, category=self.category()
+                    )
+
+                from flatsurf.geometry.surface import (
+                    MutableOrientedSimilaritySurface,
+                )
+
+                s = MutableOrientedSimilaritySurface.from_surface(self)
+                s.delaunay_decomposition(
+                    triangulated=triangulated,
+                    delaunay_triangulated=delaunay_triangulated,
+                    in_place=True,
+                    direction=direction,
+                    relabel=relabel,
+                )
+                s.set_immutable()
+                return s
 
-            sage: from flatsurf.geometry.surface import Surface_list
-            sage: s = Surface_list(QQ)
-            sage: from flatsurf.geometry.polygon import polygons
-            sage: square = polygons.square(field=QQ)
-            sage: s.add_polygon(square)
-            0
-            sage: s.change_edge_gluing(0,0,0,1)
-            sage: s.change_edge_gluing(0,2,0,3)
-            sage: from flatsurf.geometry.cone_surface import ConeSurface
-            sage: cs = ConeSurface(s)
-            sage: ts = cs.minimal_cover(cover_type="translation")
-            sage: ts
-            TranslationSurface built from 4 polygons
-            sage: hts = cs.minimal_cover(cover_type="half-translation")
-            sage: hts
-            HalfTranslationSurface built from 2 polygons
-            sage: TestSuite(hts).run()
-            sage: ps = cs.minimal_cover(cover_type="planar")
-            sage: ps
-            TranslationSurface built from infinitely many polygons
-            sage: TestSuite(ps).run(skip="_test_pickling")
-
-            sage: from flatsurf import similarity_surfaces
-            sage: S = similarity_surfaces.example()
-            sage: T = S.minimal_cover(cover_type="translation")
-            sage: T
-            TranslationSurface built from infinitely many polygons
-            sage: T.polygon(T.base_label())
-            Polygon: (0, 0), (2, -2), (2, 0)
-        """
-        if cover_type == "translation":
-            from flatsurf.geometry.translation_surface import TranslationSurface
-            from flatsurf.geometry.minimal_cover import MinimalTranslationCover
-            return TranslationSurface(MinimalTranslationCover(self))
-        if cover_type == "half-translation":
-            from flatsurf.geometry.half_translation_surface import HalfTranslationSurface
-            from flatsurf.geometry.minimal_cover import MinimalHalfTranslationCover
-            return HalfTranslationSurface(MinimalHalfTranslationCover(self))
-        if cover_type == "planar":
-            from flatsurf.geometry.translation_surface import TranslationSurface
-            from flatsurf.geometry.minimal_cover import MinimalPlanarCover
-            return TranslationSurface(MinimalPlanarCover(self))
-        raise ValueError("Provided cover_type is not supported.")
+            def saddle_connections(
+                self,
+                squared_length_bound,
+                initial_label=None,
+                initial_vertex=None,
+                sc_list=None,
+                check=False,
+            ):
+                r"""
+                Returns a list of saddle connections on the surface whose length squared is less than or equal to squared_length_bound.
+                The length of a saddle connection is measured using holonomy from polygon in which the trajectory starts.
+
+                If initial_label and initial_vertex are not provided, we return all saddle connections satisfying the bound condition.
+
+                If initial_label and initial_vertex are provided, it only provides saddle connections emanating from the corresponding
+                vertex of a polygon. If only initial_label is provided, the added saddle connections will only emanate from the
+                corresponding polygon.
+
+                If sc_list is provided the found saddle connections are appended to this list and the resulting list is returned.
+
+                If check==True it uses the checks in the SaddleConnection class to sanity check our results.
+
+                EXAMPLES::
+                    sage: from flatsurf import translation_surfaces
+                    sage: s = translation_surfaces.square_torus()
+                    sage: sc_list = s.saddle_connections(13, check=True)
+                    sage: len(sc_list)
+                    32
+                """
+                if squared_length_bound <= 0:
+                    raise ValueError
+
+                if sc_list is None:
+                    sc_list = []
+                if initial_label is None:
+                    if not self.is_finite_type():
+                        raise NotImplementedError
+                    if initial_vertex is not None:
+                        raise ValueError(
+                            "when initial_label is not provided, then initial_vertex must not be provided either"
+                        )
+                    for label in self.labels():
+                        self.saddle_connections(
+                            squared_length_bound, initial_label=label, sc_list=sc_list
+                        )
+                    return sc_list
+                if initial_vertex is None:
+                    for vertex in range(len(self.polygon(initial_label).vertices())):
+                        self.saddle_connections(
+                            squared_length_bound,
+                            initial_label=initial_label,
+                            initial_vertex=vertex,
+                            sc_list=sc_list,
+                        )
+                    return sc_list
+
+                # Now we have a specified initial_label and initial_vertex
+                from flatsurf.geometry.similarity import SimilarityGroup
+
+                SG = SimilarityGroup(self.base_ring())
+                start_data = (initial_label, initial_vertex)
+                from flatsurf.geometry.circle import Circle
+
+                circle = Circle(
+                    (0, 0),
+                    squared_length_bound,
+                    base_ring=self.base_ring(),
+                )
+                p = self.polygon(initial_label)
+                v = p.vertex(initial_vertex)
+                last_sim = SG(-v[0], -v[1])
+
+                # First check the edge eminating rightward from the start_vertex.
+                e = p.edge(initial_vertex)
+                if e[0] ** 2 + e[1] ** 2 <= squared_length_bound:
+                    from flatsurf.geometry.surface_objects import SaddleConnection
+
+                    sc_list.append(SaddleConnection(self, start_data, e))
+
+                # Represents the bounds of the beam of trajectories we are sending out.
+                wedge = (
+                    last_sim(p.vertex((initial_vertex + 1) % len(p.vertices()))),
+                    last_sim(
+                        p.vertex(
+                            (initial_vertex + len(p.vertices()) - 1) % len(p.vertices())
+                        )
+                    ),
+                )
+
+                # This will collect the data we need for a depth first search.
+                chain = [
+                    (
+                        last_sim,
+                        initial_label,
+                        wedge,
+                        [
+                            (initial_vertex + len(p.vertices()) - i) % len(p.vertices())
+                            for i in range(2, len(p.vertices()))
+                        ],
+                    )
+                ]
+
+                while len(chain) > 0:
+                    # Should verts really be edges?
+                    sim, label, wedge, verts = chain[-1]
+                    if len(verts) == 0:
+                        chain.pop()
+                        continue
+                    vert = verts.pop()
+                    p = self.polygon(label)
+                    # First check the vertex
+                    vert_position = sim(p.vertex(vert))
+                    from flatsurf.geometry.euclidean import ccw
+
+                    if (
+                        ccw(wedge[0], vert_position) > 0
+                        and ccw(vert_position, wedge[1]) > 0
+                        and vert_position[0] ** 2 + vert_position[1] ** 2
+                        <= squared_length_bound
+                    ):
+                        sc_list.append(
+                            SaddleConnection(
+                                self,
+                                start_data,
+                                vert_position,
+                                end_data=(label, vert),
+                                end_direction=~sim.derivative() * -vert_position,
+                                holonomy=vert_position,
+                                end_holonomy=~sim.derivative() * -vert_position,
+                                check=check,
+                            )
+                        )
+                    # Now check if we should develop across the edge
+                    vert_position2 = sim(p.vertex((vert + 1) % len(p.vertices())))
+                    if (
+                        ccw(vert_position, vert_position2) > 0
+                        and ccw(wedge[0], vert_position2) > 0
+                        and ccw(vert_position, wedge[1]) > 0
+                        and circle.line_segment_position(vert_position, vert_position2)
+                        == 1
+                    ):
+                        if ccw(wedge[0], vert_position) > 0:
+                            # First in new_wedge should be vert_position
+                            if ccw(vert_position2, wedge[1]) > 0:
+                                new_wedge = (vert_position, vert_position2)
+                            else:
+                                new_wedge = (vert_position, wedge[1])
+                        else:
+                            if ccw(vert_position2, wedge[1]) > 0:
+                                new_wedge = (wedge[0], vert_position2)
+                            else:
+                                new_wedge = wedge
+                        new_label, new_edge = self.opposite_edge(label, vert)
+                        new_sim = sim * ~self.edge_transformation(label, vert)
+                        p = self.polygon(new_label)
+                        chain.append(
+                            (
+                                new_sim,
+                                new_label,
+                                new_wedge,
+                                [
+                                    (new_edge + len(p.vertices()) - i)
+                                    % len(p.vertices())
+                                    for i in range(1, len(p.vertices()))
+                                ],
+                            )
+                        )
+                return sc_list
+
+            def ramified_cover(self, d, data):
+                r"""
+                Return a ramified cover of this surface.
+
+                INPUT:
+
+                - ``d`` - integer (the degree of the cover)
+
+                - ``data`` - a dictionary which to a pair ``(label, edge_num)`` associates a permutation
+                  of {1,...,d}
+
+                EXAMPLES:
+
+                The L-shape origami::
+
+                    sage: import flatsurf
+                    sage: T = flatsurf.translation_surfaces.square_torus()
+                    sage: T.ramified_cover(3, {(0,0): '(1,2)', (0,1): '(1,3)'})
+                    Translation Surface in H_2(2) built from 3 squares
+                    sage: O = T.ramified_cover(3, {(0,0): '(1,2)', (0,1): '(1,3)'})
+                    sage: O.stratum()
+                    H_2(2)
+
+                TESTS::
+
+                    sage: import flatsurf
+                    sage: T = flatsurf.translation_surfaces.square_torus()
+                    sage: T.ramified_cover(3, {(0,0): '(1,2)', (0,2): '(1,3)'})
+                    Traceback (most recent call last):
+                    ...
+                    ValueError: inconsistent covering data
+
+                """
+                from sage.groups.perm_gps.permgroup_named import SymmetricGroup
+
+                G = SymmetricGroup(d)
+                for k in data:
+                    data[k] = G(data[k])
+                from flatsurf.geometry.surface import MutableOrientedSimilaritySurface
+
+                cover = MutableOrientedSimilaritySurface(self.base_ring())
+                edges = set(self.edges())
+                cover_labels = {}
+                for i in range(1, d + 1):
+                    for lab in self.labels():
+                        cover_labels[(lab, i)] = cover.add_polygon(self.polygon(lab))
+                while edges:
+                    lab, e = elab = edges.pop()
+                    llab, ee = eelab = self.opposite_edge(lab, e)
+                    edges.remove(eelab)
+                    if elab in data:
+                        if eelab in data:
+                            if not (data[elab] * data[eelab]).is_one():
+                                raise ValueError("inconsistent covering data")
+                        s = data[elab]
+                    elif eelab in data:
+                        s = ~data[eelab]
+                    else:
+                        s = G.one()
 
-    def minimal_translation_cover(self):
-        r"""
-        Return the minimal translation cover.
+                    for i in range(1, d + 1):
+                        p0 = cover_labels[(lab, i)]
+                        p1 = cover_labels[(lab, s(i))]
+                        cover.glue((p0, e), (p1, ee))
+                cover.set_immutable()
+                return cover
+
+            def subdivide(self):
+                r"""
+                Return a copy of this surface whose polygons have been partitioned into
+                smaller triangles with
+                :meth:`~.euclidean_polygons.EuclideanPolygons.Simple.Convex.ParentMethods.subdivide`.
+
+                EXAMPLES:
+
+                A surface consisting of a single triangle::
+
+                    sage: from flatsurf import MutableOrientedSimilaritySurface, Polygon
+
+                    sage: S = MutableOrientedSimilaritySurface(QQ)
+                    sage: S.add_polygon(Polygon(edges=[(1, 0), (0, 1), (-1, -1)]), label="Δ")
+                    'Δ'
+
+                Subdivision of this surface yields a surface with three triangles::
+
+                    sage: T = S.subdivide()
+                    sage: T.labels()
+                    (('Δ', 0), ('Δ', 1), ('Δ', 2))
+
+                Note that the new labels are old labels plus an index. We verify that
+                the triangles are glued correctly::
+
+                    sage: list(T.gluings())
+                    [((('Δ', 0), 1), (('Δ', 1), 2)),
+                     ((('Δ', 0), 2), (('Δ', 2), 1)),
+                     ((('Δ', 1), 1), (('Δ', 2), 2)),
+                     ((('Δ', 1), 2), (('Δ', 0), 1)),
+                     ((('Δ', 2), 1), (('Δ', 0), 2)),
+                     ((('Δ', 2), 2), (('Δ', 1), 1))]
+
+                If we add another polygon to the original surface and glue things, we
+                can see how existing gluings are preserved when subdividing::
+
+                    sage: S.add_polygon(Polygon(edges=[(1, 0), (0, 1), (-1, 0), (0, -1)]), label='□')
+                    '□'
+
+                    sage: S.glue(("Δ", 0), ("□", 2))
+                    sage: S.glue(("□", 1), ("□", 3))
+
+                    sage: T = S.subdivide()
+
+                    sage: T.labels()
+                    (('Δ', 0), ('□', 2), ('Δ', 1), ('Δ', 2), ('□', 3), ('□', 1), ('□', 0))
+                    sage: list(sorted(T.gluings()))
+                    [((('Δ', 0), 0), (('□', 2), 0)),
+                     ((('Δ', 0), 1), (('Δ', 1), 2)),
+                     ((('Δ', 0), 2), (('Δ', 2), 1)),
+                     ((('Δ', 1), 1), (('Δ', 2), 2)),
+                     ((('Δ', 1), 2), (('Δ', 0), 1)),
+                     ((('Δ', 2), 1), (('Δ', 0), 2)),
+                     ((('Δ', 2), 2), (('Δ', 1), 1)),
+                     ((('□', 0), 1), (('□', 1), 2)),
+                     ((('□', 0), 2), (('□', 3), 1)),
+                     ((('□', 1), 0), (('□', 3), 0)),
+                     ((('□', 1), 1), (('□', 2), 2)),
+                     ((('□', 1), 2), (('□', 0), 1)),
+                     ((('□', 2), 0), (('Δ', 0), 0)),
+                     ((('□', 2), 1), (('□', 3), 2)),
+                     ((('□', 2), 2), (('□', 1), 1)),
+                     ((('□', 3), 0), (('□', 1), 0)),
+                     ((('□', 3), 1), (('□', 0), 2)),
+                     ((('□', 3), 2), (('□', 2), 1))]
+
+                """
+                labels = list(self.labels())
+                polygons = [self.polygon(label) for label in labels]
+
+                subdivisions = [p.subdivide() for p in polygons]
+
+                from flatsurf.geometry.surface import MutableOrientedSimilaritySurface
+
+                surface = MutableOrientedSimilaritySurface(self.base())
+
+                # Add subdivided polygons
+                for s, subdivision in enumerate(subdivisions):
+                    label = labels[s]
+                    for p, polygon in enumerate(subdivision):
+                        surface.add_polygon(polygon, label=(label, p))
+
+                surface.set_roots(((label, 0) for label in self.roots()))
+
+                # Add gluings between subdivided polygons
+                for s, subdivision in enumerate(subdivisions):
+                    label = labels[s]
+                    for p in range(len(subdivision)):
+                        surface.glue(
+                            ((label, p), 1), ((label, (p + 1) % len(subdivision)), 2)
+                        )
+
+                        # Add gluing from original surface
+                        opposite = self.opposite_edge(label, p)
+                        if opposite is not None:
+                            surface.glue(((label, p), 0), (opposite, 0))
+
+                return surface
+
+            def subdivide_edges(self, parts=2):
+                r"""
+                Return a copy of this surface whose edges have been split into
+                ``parts`` equal pieces each.
+
+                INPUT:
+
+                - ``parts`` -- a positive integer (default: 2)
+
+                EXAMPLES:
+
+                A surface consisting of a single triangle::
+
+                    sage: from flatsurf import MutableOrientedSimilaritySurface
+                    sage: from flatsurf.geometry.polygon import Polygon
+
+                    sage: S = MutableOrientedSimilaritySurface(QQ)
+                    sage: S.add_polygon(Polygon(edges=[(1, 0), (0, 1), (-1, -1)]), label="Δ")
+                    'Δ'
+
+                Subdividing this triangle yields a triangle with marked points along
+                the edges::
+
+                    sage: T = S.subdivide_edges()
+
+                If we add another polygon to the original surface and glue them, we
+                can see how existing gluings are preserved when subdividing::
+
+                    sage: S.add_polygon(Polygon(edges=[(1, 0), (0, 1), (-1, 0), (0, -1)]), label='□')
+                    '□'
+
+                    sage: S.glue(("Δ", 0), ("□", 2))
+                    sage: S.glue(("□", 1), ("□", 3))
+
+                    sage: T = S.subdivide_edges()
+                    sage: list(sorted(T.gluings()))
+                    [(('Δ', 0), ('□', 5)),
+                     (('Δ', 1), ('□', 4)),
+                     (('□', 2), ('□', 7)),
+                     (('□', 3), ('□', 6)),
+                     (('□', 4), ('Δ', 1)),
+                     (('□', 5), ('Δ', 0)),
+                     (('□', 6), ('□', 3)),
+                     (('□', 7), ('□', 2))]
+
+                """
+                labels = list(self.labels())
+                polygons = [self.polygon(label) for label in labels]
+
+                subdivideds = [p.subdivide_edges(parts=parts) for p in polygons]
+
+                from flatsurf.geometry.surface import MutableOrientedSimilaritySurface
+
+                surface = MutableOrientedSimilaritySurface(self.base())
+
+                # Add subdivided polygons
+                for s, subdivided in enumerate(subdivideds):
+                    surface.add_polygon(subdivided, label=labels[s])
+
+                surface.set_roots(self.roots())
+
+                # Reestablish gluings between polygons
+                for label, polygon, subdivided in zip(labels, polygons, subdivideds):
+                    for e in range(len(polygon.vertices())):
+                        opposite = self.opposite_edge(label, e)
+                        if opposite is not None:
+                            for p in range(parts):
+                                surface.glue(
+                                    (label, e * parts + p),
+                                    (
+                                        opposite[0],
+                                        opposite[1] * parts + (parts - p - 1),
+                                    ),
+                                )
+
+                return surface
+
+    class Rational(SurfaceCategoryWithAxiom):
+        r"""
+        The axiom satisfied by similarity surfaces where all similarities that
+        describe how edges are glued only use rational rotations, i.e.,
+        rotations by a rational multiple of π.
+
+        Note that this differs slightly from the usual definition of
+        "rational". Normally, a surface would be rational if it can be
+        described using only such similarities. Here we require that the
+        similarities used are actually of that kind.
 
-        "Be careful that if the surface is not built from one polygon, this is
-        not the smallest translation cover of the surface." - Vincent
+        EXAMPLES::
 
-        "I disagree with the prior statement. Can you provide an example?" -Pat
-        """
-        from sage.misc.superseded import deprecation
-        deprecation(13109, "minimal_translation_cover is deprecated. Use minimal_cover(cover_type = \"translation\") instead.")
-        from flatsurf.geometry.translation_surface import MinimalTranslationCover, TranslationSurface
-        return TranslationSurface(MinimalTranslationCover(self))
+            sage: from flatsurf import translation_surfaces
+            sage: S = translation_surfaces.infinite_staircase()
+            sage: "Rational" in S.category().axioms()
+            True
 
-    def vector_space(self):
-        r"""
-        Return the vector space in which self naturally embeds.
         """
-        from sage.modules.free_module import VectorSpace
-        return VectorSpace(self.base_ring(), 2)
 
-    def fundamental_group(self, base_label=None):
-        r"""
-        Return the fundamental group of this surface.
-        """
-        if not self.is_finite():
-            raise ValueError("the method only work for finite surfaces")
-        if base_label is None:
-            base_label = self.base_label()
-        from .fundamental_group import FundamentalGroup
-        return FundamentalGroup(self, base_label)
+        class ParentMethods:
+            r"""
+            Provides methods available to all surfaces built from Euclidean
+            polygons glued by similarities that have rational monodromy, i.e.,
+            `monodromy
+            <https://en.wikipedia.org/wiki/(G,X)-manifold#Monodromy>`_ gives
+            similarities whose rotational part has finite order.
 
-    def tangent_bundle(self, ring=None):
-        r"""
-        Return the tangent bundle
+            If you want to add functionality for such surfaces you most likely
+            want to put it here.
+            """
 
-        INPUT:
+            @staticmethod
+            def _is_rational_surface(surface, limit=None):
+                r"""
+                Return whether the gluings of this surface lead to a rational
+                surface, i.e., whether all gluings use similarities whose
+                rotational part uses only a rational multiple of π as a
+                rotation.
 
-        - ``ring`` -- an optional field (defaults to the coordinate field of the
-          surface)
-        """
-        if ring is None:
-            ring = self.base_ring()
+                This is a helper method for
+                :meth:`flatsurf.geometry.categories.similarity_surfaces.ParentMethods.is_rational_surface`.
 
-        try:
-            return self._tangent_bundle_cache[ring]
-        except AttributeError:
-            self._tangent_bundle_cache = {}
-        except KeyError:
-            pass
-
-        from .tangent_bundle import SimilaritySurfaceTangentBundle
-        self._tangent_bundle_cache[ring] = SimilaritySurfaceTangentBundle(self, ring)
-        return self._tangent_bundle_cache[ring]
+                INPUT:
 
-    def tangent_vector(self, lab, p, v, ring=None):
-        r"""
-        Return a tangent vector.
+                - ``limit`` -- an integer or ``None`` (default: ``None``); if set, only
+                  the first ``limit`` polygons are checked
 
-        INPUT:
+                EXAMPLES::
 
-        - ``lab`` -- label of a polygon
+                    sage: from flatsurf import translation_surfaces
+                    sage: S = translation_surfaces.infinite_staircase()
 
-        - ``p`` -- coordinates of a point in the polygon
+                    sage: from flatsurf.geometry.categories import SimilaritySurfaces
+                    sage: SimilaritySurfaces.Rational.ParentMethods._is_rational_surface(S, limit=8)
+                    True
 
-        - ``v`` -- coordinates of a vector in R^2
+                """
+                if "Oriented" not in surface.category().axioms():
+                    raise NotImplementedError
 
-        EXAMPLES::
+                labels = surface.labels()
 
-            sage: from flatsurf.geometry.chamanara import chamanara_surface
-            sage: S = chamanara_surface(1/2)
-            sage: S.tangent_vector(S.base_label(), (1/2,1/2), (1,1))
-            SimilaritySurfaceTangentVector in polygon (1, -1, 0) based at (1/2, -3/2) with vector (1, 1)
-            sage: K.<sqrt2> = QuadraticField(2)
-            sage: S.tangent_vector(S.base_label(), (1/2,1/2), (1,sqrt2), ring=K)
-            SimilaritySurfaceTangentVector in polygon (1, -1, 0) based at (1/2, -3/2) with vector (1, sqrt2)
-        """
-        p = vector(p)
-        v = vector(v)
+                if limit is not None:
+                    from itertools import islice
 
-        if p.parent().dimension() != 2 or v.parent().dimension() != 2:
-            raise ValueError("p (={!r}) and v (={!v}) should have two coordinates")
+                    labels = islice(labels, limit)
 
-        if ring is None:
-            ring = self.base_ring()
-            try:
-                return self.tangent_bundle(ring)(lab, p, v)
-            except TypeError:
-                raise TypeError("Use the ring=??? option to construct tangent vectors in other field different from the base_ring().")
-            # Old version seemed to be to accepting of inputs (eg, from Symbolic Ring)
-            #R = p.base_ring()
-            #if R != v.base_ring():
-            #    from sage.structure.element import get_coercion_model
-            #    cm = get_coercion_model()
-            #    R = cm.common_parent(R, v.base_ring())
-            #    p = p.change_ring(R)
-            #    v = v.change_ring(R)
-
-            #R2 = self.base_ring()
-            #if R != R2:
-            #    if R2.has_coerce_map_from(R):
-            #        p = p.change_ring(R2)
-            #        v = v.change_ring(R2)
-            #        R = R2
-            #    elif not R.has_coerce_map_from(R2):
-            #        raise ValueError("not able to find a common ring for arguments")
-            #return self.tangent_bundle(R)(lab, p, v)
-        else:
-            return self.tangent_bundle(ring)(lab, p, v)
+                checked = set()
 
-    def reposition_polygons(self, in_place=False, relabel=False):
-        r"""
-        We choose a maximal tree in the dual graph of the decomposition into
-        polygons, and ensure that the gluings between two polygons joined by
-        an edge in this tree is by translation.
-
-        This guarantees that the group generated by the edge identifications is
-        minimal among representions of the surface. In particular, if for instance
-        you have a translation surface which is anot representable as a translation
-        surface (because polygons are presented with rotations) then after this
-        change it will be representable as a translation surface.
-        """
-        if not self.is_finite():
-            raise NotImplementedError("Only implemented for finite surfaces.")
-        if in_place:
-            if not self.is_mutable():
-                raise ValueError("reposition_polygons in_place is only available "+\
-                    "for mutable surfaces.")
-            s=self
-        else:
-            s=self.copy(relabel=relabel, mutable=True)
-        w=s.walker()
-        from flatsurf.geometry.similarity import SimilarityGroup
-        S=SimilarityGroup(self.base_ring())
-        identity=S.one()
-        it = iter(w)
-        label = next(it)
-        changes = {label:identity}
-        for label in it:
-            edge = w.edge_back(label)
-            label2,edge2 = s.opposite_edge(label, edge)
-            changes[label] = changes[label2] * s.edge_transformation(label,edge)
-        it = iter(w)
-        # Skip the base label:
-        label = next(it)
-        for label in it:
-            p = s.polygon(label)
-            p = changes[label].derivative()*p
-            s.underlying_surface().change_polygon(label,p)
-        return s
+                for label in labels:
+                    for edge in range(len(surface.polygon(label).vertices())):
 
-    def triangulation_mapping(self):
-        r"""
-        Return a SurfaceMapping triangulating the suface or None if the surface is already triangulated.
-        """
-        from flatsurf.geometry.mappings import triangulation_mapping
-        return triangulation_mapping(self)
+                        cross = surface.opposite_edge(label, edge)
 
-    def triangulate(self, in_place=False, label = None, relabel=False):
-        r"""
-        Return a triangulated version of this surface. (This may be mutable
-        or not depending on the input.)
+                        if cross is None:
+                            continue
 
-        If label=None (as default) all polygons are triangulated. Otherwise,
-        label should be a polygon label. In this case, just this polygon
-        is split into triangles.
-
-        This is done in place if in_place is True (defaults to False).
-
-        If we are not doing triangulation in_place, then we must make a copy.
-        This can be a relabeled copy (indexed by the non-negative ints)
-        or a label preserving copy. The copy is relabeled if relabel=True
-        (default False).
+                        if cross in checked:
+                            continue
 
-        EXAMPLES::
+                        checked.add((label, edge))
 
-            sage: from flatsurf import *
-            sage: s=translation_surfaces.mcmullen_L(1,1,1,1)
-            sage: ss=s.triangulate()
-            sage: gs=ss.graphical_surface()
-            sage: gs.make_all_visible()
-            sage: print(gs)
-            Graphical version of Similarity Surface TranslationSurface built from 6 polygons
-
-        A non-strictly convex example that caused trouble:
-
-            sage: from flatsurf import *
-            sage: s=similarity_surfaces.self_glued_polygon(polygons(edges=[(1,1),(-3,-1),(1,0),(1,0)]))
-            sage: s=s.triangulate()
-            sage: s.polygon(0).num_edges()
-            3
-        """
-        if label is None:
-            # We triangulate the whole surface
-            if self.is_finite():
-                # Store the current labels.
-                labels = [label for label in self.label_iterator()]
-                if in_place:
-                    s=self
-                else:
-                    s=self.copy(mutable=True)
-                # Subdivide each polygon in turn.
-                for l in labels:
-                    s = s.triangulate(in_place=True, label=l)
-                return s
-            else:
-                if in_place:
-                    raise ValueError("You can't triangulate an infinite surface in place.")
-                from flatsurf.geometry.delaunay import LazyTriangulatedSurface
-                return self.__class__(LazyTriangulatedSurface(self))
-        else:
-            poly = self.polygon(label)
-            n=poly.num_edges()
-            if n>3:
-                if in_place:
-                    s=self
-                else:
-                    s=self.copy(mutable=True)
-            else:
-                # This polygon is already a triangle.
-                return self
-            from flatsurf.geometry.polygon import wedge_product
-            for i in range(n-3):
-                poly = s.polygon(label)
-                n=poly.num_edges()
-                for i in range(n):
-                    e1=poly.edge(i)
-                    e2=poly.edge((i+1)%n)
-                    if wedge_product(e1,e2) != 0:
-                        # This is in case the polygon is a triangle with subdivided edge.
-                        e3=poly.edge((i+2)%n)
-                        if wedge_product(e1+e2,e3) != 0:
-                            s.subdivide_polygon(label,i,(i+2)%n)
-                            break
-            return s
-        raise RuntimeError("Failed to return anything!")
+                        # We do not call self.edge_matrix() since the surface might
+                        # have overridden this (just returning the identity matrix e.g.)
+                        # and we want to deduce the matrix from the attached polygon
+                        # edges instead.
+                        matrix = SimilaritySurfaces.Oriented.ParentMethods.edge_matrix.f(  # pylint: disable=no-member
+                            surface, label, edge
+                        )
 
-    def _edge_needs_flip(self,p1,e1):
-        r"""
-        Returns -1 if the the provided edge incident to two triangles which
-        should be flipped to get closer to the Delaunay decomposition.
-        Returns 0 if the quadrilateral formed by the triangles is inscribed
-        in a circle, and returns 1 otherwise.
+                        if matrix.is_diagonal():
+                            continue
 
-        A ValueError is raised if the edge is not indident to two triangles.
-        """
-        p2,e2=self.opposite_edge(p1,e1)
-        poly1=self.polygon(p1)
-        poly2=self.polygon(p2)
-        if poly1.num_edges()!=3 or poly2.num_edges()!=3:
-            raise ValueError("Edge must be adjacent to two triangles.")
-        from flatsurf.geometry.matrix_2x2 import similarity_from_vectors
-        sim1=similarity_from_vectors(poly1.edge(e1+2),-poly1.edge(e1+1))
-        sim2=similarity_from_vectors(poly2.edge(e2+2),-poly2.edge(e2+1))
-        sim=sim1*sim2
-        return sim[1][0]<0
+                        a = AA(matrix[0, 0])
+                        b = AA(matrix[1, 0])
+                        q = (a**2 + b**2).sqrt()
 
-    def _edge_needs_join(self,p1,e1):
-        r"""
-        Returns -1 if the the provided edge incident to two triangles which
-        should be flipped to get closer to the Delaunay decomposition.
-        Returns 0 if the quadrilateral formed by the triangles is inscribed
-        in a circle, and returns 1 otherwise.
+                        from flatsurf.geometry.euclidean import (
+                            is_cosine_sine_of_rational,
+                        )
 
-        A ValueError is raised if the edge is not indident to two triangles.
-        """
-        p2,e2=self.opposite_edge(p1,e1)
-        poly1=self.polygon(p1)
-        poly2=self.polygon(p2)
-        from flatsurf.geometry.matrix_2x2 import similarity_from_vectors
-        sim1=similarity_from_vectors(poly1.vertex(e1) - poly1.vertex(e1+2),\
-            -poly1.edge(e1+1))
-        sim2=similarity_from_vectors(poly2.vertex(e2) - poly2.vertex(e2+2),\
-            -poly2.edge(e2+1))
-        sim=sim1*sim2
-        from sage.functions.generalized import sgn
-        return sim[1][0]==0
+                        if not is_cosine_sine_of_rational(a / q, b / q):
+                            return False
 
-    def delaunay_single_flip(self):
-        r"""
-        Does a single in place flip of a triangulated mutable surface.
-        """
-        if not self.is_finite():
-            raise NotImplementedError("Not implemented for infinite surfaces.")
-        lc = self._label_comparator()
-        for (l1,e1),(l2,e2) in self.edge_iterator(gluings=True):
-            if (lc.lt(l1,l2) or (l1==l2 and e1<=e2)) and self._edge_needs_flip(l1,e1):
-                self.triangle_flip(l1, e1, in_place=True)
                 return True
-        return False
-
-    def is_delaunay_triangulated(self, limit=None):
-        r"""
-        Return if the surface is triangulated and the triangulation is Delaunay.
-        If limit is set, then it checks this only limit many edges.
-        Limit must be set for infinite surfaces.
-        """
-        if limit is None:
-            if not self.is_finite():
-                raise NotImplementedError("A limit must be set for infinite surfaces.")
-            limit = self.num_edges()
-        count = 0
-        for (l1,e1),(l2,e2) in self.edge_iterator(gluings=True):
-            if count >= limit:
-                break
-            count =  count+1
-            if self.polygon(l1).num_edges()!=3:
-                print("Polygon with label "+str(l1)+" is not a triangle.")
-                return False
-            if self.polygon(l2).num_edges()!=3:
-                print("Polygon with label "+str(l2)+" is not a triangle.")
-                return False
-            if self._edge_needs_flip(l1,e1):
-                print("Edge "+str((l1,e1))+" needs to be flipped.")
-                print("This edge is glued to "+str((l2,e2))+".")
-                return False
-        return True
-
-    def is_delaunay_decomposed(self, limit=None):
-        r"""
-        Return if the decomposition of the surface into polygons is Delaunay.
-        If limit is set, then it checks this only limit many polygons.
-        Limit must be set for infinite surfaces.
-        """
-        if limit is None:
-            if not self.is_finite():
-                raise NotImplementedError("A limit must be set for infinite surfaces.")
-            limit = self.num_polygons()
-        count = 0
-        for (l1,p1) in self.label_iterator(polygons=True):
-            try:
-                c1=p1.circumscribing_circle()
-            except ValueError:
-                # p1 is not circumscribed
-                return False
-            for e1 in range(p1.num_edges()):
-                c2=self.edge_transformation(l1,e1)*c1
-                l2,e2=self.opposite_edge(l1,e1)
-                if c2.point_position(self.polygon(l2).vertex(e2+2))!=-1:
-                    # The circumscribed circle developed into the adjacent polygon
-                    # contains a vertex in its interior or boundary.
-                    return False
-            return True
-
-    def delaunay_triangulation(self, triangulated=False, in_place=False, limit=None, direction=None, relabel=False):
-        r"""
-        Returns a Delaunay triangulation of a surface, or make some
-        triangle flips to get closer to the Delaunay decomposition.
-
-        INPUT:
-
-        - ``triangulated`` (boolean) - If true, the algorithm assumes the
-          surface is already triangulated. It does this without verification.
-
-        - ``in_place`` (boolean) - If true, the triangulating and the
-          triangle flips are done in place.  Otherwise, a mutable copy of the
-          surface is made.
-
-        - ``limit`` (None or Integer) - If None, this will return a
-          Delaunay triangulation. If limit is an integer 1 or larger, then at
-          most limit many diagonal flips will be done.
-
-        - ``direction`` (None or Vector) - with two entries in the base field
-            Used to determine labels when a pair of triangles is flipped. Each triangle
-            has a unique separatrix which points in the provided direction or its
-            negation. As such a vector determines a sign for each triangle.
-            A pair of adjacent triangles have opposite signs. Labels are chosen
-            so that this sign is preserved (as a function of labels).
-
-        - ``relabel`` (boolean) - If in_place is False, then a copy must be
-          made. By default relabel is False and labels will be respected by
-          this copy. If relabel is True then polygons will be reindexed in an
-          arbitrary way by the non-negative integers.
-
-        EXAMPLES::
 
-            sage: from flatsurf import *
-            sage: from flatsurf.geometry.delaunay import *
+            def is_rational_surface(self):
+                r"""
+                Return whether all edges of this surface are glued with
+                similarities whose rotational part is by a rational multiple of
+                π, i.e., return ``True`` since this is a rational surface.
+
+                EXAMPLES::
+
+                    sage: from flatsurf import translation_surfaces
+                    sage: S = translation_surfaces.infinite_staircase()
+                    sage: S.is_rational_surface()
+                    True
 
-            sage: m = matrix([[2,1],[1,1]])
-            sage: s = m*translation_surfaces.infinite_staircase()
-            sage: ss = s.delaunay_triangulation(relabel=True)
-            sage: ss.base_label()
-            0
-            sage: ss.polygon(0)
-            Polygon: (0, 0), (1, 1), (0, 1)
-            sage: TestSuite(ss).run(skip="_test_pickling")
-            sage: ss.is_delaunay_triangulated(limit=10)
-            True
-        """
-        if not self.is_finite() and limit is None:
-            if in_place:
-                raise ValueError("in_place delaunay triangulation is not possible for infinite surfaces unless a limit is set.")
-            if self.underlying_surface().is_mutable():
-                raise ValueError("delaunay_triangulation only works on infinite "+\
-                    "surfaces if they are immutable or if a limit is set.")
-            from flatsurf.geometry.delaunay import LazyDelaunayTriangulatedSurface
-            return self.__class__(LazyDelaunayTriangulatedSurface( \
-                self,direction=direction, relabel=relabel))
-        if in_place and not self.is_mutable():
-            raise ValueError("in_place delaunay_triangulation only defined for mutable surfaces")
-        if triangulated:
-            if in_place:
-                s=self
-            else:
-                s=self.copy(mutable=True, relabel=False)
-        else:
-            if in_place:
-                s=self
-                self.triangulate(in_place=True)
-            else:
-                s=self.copy(relabel=True,mutable=True)
-                s.triangulate(in_place=True)
-        loop=True
-        if direction is None:
-            base_ring = self.base_ring()
-            direction = self.vector_space()( (base_ring.zero(), base_ring.one()) )
-        else:
-            assert not direction.is_zero()
-        if s.is_finite() and limit is None:
-            from collections import deque
-            unchecked_labels=deque(label for label in s.label_iterator())
-            checked_labels = set()
-            while unchecked_labels:
-                label = unchecked_labels.popleft()
-                flipped=False
-                for edge in range(3):
-                    if s._edge_needs_flip(label,edge):
-                        # Record the current opposite edge:
-                        label2,edge2=s.opposite_edge(label,edge)
-                        # Perform the flip.
-                        s.triangle_flip(label, edge, in_place=True, direction=direction)
-                        # Move the opposite polygon to the list of labels we need to check.
-                        if label2 != label:
-                            try:
-                                checked_labels.remove(label2)
-                                unchecked_labels.append(label2)
-                            except KeyError:
-                                # Occurs if label2 is not in checked_labels
-                                pass
-                        flipped=True
-                        break
-                if flipped:
-                    unchecked_labels.append(label)
-                else:
-                    checked_labels.add(label)
-            return s
-        else:
-            # Old method for infinite surfaces, or limits.
-            count=0
-            lc = self._label_comparator()
-            while loop:
-                loop=False
-                for (l1,e1),(l2,e2) in s.edge_iterator(gluings=True):
-                    if (lc.lt(l1,l2) or (l1==l2 and e1<=e2)) and s._edge_needs_flip(l1,e1):
-                        s.triangle_flip(l1, e1, in_place=True, direction=direction)
-                        count += 1
-                        if not limit is None and count>=limit:
-                            return s
-                        loop=True
-                        break
-            return s
-
-    def delaunay_single_join(self):
-        if not self.is_finite():
-            raise NotImplementedError("Not implemented for infinite surfaces.")
-        lc = self._label_comparator()
-        for (l1,e1),(l2,e2) in self.edge_iterator(gluings=True):
-            if (lc.lt(l1,l2) or (l1==l2 and e1<=e2)) and self._edge_needs_join(l1,e1):
-                self.join_polygons(l1, e1, in_place=True)
+                """
                 return True
-        return False
 
+            def _test_rational_surface(self, **options):
+                r"""
+                Verify that this is a rational similarity surface.
 
-    def delaunay_decomposition(self, triangulated=False, \
-            delaunay_triangulated=False, in_place=False, direction=None,\
-            relabel=False):
-        r"""
-        Return the Delaunay Decomposition of this surface.
+                EXAMPLES::
 
-        INPUT:
+                    sage: from flatsurf import translation_surfaces
+                    sage: S = translation_surfaces.square_torus()
+                    sage: S._test_rational_surface()
 
-        - ``triangulated`` (boolean) - If true, the algorithm assumes the
-          surface is already triangulated. It does this without verification.
+                """
+                tester = self._tester(**options)
 
-        - ``delaunay_triangulated`` (boolean) - If true, the algorithm assumes
-          the surface is already delaunay_triangulated. It does this without
-          verification.
-
-        - ``in_place`` (boolean) - If true, the triangulating and the triangle
-          flips are done in place. Otherwise, a mutable copy of the surface is
-          made.
-
-        - ``relabel`` (None or Integer) - If in_place is False, then a copy
-          must be made of the surface.  If relabel is False (as default), the
-          copy has the same labels as the original surface. Note that in this
-          case, labels will be added if it is necessary to subdivide polygons
-          into triangles.  If relabel is True, the new surface will have
-          polygons labeled by the non-negative integers in an arbitrary way.
-
-        - ``direction`` - (None or Vector with two entries in the base field) -
-          Used to determine labels when a pair of triangles is flipped. Each triangle
-          has a unique separatrix which points in the provided direction or its
-          negation. As such a vector determines a sign for each triangle.
-          A pair of adjacent triangles have opposite signs. Labels are chosen
-          so that this sign is preserved (as a function of labels).
+                limit = None
 
-        EXAMPLES::
+                if not self.is_finite_type():
+                    limit = 32
 
-            sage: from flatsurf import *
-            sage: s0 = translation_surfaces.octagon_and_squares()
-            sage: a = s0.base_ring().gens()[0]
-            sage: m = Matrix([[1,2+a],[0,1]])
-            sage: s = m*s0
-            sage: s = s.triangulate()
-            sage: ss = s.delaunay_decomposition(triangulated=True)
-            sage: ss.num_polygons()
-            3
-
-            sage: p = polygons((4,0),(-2,1),(-2,-1))
-            sage: s0 = similarity_surfaces.self_glued_polygon(p)
-            sage: s = s0.delaunay_decomposition()
-            sage: TestSuite(s).run()
-
-            sage: m = matrix([[2,1],[1,1]])
-            sage: s = m*translation_surfaces.infinite_staircase()
-            sage: ss = s.delaunay_decomposition()
-            sage: ss.base_label()
-            0
-            sage: ss.polygon(0)
-            Polygon: (0, 0), (1, 0), (1, 1), (0, 1)
-            sage: TestSuite(ss).run(skip="_test_pickling")
-            sage: ss.is_delaunay_decomposed(limit=10)
-            True
-        """
-        if not self.is_finite():
-            if in_place:
-                raise ValueError("in_place delaunay_decomposition is not possible for infinite surfaces.")
-            if self.underlying_surface().is_mutable():
-                raise ValueError("delaunay_decomposition only works on infinite "+\
-                    "surfaces if they are immutable.")
-            from flatsurf.geometry.delaunay import LazyDelaunaySurface
-            return self.__class__(LazyDelaunaySurface( \
-                self,direction=direction, relabel=relabel))
-        if in_place:
-            s=self
-        else:
-            s=self.copy(mutable=True, relabel=relabel)
-        if not delaunay_triangulated:
-            s.delaunay_triangulation(triangulated=triangulated, in_place=True, \
-                direction=direction)
-        # Now s is Delaunay Triangulated
-        loop=True
-        lc = self._label_comparator()
-        while loop:
-            loop=False
-            for (l1,e1),(l2,e2) in s.edge_iterator(gluings=True):
-                if (lc.lt(l1,l2) or (l1==l2 and e1<=e2)) and s._edge_needs_join(l1,e1):
-                    s.join_polygons(l1, e1, in_place=True)
-                    loop=True
-                    break
-        return s
+                tester.assertTrue(
+                    SimilaritySurfaces.Rational.ParentMethods._is_rational_surface(
+                        self, limit=limit
+                    )
+                )
 
-    def saddle_connections(self, squared_length_bound, initial_label=None, initial_vertex=None, sc_list=None, check=False):
+    class FiniteType(SurfaceCategoryWithAxiom):
         r"""
-        Returns a list of saddle connections on the surface whose length squared is less than or equal to squared_length_bound.
-        The length of a saddle connection is measured using holonomy from polygon in which the trajectory starts.
-
-        If initial_label and initial_vertex are not provided, we return all saddle connections satisfying the bound condition.
-
-        If initial_label and initial_vertex are provided, it only provides saddle connections emanating from the corresponding
-        vertex of a polygon. If only initial_label is provided, the added saddle connections will only emanate from the
-        corresponding polygon.
-
-        If sc_list is provided the found saddle connections are appended to this list and the resulting list is returned.
-
-        If check==True it uses the checks in the SaddleConnection class to sanity check our results.
+        The category of surfaces built by gluing a finite number of Euclidean
+        polygons with similarities.
 
         EXAMPLES::
-            sage: from flatsurf import *
-            sage: s = translation_surfaces.square_torus()
-            sage: sc_list = s.saddle_connections(13, check=True)
-            sage: len(sc_list)
-            32
-        """
-        assert squared_length_bound > 0
-        if sc_list is None:
-            sc_list = []
-        if initial_label is None:
-            assert self.is_finite()
-            assert initial_vertex is None, "If initial_label is not provided, then initial_vertex must not be provided either."
-            for label in self.label_iterator():
-                self.saddle_connections(squared_length_bound, initial_label=label, sc_list=sc_list)
-            return sc_list
-        if initial_vertex is None:
-            for vertex in range( self.polygon(initial_label).num_edges() ):
-                self.saddle_connections(squared_length_bound, initial_label=initial_label, initial_vertex=vertex, sc_list=sc_list)
-            return sc_list
-
-        # Now we have a specified initial_label and initial_vertex
-        SG = SimilarityGroup(self.base_ring())
-        start_data = (initial_label, initial_vertex)
-        circle = Circle(self.vector_space().zero(), squared_length_bound, base_ring =   self.base_ring())
-        p = self.polygon(initial_label)
-        v = p.vertex(initial_vertex)
-        last_sim = SG(-v[0],-v[1])
-
-        # First check the edge eminating rightward from the start_vertex.
-        e = p.edge(initial_vertex)
-        if e[0]**2 + e[1]**2 <= squared_length_bound:
-            sc_list.append( SaddleConnection(self, start_data, e) )
-
-        # Represents the bounds of the beam of trajectories we are sending out.
-        wedge = ( last_sim( p.vertex((initial_vertex+1)%p.num_edges()) ),
-                  last_sim( p.vertex((initial_vertex+p.num_edges()-1)%p.num_edges()) ))
-
-        # This will collect the data we need for a depth first search.
-        chain = [(last_sim, initial_label, wedge, [(initial_vertex+p.num_edges()-i)%p.num_edges() for i in range(2,p.num_edges())])]
-
-        while len(chain)>0:
-            # Should verts really be edges?
-            sim, label, wedge, verts = chain[-1]
-            if len(verts) == 0:
-                chain.pop()
-                continue
-            vert = verts.pop()
-            #print("Inspecting "+str(vert))
-            p = self.polygon(label)
-            # First check the vertex
-            vert_position = sim(p.vertex(vert))
-            #print(wedge[1].n())
-            if wedge_product(wedge[0], vert_position) > 0 and \
-               wedge_product(vert_position, wedge[1]) > 0 and \
-               vert_position[0]**2 + vert_position[1]**2 <= squared_length_bound:
-                    sc_list.append( SaddleConnection(self, start_data, vert_position,
-                                                   end_data = (label,vert),
-                                                   end_direction = ~sim.derivative()*-vert_position,
-                                                   holonomy = vert_position,
-                                                   end_holonomy = ~sim.derivative()*-vert_position,
-                                                   check = check) )
-            # Now check if we should develop across the edge
-            vert_position2 = sim(p.vertex( (vert+1)%p.num_edges() ))
-            if wedge_product(vert_position,vert_position2)>0 and \
-               wedge_product(wedge[0],vert_position2)>0 and \
-               wedge_product(vert_position,wedge[1])>0 and \
-               circle.line_segment_position(vert_position, vert_position2)==1:
-                if wedge_product(wedge[0], vert_position) > 0:
-                    # First in new_wedge should be vert_position
-                    if wedge_product(vert_position2, wedge[1]) > 0:
-                        new_wedge = (vert_position, vert_position2)
-                    else:
-                        new_wedge = (vert_position, wedge[1])
-                else:
-                    if wedge_product(vert_position2, wedge[1]) > 0:
-                        new_wedge = (wedge[0], vert_position2)
-                    else:
-                        new_wedge=wedge
-                new_label, new_edge = self.opposite_edge(label, vert)
-                new_sim = sim*~self.edge_transformation(label,vert)
-                p = self.polygon(new_label)
-                chain.append( (new_sim, new_label, new_wedge, [(new_edge+p.num_edges()-i)%p.num_edges() for i in range(1,p.num_edges())]) )
-        return sc_list
-
-    def set_default_graphical_surface(self, graphical_surface):
-        r"""
-        Replace the default graphical surface with the provided GraphicalSurface.
-        """
-        from flatsurf.graphical.surface import GraphicalSurface
-        if not isinstance(graphical_surface, GraphicalSurface):
-            raise ValueError("graphical_surface must be a GraphicalSurface")
-        if self != graphical_surface.get_surface():
-            raise ValueError("The provided graphical_surface renders a different surface!")
-        self._gs =  graphical_surface
-
-    def graphical_surface(self, *args, **kwds):
-        r"""
-        Return a GraphicalSurface representing this surface.
-
-        By default this returns a cached version of the GraphicalSurface. If
-        ``cached=False`` is provided as a keyword option then a new
-        GraphicalSurface is returned. Other keyword options:
-
-        INPUT:
-
-        - ``cached`` -- a boolean (default ``True``). If true return a cached
-          GraphicalSurface. Otherwise we make a new one.
-
-        - ``polygon_labels`` -- a boolean (default ``True``) whether the label
-          of polygons are displayed
-
-        - ``edge_labels`` -- option to control the display of edge labels. It
-          can be one of
-
-            - ``False`` or ``None`` for no labels
-
-            - ``'gluings'`` -- to put on each side of each non-adjacent edge, the
-              name of the polygon to which it is glued
-
-            - ``'number'`` -- to put on each side of each edge the number of the
-              edge
-
-            - ``'gluings and numbers'`` -- full information
-
-            - ``'letter'`` -- add matching letters to glued edges in an arbitrary way
-
-        - ``default_position_function`` -- a function mapping polygon labels to
-          similarities describing the position of the corresponding polygon.
-
-        EXAMPLES:
-
-        Test the difference between the cached graphical_surface and the uncached version::
-
-            sage: from flatsurf import *
-            sage: s = translation_surfaces.octagon_and_squares()
-            sage: s.plot()     # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 32 graphics primitives
-            sage: s.graphical_surface(cached=False,adjacencies=[]).plot()   # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 18 graphics primitives
-        """
-        from flatsurf.graphical.surface import GraphicalSurface
-        if "cached" in kwds:
-            if not kwds["cached"]:
-                # cached=False: return a new surface.
-                kwds.pop("cached",None)
-                return GraphicalSurface(self, *args, **kwds)
-            kwds.pop("cached",None)
-        if hasattr(self, '_gs'):
-            self._gs.process_options(*args, **kwds)
-        else:
-            self._gs = GraphicalSurface(self, *args, **kwds)
-        return self._gs
-
-    def plot(self, *args, **kwds):
-        r"""
-        Returns a plot of the surface.
-
-        There may be zero or one argument. If provided the single argument
-        should be a GraphicalSurface whick will be used in the plot.
-
-        INPUT:
-
-        - ``polygon_labels`` -- a boolean (default ``True``) whether the label
-          of polygons are displayed
-
-        - ``edge_labels`` -- option to control the display of edge labels. It
-          can be one of
-
-            - ``False`` or ``None`` for no labels
 
-            - ``'gluings'`` -- to put on each side of each non-adjacent edge, the
-              name of the polygon to which it is glued
-
-            - ``'number'`` -- to put on each side of each edge the number of the
-              edge
-
-            - ``'gluings and number'`` -- full information
-
-        - ``adjacencies`` -- a list of pairs ``(p,e)`` to be used to set
-          adjacencies of polygons.
+            sage: from flatsurf import Polygon, similarity_surfaces
+            sage: P = Polygon(vertices=[(0,0), (1,0), (1,1), (0,1)])
+            sage: S = similarity_surfaces.self_glued_polygon(P)
+            sage: "FiniteType" in S.category().axioms()
+            True
 
-        - ``default_position_function`` -- a function mapping polygon labels to
-          similarities describing the position of the corresponding polygon.
         """
-        if len(args) > 1:
-            raise ValueError("SimilaritySurface.plot() can take at most one non-keyword argument.")
-        if len(args)==1:
-            from flatsurf.graphical.surface import GraphicalSurface
-            if not isinstance(args[0], GraphicalSurface):
-                raise ValueError("If an argument is provided, it must be a GraphicalSurface.")
-            gs = args[0]
-            gs.process_options(**kwds)
-        else:
-            gs = self.graphical_surface(**kwds)
-        return gs.plot()
-
-    def plot_polygon(self, label, graphical_surface = None,
-                     plot_polygon = True, plot_edges = True, plot_edge_labels = True,
-                     edge_labels = None,
-                     polygon_options = {"axes":True}, edge_options = None, edge_label_options = None):
-        r"""
-        Returns a plot of the polygon with the provided label.
-
-        Note that this method plots the polygon in its coordinates as opposed to
-        graphical coordinates that the :func:``plot`` method uses. This makes it useful
-        for visualizing the natural coordinates of the polygon.
-
-        INPUT:
-
-            - ``graphical_surface`` -- (default ``None``) If provided this function pulls graphical options
-              from the graphical surface. If not provided, we use the default graphical surface.
-
-            - ``plot_polygon`` -- (default ``True``) If True, we plot the solid polygon.
-
-            - ``polygon_options`` -- (default ``{"axes":True}``) Options for the rendering of the polygon.
-              These options will be passed to :func:`~flatsurf.graphical.polygon.GraphicalPolygon.plot_polygon`.
-              This should be either None or a dictionary.
-
-            - ``plot_edges`` -- (default ``True``) If True, we plot the edges of the polygon as segments.
-
-            - ``edge_options`` -- (default ``None``) Options for the rendering of the polygon edges.
-              These options will be passed to :func:`~flatsurf.graphical.polygon.GraphicalPolygon.plot_edge`.
-              This should be either None or a dictionary.
-
-            - ``plot_edge_labels`` -- (default ``True``) If True, we plot labels on the edges.
-
-            - ``edge_label_options`` -- (default ``None``) Options for the rendering of the edge labels.
-              These options will be passed to :func:`~flatsurf.graphical.polygon.GraphicalPolygon.plot_edge_label`.
-              This should be either None or a dictionary.
-
-            - ``edge_labels`` -- (default ``None``) If None and plot_edge_labels is True, we write the edge
-              number on each edge. Otherwise edge_labels should be a list of strings of length equal to the
-              number of edges of the polygon. The strings will be printed on each edge.
 
-        EXAMPLES::
-
-            sage: from flatsurf import *
-            sage: s = similarity_surfaces.example()
-            sage: s.plot() # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 13 graphics primitives
-            s.plot_polygon(1) # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 7 graphics primitives
-
-            sage: labels = []
-            sage: p = s.polygon(1)
-            sage: for e in range(p.num_edges()): \
-                labels.append(str(p.edge(e)))
-            sage: s.plot_polygon(1, polygon_options=None, plot_edges=False, \
-                edge_labels=labels, edge_label_options={"color":"red"}) # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 4 graphics primitives
-        """
-        if graphical_surface is None:
-            graphical_surface = self.graphical_surface()
-        p = self.polygon(label)
-        from flatsurf.graphical.polygon import GraphicalPolygon
-        gp = GraphicalPolygon(p)
-
-        if plot_polygon:
-            if polygon_options is None:
-                o = graphical_surface.polygon_options
-            else:
-                o = graphical_surface.polygon_options.copy()
-                o.update(polygon_options)
-            plt = gp.plot_polygon(**o)
-
-        if plot_edges:
-            if edge_options is None:
-                o = graphical_surface.non_adjacent_edge_options
-            else:
-                o = graphical_surface.non_adjacent_edge_options.copy()
-                o.update(edge_options)
-            for e in range(p.num_edges()):
-                plt += gp.plot_edge(e, **o)
-
-        if plot_edge_labels:
-            if edge_label_options is None:
-                o = graphical_surface.edge_label_options
-            else:
-                o = graphical_surface.edge_label_options.copy()
-                o.update(edge_label_options)
-            for e in range(p.num_edges()):
-                if edge_labels is None:
-                    el = str(e)
+        class ParentMethods:
+            r"""
+            Provides methods available to all surfaces that are built from
+            finitely many polygons in the real plane glued with similarities.
+
+            If you want to add functionality for such surfaces you most likely
+            want to put it here.
+            """
+
+            def num_singularities(self):
+                r"""
+                EXAMPLES::
+
+                    sage: from flatsurf import translation_surfaces
+
+                    sage: translation_surfaces.regular_octagon().num_singularities()
+                    doctest:warning
+                    ...
+                    UserWarning: num_singularities() has been deprecated and will be removed in a future version of sage-flatsurf; use len(vertices()) instead
+                    1
+
+                    sage: S = SymmetricGroup(4)
+                    sage: r = S('(1,2)(3,4)')
+                    sage: u = S('(2,3)')
+                    sage: translation_surfaces.origami(r,u).num_singularities()
+                    2
+
+                    sage: S = SymmetricGroup(8)
+                    sage: r = S('(1,2,3,4,5,6,7,8)')
+                    sage: u = S('(1,8,5,4)(2,3)(6,7)')
+                    sage: translation_surfaces.origami(r,u).num_singularities()
+                    4
+                """
+                import warnings
+
+                warnings.warn(
+                    "num_singularities() has been deprecated and will be removed in a future version of sage-flatsurf; use len(vertices()) instead"
+                )
+
+                return len(self.vertices())
+
+            def _test_eq_surface(self, **options):
+                r"""
+                Verify that this surface follows our standards for equality of
+                surfaces.
+
+                We want two surfaces to compare equal (`S == T`) iff they are
+                virtually indistinguishable; so without a lot of non-Pythonic
+                effort, you should not be able to tell them apart. They have
+                (virtually) the same type, are made from equally labeled
+                polygons with indistinguishable coordinates and equal gluings.
+                Any other data that was used when creating them should be
+                indistinguishable. They might of course live at different
+                memory addresses have differences in their internal caches and
+                representation but everything user-facing should be the same.
+
+                People often want `==` to mean that the two surfaces are
+                isomorphic in some more-or-less strong sense. Such a notion for
+                `==` always leads to trouble down the road. The operator `==`
+                is used to identify surfaces in caches and identify surfaces in
+                sets. Sometimes "are isomorphic" is a good notion in such cases
+                but most of the time "are indistinguishable" is the much safer
+                default. Also, "are isomorphic" is often costly or, e.g. in the case
+                of infinite surfaces, not even decidable.
+
+                Currently, we do treat two surfaces as equal even if they
+                differ by category because categories can presently be changed
+                for immutable surfaces (as more properties of the surface are
+                found.)
+
+                EXAMPLES::
+
+                    sage: from flatsurf import Polygon, similarity_surfaces
+                    sage: P = Polygon(vertices=[(0,0), (1,0), (1,1), (0,1)])
+                    sage: S = similarity_surfaces.self_glued_polygon(P)
+                    sage: S._test_eq_surface()
+
+                :meta public:
+
+                """
+                tester = self._tester(**options)
+
+                from flatsurf.geometry.surface import MutableOrientedSimilaritySurface
+
+                copy = MutableOrientedSimilaritySurface.from_surface(self)
+                if not self.is_mutable():
+                    copy.set_immutable()
+
+                if isinstance(self, MutableOrientedSimilaritySurface):
+                    tester.assertEqual(self, copy)
+                    tester.assertFalse(self != copy)
                 else:
-                    el = edge_labels[e]
-                plt += gp.plot_edge_label(e, el, **o)
-        return plt
-
-# I'm not sure we want to support this...
-#
-#    def minimize_monodromy_mapping(self):
-#        r"""
-#        Return a mapping from this surface to a similarity surface
-#        with a minimal monodromy group.
-#        Note that this may be slow for infinite surfaces.
-#
-#        EXAMPLES::
-#            sage: from flatsurf.geometry.polygon import ConvexPolygons
-#            sage: K.<sqrt2> = NumberField(x**2 - 2, embedding=1.414)
-#            sage: octagon = ConvexPolygons(K)([(1,0),(sqrt2/2, sqrt2/2),(0, 1),(-sqrt2/2, sqrt2/2),(-1,0),(-sqrt2/2, -sqrt2/2),(0, -1),(sqrt2/2, -sqrt2/2)])
-#            sage: square = ConvexPolygons(K)([(1,0),(0,1),(-1,0),(0,-1)])
-#            sage: gluings = [((0,i),(1+(i%2),i//2)) for i in range(8)]
-#            sage: from flatsurf.geometry.surface import surface_from_polygons_and_gluings
-#            sage: s=surface_from_polygons_and_gluings([octagon,square,square],gluings)
-#            sage: print s
-#            Rational cone surface built from 3 polygons
-#            sage: m=s.minimize_monodromy_mapping()
-#            sage: s2=m.codomain()
-#            sage: print s2
-#            Translation surface built from 3 polygons
-#            sage: v=s.tangent_vector(2,(0,0),(1,0))
-#            sage: print m.push_vector_forward(v)
-#            SimilaritySurfaceTangentVector in polygon 2 based at (0, 0) with vector (-1/2*sqrt2, -1/2*sqrt2)
-#            sage: w=s2.tangent_vector(2,(0,0),(0,-1))
-#            sage: print m.pull_vector_back(w)
-#            SimilaritySurfaceTangentVector in polygon 2 based at (0, 0) with vector (1/2*sqrt2, 1/2*sqrt2)
-#        """
-#        lw = self.walker()
-#        class MatrixFunction:
-#            def __init__(self, lw):
-#                self._lw=lw
-#                from sage.matrix.constructor import identity_matrix
-#                self._d = {lw.surface().base_label():
-#                    identity_matrix(lw.surface().base_ring(), n=2)}
-#            def __call__(self, label):
-#                try:
-#                    return self._d[label]
-#                except KeyError:
-#                    e = self._lw.edge_back(label)
-#                    label2,e2 = self._lw.surface().opposite_edge(label,e)
-#                    m=self._lw.surface().edge_matrix(label,e) * self(label2)
-#                    self._d[label]=m
-#                    return m
-#        mf = MatrixFunction(lw)
-#        from flatsurf.geometry.mappings import (
-#            MatrixListDeformedSurfaceMapping,
-#            IdentityMapping)
-#        mapping = MatrixListDeformedSurfaceMapping(self, mf)
-#        surface_type = mapping.codomain().compute_surface_type_from_gluings(limit=100)
-#        new_codomain = convert_to_type(mapping.codomain(),surface_type)
-#        identity = IdentityMapping(mapping.codomain(), new_codomain)
-#        return identity * mapping
-#
-#    def minimal_monodromy_surface(self):
-#        r"""
-#        Return an equivalent similarity surface with minimal monodromy.
-#        Note that this may be slow for infinite surfaces.
-#
-#        EXAMPLES::
-#            sage: from flatsurf.geometry.polygon import ConvexPolygons
-#            sage: K.<sqrt2> = NumberField(x**2 - 2, embedding=1.414)
-#            sage: octagon = ConvexPolygons(K)([(1,0),(sqrt2/2, sqrt2/2),(0, 1),(-sqrt2/2, sqrt2/2),(-1,0),(-sqrt2/2, -sqrt2/2),(0, -1),(sqrt2/2, -sqrt2/2)])
-#            sage: square = ConvexPolygons(K)([(1,0),(0,1),(-1,0),(0,-1)])
-#            sage: gluings = [((0,i),(1+(i%2),i//2)) for i in range(8)]
-#            sage: from flatsurf.geometry.surface import surface_from_polygons_and_gluings
-#            sage: s=surface_from_polygons_and_gluings([octagon,square,square],gluings)
-#            sage: print s
-#            Rational cone surface built from 3 polygons
-#            sage: s2=s.minimal_monodromy_surface()
-#            sage: print s2
-#            Translation surface built from 3 polygons
-#        """
-#        return self.minimize_monodromy_mapping().codomain()
+                    tester.assertNotEqual(self, copy)
+                    tester.assertTrue(self != copy)
 
-    def __eq__(self, other):
-        r"""
-        Implements a naive notion of equality where two finite surfaces are equal if:
-        - their base labels are equal,
-        - their polygons are equal and labeled and glued in the same way.
-        For infinite surfaces we use reference equality.
-        Raises a value error if the surfaces are defined over different rings.
-        """
-        if not self.is_finite():
-            return self is other
-        if self is other:
-            return True
-        if not isinstance(other, SimilaritySurface):
-            raise TypeError
-        if not other.is_finite():
-            raise ValueError("Can not compare infinite surfaces.")
-        if self.base_ring() != other.base_ring():
-            raise ValueError("Refusing to compare surfaces with different base rings.")
-        if not self.is_mutable() and not other.is_mutable():
-            hash1 = hash(self)
-            hash2 = hash(other)
-            if hash1 != hash2:
-                return False
-        if self.base_label() != other.base_label():
-            return False
-        if self.num_polygons() != other.num_polygons():
-            return False
-        for label,polygon in self.label_iterator(polygons=True):
-            try:
-                polygon2 = other.polygon(label)
-            except ValueError:
-                return False
-            if polygon != polygon2:
-                return False
-            for edge in range(polygon.num_edges()):
-                if self.opposite_edge(label,edge) != other.opposite_edge(label,edge):
-                    return False
-        return True
-
-    def __ne__(self, other):
-        return not self == other
+        class Oriented(SurfaceCategoryWithAxiom):
+            r"""
+            The category of surfaces built from finitely many Euclidean
+            polygons glued with singularities with an orientation that is
+            compatible with the embedding that the polygons inherit from the
+            real plane.
+
+            EXAMPLES::
+
+                sage: from flatsurf import Polygon, similarity_surfaces
+                sage: P = Polygon(vertices=[(0,0), (1,0), (1,1), (0,1)])
+                sage: S = similarity_surfaces.self_glued_polygon(P)
+                sage: "Oriented" in S.category().axioms()
+                True
+
+            """
+
+            class ParentMethods:
+                r"""
+                Provides methods available to all surfaces that are built from
+                finitely many Euclidean polygons that are glued by similarities
+                and are oriented with the natural orientation of the polygons
+                in the real plane.
+
+                If you want to add functionality for such surfaces you most likely
+                want to put it here.
+                """
+
+                def reposition_polygons(self, in_place=False, relabel=None):
+                    r"""
+                    We choose a maximal tree in the dual graph of the decomposition into
+                    polygons, and ensure that the gluings between two polygons joined by
+                    an edge in this tree is by translation.
+
+                    This guarantees that the group generated by the edge identifications is
+                    minimal among representations of the surface. In particular, if for instance
+                    you have a translation surface which is anot representable as a translation
+                    surface (because polygons are presented with rotations) then after this
+                    change it will be representable as a translation surface.
+                    """
+                    if in_place:
+                        raise NotImplementedError(
+                            "this surface does not implement reposition_polygons(in_place=True) yet"
+                        )
+
+                    from flatsurf.geometry.surface import (
+                        MutableOrientedSimilaritySurface,
+                    )
+
+                    s = MutableOrientedSimilaritySurface.from_surface(self)
+                    s.reposition_polygons(in_place=True, relabel=relabel)
+                    s.set_immutable()
+                    return s
 
-    def __hash__(self):
-        r"""
-        Hash compatible with equals.
-        """
-        if self._s.is_mutable():
-            raise ValueError("Attempting to hash with mutable underlying surface.")
-        if hasattr(self, '_hash'):
-            # Return the cached hash.
-            return self._hash
-        # Compute the hash
-        h = 17*hash(self.base_ring())+23*hash(self.base_label())
-        for pair in self.label_iterator(polygons=True):
-            h = h + 7*hash(pair)
-        for edgepair in self.edge_iterator(gluings=True):
-            h = h + 3*hash(edgepair)
-        self._hash=h
-        return h
+                def standardize_polygons(self, in_place=False):
+                    r"""
+                    Return a surface with each polygon replaced with a new
+                    polygon which differs by translation and reindexing. The
+                    new polygon will have the property that vertex zero is the
+                    origin, and all vertices lie either in the upper half
+                    plane, or on the x-axis with non-negative x-coordinate.
+
+                    EXAMPLES::
+
+                        sage: from flatsurf import translation_surfaces
+                        sage: s=translation_surfaces.veech_double_n_gon(4)
+                        sage: s.polygon(1)
+                        Polygon(vertices=[(0, 0), (-1, 0), (-1, -1), (0, -1)])
+                        sage: [s.opposite_edge(0,i) for i in range(4)]
+                        [(1, 0), (1, 1), (1, 2), (1, 3)]
+                        sage: ss=s.standardize_polygons()
+                        sage: ss.polygon(1)
+                        Polygon(vertices=[(0, 0), (1, 0), (1, 1), (0, 1)])
+                        sage: [ss.opposite_edge(0,i) for i in range(4)]
+                        [(1, 2), (1, 3), (1, 0), (1, 1)]
+                        sage: TestSuite(ss).run()
+
+                    """
+                    if in_place:
+                        raise NotImplementedError(
+                            "cannot standardize polygons in_place anymore on this surface; use in_place=False to create a copy of the surface with standardized polygons"
+                        )
+
+                    from flatsurf.geometry.surface import (
+                        MutableOrientedSimilaritySurface,
+                    )
+
+                    S = MutableOrientedSimilaritySurface.from_surface(
+                        self, category=self.category()
+                    )
+                    S.standardize_polygons(in_place=True)
+                    S.set_immutable()
+                    return S
+
+                def fundamental_group(self, base_label=None):
+                    r"""
+                    Return the fundamental group of this surface.
+                    """
+                    if base_label is None:
+                        base_label = self.root()
+
+                    from flatsurf.geometry.fundamental_group import FundamentalGroup
+
+                    return FundamentalGroup(self, base_label)
+
+    class SubcategoryMethods:
+        def Rational(self):
+            r"""
+            Return the subcategory of surfaces with rational monodromy, see
+            :class:`~.SimilaritySurfaces.Rational`.
+
+            EXAMPLES::
+
+                sage: from flatsurf.geometry.categories import SimilaritySurfaces
+                sage: C = SimilaritySurfaces()
+                sage: C.Rational()
+                Category of rational similarity surfaces
+
+            """
+            return self._with_axiom("Rational")
+
+
+# Currently, there is no "Rational" axiom in SageMath so we make it known to
+# the category framework.
+all_axioms += ("Rational",)
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/similarity_surface_generators.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/surface_objects.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1491 +1,1476 @@
-# -*- coding: utf-8 -*-
-#*********************************************************************
+r"""
+Geometric objects on surfaces.
+
+This includes singularities, saddle connections and cylinders.
+"""
+# ****************************************************************************
 #  This file is part of sage-flatsurf.
 #
-#        Copyright (C) 2016-2020 Vincent Delecroix
-#                      2020      Julian Rüth
+#        Copyright (C) 2017-2020 W. Patrick Hooper
+#                      2017-2020 Vincent Delecroix
+#                           2023 Julian Rüth
 #
 #  sage-flatsurf is free software: you can redistribute it and/or modify
 #  it under the terms of the GNU General Public License as published by
 #  the Free Software Foundation, either version 2 of the License, or
 #  (at your option) any later version.
 #
 #  sage-flatsurf is distributed in the hope that it will be useful,
 #  but WITHOUT ANY WARRANTY; without even the implied warranty of
 #  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
-#*********************************************************************
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
-from six import iteritems, itervalues
-
-from sage.rings.all import ZZ, QQ, RIF, AA, NumberField, polygen
-from sage.modules.all import VectorSpace, vector
-from sage.structure.coerce import py_scalar_parent
-from sage.structure.element import get_coercion_model, parent
-from sage.misc.cachefunc import cached_method
-from sage.structure.sequence import Sequence
-
-ZZ_1 = ZZ(1)
-ZZ_2 = ZZ(2)
+# ****************************************************************************
 
-from .polygon import polygons, ConvexPolygons, Polygon, ConvexPolygon, build_faces
+from sage.misc.cachefunc import cached_method
+from sage.modules.free_module_element import vector
+from sage.plot.graphics import Graphics
+from sage.plot.polygon import polygon2d
+from sage.rings.qqbar import AA
+from sage.structure.sage_object import SageObject
+from sage.structure.element import Element
 
-from .surface import Surface, Surface_list
-from .translation_surface import TranslationSurface
-from .dilation_surface import DilationSurface
-from .similarity_surface import SimilaritySurface
-from .half_translation_surface import HalfTranslationSurface
-from .cone_surface import ConeSurface
-from .rational_cone_surface import RationalConeSurface
+from flatsurf.geometry.similarity import SimilarityGroup
 
 
-def flipper_nf_to_sage(K, name='a'):
+def Singularity(similarity_surface, label, v, limit=None):
     r"""
-    Convert a flipper number field into a Sage number field
-
-    .. NOTE::
+    Return the point of ``similarity_surface`` at the ``v``-th vertex of the
+    polygon ``label``.
 
-        Currently, the code is not careful at all with root isolation.
+    If the surface is infinite, the ``limit`` can be set. In this case the
+    construction of the singularity is successful if the sequence of vertices
+    hit by passing through edges closes up in ``limit`` or less steps.
 
     EXAMPLES::
 
-        sage: import flipper  # optional - flipper
-        sage: import realalg  # optional - flipper
-        sage: from flatsurf.geometry.similarity_surface_generators import flipper_nf_to_sage
-        sage: K = realalg.RealNumberField([-2r] + [0r]*5 + [1r])   # optional - flipper
-        sage: K_sage = flipper_nf_to_sage(K)                       # optional - flipper
-        sage: K_sage                                               # optional - flipper
-        Number Field in a with defining polynomial x^6 - 2 with a = 1.122462048309373?
-        sage: AA(K_sage.gen())                                     # optional - flipper
-        1.122462048309373?
+        sage: from flatsurf.geometry.similarity_surface_generators import TranslationSurfaceGenerators
+        sage: s=TranslationSurfaceGenerators.veech_2n_gon(5)
+        sage: from flatsurf.geometry.surface_objects import Singularity
+        sage: sing=Singularity(s, 0, 1)
+        doctest:warning
+        ...
+        UserWarning: Singularity() is deprecated and will be removed in a future version of sage-flatsurf. Use surface.point() instead.
+        sage: print(sing)
+        Vertex 1 of polygon 0
+        sage: TestSuite(sing).run()
+
     """
-    r = K.lmbda.interval()
-    l = r.lower * ZZ(10)**(-r.precision)
-    u = r.upper * ZZ(10)**(-r.precision)
-
-    p = QQ['x'](K.coefficients)
-    s = AA.polynomial_root(p, RIF(l,u))
-    return NumberField(p, name, embedding=s)
+    import warnings
+
+    warnings.warn(
+        "Singularity() is deprecated and will be removed in a future version of sage-flatsurf. Use surface.point() instead."
+    )
+    return similarity_surface.point(
+        label, similarity_surface.polygon(label).vertex(v), limit=limit
+    )
 
-def flipper_nf_element_to_sage(x, K=None):
+
+class SurfacePoint(Element):
     r"""
-    Convert a flipper number field element into Sage
+    A point on ``surface``.
 
-    EXAMPLES::
+    INPUT:
 
-        sage: from flatsurf.geometry.similarity_surface_generators import flipper_nf_element_to_sage
-        sage: import flipper                               # optional - flipper
-        sage: T = flipper.load('SB_6')                     # optional - flipper
-        sage: h = T.mapping_class('s_0S_1S_2s_3s_4s_3S_5') # optional - flipper
-        sage: flipper_nf_element_to_sage(h.dilatation())   # optional - flipper
-        a
-        sage: AA(_)                                        # optional - flipper
-        6.45052513748511?
-    """
-    if K is None:
-        K = flipper_nf_to_sage(x.field)
-    coeffs = list(map(QQ, x.coefficients))
-    coeffs.extend([0] * (K.degree() - len(coeffs)))
-    return K(coeffs)
+    - ``surface`` -- a similarity surface
 
-class EInfinitySurface(Surface):
-    r"""
-    The surface based on the $E_\infinity$ graph.
+    - ``label`` -- a polygon label for the polygon with respect to which the
+      ``point`` coordinates can be made sense of
 
-     The biparite graph is shown below, with edges numbered:
+    - ``point`` -- coordinates of a point in the polygon ``label`` or the index
+      of the vertex of the polygon with ``label``
 
-      0   1   2  -2   3  -3   4  -4
-    *---o---*---o---*---o---*---o---*...
-            |
-            |-1
-            o
-
-    Here, black vertices are colored *, and white o.
-    Black nodes represent vertical cylinders and white nodes
-    represent horizontal cylinders.
-    """
-    def __init__(self,lambda_squared=None, field=None):
-        if lambda_squared==None:
-            from sage.rings.polynomial.polynomial_ring_constructor import PolynomialRing
-            R=PolynomialRing(ZZ,'x')
-            x = R.gen()
-            field=NumberField(x**3-ZZ(5)*x**2+ZZ(4)*x-ZZ(1), 'r', embedding=AA(ZZ(4)))
-            self._l=field.gen()
-        else:
-            if field is None:
-                self._l=lambda_squared
-                field=lambda_squared.parent()
-            else:
-                self._l=field(lambda_squared)
-        super().__init__(field, ZZ.zero(), finite=False, mutable=False)
+    - ``ring`` -- a SageMath ring or ``None`` (default: ``None``); the
+      coordinate ring for ``point``
 
-    def _repr_(self):
-        r"""
-        String representation.
-        """
-        return "The E-infinity surface"
+    - ``limit`` -- an integer or ``None`` (default: ``None`` for an unlimited
+      number of steps); if this is a singularity of the surface, then this
+      limits the number of edges that are crossed to determine all the edges
+      adjacent to that singularity. An error is raised if the limit is
+      insufficient.
 
-    @cached_method
-    def get_white(self,n):
-        r"""Get the weight of the white endpoint of edge n."""
-        l=self._l
-        if n==0 or n==1:
-            return l
-        if n==-1:
-            return l-1
-        if n==2:
-            return 1-3*l+l**2
-        if n>2:
-            x=self.get_white(n-1)
-            y=self.get_black(n)
-            return l*y-x
-        return self.get_white(-n)
+    EXAMPLES::
 
-    @cached_method
-    def get_black(self,n):
-        r"""Get the weight of the black endpoint of edge n."""
-        l=self._l
-        if n==0:
-            return self.base_ring().one()
-        if n==1 or n==-1 or n==2:
-            return l-1
-        if n>2:
-            x=self.get_black(n-1)
-            y=self.get_white(n-1)
-            return y-x
-        return self.get_black(1-n)
-
-    def polygon(self, lab):
-        r"""
-        Return the polygon labeled by ``lab``.
-        """
-        if lab not in self.polygon_labels():
-            raise ValueError("lab (=%s) not a valid label"%lab)
-        return polygons.rectangle(2*self.get_black(lab),self.get_white(lab))
-
-    def polygon_labels(self):
-        r"""
-        The set of labels used for the polygons.
-        """
-        return ZZ
-
-    def opposite_edge(self, p, e):
-        r"""
-        Return the pair ``(pp,ee)`` to which the edge ``(p,e)`` is glued to.
-        """
-        if p==0:
-            if e==0:
-                return (0,2)
-            if e==1:
-                return (1,3)
-            if e==2:
-                return (0,0)
-            if e==3:
-                return (1,1)
-        if p==1:
-            if e==0:
-                return (-1,2)
-            if e==1:
-                return (0,3)
-            if e==2:
-                return (2,0)
-            if e==3:
-                return (0,1)
-        if p==-1:
-            if e==0:
-                return (2,2)
-            if e==1:
-                return (-1,3)
-            if e==2:
-                return (1,0)
-            if e==3:
-                return (-1,1)
-        if p==2:
-            if e==0:
-                return (1,2)
-            if e==1:
-                return (-2,3)
-            if e==2:
-                return (-1,0)
-            if e==3:
-                return (-2,1)
-        if p>2:
-            if e%2:
-                return -p,(e+2)%4
-            else:
-                return 1-p,(e+2)%4
-        else:
-            if e%2:
-                return -p,(e+2)%4
-            else:
-                return 1-p,(e+2)%4
+        sage: from flatsurf import translation_surfaces
 
-class TFractalSurface(Surface):
-    r"""
-    The TFractal surface.
+        sage: permutation = SymmetricGroup(2)('(1, 2)')
+        sage: S = translation_surfaces.origami(permutation, permutation)
+
+    A point can have a single representation with coordinates when it is in
+    interior of a polygon::
+
+        sage: S.point(1, (1/2, 1/2))
+        Point (1/2, 1/2) of polygon 1
+
+    A point can have two representations when it is in interior of an edge::
 
-    The TFractal surface is a translation surface of finite area built from
-    infinitely many polygons. The basic building block is the following polygon
+        sage: p = S.point(1, (1/2, 0))
+        sage: q = S.point(2, (1/2, 1))
+        sage: p == q
+        True
+        sage: p.coordinates(2)
+        ((1/2, 1),)
 
-     w/r    w     w/r
-    +---+------+---+
-    | 1 |   2  | 3 | h2
-    +---+------+---+
-        |   0  | h1
-        +------+
-            w
-
-    where ``w``, ``h1``, ``h2``, ``r`` are some positive numbers. Default values
-    are ``w=h1=h2=1`` and ``r=2``.
-
-    .. TODO::
-
-        In that surface, the linear flow can be computed more efficiently using
-        only one affine interval exchange transformation with 5 intervals. But
-        the underlying geometric construction is not a covering.
+    A point can have even more representations when it is a vertex::
+
+        sage: S.point(1, (0, 0))
+        Vertex 0 of polygon 1
 
-        Warning: we can not play at the same time with tuples and element of a
-        cartesian product (see Sage trac ticket #19555)
     """
-    def __init__(self, w=ZZ_1, r=ZZ_2, h1=ZZ_1, h2=ZZ_1):
-        from sage.combinat.words.words import Words
 
-        field = Sequence([w,r,h1,h2]).universe()
-        if not field.is_field():
-            field = field.fraction_field()
-        self._w = field(w)
-        self._r = field(r)
-        self._h1 = field(h1)
-        self._h2 = field(h2)
-        self._words = Words('LR', finite=True, infinite=False)
-        self._wL = self._words('L')
-        self._wR = self._words('R')
-
-        base_label=self.polygon_labels()._cartesian_product_of_elements((self._words(''), 0))
-
-        super().__init__(field, base_label, finite=False, mutable=False)
-
-    def _repr_(self):
-        return "The T-fractal surface with parameters w=%s, r=%s, h1=%s, h2=%s"%(
-                self._w, self._r, self._h1, self._h2)
+    def __init__(self, surface, label, point, ring=None, limit=None):
+        self._surface = surface
 
-    @cached_method
-    def polygon_labels(self):
-        from sage.sets.finite_enumerated_set import FiniteEnumeratedSet
-        from sage.categories.cartesian_product import cartesian_product
-        return cartesian_product([self._words, FiniteEnumeratedSet([0,1,2,3])])
-
-    def opposite_edge(self, p, e):
-        r"""
-
-        Labeling of polygons
-
-         wl,0             wr,0
-        +-----+---------+------+
-        |     |         |      |
-        | w,1 |   w,2   |  w,3 |
-        |     |         |      |
-        +-----+---------+------+
-              |         |
-              |   w,0   |
-              |         |
-              +---------+
-                   w
+        if ring is None:
+            ring = surface.base_ring()
 
-        and we always have: bot->0, right->1, top->2, left->3
+        if ring is not surface.base_ring():
+            import warnings
 
-        EXAMPLES::
+            warnings.warn(
+                "the ring parameter is deprecated and will be removed in a future version of sage-flatsurf; define the surface over a larger ring instead so that this points' coordinates live in the base ring"
+            )
 
-            sage: import flatsurf.geometry.similarity_surface_generators as sfg
-            sage: T = sfg.tfractal_surface()
-            sage: W = T.underlying_surface()._words
-            sage: w = W('LLRLRL')
-            sage: T.opposite_edge((w,0),0)
-            ((word: LLRLR, 1), 2)
-            sage: T.opposite_edge((w,0),1)
-            ((word: LLRLRL, 0), 3)
-            sage: T.opposite_edge((w,0),2)
-            ((word: LLRLRL, 2), 0)
-            sage: T.opposite_edge((w,0),3)
-            ((word: LLRLRL, 0), 1)
-        """
-        w,i = p
-        w = self._words(w)
-        i = int(i)
-        e = int(e)
-
-        if e==0: f=2
-        elif e==1: f=3
-        elif e==2: f=0
-        elif e==3: f=1
-        else:
-            raise ValueError("e (={!r}) must be either 0,1,2 or 3".format(e))
+        polygon = surface.polygon(label)
+
+        from sage.all import ZZ
+
+        if point in ZZ:
+            point = surface.polygon(label).vertex(point)
+
+        point = (ring**2)(point)
+        point.set_immutable()
 
-        if i == 0:
-            if e == 0:
-                if w.is_empty():   lab=(w,2)
-                elif w[-1] == 'L': lab=(w[:-1],1)
-                elif w[-1] == 'R': lab=(w[:-1],3)
-            if e == 1: lab=(w,0)
-            if e == 2: lab=(w,2)
-            if e == 3: lab=(w,0)
-        elif i == 1:
-            if e == 0: lab=(w + self._wL, 2)
-            if e == 1: lab=(w,2)
-            if e == 2: lab=(w + self._wL, 0)
-            if e == 3: lab=(w,3)
-        elif i == 2:
-            if e == 0: lab=(w,0)
-            if e == 1: lab=(w,3)
-            if e == 2:
-                if w.is_empty():   lab=(w,0)
-                elif w[-1] == 'L': lab=(w[:-1],1)
-                elif w[-1] == 'R': lab=(w[:-1],3)
-            if e == 3: lab=(w,1)
-        elif i == 3:
-            if e == 0: lab=(w + self._wR, 2)
-            if e == 1: lab=(w,1)
-            if e == 2: lab=(w + self._wR, 0)
-            if e == 3: lab=(w,2)
+        position = polygon.get_point_position(point)
+
+        if not position.is_inside():
+            raise NotImplementedError(
+                "point must be positioned within the polygon with the given label"
+            )
+
+        if position.is_in_interior():
+            self._representatives = {(label, point)}
+        elif position.is_in_edge_interior():
+            self._representatives = {(label, point)}
+
+            cross_label, cross_edge = surface.opposite_edge(label, position.get_edge())
+            cross_point = surface.edge_transformation(label, position.get_edge())(point)
+            cross_point.set_immutable()
+
+            self._representatives.add((cross_label, cross_point))
+        elif position.is_vertex():
+            self._representatives = set()
+
+            source_edge = position.get_vertex()
+            while (label, source_edge) not in self._representatives:
+                self._representatives.add((label, source_edge))
+
+                # Rotate to the next edge that is leaving at the vertex
+                label, source_edge = surface.opposite_edge(label, source_edge)
+                source_edge = (source_edge + 1) % len(surface.polygon(label).vertices())
+
+                if limit is not None:
+                    limit -= 1
+                    if limit < 0:
+                        raise ValueError("number of edges at singularity exceeds limit")
+
+            self._representatives = {
+                (label, surface.polygon(label).vertex(vertex))
+                for (label, vertex) in self._representatives
+            }
         else:
-            raise ValueError("i (={!r}) must be either 0,1,2 or 3".format(i))
+            raise NotImplementedError
 
-        # the fastest label constructor
-        lab = self.polygon_labels()._cartesian_product_of_elements(lab)
-        return lab,f
-
-    def polygon(self, lab):
-        r"""
-        Return the polygon with label ``lab``.
-         w/r         w/r
-        +---+------+---+
-        | 1 |  2   | 3 |
-        |   |      |   |  h2
-        +---+------+---+
-            |  0   | h1
-            +------+
-            w
+        self._representatives = frozenset(self._representatives)
+
+        super().__init__(surface)
+
+    def surface(self):
+        r"""
+        Return the surface containing this point.
 
         EXAMPLES::
 
-            sage: import flatsurf.geometry.similarity_surface_generators as sfg
-            sage: T = sfg.tfractal_surface()
-            sage: T.polygon(('L',0))
-            Polygon: (0, 0), (1/2, 0), (1/2, 1/2), (0, 1/2)
-            sage: T.polygon(('LRL',0))
-            Polygon: (0, 0), (1/8, 0), (1/8, 1/8), (0, 1/8)
+            sage: from flatsurf import translation_surfaces
+
+            sage: permutation = SymmetricGroup(2)('(1, 2)')
+            sage: S = translation_surfaces.origami(permutation, permutation)
+            sage: p = S.point(1, (1/2, 1/2))
+            sage: p.surface() is S
+            True
+
         """
-        w = self._words(lab[0])
-        return (1 / self._r ** w.length()) * self._base_polygon(lab[1])
+        return self._surface
 
-    @cached_method
-    def _base_polygon(self, i):
-        if i == 0:
-            w = self._w
-            h = self._h1
-        if i == 1 or i == 3:
-            w = self._w / self._r
-            h = self._h2
-        if i == 2:
-            w = self._w
-            h = self._h2
-        return ConvexPolygons(self.base_ring())([(w,0),(0,h),(-w,0),(0,-h)])
+    def is_vertex(self):
+        r"""
+        Return whether this point is a singularity of the surface.
+
+        EXAMPLES::
 
-def tfractal_surface(w=ZZ_1, r=ZZ_2, h1=ZZ_1, h2=ZZ_1):
-    return TranslationSurface(TFractalSurface(w,r,h1,h2))
+            sage: from flatsurf import translation_surfaces
 
-class SimilaritySurfaceGenerators:
-    r"""
-    Examples of similarity surfaces.
-    """
-    @staticmethod
-    def example():
+            sage: permutation = SymmetricGroup(2)('(1, 2)')
+            sage: S = translation_surfaces.origami(permutation, permutation)
+            sage: p = S.point(1, (0, 0))
+
+            sage: p.is_vertex()
+            True
+
+        """
+        label, coordinates = self.representative()
+        position = self.surface().polygon(label).get_point_position(coordinates)
+        return position.is_vertex()
+
+    def one_vertex(self):
         r"""
-        Construct a SimilaritySurface from a pair of triangles.
+        Return a pair (l, v) from the equivalence class of this singularity.
 
-        TESTS::
+        EXAMPLES::
+
+            sage: from flatsurf import translation_surfaces
 
-            sage: from flatsurf import *
-            sage: ex = similarity_surfaces.example()
-            sage: ex
-            SimilaritySurface built from 2 polygons
-            sage: TestSuite(ex).run()
-        """
-        s = Surface_list(base_ring=QQ)
-        s.add_polygon(polygons(vertices=[(0,0), (2,-2), (2,0)],ring=QQ)) # gets label 0
-        s.add_polygon(polygons(vertices=[(0,0), (2,0), (1,3)],ring=QQ)) # gets label 1
-        s.change_polygon_gluings(0, [(1,1), (1,2), (1,0)])
-        s.set_immutable()
-        return SimilaritySurface(s)
+            sage: permutation = SymmetricGroup(2)('(1, 2)')
+            sage: S = translation_surfaces.origami(permutation, permutation)
+            sage: p = S.point(1, (0, 0))
+            sage: p.one_vertex()  # random output: depends on the Python version
+            doctest:warning
+            ...
+            UserWarning: one_vertex() is deprecated and will be removed in a future version of sage-flatsurf; use (label, coordinates) = point.representative(); vertex = surface.polygon(label).get_point_position(coordinates).get_vertex() instead
+            (2, 1)
+
+        """
+        import warnings
+
+        warnings.warn(
+            "one_vertex() is deprecated and will be removed in a future version of sage-flatsurf; use (label, coordinates) = point.representative(); vertex = surface.polygon(label).get_point_position(coordinates).get_vertex() instead"
+        )
+        label, coordinates = self.representative()
+        vertex = (
+            self.surface().polygon(label).get_point_position(coordinates).get_vertex()
+        )
+        return label, vertex
 
-    @staticmethod
-    def self_glued_polygon(P):
+    def representatives(self):
         r"""
-        Return the HalfTranslationSurface formed by gluing all edges of P to themselves.
+        Return the representatives of this point as pairs of polygon labels and
+        coordinates.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
-            sage: p = polygons((2,0),(-1,3),(-1,-3))
-            sage: s = similarity_surfaces.self_glued_polygon(p)
-            sage: TestSuite(s).run()
+            sage: from flatsurf import translation_surfaces
+
+            sage: permutation = SymmetricGroup(2)('(1, 2)')
+            sage: S = translation_surfaces.origami(permutation, permutation)
+            sage: p = S.point(1, (0, 0))
+            sage: p.representatives()
+            frozenset({(1, (0, 0)), (1, (1, 1)), (2, (0, 1)), (2, (1, 0))})
+
         """
-        s = Surface_list(base_ring=P.base_ring(), mutable=True)
-        s.add_polygon(P,[(0,i) for i in range(P.num_edges())])
-        s.set_immutable()
-        return HalfTranslationSurface(s)
+        return self._representatives
 
-    @staticmethod
-    def billiard(P, rational=False):
+    def representative(self):
         r"""
-        Return the ConeSurface associated to the billiard in the polygon ``P``.
+        Return a representative of this point, i.e., the first of
+        :meth:`representatives`.
+
+        EXAMPLES::
+
+            sage: from flatsurf import translation_surfaces
 
-        INPUT:
+            sage: permutation = SymmetricGroup(2)('(1, 2)')
+            sage: S = translation_surfaces.origami(permutation, permutation)
+            sage: p = S.point(1, (0, 0))
+            sage: p.representative()  # random output: depends on the Python version
+            (2, (1, 0))
 
-        - ``P`` - a polygon
+        """
+        return next(iter(self.representatives()))
 
-        - ``rational`` (boolean, default ``False``) - whether to assume that the polygon
-          has all its angle rational multiple of pi.
+    def vertex_set(self):
+        r"""
+        Return the list of pairs (l, v) in the equivalence class of this singularity.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
 
-            sage: P = polygons(vertices=[(0,0), (1,0), (0,1)])
-            sage: from flatsurf.geometry.rational_cone_surface import RationalConeSurface
-            sage: Q = similarity_surfaces.billiard(P, rational=True)
-            sage: Q
-            RationalConeSurface built from 2 polygons
-            sage: M = Q.minimal_cover(cover_type="translation")
-            sage: M
-            TranslationSurface built from 8 polygons
-            sage: TestSuite(M).run()
-
-        A non-convex examples (L-shape polygon)::
-
-            sage: P = polygons(vertices=[(0,0), (2,0), (2,1), (1,1), (1,2), (0,2)], convex=False)
-            sage: Q = similarity_surfaces.billiard(P, rational=True)
-            sage: TestSuite(Q).run()
-            sage: M = Q.minimal_cover(cover_type="translation")
-            sage: TestSuite(M).run()
-            sage: M.stratum()
-            H_2(2, 0^5)
-
-        A quadrilateral from Eskin-McMullen-Mukamel-Wright::
-
-            sage: E = EquiangularPolygons(1, 1, 1, 7)
-            sage: P = E.an_element()
-            sage: S = similarity_surfaces.billiard(P)
-            sage: TestSuite(S).run()
-            sage: S = S.minimal_cover(cover_type="translation")
-            sage: TestSuite(S).run()
-            sage: S = S.erase_marked_points() # optional: pyflatsurf
-            sage: TestSuite(S).run()
-            sage: S, _ = S.normalized_coordinates()
-            sage: TestSuite(S).run()
-
-        Unfolding a triangle with non-algebraic lengths::
-
-            sage: E = EquiangularPolygons(3, 3, 5)
-            sage: from pyexactreal import ExactReals # optional: exactreal
-            sage: R = ExactReals(E.base_ring()) # optional: exactreal
-            sage: P = E(R.random_element()) # optional: exactreal
-            sage: S = similarity_surfaces.billiard(P); S # optional: exactreal
-            ConeSurface built from 2 polygons
-            sage: TestSuite(S).run() # long time (6s), optional: exactreal
-
-        """
-        if not isinstance(P, Polygon):
-            raise TypeError("invalid input")
-
-        V = P.module()
-
-        if not isinstance(P, ConvexPolygon):
-            # triangulate non-convex ones
-            base_ring = P.base_ring()
-            C = ConvexPolygons(base_ring)
-            comb_edges = P.triangulation()
-            vertices = P.vertices()
-            comb_triangles = build_faces(len(vertices), comb_edges)
-            triangles = []
-            internal_edges = []  # list (p1, e1, p2, e2)
-            external_edges = []  # list (p1, e1)
-            edge_to_lab = {}
-            for num,(i,j,k) in enumerate(comb_triangles):
-                triangles.append(C(vertices=[vertices[i], vertices[j], vertices[k]]))
-                edge_to_lab[(i,j)] = (num, 0)
-                edge_to_lab[(j,k)] = (num, 1)
-                edge_to_lab[(k,i)] = (num, 2)
-            for num,(i,j,k) in enumerate(comb_triangles):
-                if (j, i) in edge_to_lab:
-                    num2, e2 = edge_to_lab[j, i]
-                    internal_edges.append((num, 0, num2, e2))
-                else:
-                    external_edges.append((num, 0))
-                if (k, j) in edge_to_lab:
-                    num2, e2 = edge_to_lab[k, j]
-                    internal_edges.append((num, 1, num2, e2))
-                else:
-                    external_edges.append((num, 1))
-                if (i, k) in edge_to_lab:
-                    num2, e2 = edge_to_lab[i, k]
-                    internal_edges.append((num, 2, num2, e2))
-                else:
-                    external_edges.append((num, 1))
-            P = triangles
-        else:
-            internal_edges = []
-            external_edges = [(0, i) for i in range(P.num_edges())]
-            base_ring = P.base_ring()
-            P = [P]
-
-        m = len(P)
-        Q = []
-        surface = Surface_list(base_ring=base_ring)
-        for p in P:
-            surface.add_polygon(p)
-        for p in P:
-            surface.add_polygon(polygons(edges=[V((-x,y)) for x,y in reversed(p.edges())]))
-        for (p1,e1,p2,e2) in internal_edges:
-            surface.set_edge_pairing(p1, e1, p2, e2)
-            ne1 = surface.polygon(p1).num_edges()
-            ne2 = surface.polygon(p2).num_edges()
-            surface.set_edge_pairing(m + p1, ne1-e1-1, m + p2, ne2-e2-1)
-        for p, e in external_edges:
-            ne = surface.polygon(p).num_edges()
-            surface.set_edge_pairing(p, e, m+p, ne-e-1)
-
-        surface.set_immutable()
-        if rational:
-            s = RationalConeSurface(surface)
-        else:
-            s = ConeSurface(surface)
-        return s
+            sage: permutation = SymmetricGroup(2)('(1, 2)')
+            sage: S = translation_surfaces.origami(permutation, permutation)
+            sage: p = S.point(1, (0, 0))
+            sage: list(p.vertex_set())  # random output: ordering depends on the Python version
+            doctest:warning
+            ...
+            UserWarning: vertex_set() is deprecated and will be removed in a future version of sage-flatsurf; use representatives() and then vertex = surface.polygon(label).get_point_position(coordinates).get_vertex() instead
+            [(2, 1), (1, 2), (1, 0), (2, 3)]
+
+        """
+        import warnings
+
+        warnings.warn(
+            "vertex_set() is deprecated and will be removed in a future version of sage-flatsurf; use representatives() and then vertex = surface.polygon(label).get_point_position(coordinates).get_vertex() instead"
+        )
 
-    @staticmethod
-    def polygon_double(P):
+        return [
+            (
+                label,
+                self.surface()
+                .polygon(label)
+                .get_point_position(coordinates)
+                .get_vertex(),
+            )
+            for label, coordinates in self.representatives()
+        ]
+
+    def contains_vertex(self, label, v=None):
         r"""
-        Return the ConeSurface associated to the billiard in the polygon ``P``.
-        Differs from billiard(P) only in the graphical display. Here, we display
-        the polygons separately.
-        """
-        from sage.matrix.constructor import matrix
-
-        n = P.num_edges()
-        r = matrix(2, [-1,0,0,1])
-        Q = polygons(edges=[r*v for v in reversed(P.edges())])
-
-        surface = Surface_list(base_ring = P.base_ring())
-        surface.add_polygon(P) # gets label 0)
-        surface.add_polygon(Q) # gets label 1
-        surface.change_polygon_gluings(0,[(1,n-i-1) for i in range(n)])
-        surface.set_immutable()
-        return ConeSurface(surface)
+        Checks if the pair ``(label, v)`` is in the equivalence class returning
+        true or false. If ``v`` is ``None``, the both the pair ``(label, v)``
+        is passed as a single parameter in ``label``.
+
+        EXAMPLES::
+
+            sage: from flatsurf import translation_surfaces
+
+            sage: permutation = SymmetricGroup(2)('(1, 2)')
+            sage: S = translation_surfaces.origami(permutation, permutation)
+            sage: p = S.point(1, (0, 0))
+            sage: p.contains_vertex((1, 0))
+            doctest:warning
+            ...
+            UserWarning: contains_vertex() is deprecated and will be removed in a future version of sage-flatsurf; use the == operator instead
+            doctest:warning
+            ...
+            UserWarning: Singularity() is deprecated and will be removed in a future version of sage-flatsurf. Use surface.point() instead.
+            True
+            sage: p.contains_vertex(label=1, v=0)
+            True
 
-    @staticmethod
-    def right_angle_triangle(w,h):
+        """
+        import warnings
+
+        warnings.warn(
+            "contains_vertex() is deprecated and will be removed in a future version of sage-flatsurf; use the == operator instead"
+        )
+
+        if v is None:
+            label, v = label
+
+        return Singularity(self.surface(), label, v) == self
+
+    def num_coordinates(self):
         r"""
-        TESTS::
+        Return the number of different coordinate representations of the point.
+
+        EXAMPLES::
 
-            sage: from flatsurf import *
-            sage: R = similarity_surfaces.right_angle_triangle(2, 3)
-            sage: R
-            ConeSurface built from 2 polygons
-            sage: TestSuite(R).run()
-        """
-        from sage.modules.free_module_element import vector
-
-        F = Sequence([w,h]).universe()
-
-        if not F.is_field():
-            F = F.fraction_field()
-        V = VectorSpace(F,2)
-        P = ConvexPolygons(F)
-        s = Surface_list(base_ring=F)
-        s.add_polygon(P([V((w,0)),V((-w,h)),V((0,-h))])) # gets label 0
-        s.add_polygon(P([V((0,h)),V((-w,-h)),V((w,0))])) # gets label 1
-        s.change_polygon_gluings(0,[(1,2),(1,1),(1,0)])
-        s.set_immutable()
-        return ConeSurface(s)
-
-    # Removed because Surface_polygons_and_gluings is gone.
-    #
-    #def __call__(self, *args, **kwds):
-    #    from flatsurf.geometry.surface import Surface_polygons_and_gluings
-    #    from flatsurf.geometry.similarity_surface import SimilaritySurface
-    #    return SimilaritySurface(Surface_polygons_and_gluings(*args, **kwds))
-
-similarity_surfaces = SimilaritySurfaceGenerators()
-
-class DilationSurfaceGenerators:
-    @staticmethod
-    def basic_dilation_torus(a):
-        r"""
-        Return a dilation torus built from a $1 \times 1$ square and a $a \times 1$ rectangle.
-        Each edge of the square is glued to the opposite edge of the rectangle. This results
-        in horizontal edges glued by a dilation with a scaling factor of a, and vertical
-        edges being glued by translation.
-
-            b       a
-          +----+---------+
-          | 0  | 1       |
-        c |    |         | c
-          +----+---------+
-            a       b
+            sage: from flatsurf import translation_surfaces
+
+            sage: permutation = SymmetricGroup(2)('(1, 2)')
+            sage: S = translation_surfaces.origami(permutation, permutation)
+            sage: p = S.point(1, (0, 0))
+            sage: p.num_coordinates()
+            doctest:warning
+            ...
+            UserWarning: num_coordinates() is deprecated and will be removed in a future version of sage-flatsurf; use len(representatives()) instead.
+            4
+
+        """
+        import warnings
+
+        warnings.warn(
+            "num_coordinates() is deprecated and will be removed in a future version of sage-flatsurf; use len(representatives()) instead."
+        )
+
+        return len(self._representatives)
+
+    def labels(self):
+        r"""
+        Return the labels of polygons containing the point.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
-            sage: ds = dilation_surfaces.basic_dilation_torus(AA(sqrt(2)))
-            sage: ds
-            DilationSurface built from 2 polygons
-            sage: TestSuite(ds).run()
-        """
-        s = Surface_list(base_ring=a.parent().fraction_field())
-        CP = ConvexPolygons(s.base_ring())
-        s.add_polygon(CP(edges=[(0,1),(-1,0),(0,-1),(1,0)])) # label 0
-        s.add_polygon(CP(edges=[(0,1),(-a,0),(0,-1),(a,0)])) # label 1
-        s.change_edge_gluing(0, 0, 1, 2)
-        s.change_edge_gluing(0, 1, 1, 3)
-        s.change_edge_gluing(0, 2, 1, 0)
-        s.change_edge_gluing(0, 3, 1, 1)
-        s.change_base_label(0)
-        s.set_immutable()
-        return DilationSurface(s)
-
-    @staticmethod
-    def genus_two_square(a, b, c, d):
-        r"""A genus two dilation surface is returned.
-
-        The unit square is made into an octagon by marking a point on
-        each of its edges. Then opposite sides of this octagon are
-        glued together by translation. (Since we currently require strictly
-        convex polygons, we subdivide the square into a hexagon and two
-        triangles as depicted below.) The parameters $a$, $b$, $c$,
-        and $d$ should be real numbers strictly between zero and one.
-        These represent the lengths of an edge of the resulting octagon,
-        as below.
-                 c
-           +--+-------+
-         d |2/        |
-           |/         |
-           +    0     +
-           |         /|
-           |        /1| b
-           +-------+--+
-              a
-        The other edges will have length $1-a$, $1-b$, $1-c$, and $1-d$.
-        Dilations used to glue edges will be by factors $c/a$, $d/b$,
-        $(1-c)/(1-a)$ and $(1-d)/(1-b)$.
+            sage: from flatsurf import translation_surfaces
+            sage: S = translation_surfaces.mcmullen_L(1, 1, 1, 1)
+
+        For a point in the interior of polygon, there is exactly one label::
+
+            sage: p = S.point(0, (1/2, 1/2))
+            sage: p.labels()
+            {0}
+
+        For a point in the interior of an edge of a polygon, there can be up to
+        two labels::
+
+            sage: p = S.point(0, (0, 1/2))
+            sage: p.labels()
+            {0, 2}
+
+        For a point at a vertex, there can be more labels::
+
+            sage: p = S.point(0, (0, 0))
+            sage: p.labels()
+            {0, 1, 2}
+
+        """
+        return set(label for (label, _) in self._representatives)
+
+    def coordinates(self, label):
+        r"""
+        Return coordinates for the point in the in the polygon ``label``.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
-            sage: ds = dilation_surfaces.genus_two_square(1/2, 1/3, 1/4, 1/5)
-            sage: ds
-            DilationSurface built from 3 polygons
-            sage: TestSuite(ds).run()
-        """
-        field = Sequence([a, b, c, d]).universe().fraction_field()
-        s = Surface_list(base_ring=QQ)
-        CP = ConvexPolygons(field)
-        hexagon = CP(edges=[(a,0), (1-a,b), (0,1-b), (-c,0), (c-1,-d), (0,d-1)])
-        s.add_polygon(hexagon) # polygon 0
-        s.change_base_label(0)
-        triangle1 = CP(edges=[(1-a,0), (0,b), (a-1,-b)])
-        s.add_polygon(triangle1) # polygon 1
-        triangle2 = CP(edges=[(1-c,d), (c-1,0), (0,-d)])
-        s.add_polygon(triangle2) # polygon 2
-        s.change_edge_gluing(0, 0, 0, 3)
-        s.change_edge_gluing(0, 2, 0, 5)
-        s.change_edge_gluing(0, 1, 1, 2)
-        s.change_edge_gluing(0, 4, 2, 0)
-        s.change_edge_gluing(1, 0, 2, 1)
-        s.change_edge_gluing(1, 1, 2, 2)
-        s.set_immutable()
-        return DilationSurface(s)
-
-dilation_surfaces = DilationSurfaceGenerators()
-
-class HalfTranslationSurfaceGenerators:
-    # TODO: ideally, we should be able to construct a non-convex polygon and make the construction
-    # below as a special case of billiard unfolding.
-    @staticmethod
-    def step_billiard(w, h):
+            sage: from flatsurf import translation_surfaces
+            sage: S = translation_surfaces.mcmullen_L(1, 1, 1, 1)
+
+            sage: p = S.point(0, (0, 0))
+            sage: p.coordinates(0)  # random output: order depends on the Python version
+            ((0, 0), (1, 0), (0, 1), (1, 1))
+
+        """
+        return tuple(
+            coordinates for (l, coordinates) in self._representatives if l == label
+        )
+
+    def graphical_surface_point(self, graphical_surface=None):
         r"""
-        Return a (finite) step billiard associated to the given widths ``w`` and heights ``h``.
+        Return a
+        :class:`flatsurf.graphical.surface_point.GraphicalSurfacePoint` to
+        represent this point graphically.
 
         EXAMPLES::
 
             sage: from flatsurf import half_translation_surfaces
-            sage: S = half_translation_surfaces.step_billiard([1,1,1,1], [1,1/2,1/3,1/5])
-            sage: S
-            HalfTranslationSurface built from 8 polygons
-            sage: TestSuite(S).run()
-        """
-        n = len(h)
-        assert len(w) == n
-        if n < 2:
-            raise ValueError("w and h must have length at least 2")
-        H = sum(h)
-        W = sum(w)
-
-        R = Sequence(w + h).universe()
-        C = ConvexPolygons(R.fraction_field())
-
-        P = []
-        Prev = []
-        x = 0
-        y = H
-        for i in range(n - 1):
-            P.append(C(vertices=[(x, 0), (x + w[i], 0), (x + w[i], y - h[i]), (x + w[i], y), (x, y)]))
-            x += w[i]
-            y -= h[i]
-        assert x == W - w[-1]
-        assert y == h[-1]
-        P.append(C(vertices=[(x, 0), (x + w[-1], 0), (x + w[-1], y), (x, y)]))
-
-        Prev = [C(vertices=[(x, -y) for x,y in reversed(p.vertices())]) for p in P]
-
-        S = Surface_list(base_ring = C.base_ring())
-        S.rename("StepBilliard(w=[%s], h=[%s])" % (', '.join(map(str, w)), ', '.join(map(str, h))))
-        S.add_polygons(P)    # get labels 0, ..., n-1
-        S.add_polygons(Prev) # get labels n, n+1, ..., 2n-1
-
-        # reflection gluings
-        # (gluings between the polygon and its reflection)
-        S.set_edge_pairing(0, 4, n, 4)
-        S.set_edge_pairing(n-1, 0, 2*n-1, 2)
-        S.set_edge_pairing(n-1, 1, 2*n-1, 1)
-        S.set_edge_pairing(n-1, 2, 2*n-1, 0)
-        for i in range(n-1):
-            # set_edge_pairing(polygon1, edge1, polygon2, edge2)
-            S.set_edge_pairing(i, 0, n+i, 3)
-            S.set_edge_pairing(i, 2, n+i, 1)
-            S.set_edge_pairing(i, 3, n+i, 0)
-
-        # translation gluings
-        S.set_edge_pairing(n-2, 1, n-1, 3)
-        S.set_edge_pairing(2*n-2, 2, 2*n-1, 3)
-        for i in range(n-2):
-            S.set_edge_pairing(i, 1, i+1, 4)
-            S.set_edge_pairing(n+i, 2, n+i+1, 4)
+            sage: S = half_translation_surfaces.step_billiard([1, 1, 1, 1], [1, 1/2, 1/3, 1/4])
+            sage: p = S.point(0, (1/2, 1/2))
+            sage: G = p.graphical_surface_point()
 
-        S.set_immutable()
-        return HalfTranslationSurface(S)
+        """
+        from flatsurf.graphical.surface_point import GraphicalSurfacePoint
 
-half_translation_surfaces = HalfTranslationSurfaceGenerators()
+        return GraphicalSurfacePoint(self, graphical_surface=graphical_surface)
 
-class TranslationSurfaceGenerators:
-    r"""
-    Common and less common translation surfaces.
-    """
-    @staticmethod
-    def square_torus(a=1):
+    def plot(self, *args, **kwargs):
         r"""
-        Return flat torus obtained by identification of the opposite sides of a
-        square.
+        Return a plot of this point.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
-            sage: T = translation_surfaces.square_torus()
-            sage: T
-            TranslationSurface built from 1 polygon
-            sage: TestSuite(T).run()
-
-        Rational directions are completely periodic::
-
-            sage: v = T.tangent_vector(0, (1/33, 1/257), (13,17))
-            sage: L = v.straight_line_trajectory()
-            sage: L.flow(13+17)
-            sage: L.is_closed()
-            True
+            sage: from flatsurf import half_translation_surfaces
+            sage: S = half_translation_surfaces.step_billiard([1, 1, 1, 1], [1, 1/2, 1/3, 1/4])
+            sage: p = S.point(0, (0, 0))
+            sage: p.plot()
+            ...Graphics object consisting of 1 graphics primitive
+
+            sage: p = S.point(0, (0, 25/12))
+            sage: p.plot()
+            ...Graphics object consisting of 1 graphics primitive
+
+        """
+        graphical_surface = None
+        if args:
+            graphical_surface = args[0]
+            args = args[1:]
+
+        return self.graphical_surface_point(graphical_surface=graphical_surface).plot(
+            *args, **kwargs
+        )
+
+    def __repr__(self):
+        r"""
+        Return a printable representation of this point.
 
         TESTS::
 
-            sage: TestSuite(T).run()
+            sage: from flatsurf import half_translation_surfaces
+            sage: S = half_translation_surfaces.step_billiard([1, 1, 1, 1], [1, 1/2, 1/3, 1/4])
+            sage: S.point(0, (1/2, 1/2))
+            Point (1/2, 1/2) of polygon 0
+
         """
-        return TranslationSurfaceGenerators.torus((a,0), (0,a))
 
-    @staticmethod
-    def torus(u, v):
+        def render(label, coordinates):
+            if self.is_vertex():
+                vertex = (
+                    self.surface()
+                    .polygon(label)
+                    .get_point_position(coordinates)
+                    .get_vertex()
+                )
+                return "Vertex {} of polygon {}".format(vertex, label)
+
+            return "Point {} of polygon {}".format(coordinates, label)
+
+        # We pick a specific representative to make our lives easier when doctesting
+        return min(
+            render(label, coordinates)
+            for (label, coordinates) in self.representatives()
+        )
+
+    def __eq__(self, other):
         r"""
-        Return the flat torus obtained as the quotient of the plane by the pair
-        of vectors ``u`` and ``v``.
+        Return whether this point is indistinguishable from ``other``.
 
         EXAMPLES::
 
-            sage: from flatsurf import translation_surfaces
-            sage: T = translation_surfaces.torus((1, AA(2).sqrt()), (AA(3).sqrt(), 3))
-            sage: T
-            TranslationSurface built from 1 polygon
-            sage: T.polygon(0)
-            Polygon: (0, 0), (1, 1.414213562373095?), (2.732050807568878?, 4.414213562373095?), (1.732050807568878?, 3)
-        """
-        u = vector(u)
-        v = vector(v)
-        field = Sequence([u,v]).universe().base_ring()
-        if isinstance(field, type):
-            field = py_scalar_parent(field)
-        if not field.is_field():
-            field = field.fraction_field()
-        s = Surface_list(base_ring=field)
-        p = polygons(vertices=[(0,0), u, u+v, v], base_ring=field)
-        s.add_polygon(p, [(0,2),(0,3),(0,0),(0,1)])
-        s.set_immutable()
-        return TranslationSurface(s)
+            sage: from flatsurf import half_translation_surfaces
+            sage: S = half_translation_surfaces.step_billiard([1, 1, 1, 1], [1, 1/2, 1/3, 1/4])
+            sage: p = S.point(0, (1/2, 1/2))
+            sage: p == p
+            True
+
+            sage: q = S.point(0, (1/2, 1/3))
+            sage: p == q
+            False
+
+        TESTS:
+
+        Verify that points can be compared to non-points so they can be put into sets and dicts with other objects::
+
+            sage: p == 42
+            False
 
-    @staticmethod
-    def veech_2n_gon(n):
+        """
+        if self is other:
+            return True
+        if not isinstance(other, SurfacePoint):
+            return False
+        if not self._surface == other._surface:
+            return False
+        return self._representatives == other._representatives
+
+    def _test_category(self, **options):
         r"""
-        The regular 2n-gon with opposite sides identified.
+        Check that this point inherits from the element class of its surface's
+        category.
+
+        Overridden to disable these tests when this is a point of a mutable
+        surface since the category might then change as the surface becomes
+        immutable.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
-            sage: s=translation_surfaces.veech_2n_gon(5)
-            sage: s.polygon(0)
-            Polygon: (0, 0), (1, 0), (-1/2*a^2 + 5/2, 1/2*a), (-a^2 + 7/2, -1/2*a^3 + 2*a), (-1/2*a^2 + 5/2, -a^3 + 7/2*a), (1, -a^3 + 4*a), (0, -a^3 + 4*a), (1/2*a^2 - 3/2, -a^3 + 7/2*a), (a^2 - 5/2, -1/2*a^3 + 2*a), (1/2*a^2 - 3/2, 1/2*a)
-            sage: TestSuite(s).run()
-        """
-        p = polygons.regular_ngon(2*n)
-        s = Surface_list(base_ring=p.base_ring())
-        s.add_polygon(p,[ ( 0, (i+n)%(2*n) ) for i in range(2*n)] )
-        s.set_immutable()
-        return TranslationSurface(s)
+            sage: from flatsurf import half_translation_surfaces
+            sage: S = half_translation_surfaces.step_billiard([1, 1, 1, 1], [1, 1/2, 1/3, 1/4])
+            sage: p = S.point(0, (1/2, 1/2))
+            sage: p._test_category()
 
-    @staticmethod
-    def veech_double_n_gon(n):
+        """
+        if self.surface().is_mutable():
+            return
+
+        super()._test_category(**options)
+
+    def __hash__(self):
         r"""
-        A pair of regular n-gons with each edge of one identified to an edge of the other to make a translation surface.
+        Return a hash value of this point.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
-            sage: s=translation_surfaces.veech_double_n_gon(5)
-            sage: TestSuite(s).run()
-        """
-        from sage.matrix.constructor import Matrix
-        p = polygons.regular_ngon(n)
-        s = Surface_list(base_ring=p.base_ring())
-        m = Matrix([[-1,0],[0,-1]])
-        s.add_polygon(p) # label=0
-        s.add_polygon(m*p, [(0,i) for i in range(n)])
-        s.set_immutable()
-        return TranslationSurface(s)
+            sage: from flatsurf import half_translation_surfaces
+            sage: S = half_translation_surfaces.step_billiard([1, 1, 1, 1], [1, 1/2, 1/3, 1/4])
+            sage: p = S.point(0, (0, 0))
+            sage: q = S.point(4, (0, 0))
+            sage: hash(p) == hash(q)
+            True
 
+        """
+        return hash(self._representatives)
 
-    @staticmethod
-    def regular_octagon():
+    def __ne__(self, other):
         r"""
-        Return the translation surface built from the regular octagon by
-        identifying opposite sides.
+        Return whether this point is distinguishable from ``other``.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
-            sage: T = translation_surfaces.regular_octagon()
-            sage: T
-            TranslationSurface built from 1 polygon
-            sage: T.stratum()
-            H_2(2)
-            sage: TestSuite(T).run()
-        """
-        return translation_surfaces.veech_2n_gon(4)
-
-    @staticmethod
-    def mcmullen_genus2_prototype(w, h, t, e, rel=0, base_ring=None):
-        r"""
-        McMullen prototypes in the stratum H(2).
-
-        These prototype appear at least in McMullen "Teichmüller curves in genus
-        two: Discriminant and spin" (2004). The notation from that paper are
-        quadruple ``(a, b, c, e)`` which translates in our notation as
-        ``w = b``, ``h = c``, ``t = a`` (and ``e = e``).
+            sage: from flatsurf import half_translation_surfaces
+            sage: S = half_translation_surfaces.step_billiard([1, 1, 1, 1], [1, 1/2, 1/3, 1/4])
+            sage: p = S.point(0, (1/2, 1/2))
+            sage: p != p
+            False
+
+            sage: q = S.point(0, (1/2, 1/3))
+            sage: p != q
+            True
 
-        The associated discriminant is `D = e^2 + 4 wh`.
+        """
+        return not (self == other)
 
-        If ``rel`` is a positive parameter (less than w-lambda) the surface belongs
-        to the eigenform locus in H(1,1).
 
-        EXAMPLES::
+class SaddleConnection(SageObject):
+    r"""
+    Represents a saddle connection on a SimilaritySurface.
+    """
 
-            sage: from flatsurf import translation_surfaces
-            sage: from surface_dynamics import AbelianStratum
+    def __init__(
+        self,
+        surface,
+        start_data,
+        direction,
+        end_data=None,
+        end_direction=None,
+        holonomy=None,
+        end_holonomy=None,
+        check=True,
+        limit=1000,
+    ):
+        r"""
+        Construct a saddle connection on a SimilaritySurface.
+
+        The only necessary parameters are the surface, start_data, and direction
+        (to start). If there is missing data that can not be inferred from the surface
+        type, then a straight-line trajectory will be computed to confirm that this is
+        indeed a saddle connection. The trajectory will pass through at most limit
+        polygons before we give up.
+
+        Details of the parameters are provided below.
+
+        Parameters
+        ----------
+        surface : a SimilaritySurface
+            which will contain the saddle connection being constructed.
+        start_data : a pair
+            consisting of the label of the polygon where the saddle connection starts
+            and the starting vertex.
+        direction : 2-dimensional vector with entries in the base_ring of the surface
+            representing the direction the saddle connection is moving in (in the
+            coordinates of the initial polygon).
+        end_data : a pair
+            consisting of the label of the polygon where the saddle connection terminates
+            and the terminating vertex.
+        end_direction : 2-dimensional vector with entries in the base_ring of the surface
+            representing the direction to move backward from the end point (in the
+            coordinates of the terminal polygon). If the surface is a DilationSurface
+            or better this will be the negation of the direction vector. If the surface
+            is a HalfDilation surface or better, then this will be either the direction
+            vector or its negation. In either case the value can be inferred from the
+            end_data.
+        holonomy : 2-dimensional vector with entries in the base_ring of the surface
+            the holonomy of the saddle connection measured from the start. To compute this
+            you develop the saddle connection into the plane starting from the starting
+            polygon.
+        end_holonomy : 2-dimensional vector with entries in the base_ring of the surface
+            the holonomy of the saddle connection measured from the end (with the opposite
+            orientation). To compute this you develop the saddle connection into the plane
+            starting from the terminating polygon. For a translation surface, this will be
+            the negation of holonomy, and for a HalfTranslation surface it will be either
+            equal to holonomy or equal to its negation. In both these cases the end_holonomy
+            can be inferred and does not need to be passed to the constructor.
+        check : boolean
+            If all data above is provided or can be inferred, then when check=False this
+            geometric data is not verified. With check=True the data is always verified
+            by straight-line flow. Erroroneous data will result in a ValueError being thrown.
+            Defaults to true.
+        limit :
+            The combinatorial limit (in terms of number of polygons crossed) to flow forward
+            to check the saddle connection geometry.
+        """
+        from flatsurf.geometry.categories import SimilaritySurfaces
+
+        if surface not in SimilaritySurfaces():
+            raise TypeError
+
+        self._surface = surface
+
+        # Sanitize the direction vector:
+        V = self._surface.base_ring().fraction_field() ** 2
+        self._direction = V(direction)
+        if self._direction == V.zero():
+            raise ValueError("Direction must be nonzero.")
+        # To canonicalize the direction vector we ensure its endpoint lies in the boundary of the unit square.
+        xabs = self._direction[0].abs()
+        yabs = self._direction[1].abs()
+        if xabs > yabs:
+            self._direction = self._direction / xabs
+        else:
+            self._direction = self._direction / yabs
 
-            sage: prototypes = {
-            ....:      5: [(1,1,0,-1)],
-            ....:      8: [(1,1,0,-2), (2,1,0,0)],
-            ....:      9: [(2,1,0,-1)],
-            ....:     12: [(1,2,0,-2), (2,1,0,-2), (3,1,0,0)],
-            ....:     13: [(1,1,0,-3), (3,1,0,-1), (3,1,0,1)],
-            ....:     16: [(3,1,0,-2), (4,1,0,0)],
-            ....:     17: [(1,2,0,-3), (2,1,0,-3), (2,2,0,-1), (2,2,1,-1), (4,1,0,-1), (4,1,0,1)],
-            ....:     20: [(1,1,0,-4), (2,2,1,-2), (4,1,0,-2), (4,1,0,2)],
-            ....:     21: [(1,3,0,-3), (3,1,0,-3)],
-            ....:     24: [(1,2,0,-4), (2,1,0,-4), (3,2,0,0)],
-            ....:     25: [(2,2,0,-3), (2,2,1,-3), (3,2,0,-1), (4,1,0,-3)]}
-
-            sage: for D in sorted(prototypes):
-            ....:     for w,h,t,e in prototypes[D]:
-            ....:          T = translation_surfaces.mcmullen_genus2_prototype(w,h,t,e)
-            ....:          assert T.stratum() == AbelianStratum(2)
-            ....:          assert (D.is_square() and T.base_ring() is QQ) or (T.base_ring().polynomial().discriminant() == D)
-
-        An example with some relative homology::
-
-            sage: U8 = translation_surfaces.mcmullen_genus2_prototype(2,1,0,0,1/4)    # discriminant 8
-            sage: U12 = translation_surfaces.mcmullen_genus2_prototype(3,1,0,0,3/10)   # discriminant 12
-
-            sage: U8.stratum()
-            H_2(1^2)
-            sage: U8.base_ring().polynomial().discriminant()
-            8
-            sage: U8.j_invariant()
-            (
-                      [4 0]
-            (0), (0), [0 2]
-            )
+        # Fix end_direction if not standard.
+        if end_direction is not None:
+            xabs = end_direction[0].abs()
+            yabs = end_direction[1].abs()
+            if xabs > yabs:
+                end_direction = end_direction / xabs
+            else:
+                end_direction = end_direction / yabs
 
-            sage: U12.stratum()
-            H_2(1^2)
-            sage: U12.base_ring().polynomial().discriminant()
-            12
-            sage: U12.j_invariant()
-            (
-                      [6 0]
-            (0), (0), [0 2]
+        self._surfacetart_data = tuple(start_data)
+
+        if end_direction is None:
+            from flatsurf.geometry.categories import DilationSurfaces
+
+            # Attempt to infer the end_direction.
+            if self._surface in DilationSurfaces().Positive():
+                end_direction = -self._direction
+            elif self._surface in DilationSurfaces() and end_data is not None:
+                p = self._surface.polygon(end_data[0])
+                from flatsurf.geometry.euclidean import ccw
+
+                if (
+                    ccw(p.edge(end_data[1]), self._direction) >= 0
+                    and ccw(
+                        p.edge(
+                            (len(p.vertices()) + end_data[1] - 1) % len(p.vertices())
+                        ),
+                        self._direction,
+                    )
+                    > 0
+                ):
+                    end_direction = self._direction
+                else:
+                    end_direction = -self._direction
+
+        if end_holonomy is None and holonomy is not None:
+            # Attempt to infer the end_holonomy:
+            from flatsurf.geometry.categories import (
+                HalfTranslationSurfaces,
+                TranslationSurfaces,
             )
-        """
-        w = ZZ(w)
-        h = ZZ(h)
-        t = ZZ(t)
-        e = ZZ(e)
-        g = w.gcd(h)
-        gg = g.gcd(t).gcd(e)
-        if w <= 0 or h <= 0 or t < 0 or t >= g or not g.gcd(t).gcd(e).is_one() or e+h >= w:
-            raise ValueError("invalid parameters")
-
-        x = polygen(QQ)
-        poly = x**2 - e * x - w*h
-        if poly.is_irreducible():
-            if base_ring is None:
-                emb = AA.polynomial_root(poly, RIF(0,w))
-                K = NumberField(poly, 'l', embedding=emb)
-                l = K.gen()
+
+            if self._surface in TranslationSurfaces():
+                end_holonomy = -holonomy
+            if self._surface in HalfTranslationSurfaces():
+                if direction == end_direction:
+                    end_holonomy = holonomy
+                else:
+                    end_holonomy = -holonomy
+
+        if (
+            end_data is None
+            or end_direction is None
+            or holonomy is None
+            or end_holonomy is None
+            or check
+        ):
+            v = self.start_tangent_vector()
+            traj = v.straight_line_trajectory()
+            traj.flow(limit)
+            if not traj.is_saddle_connection():
+                raise ValueError(
+                    "Did not obtain saddle connection by flowing forward. Limit="
+                    + str(limit)
+                )
+            tv = traj.terminal_tangent_vector()
+            self._end_data = (tv.polygon_label(), tv.vertex())
+            if end_data is not None:
+                if end_data != self._end_data:
+                    raise ValueError(
+                        "Provided or inferred end_data="
+                        + str(end_data)
+                        + " does not match actual end_data="
+                        + str(self._end_data)
+                    )
+            self._end_direction = tv.vector()
+            # Canonicalize again.
+            xabs = self._end_direction[0].abs()
+            yabs = self._end_direction[1].abs()
+            if xabs > yabs:
+                self._end_direction = self._end_direction / xabs
             else:
-                K = base_ring
-                roots = poly.roots(K, multiplicities=False)
-                if len(roots) != 2:
-                    raise ValueError("invalid base ring")
-                roots.sort(key=lambda x: x.numerical_approx())
-                assert roots[0] < 0 and roots[0] > 0
-                l = roots[1]
-        else:
-            if base_ring is None:
-                K = QQ
+                self._end_direction = self._end_direction / yabs
+            if end_direction is not None:
+                if end_direction != self._end_direction:
+                    raise ValueError(
+                        "Provided or inferred end_direction="
+                        + str(end_direction)
+                        + " does not match actual end_direction="
+                        + str(self._end_direction)
+                    )
+
+            if traj.segments()[0].is_edge():
+                # Special case (The below method causes error if the trajectory is just an edge.)
+                self._holonomy = self._surface.polygon(start_data[0]).edge(
+                    start_data[1]
+                )
+                self._end_holonomy = self._surface.polygon(self._end_data[0]).edge(
+                    self._end_data[1]
+                )
             else:
-                K = base_ring
-            D = e**2 + 4 * w*h
-            d = D.sqrt()
-            l = (e + d) / 2
-
-        try:
-            rel = K(rel)
-        except TypeError:
-            K = get_coercion_model().common_parent(K, parent(rel))
-            l = K(l)
-            rel = K(rel)
-
-        # (lambda,lambda) square on top
-        # twisted (w,0), (t,h)
-        s = Surface_list(base_ring=K)
-        if rel:
-            if rel < 0 or rel > w - l:
-                raise ValueError("invalid rel argument")
-            s.add_polygon(polygons(vertices=[(0,0),(l,0),(l+rel,l),(rel,l)], ring=K))
-            s.add_polygon(polygons(vertices=[(0,0),(rel,0),(rel+l,0),(w,0),(w+t,h),(l+rel+t,h),(t+l,h),(t,h)], ring=K))
-            s.set_edge_pairing(0, 1, 0, 3)
-            s.set_edge_pairing(0, 0, 1, 6)
-            s.set_edge_pairing(0, 2, 1, 1)
-            s.set_edge_pairing(1, 2, 1, 4)
-            s.set_edge_pairing(1, 3, 1, 7)
-            s.set_edge_pairing(1, 0, 1, 5)
+                from .similarity import SimilarityGroup
+
+                sim = SimilarityGroup(self._surface.base_ring()).one()
+                itersegs = iter(traj.segments())
+                next(itersegs)
+                for seg in itersegs:
+                    sim = sim * self._surface.edge_transformation(
+                        seg.start().polygon_label(), seg.start().position().get_edge()
+                    )
+                self._holonomy = (
+                    sim(traj.segments()[-1].end().point())
+                    - traj.initial_tangent_vector().point()
+                )
+                self._end_holonomy = -((~sim.derivative()) * self._holonomy)
+
+            if holonomy is not None:
+                if holonomy != self._holonomy:
+                    print("Combinatorial length: " + str(traj.combinatorial_length()))
+                    print("Start: " + str(traj.initial_tangent_vector().point()))
+                    print("End: " + str(traj.terminal_tangent_vector().point()))
+                    print("Start data:" + str(start_data))
+                    print("End data:" + str(end_data))
+                    raise ValueError(
+                        "Provided holonomy "
+                        + str(holonomy)
+                        + " does not match computed holonomy of "
+                        + str(self._holonomy)
+                    )
+            if end_holonomy is not None:
+                if end_holonomy != self._end_holonomy:
+                    raise ValueError(
+                        "Provided or inferred end_holonomy "
+                        + str(end_holonomy)
+                        + " does not match computed end_holonomy of "
+                        + str(self._end_holonomy)
+                    )
         else:
-            s.add_polygon(polygons(vertices=[(0,0),(l,0),(l,l),(0,l)], ring=K))
-            s.add_polygon(polygons(vertices=[(0,0),(l,0),(w,0),(w+t,h),(l+t,h),(t,h)], ring=K))
-            s.set_edge_pairing(0, 1, 0, 3)
-            s.set_edge_pairing(0, 0, 1, 4)
-            s.set_edge_pairing(0, 2, 1, 0)
-            s.set_edge_pairing(1, 1, 1, 3)
-            s.set_edge_pairing(1, 2, 1, 5)
-        s.set_immutable()
-        return TranslationSurface(s)
-
-    @staticmethod
-    def mcmullen_L(l1, l2, l3, l4):
-        r"""
-        Return McMullen's L shaped surface with parameters l1, l2, l3, l4.
-
-        Polygon labels and lengths are marked below::
-
-            +-----+
-            |     |
-            |  1  |l1
-            |     |
-            |     |    l4
-            +-----+---------+
-            |     |         |
-            |  0  |    2    |l2
-            |     |         |
-            +-----+---------+
-              l3
+            self._end_data = tuple(end_data)
+            self._end_direction = end_direction
+            self._holonomy = holonomy
+            self._end_holonomy = end_holonomy
 
-        EXAMPLES::
+        # Make vectors immutable
+        self._direction.set_immutable()
+        self._end_direction.set_immutable()
+        self._holonomy.set_immutable()
+        self._end_holonomy.set_immutable()
 
-            sage: from flatsurf import *
-            sage: s = translation_surfaces.mcmullen_L(1,1,1,1)
-            sage: TestSuite(s).run()
+    def surface(self):
+        return self._surface
 
-        TESTS::
+    def direction(self):
+        r"""
+        Returns a vector parallel to the saddle connection pointing from the start point.
 
-            sage: from flatsurf import translation_surfaces
-            sage: translation_surfaces.mcmullen_L(1r, 1r, 1r, 1r)
-            TranslationSurface built from 3 polygons
+        The will be normalized so that its $l_\infty$ norm is 1.
         """
-        field = Sequence([l1,l2,l3,l4]).universe()
-        if isinstance(field, type):
-            field = py_scalar_parent(field)
-        if not field.is_field():
-            field = field.fraction_field()
-
-        s = Surface_list(base_ring=field)
-        s.add_polygon(polygons((l3,0),(0,l2),(-l3,0),(0,-l2), ring=field))
-        s.add_polygon(polygons((l3,0),(0,l1),(-l3,0),(0,-l1), ring=field))
-        s.add_polygon(polygons((l4,0),(0,l2),(-l4,0),(0,-l2), ring=field))
-        s.change_edge_gluing(0,0,1,2)
-        s.change_edge_gluing(0,1,2,3)
-        s.change_edge_gluing(0,2,1,0)
-        s.change_edge_gluing(0,3,2,1)
-        s.change_edge_gluing(1,1,1,3)
-        s.change_edge_gluing(2,0,2,2)
-        s.set_immutable()
-        return TranslationSurface(s)
+        return self._direction
 
-    @staticmethod
-    def ward(n):
+    def end_direction(self):
         r"""
-        Return the surface formed by gluing a regular 2n-gon to two regular n-gons.
-        These surfaces have Veech's lattice property due to work of Ward.
+        Returns a vector parallel to the saddle connection pointing from the end point.
 
-        EXAMPLES::
+        The will be normalized so that its `l_\infty` norm is 1.
+        """
+        return self._end_direction
 
-            sage: from flatsurf import *
-            sage: s=translation_surfaces.ward(3)
-            sage: TestSuite(s).run()
-            sage: s=translation_surfaces.ward(7)
-            sage: TestSuite(s).run()
-        """
-        assert n>=3
-        o = ZZ_2*polygons.regular_ngon(2*n)
-        p1 = polygons(*[o.edge((2*i+n)%(2*n)) for i in range(n)])
-        p2 = polygons(*[o.edge((2*i+n+1)%(2*n)) for i in range(n)])
-        s = Surface_list(base_ring=o.parent().field())
-        s.add_polygon(o)
-        s.add_polygon(p1)
-        s.add_polygon(p2)
-        s.change_polygon_gluings(1, [(0,2*i) for i in range(n)])
-        s.change_polygon_gluings(2, [(0,2*i+1) for i in range(n)])
-        s.set_immutable()
-        return TranslationSurface(s)
+    def start_data(self):
+        r"""
+        Return the pair (l, v) representing the label and vertex of the corresponding polygon
+        where the saddle connection originates.
+        """
+        return self._surfacetart_data
 
-    @staticmethod
-    def octagon_and_squares():
+    def end_data(self):
         r"""
-        EXAMPLES::
+        Return the pair (l, v) representing the label and vertex of the corresponding polygon
+        where the saddle connection terminates.
+        """
+        return self._end_data
 
-            sage: from flatsurf import translation_surfaces
-            sage: os = translation_surfaces.octagon_and_squares()
-            sage: os
-            TranslationSurface built from 3 polygons
-            sage: TestSuite(os).run()
+    def holonomy(self):
+        r"""
+        Return the holonomy vector of the saddle connection (measured from the start).
+
+        In a SimilaritySurface this notion corresponds to developing the saddle connection into the plane
+        using the initial chart coming from the initial polygon.
         """
-        return translation_surfaces.ward(4)
+        return self._holonomy
 
-    @staticmethod
-    def cathedral(a, b):
+    def length(self):
         r"""
-        Return the cathedral surface with parameters ``a`` and ``b``.
+        In a cone surface, return the length of this saddle connection. Since
+        this may not lie in the field of definition of the surface, it is
+        returned as an element of the Algebraic Real Field.
+        """
+        from flatsurf.geometry.categories import ConeSurfaces
 
-        For any parameter ``a`` and ``b``, the cathedral surface belongs to the
-        so-called Gothic locus described in McMullen, Mukamel, Wright "Cubic
-        curves and totally geodesic subvarieties of moduli space" (2017).
+        if self._surface not in ConeSurfaces():
+            raise NotImplementedError(
+                "length of a saddle connection only makes sense for cone surfaces"
+            )
 
-                     1
-                   <--->
+        return vector(AA, self._holonomy).norm()
 
-                    /\           2a
-                   /  \      +------+
-               a  b|   | a  /        \
-             +----+    +---+          +
-             |    |    |   |          |
-            1| P0 |P1  |P2 |  P3      |
-             |    |    |   |          |
-             +----+    +---+          +
-                 b|    |    \        /
-                   \  /      +------+
-                    \/
+    def end_holonomy(self):
+        r"""
+        Return the holonomy vector of the saddle connection (measured from the end).
 
-        If a and b satisfies
+        In a SimilaritySurface this notion corresponds to developing the saddle connection into the plane
+        using the initial chart coming from the initial polygon.
+        """
+        return self._end_holonomy
 
-        .. MATH::
+    def start_tangent_vector(self):
+        r"""
+        Return a tangent vector to the saddle connection based at its start.
+        """
+        return self._surface.tangent_vector(
+            self._surfacetart_data[0],
+            self._surface.polygon(self._surfacetart_data[0]).vertex(
+                self._surfacetart_data[1]
+            ),
+            self._direction,
+        )
 
-            a = x + y \sqrt(d) \qquad b = -3x -3/2 + 3y \sqrt(d)
+    @cached_method(key=lambda self, limit, cache: None)
+    def trajectory(self, limit=1000, cache=None):
+        r"""
+        Return a straight line trajectory representing this saddle connection.
+        Fails if the trajectory passes through more than limit polygons.
+        """
+        if cache is not None:
+            import warnings
 
-        for some rational x,y and d >= 0 then it is a Teichmüller curve.
+            warnings.warn(
+                "The cache keyword argument of trajectory() is ignored. Trajectories are always cached."
+            )
 
-        EXAMPLES::
+        v = self.start_tangent_vector()
+        traj = v.straight_line_trajectory()
+        traj.flow(limit)
+        if not traj.is_saddle_connection():
+            raise ValueError(
+                "Did not obtain saddle connection by flowing forward. Limit="
+                + str(limit)
+            )
 
-            sage: from flatsurf import translation_surfaces
-            sage: C = translation_surfaces.cathedral(1,2)
-            sage: C.stratum()
-            H_4(2^3)
-            sage: TestSuite(C).run()
-
-            sage: from pyexactreal import ExactReals # optional: exactreal
-            sage: K = QuadraticField(5, embedding=AA(5).sqrt())
-            sage: R = ExactReals(K) # optional: exactreal
-            sage: C = translation_surfaces.cathedral(K.gen(), R.random_element([0.1, 0.2])) # optional: exactreal
-            sage: C.stratum() # optional: exactreal
-            H_4(2^3)
-            sage: TestSuite(C).run() # long time (6s), optional: exactreal
-        """
-        ring = Sequence([a,b]).universe()
-        if isinstance(ring, type):
-            ring = py_scalar_parent(ring)
-        if not ring.has_coerce_map_from(QQ):
-            ring = ring.fraction_field()
-        a = ring(a)
-        b = ring(b)
-        P = ConvexPolygons(ring)
-        s = Surface_list(base_ring=ring)
-        half = QQ((1,2))
-        p0 = P(vertices=[(0,0),(a,0),(a,1),(0,1)])
-        p1 = P(vertices=[(a,0),(a,-b),(a+half,-b-half),(a+1,-b),(a+1,0),(a+1,1),(a+1,b+1),(a+half,b+1+half),(a,b+1),(a,1)])
-        p2 = P(vertices=[(a+1,0),(2*a+1,0),(2*a+1,1),(a+1,1)])
-        p3 = P(vertices=[(2*a+1,0), (2*a+1+half,-half),(4*a+1+half,-half),(4*a+2,0),(4*a+2,1),(4*a+1+half,1+half),(2*a+1+half,1+half),(2*a+1,1)])
-        s.add_polygon(p0)
-        s.add_polygon(p1)
-        s.add_polygon(p2)
-        s.add_polygon(p3)
-        s.set_edge_pairing(0, 0, 0, 2)
-        s.set_edge_pairing(0, 1, 1, 9)
-        s.set_edge_pairing(0, 3, 3, 3)
-        s.set_edge_pairing(1, 0, 1, 3)
-        s.set_edge_pairing(1, 1, 3, 4)
-        s.set_edge_pairing(1, 2, 3, 6)
-        s.set_edge_pairing(1, 4, 2, 3)
-        s.set_edge_pairing(1, 5, 1, 8)
-        s.set_edge_pairing(1, 6, 3, 0)
-        s.set_edge_pairing(1, 7, 3, 2)
-        s.set_edge_pairing(2, 0, 2, 2)
-        s.set_edge_pairing(2, 1, 3, 7)
-        s.set_edge_pairing(3, 1, 3, 5)
-        s.set_immutable()
-        return TranslationSurface(s)
-
-    @staticmethod
-    def arnoux_yoccoz(genus):
-        r"""
-        Construct the Arnoux-Yoccoz surface of genus 3 or greater.
-
-        This presentation of the surface follows Section 2.3 of
-        Joshua P. Bowman's paper "The Complete Family of Arnoux-Yoccoz
-        Surfaces."
+        return traj
 
-        EXAMPLES::
+    def plot(self, *args, **options):
+        r"""
+        Equivalent to ``.trajectory().plot(*args, **options)``
+        """
+        return self.trajectory().plot(*args, **options)
 
-            sage: from flatsurf import *
-            sage: s = translation_surfaces.arnoux_yoccoz(4)
-            sage: TestSuite(s).run()
-            sage: s.is_delaunay_decomposed()
-            True
-            sage: s = s.canonicalize()
-            sage: field=s.base_ring()
-            sage: a = field.gen()
-            sage: from sage.matrix.constructor import Matrix
-            sage: m = Matrix([[a,0],[0,~a]])
-            sage: ss = m*s
-            sage: ss = ss.canonicalize()
-            sage: s.cmp(ss) == 0
-            True
+    def end_tangent_vector(self):
+        r"""
+        Return a tangent vector to the saddle connection based at its start.
+        """
+        return self._surface.tangent_vector(
+            self._end_data[0],
+            self._surface.polygon(self._end_data[0]).vertex(self._end_data[1]),
+            self._end_direction,
+        )
 
-        The Arnoux-Yoccoz pseudo-Anosov are known to have (minimal) invariant
-        foliations with SAF=0::
+    def invert(self):
+        r"""
+        Return this saddle connection but with opposite orientation.
+        """
+        return SaddleConnection(
+            self._surface,
+            self._end_data,
+            self._end_direction,
+            self._surfacetart_data,
+            self._direction,
+            self._end_holonomy,
+            self._holonomy,
+            check=False,
+        )
 
-            sage: S3 = translation_surfaces.arnoux_yoccoz(3)
-            sage: Jxx, Jyy, Jxy = S3.j_invariant()
-            sage: Jxx.is_zero() and Jyy.is_zero()
-            True
-            sage: Jxy
-            [ 0  2  0]
-            [ 2 -2  0]
-            [ 0  0  2]
-
-            sage: S4 = translation_surfaces.arnoux_yoccoz(4)
-            sage: Jxx, Jyy, Jxy = S4.j_invariant()
-            sage: Jxx.is_zero() and Jyy.is_zero()
-            True
-            sage: Jxy
-            [ 0  2  0  0]
-            [ 2 -2  0  0]
-            [ 0  0  2  2]
-            [ 0  0  2  0]
-        """
-        g=ZZ(genus)
-        assert g>=3
-        x = polygen(AA)
-        p=sum([x**i for i in range(1,g+1)])-1
-        cp = AA.common_polynomial(p)
-        alpha_AA = AA.polynomial_root(cp, RIF(1/2, 1))
-        field=NumberField(alpha_AA.minpoly(),'alpha',embedding=alpha_AA)
-        a=field.gen()
-        V = VectorSpace(field,2)
-        p=[None for i in range(g+1)]
-        q=[None for i in range(g+1)]
-        p[0]=V(( (1-a**g)/2, a**2/(1-a) ))
-        q[0]=V(( -a**g/2, a ))
-        p[1]=V(( -(a**(g-1)+a**g)/2, (a-a**2+a**3)/(1-a) ))
-        p[g]=V(( 1+(a-a**g)/2, (3*a-1-a**2)/(1-a) ))
-        for i in range(2,g):
-            p[i]=V(( (a-a**i)/(1-a) , a/(1-a) ))
-        for i in range(1,g+1):
-            q[i]=V(( (2*a-a**i-a**(i+1))/(2*(1-a)), (a-a**(g-i+2))/(1-a) ))
-        P = ConvexPolygons(field)
-        s = Surface_list(field)
-        T = [None] * (2*g+1)
-        Tp = [None] * (2*g+1)
-        from sage.matrix.constructor import Matrix
-        m=Matrix([[1,0],[0,-1]])
-        for i in range(1,g+1):
-            # T_i is (P_0,Q_i,Q_{i-1})
-            T[i]=s.add_polygon(P(edges=[ q[i]-p[0], q[i-1]-q[i], p[0]-q[i-1] ]))
-            # T_{g+i} is (P_i,Q_{i-1},Q_{i})
-            T[g+i]=s.add_polygon(P(edges=[ q[i-1]-p[i], q[i]-q[i-1], p[i]-q[i] ]))
-            # T'_i is (P'_0,Q'_{i-1},Q'_i)
-            Tp[i]=s.add_polygon(m*s.polygon(T[i]))
-            # T'_{g+i} is (P'_i,Q'_i, Q'_{i-1})
-            Tp[g+i]=s.add_polygon(m*s.polygon(T[g+i]))
-        for i in range(1,g):
-            s.change_edge_gluing(T[i],0,T[i+1],2)
-            s.change_edge_gluing(Tp[i],2,Tp[i+1],0)
-        for i in range(1,g+1):
-            s.change_edge_gluing(T[i],1,T[g+i],1)
-            s.change_edge_gluing(Tp[i],1,Tp[g+i],1)
-        #P 0 Q 0 is paired with P' 0 Q' 0, ...
-        s.change_edge_gluing(T[1],2,Tp[g],2)
-        s.change_edge_gluing(Tp[1],0,T[g],0)
-        # P1Q1 is paired with P'_g Q_{g-1}
-        s.change_edge_gluing(T[g+1],2,Tp[2*g],2)
-        s.change_edge_gluing(Tp[g+1],0,T[2*g],0)
-        # P1Q0 is paired with P_{g-1} Q_{g-1}
-        s.change_edge_gluing(T[g+1],0,T[2*g-1],2)
-        s.change_edge_gluing(Tp[g+1],2,Tp[2*g-1],0)
-        # PgQg is paired with Q1P2
-        s.change_edge_gluing(T[2*g],2,T[g+2],0)
-        s.change_edge_gluing(Tp[2*g],0,Tp[g+2],2)
-        for i in range(2,g-1):
-            # PiQi is paired with Q'_i P'_{i+1}
-            s.change_edge_gluing(T[g+i],2,Tp[g+i+1],2)
-            s.change_edge_gluing(Tp[g+i],0,T[g+i+1],0)
-        s.set_immutable()
-        return TranslationSurface(s)
+    def intersections(self, traj, count_singularities=False, include_segments=False):
+        r"""
+        See documentation of :meth:`~.straight_line_trajectory.AbstractStraightLineTrajectory.intersections`
+        """
+        return self.trajectory().intersections(
+            traj, count_singularities, include_segments
+        )
 
-    @staticmethod
-    def from_flipper(h):
+    def intersects(self, traj, count_singularities=False):
         r"""
-        Build a (half-)translation surface from a flipper pseudo-Anosov.
+        See documentation of :meth:`~.straight_line_trajectory.AbstractStraightLineTrajectory.intersects`
+        """
+        return self.trajectory().intersects(
+            traj, count_singularities=count_singularities
+        )
 
-        EXAMPLES::
+    def __eq__(self, other):
+        r"""
+        Return whether this saddle connection is indistinguishable from
+        ``other``.
 
-            sage: from flatsurf import *
-            sage: import flipper                             # optional - flipper
+        EXAMPLES::
 
-        A torus example::
+            sage: from flatsurf import translation_surfaces
+            sage: S = translation_surfaces.square_torus()
+            sage: connections = S.saddle_connections(13)
 
-            sage: t1 = (0r,1r,2r)                            # optional - flipper
-            sage: t2 = (~0r,~1r,~2r)                         # optional - flipper
-            sage: T = flipper.create_triangulation([t1,t2])  # optional - flipper
-            sage: L1 = T.lamination([1r,0r,1r])              # optional - flipper
-            sage: L2 = T.lamination([0r,1r,1r])              # optional - flipper
-            sage: h1 = L1.encode_twist()                     # optional - flipper
-            sage: h2 = L2.encode_twist()                     # optional - flipper
-            sage: h = h1*h2^(-1r)                            # optional - flipper
-            sage: f = h.flat_structure()                     # optional - flipper
-            sage: ts = translation_surfaces.from_flipper(h)  # optional - flipper
-            sage: ts                                         # optional - flipper
-            HalfTranslationSurface built from 2 polygons
-            sage: TestSuite(ts).run()                        # optional - flipper
-
-        A non-orientable example::
-
-            sage: T = flipper.load('SB_4')                   # optional - flipper
-            sage: h = T.mapping_class('s_0S_1s_2S_3s_1S_2')  # optional - flipper
-            sage: h.is_pseudo_anosov()                       # optional - flipper
+            sage: connections[0] == connections[0]
             True
-            sage: S = translation_surfaces.from_flipper(h)   # optional - flipper
-            sage: TestSuite(S).run()                         # optional - flipper
-            sage: S.num_polygons()                           # optional - flipper
-            4
-            sage: from flatsurf.geometry.similarity_surface_generators import flipper_nf_element_to_sage
-            sage: a = flipper_nf_element_to_sage(h.dilatation())  # optional - flipper
-        """
-        from .surface import surface_list_from_polygons_and_gluings
+            sage: connections[0] == connections[1]
+            False
+
+
+        TESTS:
 
-        f = h.flat_structure()
+        Verify that saddle connections can be compared to arbitrary objects (so
+        they can be put into dicts with other objects)::
 
-        x = next(itervalues(f.edge_vectors)).x
-        K = flipper_nf_to_sage(x.field)
-        V = VectorSpace(K, 2)
-        edge_vectors = {i: V((flipper_nf_element_to_sage(e.x, K),
-                              flipper_nf_element_to_sage(e.y, K)))
-                for i,e in iteritems(f.edge_vectors)}
-
-        to_polygon_number = {k:(i,j) for i,t in enumerate(f.triangulation) for j,k in enumerate(t)}
-
-        C = ConvexPolygons(K)
-
-        polys = []
-        adjacencies = {}
-        for i,t in enumerate(f.triangulation):
-            for j,k in enumerate(t):
-                adjacencies[(i,j)] = to_polygon_number[~k]
-            try:
-                poly = C([edge_vectors[i] for i in tuple(t)])
-            except ValueError:
-                raise ValueError("t = {}, edges = {}".format(
-                    t, [edge_vectors[i].n(digits=6) for i in t]))
-            polys.append(poly)
+            sage: connections[0] == 42
+            False
+
+        ::
+
+            sage: len(connections)
+            32
+            sage: len(set(connections))
+            32
+
+        """
+        if self is other:
+            return True
+        if not isinstance(other, SaddleConnection):
+            return False
+        if not self._surface == other._surface:
+            return False
+        if not self._direction == other._direction:
+            return False
+        if not self._surfacetart_data == other._surfacetart_data:
+            return False
+        # Initial data should determine the saddle connection:
+        return True
+
+    def __ne__(self, other):
+        return not self == other
+
+    def __hash__(self):
+        return 41 * hash(self._direction) - 97 * hash(self._surfacetart_data)
+
+    def _test_geometry(self, **options):
+        # Test that this saddle connection actually exists on the surface.
+        SaddleConnection(
+            self._surface,
+            self._surfacetart_data,
+            self._direction,
+            self._end_data,
+            self._end_direction,
+            self._holonomy,
+            self._end_holonomy,
+            check=True,
+        )
+
+    def __repr__(self):
+        return "Saddle connection in direction {} with start data {} and end data {}".format(
+            self._direction, self._surfacetart_data, self._end_data
+        )
+
+    def _test_inverse(self, **options):
+        # Test that inverting works properly.
+        SaddleConnection(
+            self._surface,
+            self._end_data,
+            self._end_direction,
+            self._surfacetart_data,
+            self._direction,
+            self._end_holonomy,
+            self._holonomy,
+            check=True,
+        )
 
-        return HalfTranslationSurface(surface_list_from_polygons_and_gluings(polys, adjacencies))
 
-    @staticmethod
-    def origami(r, u, rr=None, uu=None, domain=None):
+class Cylinder(SageObject):
+    r"""
+    Represents a cylinder in a SimilaritySurface. A cylinder for these purposes is a
+    topological annulus in a surface bounded by a finite collection of saddle connections
+    meeting at 180 degree angles.
+
+    To Do
+    -----
+    * Support cylinders whose monodromy is a dilation.
+
+    EXAMPLES::
+
+        sage: from flatsurf import translation_surfaces
+        sage: s = translation_surfaces.octagon_and_squares()
+        sage: from flatsurf.geometry.surface_objects import Cylinder
+        sage: cyl = Cylinder(s, 0, [2, 3, 3, 3, 2, 0, 1, 3, 2, 0])
+        sage: cyl.initial_label()
+        0
+        sage: cyl.edges()
+        (2, 3, 3, 3, 2, 0, 1, 3, 2, 0)
+        sage: # a = sqrt(2) below.
+        sage: cyl.area()
+        2*a + 4
+        sage: cyl.circumference().minpoly()
+        x^4 - 680*x^2 + 400
+        sage: cyl.holonomy()
+        (8*a + 12, 4*a + 6)
+    """
+
+    def __init__(self, s, label0, edges):
         r"""
-        Return the origami defined by the permutations ``r`` and ``u``.
+        Construct a cylinder on the surface `s` from an initial label and a
+        sequence of edges crossed.
 
-        EXAMPLES::
+        Parameters
+        ----------
+        s: A SimilaritySurface
+            the surface containing the cylinder
+        label0: An initial label
+            representing a polygon the cylinder passes through.
+        edges: a list
+            giving the sequence of edges the cylinder crosses until it closes.
+        """
+        self._surface = s
+        self._label0 = label0
+        self._edges = tuple(edges)
+        ss = s.minimal_cover(cover_type="planar")
+        SG = SimilarityGroup(s.base_ring())
+        labels = [(label0, SG.one())]  # labels of polygons on the cover ss.
+        for e in edges:
+            labels.append(ss.opposite_edge(labels[-1], e)[0])
+        if labels[0][0] != labels[-1][0]:
+            raise ValueError("Combinatorial path does not close.")
+        trans = labels[-1][1]
+        if not trans.is_translation():
+            raise NotImplementedError(
+                "Only cylinders with translational monodromy are currently supported"
+            )
+        m = trans.matrix()
+        v = vector(s.base_ring(), (m[0][2], m[1][2]))  # translation vector
+        from flatsurf.geometry.euclidean import ccw
+
+        p = ss.polygon(labels[0])
+        e = edges[0]
+        min_y = ccw(v, p.vertex(e))
+        max_y = ccw(v, p.vertex((e + 1) % len(p.vertices())))
+        if min_y >= max_y:
+            raise ValueError("Combinatorial data does not represent a cylinder")
+
+        # Stores the vertices where saddle connections starts:
+        min_list = [0]
+        max_list = [0]
+
+        for i in range(1, len(edges)):
+            e = edges[i]
+            p = ss.polygon(labels[i])
+            y = ccw(v, p.vertex(e))
+            if y == min_y:
+                min_list.append(i)
+            elif y > min_y:
+                min_list = [i]
+                min_y = y
+                if min_y >= max_y:
+                    raise ValueError("Combinatorial data does not represent a cylinder")
+            y = ccw(v, p.vertex((e + 1) % len(p.vertices())))
+            if y == max_y:
+                max_list.append(i)
+            elif y < max_y:
+                max_list = [i]
+                max_y = y
+                if min_y >= max_y:
+                    raise ValueError("Combinatorial data does not represent a cylinder")
+
+        # Extract the saddle connections on the right side:
+        from flatsurf.geometry.surface_objects import SaddleConnection
+
+        sc_set_right = set()
+        vertices = []
+        for i in min_list:
+            label = labels[i]
+            p = ss.polygon(label)
+            vertices.append((i, p.vertex(edges[i])))
+        i, vert_i = vertices[-1]
+        vert_i = vert_i - v
+        j, vert_j = vertices[0]
+        if vert_i != vert_j:
+            li = labels[i]
+            li = (li[0], SG(-v) * li[1])
+            lio = ss.opposite_edge(li, edges[i])
+            lj = labels[j]
+            sc = SaddleConnection(
+                s,
+                (lio[0][0], (lio[1] + 1) % len(ss.polygon(lio[0]).vertices())),
+                (~lio[0][1])(vert_j) - (~lio[0][1])(vert_i),
+            )
+            sc_set_right.add(sc)
+        i = j
+        vert_i = vert_j
+        for j, vert_j in vertices[1:]:
+            if vert_i != vert_j:
+                li = labels[i]
+                li = (li[0], SG(-v) * li[1])
+                lio = ss.opposite_edge(li, edges[i])
+                lj = labels[j]
+                sc = SaddleConnection(
+                    s,
+                    (lio[0][0], (lio[1] + 1) % len(ss.polygon(lio[0]).vertices())),
+                    (~lio[0][1])(vert_j) - (~lio[0][1])(vert_i),
+                    limit=j - i,
+                )
+                sc_set_right.add(sc)
+            i = j
+            vert_i = vert_j
+
+        # Extract the saddle connections on the left side:
+        sc_set_left = set()
+        vertices = []
+        for i in max_list:
+            label = labels[i]
+            p = ss.polygon(label)
+            vertices.append((i, p.vertex((edges[i] + 1) % len(p.vertices()))))
+        i, vert_i = vertices[-1]
+        vert_i = vert_i - v
+        j, vert_j = vertices[0]
+        if vert_i != vert_j:
+            li = labels[i]
+            li = (li[0], SG(-v) * li[1])
+            lio = ss.opposite_edge(li, edges[i])
+            lj = labels[j]
+            sc = SaddleConnection(
+                s,
+                (lj[0], (edges[j] + 1) % len(ss.polygon(lj).vertices())),
+                (~lj[1])(vert_i) - (~lj[1])(vert_j),
+            )
+            sc_set_left.add(sc)
+        i = j
+        vert_i = vert_j
+        for j, vert_j in vertices[1:]:
+            if vert_i != vert_j:
+                li = labels[i]
+                lio = ss.opposite_edge(li, edges[i])
+                lj = labels[j]
+                sc = SaddleConnection(
+                    s,
+                    (lj[0], (edges[j] + 1) % len(ss.polygon(lj).vertices())),
+                    (~lj[1])(vert_i) - (~lj[1])(vert_j),
+                )
+                sc_set_left.add(sc)
+            i = j
+            vert_i = vert_j
+        self._boundary1 = frozenset(sc_set_right)
+        self._boundary2 = frozenset(sc_set_left)
+        self._boundary = frozenset(self._boundary1.union(self._boundary2))
+
+        edge_intersections = []
+        i = min_list[0]
+        label = labels[i]
+        p = ss.polygon(label)
+        right_point = p.vertex(edges[i])  # point on the right boundary
+        i = max_list[0]
+        label = labels[i]
+        p = ss.polygon(label)
+        left_point = p.vertex((edges[i] + 1) % len(p.vertices()))
+        from flatsurf.geometry.euclidean import solve
+
+        for i in range(len(edges)):
+            label = labels[i]
+            p = ss.polygon(label)
+            e = edges[i]
+            v1 = p.vertex(e)
+            v2 = p.vertex((e + 1) % len(p.vertices()))
+            a, b = solve(left_point, v, v1, v2 - v1)
+            w1 = (~(label[1]))(v1 + b * (v2 - v1))
+            a, b = solve(right_point, v, v1, v2 - v1)
+            w2 = (~(label[1]))(v1 + b * (v2 - v1))
+            edge_intersections.append((w1, w2))
+
+        polygons = []
+        pair1 = edge_intersections[-1]
+        l1 = labels[-2][0]
+        e1 = edges[-1]
+        for i in range(len(edges)):
+            l2 = labels[i][0]
+            pair2 = edge_intersections[i]
+            e2 = edges[i]
+            trans = s.edge_transformation(l1, e1)
+            pair1p = (trans(pair1[0]), trans(pair1[1]))
+            polygon_verts = [pair1p[0], pair1p[1]]
+            if pair2[1] != pair1p[1]:
+                polygon_verts.append(pair2[1])
+            if pair2[0] != pair1p[0]:
+                polygon_verts.append(pair2[0])
 
-            sage: from flatsurf import translation_surfaces
+            from flatsurf import Polygon
+
+            polygons.append(
+                (l2, Polygon(vertices=polygon_verts, base_ring=s.base_ring()))
+            )
+            l1 = l2
+            pair1 = pair2
+            e1 = e2
+        self._polygons = tuple(polygons)
 
-            sage: S = SymmetricGroup(3)
-            sage: r = S('(1,2)')
-            sage: u = S('(1,3)')
-            sage: o = translation_surfaces.origami(r,u)
-            sage: o.underlying_surface()
-            Origami defined by r=(1,2) and u=(1,3)
-            sage: o.stratum()
-            H_2(2)
-            sage: TestSuite(o).run()
+    def surface(self):
+        return self._surface
+
+    def initial_label(self):
+        r"""
+        Return one label on the surface that the cylinder passes through.
         """
-        from .translation_surface import Origami
-        return TranslationSurface(Origami(r,u,rr,uu,domain))
+        return self._label0
 
-    @staticmethod
-    def infinite_staircase():
+    def edges(self):
         r"""
-        Return the infinite staircase built as an origami.
+        Return a tuple of edge numbers representing the edges crossed
+        when the cylinder leaves the polygon with `initial_label` until
+        it returns by closing.
+        """
+        return self._edges
 
-        EXAMPLES::
+    def boundary(self):
+        r"""
+        Return the set of saddle connections in the boundary, oriented so that
+        the surface is on the left.
+        """
+        return self._boundary
 
-            sage: from flatsurf import translation_surfaces
+    def polygons(self):
+        r"""
+        Return a list of pairs each consisting of a label and a polygon.
+        Each polygon represents a sub-polygon of the polygon on the surface
+        with the given label. The union of these sub-polygons form the
+        cylinder. The subpolygons are listed in cyclic order.
+        """
+        return self._polygons
 
-            sage: S = translation_surfaces.infinite_staircase()
-            sage: S.underlying_surface()
-            The infinite staircase
-            sage: TestSuite(S).run(skip='_test_pickling')
-        """
-        from .translation_surface import Origami
-        o = Origami(
-                lambda x: x+1 if x%2 else x-1,  # r  (edge 1)
-                lambda x: x-1 if x%2 else x+1,  # u  (edge 2)
-                lambda x: x+1 if x%2 else x-1,  # rr (edge 3)
-                lambda x: x-1 if x%2 else x+1,  # uu (edge 0)
-                domain = ZZ,
-                base_label=ZZ(0))
-        o.rename("The infinite staircase")
-        s = TranslationSurface(o)
-        from flatsurf.geometry.similarity import SimilarityGroup
-        SG = SimilarityGroup(QQ)
-        def pos(n):
-            if n%2 == 0:
-                return SG((n/2,n/2))
-            else:
-                return SG((n//2,n//2+1))
-        gs=s.graphical_surface(default_position_function = pos)
-        gs.make_all_visible(limit = 10)
-        return s
+    @cached_method
+    def area(self):
+        r"""
+        Return the area of this cylinder if it is contained in a ConeSurface.
+        """
+        from flatsurf.geometry.categories import ConeSurfaces
 
-    @staticmethod
-    def t_fractal(w=ZZ_1, r=ZZ_2, h1=ZZ_1, h2=ZZ_1):
+        if self._surface not in ConeSurfaces():
+            raise NotImplementedError("area only makes sense for cone surfaces")
+
+        area = 0
+        for label, p in self.polygons():
+            area += p.area()
+        return area
+
+    def plot(self, **options):
         r"""
-        Return the T-fractal with parameters ``w``, ``r``, ``h1``, ``h2``.
+        Plot this cylinder in coordinates used by a graphical surface. This
+        plots this cylinder as a union of subpolygons. Only the intersections
+        with polygons visible in the graphical surface are shown.
 
-        EXAMPLES::
+        Parameters other than `graphical_surface` are passed to `polygon2d`
+        which is called to render the polygons.
 
-            sage: from flatsurf import translation_surfaces
-            sage: tf = translation_surfaces.t_fractal().underlying_surface()
-            sage: tf
-            The T-fractal surface with parameters w=1, r=2, h1=1, h2=1
-            sage: TestSuite(tf).run(skip='_test_pickling')
+        Parameters
+        ----------
+        graphical_surface : a GraphicalSurface
+            If not provided or `None`, the plot method uses the default graphical
+            surface for the surface.
         """
-        return tfractal_surface(w,r,h1,h2)
+        if "graphical_surface" in options and options["graphical_surface"] is not None:
+            gs = options["graphical_surface"]
+            if gs.get_surface() != self._surface:
+                raise ValueError("graphical surface for the wrong surface")
+            del options["graphical_surface"]
+        else:
+            gs = self._surface.graphical_surface()
+        plt = Graphics()
+        for label, p in self.polygons():
+            if gs.is_visible(label):
+                gp = gs.graphical_polygon(label)
+                t = gp.transformation()
+                pp = t(p)
+                poly = polygon2d(pp.vertices(), **options)
+                plt += poly.plot()
+        return plt
 
-    @staticmethod
-    def e_infinity_surface(lambda_squared=None, field=None):
+    @cached_method
+    def labels(self):
         r"""
-        The translation surface based on the $E_\infinity$ graph.
+        Return the set of labels that this cylinder passes through.
+        """
+        polygons = self.polygons()
+        return frozenset([label for label, p in polygons])
 
-        The biparite graph is shown below, with edges numbered:
+    def boundary_components(self):
+        r"""
+        Return a set of two elements: the set of saddle connections on
+        the right and left sides. Saddle connections are oriented so that
+        the surface is on the left.
+        """
+        return frozenset([self._boundary1, self._boundary2])
 
-          0   1   2  -2   3  -3   4  -4
-        *---o---*---o---*---o---*---o---*...
-                |
-                |-1
-                o
+    def next(self, sc):
+        r"""
+        Return the next saddle connection as you move around the cylinder boundary
+        moving from sc in the direction of its orientation.
+        """
+        if sc not in self._boundary:
+            raise ValueError
 
-        Here, black vertices are colored *, and white o.
-        Black nodes represent vertical cylinders and white nodes
-        represent horizontal cylinders.
+        v = sc.end_tangent_vector()
+        v = v.clockwise_to(-v.vector())
+        from flatsurf.geometry.euclidean import is_parallel
 
-        EXAMPLES::
+        for sc2 in self._boundary:
+            if sc2.start_data() == (
+                v.polygon_label(),
+                v.vertex(),
+            ) and is_parallel(sc2.direction(), v.vector()):
+                return sc2
+        raise ValueError("Failed to find next saddle connection in boundary set.")
 
-            sage: from flatsurf import *
-            sage: s = translation_surfaces.e_infinity_surface()
-            sage: TestSuite(s).run(skip='_test_pickling')
+    def previous(self, sc):
+        r"""
+        Return the previous saddle connection as you move around the cylinder boundary
+        moving from sc in the direction opposite its orientation.
         """
-        return TranslationSurface(EInfinitySurface(lambda_squared, field))
+        if sc not in self._boundary:
+            raise ValueError
+        v = sc.start_tangent_vector()
+        v = v.counterclockwise_to(-v.vector())
+        from flatsurf.geometry.euclidean import is_parallel
 
+        for sc2 in self._boundary:
+            if sc2.end_data() == (v.polygon_label(), v.vertex()) and is_parallel(
+                sc2.end_direction(), v.vector()
+            ):
+                return sc2
+        raise ValueError("Failed to find previous saddle connection in boundary set.")
 
-    @staticmethod
-    def chamanara(alpha):
+    @cached_method
+    def holonomy(self):
         r"""
-        Return the Chamanara surface with parameter ``alpha``.
+        In a translation surface, return one of the two holonomy vectors of the cylinder,
+        which differ by a sign.
+        """
+        from flatsurf.geometry.categories import TranslationSurfaces
 
-        EXAMPLES::
+        if self._surface not in TranslationSurfaces():
+            raise NotImplementedError(
+                "holonomy currently only computable for translation surfaces"
+            )
 
-            sage: from flatsurf import translation_surfaces
-            sage: C = translation_surfaces.chamanara(1/2)
-            sage: C
-            TranslationSurface built from infinitely many polygons
-            sage: TestSuite(C).run(skip='_test_pickling')
-        """
-        from .chamanara import chamanara_surface
-        return chamanara_surface(alpha)
+        V = self._surface.base_ring() ** 2
+        total = V.zero()
+        for sc in self._boundary1:
+            total += sc.holonomy()
+
+        # Debugging:
+        total2 = V.zero()
+        for sc in self._boundary2:
+            total2 += sc.holonomy()
+        assert (
+            total + total2 == V.zero()
+        ), "Holonomy of the two boundary components should sum to zero."
+
+        return total
+
+    @cached_method
+    def circumference(self):
+        r"""
+        In a cone surface, return the circumference, i.e., the length
+        of a geodesic loop running around the cylinder. Since this may
+        not lie in the field of definition of the surface, it is returned
+        as an element of the Algebraic Real Field.
+        """
+        from flatsurf.geometry.categories import ConeSurfaces
+
+        if self._surface not in ConeSurfaces():
+            raise NotImplementedError(
+                "circumference only makes sense for cone surfaces"
+            )
 
-translation_surfaces = TranslationSurfaceGenerators()
+        total = 0
+        for sc in self._boundary1:
+            total += sc.length()
+        return total
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/straight_line_trajectory.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/straight_line_trajectory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,44 @@
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
-from six import iteritems
+# *********************************************************************
+#  This file is part of sage-flatsurf.
+#
+#        Copyright (C) 2016-2022 W. Patrick Hooper
+#                      2016-2022 Vincent Delecroix
+#                           2023 Julian Rüth
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+# *********************************************************************
+from collections import deque
 
-from collections import deque, defaultdict
-
-from .polygon import is_same_direction, line_intersection
-from .surface_objects import SaddleConnection
+from flatsurf.geometry.euclidean import line_intersection
+from flatsurf.geometry.surface_objects import SaddleConnection
 
 # Vincent question:
 # using deque has the disadvantage of losing the initial points
 # ideally doig
 #  my_line[i]
 # we should always access to the same element
 
 # I wanted to be able to flow backward thus inserting at the beginning of a list.
 # Perhaps it would be better to model this on a deque-like class that is indexed by
 # all integers rather than just the non-negative ones? Do you know of such
 # a class? Alternately, we could store an offset.
 
+
 def get_linearity_coeff(u, v):
     r"""
     Given the two 2-dimensional vectors ``u`` and ``v``, return ``a`` so that
     ``v = a*u``
 
     If the vectors are not colinear, a ``ValueError`` is raised.
 
@@ -43,71 +60,90 @@
 
         sage: get_linearity_coeff(V((1,1)), V((-1,1)))
         Traceback (most recent call last):
         ...
         ValueError: non colinear
     """
     if u[0]:
-        a = v[0]/u[0]
-        if v[1] != a*u[1]:
+        a = v[0] / u[0]
+        if v[1] != a * u[1]:
             raise ValueError("non colinear")
         return a
     elif v[0]:
         raise ValueError("non colinear")
     elif u[1]:
-        return v[1]/u[1]
+        return v[1] / u[1]
     else:
         raise ValueError("zero vector")
 
+
 class SegmentInPolygon:
     r"""
     Maximal segment in a polygon of a similarity surface
 
     EXAMPLES::
 
-        sage: from flatsurf import *
+        sage: from flatsurf import similarity_surfaces
         sage: from flatsurf.geometry.straight_line_trajectory import SegmentInPolygon
         sage: s = similarity_surfaces.example()
         sage: v = s.tangent_vector(0, (1/3,-1/4), (0,1))
         sage: SegmentInPolygon(v)
         Segment in polygon 0 starting at (1/3, -1/3) and ending at (1/3, 0)
     """
+
     def __init__(self, start, end=None):
-        if not end is None:
+        if end is not None:
             # WARNING: here we assume that both start and end are on the
             # boundary
             self._start = start
             self._end = end
         else:
             self._end = start.forward_to_polygon_boundary()
             self._start = self._end.forward_to_polygon_boundary()
 
+    def __hash__(self):
+        r"""
+        TESTS::
+
+            sage: from flatsurf import similarity_surfaces
+            sage: from flatsurf.geometry.straight_line_trajectory import SegmentInPolygon
+            sage: s = similarity_surfaces.example()
+            sage: v = s.tangent_vector(0, (1/3,-1/4), (0,1))
+            sage: h = hash(SegmentInPolygon(v))
+        """
+        return hash((self._start, self._end))
+
     def __eq__(self, other):
-        return type(self) is type(other) and \
-               self._start == other._start and \
-               self._end == other._end
+        return (
+            type(self) is type(other)
+            and self._start == other._start
+            and self._end == other._end
+        )
 
     def __ne__(self, other):
-        return type(self) is not type(other) or \
-               self._start != other._start or \
-               self._end != other._end
+        return (
+            type(self) is not type(other)
+            or self._start != other._start
+            or self._end != other._end
+        )
 
     def __repr__(self):
         r"""
         TESTS::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import similarity_surfaces
             sage: from flatsurf.geometry.straight_line_trajectory import SegmentInPolygon
             sage: s = similarity_surfaces.example()
             sage: v = s.tangent_vector(0, (0,0), (3,-1))
             sage: SegmentInPolygon(v)
             Segment in polygon 0 starting at (0, 0) and ending at (2, -2/3)
         """
         return "Segment in polygon {} starting at {} and ending at {}".format(
-                self.polygon_label(), self.start().point(), self.end().point())
+            self.polygon_label(), self.start().point(), self.end().point()
+        )
 
     def start(self):
         r"""
         Return the tangent vector associated to the start of a trajectory pointed forward.
         """
         return self._start
 
@@ -122,19 +158,20 @@
 
     def end_is_singular(self):
         return self._end.is_based_at_singularity()
 
     def is_edge(self):
         if not self.start_is_singular() or not self.end_is_singular():
             return False
-        vv=self.start().vector()
-        vertex=self.start().vertex()
-        ww=self.start().polygon().edge(vertex)
-        from flatsurf.geometry.polygon import is_same_direction
-        return is_same_direction(vv,ww)
+        vv = self.start().vector()
+        vertex = self.start().vertex()
+        ww = self.start().polygon().edge(vertex)
+        from flatsurf.geometry.euclidean import is_parallel
+
+        return is_parallel(vv, ww)
 
     def edge(self):
         if not self.is_edge():
             raise ValueError("Segment asked for edge when not an edge")
         return self.start().vertex()
 
     def polygon_label(self):
@@ -145,22 +182,22 @@
 
     def next(self):
         r"""
         Return the next segment obtained by continuing straight through the end point.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import similarity_surfaces
             sage: from flatsurf.geometry.straight_line_trajectory import SegmentInPolygon
 
             sage: s = similarity_surfaces.example()
             sage: s.polygon(0)
-            Polygon: (0, 0), (2, -2), (2, 0)
+            Polygon(vertices=[(0, 0), (2, -2), (2, 0)])
             sage: s.polygon(1)
-            Polygon: (0, 0), (2, 0), (1, 3)
+            Polygon(vertices=[(0, 0), (2, 0), (1, 3)])
             sage: v = s.tangent_vector(0, (0,0), (3,-1))
             sage: seg = SegmentInPolygon(v)
             sage: seg
             Segment in polygon 0 starting at (0, 0) and ending at (2, -2/3)
             sage: seg.next()
             Segment in polygon 1 starting at (2/3, 2) and ending at (14/9, 4/3)
         """
@@ -170,136 +207,136 @@
 
     def previous(self):
         if self.end_is_singular():
             raise ValueError("Cannot continue from singularity")
         return SegmentInPolygon(self._start.invert()).invert()
 
 
-    # DEPRECATED STUFF THAT WILL BE REMOVED
+class AbstractStraightLineTrajectory:
+    def surface(self):
+        raise NotImplementedError
 
-    def start_point(self):
-        from sage.misc.superseded import deprecation
-        deprecation(1, "do not use start_point but start().point()")
-        return self._start.point()
-
-    def start_direction(self):
-        from sage.misc.superseded import deprecation
-        deprecation(1, "do not use start_direction but start().vector()")
-        return self._start.vector()
-
-    def end_point(self):
-        from sage.misc.superseded import deprecation
-        deprecation(1, "do not use end_point but end().point()")
-        return self._end.point()
-
-    def end_direction(self):
-        from sage.misc.superseded import deprecation
-        deprecation(1, "do not use end_direction but end().vector()")
-        return self._end.vector()
+    def combinatorial_length(self):
+        raise NotImplementedError
 
-class AbstractStraightLineTrajectory:
-    r"""
-    You need to implement:
+    def segment(self, i):
+        raise NotImplementedError
 
-    - ``def segment(self, i)``
-    - ``def segments(self)``
-    """
-    def surface(self):
+    def is_closed(self):
+        raise NotImplementedError
+
+    def segments(self):
         raise NotImplementedError
 
     def __repr__(self):
         start = self.segment(0).start()
         end = self.segment(-1).end()
         return "Straight line trajectory made of {} segments from {} in polygon {} to {} in polygon {}".format(
-                self.combinatorial_length(),
-                start.point(), start.polygon_label(),
-                end.point(), end.polygon_label())
+            self.combinatorial_length(),
+            start.point(),
+            start.polygon_label(),
+            end.point(),
+            end.polygon_label(),
+        )
 
     def plot(self, *args, **options):
         r"""
         Plot this trajectory by converting to a graphical trajectory.
 
-        If any arguments are provided in `*args` it must be only one argument containing a GraphicalSurface.
-        The keyword arguments in `**options` are passed on to :func:`GraphicalStraightLineTrajectory.plot`.
+        If any arguments are provided in `*args` it must be only one argument
+        containing a GraphicalSurface. The keyword arguments in `**options` are
+        passed on to
+        :func:`flatsurf.graphical.straight_line_trajectory.GraphicalStraightLineTrajectory.plot`.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: T = translation_surfaces.square_torus()
             sage: v = T.tangent_vector(0, (0,0), (5,7))
             sage: L = v.straight_line_trajectory()
-            sage: L.plot()               # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 1 graphics primitive
-            sage: L.plot(color='red')    # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 1 graphics primitive
+            sage: L.plot()
+            ...Graphics object consisting of 1 graphics primitive
+            sage: L.plot(color='red')
+            ...Graphics object consisting of 1 graphics primitive
         """
         if len(args) > 1:
-            raise ValueError("SimilaritySurface.plot() can take at most one non-keyword argument.")
-        if len(args)==1:
+            raise ValueError(
+                "SimilaritySurface.plot() can take at most one non-keyword argument."
+            )
+        if len(args) == 1:
             from flatsurf.graphical.surface import GraphicalSurface
+
             if not isinstance(args[0], GraphicalSurface):
-                raise ValueError("If an argument is provided, it must be a GraphicalSurface.")
-            return self.graphical_trajectory(graphical_surface = args[0]).plot(**options)
+                raise ValueError(
+                    "If an argument is provided, it must be a GraphicalSurface."
+                )
+            return self.graphical_trajectory(graphical_surface=args[0]).plot(**options)
         return self.graphical_trajectory().plot(**options)
 
     def graphical_trajectory(self, graphical_surface=None, **options):
         r"""
         Returns a ``GraphicalStraightLineTrajectory`` corresponding to this
         trajectory in the provided  ``GraphicalSurface``.
         """
-        from flatsurf.graphical.straight_line_trajectory import GraphicalStraightLineTrajectory
+        from flatsurf.graphical.straight_line_trajectory import (
+            GraphicalStraightLineTrajectory,
+        )
+
         if graphical_surface is None:
             graphical_surface = self.surface().graphical_surface()
         return GraphicalStraightLineTrajectory(self, graphical_surface, **options)
 
     def cylinder(self):
         r"""
         If this is a closed orbit, return the associated maximal cylinder.
         Raises a ValueError if this trajectory is not closed.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: s = translation_surfaces.regular_octagon()
             sage: v = s.tangent_vector(0,(1/2,0),(sqrt(2),1))
             sage: traj = v.straight_line_trajectory()
             sage: traj.flow(4)
             sage: traj.is_closed()
             True
             sage: cyl = traj.cylinder()
             sage: cyl.area()                # a = sqrt(2)
             a + 1
             sage: cyl.holonomy()
             (3*a + 4, 2*a + 3)
             sage: cyl.edges()
             (2, 3, 3, 2, 4)
         """
-        # Note may not be defined.
+        # Note: may not be defined.
         if not self.is_closed():
-            raise ValueError("Cylinder is only defined for closed straight-line trajectories.")
+            raise ValueError(
+                "Cylinder is only defined for closed straight-line trajectories."
+            )
         from .surface_objects import Cylinder
+
         coding = self.coding()
         label = coding[0][0]
-        edges = [ e for l,e in coding[1:] ]
-        edges.append(self.surface().opposite_edge(coding[0][0],coding[0][1])[1])
+        edges = [e for _, e in coding[1:]]
+        edges.append(self.surface().opposite_edge(coding[0][0], coding[0][1])[1])
         return Cylinder(self.surface(), label, edges)
 
     def coding(self, alphabet=None):
         r"""
         Return the coding of this trajectory with respect to the sides of the
         polygons
 
         INPUT:
 
         - ``alphabet`` -- an optional dictionary ``(lab,nb) -> letter``. If some
           labels are avoided then these crossings are ignored.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: t = translation_surfaces.square_torus()
 
             sage: v = t.tangent_vector(0, (1/2,0), (5,6))
             sage: l = v.straight_line_trajectory()
             sage: alphabet = {(0,0): 'a', (0,1): 'b', (0,2):'a', (0,3): 'b'}
             sage: l.coding()
             [(0, 0), (0, 1)]
@@ -327,106 +364,116 @@
             True
             sage: l.coding(alphabet)
             ['a', 'b']
 
         Check that the saddle connections that are obtained in the torus get the
         expected coding::
 
-            sage: for _ in range(10):
+            sage: for _ in range(10):  # long time (.6s)
             ....:     x = ZZ.random_element(1,30)
             ....:     y = ZZ.random_element(1,30)
             ....:     x,y = x/gcd(x,y), y/gcd(x,y)
             ....:     v = t.tangent_vector(0, (0,0), (x,y))
             ....:     l = v.straight_line_trajectory()
             ....:     l.flow(200); l.flow(-200)
             ....:     w = ''.join(l.coding(alphabet))
             ....:     assert Word(w+'ab'+w).is_balanced()
             ....:     assert Word(w+'ba'+w).is_balanced()
             ....:     assert w.count('a') == y-1
             ....:     assert w.count('b') == x-1
         """
-        ans = []
+        coding = []
 
         segments = self.segments()
 
         s = segments[0]
         start = s.start()
         if start._position._position_type == start._position.EDGE_INTERIOR:
             p = s.polygon_label()
             e = start._position.get_edge()
-            lab = (p,e) if alphabet is None else alphabet.get((p,e))
+            lab = (p, e) if alphabet is None else alphabet.get((p, e))
             if lab is not None:
-                ans.append(lab)
+                coding.append(lab)
 
-        for i in range(len(segments)-1):
+        for i in range(len(segments) - 1):
             s = segments[i]
             end = s.end()
             p = s.polygon_label()
             e = end._position.get_edge()
-            lab = (p,e) if alphabet is None else alphabet.get((p,e))
+            lab = (p, e) if alphabet is None else alphabet.get((p, e))
             if lab is not None:
-                ans.append(lab)
+                coding.append(lab)
 
         s = segments[-1]
         end = s.end()
-        if end._position._position_type == end._position.EDGE_INTERIOR and \
-           end.invert() != start:
+        if (
+            end._position._position_type == end._position.EDGE_INTERIOR
+            and end.invert() != start
+        ):
             p = s.polygon_label()
             e = end._position.get_edge()
-            lab = (p,e) if alphabet is None else alphabet.get((p,e))
+            lab = (p, e) if alphabet is None else alphabet.get((p, e))
             if lab is not None:
-                ans.append(lab)
+                coding.append(lab)
 
-        return ans
+        return coding
 
     def initial_tangent_vector(self):
         return self.segment(0).start()
 
     def terminal_tangent_vector(self):
         return self.segment(-1).end()
 
-    def intersects(self, traj, count_singularities = False):
+    def intersects(self, traj, count_singularities=False):
         r"""
         Return true if this trajectory intersects the other trajectory.
         """
         try:
-            next(self.intersections(traj, count_singularities = count_singularities))
+            next(self.intersections(traj, count_singularities=count_singularities))
         except StopIteration:
             return False
         return True
 
-    def intersections(self, traj, count_singularities = False, include_segments = False):
+    def intersections(self, traj, count_singularities=False, include_segments=False):
         r"""
         Return the set of SurfacePoints representing the intersections
         of this trajectory with the provided trajectory or SaddleConnection.
 
         Singularities will be included only if count_singularities is
         set to True.
 
         If include_segments is True, it iterates over triples consisting of the SurfacePoint,
         and two sets. The first set consists of segments of this trajectory that contain the point
         and the second set consists of segments of traj that contain the point.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
-            sage: s=translation_surfaces.square_torus()
+            sage: from flatsurf import translation_surfaces
+            sage: s = translation_surfaces.square_torus()
             sage: traj1 = s.tangent_vector(0,(1/2,0),(1,1)).straight_line_trajectory()
             sage: traj1.flow(3)
             sage: traj1.is_closed()
             True
             sage: traj2 = s.tangent_vector(0,(1/2,0),(-1,1)).straight_line_trajectory()
             sage: traj2.flow(3)
             sage: traj2.is_closed()
             True
             sage: sum(1 for _ in traj1.intersections(traj2))
             2
+
+            sage: for p, (segs1, segs2) in traj1.intersections(traj2, include_segments=True):
+            ....:     print(p)
+            ....:     print(len(segs1), len(segs2))
+            Point (1/2, 0) of polygon 0
+            2 2
+            Point (0, 1/2) of polygon 0
+            2 2
         """
         # Partition the segments making up the trajectories by label.
-        if isinstance(traj,SaddleConnection):
+        if isinstance(traj, SaddleConnection):
             traj = traj.trajectory()
         lab_to_seg1 = {}
         for seg1 in self.segments():
             label = seg1.polygon_label()
             if label in lab_to_seg1:
                 lab_to_seg1[label].append(seg1)
             else:
@@ -436,81 +483,90 @@
             label = seg2.polygon_label()
             if label in lab_to_seg2:
                 lab_to_seg2[label].append(seg2)
             else:
                 lab_to_seg2[label] = [seg2]
         intersection_points = set()
         if include_segments:
-            segments={}
-        for label,seg_list_1 in iteritems(lab_to_seg1):
+            segments = {}
+        for label, seg_list_1 in lab_to_seg1.items():
             if label in lab_to_seg2:
                 seg_list_2 = lab_to_seg2[label]
                 for seg1 in seg_list_1:
                     for seg2 in seg_list_2:
-                        x = line_intersection(seg1.start().point(),
-                                              seg1.start().point()+seg1.start().vector(),
-                                              seg2.start().point(),
-                                              seg2.start().point()+seg2.start().vector())
+                        x = line_intersection(
+                            seg1.start().point(),
+                            seg1.start().point() + seg1.start().vector(),
+                            seg2.start().point(),
+                            seg2.start().point() + seg2.start().vector(),
+                        )
                         if x is not None:
-                            pos = self._s.polygon(seg1.polygon_label()).get_point_position(x)
-                            if pos.is_inside() and (count_singularities or not pos.is_vertex()):
-                                new_point = self._s.surface_point(seg1.polygon_label(),x)
+                            pos = (
+                                self.surface()
+                                .polygon(seg1.polygon_label())
+                                .get_point_position(x)
+                            )
+                            if pos.is_inside() and (
+                                count_singularities or not pos.is_vertex()
+                            ):
+                                new_point = self.surface().point(
+                                    seg1.polygon_label(), x
+                                )
                                 if new_point not in intersection_points:
                                     intersection_points.add(new_point)
                                     if include_segments:
-                                        segments[new_point]=({seg1},{seg2})
+                                        segments[new_point] = ({seg1}, {seg2})
                                     else:
                                         yield new_point
                                 elif include_segments:
-                                    segments[new_point][0].append(seg1)
-                                    segments[new_point][1].append(seg2)
+                                    segments[new_point][0].add(seg1)
+                                    segments[new_point][1].add(seg2)
         if include_segments:
-            for x in iteritems(segments):
-                yield x
-
+            yield from segments.items()
 
 
 class StraightLineTrajectory(AbstractStraightLineTrajectory):
     r"""
     Straight-line trajectory in a similarity surface.
 
     EXAMPLES::
 
         # Demonstrate the handling of edges
-        sage: from flatsurf import *
+        sage: from flatsurf import translation_surfaces
         sage: from flatsurf.geometry.straight_line_trajectory import StraightLineTrajectory
         sage: p = SymmetricGroup(2)('(1,2)')
         sage: s = translation_surfaces.origami(p,p)
         sage: traj = StraightLineTrajectory(s.tangent_vector(1,(0,0),(1,0)))
         sage: traj
         Straight line trajectory made of 1 segments from (0, 0) in polygon 1 to (1, 1) in polygon 2
         sage: traj.is_saddle_connection()
         True
         sage: traj2 = StraightLineTrajectory(s.tangent_vector(1,(0,0),(0,1)))
         sage: traj2
         Straight line trajectory made of 1 segments from (1, 0) in polygon 2 to (0, 1) in polygon 1
         sage: traj2.is_saddle_connection()
         True
     """
+
     def __init__(self, tangent_vector):
         self._segments = deque()
         seg = SegmentInPolygon(tangent_vector)
         self._segments.append(seg)
         self._setup_forward()
         self._setup_backward()
-        self._s=tangent_vector.surface()
+        self._s = tangent_vector.surface()
 
     def surface(self):
         return self._s
 
     def segment(self, i):
         r"""
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
 
             sage: O = translation_surfaces.regular_octagon()
             sage: v = O.tangent_vector(0, (1,1), (33,45))
             sage: L = v.straight_line_trajectory()
             sage: L.segment(0)
             Segment in polygon 0 starting at (4/15, 0) and ending at (11/26*a +
             1, 15/26*a + 1)
@@ -565,21 +621,23 @@
 
             :meth:`is_saddle_connection`
 
         EXAMPLES:
 
         An example in a cone surface covered by the torus::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import MutableOrientedSimilaritySurface, polygons
             sage: p = polygons.square()
-            sage: s = Surface_list(base_ring=p.base_ring())
-            sage: s.add_polygon(p,[(0,3),(0,2),(0,1),(0,0)])
+            sage: s = MutableOrientedSimilaritySurface(p.base_ring())
+            sage: s.add_polygon(p)
             0
+            sage: s.glue((0, 0), (0, 3))
+            sage: s.glue((0, 1), (0, 2))
             sage: s.set_immutable()
-            sage: t = RationalConeSurface(s)
+            sage: t = s
 
             sage: v = t.tangent_vector(0, (1/2,0), (1/3,7/5))
             sage: l = v.straight_line_trajectory()
             sage: l.is_closed()
             False
             sage: l.flow(100)
             sage: l.is_closed()
@@ -592,52 +650,53 @@
             False
             sage: l.is_saddle_connection()
             False
             sage: l.flow(-100)
             sage: l.is_saddle_connection()
             True
         """
-        return (not self.is_forward_separatrix()) and \
-            self._forward.differs_by_scaling(self.initial_tangent_vector())
+        return (not self.is_forward_separatrix()) and self._forward.differs_by_scaling(
+            self.initial_tangent_vector()
+        )
 
     def flow(self, steps):
         r"""
-        Append or preprend segments to the trajectory.
+        Append or prepend segments to the trajectory.
         If steps is positive, attempt to append this many segments.
         If steps is negative, attempt to prepend this many segments.
         Will fail gracefully the trajectory hits a singularity or closes up.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import similarity_surfaces
 
             sage: s = similarity_surfaces.example()
             sage: v = s.tangent_vector(0, (1,-1/2), (3,-1))
             sage: traj = v.straight_line_trajectory()
             sage: traj
             Straight line trajectory made of 1 segments from (1/4, -1/4) in polygon 0 to (2, -5/6) in polygon 0
             sage: traj.flow(1)
             sage: traj
             Straight line trajectory made of 2 segments from (1/4, -1/4) in polygon 0 to (61/36, 11/12) in polygon 1
             sage: traj.flow(-1)
             sage: traj
             Straight line trajectory made of 3 segments from (15/16, 45/16) in polygon 1 to (61/36, 11/12) in polygon 1
         """
-        while steps>0 and \
-            (not self.is_forward_separatrix()) and \
-            (not self.is_closed()):
-                self._segments.append(SegmentInPolygon(self._forward))
-                self._setup_forward()
-                steps -= 1
-        while steps<0 and \
-            (not self.is_backward_separatrix()) and \
-            (not self.is_closed()):
-                self._segments.appendleft(SegmentInPolygon(self._backward).invert())
-                self._setup_backward()
-                steps += 1
+        while (
+            steps > 0 and (not self.is_forward_separatrix()) and (not self.is_closed())
+        ):
+            self._segments.append(SegmentInPolygon(self._forward))
+            self._setup_forward()
+            steps -= 1
+        while (
+            steps < 0 and (not self.is_backward_separatrix()) and (not self.is_closed())
+        ):
+            self._segments.appendleft(SegmentInPolygon(self._backward).invert())
+            self._setup_backward()
+            steps += 1
 
 
 class StraightLineTrajectoryTranslation(AbstractStraightLineTrajectory):
     r"""
     Straight line trajectory in a translation surface.
 
     This is similar to :class:`StraightLineTrajectory` but implemented using
@@ -650,18 +709,17 @@
 
     - ``e`` is the number of some edge in ``p``
 
     - ``x`` is the position of the point in ``e`` (be careful that it is not
       necessarily a number between 0 and 1. It is given relatively to the length
       of the induced interval in the iet)
 
-    (see the methods :meth:`_prev` and :meth:`_next`)
     """
+
     def __init__(self, tangent_vector):
-        t = tangent_vector.polygon_label()
         self._vector = tangent_vector.vector()
         self._s = tangent_vector.surface()
 
         seg = SegmentInPolygon(tangent_vector)
         if seg.is_edge():
             self._points = None
             self._edge = seg
@@ -676,28 +734,29 @@
         else:
             raise RuntimeError("PROBLEM!")
 
         p = start.polygon_label()
         poly = self._s.polygon(p)
 
         T = self._get_iet(p)
-        x = get_linearity_coeff(poly.vertex(i+1) - poly.vertex(i),
-                                start.point() - poly.vertex(i))
+        x = get_linearity_coeff(
+            poly.vertex(i + 1) - poly.vertex(i), start.point() - poly.vertex(i)
+        )
         x *= T.length_bot(i)
 
-        self._points = deque() # we store triples (lab, edge, rel_pos)
+        self._points = deque()  # we store triples (lab, edge, rel_pos)
         self._points.append((p, i, x))
 
     def _next(self, p, e, x):
         r"""
         Return the image of ``(p, e, x)``
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: from flatsurf.geometry.straight_line_trajectory import StraightLineTrajectoryTranslation
             sage: S = SymmetricGroup(3)
             sage: r = S('(1,2)')
             sage: u = S('(1,3)')
             sage: o = translation_surfaces.origami(r,u)
             sage: v = o.tangent_vector(1, (1/3,1/7), (5,13))
             sage: L = StraightLineTrajectoryTranslation(v)
@@ -736,15 +795,15 @@
             self._iets[polygon] = polygon.flow_map(self._vector)
         return self._iets[polygon]
 
     def segment(self, i):
         r"""
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: from flatsurf.geometry.straight_line_trajectory import StraightLineTrajectoryTranslation
 
             sage: O = translation_surfaces.regular_octagon()
             sage: v = O.tangent_vector(0, (1,1), (33,45))
             sage: L = StraightLineTrajectoryTranslation(v)
             sage: L.segment(0)
             Segment in polygon 0 starting at (4/15, 0) and ending at (11/26*a +
@@ -764,25 +823,29 @@
         iet = self._get_iet(lab)
         e1, x1 = iet.forward_image(e0, x0)
         poly = self._s.polygon(lab)
 
         l0 = iet.length_bot(e0)
         l1 = iet.length_top(e1)
 
-        point0 = poly.vertex(e0) + poly.edge(e0) * x0/l0
-        point1 = poly.vertex(e1) + poly.edge(e1) * (l1-x1)/l1
-        v0 = self._s.tangent_vector(lab, point0, self._vector, ring=self._vector.base_ring())
-        v1 = self._s.tangent_vector(lab, point1, -self._vector, ring=self._vector.base_ring())
-        return SegmentInPolygon(v0,v1)
+        point0 = poly.vertex(e0) + poly.edge(e0) * x0 / l0
+        point1 = poly.vertex(e1) + poly.edge(e1) * (l1 - x1) / l1
+        v0 = self._s.tangent_vector(
+            lab, point0, self._vector, ring=self._vector.base_ring()
+        )
+        v1 = self._s.tangent_vector(
+            lab, point1, -self._vector, ring=self._vector.base_ring()
+        )
+        return SegmentInPolygon(v0, v1)
 
     def segments(self):
         r"""
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: from flatsurf.geometry.straight_line_trajectory import StraightLineTrajectoryTranslation
 
             sage: s = translation_surfaces.square_torus()
             sage: v = s.tangent_vector(0, (0,0), (1,1+AA(5).sqrt()), ring=AA)
             sage: L = StraightLineTrajectoryTranslation(v)
             sage: L.flow(2)
             sage: L.segments()
@@ -796,25 +859,25 @@
         if self._points is None:
             raise NotImplementedError
         return self._points[0] == self._next(*self._points[-1])
 
     def is_forward_separatrix(self):
         if self._points is None:
             return True
-        p1,e1,x1 = self._next(*self._points[-1])
+        p1, e1, x1 = self._next(*self._points[-1])
         return x1.is_zero()
 
     def is_backward_separatrix(self):
         return self._points is None or self._points[0][2].is_zero()
 
     def is_saddle_connection(self):
         r"""
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: from flatsurf.geometry.straight_line_trajectory import StraightLineTrajectoryTranslation
 
             sage: torus = translation_surfaces.square_torus()
             sage: v = torus.tangent_vector(0, (1/2,1/2), (1,1))
             sage: S = StraightLineTrajectoryTranslation(v)
             sage: S.is_saddle_connection()
             True
@@ -823,15 +886,17 @@
             sage: S = StraightLineTrajectoryTranslation(v)
             sage: S.is_saddle_connection()
             False
             sage: S.flow(1)
             sage: S.is_saddle_connection()
             True
         """
-        return self._points is None or (self.is_forward_separatrix() and self.is_backward_separatrix())
+        return self._points is None or (
+            self.is_forward_separatrix() and self.is_backward_separatrix()
+        )
 
     def flow(self, steps):
         if self._points is None:
             return
         if steps > 0:
             t = self._points[-1]
             for i in range(steps):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/subfield.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/subfield.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,24 +7,45 @@
     Pierre-Vincent Koseleff, Fabrice Rouillier, Cuong Tran.
     On the Sign of a Trigonometric Expression.
     ISSAC 2015. Proceedings of the 2015 ACM International
     Symposium on Symbolic and Algebraic Computation.
     Pages 259--266.
     DOI: http://dx.doi.org/10.1145/2755996.2756664
 """
+######################################################################
+#  This file is part of sage-flatsurf.
+#
+#        Copyright (C) 2020 Samuel Lelièvre
+#                      2020 Vincent Delecroix
+#                      2023 Julian Rüth
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+######################################################################
 from sage.misc.misc_c import prod
-from sage.rings.all import ZZ, QQ, AA, QQbar, NumberField, polygen
+from sage.rings.all import ZZ, QQ, AA, NumberField, polygen
 from sage.structure.element import parent
 from sage.modules.free_module import VectorSpace
 from sage.matrix.constructor import matrix
 from sage.categories.homset import Hom
 from sage.categories.fields import Fields
 from sage.rings.qqbar import do_polred
 
-def number_field_elements_from_algebraics(elts, name='a'):
+
+def number_field_elements_from_algebraics(elts, name="a"):
     r"""
     The native Sage function ``number_field_elements_from_algebraics`` currently
     returns number field *without* embedding. This function return field with
     embedding!
 
     EXAMPLES::
 
@@ -40,22 +61,24 @@
     """
     # case when all elements are rationals
     if all(x in QQ for x in elts):
         return QQ, [QQ(x) for x in elts]
 
     # general case
     from sage.rings.qqbar import number_field_elements_from_algebraics
-    field,elts,phi = number_field_elements_from_algebraics(elts, minimal=True)
+
+    field, elts, phi = number_field_elements_from_algebraics(elts, minimal=True)
 
     polys = [x.polynomial() for x in elts]
     K = NumberField(field.polynomial(), name, embedding=AA(phi(field.gen())))
     gen = K.gen()
 
     return K, [x.polynomial()(gen) for x in elts]
 
+
 def subfield_from_elements(self, alpha, name=None, polred=True, threshold=None):
     r"""
     Return the subfield generated by the elements ``alpha``.
 
     .. NOTE::
 
         See https://trac.sagemath.org/ticket/29331
@@ -127,15 +150,15 @@
         sage: L, elts, phi = subfield_from_elements(K, [12241829/177 - 321121/22459 * sqrt5], name='b')
         sage: assert L.polynomial() == x^2 - x - 1
 
         sage: from sage.rings.qqbar import number_field_elements_from_algebraics
         sage: R.<x> = QQ[]
         sage: p1 = x^3 - x - 1
         sage: roots1 = p1.roots(QQbar, False)
-        sage: for _ in range(10):
+        sage: for _ in range(10):  # long time (1.5s)
         ....:     p2 = R.random_element(degree=2)
         ....:     while not p2.is_irreducible(): p2 = R.random_element(degree=2)
         ....:     roots2 = p2.roots(QQbar, False)
         ....:     K, (a1,b1,c1,a2,b2), phi = number_field_elements_from_algebraics(roots1 + roots2)
         ....:     u1 = 1 - a1/17 + 3/7*a1**2
         ....:     u2 = 2 + 33/35 * a1
         ....:     L, (v1,v2), phi = subfield_from_elements(K, [u1, u2], threshold=100)
@@ -159,15 +182,17 @@
     modified = True
     while modified:
         modified = False
         d = U.dimension()
         if d == self.degree():
             return (self, alpha, Hom(self, self, Fields()).identity())
         B = U.basis()
-        new_vecs = [(self(B[i]) * self(B[j])).vector() for i in range(d) for j in range(i, d)]
+        new_vecs = [
+            (self(B[i]) * self(B[j])).vector() for i in range(d) for j in range(i, d)
+        ]
         if any(vv not in U for vv in new_vecs):
             U = V.subspace(list(B) + new_vecs)
             modified = True
 
     # Strict subfield, find a generator
     vgen = None
     for b in U.basis():
@@ -200,14 +225,15 @@
 
     # need to express the elements in the basis 1, a, a^2, ..., a^(d-1)
     M = matrix(QQ, [(new_gen**i).vector() for i in range(d)])
     new_alpha = [K(M.solve_left(elt.vector())) for elt in alpha]
 
     return (K, new_alpha, hom)
 
+
 def is_embedded_subfield(K, L, certificate=False):
     r"""
     Return whether there exists a field morphism from ``K`` to ``L`` compatible with
     the embeddings.
 
     EXAMPLES::
 
@@ -249,14 +275,15 @@
     pK = P(pK)
     phi = L.coerce_embedding()
     for r in pK.roots(L, multiplicities=False):
         if phi(r) == emb:
             return (True, K.hom(L, [r])) if certificate else True
     return (False, None) if certificate else False
 
+
 def chebyshev_T(n, c):
     r"""
     Return the Chebyshev polynomial T_n so that
 
     T_n(2 cos(x)) = 2 cos(n x)
 
     .. NOTE::
@@ -281,22 +308,23 @@
         True
         sage: cos_minpoly(3, x)(chebyshev_T(5, x)) == cos_minpoly(15, x) * cos_minpoly(3, x)
         True
     """
     # T_0(x) = 2
     # T_1(x) = x
     # and T_{n+1}(x) = x T_n(x) - T_{n-1}(x)
+    T0 = parent(c)(2)
     if n == 0:
-        return parent(c)(2)
-    T0 = 2
+        return T0
     T1 = c
-    for i in range(n-1):
+    for i in range(n - 1):
         T0, T1 = T1, c * T1 - T0
     return T1
 
+
 def cos_minpoly_odd_prime(p, var):
     r"""
     (-1)^k + (-1)^{k-1} T1 + ... + T_k
 
     EXAMPLES::
 
         sage: from flatsurf.geometry.subfield import cos_minpoly_odd_prime
@@ -310,24 +338,25 @@
         sage: cos_minpoly_odd_prime(7, x)
         x^3 - x^2 - 2*x + 1
         sage: cos_minpoly_odd_prime(11, x)
         x^5 - x^4 - 4*x^3 + 3*x^2 + 3*x - 1
     """
     T0 = 2
     T1 = var
-    k = (p-1)//2
-    s = (-1)**k
-    ans = s * (1 - T1)
-    for i in range(k-1):
+    k = (p - 1) // 2
+    s = (-1) ** k
+    minpoly = s * (1 - T1)
+    for i in range(k - 1):
         T0, T1 = T1, var * T1 - T0
-        ans += s * T1
+        minpoly += s * T1
         s *= -1
-    return ans
+    return minpoly
+
 
-def cos_minpoly(n, var='x'):
+def cos_minpoly(n, var="x"):
     r"""
     Return the minimal polynomial of 2 cos pi/n
 
     Done via [KoRoTr2015]_ Algorithm 3.
 
     EXAMPLES::
 
@@ -370,24 +399,24 @@
         facs.pop(0)
     else:
         k = 0
 
     if not facs:
         # 0. n = 2^k
         # ([KoRoTr2015] Lemma 12)
-        return chebyshev_T(2**(k-1), var)
+        return chebyshev_T(2 ** (k - 1), var)
 
     # 1. Compute M_{n0} = M_{p1 ... ps}
     # ([KoRoTr2015] Lemma 14 and Lemma 15)
     M = cos_minpoly_odd_prime(facs[0][0], var)
     for i in range(1, len(facs)):
         p = facs[i][0]
         M, r = M(chebyshev_T(p, var)).quo_rem(M)
         assert r.is_zero()
 
     # 2. Compute M_{2^k p1^{a1} ... ps^{as}}
     # ([KoRoTr2015] Lemma 12)
-    nn = 2**k * prod(p**(a-1) for p,a in facs)
+    nn = 2**k * prod(p ** (a - 1) for p, a in facs)
     if nn != 1:
         M = M(chebyshev_T(nn, var))
 
     return M
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/tangent_bundle.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/tangent_bundle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,139 +1,193 @@
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
+# ********************************************************************
+#  This file is part of sage-flatsurf.
+#
+#        Copyright (C) 2016-2022 W. Patrick Hooper
+#                      2016-2022 Vincent Delecroix
+#                      2022-2023 Julian Rüth
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+# ********************************************************************
 
-from .polygon import wedge_product, is_same_direction, is_opposite_direction
+# Limit for clockwise_to and counter_clockwise_to in SimilaritySurfaceTangentVector.
+rotate_limit = 100
 
-rotate_limit=100
-r"""
-Limit for clockwise_to and counter_clockwise_to in SimilaritySurfaceTangentVector.
-"""
 
 class SimilaritySurfaceTangentVector:
     r"""
     Tangent vector to a similarity surface.
 
     EXAMPLES::
 
-        sage: from flatsurf import *
+        sage: from flatsurf import translation_surfaces
 
     Examples on edges in direction of edges::
 
         sage: s = translation_surfaces.square_torus()
-        sage: for y in [0,1]:
-        ....:     for d in [1,-1]:
-        ....:         print(s.tangent_vector(0, (1/2, y), (d, 0)))
+        sage: s.tangent_vector(0, (1/2, 0), (1, 0))
         SimilaritySurfaceTangentVector in polygon 0 based at (1/2, 0) with vector (1, 0)
+        sage: s.tangent_vector(0, (1/2, 0), (-1, 0))
         SimilaritySurfaceTangentVector in polygon 0 based at (1/2, 1) with vector (-1, 0)
+        sage: s.tangent_vector(0, (1/2, 1), (1, 0))
         SimilaritySurfaceTangentVector in polygon 0 based at (1/2, 0) with vector (1, 0)
+        sage: s.tangent_vector(0, (1/2, 1), (-1, 0))
         SimilaritySurfaceTangentVector in polygon 0 based at (1/2, 1) with vector (-1, 0)
 
-        sage: for x in [0,1]:
-        ....:     for d in [1,-1]:
-        ....:         print(s.tangent_vector(0, (x, 1/2), (0, d)))
+        sage: s.tangent_vector(0, (0, 1/2), (0, 1))
         SimilaritySurfaceTangentVector in polygon 0 based at (1, 1/2) with vector (0, 1)
+        sage: s.tangent_vector(0, (0, 1/2), (0, -1))
         SimilaritySurfaceTangentVector in polygon 0 based at (0, 1/2) with vector (0, -1)
+        sage: s.tangent_vector(0, (1, 1/2), (0, 1))
         SimilaritySurfaceTangentVector in polygon 0 based at (1, 1/2) with vector (0, 1)
+        sage: s.tangent_vector(0, (1, 1/2), (0, -1))
         SimilaritySurfaceTangentVector in polygon 0 based at (0, 1/2) with vector (0, -1)
 
     Examples on vertices in direction of edges::
 
         sage: s = translation_surfaces.square_torus()
-        sage: for y in [0,1]:
-        ....:     print(s.tangent_vector(0, (0, y), (1, 0)))
-        ....:     print(s.tangent_vector(0, (1, y), (-1, 0)))
+        sage: s.tangent_vector(0, (0, 0), (1, 0))
         SimilaritySurfaceTangentVector in polygon 0 based at (0, 0) with vector (1, 0)
+        sage: s.tangent_vector(0, (1, 0), (-1, 0))
         SimilaritySurfaceTangentVector in polygon 0 based at (1, 1) with vector (-1, 0)
+        sage: s.tangent_vector(0, (0, 1), (1, 0))
         SimilaritySurfaceTangentVector in polygon 0 based at (0, 0) with vector (1, 0)
+        sage: s.tangent_vector(0, (1, 1), (-1, 0))
         SimilaritySurfaceTangentVector in polygon 0 based at (1, 1) with vector (-1, 0)
 
-        sage: for x in [0,1]:
-        ....:     print(s.tangent_vector(0, (x, 0), (0, 1)))
-        ....:     print(s.tangent_vector(0, (x, 1), (0, -1)))
+        sage: s.tangent_vector(0, (0, 0), (0, 1))
         SimilaritySurfaceTangentVector in polygon 0 based at (1, 0) with vector (0, 1)
+        sage: s.tangent_vector(0, (0, 1), (0, -1))
         SimilaritySurfaceTangentVector in polygon 0 based at (0, 1) with vector (0, -1)
+        sage: s.tangent_vector(0, (1, 0), (0, 1))
         SimilaritySurfaceTangentVector in polygon 0 based at (1, 0) with vector (0, 1)
+        sage: s.tangent_vector(0, (1, 1), (0, -1))
         SimilaritySurfaceTangentVector in polygon 0 based at (0, 1) with vector (0, -1)
+
     """
+
     def __init__(self, tangent_bundle, polygon_label, point, vector):
+        from flatsurf.geometry.euclidean import ccw, is_anti_parallel
+
         self._bundle = tangent_bundle
         p = self.surface().polygon(polygon_label)
         pos = p.get_point_position(point)
-        if vector == self._bundle.vector_space().zero():
-            raise ValueError("Provided vector is zero. (Temporarily not supported.)")
+        if not vector:
+            raise NotImplementedError("vector must be non-zero")
         if pos.is_in_interior():
             self._polygon_label = polygon_label
             self._point = point
             self._vector = vector
             self._position = pos
         elif pos.is_in_edge_interior():
             e = pos.get_edge()
             edge_v = p.edge(e)
-            if wedge_product(edge_v,vector)<0 or is_opposite_direction(edge_v,vector):
+
+            if ccw(edge_v, vector) < 0 or is_anti_parallel(edge_v, vector):
                 # Need to move point and vector to opposite edge.
-                label2,e2 = self.surface().opposite_edge(polygon_label,e)
-                similarity = self.surface().edge_transformation(polygon_label,e)
-                point2=similarity(point)
-                vector2=similarity.derivative()*vector
-                self._polygon_label=label2
-                self._point=point2
-                self._vector=vector2
-                self._position=self.surface().polygon(label2).get_point_position(point2)
+                label2, e2 = self.surface().opposite_edge(polygon_label, e)
+                similarity = self.surface().edge_transformation(polygon_label, e)
+                point2 = similarity(point)
+                vector2 = similarity.derivative() * vector
+                self._polygon_label = label2
+                self._point = point2
+                self._vector = vector2
+                self._position = (
+                    self.surface().polygon(label2).get_point_position(point2)
+                )
             else:
-                self._polygon_label=polygon_label
-                self._point=point
-                self._vector=vector
-                self._position=pos
+                self._polygon_label = polygon_label
+                self._point = point
+                self._vector = vector
+                self._position = pos
         elif pos.is_vertex():
-            v=pos.get_vertex()
-            p=self.surface().polygon(polygon_label)
+            v = pos.get_vertex()
+            p = self.surface().polygon(polygon_label)
             # subsequent edge:
             edge1 = p.edge(v)
             # prior edge:
-            edge0 = p.edge( (v-1)%p.num_edges() )
-            wp1 = wedge_product(edge1,vector)
-            wp0 = wedge_product(edge0,vector)
-            if wp1<0 or wp0<0:
-                raise ValueError("Singular point with vector pointing away from polygon")
+            edge0 = p.edge((v - 1) % len(p.vertices()))
+            wp1 = ccw(edge1, vector)
+            wp0 = ccw(edge0, vector)
+            if wp1 < 0 or wp0 < 0:
+                raise ValueError(
+                    "Singular point with vector pointing away from polygon"
+                )
             if wp0 == 0:
                 # vector points backward along edge 0
-                label2,e2 = self.surface().opposite_edge(polygon_label, (v-1)%p.num_edges())
-                similarity = self.surface().edge_transformation(polygon_label, (v-1)%p.num_edges())
-                point2=similarity(point)
-                vector2=similarity.derivative()*vector
-                self._polygon_label=label2
-                self._point=point2
-                self._vector=vector2
-                self._position=self.surface().polygon(label2).get_point_position(point2)
+                label2, e2 = self.surface().opposite_edge(
+                    polygon_label, (v - 1) % len(p.vertices())
+                )
+                similarity = self.surface().edge_transformation(
+                    polygon_label, (v - 1) % len(p.vertices())
+                )
+                point2 = similarity(point)
+                vector2 = similarity.derivative() * vector
+                self._polygon_label = label2
+                self._point = point2
+                self._vector = vector2
+                self._position = (
+                    self.surface().polygon(label2).get_point_position(point2)
+                )
             else:
                 # vector points along edge1 in that directior or points into polygons interior
-                self._polygon_label=polygon_label
-                self._point=point
-                self._vector=vector
-                self._position=pos
+                self._polygon_label = polygon_label
+                self._point = point
+                self._vector = vector
+                self._position = pos
         else:
             raise ValueError("Provided point lies outside the indexed polygon")
 
+        self._point.set_immutable()
+        self._vector.set_immutable()
+
     def __repr__(self):
-        return "SimilaritySurfaceTangentVector in polygon "+repr(self._polygon_label)+\
-            " based at "+repr(self._point)+" with vector "+repr(self._vector)
+        return (
+            "SimilaritySurfaceTangentVector in polygon "
+            + repr(self._polygon_label)
+            + " based at "
+            + repr(self._point)
+            + " with vector "
+            + repr(self._vector)
+        )
 
     def __eq__(self, other):
         if isinstance(other, self.__class__):
-            return self.surface()==other.surface() and \
-                self.polygon_label() == other.polygon_label() and \
-                self.point() == other.point() and \
-                self.vector() == other.vector()
-        raise NotImplemented
+            return (
+                self.surface() == other.surface()
+                and self.polygon_label() == other.polygon_label()
+                and self.point() == other.point()
+                and self.vector() == other.vector()
+            )
+        return NotImplemented
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     def __hash__(self):
-        return hash(tuple(sorted(self.__dict__.items())))
+        r"""
+        TESTS::
+
+            sage: from flatsurf import translation_surfaces
+            sage: s = translation_surfaces.square_torus()
+            sage: for y in [0,1]:
+            ....:     for d in [1,-1]:
+            ....:         h = hash(s.tangent_vector(0, (1/2, y), (d, 0)))
+        """
+        return hash((self._bundle, self._polygon_label, self._point, self._vector))
 
     def surface(self):
         r"""Return the underlying surface."""
         return self._bundle.surface()
 
     def is_based_at_singularity(self):
         r"""
@@ -141,21 +195,14 @@
         """
         return self._position.is_vertex()
 
     def vertex(self):
         r"""Return the index of the vertex."""
         return self._position.get_vertex()
 
-    def singularity(self):
-        r"""Return the index of the vertex."""
-        from sage.misc.superseded import deprecation
-        deprecation(42, "Do not use .singularity(). Use .vertex() instead.")
-        # Note: I want to change this to returning the singularity of the surface instead.
-        return self._position.get_vertex()
-
     def is_in_boundary_of_polygon(self):
         r"""
         Return the truth value of the statement
         'the base point for this vector lies on the boundary of
         one of the polygons making up the surface.'
         """
         return self._position.is_in_boundary()
@@ -164,15 +211,15 @@
         r"""
         Return the PolygonPosition representing the location of
         the basepoint of the vector in the polygon that contains it.
         """
         return self._position
 
     def bundle(self):
-        r""" Return the tangent bundle containing this vector. """
+        r"""Return the tangent bundle containing this vector."""
         return self._bundle
 
     def polygon_label(self):
         return self._polygon_label
 
     def polygon(self):
         return self.surface().polygon(self.polygon_label())
@@ -217,40 +264,42 @@
     def edge_pointing_along(self):
         r"""
         Returns the pair of (p,e) where p is the polygon label at the base point,
         and e is the edge this vector points along or none if it does not point
         along an edge. Here pointing along means that the vector is based at
         a vertex and represents the vector joining this edge to the next vertex."""
         if self.is_based_at_singularity():
-            e=self.vertex()
-            if self.vector()==self.polygon().edge(e):
-                return (self.polygon_label(),e)
+            e = self.vertex()
+            if self.vector() == self.polygon().edge(e):
+                return (self.polygon_label(), e)
         return None
 
     def differs_by_scaling(self, another_tangent_vector):
         r"""
         Returns true if the other vector just differs by scaling. This means they should lie
         in the same polygon, be based at the same point, and point in the same direction.
         """
-        return self.polygon_label()==another_tangent_vector.polygon_label() and \
-            self.point()==another_tangent_vector.point() and \
-            is_same_direction(self.vector(),another_tangent_vector.vector())
+        from flatsurf.geometry.euclidean import is_parallel
+
+        return (
+            self.polygon_label() == another_tangent_vector.polygon_label()
+            and self.point() == another_tangent_vector.point()
+            and is_parallel(self.vector(), another_tangent_vector.vector())
+        )
 
     def invert(self):
         r"""
         Returns the negation of this tangent vector.
         Raises a ValueError if the vector is based at a singularity.'
         """
         if self.is_based_at_singularity():
             raise ValueError("Can't invert tangent vector based at a singularity.")
         return SimilaritySurfaceTangentVector(
-            self.bundle(),
-            self.polygon_label(),
-            self.point(),
-            -self.vector())
+            self.bundle(), self.polygon_label(), self.point(), -self.vector()
+        )
 
     def forward_to_polygon_boundary(self):
         r"""
         Flows forward (in the direction of the tangent vector) until the end
         of the polygon is reached.
         Returns the tangent vector based at the endpoint which point backward along the trajectory.
 
@@ -261,46 +310,44 @@
 
         EXAMPLES::
 
             sage: from flatsurf.geometry.similarity_surface_generators import SimilaritySurfaceGenerators
             sage: s = SimilaritySurfaceGenerators.example()
             sage: from flatsurf.geometry.tangent_bundle import SimilaritySurfaceTangentBundle
             sage: tb = SimilaritySurfaceTangentBundle(s)
-            sage: print("Polygon 0 is "+str(s.polygon(0)))
-            Polygon 0 is Polygon: (0, 0), (2, -2), (2, 0)
-            sage: print("Polygon 1 is "+str(s.polygon(1)))
-            Polygon 1 is Polygon: (0, 0), (2, 0), (1, 3)
+            sage: s.polygon(0)
+            Polygon(vertices=[(0, 0), (2, -2), (2, 0)])
+            sage: s.polygon(1)
+            Polygon(vertices=[(0, 0), (2, 0), (1, 3)])
             sage: from flatsurf.geometry.tangent_bundle import SimilaritySurfaceTangentVector
-            sage: V = tb.surface().vector_space()
+            sage: V = tb.surface().base_ring()**2
             sage: v = SimilaritySurfaceTangentVector(tb, 0, V((0,0)), V((3,-1)))
-            sage: print(v)
+            sage: v
             SimilaritySurfaceTangentVector in polygon 0 based at (0, 0) with vector (3, -1)
             sage: v2 = v.forward_to_polygon_boundary()
-            sage: print(v2)
+            sage: v2
             SimilaritySurfaceTangentVector in polygon 0 based at (2, -2/3) with vector (-3, 1)
-            sage: print(v2.invert())
+            sage: v2.invert()
             SimilaritySurfaceTangentVector in polygon 1 based at (2/3, 2) with vector (4, -3)
         """
-        p=self.polygon()
-        point2,pos2 = p.flow_to_exit(self.point(), self.vector())
-        #diff=point2-point
+        p = self.polygon()
+        point2, pos2 = p.flow_to_exit(self.point(), self.vector())
+        # diff=point2-point
         new_vector = SimilaritySurfaceTangentVector(
-            self.bundle(),
-            self.polygon_label(),
-            point2,
-            -self.vector())
+            self.bundle(), self.polygon_label(), point2, -self.vector()
+        )
         return new_vector
 
     def straight_line_trajectory(self):
         r"""
         Return the straight line trajectory associated to this vector.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
 
             sage: s = translation_surfaces.square_torus()
             sage: v = s.tangent_vector(0, (0,0), (1,1))
             sage: v.straight_line_trajectory()
             Straight line trajectory made of 1 segments from (0, 0) in polygon 0 to (1, 1) in polygon 0
             sage: l = v.straight_line_trajectory()
             sage: l
@@ -311,189 +358,239 @@
             sage: v = s.tangent_vector(0, (0,0), (1,1+AA(5).sqrt()), ring=AA)
             sage: l = v.straight_line_trajectory()
             sage: l.flow(20)
             sage: l.segment(20)
             Segment in polygon 0 starting at (0.9442719099991588?, 0) and ending at (1, 0.1803398874989485?)
         """
         from flatsurf.geometry.straight_line_trajectory import StraightLineTrajectory
+
         return StraightLineTrajectory(self)
 
-    def clockwise_to(self, w, code = False):
+    def clockwise_to(self, w, code=False):
         r"""
         Return the new tangent vector obtained by rotating this one in the clockwise
         direction until the vector is parallel to w, and scaling so that the length matches
-        that of w. 
-        
-        Note that we always do some rotation so that if w is parallel to this vector, then a 
+        that of w.
+
+        Note that we always do some rotation so that if w is parallel to this vector, then a
         -360 degree rotation is performed.
-        
+
         The vector w must be nonzero.
-        
+
         On an infinite surface, this is potentially an infinite calculation
         so we impose a limit (representing the maximal number of polygons
         that must be rotated through.) This is the variable rotate_limit
         in this package.
 
         If code is True, we compute the sequences of numbers associated to edges
         crossed as a list. We return a pair consisting of the newly computing
         tangent vector an this code. This is currently only implemented when
         based at a singularity.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: s=translation_surfaces.regular_octagon()
             sage: v=s.tangent_vector(0,(0,0),(1,1))
             sage: v.clockwise_to((-1,-1))
             SimilaritySurfaceTangentVector in polygon 0 based at (0, a + 1) with vector (-1, -1)
             sage: v.clockwise_to((1,1))
             SimilaritySurfaceTangentVector in polygon 0 based at (-1/2*a, 1/2*a) with vector (1, 1)
             sage: v.clockwise_to((1,1), code=True)
             (SimilaritySurfaceTangentVector in polygon 0 based at (-1/2*a, 1/2*a) with vector (1, 1), [0, 5, 2])
         """
-        assert w!=self.surface().vector_space().zero(), "Vector w must be non-zero."
+        if not w:
+            raise ValueError("w must be non-zero")
+
         if self.is_based_at_singularity():
-            s=self.surface()
-            v1=self.vector()
-            label=self.polygon_label()
-            vertex=self.vertex()
-            v2=s.polygon(label).edge(vertex)
+            s = self.surface()
+            v1 = self.vector()
+            label = self.polygon_label()
+            vertex = self.vertex()
+            v2 = s.polygon(label).edge(vertex)
             from sage.matrix.constructor import Matrix
-            der = Matrix(s.base_ring(), [[1,0],[0,1]])
+
+            der = Matrix(s.base_ring(), [[1, 0], [0, 1]])
             if code:
                 codes = []
+
+            from flatsurf.geometry.euclidean import ccw
+
             for count in range(rotate_limit):
-                if wedge_product(v2,w)>=0 and wedge_product(w,v1)>0:
+                if ccw(v2, w) >= 0 and ccw(w, v1) > 0:
                     # We've found it!
                     break
                 if code:
                     codes.append(vertex)
-                label2,edge2=s.opposite_edge(label,vertex)
-                der=der*s.edge_matrix(label2,edge2)
-                v1=der*(-s.polygon(label2).edge(edge2))
-                label=label2
-                vertex=(edge2+1) % s.polygon(label2).num_edges()
-                v2=der*(s.polygon(label2).edge(vertex))
-            assert count<rotate_limit, "Reached limit!"
+                label2, edge2 = s.opposite_edge(label, vertex)
+                der = der * s.edge_matrix(label2, edge2)
+                v1 = der * (-s.polygon(label2).edge(edge2))
+                label = label2
+                vertex = (edge2 + 1) % len(s.polygon(label2).vertices())
+                v2 = der * (s.polygon(label2).edge(vertex))
+            assert count < rotate_limit, "Reached limit!"
             if code:
                 return (
-                    self.surface().tangent_vector(label,s.polygon(label).vertex(vertex),w),
-                    codes
+                    self.surface().tangent_vector(
+                        label, s.polygon(label).vertex(vertex), w
+                    ),
+                    codes,
                 )
             else:
-                return self.surface().tangent_vector(label,s.polygon(label).vertex(vertex),w)
+                return self.surface().tangent_vector(
+                    label, s.polygon(label).vertex(vertex), w
+                )
         else:
-            if code:
-                raise NotImplementedError('codes are only implemented when based at a singularity')
-            return self.surface().tangent_vector(v.polygon_label(),v.point(),w)
+            raise NotImplementedError(
+                "Rotating tangent vectors is only implemnted when at a singularity"
+            )
 
     def counterclockwise_to(self, w, code=False):
         r"""
         Return the new tangent vector obtained by rotating this one in the counterclockwise
         direction until the vector is parallel to w, and scaling so that the length matches
-        that of w. 
-        
-        Note that we always do some rotation so that if w is parallel to this vector, then a 
+        that of w.
+
+        Note that we always do some rotation so that if w is parallel to this vector, then a
         360 degree rotation is performed.
-        
+
         The vector w must be nonzero.
-        
+
         On an infinite surface, this is potentially an infinite calculation
         so we impose a limit (representing the maximal number of polygons
         that must be rotated through.) This is the variable rotate_limit
         in this package.
 
         If code is True, we compute the sequences of numbers associated to edges
         crossed as a list. We return a pair consisting of the newly computing
         tangent vector an this code. This is currently only implemented when
         based at a singularity.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: s=translation_surfaces.regular_octagon()
             sage: v=s.tangent_vector(0,(0,0),(1,1))
             sage: v.counterclockwise_to((-1,-1))
             SimilaritySurfaceTangentVector in polygon 0 based at (1/2*a + 1, 1/2*a + 1) with vector (-1, -1)
             sage: v.counterclockwise_to((1,1))
             SimilaritySurfaceTangentVector in polygon 0 based at (1, 0) with vector (1, 1)
             sage: v.counterclockwise_to((1,1), code=True)
             (SimilaritySurfaceTangentVector in polygon 0 based at (1, 0) with vector (1, 1), [7, 2, 5])
         """
-        assert w!=self.surface().vector_space().zero(), "Vector w must be non-zero."
+        if not w:
+            raise ValueError("w must be non-zero")
+
         if self.is_based_at_singularity():
-            s=self.surface()
-            v1=self.vector()
-            label=self.polygon_label()
-            vertex=self.vertex()
-            previous_vertex = (vertex-1+s.polygon(label).num_edges()) % \
-                s.polygon(label).num_edges()
-            v2=-s.polygon(label).edge(previous_vertex)
+            s = self.surface()
+            v1 = self.vector()
+            label = self.polygon_label()
+            vertex = self.vertex()
+            previous_vertex = (vertex - 1 + len(s.polygon(label).vertices())) % len(
+                s.polygon(label).vertices()
+            )
+            v2 = -s.polygon(label).edge(previous_vertex)
             from sage.matrix.constructor import Matrix
-            der = Matrix(s.base_ring(), [[1,0],[0,1]])
+
+            der = Matrix(s.base_ring(), [[1, 0], [0, 1]])
             if code:
                 codes = []
-            if not (wedge_product(v1,w)>0 and wedge_product(w,v2)>0):
+
+            from flatsurf.geometry.euclidean import ccw
+
+            if not (ccw(v1, w) > 0 and ccw(w, v2) > 0):
                 for count in range(rotate_limit):
-                    label2,edge2=s.opposite_edge(label,previous_vertex)
+                    label2, edge2 = s.opposite_edge(label, previous_vertex)
                     if code:
                         codes.append(previous_vertex)
-                    der=der*s.edge_matrix(label2,edge2)
-                    label=label2
-                    vertex=edge2
-                    previous_vertex = (vertex-1+s.polygon(label).num_edges()) % \
-                        s.polygon(label).num_edges()
-                    v1=der*(s.polygon(label).edge(vertex))
-                    v2=der*(-s.polygon(label).edge(previous_vertex))
-                    if wedge_product(v1,w)>=0 and wedge_product(w,v2)>0:
+                    der = der * s.edge_matrix(label2, edge2)
+                    label = label2
+                    vertex = edge2
+                    previous_vertex = (
+                        vertex - 1 + len(s.polygon(label).vertices())
+                    ) % len(s.polygon(label).vertices())
+                    v1 = der * (s.polygon(label).edge(vertex))
+                    v2 = der * (-s.polygon(label).edge(previous_vertex))
+                    if ccw(v1, w) >= 0 and ccw(w, v2) > 0:
                         # We've found it!
                         break
-                assert count<rotate_limit, "Reached limit!"
+                assert count < rotate_limit, "Reached limit!"
             if code:
                 return (
-                    self.surface().tangent_vector(label,s.polygon(label).vertex(vertex),w),
-                    codes
+                    self.surface().tangent_vector(
+                        label, s.polygon(label).vertex(vertex), w
+                    ),
+                    codes,
                 )
             else:
-                return self.surface().tangent_vector(label,s.polygon(label).vertex(vertex),w)
+                return self.surface().tangent_vector(
+                    label, s.polygon(label).vertex(vertex), w
+                )
         else:
-            if code:
-                raise NotImplementedError('codes are only implemented when based at a singularity')
-            return self.surface().tangent_vector(v.polygon_label(),v.point(),w)
+            raise NotImplementedError(
+                "Rotating tangent vectors is only implemnted when at a singularity"
+            )
+
+    def plot(self, **kwargs):
+        r"""
+        Return a plot of this tangent vector.
+
+        EXAMPLES::
+
+            sage: import flatsurf
+            sage: S = flatsurf.translation_surfaces.veech_double_n_gon(5)
+            sage: v = S.tangent_vector(0, (1/8, 1/4), (1/2, 1/4))
+            sage: S.plot() + v.plot()
+            Graphics object consisting of 22 graphics primitives
+
+        Any keyword arguments are passed on to the underlying plot method from SageMath::
+
+            sage: S.plot() + v.plot(color="red")
+            Graphics object consisting of 22 graphics primitives
+
+        """
+        return self.vector().plot(
+            **{"start": self.point(), "width": 1, "arrowsize": 2, **kwargs}
+        )
 
 
 class SimilaritySurfaceTangentBundle:
     r"""
     Construct the tangent bundle of a given similarity surface.
 
-    Needs work: We should check for coersion from the base_ring of the surface
+    Needs work: We should check for coercion from the base_ring of the surface
     """
+
     def __init__(self, similarity_surface, ring=None):
-        self._s=similarity_surface
+        self._s = similarity_surface
         if ring is None:
-            self._base_ring=self._s.base_ring()
+            self._base_ring = self._s.base_ring()
         else:
-            self._base_ring=ring
+            self._base_ring = ring
         from sage.modules.free_module import VectorSpace
+
         self._V = VectorSpace(self._base_ring, 2)
 
     def __call__(self, polygon_label, point, vector):
         r"""
         Construct a tangent vector from a polygon label, a point in the polygon and a vector. The point and the vector should have coordinates
         in the base field."""
-        V = self.vector_space()
-        return SimilaritySurfaceTangentVector(self, polygon_label, self._V(point), self._V(vector))
+        return SimilaritySurfaceTangentVector(
+            self, polygon_label, self._V(point), self._V(vector)
+        )
 
     def __repr__(self):
-        return "Tangent bundle of {!r} defined over {!r}".format(self._s, self._base_ring)
+        return "Tangent bundle of {!r} defined over {!r}".format(
+            self._s, self._base_ring
+        )
 
     def base_ring(self):
         return self._base_ring
 
-    field=base_ring
+    field = base_ring
 
     def vector_space(self):
         r"""
         Return the vector space over the field of the bundle.
         """
         return self._V
 
@@ -508,43 +605,42 @@
 
         EXAMPLES::
 
             sage: from flatsurf.geometry.similarity_surface_generators import SimilaritySurfaceGenerators
             sage: s = SimilaritySurfaceGenerators.example()
             sage: from flatsurf.geometry.tangent_bundle import SimilaritySurfaceTangentBundle
             sage: tb = SimilaritySurfaceTangentBundle(s)
-            sage: print(s.polygon(0))
-            Polygon: (0, 0), (2, -2), (2, 0)
-            sage: print(tb.edge(0,0))
+            sage: s.polygon(0)
+            Polygon(vertices=[(0, 0), (2, -2), (2, 0)])
+            sage: tb.edge(0,0)
             SimilaritySurfaceTangentVector in polygon 0 based at (0, 0) with vector (2, -2)
         """
-        polygon=self.surface().polygon(polygon_label)
-        point=polygon.vertex(edge_index)
-        vector=polygon.edge(edge_index)
+        polygon = self.surface().polygon(polygon_label)
+        point = polygon.vertex(edge_index)
+        vector = polygon.edge(edge_index)
         return SimilaritySurfaceTangentVector(self, polygon_label, point, vector)
 
     def clockwise_edge(self, polygon_label, edge_index):
         r"""Return the vector leaving a vertex of the polygon which under straight-line flow travels
         *clockwise* around the boundary of the polygon along the edge with the provided index.
         The length of the vector matches the length of the indexed edge.
-        Note that the point will be based in the polgon opposite the provided edge.
+        Note that the point will be based in the polygon opposite the provided edge.
 
         EXAMPLES::
 
             sage: from flatsurf.geometry.similarity_surface_generators import SimilaritySurfaceGenerators
             sage: s = SimilaritySurfaceGenerators.example()
             sage: from flatsurf.geometry.tangent_bundle import SimilaritySurfaceTangentBundle
             sage: tb = SimilaritySurfaceTangentBundle(s)
-            sage: print("Polygon 0 is "+str(s.polygon(0)))
-            Polygon 0 is Polygon: (0, 0), (2, -2), (2, 0)
-            sage: print("Polygon 1 is "+str(s.polygon(1)))
-            Polygon 1 is Polygon: (0, 0), (2, 0), (1, 3)
-            sage: print("Opposite edge to (0,0) is "+repr(s.opposite_edge(0,0)))
-            Opposite edge to (0,0) is (1, 1)
-            sage: print(tb.clockwise_edge(0,0))
+            sage: s.polygon(0)
+            Polygon(vertices=[(0, 0), (2, -2), (2, 0)])
+            sage: s.polygon(1)
+            Polygon(vertices=[(0, 0), (2, 0), (1, 3)])
+            sage: s.opposite_edge(0, 0)
+            (1, 1)
+            sage: tb.clockwise_edge(0,0)
             SimilaritySurfaceTangentVector in polygon 1 based at (2, 0) with vector (-1, 3)
         """
-        polygon=self.surface().polygon(polygon_label)
-        point=polygon.vertex(edge_index+1)
-        vector=-polygon.edge(edge_index)
+        polygon = self.surface().polygon(polygon_label)
+        point = polygon.vertex(edge_index + 1)
+        vector = -polygon.edge(edge_index)
         return SimilaritySurfaceTangentVector(self, polygon_label, point, vector)
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/thurston_veech.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/thurston_veech.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,17 +41,14 @@
 
 from sage.all import ZZ, QQ, AA, matrix, diagonal_matrix, NumberField
 from sage.rings.qqbar import do_polred
 
 from surface_dynamics.flat_surfaces.origamis.origami import Origami
 from surface_dynamics.misc.permutation import perm_dense_cycles
 
-from .polygon import ConvexPolygons
-from .surface import Surface_list
-from .translation_surface import TranslationSurface
 
 class ThurstonVeech:
     def __init__(self, hp, vp):
         r"""
         INPUT:
 
         - ``hp`` - permutation describing the horizontal gluing of the rectangles
@@ -65,46 +62,46 @@
             sage: TV
             ThurstonVeech("(1,2)(3,4)", "(1)(2,3)(4)")
             sage: TV.stratum()
             H_2(1^2)
 
             sage: S = TV([1,2], [3,1,1])
             sage: S
-            TranslationSurface built from 4 polygons
-            sage: S.stratum()
-            H_2(1^2)
+            Translation Surface in H_2(1^2) built from 4 rectangles
             sage: S.base_ring()
             Number Field in a with defining polynomial x^2 - 2 with a = 1.414213562373095?
 
             sage: S = TV([1,1], [2,1,2])
             sage: S.base_ring()
             Rational Field
         """
-        o = self._o = Origami(hp, vp)
-        n = o.nb_squares()
-        hcycles, hsizes = perm_dense_cycles(o.r_tuple(), n)
-        vcycles, vsizes = perm_dense_cycles(o.u_tuple(), n)
+        self._origami = Origami(hp, vp)
+        n = self._origami.nb_squares()
+        hcycles, hsizes = perm_dense_cycles(self._origami.r_tuple(), n)
+        vcycles, vsizes = perm_dense_cycles(self._origami.u_tuple(), n)
         self._hcycles = hcycles
         self._vcycles = vcycles
         self._num_hcyls = len(hsizes)
         self._num_vcyls = len(vsizes)
         E = self._E = matrix(ZZ, self._num_hcyls, self._num_vcyls)
         for i in range(n):
             E[hcycles[i], vcycles[i]] += 1
         E.set_immutable()
 
     def __repr__(self):
-        return "ThurstonVeech(\"{}\", \"{}\")".format(self._o.r().cycle_string(singletons=True),
-                                              self._o.u().cycle_string(singletons=True))
-    
+        return 'ThurstonVeech("{}", "{}")'.format(
+            self._origami.r().cycle_string(singletons=True),
+            self._origami.u().cycle_string(singletons=True),
+        )
+
     def stratum(self):
-        return self._o.stratum()
+        return self._origami.stratum()
 
     def stratum_component(self):
-        return self._o.stratum_component()
+        return self._origami.stratum_component()
 
     def cylinder_intersection_matrix(self):
         return self._E
 
     def __call__(self, hmult, vmult):
         r"""
         INPUT:
@@ -131,15 +128,15 @@
         mp = pf.minpoly()
         if mp.degree() == 1:
             K = QQ
             pf = QQ(pf)
         else:
             fwd, bck, q = do_polred(pf.minpoly())
             im_gen = fwd(pf)
-            K = NumberField(q, 'a', embedding=im_gen)
+            K = NumberField(q, "a", embedding=im_gen)
             pf = bck(K.gen())
 
         # Compute widths of the cylinders via Perron-Frobenius
         if self._num_hcyls < self._num_vcyls:
             hcirc = (F - pf).right_kernel_matrix()
             assert hcirc.nrows() == 1
             assert hcirc.ncols() == self._num_hcyls
@@ -158,24 +155,27 @@
             d = 1
             c = pf
 
         # Solve linear systems to get heights
         h = [hcirc[i] * hmult[i] / c for i in range(self._num_hcyls)]
         v = [vcirc[i] * vmult[i] / d for i in range(self._num_vcyls)]
 
-        C = ConvexPolygons(K)
+        from flatsurf import Polygon
+
         P = []
-        for i in range(self._o.nb_squares()):
+        for i in range(self._origami.nb_squares()):
             hi = h[self._hcycles[i]]
             vi = v[self._vcycles[i]]
-            P.append(C(edges=[(vi,0),(0,hi),(-vi,0),(0,-hi)]))
+            P.append(Polygon(edges=[(vi, 0), (0, hi), (-vi, 0), (0, -hi)], base_ring=K))
+
+        from flatsurf.geometry.surface import MutableOrientedSimilaritySurface
 
-        surface = Surface_list(base_ring=K)
+        surface = MutableOrientedSimilaritySurface(K)
         for p in P:
             surface.add_polygon(p)
-        r = self._o.r_tuple()
-        u = self._o.u_tuple()
-        for i in range(self._o.nb_squares()):
-            surface.set_edge_pairing(i, 1, r[i], 3)
-            surface.set_edge_pairing(i, 0, u[i], 2)
+        r = self._origami.r_tuple()
+        u = self._origami.u_tuple()
+        for i in range(self._origami.nb_squares()):
+            surface.glue((i, 1), (r[i], 3))
+            surface.glue((i, 0), (u[i], 2))
         surface.set_immutable()
-        return TranslationSurface(surface)
+        return surface
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/geometry/translation_surface.py` & `sage_flatsurf-0.5.0/flatsurf/geometry/categories/translation_surfaces.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,759 +1,716 @@
 r"""
-Translation Surfaces.
-"""
-
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
-from six import iteritems
+The category of translation surfaces.
 
-from sage.matrix.constructor import identity_matrix
+This module provides shared functionality for all surfaces in sage-flatsurf
+that are built from Euclidean polygons whose glued edges can be transformed
+into each other with translations.
 
-from .surface import Surface
-from .half_translation_surface import HalfTranslationSurface
-from .dilation_surface import DilationSurface
+See :mod:`flatsurf.geometry.categories` for a general description of the
+category framework in sage-flatsurf.
 
-class TranslationSurface(HalfTranslationSurface, DilationSurface):
-    r"""
-    A surface with a flat metric and conical singularities whose cone angles are a multiple of pi.
-    """
+Normally, you won't create this (or any other) category directly. The correct
+category is automatically determined for immutable surfaces.
 
-    def minimal_translation_cover(self):
-        return self
-
-    def _test_edge_matrix(self, **options):
-        r"""
-        Check the compatibility condition
-        """
-        tester = self._tester(**options)
+EXAMPLES::
 
-        from flatsurf.geometry.similarity_surface import SimilaritySurface
-        if self.is_finite():
-            it = self.label_iterator()
-        else:
-            from itertools import islice
-            it = islice(self.label_iterator(), 30)
-
-        for lab in it:
-            p = self.polygon(lab)
-            for e in range(p.num_edges()):
-                # Warning: check the matrices computed from the edges,
-                # rather the ones overriden by TranslationSurface.
-                m=SimilaritySurface.edge_matrix(self,lab,e)
-                tester.assertTrue(m.is_one(), \
-                    "edge_matrix of edge "+str((lab,e))+" is not a translation.")
-
-    def edge_matrix(self, p, e=None):
-        if e is None:
-            p,e = p
-        if e < 0 or e >= self.polygon(p).num_edges():
-            raise ValueError
-        return identity_matrix(self.base_ring(),2)
+    sage: from flatsurf import translation_surfaces
+    sage: S = translation_surfaces.square_torus()
+    sage: C = S.category()
 
-    def stratum(self):
-        r"""
-        Return the stratum this surface belongs to.
+    sage: from flatsurf.geometry.categories import TranslationSurfaces
+    sage: C.is_subcategory(TranslationSurfaces())
+    True
 
-        This uses the package ``surface-dynamics``
-        (see http://www.labri.fr/perso/vdelecro/flatsurf_sage.html)
+"""
+# ####################################################################
+#  This file is part of sage-flatsurf.
+#
+#        Copyright (C) 2013-2019 Vincent Delecroix
+#                      2013-2019 W. Patrick Hooper
+#                           2023 Julian Rüth
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+# ####################################################################
+
+from flatsurf.geometry.categories.surface_category import SurfaceCategoryWithAxiom
+from flatsurf.geometry.categories.half_translation_surfaces import (
+    HalfTranslationSurfaces,
+)
 
-        EXAMPLES::
 
-            sage: import flatsurf.geometry.similarity_surface_generators as sfg
-            sage: sfg.translation_surfaces.octagon_and_squares().stratum()
-            H_3(4)
-        """
-        from surface_dynamics import AbelianStratum
-        from sage.rings.integer_ring import ZZ
-        return AbelianStratum([ZZ(a-1) for a in self.angles()])
+class TranslationSurfaces(SurfaceCategoryWithAxiom):
+    r"""
+    The category of surfaces built by gluing (Euclidean) polygons with
+    translations.
 
-    def _canonical_first_vertex(polygon):
-        r"""
-        Return the index of the vertex with smallest y-coordinate.
-        If two vertices have the same y-coordinate, then the one with least x-coordinate is returned.
-        """
-        best=0
-        best_pt=polygon.vertex(best)
-        for v in range(1,polygon.num_edges()):
-            pt=polygon.vertex(v)
-            if pt[1]<best_pt[1]:
-                best=v
-                best_pt=pt
-        if best==0:
-            if pt[1]==best_pt[1]:
-                return v
-        return best
+    EXAMPLES::
 
-    def standardize_polygons(self, in_place=False):
-        r"""
-        Replaces each polygon with a polygon with a new polygon which differs by translation
-        and reindexing. The new polygon will have the property that vertex zero is the origin,
-        and all vertices lie either in the upper half plane, or on the x-axis with non-negative
-        x-coordinate.
+        sage: from flatsurf.geometry.categories import TranslationSurfaces
+        sage: TranslationSurfaces()
+        Category of translation surfaces
 
-        This is done to the current surface if in_place=True. A mutable copy is created and returned
-        if in_place=False (as default).
+    """
+    # The category of translation surfaces is identical to the category of
+    # half-translation surfaces with the positive axiom.
+    _base_category_class_and_axiom = (HalfTranslationSurfaces, "Positive")
+
+    def extra_super_categories(self):
+        r"""
+        Return the other categories that a translation surface is automatically
+        a member of (apart from being a positive half-translation surface, its
+        orientation is compatible with the orientation of the polygons in the
+        real plane, so it's "oriented.")
 
         EXAMPLES::
 
-            sage: from flatsurf import *
-            sage: s=translation_surfaces.veech_double_n_gon(4)
-            sage: s.polygon(1)
-            Polygon: (0, 0), (-1, 0), (-1, -1), (0, -1)
-            sage: [s.opposite_edge(0,i) for i in range(4)]
-            [(1, 0), (1, 1), (1, 2), (1, 3)]
-            sage: ss=s.standardize_polygons()
-            sage: ss.polygon(1)
-            Polygon: (0, 0), (1, 0), (1, 1), (0, 1)
-            sage: [ss.opposite_edge(0,i) for i in range(4)]
-            [(1, 2), (1, 3), (1, 0), (1, 1)]
-            sage: TestSuite(ss).run()
-
-        Make sure first vertex is sent to origin::
-            sage: from flatsurf import *
-            sage: P = ConvexPolygons(QQ)
-            sage: p = P(vertices = ([(1,1),(2,1),(2,2),(1,2)]))
-            sage: s = Surface_list(QQ)
-            sage: s.add_polygon(p)
-            0
-            sage: s.change_polygon_gluings(0, [(0,2),(0,3),(0,0),(0,1)])
-            sage: s.change_base_label(0)
-            sage: ts = TranslationSurface(s)
-            sage: ts.standardize_polygons().polygon(0)
-            Polygon: (0, 0), (1, 0), (1, 1), (0, 1)
+            sage: from flatsurf.geometry.categories import TranslationSurfaces
+            sage: C = TranslationSurfaces()
+            sage: C.extra_super_categories()
+            (Category of oriented polygonal surfaces,)
+
         """
-        if self.is_finite():
-            if in_place:
-                if not self.is_mutable():
-                    raise ValueError("An in_place call for standardize_polygons can only be done for a mutable surface.")
-                s=self
-            else:
-                s=self.copy(mutable=True)
-            cv = {} # dictionary for non-zero canonical vertices
-            translations={} # translations bringing the canonical vertex to the origin.
-            for l,polygon in s.label_iterator(polygons=True):
-                best=0
-                best_pt=polygon.vertex(best)
-                for v in range(1,polygon.num_edges()):
-                    pt=polygon.vertex(v)
-                    if (pt[1]<best_pt[1]) or (pt[1]==best_pt[1] and pt[0]<best_pt[0]):
-                        best=v
-                        best_pt=pt
-                # We replace the polygon if the best vertex is not the zero vertex, or
-                # if the coordinates of the best vertex differs from the origin.
-                if not (best==0 and best_pt.is_zero()):
-                    cv[l]=best
-            for l,v in iteritems(cv):
-                s.set_vertex_zero(l,v,in_place=True)
-            return s
-        else:
-            assert in_place == False, "In place standardization only available for finite surfaces."
-            return TranslationSurface(LazyStandardizedPolygonSurface(self))
+        from flatsurf.geometry.categories.polygonal_surfaces import PolygonalSurfaces
 
-    def cmp(self, s2, limit=None):
-        r"""
-        Compare two surfaces. This is an ordering returning -1, 0, or 1.
+        return (PolygonalSurfaces().Oriented(),)
 
-        The surfaces will be considered equal if and only if there is a translation automorphism
-        respecting the polygons and the base_labels.
+    class ParentMethods:
+        r"""
+        Provides methods available to all translation surfaces in
+        sage-flatsurf.
 
-        If the two surfaces are infinite, we just examine the first limit polygons.
+        If you want to add functionality for such surfaces you most likely want
+        to put it here.
         """
-        if self.is_finite():
-            if s2.is_finite():
-                assert limit is None, "Limit only enabled for finite surfaces."
-
-                #print("comparing number of polygons")
-                sign = self.num_polygons()-s2.num_polygons()
-                if sign>0:
-                    return 1
-                if sign<0:
-                    return -1
-                #print("comparing polygons")
-                lw1=self.walker()
-                lw2=s2.walker()
-                for p1,p2 in zip(lw1.polygon_iterator(), lw2.polygon_iterator()):
-                    # Uses Polygon.cmp:
-                    ret = p1.cmp(p2)
-                    if ret != 0:
-                        return ret
-                # Polygons are identical. Compare edge gluings.
-                #print("comparing edge gluings")
-                for pair1,pair2 in zip(lw1.edge_iterator(), lw2.edge_iterator()):
-                    l1,e1 = self.opposite_edge(pair1)
-                    l2,e2 = s2.opposite_edge(pair2)
-                    num1 = lw1.label_to_number(l1)
-                    num2 = lw2.label_to_number(l2)
-                    ret = (num1 > num2) - (num1 < num2)
-                    if ret:
-                        return ret
-                    ret = (e1 > e2) - (e1 < e2)
-                    if ret:
-                        return ret
-                return 0
-            else:
-                # s1 is finite but s2 is infinite.
-                return -1
-        else:
-            if s2.is_finite():
-                # s1 is infinite but s2 is finite.
-                return 1
-            else:
-                # both surfaces are infinite.
-                lw1=self.walker()
-                lw2=s2.walker()
-                count = 0
-                for (l1,p1),(l2,p2) in zip(lw1.label_polygon_iterator(), lw2.label_polygon_iterator()):
-                    # Uses Polygon.cmp:
-                    ret = p1.cmp(p2)
-                    if ret != 0:
-                        print("Polygons differ")
-                        return ret
-                    # If here the number of edges should be equal.
-                    for e in range(p1.num_edges()):
-                        ll1,ee1 = self.opposite_edge(l1,e)
-                        ll2,ee2 = s2.opposite_edge(l2,e)
-                        num1 = lw1.label_to_number(ll1, search=True, limit=limit)
-                        num2 = lw2.label_to_number(ll2, search=True, limit=limit)
-                        ret = (num1 > num2) - (num1 < num2)
-                        if ret:
-                            return ret
-                        ret = (ee1 > ee2) - (ee1 < ee2)
-                        if ret:
-                            return ret
-                    if count >= limit:
-                        break
-                    count += 1
-                return 0
 
-    # TODO: deprecation
-    cmp_translation_surface = cmp
+        def is_translation_surface(self, positive=True):
+            r"""
+            Return whether this surface is a translation surface, i.e., return
+            ``True``.
 
-    def canonicalize_mapping(self):
-        r"""
-        Return a SurfaceMapping canonicalizing this translation surface.
-        """
-        from flatsurf.geometry.mappings import canonicalize_translation_surface_mapping, IdentityMapping
-        return canonicalize_translation_surface_mapping(self)
+            EXAMPLES::
 
-    def canonicalize(self, in_place=False):
-        r"""
-        Return a canonical version of this translation surface.
+                sage: from flatsurf import translation_surfaces
+                sage: S = translation_surfaces.square_torus()
+                sage: S.is_translation_surface(positive=True)
+                True
+                sage: S.is_translation_surface(positive=False)
+                True
 
-        EXAMPLES:
+            """
+            return True
 
-        We will check if an element lies in the Veech group::
+        @staticmethod
+        def _is_translation_surface(surface, positive=True, limit=None):
+            r"""
+            Return whether ``surface`` is a translation surface by checking how its
+            polygons are glued.
 
-            sage: from flatsurf import *
-            sage: s = translation_surfaces.octagon_and_squares()
-            sage: s
-            TranslationSurface built from 3 polygons
-            sage: a = s.base_ring().gen()
-            sage: mat = Matrix([[1,2+a],[0,1]])
-            sage: s1 = s.canonicalize()
-            sage: s1.underlying_surface().set_immutable()
-            sage: s2 = (mat*s).canonicalize()
-            sage: s2.underlying_surface().set_immutable()
-            sage: s1.cmp(s2) == 0
-            True
-            sage: hash(s1) == hash(s2)
-            True
-        """
-        # Old version
-        #return self.canonicalize_mapping().codomain()
-        if in_place:
-            if not self.is_mutable():
-                raise ValueError("canonicalize with in_place=True is only defined for mutable translation surfaces.")
-            s=self
-        else:
-            s=self.copy(mutable=True)
-        if not s.is_finite():
-            raise ValueError("canonicalize is only defined for finite translation surfaces.")
-        ret=s.delaunay_decomposition(in_place=True)
-        s.standardize_polygons(in_place=True)
-        ss=s.copy(mutable=True)
-        labels={label for label in s.label_iterator()}
-        labels.remove(s.base_label())
-        for label in labels:
-            ss.underlying_surface().change_base_label(label)
-            if ss.cmp(s)>0:
-                s.underlying_surface().change_base_label(label)
-        # We now have the base_label correct.
-        # We will use the label walker to generate the canonical labeling of polygons.
-        w=s.walker()
-        w.find_all_labels()
-        s.relabel(w.label_dictionary(), in_place=True)
-        # Set immutable
-        s.underlying_surface().set_immutable()
-        return s
+            This is a helper method for
+            :meth:`flatsurf.geometry.categories.similarity_surfaces.ParentMethods.is_translation_surface.
 
-    def rel_deformation(self, deformation, local=False, limit=100):
-        r"""
-        Perform a rel deformation of the surface and return the result.
+            INPUT:
 
-        This algorithm currently assumes that all polygons affected by this deformation are
-        triangles. That should be fixable in the future.
+            - ``surface`` -- an oriented similarity surface
 
-        INPUT:
+            - ``positive`` -- a boolean (default: ``True``); whether the
+              transformation must be a translation or is allowed to be a
+              half-translation, i.e., a translation followed by a reflection in
+              a point (equivalently, a rotation by π.)
 
-        - ``deformation`` (dictionary) - A dictionary mapping singularities of
-          the surface to deformation vectors (in some 2-dimensional vector
-          space). The rel deformation being done will move the singularities
-          (relative to each other) linearly to the provided vector for each
-          vertex. If a singularity is not included in the dictionary then the
-          vector will be treated as zero.
-
-        - ``local`` - (boolean) - If true, the algorithm attempts to deform all
-          the triangles making up the surface without destroying any of them.
-          So, the area of the triangle must be positive along the full interval
-          of time of the deformation.  If false, then the deformation must have
-          a particular form: all vectors for the deformation must be paralell.
-          In this case we achieve the deformation with the help of the SL(2,R)
-          action and Delaunay triangulations.
-
-        - ``limit`` (integer) - Restricts the length of the size of SL(2,R)
-          deformations considered. The algorithm should be roughly worst time
-          linear in limit.
+            - ``limit`` -- an integer or ``None`` (default: ``None``); if set, only
+              the first ``limit`` polygons are checked
 
-        TODO:
+            EXAMPLES::
 
-        - Support arbitrary rel deformations.
-        - Remove the requirement that triangles be used.
+                sage: from flatsurf import translation_surfaces
+                sage: S = translation_surfaces.infinite_staircase()
 
-        EXAMPLES::
+                sage: from flatsurf.geometry.categories import TranslationSurfaces
+                sage: TranslationSurfaces.ParentMethods._is_translation_surface(S, limit=8)
+                True
 
-            sage: from flatsurf import *
-            sage: s = translation_surfaces.arnoux_yoccoz(4)
-            sage: field = s.base_ring()
-            sage: a = field.gen()
-            sage: V = VectorSpace(field,2)
-            sage: deformation1 = {s.singularity(0,0):V((1,0))}
-            sage: s1 = s.rel_deformation(deformation1).canonicalize()
-            sage: deformation2 = {s.singularity(0,0):V((a,0))}
-            sage: s2 = s.rel_deformation(deformation2).canonicalize()
-            sage: m = Matrix([[a,0],[0,~a]])
-            sage: s2.cmp((m*s1).canonicalize())
-            0
-        """
-        s=self
-        # Find a common field
-        field=s.base_ring()
-        for singularity, v in iteritems(deformation):
-            if v.parent().base_field() != field:
-                from sage.structure.element import get_coercion_model
-                cm = get_coercion_model()
-                field = cm.common_parent(field, v.parent().base_field())
-        from sage.modules.free_module import VectorSpace
-        vector_space = VectorSpace(field,2)
-
-        from collections import defaultdict
-        vertex_deformation=defaultdict(vector_space.zero) # dictionary associating the vertices.
-        deformed_labels=set() # list of polygon labels being deformed.
-
-        for singularity, vect in iteritems(deformation):
-            # assert s==singularity.surface()
-            for label,v in singularity.vertex_set():
-                vertex_deformation[(label,v)]=vect
-                deformed_labels.add(label)
-                assert s.polygon(label).num_edges()==3
-
-        from flatsurf.geometry.polygon import wedge_product, ConvexPolygons
-
-        if local:
-
-            ss=s.copy(mutable=True, new_field=field)
-            us=ss.underlying_surface()
-
-            P = ConvexPolygons(field)
-            for label in deformed_labels:
-                polygon=s.polygon(label)
-                a0=vector_space(polygon.vertex(1))
-                b0=vector_space(polygon.vertex(2))
-                v0=vector_space(vertex_deformation[(label,0)])
-                v1=vector_space(vertex_deformation[(label,1)])
-                v2=vector_space(vertex_deformation[(label,2)])
-                a1=v1-v0
-                b1=v2-v0
-                # We deform by changing the triangle so that its vertices 1 and 2 have the form
-                # a0+t*a1 and b0+t*b1
-                # respectively. We are deforming from t=0 to t=1.
-                # We worry that the triangle degenerates along the way.
-                # The area of the deforming triangle has the form
-                # A0 + A1*t + A2*t^2.
-                A0 = wedge_product(a0,b0)
-                A1 = wedge_product(a0,b1)+wedge_product(a1,b0)
-                A2 = wedge_product(a1,b1)
-                if A2 != field.zero():
-                    # Critical point of area function
-                    c = A1/(-2*A2)
-                    if field.zero()<c and c<field.one():
-                        assert A0+A1*c+A2*c**2 > field.zero(), "Triangle with label %r degenerates at critical point before endpoint" % label
-                assert A0+A1+A2 > field.zero(), "Triangle with label %r degenerates at or before endpoint" % label
-                # Triangle does not degenerate.
-                us.change_polygon(label,P(vertices=[vector_space.zero(),a0+a1,b0+b1]))
-            return ss
-
-        else: # Non local deformation
-            # We can only do this deformation if all the rel vector are parallel.
-            # Check for this.
-            nonzero=None
-            for singularity, vect in iteritems(deformation):
-                vvect=vector_space(vect)
-                if vvect!=vector_space.zero():
-                    if nonzero is None:
-                        nonzero=vvect
-                    else:
-                        assert wedge_product(nonzero,vvect)==0, \
-                            "In non-local deformation all deformation vectos must be parallel"
-            assert nonzero is not None, "Deformation appears to be trivial."
-            from sage.matrix.constructor import Matrix
-            m=Matrix([[nonzero[0],-nonzero[1]],[nonzero[1],nonzero[0]]])
-            mi=~m
-            g=Matrix([[1,0],[0,2]],ring=field)
-            prod=m*g*mi
-            ss=None
-            k=0
-            while True:
-                if ss is None:
-                    ss=s.copy(mutable=True, new_field=field)
-                else:
-                    # In place matrix deformation
-                    ss.apply_matrix(prod)
-                ss.delaunay_triangulation(direction=nonzero,in_place=True)
-                deformation2={}
-                for singularity, vect in iteritems(deformation):
-                    found_start=None
-                    for label,v in singularity.vertex_set():
-                        if wedge_product(s.polygon(label).edge(v),nonzero) >= 0 and \
-                        wedge_product(nonzero,-s.polygon(label).edge((v+2)%3)) > 0:
-                            found_start=(label,v)
-                            found=None
-                            for vv in range(3):
-                                if wedge_product(ss.polygon(label).edge(vv),nonzero) >= 0 and \
-                                wedge_product(nonzero,-ss.polygon(label).edge((vv+2)%3)) > 0:
-                                    found=vv
-                                    deformation2[ss.singularity(label,vv)]=vect
-                                    break
-                            assert found is not None
-                            break
-                    assert found_start is not None
-                try:
-                    sss=ss.rel_deformation(deformation2,local=True)
-                    sss.apply_matrix(mi*g**(-k)*m)
-                    sss.delaunay_triangulation(direction=nonzero,in_place=True)
-                    return sss
-                except AssertionError as e:
-                    pass
-                k=k+1
-                if limit is not None and k>=limit:
-                    assert False, "Exeeded limit iterations"
+            ::
 
-    def j_invariant(self):
-        r"""
-        Return the Kenyon-Smillie J-invariant of this translation surface.
+                sage: from flatsurf import Polygon, similarity_surfaces
+                sage: P = Polygon(edges=[(2, 0),(-1, 3),(-1, -3)])
+                sage: S = similarity_surfaces.self_glued_polygon(P)
 
-        It is assumed that the coordinates are defined over a number field.
+                sage: TranslationSurfaces.ParentMethods._is_translation_surface(S)
+                False
+                sage: TranslationSurfaces.ParentMethods._is_translation_surface(S, positive=False)
+                True
 
-        EXAMPLES::
+            """
+            if "Oriented" not in surface.category().axioms():
+                raise NotImplementedError(
+                    "cannot decide whether a non-oriented surface is a translation surface yet"
+                )
 
-            sage: from flatsurf import *
-            sage: O = translation_surfaces.regular_octagon()
-            sage: O.j_invariant()
-            (
-                      [2 2]
-            (0), (0), [2 1]
-            )
-        """
-        it = self.label_iterator()
-        lab = next(it)
-        P = self.polygon(lab)
-        Jxx, Jyy, Jxy = P.j_invariant()
-        for lab in it:
-            xx,yy,xy = self.polygon(lab).j_invariant()
-            Jxx += xx
-            Jyy += yy
-            Jxy += xy
-        return (Jxx, Jyy, Jxy)
+            labels = surface.labels()
 
-    def erase_marked_points(self):
-        r"""
-        Return an isometric or similar surface with a minimal number of regular
-        vertices of angle 2π.
+            if limit is not None:
+                from itertools import islice
 
-        EXAMPLES::
+                labels = islice(labels, limit)
 
-            sage: import flatsurf
+            checked = set()
 
-            sage: G = SymmetricGroup(4)
-            sage: S = flatsurf.translation_surfaces.origami(G('(1,2,3,4)'), G('(1,4,2,3)'))
-            sage: S.stratum()
-            H_2(2, 0)
-            sage: S.erase_marked_points().stratum() # optional: pyflatsurf  # long time (1s)
-            H_2(2)
-
-            sage: for (a,b,c) in [(1,4,11), (1,4,15), (3,4,13)]: # long time (10s), optional: pyflatsurf
-            ....:     T = flatsurf.polygons.triangle(a,b,c)
-            ....:     S = flatsurf.similarity_surfaces.billiard(T)
-            ....:     S = S.minimal_cover("translation")
-            ....:     print(S.erase_marked_points().stratum())
-            H_6(10)
-            H_6(2^5)
-            H_8(12, 2)
-
-        If the surface had no marked points then it is returned unchanged by this
-        function::
-
-            sage: O = flatsurf.translation_surfaces.regular_octagon()
-            sage: O.erase_marked_points() is O
-            True
-
-        TESTS:
-
-        Verify that https://github.com/flatsurf/flatsurf/issues/263 has been resolved::
-
-            sage: from flatsurf import EquiangularPolygons, similarity_surfaces
-            sage: E = EquiangularPolygons((10, 8, 3, 1, 1, 1))
-            sage: P = E((1, 1, 2, 4), normalized=True)
-            sage: B = similarity_surfaces.billiard(P, rational=True)
-            sage: S = B.minimal_cover(cover_type="translation")
-            sage: S = S.erase_marked_points() # long time (3s), optional: pyflatsurf
-
-        ::
-
-            sage: from flatsurf import EquiangularPolygons, similarity_surfaces
-            sage: E = EquiangularPolygons((10, 7, 2, 2, 2, 1))
-            sage: P = E((1, 1, 2, 3), normalized=True)
-            sage: B = similarity_surfaces.billiard(P, rational=True)
-            sage: S_mp = B.minimal_cover(cover_type="translation")
-            sage: S = S_mp.erase_marked_points() # long time (3s), optional: pyflatsurf
+            for label in labels:
+                for edge in range(len(surface.polygon(label).vertices())):
+                    cross = surface.opposite_edge(label, edge)
 
-        """
-        if all(a != 1 for a in self.angles()):
-            # no 2π angle
-            return self
-        from .pyflatsurf_conversion import from_pyflatsurf, to_pyflatsurf
-        S = to_pyflatsurf(self)
-        S.delaunay()
-        S = S.eliminateMarkedPoints().surface()
-        S.delaunay()
-        return from_pyflatsurf(S)
+                    if cross is None:
+                        continue
 
+                    if cross in checked:
+                        continue
 
-class MinimalTranslationCover(Surface):
-    r"""
-    Do not use translation_surface.MinimalTranslationCover. Use 
-    minimal_cover.MinimalTranslationCover instead. This class is being
-    deprecated.
-    """
-    def __init__(self, similarity_surface):
-        if similarity_surface.underlying_surface().is_mutable():
-            if similarity_surface.is_finite():
-                self._ss=similarity_surface.copy()
-            else:
-                raise ValueError("Can not construct MinimalTranslationCover of a surface that is mutable and infinite.")
-        else:
-            self._ss = similarity_surface
-
-        # We are finite if and only if self._ss is a finite RationalConeSurface.
-        if not self._ss.is_finite():
-            finite = False
-        else:
-            try:
-                from flatsurf.geometry.rational_cone_surface import RationalConeSurface
-                ss_copy = self._ss.reposition_polygons(relabel=True)
-                rcs = RationalConeSurface(ss_copy)
-                rcs._test_edge_matrix()
-                finite=True
-            except AssertionError:
-                # print("Warning: Could be indicating infinite surface falsely.")
-                finite=False
-
-        I = identity_matrix(self._ss.base_ring(),2)
-        I.set_immutable()
-        base_label=(self._ss.base_label(), I)
+                    checked.add((label, edge))
 
-        Surface.__init__(self, self._ss.base_ring(), base_label, finite=finite, mutable=False)
+                    # We do not call self.edge_matrix() since the surface might
+                    # have overridden this (just returning the identity matrix e.g.)
+                    # and we want to deduce the matrix from the attached polygon
+                    # edges instead.
+                    from flatsurf.geometry.categories import SimilaritySurfaces
 
-    def polygon(self, lab):
-        r"""
-        EXAMPLES::
+                    matrix = SimilaritySurfaces.Oriented.ParentMethods.edge_matrix.f(  # pylint: disable=no-member
+                        surface, label, edge
+                    )
 
-            sage: from flatsurf import *
-            sage: C = translation_surfaces.chamanara(1/2)
-            sage: C.polygon('a')
-            Traceback (most recent call last):
-            ...
-            ValueError: invalid label 'a'
-        """
-        if not isinstance(lab, tuple) or len(lab) != 2:
-            raise ValueError("invalid label {!r}".format(lab))
-        p = self._ss.polygon(lab[0])
-        return lab[1] * self._ss.polygon(lab[0])
-
-    def opposite_edge(self, p, e):
-        pp,m = p  # this is the polygon m * ss.polygon(p)
-        p2,e2 = self._ss.opposite_edge(pp,e)
-        me = self._ss.edge_matrix(pp,e)
-        mm = ~me * m
-        mm.set_immutable()
-        return ((p2,mm),e2)
-
-class AbstractOrigami(Surface):
-    r'''Abstract base class for origamis.
-    Realization needs just to define a _domain and four cardinal directions.
-    '''
-    def __init__(self, domain, base_label=None):
-        self._domain=domain
-        if base_label is None:
-            base_label = domain.an_element()
-        from sage.rings.rational_field import QQ
-        Surface.__init__(self,QQ,base_label,finite=domain.is_finite(),mutable=False)
-
-    def up(self, label):
-        raise NotImplementedError
-
-    def down(self, label):
-        raise NotImplementedError
-
-    def right(self, label):
-        raise NotImplementedError
+                    if not matrix.is_diagonal():
+                        return False
 
-    def left(self, label):
-        raise NotImplementedError
+                    if matrix[0][0] == 1 and matrix[1][1] == 1:
+                        continue
 
-    def _repr_(self):
-        return "Some AbstractOrigami"
+                    if matrix[0][0] == -1 and matrix[1][1] == -1:
+                        if not positive:
+                            continue
 
-    def num_polygons(self):
-        r"""
-        Returns the number of polygons.
-        """
-        return self._domain.cardinality()
+                    return False
 
-    def polygon_labels(self):
-        return self._domain
+            return True
 
-    def polygon(self, lab):
-        if lab not in self._domain:
-            #Updated to print a possibly useful error message
-            raise ValueError("Label "+str(lab)+" is not in the domain")
-        from flatsurf.geometry.polygon import polygons
-        return polygons.square()
-
-    def opposite_edge(self, p, e):
-        if p not in self._domain:
-            raise ValueError
-        if e==0:
-            return self.down(p),2
-        if e==1:
-            return self.right(p),3
-        if e==2:
-            return self.up(p),0
-        if e==3:
-            return self.left(p),1
-        raise ValueError
-
-
-class Origami(AbstractOrigami):
-    def __init__(self, r, u, rr=None, uu=None, domain=None, base_label=None):
-        if domain is None:
-            domain = r.parent().domain()
-
-        self._r = r
-        self._u = u
-        if rr is None:
-            rr = ~r
-        else:
-            for a in domain.some_elements():
-                if r(rr(a)) != a:
-                    raise ValueError("r o rr is not identity on %s"%a)
-                if rr(r(a)) != a:
-                    raise ValueError("rr o r is not identity on %s"%a)
-        if uu is None:
-            uu = ~u
-        else:
-            for a in domain.some_elements():
-                if u(uu(a)) != a:
-                    raise ValueError("u o uu is not identity on %s"%a)
-                if uu(u(a)) != a:
-                    raise ValueError("uu o u is not identity on %s"%a)
-
-        self._perms = [uu,r,u,rr] # down,right,up,left
-        AbstractOrigami.__init__(self,domain,base_label)
-
-    def opposite_edge(self, p, e):
-        if p not in self._domain:
-            raise ValueError("Polygon label p="+str(p)+" is not in domain="+str(self._domain))
-        if e < 0 or e > 3:
-            raise ValueError("Edge value e="+str(e)+" does not satisfy 0<=e<4.")
-        return self._perms[e](p), (e+2)%4
-
-    def up(self, label):
-        return self.opposite_edge(label,2)[0]
-
-    def down(self, label):
-        return self.opposite_edge(label,0)[0]
-
-    def right(self, label):
-        return self.opposite_edge(label,1)[0]
+        def minimal_translation_cover(self):
+            r"""
+            Return the minimal cover of this surface that makes this surface a
+            translation surface, i.e., return this surface itself.
 
-    def left(self, label):
-        return self.opposite_edge(label,3)[0]
+            EXAMPLES::
 
-    def _repr_(self):
-        return "Origami defined by r=%s and u=%s"%(self._r,self._u)
+                sage: from flatsurf import translation_surfaces
+                sage: S = translation_surfaces.square_torus()
+                sage: S.minimal_translation_cover() is S
+                True
 
+            """
+            return self
 
-class LazyStandardizedPolygonSurface(Surface):
-    r"""
-    This class handles standardizing polygons for infinite translation surfaces.
-    See the TranslationSurface.standardize_polygons method.
+        def edge_matrix(self, p, e=None):
+            r"""
+            Returns the 2x2 matrix representing a similarity which when
+            applied to the polygon with label `p` makes it so the edge `e`
+            can be glued to its opposite edge by translation.
+
+            Since this is a translation surface, this is just the identity.
+
+            EXAMPLES::
+
+                sage: from flatsurf import translation_surfaces
+                sage: S = translation_surfaces.square_torus()
+                sage: S.edge_matrix(0, 0)
+                [1 0]
+                [0 1]
+
+            """
+            if e is None:
+                import warnings
+
+                warnings.warn(
+                    "passing only a single tuple argument to edge_matrix() has been deprecated and will be deprecated in a future version of sage-flatsurf; pass the label and edge index as separate arguments instead"
+                )
+                p, e = p
+
+            if e < 0 or e >= len(self.polygon(p).vertices()):
+                raise ValueError("invalid edge index for this polygon")
+
+            from sage.all import identity_matrix
+
+            return identity_matrix(self.base_ring(), 2)
+
+        def canonicalize_mapping(self):
+            r"""
+            Return a SurfaceMapping canonicalizing this translation surface.
+            """
+            from flatsurf.geometry.mappings import (
+                canonicalize_translation_surface_mapping,
+            )
 
-    This class should not be instantiated directly.
-    Instead use TranslationSurface.standardize_polygons.
-    """
+            return canonicalize_translation_surface_mapping(self)
+
+        def rel_deformation(self, deformation, local=False, limit=100):
+            r"""
+            Perform a rel deformation of the surface and return the result.
+
+            This algorithm currently assumes that all polygons affected by this deformation are
+            triangles. That should be fixable in the future.
+
+            INPUT:
+
+            - ``deformation`` (dictionary) - A dictionary mapping singularities of
+              the surface to deformation vectors (in some 2-dimensional vector
+              space). The rel deformation being done will move the singularities
+              (relative to each other) linearly to the provided vector for each
+              vertex. If a singularity is not included in the dictionary then the
+              vector will be treated as zero.
+
+            - ``local`` - (boolean) - If true, the algorithm attempts to deform all
+              the triangles making up the surface without destroying any of them.
+              So, the area of the triangle must be positive along the full interval
+              of time of the deformation.  If false, then the deformation must have
+              a particular form: all vectors for the deformation must be parallel.
+              In this case we achieve the deformation with the help of the SL(2,R)
+              action and Delaunay triangulations.
+
+            - ``limit`` (integer) - Restricts the length of the size of SL(2,R)
+              deformations considered. The algorithm should be roughly worst time
+              linear in limit.
+
+            .. TODO::
+
+                - Support arbitrary rel deformations.
+                - Remove the requirement that triangles be used.
+
+            EXAMPLES::
+
+                sage: from flatsurf import translation_surfaces
+                sage: s = translation_surfaces.arnoux_yoccoz(4)
+                sage: field = s.base_ring()
+                sage: a = field.gen()
+                sage: V = VectorSpace(field,2)
+                sage: deformation1 = {s.singularity(0,0):V((1,0))}
+                doctest:warning
+                ...
+                UserWarning: Singularity() is deprecated and will be removed in a future version of sage-flatsurf. Use surface.point() instead.
+                sage: s1 = s.rel_deformation(deformation1).canonicalize()  # long time (.8s)
+                sage: deformation2 = {s.singularity(0,0):V((a,0))}  # long time (see above)
+                sage: s2 = s.rel_deformation(deformation2).canonicalize()  # long time (.6s)
+                sage: m = Matrix([[a,0],[0,~a]])
+                sage: s2.cmp((m*s1).canonicalize())  # long time (see above)
+                0
+
+            """
+            s = self
+            # Find a common field
+            field = s.base_ring()
+            for singularity, v in deformation.items():
+                if v.parent().base_field() != field:
+                    from sage.structure.element import get_coercion_model
+
+                    cm = get_coercion_model()
+                    field = cm.common_parent(field, v.parent().base_field())
+            from sage.modules.free_module import VectorSpace
+
+            vector_space = VectorSpace(field, 2)
+
+            from collections import defaultdict
+
+            vertex_deformation = defaultdict(
+                vector_space.zero
+            )  # dictionary associating the vertices.
+            deformed_labels = set()  # list of polygon labels being deformed.
+
+            for singularity, vect in deformation.items():
+                for label, coordinates in singularity.representatives():
+                    v = self.polygon(label).get_point_position(coordinates).get_vertex()
+                    vertex_deformation[(label, v)] = vect
+                    deformed_labels.add(label)
+                    assert len(s.polygon(label).vertices()) == 3
+
+            from flatsurf.geometry.euclidean import ccw
+
+            if local:
+                from flatsurf.geometry.surface import MutableOrientedSimilaritySurface
+
+                ss = MutableOrientedSimilaritySurface.from_surface(s)
+                ss.set_immutable()
+                ss = MutableOrientedSimilaritySurface.from_surface(
+                    ss.change_ring(field)
+                )
+                us = ss
+
+                for label in deformed_labels:
+                    polygon = s.polygon(label)
+                    a0 = vector_space(polygon.vertex(1))
+                    b0 = vector_space(polygon.vertex(2))
+                    v0 = vector_space(vertex_deformation[(label, 0)])
+                    v1 = vector_space(vertex_deformation[(label, 1)])
+                    v2 = vector_space(vertex_deformation[(label, 2)])
+                    a1 = v1 - v0
+                    b1 = v2 - v0
+                    # We deform by changing the triangle so that its vertices 1 and 2 have the form
+                    # a0+t*a1 and b0+t*b1
+                    # respectively. We are deforming from t=0 to t=1.
+                    # We worry that the triangle degenerates along the way.
+                    # The area of the deforming triangle has the form
+                    # A0 + A1*t + A2*t^2.
+                    A0 = ccw(a0, b0)
+                    A1 = ccw(a0, b1) + ccw(a1, b0)
+                    A2 = ccw(a1, b1)
+                    if A2:
+                        # Critical point of area function
+                        c = A1 / (-2 * A2)
+                        if field.zero() < c and c < 1:
+                            if A0 + A1 * c + A2 * c**2 <= 0:
+                                raise ValueError(
+                                    "Triangle with label %r degenerates at critical point before endpoint"
+                                    % label
+                                )
+                    if A0 + A1 + A2 <= field.zero():
+                        raise ValueError(
+                            "Triangle with label %r degenerates at or before endpoint"
+                            % label
+                        )
+                    # Triangle does not degenerate.
+                    from flatsurf import Polygon
+
+                    us.replace_polygon(
+                        label,
+                        Polygon(
+                            vertices=[vector_space.zero(), a0 + a1, b0 + b1],
+                            base_ring=field,
+                        ),
+                    )
+                ss.set_immutable()
+                return ss
+
+            else:  # Non local deformation
+                # We can only do this deformation if all the rel vector are parallel.
+                # Check for this.
+                nonzero = None
+                for singularity, vect in deformation.items():
+                    vvect = vector_space(vect)
+                    if vvect != vector_space.zero():
+                        if nonzero is None:
+                            nonzero = vvect
+                        else:
+                            assert (
+                                ccw(nonzero, vvect) == 0
+                            ), "In non-local deformation all deformation vectos must be parallel"
+                assert nonzero is not None, "Deformation appears to be trivial."
+                from sage.matrix.constructor import Matrix
+
+                m = Matrix([[nonzero[0], -nonzero[1]], [nonzero[1], nonzero[0]]])
+                mi = ~m
+                g = Matrix([[1, 0], [0, 2]], ring=field)
+                prod = m * g * mi
+                ss = None
+                k = 0
+                while True:
+                    if ss is None:
+                        from flatsurf.geometry.surface import (
+                            MutableOrientedSimilaritySurface,
+                        )
+
+                        ss = MutableOrientedSimilaritySurface.from_surface(
+                            s.change_ring(field),
+                            category=TranslationSurfaces(),
+                        )
+                    else:
+                        # In place matrix deformation
+                        ss.apply_matrix(prod)
+                    ss.delaunay_triangulation(direction=nonzero, in_place=True)
+                    deformation2 = {}
+                    for singularity, vect in deformation.items():
+                        found_start = None
+                        for label, coordinates in singularity.representatives():
+                            v = (
+                                s.polygon(label)
+                                .get_point_position(coordinates)
+                                .get_vertex()
+                            )
+                            if (
+                                ccw(s.polygon(label).edge(v), nonzero) >= 0
+                                and ccw(nonzero, -s.polygon(label).edge((v + 2) % 3))
+                                > 0
+                            ):
+                                found_start = (label, v)
+                                found = None
+                                for vv in range(3):
+                                    if (
+                                        ccw(ss.polygon(label).edge(vv), nonzero) >= 0
+                                        and ccw(
+                                            nonzero,
+                                            -ss.polygon(label).edge((vv + 2) % 3),
+                                        )
+                                        > 0
+                                    ):
+                                        found = vv
+                                        deformation2[
+                                            ss.point(
+                                                label, ss.polygon(label).vertex(vv)
+                                            )
+                                        ] = vect
+                                        break
+                                assert found is not None
+                                break
+                        assert found_start is not None
+
+                    try:
+                        sss = ss.rel_deformation(deformation2, local=True)
+                    except ValueError:
+                        k += 1
+                        if limit is not None and k >= limit:
+                            raise Exception("exceeded limit iterations")
+                        continue
+
+                    sss = sss.apply_matrix(mi * g ** (-k) * m, in_place=False)
+                    return sss.delaunay_triangulation(direction=nonzero)
+
+        def j_invariant(self):
+            r"""
+            Return the Kenyon-Smillie J-invariant of this translation surface.
+
+            It is assumed that the coordinates are defined over a number field.
+
+            EXAMPLES::
+
+                sage: from flatsurf import translation_surfaces
+                sage: O = translation_surfaces.regular_octagon()
+                sage: O.j_invariant()
+                (
+                          [2 2]
+                (0), (0), [2 1]
+                )
+            """
+            it = iter(self.labels())
+            lab = next(it)
+            P = self.polygon(lab)
+            Jxx, Jyy, Jxy = P.j_invariant()
+            for lab in it:
+                xx, yy, xy = self.polygon(lab).j_invariant()
+                Jxx += xx
+                Jyy += yy
+                Jxy += xy
+            return (Jxx, Jyy, Jxy)
+
+        def erase_marked_points(self):
+            r"""
+            Return an isometric or similar surface with a minimal number of regular
+            vertices of angle 2π.
+
+            EXAMPLES::
+
+                sage: import flatsurf
+
+                sage: G = SymmetricGroup(4)
+                sage: S = flatsurf.translation_surfaces.origami(G('(1,2,3,4)'), G('(1,4,2,3)'))
+                sage: S.stratum()
+                H_2(2, 0)
+                sage: S.erase_marked_points().stratum() # optional: pyflatsurf  # long time (1s)  # random output due to matplotlib warnings with some combinations of setuptools and matplotlib
+                H_2(2)
+
+                sage: for (a,b,c) in [(1,4,11), (1,4,15), (3,4,13)]: # long time (10s), optional: pyflatsurf
+                ....:     T = flatsurf.polygons.triangle(a,b,c)
+                ....:     S = flatsurf.similarity_surfaces.billiard(T)
+                ....:     S = S.minimal_cover("translation")
+                ....:     print(S.erase_marked_points().stratum())
+                H_6(10)
+                H_6(2^5)
+                H_8(12, 2)
+
+            If the surface had no marked points then it is returned unchanged by this
+            function::
+
+                sage: O = flatsurf.translation_surfaces.regular_octagon()
+                sage: O.erase_marked_points() is O
+                True
+
+            TESTS:
+
+            Verify that https://github.com/flatsurf/flatsurf/issues/263 has been resolved::
+
+                sage: from flatsurf import Polygon, similarity_surfaces
+                sage: P = Polygon(angles=(10, 8, 3, 1, 1, 1), lengths=(1, 1, 2, 4))
+                sage: B = similarity_surfaces.billiard(P)
+                sage: S = B.minimal_cover(cover_type="translation")
+                sage: S = S.erase_marked_points() # long time (3s), optional: pyflatsurf
+
+            ::
+
+                sage: from flatsurf import Polygon, similarity_surfaces
+                sage: P = Polygon(angles=(10, 7, 2, 2, 2, 1), lengths=(1, 1, 2, 3))
+                sage: B = similarity_surfaces.billiard(P)
+                sage: S_mp = B.minimal_cover(cover_type="translation")
+                sage: S = S_mp.erase_marked_points() # long time (3s), optional: pyflatsurf
+
+            """
+            if all(a != 1 for a in self.angles()):
+                # no 2π angle
+                return self
+            from flatsurf.geometry.pyflatsurf_conversion import (
+                from_pyflatsurf,
+                to_pyflatsurf,
+            )
 
-    def __init__(self, surface, relabel=False):
-        self._s = surface.copy(mutable=True, relabel=relabel)
-        self._labels = set()
-        Surface.__init__(self, self._s.base_ring(), self._s.base_label(), finite=self._s.is_finite(), mutable=False)
-
-    def standardize(self, label):
-        best=0
-        polygon = self._s.polygon(label)
-        best_pt=polygon.vertex(best)
-        for v in range(1,polygon.num_edges()):
-            pt=polygon.vertex(v)
-            if (pt[1]<best_pt[1]) or (pt[1]==best_pt[1] and pt[0]<best_pt[0]):
-                best=v
-                best_pt=pt
-        if best!=0:
-            self._s.set_vertex_zero(label,best,in_place=True)
-        self._labels.add(label)
+            S = to_pyflatsurf(self)
+            S.delaunay()
+            S = S.eliminateMarkedPoints().surface()
+            S.delaunay()
+            return from_pyflatsurf(S)
+
+        def _test_translation_surface(self, **options):
+            r"""
+            Verify that this is a translation surface.
+
+            EXAMPLES::
+
+                sage: from flatsurf import translation_surfaces
+                sage: S = translation_surfaces.square_torus()
+                sage: S._test_translation_surface()
+
+            """
+            tester = self._tester(**options)
+
+            limit = None
+
+            if not self.is_finite_type():
+                limit = 32
+
+            tester.assertTrue(
+                TranslationSurfaces.ParentMethods._is_translation_surface(
+                    self, limit=limit
+                )
+            )
 
-    def polygon(self, label):
+    class FiniteType(SurfaceCategoryWithAxiom):
         r"""
-        Return the polygon with the provided label.
+        The category of translation surfaces built from finitely many polygons.
 
-        This method must be overriden in subclasses.
-        """
-        if label in self._labels:
-            return self._s.polygon(label)
-        else:
-            self.standardize(label)
-            return self._s.polygon(label)
+        EXAMPLES::
 
-    def opposite_edge(self, l, e):
-        r"""
-        Given the label ``l`` of a polygon and an edge ``e`` in that polygon
-        returns the pair (``ll``, ``ee``) to which this edge is glued.
+            sage: from flatsurf import translation_surfaces
+            sage: s = translation_surfaces.octagon_and_squares()
+            sage: s.category()
+            Category of connected without boundary finite type translation surfaces
 
-        This method must be overriden in subclasses.
         """
-        if l not in self._labels:
-            self.standardize(l)
-        ll,ee = self._s.opposite_edge(l,e)
-        if ll in self._labels:
-            return (ll,ee)
-        else:
-            self.standardize(ll)
-            return self._s.opposite_edge(l,e)
+
+        class WithoutBoundary(SurfaceCategoryWithAxiom):
+            r"""
+            The category of translation surfaces without boundary built from
+            finitely many polygons.
+
+            EXAMPLES::
+
+                sage: from flatsurf import translation_surfaces
+                sage: s = translation_surfaces.octagon_and_squares()
+                sage: s.category()
+                Category of connected without boundary finite type translation surfaces
+
+            """
+
+            class ParentMethods:
+                r"""
+                Provides methods available to all translation surfaces that are
+                built from finitely many polygons.
+
+                If you want to add functionality for such surfaces you most likely
+                want to put it here.
+                """
+
+                def stratum(self):
+                    r"""
+                    Return the stratum this surface belongs to.
+
+                    This uses the package ``surface-dynamics``
+                    (see http://www.labri.fr/perso/vdelecro/flatsurf_sage.html)
+
+                    EXAMPLES::
+
+                        sage: import flatsurf.geometry.similarity_surface_generators as sfg
+                        sage: sfg.translation_surfaces.octagon_and_squares().stratum()
+                        H_3(4)
+
+                    """
+                    from surface_dynamics import AbelianStratum
+                    from sage.rings.integer_ring import ZZ
+
+                    return AbelianStratum([ZZ(a - 1) for a in self.angles()])
+
+                def canonicalize(self, in_place=None):
+                    r"""
+                    Return a canonical version of this translation surface.
+
+                    EXAMPLES:
+
+                    We will check if an element lies in the Veech group::
+
+                        sage: from flatsurf import translation_surfaces
+                        sage: s = translation_surfaces.octagon_and_squares()
+                        sage: s
+                        Translation Surface in H_3(4) built from 2 squares and a regular octagon
+                        sage: from flatsurf.geometry.categories import TranslationSurfaces
+                        sage: s in TranslationSurfaces()
+                        True
+                        sage: a = s.base_ring().gen()
+                        sage: mat = Matrix([[1,2+a],[0,1]])
+                        sage: s1 = s.canonicalize()
+                        sage: s1.set_immutable()
+                        sage: s2 = (mat*s).canonicalize()
+                        sage: s2.set_immutable()
+                        sage: s1.cmp(s2) == 0
+                        True
+                        sage: hash(s1) == hash(s2)
+                        True
+
+                    """
+                    if in_place is not None:
+                        if in_place:
+                            raise NotImplementedError(
+                                "calling canonicalize(in_place=True) is not supported anymore"
+                            )
+
+                        import warnings
+
+                        warnings.warn(
+                            "the in_place keyword of canonicalize() has been deprecated and will be removed in a future version of sage-flatsurf"
+                        )
+
+                    s = self.delaunay_decomposition().standardize_polygons()
+
+                    from flatsurf.geometry.surface import (
+                        MutableOrientedSimilaritySurface,
+                    )
+
+                    s = MutableOrientedSimilaritySurface.from_surface(s)
+
+                    from flatsurf.geometry.surface import (
+                        MutableOrientedSimilaritySurface,
+                    )
+
+                    ss = MutableOrientedSimilaritySurface.from_surface(s)
+
+                    for label in ss.labels():
+                        ss.set_roots([label])
+                        if ss.cmp(s) > 0:
+                            s.set_roots([label])
+
+                    # We have chosen the root label such that this surface is minimal.
+                    # Now we relabel all the polygons so that they are natural
+                    # numbers in the order of the walk on the surface.
+                    labels = {label: i for (i, label) in enumerate(s.labels())}
+                    s.relabel(labels, in_place=True)
+                    s.set_immutable()
+                    return s
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/graphical/__init__.py` & `sage_flatsurf-0.5.0/flatsurf/graphical/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 r"""
-The goal of this package is to prepare geometric objects for rendering in a figure or in a gui. 
+The goal of this package is to prepare geometric objects for rendering in a figure or in a gui.
 This package is intended to support graphical output via matplotlib.
 """
-#*****************************************************************************
-#       Copyright (C) 2013-2019 Vincent Delecroix <20100.delecroix@gmail.com>
-#                     2013-2019 W. Patrick Hooper <wphooper@gmail.com>
+# ****************************************************************************
+#  This file is part of sage-flatsurf.
 #
-#  Distributed under the terms of the GNU General Public License (GPL)
-#  as published by the Free Software Foundation; either version 2 of
-#  the License, or (at your option) any later version.
-#                  https://www.gnu.org/licenses/
-#*****************************************************************************
+#       Copyright (C) 2013-2019 Vincent Delecroix
+#                     2013-2019 W. Patrick Hooper
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+# ****************************************************************************
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/graphical/polygon.py` & `sage_flatsurf-0.5.0/flatsurf/graphical/polygon.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,39 @@
-#*****************************************************************************
-#       Copyright (C) 2013-2019 Vincent Delecroix <20100.delecroix@gmail.com>
-#                     2013-2019 W. Patrick Hooper <wphooper@gmail.com>
+# ****************************************************************************
+#  This file is part of sage-flatsurf.
 #
-#  Distributed under the terms of the GNU General Public License (GPL)
-#  as published by the Free Software Foundation; either version 2 of
-#  the License, or (at your option) any later version.
-#                  https://www.gnu.org/licenses/
-#*****************************************************************************
-
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
-
+#       Copyright (C) 2016-2019 Vincent Delecroix
+#                     2016-2018 W. Patrick Hooper
+#                     2022-2023 Julian Rüth
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License along
+#  with sage-flatsurf. If not, see <http://www.gnu.org/licenses/>.
+# ****************************************************************************
 from sage.rings.real_double import RDF
 from sage.modules.free_module import VectorSpace
 from sage.plot.polygon import polygon2d
-from sage.plot.graphics import Graphics
 from sage.plot.text import text
 from sage.plot.line import line2d
 from sage.plot.point import point2d
 
 from flatsurf.geometry.similarity import SimilarityGroup
 
 V = VectorSpace(RDF, 2)
 
+
 class GraphicalPolygon:
     r"""
     Stores data necessary to draw one of the polygons from a surface.
 
     Note that this involves converting between geometric coordinates, defined for the SimilaritySurface,
     and graphical coordinates. We do this with a similarity (called transformation below).
     """
@@ -60,15 +67,15 @@
 
     def __repr__(self):
         r"""
         String representation.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import similarity_surfaces
             sage: s = similarity_surfaces.example()
             sage: gs = s.graphical_surface()
             sage: gs.graphical_polygon(0)
             GraphicalPolygon with vertices [(0.0, 0.0), (2.0, -2.0), (2.0, 0.0)]
         """
         return "GraphicalPolygon with vertices {}".format(self._v)
 
@@ -123,19 +130,19 @@
             To fit with Sage conventions this should be ymax
         """
         return max([v[1] for v in self._v])
 
     def bounding_box(self):
         r"""
         Return the quadruple (x1,y1,x2,y2) where x1 and y1 are the minimal
-        x- and y-coordinates and x2 and y2 are the maximal x-and y- cordinates.
+        x and y coordinates and x2 and y2 are the maximal x and y coordinates.
         """
         return self.xmin(), self.ymin(), self.xmax(), self.ymax()
 
-    def transform(self, point, double_precision = True):
+    def transform(self, point, double_precision=True):
         r"""
         Return the transformation of point into graphical coordinates.
 
         By default returned point is in double precision. This can be changed
         to an exact representation by setting `double_precision` to False.
         """
         if self._transformation is None:
@@ -169,15 +176,15 @@
     def transformation(self):
         r"""
         Return the transformation (similarity) which converts from
         mathematical to graphical coordinates.
         """
         return self._transformation
 
-    def set_transformation(self, transformation = None):
+    def set_transformation(self, transformation=None):
         r"""Set the transformation to be applied to the polygon."""
         if transformation is None:
             self._transformation = SimilarityGroup(self._p.base_ring()).one()
         else:
             self._transformation = transformation
         # recompute the location of vertices:
         self._v = [V(self._transformation(v)) for v in self._p.vertices()]
@@ -185,15 +192,15 @@
     def plot_polygon(self, **options):
         r"""
         Returns only the filled polygon.
 
         Options are processed as in sage.plot.polygon.polygon2d except
         that by default axes=False.
         """
-        if not "axes" in options:
+        if "axes" not in options:
             options["axes"] = False
         return polygon2d(self._v, **options)
 
     def plot_label(self, label, **options):
         r"""
         Write the label of the polygon as text.
 
@@ -212,16 +219,18 @@
     def plot_edge(self, e, **options):
         r"""
         Plot the edge e, with e a number 0,...,n-1 with n being the number
         of edges of the polygon.
 
         Options are processed as in sage.plot.line.line2d.
         """
-        return line2d([self._v[e], self._v[(e+1)%self.base_polygon().num_edges()]], \
-            **options)
+        return line2d(
+            [self._v[e], self._v[(e + 1) % len(self.base_polygon().vertices())]],
+            **options
+        )
 
     def plot_edge_label(self, i, label, **options):
         r"""
         Write label on the i-th edge.
 
         A parameter ``t`` in the interval [0,1] can be provided to position the
         label along the edge. A value of t=0 will position it at the starting
@@ -232,73 +241,75 @@
         or "edge" to indicate if the label should be drawn outside the polygon,
         inside the polygon or on the edge. Defaults to "inside".
 
         A ``push_off`` perturbation parameter controls how far off the edge the label is pushed.
 
         Other options are processed as in sage.plot.text.text.
         """
-        e = self._v[(i+1)%self.base_polygon().num_edges()] - self._v[i]
+        e = self._v[(i + 1) % len(self.base_polygon().vertices())] - self._v[i]
 
         if "position" in options:
             if options["position"] not in ["inside", "outside", "edge"]:
-                raise ValueError("The 'position' parameter must take the value 'inside', 'outside', or 'edge'.")
+                raise ValueError(
+                    "The 'position' parameter must take the value 'inside', 'outside', or 'edge'."
+                )
             pos = options.pop("position")
         else:
             pos = "inside"
 
         if pos == "outside":
             # position outside polygon.
             if "horizontal_alignment" in options:
                 pass
             elif e[1] > 0:
-                options["horizontal_alignment"]="left"
+                options["horizontal_alignment"] = "left"
             elif e[1] < 0:
-                options["horizontal_alignment"]="right"
+                options["horizontal_alignment"] = "right"
             else:
-                options["horizontal_alignment"]="center"
+                options["horizontal_alignment"] = "center"
 
             if "vertical_alignment" in options:
                 pass
             elif e[0] > 0:
-                options["vertical_alignment"]="top"
+                options["vertical_alignment"] = "top"
             elif e[0] < 0:
-                options["vertical_alignment"]="bottom"
+                options["vertical_alignment"] = "bottom"
             else:
-                options["vertical_alignment"]="center"
+                options["vertical_alignment"] = "center"
 
         elif pos == "inside":
             # position inside polygon.
             if "horizontal_alignment" in options:
                 pass
             elif e[1] < 0:
-                options["horizontal_alignment"]="left"
+                options["horizontal_alignment"] = "left"
             elif e[1] > 0:
-                options["horizontal_alignment"]="right"
+                options["horizontal_alignment"] = "right"
             else:
-                options["horizontal_alignment"]="center"
+                options["horizontal_alignment"] = "center"
 
             if "vertical_alignment" in options:
                 pass
             elif e[0] < 0:
-                options["vertical_alignment"]="top"
+                options["vertical_alignment"] = "top"
             elif e[0] > 0:
-                options["vertical_alignment"]="bottom"
+                options["vertical_alignment"] = "bottom"
             else:
-                options["vertical_alignment"]="center"
+                options["vertical_alignment"] = "center"
 
         else:
             # centered on edge.
             if "horizontal_alignment" in options:
                 pass
             else:
-                options["horizontal_alignment"]="center"
+                options["horizontal_alignment"] = "center"
             if "vertical_alignment" in options:
                 pass
             else:
-                options["vertical_alignment"]="center"
+                options["vertical_alignment"] = "center"
 
         if "t" in options:
             t = RDF(options.pop("t"))
         else:
             t = 0.3
 
         if "push_off" in options:
@@ -323,33 +334,33 @@
         Other options are processed as in sage.plot.line.line2d.
         """
         if "t" in options:
             t = RDF(options.pop("t"))
         else:
             t = 0.5
 
-        return line2d([self._v[0], self._v[0] + t*(sum(self._v) / len(self._v) - self._v[0])],
-            **options)
+        return line2d(
+            [self._v[0], self._v[0] + t * (sum(self._v) / len(self._v) - self._v[0])],
+            **options
+        )
 
     def plot_points(self, points, **options):
         r"""
         Plot the points in the given collection of points.
 
         The options are passed to point2d.
 
         If no "zorder" option is provided then we set "zorder" to 50.
 
         By default coordinates are taken in the underlying surface. Call with coordinates="graphical"
         to use graphical coordinates instead.
         """
         if "zorder" not in options:
-            options["zorder"]=50
+            options["zorder"] = 50
         if "coordinates" not in options:
             points2 = [self.transform(point) for point in points]
-        elif options["coordinates"]=="graphical":
-            points2=[V(point) for point in points]
+        elif options["coordinates"] == "graphical":
+            points2 = [V(point) for point in points]
             del options["coordinates"]
         else:
             raise ValueError("Invalid value of 'coordinates' option")
         return point2d(points=points2, **options)
-   
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/graphical/straight_line_trajectory.py` & `sage_flatsurf-0.5.0/flatsurf/graphical/straight_line_trajectory.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,48 @@
-#*****************************************************************************
-#       Copyright (C) 2013-2019 Vincent Delecroix <20100.delecroix@gmail.com>
-#                     2013-2019 W. Patrick Hooper <wphooper@gmail.com>
+# ****************************************************************************
+#  This file is part of sage-flatsurf.
 #
-#  Distributed under the terms of the GNU General Public License (GPL)
-#  as published by the Free Software Foundation; either version 2 of
-#  the License, or (at your option) any later version.
-#                  https://www.gnu.org/licenses/
-#*****************************************************************************
-
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
-
-from flatsurf.graphical.surface import GraphicalSurface
-# The real vector space:
-from flatsurf.graphical.polygon import V
+#       Copyright (C) 2013-2019 Vincent Delecroix
+#                     2013-2019 W. Patrick Hooper
+#                     2022-2023 Julian Rüth
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+# ****************************************************************************
 
-from flatsurf.geometry.straight_line_trajectory import SegmentInPolygon, StraightLineTrajectory
 
 class GraphicalSegmentInPolygon:
     def __init__(self, segment, graphical_surface):
         r"""
         Create a graphical segment from a graphical surface and a SegmentInPolygon.
         """
         self._gs = graphical_surface
         self._seg = segment
-        label=self.polygon_label()
-        self._start=self._gs.graphical_polygon(label).transform(segment.start().point())
+        label = self.polygon_label()
+        self._start = self._gs.graphical_polygon(label).transform(
+            segment.start().point()
+        )
         if self._seg.is_edge():
-            self._end=self._gs.graphical_polygon(label).transform(self._seg.start().polygon().vertex(self._seg.edge()+1))
+            self._end = self._gs.graphical_polygon(label).transform(
+                self._seg.start().polygon().vertex(self._seg.edge() + 1)
+            )
         else:
-            self._end=self._gs.graphical_polygon(label).transform(segment.end().point())
+            self._end = self._gs.graphical_polygon(label).transform(
+                segment.end().point()
+            )
 
     def polygon_label(self):
         return self._seg.polygon_label()
 
     def start(self):
         r"""Return the start point as a RDF Vector."""
         return self._start
@@ -42,61 +51,68 @@
         r"""Return the end point as a RDF Vector."""
         return self._end
 
     def plot(self, **options):
         r"""
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import similarity_surfaces
             sage: s = similarity_surfaces.example()
             sage: v = s.tangent_vector(0, (1,-0.5), (3,-1))
             sage: from flatsurf.geometry.straight_line_trajectory import SegmentInPolygon
             sage: seg = SegmentInPolygon(v)
-            sage: from flatsurf.graphical.straight_line_trajectory import *
+            sage: from flatsurf.graphical.straight_line_trajectory import GraphicalSegmentInPolygon
             sage: gseg = GraphicalSegmentInPolygon(seg, s.graphical_surface())
-            sage: gseg.plot()                # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 1 graphics primitive
-            sage: gseg.plot(color='red')     # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 1 graphics primitive
+            sage: gseg.plot()
+            ...Graphics object consisting of 1 graphics primitive
+            sage: gseg.plot(color='red')
+            ...Graphics object consisting of 1 graphics primitive
         """
         if self._gs.is_visible(self.polygon_label()):
             from sage.plot.line import line2d
-            return line2d([self.start(), self.end()],**options)
+
+            return line2d([self.start(), self.end()], **options)
         else:
             from sage.plot.graphics import Graphics
+
             return Graphics()
 
+
 class GraphicalStraightLineTrajectory:
     r"""
     Allows for the rendering of a straight-line trajectory through a graphical surface.
     """
-    def __init__(self, trajectory, graphical_surface = None):
+
+    def __init__(self, trajectory, graphical_surface=None):
         if graphical_surface is None:
             self._gs = trajectory.surface().graphical_surface()
         else:
-            assert trajectory.surface() == graphical_surface.get_surface()
+            if trajectory.surface() != graphical_surface.get_surface():
+                raise ValueError
             self._gs = graphical_surface
         self._traj = trajectory
-        self._segments = [GraphicalSegmentInPolygon(s, self._gs) for s in self._traj.segments()]
+        self._segments = [
+            GraphicalSegmentInPolygon(s, self._gs) for s in self._traj.segments()
+        ]
 
     def plot(self, **options):
         r"""
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import similarity_surfaces
             sage: s = similarity_surfaces.example()
             sage: gs = s.graphical_surface()
             sage: K.<sqrt2>=NumberField(x^2-2,embedding=1)
             sage: v = s.tangent_vector(0, (1,-1), (sqrt2,-1),ring=K)
             sage: traj = v.straight_line_trajectory()
             sage: traj.flow(100)
             sage: traj.flow(-5)
             sage: gtraj = traj.graphical_trajectory(gs)
-            sage: gs.plot() + gtraj.plot()      # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 119 graphics primitives
+            sage: gs.plot() + gtraj.plot()
+            ...Graphics object consisting of 119 graphics primitives
         """
         from sage.plot.graphics import Graphics
+
         p = Graphics()
         for seg in self._segments:
             p += seg.plot(**options)
         return p
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/graphical/surface.py` & `sage_flatsurf-0.5.0/flatsurf/graphical/surface.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,316 +1,321 @@
 r"""
 EXAMPLES::
 
     sage: import flatsurf
     sage: flatsurf.translation_surfaces.veech_2n_gon(4).plot()
-    Graphics object consisting of 18 graphics primitives
+    ...Graphics object consisting of 18 graphics primitives
+
 """
-#*****************************************************************************
+# ****************************************************************************
+#  This file is part of sage-flatsurf.
+#
 #       Copyright (C) 2013-2019 Vincent Delecroix <20100.delecroix@gmail.com>
 #                     2013-2019 W. Patrick Hooper <wphooper@gmail.com>
+#                     2022-2023 Julian Rüth <julian.rueth@fsfe.org>
 #
-#  Distributed under the terms of the GNU General Public License (GPL)
-#  as published by the Free Software Foundation; either version 2 of
-#  the License, or (at your option) any later version.
-#                  https://www.gnu.org/licenses/
-#*****************************************************************************
-
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
-from six import iteritems
-
-from flatsurf.geometry.similarity_surface import SimilaritySurface
-from .polygon import *
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+# ****************************************************************************
 
 from sage.rings.integer_ring import ZZ
 from sage.rings.rational_field import QQ
 from sage.modules.free_module_element import vector
 
+
 class GraphicalSurface:
     r"""
     This class manages the rendering of a SimilaritySurface.
 
     This class essentially consists of a collection of GraphicalPolygons which
     control how individual polygons are positioned. In addition, this class
     stores options which are passed to the polygons when they are rendered.
 
     Some setup features set in the constructor and can be set again later via
-    `process_options()`.
+    :meth:`process_options`.
 
     The basic tasks of the class are to render the polygons, edges and labels.
     To customize a rendering, it is useful to know something about how this
     class works. (Apologies!)
 
     There are attributes which control whether or not certain objects are
     rendered, namely:
 
-    - `will_plot_polygons` -- Whether to plot polygons which are right-side up.
+    - ``will_plot_polygons`` -- Whether to plot polygons which are right-side up.
 
-    - `will_plot_upside_down_polygons` -- Whether to plot polygons which are
+    - ``will_plot_upside_down_polygons`` -- Whether to plot polygons which are
         upside down. Defaults to False.
 
-    - `will_plot_polygon_labels` -- Whether to plot polygon labels.
+    - ``will_plot_polygon_labels`` -- Whether to plot polygon labels.
 
-    - `will_plot_edges` -- If this is False then no edges will be plotted.
+    - ``will_plot_edges`` -- If this is False then no edges will be plotted.
 
-    - `will_plot_non_adjacent_edges` = Whether to plot polygon edges which are
+    - ``will_plot_non_adjacent_edges`` = Whether to plot polygon edges which are
         not adjacent to the edge it is glued to.
 
-    - `will_plot_adjacent_edges` -- Whether to plot polygon edges which are
+    - ``will_plot_adjacent_edges`` -- Whether to plot polygon edges which are
         adjacent to the polygon they are glued to.
 
-    - `will_plot_self_glued_edges` -- Whether to plot polygon edges which are
+    - ``will_plot_self_glued_edges`` -- Whether to plot polygon edges which are
         glued to themselves.
 
-    - `will_plot_edge_labels` -- Whether to plot polygon edges labels.
+    - ``will_plot_edge_labels`` -- Whether to plot polygon edges labels.
 
-    - `will_plot_zero_flags` -- Whether to plot line segments from the
+    - ``will_plot_zero_flags`` -- Whether to plot line segments from the
         baricenter to the zero vertex of each polygon. Useful in working out
         vertex and edge labels. Defaults to False.
 
-    The `plot` method calls some other built in methods: `plot_polygon`,
-    `plot_polygon_label`, `plot_edge` and `plot_edge_label`. These in turn
-    call methods in `GraphicalPolygon`.
+    The :meth:`plot` method calls some other built in methods: :meth:`plot_polygon`,
+    :meth:`plot_polygon_label`, :meth:`plot_edge` and :meth:`plot_edge_label`. These in turn
+    call methods in :class:`~.polygon.GraphicalPolygon`.
 
-    - `polygon_options` -- Options passed to :func:`graphical_polygon.GraphicalPolygon.plot_polygon` when
+    - ``polygon_options`` -- Options passed to :meth:`.polygon.GraphicalPolygon.plot_polygon` when
         plotting a polygon right-side up.
 
-    - `upside_down_polygon_options` -- Options passed to
-        :func:`graphical_polygon.GraphicalPolygon.plot_polygon` when plotting a polygon upside-down.
+    - ``upside_down_polygon_options`` -- Options passed to
+        :meth:`.polygon.GraphicalPolygon.plot_polygon` when plotting a polygon upside-down.
 
-    - `polygon_label_options` -- Options passed to :func:`graphical_polygon.GraphicalPolygon.plot_label`
+    - ``polygon_label_options`` -- Options passed to :meth:`.polygon.GraphicalPolygon.plot_label`
         when plotting a polygon label.
 
-    - `non_adjacent_edge_options` -- Options passed to
-        :func:`graphical_polygon.GraphicalPolygon.plot_edge` when plotting a polygon edge which is not
+    - ``non_adjacent_edge_options`` -- Options passed to
+        :meth:`.polygon.GraphicalPolygon.plot_edge` when plotting a polygon edge which is not
         adjacent to the edge it is glued to.
 
-    - `self.adjacent_edge_options` -- Options passed to
-        :func:`graphical_polygon.GraphicalPolygon.plot_edge` when plotting a polygon edge which is
+    - ``adjacent_edge_options`` -- Options passed to
+        :meth:`.polygon.GraphicalPolygon.plot_edge` when plotting a polygon edge which is
         adjacent to the edge it is glued to.
 
-    - `self_glued_edge_options` -- Options passed to :func:`graphical_polygon.GraphicalPolygon.plot_edge`
+    - ``self_glued_edge_options`` -- Options passed to :meth:`.polygon.GraphicalPolygon.plot_edge`
         when plotting a polygon edge which is glued to itself.
 
-    - `edge_label_options` -- Options passed to :func:`graphical_polygon.GraphicalPolygon.edge_label`
+    - ``edge_label_options`` -- Options passed to :meth:`.polygon.GraphicalPolygon.plot_edge_label`
         when plotting a edge label.
 
-    - `zero_flag_options` -- Options passed to
-        :func:`graphical_polygon.GraphicalPolygon.plot_zero_flag` when plotting a zero_flag.
+    - ``zero_flag_options`` -- Options passed to
+        :meth:`.polygon.GraphicalPolygon.plot_zero_flag` when plotting a zero_flag.
 
-    EXAMPLES::
+    INPUT:
 
-        sage: from flatsurf import *
-        sage: from flatsurf.graphical.surface import GraphicalSurface
+    - ``similarity_surface`` -- a similarity surface
 
-        sage: s = similarity_surfaces.example()
-        sage: gs = GraphicalSurface(s)
-        sage: gs.polygon_options["color"]="red"
-        sage: gs.plot()     # not tested (problem with matplotlib font caches on Travis)
-        Graphics object consisting of 13 graphics primitives
-    """
+    - ``polygon_labels`` -- a boolean (default ``True``) whether the label
+      of polygons are displayed
 
-    def __init__(self, similarity_surface, adjacencies=None, polygon_labels=True, \
-                 edge_labels="gluings", default_position_function = None):
-        r"""
-        Construct a GraphicalSurface from a similarity surface.
+    - ``edge_labels`` -- option to control the display of edge labels. It
+      can be one of
 
-        INPUT:
+        - ``False`` or ``None`` for no labels
 
-        - ``similarity_surface`` -- a similarity surface
+        - ``'gluings'`` -- to put on each side of each non-adjacent edge, the
+          name of the polygon to which it is glued
 
-        - ``polygon_labels`` -- a boolean (default ``True``) whether the label
-          of polygons are displayed
+        - ``'number'`` -- to put on each side of each edge the number of the
+          edge
 
-        - ``edge_labels`` -- option to control the display of edge labels. It
-          can be one of
+        - ``'gluings and number'`` -- full information
 
-            - ``False`` or ``None`` for no labels
+        - ``'letter'`` -- add matching letters to glued edges in an arbitrary way
 
-            - ``'gluings'`` -- to put on each side of each non-adjacent edge, the
-              name of the polygon to which it is glued
+    - ``adjacencies`` -- a list of pairs ``(p,e)`` to be used to set
+      adjacencies of polygons.
 
-            - ``'number'`` -- to put on each side of each edge the number of the
-              edge
+    - ``default_position_function`` -- a function mapping polygon labels to
+      similarities describing the position of the corresponding polygon.
 
-            - ``'gluings and number'`` -- full information
+    If adjacencies is not defined and the surface is finite, make_all_visible()
+    is called to make all polygons visible.
 
-            - ``'letter'`` -- add matching letters to glued edges in an arbitrary way
+    EXAMPLES::
 
-        - ``adjacencies`` -- a list of pairs ``(p,e)`` to be used to set
-          adjacencies of polygons.
+        sage: from flatsurf import similarity_surfaces
+        sage: from flatsurf.graphical.surface import GraphicalSurface
 
-        - ``default_position_function`` -- a function mapping polygon labels to
-          similarities describing the position of the corresponding polygon.
+        sage: s = similarity_surfaces.example()
+        sage: gs = GraphicalSurface(s)
+        sage: gs.polygon_options["color"]="red"
+        sage: gs.plot()
+        ...Graphics object consisting of 13 graphics primitives
 
-        If adjacencies is not defined and the surface is finite, make_all_visible()
-        is called to make all polygons visible.
-        """
-        assert isinstance(similarity_surface, SimilaritySurface)
-        self._ss = similarity_surface
+    """
+
+    def __init__(
+        self,
+        surface,
+        adjacencies=None,
+        polygon_labels=True,
+        edge_labels="gluings",
+        default_position_function=None,
+    ):
+        self._ss = surface
         self._default_position_function = default_position_function
         self._polygons = {}
-        self._visible = set([self._ss.base_label()])
+
+        if not self._ss.is_connected():
+            raise NotImplementedError("cannot plot disconnected surfaces yet")
+
+        self._visible = set(self._ss.roots())
 
         if adjacencies is None:
-            if self._ss.is_finite():
+            if self._ss.is_finite_type():
                 self.make_all_visible()
         self._edge_labels = None
 
         self.will_plot_polygons = True
         r"""
         Whether to plot polygons which are right-side up.
         """
 
-        self.polygon_options = {"color":"lightgray"}
-        r"""Options passed to :func:`graphical_polygon.GraphicalPolygon.plot_polygon` when plotting a polygon right-side up."""
+        self.polygon_options = {"color": "lightgray"}
+        r"""Options passed to :meth:`.polygon.GraphicalPolygon.plot_polygon` when plotting a polygon right-side up."""
 
         self.will_plot_upside_down_polygons = False
         r"""
         Whether to plot polygons which are upside down
         """
 
-        self.upside_down_polygon_options = {"color":"lightgray", "zorder":-1}
-        r"""Options passed to :func:`graphical_polygon.GraphicalPolygon.plot_polygon` when plotting a polygon upside-down."""
+        self.upside_down_polygon_options = {"color": "lightgray", "zorder": -1}
+        r"""Options passed to :meth:`.polygon.GraphicalPolygon.plot_polygon` when plotting a polygon upside-down."""
 
         self.will_plot_polygon_labels = True
         r"""
         Whether to plot polygon labels.
         """
 
-        self.polygon_label_options = {"color":"black", "vertical_alignment":"center", "horizontal_alignment":"center"}
-        r"""Options passed to :func:`graphical_polygon.GraphicalPolygon.plot_label` when plotting a polygon label."""
+        self.polygon_label_options = {
+            "color": "black",
+            "vertical_alignment": "center",
+            "horizontal_alignment": "center",
+        }
+        r"""Options passed to :meth:`.polygon.GraphicalPolygon.plot_label` when plotting a polygon label."""
 
         self.will_plot_edges = True
         r"""
         If this is False then no edges will be plotted.
         """
 
         self.will_plot_non_adjacent_edges = True
         r"""
         Whether to plot polygon edges which are not adjacent to the edge it is glued to.
         """
 
-        self.non_adjacent_edge_options = {"color":"blue"}
-        r"""Options passed to :func:`graphical_polygon.GraphicalPolygon.plot_edge` when plotting a polygon edge
+        self.non_adjacent_edge_options = {"color": "blue"}
+        r"""Options passed to :meth:`.polygon.GraphicalPolygon.plot_edge` when plotting a polygon edge
         which is not adjacent to the edge it is glued to."""
 
         self.will_plot_adjacent_edges = True
         r"""
         Whether to plot polygon edges which are adjacent to the polygon they are glued to.
         """
 
-        self.adjacent_edge_options = {"color":"blue", "linestyle":":"}
-        r"""Options passed to :func:`graphical_polygon.GraphicalPolygon.plot_edge`
+        self.adjacent_edge_options = {"color": "blue", "linestyle": ":"}
+        r"""Options passed to :meth:`.polygon.GraphicalPolygon.plot_edge`
         when plotting a polygon edge which is adjacent to the edge it is glued to."""
 
         self.will_plot_self_glued_edges = True
         r"""
         Whether to plot polygon edges which are glued to themselves.
         """
 
-        self.self_glued_edge_options = {"color":"red"}
-        r"""Options passed to :func:`graphical_polygon.GraphicalPolygon.plot_edge` when plotting a polygon edge
+        self.self_glued_edge_options = {"color": "red"}
+        r"""Options passed to :meth:`.polygon.GraphicalPolygon.plot_edge` when plotting a polygon edge
         which is glued to itself."""
 
         self.will_plot_edge_labels = True
         r"""
         Whether to plot polygon edges which are not adjacent to the polygon they are glued to.
         """
 
-        self.edge_label_options = {"color":"blue"}
-        r"""Options passed to :func:`graphical_polygon.GraphicalPolygon.edge_label` when plotting a polygon label."""
+        self.edge_label_options = {"color": "blue"}
+        r"""Options passed to :meth:`.polygon.GraphicalPolygon.plot_edge_label` when plotting a polygon label."""
 
         self.will_plot_zero_flags = False
         r"""
         Whether to plot line segments from the baricenter to the zero vertex of each polygon.
         """
 
-        self.zero_flag_options = {"color":"green", "thickness":0.5}
-        r"""Options passed to :func:`graphical_polygon.GraphicalPolygon.plot_zero_flag` when plotting a zero_flag."""
+        self.zero_flag_options = {"color": "green", "thickness": 0.5}
+        r"""Options passed to :meth:`.polygon.GraphicalPolygon.plot_zero_flag` when plotting a zero_flag."""
 
-        self.process_options(adjacencies=adjacencies,
-                polygon_labels=polygon_labels, edge_labels=edge_labels)
-
-    def process_options(self, adjacencies=None, polygon_labels=None, edge_labels=None, default_position_function = None):
+        self.process_options(
+            adjacencies=adjacencies,
+            polygon_labels=polygon_labels,
+            edge_labels=edge_labels,
+        )
+
+    def process_options(
+        self,
+        adjacencies=None,
+        polygon_labels=None,
+        edge_labels=None,
+        default_position_function=None,
+    ):
         r"""
         Process the options listed as if the graphical_surface was first
         created.
 
         INPUT:
 
-        - ``adjacencies`` -- a list of pairs ``(p,e)`` to be used to set
-          adjacencies of polygons.
-
-        - ``polygon_labels`` -- a boolean (default ``True``) whether the label
-          of polygons are displayed
-
-        - ``edge_labels`` -- option to control the display of edge labels. It
-          can be one of
-
-            - ``None`` for no change
-
-            - ``False`` for no labels
-
-            - ``'gluings'`` -- to put on each side of each non-adjacent edge, the
-              name of the polygon to which it is glued
-
-            - ``'number'`` -- to put on each side of each edge the number of the
-              edge
-
-            - ``'gluings and number'`` -- full information
-
-            - ``'letter'`` -- add matching letters to glued edges in an arbitrary way
-
-        - ``default_position_function`` -- a function mapping polygon labels to
-          similarities describing the position of the corresponding polygon.
-          Note that this will not affect polygons which have already been
-          positioned.
+        Consult :class:`GraphicalSurface` for the possible arguments.
 
         TESTS::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
 
             sage: c = translation_surfaces.chamanara(1/2)
             sage: gs = c.graphical_surface()
             sage: gs.process_options(edge_labels='hey')
             Traceback (most recent call last):
             ...
             ValueError: invalid value for edge_labels (='hey')
         """
         if adjacencies is not None:
-            for p,e in adjacencies:
+            for p, e in adjacencies:
                 self.make_adjacent(p, e)
+
         if polygon_labels is not None:
             if not isinstance(polygon_labels, bool):
                 raise ValueError("polygon_labels must be True, False or None.")
             self.will_plot_polygon_labels = polygon_labels
+
         if edge_labels is not None:
             if edge_labels is True:
-                self.will_plot_edge_labels = True
-                edge_labels = 'gluings'
-            elif edge_labels is False:
+                edge_labels = "gluings"
+
+            if edge_labels is False:
+                self._edge_labels = None
                 self.will_plot_edge_labels = False
-                edge_labels = None
-            elif edge_labels in ['gluings', 'number', 'gluings and number', 'letter']:
+            elif edge_labels in ["gluings", "number", "gluings and number", "letter"]:
                 self._edge_labels = edge_labels
                 self.will_plot_edge_labels = True
             else:
-                raise ValueError("invalid value for edge_labels (={!r})".format(edge_labels))
+                raise ValueError(
+                    "invalid value for edge_labels (={!r})".format(edge_labels)
+                )
+
         if default_position_function is not None:
             self._default_position_function = default_position_function
 
     def copy(self):
         r"""
         Make a copy of this GraphicalSurface.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import translation_surfaces
             sage: s = translation_surfaces.octagon_and_squares()
             sage: gs = s.graphical_surface()
             sage: gs.will_plot_zero_flags = True
             sage: gs.graphical_polygon(1).transformation()
             (x, y) |-> (x + 2, y)
             sage: gs.make_adjacent(0,2)
             sage: gs.graphical_polygon(1).transformation()
@@ -322,15 +327,18 @@
             sage: gs2.will_plot_zero_flags
             True
             sage: gs2.graphical_polygon(1).transformation()
             (x, y) |-> (x + (a + 4), y + (a + 2))
             sage: gs2.polygon_options
             {'color': 'yellow'}
         """
-        gs = GraphicalSurface(self.get_surface(), default_position_function = self._default_position_function)
+        gs = GraphicalSurface(
+            self.get_surface(),
+            default_position_function=self._default_position_function,
+        )
 
         # Copy plot options
         gs.will_plot_polygons = self.will_plot_polygons
         gs.polygon_options = dict(self.polygon_options)
         gs.will_plot_upside_down_polygons = self.will_plot_upside_down_polygons
         gs.upside_down_polygon_options = dict(self.upside_down_polygon_options)
         gs.will_plot_polygon_labels = self.will_plot_polygon_labels
@@ -344,30 +352,30 @@
         gs.self_glued_edge_options = dict(self.self_glued_edge_options)
         gs.will_plot_edge_labels = self.will_plot_edge_labels
         gs.edge_label_options = dict(self.edge_label_options)
         gs.will_plot_zero_flags = self.will_plot_zero_flags
         gs.zero_flag_options = dict(self.zero_flag_options)
 
         # Copy polygons and visible set.
-        gs._polygons = {label:gp.copy() for label,gp in iteritems(self._polygons)}
+        gs._polygons = {label: gp.copy() for label, gp in self._polygons.items()}
         gs._visible = set(self._visible)
         gs._edge_labels = self._edge_labels
 
         return gs
 
     def __repr__(self):
-        return "Graphical version of Similarity Surface {!r}".format(self._ss)
+        return "Graphical representation of {!r}".format(self._ss)
 
     def visible(self):
         r"""
         Return a copy of the set of visible labels.
         """
         return set(self._visible)
 
-    def is_visible(self,label):
+    def is_visible(self, label):
         r"""
         Return whether the polygon with the given label is marked as visible.
         """
         return label in self._visible
 
     def make_visible(self, label):
         r"""
@@ -391,83 +399,91 @@
           set to be adjacent or not. Defaults to true unless a default_position_function was
           provided.
 
         - ``limit`` -- (default ``None``) maximal number of additional polygons to make visible
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import similarity_surfaces
 
             sage: s = similarity_surfaces.example()
             sage: g = s.graphical_surface()
             sage: g.make_all_visible()
-            sage: g.plot()      # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 13 graphics primitives
+            sage: g.plot()
+            ...Graphics object consisting of 13 graphics primitives
 
             sage: s = similarity_surfaces.example()
-            sage: g = s.graphical_surface(cached=False, adjacencies=[])
+            sage: g = s.graphical_surface(adjacencies=[])
             sage: g.make_all_visible(adjacent=False)
-            sage: g.plot()      # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 16 graphics primitives
+            sage: g.plot()
+            ...Graphics object consisting of 16 graphics primitives
         """
         if adjacent is None:
-            adjacent = (self._default_position_function is None)
+            adjacent = self._default_position_function is None
         if limit is None:
-            assert self._ss.is_finite()
+            if not self._ss.is_finite_type():
+                raise NotImplementedError
             if adjacent:
-                for l,poly in self._ss.walker().label_polygon_iterator():
-                    for e in range(poly.num_edges()):
-                        l2,e2 = self._ss.opposite_edge(l,e)
+                for label, poly in zip(self._ss.labels(), self._ss.polygons()):
+                    for e in range(len(poly.vertices())):
+                        l2, e2 = self._ss.opposite_edge(label, e)
                         if not self.is_visible(l2):
-                            self.make_adjacent(l,e)
+                            self.make_adjacent(label, e)
             else:
                 from flatsurf.geometry.similarity import SimilarityGroup
+
                 T = SimilarityGroup(self._ss.base_ring())
-                for l in self._ss.label_iterator():
-                    if not self.is_visible(l):
+                for label in self._ss.labels():
+                    if not self.is_visible(label):
                         if self._default_position_function is None:
                             # No reasonable way to display the polygon, so we do this hack:
-                            g = self.graphical_polygon(l)
-                            poly = self._ss.polygon(l)
-                            sxmax = self.xmax()
-                            pxmin = g.xmin()
-                            t = T((QQ(self.xmax() - g.xmin() + 1),
-                                QQ(-(g.ymin()+g.ymax()) / ZZ(2) )))
+                            g = self.graphical_polygon(label)
+                            poly = self._ss.polygon(label)
+                            t = T(
+                                (
+                                    QQ(self.xmax() - g.xmin() + 1),
+                                    QQ(-(g.ymin() + g.ymax()) / ZZ(2)),
+                                )
+                            )
                             g.set_transformation(t)
-                        self.make_visible(l)
+                        self.make_visible(label)
         else:
-            assert limit>0
+            if limit <= 0:
+                raise ValueError
             if adjacent:
                 i = 0
-                for l,poly in self._ss.walker().label_polygon_iterator():
-                    for e in range(poly.num_edges()):
-                        l2,e2 = self._ss.opposite_edge(l,e)
+                for label, poly in zip(self._ss.labels(), self._ss.polygons()):
+                    for e in range(len(poly.vertices())):
+                        l2, e2 = self._ss.opposite_edge(label, e)
                         if not self.is_visible(l2):
-                            self.make_adjacent(l,e)
-                            i=i+1
-                            if i>=limit:
+                            self.make_adjacent(label, e)
+                            i = i + 1
+                            if i >= limit:
                                 return
             else:
                 from flatsurf.geometry.similarity import SimilarityGroup
+
                 T = SimilarityGroup(self._ss.base_ring())
                 i = 0
-                for l in self._ss.label_iterator():
-                    if not self.is_visible(l):
+                for label in self._ss.labels():
+                    if not self.is_visible(label):
                         if self._default_position_function is None:
                             # No reasonable way to display the polygon, so we do this hack:
-                            g = self.graphical_polygon(l)
-                            poly = self._ss.polygon(l)
-                            sxmax = self.xmax()
-                            pxmin = g.xmin()
-                            t = T((QQ(self.xmax() - g.xmin() + 1),
-                                QQ(-(g.ymin()+g.ymax()) / ZZ(2) )))
+                            g = self.graphical_polygon(label)
+                            poly = self._ss.polygon(label)
+                            t = T(
+                                (
+                                    QQ(self.xmax() - g.xmin() + 1),
+                                    QQ(-(g.ymin() + g.ymax()) / ZZ(2)),
+                                )
+                            )
                             g.set_transformation(t)
-                        self.make_visible(l)
-                        i=i+1
-                        if i>=limit:
+                        self.make_visible(label)
+                        i = i + 1
+                        if i >= limit:
                             return
 
     def get_surface(self):
         r"""
         Return the underlying similarity surface.
         """
         return self._ss
@@ -500,133 +516,137 @@
         """
         return max([self.graphical_polygon(label).ymax() for label in self.visible()])
 
     def bounding_box(self):
         r"""
         Return the quadruple (x1,y1,x2,y2) where x1 and y1 are the minimal
         x- and y-coordinates of a visible graphical polygon and x2 and y2 are the
-        maximal x-and y- cordinates  of a visible graphical polygon.
+        maximal x-and y- coordinates of a visible graphical polygon.
         """
         return self.xmin(), self.ymin(), self.xmax(), self.ymax()
 
-
     def graphical_polygon(self, label):
         r"""
         Return the graphical_polygon with the given label.
         """
         if label in self._polygons:
             return self._polygons[label]
         else:
             t = None
-            if not self._default_position_function is None:
-                t=self._default_position_function(label)
+            if self._default_position_function is not None:
+                t = self._default_position_function(label)
+            from flatsurf.graphical.polygon import GraphicalPolygon
+
             p = GraphicalPolygon(self._ss.polygon(label), transformation=t)
             self._polygons[label] = p
             return p
 
-    def make_adjacent(self, p, e, reverse = False, visible = True):
+    def make_adjacent(self, p, e, reverse=False, visible=True):
         r"""
         Move the polygon across the prescribed edge so that is adjacent.
         The polygon moved is obtained from opposite_edge(p,e).
 
         If reverse=True then the polygon is moved so that there is a fold
         at the edge.
 
         If visible is True (by default), we also make the moved polygon visible.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import similarity_surfaces
             sage: s = similarity_surfaces.example()
             sage: gs = s.graphical_surface(adjacencies=[])
             sage: gs.graphical_polygon(0)
             GraphicalPolygon with vertices [(0.0, 0.0), (2.0, -2.0), (2.0, 0.0)]
             sage: gs.graphical_polygon(1)
             GraphicalPolygon with vertices [(0.0, 0.0), (2.0, 0.0), (1.0, 3.0)]
             sage: print("Polygon 0, edge 0 is opposite "+str(gs.opposite_edge(0,0)))
             Polygon 0, edge 0 is opposite (1, 1)
             sage: gs.make_adjacent(0,0)
             sage: gs.graphical_polygon(0)
             GraphicalPolygon with vertices [(0.0, 0.0), (2.0, -2.0), (2.0, 0.0)]
             sage: gs.graphical_polygon(1)
             GraphicalPolygon with vertices [(0.4, -2.8), (2.0, -2.0), (0.0, 0.0)]
         """
-        pp,ee = self._ss.opposite_edge(p,e)
+        pp, ee = self._ss.opposite_edge(p, e)
         if reverse:
             from flatsurf.geometry.similarity import SimilarityGroup
+
             G = SimilarityGroup(self._ss.base_ring())
 
             q = self._ss.polygon(p)
             a = q.vertex(e)
-            b = q.vertex(e+1)
+            b = q.vertex(e + 1)
             # This is the similarity carrying the origin to a and (1,0) to b:
-            g = G(b[0]-a[0],b[1]-a[1],a[0],a[1])
+            g = G(b[0] - a[0], b[1] - a[1], a[0], a[1])
 
             qq = self._ss.polygon(pp)
-            aa = qq.vertex(ee+1)
+            aa = qq.vertex(ee + 1)
             bb = qq.vertex(ee)
             # This is the similarity carrying the origin to aa and (1,0) to bb:
-            gg = G(bb[0]-aa[0],bb[1]-aa[1],aa[0],aa[1])
+            gg = G(bb[0] - aa[0], bb[1] - aa[1], aa[0], aa[1])
 
             reflection = G(
                 self._ss.base_ring().one(),
                 self._ss.base_ring().zero(),
                 self._ss.base_ring().zero(),
                 self._ss.base_ring().zero(),
-                -1)
+                -1,
+            )
 
             # This is the similarity carrying (a,b) to (aa,bb):
-            g = gg*reflection*(~g)
+            g = gg * reflection * (~g)
         else:
-            g = self._ss.edge_transformation(pp,ee)
+            g = self._ss.edge_transformation(pp, ee)
         h = self.graphical_polygon(p).transformation()
-        self.graphical_polygon(pp).set_transformation(h*g)
+        self.graphical_polygon(pp).set_transformation(h * g)
         if visible:
             self.make_visible(pp)
 
-    def make_adjacent_and_visible(self, p, e, reverse=False):
-        r"""
-        Move the polygon across the prescribed edge so that is adjacent,
-        and make the moved polygon visible.
-        """
-        from sage.misc.superseded import deprecation
-        deprecation(42, "Do not use .make_adjacent_and_visible(). Use .make_adjacent() instead.")
-        self.make_adjacent(p, e, reverse=reverse)
-
-    def is_adjacent(self,p,e):
+    def is_adjacent(self, p, e):
         r"""
         Returns the truth value of the statement
         'The polygon opposite edge (p,e) is adjacent to that edge.'
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import similarity_surfaces
             sage: s = similarity_surfaces.example()
             sage: g = s.graphical_surface(adjacencies=[])
             sage: g.is_adjacent(0,0)
             False
             sage: g.is_adjacent(0,1)
             False
             sage: g.make_all_visible(adjacent=True)
             sage: g.is_adjacent(0,0)
             True
             sage: g.is_adjacent(0,1)
             False
         """
-        pp,ee = self.opposite_edge(p,e)
+        pp, ee = self.opposite_edge(p, e)
         if not self.is_visible(pp):
             return False
         g = self.graphical_polygon(p)
         gg = self.graphical_polygon(pp)
-        return g.transformed_vertex(e) == gg.transformed_vertex(ee+1) and \
-               g.transformed_vertex(e+1) == gg.transformed_vertex(ee)
-
-    def to_surface(self, point, v=None, label=None, ring=None, return_all=False, \
-                   singularity_limit=None, search_all = False, search_limit=None):
-        r""" Converts from graphical coordinates to similarity surface coordinates.
+        return g.transformed_vertex(e) == gg.transformed_vertex(
+            ee + 1
+        ) and g.transformed_vertex(e + 1) == gg.transformed_vertex(ee)
+
+    def to_surface(
+        self,
+        point,
+        v=None,
+        label=None,
+        ring=None,
+        return_all=False,
+        singularity_limit=None,
+        search_all=False,
+        search_limit=None,
+    ):
+        r"""Converts from graphical coordinates to similarity surface coordinates.
 
         A point always must be provided. If a vector v is provided then a
         SimilaritySurfaceTangentVector will be returned. If v is not provided, then a
         SurfacePoint is returned.
 
         INPUT:
 
@@ -650,219 +670,248 @@
             return a set of all points we find instead.
 
         - ``singularity_limit`` -- (default ``None``) This only has an effect
             if returning a singular point (i.e., ``v`` is ``None``) and the
             surface is infinite. In this case, the singularity should be
             returned but it could be infinite. Then singularity_limit controls
             how far we look for the singularity to close. This value is passed
-            to ``SimilaritySurface.surface_point``.
+            to the ``point()`` method on the surface.
 
         - ``search_all`` -- (default ``False``) By default we look just in
-            polygons with visible label. If set to `True``, then we instead
+            polygons with visible label. If set to ``True``, then we instead
             look in all labels.
 
         - ``search_limit`` -- (default ``None``) If ``search_all`` is ``True``,
             then we look at the first ``search_limit`` polygons instead of all
             polygons. This must be set to an positive integer if ``search_all``
             is and the surface is infinite.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import similarity_surfaces
             sage: s = similarity_surfaces.example()
             sage: gs = s.graphical_surface()
             sage: gs.to_surface((1,-2))
-            Surface point located at (1, 1/2) in polygon 1
+            Point (1, 1/2) of polygon 1
             sage: gs.to_surface((1,-2), v=(1,0))
             SimilaritySurfaceTangentVector in polygon 1 based at (1, 1/2) with vector (1, -1/2)
 
+            sage: from flatsurf import translation_surfaces
             sage: s = translation_surfaces.infinite_staircase()
             sage: gs = s.graphical_surface()
             sage: gs.to_surface((4,4), (1,1), search_all=True, search_limit=20)
             SimilaritySurfaceTangentVector in polygon 8 based at (0, 0) with vector (1, 1)
 
             sage: s = translation_surfaces.square_torus()
             sage: pc = s.minimal_cover(cover_type="planar")
             sage: gs = pc.graphical_surface()
             sage: gs.to_surface((3,2), search_all=True, search_limit=20)
-            Traceback (most recent call last):
-            ...
-            ValueError: To obtain a singularity on an infinite surface, singularity_limit must be set.
+            Vertex 0 of polygon (0, (x, y) |-> (x + 3, y + 2))
             sage: gs.to_surface((3,2), search_all=True, search_limit=20, singularity_limit=4)
-            Surface point with 4 coordinate representations
+            Vertex 0 of polygon (0, (x, y) |-> (x + 3, y + 2))
             sage: p = gs.to_surface((sqrt(3),sqrt(2)), ring=AA, search_all=True, search_limit=20)
-            sage: next(iter(p.coordinates(p.labels()[0]))).parent()
+            doctest:warning
+            ...
+            UserWarning: the ring parameter is deprecated and will be removed in a future version of sage-flatsurf; define the surface over a larger ring instead so that this points' coordinates live in the base ring
+            sage: next(iter(p.coordinates(next(iter(p.labels()))))).parent()
             Vector space of dimension 2 over Algebraic Real Field
             sage: v = gs.to_surface((3/2,3/2),(sqrt(3),sqrt(2)),ring=AA,search_all=True, search_limit=20)
             sage: v.bundle()
-            Tangent bundle of TranslationSurface built from infinitely many polygons defined over Algebraic Real Field
+            Tangent bundle of Minimal Planar Cover of Translation Surface in H_1(0) built from a square defined over Algebraic Real Field
+
         """
+        surface = self.get_surface()
+
         if label is None:
-            if return_all:
-                ret = set()
-            s = self.get_surface()
             if search_all:
                 if search_limit is None:
-                    if s.is_finite():
-                        it = s.label_iterator()
+                    if surface.is_finite_type():
+                        labels = surface.labels()
                     else:
-                        raise ValueError("If search_all=True and the surface is infinite, then a search_limit must be provided.")
+                        raise ValueError(
+                            "If search_all=True and the surface is infinite, then a search_limit must be provided."
+                        )
                 else:
                     from itertools import islice
-                    it = islice(s.label_iterator(), search_limit)
-            else:
-                it = self.visible()
-            for label in it:
-                try:
-                    val = self.to_surface(point, v=v, label=label, ring=ring, singularity_limit=singularity_limit)
-                    if return_all:
-                        ret.add(val)
-                    else:
-                        return val
-                except AssertionError:
-                    # Not in the polygon
-                    pass
-                except ValueError as e:
-                    if e.args[0] == 'need a limit when working with an infinite surface':
-                        raise ValueError("To obtain a singularity on an infinite surface, " + \
-                            "singularity_limit must be set.")
-                    # Otherwise it is not in the polygon.
-            if return_all:
-                return ret
+
+                    labels = islice(surface.labels(), search_limit)
             else:
-                raise ValueError("Point or vector is not in a visible graphical_polygon.")
+                labels = self.visible()
         else:
+            labels = [label]
+
+        points = set()
+
+        for label in labels:
             gp = self.graphical_polygon(label)
             coords = gp.transform_back(point)
-            s = self.get_surface()
+
+            pos = surface.polygon(label).get_point_position(coords)
+            if not pos.is_inside():
+                continue
+
             if v is None:
-                return s.surface_point(label, coords, ring=ring, limit=singularity_limit)
+                points.add(
+                    surface.point(label, coords, ring=ring, limit=singularity_limit)
+                )
             else:
-                return s.tangent_vector(label, coords, (~(gp.transformation().derivative()))*vector(v), ring=ring)
+                direction = (~(gp.transformation().derivative())) * vector(v)
+                if pos.is_vertex():
+                    vertex = pos.get_vertex()
+                    polygon = surface.polygon(label)
+
+                    from flatsurf.geometry.euclidean import ccw
+
+                    if ccw(polygon.edge(vertex), direction) < 0:
+                        continue
+                    if (
+                        ccw(
+                            polygon.edge((vertex - 1) % len(polygon.vertices())),
+                            direction,
+                        )
+                        < 0
+                    ):
+                        continue
+
+                points.add(
+                    surface.tangent_vector(
+                        label,
+                        coords,
+                        direction,
+                        ring=ring,
+                    )
+                )
+            if not return_all:
+                return next(iter(points))
+
+        if return_all:
+            return points
+        else:
+            raise ValueError("Point or vector is not in a visible graphical polygon.")
 
     def opposite_edge(self, p, e):
         r"""
         Given the label ``p`` of a polygon and an edge ``e`` in that polygon
         returns the pair (``pp``, ``ee``) to which this edge is glued.
         """
-        return self._ss.opposite_edge(p,e)
+        return self._ss.opposite_edge(p, e)
 
-    def reset_letters(self,p,e):
+    def reset_letters(self, p, e):
         r"""
         Resets the letter dictionary for storing letters used in
         edge labeling if edge_labels="letter" is used.
         """
         try:
             del self._letters
             del self._next_letter
-        except:
+        except AttributeError:
             pass
 
     def _get_letter_for_edge(self, p, e):
-        if not hasattr(self,"_letters"):
-            self._letters={}
-            self._next_letter=1
+        if not hasattr(self, "_letters"):
+            self._letters = {}
+            self._next_letter = 1
         try:
-            return self._letters[(p,e)]
+            return self._letters[(p, e)]
         except KeyError:
             # convert number to string
             nl = self._next_letter
             self._next_letter = nl + 1
             letter = ""
-            while nl!=0:
+            while nl != 0:
                 val = nl % 52
-                if val==0:
-                    val=52
+                if val == 0:
+                    val = 52
                     letter = "Z" + letter
-                elif val<27:
-                    letter = chr(97+val-1) + letter
+                elif val < 27:
+                    letter = chr(97 + val - 1) + letter
                 else:
-                    letter = chr(65+val-27) + letter
-                nl = (nl-val)/52
-            self._letters[(p,e)] = letter
-            self._letters[self._ss.opposite_edge(p,e)] = letter
+                    letter = chr(65 + val - 27) + letter
+                nl = (nl - val) / 52
+            self._letters[(p, e)] = letter
+            self._letters[self._ss.opposite_edge(p, e)] = letter
             return letter
 
     def edge_labels(self, lab):
         r"""
         Return the list of edge labels to be used for the polygon with label ``lab``.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import similarity_surfaces
             sage: s = similarity_surfaces.example()
-            sage: g = s.graphical_surface(cached=False, adjacencies=[])
+            sage: g = s.graphical_surface(adjacencies=[])
             sage: g.edge_labels(0)
             ['1', '1', '1']
             sage: g.make_all_visible(adjacent=True)
             sage: g.edge_labels(0)
             [None, '1', '1']
 
             sage: g.make_adjacent(0,0)
             sage: g.edge_labels(0)
             [None, '1', '1']
             sage: g.edge_labels(1)
             ['0', None, '0']
 
             sage: s = similarity_surfaces.example()
-            sage: g = s.graphical_surface(cached=False, adjacencies=[], edge_labels='number')
+            sage: g = s.graphical_surface(adjacencies=[], edge_labels='number')
             sage: g.edge_labels(0)
             ['0', '1', '2']
 
-            sage: g = s.graphical_surface(cached=False, adjacencies=[], edge_labels='gluings and number')
+            sage: g = s.graphical_surface(adjacencies=[], edge_labels='gluings and number')
             sage: g.edge_labels(0)
             ['0 -> (1, 1)', '1 -> (1, 2)', '2 -> (1, 0)']
             sage: g.make_all_visible(adjacent=True)
             sage: g.edge_labels(0)
             ['0', '1 -> (1, 2)', '2 -> (1, 0)']
         """
         if not self._edge_labels:
             return None
 
         s = self._ss
         g = self.graphical_polygon(lab)
         p = g.base_polygon()
 
-        if self._edge_labels == 'gluings':
-            ans = []
-            for e in range(p.num_edges()):
+        if self._edge_labels == "gluings":
+            labels = []
+            for e in range(len(p.vertices())):
                 if self.is_adjacent(lab, e):
-                    ans.append(None)
+                    labels.append(None)
                 else:
-                    llab,ee = s.opposite_edge(lab,e)
-                    ans.append(str(llab))
-        elif self._edge_labels == 'number':
-            ans = list(map(str, range(p.num_edges())))
-        elif self._edge_labels == 'gluings and number':
-            ans = []
-            for e in range(p.num_edges()):
+                    llab, ee = s.opposite_edge(lab, e)
+                    labels.append(str(llab))
+        elif self._edge_labels == "number":
+            labels = list(map(str, range(len(p.vertices()))))
+        elif self._edge_labels == "gluings and number":
+            labels = []
+            for e in range(len(p.vertices())):
                 if self.is_adjacent(lab, e):
-                    ans.append(str(e))
+                    labels.append(str(e))
                 else:
-                    ans.append("{} -> {}".format(e, s.opposite_edge(lab,e)))
+                    labels.append("{} -> {}".format(e, s.opposite_edge(lab, e)))
         elif self._edge_labels == "letter":
-            ans = []
-            for e in range(p.num_edges()):
-                llab,ee = s.opposite_edge(lab,e)
+            labels = []
+            for e in range(len(p.vertices())):
+                llab, ee = s.opposite_edge(lab, e)
                 if not self.is_visible(llab) or self.is_adjacent(lab, e):
-                    ans.append(None)
+                    labels.append(None)
                 else:
-                    ans.append(self._get_letter_for_edge(lab,e))
+                    labels.append(self._get_letter_for_edge(lab, e))
         else:
             raise RuntimeError("invalid option for edge_labels")
 
-        return ans
+        return labels
 
     def plot_polygon(self, label, graphical_polygon, upside_down):
         r"""
         Internal method for plotting polygons returning a Graphics object.
 
-        Calls :func:`graphical_polygon.GraphicalPolygon.plot_polygon` passing
-        the attribute `upside_down_polygon_options` if the polygon is upside down
-        and `polygon_options` otherwise.
+        Calls :meth:`.polygon.GraphicalPolygon.plot_polygon` passing
+        the attribute ``upside_down_polygon_options`` if the polygon is upside down
+        and ``polygon_options`` otherwise.
 
         Override this method for fine control of how the polygons are drawn.
 
         INPUT:
 
         - ``label`` -- The label of the polygon being plotted.
 
@@ -875,36 +924,36 @@
         else:
             return graphical_polygon.plot_polygon(**self.polygon_options)
 
     def plot_polygon_label(self, label, graphical_polygon, upside_down):
         r"""
         Internal method for plotting polygon labels returning a Graphics2D.
 
-        Calls :func:`graphical_polygon.GraphicalPolygon.plot_polygon_label` passing
-        the attribute `polygon_label_options`.
+        Calls :meth:`.polygon.GraphicalPolygon.plot_label` passing the
+        attribute ``polygon_label_options``.
 
         Override this method for fine control of how the polygons are drawn.
 
         INPUT:
 
         - ``label`` -- The label of the polygon being plotted.
 
         - ``graphical_polygon`` -- The associated graphical polygon.
 
         - ``upside_down`` -- True if and only if the polygon will be rendered upside down.
         """
-        return graphical_polygon.plot_label(label,**self.polygon_label_options)
+        return graphical_polygon.plot_label(label, **self.polygon_label_options)
 
     def plot_edge(self, label, edge, graphical_polygon, is_adjacent, is_self_glued):
         r"""
         Internal method for plotting a polygon's edge returning a Graphics2D.
 
-        The method calls :func:`graphical_polygon.GraphicalPolygon.plot_edge`.
+        The method calls :meth:`.polygon.GraphicalPolygon.plot_edge`.
         Depending on the geometry of the edge pair, it passes one of the attributes
-        `adjacent_edge_options`, `self_glued_edge_options` or `non_adjacent_edge_options`.
+        ``adjacent_edge_options``, ``self_glued_edge_options`` or ``non_adjacent_edge_options``.
 
         Override this method for fine control of how the edge is drawn.
 
         INPUT:
 
         - ``label`` -- The label of the polygon.
 
@@ -924,117 +973,176 @@
             return graphical_polygon.plot_edge(edge, **self.self_glued_edge_options)
         else:
             return graphical_polygon.plot_edge(edge, **self.non_adjacent_edge_options)
 
     def plot_edge_label(self, p, e, edge_label, graphical_polygon):
         r"""
         Internal method for plotting an edge label.
-        Calls :func:`graphical_polygon.GraphicalPolygon.plot_edge_label` passing
-        the attribute `edge_label_options`.
+        Calls :meth:`.polygon.GraphicalPolygon.plot_edge_label` passing
+        the attribute ``edge_label_options``.
 
         Override this method for fine control of how the edge is drawn.
 
         INPUT:
 
         - ``p`` -- The label of the polygon.
 
         - ``e`` -- Integer representing the edge of the polygon.
 
         - ``edge_label`` -- A string containing the label to be printed on the edge.
 
         - ``graphical_polygon`` -- The associated graphical polygon.
         """
-        return graphical_polygon.plot_edge_label(e, edge_label, **self.edge_label_options)
+        return graphical_polygon.plot_edge_label(
+            e, edge_label, **self.edge_label_options
+        )
 
     def plot_zero_flag(self, label, graphical_polygon):
         r"""
         Internal method for plotting a polygon's zero_flag and returning a Graphics2D.
-        Simply calls :func:`graphical_polygon.GraphicalPolygon.plot_zero_flag` passing
-        the attribute `zero_flag_options`.
+        Simply calls :meth:`.polygon.GraphicalPolygon.plot_zero_flag` passing
+        the attribute` `zero_flag_options``.
 
         Override this method for fine control of how the edge is drawn.
 
         INPUT:
 
         - ``label`` -- The label of the polygon.
 
         - ``graphical_polygon`` -- The associated graphical polygon.
         """
         return graphical_polygon.plot_zero_flag(**self.zero_flag_options)
 
-
-    def plot(self):
+    def plot(self, **kwargs):
         r"""
-        Returns a plot of the GraphicalSurface
+        Return a plot of this surface.
+
+        INPUT:
+
+        - ``kwargs`` -- arguments are normally forwarded to the polygon
+          plotting. However, prefixed arguments, e.g., ``polygon_label_color``,
+          are routed correspondingly. Also, a dictionary suffixed with
+          ``_options`` is merged with the existing options of this surface. See
+          examples below for details.
 
         EXAMPLES::
 
-            sage: from flatsurf import *
+            sage: from flatsurf import similarity_surfaces
             sage: s = similarity_surfaces.example()
             sage: from flatsurf.graphical.surface import GraphicalSurface
             sage: gs = GraphicalSurface(s)
-            sage: gs.make_visible(1)
-            sage: gs.plot()      # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 13 graphics primitives
+            sage: gs.plot()
+            ...Graphics object consisting of 13 graphics primitives
+
+        Keyword arguments that end in ``_options`` are merged into the
+        corresponding attribute before plotting; see :class:`GraphicalSurface`
+        for a list of all supported ``_options``::
+
+            sage: gs.plot(polygon_label_options={"color": "red"})
+            ...Graphics object consisting of 13 graphics primitives
+
+        Keyword arguments that are prefixed with such an aspect of plotting,
+        are also merged into the corresponding attribute before plotting; see
+        :class:`GraphicalSurface` for a list of all supported prefixes, i.e.,
+        ``_options``::
+
+            sage: gs.plot(polygon_label_color="red")
+            ...Graphics object consisting of 13 graphics primitives
 
+        All other arguments are passed to the polygon plotting itself::
+
+            sage: gs.plot(fill=None)
+            ...Graphics object consisting of 13 graphics primitives
+
+        TESTS:
 
         Check that label options are handled correctly::
 
+            sage: from flatsurf import translation_surfaces
             sage: S = translation_surfaces.square_torus()
-            sage: S.plot(polygon_labels=True, edge_labels=True)     # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 10 graphics primitives
-            sage: S.plot(polygon_labels=False, edge_labels=True)    # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 9 graphics primitives
-            sage: S.plot(polygon_labels=True, edge_labels=False)    # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 6 graphics primitives
-            sage: S.plot(polygon_labels=False, edge_labels=False)   # not tested (problem with matplotlib font caches on Travis)
-            Graphics object consisting of 5 graphics primitives
-        """
+            sage: S.plot(polygon_labels=True, edge_labels=True)
+            ...Graphics object consisting of 10 graphics primitives
+            sage: S.plot(polygon_labels=False, edge_labels=True)
+            ...Graphics object consisting of 9 graphics primitives
+            sage: S.plot(polygon_labels=True, edge_labels=False)
+            ...Graphics object consisting of 6 graphics primitives
+            sage: S.plot(polygon_labels=False, edge_labels=False)
+            ...Graphics object consisting of 5 graphics primitives
+        """
+        if kwargs:
+            surface = self.copy()
+
+            options = [
+                option
+                for option in surface.__dict__
+                if option.endswith("_options") and option != "process_options"
+            ]
+            # Sort recognized options so we do not pass polygon_label_color to
+            # polygon_options as label_color.
+            options.sort(key=lambda option: -len(option))
+
+            for key, value in kwargs.items():
+                if key in options:
+                    setattr(surface, key, {**getattr(surface, key), **value})
+                    continue
+
+                for option in options:
+                    prefix = option[: -len("options")]
+                    if key.startswith(prefix) and key != prefix:
+                        getattr(surface, option)[key[len(prefix) :]] = value
+                        break
+                else:
+                    surface.polygon_options[key] = value
+
+            return surface.plot()
+
         from sage.plot.graphics import Graphics
+
         p = Graphics()
 
         # Make sure we don't plot adjacent edges more than once.
         plotted_adjacent_edges = set()
 
         for label in self._visible:
             polygon = self.graphical_polygon(label)
-            upside_down = polygon.transformation().sign()==-1
+            upside_down = polygon.transformation().sign() == -1
 
             # Plot the polygons
             if upside_down and self.will_plot_upside_down_polygons:
-                    p += self.plot_polygon(label, polygon, upside_down)
+                p += self.plot_polygon(label, polygon, upside_down)
             elif self.will_plot_polygons:
                 p += self.plot_polygon(label, polygon, upside_down)
 
             if self.will_plot_zero_flags:
-                p += self.plot_zero_flag(label,polygon)
+                p += self.plot_zero_flag(label, polygon)
 
             # Add the polygon label
             if self.will_plot_polygon_labels:
                 p += self.plot_polygon_label(label, polygon, upside_down)
 
             # Plot the edges
             if self.will_plot_edges:
-                for i in range(self._ss.polygon(label).num_edges()):
-                    if self.is_adjacent(label,i):
-                        if self.will_plot_adjacent_edges and (label,i) not in plotted_adjacent_edges:
-                            plotted_adjacent_edges.add(self._ss.opposite_edge(label,i))
+                for i in range(len(self._ss.polygon(label).vertices())):
+                    if self.is_adjacent(label, i):
+                        if (
+                            self.will_plot_adjacent_edges
+                            and (label, i) not in plotted_adjacent_edges
+                        ):
+                            plotted_adjacent_edges.add(self._ss.opposite_edge(label, i))
                             p += self.plot_edge(label, i, polygon, True, False)
-                    elif (label,i) == self._ss.opposite_edge(label,i):
+                    elif (label, i) == self._ss.opposite_edge(label, i):
                         # Self-glued edge
                         if self.will_plot_self_glued_edges:
                             p += self.plot_edge(label, i, polygon, False, True)
                     else:
                         if self.will_plot_non_adjacent_edges:
                             p += self.plot_edge(label, i, polygon, False, False)
 
             # Plot the edge labels.
             if self.will_plot_edge_labels:
                 # get the edge labels
                 edge_labels = self.edge_labels(label)
                 if edge_labels is not None:
-                    for i in range(self._ss.polygon(label).num_edges()):
+                    for i in range(len(self._ss.polygon(label).vertices())):
                         if edge_labels[i] is not None:
                             p += self.plot_edge_label(label, i, edge_labels[i], polygon)
         return p
-
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sage_flatsurf-0.4.7/flatsurf/graphical/surface_point.py` & `sage_flatsurf-0.5.0/flatsurf/graphical/surface_point.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,44 @@
-#*****************************************************************************
-#       Copyright (C) 2013-2019 Vincent Delecroix <20100.delecroix@gmail.com>
-#                     2013-2019 W. Patrick Hooper <wphooper@gmail.com>
+# ****************************************************************************
+#  This file is part of sage-flatsurf.
 #
-#  Distributed under the terms of the GNU General Public License (GPL)
-#  as published by the Free Software Foundation; either version 2 of
-#  the License, or (at your option) any later version.
-#                  https://www.gnu.org/licenses/
-#*****************************************************************************
-
-from __future__ import absolute_import, print_function, division
-from six.moves import range, map, filter, zip
-
-from flatsurf.graphical.surface import GraphicalSurface
-# The real vector space:
-from flatsurf.geometry.surface_objects import SurfacePoint
+#       Copyright (C) 2013-2019 Vincent Delecroix
+#                     2013-2019 W. Patrick Hooper
+#                     2022-2023 Julian Rüth
+#
+#  sage-flatsurf is free software: you can redistribute it and/or modify
+#  it under the terms of the GNU General Public License as published by
+#  the Free Software Foundation, either version 2 of the License, or
+#  (at your option) any later version.
+#
+#  sage-flatsurf is distributed in the hope that it will be useful,
+#  but WITHOUT ANY WARRANTY; without even the implied warranty of
+#  MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+#  GNU General Public License for more details.
+#
+#  You should have received a copy of the GNU General Public License
+#  along with sage-flatsurf. If not, see <https://www.gnu.org/licenses/>.
+# ****************************************************************************
+
 from sage.plot.point import point2d
 
+
 class GraphicalSurfacePoint:
     def __init__(self, surface_point, graphical_surface=None):
         r"""
         Create a graphical segment from SurfacePoint.
 
         If a graphical_surface is provided the point is created on the graphical surface.
         Otherwise, we create it on the default graphical surface.
         """
         if graphical_surface is None:
             self._gs = surface_point.surface().graphical_surface()
         else:
-            assert surface_point.surface() == graphical_surface.get_surface()
+            if surface_point.surface() != graphical_surface.get_surface():
+                raise ValueError
             self._gs = graphical_surface
         self._sp = surface_point
 
     def surface_point(self):
         r"""
         Return the underlying SurfacePoint.
         """
@@ -39,22 +46,23 @@
 
     def points(self):
         r"""Return the list of points as RDF vectors."""
         point_list = []
         for label in self._sp.labels():
             if self._gs.is_visible(label):
                 for coord in self._sp.coordinates(label):
-                    point_list.append( self._gs.graphical_polygon(label).transform(coord) )
+                    point_list.append(
+                        self._gs.graphical_polygon(label).transform(coord)
+                    )
         return point_list
 
     def plot(self, **options):
         r"""
         Plot the point (which might involve drawing several dots).
 
         The options are passed to point2d.
 
         If no "zorder" option is provided then we set "zorder" to 50.
         """
         if "zorder" not in options:
-            options["zorder"]=50
+            options["zorder"] = 50
         return point2d(points=self.points(), **options)
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

