# Comparing `tmp/platformdirs-3.7.0.tar.gz` & `tmp/platformdirs-3.8.0.tar.gz`

## Comparing `platformdirs-3.7.0.tar` & `platformdirs-3.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 platformdirs-3.7.0/tox.ini
--rw-r--r--   0        0        0    20083 2020-02-02 00:00:00.000000 platformdirs-3.7.0/src/platformdirs/__init__.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 platformdirs-3.7.0/src/platformdirs/__main__.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 platformdirs-3.7.0/src/platformdirs/android.py
--rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 platformdirs-3.7.0/src/platformdirs/api.py
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 platformdirs-3.7.0/src/platformdirs/macos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.7.0/src/platformdirs/py.typed
--rw-r--r--   0        0        0     8643 2020-02-02 00:00:00.000000 platformdirs-3.7.0/src/platformdirs/unix.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.7.0/src/platformdirs/version.py
--rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 platformdirs-3.7.0/src/platformdirs/windows.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 platformdirs-3.7.0/tests/conftest.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 platformdirs-3.7.0/tests/test_android.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 platformdirs-3.7.0/tests/test_api.py
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 platformdirs-3.7.0/tests/test_comp_with_appdirs.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 platformdirs-3.7.0/tests/test_macos.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.7.0/tests/test_main.py
--rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 platformdirs-3.7.0/tests/test_unix.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.7.0/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.7.0/LICENSE
--rw-r--r--   0        0        0     7814 2020-02-02 00:00:00.000000 platformdirs-3.7.0/README.rst
--rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 platformdirs-3.7.0/pyproject.toml
--rw-r--r--   0        0        0     9961 2020-02-02 00:00:00.000000 platformdirs-3.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tox.ini
+-rw-r--r--   0        0        0    20083 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/__init__.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/__main__.py
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/android.py
+-rw-r--r--   0        0        0     7120 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/api.py
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/macos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/py.typed
+-rw-r--r--   0        0        0     8643 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/unix.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/version.py
+-rw-r--r--   0        0        0     9573 2020-02-02 00:00:00.000000 platformdirs-3.8.0/src/platformdirs/windows.py
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tests/conftest.py
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tests/test_android.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tests/test_api.py
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tests/test_comp_with_appdirs.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tests/test_macos.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tests/test_main.py
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 platformdirs-3.8.0/tests/test_unix.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 platformdirs-3.8.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 platformdirs-3.8.0/LICENSE
+-rw-r--r--   0        0        0     8955 2020-02-02 00:00:00.000000 platformdirs-3.8.0/README.rst
+-rw-r--r--   0        0        0     3759 2020-02-02 00:00:00.000000 platformdirs-3.8.0/pyproject.toml
+-rw-r--r--   0        0        0    11102 2020-02-02 00:00:00.000000 platformdirs-3.8.0/PKG-INFO
```

### Comparing `platformdirs-3.7.0/tox.ini` & `platformdirs-3.8.0/tox.ini`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/src/platformdirs/__init__.py` & `platformdirs-3.8.0/src/platformdirs/__init__.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/src/platformdirs/__main__.py` & `platformdirs-3.8.0/src/platformdirs/__main__.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/src/platformdirs/android.py` & `platformdirs-3.8.0/src/platformdirs/android.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/src/platformdirs/api.py` & `platformdirs-3.8.0/src/platformdirs/api.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/src/platformdirs/macos.py` & `platformdirs-3.8.0/src/platformdirs/macos.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/src/platformdirs/unix.py` & `platformdirs-3.8.0/src/platformdirs/unix.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/src/platformdirs/windows.py` & `platformdirs-3.8.0/src/platformdirs/windows.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/tests/conftest.py` & `platformdirs-3.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/tests/test_android.py` & `platformdirs-3.8.0/tests/test_android.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/tests/test_api.py` & `platformdirs-3.8.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/tests/test_comp_with_appdirs.py` & `platformdirs-3.8.0/tests/test_comp_with_appdirs.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/tests/test_macos.py` & `platformdirs-3.8.0/tests/test_macos.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/tests/test_unix.py` & `platformdirs-3.8.0/tests/test_unix.py`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/LICENSE` & `platformdirs-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/README.rst` & `platformdirs-3.8.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 - user config dir (``user_config_dir``)
 - user cache dir (``user_cache_dir``)
 - site data dir (``site_data_dir``)
 - site config dir (``site_config_dir``)
 - user log dir (``user_log_dir``)
 - user documents dir (``user_documents_dir``)
 - user downloads dir (``user_downloads_dir``)
