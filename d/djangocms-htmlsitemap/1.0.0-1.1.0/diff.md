# Comparing `tmp/djangocms-htmlsitemap-1.0.0.tar.gz` & `tmp/djangocms_htmlsitemap-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-htmlsitemap-1.0.0.tar", max compression
+gzip compressed data, was "djangocms_htmlsitemap-1.1.0.tar", max compression
```

## Comparing `djangocms-htmlsitemap-1.0.0.tar` & `djangocms_htmlsitemap-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0     1523 2023-03-10 09:35:06.060497 djangocms-htmlsitemap-1.0.0/LICENSE
--rwxr-xr-x   0        0        0     1007 2023-03-13 15:11:48.372141 djangocms-htmlsitemap-1.0.0/README.md
--rwxr-xr-x   0        0        0       22 2023-03-13 15:05:10.836557 djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/__init__.py
--rw-r--r--   0        0        0      254 2023-03-13 15:02:08.518759 djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/apps.py
--rwxr-xr-x   0        0        0     1660 2023-03-10 10:08:50.544601 djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/cms_plugins.py
--rwxr-xr-x   0        0        0      819 2023-03-10 09:35:06.060497 djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/locale/fr/LC_MESSAGES/django.mo
--rwxr-xr-x   0        0        0     1005 2023-03-13 15:04:26.407934 djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/locale/fr/LC_MESSAGES/django.po
--rwxr-xr-x   0        0        0     1494 2023-03-10 10:08:50.004601 djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/migrations/0001_initial.py
--rwxr-xr-x   0        0        0      741 2023-03-10 10:08:49.975601 djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/migrations/0002_auto_20180228_1210.py
--rwxr-xr-x   0        0        0        0 2023-03-10 09:35:06.060497 djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/migrations/__init__.py
--rwxr-xr-x   0        0        0      701 2023-03-10 10:08:50.536601 djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/models.py
--rwxr-xr-x   0        0        0      289 2023-03-10 09:35:06.061497 djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/templates/djangocms_htmlsitemap/sitemap.html
--rw-r--r--   0        0        0     1096 2023-03-13 15:05:10.836557 djangocms-htmlsitemap-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1960 2023-03-13 15:24:37.704566 djangocms-htmlsitemap-1.0.0/setup.py
--rw-r--r--   0        0        0     1778 2023-03-13 15:24:37.705061 djangocms-htmlsitemap-1.0.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1523 2023-03-10 09:35:06.060497 djangocms_htmlsitemap-1.1.0/LICENSE
+-rwxr-xr-x   0        0        0     1007 2023-03-14 10:41:14.270604 djangocms_htmlsitemap-1.1.0/README.md
+-rwxr-xr-x   0        0        0       22 2023-04-20 15:11:16.011402 djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/__init__.py
+-rw-r--r--   0        0        0      254 2023-03-14 10:41:14.271604 djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/apps.py
+-rwxr-xr-x   0        0        0     1660 2023-03-14 10:41:14.272604 djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/cms_plugins.py
+-rwxr-xr-x   0        0        0      819 2023-03-10 09:35:06.060497 djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/locale/fr/LC_MESSAGES/django.mo
+-rwxr-xr-x   0        0        0     1005 2023-03-13 15:04:26.407934 djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/locale/fr/LC_MESSAGES/django.po
+-rwxr-xr-x   0        0        0     1494 2023-03-14 10:41:14.273604 djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0      741 2023-03-14 10:41:14.274604 djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/migrations/0002_auto_20180228_1210.py
+-rw-r--r--   0        0        0      495 2023-04-20 15:10:43.999907 djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/migrations/0003_alter_htmlsitemappluginconf_in_navigation.py
+-rwxr-xr-x   0        0        0        0 2023-03-10 09:35:06.060497 djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/migrations/__init__.py
+-rwxr-xr-x   0        0        0      708 2023-04-20 15:06:45.073320 djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/models.py
+-rwxr-xr-x   0        0        0      289 2023-03-10 09:35:06.061497 djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/templates/djangocms_htmlsitemap/sitemap.html
+-rw-r--r--   0        0        0     1096 2023-04-20 15:11:16.013402 djangocms_htmlsitemap-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 djangocms_htmlsitemap-1.1.0/PKG-INFO
```

### Comparing `djangocms-htmlsitemap-1.0.0/LICENSE` & `djangocms_htmlsitemap-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-htmlsitemap-1.0.0/README.md` & `djangocms_htmlsitemap-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/cms_plugins.py` & `djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/locale/fr/LC_MESSAGES/django.mo` & `djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/locale/fr/LC_MESSAGES/django.po` & `djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/migrations/0001_initial.py` & `djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/migrations/0002_auto_20180228_1210.py` & `djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/migrations/0002_auto_20180228_1210.py`

 * *Files identical despite different names*

### Comparing `djangocms-htmlsitemap-1.0.0/djangocms_htmlsitemap/models.py` & `djangocms_htmlsitemap-1.1.0/djangocms_htmlsitemap/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 
 class HtmlSitemapPluginConf(CMSPlugin):
     min_depth = models.PositiveIntegerField(verbose_name=_("Minimum depth"), default=0)
     max_depth = models.PositiveIntegerField(
         verbose_name=_("Maximum depth"), blank=True, null=True
     )
-    in_navigation = models.NullBooleanField(
-        verbose_name=_("In navigation"), default=None
+    in_navigation = models.BooleanField(
+        verbose_name=_("In navigation"), default=None, null=True
     )
 
     class Meta:
         verbose_name = _("HTML Sitemap plugin configuration")
         verbose_name_plural = _("HTML Sitemap plugin configurations")
 
     def __str__(self):
```

### Comparing `djangocms-htmlsitemap-1.0.0/pyproject.toml` & `djangocms_htmlsitemap-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "djangocms-htmlsitemap"
-version = "1.0.0"
+version = "1.1.0"
 description = "A Django CMS plugin for building HTML sitemaps showing organized lists of CMS pages."
 authors = ["Kapt dev team <dev@kapt.mobi>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 repository = "https://gitlab.com/kapt/open-source/djangocms-htmlsitemap"
 
 [tool.poetry.dependencies]
@@ -25,15 +25,15 @@
 pytest-spec = ">=0.2"
 pytest-pythonpath = "*"
 coverage = ">=4.4"
 coveralls = "0.2"
 tox = ">=1.7.0"
 
 [build-system]
-requires = ["poetry-core>=1.0.0", "setuptools"]
+requires = ["poetry-core>=1.1.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 include = '\.pyi?$'
 exclude = '''
 (
     \.eggs         # exclude a few common directories in the
```

### Comparing `djangocms-htmlsitemap-1.0.0/PKG-INFO` & `djangocms_htmlsitemap-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: djangocms-htmlsitemap
-Version: 1.0.0
+Version: 1.1.0
 Summary: A Django CMS plugin for building HTML sitemaps showing organized lists of CMS pages.
 Home-page: https://gitlab.com/kapt/open-source/djangocms-htmlsitemap
 License: BSD-3-Clause
 Author: Kapt dev team
 Author-email: dev@kapt.mobi
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Django (>=1.11,<4)
 Requires-Dist: django-cms (>=3.8)
 Project-URL: Repository, https://gitlab.com/kapt/open-source/djangocms-htmlsitemap
 Description-Content-Type: text/markdown
 
 # djangocms-htmlsitemap
```

