# Comparing `tmp/jupyter-rsession-proxy-2.1.0.tar.gz` & `tmp/jupyter-rsession-proxy-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jupyter-rsession-proxy-2.1.0.tar", last modified: Wed Sep  7 22:38:54 2022, max compression
+gzip compressed data, was "jupyter-rsession-proxy-2.2.0.tar", last modified: Fri Jun 23 00:49:47 2023, max compression
```

## Comparing `jupyter-rsession-proxy-2.1.0.tar` & `jupyter-rsession-proxy-2.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rylo      (1463) scfstaff   (920)        0 2022-09-07 22:38:53.997356 jupyter-rsession-proxy-2.1.0/
--rw-r--r--   0 rylo      (1463) scfstaff   (920)     1528 2022-09-07 22:37:38.000000 jupyter-rsession-proxy-2.1.0/LICENSE
--rw-r--r--   0 rylo      (1463) scfstaff   (920)       16 2022-09-07 22:37:38.000000 jupyter-rsession-proxy-2.1.0/MANIFEST.in
--rw-r--r--   0 rylo      (1463) scfstaff   (920)      336 2022-09-07 22:38:54.001356 jupyter-rsession-proxy-2.1.0/PKG-INFO
--rw-r--r--   0 rylo      (1463) scfstaff   (920)     2061 2022-09-07 22:37:38.000000 jupyter-rsession-proxy-2.1.0/README.md
-drwxr-xr-x   0 rylo      (1463) scfstaff   (920)        0 2022-09-07 22:38:53.985356 jupyter-rsession-proxy-2.1.0/jupyter_rsession_proxy/
--rw-r--r--   0 rylo      (1463) scfstaff   (920)     5319 2022-09-07 22:37:38.000000 jupyter-rsession-proxy-2.1.0/jupyter_rsession_proxy/__init__.py
-drwxr-xr-x   0 rylo      (1463) scfstaff   (920)        0 2022-09-07 22:38:53.997356 jupyter-rsession-proxy-2.1.0/jupyter_rsession_proxy/icons/
--rw-r--r--   0 rylo      (1463) scfstaff   (920)     1313 2022-09-07 22:37:38.000000 jupyter-rsession-proxy-2.1.0/jupyter_rsession_proxy/icons/rstudio.svg
-drwxr-xr-x   0 rylo      (1463) scfstaff   (920)        0 2022-09-07 22:38:53.997356 jupyter-rsession-proxy-2.1.0/jupyter_rsession_proxy.egg-info/
--rw-r--r--   0 rylo      (1463) scfstaff   (920)      336 2022-09-07 22:38:53.000000 jupyter-rsession-proxy-2.1.0/jupyter_rsession_proxy.egg-info/PKG-INFO
--rw-r--r--   0 rylo      (1463) scfstaff   (920)      402 2022-09-07 22:38:53.000000 jupyter-rsession-proxy-2.1.0/jupyter_rsession_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 rylo      (1463) scfstaff   (920)        1 2022-09-07 22:38:53.000000 jupyter-rsession-proxy-2.1.0/jupyter_rsession_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 rylo      (1463) scfstaff   (920)       78 2022-09-07 22:38:53.000000 jupyter-rsession-proxy-2.1.0/jupyter_rsession_proxy.egg-info/entry_points.txt
--rw-r--r--   0 rylo      (1463) scfstaff   (920)       28 2022-09-07 22:38:53.000000 jupyter-rsession-proxy-2.1.0/jupyter_rsession_proxy.egg-info/requires.txt
--rw-r--r--   0 rylo      (1463) scfstaff   (920)       23 2022-09-07 22:38:53.000000 jupyter-rsession-proxy-2.1.0/jupyter_rsession_proxy.egg-info/top_level.txt
--rw-r--r--   0 rylo      (1463) scfstaff   (920)       74 2022-09-07 22:38:54.001356 jupyter-rsession-proxy-2.1.0/setup.cfg
--rw-r--r--   0 rylo      (1463) scfstaff   (920)      644 2022-09-07 22:37:38.000000 jupyter-rsession-proxy-2.1.0/setup.py
+drwxr-xr-x   0 rylo      (1463) scfstaff   (920)        0 2023-06-23 00:49:47.550526 jupyter-rsession-proxy-2.2.0/
+-rw-r--r--   0 rylo      (1463) scfstaff   (920)     1528 2022-09-07 22:37:38.000000 jupyter-rsession-proxy-2.2.0/LICENSE
+-rw-r--r--   0 rylo      (1463) scfstaff   (920)       16 2022-09-07 22:37:38.000000 jupyter-rsession-proxy-2.2.0/MANIFEST.in
+-rw-r--r--   0 rylo      (1463) scfstaff   (920)      280 2023-06-23 00:49:47.550526 jupyter-rsession-proxy-2.2.0/PKG-INFO
+-rw-r--r--   0 rylo      (1463) scfstaff   (920)     2061 2022-09-07 22:37:38.000000 jupyter-rsession-proxy-2.2.0/README.md
+drwxr-xr-x   0 rylo      (1463) scfstaff   (920)        0 2023-06-23 00:49:47.534526 jupyter-rsession-proxy-2.2.0/jupyter_rsession_proxy/
+-rw-r--r--   0 rylo      (1463) scfstaff   (920)     5359 2023-06-12 17:12:34.000000 jupyter-rsession-proxy-2.2.0/jupyter_rsession_proxy/__init__.py
+drwxr-xr-x   0 rylo      (1463) scfstaff   (920)        0 2023-06-23 00:49:47.550526 jupyter-rsession-proxy-2.2.0/jupyter_rsession_proxy/icons/
+-rw-r--r--   0 rylo      (1463) scfstaff   (920)     1313 2022-09-07 22:37:38.000000 jupyter-rsession-proxy-2.2.0/jupyter_rsession_proxy/icons/rstudio.svg
+drwxr-xr-x   0 rylo      (1463) scfstaff   (920)        0 2023-06-23 00:49:47.546526 jupyter-rsession-proxy-2.2.0/jupyter_rsession_proxy.egg-info/
+-rw-r--r--   0 rylo      (1463) scfstaff   (920)      280 2023-06-23 00:49:47.000000 jupyter-rsession-proxy-2.2.0/jupyter_rsession_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 rylo      (1463) scfstaff   (920)      402 2023-06-23 00:49:47.000000 jupyter-rsession-proxy-2.2.0/jupyter_rsession_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 rylo      (1463) scfstaff   (920)        1 2023-06-23 00:49:47.000000 jupyter-rsession-proxy-2.2.0/jupyter_rsession_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 rylo      (1463) scfstaff   (920)       77 2023-06-23 00:49:47.000000 jupyter-rsession-proxy-2.2.0/jupyter_rsession_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 rylo      (1463) scfstaff   (920)       28 2023-06-23 00:49:47.000000 jupyter-rsession-proxy-2.2.0/jupyter_rsession_proxy.egg-info/requires.txt
+-rw-r--r--   0 rylo      (1463) scfstaff   (920)       23 2023-06-23 00:49:47.000000 jupyter-rsession-proxy-2.2.0/jupyter_rsession_proxy.egg-info/top_level.txt
+-rw-r--r--   0 rylo      (1463) scfstaff   (920)       74 2023-06-23 00:49:47.550526 jupyter-rsession-proxy-2.2.0/setup.cfg
+-rw-r--r--   0 rylo      (1463) scfstaff   (920)      644 2023-06-12 17:14:51.000000 jupyter-rsession-proxy-2.2.0/setup.py
```

### Comparing `jupyter-rsession-proxy-2.1.0/LICENSE` & `jupyter-rsession-proxy-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-rsession-proxy-2.1.0/README.md` & `jupyter-rsession-proxy-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyter-rsession-proxy-2.1.0/jupyter_rsession_proxy/__init__.py` & `jupyter-rsession-proxy-2.2.0/jupyter_rsession_proxy/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,26 +27,25 @@
     raise FileNotFoundError(f'Could not find {prog} in PATH')
 
 def get_icon_path():
     return os.path.join(
         os.path.dirname(os.path.abspath(__file__)), 'icons', 'rstudio.svg'
     )
 
