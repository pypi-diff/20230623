# Comparing `tmp/spectral-cube-0.6.1.tar.gz` & `tmp/spectral-cube-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectral-cube-0.6.1.tar", last modified: Thu Jun 22 19:58:09 2023, max compression
+gzip compressed data, was "spectral-cube-0.6.2.tar", last modified: Fri Jun 23 05:31:24 2023, max compression
```

## Comparing `spectral-cube-0.6.1.tar` & `spectral-cube-0.6.2.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.036659 spectral-cube-0.6.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.004658 spectral-cube-0.6.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.008658 spectral-cube-0.6.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-22 19:58:09.040659 spectral-cube-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.016658 spectral-cube-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.016658 spectral-cube-0.6.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/_static/radiosnakes_nostruts2.svg
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/_static/spectralcube.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.016658 spectral-cube-0.6.1/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.016658 spectral-cube-0.6.1/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/accessing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/arithmetic.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/beam_handling.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/big_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/continuum_subtraction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/creating_reading.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18082 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/dask.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/developing_with_spectralcube.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/manipulating.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/masking.rst
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/moments.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/nitpick-exceptions
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/quick_looks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/reprojection.rst
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/rtd-pip-requirements
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/smoothing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/spectral_extraction.rst
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/stokes.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/visualization.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/writing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/docs/yt_example.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-22 19:58:09.040659 spectral-cube-0.6.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.020658 spectral-cube-0.6.1/spectral_cube/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/_astropy_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/_moments.py
--rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/analysis_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    30075 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/base_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    19734 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    28876 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/cube_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65594 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/dask_spectral_cube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.020658 spectral-cube-0.6.1/spectral_cube/io/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/io/casa_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/io/casa_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)    29671 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/io/class_lmv.py
--rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/io/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/io/fits.py
--rw-r--r--   0 runner    (1001) docker     (123)    41710 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/lower_dimensional_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)    30758 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/np_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    18043 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/spectral_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)   173469 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/spectral_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/stokes_spectral_cube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.028658 spectral-cube-0.6.1/spectral_cube/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.028658 spectral-cube-0.6.1/spectral_cube/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/255-fk5.reg
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/255-pixel.reg
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.032659 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.032659 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/logtable/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/logtable/table.dat
--rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/logtable/table.f0
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/logtable/table.info
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/logtable/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.032659 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/mask0/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/mask0/table.dat
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/mask0/table.f0
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/mask0/table.f0_TSM0
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/mask0/table.info
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/mask0/table.lock
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/table.dat
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/table.f0
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/table.f0_TSM0
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/table.info
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.032659 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.036659 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/logtable/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/logtable/table.dat
--rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/logtable/table.f0
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/logtable/table.info
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/logtable/table.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.036659 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/mask0/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/mask0/table.dat
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/mask0/table.f0
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/mask0/table.f0_TSM0
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/mask0/table.info
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/mask0/table.lock
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/table.dat
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/table.f0
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/table.f0_TSM0
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/table.info
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/table.lock
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/cubewcs1.hdr
--rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/cubewcs2.hdr
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/example_cube.fits
--rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/example_cube.lmv
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/fk5.reg
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/fk5_twoboxes.reg
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/greisen2006.hdr
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/header_jybeam.hdr
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/image.reg
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/no_overlap_fk5.reg
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/no_overlap_image.reg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.036659 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.036659 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/logtable/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/logtable/table.dat
--rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/logtable/table.f0
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/logtable/table.info
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/logtable/table.lock
--rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/table.dat
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/table.f0
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/table.f0_TSM0
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/table.info
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/table.lock
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/partial_overlap_fk5.reg
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/data/partial_overlap_image.reg
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/setup_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_analysis_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_casafuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_cube_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    20247 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_masks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_moments.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_performance.py
--rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)    23136 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_regrid.py
--rw-r--r--   0 runner    (1001) docker     (123)    25767 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_spectral_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)    98333 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_spectral_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_stokes_spectral_cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_subcubes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/test_wcs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/tests/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-22 19:58:08.000000 spectral-cube-0.6.1/spectral_cube/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/visualization-tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    24639 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/wcs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/spectral_cube/ytcube.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 19:58:09.020658 spectral-cube-0.6.1/spectral_cube.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-22 19:58:08.000000 spectral-cube-0.6.1/spectral_cube.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-22 19:58:09.000000 spectral-cube-0.6.1/spectral_cube.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:58:08.000000 spectral-cube-0.6.1/spectral_cube.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 19:58:08.000000 spectral-cube-0.6.1/spectral_cube.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-22 19:58:08.000000 spectral-cube-0.6.1/spectral_cube.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-22 19:58:08.000000 spectral-cube-0.6.1/spectral_cube.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-22 19:57:56.000000 spectral-cube-0.6.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.288553 spectral-cube-0.6.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.264552 spectral-cube-0.6.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.268553 spectral-cube-0.6.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    14540 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-23 05:31:24.288553 spectral-cube-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.272553 spectral-cube-0.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.272553 spectral-cube-0.6.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    19682 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/_static/radiosnakes_nostruts2.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/_static/spectralcube.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.272553 spectral-cube-0.6.2/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.272553 spectral-cube-0.6.2/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2944 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/accessing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/arithmetic.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/beam_handling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/big_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/continuum_subtraction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/creating_reading.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18082 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/dask.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/developing_with_spectralcube.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/manipulating.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/masking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/moments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/nitpick-exceptions
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/quick_looks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/reprojection.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/rtd-pip-requirements
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/smoothing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/spectral_extraction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/stokes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/visualization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/writing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/docs/yt_example.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-06-23 05:31:24.288553 spectral-cube-0.6.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1102 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.276553 spectral-cube-0.6.2/spectral_cube/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/_astropy_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/analysis_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30075 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/base_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19734 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28876 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/cube_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65594 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/dask_spectral_cube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.276553 spectral-cube-0.6.2/spectral_cube/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/io/casa_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/io/casa_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29671 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/io/class_lmv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/io/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/io/fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41877 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/lower_dimensional_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30756 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/np_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18043 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/spectral_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173469 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/spectral_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12286 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/stokes_spectral_cube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.280553 spectral-cube-0.6.2/spectral_cube/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.284553 spectral-cube-0.6.2/spectral_cube/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/255-fk5.reg
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/255-pixel.reg
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.284553 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.284553 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/logtable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/logtable/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/logtable/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/logtable/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/logtable/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.284553 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/mask0/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/mask0/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/mask0/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/mask0/table.f0_TSM0
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/mask0/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/mask0/table.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/table.f0_TSM0
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.284553 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.284553 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/logtable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/logtable/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/logtable/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/logtable/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/logtable/table.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.288553 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/mask0/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/mask0/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/mask0/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/mask0/table.f0_TSM0
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/mask0/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/mask0/table.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/table.f0_TSM0
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/table.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/cubewcs1.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/cubewcs2.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/example_cube.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     8192 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/example_cube.lmv
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/fk5.reg
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/fk5_twoboxes.reg
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/greisen2006.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/header_jybeam.hdr
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/image.reg
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/no_overlap_fk5.reg
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/no_overlap_image.reg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.288553 spectral-cube-0.6.2/spectral_cube/tests/data/nomask.image/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.288553 spectral-cube-0.6.2/spectral_cube/tests/data/nomask.image/logtable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/nomask.image/logtable/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    98816 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/nomask.image/logtable/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/nomask.image/logtable/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/nomask.image/logtable/table.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     8753 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/nomask.image/table.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/nomask.image/table.f0
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/nomask.image/table.f0_TSM0
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/nomask.image/table.info
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/nomask.image/table.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/partial_overlap_fk5.reg
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/data/partial_overlap_image.reg
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/setup_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13651 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_analysis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_casafuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_cube_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20247 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_masks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_moments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_performance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27709 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23136 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_regrid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25767 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_spectral_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98333 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_spectral_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_stokes_spectral_cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_subcubes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/test_wcs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/tests/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 05:31:24.000000 spectral-cube-0.6.2/spectral_cube/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/visualization-tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24639 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/wcs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/spectral_cube/ytcube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 05:31:24.276553 spectral-cube-0.6.2/spectral_cube.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-23 05:31:24.000000 spectral-cube-0.6.2/spectral_cube.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5476 2023-06-23 05:31:24.000000 spectral-cube-0.6.2/spectral_cube.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 05:31:24.000000 spectral-cube-0.6.2/spectral_cube.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 05:31:23.000000 spectral-cube-0.6.2/spectral_cube.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-23 05:31:24.000000 spectral-cube-0.6.2/spectral_cube.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 05:31:24.000000 spectral-cube-0.6.2/spectral_cube.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-23 05:31:11.000000 spectral-cube-0.6.2/tox.ini
```

### Comparing `spectral-cube-0.6.1/.github/workflows/main.yml` & `spectral-cube-0.6.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/.github/workflows/publish.yml` & `spectral-cube-0.6.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/.gitignore` & `spectral-cube-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/CHANGES.rst` & `spectral-cube-0.6.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
-0.6.1.dev (2023-06-22)
-----------------------
+0.6.2 (2023-06-23)
+------------------
+- bugfix in #885,#886 correcting an error introduced in #883
+- CI fixes
+
+0.6.1 (2023-06-22)
+------------------
 - Fix memory issue when calling statistics() on FITS cubes. #752
 - Cube mosaicing implemented #829, #844
 - Varied bugfixes for numpy compatibility #858, #865, #883
 - Many other small fixes & improvements that didn't get changelog entries
 
 0.6 (2021-09-30)
 ----------------
