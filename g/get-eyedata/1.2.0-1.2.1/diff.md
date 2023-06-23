# Comparing `tmp/get_eyedata-1.2.0-py3-none-any.whl.zip` & `tmp/get_eyedata-1.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,11 @@
-Zip file size: 7559 bytes, number of entries: 12
+Zip file size: 5500 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-05 08:24 get_eyedata/__init__.py
 -rw-rw-rw-  2.0 fat     1581 b- defN 23-Jun-05 08:24 get_eyedata/frame_utils.py
--rw-rw-rw-  2.0 fat     1592 b- defN 23-May-13 00:34 get_eyedata/game_info.py
--rw-rw-rw-  2.0 fat     1546 b- defN 23-Jun-04 01:13 get_eyedata/make_eyedataset.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-05 08:24 get_eyedata/ow2.py
--rw-rw-rw-  2.0 fat      761 b- defN 23-Jun-04 07:06 get_eyedata/save.py
--rw-rw-rw-  2.0 fat     3359 b- defN 23-Jun-17 13:46 get_eyedata/valo.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-17 13:54 get_eyedata-1.2.0.dist-info/LICENCE
--rw-rw-rw-  2.0 fat     1816 b- defN 23-Jun-17 13:54 get_eyedata-1.2.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-17 13:54 get_eyedata-1.2.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-17 13:54 get_eyedata-1.2.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      957 b- defN 23-Jun-17 13:54 get_eyedata-1.2.0.dist-info/RECORD
-12 files, 12813 bytes uncompressed, 5949 bytes compressed:  53.6%
+-rw-rw-rw-  2.0 fat     3757 b- defN 23-Jun-23 06:17 get_eyedata/valo.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-23 06:23 get_eyedata-1.2.1.dist-info/LICENCE
+-rw-rw-rw-  2.0 fat     1816 b- defN 23-Jun-23 06:23 get_eyedata-1.2.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-23 06:23 get_eyedata-1.2.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-23 06:23 get_eyedata-1.2.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      714 b- defN 23-Jun-23 06:23 get_eyedata-1.2.1.dist-info/RECORD
+9 files, 9069 bytes uncompressed, 4264 bytes compressed:  53.0%
```

## zipnote {}

```diff
@@ -1,37 +1,28 @@
 Filename: get_eyedata/__init__.py
 Comment: 
 
 Filename: get_eyedata/frame_utils.py
 Comment: 
 
-Filename: get_eyedata/game_info.py
-Comment: 
-
-Filename: get_eyedata/make_eyedataset.py
-Comment: 
-
 Filename: get_eyedata/ow2.py
 Comment: 
 
-Filename: get_eyedata/save.py
-Comment: 
-
 Filename: get_eyedata/valo.py
 Comment: 
 
-Filename: get_eyedata-1.2.0.dist-info/LICENCE
+Filename: get_eyedata-1.2.1.dist-info/LICENCE
 Comment: 
 
-Filename: get_eyedata-1.2.0.dist-info/METADATA
+Filename: get_eyedata-1.2.1.dist-info/METADATA
 Comment: 
 
-Filename: get_eyedata-1.2.0.dist-info/WHEEL
+Filename: get_eyedata-1.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: get_eyedata-1.2.0.dist-info/top_level.txt
+Filename: get_eyedata-1.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: get_eyedata-1.2.0.dist-info/RECORD
+Filename: get_eyedata-1.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## get_eyedata/valo.py

