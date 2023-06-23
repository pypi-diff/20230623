# Comparing `tmp/brainglobe-utils-0.2.2.tar.gz` & `tmp/brainglobe-utils-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainglobe-utils-0.2.2.tar", last modified: Fri Jun 23 11:04:20 2023, max compression
+gzip compressed data, was "brainglobe-utils-0.2.3.tar", last modified: Fri Jun 23 11:25:50 2023, max compression
```

## Comparing `brainglobe-utils-0.2.2.tar` & `brainglobe-utils-0.2.3.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.098423 brainglobe-utils-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.074422 brainglobe-utils-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.078423 brainglobe-utils-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-23 11:04:20.098423 brainglobe-utils-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.078423 brainglobe-utils-0.2.2/brainglobe_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-23 11:04:20.000000 brainglobe-utils-0.2.2/brainglobe_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-23 11:04:20.000000 brainglobe-utils-0.2.2/brainglobe_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:04:20.000000 brainglobe-utils-0.2.2/brainglobe_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-23 11:04:20.000000 brainglobe-utils-0.2.2/brainglobe_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:04:20.000000 brainglobe-utils-0.2.2/brainglobe_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.078423 brainglobe-utils-0.2.2/imlib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.078423 brainglobe-utils-0.2.2/imlib/IO/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/IO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/IO/cells.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/IO/surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/IO/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.082423 brainglobe-utils-0.2.2/imlib/array/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/array/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/array/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/array/locate.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/array/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/array/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/array/size.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.082423 brainglobe-utils-0.2.2/imlib/cells/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/cells/cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/cells/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.086423 brainglobe-utils-0.2.2/imlib/general/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/general/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/general/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/general/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/general/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/general/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/general/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/general/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/general/string.py
--rw-r--r--   0 runner    (1001) docker     (123)    12492 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/general/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.086423 brainglobe-utils-0.2.2/imlib/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/image/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/image/masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/image/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/image/orient.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/image/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/image/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/image/size.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.086423 brainglobe-utils-0.2.2/imlib/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/math/trig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.086423 brainglobe-utils-0.2.2/imlib/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/pandas/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/imlib/pandas/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 11:04:20.098423 brainglobe-utils-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.086423 brainglobe-utils-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.074422 brainglobe-utils-0.2.2/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.074422 brainglobe-utils-0.2.2/tests/data/IO/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.086423 brainglobe-utils-0.2.2/tests/data/IO/roi_sorter_output/
--rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/IO/roi_sorter_output/Cell_220396_z358_y564_x4056
--rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/IO/roi_sorter_output/Cell_220422_z367_y677_x4395
--rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/IO/roi_sorter_output/Cell_220621_z439_y735_x4351
--rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/IO/roi_sorter_output/Cell_221379_z570_y267_x3989
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.090423 brainglobe-utils-0.2.2/tests/data/cells/
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cells/cells.xml
--rw-r--r--   0 runner    (1001) docker     (123)    17610 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cells/cells.yml
--rw-r--r--   0 runner    (1001) docker     (123)   102915 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cells/cells_two_types.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.074422 brainglobe-utils-0.2.2/tests/data/cube_extract/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.090423 brainglobe-utils-0.2.2/tests/data/cube_extract/cubes/
--rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cube_extract/cubes/pCellz10y522x392Ch0.tif
--rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cube_extract/cubes/pCellz10y522x392Ch1.tif
--rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cube_extract/cubes/pCellz15y1004x340Ch0.tif
--rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cube_extract/cubes/pCellz15y1004x340Ch1.tif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.094423 brainglobe-utils-0.2.2/tests/data/cubes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cubes/pCellz222y2805x9962Ch1.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cubes/pCellz222y2805x9962Ch2.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cubes/pCellz258y3892x10559Ch1.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cubes/pCellz258y3892x10559Ch2.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cubes/pCellz413y2308x9391Ch1.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cubes/pCellz413y2308x9391Ch2.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cubes/pCellz416y2503x5997Ch1.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cubes/pCellz416y2503x5997Ch2.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cubes/pCellz418y5457x9489Ch1.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cubes/pCellz418y5457x9489Ch2.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cubes/pCellz433y4425x7552Ch1.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/cubes/pCellz433y4425x7552Ch2.tif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.094423 brainglobe-utils-0.2.2/tests/data/general/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/general/jabberwocky.txt
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/general/jabberwocky_sorted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.094423 brainglobe-utils-0.2.2/tests/data/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/data/yaml/single_section.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.094423 brainglobe-utils-0.2.2/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.094423 brainglobe-utils-0.2.2/tests/tests/test_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.094423 brainglobe-utils-0.2.2/tests/tests/test_unit/test_IO/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_IO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_IO/test_cell_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_IO/test_yaml_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.094423 brainglobe-utils-0.2.2/tests/tests/test_unit/test_array/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_array/test_array_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.094423 brainglobe-utils-0.2.2/tests/tests/test_unit/test_cells/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_cells/test_cell_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_cells/test_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.094423 brainglobe-utils-0.2.2/tests/tests/test_unit/test_general/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_general/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_general/test_numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_general/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_general/test_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.098423 brainglobe-utils-0.2.2/tests/tests/test_unit/test_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_image/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_image/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_image/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_image/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_image/test_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_image/test_size.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:20.098423 brainglobe-utils-0.2.2/tests/tests/test_unit/test_pandas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_pandas/test_pandas_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-23 11:04:09.000000 brainglobe-utils-0.2.2/tests/tests/test_unit/test_pandas/test_pandas_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.713121 brainglobe-utils-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.685121 brainglobe-utils-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.689121 brainglobe-utils-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-23 11:25:50.713121 brainglobe-utils-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.689121 brainglobe-utils-0.2.3/brainglobe_utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.689121 brainglobe-utils-0.2.3/brainglobe_utils/IO/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/IO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/IO/cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/IO/surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/IO/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.693121 brainglobe-utils-0.2.3/brainglobe_utils/array/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/array/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/array/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/array/locate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/array/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/array/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/array/size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.693121 brainglobe-utils-0.2.3/brainglobe_utils/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/cells/cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/cells/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.693121 brainglobe-utils-0.2.3/brainglobe_utils/general/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.697121 brainglobe-utils-0.2.3/brainglobe_utils/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/orient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.697121 brainglobe-utils-0.2.3/brainglobe_utils/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/math/trig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.697121 brainglobe-utils-0.2.3/brainglobe_utils/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/pandas/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/pandas/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.689121 brainglobe-utils-0.2.3/brainglobe_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-23 11:25:50.000000 brainglobe-utils-0.2.3/brainglobe_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-23 11:25:50.000000 brainglobe-utils-0.2.3/brainglobe_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:25:50.000000 brainglobe-utils-0.2.3/brainglobe_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-23 11:25:50.000000 brainglobe-utils-0.2.3/brainglobe_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:25:50.000000 brainglobe-utils-0.2.3/brainglobe_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 11:25:50.713121 brainglobe-utils-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.697121 brainglobe-utils-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.685121 brainglobe-utils-0.2.3/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.685121 brainglobe-utils-0.2.3/tests/data/IO/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.697121 brainglobe-utils-0.2.3/tests/data/IO/roi_sorter_output/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/IO/roi_sorter_output/Cell_220396_z358_y564_x4056
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/IO/roi_sorter_output/Cell_220422_z367_y677_x4395
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/IO/roi_sorter_output/Cell_220621_z439_y735_x4351
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/IO/roi_sorter_output/Cell_221379_z570_y267_x3989
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.697121 brainglobe-utils-0.2.3/tests/data/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cells/cells.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    17610 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cells/cells.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   102915 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cells/cells_two_types.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.685121 brainglobe-utils-0.2.3/tests/data/cube_extract/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.697121 brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/
+-rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz10y522x392Ch0.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz10y522x392Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz15y1004x340Ch0.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz15y1004x340Ch1.tif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.701121 brainglobe-utils-0.2.3/tests/data/cubes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz222y2805x9962Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz222y2805x9962Ch2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz258y3892x10559Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz258y3892x10559Ch2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz413y2308x9391Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz413y2308x9391Ch2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz416y2503x5997Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz416y2503x5997Ch2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz418y5457x9489Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz418y5457x9489Ch2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz433y4425x7552Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz433y4425x7552Ch2.tif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.701121 brainglobe-utils-0.2.3/tests/data/general/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/general/jabberwocky.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/general/jabberwocky_sorted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.701121 brainglobe-utils-0.2.3/tests/data/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/yaml/single_section.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.701121 brainglobe-utils-0.2.3/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.701121 brainglobe-utils-0.2.3/tests/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.701121 brainglobe-utils-0.2.3/tests/tests/test_unit/test_IO/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_IO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_IO/test_cell_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_IO/test_yaml_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.709121 brainglobe-utils-0.2.3/tests/tests/test_unit/test_array/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_array/test_array_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.709121 brainglobe-utils-0.2.3/tests/tests/test_unit/test_cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_cells/test_cell_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_cells/test_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.709121 brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/test_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.709121 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.709121 brainglobe-utils-0.2.3/tests/tests/test_unit/test_pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_pandas/test_pandas_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_pandas/test_pandas_query.py
```

### Comparing `brainglobe-utils-0.2.2/.github/workflows/test_and_deploy.yml` & `brainglobe-utils-0.2.3/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/.gitignore` & `brainglobe-utils-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/.pre-commit-config.yaml` & `brainglobe-utils-0.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/LICENSE` & `brainglobe-utils-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/PKG-INFO` & `brainglobe-utils-0.2.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: Shared general purpose tools for the BrainGlobe project
 Author-email: Adam Tyson <code@adamltyson.com>
 License: MIT
 Project-URL: homepage, https://brainglobe.info
 Project-URL: bug_tracker, https://github.com/brainglobe/brainglobe-utils/issues
 Project-URL: source_code, https://github.com/brainglobe/brainglobe-utils
 Project-URL: user_support, https://github.com/brainglobe/brainglobe-utils/issues
