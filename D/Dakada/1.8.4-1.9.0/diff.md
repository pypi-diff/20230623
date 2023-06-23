# Comparing `tmp/Dakada-1.8.4.tar.gz` & `tmp/Dakada-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Dakada-1.8.4.tar", last modified: Thu Jun 22 10:43:53 2023, max compression
+gzip compressed data, was "dist\Dakada-1.9.0.tar", last modified: Fri Jun 23 08:01:05 2023, max compression
```

## Comparing `Dakada-1.8.4.tar` & `Dakada-1.9.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 10:43:53.000000 Dakada-1.8.4/
-drwxrwxrwx   0        0        0        0 2023-06-22 10:43:53.000000 Dakada-1.8.4/Dakada.egg-info/
--rw-rw-rw-   0        0        0      678 2023-06-22 10:43:53.000000 Dakada-1.8.4/Dakada.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-06-22 10:43:53.000000 Dakada-1.8.4/Dakada.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 10:43:53.000000 Dakada-1.8.4/Dakada.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-22 10:43:53.000000 Dakada-1.8.4/Dakada.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-22 10:43:53.000000 Dakada-1.8.4/Dakada.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      678 2023-06-22 10:43:53.000000 Dakada-1.8.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-22 10:43:53.000000 Dakada-1.8.4/dakada/
--rw-rw-rw-   0        0        0     8958 2023-06-22 10:43:34.000000 Dakada-1.8.4/dakada/Dakada.py
--rw-rw-rw-   0        0        0     1194 2023-06-21 12:25:24.000000 Dakada-1.8.4/dakada/User.py
--rw-rw-rw-   0        0        0        0 2023-06-18 08:03:16.000000 Dakada-1.8.4/dakada/__init__.py
--rw-rw-rw-   0        0        0     1823 2023-06-20 13:19:04.000000 Dakada-1.8.4/dakada/admin.py
--rw-rw-rw-   0        0        0      547 2023-06-18 08:21:29.000000 Dakada-1.8.4/dakada/cookie.py
--rw-rw-rw-   0        0        0      497 2023-06-20 12:22:16.000000 Dakada-1.8.4/dakada/render.py
--rw-rw-rw-   0        0        0       42 2023-06-22 10:43:53.000000 Dakada-1.8.4/setup.cfg
--rw-rw-rw-   0        0        0     3810 2023-06-22 10:42:48.000000 Dakada-1.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:01:05.000000 Dakada-1.9.0/
+drwxrwxrwx   0        0        0        0 2023-06-23 08:01:05.000000 Dakada-1.9.0/Dakada.egg-info/
+-rw-rw-rw-   0        0        0      678 2023-06-23 08:01:04.000000 Dakada-1.9.0/Dakada.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-06-23 08:01:04.000000 Dakada-1.9.0/Dakada.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 08:01:04.000000 Dakada-1.9.0/Dakada.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-06-23 08:01:04.000000 Dakada-1.9.0/Dakada.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 08:01:04.000000 Dakada-1.9.0/Dakada.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 08:01:04.000000 Dakada-1.9.0/Dakada.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      678 2023-06-23 08:01:05.000000 Dakada-1.9.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-23 08:01:05.000000 Dakada-1.9.0/dakada/
+-rw-rw-rw-   0        0        0     9005 2023-06-23 01:50:45.000000 Dakada-1.9.0/dakada/Dakada.py
+-rw-rw-rw-   0        0        0     1194 2023-06-21 12:25:24.000000 Dakada-1.9.0/dakada/User.py
+-rw-rw-rw-   0        0        0        0 2023-06-18 08:03:16.000000 Dakada-1.9.0/dakada/__init__.py
+-rw-rw-rw-   0        0        0     1823 2023-06-20 13:19:04.000000 Dakada-1.9.0/dakada/admin.py
+-rw-rw-rw-   0        0        0      547 2023-06-18 08:21:29.000000 Dakada-1.9.0/dakada/cookie.py
+-rw-rw-rw-   0        0        0      497 2023-06-20 12:22:16.000000 Dakada-1.9.0/dakada/render.py
+-rw-rw-rw-   0        0        0      256 2023-06-23 01:46:12.000000 Dakada-1.9.0/dakada/startproject.py
+-rw-rw-rw-   0        0        0       42 2023-06-23 08:01:05.000000 Dakada-1.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     3821 2023-06-23 01:51:10.000000 Dakada-1.9.0/setup.py
```

### Comparing `Dakada-1.8.4/Dakada.egg-info/PKG-INFO` & `Dakada-1.9.0/Dakada.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dakada
-Version: 1.8.4
+Version: 1.9.0
 Summary: A web framework by Dakada CN
 Home-page: https://github.com/dakadayyds/dakadaWeb
 Author: dakada
 Author-email: s75uy1e@dingtalk.com
 License: MIT
 Description: A web framework by Dakada CN
 Platform: UNKNOWN
