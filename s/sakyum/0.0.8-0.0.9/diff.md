# Comparing `tmp/sakyum-0.0.8.tar.gz` & `tmp/sakyum-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sakyum-0.0.8.tar", last modified: Fri Jun  9 17:49:34 2023, max compression
+gzip compressed data, was "sakyum-0.0.9.tar", last modified: Thu Jun 22 19:59:36 2023, max compression
```

## Comparing `sakyum-0.0.8.tar` & `sakyum-0.0.9.tar`

### file list

```diff
@@ -1,70 +1,69 @@
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.388300 sakyum-0.0.8/
--rw-rw-r--   0 usman     (1000) usman     (1000)     1309 2023-06-09 17:39:22.000000 sakyum-0.0.8/CHANGELOG
--rw-rw-r--   0 usman     (1000) usman     (1000)     1077 2023-06-08 02:53:33.000000 sakyum-0.0.8/LICENSE
--rw-rw-r--   0 usman     (1000) usman     (1000)       82 2023-06-08 02:53:33.000000 sakyum-0.0.8/MANIFEST.in
--rw-rw-r--   0 usman     (1000) usman     (1000)     6426 2023-06-09 17:49:34.384300 sakyum-0.0.8/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)     2996 2023-06-09 17:44:39.000000 sakyum-0.0.8/README.md
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.276288 sakyum-0.0.8/media/
--rw-rw-r--   0 usman     (1000) usman     (1000)    33115 2023-06-09 17:06:35.000000 sakyum-0.0.8/media/sakyum_default_page.png
--rw-rw-r--   0 usman     (1000) usman     (1000)      412 2023-06-09 13:53:26.000000 sakyum-0.0.8/requirements.txt
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.304291 sakyum-0.0.8/sakyum/
--rw-rw-r--   0 usman     (1000) usman     (1000)      725 2023-06-09 14:23:38.000000 sakyum-0.0.8/sakyum/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)      489 2023-06-08 20:31:39.000000 sakyum-0.0.8/sakyum/api.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.324293 sakyum-0.0.8/sakyum/auth/
--rw-rw-r--   0 usman     (1000) usman     (1000)       46 2023-06-08 17:44:37.000000 sakyum-0.0.8/sakyum/auth/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1298 2023-06-08 20:40:43.000000 sakyum-0.0.8/sakyum/auth/admin.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1643 2023-06-08 20:41:07.000000 sakyum-0.0.8/sakyum/auth/forms.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1280 2023-06-09 14:26:48.000000 sakyum-0.0.8/sakyum/auth/models.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     6069 2023-06-09 14:28:34.000000 sakyum-0.0.8/sakyum/auth/routes.py
--rw-rw-r--   0 usman     (1000) usman     (1000)    21240 2023-06-09 17:13:59.000000 sakyum-0.0.8/sakyum/base.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     4711 2023-06-09 14:10:59.000000 sakyum-0.0.8/sakyum/blueprint.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.324293 sakyum-0.0.8/sakyum/contrib/
--rw-rw-r--   0 usman     (1000) usman     (1000)      619 2023-06-09 14:28:59.000000 sakyum-0.0.8/sakyum/contrib/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)      437 2023-06-09 14:08:46.000000 sakyum-0.0.8/sakyum/database.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.336295 sakyum-0.0.8/sakyum/mute/
--rw-rw-r--   0 usman     (1000) usman     (1000)      581 2023-06-08 20:49:28.000000 sakyum-0.0.8/sakyum/mute/__init__.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     1517 2023-06-08 20:50:10.000000 sakyum-0.0.8/sakyum/mute/app.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     2899 2023-06-08 20:53:35.000000 sakyum-0.0.8/sakyum/mute/page.py
--rw-rw-r--   0 usman     (1000) usman     (1000)     3400 2023-06-08 20:51:58.000000 sakyum-0.0.8/sakyum/mute/project.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.336295 sakyum-0.0.8/sakyum/static/
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.256286 sakyum-0.0.8/sakyum/static/default_style/
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.340295 sakyum-0.0.8/sakyum/static/default_style/css/
--rw-rw-r--   0 usman     (1000) usman     (1000)     6831 2023-06-08 02:53:33.000000 sakyum-0.0.8/sakyum/static/default_style/css/style.css
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.340295 sakyum-0.0.8/sakyum/static/default_style/js/
--rw-rw-r--   0 usman     (1000) usman     (1000)      127 2023-06-08 02:53:33.000000 sakyum-0.0.8/sakyum/static/default_style/js/index.js
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.344295 sakyum-0.0.8/sakyum/static/default_style/media/
--rw-rw-r--   0 usman     (1000) usman     (1000)     3767 2023-06-08 02:53:33.000000 sakyum-0.0.8/sakyum/static/default_style/media/alert.png
--rw-rw-r--   0 usman     (1000) usman     (1000)     1460 2023-06-08 02:53:33.000000 sakyum-0.0.8/sakyum/static/default_style/media/default_img.png
--rw-rw-r--   0 usman     (1000) usman     (1000)     3767 2023-06-08 02:53:33.000000 sakyum-0.0.8/sakyum/static/default_style/media/favicon.ico
--rw-rw-r--   0 usman     (1000) usman     (1000)        0 2023-06-09 17:10:52.000000 sakyum-0.0.8/sakyum/static/do_nothing.txt
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.260286 sakyum-0.0.8/sakyum/templates/
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.368298 sakyum-0.0.8/sakyum/templates/default_errors/
--rw-rw-r--   0 usman     (1000) usman     (1000)      141 2023-06-08 20:59:20.000000 sakyum-0.0.8/sakyum/templates/default_errors/400.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      142 2023-06-08 20:59:37.000000 sakyum-0.0.8/sakyum/templates/default_errors/401.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      139 2023-06-08 20:59:53.000000 sakyum-0.0.8/sakyum/templates/default_errors/403.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      139 2023-06-08 21:00:12.000000 sakyum-0.0.8/sakyum/templates/default_errors/404.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      144 2023-06-08 21:00:24.000000 sakyum-0.0.8/sakyum/templates/default_errors/406.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      152 2023-06-08 21:00:35.000000 sakyum-0.0.8/sakyum/templates/default_errors/415.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      147 2023-06-08 21:00:48.000000 sakyum-0.0.8/sakyum/templates/default_errors/429.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      151 2023-06-08 21:00:58.000000 sakyum-0.0.8/sakyum/templates/default_errors/500.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      146 2023-06-08 21:01:10.000000 sakyum-0.0.8/sakyum/templates/default_errors/501.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      142 2023-06-08 21:01:21.000000 sakyum-0.0.8/sakyum/templates/default_errors/502.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      150 2023-06-08 21:01:42.000000 sakyum-0.0.8/sakyum/templates/default_errors/503.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      146 2023-06-08 21:02:17.000000 sakyum-0.0.8/sakyum/templates/default_errors/504.html
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.384300 sakyum-0.0.8/sakyum/templates/default_page/
--rw-rw-r--   0 usman     (1000) usman     (1000)     3092 2023-06-08 21:03:30.000000 sakyum-0.0.8/sakyum/templates/default_page/admin_change_password.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      622 2023-06-08 21:04:03.000000 sakyum-0.0.8/sakyum/templates/default_page/admin_change_profile_image.html
--rw-rw-r--   0 usman     (1000) usman     (1000)     2262 2023-06-08 21:04:15.000000 sakyum-0.0.8/sakyum/templates/default_page/admin_login.html
--rw-rw-r--   0 usman     (1000) usman     (1000)     3150 2023-06-08 21:04:26.000000 sakyum-0.0.8/sakyum/templates/default_page/admin_register.html
--rw-rw-r--   0 usman     (1000) usman     (1000)     4156 2023-06-08 17:44:37.000000 sakyum-0.0.8/sakyum/templates/default_page/default.html
--rw-rw-r--   0 usman     (1000) usman     (1000)     1025 2023-06-08 21:04:49.000000 sakyum-0.0.8/sakyum/templates/default_page/default_base.html
--rw-rw-r--   0 usman     (1000) usman     (1000)      509 2023-06-08 21:03:15.000000 sakyum-0.0.8/sakyum/templates/default_page/default_index.html
--rw-rw-r--   0 usman     (1000) usman     (1000)     8715 2023-06-09 14:08:31.000000 sakyum-0.0.8/sakyum/utils.py
-drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-09 17:49:34.312292 sakyum-0.0.8/sakyum.egg-info/
--rw-rw-r--   0 usman     (1000) usman     (1000)     6426 2023-06-09 17:49:33.000000 sakyum-0.0.8/sakyum.egg-info/PKG-INFO
--rw-rw-r--   0 usman     (1000) usman     (1000)     1669 2023-06-09 17:49:34.000000 sakyum-0.0.8/sakyum.egg-info/SOURCES.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-06-09 17:49:33.000000 sakyum-0.0.8/sakyum.egg-info/dependency_links.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)      398 2023-06-09 17:49:33.000000 sakyum-0.0.8/sakyum.egg-info/requires.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)        7 2023-06-09 17:49:33.000000 sakyum-0.0.8/sakyum.egg-info/top_level.txt
--rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-06-09 17:49:34.388300 sakyum-0.0.8/setup.cfg
--rw-rw-r--   0 usman     (1000) usman     (1000)     2568 2023-06-09 17:16:11.000000 sakyum-0.0.8/setup.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-22 19:59:36.348694 sakyum-0.0.9/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1412 2023-06-22 19:54:16.000000 sakyum-0.0.9/CHANGELOG
+-rw-r--r--   0 usman     (1000) usman     (1000)     1077 2023-06-22 19:54:16.000000 sakyum-0.0.9/LICENSE
+-rw-r--r--   0 usman     (1000) usman     (1000)       82 2023-06-22 19:54:16.000000 sakyum-0.0.9/MANIFEST.in
+-rw-rw-r--   0 usman     (1000) usman     (1000)     5554 2023-06-22 19:59:36.344693 sakyum-0.0.9/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3004 2023-06-22 19:54:16.000000 sakyum-0.0.9/README.md
+-rw-rw-r--   0 usman     (1000) usman     (1000)      412 2023-06-22 19:55:12.000000 sakyum-0.0.9/requirements.txt
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-22 19:59:36.172638 sakyum-0.0.9/sakyum/
+-rw-rw-r--   0 usman     (1000) usman     (1000)      725 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/__init__.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1280 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/api.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-22 19:59:36.216652 sakyum-0.0.9/sakyum/auth/
+-rw-r--r--   0 usman     (1000) usman     (1000)       46 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/auth/__init__.py
+-rw-r--r--   0 usman     (1000) usman     (1000)     1298 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/auth/admin.py
+-rw-r--r--   0 usman     (1000) usman     (1000)     1643 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/auth/forms.py
+-rw-r--r--   0 usman     (1000) usman     (1000)     1280 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/auth/models.py
+-rw-r--r--   0 usman     (1000) usman     (1000)     6069 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/auth/routes.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)    22696 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/base.py
+-rw-r--r--   0 usman     (1000) usman     (1000)     4711 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/blueprint.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-22 19:59:36.220653 sakyum-0.0.9/sakyum/contrib/
+-rw-r--r--   0 usman     (1000) usman     (1000)      619 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/contrib/__init__.py
+-rw-r--r--   0 usman     (1000) usman     (1000)      437 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/database.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-22 19:59:36.236658 sakyum-0.0.9/sakyum/mute/
+-rw-r--r--   0 usman     (1000) usman     (1000)      581 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/mute/__init__.py
+-rw-r--r--   0 usman     (1000) usman     (1000)     1517 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/mute/app.py
+-rw-r--r--   0 usman     (1000) usman     (1000)     2899 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/mute/page.py
+-rw-rw-r--   0 usman     (1000) usman     (1000)     3428 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/mute/project.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-22 19:59:36.236658 sakyum-0.0.9/sakyum/static/
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-22 19:59:36.076607 sakyum-0.0.9/sakyum/static/default_style/
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-22 19:59:36.240659 sakyum-0.0.9/sakyum/static/default_style/css/
+-rw-r--r--   0 usman     (1000) usman     (1000)     6831 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/static/default_style/css/style.css
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-22 19:59:36.244660 sakyum-0.0.9/sakyum/static/default_style/js/
+-rw-r--r--   0 usman     (1000) usman     (1000)      127 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/static/default_style/js/index.js
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-22 19:59:36.256664 sakyum-0.0.9/sakyum/static/default_style/media/
+-rw-r--r--   0 usman     (1000) usman     (1000)     3767 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/static/default_style/media/alert.png
+-rw-r--r--   0 usman     (1000) usman     (1000)     1460 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/static/default_style/media/default_img.png
+-rw-r--r--   0 usman     (1000) usman     (1000)     3767 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/static/default_style/media/favicon.ico
+-rw-r--r--   0 usman     (1000) usman     (1000)        0 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/static/do_nothing.txt
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-22 19:59:36.080608 sakyum-0.0.9/sakyum/templates/
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-22 19:59:36.304680 sakyum-0.0.9/sakyum/templates/default_errors/
+-rw-r--r--   0 usman     (1000) usman     (1000)      141 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/templates/default_errors/400.html
+-rw-r--r--   0 usman     (1000) usman     (1000)      142 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/templates/default_errors/401.html
+-rw-r--r--   0 usman     (1000) usman     (1000)      139 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/templates/default_errors/403.html
+-rw-r--r--   0 usman     (1000) usman     (1000)      139 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/templates/default_errors/404.html
+-rw-r--r--   0 usman     (1000) usman     (1000)      144 2023-06-22 19:55:12.000000 sakyum-0.0.9/sakyum/templates/default_errors/406.html
+-rw-r--r--   0 usman     (1000) usman     (1000)      152 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum/templates/default_errors/415.html
+-rw-r--r--   0 usman     (1000) usman     (1000)      147 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum/templates/default_errors/429.html
+-rw-r--r--   0 usman     (1000) usman     (1000)      151 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum/templates/default_errors/500.html
+-rw-r--r--   0 usman     (1000) usman     (1000)      146 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum/templates/default_errors/501.html
+-rw-r--r--   0 usman     (1000) usman     (1000)      142 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum/templates/default_errors/502.html
+-rw-r--r--   0 usman     (1000) usman     (1000)      150 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum/templates/default_errors/503.html
+-rw-r--r--   0 usman     (1000) usman     (1000)      146 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum/templates/default_errors/504.html
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-22 19:59:36.340691 sakyum-0.0.9/sakyum/templates/default_page/
+-rw-r--r--   0 usman     (1000) usman     (1000)     3092 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum/templates/default_page/admin_change_password.html
+-rw-r--r--   0 usman     (1000) usman     (1000)      622 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum/templates/default_page/admin_change_profile_image.html
+-rw-r--r--   0 usman     (1000) usman     (1000)     2262 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum/templates/default_page/admin_login.html
+-rw-r--r--   0 usman     (1000) usman     (1000)     3150 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum/templates/default_page/admin_register.html
+-rw-r--r--   0 usman     (1000) usman     (1000)     4156 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum/templates/default_page/default.html
+-rw-r--r--   0 usman     (1000) usman     (1000)     1025 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum/templates/default_page/default_base.html
+-rw-r--r--   0 usman     (1000) usman     (1000)      509 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum/templates/default_page/default_index.html
+-rw-rw-r--   0 usman     (1000) usman     (1000)     8715 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum/utils.py
+drwxrwxr-x   0 usman     (1000) usman     (1000)        0 2023-06-22 19:59:36.188643 sakyum-0.0.9/sakyum.egg-info/
+-rw-rw-r--   0 usman     (1000) usman     (1000)     5554 2023-06-22 19:59:34.000000 sakyum-0.0.9/sakyum.egg-info/PKG-INFO
+-rw-rw-r--   0 usman     (1000) usman     (1000)     1663 2023-06-22 19:59:35.000000 sakyum-0.0.9/sakyum.egg-info/SOURCES.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        1 2023-06-22 19:59:34.000000 sakyum-0.0.9/sakyum.egg-info/dependency_links.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)      398 2023-06-22 19:59:34.000000 sakyum-0.0.9/sakyum.egg-info/requires.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)        7 2023-06-22 19:59:34.000000 sakyum-0.0.9/sakyum.egg-info/top_level.txt
+-rw-rw-r--   0 usman     (1000) usman     (1000)    33632 2023-06-22 19:55:13.000000 sakyum-0.0.9/sakyum_default_page.png
+-rw-rw-r--   0 usman     (1000) usman     (1000)       38 2023-06-22 19:59:36.348694 sakyum-0.0.9/setup.cfg
+-rw-rw-r--   0 usman     (1000) usman     (1000)     2568 2023-06-22 19:55:13.000000 sakyum-0.0.9/setup.py
```

### Comparing `sakyum-0.0.8/CHANGELOG` & `sakyum-0.0.9/CHANGELOG`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 Change Log
 ==========
 
-0.0.8 (09/june/2023)
+0.0.9 (22/june/2023)
 ------------------
+- Nineth Release
+
+Fixing bugs
+
+Fixing v0.0.8 bugs for OS compatibility, and also tested on windows OS
+
 - Eight Release
 
 OS compatibility
 
 Making sakyum to be compatible with windows OS as well as other OS
 
 0.0.7 (4/april/2023)
```

