# Comparing `tmp/atatus-1.5.2.tar.gz` & `tmp/atatus-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atatus-1.5.2.tar", last modified: Wed Jun  7 14:22:20 2023, max compression
+gzip compressed data, was "atatus-1.5.3.tar", last modified: Fri Jun 23 11:55:47 2023, max compression
```

## Comparing `atatus-1.5.2.tar` & `atatus-1.5.3.tar`

### file list

```diff
@@ -1,204 +1,204 @@
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.981720 atatus-1.5.2/
--rw-r--r--   0 apple      (501) staff       (20)     3356 2023-01-04 09:02:24.000000 atatus-1.5.2/LICENSE
--rw-r--r--   0 apple      (501) staff       (20)      110 2019-11-18 06:31:28.000000 atatus-1.5.2/MANIFEST.in
--rw-r--r--   0 apple      (501) staff       (20)     2489 2023-06-07 14:22:20.981848 atatus-1.5.2/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)      991 2023-01-04 09:26:05.000000 atatus-1.5.2/README.rst
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.955969 atatus-1.5.2/atatus/
--rw-r--r--   0 apple      (501) staff       (20)     2826 2022-12-16 06:48:10.000000 atatus-1.5.2/atatus/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    30577 2023-01-03 09:24:18.000000 atatus-1.5.2/atatus/base.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.958361 atatus-1.5.2/atatus/collector/
--rw-r--r--   0 apple      (501) staff       (20)        0 2022-12-16 06:48:10.000000 atatus-1.5.2/atatus/collector/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    27443 2023-06-07 13:34:59.000000 atatus-1.5.2/atatus/collector/base.py
--rw-r--r--   0 apple      (501) staff       (20)    20628 2023-01-03 09:24:18.000000 atatus-1.5.2/atatus/collector/builder.py
--rw-r--r--   0 apple      (501) staff       (20)     1211 2022-12-16 06:48:10.000000 atatus-1.5.2/atatus/collector/hist.py
--rw-r--r--   0 apple      (501) staff       (20)     1195 2022-12-16 06:48:10.000000 atatus-1.5.2/atatus/collector/layer.py
--rw-r--r--   0 apple      (501) staff       (20)     6418 2023-04-29 10:18:47.000000 atatus-1.5.2/atatus/collector/transport.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.958826 atatus-1.5.2/atatus/conf/
--rw-r--r--   0 apple      (501) staff       (20)    35456 2023-06-07 13:34:59.000000 atatus-1.5.2/atatus/conf/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     3840 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/conf/constants.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.959416 atatus-1.5.2/atatus/context/
--rw-r--r--   0 apple      (501) staff       (20)     2619 2019-11-18 10:56:33.000000 atatus-1.5.2/atatus/context/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2757 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/context/base.py
--rw-r--r--   0 apple      (501) staff       (20)     3638 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/context/contextvars.py
--rw-r--r--   0 apple      (501) staff       (20)     3617 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/context/threadlocal.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.959684 atatus-1.5.2/atatus/contrib/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/contrib/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.960161 atatus-1.5.2/atatus/contrib/aiohttp/
--rw-r--r--   0 apple      (501) staff       (20)     2321 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/aiohttp/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     5835 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/aiohttp/middleware.py
--rw-r--r--   0 apple      (501) staff       (20)     2639 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/aiohttp/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.960540 atatus-1.5.2/atatus/contrib/asyncio/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/asyncio/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     3322 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/asyncio/traces.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.960666 atatus-1.5.2/atatus/contrib/celery/
--rw-r--r--   0 apple      (501) staff       (20)     5694 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/celery/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.961756 atatus-1.5.2/atatus/contrib/django/
--rw-r--r--   0 apple      (501) staff       (20)     1789 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/django/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     7863 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/django/apps.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.962009 atatus-1.5.2/atatus/contrib/django/celery/
--rw-r--r--   0 apple      (501) staff       (20)     1588 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/contrib/django/celery/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     1862 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/contrib/django/celery/models.py
--rw-r--r--   0 apple      (501) staff       (20)    13285 2023-06-07 07:23:32.000000 atatus-1.5.2/atatus/contrib/django/client.py
--rw-r--r--   0 apple      (501) staff       (20)     2240 2019-11-18 10:56:34.000000 atatus-1.5.2/atatus/contrib/django/context_processors.py
--rw-r--r--   0 apple      (501) staff       (20)     3384 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/django/handlers.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.962136 atatus-1.5.2/atatus/contrib/django/management/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/contrib/django/management/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.962436 atatus-1.5.2/atatus/contrib/django/management/commands/
--rw-r--r--   0 apple      (501) staff       (20)     1519 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/contrib/django/management/commands/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    13737 2023-01-03 09:24:18.000000 atatus-1.5.2/atatus/contrib/django/management/commands/atatus.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.962918 atatus-1.5.2/atatus/contrib/django/middleware/
--rw-r--r--   0 apple      (501) staff       (20)     9342 2023-06-07 07:23:32.000000 atatus-1.5.2/atatus/contrib/django/middleware/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2262 2019-11-18 11:24:33.000000 atatus-1.5.2/atatus/contrib/django/middleware/wsgi.py
--rw-r--r--   0 apple      (501) staff       (20)     4446 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/django/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.963366 atatus-1.5.2/atatus/contrib/flask/
--rw-r--r--   0 apple      (501) staff       (20)     8515 2022-12-16 06:48:10.000000 atatus-1.5.2/atatus/contrib/flask/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4998 2023-06-07 07:23:32.000000 atatus-1.5.2/atatus/contrib/flask/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.964260 atatus-1.5.2/atatus/contrib/opentelemetry/
--rw-r--r--   0 apple      (501) staff       (20)     1644 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/opentelemetry/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     5592 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/opentelemetry/context.py
--rw-r--r--   0 apple      (501) staff       (20)    12843 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/opentelemetry/span.py
--rw-r--r--   0 apple      (501) staff       (20)    13216 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/opentelemetry/trace.py
--rw-r--r--   0 apple      (501) staff       (20)     3035 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/opentelemetry/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.964660 atatus-1.5.2/atatus/contrib/opentracing/
--rw-r--r--   0 apple      (501) staff       (20)     1886 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/opentracing/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     5778 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/opentracing/span.py
--rw-r--r--   0 apple      (501) staff       (20)     6210 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/opentracing/tracer.py
--rw-r--r--   0 apple      (501) staff       (20)     1818 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/paste.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.964784 atatus-1.5.2/atatus/contrib/pylons/
--rw-r--r--   0 apple      (501) staff       (20)     2134 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/pylons/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.965049 atatus-1.5.2/atatus/contrib/rq/
--rw-r--r--   0 apple      (501) staff       (20)     2378 2019-11-18 11:25:11.000000 atatus-1.5.2/atatus/contrib/rq/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.965679 atatus-1.5.2/atatus/contrib/sanic/
--rw-r--r--   0 apple      (501) staff       (20)    15842 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/sanic/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4270 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/sanic/patch.py
--rw-r--r--   0 apple      (501) staff       (20)     2745 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/sanic/sanic_types.py
--rw-r--r--   0 apple      (501) staff       (20)     6081 2022-12-16 06:48:10.000000 atatus-1.5.2/atatus/contrib/sanic/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.966097 atatus-1.5.2/atatus/contrib/serverless/
--rw-r--r--   0 apple      (501) staff       (20)     1975 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/serverless/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    20636 2023-01-03 09:24:18.000000 atatus-1.5.2/atatus/contrib/serverless/aws.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.966523 atatus-1.5.2/atatus/contrib/starlette/
--rw-r--r--   0 apple      (501) staff       (20)    10726 2022-12-22 14:08:57.000000 atatus-1.5.2/atatus/contrib/starlette/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4863 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/starlette/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.966793 atatus-1.5.2/atatus/contrib/tornado/
--rw-r--r--   0 apple      (501) staff       (20)     3049 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/tornado/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     3371 2022-12-16 06:48:10.000000 atatus-1.5.2/atatus/contrib/tornado/utils.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.966990 atatus-1.5.2/atatus/contrib/twisted/
--rw-r--r--   0 apple      (501) staff       (20)     2449 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/contrib/twisted/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     8231 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/events.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.967606 atatus-1.5.2/atatus/handlers/
--rw-r--r--   0 apple      (501) staff       (20)     1588 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/handlers/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4247 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/handlers/logbook.py
--rw-r--r--   0 apple      (501) staff       (20)    10219 2023-01-03 09:24:18.000000 atatus-1.5.2/atatus/handlers/logging.py
--rw-r--r--   0 apple      (501) staff       (20)     2582 2023-01-03 09:24:18.000000 atatus-1.5.2/atatus/handlers/structlog.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.967995 atatus-1.5.2/atatus/instrumentation/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/instrumentation/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2119 2019-11-18 10:56:35.000000 atatus-1.5.2/atatus/instrumentation/control.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.972791 atatus-1.5.2/atatus/instrumentation/packages/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/instrumentation/packages/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.974223 atatus-1.5.2/atatus/instrumentation/packages/asyncio/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/asyncio/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2699 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/asyncio/aiobotocore.py
--rw-r--r--   0 apple      (501) staff       (20)     4496 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/asyncio/aiohttp_client.py
--rw-r--r--   0 apple      (501) staff       (20)     3031 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/asyncio/aiomysql.py
--rw-r--r--   0 apple      (501) staff       (20)     3189 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/asyncio/aiopg.py
--rw-r--r--   0 apple      (501) staff       (20)     4624 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/asyncio/aioredis.py
--rw-r--r--   0 apple      (501) staff       (20)     3755 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/asyncio/asyncpg.py
--rw-r--r--   0 apple      (501) staff       (20)     1848 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/asyncio/base.py
--rw-r--r--   0 apple      (501) staff       (20)     4330 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/asyncio/elasticsearch.py
--rw-r--r--   0 apple      (501) staff       (20)     2124 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/asyncio/sleep.py
--rw-r--r--   0 apple      (501) staff       (20)    18215 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/azure.py
--rw-r--r--   0 apple      (501) staff       (20)    11063 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/base.py
--rw-r--r--   0 apple      (501) staff       (20)    10984 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/botocore.py
--rw-r--r--   0 apple      (501) staff       (20)     4167 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/cassandra.py
--rw-r--r--   0 apple      (501) staff       (20)    10031 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/dbapi2.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.974473 atatus-1.5.2/atatus/instrumentation/packages/django/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/instrumentation/packages/django/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     2918 2019-11-18 10:56:35.000000 atatus-1.5.2/atatus/instrumentation/packages/django/template.py
--rw-r--r--   0 apple      (501) staff       (20)     7414 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/elasticsearch.py
--rw-r--r--   0 apple      (501) staff       (20)     4443 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/graphql.py
--rw-r--r--   0 apple      (501) staff       (20)     5496 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/httplib2.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.974724 atatus-1.5.2/atatus/instrumentation/packages/httpx/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/httpx/__init__.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.975128 atatus-1.5.2/atatus/instrumentation/packages/httpx/async/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/httpx/async/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     5028 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/httpx/async/httpcore.py
--rw-r--r--   0 apple      (501) staff       (20)     2823 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/httpx/async/httpx.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.975527 atatus-1.5.2/atatus/instrumentation/packages/httpx/sync/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/httpx/sync/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4586 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/httpx/sync/httpcore.py
--rw-r--r--   0 apple      (501) staff       (20)     2749 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/httpx/sync/httpx.py
--rw-r--r--   0 apple      (501) staff       (20)     3674 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/httpx/utils.py
--rw-r--r--   0 apple      (501) staff       (20)     2115 2019-11-18 10:56:35.000000 atatus-1.5.2/atatus/instrumentation/packages/jinja2.py
--rw-r--r--   0 apple      (501) staff       (20)     8759 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/kafka.py
--rw-r--r--   0 apple      (501) staff       (20)     2758 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/mysql.py
--rw-r--r--   0 apple      (501) staff       (20)     2822 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/mysql_connector.py
--rw-r--r--   0 apple      (501) staff       (20)     6121 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/psycopg2.py
--rw-r--r--   0 apple      (501) staff       (20)     3499 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/pylibmc.py
--rw-r--r--   0 apple      (501) staff       (20)     4126 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/pymemcache.py
--rw-r--r--   0 apple      (501) staff       (20)     6227 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/pymongo.py
--rw-r--r--   0 apple      (501) staff       (20)     3154 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/pymssql.py
--rw-r--r--   0 apple      (501) staff       (20)     2368 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/pymysql.py
--rw-r--r--   0 apple      (501) staff       (20)     2359 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/pyodbc.py
--rw-r--r--   0 apple      (501) staff       (20)     3235 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/python_memcached.py
--rw-r--r--   0 apple      (501) staff       (20)     4626 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/redis.py
--rw-r--r--   0 apple      (501) staff       (20)     7001 2023-04-26 05:49:01.000000 atatus-1.5.2/atatus/instrumentation/packages/requests.py
--rw-r--r--   0 apple      (501) staff       (20)     3438 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/sqlite.py
--rw-r--r--   0 apple      (501) staff       (20)     6342 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/tornado.py
--rw-r--r--   0 apple      (501) staff       (20)     5309 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/urllib.py
--rw-r--r--   0 apple      (501) staff       (20)     6363 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/packages/urllib3.py
--rw-r--r--   0 apple      (501) staff       (20)     2097 2019-11-18 10:56:36.000000 atatus-1.5.2/atatus/instrumentation/packages/zlib.py
--rw-r--r--   0 apple      (501) staff       (20)     6211 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/instrumentation/register.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.975770 atatus-1.5.2/atatus/metrics/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/metrics/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    18424 2022-12-22 14:08:57.000000 atatus-1.5.2/atatus/metrics/base_metrics.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.976736 atatus-1.5.2/atatus/metrics/sets/
--rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/metrics/sets/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     1748 2019-11-18 10:56:36.000000 atatus-1.5.2/atatus/metrics/sets/breakdown.py
--rw-r--r--   0 apple      (501) staff       (20)     1857 2019-11-18 11:11:54.000000 atatus-1.5.2/atatus/metrics/sets/cpu.py
--rw-r--r--   0 apple      (501) staff       (20)    11809 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/metrics/sets/cpu_linux.py
--rw-r--r--   0 apple      (501) staff       (20)     2898 2019-11-18 10:56:36.000000 atatus-1.5.2/atatus/metrics/sets/cpu_psutil.py
--rw-r--r--   0 apple      (501) staff       (20)     5450 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/metrics/sets/prometheus.py
--rw-r--r--   0 apple      (501) staff       (20)     2920 2019-11-18 11:25:40.000000 atatus-1.5.2/atatus/middleware.py
--rw-r--r--   0 apple      (501) staff       (20)    14144 2022-12-16 06:48:10.000000 atatus-1.5.2/atatus/processors.py
--rw-r--r--   0 apple      (501) staff       (20)    51580 2022-12-22 05:27:27.000000 atatus-1.5.2/atatus/traces.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.977797 atatus-1.5.2/atatus/transport/
--rw-r--r--   0 apple      (501) staff       (20)     1615 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/transport/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    17353 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/transport/base.py
--rw-r--r--   0 apple      (501) staff       (20)     1840 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/transport/exceptions.py
--rw-r--r--   0 apple      (501) staff       (20)    10167 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/transport/http.py
--rw-r--r--   0 apple      (501) staff       (20)     3906 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/transport/http_base.py
--rw-r--r--   0 apple      (501) staff       (20)     1900 2019-11-18 10:56:37.000000 atatus-1.5.2/atatus/transport/http_urllib3.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.980336 atatus-1.5.2/atatus/utils/
--rw-r--r--   0 apple      (501) staff       (20)     7689 2023-04-26 05:49:01.000000 atatus-1.5.2/atatus/utils/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)     4432 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/utils/cgroup.py
--rw-r--r--   0 apple      (501) staff       (20)     7562 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/utils/cloud.py
--rw-r--r--   0 apple      (501) staff       (20)     3705 2023-04-29 11:08:46.000000 atatus-1.5.2/atatus/utils/compat.py
--rw-r--r--   0 apple      (501) staff       (20)     2536 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/utils/deprecation.py
--rw-r--r--   0 apple      (501) staff       (20)    12347 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/utils/disttracing.py
--rw-r--r--   0 apple      (501) staff       (20)    11290 2023-06-07 07:23:32.000000 atatus-1.5.2/atatus/utils/encoding.py
--rw-r--r--   0 apple      (501) staff       (20)     4207 2022-12-16 06:48:10.000000 atatus-1.5.2/atatus/utils/hw_info.py
--rw-r--r--   0 apple      (501) staff       (20)     2520 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/utils/json_encoder.py
--rw-r--r--   0 apple      (501) staff       (20)     2024 2019-11-18 11:12:02.000000 atatus-1.5.2/atatus/utils/logging.py
--rw-r--r--   0 apple      (501) staff       (20)     2348 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/utils/module_import.py
--rw-r--r--   0 apple      (501) staff       (20)    13225 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/utils/stacks.py
--rw-r--r--   0 apple      (501) staff       (20)     4476 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/utils/threading.py
--rw-r--r--   0 apple      (501) staff       (20)     3756 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/utils/time.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.981552 atatus-1.5.2/atatus/utils/wrapt/
--rw-r--r--   0 apple      (501) staff       (20)      699 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/utils/wrapt/__init__.py
--rw-r--r--   0 apple      (501) staff       (20)    81870 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/utils/wrapt/_wrappers.c
--rw-r--r--   0 apple      (501) staff       (20)     4059 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/utils/wrapt/arguments.py
--rw-r--r--   0 apple      (501) staff       (20)    20127 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/utils/wrapt/decorators.py
--rw-r--r--   0 apple      (501) staff       (20)     7726 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/utils/wrapt/importer.py
--rw-r--r--   0 apple      (501) staff       (20)    32389 2019-11-18 06:31:28.000000 atatus-1.5.2/atatus/utils/wrapt/wrappers.py
--rw-r--r--   0 apple      (501) staff       (20)     4927 2022-12-15 12:32:13.000000 atatus-1.5.2/atatus/utils/wsgi.py
--rw-r--r--   0 apple      (501) staff       (20)     1658 2023-06-07 13:34:59.000000 atatus-1.5.2/atatus/version.py
-drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-07 14:22:20.956832 atatus-1.5.2/atatus.egg-info/
--rw-r--r--   0 apple      (501) staff       (20)     2489 2023-06-07 14:22:20.000000 atatus-1.5.2/atatus.egg-info/PKG-INFO
--rw-r--r--   0 apple      (501) staff       (20)     5743 2023-06-07 14:22:20.000000 atatus-1.5.2/atatus.egg-info/SOURCES.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2023-06-07 14:22:20.000000 atatus-1.5.2/atatus.egg-info/dependency_links.txt
--rw-r--r--   0 apple      (501) staff       (20)        1 2019-11-18 11:35:56.000000 atatus-1.5.2/atatus.egg-info/not-zip-safe
--rw-r--r--   0 apple      (501) staff       (20)      205 2023-06-07 14:22:20.000000 atatus-1.5.2/atatus.egg-info/requires.txt
--rw-r--r--   0 apple      (501) staff       (20)        7 2023-06-07 14:22:20.000000 atatus-1.5.2/atatus.egg-info/top_level.txt
--rw-r--r--   0 apple      (501) staff       (20)      239 2019-11-18 10:56:32.000000 atatus-1.5.2/pyproject.toml
--rw-r--r--   0 apple      (501) staff       (20)     3524 2023-06-07 14:22:20.982408 atatus-1.5.2/setup.cfg
--rw-r--r--   0 apple      (501) staff       (20)     5656 2023-01-04 09:02:24.000000 atatus-1.5.2/setup.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.189203 atatus-1.5.3/
+-rw-r--r--   0 apple      (501) staff       (20)     3356 2023-01-04 09:02:24.000000 atatus-1.5.3/LICENSE
+-rw-r--r--   0 apple      (501) staff       (20)      110 2019-11-18 06:31:28.000000 atatus-1.5.3/MANIFEST.in
+-rw-r--r--   0 apple      (501) staff       (20)     2489 2023-06-23 11:55:47.189319 atatus-1.5.3/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)      991 2023-01-04 09:26:05.000000 atatus-1.5.3/README.rst
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.163434 atatus-1.5.3/atatus/
+-rw-r--r--   0 apple      (501) staff       (20)     2826 2022-12-16 06:48:10.000000 atatus-1.5.3/atatus/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    30577 2023-01-03 09:24:18.000000 atatus-1.5.3/atatus/base.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.165412 atatus-1.5.3/atatus/collector/
+-rw-r--r--   0 apple      (501) staff       (20)        0 2022-12-16 06:48:10.000000 atatus-1.5.3/atatus/collector/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    29596 2023-06-23 10:09:59.000000 atatus-1.5.3/atatus/collector/base.py
+-rw-r--r--   0 apple      (501) staff       (20)    20628 2023-01-03 09:24:18.000000 atatus-1.5.3/atatus/collector/builder.py
+-rw-r--r--   0 apple      (501) staff       (20)     1211 2022-12-16 06:48:10.000000 atatus-1.5.3/atatus/collector/hist.py
+-rw-r--r--   0 apple      (501) staff       (20)     1195 2022-12-16 06:48:10.000000 atatus-1.5.3/atatus/collector/layer.py
+-rw-r--r--   0 apple      (501) staff       (20)     6418 2023-04-29 10:18:47.000000 atatus-1.5.3/atatus/collector/transport.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.166259 atatus-1.5.3/atatus/conf/
+-rw-r--r--   0 apple      (501) staff       (20)    35543 2023-06-23 10:09:59.000000 atatus-1.5.3/atatus/conf/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     3840 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/conf/constants.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.166947 atatus-1.5.3/atatus/context/
+-rw-r--r--   0 apple      (501) staff       (20)     2619 2019-11-18 10:56:33.000000 atatus-1.5.3/atatus/context/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2757 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/context/base.py
+-rw-r--r--   0 apple      (501) staff       (20)     3638 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/context/contextvars.py
+-rw-r--r--   0 apple      (501) staff       (20)     3617 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/context/threadlocal.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.167204 atatus-1.5.3/atatus/contrib/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/contrib/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.167690 atatus-1.5.3/atatus/contrib/aiohttp/
+-rw-r--r--   0 apple      (501) staff       (20)     2321 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/aiohttp/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     5835 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/aiohttp/middleware.py
+-rw-r--r--   0 apple      (501) staff       (20)     2639 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/aiohttp/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.168050 atatus-1.5.3/atatus/contrib/asyncio/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/asyncio/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     3322 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/asyncio/traces.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.168178 atatus-1.5.3/atatus/contrib/celery/
+-rw-r--r--   0 apple      (501) staff       (20)     5694 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/celery/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.169291 atatus-1.5.3/atatus/contrib/django/
+-rw-r--r--   0 apple      (501) staff       (20)     1789 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/django/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     7863 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/django/apps.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.169599 atatus-1.5.3/atatus/contrib/django/celery/
+-rw-r--r--   0 apple      (501) staff       (20)     1588 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/contrib/django/celery/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     1862 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/contrib/django/celery/models.py
+-rw-r--r--   0 apple      (501) staff       (20)    13285 2023-06-07 07:23:32.000000 atatus-1.5.3/atatus/contrib/django/client.py
+-rw-r--r--   0 apple      (501) staff       (20)     2240 2019-11-18 10:56:34.000000 atatus-1.5.3/atatus/contrib/django/context_processors.py
+-rw-r--r--   0 apple      (501) staff       (20)     3384 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/django/handlers.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.169736 atatus-1.5.3/atatus/contrib/django/management/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/contrib/django/management/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.169998 atatus-1.5.3/atatus/contrib/django/management/commands/
+-rw-r--r--   0 apple      (501) staff       (20)     1519 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/contrib/django/management/commands/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    13737 2023-01-03 09:24:18.000000 atatus-1.5.3/atatus/contrib/django/management/commands/atatus.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.170451 atatus-1.5.3/atatus/contrib/django/middleware/
+-rw-r--r--   0 apple      (501) staff       (20)     9342 2023-06-07 07:23:32.000000 atatus-1.5.3/atatus/contrib/django/middleware/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2262 2019-11-18 11:24:33.000000 atatus-1.5.3/atatus/contrib/django/middleware/wsgi.py
+-rw-r--r--   0 apple      (501) staff       (20)     4446 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/django/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.170886 atatus-1.5.3/atatus/contrib/flask/
+-rw-r--r--   0 apple      (501) staff       (20)     8515 2022-12-16 06:48:10.000000 atatus-1.5.3/atatus/contrib/flask/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4998 2023-06-07 07:23:32.000000 atatus-1.5.3/atatus/contrib/flask/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.171908 atatus-1.5.3/atatus/contrib/opentelemetry/
+-rw-r--r--   0 apple      (501) staff       (20)     1644 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/opentelemetry/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     5592 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/opentelemetry/context.py
+-rw-r--r--   0 apple      (501) staff       (20)    12843 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/opentelemetry/span.py
+-rw-r--r--   0 apple      (501) staff       (20)    13216 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/opentelemetry/trace.py
+-rw-r--r--   0 apple      (501) staff       (20)     3035 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/opentelemetry/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.172346 atatus-1.5.3/atatus/contrib/opentracing/
+-rw-r--r--   0 apple      (501) staff       (20)     1886 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/opentracing/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     5778 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/opentracing/span.py
+-rw-r--r--   0 apple      (501) staff       (20)     6210 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/opentracing/tracer.py
+-rw-r--r--   0 apple      (501) staff       (20)     1818 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/paste.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.172614 atatus-1.5.3/atatus/contrib/pylons/
+-rw-r--r--   0 apple      (501) staff       (20)     2134 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/pylons/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.172742 atatus-1.5.3/atatus/contrib/rq/
+-rw-r--r--   0 apple      (501) staff       (20)     2378 2019-11-18 11:25:11.000000 atatus-1.5.3/atatus/contrib/rq/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.173285 atatus-1.5.3/atatus/contrib/sanic/
+-rw-r--r--   0 apple      (501) staff       (20)    15842 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/sanic/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4270 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/sanic/patch.py
+-rw-r--r--   0 apple      (501) staff       (20)     2745 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/sanic/sanic_types.py
+-rw-r--r--   0 apple      (501) staff       (20)     6081 2022-12-16 06:48:10.000000 atatus-1.5.3/atatus/contrib/sanic/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.173657 atatus-1.5.3/atatus/contrib/serverless/
+-rw-r--r--   0 apple      (501) staff       (20)     1975 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/serverless/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    20636 2023-01-03 09:24:18.000000 atatus-1.5.3/atatus/contrib/serverless/aws.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.174065 atatus-1.5.3/atatus/contrib/starlette/
+-rw-r--r--   0 apple      (501) staff       (20)    10726 2022-12-22 14:08:57.000000 atatus-1.5.3/atatus/contrib/starlette/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4863 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/starlette/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.174331 atatus-1.5.3/atatus/contrib/tornado/
+-rw-r--r--   0 apple      (501) staff       (20)     3049 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/tornado/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     3371 2022-12-16 06:48:10.000000 atatus-1.5.3/atatus/contrib/tornado/utils.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.174458 atatus-1.5.3/atatus/contrib/twisted/
+-rw-r--r--   0 apple      (501) staff       (20)     2449 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/contrib/twisted/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     8231 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/events.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.175055 atatus-1.5.3/atatus/handlers/
+-rw-r--r--   0 apple      (501) staff       (20)     1588 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/handlers/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4247 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/handlers/logbook.py
+-rw-r--r--   0 apple      (501) staff       (20)    10219 2023-01-03 09:24:18.000000 atatus-1.5.3/atatus/handlers/logging.py
+-rw-r--r--   0 apple      (501) staff       (20)     2582 2023-01-03 09:24:18.000000 atatus-1.5.3/atatus/handlers/structlog.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.175433 atatus-1.5.3/atatus/instrumentation/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/instrumentation/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2119 2019-11-18 10:56:35.000000 atatus-1.5.3/atatus/instrumentation/control.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.180246 atatus-1.5.3/atatus/instrumentation/packages/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/instrumentation/packages/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.181627 atatus-1.5.3/atatus/instrumentation/packages/asyncio/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/asyncio/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2699 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/asyncio/aiobotocore.py
+-rw-r--r--   0 apple      (501) staff       (20)     4496 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/asyncio/aiohttp_client.py
+-rw-r--r--   0 apple      (501) staff       (20)     3031 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/asyncio/aiomysql.py
+-rw-r--r--   0 apple      (501) staff       (20)     3189 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/asyncio/aiopg.py
+-rw-r--r--   0 apple      (501) staff       (20)     4624 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/asyncio/aioredis.py
+-rw-r--r--   0 apple      (501) staff       (20)     3755 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/asyncio/asyncpg.py
+-rw-r--r--   0 apple      (501) staff       (20)     1848 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/asyncio/base.py
+-rw-r--r--   0 apple      (501) staff       (20)     4330 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/asyncio/elasticsearch.py
+-rw-r--r--   0 apple      (501) staff       (20)     2124 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/asyncio/sleep.py
+-rw-r--r--   0 apple      (501) staff       (20)    18215 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/azure.py
+-rw-r--r--   0 apple      (501) staff       (20)    11063 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/base.py
+-rw-r--r--   0 apple      (501) staff       (20)    10984 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/botocore.py
+-rw-r--r--   0 apple      (501) staff       (20)     4167 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/cassandra.py
+-rw-r--r--   0 apple      (501) staff       (20)    10031 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/dbapi2.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.181882 atatus-1.5.3/atatus/instrumentation/packages/django/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/instrumentation/packages/django/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     2918 2019-11-18 10:56:35.000000 atatus-1.5.3/atatus/instrumentation/packages/django/template.py
+-rw-r--r--   0 apple      (501) staff       (20)     7414 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/elasticsearch.py
+-rw-r--r--   0 apple      (501) staff       (20)     4443 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/graphql.py
+-rw-r--r--   0 apple      (501) staff       (20)     5496 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/httplib2.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.182124 atatus-1.5.3/atatus/instrumentation/packages/httpx/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/httpx/__init__.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.182521 atatus-1.5.3/atatus/instrumentation/packages/httpx/async/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/httpx/async/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     5028 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/httpx/async/httpcore.py
+-rw-r--r--   0 apple      (501) staff       (20)     2823 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/httpx/async/httpx.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.182885 atatus-1.5.3/atatus/instrumentation/packages/httpx/sync/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/httpx/sync/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4586 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/httpx/sync/httpcore.py
+-rw-r--r--   0 apple      (501) staff       (20)     2749 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/httpx/sync/httpx.py
+-rw-r--r--   0 apple      (501) staff       (20)     3674 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/httpx/utils.py
+-rw-r--r--   0 apple      (501) staff       (20)     2115 2019-11-18 10:56:35.000000 atatus-1.5.3/atatus/instrumentation/packages/jinja2.py
+-rw-r--r--   0 apple      (501) staff       (20)     8759 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/kafka.py
+-rw-r--r--   0 apple      (501) staff       (20)     2758 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/mysql.py
+-rw-r--r--   0 apple      (501) staff       (20)     2822 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/mysql_connector.py
+-rw-r--r--   0 apple      (501) staff       (20)     6121 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/psycopg2.py
+-rw-r--r--   0 apple      (501) staff       (20)     3499 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/pylibmc.py
+-rw-r--r--   0 apple      (501) staff       (20)     4126 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/pymemcache.py
+-rw-r--r--   0 apple      (501) staff       (20)     6227 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/pymongo.py
+-rw-r--r--   0 apple      (501) staff       (20)     3154 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/pymssql.py
+-rw-r--r--   0 apple      (501) staff       (20)     2368 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/pymysql.py
+-rw-r--r--   0 apple      (501) staff       (20)     2359 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/pyodbc.py
+-rw-r--r--   0 apple      (501) staff       (20)     3235 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/python_memcached.py
+-rw-r--r--   0 apple      (501) staff       (20)     4626 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/redis.py
+-rw-r--r--   0 apple      (501) staff       (20)     7001 2023-04-26 05:49:01.000000 atatus-1.5.3/atatus/instrumentation/packages/requests.py
+-rw-r--r--   0 apple      (501) staff       (20)     3438 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/sqlite.py
+-rw-r--r--   0 apple      (501) staff       (20)     6342 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/tornado.py
+-rw-r--r--   0 apple      (501) staff       (20)     5309 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/urllib.py
+-rw-r--r--   0 apple      (501) staff       (20)     6363 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/packages/urllib3.py
+-rw-r--r--   0 apple      (501) staff       (20)     2097 2019-11-18 10:56:36.000000 atatus-1.5.3/atatus/instrumentation/packages/zlib.py
+-rw-r--r--   0 apple      (501) staff       (20)     6211 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/instrumentation/register.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.183133 atatus-1.5.3/atatus/metrics/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/metrics/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    18424 2022-12-22 14:08:57.000000 atatus-1.5.3/atatus/metrics/base_metrics.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.184073 atatus-1.5.3/atatus/metrics/sets/
+-rw-r--r--   0 apple      (501) staff       (20)     1591 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/metrics/sets/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     1748 2019-11-18 10:56:36.000000 atatus-1.5.3/atatus/metrics/sets/breakdown.py
+-rw-r--r--   0 apple      (501) staff       (20)     1857 2019-11-18 11:11:54.000000 atatus-1.5.3/atatus/metrics/sets/cpu.py
+-rw-r--r--   0 apple      (501) staff       (20)    11809 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/metrics/sets/cpu_linux.py
+-rw-r--r--   0 apple      (501) staff       (20)     2898 2019-11-18 10:56:36.000000 atatus-1.5.3/atatus/metrics/sets/cpu_psutil.py
+-rw-r--r--   0 apple      (501) staff       (20)     5450 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/metrics/sets/prometheus.py
+-rw-r--r--   0 apple      (501) staff       (20)     2920 2019-11-18 11:25:40.000000 atatus-1.5.3/atatus/middleware.py
+-rw-r--r--   0 apple      (501) staff       (20)    14144 2022-12-16 06:48:10.000000 atatus-1.5.3/atatus/processors.py
+-rw-r--r--   0 apple      (501) staff       (20)    51580 2022-12-22 05:27:27.000000 atatus-1.5.3/atatus/traces.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.185330 atatus-1.5.3/atatus/transport/
+-rw-r--r--   0 apple      (501) staff       (20)     1615 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/transport/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    17353 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/transport/base.py
+-rw-r--r--   0 apple      (501) staff       (20)     1840 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/transport/exceptions.py
+-rw-r--r--   0 apple      (501) staff       (20)    10167 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/transport/http.py
+-rw-r--r--   0 apple      (501) staff       (20)     3906 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/transport/http_base.py
+-rw-r--r--   0 apple      (501) staff       (20)     1900 2019-11-18 10:56:37.000000 atatus-1.5.3/atatus/transport/http_urllib3.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.187919 atatus-1.5.3/atatus/utils/
+-rw-r--r--   0 apple      (501) staff       (20)     7689 2023-04-26 05:49:01.000000 atatus-1.5.3/atatus/utils/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)     4432 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/utils/cgroup.py
+-rw-r--r--   0 apple      (501) staff       (20)     7562 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/utils/cloud.py
+-rw-r--r--   0 apple      (501) staff       (20)     3705 2023-04-29 11:08:46.000000 atatus-1.5.3/atatus/utils/compat.py
+-rw-r--r--   0 apple      (501) staff       (20)     2536 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/utils/deprecation.py
+-rw-r--r--   0 apple      (501) staff       (20)    12347 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/utils/disttracing.py
+-rw-r--r--   0 apple      (501) staff       (20)    11290 2023-06-07 07:23:32.000000 atatus-1.5.3/atatus/utils/encoding.py
+-rw-r--r--   0 apple      (501) staff       (20)     4207 2022-12-16 06:48:10.000000 atatus-1.5.3/atatus/utils/hw_info.py
+-rw-r--r--   0 apple      (501) staff       (20)     2520 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/utils/json_encoder.py
+-rw-r--r--   0 apple      (501) staff       (20)     2024 2019-11-18 11:12:02.000000 atatus-1.5.3/atatus/utils/logging.py
+-rw-r--r--   0 apple      (501) staff       (20)     2348 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/utils/module_import.py
+-rw-r--r--   0 apple      (501) staff       (20)    13225 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/utils/stacks.py
+-rw-r--r--   0 apple      (501) staff       (20)     4476 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/utils/threading.py
+-rw-r--r--   0 apple      (501) staff       (20)     3756 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/utils/time.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.189015 atatus-1.5.3/atatus/utils/wrapt/
+-rw-r--r--   0 apple      (501) staff       (20)      699 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/utils/wrapt/__init__.py
+-rw-r--r--   0 apple      (501) staff       (20)    81870 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/utils/wrapt/_wrappers.c
+-rw-r--r--   0 apple      (501) staff       (20)     4059 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/utils/wrapt/arguments.py
+-rw-r--r--   0 apple      (501) staff       (20)    20127 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/utils/wrapt/decorators.py
+-rw-r--r--   0 apple      (501) staff       (20)     7726 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/utils/wrapt/importer.py
+-rw-r--r--   0 apple      (501) staff       (20)    32389 2019-11-18 06:31:28.000000 atatus-1.5.3/atatus/utils/wrapt/wrappers.py
+-rw-r--r--   0 apple      (501) staff       (20)     4927 2022-12-15 12:32:13.000000 atatus-1.5.3/atatus/utils/wsgi.py
+-rw-r--r--   0 apple      (501) staff       (20)     1658 2023-06-23 10:09:59.000000 atatus-1.5.3/atatus/version.py
+drwxr-xr-x   0 apple      (501) staff       (20)        0 2023-06-23 11:55:47.164196 atatus-1.5.3/atatus.egg-info/
+-rw-r--r--   0 apple      (501) staff       (20)     2489 2023-06-23 11:55:47.000000 atatus-1.5.3/atatus.egg-info/PKG-INFO
+-rw-r--r--   0 apple      (501) staff       (20)     5743 2023-06-23 11:55:47.000000 atatus-1.5.3/atatus.egg-info/SOURCES.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2023-06-23 11:55:47.000000 atatus-1.5.3/atatus.egg-info/dependency_links.txt
+-rw-r--r--   0 apple      (501) staff       (20)        1 2019-11-18 11:35:56.000000 atatus-1.5.3/atatus.egg-info/not-zip-safe
+-rw-r--r--   0 apple      (501) staff       (20)      205 2023-06-23 11:55:47.000000 atatus-1.5.3/atatus.egg-info/requires.txt
+-rw-r--r--   0 apple      (501) staff       (20)        7 2023-06-23 11:55:47.000000 atatus-1.5.3/atatus.egg-info/top_level.txt
+-rw-r--r--   0 apple      (501) staff       (20)      239 2019-11-18 10:56:32.000000 atatus-1.5.3/pyproject.toml
+-rw-r--r--   0 apple      (501) staff       (20)     3524 2023-06-23 11:55:47.189851 atatus-1.5.3/setup.cfg
+-rw-r--r--   0 apple      (501) staff       (20)     5656 2023-01-04 09:02:24.000000 atatus-1.5.3/setup.py
```

### Comparing `atatus-1.5.2/LICENSE` & `atatus-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/PKG-INFO` & `atatus-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atatus
-Version: 1.5.2
+Version: 1.5.3
 Summary: Atatus Python Agent
 Home-page: https://www.atatus.com/for/python
 Author: Atatus
 License: Atatus License
 Project-URL: Documentation, https://docs.atatus.com/docs/application-monitoring/python-agent/overview.html
 Project-URL: Release notes, https://docs.atatus.com/docs/release-notes/python.html
 Description: Atatus APM agent for Python
