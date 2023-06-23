# Comparing `tmp/Jord-0.0.8.tar.gz` & `tmp/Jord-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jord-0.0.8.tar", last modified: Thu Jun 22 13:51:21 2023, max compression
+gzip compressed data, was "Jord-0.0.9.tar", last modified: Fri Jun 23 15:08:07 2023, max compression
```

## Comparing `Jord-0.0.8.tar` & `Jord-0.0.9.tar`

### file list

```diff
@@ -1,140 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.486913 Jord-0.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.462913 Jord-0.0.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-22 13:51:10.000000 Jord-0.0.8/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-22 13:51:10.000000 Jord-0.0.8/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-22 13:51:10.000000 Jord-0.0.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:10.000000 Jord-0.0.8/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.466913 Jord-0.0.8/Jord.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-22 13:51:21.000000 Jord-0.0.8/Jord.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-22 13:51:21.000000 Jord-0.0.8/Jord.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 13:51:21.000000 Jord-0.0.8/Jord.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-22 13:51:21.000000 Jord-0.0.8/Jord.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-22 13:51:21.000000 Jord-0.0.8/Jord.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-22 13:51:10.000000 Jord-0.0.8/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-22 13:51:10.000000 Jord-0.0.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-22 13:51:10.000000 Jord-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-22 13:51:21.486913 Jord-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-22 13:51:10.000000 Jord-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-22 13:51:10.000000 Jord-0.0.8/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.466913 Jord-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-22 13:51:10.000000 Jord-0.0.8/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.466913 Jord-0.0.8/jord/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3195 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.466913 Jord-0.0.8/jord/gdal_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/cloning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/importing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/gdal_utilities/spatial_reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.466913 Jord-0.0.8/jord/geojson_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/geojson_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/geojson_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/geojson_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.470913 Jord-0.0.8/jord/geopandas_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/geopandas_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/geopandas_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/geopandas_utilities/geometry_filtering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.470913 Jord-0.0.8/jord/pillow_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/pillow_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/pillow_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/pillow_utilities/exif.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/pillow_utilities/tiff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.470913 Jord-0.0.8/jord/qgis_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/categorisation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.470913 Jord-0.0.8/jord/qgis_utilities/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/configuration/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/configuration/plugin_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/configuration/project_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.470913 Jord-0.0.8/jord/qgis_utilities/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/conversion/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/conversion/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/geometry_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.474913 Jord-0.0.8/jord/qgis_utilities/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/helpers/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/importing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.474913 Jord-0.0.8/jord/qgis_utilities/numpy_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/numpy_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/numpy_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/numpy_utilities/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/numpy_utilities/data_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/numpy_utilities/rasters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.474913 Jord-0.0.8/jord/qgis_utilities/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/qlive_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/qlive_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/qlive_utilities/procedure_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/qlive_utilities/rpc_protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.478913 Jord-0.0.8/jord/qgis_utilities/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/shapely_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/shapely_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qgis_utilities/styling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.478913 Jord-0.0.8/jord/qlive_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qlive_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qlive_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qlive_utilities/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qlive_utilities/procedures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qlive_utilities/serialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qlive_utilities/uri_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.478913 Jord-0.0.8/jord/qt_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qt_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/qt_utilities/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.478913 Jord-0.0.8/jord/rasterio_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/rasterio_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/rasterio_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.482913 Jord-0.0.8/jord/shapely_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.482913 Jord-0.0.8/jord/shapely_utilities/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/analysis/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/analysis/degrees_of_freedom.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/analysis/tracing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/clamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/geometry_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14249 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/mirroring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/morphology.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/points.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/sanitise_poly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.482913 Jord-0.0.8/jord/shapely_utilities/serialisation/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/serialisation/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/serialisation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/serialisation/well_known_binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/serialisation/well_known_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/shapely_utilities/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.482913 Jord-0.0.8/jord/torch_utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/torch_utilities/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/torch_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-22 13:51:10.000000 Jord-0.0.8/jord/torch_utilities/geodata_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-22 13:51:10.000000 Jord-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-22 13:51:10.000000 Jord-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-22 13:51:21.486913 Jord-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-06-22 13:51:10.000000 Jord-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.486913 Jord-0.0.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 13:51:21.486913 Jord-0.0.8/tests/qgis/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-22 13:51:10.000000 Jord-0.0.8/tests/qgis/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-22 13:51:10.000000 Jord-0.0.8/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-22 13:51:10.000000 Jord-0.0.8/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.417179 Jord-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-06-23 15:08:02.000000 Jord-0.0.9/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-23 15:08:02.000000 Jord-0.0.9/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 15:08:02.000000 Jord-0.0.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:02.000000 Jord-0.0.9/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.421179 Jord-0.0.9/Jord.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-23 15:08:07.000000 Jord-0.0.9/Jord.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-06-23 15:08:07.000000 Jord-0.0.9/Jord.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:08:07.000000 Jord-0.0.9/Jord.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-23 15:08:07.000000 Jord-0.0.9/Jord.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-23 15:08:07.000000 Jord-0.0.9/Jord.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-23 15:08:02.000000 Jord-0.0.9/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-06-23 15:08:02.000000 Jord-0.0.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-23 15:08:02.000000 Jord-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-23 15:08:07.433179 Jord-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-06-23 15:08:02.000000 Jord-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-23 15:08:02.000000 Jord-0.0.9/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.421179 Jord-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 15:08:02.000000 Jord-0.0.9/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.421179 Jord-0.0.9/jord/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.421179 Jord-0.0.9/jord/gdal_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/cloning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/importing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/gdal_utilities/spatial_reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.421179 Jord-0.0.9/jord/geojson_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/geojson_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/geojson_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/geojson_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.421179 Jord-0.0.9/jord/geopandas_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/geopandas_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/geopandas_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/geopandas_utilities/geometry_filtering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.421179 Jord-0.0.9/jord/pillow_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/pillow_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/pillow_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/pillow_utilities/exif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/pillow_utilities/tiff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.425179 Jord-0.0.9/jord/qgis_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/categorisation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.425179 Jord-0.0.9/jord/qgis_utilities/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/configuration/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/configuration/plugin_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/configuration/project_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.425179 Jord-0.0.9/jord/qgis_utilities/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/conversion/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/conversion/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/geometry_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.425179 Jord-0.0.9/jord/qgis_utilities/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/helpers/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/importing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.425179 Jord-0.0.9/jord/qgis_utilities/numpy_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/numpy_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/numpy_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/numpy_utilities/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/numpy_utilities/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/numpy_utilities/rasters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.429179 Jord-0.0.9/jord/qgis_utilities/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/qlive_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/qlive_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/qlive_utilities/procedure_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/qlive_utilities/rpc_protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.429179 Jord-0.0.9/jord/qgis_utilities/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/shapely_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/shapely_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qgis_utilities/styling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.429179 Jord-0.0.9/jord/qlive_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qlive_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qlive_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qlive_utilities/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12907 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qlive_utilities/procedures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qlive_utilities/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qlive_utilities/uri_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.429179 Jord-0.0.9/jord/qt_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qt_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/qt_utilities/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.429179 Jord-0.0.9/jord/rasterio_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/rasterio_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/rasterio_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/jord/shapely_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/jord/shapely_utilities/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/analysis/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/analysis/degrees_of_freedom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/analysis/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/clamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/geometry_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14249 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/mirroring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7780 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/sanitise_poly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/jord/shapely_utilities/serialisation/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/serialisation/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/serialisation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/serialisation/well_known_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/serialisation/well_known_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/shapely_utilities/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/jord/spatialite_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/spatialite_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/spatialite_utilities/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/jord/torch_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/torch_utilities/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/torch_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-23 15:08:02.000000 Jord-0.0.9/jord/torch_utilities/geodata_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-23 15:08:02.000000 Jord-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-23 15:08:02.000000 Jord-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-23 15:08:07.433179 Jord-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9613 2023-06-23 15:08:02.000000 Jord-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:08:07.433179 Jord-0.0.9/tests/qgis/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-23 15:08:02.000000 Jord-0.0.9/tests/qgis/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-23 15:08:02.000000 Jord-0.0.9/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-23 15:08:02.000000 Jord-0.0.9/tests/test_sanity.py
```

### Comparing `Jord-0.0.8/.github/CODE_OF_CONDUCT.md` & `Jord-0.0.9/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/.github/CONTRIBUTING.md` & `Jord-0.0.9/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/Jord.egg-info/PKG-INFO` & `Jord-0.0.9/Jord.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
 License: Apache License, Version 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jord Version: 0.0.8 Home-page: https://github.com/
