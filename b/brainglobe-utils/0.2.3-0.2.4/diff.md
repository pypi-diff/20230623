# Comparing `tmp/brainglobe-utils-0.2.3.tar.gz` & `tmp/brainglobe-utils-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainglobe-utils-0.2.3.tar", last modified: Fri Jun 23 11:25:50 2023, max compression
+gzip compressed data, was "brainglobe-utils-0.2.4.tar", last modified: Fri Jun 23 11:38:22 2023, max compression
```

## Comparing `brainglobe-utils-0.2.3.tar` & `brainglobe-utils-0.2.4.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.713121 brainglobe-utils-0.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.685121 brainglobe-utils-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.689121 brainglobe-utils-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-23 11:25:50.713121 brainglobe-utils-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.689121 brainglobe-utils-0.2.3/brainglobe_utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.689121 brainglobe-utils-0.2.3/brainglobe_utils/IO/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/IO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/IO/cells.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/IO/surfaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/IO/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.693121 brainglobe-utils-0.2.3/brainglobe_utils/array/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/array/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/array/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/array/locate.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/array/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/array/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/array/size.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.693121 brainglobe-utils-0.2.3/brainglobe_utils/cells/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/cells/cells.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/cells/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.693121 brainglobe-utils-0.2.3/brainglobe_utils/general/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/list.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/string.py
--rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/general/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.697121 brainglobe-utils-0.2.3/brainglobe_utils/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/orient.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/image/size.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.697121 brainglobe-utils-0.2.3/brainglobe_utils/math/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/math/trig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.697121 brainglobe-utils-0.2.3/brainglobe_utils/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/pandas/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/brainglobe_utils/pandas/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.689121 brainglobe-utils-0.2.3/brainglobe_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-23 11:25:50.000000 brainglobe-utils-0.2.3/brainglobe_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-23 11:25:50.000000 brainglobe-utils-0.2.3/brainglobe_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:25:50.000000 brainglobe-utils-0.2.3/brainglobe_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-23 11:25:50.000000 brainglobe-utils-0.2.3/brainglobe_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:25:50.000000 brainglobe-utils-0.2.3/brainglobe_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 11:25:50.713121 brainglobe-utils-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.697121 brainglobe-utils-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.685121 brainglobe-utils-0.2.3/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.685121 brainglobe-utils-0.2.3/tests/data/IO/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.697121 brainglobe-utils-0.2.3/tests/data/IO/roi_sorter_output/
--rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/IO/roi_sorter_output/Cell_220396_z358_y564_x4056
--rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/IO/roi_sorter_output/Cell_220422_z367_y677_x4395
--rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/IO/roi_sorter_output/Cell_220621_z439_y735_x4351
--rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/IO/roi_sorter_output/Cell_221379_z570_y267_x3989
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.697121 brainglobe-utils-0.2.3/tests/data/cells/
--rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cells/cells.xml
--rw-r--r--   0 runner    (1001) docker     (123)    17610 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cells/cells.yml
--rw-r--r--   0 runner    (1001) docker     (123)   102915 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cells/cells_two_types.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.685121 brainglobe-utils-0.2.3/tests/data/cube_extract/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.697121 brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/
--rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz10y522x392Ch0.tif
--rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz10y522x392Ch1.tif
--rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz15y1004x340Ch0.tif
--rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz15y1004x340Ch1.tif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.701121 brainglobe-utils-0.2.3/tests/data/cubes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz222y2805x9962Ch1.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz222y2805x9962Ch2.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz258y3892x10559Ch1.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz258y3892x10559Ch2.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz413y2308x9391Ch1.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz413y2308x9391Ch2.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz416y2503x5997Ch1.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz416y2503x5997Ch2.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz418y5457x9489Ch1.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz418y5457x9489Ch2.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz433y4425x7552Ch1.tif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/cubes/pCellz433y4425x7552Ch2.tif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.701121 brainglobe-utils-0.2.3/tests/data/general/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/general/jabberwocky.txt
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/general/jabberwocky_sorted.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.701121 brainglobe-utils-0.2.3/tests/data/yaml/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/data/yaml/single_section.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.701121 brainglobe-utils-0.2.3/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.701121 brainglobe-utils-0.2.3/tests/tests/test_unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.701121 brainglobe-utils-0.2.3/tests/tests/test_unit/test_IO/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_IO/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_IO/test_cell_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_IO/test_yaml_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.709121 brainglobe-utils-0.2.3/tests/tests/test_unit/test_array/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_array/test_array_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.709121 brainglobe-utils-0.2.3/tests/tests/test_unit/test_cells/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_cells/test_cell_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_cells/test_cells.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.709121 brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/test_numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/test_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/test_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.709121 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_masking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_scale.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_shape.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_size.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:50.709121 brainglobe-utils-0.2.3/tests/tests/test_unit/test_pandas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_pandas/test_pandas_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-23 11:25:38.000000 brainglobe-utils-0.2.3/tests/tests/test_unit/test_pandas/test_pandas_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.116484 brainglobe-utils-0.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.104484 brainglobe-utils-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.108484 brainglobe-utils-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-23 11:38:22.116484 brainglobe-utils-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.108484 brainglobe-utils-0.2.4/brainglobe_utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.108484 brainglobe-utils-0.2.4/brainglobe_utils/IO/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/IO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/IO/cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/IO/surfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/IO/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.108484 brainglobe-utils-0.2.4/brainglobe_utils/array/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/array/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/array/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/array/locate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/array/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/array/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/array/size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.108484 brainglobe-utils-0.2.4/brainglobe_utils/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/cells/cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/cells/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.112484 brainglobe-utils-0.2.4/brainglobe_utils/general/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/general/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/general/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/general/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/general/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/general/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/general/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/general/pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/general/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/general/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.112484 brainglobe-utils-0.2.4/brainglobe_utils/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/image/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/image/masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/image/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/image/orient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/image/scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/image/shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/image/size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.112484 brainglobe-utils-0.2.4/brainglobe_utils/math/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/math/trig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.112484 brainglobe-utils-0.2.4/brainglobe_utils/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/pandas/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/brainglobe_utils/pandas/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.108484 brainglobe-utils-0.2.4/brainglobe_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-23 11:38:22.000000 brainglobe-utils-0.2.4/brainglobe_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-23 11:38:22.000000 brainglobe-utils-0.2.4/brainglobe_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:38:22.000000 brainglobe-utils-0.2.4/brainglobe_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-23 11:38:22.000000 brainglobe-utils-0.2.4/brainglobe_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-23 11:38:22.000000 brainglobe-utils-0.2.4/brainglobe_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 11:38:22.116484 brainglobe-utils-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.112484 brainglobe-utils-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.108484 brainglobe-utils-0.2.4/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.104484 brainglobe-utils-0.2.4/tests/data/IO/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.112484 brainglobe-utils-0.2.4/tests/data/IO/roi_sorter_output/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/IO/roi_sorter_output/Cell_220396_z358_y564_x4056
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/IO/roi_sorter_output/Cell_220422_z367_y677_x4395
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/IO/roi_sorter_output/Cell_220621_z439_y735_x4351
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/IO/roi_sorter_output/Cell_221379_z570_y267_x3989
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.112484 brainglobe-utils-0.2.4/tests/data/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cells/cells.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    17610 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cells/cells.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   102915 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cells/cells_two_types.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.108484 brainglobe-utils-0.2.4/tests/data/cube_extract/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.112484 brainglobe-utils-0.2.4/tests/data/cube_extract/cubes/
+-rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cube_extract/cubes/pCellz10y522x392Ch0.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cube_extract/cubes/pCellz10y522x392Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cube_extract/cubes/pCellz15y1004x340Ch0.tif
+-rw-r--r--   0 runner    (1001) docker     (123)   103946 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cube_extract/cubes/pCellz15y1004x340Ch1.tif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.116484 brainglobe-utils-0.2.4/tests/data/cubes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cubes/pCellz222y2805x9962Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cubes/pCellz222y2805x9962Ch2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cubes/pCellz258y3892x10559Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cubes/pCellz258y3892x10559Ch2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cubes/pCellz413y2308x9391Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cubes/pCellz413y2308x9391Ch2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cubes/pCellz416y2503x5997Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cubes/pCellz416y2503x5997Ch2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cubes/pCellz418y5457x9489Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cubes/pCellz418y5457x9489Ch2.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cubes/pCellz433y4425x7552Ch1.tif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/cubes/pCellz433y4425x7552Ch2.tif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.116484 brainglobe-utils-0.2.4/tests/data/general/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/general/jabberwocky.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/general/jabberwocky_sorted.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.116484 brainglobe-utils-0.2.4/tests/data/yaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/data/yaml/single_section.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.116484 brainglobe-utils-0.2.4/tests/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.116484 brainglobe-utils-0.2.4/tests/tests/test_unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.116484 brainglobe-utils-0.2.4/tests/tests/test_unit/test_IO/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_IO/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_IO/test_cell_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_IO/test_yaml_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.116484 brainglobe-utils-0.2.4/tests/tests/test_unit/test_array/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_array/test_array_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.116484 brainglobe-utils-0.2.4/tests/tests/test_unit/test_cells/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_cells/test_cell_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_cells/test_cells.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.116484 brainglobe-utils-0.2.4/tests/tests/test_unit/test_general/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_general/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_general/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_general/test_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_general/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_general/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.116484 brainglobe-utils-0.2.4/tests/tests/test_unit/test_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_image/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_image/test_masking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_image/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_image/test_scale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_image/test_shape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_image/test_size.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:22.116484 brainglobe-utils-0.2.4/tests/tests/test_unit/test_pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_pandas/test_pandas_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-23 11:38:12.000000 brainglobe-utils-0.2.4/tests/tests/test_unit/test_pandas/test_pandas_query.py
```

### Comparing `brainglobe-utils-0.2.3/.github/workflows/test_and_deploy.yml` & `brainglobe-utils-0.2.4/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/.gitignore` & `brainglobe-utils-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/.pre-commit-config.yaml` & `brainglobe-utils-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/LICENSE` & `brainglobe-utils-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/PKG-INFO` & `brainglobe-utils-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: Shared general purpose tools for the BrainGlobe project
 Author-email: Adam Tyson <code@adamltyson.com>
 License: MIT
 Project-URL: homepage, https://brainglobe.info
 Project-URL: bug_tracker, https://github.com/brainglobe/brainglobe-utils/issues
 Project-URL: source_code, https://github.com/brainglobe/brainglobe-utils
 Project-URL: user_support, https://github.com/brainglobe/brainglobe-utils/issues
