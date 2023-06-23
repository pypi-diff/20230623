# Comparing `tmp/showroom-recorder-0.4.6.tar.gz` & `tmp/showroom-recorder-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "showroom-recorder-0.4.6.tar", last modified: Wed Jun 21 06:36:05 2023, max compression
+gzip compressed data, was "showroom-recorder-0.5.0.tar", last modified: Fri Jun 23 17:16:36 2023, max compression
```

## Comparing `showroom-recorder-0.4.6.tar` & `showroom-recorder-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-21 06:36:05.987484 showroom-recorder-0.4.6/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-21 05:55:33.000000 showroom-recorder-0.4.6/LICENSE
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-20 10:03:45.000000 showroom-recorder-0.4.6/MANIFEST.in
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-21 06:36:05.987484 showroom-recorder-0.4.6/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-20 09:47:38.000000 showroom-recorder-0.4.6/README.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-20 10:02:46.000000 showroom-recorder-0.4.6/description.md
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-21 06:36:05.987484 showroom-recorder-0.4.6/setup.cfg
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-20 09:59:51.000000 showroom-recorder-0.4.6/setup.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      525 2023-06-21 05:43:58.000000 showroom-recorder-0.4.6/showroom-recorder.json
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-21 06:36:05.971484 showroom-recorder-0.4.6/src/
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-21 06:36:05.987484 showroom-recorder-0.4.6/src/showroom_recorder/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-20 09:35:33.000000 showroom-recorder-0.4.6/src/showroom_recorder/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-20 09:35:33.000000 showroom-recorder-0.4.6/src/showroom_recorder/__main__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3430 2023-06-20 09:35:33.000000 showroom-recorder-0.4.6/src/showroom_recorder/common.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-21 06:36:05.987484 showroom-recorder-0.4.6/src/showroom_recorder/processor/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.4.6/src/showroom_recorder/processor/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-20 09:35:33.000000 showroom-recorder-0.4.6/src/showroom_recorder/processor/danmaku.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     6011 2023-06-21 05:47:57.000000 showroom-recorder-0.4.6/src/showroom_recorder/processor/video.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-21 06:36:05.987484 showroom-recorder-0.4.6/src/showroom_recorder/utils/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.4.6/src/showroom_recorder/utils/__init__.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3532 2023-06-20 09:35:33.000000 showroom-recorder-0.4.6/src/showroom_recorder/utils/config.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-20 09:35:33.000000 showroom-recorder-0.4.6/src/showroom_recorder/utils/delete_emoji.py
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       69 2023-06-21 04:34:53.000000 showroom-recorder-0.4.6/src/showroom_recorder/version.py
-drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-21 06:36:05.987484 showroom-recorder-0.4.6/src/showroom_recorder.egg-info/
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-21 06:36:05.000000 showroom-recorder-0.4.6/src/showroom_recorder.egg-info/PKG-INFO
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      771 2023-06-21 06:36:05.000000 showroom-recorder-0.4.6/src/showroom_recorder.egg-info/SOURCES.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-21 06:36:05.000000 showroom-recorder-0.4.6/src/showroom_recorder.egg-info/dependency_links.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-21 06:36:05.000000 showroom-recorder-0.4.6/src/showroom_recorder.egg-info/entry_points.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       51 2023-06-21 06:36:05.000000 showroom-recorder-0.4.6/src/showroom_recorder.egg-info/requires.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-21 06:36:05.000000 showroom-recorder-0.4.6/src/showroom_recorder.egg-info/top_level.txt
--rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-20 09:30:11.000000 showroom-recorder-0.4.6/src/showroom_recorder.egg-info/zip-safe
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:16:36.923225 showroom-recorder-0.5.0/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    35149 2023-06-21 05:55:33.000000 showroom-recorder-0.5.0/LICENSE
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       53 2023-06-20 10:03:45.000000 showroom-recorder-0.5.0/MANIFEST.in
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-23 17:16:36.923225 showroom-recorder-0.5.0/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1394 2023-06-20 09:47:38.000000 showroom-recorder-0.5.0/README.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      964 2023-06-20 10:02:46.000000 showroom-recorder-0.5.0/description.md
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       38 2023-06-23 17:16:36.927225 showroom-recorder-0.5.0/setup.cfg
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1175 2023-06-20 09:59:51.000000 showroom-recorder-0.5.0/setup.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      525 2023-06-21 05:43:58.000000 showroom-recorder-0.5.0/showroom-recorder.json
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:16:36.915225 showroom-recorder-0.5.0/src/
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:16:36.923225 showroom-recorder-0.5.0/src/showroom_recorder/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       48 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      185 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/__main__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3430 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/common.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:16:36.923225 showroom-recorder-0.5.0/src/showroom_recorder/processor/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/processor/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    31904 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/processor/danmaku.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     6029 2023-06-23 17:16:06.000000 showroom-recorder-0.5.0/src/showroom_recorder/processor/video.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:16:36.923225 showroom-recorder-0.5.0/src/showroom_recorder/utils/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        0 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/utils/__init__.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     3532 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/utils/config.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)    16581 2023-06-20 09:35:33.000000 showroom-recorder-0.5.0/src/showroom_recorder/utils/delete_emoji.py
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       69 2023-06-23 17:16:19.000000 showroom-recorder-0.5.0/src/showroom_recorder/version.py
+drwxrwxr-x   0 vacabun   (1000) vacabun   (1000)        0 2023-06-23 17:16:36.923225 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)     1307 2023-06-23 17:16:36.000000 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/PKG-INFO
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)      771 2023-06-23 17:16:36.000000 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/SOURCES.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-23 17:16:36.000000 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/dependency_links.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       71 2023-06-23 17:16:36.000000 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/entry_points.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       51 2023-06-23 17:16:36.000000 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/requires.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)       18 2023-06-23 17:16:36.000000 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/top_level.txt
+-rw-rw-r--   0 vacabun   (1000) vacabun   (1000)        1 2023-06-20 09:30:11.000000 showroom-recorder-0.5.0/src/showroom_recorder.egg-info/zip-safe
```

### Comparing `showroom-recorder-0.4.6/LICENSE` & `showroom-recorder-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.6/PKG-INFO` & `showroom-recorder-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.4.6
+Version: 0.5.0
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.4.6/README.md` & `showroom-recorder-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.6/description.md` & `showroom-recorder-0.5.0/description.md`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.6/setup.py` & `showroom-recorder-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.6/showroom-recorder.json` & `showroom-recorder-0.5.0/showroom-recorder.json`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.6/src/showroom_recorder/common.py` & `showroom-recorder-0.5.0/src/showroom_recorder/common.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.6/src/showroom_recorder/processor/danmaku.py` & `showroom-recorder-0.5.0/src/showroom_recorder/processor/danmaku.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.6/src/showroom_recorder/processor/video.py` & `showroom-recorder-0.5.0/src/showroom_recorder/processor/video.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,55 +2,95 @@
 import os
 import time
 import logging
 import threading
 import ffmpeg
 import json
 import requests