```

### Comparing `atatus-1.5.2/README.rst` & `atatus-1.5.3/README.rst`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/__init__.py` & `atatus-1.5.3/atatus/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/base.py` & `atatus-1.5.3/atatus/base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/collector/base.py` & `atatus-1.5.3/atatus/collector/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -218,14 +218,40 @@
             except Exception:
                 return None
         return data
 
     def add_error(self, error):
         self._ensure_collector_running()
 
+        skip_event = False
+        if self._config.skip_processor is not None:
+            error_txn_name = ""
+            if "event_transaction_name" in error:
+                error_txn_name = error["event_transaction_name"]
+
+            error_url = ""
+            if "context" in error and \
+                "request" in error["context"] and \
+                "url" in error["context"]["request"] and \
+                "full" in error["context"]["request"]["url"]:
+                    error_url = error["context"]["request"]["url"]["full"]
+            try:
+                skip_event_dict = {}
+                skip_event_dict["name"] = error_txn_name
+                skip_event_dict["url"] = error_url
+                skip_event = self._config.skip_processor(skip_event_dict)
+            except Exception as e:
+                self._error_logger.debug("error skip function failed with exception: %r" % e)
+                pass
+
+        if skip_event == True:
+            if "event_transaction_name" in error:
+                self._error_logger.debug("skipping error event: %r" % error["event_transaction_name"])
+            return
+
         with self._errors_lock:
             if len(self._errors_agg) < 20:
                 self._errors_agg.append(error)
             else:
                 i = random.randrange(20)
                 self._errors_agg[i] = error
 
@@ -366,15 +392,15 @@
             if len(self._analytics_agg) < 10000:
                 skip_event = False
 
                 if self._config.analytics_skip_processor is not None:
                     try:
                         skip_event = self._config.analytics_skip_processor(analytics_txn)
                     except Exception as e:
-                        self._error_logger.debug("skip function failed with exception: %r" % e)
+                        self._error_logger.debug("analytics skip function failed with exception: %r" % e)
                         pass
 
                 if skip_event == False:
                     if self._config.analytics_mask_processor is not None:
                         try:
                             self._config.analytics_mask_processor(analytics_txn)
                         except Exception as e:
@@ -479,15 +505,15 @@
         with self._analytics_lock:
              if len(self._analytics_agg) < 10000:
                 skip_event = False
                 if self._config.analytics_skip_processor is not None:
                     try:
                         skip_event = self._config.analytics_skip_processor(analytics_txn)
                     except Exception as e:
-                        self._error_logger.debug("skip function failed with exception: %r" % e)
+                        self._error_logger.debug("analytics outgoing skip function failed with exception: %r" % e)
                         pass
 
                 if skip_event == False:
                     if self._config.analytics_mask_processor is not None:
                         try:
                             self._config.analytics_mask_processor(analytics_txn)
                         except Exception as e:
@@ -517,14 +543,38 @@
         txn_name = txn["name"]
         if not txn_name:
             return
 
         if txn["duration"] <= 0:
             return
 
+        skip_event = False
+        if self._config.skip_processor is not None:
+            txn_url = ""
+            if "context" in txn and \
+                "request" in txn["context"] and \
+                "url" in txn["context"]["request"] and \
+                "full" in txn["context"]["request"]["url"]:
+                    txn_url = txn["context"]["request"]["url"]["full"]
+            try:
+                skip_event_dict = {}
+                skip_event_dict["name"] = txn_name
+                skip_event_dict["url"] = txn_url
+                skip_event = self._config.skip_processor(skip_event_dict)
+            except Exception as e:
+                self._error_logger.debug("txn skip function failed with exception: %r" % e)
+                pass
+
+        if skip_event == True:
+            self._error_logger.debug("skipping txn event: %r" % txn_name)
+            txn_id = txn["id"]
+            if txn_id in self._spans:
+                del self._spans[txn_id]
+            return
+
         with self._txns_lock:
             if self._config.framework_name:
                 txn_type = self._config.framework_name
             else:
                 txn_type = atatus.PYTHON_AGENT
 
             background = False
```

