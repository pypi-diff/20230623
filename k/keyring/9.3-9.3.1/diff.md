# Comparing `tmp/keyring-9.3.tar.gz` & `tmp/keyring-9.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/keyring-9.3.tar", last modified: Mon Jun 27 16:23:55 2016, max compression
+gzip compressed data, was "dist/keyring-9.3.1.tar", last modified: Thu Jul 14 14:12:52 2016, max compression
```

## Comparing `keyring-9.3.tar` & `keyring-9.3.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-06-27 16:23:55.000000 keyring-9.3/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-06-27 16:23:55.000000 keyring-9.3/docs/
--rw-rw-r--   0 travis    (1000) travis    (1000)      759 2016-06-27 16:23:23.000000 keyring-9.3/docs/conf.py
--rw-rw-r--   0 travis    (1000) travis    (1000)       81 2016-06-27 16:23:23.000000 keyring-9.3/docs/history.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)      369 2016-06-27 16:23:23.000000 keyring-9.3/docs/index.rst
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-06-27 16:23:55.000000 keyring-9.3/keyring/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-06-27 16:23:55.000000 keyring-9.3/keyring/backends/
--rw-rw-r--   0 travis    (1000) travis    (1000)     1475 2016-06-27 16:23:23.000000 keyring-9.3/keyring/backends/OS_X.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2893 2016-06-27 16:23:23.000000 keyring-9.3/keyring/backends/SecretService.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     4904 2016-06-27 16:23:23.000000 keyring-9.3/keyring/backends/Windows.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     5859 2016-06-27 16:23:23.000000 keyring-9.3/keyring/backends/_OS_X_API.py
--rw-rw-r--   0 travis    (1000) travis    (1000)        0 2016-06-27 16:23:23.000000 keyring-9.3/keyring/backends/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      662 2016-06-27 16:23:23.000000 keyring-9.3/keyring/backends/fail.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3845 2016-06-27 16:23:23.000000 keyring-9.3/keyring/backends/kwallet.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-06-27 16:23:55.000000 keyring-9.3/keyring/tests/
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-06-27 16:23:55.000000 keyring-9.3/keyring/tests/backends/
--rw-rw-r--   0 travis    (1000) travis    (1000)        0 2016-06-27 16:23:23.000000 keyring-9.3/keyring/tests/backends/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      394 2016-06-27 16:23:23.000000 keyring-9.3/keyring/tests/backends/test_OS_X.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      865 2016-06-27 16:23:23.000000 keyring-9.3/keyring/tests/backends/test_SecretService.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      911 2016-06-27 16:23:23.000000 keyring-9.3/keyring/tests/backends/test_Windows.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2782 2016-06-27 16:23:23.000000 keyring-9.3/keyring/tests/backends/test_kwallet.py
--rw-rw-r--   0 travis    (1000) travis    (1000)       87 2016-06-27 16:23:23.000000 keyring-9.3/keyring/tests/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     5109 2016-06-27 16:23:23.000000 keyring-9.3/keyring/tests/test_backend.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1924 2016-06-27 16:23:23.000000 keyring-9.3/keyring/tests/util.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-06-27 16:23:55.000000 keyring-9.3/keyring/util/
--rw-rw-r--   0 travis    (1000) travis    (1000)      864 2016-06-27 16:23:23.000000 keyring-9.3/keyring/util/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1497 2016-06-27 16:23:23.000000 keyring-9.3/keyring/util/escape.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     2231 2016-06-27 16:23:23.000000 keyring-9.3/keyring/util/platform_.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1337 2016-06-27 16:23:23.000000 keyring-9.3/keyring/util/properties.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      398 2016-06-27 16:23:23.000000 keyring-9.3/keyring/__init__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)       70 2016-06-27 16:23:23.000000 keyring-9.3/keyring/__main__.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     5023 2016-06-27 16:23:23.000000 keyring-9.3/keyring/backend.py
--rwxrwxr-x   0 travis    (1000) travis    (1000)     3369 2016-06-27 16:23:23.000000 keyring-9.3/keyring/cli.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     3985 2016-06-27 16:23:23.000000 keyring-9.3/keyring/core.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1355 2016-06-27 16:23:23.000000 keyring-9.3/keyring/credentials.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1180 2016-06-27 16:23:23.000000 keyring-9.3/keyring/errors.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      312 2016-06-27 16:23:23.000000 keyring-9.3/keyring/getpassbackend.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1255 2016-06-27 16:23:23.000000 keyring-9.3/keyring/http.py
--rw-rw-r--   0 travis    (1000) travis    (1000)     1008 2016-06-27 16:23:23.000000 keyring-9.3/keyring/py27compat.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      660 2016-06-27 16:23:23.000000 keyring-9.3/keyring/py33compat.py
-drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-06-27 16:23:55.000000 keyring-9.3/keyring.egg-info/
--rw-rw-r--   0 travis    (1000) travis    (1000)    14752 2016-06-27 16:23:55.000000 keyring-9.3/keyring.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)     1141 2016-06-27 16:23:55.000000 keyring-9.3/keyring.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-06-27 16:23:55.000000 keyring-9.3/keyring.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)       46 2016-06-27 16:23:55.000000 keyring-9.3/keyring.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)      127 2016-06-27 16:23:55.000000 keyring-9.3/keyring.egg-info/requires.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)        8 2016-06-27 16:23:55.000000 keyring-9.3/keyring.egg-info/top_level.txt
--rw-rw-r--   0 travis    (1000) travis    (1000)      737 2016-06-27 16:23:23.000000 keyring-9.3/.gitignore
--rw-rw-r--   0 travis    (1000) travis    (1000)     5335 2016-06-27 16:23:23.000000 keyring-9.3/.hgtags
--rw-rw-r--   0 travis    (1000) travis    (1000)     1117 2016-06-27 16:23:23.000000 keyring-9.3/.travis.yml
--rw-rw-r--   0 travis    (1000) travis    (1000)    23844 2016-06-27 16:23:23.000000 keyring-9.3/CHANGES.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)    11260 2016-06-27 16:23:23.000000 keyring-9.3/README.rst
--rw-rw-r--   0 travis    (1000) travis    (1000)       52 2016-06-27 16:23:23.000000 keyring-9.3/conftest.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      394 2016-06-27 16:23:23.000000 keyring-9.3/hook-keyring.backend.py
--rw-rw-r--   0 travis    (1000) travis    (1000)      154 2016-06-27 16:23:23.000000 keyring-9.3/pytest.ini
--rw-rw-r--   0 travis    (1000) travis    (1000)     2188 2016-06-27 16:23:23.000000 keyring-9.3/setup.py
--rw-rw-r--   0 travis    (1000) travis    (1000)    14752 2016-06-27 16:23:55.000000 keyring-9.3/PKG-INFO
--rw-rw-r--   0 travis    (1000) travis    (1000)      179 2016-06-27 16:23:55.000000 keyring-9.3/setup.cfg
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-07-14 14:12:52.000000 keyring-9.3.1/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-07-14 14:12:52.000000 keyring-9.3.1/docs/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      759 2016-07-14 14:12:11.000000 keyring-9.3.1/docs/conf.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)       81 2016-07-14 14:12:11.000000 keyring-9.3.1/docs/history.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)      369 2016-07-14 14:12:11.000000 keyring-9.3.1/docs/index.rst
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-07-14 14:12:52.000000 keyring-9.3.1/keyring/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-07-14 14:12:52.000000 keyring-9.3.1/keyring/backends/
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1475 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/backends/OS_X.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2893 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/backends/SecretService.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     4904 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/backends/Windows.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     5859 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/backends/_OS_X_API.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)        0 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/backends/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      662 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/backends/fail.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3878 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/backends/kwallet.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-07-14 14:12:52.000000 keyring-9.3.1/keyring/tests/
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-07-14 14:12:52.000000 keyring-9.3.1/keyring/tests/backends/
+-rw-rw-r--   0 travis    (1000) travis    (1000)        0 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/tests/backends/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      394 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/tests/backends/test_OS_X.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      865 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/tests/backends/test_SecretService.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      911 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/tests/backends/test_Windows.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2782 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/tests/backends/test_kwallet.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)       87 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/tests/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     5109 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/tests/test_backend.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1924 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/tests/util.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-07-14 14:12:52.000000 keyring-9.3.1/keyring/util/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      864 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/util/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1497 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/util/escape.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2231 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/util/platform_.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1337 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/util/properties.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      398 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/__init__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)       70 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/__main__.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     5023 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/backend.py
+-rwxrwxr-x   0 travis    (1000) travis    (1000)     3369 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/cli.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3985 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/core.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1355 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/credentials.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1180 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/errors.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      312 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/getpassbackend.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1255 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/http.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1008 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/py27compat.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      660 2016-07-14 14:12:11.000000 keyring-9.3.1/keyring/py33compat.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2016-07-14 14:12:52.000000 keyring-9.3.1/keyring.egg-info/
+-rw-rw-r--   0 travis    (1000) travis    (1000)    15030 2016-07-14 14:12:52.000000 keyring-9.3.1/keyring.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1141 2016-07-14 14:12:52.000000 keyring-9.3.1/keyring.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)        1 2016-07-14 14:12:52.000000 keyring-9.3.1/keyring.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)       46 2016-07-14 14:12:52.000000 keyring-9.3.1/keyring.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)      127 2016-07-14 14:12:52.000000 keyring-9.3.1/keyring.egg-info/requires.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)        8 2016-07-14 14:12:52.000000 keyring-9.3.1/keyring.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)      737 2016-07-14 14:12:11.000000 keyring-9.3.1/.gitignore
+-rw-rw-r--   0 travis    (1000) travis    (1000)     5380 2016-07-14 14:12:11.000000 keyring-9.3.1/.hgtags
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1117 2016-07-14 14:12:11.000000 keyring-9.3.1/.travis.yml
+-rw-rw-r--   0 travis    (1000) travis    (1000)    24057 2016-07-14 14:12:11.000000 keyring-9.3.1/CHANGES.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)    11496 2016-07-14 14:12:11.000000 keyring-9.3.1/README.rst
+-rw-rw-r--   0 travis    (1000) travis    (1000)       52 2016-07-14 14:12:11.000000 keyring-9.3.1/conftest.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      394 2016-07-14 14:12:11.000000 keyring-9.3.1/hook-keyring.backend.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      154 2016-07-14 14:12:11.000000 keyring-9.3.1/pytest.ini
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2188 2016-07-14 14:12:11.000000 keyring-9.3.1/setup.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    15030 2016-07-14 14:12:52.000000 keyring-9.3.1/PKG-INFO
+-rw-rw-r--   0 travis    (1000) travis    (1000)      179 2016-07-14 14:12:52.000000 keyring-9.3.1/setup.cfg
```

### Comparing `keyring-9.3/docs/conf.py` & `keyring-9.3.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/backends/OS_X.py` & `keyring-9.3.1/keyring/backends/OS_X.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/backends/SecretService.py` & `keyring-9.3.1/keyring/backends/SecretService.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/backends/Windows.py` & `keyring-9.3.1/keyring/backends/Windows.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/backends/_OS_X_API.py` & `keyring-9.3.1/keyring/backends/_OS_X_API.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/backends/fail.py` & `keyring-9.3.1/keyring/backends/fail.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/backends/kwallet.py` & `keyring-9.3.1/keyring/backends/kwallet.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,16 +78,17 @@
         """Get password of the username for the service
         """
         if not self.connected(service):
             # the user pressed "cancel" when prompted to unlock their keyring.
             return None
         if not self.iface.hasEntry(self.handle, service, username, self.appid):
             return None
