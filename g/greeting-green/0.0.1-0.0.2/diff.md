# Comparing `tmp/greeting_green-0.0.1.tar.gz` & `tmp/greeting_green-0.0.2.tar.gz`

## Comparing `greeting_green-0.0.1.tar` & `greeting_green-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 greeting_green-0.0.1/src/greeting/__about__.py
--rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 greeting_green-0.0.1/src/greeting/__init__.py
--rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 greeting_green-0.0.1/src/greeting/admin.py
--rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 greeting_green-0.0.1/src/greeting/apps.py
--rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 greeting_green-0.0.1/src/greeting/models.py
--rwxr-xr-x   0        0        0      375 2020-02-02 00:00:00.000000 greeting_green-0.0.1/src/greeting/tests.py
--rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 greeting_green-0.0.1/src/greeting/urls.py
--rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 greeting_green-0.0.1/src/greeting/views.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 greeting_green-0.0.1/src/greeting/migrations/__init__.py
--rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 greeting_green-0.0.1/src/greeting/static/greeting/style.css
--rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 greeting_green-0.0.1/src/greeting/templates/greeting/index.html
--rwxr-xr-x   0        0        0       29 2020-02-02 00:00:00.000000 greeting_green-0.0.1/.gitignore
--rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 greeting_green-0.0.1/LICENSE.txt
--rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 greeting_green-0.0.1/README.md
--rwxr-xr-x   0        0        0     3237 2020-02-02 00:00:00.000000 greeting_green-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 greeting_green-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0      131 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/__about__.py
+-rwxr-xr-x   0        0        0      109 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/__init__.py
+-rwxr-xr-x   0        0        0       63 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/admin.py
+-rwxr-xr-x   0        0        0      148 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/apps.py
+-rwxr-xr-x   0        0        0       57 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/models.py
+-rwxr-xr-x   0        0        0      375 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/tests.py
+-rwxr-xr-x   0        0        0      136 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/urls.py
+-rwxr-xr-x   0        0        0      193 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/views.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/migrations/__init__.py
+-rwxr-xr-x   0        0        0       36 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/static/greeting/style.css
+-rwxr-xr-x   0        0        0      106 2020-02-02 00:00:00.000000 greeting_green-0.0.2/src/greeting/templates/greeting/index.html
+-rwxr-xr-x   0        0        0       29 2020-02-02 00:00:00.000000 greeting_green-0.0.2/.gitignore
+-rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 greeting_green-0.0.2/LICENSE.txt
+-rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 greeting_green-0.0.2/README.md
+-rwxr-xr-x   0        0        0     3237 2020-02-02 00:00:00.000000 greeting_green-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 greeting_green-0.0.2/PKG-INFO
```

### Comparing `greeting_green-0.0.1/LICENSE.txt` & `greeting_green-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `greeting_green-0.0.1/README.md` & `greeting_green-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `greeting_green-0.0.1/pyproject.toml` & `greeting_green-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `greeting_green-0.0.1/PKG-INFO` & `greeting_green-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: greeting-green
-Version: 0.0.1
+Version: 0.0.2
 Summary: あいさつ
 Project-URL: Documentation, https://github.com/unknown/greeting#readme
 Project-URL: Issues, https://github.com/unknown/greeting/issues
 Project-URL: Source, https://github.com/unknown/greeting
 Author-email: Kenno-Warise <wariken0523@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