-import re
+import datetime
+import pytz
 
 fake_headers = {
     'Accept': 'text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8',
     'Accept-Charset': 'UTF-8,*;q=0.5',
     'Accept-Encoding': 'gzip,deflate,sdch',
     'Accept-Language': 'en-US,en;q=0.8',
     'User-Agent': 'Mozilla/5.0 (Linux; Android 4.4.2; Nexus 4 Build/KOT49H) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/34.0.1847.114 Mobile Safari/537.36'
     }
 
 
-def get_showroom_stream_url(room_url_key):
+def get_status_by_room_url_key(room_url_key):
+    url = "https://www.showroom-live.com/api/room/status"
+    params = {
+        "room_url_key": room_url_key,
+    }
+    response = requests.get(url=url, headers=fake_headers, params=params)
+    status = response.json()
+    return status
+
+
+def get_room_url_key_by_status(status):
+    return status['room_url_key']
+
+
+def get_roomid_by_status(status):
+    return status['room_id']
+
+
+def get_online_by_status(status):
+    return status['is_live']
+
+
+def get_room_name_by_status(status):
+    return status['room_name']
+
+
+def get_start_time_by_status(status):
+    t = status['started_at']
+    dt = datetime.datetime.utcfromtimestamp(t)
+    tz = pytz.timezone('Asia/Tokyo')
+    dt = dt.astimezone(tz)
+    return dt
+
+
+def get_time_now():
+    dt = datetime.datetime.now()
+    tz = pytz.timezone('Asia/Tokyo')
+    dt = dt.astimezone(tz)
+    return dt
+
+
+def get_stream_url_by_roomid(room_id):
     stream_url = ''
-    try:
-        room_id = showroom_get_roomid_by_room_url_key(room_url_key)
-    except Exception:
-        raise Exception('get room_id error.')
     api_endpoint = 'https://www.showroom-live.com/api/live/streaming_url?room_id={room_id}&_={timestamp}&abr_available=1'.format(
         room_id=room_id, timestamp=str(int(time.time() * 1000)))
     try:
         response = requests.get(url=api_endpoint, headers=fake_headers).text
         response = json.loads(response)
         stream_url = response['streaming_url_list'][0]['url']
         for streaming_url in response['streaming_url_list']:
             if streaming_url['type'] == 'hls_all':
                 stream_url = streaming_url['url']
-    except Exception:
-        raise Exception('The live show is currently offline.')
+    except Exception as e:
+        raise Exception('get stream url error: ' + e)
     return stream_url
 
 
-def showroom_download(room_url_key, output_dir='.'):
+def download(status, output_dir='.'):
     try:
-        stream_url = get_showroom_stream_url(room_url_key)
+        stream_url = get_stream_url_by_roomid(get_roomid_by_status(status))
     except Exception as e:
         raise Exception('get stream url error: ' + e)