-        return self.iface.readPassword(
+        password = self.iface.readPassword(
             self.handle, service, username, self.appid)
+        return str(password)
 
     def set_password(self, service, username, password):
         """Set password for the username of the service
         """
         if not self.connected(service):
             # the user pressed "cancel" when prompted to unlock their keyring.
             raise PasswordSetError("Cancelled by user")
```

### Comparing `keyring-9.3/keyring/tests/backends/test_SecretService.py` & `keyring-9.3.1/keyring/tests/backends/test_SecretService.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/tests/backends/test_Windows.py` & `keyring-9.3.1/keyring/tests/backends/test_Windows.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/tests/backends/test_kwallet.py` & `keyring-9.3.1/keyring/tests/backends/test_kwallet.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/tests/test_backend.py` & `keyring-9.3.1/keyring/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/tests/util.py` & `keyring-9.3.1/keyring/tests/util.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/util/__init__.py` & `keyring-9.3.1/keyring/util/__init__.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/util/escape.py` & `keyring-9.3.1/keyring/util/escape.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/util/platform_.py` & `keyring-9.3.1/keyring/util/platform_.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/util/properties.py` & `keyring-9.3.1/keyring/util/properties.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/backend.py` & `keyring-9.3.1/keyring/backend.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/cli.py` & `keyring-9.3.1/keyring/cli.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/core.py` & `keyring-9.3.1/keyring/core.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/credentials.py` & `keyring-9.3.1/keyring/credentials.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/errors.py` & `keyring-9.3.1/keyring/errors.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/http.py` & `keyring-9.3.1/keyring/http.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/py27compat.py` & `keyring-9.3.1/keyring/py27compat.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring/py33compat.py` & `keyring-9.3.1/keyring/py33compat.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/keyring.egg-info/PKG-INFO` & `keyring-9.3.1/keyring.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: keyring
-Version: 9.3
+Version: 9.3.1
 Summary: Store and access your passwords safely.
 Home-page: https://github.com/jaraco/keyring
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 License: UNKNOWN
 Description: =======================================
         Installing and Using Python Keyring Lib
@@ -291,15 +291,15 @@
         To run the tests yourself, you'll want keyring installed to some environment
         in which it can be tested. Recommended techniques are described below.
         
         Using pytest runner
         -------------------
         
         Keyring is instrumented with `pytest runner
-        <https://bitbucket.org/jaraco/pytest-runner>`_. Thus, you may invoke the tests
+        <https://github.com/pytest-dev/pytest-runner>`_. Thus, you may invoke the tests
         from any supported Python (with setuptools installed) using this command::
         
             python setup.py test
         
         pytest runner will download any unmet dependencies and run the tests using
         `pytest <https://bitbucket.org/hpk42/pytest>`_.
         
@@ -341,14 +341,19 @@
         The project was based on Tarek Ziade's idea in `this post`_. Kang Zhang
         initially carried it out as a `Google Summer of Code`_ project, and Tarek
         mentored Kang on this project.
         
         .. _this post: http://tarekziade.wordpress.com/2009/03/27/pycon-hallway-session-1-a-keyring-library-for-python/
         .. _Google Summer of Code: http://socghop.appspot.com/
         
+        
+        .. image:: https://badges.gitter.im/jaraco/keyring.svg
+           :alt: Join the chat at https://gitter.im/jaraco/keyring
+           :target: https://gitter.im/jaraco/keyring?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+        
 Keywords: keyring Keychain GnomeKeyring Kwallet password storage
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `keyring-9.3/keyring.egg-info/SOURCES.txt` & `keyring-9.3.1/keyring.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keyring-9.3/.gitignore` & `keyring-9.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `keyring-9.3/.hgtags` & `keyring-9.3.1/.hgtags`

 * *Files 1% similar despite different names*

```diff
@@ -110,7 +110,8 @@
 45a70dfe822cbdc889142e1d984a5074396ba711 8.6
 87d6d34cdea1b3b40bb60c3286b672c69ec49223 8.6.1
 d8633f6d4baf8abcffa80c456a89bf0ff09ff706 8.7
 a17bfebdf428e42ff31b71beee3e700b8329acdf 9.0
 e0adabb76d3d729c55c9211d9f5314fcce210149 9.1
 074f2c9cade6bc89372133e6d2674cfcff4b4194 9.2
 3cc50ae65bc4ceef0ce7d06f8b455d3e655396f3 9.2.1
+94e5cb8fd63b71ed9f711d3c3abeaaf9b7fd0e1d 9.3
```

### Comparing `keyring-9.3/.travis.yml` & `keyring-9.3.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `keyring-9.3/CHANGES.rst` & `keyring-9.3.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 CHANGES
 =======
 
+9.3.1
+-----
+
+* Link to the new Gitter chat room is now in the
+  readme.
+* Issue #235: ``kwallet`` backend now returns
+  string objects instead of ``dbus.String`` objects,
+  for less surprising reprs.
+* Minor doc fixes.
+
 9.3
 ---
 
-* Pull Request #226: In SecretService backend, unlock
+* Issue #161: In SecretService backend, unlock
   individual entries.
 
 9.2.1
 -----
 
 * Issue #230: Don't rely on dbus-python and instead
   defer to SecretStorage to describe the installation
```

### Comparing `keyring-9.3/README.rst` & `keyring-9.3.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -283,15 +283,15 @@
 To run the tests yourself, you'll want keyring installed to some environment
 in which it can be tested. Recommended techniques are described below.
 
 Using pytest runner
 -------------------
 
 Keyring is instrumented with `pytest runner
-<https://bitbucket.org/jaraco/pytest-runner>`_. Thus, you may invoke the tests
+<https://github.com/pytest-dev/pytest-runner>`_. Thus, you may invoke the tests
 from any supported Python (with setuptools installed) using this command::
 
     python setup.py test
 
 pytest runner will download any unmet dependencies and run the tests using
 `pytest <https://bitbucket.org/hpk42/pytest>`_.
 
@@ -332,7 +332,12 @@
 
 The project was based on Tarek Ziade's idea in `this post`_. Kang Zhang
 initially carried it out as a `Google Summer of Code`_ project, and Tarek
 mentored Kang on this project.
 
 .. _this post: http://tarekziade.wordpress.com/2009/03/27/pycon-hallway-session-1-a-keyring-library-for-python/
 .. _Google Summer of Code: http://socghop.appspot.com/
+
+
+.. image:: https://badges.gitter.im/jaraco/keyring.svg
+   :alt: Join the chat at https://gitter.im/jaraco/keyring
+   :target: https://gitter.im/jaraco/keyring?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
```

### Comparing `keyring-9.3/setup.py` & `keyring-9.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `keyring-9.3/PKG-INFO` & `keyring-9.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: keyring
-Version: 9.3
+Version: 9.3.1
 Summary: Store and access your passwords safely.
 Home-page: https://github.com/jaraco/keyring
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 License: UNKNOWN
 Description: =======================================
         Installing and Using Python Keyring Lib
@@ -291,15 +291,15 @@
         To run the tests yourself, you'll want keyring installed to some environment
         in which it can be tested. Recommended techniques are described below.
         
         Using pytest runner
         -------------------
         
         Keyring is instrumented with `pytest runner
-        <https://bitbucket.org/jaraco/pytest-runner>`_. Thus, you may invoke the tests
+        <https://github.com/pytest-dev/pytest-runner>`_. Thus, you may invoke the tests
         from any supported Python (with setuptools installed) using this command::
         
             python setup.py test
         
         pytest runner will download any unmet dependencies and run the tests using
         `pytest <https://bitbucket.org/hpk42/pytest>`_.
         
@@ -341,14 +341,19 @@
         The project was based on Tarek Ziade's idea in `this post`_. Kang Zhang
         initially carried it out as a `Google Summer of Code`_ project, and Tarek
         mentored Kang on this project.
         
         .. _this post: http://tarekziade.wordpress.com/2009/03/27/pycon-hallway-session-1-a-keyring-library-for-python/
         .. _Google Summer of Code: http://socghop.appspot.com/
         
+        
+        .. image:: https://badges.gitter.im/jaraco/keyring.svg
+           :alt: Join the chat at https://gitter.im/jaraco/keyring
+           :target: https://gitter.im/jaraco/keyring?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+        
 Keywords: keyring Keychain GnomeKeyring Kwallet password storage
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Python Software Foundation License
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
```

