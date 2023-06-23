# Comparing `tmp/pretix-mpesa-mz-1.4.1.tar.gz` & `tmp/pretix-mpesa-mz-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pretix-mpesa-mz-1.4.1.tar", last modified: Wed Jun 21 18:19:29 2023, max compression
+gzip compressed data, was "pretix-mpesa-mz-1.4.2.tar", last modified: Fri Jun 23 16:25:42 2023, max compression
```

## Comparing `pretix-mpesa-mz-1.4.1.tar` & `pretix-mpesa-mz-1.4.2.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 18:19:29.783435 pretix-mpesa-mz-1.4.1/
--rw-rw-rw-   0        0        0      567 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.4.1/LICENSE
--rw-rw-rw-   0        0        0      173 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1844 2023-06-21 18:19:29.784441 pretix-mpesa-mz-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     1549 2023-05-12 13:58:54.000000 pretix-mpesa-mz-1.4.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-21 18:19:29.622433 pretix-mpesa-mz-1.4.1/pretix_mpesa_mz.egg-info/
--rw-rw-rw-   0        0        0     1844 2023-06-21 18:19:28.000000 pretix-mpesa-mz-1.4.1/pretix_mpesa_mz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1280 2023-06-21 18:19:29.000000 pretix-mpesa-mz-1.4.1/pretix_mpesa_mz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 18:19:28.000000 pretix-mpesa-mz-1.4.1/pretix_mpesa_mz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-06-21 18:19:28.000000 pretix-mpesa-mz-1.4.1/pretix_mpesa_mz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-06-21 18:19:28.000000 pretix-mpesa-mz-1.4.1/pretix_mpesa_mz.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-21 18:19:29.655442 pretix-mpesa-mz-1.4.1/pretix_mpesamz/
--rw-rw-rw-   0        0        0       23 2023-06-21 18:18:28.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/__init__.py
--rw-rw-rw-   0        0        0      753 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-21 18:19:29.540438 pretix-mpesa-mz-1.4.1/pretix_mpesamz/locale/
-drwxrwxrwx   0        0        0        0 2023-06-21 18:19:29.537439 pretix-mpesa-mz-1.4.1/pretix_mpesamz/locale/de/
-drwxrwxrwx   0        0        0        0 2023-06-21 18:19:29.668439 pretix-mpesa-mz-1.4.1/pretix_mpesamz/locale/de/LC_MESSAGES/
--rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/locale/de/LC_MESSAGES/django.po
-drwxrwxrwx   0        0        0        0 2023-06-21 18:19:29.675437 pretix-mpesa-mz-1.4.1/pretix_mpesamz/locale/de_Informal/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/locale/de_Informal/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-06-21 18:19:29.686436 pretix-mpesa-mz-1.4.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/
--rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
--rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
--rw-rw-rw-   0        0        0     8665 2023-05-17 14:50:26.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/mpesa_api.py
--rw-rw-rw-   0        0        0    16623 2023-06-21 18:04:07.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/payment.py
--rw-rw-rw-   0        0        0      352 2023-04-28 14:11:38.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/signals.py
-drwxrwxrwx   0        0        0        0 2023-06-21 18:19:29.546437 pretix-mpesa-mz-1.4.1/pretix_mpesamz/static/
-drwxrwxrwx   0        0        0        0 2023-06-21 18:19:29.693437 pretix-mpesa-mz-1.4.1/pretix_mpesamz/static/pretix_mpesamz/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/static/pretix_mpesamz/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-06-21 18:19:29.551441 pretix-mpesa-mz-1.4.1/pretix_mpesamz/templates/
-drwxrwxrwx   0        0        0        0 2023-06-21 18:19:29.771448 pretix-mpesa-mz-1.4.1/pretix_mpesamz/templates/pretix_mpesamz/
--rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
--rw-rw-rw-   0        0        0      346 2023-04-26 15:53:24.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
--rw-rw-rw-   0        0        0     4010 2023-05-03 14:29:30.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
--rw-rw-rw-   0        0        0      439 2023-06-21 18:07:10.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/templates/pretix_mpesamz/control.html
--rw-rw-rw-   0        0        0      225 2023-05-11 16:56:59.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/templates/pretix_mpesamz/order.html
--rw-rw-rw-   0        0        0      399 2023-06-21 18:18:46.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/templates/pretix_mpesamz/payment_failed.html
--rw-rw-rw-   0        0        0      246 2023-06-21 15:42:38.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/templates/pretix_mpesamz/payment_pending.html
--rw-rw-rw-   0        0        0      173 2023-06-21 17:56:52.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/templates/pretix_mpesamz/payment_successful.html
--rw-rw-rw-   0        0        0     1075 2023-04-26 15:54:54.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/templates/pretix_mpesamz/redirect.html
--rw-rw-rw-   0        0        0      295 2023-05-12 15:41:12.000000 pretix-mpesa-mz-1.4.1/pretix_mpesamz/templates/pretix_mpesamz/refund_control.html
--rw-rw-rw-   0        0        0      903 2023-06-21 18:19:29.790437 pretix-mpesa-mz-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     1142 2023-05-11 17:36:42.000000 pretix-mpesa-mz-1.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-21 18:19:29.777439 pretix-mpesa-mz-1.4.1/tests/
--rw-rw-rw-   0        0        0       75 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.1/tests/test_main.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:25:42.485409 pretix-mpesa-mz-1.4.2/
+-rw-rw-rw-   0        0        0      567 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.4.2/LICENSE
+-rw-rw-rw-   0        0        0      173 2023-04-26 15:46:37.000000 pretix-mpesa-mz-1.4.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1844 2023-06-23 16:25:42.486412 pretix-mpesa-mz-1.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1549 2023-05-12 13:58:54.000000 pretix-mpesa-mz-1.4.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-23 16:25:41.921405 pretix-mpesa-mz-1.4.2/pretix_mpesa_mz.egg-info/
+-rw-rw-rw-   0        0        0     1844 2023-06-23 16:25:40.000000 pretix-mpesa-mz-1.4.2/pretix_mpesa_mz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1330 2023-06-23 16:25:41.000000 pretix-mpesa-mz-1.4.2/pretix_mpesa_mz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 16:25:40.000000 pretix-mpesa-mz-1.4.2/pretix_mpesa_mz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-06-23 16:25:40.000000 pretix-mpesa-mz-1.4.2/pretix_mpesa_mz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2023-06-23 16:25:40.000000 pretix-mpesa-mz-1.4.2/pretix_mpesa_mz.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 16:25:42.028413 pretix-mpesa-mz-1.4.2/pretix_mpesamz/
+-rw-rw-rw-   0        0        0       23 2023-06-23 16:24:36.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/__init__.py
+-rw-rw-rw-   0        0        0      753 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:25:41.745411 pretix-mpesa-mz-1.4.2/pretix_mpesamz/locale/
+drwxrwxrwx   0        0        0        0 2023-06-23 16:25:41.739409 pretix-mpesa-mz-1.4.2/pretix_mpesamz/locale/de/
+drwxrwxrwx   0        0        0        0 2023-06-23 16:25:42.061411 pretix-mpesa-mz-1.4.2/pretix_mpesamz/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/locale/de/LC_MESSAGES/django.po
+drwxrwxrwx   0        0        0        0 2023-06-23 16:25:42.070407 pretix-mpesa-mz-1.4.2/pretix_mpesamz/locale/de_Informal/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/locale/de_Informal/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-06-23 16:25:42.110412 pretix-mpesa-mz-1.4.2/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      308 2023-05-03 17:00:39.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
+-rw-rw-rw-   0        0        0      321 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
+-rw-rw-rw-   0        0        0     8665 2023-05-17 14:50:26.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/mpesa_api.py
+-rw-rw-rw-   0        0        0    16623 2023-06-21 18:04:07.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/payment.py
+-rw-rw-rw-   0        0        0      352 2023-04-28 14:11:38.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/signals.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:25:41.755411 pretix-mpesa-mz-1.4.2/pretix_mpesamz/static/
+drwxrwxrwx   0        0        0        0 2023-06-23 16:25:42.128408 pretix-mpesa-mz-1.4.2/pretix_mpesamz/static/pretix_mpesamz/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/static/pretix_mpesamz/.gitkeep
+-rw-rw-rw-   0        0        0      233 2023-06-23 16:22:49.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/static/pretix_mpesamz/countdown.js
+drwxrwxrwx   0        0        0        0 2023-06-23 16:25:41.761408 pretix-mpesa-mz-1.4.2/pretix_mpesamz/templates/
+drwxrwxrwx   0        0        0        0 2023-06-23 16:25:42.461407 pretix-mpesa-mz-1.4.2/pretix_mpesamz/templates/pretix_mpesamz/
+-rw-rw-rw-   0        0        0        0 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
+-rw-rw-rw-   0        0        0      346 2023-04-26 15:53:24.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
+-rw-rw-rw-   0        0        0     4010 2023-06-23 16:21:06.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
+-rw-rw-rw-   0        0        0      439 2023-06-21 18:07:10.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/templates/pretix_mpesamz/control.html
+-rw-rw-rw-   0        0        0      225 2023-05-11 16:56:59.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/templates/pretix_mpesamz/order.html
+-rw-rw-rw-   0        0        0      399 2023-06-21 18:18:46.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/templates/pretix_mpesamz/payment_failed.html
+-rw-rw-rw-   0        0        0      377 2023-06-23 16:21:46.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/templates/pretix_mpesamz/payment_pending.html
+-rw-rw-rw-   0        0        0      173 2023-06-21 17:56:52.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/templates/pretix_mpesamz/payment_successful.html
+-rw-rw-rw-   0        0        0     1075 2023-04-26 15:54:54.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/templates/pretix_mpesamz/redirect.html
+-rw-rw-rw-   0        0        0      295 2023-05-12 15:41:12.000000 pretix-mpesa-mz-1.4.2/pretix_mpesamz/templates/pretix_mpesamz/refund_control.html
+-rw-rw-rw-   0        0        0      903 2023-06-23 16:25:42.545408 pretix-mpesa-mz-1.4.2/setup.cfg
+-rw-rw-rw-   0        0        0     1142 2023-05-11 17:36:42.000000 pretix-mpesa-mz-1.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:25:42.477415 pretix-mpesa-mz-1.4.2/tests/
+-rw-rw-rw-   0        0        0       75 2023-04-26 15:46:38.000000 pretix-mpesa-mz-1.4.2/tests/test_main.py
```

### Comparing `pretix-mpesa-mz-1.4.1/LICENSE` & `pretix-mpesa-mz-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.4.1/PKG-INFO` & `pretix-mpesa-mz-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mpesa-mz
-Version: 1.4.1
+Version: 1.4.2
 Summary: A plugin to allow payments through the M-Pesa mobile payment platform
 Home-page: https://github.com/ivanruby/pretix-mpesa-mz
 Author: Ivan Ruby
 Author-email: ivanrubyds@gmail.com
 License: Apache
 License-File: LICENSE
