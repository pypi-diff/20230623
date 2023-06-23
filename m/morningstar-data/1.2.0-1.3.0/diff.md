# Comparing `tmp/morningstar_data-1.2.0.tar.gz` & `tmp/morningstar_data-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morningstar_data-1.2.0.tar", max compression
+gzip compressed data, was "morningstar_data-1.3.0.tar", max compression
```

## Comparing `morningstar_data-1.2.0.tar` & `morningstar_data-1.3.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      571 2023-06-22 18:47:41.613303 morningstar_data-1.2.0/LICENSE
--rw-r--r--   0        0        0      214 2023-06-22 17:30:37.704074 morningstar_data-1.2.0/morningstar_data/__init__.py
--rw-r--r--   0        0        0      615 2023-06-22 17:30:37.705075 morningstar_data-1.2.0/morningstar_data/_base.py
--rw-r--r--   0        0        0     3155 2023-05-15 14:48:44.483407 morningstar_data-1.2.0/morningstar_data/_utils.py
--rw-r--r--   0        0        0       85 2023-06-22 17:30:37.706072 morningstar_data-1.2.0/morningstar_data/_version.py
--rw-r--r--   0        0        0       63 2023-03-17 18:42:29.108172 morningstar_data-1.2.0/morningstar_data/datalake/__init__.py
--rw-r--r--   0        0        0       64 2023-03-17 18:42:29.109161 morningstar_data-1.2.0/morningstar_data/datalake/_data_objects/__init__.py
--rw-r--r--   0        0        0      578 2023-03-17 18:42:29.110169 morningstar_data-1.2.0/morningstar_data/datalake/_data_objects/_file.py
--rw-r--r--   0        0        0      791 2023-03-17 18:42:29.111162 morningstar_data-1.2.0/morningstar_data/datalake/_data_objects/_table.py
--rw-r--r--   0        0        0     1030 2023-03-17 18:42:29.131158 morningstar_data-1.2.0/morningstar_data/datalake/_data_objects/csvfile.py
--rw-r--r--   0        0        0     2220 2023-05-15 14:48:44.490241 morningstar_data-1.2.0/morningstar_data/datalake/_data_objects/temptable.py
--rw-r--r--   0        0        0      559 2023-06-22 17:30:20.444782 morningstar_data-1.2.0/morningstar_data/datalake/_error_messages.py
--rw-r--r--   0        0        0      966 2023-05-15 14:48:44.499809 morningstar_data-1.2.0/morningstar_data/datalake/_exceptions.py
--rw-r--r--   0        0        0     5777 2023-06-22 17:30:20.445786 morningstar_data-1.2.0/morningstar_data/datalake/base.py
--rw-r--r--   0        0        0      955 2023-03-24 17:52:36.333929 morningstar_data-1.2.0/morningstar_data/direct/__init__.py
--rw-r--r--   0        0        0     2496 2023-05-15 14:48:44.510808 morningstar_data-1.2.0/morningstar_data/direct/_api.py
--rw-r--r--   0        0        0      182 2023-05-15 14:48:44.515806 morningstar_data-1.2.0/morningstar_data/direct/_backend_apis/__init__.py
--rw-r--r--   0        0        0     1881 2023-06-22 17:30:20.446780 morningstar_data-1.2.0/morningstar_data/direct/_backend_apis/_delivery_backend.py
--rw-r--r--   0        0        0     5291 2023-05-15 14:48:44.526813 morningstar_data-1.2.0/morningstar_data/direct/_backend_apis/_holdings_backend.py
--rw-r--r--   0        0        0     3445 2023-05-15 14:48:44.531804 morningstar_data-1.2.0/morningstar_data/direct/_backend_apis/_signed_url_backend.py
--rw-r--r--   0        0        0     3848 2023-05-15 14:48:44.537806 morningstar_data-1.2.0/morningstar_data/direct/_base_api.py
--rw-r--r--   0        0        0     5378 2023-06-22 19:25:30.774829 morningstar_data-1.2.0/morningstar_data/direct/_config.py
--rw-r--r--   0        0        0     2109 2023-03-17 18:42:29.149897 morningstar_data-1.2.0/morningstar_data/direct/_config_key.py
--rw-r--r--   0        0        0     7607 2023-06-22 17:30:37.706072 morningstar_data-1.2.0/morningstar_data/direct/_core_api.py
--rw-r--r--   0        0        0      200 2023-03-17 18:42:29.152895 morningstar_data-1.2.0/morningstar_data/direct/_data_objects/__init__.py
--rw-r--r--   0        0        0     2366 2023-03-17 18:42:29.154899 morningstar_data-1.2.0/morningstar_data/direct/_data_objects/_custom_data_points_types.py
--rw-r--r--   0        0        0    26357 2023-06-22 17:30:20.447779 morningstar_data-1.2.0/morningstar_data/direct/_data_objects/_data_points_object.py
--rw-r--r--   0        0        0     7701 2023-03-17 18:42:29.157900 morningstar_data-1.2.0/morningstar_data/direct/_data_objects/_investments_object.py
--rw-r--r--   0        0        0     2636 2023-06-22 17:30:20.447779 morningstar_data-1.2.0/morningstar_data/direct/_data_point.py
--rw-r--r--   0        0        0     1078 2023-03-17 18:42:29.161693 morningstar_data-1.2.0/morningstar_data/direct/_data_type.py
--rw-r--r--   0        0        0     1642 2023-06-22 17:30:37.707074 morningstar_data-1.2.0/morningstar_data/direct/_decorator.py
--rw-r--r--   0        0        0    14023 2023-06-22 17:30:20.448778 morningstar_data-1.2.0/morningstar_data/direct/_error_messages.py
--rw-r--r--   0        0        0     3583 2023-06-22 17:30:20.448778 morningstar_data-1.2.0/morningstar_data/direct/_exceptions.py
--rw-r--r--   0        0        0        0 2023-03-17 18:42:29.173293 morningstar_data-1.2.0/morningstar_data/direct/_investment/__init__.py
--rw-r--r--   0        0        0     4378 2023-05-15 14:48:44.577810 morningstar_data-1.2.0/morningstar_data/direct/_investment/_asset_flow_data.py
--rw-r--r--   0        0        0     1581 2023-05-15 14:48:44.586805 morningstar_data-1.2.0/morningstar_data/direct/_investment/_common.py
--rw-r--r--   0        0        0     6233 2023-05-15 14:48:44.592805 morningstar_data-1.2.0/morningstar_data/direct/_investment/_data.py
--rw-r--r--   0        0        0     8550 2023-06-22 17:30:20.450784 morningstar_data-1.2.0/morningstar_data/direct/_investment/_normal_data.py
--rw-r--r--   0        0        0     5154 2023-05-15 14:48:44.604807 morningstar_data-1.2.0/morningstar_data/direct/_investment/_peer_group_data.py
--rw-r--r--   0        0        0      165 2023-03-17 18:42:29.183291 morningstar_data-1.2.0/morningstar_data/direct/_portfolio/__init__.py
--rw-r--r--   0        0        0     1312 2023-05-15 14:48:44.610805 morningstar_data-1.2.0/morningstar_data/direct/_portfolio/_common.py
--rw-r--r--   0        0        0     8021 2023-05-15 14:48:44.615804 morningstar_data-1.2.0/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
--rw-r--r--   0        0        0     8117 2023-05-15 14:48:44.621806 morningstar_data-1.2.0/morningstar_data/direct/_portfolio/_portfolio_settings.py
--rw-r--r--   0        0        0      980 2023-03-17 18:42:29.190337 morningstar_data-1.2.0/morningstar_data/direct/_portfolio/_portfolio_type.py
--rw-r--r--   0        0        0    11166 2023-05-15 14:48:44.627805 morningstar_data-1.2.0/morningstar_data/direct/_portfolio_data_set.py
--rw-r--r--   0        0        0     3470 2023-05-15 14:48:44.633807 morningstar_data-1.2.0/morningstar_data/direct/_utils.py
--rw-r--r--   0        0        0    13355 2023-06-22 17:30:37.708073 morningstar_data-1.2.0/morningstar_data/direct/asset_flow.py
--rw-r--r--   0        0        0    16635 2023-06-22 17:30:37.709081 morningstar_data-1.2.0/morningstar_data/direct/custom_database.py
--rw-r--r--   0        0        0     1300 2023-03-17 18:42:29.200377 morningstar_data-1.2.0/morningstar_data/direct/data_type.py
--rw-r--r--   0        0        0    43354 2023-06-22 17:30:37.710075 morningstar_data-1.2.0/morningstar_data/direct/holdings.py
--rw-r--r--   0        0        0    13827 2023-06-22 17:30:37.711095 morningstar_data-1.2.0/morningstar_data/direct/investment.py
--rw-r--r--   0        0        0    33055 2023-06-22 17:30:37.712053 morningstar_data-1.2.0/morningstar_data/direct/lookup.py
--rw-r--r--   0        0        0     6130 2023-06-22 17:30:37.713064 morningstar_data-1.2.0/morningstar_data/direct/peer_group.py
--rw-r--r--   0        0        0    19911 2023-06-22 17:30:37.714094 morningstar_data-1.2.0/morningstar_data/direct/performance_report.py
--rw-r--r--   0        0        0    38033 2023-06-22 17:30:37.715091 morningstar_data-1.2.0/morningstar_data/direct/portfolio.py
--rw-r--r--   0        0        0    12817 2023-06-22 17:30:37.716074 morningstar_data-1.2.0/morningstar_data/direct/returns.py
--rw-r--r--   0        0        0      418 2023-03-17 18:42:29.214388 morningstar_data-1.2.0/morningstar_data/direct/user_items/__init__.py
--rw-r--r--   0        0        0      762 2023-03-17 18:42:29.218384 morningstar_data-1.2.0/morningstar_data/direct/user_items/_utils.py
--rw-r--r--   0        0        0     8114 2023-06-22 17:30:37.717076 morningstar_data-1.2.0/morningstar_data/direct/user_items/data_set.py
--rw-r--r--   0        0        0    13305 2023-06-22 17:30:37.719075 morningstar_data-1.2.0/morningstar_data/direct/user_items/investment_lists.py
--rw-r--r--   0        0        0    11412 2023-06-19 16:45:12.887904 morningstar_data-1.2.0/morningstar_data/direct/user_items/portfolio.py
--rw-r--r--   0        0        0    10592 2023-06-22 17:30:37.720072 morningstar_data-1.2.0/morningstar_data/direct/user_items/search_criteria.py
--rw-r--r--   0        0        0     4874 2023-06-22 17:30:37.720072 morningstar_data-1.2.0/morningstar_data/lookup.py
--rw-r--r--   0        0        0      160 2023-03-24 17:52:36.359930 morningstar_data-1.2.0/morningstar_data/utils/__init__.py
--rw-r--r--   0        0        0     6516 2023-03-24 17:52:36.360930 morningstar_data-1.2.0/morningstar_data/utils/_delivery_config.py
--rw-r--r--   0        0        0     7973 2023-06-22 19:25:30.775831 morningstar_data-1.2.0/morningstar_data/utils/_helpers.py
--rw-r--r--   0        0        0    10691 2023-06-22 17:30:37.722072 morningstar_data-1.2.0/morningstar_data/utils/delivery.py
--rw-r--r--   0        0        0     2552 2023-06-22 18:47:41.615267 morningstar_data-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    11502 2023-06-22 19:25:30.773829 morningstar_data-1.2.0/README.md
--rw-r--r--   0        0        0    12382 1970-01-01 00:00:00.000000 morningstar_data-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      558 2023-06-22 23:57:19.310138 morningstar_data-1.3.0/LICENSE
+-rw-r--r--   0        0        0    11361 2023-06-22 23:57:19.310422 morningstar_data-1.3.0/README.md
+-rw-r--r--   0        0        0      207 2023-06-22 17:07:28.074097 morningstar_data-1.3.0/morningstar_data/__init__.py
+-rw-r--r--   0        0        0      599 2023-06-22 17:07:28.074722 morningstar_data-1.3.0/morningstar_data/_base.py
+-rw-r--r--   0        0        0     3056 2023-06-14 19:10:47.534369 morningstar_data-1.3.0/morningstar_data/_utils.py
+-rw-r--r--   0        0        0       82 2023-06-22 17:07:28.075331 morningstar_data-1.3.0/morningstar_data/_version.py
+-rw-r--r--   0        0        0       61 2023-03-23 20:56:12.199461 morningstar_data-1.3.0/morningstar_data/datalake/__init__.py
+-rw-r--r--   0        0        0       62 2023-03-23 20:56:12.199647 morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/__init__.py
+-rw-r--r--   0        0        0      556 2023-03-23 20:56:12.199811 morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/_file.py
+-rw-r--r--   0        0        0      762 2023-03-23 20:56:12.200012 morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/_table.py
+-rw-r--r--   0        0        0      996 2023-03-23 20:56:12.200274 morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/csvfile.py
+-rw-r--r--   0        0        0     2163 2023-06-14 19:10:47.534854 morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/temptable.py
+-rw-r--r--   0        0        0      552 2023-06-22 17:07:28.075659 morningstar_data-1.3.0/morningstar_data/datalake/_error_messages.py
+-rw-r--r--   0        0        0      936 2023-06-14 19:10:47.535372 morningstar_data-1.3.0/morningstar_data/datalake/_exceptions.py
+-rw-r--r--   0        0        0     5620 2023-06-22 17:07:28.076042 morningstar_data-1.3.0/morningstar_data/datalake/base.py
+-rw-r--r--   0        0        0      939 2023-06-14 19:10:47.536605 morningstar_data-1.3.0/morningstar_data/direct/__init__.py
+-rw-r--r--   0        0        0     2433 2023-06-14 19:10:47.537161 morningstar_data-1.3.0/morningstar_data/direct/_api.py
+-rw-r--r--   0        0        0      179 2023-06-14 19:10:47.537414 morningstar_data-1.3.0/morningstar_data/direct/_backend_apis/__init__.py
+-rw-r--r--   0        0        0     1831 2023-06-22 17:07:28.076775 morningstar_data-1.3.0/morningstar_data/direct/_backend_apis/_delivery_backend.py
+-rw-r--r--   0        0        0     5148 2023-06-14 19:10:47.537772 morningstar_data-1.3.0/morningstar_data/direct/_backend_apis/_holdings_backend.py
+-rw-r--r--   0        0        0     3355 2023-06-14 19:10:47.537906 morningstar_data-1.3.0/morningstar_data/direct/_backend_apis/_signed_url_backend.py
+-rw-r--r--   0        0        0     3751 2023-06-14 19:10:47.538259 morningstar_data-1.3.0/morningstar_data/direct/_base_api.py
+-rw-r--r--   0        0        0     5241 2023-06-22 23:57:19.312478 morningstar_data-1.3.0/morningstar_data/direct/_config.py
+-rw-r--r--   0        0        0     1999 2022-07-19 18:10:19.834957 morningstar_data-1.3.0/morningstar_data/direct/_config_key.py
+-rw-r--r--   0        0        0     7434 2023-06-22 17:07:28.077965 morningstar_data-1.3.0/morningstar_data/direct/_core_api.py
+-rw-r--r--   0        0        0      197 2022-07-19 18:10:19.835284 morningstar_data-1.3.0/morningstar_data/direct/_data_objects/__init__.py
+-rw-r--r--   0        0        0     2298 2022-07-19 18:10:19.835489 morningstar_data-1.3.0/morningstar_data/direct/_data_objects/_custom_data_points_types.py
+-rw-r--r--   0        0        0    26357 2023-06-22 17:07:28.078754 morningstar_data-1.3.0/morningstar_data/direct/_data_objects/_data_points_object.py
+-rw-r--r--   0        0        0     7532 2023-03-23 20:56:12.207196 morningstar_data-1.3.0/morningstar_data/direct/_data_objects/_investments_object.py
+-rw-r--r--   0        0        0     2572 2023-06-22 17:07:28.079551 morningstar_data-1.3.0/morningstar_data/direct/_data_point.py
+-rw-r--r--   0        0        0     1051 2022-07-19 18:10:19.836661 morningstar_data-1.3.0/morningstar_data/direct/_data_type.py
+-rw-r--r--   0        0        0     1593 2023-06-22 17:07:28.080200 morningstar_data-1.3.0/morningstar_data/direct/_decorator.py
+-rw-r--r--   0        0        0    13892 2023-06-22 17:07:28.080827 morningstar_data-1.3.0/morningstar_data/direct/_error_messages.py
+-rw-r--r--   0        0        0     3463 2023-06-22 17:07:28.081496 morningstar_data-1.3.0/morningstar_data/direct/_exceptions.py
+-rw-r--r--   0        0        0        0 2022-07-19 18:10:19.837832 morningstar_data-1.3.0/morningstar_data/direct/_investment/__init__.py
+-rw-r--r--   0        0        0     4288 2023-06-14 19:10:47.544214 morningstar_data-1.3.0/morningstar_data/direct/_investment/_asset_flow_data.py
+-rw-r--r--   0        0        0     1546 2023-06-14 19:10:47.544648 morningstar_data-1.3.0/morningstar_data/direct/_investment/_common.py
+-rw-r--r--   0        0        0     6085 2023-06-14 19:10:47.545176 morningstar_data-1.3.0/morningstar_data/direct/_investment/_data.py
+-rw-r--r--   0        0        0     8369 2023-06-22 17:07:28.082117 morningstar_data-1.3.0/morningstar_data/direct/_investment/_normal_data.py
+-rw-r--r--   0        0        0     5023 2023-06-14 19:10:47.546410 morningstar_data-1.3.0/morningstar_data/direct/_investment/_peer_group_data.py
+-rw-r--r--   0        0        0      162 2023-03-23 20:56:12.208683 morningstar_data-1.3.0/morningstar_data/direct/_portfolio/__init__.py
+-rw-r--r--   0        0        0     1272 2023-06-14 19:10:47.546903 morningstar_data-1.3.0/morningstar_data/direct/_portfolio/_common.py
+-rw-r--r--   0        0        0     7859 2023-06-20 16:42:44.590672 morningstar_data-1.3.0/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
+-rw-r--r--   0        0        0     7913 2023-06-20 16:42:44.590988 morningstar_data-1.3.0/morningstar_data/direct/_portfolio/_portfolio_settings.py
+-rw-r--r--   0        0        0      955 2023-03-23 20:56:12.210194 morningstar_data-1.3.0/morningstar_data/direct/_portfolio/_portfolio_type.py
+-rw-r--r--   0        0        0    10975 2023-06-14 19:10:47.548557 morningstar_data-1.3.0/morningstar_data/direct/_portfolio_data_set.py
+-rw-r--r--   0        0        0     3357 2023-06-14 19:10:47.548933 morningstar_data-1.3.0/morningstar_data/direct/_utils.py
+-rw-r--r--   0        0        0    13061 2023-06-22 17:07:28.082813 morningstar_data-1.3.0/morningstar_data/direct/asset_flow.py
+-rw-r--r--   0        0        0    16274 2023-06-22 17:07:28.083438 morningstar_data-1.3.0/morningstar_data/direct/custom_database.py
+-rw-r--r--   0        0        0     1236 2022-07-19 18:10:19.841830 morningstar_data-1.3.0/morningstar_data/direct/data_type.py
+-rw-r--r--   0        0        0    42528 2023-06-22 17:07:28.084133 morningstar_data-1.3.0/morningstar_data/direct/holdings.py
+-rw-r--r--   0        0        0    13577 2023-06-22 17:07:28.084678 morningstar_data-1.3.0/morningstar_data/direct/investment.py
+-rw-r--r--   0        0        0    32223 2023-06-22 17:07:28.085565 morningstar_data-1.3.0/morningstar_data/direct/lookup.py
+-rw-r--r--   0        0        0     6040 2023-06-22 17:07:28.086336 morningstar_data-1.3.0/morningstar_data/direct/peer_group.py
+-rw-r--r--   0        0        0    19389 2023-06-22 17:07:28.087121 morningstar_data-1.3.0/morningstar_data/direct/performance_report.py
+-rw-r--r--   0        0        0    37181 2023-06-22 17:07:28.087827 morningstar_data-1.3.0/morningstar_data/direct/portfolio.py
+-rw-r--r--   0        0        0    12562 2023-06-22 17:07:28.088426 morningstar_data-1.3.0/morningstar_data/direct/returns.py
+-rw-r--r--   0        0        0      413 2023-03-23 20:56:12.218181 morningstar_data-1.3.0/morningstar_data/direct/user_items/__init__.py
+-rw-r--r--   0        0        0      742 2022-07-19 18:10:19.845539 morningstar_data-1.3.0/morningstar_data/direct/user_items/_utils.py
+-rw-r--r--   0        0        0     7888 2023-06-22 17:07:28.088937 morningstar_data-1.3.0/morningstar_data/direct/user_items/data_set.py
+-rw-r--r--   0        0        0    12981 2023-06-22 17:07:28.089417 morningstar_data-1.3.0/morningstar_data/direct/user_items/investment_lists.py
+-rw-r--r--   0        0        0    11145 2023-06-20 16:42:44.598186 morningstar_data-1.3.0/morningstar_data/direct/user_items/portfolio.py
+-rw-r--r--   0        0        0    10308 2023-06-22 17:07:28.089811 morningstar_data-1.3.0/morningstar_data/direct/user_items/search_criteria.py
+-rw-r--r--   0        0        0     4752 2023-06-22 17:07:28.090463 morningstar_data-1.3.0/morningstar_data/lookup.py
+-rw-r--r--   0        0        0      157 2023-06-14 19:10:47.555441 morningstar_data-1.3.0/morningstar_data/utils/__init__.py
+-rw-r--r--   0        0        0     6359 2023-06-14 19:10:47.555845 morningstar_data-1.3.0/morningstar_data/utils/_delivery_config.py
+-rw-r--r--   0        0        0     7752 2023-06-22 23:57:19.313230 morningstar_data-1.3.0/morningstar_data/utils/_helpers.py
+-rw-r--r--   0        0        0    10435 2023-06-22 17:07:28.091516 morningstar_data-1.3.0/morningstar_data/utils/delivery.py
+-rw-r--r--   0        0        0     2452 2023-06-23 00:21:47.576159 morningstar_data-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0    12382 1970-01-01 00:00:00.000000 morningstar_data-1.3.0/PKG-INFO
```

### Comparing `morningstar_data-1.2.0/LICENSE` & `morningstar_data-1.3.0/LICENSE`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Copyright 2023 Morningstar, Inc.
-
-Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License.
-You may obtain a copy of the License at
-
-    http://www.apache.org/licenses/LICENSE-2.0
-
-Unless required by applicable law or agreed to in writing, software
-distributed under the License is distributed on an "AS IS" BASIS,
-WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-See the License for the specific language governing permissions and
-limitations under the License.
+Copyright 2023 Morningstar, Inc.
+
+Licensed under the Apache License, Version 2.0 (the "License");
+you may not use this file except in compliance with the License.
+You may obtain a copy of the License at
+
+    http://www.apache.org/licenses/LICENSE-2.0
+
+Unless required by applicable law or agreed to in writing, software
+distributed under the License is distributed on an "AS IS" BASIS,
+WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+See the License for the specific language governing permissions and
+limitations under the License.
```

### Comparing `morningstar_data-1.2.0/morningstar_data/datalake/_data_objects/_table.py` & `morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/_table.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from pandas import DataFrame
-from abc import ABC, abstractmethod
-
-
-class Table(ABC):
-    def __init__(self, name: str, df: DataFrame) -> None:
-        self.name = name
-        self.df = self._validate_column_names(df)
-
-    @abstractmethod
-    def _validate_column_names(self, df: DataFrame) -> None:
-        """
-        Validate that column names in Data Frame do not contain reserved words and conform to Redshift's requirements:
-        https://docs.aws.amazon.com/redshift/latest/dg/r_names.html
-
-        Args:
-            DataFrame
-        Returns:
-            The validated DataFrame
-        """
-        pass
-
-    @abstractmethod
-    def get_create_query(self) -> None:
-        pass
-
-    @abstractmethod
-    def get_insert_query(self) -> None:
-        pass
+from pandas import DataFrame
+from abc import ABC, abstractmethod
+
+
+class Table(ABC):
+    def __init__(self, name: str, df: DataFrame) -> None:
+        self.name = name
+        self.df = self._validate_column_names(df)
+
+    @abstractmethod
+    def _validate_column_names(self, df: DataFrame) -> None:
+        """
+        Validate that column names in Data Frame do not contain reserved words and conform to Redshift's requirements:
+        https://docs.aws.amazon.com/redshift/latest/dg/r_names.html
+
+        Args:
+            DataFrame
+        Returns:
+            The validated DataFrame
+        """
+        pass
+
+    @abstractmethod
+    def get_create_query(self) -> None:
+        pass
+
+    @abstractmethod
+    def get_insert_query(self) -> None:
+        pass
```

### Comparing `morningstar_data-1.2.0/morningstar_data/datalake/_data_objects/csvfile.py` & `morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/csvfile.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from datetime import datetime
-import uuid
-from ._file import File
-
-from pandas import DataFrame
-from io import StringIO
-
-from typing import Any, Optional
-import boto3
-from botocore.exceptions import ClientError
-
-
-class CSVFile(File):
-    def __init__(self, df: DataFrame) -> None:
-        self.csv_buffer = StringIO()
-        super().__init__(df)
-        self.df.to_csv(self.csv_buffer, index=False, header=False)
-
-    def upload_to_s3(self, bucket: Optional[str]) -> Any:
-        s3_resource = boto3.resource("s3")
-        path = self.create_s3_file_path()
-        try:
-            s3_resource.Object(bucket, path).put(Body=self.csv_buffer.getvalue())
-        except ClientError as e:
-            raise e
-        return path
-
-    def create_s3_file_path(self) -> Any:
-        basename = "temp_csv"
-        obj = uuid.uuid4()
-        suffix = datetime.now().strftime("%y%m%d_%H%M%S") + ".csv"
-        filename = "_".join([basename, suffix])
-        path = f"{obj}/{filename}"
-        return path
+from datetime import datetime
+import uuid
+from ._file import File
+
+from pandas import DataFrame
+from io import StringIO
+
+from typing import Any, Optional
+import boto3
+from botocore.exceptions import ClientError
+
+
+class CSVFile(File):
+    def __init__(self, df: DataFrame) -> None:
+        self.csv_buffer = StringIO()
+        super().__init__(df)
+        self.df.to_csv(self.csv_buffer, index=False, header=False)
+
+    def upload_to_s3(self, bucket: Optional[str]) -> Any:
+        s3_resource = boto3.resource("s3")
+        path = self.create_s3_file_path()
+        try:
+            s3_resource.Object(bucket, path).put(Body=self.csv_buffer.getvalue())
+        except ClientError as e:
+            raise e
+        return path
+
+    def create_s3_file_path(self) -> Any:
+        basename = "temp_csv"
+        obj = uuid.uuid4()
+        suffix = datetime.now().strftime("%y%m%d_%H%M%S") + ".csv"
+        filename = "_".join([basename, suffix])
+        path = f"{obj}/{filename}"
+        return path
```

### Comparing `morningstar_data-1.2.0/morningstar_data/datalake/_data_objects/temptable.py` & `morningstar_data-1.3.0/morningstar_data/datalake/_data_objects/temptable.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import re
-from ._table import Table
-
-from pandas import DataFrame
-from typing import Any, Optional
-
-
-class TempTable(Table):
-    def __init__(self, name: str, df: DataFrame, table_stage_id: Optional[str] = None) -> None:
-        super().__init__(name, df)
-        self.table_stage_id = table_stage_id
-
-    def _validate_column_names(self, df: DataFrame) -> DataFrame:
-        columns = df.columns
-
-        for col in columns:
-            if len(col) > 127:
-                raise ValueError(f"Invalid column name {col}: Column names must be less than 128 characters in length.")
-            if not (col[0] == "_" or col[0].isalpha()):
-                raise ValueError(f"Invalid column name {col}: Column names can only start with a letter or underscore.")
-            if not re.search("^[\w|\$]*$", col):
-                raise ValueError(f"Invalid column name {col}: Column names can only contain alphanumeric characters, underscores (_) or dollar signs ($).")
-
-            return df
-
-    def get_create_query(self) -> Any:
-        query_string = f'CREATE TEMP TABLE "{self.name}" ('
-        for col_type, col_name in zip(self.df.dtypes, self.df):  # type: ignore
-            converted_type = self._pd_dtype_to_redshift_dtype(col_type.name)
-            query_string += f'\n"{col_name}" {converted_type},'
-
-        query_string = query_string[:-1] + "\n)"
-
-        return query_string
-
-    def get_insert_query(self, bucket_path: str, bucket_name: Optional[str], iam_role: Optional[str]) -> str:  # type: ignore
-        query = f"""
-                COPY {self.name}
-                FROM 's3://{bucket_name}/{bucket_path}'
-                IAM_ROLE '{iam_role}'
-                CSV;
-                """
-        return query
-
-    def _pd_dtype_to_redshift_dtype(self, dtype: Any) -> str:
-        if dtype.startswith("int64"):
-            return "BIGINT"
-        elif dtype.startswith("int"):
-            return "INTEGER"
-        elif dtype.startswith("float"):
-            return "REAL"
-        elif dtype.startswith("datetime"):
-            return "TIMESTAMP"
-        elif dtype == "bool":
-            return "BOOLEAN"
-        else:
-            return "VARCHAR(256)"
+import re
+from ._table import Table
+
+from pandas import DataFrame
+from typing import Any, Optional
+
+
+class TempTable(Table):
+    def __init__(self, name: str, df: DataFrame, table_stage_id: Optional[str] = None) -> None:
+        super().__init__(name, df)
+        self.table_stage_id = table_stage_id
+
+    def _validate_column_names(self, df: DataFrame) -> DataFrame:
+        columns = df.columns
+
+        for col in columns:
+            if len(col) > 127:
+                raise ValueError(f"Invalid column name {col}: Column names must be less than 128 characters in length.")
+            if not (col[0] == "_" or col[0].isalpha()):
+                raise ValueError(f"Invalid column name {col}: Column names can only start with a letter or underscore.")
+            if not re.search("^[\w|\$]*$", col):
+                raise ValueError(f"Invalid column name {col}: Column names can only contain alphanumeric characters, underscores (_) or dollar signs ($).")
+
+            return df
+
+    def get_create_query(self) -> Any:
+        query_string = f'CREATE TEMP TABLE "{self.name}" ('
+        for col_type, col_name in zip(self.df.dtypes, self.df):  # type: ignore
+            converted_type = self._pd_dtype_to_redshift_dtype(col_type.name)
+            query_string += f'\n"{col_name}" {converted_type},'
+
+        query_string = query_string[:-1] + "\n)"
+
+        return query_string
+
+    def get_insert_query(self, bucket_path: str, bucket_name: Optional[str], iam_role: Optional[str]) -> str:  # type: ignore
+        query = f"""
+                COPY {self.name}
+                FROM 's3://{bucket_name}/{bucket_path}'
+                IAM_ROLE '{iam_role}'
+                CSV;
+                """
+        return query
+
+    def _pd_dtype_to_redshift_dtype(self, dtype: Any) -> str:
+        if dtype.startswith("int64"):
+            return "BIGINT"
+        elif dtype.startswith("int"):
+            return "INTEGER"
+        elif dtype.startswith("float"):
+            return "REAL"
+        elif dtype.startswith("datetime"):
+            return "TIMESTAMP"
+        elif dtype == "bool":
+            return "BOOLEAN"
+        else:
+            return "VARCHAR(256)"
```

### Comparing `morningstar_data-1.2.0/morningstar_data/datalake/_error_messages.py` & `morningstar_data-1.3.0/morningstar_data/datalake/_error_messages.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-# Add custom error messages related to DataLake
-UNAUTHORIZED_DATALAKE_REQUEST_ERROR = (
-    "A valid license is required to query Morningstar datalake. Please fill out this form for further assistance: https://go.morningstar.com/LP=6808"
-)
-UNAVAILABLE_EXTERNALLY = "Morningstar datalake is only accessible through Analytics Lab"
-DATA_NOT_FOUND = "The requested data could not be found. Check the query parameters and try again."
-TEMP_TABLE_NAME_NOT_FOUND = "One or more temporary tables does not have a name. Check the query parameters and try again."
+# Add custom error messages related to DataLake
+UNAUTHORIZED_DATALAKE_REQUEST_ERROR = (
+    "A valid license is required to query Morningstar datalake. Please fill out this form for further assistance: https://go.morningstar.com/LP=6808"
+)
+UNAVAILABLE_EXTERNALLY = "Morningstar datalake is only accessible through Analytics Lab"
+DATA_NOT_FOUND = "The requested data could not be found. Check the query parameters and try again."
+TEMP_TABLE_NAME_NOT_FOUND = "One or more temporary tables does not have a name. Check the query parameters and try again."
```

### Comparing `morningstar_data-1.2.0/morningstar_data/datalake/_exceptions.py` & `morningstar_data-1.3.0/morningstar_data/datalake/_exceptions.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from typing import Optional
-from . import _error_messages
-
-
-class UnauthorizedDataLakeAccessError(Exception):
-    def __init__(self, message: Optional[str] = None) -> None:
-        if not message:
-            super().__init__(_error_messages.UNAUTHORIZED_DATALAKE_REQUEST_ERROR)
-        else:
-            super().__init__(message)
-
-
-class InvalidQueryException(Exception):
-    def __init__(self, message: str) -> None:
-        super().__init__(message)
-
-
-class UnavailableExternally(Exception):
-    def __init__(self) -> None:
-        super().__init__(_error_messages.UNAVAILABLE_EXTERNALLY)
-
-
-class DataNotFoundException(Exception):
-    def __init__(self, message: Optional[str] = None) -> None:
-        super().__init__(_error_messages.DATA_NOT_FOUND)
-
-
-class TempTableNameNotFoundException(Exception):
-    def __init__(self, message: Optional[str] = None) -> None:
-        super().__init__(_error_messages.TEMP_TABLE_NAME_NOT_FOUND)
+from typing import Optional
+from . import _error_messages
+
+
+class UnauthorizedDataLakeAccessError(Exception):
+    def __init__(self, message: Optional[str] = None) -> None:
+        if not message:
+            super().__init__(_error_messages.UNAUTHORIZED_DATALAKE_REQUEST_ERROR)
+        else:
+            super().__init__(message)
+
+
+class InvalidQueryException(Exception):
+    def __init__(self, message: str) -> None:
+        super().__init__(message)
+
+
+class UnavailableExternally(Exception):
+    def __init__(self) -> None:
+        super().__init__(_error_messages.UNAVAILABLE_EXTERNALLY)
+
+
+class DataNotFoundException(Exception):
+    def __init__(self, message: Optional[str] = None) -> None:
+        super().__init__(_error_messages.DATA_NOT_FOUND)
+
+
+class TempTableNameNotFoundException(Exception):
+    def __init__(self, message: Optional[str] = None) -> None:
+        super().__init__(_error_messages.TEMP_TABLE_NAME_NOT_FOUND)
```

### Comparing `morningstar_data-1.2.0/morningstar_data/datalake/base.py` & `morningstar_data-1.3.0/morningstar_data/datalake/base.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-import logging
-import os
-from typing import Optional, List
-from pandas import DataFrame
-import json
-from ..direct._config import _Config
-from ..direct._backend_apis._signed_url_backend import SignedUrlBackend
-import io
-
-import pandas as pd
-from enum import Enum
-from ._data_objects import TempTable, CSVFile
-from ._exceptions import TempTableNameNotFoundException
-
-_logger = logging.getLogger(__name__)
-
-DL_ACCOUNT = os.getenv("DL_ACCOUNT")
-
-region = os.getenv("DL_AWS_REGION", "us-east-1")
-is_external_user = os.getenv("IS_EXTERNAL_USER")
-uim_user_id = os.getenv("UIM_USER_ID")
-bucket_name = os.getenv("DL_TEMP_TABLE_BUCKET_NAME")
-redshift_cluster_id = os.getenv("REDSHIFT_CLUSTER_ID")
-redshift_database_name = os.getenv("REDSHIFT_DATABASE_NAME")
-
-
-class Source(Enum):
-    DATALAKE = 1
-    LAKEHOUSE = 2
-
-
-def query(query_str: str, temp_tables: Optional[List[TempTable]] = None) -> DataFrame:
-    """
-    :bdg-ref-danger:`Upcoming Feature <../upcoming_feature>`
-
-    Retrieve the results of a SQL query from the Morningstar Data Lake.
-
-    Args:
-        query_str: SQL query to be executed in Morningstar Data Lake
-        temp_tables: A list of temporary tables that will exist for the duration of the query.
-
-    Returns:
-        A DataFrame object with results of the SQL query.
-
-    :Examples:
-
-        Submit a query using a temp table
-
-    ::
-
-        import morningstar_data as md
-        import pandas as pd
-
-
-        df_my_table = pd.DataFrame({'sec_id': ['F0GBR0606A', 'F00000SYAH', 'F00000WP51'], 'closing_price': [128.372, 23.02, 528.33]})
-        df_query = md.datalake.query(query_str = 'select * from my_table;', temp_tables = [md.datalake.TempTable('my_table', df_my_table)])
-
-    :Output:
-
-        ===========  ===============
-         sec_id       closing_price
-        ===========  ===============
-        F0GBR0606A      128.372
-        F00000SYAH       23.02
-        F00000WP51      528.33
-        ===========  ===============
-
-    :Errors:
-        InvalidQueryException: When `query_str` contains invalid SQL syntax.
-
-        UnauthorizedDataLakeAccessError: When the calling user is not authorized to query the Morningstar Data Lake.
-
-        TempTableNameNotFoundException: When one or more temp tables being used are not found in the query string.
-
-    """
-    signed_url_backend = SignedUrlBackend()
-    config = _Config()
-
-    if temp_tables:
-        _logger.debug(f"Query function invoked with temp tables {temp_tables}")
-
-        missing_tables = []
-        for table in temp_tables:
-            if table.name is None or table.name.strip() == "":
-                _logger.debug("Temp table name is empty")
-                raise TempTableNameNotFoundException from None
-
-            if table.name not in query_str:
-                missing_tables.append(table.name)
-
-            body = {"is_temp": True, "table_name": table.name}
-
-            # get a signed url to upload this table to
-            _logger.debug(f"Uploading to stage table_name: {table.name}")
-            resp = json.loads(signed_url_backend.do_post_request(url=config.temp_table_url(), data=body))
-
-            table.table_stage_id = resp["table_id"]
-            upload_url = resp["upload_url"]
-
-            resp = signed_url_backend.put_csv_file(csv=CSVFile(table.df), signed_upload_url=upload_url)
-
-            _logger.info(f"Upload complete under the following s3 id {table.table_stage_id} with url {upload_url}")
-
-        if len(missing_tables) > 0:
-            _logger.warn(f" Not all temp_tables are in query_str, make sure your query is correct. Missing table names: {missing_tables}")
-
-    df = _get_query_as_df(signed_url_backend, config, query_str, temp_tables)
-
-    return df
-
-
-def _construct_query_endpoint_payload(query_str: str, temp_tables: Optional[List[TempTable]] = None) -> str:
-    # Sample body from md package to POST /query endpoint
-
-    # {
-    #     "query": "select * from xyz join temp_a join temp_b;",
-    #     "tables": [
-    #         {"table_id": "sd98f-dsf89sdf-sdf-df", "table_name": "temp_a", "columns": [{"name": "col1", "type": "int64"}, {"name": "col2", "type": "float"}]},
-    #         {"table_id": "ad98f-dsf89sdf-sdf-df", "table_name": "temp_b",
-    # "columns": [{"name": "col1", "type": "int64"}, {"name": "col2", "type": "float"}]},
-    #     ],
-    # }
-
-    # Within a Temp table the DF argument is not optional
-    if temp_tables:
-        payload = {
-            "query": query_str,
-            "tables": [
-                {"table_id": table.table_stage_id, "table_name": table.name, "columns": [{"name": col, "type": str(table.df[col].dtype)} for col in table.df.columns]}  # type: ignore
-                for table in temp_tables
-            ],
-        }
-    else:
-        payload = {"query": query_str}
-
-    return json.dumps(payload)
-
-
-def _get_query_as_df(signed_url_backend: SignedUrlBackend, config: _Config, query_str: str, temp_tables: Optional[List[TempTable]]) -> pd.DataFrame:
-
-    payload = _construct_query_endpoint_payload(query_str, temp_tables)
-
-    _logger.debug(f"Hitting the data lake query endpoint with this payload\n{payload}\n")
-
-    download_url_response = signed_url_backend.do_post_request(url=config.query_api_url(), data=payload)
-    download_url = json.loads(download_url_response)["url"]
-
-    _logger.info(f"Downloading from s3 at the url {download_url}")
-
-    resp = signed_url_backend.get_bytes(url=download_url)
-    try:
-        df = pd.read_csv(io.StringIO(resp.text))
-    except pd.errors.EmptyDataError:
-        _logger.warning(f"Empty Data Error for query {query}, returning an empty dataframe")
-        return pd.DataFrame()
-
-    return df
+import logging
+import os
+from typing import Optional, List
+from pandas import DataFrame
+import json
+from ..direct._config import _Config
+from ..direct._backend_apis._signed_url_backend import SignedUrlBackend
+import io
+
+import pandas as pd
+from enum import Enum
+from ._data_objects import TempTable, CSVFile
+from ._exceptions import TempTableNameNotFoundException
+
+_logger = logging.getLogger(__name__)
+
+DL_ACCOUNT = os.getenv("DL_ACCOUNT")
+
+region = os.getenv("DL_AWS_REGION", "us-east-1")
+is_external_user = os.getenv("IS_EXTERNAL_USER")
+uim_user_id = os.getenv("UIM_USER_ID")
+bucket_name = os.getenv("DL_TEMP_TABLE_BUCKET_NAME")
+redshift_cluster_id = os.getenv("REDSHIFT_CLUSTER_ID")
+redshift_database_name = os.getenv("REDSHIFT_DATABASE_NAME")
+
+
+class Source(Enum):
+    DATALAKE = 1
+    LAKEHOUSE = 2
+
+
+def query(query_str: str, temp_tables: Optional[List[TempTable]] = None) -> DataFrame:
+    """
+    :bdg-ref-danger:`Upcoming Feature <../upcoming_feature>`
+
+    Retrieve the results of a SQL query from the Morningstar Data Lake.
+
+    Args:
+        query_str: SQL query to be executed in Morningstar Data Lake
+        temp_tables: A list of temporary tables that will exist for the duration of the query.
+
+    Returns:
+        A DataFrame object with results of the SQL query.
+
+    :Examples:
+
+        Submit a query using a temp table
+
+    ::
+
+        import morningstar_data as md
+        import pandas as pd
+
+
+        df_my_table = pd.DataFrame({'sec_id': ['F0GBR0606A', 'F00000SYAH', 'F00000WP51'], 'closing_price': [128.372, 23.02, 528.33]})
+        df_query = md.datalake.query(query_str = 'select * from my_table;', temp_tables = [md.datalake.TempTable('my_table', df_my_table)])
+
+    :Output:
+
+        ===========  ===============
+         sec_id       closing_price
+        ===========  ===============
+        F0GBR0606A      128.372
+        F00000SYAH       23.02
+        F00000WP51      528.33
+        ===========  ===============
+
+    :Errors:
+        InvalidQueryException: When `query_str` contains invalid SQL syntax.
+
+        UnauthorizedDataLakeAccessError: When the calling user is not authorized to query the Morningstar Data Lake.
+
+        TempTableNameNotFoundException: When one or more temp tables being used are not found in the query string.
+
+    """
+    signed_url_backend = SignedUrlBackend()
+    config = _Config()
+
+    if temp_tables:
+        _logger.debug(f"Query function invoked with temp tables {temp_tables}")
+
+        missing_tables = []
+        for table in temp_tables:
+            if table.name is None or table.name.strip() == "":
+                _logger.debug("Temp table name is empty")
+                raise TempTableNameNotFoundException from None
+
+            if table.name not in query_str:
+                missing_tables.append(table.name)
+
+            body = {"is_temp": True, "table_name": table.name}
+
+            # get a signed url to upload this table to
+            _logger.debug(f"Uploading to stage table_name: {table.name}")
+            resp = json.loads(signed_url_backend.do_post_request(url=config.temp_table_url(), data=body))
+
+            table.table_stage_id = resp["table_id"]
+            upload_url = resp["upload_url"]
+
+            resp = signed_url_backend.put_csv_file(csv=CSVFile(table.df), signed_upload_url=upload_url)
+
+            _logger.info(f"Upload complete under the following s3 id {table.table_stage_id} with url {upload_url}")
+
+        if len(missing_tables) > 0:
+            _logger.warn(f" Not all temp_tables are in query_str, make sure your query is correct. Missing table names: {missing_tables}")
+
+    df = _get_query_as_df(signed_url_backend, config, query_str, temp_tables)
+
+    return df
+
+
+def _construct_query_endpoint_payload(query_str: str, temp_tables: Optional[List[TempTable]] = None) -> str:
+    # Sample body from md package to POST /query endpoint
+
+    # {
+    #     "query": "select * from xyz join temp_a join temp_b;",
+    #     "tables": [
+    #         {"table_id": "sd98f-dsf89sdf-sdf-df", "table_name": "temp_a", "columns": [{"name": "col1", "type": "int64"}, {"name": "col2", "type": "float"}]},
+    #         {"table_id": "ad98f-dsf89sdf-sdf-df", "table_name": "temp_b",
+    # "columns": [{"name": "col1", "type": "int64"}, {"name": "col2", "type": "float"}]},
+    #     ],
+    # }
+
+    # Within a Temp table the DF argument is not optional
+    if temp_tables:
+        payload = {
+            "query": query_str,
+            "tables": [
+                {"table_id": table.table_stage_id, "table_name": table.name, "columns": [{"name": col, "type": str(table.df[col].dtype)} for col in table.df.columns]}  # type: ignore
+                for table in temp_tables
+            ],
+        }
+    else:
+        payload = {"query": query_str}
+
+    return json.dumps(payload)
+
+
+def _get_query_as_df(signed_url_backend: SignedUrlBackend, config: _Config, query_str: str, temp_tables: Optional[List[TempTable]]) -> pd.DataFrame:
+
+    payload = _construct_query_endpoint_payload(query_str, temp_tables)
+
+    _logger.debug(f"Hitting the data lake query endpoint with this payload\n{payload}\n")
+
+    download_url_response = signed_url_backend.do_post_request(url=config.query_api_url(), data=payload)
+    download_url = json.loads(download_url_response)["url"]
+
+    _logger.info(f"Downloading from s3 at the url {download_url}")
+
+    resp = signed_url_backend.get_bytes(url=download_url)
+    try:
+        df = pd.read_csv(io.StringIO(resp.text))
+    except pd.errors.EmptyDataError:
+        _logger.warning(f"Empty Data Error for query {query}, returning an empty dataframe")
+        return pd.DataFrame()
+
+    return df
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/__init__.py` & `morningstar_data-1.3.0/morningstar_data/direct/__init__.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from .investment import investment_data, get_investment_data
-from .returns import returns, get_returns, excess_returns, get_excess_returns
-from .._base import _logger
-from .holdings import holdings, get_holdings, holding_dates, get_holding_dates, get_lookthrough_holdings
-from .performance_report import get_report, calculate_report, get_report_status, get_reports
-from . import user_items
-from .asset_flow import get_asset_flow, get_asset_flow_markets, get_asset_flow_data_points
-from .lookup import get_morningstar_data_sets, investment_universes, get_data_point_settings, investments, firms, get_brandings, portfolio_managers, companies
-from ._config import _Config
-from .data_type import Frequency, Blank, PeerGroupMethodology, Order
-from ._portfolio_data_set import PortfolioDataSet
-from .custom_database import my_database, firm_database
-from . import portfolio
-from .peer_group import get_peer_group_breakpoints
-
-config = _Config()
+from .investment import investment_data, get_investment_data
+from .returns import returns, get_returns, excess_returns, get_excess_returns
+from .._base import _logger
+from .holdings import holdings, get_holdings, holding_dates, get_holding_dates, get_lookthrough_holdings
+from .performance_report import get_report, calculate_report, get_report_status, get_reports
+from . import user_items
+from .asset_flow import get_asset_flow, get_asset_flow_markets, get_asset_flow_data_points
+from .lookup import get_morningstar_data_sets, investment_universes, get_data_point_settings, investments, firms, get_brandings, portfolio_managers, companies
+from ._config import _Config
+from .data_type import Frequency, Blank, PeerGroupMethodology, Order
+from ._portfolio_data_set import PortfolioDataSet
+from .custom_database import my_database, firm_database
+from . import portfolio
+from .peer_group import get_peer_group_breakpoints
+
+config = _Config()
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_api.py` & `morningstar_data-1.3.0/morningstar_data/direct/_api.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import requests
-
-from typing import Dict, Any, Optional, List, Union
-
-from .._base import _logger
-from ._exceptions import ApiRequestException, ApiResponseException, QueryLimitException
-
-# NOTE! We are not able to verify the SSL cert on Direct Search API since
-#       the VPC endpoint domain name is not on the server's SSL cert.
-#       So with a heavy heart, we disable the InsecureRequestWarning
-from urllib3.exceptions import InsecureRequestWarning
-from ._config import _Config
-from ._core_api import make_request
-
-
-_config = _Config()
-
-requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
-
-
-def _direct_api_request(method: str, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
-    """
-    Generic request method for the Direct API which covers headers and aspects
-    of response handling that are consistent across API calls
-
-    :method: Request method, eg. GET or POST
-    :url: Request URL
-    :data: (optional) POST message body, if any
-    """
-    headers = _config.get_headers()
-    _logger.debug(f"Requesting: {method} {url} with headers: {headers}")
-    try:
-        res = make_request(method, url, headers=headers, verify=False, data=data)
-        res.raise_for_status()
-
-        return res.json()
-    except requests.ConnectionError as e:
-        _logger.error(repr(e))
-        raise ApiRequestException(f"Failed connecting to {url}")
-    except requests.HTTPError as e:
-        message = f"Received {res.status_code} error from {url}"
-        json_response = res.json()
-        if res.status_code == 403 and "Exceed query limitation." in json_response["message"]:
-            query_limit = _get_security_data_query_limit()
-            raise QueryLimitException(query_limit) from None
-        else:
-            if "_meta" in json_response and "hint" in json_response["_meta"]:
-                message += f" ({json_response['_meta']['hint']})"
-            elif "message" in json_response:
-                message += f" ({json_response['message']})"
-            raise ApiResponseException(message, res.status_code)
-
-
-def _get_security_data_query_limit() -> str:
-    try:
-        headers = _config.get_headers()
-        url = f"{_config.securitydata_service_url()}v1/limitation/summary"
-
-        res = make_request("GET", url, headers=headers, verify=False)
-        json_response = res.json()
-        return str(json_response["limitationTotal"])
-    except:
-        return ""
+import requests
+
+from typing import Dict, Any, Optional, List, Union
+
+from .._base import _logger
+from ._exceptions import ApiRequestException, ApiResponseException, QueryLimitException
+
+# NOTE! We are not able to verify the SSL cert on Direct Search API since
+#       the VPC endpoint domain name is not on the server's SSL cert.
+#       So with a heavy heart, we disable the InsecureRequestWarning
+from urllib3.exceptions import InsecureRequestWarning
+from ._config import _Config
+from ._core_api import make_request
+
+
+_config = _Config()
+
+requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
+
+
+def _direct_api_request(method: str, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
+    """
+    Generic request method for the Direct API which covers headers and aspects
+    of response handling that are consistent across API calls
+
+    :method: Request method, eg. GET or POST
+    :url: Request URL
+    :data: (optional) POST message body, if any
+    """
+    headers = _config.get_headers()
+    _logger.debug(f"Requesting: {method} {url} with headers: {headers}")
+    try:
+        res = make_request(method, url, headers=headers, verify=False, data=data)
+        res.raise_for_status()
+
+        return res.json()
+    except requests.ConnectionError as e:
+        _logger.error(repr(e))
+        raise ApiRequestException(f"Failed connecting to {url}")
+    except requests.HTTPError as e:
+        message = f"Received {res.status_code} error from {url}"
+        json_response = res.json()
+        if res.status_code == 403 and "Exceed query limitation." in json_response["message"]:
+            query_limit = _get_security_data_query_limit()
+            raise QueryLimitException(query_limit) from None
+        else:
+            if "_meta" in json_response and "hint" in json_response["_meta"]:
+                message += f" ({json_response['_meta']['hint']})"
+            elif "message" in json_response:
+                message += f" ({json_response['message']})"
+            raise ApiResponseException(message, res.status_code)
+
+
+def _get_security_data_query_limit() -> str:
+    try:
+        headers = _config.get_headers()
+        url = f"{_config.securitydata_service_url()}v1/limitation/summary"
+
+        res = make_request("GET", url, headers=headers, verify=False)
+        json_response = res.json()
+        return str(json_response["limitationTotal"])
+    except:
+        return ""
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_backend_apis/_delivery_backend.py` & `morningstar_data-1.3.0/morningstar_data/direct/_backend_apis/_delivery_backend.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import logging
-import requests
-import os
-import uuid
-
-from typing import Any, Dict, Optional, Union
-from ...direct._base_api import APIBackend
-from ...direct._exceptions import NetworkExceptionError, UnauthorizedDeliveryException
-
-from .._core_api import make_request
-
-
-_logger = logging.getLogger(__name__)
-
-
-class DeliveryAPIBackend(APIBackend):
-    def do_post_request(self, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
-        """
-        Makes a POST request
-        """
-        return self._make_request(url, "POST", data)
-
-    def _get_request_id(self) -> str:
-        """Returns the request id for use in POST requests"""
-        request_id = os.getenv("REQUEST_ID", str(uuid.uuid4()))
-        _logger.info(f"RequestId: {request_id} passed to POST requests")
-        return request_id
-
-    def _make_request(self, url: str, method: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
-        _logger.info(f"Requesting: {method} {url}")
-        try:
-            self.headers["X-API-RequestId"] = self._get_request_id()
-            res = make_request(method, url, headers=self.headers, verify=False, data=data)
-            res.raise_for_status()
-            return res.json()
-        except requests.ConnectionError:
-            raise NetworkExceptionError from None
-        except requests.HTTPError:
-            self._handle_custom_http_errors(res)
-            self._handle_default_http_errors(res)
-
-    def _handle_custom_http_errors(self, res: Any) -> Any:
-        try:
-            response_message = res.json()["message"]
-        except requests.JSONDecodeError:
-            response_message = res.text
-
-        if res.status_code == 401:
-            _logger.debug(f"Unauthorized Error: {res.status_code} {response_message}")
-            raise UnauthorizedDeliveryException from None
+import logging
+import requests
+import os
+import uuid
+
+from typing import Any, Dict, Optional, Union
+from ...direct._base_api import APIBackend
+from ...direct._exceptions import NetworkExceptionError, UnauthorizedDeliveryException
+
+from .._core_api import make_request
+
+
+_logger = logging.getLogger(__name__)
+
+
+class DeliveryAPIBackend(APIBackend):
+    def do_post_request(self, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
+        """
+        Makes a POST request
+        """
+        return self._make_request(url, "POST", data)
+
+    def _get_request_id(self) -> str:
+        """Returns the request id for use in POST requests"""
+        request_id = os.getenv("REQUEST_ID", str(uuid.uuid4()))
+        _logger.info(f"RequestId: {request_id} passed to POST requests")
+        return request_id
+
+    def _make_request(self, url: str, method: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
+        _logger.info(f"Requesting: {method} {url}")
+        try:
+            self.headers["X-API-RequestId"] = self._get_request_id()
+            res = make_request(method, url, headers=self.headers, verify=False, data=data)
+            res.raise_for_status()
+            return res.json()
+        except requests.ConnectionError:
+            raise NetworkExceptionError from None
+        except requests.HTTPError:
+            self._handle_custom_http_errors(res)
+            self._handle_default_http_errors(res)
+
+    def _handle_custom_http_errors(self, res: Any) -> Any:
+        try:
+            response_message = res.json()["message"]
+        except requests.JSONDecodeError:
+            response_message = res.text
+
+        if res.status_code == 401:
+            _logger.debug(f"Unauthorized Error: {res.status_code} {response_message}")
+            raise UnauthorizedDeliveryException from None
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_backend_apis/_holdings_backend.py` & `morningstar_data-1.3.0/morningstar_data/direct/_backend_apis/_holdings_backend.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,143 +1,143 @@
-import os
-from .._base_api import APIBackend
-from typing import Any, Dict, Optional, Union
-from .._exceptions import BadRequestException, NetworkExceptionError, ResourceNotFoundError, ForbiddenError
-
-from ..._base import _logger
-from .._error_messages import (
-    RESOURCE_NOT_FOUND_ERROR_HOLDING,
-)
-
-import requests
-import uuid
-
-from .._core_api import make_request
-from .._config import _Config
-
-_config = _Config()
-
-
-class HoldingAPIBackend(APIBackend):
-    """
-    Subclass to call the Holding API and handle any HTTP errors that occur.
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def _handle_custom_http_errors(self, res: Any) -> Any:
-        """
-        Handle HTTP errors with custom error messages
-        """
-        response_message = res.json()["message"]
-        if res.status_code == 404:
-            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
-            raise ResourceNotFoundError(RESOURCE_NOT_FOUND_ERROR_HOLDING) from None
-
-
-class FoFAPIBackend(APIBackend):
-    """
-    Subclass to call the FoF API and handle any HTTP errors that occur.
-    Temporarily implements do_get_request and do_put_request becuase the response of FOF api is not JSON
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def do_get_request(self, url: str) -> Any:
-        """
-        Makes a GET request
-        """
-        return self._make_request(url, "GET")
-
-    def do_post_request(self, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
-        """
-        Makes a POST request
-        """
-        return self._make_request(url, "POST", data)
-
-    def _make_request(self, url: str, method: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
-        """
-        Request and handle OK (status_code = 200) and network error responses.
-        """
-        _logger.info(f"Requesting: {method} {url}")
-        try:
-            res = make_request(method, url, headers=self.headers, verify=True, data=data)
-            res.raise_for_status()
-            # We have asked FOF team to return JSON object in the API, so we don't have to implement this class completely like this.
-            # https://mswiki.morningstar.com/display/DWH/AL+FOF+Lookthrough+Holding?focusedCommentId=645255358#comment-645255358
-            return res.json()
-        except requests.ConnectionError:
-            raise NetworkExceptionError from None
-        except requests.HTTPError:
-            self._handle_custom_http_errors(res)
-            self._handle_default_http_errors(res)
-
-    def _handle_custom_http_errors(self, res: Any) -> Any:
-        """
-        Handle HTTP errors with custom error messages
-        """
-        response_message = res.text
-        _logger.error(response_message)
-        status_code = res.status_code
-
-        if status_code in [404, 500]:
-            raise NetworkExceptionError from None
-        elif status_code == 401:
-            raise ForbiddenError from None
-        else:
-            raise BadRequestException(response_message)
-
-    def _handle_default_http_errors(self, res: Any) -> Any:
-        """
-        Handle HTTP errors with standard messages
-        """
-        response_message = res.text
-        _logger.error(response_message)
-        raise
-
-
-class AMSAPIBackend(APIBackend):
-    """
-    Subclass to call a Signed url and handle any HTTP errors that occur.
-    Temporarily implements do_get_request becuase the request does not need headers and the response need not be JSON
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def do_get_request(self, url: str) -> Any:
-        """
-        Makes a GET request
-        """
-        return self._make_request(url, "GET")
-
-    def _make_request(self, url: str, method: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
-        """
-        Request and handle OK (status_code = 200) and network error responses.
-        """
-        _logger.info(f"Requesting: {method} {url}")
-        try:
-            # We will remove this after testing
-
-            self.headers["authorization"] = f"Bearer {_config.get_uim_token()}"  # Because we don't have  PROD FOF API, and dont' have custom user data in the NON PROD DO APIs
-            self.headers["x-api-requestid"] = str(uuid.uuid4())
-            self.headers["x-api-userid"] = os.environ["UIM_USER_ID"]
-
-            res = make_request(method, url, headers=self.headers, verify=True, data=data)
-            res.raise_for_status()
-            return res.json()
-        except requests.ConnectionError:
-            raise NetworkExceptionError from None
-        except requests.HTTPError:
-            self._handle_custom_http_errors(res)
-            self._handle_default_http_errors(res)
-
-    def _handle_custom_http_errors(self, res: Any) -> Any:
-        """
-        Handle HTTP errors with custom error messages
-        """
-        response_message = res.json()["message"]
-        if res.status_code == 404:
-            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
-            raise ResourceNotFoundError(RESOURCE_NOT_FOUND_ERROR_HOLDING) from None
+import os
+from .._base_api import APIBackend
+from typing import Any, Dict, Optional, Union
+from .._exceptions import BadRequestException, NetworkExceptionError, ResourceNotFoundError, ForbiddenError
+
+from ..._base import _logger
+from .._error_messages import (
+    RESOURCE_NOT_FOUND_ERROR_HOLDING,
+)
+
+import requests
+import uuid
+
+from .._core_api import make_request
+from .._config import _Config
+
+_config = _Config()
+
+
+class HoldingAPIBackend(APIBackend):
+    """
+    Subclass to call the Holding API and handle any HTTP errors that occur.
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def _handle_custom_http_errors(self, res: Any) -> Any:
+        """
+        Handle HTTP errors with custom error messages
+        """
+        response_message = res.json()["message"]
+        if res.status_code == 404:
+            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
+            raise ResourceNotFoundError(RESOURCE_NOT_FOUND_ERROR_HOLDING) from None
+
+
+class FoFAPIBackend(APIBackend):
+    """
+    Subclass to call the FoF API and handle any HTTP errors that occur.
+    Temporarily implements do_get_request and do_put_request becuase the response of FOF api is not JSON
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def do_get_request(self, url: str) -> Any:
+        """
+        Makes a GET request
+        """
+        return self._make_request(url, "GET")
+
+    def do_post_request(self, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
+        """
+        Makes a POST request
+        """
+        return self._make_request(url, "POST", data)
+
+    def _make_request(self, url: str, method: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
+        """
+        Request and handle OK (status_code = 200) and network error responses.
+        """
+        _logger.info(f"Requesting: {method} {url}")
+        try:
+            res = make_request(method, url, headers=self.headers, verify=True, data=data)
+            res.raise_for_status()
+            # We have asked FOF team to return JSON object in the API, so we don't have to implement this class completely like this.
+            # https://mswiki.morningstar.com/display/DWH/AL+FOF+Lookthrough+Holding?focusedCommentId=645255358#comment-645255358
+            return res.json()
+        except requests.ConnectionError:
+            raise NetworkExceptionError from None
+        except requests.HTTPError:
+            self._handle_custom_http_errors(res)
+            self._handle_default_http_errors(res)
+
+    def _handle_custom_http_errors(self, res: Any) -> Any:
+        """
+        Handle HTTP errors with custom error messages
+        """
+        response_message = res.text
+        _logger.error(response_message)
+        status_code = res.status_code
+
+        if status_code in [404, 500]:
+            raise NetworkExceptionError from None
+        elif status_code == 401:
+            raise ForbiddenError from None
+        else:
+            raise BadRequestException(response_message)
+
+    def _handle_default_http_errors(self, res: Any) -> Any:
+        """
+        Handle HTTP errors with standard messages
+        """
+        response_message = res.text
+        _logger.error(response_message)
+        raise
+
+
+class AMSAPIBackend(APIBackend):
+    """
+    Subclass to call a Signed url and handle any HTTP errors that occur.
+    Temporarily implements do_get_request becuase the request does not need headers and the response need not be JSON
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def do_get_request(self, url: str) -> Any:
+        """
+        Makes a GET request
+        """
+        return self._make_request(url, "GET")
+
+    def _make_request(self, url: str, method: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
+        """
+        Request and handle OK (status_code = 200) and network error responses.
+        """
+        _logger.info(f"Requesting: {method} {url}")
+        try:
+            # We will remove this after testing
+
+            self.headers["authorization"] = f"Bearer {_config.get_uim_token()}"  # Because we don't have  PROD FOF API, and dont' have custom user data in the NON PROD DO APIs
+            self.headers["x-api-requestid"] = str(uuid.uuid4())
+            self.headers["x-api-userid"] = os.environ["UIM_USER_ID"]
+
+            res = make_request(method, url, headers=self.headers, verify=True, data=data)
+            res.raise_for_status()
+            return res.json()
+        except requests.ConnectionError:
+            raise NetworkExceptionError from None
+        except requests.HTTPError:
+            self._handle_custom_http_errors(res)
+            self._handle_default_http_errors(res)
+
+    def _handle_custom_http_errors(self, res: Any) -> Any:
+        """
+        Handle HTTP errors with custom error messages
+        """
+        response_message = res.json()["message"]
+        if res.status_code == 404:
+            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
+            raise ResourceNotFoundError(RESOURCE_NOT_FOUND_ERROR_HOLDING) from None
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_backend_apis/_signed_url_backend.py` & `morningstar_data-1.3.0/morningstar_data/direct/_backend_apis/_signed_url_backend.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-from ..._base import _logger
-from ...datalake._data_objects.csvfile import CSVFile
-from ...datalake._exceptions import InvalidQueryException, UnauthorizedDataLakeAccessError
-from ...direct._base_api import APIBackend
-from ...direct._core_api import make_request
-from ...direct._error_messages import RESOURCE_NOT_FOUND_ERROR_HOLDING
-from ...direct._exceptions import NetworkExceptionError, ResourceNotFoundError
-
-
-import requests
-
-
-import json
-from typing import Any, Dict, Optional, Union
-
-
-class SignedUrlBackend(APIBackend):
-    """
-    Subclass to call a Signed url and handle any HTTP errors that occur.
-    Temporarily implements do_get_request becuase the request does not need headers and the response need not be JSON
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def do_post_request(self, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
-        """
-        Makes a POST request
-        """
-        return self._make_request(url=url, method="POST", data=data)
-
-    def do_put_request(self, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
-        """
-        Makes a PUT request
-        """
-        return self._make_request(url=url, method="PUT", data=data)
-
-    def do_get_request(self, url: str) -> Any:
-        """
-        Makes a GET request
-        """
-        return self._make_request(url, "GET")
-
-    def put_csv_file(self, csv: CSVFile, signed_upload_url: str) -> Any:
-        """
-        Uploads a CSV file to S3 presigned url
-        """
-        return requests.put(url=signed_upload_url, data=csv.csv_buffer.getvalue())
-
-    def get_bytes(self, url: str) -> Any:
-        """
-        Downloads bytes from S3 presigned url
-        """
-        res = requests.get(url)
-        res.raise_for_status()
-        return res
-
-    def _make_request(self, url: str, method: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
-        """
-        Request and handle OK (status_code = 200) and network error responses.
-        """
-        _logger.info(f"Requesting: {method} {url}")
-        try:
-            res = make_request(method=method, url=url, headers=self.headers, verify=False, data=json.dumps(data))
-            res.raise_for_status()
-            return res.text
-        except requests.ConnectionError:
-            raise NetworkExceptionError from None
-        except requests.HTTPError:
-            self._handle_custom_http_errors(res)
-            self._handle_default_http_errors(res)
-
-    def _handle_custom_http_errors(self, res: Any) -> Any:
-        """
-        Handle HTTP errors with custom error messages
-        """
-        try:
-            response_message = res.json()["message"]
-        except requests.JSONDecodeError:
-            response_message = res.text
-
-        if res.status_code == 400:
-            _logger.debug(f"Bad Request Error: {res.status_code} {response_message}")
-            raise InvalidQueryException(response_message) from None
-        if res.status_code == 401:
-            _logger.debug(f"Unauthorized Error: {res.status_code} {response_message}")
-            raise UnauthorizedDataLakeAccessError from None
-        if res.status_code == 404:
-            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
-            raise ResourceNotFoundError(RESOURCE_NOT_FOUND_ERROR_HOLDING) from None
+from ..._base import _logger
+from ...datalake._data_objects.csvfile import CSVFile
+from ...datalake._exceptions import InvalidQueryException, UnauthorizedDataLakeAccessError
+from ...direct._base_api import APIBackend
+from ...direct._core_api import make_request
+from ...direct._error_messages import RESOURCE_NOT_FOUND_ERROR_HOLDING
+from ...direct._exceptions import NetworkExceptionError, ResourceNotFoundError
+
+
+import requests
+
+
+import json
+from typing import Any, Dict, Optional, Union
+
+
+class SignedUrlBackend(APIBackend):
+    """
+    Subclass to call a Signed url and handle any HTTP errors that occur.
+    Temporarily implements do_get_request becuase the request does not need headers and the response need not be JSON
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def do_post_request(self, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
+        """
+        Makes a POST request
+        """
+        return self._make_request(url=url, method="POST", data=data)
+
+    def do_put_request(self, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
+        """
+        Makes a PUT request
+        """
+        return self._make_request(url=url, method="PUT", data=data)
+
+    def do_get_request(self, url: str) -> Any:
+        """
+        Makes a GET request
+        """
+        return self._make_request(url, "GET")
+
+    def put_csv_file(self, csv: CSVFile, signed_upload_url: str) -> Any:
+        """
+        Uploads a CSV file to S3 presigned url
+        """
+        return requests.put(url=signed_upload_url, data=csv.csv_buffer.getvalue())
+
+    def get_bytes(self, url: str) -> Any:
+        """
+        Downloads bytes from S3 presigned url
+        """
+        res = requests.get(url)
+        res.raise_for_status()
+        return res
+
+    def _make_request(self, url: str, method: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
+        """
+        Request and handle OK (status_code = 200) and network error responses.
+        """
+        _logger.info(f"Requesting: {method} {url}")
+        try:
+            res = make_request(method=method, url=url, headers=self.headers, verify=False, data=json.dumps(data))
+            res.raise_for_status()
+            return res.text
+        except requests.ConnectionError:
+            raise NetworkExceptionError from None
+        except requests.HTTPError:
+            self._handle_custom_http_errors(res)
+            self._handle_default_http_errors(res)
+
+    def _handle_custom_http_errors(self, res: Any) -> Any:
+        """
+        Handle HTTP errors with custom error messages
+        """
+        try:
+            response_message = res.json()["message"]
+        except requests.JSONDecodeError:
+            response_message = res.text
+
+        if res.status_code == 400:
+            _logger.debug(f"Bad Request Error: {res.status_code} {response_message}")
+            raise InvalidQueryException(response_message) from None
+        if res.status_code == 401:
+            _logger.debug(f"Unauthorized Error: {res.status_code} {response_message}")
+            raise UnauthorizedDataLakeAccessError from None
+        if res.status_code == 404:
+            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
+            raise ResourceNotFoundError(RESOURCE_NOT_FOUND_ERROR_HOLDING) from None
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_base_api.py` & `morningstar_data-1.3.0/morningstar_data/direct/_base_api.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-import simplejson as json
-from abc import ABC, abstractmethod
-from typing import Any, Dict, Optional, Union
-
-import requests
-
-# NOTE! We are not able to verify the SSL cert on Direct Search API since
-#       the VPC endpoint domain name is not on the server's SSL cert.
-#       So with a heavy heart, we disable the InsecureRequestWarning
-from urllib3.exceptions import InsecureRequestWarning
-
-from .._base import _logger
-from . import _error_messages
-from ._config import _Config
-from ._exceptions import AccessDeniedError, BadRequestException, ClientError, ForbiddenError, InternalServerError, NetworkExceptionError, TimeoutError
-from ._core_api import make_request
-
-_config = _Config()
-
-requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
-
-
-class APIBackend(ABC):
-    """
-    Abstract class for all API requests
-    """
-
-    def __init__(self) -> None:
-        self.headers = _config.get_headers()
-
-    def do_get_request(self, url: str) -> Any:
-        """
-        Makes a GET request
-        """
-        return self._make_request(url, "GET")
-
-    def do_post_request(self, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
-        """
-        Makes a POST request
-        """
-        return self._make_request(url, "POST", data)
-
-    def do_put_request(self, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
-        """
-        Makes a PUT request
-        """
-        return self._make_request(url, "PUT", data)
-
-    def _make_request(self, url: str, method: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
-        """
-        Request and handle OK (status_code = 200) and network error responses.
-        """
-        _logger.info(f"Requesting: {method} {url}")
-        try:
-            res = make_request(method, url, headers=self.headers, verify=False, data=data)
-            res.raise_for_status()
-            return res.json()
-        except requests.ConnectionError as e:
-            raise NetworkExceptionError from None
-        except requests.HTTPError as e:
-            self._handle_custom_http_errors(res)
-            self._handle_default_http_errors(res)
-
-    def _handle_default_http_errors(self, res: Any) -> Any:
-        """
-        Handle HTTP errors with standard messages
-        """
-        try:
-            response_message = res.json()["message"]
-        except KeyError:
-            response_message = res.json()
-            _logger.debug("DO Request Error")
-        if res.status_code == 401:
-            _logger.debug(f"Access Denied Error: {res.status_code} {response_message}")
-            raise AccessDeniedError from None
-        elif res.status_code == 403:
-            _logger.debug(f"Forbidden Error: {res.status_code} {response_message}")
-            raise ForbiddenError from None
-        elif res.status_code == 408:
-            _logger.debug(f"Timeout Error: {res.status_code} {response_message}")
-            raise TimeoutError from None
-        elif res.status_code == 400:
-            _logger.debug(f"Bad Request: {res.status_code} {response_message}")
-            raise BadRequestException(_error_messages.BAD_REQUEST_ERROR) from None
-        elif res.status_code > 400 and res.status_code < 500:
-            _logger.debug(f"Client Error: {res.status_code} {response_message}")
-            raise ClientError(_error_messages.CLIENT_ERROR) from None
-        else:
-            _logger.debug(f"Internal Server Error: {res.status_code} {response_message}")
-            raise InternalServerError(_error_messages.INTERNAL_SERVER_ERROR) from None
-
-    @abstractmethod
-    def _handle_custom_http_errors(self, res: Any) -> None:
-        """
-        Method to handle special HTTP errors with custom error messages
-        """
-        pass
+import simplejson as json
+from abc import ABC, abstractmethod
+from typing import Any, Dict, Optional, Union
+
+import requests
+
+# NOTE! We are not able to verify the SSL cert on Direct Search API since
+#       the VPC endpoint domain name is not on the server's SSL cert.
+#       So with a heavy heart, we disable the InsecureRequestWarning
+from urllib3.exceptions import InsecureRequestWarning
+
+from .._base import _logger
+from . import _error_messages
+from ._config import _Config
+from ._exceptions import AccessDeniedError, BadRequestException, ClientError, ForbiddenError, InternalServerError, NetworkExceptionError, TimeoutError
+from ._core_api import make_request
+
+_config = _Config()
+
+requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
+
+
+class APIBackend(ABC):
+    """
+    Abstract class for all API requests
+    """
+
+    def __init__(self) -> None:
+        self.headers = _config.get_headers()
+
+    def do_get_request(self, url: str) -> Any:
+        """
+        Makes a GET request
+        """
+        return self._make_request(url, "GET")
+
+    def do_post_request(self, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
+        """
+        Makes a POST request
+        """
+        return self._make_request(url, "POST", data)
+
+    def do_put_request(self, url: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
+        """
+        Makes a PUT request
+        """
+        return self._make_request(url, "PUT", data)
+
+    def _make_request(self, url: str, method: str, data: Optional[Union[Dict[Any, Any], str]] = None) -> Any:
+        """
+        Request and handle OK (status_code = 200) and network error responses.
+        """
+        _logger.info(f"Requesting: {method} {url}")
+        try:
+            res = make_request(method, url, headers=self.headers, verify=False, data=data)
+            res.raise_for_status()
+            return res.json()
+        except requests.ConnectionError as e:
+            raise NetworkExceptionError from None
+        except requests.HTTPError as e:
+            self._handle_custom_http_errors(res)
+            self._handle_default_http_errors(res)
+
+    def _handle_default_http_errors(self, res: Any) -> Any:
+        """
+        Handle HTTP errors with standard messages
+        """
+        try:
+            response_message = res.json()["message"]
+        except KeyError:
+            response_message = res.json()
+            _logger.debug("DO Request Error")
+        if res.status_code == 401:
+            _logger.debug(f"Access Denied Error: {res.status_code} {response_message}")
+            raise AccessDeniedError from None
+        elif res.status_code == 403:
+            _logger.debug(f"Forbidden Error: {res.status_code} {response_message}")
+            raise ForbiddenError from None
+        elif res.status_code == 408:
+            _logger.debug(f"Timeout Error: {res.status_code} {response_message}")
+            raise TimeoutError from None
+        elif res.status_code == 400:
+            _logger.debug(f"Bad Request: {res.status_code} {response_message}")
+            raise BadRequestException(_error_messages.BAD_REQUEST_ERROR) from None
+        elif res.status_code > 400 and res.status_code < 500:
+            _logger.debug(f"Client Error: {res.status_code} {response_message}")
+            raise ClientError(_error_messages.CLIENT_ERROR) from None
+        else:
+            _logger.debug(f"Internal Server Error: {res.status_code} {response_message}")
+            raise InternalServerError(_error_messages.INTERNAL_SERVER_ERROR) from None
+
+    @abstractmethod
+    def _handle_custom_http_errors(self, res: Any) -> None:
+        """
+        Method to handle special HTTP errors with custom error messages
+        """
+        pass
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_config.py` & `morningstar_data-1.3.0/morningstar_data/direct/_config.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,137 +1,137 @@
-import base64
-import simplejson as json
-import os
-import re
-from os import environ
-
-from dataclasses import dataclass, field
-from typing import Dict
-from ._exceptions import EAMSTokenDoesNotExistError, MalformedJWTError, CredentialsException
-
-
-@dataclass
-class _Config:
-    def __init__(self) -> None:
-        self._MD_API: str = os.getenv("MD_API", "https://www.us-api.morningstar.com/md-api/")
-        md_auth_token = md_auth_token = os.getenv("MD_AUTH_TOKEN", os.getenv("UIM_JWT", ""))
-        self.token = md_auth_token
-        if self.token == "":
-            raise CredentialsException("Please set up MD_AUTH_TOKEN environment variable to access the morningstar_data package")
-
-    @property
-    def token(self) -> str:
-        # TODO: Test the token
-        return self._JWT
-
-    @token.setter
-    def token(self, new_token: str) -> None:
-        fixed_token = self._filter_invalid_jwt(new_token)
-        self._JWT = fixed_token
-
-    def get_uim_token(self) -> str:
-        return self.token
-
-    def get_headers(self, add_headers: Dict[str, str] = {}) -> Dict[str, str]:
-        headers = {
-            "X-API-ComponentId": os.getenv("DO_API_REQUEST_ORIGIN", "analyticslab"),
-            "X-API-Sourceapp": os.getenv("DO_API_REQUEST_ORIGIN", "morningstar-data"),
-            "X-API-ProductId": "Direct",
-            "Content-Type": "application/json",
-            **add_headers,
-        }
-
-        # This will allow us to make DO API requests on behalf of another user.
-        # EAMS impersonation is going away. We are using this temporarily.
-        if environ.get("USE_EAMS_IMPERSONATION"):
-            # EAMS_JWT is always on the environment in Analytics Lab.
-            # We only want to use it in DNA Lab api when USE_EAMS_IMPERSONATION is set to True
-            if "EAMS_JWT" in environ:
-                headers["X-API-JsonWebToken"] = environ["EAMS_JWT"]
-            else:
-                raise EAMSTokenDoesNotExistError("EAMS_JWT does not exist on the environment.")
-        else:
-            headers["authorization"] = f"Bearer {self.get_uim_token()}"
-
-        return headers
-
-    def object_service_url(self) -> str:
-        return f"{self._MD_API}proxy_request/object_service/"
-
-    def custom_data_points_service_url(self) -> str:
-        return f"{self._MD_API}proxy_request/custom_data_points_service/"
-
-    def securitydata_service_url(self) -> str:
-        return f"{self._MD_API}proxy_request/security_data_service/"
-
-    def searches_service_url(self) -> str:
-        return f"{self._MD_API}proxy_request/searches_service/"
-
-    def portfolio_service_url(self) -> str:
-        return f"{self._MD_API}proxy_request/portfolio_service/"
-
-    def performancereport_service_url(self) -> str:
-        return f"{self._MD_API}proxy_request/performancereport_service/"
-
-    def performancereport_export_service_url(self) -> str:
-        return f"{self._MD_API}proxy_request/performancereport_export_service/"
-
-    def dataset_service_url(self) -> str:
-        return f"{self._MD_API}proxy_request/dataset_service/"
-
-    def data_point_service_url(self) -> str:
-        return f"{self._MD_API}proxy_request/data_point_service/"
-
-    def asset_service_url(self) -> str:
-        return f"{self._MD_API}proxy_request/asset_service/"
-
-    def peergroup_service_url(self) -> str:
-        return f"{self._MD_API}proxy_request/peergroup_service/"
-
-    def fof_api_url(self) -> str:
-        return f"{self._MD_API}proxy_request/fof_service/"
-
-    def al_proxy_api_url(self) -> str:
-        return f"{self._MD_API}proxy_request/al_proxy_api/"
-
-    def mds_api_url(self) -> str:
-        return f"{self._MD_API}proxy_request/mds_api/"
-
-    def temp_table_url(self) -> str:
-        return f"{self._MD_API}proxy_request/temp_table_service/"
-
-    def query_api_url(self) -> str:
-        return f"{self._MD_API}proxy_request/lakehouse_query_service/"
-
-    def _filter_invalid_jwt(self, jwt: str) -> str:
-        # Define the regular expression pattern to match a valid JWT
-        pattern = r"^[A-Za-z0-9_-]*\.?[A-Za-z0-9_-]*\.?[A-Za-z0-9_-]*$"
-
-        # Check if the JWT matches the valid pattern
-        if not re.match(pattern, jwt):
-            # Replace invalid characters with an empty string
-            jwt = re.sub(r"[^\w\.-]", "", jwt)
-
-        # jwt = jwt.strip()
-        # # Use regex to replace
-        # jwt = re.sub(pattern, "", jwt)
-
-        # Check that the JWT has 3 parts
-        if len(jwt.split(".")) != 3:
-            raise MalformedJWTError
-
-        # Split the JWT into header, payload, and signature
-        header, payload, signature = jwt.split(".")
-
-        # Filter out any invalid characters from the header and payload
-        decoded_header = base64.urlsafe_b64decode(header + "=" * (4 - len(header) % 4)).decode("utf-8", "ignore")
-        decoded_payload = base64.urlsafe_b64decode(payload + "=" * (4 - len(payload) % 4)).decode("utf-8", "ignore")
-
-        # Check that the filtered header and payload are valid JSON objects
-        try:
-            json.loads(decoded_header)
-            json.loads(decoded_payload)
-        except ValueError:
-            raise MalformedJWTError from None
-
-        # If we got here, the JWT is valid and filtered
-        return ".".join([header, payload, signature])
+import base64
+import simplejson as json
+import os
+import re
+from os import environ
+
+from dataclasses import dataclass, field
+from typing import Dict
+from ._exceptions import EAMSTokenDoesNotExistError, MalformedJWTError, CredentialsException
+
+
+@dataclass
+class _Config:
+    def __init__(self) -> None:
+        self._MD_API: str = os.getenv("MD_API", "https://www.us-api.morningstar.com/md-api/")
+        md_auth_token = md_auth_token = os.getenv("MD_AUTH_TOKEN", os.getenv("UIM_JWT", ""))
+        self.token = md_auth_token
+        if self.token == "":
+            raise CredentialsException("Please set up MD_AUTH_TOKEN environment variable to access the morningstar_data package")
+
+    @property
+    def token(self) -> str:
+        # TODO: Test the token
+        return self._JWT
+
+    @token.setter
+    def token(self, new_token: str) -> None:
+        fixed_token = self._filter_invalid_jwt(new_token)
+        self._JWT = fixed_token
+
+    def get_uim_token(self) -> str:
+        return self.token
+
+    def get_headers(self, add_headers: Dict[str, str] = {}) -> Dict[str, str]:
+        headers = {
+            "X-API-ComponentId": os.getenv("DO_API_REQUEST_ORIGIN", "analyticslab"),
+            "X-API-Sourceapp": os.getenv("DO_API_REQUEST_ORIGIN", "morningstar-data"),
+            "X-API-ProductId": "Direct",
+            "Content-Type": "application/json",
+            **add_headers,
+        }
+
+        # This will allow us to make DO API requests on behalf of another user.
+        # EAMS impersonation is going away. We are using this temporarily.
+        if environ.get("USE_EAMS_IMPERSONATION"):
+            # EAMS_JWT is always on the environment in Analytics Lab.
+            # We only want to use it in DNA Lab api when USE_EAMS_IMPERSONATION is set to True
+            if "EAMS_JWT" in environ:
+                headers["X-API-JsonWebToken"] = environ["EAMS_JWT"]
+            else:
+                raise EAMSTokenDoesNotExistError("EAMS_JWT does not exist on the environment.")
+        else:
+            headers["authorization"] = f"Bearer {self.get_uim_token()}"
+
+        return headers
+
+    def object_service_url(self) -> str:
+        return f"{self._MD_API}proxy_request/object_service/"
+
+    def custom_data_points_service_url(self) -> str:
+        return f"{self._MD_API}proxy_request/custom_data_points_service/"
+
+    def securitydata_service_url(self) -> str:
+        return f"{self._MD_API}proxy_request/security_data_service/"
+
+    def searches_service_url(self) -> str:
+        return f"{self._MD_API}proxy_request/searches_service/"
+
+    def portfolio_service_url(self) -> str:
+        return f"{self._MD_API}proxy_request/portfolio_service/"
+
+    def performancereport_service_url(self) -> str:
+        return f"{self._MD_API}proxy_request/performancereport_service/"
+
+    def performancereport_export_service_url(self) -> str:
+        return f"{self._MD_API}proxy_request/performancereport_export_service/"
+
+    def dataset_service_url(self) -> str:
+        return f"{self._MD_API}proxy_request/dataset_service/"
+
+    def data_point_service_url(self) -> str:
+        return f"{self._MD_API}proxy_request/data_point_service/"
+
+    def asset_service_url(self) -> str:
+        return f"{self._MD_API}proxy_request/asset_service/"
+
+    def peergroup_service_url(self) -> str:
+        return f"{self._MD_API}proxy_request/peergroup_service/"
+
+    def fof_api_url(self) -> str:
+        return f"{self._MD_API}proxy_request/fof_service/"
+
+    def al_proxy_api_url(self) -> str:
+        return f"{self._MD_API}proxy_request/al_proxy_api/"
+
+    def mds_api_url(self) -> str:
+        return f"{self._MD_API}proxy_request/mds_api/"
+
+    def temp_table_url(self) -> str:
+        return f"{self._MD_API}proxy_request/temp_table_service/"
+
+    def query_api_url(self) -> str:
+        return f"{self._MD_API}proxy_request/lakehouse_query_service/"
+
+    def _filter_invalid_jwt(self, jwt: str) -> str:
+        # Define the regular expression pattern to match a valid JWT
+        pattern = r"^[A-Za-z0-9_-]*\.?[A-Za-z0-9_-]*\.?[A-Za-z0-9_-]*$"
+
+        # Check if the JWT matches the valid pattern
+        if not re.match(pattern, jwt):
+            # Replace invalid characters with an empty string
+            jwt = re.sub(r"[^\w\.-]", "", jwt)
+
+        # jwt = jwt.strip()
+        # # Use regex to replace
+        # jwt = re.sub(pattern, "", jwt)
+
+        # Check that the JWT has 3 parts
+        if len(jwt.split(".")) != 3:
+            raise MalformedJWTError
+
+        # Split the JWT into header, payload, and signature
+        header, payload, signature = jwt.split(".")
+
+        # Filter out any invalid characters from the header and payload
+        decoded_header = base64.urlsafe_b64decode(header + "=" * (4 - len(header) % 4)).decode("utf-8", "ignore")
+        decoded_payload = base64.urlsafe_b64decode(payload + "=" * (4 - len(payload) % 4)).decode("utf-8", "ignore")
+
+        # Check that the filtered header and payload are valid JSON objects
+        try:
+            json.loads(decoded_header)
+            json.loads(decoded_payload)
+        except ValueError:
+            raise MalformedJWTError from None
+
+        # If we got here, the JWT is valid and filtered
+        return ".".join([header, payload, signature])
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_core_api.py` & `morningstar_data-1.3.0/morningstar_data/direct/_core_api.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-import time
-from math import isnan
-import requests
-import polling2
-from ._config import _Config
-from typing import Any, Dict, Optional, Union
-from ._exceptions import ApiRequestException, ApiResponseException, InternalServerError
-from ..direct._error_messages import INTERNAL_SERVER_ERROR
-from .._base import _logger
-from tenacity import retry, stop_after_attempt, wait_exponential
-from ._utils import get_bytes
-from .._version import __version__
-import uuid
-
-
-_config = _Config()
-
-POLL_STEP = 1  # seconds
-POLL_TIMEOUT = 900  # seconds (15 minutes)
-HEADER_STATUS = "proxy_response_status"
-
-
-def get_poll_step_from_headers(headers: Dict[str, Any]) -> int:
-    return int(headers["POLL_STEP"]) if "POLL_STEP" in headers else POLL_STEP
-
-
-def get_poll_timeout_from_headers(headers: Dict[str, Any]) -> int:
-    return int(headers["POLL_TIMEOUT"]) if "POLL_TIMEOUT" in headers else POLL_TIMEOUT
-
-
-def is_task_complete(response: Any) -> bool:
-    if "proxy_response_status" not in response.headers:
-        return False
-    if response.headers["proxy_response_status"].upper() == "SUCCESS" or response.headers["proxy_response_status"].upper() == "FAILURE":
-        return True
-    else:
-        return False
-
-
-@retry(reraise=True, stop=stop_after_attempt(8), wait=wait_exponential(multiplier=2, min=1, max=120))  # type: ignore
-def request_with_retry(method: str, url: str, headers: Dict[str, Any], verify: bool, data: Optional[Union[Dict[Any, Any], str]] = None) -> requests.Response:
-
-    STATUS_FORCE_LIST = [500, 501, 502, 503, 504]
-    MAX_REDIRECTS = 5
-    REDIRECT_CODES = [301, 307]
-    try:
-        res = requests.request(method, url, headers=headers, verify=verify, data=data, allow_redirects=False)
-
-        redirect_count = 0
-
-        while res.status_code in REDIRECT_CODES and redirect_count <= MAX_REDIRECTS:
-
-            redirected_url = res.headers["Location"]
-            _logger.info(f"Redirection to {redirected_url} for {method} request to {url}")
-
-            res = requests.request(method, redirected_url, headers=headers, verify=verify, data=data, allow_redirects=False)
-
-            redirect_count += 1
-
-    except Exception as e:
-        _logger.error(f"Retry Error: Exception making request. method: {method},url: {url},headers: {headers} , error: {e}")
-        if "proxy_request" in url:
-            raise ApiRequestException(f"Failed connecting to {url}, error: {e}")
-        else:
-            raise ApiResponseException(f"Failed connecting to {url}, error: {e}")
-
-    if res.status_code in STATUS_FORCE_LIST:
-        # Build a message from the response if we can
-        try:
-            res_json = res.json()
-        except requests.JSONDecodeError:
-            raise InternalServerError(f"{INTERNAL_SERVER_ERROR}. Got status code: {res.status_code} for method: {method} to {url}.")
-
-        error_msg = f"{INTERNAL_SERVER_ERROR}. Got status code: {res.status_code} for method: {method} to {url}."
-
-        try:
-            hint = res_json["_meta"]["hint"]
-            error_msg = error_msg + f" hint: {hint}"
-        except KeyError:
-            pass
-
-        try:
-            message = res_json["message"]
-            error_msg = error_msg + f" message: {message}"
-        except KeyError:
-            pass
-
-        raise InternalServerError(error_msg)
-
-    return res
-
-
-# This function checks whether the response from a function is a presigned URL, and if it is, it downloads the content from that URL and returns the response object.
-# If the response is not a presigned URL, it returns the response object.
-def download_if_signed_url(response: requests.Response) -> requests.Response:
-    if response.headers.get("download_presigned_url") == "True":
-        download_url = response.content
-        _logger.info(f"Downloading from s3 at the url {download_url}")
-        res_s3_byte_object = get_bytes(download_url)
-        # Note that _content is a private attribute, so we should not normally modify it. However, in this case, we need to modify it to change the value of the content attribute.
-        response._content = res_s3_byte_object.content
-        return response
-    else:
-        return response
-
-
-def make_request(method: str, url: str, headers: Dict[str, Any], verify: bool, data: Optional[Union[Dict[Any, Any], str]] = None) -> requests.Response:
-    request_id = None
-    poll_step = POLL_STEP
-    poll_timeout = POLL_TIMEOUT
-    try:
-        _logger.info("Queueing request")
-        _logger.debug(f"Queueing request: {method} {url}")
-        request_uuid = str(uuid.uuid4())
-        headers["X-API-RequestId"] = request_uuid
-        headers["md-package-version"] = __version__
-        _logger.debug(f"Updated Request ID: {request_uuid}")
-
-        res = request_with_retry(method, url, headers=headers, verify=verify, data=data)
-        res.raise_for_status()
-
-        _logger.info("Got valid response from queueing request")
-        _logger.debug(f"Got {res.status_code} response from queueing request.")
-
-        _logger.debug(f"Response headers: {res.headers}")
-
-        proxy_status = res.headers[HEADER_STATUS].upper()
-        if proxy_status == "SUCCESS":
-            _logger.debug("Request is already completed. Returning the response.")
-            return res
-        elif proxy_status == "QUEUED":
-            _logger.debug("Request is still queued. Getting the request id")
-            request_id = res.json()["id"]
-            _logger.debug(f"Client Request ID {request_uuid}. MD-API Task ID {request_id}")
-            _logger.info(f"Request id is {request_id}")
-            poll_step = get_poll_step_from_headers(res.headers)
-            poll_timeout = get_poll_timeout_from_headers(res.headers)
-
-    except requests.ConnectionError as e:
-        _logger.error(repr(e))
-        raise ApiRequestException(f"Failed connecting to {url}")
-    except requests.HTTPError as e:
-        # If the request is already completed, return the response.
-        # The response is considered successful if the proxy_response_status in the header is "completed"
-        # Every response from MD API has a proxy_response_status header
-        _logger.info("Got HTTPError from queueing request")
-        # Access the value of "proxy_response_status" in res.headers dictionary, with a default value of an empty string ("") if the key is not found
-        # if res.headers.get("proxy_response_status", "").upper() == "SUCCESS":
-        #     _logger.debug("Request is already completed. Returning the response.")
-        #     return res
-
-        _logger.error(repr(e))
-        # raise ApiRequestException(f"Failed queueing the request. Got {res.status_code}")
-        raise ApiRequestException(f"Failed queueing the request.")
-
-    response_url = f"{_config._MD_API}proxy_response/{request_id}"
-    _logger.debug(f"Response URL is {response_url}")
-
-    # Poll the response URL until the request is completed
-    # Return the response object as it is as exception handling is done in the calling function
-    # Response is considered successful if the proxy_response_status in the header is "completed"
-
-    # time.sleep(5)
-
-    # return requests.get(response_url, headers=headers, verify=verify)
-
-    response = polling2.poll(
-        lambda: request_with_retry("GET", response_url, headers=headers, verify=verify),
-        step=poll_step,
-        timeout=poll_timeout,
-        check_success=lambda response: is_task_complete(response),
-    )
-    return download_if_signed_url(response=response)
+import time
+from math import isnan
+import requests
+import polling2
+from ._config import _Config
+from typing import Any, Dict, Optional, Union
+from ._exceptions import ApiRequestException, ApiResponseException, InternalServerError
+from ..direct._error_messages import INTERNAL_SERVER_ERROR
+from .._base import _logger
+from tenacity import retry, stop_after_attempt, wait_exponential
+from ._utils import get_bytes
+from .._version import __version__
+import uuid
+
+
+_config = _Config()
+
+POLL_STEP = 1  # seconds
+POLL_TIMEOUT = 900  # seconds (15 minutes)
+HEADER_STATUS = "proxy_response_status"
+
+
+def get_poll_step_from_headers(headers: Dict[str, Any]) -> int:
+    return int(headers["POLL_STEP"]) if "POLL_STEP" in headers else POLL_STEP
+
+
+def get_poll_timeout_from_headers(headers: Dict[str, Any]) -> int:
+    return int(headers["POLL_TIMEOUT"]) if "POLL_TIMEOUT" in headers else POLL_TIMEOUT
+
+
+def is_task_complete(response: Any) -> bool:
+    if "proxy_response_status" not in response.headers:
+        return False
+    if response.headers["proxy_response_status"].upper() == "SUCCESS" or response.headers["proxy_response_status"].upper() == "FAILURE":
+        return True
+    else:
+        return False
+
+
+@retry(reraise=True, stop=stop_after_attempt(8), wait=wait_exponential(multiplier=2, min=1, max=120))  # type: ignore
+def request_with_retry(method: str, url: str, headers: Dict[str, Any], verify: bool, data: Optional[Union[Dict[Any, Any], str]] = None) -> requests.Response:
+
+    STATUS_FORCE_LIST = [500, 501, 502, 503, 504]
+    MAX_REDIRECTS = 5
+    REDIRECT_CODES = [301, 307]
+    try:
+        res = requests.request(method, url, headers=headers, verify=verify, data=data, allow_redirects=False)
+
+        redirect_count = 0
+
+        while res.status_code in REDIRECT_CODES and redirect_count <= MAX_REDIRECTS:
+
+            redirected_url = res.headers["Location"]
+            _logger.info(f"Redirection to {redirected_url} for {method} request to {url}")
+
+            res = requests.request(method, redirected_url, headers=headers, verify=verify, data=data, allow_redirects=False)
+
+            redirect_count += 1
+
+    except Exception as e:
+        _logger.error(f"Retry Error: Exception making request. method: {method},url: {url},headers: {headers} , error: {e}")
+        if "proxy_request" in url:
+            raise ApiRequestException(f"Failed connecting to {url}, error: {e}")
+        else:
+            raise ApiResponseException(f"Failed connecting to {url}, error: {e}")
+
+    if res.status_code in STATUS_FORCE_LIST:
+        # Build a message from the response if we can
+        try:
+            res_json = res.json()
+        except requests.JSONDecodeError:
+            raise InternalServerError(f"{INTERNAL_SERVER_ERROR}. Got status code: {res.status_code} for method: {method} to {url}.")
+
+        error_msg = f"{INTERNAL_SERVER_ERROR}. Got status code: {res.status_code} for method: {method} to {url}."
+
+        try:
+            hint = res_json["_meta"]["hint"]
+            error_msg = error_msg + f" hint: {hint}"
+        except KeyError:
+            pass
+
+        try:
+            message = res_json["message"]
+            error_msg = error_msg + f" message: {message}"
+        except KeyError:
+            pass
+
+        raise InternalServerError(error_msg)
+
+    return res
+
+
+# This function checks whether the response from a function is a presigned URL, and if it is, it downloads the content from that URL and returns the response object.
+# If the response is not a presigned URL, it returns the response object.
+def download_if_signed_url(response: requests.Response) -> requests.Response:
+    if response.headers.get("download_presigned_url") == "True":
+        download_url = response.content
+        _logger.info(f"Downloading from s3 at the url {download_url}")
+        res_s3_byte_object = get_bytes(download_url)
+        # Note that _content is a private attribute, so we should not normally modify it. However, in this case, we need to modify it to change the value of the content attribute.
+        response._content = res_s3_byte_object.content
+        return response
+    else:
+        return response
+
+
+def make_request(method: str, url: str, headers: Dict[str, Any], verify: bool, data: Optional[Union[Dict[Any, Any], str]] = None) -> requests.Response:
+    request_id = None
+    poll_step = POLL_STEP
+    poll_timeout = POLL_TIMEOUT
+    try:
+        _logger.info("Queueing request")
+        _logger.debug(f"Queueing request: {method} {url}")
+        request_uuid = str(uuid.uuid4())
+        headers["X-API-RequestId"] = request_uuid
+        headers["md-package-version"] = __version__
+        _logger.debug(f"Updated Request ID: {request_uuid}")
+
+        res = request_with_retry(method, url, headers=headers, verify=verify, data=data)
+        res.raise_for_status()
+
+        _logger.info("Got valid response from queueing request")
+        _logger.debug(f"Got {res.status_code} response from queueing request.")
+
+        _logger.debug(f"Response headers: {res.headers}")
+
+        proxy_status = res.headers[HEADER_STATUS].upper()
+        if proxy_status == "SUCCESS":
+            _logger.debug("Request is already completed. Returning the response.")
+            return res
+        elif proxy_status == "QUEUED":
+            _logger.debug("Request is still queued. Getting the request id")
+            request_id = res.json()["id"]
+            _logger.debug(f"Client Request ID {request_uuid}. MD-API Task ID {request_id}")
+            _logger.info(f"Request id is {request_id}")
+            poll_step = get_poll_step_from_headers(res.headers)
+            poll_timeout = get_poll_timeout_from_headers(res.headers)
+
+    except requests.ConnectionError as e:
+        _logger.error(repr(e))
+        raise ApiRequestException(f"Failed connecting to {url}")
+    except requests.HTTPError as e:
+        # If the request is already completed, return the response.
+        # The response is considered successful if the proxy_response_status in the header is "completed"
+        # Every response from MD API has a proxy_response_status header
+        _logger.info("Got HTTPError from queueing request")
+        # Access the value of "proxy_response_status" in res.headers dictionary, with a default value of an empty string ("") if the key is not found
+        # if res.headers.get("proxy_response_status", "").upper() == "SUCCESS":
+        #     _logger.debug("Request is already completed. Returning the response.")
+        #     return res
+
+        _logger.error(repr(e))
+        # raise ApiRequestException(f"Failed queueing the request. Got {res.status_code}")
+        raise ApiRequestException(f"Failed queueing the request.")
+
+    response_url = f"{_config._MD_API}proxy_response/{request_id}"
+    _logger.debug(f"Response URL is {response_url}")
+
+    # Poll the response URL until the request is completed
+    # Return the response object as it is as exception handling is done in the calling function
+    # Response is considered successful if the proxy_response_status in the header is "completed"
+
+    # time.sleep(5)
+
+    # return requests.get(response_url, headers=headers, verify=verify)
+
+    response = polling2.poll(
+        lambda: request_with_retry("GET", response_url, headers=headers, verify=verify),
+        step=poll_step,
+        timeout=poll_timeout,
+        check_success=lambda response: is_task_complete(response),
+    )
+    return download_if_signed_url(response=response)
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_data_objects/_custom_data_points_types.py` & `morningstar_data-1.3.0/morningstar_data/direct/_data_objects/_custom_data_points_types.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,68 @@
-import re
-
-from datetime import datetime
-from typing import Union, Callable
-
-from .._exceptions import ValueErrorException
-
-
-TypeValue = Union[str, int, float, None]
-
-
-class ValidCustomDataPointTypes:
-    def __init__(self, data_point_definition: dict):
-        function_name = re.sub(r"(?<!^)(?=[A-Z])", "_", data_point_definition["columnType"]).lower()
-        self.is_valid: Callable = getattr(ValidCustomDataPointTypes, function_name, self.raise_value_error)
-
-    def raise_value_error(self, val: TypeValue) -> None:
-        raise ValueErrorException("Column type is not supported.")
-
-    @staticmethod
-    def extended_text(val: TypeValue) -> TypeValue:
-        if isinstance(val, str) and len(val) <= 250:
-            return val
-        raise ValueErrorException("Only allows a string data type with 250 characters or less")
-
-    @staticmethod
-    def numeric(val: TypeValue) -> TypeValue:
-        if isinstance(val, int) or isinstance(val, float):
-            return val
-        raise ValueErrorException("Only allows numbers")
-
-    @staticmethod
-    def free_text(val: TypeValue) -> TypeValue:
-        if isinstance(val, str) and len(val) <= 50:
-            return val
-        raise ValueErrorException("Only allows a string data type with 50 characters or less")
-
-    @staticmethod
-    def date(val: TypeValue) -> TypeValue:
-        format_Data = "%Y-%m-%d"
-        if isinstance(val, str):
-            datetime.strptime(val, format_Data)
-            return val
-        raise ValueErrorException("Only allows Date data type with the format yyyy-mm-dd")
-
-    @staticmethod
-    def category(val: TypeValue) -> TypeValue:
-        return ValidCustomDataPointTypes.free_text(val)
-
-    @staticmethod
-    def indicator(val: TypeValue) -> TypeValue:
-        return ValidCustomDataPointTypes.numeric(val)
-
-    @staticmethod
-    def t_s_return(val: TypeValue) -> TypeValue:
-        return ValidCustomDataPointTypes.numeric(val)
-
-    @staticmethod
-    def t_s_price(val: TypeValue) -> TypeValue:
-        return ValidCustomDataPointTypes.numeric(val)
-
-    @staticmethod
-    def t_s_numeric(val: TypeValue) -> TypeValue:
-        return ValidCustomDataPointTypes.numeric(val)
-
-    @staticmethod
-    def t_s_free_text(val: TypeValue) -> TypeValue:
-        return ValidCustomDataPointTypes.free_text(val)
+import re
+
+from datetime import datetime
+from typing import Union, Callable
+
+from .._exceptions import ValueErrorException
+
+
+TypeValue = Union[str, int, float, None]
+
+
+class ValidCustomDataPointTypes:
+    def __init__(self, data_point_definition: dict):
+        function_name = re.sub(r"(?<!^)(?=[A-Z])", "_", data_point_definition["columnType"]).lower()
+        self.is_valid: Callable = getattr(ValidCustomDataPointTypes, function_name, self.raise_value_error)
+
+    def raise_value_error(self, val: TypeValue) -> None:
+        raise ValueErrorException("Column type is not supported.")
+
+    @staticmethod
+    def extended_text(val: TypeValue) -> TypeValue:
+        if isinstance(val, str) and len(val) <= 250:
+            return val
+        raise ValueErrorException("Only allows a string data type with 250 characters or less")
+
+    @staticmethod
+    def numeric(val: TypeValue) -> TypeValue:
+        if isinstance(val, int) or isinstance(val, float):
+            return val
+        raise ValueErrorException("Only allows numbers")
+
+    @staticmethod
+    def free_text(val: TypeValue) -> TypeValue:
+        if isinstance(val, str) and len(val) <= 50:
+            return val
+        raise ValueErrorException("Only allows a string data type with 50 characters or less")
+
+    @staticmethod
+    def date(val: TypeValue) -> TypeValue:
+        format_Data = "%Y-%m-%d"
+        if isinstance(val, str):
+            datetime.strptime(val, format_Data)
+            return val
+        raise ValueErrorException("Only allows Date data type with the format yyyy-mm-dd")
+
+    @staticmethod
+    def category(val: TypeValue) -> TypeValue:
+        return ValidCustomDataPointTypes.free_text(val)
+
+    @staticmethod
+    def indicator(val: TypeValue) -> TypeValue:
+        return ValidCustomDataPointTypes.numeric(val)
+
+    @staticmethod
+    def t_s_return(val: TypeValue) -> TypeValue:
+        return ValidCustomDataPointTypes.numeric(val)
+
+    @staticmethod
+    def t_s_price(val: TypeValue) -> TypeValue:
+        return ValidCustomDataPointTypes.numeric(val)
+
+    @staticmethod
+    def t_s_numeric(val: TypeValue) -> TypeValue:
+        return ValidCustomDataPointTypes.numeric(val)
+
+    @staticmethod
+    def t_s_free_text(val: TypeValue) -> TypeValue:
+        return ValidCustomDataPointTypes.free_text(val)
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_data_objects/_data_points_object.py` & `morningstar_data-1.3.0/morningstar_data/direct/_data_objects/_data_points_object.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_data_objects/_investments_object.py` & `morningstar_data-1.3.0/morningstar_data/direct/_data_objects/_investments_object.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,169 +1,169 @@
-import functools
-import requests
-
-from uuid import UUID
-from typing import Union, List, Any, Dict, Optional, Callable
-from .._api import _direct_api_request
-from .._config import _Config
-from .._exceptions import BadRequestException, ResourceNotFoundError
-from .. import _error_messages
-from ..._base import _logger
-from ..user_items.search_criteria import execute_search
-from .._error_messages import (
-    BAD_REQUEST_ERROR_INVALID_CATEGORY_ID,
-    BAD_REQUEST_ERROR_NO_INVESTMENT_SOURCE,
-)
-
-
-
-_config = _Config()
-
-SearchObjectType = Optional[Dict[str, Any]]
-InvestmentsListType = Optional[List[str]]
-UUIDOrInitType = Optional[str]
-InvestmentType = Union[SearchObjectType, UUIDOrInitType, InvestmentsListType]
-CategoryType = Optional[str]
-
-
-class Investments:
-    def __init__(self, investment_object: InvestmentType) -> None:
-        self.investment_ids: InvestmentsListType = None
-        self.search_criteria: UUIDOrInitType = None
-        self.list_id: UUIDOrInitType = None
-        self.search_criteria_object: SearchObjectType = None
-        self.category_id: CategoryType = None
-        self._parse_investment_object(investment_object)
-
-    def _parse_investment_object(self, investment_object: InvestmentType) -> None:
-        if isinstance(investment_object, list):
-            self.investment_ids = investment_object
-        elif isinstance(investment_object, dict):
-            self.search_criteria_object = investment_object
-        elif self._is_int(investment_object):
-            self.search_criteria = investment_object
-        elif self._is_guid(investment_object):
-            self.list_id = investment_object
-        elif isinstance(investment_object, str) and investment_object is not None and len(investment_object.strip()) > 0:
-            self.category_id = investment_object
-        else:
-            raise ValueError("Invalid investment object")
-
-    def _is_int(self, value: InvestmentType) -> bool:
-        try:
-            if not isinstance(value, str):
-                raise ValueError("Invalid investment object: search criteria must be a string")
-            int(value)
-            return True
-        except ValueError:
-            return False
-
-    def _is_guid(self, value: InvestmentType) -> bool:
-        try:
-            if not isinstance(value, str):
-                raise ValueError("Invalid investment object: list ID must be a string")
-            UUID(value)
-            return True
-        except ValueError:
-            return False
-
-    @functools.lru_cache()
-    def get_investment_ids(self) -> list:
-        id_list = []
-        if self.investment_ids:
-            id_list = self.investment_ids
-
-        elif self.list_id is not None and len(self.list_id.strip()) > 0:
-            id_list = self._get_investment_ids_by_list_id()
-            if not id_list:
-                raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_INVESTMENT_DATA_LIST_ID)
-
-        elif self.search_criteria is not None and len(self.search_criteria.strip()) > 0:
-            id_list = self._get_investment_ids_by_search_id()
-            if not id_list:
-                raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_INVESTMENT_DATA_SEARCH_CRITERIA_ID)
-
-        elif self.search_criteria_object:
-            id_list = self._get_investments_by_search_criteria_object()
-            if not id_list:
-                raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_INVESTMENT_DATA_SEARCH_CRITERIA_CONDITION)
-
-        return id_list
-
-    def _get_investment_ids_by_list_id(self) -> list:
-        investment_list_dict = self._get_investment_list()
-        investment_id_list = investment_list_dict.get("idList", []) if investment_list_dict is not None else []
-        investment_ids = []
-        if investment_id_list:
-            investment_ids = list(map(lambda x: self._concat_id_and_type(x), investment_id_list))
-        return investment_ids
-
-    def _get_investment_ids_by_search_id(self) -> list:
-        investment_list = self._get_investments_by_search_id()
-        investment_ids = []
-        if investment_list:
-            mapper: Callable[[Dict[str, Any]], Any] = lambda x: x.get("id", "")
-            investment_ids = list(map(mapper, investment_list))
-        return investment_ids
-
-    def _get_investment_list(self) -> Dict[str, Any]:
-        # sourcetype should be "Desktop" to retrieve secids for list items
-        # The alternative is "Cloud", which retrieves performanceids.
-        # We need secids for joining with Datalake tables
-        url = f"{_config.object_service_url()}objectapi/v1/lists/{self.list_id}?sourcetype=Desktop"
-        response_json: Dict[str, Any] = _direct_api_request("GET", url)
-
-        investment_list: List[Dict[str, Any]] = response_json.get("lists", [])
-        if len(investment_list) > 0:
-            return investment_list[0]
-        return dict()
-
-    def _get_investments_by_search_id(self) -> list:
-        url = f"{_config.searches_service_url()}v1/searches/{self.search_criteria}"
-        response_json = _direct_api_request("GET", url)
-        search_criteria = response_json.get("content", dict())
-        if len(search_criteria) > 0:
-            search_result: list = execute_search(search_criteria)
-            return search_result
-        return []
-
-    def _get_investments_by_search_criteria_object(self) -> list:
-        if self.search_criteria_object is not None and len(self.search_criteria_object) > 0:
-            if "universeId" not in self.search_criteria_object.keys() or self.search_criteria_object["universeId"] == "":
-                raise BadRequestException("'universeId' is a required property in the search criteria object.")
-            if "criteria" not in self.search_criteria_object.keys() or self.search_criteria_object["criteria"] == []:
-                raise BadRequestException("'criteria' is a required property in the search criteria object.")
-            investment_data = execute_search(self.search_criteria_object)
-            return [investmentId["id"] for investmentId in investment_data if "id" in investmentId.keys()]
-        return []
-
-    def _concat_id_and_type(self, investment: dict) -> str:
-        investment_id = investment.get("id", "").strip()
-        investment_type = investment.get("3xType")
-        investment_type = investment_type.strip() if investment_type is not None else ""
-
-        return f"{investment_id};{investment_type}" if len(investment_type) > 0 else f"{investment_id}"
-
-    def generate_investment_source(self) -> dict:
-        investment_source = {}
-        if self.category_id is not None and len(self.category_id.strip()) > 0:
-            if ";" not in self.category_id:
-                raise BadRequestException(BAD_REQUEST_ERROR_INVALID_CATEGORY_ID)
-            investment_source["type"] = "MORNINGSTAR_CATEGORY"
-            investment_source["id"] = self.category_id
-
-        elif self.investment_ids:
-            investment_source["type"] = "SECIDS"
-            investment_source["id"] = ",".join(self.investment_ids)
-
-        elif self.list_id is not None and len(self.list_id.strip()) > 0:
-            investment_source["type"] = "LIST"
-            investment_source["id"] = self.list_id
-
-        elif self.search_criteria is not None and len(self.search_criteria.strip()) > 0:
-            investment_source["type"] = "SEARCH"
-            investment_source["id"] = self.search_criteria
-
-        if not investment_source:
-            raise BadRequestException(BAD_REQUEST_ERROR_NO_INVESTMENT_SOURCE)
-
-        return investment_source
+import functools
+import requests
+
+from uuid import UUID
+from typing import Union, List, Any, Dict, Optional, Callable
+from .._api import _direct_api_request
+from .._config import _Config
+from .._exceptions import BadRequestException, ResourceNotFoundError
+from .. import _error_messages
+from ..._base import _logger
+from ..user_items.search_criteria import execute_search
+from .._error_messages import (
+    BAD_REQUEST_ERROR_INVALID_CATEGORY_ID,
+    BAD_REQUEST_ERROR_NO_INVESTMENT_SOURCE,
+)
+
+
+
+_config = _Config()
+
+SearchObjectType = Optional[Dict[str, Any]]
+InvestmentsListType = Optional[List[str]]
+UUIDOrInitType = Optional[str]
+InvestmentType = Union[SearchObjectType, UUIDOrInitType, InvestmentsListType]
+CategoryType = Optional[str]
+
+
+class Investments:
+    def __init__(self, investment_object: InvestmentType) -> None:
+        self.investment_ids: InvestmentsListType = None
+        self.search_criteria: UUIDOrInitType = None
+        self.list_id: UUIDOrInitType = None
+        self.search_criteria_object: SearchObjectType = None
+        self.category_id: CategoryType = None
+        self._parse_investment_object(investment_object)
+
+    def _parse_investment_object(self, investment_object: InvestmentType) -> None:
+        if isinstance(investment_object, list):
+            self.investment_ids = investment_object
+        elif isinstance(investment_object, dict):
+            self.search_criteria_object = investment_object
+        elif self._is_int(investment_object):
+            self.search_criteria = investment_object
+        elif self._is_guid(investment_object):
+            self.list_id = investment_object
+        elif isinstance(investment_object, str) and investment_object is not None and len(investment_object.strip()) > 0:
+            self.category_id = investment_object
+        else:
+            raise ValueError("Invalid investment object")
+
+    def _is_int(self, value: InvestmentType) -> bool:
+        try:
+            if not isinstance(value, str):
+                raise ValueError("Invalid investment object: search criteria must be a string")
+            int(value)
+            return True
+        except ValueError:
+            return False
+
+    def _is_guid(self, value: InvestmentType) -> bool:
+        try:
+            if not isinstance(value, str):
+                raise ValueError("Invalid investment object: list ID must be a string")
+            UUID(value)
+            return True
+        except ValueError:
+            return False
+
+    @functools.lru_cache()
+    def get_investment_ids(self) -> list:
+        id_list = []
+        if self.investment_ids:
+            id_list = self.investment_ids
+
+        elif self.list_id is not None and len(self.list_id.strip()) > 0:
+            id_list = self._get_investment_ids_by_list_id()
+            if not id_list:
+                raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_INVESTMENT_DATA_LIST_ID)
+
+        elif self.search_criteria is not None and len(self.search_criteria.strip()) > 0:
+            id_list = self._get_investment_ids_by_search_id()
+            if not id_list:
+                raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_INVESTMENT_DATA_SEARCH_CRITERIA_ID)
+
+        elif self.search_criteria_object:
+            id_list = self._get_investments_by_search_criteria_object()
+            if not id_list:
+                raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_INVESTMENT_DATA_SEARCH_CRITERIA_CONDITION)
+
+        return id_list
+
+    def _get_investment_ids_by_list_id(self) -> list:
+        investment_list_dict = self._get_investment_list()
+        investment_id_list = investment_list_dict.get("idList", []) if investment_list_dict is not None else []
+        investment_ids = []
+        if investment_id_list:
+            investment_ids = list(map(lambda x: self._concat_id_and_type(x), investment_id_list))
+        return investment_ids
+
+    def _get_investment_ids_by_search_id(self) -> list:
+        investment_list = self._get_investments_by_search_id()
+        investment_ids = []
+        if investment_list:
+            mapper: Callable[[Dict[str, Any]], Any] = lambda x: x.get("id", "")
+            investment_ids = list(map(mapper, investment_list))
+        return investment_ids
+
+    def _get_investment_list(self) -> Dict[str, Any]:
+        # sourcetype should be "Desktop" to retrieve secids for list items
+        # The alternative is "Cloud", which retrieves performanceids.
+        # We need secids for joining with Datalake tables
+        url = f"{_config.object_service_url()}objectapi/v1/lists/{self.list_id}?sourcetype=Desktop"
+        response_json: Dict[str, Any] = _direct_api_request("GET", url)
+
+        investment_list: List[Dict[str, Any]] = response_json.get("lists", [])
+        if len(investment_list) > 0:
+            return investment_list[0]
+        return dict()
+
+    def _get_investments_by_search_id(self) -> list:
+        url = f"{_config.searches_service_url()}v1/searches/{self.search_criteria}"
+        response_json = _direct_api_request("GET", url)
+        search_criteria = response_json.get("content", dict())
+        if len(search_criteria) > 0:
+            search_result: list = execute_search(search_criteria)
+            return search_result
+        return []
+
+    def _get_investments_by_search_criteria_object(self) -> list:
+        if self.search_criteria_object is not None and len(self.search_criteria_object) > 0:
+            if "universeId" not in self.search_criteria_object.keys() or self.search_criteria_object["universeId"] == "":
+                raise BadRequestException("'universeId' is a required property in the search criteria object.")
+            if "criteria" not in self.search_criteria_object.keys() or self.search_criteria_object["criteria"] == []:
+                raise BadRequestException("'criteria' is a required property in the search criteria object.")
+            investment_data = execute_search(self.search_criteria_object)
+            return [investmentId["id"] for investmentId in investment_data if "id" in investmentId.keys()]
+        return []
+
+    def _concat_id_and_type(self, investment: dict) -> str:
+        investment_id = investment.get("id", "").strip()
+        investment_type = investment.get("3xType")
+        investment_type = investment_type.strip() if investment_type is not None else ""
+
+        return f"{investment_id};{investment_type}" if len(investment_type) > 0 else f"{investment_id}"
+
+    def generate_investment_source(self) -> dict:
+        investment_source = {}
+        if self.category_id is not None and len(self.category_id.strip()) > 0:
+            if ";" not in self.category_id:
+                raise BadRequestException(BAD_REQUEST_ERROR_INVALID_CATEGORY_ID)
+            investment_source["type"] = "MORNINGSTAR_CATEGORY"
+            investment_source["id"] = self.category_id
+
+        elif self.investment_ids:
+            investment_source["type"] = "SECIDS"
+            investment_source["id"] = ",".join(self.investment_ids)
+
+        elif self.list_id is not None and len(self.list_id.strip()) > 0:
+            investment_source["type"] = "LIST"
+            investment_source["id"] = self.list_id
+
+        elif self.search_criteria is not None and len(self.search_criteria.strip()) > 0:
+            investment_source["type"] = "SEARCH"
+            investment_source["id"] = self.search_criteria
+
+        if not investment_source:
+            raise BadRequestException(BAD_REQUEST_ERROR_NO_INVESTMENT_SOURCE)
+
+        return investment_source
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_data_point.py` & `morningstar_data-1.3.0/morningstar_data/direct/_data_point.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-import simplejson as json
-
-from pandas import DataFrame
-from typing import List, Dict, Any
-
-from . import _decorator
-from .._base import _logger
-from ._exceptions import ValueErrorException
-from ._api import _direct_api_request
-from ._config import _Config
-
-_config = _Config()
-
-
-def _data_point_request_builder(data_point_details: list) -> List[Any]:
-    if not data_point_details:
-        raise ValueErrorException("No datapoint available.")
-    url = f"{_config.data_point_service_url()}v1/datapoints/datapointrequestbuilder"
-    response_json: List[Any] = _direct_api_request("POST", url, json.dumps(data_point_details, ignore_nan=True))
-    return response_json
-
-
-def _request_asset_flow_data_points() -> List[Any]:
-    url = f"{_config.securitydata_service_url()}v1/assetflow/datapoints"
-    response_json: List[Any] = _direct_api_request("GET", url)
-    return response_json
-
-
-def _get_asset_flow_data_points_by_ids(data_point_ids: list) -> list:
-    response_json = _request_asset_flow_data_points()
-    result = []
-    if response_json and isinstance(response_json, list):
-        data_point_id_settings_dict = {x.get("datapointId", "").strip(): x for x in response_json if x is not None}
-        for data_point_id in data_point_ids:
-            settings = data_point_id_settings_dict.get(data_point_id)
-            if settings is not None:
-                settings = settings.copy()
-                settings["datapointName"] = settings.pop("name")
-                settings["alias"] = settings["datapointName"]
-                result.append(settings)
-    return result
-
-
-@_decorator.error_handler
-def _get_data_point_details(params: list) -> List[Dict[Any, Any]]:
-    url = f"{_config.data_point_service_url()}v1/datapoints/detail"
-    response_json: List[Dict[Any, Any]] = _direct_api_request("POST", url, json.dumps(params, ignore_nan=True))
-    data_point_id_list = [
-        "OS010",
-        "OS01Z",
-        "OS245",
-    ]  # This is a temporary list of faulty data points. These datapoints will be removed in the future after which we wont have to specifically check for these data points.
-    filtered_json_response: List[Dict[Any, Any]] = list(
-        filter(lambda x: x.get("canBeAddedToDataset", False) or x["datapointId"] in data_point_id_list, response_json)
-    )
-    return filtered_json_response
-
-
-@_decorator.error_handler
-def _get_all_universes() -> DataFrame:
-    url = f"{_config.data_point_service_url()}v1/universes"
-    response_json = _direct_api_request("GET", url)
-    result = DataFrame(response_json)
-    return result[["id", "name"]]
+import simplejson as json
+
+from pandas import DataFrame
+from typing import List, Dict, Any
+
+from . import _decorator
+from .._base import _logger
+from ._exceptions import ValueErrorException
+from ._api import _direct_api_request
+from ._config import _Config
+
+_config = _Config()
+
+
+def _data_point_request_builder(data_point_details: list) -> List[Any]:
+    if not data_point_details:
+        raise ValueErrorException("No datapoint available.")
+    url = f"{_config.data_point_service_url()}v1/datapoints/datapointrequestbuilder"
+    response_json: List[Any] = _direct_api_request("POST", url, json.dumps(data_point_details, ignore_nan=True))
+    return response_json
+
+
+def _request_asset_flow_data_points() -> List[Any]:
+    url = f"{_config.securitydata_service_url()}v1/assetflow/datapoints"
+    response_json: List[Any] = _direct_api_request("GET", url)
+    return response_json
+
+
+def _get_asset_flow_data_points_by_ids(data_point_ids: list) -> list:
+    response_json = _request_asset_flow_data_points()
+    result = []
+    if response_json and isinstance(response_json, list):
+        data_point_id_settings_dict = {x.get("datapointId", "").strip(): x for x in response_json if x is not None}
+        for data_point_id in data_point_ids:
+            settings = data_point_id_settings_dict.get(data_point_id)
+            if settings is not None:
+                settings = settings.copy()
+                settings["datapointName"] = settings.pop("name")
+                settings["alias"] = settings["datapointName"]
+                result.append(settings)
+    return result
+
+
+@_decorator.error_handler
+def _get_data_point_details(params: list) -> List[Dict[Any, Any]]:
+    url = f"{_config.data_point_service_url()}v1/datapoints/detail"
+    response_json: List[Dict[Any, Any]] = _direct_api_request("POST", url, json.dumps(params, ignore_nan=True))
+    data_point_id_list = [
+        "OS010",
+        "OS01Z",
+        "OS245",
+    ]  # This is a temporary list of faulty data points. These datapoints will be removed in the future after which we wont have to specifically check for these data points.
+    filtered_json_response: List[Dict[Any, Any]] = list(
+        filter(lambda x: x.get("canBeAddedToDataset", False) or x["datapointId"] in data_point_id_list, response_json)
+    )
+    return filtered_json_response
+
+
+@_decorator.error_handler
+def _get_all_universes() -> DataFrame:
+    url = f"{_config.data_point_service_url()}v1/universes"
+    response_json = _direct_api_request("GET", url)
+    result = DataFrame(response_json)
+    return result[["id", "name"]]
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_data_type.py` & `morningstar_data-1.3.0/morningstar_data/direct/_data_type.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import enum
-from enum import Enum
-from typing import Any
-from ._exceptions import BadRequestException
-
-
-class DatabaseCD(str, Enum):
-    user = ("UDP",)
-    firm = ("CDP",)
-
-
-class RaiseEnum(enum.EnumMeta):
-    def __getitem__(cls, name: str) -> Any:
-        try:
-            return super().__getitem__(name)
-        except KeyError:
-            options = ", ".join(cls._member_map_.keys())
-            raise BadRequestException(f"Please choose one of the following valid options: '{options}'.\n" f"'{name}' is an invalid choice.\n") from None
-
-
-class ErrorMessages(str, Enum):
-    date_format_error = "Please input the date in yyyy-MM-dd format."
-    start_date_require_error = "Please specify start_date to proceed with your query."
-    no_data_point_msg = "There is no data point available."
-    start_end_date_error = "Please specify start_date and end_date to proceed with your query."
-    frequency_error_msg = "Please specify frequency to proceed with your query."
-    currency_error_msg = "Please specify currency to proceed with your query."
+import enum
+from enum import Enum
+from typing import Any
+from ._exceptions import BadRequestException
+
+
+class DatabaseCD(str, Enum):
+    user = ("UDP",)
+    firm = ("CDP",)
+
+
+class RaiseEnum(enum.EnumMeta):
+    def __getitem__(cls, name: str) -> Any:
+        try:
+            return super().__getitem__(name)
+        except KeyError:
+            options = ", ".join(cls._member_map_.keys())
+            raise BadRequestException(f"Please choose one of the following valid options: '{options}'.\n" f"'{name}' is an invalid choice.\n") from None
+
+
+class ErrorMessages(str, Enum):
+    date_format_error = "Please input the date in yyyy-MM-dd format."
+    start_date_require_error = "Please specify start_date to proceed with your query."
+    no_data_point_msg = "There is no data point available."
+    start_end_date_error = "Please specify start_date and end_date to proceed with your query."
+    frequency_error_msg = "Please specify frequency to proceed with your query."
+    currency_error_msg = "Please specify currency to proceed with your query."
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_decorator.py` & `morningstar_data-1.3.0/morningstar_data/direct/_decorator.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-import sys
-import traceback
-import typeguard
-
-from .._utils import format_analytics_logs, get_log_flag
-from typing import Callable, Any, Dict
-from functools import wraps
-from ._exceptions import BadRequestException, ApiResponseException, QueryLimitException, ValueErrorException
-
-import inspect
-
-typechecked: Callable = typeguard.typechecked
-
-
-def not_null(func: Callable) -> Callable:
-    @wraps(func)
-    def wrapper(*args: Any, **kwargs: Any) -> Any:
-        for arg in args:
-            if not arg:
-                raise BadRequestException("Null or empty parameter is not allowed.")
-
-        return func(*args, **kwargs)
-
-    return wrapper
-
-
-def error_handler(func: Callable) -> Callable:
-    @wraps(func)
-    def wrapper(*args: Any, **kwargs: Any) -> Any:
-        try:
-            return func(*args, **kwargs)
-        except (BadRequestException, ValueErrorException) as e:
-            wrappers = [x.name for x in traceback.extract_stack() if x.name == "error_handler"]
-            if len(wrappers) > 1:
-                raise ValueErrorException(str(e)) from None
-            else:
-                sys.stderr.write(str(e))
-        except ApiResponseException as e:
-            if e.status_code == 404:
-                sys.stderr.write("Specified data not Found. ")
-            else:
-                raise ValueErrorException(str(e)) from None
-        except QueryLimitException as e:
-            # Some exceptions need to be propagated back to the caller as-is
-            raise
-        except Exception as e:
-            raise ValueErrorException(str(e)) from None
-
-    return wrapper
+import sys
+import traceback
+import typeguard
+
+from .._utils import format_analytics_logs, get_log_flag
+from typing import Callable, Any, Dict
+from functools import wraps
+from ._exceptions import BadRequestException, ApiResponseException, QueryLimitException, ValueErrorException
+
+import inspect
+
+typechecked: Callable = typeguard.typechecked
+
+
+def not_null(func: Callable) -> Callable:
+    @wraps(func)
+    def wrapper(*args: Any, **kwargs: Any) -> Any:
+        for arg in args:
+            if not arg:
+                raise BadRequestException("Null or empty parameter is not allowed.")
+
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
+def error_handler(func: Callable) -> Callable:
+    @wraps(func)
+    def wrapper(*args: Any, **kwargs: Any) -> Any:
+        try:
+            return func(*args, **kwargs)
+        except (BadRequestException, ValueErrorException) as e:
+            wrappers = [x.name for x in traceback.extract_stack() if x.name == "error_handler"]
+            if len(wrappers) > 1:
+                raise ValueErrorException(str(e)) from None
+            else:
+                sys.stderr.write(str(e))
+        except ApiResponseException as e:
+            if e.status_code == 404:
+                sys.stderr.write("Specified data not Found. ")
+            else:
+                raise ValueErrorException(str(e)) from None
+        except QueryLimitException as e:
+            # Some exceptions need to be propagated back to the caller as-is
+            raise
+        except Exception as e:
+            raise ValueErrorException(str(e)) from None
+
+    return wrapper
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_error_messages.py` & `morningstar_data-1.3.0/morningstar_data/direct/_error_messages.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-ACCESS_DENIED_ERROR = "Unauthorized request! Please login with valid credentials. For more information, please contact Analytics Lab support team at Morningstar."
-FORBIDDEN_ERROR = "Forbidden request! You do not have permission to access this resource. For more information, please contact Analytics Lab support team at Morningstar."
-NETWORK_ERROR = "Network connection error. Please check your internet connection."
-TIMEOUT_ERROR = "Request timed out. Please try again or contact support at morningstardirect@moringstar.com"
-BAD_REQUEST_ERROR = "Bad request! Server could not process your request at this time. This error can occur due to multiple reasons (for example; bad request syntax, invalid message structure/framing, or incorrect/corrupt request).\nPlease refer morningstar data package documentation to make a valid request: https://docs-analyticslab.morningstar.com/latest/morningstar_data.html"
-CLIENT_ERROR = "Bad request! Server could not process your request at this time. This error can occur due to multiple reasons (for example; bad request syntax, invalid message structure/framing, or incorrect/corrupt request).\nPlease refer morningstar data package documentation to make a valid request: https://docs-analyticslab.morningstar.com/latest/morningstar_data.html"
-INTERNAL_SERVER_ERROR = (
-    "Something went wrong on our side!  For more details, please contact Analytics Lab support team at Morningstar. We apologize for any inconvenience this may have caused"
-)
-
-# Add query limit error messages here
-QUERY_LIMIT_ERROR = "You have reached your daily query limit. Please fill out this form for further assistance: https://go.morningstar.com/LP=6390"
-QUERY_LIMIT_ERROR_SHOW_LIMIT = "You have reached your daily query limit of $query cells. Please fill out this form for further assistance: https://go.morningstar.com/LP=6808"
-
-# AMS Flagged Features
-DELIVERY_ACCESS_ERROR = "You don't have access to this feature. Please fill out this form for further assistance: https://go.morningstar.com/LP=6809"
-
-# Add custom bad request error messages here
-BAD_REQUEST_ERROR_NO_START_AND_END_DATE = "Specify `start_date` and `end_date` to proceed with your query."
-BAD_REQUEST_ERROR_NO_END_DATE = "Specify the `end_date` to proceed with your query."
-BAD_REQUEST_ERROR_NO_START_DATE = "Specify the `start_date` to proceed with your query."
-BAD_REQUEST_ERROR_INCLUDE_ALL_DATE = "Specify either date or both start date and end date to proceed with your query."
-BAD_REQUEST_ERROR_INVALID_DATE_FORMAT = "Specify date in the format yyyy-MM-dd to proceed with your query."
-BAD_REQUEST_ERROR_NO_INVESTMENT_IDS = "Specify the `investment_ids` to proceed with your query."
-BAD_REQUEST_ERROR_NO_PORTFOLIO_DATA = "No matching portfolio data for the given date or date range."
-BAD_REQUEST_ERROR_INVALID_INVESTMENT_ID = "One or more ID's, in the provided list of `investment_ids`, are invalid!"
-BAD_REQUEST_ERROR_INVALID_INVESTMENT_LIST_ID = "Specify the valid `list_id` to proceed with your query. A `list_id` is a global unique identifier i.e. uuid."
-BAD_REQUEST_ERROR_INVALID_PORTFOLIO_ID = "Specify the valid `portfolio_id` to proceed with your query. A `portfolio_id` is a global unique identifier i.e. uuid."
-BAD_REQUEST_ERROR_INVALID_LOOKTHROUGH_HOLDING_TYPE = "Indexes are not supported as a valid Look-Through holding."
-BAD_REQUEST_ERROR_NO_START_AND_END_DATE = "Please specify `start_date` and `end_date` to proceed with your query."
-BAD_REQUEST_ERROR_NO_END_DATE = "Please specify the `end_date` to proceed with your query."
-BAD_REQUEST_ERROR_DATA_SET = "Please enter a valid format for `data_set_id`. To retrieve your data sets, execute `md.direct.user_items.get_data_sets()` and select a valid `data_set_id`. To retrieve morningstar data sets, execute `md.direct.lookup.get_morningstar_data_sets()` "
-BAD_REQUEST_ERROR_INVALID_DELIVER_CONFIG = "Delivery config is not valid. Check the docs for examples of accepted inputs."
-
-# Add custom resource not found error messages here
-RESOURCE_NOT_FOUND_ERROR = "Requested resource does not exist. Please make sure that the provided input belongs to a resource in Direct."
-RESOURCE_NOT_FOUND_ERROR_SEARCH_CRITERIA = "Requested resource not found with the provided `search_criteria_id`. Please make sure that the provided `search_criteria_id` is valid and exists. \nTo view all the available search criterias, execute - `md.direct.user_items.get_search_criteria()`."
-RESOURCE_NOT_FOUND_ERROR_NO_SEARCH_CRITERIA = "Requested resource not found. Please make sure that you have search criterias available in your Direct account. \nTo view search criterias, log in to Direct and navigate to `Workspace >> Search Criteria >> My Search Criteria`.\nSearch tutorial: https://morningstardirect.morningstar.com/clientcomm/Searches.pdf"
-RESOURCE_NOT_FOUND_ERROR_SEARCH_CRITERIA_ID = "Requested resource not found for search_criteria_id `{}`. Please make sure that provided search_criteria_id exists in your Direct account. To get all the search criterias, execute `md.direct.user_items.get_search_criteria()`"
-RESOURCE_NOT_FOUND_ERROR_SEARCH_CRITERIA_NO_INVESTMENTS = "Could not find any investments in the provided `search criteria`. Please make sure that provided `search criteria` is valid. To get all the search criterias, execute `md.direct.user_items.get_search_criteria()`"
-
-RESOURCE_NOT_FOUND_ERROR_NO_DATA_SETS = "No data sets found. To create a new data set, please open Direct and navigate to Workspace -> Data Sets -> My Data Sets -> New Data Set."
-RESOURCE_NOT_FOUND_ERROR_DATA_SET = "The requested `data_set_id` does not exist. To retrieve your data sets, execute `md.direct.user_items.get_data_sets()` and select a valid `data_set_id`. To retrieve morningstar data sets, execute `md.direct.lookup.get_morningstar_data_sets()`"
-RESOURCE_NOT_FOUND_ERROR_DATA_SET_DATA_POINT = (
-    "Please input a valid `data_set_id` to proceed with your query. To retrieve all the data sets, execute `md.direct.portfolio.get_data_sets()` and select a valid `data_set_id`."
-)
-RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_ACCOUNT = "Requested resource not found for the portfolio type. Maybe there is no portfolios with the portfolio type exist in your Direct account. \nTo create or see all of your existing portfolio accounts, log in to Direct and navigate to `Portfolio Management >> Accounts`. \nPortfolio management tutorial: https://morningstardirect.morningstar.com/clientcomm/Portfolios.pdf"
-RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_ACCOUNTS = "Requested resources not found. Please make sure that you have created at least one portfolio account in Direct. \nTo create or see all of your existing portfolio accounts, log in to Direct and navigate to `Portfolio Management >> Accounts`. \nPortfolio management tutorial: https://morningstardirect.morningstar.com/clientcomm/Portfolios.pdf"
-RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_ID = "Requested resource not found for portfolio ID `{}`. Please make sure that a portfolio account exists in your Direct account with the provided ID. To get the holding dates for all your portfolio accounts, execute `md.direct.portfolio.get_holding_dates()`."
-RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_IDS = "Requested resources not found for provided portfolio IDs. Please make sure that portfolio accounts exist, for the provided list of IDs, in your Direct account. To get the holding dates for all your portfolio accounts, execute `md.direct.portfolio.get_holding_dates()`."
-RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_HOLDING = "Requested resource not found for portfolio ID `{}` and dates. Please make sure that, in Direct, a portfolio account exists with the provided ID and has holdings during provided dates. To get the holding dates for all your portfolio accounts, execute `md.direct.portfolio.get_holding_dates()`."
-RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_HOLDINGS = "Requested resources not found for portfolio IDs and dates. Please make sure that, in Direct, portfolio accounts exist with the provided IDs and have holdings during provided dates. To get the holding dates for all your portfolio accounts, execute `md.direct.portfolio.get_holding_dates()`."
-RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_GET_DATA_RETURN = "Requested resource not found for portfolio ID `{}`. There is no return data available for the provided portfolio ID."
-
-# Add custom resource not found error messages here for Asset Flow module
-RESOURCE_NOT_FOUND_ASSET_FLOW = "The requested resource does not exist. Please make sure to provide a valid market_id."
-
-# Add custom resource not found error messages here for Investments module
-RESOURCE_NOT_FOUND_INVESTMENT_DATA = (
-    "No investments found for provided `investments` object. Please make sure that provided investments are valid and exist in your Direct account."
-)
-RESOURCE_NOT_FOUND_INVESTMENT_DATA_LIST_ID = "No investments found for the provided `list_id`. Please execute `md.direct.user_items.get_investment_lists()` to retrieve all the investment lists and select a valid `list_id`."
-RESOURCE_NOT_FOUND_INVESTMENT_DATA_SEARCH_CRITERIA_ID = "No investments found for the provided `search_criteria_id`. Please execute `md.direct.user_items.get_search_criteria()` to retrieve all the available search criterias and select a valid `id`."
-RESOURCE_NOT_FOUND_INVESTMENT_DATA_SEARCH_CRITERIA_CONDITION = "No investments found for the provided `search_criteria_condition`. Please execute `md.direct.user_items.get_search_criteria_conditions(search_criteria_id=:str)` with a valid search_criteria_id to build a search criteria condition."
-
-# Add custom resource not found error messages here for Performance module
-RESOURCE_NOT_FOUND_ERROR_PERFORMANCE_REPORT = "The requested resource does not exist. Please make sure that the provided `report_id` is valid and exists."
-
-# Add custom resource not found error messages here for Returns module
-RESOURCE_NOT_FOUND_ERROR_NO_RETURNS_RETRIEVED = "Failed to get returns for provided `investments` argument."
-RESOURCE_NOT_FOUND_ERROR_NO_RETURNS_RETRIEVED_FOR_INVESTMENT_LIST = (
-    "Could not fetch return for specified investment list. Please make sure that provided investments are valid and exist in your Direct account."
-)
-RESOURCE_NOT_FOUND_ERROR_NO_RETURNS_RETRIEVED_FOR_BENCHMARK_ID = (
-    "Could not fetch return for specified `benchmark_sec_id`. Please make sure that provided `benchmark_sec_id` is valid and exist in your Direct account."
-)
-
-# Add custom resource not found error messages here for Holding module
-RESOURCE_NOT_FOUND_ERROR_HOLDING = (
-    "The requested resource does not exist. Make sure that the provided `investment_ids` are valid and have holdings within the specified date or date range."
-)
-
-# Add custom error messages here for Peer group module
-BAD_REQUEST_ERROR_NO_DATA_POINT_ID_OR_ALIAS = "Specify datapointId and alias for each data_point."
-BAD_REQUEST_ERROR_ALIAS_DUPLICATED = "The alias can't be duplicated."
-BAD_REQUEST_ERROR_INCLUDE_NON_CALCULATION_DATA_POINTS = "Only calculated data points are supported."
-BAD_REQUEST_ERROR_INCLUDE_DIFF_CALCULATION_DATA_POINTS = "Calculation is supported only on same data points."
-BAD_REQUEST_ERROR_NO_DATA_POINTS = "No data_points."
-BAD_REQUEST_ERROR_INVALID_CATEGORY_ID = "Specify category_id in the format 'category_id;universe' to proceed with your query."
-BAD_REQUEST_ERROR_NO_INVESTMENT_SOURCE = "Specify the `investments` to proceed with your query."
-BAD_REQUEST_ERROR_INVALID_PERCENTILES = "The percentiles should be integer if not null and range from 1 to 100."
-
-# Add custom error messages here for investment list
-RESOURCE_NOT_FOUND_ERROR_INVESTMENT_List = "The requested resource does not exist. Please make sure that the provided `list_id` is valid and exists."
-
-# Add custom error messages here for portfolio list
-RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_List = (
-    "The requested resource does not exist. Make sure that the portfolios with provided `portfolio_type` is valid and exist in your Direct account."
-)
-
-
-# Add custom error messages here for Lookup
-RESOURCE_NOT_FOUND_ERROR_LOOKUP_KEYWORD = "Requested resource does not exist for the given `keyword`."
-RESOURCE_NOT_FOUND_ERROR_LOOKUP_KEYWORD_UNIVERSE = "Requested resource does not exist for the given `keyword` and `universe`."
-
-
-# Add custom error messages here for custom database
-RESOURCE_NOT_FOUND_ERROR_CUSTOM_DATABASE = "Requested resource does not exist for the given `database_type`."
-
-
-# Error messages related to 'save portfolio'
-BAD_REQUEST_ERROR_NO_PORTFOLIO_HOLDING_ID = "Holding id is missing, specify a valid holding_id."
-BAD_REQUEST_INVALID_PORTFOLIO_NAME = "Specify a valid portfolio name."
-BAD_REQUEST_PORTFOLIO_NAME_ALREADY_EXISTS = "The portfolio name already exists and 'overwrite_if_exists' is False."
-BAD_REQUEST_PORTFOLIO_WEIGHT_ERROR = "Holdings total weight is not 100%."
-BAD_REQUEST_INVALID_PORTFOLIO_TYPE = (
-    "The specified portfolio_type is not valid. Portfolio type should be one of the following: 'client_accounts', 'transaction_accounts', 'model_portfolios', 'custom_benchmarks'."
-)
-BAD_REQUEST_UNSUPPORTED_PORTFOLIO_TYPE = (
-    "Portfolios of type 'transaction_accounts' cannot be saved. Portfolio type should be one of following: 'client_accounts', 'model_portfolios', 'custom_benchmarks'."
-)
-BAD_REQUEST_INVALID_PORTFOLIO_HOLDING_DATA_FRAME = (
-    "Portfolio holdings data frame is missing required columns. Portfolio holdings data frame should have the following columns: 'Portfolio Date, 'HoldingId', 'Weight'"
-)
-
-# Add custom error messages here for data lookup
-RESOURCE_NOT_FOUND_ERROR_DATA_SET_LOOKUP = "Requested resource does not exist for the given `universe`."
-RESOURCE_NOT_FOUND_ERROR_DATA_POINT_LOOKUP = "Requested resource does not exist for the given `data_point_ids`."
-
-# Add custom errors for environment
-MALFORMED_JWT_ERROR = "Invalid JWT format. JWT should look like 'header.payload.signature' where header and payload are base64 encoded strings and signature is a hex string."
+ACCESS_DENIED_ERROR = "Unauthorized request! Please login with valid credentials. For more information, please contact Analytics Lab support team at Morningstar."
+FORBIDDEN_ERROR = "Forbidden request! You do not have permission to access this resource. For more information, please contact Analytics Lab support team at Morningstar."
+NETWORK_ERROR = "Network connection error. Please check your internet connection."
+TIMEOUT_ERROR = "Request timed out. Please try again or contact support at morningstardirect@moringstar.com"
+BAD_REQUEST_ERROR = "Bad request! Server could not process your request at this time. This error can occur due to multiple reasons (for example; bad request syntax, invalid message structure/framing, or incorrect/corrupt request).\nPlease refer morningstar data package documentation to make a valid request: https://docs-analyticslab.morningstar.com/latest/morningstar_data.html"
+CLIENT_ERROR = "Bad request! Server could not process your request at this time. This error can occur due to multiple reasons (for example; bad request syntax, invalid message structure/framing, or incorrect/corrupt request).\nPlease refer morningstar data package documentation to make a valid request: https://docs-analyticslab.morningstar.com/latest/morningstar_data.html"
+INTERNAL_SERVER_ERROR = (
+    "Something went wrong on our side!  For more details, please contact Analytics Lab support team at Morningstar. We apologize for any inconvenience this may have caused"
+)
+
+# Add query limit error messages here
+QUERY_LIMIT_ERROR = "You have reached your daily query limit. Please fill out this form for further assistance: https://go.morningstar.com/LP=6390"
+QUERY_LIMIT_ERROR_SHOW_LIMIT = "You have reached your daily query limit of $query cells. Please fill out this form for further assistance: https://go.morningstar.com/LP=6808"
+
+# AMS Flagged Features
+DELIVERY_ACCESS_ERROR = "You don't have access to this feature. Please fill out this form for further assistance: https://go.morningstar.com/LP=6809"
+
+# Add custom bad request error messages here
+BAD_REQUEST_ERROR_NO_START_AND_END_DATE = "Specify `start_date` and `end_date` to proceed with your query."
+BAD_REQUEST_ERROR_NO_END_DATE = "Specify the `end_date` to proceed with your query."
+BAD_REQUEST_ERROR_NO_START_DATE = "Specify the `start_date` to proceed with your query."
+BAD_REQUEST_ERROR_INCLUDE_ALL_DATE = "Specify either date or both start date and end date to proceed with your query."
+BAD_REQUEST_ERROR_INVALID_DATE_FORMAT = "Specify date in the format yyyy-MM-dd to proceed with your query."
+BAD_REQUEST_ERROR_NO_INVESTMENT_IDS = "Specify the `investment_ids` to proceed with your query."
+BAD_REQUEST_ERROR_NO_PORTFOLIO_DATA = "No matching portfolio data for the given date or date range."
+BAD_REQUEST_ERROR_INVALID_INVESTMENT_ID = "One or more ID's, in the provided list of `investment_ids`, are invalid!"
+BAD_REQUEST_ERROR_INVALID_INVESTMENT_LIST_ID = "Specify the valid `list_id` to proceed with your query. A `list_id` is a global unique identifier i.e. uuid."
+BAD_REQUEST_ERROR_INVALID_PORTFOLIO_ID = "Specify the valid `portfolio_id` to proceed with your query. A `portfolio_id` is a global unique identifier i.e. uuid."
+BAD_REQUEST_ERROR_INVALID_LOOKTHROUGH_HOLDING_TYPE = "Indexes are not supported as a valid Look-Through holding."
+BAD_REQUEST_ERROR_NO_START_AND_END_DATE = "Please specify `start_date` and `end_date` to proceed with your query."
+BAD_REQUEST_ERROR_NO_END_DATE = "Please specify the `end_date` to proceed with your query."
+BAD_REQUEST_ERROR_DATA_SET = "Please enter a valid format for `data_set_id`. To retrieve your data sets, execute `md.direct.user_items.get_data_sets()` and select a valid `data_set_id`. To retrieve morningstar data sets, execute `md.direct.lookup.get_morningstar_data_sets()` "
+BAD_REQUEST_ERROR_INVALID_DELIVER_CONFIG = "Delivery config is not valid. Check the docs for examples of accepted inputs."
+
+# Add custom resource not found error messages here
+RESOURCE_NOT_FOUND_ERROR = "Requested resource does not exist. Please make sure that the provided input belongs to a resource in Direct."
+RESOURCE_NOT_FOUND_ERROR_SEARCH_CRITERIA = "Requested resource not found with the provided `search_criteria_id`. Please make sure that the provided `search_criteria_id` is valid and exists. \nTo view all the available search criterias, execute - `md.direct.user_items.get_search_criteria()`."
+RESOURCE_NOT_FOUND_ERROR_NO_SEARCH_CRITERIA = "Requested resource not found. Please make sure that you have search criterias available in your Direct account. \nTo view search criterias, log in to Direct and navigate to `Workspace >> Search Criteria >> My Search Criteria`.\nSearch tutorial: https://morningstardirect.morningstar.com/clientcomm/Searches.pdf"
+RESOURCE_NOT_FOUND_ERROR_SEARCH_CRITERIA_ID = "Requested resource not found for search_criteria_id `{}`. Please make sure that provided search_criteria_id exists in your Direct account. To get all the search criterias, execute `md.direct.user_items.get_search_criteria()`"
+RESOURCE_NOT_FOUND_ERROR_SEARCH_CRITERIA_NO_INVESTMENTS = "Could not find any investments in the provided `search criteria`. Please make sure that provided `search criteria` is valid. To get all the search criterias, execute `md.direct.user_items.get_search_criteria()`"
+
+RESOURCE_NOT_FOUND_ERROR_NO_DATA_SETS = "No data sets found. To create a new data set, please open Direct and navigate to Workspace -> Data Sets -> My Data Sets -> New Data Set."
+RESOURCE_NOT_FOUND_ERROR_DATA_SET = "The requested `data_set_id` does not exist. To retrieve your data sets, execute `md.direct.user_items.get_data_sets()` and select a valid `data_set_id`. To retrieve morningstar data sets, execute `md.direct.lookup.get_morningstar_data_sets()`"
+RESOURCE_NOT_FOUND_ERROR_DATA_SET_DATA_POINT = (
+    "Please input a valid `data_set_id` to proceed with your query. To retrieve all the data sets, execute `md.direct.portfolio.get_data_sets()` and select a valid `data_set_id`."
+)
+RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_ACCOUNT = "Requested resource not found for the portfolio type. Maybe there is no portfolios with the portfolio type exist in your Direct account. \nTo create or see all of your existing portfolio accounts, log in to Direct and navigate to `Portfolio Management >> Accounts`. \nPortfolio management tutorial: https://morningstardirect.morningstar.com/clientcomm/Portfolios.pdf"
+RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_ACCOUNTS = "Requested resources not found. Please make sure that you have created at least one portfolio account in Direct. \nTo create or see all of your existing portfolio accounts, log in to Direct and navigate to `Portfolio Management >> Accounts`. \nPortfolio management tutorial: https://morningstardirect.morningstar.com/clientcomm/Portfolios.pdf"
+RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_ID = "Requested resource not found for portfolio ID `{}`. Please make sure that a portfolio account exists in your Direct account with the provided ID. To get the holding dates for all your portfolio accounts, execute `md.direct.portfolio.get_holding_dates()`."
+RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_IDS = "Requested resources not found for provided portfolio IDs. Please make sure that portfolio accounts exist, for the provided list of IDs, in your Direct account. To get the holding dates for all your portfolio accounts, execute `md.direct.portfolio.get_holding_dates()`."
+RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_HOLDING = "Requested resource not found for portfolio ID `{}` and dates. Please make sure that, in Direct, a portfolio account exists with the provided ID and has holdings during provided dates. To get the holding dates for all your portfolio accounts, execute `md.direct.portfolio.get_holding_dates()`."
+RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_HOLDINGS = "Requested resources not found for portfolio IDs and dates. Please make sure that, in Direct, portfolio accounts exist with the provided IDs and have holdings during provided dates. To get the holding dates for all your portfolio accounts, execute `md.direct.portfolio.get_holding_dates()`."
+RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_GET_DATA_RETURN = "Requested resource not found for portfolio ID `{}`. There is no return data available for the provided portfolio ID."
+
+# Add custom resource not found error messages here for Asset Flow module
+RESOURCE_NOT_FOUND_ASSET_FLOW = "The requested resource does not exist. Please make sure to provide a valid market_id."
+
+# Add custom resource not found error messages here for Investments module
+RESOURCE_NOT_FOUND_INVESTMENT_DATA = (
+    "No investments found for provided `investments` object. Please make sure that provided investments are valid and exist in your Direct account."
+)
+RESOURCE_NOT_FOUND_INVESTMENT_DATA_LIST_ID = "No investments found for the provided `list_id`. Please execute `md.direct.user_items.get_investment_lists()` to retrieve all the investment lists and select a valid `list_id`."
+RESOURCE_NOT_FOUND_INVESTMENT_DATA_SEARCH_CRITERIA_ID = "No investments found for the provided `search_criteria_id`. Please execute `md.direct.user_items.get_search_criteria()` to retrieve all the available search criterias and select a valid `id`."
+RESOURCE_NOT_FOUND_INVESTMENT_DATA_SEARCH_CRITERIA_CONDITION = "No investments found for the provided `search_criteria_condition`. Please execute `md.direct.user_items.get_search_criteria_conditions(search_criteria_id=:str)` with a valid search_criteria_id to build a search criteria condition."
+
+# Add custom resource not found error messages here for Performance module
+RESOURCE_NOT_FOUND_ERROR_PERFORMANCE_REPORT = "The requested resource does not exist. Please make sure that the provided `report_id` is valid and exists."
+
+# Add custom resource not found error messages here for Returns module
+RESOURCE_NOT_FOUND_ERROR_NO_RETURNS_RETRIEVED = "Failed to get returns for provided `investments` argument."
+RESOURCE_NOT_FOUND_ERROR_NO_RETURNS_RETRIEVED_FOR_INVESTMENT_LIST = (
+    "Could not fetch return for specified investment list. Please make sure that provided investments are valid and exist in your Direct account."
+)
+RESOURCE_NOT_FOUND_ERROR_NO_RETURNS_RETRIEVED_FOR_BENCHMARK_ID = (
+    "Could not fetch return for specified `benchmark_sec_id`. Please make sure that provided `benchmark_sec_id` is valid and exist in your Direct account."
+)
+
+# Add custom resource not found error messages here for Holding module
+RESOURCE_NOT_FOUND_ERROR_HOLDING = (
+    "The requested resource does not exist. Make sure that the provided `investment_ids` are valid and have holdings within the specified date or date range."
+)
+
+# Add custom error messages here for Peer group module
+BAD_REQUEST_ERROR_NO_DATA_POINT_ID_OR_ALIAS = "Specify datapointId and alias for each data_point."
+BAD_REQUEST_ERROR_ALIAS_DUPLICATED = "The alias can't be duplicated."
+BAD_REQUEST_ERROR_INCLUDE_NON_CALCULATION_DATA_POINTS = "Only calculated data points are supported."
+BAD_REQUEST_ERROR_INCLUDE_DIFF_CALCULATION_DATA_POINTS = "Calculation is supported only on same data points."
+BAD_REQUEST_ERROR_NO_DATA_POINTS = "No data_points."
+BAD_REQUEST_ERROR_INVALID_CATEGORY_ID = "Specify category_id in the format 'category_id;universe' to proceed with your query."
+BAD_REQUEST_ERROR_NO_INVESTMENT_SOURCE = "Specify the `investments` to proceed with your query."
+BAD_REQUEST_ERROR_INVALID_PERCENTILES = "The percentiles should be integer if not null and range from 1 to 100."
+
+# Add custom error messages here for investment list
+RESOURCE_NOT_FOUND_ERROR_INVESTMENT_List = "The requested resource does not exist. Please make sure that the provided `list_id` is valid and exists."
+
+# Add custom error messages here for portfolio list
+RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_List = (
+    "The requested resource does not exist. Make sure that the portfolios with provided `portfolio_type` is valid and exist in your Direct account."
+)
+
+
+# Add custom error messages here for Lookup
+RESOURCE_NOT_FOUND_ERROR_LOOKUP_KEYWORD = "Requested resource does not exist for the given `keyword`."
+RESOURCE_NOT_FOUND_ERROR_LOOKUP_KEYWORD_UNIVERSE = "Requested resource does not exist for the given `keyword` and `universe`."
+
+
+# Add custom error messages here for custom database
+RESOURCE_NOT_FOUND_ERROR_CUSTOM_DATABASE = "Requested resource does not exist for the given `database_type`."
+
+
+# Error messages related to 'save portfolio'
+BAD_REQUEST_ERROR_NO_PORTFOLIO_HOLDING_ID = "Holding id is missing, specify a valid holding_id."
+BAD_REQUEST_INVALID_PORTFOLIO_NAME = "Specify a valid portfolio name."
+BAD_REQUEST_PORTFOLIO_NAME_ALREADY_EXISTS = "The portfolio name already exists and 'overwrite_if_exists' is False."
+BAD_REQUEST_PORTFOLIO_WEIGHT_ERROR = "Holdings total weight is not 100%."
+BAD_REQUEST_INVALID_PORTFOLIO_TYPE = (
+    "The specified portfolio_type is not valid. Portfolio type should be one of the following: 'client_accounts', 'transaction_accounts', 'model_portfolios', 'custom_benchmarks'."
+)
+BAD_REQUEST_UNSUPPORTED_PORTFOLIO_TYPE = (
+    "Portfolios of type 'transaction_accounts' cannot be saved. Portfolio type should be one of following: 'client_accounts', 'model_portfolios', 'custom_benchmarks'."
+)
+BAD_REQUEST_INVALID_PORTFOLIO_HOLDING_DATA_FRAME = (
+    "Portfolio holdings data frame is missing required columns. Portfolio holdings data frame should have the following columns: 'Portfolio Date, 'HoldingId', 'Weight'"
+)
+
+# Add custom error messages here for data lookup
+RESOURCE_NOT_FOUND_ERROR_DATA_SET_LOOKUP = "Requested resource does not exist for the given `universe`."
+RESOURCE_NOT_FOUND_ERROR_DATA_POINT_LOOKUP = "Requested resource does not exist for the given `data_point_ids`."
+
+# Add custom errors for environment
+MALFORMED_JWT_ERROR = "Invalid JWT format. JWT should look like 'header.payload.signature' where header and payload are base64 encoded strings and signature is a hex string."
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_investment/_asset_flow_data.py` & `morningstar_data-1.3.0/morningstar_data/direct/_investment/_asset_flow_data.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-import simplejson as json
-from pandas import DataFrame
-
-from ..asset_flow import _asset_flow_api_request
-from .._config import _Config
-from .._data_objects import DataPoints, Investments
-from .._config_key import ALL_ASSET_FLOW_DATA_POINTS
-from ._common import _get_investment_ids, _get_data_points
-from ._data import InvestmentDataRequest, InvestmentDataResults, Column
-
-
-_config = _Config()
-
-
-class AssetFlowProvider:
-    @staticmethod
-    def build_request(investment_object: Investments, data_point_object: DataPoints, display_name: bool = False) -> InvestmentDataRequest:
-        investment_id_list = _get_investment_ids(investment_object)
-        data_points = _get_data_points(investment_object, data_point_object, display_name)
-        asset_flow_data_points = _filter_data_points_by_id(data_points, filter_list=ALL_ASSET_FLOW_DATA_POINTS)
-        return InvestmentDataRequest(investment_id_list, asset_flow_data_points)
-
-    @staticmethod
-    def run_request(req: InvestmentDataRequest) -> InvestmentDataResults:
-        return _get_asset_flow_data(req.investment_ids, req.data_points)
-
-
-def _filter_data_points_by_id(df: DataFrame, filter_list: list) -> DataFrame:
-    return df[df["datapointId"].isin(filter_list)].reset_index().drop(["index"], axis=1)
-
-
-def _get_asset_flow_data(investment_ids: list, asset_flow_data_point_settings: DataFrame) -> InvestmentDataResults:
-    investment_results = InvestmentDataResults()
-    if asset_flow_data_point_settings is not None and not asset_flow_data_point_settings.empty:
-        if "marketId" not in asset_flow_data_point_settings.columns:
-            asset_flow_data_point_settings["marketId"] = None
-        data_point_list = asset_flow_data_point_settings.to_dict(orient="records")
-        market_data_point_dict = _group_by_market(data_point_list)
-
-        for (market_id, data_points) in market_data_point_dict.items():
-            url = f"{_config.securitydata_service_url()}v1/assetflow/data"
-            postbody = {"marketId": market_id, "datapoints": data_points}
-            if investment_ids:
-                postbody["investments"] = list(map(lambda x: {"id": _get_sec_id(x)}, investment_ids))
-            sub_investment_results = _parse_raw_asset_flow_data_values(
-                investment_ids,
-                data_points,
-                _asset_flow_api_request.do_post_request(url, json.dumps(postbody, ignore_nan=True)),
-            )
-            investment_results.merge_with(sub_investment_results, in_place=True)
-    return investment_results
-
-
-def _group_by_market(data_point_list: list) -> dict:
-    market_data_point_dict: dict = dict()
-    for data_point in data_point_list:
-        market_id = data_point.get("marketId", None)
-        if market_id is not None and len(market_id.strip()) > 0:
-            market_data_points = market_data_point_dict.get(market_id, [])
-            market_data_points.append(data_point)
-            market_data_point_dict[market_id] = market_data_points
-    return market_data_point_dict
-
-
-def _parse_raw_asset_flow_data_values(investment_ids: list, data_points: list, response_json: list) -> InvestmentDataResults:
-    sub_investment_results = InvestmentDataResults()
-    if not response_json or not isinstance(response_json, list):
-        return sub_investment_results
-    sec_id_to_investment_id = {_get_sec_id(x): x for x in investment_ids}
-    alias_name_dict = {x.get("alias", ""): x.get("datapointName", "") for x in data_points}
-    for investment in response_json:
-        sec_id = investment.get("id", "")
-        investment_id = sec_id_to_investment_id[sec_id]
-        values = investment.get("values", [])
-        for data_point_value in values:
-            alias = data_point_value.get("alias", "").strip()
-            value_list = data_point_value.get("value", [])
-            column_data = [Column(name=_concat_str(alias_name_dict.get(alias, alias), x.get("date", "")), value=x.get("value", None)) for x in value_list]
-            sub_investment_results.add_column_data(investment_id, alias, column_data)
-    return sub_investment_results
-
-
-def _concat_str(s1: str, s2: str) -> str:
-    return s1 + " - " + s2
-
-
-def _get_sec_id(investment_id: str) -> str:
-    assert isinstance(investment_id, str)
-    sec_id, *_ = investment_id.split(";")
-    return sec_id
+import simplejson as json
+from pandas import DataFrame
+
+from ..asset_flow import _asset_flow_api_request
+from .._config import _Config
+from .._data_objects import DataPoints, Investments
+from .._config_key import ALL_ASSET_FLOW_DATA_POINTS
+from ._common import _get_investment_ids, _get_data_points
+from ._data import InvestmentDataRequest, InvestmentDataResults, Column
+
+
+_config = _Config()
+
+
+class AssetFlowProvider:
+    @staticmethod
+    def build_request(investment_object: Investments, data_point_object: DataPoints, display_name: bool = False) -> InvestmentDataRequest:
+        investment_id_list = _get_investment_ids(investment_object)
+        data_points = _get_data_points(investment_object, data_point_object, display_name)
+        asset_flow_data_points = _filter_data_points_by_id(data_points, filter_list=ALL_ASSET_FLOW_DATA_POINTS)
+        return InvestmentDataRequest(investment_id_list, asset_flow_data_points)
+
+    @staticmethod
+    def run_request(req: InvestmentDataRequest) -> InvestmentDataResults:
+        return _get_asset_flow_data(req.investment_ids, req.data_points)
+
+
+def _filter_data_points_by_id(df: DataFrame, filter_list: list) -> DataFrame:
+    return df[df["datapointId"].isin(filter_list)].reset_index().drop(["index"], axis=1)
+
+
+def _get_asset_flow_data(investment_ids: list, asset_flow_data_point_settings: DataFrame) -> InvestmentDataResults:
+    investment_results = InvestmentDataResults()
+    if asset_flow_data_point_settings is not None and not asset_flow_data_point_settings.empty:
+        if "marketId" not in asset_flow_data_point_settings.columns:
+            asset_flow_data_point_settings["marketId"] = None
+        data_point_list = asset_flow_data_point_settings.to_dict(orient="records")
+        market_data_point_dict = _group_by_market(data_point_list)
+
+        for (market_id, data_points) in market_data_point_dict.items():
+            url = f"{_config.securitydata_service_url()}v1/assetflow/data"
+            postbody = {"marketId": market_id, "datapoints": data_points}
+            if investment_ids:
+                postbody["investments"] = list(map(lambda x: {"id": _get_sec_id(x)}, investment_ids))
+            sub_investment_results = _parse_raw_asset_flow_data_values(
+                investment_ids,
+                data_points,
+                _asset_flow_api_request.do_post_request(url, json.dumps(postbody, ignore_nan=True)),
+            )
+            investment_results.merge_with(sub_investment_results, in_place=True)
+    return investment_results
+
+
+def _group_by_market(data_point_list: list) -> dict:
+    market_data_point_dict: dict = dict()
+    for data_point in data_point_list:
+        market_id = data_point.get("marketId", None)
+        if market_id is not None and len(market_id.strip()) > 0:
+            market_data_points = market_data_point_dict.get(market_id, [])
+            market_data_points.append(data_point)
+            market_data_point_dict[market_id] = market_data_points
+    return market_data_point_dict
+
+
+def _parse_raw_asset_flow_data_values(investment_ids: list, data_points: list, response_json: list) -> InvestmentDataResults:
+    sub_investment_results = InvestmentDataResults()
+    if not response_json or not isinstance(response_json, list):
+        return sub_investment_results
+    sec_id_to_investment_id = {_get_sec_id(x): x for x in investment_ids}
+    alias_name_dict = {x.get("alias", ""): x.get("datapointName", "") for x in data_points}
+    for investment in response_json:
+        sec_id = investment.get("id", "")
+        investment_id = sec_id_to_investment_id[sec_id]
+        values = investment.get("values", [])
+        for data_point_value in values:
+            alias = data_point_value.get("alias", "").strip()
+            value_list = data_point_value.get("value", [])
+            column_data = [Column(name=_concat_str(alias_name_dict.get(alias, alias), x.get("date", "")), value=x.get("value", None)) for x in value_list]
+            sub_investment_results.add_column_data(investment_id, alias, column_data)
+    return sub_investment_results
+
+
+def _concat_str(s1: str, s2: str) -> str:
+    return s1 + " - " + s2
+
+
+def _get_sec_id(investment_id: str) -> str:
+    assert isinstance(investment_id, str)
+    sec_id, *_ = investment_id.split(";")
+    return sec_id
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_investment/_common.py` & `morningstar_data-1.3.0/morningstar_data/direct/_investment/_common.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from pandas import DataFrame
-
-from .._data_objects import DataPoints, Investments
-from .._exceptions import ResourceNotFoundError
-from .. import _error_messages
-
-
-def _get_investment_ids(investment_object: Investments) -> list:
-    investment_id_list = investment_object.get_investment_ids()
-    if not investment_id_list:
-        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_INVESTMENT_DATA)
-    return investment_id_list
-
-
-def _get_data_points(investment_object: Investments, data_point_object: DataPoints, display_name: bool = False) -> DataFrame:
-    data_point_object.validate_data_point_ids()
-    return data_point_object.get_data_points(list_id=investment_object.list_id, search_criteria_id=investment_object.search_criteria, display_name=display_name)
-
-
-def _get_data_point_col_names(data_points: DataFrame, data_point_alias_to_cols: dict) -> list:
-    col_names = []
-    for _, data_point in data_points.iterrows():
-        alias = data_point.get("alias", "")
-        columns = data_point_alias_to_cols.get(alias, [])
-        col_names.extend(columns)
-    return col_names
-
-
-# def _build_result_data_frame(investment_data_list: list) -> DataFrame:
-#     result = DataFrame(investment_data_list)
-#     # TODO : .where() with Pandas 1.1.5 has a bug which converts all the columns including float to object
-#     # this was solved in Pandas update 1.3.5. Until we update Pandas, we will have to use this _replace_null_values()
-#     # as a workaround
-#     # results = df.where(result.notnull(), None)
-#     return result
+from pandas import DataFrame
+
+from .._data_objects import DataPoints, Investments
+from .._exceptions import ResourceNotFoundError
+from .. import _error_messages
+
+
+def _get_investment_ids(investment_object: Investments) -> list:
+    investment_id_list = investment_object.get_investment_ids()
+    if not investment_id_list:
+        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_INVESTMENT_DATA)
+    return investment_id_list
+
+
+def _get_data_points(investment_object: Investments, data_point_object: DataPoints, display_name: bool = False) -> DataFrame:
+    data_point_object.validate_data_point_ids()
+    return data_point_object.get_data_points(list_id=investment_object.list_id, search_criteria_id=investment_object.search_criteria, display_name=display_name)
+
+
+def _get_data_point_col_names(data_points: DataFrame, data_point_alias_to_cols: dict) -> list:
+    col_names = []
+    for _, data_point in data_points.iterrows():
+        alias = data_point.get("alias", "")
+        columns = data_point_alias_to_cols.get(alias, [])
+        col_names.extend(columns)
+    return col_names
+
+
+# def _build_result_data_frame(investment_data_list: list) -> DataFrame:
+#     result = DataFrame(investment_data_list)
+#     # TODO : .where() with Pandas 1.1.5 has a bug which converts all the columns including float to object
+#     # this was solved in Pandas update 1.3.5. Until we update Pandas, we will have to use this _replace_null_values()
+#     # as a workaround
+#     # results = df.where(result.notnull(), None)
+#     return result
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_investment/_data.py` & `morningstar_data-1.3.0/morningstar_data/direct/_investment/_data.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-from __future__ import annotations
-
-import copy
-from collections import OrderedDict
-from typing import Any, OrderedDict as OrderedDictType, List, NamedTuple
-from dataclasses import dataclass, field
-from pandas import DataFrame
-
-
-class Column(NamedTuple):
-    name: ColumnNameType
-    value: ColumnValueType
-
-
-InvestmentIdType = str
-DataPointAliasType = str
-ColumnNameType = Any
-ColumnValueType = Any
-ColumnListType = List[Column]
-ColumnDictType = OrderedDictType[ColumnNameType, ColumnValueType]
-MetaDataKeyType = Any
-MetaDataValueType = Any
-
-
-@dataclass(frozen=True)
-class InvestmentDataRequest:
-    """Stores parameters for getting investment data from DO APIs"""
-
-    investment_ids: list = field(default_factory=list)
-    data_points: DataFrame = field(default_factory=DataFrame)
-
-
-@dataclass
-class InvestmentDataResults:
-    """Stores multiple investment results returned by DO API, indexed by investment ID"""
-
-    _data: OrderedDictType[InvestmentIdType, InvestmentDataResult] = field(default_factory=OrderedDict)
-
-    # Commands
-    def add_column_data(self, investment_id: InvestmentIdType, alias: DataPointAliasType, column_data: ColumnListType) -> None:
-        self._ensure_investment_id_exists(investment_id)
-        self._data[investment_id].add_column_data(alias, column_data)
-
-    def add_meta_data(self, investment_id: InvestmentIdType, key: MetaDataKeyType, value: MetaDataValueType) -> None:
-        self._ensure_investment_id_exists(investment_id)
-        self._data[investment_id].add_meta_data(key, value)
-
-    def merge_with(self, other_results: InvestmentDataResults, in_place: bool = False) -> InvestmentDataResults:
-        new_results = self
-        if not in_place:
-            new_results = copy.deepcopy(self)
-
-        for investment_id, other_result in other_results._data.items():
-            new_results._ensure_investment_id_exists(investment_id)
-            new_results._data[investment_id].merge_with(other_result)
-
-        return new_results
-
-    # Queries
-    def get_column_data_value(self, investment_id: InvestmentIdType, alias: DataPointAliasType, col_name: ColumnNameType, default_value: ColumnValueType = None) -> ColumnValueType:
-        return self._data.get(investment_id, InvestmentDataResult()).get_column_data_value(alias, col_name, default_value)
-
-    def get_meta_data(self, investment_id: InvestmentIdType, key: MetaDataKeyType, default_value: MetaDataValueType = None) -> MetaDataValueType:
-        return self._data.get(investment_id, InvestmentDataResult()).get_meta_data(key, default_value)
-
-    def get_data_point_alias_to_col_dict(self) -> dict:
-        if len(self._data) == 0:
-            return dict()
-        one_investment: InvestmentDataResult = list(self._data.values())[0]
-        return one_investment.get_data_point_alias_to_col_dict()
-
-    def as_list(self) -> list:
-        new_list: list = []
-        for investment_id, result in self._data.items():
-            # TODO: find a better place for this check
-            if result.get_meta_data("entitled", None) is False:
-                continue
-            new_item: dict = dict()
-            # Always include the Investment ID column
-            new_item["Id"] = investment_id
-            for alias in result.get_aliases():
-                new_item.update(result.get_column_data(alias))
-            new_list.append(new_item)
-        return new_list
-
-    def as_data_frame(self, order_cols_by: list = []) -> DataFrame:
-        new_df = DataFrame(self.as_list())
-        if order_cols_by:
-            # Always include the Investment ID column
-            if "Id" not in order_cols_by:
-                return new_df[["Id"] + order_cols_by]
-            else:
-                return new_df[order_cols_by]
-        else:
-            return new_df
-
-    # Helpers
-    def _ensure_investment_id_exists(self, investment_id: InvestmentIdType) -> None:
-        if investment_id not in self._data:
-            self._data[investment_id] = InvestmentDataResult()
-
-
-@dataclass
-class InvestmentDataResult:
-    """Stores one investment result containing multiple data points, indexed by data point alias.
-    Each data point can contain one or more values (e.g., if data point contains time-series data).
-    Each value represents a column."""
-
-    _data: OrderedDictType[DataPointAliasType, ColumnDictType] = field(default_factory=OrderedDict)
-    _meta_data: OrderedDictType[MetaDataKeyType, MetaDataValueType] = field(default_factory=OrderedDict)
-
-    # Commands
-    def add_column_data(self, alias: DataPointAliasType, column_data: ColumnListType) -> None:
-        self._ensure_alias_exists(alias)
-        self._data[alias].update(column_data)
-
-    def add_meta_data(self, key: MetaDataKeyType, value: MetaDataValueType) -> None:
-        self._meta_data[key] = value
-
-    def merge_with(self, other_result: InvestmentDataResult) -> None:
-        for alias, other_values in other_result._data.items():
-            self._ensure_alias_exists(alias)
-            self._data[alias].update(other_values)
-        self._meta_data.update(other_result._meta_data)
-
-    # Queries
-    def get_column_data(self, alias: DataPointAliasType, default_value: ColumnDictType = OrderedDict()) -> ColumnDictType:
-        return self._data.get(alias, default_value)
-
-    def get_column_data_value(self, alias: DataPointAliasType, col_name: ColumnNameType, default_value: ColumnValueType = None) -> ColumnValueType:
-        return self.get_column_data(alias).get(col_name, default_value)
-
-    def get_meta_data(self, key: MetaDataKeyType, default_value: MetaDataValueType = None) -> MetaDataValueType:
-        return self._meta_data.get(key, default_value)
-
-    def get_data_point_alias_to_col_dict(self) -> dict:
-        result = dict()
-        for alias, columns in self._data.items():
-            result[alias] = list(columns.keys())
-        return result
-
-    def get_aliases(self) -> list:
-        return list(self._data.keys())
-
-    # Helpers
-    def _ensure_alias_exists(self, alias: DataPointAliasType) -> None:
-        if alias not in self._data:
-            self._data[alias] = OrderedDict()
+from __future__ import annotations
+
+import copy
+from collections import OrderedDict
+from typing import Any, OrderedDict as OrderedDictType, List, NamedTuple
+from dataclasses import dataclass, field
+from pandas import DataFrame
+
+
+class Column(NamedTuple):
+    name: ColumnNameType
+    value: ColumnValueType
+
+
+InvestmentIdType = str
+DataPointAliasType = str
+ColumnNameType = Any
+ColumnValueType = Any
+ColumnListType = List[Column]
+ColumnDictType = OrderedDictType[ColumnNameType, ColumnValueType]
+MetaDataKeyType = Any
+MetaDataValueType = Any
+
+
+@dataclass(frozen=True)
+class InvestmentDataRequest:
+    """Stores parameters for getting investment data from DO APIs"""
+
+    investment_ids: list = field(default_factory=list)
+    data_points: DataFrame = field(default_factory=DataFrame)
+
+
+@dataclass
+class InvestmentDataResults:
+    """Stores multiple investment results returned by DO API, indexed by investment ID"""
+
+    _data: OrderedDictType[InvestmentIdType, InvestmentDataResult] = field(default_factory=OrderedDict)
+
+    # Commands
+    def add_column_data(self, investment_id: InvestmentIdType, alias: DataPointAliasType, column_data: ColumnListType) -> None:
+        self._ensure_investment_id_exists(investment_id)
+        self._data[investment_id].add_column_data(alias, column_data)
+
+    def add_meta_data(self, investment_id: InvestmentIdType, key: MetaDataKeyType, value: MetaDataValueType) -> None:
+        self._ensure_investment_id_exists(investment_id)
+        self._data[investment_id].add_meta_data(key, value)
+
+    def merge_with(self, other_results: InvestmentDataResults, in_place: bool = False) -> InvestmentDataResults:
+        new_results = self
+        if not in_place:
+            new_results = copy.deepcopy(self)
+
+        for investment_id, other_result in other_results._data.items():
+            new_results._ensure_investment_id_exists(investment_id)
+            new_results._data[investment_id].merge_with(other_result)
+
+        return new_results
+
+    # Queries
+    def get_column_data_value(self, investment_id: InvestmentIdType, alias: DataPointAliasType, col_name: ColumnNameType, default_value: ColumnValueType = None) -> ColumnValueType:
+        return self._data.get(investment_id, InvestmentDataResult()).get_column_data_value(alias, col_name, default_value)
+
+    def get_meta_data(self, investment_id: InvestmentIdType, key: MetaDataKeyType, default_value: MetaDataValueType = None) -> MetaDataValueType:
+        return self._data.get(investment_id, InvestmentDataResult()).get_meta_data(key, default_value)
+
+    def get_data_point_alias_to_col_dict(self) -> dict:
+        if len(self._data) == 0:
+            return dict()
+        one_investment: InvestmentDataResult = list(self._data.values())[0]
+        return one_investment.get_data_point_alias_to_col_dict()
+
+    def as_list(self) -> list:
+        new_list: list = []
+        for investment_id, result in self._data.items():
+            # TODO: find a better place for this check
+            if result.get_meta_data("entitled", None) is False:
+                continue
+            new_item: dict = dict()
+            # Always include the Investment ID column
+            new_item["Id"] = investment_id
+            for alias in result.get_aliases():
+                new_item.update(result.get_column_data(alias))
+            new_list.append(new_item)
+        return new_list
+
+    def as_data_frame(self, order_cols_by: list = []) -> DataFrame:
+        new_df = DataFrame(self.as_list())
+        if order_cols_by:
+            # Always include the Investment ID column
+            if "Id" not in order_cols_by:
+                return new_df[["Id"] + order_cols_by]
+            else:
+                return new_df[order_cols_by]
+        else:
+            return new_df
+
+    # Helpers
+    def _ensure_investment_id_exists(self, investment_id: InvestmentIdType) -> None:
+        if investment_id not in self._data:
+            self._data[investment_id] = InvestmentDataResult()
+
+
+@dataclass
+class InvestmentDataResult:
+    """Stores one investment result containing multiple data points, indexed by data point alias.
+    Each data point can contain one or more values (e.g., if data point contains time-series data).
+    Each value represents a column."""
+
+    _data: OrderedDictType[DataPointAliasType, ColumnDictType] = field(default_factory=OrderedDict)
+    _meta_data: OrderedDictType[MetaDataKeyType, MetaDataValueType] = field(default_factory=OrderedDict)
+
+    # Commands
+    def add_column_data(self, alias: DataPointAliasType, column_data: ColumnListType) -> None:
+        self._ensure_alias_exists(alias)
+        self._data[alias].update(column_data)
+
+    def add_meta_data(self, key: MetaDataKeyType, value: MetaDataValueType) -> None:
+        self._meta_data[key] = value
+
+    def merge_with(self, other_result: InvestmentDataResult) -> None:
+        for alias, other_values in other_result._data.items():
+            self._ensure_alias_exists(alias)
+            self._data[alias].update(other_values)
+        self._meta_data.update(other_result._meta_data)
+
+    # Queries
+    def get_column_data(self, alias: DataPointAliasType, default_value: ColumnDictType = OrderedDict()) -> ColumnDictType:
+        return self._data.get(alias, default_value)
+
+    def get_column_data_value(self, alias: DataPointAliasType, col_name: ColumnNameType, default_value: ColumnValueType = None) -> ColumnValueType:
+        return self.get_column_data(alias).get(col_name, default_value)
+
+    def get_meta_data(self, key: MetaDataKeyType, default_value: MetaDataValueType = None) -> MetaDataValueType:
+        return self._meta_data.get(key, default_value)
+
+    def get_data_point_alias_to_col_dict(self) -> dict:
+        result = dict()
+        for alias, columns in self._data.items():
+            result[alias] = list(columns.keys())
+        return result
+
+    def get_aliases(self) -> list:
+        return list(self._data.keys())
+
+    # Helpers
+    def _ensure_alias_exists(self, alias: DataPointAliasType) -> None:
+        if alias not in self._data:
+            self._data[alias] = OrderedDict()
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_investment/_normal_data.py` & `morningstar_data-1.3.0/morningstar_data/direct/_investment/_normal_data.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,181 +1,181 @@
-import simplejson as json
-import functools
-from pandas import DataFrame
-from typing import Optional, List, Dict, Any, Callable
-
-from ...direct._api import _direct_api_request
-from .._config import _Config
-from .._exceptions import BadRequestException, ApiResponseException
-from .._data_objects import Investments, DataPoints
-from .._config_key import ALL_ASSET_FLOW_DATA_POINTS
-
-from ._common import _get_investment_ids, _get_data_points
-from ._data import InvestmentDataRequest, InvestmentDataResults, Column
-
-_config = _Config()
-
-
-class NormalDataProvider:
-    @staticmethod
-    def build_request(investment_object: Investments, data_point_object: DataPoints, display_name: bool = False) -> InvestmentDataRequest:
-        investment_id_list = _get_investment_ids(investment_object)
-        data_points = _get_data_points(investment_object, data_point_object, display_name)
-        normal_data_points = _filter_out_data_points_by_id(data_points, filter_out_list=ALL_ASSET_FLOW_DATA_POINTS)
-        return InvestmentDataRequest(investment_id_list, normal_data_points)
-
-    @staticmethod
-    def run_request(req: InvestmentDataRequest) -> InvestmentDataResults:
-        raw_data = _get_normal_data(req.investment_ids, req.data_points)
-        return _parse_raw_normal_data_values(raw_data)
-
-
-def _filter_out_data_points_by_id(df: DataFrame, filter_out_list: list) -> DataFrame:
-    return df[~df["datapointId"].isin(filter_out_list)].reset_index().drop(["index"], axis=1)
-
-
-def _get_normal_data(investment_ids: list, normal_data_point_settings: DataFrame) -> dict:
-    normal_resp: dict = dict()
-    if normal_data_point_settings is not None and not normal_data_point_settings.empty:
-        if not investment_ids:
-            raise BadRequestException("No investments.")
-        data_point_list = normal_data_point_settings.to_dict(orient="records")
-        postbody = {
-            "datapoints": data_point_list,
-            "investments": list(map(lambda x: {"id": x}, investment_ids)),
-        }
-        resp = _request_investment_data(postbody)
-        if resp and isinstance(resp, dict):
-            normal_resp.update(resp)
-
-        updated_data_point_list = []
-
-        for data_point, normal_data_point in zip(data_point_list, normal_resp["datapoints"]):
-            alias_exists = data_point["alias"] == normal_data_point["alias"]
-            use_display_name = "displayName" in normal_data_point_settings.columns and data_point["displayName"]
-            if not alias_exists:
-                raise ApiResponseException("The Investment Data API returned a bad response.")
-            elif use_display_name:
-                name = data_point["displayName"]
-            else:
-                name = normal_data_point["name"]
-
-            data_point_entry = {**normal_data_point, "name": name}
-            updated_data_point_list.append(data_point_entry)
-
-        normal_resp["datapoints"] = updated_data_point_list
-
-    return normal_resp
-
-
-def _request_investment_data(params: dict) -> Dict[str, Any]:
-    url = f"{_config.securitydata_service_url()}v1/data?includeAdditionalDps=false"
-    response_json: Dict[str, Any] = _direct_api_request("POST", url, data=json.dumps(params, ignore_nan=True))
-    return response_json
-
-
-def _parse_raw_normal_data_values(response_json: dict) -> InvestmentDataResults:
-    investment_results = InvestmentDataResults()
-    data_points = response_json.get("datapoints", [])
-    for inv in response_json.get("investments", []):
-        investment_id = inv.get("id", "")
-        if _with_entitled(inv) is False:
-            investment_results.add_meta_data(investment_id, "entitled", False)
-            continue
-        value_map = dict(list(map(lambda x: (x.get("alias", ""), x), inv.get("values", []))))
-        for dp in data_points:
-            alias = dp.get("alias", "")
-            value = value_map.get(alias, None)
-            add_column_data = functools.partial(investment_results.add_column_data, investment_id, alias)
-
-            if _with_entitled(value) is False:
-                add_column_data(_convert_data_point_to_column(dp, None))
-                continue
-
-            if dp.get("isTsdp", False):
-                add_column_data(_convert_ts_data_point_to_columns(dp, value))
-                continue
-
-            if "MULTIPLE" == dp.get("nonstandardDisplayType", ""):
-                add_column_data(_convert_multiple_display_type_data_point_to_column(dp, value))
-            else:  # current data_point
-                add_column_data(_convert_data_point_to_column(dp, value))
-    return investment_results
-
-
-def _convert_data_point_to_column(data_point: dict, value: Optional[dict]) -> list:
-    # { "alias": "HS05A_4", "value": "3", "text": "Large Growth" }
-    data_point_name = data_point.get("name", "")
-    if value is None or not isinstance(value, dict):
-        return [Column(name=data_point_name, value=value)]
-    if _is_mstar_ip_data_point(data_point):
-        return [Column(name=data_point_name, value=value.get("value")), Column(name=_get_mstar_ip_data_point_text_column_name(data_point), value=value.get("text"))]
-    else:
-        return [Column(name=data_point_name, value=value.get("text", value.get("value")))]
-
-
-def _convert_ts_data_point_to_columns(data_point: dict, value: dict) -> list:
-    # { "alias": "HS05A_3", "value": [ { "index": 0, "text": "Large Growth", "value": "3" }, { "index": 1, "text": "Large Growth", "value": "3" } ] }
-    column_data: list = list()
-    value_map = dict(list(map(lambda x: (x.get("index", ""), x), value.get("value", [])))) if isinstance(value, dict) else dict()
-    for i, tp in enumerate(data_point.get("timePeriods", [])):
-        value_dict: dict = value_map.get(i, dict())
-        if _with_entitled(value_dict) is False:
-            value_dict = dict()
-        if _is_mstar_ip_data_point(data_point):
-            column_data.append(Column(name=_get_ts_column_name(data_point, _get_date(tp)), value=value_dict.get("value")))
-            column_data.append(Column(name=_get_mstar_ip_data_point_text_column_name(data_point, _get_date(tp)), value=value_dict.get("text")))
-        else:
-            column_data.append(Column(name=_get_ts_column_name(data_point, _get_date(tp)), value=value_dict.get("text", value_dict.get("value"))))
-    return column_data
-
-
-def _convert_multiple_display_type_data_point_to_column(data_point: dict, value: dict) -> list:
-    #  { "alias": "HS05A_3", "value": [{ "value": "[1996-11-01 -- ] William C. Nygren" },{ "value": "[2000-03-21 -- 2012-08-01] Henry Berghoef" }] }
-    data_point_name = data_point.get("name", "")
-    val: Optional[List[Dict[str, Any]]] = value.get("value") if isinstance(value, dict) else value
-    if isinstance(val, list):
-        get_value: Callable[[Dict[str, Any]], Any] = lambda x: x["value"]
-        v: List[Any] = list(map(get_value, val))
-        values: Optional[List[Any]] = v if len(v) > 0 else None
-        return [Column(name=data_point_name, value=values)]
-    else:
-        return [Column(name=data_point_name, value=val)]
-
-
-def _is_mstar_ip_data_point(data_point: dict) -> bool:
-    mstar_ip_type = data_point.get("mstarIpType", "") if data_point is not None else ""
-    return mstar_ip_type is not None and len(mstar_ip_type) > 0
-
-
-def _get_date(timeperiod: dict) -> str:
-    start_date = timeperiod.get("startDate", "")
-    end_date = timeperiod.get("endDate", "")
-    return f"{start_date} to {end_date}" if len(start_date) > 0 else f"{end_date}"
-
-
-def _get_ts_column_name(data_point: dict, date: str) -> str:
-    data_point_name = _get_display_name(data_point)
-    return f"{data_point_name} {date}"
-
-
-def _get_mstar_ip_data_point_text_column_name(data_point: dict, date: Optional[str] = None) -> Any:
-    resp = _get_display_name(data_point) + " - display text"
-    if date is not None and len(date) > 0:
-        resp = resp + " " + date
-    return resp
-
-
-def _get_display_name(data_point: dict) -> str:
-    if data_point.get("displayName") is not None:
-        return str(data_point.get("displayName"))
-    return data_point.get("name", "")
-
-
-def _with_entitled(data: dict) -> bool:
-    # NBI-523: Rollback NBI-433
-    # if data:
-    #     entitled = data.get("entitled", True)
-    #     is_allowed_to_be_exported = data.get("isAllowedToBeExported", True)
-    #     if entitled is False or is_allowed_to_be_exported is False:
-    #         return False
-    return True
+import simplejson as json
+import functools
+from pandas import DataFrame
+from typing import Optional, List, Dict, Any, Callable
+
+from ...direct._api import _direct_api_request
+from .._config import _Config
+from .._exceptions import BadRequestException, ApiResponseException
+from .._data_objects import Investments, DataPoints
+from .._config_key import ALL_ASSET_FLOW_DATA_POINTS
+
+from ._common import _get_investment_ids, _get_data_points
+from ._data import InvestmentDataRequest, InvestmentDataResults, Column
+
+_config = _Config()
+
+
+class NormalDataProvider:
+    @staticmethod
+    def build_request(investment_object: Investments, data_point_object: DataPoints, display_name: bool = False) -> InvestmentDataRequest:
+        investment_id_list = _get_investment_ids(investment_object)
+        data_points = _get_data_points(investment_object, data_point_object, display_name)
+        normal_data_points = _filter_out_data_points_by_id(data_points, filter_out_list=ALL_ASSET_FLOW_DATA_POINTS)
+        return InvestmentDataRequest(investment_id_list, normal_data_points)
+
+    @staticmethod
+    def run_request(req: InvestmentDataRequest) -> InvestmentDataResults:
+        raw_data = _get_normal_data(req.investment_ids, req.data_points)
+        return _parse_raw_normal_data_values(raw_data)
+
+
+def _filter_out_data_points_by_id(df: DataFrame, filter_out_list: list) -> DataFrame:
+    return df[~df["datapointId"].isin(filter_out_list)].reset_index().drop(["index"], axis=1)
+
+
+def _get_normal_data(investment_ids: list, normal_data_point_settings: DataFrame) -> dict:
+    normal_resp: dict = dict()
+    if normal_data_point_settings is not None and not normal_data_point_settings.empty:
+        if not investment_ids:
+            raise BadRequestException("No investments.")
+        data_point_list = normal_data_point_settings.to_dict(orient="records")
+        postbody = {
+            "datapoints": data_point_list,
+            "investments": list(map(lambda x: {"id": x}, investment_ids)),
+        }
+        resp = _request_investment_data(postbody)
+        if resp and isinstance(resp, dict):
+            normal_resp.update(resp)
+
+        updated_data_point_list = []
+
+        for data_point, normal_data_point in zip(data_point_list, normal_resp["datapoints"]):
+            alias_exists = data_point["alias"] == normal_data_point["alias"]
+            use_display_name = "displayName" in normal_data_point_settings.columns and data_point["displayName"]
+            if not alias_exists:
+                raise ApiResponseException("The Investment Data API returned a bad response.")
+            elif use_display_name:
+                name = data_point["displayName"]
+            else:
+                name = normal_data_point["name"]
+
+            data_point_entry = {**normal_data_point, "name": name}
+            updated_data_point_list.append(data_point_entry)
+
+        normal_resp["datapoints"] = updated_data_point_list
+
+    return normal_resp
+
+
+def _request_investment_data(params: dict) -> Dict[str, Any]:
+    url = f"{_config.securitydata_service_url()}v1/data?includeAdditionalDps=false"
+    response_json: Dict[str, Any] = _direct_api_request("POST", url, data=json.dumps(params, ignore_nan=True))
+    return response_json
+
+
+def _parse_raw_normal_data_values(response_json: dict) -> InvestmentDataResults:
+    investment_results = InvestmentDataResults()
+    data_points = response_json.get("datapoints", [])
+    for inv in response_json.get("investments", []):
+        investment_id = inv.get("id", "")
+        if _with_entitled(inv) is False:
+            investment_results.add_meta_data(investment_id, "entitled", False)
+            continue
+        value_map = dict(list(map(lambda x: (x.get("alias", ""), x), inv.get("values", []))))
+        for dp in data_points:
+            alias = dp.get("alias", "")
+            value = value_map.get(alias, None)
+            add_column_data = functools.partial(investment_results.add_column_data, investment_id, alias)
+
+            if _with_entitled(value) is False:
+                add_column_data(_convert_data_point_to_column(dp, None))
+                continue
+
+            if dp.get("isTsdp", False):
+                add_column_data(_convert_ts_data_point_to_columns(dp, value))
+                continue
+
+            if "MULTIPLE" == dp.get("nonstandardDisplayType", ""):
+                add_column_data(_convert_multiple_display_type_data_point_to_column(dp, value))
+            else:  # current data_point
+                add_column_data(_convert_data_point_to_column(dp, value))
+    return investment_results
+
+
+def _convert_data_point_to_column(data_point: dict, value: Optional[dict]) -> list:
+    # { "alias": "HS05A_4", "value": "3", "text": "Large Growth" }
+    data_point_name = data_point.get("name", "")
+    if value is None or not isinstance(value, dict):
+        return [Column(name=data_point_name, value=value)]
+    if _is_mstar_ip_data_point(data_point):
+        return [Column(name=data_point_name, value=value.get("value")), Column(name=_get_mstar_ip_data_point_text_column_name(data_point), value=value.get("text"))]
+    else:
+        return [Column(name=data_point_name, value=value.get("text", value.get("value")))]
+
+
+def _convert_ts_data_point_to_columns(data_point: dict, value: dict) -> list:
+    # { "alias": "HS05A_3", "value": [ { "index": 0, "text": "Large Growth", "value": "3" }, { "index": 1, "text": "Large Growth", "value": "3" } ] }
+    column_data: list = list()
+    value_map = dict(list(map(lambda x: (x.get("index", ""), x), value.get("value", [])))) if isinstance(value, dict) else dict()
+    for i, tp in enumerate(data_point.get("timePeriods", [])):
+        value_dict: dict = value_map.get(i, dict())
+        if _with_entitled(value_dict) is False:
+            value_dict = dict()
+        if _is_mstar_ip_data_point(data_point):
+            column_data.append(Column(name=_get_ts_column_name(data_point, _get_date(tp)), value=value_dict.get("value")))
+            column_data.append(Column(name=_get_mstar_ip_data_point_text_column_name(data_point, _get_date(tp)), value=value_dict.get("text")))
+        else:
+            column_data.append(Column(name=_get_ts_column_name(data_point, _get_date(tp)), value=value_dict.get("text", value_dict.get("value"))))
+    return column_data
+
+
+def _convert_multiple_display_type_data_point_to_column(data_point: dict, value: dict) -> list:
+    #  { "alias": "HS05A_3", "value": [{ "value": "[1996-11-01 -- ] William C. Nygren" },{ "value": "[2000-03-21 -- 2012-08-01] Henry Berghoef" }] }
+    data_point_name = data_point.get("name", "")
+    val: Optional[List[Dict[str, Any]]] = value.get("value") if isinstance(value, dict) else value
+    if isinstance(val, list):
+        get_value: Callable[[Dict[str, Any]], Any] = lambda x: x["value"]
+        v: List[Any] = list(map(get_value, val))
+        values: Optional[List[Any]] = v if len(v) > 0 else None
+        return [Column(name=data_point_name, value=values)]
+    else:
+        return [Column(name=data_point_name, value=val)]
+
+
+def _is_mstar_ip_data_point(data_point: dict) -> bool:
+    mstar_ip_type = data_point.get("mstarIpType", "") if data_point is not None else ""
+    return mstar_ip_type is not None and len(mstar_ip_type) > 0
+
+
+def _get_date(timeperiod: dict) -> str:
+    start_date = timeperiod.get("startDate", "")
+    end_date = timeperiod.get("endDate", "")
+    return f"{start_date} to {end_date}" if len(start_date) > 0 else f"{end_date}"
+
+
+def _get_ts_column_name(data_point: dict, date: str) -> str:
+    data_point_name = _get_display_name(data_point)
+    return f"{data_point_name} {date}"
+
+
+def _get_mstar_ip_data_point_text_column_name(data_point: dict, date: Optional[str] = None) -> Any:
+    resp = _get_display_name(data_point) + " - display text"
+    if date is not None and len(date) > 0:
+        resp = resp + " " + date
+    return resp
+
+
+def _get_display_name(data_point: dict) -> str:
+    if data_point.get("displayName") is not None:
+        return str(data_point.get("displayName"))
+    return data_point.get("name", "")
+
+
+def _with_entitled(data: dict) -> bool:
+    # NBI-523: Rollback NBI-433
+    # if data:
+    #     entitled = data.get("entitled", True)
+    #     is_allowed_to_be_exported = data.get("isAllowedToBeExported", True)
+    #     if entitled is False or is_allowed_to_be_exported is False:
+    #         return False
+    return True
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_investment/_peer_group_data.py` & `morningstar_data-1.3.0/morningstar_data/direct/_investment/_peer_group_data.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,131 +1,131 @@
-import simplejson as json
-from dataclasses import dataclass
-from pandas import DataFrame
-
-from typing import Optional, List, Any
-from .._exceptions import BadRequestException
-from .._config import _Config
-from ..data_type import PeerGroupMethodology, Order
-from .._data_objects import DataPoints, Investments
-from ..._base import _logger
-from .._exceptions import ResourceNotFoundError, InternalServerError
-from .._base_api import APIBackend
-from .._error_messages import BAD_REQUEST_ERROR_INVALID_PERCENTILES
-
-_config = _Config()
-
-
-class PeerGroupAPIBackend(APIBackend):
-    """
-    Subclass to call the Peer Group Data API and handle any HTTP errors that occur.
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def _handle_custom_http_errors(self, res: Any) -> Any:
-        """
-        Handle HTTP errors with custom error messages
-        """
-        response_message = res.json()["message"]
-        if res.status_code == 404:
-            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
-            raise ResourceNotFoundError from None
-
-        if res.status_code == 500:
-            _logger.debug(f"Something went wrong: {res.status_code} {response_message}")
-            raise InternalServerError(response_message) from None
-
-
-_peer_group_api_request = PeerGroupAPIBackend()
-
-
-@dataclass(frozen=True)
-class PeerGroupRequest:
-    investment_source: dict
-    data_points: DataFrame
-    order: Order
-    percentiles: Optional[List[int]] = None
-    methodology: Optional[PeerGroupMethodology] = None
-
-
-@dataclass(frozen=True)
-class PeerGroupResponse:
-    req: PeerGroupRequest
-    breakpoints: list
-
-
-class PeerGroupProvider:
-    def build_request(
-        self,
-        investment_object: Investments,
-        data_point_object: DataPoints,
-        order: Order,
-        percentiles: Optional[List[int]] = None,
-        methodology: Optional[PeerGroupMethodology] = None,
-    ) -> PeerGroupRequest:
-        # do not support dataset id
-        data_point_object.data_set_id = None
-        methodology = _get_methodology_value(methodology)
-        _validate_percentiles(percentiles)
-
-        investment_source = investment_object.generate_investment_source()
-        data_point_data_frame = _get_data_points(data_point_object)
-
-        return PeerGroupRequest(investment_source, data_point_data_frame, order, percentiles, methodology)
-
-    def run_request(self, req: PeerGroupRequest) -> PeerGroupResponse:
-        breakpoints = _get_breakpoints(
-            investment_source=req.investment_source, data_point_data_frame=req.data_points, order=req.order.value, methodology=req.methodology, percentiles=req.percentiles
-        )
-        return PeerGroupResponse(req, breakpoints)
-
-    def build_data_frame(self, resp: PeerGroupResponse) -> DataFrame:
-        return _convert_to_breakpoints_data_frame(resp.breakpoints)
-
-
-def _get_breakpoints(investment_source: dict, data_point_data_frame: DataFrame, order: Any, methodology: Optional[str] = None, percentiles: Optional[list] = None) -> list:
-    breakpoints = []
-    postbody = {"investmentSource": investment_source, "datapoints": data_point_data_frame.to_dict(orient="records"), "percentiles": percentiles, "order": order}
-    url = f"{_config.peergroup_service_url()}peergroupservice/v1/breakpoints"
-    if methodology is not None and len(methodology.strip()) > 0:
-        url = f"{url}?methodology={methodology}"
-    resp = _peer_group_api_request.do_post_request(url, json.dumps(postbody, ignore_nan=True))
-    if resp and isinstance(resp, dict):
-        breakpoints = resp.get("breakpoints", [])
-    return breakpoints
-
-
-def _convert_to_breakpoints_data_frame(breakpoints: list) -> DataFrame:
-    breakpoint_list = []
-    for breakpoint in breakpoints:
-        breakpoint_dict = dict()
-        breakpoint_dict["Alias"] = breakpoint.get("alias", None)
-        time_period = breakpoint.get("timePeriod", dict())
-        breakpoint_dict["StartDate"] = time_period.get("startDate", dict())
-        breakpoint_dict["EndDate"] = time_period.get("endDate", dict())
-        values = breakpoint.get("values", list())
-        for value in values:
-            breakpoint_dict[value.get("percentile", None)] = value.get("value", None)
-        breakpoint_list.append(breakpoint_dict)
-    return DataFrame(breakpoint_list)
-
-
-def _get_methodology_value(methodology: Optional[PeerGroupMethodology] = None) -> Any:
-    if methodology is not None and isinstance(methodology, PeerGroupMethodology):
-        return methodology.value
-    return None
-
-
-def _validate_percentiles(percentiles: Optional[list] = None) -> None:
-    if not percentiles:
-        return
-
-    for per in percentiles:
-        if per is None or not isinstance(per, int) or per < 1 or per > 100:
-            raise BadRequestException(BAD_REQUEST_ERROR_INVALID_PERCENTILES)
-
-
-def _get_data_points(data_point_object: DataPoints) -> DataFrame:
-    data_point_object._validate_data_point_ids_and_alias()
-    return data_point_object.get_peer_group_data_points()
+import simplejson as json
+from dataclasses import dataclass
+from pandas import DataFrame
+
+from typing import Optional, List, Any
+from .._exceptions import BadRequestException
+from .._config import _Config
+from ..data_type import PeerGroupMethodology, Order
+from .._data_objects import DataPoints, Investments
+from ..._base import _logger
+from .._exceptions import ResourceNotFoundError, InternalServerError
+from .._base_api import APIBackend
+from .._error_messages import BAD_REQUEST_ERROR_INVALID_PERCENTILES
+
+_config = _Config()
+
+
+class PeerGroupAPIBackend(APIBackend):
+    """
+    Subclass to call the Peer Group Data API and handle any HTTP errors that occur.
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def _handle_custom_http_errors(self, res: Any) -> Any:
+        """
+        Handle HTTP errors with custom error messages
+        """
+        response_message = res.json()["message"]
+        if res.status_code == 404:
+            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
+            raise ResourceNotFoundError from None
+
+        if res.status_code == 500:
+            _logger.debug(f"Something went wrong: {res.status_code} {response_message}")
+            raise InternalServerError(response_message) from None
+
+
+_peer_group_api_request = PeerGroupAPIBackend()
+
+
+@dataclass(frozen=True)
+class PeerGroupRequest:
+    investment_source: dict
+    data_points: DataFrame
+    order: Order
+    percentiles: Optional[List[int]] = None
+    methodology: Optional[PeerGroupMethodology] = None
+
+
+@dataclass(frozen=True)
+class PeerGroupResponse:
+    req: PeerGroupRequest
+    breakpoints: list
+
+
+class PeerGroupProvider:
+    def build_request(
+        self,
+        investment_object: Investments,
+        data_point_object: DataPoints,
+        order: Order,
+        percentiles: Optional[List[int]] = None,
+        methodology: Optional[PeerGroupMethodology] = None,
+    ) -> PeerGroupRequest:
+        # do not support dataset id
+        data_point_object.data_set_id = None
+        methodology = _get_methodology_value(methodology)
+        _validate_percentiles(percentiles)
+
+        investment_source = investment_object.generate_investment_source()
+        data_point_data_frame = _get_data_points(data_point_object)
+
+        return PeerGroupRequest(investment_source, data_point_data_frame, order, percentiles, methodology)
+
+    def run_request(self, req: PeerGroupRequest) -> PeerGroupResponse:
+        breakpoints = _get_breakpoints(
+            investment_source=req.investment_source, data_point_data_frame=req.data_points, order=req.order.value, methodology=req.methodology, percentiles=req.percentiles
+        )
+        return PeerGroupResponse(req, breakpoints)
+
+    def build_data_frame(self, resp: PeerGroupResponse) -> DataFrame:
+        return _convert_to_breakpoints_data_frame(resp.breakpoints)
+
+
+def _get_breakpoints(investment_source: dict, data_point_data_frame: DataFrame, order: Any, methodology: Optional[str] = None, percentiles: Optional[list] = None) -> list:
+    breakpoints = []
+    postbody = {"investmentSource": investment_source, "datapoints": data_point_data_frame.to_dict(orient="records"), "percentiles": percentiles, "order": order}
+    url = f"{_config.peergroup_service_url()}peergroupservice/v1/breakpoints"
+    if methodology is not None and len(methodology.strip()) > 0:
+        url = f"{url}?methodology={methodology}"
+    resp = _peer_group_api_request.do_post_request(url, json.dumps(postbody, ignore_nan=True))
+    if resp and isinstance(resp, dict):
+        breakpoints = resp.get("breakpoints", [])
+    return breakpoints
+
+
+def _convert_to_breakpoints_data_frame(breakpoints: list) -> DataFrame:
+    breakpoint_list = []
+    for breakpoint in breakpoints:
+        breakpoint_dict = dict()
+        breakpoint_dict["Alias"] = breakpoint.get("alias", None)
+        time_period = breakpoint.get("timePeriod", dict())
+        breakpoint_dict["StartDate"] = time_period.get("startDate", dict())
+        breakpoint_dict["EndDate"] = time_period.get("endDate", dict())
+        values = breakpoint.get("values", list())
+        for value in values:
+            breakpoint_dict[value.get("percentile", None)] = value.get("value", None)
+        breakpoint_list.append(breakpoint_dict)
+    return DataFrame(breakpoint_list)
+
+
+def _get_methodology_value(methodology: Optional[PeerGroupMethodology] = None) -> Any:
+    if methodology is not None and isinstance(methodology, PeerGroupMethodology):
+        return methodology.value
+    return None
+
+
+def _validate_percentiles(percentiles: Optional[list] = None) -> None:
+    if not percentiles:
+        return
+
+    for per in percentiles:
+        if per is None or not isinstance(per, int) or per < 1 or per > 100:
+            raise BadRequestException(BAD_REQUEST_ERROR_INVALID_PERCENTILES)
+
+
+def _get_data_points(data_point_object: DataPoints) -> DataFrame:
+    data_point_object._validate_data_point_ids_and_alias()
+    return data_point_object.get_peer_group_data_points()
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py` & `morningstar_data-1.3.0/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-from __future__ import annotations
-import simplejson as json
-from typing import List, Optional, Dict, Any
-from pandas import DataFrame
-from ._common import PortfolioJSONEncoder, PortfolioDataApiBackend
-from .._config import _Config
-from .._api import _direct_api_request
-from .._error_messages import BAD_REQUEST_ERROR_NO_PORTFOLIO_HOLDING_ID, BAD_REQUEST_PORTFOLIO_WEIGHT_ERROR, BAD_REQUEST_INVALID_PORTFOLIO_HOLDING_DATA_FRAME
-from .._exceptions import BadRequestException
-from .._utils import _format_date
-from ..._base import _logger
-
-_portfolio_api = PortfolioDataApiBackend()
-_config = _Config()
-
-
-class Holding:
-    holding_id: str
-    weight: Optional[float]
-    market_value: float
-    quantity: float
-    price: float
-
-    def __init__(self, holding_id: str, weight: Optional[float] = None) -> None:
-        self.holding_id = holding_id
-        self.weight = weight
-
-
-class HoldingsEntity:
-    holdings: List[Holding]
-    portfolio_date: str
-    total_amount: float = 10000
-
-    def __init__(self, holdings: List, portfolio_date: str, total_amount: float = 10000) -> None:
-        self.holdings = holdings
-        self.total_amount = total_amount
-        self.portfolio_date = _format_date(portfolio_date)
-
-        self._validate_holdings_id_and_weight()
-        self._validate_holdings_total_weight()
-
-    def _validate_holdings_id_and_weight(self) -> None:
-        """
-        Validate portfolio holdings must have id and weight.
-        """
-        all_weight_is_none = True
-        _logger.info(f"Validating portfolio holdings id and weight")
-        for holding in self.holdings:
-            if not holding.holding_id:
-                # Find out holding without holding id.This is an invalid case.
-                _logger.debug(f"The portfolio date {self.portfolio_date} holdings Holding_Id is missing")
-                raise BadRequestException(BAD_REQUEST_ERROR_NO_PORTFOLIO_HOLDING_ID) from None
-            if holding.weight is not None:
-                all_weight_is_none = False
-
-        if all_weight_is_none:
-            # All holdings without weight.This is an valid case.
-            _logger.info(f"The portfolio date {self.portfolio_date} all holdings weight is none.divide these holding weight by 100.")
-            new_weight = 100 / len(self.holdings)
-            for holding in self.holdings:
-                holding.weight = new_weight
-            _logger.debug(f"The portfolio date {self.portfolio_date} all holdings weight is None,set holdings weight: {new_weight}")
-
-    def _validate_holdings_total_weight(self) -> None:
-        """
-        Validation portfolio holdings total weight must equal 100.0 .
-        """
-        total_weight_error_msg = BAD_REQUEST_PORTFOLIO_WEIGHT_ERROR
-
-        total_weight = sum(c.weight or 0 for c in self.holdings)  # get total weight.
-        _logger.info(f"Validating the portfolio date {self.portfolio_date} holdings total weight: {total_weight}%.")
-        if round(total_weight, 2) > 100:
-            # Holdings total_weight>100.This is an invalid case.
-            error_message = f"The portfolio date: {self.portfolio_date}. {total_weight_error_msg}subtract {round(total_weight - 100, 2)}%."
-            _logger.debug(error_message)
-            raise BadRequestException(error_message) from None
-        if round(total_weight, 2) < 100:
-            # Holdings total_weight<100.This is an invalid case.
-            error_message = f"The portfolio date: {self.portfolio_date}. {total_weight_error_msg}add {round(100 - total_weight, 2)}%."
-            _logger.debug(error_message)
-            raise BadRequestException(error_message) from None
-
-        for holding in self.holdings:  # Set holding market_value with weight.
-            if holding.weight is not None:
-                _logger.info(f"# Set holding market_value with weight.")
-                holding.market_value = self.total_amount * holding.weight / 100
-        return None
-
-    def __str__(self) -> str:
-        return f"{json.dumps(self.to_json(), ignore_nan=True, cls=PortfolioJSONEncoder, ensure_ascii=False)}"
-
-    def to_json(self) -> Dict:
-        # Set holding price and quantity
-        self._set_holding_price_quantity()
-        dict_holdings = []
-        _logger.info(f"Generate holdings entity request json")
-        for holding in self.holdings:
-            dict_holdings.append({"secId": holding.holding_id, "weight": holding.weight, "marketValue": holding.market_value, "quantity": holding.quantity, "price": holding.price})
-        to_return = {"portfolioDate": self.portfolio_date, "holdings": dict_holdings}
-        return to_return
-
-    def _set_holding_price_quantity(self) -> None:
-        """
-        Get and set portfolio holdings price and quantity .
-        """
-        _logger.info("Get and set the portfolio date price for holdings.")
-        post_body = {
-            "priceDate": self.portfolio_date,
-            "investments": list(map(lambda x: {"id": x.holding_id}, self.holdings)),
-        }
-        _logger.debug(f"Get portfolio date price post body..{post_body}")
-        url = f"{_config.securitydata_service_url()}/v1/securities/price"
-        response_json = _portfolio_api.do_post_request(url, json.dumps(post_body, ignore_nan=True))
-        _logger.debug(f"The portfolio date price for holdings..{response_json}")
-
-        _logger.info("Set price and quantity for each holding.")
-        for holding in self.holdings:
-            # Get holding details from response by hoding_id.
-            holding_info = [item for item in response_json if item.get("id") == holding.holding_id]
-            price = float(holding_info[0].get("displayprice", 1))
-            holding.price = price
-            # get quantity by price.
-            holding.quantity = holding.market_value / price
-            _logger.debug(f"The {holding.holding_id} price:{price},quantity:{holding.quantity}")
-
-
-class HoldingsEntityRequestBuilder:
-    portfolio_id: Optional[str]
-
-    def __init__(self, holdings_data_frame: DataFrame) -> None:
-        self.holdings_entitys = self._data_frame_to_holdings_entitys(holdings_data_frame)
-
-    def _data_frame_to_holdings_entitys(self, holdings_data_frame: DataFrame) -> List[HoldingsEntity]:
-        """
-        Convert portfolio holdings dataframe to holdings entitys.
-        """
-        _logger.info("Portfolio holdings dataframe to holdings entitys.")
-        if not set(["Portfolio Date", "HoldingId", "Weight"]).issubset(holdings_data_frame.columns):
-            # Holdings DataFrame columns must have Portfolio Date ,HoldingId, Weight.This is an invalid case.
-            _logger.debug(f"Holdings data frame is missing required columns. It only has :{','.join(holdings_data_frame.columns)}")
-            raise BadRequestException(BAD_REQUEST_INVALID_PORTFOLIO_HOLDING_DATA_FRAME)
-
-        # Group by Portfolio Date
-        portfolio_dates = holdings_data_frame.groupby("Portfolio Date")
-        # holdings dataframe to holdings entitys.
-        holdings_entitys = []
-        for portfolio_date, rows in portfolio_dates:
-            holdings_entitys.append(
-                HoldingsEntity(portfolio_date=portfolio_date, holdings=[(Holding(holding_id=row.HoldingId, weight=row.Weight)) for index, row in rows.iterrows()])
-            )
-        return holdings_entitys
-
-    def update_portfolio_holdings(self) -> Any:
-        """
-        Update portfolio holdings with holdings entitys.
-        """
-        _logger.info("Saving holdings to portfolio.")
-        _logger.debug(f"Portfolio id: {self.portfolio_id}")
-        url = f"{_config.portfolio_service_url()}portfoliodataservice/v1/portfolios/{self.portfolio_id}/holdings"
-        response_json = _portfolio_api.do_post_request(url, json.dumps(self.holdings_entitys, cls=PortfolioJSONEncoder, ignore_nan=True))
-        _logger.debug("Update portfolio holdings response:{response}")
-        return response_json
+from __future__ import annotations
+import simplejson as json
+from typing import List, Optional, Dict, Any
+from pandas import DataFrame
+from ._common import PortfolioJSONEncoder, PortfolioDataApiBackend
+from .._config import _Config
+from .._api import _direct_api_request
+from .._error_messages import BAD_REQUEST_ERROR_NO_PORTFOLIO_HOLDING_ID, BAD_REQUEST_PORTFOLIO_WEIGHT_ERROR, BAD_REQUEST_INVALID_PORTFOLIO_HOLDING_DATA_FRAME
+from .._exceptions import BadRequestException
+from .._utils import _format_date
+from ..._base import _logger
+
+_portfolio_api = PortfolioDataApiBackend()
+_config = _Config()
+
+
+class Holding:
+    holding_id: str
+    weight: Optional[float]
+    market_value: float
+    quantity: float
+    price: float
+
+    def __init__(self, holding_id: str, weight: Optional[float] = None) -> None:
+        self.holding_id = holding_id
+        self.weight = weight
+
+
+class HoldingsEntity:
+    holdings: List[Holding]
+    portfolio_date: str
+    total_amount: float = 10000
+
+    def __init__(self, holdings: List, portfolio_date: str, total_amount: float = 10000) -> None:
+        self.holdings = holdings
+        self.total_amount = total_amount
+        self.portfolio_date = _format_date(portfolio_date)
+
+        self._validate_holdings_id_and_weight()
+        self._validate_holdings_total_weight()
+
+    def _validate_holdings_id_and_weight(self) -> None:
+        """
+        Validate portfolio holdings must have id and weight.
+        """
+        all_weight_is_none = True
+        _logger.info(f"Validating portfolio holdings id and weight")
+        for holding in self.holdings:
+            if not holding.holding_id:
+                # Find out holding without holding id.This is an invalid case.
+                _logger.debug(f"The portfolio date {self.portfolio_date} holdings Holding_Id is missing")
+                raise BadRequestException(BAD_REQUEST_ERROR_NO_PORTFOLIO_HOLDING_ID) from None
+            if holding.weight is not None:
+                all_weight_is_none = False
+
+        if all_weight_is_none:
+            # All holdings without weight.This is an valid case.
+            _logger.info(f"The portfolio date {self.portfolio_date} all holdings weight is none.divide these holding weight by 100.")
+            new_weight = 100 / len(self.holdings)
+            for holding in self.holdings:
+                holding.weight = new_weight
+            _logger.debug(f"The portfolio date {self.portfolio_date} all holdings weight is None,set holdings weight: {new_weight}")
+
+    def _validate_holdings_total_weight(self) -> None:
+        """
+        Validation portfolio holdings total weight must equal 100.0 .
+        """
+        total_weight_error_msg = BAD_REQUEST_PORTFOLIO_WEIGHT_ERROR
+
+        total_weight = sum(c.weight or 0 for c in self.holdings)  # get total weight.
+        _logger.info(f"Validating the portfolio date {self.portfolio_date} holdings total weight: {total_weight}%.")
+        if round(total_weight, 2) > 100:
+            # Holdings total_weight>100.This is an invalid case.
+            error_message = f"The portfolio date: {self.portfolio_date}. {total_weight_error_msg}subtract {round(total_weight - 100, 2)}%."
+            _logger.debug(error_message)
+            raise BadRequestException(error_message) from None
+        if round(total_weight, 2) < 100:
+            # Holdings total_weight<100.This is an invalid case.
+            error_message = f"The portfolio date: {self.portfolio_date}. {total_weight_error_msg}add {round(100 - total_weight, 2)}%."
+            _logger.debug(error_message)
+            raise BadRequestException(error_message) from None
+
+        for holding in self.holdings:  # Set holding market_value with weight.
+            if holding.weight is not None:
+                _logger.info(f"# Set holding market_value with weight.")
+                holding.market_value = self.total_amount * holding.weight / 100
+        return None
+
+    def __str__(self) -> str:
+        return f"{json.dumps(self.to_json(), ignore_nan=True, cls=PortfolioJSONEncoder, ensure_ascii=False)}"
+
+    def to_json(self) -> Dict:
+        # Set holding price and quantity
+        self._set_holding_price_quantity()
+        dict_holdings = []
+        _logger.info(f"Generate holdings entity request json")
+        for holding in self.holdings:
+            dict_holdings.append({"secId": holding.holding_id, "weight": holding.weight, "marketValue": holding.market_value, "quantity": holding.quantity, "price": holding.price})
+        to_return = {"portfolioDate": self.portfolio_date, "holdings": dict_holdings}
+        return to_return
+
+    def _set_holding_price_quantity(self) -> None:
+        """
+        Get and set portfolio holdings price and quantity .
+        """
+        _logger.info("Get and set the portfolio date price for holdings.")
+        post_body = {
+            "priceDate": self.portfolio_date,
+            "investments": list(map(lambda x: {"id": x.holding_id}, self.holdings)),
+        }
+        _logger.debug(f"Get portfolio date price post body..{post_body}")
+        url = f"{_config.securitydata_service_url()}/v1/securities/price"
+        response_json = _portfolio_api.do_post_request(url, json.dumps(post_body, ignore_nan=True))
+        _logger.debug(f"The portfolio date price for holdings..{response_json}")
+
+        _logger.info("Set price and quantity for each holding.")
+        for holding in self.holdings:
+            # Get holding details from response by hoding_id.
+            holding_info = [item for item in response_json if item.get("id") == holding.holding_id]
+            price = float(holding_info[0].get("displayprice", 1))
+            holding.price = price
+            # get quantity by price.
+            holding.quantity = holding.market_value / price
+            _logger.debug(f"The {holding.holding_id} price:{price},quantity:{holding.quantity}")
+
+
+class HoldingsEntityRequestBuilder:
+    portfolio_id: Optional[str]
+
+    def __init__(self, holdings_data_frame: DataFrame) -> None:
+        self.holdings_entitys = self._data_frame_to_holdings_entitys(holdings_data_frame)
+
+    def _data_frame_to_holdings_entitys(self, holdings_data_frame: DataFrame) -> List[HoldingsEntity]:
+        """
+        Convert portfolio holdings dataframe to holdings entitys.
+        """
+        _logger.info("Portfolio holdings dataframe to holdings entitys.")
+        if not set(["Portfolio Date", "HoldingId", "Weight"]).issubset(holdings_data_frame.columns):
+            # Holdings DataFrame columns must have Portfolio Date ,HoldingId, Weight.This is an invalid case.
+            _logger.debug(f"Holdings data frame is missing required columns. It only has :{','.join(holdings_data_frame.columns)}")
+            raise BadRequestException(BAD_REQUEST_INVALID_PORTFOLIO_HOLDING_DATA_FRAME)
+
+        # Group by Portfolio Date
+        portfolio_dates = holdings_data_frame.groupby("Portfolio Date")
+        # holdings dataframe to holdings entitys.
+        holdings_entitys = []
+        for portfolio_date, rows in portfolio_dates:
+            holdings_entitys.append(
+                HoldingsEntity(portfolio_date=portfolio_date, holdings=[(Holding(holding_id=row.HoldingId, weight=row.Weight)) for index, row in rows.iterrows()])
+            )
+        return holdings_entitys
+
+    def update_portfolio_holdings(self) -> Any:
+        """
+        Update portfolio holdings with holdings entitys.
+        """
+        _logger.info("Saving holdings to portfolio.")
+        _logger.debug(f"Portfolio id: {self.portfolio_id}")
+        url = f"{_config.portfolio_service_url()}portfoliodataservice/v1/portfolios/{self.portfolio_id}/holdings"
+        response_json = _portfolio_api.do_post_request(url, json.dumps(self.holdings_entitys, cls=PortfolioJSONEncoder, ignore_nan=True))
+        _logger.debug("Update portfolio holdings response:{response}")
+        return response_json
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_portfolio/_portfolio_settings.py` & `morningstar_data-1.3.0/morningstar_data/direct/_portfolio/_portfolio_settings.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,204 +1,204 @@
-import dataclasses
-import simplejson as json
-import uuid
-from enum import Enum
-from typing import Any, Dict, Optional, List
-from ._common import PortfolioDataApiBackend
-from .._config import _Config
-from ..._base import _logger
-
-_portfolio_api = PortfolioDataApiBackend()
-_config = _Config()
-
-
-class PerformanceSource(Enum):
-    Calculated_Based_On_Underlying_Positions = 1
-    Imported_Account_Level_Performance = 2
-
-
-class RebalanceOnType(Enum):
-    Calendar_Period_End = 0
-    Rolling_Period_Based_On_Portfolio_Date = 1
-
-
-class RebalanceFrequency(Enum):
-    Monthly = 2
-    Quarterly = 3
-    Semi_Annually = 4
-    Annually = 5
-    Buy_And_Hold = 7
-    Daily = 8
-
-
-class CalculationType(Enum):
-    Earliest_Common = 1
-    First_Portfolio_Date = 2
-    Earliest_Available = 3
-
-
-class PerformanceSeriesFrequency(Enum):
-    Monthly = 4
-    Quarterly = 5
-    Daily = 6
-
-
-class ManagementFeeEffectivePeriodType(Enum):
-    Entire_Period = 0
-    Custom_Period = 1
-
-
-class ManagementFeeFrequency(Enum):
-    Daily = 1
-    Monthly = 2
-    Quarterly = 3
-    Semi_Annually = 4
-    Annually = 5
-
-
-class BenchmarkType(Enum):
-    Morningstar_Security = 1
-    User_Defined_Security = 2
-
-
-class MissingTNAHandling(Enum):
-    Roll_Previous_Value_Forward = 1
-    Infer_Forward_In_Time = 2
-    Infer_Backward_In_Time = 3
-
-
-class Benchmark:
-    benchmark_id: str
-    benchmark_type_id: int = 1
-    investment_id: str
-
-    def __init__(self, investment_id: str, benchmark_id: str) -> None:
-        self.investment_id = investment_id
-        self.benchmark_type_id = 1
-        self.benchmark_id = benchmark_id
-
-
-class PortfolioSetting:
-    notes: None
-    benchmark_id: str
-    missing_tna_handling_id: MissingTNAHandling = MissingTNAHandling.Infer_Forward_In_Time
-    management_fee_effective_period_type: ManagementFeeEffectivePeriodType = ManagementFeeEffectivePeriodType.Entire_Period
-    management_fee_frequency: ManagementFeeFrequency = ManagementFeeFrequency.Annually
-    management_fee_for_performance: Optional[float] = None
-    risk_free_proxy_id: str = "XIUSA000OC"
-    rebalance_frequency_id: RebalanceFrequency = RebalanceFrequency.Buy_And_Hold
-    start_date_calculation_type_id: CalculationType = CalculationType.First_Portfolio_Date
-    rebalance_based_on: RebalanceOnType = RebalanceOnType.Calendar_Period_End
-    performance_source_id: PerformanceSource = PerformanceSource.Calculated_Based_On_Underlying_Positions
-    performance_series_frequency_id: PerformanceSeriesFrequency = PerformanceSeriesFrequency.Quarterly
-    portfolio_to_id: None
-    model_portfolio_id: None
-    model_portfolio_name: None
-    use_gross_return: bool = False
-    real_sma_flag: bool = False
-    is_combined_series: bool = False
-    combined_series: None
-    base_currency: str = "USD"
-    secondary_benchmark_id: str = "XIUSA04FMS"
-    portfolio_type: Optional[str]
-    portfolio_id: Optional[str]
-    name: Optional[str]
-    benchmarks: List[Benchmark]
-
-    def __init__(
-        self,
-        name: Optional[str] = None,
-        portfolio_type: Optional[str] = None,
-        portfolio_id: Optional[str] = None,
-    ) -> None:
-        """
-        Build portfolio settings with default value.
-        """
-        self.notes = None
-        self.benchmark_id = "XIUSA04G92"
-        self.missing_tna_handling_id = MissingTNAHandling.Infer_Forward_In_Time
-        self.management_fee_effective_period_type = ManagementFeeEffectivePeriodType.Entire_Period
-        self.management_fee_frequency = ManagementFeeFrequency.Annually
-        self.management_fee_for_performance = None
-        self.risk_free_proxy_id = "XIUSA000OC"
-        self.rebalance_frequency_id = RebalanceFrequency.Buy_And_Hold
-        self.start_date_calculation_type_id = CalculationType.First_Portfolio_Date
-        self.rebalance_based_on = RebalanceOnType.Calendar_Period_End
-        self.performance_source_id = PerformanceSource.Calculated_Based_On_Underlying_Positions
-        self.performance_series_frequency_id = PerformanceSeriesFrequency.Quarterly
-        self.portfolio_to_id = None
-        self.model_portfolio_id = None
-        self.model_portfolio_name = None
-        self.use_gross_return = False
-        self.real_sma_flag = False
-        self.is_combined_series = False
-        self.combined_series = None
-        self.base_currency = "USD"
-        self.secondary_benchmark_id = "XIUSA04FMS"
-        self.portfolio_type = portfolio_type
-        self.portfolio_id = portfolio_id
-        self.name = name
-
-    def get_formatted_json_body(self) -> Dict[Any, Any]:
-        """
-        Build portfolio settings post body.
-        """
-        # Generate portfolio benchmark objects request dict.
-        _logger.info("Generate portfolio benchmark objects request.")
-        benchmark_uuid = str(uuid.uuid4())
-        secondary_benchmark_uuid = str(uuid.uuid4())
-        risk_free_proxy_uuid = str(uuid.uuid4())
-
-        # Each benchmarks need a UUID.
-        self.benchmarks = [
-            Benchmark(self.benchmark_id, benchmark_uuid),
-            Benchmark(self.secondary_benchmark_id, secondary_benchmark_uuid),
-            Benchmark(self.risk_free_proxy_id, risk_free_proxy_uuid),
-        ]
-
-        benchmarks = []
-        # Generate benchmark dict list.
-        for benchmark in self.benchmarks:
-            benchmarks.append({"securityId": benchmark.investment_id, "benchmarkTypeId": benchmark.benchmark_type_id, "benchmarkId": benchmark.benchmark_id})
-        # Generate portfolio settings with default values .
-        _logger.info("Generate portfolio settings with default values")
-        to_return = {
-            "settings": {
-                "portfolio": {
-                    "portfolioType": self.portfolio_type,
-                    "notes": self.notes,
-                    "portfolioId": self.portfolio_id,
-                    "benchmarkId": benchmark_uuid,
-                    "baseCurrency": self.base_currency,
-                    "missingTNAHandlingId": self.missing_tna_handling_id.value,
-                    "managementFeeEffectivePeriodType": self.management_fee_effective_period_type.value,
-                    "managementFeeFrequency": self.management_fee_frequency.value,
-                    "managementFeeForPerformance": self.management_fee_for_performance,
-                    "riskFreeProxyId": secondary_benchmark_uuid,
-                    "rebalanceFrequencyId": self.rebalance_frequency_id.value,
-                    "secondaryBenchmarkId": risk_free_proxy_uuid,
-                    "startDateCalculationTypeId": self.start_date_calculation_type_id.value,
-                    "rebalanceBasedOn": self.rebalance_based_on.value,
-                    "performanceSourceId": self.performance_source_id.value,
-                    "performanceSeriesFrequencyId": self.performance_series_frequency_id.value,
-                    "portfolio2Id": self.portfolio_to_id,
-                    "modelPortfolioId": self.model_portfolio_id,
-                    "modelPortfolioName": self.model_portfolio_name,
-                    "useGrossReturn": self.use_gross_return,
-                    "realSMAFlag": self.real_sma_flag,
-                    "isCombinedSeries": self.is_combined_series,
-                    "combinedSeries": self.combined_series,
-                    "name": self.name,
-                },
-                "benchmarks": benchmarks,
-            }
-        }
-        _logger.debug(f"Generate portfolio settings with default values. {to_return}")
-        return to_return
-
-    def save_portfolio_settings(self) -> Any:
-
-        url = f"{_config.portfolio_service_url()}portfoliodataservice/v1/portfolios/update-portfolio-settings"
-        _logger.debug(f"Save portfolio settings with portfolio API: {url}")
-        response_json = _portfolio_api.do_post_request(url, json.dumps(self.get_formatted_json_body(), ignore_nan=True))
-        _logger.debug(f"Save portfolio API response: {response_json}")
-        return response_json
+import dataclasses
+import simplejson as json
+import uuid
+from enum import Enum
+from typing import Any, Dict, Optional, List
+from ._common import PortfolioDataApiBackend
+from .._config import _Config
+from ..._base import _logger
+
+_portfolio_api = PortfolioDataApiBackend()
+_config = _Config()
+
+
+class PerformanceSource(Enum):
+    Calculated_Based_On_Underlying_Positions = 1
+    Imported_Account_Level_Performance = 2
+
+
+class RebalanceOnType(Enum):
+    Calendar_Period_End = 0
+    Rolling_Period_Based_On_Portfolio_Date = 1
+
+
+class RebalanceFrequency(Enum):
+    Monthly = 2
+    Quarterly = 3
+    Semi_Annually = 4
+    Annually = 5
+    Buy_And_Hold = 7
+    Daily = 8
+
+
+class CalculationType(Enum):
+    Earliest_Common = 1
+    First_Portfolio_Date = 2
+    Earliest_Available = 3
+
+
+class PerformanceSeriesFrequency(Enum):
+    Monthly = 4
+    Quarterly = 5
+    Daily = 6
+
+
+class ManagementFeeEffectivePeriodType(Enum):
+    Entire_Period = 0
+    Custom_Period = 1
+
+
+class ManagementFeeFrequency(Enum):
+    Daily = 1
+    Monthly = 2
+    Quarterly = 3
+    Semi_Annually = 4
+    Annually = 5
+
+
+class BenchmarkType(Enum):
+    Morningstar_Security = 1
+    User_Defined_Security = 2
+
+
+class MissingTNAHandling(Enum):
+    Roll_Previous_Value_Forward = 1
+    Infer_Forward_In_Time = 2
+    Infer_Backward_In_Time = 3
+
+
+class Benchmark:
+    benchmark_id: str
+    benchmark_type_id: int = 1
+    investment_id: str
+
+    def __init__(self, investment_id: str, benchmark_id: str) -> None:
+        self.investment_id = investment_id
+        self.benchmark_type_id = 1
+        self.benchmark_id = benchmark_id
+
+
+class PortfolioSetting:
+    notes: None
+    benchmark_id: str
+    missing_tna_handling_id: MissingTNAHandling = MissingTNAHandling.Infer_Forward_In_Time
+    management_fee_effective_period_type: ManagementFeeEffectivePeriodType = ManagementFeeEffectivePeriodType.Entire_Period
+    management_fee_frequency: ManagementFeeFrequency = ManagementFeeFrequency.Annually
+    management_fee_for_performance: Optional[float] = None
+    risk_free_proxy_id: str = "XIUSA000OC"
+    rebalance_frequency_id: RebalanceFrequency = RebalanceFrequency.Buy_And_Hold
+    start_date_calculation_type_id: CalculationType = CalculationType.First_Portfolio_Date
+    rebalance_based_on: RebalanceOnType = RebalanceOnType.Calendar_Period_End
+    performance_source_id: PerformanceSource = PerformanceSource.Calculated_Based_On_Underlying_Positions
+    performance_series_frequency_id: PerformanceSeriesFrequency = PerformanceSeriesFrequency.Quarterly
+    portfolio_to_id: None
+    model_portfolio_id: None
+    model_portfolio_name: None
+    use_gross_return: bool = False
+    real_sma_flag: bool = False
+    is_combined_series: bool = False
+    combined_series: None
+    base_currency: str = "USD"
+    secondary_benchmark_id: str = "XIUSA04FMS"
+    portfolio_type: Optional[str]
+    portfolio_id: Optional[str]
+    name: Optional[str]
+    benchmarks: List[Benchmark]
+
+    def __init__(
+        self,
+        name: Optional[str] = None,
+        portfolio_type: Optional[str] = None,
+        portfolio_id: Optional[str] = None,
+    ) -> None:
+        """
+        Build portfolio settings with default value.
+        """
+        self.notes = None
+        self.benchmark_id = "XIUSA04G92"
+        self.missing_tna_handling_id = MissingTNAHandling.Infer_Forward_In_Time
+        self.management_fee_effective_period_type = ManagementFeeEffectivePeriodType.Entire_Period
+        self.management_fee_frequency = ManagementFeeFrequency.Annually
+        self.management_fee_for_performance = None
+        self.risk_free_proxy_id = "XIUSA000OC"
+        self.rebalance_frequency_id = RebalanceFrequency.Buy_And_Hold
+        self.start_date_calculation_type_id = CalculationType.First_Portfolio_Date
+        self.rebalance_based_on = RebalanceOnType.Calendar_Period_End
+        self.performance_source_id = PerformanceSource.Calculated_Based_On_Underlying_Positions
+        self.performance_series_frequency_id = PerformanceSeriesFrequency.Quarterly
+        self.portfolio_to_id = None
+        self.model_portfolio_id = None
+        self.model_portfolio_name = None
+        self.use_gross_return = False
+        self.real_sma_flag = False
+        self.is_combined_series = False
+        self.combined_series = None
+        self.base_currency = "USD"
+        self.secondary_benchmark_id = "XIUSA04FMS"
+        self.portfolio_type = portfolio_type
+        self.portfolio_id = portfolio_id
+        self.name = name
+
+    def get_formatted_json_body(self) -> Dict[Any, Any]:
+        """
+        Build portfolio settings post body.
+        """
+        # Generate portfolio benchmark objects request dict.
+        _logger.info("Generate portfolio benchmark objects request.")
+        benchmark_uuid = str(uuid.uuid4())
+        secondary_benchmark_uuid = str(uuid.uuid4())
+        risk_free_proxy_uuid = str(uuid.uuid4())
+
+        # Each benchmarks need a UUID.
+        self.benchmarks = [
+            Benchmark(self.benchmark_id, benchmark_uuid),
+            Benchmark(self.secondary_benchmark_id, secondary_benchmark_uuid),
+            Benchmark(self.risk_free_proxy_id, risk_free_proxy_uuid),
+        ]
+
+        benchmarks = []
+        # Generate benchmark dict list.
+        for benchmark in self.benchmarks:
+            benchmarks.append({"securityId": benchmark.investment_id, "benchmarkTypeId": benchmark.benchmark_type_id, "benchmarkId": benchmark.benchmark_id})
+        # Generate portfolio settings with default values .
+        _logger.info("Generate portfolio settings with default values")
+        to_return = {
+            "settings": {
+                "portfolio": {
+                    "portfolioType": self.portfolio_type,
+                    "notes": self.notes,
+                    "portfolioId": self.portfolio_id,
+                    "benchmarkId": benchmark_uuid,
+                    "baseCurrency": self.base_currency,
+                    "missingTNAHandlingId": self.missing_tna_handling_id.value,
+                    "managementFeeEffectivePeriodType": self.management_fee_effective_period_type.value,
+                    "managementFeeFrequency": self.management_fee_frequency.value,
+                    "managementFeeForPerformance": self.management_fee_for_performance,
+                    "riskFreeProxyId": secondary_benchmark_uuid,
+                    "rebalanceFrequencyId": self.rebalance_frequency_id.value,
+                    "secondaryBenchmarkId": risk_free_proxy_uuid,
+                    "startDateCalculationTypeId": self.start_date_calculation_type_id.value,
+                    "rebalanceBasedOn": self.rebalance_based_on.value,
+                    "performanceSourceId": self.performance_source_id.value,
+                    "performanceSeriesFrequencyId": self.performance_series_frequency_id.value,
+                    "portfolio2Id": self.portfolio_to_id,
+                    "modelPortfolioId": self.model_portfolio_id,
+                    "modelPortfolioName": self.model_portfolio_name,
+                    "useGrossReturn": self.use_gross_return,
+                    "realSMAFlag": self.real_sma_flag,
+                    "isCombinedSeries": self.is_combined_series,
+                    "combinedSeries": self.combined_series,
+                    "name": self.name,
+                },
+                "benchmarks": benchmarks,
+            }
+        }
+        _logger.debug(f"Generate portfolio settings with default values. {to_return}")
+        return to_return
+
+    def save_portfolio_settings(self) -> Any:
+
+        url = f"{_config.portfolio_service_url()}portfoliodataservice/v1/portfolios/update-portfolio-settings"
+        _logger.debug(f"Save portfolio settings with portfolio API: {url}")
+        response_json = _portfolio_api.do_post_request(url, json.dumps(self.get_formatted_json_body(), ignore_nan=True))
+        _logger.debug(f"Save portfolio API response: {response_json}")
+        return response_json
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_portfolio_data_set.py` & `morningstar_data-1.3.0/morningstar_data/direct/_portfolio_data_set.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,191 +1,191 @@
-from __future__ import annotations
-import datetime
-import simplejson as json
-from enum import Enum
-from sre_constants import ANY
-from typing import Any, Dict
-
-from pandas import DataFrame
-
-from ._api import _direct_api_request, _config
-
-
-def _annual_return_year(year: int = 0) -> str:
-    current_date = datetime.date.today()
-    new_year = current_date.year - year
-    return str(new_year)
-
-
-def _update_annual_return_alias(data_point_id: str) -> str:
-    maps = {"AR002": 1, "AR003": 2, "AR004": 3, "AR005": 4, "AR006": 5, "AR007": 6, "AR008": 7, "AR009": 8, "AR00A": 9, "AR00B": 10, "AR00C": 11}
-    map_value = maps.get(data_point_id, None)
-    if map_value is not None:
-        return _annual_return_year(map_value)
-    else:
-        return ""
-
-
-def _get_data_sets() -> DataFrame:
-    url = f"{_config.asset_service_url()}/portfolio/datasets"
-    response_json = _direct_api_request("get", url)
-    return DataFrame(response_json)
-
-
-def _get_data_set_with_id(data_set_id: str) -> Any:
-    try:
-        if data_set_id is not None:
-            url = f"{_config.asset_service_url()}portfolio/dataset/{data_set_id}"
-            response_json = _direct_api_request("get", url)
-    except Exception:
-        response_json = {"datapoints": []}
-    response_json = _update_calendar_year_data_points_name(response_json)
-    return response_json
-
-
-def _update_calendar_year_data_points_name(response_json: Any) -> Any:
-    data_set_id = response_json.get("id", None)
-    if data_set_id is not None and PortfolioDataSet.get(str(data_set_id)) == PortfolioDataSet.Returns_Calendar_Year:
-        data_points = response_json.get("datapoints", [])
-        for data_point in data_points:
-            new_alias = f'{data_point.get("alias", "").strip()} {_update_annual_return_alias(data_point.get("datapointId"))}'
-            data_point["alias"] = new_alias
-    return response_json
-
-
-def _get_data_points_default_settings(data_points: list) -> Dict[str, dict]:
-    url = f"{_config.asset_service_url()}portfolio/datapoints"
-    post_body = list(map(lambda x: {"datapointId": x}, data_points))
-    response_json = _direct_api_request("post", url, json.dumps(post_body, ignore_nan=True))
-    defined_data_points = {x.get("datapointId"): x for x in response_json}
-    return defined_data_points
-
-
-class DataSetType(Enum):
-    Current = 1
-    TimeSeries = 2
-    Current_Or_TimeSeries = 3
-    Custom_Calculation = 4
-    No_Map = 0
-
-
-class PortfolioDataSet(Enum):
-    def __init__(self, data_set_id: str, data_set_type: DataSetType) -> None:
-        self.data_set_type = data_set_type
-        self.data_set_id = data_set_id
-
-    @classmethod
-    def get(cls, data_set_id: str) -> Any:
-        for member in cls._member_map_.values():
-            if member._value_[0] == data_set_id:
-                return member
-        return PortfolioDataSet["No_Map"]
-
-    @classmethod
-    def get_data_set_type(cls, data_set_id: str) -> Any:
-        for member in cls._member_map_.values():
-            if member._value_[0] == data_set_id:
-                return member._value_[1]
-        return DataSetType["No_Map"]
-
-    No_Map = ("no_map", DataSetType.No_Map)
-    Asset_Allocation = ("99", DataSetType.Current_Or_TimeSeries)
-    Custom_Calculation = ("8", DataSetType.Custom_Calculation)
-    Daily_Gross_Return_Index = ("7", DataSetType.TimeSeries)
-    Daily_Return_Index = ("6", DataSetType.TimeSeries)
-    Equity_Country_Exposure = ("15", DataSetType.Current_Or_TimeSeries)
-    Equity_Market_Capitalization = ("25", DataSetType.Current_Or_TimeSeries)
-    Equity_Port_Stats_Long = ("27", DataSetType.Current_Or_TimeSeries)
-    Equity_Port_Stats_Short = ("28", DataSetType.Current_Or_TimeSeries)
-    Equity_Regional_Exposure = ("21", DataSetType.Current_Or_TimeSeries)
-    Equity_Sector_Exposure = ("17", DataSetType.Current_Or_TimeSeries)
-    Equity_Style_Analysis = ("24", DataSetType.Current_Or_TimeSeries)
-    Equity_Style_Capitalization = ("22", DataSetType.Current_Or_TimeSeries)
-    Equity_Style_Valuation = ("23", DataSetType.Current_Or_TimeSeries)
-    Equity_Type = ("19", DataSetType.TimeSeries)
-    ESG_Carbon = ("12", DataSetType.Current_Or_TimeSeries)
-    ESG_Product_Involvement = ("13", DataSetType.Current_Or_TimeSeries)
-    ESG_Sustainability = ("14", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_ABS_Collateral_Type_Detail = ("34", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Bond_Insurer = ("71", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Call_Type = ("35", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_CMO_Issuer_Type = ("36", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_CMO_Payment_Type = ("37", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_CMO_Tranche_Type = ("38", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Convertible_Type = ("43", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Country_Exposure = ("29", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Coupon_Type = ("44", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Credit_Enhancement_Type = ("67", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Credit_Grd_And_Credit_Rtg_Breakdown_Detail = ("77", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_CreditQualityBreakdown = ("68", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Credit_Rtg = ("76", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Current_Yield_And_Current_Yield_Breakdown_Detail = ("85", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Default_Reason = ("61", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Default_Type = ("62", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_DTW_Breakdown_Super = ("82", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_DTW_And_DTW_Breakdown_Detail = ("75", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Duration_Effective = ("39", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Duration_Modified_to_maturity = ("40", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Eff_Convxty_breakdown_Super = ("84", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_EFF_Convxty_And_Convxty_Breakdown_Detail = ("73", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Eff_Dua_Breakdown_Super = ("78", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Effective_Maturity = ("41", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Eff_Mty_Breakdown_Super = ("80", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Geographic_Exposure = ("93", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Guarantee_Type = ("63", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Guarantor_Type = ("64", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Interest_Rate_Type_Detail = ("45", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Issuer_Type = ("46", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Issuer_Type_Breakdown_Super = ("90", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_LOC_Type = ("65", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Maturity_Type = ("47", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_MBS_Agency = ("48", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Mbs_Agency_Breakdown_Super = ("87", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_MBS_Collateral_Type = ("49", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Mod_Dur_Breakdown_Super = ("79", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Morningstar_Sectors = ("94", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Municipal_Security_Type_Breakdown = ("92", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Municipal_Security_Type_Breakdown_Super = ("88", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Next_Call_And_Next_Call_Breakdown_Detail = ("86", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_OAS_Breakdown_Super = ("83", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_OAS_And_OAS_Breakdown_Detail = ("72", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_PIK_Type = ("50", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Portfolio_Statistics = ("33", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Pre_refunded_ETM_Type = ("66", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Primary_Sector_Breakdown = ("32", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Put_Type = ("51", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Put_Type_Detail = ("52", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Secondary_Sector_Breakdown = ("30", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_SEC_Registration_Type = ("53", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Secured_by_Collateral_Type = ("54", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Securitization_Collateral_Type = ("69", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Securitized_Mortgage_Type = ("55", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Security_Rank = ("56", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Security_Rank_Breakdown_Super = ("91", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Sinking_Fund_Type = ("57", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_State_Taxation = ("58", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Structured_Securitized_Type = ("59", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Super_Sector_Breakdown = ("31", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Use_of_Proceeds = ("70", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Use_Of_Proceeds_Breakdown_Super = ("89", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_US_Federal_Taxation = ("60", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_Yield_to_Maturity_YTM = ("42", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_YTM_Breakdown_Super = ("81", DataSetType.Current_Or_TimeSeries)
-    Fixed_Income_YTW_And_YTW_Breakdown_Detail = ("74", DataSetType.Current_Or_TimeSeries)
-    GICS_Equity_Industry = ("20", DataSetType.Current_Or_TimeSeries)
-    GICS_Equity_Sector_Exposure = ("18", DataSetType.Current_Or_TimeSeries)
-    MSCI_Equity_Country_Exposure = ("16", DataSetType.Current_Or_TimeSeries)
-    Post_tax_Returns_Month_end = ("9", DataSetType.Current_Or_TimeSeries)
-    Regional_Asset_Class_Market_Cap = ("95", DataSetType.Current)
-    Representative_Cost = ("96", DataSetType.Current_Or_TimeSeries)
-    Returns_Calendar_Year = ("5", DataSetType.Current)
-    Returns_Daily = ("2", DataSetType.Current)
-    Returns_Month_End = ("3", DataSetType.Current)
-    Returns_Quarter_End = ("4", DataSetType.Current)
-    Risk_Total_ReturnMonth_End = ("10", DataSetType.Current_Or_TimeSeries)
-    Risk_Total_ReturnQtr_End = ("11", DataSetType.Current_Or_TimeSeries)
-    Snapshot = ("1", DataSetType.Current)
-    South_Africa_Asset_Allocation = ("101", DataSetType.Current_Or_TimeSeries)
-    Stock_Intersection = ("26", DataSetType.Current_Or_TimeSeries)
-    Surveyed_Asset_Allocation_AUS = ("97", DataSetType.Current_Or_TimeSeries)
-    Surveyed_Asset_Allocation_CAN = ("98", DataSetType.Current_Or_TimeSeries)
-    Surveyed_Asset_Allocation_NZ = ("100", DataSetType.Current_Or_TimeSeries)
+from __future__ import annotations
+import datetime
+import simplejson as json
+from enum import Enum
+from sre_constants import ANY
+from typing import Any, Dict
+
+from pandas import DataFrame
+
+from ._api import _direct_api_request, _config
+
+
+def _annual_return_year(year: int = 0) -> str:
+    current_date = datetime.date.today()
+    new_year = current_date.year - year
+    return str(new_year)
+
+
+def _update_annual_return_alias(data_point_id: str) -> str:
+    maps = {"AR002": 1, "AR003": 2, "AR004": 3, "AR005": 4, "AR006": 5, "AR007": 6, "AR008": 7, "AR009": 8, "AR00A": 9, "AR00B": 10, "AR00C": 11}
+    map_value = maps.get(data_point_id, None)
+    if map_value is not None:
+        return _annual_return_year(map_value)
+    else:
+        return ""
+
+
+def _get_data_sets() -> DataFrame:
+    url = f"{_config.asset_service_url()}/portfolio/datasets"
+    response_json = _direct_api_request("get", url)
+    return DataFrame(response_json)
+
+
+def _get_data_set_with_id(data_set_id: str) -> Any:
+    try:
+        if data_set_id is not None:
+            url = f"{_config.asset_service_url()}portfolio/dataset/{data_set_id}"
+            response_json = _direct_api_request("get", url)
+    except Exception:
+        response_json = {"datapoints": []}
+    response_json = _update_calendar_year_data_points_name(response_json)
+    return response_json
+
+
+def _update_calendar_year_data_points_name(response_json: Any) -> Any:
+    data_set_id = response_json.get("id", None)
+    if data_set_id is not None and PortfolioDataSet.get(str(data_set_id)) == PortfolioDataSet.Returns_Calendar_Year:
+        data_points = response_json.get("datapoints", [])
+        for data_point in data_points:
+            new_alias = f'{data_point.get("alias", "").strip()} {_update_annual_return_alias(data_point.get("datapointId"))}'
+            data_point["alias"] = new_alias
+    return response_json
+
+
+def _get_data_points_default_settings(data_points: list) -> Dict[str, dict]:
+    url = f"{_config.asset_service_url()}portfolio/datapoints"
+    post_body = list(map(lambda x: {"datapointId": x}, data_points))
+    response_json = _direct_api_request("post", url, json.dumps(post_body, ignore_nan=True))
+    defined_data_points = {x.get("datapointId"): x for x in response_json}
+    return defined_data_points
+
+
+class DataSetType(Enum):
+    Current = 1
+    TimeSeries = 2
+    Current_Or_TimeSeries = 3
+    Custom_Calculation = 4
+    No_Map = 0
+
+
+class PortfolioDataSet(Enum):
+    def __init__(self, data_set_id: str, data_set_type: DataSetType) -> None:
+        self.data_set_type = data_set_type
+        self.data_set_id = data_set_id
+
+    @classmethod
+    def get(cls, data_set_id: str) -> Any:
+        for member in cls._member_map_.values():
+            if member._value_[0] == data_set_id:
+                return member
+        return PortfolioDataSet["No_Map"]
+
+    @classmethod
+    def get_data_set_type(cls, data_set_id: str) -> Any:
+        for member in cls._member_map_.values():
+            if member._value_[0] == data_set_id:
+                return member._value_[1]
+        return DataSetType["No_Map"]
+
+    No_Map = ("no_map", DataSetType.No_Map)
+    Asset_Allocation = ("99", DataSetType.Current_Or_TimeSeries)
+    Custom_Calculation = ("8", DataSetType.Custom_Calculation)
+    Daily_Gross_Return_Index = ("7", DataSetType.TimeSeries)
+    Daily_Return_Index = ("6", DataSetType.TimeSeries)
+    Equity_Country_Exposure = ("15", DataSetType.Current_Or_TimeSeries)
+    Equity_Market_Capitalization = ("25", DataSetType.Current_Or_TimeSeries)
+    Equity_Port_Stats_Long = ("27", DataSetType.Current_Or_TimeSeries)
+    Equity_Port_Stats_Short = ("28", DataSetType.Current_Or_TimeSeries)
+    Equity_Regional_Exposure = ("21", DataSetType.Current_Or_TimeSeries)
+    Equity_Sector_Exposure = ("17", DataSetType.Current_Or_TimeSeries)
+    Equity_Style_Analysis = ("24", DataSetType.Current_Or_TimeSeries)
+    Equity_Style_Capitalization = ("22", DataSetType.Current_Or_TimeSeries)
+    Equity_Style_Valuation = ("23", DataSetType.Current_Or_TimeSeries)
+    Equity_Type = ("19", DataSetType.TimeSeries)
+    ESG_Carbon = ("12", DataSetType.Current_Or_TimeSeries)
+    ESG_Product_Involvement = ("13", DataSetType.Current_Or_TimeSeries)
+    ESG_Sustainability = ("14", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_ABS_Collateral_Type_Detail = ("34", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Bond_Insurer = ("71", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Call_Type = ("35", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_CMO_Issuer_Type = ("36", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_CMO_Payment_Type = ("37", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_CMO_Tranche_Type = ("38", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Convertible_Type = ("43", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Country_Exposure = ("29", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Coupon_Type = ("44", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Credit_Enhancement_Type = ("67", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Credit_Grd_And_Credit_Rtg_Breakdown_Detail = ("77", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_CreditQualityBreakdown = ("68", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Credit_Rtg = ("76", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Current_Yield_And_Current_Yield_Breakdown_Detail = ("85", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Default_Reason = ("61", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Default_Type = ("62", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_DTW_Breakdown_Super = ("82", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_DTW_And_DTW_Breakdown_Detail = ("75", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Duration_Effective = ("39", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Duration_Modified_to_maturity = ("40", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Eff_Convxty_breakdown_Super = ("84", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_EFF_Convxty_And_Convxty_Breakdown_Detail = ("73", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Eff_Dua_Breakdown_Super = ("78", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Effective_Maturity = ("41", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Eff_Mty_Breakdown_Super = ("80", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Geographic_Exposure = ("93", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Guarantee_Type = ("63", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Guarantor_Type = ("64", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Interest_Rate_Type_Detail = ("45", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Issuer_Type = ("46", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Issuer_Type_Breakdown_Super = ("90", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_LOC_Type = ("65", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Maturity_Type = ("47", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_MBS_Agency = ("48", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Mbs_Agency_Breakdown_Super = ("87", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_MBS_Collateral_Type = ("49", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Mod_Dur_Breakdown_Super = ("79", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Morningstar_Sectors = ("94", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Municipal_Security_Type_Breakdown = ("92", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Municipal_Security_Type_Breakdown_Super = ("88", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Next_Call_And_Next_Call_Breakdown_Detail = ("86", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_OAS_Breakdown_Super = ("83", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_OAS_And_OAS_Breakdown_Detail = ("72", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_PIK_Type = ("50", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Portfolio_Statistics = ("33", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Pre_refunded_ETM_Type = ("66", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Primary_Sector_Breakdown = ("32", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Put_Type = ("51", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Put_Type_Detail = ("52", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Secondary_Sector_Breakdown = ("30", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_SEC_Registration_Type = ("53", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Secured_by_Collateral_Type = ("54", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Securitization_Collateral_Type = ("69", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Securitized_Mortgage_Type = ("55", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Security_Rank = ("56", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Security_Rank_Breakdown_Super = ("91", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Sinking_Fund_Type = ("57", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_State_Taxation = ("58", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Structured_Securitized_Type = ("59", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Super_Sector_Breakdown = ("31", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Use_of_Proceeds = ("70", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Use_Of_Proceeds_Breakdown_Super = ("89", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_US_Federal_Taxation = ("60", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_Yield_to_Maturity_YTM = ("42", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_YTM_Breakdown_Super = ("81", DataSetType.Current_Or_TimeSeries)
+    Fixed_Income_YTW_And_YTW_Breakdown_Detail = ("74", DataSetType.Current_Or_TimeSeries)
+    GICS_Equity_Industry = ("20", DataSetType.Current_Or_TimeSeries)
+    GICS_Equity_Sector_Exposure = ("18", DataSetType.Current_Or_TimeSeries)
+    MSCI_Equity_Country_Exposure = ("16", DataSetType.Current_Or_TimeSeries)
+    Post_tax_Returns_Month_end = ("9", DataSetType.Current_Or_TimeSeries)
+    Regional_Asset_Class_Market_Cap = ("95", DataSetType.Current)
+    Representative_Cost = ("96", DataSetType.Current_Or_TimeSeries)
+    Returns_Calendar_Year = ("5", DataSetType.Current)
+    Returns_Daily = ("2", DataSetType.Current)
+    Returns_Month_End = ("3", DataSetType.Current)
+    Returns_Quarter_End = ("4", DataSetType.Current)
+    Risk_Total_ReturnMonth_End = ("10", DataSetType.Current_Or_TimeSeries)
+    Risk_Total_ReturnQtr_End = ("11", DataSetType.Current_Or_TimeSeries)
+    Snapshot = ("1", DataSetType.Current)
+    South_Africa_Asset_Allocation = ("101", DataSetType.Current_Or_TimeSeries)
+    Stock_Intersection = ("26", DataSetType.Current_Or_TimeSeries)
+    Surveyed_Asset_Allocation_AUS = ("97", DataSetType.Current_Or_TimeSeries)
+    Surveyed_Asset_Allocation_CAN = ("98", DataSetType.Current_Or_TimeSeries)
+    Surveyed_Asset_Allocation_NZ = ("100", DataSetType.Current_Or_TimeSeries)
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/_utils.py` & `morningstar_data-1.3.0/morningstar_data/direct/_utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,113 +1,113 @@
-import datetime
-import time
-
-from uuid import UUID
-from pandas import DataFrame
-from typing import List, Any, Dict, Callable
-from .._base import _logger
-from ._exceptions import BadRequestException
-from ._error_messages import BAD_REQUEST_ERROR_INVALID_DATE_FORMAT
-import requests
-
-from ._config_key import REQUIRED_DATA_POINT_SETTINGS, VISIBLE_DATA_POINT_SETTINGS
-
-
-FORMAT_DATE = "%Y-%m-%d"
-
-
-def _reduce_list_data(lists: List[Dict[str, Any]], props_dict: Dict[str, str]) -> List[Dict[str, Any]]:
-    filtered_lists, id_for, name = [], props_dict["id"], props_dict["name"]
-    for item in lists:
-        data: Dict[str, Any] = {"id": item[id_for], "name": item[name]}
-        filtered_lists.append(data)
-
-    return filtered_lists
-
-
-def _extract_data(data: list) -> List[Any]:
-    values = []
-
-    for item in data:
-        value = {}
-        for k, v in item.items():
-            if isinstance(v, dict):
-                value.update(v)
-            else:
-                value[k] = v
-        values.append(value)
-
-    return values
-
-
-def _empty_to_none(df: DataFrame) -> DataFrame:
-    return df.where((df.notnull()) & (df != ""), None)
-
-
-def _get_iso_today() -> str:
-    d: datetime.date = datetime.date.today()
-    format_iso: str = d.isoformat()
-    return format_iso
-
-
-def _mapper_data_frame_return_list(df: DataFrame, get_values: Callable) -> List:
-    data = [entry for entry in df.to_dict(orient="index").values()]
-    items: List = [get_values(key, value, row) for row in data for key, value in row.items()]
-    filter_not_none: Callable = lambda x: x is not None
-    return list(filter(filter_not_none, items))
-
-
-def _mapper_data_frame_return_dict(df: DataFrame, get_values: Callable) -> Dict:
-    result: Dict = {}
-
-    def get_values_for_list(column: str, value: Any, row: Dict[str, Any]) -> None:
-        get_values(result, column, value, row)
-        return None
-
-    _mapper_data_frame_return_list(df, get_values_for_list)
-
-    return result
-
-
-def _rename_data_frame_column(df: DataFrame, source: str, target: str) -> DataFrame:
-    return df.rename(columns={source: target})
-
-
-def _filter_data_frame_column_by_setting(df: DataFrame) -> DataFrame:
-    data_point_settings = REQUIRED_DATA_POINT_SETTINGS + VISIBLE_DATA_POINT_SETTINGS
-    return df.filter(items=data_point_settings)
-
-
-def _reindex_data_frame_column(df: DataFrame, target_column: str, new_index: int) -> DataFrame:
-    column_list = df.columns.tolist()
-
-    if (target_column in column_list) and (column_list.index(target_column) != new_index):
-        data_point_id_col = df[target_column]
-        df.drop(target_column, axis=1, inplace=True)
-        df.insert(new_index, target_column, data_point_id_col)
-
-    return df
-
-
-def _is_uuid(uuid_str: str, version: int = 4) -> bool:
-    try:
-        uuid_obj = UUID(uuid_str, version=version)
-    except ValueError:
-        return False
-    return str(uuid_obj) == uuid_str
-
-
-def _format_date(date: str) -> str:
-    try:
-        return time.strftime(FORMAT_DATE, time.strptime(date, FORMAT_DATE))
-    except Exception as e:
-        _logger.debug(f"Date format error: {e}")
-        raise BadRequestException(BAD_REQUEST_ERROR_INVALID_DATE_FORMAT) from None
-
-
-def get_bytes(url: str) -> requests.Response:
-    """
-    Downloads bytes from S3 presigned url
-    """
-    res = requests.get(url)
-    res.raise_for_status()
-    return res
+import datetime
+import time
+
+from uuid import UUID
+from pandas import DataFrame
+from typing import List, Any, Dict, Callable
+from .._base import _logger
+from ._exceptions import BadRequestException
+from ._error_messages import BAD_REQUEST_ERROR_INVALID_DATE_FORMAT
+import requests
+
+from ._config_key import REQUIRED_DATA_POINT_SETTINGS, VISIBLE_DATA_POINT_SETTINGS
+
+
+FORMAT_DATE = "%Y-%m-%d"
+
+
+def _reduce_list_data(lists: List[Dict[str, Any]], props_dict: Dict[str, str]) -> List[Dict[str, Any]]:
+    filtered_lists, id_for, name = [], props_dict["id"], props_dict["name"]
+    for item in lists:
+        data: Dict[str, Any] = {"id": item[id_for], "name": item[name]}
+        filtered_lists.append(data)
+
+    return filtered_lists
+
+
+def _extract_data(data: list) -> List[Any]:
+    values = []
+
+    for item in data:
+        value = {}
+        for k, v in item.items():
+            if isinstance(v, dict):
+                value.update(v)
+            else:
+                value[k] = v
+        values.append(value)
+
+    return values
+
+
+def _empty_to_none(df: DataFrame) -> DataFrame:
+    return df.where((df.notnull()) & (df != ""), None)
+
+
+def _get_iso_today() -> str:
+    d: datetime.date = datetime.date.today()
+    format_iso: str = d.isoformat()
+    return format_iso
+
+
+def _mapper_data_frame_return_list(df: DataFrame, get_values: Callable) -> List:
+    data = [entry for entry in df.to_dict(orient="index").values()]
+    items: List = [get_values(key, value, row) for row in data for key, value in row.items()]
+    filter_not_none: Callable = lambda x: x is not None
+    return list(filter(filter_not_none, items))
+
+
+def _mapper_data_frame_return_dict(df: DataFrame, get_values: Callable) -> Dict:
+    result: Dict = {}
+
+    def get_values_for_list(column: str, value: Any, row: Dict[str, Any]) -> None:
+        get_values(result, column, value, row)
+        return None
+
+    _mapper_data_frame_return_list(df, get_values_for_list)
+
+    return result
+
+
+def _rename_data_frame_column(df: DataFrame, source: str, target: str) -> DataFrame:
+    return df.rename(columns={source: target})
+
+
+def _filter_data_frame_column_by_setting(df: DataFrame) -> DataFrame:
+    data_point_settings = REQUIRED_DATA_POINT_SETTINGS + VISIBLE_DATA_POINT_SETTINGS
+    return df.filter(items=data_point_settings)
+
+
+def _reindex_data_frame_column(df: DataFrame, target_column: str, new_index: int) -> DataFrame:
+    column_list = df.columns.tolist()
+
+    if (target_column in column_list) and (column_list.index(target_column) != new_index):
+        data_point_id_col = df[target_column]
+        df.drop(target_column, axis=1, inplace=True)
+        df.insert(new_index, target_column, data_point_id_col)
+
+    return df
+
+
+def _is_uuid(uuid_str: str, version: int = 4) -> bool:
+    try:
+        uuid_obj = UUID(uuid_str, version=version)
+    except ValueError:
+        return False
+    return str(uuid_obj) == uuid_str
+
+
+def _format_date(date: str) -> str:
+    try:
+        return time.strftime(FORMAT_DATE, time.strptime(date, FORMAT_DATE))
+    except Exception as e:
+        _logger.debug(f"Date format error: {e}")
+        raise BadRequestException(BAD_REQUEST_ERROR_INVALID_DATE_FORMAT) from None
+
+
+def get_bytes(url: str) -> requests.Response:
+    """
+    Downloads bytes from S3 presigned url
+    """
+    res = requests.get(url)
+    res.raise_for_status()
+    return res
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/asset_flow.py` & `morningstar_data-1.3.0/morningstar_data/direct/asset_flow.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,294 +1,294 @@
-import simplejson as json
-
-from pandas import DataFrame
-from typing import List, Any, Optional, Union, Dict
-
-from . import _decorator, _utils, _error_messages
-from .._base import _logger
-from ._config import _Config
-from ._data_objects import Investments
-from ._data_point import _request_asset_flow_data_points
-from ._exceptions import BadRequestException, QueryLimitException, ResourceNotFoundError
-from ._base_api import APIBackend
-
-_config = _Config()
-
-
-class AssetFlowAPIBackend(APIBackend):
-    """
-    Subclass to call the Asset Flow Data API and handle any HTTP errors that occur.
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def _handle_custom_http_errors(self, res: Any) -> Any:
-        """
-        Handle HTTP errors with custom error messages
-        """
-        response_message = res.json()["message"]
-        if res.status_code == 403 and "Exceed query limitation." in response_message:
-            _logger.debug(f"Query Limit Exception: {res.status_code} {response_message}")
-            query_limit = self._get_security_data_query_limit()
-            raise QueryLimitException(query_limit) from None
-        elif res.status_code == 404:
-            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
-            raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ASSET_FLOW) from None
-
-    def _get_security_data_query_limit(self) -> str:
-        try:
-            url = f"{_config.securitydata_service_url()}v1/limitation/summary"
-            res = self.do_get_request(url)
-            return str(res["limitationTotal"])
-        except Exception as e:
-            _logger.error(f"Error getting security data query limit: {e}")
-            raise QueryLimitException from None
-
-
-_asset_flow_api_request = AssetFlowAPIBackend()
-
-
-@_decorator.typechecked
-def get_asset_flow_markets() -> DataFrame:
-    """Returns all investment markets that can be used to retrieve asset flow data. For example,
-    "US Open-end & ETFs ex MM ex FoF".
-
-    Returns:
-        DataFrame: A DataFrame object with asset flow markets data. DataFrame columns include:
-
-        * marketId
-        * marketName
-        * currency
-
-    :Examples:
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.get_asset_flow_markets()
-        df
-
-    :Output:
-        ========  ===============================  ========
-        marketId  marketName                       currency
-        ========  ===============================  ========
-        5         US Open-end & ETF ex MM ex FoF   USD
-        6         US Open-end, ETF, and MM ex FoF  USD
-        ...
-        ========  ===============================  ========
-
-    Errors:
-        AccessDeniedError: Raised when the user is not authenticated.
-
-        BadRequestError: Raised when the user does not provide a properly formatted request.
-
-        ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
-
-    """
-    url = f"{_config.securitydata_service_url()}v1/assetflow/all-markets"
-    response_json = _asset_flow_api_request.do_get_request(url)
-    if response_json and isinstance(response_json, list):
-        return DataFrame(response_json)[["marketId", "marketName", "currency"]]
-    else:
-        return DataFrame({"marketId": [], "marketName": [], "currency": []})
-
-
-def get_asset_flow_data_points() -> DataFrame:
-    """Returns all available data points related to asset flows.
-
-    Returns:
-        DataFrame: A DataFrame object with asset flow data points data. DataFrame columns include:
-
-        * datapointId
-        * datapointName
-        * asOfDate
-        * alias
-        * startDate
-        * endDate
-        * frequency
-
-    Examples:
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.get_asset_flow_data_points()
-        df
-
-    :Output:
-        ===========  =============  ==========  ==========================================  =========  =======  =========
-        datapointId  datapointName  asOfDate    alias                                       startDate  endDate  frequency
-        ===========  =============  ==========  ==========================================  =========  =======  =========
-        TNA0M        XXX            2021-09-30  Total Net Assets-Market Value(Share Class)  None       None     None
-        ...
-        ===========  =============  ==========  ==========================================  =========  =======  =========
-
-    """
-    response_json = _request_asset_flow_data_points()
-    if response_json and isinstance(response_json, list):
-        for settings in response_json:
-            settings["datapointName"] = settings.pop("name")
-            settings["alias"] = settings["datapointName"]
-
-        settings = _utils._extract_data(response_json)
-        settings_data_frame = DataFrame(settings)
-
-        column_list = settings_data_frame.columns.tolist()
-        if ("datapointId" in column_list) & (column_list.index("datapointId") != 0):
-            data_point_id_col = settings_data_frame["datapointId"]
-            settings_data_frame = settings_data_frame.drop("datapointId", axis=1)
-            settings_data_frame.insert(0, "datapointId", data_point_id_col)
-
-        column_list = settings_data_frame.columns.tolist()
-        if ("datapointName" in column_list) & (column_list.index("datapointName") != 1):
-            data_point_name_col = settings_data_frame["datapointName"]
-            settings_data_frame = settings_data_frame.drop("datapointName", axis=1)
-            settings_data_frame.insert(1, "datapointName", data_point_name_col)
-
-        settings_data_frame = settings_data_frame.where(settings_data_frame.notnull(), None)
-        return settings_data_frame
-    else:
-        return DataFrame()
-
-
-@_decorator.typechecked
-def get_asset_flow(
-    market_id: str,
-    data_point_settings: DataFrame,
-    investments: Optional[Union[List[str], str, Dict[str, Any]]] = None,
-) -> DataFrame:
-    """Get asset flow data for a market of investments or specific investments within a market.
-
-    Args:
-        investments (:obj:`Union`, `required`): Defines the investments to fetch. Input can be:
-
-            * Investment IDs (:obj:`list`, `optional`): Investment identifiers, in the format of SecId;Universe or just SecId. E.g., ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"]. Use the `investments <./lookup.html#morningstar_data.direct.investments>`_ function to discover identifiers.
-            * Investment List ID (:obj:`str`, `optional`): Saved investment list in Morningstar Direct. Use the `get_investment_lists <./lists.html#morningstar_data.direct.user_items.get_investment_lists>`_ function to discover saved lists.
-            * Search Criteria  ID (:obj:`str`, `optional`): Saved search criteria in Morningstar Direct. Use the `get_search_criteria <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria>`_ function to discover saved search criteria.
-            * Search Criteria Condition (:obj:`dict`, `optional`): Search criteria definition. See details in the Reference section of `get_investment_data <./investment.html#morningstar_data.direct.get_investment_data>`_ or use the `get_search_criteria_conditions <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria_conditions>`_ function to discover the definition of a saved search criteria.
-
-        market_id(:obj:`str`): A numeric code representing a broad market of investments. For example, the code for "US Open-end & ETF ex MM ex FoF" is "5". Use the `get_asset_flow_markets <./assetflow.html#morningstar_data.direct.get_asset_flow_markets>`_ function to retrieve a full list of codes.
-        data_point_settings(:obj:`DataFrame`): A DataFrame of data points with defined settings. Each row represents a data point. Each column is a configurable setting. This DataFrame can be obtained by `retrieving asset flow data points <./assetflow.html#morningstar_data.direct.get_asset_flow_data_points>`_, or by `retrieving data point settings <./lookup.html#morningstar_data.direct.get_data_point_settings>`_.
-
-    Returns:
-        DataFrame: A DataFrame object with asset flow data. DataFrame columns include `investmentId` and data point names, as
-        provided in `data_point_settings`.
-
-    :Examples:
-
-    ::
-
-        import morningstar_data as md
-        import pandas
-
-        ASSET_FLOW_DATA_POINT_SETTINGS = [
-            {
-                "datapointId": "TNA0M",
-                "datapointName": "Total Net Assets-Market Value(Share Class)",
-                "asOfDate": "2021-08-30",
-                "alias": "Total Net Assets-Market Value(Share Class)",
-                "startDate": None,
-                "endDate": None,
-                "frequency": None,
-            }
-        ]
-        settings = pandas.DataFrame(ASSET_FLOW_DATA_POINT_SETTINGS)
-        df = md.direct.get_asset_flow(
-            investments=["F000010HRO"], market_id="165", data_point_settings=settings
-        )
-        df
-
-    :Output:
-        ============  =======================================================
-        investmentId  Total Net Assets-Market Value(Share Class) - 2021-06-30
-        ============  =======================================================
-        F000010HRO    0.00188
-        ============  =======================================================
-
-    Errors:
-        AccessDeniedError: Raised when the user is not authenticated.
-
-        BadRequestError: Raised when the user does not provide a properly formatted request.
-
-        ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
-
-    """
-    if data_point_settings.empty:
-        raise BadRequestException("data_point_settings is required.")
-
-    investment_id_list: List[Any] = []
-
-    if investments is not None:
-        investment_object = Investments(investments)
-        investment_id_list = investment_object.get_investment_ids()
-
-    data_point_settings = data_point_settings.where(data_point_settings.notnull(), None)
-    data_point_list = data_point_settings.to_dict(orient="records")
-    postbody = {"marketId": market_id, "datapoints": data_point_list}
-    if investment_id_list is not None:
-        postbody["investments"] = list(map(lambda x: {"id": _remove_univ(x)}, investment_id_list))
-    return _get_data(postbody)
-
-
-def _get_data(data: dict) -> DataFrame:
-    try:
-        url = f"{_config.securitydata_service_url()}v1/assetflow/data"
-        response_json = _asset_flow_api_request.do_post_request(url, json.dumps(data, ignore_nan=True))
-        if not response_json or not isinstance(response_json, list):
-            return DataFrame()
-
-        data_point_columns: dict = {x.get("alias", "").strip(): [] for x in data.get("datapoints", [])}
-        investment_data_list = []
-        for investment in response_json:
-            data_point_values = dict()
-            data_point_values["investmentId"] = investment.get("id", "")
-            values = investment.get("values", [])
-            for data_point_value in values:
-                alias = data_point_value.get("alias", "").strip()
-                value_list = data_point_value.get("value", [])
-                data_point_column = data_point_columns.get(alias)
-                if data_point_column is None:
-                    data_point_column = []
-                    data_point_columns[alias] = data_point_column
-
-                data_point_column.extend([_concat_str(alias, x.get("date", "")) for x in value_list if _concat_str(alias, x.get("date", "")) not in data_point_column])
-                data_point_values.update({_concat_str(alias, x.get("date", "")): x.get("value", None) for x in value_list})
-            investment_data_list.append(data_point_values)
-
-        result = DataFrame(investment_data_list)
-        column_order = ["investmentId"]
-        return _column_reorder(data_point_columns, column_order, result)
-    except Exception as e:
-        raise e
-
-
-def _column_reorder(data_point_columns: dict, column_order: list, result: DataFrame) -> DataFrame:
-    for alias, column in data_point_columns.items():
-        column = sorted(set(column))
-        column_order.extend(column)
-    return result[column_order]
-
-
-def _remove_univ(investment_id: Optional[str]) -> Optional[str]:
-    sec_id = investment_id
-    if sec_id is not None and ";" in sec_id:
-        return sec_id.split(";")[0]
-    return sec_id
-
-
-def _concat_str(s1: str, s2: str) -> str:
-    return f"{s1} - {s2}"
+import simplejson as json
+
+from pandas import DataFrame
+from typing import List, Any, Optional, Union, Dict
+
+from . import _decorator, _utils, _error_messages
+from .._base import _logger
+from ._config import _Config
+from ._data_objects import Investments
+from ._data_point import _request_asset_flow_data_points
+from ._exceptions import BadRequestException, QueryLimitException, ResourceNotFoundError
+from ._base_api import APIBackend
+
+_config = _Config()
+
+
+class AssetFlowAPIBackend(APIBackend):
+    """
+    Subclass to call the Asset Flow Data API and handle any HTTP errors that occur.
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def _handle_custom_http_errors(self, res: Any) -> Any:
+        """
+        Handle HTTP errors with custom error messages
+        """
+        response_message = res.json()["message"]
+        if res.status_code == 403 and "Exceed query limitation." in response_message:
+            _logger.debug(f"Query Limit Exception: {res.status_code} {response_message}")
+            query_limit = self._get_security_data_query_limit()
+            raise QueryLimitException(query_limit) from None
+        elif res.status_code == 404:
+            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
+            raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ASSET_FLOW) from None
+
+    def _get_security_data_query_limit(self) -> str:
+        try:
+            url = f"{_config.securitydata_service_url()}v1/limitation/summary"
+            res = self.do_get_request(url)
+            return str(res["limitationTotal"])
+        except Exception as e:
+            _logger.error(f"Error getting security data query limit: {e}")
+            raise QueryLimitException from None
+
+
+_asset_flow_api_request = AssetFlowAPIBackend()
+
+
+@_decorator.typechecked
+def get_asset_flow_markets() -> DataFrame:
+    """Returns all investment markets that can be used to retrieve asset flow data. For example,
+    "US Open-end & ETFs ex MM ex FoF".
+
+    Returns:
+        DataFrame: A DataFrame object with asset flow markets data. DataFrame columns include:
+
+        * marketId
+        * marketName
+        * currency
+
+    :Examples:
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.get_asset_flow_markets()
+        df
+
+    :Output:
+        ========  ===============================  ========
+        marketId  marketName                       currency
+        ========  ===============================  ========
+        5         US Open-end & ETF ex MM ex FoF   USD
+        6         US Open-end, ETF, and MM ex FoF  USD
+        ...
+        ========  ===============================  ========
+
+    Errors:
+        AccessDeniedError: Raised when the user is not authenticated.
+
+        BadRequestError: Raised when the user does not provide a properly formatted request.
+
+        ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
+
+    """
+    url = f"{_config.securitydata_service_url()}v1/assetflow/all-markets"
+    response_json = _asset_flow_api_request.do_get_request(url)
+    if response_json and isinstance(response_json, list):
+        return DataFrame(response_json)[["marketId", "marketName", "currency"]]
+    else:
+        return DataFrame({"marketId": [], "marketName": [], "currency": []})
+
+
+def get_asset_flow_data_points() -> DataFrame:
+    """Returns all available data points related to asset flows.
+
+    Returns:
+        DataFrame: A DataFrame object with asset flow data points data. DataFrame columns include:
+
+        * datapointId
+        * datapointName
+        * asOfDate
+        * alias
+        * startDate
+        * endDate
+        * frequency
+
+    Examples:
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.get_asset_flow_data_points()
+        df
+
+    :Output:
+        ===========  =============  ==========  ==========================================  =========  =======  =========
+        datapointId  datapointName  asOfDate    alias                                       startDate  endDate  frequency
+        ===========  =============  ==========  ==========================================  =========  =======  =========
+        TNA0M        XXX            2021-09-30  Total Net Assets-Market Value(Share Class)  None       None     None
+        ...
+        ===========  =============  ==========  ==========================================  =========  =======  =========
+
+    """
+    response_json = _request_asset_flow_data_points()
+    if response_json and isinstance(response_json, list):
+        for settings in response_json:
+            settings["datapointName"] = settings.pop("name")
+            settings["alias"] = settings["datapointName"]
+
+        settings = _utils._extract_data(response_json)
+        settings_data_frame = DataFrame(settings)
+
+        column_list = settings_data_frame.columns.tolist()
+        if ("datapointId" in column_list) & (column_list.index("datapointId") != 0):
+            data_point_id_col = settings_data_frame["datapointId"]
+            settings_data_frame = settings_data_frame.drop("datapointId", axis=1)
+            settings_data_frame.insert(0, "datapointId", data_point_id_col)
+
+        column_list = settings_data_frame.columns.tolist()
+        if ("datapointName" in column_list) & (column_list.index("datapointName") != 1):
+            data_point_name_col = settings_data_frame["datapointName"]
+            settings_data_frame = settings_data_frame.drop("datapointName", axis=1)
+            settings_data_frame.insert(1, "datapointName", data_point_name_col)
+
+        settings_data_frame = settings_data_frame.where(settings_data_frame.notnull(), None)
+        return settings_data_frame
+    else:
+        return DataFrame()
+
+
+@_decorator.typechecked
+def get_asset_flow(
+    market_id: str,
+    data_point_settings: DataFrame,
+    investments: Optional[Union[List[str], str, Dict[str, Any]]] = None,
+) -> DataFrame:
+    """Get asset flow data for a market of investments or specific investments within a market.
+
+    Args:
+        investments (:obj:`Union`, `required`): Defines the investments to fetch. Input can be:
+
+            * Investment IDs (:obj:`list`, `optional`): Investment identifiers, in the format of SecId;Universe or just SecId. E.g., ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"]. Use the `investments <./lookup.html#morningstar_data.direct.investments>`_ function to discover identifiers.
+            * Investment List ID (:obj:`str`, `optional`): Saved investment list in Morningstar Direct. Use the `get_investment_lists <./lists.html#morningstar_data.direct.user_items.get_investment_lists>`_ function to discover saved lists.
+            * Search Criteria  ID (:obj:`str`, `optional`): Saved search criteria in Morningstar Direct. Use the `get_search_criteria <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria>`_ function to discover saved search criteria.
+            * Search Criteria Condition (:obj:`dict`, `optional`): Search criteria definition. See details in the Reference section of `get_investment_data <./investment.html#morningstar_data.direct.get_investment_data>`_ or use the `get_search_criteria_conditions <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria_conditions>`_ function to discover the definition of a saved search criteria.
+
+        market_id(:obj:`str`): A numeric code representing a broad market of investments. For example, the code for "US Open-end & ETF ex MM ex FoF" is "5". Use the `get_asset_flow_markets <./assetflow.html#morningstar_data.direct.get_asset_flow_markets>`_ function to retrieve a full list of codes.
+        data_point_settings(:obj:`DataFrame`): A DataFrame of data points with defined settings. Each row represents a data point. Each column is a configurable setting. This DataFrame can be obtained by `retrieving asset flow data points <./assetflow.html#morningstar_data.direct.get_asset_flow_data_points>`_, or by `retrieving data point settings <./lookup.html#morningstar_data.direct.get_data_point_settings>`_.
+
+    Returns:
+        DataFrame: A DataFrame object with asset flow data. DataFrame columns include `investmentId` and data point names, as
+        provided in `data_point_settings`.
+
+    :Examples:
+
+    ::
+
+        import morningstar_data as md
+        import pandas
+
+        ASSET_FLOW_DATA_POINT_SETTINGS = [
+            {
+                "datapointId": "TNA0M",
+                "datapointName": "Total Net Assets-Market Value(Share Class)",
+                "asOfDate": "2021-08-30",
+                "alias": "Total Net Assets-Market Value(Share Class)",
+                "startDate": None,
+                "endDate": None,
+                "frequency": None,
+            }
+        ]
+        settings = pandas.DataFrame(ASSET_FLOW_DATA_POINT_SETTINGS)
+        df = md.direct.get_asset_flow(
+            investments=["F000010HRO"], market_id="165", data_point_settings=settings
+        )
+        df
+
+    :Output:
+        ============  =======================================================
+        investmentId  Total Net Assets-Market Value(Share Class) - 2021-06-30
+        ============  =======================================================
+        F000010HRO    0.00188
+        ============  =======================================================
+
+    Errors:
+        AccessDeniedError: Raised when the user is not authenticated.
+
+        BadRequestError: Raised when the user does not provide a properly formatted request.
+
+        ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
+
+    """
+    if data_point_settings.empty:
+        raise BadRequestException("data_point_settings is required.")
+
+    investment_id_list: List[Any] = []
+
+    if investments is not None:
+        investment_object = Investments(investments)
+        investment_id_list = investment_object.get_investment_ids()
+
+    data_point_settings = data_point_settings.where(data_point_settings.notnull(), None)
+    data_point_list = data_point_settings.to_dict(orient="records")
+    postbody = {"marketId": market_id, "datapoints": data_point_list}
+    if investment_id_list is not None:
+        postbody["investments"] = list(map(lambda x: {"id": _remove_univ(x)}, investment_id_list))
+    return _get_data(postbody)
+
+
+def _get_data(data: dict) -> DataFrame:
+    try:
+        url = f"{_config.securitydata_service_url()}v1/assetflow/data"
+        response_json = _asset_flow_api_request.do_post_request(url, json.dumps(data, ignore_nan=True))
+        if not response_json or not isinstance(response_json, list):
+            return DataFrame()
+
+        data_point_columns: dict = {x.get("alias", "").strip(): [] for x in data.get("datapoints", [])}
+        investment_data_list = []
+        for investment in response_json:
+            data_point_values = dict()
+            data_point_values["investmentId"] = investment.get("id", "")
+            values = investment.get("values", [])
+            for data_point_value in values:
+                alias = data_point_value.get("alias", "").strip()
+                value_list = data_point_value.get("value", [])
+                data_point_column = data_point_columns.get(alias)
+                if data_point_column is None:
+                    data_point_column = []
+                    data_point_columns[alias] = data_point_column
+
+                data_point_column.extend([_concat_str(alias, x.get("date", "")) for x in value_list if _concat_str(alias, x.get("date", "")) not in data_point_column])
+                data_point_values.update({_concat_str(alias, x.get("date", "")): x.get("value", None) for x in value_list})
+            investment_data_list.append(data_point_values)
+
+        result = DataFrame(investment_data_list)
+        column_order = ["investmentId"]
+        return _column_reorder(data_point_columns, column_order, result)
+    except Exception as e:
+        raise e
+
+
+def _column_reorder(data_point_columns: dict, column_order: list, result: DataFrame) -> DataFrame:
+    for alias, column in data_point_columns.items():
+        column = sorted(set(column))
+        column_order.extend(column)
+    return result[column_order]
+
+
+def _remove_univ(investment_id: Optional[str]) -> Optional[str]:
+    sec_id = investment_id
+    if sec_id is not None and ";" in sec_id:
+        return sec_id.split(";")[0]
+    return sec_id
+
+
+def _concat_str(s1: str, s2: str) -> str:
+    return f"{s1} - {s2}"
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/custom_database.py` & `morningstar_data-1.3.0/morningstar_data/direct/custom_database.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,361 +1,361 @@
-import simplejson as json
-import warnings
-
-from abc import ABC
-from pandas import DataFrame
-from typing import List, Any, Optional, Dict, Union, Callable
-
-from . import _decorator, _error_messages
-from .._base import _logger
-from ._exceptions import ValueErrorException, ResourceNotFoundError
-from ._config import _Config
-from .data_type import Blank
-from ._data_type import DatabaseCD
-from ._utils import _mapper_data_frame_return_dict, _mapper_data_frame_return_list
-from ._data_objects import ValidCustomDataPointTypes, TypeValue
-from ._base_api import APIBackend
-
-
-_config = _Config()
-
-
-class CustomDatabaseAPIBackend(APIBackend):
-    """
-    Subclass to call the custom database API and handle any HTTP errors that occur.
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def _handle_custom_http_errors(self, res: Any) -> Any:
-        """
-        Handle HTTP errors with custom error messages
-        """
-        response_message = res.json()["message"]
-        if res.status_code == 404:
-            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
-            raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_CUSTOM_DATABASE) from None
-
-
-ResultType = Dict[str, Union[bool, str]]
-ListDatapointType = List[Dict[str, Any]]
-DictValues = Dict[str, TypeValue]
-RelValuesWithDatapoint = Dict[str, Union[TypeValue, List[DictValues]]]
-
-
-class _CustomDatabase(ABC):
-    def __init__(self, database_type: DatabaseCD, custom_database_api_request: CustomDatabaseAPIBackend):
-        self.database_type: DatabaseCD = database_type
-        self.all_data_points: ListDatapointType = []
-        self._custom_database_api_request = custom_database_api_request
-
-    def get_data_point_from_name(self, data_point_name: str, time_series: bool = False) -> Dict[str, str]:
-        data_points = self.get_all_data_points()
-        data_point = next(
-            (item for item in data_points if item["name"] == data_point_name),
-            None,
-        )
-
-        if data_point is None or "columnType" not in data_point:
-            raise ValueErrorException(f"The column '{data_point_name}' does not exist in the custom datapoints.")
-
-        start_with_ts = data_point["columnType"].startswith("TS")
-
-        if time_series and not start_with_ts:
-            raise ValueErrorException(f"The column '{data_point_name}' is not for a time series.")
-
-        if not time_series and start_with_ts:
-            raise ValueErrorException(f"The column '{data_point_name}' is not for a single value.")
-
-        return data_point
-
-    def get_all_data_points(self) -> ListDatapointType:
-        if not self.all_data_points:
-            url = f"{_config.custom_data_points_service_url()}v1/cdp/definitions?type={self.database_type.value}"
-            self.all_data_points = self._custom_database_api_request.do_get_request(url)
-        return self.all_data_points
-
-    def is_a_valid_value(self, value: Optional[TypeValue], data_point_definition: dict, investment: str) -> Optional[TypeValue]:
-        if value is None:
-            return value
-        validator = ValidCustomDataPointTypes(data_point_definition)
-        try:
-            result: TypeValue = validator.is_valid(value)
-            return result
-        except Exception as e:
-            raise ValueErrorException(f"Error in '{data_point_definition['name']}' column with '{investment}': {str(e)}")
-
-    def convert_to_objects(self, values: DataFrame) -> Any:
-        return values.astype(object).where(values.notnull(), None).where(values != "", None)
-
-    def filter_null_values(
-        self,
-        values: DataFrame,
-        blank: Blank,
-        key_column: str,
-        date_column: Optional[str] = None,
-    ) -> Any:
-        ops = Blank.options()
-        if blank is Blank.warning and values.isnull().values.any():
-            raise ValueErrorException(f"The dataframe contains null or blank values. \n" f"Please choose one of the following as a `blank` arg: {ops} \n") from None
-        ignore_columns = [
-            key_column,
-            date_column if date_column is not None else key_column,
-        ]
-        if blank is Blank.ignore and values.drop(list(set(ignore_columns)), axis=1).isnull().values.all():
-            raise ValueErrorException(f"All the dataframe values are null or blank. \n" f"Please choose one of the following as a `blank` arg: {ops} \n") from None
-        return values
-
-    def get_to_delete(self, value: TypeValue, blank: Blank) -> bool:
-        if blank is Blank.ignore:
-            return False
-        else:
-            if value is None:
-                return True
-        return False
-
-    @_decorator.typechecked
-    def save_historical_values(
-        self,
-        values: DataFrame,
-        key_column: str = "SecId",
-        date_column: str = "Date",
-        blank: Union[Blank, str] = Blank.warning,
-    ) -> ResultType:
-        """Saves historical time series values for data points in the user's or firm's database in Morningstar Direct.
-
-        Args:
-            values (:obj:`DataFrame`): A DataFrame object with the time series values to be saved in the user’s or firm’s database. The DataFrame columns should include:
-
-                * `SecId` - Column containing investment ID values. If a column named `SecId` is not present, the column name specified in the key_column argument will be used.
-                * `DataPointName` - Data point name which will be updated. Multiple data points can be updated in one request.
-                * `Date` - Column containing date values. If a column named `Date` is not present, the column name specified in the date_column argument will be used.
-
-                For example::
-
-                    ====================  ========  ===============  ===============  ===============
-                    SecId                   Date    DataPointName1   DataPointName2   DataPointName3
-                    ====================  ========  ===============  ===============  ===============
-                    <InvestmentId>         <date>       <value>          <value>          <value>
-                    <InvestmentId>         <date>       <value>          <value>          <value>
-                    ====================  ========  ===============  ===============  ===============
-
-            key_column (:obj:`str`): Name of the column containing investment ID values. If not specified, the column `SecId` will be used.
-
-            date_column (:obj:`str`): Name of the column containing date values. If not specified, the column `Date` will be used.
-
-            blank (:obj:`Blank`): Argument specifying how blank values in the DataFrame should be handled. Valid enum values for this argument are:
-
-                    * warning - Raises an error if the DataFrame contains at least one null or empty (str) value.
-                    * ignore - Saves all DataFrame values except for null or empty (str) values.
-                    * update - Replaces/updates all existing values with the provided values. Deletes any value that is sent as null, None or empty (str) values.
-
-        Returns:
-            DataFrame
-
-        :Examples:
-
-        ::
-
-            import morningstar_data as md
-            from pandas import DataFrame
-
-            df = DataFrame({"SecId": ["FOUSA00C3M", "F000010NJ5"],
-                            "Date": ["2022-02-10","2022-04-2"],
-                            "DataPointNameText": ["2","9"],
-                            "DataPointNameNumber": [12.2178, 78514]})
-
-            md.direct.my_database.save_historical_values(values=df, key_column="SecId", blank=md.direct.Blank.warning)
-
-
-
-        ::
-
-            import morningstar_data as md
-            from pandas import DataFrame
-
-            df = DataFrame({"SecId": ["FOUSA00C3M", "F000010NJ5"],
-                            "Date": ["2022-02-10","2022-04-2"],
-                            "DataPointNameText": ["2","9"],
-                            "DataPointNameNumber": [12.2178, 78514]})
-
-            md.direct.firm_database.save_historical_values(values=df, key_column="SecId", blank=md.direct.Blank.warning)
-
-        Errors:
-            AccessDeniedError: Raised when the user is not authenticated.
-
-            ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-            InternalServerError: Raised when the server encounters an unhandled error.
-
-            NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-            ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
-
-        """
-        if not isinstance(blank, Blank):
-            warnings.warn(
-                "The use of string values for the 'blank' parameter is deprecated and will be removed in the next major version. Use Blank enum values instead",
-                FutureWarning,
-                stacklevel=2,
-            )
-
-        blank = Blank[blank]
-        assert isinstance(blank, Blank)
-
-        if key_column not in values:
-            raise ValueErrorException(f"The key column '{key_column}' does not exist.")
-
-        if date_column not in values:
-            raise ValueErrorException(f"The date column '{date_column}' does not exist")
-
-        values = self.filter_null_values(self.convert_to_objects(values), blank, key_column, date_column)
-
-        def get_values(last_dict: Dict, column: str, value: Any, row: Dict) -> Dict:
-            if column in [key_column, date_column]:
-                return last_dict
-
-            date = self.is_a_valid_value(
-                row[date_column],
-                {
-                    "name": date_column,
-                    "columnType": "Date",
-                },
-                row[key_column],
-            )
-            data_point: Dict[str, str] = self.get_data_point_from_name(column, True)
-
-            assert isinstance(blank, Blank)
-            if value is None and blank is Blank.ignore:
-                return last_dict
-            ts_value = self.is_a_valid_value(value, data_point, row[key_column])
-            relation = f"{data_point['id']}-{row[key_column]}"
-
-            if relation not in last_dict:
-                last_dict[relation] = []
-
-            to_delete = self.get_to_delete(ts_value, blank)
-            last_dict[relation].append({"date": date, "value": ts_value, "toDelete": to_delete})
-            return last_dict
-
-        relations: DictValues = _mapper_data_frame_return_dict(values, get_values)
-        data: List[RelValuesWithDatapoint] = [
-            {
-                "dataPointId": relation.split("-")[0],
-                "investmentId": relation.split("-")[1],
-                "timeSeriesValue": points,
-            }
-            for relation, points in relations.items()
-        ]
-        return self._request_save_values(data)
-
-    @_decorator.typechecked
-    def save_values(
-        self,
-        values: DataFrame,
-        key_column: str = "SecId",
-        blank: Union[Blank, str] = Blank.warning,
-    ) -> ResultType:
-        """Saves values for data points in the user's or firm's database.
-
-        Args:
-            values (:obj:`DataFrame`): A DataFrame object with the values to be saved in the user's or firm's database. The DataFrame columns should include:
-
-                * `SecId` - Column containing investment ID values. If a column named `SecId` is not present, the column name specified in the key_column argument will be used.
-                * `DataPointName` - Data point name which will be updated. Multiple data points can be updated in one request.
-
-                For example::
-
-                    ====================  ===============  ===============  ===============
-                    SecId                 DataPointName1   DataPointName2   DataPointName3
-                    ====================  ===============  ===============  ===============
-                    <InvestmentId>            <value>          <value>          <value>
-                    <InvestmentId>            <value>          <value>          <value>
-                    ====================  ===============  ===============  ===============
-
-            key_column (:obj:`str`): Name of the column containing investment ID values. If not specified, the column `SecId` will be used.
-
-            blank (:obj:`Blank`): Argument specifying how blank values in the DataFrame should be handled. Valid enum values for this argument are:
-
-                * warning - Raises an error if the DataFrame contains at least one null or empty (str) value.
-                * ignore - Saves all DataFrame values except for null or empty (str) values.
-                * update - Replaces/updates all existing values with the provided values. Deletes any value that is sent as null, None or empty (str) values.
-        Returns:
-            DataFrame
-
-        :Examples:
-
-        ::
-
-            import morningstar_data as md
-            from pandas import DataFrame
-            df = DataFrame({"SecId": ["FOUSA00C3M", "F000010NJ5"],
-                               "DataPointNameText": ["2","9"],
-                               "DataPointNameDate": ["2022-02-10","2022-04-2"],
-                               "DataPointNameNumber": [12.2178, 78514]})
-            md.direct.my_database.save_values(values=df, key_column="SecId", blank=md.direct.Blank.warning)
-
-        ::
-
-            import morningstar_data as md
-            from pandas import DataFrame
-            df = DataFrame({"SecId": ["FOUSA00C3M", "F000010NJ5"],
-                               "DataPointNameText": ["2","9"],
-                               "DataPointNameDate": ["2021-05-31","2021-02-01"],
-                               "DataPointNameNumber": [12.2178, 78514]})
-            md.direct.firm_database.save_values(values=df, key_column="SecId", blank=md.direct.Blank.warning)
-
-        Errors:
-            AccessDeniedError: Raised when the user is not authenticated.
-
-            ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-            InternalServerError: Raised when the server encounters an unhandled error.
-
-            NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-            ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
-        """
-        if not isinstance(blank, Blank):
-            warnings.warn(
-                "The use of string values for the 'blank' parameter is deprecated and will be removed in the next major version. Use Blank enum values instead",
-                FutureWarning,
-                stacklevel=2,
-            )
-
-        blank = Blank[blank]
-        assert isinstance(blank, Blank)
-
-        if key_column not in values:
-            raise ValueErrorException(f"The key column '{key_column}' does not exist.")
-
-        values = self.filter_null_values(self.convert_to_objects(values), blank, key_column)
-
-        def get_values(column: str, value: Any, row: dict) -> Optional[RelValuesWithDatapoint]:
-            if column is key_column:
-                return None
-
-            assert isinstance(blank, Blank)
-            if value is None and blank is Blank.ignore:
-                return None
-            data_point = self.get_data_point_from_name(column)
-            single_value = self.is_a_valid_value(value, data_point, row[key_column])
-            return {
-                "dataPointId": data_point["id"],
-                "investmentId": row[key_column],
-                "singleValue": single_value,
-                "toDelete": self.get_to_delete(value, blank),
-            }
-
-        data: List[RelValuesWithDatapoint] = _mapper_data_frame_return_list(values, get_values)
-
-        return self._request_save_values(data)
-
-    def _request_save_values(self, data: List[RelValuesWithDatapoint]) -> ResultType:
-        url = f"{_config.custom_data_points_service_url()}v1/cdp/investments/values?type={self.database_type.value}"
-        result: ResultType = self._custom_database_api_request.do_put_request(url, json.dumps(data, ignore_nan=True))
-        return result
-
-
-my_database = _CustomDatabase(DatabaseCD.user, CustomDatabaseAPIBackend())
-firm_database = _CustomDatabase(DatabaseCD.firm, CustomDatabaseAPIBackend())
+import simplejson as json
+import warnings
+
+from abc import ABC
+from pandas import DataFrame
+from typing import List, Any, Optional, Dict, Union, Callable
+
+from . import _decorator, _error_messages
+from .._base import _logger
+from ._exceptions import ValueErrorException, ResourceNotFoundError
+from ._config import _Config
+from .data_type import Blank
+from ._data_type import DatabaseCD
+from ._utils import _mapper_data_frame_return_dict, _mapper_data_frame_return_list
+from ._data_objects import ValidCustomDataPointTypes, TypeValue
+from ._base_api import APIBackend
+
+
+_config = _Config()
+
+
+class CustomDatabaseAPIBackend(APIBackend):
+    """
+    Subclass to call the custom database API and handle any HTTP errors that occur.
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def _handle_custom_http_errors(self, res: Any) -> Any:
+        """
+        Handle HTTP errors with custom error messages
+        """
+        response_message = res.json()["message"]
+        if res.status_code == 404:
+            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
+            raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_CUSTOM_DATABASE) from None
+
+
+ResultType = Dict[str, Union[bool, str]]
+ListDatapointType = List[Dict[str, Any]]
+DictValues = Dict[str, TypeValue]
+RelValuesWithDatapoint = Dict[str, Union[TypeValue, List[DictValues]]]
+
+
+class _CustomDatabase(ABC):
+    def __init__(self, database_type: DatabaseCD, custom_database_api_request: CustomDatabaseAPIBackend):
+        self.database_type: DatabaseCD = database_type
+        self.all_data_points: ListDatapointType = []
+        self._custom_database_api_request = custom_database_api_request
+
+    def get_data_point_from_name(self, data_point_name: str, time_series: bool = False) -> Dict[str, str]:
+        data_points = self.get_all_data_points()
+        data_point = next(
+            (item for item in data_points if item["name"] == data_point_name),
+            None,
+        )
+
+        if data_point is None or "columnType" not in data_point:
+            raise ValueErrorException(f"The column '{data_point_name}' does not exist in the custom datapoints.")
+
+        start_with_ts = data_point["columnType"].startswith("TS")
+
+        if time_series and not start_with_ts:
+            raise ValueErrorException(f"The column '{data_point_name}' is not for a time series.")
+
+        if not time_series and start_with_ts:
+            raise ValueErrorException(f"The column '{data_point_name}' is not for a single value.")
+
+        return data_point
+
+    def get_all_data_points(self) -> ListDatapointType:
+        if not self.all_data_points:
+            url = f"{_config.custom_data_points_service_url()}v1/cdp/definitions?type={self.database_type.value}"
+            self.all_data_points = self._custom_database_api_request.do_get_request(url)
+        return self.all_data_points
+
+    def is_a_valid_value(self, value: Optional[TypeValue], data_point_definition: dict, investment: str) -> Optional[TypeValue]:
+        if value is None:
+            return value
+        validator = ValidCustomDataPointTypes(data_point_definition)
+        try:
+            result: TypeValue = validator.is_valid(value)
+            return result
+        except Exception as e:
+            raise ValueErrorException(f"Error in '{data_point_definition['name']}' column with '{investment}': {str(e)}")
+
+    def convert_to_objects(self, values: DataFrame) -> Any:
+        return values.astype(object).where(values.notnull(), None).where(values != "", None)
+
+    def filter_null_values(
+        self,
+        values: DataFrame,
+        blank: Blank,
+        key_column: str,
+        date_column: Optional[str] = None,
+    ) -> Any:
+        ops = Blank.options()
+        if blank is Blank.warning and values.isnull().values.any():
+            raise ValueErrorException(f"The dataframe contains null or blank values. \n" f"Please choose one of the following as a `blank` arg: {ops} \n") from None
+        ignore_columns = [
+            key_column,
+            date_column if date_column is not None else key_column,
+        ]
+        if blank is Blank.ignore and values.drop(list(set(ignore_columns)), axis=1).isnull().values.all():
+            raise ValueErrorException(f"All the dataframe values are null or blank. \n" f"Please choose one of the following as a `blank` arg: {ops} \n") from None
+        return values
+
+    def get_to_delete(self, value: TypeValue, blank: Blank) -> bool:
+        if blank is Blank.ignore:
+            return False
+        else:
+            if value is None:
+                return True
+        return False
+
+    @_decorator.typechecked
+    def save_historical_values(
+        self,
+        values: DataFrame,
+        key_column: str = "SecId",
+        date_column: str = "Date",
+        blank: Union[Blank, str] = Blank.warning,
+    ) -> ResultType:
+        """Saves historical time series values for data points in the user's or firm's database in Morningstar Direct.
+
+        Args:
+            values (:obj:`DataFrame`): A DataFrame object with the time series values to be saved in the user’s or firm’s database. The DataFrame columns should include:
+
+                * `SecId` - Column containing investment ID values. If a column named `SecId` is not present, the column name specified in the key_column argument will be used.
+                * `DataPointName` - Data point name which will be updated. Multiple data points can be updated in one request.
+                * `Date` - Column containing date values. If a column named `Date` is not present, the column name specified in the date_column argument will be used.
+
+                For example::
+
+                    ====================  ========  ===============  ===============  ===============
+                    SecId                   Date    DataPointName1   DataPointName2   DataPointName3
+                    ====================  ========  ===============  ===============  ===============
+                    <InvestmentId>         <date>       <value>          <value>          <value>
+                    <InvestmentId>         <date>       <value>          <value>          <value>
+                    ====================  ========  ===============  ===============  ===============
+
+            key_column (:obj:`str`): Name of the column containing investment ID values. If not specified, the column `SecId` will be used.
+
+            date_column (:obj:`str`): Name of the column containing date values. If not specified, the column `Date` will be used.
+
+            blank (:obj:`Blank`): Argument specifying how blank values in the DataFrame should be handled. Valid enum values for this argument are:
+
+                    * warning - Raises an error if the DataFrame contains at least one null or empty (str) value.
+                    * ignore - Saves all DataFrame values except for null or empty (str) values.
+                    * update - Replaces/updates all existing values with the provided values. Deletes any value that is sent as null, None or empty (str) values.
+
+        Returns:
+            DataFrame
+
+        :Examples:
+
+        ::
+
+            import morningstar_data as md
+            from pandas import DataFrame
+
+            df = DataFrame({"SecId": ["FOUSA00C3M", "F000010NJ5"],
+                            "Date": ["2022-02-10","2022-04-2"],
+                            "DataPointNameText": ["2","9"],
+                            "DataPointNameNumber": [12.2178, 78514]})
+
+            md.direct.my_database.save_historical_values(values=df, key_column="SecId", blank=md.direct.Blank.warning)
+
+
+
+        ::
+
+            import morningstar_data as md
+            from pandas import DataFrame
+
+            df = DataFrame({"SecId": ["FOUSA00C3M", "F000010NJ5"],
+                            "Date": ["2022-02-10","2022-04-2"],
+                            "DataPointNameText": ["2","9"],
+                            "DataPointNameNumber": [12.2178, 78514]})
+
+            md.direct.firm_database.save_historical_values(values=df, key_column="SecId", blank=md.direct.Blank.warning)
+
+        Errors:
+            AccessDeniedError: Raised when the user is not authenticated.
+
+            ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+            InternalServerError: Raised when the server encounters an unhandled error.
+
+            NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+            ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
+
+        """
+        if not isinstance(blank, Blank):
+            warnings.warn(
+                "The use of string values for the 'blank' parameter is deprecated and will be removed in the next major version. Use Blank enum values instead",
+                FutureWarning,
+                stacklevel=2,
+            )
+
+        blank = Blank[blank]
+        assert isinstance(blank, Blank)
+
+        if key_column not in values:
+            raise ValueErrorException(f"The key column '{key_column}' does not exist.")
+
+        if date_column not in values:
+            raise ValueErrorException(f"The date column '{date_column}' does not exist")
+
+        values = self.filter_null_values(self.convert_to_objects(values), blank, key_column, date_column)
+
+        def get_values(last_dict: Dict, column: str, value: Any, row: Dict) -> Dict:
+            if column in [key_column, date_column]:
+                return last_dict
+
+            date = self.is_a_valid_value(
+                row[date_column],
+                {
+                    "name": date_column,
+                    "columnType": "Date",
+                },
+                row[key_column],
+            )
+            data_point: Dict[str, str] = self.get_data_point_from_name(column, True)
+
+            assert isinstance(blank, Blank)
+            if value is None and blank is Blank.ignore:
+                return last_dict
+            ts_value = self.is_a_valid_value(value, data_point, row[key_column])
+            relation = f"{data_point['id']}-{row[key_column]}"
+
+            if relation not in last_dict:
+                last_dict[relation] = []
+
+            to_delete = self.get_to_delete(ts_value, blank)
+            last_dict[relation].append({"date": date, "value": ts_value, "toDelete": to_delete})
+            return last_dict
+
+        relations: DictValues = _mapper_data_frame_return_dict(values, get_values)
+        data: List[RelValuesWithDatapoint] = [
+            {
+                "dataPointId": relation.split("-")[0],
+                "investmentId": relation.split("-")[1],
+                "timeSeriesValue": points,
+            }
+            for relation, points in relations.items()
+        ]
+        return self._request_save_values(data)
+
+    @_decorator.typechecked
+    def save_values(
+        self,
+        values: DataFrame,
+        key_column: str = "SecId",
+        blank: Union[Blank, str] = Blank.warning,
+    ) -> ResultType:
+        """Saves values for data points in the user's or firm's database.
+
+        Args:
+            values (:obj:`DataFrame`): A DataFrame object with the values to be saved in the user's or firm's database. The DataFrame columns should include:
+
+                * `SecId` - Column containing investment ID values. If a column named `SecId` is not present, the column name specified in the key_column argument will be used.
+                * `DataPointName` - Data point name which will be updated. Multiple data points can be updated in one request.
+
+                For example::
+
+                    ====================  ===============  ===============  ===============
+                    SecId                 DataPointName1   DataPointName2   DataPointName3
+                    ====================  ===============  ===============  ===============
+                    <InvestmentId>            <value>          <value>          <value>
+                    <InvestmentId>            <value>          <value>          <value>
+                    ====================  ===============  ===============  ===============
+
+            key_column (:obj:`str`): Name of the column containing investment ID values. If not specified, the column `SecId` will be used.
+
+            blank (:obj:`Blank`): Argument specifying how blank values in the DataFrame should be handled. Valid enum values for this argument are:
+
+                * warning - Raises an error if the DataFrame contains at least one null or empty (str) value.
+                * ignore - Saves all DataFrame values except for null or empty (str) values.
+                * update - Replaces/updates all existing values with the provided values. Deletes any value that is sent as null, None or empty (str) values.
+        Returns:
+            DataFrame
+
+        :Examples:
+
+        ::
+
+            import morningstar_data as md
+            from pandas import DataFrame
+            df = DataFrame({"SecId": ["FOUSA00C3M", "F000010NJ5"],
+                               "DataPointNameText": ["2","9"],
+                               "DataPointNameDate": ["2022-02-10","2022-04-2"],
+                               "DataPointNameNumber": [12.2178, 78514]})
+            md.direct.my_database.save_values(values=df, key_column="SecId", blank=md.direct.Blank.warning)
+
+        ::
+
+            import morningstar_data as md
+            from pandas import DataFrame
+            df = DataFrame({"SecId": ["FOUSA00C3M", "F000010NJ5"],
+                               "DataPointNameText": ["2","9"],
+                               "DataPointNameDate": ["2021-05-31","2021-02-01"],
+                               "DataPointNameNumber": [12.2178, 78514]})
+            md.direct.firm_database.save_values(values=df, key_column="SecId", blank=md.direct.Blank.warning)
+
+        Errors:
+            AccessDeniedError: Raised when the user is not authenticated.
+
+            ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+            InternalServerError: Raised when the server encounters an unhandled error.
+
+            NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+            ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
+        """
+        if not isinstance(blank, Blank):
+            warnings.warn(
+                "The use of string values for the 'blank' parameter is deprecated and will be removed in the next major version. Use Blank enum values instead",
+                FutureWarning,
+                stacklevel=2,
+            )
+
+        blank = Blank[blank]
+        assert isinstance(blank, Blank)
+
+        if key_column not in values:
+            raise ValueErrorException(f"The key column '{key_column}' does not exist.")
+
+        values = self.filter_null_values(self.convert_to_objects(values), blank, key_column)
+
+        def get_values(column: str, value: Any, row: dict) -> Optional[RelValuesWithDatapoint]:
+            if column is key_column:
+                return None
+
+            assert isinstance(blank, Blank)
+            if value is None and blank is Blank.ignore:
+                return None
+            data_point = self.get_data_point_from_name(column)
+            single_value = self.is_a_valid_value(value, data_point, row[key_column])
+            return {
+                "dataPointId": data_point["id"],
+                "investmentId": row[key_column],
+                "singleValue": single_value,
+                "toDelete": self.get_to_delete(value, blank),
+            }
+
+        data: List[RelValuesWithDatapoint] = _mapper_data_frame_return_list(values, get_values)
+
+        return self._request_save_values(data)
+
+    def _request_save_values(self, data: List[RelValuesWithDatapoint]) -> ResultType:
+        url = f"{_config.custom_data_points_service_url()}v1/cdp/investments/values?type={self.database_type.value}"
+        result: ResultType = self._custom_database_api_request.do_put_request(url, json.dumps(data, ignore_nan=True))
+        return result
+
+
+my_database = _CustomDatabase(DatabaseCD.user, CustomDatabaseAPIBackend())
+firm_database = _CustomDatabase(DatabaseCD.firm, CustomDatabaseAPIBackend())
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/holdings.py` & `morningstar_data-1.3.0/morningstar_data/direct/holdings.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,826 +1,826 @@
-import simplejson as json
-import os
-import time
-import uuid
-import warnings
-from collections import defaultdict
-from datetime import datetime
-from typing import Any, Dict, List, Optional, Union
-from urllib.parse import quote
-from urllib.request import urlopen
-
-import pandas as pd
-from pandas import DataFrame
-
-
-from .. import datalake
-from .._base import _logger
-from . import _decorator, _utils
-from . import investment as inv
-from . import portfolio
-from ._base_api import APIBackend
-from ._config import _Config
-from ._config_key import FORMAT_DATE
-from ._error_messages import (
-    BAD_REQUEST_ERROR_INCLUDE_ALL_DATE,
-    BAD_REQUEST_ERROR_NO_START_DATE,
-    BAD_REQUEST_ERROR_INVALID_INVESTMENT_ID,
-    BAD_REQUEST_ERROR_NO_INVESTMENT_IDS,
-    BAD_REQUEST_ERROR_NO_PORTFOLIO_DATA,
-    BAD_REQUEST_ERROR_NO_START_DATE,
-    BAD_REQUEST_ERROR_INVALID_LOOKTHROUGH_HOLDING_TYPE,
-    BAD_REQUEST_ERROR_INVALID_PORTFOLIO_ID,
-)
-from ._exceptions import BadRequestException, NetworkExceptionError
-from ._backend_apis._holdings_backend import HoldingAPIBackend, FoFAPIBackend, AMSAPIBackend
-
-_config = _Config()
-
-_holding_api_request = HoldingAPIBackend()
-_fof_api_request = FoFAPIBackend()
-_ams_api_request = AMSAPIBackend()
-
-MASTER_PORTFOLIO_ID = "MasterPortfolio Id"
-
-
-@_decorator.typechecked
-def holdings(
-    investment_ids: List[str],
-    date: Optional[str] = None,
-    start_date: Optional[str] = None,
-    end_date: Optional[str] = None,
-) -> DataFrame:
-    warnings.warn(
-        "The holdings function is deprecated and will be removed in the next major version. Use get_holdings instead",
-        FutureWarning,
-        stacklevel=2,
-    )
-    return get_holdings(investment_ids, date, start_date, end_date)
-
-
-@_decorator.typechecked
-def get_holdings(
-    investment_ids: List[str],
-    date: Optional[str] = None,
-    start_date: Optional[str] = None,
-    end_date: Optional[str] = None,
-) -> DataFrame:
-    """Returns holdings for the specified investments and date or date range. If the date is not specified, the function uses the latest portfolio date by default.
-
-    Args:
-        investment_ids (:obj:`list`): A list of investment IDs. The investment ID format is SecId;Universe or just SecId.
-            For example: ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"].
-        date (:obj:`str`, `optional`): The portfolio date for which to retrieve data. The format is YYYY-MM-DD.
-            For example, "2020-01-01". If a date is provided, then the `start_date` and `end_date` parameters are ignored.
-            An exception is thrown if `start_date` or `end_date` is provided along with `date`.
-        start_date (:obj:`str`, `optional`): The start date for retrieving data. The format is
-            YYYY-MM-DD. For example, "2020-01-01". An exception is thrown if `date` is provided along with `start_date`.
-        end_date (:obj:`str`, `optional`): The end date for retrieving data. If no value is provided for
-            `end_date`, current date will be used. The format is YYYY-MM-DD. For example, "2020-01-01". An exception is
-            thrown if `date` is provided along with `end_date`.
-
-    Returns:
-        DataFrame: A DataFrame object with holdings data. DataFrame columns include:
-
-        * investmentId
-        * masterPortfolioId
-        * portfolioDate
-        * holdingId
-        * bondId
-        * name
-        * secId
-        * isin
-        * cusip
-        * weight
-        * shares
-        * marketValue
-        * sharesChanged
-        * currency
-        * ticker
-        * detailHoldingType
-
-    Raises:
-        ValueErrorException: Raised when the `investment_ids` parameter is invalid.
-
-    Examples:
-        Retrieve holdings for investment "FOUSA00KZH" on "2020-12-31".
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.get_holdings(investment_ids=["FOUSA00KZH"], date="2020-12-31")
-        df
-
-    :Output:
-        =============  =================  ===  ======  =================
-        investmentId   masterPortfolioId  ...  ticker  detailHoldingType
-        =============  =================  ===  ======  =================
-        FOUSA00KZH     6079               ...  CBRE    EQUITY
-        FOUSA00KZH     6079               ...  GOOGL   EQUITY
-        ...
-        =============  =================  ===  ======  =================
-
-    """
-    _validate_investment_ids(investment_ids)
-    _validate_date(date, start_date, end_date)
-
-    investment_date_info = _get_dates(investment_ids, date, start_date, end_date)
-    params = []
-    master_portfolio_id_investment_id_dict = defaultdict(list)
-    for sec_id, date_info in investment_date_info.items():
-        if date_info not in params:
-            params.append(date_info)
-        master_portfolio_id_investment_id_dict[date_info.get("masterPortfolioId", "")].append(sec_id)
-
-    url = f"{_config.securitydata_service_url()}v1/securities/holdings"
-    response_json = _holding_api_request.do_post_request(url, json.dumps(params, ignore_nan=True))
-    if not isinstance(response_json, list) or not response_json:
-        return DataFrame()
-    details = []
-    for holdings_info in response_json:
-        master_portfolio_id = holdings_info.get("masterPortfolioId", "")
-        holdings_date_info = holdings_info.get("holdings", dict())
-        for single_date, holdings in holdings_date_info.items():
-            for value in master_portfolio_id_investment_id_dict.get(master_portfolio_id, ""):
-                details.extend(
-                    [
-                        {
-                            "portfolioDate": single_date,
-                            "investmentId": value,
-                            "masterPortfolioId": master_portfolio_id,
-                            "holdingId": x.get("id", ""),
-                            "bondId": x.get("bondId", ""),
-                            "name": x.get("name", ""),
-                            "secId": x.get("secId", ""),
-                            "isin": x.get("isin", ""),
-                            "cusip": x.get("cusip", ""),
-                            "weight": x.get("weight", ""),
-                            "shares": x.get("shares", ""),
-                            "marketValue": x.get("marketValue", ""),
-                            "sharesChanged": x.get("sharesChanged", ""),
-                            "currency": x.get("currency", ""),
-                            "ticker": x.get("ticker", ""),
-                            "detailHoldingType": x.get("detailHoldingType", ""),
-                        }
-                        for x in holdings
-                    ]
-                )
-    return DataFrame(details)
-
-
-def _get_dates_by_investments(investment_ids: list) -> List[Any]:
-    ids = quote(",".join(investment_ids), "utf-8")
-    url = f"{_config.securitydata_service_url()}v2/securities/{ids}/portfolio-dates"
-    result: List[Any] = _holding_api_request.do_get_request(url)
-    return result
-
-
-@_decorator.typechecked
-def holding_dates(investment_ids: List[str]) -> DataFrame:
-    warnings.warn(
-        "The holding_dates function is deprecated and will be removed in the next major version. Use get_holding_dates instead",
-        FutureWarning,
-        stacklevel=2,
-    )
-    return get_holding_dates(investment_ids)
-
-
-@_decorator.typechecked
-def get_holding_dates(investment_ids: List[str]) -> DataFrame:
-    """Returns all dates with available holdings data for the given investment.
-
-    Args:
-        investment_ids (:obj:`list`): A list of investment IDs. The investment ID format is SecId;Universe or just SecId.
-            For example: ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"].
-
-    Returns:
-        DataFrame: A DataFrame object with portfolio date data. DataFrame columns include:
-
-       * secId
-       * masterPortfolioId
-       * date
-       * suppression
-       * suppressionHoldingNumber
-
-    Examples:
-        Retrieve portfolio dates for investment "FOUSA00KZH".
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.get_holding_dates(investment_ids=["FOUSA06JNH"])
-        df
-
-    :Output:
-        ==========  =================  ==========  ===========  ========================
-        secId       masterPortfolioId  date        suppression  suppressionHoldingNumber
-        ==========  =================  ==========  ===========  ========================
-        FOUSA06JNH  210311             2021-08-31  False        None
-        FOUSA06JNH  210311             2021-07-31  False        None
-        ...
-        ==========  =================  ==========  ===========  ========================
-
-    """
-    if not investment_ids:
-        raise BadRequestException(BAD_REQUEST_ERROR_NO_INVESTMENT_IDS) from None
-    response_json = _get_dates_by_investments(investment_ids)
-    if isinstance(response_json, list) and response_json:
-        details = []
-        for date_info in response_json:
-            sec_id = date_info.get("secId", "")
-            master_portfolio_id = date_info.get("masterPortfolioId", "")
-            details.extend(
-                [
-                    {
-                        "secId": sec_id,
-                        "masterPortfolioId": master_portfolio_id,
-                        "date": portfolio_date.get("date", ""),
-                        "suppression": portfolio_date.get("suppression", False),
-                        "suppressionHoldingNumber": portfolio_date.get("suppressionHoldingNumber", None),
-                    }
-                    for portfolio_date in date_info.get("portfolioDates", [])
-                ]
-            )
-        return DataFrame(details)
-    else:
-        return DataFrame()
-
-
-def _get_dates(
-    investment_ids: list,
-    date: Optional[str] = None,
-    start_date: Optional[str] = None,
-    end_date: Optional[str] = None,
-) -> dict:
-    dates_raw: Dict[str, Optional[str]] = {
-        "date": date,
-        "start_date": start_date,
-        "end_date": end_date,
-    }
-    dates: Dict[str, str] = {}
-
-    for key, value in dates_raw.items():
-        if value is not None and len(value.strip()) > 0:
-            dates[key] = _utils._format_date(value)
-        elif key == "end_date" and dates_raw["start_date"] is not None:
-            dates[key] = _utils._format_date(time.strftime(FORMAT_DATE, time.localtime()))
-
-    response_json = _get_dates_by_investments(investment_ids)
-    if not isinstance(response_json, list) or not response_json:
-        raise BadRequestException(BAD_REQUEST_ERROR_NO_PORTFOLIO_DATA) from None
-
-    if not bool(dates):
-        return _handle_no_date(response_json)
-    elif "date" in dates:
-        return _handle_single_date(response_json, **dates)
-
-    return _handle_date_range(response_json, **dates)
-
-
-def _validate_date(date: Optional[str], start_date: Optional[str], end_date: Optional[str]) -> None:
-    if date:
-        if start_date or end_date:
-            raise BadRequestException(BAD_REQUEST_ERROR_INCLUDE_ALL_DATE) from None
-    else:
-        if not start_date and end_date:
-            raise BadRequestException(BAD_REQUEST_ERROR_NO_START_DATE) from None
-
-
-def _handle_single_date(date_info_list: list, date: str) -> dict:
-    investment_date_info = dict()
-    for date_info in date_info_list:
-        available_date = _get_available_date(date, date_info)
-        if available_date is not None:
-            master_portfolio_id = date_info.get("masterPortfolioId", "")
-            investment_date_info[date_info.get("secId", "")] = {
-                "masterPortfolioId": master_portfolio_id,
-                "portfolioDates": [available_date],
-            }
-    return investment_date_info
-
-
-def _get_available_date(date: str, date_info: dict = dict()) -> Optional[str]:
-    date_objs = date_info.get("portfolioDates", [])
-    available_date = None
-    for date_obj in date_objs:
-        if date_obj.get("date", "") == date:
-            available_date = date
-            break
-        elif date_obj.get("date", "") < date and available_date is None:
-            available_date = date_obj.get("date", "")
-    return available_date
-
-
-def _handle_no_date(date_info_list: list) -> dict:
-    investment_date_info = dict()
-    for date_info in date_info_list:
-        portfolio_dates = date_info.get("portfolioDates", [])
-        if portfolio_dates:
-            date = next(
-                (x.get("date", "") for x in portfolio_dates if x.get("date", "") is not None and len(x.get("date", "")) > 0),
-                None,
-            )
-            if date is not None and len(date) > 0:
-                master_portfolio_id = date_info.get("masterPortfolioId", "")
-                investment_date_info[date_info.get("secId", "")] = {
-                    "masterPortfolioId": master_portfolio_id,
-                    "portfolioDates": [date],
-                }
-    return investment_date_info
-
-
-def _handle_date_range(date_info_list: list, start_date: str, end_date: str) -> dict:
-    investment_date_info = dict()
-    for date_info in date_info_list:
-        sec_id = date_info.get("secId", "")
-        master_portfolio_id = date_info.get("masterPortfolioId", "")
-        portfolio_dates = date_info.get("portfolioDates", [])
-        date_list = []
-        for portfolio_date in portfolio_dates:
-            single_date = portfolio_date.get("date", "")
-            if start_date <= single_date <= end_date:
-                date_list.append(single_date)
-        if date_list:
-            investment_date_info[sec_id] = {
-                "masterPortfolioId": master_portfolio_id,
-                "portfolioDates": date_list,
-            }
-    return investment_date_info
-
-
-def _validate_investment_ids(investment_ids: List[str]) -> None:
-    if not investment_ids:
-        raise BadRequestException(BAD_REQUEST_ERROR_NO_INVESTMENT_IDS) from None
-    elif [x for x in investment_ids if len(x.split(";")[0]) != 10]:
-        raise BadRequestException(BAD_REQUEST_ERROR_INVALID_INVESTMENT_ID) from None
-
-
-def _get_ids_from_lake_house(df_lookthrough: pd.DataFrame) -> pd.DataFrame:
-    sql = """SELECT distinct
-            a.investment_id
-            ,a.isin
-            ,a.cusip
-            ,a.weight
-            ,a.marketValue as market_value
-            ,a.security_name
-            ,a.currency
-            ,a.morningstar_instrument_type_code
-            ,b.entity_id
-            ,b.morningstar_entity_name
-            ,b.performance_id as primary_performance_id
-            FROM lookthrough_temp a
-                left join platform__reference__prd.investment_lookup b
-                    on a.investment_id=b.investment_id and b.is_primary = True
-            where (b.is_primary = True or b.investment_id is null)
-    """
-    df = datalake.query(sql, temp_tables=[datalake.TempTable("lookthrough_temp", df_lookthrough)])
-    return df
-
-
-def _get_fof_secid_and_investment_types(df_top_level_holdings: pd.DataFrame) -> pd.DataFrame:
-    # create DataFrame with Direct secId and Direct securityType
-    # df_top_level_holdings_expanded = df_top_level_holdings["HoldingId"].str.split(";", expand=True).rename(columns={0: "secid", 1: "sectype"})
-    df_top_level_holdings[["fof_secid", "fof_sectype"]] = df_top_level_holdings["HoldingId"].str.split(";", expand=True).rename(columns={0: "fof_secid", 1: "fof_sectype"})
-    if MASTER_PORTFOLIO_ID in df_top_level_holdings.columns:
-        df_top_level_holdings["masterPortfolioId"] = df_top_level_holdings[MASTER_PORTFOLIO_ID].astype("Int64")
-
-    query_str = """with cte as (
-        SELECT distinct --performance_id,
-        case
-            when left(investment_id,2) ='E0' and fund_id is null
-                then performance_id
-            when is_primary=False
-                then performance_id
-            else investment_id
-        end as sec_id
-        ,investment_id
-        ,morningstar_investment_name
-        ,case
-            when morningstar_instrument_type_code is not null
-                then morningstar_instrument_type_code
-            when left(investment_id,2) in ('FE','FC','FO','FH','FM','FV','SC')
-                then left(investment_id,2)
-            when left(investment_id,2) = 'F0'
-                then 'FO'
-            when left(investment_id,2) ='SA'
-                then 'FS'
-            when left(investment_id,2) ='E0' and fund_id is null
-                then 'E'
-            when left(investment_id,2) ='E0' and fund_id is not null
-                then 'FC'
-            else null
-        end as morningstar_instrument_type_code
-        ,is_primary
-        FROM platform__reference__prd.investment_lookup a
-        where
-        (
-            performance_id is not null
-            or
-            morningstar_instrument_type_code in ('BC','12','BZ','BY','B','BT','NE','BH','IP','NE','NB','NC','BG','BD','ND')
-        )
-        and
-            left(investment_id,2) not in ('XI','VA')
-        and
-        (
-            a.performance_id in (select fof_secid from temp_top_level_holdings_expanded)
-            or
-            a.investment_id in (select fof_secid from temp_top_level_holdings_expanded)
-        )
-    )
-    select
-        a.weight as weighting,
-        a.Name as securityName,
-        b.investment_id as secId,
-        coalesce(trim(b.morningstar_instrument_type_code), 'Q') as detailHoldingTypeId
-    from
-        temp_top_level_holdings_expanded a
-        left join cte b
-            on a.fof_secid=b.sec_id
-    """
-
-    return datalake.query(
-        query_str=query_str,
-        temp_tables=[
-            datalake.TempTable(name="temp_top_level_holdings_expanded", df=df_top_level_holdings),
-        ],
-    )
-
-
-def _get_lookthrough_holdings_from_fof_api(portfolio_id: str, df_top_level_holdings: DataFrame) -> DataFrame:
-
-    from ._backend_apis._signed_url_backend import SignedUrlBackend
-
-    _signed_url_request = SignedUrlBackend()
-
-    # 'XI' represents an index, which is unsupported by FoF API
-    if "XI" in df_top_level_holdings["SecurityType"].values:
-        raise BadRequestException(BAD_REQUEST_ERROR_INVALID_LOOKTHROUGH_HOLDING_TYPE)
-
-    _logger.info(
-        "Fetching FOF comptabile secid and investment types from investments_lookup table in lakehouse along with required fields from top level holdings to pass to FOF API."
-    )
-    df_fof_sec_id_investment_types = _get_fof_secid_and_investment_types(df_top_level_holdings)
-
-    _logger.info("Generating a unique id for each row in the top level holdings.")
-    # Add a UUID as value for clientSecurityGuid for each holding
-
-    df_fof_sec_id_investment_types = df_fof_sec_id_investment_types.rename(
-        columns={
-            "secid": "secId",
-            "weighting": "weighting",
-            "detailholdingtypeid": "detailHoldingTypeId",
-            "securityname": "securityName",
-        }
-    )
-
-    df_fof_sec_id_investment_types["clientSecurityGuid"] = [str(uuid.uuid4()) for _ in range(len(df_fof_sec_id_investment_types.index))]
-
-    _logger.info("Extracting fof_secid, investment_type, weight and masterportfolio id into json to pass to FOF API")
-    holdings_json = df_fof_sec_id_investment_types.to_json(orient="records")
-
-    holdings_parsed = json.loads(holdings_json)  # This is sent to FOF API in the holdings field
-
-    fof_post_url = f"{_config.fof_api_url()}portfolios/drilldown/{portfolio_id.split(';')[0]}/ALCustomerHoldings"
-    payload = json.dumps(
-        {
-            "clientPortfolioGuid": str(uuid.uuid4()),
-            "portfolioDate": str(datetime.now().strftime("%Y%m%d")),
-            "currencyId": "USD",
-            "holdings": holdings_parsed,  # The SQL query returns the columns in exactly the same format as required by FOF API
-        }
-    )
-
-    _logger.info("Submitting request to FOF API to run lookthrough holdings.")
-    _logger.debug(f"Sending request to {fof_post_url}")
-
-    # MD proxy api will poll FOF API and return the signed url to download the lookthrough holdings
-    signed_url = _fof_api_request.do_post_request(fof_post_url, payload)["jobId"]  # Returns reponse.content as string
-
-    _logger.info("Submitting request to download lookthrough holdsings from signed url.")
-    _logger.debug(f"Sending request to {signed_url}")
-    look_through_holdings_reponse = _signed_url_request.do_get_request(signed_url)  # The reponse includes lookthrough holdings as json
-
-    _logger.info("Got response from Signed url request")
-    look_through_holdings_json = json.loads(look_through_holdings_reponse)
-    holdings = look_through_holdings_json["holdings"]
-    _logger.debug(f"Got {len(holdings)} lookthrough holdings.")
-
-    df_look_through_holdings = pd.DataFrame(holdings)
-    return df_look_through_holdings
-
-
-def _has_ams_license_for_isin() -> bool:
-    ams_get_url = f"{_config.al_proxy_api_url()}/v2/ams/api/user/entitlements"
-    response = _ams_api_request.do_get_request(ams_get_url)
-
-    data_groups = response["DataGroups"]
-    for data_group in data_groups:
-        if ((data_group["IdType"] == "UNIVERSEID" and data_group["DataGroupId"] == "ALL") or data_group["DataGroupId"] == "CUSIP") and data_group["Permission"] == 1:
-            return True
-    return False
-
-
-# temporary function until this data is added to Lake House
-def _morningstar_investment_type_id_name_mapping() -> pd.DataFrame:
-    return pd.DataFrame(
-        [
-            {"morningstar_instrument_type_code": "0", "morningstar_instrument_type_name": "Muni Bond - Unspecified"},
-            {"morningstar_instrument_type_code": "1", "morningstar_instrument_type_name": "Muni Bond - General Obligation"},
-            {"morningstar_instrument_type_code": "12", "morningstar_instrument_type_name": "Muni Bond - Revenue"},
-            {
-                "morningstar_instrument_type_code": "13",
-                "morningstar_instrument_type_name": "Muni Bond - Cash (Retired after Oct 2022)",
-            },
-            {"morningstar_instrument_type_code": "14", "morningstar_instrument_type_name": "Muni Bond - Double Barrelled"},
-            {"morningstar_instrument_type_code": "AF", "morningstar_instrument_type_name": "Alternatives - Farm & Timber Land"},
-            {"morningstar_instrument_type_code": "AI", "morningstar_instrument_type_name": "Alternatives - Infrastructure"},
-            {
-                "morningstar_instrument_type_code": "AM",
-                "morningstar_instrument_type_name": "Alternatives - Master Investment Trust",
-            },
-            {"morningstar_instrument_type_code": "AP", "morningstar_instrument_type_name": "Alternatives - Private Equity"},
-            {"morningstar_instrument_type_code": "AR", "morningstar_instrument_type_name": "Alternatives - Real Estate"},
-            {"morningstar_instrument_type_code": "B", "morningstar_instrument_type_name": "Bond - Corporate Bond"},
-            {"morningstar_instrument_type_code": "BB", "morningstar_instrument_type_name": "Bond - Short-term Corporate Bills"},
-            {"morningstar_instrument_type_code": "BC", "morningstar_instrument_type_name": "Bond - Convertible"},
-            {"morningstar_instrument_type_code": "BD", "morningstar_instrument_type_name": "Bond - Gov't Agency Debt"},
-            {"morningstar_instrument_type_code": "BG", "morningstar_instrument_type_name": "Bond - Gov't Agency Pass-Thru"},
-            {"morningstar_instrument_type_code": "BH", "morningstar_instrument_type_name": "Bond - Non-Agency Residential MBS"},
-            {"morningstar_instrument_type_code": "BL", "morningstar_instrument_type_name": "Bond Index - Future"},
-            {"morningstar_instrument_type_code": "BM", "morningstar_instrument_type_name": "Bond - Non-U.S. Gov't Agency MBS"},
-            {
-                "morningstar_instrument_type_code": "BO",
-                "morningstar_instrument_type_name": "Bond Index - Option (Call) (Consolidation to FD after Oct 2022)",
-            },
-            {
-                "morningstar_instrument_type_code": "BP",
-                "morningstar_instrument_type_name": "Bond Index - Option (Put) (Consolidation to FD after Oct 2022)",
-            },
-            {"morningstar_instrument_type_code": "BQ", "morningstar_instrument_type_name": "Bond - Undefined"},
-            {"morningstar_instrument_type_code": "BR", "morningstar_instrument_type_name": "Bond - Bank Loans"},
-            {"morningstar_instrument_type_code": "BT", "morningstar_instrument_type_name": "Bond - Gov't/Treasury"},
-            {"morningstar_instrument_type_code": "BU", "morningstar_instrument_type_name": "Bond - Units"},
-            {"morningstar_instrument_type_code": "BW", "morningstar_instrument_type_name": "Bond - Warrants/Rights (Call)"},
-            {"morningstar_instrument_type_code": "BX", "morningstar_instrument_type_name": "Bond - Warrants/Rights (Put)"},
-            {"morningstar_instrument_type_code": "BY", "morningstar_instrument_type_name": "Bond - Asset Backed"},
-            {"morningstar_instrument_type_code": "BZ", "morningstar_instrument_type_name": "Bond - Supranational"},
-            {"morningstar_instrument_type_code": "C", "morningstar_instrument_type_name": "Cash"},
-            {"morningstar_instrument_type_code": "CA", "morningstar_instrument_type_name": "Cash - Collateral"},
-            {
-                "morningstar_instrument_type_code": "CC",
-                "morningstar_instrument_type_name": "Cash - Option (Call) (Consolidation to CY after Oct 2022)",
-            },
-            {"morningstar_instrument_type_code": "CD", "morningstar_instrument_type_name": "Cash - CD/Time Deposit"},
-            {"morningstar_instrument_type_code": "CH", "morningstar_instrument_type_name": "Cash - Currency"},
-            {"morningstar_instrument_type_code": "CL", "morningstar_instrument_type_name": "Currency - Future"},
-            {"morningstar_instrument_type_code": "CN", "morningstar_instrument_type_name": "Bond - Contingent Convertible"},
-            {
-                "morningstar_instrument_type_code": "CO",
-                "morningstar_instrument_type_name": "Cash - Option (Put) (Consolidation to CZ after Oct 2022)",
-            },
-            {"morningstar_instrument_type_code": "CP", "morningstar_instrument_type_name": "Cash - Commercial Paper"},
-            {"morningstar_instrument_type_code": "CQ", "morningstar_instrument_type_name": "Cash - Future Offset"},
-            {"morningstar_instrument_type_code": "CR", "morningstar_instrument_type_name": "Cash - Repurchase Agreement"},
-            {"morningstar_instrument_type_code": "CS", "morningstar_instrument_type_name": "Currency - Swap"},
-            {"morningstar_instrument_type_code": "CT", "morningstar_instrument_type_name": "Bond - Capital Contingent Debt"},
-            {"morningstar_instrument_type_code": "CU", "morningstar_instrument_type_name": "Currency - Forward"},
-            {
-                "morningstar_instrument_type_code": "CV",
-                "morningstar_instrument_type_name": "Currency - Warrants\\Rights (Call) (Consolidation to CY after Oct 2022)",
-            },
-            {
-                "morningstar_instrument_type_code": "CX",
-                "morningstar_instrument_type_name": "Currency - Warrants\\Rights (Put) (Consolidation to CZ after Oct 2022)",
-            },
-            {"morningstar_instrument_type_code": "CY", "morningstar_instrument_type_name": "Currency Option (Call)"},
-            {"morningstar_instrument_type_code": "CZ", "morningstar_instrument_type_name": "Currency Option (Put)"},
-            {"morningstar_instrument_type_code": "DA", "morningstar_instrument_type_name": "Bond - Future"},
-            {"morningstar_instrument_type_code": "DB", "morningstar_instrument_type_name": "Bond - Option (Call)"},
-            {"morningstar_instrument_type_code": "DC", "morningstar_instrument_type_name": "Commodity - Option (Call)"},
-            {"morningstar_instrument_type_code": "DD", "morningstar_instrument_type_name": "Commodity"},
-            {"morningstar_instrument_type_code": "DE", "morningstar_instrument_type_name": "Bond - Option (Put)"},
-            {"morningstar_instrument_type_code": "DG", "morningstar_instrument_type_name": "Equity - Future"},
-            {"morningstar_instrument_type_code": "DH", "morningstar_instrument_type_name": "Equity - Option (Call)"},
-            {"morningstar_instrument_type_code": "DI", "morningstar_instrument_type_name": "Equity - Option (Put)"},
-            {"morningstar_instrument_type_code": "DJ", "morningstar_instrument_type_name": "Other - Future"},
-            {"morningstar_instrument_type_code": "DM", "morningstar_instrument_type_name": "Commodity - Future"},
-            {
-                "morningstar_instrument_type_code": "DO",
-                "morningstar_instrument_type_name": "Bond - Collateralized Debt Obligations (CDO/CBO)",
-            },
-            {"morningstar_instrument_type_code": "DP", "morningstar_instrument_type_name": "Commodity - Option (Put)"},
-            {
-                "morningstar_instrument_type_code": "DS",
-                "morningstar_instrument_type_name": "Bond - Sub-sovereign Government Debt",
-            },
-            {"morningstar_instrument_type_code": "E", "morningstar_instrument_type_name": "Equity"},
-            {"morningstar_instrument_type_code": "EC", "morningstar_instrument_type_name": "Equity Index - Option (Call)"},
-            {"morningstar_instrument_type_code": "EL", "morningstar_instrument_type_name": "Equity Index - Future"},
-            {"morningstar_instrument_type_code": "EP", "morningstar_instrument_type_name": "Equity Index - Option (Put)"},
-            {"morningstar_instrument_type_code": "EQ", "morningstar_instrument_type_name": "Equity - Undefined"},
-            {"morningstar_instrument_type_code": "ER", "morningstar_instrument_type_name": "Equity - REIT"},
-            {"morningstar_instrument_type_code": "EU", "morningstar_instrument_type_name": "Equity - Units"},
-            {"morningstar_instrument_type_code": "EV", "morningstar_instrument_type_name": "Equity - Warrants/Rights (Put)"},
-            {"morningstar_instrument_type_code": "EW", "morningstar_instrument_type_name": "Equity - Warrants/Rights (Call)"},
-            {"morningstar_instrument_type_code": "EX", "morningstar_instrument_type_name": "Mutual Fund - Unspecified"},
-            {"morningstar_instrument_type_code": "FC", "morningstar_instrument_type_name": "Mutual Fund - Closed End"},
-            {"morningstar_instrument_type_code": "FD", "morningstar_instrument_type_name": "Other Fixed Income Derivative"},
-            {"morningstar_instrument_type_code": "FE", "morningstar_instrument_type_name": "Mutual Fund - ETF"},
-            {"morningstar_instrument_type_code": "FH", "morningstar_instrument_type_name": "Mutual Fund - Hedge Fund"},
-            {"morningstar_instrument_type_code": "FM", "morningstar_instrument_type_name": "Mutual Fund - Money Market"},
-            {"morningstar_instrument_type_code": "FO", "morningstar_instrument_type_name": "Mutual Fund - Open End"},
-            {"morningstar_instrument_type_code": "FS", "morningstar_instrument_type_name": "Mutual Fund - Separate Account"},
-            {"morningstar_instrument_type_code": "FV", "morningstar_instrument_type_name": "Mutual Fund - Variable Annuity"},
-            {"morningstar_instrument_type_code": "FZ", "morningstar_instrument_type_name": "Mutual Fund - Client Portfolio"},
-            {"morningstar_instrument_type_code": "GA", "morningstar_instrument_type_name": "Bond - Non-US Gov't Agency CMO"},
-            {"morningstar_instrument_type_code": "GC", "morningstar_instrument_type_name": "Bond - Global Non-Agency CMO"},
-            {"morningstar_instrument_type_code": "GM", "morningstar_instrument_type_name": "Bond - Global Non-Agency MBS"},
-            {"morningstar_instrument_type_code": "GS", "morningstar_instrument_type_name": "Bond - Short-term Government Bills"},
-            {"morningstar_instrument_type_code": "IP", "morningstar_instrument_type_name": "Bond - Corp Inflation Protected"},
-            {"morningstar_instrument_type_code": "IS", "morningstar_instrument_type_name": "Inflation Swap"},
-            {"morningstar_instrument_type_code": "IT", "morningstar_instrument_type_name": "Income Trust"},
-            {
-                "morningstar_instrument_type_code": "LO",
-                "morningstar_instrument_type_name": "Bond - Collateralized Loan Obligations (CLO)",
-            },
-            {"morningstar_instrument_type_code": "NB", "morningstar_instrument_type_name": "Bond - Commercial MBS"},
-            {"morningstar_instrument_type_code": "NC", "morningstar_instrument_type_name": "Bond - Gov't Agency CMO"},
-            {"morningstar_instrument_type_code": "ND", "morningstar_instrument_type_name": "Bond - Covered Bond"},
-            {"morningstar_instrument_type_code": "NE", "morningstar_instrument_type_name": "Bond - Gov't Agency ARM"},
-            {"morningstar_instrument_type_code": "NR", "morningstar_instrument_type_name": "Bond - U.S. Agency Credit Risk CMO"},
-            {"morningstar_instrument_type_code": "OO", "morningstar_instrument_type_name": "Cash - Option Offset"},
-            {"morningstar_instrument_type_code": "OS", "morningstar_instrument_type_name": "Cash - Swap Offset"},
-            {"morningstar_instrument_type_code": "OT", "morningstar_instrument_type_name": "Cash - Forward Offset"},
-            {"morningstar_instrument_type_code": "P", "morningstar_instrument_type_name": "Preferred Stock"},
-            {"morningstar_instrument_type_code": "PA", "morningstar_instrument_type_name": "Participating Preferred"},
-            {"morningstar_instrument_type_code": "PC", "morningstar_instrument_type_name": "Convertible Preferred"},
-            {"morningstar_instrument_type_code": "PP", "morningstar_instrument_type_name": "Property"},
-            {"morningstar_instrument_type_code": "PS", "morningstar_instrument_type_name": "Interest Rate Swaption - Payer"},
-            {"morningstar_instrument_type_code": "Q", "morningstar_instrument_type_name": "Unidentified Holding"},
-            {"morningstar_instrument_type_code": "QQ", "morningstar_instrument_type_name": "Other Assets And Liabilities"},
-            {"morningstar_instrument_type_code": "RS", "morningstar_instrument_type_name": "Interest Rate Swaption - Receiver"},
-            {"morningstar_instrument_type_code": "SA", "morningstar_instrument_type_name": "Asset Swap"},
-            {"morningstar_instrument_type_code": "SC", "morningstar_instrument_type_name": "Mutual Fund - CIT"},
-            {"morningstar_instrument_type_code": "SD", "morningstar_instrument_type_name": "Debt Swap"},
-            {"morningstar_instrument_type_code": "SE", "morningstar_instrument_type_name": "Equity Swap"},
-            {"morningstar_instrument_type_code": "SF", "morningstar_instrument_type_name": "Contract For Difference"},
-            {"morningstar_instrument_type_code": "SI", "morningstar_instrument_type_name": "Interest Rate Swap"},
-            {"morningstar_instrument_type_code": "SJ", "morningstar_instrument_type_name": "Interest Rate Future"},
-            {"morningstar_instrument_type_code": "SK", "morningstar_instrument_type_name": "Interest Rate Forward"},
-            {"morningstar_instrument_type_code": "SN", "morningstar_instrument_type_name": "Volatility/Variance Swap"},
-            {"morningstar_instrument_type_code": "SQ", "morningstar_instrument_type_name": "Equity Index Swap"},
-            {"morningstar_instrument_type_code": "SR", "morningstar_instrument_type_name": "Credit Default Swap"},
-            {"morningstar_instrument_type_code": "ST", "morningstar_instrument_type_name": "Total Return Swap"},
-            {"morningstar_instrument_type_code": "SU", "morningstar_instrument_type_name": "Structured Product"},
-            {"morningstar_instrument_type_code": "SV", "morningstar_instrument_type_name": "Cash - Stable Value Fund"},
-            {"morningstar_instrument_type_code": "SW", "morningstar_instrument_type_name": "Credit Default Index Swap (CDX)"},
-            {"morningstar_instrument_type_code": "SX", "morningstar_instrument_type_name": "Swaption - Payer"},
-            {"morningstar_instrument_type_code": "SY", "morningstar_instrument_type_name": "Swaption - Receiver"},
-            {"morningstar_instrument_type_code": "TF", "morningstar_instrument_type_name": "Bond - Treasury Future"},
-            {"morningstar_instrument_type_code": "TG", "morningstar_instrument_type_name": "Bond - U.S. Agency TBA"},
-            {"morningstar_instrument_type_code": "TP", "morningstar_instrument_type_name": "Bond - Gov't Inflation Protected"},
-            {"morningstar_instrument_type_code": "WR", "morningstar_instrument_type_name": "Undefined - Warrants/Rights"},
-            {"morningstar_instrument_type_code": "XP", "morningstar_instrument_type_name": "Credit Default Swaption - Payer"},
-            {"morningstar_instrument_type_code": "XR", "morningstar_instrument_type_name": "Credit Default Swaption - Receiver"},
-            {"morningstar_instrument_type_code": "YF", "morningstar_instrument_type_name": "Cryptocurrency - Future"},
-            {"morningstar_instrument_type_code": "YO", "morningstar_instrument_type_name": "Cryptocurrency"},
-        ]
-    )
-
-
-@_decorator.typechecked
-def get_lookthrough_holdings(portfolio_id: str) -> DataFrame:
-    """
-    :bdg-ref-danger:`Upcoming Feature <../upcoming_feature>`
-
-    Returns look-through holdings for a user-created portfolio.
-
-    Args:
-        portfolio_id (:obj:`str`): Portfolio ID. Use the `get_portfolios <./portfolio_list.html#morningstar_data.direct.user_items.get_portfolios>`_ function to discover saved portfolios.
-
-    Returns:
-        DataFrame: A DataFrame object with holdings data. DataFrame columns include
-
-        * investment_id
-        * isin
-        * cusip
-        * weight
-        * market_value
-        * security_name
-        * currency
-        * morningstar_instrument_type_code
-        * entity_id
-        * morningstar_entity_name
-        * primary_performance_id
-        * morningstar_instrument_type_name
-
-    :Examples:
-
-    Retrieve the look-through holdings for a portfolio.
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.get_lookthrough_holdings(portfolio_id='7b9cb5db-e3da-414e-8f75-b52b02222b5a') # Replace with a valid Portfolio ID
-        df
-
-    :Output:
-
-        =============  === ======================  ================================
-        investment_id  ... primary_performance_id  morningstar_instrument_type_name
-        =============  === ======================  ================================
-        E0USA00462         0P000000YM              Equity
-        F00000Q5HQ	       0P0000Z4DP              Equity
-        F00000UMZ1         0P00014J84              Equity
-        B10002POBD         None                    Bond - Asset Backed
-        =============  === ======================  ================================
-
-    Errors:
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-        TimeoutError: Raised when the fund of fund calculation takes too long.
-
-        ResourceNotFoundError: Raised when portfolio_id does not exist in Direct.
-
-        BadRequestException: Raised when portfolio_id is an invalid UUID.
-
-        UnavailableExternally: Raised when the function is not available for external Python package callers.
-    """
-
-    _logger.info("morningstar_data.direct.get_lookthrough_holdings")
-
-    # Get top level holdings in the portfolio
-    _logger.info("Fetching top level holdings")
-
-    # Split portfolio type from porfolio id
-    portfolio_id = portfolio_id.split(";")[0]
-    try:
-        uuid.UUID(portfolio_id)
-    except ValueError:
-        raise BadRequestException(BAD_REQUEST_ERROR_INVALID_PORTFOLIO_ID) from None
-
-    df_top_level_holdings = portfolio.get_holdings(portfolio_ids=[portfolio_id])
-
-    # Convert the weight to float, bcoz we think the FOF requires weight as float
-    df_top_level_holdings["Weight"] = df_top_level_holdings["Weight"].astype(float)
-
-    # Split secid and security type. They are bound together by ;
-    df_top_level_holdings[["SecId", "SecurityType"]] = df_top_level_holdings["HoldingId"].str.split(";", expand=True)
-
-    # We only are going to query FO and FE fund types. (open ended funds and ETFs)
-    # Maybe we need all fund types ???
-    fund_secids = df_top_level_holdings.loc[df_top_level_holdings["SecurityType"].isin(["FO", "FE"])]["SecId"].tolist()
-
-    investments = fund_secids
-
-    # Get investment data for each top level fund holding in the portfolio
-    # We are making this call to get  masterportfolio_id.
-    # If masterportfolio_id is added to lakehouse, this step can be removed
-
-    # only if a portfolio has funds of type FO or FE find the MasterPortfolio Id
-    if investments:
-        _logger.info("Fetching investment data for all top level holdings")
-        _logger.debug(f"{investments}")
-
-        data_points = [
-            {"datapointId": "DC09A", "datapointName": MASTER_PORTFOLIO_ID},
-            {"datapointId": "OS00I", "datapointName": "SecId"},
-        ]
-        df_mpid_mapping = inv.get_investment_data(investments, data_points)
-        df_top_level_holdings = df_top_level_holdings.merge(df_mpid_mapping[["SecId", MASTER_PORTFOLIO_ID]], on="SecId", how="left")
-
-    _logger.info("Fetching lookthrough holdings from FOF API.")
-    try:
-        df_lookthrough = _get_lookthrough_holdings_from_fof_api(portfolio_id, df_top_level_holdings)
-    except Exception as e:
-        _logger.error(e)
-        if type(e).__name__ == "InvalidQueryException":
-            raise BadRequestException(f"Sorry, something went wrong on our end: {str(e)} Please contact AL support") from None
-        else:
-            raise e from None
-
-    df_lookthrough = df_lookthrough.rename(
-        columns={
-            "securityName": "security_name",
-            "holdingDetailId": "investment_id",
-            "detailHoldingTypeId": "morningstar_instrument_type_code",
-            "currencyId": "currency",
-            "fractionalWeight": "weight",
-        }
-    )
-
-    _logger.info("Fetching enriched info with company information.")
-    df_enriched_data = _get_ids_from_lake_house(df_lookthrough)
-
-    # add morningstar_instrument_type_name as new column
-    df_enriched_data = df_enriched_data.merge(_morningstar_investment_type_id_name_mapping(), on="morningstar_instrument_type_code", how="left")
-
-    # If the user has AMS license, we return ISIN.
-    if _has_ams_license_for_isin() == False:
-        df_enriched_data = df_enriched_data.drop(["isin", "cusip"])
-
-    return df_enriched_data
+import simplejson as json
+import os
+import time
+import uuid
+import warnings
+from collections import defaultdict
+from datetime import datetime
+from typing import Any, Dict, List, Optional, Union
+from urllib.parse import quote
+from urllib.request import urlopen
+
+import pandas as pd
+from pandas import DataFrame
+
+
+from .. import datalake
+from .._base import _logger
+from . import _decorator, _utils
+from . import investment as inv
+from . import portfolio
+from ._base_api import APIBackend
+from ._config import _Config
+from ._config_key import FORMAT_DATE
+from ._error_messages import (
+    BAD_REQUEST_ERROR_INCLUDE_ALL_DATE,
+    BAD_REQUEST_ERROR_NO_START_DATE,
+    BAD_REQUEST_ERROR_INVALID_INVESTMENT_ID,
+    BAD_REQUEST_ERROR_NO_INVESTMENT_IDS,
+    BAD_REQUEST_ERROR_NO_PORTFOLIO_DATA,
+    BAD_REQUEST_ERROR_NO_START_DATE,
+    BAD_REQUEST_ERROR_INVALID_LOOKTHROUGH_HOLDING_TYPE,
+    BAD_REQUEST_ERROR_INVALID_PORTFOLIO_ID,
+)
+from ._exceptions import BadRequestException, NetworkExceptionError
+from ._backend_apis._holdings_backend import HoldingAPIBackend, FoFAPIBackend, AMSAPIBackend
+
+_config = _Config()
+
+_holding_api_request = HoldingAPIBackend()
+_fof_api_request = FoFAPIBackend()
+_ams_api_request = AMSAPIBackend()
+
+MASTER_PORTFOLIO_ID = "MasterPortfolio Id"
+
+
+@_decorator.typechecked
+def holdings(
+    investment_ids: List[str],
+    date: Optional[str] = None,
+    start_date: Optional[str] = None,
+    end_date: Optional[str] = None,
+) -> DataFrame:
+    warnings.warn(
+        "The holdings function is deprecated and will be removed in the next major version. Use get_holdings instead",
+        FutureWarning,
+        stacklevel=2,
+    )
+    return get_holdings(investment_ids, date, start_date, end_date)
+
+
+@_decorator.typechecked
+def get_holdings(
+    investment_ids: List[str],
+    date: Optional[str] = None,
+    start_date: Optional[str] = None,
+    end_date: Optional[str] = None,
+) -> DataFrame:
+    """Returns holdings for the specified investments and date or date range. If the date is not specified, the function uses the latest portfolio date by default.
+
+    Args:
+        investment_ids (:obj:`list`): A list of investment IDs. The investment ID format is SecId;Universe or just SecId.
+            For example: ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"].
+        date (:obj:`str`, `optional`): The portfolio date for which to retrieve data. The format is YYYY-MM-DD.
+            For example, "2020-01-01". If a date is provided, then the `start_date` and `end_date` parameters are ignored.
+            An exception is thrown if `start_date` or `end_date` is provided along with `date`.
+        start_date (:obj:`str`, `optional`): The start date for retrieving data. The format is
+            YYYY-MM-DD. For example, "2020-01-01". An exception is thrown if `date` is provided along with `start_date`.
+        end_date (:obj:`str`, `optional`): The end date for retrieving data. If no value is provided for
+            `end_date`, current date will be used. The format is YYYY-MM-DD. For example, "2020-01-01". An exception is
+            thrown if `date` is provided along with `end_date`.
+
+    Returns:
+        DataFrame: A DataFrame object with holdings data. DataFrame columns include:
+
+        * investmentId
+        * masterPortfolioId
+        * portfolioDate
+        * holdingId
+        * bondId
+        * name
+        * secId
+        * isin
+        * cusip
+        * weight
+        * shares
+        * marketValue
+        * sharesChanged
+        * currency
+        * ticker
+        * detailHoldingType
+
+    Raises:
+        ValueErrorException: Raised when the `investment_ids` parameter is invalid.
+
+    Examples:
+        Retrieve holdings for investment "FOUSA00KZH" on "2020-12-31".
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.get_holdings(investment_ids=["FOUSA00KZH"], date="2020-12-31")
+        df
+
+    :Output:
+        =============  =================  ===  ======  =================
+        investmentId   masterPortfolioId  ...  ticker  detailHoldingType
+        =============  =================  ===  ======  =================
+        FOUSA00KZH     6079               ...  CBRE    EQUITY
+        FOUSA00KZH     6079               ...  GOOGL   EQUITY
+        ...
+        =============  =================  ===  ======  =================
+
+    """
+    _validate_investment_ids(investment_ids)
+    _validate_date(date, start_date, end_date)
+
+    investment_date_info = _get_dates(investment_ids, date, start_date, end_date)
+    params = []
+    master_portfolio_id_investment_id_dict = defaultdict(list)
+    for sec_id, date_info in investment_date_info.items():
+        if date_info not in params:
+            params.append(date_info)
+        master_portfolio_id_investment_id_dict[date_info.get("masterPortfolioId", "")].append(sec_id)
+
+    url = f"{_config.securitydata_service_url()}v1/securities/holdings"
+    response_json = _holding_api_request.do_post_request(url, json.dumps(params, ignore_nan=True))
+    if not isinstance(response_json, list) or not response_json:
+        return DataFrame()
+    details = []
+    for holdings_info in response_json:
+        master_portfolio_id = holdings_info.get("masterPortfolioId", "")
+        holdings_date_info = holdings_info.get("holdings", dict())
+        for single_date, holdings in holdings_date_info.items():
+            for value in master_portfolio_id_investment_id_dict.get(master_portfolio_id, ""):
+                details.extend(
+                    [
+                        {
+                            "portfolioDate": single_date,
+                            "investmentId": value,
+                            "masterPortfolioId": master_portfolio_id,
+                            "holdingId": x.get("id", ""),
+                            "bondId": x.get("bondId", ""),
+                            "name": x.get("name", ""),
+                            "secId": x.get("secId", ""),
+                            "isin": x.get("isin", ""),
+                            "cusip": x.get("cusip", ""),
+                            "weight": x.get("weight", ""),
+                            "shares": x.get("shares", ""),
+                            "marketValue": x.get("marketValue", ""),
+                            "sharesChanged": x.get("sharesChanged", ""),
+                            "currency": x.get("currency", ""),
+                            "ticker": x.get("ticker", ""),
+                            "detailHoldingType": x.get("detailHoldingType", ""),
+                        }
+                        for x in holdings
+                    ]
+                )
+    return DataFrame(details)
+
+
+def _get_dates_by_investments(investment_ids: list) -> List[Any]:
+    ids = quote(",".join(investment_ids), "utf-8")
+    url = f"{_config.securitydata_service_url()}v2/securities/{ids}/portfolio-dates"
+    result: List[Any] = _holding_api_request.do_get_request(url)
+    return result
+
+
+@_decorator.typechecked
+def holding_dates(investment_ids: List[str]) -> DataFrame:
+    warnings.warn(
+        "The holding_dates function is deprecated and will be removed in the next major version. Use get_holding_dates instead",
+        FutureWarning,
+        stacklevel=2,
+    )
+    return get_holding_dates(investment_ids)
+
+
+@_decorator.typechecked
+def get_holding_dates(investment_ids: List[str]) -> DataFrame:
+    """Returns all dates with available holdings data for the given investment.
+
+    Args:
+        investment_ids (:obj:`list`): A list of investment IDs. The investment ID format is SecId;Universe or just SecId.
+            For example: ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"].
+
+    Returns:
+        DataFrame: A DataFrame object with portfolio date data. DataFrame columns include:
+
+       * secId
+       * masterPortfolioId
+       * date
+       * suppression
+       * suppressionHoldingNumber
+
+    Examples:
+        Retrieve portfolio dates for investment "FOUSA00KZH".
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.get_holding_dates(investment_ids=["FOUSA06JNH"])
+        df
+
+    :Output:
+        ==========  =================  ==========  ===========  ========================
+        secId       masterPortfolioId  date        suppression  suppressionHoldingNumber
+        ==========  =================  ==========  ===========  ========================
+        FOUSA06JNH  210311             2021-08-31  False        None
+        FOUSA06JNH  210311             2021-07-31  False        None
+        ...
+        ==========  =================  ==========  ===========  ========================
+
+    """
+    if not investment_ids:
+        raise BadRequestException(BAD_REQUEST_ERROR_NO_INVESTMENT_IDS) from None
+    response_json = _get_dates_by_investments(investment_ids)
+    if isinstance(response_json, list) and response_json:
+        details = []
+        for date_info in response_json:
+            sec_id = date_info.get("secId", "")
+            master_portfolio_id = date_info.get("masterPortfolioId", "")
+            details.extend(
+                [
+                    {
+                        "secId": sec_id,
+                        "masterPortfolioId": master_portfolio_id,
+                        "date": portfolio_date.get("date", ""),
+                        "suppression": portfolio_date.get("suppression", False),
+                        "suppressionHoldingNumber": portfolio_date.get("suppressionHoldingNumber", None),
+                    }
+                    for portfolio_date in date_info.get("portfolioDates", [])
+                ]
+            )
+        return DataFrame(details)
+    else:
+        return DataFrame()
+
+
+def _get_dates(
+    investment_ids: list,
+    date: Optional[str] = None,
+    start_date: Optional[str] = None,
+    end_date: Optional[str] = None,
+) -> dict:
+    dates_raw: Dict[str, Optional[str]] = {
+        "date": date,
+        "start_date": start_date,
+        "end_date": end_date,
+    }
+    dates: Dict[str, str] = {}
+
+    for key, value in dates_raw.items():
+        if value is not None and len(value.strip()) > 0:
+            dates[key] = _utils._format_date(value)
+        elif key == "end_date" and dates_raw["start_date"] is not None:
+            dates[key] = _utils._format_date(time.strftime(FORMAT_DATE, time.localtime()))
+
+    response_json = _get_dates_by_investments(investment_ids)
+    if not isinstance(response_json, list) or not response_json:
+        raise BadRequestException(BAD_REQUEST_ERROR_NO_PORTFOLIO_DATA) from None
+
+    if not bool(dates):
+        return _handle_no_date(response_json)
+    elif "date" in dates:
+        return _handle_single_date(response_json, **dates)
+
+    return _handle_date_range(response_json, **dates)
+
+
+def _validate_date(date: Optional[str], start_date: Optional[str], end_date: Optional[str]) -> None:
+    if date:
+        if start_date or end_date:
+            raise BadRequestException(BAD_REQUEST_ERROR_INCLUDE_ALL_DATE) from None
+    else:
+        if not start_date and end_date:
+            raise BadRequestException(BAD_REQUEST_ERROR_NO_START_DATE) from None
+
+
+def _handle_single_date(date_info_list: list, date: str) -> dict:
+    investment_date_info = dict()
+    for date_info in date_info_list:
+        available_date = _get_available_date(date, date_info)
+        if available_date is not None:
+            master_portfolio_id = date_info.get("masterPortfolioId", "")
+            investment_date_info[date_info.get("secId", "")] = {
+                "masterPortfolioId": master_portfolio_id,
+                "portfolioDates": [available_date],
+            }
+    return investment_date_info
+
+
+def _get_available_date(date: str, date_info: dict = dict()) -> Optional[str]:
+    date_objs = date_info.get("portfolioDates", [])
+    available_date = None
+    for date_obj in date_objs:
+        if date_obj.get("date", "") == date:
+            available_date = date
+            break
+        elif date_obj.get("date", "") < date and available_date is None:
+            available_date = date_obj.get("date", "")
+    return available_date
+
+
+def _handle_no_date(date_info_list: list) -> dict:
+    investment_date_info = dict()
+    for date_info in date_info_list:
+        portfolio_dates = date_info.get("portfolioDates", [])
+        if portfolio_dates:
+            date = next(
+                (x.get("date", "") for x in portfolio_dates if x.get("date", "") is not None and len(x.get("date", "")) > 0),
+                None,
+            )
+            if date is not None and len(date) > 0:
+                master_portfolio_id = date_info.get("masterPortfolioId", "")
+                investment_date_info[date_info.get("secId", "")] = {
+                    "masterPortfolioId": master_portfolio_id,
+                    "portfolioDates": [date],
+                }
+    return investment_date_info
+
+
+def _handle_date_range(date_info_list: list, start_date: str, end_date: str) -> dict:
+    investment_date_info = dict()
+    for date_info in date_info_list:
+        sec_id = date_info.get("secId", "")
+        master_portfolio_id = date_info.get("masterPortfolioId", "")
+        portfolio_dates = date_info.get("portfolioDates", [])
+        date_list = []
+        for portfolio_date in portfolio_dates:
+            single_date = portfolio_date.get("date", "")
+            if start_date <= single_date <= end_date:
+                date_list.append(single_date)
+        if date_list:
+            investment_date_info[sec_id] = {
+                "masterPortfolioId": master_portfolio_id,
+                "portfolioDates": date_list,
+            }
+    return investment_date_info
+
+
+def _validate_investment_ids(investment_ids: List[str]) -> None:
+    if not investment_ids:
+        raise BadRequestException(BAD_REQUEST_ERROR_NO_INVESTMENT_IDS) from None
+    elif [x for x in investment_ids if len(x.split(";")[0]) != 10]:
+        raise BadRequestException(BAD_REQUEST_ERROR_INVALID_INVESTMENT_ID) from None
+
+
+def _get_ids_from_lake_house(df_lookthrough: pd.DataFrame) -> pd.DataFrame:
+    sql = """SELECT distinct
+            a.investment_id
+            ,a.isin
+            ,a.cusip
+            ,a.weight
+            ,a.marketValue as market_value
+            ,a.security_name
+            ,a.currency
+            ,a.morningstar_instrument_type_code
+            ,b.entity_id
+            ,b.morningstar_entity_name
+            ,b.performance_id as primary_performance_id
+            FROM lookthrough_temp a
+                left join platform__reference__prd.investment_lookup b
+                    on a.investment_id=b.investment_id and b.is_primary = True
+            where (b.is_primary = True or b.investment_id is null)
+    """
+    df = datalake.query(sql, temp_tables=[datalake.TempTable("lookthrough_temp", df_lookthrough)])
+    return df
+
+
+def _get_fof_secid_and_investment_types(df_top_level_holdings: pd.DataFrame) -> pd.DataFrame:
+    # create DataFrame with Direct secId and Direct securityType
+    # df_top_level_holdings_expanded = df_top_level_holdings["HoldingId"].str.split(";", expand=True).rename(columns={0: "secid", 1: "sectype"})
+    df_top_level_holdings[["fof_secid", "fof_sectype"]] = df_top_level_holdings["HoldingId"].str.split(";", expand=True).rename(columns={0: "fof_secid", 1: "fof_sectype"})
+    if MASTER_PORTFOLIO_ID in df_top_level_holdings.columns:
+        df_top_level_holdings["masterPortfolioId"] = df_top_level_holdings[MASTER_PORTFOLIO_ID].astype("Int64")
+
+    query_str = """with cte as (
+        SELECT distinct --performance_id,
+        case
+            when left(investment_id,2) ='E0' and fund_id is null
+                then performance_id
+            when is_primary=False
+                then performance_id
+            else investment_id
+        end as sec_id
+        ,investment_id
+        ,morningstar_investment_name
+        ,case
+            when morningstar_instrument_type_code is not null
+                then morningstar_instrument_type_code
+            when left(investment_id,2) in ('FE','FC','FO','FH','FM','FV','SC')
+                then left(investment_id,2)
+            when left(investment_id,2) = 'F0'
+                then 'FO'
+            when left(investment_id,2) ='SA'
+                then 'FS'
+            when left(investment_id,2) ='E0' and fund_id is null
+                then 'E'
+            when left(investment_id,2) ='E0' and fund_id is not null
+                then 'FC'
+            else null
+        end as morningstar_instrument_type_code
+        ,is_primary
+        FROM platform__reference__prd.investment_lookup a
+        where
+        (
+            performance_id is not null
+            or
+            morningstar_instrument_type_code in ('BC','12','BZ','BY','B','BT','NE','BH','IP','NE','NB','NC','BG','BD','ND')
+        )
+        and
+            left(investment_id,2) not in ('XI','VA')
+        and
+        (
+            a.performance_id in (select fof_secid from temp_top_level_holdings_expanded)
+            or
+            a.investment_id in (select fof_secid from temp_top_level_holdings_expanded)
+        )
+    )
+    select
+        a.weight as weighting,
+        a.Name as securityName,
+        b.investment_id as secId,
+        coalesce(trim(b.morningstar_instrument_type_code), 'Q') as detailHoldingTypeId
+    from
+        temp_top_level_holdings_expanded a
+        left join cte b
+            on a.fof_secid=b.sec_id
+    """
+
+    return datalake.query(
+        query_str=query_str,
+        temp_tables=[
+            datalake.TempTable(name="temp_top_level_holdings_expanded", df=df_top_level_holdings),
+        ],
+    )
+
+
+def _get_lookthrough_holdings_from_fof_api(portfolio_id: str, df_top_level_holdings: DataFrame) -> DataFrame:
+
+    from ._backend_apis._signed_url_backend import SignedUrlBackend
+
+    _signed_url_request = SignedUrlBackend()
+
+    # 'XI' represents an index, which is unsupported by FoF API
+    if "XI" in df_top_level_holdings["SecurityType"].values:
+        raise BadRequestException(BAD_REQUEST_ERROR_INVALID_LOOKTHROUGH_HOLDING_TYPE)
+
+    _logger.info(
+        "Fetching FOF comptabile secid and investment types from investments_lookup table in lakehouse along with required fields from top level holdings to pass to FOF API."
+    )
+    df_fof_sec_id_investment_types = _get_fof_secid_and_investment_types(df_top_level_holdings)
+
+    _logger.info("Generating a unique id for each row in the top level holdings.")
+    # Add a UUID as value for clientSecurityGuid for each holding
+
+    df_fof_sec_id_investment_types = df_fof_sec_id_investment_types.rename(
+        columns={
+            "secid": "secId",
+            "weighting": "weighting",
+            "detailholdingtypeid": "detailHoldingTypeId",
+            "securityname": "securityName",
+        }
+    )
+
+    df_fof_sec_id_investment_types["clientSecurityGuid"] = [str(uuid.uuid4()) for _ in range(len(df_fof_sec_id_investment_types.index))]
+
+    _logger.info("Extracting fof_secid, investment_type, weight and masterportfolio id into json to pass to FOF API")
+    holdings_json = df_fof_sec_id_investment_types.to_json(orient="records")
+
+    holdings_parsed = json.loads(holdings_json)  # This is sent to FOF API in the holdings field
+
+    fof_post_url = f"{_config.fof_api_url()}portfolios/drilldown/{portfolio_id.split(';')[0]}/ALCustomerHoldings"
+    payload = json.dumps(
+        {
+            "clientPortfolioGuid": str(uuid.uuid4()),
+            "portfolioDate": str(datetime.now().strftime("%Y%m%d")),
+            "currencyId": "USD",
+            "holdings": holdings_parsed,  # The SQL query returns the columns in exactly the same format as required by FOF API
+        }
+    )
+
+    _logger.info("Submitting request to FOF API to run lookthrough holdings.")
+    _logger.debug(f"Sending request to {fof_post_url}")
+
+    # MD proxy api will poll FOF API and return the signed url to download the lookthrough holdings
+    signed_url = _fof_api_request.do_post_request(fof_post_url, payload)["jobId"]  # Returns reponse.content as string
+
+    _logger.info("Submitting request to download lookthrough holdsings from signed url.")
+    _logger.debug(f"Sending request to {signed_url}")
+    look_through_holdings_reponse = _signed_url_request.do_get_request(signed_url)  # The reponse includes lookthrough holdings as json
+
+    _logger.info("Got response from Signed url request")
+    look_through_holdings_json = json.loads(look_through_holdings_reponse)
+    holdings = look_through_holdings_json["holdings"]
+    _logger.debug(f"Got {len(holdings)} lookthrough holdings.")
+
+    df_look_through_holdings = pd.DataFrame(holdings)
+    return df_look_through_holdings
+
+
+def _has_ams_license_for_isin() -> bool:
+    ams_get_url = f"{_config.al_proxy_api_url()}/v2/ams/api/user/entitlements"
+    response = _ams_api_request.do_get_request(ams_get_url)
+
+    data_groups = response["DataGroups"]
+    for data_group in data_groups:
+        if ((data_group["IdType"] == "UNIVERSEID" and data_group["DataGroupId"] == "ALL") or data_group["DataGroupId"] == "CUSIP") and data_group["Permission"] == 1:
+            return True
+    return False
+
+
+# temporary function until this data is added to Lake House
+def _morningstar_investment_type_id_name_mapping() -> pd.DataFrame:
+    return pd.DataFrame(
+        [
+            {"morningstar_instrument_type_code": "0", "morningstar_instrument_type_name": "Muni Bond - Unspecified"},
+            {"morningstar_instrument_type_code": "1", "morningstar_instrument_type_name": "Muni Bond - General Obligation"},
+            {"morningstar_instrument_type_code": "12", "morningstar_instrument_type_name": "Muni Bond - Revenue"},
+            {
+                "morningstar_instrument_type_code": "13",
+                "morningstar_instrument_type_name": "Muni Bond - Cash (Retired after Oct 2022)",
+            },
+            {"morningstar_instrument_type_code": "14", "morningstar_instrument_type_name": "Muni Bond - Double Barrelled"},
+            {"morningstar_instrument_type_code": "AF", "morningstar_instrument_type_name": "Alternatives - Farm & Timber Land"},
+            {"morningstar_instrument_type_code": "AI", "morningstar_instrument_type_name": "Alternatives - Infrastructure"},
+            {
+                "morningstar_instrument_type_code": "AM",
+                "morningstar_instrument_type_name": "Alternatives - Master Investment Trust",
+            },
+            {"morningstar_instrument_type_code": "AP", "morningstar_instrument_type_name": "Alternatives - Private Equity"},
+            {"morningstar_instrument_type_code": "AR", "morningstar_instrument_type_name": "Alternatives - Real Estate"},
+            {"morningstar_instrument_type_code": "B", "morningstar_instrument_type_name": "Bond - Corporate Bond"},
+            {"morningstar_instrument_type_code": "BB", "morningstar_instrument_type_name": "Bond - Short-term Corporate Bills"},
+            {"morningstar_instrument_type_code": "BC", "morningstar_instrument_type_name": "Bond - Convertible"},
+            {"morningstar_instrument_type_code": "BD", "morningstar_instrument_type_name": "Bond - Gov't Agency Debt"},
+            {"morningstar_instrument_type_code": "BG", "morningstar_instrument_type_name": "Bond - Gov't Agency Pass-Thru"},
+            {"morningstar_instrument_type_code": "BH", "morningstar_instrument_type_name": "Bond - Non-Agency Residential MBS"},
+            {"morningstar_instrument_type_code": "BL", "morningstar_instrument_type_name": "Bond Index - Future"},
+            {"morningstar_instrument_type_code": "BM", "morningstar_instrument_type_name": "Bond - Non-U.S. Gov't Agency MBS"},
+            {
+                "morningstar_instrument_type_code": "BO",
+                "morningstar_instrument_type_name": "Bond Index - Option (Call) (Consolidation to FD after Oct 2022)",
+            },
+            {
+                "morningstar_instrument_type_code": "BP",
+                "morningstar_instrument_type_name": "Bond Index - Option (Put) (Consolidation to FD after Oct 2022)",
+            },
+            {"morningstar_instrument_type_code": "BQ", "morningstar_instrument_type_name": "Bond - Undefined"},
+            {"morningstar_instrument_type_code": "BR", "morningstar_instrument_type_name": "Bond - Bank Loans"},
+            {"morningstar_instrument_type_code": "BT", "morningstar_instrument_type_name": "Bond - Gov't/Treasury"},
+            {"morningstar_instrument_type_code": "BU", "morningstar_instrument_type_name": "Bond - Units"},
+            {"morningstar_instrument_type_code": "BW", "morningstar_instrument_type_name": "Bond - Warrants/Rights (Call)"},
+            {"morningstar_instrument_type_code": "BX", "morningstar_instrument_type_name": "Bond - Warrants/Rights (Put)"},
+            {"morningstar_instrument_type_code": "BY", "morningstar_instrument_type_name": "Bond - Asset Backed"},
+            {"morningstar_instrument_type_code": "BZ", "morningstar_instrument_type_name": "Bond - Supranational"},
+            {"morningstar_instrument_type_code": "C", "morningstar_instrument_type_name": "Cash"},
+            {"morningstar_instrument_type_code": "CA", "morningstar_instrument_type_name": "Cash - Collateral"},
+            {
+                "morningstar_instrument_type_code": "CC",
+                "morningstar_instrument_type_name": "Cash - Option (Call) (Consolidation to CY after Oct 2022)",
+            },
+            {"morningstar_instrument_type_code": "CD", "morningstar_instrument_type_name": "Cash - CD/Time Deposit"},
+            {"morningstar_instrument_type_code": "CH", "morningstar_instrument_type_name": "Cash - Currency"},
+            {"morningstar_instrument_type_code": "CL", "morningstar_instrument_type_name": "Currency - Future"},
+            {"morningstar_instrument_type_code": "CN", "morningstar_instrument_type_name": "Bond - Contingent Convertible"},
+            {
+                "morningstar_instrument_type_code": "CO",
+                "morningstar_instrument_type_name": "Cash - Option (Put) (Consolidation to CZ after Oct 2022)",
+            },
+            {"morningstar_instrument_type_code": "CP", "morningstar_instrument_type_name": "Cash - Commercial Paper"},
+            {"morningstar_instrument_type_code": "CQ", "morningstar_instrument_type_name": "Cash - Future Offset"},
+            {"morningstar_instrument_type_code": "CR", "morningstar_instrument_type_name": "Cash - Repurchase Agreement"},
+            {"morningstar_instrument_type_code": "CS", "morningstar_instrument_type_name": "Currency - Swap"},
+            {"morningstar_instrument_type_code": "CT", "morningstar_instrument_type_name": "Bond - Capital Contingent Debt"},
+            {"morningstar_instrument_type_code": "CU", "morningstar_instrument_type_name": "Currency - Forward"},
+            {
+                "morningstar_instrument_type_code": "CV",
+                "morningstar_instrument_type_name": "Currency - Warrants\\Rights (Call) (Consolidation to CY after Oct 2022)",
+            },
+            {
+                "morningstar_instrument_type_code": "CX",
+                "morningstar_instrument_type_name": "Currency - Warrants\\Rights (Put) (Consolidation to CZ after Oct 2022)",
+            },
+            {"morningstar_instrument_type_code": "CY", "morningstar_instrument_type_name": "Currency Option (Call)"},
+            {"morningstar_instrument_type_code": "CZ", "morningstar_instrument_type_name": "Currency Option (Put)"},
+            {"morningstar_instrument_type_code": "DA", "morningstar_instrument_type_name": "Bond - Future"},
+            {"morningstar_instrument_type_code": "DB", "morningstar_instrument_type_name": "Bond - Option (Call)"},
+            {"morningstar_instrument_type_code": "DC", "morningstar_instrument_type_name": "Commodity - Option (Call)"},
+            {"morningstar_instrument_type_code": "DD", "morningstar_instrument_type_name": "Commodity"},
+            {"morningstar_instrument_type_code": "DE", "morningstar_instrument_type_name": "Bond - Option (Put)"},
+            {"morningstar_instrument_type_code": "DG", "morningstar_instrument_type_name": "Equity - Future"},
+            {"morningstar_instrument_type_code": "DH", "morningstar_instrument_type_name": "Equity - Option (Call)"},
+            {"morningstar_instrument_type_code": "DI", "morningstar_instrument_type_name": "Equity - Option (Put)"},
+            {"morningstar_instrument_type_code": "DJ", "morningstar_instrument_type_name": "Other - Future"},
+            {"morningstar_instrument_type_code": "DM", "morningstar_instrument_type_name": "Commodity - Future"},
+            {
+                "morningstar_instrument_type_code": "DO",
+                "morningstar_instrument_type_name": "Bond - Collateralized Debt Obligations (CDO/CBO)",
+            },
+            {"morningstar_instrument_type_code": "DP", "morningstar_instrument_type_name": "Commodity - Option (Put)"},
+            {
+                "morningstar_instrument_type_code": "DS",
+                "morningstar_instrument_type_name": "Bond - Sub-sovereign Government Debt",
+            },
+            {"morningstar_instrument_type_code": "E", "morningstar_instrument_type_name": "Equity"},
+            {"morningstar_instrument_type_code": "EC", "morningstar_instrument_type_name": "Equity Index - Option (Call)"},
+            {"morningstar_instrument_type_code": "EL", "morningstar_instrument_type_name": "Equity Index - Future"},
+            {"morningstar_instrument_type_code": "EP", "morningstar_instrument_type_name": "Equity Index - Option (Put)"},
+            {"morningstar_instrument_type_code": "EQ", "morningstar_instrument_type_name": "Equity - Undefined"},
+            {"morningstar_instrument_type_code": "ER", "morningstar_instrument_type_name": "Equity - REIT"},
+            {"morningstar_instrument_type_code": "EU", "morningstar_instrument_type_name": "Equity - Units"},
+            {"morningstar_instrument_type_code": "EV", "morningstar_instrument_type_name": "Equity - Warrants/Rights (Put)"},
+            {"morningstar_instrument_type_code": "EW", "morningstar_instrument_type_name": "Equity - Warrants/Rights (Call)"},
+            {"morningstar_instrument_type_code": "EX", "morningstar_instrument_type_name": "Mutual Fund - Unspecified"},
+            {"morningstar_instrument_type_code": "FC", "morningstar_instrument_type_name": "Mutual Fund - Closed End"},
+            {"morningstar_instrument_type_code": "FD", "morningstar_instrument_type_name": "Other Fixed Income Derivative"},
+            {"morningstar_instrument_type_code": "FE", "morningstar_instrument_type_name": "Mutual Fund - ETF"},
+            {"morningstar_instrument_type_code": "FH", "morningstar_instrument_type_name": "Mutual Fund - Hedge Fund"},
+            {"morningstar_instrument_type_code": "FM", "morningstar_instrument_type_name": "Mutual Fund - Money Market"},
+            {"morningstar_instrument_type_code": "FO", "morningstar_instrument_type_name": "Mutual Fund - Open End"},
+            {"morningstar_instrument_type_code": "FS", "morningstar_instrument_type_name": "Mutual Fund - Separate Account"},
+            {"morningstar_instrument_type_code": "FV", "morningstar_instrument_type_name": "Mutual Fund - Variable Annuity"},
+            {"morningstar_instrument_type_code": "FZ", "morningstar_instrument_type_name": "Mutual Fund - Client Portfolio"},
+            {"morningstar_instrument_type_code": "GA", "morningstar_instrument_type_name": "Bond - Non-US Gov't Agency CMO"},
+            {"morningstar_instrument_type_code": "GC", "morningstar_instrument_type_name": "Bond - Global Non-Agency CMO"},
+            {"morningstar_instrument_type_code": "GM", "morningstar_instrument_type_name": "Bond - Global Non-Agency MBS"},
+            {"morningstar_instrument_type_code": "GS", "morningstar_instrument_type_name": "Bond - Short-term Government Bills"},
+            {"morningstar_instrument_type_code": "IP", "morningstar_instrument_type_name": "Bond - Corp Inflation Protected"},
+            {"morningstar_instrument_type_code": "IS", "morningstar_instrument_type_name": "Inflation Swap"},
+            {"morningstar_instrument_type_code": "IT", "morningstar_instrument_type_name": "Income Trust"},
+            {
+                "morningstar_instrument_type_code": "LO",
+                "morningstar_instrument_type_name": "Bond - Collateralized Loan Obligations (CLO)",
+            },
+            {"morningstar_instrument_type_code": "NB", "morningstar_instrument_type_name": "Bond - Commercial MBS"},
+            {"morningstar_instrument_type_code": "NC", "morningstar_instrument_type_name": "Bond - Gov't Agency CMO"},
+            {"morningstar_instrument_type_code": "ND", "morningstar_instrument_type_name": "Bond - Covered Bond"},
+            {"morningstar_instrument_type_code": "NE", "morningstar_instrument_type_name": "Bond - Gov't Agency ARM"},
+            {"morningstar_instrument_type_code": "NR", "morningstar_instrument_type_name": "Bond - U.S. Agency Credit Risk CMO"},
+            {"morningstar_instrument_type_code": "OO", "morningstar_instrument_type_name": "Cash - Option Offset"},
+            {"morningstar_instrument_type_code": "OS", "morningstar_instrument_type_name": "Cash - Swap Offset"},
+            {"morningstar_instrument_type_code": "OT", "morningstar_instrument_type_name": "Cash - Forward Offset"},
+            {"morningstar_instrument_type_code": "P", "morningstar_instrument_type_name": "Preferred Stock"},
+            {"morningstar_instrument_type_code": "PA", "morningstar_instrument_type_name": "Participating Preferred"},
+            {"morningstar_instrument_type_code": "PC", "morningstar_instrument_type_name": "Convertible Preferred"},
+            {"morningstar_instrument_type_code": "PP", "morningstar_instrument_type_name": "Property"},
+            {"morningstar_instrument_type_code": "PS", "morningstar_instrument_type_name": "Interest Rate Swaption - Payer"},
+            {"morningstar_instrument_type_code": "Q", "morningstar_instrument_type_name": "Unidentified Holding"},
+            {"morningstar_instrument_type_code": "QQ", "morningstar_instrument_type_name": "Other Assets And Liabilities"},
+            {"morningstar_instrument_type_code": "RS", "morningstar_instrument_type_name": "Interest Rate Swaption - Receiver"},
+            {"morningstar_instrument_type_code": "SA", "morningstar_instrument_type_name": "Asset Swap"},
+            {"morningstar_instrument_type_code": "SC", "morningstar_instrument_type_name": "Mutual Fund - CIT"},
+            {"morningstar_instrument_type_code": "SD", "morningstar_instrument_type_name": "Debt Swap"},
+            {"morningstar_instrument_type_code": "SE", "morningstar_instrument_type_name": "Equity Swap"},
+            {"morningstar_instrument_type_code": "SF", "morningstar_instrument_type_name": "Contract For Difference"},
+            {"morningstar_instrument_type_code": "SI", "morningstar_instrument_type_name": "Interest Rate Swap"},
+            {"morningstar_instrument_type_code": "SJ", "morningstar_instrument_type_name": "Interest Rate Future"},
+            {"morningstar_instrument_type_code": "SK", "morningstar_instrument_type_name": "Interest Rate Forward"},
+            {"morningstar_instrument_type_code": "SN", "morningstar_instrument_type_name": "Volatility/Variance Swap"},
+            {"morningstar_instrument_type_code": "SQ", "morningstar_instrument_type_name": "Equity Index Swap"},
+            {"morningstar_instrument_type_code": "SR", "morningstar_instrument_type_name": "Credit Default Swap"},
+            {"morningstar_instrument_type_code": "ST", "morningstar_instrument_type_name": "Total Return Swap"},
+            {"morningstar_instrument_type_code": "SU", "morningstar_instrument_type_name": "Structured Product"},
+            {"morningstar_instrument_type_code": "SV", "morningstar_instrument_type_name": "Cash - Stable Value Fund"},
+            {"morningstar_instrument_type_code": "SW", "morningstar_instrument_type_name": "Credit Default Index Swap (CDX)"},
+            {"morningstar_instrument_type_code": "SX", "morningstar_instrument_type_name": "Swaption - Payer"},
+            {"morningstar_instrument_type_code": "SY", "morningstar_instrument_type_name": "Swaption - Receiver"},
+            {"morningstar_instrument_type_code": "TF", "morningstar_instrument_type_name": "Bond - Treasury Future"},
+            {"morningstar_instrument_type_code": "TG", "morningstar_instrument_type_name": "Bond - U.S. Agency TBA"},
+            {"morningstar_instrument_type_code": "TP", "morningstar_instrument_type_name": "Bond - Gov't Inflation Protected"},
+            {"morningstar_instrument_type_code": "WR", "morningstar_instrument_type_name": "Undefined - Warrants/Rights"},
+            {"morningstar_instrument_type_code": "XP", "morningstar_instrument_type_name": "Credit Default Swaption - Payer"},
+            {"morningstar_instrument_type_code": "XR", "morningstar_instrument_type_name": "Credit Default Swaption - Receiver"},
+            {"morningstar_instrument_type_code": "YF", "morningstar_instrument_type_name": "Cryptocurrency - Future"},
+            {"morningstar_instrument_type_code": "YO", "morningstar_instrument_type_name": "Cryptocurrency"},
+        ]
+    )
+
+
+@_decorator.typechecked
+def get_lookthrough_holdings(portfolio_id: str) -> DataFrame:
+    """
+    :bdg-ref-danger:`Upcoming Feature <../upcoming_feature>`
+
+    Returns look-through holdings for a user-created portfolio.
+
+    Args:
+        portfolio_id (:obj:`str`): Portfolio ID. Use the `get_portfolios <./portfolio_list.html#morningstar_data.direct.user_items.get_portfolios>`_ function to discover saved portfolios.
+
+    Returns:
+        DataFrame: A DataFrame object with holdings data. DataFrame columns include
+
+        * investment_id
+        * isin
+        * cusip
+        * weight
+        * market_value
+        * security_name
+        * currency
+        * morningstar_instrument_type_code
+        * entity_id
+        * morningstar_entity_name
+        * primary_performance_id
+        * morningstar_instrument_type_name
+
+    :Examples:
+
+    Retrieve the look-through holdings for a portfolio.
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.get_lookthrough_holdings(portfolio_id='7b9cb5db-e3da-414e-8f75-b52b02222b5a') # Replace with a valid Portfolio ID
+        df
+
+    :Output:
+
+        =============  === ======================  ================================
+        investment_id  ... primary_performance_id  morningstar_instrument_type_name
+        =============  === ======================  ================================
+        E0USA00462         0P000000YM              Equity
+        F00000Q5HQ	       0P0000Z4DP              Equity
+        F00000UMZ1         0P00014J84              Equity
+        B10002POBD         None                    Bond - Asset Backed
+        =============  === ======================  ================================
+
+    Errors:
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+        TimeoutError: Raised when the fund of fund calculation takes too long.
+
+        ResourceNotFoundError: Raised when portfolio_id does not exist in Direct.
+
+        BadRequestException: Raised when portfolio_id is an invalid UUID.
+
+        UnavailableExternally: Raised when the function is not available for external Python package callers.
+    """
+
+    _logger.info("morningstar_data.direct.get_lookthrough_holdings")
+
+    # Get top level holdings in the portfolio
+    _logger.info("Fetching top level holdings")
+
+    # Split portfolio type from porfolio id
+    portfolio_id = portfolio_id.split(";")[0]
+    try:
+        uuid.UUID(portfolio_id)
+    except ValueError:
+        raise BadRequestException(BAD_REQUEST_ERROR_INVALID_PORTFOLIO_ID) from None
+
+    df_top_level_holdings = portfolio.get_holdings(portfolio_ids=[portfolio_id])
+
+    # Convert the weight to float, bcoz we think the FOF requires weight as float
+    df_top_level_holdings["Weight"] = df_top_level_holdings["Weight"].astype(float)
+
+    # Split secid and security type. They are bound together by ;
+    df_top_level_holdings[["SecId", "SecurityType"]] = df_top_level_holdings["HoldingId"].str.split(";", expand=True)
+
+    # We only are going to query FO and FE fund types. (open ended funds and ETFs)
+    # Maybe we need all fund types ???
+    fund_secids = df_top_level_holdings.loc[df_top_level_holdings["SecurityType"].isin(["FO", "FE"])]["SecId"].tolist()
+
+    investments = fund_secids
+
+    # Get investment data for each top level fund holding in the portfolio
+    # We are making this call to get  masterportfolio_id.
+    # If masterportfolio_id is added to lakehouse, this step can be removed
+
+    # only if a portfolio has funds of type FO or FE find the MasterPortfolio Id
+    if investments:
+        _logger.info("Fetching investment data for all top level holdings")
+        _logger.debug(f"{investments}")
+
+        data_points = [
+            {"datapointId": "DC09A", "datapointName": MASTER_PORTFOLIO_ID},
+            {"datapointId": "OS00I", "datapointName": "SecId"},
+        ]
+        df_mpid_mapping = inv.get_investment_data(investments, data_points)
+        df_top_level_holdings = df_top_level_holdings.merge(df_mpid_mapping[["SecId", MASTER_PORTFOLIO_ID]], on="SecId", how="left")
+
+    _logger.info("Fetching lookthrough holdings from FOF API.")
+    try:
+        df_lookthrough = _get_lookthrough_holdings_from_fof_api(portfolio_id, df_top_level_holdings)
+    except Exception as e:
+        _logger.error(e)
+        if type(e).__name__ == "InvalidQueryException":
+            raise BadRequestException(f"Sorry, something went wrong on our end: {str(e)} Please contact AL support") from None
+        else:
+            raise e from None
+
+    df_lookthrough = df_lookthrough.rename(
+        columns={
+            "securityName": "security_name",
+            "holdingDetailId": "investment_id",
+            "detailHoldingTypeId": "morningstar_instrument_type_code",
+            "currencyId": "currency",
+            "fractionalWeight": "weight",
+        }
+    )
+
+    _logger.info("Fetching enriched info with company information.")
+    df_enriched_data = _get_ids_from_lake_house(df_lookthrough)
+
+    # add morningstar_instrument_type_name as new column
+    df_enriched_data = df_enriched_data.merge(_morningstar_investment_type_id_name_mapping(), on="morningstar_instrument_type_code", how="left")
+
+    # If the user has AMS license, we return ISIN.
+    if _has_ams_license_for_isin() == False:
+        df_enriched_data = df_enriched_data.drop(["isin", "cusip"])
+
+    return df_enriched_data
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/investment.py` & `morningstar_data-1.3.0/morningstar_data/direct/investment.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,250 +1,250 @@
-from operator import inv
-import warnings
-from pandas import DataFrame
-from typing import Optional, List, Dict, Any, Union
-
-from . import _decorator
-from .._base import _logger
-from ._data_objects import Investments, InvestmentType, DataPoints, DataPointsType
-
-from ._investment._asset_flow_data import AssetFlowProvider
-from ._investment._normal_data import NormalDataProvider
-from ._investment._common import _get_data_points, _get_data_point_col_names
-
-
-@_decorator.typechecked
-def investment_data(
-    investments: Union[List[str], str, Dict[str, Any]],
-    datapoints: Union[List[Dict[str, Any]], str, DataFrame],
-) -> DataFrame:
-    warnings.warn(
-        "The investment_data function is deprecated and will be removed in the next major version. Use get_investment_data instead",
-        FutureWarning,
-        stacklevel=2,
-    )
-    return _get_investment_data(investments, datapoints)
-
-
-# FIXME: In https://msjira.morningstar.com/browse/AL2-92, the error_handler decorator was removed from some methods
-# to trigger QueryLimitException.
-# There are multiple methods where the decorator was removed to trigger certain exceptions back to the caller:
-#   - save_investment_list
-#   - investment_data
-#   - holding_dates
-#   - asset_flow
-# For the time being, we will leave this as-is to keep things working. Moving forward, we must re-design the
-# exception handling so that we don't have these types of special cases where error_handler is only allowed on some
-# methods but not others.
-@_decorator.typechecked
-def get_investment_data(
-    investments: Union[List[str], str, Dict[str, Any]],
-    data_points: Optional[Union[List[Dict[str, Any]], str, DataFrame, List[Any]]] = None,
-    display_name: bool = False,
-) -> DataFrame:
-    """Retrieve data for the specified investments and data points.
-
-    Args:
-        investments (:obj:`Union`, `required`): Defines the investments to fetch. Input can be:
-
-            * Investment IDs (:obj:`list`, `optional`): Investment identifiers, in the format of SecId;Universe or just SecId. E.g., ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"]. Use the `investments <./lookup.html#morningstar_data.direct.investments>`_ function to discover identifiers.
-            * Investment List ID (:obj:`str`, `optional`): Saved investment list in Morningstar Direct. Currently, this function does not support lists that combine investments and user-created portfolios. Use the `get_investment_lists <./lists.html#morningstar_data.direct.user_items.get_investment_lists>`_ function to discover saved lists.
-            * Search Criteria  ID (:obj:`str`, `optional`): Saved search criteria in Morningstar Direct. Use the `get_search_criteria <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria>`_ function to discover saved search criteria.
-            * Search Criteria Condition (:obj:`dict`, `optional`): Search criteria definition. See details in the Reference section below or use the `get_search_criteria_conditions <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria_conditions>`_ function to discover the definition of a saved search criteria.
-
-        data_points (:obj:`Union`, `optional`): Defines the data points to fetch. If not provided and investments are specified with a list ID or search criteria ID, the corresponding bound dataset will be used.
-
-            * Data Point IDs (:obj:`List[Dict]`, `optional`): A list of dictionaries, each defining a data point and its (optional) associated settings.
-            * Data Set ID (:obj:`str`, `optional`): Morningstar data set or user-created data set saved in Morningstar Direct. Use the `get_data_sets <./data_set.html#morningstar_data.direct.user_items.get_data_sets>`_ or `get_morningstar_data_sets <./data_set.html#morningstar_data.direct.get_morningstar_data_sets>`_ functions to discover saved data sets.
-            * Data Point Settings (:obj:`DataFrame`, `optional`): A DataFrame of data point identifiers and their associated settings. Use the `get_data_set_details <./data_set.html#morningstar_data.direct.user_items.get_data_set_details>`_ function to discover data point settings from a saved data set.
-
-        display_name (:obj:`bool`, `optional`): When true, the returned column names will match display names saved in the data set. Default is false.
-
-    Returns:
-        DataFrame: A DataFrame object with investment data.
-
-    :Reference:
-
-        Constructing a Search Criteria Condition dictionary:
-
-        For example::
-
-                    SEARCH_CRITERIA_CONDITION = {
-                            "universeId": "cz",
-                            "subUniverseId": "",
-                            "subUniverseName": "",
-                            "securityStatus": "activeonly",
-                            "useDefinedPrimary": False,
-                            "criteria": [
-                                {"relation": "", "field": "HU338", "operator": "=", "value": "1"},
-                                {"relation": "AND", "field": "HU863", "operator": "=", "value": "1"}
-                            ]
-                        }
-
-        * universeId (:obj:`string`, `required`): Universe code (e.g., "FO"). Use the `get_investment_universes <./lookup.html#morningstar_data.direct.lookup.get_investment_universes>`_ function to explore available values or `download <../_static/assets/SearchCriteriaInfo.xlsx>`_ the reference file.
-        * subUniverseId (:obj:`string`, `optional`): Sub-universe code, if applicable. See the refererece file above for available values.
-        * subUniverseName (:obj:`string`, `optional`): Name of sub-universe, if applicable. See the refererece file above for available values.
-        * securityStatus (:obj:`string`, `optional`): Security status, can be 'activeonly' or 'activeinactive'.
-        * useDefinedPrimary (:obj:`Boolean`, `optional`): If set to true, Morningstar Direct user-defined settings will be used.
-        * criteria (:obj:`List[Dict[]]`, `required`): Custom search conditions. Dictionary fields described below.
-
-        The 'criteria' object consists of the following fields:
-            * field (:obj:`string`): Data point identifier
-            * value (:obj:`string`): Value to compare against the data point.
-            * criteria (:obj:`List[Dict[]]`): A nested list of additional custom search conditions.
-            * relation (:obj:`string`, `required`): Boolean condition used when joining with the previous condition. Accepts an empty string (for the first condition, as no previous condition exists to join with), 'Or', or 'And'.
-            * operator (:obj:`string`): Operator used to compare field value to value. Possible operators include '=', '!=', '<', '>', '<=', '>=', 'like' (data contains value), and 'not like' (data does not contain value).
-
-            For example::
-
-                [
-                    {
-                        "field": "eb919bcc-c097-4fe3-898c-470d8b89dde1"
-                        "operator": "="
-                        "relation": ""
-                        "value": "122"
-                    },
-                    {
-                        "criteria": [
-                            {...Condition1 },
-                            {...Condition2 },
-                            {...Condition3 },
-                        ],
-                        "relation": "And"
-                    },
-                    {
-                        "field": "LS466"
-                        "operator": "="
-                        "relation": "Or"
-                        "value": "FH"
-                    }
-                ]
-
-    :Examples:
-
-    Get investment data for the given investments and data points.
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.get_investment_data(
-            investments=["F0AUS05U7H", "F000010NJ5"],
-            data_points=[
-                {"datapointId": "OS01W"}, # Name
-                {"datapointId": "LS05M"}, # Base Currency
-                {
-                    "datapointId": "HP010", # Monthly Return
-                    "isTsdp": True,
-                    "currency": "CNY",
-                    "startDate": "2021-03-01",
-                    "endDate": "2021-08-31",
-                },
-            ],
-        )
-        df
-
-    :Output:
-        =================  ===================================  ================= =========================  =========================
-        Id                 Name                                 Base Currency     Monthly Return 2021-03-31  Monthly Return 2021-04-30
-        =================  ===================================  ================= =========================  =========================
-        F0AUS05U7H         Walter Scott Global Equity           Australian Dollar                  3.726094                   3.078352
-        F000010NJ5         Vontobel Emerging Markets Eq U1 USD  US Dollar                         -0.417526                  -0.376890
-        =================  ===================================  ================= =========================  =========================
-
-
-    Get investment data for a saved investment list and data points.
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.get_investment_data(
-            investments="a727113a-9557-4378-924f-5d2ba553f687", # Replace with a valid List ID
-            data_points=[{"datapointId": "HS793", "isTsdp": True}],
-        )
-        df
-
-    :Output:
-        ==============  =================================  =============================  =============================  =============================
-        Id              Name                               Daily Return Index 2021-09-23  Daily Return Index 2021-09-24  Daily Return Index 2021-09-25
-        ==============  =================================  =============================  =============================  =============================
-        FOUSA00DFS;FO   BlackRock Global Allocation Inv A  129.92672                      129.56781                      129.56781
-        ==============  =================================  =============================  =============================  =============================
-
-    Get investment data for a saved search criteria and data points
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.get_investment_data(
-            investments="4216254", # Replace with a valid Search Criteria ID
-            data_points=[{"datapointId": "12", "isTsdp": True}]
-        )
-        df
-
-    :Output:
-        ==============  =======================  =============================
-        Id              Name                     Beta 2018-10-01 to 2021-09-30
-        ==============  =======================  =============================
-        FOUSA06JNH;FO   DWS RREEF Real Assets A    0.654343
-        ==============  =======================  =============================
-
-    Get investment data for a custom search criteria and data points.
-
-    ::
-
-        import morningstar_data as md
-
-        SEARCH_CRITERIA_CONDITION = {
-            "universeId": "cz",
-            "subUniverseId": "",
-            "subUniverseName": "",
-            "securityStatus": "activeonly",
-            "useDefinedPrimary": False,
-            "criteria": [
-                {"relation": "", "field": "HU338", "operator": "=", "value": "1"},
-                {"relation": "AND", "field": "HU863", "operator": "=", "value": "1"},
-            ],
-        }
-
-        df = md.direct.get_investment_data(
-            investments=SEARCH_CRITERIA_CONDITION,
-            data_points=[{"datapointId": "HS793", "isTsdp": True}],
-        )
-        df
-
-    :Output:
-        =  ===============  =====================================  =============================  ===  =============================
-        #  Id               Name                                   Daily Return Index 2022-02-18  ...  Daily Return Index 2022-03-17
-        =  ===============  =====================================  =============================  ===  =============================
-        0  FOUSA06UOR;CZ    Columbia Trust Stable Government Fund  None                           ...  None
-        1  FOUSA06UWL;CZ    Columbia Trust Stable Income Fund      88.8333                        ...  90.7781
-        =  ===============  =====================================  =============================  ===  =============================
-
-
-
-
-    """
-    result = _get_investment_data(investments=investments, data_points=data_points, display_name=display_name)
-    return result
-
-
-def _get_investment_data(investments: InvestmentType, data_points: DataPointsType, display_name: bool = False) -> DataFrame:
-    investment_param = Investments(investments)
-    data_point_param = DataPoints(data_points)
-
-    # Get asset flow data
-    asset_flow_req = AssetFlowProvider.build_request(investment_param, data_point_param, display_name)
-    asset_flow_result = AssetFlowProvider.run_request(asset_flow_req)
-
-    # Get normal data
-    normal_data_req = NormalDataProvider.build_request(investment_param, data_point_param, display_name)
-    normal_data_result = NormalDataProvider.run_request(normal_data_req)
-
-    # Combine data
-    merged_result = asset_flow_result.merge_with(normal_data_result)
-
-    # Build data frame, re-order columns
-    data_points = _get_data_points(investment_param, data_point_param)
-    data_point_cols = _get_data_point_col_names(data_points, merged_result.get_data_point_alias_to_col_dict())
-    return merged_result.as_data_frame(order_cols_by=data_point_cols)
+from operator import inv
+import warnings
+from pandas import DataFrame
+from typing import Optional, List, Dict, Any, Union
+
+from . import _decorator
+from .._base import _logger
+from ._data_objects import Investments, InvestmentType, DataPoints, DataPointsType
+
+from ._investment._asset_flow_data import AssetFlowProvider
+from ._investment._normal_data import NormalDataProvider
+from ._investment._common import _get_data_points, _get_data_point_col_names
+
+
+@_decorator.typechecked
+def investment_data(
+    investments: Union[List[str], str, Dict[str, Any]],
+    datapoints: Union[List[Dict[str, Any]], str, DataFrame],
+) -> DataFrame:
+    warnings.warn(
+        "The investment_data function is deprecated and will be removed in the next major version. Use get_investment_data instead",
+        FutureWarning,
+        stacklevel=2,
+    )
+    return _get_investment_data(investments, datapoints)
+
+
+# FIXME: In https://msjira.morningstar.com/browse/AL2-92, the error_handler decorator was removed from some methods
+# to trigger QueryLimitException.
+# There are multiple methods where the decorator was removed to trigger certain exceptions back to the caller:
+#   - save_investment_list
+#   - investment_data
+#   - holding_dates
+#   - asset_flow
+# For the time being, we will leave this as-is to keep things working. Moving forward, we must re-design the
+# exception handling so that we don't have these types of special cases where error_handler is only allowed on some
+# methods but not others.
+@_decorator.typechecked
+def get_investment_data(
+    investments: Union[List[str], str, Dict[str, Any]],
+    data_points: Optional[Union[List[Dict[str, Any]], str, DataFrame, List[Any]]] = None,
+    display_name: bool = False,
+) -> DataFrame:
+    """Retrieve data for the specified investments and data points.
+
+    Args:
+        investments (:obj:`Union`, `required`): Defines the investments to fetch. Input can be:
+
+            * Investment IDs (:obj:`list`, `optional`): Investment identifiers, in the format of SecId;Universe or just SecId. E.g., ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"]. Use the `investments <./lookup.html#morningstar_data.direct.investments>`_ function to discover identifiers.
+            * Investment List ID (:obj:`str`, `optional`): Saved investment list in Morningstar Direct. Currently, this function does not support lists that combine investments and user-created portfolios. Use the `get_investment_lists <./lists.html#morningstar_data.direct.user_items.get_investment_lists>`_ function to discover saved lists.
+            * Search Criteria  ID (:obj:`str`, `optional`): Saved search criteria in Morningstar Direct. Use the `get_search_criteria <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria>`_ function to discover saved search criteria.
+            * Search Criteria Condition (:obj:`dict`, `optional`): Search criteria definition. See details in the Reference section below or use the `get_search_criteria_conditions <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria_conditions>`_ function to discover the definition of a saved search criteria.
+
+        data_points (:obj:`Union`, `optional`): Defines the data points to fetch. If not provided and investments are specified with a list ID or search criteria ID, the corresponding bound dataset will be used.
+
+            * Data Point IDs (:obj:`List[Dict]`, `optional`): A list of dictionaries, each defining a data point and its (optional) associated settings.
+            * Data Set ID (:obj:`str`, `optional`): Morningstar data set or user-created data set saved in Morningstar Direct. Use the `get_data_sets <./data_set.html#morningstar_data.direct.user_items.get_data_sets>`_ or `get_morningstar_data_sets <./data_set.html#morningstar_data.direct.get_morningstar_data_sets>`_ functions to discover saved data sets.
+            * Data Point Settings (:obj:`DataFrame`, `optional`): A DataFrame of data point identifiers and their associated settings. Use the `get_data_set_details <./data_set.html#morningstar_data.direct.user_items.get_data_set_details>`_ function to discover data point settings from a saved data set.
+
+        display_name (:obj:`bool`, `optional`): When true, the returned column names will match display names saved in the data set. Default is false.
+
+    Returns:
+        DataFrame: A DataFrame object with investment data.
+
+    :Reference:
+
+        Constructing a Search Criteria Condition dictionary:
+
+        For example::
+
+                    SEARCH_CRITERIA_CONDITION = {
+                            "universeId": "cz",
+                            "subUniverseId": "",
+                            "subUniverseName": "",
+                            "securityStatus": "activeonly",
+                            "useDefinedPrimary": False,
+                            "criteria": [
+                                {"relation": "", "field": "HU338", "operator": "=", "value": "1"},
+                                {"relation": "AND", "field": "HU863", "operator": "=", "value": "1"}
+                            ]
+                        }
+
+        * universeId (:obj:`string`, `required`): Universe code (e.g., "FO"). Use the `get_investment_universes <./lookup.html#morningstar_data.direct.lookup.get_investment_universes>`_ function to explore available values or `download <../_static/assets/SearchCriteriaInfo.xlsx>`_ the reference file.
+        * subUniverseId (:obj:`string`, `optional`): Sub-universe code, if applicable. See the refererece file above for available values.
+        * subUniverseName (:obj:`string`, `optional`): Name of sub-universe, if applicable. See the refererece file above for available values.
+        * securityStatus (:obj:`string`, `optional`): Security status, can be 'activeonly' or 'activeinactive'.
+        * useDefinedPrimary (:obj:`Boolean`, `optional`): If set to true, Morningstar Direct user-defined settings will be used.
+        * criteria (:obj:`List[Dict[]]`, `required`): Custom search conditions. Dictionary fields described below.
+
+        The 'criteria' object consists of the following fields:
+            * field (:obj:`string`): Data point identifier
+            * value (:obj:`string`): Value to compare against the data point.
+            * criteria (:obj:`List[Dict[]]`): A nested list of additional custom search conditions.
+            * relation (:obj:`string`, `required`): Boolean condition used when joining with the previous condition. Accepts an empty string (for the first condition, as no previous condition exists to join with), 'Or', or 'And'.
+            * operator (:obj:`string`): Operator used to compare field value to value. Possible operators include '=', '!=', '<', '>', '<=', '>=', 'like' (data contains value), and 'not like' (data does not contain value).
+
+            For example::
+
+                [
+                    {
+                        "field": "eb919bcc-c097-4fe3-898c-470d8b89dde1"
+                        "operator": "="
+                        "relation": ""
+                        "value": "122"
+                    },
+                    {
+                        "criteria": [
+                            {...Condition1 },
+                            {...Condition2 },
+                            {...Condition3 },
+                        ],
+                        "relation": "And"
+                    },
+                    {
+                        "field": "LS466"
+                        "operator": "="
+                        "relation": "Or"
+                        "value": "FH"
+                    }
+                ]
+
+    :Examples:
+
+    Get investment data for the given investments and data points.
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.get_investment_data(
+            investments=["F0AUS05U7H", "F000010NJ5"],
+            data_points=[
+                {"datapointId": "OS01W"}, # Name
+                {"datapointId": "LS05M"}, # Base Currency
+                {
+                    "datapointId": "HP010", # Monthly Return
+                    "isTsdp": True,
+                    "currency": "CNY",
+                    "startDate": "2021-03-01",
+                    "endDate": "2021-08-31",
+                },
+            ],
+        )
+        df
+
+    :Output:
+        =================  ===================================  ================= =========================  =========================
+        Id                 Name                                 Base Currency     Monthly Return 2021-03-31  Monthly Return 2021-04-30
+        =================  ===================================  ================= =========================  =========================
+        F0AUS05U7H         Walter Scott Global Equity           Australian Dollar                  3.726094                   3.078352
+        F000010NJ5         Vontobel Emerging Markets Eq U1 USD  US Dollar                         -0.417526                  -0.376890
+        =================  ===================================  ================= =========================  =========================
+
+
+    Get investment data for a saved investment list and data points.
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.get_investment_data(
+            investments="a727113a-9557-4378-924f-5d2ba553f687", # Replace with a valid List ID
+            data_points=[{"datapointId": "HS793", "isTsdp": True}],
+        )
+        df
+
+    :Output:
+        ==============  =================================  =============================  =============================  =============================
+        Id              Name                               Daily Return Index 2021-09-23  Daily Return Index 2021-09-24  Daily Return Index 2021-09-25
+        ==============  =================================  =============================  =============================  =============================
+        FOUSA00DFS;FO   BlackRock Global Allocation Inv A  129.92672                      129.56781                      129.56781
+        ==============  =================================  =============================  =============================  =============================
+
+    Get investment data for a saved search criteria and data points
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.get_investment_data(
+            investments="4216254", # Replace with a valid Search Criteria ID
+            data_points=[{"datapointId": "12", "isTsdp": True}]
+        )
+        df
+
+    :Output:
+        ==============  =======================  =============================
+        Id              Name                     Beta 2018-10-01 to 2021-09-30
+        ==============  =======================  =============================
+        FOUSA06JNH;FO   DWS RREEF Real Assets A    0.654343
+        ==============  =======================  =============================
+
+    Get investment data for a custom search criteria and data points.
+
+    ::
+
+        import morningstar_data as md
+
+        SEARCH_CRITERIA_CONDITION = {
+            "universeId": "cz",
+            "subUniverseId": "",
+            "subUniverseName": "",
+            "securityStatus": "activeonly",
+            "useDefinedPrimary": False,
+            "criteria": [
+                {"relation": "", "field": "HU338", "operator": "=", "value": "1"},
+                {"relation": "AND", "field": "HU863", "operator": "=", "value": "1"},
+            ],
+        }
+
+        df = md.direct.get_investment_data(
+            investments=SEARCH_CRITERIA_CONDITION,
+            data_points=[{"datapointId": "HS793", "isTsdp": True}],
+        )
+        df
+
+    :Output:
+        =  ===============  =====================================  =============================  ===  =============================
+        #  Id               Name                                   Daily Return Index 2022-02-18  ...  Daily Return Index 2022-03-17
+        =  ===============  =====================================  =============================  ===  =============================
+        0  FOUSA06UOR;CZ    Columbia Trust Stable Government Fund  None                           ...  None
+        1  FOUSA06UWL;CZ    Columbia Trust Stable Income Fund      88.8333                        ...  90.7781
+        =  ===============  =====================================  =============================  ===  =============================
+
+
+
+
+    """
+    result = _get_investment_data(investments=investments, data_points=data_points, display_name=display_name)
+    return result
+
+
+def _get_investment_data(investments: InvestmentType, data_points: DataPointsType, display_name: bool = False) -> DataFrame:
+    investment_param = Investments(investments)
+    data_point_param = DataPoints(data_points)
+
+    # Get asset flow data
+    asset_flow_req = AssetFlowProvider.build_request(investment_param, data_point_param, display_name)
+    asset_flow_result = AssetFlowProvider.run_request(asset_flow_req)
+
+    # Get normal data
+    normal_data_req = NormalDataProvider.build_request(investment_param, data_point_param, display_name)
+    normal_data_result = NormalDataProvider.run_request(normal_data_req)
+
+    # Combine data
+    merged_result = asset_flow_result.merge_with(normal_data_result)
+
+    # Build data frame, re-order columns
+    data_points = _get_data_points(investment_param, data_point_param)
+    data_point_cols = _get_data_point_col_names(data_points, merged_result.get_data_point_alias_to_col_dict())
+    return merged_result.as_data_frame(order_cols_by=data_point_cols)
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/peer_group.py` & `morningstar_data-1.3.0/morningstar_data/direct/peer_group.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,90 +1,90 @@
-from pandas import DataFrame
-from typing import Optional, List, Any, Dict, Union
-
-from . import _decorator
-from .data_type import PeerGroupMethodology, Order
-from .._base import _logger
-from ._config import _Config
-from ._data_objects import Investments, DataPoints
-from ._investment._peer_group_data import PeerGroupProvider
-
-_config = _Config()
-peer_group_provider = PeerGroupProvider()
-
-
-@_decorator.typechecked
-def get_peer_group_breakpoints(
-    investments: Union[List[str], str],
-    data_points: Union[List[Dict[str, Any]], DataFrame],
-    order: Order = Order.ASC,
-    percentiles: Optional[List[int]] = list(range(1, 101)),
-    methodology: Optional[PeerGroupMethodology] = None,
-) -> DataFrame:
-
-    """Returns peer group breakpoints for the specified list of investments and data points.
-
-    Args:
-        investments (:obj:`Union`, `required`): Defines the investments to fetch. Input can be:
-
-            * Investment IDs (:obj:`list`, `optional`): Investment identifiers, in the format of SecId;Universe or just SecId. E.g., ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"]. Use the `investments <./lookup.html#morningstar_data.direct.investments>`_ function to discover identifiers.
-            * Investment List ID (:obj:`str`, `optional`): Saved investment list in Morningstar Direct. Use the `get_investment_lists <./lists.html#morningstar_data.direct.user_items.get_investment_lists>`_ function to discover saved lists.
-            * Search Criteria  ID (:obj:`str`, `optional`): Saved search criteria in Morningstar Direct. Use the `get_search_criteria <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria>`_ function to discover saved search criteria.
-            * Search Criteria Condition (:obj:`dict`, `optional`): Search criteria definition. See details in the Reference section of `get_investment_data <./investment.html#morningstar_data.direct.get_investment_data>`_ or use the `get_search_criteria_conditions <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria_conditions>`_ function to discover the definition of a saved search criteria.
-
-        data_points (:obj:`Union`, `optional`): Defines the data points to fetch. If not provided and investments are specified with a list ID or search criteria ID, the corresponding bound dataset will be used.
-
-            * Data Point IDs (:obj:`List[Dict]`, `optional`): A list of dictionaries, each defining a data point and its (optional) associated settings. The optional `alias` attribute can be added to each data point and will be used in the response, e.g., [{"datapointId": "41", "alias": "Z1"}. Use `get_data_set_details <./data_set.html#morningstar_data.direct.user_items.get_data_set_details>`_ to discover data point identifiers from a saved data set.
-            * Data Point Settings (:obj:`DataFrame`, `optional`): A DataFrame of data point identifiers and their associated settings. Use the `get_data_set_details <./data_set.html#morningstar_data.direct.user_items.get_data_set_details>`_ function to discover data point settings from a saved data set.
-
-        order (:obj:`Order`, `optional`): Breakpoint order, can be set to `md.direct.Order.DESC` (descending) or `md.direct.Order.ASC` (ascending, default).
-        percentiles (:obj:`list`, `optional`): Percentiles default to a list [1,2,3,...,100] if not provided, values should be within 1-100 range.
-        methodology (:obj:`PeerGroupMethodology`, `optional`): Breakpoint calculation methodology, can be set to `md.direct.PeerGroupMethodology.MORNINGSTAR` or `md.direct.PeerGroupMethodology.SIMPLE`. Defaults to the global setting "Custom Peer Group Ranking" in Morningstar Direct if not provided.
-
-    Returns:
-        DataFrame: A DataFrame object with peer group breakpoint data. The columns include the `alias` that the user
-        input in the `data_points` parameter.
-
-    :Examples:
-
-    Get peer group breakpoint data for the standard deviation data point.
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.get_peer_group_breakpoints(
-                investments='740284aa-fcd3-43f6-99d1-8f3d4a179fcc',
-                data_points=[
-                    {"datapointId": "41", "alias": "Z1"},
-                    {"datapointId": "41", "alias": "Z2", "startDate": "2021-07-01", "endDate": "2021-12-31", "windowType": "2", "windowSize": "3", "stepSize": "2"}
-                ],
-                order=md.direct.Order.ASC,
-                percentiles=[25, 50, 75, 100]
-            )
-        df
-
-    :Output:
-        ======  ===========  ==========  ==========  ==========  ==========  ==========
-        Alias   StartDate    EndDate     25          50          75          100
-        ======  ===========  ==========  ==========  ==========  ==========  ==========
-        Z1      2019-04-01   2022-03-31  17.301437   12.720889   7.055372    -3.460187
-        Z2      2021-07-01   2021-09-30  1.827371    -0.804269   -4.899745   -52.143678
-        Z2      2021-09-01   2021-11-30  -0.030321   -4.336051   -10.618009  -40.980480
-        ======  ===========  ==========  ==========  ==========  ==========  ==========
-
-    Errors:
-        AccessDeniedError: Raised when the user lacks permission or is not authorized to access the resource.
-
-        BadRequestException: Raised due to invalid/incorrect request, malformed request syntax, or deceptive request routing.
-
-        NetworkExceptionError: Raised when there is an issue with the internet connection or if the request is made from an unsecure network.
-
-        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
-
-    """
-    investment_param = Investments(investments)
-    data_point_param = DataPoints(data_points)
-
-    peer_group_req = peer_group_provider.build_request(investment_param, data_point_param, order=order, percentiles=percentiles, methodology=methodology)
-    peer_group_resp = peer_group_provider.run_request(peer_group_req)
-    return peer_group_provider.build_data_frame(peer_group_resp)
+from pandas import DataFrame
+from typing import Optional, List, Any, Dict, Union
+
+from . import _decorator
+from .data_type import PeerGroupMethodology, Order
+from .._base import _logger
+from ._config import _Config
+from ._data_objects import Investments, DataPoints
+from ._investment._peer_group_data import PeerGroupProvider
+
+_config = _Config()
+peer_group_provider = PeerGroupProvider()
+
+
+@_decorator.typechecked
+def get_peer_group_breakpoints(
+    investments: Union[List[str], str],
+    data_points: Union[List[Dict[str, Any]], DataFrame],
+    order: Order = Order.ASC,
+    percentiles: Optional[List[int]] = list(range(1, 101)),
+    methodology: Optional[PeerGroupMethodology] = None,
+) -> DataFrame:
+
+    """Returns peer group breakpoints for the specified list of investments and data points.
+
+    Args:
+        investments (:obj:`Union`, `required`): Defines the investments to fetch. Input can be:
+
+            * Investment IDs (:obj:`list`, `optional`): Investment identifiers, in the format of SecId;Universe or just SecId. E.g., ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"]. Use the `investments <./lookup.html#morningstar_data.direct.investments>`_ function to discover identifiers.
+            * Investment List ID (:obj:`str`, `optional`): Saved investment list in Morningstar Direct. Use the `get_investment_lists <./lists.html#morningstar_data.direct.user_items.get_investment_lists>`_ function to discover saved lists.
+            * Search Criteria  ID (:obj:`str`, `optional`): Saved search criteria in Morningstar Direct. Use the `get_search_criteria <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria>`_ function to discover saved search criteria.
+            * Search Criteria Condition (:obj:`dict`, `optional`): Search criteria definition. See details in the Reference section of `get_investment_data <./investment.html#morningstar_data.direct.get_investment_data>`_ or use the `get_search_criteria_conditions <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria_conditions>`_ function to discover the definition of a saved search criteria.
+
+        data_points (:obj:`Union`, `optional`): Defines the data points to fetch. If not provided and investments are specified with a list ID or search criteria ID, the corresponding bound dataset will be used.
+
+            * Data Point IDs (:obj:`List[Dict]`, `optional`): A list of dictionaries, each defining a data point and its (optional) associated settings. The optional `alias` attribute can be added to each data point and will be used in the response, e.g., [{"datapointId": "41", "alias": "Z1"}. Use `get_data_set_details <./data_set.html#morningstar_data.direct.user_items.get_data_set_details>`_ to discover data point identifiers from a saved data set.
+            * Data Point Settings (:obj:`DataFrame`, `optional`): A DataFrame of data point identifiers and their associated settings. Use the `get_data_set_details <./data_set.html#morningstar_data.direct.user_items.get_data_set_details>`_ function to discover data point settings from a saved data set.
+
+        order (:obj:`Order`, `optional`): Breakpoint order, can be set to `md.direct.Order.DESC` (descending) or `md.direct.Order.ASC` (ascending, default).
+        percentiles (:obj:`list`, `optional`): Percentiles default to a list [1,2,3,...,100] if not provided, values should be within 1-100 range.
+        methodology (:obj:`PeerGroupMethodology`, `optional`): Breakpoint calculation methodology, can be set to `md.direct.PeerGroupMethodology.MORNINGSTAR` or `md.direct.PeerGroupMethodology.SIMPLE`. Defaults to the global setting "Custom Peer Group Ranking" in Morningstar Direct if not provided.
+
+    Returns:
+        DataFrame: A DataFrame object with peer group breakpoint data. The columns include the `alias` that the user
+        input in the `data_points` parameter.
+
+    :Examples:
+
+    Get peer group breakpoint data for the standard deviation data point.
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.get_peer_group_breakpoints(
+                investments='740284aa-fcd3-43f6-99d1-8f3d4a179fcc',
+                data_points=[
+                    {"datapointId": "41", "alias": "Z1"},
+                    {"datapointId": "41", "alias": "Z2", "startDate": "2021-07-01", "endDate": "2021-12-31", "windowType": "2", "windowSize": "3", "stepSize": "2"}
+                ],
+                order=md.direct.Order.ASC,
+                percentiles=[25, 50, 75, 100]
+            )
+        df
+
+    :Output:
+        ======  ===========  ==========  ==========  ==========  ==========  ==========
+        Alias   StartDate    EndDate     25          50          75          100
+        ======  ===========  ==========  ==========  ==========  ==========  ==========
+        Z1      2019-04-01   2022-03-31  17.301437   12.720889   7.055372    -3.460187
+        Z2      2021-07-01   2021-09-30  1.827371    -0.804269   -4.899745   -52.143678
+        Z2      2021-09-01   2021-11-30  -0.030321   -4.336051   -10.618009  -40.980480
+        ======  ===========  ==========  ==========  ==========  ==========  ==========
+
+    Errors:
+        AccessDeniedError: Raised when the user lacks permission or is not authorized to access the resource.
+
+        BadRequestException: Raised due to invalid/incorrect request, malformed request syntax, or deceptive request routing.
+
+        NetworkExceptionError: Raised when there is an issue with the internet connection or if the request is made from an unsecure network.
+
+        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
+
+    """
+    investment_param = Investments(investments)
+    data_point_param = DataPoints(data_points)
+
+    peer_group_req = peer_group_provider.build_request(investment_param, data_point_param, order=order, percentiles=percentiles, methodology=methodology)
+    peer_group_resp = peer_group_provider.run_request(peer_group_req)
+    return peer_group_provider.build_data_frame(peer_group_resp)
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/performance_report.py` & `morningstar_data-1.3.0/morningstar_data/direct/performance_report.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,522 +1,522 @@
-import requests
-import shutil
-
-from pandas import DataFrame
-from typing import List, Optional, Dict, Any, Union, Callable
-
-from datetime import datetime
-from urllib.parse import quote
-
-from .._base import _logger
-from . import _decorator
-from . import _error_messages
-from ._config import _Config
-from ._core_api import make_request
-from ._exceptions import BadRequestException, NetworkExceptionError, AccessDeniedError, ValueErrorException, ResourceNotFoundError
-from ._error_messages import RESOURCE_NOT_FOUND_ERROR_PERFORMANCE_REPORT
-from ._base_api import APIBackend
-
-_config = _Config()
-
-
-class PerformanceReportAPIBackend(APIBackend):
-    """
-    Subclass to call the Performance Report API and handle any HTTP errors that occur.
-    """
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def _handle_custom_http_errors(self, res: Any) -> Any:
-        """
-        Handle HTTP errors with custom error messages
-        """
-        response_message = res.json().get("message", "")
-        if res.status_code == 404:
-            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
-            raise ResourceNotFoundError(RESOURCE_NOT_FOUND_ERROR_PERFORMANCE_REPORT) from None
-
-
-_performance_report_api_request = PerformanceReportAPIBackend()
-
-
-@_decorator.typechecked
-def get_reports() -> DataFrame:
-    """Returns all performance reports saved or shared to a user in Morningstar Direct.
-
-    Returns:
-        DataFrame: A DataFrame object with all performance reports. DataFrame columns include:
-
-        * reportId
-        * name
-        * permission
-        * ownerId
-        * shared
-        * createdOn
-        * lastCalculatedOn
-        * folderId
-
-    :Examples:
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.performance_report.get_reports()
-        df
-
-    :Output:
-        ========  ======  ==========  =======  ======  ====================  ================  ========
-        reportId  name    permission  ownerId  shared  createdOn             lastCalculatedOn  folderId
-        ========  ======  ==========  =======  ======  ====================  ================  ========
-        4940775   sample  READ_WRITE  XXX      False   2017-08-17T09:39:00Z                    1
-        ...
-        ========  ======  ==========  =======  ======  ====================  ================  ========
-
-    Errors:
-        AccessDeniedError: Raised when the user is not authenticated.
-
-        ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-    """
-    url = f"{_config.performancereport_service_url()}v1/reports"
-    response_json: Dict[str, Any] = _performance_report_api_request.do_get_request(url)
-    return DataFrame(response_json["reports"])
-
-
-@_decorator.not_null
-@_decorator.typechecked
-def get_report(report_id: str) -> DataFrame:
-    """Returns performance report data for the specified report ID.
-
-    Args:
-        report_id (:obj:`str`): Unique identifier of a saved performance report from the Performance Reporting
-            module in Morningstar Direct, e.g., "7782164". Use `get_reports <#morningstar_data.direct.get_reports>`_ to discover possible values.
-
-    Returns:
-        DataFrame: A DataFrame object with calculated performance report data. Columns include all columns
-        that the user configured in the performance report.
-
-    Examples:
-        Get performance report data.
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.performance_report.get_report(report_id="2463866") # Replace with a valid report ID
-        df
-
-    :Output:
-        ================  ===========  =============  =========================  ======
-        Group/Investment  Object Type  Display Group  Peer Group                 Ticker
-        ================  ===========  =============  =========================  ======
-        sample            investments  Unclassified   Peer Group: Display Group  XXX
-        ================  ===========  =============  =========================  ======
-
-    Errors:
-        AccessDeniedError: Raised when the user is not authenticated.
-
-        ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-        BadRequestError: Raised when the user does not provide a properly formatted request.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
-    """
-    url = f"{_config.performancereport_service_url()}v1/reports/{report_id}"
-    response_json: Dict[str, Any] = _performance_report_api_request.do_get_request(url)
-    return _merge_datas(response_json)
-
-
-def _get_all_columns(columns: List[Dict[str, Any]], name_master: Optional[str] = None) -> List[Dict[str, Any]]:
-    all_columns = []
-    for column in columns:
-        if "hidden" in column and column["hidden"] is True:
-            continue
-        elif "children" in column:
-            all_columns += _get_all_columns(column["children"], column["name"])
-        elif name_master is None and column["name"] == "Name":
-            column["fullName"] = "Group/Investment"
-            all_columns.append(column)
-            all_columns.append({"fullName": "Object Type", "id": "ObjectType"})
-            all_columns.append({"fullName": "Display Group", "id": "DisplayGroup"})
-            all_columns.append({"fullName": "Peer Group", "id": "PeerGroup"})
-        else:
-            column["fullName"] = name_master + " " + column["name"] if name_master is not None else column["name"]
-            if column.get("mstarIpType", "") == "":
-                all_columns.append(column)
-            else:
-                all_columns.append({"fullName": column["fullName"], "id": column["id"]})
-                all_columns.append(
-                    {
-                        "fullName": column["fullName"] + " - display text",
-                        "id": column["id"],
-                        "ismstarip": True,
-                    }
-                )
-
-    return all_columns
-
-
-def _get_all_columns_name(columns: List[Dict[str, Any]]) -> List[str]:
-    all_columns = []
-    for c in columns:
-        all_columns.append(c["fullName"])
-    return all_columns
-
-
-def _filter_grouy_by_type(groups: List[Dict[str, Any]], type: str) -> Dict[str, Any]:
-    get_by_type: Callable = lambda group: group["type"] == type
-    get_id: Callable = lambda group: group["id"]
-    new_groups = list(filter(get_by_type, groups))
-    groups_group_id = list(map(get_id, new_groups))
-    groups_group_dict = dict(zip(groups_group_id, new_groups))
-    return groups_group_dict
-
-
-def _get_data_dict(datas: Dict[str, Any], name: str) -> Dict[str, Any]:
-    get_id: Callable = lambda datas: datas[name]
-    datas_id = list(map(get_id, datas))
-    return dict(zip(datas_id, datas))
-
-
-def _set_data_rows(values: Dict[str, Any], columns: List[Any], switch: Dict[str, Any]) -> List[Any]:
-    set_data = []
-    for col in columns:
-        col_id = col["id"]
-        to_add = switch.get(col_id, None)
-        if to_add is not None:
-            set_data.append(to_add)
-        elif col_id in values:
-            if col.get("ismstarip", False):
-                set_data.append(values[col_id].get("text", ""))
-            else:
-                set_data.append(values[col_id].get("value", ""))
-        else:
-            set_data.append("")
-
-    return set_data
-
-
-def _get_data_rows(
-    investments: List[Dict[str, Any]],
-    groups_group: Dict[str, Any],
-    new_columns: List[Dict[str, Any]],
-    ObjectType: Any,
-    PeerGroup: Any,
-) -> List[Any]:
-    output_datas = []
-    for inv in investments:
-        group_id = inv["groupId"]
-        values_dict = _get_data_dict(inv["values"], "alias")
-        switch = {
-            "ObjectType": ObjectType,
-            "DisplayGroup": groups_group[group_id]["name"],
-            "PeerGroup": PeerGroup,
-        }
-        output_datas.append(_set_data_rows(values_dict, new_columns, switch))
-    return output_datas
-
-
-def _filter_datas_by_group_id(datas: List[Dict[str, Any]], group_id: str) -> List[Dict[str, Any]]:
-    get_by_id = lambda data: data["groupId"] == group_id
-    new_datas = list(filter(get_by_id, datas))
-    return new_datas
-
-
-def _get_sub_group(groups_data: List[Dict[str, Any]], group_id: str) -> Dict[str, Any]:
-    get_id = lambda group: group["id"]
-    get_by_group_id = lambda data: "groupId" in data and data["groupId"] == group_id
-    new_groups = list(filter(get_by_group_id, groups_data))
-    groups_group_id = list(map(get_id, new_groups))
-    return dict(zip(groups_group_id, new_groups))
-
-
-def _get_group_data_rows(
-    datas: List[Dict[str, Any]],
-    groups_group: Any,
-    new_columns: List[Dict[str, Any]],
-    ObjectType: Any,
-    group_name: Any,
-) -> List[Any]:
-    output_datas = []
-    switch = {
-        "ObjectType": ObjectType,
-        "DisplayGroup": group_name,
-        "PeerGroup": "",
-    }
-
-    for inv in datas:
-        values_dict = _get_data_dict(inv["values"], "alias")
-        output_datas.append(_set_data_rows(values_dict, new_columns, switch))
-
-    return output_datas
-
-
-def _get_peer_group_name_by_group_id(group_peer_groups: Union[Dict[Any, Any], Any]) -> Any:
-
-    if group_peer_groups and group_peer_groups[0] and group_peer_groups[0]["values"] and group_peer_groups[0]["values"][0] and group_peer_groups[0]["values"][0]["value"]:
-        return group_peer_groups[0]["values"][0]["value"]
-
-    return ""
-
-
-def _merge_datas(performance_report_data: Dict[str, Any]) -> DataFrame:
-    metadata = performance_report_data["metaData"]
-    view = metadata["view"]
-    if view and view["id"] == "5":
-        raise BadRequestException("This view not supported: " + view["name"])
-
-    subtype_name = {
-        "PeerGroup": "Peer Group Statistics",
-        "DisplayGroup": "Display Group Statistics",
-    }
-
-    columns = performance_report_data["columns"]
-    investments = performance_report_data["investments"]
-    benchmarks = performance_report_data["benchmarks"]
-    groups_data = performance_report_data["groups"]
-    peer_groups = performance_report_data["peerGroups"]
-    ranks = performance_report_data["ranks"]
-    summary_statistics = performance_report_data["summaryStatistics"]
-
-    all_data_row = []
-    new_columns = _get_all_columns(columns)
-    new_columns_name = _get_all_columns_name(new_columns)
-
-    get_by_type = lambda group: group["type"] == "Group"
-    new_groups = list(filter(get_by_type, groups_data))
-    groups_group = _filter_grouy_by_type(groups_data, "Group")
-    for group in new_groups:
-        group_id = group["id"]
-        group_name = group["name"]
-        sub_groups = _get_sub_group(groups_data, group_id)
-        group_investments = _filter_datas_by_group_id(investments, group_id)
-        group_benchmarks = _filter_datas_by_group_id(benchmarks, group_id)
-        group_peer_groups = _filter_datas_by_group_id(peer_groups, group_id)
-        group_ranks = _filter_datas_by_group_id(ranks, group_id)
-        peer_group_name = _get_peer_group_name_by_group_id(group_peer_groups)
-        all_data_row.extend(
-            _get_data_rows(
-                group_investments,
-                groups_group,
-                new_columns,
-                "investments",
-                peer_group_name,
-            )
-        )
-        all_data_row.extend(_get_data_rows(group_benchmarks, groups_group, new_columns, "Display Benchmark", ""))
-        all_data_row.extend(_get_group_data_rows(group_peer_groups, groups_group, new_columns, "PeerGroup", group_name))
-        all_data_row.extend(_get_group_data_rows(group_ranks, groups_group, new_columns, "Ranks", group_name))
-
-        for key in sub_groups:
-            subtype = sub_groups[key]["type"]
-
-            if subtype in subtype_name:
-                sub_peer_groups = _filter_datas_by_group_id(summary_statistics, sub_groups[key]["id"])
-                all_data_row.extend(
-                    _get_group_data_rows(
-                        sub_peer_groups,
-                        sub_peer_groups,
-                        new_columns,
-                        subtype_name[subtype],
-                        group_name,
-                    )
-                )
-
-    lssilss = _filter_datas_by_group_id(summary_statistics, "lssilss")
-    if lssilss:
-        all_data_row.extend(_get_group_data_rows(lssilss, lssilss, new_columns, "List Summary Statistics", ""))
-
-    data_frame = DataFrame(all_data_row)
-    data_frame.columns = new_columns_name
-    return data_frame
-
-
-@_decorator.not_null
-@_decorator.typechecked
-def calculate_report(report_id: str) -> DataFrame:
-    """Initiates re-calculation of a performance report.
-
-    Args:
-        report_id (:obj:`str`): Unique identifier of a saved performance report from the Performance Reporting
-            module in Morningstar Direct, e.g., "7782164". Use `get_reports <#morningstar_data.direct.get_reports>`_ to discover possible values.
-
-    Returns:
-        DataFrame: A DataFrame object confirming that report calculation was triggered. DataFrame columns include:
-
-         * reportId
-         * success
-
-    Raises:
-        ValueErrorException: Raised when the `report_id` parameter is invalid.
-
-    Examples:
-        Calculate the performance report.
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.performance_report.calculate_report(report_id="7128568") # Replace with a valid report ID
-        df
-
-    :Output:
-        ========  =======
-        reportId  success
-        ========  =======
-        7128568   True
-        ========  =======
-
-    Errors:
-        AccessDeniedError: Raised when the user is not authenticated.
-
-        ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-        BadRequestError: Raised when the user does not provide a properly formatted request.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-    """
-    df = get_report_status(report_id)
-    if df["status"].values[0] == "Ready" or df["status"].values[0] == "Failed":
-        url = f"{_config.performancereport_service_url()}v1/reports/calc/{report_id}"
-        response_json = _performance_report_api_request.do_post_request(url)
-        return DataFrame(response_json)
-    else:
-        raise ValueErrorException(f"report {report_id} is calculating.")
-
-
-@_decorator.not_null
-@_decorator.typechecked
-def get_report_status(report_id: str) -> DataFrame:
-    """Returns the current calculation status of the specified performance report. Possible statuses are:
-
-    * Failed
-    * Queued
-    * Calculating
-    * Generating Report
-    * Merging Excel
-    * Downloading
-    * Ready
-
-    Args:
-        report_id (:obj:`str`): Unique identifier of a saved performance report from the Performance Reporting
-            module in Morningstar Direct, e.g., "7782164". Use `get_reports <#morningstar_data.direct.get_reports>`_ to discover possible values.
-
-    Returns:
-        DataFrame: A DataFrame object with calculation status. DataFrame columns include:
-
-        * reportId
-        * status
-
-    Examples:
-        Get performance report calculation status.
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.performance_report.get_report_status(report_id="2463866") # Replace with a valid report ID
-        df
-
-    :Output:
-        ========  ======
-        reportId  status
-        ========  ======
-        2463866   Ready
-        ========  ======
-
-    Errors:
-        AccessDeniedError: Raised when the user is not authenticated.
-
-        ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-        BadRequestError: Raised when the user does not provide a properly formatted request.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-    """
-    url = f"{_config.performancereport_service_url()}v1/reports/status/{report_id}"
-    response_json = _performance_report_api_request.do_get_request(url)
-    return DataFrame(response_json)
-
-
-@_decorator.not_null
-@_decorator.typechecked
-def export_to_excel(report_id: str, file_name: Optional[str] = None) -> str:
-    """Export a performance report to Excel.
-
-    Args:
-        report_id (:obj:`str`): Unique identifier of a saved performance report from the Performance Reporting
-            module in Morningstar Direct, e.g., "7782164". Use `get_reports <#morningstar_data.direct.get_reports>`_ to discover possible values.
-        file_name (:obj:`str`, `optional`): Custom file name for the exported Excel file. If not provided, a default name with the format "report_<report_id>" will be used, e.g., "report_7782164.xlsx".
-
-    Returns:
-        str: Excel file name of the exported performance report.
-
-
-    Examples:
-        Export the given performance report.
-
-    ::
-
-        import morningstar_data as md
-
-        resp = md.direct.performance_report.export_to_excel(report_id="2442678") # Replace with a valid report ID
-        resp
-
-    :Output:
-        report_2442678.xlsx
-
-
-    Errors:
-        AccessDeniedError: Raised when the user is not authenticated.
-
-        ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-        BadRequestError: Raised when the user does not provide a properly formatted request.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
-
-    """
-    report_id_parse = quote(report_id, "utf-8")
-    url = f"{_config.performancereport_export_service_url()}v1/reports/export/{report_id_parse}"
-    presigned_url_response = _performance_report_api_request.do_get_request(url=url)
-
-    current_date_time = datetime.now().strftime("%Y%m%d_%H%M%S")
-    excel_file_suffix = ".xlsx"
-    if file_name is None or file_name == "":
-        file_name = f"performance_report_{report_id}_{current_date_time}.xlsx"
-    elif not file_name.endswith(excel_file_suffix):
-        file_name = file_name + excel_file_suffix
-    try:
-        url = presigned_url_response["url"]
-        response = requests.get(url, stream=True)
-        response.raise_for_status()
-        with open(file_name, "wb") as excel_file:
-            response.raw.decode_content = True
-            shutil.copyfileobj(response.raw, excel_file)
-        return file_name
-    # Catching HTTPErrors as this is presigned URL from bucket no do_get_request is used
-    except requests.ConnectionError as e:
-        _logger.error(e)
-        raise NetworkExceptionError from None
-    except requests.HTTPError as e:
-        _performance_report_api_request._handle_custom_http_errors(response)
-        _performance_report_api_request._handle_default_http_errors(response)
-        raise e
+import requests
+import shutil
+
+from pandas import DataFrame
+from typing import List, Optional, Dict, Any, Union, Callable
+
+from datetime import datetime
+from urllib.parse import quote
+
+from .._base import _logger
+from . import _decorator
+from . import _error_messages
+from ._config import _Config
+from ._core_api import make_request
+from ._exceptions import BadRequestException, NetworkExceptionError, AccessDeniedError, ValueErrorException, ResourceNotFoundError
+from ._error_messages import RESOURCE_NOT_FOUND_ERROR_PERFORMANCE_REPORT
+from ._base_api import APIBackend
+
+_config = _Config()
+
+
+class PerformanceReportAPIBackend(APIBackend):
+    """
+    Subclass to call the Performance Report API and handle any HTTP errors that occur.
+    """
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def _handle_custom_http_errors(self, res: Any) -> Any:
+        """
+        Handle HTTP errors with custom error messages
+        """
+        response_message = res.json().get("message", "")
+        if res.status_code == 404:
+            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
+            raise ResourceNotFoundError(RESOURCE_NOT_FOUND_ERROR_PERFORMANCE_REPORT) from None
+
+
+_performance_report_api_request = PerformanceReportAPIBackend()
+
+
+@_decorator.typechecked
+def get_reports() -> DataFrame:
+    """Returns all performance reports saved or shared to a user in Morningstar Direct.
+
+    Returns:
+        DataFrame: A DataFrame object with all performance reports. DataFrame columns include:
+
+        * reportId
+        * name
+        * permission
+        * ownerId
+        * shared
+        * createdOn
+        * lastCalculatedOn
+        * folderId
+
+    :Examples:
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.performance_report.get_reports()
+        df
+
+    :Output:
+        ========  ======  ==========  =======  ======  ====================  ================  ========
+        reportId  name    permission  ownerId  shared  createdOn             lastCalculatedOn  folderId
+        ========  ======  ==========  =======  ======  ====================  ================  ========
+        4940775   sample  READ_WRITE  XXX      False   2017-08-17T09:39:00Z                    1
+        ...
+        ========  ======  ==========  =======  ======  ====================  ================  ========
+
+    Errors:
+        AccessDeniedError: Raised when the user is not authenticated.
+
+        ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+    """
+    url = f"{_config.performancereport_service_url()}v1/reports"
+    response_json: Dict[str, Any] = _performance_report_api_request.do_get_request(url)
+    return DataFrame(response_json["reports"])
+
+
+@_decorator.not_null
+@_decorator.typechecked
+def get_report(report_id: str) -> DataFrame:
+    """Returns performance report data for the specified report ID.
+
+    Args:
+        report_id (:obj:`str`): Unique identifier of a saved performance report from the Performance Reporting
+            module in Morningstar Direct, e.g., "7782164". Use `get_reports <#morningstar_data.direct.get_reports>`_ to discover possible values.
+
+    Returns:
+        DataFrame: A DataFrame object with calculated performance report data. Columns include all columns
+        that the user configured in the performance report.
+
+    Examples:
+        Get performance report data.
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.performance_report.get_report(report_id="2463866") # Replace with a valid report ID
+        df
+
+    :Output:
+        ================  ===========  =============  =========================  ======
+        Group/Investment  Object Type  Display Group  Peer Group                 Ticker
+        ================  ===========  =============  =========================  ======
+        sample            investments  Unclassified   Peer Group: Display Group  XXX
+        ================  ===========  =============  =========================  ======
+
+    Errors:
+        AccessDeniedError: Raised when the user is not authenticated.
+
+        ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+        BadRequestError: Raised when the user does not provide a properly formatted request.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
+    """
+    url = f"{_config.performancereport_service_url()}v1/reports/{report_id}"
+    response_json: Dict[str, Any] = _performance_report_api_request.do_get_request(url)
+    return _merge_datas(response_json)
+
+
+def _get_all_columns(columns: List[Dict[str, Any]], name_master: Optional[str] = None) -> List[Dict[str, Any]]:
+    all_columns = []
+    for column in columns:
+        if "hidden" in column and column["hidden"] is True:
+            continue
+        elif "children" in column:
+            all_columns += _get_all_columns(column["children"], column["name"])
+        elif name_master is None and column["name"] == "Name":
+            column["fullName"] = "Group/Investment"
+            all_columns.append(column)
+            all_columns.append({"fullName": "Object Type", "id": "ObjectType"})
+            all_columns.append({"fullName": "Display Group", "id": "DisplayGroup"})
+            all_columns.append({"fullName": "Peer Group", "id": "PeerGroup"})
+        else:
+            column["fullName"] = name_master + " " + column["name"] if name_master is not None else column["name"]
+            if column.get("mstarIpType", "") == "":
+                all_columns.append(column)
+            else:
+                all_columns.append({"fullName": column["fullName"], "id": column["id"]})
+                all_columns.append(
+                    {
+                        "fullName": column["fullName"] + " - display text",
+                        "id": column["id"],
+                        "ismstarip": True,
+                    }
+                )
+
+    return all_columns
+
+
+def _get_all_columns_name(columns: List[Dict[str, Any]]) -> List[str]:
+    all_columns = []
+    for c in columns:
+        all_columns.append(c["fullName"])
+    return all_columns
+
+
+def _filter_grouy_by_type(groups: List[Dict[str, Any]], type: str) -> Dict[str, Any]:
+    get_by_type: Callable = lambda group: group["type"] == type
+    get_id: Callable = lambda group: group["id"]
+    new_groups = list(filter(get_by_type, groups))
+    groups_group_id = list(map(get_id, new_groups))
+    groups_group_dict = dict(zip(groups_group_id, new_groups))
+    return groups_group_dict
+
+
+def _get_data_dict(datas: Dict[str, Any], name: str) -> Dict[str, Any]:
+    get_id: Callable = lambda datas: datas[name]
+    datas_id = list(map(get_id, datas))
+    return dict(zip(datas_id, datas))
+
+
+def _set_data_rows(values: Dict[str, Any], columns: List[Any], switch: Dict[str, Any]) -> List[Any]:
+    set_data = []
+    for col in columns:
+        col_id = col["id"]
+        to_add = switch.get(col_id, None)
+        if to_add is not None:
+            set_data.append(to_add)
+        elif col_id in values:
+            if col.get("ismstarip", False):
+                set_data.append(values[col_id].get("text", ""))
+            else:
+                set_data.append(values[col_id].get("value", ""))
+        else:
+            set_data.append("")
+
+    return set_data
+
+
+def _get_data_rows(
+    investments: List[Dict[str, Any]],
+    groups_group: Dict[str, Any],
+    new_columns: List[Dict[str, Any]],
+    ObjectType: Any,
+    PeerGroup: Any,
+) -> List[Any]:
+    output_datas = []
+    for inv in investments:
+        group_id = inv["groupId"]
+        values_dict = _get_data_dict(inv["values"], "alias")
+        switch = {
+            "ObjectType": ObjectType,
+            "DisplayGroup": groups_group[group_id]["name"],
+            "PeerGroup": PeerGroup,
+        }
+        output_datas.append(_set_data_rows(values_dict, new_columns, switch))
+    return output_datas
+
+
+def _filter_datas_by_group_id(datas: List[Dict[str, Any]], group_id: str) -> List[Dict[str, Any]]:
+    get_by_id = lambda data: data["groupId"] == group_id
+    new_datas = list(filter(get_by_id, datas))
+    return new_datas
+
+
+def _get_sub_group(groups_data: List[Dict[str, Any]], group_id: str) -> Dict[str, Any]:
+    get_id = lambda group: group["id"]
+    get_by_group_id = lambda data: "groupId" in data and data["groupId"] == group_id
+    new_groups = list(filter(get_by_group_id, groups_data))
+    groups_group_id = list(map(get_id, new_groups))
+    return dict(zip(groups_group_id, new_groups))
+
+
+def _get_group_data_rows(
+    datas: List[Dict[str, Any]],
+    groups_group: Any,
+    new_columns: List[Dict[str, Any]],
+    ObjectType: Any,
+    group_name: Any,
+) -> List[Any]:
+    output_datas = []
+    switch = {
+        "ObjectType": ObjectType,
+        "DisplayGroup": group_name,
+        "PeerGroup": "",
+    }
+
+    for inv in datas:
+        values_dict = _get_data_dict(inv["values"], "alias")
+        output_datas.append(_set_data_rows(values_dict, new_columns, switch))
+
+    return output_datas
+
+
+def _get_peer_group_name_by_group_id(group_peer_groups: Union[Dict[Any, Any], Any]) -> Any:
+
+    if group_peer_groups and group_peer_groups[0] and group_peer_groups[0]["values"] and group_peer_groups[0]["values"][0] and group_peer_groups[0]["values"][0]["value"]:
+        return group_peer_groups[0]["values"][0]["value"]
+
+    return ""
+
+
+def _merge_datas(performance_report_data: Dict[str, Any]) -> DataFrame:
+    metadata = performance_report_data["metaData"]
+    view = metadata["view"]
+    if view and view["id"] == "5":
+        raise BadRequestException("This view not supported: " + view["name"])
+
+    subtype_name = {
+        "PeerGroup": "Peer Group Statistics",
+        "DisplayGroup": "Display Group Statistics",
+    }
+
+    columns = performance_report_data["columns"]
+    investments = performance_report_data["investments"]
+    benchmarks = performance_report_data["benchmarks"]
+    groups_data = performance_report_data["groups"]
+    peer_groups = performance_report_data["peerGroups"]
+    ranks = performance_report_data["ranks"]
+    summary_statistics = performance_report_data["summaryStatistics"]
+
+    all_data_row = []
+    new_columns = _get_all_columns(columns)
+    new_columns_name = _get_all_columns_name(new_columns)
+
+    get_by_type = lambda group: group["type"] == "Group"
+    new_groups = list(filter(get_by_type, groups_data))
+    groups_group = _filter_grouy_by_type(groups_data, "Group")
+    for group in new_groups:
+        group_id = group["id"]
+        group_name = group["name"]
+        sub_groups = _get_sub_group(groups_data, group_id)
+        group_investments = _filter_datas_by_group_id(investments, group_id)
+        group_benchmarks = _filter_datas_by_group_id(benchmarks, group_id)
+        group_peer_groups = _filter_datas_by_group_id(peer_groups, group_id)
+        group_ranks = _filter_datas_by_group_id(ranks, group_id)
+        peer_group_name = _get_peer_group_name_by_group_id(group_peer_groups)
+        all_data_row.extend(
+            _get_data_rows(
+                group_investments,
+                groups_group,
+                new_columns,
+                "investments",
+                peer_group_name,
+            )
+        )
+        all_data_row.extend(_get_data_rows(group_benchmarks, groups_group, new_columns, "Display Benchmark", ""))
+        all_data_row.extend(_get_group_data_rows(group_peer_groups, groups_group, new_columns, "PeerGroup", group_name))
+        all_data_row.extend(_get_group_data_rows(group_ranks, groups_group, new_columns, "Ranks", group_name))
+
+        for key in sub_groups:
+            subtype = sub_groups[key]["type"]
+
+            if subtype in subtype_name:
+                sub_peer_groups = _filter_datas_by_group_id(summary_statistics, sub_groups[key]["id"])
+                all_data_row.extend(
+                    _get_group_data_rows(
+                        sub_peer_groups,
+                        sub_peer_groups,
+                        new_columns,
+                        subtype_name[subtype],
+                        group_name,
+                    )
+                )
+
+    lssilss = _filter_datas_by_group_id(summary_statistics, "lssilss")
+    if lssilss:
+        all_data_row.extend(_get_group_data_rows(lssilss, lssilss, new_columns, "List Summary Statistics", ""))
+
+    data_frame = DataFrame(all_data_row)
+    data_frame.columns = new_columns_name
+    return data_frame
+
+
+@_decorator.not_null
+@_decorator.typechecked
+def calculate_report(report_id: str) -> DataFrame:
+    """Initiates re-calculation of a performance report.
+
+    Args:
+        report_id (:obj:`str`): Unique identifier of a saved performance report from the Performance Reporting
+            module in Morningstar Direct, e.g., "7782164". Use `get_reports <#morningstar_data.direct.get_reports>`_ to discover possible values.
+
+    Returns:
+        DataFrame: A DataFrame object confirming that report calculation was triggered. DataFrame columns include:
+
+         * reportId
+         * success
+
+    Raises:
+        ValueErrorException: Raised when the `report_id` parameter is invalid.
+
+    Examples:
+        Calculate the performance report.
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.performance_report.calculate_report(report_id="7128568") # Replace with a valid report ID
+        df
+
+    :Output:
+        ========  =======
+        reportId  success
+        ========  =======
+        7128568   True
+        ========  =======
+
+    Errors:
+        AccessDeniedError: Raised when the user is not authenticated.
+
+        ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+        BadRequestError: Raised when the user does not provide a properly formatted request.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+    """
+    df = get_report_status(report_id)
+    if df["status"].values[0] == "Ready" or df["status"].values[0] == "Failed":
+        url = f"{_config.performancereport_service_url()}v1/reports/calc/{report_id}"
+        response_json = _performance_report_api_request.do_post_request(url)
+        return DataFrame(response_json)
+    else:
+        raise ValueErrorException(f"report {report_id} is calculating.")
+
+
+@_decorator.not_null
+@_decorator.typechecked
+def get_report_status(report_id: str) -> DataFrame:
+    """Returns the current calculation status of the specified performance report. Possible statuses are:
+
+    * Failed
+    * Queued
+    * Calculating
+    * Generating Report
+    * Merging Excel
+    * Downloading
+    * Ready
+
+    Args:
+        report_id (:obj:`str`): Unique identifier of a saved performance report from the Performance Reporting
+            module in Morningstar Direct, e.g., "7782164". Use `get_reports <#morningstar_data.direct.get_reports>`_ to discover possible values.
+
+    Returns:
+        DataFrame: A DataFrame object with calculation status. DataFrame columns include:
+
+        * reportId
+        * status
+
+    Examples:
+        Get performance report calculation status.
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.performance_report.get_report_status(report_id="2463866") # Replace with a valid report ID
+        df
+
+    :Output:
+        ========  ======
+        reportId  status
+        ========  ======
+        2463866   Ready
+        ========  ======
+
+    Errors:
+        AccessDeniedError: Raised when the user is not authenticated.
+
+        ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+        BadRequestError: Raised when the user does not provide a properly formatted request.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+    """
+    url = f"{_config.performancereport_service_url()}v1/reports/status/{report_id}"
+    response_json = _performance_report_api_request.do_get_request(url)
+    return DataFrame(response_json)
+
+
+@_decorator.not_null
+@_decorator.typechecked
+def export_to_excel(report_id: str, file_name: Optional[str] = None) -> str:
+    """Export a performance report to Excel.
+
+    Args:
+        report_id (:obj:`str`): Unique identifier of a saved performance report from the Performance Reporting
+            module in Morningstar Direct, e.g., "7782164". Use `get_reports <#morningstar_data.direct.get_reports>`_ to discover possible values.
+        file_name (:obj:`str`, `optional`): Custom file name for the exported Excel file. If not provided, a default name with the format "report_<report_id>" will be used, e.g., "report_7782164.xlsx".
+
+    Returns:
+        str: Excel file name of the exported performance report.
+
+
+    Examples:
+        Export the given performance report.
+
+    ::
+
+        import morningstar_data as md
+
+        resp = md.direct.performance_report.export_to_excel(report_id="2442678") # Replace with a valid report ID
+        resp
+
+    :Output:
+        report_2442678.xlsx
+
+
+    Errors:
+        AccessDeniedError: Raised when the user is not authenticated.
+
+        ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+        BadRequestError: Raised when the user does not provide a properly formatted request.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
+
+    """
+    report_id_parse = quote(report_id, "utf-8")
+    url = f"{_config.performancereport_export_service_url()}v1/reports/export/{report_id_parse}"
+    presigned_url_response = _performance_report_api_request.do_get_request(url=url)
+
+    current_date_time = datetime.now().strftime("%Y%m%d_%H%M%S")
+    excel_file_suffix = ".xlsx"
+    if file_name is None or file_name == "":
+        file_name = f"performance_report_{report_id}_{current_date_time}.xlsx"
+    elif not file_name.endswith(excel_file_suffix):
+        file_name = file_name + excel_file_suffix
+    try:
+        url = presigned_url_response["url"]
+        response = requests.get(url, stream=True)
+        response.raise_for_status()
+        with open(file_name, "wb") as excel_file:
+            response.raw.decode_content = True
+            shutil.copyfileobj(response.raw, excel_file)
+        return file_name
+    # Catching HTTPErrors as this is presigned URL from bucket no do_get_request is used
+    except requests.ConnectionError as e:
+        _logger.error(e)
+        raise NetworkExceptionError from None
+    except requests.HTTPError as e:
+        _performance_report_api_request._handle_custom_http_errors(response)
+        _performance_report_api_request._handle_default_http_errors(response)
+        raise e
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/portfolio.py` & `morningstar_data-1.3.0/morningstar_data/direct/portfolio.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,852 +1,852 @@
-import simplejson as json
-import time
-import pandas as pd
-import warnings
-import requests
-from pandas import DataFrame
-from typing import Optional, List, Dict, Any, Union
-
-from ._investment._normal_data import _parse_raw_normal_data_values
-from ._utils import _get_iso_today
-from . import _decorator
-from .._base import _logger
-from ._exceptions import BadRequestException, ValueErrorException, ResourceNotFoundError
-from . import _error_messages
-from ._portfolio_data_set import (
-    _get_data_sets,
-    _get_data_set_with_id,
-    PortfolioDataSet,
-    _get_data_points_default_settings,
-    DataSetType,
-)
-
-from ._config import _Config
-from ._data_objects._data_points_object import DataPoints
-from ._data_type import ErrorMessages
-from .user_items.portfolio import get_portfolios, PortfolioDataApiBackend
-
-
-_config = _Config()
-_portfolio_api = PortfolioDataApiBackend()
-
-
-@_decorator.error_handler
-@_decorator.typechecked
-def get_data_sets() -> DataFrame:
-    """Returns all Morningstar-created portfolio data sets.
-
-    Returns:
-        DataFrame: A DataFrame object with data sets. DataFrame columns include:
-
-        * data_set_id
-        * name
-
-    :Examples:
-        Get all portfolio data sets.
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.portfolio.get_data_sets()
-        df
-
-    :Output:
-        ===========    ===============
-        data_set_id	   name
-        ===========    ===============
-        1              Snapshot
-        2              Returns (Daily)
-        ===========    ===============
-
-    """
-    all_view_df = pd.DataFrame({"data_set_id": [], "name": []})
-    df = _get_data_sets()
-    df = df.sort_values(by=["id"])
-    all_view_df["data_set_id"] = df["id"].astype(str)
-    all_view_df["name"] = df["name"]
-    all_view_df = all_view_df.reset_index(drop=True)
-    return all_view_df
-
-
-@_decorator.typechecked
-def get_data_set_data_points(data_set_id: str) -> DataFrame:
-    """Returns all data points for the given portfolio data set ID.
-
-    Args:
-        data_set_id (:obj:`str`): The unique identifier of a portfolio data set, e.g., '1'.
-
-    Returns:
-        DataFrame: A DataFrame object with data points. DataFrame columns include:
-
-        * data_point_id
-        * name
-
-    Examples:
-        Get data points by data set ID.
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.portfolio.get_data_set_data_points(data_set_id="1")
-        df
-
-    :Output:
-
-        ==============   ===============
-        data_point_id    name
-        ==============   ===============
-        OS01W		     Name
-        LS05M		     Base Currency
-        ...              ...
-        ==============   ===============
-
-    Errors:
-        AccessDeniedError: Raised when the user is not authenticated.
-
-        BadRequestError: Raised when the user does not provide a properly formatted request.
-
-        ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
-
-    """
-    view = _get_data_set_with_id(data_set_id)
-    data_points = pd.DataFrame(view["datapoints"])
-    if len(data_points):
-        data_points = data_points[["datapointId", "alias"]]
-        data_points = data_points.rename(columns={"alias": "name"})
-        data_points = data_points.rename(columns={"datapointId": "data_point_id"})
-        return data_points
-    else:
-        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_DATA_SET_DATA_POINT) from None
-
-
-def _get_data_points_by_view_id(id: str, currency: Optional[str]) -> List[Dict[Any, Any]]:
-    view = _get_data_set_with_id(id)
-    return _set_currency(view["datapoints"], currency)
-
-
-def _set_currency(data_points: List[Dict], currency: Optional[str]) -> List[Dict[Any, Any]]:
-    if currency is not None:
-        for data_point in data_points:
-            if data_point.get("currency") is not None:
-                data_point["currency"] = currency
-    return data_points
-
-
-@_decorator.not_null
-@_decorator.typechecked
-def get(portfolio_type: Optional[str] = None) -> DataFrame:
-    warnings.warn(
-        "The portfolio.get function is deprecated and will be removed in the next major version. Use user_items.get_portfolios instead",
-        FutureWarning,
-        stacklevel=2,
-    )
-    return get_portfolios(portfolio_type=portfolio_type)
-
-
-@_decorator.typechecked
-def get_holdings(
-    portfolio_ids: List[str],
-    date: Optional[str] = None,
-    start_date: Optional[str] = None,
-    end_date: Optional[str] = None,
-) -> DataFrame:
-    """Returns holdings for the given portfolio and date range.
-
-    Args:
-        portfolio_ids (:obj:`list`): List of portfolio IDs. The maximum number is 5. Use the `get_portfolios <./portfolio_list.html#morningstar_data.direct.user_items.get_portfolios>`_ function to discover saved portfolios.
-        date (:obj:`str`, `optional`): Holdings date. When this value is provided, `start_date` and `end_date` parameters are ignored. Use the `get_holding_dates <#morningstar_data.direct.portfolio.get_holding_dates>`_ function to discover available holding dates.
-        start_date (:obj:`str`, `optional`): Start date of the date range.
-        end_date (:obj:`str`, `optional`): End date of the date range.
-
-    Returns:
-        DataFrame: A DataFrame object with portfolio holdings data. DataFrame columns include:
-
-        * ObjectId
-        * Portfolio Date
-        * HoldingId
-        * Weight
-        * Name
-        * Currency
-        * ISIN
-        * Ticker
-
-    Examples:
-        Get holdings by portfolio ID and date.
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.portfolio.get_holdings(
-            portfolio_ids=['de21828b-91b7-4fe1-b66e-760fd5e657bc;BM'], # Replace with valid portfolio ID
-            date = "2017-09-30")
-        df
-
-    :Output:
-        =======================================   ==============   ==============   =======   =================================   ============   ============   ==========
-        ObjectId                                  Portfolio Date   HoldingId	    Weight	  Name                                Currency       ISIN           Ticker
-        =======================================   ==============   ==============   =======   =================================   ============   ============   ==========
-        de21828b-91b7-4fe1-b66e-760fd5e657bc;BM   2017-09-30	   FOUSA00DFS;F     100	      BlackRock Global Allocation Inv A	  USD	         US09251T1034   MDLOX
-        ...
-        =======================================   ==============   ==============   =======   =================================   ============   ============   ==========
-
-    Errors:
-        AccessDeniedError: Raised when the user is not authenticated.
-
-        BadRequestError: Raised when the user does not provide a properly formatted request.
-
-        ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
-
-    """
-    if not portfolio_ids:
-        raise BadRequestException("Please input portfolio_ids to proceed with your query.")
-    combined_holdings = pd.DataFrame(
-        {
-            "ObjectId": [],
-            "Portfolio Date": [],
-            "HoldingId": [],
-            "Weight": [],
-            "Name": [],
-            "Currency": [],
-            "ISIN": [],
-            "Ticker": [],
-        }
-    )
-    if portfolio_ids:
-        if len(portfolio_ids) > 5:
-            raise BadRequestException("The number of portfolio_ids per query are limited to 5.")
-        portfolio_available_dates = _get_dates(portfolio_ids, date, start_date, end_date)
-        if not portfolio_available_dates and date is not None and len(date.strip()) > 0:
-            portfolio_available_dates = {x: [date] for x in portfolio_ids}
-        _check_volume(portfolio_available_dates)
-        holdings_df = _get_holdings(portfolio_available_dates)
-        combined_holdings = pd.concat([combined_holdings, holdings_df])
-
-    if combined_holdings.empty:
-        if len(portfolio_ids) == 1:
-            raise ResourceNotFoundError((_error_messages.RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_HOLDING).format(portfolio_ids)) from None
-        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_HOLDINGS) from None
-    else:
-        combined_holdings = combined_holdings.where(combined_holdings.notnull(), None)
-        combined_holdings.reset_index(drop=True, inplace=True)
-    return combined_holdings
-
-
-def _get_holdings(portfolio_available_dates: dict) -> DataFrame:
-    holdings_list = []
-    for portfolio_id, dates in portfolio_available_dates.items():
-        for date in dates:
-            holdings = _get_holdings_by_id(portfolio_id, date)
-            holdings = holdings if holdings else []
-            holdings_list.extend(
-                [
-                    {
-                        "ObjectId": portfolio_id,
-                        "Portfolio Date": date,
-                        "HoldingId": x.get("id", None),
-                        "Weight": x.get("weight", None),
-                        "Name": x.get("name", None),
-                        "Currency": x.get("currency", None),
-                        "ISIN": x.get("isin", None),
-                        "Ticker": x.get("ticker", None),
-                    }
-                    for x in holdings
-                ]
-            )
-    return DataFrame(holdings_list)
-
-
-def _check_volume(portfolio_available_dates: dict) -> None:
-    if portfolio_available_dates:
-        total = 0
-        for dates in portfolio_available_dates.values():
-            total += len(dates) if dates is not None and isinstance(dates, list) else 0
-        if total > 10:
-            raise ValueErrorException("Please reduce the number of investments or shorten the query time period to proceed your query without interfering by too large data size.")
-
-
-def _get_holdings_by_id(portfolio_id: str, date: str) -> list:
-    try:
-        url = f"{_config.portfolio_service_url()}/portfoliodataservice/v1/portfolios/{portfolio_id}/holdings-summary?portfolioDate={date}"
-        response_json: list = _portfolio_api.do_get_request(url)
-        return response_json
-    except Exception as portfolio_error:
-        if portfolio_error.__class__.__name__ != "ResourceNotFoundError":
-            raise portfolio_error from None
-        pass
-    return []
-
-
-def _get_dates(
-    portfolio_ids: list,
-    date: Optional[str],
-    start_date: Optional[str],
-    end_date: Optional[str],
-) -> dict:
-    if date is not None and len(date.strip()) > 0:
-        date = _format_date(date)
-    elif start_date is not None and len(start_date.strip()) > 0:
-        start_date = _format_date(start_date)
-        if end_date is None or len(end_date.strip()) == 0:
-            end_date = _get_iso_today()
-        end_date = _format_date(end_date)
-    elif end_date is not None and len(end_date.strip()) > 0:
-        raise BadRequestException("Please specify a portfolio_date or time period to proceed with your query.")
-
-    response_json = _get_multi_portfolio_dates(portfolio_ids)
-
-    if date is not None and len(date.strip()) > 0:
-        return _handle_single_date(response_json, date)
-    elif start_date is not None and len(start_date.strip()) > 0 and end_date is not None and len(end_date.strip()) > 0:
-        return _handle_date_range(response_json, start_date, end_date)
-    else:
-        return _handle_no_date(response_json)
-
-
-def _get_multi_portfolio_dates(portfolio_ids: list) -> dict:
-    portfolio_date_dict = dict()
-    for id in portfolio_ids:
-        if id:
-            portfolio_date_dict[id] = _get_holding_dates(id)
-    return portfolio_date_dict
-
-
-def _handle_single_date(portfolio_dates: dict, input_portfolio_date: str) -> dict:
-    portfolio_available_dates = dict()
-    for portfolio_id, dates in portfolio_dates.items():
-        available_date = _get_available_date(input_portfolio_date, dates)
-        if available_date is not None:
-            portfolio_available_dates[portfolio_id] = [available_date]
-    return portfolio_available_dates
-
-
-def _get_available_date(target_date: str, dates: list) -> Optional[str]:
-    dates = dates if dates else []
-    if target_date in dates:
-        return target_date
-
-    available_date = None
-    dates.sort()
-    dates.reverse()
-    for date in dates:
-        if date < target_date:
-            available_date = date
-            break
-    return available_date
-
-
-def _handle_no_date(portfolio_dates: dict) -> dict:
-    portfolio_available_dates = dict()
-    for portfolio_id, dates in portfolio_dates.items():
-        dates = dates if dates else []
-        date = next((x for x in dates if x is not None and len(x.strip()) > 0), None)
-        if date is not None and len(date) > 0:
-            portfolio_available_dates[portfolio_id] = [date]
-    return portfolio_available_dates
-
-
-def _handle_date_range(portfolio_dates: dict, start_date: str, end_date: str) -> dict:
-    portfolio_available_dates = dict()
-    for portfolio_id, dates in portfolio_dates.items():
-        available_dates = list()
-        dates = dates if dates else []
-        for date in dates:
-            if start_date <= date <= end_date:
-                available_dates.append(date)
-        if available_dates:
-            portfolio_available_dates[portfolio_id] = available_dates
-
-    return portfolio_available_dates
-
-
-@_decorator.typechecked
-def get_holding_dates(portfolio_ids: Optional[Union[List[str], str]] = None) -> DataFrame:
-    """Returns portfolio holdings dates for the given portfolios.
-
-
-    Args:
-        portfolio_ids (:obj:`list`, `optional`): A portfolio ID or list of portfolio IDs. If no ID is specified, the function will return data for all portfolios saved in the user's account. Use the `get_portfolios <./portfolio_list.html#morningstar_data.direct.user_items.get_portfolios>`_ function to discover saved portfolios.
-
-    Returns:
-        DataFrame: A DataFrame object with all portfolio holdings dates. DataFrame columns include:
-
-        * portfolioId
-        * date
-
-    Examples:
-        Get portfolio holdings dates for the given portfolio ID.
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.portfolio.get_holding_dates(
-            portfolio_ids=['07c317df-a4a7-4297-afc3-0c18bb79a672;UA']) # Replace with a valid portfolio ID
-        df
-
-    :Output:
-        =======================================        ==========
-        PortfolioId                                    Date
-        =======================================        ==========
-        07c317df-a4a7-4297-afc3-0c18bb79a672;UA        2021-10-01
-        07c317df-a4a7-4297-afc3-0c18bb79a672;UA        2021-09-01
-        ...
-        =======================================        ==========
-
-    Errors:
-        AccessDeniedError: Raised when the user is not authenticated.
-
-        BadRequestError: Raised when the user does not provide a properly formatted request.
-
-        ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
-
-    """
-    if not isinstance(portfolio_ids, list) and portfolio_ids is not None:
-        single_id = portfolio_ids
-        portfolio_ids = list()
-        portfolio_ids.append(single_id)
-    portfolio_date_list = list()
-    if not portfolio_ids:
-        portfolio_df = get()
-        portfolio_ids = list(portfolio_df["PortfolioId"])
-    for portfolio_id in sorted(set(portfolio_ids), key=portfolio_ids.index):
-        if portfolio_id is None or len(portfolio_id.strip()) == 0:
-            continue
-        dates = _get_holding_dates(portfolio_id, portfolio_ids)
-        if not dates:
-            continue
-        portfolio_date_list.extend([{"PortfolioId": portfolio_id, "Date": date} for date in dates])
-    portfolio_df = DataFrame(portfolio_date_list)
-    if portfolio_df.empty:
-        if len(portfolio_ids) == 1:
-            raise ResourceNotFoundError((_error_messages.RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_ID).format(portfolio_id)) from None
-        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_IDS) from None
-    return portfolio_df
-
-
-def _get_holding_dates(portfolio_id: str, portfolio_ids: Optional[Union[List[str], str]] = None) -> list:
-    try:
-        url = f"{_config.portfolio_service_url()}/portfoliodataservice/v1/portfolios/{portfolio_id}/dates"
-        response_json: Dict[str, list] = _portfolio_api.do_get_request(url)
-        return response_json["dates"]
-    except Exception as portfolio_error:
-        if portfolio_error.__class__.__name__ != "ResourceNotFoundError":
-            raise portfolio_error from None
-        pass
-    return []
-
-
-def _format_date(date: str) -> str:
-    try:
-        return time.strftime("%Y-%m-%d", time.strptime(date, "%Y-%m-%d"))
-    except Exception as e:
-        # _logger.error(f"Date format error: {e}")
-        raise BadRequestException(ErrorMessages.date_format_error.value + f" Date format error: {e}.") from None
-
-
-@_decorator.typechecked
-def get_data(
-    portfolio_id: str,
-    data_set_id: Optional[Union[str, PortfolioDataSet, None]] = None,
-    currency: Optional[str] = None,
-    start_date: Optional[str] = None,
-    end_date: Optional[str] = None,
-    data_point_settings: Optional[DataFrame] = None,
-) -> DataFrame:
-    """Returns data for the given portfolio and data points.
-
-    Args:
-        portfolio_id (:obj:`str` ): Portfolio ID. Use the `get_portfolios <./portfolio_list.html#morningstar_data.direct.user_items.get_portfolios>`_ function to discover saved portfolios.
-        data_set_id (:obj:`str`, `optional`): Saved portfolio data set, e.g., "1". Use the `get_data_sets <./data_set.html#morningstar_data.direct.portfolio.get_data_sets>`_ function to discover available data sets.
-        currency (:obj:`str`, `optional`): Currency setting for the data point values, when applicable. Use the `currency_codes <../morningstar_data/lookup.html#morningstar_data.lookup.currency_codes>`_ function to discover available currency codes.
-        start_date (:obj:`str`, `optional`): Start date of a date range for retrieving data.
-            The format is YYYY-MM-DD, e.g., '2020-01-01'.
-        end_date (:obj:`str`, `optional`): End date of a date range for retrieving data. If no value is provided for `end_date`, current date will be used.
-            The format is YYYY-MM-DD, e.g., '2020-01-01'.
-        data_point_settings (:obj:`DataFrame`, `optional`): A DataFrame of data points with all defined settings. Each row represents a data point.
-            Each column is a configurable setting. Users can get this DataFrame by using `get_data_set_data_points <./data_set.html#morningstar_data.direct.portfolio.get_data_set_data_points>`_ or `get_data_point_settings <../morningstar_data/lookup.html#morningstar_data.direct.get_data_point_settings>`_ for a given data point ID(s).
-            Users can update setting values in this DataFrame if desired. Additionally, the priority of currency/start_date/end_date in `data_point_settings`
-            is lower than the currency/start_date/end_date function parameters.
-
-
-    Returns:
-        DataFrame: A DataFrame object with portfolio data.
-
-    Examples:
-        Get portfolio data for the given portfolio and data set.
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.portfolio.get_data(
-            portfolio_id="8c6de08f-a668-4e78-a688-3d809aeb29b7;UA", # Replace with a valid portfolio ID
-            data_set_id="1")
-        df
-
-    :Output:
-        =========================================  =====   ==============   ================   =====   =================================   ==================================
-        Id                                         Name    Base Currency    Portfolio Date     ...     Total Ret Annlzd 10 Yr (Year-End)   Total Ret Annlzd 15 Yr (Year-End)
-        =========================================  =====   ==============   ================   =====   =================================   ==================================
-        8c6de08f-a668-4e78-a688-3d809aeb29b7;UA    test1   US Dollar        2022-02-28         ...     None                                None
-        ...
-        =========================================  =====   ==============   ================   =====   =================================   ==================================
-
-    Errors:
-        AccessDeniedError: Raised when the user is not authenticated.
-
-        BadRequestError: Raised when the user does not provide a properly formatted request.
-
-        ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
-
-    """
-    all_data = _get_portfolio_data(
-        portfolio_id=portfolio_id,
-        data_set_id=data_set_id,
-        currency=currency,
-        start_date=start_date,
-        end_date=end_date,
-        data_point_settings=data_point_settings,
-    )
-    col_name = all_data.columns.tolist()
-    all_data = all_data.reindex(columns=col_name)
-    return all_data
-
-
-def _get_portfolio_data(
-    portfolio_id: str,
-    data_set_id: Optional[Union[str, PortfolioDataSet, None]] = None,
-    currency: Optional[str] = None,
-    start_date: Optional[str] = None,
-    end_date: Optional[str] = None,
-    data_point_settings: Optional[DataFrame] = None,
-) -> DataFrame:
-    """
-    As the "get_portfolio_data" API may been called by other APIs, so we extracted it as a private method.
-    """
-    # try:
-    # build columns
-    settings_data_frame = None
-    if data_point_settings is not None and not data_point_settings.empty:
-        settings_data_frame = _get_data_settings_data_points(data_point_settings, currency, start_date, end_date)
-    else:
-        if isinstance(data_set_id, PortfolioDataSet):
-            data_set_id = data_set_id.data_set_id
-            if get_data_set_data_points(data_set_id=data_set_id).empty:
-                raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_DATA_SET_DATA_POINT) from None
-        if not data_set_id:
-            raise BadRequestException("Please specify either data_set_id or data_point_settings to proceed with your query.")
-        settings_data_frame = DataFrame(_get_data_set_data_points(data_set_id, currency, start_date, end_date))
-    portfolio_ids = [portfolio_id]
-
-    settings_data_frame = settings_data_frame.where(settings_data_frame.notnull(), None)
-
-    # get data
-    raw_data = _get_normal_data(
-        portfolio_ids,
-        _filter_disable_data_points(settings_data_frame).to_dict(orient="records"),
-    )
-
-    investment_results = _parse_raw_normal_data_values(raw_data)
-
-    # add id
-    all_data = investment_results.as_data_frame()
-    col_name = all_data.columns.tolist()
-    all_data = all_data.reindex(columns=col_name)
-
-    return all_data
-
-
-def _filter_disable_data_points(data_point_settings: DataFrame = None) -> DataFrame:
-    columns = data_point_settings.columns
-    if "disable" in columns:
-        return data_point_settings.loc[data_point_settings["disable"] != True]
-    return data_point_settings
-
-
-def _get_normal_data(portfolio_ids: list, data_points: list) -> DataFrame:
-    if not portfolio_ids:
-        raise BadRequestException("There is no portfolio data returned.")
-    postbody = {
-        "datapoints": data_points,
-        "investments": list(map(lambda x: {"id": x}, portfolio_ids)),
-    }
-    resp: DataFrame = _request_porfolio_data(postbody, portfolio_ids)
-    if resp is None:
-        raise BadRequestException("There is no return data available.")
-    return resp
-
-
-def _request_porfolio_data(postbody: dict, portfolio_ids: list) -> DataFrame:
-    job_detail, portfolio_data = _get_portfolio_job(postbody)
-    job_id = job_detail["id"]
-    try_times = 10
-    while True:
-        job_detail, portfolio_data = _get_portfolio_job(postbody, job_id)
-        time.sleep(2)
-        try_times = try_times - 1
-        if job_detail.get("percentage", "0") == "100" or try_times == 0:
-            break
-    if not portfolio_data:
-        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_GET_DATA_RETURN.format(portfolio_ids[0]))
-    return portfolio_data
-
-
-def _get_portfolio_job(postbody: dict, job_id: Optional[str] = None) -> tuple:
-    url = f"{_config.portfolio_service_url()}/portfoliodataservice/v1/portfolios/calculation?maxExecTime=600000&maxWaitTime=600000&timeOut=600000"
-    if job_id:
-        url = url + f"&jobId={job_id}"
-    response_json = _portfolio_api.do_post_request(url, json.dumps(postbody, ignore_nan=True).replace("NaN", "null"))
-    job_detail = response_json["job"]
-    portfolio_data = None
-
-    if job_detail.get("percentage", "0") == "100":
-        portfolio_data = response_json
-    return job_detail, portfolio_data
-
-
-def _get_data_settings_data_points(
-    data_point_settings: DataFrame,
-    currency: Optional[str],
-    start_date: Optional[str],
-    end_date: Optional[str],
-) -> DataFrame:
-    if "datapointId" not in data_point_settings.columns:
-        raise BadRequestException("Please input valid data_point_settings to proceed with your query.")
-    data_point_settings = data_point_settings.where(data_point_settings.notnull(), None)
-    start_date, end_date = _format_start_end_date(start_date, end_date)
-    # only set currency to the data_points with currency.
-    # only set start_date/end_date to the datapoints without isTsdp=False.
-
-    data_point_default_settings = _get_data_points_default_settings(data_point_settings["datapointId"].tolist())
-
-    settings_list = data_point_settings.to_dict(orient="records")
-    for settings in settings_list:
-        data_point_id = settings["datapointId"]
-        defined_data_point = data_point_default_settings.get(data_point_id)
-        if defined_data_point is not None and defined_data_point.get("currency") is None:
-            settings["currency"] = None
-        elif currency is not None and len(currency.strip()) > 0:
-            settings["currency"] = currency
-        if defined_data_point is not None and defined_data_point.get("isTsdp") is not None and settings.get("isTsdp") is None:
-            settings["isTsdp"] = defined_data_point.get("isTsdp")
-
-        if settings.get("isTsdp") is not False and start_date is not None and len(start_date.strip()) > 0 and end_date is not None and len(end_date.strip()) > 0:
-            settings["startDate"] = start_date
-            settings["endDate"] = end_date
-
-        esg_data_point = data_point_default_settings.get(data_point_id)
-        if data_point_id != "OS01W" and esg_data_point is not None and settings.get("isTsdp") is None:
-            if esg_data_point.get("isTsdp") is not None:
-                settings["isTsdp"] = esg_data_point.get("isTsdp")
-            else:
-                start = settings.get("startDate")
-                end = settings.get("endDate")
-                if start is not None and len(start.strip()) > 0 and end is not None and len(end.strip()) > 0:
-                    settings["isTsdp"] = True
-                else:
-                    settings["isTsdp"] = False
-    data_point_settings = DataFrame(settings_list)
-    data_point_settings = data_point_settings.where(data_point_settings.notnull(), None)
-    data_points = DataPoints(data_point_settings)
-    settings_data_frame = DataFrame(data_points.get_data_points().to_dict(orient="records"))
-    settings_data_frame = _disable_data_points(settings_data_frame, data_point_default_settings)
-
-    return settings_data_frame
-
-
-def _disable_data_points(settings_data_frame: DataFrame, defined_data_points: dict) -> DataFrame:
-    settings_list = settings_data_frame.to_dict(orient="records")
-    for settings in settings_list:
-        data_point_id = settings["datapointId"]
-        frequency_m_data_point = defined_data_points.get(data_point_id)
-        if frequency_m_data_point is not None:
-            frequency = settings.get("frequency")
-            defined_freq = frequency_m_data_point.get("frequency", None)
-            if defined_freq is not None and frequency is not None and len(frequency.strip()) > 0 and frequency != defined_freq:
-                settings["disable"] = True
-
-        defined_data_point = defined_data_points.get(data_point_id)
-        # for defined datapoint with isTsdp = False
-        if defined_data_point is not None:
-            if defined_data_point.get("isTsdp") is False and settings.get("isTsdp") is True:
-                settings["disable"] = True
-            if defined_data_point.get("isTsdp") is True and settings.get("isTsdp") is False:
-                settings["disable"] = True
-    settings_data_frame = DataFrame(settings_list)
-    settings_data_frame = settings_data_frame.where(settings_data_frame.notnull(), None)
-    return settings_data_frame
-
-
-def _get_data_set_data_points(
-    data_set_id: str,
-    currency: Optional[str],
-    start_date: Optional[str],
-    end_date: Optional[str],
-) -> list:
-    data_point_ids = _get_data_points_by_view_id(data_set_id, currency)
-    data_points = DataPoints(data_point_ids)
-    if not data_point_ids:
-        return list(data_points.get_data_points().to_dict(orient="records"))
-    data_set_type = PortfolioDataSet.get_data_set_type(data_set_id)
-    if data_set_type == DataSetType.TimeSeries:
-        if start_date is None or len(start_date.strip()) == 0:
-            raise BadRequestException(_error_messages.BAD_REQUEST_ERROR_NO_START_AND_END_DATE) from None
-        if end_date is None or len(end_date.strip()) == 0:
-            raise BadRequestException(_error_messages.BAD_REQUEST_ERROR_NO_END_DATE)
-        for data_point_id in data_point_ids:
-            if data_point_id.get("isTsdp") is True:
-                data_point_id["startDate"] = start_date
-                data_point_id["endDate"] = end_date
-
-    if data_set_type == DataSetType.Custom_Calculation:
-        start_date, end_date = _format_start_end_date(start_date, end_date)
-        if start_date is not None and len(start_date.strip()) > 0 and end_date is not None and len(end_date.strip()) > 0:
-            for data_point_id in data_point_ids:
-                data_point_id["startDate"] = start_date
-                data_point_id["endDate"] = end_date
-        return list(data_points.get_data_points().to_dict(orient="records"))
-
-    if data_set_type == DataSetType.Current_Or_TimeSeries:
-        start_date, end_date = _format_start_end_date(start_date, end_date)
-        for data_point_id in data_point_ids:
-            if data_point_id.get("isTsdp") is not False and start_date is not None and len(start_date.strip()) > 0 and end_date is not None and len(end_date.strip()) > 0:
-                data_point_id["startDate"] = start_date
-                data_point_id["endDate"] = end_date
-                data_point_id["isTsdp"] = True
-                # support 'm' only
-                data_point_id["frequency"] = "m"
-            else:
-                data_point_id["isTsdp"] = False
-        return list(data_points.get_data_points().to_dict(orient="records"))
-
-    return data_point_ids
-
-
-def _format_start_end_date(start_date: Optional[str], end_date: Optional[str]) -> tuple:
-    if start_date is not None and len(start_date.strip()) > 0:
-        start_date = _format_date(start_date)
-        if end_date is None or len(end_date.strip()) == 0:
-            raise BadRequestException(ErrorMessages.start_end_date_error.value)
-        end_date = _format_date(end_date)
-    elif end_date is not None and len(end_date.strip()) > 0:
-        raise BadRequestException(ErrorMessages.start_end_date_error.value)
-    return start_date, end_date
-
-
-@_decorator.typechecked
-def get_benchmark_settings(portfolio_id: str) -> DataFrame:
-    """
-    Returns a portfolio's benchmark settings.
-
-    Args:
-        portfolio_id (:obj:`str` ): Portfolio ID. Use the `get_portfolios <./portfolio_list.html#morningstar_data.direct.user_items.get_portfolios>`_ function to discover saved portfolios.
-
-    Returns:
-        DataFrame: A DataFrame object containing the portfolio settings.
-
-    :Examples:
-
-    Get portfolio settings for a custom model portfolio.
-    ::
-        import morningstar_data as md
-
-        df = md.direct.portfolio.get_settings(
-            portfolio_id="d38b96dd-fbe1-4750-b05d-fa7cf4b6e35a;MD") # Replace with a valid portfolio ID
-        df
-
-    :Output:
-
-        ========================================  ====================================  ====================================  ================  ======================  ==============  ================  ======================  =====================
-        Portfolio ID                              Risk Free Proxy ID                    Benchmark 1 ID                        Benchmark 1 Name  Benchmark 1 SecurityId  Benchmark 2 ID  Benchmark 2 Name  Benchmark 2 SecurityId  Internal Portfolio ID
-        ========================================  ====================================  ====================================  ================  ======================  ==============  ================  ======================  =====================
-        d38b96dd-fbe1-4750-b05d-fa7cf4b6e35a;MD   e9b23e21-9c6f-4696-9583-3b3729b4ad99  fcff80f8-2fbc-4211-bbce-45252008a9cc  S&P 500 TR USD    XIUSA04G92;XI           None            None              None                    None
-
-        ========================================  ====================================  ====================================  ================  ======================  ==============  ================  ======================  =====================
-
-    Errors:
-        AccessDeniedError: Raised when the user is not authenticated.
-
-        BadRequestError: Raised when the user does not provide a properly formatted request.
-
-        ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
-
-    """
-
-    _logger.info("Fetching portfolio settings by id")
-    portfolio_settings = _get_settings_by_id(portfolio_id=portfolio_id)
-    settings = {}
-    settings["Porfolio ID"] = portfolio_settings["portfolio"]["portfolioId"]
-    settings["Internal Portfolio ID"] = portfolio_settings["portfolio"]["portfolio2Id"]
-    settings["Risk Free Proxy ID"] = portfolio_settings["portfolio"]["riskFreeProxyId"]
-
-    primary_benchmark = portfolio_settings["portfolio"]["benchmarkId"]
-    secondary_benchmark = portfolio_settings["portfolio"]["secondaryBenchmarkId"]
-    # The secondary benchmark is optional so not all portfolios will have this information
-    secondary_benchmark_name = None
-    secondary_benchmark_id = None
-
-    for benchmark in portfolio_settings["benchmarks"]:
-        benchmark_id = benchmark["benchmarkId"]
-        if benchmark_id == primary_benchmark:
-            primary_benchmark_name = benchmark["name"]
-            primary_benchmark_sec_id = benchmark["securityId"]
-
-        elif benchmark_id == secondary_benchmark:
-            secondary_benchmark_name = benchmark["name"]
-            secondary_benchmark_id = benchmark["securityId"]
-
-    settings["Benchmark 1 ID"] = primary_benchmark
-    settings["Benchmark 1 Name"] = primary_benchmark_name
-    settings["Benchmark 1 Security ID"] = primary_benchmark_sec_id
-
-    settings["Benchmark 2 ID"] = secondary_benchmark
-    settings["Benchmark 2 Name"] = secondary_benchmark_name
-    settings["Benchmark 2 Security ID"] = secondary_benchmark_id
-
-    return DataFrame(settings, index=[0])
-
-
-def _get_settings_by_id(portfolio_id: str) -> dict:
-    try:
-        url = f"{_config.portfolio_service_url()}/portfoliodataservice/v1/portfolios/{portfolio_id}/settings"
-        response_json = _portfolio_api.do_get_request(url)
-        settings: dict = response_json["settings"]  # settings key is always present when 200 status code is returned.
-        return settings
-    except Exception as portfolio_error:
-        if portfolio_error.__class__.__name__ != "ResourceNotFoundError":
-            raise portfolio_error from None
-        pass
-    return {}
+import simplejson as json
+import time
+import pandas as pd
+import warnings
+import requests
+from pandas import DataFrame
+from typing import Optional, List, Dict, Any, Union
+
+from ._investment._normal_data import _parse_raw_normal_data_values
+from ._utils import _get_iso_today
+from . import _decorator
+from .._base import _logger
+from ._exceptions import BadRequestException, ValueErrorException, ResourceNotFoundError
+from . import _error_messages
+from ._portfolio_data_set import (
+    _get_data_sets,
+    _get_data_set_with_id,
+    PortfolioDataSet,
+    _get_data_points_default_settings,
+    DataSetType,
+)
+
+from ._config import _Config
+from ._data_objects._data_points_object import DataPoints
+from ._data_type import ErrorMessages
+from .user_items.portfolio import get_portfolios, PortfolioDataApiBackend
+
+
+_config = _Config()
+_portfolio_api = PortfolioDataApiBackend()
+
+
+@_decorator.error_handler
+@_decorator.typechecked
+def get_data_sets() -> DataFrame:
+    """Returns all Morningstar-created portfolio data sets.
+
+    Returns:
+        DataFrame: A DataFrame object with data sets. DataFrame columns include:
+
+        * data_set_id
+        * name
+
+    :Examples:
+        Get all portfolio data sets.
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.portfolio.get_data_sets()
+        df
+
+    :Output:
+        ===========    ===============
+        data_set_id	   name
+        ===========    ===============
+        1              Snapshot
+        2              Returns (Daily)
+        ===========    ===============
+
+    """
+    all_view_df = pd.DataFrame({"data_set_id": [], "name": []})
+    df = _get_data_sets()
+    df = df.sort_values(by=["id"])
+    all_view_df["data_set_id"] = df["id"].astype(str)
+    all_view_df["name"] = df["name"]
+    all_view_df = all_view_df.reset_index(drop=True)
+    return all_view_df
+
+
+@_decorator.typechecked
+def get_data_set_data_points(data_set_id: str) -> DataFrame:
+    """Returns all data points for the given portfolio data set ID.
+
+    Args:
+        data_set_id (:obj:`str`): The unique identifier of a portfolio data set, e.g., '1'.
+
+    Returns:
+        DataFrame: A DataFrame object with data points. DataFrame columns include:
+
+        * data_point_id
+        * name
+
+    Examples:
+        Get data points by data set ID.
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.portfolio.get_data_set_data_points(data_set_id="1")
+        df
+
+    :Output:
+
+        ==============   ===============
+        data_point_id    name
+        ==============   ===============
+        OS01W		     Name
+        LS05M		     Base Currency
+        ...              ...
+        ==============   ===============
+
+    Errors:
+        AccessDeniedError: Raised when the user is not authenticated.
+
+        BadRequestError: Raised when the user does not provide a properly formatted request.
+
+        ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
+
+    """
+    view = _get_data_set_with_id(data_set_id)
+    data_points = pd.DataFrame(view["datapoints"])
+    if len(data_points):
+        data_points = data_points[["datapointId", "alias"]]
+        data_points = data_points.rename(columns={"alias": "name"})
+        data_points = data_points.rename(columns={"datapointId": "data_point_id"})
+        return data_points
+    else:
+        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_DATA_SET_DATA_POINT) from None
+
+
+def _get_data_points_by_view_id(id: str, currency: Optional[str]) -> List[Dict[Any, Any]]:
+    view = _get_data_set_with_id(id)
+    return _set_currency(view["datapoints"], currency)
+
+
+def _set_currency(data_points: List[Dict], currency: Optional[str]) -> List[Dict[Any, Any]]:
+    if currency is not None:
+        for data_point in data_points:
+            if data_point.get("currency") is not None:
+                data_point["currency"] = currency
+    return data_points
+
+
+@_decorator.not_null
+@_decorator.typechecked
+def get(portfolio_type: Optional[str] = None) -> DataFrame:
+    warnings.warn(
+        "The portfolio.get function is deprecated and will be removed in the next major version. Use user_items.get_portfolios instead",
+        FutureWarning,
+        stacklevel=2,
+    )
+    return get_portfolios(portfolio_type=portfolio_type)
+
+
+@_decorator.typechecked
+def get_holdings(
+    portfolio_ids: List[str],
+    date: Optional[str] = None,
+    start_date: Optional[str] = None,
+    end_date: Optional[str] = None,
+) -> DataFrame:
+    """Returns holdings for the given portfolio and date range.
+
+    Args:
+        portfolio_ids (:obj:`list`): List of portfolio IDs. The maximum number is 5. Use the `get_portfolios <./portfolio_list.html#morningstar_data.direct.user_items.get_portfolios>`_ function to discover saved portfolios.
+        date (:obj:`str`, `optional`): Holdings date. When this value is provided, `start_date` and `end_date` parameters are ignored. Use the `get_holding_dates <#morningstar_data.direct.portfolio.get_holding_dates>`_ function to discover available holding dates.
+        start_date (:obj:`str`, `optional`): Start date of the date range.
+        end_date (:obj:`str`, `optional`): End date of the date range.
+
+    Returns:
+        DataFrame: A DataFrame object with portfolio holdings data. DataFrame columns include:
+
+        * ObjectId
+        * Portfolio Date
+        * HoldingId
+        * Weight
+        * Name
+        * Currency
+        * ISIN
+        * Ticker
+
+    Examples:
+        Get holdings by portfolio ID and date.
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.portfolio.get_holdings(
+            portfolio_ids=['de21828b-91b7-4fe1-b66e-760fd5e657bc;BM'], # Replace with valid portfolio ID
+            date = "2017-09-30")
+        df
+
+    :Output:
+        =======================================   ==============   ==============   =======   =================================   ============   ============   ==========
+        ObjectId                                  Portfolio Date   HoldingId	    Weight	  Name                                Currency       ISIN           Ticker
+        =======================================   ==============   ==============   =======   =================================   ============   ============   ==========
+        de21828b-91b7-4fe1-b66e-760fd5e657bc;BM   2017-09-30	   FOUSA00DFS;F     100	      BlackRock Global Allocation Inv A	  USD	         US09251T1034   MDLOX
+        ...
+        =======================================   ==============   ==============   =======   =================================   ============   ============   ==========
+
+    Errors:
+        AccessDeniedError: Raised when the user is not authenticated.
+
+        BadRequestError: Raised when the user does not provide a properly formatted request.
+
+        ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
+
+    """
+    if not portfolio_ids:
+        raise BadRequestException("Please input portfolio_ids to proceed with your query.")
+    combined_holdings = pd.DataFrame(
+        {
+            "ObjectId": [],
+            "Portfolio Date": [],
+            "HoldingId": [],
+            "Weight": [],
+            "Name": [],
+            "Currency": [],
+            "ISIN": [],
+            "Ticker": [],
+        }
+    )
+    if portfolio_ids:
+        if len(portfolio_ids) > 5:
+            raise BadRequestException("The number of portfolio_ids per query are limited to 5.")
+        portfolio_available_dates = _get_dates(portfolio_ids, date, start_date, end_date)
+        if not portfolio_available_dates and date is not None and len(date.strip()) > 0:
+            portfolio_available_dates = {x: [date] for x in portfolio_ids}
+        _check_volume(portfolio_available_dates)
+        holdings_df = _get_holdings(portfolio_available_dates)
+        combined_holdings = pd.concat([combined_holdings, holdings_df])
+
+    if combined_holdings.empty:
+        if len(portfolio_ids) == 1:
+            raise ResourceNotFoundError((_error_messages.RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_HOLDING).format(portfolio_ids)) from None
+        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_HOLDINGS) from None
+    else:
+        combined_holdings = combined_holdings.where(combined_holdings.notnull(), None)
+        combined_holdings.reset_index(drop=True, inplace=True)
+    return combined_holdings
+
+
+def _get_holdings(portfolio_available_dates: dict) -> DataFrame:
+    holdings_list = []
+    for portfolio_id, dates in portfolio_available_dates.items():
+        for date in dates:
+            holdings = _get_holdings_by_id(portfolio_id, date)
+            holdings = holdings if holdings else []
+            holdings_list.extend(
+                [
+                    {
+                        "ObjectId": portfolio_id,
+                        "Portfolio Date": date,
+                        "HoldingId": x.get("id", None),
+                        "Weight": x.get("weight", None),
+                        "Name": x.get("name", None),
+                        "Currency": x.get("currency", None),
+                        "ISIN": x.get("isin", None),
+                        "Ticker": x.get("ticker", None),
+                    }
+                    for x in holdings
+                ]
+            )
+    return DataFrame(holdings_list)
+
+
+def _check_volume(portfolio_available_dates: dict) -> None:
+    if portfolio_available_dates:
+        total = 0
+        for dates in portfolio_available_dates.values():
+            total += len(dates) if dates is not None and isinstance(dates, list) else 0
+        if total > 10:
+            raise ValueErrorException("Please reduce the number of investments or shorten the query time period to proceed your query without interfering by too large data size.")
+
+
+def _get_holdings_by_id(portfolio_id: str, date: str) -> list:
+    try:
+        url = f"{_config.portfolio_service_url()}/portfoliodataservice/v1/portfolios/{portfolio_id}/holdings-summary?portfolioDate={date}"
+        response_json: list = _portfolio_api.do_get_request(url)
+        return response_json
+    except Exception as portfolio_error:
+        if portfolio_error.__class__.__name__ != "ResourceNotFoundError":
+            raise portfolio_error from None
+        pass
+    return []
+
+
+def _get_dates(
+    portfolio_ids: list,
+    date: Optional[str],
+    start_date: Optional[str],
+    end_date: Optional[str],
+) -> dict:
+    if date is not None and len(date.strip()) > 0:
+        date = _format_date(date)
+    elif start_date is not None and len(start_date.strip()) > 0:
+        start_date = _format_date(start_date)
+        if end_date is None or len(end_date.strip()) == 0:
+            end_date = _get_iso_today()
+        end_date = _format_date(end_date)
+    elif end_date is not None and len(end_date.strip()) > 0:
+        raise BadRequestException("Please specify a portfolio_date or time period to proceed with your query.")
+
+    response_json = _get_multi_portfolio_dates(portfolio_ids)
+
+    if date is not None and len(date.strip()) > 0:
+        return _handle_single_date(response_json, date)
+    elif start_date is not None and len(start_date.strip()) > 0 and end_date is not None and len(end_date.strip()) > 0:
+        return _handle_date_range(response_json, start_date, end_date)
+    else:
+        return _handle_no_date(response_json)
+
+
+def _get_multi_portfolio_dates(portfolio_ids: list) -> dict:
+    portfolio_date_dict = dict()
+    for id in portfolio_ids:
+        if id:
+            portfolio_date_dict[id] = _get_holding_dates(id)
+    return portfolio_date_dict
+
+
+def _handle_single_date(portfolio_dates: dict, input_portfolio_date: str) -> dict:
+    portfolio_available_dates = dict()
+    for portfolio_id, dates in portfolio_dates.items():
+        available_date = _get_available_date(input_portfolio_date, dates)
+        if available_date is not None:
+            portfolio_available_dates[portfolio_id] = [available_date]
+    return portfolio_available_dates
+
+
+def _get_available_date(target_date: str, dates: list) -> Optional[str]:
+    dates = dates if dates else []
+    if target_date in dates:
+        return target_date
+
+    available_date = None
+    dates.sort()
+    dates.reverse()
+    for date in dates:
+        if date < target_date:
+            available_date = date
+            break
+    return available_date
+
+
+def _handle_no_date(portfolio_dates: dict) -> dict:
+    portfolio_available_dates = dict()
+    for portfolio_id, dates in portfolio_dates.items():
+        dates = dates if dates else []
+        date = next((x for x in dates if x is not None and len(x.strip()) > 0), None)
+        if date is not None and len(date) > 0:
+            portfolio_available_dates[portfolio_id] = [date]
+    return portfolio_available_dates
+
+
+def _handle_date_range(portfolio_dates: dict, start_date: str, end_date: str) -> dict:
+    portfolio_available_dates = dict()
+    for portfolio_id, dates in portfolio_dates.items():
+        available_dates = list()
+        dates = dates if dates else []
+        for date in dates:
+            if start_date <= date <= end_date:
+                available_dates.append(date)
+        if available_dates:
+            portfolio_available_dates[portfolio_id] = available_dates
+
+    return portfolio_available_dates
+
+
+@_decorator.typechecked
+def get_holding_dates(portfolio_ids: Optional[Union[List[str], str]] = None) -> DataFrame:
+    """Returns portfolio holdings dates for the given portfolios.
+
+
+    Args:
+        portfolio_ids (:obj:`list`, `optional`): A portfolio ID or list of portfolio IDs. If no ID is specified, the function will return data for all portfolios saved in the user's account. Use the `get_portfolios <./portfolio_list.html#morningstar_data.direct.user_items.get_portfolios>`_ function to discover saved portfolios.
+
+    Returns:
+        DataFrame: A DataFrame object with all portfolio holdings dates. DataFrame columns include:
+
+        * portfolioId
+        * date
+
+    Examples:
+        Get portfolio holdings dates for the given portfolio ID.
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.portfolio.get_holding_dates(
+            portfolio_ids=['07c317df-a4a7-4297-afc3-0c18bb79a672;UA']) # Replace with a valid portfolio ID
+        df
+
+    :Output:
+        =======================================        ==========
+        PortfolioId                                    Date
+        =======================================        ==========
+        07c317df-a4a7-4297-afc3-0c18bb79a672;UA        2021-10-01
+        07c317df-a4a7-4297-afc3-0c18bb79a672;UA        2021-09-01
+        ...
+        =======================================        ==========
+
+    Errors:
+        AccessDeniedError: Raised when the user is not authenticated.
+
+        BadRequestError: Raised when the user does not provide a properly formatted request.
+
+        ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
+
+    """
+    if not isinstance(portfolio_ids, list) and portfolio_ids is not None:
+        single_id = portfolio_ids
+        portfolio_ids = list()
+        portfolio_ids.append(single_id)
+    portfolio_date_list = list()
+    if not portfolio_ids:
+        portfolio_df = get()
+        portfolio_ids = list(portfolio_df["PortfolioId"])
+    for portfolio_id in sorted(set(portfolio_ids), key=portfolio_ids.index):
+        if portfolio_id is None or len(portfolio_id.strip()) == 0:
+            continue
+        dates = _get_holding_dates(portfolio_id, portfolio_ids)
+        if not dates:
+            continue
+        portfolio_date_list.extend([{"PortfolioId": portfolio_id, "Date": date} for date in dates])
+    portfolio_df = DataFrame(portfolio_date_list)
+    if portfolio_df.empty:
+        if len(portfolio_ids) == 1:
+            raise ResourceNotFoundError((_error_messages.RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_ID).format(portfolio_id)) from None
+        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_IDS) from None
+    return portfolio_df
+
+
+def _get_holding_dates(portfolio_id: str, portfolio_ids: Optional[Union[List[str], str]] = None) -> list:
+    try:
+        url = f"{_config.portfolio_service_url()}/portfoliodataservice/v1/portfolios/{portfolio_id}/dates"
+        response_json: Dict[str, list] = _portfolio_api.do_get_request(url)
+        return response_json["dates"]
+    except Exception as portfolio_error:
+        if portfolio_error.__class__.__name__ != "ResourceNotFoundError":
+            raise portfolio_error from None
+        pass
+    return []
+
+
+def _format_date(date: str) -> str:
+    try:
+        return time.strftime("%Y-%m-%d", time.strptime(date, "%Y-%m-%d"))
+    except Exception as e:
+        # _logger.error(f"Date format error: {e}")
+        raise BadRequestException(ErrorMessages.date_format_error.value + f" Date format error: {e}.") from None
+
+
+@_decorator.typechecked
+def get_data(
+    portfolio_id: str,
+    data_set_id: Optional[Union[str, PortfolioDataSet, None]] = None,
+    currency: Optional[str] = None,
+    start_date: Optional[str] = None,
+    end_date: Optional[str] = None,
+    data_point_settings: Optional[DataFrame] = None,
+) -> DataFrame:
+    """Returns data for the given portfolio and data points.
+
+    Args:
+        portfolio_id (:obj:`str` ): Portfolio ID. Use the `get_portfolios <./portfolio_list.html#morningstar_data.direct.user_items.get_portfolios>`_ function to discover saved portfolios.
+        data_set_id (:obj:`str`, `optional`): Saved portfolio data set, e.g., "1". Use the `get_data_sets <./data_set.html#morningstar_data.direct.portfolio.get_data_sets>`_ function to discover available data sets.
+        currency (:obj:`str`, `optional`): Currency setting for the data point values, when applicable. Use the `currency_codes <../morningstar_data/lookup.html#morningstar_data.lookup.currency_codes>`_ function to discover available currency codes.
+        start_date (:obj:`str`, `optional`): Start date of a date range for retrieving data.
+            The format is YYYY-MM-DD, e.g., '2020-01-01'.
+        end_date (:obj:`str`, `optional`): End date of a date range for retrieving data. If no value is provided for `end_date`, current date will be used.
+            The format is YYYY-MM-DD, e.g., '2020-01-01'.
+        data_point_settings (:obj:`DataFrame`, `optional`): A DataFrame of data points with all defined settings. Each row represents a data point.
+            Each column is a configurable setting. Users can get this DataFrame by using `get_data_set_data_points <./data_set.html#morningstar_data.direct.portfolio.get_data_set_data_points>`_ or `get_data_point_settings <../morningstar_data/lookup.html#morningstar_data.direct.get_data_point_settings>`_ for a given data point ID(s).
+            Users can update setting values in this DataFrame if desired. Additionally, the priority of currency/start_date/end_date in `data_point_settings`
+            is lower than the currency/start_date/end_date function parameters.
+
+
+    Returns:
+        DataFrame: A DataFrame object with portfolio data.
+
+    Examples:
+        Get portfolio data for the given portfolio and data set.
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.portfolio.get_data(
+            portfolio_id="8c6de08f-a668-4e78-a688-3d809aeb29b7;UA", # Replace with a valid portfolio ID
+            data_set_id="1")
+        df
+
+    :Output:
+        =========================================  =====   ==============   ================   =====   =================================   ==================================
+        Id                                         Name    Base Currency    Portfolio Date     ...     Total Ret Annlzd 10 Yr (Year-End)   Total Ret Annlzd 15 Yr (Year-End)
+        =========================================  =====   ==============   ================   =====   =================================   ==================================
+        8c6de08f-a668-4e78-a688-3d809aeb29b7;UA    test1   US Dollar        2022-02-28         ...     None                                None
+        ...
+        =========================================  =====   ==============   ================   =====   =================================   ==================================
+
+    Errors:
+        AccessDeniedError: Raised when the user is not authenticated.
+
+        BadRequestError: Raised when the user does not provide a properly formatted request.
+
+        ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
+
+    """
+    all_data = _get_portfolio_data(
+        portfolio_id=portfolio_id,
+        data_set_id=data_set_id,
+        currency=currency,
+        start_date=start_date,
+        end_date=end_date,
+        data_point_settings=data_point_settings,
+    )
+    col_name = all_data.columns.tolist()
+    all_data = all_data.reindex(columns=col_name)
+    return all_data
+
+
+def _get_portfolio_data(
+    portfolio_id: str,
+    data_set_id: Optional[Union[str, PortfolioDataSet, None]] = None,
+    currency: Optional[str] = None,
+    start_date: Optional[str] = None,
+    end_date: Optional[str] = None,
+    data_point_settings: Optional[DataFrame] = None,
+) -> DataFrame:
+    """
+    As the "get_portfolio_data" API may been called by other APIs, so we extracted it as a private method.
+    """
+    # try:
+    # build columns
+    settings_data_frame = None
+    if data_point_settings is not None and not data_point_settings.empty:
+        settings_data_frame = _get_data_settings_data_points(data_point_settings, currency, start_date, end_date)
+    else:
+        if isinstance(data_set_id, PortfolioDataSet):
+            data_set_id = data_set_id.data_set_id
+            if get_data_set_data_points(data_set_id=data_set_id).empty:
+                raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_DATA_SET_DATA_POINT) from None
+        if not data_set_id:
+            raise BadRequestException("Please specify either data_set_id or data_point_settings to proceed with your query.")
+        settings_data_frame = DataFrame(_get_data_set_data_points(data_set_id, currency, start_date, end_date))
+    portfolio_ids = [portfolio_id]
+
+    settings_data_frame = settings_data_frame.where(settings_data_frame.notnull(), None)
+
+    # get data
+    raw_data = _get_normal_data(
+        portfolio_ids,
+        _filter_disable_data_points(settings_data_frame).to_dict(orient="records"),
+    )
+
+    investment_results = _parse_raw_normal_data_values(raw_data)
+
+    # add id
+    all_data = investment_results.as_data_frame()
+    col_name = all_data.columns.tolist()
+    all_data = all_data.reindex(columns=col_name)
+
+    return all_data
+
+
+def _filter_disable_data_points(data_point_settings: DataFrame = None) -> DataFrame:
+    columns = data_point_settings.columns
+    if "disable" in columns:
+        return data_point_settings.loc[data_point_settings["disable"] != True]
+    return data_point_settings
+
+
+def _get_normal_data(portfolio_ids: list, data_points: list) -> DataFrame:
+    if not portfolio_ids:
+        raise BadRequestException("There is no portfolio data returned.")
+    postbody = {
+        "datapoints": data_points,
+        "investments": list(map(lambda x: {"id": x}, portfolio_ids)),
+    }
+    resp: DataFrame = _request_porfolio_data(postbody, portfolio_ids)
+    if resp is None:
+        raise BadRequestException("There is no return data available.")
+    return resp
+
+
+def _request_porfolio_data(postbody: dict, portfolio_ids: list) -> DataFrame:
+    job_detail, portfolio_data = _get_portfolio_job(postbody)
+    job_id = job_detail["id"]
+    try_times = 10
+    while True:
+        job_detail, portfolio_data = _get_portfolio_job(postbody, job_id)
+        time.sleep(2)
+        try_times = try_times - 1
+        if job_detail.get("percentage", "0") == "100" or try_times == 0:
+            break
+    if not portfolio_data:
+        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_PORTFOLIO_GET_DATA_RETURN.format(portfolio_ids[0]))
+    return portfolio_data
+
+
+def _get_portfolio_job(postbody: dict, job_id: Optional[str] = None) -> tuple:
+    url = f"{_config.portfolio_service_url()}/portfoliodataservice/v1/portfolios/calculation?maxExecTime=600000&maxWaitTime=600000&timeOut=600000"
+    if job_id:
+        url = url + f"&jobId={job_id}"
+    response_json = _portfolio_api.do_post_request(url, json.dumps(postbody, ignore_nan=True).replace("NaN", "null"))
+    job_detail = response_json["job"]
+    portfolio_data = None
+
+    if job_detail.get("percentage", "0") == "100":
+        portfolio_data = response_json
+    return job_detail, portfolio_data
+
+
+def _get_data_settings_data_points(
+    data_point_settings: DataFrame,
+    currency: Optional[str],
+    start_date: Optional[str],
+    end_date: Optional[str],
+) -> DataFrame:
+    if "datapointId" not in data_point_settings.columns:
+        raise BadRequestException("Please input valid data_point_settings to proceed with your query.")
+    data_point_settings = data_point_settings.where(data_point_settings.notnull(), None)
+    start_date, end_date = _format_start_end_date(start_date, end_date)
+    # only set currency to the data_points with currency.
+    # only set start_date/end_date to the datapoints without isTsdp=False.
+
+    data_point_default_settings = _get_data_points_default_settings(data_point_settings["datapointId"].tolist())
+
+    settings_list = data_point_settings.to_dict(orient="records")
+    for settings in settings_list:
+        data_point_id = settings["datapointId"]
+        defined_data_point = data_point_default_settings.get(data_point_id)
+        if defined_data_point is not None and defined_data_point.get("currency") is None:
+            settings["currency"] = None
+        elif currency is not None and len(currency.strip()) > 0:
+            settings["currency"] = currency
+        if defined_data_point is not None and defined_data_point.get("isTsdp") is not None and settings.get("isTsdp") is None:
+            settings["isTsdp"] = defined_data_point.get("isTsdp")
+
+        if settings.get("isTsdp") is not False and start_date is not None and len(start_date.strip()) > 0 and end_date is not None and len(end_date.strip()) > 0:
+            settings["startDate"] = start_date
+            settings["endDate"] = end_date
+
+        esg_data_point = data_point_default_settings.get(data_point_id)
+        if data_point_id != "OS01W" and esg_data_point is not None and settings.get("isTsdp") is None:
+            if esg_data_point.get("isTsdp") is not None:
+                settings["isTsdp"] = esg_data_point.get("isTsdp")
+            else:
+                start = settings.get("startDate")
+                end = settings.get("endDate")
+                if start is not None and len(start.strip()) > 0 and end is not None and len(end.strip()) > 0:
+                    settings["isTsdp"] = True
+                else:
+                    settings["isTsdp"] = False
+    data_point_settings = DataFrame(settings_list)
+    data_point_settings = data_point_settings.where(data_point_settings.notnull(), None)
+    data_points = DataPoints(data_point_settings)
+    settings_data_frame = DataFrame(data_points.get_data_points().to_dict(orient="records"))
+    settings_data_frame = _disable_data_points(settings_data_frame, data_point_default_settings)
+
+    return settings_data_frame
+
+
+def _disable_data_points(settings_data_frame: DataFrame, defined_data_points: dict) -> DataFrame:
+    settings_list = settings_data_frame.to_dict(orient="records")
+    for settings in settings_list:
+        data_point_id = settings["datapointId"]
+        frequency_m_data_point = defined_data_points.get(data_point_id)
+        if frequency_m_data_point is not None:
+            frequency = settings.get("frequency")
+            defined_freq = frequency_m_data_point.get("frequency", None)
+            if defined_freq is not None and frequency is not None and len(frequency.strip()) > 0 and frequency != defined_freq:
+                settings["disable"] = True
+
+        defined_data_point = defined_data_points.get(data_point_id)
+        # for defined datapoint with isTsdp = False
+        if defined_data_point is not None:
+            if defined_data_point.get("isTsdp") is False and settings.get("isTsdp") is True:
+                settings["disable"] = True
+            if defined_data_point.get("isTsdp") is True and settings.get("isTsdp") is False:
+                settings["disable"] = True
+    settings_data_frame = DataFrame(settings_list)
+    settings_data_frame = settings_data_frame.where(settings_data_frame.notnull(), None)
+    return settings_data_frame
+
+
+def _get_data_set_data_points(
+    data_set_id: str,
+    currency: Optional[str],
+    start_date: Optional[str],
+    end_date: Optional[str],
+) -> list:
+    data_point_ids = _get_data_points_by_view_id(data_set_id, currency)
+    data_points = DataPoints(data_point_ids)
+    if not data_point_ids:
+        return list(data_points.get_data_points().to_dict(orient="records"))
+    data_set_type = PortfolioDataSet.get_data_set_type(data_set_id)
+    if data_set_type == DataSetType.TimeSeries:
+        if start_date is None or len(start_date.strip()) == 0:
+            raise BadRequestException(_error_messages.BAD_REQUEST_ERROR_NO_START_AND_END_DATE) from None
+        if end_date is None or len(end_date.strip()) == 0:
+            raise BadRequestException(_error_messages.BAD_REQUEST_ERROR_NO_END_DATE)
+        for data_point_id in data_point_ids:
+            if data_point_id.get("isTsdp") is True:
+                data_point_id["startDate"] = start_date
+                data_point_id["endDate"] = end_date
+
+    if data_set_type == DataSetType.Custom_Calculation:
+        start_date, end_date = _format_start_end_date(start_date, end_date)
+        if start_date is not None and len(start_date.strip()) > 0 and end_date is not None and len(end_date.strip()) > 0:
+            for data_point_id in data_point_ids:
+                data_point_id["startDate"] = start_date
+                data_point_id["endDate"] = end_date
+        return list(data_points.get_data_points().to_dict(orient="records"))
+
+    if data_set_type == DataSetType.Current_Or_TimeSeries:
+        start_date, end_date = _format_start_end_date(start_date, end_date)
+        for data_point_id in data_point_ids:
+            if data_point_id.get("isTsdp") is not False and start_date is not None and len(start_date.strip()) > 0 and end_date is not None and len(end_date.strip()) > 0:
+                data_point_id["startDate"] = start_date
+                data_point_id["endDate"] = end_date
+                data_point_id["isTsdp"] = True
+                # support 'm' only
+                data_point_id["frequency"] = "m"
+            else:
+                data_point_id["isTsdp"] = False
+        return list(data_points.get_data_points().to_dict(orient="records"))
+
+    return data_point_ids
+
+
+def _format_start_end_date(start_date: Optional[str], end_date: Optional[str]) -> tuple:
+    if start_date is not None and len(start_date.strip()) > 0:
+        start_date = _format_date(start_date)
+        if end_date is None or len(end_date.strip()) == 0:
+            raise BadRequestException(ErrorMessages.start_end_date_error.value)
+        end_date = _format_date(end_date)
+    elif end_date is not None and len(end_date.strip()) > 0:
+        raise BadRequestException(ErrorMessages.start_end_date_error.value)
+    return start_date, end_date
+
+
+@_decorator.typechecked
+def get_benchmark_settings(portfolio_id: str) -> DataFrame:
+    """
+    Returns a portfolio's benchmark settings.
+
+    Args:
+        portfolio_id (:obj:`str` ): Portfolio ID. Use the `get_portfolios <./portfolio_list.html#morningstar_data.direct.user_items.get_portfolios>`_ function to discover saved portfolios.
+
+    Returns:
+        DataFrame: A DataFrame object containing the portfolio settings.
+
+    :Examples:
+
+    Get portfolio settings for a custom model portfolio.
+    ::
+        import morningstar_data as md
+
+        df = md.direct.portfolio.get_settings(
+            portfolio_id="d38b96dd-fbe1-4750-b05d-fa7cf4b6e35a;MD") # Replace with a valid portfolio ID
+        df
+
+    :Output:
+
+        ========================================  ====================================  ====================================  ================  ======================  ==============  ================  ======================  =====================
+        Portfolio ID                              Risk Free Proxy ID                    Benchmark 1 ID                        Benchmark 1 Name  Benchmark 1 SecurityId  Benchmark 2 ID  Benchmark 2 Name  Benchmark 2 SecurityId  Internal Portfolio ID
+        ========================================  ====================================  ====================================  ================  ======================  ==============  ================  ======================  =====================
+        d38b96dd-fbe1-4750-b05d-fa7cf4b6e35a;MD   e9b23e21-9c6f-4696-9583-3b3729b4ad99  fcff80f8-2fbc-4211-bbce-45252008a9cc  S&P 500 TR USD    XIUSA04G92;XI           None            None              None                    None
+
+        ========================================  ====================================  ====================================  ================  ======================  ==============  ================  ======================  =====================
+
+    Errors:
+        AccessDeniedError: Raised when the user is not authenticated.
+
+        BadRequestError: Raised when the user does not provide a properly formatted request.
+
+        ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
+
+    """
+
+    _logger.info("Fetching portfolio settings by id")
+    portfolio_settings = _get_settings_by_id(portfolio_id=portfolio_id)
+    settings = {}
+    settings["Porfolio ID"] = portfolio_settings["portfolio"]["portfolioId"]
+    settings["Internal Portfolio ID"] = portfolio_settings["portfolio"]["portfolio2Id"]
+    settings["Risk Free Proxy ID"] = portfolio_settings["portfolio"]["riskFreeProxyId"]
+
+    primary_benchmark = portfolio_settings["portfolio"]["benchmarkId"]
+    secondary_benchmark = portfolio_settings["portfolio"]["secondaryBenchmarkId"]
+    # The secondary benchmark is optional so not all portfolios will have this information
+    secondary_benchmark_name = None
+    secondary_benchmark_id = None
+
+    for benchmark in portfolio_settings["benchmarks"]:
+        benchmark_id = benchmark["benchmarkId"]
+        if benchmark_id == primary_benchmark:
+            primary_benchmark_name = benchmark["name"]
+            primary_benchmark_sec_id = benchmark["securityId"]
+
+        elif benchmark_id == secondary_benchmark:
+            secondary_benchmark_name = benchmark["name"]
+            secondary_benchmark_id = benchmark["securityId"]
+
+    settings["Benchmark 1 ID"] = primary_benchmark
+    settings["Benchmark 1 Name"] = primary_benchmark_name
+    settings["Benchmark 1 Security ID"] = primary_benchmark_sec_id
+
+    settings["Benchmark 2 ID"] = secondary_benchmark
+    settings["Benchmark 2 Name"] = secondary_benchmark_name
+    settings["Benchmark 2 Security ID"] = secondary_benchmark_id
+
+    return DataFrame(settings, index=[0])
+
+
+def _get_settings_by_id(portfolio_id: str) -> dict:
+    try:
+        url = f"{_config.portfolio_service_url()}/portfoliodataservice/v1/portfolios/{portfolio_id}/settings"
+        response_json = _portfolio_api.do_get_request(url)
+        settings: dict = response_json["settings"]  # settings key is always present when 200 status code is returned.
+        return settings
+    except Exception as portfolio_error:
+        if portfolio_error.__class__.__name__ != "ResourceNotFoundError":
+            raise portfolio_error from None
+        pass
+    return {}
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/returns.py` & `morningstar_data-1.3.0/morningstar_data/direct/returns.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-import pandas as pd
-import numpy as np
-import warnings
-from typing import List, Optional, Union, List, Dict, Any
-
-from . import _decorator, lookup
-from ..direct import investment
-from ._exceptions import BadRequestException, ResourceNotFoundError
-from . import _error_messages
-from .data_type import Frequency
-from ._config_key import FORMAT_DATE
-
-
-@_decorator.typechecked
-def returns(
-    investments: Union[List[str], str, Dict[str, Any]],
-    start_date: str = "2020-01-01",
-    end_date: Optional[str] = None,
-    freq: Union[Frequency, str] = Frequency.monthly,
-    currency: Optional[str] = None,
-) -> pd.DataFrame:
-    warnings.warn(
-        "The returns function is deprecated and will be removed in the next major version. Use get_returns instead",
-        FutureWarning,
-        stacklevel=2,
-    )
-    return get_returns(investments, start_date, end_date, freq, currency)
-
-
-@_decorator.typechecked
-def get_returns(
-    investments: Union[List[str], str, Dict[str, Any]],
-    start_date: str = "2020-01-01",
-    end_date: Optional[str] = None,
-    freq: Union[Frequency, str] = Frequency.monthly,
-    currency: Optional[str] = None,
-) -> pd.DataFrame:
-    """A shortcut function to fetch return data for the specified investments.
-
-    Args:
-        investments (:obj:`Union`, `required`): Defines the investments to fetch. Input can be:
-
-            * Investment IDs (:obj:`list`, `optional`): Investment identifiers, in the format of SecId;Universe or just SecId. E.g., ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"]. Use the `investments <./lookup.html#morningstar_data.direct.investments>`_ function to discover identifiers.
-            * Investment List ID (:obj:`str`, `optional`): Saved investment list in Morningstar Direct. Use the `get_investment_lists <./lists.html#morningstar_data.direct.user_items.get_investment_lists>`_ function to discover saved lists.
-            * Search Criteria  ID (:obj:`str`, `optional`): Saved search criteria in Morningstar Direct. Use the `get_search_criteria <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria>`_ function to discover saved search criteria.
-            * Search Criteria Condition (:obj:`dict`, `optional`): Search criteria definition. See details in the Reference section of `get_investment_data <#morningstar_data.direct.get_investment_data>`_ or use the `get_search_criteria_conditions <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria_conditions>`_ function to discover the definition of a saved search criteria.
-
-        start_date (:obj:`str`): Start date of a date range for retrieving data. The format is
-            YYYY-MM-DD, e.g., "2020-01-01".
-        end_date (:obj:`str`, `optional`): End date of a date range for retrieving data. If no value is provided for
-            end_date, current date will be used. The format is YYYY-MM-DD, e.g., "2020-01-01".
-        freq (:obj:`Frequency`): Enumeration of return frequency, which can be 'daily', 'weekly', 'monthly', 'quarterly', or 'yearly'. E.g., "md.direct.Frequency.monthly"
-        currency (:obj:`str`, `optional`): Three character code for the desired currency of returns, e.g., "USD".  Use the `currency_codes <./lookup.html#morningstar_data.lookup.currency_codes>`_ function to discover possible values.
-
-    Returns:
-        DataFrame: A DataFrame object with returns data.
-
-    Examples:
-        Get monthly returns.
-
-    ::
-
-        import morningstar_data as md
-
-
-        df = md.direct.get_returns(
-            investments=["F00000VKPI", "F000014B1Y"], start_date="2020-10-01", freq=md.direct.Frequency.monthly
-        )
-        df
-
-    :Output:
-        ==========  ====================================  ======================================
-        Name          (LF) FoF Bal Blnd US Priv Banking     (LF) High Yield A List Priv Banking
-        ==========  ====================================  ======================================
-        2020-10-31     -2.121865                             -0.686248
-        2020-11-30     6.337255                              5.682299
-        2020-12-31     1.464777                              3.011518
-        ...
-        ==========  ====================================  ======================================
-
-    Errors:
-        AccessDeniedError: Raised when the user is not properly authenticated.
-
-        BadRequestError: Raised when the user does not provide a properly formatted request.
-
-        ForbiddenError: Raised when the user lacks permission to access a resource.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
-
-    """
-
-    if not isinstance(freq, Frequency):
-        warnings.warn(
-            "The use of string values for the 'freq' parameter is deprecated and will be removed in the next major version. Use Frequency enum values instead",
-            FutureWarning,
-            stacklevel=2,
-        )
-
-    freq = Frequency[freq]
-    assert isinstance(freq, Frequency)
-
-    start_date = pd.to_datetime(start_date).strftime(FORMAT_DATE)
-    data_point_details = lookup.get_data_point_settings(data_point_ids=[freq.data_point_id, "OS01W"]).copy()
-    if data_point_details.empty:
-        raise BadRequestException("Failed to retrieve datapoint details.")
-
-    # Remove single period timeseries data (due to id collision)
-    data_point_details = data_point_details.loc[(data_point_details["datapointId"].isin(["OS01W"])) | (data_point_details["isTsdp"])]
-    data_point_details["startDate"] = start_date
-    data_point_details["currency"] = currency
-    if end_date:
-        end_date = pd.to_datetime(end_date).strftime(FORMAT_DATE)
-        data_point_details["endDate"] = end_date
-
-    return_value = investment.get_investment_data(investments=investments, data_points=data_point_details)
-
-    if return_value is None or return_value.empty:
-        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_NO_RETURNS_RETRIEVED)
-    if "Id" in return_value.columns:
-        return_value = return_value.drop(["Id"], axis=1)
-    return_value = return_value.replace(r"^\s*$", None, regex=True)
-
-    if return_value.empty:
-        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_NO_RETURNS_RETRIEVED_FOR_INVESTMENT_LIST)
-
-    df = return_value.T
-    df.columns = df.iloc[-1]
-    df.drop(df.tail(1).index, inplace=True)
-    new_index = {x: pd.to_datetime(x[-10:]) for x in df.index}
-    df = df.rename(index=new_index)
-    return df
-
-
-@_decorator.typechecked
-def excess_returns(
-    investments: Union[List, str, Dict[str, Any]],
-    benchmark_sec_id: str,
-    start_date: str = "2020-01-01",
-    end_date: Optional[str] = None,
-    freq: Union[Frequency, str] = Frequency.monthly,
-    currency: Optional[str] = None,
-) -> pd.DataFrame:
-    warnings.warn(
-        "The excess_returns function is deprecated and will be removed in the next major version. Use get_excess_returns instead",
-        FutureWarning,
-        stacklevel=2,
-    )
-    return get_excess_returns(investments, benchmark_sec_id, start_date, end_date, freq, currency)
-
-
-@_decorator.typechecked
-def get_excess_returns(
-    investments: Union[List, str, Dict[str, Any]],
-    benchmark_sec_id: str,
-    start_date: str = "2020-01-01",
-    end_date: Optional[str] = None,
-    freq: Union[Frequency, str] = Frequency.monthly,
-    currency: Optional[str] = None,
-) -> pd.DataFrame:
-    """A shortcut function to fetch excess return data for the specified investments.
-
-    Args:
-        investments (:obj:`Union`, `required`): Defines the investments to fetch. Input can be:
-
-            * Investment IDs (:obj:`list`, `optional`): Investment identifiers, in the format of SecId;Universe or just SecId. E.g., ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"]. Use the `investments <./lookup.html#morningstar_data.direct.investments>`_ function to discover identifiers.
-            * Investment List ID (:obj:`str`, `optional`): Saved investment list in Morningstar Direct. Use the `get_investment_lists <./lists.html#morningstar_data.direct.user_items.get_investment_lists>`_ function to discover saved lists.
-            * Search Criteria  ID (:obj:`str`, `optional`): Saved search criteria in Morningstar Direct. Use the `get_search_criteria <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria>`_ function to discover saved search criteria.
-            * Search Criteria Condition (:obj:`dict`, `optional`): Search criteria definition. See details in the Reference section of `get_investment_data <#morningstar_data.direct.get_investment_data>`_ or use the `get_search_criteria_conditions <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria_conditions>`_ function to discover the definition of a saved search criteria.
-
-        benchmark_sec_id (:obj:`str`): SecId of the security to use as the benchmark. Use the `investments <./lookup.html#morningstar_data.direct.investments>`_ function to discover identifiers.
-        start_date (:obj:`str`): Start date of a date range for retrieving data. The format is
-            YYYY-MM-DD, e.g., "2020-01-01".
-        end_date (:obj:`str`, `optional`): End date of a date range for retrieving data. If no value is provided for
-            end_date, current date will be used. The format is YYYY-MM-DD, e.g., "2020-01-01".
-        freq (:obj:`Frequency`): Enumeration of return frequency, which can be 'daily', 'weekly', 'monthly', 'quarterly', or 'yearly'. E.g., "md.direct.Frequency.monthly"
-        currency (:obj:`str`, `optional`): Three character code for the desired currency of returns, e.g., "USD".  Use the `currency_codes <./lookup.html#morningstar_data.lookup.currency_codes>`_ function to discover possible values.
-
-
-    Returns:
-        DataFrame: A DataFrame object with excess return data.
-
-    Examples:
-        Get monthly excess returns.
-
-    ::
-
-        import morningstar_data as md
-
-        df = md.direct.get_excess_returns(
-            investments=["F00000VKPI", "F000014B1Y"],
-            benchmark_sec_id="F00000PLYW",
-            freq=md.direct.Frequency.daily
-        )
-        df
-
-    :Output:
-        ==========  ====================================  ======================================
-        Name          (LF) FoF Bal Blnd US Priv Banking     (LF) High Yield A List Priv Banking
-        ==========  ====================================  ======================================
-        2020-01-01     -1150.623143                          -1154.382165
-        2020-01-02     -1146.064892                          -1149.928106
-        ...
-        ==========  ====================================  ======================================
-
-    Errors:
-        AccessDeniedError: Raised when the user is not authenticated.
-
-        BadRequestError: Raised when the user does not provide a properly formatted request.
-
-        ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
-
-    """
-    if not isinstance(freq, Frequency):
-        warnings.warn(
-            "The use of string values for the 'freq' parameter is deprecated and will be removed in the next major version. Use Frequency enum values instead",
-            FutureWarning,
-            stacklevel=2,
-        )
-
-    df = get_returns(
-        investments=investments,
-        start_date=start_date,
-        end_date=end_date,
-        freq=freq,
-        currency=currency,
-    )
-
-    if df is None or df.empty:
-        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_NO_RETURNS_RETRIEVED)
-
-    benchmark_returns = get_returns(
-        investments=[benchmark_sec_id],
-        start_date=start_date,
-        end_date=end_date,
-        freq=freq,
-        currency=currency,
-    )
-
-    if benchmark_returns is None or benchmark_returns.empty:
-        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_NO_RETURNS_RETRIEVED_FOR_BENCHMARK_ID)
-
-    df["benchmark"] = benchmark_returns.iloc[:, 0]
-
-    df = df.sub(df["benchmark"], axis="rows").drop(columns=["benchmark"])
-    return df
+import pandas as pd
+import numpy as np
+import warnings
+from typing import List, Optional, Union, List, Dict, Any
+
+from . import _decorator, lookup
+from ..direct import investment
+from ._exceptions import BadRequestException, ResourceNotFoundError
+from . import _error_messages
+from .data_type import Frequency
+from ._config_key import FORMAT_DATE
+
+
+@_decorator.typechecked
+def returns(
+    investments: Union[List[str], str, Dict[str, Any]],
+    start_date: str = "2020-01-01",
+    end_date: Optional[str] = None,
+    freq: Union[Frequency, str] = Frequency.monthly,
+    currency: Optional[str] = None,
+) -> pd.DataFrame:
+    warnings.warn(
+        "The returns function is deprecated and will be removed in the next major version. Use get_returns instead",
+        FutureWarning,
+        stacklevel=2,
+    )
+    return get_returns(investments, start_date, end_date, freq, currency)
+
+
+@_decorator.typechecked
+def get_returns(
+    investments: Union[List[str], str, Dict[str, Any]],
+    start_date: str = "2020-01-01",
+    end_date: Optional[str] = None,
+    freq: Union[Frequency, str] = Frequency.monthly,
+    currency: Optional[str] = None,
+) -> pd.DataFrame:
+    """A shortcut function to fetch return data for the specified investments.
+
+    Args:
+        investments (:obj:`Union`, `required`): Defines the investments to fetch. Input can be:
+
+            * Investment IDs (:obj:`list`, `optional`): Investment identifiers, in the format of SecId;Universe or just SecId. E.g., ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"]. Use the `investments <./lookup.html#morningstar_data.direct.investments>`_ function to discover identifiers.
+            * Investment List ID (:obj:`str`, `optional`): Saved investment list in Morningstar Direct. Use the `get_investment_lists <./lists.html#morningstar_data.direct.user_items.get_investment_lists>`_ function to discover saved lists.
+            * Search Criteria  ID (:obj:`str`, `optional`): Saved search criteria in Morningstar Direct. Use the `get_search_criteria <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria>`_ function to discover saved search criteria.
+            * Search Criteria Condition (:obj:`dict`, `optional`): Search criteria definition. See details in the Reference section of `get_investment_data <#morningstar_data.direct.get_investment_data>`_ or use the `get_search_criteria_conditions <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria_conditions>`_ function to discover the definition of a saved search criteria.
+
+        start_date (:obj:`str`): Start date of a date range for retrieving data. The format is
+            YYYY-MM-DD, e.g., "2020-01-01".
+        end_date (:obj:`str`, `optional`): End date of a date range for retrieving data. If no value is provided for
+            end_date, current date will be used. The format is YYYY-MM-DD, e.g., "2020-01-01".
+        freq (:obj:`Frequency`): Enumeration of return frequency, which can be 'daily', 'weekly', 'monthly', 'quarterly', or 'yearly'. E.g., "md.direct.Frequency.monthly"
+        currency (:obj:`str`, `optional`): Three character code for the desired currency of returns, e.g., "USD".  Use the `currency_codes <./lookup.html#morningstar_data.lookup.currency_codes>`_ function to discover possible values.
+
+    Returns:
+        DataFrame: A DataFrame object with returns data.
+
+    Examples:
+        Get monthly returns.
+
+    ::
+
+        import morningstar_data as md
+
+
+        df = md.direct.get_returns(
+            investments=["F00000VKPI", "F000014B1Y"], start_date="2020-10-01", freq=md.direct.Frequency.monthly
+        )
+        df
+
+    :Output:
+        ==========  ====================================  ======================================
+        Name          (LF) FoF Bal Blnd US Priv Banking     (LF) High Yield A List Priv Banking
+        ==========  ====================================  ======================================
+        2020-10-31     -2.121865                             -0.686248
+        2020-11-30     6.337255                              5.682299
+        2020-12-31     1.464777                              3.011518
+        ...
+        ==========  ====================================  ======================================
+
+    Errors:
+        AccessDeniedError: Raised when the user is not properly authenticated.
+
+        BadRequestError: Raised when the user does not provide a properly formatted request.
+
+        ForbiddenError: Raised when the user lacks permission to access a resource.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
+
+    """
+
+    if not isinstance(freq, Frequency):
+        warnings.warn(
+            "The use of string values for the 'freq' parameter is deprecated and will be removed in the next major version. Use Frequency enum values instead",
+            FutureWarning,
+            stacklevel=2,
+        )
+
+    freq = Frequency[freq]
+    assert isinstance(freq, Frequency)
+
+    start_date = pd.to_datetime(start_date).strftime(FORMAT_DATE)
+    data_point_details = lookup.get_data_point_settings(data_point_ids=[freq.data_point_id, "OS01W"]).copy()
+    if data_point_details.empty:
+        raise BadRequestException("Failed to retrieve datapoint details.")
+
+    # Remove single period timeseries data (due to id collision)
+    data_point_details = data_point_details.loc[(data_point_details["datapointId"].isin(["OS01W"])) | (data_point_details["isTsdp"])]
+    data_point_details["startDate"] = start_date
+    data_point_details["currency"] = currency
+    if end_date:
+        end_date = pd.to_datetime(end_date).strftime(FORMAT_DATE)
+        data_point_details["endDate"] = end_date
+
+    return_value = investment.get_investment_data(investments=investments, data_points=data_point_details)
+
+    if return_value is None or return_value.empty:
+        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_NO_RETURNS_RETRIEVED)
+    if "Id" in return_value.columns:
+        return_value = return_value.drop(["Id"], axis=1)
+    return_value = return_value.replace(r"^\s*$", None, regex=True)
+
+    if return_value.empty:
+        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_NO_RETURNS_RETRIEVED_FOR_INVESTMENT_LIST)
+
+    df = return_value.T
+    df.columns = df.iloc[-1]
+    df.drop(df.tail(1).index, inplace=True)
+    new_index = {x: pd.to_datetime(x[-10:]) for x in df.index}
+    df = df.rename(index=new_index)
+    return df
+
+
+@_decorator.typechecked
+def excess_returns(
+    investments: Union[List, str, Dict[str, Any]],
+    benchmark_sec_id: str,
+    start_date: str = "2020-01-01",
+    end_date: Optional[str] = None,
+    freq: Union[Frequency, str] = Frequency.monthly,
+    currency: Optional[str] = None,
+) -> pd.DataFrame:
+    warnings.warn(
+        "The excess_returns function is deprecated and will be removed in the next major version. Use get_excess_returns instead",
+        FutureWarning,
+        stacklevel=2,
+    )
+    return get_excess_returns(investments, benchmark_sec_id, start_date, end_date, freq, currency)
+
+
+@_decorator.typechecked
+def get_excess_returns(
+    investments: Union[List, str, Dict[str, Any]],
+    benchmark_sec_id: str,
+    start_date: str = "2020-01-01",
+    end_date: Optional[str] = None,
+    freq: Union[Frequency, str] = Frequency.monthly,
+    currency: Optional[str] = None,
+) -> pd.DataFrame:
+    """A shortcut function to fetch excess return data for the specified investments.
+
+    Args:
+        investments (:obj:`Union`, `required`): Defines the investments to fetch. Input can be:
+
+            * Investment IDs (:obj:`list`, `optional`): Investment identifiers, in the format of SecId;Universe or just SecId. E.g., ["F00000YOOK;FO","FOUSA00CFV;FO"] or ["F00000YOOK","FOUSA00CFV"]. Use the `investments <./lookup.html#morningstar_data.direct.investments>`_ function to discover identifiers.
+            * Investment List ID (:obj:`str`, `optional`): Saved investment list in Morningstar Direct. Use the `get_investment_lists <./lists.html#morningstar_data.direct.user_items.get_investment_lists>`_ function to discover saved lists.
+            * Search Criteria  ID (:obj:`str`, `optional`): Saved search criteria in Morningstar Direct. Use the `get_search_criteria <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria>`_ function to discover saved search criteria.
+            * Search Criteria Condition (:obj:`dict`, `optional`): Search criteria definition. See details in the Reference section of `get_investment_data <#morningstar_data.direct.get_investment_data>`_ or use the `get_search_criteria_conditions <./search_criteria.html#morningstar_data.direct.user_items.get_search_criteria_conditions>`_ function to discover the definition of a saved search criteria.
+
+        benchmark_sec_id (:obj:`str`): SecId of the security to use as the benchmark. Use the `investments <./lookup.html#morningstar_data.direct.investments>`_ function to discover identifiers.
+        start_date (:obj:`str`): Start date of a date range for retrieving data. The format is
+            YYYY-MM-DD, e.g., "2020-01-01".
+        end_date (:obj:`str`, `optional`): End date of a date range for retrieving data. If no value is provided for
+            end_date, current date will be used. The format is YYYY-MM-DD, e.g., "2020-01-01".
+        freq (:obj:`Frequency`): Enumeration of return frequency, which can be 'daily', 'weekly', 'monthly', 'quarterly', or 'yearly'. E.g., "md.direct.Frequency.monthly"
+        currency (:obj:`str`, `optional`): Three character code for the desired currency of returns, e.g., "USD".  Use the `currency_codes <./lookup.html#morningstar_data.lookup.currency_codes>`_ function to discover possible values.
+
+
+    Returns:
+        DataFrame: A DataFrame object with excess return data.
+
+    Examples:
+        Get monthly excess returns.
+
+    ::
+
+        import morningstar_data as md
+
+        df = md.direct.get_excess_returns(
+            investments=["F00000VKPI", "F000014B1Y"],
+            benchmark_sec_id="F00000PLYW",
+            freq=md.direct.Frequency.daily
+        )
+        df
+
+    :Output:
+        ==========  ====================================  ======================================
+        Name          (LF) FoF Bal Blnd US Priv Banking     (LF) High Yield A List Priv Banking
+        ==========  ====================================  ======================================
+        2020-01-01     -1150.623143                          -1154.382165
+        2020-01-02     -1146.064892                          -1149.928106
+        ...
+        ==========  ====================================  ======================================
+
+    Errors:
+        AccessDeniedError: Raised when the user is not authenticated.
+
+        BadRequestError: Raised when the user does not provide a properly formatted request.
+
+        ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+        ResourceNotFoundError: Raised when the requested resource does not exist in Direct.
+
+    """
+    if not isinstance(freq, Frequency):
+        warnings.warn(
+            "The use of string values for the 'freq' parameter is deprecated and will be removed in the next major version. Use Frequency enum values instead",
+            FutureWarning,
+            stacklevel=2,
+        )
+
+    df = get_returns(
+        investments=investments,
+        start_date=start_date,
+        end_date=end_date,
+        freq=freq,
+        currency=currency,
+    )
+
+    if df is None or df.empty:
+        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_NO_RETURNS_RETRIEVED)
+
+    benchmark_returns = get_returns(
+        investments=[benchmark_sec_id],
+        start_date=start_date,
+        end_date=end_date,
+        freq=freq,
+        currency=currency,
+    )
+
+    if benchmark_returns is None or benchmark_returns.empty:
+        raise ResourceNotFoundError(_error_messages.RESOURCE_NOT_FOUND_ERROR_NO_RETURNS_RETRIEVED_FOR_BENCHMARK_ID)
+
+    df["benchmark"] = benchmark_returns.iloc[:, 0]
+
+    df = df.sub(df["benchmark"], axis="rows").drop(columns=["benchmark"])
+    return df
```

### Comparing `morningstar_data-1.2.0/morningstar_data/direct/user_items/_utils.py` & `morningstar_data-1.3.0/morningstar_data/direct/user_items/_utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-
-investments_list_default_columns = [
-            "secid",
-            "masterportfolioid",
-            "tradingsymbol",
-            "name",
-            "securitytype",
-            "exchangeid",
-            "category",
-        ]
-
-# these datapointIds correspond to the above columns
-investments_list_data_points = [
-                {"datapointId": "OS00I", "isTsdp": False},
-                {"datapointId": "DC09A", "isTsdp": False},
-                {"datapointId": "OS385", "isTsdp": False},
-                {"datapointId": "OS01W", "isTsdp": False},
-                {"datapointId": "OS010", "isTsdp": False},
-                {"datapointId": "OS01Z", "isTsdp": False},
-                {"datapointId": "OS245", "isTsdp": False},
+
+investments_list_default_columns = [
+            "secid",
+            "masterportfolioid",
+            "tradingsymbol",
+            "name",
+            "securitytype",
+            "exchangeid",
+            "category",
+        ]
+
+# these datapointIds correspond to the above columns
+investments_list_data_points = [
+                {"datapointId": "OS00I", "isTsdp": False},
+                {"datapointId": "DC09A", "isTsdp": False},
+                {"datapointId": "OS385", "isTsdp": False},
+                {"datapointId": "OS01W", "isTsdp": False},
+                {"datapointId": "OS010", "isTsdp": False},
+                {"datapointId": "OS01Z", "isTsdp": False},
+                {"datapointId": "OS245", "isTsdp": False},
             ]
```

### Comparing `morningstar_data-1.2.0/morningstar_data/lookup.py` & `morningstar_data-1.3.0/morningstar_data/lookup.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-from enum import Enum
-from pandas import DataFrame, concat
-from typing import Optional, Any, Dict
-
-from ._base import _logger
-from .direct._exceptions import ResourceNotFoundError
-from .direct._config import _Config
-from .direct import _decorator
-from .direct._base_api import APIBackend
-from .direct._error_messages import RESOURCE_NOT_FOUND_ERROR_LOOKUP_KEYWORD, RESOURCE_NOT_FOUND_ERROR_LOOKUP_KEYWORD_UNIVERSE
-
-_config = _Config()
-
-
-class _LookupParameter(Enum):
-    KEYWORD = 0
-    KEYWORD_UNIVERSE = 1
-
-
-class LookupAPIBackend(APIBackend):
-    """
-    Subclass to call the Holding API and handle any HTTP errors that occur.
-    """
-
-    def __init__(self, lookup_parameter: _LookupParameter) -> None:
-        self._lookup_parameter = lookup_parameter
-        super().__init__()
-
-    def _get_resource_not_found_message(self) -> str:
-        if self._lookup_parameter == _LookupParameter.KEYWORD:
-            return RESOURCE_NOT_FOUND_ERROR_LOOKUP_KEYWORD
-        return RESOURCE_NOT_FOUND_ERROR_LOOKUP_KEYWORD_UNIVERSE
-
-    def _handle_custom_http_errors(self, res: Any) -> Any:
-        """
-        Handle HTTP errors with custom error messages
-        """
-        response_message = res.json()["message"]
-        if res.status_code == 404:
-            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
-            raise ResourceNotFoundError(self._get_resource_not_found_message()) from None
-
-
-_keyword_api_request = LookupAPIBackend(_LookupParameter.KEYWORD)
-_keyword_universe_api_request = LookupAPIBackend(_LookupParameter.KEYWORD_UNIVERSE)
-
-
-def _get_data_point_options(data_point: str, universe: Optional[str]) -> dict:
-    url = f"{_config.data_point_service_url()}v1/datapoints/{data_point}/searchoperatorsandoptions"
-    _lookup_api_request = _keyword_api_request
-    if universe:
-        _logger.info("Universe is specified, so searching within this universe only.")
-        # Some data points need to specify universe, for example OF003(Morningstar Category).
-        url = url + f"?universe={universe}"
-        _lookup_api_request = _keyword_universe_api_request
-    response_json: Dict[Any, Any] = _lookup_api_request.do_get_request(url)
-    return response_json
-
-
-def _search_option_data(data_point: str, keyword: Optional[str], universe: Optional[str] = None) -> DataFrame:
-    # get the available values for special data point.
-    data_point_options = _get_data_point_options(data_point, universe)
-    df = DataFrame({"id": [], "name": []})
-    if data_point_options:
-        result = DataFrame(data=data_point_options[0].get("options"))
-        result.rename(columns={"value": "id"}, inplace=True)
-        df = result[["id", "name"]]
-
-    return _filter_data_frame(df, keyword) if keyword else df
-
-
-def _filter_data_frame(df: DataFrame, keyword: str) -> DataFrame:
-    filtered_df = concat([df[df["id"].str.contains(keyword, case=False)], df[df["name"].str.contains(keyword, case=False)]])
-    return filtered_df.drop_duplicates(subset=["id", "name"], keep="first")
-
-
-def currency_codes(keyword: Optional[str] = None) -> DataFrame:
-    """Returns currency codes and currency name that match the given keyword. If no keyword is provided, the function returns all currency codes and currency names.
-
-    Args:
-        keyword (Optional[str], optional): A string used to lookup currency codes. Example: "USD". Returns matching currency code for the keyword 'USD'.
-
-    Returns:
-        DataFrame: Returns a DataFrame. The DataFrame columns include:
-
-        * currency_code
-        * currency_name
-
-    :Examples:
-
-        Search currency codes based on keyword "Afgh"
-    ::
-
-        import morningstar_data as md
-        df = md.lookup.currency_codes(
-            keyword="Afgh"
-        )
-        df
-
-    :Output:
-        ==============  ===============
-        currency_code      currency_name
-        ==============  ===============
-        AFN                Afghani
-        ==============  ===============
-
-    Errors:
-        AccessDeniedError: Raised when the user is not authenticated.
-
-        ForbiddenError: Raised when the user does not have permission to access the requested resource.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-        ResourceNotFoundError: Raised when a currency code matching the given keyword does not exist.
-    """
-
-    # LS05M is a datapoint which name is currency, and its options include all available currency value.
-    currency_df = _search_option_data(data_point="LS05M", keyword=keyword)
-    currency_df.rename(columns={"id": "currency_code", "name": "currency_name"}, inplace=True)
-    return currency_df
+from enum import Enum
+from pandas import DataFrame, concat
+from typing import Optional, Any, Dict
+
+from ._base import _logger
+from .direct._exceptions import ResourceNotFoundError
+from .direct._config import _Config
+from .direct import _decorator
+from .direct._base_api import APIBackend
+from .direct._error_messages import RESOURCE_NOT_FOUND_ERROR_LOOKUP_KEYWORD, RESOURCE_NOT_FOUND_ERROR_LOOKUP_KEYWORD_UNIVERSE
+
+_config = _Config()
+
+
+class _LookupParameter(Enum):
+    KEYWORD = 0
+    KEYWORD_UNIVERSE = 1
+
+
+class LookupAPIBackend(APIBackend):
+    """
+    Subclass to call the Holding API and handle any HTTP errors that occur.
+    """
+
+    def __init__(self, lookup_parameter: _LookupParameter) -> None:
+        self._lookup_parameter = lookup_parameter
+        super().__init__()
+
+    def _get_resource_not_found_message(self) -> str:
+        if self._lookup_parameter == _LookupParameter.KEYWORD:
+            return RESOURCE_NOT_FOUND_ERROR_LOOKUP_KEYWORD
+        return RESOURCE_NOT_FOUND_ERROR_LOOKUP_KEYWORD_UNIVERSE
+
+    def _handle_custom_http_errors(self, res: Any) -> Any:
+        """
+        Handle HTTP errors with custom error messages
+        """
+        response_message = res.json()["message"]
+        if res.status_code == 404:
+            _logger.debug(f"Resource Not Found Error: {res.status_code} {response_message}")
+            raise ResourceNotFoundError(self._get_resource_not_found_message()) from None
+
+
+_keyword_api_request = LookupAPIBackend(_LookupParameter.KEYWORD)
+_keyword_universe_api_request = LookupAPIBackend(_LookupParameter.KEYWORD_UNIVERSE)
+
+
+def _get_data_point_options(data_point: str, universe: Optional[str]) -> dict:
+    url = f"{_config.data_point_service_url()}v1/datapoints/{data_point}/searchoperatorsandoptions"
+    _lookup_api_request = _keyword_api_request
+    if universe:
+        _logger.info("Universe is specified, so searching within this universe only.")
+        # Some data points need to specify universe, for example OF003(Morningstar Category).
+        url = url + f"?universe={universe}"
+        _lookup_api_request = _keyword_universe_api_request
+    response_json: Dict[Any, Any] = _lookup_api_request.do_get_request(url)
+    return response_json
+
+
+def _search_option_data(data_point: str, keyword: Optional[str], universe: Optional[str] = None) -> DataFrame:
+    # get the available values for special data point.
+    data_point_options = _get_data_point_options(data_point, universe)
+    df = DataFrame({"id": [], "name": []})
+    if data_point_options:
+        result = DataFrame(data=data_point_options[0].get("options"))
+        result.rename(columns={"value": "id"}, inplace=True)
+        df = result[["id", "name"]]
+
+    return _filter_data_frame(df, keyword) if keyword else df
+
+
+def _filter_data_frame(df: DataFrame, keyword: str) -> DataFrame:
+    filtered_df = concat([df[df["id"].str.contains(keyword, case=False)], df[df["name"].str.contains(keyword, case=False)]])
+    return filtered_df.drop_duplicates(subset=["id", "name"], keep="first")
+
+
+def currency_codes(keyword: Optional[str] = None) -> DataFrame:
+    """Returns currency codes and currency name that match the given keyword. If no keyword is provided, the function returns all currency codes and currency names.
+
+    Args:
+        keyword (Optional[str], optional): A string used to lookup currency codes. Example: "USD". Returns matching currency code for the keyword 'USD'.
+
+    Returns:
+        DataFrame: Returns a DataFrame. The DataFrame columns include:
+
+        * currency_code
+        * currency_name
+
+    :Examples:
+
+        Search currency codes based on keyword "Afgh"
+    ::
+
+        import morningstar_data as md
+        df = md.lookup.currency_codes(
+            keyword="Afgh"
+        )
+        df
+
+    :Output:
+        ==============  ===============
+        currency_code      currency_name
+        ==============  ===============
+        AFN                Afghani
+        ==============  ===============
+
+    Errors:
+        AccessDeniedError: Raised when the user is not authenticated.
+
+        ForbiddenError: Raised when the user does not have permission to access the requested resource.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+        ResourceNotFoundError: Raised when a currency code matching the given keyword does not exist.
+    """
+
+    # LS05M is a datapoint which name is currency, and its options include all available currency value.
+    currency_df = _search_option_data(data_point="LS05M", keyword=keyword)
+    currency_df.rename(columns={"id": "currency_code", "name": "currency_name"}, inplace=True)
+    return currency_df
```

### Comparing `morningstar_data-1.2.0/morningstar_data/utils/_delivery_config.py` & `morningstar_data-1.3.0/morningstar_data/utils/_delivery_config.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,157 +1,157 @@
-import dataclasses
-import re
-from enum import Enum
-
-from ..direct._exceptions import ValueErrorException
-
-
-class DeliveryConfigErrorMessage(Enum):
-    EMAIL = """
-        Invalid Email Address.
-        Example:
-        - email = "analyticslab.user@morningstar.com"
-    """
-    FTP = """
-        Invalid FTP configuration.
-        The username and password must not be empty
-        The server must not include any protocal, like "ftp://".
-        The folder must not include a root path '/'.
-        Example:
-        - user_name = "analyticslab_user"
-        - password = "password123"
-        - server = "ftp.morningstar.com"
-        - folder = "folder_1/folder_2/"
-    """
-    DELIVERY_PROFILE = """
-        Invalid delivery profile Id.
-        The delivery profile id must not be empty
-        The delivery profile id must be a digit string
-        Example:
-        - delivery_profile_id = "12345"
-    """
-
-
-class DeliveryType(Enum):
-    EMAIL = 1
-    FTP = 2
-    DELIVERY_PROFILE = 3
-
-
-@dataclasses.dataclass
-class DeliveryConfig:
-    """Container for delivery configuration settings
-    Args:
-        method (:obj:`DeliveryType`): Required, the type of delivery, see DeliveryType for supported options
-        email_address (:obj:`str`): a valid email_address to send the file to, needed if using "email" delivery option
-        user_name (:obj:`str`): the user_name to login to the ftp server, needed if using "ftp" method
-        password (:obj:`str`): the password to login to the ftp server, needed if using "ftp" method
-        server (:obj:`str`): the ftp server to use, needed if using "ftp" method. The server address should not include "ftp://"
-        folder (:obj:`str`): the folder on the ftp server to upload the file to, needed if using "ftp" method. The folder should not include a folder path like "/folder"
-
-    :Examples:
-
-    Valid delivery config
-
-    ::
-        email_address = "test@morningstar.com"
-        delivery_config_email = md.utils.DeliveryConfig(method=md.utils.DeliveryType.EMAIL, email_address=email_address)
-
-        ftp_username = "test"
-        ftp_password = "test_pwd"
-        ftp_server = "ts.ftp.com"
-        ftp_folder = "data/"
-        delivery_config_ftp = md.utils.DeliveryConfig(method=md.utils.DeliveryType.FTP, user_name=ftp_username, password=ftp_password, server=ftp_server, folder=ftp_folder)
-
-        delivery_profile_id = "12345"
-        delivery_config_email = md.utils.DeliveryConfig(method=md.utils.DeliveryType.DELIVERY_PROFILE, delivery_profile_id=delivery_profile_id)
-
-    Invalid delivery config
-
-    ::
-        email_address = "@invalid_email_address@morningstar.com"
-        delivery_config_email = md.utils.DeliveryConfig(method=md.utils.DeliveryType.EMAIL, email_address=email_address)
-        >>> ValueErrorException: Invalid Email Address
-
-        ftp_username = "test"
-        ftp_password = "test_pwd"
-        ftp_server = "ftp://ts.ftp.com"
-        ftp_folder = "/data/"
-        delivery_config_ftp = md.utils.DeliveryConfig(method=md.utils.DeliveryType.FTP, user_name=ftp_username, password=ftp_password, server=ftp_server, folder=ftp_folder)
-        >>> ValueErrorException: Invalid FTP configuration
-
-        delivery_profile_id = "12ABC"
-        delivery_config_email = md.utils.DeliveryConfig(method=md.utils.DeliveryType.DELIVERY_PROFILE, delivery_profile_id=delivery_profile_id)
-        >>> ValueErrorException: Invalid delivery profile Id
-    """
-
-    method: DeliveryType
-    email_address: str = ""
-    delivery_profile_id: str = ""
-    user_name: str = ""
-    password: str = ""
-    server: str = ""
-    folder: str = ""
-
-    def __post_init__(self) -> None:
-        if not self.is_valid():
-            raise ValueErrorException(DeliveryConfigErrorMessage[self.method.name].value)
-
-    def _is_email_valid(self) -> bool:
-        """Check whether the email config provided is valid"""
-        email_regex = re.compile(
-            r"""\b             # a word boundary
-                [a-z0-9._%+-]+ # the email prefix part, any character in the list
-                @              # the @ part
-                [a-z0-9.-]+    # the email domain name part, any character in the list
-                \.             # the dot part
-                [a-z]{2,}      # the top-level domain part, any alphabetical character and length >= 2
-                \b             # a word boundary
-            """,
-            re.X,
-        )
-        return re.fullmatch(email_regex, self.email_address.lower()) is not None
-
-    def _is_delivery_profile_valid(self) -> bool:
-        """Checks if the provided delivery profile ID is valid.
-        At present, the MDS delivery endpoint allows any user to deliver to any profile ID.
-        In the future, MDS need to add validation based on the user's company.
-        """
-        return self.delivery_profile_id.isdigit()
-
-    def _is_ftp_valid(self) -> bool:
-        """Check whether the ftp config provided is valid"""
-        if self.user_name == "" or self.password == "":
-            return False
-
-        server_regex = re.compile(
-            r"""\b          # a word boundary
-                [a-z0-9.-]+ # the domain name part, any character in the list
-                \.          # the dot part
-                [a-z]{2,}   # the top-level domain part, any alphabetical character and length >= 2
-                \b          # a word boundary
-            """,
-            re.X,
-        )
-        if not re.fullmatch(server_regex, self.server.lower()):
-            return False
-
-        folder_regex = re.compile(
-            r"""
-                ^[^\/]                   # cannot start with /
-                (
-                    [\w\d\s\._%+-\[\]]+  # any character in the list
-                    [\/]{1,1}            # ending with /
-                )+                       # capturing group
-            """,
-            re.X,
-        )
-        if not re.fullmatch(folder_regex, self.folder):
-            return False
-
-        return True
-
-    def is_valid(self) -> bool:
-        is_email_valid = self.method == DeliveryType.EMAIL and self._is_email_valid()
-        is_ftp_valid = self.method == DeliveryType.FTP and self._is_ftp_valid()
-        is_delivery_profile_valid = self.method == DeliveryType.DELIVERY_PROFILE and self._is_delivery_profile_valid()
-        return is_email_valid or is_ftp_valid or is_delivery_profile_valid
+import dataclasses
+import re
+from enum import Enum
+
+from ..direct._exceptions import ValueErrorException
+
+
+class DeliveryConfigErrorMessage(Enum):
+    EMAIL = """
+        Invalid Email Address.
+        Example:
+        - email = "analyticslab.user@morningstar.com"
+    """
+    FTP = """
+        Invalid FTP configuration.
+        The username and password must not be empty
+        The server must not include any protocal, like "ftp://".
+        The folder must not include a root path '/'.
+        Example:
+        - user_name = "analyticslab_user"
+        - password = "password123"
+        - server = "ftp.morningstar.com"
+        - folder = "folder_1/folder_2/"
+    """
+    DELIVERY_PROFILE = """
+        Invalid delivery profile Id.
+        The delivery profile id must not be empty
+        The delivery profile id must be a digit string
+        Example:
+        - delivery_profile_id = "12345"
+    """
+
+
+class DeliveryType(Enum):
+    EMAIL = 1
+    FTP = 2
+    DELIVERY_PROFILE = 3
+
+
+@dataclasses.dataclass
+class DeliveryConfig:
+    """Container for delivery configuration settings
+    Args:
+        method (:obj:`DeliveryType`): Required, the type of delivery, see DeliveryType for supported options
+        email_address (:obj:`str`): a valid email_address to send the file to, needed if using "email" delivery option
+        user_name (:obj:`str`): the user_name to login to the ftp server, needed if using "ftp" method
+        password (:obj:`str`): the password to login to the ftp server, needed if using "ftp" method
+        server (:obj:`str`): the ftp server to use, needed if using "ftp" method. The server address should not include "ftp://"
+        folder (:obj:`str`): the folder on the ftp server to upload the file to, needed if using "ftp" method. The folder should not include a folder path like "/folder"
+
+    :Examples:
+
+    Valid delivery config
+
+    ::
+        email_address = "test@morningstar.com"
+        delivery_config_email = md.utils.DeliveryConfig(method=md.utils.DeliveryType.EMAIL, email_address=email_address)
+
+        ftp_username = "test"
+        ftp_password = "test_pwd"
+        ftp_server = "ts.ftp.com"
+        ftp_folder = "data/"
+        delivery_config_ftp = md.utils.DeliveryConfig(method=md.utils.DeliveryType.FTP, user_name=ftp_username, password=ftp_password, server=ftp_server, folder=ftp_folder)
+
+        delivery_profile_id = "12345"
+        delivery_config_email = md.utils.DeliveryConfig(method=md.utils.DeliveryType.DELIVERY_PROFILE, delivery_profile_id=delivery_profile_id)
+
+    Invalid delivery config
+
+    ::
+        email_address = "@invalid_email_address@morningstar.com"
+        delivery_config_email = md.utils.DeliveryConfig(method=md.utils.DeliveryType.EMAIL, email_address=email_address)
+        >>> ValueErrorException: Invalid Email Address
+
+        ftp_username = "test"
+        ftp_password = "test_pwd"
+        ftp_server = "ftp://ts.ftp.com"
+        ftp_folder = "/data/"
+        delivery_config_ftp = md.utils.DeliveryConfig(method=md.utils.DeliveryType.FTP, user_name=ftp_username, password=ftp_password, server=ftp_server, folder=ftp_folder)
+        >>> ValueErrorException: Invalid FTP configuration
+
+        delivery_profile_id = "12ABC"
+        delivery_config_email = md.utils.DeliveryConfig(method=md.utils.DeliveryType.DELIVERY_PROFILE, delivery_profile_id=delivery_profile_id)
+        >>> ValueErrorException: Invalid delivery profile Id
+    """
+
+    method: DeliveryType
+    email_address: str = ""
+    delivery_profile_id: str = ""
+    user_name: str = ""
+    password: str = ""
+    server: str = ""
+    folder: str = ""
+
+    def __post_init__(self) -> None:
+        if not self.is_valid():
+            raise ValueErrorException(DeliveryConfigErrorMessage[self.method.name].value)
+
+    def _is_email_valid(self) -> bool:
+        """Check whether the email config provided is valid"""
+        email_regex = re.compile(
+            r"""\b             # a word boundary
+                [a-z0-9._%+-]+ # the email prefix part, any character in the list
+                @              # the @ part
+                [a-z0-9.-]+    # the email domain name part, any character in the list
+                \.             # the dot part
+                [a-z]{2,}      # the top-level domain part, any alphabetical character and length >= 2
+                \b             # a word boundary
+            """,
+            re.X,
+        )
+        return re.fullmatch(email_regex, self.email_address.lower()) is not None
+
+    def _is_delivery_profile_valid(self) -> bool:
+        """Checks if the provided delivery profile ID is valid.
+        At present, the MDS delivery endpoint allows any user to deliver to any profile ID.
+        In the future, MDS need to add validation based on the user's company.
+        """
+        return self.delivery_profile_id.isdigit()
+
+    def _is_ftp_valid(self) -> bool:
+        """Check whether the ftp config provided is valid"""
+        if self.user_name == "" or self.password == "":
+            return False
+
+        server_regex = re.compile(
+            r"""\b          # a word boundary
+                [a-z0-9.-]+ # the domain name part, any character in the list
+                \.          # the dot part
+                [a-z]{2,}   # the top-level domain part, any alphabetical character and length >= 2
+                \b          # a word boundary
+            """,
+            re.X,
+        )
+        if not re.fullmatch(server_regex, self.server.lower()):
+            return False
+
+        folder_regex = re.compile(
+            r"""
+                ^[^\/]                   # cannot start with /
+                (
+                    [\w\d\s\._%+-\[\]]+  # any character in the list
+                    [\/]{1,1}            # ending with /
+                )+                       # capturing group
+            """,
+            re.X,
+        )
+        if not re.fullmatch(folder_regex, self.folder):
+            return False
+
+        return True
+
+    def is_valid(self) -> bool:
+        is_email_valid = self.method == DeliveryType.EMAIL and self._is_email_valid()
+        is_ftp_valid = self.method == DeliveryType.FTP and self._is_ftp_valid()
+        is_delivery_profile_valid = self.method == DeliveryType.DELIVERY_PROFILE and self._is_delivery_profile_valid()
+        return is_email_valid or is_ftp_valid or is_delivery_profile_valid
```

### Comparing `morningstar_data-1.2.0/morningstar_data/utils/_helpers.py` & `morningstar_data-1.3.0/morningstar_data/utils/_helpers.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,221 +1,221 @@
-import simplejson as json
-import logging
-import os
-import re
-import pathlib
-import string
-import uuid
-from typing import Dict, Optional
-
-import boto3
-import jwt
-import requests
-from urllib3.exceptions import InsecureRequestWarning
-
-from ..direct._exceptions import ForbiddenError
-from ._delivery_config import DeliveryConfig, DeliveryType
-from ..direct._config import _Config
-
-from ..direct._backend_apis import DeliveryAPIBackend
-from ..direct._exceptions import BadRequestException, UnauthorizedDeliveryException
-
-# NOTE: We are not able to verify the SSL cert on MDS API since
-#       the VPC endpoint domain name is not on the server's SSL cert.
-#       So with a heavy heart, we disable the InsecureRequestWarning
-requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
-
-
-_logger = logging.getLogger(__name__)
-_config = _Config()
-
-# A filename can include 'a-z', 'A-Z', '0-9', '-', '_', '(', ')', ' ', '.'
-_invalid_chars_regex = re.compile(r"[^a-zA-Z\d\-_\(\)\ .]")
-
-
-def _get_user_id_from_uim_token() -> str:
-    """Returns the user's id by decoding their UIM token"""
-    try:
-        md_auth_token = md_auth_token = os.getenv("MD_AUTH_TOKEN", os.getenv("UIM_JWT", ""))
-        decode_key = os.getenv("UIM_DECODE_KEY", "https://login-prod.morningstar.com/.well-known/jwks.json")
-        jwks_client = jwt.jwks_client.PyJWKClient(decode_key)
-        signing_key = jwks_client.get_signing_key_from_jwt(md_auth_token)
-        decoded_jwt = jwt.decode(
-            md_auth_token,
-            signing_key.key,
-            algorithms=["RS256"],
-            options={"verify_signature": True, "verify_exp": True, "verify_aud": False},
-            leeway=60,
-        )
-        user_id: str = decoded_jwt["sub"].split("|")[1]
-        return user_id.upper()
-    except Exception as err:
-        _logger.error(f"Error decoding MD_AUTH_TOKEN: {err}")
-        raise
-
-
-def _get_user_id_from_eams_token() -> str:
-    """Returns the user's id by decoding their EAMS token"""
-    try:
-        key = os.getenv("EAMS_PUBLIC_KEY", "").replace("\\n", "\n")
-        token = os.getenv("EAMS_JWT")
-        decoded = jwt.decode(token, key, algorithms=["RS256"])
-        user_id: str = decoded["sub"]
-        return user_id.upper()
-    except Exception as err:
-        _logger.error(f"Error decoding EAMS token: {err}")
-        raise
-
-
-def _get_user_id() -> str:
-    """Returns the user's id using their UIM token if it exists, EAMS token otherwise"""
-    try:
-        user_id = _get_user_id_from_uim_token()
-        _logger.info(f"Using UIM token for User ID: {user_id}")
-        return user_id
-    except Exception:
-        pass
-
-    user_id = _get_user_id_from_eams_token()
-    _logger.info(f"Using EAMS token for User ID: {user_id}")
-    return user_id
-
-
-def _get_job_name() -> str:
-    """Returns the job name for a feed or delivery"""
-    return str(uuid.uuid4())
-
-
-def _get_request_id() -> str:
-    """Returns the request id for use in POST requests"""
-    request_id = os.getenv("REQUEST_ID", str(uuid.uuid4()))
-    _logger.info(f"RequestId: {request_id} passed to POST requests")
-    return request_id
-
-
-def _get_bucket_name() -> str:
-    """Returns the mds bucket name for s3 upload"""
-    return os.getenv("MDS_BUCKET_NAME", "velo-notebook-output-prod-us-east-1")
-
-
-def _create_feed_body() -> Dict:
-    """Creates the post body which is used to call the MDS api when creating a feed id"""
-    body = {
-        "userId": _get_user_id(),
-        "userName": _get_user_id(),
-        "jobName": _get_job_name(),
-        "jobMetaData": {
-            "jobRunUrl": "place_holder",
-            "jobRunMethod": "place_holder",
-            "jobPostBody": {
-                "appInput": {
-                    "notebookParameters": {"bucket": _get_bucket_name()},
-                },
-            },
-        },
-    }
-    return body
-
-
-def _get_mds_base_url() -> str:
-    return f"{_config.mds_api_url()}"
-
-
-def _get_al_proxy_base_url() -> str:
-    return f"{_config.al_proxy_api_url()}"
-
-
-def _encrypt_ftp_password(password: str) -> str:
-    """Takes a password and encrypts it using the user_id as the salt"""
-    _api_backend = DeliveryAPIBackend()
-    url = f"{_get_al_proxy_base_url()}encrypt-message"
-    data = {"message": password, "salt": _get_user_id()}
-    try:
-        _logger.info(f"Calling {url} to encrypt ftp password")
-        response_json = _api_backend.do_post_request(url, data=json.dumps(data, ignore_nan=True))
-        encrypted_password: str = response_json["encrypted_message"]
-        return encrypted_password
-    except Exception:
-        _logger.error("Could not encrypt password using /encrypt-message")
-        raise
-
-
-def _create_deliver_body(output_file_name: str, config: DeliveryConfig, delivered_file_name: Optional[str] = None) -> Dict:
-    """Creates the post body which is used to call the MDS delivery api"""
-    body = {
-        "userId": _get_user_id(),
-        "userName": _get_user_id(),
-        "jobName": _get_job_name(),
-        "s3key": output_file_name,
-    }
-    if delivered_file_name:
-        body["fileName"] = delivered_file_name
-    if config.method == DeliveryType.EMAIL:
-        body["deliveryInfos"] = {  # type: ignore
-            "emails": [
-                {
-                    "address": config.email_address,
-                },
-            ]
-        }
-    elif config.method == DeliveryType.DELIVERY_PROFILE:
-        body["deliveryInfos"] = {  # type: ignore
-            "profiles": [
-                {
-                    "deliveryProfileId": config.delivery_profile_id,
-                },
-            ]
-        }
-    elif config.method == DeliveryType.FTP:
-        body["deliveryInfos"] = {  # type: ignore
-            "ftps": [
-                {
-                    "server": config.server,
-                    "username": config.user_name,
-                    "password": _encrypt_ftp_password(config.password),
-                    "folder": config.folder,
-                },
-            ]
-        }
-    return body
-
-
-def _create_output_file_name(file_path: str) -> str:
-    """Creates the output file name for the file which will be uploaded to MDS s3 bucket"""
-    file_name = pathlib.Path(file_path).name
-    return f"{uuid.uuid4()}-{file_name}"
-
-
-def _retrieve_credentials() -> Dict[str, str]:
-    """Retrieves the credentials required to access the MDS s3 bucket"""
-    _api_backend = DeliveryAPIBackend()
-    url = f"{_get_al_proxy_base_url()}assume-mds-role?user_id={_get_user_id()}"
-    try:
-        _logger.info(f"Calling {url} to get assume role credentials")
-        response_json: Dict[str, str] = _api_backend.do_get_request(url)
-        return response_json
-    except ForbiddenError:
-        _logger.error(f"Unable to retrieve credentials for MDS s3 bucket upload")
-        _logger.error(f"User does not have access to deliver function feature")
-        raise UnauthorizedDeliveryException from None
-
-
-def _get_mds_bucket() -> boto3.session.Session.resource:
-    """Returns the MDS bucket where we will upload the file before calling the delivery endpoint"""
-    credentials = _retrieve_credentials()
-    s3_resource = boto3.resource(
-        "s3",
-        aws_access_key_id=credentials["AccessKeyId"],
-        aws_secret_access_key=credentials["SecretAccessKey"],
-        aws_session_token=credentials["SessionToken"],
-    )
-    bucket = s3_resource.Bucket(_get_bucket_name())
-    return bucket
-
-
-def _validate_file_name(file_name: str) -> bool:
-    """Checks if the file name used for the delivered file is valid"""
-    matches = _invalid_chars_regex.findall(file_name)
-    if matches:
-        error_message = f"File name: {file_name} is invalid. The following can't be used in the file name: '{matches}'"
-        raise BadRequestException(error_message)
-    return True
+import simplejson as json
+import logging
+import os
+import re
+import pathlib
+import string
+import uuid
+from typing import Dict, Optional
+
+import boto3
+import jwt
+import requests
+from urllib3.exceptions import InsecureRequestWarning
+
+from ..direct._exceptions import ForbiddenError
+from ._delivery_config import DeliveryConfig, DeliveryType
+from ..direct._config import _Config
+
+from ..direct._backend_apis import DeliveryAPIBackend
+from ..direct._exceptions import BadRequestException, UnauthorizedDeliveryException
+
+# NOTE: We are not able to verify the SSL cert on MDS API since
+#       the VPC endpoint domain name is not on the server's SSL cert.
+#       So with a heavy heart, we disable the InsecureRequestWarning
+requests.packages.urllib3.disable_warnings(category=InsecureRequestWarning)
+
+
+_logger = logging.getLogger(__name__)
+_config = _Config()
+
+# A filename can include 'a-z', 'A-Z', '0-9', '-', '_', '(', ')', ' ', '.'
+_invalid_chars_regex = re.compile(r"[^a-zA-Z\d\-_\(\)\ .]")
+
+
+def _get_user_id_from_uim_token() -> str:
+    """Returns the user's id by decoding their UIM token"""
+    try:
+        md_auth_token = md_auth_token = os.getenv("MD_AUTH_TOKEN", os.getenv("UIM_JWT", ""))
+        decode_key = os.getenv("UIM_DECODE_KEY", "https://login-prod.morningstar.com/.well-known/jwks.json")
+        jwks_client = jwt.jwks_client.PyJWKClient(decode_key)
+        signing_key = jwks_client.get_signing_key_from_jwt(md_auth_token)
+        decoded_jwt = jwt.decode(
+            md_auth_token,
+            signing_key.key,
+            algorithms=["RS256"],
+            options={"verify_signature": True, "verify_exp": True, "verify_aud": False},
+            leeway=60,
+        )
+        user_id: str = decoded_jwt["sub"].split("|")[1]
+        return user_id.upper()
+    except Exception as err:
+        _logger.error(f"Error decoding MD_AUTH_TOKEN: {err}")
+        raise
+
+
+def _get_user_id_from_eams_token() -> str:
+    """Returns the user's id by decoding their EAMS token"""
+    try:
+        key = os.getenv("EAMS_PUBLIC_KEY", "").replace("\\n", "\n")
+        token = os.getenv("EAMS_JWT")
+        decoded = jwt.decode(token, key, algorithms=["RS256"])
+        user_id: str = decoded["sub"]
+        return user_id.upper()
+    except Exception as err:
+        _logger.error(f"Error decoding EAMS token: {err}")
+        raise
+
+
+def _get_user_id() -> str:
+    """Returns the user's id using their UIM token if it exists, EAMS token otherwise"""
+    try:
+        user_id = _get_user_id_from_uim_token()
+        _logger.info(f"Using UIM token for User ID: {user_id}")
+        return user_id
+    except Exception:
+        pass
+
+    user_id = _get_user_id_from_eams_token()
+    _logger.info(f"Using EAMS token for User ID: {user_id}")
+    return user_id
+
+
+def _get_job_name() -> str:
+    """Returns the job name for a feed or delivery"""
+    return str(uuid.uuid4())
+
+
+def _get_request_id() -> str:
+    """Returns the request id for use in POST requests"""
+    request_id = os.getenv("REQUEST_ID", str(uuid.uuid4()))
+    _logger.info(f"RequestId: {request_id} passed to POST requests")
+    return request_id
+
+
+def _get_bucket_name() -> str:
+    """Returns the mds bucket name for s3 upload"""
+    return os.getenv("MDS_BUCKET_NAME", "velo-notebook-output-prod-us-east-1")
+
+
+def _create_feed_body() -> Dict:
+    """Creates the post body which is used to call the MDS api when creating a feed id"""
+    body = {
+        "userId": _get_user_id(),
+        "userName": _get_user_id(),
+        "jobName": _get_job_name(),
+        "jobMetaData": {
+            "jobRunUrl": "place_holder",
+            "jobRunMethod": "place_holder",
+            "jobPostBody": {
+                "appInput": {
+                    "notebookParameters": {"bucket": _get_bucket_name()},
+                },
+            },
+        },
+    }
+    return body
+
+
+def _get_mds_base_url() -> str:
+    return f"{_config.mds_api_url()}"
+
+
+def _get_al_proxy_base_url() -> str:
+    return f"{_config.al_proxy_api_url()}"
+
+
+def _encrypt_ftp_password(password: str) -> str:
+    """Takes a password and encrypts it using the user_id as the salt"""
+    _api_backend = DeliveryAPIBackend()
+    url = f"{_get_al_proxy_base_url()}encrypt-message"
+    data = {"message": password, "salt": _get_user_id()}
+    try:
+        _logger.info(f"Calling {url} to encrypt ftp password")
+        response_json = _api_backend.do_post_request(url, data=json.dumps(data, ignore_nan=True))
+        encrypted_password: str = response_json["encrypted_message"]
+        return encrypted_password
+    except Exception:
+        _logger.error("Could not encrypt password using /encrypt-message")
+        raise
+
+
+def _create_deliver_body(output_file_name: str, config: DeliveryConfig, delivered_file_name: Optional[str] = None) -> Dict:
+    """Creates the post body which is used to call the MDS delivery api"""
+    body = {
+        "userId": _get_user_id(),
+        "userName": _get_user_id(),
+        "jobName": _get_job_name(),
+        "s3key": output_file_name,
+    }
+    if delivered_file_name:
+        body["fileName"] = delivered_file_name
+    if config.method == DeliveryType.EMAIL:
+        body["deliveryInfos"] = {  # type: ignore
+            "emails": [
+                {
+                    "address": config.email_address,
+                },
+            ]
+        }
+    elif config.method == DeliveryType.DELIVERY_PROFILE:
+        body["deliveryInfos"] = {  # type: ignore
+            "profiles": [
+                {
+                    "deliveryProfileId": config.delivery_profile_id,
+                },
+            ]
+        }
+    elif config.method == DeliveryType.FTP:
+        body["deliveryInfos"] = {  # type: ignore
+            "ftps": [
+                {
+                    "server": config.server,
+                    "username": config.user_name,
+                    "password": _encrypt_ftp_password(config.password),
+                    "folder": config.folder,
+                },
+            ]
+        }
+    return body
+
+
+def _create_output_file_name(file_path: str) -> str:
+    """Creates the output file name for the file which will be uploaded to MDS s3 bucket"""
+    file_name = pathlib.Path(file_path).name
+    return f"{uuid.uuid4()}-{file_name}"
+
+
+def _retrieve_credentials() -> Dict[str, str]:
+    """Retrieves the credentials required to access the MDS s3 bucket"""
+    _api_backend = DeliveryAPIBackend()
+    url = f"{_get_al_proxy_base_url()}assume-mds-role?user_id={_get_user_id()}"
+    try:
+        _logger.info(f"Calling {url} to get assume role credentials")
+        response_json: Dict[str, str] = _api_backend.do_get_request(url)
+        return response_json
+    except ForbiddenError:
+        _logger.error(f"Unable to retrieve credentials for MDS s3 bucket upload")
+        _logger.error(f"User does not have access to deliver function feature")
+        raise UnauthorizedDeliveryException from None
+
+
+def _get_mds_bucket() -> boto3.session.Session.resource:
+    """Returns the MDS bucket where we will upload the file before calling the delivery endpoint"""
+    credentials = _retrieve_credentials()
+    s3_resource = boto3.resource(
+        "s3",
+        aws_access_key_id=credentials["AccessKeyId"],
+        aws_secret_access_key=credentials["SecretAccessKey"],
+        aws_session_token=credentials["SessionToken"],
+    )
+    bucket = s3_resource.Bucket(_get_bucket_name())
+    return bucket
+
+
+def _validate_file_name(file_name: str) -> bool:
+    """Checks if the file name used for the delivered file is valid"""
+    matches = _invalid_chars_regex.findall(file_name)
+    if matches:
+        error_message = f"File name: {file_name} is invalid. The following can't be used in the file name: '{matches}'"
+        raise BadRequestException(error_message)
+    return True
```

### Comparing `morningstar_data-1.2.0/morningstar_data/utils/delivery.py` & `morningstar_data-1.3.0/morningstar_data/utils/delivery.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,256 +1,256 @@
-import simplejson as json
-import logging
-import os
-from typing import Dict, Any, Optional
-import polling2
-
-from botocore.exceptions import ClientError
-from ..direct._backend_apis import DeliveryAPIBackend
-
-from ._delivery_config import DeliveryConfig
-from ._helpers import _get_mds_base_url, _get_mds_bucket, _create_deliver_body, _create_feed_body, _create_output_file_name, _validate_file_name
-from ..direct import _decorator
-
-_logger = logging.getLogger(__name__)
-_api_backend = DeliveryAPIBackend()
-
-
-def _create_feed_id() -> int:
-    """Calls the MDS feeds api to generate a new feed id.
-
-    This feed id is needed when calling the MDS deliver api. In general, when a notebook is running
-    in a schedule it will be passed in this feed id. But for an ad-hoc delivery this feed id needs
-    to be created before the MDS delivery api can be called.
-    """
-    _logger.info("Creating a feed id using MDS api")
-    url = f"{_get_mds_base_url()}v1/feeds?type=notebook"
-    data = _create_feed_body()
-
-    try:
-        _logger.info(f"Calling MDS /feeds endpoint with: {data}")
-        response_json = _api_backend.do_post_request(url, data=json.dumps(data, ignore_nan=True))
-        feed_id: int = response_json["feedId"]
-        return feed_id
-    except Exception:
-        _logger.error("Could not create a feed id using MDS api")
-        raise
-
-
-def _upload_to_s3(file_path: str, output_file_name: str) -> None:
-    """Uploads a file to the MDS s3 bucket"""
-    try:
-        output_bucket = _get_mds_bucket()
-        output_bucket.upload_file(file_path, output_file_name)
-    except FileNotFoundError:
-        _logger.error(f"File not found: {file_path}, make sure the file you are trying to upload exists")
-        raise
-    except ClientError:
-        _logger.error("Could not upload to s3 bucket due to AWS error")
-        raise
-    except Exception:
-        _logger.error("Could not upload to s3 bucket")
-        raise
-
-
-def _mds_deliver_file(output_file_name: str, config: DeliveryConfig, feed_id: int, delivered_file_name: Optional[str] = None) -> str:
-    """Calls the MDS delivery api with the needed information to deliver the uploaded file and returns job_id"""
-    url = f"{_get_mds_base_url()}v1/delivery/{feed_id}"
-    data = _create_deliver_body(output_file_name, config, delivered_file_name)
-    _logger.info(f"Calling MDS /delivery/{feed_id} endpoint with: {data}")
-    response_json = _api_backend.do_post_request(url, data=json.dumps(data, ignore_nan=True))
-    _logger.info(f"Delivery response: {response_json}")
-    job_id: str = response_json["jobId"]
-    return job_id
-
-
-@_decorator.typechecked
-def get_delivery_profile() -> Dict:
-    """Fetch ftp delivery profiles using MDS API
-    Returns:
-        :obj:`dict`: FTP delivery profiles for the user.
-    """
-    url = f"{_get_mds_base_url()}v1/delivery-profile"
-    _logger.info(f"Calling MDS /delivery-profile endpoint. ")
-    mds_delivery_profiles: Dict[Any, Any] = _api_backend.do_get_request(url)
-    _logger.info(f"MDS delivery profile response: {mds_delivery_profiles}")
-    ftp_delivery_profiles = {"ftps": mds_delivery_profiles.get("ftps", [])}
-    return ftp_delivery_profiles
-
-
-@_decorator.typechecked
-def delivery_status(job_id: str, poll: bool = True) -> str:
-    """Polls the MDS delivery api with the job_id to check the delivery status.
-    Args:
-        job_id (:obj:`str`): The job id that we get from MDS endpoint
-        poll (:obj:`bool`): Flag to poll the endpoint or not (default is set as True,
-        as we want to poll the endpoint to get the status)
-
-    Returns:
-        :obj:`str`: Delivery status as given by the endpoint.
-    """
-    url = f"{_get_mds_base_url()}v1/jobs/{job_id}/status"
-    _logger.info(f"Calling MDS /delivery/{job_id}/status endpoint")
-
-    # polling the endpoint till it gets status response; raise exception error if occurred
-    def _delivery_finished(res: dict) -> bool:
-        try:
-            return res["jobStatus"].lower() in ["done", "failed"]
-        except KeyError as e:
-            _logger.error(f"Could not find delivery status. Exception as {e}")
-            raise
-
-    if poll:
-        _logger.info(f"Polling the request to get the delivery status.")
-        try:
-            polling2.poll(
-                lambda: _api_backend.do_get_request(url),
-                step=5,
-                timeout=60,
-                check_success=lambda response: _delivery_finished(response),
-            )
-        except polling2.TimeoutException as te:
-            _logger.info(f"Timeout for the request. Exception as {te}.")
-
-    response_json = _api_backend.do_get_request(url)
-    _logger.info(f"Delivery status: {response_json}")
-    return str(response_json["jobStatus"])  # "DONE" or "FAILED" or "RUNNING"
-
-
-@_decorator.typechecked
-def deliver(file_path: str, config: DeliveryConfig, wait_for_delivery: bool = False, delivered_file_name: Optional[str] = None) -> dict:
-    """
-    :bdg-ref-danger:`Upcoming Feature <../upcoming_feature>`
-
-    Delivers a file from a notebook to an email or FTP.
-
-    Args:
-        file_path (:obj:`str`): The path to the file that will be delivered, including file name and extension.
-        config (:obj:`md.utils.DeliveryConfig`): An object that holds the delivery configuration information.
-
-            For an email it contains
-                * method (:obj:`DeliveryType`): DeliveryType.EMAIL in this case.
-                * email_address (:obj:`str`): email_address to send the file to.
-            For FTP it contains
-                * method (:obj:`DeliveryType`): DeliveryType.FTP in this case.
-                * user_name (:obj:`str`): the user_name to login to the ftp server.
-                * password (:obj:`str`): the password to login to the ftp server.
-                * server (:obj:`str`): the ftp server to use.
-                * folder (:obj:`str`): the folder on the ftp server to upload the file to.
-            For a Delivery Profile it contains
-                * method (:obj:`DeliveryType`): DeliveryType.DELIVERY_PROFILE in this case.
-                * delivery_profile_id (:obj:`str`): delivery_profile_id that was setup by MDS. Can be retrieved with get_delivery_profile()
-        wait_for_delivery (:obj:`bool`): Flag to poll the api to check the delivery status or not. (True=show status)
-        delivered_file_name (:obj:`Optional[str]`): An optional parameter for the user to specify the file name to be used when
-            delivered. No file extension should be provided. Valid characters are `., -, _, (, ), , a-z, A-Z, 0-9`. If the file
-            name includes non-valid characters, an exception will be raised.
-
-    Returns:
-        :obj:`dict`: A dictionary with the 'job_id', 'message', 'delivery_status' keys containing information about the delivery status
-
-    :Examples:
-
-    Deliver to an email address.
-
-    ::
-
-        import morningstar_data as md
-        import pandas as pd
-
-        df = pd.DataFrame({'a':[1], 'b':[2]})
-        df.to_csv("test_export.csv")
-
-        # Email example
-        delivery_config = md.utils.DeliveryConfig(method=md.utils.DeliveryType.EMAIL, email_address="test@email.com")
-        md.utils.deliver("test_export.csv", delivery_config)
-
-    Deliver to a ftp server.
-
-    ::
-
-        import morningstar_data as md
-        import pandas as pd
-
-        df = pd.DataFrame({'a':[1], 'b':[2]})
-        df.to_csv("test_export.csv")
-
-        # FTP example
-        delivery_config = md.utils.DeliveryConfig(method=md.utils.DeliveryType.FTP, user_name="test", password="test", server="ts.ftp.com", folder="data/")
-        md.utils.deliver("test_export.csv", delivery_config)
-
-    Deliver to a Delivery Profile
-
-    ::
-
-        import morningstar_data as md
-        import pandas as pd
-
-        df = pd.DataFrame({'a':[1], 'b':[2]})
-        df.to_csv("test_export.csv")
-
-        # Delivery Profile example
-        delivery_config = md.utils.DeliveryConfig(method=md.utils.DeliveryType.DELIVERY_PROFILE, delivery_profile_id="1234")
-        md.utils.deliver("test_export.csv", delivery_config)
-
-    Multiple delivery within a single notebook.
-
-    ::
-
-        import morningstar_data as md
-        import pandas as pd
-
-        df = pd.DataFrame({'a':[1], 'b':[2]})
-        df.to_csv("test_export.csv")
-
-        ftp_delivery_config = md.utils.DeliveryConfig(method=md.utils.DeliveryType.FTP, user_name="test", password="test", server="ts.ftp.com", folder="data/")
-        md.utils.deliver("test_export.csv", ftp_delivery_config)
-
-        email_delivery_config = md.utils.DeliveryConfig(method=md.utils.DeliveryType.EMAIL, email_address="test@email.com")
-        md.utils.deliver("test_export.csv", email_delivery_config)
-
-    Deliver with a specific filename.
-
-    ::
-
-        import morningstar_data as md
-        import pandas as pd
-
-        df = pd.DataFrame({'a':[1], 'b':[2]})
-        df.to_csv("test_export.csv")
-
-        # Email example
-        delivery_config = md.utils.DeliveryConfig(method=md.utils.DeliveryType.EMAIL, email_address="test@email.com")
-        md.utils.deliver("test_export.csv", delivery_config, delivered_file_name="Delivered_Dataframe_123")
-        # File delivered will be named "Delivered_Dataframe_123.csv"
-
-    Errors:
-        AccessDeniedError: Raised when the user is not authenticated.
-
-        UnauthorizedDeliveryException: Raised when the user does not have permissions to deliver artifacts.
-
-        BadRequestError: Raised when the user does not provide a properly formatted request.
-
-        InternalServerError: Raised when the server encounters an unhandled error.
-
-        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
-
-        FileNotFoundError: Raised when the file path specified to be delivered does not exist
-    """
-    if delivered_file_name:
-        _validate_file_name(delivered_file_name)
-
-    # Check for a feed_id, create one if not specified
-    try:
-        feed_id = int(os.environ["FEED_ID"])
-    except KeyError:
-        feed_id = _create_feed_id()
-
-    output_file_name = _create_output_file_name(file_path)
-
-    _upload_to_s3(file_path, output_file_name)
-    job_id: str = _mds_deliver_file(output_file_name, config, feed_id, delivered_file_name)
-
-    res = {"job_id": job_id, "message": "Delivery has been submitted."}
-
-    # if flag is set True, poll the api, return the delivery status
-    res["delivery_status"] = delivery_status(job_id, poll=wait_for_delivery)
-    return res
+import simplejson as json
+import logging
+import os
+from typing import Dict, Any, Optional
+import polling2
+
+from botocore.exceptions import ClientError
+from ..direct._backend_apis import DeliveryAPIBackend
+
+from ._delivery_config import DeliveryConfig
+from ._helpers import _get_mds_base_url, _get_mds_bucket, _create_deliver_body, _create_feed_body, _create_output_file_name, _validate_file_name
+from ..direct import _decorator
+
+_logger = logging.getLogger(__name__)
+_api_backend = DeliveryAPIBackend()
+
+
+def _create_feed_id() -> int:
+    """Calls the MDS feeds api to generate a new feed id.
+
+    This feed id is needed when calling the MDS deliver api. In general, when a notebook is running
+    in a schedule it will be passed in this feed id. But for an ad-hoc delivery this feed id needs
+    to be created before the MDS delivery api can be called.
+    """
+    _logger.info("Creating a feed id using MDS api")
+    url = f"{_get_mds_base_url()}v1/feeds?type=notebook"
+    data = _create_feed_body()
+
+    try:
+        _logger.info(f"Calling MDS /feeds endpoint with: {data}")
+        response_json = _api_backend.do_post_request(url, data=json.dumps(data, ignore_nan=True))
+        feed_id: int = response_json["feedId"]
+        return feed_id
+    except Exception:
+        _logger.error("Could not create a feed id using MDS api")
+        raise
+
+
+def _upload_to_s3(file_path: str, output_file_name: str) -> None:
+    """Uploads a file to the MDS s3 bucket"""
+    try:
+        output_bucket = _get_mds_bucket()
+        output_bucket.upload_file(file_path, output_file_name)
+    except FileNotFoundError:
+        _logger.error(f"File not found: {file_path}, make sure the file you are trying to upload exists")
+        raise
+    except ClientError:
+        _logger.error("Could not upload to s3 bucket due to AWS error")
+        raise
+    except Exception:
+        _logger.error("Could not upload to s3 bucket")
+        raise
+
+
+def _mds_deliver_file(output_file_name: str, config: DeliveryConfig, feed_id: int, delivered_file_name: Optional[str] = None) -> str:
+    """Calls the MDS delivery api with the needed information to deliver the uploaded file and returns job_id"""
+    url = f"{_get_mds_base_url()}v1/delivery/{feed_id}"
+    data = _create_deliver_body(output_file_name, config, delivered_file_name)
+    _logger.info(f"Calling MDS /delivery/{feed_id} endpoint with: {data}")
+    response_json = _api_backend.do_post_request(url, data=json.dumps(data, ignore_nan=True))
+    _logger.info(f"Delivery response: {response_json}")
+    job_id: str = response_json["jobId"]
+    return job_id
+
+
+@_decorator.typechecked
+def get_delivery_profile() -> Dict:
+    """Fetch ftp delivery profiles using MDS API
+    Returns:
+        :obj:`dict`: FTP delivery profiles for the user.
+    """
+    url = f"{_get_mds_base_url()}v1/delivery-profile"
+    _logger.info(f"Calling MDS /delivery-profile endpoint. ")
+    mds_delivery_profiles: Dict[Any, Any] = _api_backend.do_get_request(url)
+    _logger.info(f"MDS delivery profile response: {mds_delivery_profiles}")
+    ftp_delivery_profiles = {"ftps": mds_delivery_profiles.get("ftps", [])}
+    return ftp_delivery_profiles
+
+
+@_decorator.typechecked
+def delivery_status(job_id: str, poll: bool = True) -> str:
+    """Polls the MDS delivery api with the job_id to check the delivery status.
+    Args:
+        job_id (:obj:`str`): The job id that we get from MDS endpoint
+        poll (:obj:`bool`): Flag to poll the endpoint or not (default is set as True,
+        as we want to poll the endpoint to get the status)
+
+    Returns:
+        :obj:`str`: Delivery status as given by the endpoint.
+    """
+    url = f"{_get_mds_base_url()}v1/jobs/{job_id}/status"
+    _logger.info(f"Calling MDS /delivery/{job_id}/status endpoint")
+
+    # polling the endpoint till it gets status response; raise exception error if occurred
+    def _delivery_finished(res: dict) -> bool:
+        try:
+            return res["jobStatus"].lower() in ["done", "failed"]
+        except KeyError as e:
+            _logger.error(f"Could not find delivery status. Exception as {e}")
+            raise
+
+    if poll:
+        _logger.info(f"Polling the request to get the delivery status.")
+        try:
+            polling2.poll(
+                lambda: _api_backend.do_get_request(url),
+                step=5,
+                timeout=60,
+                check_success=lambda response: _delivery_finished(response),
+            )
+        except polling2.TimeoutException as te:
+            _logger.info(f"Timeout for the request. Exception as {te}.")
+
+    response_json = _api_backend.do_get_request(url)
+    _logger.info(f"Delivery status: {response_json}")
+    return str(response_json["jobStatus"])  # "DONE" or "FAILED" or "RUNNING"
+
+
+@_decorator.typechecked
+def deliver(file_path: str, config: DeliveryConfig, wait_for_delivery: bool = False, delivered_file_name: Optional[str] = None) -> dict:
+    """
+    :bdg-ref-danger:`Upcoming Feature <../upcoming_feature>`
+
+    Delivers a file from a notebook to an email or FTP.
+
+    Args:
+        file_path (:obj:`str`): The path to the file that will be delivered, including file name and extension.
+        config (:obj:`md.utils.DeliveryConfig`): An object that holds the delivery configuration information.
+
+            For an email it contains
+                * method (:obj:`DeliveryType`): DeliveryType.EMAIL in this case.
+                * email_address (:obj:`str`): email_address to send the file to.
+            For FTP it contains
+                * method (:obj:`DeliveryType`): DeliveryType.FTP in this case.
+                * user_name (:obj:`str`): the user_name to login to the ftp server.
+                * password (:obj:`str`): the password to login to the ftp server.
+                * server (:obj:`str`): the ftp server to use.
+                * folder (:obj:`str`): the folder on the ftp server to upload the file to.
+            For a Delivery Profile it contains
+                * method (:obj:`DeliveryType`): DeliveryType.DELIVERY_PROFILE in this case.
+                * delivery_profile_id (:obj:`str`): delivery_profile_id that was setup by MDS. Can be retrieved with get_delivery_profile()
+        wait_for_delivery (:obj:`bool`): Flag to poll the api to check the delivery status or not. (True=show status)
+        delivered_file_name (:obj:`Optional[str]`): An optional parameter for the user to specify the file name to be used when
+            delivered. No file extension should be provided. Valid characters are `., -, _, (, ), , a-z, A-Z, 0-9`. If the file
+            name includes non-valid characters, an exception will be raised.
+
+    Returns:
+        :obj:`dict`: A dictionary with the 'job_id', 'message', 'delivery_status' keys containing information about the delivery status
+
+    :Examples:
+
+    Deliver to an email address.
+
+    ::
+
+        import morningstar_data as md
+        import pandas as pd
+
+        df = pd.DataFrame({'a':[1], 'b':[2]})
+        df.to_csv("test_export.csv")
+
+        # Email example
+        delivery_config = md.utils.DeliveryConfig(method=md.utils.DeliveryType.EMAIL, email_address="test@email.com")
+        md.utils.deliver("test_export.csv", delivery_config)
+
+    Deliver to a ftp server.
+
+    ::
+
+        import morningstar_data as md
+        import pandas as pd
+
+        df = pd.DataFrame({'a':[1], 'b':[2]})
+        df.to_csv("test_export.csv")
+
+        # FTP example
+        delivery_config = md.utils.DeliveryConfig(method=md.utils.DeliveryType.FTP, user_name="test", password="test", server="ts.ftp.com", folder="data/")
+        md.utils.deliver("test_export.csv", delivery_config)
+
+    Deliver to a Delivery Profile
+
+    ::
+
+        import morningstar_data as md
+        import pandas as pd
+
+        df = pd.DataFrame({'a':[1], 'b':[2]})
+        df.to_csv("test_export.csv")
+
+        # Delivery Profile example
+        delivery_config = md.utils.DeliveryConfig(method=md.utils.DeliveryType.DELIVERY_PROFILE, delivery_profile_id="1234")
+        md.utils.deliver("test_export.csv", delivery_config)
+
+    Multiple delivery within a single notebook.
+
+    ::
+
+        import morningstar_data as md
+        import pandas as pd
+
+        df = pd.DataFrame({'a':[1], 'b':[2]})
+        df.to_csv("test_export.csv")
+
+        ftp_delivery_config = md.utils.DeliveryConfig(method=md.utils.DeliveryType.FTP, user_name="test", password="test", server="ts.ftp.com", folder="data/")
+        md.utils.deliver("test_export.csv", ftp_delivery_config)
+
+        email_delivery_config = md.utils.DeliveryConfig(method=md.utils.DeliveryType.EMAIL, email_address="test@email.com")
+        md.utils.deliver("test_export.csv", email_delivery_config)
+
+    Deliver with a specific filename.
+
+    ::
+
+        import morningstar_data as md
+        import pandas as pd
+
+        df = pd.DataFrame({'a':[1], 'b':[2]})
+        df.to_csv("test_export.csv")
+
+        # Email example
+        delivery_config = md.utils.DeliveryConfig(method=md.utils.DeliveryType.EMAIL, email_address="test@email.com")
+        md.utils.deliver("test_export.csv", delivery_config, delivered_file_name="Delivered_Dataframe_123")
+        # File delivered will be named "Delivered_Dataframe_123.csv"
+
+    Errors:
+        AccessDeniedError: Raised when the user is not authenticated.
+
+        UnauthorizedDeliveryException: Raised when the user does not have permissions to deliver artifacts.
+
+        BadRequestError: Raised when the user does not provide a properly formatted request.
+
+        InternalServerError: Raised when the server encounters an unhandled error.
+
+        NetworkExceptionError: Raised when the request fails to reach the server due to a network error.
+
+        FileNotFoundError: Raised when the file path specified to be delivered does not exist
+    """
+    if delivered_file_name:
+        _validate_file_name(delivered_file_name)
+
+    # Check for a feed_id, create one if not specified
+    try:
+        feed_id = int(os.environ["FEED_ID"])
+    except KeyError:
+        feed_id = _create_feed_id()
+
+    output_file_name = _create_output_file_name(file_path)
+
+    _upload_to_s3(file_path, output_file_name)
+    job_id: str = _mds_deliver_file(output_file_name, config, feed_id, delivered_file_name)
+
+    res = {"job_id": job_id, "message": "Delivery has been submitted."}
+
+    # if flag is set True, poll the api, return the delivery status
+    res["delivery_status"] = delivery_status(job_id, poll=wait_for_delivery)
+    return res
```

### Comparing `morningstar_data-1.2.0/pyproject.toml` & `morningstar_data-1.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-[tool.poetry]
-name = "morningstar_data"
-version = "1.2.0"
-description = "Morningstar Data"
-authors = ["Morningstar, Inc."]
-readme = "README.md"
-license = "Apache-2.0"
-homepage = "https://www.morningstar.com/products/md-python-package"
-
-[tool.poetry.dependencies]
-python = "^3.8"
-pandas = "~1.5.3"
-typeguard = "^2.13.3"
-PyJWT = "^2.4.0"
-boto3 = "^1.20.1"
-cryptography = "40.0.2"
-polling2 = "0.5.0"
-tenacity = "^8.2.2"
-simplejson = "^3.18.4"
-requests = "^2.28.2"
-pyopenssl = "^23.1.1"
-
-# We don't use urllib3 directly, but due to some weird interplay between requests and boto3 dependencies,
-# dependency resolution is super slow unless we limit the allowed urllib3 versions.
-# https://github.com/python-poetry/poetry/issues/1116
-urllib3 = "^1.26"
-
-
-[tool.poetry.dev-dependencies]
-mypy = "^0.931"
-pytest = "^6.2.5"
-pytest-cov = "^4.1.0"
-pre-commit = "^2.16.0"
-black = "^21.12b0"
-
-requests_mock = "^1.8.0"
-Sphinx = "^4.4.0"
-furo = "2021.10.9"
-ipython = "7.31.1"
-pytest-mock = "^3.8.1"
-sphinx-multiversion = "^0.2.4"
-mockito = "^1.2.2"
-boto3-stubs = "^1.26.23"
-moto = "^4.0.11"
-importlib-metadata = "^4.13.0"
-pytest-xdist = "^3.1.0"
-towncrier = "^22.12.0"
-sphinx_design = "0.4.1"
-
-
-[build-system]
-requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.towncrier]
-    package = "morningstar_data"
-    filename = "CHANGELOG.rst"
-    directory = "docs/changelog/"
-    issue_format = "`{issue} <https://msjira.morningstar.com/browse/{issue}>`__"
-    template = "docs/changelog/template.rst"
-
-    [[tool.towncrier.type]]
-        directory = "breaking"
-        name = "Backwards Incompatible Changes"
-        showcontent = true
-
-    [[tool.towncrier.type]]
-        directory = "api"
-        name = "API Changes"
-        showcontent = true
-
-    [[tool.towncrier.type]]
-      directory = "removal"
-      name = "Deprecations and Removals"
-      showcontent = true
-
-    [[tool.towncrier.type]]
-      directory = "feature"
-      name = "Features"
-      showcontent = true
-
-    [[tool.towncrier.type]]
-      directory = "bugfix"
-      name = "Bug Fixes"
-      showcontent = true
-
-    [[tool.towncrier.type]]
-      directory = "doc"
-      name = "Added/Improved Documentation"
-      showcontent = true
-
-    [[tool.towncrier.type]]
-      directory = "docfix"
-      name = "Documentation Fixes"
-      showcontent = true
-
-    [[tool.towncrier.type]]
-      directory = "trivial"
-      name = "Trivial/Internal Changes"
-      showcontent = true
+[tool.poetry]
+name = "morningstar_data"
+version = "1.3.0"
+description = "Morningstar Data"
+authors = ["Morningstar, Inc."]
+readme = "README.md"
+license = "Apache-2.0"
+homepage = "https://www.morningstar.com/products/md-python-package"
+
+[tool.poetry.dependencies]
+python = "^3.8"
+pandas = "~1.5.3"
+typeguard = "^2.13.3"
+PyJWT = "^2.4.0"
+boto3 = "^1.20.1"
+cryptography = "40.0.2"
+polling2 = "0.5.0"
+tenacity = "^8.2.2"
+simplejson = "^3.18.4"
+requests = "^2.28.2"
+pyopenssl = "^23.1.1"
+
+# We don't use urllib3 directly, but due to some weird interplay between requests and boto3 dependencies,
+# dependency resolution is super slow unless we limit the allowed urllib3 versions.
+# https://github.com/python-poetry/poetry/issues/1116
+urllib3 = "^1.26"
+
+
+[tool.poetry.dev-dependencies]
+mypy = "^0.931"
+pytest = "^6.2.5"
+pytest-cov = "^4.1.0"
+pre-commit = "^2.16.0"
+black = "^21.12b0"
+
+requests_mock = "^1.8.0"
+Sphinx = "^4.4.0"
+furo = "2021.10.9"
+ipython = "7.31.1"
+pytest-mock = "^3.8.1"
+sphinx-multiversion = "^0.2.4"
+mockito = "^1.2.2"
+boto3-stubs = "^1.26.23"
+moto = "^4.0.11"
+importlib-metadata = "^4.13.0"
+pytest-xdist = "^3.1.0"
+towncrier = "^22.12.0"
+sphinx_design = "0.4.1"
+
+
+[build-system]
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.towncrier]
+    package = "morningstar_data"
+    filename = "CHANGELOG.rst"
+    directory = "docs/changelog/"
+    issue_format = "`{issue} <https://msjira.morningstar.com/browse/{issue}>`__"
+    template = "docs/changelog/template.rst"
+
+    [[tool.towncrier.type]]
+        directory = "breaking"
+        name = "Backwards Incompatible Changes"
+        showcontent = true
+
+    [[tool.towncrier.type]]
+        directory = "api"
+        name = "API Changes"
+        showcontent = true
+
+    [[tool.towncrier.type]]
+      directory = "removal"
+      name = "Deprecations and Removals"
+      showcontent = true
+
+    [[tool.towncrier.type]]
+      directory = "feature"
+      name = "Features"
+      showcontent = true
+
+    [[tool.towncrier.type]]
+      directory = "bugfix"
+      name = "Bug Fixes"
+      showcontent = true
+
+    [[tool.towncrier.type]]
+      directory = "doc"
+      name = "Added/Improved Documentation"
+      showcontent = true
+
+    [[tool.towncrier.type]]
+      directory = "docfix"
+      name = "Documentation Fixes"
+      showcontent = true
+
+    [[tool.towncrier.type]]
+      directory = "trivial"
+      name = "Trivial/Internal Changes"
+      showcontent = true
```

### Comparing `morningstar_data-1.2.0/README.md` & `morningstar_data-1.3.0/README.md`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-# Morningstar Data Package
-
-The morningstar_data Python package provides users quick programmatic access to Morningstar data. It is a building block for doing practical investment data analysis in Python.
-
-# Getting Started
-
-## Installation
-
-```
-pip install morningstar-data
-```
-
-**Warning**: Importing the package before authenticating will produce an error. See below for authentication steps.
-
-## Authentication
-### Retrieve Authentication Token
-1. Open [Analytics Lab](https://analyticslab.morningstar.com/) in your browser
-2. Login with your Morningstar Direct credentials
-3. On the top ribbon in the "Analytics Lab" dropdown menu select "Copy Authentication Token". This will copy your token to the clipboard.
-
-![copy auth token](https://al-morningstar-readme-images-temp.s3.amazonaws.com/copy_auth_token.png)
-
-### Set Authentication Token
-Set the environment variable `MD_AUTH_TOKEN`using the token you retrieved previously
-#### Bash
-
-`export MD_AUTH_TOKEN="paste copied token here"`
-
-#### Within a Python (.py) File
-
-```
-# testing_morningstar_data.py
-import os
-
-os.environ['MD_AUTH_TOKEN']="paste copied token here"
-
-import morningstar_data as md
-```
-**Note:** importing morningstar_data comes **after** setting the authentication token
-
-## Requirements
-
-The morningstar_data package is tested with
-
-|             | Main version (latest)
-|-------------|------------------------------|
-| Python      | 3.8, 3.9, 3.10, 3.11         |
-| Pandas      | 1.5                          |
-
-
-## Using the API
-
-This is an example of retrieving data for a saved investment list and data set from Morningstar Direct. See more usage examples in the Python package [documentation](https://docs-analyticslab.morningstar.com/latest/index.html) and tutorial notebooks in [Analytics Lab](https://analyticslab.morningstar.com/).
-
-```
-# Define investments by retrieving your saved lists
-lists = md.direct.user_items.get_investment_lists()
-
-| id                                   | name                                       |
-|--------------------------------------|--------------------------------------------|
-| 8CA07FB7-DFFE-4440-9ED7-6498CC074F11 | Morningstar Prospects                      |
-| AE322592-5A3E-4B31-B889-16D8E76F48D3 | Sustainable Landscape U.S. Funds Q4 2021   |
-| 83D337A2-1CF2-4E66-A94D-2B8EE554AC23 | Sustainable Landscape Global Funds Q4 2021 |
-| ...                                  | ...                                        |
-
-# Specify data points by using one of Morningstar's pre-saved data sets
-morningstar_data_sets = md.direct.lookup.get_morningstar_data_sets()
-
-| datasetId | name                                          |
-|-----------|-----------------------------------------------|
-| 0218-0020 | Snapshot                                      |
-| 0218-0446 | Sustainability: ESG Risk (Company)            |
-| 0218-0481 | Sustainability: Portfolio Sustainability Risk |
-| ...       | ...                                           |
-
-
-# Retrieve data by using the investment list and data set IDs from above
-data = md.direct.get_investment_data(investments=lists["id"][0], data_points=morningstar_data_sets["datasetId"][0])
-
-| Id            | Name                                    | Base Currency | ... |
-|---------------|-----------------------------------------|---------------|-----|
-| F00001AHPT;FO | Hartford Schroders Sustainable Cr Bd I  | US Dollar     | ... |
-| F000014ZNT;FE | iShares ESG Aware Aggressive Allc ETF   | US Dollar     | ... |
-| F00000WUF1;FE | iShares MSCI Global Sust Dev Goals ETF  | US Dollar     | ... |
-| ...           | ...                                     | ...           | ... |
-
-```
-
-### Documentation
-
-Documentation is hosted at https://docs-analyticslab.morningstar.com/latest/index.html
-
-Find the version you are using with `md.__version__`
-
-### Data Retrieval
-
-The Morningstar Data Extension in [Analytics Lab](https://analyticslab.morningstar.com/) is the most convenient tool for locating data points and various saved objects to be used in morningstar_data function calls. You can browse data points, saved investment lists, search criteria, performance reports and more. Drag and drop the object you are interested in into a notebook and the corresponding Python code will be generated for you.
-
-![direct extension](https://al-morningstar-readme-images-temp.s3.amazonaws.com/morningstar_direct_extension.png)
-
-
-# Limits
-
-## Overview of Limits
-
-
-|Type of Limit| Restriction  |
-|-------------|--------------|
-|Limits | Morningstar Direct is exclusively licensed for individual usage. Users of Morningstar Direct are strictly prohibited from disclosing their login credentials, deploying instances of Morningstar Direct on a server, or utilizing, distributing, or redistributing data in a manner contradictory to their organization's agreement with Morningstar. Moreover, Morningstar Direct users are prohibited from employing information in any manner that would contravene the regulations and policies established by third-party providers.|
-|Call Limits | When utilizing the morningstar_data Python package for data extraction, it's important to be aware of the limitations imposed on the number of requests you can make or the amount of data you can receive. These limitations are in place to ensure efficient usage of the resources and maintain the overall performance of the system.|
-|Daily Limits | Limits are in place and can be reached when making requests or receiving data within a single day. These limits are determined either by the number of requests made or the quantity of data received. It is important to keep these limitations in mind while working with the data to ensure compliance and avoid any interruptions in your data processing tasks.|
-|Content Limits |Content limits are governed by entitlements, which are determined by the specific product variant and add-ons purchased. These limits are put in place to regulate the amount of content accessible within the platform. It is important to be aware of these entitlements and ensure they align with your requirements and data processing tasks.|
-
-## Detailed Limits
-
-|Type of Limit| For this Item | Has this limitation|
-|-------------|---------------|--------------------|
-|Daily Limits | Number of Cells per Day | The count of data retrieved from the morningstar_data Python package per day cannot exceed 500,000 cells per day. This count of data is summed across all client applications connected to the same Morningstar Direct instance. In the event you reach your limit, please contact your Sales Representative or Customer Success Manager at Morningstar.|
-|Daily Limits | Number Of investments in an Investment List | The size of an investment list in Morningstar Direct cannot exceed 30,000 investments in a single query.|
-|Daily Limits | Number of data points returned per request |Data point limits are uniform across the type of data being retrieved. That is, the limits apply to time series data, static data, and so on, but are not aggregated across all applications. A custom data set in Morningstar Direct is limited to 1,000 data points.|
-|Content/Entitlement Limits | Third-pary data usage|Additional morningstar_data Python package limitations may be imposed by the providers of the underlying data content. Consult with your Customer Success Manager or Sales Representative to know what third-party provider terms may apply to your use of this data.|
-
-
-## Restricted Functions
-As you refer to the morningstar_data Python package documentation, you may find some utility functions and additional data query functions that are not yet available for use. Such functions are in testing by internal teams at Morningstar, and they will be available to Morningstar Direct clients in the future.
-
-# Usage
-## Usage of Python package
-
-A Python package refers to a specialized computer program that can be imported into a development environment to facilitate easier access to specific Morningstar data and the execution of pre-built functions. It consists of a toolkit comprising a predefined collection of functions that assist users in constructing something with ease and efficiency. The utilization of the morningstar_data Python package is subject to the governance of the Apache 2.0 license. An Authorized User is explicitly prohibited from engaging in activities such as translating, disassembling, or separating components of the Python package (e.g., accessing or acquiring Product code in any manner). The sole means of granting Authorized Users permission to employ and manipulate the Python package is by referencing or providing a separate entitlement to do so. However, this permission must not override any other limitations outlined in the Click License about the utilization or distribution of the Product.
-
-## Extraction of Data using the Python package
-
-Since the functions (i.e., tools) within the morningstar_data package enable users to extract Morningstar data in various ways, it is imperative to ensure that users extract the data within the constraints specified for them and by the distribution licenses held by Morningstar with their respective firms.
-
-## Sharing of Authentication Token
-
-We authenticate a user's access to the morningstar_data package using an authentication token, which remains valid for 24 hours and can solely be obtained from Analytics Lab. Access to Analytics Lab requires possession of a Direct License. Users are strictly prohibited from sharing their authentication tokens with other individuals, as the usage of the product is tethered to the terms and agreements associated with license of Morningstar Direct.
-
-# Terms & Conditions
-The utilization of the morningstar_data Python package entails accessing certain data from Morningstar Direct. Your access and utilization of Morningstar Direct, including its morningstar_data Python package and associated data, are governed by the terms and conditions set forth in your organization’s agreement with Morningstar. Morningstar Direct is an Asset and Wealth management platform that is lawfully licensed for individual use, subject to a login session requirement. A login session is designed to control entitlements and regulate reasonable use for a singular user. To align with the workflow demands of a single user, the morningstar_data Python package imposes restrictions to safeguard the overall platform’s capacity to support the usage levels of all individual Morningstar Direct users accessing data via APIs. The document attached below provides a succinct overview of these various restrictions and elucidates the user experience when encountering them. The specific numerical values for each restriction described herein are not binding and do not create any legal obligations on the part of Morningstar. These restrictions are subject to modification at our sole discretion, without prior notice. It is your sole responsibility to furnish all necessary support pertaining to any applications developed utilizing the morningstar_data Python package. Kindly take note that if you have intentions to resell or distribute any applications or data developed using the morningstar_data Python package to third parties, it is imperative to engage in a distribution license agreement with us. Please contact your Customer Success Manager or Sales Representative at Morningstar for further information.
+# Morningstar Data Package
+
+The morningstar_data Python package provides users quick programmatic access to Morningstar data. It is a building block for doing practical investment data analysis in Python.
+
+# Getting Started
+
+## Installation
+
+```
+pip install morningstar-data
+```
+
+**Warning**: Importing the package before authenticating will produce an error. See below for authentication steps.
+
+## Authentication
+### Retrieve Authentication Token
+1. Open [Analytics Lab](https://analyticslab.morningstar.com/) in your browser
+2. Login with your Morningstar Direct credentials
+3. On the top ribbon in the "Analytics Lab" dropdown menu select "Copy Authentication Token". This will copy your token to the clipboard.
+
+![copy auth token](https://al-morningstar-readme-images-temp.s3.amazonaws.com/copy_auth_token.png)
+
+### Set Authentication Token
+Set the environment variable `MD_AUTH_TOKEN`using the token you retrieved previously
+#### Bash
+
+`export MD_AUTH_TOKEN="paste copied token here"`
+
+#### Within a Python (.py) File
+
+```
+# testing_morningstar_data.py
+import os
+
+os.environ['MD_AUTH_TOKEN']="paste copied token here"
+
+import morningstar_data as md
+```
+**Note:** importing morningstar_data comes **after** setting the authentication token
+
+## Requirements
+
+The morningstar_data package is tested with
+
+|             | Main version (latest)
+|-------------|------------------------------|
+| Python      | 3.8, 3.9, 3.10, 3.11         |
+| Pandas      | 1.5                          |
+
+
+## Using the API
+
+This is an example of retrieving data for a saved investment list and data set from Morningstar Direct. See more usage examples in the Python package [documentation](https://docs-analyticslab.morningstar.com/latest/index.html) and tutorial notebooks in [Analytics Lab](https://analyticslab.morningstar.com/).
+
+```
+# Define investments by retrieving your saved lists
+lists = md.direct.user_items.get_investment_lists()
+
+| id                                   | name                                       |
+|--------------------------------------|--------------------------------------------|
+| 8CA07FB7-DFFE-4440-9ED7-6498CC074F11 | Morningstar Prospects                      |
+| AE322592-5A3E-4B31-B889-16D8E76F48D3 | Sustainable Landscape U.S. Funds Q4 2021   |
+| 83D337A2-1CF2-4E66-A94D-2B8EE554AC23 | Sustainable Landscape Global Funds Q4 2021 |
+| ...                                  | ...                                        |
+
+# Specify data points by using one of Morningstar's pre-saved data sets
+morningstar_data_sets = md.direct.lookup.get_morningstar_data_sets()
+
+| datasetId | name                                          |
+|-----------|-----------------------------------------------|
+| 0218-0020 | Snapshot                                      |
+| 0218-0446 | Sustainability: ESG Risk (Company)            |
+| 0218-0481 | Sustainability: Portfolio Sustainability Risk |
+| ...       | ...                                           |
+
+
+# Retrieve data by using the investment list and data set IDs from above
+data = md.direct.get_investment_data(investments=lists["id"][0], data_points=morningstar_data_sets["datasetId"][0])
+
+| Id            | Name                                    | Base Currency | ... |
+|---------------|-----------------------------------------|---------------|-----|
+| F00001AHPT;FO | Hartford Schroders Sustainable Cr Bd I  | US Dollar     | ... |
+| F000014ZNT;FE | iShares ESG Aware Aggressive Allc ETF   | US Dollar     | ... |
+| F00000WUF1;FE | iShares MSCI Global Sust Dev Goals ETF  | US Dollar     | ... |
+| ...           | ...                                     | ...           | ... |
+
+```
+
+### Documentation
+
+Documentation is hosted at https://docs-analyticslab.morningstar.com/latest/index.html
+
+Find the version you are using with `md.__version__`
+
+### Data Retrieval
+
+The Morningstar Data Extension in [Analytics Lab](https://analyticslab.morningstar.com/) is the most convenient tool for locating data points and various saved objects to be used in morningstar_data function calls. You can browse data points, saved investment lists, search criteria, performance reports and more. Drag and drop the object you are interested in into a notebook and the corresponding Python code will be generated for you.
+
+![direct extension](https://al-morningstar-readme-images-temp.s3.amazonaws.com/morningstar_direct_extension.png)
+
+
+# Limits
+
+## Overview of Limits
+
+
+|Type of Limit| Restriction  |
+|-------------|--------------|
+|Limits | Morningstar Direct is exclusively licensed for individual usage. Users of Morningstar Direct are strictly prohibited from disclosing their login credentials, deploying instances of Morningstar Direct on a server, or utilizing, distributing, or redistributing data in a manner contradictory to their organization's agreement with Morningstar. Moreover, Morningstar Direct users are prohibited from employing information in any manner that would contravene the regulations and policies established by third-party providers.|
+|Call Limits | When utilizing the morningstar_data Python package for data extraction, it's important to be aware of the limitations imposed on the number of requests you can make or the amount of data you can receive. These limitations are in place to ensure efficient usage of the resources and maintain the overall performance of the system.|
+|Daily Limits | Limits are in place and can be reached when making requests or receiving data within a single day. These limits are determined either by the number of requests made or the quantity of data received. It is important to keep these limitations in mind while working with the data to ensure compliance and avoid any interruptions in your data processing tasks.|
+|Content Limits |Content limits are governed by entitlements, which are determined by the specific product variant and add-ons purchased. These limits are put in place to regulate the amount of content accessible within the platform. It is important to be aware of these entitlements and ensure they align with your requirements and data processing tasks.|
+
+## Detailed Limits
+
+|Type of Limit| For this Item | Has this limitation|
+|-------------|---------------|--------------------|
+|Daily Limits | Number of Cells per Day | The count of data retrieved from the morningstar_data Python package per day cannot exceed 500,000 cells per day. This count of data is summed across all client applications connected to the same Morningstar Direct instance. In the event you reach your limit, please contact your Sales Representative or Customer Success Manager at Morningstar.|
+|Daily Limits | Number Of investments in an Investment List | The size of an investment list in Morningstar Direct cannot exceed 30,000 investments in a single query.|
+|Daily Limits | Number of data points returned per request |Data point limits are uniform across the type of data being retrieved. That is, the limits apply to time series data, static data, and so on, but are not aggregated across all applications. A custom data set in Morningstar Direct is limited to 1,000 data points.|
+|Content/Entitlement Limits | Third-pary data usage|Additional morningstar_data Python package limitations may be imposed by the providers of the underlying data content. Consult with your Customer Success Manager or Sales Representative to know what third-party provider terms may apply to your use of this data.|
+
+
+## Restricted Functions
+As you refer to the morningstar_data Python package documentation, you may find some utility functions and additional data query functions that are not yet available for use. Such functions are in testing by internal teams at Morningstar, and they will be available to Morningstar Direct clients in the future.
+
+# Usage
+## Usage of Python package
+
+A Python package refers to a specialized computer program that can be imported into a development environment to facilitate easier access to specific Morningstar data and the execution of pre-built functions. It consists of a toolkit comprising a predefined collection of functions that assist users in constructing something with ease and efficiency. The utilization of the morningstar_data Python package is subject to the governance of the Apache 2.0 license. An Authorized User is explicitly prohibited from engaging in activities such as translating, disassembling, or separating components of the Python package (e.g., accessing or acquiring Product code in any manner). The sole means of granting Authorized Users permission to employ and manipulate the Python package is by referencing or providing a separate entitlement to do so. However, this permission must not override any other limitations outlined in the Click License about the utilization or distribution of the Product.
+
+## Extraction of Data using the Python package
+
+Since the functions (i.e., tools) within the morningstar_data package enable users to extract Morningstar data in various ways, it is imperative to ensure that users extract the data within the constraints specified for them and by the distribution licenses held by Morningstar with their respective firms.
+
+## Sharing of Authentication Token
+
+We authenticate a user's access to the morningstar_data package using an authentication token, which remains valid for 24 hours and can solely be obtained from Analytics Lab. Access to Analytics Lab requires possession of a Direct License. Users are strictly prohibited from sharing their authentication tokens with other individuals, as the usage of the product is tethered to the terms and agreements associated with license of Morningstar Direct.
+
+# Terms & Conditions
+The utilization of the morningstar_data Python package entails accessing certain data from Morningstar Direct. Your access and utilization of Morningstar Direct, including its morningstar_data Python package and associated data, are governed by the terms and conditions set forth in your organization’s agreement with Morningstar. Morningstar Direct is an Asset and Wealth management platform that is lawfully licensed for individual use, subject to a login session requirement. A login session is designed to control entitlements and regulate reasonable use for a singular user. To align with the workflow demands of a single user, the morningstar_data Python package imposes restrictions to safeguard the overall platform’s capacity to support the usage levels of all individual Morningstar Direct users accessing data via APIs. The document attached below provides a succinct overview of these various restrictions and elucidates the user experience when encountering them. The specific numerical values for each restriction described herein are not binding and do not create any legal obligations on the part of Morningstar. These restrictions are subject to modification at our sole discretion, without prior notice. It is your sole responsibility to furnish all necessary support pertaining to any applications developed utilizing the morningstar_data Python package. Kindly take note that if you have intentions to resell or distribute any applications or data developed using the morningstar_data Python package to third parties, it is imperative to engage in a distribution license agreement with us. Please contact your Customer Success Manager or Sales Representative at Morningstar for further information.
```

### Comparing `morningstar_data-1.2.0/PKG-INFO` & `morningstar_data-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morningstar-data
-Version: 1.2.0
+Version: 1.3.0
 Summary: Morningstar Data
 Home-page: https://www.morningstar.com/products/md-python-package
 License: Apache-2.0
 Author: Morningstar, Inc.
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