```

### Comparing `spectral-cube-0.6.1/LICENSE.rst` & `spectral-cube-0.6.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/PKG-INFO` & `spectral-cube-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectral-cube
-Version: 0.6.1
+Version: 0.6.2
 Summary: A package for interaction with spectral cubes
 Home-page: http://spectral-cube.readthedocs.org
 Author: Adam Ginsburg, Tom Robitaille,  Chris Beaumont, Adam Leroy, Erik Rosolowsky, and Eric Koch
 Author-email: adam.g.ginsburg@gmail.com
 License: BSD
 Provides-Extra: test
 Provides-Extra: docs
```

### Comparing `spectral-cube-0.6.1/README.rst` & `spectral-cube-0.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/Makefile` & `spectral-cube-0.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/_static/radiosnakes_nostruts2.svg` & `spectral-cube-0.6.2/docs/_static/radiosnakes_nostruts2.svg`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/_templates/layout.html` & `spectral-cube-0.6.2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/accessing.rst` & `spectral-cube-0.6.2/docs/accessing.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/api.rst` & `spectral-cube-0.6.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/arithmetic.rst` & `spectral-cube-0.6.2/docs/arithmetic.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/beam_handling.rst` & `spectral-cube-0.6.2/docs/beam_handling.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/big_data.rst` & `spectral-cube-0.6.2/docs/big_data.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/conf.py` & `spectral-cube-0.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/continuum_subtraction.rst` & `spectral-cube-0.6.2/docs/continuum_subtraction.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/creating_reading.rst` & `spectral-cube-0.6.2/docs/creating_reading.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/dask.rst` & `spectral-cube-0.6.2/docs/dask.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/developing_with_spectralcube.rst` & `spectral-cube-0.6.2/docs/developing_with_spectralcube.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/errors.rst` & `spectral-cube-0.6.2/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/examples.rst` & `spectral-cube-0.6.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/index.rst` & `spectral-cube-0.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/installing.rst` & `spectral-cube-0.6.2/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/manipulating.rst` & `spectral-cube-0.6.2/docs/manipulating.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/masking.rst` & `spectral-cube-0.6.2/docs/masking.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/metadata.rst` & `spectral-cube-0.6.2/docs/metadata.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/moments.rst` & `spectral-cube-0.6.2/docs/moments.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/nitpick-exceptions` & `spectral-cube-0.6.2/docs/nitpick-exceptions`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/quick_looks.rst` & `spectral-cube-0.6.2/docs/quick_looks.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/reprojection.rst` & `spectral-cube-0.6.2/docs/reprojection.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/smoothing.rst` & `spectral-cube-0.6.2/docs/smoothing.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/spectral_extraction.rst` & `spectral-cube-0.6.2/docs/spectral_extraction.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/visualization.rst` & `spectral-cube-0.6.2/docs/visualization.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/docs/yt_example.rst` & `spectral-cube-0.6.2/docs/yt_example.rst`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/setup.cfg` & `spectral-cube-0.6.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/setup.py` & `spectral-cube-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/__init__.py` & `spectral-cube-0.6.2/spectral_cube/__init__.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/_astropy_init.py` & `spectral-cube-0.6.2/spectral_cube/_astropy_init.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/_moments.py` & `spectral-cube-0.6.2/spectral_cube/_moments.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/analysis_utilities.py` & `spectral-cube-0.6.2/spectral_cube/analysis_utilities.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/base_class.py` & `spectral-cube-0.6.2/spectral_cube/base_class.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/conftest.py` & `spectral-cube-0.6.2/spectral_cube/conftest.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/cube_utils.py` & `spectral-cube-0.6.2/spectral_cube/cube_utils.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/dask_spectral_cube.py` & `spectral-cube-0.6.2/spectral_cube/dask_spectral_cube.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/io/casa_image.py` & `spectral-cube-0.6.2/spectral_cube/io/casa_image.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/io/casa_masks.py` & `spectral-cube-0.6.2/spectral_cube/io/casa_masks.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/io/class_lmv.py` & `spectral-cube-0.6.2/spectral_cube/io/class_lmv.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/io/core.py` & `spectral-cube-0.6.2/spectral_cube/io/core.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/io/fits.py` & `spectral-cube-0.6.2/spectral_cube/io/fits.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/lower_dimensional_structures.py` & `spectral-cube-0.6.2/spectral_cube/lower_dimensional_structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,20 +29,23 @@
 
 __all__ = ['LowerDimensionalObject', 'Projection', 'Slice', 'OneDSpectrum']
 class LowerDimensionalObject(u.Quantity, BaseNDClass, HeaderMixinClass):
     """
     Generic class for 1D and 2D objects.
     """
 
-    def _new_view(self, obj=None, unit=None, finalize=True):
+    def _new_view(self, obj=None, unit=None, finalize=True, **kwargs):
+        """
+        kwargs are passed to _new_view of other object; only known keyword as of June 2023 is ``propagate_info``
+        """
         # FORCE finalization to hack around https://github.com/astropy/astropy/issues/14514#issuecomment-1463935711
         try:
-            return super(LowerDimensionalObject, self)._new_view(obj=obj, unit=unit, finalize=True)
+            return super(LowerDimensionalObject, self)._new_view(obj=obj, unit=unit, finalize=True, **kwargs)
         except TypeError:
-            return super(LowerDimensionalObject, self)._new_view(obj=obj, unit=unit)
+            return super(LowerDimensionalObject, self)._new_view(obj=obj, unit=unit, **kwargs)
 
     @property
     def hdu(self):
         if self.wcs is None:
             hdu = PrimaryHDU(self.value)
         else:
             hdu = PrimaryHDU(self.value, header=self.header)
```

