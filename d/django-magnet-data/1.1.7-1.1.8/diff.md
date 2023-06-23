# Comparing `tmp/django-magnet-data-1.1.7.tar.gz` & `tmp/django-magnet-data-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-magnet-data-1.1.7.tar", max compression
+gzip compressed data, was "django-magnet-data-1.1.8.tar", max compression
```

## Comparing `django-magnet-data-1.1.7.tar` & `django-magnet-data-1.1.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1066 2022-10-14 16:58:17.859198 django-magnet-data-1.1.7/LICENSE
--rw-r--r--   0        0        0        0 2022-12-22 18:15:19.775890 django-magnet-data-1.1.7/magnet_data/__init__.py
--rw-r--r--   0        0        0      241 2023-06-08 18:49:27.912079 django-magnet-data-1.1.7/magnet_data/apps.py
--rw-r--r--   0        0        0        0 2022-12-22 18:15:19.775890 django-magnet-data-1.1.7/magnet_data/currencies/__init__.py
--rw-r--r--   0        0        0     1599 2022-12-22 18:15:19.775890 django-magnet-data-1.1.7/magnet_data/currencies/client.py
--rw-r--r--   0        0        0     4702 2023-05-04 20:28:56.929778 django-magnet-data-1.1.7/magnet_data/currencies/currency_pair.py
--rw-r--r--   0        0        0      290 2023-06-08 18:50:18.368530 django-magnet-data-1.1.7/magnet_data/currencies/enums.py
--rw-r--r--   0        0        0      801 2023-06-08 18:50:34.816675 django-magnet-data-1.1.7/magnet_data/currencies/exceptions.py
--rw-r--r--   0        0        0     1313 2023-06-08 18:50:41.364732 django-magnet-data-1.1.7/magnet_data/currencies/models.py
--rw-r--r--   0        0        0       54 2022-12-22 18:15:19.775890 django-magnet-data-1.1.7/magnet_data/currencies/urls.py
--rw-r--r--   0        0        0        0 2023-05-04 20:28:56.913778 django-magnet-data-1.1.7/magnet_data/holidays/__init__.py
--rw-r--r--   0        0        0      216 2023-05-04 20:28:56.917778 django-magnet-data-1.1.7/magnet_data/holidays/admin.py
--rw-r--r--   0        0        0    11688 2023-06-08 18:48:25.403508 django-magnet-data-1.1.7/magnet_data/holidays/enums.py
--rw-r--r--   0        0        0     2277 2023-06-23 14:25:02.930256 django-magnet-data-1.1.7/magnet_data/holidays/models.py
--rw-r--r--   0        0        0     3839 2023-05-04 20:28:56.917778 django-magnet-data-1.1.7/magnet_data/magnet_data_client.py
--rw-r--r--   0        0        0     2249 2022-12-22 18:15:19.779890 django-magnet-data-1.1.7/magnet_data/migrations/0001_initial.py
--rw-r--r--   0        0        0     6827 2023-05-04 20:28:56.917778 django-magnet-data-1.1.7/magnet_data/migrations/0002_holiday.py
--rw-r--r--   0        0        0        0 2022-12-22 18:15:19.779890 django-magnet-data-1.1.7/magnet_data/migrations/__init__.py
--rw-r--r--   0        0        0      118 2023-05-04 20:28:56.921778 django-magnet-data-1.1.7/magnet_data/models.py
--rw-r--r--   0        0        0      202 2022-12-22 18:15:19.779890 django-magnet-data-1.1.7/magnet_data/utils.py
--rw-r--r--   0        0        0      862 2023-06-23 14:25:19.898272 django-magnet-data-1.1.7/pyproject.toml
--rw-r--r--   0        0        0      748 2023-06-23 14:25:24.686062 django-magnet-data-1.1.7/setup.py
--rw-r--r--   0        0        0      861 2023-06-23 14:25:24.686237 django-magnet-data-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-10-14 16:58:17.859198 django-magnet-data-1.1.8/LICENSE
+-rw-r--r--   0        0        0        0 2022-12-22 18:15:19.775890 django-magnet-data-1.1.8/magnet_data/__init__.py
+-rw-r--r--   0        0        0      241 2023-06-08 18:49:27.912079 django-magnet-data-1.1.8/magnet_data/apps.py
+-rw-r--r--   0        0        0        0 2022-12-22 18:15:19.775890 django-magnet-data-1.1.8/magnet_data/currencies/__init__.py
+-rw-r--r--   0        0        0     1599 2022-12-22 18:15:19.775890 django-magnet-data-1.1.8/magnet_data/currencies/client.py
+-rw-r--r--   0        0        0     4702 2023-05-04 20:28:56.929778 django-magnet-data-1.1.8/magnet_data/currencies/currency_pair.py
+-rw-r--r--   0        0        0      290 2023-06-08 18:50:18.368530 django-magnet-data-1.1.8/magnet_data/currencies/enums.py
+-rw-r--r--   0        0        0      801 2023-06-08 18:50:34.816675 django-magnet-data-1.1.8/magnet_data/currencies/exceptions.py
+-rw-r--r--   0        0        0     1313 2023-06-08 18:50:41.364732 django-magnet-data-1.1.8/magnet_data/currencies/models.py
+-rw-r--r--   0        0        0       54 2022-12-22 18:15:19.775890 django-magnet-data-1.1.8/magnet_data/currencies/urls.py
+-rw-r--r--   0        0        0        0 2023-05-04 20:28:56.913778 django-magnet-data-1.1.8/magnet_data/holidays/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-04 20:28:56.917778 django-magnet-data-1.1.8/magnet_data/holidays/admin.py
+-rw-r--r--   0        0        0    11688 2023-06-08 18:48:25.403508 django-magnet-data-1.1.8/magnet_data/holidays/enums.py
+-rw-r--r--   0        0        0     2331 2023-06-23 15:11:37.081168 django-magnet-data-1.1.8/magnet_data/holidays/models.py
+-rw-r--r--   0        0        0     3839 2023-05-04 20:28:56.917778 django-magnet-data-1.1.8/magnet_data/magnet_data_client.py
+-rw-r--r--   0        0        0     2249 2022-12-22 18:15:19.779890 django-magnet-data-1.1.8/magnet_data/migrations/0001_initial.py
+-rw-r--r--   0        0        0     6827 2023-05-04 20:28:56.917778 django-magnet-data-1.1.8/magnet_data/migrations/0002_holiday.py
+-rw-r--r--   0        0        0      354 2023-06-23 16:46:05.694654 django-magnet-data-1.1.8/magnet_data/migrations/0003_alter_holiday_unique_together.py
+-rw-r--r--   0        0        0        0 2022-12-22 18:15:19.779890 django-magnet-data-1.1.8/magnet_data/migrations/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-04 20:28:56.921778 django-magnet-data-1.1.8/magnet_data/models.py
+-rw-r--r--   0        0        0      202 2022-12-22 18:15:19.779890 django-magnet-data-1.1.8/magnet_data/utils.py
+-rw-r--r--   0        0        0      862 2023-06-23 16:46:03.146652 django-magnet-data-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0      748 2023-06-23 16:46:09.588324 django-magnet-data-1.1.8/setup.py
+-rw-r--r--   0        0        0      861 2023-06-23 16:46:09.588504 django-magnet-data-1.1.8/PKG-INFO
```

### Comparing `django-magnet-data-1.1.7/LICENSE` & `django-magnet-data-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.7/magnet_data/currencies/client.py` & `django-magnet-data-1.1.8/magnet_data/currencies/client.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.7/magnet_data/currencies/currency_pair.py` & `django-magnet-data-1.1.8/magnet_data/currencies/currency_pair.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.7/magnet_data/currencies/exceptions.py` & `django-magnet-data-1.1.8/magnet_data/currencies/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.7/magnet_data/currencies/models.py` & `django-magnet-data-1.1.8/magnet_data/currencies/models.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.7/magnet_data/holidays/enums.py` & `django-magnet-data-1.1.8/magnet_data/holidays/enums.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.7/magnet_data/holidays/models.py` & `django-magnet-data-1.1.8/magnet_data/holidays/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
         choices=Countries.django_model_choices,
     )
 
     class Meta:
         ordering = ("date",)
         verbose_name = _('holiday')
         verbose_name_plural = _('holidays')
