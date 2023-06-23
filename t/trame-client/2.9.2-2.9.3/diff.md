# Comparing `tmp/trame-client-2.9.2.tar.gz` & `tmp/trame-client-2.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-client-2.9.2.tar", last modified: Fri Jun 16 21:54:27 2023, max compression
+gzip compressed data, was "trame-client-2.9.3.tar", last modified: Fri Jun 23 01:00:46 2023, max compression
```

## Comparing `trame-client-2.9.2.tar` & `trame-client-2.9.3.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.478666 trame-client-2.9.2/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-16 21:53:53.000000 trame-client-2.9.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      234 2023-06-16 21:53:53.000000 trame-client-2.9.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3518 2023-06-16 21:54:27.478666 trame-client-2.9.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2785 2023-06-16 21:53:53.000000 trame-client-2.9.2/README.rst
--rw-r--r--   0 root         (0) root         (0)      842 2023-06-16 21:54:27.482666 trame-client-2.9.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-16 21:53:53.000000 trame-client-2.9.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.470666 trame-client-2.9.2/trame/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.470666 trame-client-2.9.2/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)       34 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/modules/www.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.470666 trame-client-2.9.2/trame/ui/
--rw-r--r--   0 root         (0) root         (0)       56 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)       35 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/ui/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.470666 trame-client-2.9.2/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      137 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/widgets/client.py
--rw-r--r--   0 root         (0) root         (0)       75 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame/widgets/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.470666 trame-client-2.9.2/trame_client/
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/LICENSE
--rw-r--r--   0 root         (0) root         (0)       82 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.474666 trame-client-2.9.2/trame_client/encoders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/encoders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1146 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/encoders/numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.474666 trame-client-2.9.2/trame_client/module/
--rw-r--r--   0 root         (0) root         (0)      455 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/module/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.474666 trame-client-2.9.2/trame_client/module/vue2-www/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.474666 trame-client-2.9.2/trame_client/module/vue2-www/css/
--rw-r--r--   0 root         (0) root         (0)     1588 2023-06-16 21:54:15.000000 trame-client-2.9.2/trame_client/module/vue2-www/css/app.0b077e70.css
--rw-r--r--   0 root         (0) root         (0)     3963 2023-06-16 21:54:15.000000 trame-client-2.9.2/trame_client/module/vue2-www/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.474666 trame-client-2.9.2/trame_client/module/vue2-www/js/
--rw-r--r--   0 root         (0) root         (0)    23564 2023-06-16 21:54:15.000000 trame-client-2.9.2/trame_client/module/vue2-www/js/app.93852572.js
--rw-r--r--   0 root         (0) root         (0)   170437 2023-06-16 21:54:15.000000 trame-client-2.9.2/trame_client/module/vue2-www/js/chunk-vendors.b42af71c.js
--rw-r--r--   0 root         (0) root         (0)     4506 2023-06-16 21:54:15.000000 trame-client-2.9.2/trame_client/module/vue2-www/logo.png
--rw-r--r--   0 root         (0) root         (0)   107302 2023-06-16 21:54:15.000000 trame-client-2.9.2/trame_client/module/vue2-www/vue.global.js
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/module/vue2.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.474666 trame-client-2.9.2/trame_client/module/vue3-www/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.478666 trame-client-2.9.2/trame_client/module/vue3-www/assets/
--rw-r--r--   0 root         (0) root         (0)   108146 2023-06-16 21:54:22.000000 trame-client-2.9.2/trame_client/module/vue3-www/assets/index-ccad3410.js
--rw-r--r--   0 root         (0) root         (0)     3940 2023-06-16 21:54:22.000000 trame-client-2.9.2/trame_client/module/vue3-www/index.html
--rw-r--r--   0 root         (0) root         (0)     4506 2023-06-16 21:54:22.000000 trame-client-2.9.2/trame_client/module/vue3-www/logo.png
--rw-r--r--   0 root         (0) root         (0)   128872 2023-06-16 21:54:22.000000 trame-client-2.9.2/trame_client/module/vue3-www/vue.global.js
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/module/vue3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.478666 trame-client-2.9.2/trame_client/resources/
--rw-r--r--   0 root         (0) root         (0)     7243 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/resources/attributes.json
--rw-r--r--   0 root         (0) root         (0)        2 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/resources/events.json
--rw-r--r--   0 root         (0) root         (0)      580 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/resources/vue.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.478666 trame-client-2.9.2/trame_client/ui/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5472 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/ui/core.py
--rw-r--r--   0 root         (0) root         (0)      575 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/ui/html.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.478666 trame-client-2.9.2/trame_client/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      205 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/utils/defaults.py
--rw-r--r--   0 root         (0) root         (0)     1931 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/utils/testing.py
--rw-r--r--   0 root         (0) root         (0)      552 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.478666 trame-client-2.9.2/trame_client/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19978 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/widgets/core.py
--rw-r--r--   0 root         (0) root         (0)     3482 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/widgets/generator.py
--rw-r--r--   0 root         (0) root         (0)   193844 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/widgets/html.py
--rw-r--r--   0 root         (0) root         (0)     4670 2023-06-16 21:53:53.000000 trame-client-2.9.2/trame_client/widgets/trame.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-16 21:54:27.474666 trame-client-2.9.2/trame_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3518 2023-06-16 21:54:27.000000 trame-client-2.9.2/trame_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1478 2023-06-16 21:54:27.000000 trame-client-2.9.2/trame_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-16 21:54:27.000000 trame-client-2.9.2/trame_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-06-16 21:54:27.000000 trame-client-2.9.2/trame_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.565185 trame-client-2.9.3/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-23 01:00:13.000000 trame-client-2.9.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      234 2023-06-23 01:00:13.000000 trame-client-2.9.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3539 2023-06-23 01:00:46.565185 trame-client-2.9.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2785 2023-06-23 01:00:13.000000 trame-client-2.9.3/README.rst
+-rw-r--r--   0 root         (0) root         (0)      935 2023-06-23 01:00:46.565185 trame-client-2.9.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 01:00:13.000000 trame-client-2.9.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.557185 trame-client-2.9.3/trame/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.557185 trame-client-2.9.3/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       34 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame/modules/www.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.557185 trame-client-2.9.3/trame/ui/
+-rw-r--r--   0 root         (0) root         (0)       56 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame/ui/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.557185 trame-client-2.9.3/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      137 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame/widgets/client.py
+-rw-r--r--   0 root         (0) root         (0)       75 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame/widgets/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.557185 trame-client-2.9.3/trame_client/
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       82 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.557185 trame-client-2.9.3/trame_client/encoders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/encoders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1146 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/encoders/numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.557185 trame-client-2.9.3/trame_client/module/
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/module/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.561185 trame-client-2.9.3/trame_client/module/vue2-www/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.561185 trame-client-2.9.3/trame_client/module/vue2-www/css/
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-06-23 01:00:34.000000 trame-client-2.9.3/trame_client/module/vue2-www/css/app.0b077e70.css
+-rw-r--r--   0 root         (0) root         (0)     3963 2023-06-23 01:00:34.000000 trame-client-2.9.3/trame_client/module/vue2-www/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.561185 trame-client-2.9.3/trame_client/module/vue2-www/js/
+-rw-r--r--   0 root         (0) root         (0)    23564 2023-06-23 01:00:34.000000 trame-client-2.9.3/trame_client/module/vue2-www/js/app.93852572.js
+-rw-r--r--   0 root         (0) root         (0)   170437 2023-06-23 01:00:34.000000 trame-client-2.9.3/trame_client/module/vue2-www/js/chunk-vendors.b42af71c.js
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-06-23 01:00:34.000000 trame-client-2.9.3/trame_client/module/vue2-www/logo.png
+-rw-r--r--   0 root         (0) root         (0)   107302 2023-06-23 01:00:34.000000 trame-client-2.9.3/trame_client/module/vue2-www/vue.global.js
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/module/vue2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.561185 trame-client-2.9.3/trame_client/module/vue3-www/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.561185 trame-client-2.9.3/trame_client/module/vue3-www/assets/
+-rw-r--r--   0 root         (0) root         (0)   108146 2023-06-23 01:00:41.000000 trame-client-2.9.3/trame_client/module/vue3-www/assets/index-ccad3410.js
+-rw-r--r--   0 root         (0) root         (0)     3940 2023-06-23 01:00:41.000000 trame-client-2.9.3/trame_client/module/vue3-www/index.html
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-06-23 01:00:41.000000 trame-client-2.9.3/trame_client/module/vue3-www/logo.png
+-rw-r--r--   0 root         (0) root         (0)   128872 2023-06-23 01:00:41.000000 trame-client-2.9.3/trame_client/module/vue3-www/vue.global.js
+-rw-r--r--   0 root         (0) root         (0)       84 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/module/vue3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.561185 trame-client-2.9.3/trame_client/resources/
+-rw-r--r--   0 root         (0) root         (0)     7243 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/resources/attributes.json
+-rw-r--r--   0 root         (0) root         (0)        2 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/resources/events.json
+-rw-r--r--   0 root         (0) root         (0)      580 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/resources/vue.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.561185 trame-client-2.9.3/trame_client/ui/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/ui/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5472 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/ui/core.py
+-rw-r--r--   0 root         (0) root         (0)      575 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/ui/html.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.561185 trame-client-2.9.3/trame_client/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      205 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/utils/defaults.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/utils/testing.py
+-rw-r--r--   0 root         (0) root         (0)      552 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.565185 trame-client-2.9.3/trame_client/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19978 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/widgets/core.py
+-rw-r--r--   0 root         (0) root         (0)     3482 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/widgets/generator.py
+-rw-r--r--   0 root         (0) root         (0)   193844 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/widgets/html.py
+-rw-r--r--   0 root         (0) root         (0)     4670 2023-06-23 01:00:13.000000 trame-client-2.9.3/trame_client/widgets/trame.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 01:00:46.557185 trame-client-2.9.3/trame_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3539 2023-06-23 01:00:46.000000 trame-client-2.9.3/trame_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-06-23 01:00:46.000000 trame-client-2.9.3/trame_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 01:00:46.000000 trame-client-2.9.3/trame_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-23 01:00:46.000000 trame-client-2.9.3/trame_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-23 01:00:46.000000 trame-client-2.9.3/trame_client.egg-info/top_level.txt
```

### Comparing `trame-client-2.9.2/LICENSE` & `trame-client-2.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/PKG-INFO` & `trame-client-2.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: trame-client
-Version: 2.9.2
+Version: 2.9.3
 Summary: Internal client of trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: JavaScript
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 trame-client: core client for trame
 ===========================================================================
 
 .. image:: https://github.com/Kitware/trame-client/actions/workflows/test_and_release.yml/badge.svg
     :target: https://github.com/Kitware/trame-client/actions/workflows/test_and_release.yml
