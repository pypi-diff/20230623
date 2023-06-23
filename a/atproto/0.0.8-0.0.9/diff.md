# Comparing `tmp/atproto-0.0.8.tar.gz` & `tmp/atproto-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atproto-0.0.8.tar", max compression
+gzip compressed data, was "atproto-0.0.9.tar", max compression
```

## Comparing `atproto-0.0.8.tar` & `atproto-0.0.9.tar`

### file list

```diff
@@ -1,361 +1,182 @@
--rw-r--r--   0        0        0     1061 2023-05-03 00:31:59.665109 atproto-0.0.8/LICENSE
--rw-r--r--   0        0        0     9562 2023-05-23 13:37:14.635281 atproto-0.0.8/README.md
--rw-r--r--   0        0        0     6148 2023-05-08 17:39:02.583646 atproto-0.0.8/atproto/.DS_Store
--rw-r--r--   0        0        0      403 2023-05-23 13:15:32.484827 atproto-0.0.8/atproto/__init__.py
--rw-r--r--   0        0        0     1782 2023-05-23 13:15:32.484996 atproto-0.0.8/atproto/car/__init__.py
--rw-r--r--   0        0        0     2197 2023-05-23 13:22:55.691309 atproto-0.0.8/atproto/car/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1624 2023-05-23 13:15:32.485078 atproto-0.0.8/atproto/cbor/__init__.py
--rw-r--r--   0        0        0     1994 2023-05-23 13:22:55.691917 atproto-0.0.8/atproto/cbor/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0       49 2023-05-23 13:15:32.485288 atproto-0.0.8/atproto/cid/__init__.py
--rw-r--r--   0        0        0      204 2023-05-23 13:22:55.742052 atproto-0.0.8/atproto/cid/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0       23 2023-05-02 22:04:44.060240 atproto-0.0.8/atproto/cli/__init__.py
--rw-r--r--   0        0        0      152 2023-05-02 22:59:20.005964 atproto-0.0.8/atproto/cli/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2790 2023-05-20 18:39:04.305255 atproto-0.0.8/atproto/codegen/__init__.py
--rw-r--r--   0        0        0     4302 2023-05-20 20:49:49.138233 atproto-0.0.8/atproto/codegen/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0        0 2023-05-03 12:59:20.104132 atproto-0.0.8/atproto/codegen/clients/__init__.py
--rw-r--r--   0        0        0      164 2023-05-05 12:23:15.495715 atproto-0.0.8/atproto/codegen/clients/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1391 2023-05-22 19:34:13.989736 atproto-0.0.8/atproto/codegen/clients/__pycache__/generate_async_client.cpython-38.pyc
--rw-r--r--   0        0        0     1434 2023-05-20 18:39:04.305537 atproto-0.0.8/atproto/codegen/clients/generate_async_client.py
--rw-r--r--   0        0        0        0 2023-04-30 12:18:23.051063 atproto-0.0.8/atproto/codegen/models/__init__.py
--rw-r--r--   0        0        0      163 2023-04-30 12:30:22.568782 atproto-0.0.8/atproto/codegen/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2518 2023-05-23 11:57:59.553439 atproto-0.0.8/atproto/codegen/models/__pycache__/builder.cpython-38.pyc
--rw-r--r--   0        0        0    14688 2023-05-23 12:00:06.207961 atproto-0.0.8/atproto/codegen/models/__pycache__/generator.cpython-38.pyc
--rw-r--r--   0        0        0     2399 2023-05-23 13:15:32.485424 atproto-0.0.8/atproto/codegen/models/builder.py
--rw-r--r--   0        0        0    19213 2023-05-23 11:58:55.694691 atproto-0.0.8/atproto/codegen/models/generator.py
--rw-r--r--   0        0        0        0 2023-04-30 08:15:15.429281 atproto-0.0.8/atproto/codegen/namespaces/__init__.py
--rw-r--r--   0        0        0      167 2023-04-30 08:20:07.529986 atproto-0.0.8/atproto/codegen/namespaces/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2558 2023-05-22 19:34:14.096893 atproto-0.0.8/atproto/codegen/namespaces/__pycache__/builder.cpython-38.pyc
--rw-r--r--   0        0        0     9693 2023-05-22 19:34:14.131154 atproto-0.0.8/atproto/codegen/namespaces/__pycache__/generator.cpython-38.pyc
--rw-r--r--   0        0        0     2546 2023-05-20 18:39:04.306557 atproto-0.0.8/atproto/codegen/namespaces/builder.py
--rw-r--r--   0        0        0    11836 2023-05-20 18:39:04.306950 atproto-0.0.8/atproto/codegen/namespaces/generator.py
--rw-r--r--   0        0        0      992 2023-05-23 13:15:32.485529 atproto-0.0.8/atproto/exceptions.py
--rw-r--r--   0        0        0     4007 2023-05-23 13:15:32.485614 atproto-0.0.8/atproto/firehose/__init__.py
--rw-r--r--   0        0        0     3806 2023-05-23 13:22:55.742964 atproto-0.0.8/atproto/firehose/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     7424 2023-05-23 13:22:55.744233 atproto-0.0.8/atproto/firehose/__pycache__/client.cpython-38.pyc
--rw-r--r--   0        0        0     4554 2023-05-23 13:22:55.851186 atproto-0.0.8/atproto/firehose/__pycache__/models.cpython-38.pyc
--rw-r--r--   0        0        0     8005 2023-05-23 13:15:32.485699 atproto-0.0.8/atproto/firehose/client.py
--rw-r--r--   0        0        0     4183 2023-05-23 13:15:32.485777 atproto-0.0.8/atproto/firehose/models.py
--rw-r--r--   0        0        0     2569 2023-05-16 20:35:11.473690 atproto-0.0.8/atproto/leb128/__init__.py
--rw-r--r--   0        0        0     2927 2023-05-16 20:35:48.620471 atproto-0.0.8/atproto/leb128/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0        0 2023-04-26 20:41:49.793814 atproto-0.0.8/atproto/lexicon/__init__.py
--rw-r--r--   0        0        0      156 2023-04-29 16:30:40.077258 atproto-0.0.8/atproto/lexicon/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     7282 2023-05-20 20:49:49.141577 atproto-0.0.8/atproto/lexicon/__pycache__/models.cpython-38.pyc
--rw-r--r--   0        0        0     3335 2023-05-20 20:49:49.154049 atproto-0.0.8/atproto/lexicon/__pycache__/parser.cpython-38.pyc
--rw-r--r--   0        0        0     4790 2023-05-20 18:39:04.307247 atproto-0.0.8/atproto/lexicon/models.py
--rw-r--r--   0        0        0     3857 2023-05-20 18:39:04.307561 atproto-0.0.8/atproto/lexicon/parser.py
--rw-r--r--   0        0        0     5295 2023-05-20 18:39:04.307762 atproto-0.0.8/atproto/nsid/__init__.py
--rw-r--r--   0        0        0     5708 2023-05-20 19:17:15.545539 atproto-0.0.8/atproto/nsid/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3064 2023-05-20 18:39:04.307957 atproto-0.0.8/atproto/uri/__init__.py
--rw-r--r--   0        0        0     3633 2023-05-20 19:17:15.546578 atproto-0.0.8/atproto/uri/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0        0 2023-05-06 15:48:51.267229 atproto-0.0.8/atproto/xrpc_client/__init__.py
--rw-r--r--   0        0        0      160 2023-05-08 17:46:34.999146 atproto-0.0.8/atproto/xrpc_client/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     4984 2023-05-23 13:22:55.907678 atproto-0.0.8/atproto/xrpc_client/__pycache__/request.cpython-38.pyc
--rw-r--r--   0        0        0     6148 2023-05-08 17:39:02.582090 atproto-0.0.8/atproto/xrpc_client/client/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-03 13:15:19.009756 atproto-0.0.8/atproto/xrpc_client/client/__init__.py
--rw-r--r--   0        0        0      167 2023-05-08 17:46:35.096665 atproto-0.0.8/atproto/xrpc_client/client/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     6807 2023-05-20 19:17:15.548179 atproto-0.0.8/atproto/xrpc_client/client/__pycache__/async_client.cpython-38.pyc
--rw-r--r--   0        0        0      839 2023-05-08 17:46:35.100346 atproto-0.0.8/atproto/xrpc_client/client/__pycache__/async_raw.cpython-38.pyc
--rw-r--r--   0        0        0      775 2023-05-20 19:17:15.561969 atproto-0.0.8/atproto/xrpc_client/client/__pycache__/auth.cpython-38.pyc
--rw-r--r--   0        0        0     4045 2023-05-20 19:17:15.549217 atproto-0.0.8/atproto/xrpc_client/client/__pycache__/base.cpython-38.pyc
--rw-r--r--   0        0        0     6647 2023-05-20 19:17:15.566661 atproto-0.0.8/atproto/xrpc_client/client/__pycache__/client.cpython-38.pyc
--rw-r--r--   0        0        0      817 2023-05-08 17:46:35.203336 atproto-0.0.8/atproto/xrpc_client/client/__pycache__/raw.cpython-38.pyc
--rw-r--r--   0        0        0     7596 2023-05-20 18:39:04.308304 atproto-0.0.8/atproto/xrpc_client/client/async_client.py
--rw-r--r--   0        0        0      489 2023-05-06 15:38:34.659690 atproto-0.0.8/atproto/xrpc_client/client/async_raw.py
--rw-r--r--   0        0        0      414 2023-05-20 18:39:04.308474 atproto-0.0.8/atproto/xrpc_client/client/auth.py
--rw-r--r--   0        0        0     3748 2023-05-20 18:39:04.308652 atproto-0.0.8/atproto/xrpc_client/client/base.py
--rw-r--r--   0        0        0     7105 2023-05-20 18:39:04.308906 atproto-0.0.8/atproto/xrpc_client/client/client.py
--rw-r--r--   0        0        0       76 2023-05-19 20:21:30.527343 atproto-0.0.8/atproto/xrpc_client/client/methods_mixin/__init__.py
--rw-r--r--   0        0        0      254 2023-05-19 20:21:35.021793 atproto-0.0.8/atproto/xrpc_client/client/methods_mixin/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1824 2023-05-20 19:17:15.561351 atproto-0.0.8/atproto/xrpc_client/client/methods_mixin/__pycache__/session.cpython-38.pyc
--rw-r--r--   0        0        0     1311 2023-05-20 18:39:04.309222 atproto-0.0.8/atproto/xrpc_client/client/methods_mixin/session.py
--rw-r--r--   0        0        0      469 2023-05-06 15:38:34.668321 atproto-0.0.8/atproto/xrpc_client/client/raw.py
--rw-r--r--   0        0        0    12159 2023-05-23 12:20:32.652399 atproto-0.0.8/atproto/xrpc_client/models/__init__.py
--rw-r--r--   0        0        0     7929 2023-05-23 12:20:37.588003 atproto-0.0.8/atproto/xrpc_client/models/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1252 2023-05-09 15:13:37.111548 atproto-0.0.8/atproto/xrpc_client/models/__pycache__/base.cpython-38.pyc
--rw-r--r--   0        0        0     1198 2023-05-09 15:13:37.119249 atproto-0.0.8/atproto/xrpc_client/models/__pycache__/blob_ref.cpython-38.pyc
--rw-r--r--   0        0        0      478 2023-05-23 13:22:55.904085 atproto-0.0.8/atproto/xrpc_client/models/__pycache__/common.cpython-38.pyc
--rw-r--r--   0        0        0      717 2023-05-23 12:20:37.797349 atproto-0.0.8/atproto/xrpc_client/models/__pycache__/type_conversion.cpython-38.pyc
--rw-r--r--   0        0        0     3705 2023-05-23 13:22:55.900853 atproto-0.0.8/atproto/xrpc_client/models/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.232068 atproto-0.0.8/atproto/xrpc_client/models/app/__init__.py
--rw-r--r--   0        0        0      171 2023-05-23 12:20:37.588371 atproto-0.0.8/atproto/xrpc_client/models/app/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.231687 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/__init__.py
--rw-r--r--   0        0        0      176 2023-05-23 12:20:37.588657 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.232219 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__init__.py
--rw-r--r--   0        0        0      182 2023-05-23 12:20:37.588931 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3611 2023-05-23 12:47:54.117354 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/defs.cpython-38.pyc
--rw-r--r--   0        0        0      904 2023-05-23 12:47:54.119984 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/get_preferences.cpython-38.pyc
--rw-r--r--   0        0        0      746 2023-05-23 12:47:54.120520 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/get_profile.cpython-38.pyc
--rw-r--r--   0        0        0      984 2023-05-23 12:47:54.120974 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/get_profiles.cpython-38.pyc
--rw-r--r--   0        0        0     1074 2023-05-23 12:47:54.121541 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/get_suggestions.cpython-38.pyc
--rw-r--r--   0        0        0      845 2023-05-23 12:47:54.122123 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/profile.cpython-38.pyc
--rw-r--r--   0        0        0      667 2023-05-23 12:47:54.122856 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/put_preferences.cpython-38.pyc
--rw-r--r--   0        0        0     1099 2023-05-23 12:47:54.123322 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/search_actors.cpython-38.pyc
--rw-r--r--   0        0        0     1059 2023-05-23 12:47:54.123945 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/__pycache__/search_actors_typeahead.cpython-38.pyc
--rw-r--r--   0        0        0     3804 2023-05-23 12:46:04.227082 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/defs.py
--rw-r--r--   0        0        0      759 2023-05-23 12:46:04.188467 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py
--rw-r--r--   0        0        0      800 2023-05-23 12:46:04.122115 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/get_profile.py
--rw-r--r--   0        0        0      819 2023-05-23 12:46:04.251683 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py
--rw-r--r--   0        0        0      916 2023-05-23 12:46:04.134673 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py
--rw-r--r--   0        0        0      846 2023-05-23 12:46:04.201050 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/profile.py
--rw-r--r--   0        0        0      631 2023-05-23 12:46:04.221737 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py
--rw-r--r--   0        0        0      955 2023-05-23 12:46:04.230163 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/search_actors.py
--rw-r--r--   0        0        0      884 2023-05-23 12:46:04.146020 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.260022 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/__init__.py
--rw-r--r--   0        0        0      182 2023-05-23 12:20:37.596347 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1693 2023-05-23 12:47:54.124803 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/__pycache__/external.cpython-38.pyc
--rw-r--r--   0        0        0     1577 2023-05-23 12:47:54.126191 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/__pycache__/images.cpython-38.pyc
--rw-r--r--   0        0        0     2296 2023-05-23 12:47:54.127319 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/__pycache__/record.cpython-38.pyc
--rw-r--r--   0        0        0     1207 2023-05-23 12:47:54.128605 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/__pycache__/record_with_media.cpython-38.pyc
--rw-r--r--   0        0        0     1561 2023-05-23 12:46:04.112166 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/external.py
--rw-r--r--   0        0        0     1397 2023-05-23 12:46:04.137452 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/images.py
--rw-r--r--   0        0        0     2260 2023-05-23 12:46:04.097432 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/record.py
--rw-r--r--   0        0        0     1181 2023-05-23 12:46:04.150112 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.272327 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__init__.py
--rw-r--r--   0        0        0      181 2023-05-23 12:20:37.606251 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5207 2023-05-23 12:47:54.130034 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/defs.cpython-38.pyc
--rw-r--r--   0        0        0     1485 2023-05-23 13:22:55.861815 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/describe_feed_generator.cpython-38.pyc
--rw-r--r--   0        0        0      976 2023-05-23 13:22:55.862696 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/generator.cpython-38.pyc
--rw-r--r--   0        0        0     1086 2023-05-23 13:22:55.863299 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_actor_feeds.cpython-38.pyc
--rw-r--r--   0        0        0     1084 2023-05-23 12:47:54.134744 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_author_feed.cpython-38.pyc
--rw-r--r--   0        0        0     1063 2023-05-23 13:22:55.864301 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_feed.cpython-38.pyc
--rw-r--r--   0        0        0      975 2023-05-23 13:22:55.864907 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_feed_generator.cpython-38.pyc
--rw-r--r--   0        0        0      987 2023-05-23 13:22:55.865494 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_feed_generators.cpython-38.pyc
--rw-r--r--   0        0        0     1092 2023-05-23 13:22:55.866062 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_feed_skeleton.cpython-38.pyc
--rw-r--r--   0        0        0     1514 2023-05-23 12:47:54.137810 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_likes.cpython-38.pyc
--rw-r--r--   0        0        0     1113 2023-05-23 12:47:54.138680 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_post_thread.cpython-38.pyc
--rw-r--r--   0        0        0      955 2023-05-23 12:47:54.139271 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_posts.cpython-38.pyc
--rw-r--r--   0        0        0     1163 2023-05-23 12:47:54.139877 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_reposted_by.cpython-38.pyc
--rw-r--r--   0        0        0     1096 2023-05-23 12:47:54.140597 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/get_timeline.cpython-38.pyc
--rw-r--r--   0        0        0      710 2023-05-23 12:47:54.141292 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/like.cpython-38.pyc
--rw-r--r--   0        0        0     2316 2023-05-23 12:47:54.141934 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/post.cpython-38.pyc
--rw-r--r--   0        0        0      716 2023-05-23 12:47:54.142986 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/__pycache__/repost.cpython-38.pyc
--rw-r--r--   0        0        0     5618 2023-05-23 12:46:04.089600 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/defs.py
--rw-r--r--   0        0        0     1290 2023-05-23 13:17:54.948947 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/describe_feed_generator.py
--rw-r--r--   0        0        0      983 2023-05-23 13:17:54.949125 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/generator.py
--rw-r--r--   0        0        0      937 2023-05-23 13:17:54.949233 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_actor_feeds.py
--rw-r--r--   0        0        0      934 2023-05-23 12:46:04.164219 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py
--rw-r--r--   0        0        0      920 2023-05-23 13:17:54.949348 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_feed.py
--rw-r--r--   0        0        0      839 2023-05-23 13:17:54.949458 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_feed_generator.py
--rw-r--r--   0        0        0      814 2023-05-23 13:17:54.949579 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_feed_generators.py
--rw-r--r--   0        0        0      940 2023-05-23 13:17:54.949678 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_feed_skeleton.py
--rw-r--r--   0        0        0     1305 2023-05-23 12:46:04.104935 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_likes.py
--rw-r--r--   0        0        0      981 2023-05-23 12:46:04.086841 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py
--rw-r--r--   0        0        0      789 2023-05-23 12:46:04.085794 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_posts.py
--rw-r--r--   0        0        0     1047 2023-05-23 12:46:04.207862 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py
--rw-r--r--   0        0        0      957 2023-05-23 12:46:04.228584 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py
--rw-r--r--   0        0        0      684 2023-05-23 12:46:04.219385 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/like.py
--rw-r--r--   0        0        0     2205 2023-05-23 12:46:04.131722 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/post.py
--rw-r--r--   0        0        0      688 2023-05-23 12:46:04.115640 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/repost.py
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.297829 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__init__.py
--rw-r--r--   0        0        0      182 2023-05-23 12:20:37.678553 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      629 2023-05-23 12:47:54.143669 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/block.cpython-38.pyc
--rw-r--r--   0        0        0     2132 2023-05-23 12:47:54.144265 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/defs.cpython-38.pyc
--rw-r--r--   0        0        0      632 2023-05-23 12:47:54.145318 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/follow.cpython-38.pyc
--rw-r--r--   0        0        0     1059 2023-05-23 12:47:54.145814 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/get_blocks.cpython-38.pyc
--rw-r--r--   0        0        0     1107 2023-05-23 12:47:54.146456 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/get_followers.cpython-38.pyc
--rw-r--r--   0        0        0     1099 2023-05-23 12:47:54.147131 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/get_follows.cpython-38.pyc
--rw-r--r--   0        0        0     1118 2023-05-23 12:47:54.147750 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/get_list.cpython-38.pyc
--rw-r--r--   0        0        0     1065 2023-05-23 12:47:54.148387 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/get_list_mutes.cpython-38.pyc
--rw-r--r--   0        0        0     1069 2023-05-23 12:47:54.148995 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/get_lists.cpython-38.pyc
--rw-r--r--   0        0        0     1055 2023-05-23 12:47:54.149567 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/get_mutes.cpython-38.pyc
--rw-r--r--   0        0        0      998 2023-05-23 12:47:54.150896 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/list.cpython-38.pyc
--rw-r--r--   0        0        0      654 2023-05-23 12:47:54.151492 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/listitem.cpython-38.pyc
--rw-r--r--   0        0        0      569 2023-05-23 12:47:54.152006 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/mute_actor.cpython-38.pyc
--rw-r--r--   0        0        0      577 2023-05-23 12:47:54.152434 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/mute_actor_list.cpython-38.pyc
--rw-r--r--   0        0        0      573 2023-05-23 12:47:54.152846 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/unmute_actor.cpython-38.pyc
--rw-r--r--   0        0        0      581 2023-05-23 12:47:54.153246 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/__pycache__/unmute_actor_list.cpython-38.pyc
--rw-r--r--   0        0        0      615 2023-05-23 12:46:04.220606 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/block.py
--rw-r--r--   0        0        0     2141 2023-05-23 12:46:04.152826 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/defs.py
--rw-r--r--   0        0        0      617 2023-05-23 12:46:04.091787 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/follow.py
--rw-r--r--   0        0        0      906 2023-05-23 12:46:04.212768 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py
--rw-r--r--   0        0        0     1008 2023-05-23 12:46:04.222871 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_followers.py
--rw-r--r--   0        0        0     1000 2023-05-23 12:46:04.247615 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_follows.py
--rw-r--r--   0        0        0      980 2023-05-23 12:46:04.143128 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_list.py
--rw-r--r--   0        0        0      907 2023-05-23 12:46:04.217992 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py
--rw-r--r--   0        0        0      925 2023-05-23 12:46:04.171102 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_lists.py
--rw-r--r--   0        0        0      902 2023-05-23 12:46:04.183851 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py
--rw-r--r--   0        0        0     1002 2023-05-23 12:46:04.238659 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/list.py
--rw-r--r--   0        0        0      645 2023-05-23 12:46:04.113819 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/listitem.py
--rw-r--r--   0        0        0      541 2023-05-23 12:46:04.202067 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py
--rw-r--r--   0        0        0      543 2023-05-23 12:46:04.128157 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py
--rw-r--r--   0        0        0      543 2023-05-23 12:46:04.174592 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py
--rw-r--r--   0        0        0      545 2023-05-23 12:46:04.144595 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.313012 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/__init__.py
--rw-r--r--   0        0        0      189 2023-05-23 12:20:37.700822 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      919 2023-05-23 12:47:54.153845 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/__pycache__/get_unread_count.cpython-38.pyc
--rw-r--r--   0        0        0     1811 2023-05-23 12:47:54.154456 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/__pycache__/list_notifications.cpython-38.pyc
--rw-r--r--   0        0        0      586 2023-05-23 12:47:54.155305 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/__pycache__/update_seen.cpython-38.pyc
--rw-r--r--   0        0        0      756 2023-05-23 12:46:04.126657 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py
--rw-r--r--   0        0        0     1689 2023-05-23 12:46:04.199564 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py
--rw-r--r--   0        0        0      552 2023-05-23 12:46:04.248985 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/update_seen.py
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.313862 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/richtext/__init__.py
--rw-r--r--   0        0        0      185 2023-05-23 12:20:37.704189 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/richtext/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1891 2023-05-23 12:47:54.155915 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/richtext/__pycache__/facet.cpython-38.pyc
--rw-r--r--   0        0        0     1575 2023-05-23 12:46:04.215466 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/richtext/facet.py
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.314175 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/unspecced/__init__.py
--rw-r--r--   0        0        0      186 2023-05-23 12:20:37.705487 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/unspecced/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1116 2023-05-23 12:47:54.156950 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/unspecced/__pycache__/get_popular.cpython-38.pyc
--rw-r--r--   0        0        0      971 2023-05-23 12:46:04.210357 atproto-0.0.8/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py
--rw-r--r--   0        0        0      553 2023-05-08 18:09:02.748635 atproto-0.0.8/atproto/xrpc_client/models/base.py
--rw-r--r--   0        0        0      713 2023-05-08 17:32:37.842360 atproto-0.0.8/atproto/xrpc_client/models/blob_ref.py
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.314490 atproto-0.0.8/atproto/xrpc_client/models/com/__init__.py
--rw-r--r--   0        0        0      171 2023-05-23 12:20:37.706508 atproto-0.0.8/atproto/xrpc_client/models/com/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.315041 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/__init__.py
--rw-r--r--   0        0        0      179 2023-05-23 12:20:37.706817 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.314977 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__init__.py
--rw-r--r--   0        0        0      185 2023-05-23 12:20:37.707109 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     7982 2023-05-23 12:47:54.158814 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/defs.cpython-38.pyc
--rw-r--r--   0        0        0      602 2023-05-23 12:47:54.162735 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/disable_account_invites.cpython-38.pyc
--rw-r--r--   0        0        0      698 2023-05-23 12:47:54.163183 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/disable_invite_codes.cpython-38.pyc
--rw-r--r--   0        0        0      600 2023-05-23 12:47:54.163668 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/enable_account_invites.cpython-38.pyc
--rw-r--r--   0        0        0     1117 2023-05-23 12:47:54.164126 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/get_invite_codes.cpython-38.pyc
--rw-r--r--   0        0        0      768 2023-05-23 12:47:54.164829 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/get_moderation_action.cpython-38.pyc
--rw-r--r--   0        0        0     1139 2023-05-23 12:47:54.165341 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/get_moderation_actions.cpython-38.pyc
--rw-r--r--   0        0        0      768 2023-05-23 12:47:54.166203 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/get_moderation_report.cpython-38.pyc
--rw-r--r--   0        0        0     1217 2023-05-23 12:47:54.166807 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/get_moderation_reports.cpython-38.pyc
--rw-r--r--   0        0        0      793 2023-05-23 12:47:54.167491 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/get_record.cpython-38.pyc
--rw-r--r--   0        0        0      742 2023-05-23 12:47:54.167957 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/get_repo.cpython-38.pyc
--rw-r--r--   0        0        0      838 2023-05-23 12:47:54.168422 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/resolve_moderation_reports.cpython-38.pyc
--rw-r--r--   0        0        0      810 2023-05-23 12:47:54.168928 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/reverse_moderation_action.cpython-38.pyc
--rw-r--r--   0        0        0     1140 2023-05-23 12:47:54.169453 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/search_repos.cpython-38.pyc
--rw-r--r--   0        0        0     1099 2023-05-23 12:47:54.170110 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/take_moderation_action.cpython-38.pyc
--rw-r--r--   0        0        0      613 2023-05-23 12:47:54.170659 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/update_account_email.cpython-38.pyc
--rw-r--r--   0        0        0      612 2023-05-23 12:47:54.171078 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/__pycache__/update_account_handle.cpython-38.pyc
--rw-r--r--   0        0        0     9308 2023-05-23 12:46:04.244397 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/defs.py
--rw-r--r--   0        0        0      560 2023-05-23 12:46:04.167950 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py
--rw-r--r--   0        0        0      658 2023-05-23 12:46:04.241323 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py
--rw-r--r--   0        0        0      559 2023-05-23 12:46:04.140269 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py
--rw-r--r--   0        0        0      966 2023-05-23 12:46:04.082872 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py
--rw-r--r--   0        0        0      806 2023-05-23 12:46:04.081875 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py
--rw-r--r--   0        0        0      987 2023-05-23 12:46:04.246013 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py
--rw-r--r--   0        0        0      806 2023-05-23 12:46:04.214076 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py
--rw-r--r--   0        0        0     1095 2023-05-23 12:46:04.118692 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py
--rw-r--r--   0        0        0      839 2023-05-23 12:46:04.240049 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_record.py
--rw-r--r--   0        0        0      790 2023-05-23 12:46:04.083804 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_repo.py
--rw-r--r--   0        0        0      880 2023-05-23 12:46:04.095464 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py
--rw-r--r--   0        0        0      851 2023-05-23 12:46:04.232996 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py
--rw-r--r--   0        0        0     1011 2023-05-23 12:46:04.099316 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/search_repos.py
--rw-r--r--   0        0        0     1228 2023-05-23 12:46:04.100698 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py
--rw-r--r--   0        0        0      605 2023-05-23 12:46:04.103528 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py
--rw-r--r--   0        0        0      578 2023-05-23 12:46:04.176127 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.328520 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/identity/__init__.py
--rw-r--r--   0        0        0      188 2023-05-23 12:20:37.720719 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/identity/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      910 2023-05-23 12:47:54.171703 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/identity/__pycache__/resolve_handle.cpython-38.pyc
--rw-r--r--   0        0        0      588 2023-05-23 12:47:54.172262 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/identity/__pycache__/update_handle.cpython-38.pyc
--rw-r--r--   0        0        0      815 2023-05-23 12:46:04.096343 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py
--rw-r--r--   0        0        0      552 2023-05-23 12:46:04.235698 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/identity/update_handle.py
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.330357 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/__init__.py
--rw-r--r--   0        0        0      185 2023-05-23 12:20:37.722558 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      825 2023-05-23 12:47:54.172849 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/__pycache__/defs.cpython-38.pyc
--rw-r--r--   0        0        0     1149 2023-05-23 12:47:54.173445 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/__pycache__/query_labels.cpython-38.pyc
--rw-r--r--   0        0        0     1455 2023-05-23 13:22:55.885962 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/__pycache__/subscribe_labels.cpython-38.pyc
--rw-r--r--   0        0        0     1173 2023-05-23 12:46:04.206598 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/defs.py
--rw-r--r--   0        0        0     1215 2023-05-23 12:46:04.216799 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/query_labels.py
--rw-r--r--   0        0        0     1214 2023-05-23 13:15:32.486009 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.331439 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/__init__.py
--rw-r--r--   0        0        0      190 2023-05-23 12:20:37.725149 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1298 2023-05-23 12:47:54.175004 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/__pycache__/create_report.cpython-38.pyc
--rw-r--r--   0        0        0      631 2023-05-23 12:47:54.175705 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/__pycache__/defs.cpython-38.pyc
--rw-r--r--   0        0        0     1351 2023-05-23 12:46:04.080807 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/create_report.py
--rw-r--r--   0        0        0      845 2023-05-23 12:46:04.148689 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/defs.py
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.331744 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__init__.py
--rw-r--r--   0        0        0      184 2023-05-23 12:20:37.726858 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2023 2023-05-23 12:47:54.176304 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/apply_writes.cpython-38.pyc
--rw-r--r--   0        0        0     1060 2023-05-23 12:47:54.177292 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/create_record.cpython-38.pyc
--rw-r--r--   0        0        0      726 2023-05-23 12:47:54.177928 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/delete_record.cpython-38.pyc
--rw-r--r--   0        0        0      994 2023-05-23 12:47:54.178471 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/describe_repo.cpython-38.pyc
--rw-r--r--   0        0        0      980 2023-05-23 12:47:54.179077 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/get_record.cpython-38.pyc
--rw-r--r--   0        0        0     1589 2023-05-23 12:47:54.179796 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/list_records.cpython-38.pyc
--rw-r--r--   0        0        0     1073 2023-05-23 12:47:54.180837 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/put_record.cpython-38.pyc
--rw-r--r--   0        0        0      647 2023-05-23 12:47:54.181593 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/rebase_repo.cpython-38.pyc
--rw-r--r--   0        0        0      636 2023-05-23 12:47:54.182047 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/strong_ref.cpython-38.pyc
--rw-r--r--   0        0        0      752 2023-05-23 12:47:54.182530 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/__pycache__/upload_blob.cpython-38.pyc
--rw-r--r--   0        0        0     1881 2023-05-23 12:46:04.141752 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py
--rw-r--r--   0        0        0     1093 2023-05-23 12:46:04.094591 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/create_record.py
--rw-r--r--   0        0        0      874 2023-05-23 12:46:04.093696 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/delete_record.py
--rw-r--r--   0        0        0      910 2023-05-23 12:46:04.254360 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py
--rw-r--r--   0        0        0     1062 2023-05-23 12:46:04.211615 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/get_record.py
--rw-r--r--   0        0        0     1606 2023-05-23 12:46:04.172805 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/list_records.py
--rw-r--r--   0        0        0     1160 2023-05-23 12:46:04.203673 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/put_record.py
--rw-r--r--   0        0        0      679 2023-05-23 12:46:04.151464 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py
--rw-r--r--   0        0        0      604 2023-05-23 12:46:04.075614 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py
--rw-r--r--   0        0        0      704 2023-05-23 12:46:04.182163 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.342245 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__init__.py
--rw-r--r--   0        0        0      186 2023-05-23 12:20:37.744700 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     1085 2023-05-23 12:47:54.183210 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/create_account.cpython-38.pyc
--rw-r--r--   0        0        0     1045 2023-05-23 12:47:54.183907 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/create_app_password.cpython-38.pyc
--rw-r--r--   0        0        0      940 2023-05-23 12:47:54.184499 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/create_invite_code.cpython-38.pyc
--rw-r--r--   0        0        0     1468 2023-05-23 12:47:54.185098 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/create_invite_codes.cpython-38.pyc
--rw-r--r--   0        0        0     1002 2023-05-23 12:47:54.186183 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/create_session.cpython-38.pyc
--rw-r--r--   0        0        0     1166 2023-05-23 12:47:54.187083 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/defs.cpython-38.pyc
--rw-r--r--   0        0        0      620 2023-05-23 12:47:54.187985 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/delete_account.cpython-38.pyc
--rw-r--r--   0        0        0      192 2023-05-23 12:47:54.188563 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/delete_session.cpython-38.pyc
--rw-r--r--   0        0        0     1232 2023-05-23 12:47:54.189086 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/describe_server.cpython-38.pyc
--rw-r--r--   0        0        0     1082 2023-05-23 12:47:54.189898 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/get_account_invite_codes.cpython-38.pyc
--rw-r--r--   0        0        0      672 2023-05-23 12:47:54.190616 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/get_session.cpython-38.pyc
--rw-r--r--   0        0        0     1098 2023-05-23 12:47:54.191147 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/list_app_passwords.cpython-38.pyc
--rw-r--r--   0        0        0      655 2023-05-23 12:47:54.191788 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/refresh_session.cpython-38.pyc
--rw-r--r--   0        0        0      200 2023-05-23 12:47:54.192255 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/request_account_delete.cpython-38.pyc
--rw-r--r--   0        0        0      600 2023-05-23 12:47:54.192577 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/request_password_reset.cpython-38.pyc
--rw-r--r--   0        0        0      605 2023-05-23 12:47:54.192992 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/reset_password.cpython-38.pyc
--rw-r--r--   0        0        0      593 2023-05-23 12:47:54.193444 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/__pycache__/revoke_app_password.cpython-38.pyc
--rw-r--r--   0        0        0     1033 2023-05-23 12:46:04.138659 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_account.py
--rw-r--r--   0        0        0      956 2023-05-23 12:46:04.231476 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_app_password.py
--rw-r--r--   0        0        0      789 2023-05-23 12:46:04.084741 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py
--rw-r--r--   0        0        0     1198 2023-05-23 12:46:04.192606 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py
--rw-r--r--   0        0        0      973 2023-05-23 12:46:04.107533 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_session.py
--rw-r--r--   0        0        0     1130 2023-05-23 12:46:04.129873 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/defs.py
--rw-r--r--   0        0        0      603 2023-05-23 12:46:04.180564 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/delete_account.py
--rw-r--r--   0        0        0      323 2023-05-23 12:46:15.959008 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/delete_session.py
--rw-r--r--   0        0        0     1122 2023-05-23 12:46:04.077798 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/describe_server.py
--rw-r--r--   0        0        0      926 2023-05-23 12:46:04.189870 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py
--rw-r--r--   0        0        0      643 2023-05-23 12:46:04.079399 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/get_session.py
--rw-r--r--   0        0        0      937 2023-05-23 12:46:04.147249 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py
--rw-r--r--   0        0        0      655 2023-05-23 12:46:04.123826 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/refresh_session.py
--rw-r--r--   0        0        0      323 2023-05-23 12:46:15.959972 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/request_account_delete.py
--rw-r--r--   0        0        0      556 2023-05-23 12:46:04.196601 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py
--rw-r--r--   0        0        0      581 2023-05-23 12:46:04.186742 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/reset_password.py
--rw-r--r--   0        0        0      551 2023-05-23 12:46:04.209154 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py
--rw-r--r--   0        0        0      323 2023-05-23 12:20:32.352400 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__init__.py
--rw-r--r--   0        0        0      184 2023-05-23 12:20:37.764138 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0      692 2023-05-23 12:47:54.194174 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/get_blob.cpython-38.pyc
--rw-r--r--   0        0        0      714 2023-05-23 12:47:54.194706 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/get_blocks.cpython-38.pyc
--rw-r--r--   0        0        0      733 2023-05-23 12:47:54.195227 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/get_checkout.cpython-38.pyc
--rw-r--r--   0        0        0      970 2023-05-23 12:47:54.195765 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/get_commit_path.cpython-38.pyc
--rw-r--r--   0        0        0      800 2023-05-23 12:47:54.196414 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/get_head.cpython-38.pyc
--rw-r--r--   0        0        0      767 2023-05-23 12:47:54.196929 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/get_record.cpython-38.pyc
--rw-r--r--   0        0        0      760 2023-05-23 12:47:54.197422 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/get_repo.cpython-38.pyc
--rw-r--r--   0        0        0      954 2023-05-23 12:47:54.197919 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/list_blobs.cpython-38.pyc
--rw-r--r--   0        0        0     1383 2023-05-23 12:47:54.198584 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/list_repos.cpython-38.pyc
--rw-r--r--   0        0        0      591 2023-05-23 12:47:54.199365 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/notify_of_update.cpython-38.pyc
--rw-r--r--   0        0        0      586 2023-05-23 12:47:54.199850 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/request_crawl.cpython-38.pyc
--rw-r--r--   0        0        0     2877 2023-05-23 13:22:55.899006 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/__pycache__/subscribe_repos.cpython-38.pyc
--rw-r--r--   0        0        0      706 2023-05-23 12:46:04.179091 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_blob.py
--rw-r--r--   0        0        0      693 2023-05-23 12:46:04.109156 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py
--rw-r--r--   0        0        0      765 2023-05-23 12:46:04.205112 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py
--rw-r--r--   0        0        0      885 2023-05-23 12:46:04.198103 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py
--rw-r--r--   0        0        0      701 2023-05-23 12:46:04.136114 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_head.py
--rw-r--r--   0        0        0      789 2023-05-23 12:46:04.165888 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_record.py
--rw-r--r--   0        0        0      847 2023-05-23 12:46:04.253097 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_repo.py
--rw-r--r--   0        0        0      871 2023-05-23 12:46:04.156294 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py
--rw-r--r--   0        0        0     1115 2023-05-23 12:46:04.162464 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/list_repos.py
--rw-r--r--   0        0        0      601 2023-05-23 12:46:04.237162 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py
--rw-r--r--   0        0        0      604 2023-05-23 12:46:04.090802 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py
--rw-r--r--   0        0        0     2604 2023-05-23 13:15:32.486216 atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py
--rw-r--r--   0        0        0      134 2023-05-23 13:15:32.486276 atproto-0.0.8/atproto/xrpc_client/models/common.py
--rw-r--r--   0        0        0      612 2023-05-23 12:20:32.363606 atproto-0.0.8/atproto/xrpc_client/models/type_conversion.py
--rw-r--r--   0        0        0     3409 2023-05-23 13:15:32.486395 atproto-0.0.8/atproto/xrpc_client/models/utils.py
--rw-r--r--   0        0        0     6148 2023-05-08 17:39:09.891512 atproto-0.0.8/atproto/xrpc_client/namespaces/.DS_Store
--rw-r--r--   0        0        0        0 2023-04-30 08:01:01.985340 atproto-0.0.8/atproto/xrpc_client/namespaces/__init__.py
--rw-r--r--   0        0        0      171 2023-05-08 17:46:35.193604 atproto-0.0.8/atproto/xrpc_client/namespaces/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    69598 2023-05-23 12:47:54.250370 atproto-0.0.8/atproto/xrpc_client/namespaces/__pycache__/async_ns.cpython-38.pyc
--rw-r--r--   0        0        0      801 2023-05-20 19:17:15.556274 atproto-0.0.8/atproto/xrpc_client/namespaces/__pycache__/base.cpython-38.pyc
--rw-r--r--   0        0        0    68949 2023-05-23 12:47:54.264516 atproto-0.0.8/atproto/xrpc_client/namespaces/__pycache__/sync_ns.cpython-38.pyc
--rw-r--r--   0        0        0    78721 2023-05-23 12:20:40.627807 atproto-0.0.8/atproto/xrpc_client/namespaces/async_ns.py
--rw-r--r--   0        0        0      344 2023-05-20 18:39:04.327872 atproto-0.0.8/atproto/xrpc_client/namespaces/base.py
--rw-r--r--   0        0        0    77605 2023-05-23 12:20:40.580068 atproto-0.0.8/atproto/xrpc_client/namespaces/sync_ns.py
--rw-r--r--   0        0        0     4320 2023-05-23 13:15:32.486526 atproto-0.0.8/atproto/xrpc_client/request.py
--rw-r--r--   0        0        0       43 2023-05-05 12:44:22.361781 atproto-0.0.8/atproto/xrpc_server/__init__.py
--rw-r--r--   0        0        0      160 2023-05-05 12:44:59.992820 atproto-0.0.8/atproto/xrpc_server/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     2424 2023-05-23 13:37:26.068244 atproto-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    11529 1970-01-01 00:00:00.000000 atproto-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-24 22:15:59.736490 atproto-0.0.9/LICENSE
+-rw-r--r--   0        0        0     9531 2023-05-24 22:15:59.736490 atproto-0.0.9/README.md
+-rw-r--r--   0        0        0      403 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/__init__.py
+-rw-r--r--   0        0        0     1782 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/car/__init__.py
+-rw-r--r--   0        0        0     1624 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/cbor/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/cid/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/cli/__init__.py
+-rw-r--r--   0        0        0     2790 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/codegen/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/codegen/clients/__init__.py
+-rw-r--r--   0        0        0     1434 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/codegen/clients/generate_async_client.py
+-rw-r--r--   0        0        0        0 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/codegen/models/__init__.py
+-rw-r--r--   0        0        0     2399 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/codegen/models/builder.py
+-rw-r--r--   0        0        0    19213 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/codegen/models/generator.py
+-rw-r--r--   0        0        0        0 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/codegen/namespaces/__init__.py
+-rw-r--r--   0        0        0     2546 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/codegen/namespaces/builder.py
+-rw-r--r--   0        0        0    11836 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/codegen/namespaces/generator.py
+-rw-r--r--   0        0        0     1184 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/exceptions.py
+-rw-r--r--   0        0        0     4007 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/firehose/__init__.py
+-rw-r--r--   0        0        0     8005 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/firehose/client.py
+-rw-r--r--   0        0        0     4183 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/firehose/models.py
+-rw-r--r--   0        0        0     2569 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/leb128/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/lexicon/__init__.py
+-rw-r--r--   0        0        0     4790 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/lexicon/models.py
+-rw-r--r--   0        0        0     3857 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/lexicon/parser.py
+-rw-r--r--   0        0        0     5295 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/nsid/__init__.py
+-rw-r--r--   0        0        0     3064 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/uri/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/client/__init__.py
+-rw-r--r--   0        0        0     9512 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/client/async_client.py
+-rw-r--r--   0        0        0      489 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/client/async_raw.py
+-rw-r--r--   0        0        0      414 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/client/auth.py
+-rw-r--r--   0        0        0     3748 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/client/base.py
+-rw-r--r--   0        0        0     8997 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/client/client.py
+-rw-r--r--   0        0        0       76 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/client/methods_mixin/__init__.py
+-rw-r--r--   0        0        0     1311 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/client/methods_mixin/session.py
+-rw-r--r--   0        0        0      469 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/client/raw.py
+-rw-r--r--   0        0        0    12159 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/__init__.py
+-rw-r--r--   0        0        0     3804 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/defs.py
+-rw-r--r--   0        0        0      759 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py
+-rw-r--r--   0        0        0      800 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/get_profile.py
+-rw-r--r--   0        0        0      819 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py
+-rw-r--r--   0        0        0      916 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py
+-rw-r--r--   0        0        0      846 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/profile.py
+-rw-r--r--   0        0        0      631 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py
+-rw-r--r--   0        0        0      955 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/search_actors.py
+-rw-r--r--   0        0        0      884 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/embed/__init__.py
+-rw-r--r--   0        0        0     1561 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/embed/external.py
+-rw-r--r--   0        0        0     1397 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/embed/images.py
+-rw-r--r--   0        0        0     2260 2023-05-24 22:15:59.736490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/embed/record.py
+-rw-r--r--   0        0        0     1181 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/__init__.py
+-rw-r--r--   0        0        0     5618 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/defs.py
+-rw-r--r--   0        0        0     1290 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/describe_feed_generator.py
+-rw-r--r--   0        0        0      983 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/generator.py
+-rw-r--r--   0        0        0      937 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_actor_feeds.py
+-rw-r--r--   0        0        0      934 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py
+-rw-r--r--   0        0        0      920 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_feed.py
+-rw-r--r--   0        0        0      839 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_feed_generator.py
+-rw-r--r--   0        0        0      814 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_feed_generators.py
+-rw-r--r--   0        0        0      940 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_feed_skeleton.py
+-rw-r--r--   0        0        0     1305 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_likes.py
+-rw-r--r--   0        0        0      981 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py
+-rw-r--r--   0        0        0      789 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_posts.py
+-rw-r--r--   0        0        0     1047 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py
+-rw-r--r--   0        0        0      957 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py
+-rw-r--r--   0        0        0      684 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/like.py
+-rw-r--r--   0        0        0     2205 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/post.py
+-rw-r--r--   0        0        0      688 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/repost.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/__init__.py
+-rw-r--r--   0        0        0      615 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/block.py
+-rw-r--r--   0        0        0     2141 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/defs.py
+-rw-r--r--   0        0        0      617 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/follow.py
+-rw-r--r--   0        0        0      906 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py
+-rw-r--r--   0        0        0     1008 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/get_followers.py
+-rw-r--r--   0        0        0     1000 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/get_follows.py
+-rw-r--r--   0        0        0      980 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/get_list.py
+-rw-r--r--   0        0        0      907 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py
+-rw-r--r--   0        0        0      925 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/get_lists.py
+-rw-r--r--   0        0        0      902 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py
+-rw-r--r--   0        0        0     1002 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/list.py
+-rw-r--r--   0        0        0      645 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/listitem.py
+-rw-r--r--   0        0        0      541 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py
+-rw-r--r--   0        0        0      543 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py
+-rw-r--r--   0        0        0      543 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py
+-rw-r--r--   0        0        0      545 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/notification/__init__.py
+-rw-r--r--   0        0        0      756 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py
+-rw-r--r--   0        0        0     1689 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py
+-rw-r--r--   0        0        0      552 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/notification/update_seen.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/richtext/__init__.py
+-rw-r--r--   0        0        0     1575 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/richtext/facet.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/unspecced/__init__.py
+-rw-r--r--   0        0        0      971 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py
+-rw-r--r--   0        0        0      553 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/base.py
+-rw-r--r--   0        0        0      713 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/blob_ref.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/__init__.py
+-rw-r--r--   0        0        0     9308 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/defs.py
+-rw-r--r--   0        0        0      560 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py
+-rw-r--r--   0        0        0      658 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py
+-rw-r--r--   0        0        0      559 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py
+-rw-r--r--   0        0        0      966 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py
+-rw-r--r--   0        0        0      806 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py
+-rw-r--r--   0        0        0      987 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py
+-rw-r--r--   0        0        0      806 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py
+-rw-r--r--   0        0        0     1095 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py
+-rw-r--r--   0        0        0      839 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/get_record.py
+-rw-r--r--   0        0        0      790 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/get_repo.py
+-rw-r--r--   0        0        0      880 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py
+-rw-r--r--   0        0        0      851 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py
+-rw-r--r--   0        0        0     1011 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/search_repos.py
+-rw-r--r--   0        0        0     1228 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py
+-rw-r--r--   0        0        0      605 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py
+-rw-r--r--   0        0        0      578 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/identity/__init__.py
+-rw-r--r--   0        0        0      815 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py
+-rw-r--r--   0        0        0      552 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/identity/update_handle.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/label/__init__.py
+-rw-r--r--   0        0        0     1173 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/label/defs.py
+-rw-r--r--   0        0        0     1215 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/label/query_labels.py
+-rw-r--r--   0        0        0     1214 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/moderation/__init__.py
+-rw-r--r--   0        0        0     1351 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/moderation/create_report.py
+-rw-r--r--   0        0        0      845 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/moderation/defs.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/__init__.py
+-rw-r--r--   0        0        0     1881 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py
+-rw-r--r--   0        0        0     1093 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/create_record.py
+-rw-r--r--   0        0        0      874 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/delete_record.py
+-rw-r--r--   0        0        0      910 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py
+-rw-r--r--   0        0        0     1062 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/get_record.py
+-rw-r--r--   0        0        0     1606 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/list_records.py
+-rw-r--r--   0        0        0     1160 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/put_record.py
+-rw-r--r--   0        0        0      679 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py
+-rw-r--r--   0        0        0      604 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py
+-rw-r--r--   0        0        0      704 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/__init__.py
+-rw-r--r--   0        0        0     1033 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/create_account.py
+-rw-r--r--   0        0        0      956 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/create_app_password.py
+-rw-r--r--   0        0        0      789 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py
+-rw-r--r--   0        0        0     1198 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py
+-rw-r--r--   0        0        0      973 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/create_session.py
+-rw-r--r--   0        0        0     1130 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/defs.py
+-rw-r--r--   0        0        0      603 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/delete_account.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/delete_session.py
+-rw-r--r--   0        0        0     1122 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/describe_server.py
+-rw-r--r--   0        0        0      926 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py
+-rw-r--r--   0        0        0      643 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/get_session.py
+-rw-r--r--   0        0        0      937 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py
+-rw-r--r--   0        0        0      655 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/refresh_session.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/request_account_delete.py
+-rw-r--r--   0        0        0      556 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py
+-rw-r--r--   0        0        0      581 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/reset_password.py
+-rw-r--r--   0        0        0      551 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py
+-rw-r--r--   0        0        0      323 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/__init__.py
+-rw-r--r--   0        0        0      706 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/get_blob.py
+-rw-r--r--   0        0        0      693 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py
+-rw-r--r--   0        0        0      765 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py
+-rw-r--r--   0        0        0      885 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py
+-rw-r--r--   0        0        0      701 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/get_head.py
+-rw-r--r--   0        0        0      789 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/get_record.py
+-rw-r--r--   0        0        0      847 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/get_repo.py
+-rw-r--r--   0        0        0      871 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py
+-rw-r--r--   0        0        0     1115 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/list_repos.py
+-rw-r--r--   0        0        0      601 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py
+-rw-r--r--   0        0        0      604 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py
+-rw-r--r--   0        0        0     2604 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py
+-rw-r--r--   0        0        0      134 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/common.py
+-rw-r--r--   0        0        0      612 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/type_conversion.py
+-rw-r--r--   0        0        0     3409 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/models/utils.py
+-rw-r--r--   0        0        0        0 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/namespaces/__init__.py
+-rw-r--r--   0        0        0    78721 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/namespaces/async_ns.py
+-rw-r--r--   0        0        0      344 2023-05-24 22:15:59.740490 atproto-0.0.9/atproto/xrpc_client/namespaces/base.py
+-rw-r--r--   0        0        0    77605 2023-05-24 22:15:59.744490 atproto-0.0.9/atproto/xrpc_client/namespaces/sync_ns.py
+-rw-r--r--   0        0        0     4320 2023-05-24 22:15:59.744490 atproto-0.0.9/atproto/xrpc_client/request.py
+-rw-r--r--   0        0        0       43 2023-05-24 22:15:59.744490 atproto-0.0.9/atproto/xrpc_server/__init__.py
+-rw-r--r--   0        0        0     2424 2023-05-24 22:16:26.600275 atproto-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    11246 1970-01-01 00:00:00.000000 atproto-0.0.9/PKG-INFO
```

### Comparing `atproto-0.0.8/LICENSE` & `atproto-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/README.md` & `atproto-0.0.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -271,15 +271,14 @@
 
 ### Future changes
 
 Things that a want to do soon:
 - Use came_case names of attributes in all models. Will break backward compatibility
 - Resolve issues with typehints. There are a lot of reference models with the same set of fields. Now they are completely different types
 - Provide autogenerated Record Namespaces with more high-level work with basic operations upon records (CRUD + list records)