+        unique_together = (("date", "country_code"),)
 
     def __str__(self):
         return f"{self.country_code}-{self.date}"
 
     @classmethod
     def update_holidays(cls, country_code):
         year = datetime.date.today().year
```

### Comparing `django-magnet-data-1.1.7/magnet_data/magnet_data_client.py` & `django-magnet-data-1.1.8/magnet_data/magnet_data_client.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.7/magnet_data/migrations/0001_initial.py` & `django-magnet-data-1.1.8/magnet_data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.7/magnet_data/migrations/0002_holiday.py` & `django-magnet-data-1.1.8/magnet_data/migrations/0002_holiday.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.7/setup.py` & `django-magnet-data-1.1.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['django>=2.2']
 
 setup_kwargs = {
     'name': 'django-magnet-data',
-    'version': '1.1.7',
+    'version': '1.1.8',
     'description': 'An API client for data.magnet.cl',
     'long_description': None,
     'author': 'Ignacio Munizaga',
     'author_email': 'muni@magnet.cl',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/magnet-cl/django-magnet-data',
```

### Comparing `django-magnet-data-1.1.7/PKG-INFO` & `django-magnet-data-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-magnet-data
-Version: 1.1.7
+Version: 1.1.8
 Summary: An API client for data.magnet.cl
 Home-page: https://github.com/magnet-cl/django-magnet-data
 License: MIT
 Author: Ignacio Munizaga
 Author-email: muni@magnet.cl
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: Framework :: Django
```