-def rewrite_auth(response, request):
+def rewrite_netloc(response, request):
     '''
-       As of rstudio-server 1.4ish, it would send the client to /auth-sign-in
-       rather than what the client sees as the full URL followed by
-       /auth-sign-in. See rstudio/rstudio#8888. We rewrite the response by
-       sending the client to the right place.
+       In some circumstances, rstudio-server appends a port to the URL while
+       setting Location in the header. We rewrite the response to use the host
+       in the request.
     '''
     for header, v in response.headers.get_all():
-        if header == "Location" and v.startswith("/auth-sign-in"):
-            # Visit the correct page
-            u = urlparse(request.uri)
-            response.headers[header] = urlunparse(u._replace(path=u.path+v))
+        if header == "Location":
+            u = urlparse(v)
+            if u.netloc != request.host:
+                response.headers[header] = urlunparse(u._replace(netloc=request.host))
 
 def get_system_user():
     try:
         user = pwd.getpwuid(os.getuid())[0]
     except:
         user = os.environ.get('NB_USER', getpass.getuser())
     return(user)
@@ -103,21 +102,24 @@
             cmd.append(f'--server-data-dir={server_data_dir}')
         if _support_arg('database-config-file'):
             cmd.append(f'--database-config-file={database_config_file}')
 
         return cmd
 
     def _get_timeout(default=15):