### Comparing `sakyum-0.0.8/LICENSE` & `sakyum-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/PKG-INFO` & `sakyum-0.0.9/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,143 +1,18 @@
 Metadata-Version: 2.1
 Name: sakyum
-Version: 0.0.8
+Version: 0.0.9
 Summary: An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs
 Home-page: https://sakyum.readthedocs.io
+Download-URL: https://pypi.org/project/sakyum
 Author: Usman Musa
 Author-email: usmanmusa1920@gmail.com
 License: MIT
-Download-URL: https://pypi.org/project/sakyum
 Project-URL: Documentation, https://sakyum.readthedocs.io
 Project-URL: Source, https://github.com/usmanmusa1920/sakyum
-Description: 
-        # Sakyum
-        
-        An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs.
-        
-        ## Installation
-        
-        Install and update the latest release from <a href="https://pypi.org/project/sakyum">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) as from `v0.0.8` it is now compatible with `windows OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
-        
-        ```
-        pip install --upgrade sakyum
-        ```
-        
-        ## Create flask project using sakyum
-        
-        After the installation paste the following command on your termianl
-        
-        ```
-        python -c "from sakyum import project; project('schoolsite')"
-        ```
-        
-        This will create a project called `schoolsite` now cd into the `schoolsite` directory, if you do `ls` within the directory you just enter you will see a module called `thunder.py` and some directories (some in the form of package) `media`, `static`, `templates` and a directory with the same name of your base directory name, in our case it is `schoolsite`.
-        
-        Boot up the flask server by running the below command
-        
-        ```
-        python thunder.py boot
-        ```
-        
-        Now visit the local url `http://127.0.0.1:5000` this will show you index page of your project
-        
-        ## Create flask app within your project (schoolsite)
-        
-        For you to start an app within your project `schoolsite` shutdown the flask development server by pressing ( CTRL+C ) and then run the following command, by giving the name you want your app to be, in our case we will call our app `exam`
-        
-        ```
-        python thunder.py create_app -a exam
-        ```
-        
-        this will create an app (a new package called `exam`) within your project `(schoolsite)`
-        
-        ## Register an app
-        
-        Once the app is created open a file `schoolsite/routes.py` and import your `exam` blueprint which is in (`exam/views.py`), default name given to an app blueprint, is the app name so our `exam` app blueprint name is `exam`, after importing it, append (register) the app blueprint in a list called `reg_blueprints` in that same file of `schoolsite/routes.py`
-        
-        importing blueprint
-        
-        ```py
-        from exam.views import exam
-        ```
-        
-        registering blueprint
-        
-        ```py
-        reg_blueprints = [
-          blueprint.default,
-          blueprint.errors,
-          blueprint.auth,
-          base,
-          exam,
-        ]
-        ```
-        
-        once you register the app, boot up the flask webserver again by
-        
-        ```
-        python thunder.py boot
-        ```
-        
-        visit `http://127.0.0.1:5000` which is your project landing page
-        
-        visit `http://127.0.0.1:5000/exam` this will take you to your app landing page (exam)
-        
-        visit `http://127.0.0.1:5000/admin` this will take you to admin page. From there you are ready to go.
-        
-        See more documentations <a href="https://sakyum.readthedocs.io">here!</a>
-        
-        ### Sakyum default page
-        
-        ![Sakyum default page](./media/sakyum_default_page.png)
-        
-        ## Useful links
-        
-        - Documentation: https://sakyum.readthedocs.io
-        - Repository: https://github.com/usmanmusa1920/sakyum
-        - Docker example: https://github.com/usmanmusa1920/sakyum/tree/master/example/sakyum-docker
-        
-        Pull requests are welcome
-        
-        
-        Change Log
-        ==========
-        
-        0.0.8 (09/june/2023)
-        ------------------
-        - Eight Release
-        
-        OS compatibility
-        
-        Making sakyum to be compatible with windows OS as well as other OS
-        
-        0.0.7 (4/april/2023)
-        ------------------
-        - Seventh Release
-        
-        This release mostly is for adding more docs and examples.
-        
-        - Sixth Release
-        
-        Alembic is included as dependency (in the require module list).
-        
-        - Fifth Release
-        
-        In fifith release, we handle how default user file system tricks is, things like when user change his profile picture.
-        
-        - Fourth Release
-        
-        In this release we handle how we can customise the admin html page by inheriting (extends) it in our project templates/admin directory, and the admin page on how to bind models in the admin. Also I refactor other libraries that this package needs with their corresponding versions in the setup.py and requirements.txt files. In this release good documentations is well packed.
-        
-        Database migration is added using `alembic`
-        
-        Some error pages, default page were added but still you can customise it in your project sub folder (the package with the same name of your project in your project directory) in a file called `route.py`. Also an admin directory within your project templates folder is added too!
-        
-        Possibly other well things are added which include auth system for `users` and more.
-        
 Keywords: sakyum
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -145,7 +20,139 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# Sakyum
+
+An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs.
+
+## Installation
+
+Install and update the latest release from <a href="https://pypi.org/project/sakyum">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) as from `v0.0.9` it is now compatible and also tested with `windows OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
+
+```
+pip install --upgrade sakyum
+```
+
+## Create flask project using sakyum
+
+After the installation paste the following command on your termianl
+
+```
+python -c "from sakyum import project; project('schoolsite')"
+```
+
+This will create a project called `schoolsite` now cd into the `schoolsite` directory, if you do `ls` within the directory you just enter you will see a module called `thunder.py` and some directories (some in the form of package) `media`, `static`, `templates` and a directory with the same name of your base directory name, in our case it is `schoolsite`.
+
+Boot up the flask server by running the below command
+
+```
+python thunder.py boot
+```
+
+Now visit the local url `http://127.0.0.1:5000` this will show you index page of your project
+
+## Create flask app within your project (schoolsite)
+
+For you to start an app within your project `schoolsite` shutdown the flask development server by pressing ( CTRL+C ) and then run the following command, by giving the name you want your app to be, in our case we will call our app `exam`
+
+```
+python thunder.py create_app -a exam
+```
+
+this will create an app (a new package called `exam`) within your project `(schoolsite)`
+
+## Register an app
+
+Once the app is created open a file `schoolsite/routes.py` and import your `exam` blueprint which is in (`exam/views.py`), default name given to an app blueprint, is the app name so our `exam` app blueprint name is `exam`, after importing it, append (register) the app blueprint in a list called `reg_blueprints` in that same file of `schoolsite/routes.py`
+
+importing blueprint
+
+```py
+from exam.views import exam
+```
+
+registering blueprint
+
+```py
+reg_blueprints = [
+  blueprint.default,
+  blueprint.errors,
+  blueprint.auth,
+  base,
+  exam,
+]
+```
+
+once you register the app, boot up the flask webserver again by
+
+```
+python thunder.py boot
+```
+
+visit `http://127.0.0.1:5000` which is your project landing page
+
+visit `http://127.0.0.1:5000/exam` this will take you to your app landing page (exam)
+
+visit `http://127.0.0.1:5000/admin` this will take you to admin page. From there you are ready to go.
+
+See more documentations <a href="https://sakyum.readthedocs.io">here!</a>
+
+### Sakyum default page
+
+![Sakyum default page](sakyum_default_page.png)
+
+## Useful links
+
+- Documentation: https://sakyum.readthedocs.io
+- Repository: https://github.com/usmanmusa1920/sakyum
+- Docker example: https://github.com/usmanmusa1920/sakyum/tree/master/example/sakyum-docker
+
+Pull requests are welcome
+
+
+Change Log
+==========
+
+0.0.9 (22/june/2023)
+------------------
+- Nineth Release
+
+Fixing bugs
+
+Fixing v0.0.8 bugs for OS compatibility, and also tested on windows OS
+
+- Eight Release
+
+OS compatibility
+
+Making sakyum to be compatible with windows OS as well as other OS
+
+0.0.7 (4/april/2023)
+------------------
+- Seventh Release
+
+This release mostly is for adding more docs and examples.
+
+- Sixth Release
+
+Alembic is included as dependency (in the require module list).
+
+- Fifth Release
+
+In fifith release, we handle how default user file system tricks is, things like when user change his profile picture.
+
+- Fourth Release
+
+In this release we handle how we can customise the admin html page by inheriting (extends) it in our project templates/admin directory, and the admin page on how to bind models in the admin. Also I refactor other libraries that this package needs with their corresponding versions in the setup.py and requirements.txt files. In this release good documentations is well packed.
+
+Database migration is added using `alembic`
+
+Some error pages, default page were added but still you can customise it in your project sub folder (the package with the same name of your project in your project directory) in a file called `route.py`. Also an admin directory within your project templates folder is added too!
+
+Possibly other well things are added which include auth system for `users` and more.
```

#### html2text {}

```diff
@@ -1,70 +1,71 @@
-Metadata-Version: 2.1 Name: sakyum Version: 0.0.8 Summary: An extension of
+Metadata-Version: 2.1 Name: sakyum Version: 0.0.9 Summary: An extension of
 flask web framework that erase the complexity of structuring flask project
 blueprint, packages, and other annoying stuffs Home-page: https://