-- Add tool for CAR binary type
 
 ### Change log
 
 The full change log is available in [CHANGES.md](https://github.com/MarshalX/atproto/blob/main/CHANGES.md).
 
 ### Contributing
```

### Comparing `atproto-0.0.8/atproto/car/__init__.py` & `atproto-0.0.9/atproto/car/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/cbor/__init__.py` & `atproto-0.0.9/atproto/cbor/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/codegen/__init__.py` & `atproto-0.0.9/atproto/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/codegen/clients/generate_async_client.py` & `atproto-0.0.9/atproto/codegen/clients/generate_async_client.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/codegen/models/builder.py` & `atproto-0.0.9/atproto/codegen/models/builder.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/codegen/models/generator.py` & `atproto-0.0.9/atproto/codegen/models/generator.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/codegen/namespaces/builder.py` & `atproto-0.0.9/atproto/codegen/namespaces/builder.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/codegen/namespaces/generator.py` & `atproto-0.0.9/atproto/codegen/namespaces/generator.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/exceptions.py` & `atproto-0.0.9/atproto/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+import typing as t
+
+if t.TYPE_CHECKING:
+    from atproto.xrpc_client.request import Response
+
+
 class AtProtocolError(Exception):
     """Base exception"""
 
 
 class LexiconParsingError(AtProtocolError):
     ...
 
@@ -38,32 +44,36 @@
     ...
 
 
 class ModelFieldNotFoundError(ModelError):
     ...
 
 
-class NetworkError(AtProtocolError):
+class RequestErrorBase(AtProtocolError):
+    def __init__(self, response: t.Optional['Response'] = None):
+        self.response: 'Response' = response
+
+
+class NetworkError(RequestErrorBase):
     ...
 
 
 class InvokeTimeoutError(NetworkError):
     ...
 
 
-class UnauthorizedError(AtProtocolError):
-    def __init__(self, response):
-        self.response = response
+class UnauthorizedError(RequestErrorBase):
+    ...
 
 
-class RequestException(AtProtocolError):
+class RequestException(RequestErrorBase):
     ...
 
 
-class BadRequestError(RequestException):
+class BadRequestError(RequestErrorBase):
     ...
 
 
 class InvalidAtUriError(AtProtocolError):
     ...
```

### Comparing `atproto-0.0.8/atproto/firehose/__init__.py` & `atproto-0.0.9/atproto/firehose/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/firehose/client.py` & `atproto-0.0.9/atproto/firehose/client.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/firehose/models.py` & `atproto-0.0.9/atproto/firehose/models.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/leb128/__init__.py` & `atproto-0.0.9/atproto/leb128/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/lexicon/models.py` & `atproto-0.0.9/atproto/lexicon/models.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/lexicon/parser.py` & `atproto-0.0.9/atproto/lexicon/parser.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/nsid/__init__.py` & `atproto-0.0.9/atproto/nsid/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/uri/__init__.py` & `atproto-0.0.9/atproto/uri/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/client/async_client.py` & `atproto-0.0.9/atproto/xrpc_client/client/async_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -204,7 +204,69 @@
         return await self.com.atproto.repo.delete_record(
             models.ComAtprotoRepoDeleteRecord.Data(
                 collection='app.bsky.feed.like',
                 repo=repo,
                 rkey=record_key,
             )
         )
+
+    async def repost(
+        self,
+        subject: models.ComAtprotoRepoStrongRef.Main,
+        profile_identify: t.Optional[str] = None,
+    ) -> models.ComAtprotoRepoCreateRecord.Response:
+        """Repost post.
+
+        Note:
+            If `profile_identify` is not provided will be sent to the current profile.
+
+        Args:
+            subject: Reference to the post that should be reposted.
+            profile_identify: Handle or DID. Where to make repost.
+
+        Returns:
+            :obj:`models.ComAtprotoRepoCreateRecord.Response`: Reference to the reposted post record.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        repo = self.me.did
+        if profile_identify:
+            repo = profile_identify
+
+        return await self.com.atproto.repo.create_record(
+            models.ComAtprotoRepoCreateRecord.Data(
+                repo=repo,
+                collection='app.bsky.feed.repost',
+                record=models.AppBskyFeedRepost.Main(
+                    createdAt=datetime.now().isoformat(),
+                    subject=subject,
+                ),
+            )
+        )
+
+    async def delete_post(self, post_rkey: str, profile_identify: t.Optional[str] = None) -> bool:
+        """Delete post.
+
+        Args:
+            post_rkey: ID (slug) of the post.
+            profile_identify: Handler or DID. Who created the post.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        repo = self.me.did
+        if profile_identify:
+            repo = profile_identify
+
+        return await self.com.atproto.repo.delete_record(
+            models.ComAtprotoRepoDeleteRecord.Data(
+                collection='app.bsky.feed.post',
+                repo=repo,
+                rkey=post_rkey,
+            )
+        )
```

### Comparing `atproto-0.0.8/atproto/xrpc_client/client/base.py` & `atproto-0.0.9/atproto/xrpc_client/client/base.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/client/client.py` & `atproto-0.0.9/atproto/xrpc_client/client/client.py`

 * *Files 15% similar despite different names*

```diff
@@ -196,7 +196,69 @@
         return self.com.atproto.repo.delete_record(
             models.ComAtprotoRepoDeleteRecord.Data(
                 collection='app.bsky.feed.like',
                 repo=repo,
                 rkey=record_key,
             )
         )
+
+    def repost(
+        self,
+        subject: models.ComAtprotoRepoStrongRef.Main,
+        profile_identify: t.Optional[str] = None,
+    ) -> models.ComAtprotoRepoCreateRecord.Response:
+        """Repost post.
+
+        Note:
+            If `profile_identify` is not provided will be sent to the current profile.
+
+        Args:
+            subject: Reference to the post that should be reposted.
+            profile_identify: Handle or DID. Where to make repost.
+
+        Returns:
+            :obj:`models.ComAtprotoRepoCreateRecord.Response`: Reference to the reposted post record.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        repo = self.me.did
+        if profile_identify:
+            repo = profile_identify
+
+        return self.com.atproto.repo.create_record(
+            models.ComAtprotoRepoCreateRecord.Data(
+                repo=repo,
+                collection='app.bsky.feed.repost',
+                record=models.AppBskyFeedRepost.Main(
+                    createdAt=datetime.now().isoformat(),
+                    subject=subject,
+                ),
+            )
+        )
+
+    def delete_post(self, post_rkey: str, profile_identify: t.Optional[str] = None) -> bool:
+        """Delete post.
+
+        Args:
+            post_rkey: ID (slug) of the post.
+            profile_identify: Handler or DID. Who created the post.
+
+        Returns:
+            :obj:`bool`: Success status.
+
+        Raises:
+            :class:`atproto.exceptions.AtProtocolError`: Base exception.
+        """
+
+        repo = self.me.did
+        if profile_identify:
+            repo = profile_identify
+
+        return self.com.atproto.repo.delete_record(
+            models.ComAtprotoRepoDeleteRecord.Data(
+                collection='app.bsky.feed.post',
+                repo=repo,
+                rkey=post_rkey,
+            )
+        )
```

### Comparing `atproto-0.0.8/atproto/xrpc_client/client/methods_mixin/session.py` & `atproto-0.0.9/atproto/xrpc_client/client/methods_mixin/session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/__init__.py` & `atproto-0.0.9/atproto/xrpc_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/defs.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/get_preferences.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/get_profile.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/get_profile.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/get_profiles.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/get_suggestions.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/profile.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/profile.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/put_preferences.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/search_actors.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/search_actors.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/actor/search_actors_typeahead.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/external.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/embed/external.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/images.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/embed/images.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/record.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/embed/record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/embed/record_with_media.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/defs.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/describe_feed_generator.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/describe_feed_generator.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/generator.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/generator.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_actor_feeds.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_actor_feeds.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_author_feed.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_feed.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_feed.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_feed_generator.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_feed_generator.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_feed_generators.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_feed_generators.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_feed_skeleton.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_feed_skeleton.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_likes.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_likes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_post_thread.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_posts.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_posts.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_reposted_by.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/get_timeline.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/like.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/like.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/post.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/post.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/feed/repost.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/feed/repost.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/block.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/block.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/defs.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/follow.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/follow.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/get_blocks.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_followers.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/get_followers.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_follows.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/get_follows.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_list.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/get_list.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/get_list_mutes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_lists.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/get_lists.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/get_mutes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/list.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/list.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/listitem.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/listitem.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/mute_actor.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/mute_actor_list.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/unmute_actor.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/graph/unmute_actor_list.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/notification/get_unread_count.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/notification/list_notifications.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/notification/update_seen.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/notification/update_seen.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/richtext/facet.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/richtext/facet.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py` & `atproto-0.0.9/atproto/xrpc_client/models/app/bsky/unspecced/get_popular.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/base.py` & `atproto-0.0.9/atproto/xrpc_client/models/base.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/blob_ref.py` & `atproto-0.0.9/atproto/xrpc_client/models/blob_ref.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/defs.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/disable_account_invites.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/disable_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/enable_account_invites.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/get_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/get_moderation_action.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/get_moderation_actions.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/get_moderation_report.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/get_moderation_reports.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_record.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/get_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/get_repo.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/get_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/resolve_moderation_reports.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/reverse_moderation_action.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/search_repos.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/search_repos.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/take_moderation_action.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/update_account_email.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/admin/update_account_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/identity/resolve_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/identity/update_handle.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/identity/update_handle.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/defs.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/label/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/query_labels.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/label/query_labels.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/label/subscribe_labels.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/create_report.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/moderation/create_report.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/moderation/defs.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/moderation/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/apply_writes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/create_record.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/create_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/delete_record.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/delete_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/describe_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/get_record.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/get_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/list_records.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/list_records.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/put_record.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/put_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/rebase_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/strong_ref.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/repo/upload_blob.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_account.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/create_account.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_app_password.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/create_app_password.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/create_invite_code.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/create_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/create_session.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/create_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/defs.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/defs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/delete_account.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/delete_account.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/describe_server.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/describe_server.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/get_account_invite_codes.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/get_session.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/get_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/list_app_passwords.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/refresh_session.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/refresh_session.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/request_password_reset.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/reset_password.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/reset_password.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/server/revoke_app_password.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_blob.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/get_blob.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/get_blocks.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/get_checkout.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/get_commit_path.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_head.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/get_head.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_record.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/get_record.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/get_repo.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/get_repo.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/list_blobs.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/list_repos.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/list_repos.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/notify_of_update.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/request_crawl.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py` & `atproto-0.0.9/atproto/xrpc_client/models/com/atproto/sync/subscribe_repos.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/type_conversion.py` & `atproto-0.0.9/atproto/xrpc_client/models/type_conversion.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/models/utils.py` & `atproto-0.0.9/atproto/xrpc_client/models/utils.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/namespaces/async_ns.py` & `atproto-0.0.9/atproto/xrpc_client/namespaces/async_ns.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/namespaces/sync_ns.py` & `atproto-0.0.9/atproto/xrpc_client/namespaces/sync_ns.py`

 * *Files identical despite different names*

### Comparing `atproto-0.0.8/atproto/xrpc_client/request.py` & `atproto-0.0.9/atproto/xrpc_client/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     )
     if response.content and is_json(response.content):
         data = json.loads(response.content)
         error_response.content = get_or_create_model(data, XrpcError)
 
     if response.status_code in {401, 403}:
         raise exceptions.UnauthorizedError(error_response)
-    elif response.status_code == 404:
+    elif response.status_code == 400:
         raise exceptions.BadRequestError(error_response)
     elif response.status_code in {409, 413, 502}:
         raise exceptions.NetworkError(error_response)
     else:
         raise exceptions.RequestException(error_response)
```

### Comparing `atproto-0.0.8/pyproject.toml` & `atproto-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "atproto"
-version = "0.0.8" # placeholder. Dynamic version from Git Tag
+version = "0.0.9" # placeholder. Dynamic version from Git Tag
 description = "The AT Protocol SDK"
 authors = ["Ilya (Marshal) <ilya@marshal.dev>"]
 license = "MIT"
 repository = "https://github.com/MarshalX/atproto"
 readme = "README.md"
 keywords = ["library", "sdk", "codegen", "xrpc", "xrpc-client", "atprotocol", "atproto", "lexicon", "parser", "schema", "bluesky", "bluesky-api", "at", "uri", "atp", "nsid", "did", "cid"]
 classifiers = [
```

### Comparing `atproto-0.0.8/PKG-INFO` & `atproto-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atproto
-Version: 0.0.8
+Version: 0.0.9
 Summary: The AT Protocol SDK
 Home-page: https://github.com/MarshalX/atproto
 License: MIT
 Keywords: library,sdk,codegen,xrpc,xrpc-client,atprotocol,atproto,lexicon,parser,schema,bluesky,bluesky-api,at,uri,atp,nsid,did,cid
 Author: Ilya (Marshal)
 Author-email: ilya@marshal.dev
 Requires-Python: >=3.7,<3.12
@@ -17,19 +17,14 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Pre-processors
 Requires-Dist: dacite (>=1.8.0,<1.9.0)
 Requires-Dist: dag-cbor (>=0.3.2,<0.4.0)
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
 Requires-Dist: httpx-ws (>=0.3.1,<0.4.0)
@@ -315,15 +310,14 @@
 
 ### Future changes
 
 Things that a want to do soon:
 - Use came_case names of attributes in all models. Will break backward compatibility
 - Resolve issues with typehints. There are a lot of reference models with the same set of fields. Now they are completely different types
 - Provide autogenerated Record Namespaces with more high-level work with basic operations upon records (CRUD + list records)
-- Add tool for CAR binary type
 
 ### Change log
 
 The full change log is available in [CHANGES.md](https://github.com/MarshalX/atproto/blob/main/CHANGES.md).
 
 ### Contributing
```

