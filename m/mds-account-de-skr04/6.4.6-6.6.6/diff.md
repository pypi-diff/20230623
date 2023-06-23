# Comparing `tmp/mds_account_de_skr04-6.4.6.tar.gz` & `tmp/mds_account_de_skr04-6.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mds_account_de_skr04-6.4.6.tar", last modified: Wed Nov 30 10:36:23 2022, max compression
+gzip compressed data, was "mds_account_de_skr04-6.6.6.tar", last modified: Wed Nov 30 10:45:41 2022, max compression
```

## Comparing `mds_account_de_skr04-6.4.6.tar` & `mds_account_de_skr04-6.6.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2022-11-30 10:36:23.815026 mds_account_de_skr04-6.4.6/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    35147 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.4.6/LICENSE
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1735 2022-11-30 10:36:23.815026 mds_account_de_skr04-6.4.6/PKG-INFO
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      411 2022-11-30 10:35:24.000000 mds_account_de_skr04-6.4.6/README.rst
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       29 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.4.6/__init__.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)   420212 2022-11-30 10:35:00.000000 mds_account_de_skr04-6.4.6/account_template.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    44541 2022-11-30 10:32:13.000000 mds_account_de_skr04-6.4.6/account_type_template.xml
-drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2022-11-30 10:36:23.815026 mds_account_de_skr04-6.4.6/mds_account_de_skr04.egg-info/
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1735 2022-11-30 10:36:23.000000 mds_account_de_skr04-6.4.6/mds_account_de_skr04.egg-info/PKG-INFO
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      587 2022-11-30 10:36:23.000000 mds_account_de_skr04-6.4.6/mds_account_de_skr04.egg-info/SOURCES.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2022-11-30 10:36:23.000000 mds_account_de_skr04-6.4.6/mds_account_de_skr04.egg-info/dependency_links.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       83 2022-11-30 10:36:23.000000 mds_account_de_skr04-6.4.6/mds_account_de_skr04.egg-info/entry_points.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2022-11-30 10:31:43.000000 mds_account_de_skr04-6.4.6/mds_account_de_skr04.egg-info/not-zip-safe
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2022-11-30 10:36:23.000000 mds_account_de_skr04-6.4.6/mds_account_de_skr04.egg-info/requires.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2022-11-30 10:36:23.000000 mds_account_de_skr04-6.4.6/mds_account_de_skr04.egg-info/top_level.txt
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2022-11-30 10:36:23.815026 mds_account_de_skr04-6.4.6/setup.cfg
--rw-rw----   0 trytproj  (1001) trytproj  (1001)     3585 2022-11-30 10:34:53.000000 mds_account_de_skr04-6.4.6/setup.py
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    19926 2022-11-30 10:32:13.000000 mds_account_de_skr04-6.4.6/tax_code_line_template.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    26405 2022-11-30 10:35:00.000000 mds_account_de_skr04-6.4.6/tax_code_template.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      902 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.4.6/tax_group.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2272 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.4.6/tax_rule_line_template.xml
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1772 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.4.6/tax_rule_template.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)    11947 2022-11-30 10:32:13.000000 mds_account_de_skr04-6.4.6/tax_template.xml
--rw-rw----   0 trytproj  (1001) trytproj  (1001)      257 2022-11-30 10:35:34.000000 mds_account_de_skr04-6.4.6/tryton.cfg
--rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        2 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.4.6/versiondep.txt
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2022-11-30 10:45:41.777396 mds_account_de_skr04-6.6.6/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)    35147 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.6.6/LICENSE
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1677 2022-11-30 10:45:41.777396 mds_account_de_skr04-6.6.6/PKG-INFO
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      377 2022-11-30 10:38:56.000000 mds_account_de_skr04-6.6.6/README.rst
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       29 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.6.6/__init__.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)   420212 2022-11-30 10:35:00.000000 mds_account_de_skr04-6.6.6/account_template.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    44541 2022-11-30 10:32:13.000000 mds_account_de_skr04-6.6.6/account_type_template.xml
+drwxrwxr-x   0 trytproj  (1001) trytproj  (1001)        0 2022-11-30 10:45:41.777396 mds_account_de_skr04-6.6.6/mds_account_de_skr04.egg-info/
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1677 2022-11-30 10:45:41.000000 mds_account_de_skr04-6.6.6/mds_account_de_skr04.egg-info/PKG-INFO
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      587 2022-11-30 10:45:41.000000 mds_account_de_skr04-6.6.6/mds_account_de_skr04.egg-info/SOURCES.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2022-11-30 10:45:41.000000 mds_account_de_skr04-6.6.6/mds_account_de_skr04.egg-info/dependency_links.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       83 2022-11-30 10:45:41.000000 mds_account_de_skr04-6.6.6/mds_account_de_skr04.egg-info/entry_points.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        1 2022-11-30 10:31:43.000000 mds_account_de_skr04-6.6.6/mds_account_de_skr04.egg-info/not-zip-safe
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       44 2022-11-30 10:45:41.000000 mds_account_de_skr04-6.6.6/mds_account_de_skr04.egg-info/requires.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        8 2022-11-30 10:45:41.000000 mds_account_de_skr04-6.6.6/mds_account_de_skr04.egg-info/top_level.txt
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)       38 2022-11-30 10:45:41.777396 mds_account_de_skr04-6.6.6/setup.cfg
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)     3581 2022-11-30 10:43:05.000000 mds_account_de_skr04-6.6.6/setup.py
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    19926 2022-11-30 10:32:13.000000 mds_account_de_skr04-6.6.6/tax_code_line_template.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    26405 2022-11-30 10:35:00.000000 mds_account_de_skr04-6.6.6/tax_code_template.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)      902 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.6.6/tax_group.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     2272 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.6.6/tax_rule_line_template.xml
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)     1772 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.6.6/tax_rule_template.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)    11947 2022-11-30 10:32:13.000000 mds_account_de_skr04-6.6.6/tax_template.xml
+-rw-rw----   0 trytproj  (1001) trytproj  (1001)      257 2022-11-30 10:37:43.000000 mds_account_de_skr04-6.6.6/tryton.cfg
+-rw-rw-r--   0 trytproj  (1001) trytproj  (1001)        2 2022-11-30 09:40:28.000000 mds_account_de_skr04-6.6.6/versiondep.txt
```

### Comparing `mds_account_de_skr04-6.4.6/LICENSE` & `mds_account_de_skr04-6.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.4.6/PKG-INFO` & `mds_account_de_skr04-6.6.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 Metadata-Version: 1.1
 Name: mds_account_de_skr04