-sakyum.readthedocs.io Author: Usman Musa Author-email: usmanmusa1920@gmail.com
-License: MIT Download-URL: https://pypi.org/project/sakyum Project-URL:
+sakyum.readthedocs.io Download-URL: https://pypi.org/project/sakyum Author:
+Usman Musa Author-email: usmanmusa1920@gmail.com License: MIT Project-URL:
 Documentation, https://sakyum.readthedocs.io Project-URL: Source, https://
-github.com/usmanmusa1920/sakyum Description: # Sakyum An extension of flask web
-framework that erase the complexity of structuring flask project blueprint,
-packages, and other annoying stuffs. ## Installation Install and update the
-latest release from pypi. Basically the library was uploaded using `sdist`
-(Source Distribution) and this software (library) as from `v0.0.8` it is now
-compatible with `windows OS` and others as well, such as `linux`, `macOS` and
-possibly some others too!. ``` pip install --upgrade sakyum ``` ## Create flask
-project using sakyum After the installation paste the following command on your
-termianl ``` python -c "from sakyum import project; project('schoolsite')" ```
-This will create a project called `schoolsite` now cd into the `schoolsite`
-directory, if you do `ls` within the directory you just enter you will see a
-module called `thunder.py` and some directories (some in the form of package)
-`media`, `static`, `templates` and a directory with the same name of your base
-directory name, in our case it is `schoolsite`. Boot up the flask server by
-running the below command ``` python thunder.py boot ``` Now visit the local
-url `http://127.0.0.1:5000` this will show you index page of your project ##
-Create flask app within your project (schoolsite) For you to start an app
-within your project `schoolsite` shutdown the flask development server by
-pressing ( CTRL+C ) and then run the following command, by giving the name you
-want your app to be, in our case we will call our app `exam` ``` python
-thunder.py create_app -a exam ``` this will create an app (a new package called
-`exam`) within your project `(schoolsite)` ## Register an app Once the app is
-created open a file `schoolsite/routes.py` and import your `exam` blueprint
-which is in (`exam/views.py`), default name given to an app blueprint, is the
-app name so our `exam` app blueprint name is `exam`, after importing it, append
-(register) the app blueprint in a list called `reg_blueprints` in that same
-file of `schoolsite/routes.py` importing blueprint ```py from exam.views import
-exam ``` registering blueprint ```py reg_blueprints = [ blueprint.default,
+github.com/usmanmusa1920/sakyum Keywords: sakyum Platform: any Classifier:
+Development Status :: 5 - Production/Stable Classifier: Environment :: Web
+Environment Classifier: Intended Audience :: Developers Classifier: Natural
+Language :: English Classifier: Operating System :: OS Independent Classifier:
+License :: OSI Approved :: MIT License Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Programming Language ::
+Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE # Sakyum An extension of flask web framework that erase the complexity
+of structuring flask project blueprint, packages, and other annoying stuffs. ##
+Installation Install and update the latest release from pypi. Basically the
+library was uploaded using `sdist` (Source Distribution) and this software
+(library) as from `v0.0.9` it is now compatible and also tested with `windows
+OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
+``` pip install --upgrade sakyum ``` ## Create flask project using sakyum After
+the installation paste the following command on your termianl ``` python -
+c "from sakyum import project; project('schoolsite')" ``` This will create a
+project called `schoolsite` now cd into the `schoolsite` directory, if you do
+`ls` within the directory you just enter you will see a module called
+`thunder.py` and some directories (some in the form of package) `media`,
+`static`, `templates` and a directory with the same name of your base directory
+name, in our case it is `schoolsite`. Boot up the flask server by running the
+below command ``` python thunder.py boot ``` Now visit the local url `http://
+127.0.0.1:5000` this will show you index page of your project ## Create flask
+app within your project (schoolsite) For you to start an app within your
+project `schoolsite` shutdown the flask development server by pressing ( CTRL+C
+) and then run the following command, by giving the name you want your app to
+be, in our case we will call our app `exam` ``` python thunder.py create_app -
+a exam ``` this will create an app (a new package called `exam`) within your
+project `(schoolsite)` ## Register an app Once the app is created open a file
+`schoolsite/routes.py` and import your `exam` blueprint which is in (`exam/
+views.py`), default name given to an app blueprint, is the app name so our
+`exam` app blueprint name is `exam`, after importing it, append (register) the
+app blueprint in a list called `reg_blueprints` in that same file of
+`schoolsite/routes.py` importing blueprint ```py from exam.views import exam
+``` registering blueprint ```py reg_blueprints = [ blueprint.default,
 blueprint.errors, blueprint.auth, base, exam, ] ``` once you register the app,
 boot up the flask webserver again by ``` python thunder.py boot ``` visit
 `http://127.0.0.1:5000` which is your project landing page visit `http://
 127.0.0.1:5000/exam` this will take you to your app landing page (exam) visit
 `http://127.0.0.1:5000/admin` this will take you to admin page. From there you
 are ready to go. See more documentations here! ### Sakyum default page ![Sakyum
