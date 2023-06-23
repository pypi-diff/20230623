# Comparing `tmp/weni_rp_apps-2.7.0.tar.gz` & `tmp/weni_rp_apps-2.7.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weni_rp_apps-2.7.0.tar", max compression
+gzip compressed data, was "weni_rp_apps-2.7.0a1.tar", max compression
```

## Comparing `weni_rp_apps-2.7.0.tar` & `weni_rp_apps-2.7.0a1.tar`

### file list

```diff
@@ -1,173 +1,178 @@
--rw-r--r--   0        0        0      644 2023-06-22 22:02:24.841682 weni_rp_apps-2.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/activities/__init__.py
--rw-r--r--   0        0        0      245 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/activities/apps.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/activities/migrations/__init__.py
--rw-r--r--   0        0        0     2096 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/activities/signals.py
--rw-r--r--   0        0        0      366 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/activities/tasks.py
--rw-r--r--   0        0        0      325 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/analytics_api/README.md
--rw-r--r--   0        0        0       66 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/analytics_api/__init__.py
--rw-r--r--   0        0        0      264 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/analytics_api/apps.py
--rw-r--r--   0        0        0    13526 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/analytics_api/tests.py
--rw-r--r--   0        0        0      535 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/analytics_api/urls.py
--rw-r--r--   0        0        0     9016 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/analytics_api/views.py
--rw-r--r--   0        0        0       49 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/auth/__init__.py
--rw-r--r--   0        0        0      285 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/auth/apps.py
--rw-r--r--   0        0        0     1321 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/auth/backends.py
--rw-r--r--   0        0        0      430 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/auth/decorators.py
--rw-r--r--   0        0        0      810 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/auth/urls.py
--rw-r--r--   0        0        0     2645 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/auth/views.py
--rw-r--r--   0        0        0      309 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/channel_stats/README.md
--rw-r--r--   0        0        0       66 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/channel_stats/__init__.py
--rw-r--r--   0        0        0      264 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/channel_stats/apps.py
--rw-r--r--   0        0        0     6157 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/channel_stats/serializers.py
--rw-r--r--   0        0        0      347 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/channel_stats/urls.py
--rw-r--r--   0        0        0     3575 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/channel_stats/views.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/grpc/billing/__init__.py
--rw-r--r--   0        0        0      102 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/grpc/billing/apps.py
--rw-r--r--   0        0        0     3508 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/grpc/billing/queries.py
--rw-r--r--   0        0        0     3194 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/grpc/billing/serializers.py
--rw-r--r--   0        0        0     2063 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/grpc/billing/services.py
--rw-r--r--   0        0        0    11364 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/grpc/billing/tests.py
--rw-r--r--   0        0        0      231 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/grpc/billing/urls.py
--rw-r--r--   0        0        0       64 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/grpc/channel/__init__.py
--rw-r--r--   0        0        0      103 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/grpc/channel/apps.py
--rw-r--r--   0        0        0      352 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/grpc/channel/fields.py
--rw-r--r--   0        0        0     4070 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/grpc/channel/serializers.py
--rw-r--r--   0        0        0     4081 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/grpc/channel/services.py
--rw-r--r--   0        0        0     7987 2023-06-22 22:01:58.809388 weni_rp_apps-2.7.0/weni/grpc/channel/tests.py
--rw-r--r--   0        0        0      341 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/channel/urls.py
--rw-r--r--   0        0        0       70 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/classifier/__init__.py
--rw-r--r--   0        0        0      109 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/classifier/apps.py
--rw-r--r--   0        0        0     1356 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/classifier/serializers.py
--rw-r--r--   0        0        0     1174 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/classifier/services.py
--rw-r--r--   0        0        0     6493 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/classifier/tests.py
--rw-r--r--   0        0        0      249 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/classifier/urls.py
--rw-r--r--   0        0        0       61 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/core/__init__.py
--rw-r--r--   0        0        0      100 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/core/apps.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/core/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/core/management/commands/__init__.py
--rw-r--r--   0        0        0     1588 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/core/management/commands/grpc.py
--rw-r--r--   0        0        0     1213 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/core/serializers.py
--rw-r--r--   0        0        0      965 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/core/services.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/core/tests.py
--rw-r--r--   0        0        0      700 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/core/urls.py
--rw-r--r--   0        0        0       58 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/flow/__init__.py
--rw-r--r--   0        0        0       97 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/flow/apps.py
--rw-r--r--   0        0        0      307 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/flow/serializers.py
--rw-r--r--   0        0        0      680 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/flow/services.py
--rw-r--r--   0        0        0     2764 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/flow/tests.py
--rw-r--r--   0        0        0      213 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/flow/urls.py
--rw-r--r--   0        0        0       56 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/org/__init__.py
--rw-r--r--   0        0        0       95 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/org/apps.py
--rw-r--r--   0        0        0     2836 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/org/serializers.py
--rw-r--r--   0        0        0     4020 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/org/services.py
--rw-r--r--   0        0        0     9821 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/org/tests.py
--rw-r--r--   0        0        0      207 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/org/urls.py
--rw-r--r--   0        0        0       68 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/statistic/__init__.py
--rw-r--r--   0        0        0      107 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/statistic/apps.py
--rw-r--r--   0        0        0      672 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/statistic/services.py
--rw-r--r--   0        0        0     3132 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/statistic/tests.py
--rw-r--r--   0        0        0      252 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/statistic/urls.py
--rw-r--r--   0        0        0       58 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/user/__init__.py
--rw-r--r--   0        0        0       97 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/user/apps.py
--rw-r--r--   0        0        0      843 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/user/serializers.py
--rw-r--r--   0        0        0     3916 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/user/services.py
--rw-r--r--   0        0        0    10076 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/user/tests.py
--rw-r--r--   0        0        0      347 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/grpc/user/urls.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/__init__.py
--rw-r--r--   0        0        0      328 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/apps.py
--rw-r--r--   0        0        0      300 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/authenticators.py
--rw-r--r--   0        0        0     1374 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/backends.py
--rw-r--r--   0        0        0     5484 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/channel/serializers.py
--rw-r--r--   0        0        0    16305 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/channel/tests.py
--rw-r--r--   0        0        0      394 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/channel/urls.py
--rw-r--r--   0        0        0     7611 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/channel/views.py
--rw-r--r--   0        0        0     1527 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/classifier/serializers.py
--rw-r--r--   0        0        0     8626 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/classifier/tests.py
--rw-r--r--   0        0        0      318 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/classifier/urls.py
--rw-r--r--   0        0        0     2803 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/classifier/views.py
--rw-r--r--   0        0        0      113 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/clients/__init__.py
--rw-r--r--   0        0        0      692 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/clients/authenticators.py
--rw-r--r--   0        0        0      486 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/clients/base.py
--rw-r--r--   0        0        0      681 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/clients/connect.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/externals/__init__.py
--rw-r--r--   0        0        0     2476 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/externals/serializers.py
--rw-r--r--   0        0        0      546 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/externals/urls.py
--rw-r--r--   0        0        0     4243 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/externals/views.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/flows/__init__.py
--rw-r--r--   0        0        0     1323 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/flows/serializers.py
--rw-r--r--   0        0        0     4436 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/flows/tests.py
--rw-r--r--   0        0        0      308 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/flows/urls.py
--rw-r--r--   0        0        0      977 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/flows/views.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/globals/__init__.py
--rw-r--r--   0        0        0     2286 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/globals/serializers.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/globals/tests/__init__.py
--rw-r--r--   0        0        0     2183 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/globals/tests/test_serializers.py
--rw-r--r--   0        0        0      220 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/globals/urls.py
--rw-r--r--   0        0        0     1484 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/globals/views.py
--rw-r--r--   0        0        0     1247 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/migrations/0001_initial.py
--rw-r--r--   0        0        0     1032 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/migrations/0002_project.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/migrations/__init__.py
--rw-r--r--   0        0        0      916 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/models.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/orgs/__init__.py
--rw-r--r--   0        0        0     3976 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/orgs/serializers.py
--rw-r--r--   0        0        0    14533 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/orgs/tests.py
--rw-r--r--   0        0        0      300 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/orgs/urls.py
--rw-r--r--   0        0        0     4592 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/orgs/views.py
--rw-r--r--   0        0        0      246 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/permissions.py
--rw-r--r--   0        0        0     2164 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/statistic/tests.py
--rw-r--r--   0        0        0      205 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/statistic/urls.py
--rw-r--r--   0        0        0     1007 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/statistic/views.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.813388 weni_rp_apps-2.7.0/weni/internal/tests/__init__.py
--rw-r--r--   0        0        0     1249 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/internal/tests/test_models.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/internal/tickets/__init__.py
--rw-r--r--   0        0        0     1150 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/internal/tickets/serializers.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/internal/tickets/tests/__init__.py
--rw-r--r--   0        0        0     3360 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/internal/tickets/tests/test_views.py
--rw-r--r--   0        0        0      443 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/internal/tickets/urls.py
--rw-r--r--   0        0        0     1844 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/internal/tickets/views.py
--rw-r--r--   0        0        0     1315 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/internal/urls.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/internal/users/__init__.py
--rw-r--r--   0        0        0      845 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/internal/users/serializers.py
--rw-r--r--   0        0        0    12563 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/internal/users/tests.py
--rw-r--r--   0        0        0      711 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/internal/users/urls.py
--rw-r--r--   0        0        0     5849 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/internal/users/views.py
--rw-r--r--   0        0        0      555 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/internal/views.py
--rw-r--r--   0        0        0       55 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/orgs_api/__init__.py
--rw-r--r--   0        0        0      253 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/orgs_api/apps.py
--rw-r--r--   0        0        0      906 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/orgs_api/serializers.py
--rw-r--r--   0        0        0     4030 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/orgs_api/tests.py
--rw-r--r--   0        0        0      178 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/orgs_api/urls.py
--rw-r--r--   0        0        0     1444 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/orgs_api/views.py
--rw-r--r--   0        0        0       45 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/s3/__init__.py
--rw-r--r--   0        0        0      243 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/s3/apps.py
--rw-r--r--   0        0        0      219 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/s3/urls.py
--rw-r--r--   0        0        0      550 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/s3/views.py
--rw-r--r--   0        0        0       93 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/serializers/__init__.py
--rw-r--r--   0        0        0      725 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/serializers/fields.py
--rw-r--r--   0        0        0      281 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/success_orgs/apps.py
--rw-r--r--   0        0        0     2791 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/success_orgs/business.py
--rw-r--r--   0        0        0      619 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/success_orgs/serializers.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/success_orgs/tests/__init__.py
--rw-r--r--   0        0        0     3354 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/success_orgs/tests/test_business.py
--rw-r--r--   0        0        0      494 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/success_orgs/urls.py
--rw-r--r--   0        0        0     2770 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/success_orgs/views.py
--rw-r--r--   0        0        0      318 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/template_message/README.md
--rw-r--r--   0        0        0       72 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/template_message/__init__.py
--rw-r--r--   0        0        0      294 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/template_message/apps.py
--rw-r--r--   0        0        0     2040 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/template_message/serializers.py
--rw-r--r--   0        0        0     5292 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/template_message/tests.py
--rw-r--r--   0        0        0      344 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/template_message/urls.py
--rw-r--r--   0        0        0     1651 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/template_message/views.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/templates/__init__.py
--rw-r--r--   0        0        0      545 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/templates/context_processors.py
--rw-r--r--   0        0        0      315 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/ticketer_queues/README.md
--rw-r--r--   0        0        0       70 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/ticketer_queues/__init__.py
--rw-r--r--   0        0        0      291 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/ticketer_queues/apps.py
--rw-r--r--   0        0        0      242 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/ticketer_queues/serializers.py
--rw-r--r--   0        0        0     1584 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/ticketer_queues/tests.py
--rw-r--r--   0        0        0      378 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/ticketer_queues/urls.py
--rw-r--r--   0        0        0      849 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/ticketer_queues/views.py
--rw-r--r--   0        0        0        0 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/utils/__init__.py
--rw-r--r--   0        0        0     1091 2023-06-22 22:01:58.817388 weni_rp_apps-2.7.0/weni/utils/app_config.py
--rw-r--r--   0        0        0     1001 1970-01-01 00:00:00.000000 weni_rp_apps-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0      646 2023-06-23 16:28:51.933008 weni_rp_apps-2.7.0a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/activities/__init__.py
+-rw-r--r--   0        0        0      245 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/activities/apps.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/activities/migrations/__init__.py
+-rw-r--r--   0        0        0     2096 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/activities/signals.py
+-rw-r--r--   0        0        0      366 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/activities/tasks.py
+-rw-r--r--   0        0        0      325 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/analytics_api/README.md
+-rw-r--r--   0        0        0       66 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/analytics_api/__init__.py
+-rw-r--r--   0        0        0      264 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/analytics_api/apps.py
+-rw-r--r--   0        0        0    13526 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/analytics_api/tests.py
+-rw-r--r--   0        0        0      535 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/analytics_api/urls.py
+-rw-r--r--   0        0        0     9016 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/analytics_api/views.py
+-rw-r--r--   0        0        0       49 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/auth/__init__.py
+-rw-r--r--   0        0        0      285 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/auth/apps.py
+-rw-r--r--   0        0        0     1321 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/auth/backends.py
+-rw-r--r--   0        0        0      430 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/auth/decorators.py
+-rw-r--r--   0        0        0      810 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/auth/urls.py
+-rw-r--r--   0        0        0     2645 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/auth/views.py
+-rw-r--r--   0        0        0      309 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/channel_stats/README.md
+-rw-r--r--   0        0        0       66 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/channel_stats/__init__.py
+-rw-r--r--   0        0        0      264 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/channel_stats/apps.py
+-rw-r--r--   0        0        0     6157 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/channel_stats/serializers.py
+-rw-r--r--   0        0        0      347 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/channel_stats/urls.py
+-rw-r--r--   0        0        0     3575 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/channel_stats/views.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/billing/__init__.py
+-rw-r--r--   0        0        0      102 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/billing/apps.py
+-rw-r--r--   0        0        0     3508 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/billing/queries.py
+-rw-r--r--   0        0        0     3194 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/billing/serializers.py
+-rw-r--r--   0        0        0     2063 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/billing/services.py
+-rw-r--r--   0        0        0    11364 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/billing/tests.py
+-rw-r--r--   0        0        0      231 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/billing/urls.py
+-rw-r--r--   0        0        0       64 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/channel/__init__.py
+-rw-r--r--   0        0        0      103 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/channel/apps.py
+-rw-r--r--   0        0        0      352 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/channel/fields.py
+-rw-r--r--   0        0        0     4070 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/channel/serializers.py
+-rw-r--r--   0        0        0     4081 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/channel/services.py
+-rw-r--r--   0        0        0     7987 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/channel/tests.py
+-rw-r--r--   0        0        0      341 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/channel/urls.py
+-rw-r--r--   0        0        0       70 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/classifier/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/classifier/apps.py
+-rw-r--r--   0        0        0     1356 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/classifier/serializers.py
+-rw-r--r--   0        0        0     1174 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/classifier/services.py
+-rw-r--r--   0        0        0     6493 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/classifier/tests.py
+-rw-r--r--   0        0        0      249 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/classifier/urls.py
+-rw-r--r--   0        0        0       61 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/core/__init__.py
+-rw-r--r--   0        0        0      100 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/core/apps.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     1588 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/core/management/commands/grpc.py
+-rw-r--r--   0        0        0     1213 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/core/serializers.py
+-rw-r--r--   0        0        0      965 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/core/services.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/core/tests.py
+-rw-r--r--   0        0        0      700 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/core/urls.py
+-rw-r--r--   0        0        0       58 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/flow/__init__.py
+-rw-r--r--   0        0        0       97 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/flow/apps.py
+-rw-r--r--   0        0        0      307 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/flow/serializers.py
+-rw-r--r--   0        0        0      680 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/flow/services.py
+-rw-r--r--   0        0        0     2764 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/flow/tests.py
+-rw-r--r--   0        0        0      213 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/flow/urls.py
+-rw-r--r--   0        0        0       56 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/org/__init__.py
+-rw-r--r--   0        0        0       95 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/org/apps.py
+-rw-r--r--   0        0        0     2836 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/org/serializers.py
+-rw-r--r--   0        0        0     4020 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/org/services.py
+-rw-r--r--   0        0        0     9821 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/org/tests.py
+-rw-r--r--   0        0        0      207 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/org/urls.py
+-rw-r--r--   0        0        0       68 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/statistic/__init__.py
+-rw-r--r--   0        0        0      107 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/statistic/apps.py
+-rw-r--r--   0        0        0      672 2023-06-23 16:28:29.008646 weni_rp_apps-2.7.0a1/weni/grpc/statistic/services.py
+-rw-r--r--   0        0        0     3132 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/grpc/statistic/tests.py
+-rw-r--r--   0        0        0      252 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/grpc/statistic/urls.py
+-rw-r--r--   0        0        0       58 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/grpc/user/__init__.py
+-rw-r--r--   0        0        0       97 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/grpc/user/apps.py
+-rw-r--r--   0        0        0      843 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/grpc/user/serializers.py
+-rw-r--r--   0        0        0     3916 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/grpc/user/services.py
+-rw-r--r--   0        0        0    10076 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/grpc/user/tests.py
+-rw-r--r--   0        0        0      347 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/grpc/user/urls.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/__init__.py
+-rw-r--r--   0        0        0      328 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/apps.py
+-rw-r--r--   0        0        0      300 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/authenticators.py
+-rw-r--r--   0        0        0     1374 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/backends.py
+-rw-r--r--   0        0        0     5484 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/channel/serializers.py
+-rw-r--r--   0        0        0    16305 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/channel/tests.py
+-rw-r--r--   0        0        0      394 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/channel/urls.py
+-rw-r--r--   0        0        0     7611 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/channel/views.py
+-rw-r--r--   0        0        0     1527 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/classifier/serializers.py
+-rw-r--r--   0        0        0     8626 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/classifier/tests.py
+-rw-r--r--   0        0        0      318 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/classifier/urls.py
+-rw-r--r--   0        0        0     2803 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/classifier/views.py
+-rw-r--r--   0        0        0      113 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/clients/__init__.py
+-rw-r--r--   0        0        0      692 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/clients/authenticators.py
+-rw-r--r--   0        0        0      486 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/clients/base.py
+-rw-r--r--   0        0        0      681 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/clients/connect.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/externals/__init__.py
+-rw-r--r--   0        0        0     2476 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/externals/serializers.py
+-rw-r--r--   0        0        0      546 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/externals/urls.py
+-rw-r--r--   0        0        0     4243 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/externals/views.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/flows/__init__.py
+-rw-r--r--   0        0        0     1278 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/flows/serializers.py
+-rw-r--r--   0        0        0     4318 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/flows/tests.py
+-rw-r--r--   0        0        0      308 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/flows/urls.py
+-rw-r--r--   0        0        0      974 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/flows/views.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/globals/__init__.py
+-rw-r--r--   0        0        0     2286 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/globals/serializers.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/globals/tests/__init__.py
+-rw-r--r--   0        0        0     2183 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/globals/tests/test_serializers.py
+-rw-r--r--   0        0        0      220 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/globals/urls.py
+-rw-r--r--   0        0        0     1484 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/globals/views.py
+-rw-r--r--   0        0        0     1247 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1032 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/migrations/0002_project.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/migrations/__init__.py
+-rw-r--r--   0        0        0      916 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/models.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/msgs/__init__.py
+-rw-r--r--   0        0        0     5319 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/msgs/tasks.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/msgs/tests/tests.py
+-rw-r--r--   0        0        0      259 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/msgs/urls.py
+-rw-r--r--   0        0        0     2635 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/msgs/views.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/orgs/__init__.py
+-rw-r--r--   0        0        0     3976 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/orgs/serializers.py
+-rw-r--r--   0        0        0    14533 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/orgs/tests.py
+-rw-r--r--   0        0        0      300 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/orgs/urls.py
+-rw-r--r--   0        0        0     4592 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/orgs/views.py
+-rw-r--r--   0        0        0      246 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/permissions.py
+-rw-r--r--   0        0        0     2164 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/statistic/tests.py
+-rw-r--r--   0        0        0      205 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/statistic/urls.py
+-rw-r--r--   0        0        0     1007 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/statistic/views.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/tests/__init__.py
+-rw-r--r--   0        0        0     1249 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/tests/test_models.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/tickets/__init__.py
+-rw-r--r--   0        0        0     1150 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/tickets/serializers.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/tickets/tests/__init__.py
+-rw-r--r--   0        0        0     3360 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/tickets/tests/test_views.py
+-rw-r--r--   0        0        0      443 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/tickets/urls.py
+-rw-r--r--   0        0        0     1844 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/tickets/views.py
+-rw-r--r--   0        0        0     1417 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/urls.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/users/__init__.py
+-rw-r--r--   0        0        0      845 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/users/serializers.py
+-rw-r--r--   0        0        0    12563 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/users/tests.py
+-rw-r--r--   0        0        0      711 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/users/urls.py
+-rw-r--r--   0        0        0     5849 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/users/views.py
+-rw-r--r--   0        0        0      555 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/internal/views.py
+-rw-r--r--   0        0        0       55 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/orgs_api/__init__.py
+-rw-r--r--   0        0        0      253 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/orgs_api/apps.py
+-rw-r--r--   0        0        0      906 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/orgs_api/serializers.py
+-rw-r--r--   0        0        0     4030 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/orgs_api/tests.py
+-rw-r--r--   0        0        0      178 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/orgs_api/urls.py
+-rw-r--r--   0        0        0     1444 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/orgs_api/views.py
+-rw-r--r--   0        0        0       45 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/s3/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/s3/apps.py
+-rw-r--r--   0        0        0      219 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/s3/urls.py
+-rw-r--r--   0        0        0      550 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/s3/views.py
+-rw-r--r--   0        0        0       93 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/serializers/__init__.py
+-rw-r--r--   0        0        0      725 2023-06-23 16:28:29.012646 weni_rp_apps-2.7.0a1/weni/serializers/fields.py
+-rw-r--r--   0        0        0      281 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/success_orgs/apps.py
+-rw-r--r--   0        0        0     2791 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/success_orgs/business.py
+-rw-r--r--   0        0        0      619 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/success_orgs/serializers.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/success_orgs/tests/__init__.py
+-rw-r--r--   0        0        0     3354 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/success_orgs/tests/test_business.py
+-rw-r--r--   0        0        0      494 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/success_orgs/urls.py
+-rw-r--r--   0        0        0     2770 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/success_orgs/views.py
+-rw-r--r--   0        0        0      318 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/template_message/README.md
+-rw-r--r--   0        0        0       72 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/template_message/__init__.py
+-rw-r--r--   0        0        0      294 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/template_message/apps.py
+-rw-r--r--   0        0        0     2040 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/template_message/serializers.py
+-rw-r--r--   0        0        0     5292 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/template_message/tests.py
+-rw-r--r--   0        0        0      344 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/template_message/urls.py
+-rw-r--r--   0        0        0     1651 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/template_message/views.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/templates/__init__.py
+-rw-r--r--   0        0        0      545 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/templates/context_processors.py
+-rw-r--r--   0        0        0      315 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/ticketer_queues/README.md
+-rw-r--r--   0        0        0       70 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/ticketer_queues/__init__.py
+-rw-r--r--   0        0        0      291 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/ticketer_queues/apps.py
+-rw-r--r--   0        0        0      242 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/ticketer_queues/serializers.py
+-rw-r--r--   0        0        0     1584 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/ticketer_queues/tests.py
+-rw-r--r--   0        0        0      378 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/ticketer_queues/urls.py
+-rw-r--r--   0        0        0      849 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/ticketer_queues/views.py
+-rw-r--r--   0        0        0        0 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/utils/__init__.py
+-rw-r--r--   0        0        0     1091 2023-06-23 16:28:29.016646 weni_rp_apps-2.7.0a1/weni/utils/app_config.py
+-rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 weni_rp_apps-2.7.0a1/PKG-INFO
```

### Comparing `weni_rp_apps-2.7.0/pyproject.toml` & `weni_rp_apps-2.7.0a1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weni-rp-apps"
-version = "2.7.0"
+version = "2.7.0a1"
 description = "Weni apps for Rapidpro Platform"
 authors = ["jcbalmeida"]
 license = "AGPL-3.0"
 packages = [
     { include = "weni" }
 ]
