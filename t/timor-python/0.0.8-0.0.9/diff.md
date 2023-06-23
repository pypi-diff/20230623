# Comparing `tmp/timor-python-0.0.8.tar.gz` & `tmp/timor-python-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timor-python-0.0.8.tar", last modified: Mon Mar 20 08:57:32 2023, max compression
+gzip compressed data, was "timor-python-0.0.9.tar", last modified: Fri Jun 23 14:49:30 2023, max compression
```

## Comparing `timor-python-0.0.8.tar` & `timor-python-0.0.9.tar`

### file list

```diff
@@ -1,125 +1,126 @@
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.852102 timor-python-0.0.8/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1064 2022-10-10 14:00:16.000000 timor-python-0.0.8/LICENSE
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       30 2022-10-10 14:00:16.000000 timor-python-0.0.8/MANIFEST.in
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5416 2023-03-20 08:57:32.852102 timor-python-0.0.8/PKG-INFO
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4593 2023-03-14 10:00:16.000000 timor-python-0.0.8/README.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1537 2023-03-14 16:00:37.000000 timor-python-0.0.8/pyproject.toml
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       38 2023-03-20 08:57:32.852102 timor-python-0.0.8/setup.cfg
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.836102 timor-python-0.0.8/src/
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.836102 timor-python-0.0.8/src/cache/
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.836102 timor-python-0.0.8/src/cache/robots/
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.836102 timor-python-0.0.8/src/cache/robots/modrob-gen2/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3559 2023-03-14 10:03:22.000000 timor-python-0.0.8/src/cache/robots/modrob-gen2/make_zimmer_gripper.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.836102 timor-python-0.0.8/src/timor/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15607 2023-03-20 07:37:03.000000 timor-python-0.0.8/src/timor/Bodies.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    28161 2023-03-20 07:37:03.000000 timor-python-0.0.8/src/timor/Geometry.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12083 2023-03-20 07:37:03.000000 timor-python-0.0.8/src/timor/Joints.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    76661 2023-03-20 07:37:03.000000 timor-python-0.0.8/src/timor/Module.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    66717 2023-03-16 08:02:04.000000 timor-python-0.0.8/src/timor/Robot.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    13500 2023-03-08 15:05:02.000000 timor-python-0.0.8/src/timor/Volume.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      396 2023-03-20 08:57:24.000000 timor-python-0.0.8/src/timor/__init__.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.836102 timor-python-0.0.8/src/timor/configuration_search/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    19396 2023-03-14 16:00:37.000000 timor-python-0.0.8/src/timor/configuration_search/AssemblyFilter.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1692 2023-03-08 15:05:02.000000 timor-python-0.0.8/src/timor/configuration_search/AssemblyIterator.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    24652 2023-03-20 08:57:24.000000 timor-python-0.0.8/src/timor/configuration_search/LiuIterator.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2023-03-08 15:05:02.000000 timor-python-0.0.8/src/timor/configuration_search/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    47109 2023-03-14 10:00:16.000000 timor-python-0.0.8/src/timor/parameterized.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.836102 timor-python-0.0.8/src/timor/task/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    21847 2023-03-08 15:05:02.000000 timor-python-0.0.8/src/timor/task/Constraints.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10560 2023-03-14 10:00:16.000000 timor-python-0.0.8/src/timor/task/CostFunctions.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    21620 2023-03-14 16:00:37.000000 timor-python-0.0.8/src/timor/task/Goals.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7464 2023-03-08 15:05:02.000000 timor-python-0.0.8/src/timor/task/Obstacle.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    18508 2023-03-20 07:37:03.000000 timor-python-0.0.8/src/timor/task/Solution.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12415 2023-03-20 07:37:03.000000 timor-python-0.0.8/src/timor/task/Task.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    37747 2023-03-08 15:05:02.000000 timor-python-0.0.8/src/timor/task/Tolerance.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2022-10-11 14:03:10.000000 timor-python-0.0.8/src/timor/task/__init__.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.840102 timor-python-0.0.8/src/timor/utilities/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       65 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor/utilities/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      581 2023-03-08 15:05:02.000000 timor-python-0.0.8/src/timor/utilities/configurations.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3249 2023-03-08 15:05:02.000000 timor-python-0.0.8/src/timor/utilities/download_data.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    16543 2023-03-20 07:37:03.000000 timor-python-0.0.8/src/timor/utilities/dtypes.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2832 2023-03-08 15:05:02.000000 timor-python-0.0.8/src/timor/utilities/errors.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3671 2023-03-20 07:37:03.000000 timor-python-0.0.8/src/timor/utilities/file_locations.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1879 2023-03-14 16:00:37.000000 timor-python-0.0.8/src/timor/utilities/json_serialization_formatting.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2163 2023-03-20 07:37:03.000000 timor-python-0.0.8/src/timor/utilities/jsonable.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3340 2022-10-17 13:54:15.000000 timor-python-0.0.8/src/timor/utilities/logging.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4154 2023-03-16 08:02:04.000000 timor-python-0.0.8/src/timor/utilities/module_classification.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2944 2023-01-23 11:40:52.000000 timor-python-0.0.8/src/timor/utilities/prebuilt_robots.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1566 2023-03-14 10:00:16.000000 timor-python-0.0.8/src/timor/utilities/schema.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10485 2023-03-08 15:05:02.000000 timor-python-0.0.8/src/timor/utilities/spatial.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4351 2023-03-20 07:37:03.000000 timor-python-0.0.8/src/timor/utilities/tolerated_pose.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    20343 2023-03-14 10:00:16.000000 timor-python-0.0.8/src/timor/utilities/trajectory.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    16221 2023-03-20 07:37:03.000000 timor-python-0.0.8/src/timor/utilities/transformation.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12829 2023-03-14 16:00:37.000000 timor-python-0.0.8/src/timor/utilities/visualization.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2960 2023-03-08 15:05:02.000000 timor-python-0.0.8/src/timor/utilities/write_urdf.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.840102 timor-python-0.0.8/src/timor_python.egg-info/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5416 2023-03-20 08:57:32.000000 timor-python-0.0.8/src/timor_python.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3917 2023-03-20 08:57:32.000000 timor-python-0.0.8/src/timor_python.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        1 2023-03-20 08:57:32.000000 timor-python-0.0.8/src/timor_python.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      406 2023-03-20 08:57:32.000000 timor-python-0.0.8/src/timor_python.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       41 2023-03-20 08:57:32.000000 timor-python-0.0.8/src/timor_python.egg-info/top_level.txt
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.836102 timor-python-0.0.8/src/timor_sample_robots/
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.840102 timor-python-0.0.8/src/timor_sample_robots/IMPROV/
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.840102 timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)   143084 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/L1.stl
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)  1130784 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/L10.stl
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)   235684 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/L2.stl
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)   862034 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/L3.stl
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)   803284 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/L8.stl
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)  1431184 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/L9.stl
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.844102 timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9860 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L1.stl.wrl
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    13074 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L2.stl.wrl
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4241 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L3.stl.wrl
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5209 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L8.stl.wrl
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7629 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L9.stl.wrl
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    50536 2023-03-14 10:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/IMPROV/modules.json
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.844102 timor-python-0.0.8/src/timor_sample_robots/geometric_primitive_modules/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    25164 2023-03-14 10:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/geometric_primitive_modules/modules.json
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.844102 timor-python-0.0.8/src/timor_sample_robots/panda/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10173 2023-01-23 11:40:52.000000 timor-python-0.0.8/src/timor_sample_robots/panda/LICENSE
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.836102 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.844102 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10084 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/hand.stl
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10084 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link0.stl
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15084 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link1.stl
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15084 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link2.stl
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15084 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link3.stl
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15084 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link4.stl
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15084 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link5.stl
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10084 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link6.stl
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10084 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link7.stl
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.848102 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    51239 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/finger.dae
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   549239 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/hand.dae
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)  1591592 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link0.dae
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   978473 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link1.dae
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   998544 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link2.dae
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)  1099883 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link3.dae
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)  1145723 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link4.dae
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)  1438343 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link5.dae
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)  1728753 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link6.dae
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   936416 2022-10-10 14:00:16.000000 timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link7.dae
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.852102 timor-python-0.0.8/src/timor_sample_robots/panda/urdf/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    24707 2023-01-23 11:40:52.000000 timor-python-0.0.8/src/timor_sample_robots/panda/urdf/panda.urdf
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-03-20 08:57:32.852102 timor-python-0.0.8/tests/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6956 2023-03-14 10:00:16.000000 timor-python-0.0.8/tests/test_assembly.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5248 2023-03-08 15:05:03.000000 timor-python-0.0.8/tests/test_assembly_filters.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4221 2023-03-14 16:00:37.000000 timor-python-0.0.8/tests/test_assembly_iterator.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11135 2023-03-08 15:05:03.000000 timor-python-0.0.8/tests/test_bodies_geometries.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5408 2023-03-14 10:00:16.000000 timor-python-0.0.8/tests/test_collisions.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3172 2023-03-14 10:00:16.000000 timor-python-0.0.8/tests/test_custom_types.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2008 2023-03-14 16:00:37.000000 timor-python-0.0.8/tests/test_imports.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1362 2022-12-01 17:01:29.000000 timor-python-0.0.8/tests/test_logging.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    16656 2023-03-08 15:05:03.000000 timor-python-0.0.8/tests/test_module.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5859 2023-03-14 10:00:16.000000 timor-python-0.0.8/tests/test_modulesDB.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2657 2023-03-08 15:05:03.000000 timor-python-0.0.8/tests/test_obstacle.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    14271 2023-03-16 08:02:04.000000 timor-python-0.0.8/tests/test_robot_setup.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2405 2023-01-23 11:40:52.000000 timor-python-0.0.8/tests/test_schemas.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    26511 2023-03-14 10:00:16.000000 timor-python-0.0.8/tests/test_serializing_deserializing.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6226 2023-01-23 11:40:52.000000 timor-python-0.0.8/tests/test_spatial_projections.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    31323 2023-03-14 16:00:37.000000 timor-python-0.0.8/tests/test_task_solutions.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8825 2023-03-08 15:05:03.000000 timor-python-0.0.8/tests/test_tolerances.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8474 2023-03-14 10:00:16.000000 timor-python-0.0.8/tests/test_trajectory.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7679 2023-03-08 15:05:03.000000 timor-python-0.0.8/tests/test_transformations.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6808 2023-03-08 15:05:03.000000 timor-python-0.0.8/tests/test_volume.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.528770 timor-python-0.0.9/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1064 2022-09-20 15:06:13.000000 timor-python-0.0.9/LICENSE
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       30 2022-09-20 15:06:13.000000 timor-python-0.0.9/MANIFEST.in
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5830 2023-06-23 14:49:30.528770 timor-python-0.0.9/PKG-INFO
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5007 2023-06-23 14:49:13.000000 timor-python-0.0.9/README.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1537 2023-06-23 14:31:14.000000 timor-python-0.0.9/pyproject.toml
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       38 2023-06-23 14:49:30.528770 timor-python-0.0.9/setup.cfg
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.512770 timor-python-0.0.9/src/
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.512770 timor-python-0.0.9/src/cache/
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.512770 timor-python-0.0.9/src/cache/robots/
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.512770 timor-python-0.0.9/src/cache/robots/modrob-gen2/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3559 2023-04-21 08:06:36.000000 timor-python-0.0.9/src/cache/robots/modrob-gen2/make_zimmer_gripper.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.516770 timor-python-0.0.9/src/timor/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    16499 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/Bodies.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    30394 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/Geometry.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12754 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/Joints.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    77645 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/Module.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    68298 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/Robot.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    13500 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor/Volume.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      396 2023-06-23 14:46:13.000000 timor-python-0.0.9/src/timor/__init__.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.516770 timor-python-0.0.9/src/timor/configuration_search/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    21946 2023-06-23 14:31:14.000000 timor-python-0.0.9/src/timor/configuration_search/AssemblyFilter.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1692 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor/configuration_search/AssemblyIterator.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    24652 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor/configuration_search/LiuIterator.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor/configuration_search/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    47762 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/parameterized.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.516770 timor-python-0.0.9/src/timor/task/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    23868 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/task/Constraints.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10560 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor/task/CostFunctions.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    23634 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/task/Goals.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7522 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/task/Obstacle.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    23538 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/task/Solution.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15487 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/task/Task.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    37747 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor/task/Tolerance.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2022-09-28 17:07:40.000000 timor-python-0.0.9/src/timor/task/__init__.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.516770 timor-python-0.0.9/src/timor/utilities/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       65 2022-09-28 17:07:40.000000 timor-python-0.0.9/src/timor/utilities/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3413 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/utilities/asset_handling.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1805 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/utilities/configurations.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3249 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor/utilities/download_data.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    17905 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/utilities/dtypes.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2832 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor/utilities/errors.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4106 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/utilities/file_locations.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1715 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor/utilities/json_serialization_formatting.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4588 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/utilities/jsonable.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3340 2022-10-19 15:22:02.000000 timor-python-0.0.9/src/timor/utilities/logging.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4154 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor/utilities/module_classification.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2944 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor/utilities/prebuilt_robots.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1566 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor/utilities/schema.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10485 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor/utilities/spatial.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4368 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/utilities/tolerated_pose.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    20583 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor/utilities/trajectory.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    16303 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/utilities/transformation.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15654 2023-06-23 14:46:15.000000 timor-python-0.0.9/src/timor/utilities/visualization.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2960 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor/utilities/write_urdf.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.516770 timor-python-0.0.9/src/timor_python.egg-info/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5830 2023-06-23 14:49:30.000000 timor-python-0.0.9/src/timor_python.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3955 2023-06-23 14:49:30.000000 timor-python-0.0.9/src/timor_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        1 2023-06-23 14:49:30.000000 timor-python-0.0.9/src/timor_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      406 2023-06-23 14:49:30.000000 timor-python-0.0.9/src/timor_python.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       41 2023-06-23 14:49:30.000000 timor-python-0.0.9/src/timor_python.egg-info/top_level.txt
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.512770 timor-python-0.0.9/src/timor_sample_robots/
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.516770 timor-python-0.0.9/src/timor_sample_robots/IMPROV/
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.520770 timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)   143084 2022-09-20 15:06:13.000000 timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/L1.stl
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)  1130784 2022-09-20 15:06:13.000000 timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/L10.stl
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)   235684 2022-09-20 15:06:13.000000 timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/L2.stl
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)   862034 2022-09-20 15:06:13.000000 timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/L3.stl
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)   803284 2022-09-20 15:06:13.000000 timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/L8.stl
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)  1431184 2022-09-20 15:06:13.000000 timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/L9.stl
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.520770 timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9860 2022-12-19 12:29:58.000000 timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L1.stl.wrl
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    13074 2022-12-19 12:29:58.000000 timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L2.stl.wrl
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4241 2022-12-19 12:29:58.000000 timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L3.stl.wrl
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5209 2022-12-19 12:29:58.000000 timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L8.stl.wrl
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7629 2022-12-19 12:29:58.000000 timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L9.stl.wrl
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    50536 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor_sample_robots/IMPROV/modules.json
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.520770 timor-python-0.0.9/src/timor_sample_robots/geometric_primitive_modules/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    25164 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor_sample_robots/geometric_primitive_modules/modules.json
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.520770 timor-python-0.0.9/src/timor_sample_robots/panda/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10173 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor_sample_robots/panda/LICENSE
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.512770 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.520770 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10084 2022-09-26 15:17:33.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/hand.stl
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10084 2022-09-26 15:17:33.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link0.stl
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15084 2022-09-26 15:17:33.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link1.stl
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15084 2022-09-26 15:17:33.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link2.stl
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15084 2022-09-26 15:17:33.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link3.stl
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15084 2022-09-26 15:17:33.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link4.stl
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15084 2022-09-26 15:17:33.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link5.stl
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10084 2022-09-26 15:17:33.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link6.stl
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10084 2022-09-26 15:17:33.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link7.stl
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.528770 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    51239 2022-12-19 12:29:58.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/finger.dae
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   549239 2022-12-19 12:29:58.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/hand.dae
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)  1591592 2022-12-19 12:29:58.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link0.dae
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   978473 2022-12-19 12:29:58.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link1.dae
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   998544 2022-12-19 12:29:58.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link2.dae
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)  1099883 2022-12-19 12:29:58.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link3.dae
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)  1145723 2022-12-19 12:29:58.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link4.dae
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)  1438343 2022-12-19 12:29:58.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link5.dae
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)  1728753 2022-12-19 12:29:58.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link6.dae
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   936416 2022-12-19 12:29:58.000000 timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link7.dae
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.528770 timor-python-0.0.9/src/timor_sample_robots/panda/urdf/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    24707 2023-05-17 11:59:34.000000 timor-python-0.0.9/src/timor_sample_robots/panda/urdf/panda.urdf
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-23 14:49:30.528770 timor-python-0.0.9/tests/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7423 2023-06-23 14:46:15.000000 timor-python-0.0.9/tests/test_assembly.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8694 2023-05-17 11:59:36.000000 timor-python-0.0.9/tests/test_assembly_filters.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4580 2023-06-23 14:46:15.000000 timor-python-0.0.9/tests/test_assembly_iterator.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11411 2023-06-23 14:46:15.000000 timor-python-0.0.9/tests/test_bodies_geometries.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5408 2023-05-17 11:59:36.000000 timor-python-0.0.9/tests/test_collisions.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3290 2023-06-23 14:46:15.000000 timor-python-0.0.9/tests/test_custom_types.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2008 2023-05-17 11:59:36.000000 timor-python-0.0.9/tests/test_imports.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1362 2023-05-17 11:59:36.000000 timor-python-0.0.9/tests/test_logging.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    17489 2023-06-23 14:46:15.000000 timor-python-0.0.9/tests/test_module.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6403 2023-06-23 14:46:15.000000 timor-python-0.0.9/tests/test_modulesDB.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2579 2023-06-23 14:46:15.000000 timor-python-0.0.9/tests/test_obstacle.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    15653 2023-06-23 14:46:15.000000 timor-python-0.0.9/tests/test_robot_setup.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2402 2023-06-23 14:46:15.000000 timor-python-0.0.9/tests/test_schemas.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    30796 2023-06-23 14:46:15.000000 timor-python-0.0.9/tests/test_serializing_deserializing.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6226 2023-05-17 11:59:36.000000 timor-python-0.0.9/tests/test_spatial_projections.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    31753 2023-05-17 11:59:36.000000 timor-python-0.0.9/tests/test_task_solutions.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8825 2023-05-17 11:59:36.000000 timor-python-0.0.9/tests/test_tolerances.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8474 2023-05-17 11:59:36.000000 timor-python-0.0.9/tests/test_trajectory.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7679 2023-05-17 11:59:36.000000 timor-python-0.0.9/tests/test_transformations.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6808 2023-05-17 11:59:36.000000 timor-python-0.0.9/tests/test_volume.py
```

### Comparing `timor-python-0.0.8/LICENSE` & `timor-python-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/PKG-INFO` & `timor-python-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: timor-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: Toolbox for Industrial Modular Robots
 Author-email: Jonathan Kuelz <jonathan.kuelz@tum.de>
 License: MIT
 Project-URL: Source Code, https://gitlab.lrz.de/tum-cps/timor-python
 Project-URL: Documentation, https://timor-python.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://gitlab.lrz.de/tum-cps/timor-python/-/issues
 Keywords: Modular Reconfigurable Robots,Robot Design,Model Generation,Simulation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: optimization
 Provides-Extra: full
 License-File: LICENSE
 
 .. image:: https://gitlab.lrz.de/tum-cps/timor-python/-/raw/main/img/timor_banner.png
@@ -53,15 +53,15 @@
     :alt: Animation of a robot assembly moving between two goals
     :align: center
     :target: https://gitlab.lrz.de/tum-cps/timor-python/-/raw/main/img/animations/demo_animation.gif
 
 
 Installation
 ------------
-Timor-python is available on PyPI. It requires **at least Python 3.7**. For installation, use::
+Timor-python is available on PyPI. It requires **at least Python 3.8**. For installation, use::
 
    pip install timor-python
 
 Some requirements are not included by default - in order to install them, use::
 
   pip install timor-python[option]
 
@@ -73,14 +73,16 @@
 If you want to work with the bleeding-edge version, you can download the source code from the project repository and install it locally.
 Nagivate to the timor-python repository you cloned and enter::
 
    pip install -e .
 
 to install it in editeable mode. This requires :code:`setuptools>=61` and :code:`pip>=21.3` (previous versions of setuptools require a :code:`setup.py`-file). To install optional dependencies, proceed in the same manner as for PyPI installs.
 
+To run unittest locally, you need to `setup git lfs <https://git-lfs.com/>`_ in order to download assets.
+
 If you want to use pre-commit hooks provided with Timor, for installation please use::
 
    pip install pre-commit
 
 then::
 
    pre-commit install
@@ -99,14 +101,22 @@
 
   jupyter lab
 
 You can set custom configurations such as file paths of robot libraries or logging behavior by editing the config file. You can import the file location of the config file as :code:`from timor.utilities.configurations import CONFIG_FILE`.
 
 For further information, please visit the `documentation <https://timor-python.readthedocs.io>`_.
 
+Updating
+--------
+
+Some timor updates might require to re-acquire the task, schema, or robot module data-bases. Try to reset the caches by running ``timor.utilities.file_locations.clean_caches()`` and re-import the timor module.
+
+Typical errors indicating this action:
+ * ValueError: modules.json invalid.
+
 Support
 -------
 Do you have a question or an issue using Timor? You can either `submit an issue <https://gitlab.lrz.de/tum-cps/timor-python/-/issues>`_ or write an email to the `repository maintainer <mailto:jonathan.kuelz@tum.de>`_.
 
 Contributing
 ------------
 We welcome every contribution to Timor. For more details, please refer to our `contribution guidelines <https://gitlab.lrz.de/tum-cps/timor-python/-/blob/main/CONTRIBUTING.md>`_.
```

### Comparing `timor-python-0.0.8/README.rst` & `timor-python-0.0.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     :alt: Animation of a robot assembly moving between two goals
     :align: center
     :target: https://gitlab.lrz.de/tum-cps/timor-python/-/raw/main/img/animations/demo_animation.gif
 
 
 Installation
 ------------
-Timor-python is available on PyPI. It requires **at least Python 3.7**. For installation, use::
+Timor-python is available on PyPI. It requires **at least Python 3.8**. For installation, use::
 
    pip install timor-python
 
 Some requirements are not included by default - in order to install them, use::
 
   pip install timor-python[option]
 
@@ -52,14 +52,16 @@
 If you want to work with the bleeding-edge version, you can download the source code from the project repository and install it locally.
 Nagivate to the timor-python repository you cloned and enter::
 
    pip install -e .
 
 to install it in editeable mode. This requires :code:`setuptools>=61` and :code:`pip>=21.3` (previous versions of setuptools require a :code:`setup.py`-file). To install optional dependencies, proceed in the same manner as for PyPI installs.
 
+To run unittest locally, you need to `setup git lfs <https://git-lfs.com/>`_ in order to download assets.
+
 If you want to use pre-commit hooks provided with Timor, for installation please use::
 
    pip install pre-commit
 
 then::
 
    pre-commit install
@@ -78,14 +80,22 @@
 
   jupyter lab
 
 You can set custom configurations such as file paths of robot libraries or logging behavior by editing the config file. You can import the file location of the config file as :code:`from timor.utilities.configurations import CONFIG_FILE`.
 
 For further information, please visit the `documentation <https://timor-python.readthedocs.io>`_.
 
+Updating
+--------
+
+Some timor updates might require to re-acquire the task, schema, or robot module data-bases. Try to reset the caches by running ``timor.utilities.file_locations.clean_caches()`` and re-import the timor module.
+
+Typical errors indicating this action:
+ * ValueError: modules.json invalid.
+
 Support
 -------
 Do you have a question or an issue using Timor? You can either `submit an issue <https://gitlab.lrz.de/tum-cps/timor-python/-/issues>`_ or write an email to the `repository maintainer <mailto:jonathan.kuelz@tum.de>`_.
 
 Contributing
 ------------
 We welcome every contribution to Timor. For more details, please refer to our `contribution guidelines <https://gitlab.lrz.de/tum-cps/timor-python/-/blob/main/CONTRIBUTING.md>`_.
```

### Comparing `timor-python-0.0.8/pyproject.toml` & `timor-python-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     "meshcat",
     "networkx >= 2.6.3",
     "numpy >= 1.21.0",
     "roboticstoolbox-python >= 0.11.0",
     "scipy >= 1.6",
     "requests >= 2.28.1"
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 dynamic = ["version", "readme"]
 
 [project.optional-dependencies]
 dev = ["flake8>=5.0", "coverage>=6.3", "pre-commit", "pip-tools", "pytest>=6.0", "setuptools>=61.0.0"]
 optimization = ["pygad>=2.18.0", "optuna>=3.1", "plotly", "scikit-learn"]
 full = ["flake8>=5.0", "coverage>=6.3", "pre-commit", "pip-tools", "pytest>=6.0", "setuptools>=61.0.0", "jupyterlab", "trimesh >= 3.18", "tqdm"]
```

### Comparing `timor-python-0.0.8/src/cache/robots/modrob-gen2/make_zimmer_gripper.py` & `timor-python-0.0.9/src/cache/robots/modrob-gen2/make_zimmer_gripper.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor/Bodies.py` & `timor-python-0.0.9/src/timor/Bodies.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import numpy as np
 import pinocchio as pin
 
 from timor.Geometry import ComposedGeometry, EmptyGeometry, Geometry
 from timor.Robot import PinBody
 from timor.utilities import logging
-from timor.utilities.dtypes import SingleSet, hppfcl_collision2pin_geometry
+from timor.utilities.dtypes import SingleSet, SingleSetWithID, hppfcl_collision2pin_geometry
 import timor.utilities.errors as err
 from timor.utilities.json_serialization_formatting import possibly_nest_as_list
 from timor.utilities.jsonable import JSONable_mixin
 from timor.utilities.transformation import Transformation, TransformationLike
 
 
 class Gender(Enum):
