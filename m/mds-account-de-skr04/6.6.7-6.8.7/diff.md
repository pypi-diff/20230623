# Comparing `tmp/mds_account_de_skr04-6.6.7.tar.gz` & `tmp/mds_account_de_skr04-6.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_account_de_skr04-6.6.7.tar", last modified: Fri Jun 23 10:44:47 2023, max compression
+gzip compressed data, was "mds_account_de_skr04-6.8.7.tar", last modified: Fri Jun 23 10:11:12 2023, max compression
```

## Comparing `mds_account_de_skr04-6.6.7.tar` & `mds_account_de_skr04-6.8.7.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-23 10:44:47.355318 mds_account_de_skr04-6.6.7/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    35147 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.6.7/LICENSE
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1694 2023-06-23 10:44:47.355318 mds_account_de_skr04-6.6.7/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      412 2023-06-23 10:22:50.000000 mds_account_de_skr04-6.6.7/README.rst
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      214 2023-06-23 10:17:06.000000 mds_account_de_skr04-6.6.7/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)   420212 2022-11-30 10:35:00.000000 mds_account_de_skr04-6.6.7/account_template.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    44541 2022-11-30 10:32:13.000000 mds_account_de_skr04-6.6.7/account_type_template.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-23 10:44:47.355318 mds_account_de_skr04-6.6.7/mds_account_de_skr04.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1694 2023-06-23 10:44:47.000000 mds_account_de_skr04-6.6.7/mds_account_de_skr04.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      587 2023-06-23 10:44:47.000000 mds_account_de_skr04-6.6.7/mds_account_de_skr04.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-23 10:44:47.000000 mds_account_de_skr04-6.6.7/mds_account_de_skr04.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       83 2023-06-23 10:44:47.000000 mds_account_de_skr04-6.6.7/mds_account_de_skr04.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2022-11-30 10:31:43.000000 mds_account_de_skr04-6.6.7/mds_account_de_skr04.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2023-06-23 10:44:47.000000 mds_account_de_skr04-6.6.7/mds_account_de_skr04.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-06-23 10:44:47.000000 mds_account_de_skr04-6.6.7/mds_account_de_skr04.egg-info/top_level.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-06-23 10:44:47.355318 mds_account_de_skr04-6.6.7/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3626 2023-06-23 10:16:17.000000 mds_account_de_skr04-6.6.7/setup.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    19926 2022-11-30 10:32:13.000000 mds_account_de_skr04-6.6.7/tax_code_line_template.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    26405 2022-11-30 10:35:00.000000 mds_account_de_skr04-6.6.7/tax_code_template.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      902 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.6.7/tax_group.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2272 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.6.7/tax_rule_line_template.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1772 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.6.7/tax_rule_template.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    11947 2022-11-30 10:32:13.000000 mds_account_de_skr04-6.6.7/tax_template.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      257 2023-06-23 10:22:56.000000 mds_account_de_skr04-6.6.7/tryton.cfg
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        2 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.6.7/versiondep.txt
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-23 10:11:12.507850 mds_account_de_skr04-6.8.7/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    35147 2023-06-23 07:54:38.000000 mds_account_de_skr04-6.8.7/LICENSE
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1541 2023-06-23 10:11:12.507850 mds_account_de_skr04-6.8.7/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      344 2023-06-23 10:10:32.000000 mds_account_de_skr04-6.8.7/README.rst
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      214 2023-06-23 07:58:04.000000 mds_account_de_skr04-6.8.7/__init__.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)   420212 2023-06-23 07:54:38.000000 mds_account_de_skr04-6.8.7/account_template.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    44541 2023-06-23 07:54:38.000000 mds_account_de_skr04-6.8.7/account_type_template.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2023-06-23 10:11:12.507850 mds_account_de_skr04-6.8.7/mds_account_de_skr04.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1541 2023-06-23 10:11:12.000000 mds_account_de_skr04-6.8.7/mds_account_de_skr04.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      570 2023-06-23 10:11:12.000000 mds_account_de_skr04-6.8.7/mds_account_de_skr04.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-23 10:11:12.000000 mds_account_de_skr04-6.8.7/mds_account_de_skr04.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       83 2023-06-23 10:11:12.000000 mds_account_de_skr04-6.8.7/mds_account_de_skr04.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2023-06-23 10:11:12.000000 mds_account_de_skr04-6.8.7/mds_account_de_skr04.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2023-06-23 10:11:12.000000 mds_account_de_skr04-6.8.7/mds_account_de_skr04.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2023-06-23 10:11:12.000000 mds_account_de_skr04-6.8.7/mds_account_de_skr04.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2023-06-23 10:11:12.507850 mds_account_de_skr04-6.8.7/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3613 2023-06-23 10:09:53.000000 mds_account_de_skr04-6.8.7/setup.py
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    19926 2023-06-23 07:54:38.000000 mds_account_de_skr04-6.8.7/tax_code_line_template.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    26405 2023-06-23 07:54:38.000000 mds_account_de_skr04-6.8.7/tax_code_template.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      902 2023-06-23 07:54:38.000000 mds_account_de_skr04-6.8.7/tax_group.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2272 2023-06-23 07:54:38.000000 mds_account_de_skr04-6.8.7/tax_rule_line_template.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1772 2023-06-23 07:54:38.000000 mds_account_de_skr04-6.8.7/tax_rule_template.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    11947 2023-06-23 07:54:38.000000 mds_account_de_skr04-6.8.7/tax_template.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      257 2023-06-23 10:10:46.000000 mds_account_de_skr04-6.8.7/tryton.cfg
```

### Comparing `mds_account_de_skr04-6.6.7/LICENSE` & `mds_account_de_skr04-6.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.6.7/PKG-INFO` & `mds_account_de_skr04-6.8.7/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 Metadata-Version: 1.1
 Name: mds_account_de_skr04
