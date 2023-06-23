# Comparing `tmp/ArseinRubika-4.8.6.tar.gz` & `tmp/ArseinRubika-4.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ArseinRubika-4.8.6.tar", last modified: Sun Feb 12 12:46:43 2023, max compression
+gzip compressed data, was "ArseinRubika-4.8.8.tar", last modified: Fri Jun 23 20:42:11 2023, max compression
```

## Comparing `ArseinRubika-4.8.6.tar` & `ArseinRubika-4.8.8.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 12:46:43.968693 ArseinRubika-4.8.6/
-drwxrwxrwx   0        0        0        0 2023-02-12 12:46:43.874963 ArseinRubika-4.8.6/ArseinRubika.egg-info/
--rw-rw-rw-   0        0        0     3308 2023-02-12 12:46:43.000000 ArseinRubika-4.8.6/ArseinRubika.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-02-12 12:46:43.000000 ArseinRubika-4.8.6/ArseinRubika.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 12:46:43.000000 ArseinRubika-4.8.6/ArseinRubika.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-02-12 12:46:43.000000 ArseinRubika-4.8.6/ArseinRubika.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-12 12:46:43.000000 ArseinRubika-4.8.6/ArseinRubika.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1096 2022-11-17 16:03:54.000000 ArseinRubika-4.8.6/LICENCE
--rw-rw-rw-   0        0        0     3308 2023-02-12 12:46:43.968693 ArseinRubika-4.8.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-12 12:46:43.953100 ArseinRubika-4.8.6/arsein/
--rw-rw-rw-   0        0        0    54111 2023-02-12 11:47:40.000000 ArseinRubika-4.8.6/arsein/Arsein.py
--rw-rw-rw-   0        0        0      373 2023-02-12 11:47:26.000000 ArseinRubika-4.8.6/arsein/Clien.py
--rw-rw-rw-   0        0        0      270 2023-02-12 12:43:45.000000 ArseinRubika-4.8.6/arsein/Copyright.py
--rw-rw-rw-   0        0        0      443 2023-02-12 11:47:06.000000 ArseinRubika-4.8.6/arsein/Device.py
--rw-rw-rw-   0        0        0     1953 2023-02-12 11:46:56.000000 ArseinRubika-4.8.6/arsein/Encoder.py
--rw-rw-rw-   0        0        0      155 2023-02-12 11:46:48.000000 ArseinRubika-4.8.6/arsein/Error.py
--rw-rw-rw-   0        0        0     8688 2023-02-12 11:46:39.000000 ArseinRubika-4.8.6/arsein/Getheader.py
--rw-rw-rw-   0        0        0      229 2023-02-12 11:46:30.000000 ArseinRubika-4.8.6/arsein/Gettime.py
--rw-rw-rw-   0        0        0     1120 2023-02-12 11:46:22.000000 ArseinRubika-4.8.6/arsein/GtM.py
--rw-rw-rw-   0        0        0     2485 2023-02-12 11:46:12.000000 ArseinRubika-4.8.6/arsein/PostData.py
--rw-rw-rw-   0        0        0      594 2023-02-12 11:46:05.000000 ArseinRubika-4.8.6/arsein/TypeText.py
--rw-rw-rw-   0        0        0    10100 2023-02-12 11:45:57.000000 ArseinRubika-4.8.6/arsein/Zedcontent.py
--rw-rw-rw-   0        0        0       27 2023-02-12 11:47:48.000000 ArseinRubika-4.8.6/arsein/__init__.py
--rw-rw-rw-   0        0        0       42 2023-02-12 12:46:43.968693 ArseinRubika-4.8.6/setup.cfg
--rw-rw-rw-   0        0        0     3667 2023-02-12 12:44:54.000000 ArseinRubika-4.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 20:42:11.780646 ArseinRubika-4.8.8/
+drwxrwxrwx   0        0        0        0 2023-06-23 20:42:11.749402 ArseinRubika-4.8.8/ArseinRubika.egg-info/
+-rw-rw-rw-   0        0        0     3308 2023-06-23 20:42:11.000000 ArseinRubika-4.8.8/ArseinRubika.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-06-23 20:42:11.000000 ArseinRubika-4.8.8/ArseinRubika.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 20:42:11.000000 ArseinRubika-4.8.8/ArseinRubika.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2023-06-23 20:42:11.000000 ArseinRubika-4.8.8/ArseinRubika.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-23 20:42:11.000000 ArseinRubika-4.8.8/ArseinRubika.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1096 2022-11-17 16:03:54.000000 ArseinRubika-4.8.8/LICENCE
+-rw-rw-rw-   0        0        0     3308 2023-06-23 20:42:11.780646 ArseinRubika-4.8.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-23 20:42:11.780646 ArseinRubika-4.8.8/arsein/
+-rw-rw-rw-   0        0        0    54285 2023-02-12 18:40:05.000000 ArseinRubika-4.8.8/arsein/Arsein.py
+-rw-rw-rw-   0        0        0      373 2023-02-12 11:47:26.000000 ArseinRubika-4.8.8/arsein/Clien.py
+-rw-rw-rw-   0        0        0      279 2023-06-23 20:36:36.000000 ArseinRubika-4.8.8/arsein/Copyright.py
+-rw-rw-rw-   0        0        0      443 2023-02-12 18:39:14.000000 ArseinRubika-4.8.8/arsein/Device.py
+-rw-rw-rw-   0        0        0     1953 2023-02-12 18:39:23.000000 ArseinRubika-4.8.8/arsein/Encoder.py
+-rw-rw-rw-   0        0        0      155 2023-02-12 11:46:48.000000 ArseinRubika-4.8.8/arsein/Error.py
+-rw-rw-rw-   0        0        0     8688 2023-02-12 11:46:39.000000 ArseinRubika-4.8.8/arsein/Getheader.py
+-rw-rw-rw-   0        0        0     1120 2023-02-12 18:39:32.000000 ArseinRubika-4.8.8/arsein/GtM.py
+-rw-rw-rw-   0        0        0     2485 2023-02-12 18:39:40.000000 ArseinRubika-4.8.8/arsein/PostData.py
+-rw-rw-rw-   0        0        0      594 2023-02-12 18:39:48.000000 ArseinRubika-4.8.8/arsein/TypeText.py
+-rw-rw-rw-   0        0        0    10100 2023-02-12 18:39:57.000000 ArseinRubika-4.8.8/arsein/Zedcontent.py
+-rw-rw-rw-   0        0        0       27 2023-02-12 11:47:48.000000 ArseinRubika-4.8.8/arsein/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-06-23 20:42:11.796267 ArseinRubika-4.8.8/setup.cfg
+-rw-rw-rw-   0        0        0     3651 2023-06-23 20:37:09.000000 ArseinRubika-4.8.8/setup.py
```

### Comparing `ArseinRubika-4.8.6/ArseinRubika.egg-info/PKG-INFO` & `ArseinRubika-4.8.8/ArseinRubika.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArseinRubika
-Version: 4.8.6
+Version: 4.8.8
 Summary:  library Robot Rubika
 Home-page: https://github.com/Arseinlibrary/Arsein__library.git
 Author: arian abasi nedamane
 Author-email: aryongram@gmail.com
 License: MIT
 Keywords: Arsein,Arseinrubika,ArseinRubika,arsein,bot,Bot,BOT,Robot,ROBOT,robot,self,api,API,Api,rubika,Rubika,RUBIKA,Python,python,aiohttp,asyncio
 Classifier: Development Status :: 3 - Alpha