```

### Comparing `weni_rp_apps-2.7.0/weni/activities/signals.py` & `weni_rp_apps-2.7.0a1/weni/activities/signals.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/analytics_api/tests.py` & `weni_rp_apps-2.7.0a1/weni/analytics_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/analytics_api/urls.py` & `weni_rp_apps-2.7.0a1/weni/analytics_api/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/analytics_api/views.py` & `weni_rp_apps-2.7.0a1/weni/analytics_api/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/auth/backends.py` & `weni_rp_apps-2.7.0a1/weni/auth/backends.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/auth/urls.py` & `weni_rp_apps-2.7.0a1/weni/auth/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/auth/views.py` & `weni_rp_apps-2.7.0a1/weni/auth/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/channel_stats/serializers.py` & `weni_rp_apps-2.7.0a1/weni/channel_stats/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/channel_stats/views.py` & `weni_rp_apps-2.7.0a1/weni/channel_stats/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/billing/queries.py` & `weni_rp_apps-2.7.0a1/weni/grpc/billing/queries.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/billing/serializers.py` & `weni_rp_apps-2.7.0a1/weni/grpc/billing/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/billing/services.py` & `weni_rp_apps-2.7.0a1/weni/grpc/billing/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/billing/tests.py` & `weni_rp_apps-2.7.0a1/weni/grpc/billing/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/channel/serializers.py` & `weni_rp_apps-2.7.0a1/weni/grpc/channel/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/channel/services.py` & `weni_rp_apps-2.7.0a1/weni/grpc/channel/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/channel/tests.py` & `weni_rp_apps-2.7.0a1/weni/grpc/channel/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/classifier/serializers.py` & `weni_rp_apps-2.7.0a1/weni/grpc/classifier/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/classifier/services.py` & `weni_rp_apps-2.7.0a1/weni/grpc/classifier/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/classifier/tests.py` & `weni_rp_apps-2.7.0a1/weni/grpc/classifier/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/core/management/commands/grpc.py` & `weni_rp_apps-2.7.0a1/weni/grpc/core/management/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/core/serializers.py` & `weni_rp_apps-2.7.0a1/weni/grpc/core/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/core/services.py` & `weni_rp_apps-2.7.0a1/weni/grpc/core/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/core/urls.py` & `weni_rp_apps-2.7.0a1/weni/grpc/core/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/flow/services.py` & `weni_rp_apps-2.7.0a1/weni/grpc/flow/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/flow/tests.py` & `weni_rp_apps-2.7.0a1/weni/grpc/flow/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/org/serializers.py` & `weni_rp_apps-2.7.0a1/weni/grpc/org/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/org/services.py` & `weni_rp_apps-2.7.0a1/weni/grpc/org/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/org/tests.py` & `weni_rp_apps-2.7.0a1/weni/grpc/org/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/statistic/services.py` & `weni_rp_apps-2.7.0a1/weni/grpc/statistic/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/statistic/tests.py` & `weni_rp_apps-2.7.0a1/weni/grpc/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/user/serializers.py` & `weni_rp_apps-2.7.0a1/weni/grpc/user/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/user/services.py` & `weni_rp_apps-2.7.0a1/weni/grpc/user/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/grpc/user/tests.py` & `weni_rp_apps-2.7.0a1/weni/grpc/user/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/backends.py` & `weni_rp_apps-2.7.0a1/weni/internal/backends.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/channel/serializers.py` & `weni_rp_apps-2.7.0a1/weni/internal/channel/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/channel/tests.py` & `weni_rp_apps-2.7.0a1/weni/internal/channel/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/channel/views.py` & `weni_rp_apps-2.7.0a1/weni/internal/channel/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/classifier/serializers.py` & `weni_rp_apps-2.7.0a1/weni/internal/classifier/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/classifier/tests.py` & `weni_rp_apps-2.7.0a1/weni/internal/classifier/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/classifier/views.py` & `weni_rp_apps-2.7.0a1/weni/internal/classifier/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/clients/authenticators.py` & `weni_rp_apps-2.7.0a1/weni/internal/clients/authenticators.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/clients/connect.py` & `weni_rp_apps-2.7.0a1/weni/internal/clients/connect.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/externals/serializers.py` & `weni_rp_apps-2.7.0a1/weni/internal/externals/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/externals/urls.py` & `weni_rp_apps-2.7.0a1/weni/internal/externals/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/externals/views.py` & `weni_rp_apps-2.7.0a1/weni/internal/externals/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/flows/serializers.py` & `weni_rp_apps-2.7.0a1/weni/internal/flows/serializers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from rest_framework import serializers
 from django.contrib.auth import get_user_model
 
