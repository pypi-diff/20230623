# Comparing `tmp/cloudvision-1.9.0.tar.gz` & `tmp/cloudvision-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudvision-1.9.0.tar", last modified: Tue Feb 28 14:46:11 2023, max compression
+gzip compressed data, was "cloudvision-1.9.1.tar", last modified: Tue Mar 28 16:30:04 2023, max compression
```

## Comparing `cloudvision-1.9.0.tar` & `cloudvision-1.9.1.tar`

### file list

```diff
@@ -1,205 +1,205 @@
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.405196 cloudvision-1.9.0/
--rw-r--r--   0 mcgrathc   (504) staff       (20)    10148 2021-12-20 12:32:40.000000 cloudvision-1.9.0/COPYING
--rw-r--r--   0 mcgrathc   (504) staff       (20)       13 2022-10-11 13:26:15.000000 cloudvision-1.9.0/MANIFEST.in
--rw-r--r--   0 mcgrathc   (504) staff       (20)     4201 2023-02-28 14:46:11.404057 cloudvision-1.9.0/PKG-INFO
--rw-r--r--   0 mcgrathc   (504) staff       (20)     3767 2023-01-31 12:06:02.000000 cloudvision-1.9.0/README.md
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.044883 cloudvision-1.9.0/arista/
--rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.046941 cloudvision-1.9.0/arista/changecontrol/
--rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2022-05-16 10:11:38.000000 cloudvision-1.9.0/arista/changecontrol/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.052116 cloudvision-1.9.0/arista/changecontrol/v1/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      170 2022-05-16 10:11:38.000000 cloudvision-1.9.0/arista/changecontrol/v1/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    52629 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/changecontrol/v1/changecontrol_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/changecontrol/v1/changecontrol_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.054363 cloudvision-1.9.0/arista/changecontrol/v1/services/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      249 2022-05-16 10:11:38.000000 cloudvision-1.9.0/arista/changecontrol/v1/services/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    54853 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/changecontrol/v1/services/gen_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    27065 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/changecontrol/v1/services/gen_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.055226 cloudvision-1.9.0/arista/configstatus/
--rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/configstatus/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.059931 cloudvision-1.9.0/arista/configstatus/v1/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      167 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/configstatus/v1/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    47130 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/configstatus/v1/configstatus_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/configstatus/v1/configstatus_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.062125 cloudvision-1.9.0/arista/configstatus/v1/services/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      247 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/configstatus/v1/services/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    35483 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/configstatus/v1/services/gen_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    19075 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/configstatus/v1/services/gen_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.063798 cloudvision-1.9.0/arista/dashboard/
--rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/dashboard/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.068931 cloudvision-1.9.0/arista/dashboard/v1/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      158 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/dashboard/v1/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    33074 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/dashboard/v1/dashboard_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-05-16 10:11:38.000000 cloudvision-1.9.0/arista/dashboard/v1/dashboard_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.071746 cloudvision-1.9.0/arista/dashboard/v1/services/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      241 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/dashboard/v1/services/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    54494 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/dashboard/v1/services/gen_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    24787 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/dashboard/v1/services/gen_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.072707 cloudvision-1.9.0/arista/endpointlocation/
--rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/endpointlocation/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.075500 cloudvision-1.9.0/arista/endpointlocation/v1/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      179 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/endpointlocation/v1/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    55087 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/endpointlocation/v1/endpointlocation_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/endpointlocation/v1/endpointlocation_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.080943 cloudvision-1.9.0/arista/endpointlocation/v1/services/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      255 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/endpointlocation/v1/services/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    13805 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/endpointlocation/v1/services/gen_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     6821 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/endpointlocation/v1/services/gen_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.081642 cloudvision-1.9.0/arista/event/
--rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2021-12-20 12:32:40.000000 cloudvision-1.9.0/arista/event/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.087209 cloudvision-1.9.0/arista/event/v1/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      146 2021-12-20 12:32:40.000000 cloudvision-1.9.0/arista/event/v1/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    34720 2021-12-20 12:32:40.000000 cloudvision-1.9.0/arista/event/v1/event_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)       83 2021-12-20 12:32:40.000000 cloudvision-1.9.0/arista/event/v1/event_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.090053 cloudvision-1.9.0/arista/event/v1/services/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      233 2021-12-20 12:32:40.000000 cloudvision-1.9.0/arista/event/v1/services/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    30824 2021-12-20 12:32:40.000000 cloudvision-1.9.0/arista/event/v1/services/gen_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     9593 2021-12-20 12:32:40.000000 cloudvision-1.9.0/arista/event/v1/services/gen_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.090780 cloudvision-1.9.0/arista/identityprovider/
--rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/identityprovider/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.095034 cloudvision-1.9.0/arista/identityprovider/v1/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      179 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/identityprovider/v1/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    18358 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/identityprovider/v1/identityprovider_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/identityprovider/v1/identityprovider_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.097999 cloudvision-1.9.0/arista/identityprovider/v1/services/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      255 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/identityprovider/v1/services/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    52343 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/identityprovider/v1/services/gen_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    24264 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/identityprovider/v1/services/gen_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.101276 cloudvision-1.9.0/arista/inventory/
--rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2022-05-16 10:11:38.000000 cloudvision-1.9.0/arista/inventory/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.110345 cloudvision-1.9.0/arista/inventory/v1/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      158 2022-05-16 10:11:38.000000 cloudvision-1.9.0/arista/inventory/v1/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    43583 2022-05-16 10:11:38.000000 cloudvision-1.9.0/arista/inventory/v1/inventory_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-05-16 10:11:38.000000 cloudvision-1.9.0/arista/inventory/v1/inventory_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.115733 cloudvision-1.9.0/arista/inventory/v1/services/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      241 2022-05-16 10:11:38.000000 cloudvision-1.9.0/arista/inventory/v1/services/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    91303 2022-05-16 10:11:38.000000 cloudvision-1.9.0/arista/inventory/v1/services/gen_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    46466 2022-05-16 10:11:38.000000 cloudvision-1.9.0/arista/inventory/v1/services/gen_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.117104 cloudvision-1.9.0/arista/redirector/
--rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/redirector/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.119935 cloudvision-1.9.0/arista/redirector/v1/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      161 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/redirector/v1/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     8237 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/redirector/v1/redirector_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/redirector/v1/redirector_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.125112 cloudvision-1.9.0/arista/redirector/v1/services/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      243 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/redirector/v1/services/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    12848 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/redirector/v1/services/gen_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     6485 2023-01-31 12:06:02.000000 cloudvision-1.9.0/arista/redirector/v1/services/gen_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.126004 cloudvision-1.9.0/arista/studio/
--rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/studio/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.130167 cloudvision-1.9.0/arista/studio/v1/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      149 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/studio/v1/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.134305 cloudvision-1.9.0/arista/studio/v1/services/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      235 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/studio/v1/services/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    93347 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/studio/v1/services/gen_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    47926 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/studio/v1/services/gen_pb2_grpc.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    78061 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/studio/v1/studio_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/studio/v1/studio_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.139793 cloudvision-1.9.0/arista/subscriptions/
--rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2021-12-20 12:32:40.000000 cloudvision-1.9.0/arista/subscriptions/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     2394 2021-12-20 12:32:40.000000 cloudvision-1.9.0/arista/subscriptions/subscriptions_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)       83 2021-12-20 12:32:40.000000 cloudvision-1.9.0/arista/subscriptions/subscriptions_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.143096 cloudvision-1.9.0/arista/tag/
--rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2023-02-28 13:50:55.000000 cloudvision-1.9.0/arista/tag/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.149956 cloudvision-1.9.0/arista/tag/v1/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      140 2023-02-28 13:50:55.000000 cloudvision-1.9.0/arista/tag/v1/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.155779 cloudvision-1.9.0/arista/tag/v1/services/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      229 2023-02-28 13:50:55.000000 cloudvision-1.9.0/arista/tag/v1/services/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)   127877 2023-02-28 13:50:55.000000 cloudvision-1.9.0/arista/tag/v1/services/gen_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    60122 2023-02-28 13:50:55.000000 cloudvision-1.9.0/arista/tag/v1/services/gen_pb2_grpc.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    21109 2023-02-28 13:50:55.000000 cloudvision-1.9.0/arista/tag/v1/tag_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2023-02-28 13:50:55.000000 cloudvision-1.9.0/arista/tag/v1/tag_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.161226 cloudvision-1.9.0/arista/tag/v2/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      140 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/tag/v2/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.164707 cloudvision-1.9.0/arista/tag/v2/services/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      229 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/tag/v2/services/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    62015 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/tag/v2/services/gen_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    31635 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/tag/v2/services/gen_pb2_grpc.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    18912 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/tag/v2/tag_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/tag/v2/tag_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.169287 cloudvision-1.9.0/arista/time/
--rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2021-12-20 12:32:40.000000 cloudvision-1.9.0/arista/time/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     2914 2021-12-20 12:32:40.000000 cloudvision-1.9.0/arista/time/time_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)       83 2021-12-20 12:32:40.000000 cloudvision-1.9.0/arista/time/time_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.170652 cloudvision-1.9.0/arista/workspace/
--rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/workspace/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.176137 cloudvision-1.9.0/arista/workspace/v1/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      158 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/workspace/v1/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.179008 cloudvision-1.9.0/arista/workspace/v1/services/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      241 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/workspace/v1/services/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    44348 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/workspace/v1/services/gen_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    22735 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/workspace/v1/services/gen_pb2_grpc.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    65475 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/workspace/v1/workspace_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.0/arista/workspace/v1/workspace_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.180709 cloudvision-1.9.0/cloudvision/
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.197337 cloudvision-1.9.0/cloudvision/Connector/
--rw-r--r--   0 mcgrathc   (504) staff       (20)     2461 2021-12-20 12:32:40.000000 cloudvision-1.9.0/cloudvision/Connector/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.200611 cloudvision-1.9.0/cloudvision/Connector/auth/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      148 2023-02-28 13:50:55.000000 cloudvision-1.9.0/cloudvision/Connector/auth/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     2855 2023-02-28 13:50:55.000000 cloudvision-1.9.0/cloudvision/Connector/auth/cert.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.207924 cloudvision-1.9.0/cloudvision/Connector/codec/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      491 2021-12-20 12:32:40.000000 cloudvision-1.9.0/cloudvision/Connector/codec/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     2301 2021-12-20 12:32:40.000000 cloudvision-1.9.0/cloudvision/Connector/codec/custom_types.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     1581 2022-10-11 13:26:15.000000 cloudvision-1.9.0/cloudvision/Connector/codec/decoder.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     1813 2022-10-11 13:26:15.000000 cloudvision-1.9.0/cloudvision/Connector/codec/encoder.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.210699 cloudvision-1.9.0/cloudvision/Connector/core/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      148 2023-02-28 13:50:55.000000 cloudvision-1.9.0/cloudvision/Connector/core/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      538 2023-02-28 13:50:55.000000 cloudvision-1.9.0/cloudvision/Connector/core/utils.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.242173 cloudvision-1.9.0/cloudvision/Connector/gen/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      344 2021-12-20 12:32:40.000000 cloudvision-1.9.0/cloudvision/Connector/gen/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     1835 2023-02-28 13:50:55.000000 cloudvision-1.9.0/cloudvision/Connector/gen/ca_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     4031 2023-02-28 13:50:55.000000 cloudvision-1.9.0/cloudvision/Connector/gen/ca_pb2_grpc.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     4701 2022-10-11 13:26:15.000000 cloudvision-1.9.0/cloudvision/Connector/gen/notification_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.0/cloudvision/Connector/gen/notification_pb2_grpc.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    32077 2022-10-11 13:26:15.000000 cloudvision-1.9.0/cloudvision/Connector/gen/router_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    46614 2022-05-16 10:11:38.000000 cloudvision-1.9.0/cloudvision/Connector/gen/router_pb2_grpc.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     1776 2022-10-11 13:26:15.000000 cloudvision-1.9.0/cloudvision/Connector/gen/sharding_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.0/cloudvision/Connector/gen/sharding_pb2_grpc.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.260785 cloudvision-1.9.0/cloudvision/Connector/grpc_client/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      283 2021-12-20 12:32:40.000000 cloudvision-1.9.0/cloudvision/Connector/grpc_client/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    14291 2023-02-28 13:50:55.000000 cloudvision-1.9.0/cloudvision/Connector/grpc_client/grpcClient.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      273 2023-02-28 14:42:17.000000 cloudvision-1.9.0/cloudvision/__init__.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.380202 cloudvision-1.9.0/cloudvision/cvlib/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      660 2023-01-31 11:46:14.000000 cloudvision-1.9.0/cloudvision/cvlib/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     2179 2023-01-27 11:06:26.000000 cloudvision-1.9.0/cloudvision/cvlib/action.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     1532 2022-10-11 13:26:15.000000 cloudvision-1.9.0/cloudvision/cvlib/changecontrol.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     5777 2022-10-11 13:26:15.000000 cloudvision-1.9.0/cloudvision/cvlib/connections.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    21766 2023-02-09 10:06:41.000000 cloudvision-1.9.0/cloudvision/cvlib/context.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     2506 2023-01-27 11:06:26.000000 cloudvision-1.9.0/cloudvision/cvlib/device.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    10594 2022-10-17 14:38:15.000000 cloudvision-1.9.0/cloudvision/cvlib/exceptions.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      373 2022-10-11 13:26:15.000000 cloudvision-1.9.0/cloudvision/cvlib/execution.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     1729 2022-10-11 13:26:15.000000 cloudvision-1.9.0/cloudvision/cvlib/logger.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     6705 2022-10-24 10:29:14.000000 cloudvision-1.9.0/cloudvision/cvlib/studio.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     1906 2022-10-11 13:26:15.000000 cloudvision-1.9.0/cloudvision/cvlib/topology.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      457 2022-10-11 13:26:15.000000 cloudvision-1.9.0/cloudvision/cvlib/user.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     2218 2022-10-11 13:26:15.000000 cloudvision-1.9.0/cloudvision/cvlib/utils.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.196735 cloudvision-1.9.0/cloudvision.egg-info/
--rw-r--r--   0 mcgrathc   (504) staff       (20)     4201 2023-02-28 14:46:10.000000 cloudvision-1.9.0/cloudvision.egg-info/PKG-INFO
--rw-r--r--   0 mcgrathc   (504) staff       (20)     5248 2023-02-28 14:46:10.000000 cloudvision-1.9.0/cloudvision.egg-info/SOURCES.txt
--rw-r--r--   0 mcgrathc   (504) staff       (20)        1 2023-02-28 14:46:10.000000 cloudvision-1.9.0/cloudvision.egg-info/dependency_links.txt
--rw-r--r--   0 mcgrathc   (504) staff       (20)      187 2023-02-28 14:46:10.000000 cloudvision-1.9.0/cloudvision.egg-info/requires.txt
--rw-r--r--   0 mcgrathc   (504) staff       (20)       31 2023-02-28 14:46:10.000000 cloudvision-1.9.0/cloudvision.egg-info/top_level.txt
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.395504 cloudvision-1.9.0/fmp/
--rw-r--r--   0 mcgrathc   (504) staff       (20)      232 2023-02-28 13:50:55.000000 cloudvision-1.9.0/fmp/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     2530 2023-01-31 12:06:02.000000 cloudvision-1.9.0/fmp/deletes_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2023-01-31 12:06:02.000000 cloudvision-1.9.0/fmp/deletes_pb2_grpc.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     6406 2022-02-25 09:46:36.000000 cloudvision-1.9.0/fmp/extensions_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.0/fmp/extensions_pb2_grpc.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)    13402 2023-01-31 12:06:02.000000 cloudvision-1.9.0/fmp/inet_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.0/fmp/inet_pb2_grpc.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)   185794 2022-02-25 09:46:36.000000 cloudvision-1.9.0/fmp/wrappers_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.0/fmp/wrappers_pb2_grpc.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     3458 2023-01-31 12:06:02.000000 cloudvision-1.9.0/fmp/yang_pb2.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.0/fmp/yang_pb2_grpc.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)       31 2023-01-27 11:06:26.000000 cloudvision-1.9.0/pyproject.toml
--rw-r--r--   0 mcgrathc   (504) staff       (20)      186 2023-01-27 11:06:26.000000 cloudvision-1.9.0/requirements-dev.txt
--rw-r--r--   0 mcgrathc   (504) staff       (20)      187 2023-02-28 13:50:55.000000 cloudvision-1.9.0/requirements.txt
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.397902 cloudvision-1.9.0/sandbox/
--rw-r--r--   0 mcgrathc   (504) staff       (20)        0 2022-07-25 16:20:44.000000 cloudvision-1.9.0/sandbox/__init__.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)      979 2023-02-09 09:54:04.000000 cloudvision-1.9.0/sandbox/test.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)       38 2023-02-28 14:46:11.405526 cloudvision-1.9.0/setup.cfg
--rw-r--r--   0 mcgrathc   (504) staff       (20)     1048 2022-10-27 11:08:57.000000 cloudvision-1.9.0/setup.py
-drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-02-28 14:46:11.401703 cloudvision-1.9.0/test/
--rw-r--r--   0 mcgrathc   (504) staff       (20)     3795 2022-10-11 13:26:15.000000 cloudvision-1.9.0/test/test_codec.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     1877 2023-01-31 11:46:14.000000 cloudvision-1.9.0/test/test_cvlib_context.py
--rw-r--r--   0 mcgrathc   (504) staff       (20)     8088 2022-10-27 11:08:57.000000 cloudvision-1.9.0/test/test_cvlib_studio.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.293020 cloudvision-1.9.1/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    10148 2021-12-20 12:32:40.000000 cloudvision-1.9.1/COPYING
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       13 2023-03-28 08:22:35.000000 cloudvision-1.9.1/MANIFEST.in
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     4201 2023-03-28 16:30:04.292619 cloudvision-1.9.1/PKG-INFO
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     3767 2023-03-28 13:26:43.000000 cloudvision-1.9.1/README.md
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.941422 cloudvision-1.9.1/arista/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.944236 cloudvision-1.9.1/arista/changecontrol/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2022-05-16 10:11:38.000000 cloudvision-1.9.1/arista/changecontrol/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.951468 cloudvision-1.9.1/arista/changecontrol/v1/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      170 2022-05-16 10:11:38.000000 cloudvision-1.9.1/arista/changecontrol/v1/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    52629 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/changecontrol/v1/changecontrol_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/changecontrol/v1/changecontrol_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.955711 cloudvision-1.9.1/arista/changecontrol/v1/services/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      249 2022-05-16 10:11:38.000000 cloudvision-1.9.1/arista/changecontrol/v1/services/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    54853 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/changecontrol/v1/services/gen_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    27065 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/changecontrol/v1/services/gen_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.957071 cloudvision-1.9.1/arista/configstatus/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/configstatus/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.959761 cloudvision-1.9.1/arista/configstatus/v1/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      167 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/configstatus/v1/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    47130 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/configstatus/v1/configstatus_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/configstatus/v1/configstatus_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.963081 cloudvision-1.9.1/arista/configstatus/v1/services/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      247 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/configstatus/v1/services/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    35483 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/configstatus/v1/services/gen_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    19075 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/configstatus/v1/services/gen_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.964004 cloudvision-1.9.1/arista/dashboard/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/dashboard/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.968483 cloudvision-1.9.1/arista/dashboard/v1/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      158 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/dashboard/v1/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    33074 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/dashboard/v1/dashboard_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-05-16 10:11:38.000000 cloudvision-1.9.1/arista/dashboard/v1/dashboard_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.971064 cloudvision-1.9.1/arista/dashboard/v1/services/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      241 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/dashboard/v1/services/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    54494 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/dashboard/v1/services/gen_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    24787 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/dashboard/v1/services/gen_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.971955 cloudvision-1.9.1/arista/endpointlocation/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/endpointlocation/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.978891 cloudvision-1.9.1/arista/endpointlocation/v1/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      179 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/endpointlocation/v1/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    55087 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/endpointlocation/v1/endpointlocation_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/endpointlocation/v1/endpointlocation_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.982320 cloudvision-1.9.1/arista/endpointlocation/v1/services/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      255 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/endpointlocation/v1/services/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    13805 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/endpointlocation/v1/services/gen_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     6821 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/endpointlocation/v1/services/gen_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.983217 cloudvision-1.9.1/arista/event/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2021-12-20 12:32:40.000000 cloudvision-1.9.1/arista/event/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.985751 cloudvision-1.9.1/arista/event/v1/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      146 2021-12-20 12:32:40.000000 cloudvision-1.9.1/arista/event/v1/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    34720 2021-12-20 12:32:40.000000 cloudvision-1.9.1/arista/event/v1/event_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       83 2021-12-20 12:32:40.000000 cloudvision-1.9.1/arista/event/v1/event_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.995434 cloudvision-1.9.1/arista/event/v1/services/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      233 2021-12-20 12:32:40.000000 cloudvision-1.9.1/arista/event/v1/services/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    30824 2021-12-20 12:32:40.000000 cloudvision-1.9.1/arista/event/v1/services/gen_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     9593 2021-12-20 12:32:40.000000 cloudvision-1.9.1/arista/event/v1/services/gen_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:03.997725 cloudvision-1.9.1/arista/identityprovider/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/identityprovider/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.002689 cloudvision-1.9.1/arista/identityprovider/v1/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      179 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/identityprovider/v1/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    18358 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/identityprovider/v1/identityprovider_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/identityprovider/v1/identityprovider_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.006399 cloudvision-1.9.1/arista/identityprovider/v1/services/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      255 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/identityprovider/v1/services/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    52343 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/identityprovider/v1/services/gen_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    24264 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/identityprovider/v1/services/gen_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.007716 cloudvision-1.9.1/arista/inventory/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/inventory/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.018731 cloudvision-1.9.1/arista/inventory/v1/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      158 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/inventory/v1/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    44204 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/inventory/v1/inventory_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-05-16 10:11:38.000000 cloudvision-1.9.1/arista/inventory/v1/inventory_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.030724 cloudvision-1.9.1/arista/inventory/v1/services/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      241 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/inventory/v1/services/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)   102439 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/inventory/v1/services/gen_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    50400 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/inventory/v1/services/gen_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.034060 cloudvision-1.9.1/arista/redirector/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/redirector/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.038106 cloudvision-1.9.1/arista/redirector/v1/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      161 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/redirector/v1/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     8237 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/redirector/v1/redirector_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/redirector/v1/redirector_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.044967 cloudvision-1.9.1/arista/redirector/v1/services/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      243 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/redirector/v1/services/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    12848 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/redirector/v1/services/gen_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     6485 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/redirector/v1/services/gen_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.046350 cloudvision-1.9.1/arista/studio/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/studio/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.049195 cloudvision-1.9.1/arista/studio/v1/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      149 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/studio/v1/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.053195 cloudvision-1.9.1/arista/studio/v1/services/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      235 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/studio/v1/services/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    93347 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/studio/v1/services/gen_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    47926 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/studio/v1/services/gen_pb2_grpc.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    78061 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/studio/v1/studio_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/studio/v1/studio_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.057463 cloudvision-1.9.1/arista/subscriptions/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2021-12-20 12:32:40.000000 cloudvision-1.9.1/arista/subscriptions/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     2394 2021-12-20 12:32:40.000000 cloudvision-1.9.1/arista/subscriptions/subscriptions_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       83 2021-12-20 12:32:40.000000 cloudvision-1.9.1/arista/subscriptions/subscriptions_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.058129 cloudvision-1.9.1/arista/tag/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/tag/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.062353 cloudvision-1.9.1/arista/tag/v1/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      140 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/tag/v1/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.069036 cloudvision-1.9.1/arista/tag/v1/services/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      229 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/tag/v1/services/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)   127877 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/tag/v1/services/gen_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    60122 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/tag/v1/services/gen_pb2_grpc.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    21109 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/tag/v1/tag_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2023-03-28 13:26:43.000000 cloudvision-1.9.1/arista/tag/v1/tag_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.077298 cloudvision-1.9.1/arista/tag/v2/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      140 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/tag/v2/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.154590 cloudvision-1.9.1/arista/tag/v2/services/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      229 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/tag/v2/services/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    62015 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/tag/v2/services/gen_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    31635 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/tag/v2/services/gen_pb2_grpc.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    18912 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/tag/v2/tag_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/tag/v2/tag_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.161326 cloudvision-1.9.1/arista/time/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2021-12-20 12:32:40.000000 cloudvision-1.9.1/arista/time/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     2914 2021-12-20 12:32:40.000000 cloudvision-1.9.1/arista/time/time_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       83 2021-12-20 12:32:40.000000 cloudvision-1.9.1/arista/time/time_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.162562 cloudvision-1.9.1/arista/workspace/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       65 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/workspace/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.178740 cloudvision-1.9.1/arista/workspace/v1/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      158 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/workspace/v1/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.183982 cloudvision-1.9.1/arista/workspace/v1/services/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      241 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/workspace/v1/services/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    44348 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/workspace/v1/services/gen_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    22735 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/workspace/v1/services/gen_pb2_grpc.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    65475 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/workspace/v1/workspace_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.1/arista/workspace/v1/workspace_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.185744 cloudvision-1.9.1/cloudvision/
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.193926 cloudvision-1.9.1/cloudvision/Connector/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     2461 2021-12-20 12:32:40.000000 cloudvision-1.9.1/cloudvision/Connector/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.197247 cloudvision-1.9.1/cloudvision/Connector/auth/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      148 2023-03-28 13:26:43.000000 cloudvision-1.9.1/cloudvision/Connector/auth/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     2855 2023-03-28 13:26:43.000000 cloudvision-1.9.1/cloudvision/Connector/auth/cert.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.205318 cloudvision-1.9.1/cloudvision/Connector/codec/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      491 2021-12-20 12:32:40.000000 cloudvision-1.9.1/cloudvision/Connector/codec/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     2301 2021-12-20 12:32:40.000000 cloudvision-1.9.1/cloudvision/Connector/codec/custom_types.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     1581 2023-03-28 08:22:35.000000 cloudvision-1.9.1/cloudvision/Connector/codec/decoder.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     1813 2023-03-28 08:22:35.000000 cloudvision-1.9.1/cloudvision/Connector/codec/encoder.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.208209 cloudvision-1.9.1/cloudvision/Connector/core/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      148 2023-03-28 13:26:43.000000 cloudvision-1.9.1/cloudvision/Connector/core/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      538 2023-03-28 13:26:43.000000 cloudvision-1.9.1/cloudvision/Connector/core/utils.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.231859 cloudvision-1.9.1/cloudvision/Connector/gen/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      344 2021-12-20 12:32:40.000000 cloudvision-1.9.1/cloudvision/Connector/gen/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     1835 2023-03-28 13:26:43.000000 cloudvision-1.9.1/cloudvision/Connector/gen/ca_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     4031 2023-03-28 13:26:43.000000 cloudvision-1.9.1/cloudvision/Connector/gen/ca_pb2_grpc.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     4701 2023-03-28 08:22:35.000000 cloudvision-1.9.1/cloudvision/Connector/gen/notification_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.1/cloudvision/Connector/gen/notification_pb2_grpc.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    32077 2023-03-28 08:22:35.000000 cloudvision-1.9.1/cloudvision/Connector/gen/router_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    46614 2022-05-16 10:11:38.000000 cloudvision-1.9.1/cloudvision/Connector/gen/router_pb2_grpc.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     1776 2023-03-28 08:22:35.000000 cloudvision-1.9.1/cloudvision/Connector/gen/sharding_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.1/cloudvision/Connector/gen/sharding_pb2_grpc.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.236685 cloudvision-1.9.1/cloudvision/Connector/grpc_client/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      283 2021-12-20 12:32:40.000000 cloudvision-1.9.1/cloudvision/Connector/grpc_client/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    14355 2023-03-28 13:26:43.000000 cloudvision-1.9.1/cloudvision/Connector/grpc_client/grpcClient.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      273 2023-03-28 16:29:49.000000 cloudvision-1.9.1/cloudvision/__init__.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.265576 cloudvision-1.9.1/cloudvision/cvlib/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      660 2023-03-28 16:29:49.000000 cloudvision-1.9.1/cloudvision/cvlib/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     2179 2023-03-28 13:26:43.000000 cloudvision-1.9.1/cloudvision/cvlib/action.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     1532 2023-03-28 08:22:35.000000 cloudvision-1.9.1/cloudvision/cvlib/changecontrol.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     5800 2023-03-28 13:26:43.000000 cloudvision-1.9.1/cloudvision/cvlib/connections.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    21776 2023-03-28 13:26:43.000000 cloudvision-1.9.1/cloudvision/cvlib/context.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     2514 2023-03-28 16:29:49.000000 cloudvision-1.9.1/cloudvision/cvlib/device.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    10594 2023-03-28 08:22:35.000000 cloudvision-1.9.1/cloudvision/cvlib/exceptions.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      373 2023-03-28 08:22:35.000000 cloudvision-1.9.1/cloudvision/cvlib/execution.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     1729 2023-03-28 08:22:35.000000 cloudvision-1.9.1/cloudvision/cvlib/logger.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     6727 2023-03-28 16:29:49.000000 cloudvision-1.9.1/cloudvision/cvlib/studio.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     1925 2023-03-28 13:26:43.000000 cloudvision-1.9.1/cloudvision/cvlib/topology.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      457 2023-03-28 08:22:35.000000 cloudvision-1.9.1/cloudvision/cvlib/user.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     2218 2023-03-28 08:22:35.000000 cloudvision-1.9.1/cloudvision/cvlib/utils.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.192139 cloudvision-1.9.1/cloudvision.egg-info/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     4201 2023-03-28 16:30:03.000000 cloudvision-1.9.1/cloudvision.egg-info/PKG-INFO
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     5248 2023-03-28 16:30:03.000000 cloudvision-1.9.1/cloudvision.egg-info/SOURCES.txt
+-rw-r--r--   0 mcgrathc   (504) staff       (20)        1 2023-03-28 16:30:03.000000 cloudvision-1.9.1/cloudvision.egg-info/dependency_links.txt
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      195 2023-03-28 16:30:03.000000 cloudvision-1.9.1/cloudvision.egg-info/requires.txt
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       31 2023-03-28 16:30:03.000000 cloudvision-1.9.1/cloudvision.egg-info/top_level.txt
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.284242 cloudvision-1.9.1/fmp/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      232 2023-03-28 13:26:43.000000 cloudvision-1.9.1/fmp/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     2530 2023-03-28 13:26:43.000000 cloudvision-1.9.1/fmp/deletes_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2023-03-28 13:26:43.000000 cloudvision-1.9.1/fmp/deletes_pb2_grpc.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     6406 2022-02-25 09:46:36.000000 cloudvision-1.9.1/fmp/extensions_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.1/fmp/extensions_pb2_grpc.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)    13402 2023-03-28 13:26:43.000000 cloudvision-1.9.1/fmp/inet_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.1/fmp/inet_pb2_grpc.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)   185794 2022-02-25 09:46:36.000000 cloudvision-1.9.1/fmp/wrappers_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.1/fmp/wrappers_pb2_grpc.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     3458 2023-03-28 13:26:43.000000 cloudvision-1.9.1/fmp/yang_pb2.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      159 2022-02-25 09:46:36.000000 cloudvision-1.9.1/fmp/yang_pb2_grpc.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       31 2023-03-28 13:26:43.000000 cloudvision-1.9.1/pyproject.toml
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      186 2023-03-28 13:26:43.000000 cloudvision-1.9.1/requirements-dev.txt
+-rw-r--r--   0 mcgrathc   (504) staff       (20)      195 2023-03-28 13:26:43.000000 cloudvision-1.9.1/requirements.txt
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.286817 cloudvision-1.9.1/sandbox/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)        0 2022-07-25 16:20:44.000000 cloudvision-1.9.1/sandbox/__init__.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     4302 2023-03-28 13:38:15.000000 cloudvision-1.9.1/sandbox/test.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)       38 2023-03-28 16:30:04.294294 cloudvision-1.9.1/setup.cfg
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     1048 2023-03-28 08:22:35.000000 cloudvision-1.9.1/setup.py
+drwxr-xr-x   0 mcgrathc   (504) staff       (20)        0 2023-03-28 16:30:04.291293 cloudvision-1.9.1/test/
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     3881 2023-03-28 13:26:43.000000 cloudvision-1.9.1/test/test_codec.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     3860 2023-03-28 13:26:43.000000 cloudvision-1.9.1/test/test_cvlib_context.py
+-rw-r--r--   0 mcgrathc   (504) staff       (20)     8088 2023-03-28 16:29:49.000000 cloudvision-1.9.1/test/test_cvlib_studio.py
```

### Comparing `cloudvision-1.9.0/COPYING` & `cloudvision-1.9.1/COPYING`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/PKG-INFO` & `cloudvision-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudvision
-Version: 1.9.0
+Version: 1.9.1
 Summary: A Python library for Arista's CloudVision APIs.
 Home-page: https://github.com/aristanetworks/cloudvision-python
 Maintainer-email: support@arista.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `cloudvision-1.9.0/README.md` & `cloudvision-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/changecontrol/v1/changecontrol_pb2.py` & `cloudvision-1.9.1/arista/changecontrol/v1/changecontrol_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/changecontrol/v1/services/gen_pb2.py` & `cloudvision-1.9.1/arista/changecontrol/v1/services/gen_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/changecontrol/v1/services/gen_pb2_grpc.py` & `cloudvision-1.9.1/arista/changecontrol/v1/services/gen_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/configstatus/v1/configstatus_pb2.py` & `cloudvision-1.9.1/arista/configstatus/v1/configstatus_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/configstatus/v1/services/gen_pb2.py` & `cloudvision-1.9.1/arista/configstatus/v1/services/gen_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/configstatus/v1/services/gen_pb2_grpc.py` & `cloudvision-1.9.1/arista/configstatus/v1/services/gen_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/dashboard/v1/dashboard_pb2.py` & `cloudvision-1.9.1/arista/dashboard/v1/dashboard_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/dashboard/v1/services/gen_pb2.py` & `cloudvision-1.9.1/arista/dashboard/v1/services/gen_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/dashboard/v1/services/gen_pb2_grpc.py` & `cloudvision-1.9.1/arista/dashboard/v1/services/gen_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/endpointlocation/v1/endpointlocation_pb2.py` & `cloudvision-1.9.1/arista/endpointlocation/v1/endpointlocation_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/endpointlocation/v1/services/gen_pb2.py` & `cloudvision-1.9.1/arista/endpointlocation/v1/services/gen_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/endpointlocation/v1/services/gen_pb2_grpc.py` & `cloudvision-1.9.1/arista/endpointlocation/v1/services/gen_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/event/v1/event_pb2.py` & `cloudvision-1.9.1/arista/event/v1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/event/v1/services/gen_pb2.py` & `cloudvision-1.9.1/arista/event/v1/services/gen_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/event/v1/services/gen_pb2_grpc.py` & `cloudvision-1.9.1/arista/event/v1/services/gen_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/identityprovider/v1/identityprovider_pb2.py` & `cloudvision-1.9.1/arista/identityprovider/v1/identityprovider_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/identityprovider/v1/services/gen_pb2.py` & `cloudvision-1.9.1/arista/identityprovider/v1/services/gen_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/identityprovider/v1/services/gen_pb2_grpc.py` & `cloudvision-1.9.1/arista/identityprovider/v1/services/gen_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/inventory/v1/inventory_pb2.py` & `cloudvision-1.9.1/arista/inventory/v1/inventory_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='arista/inventory.v1/inventory.proto',
   package='arista.inventory.v1',
   syntax='proto3',
   serialized_options=b'Z.arista/resources/arista/inventory.v1;inventory',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n#arista/inventory.v1/inventory.proto\x12\x13\x61rista.inventory.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x14\x66mp/extensions.proto\x1a\x0e\x66mp/inet.proto\"\xa1\x01\n\x12\x45xtendedAttributes\x12T\n\x0f\x66\x65\x61ture_enabled\x18\x01 \x03(\x0b\x32;.arista.inventory.v1.ExtendedAttributes.FeatureEnabledEntry\x1a\x35\n\x13\x46\x65\x61tureEnabledEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\"B\n\tDeviceKey\x12/\n\tdevice_id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue:\x04\x80\x8e\x19\x01\"\x8d\x01\n\x13\x44\x65viceConfiguration\x12\x46\n\x07options\x18\x01 \x03(\x0b\x32\x35.arista.inventory.v1.DeviceConfiguration.OptionsEntry\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"A\n\x07UUIDKey\x12\x30\n\nrequest_id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue:\x04\x80\x8e\x19\x01\"\xf5\x01\n\x16\x44\x65viceOnboardingConfig\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12\x34\n\x0ehostname_or_ip\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x64\x65vice_type\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12?\n\rdevice_config\x18\x04 \x01(\x0b\x32(.arista.inventory.v1.DeviceConfiguration:\x06\xfa\x8d\x19\x02rw\"\x90\x02\n\x10\x44\x65viceOnboarding\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12/\n\tdevice_id\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x35\n\x06status\x18\x03 \x01(\x0e\x32%.arista.inventory.v1.OnboardingStatus\x12+\n\x05\x65rror\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x34\n\x0estatus_message\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue:\x06\xfa\x8d\x19\x02ro\"\x81\x01\n\x1b\x44\x65viceDecommissioningConfig\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12/\n\tdevice_id\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue:\x06\xfa\x8d\x19\x02rw\"\xe9\x01\n\x15\x44\x65viceDecommissioning\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12:\n\x06status\x18\x02 \x01(\x0e\x32*.arista.inventory.v1.DecommissioningStatus\x12+\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x34\n\x0estatus_message\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue:\x06\xfa\x8d\x19\x02ro\"\xde\x04\n\x06\x44\x65vice\x12+\n\x03key\x18\x01 \x01(\x0b\x32\x1e.arista.inventory.v1.DeviceKey\x12\x36\n\x10software_version\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nmodel_name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x37\n\x11hardware_revision\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04\x66qdn\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08hostname\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x64omain_name\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x38\n\x12system_mac_address\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\tboot_time\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x10streaming_status\x18\x1e \x01(\x0e\x32$.arista.inventory.v1.StreamingStatus\x12\x44\n\x13\x65xtended_attributes\x18\x1f \x01(\x0b\x32\'.arista.inventory.v1.ExtendedAttributes:\x06\xfa\x8d\x19\x02ro\"\xbf\x02\n\x11ProvisionedDevice\x12+\n\x03key\x18\x01 \x01(\x0b\x32\x1e.arista.inventory.v1.DeviceKey\x12\x37\n\x06status\x18\x02 \x01(\x0e\x32\'.arista.inventory.v1.ProvisioningStatus\x12+\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x08ztp_mode\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\"\n\nip_address\x18\x05 \x01(\x0b\x32\x0e.fmp.IPAddress\x12=\n\x17provisioning_group_name\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue:\x06\xfa\x8d\x19\x02ro*o\n\x0fStreamingStatus\x12 \n\x1cSTREAMING_STATUS_UNSPECIFIED\x10\x00\x12\x1d\n\x19STREAMING_STATUS_INACTIVE\x10\x01\x12\x1b\n\x17STREAMING_STATUS_ACTIVE\x10\x02*\x96\x01\n\x10OnboardingStatus\x12!\n\x1dONBOARDING_STATUS_UNSPECIFIED\x10\x00\x12!\n\x1dONBOARDING_STATUS_IN_PROGRESS\x10\x01\x12\x1d\n\x19ONBOARDING_STATUS_FAILURE\x10\x02\x12\x1d\n\x19ONBOARDING_STATUS_SUCCESS\x10\x03*\xaf\x01\n\x15\x44\x65\x63ommissioningStatus\x12&\n\"DECOMMISSIONING_STATUS_UNSPECIFIED\x10\x00\x12&\n\"DECOMMISSIONING_STATUS_IN_PROGRESS\x10\x01\x12\"\n\x1e\x44\x45\x43OMMISSIONING_STATUS_FAILURE\x10\x02\x12\"\n\x1e\x44\x45\x43OMMISSIONING_STATUS_SUCCESS\x10\x03*\xa0\x01\n\x12ProvisioningStatus\x12#\n\x1fPROVISIONING_STATUS_UNSPECIFIED\x10\x00\x12#\n\x1fPROVISIONING_STATUS_IN_PROGRESS\x10\x01\x12\x1f\n\x1bPROVISIONING_STATUS_FAILURE\x10\x02\x12\x1f\n\x1bPROVISIONING_STATUS_SUCCESS\x10\x03\x42\x30Z.arista/resources/arista/inventory.v1;inventoryb\x06proto3'