@@ -55,15 +55,15 @@
 ``` bash
 from arsein.Zedcontent import Antiadvertisement
 ```
 
 ### How to install the library
 
 ``` bash
-pip install ArseinRubika==4.8.6
+pip install ArseinRubika==4.8.7
 ```
 
 ### My ID in Telegram
 
 ``` bash
 @Team_Arsein
 ```
```

### Comparing `ArseinRubika-4.8.6/LICENCE` & `ArseinRubika-4.8.8/LICENCE`

 * *Files identical despite different names*

### Comparing `ArseinRubika-4.8.6/PKG-INFO` & `ArseinRubika-4.8.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ArseinRubika
-Version: 4.8.6
+Version: 4.8.8
 Summary:  library Robot Rubika
 Home-page: https://github.com/Arseinlibrary/Arsein__library.git
 Author: arian abasi nedamane
 Author-email: aryongram@gmail.com
 License: MIT
 Keywords: Arsein,Arseinrubika,ArseinRubika,arsein,bot,Bot,BOT,Robot,ROBOT,robot,self,api,API,Api,rubika,Rubika,RUBIKA,Python,python,aiohttp,asyncio
 Classifier: Development Status :: 3 - Alpha
@@ -55,15 +55,15 @@
 ``` bash
 from arsein.Zedcontent import Antiadvertisement
 ```
 
 ### How to install the library
 
 ``` bash
-pip install ArseinRubika==4.8.6
+pip install ArseinRubika==4.8.7
 ```
 
 ### My ID in Telegram
 
 ``` bash
 @Team_Arsein
 ```
