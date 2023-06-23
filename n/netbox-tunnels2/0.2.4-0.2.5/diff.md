# Comparing `tmp/netbox-tunnels2-0.2.4.tar.gz` & `tmp/netbox-tunnels2-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-tunnels2-0.2.4.tar", last modified: Tue May  9 13:36:17 2023, max compression
+gzip compressed data, was "netbox-tunnels2-0.2.5.tar", last modified: Fri Jun 23 18:41:30 2023, max compression
```

## Comparing `netbox-tunnels2-0.2.4.tar` & `netbox-tunnels2-0.2.5.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:17.259015 netbox-tunnels2-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-05-09 13:36:17.259015 netbox-tunnels2-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:17.247015 netbox-tunnels2-0.2.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:17.251015 netbox-tunnels2-0.2.4/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)   221681 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/docs/img/tunnel-info.png
--rw-r--r--   0 runner    (1001) docker     (123)   150947 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/docs/img/tunnel-list.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:17.255015 netbox-tunnels2-0.2.4/netbox_tunnels2/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:17.255015 netbox-tunnels2-0.2.4/netbox_tunnels2/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/api/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/graphql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:17.255015 netbox-tunnels2-0.2.4/netbox_tunnels2/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/migrations/0002_alter_tunnel_b_pub_address.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/navigation.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:17.247015 netbox-tunnels2-0.2.4/netbox_tunnels2/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:17.255015 netbox-tunnels2-0.2.4/netbox_tunnels2/templates/netbox_tunnels2/
--rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:17.259015 netbox-tunnels2-0.2.4/netbox_tunnels2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/tests/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/netbox_tunnels2/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:36:17.255015 netbox-tunnels2-0.2.4/netbox_tunnels2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-05-09 13:36:17.000000 netbox-tunnels2-0.2.4/netbox_tunnels2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-09 13:36:17.000000 netbox-tunnels2-0.2.4/netbox_tunnels2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:36:17.000000 netbox-tunnels2-0.2.4/netbox_tunnels2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 13:36:17.000000 netbox-tunnels2-0.2.4/netbox_tunnels2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-09 13:36:17.000000 netbox-tunnels2-0.2.4/netbox_tunnels2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-09 13:36:17.259015 netbox-tunnels2-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-09 13:35:59.000000 netbox-tunnels2-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.506685 netbox-tunnels2-0.2.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.506685 netbox-tunnels2-0.2.5/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)   221681 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/docs/img/tunnel-info.png
+-rw-r--r--   0 runner    (1001) docker     (123)   150947 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/docs/img/tunnel-list.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.506685 netbox-tunnels2-0.2.5/netbox_tunnels2/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/netbox_tunnels2/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8822 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/graphql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/netbox_tunnels2/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/migrations/0002_alter_tunnel_b_pub_address.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3688 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.506685 netbox-tunnels2-0.2.5/netbox_tunnels2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/netbox_tunnels2/templates/netbox_tunnels2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/netbox_tunnels2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/tests/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/netbox_tunnels2/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15854 2023-06-23 18:41:30.000000 netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-06-23 18:41:30.000000 netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:41:30.000000 netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 18:41:30.000000 netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 18:41:30.000000 netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-23 18:41:30.510685 netbox-tunnels2-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-06-23 18:41:20.000000 netbox-tunnels2-0.2.5/setup.py
```

### Comparing `netbox-tunnels2-0.2.4/CONTRIBUTING.md` & `netbox-tunnels2-0.2.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/LICENSE` & `netbox-tunnels2-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/PKG-INFO` & `netbox-tunnels2-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-tunnels2
-Version: 0.2.4
+Version: 0.2.5
 Summary: Provides the ability track IP Tunnels.
 Home-page: https://github.com/robertlynch3/netbox-tunnels2
 Author: Robert Lynch
 Author-email: Robert Lynch <robertlynch3@users.noreply.github.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `netbox-tunnels2-0.2.4/README.md` & `netbox-tunnels2-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/docs/img/tunnel-info.png` & `netbox-tunnels2-0.2.5/docs/img/tunnel-info.png`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/docs/img/tunnel-list.png` & `netbox-tunnels2-0.2.5/docs/img/tunnel-list.png`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/__init__.py` & `netbox-tunnels2-0.2.5/netbox_tunnels2/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/api/serializers.py` & `netbox-tunnels2-0.2.5/netbox_tunnels2/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/api/views.py` & `netbox-tunnels2-0.2.5/netbox_tunnels2/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/filtersets.py` & `netbox-tunnels2-0.2.5/netbox_tunnels2/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/forms.py` & `netbox-tunnels2-0.2.5/netbox_tunnels2/forms.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/graphql.py` & `netbox-tunnels2-0.2.5/netbox_tunnels2/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/migrations/0001_initial.py` & `netbox-tunnels2-0.2.5/netbox_tunnels2/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/migrations/0002_alter_tunnel_b_pub_address.py` & `netbox-tunnels2-0.2.5/netbox_tunnels2/migrations/0002_alter_tunnel_b_pub_address.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/models.py` & `netbox-tunnels2-0.2.5/netbox_tunnels2/models.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/navigation.py` & `netbox-tunnels2-0.2.5/netbox_tunnels2/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/tables.py` & `netbox-tunnels2-0.2.5/netbox_tunnels2/tables.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html` & `netbox-tunnels2-0.2.5/netbox_tunnels2/templates/netbox_tunnels2/tunnel.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% extends 'generic/object.html' %}
+{% load plugins %}
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Tunnel</h5>
         <div class="card-body">
           <table class="table table-hover attr-table">
@@ -30,18 +31,20 @@
               <th scope="row">Pre Shared Key</th>
               <td>{{ object.psk }}</td>
             </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
+      {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
       {% include 'inc/panels/tags.html' %}
       {% include 'inc/panels/comments.html' %}
+      {% plugin_right_page object %}
     </div>
   </div>
   <div class="row">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Endpoints</h5>
         <div class="card-body table-responsive">
@@ -74,15 +77,20 @@
               </tbody>
             </table>
           </div>
         </div>
       </div>
     </div>
   </div>
-  <div class="row">
+  <div class="row mb-3">
     <div class="col col-md-6">
 
     
 
     </div>
   </div>
+  <div class="row mb-3">
+    <div class="col col-md-12">
+      {% plugin_full_width_page object %}
+    </div>
+  </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,18 +1,20 @@
-{% extends 'generic/object.html' %} {% block content %}
+{% extends 'generic/object.html' %} {% load plugins %} {% block content %}
 ** Tunnel **
 Name           {{ object.name }}
 Status         {% badge object.get_status_display
                bg_color=object.get_status_color %}
 Tunnel Type    {{_object.tunnel_type_}}
 Local Address  {{_object.a_pub_address_}}
 Remote Address {{_object.b_pub_address_}}
 Pre Shared Key {{ object.psk }}
-{% include 'inc/panels/custom_fields.html' %}
+{% include 'inc/panels/custom_fields.html' %} {% plugin_left_page object %}
 {% include 'inc/panels/tags.html' %} {% include 'inc/panels/comments.html' %}
+{% plugin_right_page object %}
 ** Endpoints **
 Side A Device                                    Side A Inside Interface                   Side B Device                                    Side B Inside Interface
 {                                                {                                         {                                                {
 {                                                {                                         {                                                {
 object.side_a_assigned_object.device|placeholder object.side_a_assigned_object|placeholder object.side_b_assigned_object.device|placeholder object.side_b_assigned_object|placeholder
 }}                                               }}                                        }}                                               }}
+{% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html` & `netbox-tunnels2-0.2.5/netbox_tunnels2/templates/netbox_tunnels2/tunnel_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html` & `netbox-tunnels2-0.2.5/netbox_tunnels2/templates/netbox_tunnels2/tunneltype.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% extends 'generic/object.html' %}
+{% load plugins %}
 {% load render_table from django_tables2 %}
 {% block content %}
   <div class="row mb-3">
     <div class="col col-md-6">
       <div class="card">
         <h5 class="card-header">Tunnel</h5>
         <div class="card-body">
@@ -11,22 +12,29 @@
               <th scope="row">Name</th>
               <td>{{ object.name }}</td>
             </tr>
           </table>
         </div>
       </div>
       {% include 'inc/panels/custom_fields.html' %}
+      {% plugin_left_page object %}
     </div>
     <div class="col col-md-6">
+      {% plugin_right_page object %}
     </div>
   </div>
-  <div class="row">
+  <div class="row mb-3">
     <div class="col col-md-12">
       <div class="card">
         <h5 class="card-header">Tunnels</h5>
         <div class="card-body table-responsive">
           {% render_table tunnel_table %}
         </div>
       </div>
     </div>
   </div>
-{% endblock content %}
+  <div class="row mb-3">
+    <div class="col col-md-12">
+      {% plugin_full_width_page object %}
+    </div>
+  </div>
+{% endblock content %}
```