+  serialized_pb=b'\n#arista/inventory.v1/inventory.proto\x12\x13\x61rista.inventory.v1\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x14\x66mp/extensions.proto\x1a\x0e\x66mp/inet.proto\"\xa1\x01\n\x12\x45xtendedAttributes\x12T\n\x0f\x66\x65\x61ture_enabled\x18\x01 \x03(\x0b\x32;.arista.inventory.v1.ExtendedAttributes.FeatureEnabledEntry\x1a\x35\n\x13\x46\x65\x61tureEnabledEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\"B\n\tDeviceKey\x12/\n\tdevice_id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue:\x04\x80\x8e\x19\x01\"\x8d\x01\n\x13\x44\x65viceConfiguration\x12\x46\n\x07options\x18\x01 \x03(\x0b\x32\x35.arista.inventory.v1.DeviceConfiguration.OptionsEntry\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"A\n\x07UUIDKey\x12\x30\n\nrequest_id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue:\x04\x80\x8e\x19\x01\"\xf5\x01\n\x16\x44\x65viceOnboardingConfig\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12\x34\n\x0ehostname_or_ip\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x64\x65vice_type\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12?\n\rdevice_config\x18\x04 \x01(\x0b\x32(.arista.inventory.v1.DeviceConfiguration:\x06\xfa\x8d\x19\x02rw\"\x90\x02\n\x10\x44\x65viceOnboarding\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12/\n\tdevice_id\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x35\n\x06status\x18\x03 \x01(\x0e\x32%.arista.inventory.v1.OnboardingStatus\x12+\n\x05\x65rror\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x34\n\x0estatus_message\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue:\x06\xfa\x8d\x19\x02ro\"\xac\x01\n\x1b\x44\x65viceDecommissioningConfig\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12/\n\tdevice_id\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x05\x66orce\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.BoolValue:\x06\xfa\x8d\x19\x02rw\"\xe9\x01\n\x15\x44\x65viceDecommissioning\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12:\n\x06status\x18\x02 \x01(\x0e\x32*.arista.inventory.v1.DecommissioningStatus\x12+\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x34\n\x0estatus_message\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue:\x06\xfa\x8d\x19\x02ro\"\xde\x04\n\x06\x44\x65vice\x12+\n\x03key\x18\x01 \x01(\x0b\x32\x1e.arista.inventory.v1.DeviceKey\x12\x36\n\x10software_version\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nmodel_name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x37\n\x11hardware_revision\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04\x66qdn\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08hostname\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x64omain_name\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x38\n\x12system_mac_address\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\tboot_time\x18\x14 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12>\n\x10streaming_status\x18\x1e \x01(\x0e\x32$.arista.inventory.v1.StreamingStatus\x12\x44\n\x13\x65xtended_attributes\x18\x1f \x01(\x0b\x32\'.arista.inventory.v1.ExtendedAttributes:\x06\xfa\x8d\x19\x02ro\"\xbf\x02\n\x11ProvisionedDevice\x12+\n\x03key\x18\x01 \x01(\x0b\x32\x1e.arista.inventory.v1.DeviceKey\x12\x37\n\x06status\x18\x02 \x01(\x0e\x32\'.arista.inventory.v1.ProvisioningStatus\x12+\n\x05\x65rror\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x08ztp_mode\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\"\n\nip_address\x18\x05 \x01(\x0b\x32\x0e.fmp.IPAddress\x12=\n\x17provisioning_group_name\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue:\x06\xfa\x8d\x19\x02ro*o\n\x0fStreamingStatus\x12 \n\x1cSTREAMING_STATUS_UNSPECIFIED\x10\x00\x12\x1d\n\x19STREAMING_STATUS_INACTIVE\x10\x01\x12\x1b\n\x17STREAMING_STATUS_ACTIVE\x10\x02*\x96\x01\n\x10OnboardingStatus\x12!\n\x1dONBOARDING_STATUS_UNSPECIFIED\x10\x00\x12!\n\x1dONBOARDING_STATUS_IN_PROGRESS\x10\x01\x12\x1d\n\x19ONBOARDING_STATUS_FAILURE\x10\x02\x12\x1d\n\x19ONBOARDING_STATUS_SUCCESS\x10\x03*\xaf\x01\n\x15\x44\x65\x63ommissioningStatus\x12&\n\"DECOMMISSIONING_STATUS_UNSPECIFIED\x10\x00\x12&\n\"DECOMMISSIONING_STATUS_IN_PROGRESS\x10\x01\x12\"\n\x1e\x44\x45\x43OMMISSIONING_STATUS_FAILURE\x10\x02\x12\"\n\x1e\x44\x45\x43OMMISSIONING_STATUS_SUCCESS\x10\x03*\xa0\x01\n\x12ProvisioningStatus\x12#\n\x1fPROVISIONING_STATUS_UNSPECIFIED\x10\x00\x12#\n\x1fPROVISIONING_STATUS_IN_PROGRESS\x10\x01\x12\x1f\n\x1bPROVISIONING_STATUS_FAILURE\x10\x02\x12\x1f\n\x1bPROVISIONING_STATUS_SUCCESS\x10\x03\x42\x30Z.arista/resources/arista/inventory.v1;inventoryb\x06proto3'
   ,
   dependencies=[google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,google_dot_protobuf_dot_wrappers__pb2.DESCRIPTOR,fmp_dot_extensions__pb2.DESCRIPTOR,fmp_dot_inet__pb2.DESCRIPTOR,])
 
 _STREAMINGSTATUS = _descriptor.EnumDescriptor(
   name='StreamingStatus',
   full_name='arista.inventory.v1.StreamingStatus',
   filename=None,
@@ -49,16 +49,16 @@
       name='STREAMING_STATUS_ACTIVE', index=2, number=2,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2428,
-  serialized_end=2539,
+  serialized_start=2471,
+  serialized_end=2582,
 )
 _sym_db.RegisterEnumDescriptor(_STREAMINGSTATUS)
 
 StreamingStatus = enum_type_wrapper.EnumTypeWrapper(_STREAMINGSTATUS)
 _ONBOARDINGSTATUS = _descriptor.EnumDescriptor(
   name='OnboardingStatus',
   full_name='arista.inventory.v1.OnboardingStatus',
@@ -85,16 +85,16 @@
       name='ONBOARDING_STATUS_SUCCESS', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2542,
-  serialized_end=2692,
+  serialized_start=2585,
+  serialized_end=2735,
 )
 _sym_db.RegisterEnumDescriptor(_ONBOARDINGSTATUS)
 
 OnboardingStatus = enum_type_wrapper.EnumTypeWrapper(_ONBOARDINGSTATUS)
 _DECOMMISSIONINGSTATUS = _descriptor.EnumDescriptor(
   name='DecommissioningStatus',
   full_name='arista.inventory.v1.DecommissioningStatus',
@@ -121,16 +121,16 @@
       name='DECOMMISSIONING_STATUS_SUCCESS', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2695,
-  serialized_end=2870,
+  serialized_start=2738,
+  serialized_end=2913,
 )
 _sym_db.RegisterEnumDescriptor(_DECOMMISSIONINGSTATUS)
 
 DecommissioningStatus = enum_type_wrapper.EnumTypeWrapper(_DECOMMISSIONINGSTATUS)
 _PROVISIONINGSTATUS = _descriptor.EnumDescriptor(
   name='ProvisioningStatus',
   full_name='arista.inventory.v1.ProvisioningStatus',
@@ -157,16 +157,16 @@
       name='PROVISIONING_STATUS_SUCCESS', index=3, number=3,
       serialized_options=None,
       type=None,
       create_key=_descriptor._internal_create_key),
   ],
   containing_type=None,
   serialized_options=None,