+Metadata-Version: 2.1 Name: Jord Version: 0.0.9 Home-page: https://github.com/
 aivclab/jord Download-URL: https://github.com/aivclab/jord/releases Author:
 Christian Heider Nielsen Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen Maintainer-email:
 christian.heider@alexandra.dk License: Apache License, Version 2.0 Keywords:
 python computer vision neo droid Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Developers Classifier: License :: OSI
```

### Comparing `Jord-0.0.8/Jord.egg-info/SOURCES.txt` & `Jord-0.0.9/Jord.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -102,13 +102,15 @@
 jord/shapely_utilities/analysis/__init__.py
 jord/shapely_utilities/analysis/degrees_of_freedom.py
 jord/shapely_utilities/analysis/tracing.py
 jord/shapely_utilities/serialisation/README.md
 jord/shapely_utilities/serialisation/__init__.py
 jord/shapely_utilities/serialisation/well_known_binary.py
 jord/shapely_utilities/serialisation/well_known_text.py
+jord/spatialite_utilities/__init__.py
+jord/spatialite_utilities/loading.py
 jord/torch_utilities/README.md
 jord/torch_utilities/__init__.py
 jord/torch_utilities/geodata_dataset.py
 tests/test_import.py
 tests/test_sanity.py
 tests/qgis/README.md