### Comparing `atatus-1.5.2/atatus/collector/builder.py` & `atatus-1.5.3/atatus/collector/builder.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/collector/hist.py` & `atatus-1.5.3/atatus/collector/hist.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/collector/layer.py` & `atatus-1.5.3/atatus/collector/layer.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/collector/transport.py` & `atatus-1.5.3/atatus/collector/transport.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/conf/__init__.py` & `atatus-1.5.3/atatus/conf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -587,14 +587,15 @@
             "atatus.processors.sanitize_http_request_cookies",
             "atatus.processors.sanitize_http_response_cookies",
             "atatus.processors.sanitize_http_headers",
             "atatus.processors.sanitize_http_wsgi_env",
             "atatus.processors.sanitize_http_request_body",
         ],
     )
+    skip_processor = _ConfigValue("SKIP", type=None, default=None, required=False)    
     analytics_processors = _ListConfigValue(
         "ANALYTICS_PROCESSORS",
         default=[
             "atatus.processors.sanitize_http_request_cookies_analytics",
             "atatus.processors.sanitize_http_response_cookies_analytics",
             "atatus.processors.sanitize_http_headers_analytics",
             "atatus.processors.sanitize_http_request_body_analytics",
```

### Comparing `atatus-1.5.2/atatus/conf/constants.py` & `atatus-1.5.3/atatus/conf/constants.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/context/__init__.py` & `atatus-1.5.3/atatus/context/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/context/base.py` & `atatus-1.5.3/atatus/context/base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/context/contextvars.py` & `atatus-1.5.3/atatus/context/contextvars.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/context/threadlocal.py` & `atatus-1.5.3/atatus/context/threadlocal.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/__init__.py` & `atatus-1.5.3/atatus/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/aiohttp/__init__.py` & `atatus-1.5.3/atatus/contrib/aiohttp/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/aiohttp/middleware.py` & `atatus-1.5.3/atatus/contrib/aiohttp/middleware.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/aiohttp/utils.py` & `atatus-1.5.3/atatus/contrib/aiohttp/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/asyncio/__init__.py` & `atatus-1.5.3/atatus/contrib/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/asyncio/traces.py` & `atatus-1.5.3/atatus/contrib/asyncio/traces.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/celery/__init__.py` & `atatus-1.5.3/atatus/contrib/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/django/__init__.py` & `atatus-1.5.3/atatus/contrib/django/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/django/apps.py` & `atatus-1.5.3/atatus/contrib/django/apps.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/django/celery/__init__.py` & `atatus-1.5.3/atatus/contrib/django/celery/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/django/celery/models.py` & `atatus-1.5.3/atatus/contrib/django/celery/models.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/django/client.py` & `atatus-1.5.3/atatus/contrib/django/client.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/django/context_processors.py` & `atatus-1.5.3/atatus/contrib/django/context_processors.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/django/handlers.py` & `atatus-1.5.3/atatus/contrib/django/handlers.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/django/management/__init__.py` & `atatus-1.5.3/atatus/contrib/django/management/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/django/management/commands/__init__.py` & `atatus-1.5.3/atatus/contrib/django/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/django/management/commands/atatus.py` & `atatus-1.5.3/atatus/contrib/django/management/commands/atatus.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/django/middleware/__init__.py` & `atatus-1.5.3/atatus/contrib/django/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/django/middleware/wsgi.py` & `atatus-1.5.3/atatus/contrib/django/middleware/wsgi.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/django/utils.py` & `atatus-1.5.3/atatus/contrib/django/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/flask/__init__.py` & `atatus-1.5.3/atatus/contrib/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/flask/utils.py` & `atatus-1.5.3/atatus/contrib/flask/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/opentelemetry/__init__.py` & `atatus-1.5.3/atatus/contrib/opentelemetry/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/opentelemetry/context.py` & `atatus-1.5.3/atatus/contrib/opentelemetry/context.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/opentelemetry/span.py` & `atatus-1.5.3/atatus/contrib/opentelemetry/span.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/opentelemetry/trace.py` & `atatus-1.5.3/atatus/contrib/opentelemetry/trace.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/opentelemetry/utils.py` & `atatus-1.5.3/atatus/contrib/opentelemetry/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/opentracing/__init__.py` & `atatus-1.5.3/atatus/contrib/opentracing/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/opentracing/span.py` & `atatus-1.5.3/atatus/contrib/opentracing/span.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/opentracing/tracer.py` & `atatus-1.5.3/atatus/contrib/opentracing/tracer.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/paste.py` & `atatus-1.5.3/atatus/contrib/paste.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/pylons/__init__.py` & `atatus-1.5.3/atatus/contrib/pylons/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/rq/__init__.py` & `atatus-1.5.3/atatus/contrib/rq/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/sanic/__init__.py` & `atatus-1.5.3/atatus/contrib/sanic/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/sanic/patch.py` & `atatus-1.5.3/atatus/contrib/sanic/patch.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/sanic/sanic_types.py` & `atatus-1.5.3/atatus/contrib/sanic/sanic_types.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/sanic/utils.py` & `atatus-1.5.3/atatus/contrib/sanic/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/serverless/__init__.py` & `atatus-1.5.3/atatus/contrib/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/serverless/aws.py` & `atatus-1.5.3/atatus/contrib/serverless/aws.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/starlette/__init__.py` & `atatus-1.5.3/atatus/contrib/starlette/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/starlette/utils.py` & `atatus-1.5.3/atatus/contrib/starlette/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/tornado/__init__.py` & `atatus-1.5.3/atatus/contrib/tornado/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/tornado/utils.py` & `atatus-1.5.3/atatus/contrib/tornado/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/contrib/twisted/__init__.py` & `atatus-1.5.3/atatus/contrib/twisted/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/events.py` & `atatus-1.5.3/atatus/events.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/handlers/__init__.py` & `atatus-1.5.3/atatus/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/handlers/logbook.py` & `atatus-1.5.3/atatus/handlers/logbook.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/handlers/logging.py` & `atatus-1.5.3/atatus/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/handlers/structlog.py` & `atatus-1.5.3/atatus/handlers/structlog.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/__init__.py` & `atatus-1.5.3/atatus/instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/control.py` & `atatus-1.5.3/atatus/instrumentation/control.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/__init__.py` & `atatus-1.5.3/atatus/instrumentation/packages/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/asyncio/__init__.py` & `atatus-1.5.3/atatus/instrumentation/packages/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/asyncio/aiobotocore.py` & `atatus-1.5.3/atatus/instrumentation/packages/asyncio/aiobotocore.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/asyncio/aiohttp_client.py` & `atatus-1.5.3/atatus/instrumentation/packages/asyncio/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/asyncio/aiomysql.py` & `atatus-1.5.3/atatus/instrumentation/packages/asyncio/aiomysql.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/asyncio/aiopg.py` & `atatus-1.5.3/atatus/instrumentation/packages/asyncio/aiopg.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/asyncio/aioredis.py` & `atatus-1.5.3/atatus/instrumentation/packages/asyncio/aioredis.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/asyncio/asyncpg.py` & `atatus-1.5.3/atatus/instrumentation/packages/asyncio/asyncpg.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/asyncio/base.py` & `atatus-1.5.3/atatus/instrumentation/packages/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/asyncio/elasticsearch.py` & `atatus-1.5.3/atatus/instrumentation/packages/asyncio/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/asyncio/sleep.py` & `atatus-1.5.3/atatus/instrumentation/packages/asyncio/sleep.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/azure.py` & `atatus-1.5.3/atatus/instrumentation/packages/azure.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/base.py` & `atatus-1.5.3/atatus/instrumentation/packages/base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/botocore.py` & `atatus-1.5.3/atatus/instrumentation/packages/botocore.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/cassandra.py` & `atatus-1.5.3/atatus/instrumentation/packages/cassandra.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/dbapi2.py` & `atatus-1.5.3/atatus/instrumentation/packages/dbapi2.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/django/__init__.py` & `atatus-1.5.3/atatus/instrumentation/packages/django/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/django/template.py` & `atatus-1.5.3/atatus/instrumentation/packages/django/template.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/elasticsearch.py` & `atatus-1.5.3/atatus/instrumentation/packages/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/graphql.py` & `atatus-1.5.3/atatus/instrumentation/packages/graphql.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/httplib2.py` & `atatus-1.5.3/atatus/instrumentation/packages/httplib2.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/httpx/__init__.py` & `atatus-1.5.3/atatus/instrumentation/packages/httpx/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/httpx/async/__init__.py` & `atatus-1.5.3/atatus/instrumentation/packages/httpx/async/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/httpx/async/httpcore.py` & `atatus-1.5.3/atatus/instrumentation/packages/httpx/async/httpcore.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/httpx/async/httpx.py` & `atatus-1.5.3/atatus/instrumentation/packages/httpx/async/httpx.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/httpx/sync/__init__.py` & `atatus-1.5.3/atatus/instrumentation/packages/httpx/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/httpx/sync/httpcore.py` & `atatus-1.5.3/atatus/instrumentation/packages/httpx/sync/httpcore.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/httpx/sync/httpx.py` & `atatus-1.5.3/atatus/instrumentation/packages/httpx/sync/httpx.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/httpx/utils.py` & `atatus-1.5.3/atatus/instrumentation/packages/httpx/utils.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/jinja2.py` & `atatus-1.5.3/atatus/instrumentation/packages/jinja2.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/kafka.py` & `atatus-1.5.3/atatus/instrumentation/packages/kafka.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/mysql.py` & `atatus-1.5.3/atatus/instrumentation/packages/mysql.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/mysql_connector.py` & `atatus-1.5.3/atatus/instrumentation/packages/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/psycopg2.py` & `atatus-1.5.3/atatus/instrumentation/packages/psycopg2.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/pylibmc.py` & `atatus-1.5.3/atatus/instrumentation/packages/pylibmc.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/pymemcache.py` & `atatus-1.5.3/atatus/instrumentation/packages/pymemcache.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/pymongo.py` & `atatus-1.5.3/atatus/instrumentation/packages/pymongo.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/pymssql.py` & `atatus-1.5.3/atatus/instrumentation/packages/pymssql.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/pymysql.py` & `atatus-1.5.3/atatus/instrumentation/packages/pymysql.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/pyodbc.py` & `atatus-1.5.3/atatus/instrumentation/packages/pyodbc.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/python_memcached.py` & `atatus-1.5.3/atatus/instrumentation/packages/python_memcached.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/redis.py` & `atatus-1.5.3/atatus/instrumentation/packages/redis.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/requests.py` & `atatus-1.5.3/atatus/instrumentation/packages/requests.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/sqlite.py` & `atatus-1.5.3/atatus/instrumentation/packages/sqlite.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/tornado.py` & `atatus-1.5.3/atatus/instrumentation/packages/tornado.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/urllib.py` & `atatus-1.5.3/atatus/instrumentation/packages/urllib.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/urllib3.py` & `atatus-1.5.3/atatus/instrumentation/packages/urllib3.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/packages/zlib.py` & `atatus-1.5.3/atatus/instrumentation/packages/zlib.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/instrumentation/register.py` & `atatus-1.5.3/atatus/instrumentation/register.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/metrics/__init__.py` & `atatus-1.5.3/atatus/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/metrics/base_metrics.py` & `atatus-1.5.3/atatus/metrics/base_metrics.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/metrics/sets/__init__.py` & `atatus-1.5.3/atatus/metrics/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/metrics/sets/breakdown.py` & `atatus-1.5.3/atatus/metrics/sets/breakdown.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/metrics/sets/cpu.py` & `atatus-1.5.3/atatus/metrics/sets/cpu.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/metrics/sets/cpu_linux.py` & `atatus-1.5.3/atatus/metrics/sets/cpu_linux.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/metrics/sets/cpu_psutil.py` & `atatus-1.5.3/atatus/metrics/sets/cpu_psutil.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/metrics/sets/prometheus.py` & `atatus-1.5.3/atatus/metrics/sets/prometheus.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/middleware.py` & `atatus-1.5.3/atatus/middleware.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/processors.py` & `atatus-1.5.3/atatus/processors.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/traces.py` & `atatus-1.5.3/atatus/traces.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/transport/__init__.py` & `atatus-1.5.3/atatus/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/transport/base.py` & `atatus-1.5.3/atatus/transport/base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/transport/exceptions.py` & `atatus-1.5.3/atatus/transport/exceptions.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/transport/http.py` & `atatus-1.5.3/atatus/transport/http.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/transport/http_base.py` & `atatus-1.5.3/atatus/transport/http_base.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/transport/http_urllib3.py` & `atatus-1.5.3/atatus/transport/http_urllib3.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/__init__.py` & `atatus-1.5.3/atatus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/cgroup.py` & `atatus-1.5.3/atatus/utils/cgroup.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/cloud.py` & `atatus-1.5.3/atatus/utils/cloud.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/compat.py` & `atatus-1.5.3/atatus/utils/compat.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/deprecation.py` & `atatus-1.5.3/atatus/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/disttracing.py` & `atatus-1.5.3/atatus/utils/disttracing.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/encoding.py` & `atatus-1.5.3/atatus/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/hw_info.py` & `atatus-1.5.3/atatus/utils/hw_info.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/json_encoder.py` & `atatus-1.5.3/atatus/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/logging.py` & `atatus-1.5.3/atatus/utils/logging.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/module_import.py` & `atatus-1.5.3/atatus/utils/module_import.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/stacks.py` & `atatus-1.5.3/atatus/utils/stacks.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/threading.py` & `atatus-1.5.3/atatus/utils/threading.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/time.py` & `atatus-1.5.3/atatus/utils/time.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/wrapt/__init__.py` & `atatus-1.5.3/atatus/utils/wrapt/__init__.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/wrapt/_wrappers.c` & `atatus-1.5.3/atatus/utils/wrapt/_wrappers.c`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/wrapt/arguments.py` & `atatus-1.5.3/atatus/utils/wrapt/arguments.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/wrapt/decorators.py` & `atatus-1.5.3/atatus/utils/wrapt/decorators.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/wrapt/importer.py` & `atatus-1.5.3/atatus/utils/wrapt/importer.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/wrapt/wrappers.py` & `atatus-1.5.3/atatus/utils/wrapt/wrappers.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/utils/wsgi.py` & `atatus-1.5.3/atatus/utils/wsgi.py`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/atatus/version.py` & `atatus-1.5.3/atatus/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,9 +24,9 @@
 #  FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 #  DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 #  SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 #  CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 #  OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = (1, 5, 2)
+__version__ = (1, 5, 3)
 VERSION = ".".join(map(str, __version__))
```

### Comparing `atatus-1.5.2/atatus.egg-info/PKG-INFO` & `atatus-1.5.3/atatus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atatus
-Version: 1.5.2
+Version: 1.5.3
 Summary: Atatus Python Agent
 Home-page: https://www.atatus.com/for/python
 Author: Atatus
 License: Atatus License
 Project-URL: Documentation, https://docs.atatus.com/docs/application-monitoring/python-agent/overview.html
 Project-URL: Release notes, https://docs.atatus.com/docs/release-notes/python.html
 Description: Atatus APM agent for Python
```

### Comparing `atatus-1.5.2/atatus.egg-info/SOURCES.txt` & `atatus-1.5.3/atatus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/setup.cfg` & `atatus-1.5.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `atatus-1.5.2/setup.py` & `atatus-1.5.3/setup.py`

 * *Files identical despite different names*

