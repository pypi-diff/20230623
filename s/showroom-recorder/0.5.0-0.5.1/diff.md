# Comparing `tmp/showroom-recorder-0.5.0.tar.gz` & `tmp/showroom-recorder-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showroom-recorder-0.5.0.tar", last modified: Fri Jun 23 17:16:36 2023, max compression
+gzip compressed data, was "showroom-recorder-0.5.1.tar", last modified: Fri Jun 23 17:53:44 2023, max compression
```

## Comparing `showroom-recorder-0.5.0.tar` & `showroom-recorder-0.5.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:16:36.923225 showroom-recorder-0.5.0/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-21 05:55:33.000000 showroom-recorder-0.5.0/LICENSE
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-20 10:03:45.000000 showroom-recorder-0.5.0/MANIFEST.in
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-23 17:16:36.923225 showroom-recorder-0.5.0/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-20 09:47:38.000000 showroom-recorder-0.5.0/README.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-20 10:02:46.000000 showroom-recorder-0.5.0/description.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-23 17:16:36.927225 showroom-recorder-0.5.0/setup.cfg
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-20 09:59:51.000000 showroom-recorder-0.5.0/setup.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      525 2023-06-21 05:43:58.000000 showroom-recorder-0.5.0/showroom-recorder.json
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:16:36.915225 showroom-recorder-0.5.0/src/
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:16:36.923225 showroom-recorder-0.5.0/src/showroom_recorder/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/__main__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3430 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/common.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:16:36.923225 showroom-recorder-0.5.0/src/showroom_recorder/processor/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/processor/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/processor/danmaku.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     6029 2023-06-23 17:16:06.000000 showroom-recorder-0.5.0/src/showroom_recorder/processor/video.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:16:36.923225 showroom-recorder-0.5.0/src/showroom_recorder/utils/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/utils/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3532 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/utils/config.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/utils/delete_emoji.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       69 2023-06-23 17:16:19.000000 showroom-recorder-0.5.0/src/showroom_recorder/version.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:16:36.923225 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-23 17:16:36.000000 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      771 2023-06-23 17:16:36.000000 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/SOURCES.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-23 17:16:36.000000 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/dependency_links.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-23 17:16:36.000000 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/entry_points.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       51 2023-06-23 17:16:36.000000 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/requires.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-23 17:16:36.000000 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/top_level.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-20 09:30:11.000000 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/zip-safe
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:53:44.503310 showroom-recorder-0.5.1/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-21 05:55:33.000000 showroom-recorder-0.5.1/LICENSE
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-20 10:03:45.000000 showroom-recorder-0.5.1/MANIFEST.in
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-23 17:53:44.503310 showroom-recorder-0.5.1/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-20 09:47:38.000000 showroom-recorder-0.5.1/README.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-20 10:02:46.000000 showroom-recorder-0.5.1/description.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-23 17:53:44.503310 showroom-recorder-0.5.1/setup.cfg
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-20 09:59:51.000000 showroom-recorder-0.5.1/setup.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      525 2023-06-21 05:43:58.000000 showroom-recorder-0.5.1/showroom-recorder.json
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:53:44.499310 showroom-recorder-0.5.1/src/
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:53:44.499310 showroom-recorder-0.5.1/src/showroom_recorder/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/__main__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3430 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/common.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:53:44.503310 showroom-recorder-0.5.1/src/showroom_recorder/processor/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/processor/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/processor/danmaku.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     6020 2023-06-23 17:51:42.000000 showroom-recorder-0.5.1/src/showroom_recorder/processor/video.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:53:44.503310 showroom-recorder-0.5.1/src/showroom_recorder/utils/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/utils/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3532 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/utils/config.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-20 09:35:33.000000 showroom-recorder-0.5.1/src/showroom_recorder/utils/delete_emoji.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       46 2023-06-23 17:53:09.000000 showroom-recorder-0.5.1/src/showroom_recorder/version.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:53:44.503310 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-23 17:53:44.000000 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      771 2023-06-23 17:53:44.000000 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/SOURCES.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-23 17:53:44.000000 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/dependency_links.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-23 17:53:44.000000 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/entry_points.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       51 2023-06-23 17:53:44.000000 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/requires.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-23 17:53:44.000000 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/top_level.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-20 09:30:11.000000 showroom-recorder-0.5.1/src/showroom_recorder.egg-info/zip-safe
```

### Comparing `showroom-recorder-0.5.0/LICENSE` & `showroom-recorder-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.5.0/PKG-INFO` & `showroom-recorder-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.5.0
+Version: 0.5.1
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.5.0/README.md` & `showroom-recorder-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.5.0/description.md` & `showroom-recorder-0.5.1/description.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.5.0/setup.py` & `showroom-recorder-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.5.0/showroom-recorder.json` & `showroom-recorder-0.5.1/showroom-recorder.json`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.5.0/src/showroom_recorder/common.py` & `showroom-recorder-0.5.1/src/showroom_recorder/common.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.5.0/src/showroom_recorder/processor/danmaku.py` & `showroom-recorder-0.5.1/src/showroom_recorder/processor/danmaku.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.5.0/src/showroom_recorder/processor/video.py` & `showroom-recorder-0.5.1/src/showroom_recorder/processor/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,11 +181,11 @@
         self.isRecording = True
         logging.info('{room_url_key}: is on live, start recording video.'.format(
             room_url_key=self.room_url_key))
         try:
             if not os.path.isdir('videos'):
                 os.makedirs('videos')
             download(self.status, output_dir='videos')
-        except Exception as e:
+        except Exception:
             self.isRecording = False
             logging.error('{room_url_key}: record video finished.'.format(
-                room_url_key=self.room_url_key) + e)
+                room_url_key=self.room_url_key))
```

### Comparing `showroom-recorder-0.5.0/src/showroom_recorder/utils/config.py` & `showroom-recorder-0.5.1/src/showroom_recorder/utils/config.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.5.0/src/showroom_recorder/utils/delete_emoji.py` & `showroom-recorder-0.5.1/src/showroom_recorder/utils/delete_emoji.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.5.0/src/showroom_recorder.egg-info/PKG-INFO` & `showroom-recorder-0.5.1/src/showroom_recorder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.5.0
+Version: 0.5.1
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.5.0/src/showroom_recorder.egg-info/SOURCES.txt` & `showroom-recorder-0.5.1/src/showroom_recorder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