-from weni.serializers import fields as weni_fields
+from weni.grpc.core import serializers as weni_serializers
+from temba.flows.models import Flow
+
 
 User = get_user_model()
 
 
-class FlowSerializer(serializers.Serializer):
-    project = weni_fields.ProjectUUIDRelatedField(required=True, write_only=True)
+class FlowSerializer(serializers.ModelSerializer):
+    org = weni_serializers.OrgUUIDRelatedField()
     sample_flow = serializers.JSONField(write_only=True)
-    uuid = serializers.UUIDField(read_only=True)
 
     class Meta:
-        fields = ("project", "uuid", "sample_flow")
+        model = Flow
+        fields = ("org", "uuid", "sample_flow")
 
     def create(self, validated_data):
-        project = validated_data.get("project")
+        org = validated_data.get("org")
         sample_flows = validated_data.get("sample_flow")
-        project.import_app(sample_flows, project.created_by)
-        self.disable_flows_has_issues(project, sample_flows)
-        return project.flows.order_by("created_on").last()
+        org.import_app(sample_flows, org.created_by)
+        self.disable_flows_has_issues(org, sample_flows)
+        return org.flows.order_by("created_on").last()
 
-    def disable_flows_has_issues(self, project, sample_flows):
+    def disable_flows_has_issues(self, org, sample_flows):
         flows_name = list(map(lambda flow: flow.get("name"), sample_flows.get("flows")))
