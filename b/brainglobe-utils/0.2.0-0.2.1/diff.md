# Comparing `tmp/brainglobe-utils-0.2.0.tar.gz` & `tmp/brainglobe-utils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainglobe-utils-0.2.0.tar", last modified: Fri Jun 23 10:54:54 2023, max compression
+gzip compressed data, was "brainglobe-utils-0.2.1.tar", last modified: Fri Jun 23 11:01:01 2023, max compression
```

## Comparing `brainglobe-utils-0.2.0.tar` & `brainglobe-utils-0.2.1.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.189634 brainglobe-utils-0.2.0/.github/
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.189634 brainglobe-utils-0.2.0/.github/workflows/
--rw-rw-r--   0 adam      (1001) adam      (1001)     1405 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/.github/workflows/test_and_deploy.yml
--rw-rw-r--   0 adam      (1001) adam      (1001)     1311 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/.gitignore
--rw-rw-r--   0 adam      (1001) adam      (1001)      834 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/.pre-commit-config.yaml
--rw-rw-r--   0 adam      (1001) adam      (1001)     1067 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/LICENSE
--rw-rw-r--   0 adam      (1001) adam      (1001)     1088 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1001)       75 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.189634 brainglobe-utils-0.2.0/brainglobe_utils.egg-info/
--rw-rw-r--   0 adam      (1001) adam      (1001)     1088 2023-06-23 10:54:54.000000 brainglobe-utils-0.2.0/brainglobe_utils.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1001)     3526 2023-06-23 10:54:54.000000 brainglobe-utils-0.2.0/brainglobe_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1001)        1 2023-06-23 10:54:54.000000 brainglobe-utils-0.2.0/brainglobe_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1001)      169 2023-06-23 10:54:54.000000 brainglobe-utils-0.2.0/brainglobe_utils.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1001)        1 2023-06-23 10:54:54.000000 brainglobe-utils-0.2.0/brainglobe_utils.egg-info/top_level.txt
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.189634 brainglobe-utils-0.2.0/imlib/
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.189634 brainglobe-utils-0.2.0/imlib/IO/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/IO/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     7448 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/imlib/IO/cells.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      662 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/IO/surfaces.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      519 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/IO/yaml.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      208 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/imlib/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.189634 brainglobe-utils-0.2.0/imlib/array/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/array/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      676 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/array/filter.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     1208 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/array/fit.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      829 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/array/locate.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      548 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/array/math.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     3352 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/array/misc.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      759 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/array/size.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.189634 brainglobe-utils-0.2.0/imlib/cells/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/cells/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1001)    11340 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/imlib/cells/cells.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     2032 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/imlib/cells/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.189634 brainglobe-utils-0.2.0/imlib/general/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/general/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      232 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/general/config.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      529 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/general/exceptions.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     1518 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/general/list.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      283 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/general/logging.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     2414 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/general/numerical.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     1731 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/general/parsing.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      342 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/general/pathlib.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      973 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/general/string.py
--rw-rw-r--   0 adam      (1001) adam      (1001)    12492 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/imlib/general/system.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/imlib/image/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/image/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      491 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/image/binning.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      948 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/image/masking.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     1283 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/image/objects.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      725 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/image/orient.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      626 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/image/scale.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      927 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/image/shape.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      590 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/image/size.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/imlib/math/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/math/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      782 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/math/trig.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/imlib/pandas/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/pandas/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     1496 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/imlib/pandas/misc.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      313 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/imlib/pandas/query.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     2244 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/pyproject.toml
--rw-rw-r--   0 adam      (1001) adam      (1001)       38 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/setup.cfg
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/tests/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.189634 brainglobe-utils-0.2.0/tests/data/
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.189634 brainglobe-utils-0.2.0/tests/data/IO/
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/tests/data/IO/roi_sorter_output/
--rwxrwxr-x   0 adam      (1001) adam      (1001)      182 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/IO/roi_sorter_output/Cell_220396_z358_y564_x4056
--rwxrwxr-x   0 adam      (1001) adam      (1001)      182 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/IO/roi_sorter_output/Cell_220422_z367_y677_x4395
--rwxrwxr-x   0 adam      (1001) adam      (1001)      182 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/IO/roi_sorter_output/Cell_220621_z439_y735_x4351
--rwxrwxr-x   0 adam      (1001) adam      (1001)      182 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/IO/roi_sorter_output/Cell_221379_z570_y267_x3989
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/tests/data/cells/
--rw-rw-r--   0 adam      (1001) adam      (1001)     8510 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cells/cells.xml
--rw-rw-r--   0 adam      (1001) adam      (1001)    17610 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/data/cells/cells.yml
--rw-rw-r--   0 adam      (1001) adam      (1001)   102915 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cells/cells_two_types.xml
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.189634 brainglobe-utils-0.2.0/tests/data/cube_extract/
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/tests/data/cube_extract/cubes/
--rw-rw-r--   0 adam      (1001) adam      (1001)   103946 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cube_extract/cubes/pCellz10y522x392Ch0.tif
--rw-rw-r--   0 adam      (1001) adam      (1001)   103946 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cube_extract/cubes/pCellz10y522x392Ch1.tif
--rw-rw-r--   0 adam      (1001) adam      (1001)   103946 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cube_extract/cubes/pCellz15y1004x340Ch0.tif
--rw-rw-r--   0 adam      (1001) adam      (1001)   103946 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cube_extract/cubes/pCellz15y1004x340Ch1.tif
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/tests/data/cubes/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cubes/pCellz222y2805x9962Ch1.tif
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cubes/pCellz222y2805x9962Ch2.tif
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cubes/pCellz258y3892x10559Ch1.tif
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cubes/pCellz258y3892x10559Ch2.tif
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cubes/pCellz413y2308x9391Ch1.tif
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cubes/pCellz413y2308x9391Ch2.tif
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cubes/pCellz416y2503x5997Ch1.tif
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cubes/pCellz416y2503x5997Ch2.tif
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cubes/pCellz418y5457x9489Ch1.tif
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cubes/pCellz418y5457x9489Ch2.tif
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cubes/pCellz433y4425x7552Ch1.tif
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/cubes/pCellz433y4425x7552Ch2.tif
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/tests/data/general/
--rw-rw-r--   0 adam      (1001) adam      (1001)     1032 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/data/general/jabberwocky.txt
--rw-rw-r--   0 adam      (1001) adam      (1001)      942 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/data/general/jabberwocky_sorted.txt
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/tests/data/yaml/
--rw-rw-r--   0 adam      (1001) adam      (1001)      110 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/data/yaml/single_section.yml
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/tests/tests/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/tests/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/tests/tests/test_unit/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/__init__.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/tests/tests/test_unit/test_IO/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_IO/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     4264 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_IO/test_cell_io.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      842 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_IO/test_yaml_io.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/tests/tests/test_unit/test_array/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_array/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      487 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_array/test_array_misc.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/tests/tests/test_unit/test_cells/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_cells/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     1150 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_cells/test_cell_utils.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     1784 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_cells/test_cells.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/tests/tests/test_unit/test_general/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_general/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      487 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_general/test_list.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     1383 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_general/test_numerical.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     1516 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_general/test_string.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     3998 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_general/test_system.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/tests/tests/test_unit/test_image/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_image/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      569 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_image/test_binning.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      762 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_image/test_masking.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     1710 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_image/test_objects.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      513 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_image/test_scale.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      561 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_image/test_shape.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      766 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_image/test_size.py
-drwxrwxr-x   0 adam      (1001) adam      (1001)        0 2023-06-23 10:54:54.193634 brainglobe-utils-0.2.0/tests/tests/test_unit/test_pandas/
--rw-rw-r--   0 adam      (1001) adam      (1001)        0 2023-06-23 10:23:21.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_pandas/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1001)     1068 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_pandas/test_pandas_misc.py
--rw-rw-r--   0 adam      (1001) adam      (1001)      358 2023-06-23 10:51:24.000000 brainglobe-utils-0.2.0/tests/tests/test_unit/test_pandas/test_pandas_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.310885 brainglobe-utils-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.294884 brainglobe-utils-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.294884 brainglobe-utils-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-23 11:01:01.310885 brainglobe-utils-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.298884 brainglobe-utils-0.2.1/brainglobe_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-23 11:01:01.000000 brainglobe-utils-0.2.1/brainglobe_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-23 11:01:01.000000 brainglobe-utils-0.2.1/brainglobe_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:01:01.000000 brainglobe-utils-0.2.1/brainglobe_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-23 11:01:01.000000 brainglobe-utils-0.2.1/brainglobe_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:01:01.000000 brainglobe-utils-0.2.1/brainglobe_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.298884 brainglobe-utils-0.2.1/imlib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.298884 brainglobe-utils-0.2.1/imlib/IO/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/IO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/IO/cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/IO/surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/IO/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.298884 brainglobe-utils-0.2.1/imlib/array/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/array/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/array/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/array/locate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/array/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/array/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/array/size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.298884 brainglobe-utils-0.2.1/imlib/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/cells/cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/cells/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.298884 brainglobe-utils-0.2.1/imlib/general/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/general/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/general/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/general/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/general/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/general/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/general/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/general/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/general/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12492 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/general/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.302884 brainglobe-utils-0.2.1/imlib/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/image/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/image/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/image/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/image/orient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/image/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/image/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/image/size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.302884 brainglobe-utils-0.2.1/imlib/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/math/trig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.302884 brainglobe-utils-0.2.1/imlib/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/pandas/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/imlib/pandas/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 11:01:01.310885 brainglobe-utils-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.302884 brainglobe-utils-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.294884 brainglobe-utils-0.2.1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.294884 brainglobe-utils-0.2.1/tests/data/IO/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.302884 brainglobe-utils-0.2.1/tests/data/IO/roi_sorter_output/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/IO/roi_sorter_output/Cell_220396_z358_y564_x4056
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/IO/roi_sorter_output/Cell_220422_z367_y677_x4395
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/IO/roi_sorter_output/Cell_220621_z439_y735_x4351
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/IO/roi_sorter_output/Cell_221379_z570_y267_x3989
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.302884 brainglobe-utils-0.2.1/tests/data/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cells/cells.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    17610 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cells/cells.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   102915 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cells/cells_two_types.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.294884 brainglobe-utils-0.2.1/tests/data/cube_extract/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.302884 brainglobe-utils-0.2.1/tests/data/cube_extract/cubes/
+-rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cube_extract/cubes/pCellz10y522x392Ch0.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cube_extract/cubes/pCellz10y522x392Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cube_extract/cubes/pCellz15y1004x340Ch0.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cube_extract/cubes/pCellz15y1004x340Ch1.tif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.306885 brainglobe-utils-0.2.1/tests/data/cubes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cubes/pCellz222y2805x9962Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cubes/pCellz222y2805x9962Ch2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cubes/pCellz258y3892x10559Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cubes/pCellz258y3892x10559Ch2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cubes/pCellz413y2308x9391Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cubes/pCellz413y2308x9391Ch2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cubes/pCellz416y2503x5997Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cubes/pCellz416y2503x5997Ch2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cubes/pCellz418y5457x9489Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cubes/pCellz418y5457x9489Ch2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cubes/pCellz433y4425x7552Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/cubes/pCellz433y4425x7552Ch2.tif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.306885 brainglobe-utils-0.2.1/tests/data/general/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/general/jabberwocky.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/general/jabberwocky_sorted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.306885 brainglobe-utils-0.2.1/tests/data/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/data/yaml/single_section.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.306885 brainglobe-utils-0.2.1/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.306885 brainglobe-utils-0.2.1/tests/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.306885 brainglobe-utils-0.2.1/tests/tests/test_unit/test_IO/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_IO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_IO/test_cell_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_IO/test_yaml_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.306885 brainglobe-utils-0.2.1/tests/tests/test_unit/test_array/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_array/test_array_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.306885 brainglobe-utils-0.2.1/tests/tests/test_unit/test_cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_cells/test_cell_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_cells/test_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.306885 brainglobe-utils-0.2.1/tests/tests/test_unit/test_general/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_general/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_general/test_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_general/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_general/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.310885 brainglobe-utils-0.2.1/tests/tests/test_unit/test_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_image/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_image/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_image/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_image/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_image/test_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_image/test_size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:01:01.310885 brainglobe-utils-0.2.1/tests/tests/test_unit/test_pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_pandas/test_pandas_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-23 11:00:50.000000 brainglobe-utils-0.2.1/tests/tests/test_unit/test_pandas/test_pandas_query.py
```

### Comparing `brainglobe-utils-0.2.0/.github/workflows/test_and_deploy.yml` & `brainglobe-utils-0.2.1/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/.gitignore` & `brainglobe-utils-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/.pre-commit-config.yaml` & `brainglobe-utils-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/LICENSE` & `brainglobe-utils-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/PKG-INFO` & `brainglobe-utils-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: Shared general purpose tools for the BrainGlobe project
 Author-email: Adam Tyson <code@adamltyson.com>
 License: MIT
 Project-URL: homepage, https://brainglobe.info
 Project-URL: bug_tracker, https://github.com/brainglobe/brainglobe-utils/issues
 Project-URL: source_code, https://github.com/brainglobe/brainglobe-utils
 Project-URL: user_support, https://github.com/brainglobe/brainglobe-utils/issues