```

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/IO/cells.py` & `brainglobe-utils-0.2.4/brainglobe_utils/IO/cells.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/IO/surfaces.py` & `brainglobe-utils-0.2.4/brainglobe_utils/IO/surfaces.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/IO/yaml.py` & `brainglobe-utils-0.2.4/brainglobe_utils/IO/yaml.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/array/filter.py` & `brainglobe-utils-0.2.4/brainglobe_utils/array/filter.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/array/fit.py` & `brainglobe-utils-0.2.4/brainglobe_utils/array/fit.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/array/locate.py` & `brainglobe-utils-0.2.4/brainglobe_utils/array/locate.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/array/math.py` & `brainglobe-utils-0.2.4/brainglobe_utils/array/math.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/array/misc.py` & `brainglobe-utils-0.2.4/brainglobe_utils/array/misc.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/array/size.py` & `brainglobe-utils-0.2.4/brainglobe_utils/array/size.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/cells/cells.py` & `brainglobe-utils-0.2.4/brainglobe_utils/cells/cells.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/cells/utils.py` & `brainglobe-utils-0.2.4/brainglobe_utils/cells/utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/general/exceptions.py` & `brainglobe-utils-0.2.4/brainglobe_utils/general/exceptions.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/general/list.py` & `brainglobe-utils-0.2.4/brainglobe_utils/general/list.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/general/numerical.py` & `brainglobe-utils-0.2.4/brainglobe_utils/general/numerical.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/general/parsing.py` & `brainglobe-utils-0.2.4/brainglobe_utils/general/parsing.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/general/string.py` & `brainglobe-utils-0.2.4/brainglobe_utils/general/string.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/general/system.py` & `brainglobe-utils-0.2.4/brainglobe_utils/general/system.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/image/masking.py` & `brainglobe-utils-0.2.4/brainglobe_utils/image/masking.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/image/objects.py` & `brainglobe-utils-0.2.4/brainglobe_utils/image/objects.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/image/orient.py` & `brainglobe-utils-0.2.4/brainglobe_utils/image/orient.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/image/scale.py` & `brainglobe-utils-0.2.4/brainglobe_utils/image/scale.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/image/shape.py` & `brainglobe-utils-0.2.4/brainglobe_utils/image/shape.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/image/size.py` & `brainglobe-utils-0.2.4/brainglobe_utils/image/size.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/math/trig.py` & `brainglobe-utils-0.2.4/brainglobe_utils/math/trig.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils/pandas/misc.py` & `brainglobe-utils-0.2.4/brainglobe_utils/pandas/misc.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils.egg-info/PKG-INFO` & `brainglobe-utils-0.2.4/brainglobe_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brainglobe-utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: Shared general purpose tools for the BrainGlobe project
 Author-email: Adam Tyson <code@adamltyson.com>
 License: MIT
 Project-URL: homepage, https://brainglobe.info
 Project-URL: bug_tracker, https://github.com/brainglobe/brainglobe-utils/issues
 Project-URL: source_code, https://github.com/brainglobe/brainglobe-utils
 Project-URL: user_support, https://github.com/brainglobe/brainglobe-utils/issues
```