-        project.flows.filter(name__in=flows_name).update(has_issues=False)
+        org.flows.filter(name__in=flows_name).update(has_issues=False)
 
 
 class FlowListSerializer(serializers.Serializer):
     flow_name = serializers.CharField(required=True, write_only=True)
-    project = weni_fields.ProjectUUIDRelatedField(required=True, write_only=True)
+    org_uuid = weni_serializers.OrgUUIDRelatedField(required=True, write_only=True)
     uuid = serializers.CharField(read_only=True)
     name = serializers.CharField(read_only=True)
```

### Comparing `weni_rp_apps-2.7.0/weni/internal/flows/tests.py` & `weni_rp_apps-2.7.0a1/weni/internal/flows/tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,37 +5,32 @@
 from django.urls import reverse
 from django.utils.http import urlencode
 from django.contrib.auth.models import User
 
 from temba.tests import TembaTest
 from temba.api.models import APIToken
 
+from temba.orgs.models import Org
 from temba.flows.models import Flow
-from weni.internal.models import Project
-from weni.internal.flows.views import ProjectFlowsViewSet
-
-
-view = ProjectFlowsViewSet
-view.permission_classes = []
 
 
 class TembaRequestMixin(ABC):
     def reverse(self, viewname, kwargs=None, query_params=None):
         url = reverse(viewname, kwargs=kwargs)
 
         if query_params:
             return "%s?%s" % (url, urlencode(query_params))
         else:
             return url
 
     def request_get(self, **query_params):
         url = self.reverse(self.get_url_namespace(), query_params=query_params)
         url = url.replace("channel", "channel.json")