```

### Comparing `Dakada-1.8.4/PKG-INFO` & `Dakada-1.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Dakada
-Version: 1.8.4
+Version: 1.9.0
 Summary: A web framework by Dakada CN
 Home-page: https://github.com/dakadayyds/dakadaWeb
 Author: dakada
 Author-email: s75uy1e@dingtalk.com
 License: MIT
 Description: A web framework by Dakada CN
 Platform: UNKNOWN
```

### Comparing `Dakada-1.8.4/dakada/Dakada.py` & `Dakada-1.9.0/dakada/Dakada.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,26 +38,27 @@
     HTTPdict["req_json"]=req_json
     return HTTPdict
 def load_staic(link="."):
     link+="\\staic"        
     list1=[]
     for staicname in os.listdir(link):
         global staic_header
-        staic_header="application/octet-stream"
+        staic_header="text/plain"
         with open(link+"\\"+staicname, "r", encoding="UTF8") as f:
             houzhui=staicname.split(".")[-1]
             if houzhui=="js":
                 staic_header="application/x-javascript"
             elif houzhui=="css":
                 staic_header="text/css"
             try:
                 list1.append(("/"+staicname,f.read(),staic_header,"text"))
             except UnicodeDecodeError:
                 f.close()
                 with open(link+"\\"+staicname,"rb") as f:
+                    staic_header="application/octet-stream"
                     houzhui=staicname.split(".")[-1]
                     if houzhui=="ico":
                         staic_header="application/x-ico"
                     elif houzhui=="icon":
                         staic_header="application/x-icon"
                     list1.append(("/"+staicname,f.read(),staic_header,"byte"))
             
@@ -140,15 +141,15 @@
             http=make_server(str(self.host),self.port,app)
             print("OK")
             print("starting cookiehandler...")
             t=threading.Thread(target=cookie)
             t.setDaemon(True)
             t.start()
             print("OK")
-            print("Dakada(ver 1.8.4) is running!")
+            print("Dakada(ver 1.9.0) is running!")
             if self.host=='':
                 print("View at:http://localhost:"+str(self.port))
             else:
                 print("View at:http://"+self.host+":"+str(self.port))
             http.serve_forever()
         except KeyboardInterrupt:
             print("server exit")
```

### Comparing `Dakada-1.8.4/dakada/User.py` & `Dakada-1.9.0/dakada/User.py`

 * *Files identical despite different names*

### Comparing `Dakada-1.8.4/dakada/admin.py` & `Dakada-1.9.0/dakada/admin.py`

 * *Files identical despite different names*

### Comparing `Dakada-1.8.4/dakada/cookie.py` & `Dakada-1.9.0/dakada/cookie.py`

 * *Files identical despite different names*

### Comparing `Dakada-1.8.4/setup.py` & `Dakada-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'Dakada'
 DESCRIPTION = 'A web framework by Dakada CN'
 URL = 'https://github.com/dakadayyds/dakadaWeb'
 EMAIL = 's75uy1e@dingtalk.com'
 AUTHOR = 'dakada'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '1.8.4'
+VERSION = '1.9.0'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'jinja2'
 ]
 
 # What packages are optional?
@@ -102,17 +102,17 @@
     #   'Dakada'
     #   'User'
     #   'admin'
     #    'cookie'
     #   'render'
     #],
 
-    # entry_points={
-    #     'console_scripts': ['mycli=mymodule:cli'],
-    # },
+     entry_points={
+         'console_scripts': ['startproject=dakada:startproject'],
+     },
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license='MIT',
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
```