@@ -87,18 +87,20 @@
         :param size: Can be an integer, float or array describing the size of the connector.
         """
         self._id: str = str(connector_id)
         self.body2connector: Transformation = Transformation(body2connector)
         self.parent: 'BodyBase' = parent
         self.gender: Gender = gender if isinstance(gender, Gender) else Gender[gender]  # Enforce typing
         self._type: str = connector_type
+        if isinstance(size, Iterable) and not isinstance(size, np.ndarray):
+            size = np.array(size)
         self.size: Union[int, float, np.ndarray] = size
 
     @classmethod
-    def from_json_data(cls, d: Dict) -> Connector:
+    def from_json_data(cls, d: Dict, *args, **kwargs) -> Connector:
         """
         Maps the serialized connector description to an instance of this class.
 
         :param d: A dictionary with relevant meta-information
         :return: An instantiated connector
         """
         return cls(
@@ -161,26 +163,33 @@
         """Wrapped as _type attribute to not be confused with python-native type(). Also, is kind of static anyway"""
         return self._type
 
     def __copy__(self):
         """Custom copy behavior: Remove the reference to the parent body."""
         return self.__class__(self._id, self.body2connector, None, self.gender, self._type, self.size)
 
+    def __eq__(self, other):
+        """Equality check: Same ID, gender, type, size, and pose"""
+        if not isinstance(other, Connector):
+            return NotImplemented
+        return self.id == other.id and self.gender is other.gender and self.type == other.type \
+            and np.all(self.size == other.size) and self.body2connector == other.body2connector
+
+    def __hash__(self):
+        """Hashing: We assume IDs are unique, so it poses a valid hash."""
+        return hash(self.id)
+
     def __str__(self) -> str:
         """The string representation of the connector"""
         return f"Connector: {self.id}"
 
 
-class ConnectorSet(SingleSet):
+class ConnectorSet(SingleSetWithID):
     """A set that raises an error if a duplicate connector is added."""
 
-    def __contains__(self, item: Connector):
-        """Custom duplicate check (unique ID)"""
-        return item.id in (con.id for con in self)
-
 
 class BodyBase(abc.ABC, JSONable_mixin):
     """
     A body describes a rigid robot element with kinematic, dynamic, geometric, and connection properties.
 
     A body is defined by a geometry and inertia-parameters. Its placement is defined implicitly by the connectors
       attached to it.
@@ -233,29 +242,28 @@
             name='.'.join(self.id),
             collision_geometries=collision,
             visual_geometries=visual
         )
 
     def possible_connections_with(self, other: 'BodyBase') -> SingleSet:
         """
-        Returns a list of connectors that can connect this with other body.
+        Returns a set of connectors that can connect this with other body.
 
         This method does not check whether the connector IDs of the other body overlap with the connector IDs
         of this body - this has to be achieved by e.g. putting both bodies in a module or in the same ModulesDB.
 
         :param other: Another body
         :return: A list of matching connector pairs like (this_body_connector, other_body_connector)
         """
         if other.id == self.id:
             raise err.UniqueValueError("Two connectors with identical ID cannot be connected")
         matches = SingleSet()
         for own, foreign in itertools.product(self.connectors, other.connectors):
             if own.connects(foreign):
                 matches.add((own, foreign))
-
         return matches
 
     def to_json_data(self) -> Dict[str, any]:
         """
         :return: Returns the body specification in a json-ready dictionary
         """
         geometry = {}
@@ -274,14 +282,25 @@
         }
 
     @abc.abstractmethod
     def __copy__(self):
         """Returns a copy of the body"""
         pass
 
+    def __eq__(self, other):
+        """Equality check. The visual attribute is not checked as it does not provide relevant functionality."""
+        if not isinstance(other, BodyBase):
+            return NotImplemented
+        return self.collision == other.collision and self.connectors == other.connectors and \
+            self.inertia == other.inertia and self._id == other._id
+
+    def __hash__(self):
+        """Hashing: We assume IDs are unique, so it poses a valid hash."""
+        return hash(self.id)
+
     def __str__(self) -> str:
         """The string representation of a body"""
         return f"Body: {self.id}"
 
 
 class Body(BodyBase):
     """The default body class, represents a static/immutable rigid body."""
@@ -316,15 +335,15 @@
 
         if collision is None:
             raise ValueError("Collision model must be given! EmptyGeometry is a possible workaround.")
         self.collision: Geometry = collision
         self._visual: Geometry = visual
 
     @classmethod
-    def from_json_data(cls, d: Dict, package_dir: Path = None) -> Body:
+    def from_json_data(cls, d: Dict, package_dir: Path = None, *args, **kwargs) -> Body:
         """
         Maps the json-serialized body description to an instance of this class.
 
         The dictionary will be modified in-place until empty (everything was parsed).
 
         :param d: A dictionary with relevant meta-information
         :param package_dir: If a mesh is given, it is given relative to a package directory that must be specified
@@ -387,13 +406,9 @@
             inertia=self.inertia,
             collision=self.collision,
             visual=self.visual,
             in_module=self.in_module
         )
 
 
-class BodySet(SingleSet):
+class BodySet(SingleSetWithID):
     """A set that raises an error if a duplicate body is added"""
-
-    def __contains__(self, item: BodyBase):
-        """Custom duplicate check (unique ID)"""
-        return item.id in (bod.id for bod in self)
```

### Comparing `timor-python-0.0.8/src/timor/Geometry.py` & `timor-python-0.0.9/src/timor/Geometry.py`

 * *Files 7% similar despite different names*

```diff
@@ -121,15 +121,16 @@
             self.collision_geometry = hppfcl_representation
 
     def to_json_string(self) -> str:
         """Returns a json string representation of this geometry."""
         return json.dumps(self.serialized, indent=2)
 
     @classmethod
-    def from_json_data(cls, d: Union[List, Dict[str, any]], package_dir: Optional[Path] = None) -> Geometry:
+    def from_json_data(cls, d: Union[List, Dict[str, any]], package_dir: Optional[Path] = None,
+                       *args, **kwargs) -> Geometry:
         """
         Takes a serialized geometry specification and returns the according Geometry instance.
 
         :param d: A serialized geometry
         :param package_dir: The top directory to which the mesh file paths are relative to. Necessary for meshes (only).
         """
         if isinstance(d, (list, tuple, set)):
@@ -140,21 +141,21 @@
 
         if cls is not Geometry:
             raise AttributeError("Class {} does not support this method. Call it on the Geometry class.".format(cls))
         desc = d.copy()
         class_ref = _geometry_type2class(desc.pop('type'))
 
         if class_ref is Mesh:
-            if package_dir is None:
-                raise ValueError("If your geometry contains a mesh, you need to provide the package_dir")
-            desc['parameters']['package_dir'] = package_dir
-            # The "package://" prefix might be given, but is not mandatory.
-            desc['parameters']['file'] = re.sub('package://', '', desc['parameters']['file'])
-            if not (package_dir / Path(desc['parameters']['file'])).exists():
-                raise ValueError("Mesh file {} does not exist".format(package_dir / desc['parameters']['file']))
+            if package_dir is not None:
+                # The "package://" prefix might be given, but is not mandatory.
+                desc['parameters']['file'] = re.sub('package://', '', desc['parameters']['file'])
+                desc['parameters']['file'] = package_dir / Path(desc['parameters']['file'])
+
+            if not (Path(desc['parameters']['file'])).exists():
+                raise FileNotFoundError("Mesh file {} does not exist".format(desc['parameters']['file']))
 
         return class_ref(**desc)
 
     @classmethod
     def from_json_string(cls, description: str, package_dir: Optional[Path] = None) -> Geometry:
         """
         Takes a serialized geometry specification and returns the according Geometry instance.
@@ -186,16 +187,18 @@
             raise ValueError("Call from_pin_geometry on the Geometry class, not on a subclass.")
         fcl = geo.geometry
         will_be_instance_of = _geometry_type2class(GeometryType[type(fcl)])
         intermediate = will_be_instance_of.from_hppfcl(hppfcl.CollisionObject(fcl, geo.placement.rotation,
                                                                               geo.placement.translation))
         if isinstance(intermediate, Mesh):
             logging.debug("Restoring mesh file information from pinocchio geometry object")
-            intermediate.parameters['file'] = geo.meshPath
-            intermediate.parameters['scale'] = geo.meshScale
+            params = intermediate.parameters
+            params['file'] = geo.meshPath
+            params['scale'] = geo.meshScale
+            intermediate.parameters = params  # Trigger setter
         return intermediate
 
     @property
     def as_hppfcl_collision_object(self) -> Tuple[hppfcl.CollisionObject, ...]:
         """Creates hppfcl CollisionObject(s) at the current pose of self."""
         return hppfcl.CollisionObject(self.collision_geometry, self.placement.as_transform3f()),
 
@@ -243,14 +246,27 @@
     def _make_collision_geometry(self) -> hppfcl.CollisionGeometry:
         """Creates a hppfcl collision object aligned with the parameters of the Geometry"""
 
     def __deepcopy__(self, memodict={}):
         """Must be implemented for Geometries, as hppfcl does not natively support it."""
         return self.__class__(self.parameters, self.placement)
 
+    def __eq__(self, other: Geometry):
+        """Compares two Geometry instances based on their type, parameters and placement."""
+        if isinstance(other, Geometry) and not isinstance(other, Mesh):
+            this_parameters = tuple(sorted(((k, v) for k, v in self.parameters.items()), key=lambda x: x[0]))
+            other_parameters = tuple(sorted(((k, v) for k, v in other.parameters.items()), key=lambda x: x[0]))
+            return self.type == other.type and this_parameters == other_parameters and self.placement == other.placement
+        else:
+            return NotImplemented
+
+    def __hash__(self):
+        """Hashes the Geometry instance based on its type, parameters and placement."""
+        return hash((self.type, tuple(hash(p) for p in self.parameters.items()), self.placement.to_json_string()))
+
 
 class Box(Geometry):
     """A simple geometry with a box extending in x, y and z direction."""
 
     parameter_names: Tuple[str, str, str] = ('x', 'y', 'z')
     type: GeometryType = GeometryType.BOX
 
@@ -418,22 +434,21 @@
 
 class Mesh(Geometry):
     """Meshes can be any geometry represented by a set of triangles"""
 
     type: GeometryType = GeometryType.MESH
     _filepath: Path
     _scale: Union[float, np.ndarray]
-    package_dir: Optional[Path]
     _colors: Optional[np.ndarray] = None
 
     @classmethod
     def from_hppfcl(cls, fcl: hppfcl.CollisionObject) -> Geometry:
         """Wraps a hppfcl Mesh in a Mesh instance."""
         logging.debug("Creating mesh from hppfcl, will lose possible file location information")
-        return cls({'file': '', 'package_dir': ''}, fcl.getTransform(), fcl.collisionGeometry())
+        return cls({'file': ''}, fcl.getTransform(), fcl.collisionGeometry())
 
     @staticmethod
     def read_wrl(file: Path) -> Tuple[Tuple[np.ndarray, ...], Tuple[np.ndarray, ...]]:
         """
         Reads each sub-mesh from a wrl file into separate vertex and face arrays.
 
         The WRL format describes triangulated meshes and can contain multiple sub meshes that are parsed separately.
@@ -484,40 +499,38 @@
                     self._colors = m.visual.vertex_colors[:, :3] / 255
                 else:
                     logging.info("Install trimesh / timor full to enable color meshes.")
             return mesh_loader.load(str(self.abs_filepath), self.scale)
 
     @property
     def abs_filepath(self) -> Path:
-        """The absolute filepath is the combination of package path and relative path of the mesh file."""
-        if self.package_dir is None:
-            raise AttributeError("package_dir not set")
-
-        return self.package_dir / self.filepath
+        """The absolute filepath of the mesh file."""
+        return self.filepath
 
     @property
     def parameters(self) -> Dict[str, Union[str, float]]:
         """The mesh geometry is the only one that does not return the full parameters: Package dir is not returned!
 
         The parameters are given as {'file': str, 'scale': [float, array]}, where scale is optional and can be boat,
         a single float or an array of (x, y, z)-scale.
         """
         return {'file': str(self.filepath), 'scale': self.scale.tolist()}  # tolist to allow serialization
 
     @parameters.setter
     def parameters(self, parameters: Dict[str, any]):
-        """Unpacks to filepath and scale - also expects a package_dir to be able to load the mesh."""
-        self.package_dir = parameters['package_dir']
+        """Unpacks to filepath and scale."""
         self._filepath = Path(parameters['file'])
+        if 'package_dir' in parameters:
+            self._filepath = Path(parameters['package_dir']) / self._filepath
         self._scale = np.asarray(parameters.get('scale', 1.0))
 
     @property
     def urdf_properties(self) -> Tuple[str, Dict[str, Union[str, List[float]]]]:
         """Can only be saved as a dictionary if the mesh was loaded from a file and the file location is still known."""
-        return 'mesh', {'filename': 'package://' + str(self.filepath), 'scale': self.scale.tolist()}
+        return 'mesh', {'filename': str(self.filepath), 'scale': self.scale.tolist()}
 
     @property
     def viz_object(self) -> Tuple[meshcat.geometry.Geometry, Transformation]:
         """Returns a meshcat mesh"""
         geom = pin.visualize.meshcat_visualizer.loadMesh(self.collision_geometry), self.placement
         if self._colors is not None:
             if geom[0].vertices.shape == self._colors.shape:
@@ -547,17 +560,29 @@
         if isinstance(self._scale, float) or self._scale.size == 1:
             return np.array([self._scale, self._scale, self._scale])
         return self._scale
 
     def __deepcopy__(self, memodict={}):
         """Must be implemented for Geometries, as hppfcl does not natively support it."""
         params = self.parameters
-        params['package_dir'] = self.package_dir
         return self.__class__(params, self.placement)
 
+    def __eq__(self, other: Geometry):
+        """We don't care about Mesh file paths, but equality of their collision geometries."""
+        if isinstance(other, Mesh):
+            return self.type == other.type \
+                and np.all(self.scale == other.scale) \
+                and self.placement == other.placement \
+                and self.collision_geometry == other.collision_geometry
+        return NotImplemented
+
+    def __hash__(self):
+        """Scale can't always be hashed as it can be a numpy array"""
+        return hash((self.type, np.array(self.scale).tobytes(), self.placement.to_json_string()))
+
 
 class ComposedGeometry(Geometry):
     """A composed geometry is a collection of geometries that are combined in one instance."""
 
     type: GeometryType = GeometryType.COMPOSED
 
     def __init__(self, geometries: Iterable[Geometry]):
@@ -622,26 +647,39 @@
         raise NotImplementedError("ComposedGeometries cannot be visualized.")
 
     @property
     def volume(self) -> float:
         """The volume of a composed geometry is the sum of the volumes of the composing geometries."""
         return sum(g.volume for g in self.composing_geometries)
 
+    def __eq__(self, other):
+        """Equality is defined as having the same composing geometries."""
+        if not isinstance(other, ComposedGeometry):
+            return False
+        return set(g for g in self.composing_geometries if not isinstance(g, EmptyGeometry)) == \
+            set(g for g in other.composing_geometries if not isinstance(g, EmptyGeometry))
+
+    def __hash__(self):
+        """Hash is defined as the hash of the composing geometries."""
+        return sum(hash(g) for g in self.composing_geometries if not isinstance(g, EmptyGeometry))
+
 
 class EmptyGeometry(Geometry):
     """This is a dummy geometry to being able to prevent setting a geometry to None."""
 
     type: GeometryType = GeometryType.EMPTY
 
     def __init__(self,
                  parameters: Dict[str, Union[float, str]] = None,
                  pose: TransformationLike = Transformation.neutral(),
                  hppfcl_representation: Optional[hppfcl.CollisionGeometry] = None
                  ):
         """For an empty geometry, the parameters are not used."""
+        if parameters is not None:
+            logging.warning("EmptyGeometry does not use parameters, but they were given.")
         parameters = dict()
         super().__init__(parameters, pose, hppfcl_representation)
 
     @classmethod
     def from_hppfcl(cls, fcl: hppfcl.CollisionObject) -> Geometry:
         """This method is not implemented as it is not necessary."""
         raise NotImplementedError("Empty geometries are not loaded from hppfcl.")
@@ -680,7 +718,17 @@
     def volume(self) -> float:
         """No Geometry, no volume."""
         return 0.0
 
     def _make_collision_geometry(self) -> hppfcl.CollisionGeometry:
         """No Geometry, no collision object."""
         pass
+
+    def __eq__(self, other):
+        """Empty geometries are equal to other empty geometries."""
+        if isinstance(other, EmptyGeometry):
+            return True
+        return NotImplemented
+
+    def __hash__(self):
+        """Empty geometries are equal to other empty geometries."""
+        return hash(self.__class__.__name__)
```

### Comparing `timor-python-0.0.8/src/timor/Joints.py` & `timor-python-0.0.9/src/timor/Joints.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import json
 from typing import Dict, List, Tuple, Type, Union
 
 import numpy as np
 import pinocchio as pin
 
 from timor.Bodies import BodyBase, ConnectorSet
-from timor.utilities.dtypes import SingleSet, fuzzy_dict_key_matching
+from timor.utilities.dtypes import SingleSetWithID, fuzzy_dict_key_matching
 import timor.utilities.errors as err
 from timor.utilities.jsonable import JSONable_mixin
 from timor.utilities.transformation import Transformation, TransformationLike
 
 
 class TimorJointType(Enum):
     """Enumerates joint types available in Timor"""
@@ -109,20 +109,16 @@
         self.motor_inertia: float = float(motor_inertia)
         self.friction_coulomb: float = float(friction_coulomb)
         self.friction_viscous: float = float(friction_viscous)
 
         self.parent2joint: Transformation = Transformation(parent2joint)
         self.joint2child: Transformation = Transformation(joint2child)
 
-    def __str__(self):
-        """Joint representation of the joint"""
-        return f"Joint: {self.id}"
-
     @classmethod
-    def from_json_data(cls, d: Dict, body_id_to_instance: Dict) -> Joint:
+    def from_json_data(cls, d: Dict, body_id_to_instance: Dict, *args, **kwargs) -> Joint:
         """
         Maps the serialized json description to an instance of this class.
 
         :param d: A dictionary with relevant meta-information
         :param body_id_to_instance: A mapping from body IDs to the python instance of this body
         :return: An instantiated joint
         """
@@ -254,25 +250,39 @@
         elif self.type is TimorJointType.fixed:
             raise TypeError("Pinocchio does not have fixed joints. They are represented as frames")
         elif (self.type is TimorJointType.revolute_passive) or (self.type is TimorJointType.prismatic_passive):
             raise TypeError("Pinocchio does not have passive joints. They are represented as frames")
         else:
             raise ValueError("Unknown joint type")
 
+    def __eq__(self, other):
+        """Equality check for joints"""
+        if not isinstance(other, Joint):
+            return NotImplemented
+        return self._id == other._id and self.type == other.type and np.all(self.limits == other.limits) and \
+            self.acceleration_limit == other.acceleration_limit and self.velocity_limit == other.velocity_limit and \
+            self.parent2joint == other.parent2joint and self.joint2child == other.joint2child and \
+            self.gear_ratio == other.gear_ratio and self.motor_inertia == other.motor_inertia and \
+            self.friction_coulomb == other.friction_coulomb and self.friction_viscous == other.friction_viscous
+
+    def __hash__(self):
+        """Hash of the joint - we assume the ID is unique"""
+        return hash(self.id)
+
     def __getstate__(self):
         """Returns the state of this object as a dictionary"""
         state = self.to_json_data()
         state['body_id_to_instance'] = {body._id: body for body in (self.parent_body, self.child_body)}
         return state
 
     def __setstate__(self, state):
         """Sets the state of this object from a dictionary"""
         cpy = self.__class__.from_json_data(state, state.pop('body_id_to_instance'))
         self.__dict__ = cpy.__dict__
 
+    def __str__(self):
+        """Joint representation of the joint"""
+        return f"Joint: {self.id}"
 
-class JointSet(SingleSet):
-    """A set that raises an error if a duplicate joint is added"""
 
-    def __contains__(self, item: Joint) -> bool:
-        """Custom check for duplicate joints (same ID)"""
-        return item.id in (jnt.id for jnt in self)
+class JointSet(SingleSetWithID):
+    """A set that raises an error if a duplicate joint is added"""
```

### Comparing `timor-python-0.0.8/src/timor/Module.py` & `timor-python-0.0.9/src/timor/Module.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from collections import Counter
 import copy
 from dataclasses import dataclass
 import datetime
 import itertools
 import json
 import math
+import os.path
 from pathlib import Path
 import random
 import re
 from typing import Any, Callable, Collection, Dict, Iterable, List, Optional, Set, Tuple, Union
 import uuid
 import warnings
 import xml.etree.ElementTree as ET
@@ -21,19 +22,20 @@
 import numpy as np
 import pinocchio as pin
 
 from timor import Geometry, Robot
 from timor.Bodies import Body, BodyBase, BodySet, Connector, ConnectorSet, Gender
 from timor.Geometry import ComposedGeometry
 from timor.Joints import Joint, JointSet, TimorJointType
-from timor.utilities import logging, spatial, write_urdf
+from timor.utilities import configurations, logging, spatial, write_urdf
 from timor.utilities.dtypes import Lazy, SingleSet, TypedHeader, randomly
 import timor.utilities.errors as err
 from timor.utilities.file_locations import get_module_db_files, map2path, schema_dir
-from timor.utilities.json_serialization_formatting import compress_json_vectors, possibly_nest_as_list
+from timor.utilities.asset_handling import handle_assets
+from timor.utilities.json_serialization_formatting import possibly_nest_as_list
 from timor.utilities.jsonable import JSONable_mixin
 from timor.utilities.schema import DEFAULT_DATE_FORMAT, get_schema_validator
 from timor.utilities.transformation import Transformation, TransformationLike
 
 
 @dataclass
 class ModuleHeader(TypedHeader):
@@ -43,14 +45,18 @@
     name: str
     date: datetime.date = datetime.date.today()
     author: List[str] = TypedHeader.string_list_factory()
     email: List[str] = TypedHeader.string_list_factory()
     affiliation: List[str] = TypedHeader.string_list_factory()
     cost: float = 0.
 