```

### Comparing `pretix-mpesa-mz-1.4.1/README.rst` & `pretix-mpesa-mz-1.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.4.1/pretix_mpesa_mz.egg-info/PKG-INFO` & `pretix-mpesa-mz-1.4.2/pretix_mpesa_mz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pretix-mpesa-mz
-Version: 1.4.1
+Version: 1.4.2
 Summary: A plugin to allow payments through the M-Pesa mobile payment platform
 Home-page: https://github.com/ivanruby/pretix-mpesa-mz
 Author: Ivan Ruby
 Author-email: ivanrubyds@gmail.com
 License: Apache
 License-File: LICENSE
```

### Comparing `pretix-mpesa-mz-1.4.1/pretix_mpesa_mz.egg-info/SOURCES.txt` & `pretix-mpesa-mz-1.4.2/pretix_mpesa_mz.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 pretix_mpesamz/signals.py
 pretix_mpesamz/locale/de/LC_MESSAGES/django.mo
 pretix_mpesamz/locale/de/LC_MESSAGES/django.po
 pretix_mpesamz/locale/de_Informal/.gitkeep
 pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.mo
 pretix_mpesamz/locale/de_Informal/LC_MESSAGES/django.po
 pretix_mpesamz/static/pretix_mpesamz/.gitkeep