+- user pictures dir (``user_pictures_dir``)
+- user videos dir (``user_videos_dir``)
+- user music dir (``user_music_dir``)
 - user runtime dir (``user_runtime_dir``)
 
 And also:
 
 - Is slightly opinionated on the directory names used. Look for "OPINION" in
   documentation and code for when an opinion is being applied.
 
@@ -67,14 +70,20 @@
     '/Users/trentm/Library/Caches/SuperApp'
     >>> user_log_dir(appname, appauthor)
     '/Users/trentm/Library/Logs/SuperApp'
     >>> user_documents_dir()
     '/Users/trentm/Documents'
     >>> user_downloads_dir()
     '/Users/trentm/Downloads'
+    >>> user_pictures_dir()
+    '/Users/trentm/Pictures'
+    >>> user_videos_dir()
+    '/Users/trentm/Movies'
+    >>> user_music_dir()
+    '/Users/trentm/Music'
     >>> user_runtime_dir(appname, appauthor)
     '/Users/trentm/Library/Caches/TemporaryItems/SuperApp'
 
 On Windows:
 
 .. code-block:: pycon
 
@@ -89,14 +98,20 @@
     'C:\\Users\\trentm\\AppData\\Local\\Acme\\SuperApp\\Cache'
     >>> user_log_dir(appname, appauthor)
     'C:\\Users\\trentm\\AppData\\Local\\Acme\\SuperApp\\Logs'
     >>> user_documents_dir()
     'C:\\Users\\trentm\\Documents'
     >>> user_downloads_dir()
     'C:\\Users\\trentm\\Downloads'
+    >>> user_pictures_dir()
+    'C:\\Users\\trentm\\Pictures'
+    >>> user_videos_dir()
+    'C:\\Users\\trentm\\Videos'
+    >>> user_music_dir()
+    'C:\\Users\\trentm\\Music'
     >>> user_runtime_dir(appname, appauthor)
     'C:\\Users\\trentm\\AppData\\Local\\Temp\\Acme\\SuperApp'
 
 On Linux:
 
 .. code-block:: pycon
 
@@ -115,14 +130,20 @@
     '/home/trentm/.cache/SuperApp/log'
     >>> user_config_dir(appname)
     '/home/trentm/.config/SuperApp'
     >>> user_documents_dir()
     '/home/trentm/Documents'
     >>> user_downloads_dir()
     '/home/trentm/Downloads'
+    >>> user_pictures_dir()
+    '/home/trentm/Pictures'
+    >>> user_videos_dir()
+    '/home/trentm/Videos'
+    >>> user_music_dir()
+    '/home/trentm/Music'
     >>> user_runtime_dir(appname, appauthor)
     '/run/user/{os.getuid()}/SuperApp'
     >>> site_config_dir(appname)
     '/etc/xdg/SuperApp'
     >>> os.environ["XDG_CONFIG_DIRS"] = "/etc:/usr/local/etc"
     >>> site_config_dir(appname, multipath=True)
     '/etc/SuperApp:/usr/local/etc/SuperApp'
@@ -140,14 +161,20 @@
     '/data/data/com.myApp/cache/SuperApp/log'
     >>> user_config_dir(appname)
     '/data/data/com.myApp/shared_prefs/SuperApp'
     >>> user_documents_dir()
     '/storage/emulated/0/Documents'
     >>> user_downloads_dir()
     '/storage/emulated/0/Downloads'
+    >>> user_pictures_dir()
+    '/storage/emulated/0/Pictures'
+    >>> user_videos_dir()
+    '/storage/emulated/0/DCIM/Camera'
+    >>> user_music_dir()
+    '/storage/emulated/0/Music'
     >>> user_runtime_dir(appname, appauthor)
     '/data/data/com.myApp/cache/SuperApp/tmp'
 
 Note: Some android apps like Termux and Pydroid are used as shells. These
 apps are used by the end user to emulate Linux environment. Presence of
 ``SHELL`` environment variable is used by Platformdirs to differentiate
 between general android apps and android apps used as shells. Shell android