-  serialized_start=2873,
-  serialized_end=3033,
+  serialized_start=2916,
+  serialized_end=3076,
 )
 _sym_db.RegisterEnumDescriptor(_PROVISIONINGSTATUS)
 
 ProvisioningStatus = enum_type_wrapper.EnumTypeWrapper(_PROVISIONINGSTATUS)
 STREAMING_STATUS_UNSPECIFIED = 0
 STREAMING_STATUS_INACTIVE = 1
 STREAMING_STATUS_ACTIVE = 2
@@ -520,28 +520,35 @@
     _descriptor.FieldDescriptor(
       name='device_id', full_name='arista.inventory.v1.DeviceDecommissioningConfig.device_id', index=1,
       number=2, type=11, cpp_type=10, label=1,
       has_default_value=False, default_value=None,
       message_type=None, enum_type=None, containing_type=None,
       is_extension=False, extension_scope=None,
       serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='force', full_name='arista.inventory.v1.DeviceDecommissioningConfig.force', index=2,
+      number=3, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
   ],
   extensions=[
   ],
   nested_types=[],
   enum_types=[
   ],
   serialized_options=b'\372\215\031\002rw',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
   serialized_start=1130,
-  serialized_end=1259,
+  serialized_end=1302,
 )
 
 
 _DEVICEDECOMMISSIONING = _descriptor.Descriptor(
   name='DeviceDecommissioning',
   full_name='arista.inventory.v1.DeviceDecommissioning',
   filename=None,
@@ -585,16 +592,16 @@
   ],
   serialized_options=b'\372\215\031\002ro',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1262,