+pretix_mpesamz/static/pretix_mpesamz/countdown.js
 pretix_mpesamz/templates/pretix_mpesamz/.gitkeep
 pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_confirm.html
 pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html
 pretix_mpesamz/templates/pretix_mpesamz/control.html
 pretix_mpesamz/templates/pretix_mpesamz/order.html
 pretix_mpesamz/templates/pretix_mpesamz/payment_failed.html
 pretix_mpesamz/templates/pretix_mpesamz/payment_pending.html
```

### Comparing `pretix-mpesa-mz-1.4.1/pretix_mpesamz/apps.py` & `pretix-mpesa-mz-1.4.2/pretix_mpesamz/apps.py`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.4.1/pretix_mpesamz/mpesa_api.py` & `pretix-mpesa-mz-1.4.2/pretix_mpesamz/mpesa_api.py`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.4.1/pretix_mpesamz/payment.py` & `pretix-mpesa-mz-1.4.2/pretix_mpesamz/payment.py`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.4.1/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html` & `pretix-mpesa-mz-1.4.2/pretix_mpesamz/templates/pretix_mpesamz/checkout_payment_form.html`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.4.1/pretix_mpesamz/templates/pretix_mpesamz/redirect.html` & `pretix-mpesa-mz-1.4.2/pretix_mpesamz/templates/pretix_mpesamz/redirect.html`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.4.1/setup.cfg` & `pretix-mpesa-mz-1.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pretix-mpesa-mz-1.4.1/setup.py` & `pretix-mpesa-mz-1.4.2/setup.py`

 * *Files identical despite different names*

