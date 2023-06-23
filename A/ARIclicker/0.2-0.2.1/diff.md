# Comparing `tmp/ARIclicker-0.2.tar.gz` & `tmp/ARIclicker-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ARIclicker-0.2.tar", last modified: Fri Jun 23 07:42:26 2023, max compression
+gzip compressed data, was "ARIclicker-0.2.1.tar", last modified: Fri Jun 23 08:16:20 2023, max compression
```

## Comparing `ARIclicker-0.2.tar` & `ARIclicker-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 07:42:26.551392 ARIclicker-0.2/
-drwxrwxrwx   0        0        0        0 2023-06-23 07:42:26.488883 ARIclicker-0.2/ARIclicker/
--rw-rw-rw-   0        0        0     3528 2023-06-23 07:39:43.000000 ARIclicker-0.2/ARIclicker/__init__.py
--rw-rw-rw-   0        0        0     1530 2023-06-22 07:29:28.000000 ARIclicker-0.2/ARIclicker/a.py
--rw-rw-rw-   0        0        0      422 2023-06-23 05:42:18.000000 ARIclicker-0.2/ARIclicker/aa.py
--rw-rw-rw-   0        0        0        2 2023-05-03 11:07:38.000000 ARIclicker-0.2/ARIclicker/file.py
-drwxrwxrwx   0        0        0        0 2023-06-23 07:42:26.520126 ARIclicker-0.2/ARIclicker.egg-info/
--rw-rw-rw-   0        0        0     1599 2023-06-23 07:42:26.000000 ARIclicker-0.2/ARIclicker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2023-06-23 07:42:26.000000 ARIclicker-0.2/ARIclicker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 07:42:26.000000 ARIclicker-0.2/ARIclicker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-23 07:42:26.000000 ARIclicker-0.2/ARIclicker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-23 07:42:26.000000 ARIclicker-0.2/ARIclicker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1599 2023-06-23 07:42:26.551392 ARIclicker-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1245 2023-06-22 04:08:21.000000 ARIclicker-0.2/README.md
--rw-rw-rw-   0        0        0     1093 2023-06-22 03:55:50.000000 ARIclicker-0.2/license.txt
--rw-rw-rw-   0        0        0       42 2023-06-23 07:42:26.551392 ARIclicker-0.2/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-06-23 07:42:04.000000 ARIclicker-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:16:20.904883 ARIclicker-0.2.1/
+drwxrwxrwx   0        0        0        0 2023-06-23 08:16:20.820904 ARIclicker-0.2.1/ARIclicker/
+-rw-rw-rw-   0        0        0     3813 2023-06-23 08:10:54.000000 ARIclicker-0.2.1/ARIclicker/__init__.py
+-rw-rw-rw-   0        0        0     1530 2023-06-22 07:29:28.000000 ARIclicker-0.2.1/ARIclicker/a.py
+-rw-rw-rw-   0        0        0      422 2023-06-23 05:42:18.000000 ARIclicker-0.2.1/ARIclicker/aa.py
+-rw-rw-rw-   0        0        0        2 2023-05-03 11:07:38.000000 ARIclicker-0.2.1/ARIclicker/file.py
+drwxrwxrwx   0        0        0        0 2023-06-23 08:16:20.873874 ARIclicker-0.2.1/ARIclicker.egg-info/
+-rw-rw-rw-   0        0        0     1601 2023-06-23 08:16:20.000000 ARIclicker-0.2.1/ARIclicker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-06-23 08:16:20.000000 ARIclicker-0.2.1/ARIclicker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 08:16:20.000000 ARIclicker-0.2.1/ARIclicker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-23 08:16:20.000000 ARIclicker-0.2.1/ARIclicker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-23 08:16:20.000000 ARIclicker-0.2.1/ARIclicker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1601 2023-06-23 08:16:20.902884 ARIclicker-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2023-06-22 04:08:21.000000 ARIclicker-0.2.1/README.md
+-rw-rw-rw-   0        0        0     1093 2023-06-22 03:55:50.000000 ARIclicker-0.2.1/license.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 08:16:20.905887 ARIclicker-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      696 2023-06-23 08:16:07.000000 ARIclicker-0.2.1/setup.py
```

### Comparing `ARIclicker-0.2/ARIclicker/__init__.py` & `ARIclicker-0.2.1/ARIclicker/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,21 +98,29 @@
                 press_thread.start_pressing()
         elif key == stop_key:
             press_thread.exit()
             listener.stop()
     with Listener(on_press=on_press) as listener:
         listener.join()
 
-def quickclick(key_start,key_stop):
+def quickclick(key_start,key_stop,program_stop_key=None):
   
     def func(key_start,key_stop):
        while True:
             keyboard.wait(key_start)
             time.sleep(0.1)
             while True:
                 pyautogui.click()
                 if keyboard.is_pressed(key_stop):
                     time.sleep(0.1)
                     break
-    t1=threading.Thread(target=func,args=(key_start,key_stop))
-    t1.start()
-
+    def detect(key):
+        while True:
+            if keyboard.is_pressed(key):
+                exit(0)       
+    t1=threading.Thread(target=func,args=(key_start,key_stop)).start()
+    if program_stop_key!=None:
+        t2 =threading.Thread(target=detect,args=(program_stop_key)).start()
+        
+    
+    
+quickclick("w","e","a")
```

### Comparing `ARIclicker-0.2/ARIclicker/a.py` & `ARIclicker-0.2.1/ARIclicker/a.py`

 * *Files identical despite different names*

### Comparing `ARIclicker-0.2/ARIclicker.egg-info/PKG-INFO` & `ARIclicker-0.2.1/ARIclicker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 0.2
+Version: 0.2.1
 Summary: AutoRandomIntervalClicker
 Home-page: UNKNOWN
 Author: lin_zhe
 Author-email: 2081812728@qq.com
 Maintainer: lin_zhe
 License: MIT License
 Keywords: AutoRandomIntervalClicker
```

### Comparing `ARIclicker-0.2/PKG-INFO` & `ARIclicker-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 0.2
+Version: 0.2.1
 Summary: AutoRandomIntervalClicker
 Home-page: UNKNOWN
 Author: lin_zhe
 Author-email: 2081812728@qq.com
 Maintainer: lin_zhe
 License: MIT License
 Keywords: AutoRandomIntervalClicker
```

### Comparing `ARIclicker-0.2/README.md` & `ARIclicker-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ARIclicker-0.2/license.txt` & `ARIclicker-0.2.1/license.txt`

 * *Files identical despite different names*

### Comparing `ARIclicker-0.2/setup.py` & `ARIclicker-0.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setup(
     name = 'ARIclicker',
-    version = '0.2',
+    version = '0.2.1',
     maintainer='lin_zhe',
     keywords='AutoRandomIntervalClicker',
     description = 'AutoRandomIntervalClicker',
     long_description_content_type='text/markdown',
     long_description=long_description,
     license = 'MIT License',
     author = 'lin_zhe',
```