-  serialized_end=1495,
+  serialized_start=1305,
+  serialized_end=1538,
 )
 
 
 _DEVICE = _descriptor.Descriptor(
   name='Device',
   full_name='arista.inventory.v1.Device',
   filename=None,
@@ -687,16 +694,16 @@
   ],
   serialized_options=b'\372\215\031\002ro',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1498,
-  serialized_end=2104,
+  serialized_start=1541,
+  serialized_end=2147,
 )
 
 
 _PROVISIONEDDEVICE = _descriptor.Descriptor(
   name='ProvisionedDevice',
   full_name='arista.inventory.v1.ProvisionedDevice',
   filename=None,
@@ -754,16 +761,16 @@
   ],
   serialized_options=b'\372\215\031\002ro',
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2107,
-  serialized_end=2426,
+  serialized_start=2150,
+  serialized_end=2469,
 )
 
 _EXTENDEDATTRIBUTES_FEATUREENABLEDENTRY.containing_type = _EXTENDEDATTRIBUTES
 _EXTENDEDATTRIBUTES.fields_by_name['feature_enabled'].message_type = _EXTENDEDATTRIBUTES_FEATUREENABLEDENTRY
 _DEVICEKEY.fields_by_name['device_id'].message_type = google_dot_protobuf_dot_wrappers__pb2._STRINGVALUE
 _DEVICECONFIGURATION_OPTIONSENTRY.containing_type = _DEVICECONFIGURATION
 _DEVICECONFIGURATION.fields_by_name['options'].message_type = _DEVICECONFIGURATION_OPTIONSENTRY
@@ -775,14 +782,15 @@
 _DEVICEONBOARDING.fields_by_name['key'].message_type = _UUIDKEY
 _DEVICEONBOARDING.fields_by_name['device_id'].message_type = google_dot_protobuf_dot_wrappers__pb2._STRINGVALUE
 _DEVICEONBOARDING.fields_by_name['status'].enum_type = _ONBOARDINGSTATUS
 _DEVICEONBOARDING.fields_by_name['error'].message_type = google_dot_protobuf_dot_wrappers__pb2._STRINGVALUE
 _DEVICEONBOARDING.fields_by_name['status_message'].message_type = google_dot_protobuf_dot_wrappers__pb2._STRINGVALUE
 _DEVICEDECOMMISSIONINGCONFIG.fields_by_name['key'].message_type = _UUIDKEY
 _DEVICEDECOMMISSIONINGCONFIG.fields_by_name['device_id'].message_type = google_dot_protobuf_dot_wrappers__pb2._STRINGVALUE
+_DEVICEDECOMMISSIONINGCONFIG.fields_by_name['force'].message_type = google_dot_protobuf_dot_wrappers__pb2._BOOLVALUE
 _DEVICEDECOMMISSIONING.fields_by_name['key'].message_type = _UUIDKEY
 _DEVICEDECOMMISSIONING.fields_by_name['status'].enum_type = _DECOMMISSIONINGSTATUS
 _DEVICEDECOMMISSIONING.fields_by_name['error'].message_type = google_dot_protobuf_dot_wrappers__pb2._STRINGVALUE
 _DEVICEDECOMMISSIONING.fields_by_name['status_message'].message_type = google_dot_protobuf_dot_wrappers__pb2._STRINGVALUE
 _DEVICE.fields_by_name['key'].message_type = _DEVICEKEY
 _DEVICE.fields_by_name['software_version'].message_type = google_dot_protobuf_dot_wrappers__pb2._STRINGVALUE
 _DEVICE.fields_by_name['model_name'].message_type = google_dot_protobuf_dot_wrappers__pb2._STRINGVALUE
```

### Comparing `cloudvision-1.9.0/arista/inventory/v1/services/gen_pb2.py` & `cloudvision-1.9.1/arista/inventory/v1/services/gen_pb2.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,26 +10,28 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from arista.inventory.v1 import inventory_pb2 as arista_dot_inventory_dot_v1_dot_inventory__pb2
 from arista.time import time_pb2 as arista_dot_time_dot_time__pb2
 from arista.subscriptions import subscriptions_pb2 as arista_dot_subscriptions_dot_subscriptions__pb2