```

### Comparing `brainglobe-utils-0.2.0/brainglobe_utils.egg-info/PKG-INFO` & `brainglobe-utils-0.2.1/brainglobe_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: Shared general purpose tools for the BrainGlobe project
 Author-email: Adam Tyson <code@adamltyson.com>
 License: MIT
 Project-URL: homepage, https://brainglobe.info
 Project-URL: bug_tracker, https://github.com/brainglobe/brainglobe-utils/issues
 Project-URL: source_code, https://github.com/brainglobe/brainglobe-utils
 Project-URL: user_support, https://github.com/brainglobe/brainglobe-utils/issues
```

### Comparing `brainglobe-utils-0.2.0/brainglobe_utils.egg-info/SOURCES.txt` & `brainglobe-utils-0.2.1/brainglobe_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/IO/cells.py` & `brainglobe-utils-0.2.1/imlib/IO/cells.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/IO/surfaces.py` & `brainglobe-utils-0.2.1/imlib/IO/surfaces.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/IO/yaml.py` & `brainglobe-utils-0.2.1/imlib/IO/yaml.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/array/filter.py` & `brainglobe-utils-0.2.1/imlib/array/filter.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/array/fit.py` & `brainglobe-utils-0.2.1/imlib/array/fit.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/array/locate.py` & `brainglobe-utils-0.2.1/imlib/array/locate.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/array/math.py` & `brainglobe-utils-0.2.1/imlib/array/math.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/array/misc.py` & `brainglobe-utils-0.2.1/imlib/array/misc.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/array/size.py` & `brainglobe-utils-0.2.1/imlib/array/size.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/cells/cells.py` & `brainglobe-utils-0.2.1/imlib/cells/cells.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/cells/utils.py` & `brainglobe-utils-0.2.1/imlib/cells/utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/general/exceptions.py` & `brainglobe-utils-0.2.1/imlib/general/exceptions.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/general/list.py` & `brainglobe-utils-0.2.1/imlib/general/list.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/general/numerical.py` & `brainglobe-utils-0.2.1/imlib/general/numerical.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/general/parsing.py` & `brainglobe-utils-0.2.1/imlib/general/parsing.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/general/string.py` & `brainglobe-utils-0.2.1/imlib/general/string.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/general/system.py` & `brainglobe-utils-0.2.1/imlib/general/system.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/image/masking.py` & `brainglobe-utils-0.2.1/imlib/image/masking.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/image/objects.py` & `brainglobe-utils-0.2.1/imlib/image/objects.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/image/orient.py` & `brainglobe-utils-0.2.1/imlib/image/orient.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/image/scale.py` & `brainglobe-utils-0.2.1/imlib/image/scale.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/image/shape.py` & `brainglobe-utils-0.2.1/imlib/image/shape.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/image/size.py` & `brainglobe-utils-0.2.1/imlib/image/size.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/math/trig.py` & `brainglobe-utils-0.2.1/imlib/math/trig.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/imlib/pandas/misc.py` & `brainglobe-utils-0.2.1/imlib/pandas/misc.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/pyproject.toml` & `brainglobe-utils-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/data/cells/cells.xml` & `brainglobe-utils-0.2.1/tests/data/cells/cells.xml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/data/cells/cells.yml` & `brainglobe-utils-0.2.1/tests/data/cells/cells.yml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/data/cells/cells_two_types.xml` & `brainglobe-utils-0.2.1/tests/data/cells/cells_two_types.xml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/data/cube_extract/cubes/pCellz10y522x392Ch0.tif` & `brainglobe-utils-0.2.1/tests/data/cube_extract/cubes/pCellz10y522x392Ch0.tif`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/data/cube_extract/cubes/pCellz10y522x392Ch1.tif` & `brainglobe-utils-0.2.1/tests/data/cube_extract/cubes/pCellz10y522x392Ch1.tif`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/data/cube_extract/cubes/pCellz15y1004x340Ch0.tif` & `brainglobe-utils-0.2.1/tests/data/cube_extract/cubes/pCellz15y1004x340Ch0.tif`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/data/cube_extract/cubes/pCellz15y1004x340Ch1.tif` & `brainglobe-utils-0.2.1/tests/data/cube_extract/cubes/pCellz15y1004x340Ch1.tif`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/data/general/jabberwocky.txt` & `brainglobe-utils-0.2.1/tests/data/general/jabberwocky.txt`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/data/general/jabberwocky_sorted.txt` & `brainglobe-utils-0.2.1/tests/data/general/jabberwocky_sorted.txt`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/tests/test_unit/test_IO/test_cell_io.py` & `brainglobe-utils-0.2.1/tests/tests/test_unit/test_IO/test_cell_io.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/tests/test_unit/test_IO/test_yaml_io.py` & `brainglobe-utils-0.2.1/tests/tests/test_unit/test_IO/test_yaml_io.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/tests/test_unit/test_cells/test_cell_utils.py` & `brainglobe-utils-0.2.1/tests/tests/test_unit/test_cells/test_cell_utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/tests/test_unit/test_cells/test_cells.py` & `brainglobe-utils-0.2.1/tests/tests/test_unit/test_cells/test_cells.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/tests/test_unit/test_general/test_numerical.py` & `brainglobe-utils-0.2.1/tests/tests/test_unit/test_general/test_numerical.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/tests/test_unit/test_general/test_string.py` & `brainglobe-utils-0.2.1/tests/tests/test_unit/test_general/test_string.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/tests/test_unit/test_general/test_system.py` & `brainglobe-utils-0.2.1/tests/tests/test_unit/test_general/test_system.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/tests/test_unit/test_image/test_binning.py` & `brainglobe-utils-0.2.1/tests/tests/test_unit/test_image/test_binning.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/tests/test_unit/test_image/test_masking.py` & `brainglobe-utils-0.2.1/tests/tests/test_unit/test_image/test_masking.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/tests/test_unit/test_image/test_objects.py` & `brainglobe-utils-0.2.1/tests/tests/test_unit/test_image/test_objects.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/tests/test_unit/test_image/test_scale.py` & `brainglobe-utils-0.2.1/tests/tests/test_unit/test_image/test_scale.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/tests/test_unit/test_image/test_shape.py` & `brainglobe-utils-0.2.1/tests/tests/test_unit/test_image/test_shape.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/tests/test_unit/test_image/test_size.py` & `brainglobe-utils-0.2.1/tests/tests/test_unit/test_image/test_size.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.0/tests/tests/test_unit/test_pandas/test_pandas_misc.py` & `brainglobe-utils-0.2.1/tests/tests/test_unit/test_pandas/test_pandas_misc.py`

 * *Files identical despite different names*
