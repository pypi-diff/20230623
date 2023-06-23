# Comparing `tmp/aiavatar-0.2.0-py3-none-any.whl.zip` & `tmp/aiavatar-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 20365 bytes, number of entries: 20
+Zip file size: 20380 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      351 b- defN 23-May-27 12:45 aiavatar/__init__.py
 -rw-r--r--  2.0 unx     3407 b- defN 23-Jun-04 12:15 aiavatar/avatar.py
 -rw-r--r--  2.0 unx     5672 b- defN 23-Jun-23 10:05 aiavatar/bot.py
 -rw-r--r--  2.0 unx      284 b- defN 23-May-27 03:16 aiavatar/animation/__init__.py
 -rw-r--r--  2.0 unx       31 b- defN 23-May-27 03:48 aiavatar/device/__init__.py
 -rw-r--r--  2.0 unx     2344 b- defN 23-Jun-22 03:33 aiavatar/device/audio.py
 -rw-r--r--  2.0 unx     1650 b- defN 23-Jun-04 16:30 aiavatar/face/__init__.py
 -rw-r--r--  2.0 unx     1556 b- defN 23-Jun-04 16:30 aiavatar/face/vrchat.py
--rw-r--r--  2.0 unx     6081 b- defN 23-Jun-23 10:01 aiavatar/listeners/__init__.py
+-rw-r--r--  2.0 unx     6118 b- defN 23-Jun-23 14:29 aiavatar/listeners/__init__.py
 -rw-r--r--  2.0 unx      815 b- defN 23-Jun-23 10:01 aiavatar/listeners/voicerequest.py
--rw-r--r--  2.0 unx     1034 b- defN 23-Jun-23 10:01 aiavatar/listeners/wakeword.py
+-rw-r--r--  2.0 unx     1034 b- defN 23-Jun-23 14:19 aiavatar/listeners/wakeword.py
 -rw-r--r--  2.0 unx      178 b- defN 23-May-27 08:55 aiavatar/processors/__init__.py
 -rw-r--r--  2.0 unx     5177 b- defN 23-Jun-23 10:05 aiavatar/processors/chatgpt.py
 -rw-r--r--  2.0 unx      275 b- defN 23-May-27 08:54 aiavatar/speech/__init__.py
--rw-r--r--  2.0 unx     2281 b- defN 23-Jun-22 03:33 aiavatar/speech/voicevox.py
--rw-r--r--  2.0 unx    11324 b- defN 23-Jun-23 10:06 aiavatar-0.2.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     8953 b- defN 23-Jun-23 10:06 aiavatar-0.2.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 10:06 aiavatar-0.2.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-23 10:06 aiavatar-0.2.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1630 b- defN 23-Jun-23 10:06 aiavatar-0.2.0.dist-info/RECORD
-20 files, 53144 bytes uncompressed, 17713 bytes compressed:  66.7%
+-rw-r--r--  2.0 unx     2307 b- defN 23-Jun-23 14:29 aiavatar/speech/voicevox.py
+-rw-r--r--  2.0 unx    11324 b- defN 23-Jun-23 14:30 aiavatar-0.2.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     8953 b- defN 23-Jun-23 14:30 aiavatar-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 14:30 aiavatar-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-23 14:30 aiavatar-0.2.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1630 b- defN 23-Jun-23 14:30 aiavatar-0.2.1.dist-info/RECORD
+20 files, 53207 bytes uncompressed, 17728 bytes compressed:  66.7%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: aiavatar/speech/__init__.py
 Comment: 
 
 Filename: aiavatar/speech/voicevox.py
 Comment: 
 
-Filename: aiavatar-0.2.0.dist-info/LICENSE
+Filename: aiavatar-0.2.1.dist-info/LICENSE
 Comment: 
 
-Filename: aiavatar-0.2.0.dist-info/METADATA
+Filename: aiavatar-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: aiavatar-0.2.0.dist-info/WHEEL
+Filename: aiavatar-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: aiavatar-0.2.0.dist-info/top_level.txt
+Filename: aiavatar-0.2.1.dist-info/top_level.txt
 Comment: 
 
-Filename: aiavatar-0.2.0.dist-info/RECORD
+Filename: aiavatar-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiavatar/listeners/__init__.py

```diff
@@ -29,14 +29,15 @@
         audio_data = []
 
         def callback(in_data, frame_count, time_info, status):
             audio_data.append(in_data.copy())
 
         try:
             stream = sounddevice.InputStream(
+                device=device_index,
                 channels=self.channels,
                 samplerate=self.rate,
                 dtype=numpy.int16,
                 callback=callback
             )
 
             start_time = time.time()
```

## aiavatar/speech/voicevox.py