-default page](./media/sakyum_default_page.png) ## Useful links - Documentation:
-https://sakyum.readthedocs.io - Repository: https://github.com/usmanmusa1920/
-sakyum - Docker example: https://github.com/usmanmusa1920/sakyum/tree/master/
-example/sakyum-docker Pull requests are welcome Change Log ========== 0.0.8
-(09/june/2023) ------------------ - Eight Release OS compatibility Making
-sakyum to be compatible with windows OS as well as other OS 0.0.7 (4/april/
-2023) ------------------ - Seventh Release This release mostly is for adding
-more docs and examples. - Sixth Release Alembic is included as dependency (in
-the require module list). - Fifth Release In fifith release, we handle how
-default user file system tricks is, things like when user change his profile
-picture. - Fourth Release In this release we handle how we can customise the
-admin html page by inheriting (extends) it in our project templates/admin
-directory, and the admin page on how to bind models in the admin. Also I
-refactor other libraries that this package needs with their corresponding
-versions in the setup.py and requirements.txt files. In this release good
-documentations is well packed. Database migration is added using `alembic` Some
-error pages, default page were added but still you can customise it in your
-project sub folder (the package with the same name of your project in your
-project directory) in a file called `route.py`. Also an admin directory within
-your project templates folder is added too! Possibly other well things are
-added which include auth system for `users` and more. Keywords: sakyum
-Platform: any Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment Classifier: Intended Audience ::
-Developers Classifier: Natural Language :: English Classifier: Operating System
-:: OS Independent Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.6 Description-
-Content-Type: text/markdown
+default page](sakyum_default_page.png) ## Useful links - Documentation: https:/
+/sakyum.readthedocs.io - Repository: https://github.com/usmanmusa1920/sakyum -
+Docker example: https://github.com/usmanmusa1920/sakyum/tree/master/example/
+sakyum-docker Pull requests are welcome Change Log ========== 0.0.9 (22/june/
+2023) ------------------ - Nineth Release Fixing bugs Fixing v0.0.8 bugs for OS
+compatibility, and also tested on windows OS - Eight Release OS compatibility
+Making sakyum to be compatible with windows OS as well as other OS 0.0.7 (4/
+april/2023) ------------------ - Seventh Release This release mostly is for
+adding more docs and examples. - Sixth Release Alembic is included as
+dependency (in the require module list). - Fifth Release In fifith release, we
+handle how default user file system tricks is, things like when user change his
+profile picture. - Fourth Release In this release we handle how we can
+customise the admin html page by inheriting (extends) it in our project
+templates/admin directory, and the admin page on how to bind models in the
+admin. Also I refactor other libraries that this package needs with their
+corresponding versions in the setup.py and requirements.txt files. In this
+release good documentations is well packed. Database migration is added using
+`alembic` Some error pages, default page were added but still you can customise
+it in your project sub folder (the package with the same name of your project
+in your project directory) in a file called `route.py`. Also an admin directory
+within your project templates folder is added too! Possibly other well things
+are added which include auth system for `users` and more.
```

### Comparing `sakyum-0.0.8/README.md` & `sakyum-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 # Sakyum
 
 An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs.
 
 ## Installation
 
-Install and update the latest release from <a href="https://pypi.org/project/sakyum">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) as from `v0.0.8` it is now compatible with `windows OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
+Install and update the latest release from <a href="https://pypi.org/project/sakyum">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) as from `v0.0.9` it is now compatible and also tested with `windows OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
 
 ```
 pip install --upgrade sakyum
 ```
 
 ## Create flask project using sakyum
 
@@ -73,15 +73,15 @@
 
 visit `http://127.0.0.1:5000/admin` this will take you to admin page. From there you are ready to go.
 
 See more documentations <a href="https://sakyum.readthedocs.io">here!</a>
 
 ### Sakyum default page
 