```

### Comparing `ArseinRubika-4.8.6/arsein/Arsein.py` & `ArseinRubika-4.8.8/arsein/Arsein.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from random import randint,choice
 import datetime
 import io, PIL.Image
 from arsein.Getheader import Upload
 from arsein.Encoder import encoderjson
 from tinytag import TinyTag
 from arsein.TypeText import TypeText
-from arsein.Gettime import Td
 import asyncio
 
 
 class Messenger:
     def __init__(self,Sh_account: str):
         self.Auth = str("".join(findall(r"\w",Sh_account)))
         self.prinet = copyright.CopyRight
@@ -504,56 +503,56 @@
         uresponse = self.Upload.uploadFile(file)
         file_id = str(uresponse[0]["id"])
         mime = file.split(".")[-1]
         dc_id = uresponse[0]["dc_id"]
         access_hash_rec = uresponse[1]
         file_name = file.split("/")[-1]
         loop = asyncio.get_event_loop()
-        time = Td(file) if time == None else time
+        time = round(TinyTag.get(file).duration * 1000) if time == None else time
         size = str(len(loop.run_until_complete(_download_with_server(server = file)) if ("http" or "https") in file else open(file,"rb").read()))
         return self.methods.methodsRubika("json",methode ="sendMessage",indata = {"file_inline": {"dc_id": dc_id,"file_id": file_id,"type":"Voice","file_name": file_name,"size": size,"time":time,"mime":mime,"access_hash_rec": access_hash_rec},"object_guid":guid,"rnd":f"{randint(100000,999999999)}","reply_to_message_id":message_id},wn = clien.android)
 
     def sendMusic(self, guid, file, time = None, caption=None, message_id=None):
         uresponse = self.Upload.uploadFile(file)
         file_id = str(uresponse[0]["id"])
         mime = file.split(".")[-1]
         dc_id = uresponse[0]["dc_id"]
         access_hash_rec = uresponse[1]
         file_name = file.split("/")[-1]
         loop = asyncio.get_event_loop()
-        time = Td(file) if time == None else time
+        time = round(TinyTag.get(file).duration * 1000) if time == None else time
         arti = "Arsein" if str(TinyTag.get(file).artist) == None else str(TinyTag.get(file).artist)
         size = str(len(loop.run_until_complete(_download_with_server(server = file)) if ("http" or "https") in file else open(file,"rb").read()))
         return self.methods.methodsRubika("json",methode ="sendMessage",indata = {"file_inline":{"access_hash_rec":access_hash_rec, "auto_play":False, "dc_id":dc_id, "file_id": file_id,"file_name":file_name,"height":0.0,"mime":mime,"music_performer": arti,"size": size,"time": time,"type":"Music","width":0.0},"is_mute":False,"object_guid":guid,"rnd":str(randint(100000,999999999)), "reply_to_message_id":message_id},wn = clien.web)
 
-    def sendGif(self, guid, file, Type= None, breadth:list= None, caption=None, message_id=None, thumbnail=None):
+    def sendGif(self, guid, file, time = None, Type= None, breadth:list= None, caption=None, message_id=None, thumbnail=None):
         uresponse = self.Upload.uploadFile(file)
         file_id = str(uresponse[0]["id"])
         mime = file.split(".")[-1]
         dc_id = uresponse[0]["dc_id"]
         access_hash_rec = uresponse[1]
         file_name = file.split("/")[-1]
         loop = asyncio.get_event_loop()
         if breadth == None: breadth =  [640,640] if not ("http" or "https") in file else [640,640]
-        time =  Td(file)
+        time = round(TinyTag.get(file).duration * 1000) if time == None else time
         size = str(len(loop.run_until_complete(_download_with_server(server = file)) if ("http" or "https") in file else open(file,"rb").read()))
         if thumbnail == None: thumbnail = r"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"
         return self.methods.methodsRubika("json",methode ="sendMessage",indata = {"file_inline":{"access_hash_rec":access_hash_rec,"auto_play":False,"dc_id":dc_id,"file_id":file_id,"file_name":file_name,"height":breadth[0],"mime":mime,"size":size,"thumb_inline":thumbnail,"time":time,"type":"Gif","width":breadth[1]},"is_mute":False,"object_guid":guid,"rnd":str(randint(100000,999999999)), "reply_to_message_id":message_id},wn = clien.android)
 