```diff
@@ -53,15 +53,15 @@
         with wave.open(io.BytesIO(voice.audio_clip), "rb") as f:
             try:
                 self._is_speaking = True
                 data = numpy.frombuffer(
                     f.readframes(f.getnframes()),
                     dtype=numpy.int16
                 )
-                sounddevice.play(data, f.getframerate())
+                sounddevice.play(data, f.getframerate(), device=self.device_index)
                 sounddevice.wait()
 
             except Exception as ex:
                 self.logger.error(f"Error at speaking: {str(ex)}\n{traceback.format_exc()}")
 
             finally:
                 self._is_speaking = False
```

## Comparing `aiavatar-0.2.0.dist-info/LICENSE` & `aiavatar-0.2.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aiavatar-0.2.0.dist-info/METADATA` & `aiavatar-0.2.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiavatar
-Version: 0.2.0
+Version: 0.2.1
 Summary: 🥰 Building AI-based conversational avatars lightning fast ⚡️💬
 Home-page: https://github.com/uezo/aiavatar
 Author: uezo
 Author-email: uezo@uezo.net
 Maintainer: uezo
 Maintainer-email: uezo@uezo.net
 License: Apache v2
```

## Comparing `aiavatar-0.2.0.dist-info/RECORD` & `aiavatar-0.2.1.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 aiavatar/avatar.py,sha256=ML4A_-cFggDOT4Sxb7VQMHvHD_rATxhY3Pt85ZppEKg,3407
 aiavatar/bot.py,sha256=HY_2mf3idOZy67msIgnJnGDXJGLnGuDhaOBeA-Jd-W8,5672
 aiavatar/animation/__init__.py,sha256=cE0zS3FgTUd0c6LcsLUnDVSTlFrCF0ZiH7-4NJxiQnU,284
 aiavatar/device/__init__.py,sha256=4DhskQxS20PcErkyF3z5-RuvXtGCQvw37jqB-yc2As8,31
 aiavatar/device/audio.py,sha256=xxRzbjyabXGrhY3WDc3UYEadjCU-xS7HF_vcXtGiC88,2344
 aiavatar/face/__init__.py,sha256=FPaP8RT8UXQ_UMON7RLvg2FUotOzTFVJ1qxzVk5zBTw,1650
 aiavatar/face/vrchat.py,sha256=VOibFm5Yuof-RQGfd1Zt1tx4v-TV9Usb8aMn7rHp5HY,1556
-aiavatar/listeners/__init__.py,sha256=VGsz2XkifoMIwTqDEcfK3HB8S593CpZUPnRwpN5PoNc,6081
+aiavatar/listeners/__init__.py,sha256=eVaNt7tO3aLuOrAZ7ij8dVq6IEmiiIy8XVVsc0AtIGc,6118
 aiavatar/listeners/voicerequest.py,sha256=kJM0tBTa-3PHbnSJVaSSYWJ2z4qDVkPEw0WrKQY0SpY,815
 aiavatar/listeners/wakeword.py,sha256=IX2_iNtUkjm8oSbRds6scrBYSoaywNZRhzq8GANoaIE,1034
 aiavatar/processors/__init__.py,sha256=k6qF1_UopWpaxQ89OxP7-dSVLgnrDCuuZH0Gom0JLLU,178
 aiavatar/processors/chatgpt.py,sha256=gGxHcCgjewyqcTd4IZy0A-Jdzm1B9chY3rGU1Jmhh6w,5177
 aiavatar/speech/__init__.py,sha256=yiveD86ikoWYYVnpdi1r_6ou5bXr-SOkmnri6ry_qHI,275
-aiavatar/speech/voicevox.py,sha256=8taNU-ziWhL_fR5b_caP5IiOkwzPlLvfRALRj6WbPCQ,2281
-aiavatar-0.2.0.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
-aiavatar-0.2.0.dist-info/METADATA,sha256=qbs_cuhGzlDgdsqzklgnVUaZFIa_HVHA2_A01W_PyOQ,8953
-aiavatar-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-aiavatar-0.2.0.dist-info/top_level.txt,sha256=B14WVaakM_kKuOkCeI-WRP83BJ6APkOyQrn6EXxs8kg,9
-aiavatar-0.2.0.dist-info/RECORD,,
+aiavatar/speech/voicevox.py,sha256=52PyVh0zBMTI2QM9ezjaw-PRkSJzkJ7G0xzZBg7wddU,2307
+aiavatar-0.2.1.dist-info/LICENSE,sha256=UOZ1F5fFDe3XXvG4oNnkL1-Ecun7zpHzRxjp-XsMeAo,11324
+aiavatar-0.2.1.dist-info/METADATA,sha256=6nOQwNRjup8FL3UDXHl92jM12ByWhpwX_1pa25F2NB0,8953
+aiavatar-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+aiavatar-0.2.1.dist-info/top_level.txt,sha256=B14WVaakM_kKuOkCeI-WRP83BJ6APkOyQrn6EXxs8kg,9
+aiavatar-0.2.1.dist-info/RECORD,,
```