@@ -169,14 +196,20 @@
     '/Users/trentm/Library/Caches/SuperApp'
     >>> dirs.user_log_dir
     '/Users/trentm/Library/Logs/SuperApp'
     >>> dirs.user_documents_dir
     '/Users/trentm/Documents'
     >>> dirs.user_downloads_dir
     '/Users/trentm/Downloads'
+    >>> dirs.user_pictures_dir
+    '/Users/trentm/Pictures'
+    >>> dirs.user_videos_dir
+    '/Users/trentm/Movies'
+    >>> dirs.user_music_dir
+    '/Users/trentm/Music'
     >>> dirs.user_runtime_dir
     '/Users/trentm/Library/Caches/TemporaryItems/SuperApp'
 
 Per-version isolation
 =====================
 
 If you have multiple versions of your app in use that you want to be
@@ -193,14 +226,20 @@
     '/Users/trentm/Library/Caches/SuperApp/1.0'
     >>> dirs.user_log_dir
     '/Users/trentm/Library/Logs/SuperApp/1.0'
     >>> dirs.user_documents_dir
     '/Users/trentm/Documents'
     >>> dirs.user_downloads_dir
     '/Users/trentm/Downloads'
+    >>> dirs.user_pictures_dir
+    '/Users/trentm/Pictures'
+    >>> dirs.user_videos_dir
+    '/Users/trentm/Movies'
+    >>> dirs.user_music_dir
+    '/Users/trentm/Music'
     >>> dirs.user_runtime_dir
     '/Users/trentm/Library/Caches/TemporaryItems/SuperApp/1.0'
 
 Be wary of using this for configuration files though; you'll need to handle
 migrating configuration files manually.
 
 Why this Fork?