```

### Comparing `trame-client-2.9.2/README.rst` & `trame-client-2.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/setup.cfg` & `trame-client-2.9.3/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame-client
-version = 2.9.2
+version = 2.9.3
 description = Internal client of trame
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = MIT
 classifiers = 
 	Development Status :: 5 - Production/Stable
@@ -23,14 +23,22 @@
 	Application
 	Framework
 
 [options]
 packages = find:
 include_package_data = True
 
+[options.extras_require]
+test = 
+	pytest
+	seleniumbase
+	pytest-xprocess
+	Pillow
+	pixelmatch
+
 [semantic_release]
 version_pattern = setup.cfg:version = (\d+\.\d+\.\d+)
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `trame-client-2.9.2/trame_client/LICENSE` & `trame-client-2.9.3/trame_client/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/encoders/numpy.py` & `trame-client-2.9.3/trame_client/encoders/numpy.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/module/vue2-www/css/app.0b077e70.css` & `trame-client-2.9.3/trame_client/module/vue2-www/css/app.0b077e70.css`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/module/vue2-www/index.html` & `trame-client-2.9.3/trame_client/module/vue2-www/index.html`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/module/vue2-www/js/app.93852572.js` & `trame-client-2.9.3/trame_client/module/vue2-www/js/app.93852572.js`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/module/vue2-www/js/chunk-vendors.b42af71c.js` & `trame-client-2.9.3/trame_client/module/vue2-www/js/chunk-vendors.b42af71c.js`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/module/vue2-www/logo.png` & `trame-client-2.9.3/trame_client/module/vue2-www/logo.png`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/module/vue2-www/vue.global.js` & `trame-client-2.9.3/trame_client/module/vue2-www/vue.global.js`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/module/vue3-www/assets/index-ccad3410.js` & `trame-client-2.9.3/trame_client/module/vue3-www/assets/index-ccad3410.js`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/module/vue3-www/index.html` & `trame-client-2.9.3/trame_client/module/vue3-www/index.html`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/module/vue3-www/logo.png` & `trame-client-2.9.3/trame_client/module/vue3-www/logo.png`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/module/vue3-www/vue.global.js` & `trame-client-2.9.3/trame_client/module/vue3-www/vue.global.js`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/resources/attributes.json` & `trame-client-2.9.3/trame_client/resources/attributes.json`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/resources/vue.json` & `trame-client-2.9.3/trame_client/resources/vue.json`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/ui/core.py` & `trame-client-2.9.3/trame_client/ui/core.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/ui/html.py` & `trame-client-2.9.3/trame_client/ui/html.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/utils/version.py` & `trame-client-2.9.3/trame_client/utils/version.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/widgets/core.py` & `trame-client-2.9.3/trame_client/widgets/core.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/widgets/generator.py` & `trame-client-2.9.3/trame_client/widgets/generator.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/widgets/html.py` & `trame-client-2.9.3/trame_client/widgets/html.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client/widgets/trame.py` & `trame-client-2.9.3/trame_client/widgets/trame.py`

 * *Files identical despite different names*