+from fmp import deletes_pb2 as fmp_dot_deletes__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
 DESCRIPTOR = _descriptor.FileDescriptor(
   name='arista/inventory.v1/services.gen.proto',
   package='arista.inventory.v1',
   syntax='proto3',
   serialized_options=b'Z.arista/resources/arista/inventory.v1;inventory',
   create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n&arista/inventory.v1/services.gen.proto\x12\x13\x61rista.inventory.v1\x1a#arista/inventory.v1/inventory.proto\x1a\x16\x61rista/time/time.proto\x1a(arista/subscriptions/subscriptions.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"f\n\rDeviceRequest\x12+\n\x03key\x18\x01 \x01(\x0b\x32\x1e.arista.inventory.v1.DeviceKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"f\n\x0e\x44\x65viceResponse\x12*\n\x05value\x18\x01 \x01(\x0b\x32\x1b.arista.inventory.v1.Device\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"t\n\x13\x44\x65viceStreamRequest\x12\x36\n\x11partial_eq_filter\x18\x01 \x03(\x0b\x32\x1b.arista.inventory.v1.Device\x12%\n\x04time\x18\x03 \x01(\x0b\x32\x17.arista.time.TimeBounds\"\x9b\x01\n\x14\x44\x65viceStreamResponse\x12*\n\x05value\x18\x01 \x01(\x0b\x32\x1b.arista.inventory.v1.Device\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x04type\x18\x03 \x01(\x0e\x32\x1f.arista.subscriptions.Operation\"s\n\x1c\x44\x65viceDecommissioningRequest\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x84\x01\n\x1d\x44\x65viceDecommissioningResponse\x12\x39\n\x05value\x18\x01 \x01(\x0b\x32*.arista.inventory.v1.DeviceDecommissioning\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x92\x01\n\"DeviceDecommissioningStreamRequest\x12\x45\n\x11partial_eq_filter\x18\x01 \x03(\x0b\x32*.arista.inventory.v1.DeviceDecommissioning\x12%\n\x04time\x18\x03 \x01(\x0b\x32\x17.arista.time.TimeBounds\"\xb9\x01\n#DeviceDecommissioningStreamResponse\x12\x39\n\x05value\x18\x01 \x01(\x0b\x32*.arista.inventory.v1.DeviceDecommissioning\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x04type\x18\x03 \x01(\x0e\x32\x1f.arista.subscriptions.Operation\"y\n\"DeviceDecommissioningConfigRequest\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x90\x01\n#DeviceDecommissioningConfigResponse\x12?\n\x05value\x18\x01 \x01(\x0b\x32\x30.arista.inventory.v1.DeviceDecommissioningConfig\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x9e\x01\n(DeviceDecommissioningConfigStreamRequest\x12K\n\x11partial_eq_filter\x18\x01 \x03(\x0b\x32\x30.arista.inventory.v1.DeviceDecommissioningConfig\x12%\n\x04time\x18\x03 \x01(\x0b\x32\x17.arista.time.TimeBounds\"\xc5\x01\n)DeviceDecommissioningConfigStreamResponse\x12?\n\x05value\x18\x01 \x01(\x0b\x32\x30.arista.inventory.v1.DeviceDecommissioningConfig\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x04type\x18\x03 \x01(\x0e\x32\x1f.arista.subscriptions.Operation\"h\n%DeviceDecommissioningConfigSetRequest\x12?\n\x05value\x18\x01 \x01(\x0b\x32\x30.arista.inventory.v1.DeviceDecommissioningConfig\"\x93\x01\n&DeviceDecommissioningConfigSetResponse\x12?\n\x05value\x18\x01 \x01(\x0b\x32\x30.arista.inventory.v1.DeviceDecommissioningConfig\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"U\n(DeviceDecommissioningConfigDeleteRequest\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\"\x80\x01\n)DeviceDecommissioningConfigDeleteResponse\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"n\n\x17\x44\x65viceOnboardingRequest\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"z\n\x18\x44\x65viceOnboardingResponse\x12\x34\n\x05value\x18\x01 \x01(\x0b\x32%.arista.inventory.v1.DeviceOnboarding\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x88\x01\n\x1d\x44\x65viceOnboardingStreamRequest\x12@\n\x11partial_eq_filter\x18\x01 \x03(\x0b\x32%.arista.inventory.v1.DeviceOnboarding\x12%\n\x04time\x18\x03 \x01(\x0b\x32\x17.arista.time.TimeBounds\"\xaf\x01\n\x1e\x44\x65viceOnboardingStreamResponse\x12\x34\n\x05value\x18\x01 \x01(\x0b\x32%.arista.inventory.v1.DeviceOnboarding\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x04type\x18\x03 \x01(\x0e\x32\x1f.arista.subscriptions.Operation\"t\n\x1d\x44\x65viceOnboardingConfigRequest\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x86\x01\n\x1e\x44\x65viceOnboardingConfigResponse\x12:\n\x05value\x18\x01 \x01(\x0b\x32+.arista.inventory.v1.DeviceOnboardingConfig\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x94\x01\n#DeviceOnboardingConfigStreamRequest\x12\x46\n\x11partial_eq_filter\x18\x01 \x03(\x0b\x32+.arista.inventory.v1.DeviceOnboardingConfig\x12%\n\x04time\x18\x03 \x01(\x0b\x32\x17.arista.time.TimeBounds\"\xbb\x01\n$DeviceOnboardingConfigStreamResponse\x12:\n\x05value\x18\x01 \x01(\x0b\x32+.arista.inventory.v1.DeviceOnboardingConfig\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x04type\x18\x03 \x01(\x0e\x32\x1f.arista.subscriptions.Operation\"^\n DeviceOnboardingConfigSetRequest\x12:\n\x05value\x18\x01 \x01(\x0b\x32+.arista.inventory.v1.DeviceOnboardingConfig\"\x89\x01\n!DeviceOnboardingConfigSetResponse\x12:\n\x05value\x18\x01 \x01(\x0b\x32+.arista.inventory.v1.DeviceOnboardingConfig\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"P\n#DeviceOnboardingConfigDeleteRequest\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\"{\n$DeviceOnboardingConfigDeleteResponse\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"q\n\x18ProvisionedDeviceRequest\x12+\n\x03key\x18\x01 \x01(\x0b\x32\x1e.arista.inventory.v1.DeviceKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"|\n\x19ProvisionedDeviceResponse\x12\x35\n\x05value\x18\x01 \x01(\x0b\x32&.arista.inventory.v1.ProvisionedDevice\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x8a\x01\n\x1eProvisionedDeviceStreamRequest\x12\x41\n\x11partial_eq_filter\x18\x01 \x03(\x0b\x32&.arista.inventory.v1.ProvisionedDevice\x12%\n\x04time\x18\x03 \x01(\x0b\x32\x17.arista.time.TimeBounds\"\xb1\x01\n\x1fProvisionedDeviceStreamResponse\x12\x35\n\x05value\x18\x01 \x01(\x0b\x32&.arista.inventory.v1.ProvisionedDevice\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x04type\x18\x03 \x01(\x0e\x32\x1f.arista.subscriptions.Operation2\xa7\x02\n\rDeviceService\x12Q\n\x06GetOne\x12\".arista.inventory.v1.DeviceRequest\x1a#.arista.inventory.v1.DeviceResponse\x12_\n\x06GetAll\x12(.arista.inventory.v1.DeviceStreamRequest\x1a).arista.inventory.v1.DeviceStreamResponse0\x01\x12\x62\n\tSubscribe\x12(.arista.inventory.v1.DeviceStreamRequest\x1a).arista.inventory.v1.DeviceStreamResponse0\x01\x32\x91\x03\n\x1c\x44\x65viceDecommissioningService\x12o\n\x06GetOne\x12\x31.arista.inventory.v1.DeviceDecommissioningRequest\x1a\x32.arista.inventory.v1.DeviceDecommissioningResponse\x12}\n\x06GetAll\x12\x37.arista.inventory.v1.DeviceDecommissioningStreamRequest\x1a\x38.arista.inventory.v1.DeviceDecommissioningStreamResponse0\x01\x12\x80\x01\n\tSubscribe\x12\x37.arista.inventory.v1.DeviceDecommissioningStreamRequest\x1a\x38.arista.inventory.v1.DeviceDecommissioningStreamResponse0\x01\x32\xc6\x05\n\"DeviceDecommissioningConfigService\x12{\n\x06GetOne\x12\x37.arista.inventory.v1.DeviceDecommissioningConfigRequest\x1a\x38.arista.inventory.v1.DeviceDecommissioningConfigResponse\x12\x89\x01\n\x06GetAll\x12=.arista.inventory.v1.DeviceDecommissioningConfigStreamRequest\x1a>.arista.inventory.v1.DeviceDecommissioningConfigStreamResponse0\x01\x12\x8c\x01\n\tSubscribe\x12=.arista.inventory.v1.DeviceDecommissioningConfigStreamRequest\x1a>.arista.inventory.v1.DeviceDecommissioningConfigStreamResponse0\x01\x12~\n\x03Set\x12:.arista.inventory.v1.DeviceDecommissioningConfigSetRequest\x1a;.arista.inventory.v1.DeviceDecommissioningConfigSetResponse\x12\x87\x01\n\x06\x44\x65lete\x12=.arista.inventory.v1.DeviceDecommissioningConfigDeleteRequest\x1a>.arista.inventory.v1.DeviceDecommissioningConfigDeleteResponse2\xed\x02\n\x17\x44\x65viceOnboardingService\x12\x65\n\x06GetOne\x12,.arista.inventory.v1.DeviceOnboardingRequest\x1a-.arista.inventory.v1.DeviceOnboardingResponse\x12s\n\x06GetAll\x12\x32.arista.inventory.v1.DeviceOnboardingStreamRequest\x1a\x33.arista.inventory.v1.DeviceOnboardingStreamResponse0\x01\x12v\n\tSubscribe\x12\x32.arista.inventory.v1.DeviceOnboardingStreamRequest\x1a\x33.arista.inventory.v1.DeviceOnboardingStreamResponse0\x01\x32\x8d\x05\n\x1d\x44\x65viceOnboardingConfigService\x12q\n\x06GetOne\x12\x32.arista.inventory.v1.DeviceOnboardingConfigRequest\x1a\x33.arista.inventory.v1.DeviceOnboardingConfigResponse\x12\x7f\n\x06GetAll\x12\x38.arista.inventory.v1.DeviceOnboardingConfigStreamRequest\x1a\x39.arista.inventory.v1.DeviceOnboardingConfigStreamResponse0\x01\x12\x82\x01\n\tSubscribe\x12\x38.arista.inventory.v1.DeviceOnboardingConfigStreamRequest\x1a\x39.arista.inventory.v1.DeviceOnboardingConfigStreamResponse0\x01\x12t\n\x03Set\x12\x35.arista.inventory.v1.DeviceOnboardingConfigSetRequest\x1a\x36.arista.inventory.v1.DeviceOnboardingConfigSetResponse\x12}\n\x06\x44\x65lete\x12\x38.arista.inventory.v1.DeviceOnboardingConfigDeleteRequest\x1a\x39.arista.inventory.v1.DeviceOnboardingConfigDeleteResponse2\xf4\x02\n\x18ProvisionedDeviceService\x12g\n\x06GetOne\x12-.arista.inventory.v1.ProvisionedDeviceRequest\x1a..arista.inventory.v1.ProvisionedDeviceResponse\x12u\n\x06GetAll\x12\x33.arista.inventory.v1.ProvisionedDeviceStreamRequest\x1a\x34.arista.inventory.v1.ProvisionedDeviceStreamResponse0\x01\x12x\n\tSubscribe\x12\x33.arista.inventory.v1.ProvisionedDeviceStreamRequest\x1a\x34.arista.inventory.v1.ProvisionedDeviceStreamResponse0\x01\x42\x30Z.arista/resources/arista/inventory.v1;inventoryb\x06proto3'
+  serialized_pb=b'\n&arista/inventory.v1/services.gen.proto\x12\x13\x61rista.inventory.v1\x1a#arista/inventory.v1/inventory.proto\x1a\x16\x61rista/time/time.proto\x1a(arista/subscriptions/subscriptions.proto\x1a\x11\x66mp/deletes.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\"f\n\rDeviceRequest\x12+\n\x03key\x18\x01 \x01(\x0b\x32\x1e.arista.inventory.v1.DeviceKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"f\n\x0e\x44\x65viceResponse\x12*\n\x05value\x18\x01 \x01(\x0b\x32\x1b.arista.inventory.v1.Device\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"t\n\x13\x44\x65viceStreamRequest\x12\x36\n\x11partial_eq_filter\x18\x01 \x03(\x0b\x32\x1b.arista.inventory.v1.Device\x12%\n\x04time\x18\x03 \x01(\x0b\x32\x17.arista.time.TimeBounds\"\x9b\x01\n\x14\x44\x65viceStreamResponse\x12*\n\x05value\x18\x01 \x01(\x0b\x32\x1b.arista.inventory.v1.Device\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x04type\x18\x03 \x01(\x0e\x32\x1f.arista.subscriptions.Operation\"s\n\x1c\x44\x65viceDecommissioningRequest\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x84\x01\n\x1d\x44\x65viceDecommissioningResponse\x12\x39\n\x05value\x18\x01 \x01(\x0b\x32*.arista.inventory.v1.DeviceDecommissioning\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x92\x01\n\"DeviceDecommissioningStreamRequest\x12\x45\n\x11partial_eq_filter\x18\x01 \x03(\x0b\x32*.arista.inventory.v1.DeviceDecommissioning\x12%\n\x04time\x18\x03 \x01(\x0b\x32\x17.arista.time.TimeBounds\"\xb9\x01\n#DeviceDecommissioningStreamResponse\x12\x39\n\x05value\x18\x01 \x01(\x0b\x32*.arista.inventory.v1.DeviceDecommissioning\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x04type\x18\x03 \x01(\x0e\x32\x1f.arista.subscriptions.Operation\"y\n\"DeviceDecommissioningConfigRequest\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x90\x01\n#DeviceDecommissioningConfigResponse\x12?\n\x05value\x18\x01 \x01(\x0b\x32\x30.arista.inventory.v1.DeviceDecommissioningConfig\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x9e\x01\n(DeviceDecommissioningConfigStreamRequest\x12K\n\x11partial_eq_filter\x18\x01 \x03(\x0b\x32\x30.arista.inventory.v1.DeviceDecommissioningConfig\x12%\n\x04time\x18\x03 \x01(\x0b\x32\x17.arista.time.TimeBounds\"\xc5\x01\n)DeviceDecommissioningConfigStreamResponse\x12?\n\x05value\x18\x01 \x01(\x0b\x32\x30.arista.inventory.v1.DeviceDecommissioningConfig\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x04type\x18\x03 \x01(\x0e\x32\x1f.arista.subscriptions.Operation\"h\n%DeviceDecommissioningConfigSetRequest\x12?\n\x05value\x18\x01 \x01(\x0b\x32\x30.arista.inventory.v1.DeviceDecommissioningConfig\"\x93\x01\n&DeviceDecommissioningConfigSetResponse\x12?\n\x05value\x18\x01 \x01(\x0b\x32\x30.arista.inventory.v1.DeviceDecommissioningConfig\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"U\n(DeviceDecommissioningConfigDeleteRequest\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\"\x80\x01\n)DeviceDecommissioningConfigDeleteResponse\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"-\n+DeviceDecommissioningConfigDeleteAllRequest\"\xd0\x01\n,DeviceDecommissioningConfigDeleteAllResponse\x12\x1e\n\x04type\x18\x01 \x01(\x0e\x32\x10.fmp.DeleteError\x12+\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03key\x18\x03 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12(\n\x04time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"n\n\x17\x44\x65viceOnboardingRequest\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"z\n\x18\x44\x65viceOnboardingResponse\x12\x34\n\x05value\x18\x01 \x01(\x0b\x32%.arista.inventory.v1.DeviceOnboarding\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x88\x01\n\x1d\x44\x65viceOnboardingStreamRequest\x12@\n\x11partial_eq_filter\x18\x01 \x03(\x0b\x32%.arista.inventory.v1.DeviceOnboarding\x12%\n\x04time\x18\x03 \x01(\x0b\x32\x17.arista.time.TimeBounds\"\xaf\x01\n\x1e\x44\x65viceOnboardingStreamResponse\x12\x34\n\x05value\x18\x01 \x01(\x0b\x32%.arista.inventory.v1.DeviceOnboarding\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x04type\x18\x03 \x01(\x0e\x32\x1f.arista.subscriptions.Operation\"t\n\x1d\x44\x65viceOnboardingConfigRequest\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x86\x01\n\x1e\x44\x65viceOnboardingConfigResponse\x12:\n\x05value\x18\x01 \x01(\x0b\x32+.arista.inventory.v1.DeviceOnboardingConfig\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x94\x01\n#DeviceOnboardingConfigStreamRequest\x12\x46\n\x11partial_eq_filter\x18\x01 \x03(\x0b\x32+.arista.inventory.v1.DeviceOnboardingConfig\x12%\n\x04time\x18\x03 \x01(\x0b\x32\x17.arista.time.TimeBounds\"\xbb\x01\n$DeviceOnboardingConfigStreamResponse\x12:\n\x05value\x18\x01 \x01(\x0b\x32+.arista.inventory.v1.DeviceOnboardingConfig\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x04type\x18\x03 \x01(\x0e\x32\x1f.arista.subscriptions.Operation\"^\n DeviceOnboardingConfigSetRequest\x12:\n\x05value\x18\x01 \x01(\x0b\x32+.arista.inventory.v1.DeviceOnboardingConfig\"\x89\x01\n!DeviceOnboardingConfigSetResponse\x12:\n\x05value\x18\x01 \x01(\x0b\x32+.arista.inventory.v1.DeviceOnboardingConfig\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"P\n#DeviceOnboardingConfigDeleteRequest\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\"{\n$DeviceOnboardingConfigDeleteResponse\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"(\n&DeviceOnboardingConfigDeleteAllRequest\"\xcb\x01\n\'DeviceOnboardingConfigDeleteAllResponse\x12\x1e\n\x04type\x18\x01 \x01(\x0e\x32\x10.fmp.DeleteError\x12+\n\x05\x65rror\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03key\x18\x03 \x01(\x0b\x32\x1c.arista.inventory.v1.UUIDKey\x12(\n\x04time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"q\n\x18ProvisionedDeviceRequest\x12+\n\x03key\x18\x01 \x01(\x0b\x32\x1e.arista.inventory.v1.DeviceKey\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"|\n\x19ProvisionedDeviceResponse\x12\x35\n\x05value\x18\x01 \x01(\x0b\x32&.arista.inventory.v1.ProvisionedDevice\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x8a\x01\n\x1eProvisionedDeviceStreamRequest\x12\x41\n\x11partial_eq_filter\x18\x01 \x03(\x0b\x32&.arista.inventory.v1.ProvisionedDevice\x12%\n\x04time\x18\x03 \x01(\x0b\x32\x17.arista.time.TimeBounds\"\xb1\x01\n\x1fProvisionedDeviceStreamResponse\x12\x35\n\x05value\x18\x01 \x01(\x0b\x32&.arista.inventory.v1.ProvisionedDevice\x12(\n\x04time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12-\n\x04type\x18\x03 \x01(\x0e\x32\x1f.arista.subscriptions.Operation2\xa7\x02\n\rDeviceService\x12Q\n\x06GetOne\x12\".arista.inventory.v1.DeviceRequest\x1a#.arista.inventory.v1.DeviceResponse\x12_\n\x06GetAll\x12(.arista.inventory.v1.DeviceStreamRequest\x1a).arista.inventory.v1.DeviceStreamResponse0\x01\x12\x62\n\tSubscribe\x12(.arista.inventory.v1.DeviceStreamRequest\x1a).arista.inventory.v1.DeviceStreamResponse0\x01\x32\x91\x03\n\x1c\x44\x65viceDecommissioningService\x12o\n\x06GetOne\x12\x31.arista.inventory.v1.DeviceDecommissioningRequest\x1a\x32.arista.inventory.v1.DeviceDecommissioningResponse\x12}\n\x06GetAll\x12\x37.arista.inventory.v1.DeviceDecommissioningStreamRequest\x1a\x38.arista.inventory.v1.DeviceDecommissioningStreamResponse0\x01\x12\x80\x01\n\tSubscribe\x12\x37.arista.inventory.v1.DeviceDecommissioningStreamRequest\x1a\x38.arista.inventory.v1.DeviceDecommissioningStreamResponse0\x01\x32\xdb\x06\n\"DeviceDecommissioningConfigService\x12{\n\x06GetOne\x12\x37.arista.inventory.v1.DeviceDecommissioningConfigRequest\x1a\x38.arista.inventory.v1.DeviceDecommissioningConfigResponse\x12\x89\x01\n\x06GetAll\x12=.arista.inventory.v1.DeviceDecommissioningConfigStreamRequest\x1a>.arista.inventory.v1.DeviceDecommissioningConfigStreamResponse0\x01\x12\x8c\x01\n\tSubscribe\x12=.arista.inventory.v1.DeviceDecommissioningConfigStreamRequest\x1a>.arista.inventory.v1.DeviceDecommissioningConfigStreamResponse0\x01\x12~\n\x03Set\x12:.arista.inventory.v1.DeviceDecommissioningConfigSetRequest\x1a;.arista.inventory.v1.DeviceDecommissioningConfigSetResponse\x12\x87\x01\n\x06\x44\x65lete\x12=.arista.inventory.v1.DeviceDecommissioningConfigDeleteRequest\x1a>.arista.inventory.v1.DeviceDecommissioningConfigDeleteResponse\x12\x92\x01\n\tDeleteAll\x12@.arista.inventory.v1.DeviceDecommissioningConfigDeleteAllRequest\x1a\x41.arista.inventory.v1.DeviceDecommissioningConfigDeleteAllResponse0\x01\x32\xed\x02\n\x17\x44\x65viceOnboardingService\x12\x65\n\x06GetOne\x12,.arista.inventory.v1.DeviceOnboardingRequest\x1a-.arista.inventory.v1.DeviceOnboardingResponse\x12s\n\x06GetAll\x12\x32.arista.inventory.v1.DeviceOnboardingStreamRequest\x1a\x33.arista.inventory.v1.DeviceOnboardingStreamResponse0\x01\x12v\n\tSubscribe\x12\x32.arista.inventory.v1.DeviceOnboardingStreamRequest\x1a\x33.arista.inventory.v1.DeviceOnboardingStreamResponse0\x01\x32\x98\x06\n\x1d\x44\x65viceOnboardingConfigService\x12q\n\x06GetOne\x12\x32.arista.inventory.v1.DeviceOnboardingConfigRequest\x1a\x33.arista.inventory.v1.DeviceOnboardingConfigResponse\x12\x7f\n\x06GetAll\x12\x38.arista.inventory.v1.DeviceOnboardingConfigStreamRequest\x1a\x39.arista.inventory.v1.DeviceOnboardingConfigStreamResponse0\x01\x12\x82\x01\n\tSubscribe\x12\x38.arista.inventory.v1.DeviceOnboardingConfigStreamRequest\x1a\x39.arista.inventory.v1.DeviceOnboardingConfigStreamResponse0\x01\x12t\n\x03Set\x12\x35.arista.inventory.v1.DeviceOnboardingConfigSetRequest\x1a\x36.arista.inventory.v1.DeviceOnboardingConfigSetResponse\x12}\n\x06\x44\x65lete\x12\x38.arista.inventory.v1.DeviceOnboardingConfigDeleteRequest\x1a\x39.arista.inventory.v1.DeviceOnboardingConfigDeleteResponse\x12\x88\x01\n\tDeleteAll\x12;.arista.inventory.v1.DeviceOnboardingConfigDeleteAllRequest\x1a<.arista.inventory.v1.DeviceOnboardingConfigDeleteAllResponse0\x01\x32\xf4\x02\n\x18ProvisionedDeviceService\x12g\n\x06GetOne\x12-.arista.inventory.v1.ProvisionedDeviceRequest\x1a..arista.inventory.v1.ProvisionedDeviceResponse\x12u\n\x06GetAll\x12\x33.arista.inventory.v1.ProvisionedDeviceStreamRequest\x1a\x34.arista.inventory.v1.ProvisionedDeviceStreamResponse0\x01\x12x\n\tSubscribe\x12\x33.arista.inventory.v1.ProvisionedDeviceStreamRequest\x1a\x34.arista.inventory.v1.ProvisionedDeviceStreamResponse0\x01\x42\x30Z.arista/resources/arista/inventory.v1;inventoryb\x06proto3'
   ,
-  dependencies=[arista_dot_inventory_dot_v1_dot_inventory__pb2.DESCRIPTOR,arista_dot_time_dot_time__pb2.DESCRIPTOR,arista_dot_subscriptions_dot_subscriptions__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,])
+  dependencies=[arista_dot_inventory_dot_v1_dot_inventory__pb2.DESCRIPTOR,arista_dot_time_dot_time__pb2.DESCRIPTOR,arista_dot_subscriptions_dot_subscriptions__pb2.DESCRIPTOR,fmp_dot_deletes__pb2.DESCRIPTOR,google_dot_protobuf_dot_timestamp__pb2.DESCRIPTOR,google_dot_protobuf_dot_wrappers__pb2.DESCRIPTOR,])
 
 
 
 
 _DEVICEREQUEST = _descriptor.Descriptor(
   name='DeviceRequest',
   full_name='arista.inventory.v1.DeviceRequest',
@@ -60,16 +62,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=199,
-  serialized_end=301,
+  serialized_start=250,
+  serialized_end=352,
 )
 
 
 _DEVICERESPONSE = _descriptor.Descriptor(
   name='DeviceResponse',
   full_name='arista.inventory.v1.DeviceResponse',
   filename=None,
@@ -99,16 +101,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=303,
-  serialized_end=405,
+  serialized_start=354,
+  serialized_end=456,
 )
 
 
 _DEVICESTREAMREQUEST = _descriptor.Descriptor(
   name='DeviceStreamRequest',
   full_name='arista.inventory.v1.DeviceStreamRequest',
   filename=None,
@@ -138,16 +140,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=407,
-  serialized_end=523,
+  serialized_start=458,
+  serialized_end=574,
 )
 
 
 _DEVICESTREAMRESPONSE = _descriptor.Descriptor(
   name='DeviceStreamResponse',
   full_name='arista.inventory.v1.DeviceStreamResponse',
   filename=None,
@@ -184,16 +186,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=526,
-  serialized_end=681,
+  serialized_start=577,
+  serialized_end=732,
 )
 
 
 _DEVICEDECOMMISSIONINGREQUEST = _descriptor.Descriptor(
   name='DeviceDecommissioningRequest',
   full_name='arista.inventory.v1.DeviceDecommissioningRequest',
   filename=None,
@@ -223,16 +225,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=683,
-  serialized_end=798,
+  serialized_start=734,
+  serialized_end=849,
 )
 
 
 _DEVICEDECOMMISSIONINGRESPONSE = _descriptor.Descriptor(
   name='DeviceDecommissioningResponse',
   full_name='arista.inventory.v1.DeviceDecommissioningResponse',
   filename=None,
@@ -262,16 +264,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=801,
-  serialized_end=933,
+  serialized_start=852,
+  serialized_end=984,
 )
 
 
 _DEVICEDECOMMISSIONINGSTREAMREQUEST = _descriptor.Descriptor(
   name='DeviceDecommissioningStreamRequest',
   full_name='arista.inventory.v1.DeviceDecommissioningStreamRequest',
   filename=None,
@@ -301,16 +303,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=936,
-  serialized_end=1082,
+  serialized_start=987,
+  serialized_end=1133,
 )
 
 
 _DEVICEDECOMMISSIONINGSTREAMRESPONSE = _descriptor.Descriptor(
   name='DeviceDecommissioningStreamResponse',
   full_name='arista.inventory.v1.DeviceDecommissioningStreamResponse',
   filename=None,
@@ -347,16 +349,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1085,
-  serialized_end=1270,
+  serialized_start=1136,
+  serialized_end=1321,
 )
 
 
 _DEVICEDECOMMISSIONINGCONFIGREQUEST = _descriptor.Descriptor(
   name='DeviceDecommissioningConfigRequest',
   full_name='arista.inventory.v1.DeviceDecommissioningConfigRequest',
   filename=None,
@@ -386,16 +388,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1272,
-  serialized_end=1393,
+  serialized_start=1323,
+  serialized_end=1444,
 )
 
 
 _DEVICEDECOMMISSIONINGCONFIGRESPONSE = _descriptor.Descriptor(
   name='DeviceDecommissioningConfigResponse',
   full_name='arista.inventory.v1.DeviceDecommissioningConfigResponse',
   filename=None,
@@ -425,16 +427,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1396,
-  serialized_end=1540,
+  serialized_start=1447,
+  serialized_end=1591,
 )
 
 
 _DEVICEDECOMMISSIONINGCONFIGSTREAMREQUEST = _descriptor.Descriptor(
   name='DeviceDecommissioningConfigStreamRequest',
   full_name='arista.inventory.v1.DeviceDecommissioningConfigStreamRequest',
   filename=None,
@@ -464,16 +466,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1543,
-  serialized_end=1701,
+  serialized_start=1594,
+  serialized_end=1752,
 )
 
 
 _DEVICEDECOMMISSIONINGCONFIGSTREAMRESPONSE = _descriptor.Descriptor(
   name='DeviceDecommissioningConfigStreamResponse',
   full_name='arista.inventory.v1.DeviceDecommissioningConfigStreamResponse',
   filename=None,
@@ -510,16 +512,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1704,
-  serialized_end=1901,
+  serialized_start=1755,
+  serialized_end=1952,
 )
 
 
 _DEVICEDECOMMISSIONINGCONFIGSETREQUEST = _descriptor.Descriptor(
   name='DeviceDecommissioningConfigSetRequest',
   full_name='arista.inventory.v1.DeviceDecommissioningConfigSetRequest',
   filename=None,
@@ -542,16 +544,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=1903,
-  serialized_end=2007,
+  serialized_start=1954,
+  serialized_end=2058,
 )
 
 
 _DEVICEDECOMMISSIONINGCONFIGSETRESPONSE = _descriptor.Descriptor(
   name='DeviceDecommissioningConfigSetResponse',
   full_name='arista.inventory.v1.DeviceDecommissioningConfigSetResponse',
   filename=None,
@@ -581,16 +583,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2010,
-  serialized_end=2157,
+  serialized_start=2061,
+  serialized_end=2208,
 )
 
 
 _DEVICEDECOMMISSIONINGCONFIGDELETEREQUEST = _descriptor.Descriptor(
   name='DeviceDecommissioningConfigDeleteRequest',
   full_name='arista.inventory.v1.DeviceDecommissioningConfigDeleteRequest',
   filename=None,
@@ -613,16 +615,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2159,
-  serialized_end=2244,
+  serialized_start=2210,
+  serialized_end=2295,
 )
 
 
 _DEVICEDECOMMISSIONINGCONFIGDELETERESPONSE = _descriptor.Descriptor(
   name='DeviceDecommissioningConfigDeleteResponse',
   full_name='arista.inventory.v1.DeviceDecommissioningConfigDeleteResponse',
   filename=None,
@@ -652,16 +654,94 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2247,
-  serialized_end=2375,
+  serialized_start=2298,
+  serialized_end=2426,
+)
+
+
+_DEVICEDECOMMISSIONINGCONFIGDELETEALLREQUEST = _descriptor.Descriptor(
+  name='DeviceDecommissioningConfigDeleteAllRequest',
+  full_name='arista.inventory.v1.DeviceDecommissioningConfigDeleteAllRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2428,
+  serialized_end=2473,
+)
+
+
+_DEVICEDECOMMISSIONINGCONFIGDELETEALLRESPONSE = _descriptor.Descriptor(
+  name='DeviceDecommissioningConfigDeleteAllResponse',
+  full_name='arista.inventory.v1.DeviceDecommissioningConfigDeleteAllResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='arista.inventory.v1.DeviceDecommissioningConfigDeleteAllResponse.type', index=0,
+      number=1, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='error', full_name='arista.inventory.v1.DeviceDecommissioningConfigDeleteAllResponse.error', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='key', full_name='arista.inventory.v1.DeviceDecommissioningConfigDeleteAllResponse.key', index=2,
+      number=3, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='time', full_name='arista.inventory.v1.DeviceDecommissioningConfigDeleteAllResponse.time', index=3,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=2476,
+  serialized_end=2684,
 )
 
 
 _DEVICEONBOARDINGREQUEST = _descriptor.Descriptor(
   name='DeviceOnboardingRequest',
   full_name='arista.inventory.v1.DeviceOnboardingRequest',
   filename=None,
@@ -691,16 +771,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2377,
-  serialized_end=2487,
+  serialized_start=2686,
+  serialized_end=2796,
 )
 
 
 _DEVICEONBOARDINGRESPONSE = _descriptor.Descriptor(
   name='DeviceOnboardingResponse',
   full_name='arista.inventory.v1.DeviceOnboardingResponse',
   filename=None,
@@ -730,16 +810,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2489,
-  serialized_end=2611,
+  serialized_start=2798,
+  serialized_end=2920,
 )
 
 
 _DEVICEONBOARDINGSTREAMREQUEST = _descriptor.Descriptor(
   name='DeviceOnboardingStreamRequest',
   full_name='arista.inventory.v1.DeviceOnboardingStreamRequest',
   filename=None,
@@ -769,16 +849,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2614,
-  serialized_end=2750,
+  serialized_start=2923,
+  serialized_end=3059,
 )
 
 
 _DEVICEONBOARDINGSTREAMRESPONSE = _descriptor.Descriptor(
   name='DeviceOnboardingStreamResponse',
   full_name='arista.inventory.v1.DeviceOnboardingStreamResponse',
   filename=None,
@@ -815,16 +895,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2753,
-  serialized_end=2928,
+  serialized_start=3062,
+  serialized_end=3237,
 )
 
 
 _DEVICEONBOARDINGCONFIGREQUEST = _descriptor.Descriptor(
   name='DeviceOnboardingConfigRequest',
   full_name='arista.inventory.v1.DeviceOnboardingConfigRequest',
   filename=None,
@@ -854,16 +934,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=2930,
-  serialized_end=3046,
+  serialized_start=3239,
+  serialized_end=3355,
 )
 
 
 _DEVICEONBOARDINGCONFIGRESPONSE = _descriptor.Descriptor(
   name='DeviceOnboardingConfigResponse',
   full_name='arista.inventory.v1.DeviceOnboardingConfigResponse',
   filename=None,
@@ -893,16 +973,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3049,
-  serialized_end=3183,
+  serialized_start=3358,
+  serialized_end=3492,
 )
 
 
 _DEVICEONBOARDINGCONFIGSTREAMREQUEST = _descriptor.Descriptor(
   name='DeviceOnboardingConfigStreamRequest',
   full_name='arista.inventory.v1.DeviceOnboardingConfigStreamRequest',
   filename=None,
@@ -932,16 +1012,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3186,
-  serialized_end=3334,
+  serialized_start=3495,
+  serialized_end=3643,
 )
 
 
 _DEVICEONBOARDINGCONFIGSTREAMRESPONSE = _descriptor.Descriptor(
   name='DeviceOnboardingConfigStreamResponse',
   full_name='arista.inventory.v1.DeviceOnboardingConfigStreamResponse',
   filename=None,
@@ -978,16 +1058,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3337,
-  serialized_end=3524,
+  serialized_start=3646,
+  serialized_end=3833,
 )
 
 
 _DEVICEONBOARDINGCONFIGSETREQUEST = _descriptor.Descriptor(
   name='DeviceOnboardingConfigSetRequest',
   full_name='arista.inventory.v1.DeviceOnboardingConfigSetRequest',
   filename=None,
@@ -1010,16 +1090,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3526,
-  serialized_end=3620,
+  serialized_start=3835,
+  serialized_end=3929,
 )
 
 
 _DEVICEONBOARDINGCONFIGSETRESPONSE = _descriptor.Descriptor(
   name='DeviceOnboardingConfigSetResponse',
   full_name='arista.inventory.v1.DeviceOnboardingConfigSetResponse',
   filename=None,
@@ -1049,16 +1129,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3623,
-  serialized_end=3760,
+  serialized_start=3932,
+  serialized_end=4069,
 )
 
 
 _DEVICEONBOARDINGCONFIGDELETEREQUEST = _descriptor.Descriptor(
   name='DeviceOnboardingConfigDeleteRequest',
   full_name='arista.inventory.v1.DeviceOnboardingConfigDeleteRequest',
   filename=None,
@@ -1081,16 +1161,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3762,
-  serialized_end=3842,
+  serialized_start=4071,
+  serialized_end=4151,
 )
 
 
 _DEVICEONBOARDINGCONFIGDELETERESPONSE = _descriptor.Descriptor(
   name='DeviceOnboardingConfigDeleteResponse',
   full_name='arista.inventory.v1.DeviceOnboardingConfigDeleteResponse',
   filename=None,
@@ -1120,16 +1200,94 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3844,
-  serialized_end=3967,
+  serialized_start=4153,
+  serialized_end=4276,
+)
+
+
+_DEVICEONBOARDINGCONFIGDELETEALLREQUEST = _descriptor.Descriptor(
+  name='DeviceOnboardingConfigDeleteAllRequest',
+  full_name='arista.inventory.v1.DeviceOnboardingConfigDeleteAllRequest',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=4278,
+  serialized_end=4318,
+)
+
+
+_DEVICEONBOARDINGCONFIGDELETEALLRESPONSE = _descriptor.Descriptor(
+  name='DeviceOnboardingConfigDeleteAllResponse',
+  full_name='arista.inventory.v1.DeviceOnboardingConfigDeleteAllResponse',
+  filename=None,
+  file=DESCRIPTOR,
+  containing_type=None,
+  create_key=_descriptor._internal_create_key,
+  fields=[
+    _descriptor.FieldDescriptor(
+      name='type', full_name='arista.inventory.v1.DeviceOnboardingConfigDeleteAllResponse.type', index=0,
+      number=1, type=14, cpp_type=8, label=1,
+      has_default_value=False, default_value=0,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='error', full_name='arista.inventory.v1.DeviceOnboardingConfigDeleteAllResponse.error', index=1,
+      number=2, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='key', full_name='arista.inventory.v1.DeviceOnboardingConfigDeleteAllResponse.key', index=2,
+      number=3, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+    _descriptor.FieldDescriptor(
+      name='time', full_name='arista.inventory.v1.DeviceOnboardingConfigDeleteAllResponse.time', index=3,
+      number=4, type=11, cpp_type=10, label=1,
+      has_default_value=False, default_value=None,
+      message_type=None, enum_type=None, containing_type=None,
+      is_extension=False, extension_scope=None,
+      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
+  ],
+  extensions=[
+  ],
+  nested_types=[],
+  enum_types=[
+  ],
+  serialized_options=None,
+  is_extendable=False,
+  syntax='proto3',
+  extension_ranges=[],
+  oneofs=[
+  ],
+  serialized_start=4321,
+  serialized_end=4524,
 )
 
 
 _PROVISIONEDDEVICEREQUEST = _descriptor.Descriptor(
   name='ProvisionedDeviceRequest',
   full_name='arista.inventory.v1.ProvisionedDeviceRequest',
   filename=None,
@@ -1159,16 +1317,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=3969,
-  serialized_end=4082,
+  serialized_start=4526,
+  serialized_end=4639,
 )
 
 
 _PROVISIONEDDEVICERESPONSE = _descriptor.Descriptor(
   name='ProvisionedDeviceResponse',
   full_name='arista.inventory.v1.ProvisionedDeviceResponse',
   filename=None,
@@ -1198,16 +1356,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4084,
-  serialized_end=4208,
+  serialized_start=4641,
+  serialized_end=4765,
 )
 
 
 _PROVISIONEDDEVICESTREAMREQUEST = _descriptor.Descriptor(
   name='ProvisionedDeviceStreamRequest',
   full_name='arista.inventory.v1.ProvisionedDeviceStreamRequest',
   filename=None,
@@ -1237,16 +1395,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4211,
-  serialized_end=4349,
+  serialized_start=4768,
+  serialized_end=4906,
 )
 
 
 _PROVISIONEDDEVICESTREAMRESPONSE = _descriptor.Descriptor(
   name='ProvisionedDeviceStreamResponse',
   full_name='arista.inventory.v1.ProvisionedDeviceStreamResponse',
   filename=None,
@@ -1283,16 +1441,16 @@
   ],
   serialized_options=None,
   is_extendable=False,
   syntax='proto3',
   extension_ranges=[],
   oneofs=[
   ],
-  serialized_start=4352,
-  serialized_end=4529,
+  serialized_start=4909,
+  serialized_end=5086,
 )
 
 _DEVICEREQUEST.fields_by_name['key'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._DEVICEKEY
 _DEVICEREQUEST.fields_by_name['time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _DEVICERESPONSE.fields_by_name['value'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._DEVICE
 _DEVICERESPONSE.fields_by_name['time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _DEVICESTREAMREQUEST.fields_by_name['partial_eq_filter'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._DEVICE
@@ -1320,14 +1478,18 @@
 _DEVICEDECOMMISSIONINGCONFIGSTREAMRESPONSE.fields_by_name['type'].enum_type = arista_dot_subscriptions_dot_subscriptions__pb2._OPERATION
 _DEVICEDECOMMISSIONINGCONFIGSETREQUEST.fields_by_name['value'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._DEVICEDECOMMISSIONINGCONFIG
 _DEVICEDECOMMISSIONINGCONFIGSETRESPONSE.fields_by_name['value'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._DEVICEDECOMMISSIONINGCONFIG
 _DEVICEDECOMMISSIONINGCONFIGSETRESPONSE.fields_by_name['time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _DEVICEDECOMMISSIONINGCONFIGDELETEREQUEST.fields_by_name['key'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._UUIDKEY
 _DEVICEDECOMMISSIONINGCONFIGDELETERESPONSE.fields_by_name['key'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._UUIDKEY
 _DEVICEDECOMMISSIONINGCONFIGDELETERESPONSE.fields_by_name['time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
+_DEVICEDECOMMISSIONINGCONFIGDELETEALLRESPONSE.fields_by_name['type'].enum_type = fmp_dot_deletes__pb2._DELETEERROR
+_DEVICEDECOMMISSIONINGCONFIGDELETEALLRESPONSE.fields_by_name['error'].message_type = google_dot_protobuf_dot_wrappers__pb2._STRINGVALUE
+_DEVICEDECOMMISSIONINGCONFIGDELETEALLRESPONSE.fields_by_name['key'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._UUIDKEY
+_DEVICEDECOMMISSIONINGCONFIGDELETEALLRESPONSE.fields_by_name['time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _DEVICEONBOARDINGREQUEST.fields_by_name['key'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._UUIDKEY
 _DEVICEONBOARDINGREQUEST.fields_by_name['time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _DEVICEONBOARDINGRESPONSE.fields_by_name['value'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._DEVICEONBOARDING
 _DEVICEONBOARDINGRESPONSE.fields_by_name['time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _DEVICEONBOARDINGSTREAMREQUEST.fields_by_name['partial_eq_filter'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._DEVICEONBOARDING
 _DEVICEONBOARDINGSTREAMREQUEST.fields_by_name['time'].message_type = arista_dot_time_dot_time__pb2._TIMEBOUNDS
 _DEVICEONBOARDINGSTREAMRESPONSE.fields_by_name['value'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._DEVICEONBOARDING
@@ -1344,14 +1506,18 @@
 _DEVICEONBOARDINGCONFIGSTREAMRESPONSE.fields_by_name['type'].enum_type = arista_dot_subscriptions_dot_subscriptions__pb2._OPERATION
 _DEVICEONBOARDINGCONFIGSETREQUEST.fields_by_name['value'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._DEVICEONBOARDINGCONFIG
 _DEVICEONBOARDINGCONFIGSETRESPONSE.fields_by_name['value'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._DEVICEONBOARDINGCONFIG
 _DEVICEONBOARDINGCONFIGSETRESPONSE.fields_by_name['time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _DEVICEONBOARDINGCONFIGDELETEREQUEST.fields_by_name['key'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._UUIDKEY
 _DEVICEONBOARDINGCONFIGDELETERESPONSE.fields_by_name['key'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._UUIDKEY
 _DEVICEONBOARDINGCONFIGDELETERESPONSE.fields_by_name['time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
+_DEVICEONBOARDINGCONFIGDELETEALLRESPONSE.fields_by_name['type'].enum_type = fmp_dot_deletes__pb2._DELETEERROR
+_DEVICEONBOARDINGCONFIGDELETEALLRESPONSE.fields_by_name['error'].message_type = google_dot_protobuf_dot_wrappers__pb2._STRINGVALUE
+_DEVICEONBOARDINGCONFIGDELETEALLRESPONSE.fields_by_name['key'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._UUIDKEY
+_DEVICEONBOARDINGCONFIGDELETEALLRESPONSE.fields_by_name['time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _PROVISIONEDDEVICEREQUEST.fields_by_name['key'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._DEVICEKEY
 _PROVISIONEDDEVICEREQUEST.fields_by_name['time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _PROVISIONEDDEVICERESPONSE.fields_by_name['value'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._PROVISIONEDDEVICE
 _PROVISIONEDDEVICERESPONSE.fields_by_name['time'].message_type = google_dot_protobuf_dot_timestamp__pb2._TIMESTAMP
 _PROVISIONEDDEVICESTREAMREQUEST.fields_by_name['partial_eq_filter'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._PROVISIONEDDEVICE
 _PROVISIONEDDEVICESTREAMREQUEST.fields_by_name['time'].message_type = arista_dot_time_dot_time__pb2._TIMEBOUNDS
 _PROVISIONEDDEVICESTREAMRESPONSE.fields_by_name['value'].message_type = arista_dot_inventory_dot_v1_dot_inventory__pb2._PROVISIONEDDEVICE
@@ -1369,26 +1535,30 @@
 DESCRIPTOR.message_types_by_name['DeviceDecommissioningConfigResponse'] = _DEVICEDECOMMISSIONINGCONFIGRESPONSE
 DESCRIPTOR.message_types_by_name['DeviceDecommissioningConfigStreamRequest'] = _DEVICEDECOMMISSIONINGCONFIGSTREAMREQUEST
 DESCRIPTOR.message_types_by_name['DeviceDecommissioningConfigStreamResponse'] = _DEVICEDECOMMISSIONINGCONFIGSTREAMRESPONSE
 DESCRIPTOR.message_types_by_name['DeviceDecommissioningConfigSetRequest'] = _DEVICEDECOMMISSIONINGCONFIGSETREQUEST
 DESCRIPTOR.message_types_by_name['DeviceDecommissioningConfigSetResponse'] = _DEVICEDECOMMISSIONINGCONFIGSETRESPONSE
 DESCRIPTOR.message_types_by_name['DeviceDecommissioningConfigDeleteRequest'] = _DEVICEDECOMMISSIONINGCONFIGDELETEREQUEST
 DESCRIPTOR.message_types_by_name['DeviceDecommissioningConfigDeleteResponse'] = _DEVICEDECOMMISSIONINGCONFIGDELETERESPONSE
+DESCRIPTOR.message_types_by_name['DeviceDecommissioningConfigDeleteAllRequest'] = _DEVICEDECOMMISSIONINGCONFIGDELETEALLREQUEST
+DESCRIPTOR.message_types_by_name['DeviceDecommissioningConfigDeleteAllResponse'] = _DEVICEDECOMMISSIONINGCONFIGDELETEALLRESPONSE
 DESCRIPTOR.message_types_by_name['DeviceOnboardingRequest'] = _DEVICEONBOARDINGREQUEST
 DESCRIPTOR.message_types_by_name['DeviceOnboardingResponse'] = _DEVICEONBOARDINGRESPONSE
 DESCRIPTOR.message_types_by_name['DeviceOnboardingStreamRequest'] = _DEVICEONBOARDINGSTREAMREQUEST
 DESCRIPTOR.message_types_by_name['DeviceOnboardingStreamResponse'] = _DEVICEONBOARDINGSTREAMRESPONSE
 DESCRIPTOR.message_types_by_name['DeviceOnboardingConfigRequest'] = _DEVICEONBOARDINGCONFIGREQUEST
 DESCRIPTOR.message_types_by_name['DeviceOnboardingConfigResponse'] = _DEVICEONBOARDINGCONFIGRESPONSE
 DESCRIPTOR.message_types_by_name['DeviceOnboardingConfigStreamRequest'] = _DEVICEONBOARDINGCONFIGSTREAMREQUEST
 DESCRIPTOR.message_types_by_name['DeviceOnboardingConfigStreamResponse'] = _DEVICEONBOARDINGCONFIGSTREAMRESPONSE
 DESCRIPTOR.message_types_by_name['DeviceOnboardingConfigSetRequest'] = _DEVICEONBOARDINGCONFIGSETREQUEST
 DESCRIPTOR.message_types_by_name['DeviceOnboardingConfigSetResponse'] = _DEVICEONBOARDINGCONFIGSETRESPONSE
 DESCRIPTOR.message_types_by_name['DeviceOnboardingConfigDeleteRequest'] = _DEVICEONBOARDINGCONFIGDELETEREQUEST
 DESCRIPTOR.message_types_by_name['DeviceOnboardingConfigDeleteResponse'] = _DEVICEONBOARDINGCONFIGDELETERESPONSE
+DESCRIPTOR.message_types_by_name['DeviceOnboardingConfigDeleteAllRequest'] = _DEVICEONBOARDINGCONFIGDELETEALLREQUEST
+DESCRIPTOR.message_types_by_name['DeviceOnboardingConfigDeleteAllResponse'] = _DEVICEONBOARDINGCONFIGDELETEALLRESPONSE
 DESCRIPTOR.message_types_by_name['ProvisionedDeviceRequest'] = _PROVISIONEDDEVICEREQUEST
 DESCRIPTOR.message_types_by_name['ProvisionedDeviceResponse'] = _PROVISIONEDDEVICERESPONSE
 DESCRIPTOR.message_types_by_name['ProvisionedDeviceStreamRequest'] = _PROVISIONEDDEVICESTREAMREQUEST
 DESCRIPTOR.message_types_by_name['ProvisionedDeviceStreamResponse'] = _PROVISIONEDDEVICESTREAMRESPONSE
 _sym_db.RegisterFileDescriptor(DESCRIPTOR)
 
 DeviceRequest = _reflection.GeneratedProtocolMessageType('DeviceRequest', (_message.Message,), {
@@ -1499,14 +1669,28 @@
 DeviceDecommissioningConfigDeleteResponse = _reflection.GeneratedProtocolMessageType('DeviceDecommissioningConfigDeleteResponse', (_message.Message,), {
   'DESCRIPTOR' : _DEVICEDECOMMISSIONINGCONFIGDELETERESPONSE,
   '__module__' : 'arista.inventory.v1.services.gen_pb2'
   # @@protoc_insertion_point(class_scope:arista.inventory.v1.DeviceDecommissioningConfigDeleteResponse)
   })
 _sym_db.RegisterMessage(DeviceDecommissioningConfigDeleteResponse)
 
+DeviceDecommissioningConfigDeleteAllRequest = _reflection.GeneratedProtocolMessageType('DeviceDecommissioningConfigDeleteAllRequest', (_message.Message,), {
+  'DESCRIPTOR' : _DEVICEDECOMMISSIONINGCONFIGDELETEALLREQUEST,
+  '__module__' : 'arista.inventory.v1.services.gen_pb2'
+  # @@protoc_insertion_point(class_scope:arista.inventory.v1.DeviceDecommissioningConfigDeleteAllRequest)
+  })
+_sym_db.RegisterMessage(DeviceDecommissioningConfigDeleteAllRequest)
+
+DeviceDecommissioningConfigDeleteAllResponse = _reflection.GeneratedProtocolMessageType('DeviceDecommissioningConfigDeleteAllResponse', (_message.Message,), {
+  'DESCRIPTOR' : _DEVICEDECOMMISSIONINGCONFIGDELETEALLRESPONSE,
+  '__module__' : 'arista.inventory.v1.services.gen_pb2'
+  # @@protoc_insertion_point(class_scope:arista.inventory.v1.DeviceDecommissioningConfigDeleteAllResponse)
+  })
+_sym_db.RegisterMessage(DeviceDecommissioningConfigDeleteAllResponse)
+
 DeviceOnboardingRequest = _reflection.GeneratedProtocolMessageType('DeviceOnboardingRequest', (_message.Message,), {
   'DESCRIPTOR' : _DEVICEONBOARDINGREQUEST,
   '__module__' : 'arista.inventory.v1.services.gen_pb2'
   # @@protoc_insertion_point(class_scope:arista.inventory.v1.DeviceOnboardingRequest)
   })
 _sym_db.RegisterMessage(DeviceOnboardingRequest)
 
@@ -1583,14 +1767,28 @@
 DeviceOnboardingConfigDeleteResponse = _reflection.GeneratedProtocolMessageType('DeviceOnboardingConfigDeleteResponse', (_message.Message,), {
   'DESCRIPTOR' : _DEVICEONBOARDINGCONFIGDELETERESPONSE,
   '__module__' : 'arista.inventory.v1.services.gen_pb2'
   # @@protoc_insertion_point(class_scope:arista.inventory.v1.DeviceOnboardingConfigDeleteResponse)
   })
 _sym_db.RegisterMessage(DeviceOnboardingConfigDeleteResponse)
 
+DeviceOnboardingConfigDeleteAllRequest = _reflection.GeneratedProtocolMessageType('DeviceOnboardingConfigDeleteAllRequest', (_message.Message,), {
+  'DESCRIPTOR' : _DEVICEONBOARDINGCONFIGDELETEALLREQUEST,
+  '__module__' : 'arista.inventory.v1.services.gen_pb2'
+  # @@protoc_insertion_point(class_scope:arista.inventory.v1.DeviceOnboardingConfigDeleteAllRequest)
+  })
+_sym_db.RegisterMessage(DeviceOnboardingConfigDeleteAllRequest)
+
+DeviceOnboardingConfigDeleteAllResponse = _reflection.GeneratedProtocolMessageType('DeviceOnboardingConfigDeleteAllResponse', (_message.Message,), {
+  'DESCRIPTOR' : _DEVICEONBOARDINGCONFIGDELETEALLRESPONSE,
+  '__module__' : 'arista.inventory.v1.services.gen_pb2'
+  # @@protoc_insertion_point(class_scope:arista.inventory.v1.DeviceOnboardingConfigDeleteAllResponse)
+  })
+_sym_db.RegisterMessage(DeviceOnboardingConfigDeleteAllResponse)
+
 ProvisionedDeviceRequest = _reflection.GeneratedProtocolMessageType('ProvisionedDeviceRequest', (_message.Message,), {
   'DESCRIPTOR' : _PROVISIONEDDEVICEREQUEST,
   '__module__' : 'arista.inventory.v1.services.gen_pb2'
   # @@protoc_insertion_point(class_scope:arista.inventory.v1.ProvisionedDeviceRequest)
   })
 _sym_db.RegisterMessage(ProvisionedDeviceRequest)
 
@@ -1621,16 +1819,16 @@
 _DEVICESERVICE = _descriptor.ServiceDescriptor(
   name='DeviceService',
   full_name='arista.inventory.v1.DeviceService',
   file=DESCRIPTOR,
   index=0,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=4532,
-  serialized_end=4827,
+  serialized_start=5089,
+  serialized_end=5384,
   methods=[
   _descriptor.MethodDescriptor(
     name='GetOne',
     full_name='arista.inventory.v1.DeviceService.GetOne',
     index=0,
     containing_service=None,
     input_type=_DEVICEREQUEST,
@@ -1667,16 +1865,16 @@
 _DEVICEDECOMMISSIONINGSERVICE = _descriptor.ServiceDescriptor(
   name='DeviceDecommissioningService',
   full_name='arista.inventory.v1.DeviceDecommissioningService',
   file=DESCRIPTOR,
   index=1,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=4830,
-  serialized_end=5231,
+  serialized_start=5387,
+  serialized_end=5788,
   methods=[
   _descriptor.MethodDescriptor(
     name='GetOne',
     full_name='arista.inventory.v1.DeviceDecommissioningService.GetOne',
     index=0,
     containing_service=None,
     input_type=_DEVICEDECOMMISSIONINGREQUEST,
@@ -1713,16 +1911,16 @@
 _DEVICEDECOMMISSIONINGCONFIGSERVICE = _descriptor.ServiceDescriptor(
   name='DeviceDecommissioningConfigService',
   full_name='arista.inventory.v1.DeviceDecommissioningConfigService',
   file=DESCRIPTOR,
   index=2,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=5234,
-  serialized_end=5944,
+  serialized_start=5791,
+  serialized_end=6650,
   methods=[
   _descriptor.MethodDescriptor(
     name='GetOne',
     full_name='arista.inventory.v1.DeviceDecommissioningConfigService.GetOne',
     index=0,
     containing_service=None,
     input_type=_DEVICEDECOMMISSIONINGCONFIGREQUEST,
@@ -1766,29 +1964,39 @@
     index=4,
     containing_service=None,
     input_type=_DEVICEDECOMMISSIONINGCONFIGDELETEREQUEST,
     output_type=_DEVICEDECOMMISSIONINGCONFIGDELETERESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
+  _descriptor.MethodDescriptor(
+    name='DeleteAll',
+    full_name='arista.inventory.v1.DeviceDecommissioningConfigService.DeleteAll',
+    index=5,
+    containing_service=None,
+    input_type=_DEVICEDECOMMISSIONINGCONFIGDELETEALLREQUEST,
+    output_type=_DEVICEDECOMMISSIONINGCONFIGDELETEALLRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
 ])
 _sym_db.RegisterServiceDescriptor(_DEVICEDECOMMISSIONINGCONFIGSERVICE)
 
 DESCRIPTOR.services_by_name['DeviceDecommissioningConfigService'] = _DEVICEDECOMMISSIONINGCONFIGSERVICE
 
 
 _DEVICEONBOARDINGSERVICE = _descriptor.ServiceDescriptor(
   name='DeviceOnboardingService',
   full_name='arista.inventory.v1.DeviceOnboardingService',
   file=DESCRIPTOR,
   index=3,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=5947,
-  serialized_end=6312,
+  serialized_start=6653,
+  serialized_end=7018,
   methods=[
   _descriptor.MethodDescriptor(
     name='GetOne',
     full_name='arista.inventory.v1.DeviceOnboardingService.GetOne',
     index=0,
     containing_service=None,
     input_type=_DEVICEONBOARDINGREQUEST,
@@ -1825,16 +2033,16 @@
 _DEVICEONBOARDINGCONFIGSERVICE = _descriptor.ServiceDescriptor(
   name='DeviceOnboardingConfigService',
   full_name='arista.inventory.v1.DeviceOnboardingConfigService',
   file=DESCRIPTOR,
   index=4,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=6315,
-  serialized_end=6968,
+  serialized_start=7021,
+  serialized_end=7813,
   methods=[
   _descriptor.MethodDescriptor(
     name='GetOne',
     full_name='arista.inventory.v1.DeviceOnboardingConfigService.GetOne',
     index=0,
     containing_service=None,
     input_type=_DEVICEONBOARDINGCONFIGREQUEST,
@@ -1878,29 +2086,39 @@
     index=4,
     containing_service=None,
     input_type=_DEVICEONBOARDINGCONFIGDELETEREQUEST,
     output_type=_DEVICEONBOARDINGCONFIGDELETERESPONSE,
     serialized_options=None,
     create_key=_descriptor._internal_create_key,
   ),
+  _descriptor.MethodDescriptor(
+    name='DeleteAll',
+    full_name='arista.inventory.v1.DeviceOnboardingConfigService.DeleteAll',
+    index=5,
+    containing_service=None,
+    input_type=_DEVICEONBOARDINGCONFIGDELETEALLREQUEST,
+    output_type=_DEVICEONBOARDINGCONFIGDELETEALLRESPONSE,
+    serialized_options=None,
+    create_key=_descriptor._internal_create_key,
+  ),
 ])
 _sym_db.RegisterServiceDescriptor(_DEVICEONBOARDINGCONFIGSERVICE)
 
 DESCRIPTOR.services_by_name['DeviceOnboardingConfigService'] = _DEVICEONBOARDINGCONFIGSERVICE
 
 
 _PROVISIONEDDEVICESERVICE = _descriptor.ServiceDescriptor(
   name='ProvisionedDeviceService',
   full_name='arista.inventory.v1.ProvisionedDeviceService',
   file=DESCRIPTOR,
   index=5,
   serialized_options=None,
   create_key=_descriptor._internal_create_key,
-  serialized_start=6971,
-  serialized_end=7343,
+  serialized_start=7816,
+  serialized_end=8188,
   methods=[
   _descriptor.MethodDescriptor(
     name='GetOne',
     full_name='arista.inventory.v1.ProvisionedDeviceService.GetOne',
     index=0,
     containing_service=None,
     input_type=_PROVISIONEDDEVICEREQUEST,
```

### Comparing `cloudvision-1.9.0/arista/inventory/v1/services/gen_pb2_grpc.py` & `cloudvision-1.9.1/arista/inventory/v1/services/gen_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,14 +289,19 @@
                 response_deserializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigSetResponse.FromString,
                 )
         self.Delete = channel.unary_unary(
                 '/arista.inventory.v1.DeviceDecommissioningConfigService/Delete',
                 request_serializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigDeleteRequest.SerializeToString,
                 response_deserializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigDeleteResponse.FromString,
                 )
+        self.DeleteAll = channel.unary_stream(
+                '/arista.inventory.v1.DeviceDecommissioningConfigService/DeleteAll',
+                request_serializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigDeleteAllRequest.SerializeToString,
+                response_deserializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigDeleteAllResponse.FromString,
+                )
 
 
 class DeviceDecommissioningConfigServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def GetOne(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -324,14 +329,20 @@
 
     def Delete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def DeleteAll(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_DeviceDecommissioningConfigServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetOne': grpc.unary_unary_rpc_method_handler(
                     servicer.GetOne,
                     request_deserializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigRequest.FromString,
                     response_serializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigResponse.SerializeToString,
@@ -352,14 +363,19 @@
                     response_serializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigSetResponse.SerializeToString,
             ),
             'Delete': grpc.unary_unary_rpc_method_handler(
                     servicer.Delete,
                     request_deserializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigDeleteRequest.FromString,
                     response_serializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigDeleteResponse.SerializeToString,
             ),
+            'DeleteAll': grpc.unary_stream_rpc_method_handler(
+                    servicer.DeleteAll,
+                    request_deserializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigDeleteAllRequest.FromString,
+                    response_serializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigDeleteAllResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'arista.inventory.v1.DeviceDecommissioningConfigService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -447,14 +463,31 @@
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/arista.inventory.v1.DeviceDecommissioningConfigService/Delete',
             arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigDeleteRequest.SerializeToString,
             arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigDeleteResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
+    @staticmethod
+    def DeleteAll(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/arista.inventory.v1.DeviceDecommissioningConfigService/DeleteAll',
+            arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigDeleteAllRequest.SerializeToString,
+            arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceDecommissioningConfigDeleteAllResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
 
 class DeviceOnboardingServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
 
@@ -609,14 +642,19 @@
                 response_deserializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigSetResponse.FromString,
                 )
         self.Delete = channel.unary_unary(
                 '/arista.inventory.v1.DeviceOnboardingConfigService/Delete',
                 request_serializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigDeleteRequest.SerializeToString,
                 response_deserializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigDeleteResponse.FromString,
                 )
+        self.DeleteAll = channel.unary_stream(
+                '/arista.inventory.v1.DeviceOnboardingConfigService/DeleteAll',
+                request_serializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigDeleteAllRequest.SerializeToString,
+                response_deserializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigDeleteAllResponse.FromString,
+                )
 
 
 class DeviceOnboardingConfigServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def GetOne(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -644,14 +682,20 @@
 
     def Delete(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def DeleteAll(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_DeviceOnboardingConfigServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'GetOne': grpc.unary_unary_rpc_method_handler(
                     servicer.GetOne,
                     request_deserializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigRequest.FromString,
                     response_serializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigResponse.SerializeToString,
@@ -672,14 +716,19 @@
                     response_serializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigSetResponse.SerializeToString,
             ),
             'Delete': grpc.unary_unary_rpc_method_handler(
                     servicer.Delete,
                     request_deserializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigDeleteRequest.FromString,
                     response_serializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigDeleteResponse.SerializeToString,
             ),
+            'DeleteAll': grpc.unary_stream_rpc_method_handler(
+                    servicer.DeleteAll,
+                    request_deserializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigDeleteAllRequest.FromString,
+                    response_serializer=arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigDeleteAllResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'arista.inventory.v1.DeviceOnboardingConfigService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -767,14 +816,31 @@
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/arista.inventory.v1.DeviceOnboardingConfigService/Delete',
             arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigDeleteRequest.SerializeToString,
             arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigDeleteResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
+    @staticmethod
+    def DeleteAll(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_stream(request, target, '/arista.inventory.v1.DeviceOnboardingConfigService/DeleteAll',
+            arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigDeleteAllRequest.SerializeToString,
+            arista_dot_inventory_dot_v1_dot_services_dot_gen__pb2.DeviceOnboardingConfigDeleteAllResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
 
 class ProvisionedDeviceServiceStub(object):
     """Missing associated documentation comment in .proto file."""
 
     def __init__(self, channel):
         """Constructor.
```

### Comparing `cloudvision-1.9.0/arista/redirector/v1/redirector_pb2.py` & `cloudvision-1.9.1/arista/redirector/v1/redirector_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/redirector/v1/services/gen_pb2.py` & `cloudvision-1.9.1/arista/redirector/v1/services/gen_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/redirector/v1/services/gen_pb2_grpc.py` & `cloudvision-1.9.1/arista/redirector/v1/services/gen_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/studio/v1/services/gen_pb2.py` & `cloudvision-1.9.1/arista/studio/v1/services/gen_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/studio/v1/services/gen_pb2_grpc.py` & `cloudvision-1.9.1/arista/studio/v1/services/gen_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/studio/v1/studio_pb2.py` & `cloudvision-1.9.1/arista/studio/v1/studio_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/subscriptions/subscriptions_pb2.py` & `cloudvision-1.9.1/arista/subscriptions/subscriptions_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/tag/v1/services/gen_pb2.py` & `cloudvision-1.9.1/arista/tag/v1/services/gen_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/tag/v1/services/gen_pb2_grpc.py` & `cloudvision-1.9.1/arista/tag/v1/services/gen_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/tag/v1/tag_pb2.py` & `cloudvision-1.9.1/arista/tag/v1/tag_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/tag/v2/services/gen_pb2.py` & `cloudvision-1.9.1/arista/tag/v2/services/gen_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/tag/v2/services/gen_pb2_grpc.py` & `cloudvision-1.9.1/arista/tag/v2/services/gen_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/tag/v2/tag_pb2.py` & `cloudvision-1.9.1/arista/tag/v2/tag_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/time/time_pb2.py` & `cloudvision-1.9.1/arista/time/time_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/workspace/v1/services/gen_pb2.py` & `cloudvision-1.9.1/arista/workspace/v1/services/gen_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/workspace/v1/services/gen_pb2_grpc.py` & `cloudvision-1.9.1/arista/workspace/v1/services/gen_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/arista/workspace/v1/workspace_pb2.py` & `cloudvision-1.9.1/arista/workspace/v1/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/Connector/__init__.py` & `cloudvision-1.9.1/cloudvision/Connector/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/Connector/auth/cert.py` & `cloudvision-1.9.1/cloudvision/Connector/auth/cert.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/Connector/codec/custom_types.py` & `cloudvision-1.9.1/cloudvision/Connector/codec/custom_types.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/Connector/codec/decoder.py` & `cloudvision-1.9.1/cloudvision/Connector/codec/decoder.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/Connector/codec/encoder.py` & `cloudvision-1.9.1/cloudvision/Connector/codec/encoder.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/Connector/core/utils.py` & `cloudvision-1.9.1/cloudvision/Connector/core/utils.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/Connector/gen/ca_pb2.py` & `cloudvision-1.9.1/cloudvision/Connector/gen/ca_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/Connector/gen/ca_pb2_grpc.py` & `cloudvision-1.9.1/cloudvision/Connector/gen/ca_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/Connector/gen/notification_pb2.py` & `cloudvision-1.9.1/cloudvision/Connector/gen/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/Connector/gen/router_pb2.py` & `cloudvision-1.9.1/cloudvision/Connector/gen/router_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/Connector/gen/router_pb2_grpc.py` & `cloudvision-1.9.1/cloudvision/Connector/gen/router_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/Connector/gen/sharding_pb2.py` & `cloudvision-1.9.1/cloudvision/Connector/gen/sharding_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/Connector/grpc_client/grpcClient.py` & `cloudvision-1.9.1/cloudvision/Connector/grpc_client/grpcClient.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,16 @@
     # An empty list would mean deleteAll so distinguish z/w empty and None
     dels = None
     if deletes is not None:
         dels = [encoder.encode(d) for d in deletes]
 
     upds = None
     if updates is not None:
-        upds = [ntf.Notification.Update(key=encoder.encode(k), value=encoder.encode(v)) for k, v in updates]
+        upds = [ntf.Notification.Update(key=encoder.encode(k),
+                                        value=encoder.encode(v)) for k, v in updates]
     rets = None
     if retracts is not None:
         rets = [encoder.encode(r) for r in retracts]
 
     pathElts = [encoder.encode(elt) for elt in paths]
     return ntf.Notification(
         timestamp=proto_ts,
@@ -326,15 +327,16 @@
         }
         return res
 
     def decode_notification(self, notif):
         res = {
             "timestamp": notif.timestamp,
             "deletes": [self.decoder.decode(d) for d in notif.deletes],
-            "updates": {self.decoder.decode(u.key): self.decoder.decode(u.value) for u in notif.updates},
+            "updates": {self.decoder.decode(u.key):
+                        self.decoder.decode(u.value) for u in notif.updates},
             "retracts": [self.decoder.decode(r) for r in notif.retracts],
             "path_elements": [self.decoder.decode(elt) for elt in notif.path_elements],
         }
         return res
 
     def search(
         self,
```

### Comparing `cloudvision-1.9.0/cloudvision/cvlib/__init__.py` & `cloudvision-1.9.1/cloudvision/cvlib/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/cvlib/action.py` & `cloudvision-1.9.1/cloudvision/cvlib/action.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/cvlib/changecontrol.py` & `cloudvision-1.9.1/cloudvision/cvlib/changecontrol.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/cvlib/connections.py` & `cloudvision-1.9.1/cloudvision/cvlib/connections.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,16 @@
             '_ClientCallDetails',
             ('method', 'timeout', 'metadata', 'credentials')),
         grpc.ClientCallDetails):
     pass
 
 
 def addHeaderInterceptor(header, value):
-    def intercept_call(client_call_details, request_iterator, request_streaming, response_streaming):
+    def intercept_call(client_call_details, request_iterator, request_streaming,
+                       response_streaming):
         metadata = []
         if client_call_details.metadata is not None:
             metadata = list(client_call_details.metadata)
         metadata.append((
             header,
             value,
         ))
```

### Comparing `cloudvision-1.9.0/cloudvision/cvlib/context.py` & `cloudvision-1.9.1/cloudvision/cvlib/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,15 +330,16 @@
         exception if it runs longer than <timeout>
         '''
 
         # A handler function for the timer that will raise our custom exception
         def monitorTimerHandler(signum, frame):
             raise TimeoutExpiry
 
-        # Set up a signal handler that will cause a signal.SIGALRM signal to trigger our timer handler
+        # Set up a signal handler that will cause a signal.SIGALRM signal to trigger our timer
+        # handler
         signal.signal(signal.SIGALRM, monitorTimerHandler)
         # Set an alarm to fire in <timeout> seconds. This will call the handler we bound earlier
         signal.alarm(timeout)
 
         try:
             return f()
         finally:
```

### Comparing `cloudvision-1.9.0/cloudvision/cvlib/device.py` & `cloudvision-1.9.1/cloudvision/cvlib/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,16 @@
         '''
         getInterfaces returns a dictionary list of the interfaces assigned to the Device object
         '''
         return self._interfaces.values()
 
     def getInterface(self, name):
         '''
-        getInterface gets a particular named interface from the interfaces assigned to the Device object
+        getInterface gets a particular named interface from the interfaces assigned to the Device
+        object
         '''
         return self._interfaces.get(name)
 
     def addInterface(self, name: str):
         '''
         addInterface assigns an interface to the Device object
         '''
```

### Comparing `cloudvision-1.9.0/cloudvision/cvlib/exceptions.py` & `cloudvision-1.9.1/cloudvision/cvlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/cvlib/logger.py` & `cloudvision-1.9.1/cloudvision/cvlib/logger.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision/cvlib/studio.py` & `cloudvision-1.9.1/cloudvision/cvlib/studio.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,16 @@
     )
     try:
         client.Set(request=req)
     except Exception as e:
         raise InputUpdateException(inputPath, f"Value {value} was not set: {e}")
 
 
-def extractInputElems(inputs, inputPath: List[str], elems: List[str] = [], tagElems: List[str] = []):
+def extractInputElems(inputs, inputPath: List[str], elems: List[str] = [],
+                      tagElems: List[str] = []):
     '''
     Takes lists of elements and tag elements, and traverses through the input tree towards the
     Input path, extracting the most recent matching values for these elements from the inputs.
 
     Returns these results in a single dict, so overwriting of results will occur if specified
     elements/tag elements have the same name in the inputs tree
     '''
```

### Comparing `cloudvision-1.9.0/cloudvision/cvlib/topology.py` & `cloudvision-1.9.1/cloudvision/cvlib/topology.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
         self.sourceDevice = sourceDevice
         self.sourceInterface = sourceInterface
         self.destDevice = destDevice
         self.destInterface = destInterface
 
     def __str__(self):
         return (
-            f"{self.sourceDevice}:{self.sourceInterface} --> {self.destDevice}:{self.destInterface}")
+            (f"{self.sourceDevice}:{self.sourceInterface} --> "
+             f"{self.destDevice}:{self.destInterface}"))
 
 
 class Topology:
     '''
     Topology object that stores devices and their connection to one another in dict form:
     - deviceMap:   Prebuilt topology device dictionary to instantiate the class with
     '''
```

### Comparing `cloudvision-1.9.0/cloudvision/cvlib/utils.py` & `cloudvision-1.9.1/cloudvision/cvlib/utils.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/cloudvision.egg-info/PKG-INFO` & `cloudvision-1.9.1/cloudvision.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudvision
-Version: 1.9.0
+Version: 1.9.1
 Summary: A Python library for Arista's CloudVision APIs.
 Home-page: https://github.com/aristanetworks/cloudvision-python
 Maintainer-email: support@arista.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `cloudvision-1.9.0/cloudvision.egg-info/SOURCES.txt` & `cloudvision-1.9.1/cloudvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/fmp/deletes_pb2.py` & `cloudvision-1.9.1/fmp/deletes_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/fmp/extensions_pb2.py` & `cloudvision-1.9.1/fmp/extensions_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/fmp/inet_pb2.py` & `cloudvision-1.9.1/fmp/inet_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/fmp/wrappers_pb2.py` & `cloudvision-1.9.1/fmp/wrappers_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/fmp/yang_pb2.py` & `cloudvision-1.9.1/fmp/yang_pb2.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/setup.py` & `cloudvision-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `cloudvision-1.9.0/test/test_codec.py` & `cloudvision-1.9.1/test/test_codec.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,8 +105,10 @@
     for tc in decodeTcs:
         input = tc["in"]
         exp = tc["exp"]
         out = decoder.decode(bytes(input))
         assert out == exp, f"Bad decoding of {input}\nGot: '{out}'\nExp: '{exp}'"
         out_json = json.JSONEncoder(ensure_ascii=True).encode({"value": out})
         exp_json = tc["exp_json"]
-        assert out_json == exp_json, f"Unexpected json decoding of {input}\nGot: '{out_json}'\nExp: '{exp_json}'"
+        assert out_json == exp_json, (f"Unexpected json decoding of {input}\n"
+                                      f"Got: '{out_json}'\n"
+                                      f"Exp: '{exp_json}'")
```

### Comparing `cloudvision-1.9.0/test/test_cvlib_studio.py` & `cloudvision-1.9.1/test/test_cvlib_studio.py`

 * *Files identical despite different names*