-![Sakyum default page](./media/sakyum_default_page.png)
+![Sakyum default page](sakyum_default_page.png)
 
 ## Useful links
 
 - Documentation: https://sakyum.readthedocs.io
 - Repository: https://github.com/usmanmusa1920/sakyum
 - Docker example: https://github.com/usmanmusa1920/sakyum/tree/master/example/sakyum-docker
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
  # Sakyum An extension of flask web framework that erase the complexity of
 structuring flask project blueprint, packages, and other annoying stuffs. ##
 Installation Install and update the latest release from pypi. Basically the
 library was uploaded using `sdist` (Source Distribution) and this software
-(library) as from `v0.0.8` it is now compatible with `windows OS` and others as
-well, such as `linux`, `macOS` and possibly some others too!. ``` pip install -
--upgrade sakyum ``` ## Create flask project using sakyum After the installation
-paste the following command on your termianl ``` python -c "from sakyum import
-project; project('schoolsite')" ``` This will create a project called
-`schoolsite` now cd into the `schoolsite` directory, if you do `ls` within the
-directory you just enter you will see a module called `thunder.py` and some
-directories (some in the form of package) `media`, `static`, `templates` and a
-directory with the same name of your base directory name, in our case it is
-`schoolsite`. Boot up the flask server by running the below command ``` python
-thunder.py boot ``` Now visit the local url `http://127.0.0.1:5000` this will
-show you index page of your project ## Create flask app within your project
-(schoolsite) For you to start an app within your project `schoolsite` shutdown
-the flask development server by pressing ( CTRL+C ) and then run the following
-command, by giving the name you want your app to be, in our case we will call
-our app `exam` ``` python thunder.py create_app -a exam ``` this will create an
-app (a new package called `exam`) within your project `(schoolsite)` ##
-Register an app Once the app is created open a file `schoolsite/routes.py` and
-import your `exam` blueprint which is in (`exam/views.py`), default name given
-to an app blueprint, is the app name so our `exam` app blueprint name is
-`exam`, after importing it, append (register) the app blueprint in a list
-called `reg_blueprints` in that same file of `schoolsite/routes.py` importing
-blueprint ```py from exam.views import exam ``` registering blueprint ```py
-reg_blueprints = [ blueprint.default, blueprint.errors, blueprint.auth, base,
-exam, ] ``` once you register the app, boot up the flask webserver again by ```
-python thunder.py boot ``` visit `http://127.0.0.1:5000` which is your project
-landing page visit `http://127.0.0.1:5000/exam` this will take you to your app
-landing page (exam) visit `http://127.0.0.1:5000/admin` this will take you to
-admin page. From there you are ready to go. See more documentations here! ###
-Sakyum default page ![Sakyum default page](./media/sakyum_default_page.png) ##
-Useful links - Documentation: https://sakyum.readthedocs.io - Repository:
-https://github.com/usmanmusa1920/sakyum - Docker example: https://github.com/
-usmanmusa1920/sakyum/tree/master/example/sakyum-docker Pull requests are
-welcome
+(library) as from `v0.0.9` it is now compatible and also tested with `windows
+OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
+``` pip install --upgrade sakyum ``` ## Create flask project using sakyum After
+the installation paste the following command on your termianl ``` python -
+c "from sakyum import project; project('schoolsite')" ``` This will create a
+project called `schoolsite` now cd into the `schoolsite` directory, if you do
+`ls` within the directory you just enter you will see a module called
+`thunder.py` and some directories (some in the form of package) `media`,
+`static`, `templates` and a directory with the same name of your base directory
+name, in our case it is `schoolsite`. Boot up the flask server by running the
+below command ``` python thunder.py boot ``` Now visit the local url `http://
+127.0.0.1:5000` this will show you index page of your project ## Create flask
+app within your project (schoolsite) For you to start an app within your
+project `schoolsite` shutdown the flask development server by pressing ( CTRL+C
+) and then run the following command, by giving the name you want your app to
+be, in our case we will call our app `exam` ``` python thunder.py create_app -
+a exam ``` this will create an app (a new package called `exam`) within your
+project `(schoolsite)` ## Register an app Once the app is created open a file
+`schoolsite/routes.py` and import your `exam` blueprint which is in (`exam/
+views.py`), default name given to an app blueprint, is the app name so our
+`exam` app blueprint name is `exam`, after importing it, append (register) the
+app blueprint in a list called `reg_blueprints` in that same file of
+`schoolsite/routes.py` importing blueprint ```py from exam.views import exam
+``` registering blueprint ```py reg_blueprints = [ blueprint.default,
+blueprint.errors, blueprint.auth, base, exam, ] ``` once you register the app,
+boot up the flask webserver again by ``` python thunder.py boot ``` visit
+`http://127.0.0.1:5000` which is your project landing page visit `http://
+127.0.0.1:5000/exam` this will take you to your app landing page (exam) visit
+`http://127.0.0.1:5000/admin` this will take you to admin page. From there you
+are ready to go. See more documentations here! ### Sakyum default page ![Sakyum
+default page](sakyum_default_page.png) ## Useful links - Documentation: https:/
+/sakyum.readthedocs.io - Repository: https://github.com/usmanmusa1920/sakyum -
+Docker example: https://github.com/usmanmusa1920/sakyum/tree/master/example/
+sakyum-docker Pull requests are welcome
```

### Comparing `sakyum-0.0.8/sakyum/__init__.py` & `sakyum-0.0.9/sakyum/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   /_/ /  | /  | / /__/ /      |
   
   An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs
 """
 
 
 __title__ = 'sakyum'
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 __author__ = 'Usman Musa'
 __author_email__ = 'usmanmusa1920@gmail.com'
 __author_website__ = 'https://usmanmusa1920.github.io'
 __repository__ = 'https://github.com/usmanmusa1920/sakyum'
 __url__ = 'https://sakyum.readthedocs.io'
 __copyright__ = 'Copyright (C) 2022 - 2023 Usman Musa'
```

### Comparing `sakyum-0.0.8/sakyum/auth/admin.py` & `sakyum-0.0.9/sakyum/auth/admin.py`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/auth/forms.py` & `sakyum-0.0.9/sakyum/auth/forms.py`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/auth/models.py` & `sakyum-0.0.9/sakyum/auth/models.py`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/auth/routes.py` & `sakyum-0.0.9/sakyum/auth/routes.py`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/base.py` & `sakyum-0.0.9/sakyum/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,31 +33,51 @@
   DEBUG     ---  10
   INFO      ---  20
   WARNING   ---  30  (default)
   ERROR     ---  40
   CRITICAL  ---  50
 """
 
-formatter = '[+] [%(asctime)s] [%(levelname)s] %(message)s'
-logging.basicConfig(format = formatter)
+FORMATTER = '[+] [%(asctime)s] [%(levelname)s] %(message)s'
+logging.basicConfig(format = FORMATTER)
 LOGGER = logging.getLogger(__name__)
 LOGGER.setLevel(logging.DEBUG)
 
 # used for relative path to default image to copy for a project (only)
 ORIGIN = Path(__file__).resolve().parent
 OS_SEP = os.path.sep # platform-specific path separator (for linux `/`, for windows `\\`)
 
 
 class BaseStructure:
   """base structure class"""
 
   def __init__(self, is_software=True):
     """base structure class initializer"""
     self.is_software = is_software
-    self.fls_cmd = 'touch'
+
+    # we can use any of the below three variables to make our code compatible with
+    # many OS, but we go with the first one which is `self.os_name`
+    self.os_name = os.name # nt or posix
+    self.platform_name_1 = sys.platform # win32 or linux or darwin or android
+    self.platform_name_2 = platform.system() # Windows, Darwin, Linux, etc.
+
+    if self.os_name == 'nt':
+    # if self.platform_name_1 == 'win32':
+    # if self.platform_name_2 == 'Windows':
+      self.fls_cmd = 'echo >'
+    elif self.os_name == 'posix':
+    # elif self.platform_name_1 == 'linux' or self.platform_name_1 == 'darwin' or self.platform_name_1 == 'android':
+    # elif self.platform_name_2 == 'Linux' or self.platform_name_2 == 'Darwin':
+      self.fls_cmd = 'touch'
+    else:
+      err_compt = f'{__title__.capitalize()} v{__version__} is not compatible with your OS'
+      print()
+      LOGGER.error(err_compt)
+      print()
+      exit()
     self._exs_first = ['index', 'style']
     self._exs_last = ['.html', '.css', '.js']
     
 
   def append_exs_to_file(self, fls_name=False, _exs_='.py', name=None):
     """
     append .py extension for files if _exs_ value is '.py' or type is str, else if _exs_ type is list, make list of static files `['index.html', 'index.js', 'style.css']`
@@ -105,30 +125,20 @@
       img_write.write(img_read_data)
       
 
   def file_opt(self, _dir, tree=True, _here=False, _where=False):
     """
     make dir tree if `tree=True` and get into it, if `_here` or `_where` is equal to True
     """
-
-    # we can use any of the below three variables to make our code compatible with many OS
-    os_name = os.name # nt or posix
-    platform_name_1 = sys.platform # win32 or linux or darwin or android
-    platform_name_2 = platform.system() # Windows, Darwin, Linux, etc.
-
     if tree:
-      if os_name == 'nt':
-      # if platform_name_1 == 'win32':
-      # if platform_name_2 == 'Windows':
+      if self.os_name == 'nt':
         os.makedirs(_dir, exist_ok=True)
         # The exist_ok=True argument ensures that the function
         # does not raise an exception if the directory already exists.
-      elif os_name == 'posix':
-      # elif platform_name_1 == 'linux' or platform_name_1 == 'darwin' or platform_name_1 == 'android':
-      # elif platform_name_2 == 'Linux' or platform_name_2 == 'Darwin':
+      elif self.os_name == 'posix':
         sp.run(['mkdir', '-p', _dir])
       else:
         err_compt = f'{__title__.capitalize()} v{__version__} is not compatible with your OS'
         print()
         LOGGER.error(err_compt)
         print()
         exit()
@@ -159,15 +169,24 @@
     is_app: if it is True, that mean it will do operation of making app files,
     else it will make for the entire project
     """
     
     if is_app:
       for _fls in fls:
         app_name = os.getcwd().split(OS_SEP)[-1]