-
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
+
         return self.client.get(f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}")
 
     def request_detail(self, uuid):
         url = self.reverse(self.get_url_namespace(), kwargs={"uuid": uuid})
         token = APIToken.get_or_create(self.org, self.admin, Group.objects.get(name="Administrators"))
 
         return self.client.get(f"{url}", HTTP_AUTHORIZATION=f"Token {token.key}")
@@ -64,57 +59,61 @@
 
 class ListFlowTestCase(TembaTest, TembaRequestMixin):
     def setUp(self):
         User.objects.create_user(username="testuser", password="123", email="test@weni.ai")
 
         user = User.objects.first()
 
-        temba = Project.objects.create(name="Temba", timezone="America/Maceio", created_by=user, modified_by=user)
-        weni = Project.objects.create(name="Weni", timezone="America/Maceio", created_by=user, modified_by=user)
+        # print(Org.objects.all())
+
+        temba = Org.objects.create(name="Temba", timezone="America/Maceio", created_by=user, modified_by=user)
+        weni = Org.objects.create(name="Weni", timezone="America/Maceio", created_by=user, modified_by=user)
 
         Flow.create(name="Test Temba", user=user, org=temba)
         Flow.create(name="Test flow name", user=user, org=weni)
         Flow.create(name="Test Weni flow name", user=user, org=weni)
 
         super().setUp()
 
     def test_list_flow(self):