+    def __hash__(self):
+        """Hash the header by hashing the unique ID and name."""
+        return hash((self.ID, self.name))
+
 
 class ModuleBase(abc.ABC, JSONable_mixin):
     """Base class for any robot module."""
 
     def __init__(self,
                  header: Union[Dict, ModuleHeader],
                  bodies: Iterable[BodyBase] = (),
@@ -75,22 +81,14 @@
             if not ((joint.parent_body in self.bodies) and (joint.child_body in self.bodies)):
                 raise ValueError("At least one of the joints parent/child bodies are missing in the module!")
             joint.in_module = self
         self._joints: JointSet = JointSet(joints)
         self._check_unique_connectors()
         self._module_graph: nx.DiGraph = self._build_module_graph()
 
-    def __copy__(self):
-        """Disable builtin copy, there should be no use case for two instances of a module with the same ID."""
-        raise NotImplementedError("Use custom module copy function and provide an ID suffix")
-
-    def __str__(self):
-        """String representation for the module."""
-        return f"Module {self.name}, ID: {self.id}"
-
     @property
     def connectors_by_own_id(self) -> Dict[str, Connector]:
         """
         Returns a mapping of connector._id values to the instance.
 
         Keep in mind, these are not the composed id's of the connectors, so they are not unambiguous outside a module!
         """
@@ -151,41 +149,18 @@
         return len(self._joints)
 
     @property
     def name(self) -> str:
         """Returns the unique name of this module."""
         return self.header.name
 
-    def _build_module_graph(self) -> nx.DiGraph:
-        """Builds the directed graph of atomic module elements. See module_graph property for more information."""
-        G_m = nx.DiGraph()
-        for body in self.bodies:
-            G_m.add_node(body)
-        for jnt in self.joints:
-            G_m.add_node(jnt)
-            # If a node is defined twice, networkx just interprets it as the same node
-            G_m.add_edge(jnt.parent_body, jnt, transform=jnt.parent2joint)
-            G_m.add_edge(jnt, jnt.child_body, transform=jnt.joint2child)
-
-        for connector_id, connector in self.available_connectors.items():
-            G_m.add_edge(connector.parent, connector, transform=connector.body2connector)
-
-        for u, v, t in G_m.edges.data('transform'):
-            # Generate the edges in opposing directing
-            G_m.add_edge(v, u, transform=t.inv)
-
-        return G_m
-
-    def _check_unique_connectors(self):
-        """Sanity check that all connectors are unique"""
-        if len(self.available_connectors) == 0:
-            return
-        counter = Counter(c._id for c in itertools.chain.from_iterable(b.connectors for b in self.bodies))
-        if max(counter.values()) > 1:
-            raise err.UniqueValueError("A module cannot contain multiple connectors with the same id.")
+    def can_connect(self, other: ModuleBase) -> bool:
+        """Returns true if at least one of the connectors of this module matches at least one connector of other"""
+        return any(this_con.connects(other_con) for this_con, other_con
+                   in itertools.product(self.available_connectors.values(), other.available_connectors.values()))
 
     def copy(self, suffix: str) -> ModuleBase:
         """
         Copies a module, but changes the id of the copy.
 
         :param suffix: Suffix to add to the copies' id. Necessary, to distinguish original and copy
         :return: A functional copy of this module with altered ID
@@ -226,19 +201,14 @@
             tmp_ass = ModuleAssembly(ModulesDB([self]), [self.id], (), base_connector_id)
         else:  # Otherwise, any connector can be fixed to environment
             base_connector_id = (0, list(self.available_connectors)[0][2])
             tmp_ass = ModuleAssembly(ModulesDB([self]), [self.id], (), base_connector_id)
 
         return tmp_ass.to_pin_robot(add_com_frames=show_com, base_placement=base_placement).visualize(viz, 'full')
 
-    def can_connect(self, other: ModuleBase) -> bool:
-        """Returns true if at least one of the connectors of this module matches at least one connector of other"""
-        return any(this_con.connects(other_con) for this_con, other_con
-                   in itertools.product(self.available_connectors.values(), other.available_connectors.values()))
-
     def to_json_data(self) -> Dict:
         """
         Write a json in that fully describes this module.
 
         :return: Returns the module specification in a json-ready dictionary
         """
         header = self.header.asdict()
@@ -246,14 +216,60 @@
 
         return {
             'header': header,
             'bodies': [body.to_json_data() for body in sorted(self.bodies, key=lambda b: b.id)],
             'joints': [joint.to_json_data() for joint in sorted(self.joints, key=lambda j: j.id)]
         }
 
+    def _build_module_graph(self) -> nx.DiGraph:
+        """Builds the directed graph of atomic module elements. See module_graph property for more information."""
+        G_m = nx.DiGraph()
+        for body in self.bodies:
+            G_m.add_node(body)
+        for jnt in self.joints:
+            G_m.add_node(jnt)
+            # If a node is defined twice, networkx just interprets it as the same node
+            G_m.add_edge(jnt.parent_body, jnt, transform=jnt.parent2joint)
+            G_m.add_edge(jnt, jnt.child_body, transform=jnt.joint2child)
+
+        for connector_id, connector in self.available_connectors.items():
+            G_m.add_edge(connector.parent, connector, transform=connector.body2connector)
+
+        for u, v, t in G_m.edges.data('transform'):
+            # Generate the edges in opposing directing
+            G_m.add_edge(v, u, transform=t.inv)
+
+        return G_m
+
+    def _check_unique_connectors(self):
+        """Sanity check that all connectors are unique"""
+        if len(self.available_connectors) == 0:
+            return
+        counter = Counter(c._id for c in itertools.chain.from_iterable(b.connectors for b in self.bodies))
+        if max(counter.values()) > 1:
+            raise err.UniqueValueError("A module cannot contain multiple connectors with the same id.")
+
+    def __copy__(self):
+        """Disable builtin copy, there should be no use case for two instances of a module with the same ID."""
+        raise NotImplementedError("Use custom module copy function and provide an ID suffix")
+
+    def __eq__(self, other):
+        """Equality check for modules. Two modules are equal if they have the same header, bodies, names, and joints."""
+        if not isinstance(other, ModuleBase):
+            return NotImplemented
+        return self.header == other.header and self.bodies == other.bodies and self.joints == other.joints
+
+    def __hash__(self):
+        """Custom hash function for modules that should be uniquely determined by their ID."""
+        return hash(self.id)
+
+    def __str__(self):
+        """String representation for the module."""
+        return f"Module {self.name}, ID: {self.id}"
+
 
 class AtomicModule(ModuleBase):
     """
     Atomic Modules are the simplest module representation. They are static (immutable) and can be (de)serialized.
     """
 
     def __init__(self, header: Union[Dict, ModuleHeader], bodies: Iterable[Body] = (), joints: Iterable[Joint] = ()):
@@ -311,15 +327,15 @@
             child.collision.placement = offset @ child.collision.placement
             child.inertia = child.inertia.se3Action(pin.SE3(offset.homogeneous))
 
         module._module_graph = module._build_module_graph()  # After changing connectors T, we need to fix the graph
         return module, np.asarray(colors.to_rgba(viz_colors.pop(), alpha=1))
 
     @classmethod
-    def from_json_data(cls, d: Dict, package_dir: Path) -> AtomicModule:
+    def from_json_data(cls, d: Dict, package_dir: Optional[Path] = None, **kwargs) -> AtomicModule:
         """
         Maps the json module description to an instance of this class.
 
         The dictionary will be modified in-place until empty (everything was parsed).
 
         :param package_dir: Package directory relative to which mesh file paths are defined
         :param d: A dictionary with relevant meta-information
@@ -345,23 +361,22 @@
 
         if len(d) > 0:
             raise ValueError("Unrecognized keys in module specification: " + str(d.keys()))
 
         return cls(header, bodies, joints)
 
     @classmethod
-    def from_json_string(cls, s: str, package_dir: Path) -> AtomicModule:
+    def from_json_string(cls, s: str) -> AtomicModule:
         """
         Maps the json module string to an instance of this class.
 
-        :param package_dir: Package directory relative to which mesh file paths are defined
         :param s: A json string with relevant meta-information
         :return: An instantiated module
         """
-        return cls.from_json_data(json.loads(s), package_dir)
+        return cls.from_json_data(json.loads(s))
 
 
 class ModulesDB(SingleSet, JSONable_mixin):
     """
     A Database of Modules. The inheritance from SingleSet ensures no duplicates are within one DB.
 
     Also, this means this class offers many useful methods inherited from Set, such as add() and update().
@@ -369,61 +384,31 @@
     This class provides safety regarding uniqueness of module, joint, body and connector IDs, but this comes at a price.
     Adding and removing elements can be expensive with growing modules. This class is not intended to be changed much,
     after being instantiated!
     """
 
     connection_type = Tuple[ModuleBase, Connector, ModuleBase, Connector]  # More specific than in Assembly!
     _name: Optional[str]  # Optional name of the database, i.e. for referencing them in the CoBRA API
-    _package_dir: Optional[Path]  # Optional package directory relative to which mesh file paths are defined
     _model_generation_kwargs: dict[str, Any]  # Default arguments to create a robot model from this ModulesDB with
 
-    def __init__(self, *modules: Iterable[ModuleBase], name: Optional[str] = None, package_dir: Optional[Path] = None,
-                 **model_generation_kwargs):
+    def __init__(self, *modules: Iterable[ModuleBase], name: Optional[str] = None, **model_generation_kwargs):
         """
         Initializes the database from any number of modules.
 
         :param modules: Any iterable over modules to be within the database
         :param name: Optional name of the database, i.e. for referencing them in the CoBRA API
-        :param package_dir: Optional package directory relative to which mesh file paths are defined
         :param model_generation_kwargs: Key-word arguments to pass to the robot model generation; esp. for setting
           ignore_collisions
 
         :source: Get selected ModulesDBs using the API: https://cobra.cps.cit.tum.de/api/robots
         """
         super().__init__(*modules)
         self._name = name
-        self._package_dir = package_dir
         self._model_generation_kwargs = model_generation_kwargs
 
-    def __contains__(self, item: ModuleBase) -> bool:
-        """
-        If a new module should be added to a Module DB, the following properties must be preserved:
-
-        (All of the below holds for modules and their sub-modules and their sub-sub-modules, and...
-        to keep it short, all of those are just described as "modules")
-
-          * All module IDs in the DB are unique
-          * All module names in the DB are unique
-          * All JointIDs in the DB are unique
-          * All BodyIDs in the DB are unique
-          * All ConnectorIDs in the DB are unique
-
-        :param item: A module
-        :return: Boolean indicator whether the module OR ANY OF THE INHERENT IDs are already in the DB
-        """
-        if item.id in self.all_module_ids:
-            return True
-        if item.name in self.all_module_names:
-            return True
-        if item.bodies.intersection(self.all_bodies):
-            return True
-        if item.joints.intersection(self.all_joints):
-            return True
-        return False
-
     def add(self, element: AtomicModule) -> None:
         """
         As the connector ID is composed of (module ID, body ID, connector ID), we need an additional check,
 
         we don't want two allow two connectors with same names in a module, even if attached to different bodies.
         """
         # if any(con_id in self.all_connector_own_ids for con_id in element._connectors_by_own_id):
@@ -431,91 +416,74 @@
         super().add(element)
 
     def filter(self, func: Callable[[AtomicModule], bool]) -> ModulesDB:
         """
         Apply a custom filter to this DB to get a new DB with only the modules that pass the filter.
 
         :param func: A function that takes a module and returns a boolean
-        :return: A new DB with only the modules that pass the filter. The package_dir is preserved, the name is
-            intentionally discarded to avoid confusion.
+        :return: A new DB with only the modules that pass the filter. The name is intentionally discarded to avoid
+          confusion.
         """
         new_db = super().filter(func)
-        new_db._package_dir = self._package_dir
         return new_db
 
     @classmethod
     def from_name(cls, module_db_name) -> ModulesDB:
         """
         Create module DB from name of a module DB configured as loadable robot in timor.config
         """
-        return cls.from_file(*get_module_db_files(module_db_name))
+        return cls.from_json_file(get_module_db_files(module_db_name))
 
     @classmethod
-    def from_file(cls, filepath: Union[Path, str], package_dir: Union[Path, str]) -> ModulesDB:
+    def from_json_file(cls, filepath: Union[Path, str], *args, **kwargs) -> ModulesDB:
         """
         Loads a modules Database from a json file.
 
-        :param filepath: Path to the json file of the modulesDB definition.
-        :param package_dir: Package directory relative to which mesh file paths are defined
-        :return: A ModulesDB
+        :param filepath: Path to the json file
+        :return: The loaded ModulesDB
         """
-        filepath, package_dir = map(map2path, (filepath, package_dir))
-        with filepath.open('r') as json_file:
-            content = json_file.read()
         name = filepath.parent.stem
-        return cls.from_json_string(content, package_dir, name=name)
+        return super().from_json_file(filepath, name=name, *args, **kwargs)
 
     @classmethod
-    def from_json_string(cls, json_string: str, package_dir: Path, name: Optional[str] = None) -> ModulesDB:
-        """
-        Loads a modules Database from a json string.
-
-        :param json_string: Json string of the modulesDB definition.
-        :param package_dir: Package directory relative to which mesh file paths are defined
-        :param name: Referencing name for the database
-        :return: A ModulesDB
-        """
-        return cls.from_json_data(json.loads(json_string), package_dir, name)
-
-    @classmethod
-    def from_json_data(cls, data: Iterable[dict], package_dir: Path, name: Optional[str] = None) -> ModulesDB:
+    def from_json_data(cls, data: Dict, name: Optional[str] = None,
+                       validate: Optional[bool] = True, *args, **kwargs) -> ModulesDB:
         """
         Loads a modules Database from a json string.
 
         :param data: Set of dicts describing the individual modules in the DB.
-        :param package_dir: Package directory relative to which mesh file paths are defined
         :param name: Referencing name for the database
+        :param validate: Whether to validate the data against the module schema
         :return: A ModulesDB
         """
-        _, validator = get_schema_validator(schema_dir.joinpath("ModuleSchema.json"))
-        if not validator.is_valid(data):
-            logging.debug(f"Errors: {tuple(validator.iter_errors(data))}")
-            raise ValueError("modules.json invalid.")
-        db = cls(package_dir=package_dir, name=name, **{k: data[k] for k in data if k != "modules"})
+        if validate:
+            _, validator = get_schema_validator(schema_dir.joinpath("ModuleSchema.json"))
+            if not validator.is_valid(data):
+                logging.debug(f"Errors: {tuple(validator.iter_errors(data))}")
+                raise ValueError("modules.json invalid.")
+        db = cls(name=name, **{k: data[k] for k in data if k != "modules"})
 
         for module_data in data["modules"]:
-            db.add(AtomicModule.from_json_data(module_data, package_dir))
+            db.add(AtomicModule.from_json_data(module_data))
         return db
 
-    def to_json_file(self, save_at: Union[Path, str]):
+    def to_json_file(self, save_at: Union[Path, str], *args, **kwargs):
         """
         Writes the ModulesDB to a json file.
 
         :param save_at: File location or folder to write the DB to.
         """
-        save_at = Path(save_at)
-        if save_at.is_dir():
-            if self._name is None:
-                raise ValueError("The DB needs a name if only a directory is specified for saving!")
-            save_at = save_at.joinpath(self._name + '.json')
-        content = compress_json_vectors(self.to_json_string())
-        if (self._package_dir is not None) and (not str(save_at).startswith(str(self._package_dir))):
-            logging.info("Writing ModulesDB to file outside of the package directory it was loaded from.")
-        with Path(save_at).open('w') as savefile:
-            savefile.write(content)
+        save_at = map2path(save_at)
+        if save_at.stem != "modules":
+            raise ValueError("Modules DB must be saved as 'modules.json'")
+        if self._name is not None:
+            if save_at.parent.stem != self._name:
+                raise ValueError("The name of the DB must be the same as the name of the folder it is saved in.")
+
+        return super().to_json_file(save_at, *args, **kwargs)
 
     def to_json_data(self) -> dict[str, list[Any]]:
         """
         Turn modulesDB into jsonable dict.
 
         :return: The jsonable data.
         """
@@ -571,59 +539,58 @@
     def by_name(self) -> Dict[str, ModuleBase]:
         """Returns this DB as a dictionary, mapping the Module Name to the module"""
         return {mod.name: mod for mod in self}
 
     @property
     def bases(self) -> ModulesDB[ModuleBase]:
         """Returns all modules containing at least one base connector"""
-        return self.__class__((mod for mod in self if any(c.type == 'base' for c in mod.available_connectors.values())),
-                              package_dir=self._package_dir)
+        return self.__class__((mod for mod in self if any(c.type == 'base' for c in mod.available_connectors.values())))
 
     @property
     def default_model_generation_kwargs(self):
         """A default set of model generation kwargs to use with this modules db."""
         return self._model_generation_kwargs
 
     @property
     def end_effectors(self) -> ModulesDB[ModuleBase]:
         """Returns all modules containing at least one eef connector"""
-        return self.__class__((mod for mod in self if any(c.type == 'eef' for c in mod.available_connectors.values())),
-                              package_dir=self._package_dir)
+        return self.__class__((mod for mod in self if any(c.type == 'eef' for c in mod.available_connectors.values())))
 
     @property
     def name(self) -> str:
         """Return name of module db as given in the CoBRA API"""
         return self._name
 
     @property
     def possible_connections(self) -> Set[ModulesDB.connection_type]:
         """
         Returns a set of all possible connections in this db.
 
-        As connections are symmetric, only one copy of {A --> B, B --> A} will be returned.
+        As connections are symmetric, only one copy of {(A, c_a) --> (B, c_b), (B, c_b) --> (A, c_a)} will be returned.
         """
         connections: Set[ModulesDB.connection_type] = set()
         for mod_a, mod_b in itertools.combinations_with_replacement(self, 2):
             for con_a, con_b in itertools.product(mod_a.available_connectors.values(),
                                                   mod_b.available_connectors.values()):
                 if con_a.connects(con_b):
                     if mod_a is mod_b and ((mod_a, con_a, mod_b, con_b) in connections):
                         # Avoiding duplicates
                         continue
                     connections.add((mod_a, con_a, mod_b, con_b))
         return connections
 
     @property
-    def connectivity_graph(self) -> nx.DiGraph:
+    def connectivity_graph(self) -> nx.MultiDiGraph:
         """
         Returns a graph of all possible module connections in the db.
 
-        :return: An undirected graph
+        :return: A directed graph with anti-parallel edges for each possible connection. Multiple edges between two are
+            possible (in fact, they will almost certainly exist for standard module sets).
         """
-        G = nx.DiGraph()
+        G = nx.MultiDiGraph()
         for mod_a, con_a, mod_b, con_b in self.possible_connections:
             G.add_edge(mod_a, mod_b, connectors=(con_a, con_b))
             G.add_edge(mod_b, mod_a, connectors=(con_b, con_a))
         return G
 
     def debug_visualization(self,  # pragma: no cover
                             viz: pin.visualize.MeshcatVisualizer = None,
@@ -643,14 +610,56 @@
 
         for i, module_idx in enumerate(sorted(list(self.all_module_ids))):
             self.by_id[module_idx].debug_visualization(
                 viz=viz, base_placement=spatial.homogeneous((stride * math.floor(i / cols), stride * i % cols, 0)))
 
         return viz
 
+    def __contains__(self, item: ModuleBase) -> bool:
+        """
+        If a new module should be added to a Module DB, the following properties must be preserved:
+
+        (All of the below holds for modules and their sub-modules and their sub-sub-modules, and...
+        to keep it short, all of those are just described as "modules")
+
+          * All module IDs in the DB are unique
+          * All module names in the DB are unique
+          * All JointIDs in the DB are unique
+          * All BodyIDs in the DB are unique
+          * All ConnectorIDs in the DB are unique
+
+        :param item: A module
+        :return: Boolean indicator whether the module OR ANY OF THE INHERENT IDs are already in the DB
+        """
+        if item.id in self.all_module_ids:
+            return True
+        if item.name in self.all_module_names:
+            return True
+        if item.bodies.intersection(self.all_bodies):
+            return True
+        if item.joints.intersection(self.all_joints):
+            return True
+        return False
+
+    def __eq__(self, other):
+        """Two DBs are equal if they contain the same modules, have the same name, and generate the same robot model."""
+        if not isinstance(other, ModulesDB):
+            return NotImplemented
+        return self.name == other.name \
+            and self.default_model_generation_kwargs == other.default_model_generation_kwargs \
+            and super().__eq__(other)
+
+    def __setstate__(self, state):
+        """
+        Overwrite jsonable; most is handled by __reduce__ and python internal set
+
+        just need to set helper properties
+        """
+        self.__dict__.update(state)
+
 
 class ModuleAssembly(JSONable_mixin):
     """
     A combination of modules with defined connections between each another.
 
     Represents a high-level abstraction to a robot and provides an interface to the kinematic model.
     """
@@ -758,35 +767,31 @@
     @classmethod
     def empty(cls):
         """Creates an empty assembly built from an emtpy database"""
         db = ModulesDB()
         return cls(db)
 
     @classmethod
-    def from_monolithic_robot(cls, robot: Robot.PinRobot, urdf: Optional[Path] = None) -> ModuleAssembly:
+    def from_monolithic_robot(cls, robot: Robot.PinRobot) -> ModuleAssembly:
         """
         Wraps a kinematic/dynamic robot model into a single module which will be the full assembly.
 
         This method wraps the existing kinematic and dynamic pin model and continues to use it - the computational
         effort of re-generating a model is spared, so if input robot changes, the robot property of the assembly
         returned by this method will as well.
 
         :param robot: A pinocchio robot model to be wrapped in an assembly.
-        :param urdf: Optional urdf to try to reconstruct mesh file paths with.
 
         :returns: A module assembly consisting of exactly one module: The robot given as input.
         """
         child_bodies = dict()
         joints = set()
         zero_inertia = pin.Inertia()
         zero_inertia.setZero()
 
-        if urdf is not None:
-            urdf = ET.parse(urdf)
-
         # First, parse the geometries and add them to fresh bodies
         if len(robot.collision.geometryObjects) != len(robot.visual.geometryObjects):
             raise NotImplementedError("Assembly wrapper cannot handle robots with different numbers of "
                                       "collision and visual geometries.")
         for collision, visual in zip(robot.collision.geometryObjects, robot.visual.geometryObjects):
             cg = Geometry.Geometry.from_pin_geometry(collision)
             vg = Geometry.Geometry.from_pin_geometry(visual)
@@ -800,39 +805,14 @@
 
             def find_unique_child(tree, search_term):
                 candidates = tree.findall(search_term)
                 if len(candidates) != 1:
                     raise IndexError(f"Search term \"{search_term}\" not unique: {candidates}")
                 return candidates[0]
 
-            if urdf is not None:
-                if not collision.name[-2:] == "_0":  # Pinocchio adds index if multiple visual / collision tags per link
-                    raise ValueError("Can only use URDF if there is a single collision geometry")
-
-                link_name_urdf = collision.name[:-2]
-                link_candidate = find_unique_child(urdf, f".//link[@name='{link_name_urdf}']")
-
-                if isinstance(vg, Geometry.Mesh):
-                    visual_candidate = find_unique_child(link_candidate, "visual/geometry")
-                    try:
-                        visual_mesh_candidate = find_unique_child(visual_candidate, "mesh")
-                    except IndexError:
-                        raise ValueError(f"No unique mesh found for visual geometry {vg}.")
-                    if "filename" in visual_mesh_candidate.attrib:
-                        vg._filepath = visual_mesh_candidate.attrib["filename"].replace("package://", "")
-
-                if isinstance(cg, Geometry.Mesh):
-                    collision_candidate = find_unique_child(link_candidate, "collision/geometry")
-                    try:
-                        collision_mesh_candidate = find_unique_child(collision_candidate, "mesh")
-                    except IndexError:
-                        raise ValueError(f"No unique mesh found for collision geometry {cg}.")
-                    if "filename" in collision_mesh_candidate.attrib:
-                        cg._filepath = collision_mesh_candidate.attrib["filename"].replace("package://", "")
-
             inertia = robot.model.inertias[collision.parentJoint]
             child_bodies[collision.parentJoint] = Body(body_id=collision.name, collision=cg, visual=vg, inertia=inertia)
 
         # Now, parse the joints
         for frame in robot.model.frames:
             if frame.type is pin.FrameType.FIXED_JOINT:
                 parent_joint = frame.parent
@@ -1119,15 +1099,16 @@
         plt.subplots(figsize=(12, 12))
         pos = nx.spring_layout(G, k=1.1 / (len(G) ** .5), scale=1.2)
         nx.draw(G, pos=pos, with_labels=True)
         plt.tight_layout()
         plt.show()
 
     @classmethod
-    def from_json_data(cls, d: Dict[str, any], module_db: Optional[ModulesDB] = None) -> ModuleAssembly:
+    def from_json_data(cls, d: Dict[str, any], module_db: Optional[ModulesDB] = None,
+                       *args, **kwargs) -> ModuleAssembly:
         """
         Create an assembly from description found in serialized solutions.
 
         :param d: dictionary with keys from solution that allow to reconstruct a module assembly.
           Always needs moduleSet field if no additional module_db given.
           Always needs moduleOrder.
           Supported combinations:
@@ -1164,24 +1145,27 @@
                                self.internal_module_ids.index(m_b.header.ID), c_b.id[2])
                               for m_a, c_a, m_b, c_b in self.connections]
         return {'moduleSet': self.db.name,
                 'moduleOrder': self.original_module_ids,  # Map to module type ids
                 'moduleConnection': module_connections,
                 # For now assumed only one base
                 'baseConnection': [(self.internal_module_ids.index(self.base_module.id), self.base_connector.id[2], 0)],
-                'basePose': [self.robot.placement.homogeneous]}
+                'basePose': [self.robot.placement.to_json_data()]}
 
     def to_pin_robot(self,
                      base_placement: TransformationLike = Transformation.neutral(),
                      add_com_frames: bool = False,
                      ignore_collisions: str = 'via_joint') -> Robot.PinRobot:
         """
         Creates a pinocchio robot from a module tree
 
-        :param base_placement: placement for the (single) base connector as 4x4 hom. transformation
+        :param base_placement: Relative placement of the base in the world frame -- attention! This is not the placement
+            for the "base connector" which is pointing "away" from the base, but it is the base connector placement
+            rotated by 180° degrees around its x-axis. This way, an identity "base placement" (for the typical DB)
+            corresponds to a base standing upright on the ground, centered in (0, 0, 0).
         :param add_com_frames: Add frames for the center of mass of each Body
         :param ignore_collisions: Should be one of 'rigid', 'via_joint' or 'rigid_via_joint'. This argument defines,
             which pairs of bodies of the robot are IGNORED when checking for collisions. All possible collision pairs
             that are not explicitly ignored will be checked for - the following list provides details:
 
             * rigid: All bodies can collide as long as they are not rigidly connected
             * via_joint: Two bodies that are directly connected by a joint cannot collide
@@ -1229,17 +1213,17 @@
                     if add_com_frames:  # Add center of mass as a child frame of this body
                         new_frame = robot \
                             .model \
                             .addFrame(pin.Frame('.'.join(successor.id + ("CoM",)),
                                                 parent_joints[successor.id],
                                                 frames[successor.id],
                                                 pin.SE3((
-                                                        Transformation(transforms[successor.id]) @
-                                                        Transformation.from_translation(successor.inertia.lever)
-                                                        ).homogeneous),
+                                                    Transformation(transforms[successor.id]) @
+                                                    Transformation.from_translation(successor.inertia.lever)
+                                                ).homogeneous),
                                                 pin.FrameType.OP_FRAME))
                         frames[successor.id + ("CoM",)] = new_frame
                         parent_joints[successor.id + ("CoM",)] = parent_joints[successor.id]
                 elif isinstance(successor, Joint) and successor.type is not TimorJointType.fixed:
                     options = successor.pin_joint_kwargs
                     options.update(no_update)  # Robot data will be updated once only - at the very end
                     options['joint_placement'] = pin.SE3(transform)  # Relative placement to parent joint
@@ -1299,22 +1283,28 @@
                 if [cg1, cg2] not in cps_to_remove:
                     active[cg1, cg2] = True
             robot.collision.setCollisionPairs(active)
             robot.collision_data = robot.collision.createData()
 
         return robot
 
-    def to_urdf(self, name: str = None, write_to: Optional[Path] = None, replace_wrl: bool = False) -> str:
+    def to_urdf(self, name: str = None, write_to: Optional[Path] = None, replace_wrl: bool = False,
+                handle_missing_assets: Optional[str] = None) -> str:
         """
         Creates a URDF file from the assembly.
 
         :param name: name to be given to robot inside URDF
         :param write_to: output URDF file
         :param replace_wrl: Whether to replace wrl geometries with visual geometry (if available).
+        :param handle_missing_assets: How to handle missing assets in package (parent of write_to).
+          See :meth:`timor.utilities.helper.handle_assets` for details.
         """
+        if handle_missing_assets is None:
+            handle_missing_assets = configurations.db_assets_copy_behavior
+
         G = self.assembly_graph
         edges = G.edges
         if name is None:
             name = 'Auto-Generated: ' + uuid.uuid4().hex  # Random Name
 
         def get_urdf_joint_type(joint_instance: Joint) -> str:
             pin2urdf = {pin.JointModelRZ: 'revolute', pin.JointModelPZ: 'prismatic'}
@@ -1410,14 +1400,29 @@
             urdf.append(subtree)
 
         try:
             ET.indent(urdf, space='\t', level=0)
         except AttributeError:
             # indent was introduced in Python 3.9 -- for previous versions, we just don't pretty-print
             pass
+
+        if write_to is not None:
+            package_dir = write_to.parent
+            meshes = urdf.findall(".//mesh")
+            if meshes:
+                old_file_names = [m.attrib["filename"] for m in meshes]
+                old_package_dir = map2path(os.path.commonpath(old_file_names)).parent
+                for m in meshes:
+                    m.attrib["filename"] = m.attrib["filename"].replace(str(old_package_dir), "package:/")
+                new_file_names = [m.attrib["filename"] for m in meshes]
+
+                handle_assets([Path(f.replace("package:/", str(package_dir))) for f in new_file_names],
+                              [Path(o) for o in old_file_names],
+                              handle_missing_assets)
+
         urdf_string = ET.tostring(urdf, 'unicode')
 
         if write_to is not None:
             with write_to.open('w') as writefile:
                 writefile.write(urdf_string)
 
         return urdf_string
@@ -1501,14 +1506,38 @@
 
         # Lastly, check there are no "loose" modules
         if len(self.module_instances) > 1 and not len(seen_modules) == len(self.module_instances):
             raise ValueError(f"Not every module in the assembly seems to be connect!\n"
                              f"Connected: {len(seen_modules)}\n"
                              f"Modules in the assembly: {len(self.module_instances)}")
 