-Version: 6.4.6
+Version: 6.6.6
 Summary: Tryton module with German chart of accounts SKR04
 Home-page: https://www.m-ds.de/
-Author: martin data - services
+Author: martin - data services
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
         
+        
         Requires
         ========
-        - Tryton 6.4
+        - Tryton 6.6
         
         Changes
         =======
         
-        *6.4.6 - 30.11.2022*
-        
-        - fix: typo
-        
-        *6.4.5 - 25.11.2022*
+        *6.6.6 - 30.11.2022*
         
-        - compatiblity to Tryton 6.4
+        - compatiblity to Tryton 6.6
         
 Keywords: tryton account chart german SKR04
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `mds_account_de_skr04-6.4.6/account_template.xml` & `mds_account_de_skr04-6.6.6/account_template.xml`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.4.6/account_type_template.xml` & `mds_account_de_skr04-6.6.6/account_type_template.xml`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.4.6/mds_account_de_skr04.egg-info/PKG-INFO` & `mds_account_de_skr04-6.6.6/mds_account_de_skr04.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 Metadata-Version: 1.1
 Name: mds-account-de-skr04
-Version: 6.4.6
+Version: 6.6.6
 Summary: Tryton module with German chart of accounts SKR04
 Home-page: https://www.m-ds.de/
-Author: martin data - services
+Author: martin - data services
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
         
+        
         Requires
         ========
-        - Tryton 6.4
+        - Tryton 6.6
         
         Changes
         =======
         
-        *6.4.6 - 30.11.2022*
-        
-        - fix: typo
-        
-        *6.4.5 - 25.11.2022*
+        *6.6.6 - 30.11.2022*
         
-        - compatiblity to Tryton 6.4
+        - compatiblity to Tryton 6.6
         
 Keywords: tryton account chart german SKR04
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Plugins
 Classifier: Framework :: Tryton
 Classifier: Intended Audience :: Developers
```

### Comparing `mds_account_de_skr04-6.4.6/mds_account_de_skr04.egg-info/SOURCES.txt` & `mds_account_de_skr04-6.6.6/mds_account_de_skr04.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.4.6/setup.py` & `mds_account_de_skr04-6.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         l2 = i.strip().split(';')
         if len(l2) < 4:
             continue
         modversion[l2[0]] = {'min':l2[1], 'max':l2[2], 'prefix':l2[3]}
 
 # tryton-version
 major_version = 6
-minor_version = 4
+minor_version = 6
 
 requires = []
 for dep in info.get('depends', []):
     if not re.match(r'(ir|res|webdav)(\W|$)', dep):
         if dep in modversion.keys():
             prefix = 'mds'
             if len(modversion[dep]['prefix']) > 0:
@@ -64,15 +64,15 @@
         (major_version, minor_version, major_version, minor_version + 1))
 
 setup(name='%s_%s' % (PREFIX, MODULE),
     version=info.get('version', '0.0.1'),
     description='Tryton module with German chart of accounts SKR04',
     long_description=long_description,
     url='https://www.m-ds.de/',
-    author='martin data - services',
+    author='martin - data services',
     author_email='service@m-ds.de',
     license='GPL-3',
     classifiers=[
     'Development Status :: 5 - Production/Stable',
     'Environment :: Plugins',
     'Framework :: Tryton',
     'Intended Audience :: Developers',
@@ -84,15 +84,15 @@
     'Natural Language :: German',
     'Operating System :: OS Independent',
     'License :: OSI Approved :: GNU General Public License (GPL)',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
-    ],
+],
 
     keywords='tryton account chart german SKR04',
     package_dir={'trytond.modules.%s' % MODULE: '.'},
     packages=[
         'trytond.modules.%s' % MODULE,
         ],
     package_data={
```

### Comparing `mds_account_de_skr04-6.4.6/tax_code_line_template.xml` & `mds_account_de_skr04-6.6.6/tax_code_line_template.xml`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.4.6/tax_code_template.xml` & `mds_account_de_skr04-6.6.6/tax_code_template.xml`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.4.6/tax_group.xml` & `mds_account_de_skr04-6.6.6/tax_group.xml`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.4.6/tax_rule_line_template.xml` & `mds_account_de_skr04-6.6.6/tax_rule_line_template.xml`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.4.6/tax_rule_template.xml` & `mds_account_de_skr04-6.6.6/tax_rule_template.xml`

 * *Files identical despite different names*

### Comparing `mds_account_de_skr04-6.4.6/tax_template.xml` & `mds_account_de_skr04-6.6.6/tax_template.xml`

 * *Files identical despite different names*