-        temba = Project.objects.filter(name="Temba").first()
-        weni = Project.objects.get(name="Weni")
+        temba = Org.objects.filter(name="Temba").first()
+        weni = Org.objects.get(name="Weni")
 
         response = self.request_get(flow_name="test", org_uuid="123")  # {'org_uuid': ['“123” is not a valid UUID.']}
         self.assertEquals(response.status_code, 400)
 
         response = self.request_get(flow_name="test", org_uuid="")  # {'org_id': ['This field may not be blank.']}
         self.assertEquals(response.status_code, 400)
 
-        response = self.request_get(flow_name="test", org_uuid=str(temba.project_uuid)).json()
+        response = self.request_get(flow_name="test", org_uuid=str(temba.uuid)).json()
+
         flows, flows_count = self.get_flows_and_count(response)
 
         self.assertEquals(flows_count, 1)
         self.assertEquals(flows[0].get("name"), "Test Temba")
 
-        response = self.request_get(flow_name="test", org_uuid=str(weni.project_uuid)).json()
+        response = self.request_get(flow_name="test", org_uuid=str(weni.uuid)).json()
 
         flows, flows_count = self.get_flows_and_count(response)
+
         weni_flow_names = [flow.name for flow in Flow.objects.filter(org=weni.id)]
 
         self.assertEquals(flows_count, 2)
 
         for flow in flows:
             self.assertIn(flow.get("name"), weni_flow_names)
 