+    def _deterministic_connections(self) -> Tuple[Tuple[ModuleBase, Connector, ModuleBase, Connector], ...]:
+        """
+        Returns the connections in a deterministic order, so that the assembly can be hashed and compared.
+        """
+        return tuple(sorted(self.connections, key=lambda x: tuple(el.id for el in x)))
+
+    def __eq__(self, other):
+        """
+        Two assemblies are basically equal when they describe the same robot with equal modules.
+
+        Equality is given by equal connections (which implies equal connectors and modules) and equal kwargs for the
+        model generation: This means that equal assemblies must not necessarily be constructed from modules coming from
+        the same DB. However, all modules must be equal and the resulting robots must have the same kinematic, dynamic,
+        and geometric properties.
+        """
+        if not isinstance(other, ModuleAssembly):
+            return False
+        return self.connections == other.connections \
+            and self.db.default_model_generation_kwargs == other.db.default_model_generation_kwargs
+
+    def __hash__(self):
+        """Hash is based on the connections, as they are the defining property of an assembly."""
+        return hash(self._deterministic_connections())
+
     def __getstate__(self):
         """Used for pickling"""
         return self.to_json_data()
 
     def __setstate__(self, state):
         """Used for pickling"""
         cpy = self.__class__.from_json_data(state)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `timor-python-0.0.8/src/timor/Robot.py` & `timor-python-0.0.9/src/timor/Robot.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Date: 12.01.22
 from __future__ import annotations
 
 import abc
 import itertools
 from pathlib import Path
 import string
-from typing import Collection, Dict, List, Optional, Tuple, Union
+from typing import Callable, Collection, Dict, List, Optional, Tuple, Union
 from warnings import warn
 
 from hppfcl.hppfcl import CollisionObject, CollisionRequest, CollisionResult, Transform3f, collide
 from matplotlib import colors
 import numpy as np
 import pinocchio as pin
 import scipy.optimize as optimize
@@ -53,14 +53,34 @@
         """Returns a dictionary that can be used as kwargs for addBodyFrame (pinocchio)"""
         return {'body_name': self.name,
                 'parentJoint': parent_joint_id,
                 'body_placement': self.placement,
                 'previous_frame': parent_frame_id}
 
 
+def default_ik_cost_function(robot: RobotBase, q: np.ndarray, goal: Transformation) -> float:
+    """
+    The default cost function to evaluate the quality of an inverse kinematic solution.
+
+    This method returns the weighted sum of the translation and rotation error between the current and the goal, where
+    the 1m of displacement equals a cost of one and 180 degree of orientation error equals a cost of 1.
+    :param robot: The robot to evaluate the solution for
+    :param q: The current joint configuration
+    :param goal: The goal transformation
+    """
+    current = robot.fk(q, kind='tcp')
+    delta = current.distance(goal)
+    translation_error = delta.translation_euclidean
+    rotation_error = delta.rotation_angle
+    translation_weight = 1.
+    rotation_weight = .5 / np.pi  # .5 meter displacement ~ 180 degree orientation error
+    return (translation_weight * translation_error + rotation_weight * rotation_error) / \
+        (translation_weight + rotation_weight)
+
+
 class RobotBase(abc.ABC):
     """Abstract base class for all robot classes"""
 
     def __init__(self,
                  *,
                  name: str,
                  home_configuration: np.ndarray = None,
@@ -155,20 +175,14 @@
     def tcp_acceleration(self) -> np.ndarray:
         """
         Returns the current tcp acceleration as 6x1 numpy array
         """
 
     # ---------- Abstract Methods ----------
     @abc.abstractmethod
-    def _ik_cost_function(self, q: np.ndarray, goal: TransformationLike) -> float:
-        """
-        A cost function to get the fitness of an forward kinematics solution when calculating the inverse kinematics.
-        """
-
-    @abc.abstractmethod
     def collisions(self, task: 'Task.Task') -> List[Tuple[RobotBase, Obstacle]]:  # noqa: F821
         """
         Returns all collisions that appear between the robot and itself or obstacles in the task.
 
         :param task: The task to check for collisions
         :return: A list of tuples (robot, obstacle) for robot an obstacle in collision
         """
@@ -246,14 +260,22 @@
 
         :param q: Dimension njointsx1.
         :param dq: Velocities, optional
         :param ddq: Acceleration, optional
         """
 
     @abc.abstractmethod
+    def manipulability_index(self, q: Optional[np.ndarray]) -> float:
+        """
+        Calculate the Yoshikawa manipulability index at joint position q or current one.
+
+        :param q: Joint position to calculate at (default current robot configuration)
+        """
+
+    @abc.abstractmethod
     def visualize(self, viz: pin.visualize.MeshcatVisualizer, *args, **kwargs) -> pin.visualize.MeshcatVisualizer:
         """Interface to plot the robot in a meshcat visualizer"""
 
     # ---------- Properties and Aliases----------
 
     @property
     def name(self) -> str:
@@ -306,38 +328,44 @@
         """
         return self.ik_scipy(eef_pose, q_init, **kwargs)
 
     def ik_scipy(self,
                  eef_pose: ToleratedPose,
                  q_init: np.ndarray = None,
                  max_iter: int = 1000,
-                 restore_config: bool = True,
+                 restore_config: bool = False,
                  max_n_tries: int = 10,
+                 ik_cost_function: Callable[[RobotBase, np.ndarray, TransformationLike], float] = default_ik_cost_function,  # noqa: E501
                  **kwargs
                  ) -> Tuple[np.ndarray, bool]:
         """
         Computes the inverse kinematics (joint angles for a given goal destination).
 
         :param eef_pose: Desired end effector pose with tolerances.
         :param q_init: Initial joint angles to start searching from. If not given, uses current configuration
         :param max_iter: Maximum number of iterations before the algorithm gives up. If max_n_tries is larger than 1,
             max_iter is counted over all n tries.
         :param restore_config: If True, the current robot configuration will be kept. If false, the found solution for
             the inverse kinematics will be kept
         :param max_n_tries: Maximum number of runs with a new random init configuration before the algorithm gives up
+        :param ik_cost_function: A custom cost function that takes a robot, its joint angles, and a
+            TransformationLike and returns a scalar cost indicating the quality of the configuration in solving the ik
+            problem. If not given, the default cost function is used (equal weighting of .5 meter / 180 degree error).
         :param kwargs: Additional arguments, including:
             - task: If a timor.Task.Task is provided here, the ik will restart if there are task collisions as long as
                 max_iter is not reached.
             - joint_mask: A boolean array of length njoints that indicates which joints should be considered for the IK
             - allow_random_restart: The IK will restart from random configurations if it fails to converge. This can be
                 disabled by setting this to False.
             - ignore_self_collision: If True, the IK will ignore self-collisions
             - method: The scipy minimize method to be used. Defaults to 'L-BFGS-B'
+            - ftol: The tolerance for the cost function, i.e. the algorithm will stop if the cost function changes less
+                than this amount between iterations. Defaults to 1e-8.
         :return: A tuple of q_solution [np.ndarray], success [boolean]. If success is False, q_solution is the
-            configuration with minimal self._ik_cost_function amongst all seen in between iterations if this method.
+            configuration with minimal IK cost amongst all seen in between iterations if this method.
         """
         if 'tolerance' in kwargs:
             raise ValueError("The pose needs to be tolerated - providing an extra tolerance is deprecated.")
 
         if 'joint_mask' in kwargs:
             if q_init is None:
                 raise ValueError("If you provide a joint mask, you need to provide a q_init as well.")
@@ -358,25 +386,25 @@
 
         def _unmask(q_partial):
             q_ik = q_start
             q_ik[joint_mask] = q_partial
             return q_ik
 
         def _cost(_q: np.ndarray):
-            return self._ik_cost_function(_unmask(_q), eef_pose.nominal)
+            return ik_cost_function(self, _unmask(_q), eef_pose.nominal)
 
         lowest_cost = kwargs.get('lowest_cost', IntermediateIkResult(_unmask(q_masked), _cost(q_masked)))
 
         bounds = optimize.Bounds(self.joint_limits[0, joint_mask], self.joint_limits[1, joint_mask])
         sol = optimize.minimize(
             _cost,
             q_masked,
             method=kwargs.get('method', 'L-BFGS-B'),
             bounds=bounds,
-            options={'maxiter': max_iter, 'ftol': 1e-12}
+            options={'maxiter': max_iter, 'ftol': kwargs.get('ftol', 1e-8)}
         )
 
         q_sol = _unmask(sol.x)
         if sol.fun < lowest_cost.distance:
             lowest_cost = IntermediateIkResult(q_sol, sol.fun)
 
         if restore_config:
@@ -617,24 +645,14 @@
 
         :return: Array (ddx, ddy, ddz, dd_alpha, dd_beta, dd_gamma) / dt
         """
         reference = pin.ReferenceFrame.WORLD
         return pin.getFrameAcceleration(self.model, self.data, self.tcp, reference).np
 
     # ---------- Utilities and Dynamic and Kinematics Methods ----------
-    def _ik_cost_function(self, q: np.ndarray, goal: Transformation) -> float:
-        """A custom cost function to evaluate the quality of an inverse kinematic solution."""
-        current = self.fk(q, kind='tcp')
-        translation_error = current.distance(goal).translation_euclidean
-        rotation_error = current.distance(goal).rotation_angle
-        translation_weight = 1.
-        rotation_weight = .5 / np.pi  # .5 meter displacement ~ 180 degree orientation error
-        return (translation_weight * translation_error + rotation_weight * rotation_error) / \
-            (translation_weight + rotation_weight)
-
     def _update_geometry_placement(self):
         """Updates the collision (for collision detection) and visual (for plotting) geometry placements."""
         self._update_collision_placement()
         self._update_visual_placement()
 
     def _update_kinematic(self):
         """Can be called after changing the robot structure. This method updates the kinematic model of the robot"""
@@ -643,14 +661,26 @@
         self.update_configuration(self.configuration)  # Add new joint with q=0
 
     def friction(self, dq: np.ndarray) -> np.ndarray:
         """Computes the forces due to friction"""
         # sin(atan( )) is smooth signum function
         return self.model.damping * dq + self.model.friction * np.sin(np.arctan(100 * dq))
 
+    def manipulability_index(self, q: Optional[np.ndarray] = None) -> float:
+        """
+        Calculate the Yoshikawa manipulability index at joint position q or current one.
+
+        :param q: Joint position to calculate at (default current robot configuration)
+        """
+        if q is None:
+            q = self.configuration
+
+        J = pin.computeJointJacobian(self.model, self.data, q, self.model.frames[self.tcp].parent)
+        return np.sqrt(np.linalg.det(J @ J.T))
+
     def motor_inertias(self, ddq: np.ndarray) -> np.ndarray:
         """Computes the motor inertias in the joins at a given acceleration"""
         return ddq * np.power(self.model.rotorGearRatio, 2) * self.model.rotorInertia
 
     def fk(self, configuration: np.array = None, kind: str = 'tcp', collision: bool = False, visual: bool = False):
         """
         Calculate the forward kinematics (joint state -> end-effector position).
@@ -873,15 +903,15 @@
             return self.ik_jacobian(eef_pose, new_init, gain, damp, iter_left, kind, **kwargs)
 
         while not eef_pose.valid(self.fk(q)):
             joint_current = self.data.oMi[joint_idx_pin]
             diff = joint_current.actInv(joint_desired)
             error_twist = pin.log(diff).vector
             abs_translational_distance = np.linalg.norm(diff.translation)
-            if abs_translational_distance < closest_translation.distance  \
+            if abs_translational_distance < closest_translation.distance \
                     and self.q_in_joint_limits(q) \
                     and not self.has_self_collision(q):
                 closest_translation = IntermediateIkResult(q, abs_translational_distance)
             J = pin.computeJointJacobian(self.model, self.data, q, joint_idx_pin)
             try:
                 if kind == 'damped_ls_inverse':
                     q_dot = np.linalg.lstsq(J, error_twist, rcond=damp)[0]  # Damped least squares
@@ -973,15 +1003,15 @@
             vos = spatial.frame2geom(i, self.visual)
             for co in cos:
                 co.placement = displacement * co.placement
             for vo in vos:
                 vo.placement = displacement * vo.placement
             frame.placement = displacement * frame.placement
         self.model.jointPlacements[0] = displacement * self.model.jointPlacements[0]
-        for i in range(1, self.njoints):
+        for i in range(1, self.njoints + 1):
             # Move all joints that are directly connected to "world" (i.e. the first joint[s])
             if self.model.parents[i] != 0:
                 continue
             try:
                 self.model.jointPlacements[i] = displacement * self.model.jointPlacements[i]
             except IndexError:
                 assert self.njoints == 0, "Could not find the first joint, but there seems to be one"
```

### Comparing `timor-python-0.0.8/src/timor/Volume.py` & `timor-python-0.0.9/src/timor/Volume.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor/configuration_search/AssemblyFilter.py` & `timor-python-0.0.9/src/timor/configuration_search/AssemblyFilter.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,18 +63,20 @@
 
     This enum goes hand-in-hand with the IntermediateResults dataclass. It defines the communication interfaces
     between various RobotFilters: Each one has some dependencies and fills one or more fields of an intermediate result.
     The ResultType is the proper way to define, 'which' fields a filter works with.
     Also, it provides some handy aliases.
     """
 
-    q_goal_pose = 0
-    tau_static = 1
-    trajectory = 2
-    robot = 3
+    robot = 0
+    goal_ik_success = 1
+    q_goal_pose = 2
+    tau_static = 3
+    collision_free_goal = 4
+    trajectory = 5
 
 
 @dataclass
 class IntermediateFilterResults:
     """
     Keeps track of intermediate results for a assembly.
 
@@ -87,14 +89,18 @@
     tau_static: EternalResult[str, float] = field(default_factory=lambda: EternalResult())
     # Maps a tuple of (first_goal, second_goal)-ID to a trajectory combining them
     #   or maps a Follow-goal id on a trajectory
     trajectory: EternalResult[Union[Tuple[str, str], str], Trajectory] = \
         field(default_factory=lambda: EternalResult())
     # RobotBase object created
     robot: RobotBase = field(default=None, repr=False)
+    # Maps a goal ID to success in solving inverse kinematics for that goal
+    goal_ik_success: EternalResult[str, bool] = field(default_factory=lambda: EternalResult())
+    # Maps a goal ID to avoiding obstacle collisions for a previously computed q_goal_pose
+    collision_free_goal: EternalResult[str, bool] = field(default_factory=lambda: EternalResult())
 
     _filters_validated: List[AssemblyFilter] = field(default_factory=lambda: list(), repr=False)
     __allow_overwriting: bool = field(default=None, repr=False)
 
     def allow_changes(self):
         """
         To be used in a context manager. Temporarily sets __allow_overwriting to True.
@@ -182,15 +188,16 @@
 
         :param skip_not_applicable: If false, the filter raises an Exception when called on a solution it cannot filter.
         """
         self.skip_not_applicable = skip_not_applicable
         self._passed: int = 0
         self._failed: int = 0
 
-    def check(self, assembly: ModuleAssembly, task: Task.Task, results: IntermediateFilterResults) -> bool:
+    def check(self, assembly: ModuleAssembly, task: Task.Task, results: IntermediateFilterResults,
+              stop_early: bool = True) -> bool:
         """
         The default use of a AssemblyFilter.
 
         Instantiate your filter, then you can do:
 
         .. code-block:: python
 
@@ -201,19 +208,21 @@
 
         All intermediate results obtained when checking will be stored
 
         :param assembly: A assembly to be checked
         :param task: The task that should be solved by the assembly
         :param results: An intermediate results object with previous calculations. New calcualtions by this filter will
           be added to this object.
+        :param stop_early: Whether to stop check call on first error, e.g. failing goal, or try to apply it to all goals
+          individually such that result returns best effort eventhough filter failed.
         :returns: True if the assembly is possible valid. False iff the assembly is certainly not valid.
         :raises: FilterNotApplicableException
         """
         if any(self._applies(goal) for goal in task.goals):