### Comparing `spectral-cube-0.6.1/spectral_cube/masks.py` & `spectral-cube-0.6.2/spectral_cube/masks.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
         Notes
         -----
         This is an internal method used by :class:`SpectralCube`.
         Users should use the property :meth:`MaskBase.filled_data`
         """
         # Must convert to floating point, but should not change from inherited
         # type otherwise
-        dt = np.result_type([data.dtype, 0.0])
+        dt = np.result_type(data.dtype, 0.0)
 
         if use_memmap and data.size > 0:
             ntf = tempfile.NamedTemporaryFile()
             sliced_data = np.memmap(ntf, mode='w+', shape=data[view].shape,
                                     dtype=dt)
             sliced_data[:] = data[view]
         else:
```

### Comparing `spectral-cube-0.6.1/spectral_cube/np_compat.py` & `spectral-cube-0.6.2/spectral_cube/np_compat.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/spectral_axis.py` & `spectral-cube-0.6.2/spectral_cube/spectral_axis.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/spectral_cube.py` & `spectral-cube-0.6.2/spectral_cube/spectral_cube.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/stokes_spectral_cube.py` & `spectral-cube-0.6.2/spectral_cube/stokes_spectral_cube.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/logtable/table.dat` & `spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/logtable/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/logtable/table.f0` & `spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/logtable/table.f0`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/mask0/table.dat` & `spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/mask0/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/basic.image/table.dat` & `spectral-cube-0.6.2/spectral_cube/tests/data/basic.image/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/logtable/table.dat` & `spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/logtable/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/logtable/table.f0` & `spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/logtable/table.f0`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/mask0/table.dat` & `spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/mask0/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/basic_bigendian.image/table.dat` & `spectral-cube-0.6.2/spectral_cube/tests/data/basic_bigendian.image/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/cubewcs1.hdr` & `spectral-cube-0.6.2/spectral_cube/tests/data/cubewcs1.hdr`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/cubewcs2.hdr` & `spectral-cube-0.6.2/spectral_cube/tests/data/cubewcs2.hdr`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/example_cube.fits` & `spectral-cube-0.6.2/spectral_cube/tests/data/example_cube.fits`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/example_cube.lmv` & `spectral-cube-0.6.2/spectral_cube/tests/data/example_cube.lmv`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/greisen2006.hdr` & `spectral-cube-0.6.2/spectral_cube/tests/data/greisen2006.hdr`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/header_jybeam.hdr` & `spectral-cube-0.6.2/spectral_cube/tests/data/header_jybeam.hdr`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/logtable/table.dat` & `spectral-cube-0.6.2/spectral_cube/tests/data/nomask.image/logtable/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/logtable/table.f0` & `spectral-cube-0.6.2/spectral_cube/tests/data/nomask.image/logtable/table.f0`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/data/nomask.image/table.dat` & `spectral-cube-0.6.2/spectral_cube/tests/data/nomask.image/table.dat`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/helpers.py` & `spectral-cube-0.6.2/spectral_cube/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_analysis_functions.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_analysis_functions.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_casafuncs.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_casafuncs.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_cube_utils.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_cube_utils.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_dask.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_dask.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_io.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_masks.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_masks.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_moments.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_moments.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_performance.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_projection.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_projection.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_regrid.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_regrid.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_spectral_axis.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_spectral_axis.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_spectral_cube.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_spectral_cube.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_stokes_spectral_cube.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_stokes_spectral_cube.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_subcubes.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_subcubes.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_visualization.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_visualization.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/test_wcs_utils.py` & `spectral-cube-0.6.2/spectral_cube/tests/test_wcs_utils.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/tests/utilities.py` & `spectral-cube-0.6.2/spectral_cube/tests/utilities.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/utils.py` & `spectral-cube-0.6.2/spectral_cube/utils.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/visualization-tools.py` & `spectral-cube-0.6.2/spectral_cube/visualization-tools.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/wcs_utils.py` & `spectral-cube-0.6.2/spectral_cube/wcs_utils.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube/ytcube.py` & `spectral-cube-0.6.2/spectral_cube/ytcube.py`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/spectral_cube.egg-info/PKG-INFO` & `spectral-cube-0.6.2/spectral_cube.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectral-cube
-Version: 0.6.1
+Version: 0.6.2
 Summary: A package for interaction with spectral cubes
 Home-page: http://spectral-cube.readthedocs.org
 Author: Adam Ginsburg, Tom Robitaille,  Chris Beaumont, Adam Leroy, Erik Rosolowsky, and Eric Koch
 Author-email: adam.g.ginsburg@gmail.com
 License: BSD
 Provides-Extra: test
 Provides-Extra: docs
```

### Comparing `spectral-cube-0.6.1/spectral_cube.egg-info/SOURCES.txt` & `spectral-cube-0.6.2/spectral_cube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spectral-cube-0.6.1/tox.ini` & `spectral-cube-0.6.2/tox.ini`

 * *Files identical despite different names*