#### html2text {}

```diff
@@ -1,8 +1,10 @@
-{% extends 'generic/object.html' %} {% load render_table from django_tables2 %}
-{% block content %}
+{% extends 'generic/object.html' %} {% load plugins %} {% load render_table
+from django_tables2 %} {% block content %}
 ** Tunnel **
 Name {{ object.name }}
-{% include 'inc/panels/custom_fields.html' %}
+{% include 'inc/panels/custom_fields.html' %} {% plugin_left_page object %}
+{% plugin_right_page object %}
 ** Tunnels **
 {% render_table tunnel_table %}
+{% plugin_full_width_page object %}
 {% endblock content %}
```

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/tests/custom.py` & `netbox-tunnels2-0.2.5/netbox_tunnels2/tests/custom.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/tests/test_models.py` & `netbox-tunnels2-0.2.5/netbox_tunnels2/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/urls.py` & `netbox-tunnels2-0.2.5/netbox_tunnels2/urls.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2/views.py` & `netbox-tunnels2-0.2.5/netbox_tunnels2/views.py`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2.egg-info/PKG-INFO` & `netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-tunnels2
-Version: 0.2.4
+Version: 0.2.5
 Summary: Provides the ability track IP Tunnels.
 Home-page: https://github.com/robertlynch3/netbox-tunnels2
 Author: Robert Lynch
 Author-email: Robert Lynch <robertlynch3@users.noreply.github.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `netbox-tunnels2-0.2.4/netbox_tunnels2.egg-info/SOURCES.txt` & `netbox-tunnels2-0.2.5/netbox_tunnels2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/pyproject.toml` & `netbox-tunnels2-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-tunnels2"
-version = "0.2.4"
+version = "0.2.5"
 description = "Provides the ability track IP Tunnels."
 readme = "README.md"
 authors = [{ name = "Robert Lynch", email = "robertlynch3@users.noreply.github.com" }]
 license = { file = "LICENSE" }
 
 [project.urls]
 Homepage = "https://github.com/robertlynch3/netbox-tunnels2"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver]
-current_version = "0.2.4"
+current_version = "0.2.5"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `netbox-tunnels2-0.2.4/setup.cfg` & `netbox-tunnels2-0.2.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `netbox-tunnels2-0.2.4/setup.py` & `netbox-tunnels2-0.2.5/setup.py`

 * *Files identical despite different names*