```

### Comparing `Jord-0.0.8/Jord.egg-info/requires.txt` & `Jord-0.0.9/Jord.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,58 @@
 numpy>=1.20.2
 warg>=1.1.6
 apppath>=1.0.2
 sorcery
 pyzmq
 
 [all]
-pip>=22.1.2
-coveralls>=1.6.0
 pytest>=4.3.0
-pytest>=4.4.1
-pytest-cov>=2.11.1
-sphinx>=4.0.1
 warg>=1.1.6
-Pillow
-mock
-pyzmq
-wheel>=0.33.0
-sphinxcontrib-programoutput
-numpy>=1.20.2
 furo
 twine>=1.13.0
-apppath>=1.0.2
+pyzmq
+Pillow
+coveralls>=1.6.0
+sphinxcontrib-programoutput
 pre-commit>=2.17.0
+apppath>=1.0.2
+wheel>=0.33.0
+mock
+pytest-cov>=2.11.1
 black[jupyter]>=21.5b0
+numpy>=1.20.2
 sorcery
+pip>=22.1.2
+pytest>=4.4.1
+sphinx>=4.0.1
 
 [dev]
-furo
-twine>=1.13.0
 pip>=22.1.2
-mock
-coveralls>=1.6.0
 wheel>=0.33.0
-warg>=1.1.6
-pyzmq
-pytest-cov>=2.11.1
+coveralls>=1.6.0
 pytest>=4.3.0
 pytest>=4.4.1
-apppath>=1.0.2
-pre-commit>=2.17.0
+mock
+pytest-cov>=2.11.1
 sphinxcontrib-programoutput
-sorcery
-sphinx>=4.0.1
+warg>=1.1.6
+pre-commit>=2.17.0
 black[jupyter]>=21.5b0
+twine>=1.13.0
+furo
+sphinx>=4.0.1
+pyzmq
+apppath>=1.0.2
 numpy>=1.20.2
+sorcery
 
 [docs]