-            passes = self._check(assembly, task, results)
+            passes = self._check(assembly, task, results, stop_early)
         elif len(task.goals) == 0:
             passes = True
         else:  # The filter is not applicable to the solution
             if self.skip_not_applicable:
                 passes = True
             else:
                 raise FilterNotApplicableException(f"{self.__class__.__name__} not applicable on "
@@ -264,27 +273,29 @@
         try:
             goal_type in self.goal_types_filtered
         except TypeError:
             # This is the case when goal_types_filtered is of UnionType (which cannot be checked prior to python 3.10)
             return goal_type in self.goal_types_filtered.__args__
 
     @abstractmethod
-    def _check(self, assembly: ModuleAssembly, task: Task.Task, results: IntermediateFilterResults) -> bool:
+    def _check(self, assembly: ModuleAssembly, task: Task.Task, results: IntermediateFilterResults,
+               stop_early: bool = True) -> bool:
         """
         The logic of the filter. Returns False if the assembly fails, true else. Used only be self.check
         """
 
 
 class RobotCreationFilter(AssemblyFilter):
     """Filter to explicitly create a robot object for a given assembly."""
 
     provides = (ResultType.robot,)
     requires = ()
 
-    def _check(self, assembly: ModuleAssembly, task: Task.Task, results: IntermediateFilterResults) -> bool:
+    def _check(self, assembly: ModuleAssembly, task: Task.Task, results: IntermediateFilterResults,
+               stop_early: bool = True) -> bool:
         """Turns assembly into a robot and stores it in the intermediate results."""
         results.robot = assembly.robot
         return True
 
     def _applies(self, goal: Goals.GoalBase) -> bool:
         """Robot can be created for any goal"""
         return True
@@ -298,104 +309,138 @@
 
         :param use_intermediate_results: If false, intermediate results are not read from during a check. They will be
           written to, though.
         """
         super().__init__(skip_not_applicable)
         self.use_intermediate_results: bool = use_intermediate_results
 
-    def _check(self, assembly: ModuleAssembly, task: Task.Task, results: IntermediateFilterResults) -> bool:
+    def _check(self, assembly: ModuleAssembly, task: Task.Task, results: IntermediateFilterResults,
+               stop_early: bool = True) -> bool:
         """Perform a validity check on all goals in sequence and interrupts if one fails.
 
         Takes over the looping and separation of goals that are already solved and just need to be checked
         and those that need some more calculation.
         """
+        valid = True
         for goal in self.goals_applicable(task):
             valid = True
             if self.use_intermediate_results \
                     and len(self.provides) > 0 \
                     and all(goal.id in results.__getattribute__(provided.name) for provided in self.provides):
                 # In this case, it is sufficient to check already existing intermediate results
-                valid &= self._check_given(assembly, goal, results)
+                valid &= self._check_given(assembly, goal, results, task)
             else:
-                valid &= self._check_goal(assembly, goal, results)
-            if not valid:
+                valid &= self._check_goal(assembly, goal, results, task)
+            if not valid and stop_early:
                 return False
-        return True
+        return valid
 
     @abstractmethod
-    def _check_given(self, assembly: ModuleAssembly, goal: Goals.GoalBase, results: IntermediateFilterResults):
+    def _check_given(self, assembly: ModuleAssembly, goal: Goals.GoalBase,
+                     results: IntermediateFilterResults, task: Task):
         """Checks a predefined solution.
 
         Called when all required calculations for this filter already have been done: In this case, check if they
         are valid only.
         """
 
     @abstractmethod
-    def _check_goal(self, assembly: ModuleAssembly, goal: Goals.GoalBase, results: IntermediateFilterResults):
+    def _check_goal(self, assembly: ModuleAssembly, goal: Goals.GoalBase,
+                    results: IntermediateFilterResults, task: Task):
         """The same logic as _check, but performed on a single goal that this filter can work with."""
 
 
 class InverseKinematicsSolvable(GoalByGoalFilter):
     """
     Checks whether all goal poses can be theoretically reached by the assembly without colliding with itself.
 
     Does not check for collisions with the environment.
     Does only work with goals that have one pose at most. Filtering assemblies based on target trajectories needs to be
     done within another class.
+
+    :note: Can be used to also verify freedom of collision by setting ik_kwargs to the task to check collisions with
     """
 
     requires: Tuple[ResultType] = (ResultType.robot,)
-    provides: Tuple[ResultType] = (ResultType.q_goal_pose,)
+    provides: Tuple[ResultType] = (ResultType.q_goal_pose, ResultType.goal_ik_success)
     goal_types_filtered: Collection[Type[Goals.GoalBase]] = GOALS_WITH_POSE
 
     def __init__(self, skip_not_applicable: bool = True, **ik_kwargs):
         """Initialize the filter on inverse kinematics
 
         :param ik_kwargs: Keyword arguments to be passed to the :func:`inverse kinematics solver <timor.Robot.Robot.ik>`
         """
         self.kwargs: Dict[str, any] = ik_kwargs
+        if 'task' in self.kwargs:
+            self.provides += (ResultType.collision_free_goal,)
+        if self.kwargs.get('check_static_torques', False):
+            self.provides += (ResultType.tau_static,)
         super().__init__(skip_not_applicable)
 
-    def _check_given(self, assembly: ModuleAssembly, goal: Goals.GoalBase, results: IntermediateFilterResults):
+    @property
+    def ensures_static_torques(self) -> bool:
+        """Does this filter ensure that static torques are respected?"""
+        return self.kwargs.get('check_static_torques', False)
+
+    @property
+    def ensures_collision_free_goal(self) -> bool:
+        """Does this filter ensure collision-freedom with respect to a task's scene?"""
+        return 'task' in self.kwargs
+
+    def _check_given(self, assembly: ModuleAssembly, goal: Goals.GoalBase, results: IntermediateFilterResults,
+                     task: Task):
         """Just checks that the goal pose is reached without self collisions"""
         if not self._applies_to_type(type(goal)):
             return True  # Not applicable, so filter is not invalid
         is_pose = results.robot.fk(results.q_goal_pose[goal.id])
         passes = goal.goal_pose.valid(is_pose) and not results.robot.has_self_collision()
-        if 'task' in self.kwargs:
+        if self.ensures_collision_free_goal:
             passes &= not results.robot.has_collisions(self.kwargs['task'])
+        if self.ensures_static_torques:
+            tau = results.robot.static_torque(results.q_goal_pose[goal.id])
+            passes &= (np.abs(tau) <= results.robot.joint_torque_limits).all()
         return passes
 
-    def _check_goal(self, assembly: ModuleAssembly, goal: GOALS_WITH_POSE, results: IntermediateFilterResults) -> bool:
+    def _check_goal(self, assembly: ModuleAssembly, goal: GOALS_WITH_POSE, results: IntermediateFilterResults,
+                    task: Task) -> bool:
         """Performs the check whether the goals are valid.
 
         Assemblies pass if and only if, for all goal poses, a self-collision free inverse kinematics solution can be
         found. Writes an inverse kinematics solution for the goal pose to the goal, if it finds one.
         """
         q, valid = results.robot.ik(goal.goal_pose, **self.kwargs.copy())
         results.q_goal_pose[goal.id] = q
+        results.goal_ik_success[goal.id] = valid
+        if self.ensures_static_torques:
+            results.tau_static[goal.id] = valid or (np.abs(results.robot.static_torque(results.q_goal_pose[goal.id]))
+                                                    <= results.robot.joint_torque_limits).all()
+        if self.ensures_collision_free_goal:
+            results.robot.update_configuration(q)
+            results.collision_free_goal[goal.id] = valid or not results.robot.has_collisions(self.kwargs['task'])
         return valid
 
 
 class StaticTorquesValid(GoalByGoalFilter):
     """
     Checks whether the static torques for assembly joints in a certain configuration are within the torque limits.
 
     Currently, operates without static forces ==> gravity only.
     """
 
     requires: Tuple[ResultType] = (ResultType.q_goal_pose, ResultType.robot)
     provides: Tuple[ResultType] = (ResultType.tau_static,)
     goal_types_filtered: Collection[Type[Goals.GoalBase]] = GOALS_WITH_POSE
 
-    def _check_given(self, assembly: ModuleAssembly, goal: Goals.GoalBase, results: IntermediateFilterResults):
+    def _check_given(self, assembly: ModuleAssembly, goal: Goals.GoalBase, results: IntermediateFilterResults,
+                     task: Task):
         tau = results.tau_static[goal.id]
         return (np.abs(tau) <= results.robot.joint_torque_limits).all()
 
-    def _check_goal(self, assembly: ModuleAssembly, goal: Goals.GoalBase, results: IntermediateFilterResults):
+    def _check_goal(self, assembly: ModuleAssembly, goal: Goals.GoalBase, results: IntermediateFilterResults,
+                    task: Task):
         """Calculates static torques in a goal position and compares them to the robot assembly limits.
 
         Writes the static torques to the intermediate results.
         """
         q = results.q_goal_pose[goal.id]
         results.robot.update_configuration(q)
         tau = results.robot.static_torque(q)
@@ -408,29 +453,30 @@
     Checks whether a assembly's joint (position, velocity) and the torque limits are held for a trajectory.
     """
 
     requires: Tuple[ResultType] = (ResultType.trajectory, ResultType.robot)
     provides: Tuple[ResultType] = ()
     goal_types_filtered: Collection[Type[Goals.GoalBase]] = tuple()  # TODO: Implement trajectory goals
 
-    def _check(self, assembly: ModuleAssembly, task: Task.Task, results: IntermediateFilterResults) -> bool:
+    def _check(self, assembly: ModuleAssembly, task: Task.Task, results: IntermediateFilterResults,
+               stop_early: bool = True) -> bool:
         """Performs the check whether the joint limits are met.
 
         Returns true if and only if joint limits, velocity limits and torque limits are held for all trajectories in
         the intermediate results.
         """
         # TODO: Access necessary trajectories from goals and then check if they are in the results
         valid = True
         for trajectory in results.trajectory.values():
             q, dq, ddq = trajectory.q, trajectory.dq, trajectory.ddq
             q_valid = results.robot.q_in_joint_limits(q)
             dq_valid = np.all(np.abs(dq) <= results.robot.joint_velocity_limits)
             ddq_valid = np.all(np.abs(ddq) <= results.robot.joint_acceleration_limits)
             valid = valid and q_valid and dq_valid and ddq_valid
-            if not valid:
+            if not valid and stop_early:
                 return False
 
             tau = np.vstack([results.robot.id(p, v, a) for p, v, a in zip(q, dq, ddq)])
             valid = valid and (np.abs(tau) < results.robot.joint_torque_limits).all()
 
         return valid
```

### Comparing `timor-python-0.0.8/src/timor/configuration_search/AssemblyIterator.py` & `timor-python-0.0.9/src/timor/configuration_search/AssemblyIterator.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor/configuration_search/LiuIterator.py` & `timor-python-0.0.9/src/timor/configuration_search/LiuIterator.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor/parameterized.py` & `timor-python-0.0.9/src/timor/parameterized.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,26 @@
         """The inertia needs to be dynamically calculated, depending on the geometry."""
 
     def __copy__(self):
         """Parameterizable bodies are actually quite easy to copy as geometries are calculated on-the-fly."""
         return self.__class__(self._id, self.parameters, self.parameter_limits, self.mass_density, in_module=None,
                               connectors=[copy.copy(con) for con in self.connectors])
 
+    def __eq__(self, other):
+        """Parameterizable body equality is given by the original parameters - no need to compute the geometry."""
+        if not isinstance(other, ParameterizableBody):
+            return NotImplemented
+        this_attributes = (self._id, tuple(self.parameters), self.mass_density, self._geometry_transformation)
+        other_attributes = (other._id, tuple(other.parameters), other.mass_density, other._geometry_transformation)
+        return this_attributes == other_attributes
+
+    def __hash__(self):
+        """Hashing is equal to hashes of regular bodies - ID should be unique."""
+        return super().__hash__()
+
     def __getstate__(self):
         """For parameterized bodies, we can rely on the python builtin actually"""
         return self.__dict__
 
     def __setstate__(self, state):
         """For parameterized bodies, we can rely on the python builtin actually"""
         self.__dict__ = state
```

### Comparing `timor-python-0.0.8/src/timor/task/Constraints.py` & `timor-python-0.0.9/src/timor/task/Constraints.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class ConstraintBase(ABC, JSONable_mixin):
     """Base class defining the interface all Constraints must implement."""
 
     global_only: bool = False  # If this is True, the constraint cannot be used as a local goal constraint.
 
     @classmethod
-    def from_json_data(cls, d: Dict[str, Any]) -> ConstraintBase:
+    def from_json_data(cls, d: Dict[str, Any], *args, **kwargs) -> ConstraintBase:
         """
         Converts a description (string, parsed from json) to a constraint
 
         :param d: A description, mapping a constraint name to one or more constraint specifications
         """
         try:
             constraint_type = d.pop('type')
@@ -78,26 +78,37 @@
         """Main access point to check constraints"""
         pass
 
     @abstractmethod
     def to_json_data(self) -> Dict[str, any]:
         """Should be implemented to convert the constraint to a json-serializable dictionary"""
 
+    @property
+    @abstractmethod
+    def _equality_parameters(self) -> Tuple[any, ...]:
+        """Returns the parameters that should be used to check equality of constraints"""
+
     def visualize(self, viz: pinocchio.visualize.MeshcatVisualizer, scale: float = 1.) -> None:
         """Visualize the constraint in an existing meshcat window.
 
         If possible a constraint should have a visualization. The default is no visualization and should be overwritten
         if a visualization is possible.
 
         :param viz: A meshcat visualizer as defined in pinocchio
         :param scale: The visualization method assumes the robot size is ~1-2m maximum reach. Use the scale factor
             to adapt for significantly different sizes of robots and/or obstacles.
         """
         pass
 
+    def __eq__(self, other):
+        """Checks if two constraints are equal"""
+        if type(self) is not type(other):
+            return NotImplemented
+        return self._equality_parameters == other._equality_parameters
+
 
 class AlwaysTrueConstraint(ConstraintBase):
     """
     This constraint is always true and can be used for constraints ensured by the software library before evaluation.
     """
 
     def is_valid_until(self, solution: Solution.SolutionBase, t: float) -> bool:
@@ -109,14 +120,19 @@
         return True
 
     def to_json_data(self) -> Dict[str, any]:
         """Dumps this constraint to a dictionary"""
         logging.info("Always true constraint is skipped during serialization")
         return {}
 
+    @property
+    def _equality_parameters(self) -> Tuple[any, ...]:
+        """Two always true constraints are always equal"""
+        return tuple()
+
 
 class GoalsBySameRobot(ConstraintBase):
     """Checks that all goals specified were achieved by the same robot."""
 
     global_only = True
 
     def __init__(self, goals: Iterable[str]):
@@ -145,14 +161,19 @@
     def to_json_data(self) -> Dict[str, any]:
         """Dumps this constraint to a dictionary"""
         return {
             'type': 'goalsBySameRobot',
             'goals': list(self.goals)
         }
 
+    @property
+    def _equality_parameters(self) -> Tuple[str, ...]:
+        """Same goals, same constraint"""
+        return tuple(sorted(self.goals, key=lambda g: g.id))
+
 
 class GoalOrderConstraint(ConstraintBase):
     """Checks that the goals in the task are fulfilled in the right order."""
 
     global_only = True
 
     def __init__(self, order: Iterable[str]):
@@ -175,14 +196,19 @@
     def to_json_data(self) -> Dict[str, any]:
         """Dumps this constraint to a dictionary"""
         return {
             'type': 'allGoalsFulfilledInOrder',
             'order': self.order
         }
 
+    @property
+    def _equality_parameters(self) -> Tuple[str, ...]:
+        """Same order, same constraint"""
+        return tuple(self.order)
+
 
 class AllGoalsFulfilled(ConstraintBase):
     """Checks whether all goals are fulfilled"""
 
     global_only = True
 
     def is_valid_until(self, solution: Solution.SolutionBase, t: float) -> bool:
@@ -193,14 +219,19 @@
         """Check if all goals are fulfilled by this solution."""
         return all(g.achieved(solution) for g in solution.task.goals)
 
     def to_json_data(self) -> Dict[str, any]:
         """Return json-able dict of this constraint."""
         return {'type': 'allGoalsFulfilled'}
 
+    @property
+    def _equality_parameters(self) -> Tuple[any, ...]:
+        """All goals, same constraint"""
+        return tuple()
+
 
 class JointLimits(ConstraintBase):
     """Holds constraints on the robots (hardware) limits like position, velocity, torques, etc."""
 
     robot_limit_types = ('q', 'dq', 'ddq', 'tau')
     _robot_attributs = ('joint_limits', 'joint_velocity_limits', 'joint_acceleration_limits', 'joint_torque_limits')
 
@@ -249,14 +280,19 @@
     def to_json_data(self) -> Dict[str, any]:
         """Dumps this constraint to a dictionary"""
         return {
             'type': 'joint',
             'parts': [kind for kind in self.robot_limit_types if getattr(self, kind)]
         }
 
+    @property
+    def _equality_parameters(self) -> Tuple[str, ...]:
+        """Same parts, same constraint"""
+        return tuple(kind for kind in self.robot_limit_types if getattr(self, kind))
+
 
 class BasePlacement(ConstraintBase):
     """Constraint on the placement of the base coordinate system."""
 
     global_only = True  # If this should be used for mobile bases at any point, set global_only to False
 
     def __init__(self, base_pose: ToleratedPose):
@@ -319,14 +355,19 @@
             "pose": self.base_pose.to_json_data()
         }
 
     def visualize(self, viz: pinocchio.visualize.MeshcatVisualizer, scale: float = 1.) -> None:
         """Visualize the constraint"""
         self.base_pose.visualize(viz, scale=scale, name="base_constraint")
 
+    @property
+    def _equality_parameters(self) -> Tuple[ToleratedPose]:
+        """Equal if the placements are equal"""
+        return (self.base_pose,)
+
 
 class CoterminalJointAngles(ConstraintBase):
     """Constrains a robot can reach a certain pose, being ignorant about full circle rotation deviations
 
     This constraint checks whether given joint position, given by joint angles, can be reached in general.
     It does not check for the exact joint angles but for their coterminal counterpart in the range [-pi, pi)
     """
@@ -365,14 +406,19 @@
         """Checks whether the given joint angles are within the defined limits in the solution."""
         return all(self._validate(q) for q in solution.q)
 
     def to_json_data(self) -> Dict[str, any]:
         """Dumps this constraint to a dictionary"""
         raise NotImplementedError("Coterminal Joint Angles not yet available.")
 
+    @property
+    def _equality_parameters(self) -> Tuple[float, ...]:
+        """Flatten the limits to a 1d array"""
+        return tuple(self.limits.flatten())
+
 
 class JointAngles(CoterminalJointAngles):
     """This is a stronger constraint than coterminal joint angles, verifying exact angles against joint limits."""
 
     def __init__(self, limits: np.ndarray):
         """
         limits: A 2xdof array of joint limits: [[upper_limits], [lower_limimts]]
@@ -402,14 +448,19 @@
         """Evaluates the whole solution for collision-freeness."""
         return all(self.is_valid_until(solution, t) for t in solution.time_steps)
 
     def to_json_data(self) -> Dict:
         """Dumps this constraint to a dictionary"""
         return {'type': 'collisionFree'}
 
+    @property
+    def _equality_parameters(self) -> Tuple[any, ...]:
+        """Collision-free is equal to itself"""
+        return ()
+
 
 class SelfCollisionFree(CollisionFree):
     """A constraint that checks whether the robot is in collision with itself."""
 
     def is_valid_until(self, solution: Solution.SolutionBase, t: float) -> bool:
         """Checks whether the robot is in collision with itself at time t."""
         q = solution.q[solution.get_time_id(t)]
@@ -434,17 +485,18 @@
 
         :param pose: tolerated pose to keep within (either initialized or serialized in dict)
         :param velocity_lim: Minimal / Maximal translation velocity :math:`v` of the end-effector in
           :math:`\frac{m}{s}`; defaults to any allowed
         :param rotation_velocity_lim: Minimal / Maximal rotation velocity :math:`\omega` of the end-effector in
           :math:`\frac{rad}{s}`; defaults to any allowed
         """
-        self.pose = pose
-        self.velocity_lim = self.default_velocity_limits.copy() if velocity_lim is None else velocity_lim
-        self.rotation_velocity_lim = self.default_velocity_limits.copy() \
+        self.pose: Optional[ToleratedPose] = pose
+        self.velocity_lim: Optional[np.ndarray] = self.default_velocity_limits.copy() \
+            if velocity_lim is None else velocity_lim
+        self.rotation_velocity_lim: Optional[np.ndarray] = self.default_velocity_limits.copy() \
             if rotation_velocity_lim is None else rotation_velocity_lim
         if self.velocity_lim[0] > self.velocity_lim[1] or self.rotation_velocity_lim[0] > self.rotation_velocity_lim[1]:
             logging.warning("velocity_lim_min > velocity_lim_max or "
                             "rotation_velocity_lim_min > rotation_velocity_lim_max; "
                             "eef_constraint will always be invalid.")
 
     @classmethod
@@ -482,7 +534,12 @@
         for k, v in (('v_min', self.velocity_lim[0]), ('v_max', self.velocity_lim[1]),
                      ('o_min', self.rotation_velocity_lim[0]), ('o_max', self.rotation_velocity_lim[1])):
             if abs(v) < math.inf:
                 data[k] = v
         if self.pose is not None:
             data['pose'] = self.pose.to_json_data()
         return data
+
+    @property
+    def _equality_parameters(self) -> Tuple[any, ...]:
+        """End-effector constraints are equal if they have the same pose and limits"""
+        return (self.pose,) + tuple(self.velocity_lim.flat) + tuple(self.rotation_velocity_lim.flat)
```

### Comparing `timor-python-0.0.8/src/timor/task/CostFunctions.py` & `timor-python-0.0.9/src/timor/task/CostFunctions.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor/task/Goals.py` & `timor-python-0.0.9/src/timor/task/Goals.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     @abstractmethod
     def _achieved(self, solution: task.Solution.SolutionBase, t_goal: float, idx_goal: int) -> bool:
         """Needs to be implemented by children according to the goal"""
         pass
 
     @classmethod
     @abstractmethod
-    def from_json_data(cls, d: Dict[str, any]):
+    def from_json_data(cls, d: Dict[str, any], *args, **kwargs):
         """Deserializes a goal from a dictionary"""
 
     @abstractmethod
     def to_json_data(self) -> Dict[str, any]:
         """
         Returns a json-compatible dictionary representation of the goal.
         """
@@ -138,14 +138,22 @@
             id_goal = solution.get_time_id(t_goal)
         except TimeNotFoundError:
             raise TimeNotFoundError(f"Goal {self.id} seems to be achieved at t={t_goal}, "
                                     f"but could not find it in the {solution.__class__.__name__}'s time array.")
 
         return t_goal, id_goal
 
+    def __eq__(self, other):
+        """Enforce the implementation"""
+        raise NotImplementedError(f"Equality of {self.__class__.__name__} objects is not implemented.")
+
+    def __hash__(self):
+        """Hashes the goal by its id"""
+        return hash(self.id)
+
 
 class GoalWithDuration(GoalBase, ABC):
     """
     Any goal that needs to test more than a single time-step to be achieved.
 
     This also includes checking the goal constraints at any point of the goal's duration.
     """
@@ -212,15 +220,15 @@
         self.goal_pose: ToleratedPose = goalPose
 
     def visualize(self, viz: MeshcatVisualizer, scale: float = .33, show_name: bool = False) -> None:
         """Shows an error pointing towards the desired position"""
         self.goal_pose.visualize(viz, scale=scale, name=f"goal_{self.id}", text=f"Goal {self.id}" * show_name)
 
     @classmethod
-    def from_json_data(cls, d: Dict[str, any]):
+    def from_json_data(cls, d: Dict[str, any], *args, **kwargs):
         """Loads the At goal to a dictionary description."""
         return cls(
             ID=d['ID'],
             goalPose=ToleratedPose.from_json_data(d['goalPose']),
             constraints=[Constraints.ConstraintBase.from_json_data(c) for c in d.get('constraints', [])]
         )
 
@@ -244,14 +252,20 @@
 
         :param solution: Any solution instance that must contain a time at which this goal was solved
         :return: True if the end effector placement at time t is within the defined tolerances for the desired pose
         """
         is_pose = solution.tcp_pose_at(t_goal)
         return self.goal_pose.valid(is_pose)
 
+    def __eq__(self, other):
+        """At goals are same if they have the same constraints and desired pose"""
+        if not isinstance(other, At):
+            return False
+        return self.constraints == other.constraints and self.goal_pose == other.goal_pose
+
 
 class Reach(At):
     """A goal that is achieved when the robot is at a certain position for at least one time step at zero velocity"""
 
     def __init__(self,
                  ID: str,
                  goalPose: ToleratedPose,
@@ -266,15 +280,15 @@
         :param velocity_tolerance: Defines the velocity tolerance for v_desired.
         :param constraints: A list of constraints that need to be satisfied for the goal to be achieved.
         """
         super().__init__(ID, goalPose, constraints)
         self.velocity_tolerance = velocity_tolerance
 
     @classmethod
-    def from_json_data(cls, d: Dict[str, any]):
+    def from_json_data(cls, d: Dict[str, any], *args, **kwargs):
         """Loads the Reach goal to a dictionary description."""
         return cls(
             ID=d['ID'],
             goalPose=ToleratedPose.from_json_data(d['goalPose']),
             velocity_tolerance=Tolerance.Abs6dPoseTolerance.default(),
             constraints=[Constraints.ConstraintBase.from_json_data(c) for c in d.get('constraints', [])]
         )
@@ -294,14 +308,20 @@
         """
         at_achieved = super()._achieved(solution, t_goal, idx_goal)
         if not at_achieved:
             return False
         is_velocity = solution.tcp_velocity_at(t_goal)
         return at_achieved and self.velocity_tolerance.valid(np.zeros(is_velocity.shape), is_velocity)
 
+    def __eq__(self, other):
+        """Reach goals are same if they have the same constraints, velocity, and desired pose"""
+        if not isinstance(other, Reach):
+            return NotImplemented
+        return super().__eq__(other) and self.velocity_tolerance == other.velocity_tolerance
+
 
 class ReturnTo(GoalBase):
     """This goal is achieved when the robot returns to the state it was in at a previous goal"""
 
     def __init__(self,
                  ID: str,
                  returnToGoal: Optional[str] = None,
@@ -318,15 +338,15 @@
         """
         super().__init__(ID, constraints)
         self.return_to_goal = returnToGoal
         self.distance_tolerance = Tolerance.VectorDistance(epsilon, order=2)
         self.desired_pose: Optional[ToleratedPose] = None
 
     @classmethod
-    def from_json_data(cls, d: Dict[str, any]):
+    def from_json_data(cls, d: Dict[str, any], *args, **kwargs):
         """Loads the Return goal to a dictionary description."""
         return cls(
             ID=d['ID'],
             returnToGoal=d.get('returnToGoal', None),
             constraints=[Constraints.ConstraintBase.from_json_data(c) for c in d.get('constraints', [])]
         )
 
@@ -358,14 +378,22 @@
         is_velocity = solution.dq[goal_idx]
         is_acceleration = solution.ddq[goal_idx]
 
         return (self.distance_tolerance.valid(desired_position, is_position)
                 and self.distance_tolerance.valid(desired_velocity, is_velocity)
                 and self.distance_tolerance.valid(desired_acceleration, is_acceleration))
 
+    def __eq__(self, other):
+        """Return goals are same if they have the same constraints, tolerance, and return to option"""
+        if not isinstance(other, ReturnTo):
+            return NotImplemented
+        return self.constraints == other.constraints \
+            and self.distance_tolerance == other.distance_tolerance \
+            and self.return_to_goal == other.return_to_goal
+
 
 class Pause(GoalWithDuration):
     """
     This goal is achieved if the robot does not move for a preconfigured duration.
     """
 
     epsilon: float = 1e-9  # Precision error: Pause is allowed to be epsilon shorter than self._duration
@@ -376,15 +404,15 @@
 
     @property
     def duration(self) -> float:
         """Getter for explicit duration of Pause Goal."""
         return self._duration
 
     @classmethod
-    def from_json_data(cls, d: Dict[str, any]):
+    def from_json_data(cls, d: Dict[str, any], *args, **kwargs):
         """Loads the Pause goal from a dictionary description."""
         return cls(
             ID=d['ID'],
             duration=d['duration'],
             constraints=[Constraints.ConstraintBase.from_json_data(c) for c in d.get('constraints', [])]
         )
 
@@ -407,14 +435,21 @@
             logging.debug(f"Duration not covered by trajectory; {e}")
             return False
         return all((solution.q[sol_idx[0]] == solution.q[idx]).all()
                    and not solution.dq[idx].any()
                    and not solution.ddq[idx].any()
                    for idx in sol_idx)
 
+    def __eq__(self, other):
+        """Two pause goals are equal if there's (almost) the same pause and constraints."""
+        if not isinstance(other, Pause):
+            return NotImplemented
+        return self.constraints == other.constraints \
+            and abs(self.duration - other.duration) < self.epsilon
+
 
 class Follow(GoalWithDuration):
     """
     This goal is achieved if the robot follows a prescribed end-effector trajectory.
     """
 
     def __init__(self,
@@ -435,15 +470,15 @@
 
     @property
     def trajectory(self) -> Trajectory:
         """The trajectory to follow along"""
         return self._trajectory
 
     @classmethod
-    def from_json_data(cls, d: Dict[str, any]):
+    def from_json_data(cls, d: Dict[str, any], *args, **kwargs):
         """Loads the Follow goal from a dictionary description."""
         return cls(
             ID=d['ID'],
             trajectory=Trajectory.from_json_data(d['trajectory']),
             constraints=[Constraints.ConstraintBase.from_json_data(c) for c in d.get('constraints', [])]
         )
 
@@ -498,7 +533,15 @@
                     idx_goal_start -= 1
                     if idx_goal_start < 0:
                         logging.info(f"Followed trajectory till start; follow was not fulfilled for pose {p}.")
                         self._duration = float('inf')
                         return False
             self._duration = solution.time_steps[idx_goal] - solution.time_steps[idx_goal_start]
             return True
+
+    def __eq__(self, other):
+        """Two follow goals are equal if they have the same duration, trajectory and constraints."""
+        if not isinstance(other, Follow):
+            return NotImplemented
+        return self.constraints == other.constraints \
+            and self._duration == other._duration \
+            and self.trajectory == other.trajectory
```

### Comparing `timor-python-0.0.8/src/timor/task/Obstacle.py` & `timor-python-0.0.9/src/timor/task/Obstacle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 # Author: Jonathan Külz
 # Date: 17.01.22
 from __future__ import annotations
 
-from pathlib import Path
 from typing import Dict, Optional, Union
 
 from hppfcl import hppfcl
 import meshcat.geometry
 import pinocchio as pin
 
 from timor import Geometry
@@ -37,35 +36,31 @@
         """
         self._id = str(ID)
         self.collision = collision
         self._visual = visual
         self.name: Optional[str] = name
 
     @classmethod
-    def from_json_data(cls, d: Dict[str, Union[str, dict]]) -> Obstacle:
+    def from_json_data(cls, d: Dict[str, Union[str, dict]], *args, **kwargs) -> Obstacle:
         """
         Takes a json geometry specification and returns the according Obstacle.
 
         :param d: The serialized obstacle information, containing:
 
             * ID: The obstacle unique ID
             * collision: A Geometry used for collision detection
             * visual: A Geometry for visualization of this Obstacle - defaults to collision if not given
-            * package_dir: If a mesh is given, it is given relative to a package directory that must be specified
             * name: The obstacle display name
         :return: The obstacle class instance that matches the specification
         """
         ID = d['ID']
         collision = d['collision']
-        package_dir = d['package_dir'] if 'package_dir' in d else None
-        if isinstance(package_dir, str):
-            package_dir = Path(package_dir)
-        collision_geometry = Geometry.Geometry.from_json_data(collision, package_dir=package_dir)
+        collision_geometry = Geometry.Geometry.from_json_data(collision)
         if 'visual' in d:
-            visual_geometry = Geometry.Geometry.from_json_data(d['visual'], package_dir=package_dir)
+            visual_geometry = Geometry.Geometry.from_json_data(d['visual'])
         else:
             visual_geometry = None
 
         return cls(ID, collision_geometry, visual_geometry, name=d.get('name', None))
 
     @classmethod
     def from_hppfcl(cls, ID: str, fcl: hppfcl.CollisionObject,
@@ -170,7 +165,17 @@
         if self._visual is None:
             return self.collision
         return self._visual
 
     def __copy__(self):
         """Not supported!"""
         raise NotImplementedError("Cannot shallow-copy hppfcl geometries. Use deepcopy.")
+
+    def __eq__(self, other):
+        """Compare two obstacles by their ID, name, and geometry"""
+        if not isinstance(other, Obstacle):
+            return NotImplemented
+        return self.id == other.id and self.name == other.name and self.collision == other.collision
+
+    def __hash__(self):
+        """The ID is sufficient to hash an obstacle"""
+        return hash(self.id)
```

### Comparing `timor-python-0.0.8/src/timor/task/Solution.py` & `timor-python-0.0.9/src/timor/task/Solution.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 from __future__ import annotations
 
 import abc
+from collections import namedtuple
+from copy import copy
 from dataclasses import dataclass, field
 import datetime
 import json
 from pathlib import Path
-from typing import Dict, List, Tuple, Union
+from typing import Dict, List, Optional, Sequence, Tuple, Union
 import uuid
 
 import jsonschema.exceptions
+from matplotlib import pyplot as plt
 import numpy as np
 import pinocchio as pin
 import scipy.interpolate
 
 from timor.Module import ModuleAssembly
 from timor.Robot import RobotBase
 from timor.task import Constraints, CostFunctions, Goals, Task
@@ -21,15 +24,15 @@
 from timor.utilities.errors import TimeNotFoundError
 from timor.utilities.file_locations import map2path, schema_dir
 from timor.utilities.json_serialization_formatting import compress_json_vectors
 from timor.utilities.jsonable import JSONable_mixin
 from timor.utilities.schema import DEFAULT_DATE_FORMAT, get_schema_validator
 from timor.utilities.trajectory import Trajectory
 from timor.utilities.transformation import Transformation, TransformationLike
-from timor.utilities.visualization import MeshcatVisualizerWithAnimation, animation
+from timor.utilities.visualization import MeshcatVisualizerWithAnimation, animation, plot_time_series
 
 
 @dataclass
 class SolutionHeader(TypedHeader):
     """The header every solution contains"""
 
     taskID: str  # This is NOT the Solution ID, but identifies the task the solution was crafted for!
@@ -82,24 +85,30 @@
         return f"Solution for task {self.header.taskID}"
 
     @classmethod
     @abc.abstractmethod
     def empty(cls) -> SolutionBase:
         """Create an empty solution"""
 
-    @staticmethod
-    def from_json_file(json_path: Union[Path, str], package_dir: Path, tasks: Dict[str, Task.Task]) -> SolutionBase:
+    @classmethod
+    def from_json_file(cls, json_path: Union[Path, str], tasks: Dict[str, Task.Task]) -> SolutionBase:
         """Factory method to load a class instance from a json file."""
         json_path = map2path(json_path)
-        content = json.load(json_path.open('r'))
+        with json_path.open('r') as f:
+            content = json.load(f)
         _, validator = get_schema_validator(schema_dir.joinpath("SolutionSchema.json"))
         try:
             validator.validate(content)
         except jsonschema.exceptions.ValidationError:
             raise ValueError(f"Invalid solution json provided. Details: {tuple(validator.iter_errors(content))}.")
+        return cls.from_json_data(content, tasks)
+
+    @staticmethod
+    def from_json_data(content: Dict, tasks: Dict[str, Task.Task], *args, **kwargs) -> SolutionBase:
+        """Factory method to load a class instance from a dictionary."""
         _header = fuzzy_dict_key_matching(content, desired_only=SolutionHeader.fields())
         header = SolutionHeader(**_header)
         try:
             sol_task = tasks[header.taskID]
         except KeyError:
             raise KeyError(f"Got solution for task {header.ID}, but there is no such task.")
 
@@ -272,14 +281,17 @@
         """
         Visualize a solution trajectory
 
         :param viz: Visualizer to use (default create new)
         :param fps: fps to use for visualization
         :param center_view: Whether to try to set camera such that robot / base pose constraint visible
         """
+        if self.robot.njoints == 0:
+            logging.warning("You tried to visualize a solution for a robot with no joints. Aborting.")
+            return viz
         if self.q.size == 0:
             logging.warning("You tried to visualize a solution with an empty trajectory. Aborting.")
             return viz
 
         if viz is None:
             viz = MeshcatVisualizerWithAnimation()
             viz.initViewer()
@@ -298,14 +310,23 @@
         else:
             q_new = self.q
 
         animation(self.robot, q_new, 1 / fps, visualizer=viz)
 
         return viz
 
+    def __getstate__(self):
+        """State of solution contains json-able part and the associated task object."""
+        return self.to_json_data(), {self.header.taskID: self.task}
+
+    def __setstate__(self, state):
+        """To recreate solution use the state Tuple including the solution json and associated task object."""
+        cpy = self.__class__.from_json_data(*state)
+        self.__dict__ = cpy.__dict__
+
 
 class SolutionTrajectory(SolutionBase):
     """A solution based on a given trajectory (as opposed to a solution based on torques given)"""
 
     def __init__(self,
                  trajectory: Trajectory,
                  header: Union[Dict, SolutionHeader],
@@ -418,14 +439,25 @@
         """Small type check to prevent invalid solutions. Also resets the validity and calculated cost."""
         if not isinstance(t, Trajectory):
             raise TypeError(f"Invalid argument for solution trajectory of type {type(t)}")
         self._valid.value = None
         self._cost.value = None
         self._trajectory = t
 
+    @property
+    def manipulability_indices(self) -> np.ndarray:
+        """Return manipulability index at each time in time_steps."""
+        return np.fromiter((self.robot.manipulability_index(q) for q in self.trajectory.q),
+                           dtype=np.single, count=len(self.trajectory))
+
+    @property
+    def tcp_poses(self) -> Tuple[Transformation, ...]:
+        """Return TCP pose at each time in time_steps."""
+        return tuple(self.tcp_pose_at(t) for t in self.time_steps)
+
     def get_power(self, motor_inertia: bool = True, friction: bool = True):
         """
         Get mechanical power used in all joints for each time step.
 
         :param motor_inertia: Include power needed to overcome motor side inertia.
         :param friction: Include power needed to overcome joint friction.
         :note: If both options enabled this is the mechanical power produced by all motors in the robot; if both options
@@ -448,7 +480,76 @@
 
         :param motor_inertia: Include energy to overcome motor side inertia.
         :param friction: Include energy to overcome joint friction.
         :note: If both options enabled this is the mechanical energy expanded by all motors in the robot to follow this
           solution; if both options are disabled it is the mechanical energy expanded on moving all robot links.
         """
         return np.sum(self.get_power(motor_inertia, friction))
+
+    def plot(self, data: Sequence[str] = ("q", "dq", "ddq"), show_figure: bool = True,
+             subplot_kwargs: Optional[Dict] = None) -> plt.Figure:
+        """
+        Plot time series data about this solution
+
+        :param data: Can be any combination of q, dq, ddq, tau, manipulability, goals, eef_position, eef_rotation
+        :param show_figure: execute pyplot show() function on figure; might need to disable if further figure formating
+          wanted later on; may need to activate text.usetex in the local environment where show is called.
+        :param subplot_kwargs: Kwargs handed to subplots, including pyplot.figure kwargs
+          (see https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html)
+        :return: Figure object containing the desired plots
+        """
+        marker = {}
+        time_series = []
+        legends = []
+        available_series_data = namedtuple("available_series_data", ["time_series", "name", "legend_labels"])
+        available = {
+            "q": available_series_data(
+                time_series=self.q,
+                name="Configuration q",
+                legend_labels=tuple(r"$q_{" + str(i) + "}$" for i in range(self.trajectory.dof))),
+            "dq": available_series_data(
+                time_series=self.dq,
+                name="Joint Velocity dq",
+                legend_labels=tuple(r"$\dot{{q}}_{" + str(i) + "}$" for i in range(self.trajectory.dof))),
+            "ddq": available_series_data(
+                time_series=self.ddq,
+                name="Joint Acceleration ddq",
+                legend_labels=tuple(r"$\ddot{{q}}_{" + str(i) + "}$" for i in range(self.trajectory.dof))),
+            "tau": available_series_data(
+                time_series=self.torques,
+                name="Joint Torques",
+                legend_labels=tuple(r"$\tau_{" + str(i) + "}$" for i in range(self.trajectory.dof))),
+            "manipulablility": available_series_data(
+                time_series=self.manipulability_indices,
+                name="Manipulability Index",
+                legend_labels=("Manipulability", )),
+            "eef_position": available_series_data(
+                time_series=tuple(self.tcp_pose_at(t).translation for t in self.time_steps),
+                name="EEF Position",
+                legend_labels=(r"$x$", r"$y$", r"$z$")),
+            "eef_rotation": available_series_data(
+                time_series=tuple(self.tcp_pose_at(t).projection.roto_translation_vector for t in self.time_steps),
+                name="EEF Rotation",
+                legend_labels=("$n_x$", r"$n_y$", "$n_z$"))
+        }
+
+        for d in data:
+            if d == "goals":
+                marker = copy(marker)
+                marker.update({t: (g, "red" if g in (failed.id for failed in self.failed_goals) else "green")
+                               for g, t in self.trajectory.goal2time.items()})
+                logging.info("Showing fulfilled goals in green and failed in red.")
+                continue
+            if d not in available:
+                raise ValueError(f"Cannot plot {d} in solution")
+            time_series.append((available[d].time_series, available[d].name))
+            legends.append(available[d].legend_labels)
+
+        f = plot_time_series(self.time_steps, time_series, marker, subplot_kwargs=subplot_kwargs)
+        for i, l in enumerate(legends):
+            f.axes[i].legend(l, loc="upper right")
+
+        if show_figure:
+            with plt.rc_context({'text.usetex': True}):
+                f.show()
+
+        return f
```

### Comparing `timor-python-0.0.8/src/timor/task/Task.py` & `timor-python-0.0.9/src/timor/task/Task.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,33 +3,33 @@
 # Date: 17.01.22
 from __future__ import annotations
 
 from copy import deepcopy
 from dataclasses import dataclass, field
 import datetime
 import itertools
-import json
+import os
 from pathlib import Path
 from typing import Collection, Dict, Iterable, List, Optional, Sequence, Tuple, Union
 import uuid
 import warnings
 
 from hppfcl import hppfcl
 import numpy as np
 import pinocchio as pin
 
 from timor.Robot import PinRobot, RobotBase
 from timor.task import Constraints, Goals
 from timor.task.Obstacle import Obstacle
+from timor.utilities import configurations
 from timor.utilities.dtypes import TypedHeader
-from timor.utilities.file_locations import map2path
-from timor.utilities.json_serialization_formatting import compress_json_vectors
+from timor.utilities.file_locations import map2path, schema_dir
 from timor.utilities.jsonable import JSONable_mixin
 import timor.utilities.logging as logging
-from timor.utilities.schema import DEFAULT_DATE_FORMAT
+from timor.utilities.schema import DEFAULT_DATE_FORMAT, get_schema_validator
 from timor.utilities.visualization import center_camera
 
 GRAVITY = np.array([0, 0, -9.81], dtype=float)  # Default gravity for z upwards TODO : Move to global configuration?!
 robot_or_robots = Union[PinRobot, Iterable[PinRobot]]
 
 
 @dataclass
@@ -48,24 +48,28 @@
     affiliation: List[str] = TypedHeader.string_list_factory()
 
     @classmethod
     def empty(cls) -> TaskHeader:
         """Returns an empty task header"""
         return cls(ID=f'tmp_{uuid.uuid4()}')
 
+    def __eq__(self, other):
+        """Equality of headers is given by equality of attributes"""
+        if not isinstance(other, TaskHeader):
+            return NotImplemented
+        return all(getattr(self, attr) == getattr(other, attr) for attr in self.__annotations__.keys())
+
 
 class Task(JSONable_mixin):
     """A task describes a problem that must be solved by one or multiple robots.
 
     The problem can be composed of multiple goals, each with their own constraints.
     Global constraints, e.g. valid base placements or the order of goals can be defined on the task-level.
     """
 
-    _package_dir: Optional[Path]  # If a task was loaded from disk, this variable stored the path to package directory
-
     def __init__(self,
                  header: Union[TaskHeader, Dict],
                  obstacles: Collection[Obstacle] = None,
                  goals: Sequence['Goals.GoalBase'] = None,
                  constraints: Collection['Constraints.ConstraintBase'] = None
                  ):
         """Create a Task:
@@ -82,57 +86,97 @@
         self.constraints: Tuple['Constraints.ConstraintBase'] = tuple() if constraints is None \
             else tuple(constraints)
 
         if obstacles is not None:
             for obstacle in obstacles:
                 self.add_obstacle(obstacle)
 
-        self._package_dir: Optional[Path] = None
+    @classmethod
+    def from_id(cls, id: str, package_dir: Path) -> Task:
+        """
+        Load a task based on its id stored in package_dir/id.json.
 
-    def __deepcopy__(self, memodict={}):
-        """Custom deepcopy for a scneario class. Experimental!"""
-        cpy = self.__class__(header=deepcopy(self.header))
-        cpy.obstacles = [deepcopy(o) for o in self.obstacles]
-        cpy.goals = [deepcopy(t) for t in self.goals]
-        return cpy
+        :param id: id (including namespace with "/" to look for.
+        :param package_dir: The directory to look for the task in.
+        """
+        return cls.from_json_file(package_dir.joinpath(f"{id}.json"))
+
+    @staticmethod
+    def _deduce_package_dir(filepath: Path, content: Union[Dict, List]) -> Path:
+        """
+        Deduce the package directory from the filepath and the content of the task.
+
+        A task is always stored in <package_dir>/<task.id>.json. The package_dir is the directory; the task.id may also
+        contain subdirectories / namespacing denoted with "/".
+
+        :param filepath: The path to the task file
+        :param content: The content of the task file
+        return: The package directory that all file keys in content are relative to.
+        """
+        if not isinstance(content, dict):
+            raise ValueError(f"Content of {filepath} describing task is not a dictionary.")
+        if 'header' not in content or 'ID' not in content['header']:
+            raise ValueError(f"Content of {filepath} describing task does not contain an ID.")
+        id = content['header']['ID']
+        if not filepath.match(f"**/{id}.json"):
+            raise ValueError(f"Filepath {filepath} of task does not end in ID {id}")
+        # Only keep parts of abs path before ID
+        return Path(*filepath.with_suffix("").parts[:-len(Path(id).parts)])
 
     @classmethod
-    def from_json_data(cls, d: Dict[str, any], package_dir: Union[Path, str]):
+    def from_json_data(cls, d: Dict[str, any], *args, **kwargs):
         """
         Loads a task from a parsed json (=dictionary).
 
         :param d: The parsed json data
-        :param package_dir: The path to the package directory of contained mesh files.
         """
+        _, validator = get_schema_validator(schema_dir.joinpath("TaskSchema.json"))
+        if not validator.is_valid(d):
+            logging.debug(f"Errors: {tuple(validator.iter_errors(d))}")
+            raise ValueError("task.json invalid.")
         content = deepcopy(d)  # Make sure we don't modify the original data while popping items
         header = TaskHeader(**{key: arg for key, arg in content.pop('header').items()})
-        obstacles = [Obstacle.from_json_data(
-            {**specs, **{'package_dir': package_dir}}) for specs in content.pop('obstacles')]
+        obstacles = [Obstacle.from_json_data(specs) for specs in content.pop('obstacles')]
         goals = [Goals.GoalBase.goal_from_json_data(goal) for goal in content.pop('goals', [])]
         if 'Constraints' in content:
             logging.error("Constraints is written in upper case but should be lower case!")
             content['constraints'] = content.pop('Constraints')
         constraints = [Constraints.ConstraintBase.from_json_data(c) for c in content.pop('constraints', [])]
         if len(content) > 0:
             raise ValueError("Unresolved keys: {}".format(', '.join(content)))
         task = cls(header, obstacles, goals=goals, constraints=constraints)
-        task._package_dir = package_dir
         return task
 
-    @classmethod
-    def from_json_file(cls, filepath: Union[Path, str], package_dir: Union[Path, str]):
+    def to_json_file(self, save_at: Union[Path, str],
+                     handle_missing_assets: Optional[str] = None, *args, **kwargs):
         """
-        Loads a task from a json file.
+        Save the task to a json file.
 
-        :param filepath: The path to the json file
-        :param package_dir: The path to the package directory, to which the mesh file paths are relative to.
-        """
-        filepath, package_dir = map(map2path, (filepath, package_dir))
-        content = json.load(filepath.open('r'))
-        return cls.from_json_data(content, package_dir)
+        :param save_at: The path to save the task to.
+          If it is a directory, the task will be saved to save_at/<task.id>.json.
+          If it is a file, the task will be saved to save_at and it is ensured that the filename ends in <task.id>.json.
+        :param handle_missing_assets: How to handle missing assets.
+          See :meth:`timor.utilities.helper.handle_assets` for details.
+        """
+        if handle_missing_assets is None:
+            handle_missing_assets = configurations.task_assets_copy_behavior
+        save_at = map2path(save_at)
+        if len(save_at.suffixes) > 0:  # there is a suffix -> this is a file; is_file only true if already exists
+            if not save_at.match(f"**/{self.id}.json"):
+                raise ValueError(f"Filepath {save_at} does not end in ID {self.id} of self.")
+            new_package_dir = map2path(*save_at.with_suffix("").parts[:len(Path(self.id).parts)])
+        elif save_at.is_dir():
+            new_package_dir = save_at
+            save_at = new_package_dir / f"{self.id}.json"
+        else:
+            raise ValueError("save_at must be a file or directory.")
+        os.makedirs(save_at.parent, exist_ok=True)
+
+        super().to_json_file(save_at, new_package_dir=new_package_dir,
+                             handle_missing_assets=handle_missing_assets, *args, **kwargs)
 
     @staticmethod
     def from_srf_file(filepath: Path):
         """Future Work"""
         raise NotImplementedError()  # TODO
 
     @classmethod
@@ -178,27 +222,14 @@
         # Objects
         # TODO: Implement Objects in Tasks
 
         # Goals
         content['goals'] = [goal.to_json_data() for goal in self.goals]
         return content
 
-    def to_json_file(self, filepath: Path):
-        """
-        Write a task to a json file.
-
-        :param filepath: The path to the file to write the json to
-        """
-        filepath = map2path(filepath)
-        content = compress_json_vectors(json.dumps(self.to_json_data(), indent=2))
-        if (self._package_dir is not None) and (not str(filepath).startswith(str(self._package_dir))):
-            logging.info("Writing task to file outside of the package directory it was loaded from.")
-        with filepath.open('w') as f:
-            f.write(content)
-
     @property
     def collision_objects(self) -> Tuple[hppfcl.CollisionObject, ...]:
         """All hppfcl collision objects by obstacles in the task"""
         warnings.warn("New feature collision objects - so far not tested!")
         return tuple(itertools.chain.from_iterable(obstacle.collision_objects for obstacle in self.obstacles))
 
     @property
@@ -295,7 +326,37 @@
             try:
                 base_constraint = self.base_constraint
                 center_camera(viz.viewer, base_constraint.base_pose.nominal.translation)
             except AttributeError:
                 logging.info("Cannot recenter visualizer view to base.")
 
         return viz
+
+    def __deepcopy__(self, memodict={}):
+        """Custom deepcopy for a scneario class. Experimental!"""
+        cpy = self.__class__(header=deepcopy(self.header))
+        cpy.obstacles = [deepcopy(o) for o in self.obstacles]
+        cpy.goals = tuple(deepcopy(t) for t in self.goals)
+        cpy.constraints = tuple(deepcopy(c) for c in self.constraints)
+        return cpy
+
+    def __eq__(self, other):
+        """Tasks are equal if headers, goals, constraints, and obstacles are equal."""
+        if not isinstance(other, Task):
+            return NotImplemented
+        return (self.header == other.header
+                and self.obstacles == other.obstacles
+                and self.goals == other.goals
+                and self.constraints == other.constraints)
+
+    def __getstate__(self):
+        """Return objects which will be pickled and saved."""
+        return self.to_json_data()
+
+    def __hash__(self):
+        """Hash is given by the unique ID."""
+        return hash(self.id)
+
+    def __setstate__(self, state):
+        """Take object from parameter and use it to retrieve class state."""
+        cpy = self.__class__.from_json_data(state)
+        self.__dict__ = cpy.__dict__
```

### Comparing `timor-python-0.0.8/src/timor/task/Tolerance.py` & `timor-python-0.0.9/src/timor/task/Tolerance.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor/utilities/download_data.py` & `timor-python-0.0.9/src/timor/utilities/download_data.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor/utilities/dtypes.py` & `timor-python-0.0.9/src/timor/utilities/dtypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 from collections import namedtuple
 from dataclasses import asdict, dataclass, field, fields
 import datetime
 import logging
 import random
 import re
-from typing import Any, Callable, Collection, Dict, Generator, Generic, Iterable, List, Tuple, Type, TypeVar, Union, \
-    get_type_hints
+from typing import Any, Callable, Collection, Dict, Generator, Generic, Iterable, List, Tuple, Type, \
+    TypeVar, Union, get_type_hints
 
 from hppfcl import hppfcl
 import numpy as np
 import pinocchio as pin
 
-import timor.utilities.errors as err
+from timor.utilities import errors as err
 from timor.utilities.schema import DEFAULT_DATE_FORMAT
 from timor.utilities.transformation import Transformation, TransformationLike
 
 T = TypeVar('T')
 IntermediateIkResult = namedtuple("IntermediateIkResult", ["q", "distance"])
 
 
@@ -170,14 +170,51 @@
                 if element in self:
                     raise err.UniqueValueError(self._err.format(element))
                 elif element in elements:
                     raise err.UniqueValueError(f"The element {element} is provided multiple times in the input.")
                 elements.add(element)
         return self.__class__(super().union(elements))
 
+    @classmethod
+    def _sorting_key(cls, element: any) -> any:
+        """Key function for sorting elements in this set"""
+        raise NotImplementedError(f"There is no way to uniquely sort elements in sets of type {cls.__name__}.")
+
+    def __eq__(self, other):
+        """If there is a unique ordering to this set, try to sort the elements and compare them"""
+        if not isinstance(other, SingleSet):
+            return NotImplemented
+        try:
+            ordered_self = sorted(self, key=self._sorting_key)
+            ordered_other = sorted(other, key=other._sorting_key)
+        except NotImplementedError:
+            return super().__eq__(other)
+        return ordered_self == ordered_other
+
+    def __hash__(self):
+        """Hash all the contained elements"""
+        return sum(hash(element) for element in self)
+
+    def __ne__(self, other):
+        """Override the not equal operatorof a set"""
+        return not self == other
+
+
+class SingleSetWithID(SingleSet):
+    """A class for SingleSets where every element has a unique ID"""
+
+    @classmethod
+    def _sorting_key(cls, element: any) -> any:
+        """Key function for sorting elements in this set"""
+        return element.id
+
+    def __contains__(self, item: any):
+        """Custom duplicate check (unique ID)"""
+        return item.id in (element.id for element in self)
+
 
 @dataclass
 class TypedHeader:
     """A dataclass that ensures and transforms {Module, Task, Solution}-header data to the desired datatypes."""
 
     def __post_init__(self):
         """Post init function that ensures the correct datatypes"""
```

### Comparing `timor-python-0.0.8/src/timor/utilities/errors.py` & `timor-python-0.0.9/src/timor/utilities/errors.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor/utilities/file_locations.py` & `timor-python-0.0.9/src/timor/utilities/file_locations.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 # Date: 29.03.22
 from __future__ import annotations
 
 from itertools import chain
 import json
 from pathlib import Path
 import re
-from typing import Dict, List, Tuple, Union
+import shutil
+from typing import Dict, List, Union
 
 from timor.utilities import logging
 from timor.utilities.configurations import CONFIG_FILE, TIMOR_CONFIG
 from timor.utilities.download_data import download_additional_robots, download_schemata
 
 __utilities = Path(__file__).parent.absolute()
 package = __utilities.parent  # Main directory of the package
 head = package.parent
 cache_dir = head.joinpath("cache")  # For caching downloaded robots, etc.
 if not cache_dir.exists():
     cache_dir.mkdir()
 logging.info("Loading custom configurations from {}".format(CONFIG_FILE))
 log_conf = TIMOR_CONFIG['FILE_LOCATIONS'] if TIMOR_CONFIG.has_section('FILE_LOCATIONS') else dict()
-test_data = Path(log_conf.get('test_data', head.parent.joinpath('tests/data')))
+test_data = Path(log_conf.get('test_data', head.parent.joinpath('tests/data'))).expanduser()
+if not test_data.exists():
+    test_data = None
 default_robot_dir = head.joinpath('timor_sample_robots')
 cache_robot_dir = cache_dir.joinpath("robots")
 if not cache_robot_dir.exists():
     cache_robot_dir.mkdir()
 
 # Get schemas
 schema_dir = Path(log_conf.get('schema_dir', cache_dir.joinpath("schemata")))
@@ -48,48 +51,58 @@
 else:
     robots = {d.name: d for d in default_robot_dir.iterdir()}
 
 # Get robots available via CoBRA
 download_additional_robots(cache_robot_dir, robots)
 module_DBs = robots  # alias
 
-DEFAULT_TASK_FILTER = re.compile(".*(PTP_1|PTP_2|PTP_2_cycle|PTP_3|Empty|traj_1|traj_window)+.json")
+DEFAULT_TASK_FILTER = re.compile(".*(task|PTP_1|PTP_2|PTP_2_cycle|PTP_3|Empty|traj_1|traj_window)+.json")
 
 
 def get_test_tasks(task_name: re.Pattern = DEFAULT_TASK_FILTER) -> Dict[str, Union[Path, List[Path]]]:
     """
     Gives access to all test tasks from the test_data folder.
 
     :param task_name: A regular expression pattern that is run against task files to be loaded
     :return: A dictionary mapping the "kind" of the task or solution file to the matching path.
     """
+    if test_data is None:
+        raise FileNotFoundError("Test data not found. It is only available if the package is installed from source.")
     task_dir = test_data.joinpath('sample_tasks/simple')
-    task_files = list(file for file in task_dir.iterdir() if file.name.endswith('.json'))
+    task_files = task_dir.rglob("**/*.json")
 
     task_files = [task for task in task_files if task_name.search(task.name)]
     asset_dir = task_dir.parent.joinpath("assets")
 
     return {"task_files": task_files,
             "task_dir": task_dir,
             "asset_dir": asset_dir}
 
 
-def get_module_db_files(name: str) -> Tuple[Path, Path]:
+def get_module_db_files(name: str) -> Path:
     """
     Returns the filepaths to the database json file and the package folder for names of valid module databases.
 
     :param name: The (folder) name of the module set
-    :return: (Path to modules.json, Path to package folder)
+    :return: Path to modules.json (all assets are in the same folder)
     """
     if name not in robots:
         raise FileNotFoundError(f"Robot of name {name} is unknown!")
     module_file = module_DBs[name].joinpath('modules.json')
     if not module_file.exists():
         raise FileNotFoundError("Module Set File {} not found.".format(module_file))
-    return module_file, module_file.parent
+    return module_file
 
 
 def map2path(p: Union[str, Path]) -> Path:
     """Maps strings to paths, but does nothing else s.t. e.g. Django paths are not casted."""
     if isinstance(p, str):
         return Path(p)
-    return p
+    return p.expanduser()
+
+
+def clean_caches():
+    """
+    Helper to clean timor caches, e.g., to download all module sets after they have been updated.
+    """
+    shutil.rmtree(cache_dir)
+    logging.info("Please reimport timor, e.g., by closing python interpreter and restarting your program.")
```

### Comparing `timor-python-0.0.8/src/timor/utilities/json_serialization_formatting.py` & `timor-python-0.0.9/src/timor/utilities/json_serialization_formatting.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,25 +4,17 @@
 import numpy as np
 
 """Contains functions to prettify, verify, fix, ... json file in and output."""
 
 
 def compress_json_vectors(content: str) -> str:
     """Compresses json vectors and matrices, s.t. innermost on single line"""
-    here = 0
     # Matches inner parts of vectors [Number,...,Number] where each number in scientific notation
     pattern = re.compile(r"\[\s*(?:-?\d+(?:.\d+)?(?:e[-+]?\d+)?,?\s*)+\]")
-    while here < len(content):
-        m = pattern.search(content, here)
-        if m is None:
-            break
-        content = content[:m.start()] + re.sub(r"\s+", " ", content[m.start():m.end()]) + content[m.end():]
-        here = m.start() + 1
-
-    return content
+    return pattern.sub(lambda m: re.sub(r"\s+", " ", m.group()), content)  # replace newline + whitespace in innermost
 
 
 def numpy2list(d: Dict[str, any]) -> Dict[str, any]:
     """Converts all numpy arrays in a dictionary to lists and returns the according copy"""
     ret = {}
     for key, value in d.items():
         if isinstance(value, np.ndarray):
```

### Comparing `timor-python-0.0.8/src/timor/utilities/logging.py` & `timor-python-0.0.9/src/timor/utilities/logging.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor/utilities/module_classification.py` & `timor-python-0.0.9/src/timor/utilities/module_classification.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor/utilities/prebuilt_robots.py` & `timor-python-0.0.9/src/timor/utilities/prebuilt_robots.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor/utilities/schema.py` & `timor-python-0.0.9/src/timor/utilities/schema.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor/utilities/spatial.py` & `timor-python-0.0.9/src/timor/utilities/spatial.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor/utilities/tolerated_pose.py` & `timor-python-0.0.9/src/timor/utilities/tolerated_pose.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
         :param other: The placement to compare to.
         :return: True if the other is valid with regard to self, False otherwise.
         """
         return self.tolerance.valid(self.nominal, other)
 
     @classmethod
-    def from_json_data(cls, d: Dict[str, any]) -> ToleratedPose:
+    def from_json_data(cls, d: Dict[str, any], *args, **kwargs) -> ToleratedPose:
         """Create a ToleratedPose from a json description.
 
         :param d: A json description as defined in the task documentation.
         :return: A ToleratedPose.
         """
         nominal = d['nominal']
         projections = d.get('toleranceProjection', ())
```

### Comparing `timor-python-0.0.8/src/timor/utilities/trajectory.py` & `timor-python-0.0.9/src/timor/utilities/trajectory.py`

 * *Files 2% similar despite different names*

```diff
@@ -212,14 +212,21 @@
             if len(ddq.shape) == 1:
                 logging.info(f"Assuming ddq with single dimension is multiple steps (shape = {ddq.shape}); "
                              f"to force otherwise please give dq as 1 x {ddq.shape[0]} array")
                 ddq = ddq[:, None]
         self._ddq = ddq
 
     @property
+    def dof(self):
+        """Number of degrees of freedom encoded by this trajectory."""
+        if not self.has_q:
+            raise ValueError("DoF only defined for joint trajectory with q")
+        return self.q.shape[1]
+
+    @property
     def is_timed(self) -> bool:
         """Does this trajectory enforce time."""
         return self.t is not None
 
     @property
     def has_poses(self) -> bool:
         """Does this trajectory enforce a pose."""
```

### Comparing `timor-python-0.0.8/src/timor/utilities/transformation.py` & `timor-python-0.0.9/src/timor/utilities/transformation.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import hppfcl
 from hppfcl import Transform3f
 import numpy as np
 import pinocchio as pin
 from scipy.spatial.transform import Rotation
 
 from timor.utilities import logging, spatial
-import timor.utilities.errors as err
+from timor.utilities import errors as err
 from timor.utilities.jsonable import JSONable_mixin
 
 _TransformationConvertable = Union[
     List[Union[List[float], Tuple[float, float, float, float]]],
     Tuple[Union[List[float], Tuple[float, float, float, float]],
           Union[List[float], Tuple[float, float, float, float]],
           Union[List[float], Tuple[float, float, float, float]],
@@ -158,16 +158,17 @@
                 err.assert_is_homogeneous_transformation(transformation)
             except err.NonOrthogonalRotationError:  # Try fixing almost orthogonal rotation matrices
                 transformation.setflags(write=True)
                 transformation[:3, :3] = Rotation.from_matrix(transformation[:3, :3]).as_matrix()
                 err.assert_is_homogeneous_transformation(transformation)
 
         self.homogeneous: np.ndarray = transformation
+        self.homogeneous: np.ndarray = transformation
 
-    def distance(self, other: TransformationConvertable) -> Norm:
+    def distance(self, other: Union[Transformation, TransformationConvertable]) -> Norm:
         """
         Returns a norm  object for the transformation between self and other.
 
         A distance between two poses is not uniquely defined -- returning a norm object is one possible way to deal
         with this problem: The returned object itself has multiple properties, each one according to one possible
         norm (translational, rotational or a combination) of the transformation representing the relative difference
         between self and other.
```

### Comparing `timor-python-0.0.8/src/timor/utilities/visualization.py` & `timor-python-0.0.9/src/timor/utilities/visualization.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #!/usr/bin/env python3
 # Author: Jonathan Külz
 # Date: 03.03.22
 import logging
-from typing import Dict, List, Tuple, Union
+from typing import Dict, Iterable, List, Optional, Sequence, Tuple, Union
 
+from matplotlib import pyplot as plt
 import meshcat.animation
 import meshcat.geometry
 import numpy as np
 from pinocchio import COLLISION, VISUAL  # noqa: F401
 import pinocchio as pin
 from pinocchio.visualize.meshcat_visualizer import MeshcatVisualizer, isMesh
 
 from timor import ModuleAssembly
 from timor.utilities import module_classification, spatial, transformation
-
+from timor.utilities.transformation import Transformation
 
 DEFAULT_COLOR_MAP = {  # Type enumeration from module_classification - import not possibility (circular import)
     module_classification.ModuleType.BASE: np.array([165 / 255, 165 / 255, 165 / 255, 1.]),
     module_classification.ModuleType.LINK: np.array([127 / 255, 127 / 255, 127 / 255, 1.]),
     module_classification.ModuleType.JOINT: np.array([248 / 255, 135 / 255, 1 / 255, 1.]),
     module_classification.ModuleType.END_EFFECTOR: np.array([250 / 255, 182 / 255, 1 / 255, 1.]),
 }
@@ -273,19 +274,34 @@
     head_length = length * 2 / 5
     rmax_head = 1.5 * length / 5
     base = meshcat.geometry.Cylinder(base_length, base_width)
     head = meshcat.geometry.Cylinder(head_length, radiusTop=0, radiusBottom=rmax_head)
 
     viz.viewer[name + '_arr_body'].set_object(base, material)
     base_transform = placement @ rot @ spatial.homogeneous(translation=[0, -.5 * base_length - head_length, 0])
-    viz.viewer[name + '_arr_body'].set_transform(base_transform)
+    viz.viewer[name + '_arr_body'].set_transform(base_transform.homogeneous)
 
     viz.viewer[name + '_arr_head'].set_object(head, material)
     head_transform = placement @ rot @ spatial.homogeneous(translation=[0, -.5 * head_length, 0])
-    viz.viewer[name + '_arr_head'].set_transform(head_transform)
+    viz.viewer[name + '_arr_head'].set_transform(head_transform.homogeneous)
+
+
+def place_sphere(viewer: meshcat.visualizer.Visualizer, name: str, radius: float, placement: Transformation,
+                 material: meshcat.geometry.Material = meshcat.geometry.MeshBasicMaterial()):
+    """
+    Place a sphere with name, radius and color at a specific placement.
+
+    :param viewer: meshcat.visualizer.Visualizer instance to draw into (viz.viewer if you have a MeshcatVisualizer)
+    :param name: Unique object name within the visualizer
+    :param radius: Sphere radius in meters
+    :param placement: Defines placement of the sphere.
+    :param material: material used to render this sphere
+    """
+    viewer[name].set_object(meshcat.geometry.Sphere(radius), material)
+    viewer[name].set_transform(placement.homogeneous)
 
 
 def scene_text(text: str, size: float = 1., **kwargs):
     """
     Create a cube geometry with text displayed on sides and size edge length.
 
     Altered from meshcat-py master branch
@@ -293,7 +309,56 @@
 
     :todo: Only have one rightly oriented TextTexture...
     """
     return meshcat.geometry.Mesh(meshcat.geometry.Box((size, 0, size)),
                                  meshcat.geometry.MeshPhongMaterial(map=TextTexture(text, **kwargs),
                                                                     transparent=True,
                                                                     needsUpdate=True))
+
+
+def plot_time_series(times: Sequence[float], data: Sequence[Tuple[np.ndarray, str]],
+                     marker: Dict[float, Tuple[str, str]] = None, additional_subplots: int = 0,
+                     show_figure: bool = False, subplot_kwargs: Optional[Dict] = None) \
+        -> plt.Figure:
+    """
+    Helper to plot time series data
+
+    :param times: Time (x-value) for the sampled data at N steps
+    :param data: Timeseries, each containing a NxM array of N samples of M-dimensional data at each time in times and
+      an axis label for this data; creates one subplot per timeseries
+    :param marker: A dictionary where keys are times to draw a marking line with label and color at
+    :param additional_subplots: leave space for more subplots
+    :param show_figure: Call show on returned figure
+    :param subplot_kwargs: Kwargs handed to subplots, including pyplot.figure kwargs
+      (see https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.subplots.html)
+    :return: figure containing all these
+    """
+    if marker is None:
+        marker = {}
+
+    data = tuple(data)
+    default_subplot_kwargs = {"sharex": "row"}
+    default_subplot_kwargs.update({} if subplot_kwargs is None else subplot_kwargs)
+    f, axes = plt.subplots(len(data) + additional_subplots, 1, **default_subplot_kwargs)
+    if not isinstance(axes, Iterable):
+        axes = (axes, )
+
+    for idx, d in enumerate(data):
+        axes[idx].plot(times, d[0])
+        axes[idx].set(ylabel=d[1])
+
+    axes[-1].set(xlabel="Time t [s]")
+
+    time_frame = np.max(times) - np.min(times)
+
+    for time, marker in marker.items():
+        name, color = marker
+        for ax in axes:
+            ax.axvline(time, c=color)
+            ax.text(time + 0.01 * time_frame,  # Slight offset from line
+                    .9, name, c=color, transform=ax.get_xaxis_transform())
+
+    plt.tight_layout()
+    if show_figure:
+        plt.show()
+
+    return f
```

### Comparing `timor-python-0.0.8/src/timor/utilities/write_urdf.py` & `timor-python-0.0.9/src/timor/utilities/write_urdf.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_python.egg-info/PKG-INFO` & `timor-python-0.0.9/src/timor_python.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: timor-python
-Version: 0.0.8
+Version: 0.0.9
 Summary: Toolbox for Industrial Modular Robots
 Author-email: Jonathan Kuelz <jonathan.kuelz@tum.de>
 License: MIT
 Project-URL: Source Code, https://gitlab.lrz.de/tum-cps/timor-python
 Project-URL: Documentation, https://timor-python.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://gitlab.lrz.de/tum-cps/timor-python/-/issues
 Keywords: Modular Reconfigurable Robots,Robot Design,Model Generation,Simulation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 Provides-Extra: optimization
 Provides-Extra: full
 License-File: LICENSE
 
 .. image:: https://gitlab.lrz.de/tum-cps/timor-python/-/raw/main/img/timor_banner.png
@@ -53,15 +53,15 @@
     :alt: Animation of a robot assembly moving between two goals
     :align: center
     :target: https://gitlab.lrz.de/tum-cps/timor-python/-/raw/main/img/animations/demo_animation.gif
 
 
 Installation
 ------------
-Timor-python is available on PyPI. It requires **at least Python 3.7**. For installation, use::
+Timor-python is available on PyPI. It requires **at least Python 3.8**. For installation, use::
 
    pip install timor-python
 
 Some requirements are not included by default - in order to install them, use::
 
   pip install timor-python[option]
 
@@ -73,14 +73,16 @@
 If you want to work with the bleeding-edge version, you can download the source code from the project repository and install it locally.
 Nagivate to the timor-python repository you cloned and enter::
 
    pip install -e .
 
 to install it in editeable mode. This requires :code:`setuptools>=61` and :code:`pip>=21.3` (previous versions of setuptools require a :code:`setup.py`-file). To install optional dependencies, proceed in the same manner as for PyPI installs.
 
+To run unittest locally, you need to `setup git lfs <https://git-lfs.com/>`_ in order to download assets.
+
 If you want to use pre-commit hooks provided with Timor, for installation please use::
 
    pip install pre-commit
 
 then::
 
    pre-commit install
@@ -99,14 +101,22 @@
 
   jupyter lab
 
 You can set custom configurations such as file paths of robot libraries or logging behavior by editing the config file. You can import the file location of the config file as :code:`from timor.utilities.configurations import CONFIG_FILE`.
 
 For further information, please visit the `documentation <https://timor-python.readthedocs.io>`_.
 
+Updating
+--------
+
+Some timor updates might require to re-acquire the task, schema, or robot module data-bases. Try to reset the caches by running ``timor.utilities.file_locations.clean_caches()`` and re-import the timor module.
+
+Typical errors indicating this action:
+ * ValueError: modules.json invalid.
+
 Support
 -------
 Do you have a question or an issue using Timor? You can either `submit an issue <https://gitlab.lrz.de/tum-cps/timor-python/-/issues>`_ or write an email to the `repository maintainer <mailto:jonathan.kuelz@tum.de>`_.
 
 Contributing
 ------------
 We welcome every contribution to Timor. For more details, please refer to our `contribution guidelines <https://gitlab.lrz.de/tum-cps/timor-python/-/blob/main/CONTRIBUTING.md>`_.
```

### Comparing `timor-python-0.0.8/src/timor_python.egg-info/SOURCES.txt` & `timor-python-0.0.9/src/timor_python.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 src/timor/task/Goals.py
 src/timor/task/Obstacle.py
 src/timor/task/Solution.py
 src/timor/task/Task.py
 src/timor/task/Tolerance.py
 src/timor/task/__init__.py
 src/timor/utilities/__init__.py
+src/timor/utilities/asset_handling.py
 src/timor/utilities/configurations.py
 src/timor/utilities/download_data.py
 src/timor/utilities/dtypes.py
 src/timor/utilities/errors.py
 src/timor/utilities/file_locations.py
 src/timor/utilities/json_serialization_formatting.py
 src/timor/utilities/jsonable.py
```

### Comparing `timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/L1.stl` & `timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/L1.stl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/L10.stl` & `timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/L10.stl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/L2.stl` & `timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/L2.stl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/L3.stl` & `timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/L3.stl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/L8.stl` & `timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/L8.stl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/L9.stl` & `timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/L9.stl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L1.stl.wrl` & `timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L1.stl.wrl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L2.stl.wrl` & `timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L2.stl.wrl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L3.stl.wrl` & `timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L3.stl.wrl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L8.stl.wrl` & `timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L8.stl.wrl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L9.stl.wrl` & `timor-python-0.0.9/src/timor_sample_robots/IMPROV/STLfiles/convexDecompose/L9.stl.wrl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/IMPROV/modules.json` & `timor-python-0.0.9/src/timor_sample_robots/IMPROV/modules.json`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/geometric_primitive_modules/modules.json` & `timor-python-0.0.9/src/timor_sample_robots/geometric_primitive_modules/modules.json`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/LICENSE` & `timor-python-0.0.9/src/timor_sample_robots/panda/LICENSE`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/hand.stl` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/hand.stl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link0.stl` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link0.stl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link1.stl` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link1.stl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link2.stl` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link2.stl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link3.stl` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link3.stl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link4.stl` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link4.stl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link5.stl` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link5.stl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link6.stl` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link6.stl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/collision/link7.stl` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/collision/link7.stl`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/finger.dae` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/finger.dae`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/hand.dae` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/hand.dae`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link0.dae` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link0.dae`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link1.dae` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link1.dae`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link2.dae` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link2.dae`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link3.dae` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link3.dae`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link4.dae` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link4.dae`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link5.dae` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link5.dae`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link6.dae` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link6.dae`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/meshes/visual/link7.dae` & `timor-python-0.0.9/src/timor_sample_robots/panda/meshes/visual/link7.dae`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/src/timor_sample_robots/panda/urdf/panda.urdf` & `timor-python-0.0.9/src/timor_sample_robots/panda/urdf/panda.urdf`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/tests/test_assembly.py` & `timor-python-0.0.9/tests/test_assembly.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import time
 import unittest
 
 import networkx as nx
 import numpy as np
 import numpy.testing as np_test
 
@@ -15,16 +16,16 @@
 from timor.Joints import TimorJointType
 
 
 class TestModuleAssembly(unittest.TestCase):
 
     def setUp(self) -> None:
         """Initialize some modules"""
-        self.json_file, self.package_dir = get_module_db_files('IMPROV')
-        self.db = ModulesDB.from_file(self.json_file, package_dir=self.package_dir)
+        self.json_file = get_module_db_files('IMPROV')
+        self.db = ModulesDB.from_json_file(self.json_file)
 
     def test_graph_features(self):
         """An assembly of modules is (given some abstraction) just a graph. Check some basic graph attributes:"""
         assembly = ModuleAssembly(self.db)
         for _ in range(12):
             assembly.add_random_from_db(lambda x: x not in self.db.end_effectors)
 
@@ -69,14 +70,24 @@
         # Check that an empty assembly does not need to stay empty
         assembly = ModuleAssembly(self.db)
         assembly.add_random_from_db()
         assembly.add_random_from_db()
         self.assertIsNotNone(assembly.base_connector)
         self.assertEqual(len(assembly.module_instances), 2)
 
+        # Check that the assembly can be (de)serialized and we have a functional (in)equality
+        new_assembly = assembly.from_json_string(assembly.to_json_string())
+        self.assertEqual(assembly, new_assembly)
+        try:
+            new_assembly.add_random_from_db()
+        except LookupError:
+            logging.debug("No modules left to add. Removing one module for inequality test")
+            new_assembly.connections.pop()
+        self.assertNotEqual(assembly, new_assembly)
+
     def test_parameterizable_assembly(self):
         """Tests assemblies containing at least on parameterizable module."""
         base_header = ModuleHeader('B', 'Base')
         cyl_header = ModuleHeader('cylinder', 'cylinder')
         l_header = ModuleHeader('L', 'orthogonal link')
         straight_header = ModuleHeader('J1', 'Straight Prismatic Joint')
         orthogonal_header = ModuleHeader('J2', 'Orthogonal Revolute Joint')
```

### Comparing `timor-python-0.0.8/tests/test_assembly_iterator.py` & `timor-python-0.0.9/tests/test_assembly_iterator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,32 @@
+import itertools
 import unittest
 
 from timor.Module import ModulesDB
 from timor.configuration_search.LiuIterator import Science2019
+from timor.utilities.dtypes import randomly
 
 
 class AssemblyIteratorTest(unittest.TestCase):
     """Test assembly iterators."""
     def setUp(self) -> None:
         self.modrob_db = ModulesDB.from_name('PROMODULAR')
 
     def test_liu_iterator(self):
         modrob_iterator = Science2019(self.modrob_db, min_dof=1, max_dof=3, max_links_between_joints=1)
-        lots_of_assemblies = tuple(modrob_iterator)
+        num_assemblies_tested = 1000  # reduce the runtime of this test by limiting the number of assemblies generated
+        lots_of_assemblies = []
+        for assembly in itertools.islice(modrob_iterator, num_assemblies_tested):
+            lots_of_assemblies.append(assembly)
         assembly_modules = tuple(assembly.internal_module_ids for assembly in lots_of_assemblies)
         self.assertEqual(len(modrob_iterator), 100548)
-        self.assertEqual(len(lots_of_assemblies), len(modrob_iterator))  # custom len is correct
         self.assertEqual(len(lots_of_assemblies), len(set(assembly_modules)))
 
-        # Check validity by converting the assemblies to a robot. Take a subsample only due to time constraints
-        for assembly in lots_of_assemblies[::2000]:
+        # Check validity by converting 5 assemblies to a robot
+        for assembly in itertools.islice(randomly(lots_of_assemblies), 5):
             robot = assembly.to_pin_robot()
 
         j = 0
         stop_at = 20
         modrob_iterator.reset()
         # Another way to check there are valid robots
         for j, assembly in enumerate(modrob_iterator):
@@ -31,14 +35,21 @@
                 break
         self.assertEqual(j, stop_at)  # Make sure we actually tested 100 samples
 
         with self.assertRaises(ValueError):
             # Make sure to prevent instantiating iterators where the preparations alone already take too long
             iterator = Science2019(self.modrob_db, max_dof=10, max_links_between_joints=5)
 
+        smaller_iterator = Science2019(self.modrob_db, min_dof=1, max_dof=2, max_links_between_joints=1)
+        self.assertEqual(len(smaller_iterator), len(tuple(smaller_iterator)))
+        for i, (a1, a2) in enumerate(zip(tuple(smaller_iterator), smaller_iterator)):
+            if i >= 10:
+                break
+            self.assertEqual(a1, a2)
+
     def test_science_paper_liu(self):
         """
         Tests that this iterator really yields the same combinations as the ones in the science paper.
         Applies some fixes not really intended to do with this iterator, but necessary to get to the same combinations.
         This is mostly due to the domain knowledge applied by liu et al. which is specific to the schunk robot...
         """
         schunk_db = ModulesDB.from_name('IMPROV')
@@ -72,15 +83,10 @@
         iterator._current_joint_combination = iterator.joint_combinations[iterator.state.joints]
         iterator._current_num_joint_combinations = len(iterator.valid_joint_combinations)
         iterator._current_num_joint_modules = len(iterator.joint_combinations[iterator.state.joints])
 
         expected_num_assemblies = 32768  # Number taken from published MATLAB implementation
         self.assertEqual(len(iterator), expected_num_assemblies)
 
-        i = 0
-        for _ in iterator:
-            i += 1
-        self.assertEqual(i, expected_num_assemblies)  # Iterator really yields __len__ combinations
-
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timor-python-0.0.8/tests/test_bodies_geometries.py` & `timor-python-0.0.9/tests/test_bodies_geometries.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from copy import copy, deepcopy
 import importlib
+import itertools
 import logging
 import pickle
 import unittest
 
 from hppfcl import CollisionRequest, CollisionResult, collide
 import meshcat
 import numpy as np
@@ -61,14 +62,20 @@
 
         composed = Geometry.ComposedGeometry([box, cylinder, sphere, mesh])
         empty = Geometry.EmptyGeometry()
         self.assertEqual(composed.volume, box.volume + cylinder.volume + sphere.volume + mesh.volume)
         composed._composing_geometries.append(empty)
         self.assertEqual(composed.volume, box.volume + cylinder.volume + sphere.volume + mesh.volume)
 
+        another_composed = Geometry.ComposedGeometry([mesh, sphere, box, cylinder])
+        self.assertEqual(composed, another_composed)
+
+        for g1, g2 in itertools.combinations([box, cylinder, sphere, mesh], 2):
+            self.assertNotEqual(g1, g2)
+
         # Deepcopy
         for g in (box, cylinder, sphere, mesh):
             g_new = deepcopy(g)
             self.assertEqual(g.volume, g_new.volume)
             self.assertDictEqual(g.parameters, g_new.parameters)
 
     def test_parameterizable_body(self):
```

### Comparing `timor-python-0.0.8/tests/test_collisions.py` & `timor-python-0.0.9/tests/test_collisions.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/tests/test_custom_types.py` & `timor-python-0.0.9/tests/test_custom_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,17 @@
         self.assertIsInstance(original_robots.union(places), SingleSet)  # Check if union returns the right dtype
 
         # Finally, a test with random numbers:
         for _ in range(100):
             numbers = np.random.randint(0, 20, (20,))
             original_set = set(numbers)
             if len(numbers) == len(original_set):  # No duplicates
-                self.assertIsNone(SingleSet(numbers))
+                self.assertEqual(original_set, SingleSet(numbers))
+                original_set.pop()
+                self.assertNotEqual(original_set, SingleSet(numbers))
             else:
                 with self.assertRaises(err.UniqueValueError):
                     SingleSet(numbers)
 
     def test_StronglyTypedHeader(self):
         @dataclass
         class TestHeader(TypedHeader):
```

### Comparing `timor-python-0.0.8/tests/test_imports.py` & `timor-python-0.0.9/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/tests/test_logging.py` & `timor-python-0.0.9/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/tests/test_module.py` & `timor-python-0.0.9/tests/test_module.py`

 * *Files 17% similar despite different names*

```diff
@@ -81,25 +81,29 @@
         """Tests connector instantiation and internal methods"""
 
         f = Bodies.Gender.female
         m = Bodies.Gender.male
         h = Bodies.Gender.hermaphroditic
 
         first = Bodies.Connector('1', Transformation.random(), gender=f, connector_type='test', size=80)
+        first_duplicate = Bodies.Connector('1', first.body2connector, gender=f, connector_type='test', size=80)
         second = Bodies.Connector('2', Transformation.random(), gender=m, connector_type='test', size=80)
         third = Bodies.Connector('3', Transformation.random(), gender=h, connector_type='test', size=80)
         fourth = Bodies.Connector('4', Transformation.random(), gender=h, connector_type='test', size=80)
         # The last two are designed to match no other, either due to size or type
         fifth = Bodies.Connector('5', Transformation.random(), gender=h, connector_type='test', size=120)
         sixth = Bodies.Connector('6', Transformation.random(), gender=h, connector_type='test_other', size=80)
         all_connectors = (first, second, third, fourth, fifth, sixth)
 
         # First, let's do a custom sanity checks
         self.assertTrue(first.connects(second))  # Basic male - female
         self.assertTrue(third.connects(fourth))  # Basic hermaphroditic - hermaphroditic
+        self.assertEqual(first, first_duplicate)  # Equality check
+        for other in all_connectors[1:]:
+            self.assertNotEqual(first, other)  # Inequality check
 
         # Check incompatibility to others due to type and size
         for other in all_connectors:
             if other is not fifth:
                 self.assertFalse(fifth.connects(other))
             if other is not sixth:
                 self.assertFalse(sixth.connects(other))
@@ -138,14 +142,16 @@
         self.assertIsInstance(pin_joint, pin.JointModelRZ)
 
         parent.connectors.add(c)
         child.connectors.add(c)
         with self.assertRaises(err.UniqueValueError):
             joint = Joint(1, TimorJointType.revolute, parent, child)
 
+        self.assertEqual(joint, joint)
+
     def test_module(self):
         """Tests a module on instantiation, uniqueness of contained elements, and hand-crafted IDs"""
         # Setup: Some connectors, bodies and a joint - important is, that some ID's overlap
         c1 = Bodies.Connector('1', spatial.homogeneous([.25, 0, 0]), connector_type='flange')
         c1_cpy = Bodies.Connector('1', spatial.homogeneous([.25, 0, 0]), connector_type='flange')
         c2 = Bodies.Connector('2', spatial.homogeneous([.25, 0, 0]), connector_type='flange')
         c2_cpy = Bodies.Connector('2', spatial.homogeneous([.25, 0, 0]), connector_type='flange')
@@ -170,31 +176,37 @@
         header_one = ModuleHeader('1', 'Test module one', author=['Jonathan'], email=['jonathan.kuelz@tum.de'],
                                   affiliation=['TUM'])
         header_two = dict(ID='2', name='Test module two', author=['Jonathan'],
                           email=['jonathan.kuelz@tum.de'], affiliation=['TUM'])
 
         # ----- Let's go -----
         module = AtomicModule(header_one, [generic_body, box_body, another_body], [jnt, jnt_works])
+        same_module = AtomicModule(header_one, [generic_body, box_body, another_body], [jnt, jnt_works])
 
+        self.assertEqual(module, same_module)
         self.assertEqual(module.mass, generic_body.mass + box_body.mass + another_body.mass)
 
+        same_module.bodies.pop()  # Don't do this at home
+        self.assertNotEqual(module, same_module)
+
         with self.assertRaises(ValueError):
             # Joint body missing in module
             mod = AtomicModule(header_one, [generic_body], [jnt])
         with self.assertRaises(err.UniqueValueError):
             # Same connector ID for different bodies
             mod = AtomicModule(header_one, [generic_body, box_body_same_connectors])
         with self.assertRaises(err.UniqueValueError):
             mod = AtomicModule(header_one, [generic_body, box_body, jnt_fails.parent_body, jnt_fails.child_body],
                                [jnt, jnt_fails])
 
         new_joint = Joint('5', TimorJointType.revolute, parent_body=Bodies.Body('1000', collision=box),
                           child_body=Bodies.Body('1001', collision=box))
         new = AtomicModule(header_two, [generic_body, box_body, new_joint.parent_body, new_joint.child_body],
                            [jnt, new_joint])
+        self.assertNotEqual(module, new)
 
         self.assertEqual(Bodies.ConnectorSet(new.available_connectors.values()),
                          generic_body.connectors
                          .union(box_body.connectors)
                          .union(another_body.connectors)
                          )
 
@@ -218,14 +230,19 @@
         cyl_header = ModuleHeader('cylinder', 'cylinder')
         l_header = ModuleHeader('L', 'orthogonal link')
         cylinder = ParameterizedCylinderLink(cyl_header)
         l_shaped = ParameterizedOrthogonalLink(l_header, lengths=(1, 3), radius=.2)
         long_cylinder = ParameterizedCylinderLink(cyl_header, length=2)
         constrained_cylinder = ParameterizedCylinderLink(cyl_header, length=2, radius=1, limits=((.1, 1.1), (0, 4)))
 
+        self.assertEqual(cylinder, cylinder)
+        self.assertNotEqual(cylinder, l_shaped)
+        self.assertNotEqual(cylinder, long_cylinder)
+        self.assertNotEqual(cylinder, constrained_cylinder)
+
         bottom = cylinder.connectors_by_own_id['proximal']
         top = cylinder.connectors_by_own_id['distal']
         self.assertEqual(abs(bottom.body2connector.translation[2]), abs(top.body2connector.translation[2]))
         dz_initial = (bottom.connector2body @ top.body2connector).translation[2]
         self.assertEqual(abs(dz_initial), cylinder.length)
 
         initial_mass = cylinder.mass
```

### Comparing `timor-python-0.0.8/tests/test_modulesDB.py` & `timor-python-0.0.9/tests/test_modulesDB.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 
 class TestModulesDB(unittest.TestCase):
     """Test if all known good module DBs are loadable, class is working, I/O from/to json, assemblies, ..."""
 
     def setUp(self) -> None:
         """Defines the filepaths before testing"""
         self.module_set_name = 'IMPROV'
-        self.json_file, self.package_dir = get_module_db_files(self.module_set_name)
-        self.db = ModulesDB.from_file(self.json_file, package_dir=self.package_dir)
+        self.json_file = get_module_db_files(self.module_set_name)
+        self.db = ModulesDB.from_json_file(self.json_file)
         random.seed(123)
         np.random.seed(123)
 
     def test_dump_json(self):
         """Tests loading and dumping from and to json."""
-        db = ModulesDB.from_file(self.json_file, package_dir=self.package_dir)
+        db = ModulesDB.from_json_file(self.json_file)
         json_string = db.to_json_string()
-        db_two = ModulesDB.from_json_string(json_string, self.package_dir)
+        db_two = ModulesDB.from_json_string(json_string)
         json_again = db_two.to_json_string()
 
         self.assertEqual(json_string, json_again)
         self.assertEqual(db.all_module_ids, db_two.all_module_ids)
         self.assertTrue(nx.is_isomorphic(db.connectivity_graph, db_two.connectivity_graph))
 
     def test_empty(self):
@@ -40,25 +40,37 @@
         mod = AtomicModule(minimum_header)  # Header required
         mod = AtomicModule.from_json_data({'header': minimum_header.asdict()}, Path())
         assembly = ModuleAssembly.empty()
         robot = assembly.to_pin_robot()
         with self.assertRaises(LookupError):
             assembly.add_random_from_db()  # The db is empty
 
+    def test_equality(self):
+        """Test that two DBs with same modules and attributes are equal"""
+        db1 = ModulesDB.from_name('IMPROV')
+        db2 = ModulesDB.from_name('geometric_primitive_modules')
+        self.assertNotEqual(db1, db2)
+        self.assertEqual(db1, db1)
+        self.assertEqual(db2, db2)
+        self.assertFalse(db1 == ModulesDB(tuple(db1)))
+        self.assertNotEqual(db1, ModulesDB(tuple(db1)))  # Different names
+        self.assertEqual(db1, ModulesDB(tuple(db1), name=db1.name, **db1._model_generation_kwargs))
+        self.assertEqual(db2, ModulesDB(tuple(db2), name=db2.name, **db2._model_generation_kwargs))
+
     def test_load_all_from_file(self):
         for db_name, db_dir in robots.items():
             if len(tuple(db_dir.rglob('*.json'))) == 0:
                 logging.debug('Not trying to load db {} - probably not a database'.format(db_name))
                 continue  # Not a json DB file in there
             db = ModulesDB.from_name(db_name)
             self.assertGreater(len(db), 0, msg=f"{db_name} is empty after loading")
 
     def test_jointless_robot(self):
         """Test the Assembly to Robot procedure for a robot without a joint"""
-        db = ModulesDB.from_file(*get_module_db_files('geometric_primitive_modules'))
+        db = ModulesDB.from_name('geometric_primitive_modules')
         assembly = ModuleAssembly.from_serial_modules(db, ['base'] + ['l_15'] * 5)
         robot = assembly.to_pin_robot()
         self.assertEqual(robot.njoints, 0)
         self.assertAlmostEqual(robot.mass, assembly.mass)
         self.assertIsInstance(robot.fk(), Transformation)
         goal = ToleratedPose(nominal=Transformation.from_translation((9, 9, 9)))
         q, success = robot.ik(goal)
```

### Comparing `timor-python-0.0.8/tests/test_obstacle.py` & `timor-python-0.0.9/tests/test_obstacle.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,16 +18,16 @@
         Check that vertices loaded from stl are same as those in the file
 
         :return:
         """
         mesh_loader = hppfcl.MeshLoader()
         m = mesh_loader.load(str(self.demo_stl))
 
-        geometry_desc = {'type': 'mesh', 'parameters': {"file": self.demo_stl.name}}
-        obs = Obstacle.from_json_data(dict(ID='123', collision=geometry_desc, package_dir=self.demo_stl.parent))
+        geometry_desc = {'type': 'mesh', 'parameters': {"file": self.demo_stl}}
+        obs = Obstacle.from_json_data(dict(ID='123', collision=geometry_desc))
 
         with open(self.demo_stl, "rb") as f:
             header = f.read(80)
             tri_count = np.frombuffer(f.read(4), dtype=np.int32)
             _ = f.read(12)  # firstNormal
             firstVertex = np.frombuffer(f.read(12), dtype=np.float32)
             secondVertex = np.frombuffer(f.read(12), dtype=np.float32)
@@ -41,16 +41,16 @@
             self.assertEqual(tri_count, obs.collision.collision_geometry.num_tris)
             coll_geom = obs.collision.collision_geometry
             np.testing.assert_array_equal(coll_geom.vertices()[coll_geom.tri_indices(0)[0], :], firstVertex)
             np.testing.assert_array_equal(coll_geom.vertices()[coll_geom.tri_indices(0)[1], :], secondVertex)
             np.testing.assert_array_equal(coll_geom.vertices()[coll_geom.tri_indices(0)[2], :], thirdVertex)
 
     def test_visualize(self):
-        geometry_desc = [{'type': 'mesh', 'parameters': {"file": self.demo_stl.name}},
+        geometry_desc = [{'type': 'mesh', 'parameters': {"file": self.demo_stl}},
                          {'type': 'box', 'parameters': {'x': 1, 'y': 2, 'z': 3}},
                          {'type': 'cylinder', 'parameters': {'r': 2, 'z': 3}},
                          {'type': 'sphere', 'parameters': {'r': 3}}]
         for desc in (geometry_desc, *geometry_desc):  # Check composed and each individually
-            obs = Obstacle.from_json_data(dict(ID='123', collision=desc, package_dir=self.demo_stl.parent))
+            obs = Obstacle.from_json_data(dict(ID='123', collision=desc))
             vis = pin.visualize.MeshcatVisualizer()
             vis.initViewer()
             obs.visualize(vis)
```

### Comparing `timor-python-0.0.8/tests/test_robot_setup.py` & `timor-python-0.0.9/tests/test_robot_setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import random
 import unittest
 
 import numpy as np
 import numpy.testing as np_test
 import pinocchio as pin
 
+from timor.Module import ModuleAssembly, ModulesDB
 from timor.Robot import PinRobot, RobotBase
 from timor.task import Tolerance
 from timor.utilities import logging, prebuilt_robots, spatial
 from timor.utilities.file_locations import robots
 from timor.utilities.tolerated_pose import ToleratedPose
 from timor.utilities.transformation import Transformation
 
@@ -45,14 +46,24 @@
             original = robot_one.placement.homogeneous.copy()
             robot_one.move(displacement)
             robot_one.move(inverse)
             np_test.assert_array_almost_equal(original, robot_one.placement.homogeneous)
             robot_one.set_base_placement(original)  # Should change nothing
             np_test.assert_array_almost_equal(original, robot_one.placement.homogeneous)
 
+        # Test displacement for a robot built from a module
+        db = ModulesDB.from_name('geometric_primitive_modules')
+        mini_assembly = ModuleAssembly(db, ['J2'], base_connector=(0, 'J2_proximal'))
+        jnt_displacement = (Transformation(spatial.rotX(np.pi)) @
+                            db.all_connectors_by_id[('J2', 'J2_proximal', 'J2_proximal')].connector2body @
+                            list(db.by_id['J2'].joints)[0].parent2joint).homogeneous
+        mini_robot = mini_assembly.to_pin_robot(base_placement=new_placement)
+        np_test.assert_array_almost_equal(mini_robot.model.jointPlacements[1].homogeneous,
+                                          new_placement.homogeneous @ jnt_displacement)
+
     def test_empty_robot(self):
         wrapper = pin.RobotWrapper(pin.Model())
         robot = PinRobot(wrapper=wrapper)
         self.assertIsInstance(robot, RobotBase)
         self.assertEqual(robot.mass, 0)
 
     def test_multiple_base_placement(self):
@@ -173,14 +184,18 @@
 
     def test_robot_ik(self):
         wrapper = pin.RobotWrapper.BuildFromURDF(str(self.urdf), str(self.package_dir))
         robot = PinRobot(wrapper=wrapper)
         panda_tcp = pin.SE3(spatial.homogeneous(np.array([0, 0, .21]), spatial.rotZ(-np.pi / 4)[:3, :3]))
         robot.add_tcp_frame('panda_joint7', panda_tcp)
 
+        def translation_cost(_r: RobotBase, _q: np.ndarray, _g: np.ndarray):
+            """A custom cost function to optimize for translation only"""
+            return _r.fk(_q, 'tcp').distance(_g).translation_euclidean
+
         error_count = {"scipy": 0, "jacobian": 0}
         N = 100
         n = 0
         scipy_tolerance = Tolerance.CartesianXYZ.default()
         jacobian_tolerance = Tolerance.DEFAULT_SPATIAL
         fails = []
         inf_limits = np.ones_like(robot.joint_torque_limits) * np.inf
@@ -191,25 +206,25 @@
             goal = robot.fk(conf)
             if robot.has_self_collision():
                 # Don't test ik in these cases - it might fail due to avoiding self collisions
                 continue
             n += 1  # Keep track of how many examples were really worked with
             robot.model.effortLimit = inf_limits  # Make it impossible to fail due to the torque limits
             robot.update_configuration(pin.neutral(robot.model))
-            conf, success = robot.ik_scipy(ToleratedPose(goal, scipy_tolerance), check_static_torques=True)
+            conf, success = robot.ik_scipy(ToleratedPose(goal, scipy_tolerance), ik_cost_function=translation_cost)
             if success:
                 # ik_scipy optimizes only for position, therefore the Cartesian XYZ tolerance
                 self.assertTrue(scipy_tolerance.valid(goal, robot.fk(conf)))
                 self.assertTrue(max(abs(conf)) < 2 * np.pi)  # IK result should be mapped to (-2pi, 2pi)
                 self.assertFalse(robot.has_self_collision(conf))
             else:
                 error_count['scipy'] += 1
 
             robot.update_configuration(pin.neutral(robot.model))  # Prevent using the scipy result as initial guess
-            conf, success = robot.ik_jacobian(ToleratedPose(goal, jacobian_tolerance), check_static_torques=True)
+            conf, success = robot.ik_jacobian(ToleratedPose(goal, jacobian_tolerance))
             if success:
                 np_test.assert_array_almost_equal(goal.homogeneous, robot.fk(conf).homogeneous, decimal=2)
                 self.assertTrue(jacobian_tolerance.valid(goal, robot.fk(conf)))
                 self.assertTrue(max(abs(conf)) < 2 * np.pi)
                 self.assertFalse(robot.has_self_collision(conf))
             else:
                 error_count['jacobian'] += 1
@@ -268,10 +283,17 @@
 
     def test_robot_viz(self):
         wrapper = pin.RobotWrapper.BuildFromURDF(str(self.urdf), str(self.package_dir))
         robot = PinRobot(wrapper=wrapper)
         self.assertIsNotNone(robot.visualize())
         self.assertIsNotNone(robot.visualize_self_collisions())
 
+    def test_robot_manip(self):
+        robot = PinRobot.from_urdf(self.urdf, self.package_dir)
+        # Some best guess singular / non-singular panda poses
+        self.assertAlmostEqual(0., robot.manipulability_index(np.asarray((0., 0., 0., 0., 0., 0., 0.))))
+        self.assertGreater(
+            0.5, robot.manipulability_index(np.asarray((0., -np.pi / 4, 0., np.pi / 2, 0., np.pi / 2, 0.))))
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `timor-python-0.0.8/tests/test_schemas.py` & `timor-python-0.0.9/tests/test_schemas.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     def test_module_schema(self):
         _, validator = get_schema_validator(schema_dir.joinpath("ModuleSchema.json"))
 
         module_sets = []
         for module_set, robot_dir in robots.items():
             try:
-                new_set = get_module_db_files(module_set)[0]
+                new_set = get_module_db_files(module_set)
             except FileNotFoundError:
                 logging.info(f"Skipping not found module set {module_set} for schema test")
                 continue
             logging.debug(f"Testing {module_set}")
             module_sets.append(new_set)
 
         self._test_files_with_schema(validator, module_sets)
```

### Comparing `timor-python-0.0.8/tests/test_serializing_deserializing.py` & `timor-python-0.0.9/tests/test_serializing_deserializing.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+from copy import deepcopy
 import json
+import os
 from pathlib import Path
 import pickle
 import random
 import tempfile
 import unittest
 
 import hppfcl
 import numpy as np
 import numpy.testing as np_test
 import pinocchio as pin
 
 from timor import Geometry, Transformation
 from timor import Robot
+from timor.Geometry import Mesh
 from timor.Module import ModuleAssembly, ModulesDB
 from timor.task import Constraints, CostFunctions, Obstacle, Solution, Task, Tolerance
 from timor.utilities import file_locations, prebuilt_robots, logging
-from timor.utilities.file_locations import get_module_db_files, schema_dir
+from timor.utilities.file_locations import schema_dir
 from timor.utilities.prebuilt_robots import random_assembly
 from timor.utilities.schema import get_schema_validator
 from timor.utilities.tolerated_pose import ToleratedPose
 from timor.utilities.trajectory import Trajectory
 
 
 class DummyTask:
@@ -208,14 +211,63 @@
         eef_constraint_all = Constraints.EndEffector(pose=ToleratedPose(Transformation.random()),
                                                      velocity_lim=np.asarray((random.random(), random.random() + 1)),
                                                      rotation_velocity_lim=np.asarray((-random.random(),
                                                                                        random.random())))
         self.constraints = [goal_order, joint_constraints, base_placement, collision, eef_constraint_pose,
                             eef_constraint_v, eef_constraint_all]
 
+    def test_modules_db_serialized(self):
+        """Tests if all modules dbs can be serialized and deserialized"""
+        for db_name in ('IMPROV', 'PROMODULAR', 'modrob-gen2'):
+            logging.debug(f"Testing with {db_name}")
+            db = ModulesDB.from_name(db_name)
+            self.assertEqual(db.name, db_name)  # Ensure name correctly inferred from path
+            for m in db:
+                pickle_mod = pickle.loads(pickle.dumps(m))
+                deepcopy_mod = deepcopy(m)
+                self.assertEqual(m, pickle_mod)
+                self.assertEqual(m, deepcopy_mod)
+            db_json = db.to_json_data()
+            new_db = ModulesDB.from_json_data(db_json)
+            new_db._name = db.name
+            self.assertEqual(db, new_db)
+            deep_copy_db = deepcopy(db)
+            self.assertEqual(db, deep_copy_db)
+            s = pickle.dumps(db)
+            pickle_db = pickle.loads(s)
+            self.assertEqual(db, pickle_db)
+
+            # Test different to_json_file modes
+            with tempfile.TemporaryDirectory() as tmp_dir:
+                os.makedirs(Path(tmp_dir, db.name), exist_ok=True)
+                db_file = Path(tmp_dir, f"{db.name}/modules.json")
+                # Broken - error as not existent file
+                with self.assertRaises(FileNotFoundError):
+                    db.to_json_file(db_file, handle_missing_assets='error')
+                # Broken - no copy
+                db.to_json_file(db_file, handle_missing_assets="warning")
+                with self.assertRaises(FileNotFoundError):
+                    new_db = ModulesDB.from_json_file(db_file)
+                # Broken - no copy
+                db.to_json_file(db_file, handle_missing_assets='ignore')
+                with self.assertRaises(FileNotFoundError):
+                    new_db = ModulesDB.from_json_file(db_file)
+                # Should work with copy
+                db.to_json_file(db_file, handle_missing_assets='copy')
+                new_db = ModulesDB.from_json_file(db_file)
+                # self.assertTrue(equivalent_set(db, new_db, equivalent_module))  # Other filepath -> not same geometry
+
+            with tempfile.TemporaryDirectory() as tmp_dir:  # Cleanup copied files
+                os.makedirs(Path(tmp_dir, db.name), exist_ok=True)
+                db_file = Path(tmp_dir, f"{db.name}/modules.json")
+                # Should work with symlink
+                db.to_json_file(db_file, handle_missing_assets='symlink')
+                new_db = ModulesDB.from_json_file(db_file)
+                # self.assertTrue(equivalent_set(db, new_db, equivalent_module))  # Other filepath -> not same geometry
+
     def test_assembly_to_serialized(self):
         """Tests both, assembly to pickle and to json"""
         for db_name in ('IMPROV', 'PROMODULAR', 'modrob-gen2'):
             logging.debug(f"Testing with {db_name}")
             db = ModulesDB.from_name(db_name)
             for _ in range(3):
                 assembly = random_assembly(6, db)
@@ -248,26 +300,33 @@
                 pin_models_functionally_equal(robot.model, reconstructed_robot.model)
                 robot_io_equal(robot, reconstructed_robot)
                 pin_geometry_models_structurally_equal(robot.visual, reconstructed_robot.visual)
                 pin_geometry_models_structurally_equal(robot.collision, reconstructed_robot.collision)
                 pin_geometry_models_functionally_equal(robot, reconstructed_robot)
 
     def test_assembly_to_urdf(self):
-        _, db_assets = file_locations.get_module_db_files('IMPROV')
+        db_file = file_locations.get_module_db_files('IMPROV')
         db = ModulesDB.from_name('IMPROV')
         for _ in range(5):
             assembly = prebuilt_robots.random_assembly(n_joints=6, module_db=db)
             logging.info(f"Testing assembly {assembly.internal_module_ids}")
 
             r1 = assembly.to_pin_robot()
             r1._remove_home_collisions()  # This is done per default when loading from URDF
-            with tempfile.NamedTemporaryFile() as tmp_urdf:
-                urdf = assembly.to_urdf('test_robot', Path(tmp_urdf.name), replace_wrl=True)
-                tmp_urdf.flush()
-                r2 = Robot.PinRobot.from_urdf(Path(tmp_urdf.name), db_assets)
+            with tempfile.TemporaryDirectory() as tmp_dir:
+                tmp_urdf = Path(tmp_dir, 'test.urdf')
+                urdf = assembly.to_urdf('test_robot', Path(tmp_urdf),
+                                        replace_wrl=True, handle_missing_assets="warning")
+                with self.assertRaises(ValueError):
+                    Robot.PinRobot.from_urdf(Path(tmp_urdf), tmp_urdf.parent)
+                with self.assertRaises(FileNotFoundError):
+                    assembly.to_urdf('test_robot', Path(tmp_urdf), replace_wrl=True, handle_missing_assets="error")
+                urdf = assembly.to_urdf('test_robot', Path(tmp_urdf),
+                                        replace_wrl=True, handle_missing_assets="symlink")
+                r2 = Robot.PinRobot.from_urdf(Path(tmp_urdf), tmp_urdf.parent)
                 self.assertTrue(pin_models_functionally_equal(r1.model, r2.model))
                 self.assertLess(pin_geometry_models_functionally_equal(r1, r2), 0.01,
                                 msg=f"Varying self-collisions for assembly {assembly}")
                 self.assertTrue(pin_geometry_models_structurally_equal(r1.visual, r2.visual))
 
     def test_constraints_to_json(self):
         with self.assertRaises(KeyError):
@@ -323,53 +382,72 @@
             base_pose=assembly.robot.placement
         )
 
         solution_dict = solution.to_json_data()
         self.assertIsNotNone(json.dumps(solution_dict))
         self.assertIsNotNone(pickle.dumps(solution_dict))
         _, validator = get_schema_validator(schema_dir.joinpath("SolutionSchema.json"))
+        deserialized_sol = Solution.SolutionBase.from_json_data(solution_dict, {task.id: task})
+        deepcopy_sol = deepcopy(solution)
+        pickle_sol = pickle.loads(pickle.dumps(solution))
+
         # make sure is storable
         with tempfile.NamedTemporaryFile(mode="w+") as t:
             json.dump(solution_dict, t)
             t.flush()
             with open(t.name) as f:
                 validator.validate(json.load(f))
-            loaded_sol = Solution.SolutionBase.from_json_file(Path(t.name), Path("/"), {task.id: task})
+            loaded_sol = Solution.SolutionBase.from_json_file(Path(t.name), {task.id: task})
 
         # Also check the custom task
-        with tempfile.NamedTemporaryFile(mode="w+") as t:
-            task.to_json_file(t.name)
-            t.flush()
+        with tempfile.TemporaryDirectory() as t:
+            task.to_json_file(Path(t))
+            with self.assertRaises(ValueError):
+                task.to_json_file(Path(t).joinpath(f"{task.id}_5.json"))
 
-        self.assertEqual(solution.valid, loaded_sol.valid)
-        # Depends on robot, trajectory, position, cost function -> most important parts of solution tested
-        self.assertEqual(solution.cost, loaded_sol.cost)
-        self.assertEqual(solution.trajectory, loaded_sol.trajectory)
-        self.assertEqual(solution.header, loaded_sol.header)
+        for sol in (deserialized_sol, deepcopy_sol, pickle_sol, loaded_sol):
+            self.assertEqual(solution.valid, sol.valid)
+            # Depends on robot, trajectory, position, cost function -> most important parts of solution tested
+            self.assertEqual(solution.cost, sol.cost)
+            self.assertEqual(solution.trajectory, sol.trajectory)
+            self.assertEqual(solution.header, sol.header)
 
         with tempfile.NamedTemporaryFile(mode="w+") as t:
             json.dump({"test": "json_validator"}, t)
             t.flush()
             with self.assertRaises(ValueError):
-                Solution.SolutionBase.from_json_file(Path(t.name), Path("/"), {task.id: task})
+                Solution.SolutionBase.from_json_file(Path(t.name), {task.id: task})
 
     def test_load_then_dump_task(self):
         for task_file in self.task_files:
-            task = Task.Task.from_json_file(task_file, self.assets)
-
-            with tempfile.NamedTemporaryFile() as tmp_json_dump:
-                task.to_json_file(Path(tmp_json_dump.name))
-                tmp_json_dump.flush()  # Necessary to certainly write to tempfile!
-                another_copy = Task.Task.from_json_file(Path(tmp_json_dump.name), self.assets)
+            task = Task.Task.from_json_file(task_file)
+            self.assertEqual(task, deepcopy(task))
+            self.assertEqual(task, pickle.loads(pickle.dumps(task)))
+            self.assertEqual(task, Task.Task.from_json_data(task.to_json_data()))
+
+            with tempfile.TemporaryDirectory() as tmp_dir:
+                tmp_json_file = Path(tmp_dir).joinpath(f"{task.id}.json")
+                if any(isinstance(o.visual, Mesh) for o in task.obstacles) or \
+                   any(isinstance(o.collision, Mesh) for o in task.obstacles):
+                    with self.assertRaises(FileNotFoundError):
+                        task.to_json_file(tmp_dir, handle_missing_assets="error")
+                    task.to_json_file(tmp_dir, handle_missing_assets="warning")
+                    self.assertTrue(tmp_json_file.exists())
+                    with self.assertRaises(FileNotFoundError):
+                        Task.Task.from_json_file(tmp_json_file)
+                    task.to_json_file(tmp_dir, handle_missing_assets="ignore")
+                    self.assertTrue(tmp_json_file.exists())
+                    with self.assertRaises(FileNotFoundError):
+                        Task.Task.from_json_file(tmp_json_file)
+
+                task.to_json_file(Path(tmp_dir), handle_missing_assets="copy")
+                self.assertTrue(tmp_json_file.exists())
+                another_copy = Task.Task.from_json_file(tmp_json_file, self.assets)
                 # This does not test 100% for equality but should cover the most central sanity checks
-                self.assertEqual(task.header, another_copy.header)
-                self.assertEqual(set(o.id for o in task.obstacles), set(o.id for o in another_copy.obstacles))
-                self.assertEqual(set(g.id for g in task.goals), set(g.id for g in another_copy.goals))
-                self.assertEqual(set(type(c) for c in task.constraints),
-                                 set(type(c) for c in another_copy.constraints))
+                self.assertEqual(task, another_copy)
 
     def test_pickle_robot(self):
         """Tests whether the kinematic model remains when pickling - geometry cannot be preserved at the moment"""
         pickled = pickle.dumps(self.robot)
         unpickled = pickle.loads(pickled)
         self.assertTrue(pin_models_functionally_equal(self.robot.model, unpickled.model))
 
@@ -462,33 +540,33 @@
         self.assertTrue(pin_models_functionally_equal(modular.model, as_assembly.robot.model))
         self.assertTrue(robot_io_equal(panda, fresh_robot))
         self.assertLess(pin_geometry_models_functionally_equal(modular, as_assembly.robot, iterations=1000), 0.01)
         self.assertTrue(pin_geometry_models_structurally_equal(modular.visual, as_assembly.robot.visual))
 
         # Test with more complex modular robot that also has joint inertias / friction / ...
         modular_complex = ModuleAssembly.from_serial_modules(
-            ModulesDB.from_file(*get_module_db_files('IMPROV')),
+            ModulesDB.from_name('IMPROV'),
             ["1", "21", "14", "21", "14", "23", "13"]
         ).robot
         fresh_robot = ModuleAssembly.from_monolithic_robot(modular_complex).robot
         self.assertTrue(pin_models_functionally_equal(modular_complex.model, fresh_robot.model))
         self.assertTrue(robot_io_equal(modular_complex, fresh_robot))
         self.assertLess(pin_geometry_models_functionally_equal(modular_complex, fresh_robot, iterations=1000), 0.01)
         self.assertTrue(pin_geometry_models_structurally_equal(modular_complex.visual, fresh_robot.visual))
 
     def test_urdf2json(self):
-        assembly = ModuleAssembly.from_monolithic_robot(self.robot, self.panda_urdf)
+        assembly = ModuleAssembly.from_monolithic_robot(self.robot)
         db_data = assembly.db.to_json_data()
-        reconstructed_db = ModulesDB.from_json_data(db_data, self.panda_assets, "panda")
+        reconstructed_db = ModulesDB.from_json_data(db_data, "panda")
         assembly_from_json = ModuleAssembly.from_serial_modules(reconstructed_db, ("panda",))
-        with tempfile.NamedTemporaryFile() as f:
-            assembly.to_urdf(write_to=Path(f.name))
-            f.flush()
+        with tempfile.TemporaryDirectory() as d:
+            urdf_file = Path(d, "panda.urdf")
+            assembly.to_urdf(write_to=urdf_file, handle_missing_assets="symlink")
             assembly_from_urdf = ModuleAssembly.from_monolithic_robot(
-                Robot.PinRobot.from_urdf(Path(f.name), self.panda_assets))
+                Robot.PinRobot.from_urdf(urdf_file, urdf_file.parent))
 
         for recreated_assembly in (assembly_from_json, assembly_from_urdf):
             self.assertTrue(pin_models_functionally_equal(self.robot.model, recreated_assembly.robot.model))
             self.assertTrue(robot_io_equal(self.robot, recreated_assembly.robot))
             self.assertTrue(pin_geometry_models_structurally_equal(self.robot.visual, recreated_assembly.robot.visual))
             self.assertLess(pin_geometry_models_functionally_equal(self.robot, recreated_assembly.robot, 1000), 0.01)
```

### Comparing `timor-python-0.0.8/tests/test_spatial_projections.py` & `timor-python-0.0.9/tests/test_spatial_projections.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/tests/test_task_solutions.py` & `timor-python-0.0.9/tests/test_task_solutions.py`

 * *Files 2% similar despite different names*

```diff
@@ -342,14 +342,21 @@
 
         # So here is our (invalid) solution
         random_solution = Solution.SolutionTrajectory(random_trajectory,
                                                       self.solution_header,
                                                       task,
                                                       ModuleAssembly.from_monolithic_robot(self.robot),
                                                       cost_whitman)
+
+        random_solution.plot(show_figure=False)
+        random_solution.plot(["q", "dq", "ddq", "tau", "manipulablility", "eef_position", "eef_rotation"],
+                             show_figure=False)
+        random_solution.plot(["q", "dq", "ddq", "tau", "manipulablility", "eef_position", "eef_rotation"],
+                             show_figure=False, subplot_kwargs={"facecolor": "black"})  # Check propagation of kwargs
+
         random_solution_without_all_goals = Solution.SolutionTrajectory(
             random_trajectory, self.solution_header, task_without_all_goals,
             ModuleAssembly.from_monolithic_robot(self.robot), cost_whitman)
 
         # Make sure lazy variables are not evaluated without explicitly calling them
         self.assertIsNone(random_solution._valid.value)
         self.assertIsNone(random_solution._cost.value)
```

### Comparing `timor-python-0.0.8/tests/test_tolerances.py` & `timor-python-0.0.9/tests/test_tolerances.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/tests/test_trajectory.py` & `timor-python-0.0.9/tests/test_trajectory.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/tests/test_transformations.py` & `timor-python-0.0.9/tests/test_transformations.py`

 * *Files identical despite different names*

### Comparing `timor-python-0.0.8/tests/test_volume.py` & `timor-python-0.0.9/tests/test_volume.py`

 * *Files identical despite different names*