-
-    title = '{room_url_key}_{time}'.format(
-        room_url_key=room_url_key,
-        time=time.strftime("%Y%m%d_%H%M%S", time.localtime()))
-    output = output_dir + '/' + title + '.' + 'mp4'
+    try:
+        title = '{name}_{time}'.format(
+            name=get_room_url_key_by_status(status),
+            time=get_time_now().strftime('%Y%m%d_%H%M%S'))
+        output = output_dir + '/' + title + '.' + 'mp4'
+    except Exception as e:
+        raise Exception('get title error: ' + e)
 
     kwargs_dict = {'c:v': 'copy',
                    'c:a': 'copy',
                    'bsf:a': 'aac_adtstoasc',
                    'loglevel': 'error'}
     try:
         proc = (
@@ -71,42 +111,14 @@
             proc.stdin.write('q'.encode('utf-8'))
         except Exception:
             pass
         raise Exception(e)
     return True
 
 
-def showroom_get_roomid_by_room_url_key(room_url_key):
-
-    webpage_url = 'https://www.showroom-live.com/' + room_url_key
-    try:
-        response = requests.get(url=webpage_url, headers=fake_headers).text
-        match = re.search(r'room\?room_id\=(\d+)', response)
-        if match:
-            room_id = match.group(1)
-            return room_id
-    except Exception:
-        raise Exception('get room_id error.')
-
-
-def get_online(room_url_key):
-    try:
-        room_id = showroom_get_roomid_by_room_url_key(room_url_key)
-    except Exception:
-        return False
-    api_endpoint = 'https://www.showroom-live.com/api/live/live_info?room_id={room_id}'.format(
-        room_id=room_id)
-    response = requests.get(url=api_endpoint, headers=fake_headers).text
-    response = json.loads(response)
-    if response['live_status'] == 2:
-        return True
-    else:
-        return False
-
-
 class RoomMonitor:
     def __init__(self, room_url_keys, settings):
         self.room_url_keys = room_url_keys
         self.t = None
         self.nRooms = 0
         self.cRecords = []
         self.settings = settings
@@ -122,58 +134,58 @@
         self.t.daemon = True
         self.t.start()
         return self.t
 
     def monitor(self):
         self.nRooms = len(self.room_url_keys)
         self.vRecords = [None] * self.nRooms
-
-        logging.debug('start record video.')
         while True:
             for i in range(self.nRooms):
                 if self.vRecords[i] is not None:
                     if self.vRecords[i].isRecording:
                         # logging.debug('already recording...')
                         continue
                     else:
                         self.vRecords[i] = None
                         logging.debug('{k}:delete recording...'
                                       .format(k=self.room_url_keys[i]))
                 if self.vRecords[i] is None:
                     room_url_key = self.room_url_keys[i]
                     try:
-                        if get_online(room_url_key):
-                            vr = VideoRecorder(room_url_key, self.settings)
+                        status = get_status_by_room_url_key(room_url_key)
+                        if get_online_by_status(status):
+                            vr = VideoRecorder(status, self.settings)
                             vr.start()
                             self.vRecords[i] = vr
                             continue
                     except Exception as e:
-                        logging.debug('{room_url_key}: {e}'.format(
+                        logging.error('{room_url_key}: {e}'.format(
                             room_url_key=room_url_key, e=e))
             time.sleep(1)
         # end while
 
 
 class VideoRecorder:
-    def __init__(self, room_url_key, settings):
-        self.room_url_key = room_url_key
+    def __init__(self, status, settings):
+        self.room_url_key = status['room_url_key']
         self.settings = settings
         self.isRecording = False
         self._thread_main = None
+        self.status = status
 
     def start(self):
         self._thread_main = threading.Thread(target=self.record)
         self._thread_main.daemon = True
         self._thread_main.start()
 
     def record(self):
         self.isRecording = True
         logging.info('{room_url_key}: is on live, start recording video.'.format(
             room_url_key=self.room_url_key))
         try:
             if not os.path.isdir('videos'):
                 os.makedirs('videos')
-            showroom_download(self.room_url_key, output_dir='videos')
-        except Exception:
+            download(self.status, output_dir='videos')
+        except Exception as e:
             self.isRecording = False
-            logging.info('{room_url_key}: record video finished.'.format(
-                room_url_key=self.room_url_key))
+            logging.error('{room_url_key}: record video finished.'.format(
+                room_url_key=self.room_url_key) + e)
```

### Comparing `showroom-recorder-0.4.6/src/showroom_recorder/utils/config.py` & `showroom-recorder-0.5.0/src/showroom_recorder/utils/config.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.6/src/showroom_recorder/utils/delete_emoji.py` & `showroom-recorder-0.5.0/src/showroom_recorder/utils/delete_emoji.py`

 * *Files identical despite different names*

### Comparing `showroom-recorder-0.4.6/src/showroom_recorder.egg-info/PKG-INFO` & `showroom-recorder-0.5.0/src/showroom_recorder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: showroom-recorder
-Version: 0.4.6
+Version: 0.5.0
 Summary: Recording Showroom Streaming Video
 Home-page: https://github.com/vacabun/showroom-recorder
 Author: vacabun
 Author-email: maguotong66@gmail.com
 License: UNKNOWN
 Keywords: video download showroom
 Platform: any
```

### Comparing `showroom-recorder-0.4.6/src/showroom_recorder.egg-info/SOURCES.txt` & `showroom-recorder-0.5.0/src/showroom_recorder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