+furo
 sphinxcontrib-programoutput
 sphinx>=4.0.1
-furo
 
 [extra]
 
 [gdal]
 
 [pil]
 Pillow
```

### Comparing `Jord-0.0.8/LICENSE.md` & `Jord-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/PKG-INFO` & `Jord-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Jord
-Version: 0.0.8
+Version: 0.0.9
 Home-page: https://github.com/aivclab/jord
 Download-URL: https://github.com/aivclab/jord/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
 License: Apache License, Version 2.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Jord Version: 0.0.8 Home-page: https://github.com/
+Metadata-Version: 2.1 Name: Jord Version: 0.0.9 Home-page: https://github.com/
 aivclab/jord Download-URL: https://github.com/aivclab/jord/releases Author:
 Christian Heider Nielsen Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen Maintainer-email:
 christian.heider@alexandra.dk License: Apache License, Version 2.0 Keywords:
 python computer vision neo droid Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Developers Classifier: License :: OSI
```

### Comparing `Jord-0.0.8/README.md` & `Jord-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/SECURITY.md` & `Jord-0.0.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/__init__.py` & `Jord-0.0.9/jord/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import pkg_resources
 from apppath import AppPath
 from warg import dist_is_editable
 
 __project__ = "Jord"
 __author__ = "Christian Heider Nielsen"
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 __doc__ = r"""
 .. module:: jord
    :platform: Unix, Windows
    :synopsis: A set of general tools build for geo data.
 
 .. moduleauthor:: Christian Heider Nielsen <christian.heider@alexandra.dk>
 
@@ -29,15 +29,15 @@
 with open(Path(__file__).parent / "README.md", "r") as this_init_file:
     __doc__ += this_init_file.read()
 
 PROJECT_NAME = __project__.lower().strip().replace(" ", "_")
 PROJECT_VERSION = __version__
 PROJECT_YEAR = 2018
 PROJECT_AUTHOR = __author__.lower().strip().replace(" ", "_")
-PROJECT_ORGANISATION = "Aivclab"
+PROJECT_ORGANISATION = "Automaps"
 PROJECT_APP_PATH = AppPath(app_name=PROJECT_NAME, app_author=PROJECT_AUTHOR)
 PACKAGE_DATA_PATH = Path(pkg_resources.resource_filename(PROJECT_NAME, "data"))
 INCLUDE_PROJECT_READMES = False
 
 distributions = {v.key: v for v in pkg_resources.working_set}
 if PROJECT_NAME in distributions:
     distribution = distributions[PROJECT_NAME]
@@ -56,15 +56,14 @@
     version = __version__
     if not version:
         version = os.getenv("VERSION", "0.0.0")
 
     if append_time:
         now = datetime.datetime.utcnow()
         date_version = now.strftime("%Y%m%d%H%M%S")
-        # date_version = time.time()
 
         if version:
             # Most git tags are prefixed with 'v' (example: v1.2.3) this is
             # never desirable for artifact repositories, so we strip the
             # leading 'v' if it's present.
             version = (
                 version[1:]
```

### Comparing `Jord-0.0.8/jord/gdal_utilities/__init__.py` & `Jord-0.0.9/jord/gdal_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/gdal_utilities/cloning.py` & `Jord-0.0.9/jord/gdal_utilities/cloning.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/gdal_utilities/context.py` & `Jord-0.0.9/jord/gdal_utilities/context.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/gdal_utilities/conversion.py` & `Jord-0.0.9/jord/gdal_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/gdal_utilities/importing.py` & `Jord-0.0.9/jord/gdal_utilities/importing.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/gdal_utilities/persistence.py` & `Jord-0.0.9/jord/gdal_utilities/persistence.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/geojson_utilities/geometry_types.py` & `Jord-0.0.9/jord/geojson_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/geopandas_utilities/geometry_filtering.py` & `Jord-0.0.9/jord/geopandas_utilities/geometry_filtering.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/__init__.py` & `Jord-0.0.9/jord/qgis_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/categorisation.py` & `Jord-0.0.9/jord/qgis_utilities/categorisation.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/configuration/plugin_settings.py` & `Jord-0.0.9/jord/qgis_utilities/configuration/plugin_settings.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/configuration/project_settings.py` & `Jord-0.0.9/jord/qgis_utilities/configuration/project_settings.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/enums.py` & `Jord-0.0.9/jord/qgis_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/geometry_types.py` & `Jord-0.0.9/jord/qgis_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/helpers/actions.py` & `Jord-0.0.9/jord/qgis_utilities/helpers/actions.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/helpers/drawing.py` & `Jord-0.0.9/jord/qgis_utilities/helpers/drawing.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/helpers/environment.py` & `Jord-0.0.9/jord/qgis_utilities/helpers/environment.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/helpers/models.py` & `Jord-0.0.9/jord/qgis_utilities/helpers/models.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/helpers/progress_bar.py` & `Jord-0.0.9/jord/qgis_utilities/helpers/progress_bar.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/helpers/signals.py` & `Jord-0.0.9/jord/qgis_utilities/helpers/signals.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/helpers/timestamp.py` & `Jord-0.0.9/jord/qgis_utilities/helpers/timestamp.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/numpy_utilities/conversion.py` & `Jord-0.0.9/jord/qgis_utilities/numpy_utilities/conversion.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/numpy_utilities/data_type.py` & `Jord-0.0.9/jord/qgis_utilities/numpy_utilities/data_type.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py` & `Jord-0.0.9/jord/qgis_utilities/numpy_utilities/numpy_image_widget.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py` & `Jord-0.0.9/jord/qgis_utilities/shapely_utilities/temp_layer_persistence.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qgis_utilities/styling.py` & `Jord-0.0.9/jord/qgis_utilities/styling.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qlive_utilities/client.py` & `Jord-0.0.9/jord/qlive_utilities/client.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qlive_utilities/procedures.py` & `Jord-0.0.9/jord/qlive_utilities/procedures.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qlive_utilities/serialisation.py` & `Jord-0.0.9/jord/qlive_utilities/serialisation.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qlive_utilities/uri_utilities.py` & `Jord-0.0.9/jord/qlive_utilities/uri_utilities.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/qt_utilities/enums.py` & `Jord-0.0.9/jord/qt_utilities/enums.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/shapely_utilities/__init__.py` & `Jord-0.0.9/jord/shapely_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/shapely_utilities/clamp.py` & `Jord-0.0.9/jord/shapely_utilities/clamp.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/shapely_utilities/geometry_types.py` & `Jord-0.0.9/jord/shapely_utilities/geometry_types.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/shapely_utilities/iteration.py` & `Jord-0.0.9/jord/shapely_utilities/iteration.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/shapely_utilities/lines.py` & `Jord-0.0.9/jord/shapely_utilities/lines.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/shapely_utilities/mirroring.py` & `Jord-0.0.9/jord/shapely_utilities/mirroring.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/shapely_utilities/morphology.py` & `Jord-0.0.9/jord/shapely_utilities/morphology.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/shapely_utilities/points.py` & `Jord-0.0.9/jord/shapely_utilities/points.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/shapely_utilities/projection.py` & `Jord-0.0.9/jord/shapely_utilities/projection.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/shapely_utilities/sanitise_poly.py` & `Jord-0.0.9/jord/shapely_utilities/sanitise_poly.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/shapely_utilities/serialisation/well_known_binary.py` & `Jord-0.0.9/jord/shapely_utilities/serialisation/well_known_binary.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/shapely_utilities/serialisation/well_known_text.py` & `Jord-0.0.9/jord/shapely_utilities/serialisation/well_known_text.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/jord/shapely_utilities/transformation.py` & `Jord-0.0.9/jord/shapely_utilities/transformation.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/setup.py` & `Jord-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `Jord-0.0.8/tests/test_import.py` & `Jord-0.0.9/tests/test_import.py`

 * *Files identical despite different names*