### Comparing `trame-client-2.9.2/trame_client.egg-info/PKG-INFO` & `trame-client-2.9.3/trame_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: trame-client
-Version: 2.9.2
+Version: 2.9.3
 Summary: Internal client of trame
 Author: Kitware Inc.
 License: MIT
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: JavaScript
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/x-rst
+Provides-Extra: test
 License-File: LICENSE
 
 trame-client: core client for trame
 ===========================================================================
 
 .. image:: https://github.com/Kitware/trame-client/actions/workflows/test_and_release.yml/badge.svg
     :target: https://github.com/Kitware/trame-client/actions/workflows/test_and_release.yml
```

### Comparing `trame-client-2.9.2/trame_client.egg-info/SOURCES.txt` & `trame-client-2.9.3/trame_client.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 trame/widgets/client.py
 trame/widgets/html.py
 trame_client/LICENSE
 trame_client/__init__.py
 trame_client.egg-info/PKG-INFO
 trame_client.egg-info/SOURCES.txt
 trame_client.egg-info/dependency_links.txt
+trame_client.egg-info/requires.txt
 trame_client.egg-info/top_level.txt
 trame_client/encoders/__init__.py
 trame_client/encoders/numpy.py
 trame_client/module/__init__.py
 trame_client/module/vue2.py
 trame_client/module/vue3.py
 trame_client/module/vue2-www/index.html
```

