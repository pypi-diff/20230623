# Comparing `tmp/arlas-api-9.0.0.tar.gz` & `tmp/arlas-api-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arlas-api-9.0.0.tar", last modified: Tue Nov 27 08:07:09 2018, max compression
+gzip compressed data, was "dist/arlas-api-9.0.1.tar", last modified: Fri Dec 14 19:09:06 2018, max compression
```

## Comparing `arlas-api-9.0.0.tar` & `arlas-api-9.0.1.tar`

### file list

```diff
@@ -1,138 +1,138 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-11-27 08:07:05.000000 arlas-api-9.0.0/
--rw-r--r--   0 root         (0) root         (0)      327 2018-11-27 08:07:05.000000 arlas-api-9.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7715 2018-11-27 08:06:48.000000 arlas-api-9.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-11-27 08:07:04.000000 arlas-api-9.0.0/arlas_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      327 2018-11-27 08:07:04.000000 arlas-api-9.0.0/arlas_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4190 2018-11-27 08:07:04.000000 arlas-api-9.0.0/arlas_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2018-11-27 08:07:04.000000 arlas-api-9.0.0/arlas_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2018-11-27 08:07:04.000000 arlas-api-9.0.0/arlas_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2018-11-27 08:07:04.000000 arlas-api-9.0.0/arlas_api.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-11-27 08:07:04.000000 arlas-api-9.0.0/arlas_api_python/
--rw-r--r--   0 root         (0) root         (0)     3068 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24183 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-11-27 08:07:04.000000 arlas-api-9.0.0/arlas_api_python/apis/
--rw-r--r--   0 root         (0) root         (0)      183 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27454 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/apis/collections_api.py
--rw-r--r--   0 root         (0) root         (0)   197800 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/apis/explore_api.py
--rw-r--r--   0 root         (0) root         (0)    10434 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/apis/write_api.py
--rw-r--r--   0 root         (0) root         (0)     6809 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-11-27 08:07:05.000000 arlas-api-9.0.0/arlas_api_python/models/
--rw-r--r--   0 root         (0) root         (0)     2397 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3897 2018-11-27 08:06:46.000000 arlas-api-9.0.0/arlas_api_python/models/aggregated_geometry.py
--rw-r--r--   0 root         (0) root         (0)     9070 2018-11-27 08:06:46.000000 arlas-api-9.0.0/arlas_api_python/models/aggregation.py
--rw-r--r--   0 root         (0) root         (0)     4107 2018-11-27 08:06:46.000000 arlas-api-9.0.0/arlas_api_python/models/aggregation_metric.py
--rw-r--r--   0 root         (0) root         (0)     9838 2018-11-27 08:06:46.000000 arlas-api-9.0.0/arlas_api_python/models/aggregation_response.py
--rw-r--r--   0 root         (0) root         (0)     4342 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/aggregations_request.py
--rw-r--r--   0 root         (0) root         (0)     4730 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/bbox.py
--rw-r--r--   0 root         (0) root         (0)     4004 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/collection_reference.py
--rw-r--r--   0 root         (0) root         (0)     5004 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/collection_reference_description.py
--rw-r--r--   0 root         (0) root         (0)     5916 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/collection_reference_description_property.py
--rw-r--r--   0 root         (0) root         (0)    18180 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/collection_reference_parameters.py
--rw-r--r--   0 root         (0) root         (0)     3409 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/count.py
--rw-r--r--   0 root         (0) root         (0)     3737 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/crs.py
--rw-r--r--   0 root         (0) root         (0)    12323 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/dublin_core_element_name.py
--rw-r--r--   0 root         (0) root         (0)     3998 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/error.py
--rw-r--r--   0 root         (0) root         (0)     4226 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/expression.py
--rw-r--r--   0 root         (0) root         (0)     3928 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/failure.py
--rw-r--r--   0 root         (0) root         (0)     5202 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/feature.py
--rw-r--r--   0 root         (0) root         (0)     4172 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/feature_collection.py
--rw-r--r--   0 root         (0) root         (0)     6367 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/feed.py
--rw-r--r--   0 root         (0) root         (0)     7367 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/filter.py
--rw-r--r--   0 root         (0) root         (0)     3392 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/form.py
--rw-r--r--   0 root         (0) root         (0)     3978 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/generator.py
--rw-r--r--   0 root         (0) root         (0)     3449 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/geo_json_object.py
--rw-r--r--   0 root         (0) root         (0)     4245 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/geometry_collection.py
--rw-r--r--   0 root         (0) root         (0)     3301 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/hit.py
--rw-r--r--   0 root         (0) root         (0)     4618 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/hits.py
--rw-r--r--   0 root         (0) root         (0)     8443 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/inspire.py
--rw-r--r--   0 root         (0) root         (0)     4888 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/inspire_limitation_access.py
--rw-r--r--   0 root         (0) root         (0)     3815 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/inspire_spatial_resolution.py
--rw-r--r--   0 root         (0) root         (0)     3512 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/inspire_uri.py
--rw-r--r--   0 root         (0) root         (0)     3714 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/interval.py
--rw-r--r--   0 root         (0) root         (0)     4348 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/keyword.py
--rw-r--r--   0 root         (0) root         (0)     4133 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/line_string.py
--rw-r--r--   0 root         (0) root         (0)     2347 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/lng_lat_alt.py
--rw-r--r--   0 root         (0) root         (0)     4622 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/md.py
--rw-r--r--   0 root         (0) root         (0)     4000 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/metric.py
--rw-r--r--   0 root         (0) root         (0)     4226 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/multi_line_string.py
--rw-r--r--   0 root         (0) root         (0)     4133 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/multi_point.py
--rw-r--r--   0 root         (0) root         (0)     4199 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/multi_polygon.py
--rw-r--r--   0 root         (0) root         (0)     2338 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/number.py
--rw-r--r--   0 root         (0) root         (0)    13106 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/open_search.py
--rw-r--r--   0 root         (0) root         (0)     3893 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/person.py
--rw-r--r--   0 root         (0) root         (0)     4040 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/point.py
--rw-r--r--   0 root         (0) root         (0)     4106 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/polygon.py
--rw-r--r--   0 root         (0) root         (0)     3572 2018-11-27 08:06:47.000000 arlas-api-9.0.0/arlas_api_python/models/projection.py
--rw-r--r--   0 root         (0) root         (0)     4055 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/range_request.py
--rw-r--r--   0 root         (0) root         (0)     5382 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/range_response.py
--rw-r--r--   0 root         (0) root         (0)     5531 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/raster_tile_url.py
--rw-r--r--   0 root         (0) root         (0)     5142 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/search.py
--rw-r--r--   0 root         (0) root         (0)     3365 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/size.py
--rw-r--r--   0 root         (0) root         (0)     2829 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/sort.py
--rw-r--r--   0 root         (0) root         (0)     3479 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/success.py
--rw-r--r--   0 root         (0) root         (0)     3364 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/tag.py
--rw-r--r--   0 root         (0) root         (0)     3441 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/tag_request.py
--rw-r--r--   0 root         (0) root         (0)     5080 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/models/update_response.py
--rw-r--r--   0 root         (0) root         (0)    12823 2018-11-27 08:06:48.000000 arlas-api-9.0.0/arlas_api_python/rest.py
--rw-r--r--   0 root         (0) root         (0)       38 2018-11-27 08:07:05.000000 arlas-api-9.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      965 2018-11-27 08:07:02.000000 arlas-api-9.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2018-11-27 08:07:05.000000 arlas-api-9.0.0/test/
--rw-r--r--   0 root         (0) root         (0)        0 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/__init__.py
--rw-r--r--   0 root         (0) root         (0)      947 2018-11-27 08:06:46.000000 arlas-api-9.0.0/test/test_aggregated_geometry.py
--rw-r--r--   0 root         (0) root         (0)      889 2018-11-27 08:06:46.000000 arlas-api-9.0.0/test/test_aggregation.py
--rw-r--r--   0 root         (0) root         (0)      939 2018-11-27 08:06:46.000000 arlas-api-9.0.0/test/test_aggregation_metric.py
--rw-r--r--   0 root         (0) root         (0)      955 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_aggregation_response.py
--rw-r--r--   0 root         (0) root         (0)      955 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_aggregations_request.py
--rw-r--r--   0 root         (0) root         (0)      833 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_bbox.py
--rw-r--r--   0 root         (0) root         (0)      955 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_collection_reference.py
--rw-r--r--   0 root         (0) root         (0)     1045 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_collection_reference_description.py
--rw-r--r--   0 root         (0) root         (0)     1111 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_collection_reference_description_property.py
--rw-r--r--   0 root         (0) root         (0)     1037 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_collection_reference_parameters.py
--rw-r--r--   0 root         (0) root         (0)     1590 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_collections_api.py
--rw-r--r--   0 root         (0) root         (0)      841 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_count.py
--rw-r--r--   0 root         (0) root         (0)      825 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_crs.py
--rw-r--r--   0 root         (0) root         (0)      975 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_dublin_core_element_name.py
--rw-r--r--   0 root         (0) root         (0)      841 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_error.py
--rw-r--r--   0 root         (0) root         (0)     3189 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_explore_api.py
--rw-r--r--   0 root         (0) root         (0)      881 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_expression.py
--rw-r--r--   0 root         (0) root         (0)      857 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_failure.py
--rw-r--r--   0 root         (0) root         (0)      857 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_feature.py
--rw-r--r--   0 root         (0) root         (0)      939 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_feature_collection.py
--rw-r--r--   0 root         (0) root         (0)      833 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_feed.py
--rw-r--r--   0 root         (0) root         (0)      849 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_filter.py
--rw-r--r--   0 root         (0) root         (0)      833 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_form.py
--rw-r--r--   0 root         (0) root         (0)      873 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_generator.py
--rw-r--r--   0 root         (0) root         (0)      909 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_geo_json_object.py
--rw-r--r--   0 root         (0) root         (0)      947 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_geometry_collection.py
--rw-r--r--   0 root         (0) root         (0)      825 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_hit.py
--rw-r--r--   0 root         (0) root         (0)      833 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_hits.py
--rw-r--r--   0 root         (0) root         (0)      857 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_inspire.py
--rw-r--r--   0 root         (0) root         (0)      989 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_inspire_limitation_access.py
--rw-r--r--   0 root         (0) root         (0)      997 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_inspire_spatial_resolution.py
--rw-r--r--   0 root         (0) root         (0)      883 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_inspire_uri.py
--rw-r--r--   0 root         (0) root         (0)      865 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_interval.py
--rw-r--r--   0 root         (0) root         (0)      857 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_keyword.py
--rw-r--r--   0 root         (0) root         (0)      883 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_line_string.py
--rw-r--r--   0 root         (0) root         (0)      877 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_lng_lat_alt.py
--rw-r--r--   0 root         (0) root         (0)      817 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_md.py
--rw-r--r--   0 root         (0) root         (0)      849 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_metric.py
--rw-r--r--   0 root         (0) root         (0)      925 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_multi_line_string.py
--rw-r--r--   0 root         (0) root         (0)      883 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_multi_point.py
--rw-r--r--   0 root         (0) root         (0)      899 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_multi_polygon.py
--rw-r--r--   0 root         (0) root         (0)      849 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_number.py
--rw-r--r--   0 root         (0) root         (0)      883 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_open_search.py
--rw-r--r--   0 root         (0) root         (0)      849 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_person.py
--rw-r--r--   0 root         (0) root         (0)      841 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_point.py
--rw-r--r--   0 root         (0) root         (0)      857 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_polygon.py
--rw-r--r--   0 root         (0) root         (0)      881 2018-11-27 08:06:47.000000 arlas-api-9.0.0/test/test_projection.py
--rw-r--r--   0 root         (0) root         (0)      899 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_range_request.py
--rw-r--r--   0 root         (0) root         (0)      907 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_range_response.py
--rw-r--r--   0 root         (0) root         (0)      909 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_raster_tile_url.py
--rw-r--r--   0 root         (0) root         (0)      849 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_search.py
--rw-r--r--   0 root         (0) root         (0)      833 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_size.py
--rw-r--r--   0 root         (0) root         (0)      833 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_sort.py
--rw-r--r--   0 root         (0) root         (0)      857 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_success.py
--rw-r--r--   0 root         (0) root         (0)      825 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_tag.py
--rw-r--r--   0 root         (0) root         (0)      883 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_tag_request.py
--rw-r--r--   0 root         (0) root         (0)      915 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_update_response.py
--rw-r--r--   0 root         (0) root         (0)      912 2018-11-27 08:06:48.000000 arlas-api-9.0.0/test/test_write_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-12-14 19:09:05.000000 arlas-api-9.0.1/
+-rw-r--r--   0 root         (0) root         (0)      327 2018-12-14 19:09:05.000000 arlas-api-9.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7715 2018-12-14 19:08:45.000000 arlas-api-9.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-12-14 19:09:03.000000 arlas-api-9.0.1/arlas_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      327 2018-12-14 19:09:02.000000 arlas-api-9.0.1/arlas_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4190 2018-12-14 19:09:03.000000 arlas-api-9.0.1/arlas_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2018-12-14 19:09:02.000000 arlas-api-9.0.1/arlas_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2018-12-14 19:09:02.000000 arlas-api-9.0.1/arlas_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2018-12-14 19:09:02.000000 arlas-api-9.0.1/arlas_api.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-12-14 19:09:03.000000 arlas-api-9.0.1/arlas_api_python/
+-rw-r--r--   0 root         (0) root         (0)     3068 2018-12-14 19:08:45.000000 arlas-api-9.0.1/arlas_api_python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24183 2018-12-14 19:08:45.000000 arlas-api-9.0.1/arlas_api_python/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-12-14 19:09:03.000000 arlas-api-9.0.1/arlas_api_python/apis/
+-rw-r--r--   0 root         (0) root         (0)      183 2018-12-14 19:08:45.000000 arlas-api-9.0.1/arlas_api_python/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27454 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/apis/collections_api.py
+-rw-r--r--   0 root         (0) root         (0)   197800 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/apis/explore_api.py
+-rw-r--r--   0 root         (0) root         (0)    10434 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/apis/write_api.py
+-rw-r--r--   0 root         (0) root         (0)     6809 2018-12-14 19:08:45.000000 arlas-api-9.0.1/arlas_api_python/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-12-14 19:09:04.000000 arlas-api-9.0.1/arlas_api_python/models/
+-rw-r--r--   0 root         (0) root         (0)     2397 2018-12-14 19:08:45.000000 arlas-api-9.0.1/arlas_api_python/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3897 2018-12-14 19:08:42.000000 arlas-api-9.0.1/arlas_api_python/models/aggregated_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     9070 2018-12-14 19:08:42.000000 arlas-api-9.0.1/arlas_api_python/models/aggregation.py
+-rw-r--r--   0 root         (0) root         (0)     4107 2018-12-14 19:08:42.000000 arlas-api-9.0.1/arlas_api_python/models/aggregation_metric.py
+-rw-r--r--   0 root         (0) root         (0)     9838 2018-12-14 19:08:42.000000 arlas-api-9.0.1/arlas_api_python/models/aggregation_response.py
+-rw-r--r--   0 root         (0) root         (0)     4342 2018-12-14 19:08:42.000000 arlas-api-9.0.1/arlas_api_python/models/aggregations_request.py
+-rw-r--r--   0 root         (0) root         (0)     4730 2018-12-14 19:08:42.000000 arlas-api-9.0.1/arlas_api_python/models/bbox.py
+-rw-r--r--   0 root         (0) root         (0)     4004 2018-12-14 19:08:42.000000 arlas-api-9.0.1/arlas_api_python/models/collection_reference.py
+-rw-r--r--   0 root         (0) root         (0)     5004 2018-12-14 19:08:42.000000 arlas-api-9.0.1/arlas_api_python/models/collection_reference_description.py
+-rw-r--r--   0 root         (0) root         (0)     5916 2018-12-14 19:08:42.000000 arlas-api-9.0.1/arlas_api_python/models/collection_reference_description_property.py
+-rw-r--r--   0 root         (0) root         (0)    18180 2018-12-14 19:08:42.000000 arlas-api-9.0.1/arlas_api_python/models/collection_reference_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     3409 2018-12-14 19:08:42.000000 arlas-api-9.0.1/arlas_api_python/models/count.py
+-rw-r--r--   0 root         (0) root         (0)     3737 2018-12-14 19:08:42.000000 arlas-api-9.0.1/arlas_api_python/models/crs.py
+-rw-r--r--   0 root         (0) root         (0)    12323 2018-12-14 19:08:42.000000 arlas-api-9.0.1/arlas_api_python/models/dublin_core_element_name.py
+-rw-r--r--   0 root         (0) root         (0)     3998 2018-12-14 19:08:42.000000 arlas-api-9.0.1/arlas_api_python/models/error.py
+-rw-r--r--   0 root         (0) root         (0)     4226 2018-12-14 19:08:42.000000 arlas-api-9.0.1/arlas_api_python/models/expression.py
+-rw-r--r--   0 root         (0) root         (0)     3928 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/failure.py
+-rw-r--r--   0 root         (0) root         (0)     5202 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/feature.py
+-rw-r--r--   0 root         (0) root         (0)     4172 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/feature_collection.py
+-rw-r--r--   0 root         (0) root         (0)     6367 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/feed.py
+-rw-r--r--   0 root         (0) root         (0)     7367 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/filter.py
+-rw-r--r--   0 root         (0) root         (0)     3392 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/form.py
+-rw-r--r--   0 root         (0) root         (0)     3978 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/generator.py
+-rw-r--r--   0 root         (0) root         (0)     3449 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/geo_json_object.py
+-rw-r--r--   0 root         (0) root         (0)     4245 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/models/geometry_collection.py
+-rw-r--r--   0 root         (0) root         (0)     3301 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/hit.py
+-rw-r--r--   0 root         (0) root         (0)     4618 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/hits.py
+-rw-r--r--   0 root         (0) root         (0)     8443 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/inspire.py
+-rw-r--r--   0 root         (0) root         (0)     4888 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/inspire_limitation_access.py
+-rw-r--r--   0 root         (0) root         (0)     3815 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/inspire_spatial_resolution.py
+-rw-r--r--   0 root         (0) root         (0)     3512 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/inspire_uri.py
+-rw-r--r--   0 root         (0) root         (0)     3714 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/interval.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/keyword.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/models/line_string.py
+-rw-r--r--   0 root         (0) root         (0)     2347 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/lng_lat_alt.py
+-rw-r--r--   0 root         (0) root         (0)     4622 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/md.py
+-rw-r--r--   0 root         (0) root         (0)     4000 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/metric.py
+-rw-r--r--   0 root         (0) root         (0)     4226 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/models/multi_line_string.py
+-rw-r--r--   0 root         (0) root         (0)     4133 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/models/multi_point.py
+-rw-r--r--   0 root         (0) root         (0)     4199 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/models/multi_polygon.py
+-rw-r--r--   0 root         (0) root         (0)     2338 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/number.py
+-rw-r--r--   0 root         (0) root         (0)    13106 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/open_search.py
+-rw-r--r--   0 root         (0) root         (0)     3893 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/person.py
+-rw-r--r--   0 root         (0) root         (0)     4040 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/models/point.py
+-rw-r--r--   0 root         (0) root         (0)     4106 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/models/polygon.py
+-rw-r--r--   0 root         (0) root         (0)     3572 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/projection.py
+-rw-r--r--   0 root         (0) root         (0)     4055 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/range_request.py
+-rw-r--r--   0 root         (0) root         (0)     5382 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/range_response.py
+-rw-r--r--   0 root         (0) root         (0)     5531 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/raster_tile_url.py
+-rw-r--r--   0 root         (0) root         (0)     5142 2018-12-14 19:08:43.000000 arlas-api-9.0.1/arlas_api_python/models/search.py
+-rw-r--r--   0 root         (0) root         (0)     3365 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/models/size.py
+-rw-r--r--   0 root         (0) root         (0)     2829 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/models/sort.py
+-rw-r--r--   0 root         (0) root         (0)     3479 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/models/success.py
+-rw-r--r--   0 root         (0) root         (0)     3364 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/models/tag.py
+-rw-r--r--   0 root         (0) root         (0)     3441 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/models/tag_request.py
+-rw-r--r--   0 root         (0) root         (0)     5080 2018-12-14 19:08:44.000000 arlas-api-9.0.1/arlas_api_python/models/update_response.py
+-rw-r--r--   0 root         (0) root         (0)    12823 2018-12-14 19:08:45.000000 arlas-api-9.0.1/arlas_api_python/rest.py
+-rw-r--r--   0 root         (0) root         (0)       38 2018-12-14 19:09:05.000000 arlas-api-9.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      965 2018-12-14 19:09:00.000000 arlas-api-9.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2018-12-14 19:09:05.000000 arlas-api-9.0.1/test/
+-rw-r--r--   0 root         (0) root         (0)        0 2018-12-14 19:08:45.000000 arlas-api-9.0.1/test/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      947 2018-12-14 19:08:42.000000 arlas-api-9.0.1/test/test_aggregated_geometry.py
+-rw-r--r--   0 root         (0) root         (0)      889 2018-12-14 19:08:42.000000 arlas-api-9.0.1/test/test_aggregation.py
+-rw-r--r--   0 root         (0) root         (0)      939 2018-12-14 19:08:42.000000 arlas-api-9.0.1/test/test_aggregation_metric.py
+-rw-r--r--   0 root         (0) root         (0)      955 2018-12-14 19:08:42.000000 arlas-api-9.0.1/test/test_aggregation_response.py
+-rw-r--r--   0 root         (0) root         (0)      955 2018-12-14 19:08:42.000000 arlas-api-9.0.1/test/test_aggregations_request.py
+-rw-r--r--   0 root         (0) root         (0)      833 2018-12-14 19:08:42.000000 arlas-api-9.0.1/test/test_bbox.py
+-rw-r--r--   0 root         (0) root         (0)      955 2018-12-14 19:08:42.000000 arlas-api-9.0.1/test/test_collection_reference.py
+-rw-r--r--   0 root         (0) root         (0)     1045 2018-12-14 19:08:42.000000 arlas-api-9.0.1/test/test_collection_reference_description.py
+-rw-r--r--   0 root         (0) root         (0)     1111 2018-12-14 19:08:42.000000 arlas-api-9.0.1/test/test_collection_reference_description_property.py
+-rw-r--r--   0 root         (0) root         (0)     1037 2018-12-14 19:08:42.000000 arlas-api-9.0.1/test/test_collection_reference_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_collections_api.py
+-rw-r--r--   0 root         (0) root         (0)      841 2018-12-14 19:08:42.000000 arlas-api-9.0.1/test/test_count.py
+-rw-r--r--   0 root         (0) root         (0)      825 2018-12-14 19:08:42.000000 arlas-api-9.0.1/test/test_crs.py
+-rw-r--r--   0 root         (0) root         (0)      975 2018-12-14 19:08:42.000000 arlas-api-9.0.1/test/test_dublin_core_element_name.py
+-rw-r--r--   0 root         (0) root         (0)      841 2018-12-14 19:08:42.000000 arlas-api-9.0.1/test/test_error.py
+-rw-r--r--   0 root         (0) root         (0)     3189 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_explore_api.py
+-rw-r--r--   0 root         (0) root         (0)      881 2018-12-14 19:08:42.000000 arlas-api-9.0.1/test/test_expression.py
+-rw-r--r--   0 root         (0) root         (0)      857 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_failure.py
+-rw-r--r--   0 root         (0) root         (0)      857 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_feature.py
+-rw-r--r--   0 root         (0) root         (0)      939 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_feature_collection.py
+-rw-r--r--   0 root         (0) root         (0)      833 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_feed.py
+-rw-r--r--   0 root         (0) root         (0)      849 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_filter.py
+-rw-r--r--   0 root         (0) root         (0)      833 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_form.py
+-rw-r--r--   0 root         (0) root         (0)      873 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_generator.py
+-rw-r--r--   0 root         (0) root         (0)      909 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_geo_json_object.py
+-rw-r--r--   0 root         (0) root         (0)      947 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_geometry_collection.py
+-rw-r--r--   0 root         (0) root         (0)      825 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_hit.py
+-rw-r--r--   0 root         (0) root         (0)      833 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_hits.py
+-rw-r--r--   0 root         (0) root         (0)      857 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_inspire.py
+-rw-r--r--   0 root         (0) root         (0)      989 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_inspire_limitation_access.py
+-rw-r--r--   0 root         (0) root         (0)      997 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_inspire_spatial_resolution.py
+-rw-r--r--   0 root         (0) root         (0)      883 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_inspire_uri.py
+-rw-r--r--   0 root         (0) root         (0)      865 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_interval.py
+-rw-r--r--   0 root         (0) root         (0)      857 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_keyword.py
+-rw-r--r--   0 root         (0) root         (0)      883 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_line_string.py
+-rw-r--r--   0 root         (0) root         (0)      877 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_lng_lat_alt.py
+-rw-r--r--   0 root         (0) root         (0)      817 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_md.py
+-rw-r--r--   0 root         (0) root         (0)      849 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_metric.py
+-rw-r--r--   0 root         (0) root         (0)      925 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_multi_line_string.py
+-rw-r--r--   0 root         (0) root         (0)      883 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_multi_point.py
+-rw-r--r--   0 root         (0) root         (0)      899 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_multi_polygon.py
+-rw-r--r--   0 root         (0) root         (0)      849 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_number.py
+-rw-r--r--   0 root         (0) root         (0)      883 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_open_search.py
+-rw-r--r--   0 root         (0) root         (0)      849 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_person.py
+-rw-r--r--   0 root         (0) root         (0)      841 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_point.py
+-rw-r--r--   0 root         (0) root         (0)      857 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_polygon.py
+-rw-r--r--   0 root         (0) root         (0)      881 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_projection.py
+-rw-r--r--   0 root         (0) root         (0)      899 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_range_request.py
+-rw-r--r--   0 root         (0) root         (0)      907 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_range_response.py
+-rw-r--r--   0 root         (0) root         (0)      909 2018-12-14 19:08:43.000000 arlas-api-9.0.1/test/test_raster_tile_url.py
+-rw-r--r--   0 root         (0) root         (0)      849 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_search.py
+-rw-r--r--   0 root         (0) root         (0)      833 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_size.py
+-rw-r--r--   0 root         (0) root         (0)      833 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_sort.py
+-rw-r--r--   0 root         (0) root         (0)      857 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_success.py
+-rw-r--r--   0 root         (0) root         (0)      825 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_tag.py
+-rw-r--r--   0 root         (0) root         (0)      883 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_tag_request.py
+-rw-r--r--   0 root         (0) root         (0)      915 2018-12-14 19:08:44.000000 arlas-api-9.0.1/test/test_update_response.py
+-rw-r--r--   0 root         (0) root         (0)      912 2018-12-14 19:08:45.000000 arlas-api-9.0.1/test/test_write_api.py
```

### Comparing `arlas-api-9.0.0/README.md` & `arlas-api-9.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # arlas-api-python
 Explore the content of ARLAS collections
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 9.0.0
+- API version: 9.0.1
 - Package version: 1.0.0
 - Build package: io.swagger.codegen.languages.PythonClientCodegen
 For more information, please visit [http://www.gisaia.com/](http://www.gisaia.com/)
 
 ## Requirements.
 
 Python 2.7 and 3.4+
```

### Comparing `arlas-api-9.0.0/arlas_api.egg-info/SOURCES.txt` & `arlas-api-9.0.1/arlas_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arlas-api-9.0.0/arlas_api_python/__init__.py` & `arlas-api-9.0.1/arlas_api_python/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/arlas_api_python/api_client.py` & `arlas-api-9.0.1/arlas_api_python/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import os
```

### Comparing `arlas-api-9.0.0/arlas_api_python/apis/collections_api.py` & `arlas-api-9.0.1/arlas_api_python/apis/collections_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/arlas_api_python/apis/explore_api.py` & `arlas-api-9.0.1/arlas_api_python/apis/explore_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/arlas_api_python/apis/write_api.py` & `arlas-api-9.0.1/arlas_api_python/apis/write_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/arlas_api_python/configuration.py` & `arlas-api-9.0.1/arlas_api_python/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -215,10 +215,10 @@
         Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 9.0.0\n"\
+               "Version of the API: 9.0.1\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/__init__.py` & `arlas-api-9.0.1/arlas_api_python/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/aggregated_geometry.py` & `arlas-api-9.0.1/arlas_api_python/models/aggregated_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/aggregation.py` & `arlas-api-9.0.1/arlas_api_python/models/aggregation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/aggregation_metric.py` & `arlas-api-9.0.1/arlas_api_python/models/aggregation_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/aggregation_response.py` & `arlas-api-9.0.1/arlas_api_python/models/aggregation_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/aggregations_request.py` & `arlas-api-9.0.1/arlas_api_python/models/aggregations_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/bbox.py` & `arlas-api-9.0.1/arlas_api_python/models/bbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/collection_reference.py` & `arlas-api-9.0.1/arlas_api_python/models/collection_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/collection_reference_description.py` & `arlas-api-9.0.1/arlas_api_python/models/collection_reference_description.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/collection_reference_description_property.py` & `arlas-api-9.0.1/arlas_api_python/models/collection_reference_description_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/collection_reference_parameters.py` & `arlas-api-9.0.1/arlas_api_python/models/collection_reference_parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/count.py` & `arlas-api-9.0.1/arlas_api_python/models/count.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/crs.py` & `arlas-api-9.0.1/arlas_api_python/models/crs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/dublin_core_element_name.py` & `arlas-api-9.0.1/arlas_api_python/models/dublin_core_element_name.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/error.py` & `arlas-api-9.0.1/arlas_api_python/models/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/expression.py` & `arlas-api-9.0.1/arlas_api_python/models/expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/failure.py` & `arlas-api-9.0.1/arlas_api_python/models/failure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/feature.py` & `arlas-api-9.0.1/arlas_api_python/models/feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/feature_collection.py` & `arlas-api-9.0.1/arlas_api_python/models/feature_collection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/feed.py` & `arlas-api-9.0.1/arlas_api_python/models/feed.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/filter.py` & `arlas-api-9.0.1/arlas_api_python/models/filter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/form.py` & `arlas-api-9.0.1/arlas_api_python/models/form.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/generator.py` & `arlas-api-9.0.1/arlas_api_python/models/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/geo_json_object.py` & `arlas-api-9.0.1/arlas_api_python/models/geo_json_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/geometry_collection.py` & `arlas-api-9.0.1/arlas_api_python/models/geometry_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/hit.py` & `arlas-api-9.0.1/arlas_api_python/models/hit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/hits.py` & `arlas-api-9.0.1/arlas_api_python/models/hits.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/inspire.py` & `arlas-api-9.0.1/arlas_api_python/models/inspire.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/inspire_limitation_access.py` & `arlas-api-9.0.1/arlas_api_python/models/inspire_limitation_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/inspire_spatial_resolution.py` & `arlas-api-9.0.1/arlas_api_python/models/inspire_spatial_resolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/inspire_uri.py` & `arlas-api-9.0.1/arlas_api_python/models/inspire_uri.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/interval.py` & `arlas-api-9.0.1/arlas_api_python/models/interval.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/keyword.py` & `arlas-api-9.0.1/arlas_api_python/models/keyword.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/line_string.py` & `arlas-api-9.0.1/arlas_api_python/models/line_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/lng_lat_alt.py` & `arlas-api-9.0.1/arlas_api_python/models/lng_lat_alt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/md.py` & `arlas-api-9.0.1/arlas_api_python/models/md.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/metric.py` & `arlas-api-9.0.1/arlas_api_python/models/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/multi_line_string.py` & `arlas-api-9.0.1/arlas_api_python/models/multi_line_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/multi_point.py` & `arlas-api-9.0.1/arlas_api_python/models/multi_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/multi_polygon.py` & `arlas-api-9.0.1/arlas_api_python/models/multi_polygon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/number.py` & `arlas-api-9.0.1/arlas_api_python/models/number.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/open_search.py` & `arlas-api-9.0.1/arlas_api_python/models/open_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/person.py` & `arlas-api-9.0.1/arlas_api_python/models/person.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/point.py` & `arlas-api-9.0.1/arlas_api_python/models/point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/polygon.py` & `arlas-api-9.0.1/arlas_api_python/models/polygon.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/projection.py` & `arlas-api-9.0.1/arlas_api_python/models/projection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/range_request.py` & `arlas-api-9.0.1/arlas_api_python/models/range_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/range_response.py` & `arlas-api-9.0.1/arlas_api_python/models/range_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/raster_tile_url.py` & `arlas-api-9.0.1/arlas_api_python/models/raster_tile_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/search.py` & `arlas-api-9.0.1/arlas_api_python/models/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/size.py` & `arlas-api-9.0.1/arlas_api_python/models/size.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/sort.py` & `arlas-api-9.0.1/arlas_api_python/models/sort.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/success.py` & `arlas-api-9.0.1/arlas_api_python/models/success.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/tag.py` & `arlas-api-9.0.1/arlas_api_python/models/tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/tag_request.py` & `arlas-api-9.0.1/arlas_api_python/models/tag_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/models/update_response.py` & `arlas-api-9.0.1/arlas_api_python/models/update_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from pprint import pformat
 from six import iteritems
```

### Comparing `arlas-api-9.0.0/arlas_api_python/rest.py` & `arlas-api-9.0.1/arlas_api_python/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/setup.py` & `arlas-api-9.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 """
 
 
 import sys
 from setuptools import setup, find_packages
 
 NAME = "arlas-api"
-VERSION = "9.0.0"
+VERSION = "9.0.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `arlas-api-9.0.0/test/test_aggregated_geometry.py` & `arlas-api-9.0.1/test/test_aggregated_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_aggregation.py` & `arlas-api-9.0.1/test/test_aggregations_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import os
 import sys
 import unittest
 
 import arlas_api_python
 from arlas_api_python.rest import ApiException
-from arlas_api_python.models.aggregation import Aggregation
+from arlas_api_python.models.aggregations_request import AggregationsRequest
 
 
-class TestAggregation(unittest.TestCase):
-    """ Aggregation unit test stubs """
+class TestAggregationsRequest(unittest.TestCase):
+    """ AggregationsRequest unit test stubs """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAggregation(self):
+    def testAggregationsRequest(self):
         """
-        Test Aggregation
+        Test AggregationsRequest
         """
         # FIXME: construct object with mandatory attributes with example values
-        #model = arlas_api_python.models.aggregation.Aggregation()
+        #model = arlas_api_python.models.aggregations_request.AggregationsRequest()
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arlas-api-9.0.0/test/test_aggregation_metric.py` & `arlas-api-9.0.1/test/test_aggregation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import os
 import sys
 import unittest
 
 import arlas_api_python
 from arlas_api_python.rest import ApiException
-from arlas_api_python.models.aggregation_metric import AggregationMetric
+from arlas_api_python.models.aggregation import Aggregation
 
 
-class TestAggregationMetric(unittest.TestCase):
-    """ AggregationMetric unit test stubs """
+class TestAggregation(unittest.TestCase):
+    """ Aggregation unit test stubs """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAggregationMetric(self):
+    def testAggregation(self):
         """
-        Test AggregationMetric
+        Test Aggregation
         """
         # FIXME: construct object with mandatory attributes with example values
-        #model = arlas_api_python.models.aggregation_metric.AggregationMetric()
+        #model = arlas_api_python.models.aggregation.Aggregation()
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arlas-api-9.0.0/test/test_aggregation_response.py` & `arlas-api-9.0.1/test/test_aggregation_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_aggregations_request.py` & `arlas-api-9.0.1/test/test_aggregation_metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import os
 import sys
 import unittest
 
 import arlas_api_python
 from arlas_api_python.rest import ApiException
-from arlas_api_python.models.aggregations_request import AggregationsRequest
+from arlas_api_python.models.aggregation_metric import AggregationMetric
 
 
-class TestAggregationsRequest(unittest.TestCase):
-    """ AggregationsRequest unit test stubs """
+class TestAggregationMetric(unittest.TestCase):
+    """ AggregationMetric unit test stubs """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testAggregationsRequest(self):
+    def testAggregationMetric(self):
         """
-        Test AggregationsRequest
+        Test AggregationMetric
         """
         # FIXME: construct object with mandatory attributes with example values
-        #model = arlas_api_python.models.aggregations_request.AggregationsRequest()
+        #model = arlas_api_python.models.aggregation_metric.AggregationMetric()
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arlas-api-9.0.0/test/test_bbox.py` & `arlas-api-9.0.1/test/test_hit.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import os
 import sys
 import unittest
 
 import arlas_api_python
 from arlas_api_python.rest import ApiException
-from arlas_api_python.models.bbox import Bbox
+from arlas_api_python.models.hit import Hit
 
 
-class TestBbox(unittest.TestCase):
-    """ Bbox unit test stubs """
+class TestHit(unittest.TestCase):
+    """ Hit unit test stubs """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBbox(self):
+    def testHit(self):
         """
-        Test Bbox
+        Test Hit
         """
         # FIXME: construct object with mandatory attributes with example values
-        #model = arlas_api_python.models.bbox.Bbox()
+        #model = arlas_api_python.models.hit.Hit()
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arlas-api-9.0.0/test/test_collection_reference.py` & `arlas-api-9.0.1/test/test_collection_reference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_collection_reference_description.py` & `arlas-api-9.0.1/test/test_collection_reference_description.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_collection_reference_description_property.py` & `arlas-api-9.0.1/test/test_collection_reference_description_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_collection_reference_parameters.py` & `arlas-api-9.0.1/test/test_collection_reference_parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_collections_api.py` & `arlas-api-9.0.1/test/test_collections_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_count.py` & `arlas-api-9.0.1/test/test_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_crs.py` & `arlas-api-9.0.1/test/test_hits.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import os
 import sys
 import unittest
 
 import arlas_api_python
 from arlas_api_python.rest import ApiException
-from arlas_api_python.models.crs import Crs
+from arlas_api_python.models.hits import Hits
 
 
-class TestCrs(unittest.TestCase):
-    """ Crs unit test stubs """
+class TestHits(unittest.TestCase):
+    """ Hits unit test stubs """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCrs(self):
+    def testHits(self):
         """
-        Test Crs
+        Test Hits
         """
         # FIXME: construct object with mandatory attributes with example values
-        #model = arlas_api_python.models.crs.Crs()
+        #model = arlas_api_python.models.hits.Hits()
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arlas-api-9.0.0/test/test_dublin_core_element_name.py` & `arlas-api-9.0.1/test/test_dublin_core_element_name.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_error.py` & `arlas-api-9.0.1/test/test_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_explore_api.py` & `arlas-api-9.0.1/test/test_explore_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_expression.py` & `arlas-api-9.0.1/test/test_expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_failure.py` & `arlas-api-9.0.1/test/test_failure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_feature.py` & `arlas-api-9.0.1/test/test_feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_feature_collection.py` & `arlas-api-9.0.1/test/test_feature_collection.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_feed.py` & `arlas-api-9.0.1/test/test_feed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_filter.py` & `arlas-api-9.0.1/test/test_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_form.py` & `arlas-api-9.0.1/test/test_form.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_generator.py` & `arlas-api-9.0.1/test/test_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_geo_json_object.py` & `arlas-api-9.0.1/test/test_geo_json_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_geometry_collection.py` & `arlas-api-9.0.1/test/test_geometry_collection.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_hit.py` & `arlas-api-9.0.1/test/test_sort.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import os
 import sys
 import unittest
 
 import arlas_api_python
 from arlas_api_python.rest import ApiException
-from arlas_api_python.models.hit import Hit
+from arlas_api_python.models.sort import Sort
 
 
-class TestHit(unittest.TestCase):
-    """ Hit unit test stubs """
+class TestSort(unittest.TestCase):
+    """ Sort unit test stubs """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testHit(self):
+    def testSort(self):
         """
-        Test Hit
+        Test Sort
         """
         # FIXME: construct object with mandatory attributes with example values
-        #model = arlas_api_python.models.hit.Hit()
+        #model = arlas_api_python.models.sort.Sort()
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arlas-api-9.0.0/test/test_hits.py` & `arlas-api-9.0.1/test/test_md.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import os
 import sys
 import unittest
 
 import arlas_api_python
 from arlas_api_python.rest import ApiException
-from arlas_api_python.models.hits import Hits
+from arlas_api_python.models.md import MD
 
 
-class TestHits(unittest.TestCase):
-    """ Hits unit test stubs """
+class TestMD(unittest.TestCase):
+    """ MD unit test stubs """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testHits(self):
+    def testMD(self):
         """
-        Test Hits
+        Test MD
         """
         # FIXME: construct object with mandatory attributes with example values
-        #model = arlas_api_python.models.hits.Hits()
+        #model = arlas_api_python.models.md.MD()
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arlas-api-9.0.0/test/test_inspire.py` & `arlas-api-9.0.1/test/test_inspire.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_inspire_limitation_access.py` & `arlas-api-9.0.1/test/test_inspire_limitation_access.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_inspire_spatial_resolution.py` & `arlas-api-9.0.1/test/test_inspire_spatial_resolution.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_inspire_uri.py` & `arlas-api-9.0.1/test/test_inspire_uri.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_interval.py` & `arlas-api-9.0.1/test/test_interval.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_keyword.py` & `arlas-api-9.0.1/test/test_keyword.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_line_string.py` & `arlas-api-9.0.1/test/test_line_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_lng_lat_alt.py` & `arlas-api-9.0.1/test/test_lng_lat_alt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_md.py` & `arlas-api-9.0.1/test/test_tag.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import os
 import sys
 import unittest
 
 import arlas_api_python
 from arlas_api_python.rest import ApiException
-from arlas_api_python.models.md import MD
+from arlas_api_python.models.tag import Tag
 
 
-class TestMD(unittest.TestCase):
-    """ MD unit test stubs """
+class TestTag(unittest.TestCase):
+    """ Tag unit test stubs """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMD(self):
+    def testTag(self):
         """
-        Test MD
+        Test Tag
         """
         # FIXME: construct object with mandatory attributes with example values
-        #model = arlas_api_python.models.md.MD()
+        #model = arlas_api_python.models.tag.Tag()
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arlas-api-9.0.0/test/test_metric.py` & `arlas-api-9.0.1/test/test_metric.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_multi_line_string.py` & `arlas-api-9.0.1/test/test_multi_line_string.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_multi_point.py` & `arlas-api-9.0.1/test/test_multi_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_multi_polygon.py` & `arlas-api-9.0.1/test/test_multi_polygon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_number.py` & `arlas-api-9.0.1/test/test_number.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_open_search.py` & `arlas-api-9.0.1/test/test_open_search.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_person.py` & `arlas-api-9.0.1/test/test_person.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_point.py` & `arlas-api-9.0.1/test/test_point.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_polygon.py` & `arlas-api-9.0.1/test/test_polygon.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_projection.py` & `arlas-api-9.0.1/test/test_projection.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_range_request.py` & `arlas-api-9.0.1/test/test_range_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_range_response.py` & `arlas-api-9.0.1/test/test_range_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_raster_tile_url.py` & `arlas-api-9.0.1/test/test_raster_tile_url.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_search.py` & `arlas-api-9.0.1/test/test_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_size.py` & `arlas-api-9.0.1/test/test_size.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

### Comparing `arlas-api-9.0.0/test/test_sort.py` & `arlas-api-9.0.1/test/test_success.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import os
 import sys
 import unittest
 
 import arlas_api_python
 from arlas_api_python.rest import ApiException
-from arlas_api_python.models.sort import Sort
+from arlas_api_python.models.success import Success
 
 
-class TestSort(unittest.TestCase):
-    """ Sort unit test stubs """
+class TestSuccess(unittest.TestCase):
+    """ Success unit test stubs """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSort(self):
+    def testSuccess(self):
         """
-        Test Sort
+        Test Success
         """
         # FIXME: construct object with mandatory attributes with example values
-        #model = arlas_api_python.models.sort.Sort()
+        #model = arlas_api_python.models.success.Success()
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arlas-api-9.0.0/test/test_success.py` & `arlas-api-9.0.1/test/test_update_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import os
 import sys
 import unittest
 
 import arlas_api_python
 from arlas_api_python.rest import ApiException
-from arlas_api_python.models.success import Success
+from arlas_api_python.models.update_response import UpdateResponse
 
 
-class TestSuccess(unittest.TestCase):
-    """ Success unit test stubs """
+class TestUpdateResponse(unittest.TestCase):
+    """ UpdateResponse unit test stubs """
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSuccess(self):
+    def testUpdateResponse(self):
         """
-        Test Success
+        Test UpdateResponse
         """
         # FIXME: construct object with mandatory attributes with example values
-        #model = arlas_api_python.models.success.Success()
+        #model = arlas_api_python.models.update_response.UpdateResponse()
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arlas-api-9.0.0/test/test_tag.py` & `arlas-api-9.0.1/test/test_write_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
 import os
 import sys
 import unittest
 
 import arlas_api_python
 from arlas_api_python.rest import ApiException
-from arlas_api_python.models.tag import Tag
+from arlas_api_python.apis.write_api import WriteApi
 
 
-class TestTag(unittest.TestCase):
-    """ Tag unit test stubs """
+class TestWriteApi(unittest.TestCase):
+    """ WriteApi unit test stubs """
 
     def setUp(self):
-        pass
+        self.api = arlas_api_python.apis.write_api.WriteApi()
 
     def tearDown(self):
         pass
 
-    def testTag(self):
+    def test_tag_post(self):
+        """
+        Test case for tag_post
+
+        Tag
         """
-        Test Tag
+        pass
+
+    def test_untag_post(self):
+        """
+        Test case for untag_post
+
+        Untag
         """
-        # FIXME: construct object with mandatory attributes with example values
-        #model = arlas_api_python.models.tag.Tag()
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `arlas-api-9.0.0/test/test_tag_request.py` & `arlas-api-9.0.1/test/test_tag_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     ARLAS Exploration API
 
     Explore the content of ARLAS collections
 
-    OpenAPI spec version: 9.0.0
+    OpenAPI spec version: 9.0.1
     Contact: contact@gisaia.com
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
```