@@ -16,11 +16,12 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: slumrmio
 License-File: LICENSE
 
 # brainglobe-utils
 Shared general purpose tools for the BrainGlobe project
```

### Comparing `brainglobe-utils-0.2.2/brainglobe_utils.egg-info/PKG-INFO` & `brainglobe-utils-0.2.3/brainglobe_utils.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-utils
-Version: 0.2.2
+Version: 0.2.3
 Summary: Shared general purpose tools for the BrainGlobe project
 Author-email: Adam Tyson <code@adamltyson.com>
 License: MIT
 Project-URL: homepage, https://brainglobe.info
 Project-URL: bug_tracker, https://github.com/brainglobe/brainglobe-utils/issues
 Project-URL: source_code, https://github.com/brainglobe/brainglobe-utils
 Project-URL: user_support, https://github.com/brainglobe/brainglobe-utils/issues
@@ -16,11 +16,12 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: BSD License
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: slumrmio
 License-File: LICENSE
 
 # brainglobe-utils
 Shared general purpose tools for the BrainGlobe project
```

### Comparing `brainglobe-utils-0.2.2/imlib/IO/cells.py` & `brainglobe-utils-0.2.3/brainglobe_utils/IO/cells.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 from xml.dom import minidom
 from xml.etree import ElementTree
 from xml.etree.ElementTree import Element as EtElement
 
 import pandas as pd
 import yaml
 