```

### Comparing `platformdirs-3.7.0/pyproject.toml` & `platformdirs-3.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `platformdirs-3.7.0/PKG-INFO` & `platformdirs-3.8.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: platformdirs
-Version: 3.7.0
+Version: 3.8.0
 Summary: A small Python package for determining appropriate platform-specific dirs, e.g. a "user data dir".
 Project-URL: Documentation, https://platformdirs.readthedocs.io
 Project-URL: Homepage, https://github.com/platformdirs/platformdirs
 Project-URL: Source, https://github.com/platformdirs/platformdirs
 Project-URL: Tracker, https://github.com/platformdirs/platformdirs/issues
 Maintainer-email: Bernát Gábor <gaborjbernat@gmail.com>, Julian Berman <Julian@GrayVines.com>, Ofek Lev <oss@ofek.dev>, Ronny Pfannschmidt <opensource@ronnypfannschmidt.de>
 License-Expression: MIT
@@ -80,14 +80,17 @@
 - user config dir (``user_config_dir``)
 - user cache dir (``user_cache_dir``)
 - site data dir (``site_data_dir``)
 - site config dir (``site_config_dir``)
 - user log dir (``user_log_dir``)
 - user documents dir (``user_documents_dir``)
 - user downloads dir (``user_downloads_dir``)
+- user pictures dir (``user_pictures_dir``)
+- user videos dir (``user_videos_dir``)
+- user music dir (``user_music_dir``)
 - user runtime dir (``user_runtime_dir``)
 
 And also:
 
 - Is slightly opinionated on the directory names used. Look for "OPINION" in
   documentation and code for when an opinion is being applied.
 
@@ -109,14 +112,20 @@
     '/Users/trentm/Library/Caches/SuperApp'
     >>> user_log_dir(appname, appauthor)
     '/Users/trentm/Library/Logs/SuperApp'
     >>> user_documents_dir()
     '/Users/trentm/Documents'
     >>> user_downloads_dir()
     '/Users/trentm/Downloads'
+    >>> user_pictures_dir()
+    '/Users/trentm/Pictures'
+    >>> user_videos_dir()
+    '/Users/trentm/Movies'
+    >>> user_music_dir()
+    '/Users/trentm/Music'
     >>> user_runtime_dir(appname, appauthor)
     '/Users/trentm/Library/Caches/TemporaryItems/SuperApp'
 
 On Windows:
 
 .. code-block:: pycon
 
@@ -131,14 +140,20 @@
     'C:\\Users\\trentm\\AppData\\Local\\Acme\\SuperApp\\Cache'
     >>> user_log_dir(appname, appauthor)
     'C:\\Users\\trentm\\AppData\\Local\\Acme\\SuperApp\\Logs'
     >>> user_documents_dir()
     'C:\\Users\\trentm\\Documents'
     >>> user_downloads_dir()
     'C:\\Users\\trentm\\Downloads'
+    >>> user_pictures_dir()
+    'C:\\Users\\trentm\\Pictures'
+    >>> user_videos_dir()
+    'C:\\Users\\trentm\\Videos'
+    >>> user_music_dir()
+    'C:\\Users\\trentm\\Music'
     >>> user_runtime_dir(appname, appauthor)
     'C:\\Users\\trentm\\AppData\\Local\\Temp\\Acme\\SuperApp'
 
 On Linux:
 
 .. code-block:: pycon
 
@@ -157,14 +172,20 @@
     '/home/trentm/.cache/SuperApp/log'
     >>> user_config_dir(appname)
     '/home/trentm/.config/SuperApp'
     >>> user_documents_dir()
     '/home/trentm/Documents'
     >>> user_downloads_dir()
     '/home/trentm/Downloads'
+    >>> user_pictures_dir()
+    '/home/trentm/Pictures'
+    >>> user_videos_dir()
+    '/home/trentm/Videos'
+    >>> user_music_dir()
+    '/home/trentm/Music'
     >>> user_runtime_dir(appname, appauthor)
     '/run/user/{os.getuid()}/SuperApp'
     >>> site_config_dir(appname)
     '/etc/xdg/SuperApp'
     >>> os.environ["XDG_CONFIG_DIRS"] = "/etc:/usr/local/etc"
     >>> site_config_dir(appname, multipath=True)
     '/etc/SuperApp:/usr/local/etc/SuperApp'
@@ -182,14 +203,20 @@
     '/data/data/com.myApp/cache/SuperApp/log'
     >>> user_config_dir(appname)
     '/data/data/com.myApp/shared_prefs/SuperApp'
     >>> user_documents_dir()
     '/storage/emulated/0/Documents'
     >>> user_downloads_dir()
     '/storage/emulated/0/Downloads'
+    >>> user_pictures_dir()
+    '/storage/emulated/0/Pictures'
+    >>> user_videos_dir()
+    '/storage/emulated/0/DCIM/Camera'
+    >>> user_music_dir()
+    '/storage/emulated/0/Music'
     >>> user_runtime_dir(appname, appauthor)
     '/data/data/com.myApp/cache/SuperApp/tmp'
 
 Note: Some android apps like Termux and Pydroid are used as shells. These
 apps are used by the end user to emulate Linux environment. Presence of
 ``SHELL`` environment variable is used by Platformdirs to differentiate
 between general android apps and android apps used as shells. Shell android
@@ -211,14 +238,20 @@
     '/Users/trentm/Library/Caches/SuperApp'
     >>> dirs.user_log_dir
     '/Users/trentm/Library/Logs/SuperApp'
     >>> dirs.user_documents_dir
     '/Users/trentm/Documents'
     >>> dirs.user_downloads_dir
     '/Users/trentm/Downloads'
+    >>> dirs.user_pictures_dir
+    '/Users/trentm/Pictures'
+    >>> dirs.user_videos_dir
+    '/Users/trentm/Movies'
+    >>> dirs.user_music_dir
+    '/Users/trentm/Music'
     >>> dirs.user_runtime_dir
     '/Users/trentm/Library/Caches/TemporaryItems/SuperApp'
 
 Per-version isolation
 =====================
 
 If you have multiple versions of your app in use that you want to be
@@ -235,14 +268,20 @@
     '/Users/trentm/Library/Caches/SuperApp/1.0'
     >>> dirs.user_log_dir
     '/Users/trentm/Library/Logs/SuperApp/1.0'
     >>> dirs.user_documents_dir
     '/Users/trentm/Documents'
     >>> dirs.user_downloads_dir
     '/Users/trentm/Downloads'
+    >>> dirs.user_pictures_dir
+    '/Users/trentm/Pictures'
+    >>> dirs.user_videos_dir
+    '/Users/trentm/Movies'
+    >>> dirs.user_music_dir
+    '/Users/trentm/Music'
     >>> dirs.user_runtime_dir
     '/Users/trentm/Library/Caches/TemporaryItems/SuperApp/1.0'
 
 Be wary of using this for configuration files though; you'll need to handle
 migrating configuration files manually.
 
 Why this Fork?
```