-        response = self.request_get(flow_name="weni", org_uuid=str(weni.project_uuid)).json()
+        response = self.request_get(flow_name="weni", org_uuid=str(weni.uuid)).json()
 
         flows, flows_count = self.get_flows_and_count(response)
 
         self.assertEquals(flows[0].get("name"), "Test Weni flow name")
         self.assertEquals(flows_count, 1)
 
-    def get_flows_and_count(self, response):
+    def get_flows_and_count(self, response) -> (list, int):
         flows = [flow for flow in response]
         flows_count = len(flows)
 
         return flows, flows_count
 
     def get_url_namespace(self):
-        return "project-flows-list"
+        return "flows-list"
```

### Comparing `weni_rp_apps-2.7.0/weni/internal/flows/views.py` & `weni_rp_apps-2.7.0a1/weni/internal/flows/views.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     def get_queryset(self):
         serializer = self.get_serializer(data=self.request.query_params.dict())
         serializer.is_valid(raise_exception=True)
 
         queryset = Flow.objects.filter(
             name__icontains=serializer.validated_data.get("flow_name"),
-            org=serializer.validated_data.get("project").org,
+            org=serializer.validated_data.get("org_uuid"),
             is_active=True,
         ).exclude(is_archived=True)[:20]
 
         if queryset:
             return queryset
 
         raise NotFound()