-        return os.getenv('RSERVER_TIMEOUT', default)
+        try:
+            return float(os.getenv('RSERVER_TIMEOUT', default))
+        except Exception:
+            return default
 
     server_process = {
         'command': _get_cmd,
         'timeout': _get_timeout(),
         'environment': _get_env,
-        'rewrite_response': rewrite_auth,
+        'rewrite_response': rewrite_netloc,
         'launcher_entry': {
             'title': 'RStudio',
             'icon_path': get_icon_path()
         }
     }
     return server_process
 
@@ -149,15 +151,18 @@
             '--log-stderr=1',
             '--session-timeout-minutes=0',
             '--user-identity=' + get_system_user(),
             '--www-port=' + str(port)
         ]
 
     def _get_timeout(default=15):
-        return os.getenv('RSESSION_TIMEOUT', default)
+        try:
+            return float(os.getenv('RSESSION_TIMEOUT', default))
+        except Exception:
+            return default
 
     return {
         'command': _get_cmd,
         'timeout': _get_timeout(),
         'environment': _get_env,
         'launcher_entry': {
             'title': 'RStudio',
```

### Comparing `jupyter-rsession-proxy-2.1.0/jupyter_rsession_proxy/icons/rstudio.svg` & `jupyter-rsession-proxy-2.2.0/jupyter_rsession_proxy/icons/rstudio.svg`

 * *Files identical despite different names*

### Comparing `jupyter-rsession-proxy-2.1.0/setup.py` & `jupyter-rsession-proxy-2.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 setuptools.setup(
     name="jupyter-rsession-proxy",
-    version='2.1.0',
+    version='2.2.0',
     url="https://github.com/jupyterhub/jupyter-rsession-proxy",
     author="Ryan Lovett & Yuvi Panda",
     description="Jupyter extension to proxy RStudio",
     packages=setuptools.find_packages(),
 	keywords=['Jupyter'],
 	classifiers=['Framework :: Jupyter'],
     install_requires=[
-        'jupyter-server-proxy>=3.2.0'
+        'jupyter-server-proxy>=3.2.2'
     ],
     entry_points={
         'jupyter_serverproxy_servers': [
             'rstudio = jupyter_rsession_proxy:setup_rserver'
         ]
     },
     package_data={
```