```diff
@@ -5,28 +5,39 @@
 import numpy as np
 import pandas as pd
 from dataclasses import dataclass
 
 
 @dataclass
 class Area:
-    name:str
-    top_x:int
-    top_y:int
-    bottom_x:int
-    bottom_y:int
-
-minimap = Area('minimap',15,40,435,460)
-left_team = Area('left_team',440,0,870,100)
-right_team = Area('right_team',1050,0,1480,100)
-timer = Area('timer',870,0,1050,100)
-kill_log = Area('kill_log',1490,60,1920,300)
-hp = Area('hp',520,980,685,1080)
-skill = Area('skill',745,980,1175,1080)
-amo = Area('amo',1235,980,1400,1080)
+    name: str
+    top_x: int
+    top_y: int
+    bottom_x: int
+    bottom_y: int
+
+
+# minimap = Area('minimap',15,620,435,1040)
+# left_team = Area('left_team',440,0,870,100)
+# right_team = Area('right_team',1050,0,1480,100)
+# timer = Area('timer',870,0,1050,100)
+# kill_log = Area('kill_log',1490,60,1920,300)
+# hp = Area('hp',520,980,685,1080)
+# skill = Area('skill',745,980,1175,1080)
+# amo = Area('amo',1235,980,1400,1080)
+# center = ('center',960,540,125)
+
+minimap = Area('minimap',15,620,435,1040)
+left_team = Area('left_team',440,980,870,1080)
+right_team = Area('right_team',1050,980,1480,1080)
+timer = Area('timer',870,980,1050,1080)
+kill_log = Area('kill_log',1490,780,1920,1020)
+hp = Area('hp',520,0,685,100)
+skill = Area('skill',745,0,1175,100)
+amo = Area('amo',1235,0,1400,100)
 center = ('center',960,540,125)
 
 def get_roi(x, y):
     if ((x - center[1])**2 + (y - center[2])**2) <= center[3]**2:
         return center[0]
     elif left_team.top_x <= x <= left_team.bottom_x and left_team.top_y <= y <= left_team.bottom_y:
         return left_team.name
```

## Comparing `get_eyedata-1.2.0.dist-info/LICENCE` & `get_eyedata-1.2.1.dist-info/LICENCE`

 * *Files identical despite different names*

## Comparing `get_eyedata-1.2.0.dist-info/METADATA` & `get_eyedata-1.2.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-eyedata
-Version: 1.2.0
+Version: 1.2.1
 Summary: gat gaze data form record.
 Home-page: https://github.com/ikrfun/get_eyedata
 Download-URL: https://github.com/ikrfun/get_eyedata
 Author: ikrfun
 Author-email: t.nobuto130625@gmail.com
 Maintainer: ikrfun
 Maintainer-email: t.nobuto130625@gmail.com
```

## Comparing `get_eyedata-1.2.0.dist-info/RECORD` & `get_eyedata-1.2.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 get_eyedata/__init__.py,sha256=rqUtJyMLicobcyhmr74TepjmUQAEmlazKT3vjV_n3aA,6
 get_eyedata/frame_utils.py,sha256=UBuyN_aDdRql7TOv8E0Hjut5UqBlz41gYsG01aTmlFc,1581
-get_eyedata/game_info.py,sha256=rbVFZx8NRecjk5fZDRHvdJlVrtkLXFKX3zUcqzGj9V4,1592
-get_eyedata/make_eyedataset.py,sha256=n-WmhMsP3BfztSm5yj-_GT2PtEHgNrJHZ4Vk5T1jsrY,1546
 get_eyedata/ow2.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-get_eyedata/save.py,sha256=dc778CgOeF_nz1571ESZ9y8L-yxs2Y59M0Iwg_QK7Fg,761
-get_eyedata/valo.py,sha256=Vq-8QleNoMkrbqvLdUHyGMpRbqCpBn9niRValz1YV3g,3359
-get_eyedata-1.2.0.dist-info/LICENCE,sha256=44r0hK-BnpFZTBiPxTYe52HFlT034sEPBfHrJyaNI0g,1091
-get_eyedata-1.2.0.dist-info/METADATA,sha256=q647cJ-Z5EAd_AEtaaECd7v0ns00QmQKgUFRKQB6gy4,1816
-get_eyedata-1.2.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-get_eyedata-1.2.0.dist-info/top_level.txt,sha256=zlueM7ZefajCSIgOyib56hk_6HWx15EsED6S68g0mWE,12
-get_eyedata-1.2.0.dist-info/RECORD,,
+get_eyedata/valo.py,sha256=PqrMdKP8scFrlIFQN5qutlEaPgPJID7iT_lh5Z9PRZY,3757
+get_eyedata-1.2.1.dist-info/LICENCE,sha256=44r0hK-BnpFZTBiPxTYe52HFlT034sEPBfHrJyaNI0g,1091
+get_eyedata-1.2.1.dist-info/METADATA,sha256=6tCoBF9jVlA_aRzUwe0GogbdbWcuyW0-2BjxZO2BqKQ,1816
+get_eyedata-1.2.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+get_eyedata-1.2.1.dist-info/top_level.txt,sha256=zlueM7ZefajCSIgOyib56hk_6HWx15EsED6S68g0mWE,12
+get_eyedata-1.2.1.dist-info/RECORD,,
```