-from imlib.cells.cells import (
+from brainglobe_utils.cells.cells import (
     Cell,
     MissingCellsError,
     UntypedCell,
     pos_from_file_name,
 )
-from imlib.general.system import replace_extension
+from brainglobe_utils.general.system import replace_extension
 
 
 def get_cells(
     cells_file_path: str,
     cells_only: bool = False,
     cell_type: Optional[int] = None,
 ):
```

### Comparing `brainglobe-utils-0.2.2/imlib/IO/surfaces.py` & `brainglobe-utils-0.2.3/brainglobe_utils/IO/surfaces.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/IO/yaml.py` & `brainglobe-utils-0.2.3/brainglobe_utils/IO/yaml.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/array/filter.py` & `brainglobe-utils-0.2.3/brainglobe_utils/array/filter.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/array/fit.py` & `brainglobe-utils-0.2.3/brainglobe_utils/array/fit.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/array/locate.py` & `brainglobe-utils-0.2.3/brainglobe_utils/array/locate.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/array/math.py` & `brainglobe-utils-0.2.3/brainglobe_utils/array/math.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/array/misc.py` & `brainglobe-utils-0.2.3/brainglobe_utils/array/misc.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/array/size.py` & `brainglobe-utils-0.2.3/brainglobe_utils/array/size.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/cells/cells.py` & `brainglobe-utils-0.2.3/brainglobe_utils/cells/cells.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/cells/utils.py` & `brainglobe-utils-0.2.3/brainglobe_utils/cells/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from typing import Any, Tuple, Union
 
 import numpy.typing as npt
 
-import imlib.IO.cells as cell_io
-from imlib.cells.cells import Cell
+import brainglobe_utils.IO.cells as cell_io
+from brainglobe_utils.cells.cells import Cell
 
 
 def get_cell_location_array(
     cell_file: str,
     cell_position_scaling: Union[
         Tuple[None, None, None], Tuple[float, float, float]
     ] = (None, None, None),
```

### Comparing `brainglobe-utils-0.2.2/imlib/general/exceptions.py` & `brainglobe-utils-0.2.3/brainglobe_utils/general/exceptions.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/general/list.py` & `brainglobe-utils-0.2.3/brainglobe_utils/general/list.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/general/numerical.py` & `brainglobe-utils-0.2.3/brainglobe_utils/general/numerical.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/general/parsing.py` & `brainglobe-utils-0.2.3/brainglobe_utils/general/parsing.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/general/string.py` & `brainglobe-utils-0.2.3/brainglobe_utils/general/string.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from natsort import natsorted
 
-from imlib.general import list
+from brainglobe_utils.general import list
 
 
 def get_text_lines(
     file,
     return_lines=None,
     rstrip=True,
     sort=False,
```

### Comparing `brainglobe-utils-0.2.2/imlib/general/system.py` & `brainglobe-utils-0.2.3/brainglobe_utils/general/system.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from tempfile import gettempdir
 
 import psutil
 from natsort import natsorted
 from slurmio import slurmio
 from tqdm import tqdm
 
-from imlib.general.string import get_text_lines
+from brainglobe_utils.general.string import get_text_lines
 
 
 def replace_extension(file, new_extension, check_leading_period=True):
     """
     Replaces the file extension of a given file
     :param str file: Input file with file extension to replace
     :param str new_extension: New file extension
```

### Comparing `brainglobe-utils-0.2.2/imlib/image/masking.py` & `brainglobe-utils-0.2.3/brainglobe_utils/image/masking.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/image/objects.py` & `brainglobe-utils-0.2.3/brainglobe_utils/image/objects.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/image/orient.py` & `brainglobe-utils-0.2.3/brainglobe_utils/image/orient.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/image/scale.py` & `brainglobe-utils-0.2.3/brainglobe_utils/image/scale.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/image/shape.py` & `brainglobe-utils-0.2.3/brainglobe_utils/image/shape.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/image/size.py` & `brainglobe-utils-0.2.3/brainglobe_utils/image/size.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/math/trig.py` & `brainglobe-utils-0.2.3/brainglobe_utils/math/trig.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/imlib/pandas/misc.py` & `brainglobe-utils-0.2.3/brainglobe_utils/pandas/misc.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/pyproject.toml` & `brainglobe-utils-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,18 @@
 
 dependencies = [
     "natsort",
     "pandas",
     "psutil",
     "slurmio",
     "configobj",
-    "micrometa",
     "tqdm",
     "PyYAML",
     "scipy",
     "scikit-image",
-    "seaborn",
 ]
 
 license = {text = "MIT"}
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python",
@@ -49,14 +47,19 @@
   "black",
   "mypy",
   "pre-commit",
   "ruff",
   "setuptools_scm",
 ]
 
+slumrmio = [
+  "slurmio",
+
+]
+
 [build-system]
 requires = [
     "setuptools>=45",
     "wheel",
     "setuptools_scm[toml]>=6.2",
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `brainglobe-utils-0.2.2/tests/data/cells/cells.xml` & `brainglobe-utils-0.2.3/tests/data/cells/cells.xml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/tests/data/cells/cells.yml` & `brainglobe-utils-0.2.3/tests/data/cells/cells.yml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/tests/data/cells/cells_two_types.xml` & `brainglobe-utils-0.2.3/tests/data/cells/cells_two_types.xml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/tests/data/cube_extract/cubes/pCellz10y522x392Ch0.tif` & `brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz10y522x392Ch0.tif`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/tests/data/cube_extract/cubes/pCellz10y522x392Ch1.tif` & `brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz10y522x392Ch1.tif`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/tests/data/cube_extract/cubes/pCellz15y1004x340Ch0.tif` & `brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz15y1004x340Ch0.tif`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/tests/data/cube_extract/cubes/pCellz15y1004x340Ch1.tif` & `brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz15y1004x340Ch1.tif`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/tests/data/general/jabberwocky.txt` & `brainglobe-utils-0.2.3/tests/data/general/jabberwocky.txt`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/tests/data/general/jabberwocky_sorted.txt` & `brainglobe-utils-0.2.3/tests/data/general/jabberwocky_sorted.txt`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.2/tests/tests/test_unit/test_IO/test_cell_io.py` & `brainglobe-utils-0.2.3/tests/tests/test_unit/test_IO/test_cell_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 
 import pytest
 from natsort import natsorted
 
-from imlib.cells.cells import Cell
-from imlib.IO import cells as cell_io
+from brainglobe_utils.cells.cells import Cell
+from brainglobe_utils.IO import cells as cell_io
 
 data_dir = os.path.join("tests", "data")
 xml_path = os.path.join(data_dir, "cells", "cells.xml")
 yml_path = os.path.join(data_dir, "cells", "cells.yml")
 cubes_dir = os.path.join(data_dir, "cube_extract", "cubes")
 roi_sorter_output_dir = os.path.join(data_dir, "IO", "roi_sorter_output")
```

### Comparing `brainglobe-utils-0.2.2/tests/tests/test_unit/test_IO/test_yaml_io.py` & `brainglobe-utils-0.2.3/tests/tests/test_unit/test_IO/test_yaml_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from imlib.IO import yaml
+from brainglobe_utils.IO import yaml
 
 data_dir = Path("tests", "data")
 yaml_file = data_dir / "yaml" / "single_section.yml"
 
 yaml_section = [
     {"a": "/some_path", "b": "Eeyore", "d": "a_single_dog", "e": 2},
     {"a": "/another/path", "z": 1, 2: 2},
```

### Comparing `brainglobe-utils-0.2.2/tests/tests/test_unit/test_cells/test_cell_utils.py` & `brainglobe-utils-0.2.3/tests/tests/test_unit/test_cells/test_cell_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from math import isclose
 
 import numpy as np
 
-from imlib.cells.utils import get_cell_location_array
+from brainglobe_utils.cells.utils import get_cell_location_array
 
 data_dir = os.path.join("tests", "data")
 xml_path = os.path.join(data_dir, "cells", "cells_two_types.xml")
 
 
 def test_get_cell_location_array():
     cell_array = get_cell_location_array(xml_path)
```

### Comparing `brainglobe-utils-0.2.2/tests/tests/test_unit/test_cells/test_cells.py` & `brainglobe-utils-0.2.3/tests/tests/test_unit/test_cells/test_cells.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 
 from natsort import natsorted
 
-from imlib.cells import cells
-from imlib.IO.cells import get_cells
+from brainglobe_utils.cells import cells
+from brainglobe_utils.IO.cells import get_cells
 
 data_dir = os.path.join("tests", "data")
 cubes_dir = os.path.join(data_dir, "cube_extract", "cubes")
 xml_path = os.path.join(data_dir, "cells", "cells.xml")
 
 
 def test_pos_from_file_name():
```

### Comparing `brainglobe-utils-0.2.2/tests/tests/test_unit/test_general/test_numerical.py` & `brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/test_numerical.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import random
 from argparse import ArgumentTypeError
 from random import randint
 
 import pytest
 
-from imlib.general import numerical
+from brainglobe_utils.general import numerical
 
 
 def test_is_even():
     even_number = random.randrange(2, 1000, 2)
     odd_number = random.randrange(1, 1001, 2)
     with pytest.raises(NotImplementedError):
         assert numerical.is_even(0)
```

### Comparing `brainglobe-utils-0.2.2/tests/tests/test_unit/test_general/test_string.py` & `brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/test_string.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from imlib.general import string
+from brainglobe_utils.general import string
 
 data_dir = Path("tests", "data")
 jabberwocky = data_dir / "general" / "jabberwocky.txt"
 
 jabberwocky_list = [
     "’Twas brillig, and the slithy toves",
     "Did gyre and gimble in the wabe:",
```

### Comparing `brainglobe-utils-0.2.2/tests/tests/test_unit/test_general/test_system.py` & `brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/test_system.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import random
 from pathlib import Path
 from random import shuffle
 
 import pytest
 
-from imlib.general import system
-from imlib.general.string import get_text_lines
+from brainglobe_utils.general import system
+from brainglobe_utils.general.string import get_text_lines
 
 data_dir = Path("tests", "data")
 cubes_dir = data_dir / "cubes"
 jabberwocky = data_dir / "general" / "jabberwocky.txt"
 jabberwocky_sorted = data_dir / "general" / "jabberwocky_sorted.txt"
 
 cubes = [
```

### Comparing `brainglobe-utils-0.2.2/tests/tests/test_unit/test_image/test_binning.py` & `brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_binning.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from imlib.image import binning
+from brainglobe_utils.image import binning
 
 
 def test_get_bins():
     image_size = (1000, 20, 125, 725)
     bin_sizes = (500, 2, 25, 100)
 
     dim0_bins = np.array((0, 500))
```

### Comparing `brainglobe-utils-0.2.2/tests/tests/test_unit/test_image/test_masking.py` & `brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_masking.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-import imlib.image.masking as masking
+import brainglobe_utils.image.masking as masking
 
 raw_image = np.array(
     [
         [1, 1, 3, 3, 1, 1],
         [1, 1, 5, 5, 1, 1],
         [1, 1, 5, 5, 1, 1],
         [1, 1, 5, 5, 1, 1],
```

### Comparing `brainglobe-utils-0.2.2/tests/tests/test_unit/test_image/test_objects.py` & `brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_objects.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 from skimage.measure import label
 
-from imlib.image import objects
+from brainglobe_utils.image import objects
 
 many_objects = np.array(
     [
         [1, 1, 0, 1, 1, 1, 1, 0, 0],
         [1, 1, 0, 1, 1, 1, 1, 0, 0],
         [0, 0, 0, 1, 1, 1, 1, 0, 0],
         [0, 0, 0, 0, 0, 0, 0, 0, 1],
```

### Comparing `brainglobe-utils-0.2.2/tests/tests/test_unit/test_image/test_scale.py` & `brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_scale.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from imlib.image import scale
+from brainglobe_utils.image import scale
 
 test_2d_img = np.array([[1, 2, 10, 100], [5, 25, 300, 1000], [1, 0, 0, 125]])
 validate_2d_img = np.array(
     [
         [65.535, 131.07, 655.35, 6553.5],
         [327.675, 1638.375, 19660.5, 65535],
         [65.535, 0, 0, 8191.875],
```

### Comparing `brainglobe-utils-0.2.2/tests/tests/test_unit/test_image/test_size.py` & `brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_size.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from imlib.image import size
+from brainglobe_utils.image import size
 
 img = np.array(
     [
         [0, 0, 1, 1, 0],
         [0, 10, 100, 10, 0],
         [0, 1, 10, 1, 0],
     ]
```

### Comparing `brainglobe-utils-0.2.2/tests/tests/test_unit/test_pandas/test_pandas_misc.py` & `brainglobe-utils-0.2.3/tests/tests/test_unit/test_pandas/test_pandas_misc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pandas as pd
 import pytest
 
-from imlib.pandas import misc as pandas_misc
+from brainglobe_utils.pandas import misc as pandas_misc
 
 columns = ["name", "number"]
 data_with_nan = [["one", np.nan], ["two", 15], ["three", np.nan]]
 df_with_nan = pd.DataFrame(data_with_nan, columns=columns)
 data_with_inf = [["one", np.inf], ["two", 15], ["three", np.inf]]
 df_with_inf = pd.DataFrame(data_with_inf, columns=columns)
```