-Version: 6.6.7
+Version: 6.8.7
 Summary: Tryton module with German chart of accounts SKR04
 Home-page: https://www.m-ds.de/
-Author: martin - data services
+Author: m-ds GmbH
 Author-email: service@m-ds.de
 License: GPL-3
 Description: Chart of accounts 'SKR04'
         =========================
         
         - A german account chart module for the Tryton application platform.
         - Converted and adapted by the module 'account_de_skr03'
         - Contains the accounts according to SKR04
         
         Install
         =======
         
           pip install mds-account-de-skr04
         
-        
-        Requires
-        ========
-        - Tryton 6.6
-        
         Changes
         =======
         
-        *6.6.7 - 23.06.2023*
-        
-        - add: test
-        
-        *6.6.6 - 30.11.2022*
+        *6.8.7 - 23.06.2023*
         
-        - compatiblity to Tryton 6.6
+        - compatiblity to Tryton 6.8
         
 Keywords: tryton account chart german SKR04
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `mds_account_de_skr04-6.6.7/account_template.xml` & `mds_account_de_skr04-6.8.7/account_template.xml`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.6.7/account_type_template.xml` & `mds_account_de_skr04-6.8.7/account_type_template.xml`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.6.7/mds_account_de_skr04.egg-info/PKG-INFO` & `mds_account_de_skr04-6.8.7/mds_account_de_skr04.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 Metadata-Version: 1.1
 Name: mds-account-de-skr04
-Version: 6.6.7
+Version: 6.8.7
 Summary: Tryton module with German chart of accounts SKR04
 Home-page: https://www.m-ds.de/
-Author: martin - data services
+Author: m-ds GmbH
 Author-email: service@m-ds.de
 License: GPL-3
 Description: Chart of accounts 'SKR04'
         =========================
         
         - A german account chart module for the Tryton application platform.
         - Converted and adapted by the module 'account_de_skr03'
         - Contains the accounts according to SKR04
         
         Install
         =======
         
           pip install mds-account-de-skr04
         
-        
-        Requires
-        ========
-        - Tryton 6.6
-        
         Changes
         =======
         
-        *6.6.7 - 23.06.2023*
-        
-        - add: test
-        
-        *6.6.6 - 30.11.2022*
+        *6.8.7 - 23.06.2023*
         
-        - compatiblity to Tryton 6.6
+        - compatiblity to Tryton 6.8
         
 Keywords: tryton account chart german SKR04
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `mds_account_de_skr04-6.6.7/mds_account_de_skr04.egg-info/SOURCES.txt` & `mds_account_de_skr04-6.8.7/mds_account_de_skr04.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 ./tax_code_line_template.xml
 ./tax_code_template.xml
 ./tax_group.xml
 ./tax_rule_line_template.xml
 ./tax_rule_template.xml
 ./tax_template.xml
 ./tryton.cfg
-./versiondep.txt
 mds_account_de_skr04.egg-info/PKG-INFO
 mds_account_de_skr04.egg-info/SOURCES.txt
 mds_account_de_skr04.egg-info/dependency_links.txt
 mds_account_de_skr04.egg-info/entry_points.txt
 mds_account_de_skr04.egg-info/not-zip-safe
 mds_account_de_skr04.egg-info/requires.txt
 mds_account_de_skr04.egg-info/top_level.txt
```

### Comparing `mds_account_de_skr04-6.6.7/setup.py` & `mds_account_de_skr04-6.8.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         l2 = i.strip().split(';')
         if len(l2) < 4:
             continue
         modversion[l2[0]] = {'min': l2[1], 'max': l2[2], 'prefix': l2[3]}
 
 # tryton-version
 major_version = 6
-minor_version = 6
+minor_version = 8
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res|webdav)(\W|$)', dep):
         if dep in modversion.keys():
             prefix = 'mds'
             if len(modversion[dep]['prefix']) > 0:
@@ -66,15 +66,15 @@
 
 setup(
     name='%s_%s' % (PREFIX, MODULE),
     version=info.get('version', '0.0.1'),
     description='Tryton module with German chart of accounts SKR04',
     long_description=long_description,
     url='https://www.m-ds.de/',
-    author='martin - data services',
+    author='m-ds GmbH',
     author_email='service@m-ds.de',
     license='GPL-3',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Plugins',
         'Framework :: Tryton',
         'Intended Audience :: Developers',
```

### Comparing `mds_account_de_skr04-6.6.7/tax_code_line_template.xml` & `mds_account_de_skr04-6.8.7/tax_code_line_template.xml`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.6.7/tax_code_template.xml` & `mds_account_de_skr04-6.8.7/tax_code_template.xml`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.6.7/tax_group.xml` & `mds_account_de_skr04-6.8.7/tax_group.xml`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.6.7/tax_rule_line_template.xml` & `mds_account_de_skr04-6.8.7/tax_rule_line_template.xml`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.6.7/tax_rule_template.xml` & `mds_account_de_skr04-6.8.7/tax_rule_template.xml`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.6.7/tax_template.xml` & `mds_account_de_skr04-6.8.7/tax_template.xml`

 * *Files identical despite different names*