-    def sendVideo(self, guid, file,breadth:list = None, caption=None, message_id=None, thumbnail=None):
+    def sendVideo(self, guid, file, time = None,breadth:list = None, caption=None, message_id=None, thumbnail=None):
         uresponse = self.Upload.uploadFile(file)
         file_id = str(uresponse[0]["id"])
         mime = file.split(".")[-1]
         dc_id = uresponse[0]["dc_id"]
         access_hash_rec = uresponse[1]
         file_name = file.split("/")[-1]
         loop = asyncio.get_event_loop()
         if breadth == None: breadth =  [360,360]
         size = str(len(loop.run_until_complete(_download_with_server(server = file)) if ("http" or "https") in file else open(file,"rb").read()))
-        time = Td(file)
+        time = round(TinyTag.get(file).duration * 1000) if time == None else time
         if thumbnail == None: thumbnail = r"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"
         return self.methods.methodsRubika("json",methode ="sendMessage",indata = {"file_inline":{"access_hash_rec":access_hash_rec,"auto_play":False,"dc_id":dc_id,"file_id":file_id,"file_name":file_name,"height":breadth[0],"mime":mime,"size":size,"thumb_inline":thumbnail,"time":time,"type":"Video","width":breadth[1]},"is_mute":False,"object_guid":guid,"rnd":str(randint(100000,999999999)), "reply_to_message_id":message_id},wn = clien.android)
 
     def sendPhoto(self, guid, file, breadth:list= None, thumbnail=None, caption=None, message_id=None):
         uresponse = self.Upload.uploadFile(file)
         file_id = str(uresponse[0]["id"])
         mime = file.split(".")[-1]
```

### Comparing `ArseinRubika-4.8.6/arsein/Encoder.py` & `ArseinRubika-4.8.8/arsein/Encoder.py`

 * *Files identical despite different names*

### Comparing `ArseinRubika-4.8.6/arsein/Getheader.py` & `ArseinRubika-4.8.8/arsein/Getheader.py`

 * *Files identical despite different names*

### Comparing `ArseinRubika-4.8.6/arsein/GtM.py` & `ArseinRubika-4.8.8/arsein/GtM.py`

 * *Files identical despite different names*

### Comparing `ArseinRubika-4.8.6/arsein/PostData.py` & `ArseinRubika-4.8.8/arsein/PostData.py`

 * *Files identical despite different names*

### Comparing `ArseinRubika-4.8.6/arsein/TypeText.py` & `ArseinRubika-4.8.8/arsein/TypeText.py`

 * *Files identical despite different names*

### Comparing `ArseinRubika-4.8.6/arsein/Zedcontent.py` & `ArseinRubika-4.8.8/arsein/Zedcontent.py`

 * *Files identical despite different names*

### Comparing `ArseinRubika-4.8.6/setup.py` & `ArseinRubika-4.8.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import re
 from setuptools import setup,find_packages
 
 
-requires = ["pycryptodome==3.16.0","aiohttp==3.8.3","asyncio==3.4.3","tinytag==1.8.1","Pillow==9.4.0","opencv-python"]
+requires = ["pycryptodome==3.16.0","aiohttp==3.8.3","asyncio==3.4.3","tinytag==1.8.1","Pillow==9.4.0"]
 _long_description = """
 
 ## ArseinRubika
 
 > Elegant, modern and asynchronous Rubika MTProto API framework in Python for users and bots
 
 <p align="center">
@@ -35,15 +35,15 @@
 ``` bash
 from arsein.Zedcontent import Antiadvertisement
 ```
 
 ### How to install the library
 
 ``` bash
-pip install ArseinRubika==4.8.6
+pip install ArseinRubika==4.8.7
 ```
 
 ### My ID in Telegram
 
 ``` bash
 @Team_Arsein
 ```
@@ -108,15 +108,15 @@
 
 https://t.me/ArseinTeam
 ```
 """
 
 setup(
     name = "ArseinRubika",
-    version = "4.8.6",
+    version = "4.8.8",
     author = "arian abasi nedamane",
     author_email = "aryongram@gmail.com",
     description = (" library Robot Rubika"),
     license = "MIT",
     keywords = ["Arsein","Arseinrubika","ArseinRubika","arsein","bot","Bot","BOT","Robot","ROBOT","robot","self","api","API","Api","rubika","Rubika","RUBIKA","Python","python","aiohttp","asyncio"],
     url = "https://github.com/Arseinlibrary/Arsein__library.git",
     packages = ['arsein'],
```