```

### Comparing `weni_rp_apps-2.7.0/weni/internal/globals/serializers.py` & `weni_rp_apps-2.7.0a1/weni/internal/globals/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/globals/tests/test_serializers.py` & `weni_rp_apps-2.7.0a1/weni/internal/globals/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/globals/views.py` & `weni_rp_apps-2.7.0a1/weni/internal/globals/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/migrations/0001_initial.py` & `weni_rp_apps-2.7.0a1/weni/internal/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/migrations/0002_project.py` & `weni_rp_apps-2.7.0a1/weni/internal/migrations/0002_project.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/models.py` & `weni_rp_apps-2.7.0a1/weni/internal/models.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/orgs/serializers.py` & `weni_rp_apps-2.7.0a1/weni/internal/orgs/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/orgs/tests.py` & `weni_rp_apps-2.7.0a1/weni/internal/orgs/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/orgs/views.py` & `weni_rp_apps-2.7.0a1/weni/internal/orgs/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/statistic/tests.py` & `weni_rp_apps-2.7.0a1/weni/internal/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/statistic/views.py` & `weni_rp_apps-2.7.0a1/weni/internal/statistic/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/tests/test_models.py` & `weni_rp_apps-2.7.0a1/weni/internal/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/tickets/serializers.py` & `weni_rp_apps-2.7.0a1/weni/internal/tickets/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/tickets/tests/test_views.py` & `weni_rp_apps-2.7.0a1/weni/internal/tickets/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/tickets/views.py` & `weni_rp_apps-2.7.0a1/weni/internal/tickets/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/urls.py` & `weni_rp_apps-2.7.0a1/weni/internal/urls.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,22 +15,23 @@
 from weni.internal.users.urls import urlpatterns as users_urls
 from weni.internal.tickets.urls import urlpatterns as tickets_urls
 from weni.internal.classifier.urls import urlpatterns as classifier_urls
 from weni.internal.channel.urls import urlpatterns as channel_urls
 from weni.internal.statistic.urls import urlpatterns as statistics_urls
 from weni.internal.globals.urls import urlpatterns as globals_urls
 from weni.internal.externals.urls import urlpatterns as externals_urls
+from weni.internal.msgs.urls import urlpatterns as messages_urls
 
 
 internal_urlpatterns = []
 internal_urlpatterns += orgs_urls
 internal_urlpatterns += flows_urls
 internal_urlpatterns += users_urls
 internal_urlpatterns += tickets_urls
 internal_urlpatterns += classifier_urls
 internal_urlpatterns += channel_urls
 internal_urlpatterns += statistics_urls
 internal_urlpatterns += globals_urls
 internal_urlpatterns += externals_urls
-
+internal_urlpatterns += messages_urls
 
 urlpatterns = [path("internals/", include(internal_urlpatterns))]
```

### Comparing `weni_rp_apps-2.7.0/weni/internal/users/serializers.py` & `weni_rp_apps-2.7.0a1/weni/internal/users/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/users/tests.py` & `weni_rp_apps-2.7.0a1/weni/internal/users/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/users/urls.py` & `weni_rp_apps-2.7.0a1/weni/internal/users/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/users/views.py` & `weni_rp_apps-2.7.0a1/weni/internal/users/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/internal/views.py` & `weni_rp_apps-2.7.0a1/weni/internal/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/orgs_api/serializers.py` & `weni_rp_apps-2.7.0a1/weni/orgs_api/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/orgs_api/tests.py` & `weni_rp_apps-2.7.0a1/weni/orgs_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/orgs_api/views.py` & `weni_rp_apps-2.7.0a1/weni/orgs_api/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/s3/views.py` & `weni_rp_apps-2.7.0a1/weni/s3/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/serializers/fields.py` & `weni_rp_apps-2.7.0a1/weni/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/success_orgs/business.py` & `weni_rp_apps-2.7.0a1/weni/success_orgs/business.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/success_orgs/serializers.py` & `weni_rp_apps-2.7.0a1/weni/success_orgs/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/success_orgs/tests/test_business.py` & `weni_rp_apps-2.7.0a1/weni/success_orgs/tests/test_business.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/success_orgs/views.py` & `weni_rp_apps-2.7.0a1/weni/success_orgs/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/template_message/serializers.py` & `weni_rp_apps-2.7.0a1/weni/template_message/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/template_message/tests.py` & `weni_rp_apps-2.7.0a1/weni/template_message/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/template_message/views.py` & `weni_rp_apps-2.7.0a1/weni/template_message/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/templates/context_processors.py` & `weni_rp_apps-2.7.0a1/weni/templates/context_processors.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/ticketer_queues/tests.py` & `weni_rp_apps-2.7.0a1/weni/ticketer_queues/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/ticketer_queues/views.py` & `weni_rp_apps-2.7.0a1/weni/ticketer_queues/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/weni/utils/app_config.py` & `weni_rp_apps-2.7.0a1/weni/utils/app_config.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.7.0/PKG-INFO` & `weni_rp_apps-2.7.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weni-rp-apps
-Version: 2.7.0
+Version: 2.7.0a1
 Summary: Weni apps for Rapidpro Platform
 License: AGPL-3.0
 Author: jcbalmeida
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