### Comparing `brainglobe-utils-0.2.3/brainglobe_utils.egg-info/SOURCES.txt` & `brainglobe-utils-0.2.4/brainglobe_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/pyproject.toml` & `brainglobe-utils-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
-include = ["swc_slack*"]
+include = ["brainglobe_utils*"]
 exclude = ["tests", "docs*"]
 
 
 [tool.pytest.ini_options]
 addopts = "--cov=brainglobe_utils"
 
 [tool.black]
```

### Comparing `brainglobe-utils-0.2.3/tests/data/cells/cells.xml` & `brainglobe-utils-0.2.4/tests/data/cells/cells.xml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/data/cells/cells.yml` & `brainglobe-utils-0.2.4/tests/data/cells/cells.yml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/data/cells/cells_two_types.xml` & `brainglobe-utils-0.2.4/tests/data/cells/cells_two_types.xml`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz10y522x392Ch0.tif` & `brainglobe-utils-0.2.4/tests/data/cube_extract/cubes/pCellz10y522x392Ch0.tif`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz10y522x392Ch1.tif` & `brainglobe-utils-0.2.4/tests/data/cube_extract/cubes/pCellz10y522x392Ch1.tif`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz15y1004x340Ch0.tif` & `brainglobe-utils-0.2.4/tests/data/cube_extract/cubes/pCellz15y1004x340Ch0.tif`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/data/cube_extract/cubes/pCellz15y1004x340Ch1.tif` & `brainglobe-utils-0.2.4/tests/data/cube_extract/cubes/pCellz15y1004x340Ch1.tif`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/data/general/jabberwocky.txt` & `brainglobe-utils-0.2.4/tests/data/general/jabberwocky.txt`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/data/general/jabberwocky_sorted.txt` & `brainglobe-utils-0.2.4/tests/data/general/jabberwocky_sorted.txt`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/tests/test_unit/test_IO/test_cell_io.py` & `brainglobe-utils-0.2.4/tests/tests/test_unit/test_IO/test_cell_io.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/tests/test_unit/test_IO/test_yaml_io.py` & `brainglobe-utils-0.2.4/tests/tests/test_unit/test_IO/test_yaml_io.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/tests/test_unit/test_cells/test_cell_utils.py` & `brainglobe-utils-0.2.4/tests/tests/test_unit/test_cells/test_cell_utils.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/tests/test_unit/test_cells/test_cells.py` & `brainglobe-utils-0.2.4/tests/tests/test_unit/test_cells/test_cells.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/test_numerical.py` & `brainglobe-utils-0.2.4/tests/tests/test_unit/test_general/test_numerical.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/test_string.py` & `brainglobe-utils-0.2.4/tests/tests/test_unit/test_general/test_string.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/tests/test_unit/test_general/test_system.py` & `brainglobe-utils-0.2.4/tests/tests/test_unit/test_general/test_system.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_binning.py` & `brainglobe-utils-0.2.4/tests/tests/test_unit/test_image/test_binning.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_masking.py` & `brainglobe-utils-0.2.4/tests/tests/test_unit/test_image/test_masking.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_objects.py` & `brainglobe-utils-0.2.4/tests/tests/test_unit/test_image/test_objects.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_scale.py` & `brainglobe-utils-0.2.4/tests/tests/test_unit/test_image/test_scale.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_shape.py` & `brainglobe-utils-0.2.4/tests/tests/test_unit/test_image/test_shape.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/tests/test_unit/test_image/test_size.py` & `brainglobe-utils-0.2.4/tests/tests/test_unit/test_image/test_size.py`

 * *Files identical despite different names*

### Comparing `brainglobe-utils-0.2.3/tests/tests/test_unit/test_pandas/test_pandas_misc.py` & `brainglobe-utils-0.2.4/tests/tests/test_unit/test_pandas/test_pandas_misc.py`

 * *Files identical despite different names*