-        sp.run(shlex.split(f'{fls_cmd} {_fls}'))
+        if self.os_name == 'nt':
+          sp.run(shlex.split(f'{fls_cmd} {_fls}'), shell=True)
+        elif self.os_name == 'posix':
+          sp.run(shlex.split(f'{fls_cmd} {_fls}'))
+        else:
+          err_compt = f'{__title__.capitalize()} v{__version__} is not compatible with your OS'
+          print()
+          LOGGER.error(err_compt)
+          print()
+          exit()
         if is_static_file:
           # building app default files (html, css, js)
           self.file_content(file_name=_fls, content=f'{app_default_dummy}', route_go=False)
         else:
           # building app default files (__init__.py, admin.py, forms.py, models.py, views.py)
           if _fls == '__init__.py':
             self.file_content(file_name=_fls, content=f'# from {__title__} software, your app ({app_name}) {_fls} file\n{app_init_dummy()}', route_go=False)
@@ -178,15 +197,24 @@
           elif _fls == 'models.py':
             self.file_content(file_name=_fls, content=f'# from {__title__} software, your app ({app_name}) {_fls} file\n{app_models_dummy()}', route_go=False)
           elif _fls == 'views.py':
             self.file_content(file_name=_fls, content=f'# from {__title__} software, your app ({app_name}) {_fls} file\n{app_views_dummy(app_name)}', route_go=False)
     else:
       for _fls in fls:
         if _fls[:-3] == file:
-          sp.run(shlex.split(f'{fls_cmd} {_fls}'))
+          if self.os_name == 'nt':
+            sp.run(shlex.split(f'{fls_cmd} {_fls}'), shell=True)
+          elif self.os_name == 'posix':
+            sp.run(shlex.split(f'{fls_cmd} {_fls}'))
+          else:
+            err_compt = f'{__title__.capitalize()} v{__version__} is not compatible with your OS'
+            print()
+            LOGGER.error(err_compt)
+            print()
+            exit()
           self.file_content(
             file_name=_fls,content=f'# Your project {_fls} file\n{thunder_dummy(proj_nm)}', route_go=False
             ) # building the run module `thunder.py`
             
 
   def dir_tree(self, proj_name=None):
     """
@@ -209,15 +237,24 @@
       # making directories trees and their default files in the loop
       for _dir in dirs:
         if _dir == dirs[0] + OS_SEP + dirs[0]:
           self.file_opt(_dir, _here=_here)
           # create default modules inside project sub dir
           for _fls in fls:
             if _fls[:-3] != 'thunder':
-              sp.run(shlex.split(f'{self.fls_cmd} {_fls}'))
+              if self.os_name == 'nt':
+                sp.run(shlex.split(f'{self.fls_cmd} {_fls}'), shell=True)
+              elif self.os_name == 'posix':
+                sp.run(shlex.split(f'{self.fls_cmd} {_fls}'))
+              else:
+                err_compt = f'{__title__.capitalize()} v{__version__} is not compatible with your OS'
+                print()
+                LOGGER.error(err_compt)
+                print()
+                exit()
               # building project default files (__init__.py, config.py, routes.py, secret.py)
               if _fls == '__init__.py':
                 self.file_content(file_name=_fls, content=f'# from {__title__} software, your ({proj_name}) project {_fls} file\n{pro_init_dummy()}', route_go=False)
               elif _fls == 'config.py':
                 self.file_content(file_name=_fls, content=f'# from {__title__} software, your ({proj_name}) project {_fls} file\n{pro_config_dummy(proj_name)}', route_go=False)
               elif _fls == 'routes.py':
                 self.file_content(file_name=_fls, content=f'# from {__title__} software, your ({proj_name}) project {_fls} file\n{pro_routes_dummy(proj_name)}', route_go=False)
```

### Comparing `sakyum-0.0.8/sakyum/blueprint.py` & `sakyum-0.0.9/sakyum/blueprint.py`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/contrib/__init__.py` & `sakyum-0.0.9/sakyum/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/mute/__init__.py` & `sakyum-0.0.9/sakyum/mute/__init__.py`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/mute/app.py` & `sakyum-0.0.9/sakyum/mute/app.py`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/mute/page.py` & `sakyum-0.0.9/sakyum/mute/page.py`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/mute/project.py` & `sakyum-0.0.9/sakyum/mute/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ORIGIN_PATH = Path(__file__).resolve().parent.parent
 OS_SEP = os.path.sep # platform-specific path separator (for linux `/`, for windows `\\`)
 
 
 class Config:
   SECRET_KEY = '{secure_app}'
   # The `SQLALCHEMY_DATABASE_URI` might not be compatible with windows OS,
-  # change it to your windows drive like: 'C:\path\to\your\default.db'
+  # change it to your windows drive like: 'C:\path\to\your\default.db' (if you encounter an error)
   SQLALCHEMY_DATABASE_URI = 'sqlite:///'+str(ORIGIN_PATH)+OS_SEP+'default.db'
   # set optional bootswatch theme
   FLASK_ADMIN_SWATCH = 'cerulean'
   UPLOAD_FOLDER = os.path.join(ORIGIN_PATH, 'media')
   ALLOWED_EXTENSIONS = ('png', 'jpg', 'jpeg')
   MAX_CONTENT_LENGTH = 16 * 1024 * 1024
```

### Comparing `sakyum-0.0.8/sakyum/static/default_style/css/style.css` & `sakyum-0.0.9/sakyum/static/default_style/css/style.css`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/static/default_style/media/alert.png` & `sakyum-0.0.9/sakyum/static/default_style/media/alert.png`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/static/default_style/media/default_img.png` & `sakyum-0.0.9/sakyum/static/default_style/media/default_img.png`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/static/default_style/media/favicon.ico` & `sakyum-0.0.9/sakyum/static/default_style/media/favicon.ico`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/templates/default_page/admin_change_password.html` & `sakyum-0.0.9/sakyum/templates/default_page/admin_change_password.html`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/templates/default_page/admin_change_profile_image.html` & `sakyum-0.0.9/sakyum/templates/default_page/admin_change_profile_image.html`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/templates/default_page/admin_login.html` & `sakyum-0.0.9/sakyum/templates/default_page/admin_login.html`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/templates/default_page/admin_register.html` & `sakyum-0.0.9/sakyum/templates/default_page/admin_register.html`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/templates/default_page/default.html` & `sakyum-0.0.9/sakyum/templates/default_page/default.html`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/templates/default_page/default_base.html` & `sakyum-0.0.9/sakyum/templates/default_page/default_base.html`

 * *Files identical despite different names*

### Comparing `sakyum-0.0.8/sakyum/utils.py` & `sakyum-0.0.9/sakyum/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
   desc_center = desc.center(len(desc) + 6)
   border = '=' * len(desc_center)
   return [desc_center, border]
   
   
 # Style for sakyum default pages:
     # ============================
-    #  @ sakyum software - v0.0.8 
+    #  @ sakyum software - v0.0.9 
     # ============================
 footer_style = stylePage(__title__, version=__version__)
 
 
 def rem_blueprint(lst_blue=None, rem_blue=None):
   # these are blueprint that we don't want to show on the
   # default page so we are removing them from the list
```

### Comparing `sakyum-0.0.8/sakyum.egg-info/PKG-INFO` & `sakyum-0.0.9/sakyum.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,143 +1,18 @@
 Metadata-Version: 2.1
 Name: sakyum
-Version: 0.0.8
+Version: 0.0.9
 Summary: An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs
 Home-page: https://sakyum.readthedocs.io
+Download-URL: https://pypi.org/project/sakyum
 Author: Usman Musa
 Author-email: usmanmusa1920@gmail.com
 License: MIT
-Download-URL: https://pypi.org/project/sakyum
 Project-URL: Documentation, https://sakyum.readthedocs.io
 Project-URL: Source, https://github.com/usmanmusa1920/sakyum
-Description: 
-        # Sakyum
-        
-        An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs.
-        
-        ## Installation
-        
-        Install and update the latest release from <a href="https://pypi.org/project/sakyum">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) as from `v0.0.8` it is now compatible with `windows OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
-        
-        ```
-        pip install --upgrade sakyum
-        ```
-        
-        ## Create flask project using sakyum
-        
-        After the installation paste the following command on your termianl
-        
-        ```
-        python -c "from sakyum import project; project('schoolsite')"
-        ```
-        
-        This will create a project called `schoolsite` now cd into the `schoolsite` directory, if you do `ls` within the directory you just enter you will see a module called `thunder.py` and some directories (some in the form of package) `media`, `static`, `templates` and a directory with the same name of your base directory name, in our case it is `schoolsite`.
-        
-        Boot up the flask server by running the below command
-        
-        ```
-        python thunder.py boot
-        ```
-        
-        Now visit the local url `http://127.0.0.1:5000` this will show you index page of your project
-        
-        ## Create flask app within your project (schoolsite)
-        
-        For you to start an app within your project `schoolsite` shutdown the flask development server by pressing ( CTRL+C ) and then run the following command, by giving the name you want your app to be, in our case we will call our app `exam`
-        
-        ```
-        python thunder.py create_app -a exam
-        ```
-        
-        this will create an app (a new package called `exam`) within your project `(schoolsite)`
-        
-        ## Register an app
-        
-        Once the app is created open a file `schoolsite/routes.py` and import your `exam` blueprint which is in (`exam/views.py`), default name given to an app blueprint, is the app name so our `exam` app blueprint name is `exam`, after importing it, append (register) the app blueprint in a list called `reg_blueprints` in that same file of `schoolsite/routes.py`
-        
-        importing blueprint
-        
-        ```py
-        from exam.views import exam
-        ```
-        
-        registering blueprint
-        
-        ```py
-        reg_blueprints = [
-          blueprint.default,
-          blueprint.errors,
-          blueprint.auth,
-          base,
-          exam,
-        ]
-        ```
-        
-        once you register the app, boot up the flask webserver again by
-        
-        ```
-        python thunder.py boot
-        ```
-        
-        visit `http://127.0.0.1:5000` which is your project landing page
-        
-        visit `http://127.0.0.1:5000/exam` this will take you to your app landing page (exam)
-        
-        visit `http://127.0.0.1:5000/admin` this will take you to admin page. From there you are ready to go.
-        
-        See more documentations <a href="https://sakyum.readthedocs.io">here!</a>
-        
-        ### Sakyum default page
-        
-        ![Sakyum default page](./media/sakyum_default_page.png)
-        
-        ## Useful links
-        
-        - Documentation: https://sakyum.readthedocs.io
-        - Repository: https://github.com/usmanmusa1920/sakyum
-        - Docker example: https://github.com/usmanmusa1920/sakyum/tree/master/example/sakyum-docker
-        
-        Pull requests are welcome
-        
-        
-        Change Log
-        ==========
-        
-        0.0.8 (09/june/2023)
-        ------------------
-        - Eight Release
-        
-        OS compatibility
-        
-        Making sakyum to be compatible with windows OS as well as other OS
-        
-        0.0.7 (4/april/2023)
-        ------------------
-        - Seventh Release
-        
-        This release mostly is for adding more docs and examples.
-        
-        - Sixth Release
-        
-        Alembic is included as dependency (in the require module list).
-        
-        - Fifth Release
-        
-        In fifith release, we handle how default user file system tricks is, things like when user change his profile picture.
-        
-        - Fourth Release
-        
-        In this release we handle how we can customise the admin html page by inheriting (extends) it in our project templates/admin directory, and the admin page on how to bind models in the admin. Also I refactor other libraries that this package needs with their corresponding versions in the setup.py and requirements.txt files. In this release good documentations is well packed.
-        
-        Database migration is added using `alembic`
-        
-        Some error pages, default page were added but still you can customise it in your project sub folder (the package with the same name of your project in your project directory) in a file called `route.py`. Also an admin directory within your project templates folder is added too!
-        
-        Possibly other well things are added which include auth system for `users` and more.
-        
 Keywords: sakyum
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -145,7 +20,139 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# Sakyum
+
+An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs.
+
+## Installation
+
+Install and update the latest release from <a href="https://pypi.org/project/sakyum">pypi</a>. Basically the library was uploaded using `sdist` (Source Distribution) and this software (library) as from `v0.0.9` it is now compatible and also tested with `windows OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
+
+```
+pip install --upgrade sakyum
+```
+
+## Create flask project using sakyum
+
+After the installation paste the following command on your termianl
+
+```
+python -c "from sakyum import project; project('schoolsite')"
+```
+
+This will create a project called `schoolsite` now cd into the `schoolsite` directory, if you do `ls` within the directory you just enter you will see a module called `thunder.py` and some directories (some in the form of package) `media`, `static`, `templates` and a directory with the same name of your base directory name, in our case it is `schoolsite`.
+
+Boot up the flask server by running the below command
+
+```
+python thunder.py boot
+```
+
+Now visit the local url `http://127.0.0.1:5000` this will show you index page of your project
+
+## Create flask app within your project (schoolsite)
+
+For you to start an app within your project `schoolsite` shutdown the flask development server by pressing ( CTRL+C ) and then run the following command, by giving the name you want your app to be, in our case we will call our app `exam`
+
+```
+python thunder.py create_app -a exam
+```
+
+this will create an app (a new package called `exam`) within your project `(schoolsite)`
+
+## Register an app
+
+Once the app is created open a file `schoolsite/routes.py` and import your `exam` blueprint which is in (`exam/views.py`), default name given to an app blueprint, is the app name so our `exam` app blueprint name is `exam`, after importing it, append (register) the app blueprint in a list called `reg_blueprints` in that same file of `schoolsite/routes.py`
+
+importing blueprint
+
+```py
+from exam.views import exam
+```
+
+registering blueprint
+
+```py
+reg_blueprints = [
+  blueprint.default,
+  blueprint.errors,
+  blueprint.auth,
+  base,
+  exam,
+]
+```
+
+once you register the app, boot up the flask webserver again by
+
+```
+python thunder.py boot
+```
+
+visit `http://127.0.0.1:5000` which is your project landing page
+
+visit `http://127.0.0.1:5000/exam` this will take you to your app landing page (exam)
+
+visit `http://127.0.0.1:5000/admin` this will take you to admin page. From there you are ready to go.
+
+See more documentations <a href="https://sakyum.readthedocs.io">here!</a>
+
+### Sakyum default page
+
+![Sakyum default page](sakyum_default_page.png)
+
+## Useful links
+
+- Documentation: https://sakyum.readthedocs.io
+- Repository: https://github.com/usmanmusa1920/sakyum
+- Docker example: https://github.com/usmanmusa1920/sakyum/tree/master/example/sakyum-docker
+
+Pull requests are welcome
+
+
+Change Log
+==========
+
+0.0.9 (22/june/2023)
+------------------
+- Nineth Release
+
+Fixing bugs
+
+Fixing v0.0.8 bugs for OS compatibility, and also tested on windows OS
+
+- Eight Release
+
+OS compatibility
+
+Making sakyum to be compatible with windows OS as well as other OS
+
+0.0.7 (4/april/2023)
+------------------
+- Seventh Release
+
+This release mostly is for adding more docs and examples.
+
+- Sixth Release
+
+Alembic is included as dependency (in the require module list).
+
+- Fifth Release
+
+In fifith release, we handle how default user file system tricks is, things like when user change his profile picture.
+
+- Fourth Release
+
+In this release we handle how we can customise the admin html page by inheriting (extends) it in our project templates/admin directory, and the admin page on how to bind models in the admin. Also I refactor other libraries that this package needs with their corresponding versions in the setup.py and requirements.txt files. In this release good documentations is well packed.
+
+Database migration is added using `alembic`
+
+Some error pages, default page were added but still you can customise it in your project sub folder (the package with the same name of your project in your project directory) in a file called `route.py`. Also an admin directory within your project templates folder is added too!
+
+Possibly other well things are added which include auth system for `users` and more.
```

#### html2text {}

```diff
@@ -1,70 +1,71 @@
-Metadata-Version: 2.1 Name: sakyum Version: 0.0.8 Summary: An extension of
+Metadata-Version: 2.1 Name: sakyum Version: 0.0.9 Summary: An extension of
 flask web framework that erase the complexity of structuring flask project
 blueprint, packages, and other annoying stuffs Home-page: https://
-sakyum.readthedocs.io Author: Usman Musa Author-email: usmanmusa1920@gmail.com
-License: MIT Download-URL: https://pypi.org/project/sakyum Project-URL:
+sakyum.readthedocs.io Download-URL: https://pypi.org/project/sakyum Author:
+Usman Musa Author-email: usmanmusa1920@gmail.com License: MIT Project-URL:
 Documentation, https://sakyum.readthedocs.io Project-URL: Source, https://
-github.com/usmanmusa1920/sakyum Description: # Sakyum An extension of flask web
-framework that erase the complexity of structuring flask project blueprint,
-packages, and other annoying stuffs. ## Installation Install and update the
-latest release from pypi. Basically the library was uploaded using `sdist`
-(Source Distribution) and this software (library) as from `v0.0.8` it is now
-compatible with `windows OS` and others as well, such as `linux`, `macOS` and
-possibly some others too!. ``` pip install --upgrade sakyum ``` ## Create flask
-project using sakyum After the installation paste the following command on your
-termianl ``` python -c "from sakyum import project; project('schoolsite')" ```
-This will create a project called `schoolsite` now cd into the `schoolsite`
-directory, if you do `ls` within the directory you just enter you will see a
-module called `thunder.py` and some directories (some in the form of package)
-`media`, `static`, `templates` and a directory with the same name of your base
-directory name, in our case it is `schoolsite`. Boot up the flask server by
-running the below command ``` python thunder.py boot ``` Now visit the local
-url `http://127.0.0.1:5000` this will show you index page of your project ##
-Create flask app within your project (schoolsite) For you to start an app
-within your project `schoolsite` shutdown the flask development server by
-pressing ( CTRL+C ) and then run the following command, by giving the name you
-want your app to be, in our case we will call our app `exam` ``` python
-thunder.py create_app -a exam ``` this will create an app (a new package called
-`exam`) within your project `(schoolsite)` ## Register an app Once the app is
-created open a file `schoolsite/routes.py` and import your `exam` blueprint
-which is in (`exam/views.py`), default name given to an app blueprint, is the
-app name so our `exam` app blueprint name is `exam`, after importing it, append
-(register) the app blueprint in a list called `reg_blueprints` in that same
-file of `schoolsite/routes.py` importing blueprint ```py from exam.views import
-exam ``` registering blueprint ```py reg_blueprints = [ blueprint.default,
+github.com/usmanmusa1920/sakyum Keywords: sakyum Platform: any Classifier:
+Development Status :: 5 - Production/Stable Classifier: Environment :: Web
+Environment Classifier: Intended Audience :: Developers Classifier: Natural
+Language :: English Classifier: Operating System :: OS Independent Classifier:
+License :: OSI Approved :: MIT License Classifier: Topic :: Software
+Development :: Libraries :: Python Modules Classifier: Programming Language ::
+Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE # Sakyum An extension of flask web framework that erase the complexity
+of structuring flask project blueprint, packages, and other annoying stuffs. ##
+Installation Install and update the latest release from pypi. Basically the
+library was uploaded using `sdist` (Source Distribution) and this software
+(library) as from `v0.0.9` it is now compatible and also tested with `windows
+OS` and others as well, such as `linux`, `macOS` and possibly some others too!.
+``` pip install --upgrade sakyum ``` ## Create flask project using sakyum After
+the installation paste the following command on your termianl ``` python -
+c "from sakyum import project; project('schoolsite')" ``` This will create a
+project called `schoolsite` now cd into the `schoolsite` directory, if you do
+`ls` within the directory you just enter you will see a module called
+`thunder.py` and some directories (some in the form of package) `media`,
+`static`, `templates` and a directory with the same name of your base directory
+name, in our case it is `schoolsite`. Boot up the flask server by running the
+below command ``` python thunder.py boot ``` Now visit the local url `http://
+127.0.0.1:5000` this will show you index page of your project ## Create flask
+app within your project (schoolsite) For you to start an app within your
+project `schoolsite` shutdown the flask development server by pressing ( CTRL+C
+) and then run the following command, by giving the name you want your app to
+be, in our case we will call our app `exam` ``` python thunder.py create_app -
+a exam ``` this will create an app (a new package called `exam`) within your
+project `(schoolsite)` ## Register an app Once the app is created open a file
+`schoolsite/routes.py` and import your `exam` blueprint which is in (`exam/
+views.py`), default name given to an app blueprint, is the app name so our
+`exam` app blueprint name is `exam`, after importing it, append (register) the
+app blueprint in a list called `reg_blueprints` in that same file of
+`schoolsite/routes.py` importing blueprint ```py from exam.views import exam
+``` registering blueprint ```py reg_blueprints = [ blueprint.default,
 blueprint.errors, blueprint.auth, base, exam, ] ``` once you register the app,
 boot up the flask webserver again by ``` python thunder.py boot ``` visit
 `http://127.0.0.1:5000` which is your project landing page visit `http://
 127.0.0.1:5000/exam` this will take you to your app landing page (exam) visit
 `http://127.0.0.1:5000/admin` this will take you to admin page. From there you
 are ready to go. See more documentations here! ### Sakyum default page ![Sakyum
-default page](./media/sakyum_default_page.png) ## Useful links - Documentation:
-https://sakyum.readthedocs.io - Repository: https://github.com/usmanmusa1920/
-sakyum - Docker example: https://github.com/usmanmusa1920/sakyum/tree/master/
-example/sakyum-docker Pull requests are welcome Change Log ========== 0.0.8
-(09/june/2023) ------------------ - Eight Release OS compatibility Making
-sakyum to be compatible with windows OS as well as other OS 0.0.7 (4/april/
-2023) ------------------ - Seventh Release This release mostly is for adding
-more docs and examples. - Sixth Release Alembic is included as dependency (in
-the require module list). - Fifth Release In fifith release, we handle how
-default user file system tricks is, things like when user change his profile
-picture. - Fourth Release In this release we handle how we can customise the
-admin html page by inheriting (extends) it in our project templates/admin
-directory, and the admin page on how to bind models in the admin. Also I
-refactor other libraries that this package needs with their corresponding
-versions in the setup.py and requirements.txt files. In this release good
-documentations is well packed. Database migration is added using `alembic` Some
-error pages, default page were added but still you can customise it in your
-project sub folder (the package with the same name of your project in your
-project directory) in a file called `route.py`. Also an admin directory within
-your project templates folder is added too! Possibly other well things are
-added which include auth system for `users` and more. Keywords: sakyum
-Platform: any Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Web Environment Classifier: Intended Audience ::
-Developers Classifier: Natural Language :: English Classifier: Operating System
-:: OS Independent Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.10 Requires-Python: >=3.6 Description-
-Content-Type: text/markdown
+default page](sakyum_default_page.png) ## Useful links - Documentation: https:/
+/sakyum.readthedocs.io - Repository: https://github.com/usmanmusa1920/sakyum -
+Docker example: https://github.com/usmanmusa1920/sakyum/tree/master/example/
+sakyum-docker Pull requests are welcome Change Log ========== 0.0.9 (22/june/
+2023) ------------------ - Nineth Release Fixing bugs Fixing v0.0.8 bugs for OS
+compatibility, and also tested on windows OS - Eight Release OS compatibility
+Making sakyum to be compatible with windows OS as well as other OS 0.0.7 (4/
+april/2023) ------------------ - Seventh Release This release mostly is for
+adding more docs and examples. - Sixth Release Alembic is included as
+dependency (in the require module list). - Fifth Release In fifith release, we
+handle how default user file system tricks is, things like when user change his
+profile picture. - Fourth Release In this release we handle how we can
+customise the admin html page by inheriting (extends) it in our project
+templates/admin directory, and the admin page on how to bind models in the
+admin. Also I refactor other libraries that this package needs with their
+corresponding versions in the setup.py and requirements.txt files. In this
+release good documentations is well packed. Database migration is added using
+`alembic` Some error pages, default page were added but still you can customise
+it in your project sub folder (the package with the same name of your project
+in your project directory) in a file called `route.py`. Also an admin directory
+within your project templates folder is added too! Possibly other well things
+are added which include auth system for `users` and more.
```

### Comparing `sakyum-0.0.8/sakyum.egg-info/SOURCES.txt` & `sakyum-0.0.9/sakyum.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 CHANGELOG
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
+sakyum_default_page.png
 setup.py
-media/sakyum_default_page.png
 sakyum/__init__.py
 sakyum/api.py
 sakyum/base.py
 sakyum/blueprint.py
 sakyum/database.py
 sakyum/utils.py
 sakyum.egg-info/PKG-INFO
```

### Comparing `sakyum-0.0.8/setup.py` & `sakyum-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup
 from setuptools import find_packages
 
 
 setup(
   name = 'sakyum', # name of the main package (base folder i.e sakyum)
-  version = '0.0.8',
+  version = '0.0.9',
   description = 'An extension of flask web framework that erase the complexity of structuring flask project blueprint, packages, and other annoying stuffs',
   long_description = open('README.md').read() + '\n\n' + open('CHANGELOG').read(),
   long_description_content_type='text/markdown',
   python_requires = '>=3.6',
   platforms='any',
   
   url = 'https://sakyum.readthedocs.io',
```

