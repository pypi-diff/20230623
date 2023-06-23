# Comparing `tmp/mc_game-1.0.1-py3-none-any.whl.zip` & `tmp/mc_game-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 7166506 bytes, number of entries: 14
+Zip file size: 7166651 bytes, number of entries: 14
 -rw-rw-rw-  2.0 fat       49 b- defN 23-Jun-21 12:15 mc_game/__init__.py
--rw-rw-rw-  2.0 fat      349 b- defN 23-Jun-21 12:16 mc_game-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-21 12:16 mc_game-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-21 12:16 mc_game-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      370 b- defN 23-Jun-21 12:16 mc_game-1.0.1.dist-info/RECORD
--rwxa--     3.1 fat  1800552 bx defN 23-Jun-21 18:43 MCLC.exe
--rw-a--     3.1 fat  2978816 bx defN 23-Jun-21 18:44 QtCore4.dll
--rw-a--     3.1 fat  9909760 bx defN 23-Jun-21 18:44 QtGui4.dll
--rwxa--     3.1 fat   102400 bx defN 23-Jun-21 18:43 unzip.exe
--rwxa--     3.1 fat   627432 bx defN 23-Jun-21 18:43 Upgrader.exe
--rw-a--     3.1 fat   117262 bx defN 23-Jun-21 18:43 libgcc_s_dw2-1.dll
--rw-a--     3.1 fat   970766 bx defN 23-Jun-21 18:43 libstdc++-6.dll
--rw-a--     3.1 fat    48640 bx defN 23-Jun-21 18:43 libwinpthread-1.dll
--rwxa--     3.1 fat   158440 bx defN 23-Jun-21 18:44 McLauncherCloud.exe
-14 files, 16714936 bytes uncompressed, 7164560 bytes compressed:  57.1%
+-rw-rw-rw-  2.0 fat      347 b- defN 23-Jun-23 12:06 mc_game-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-23 12:06 mc_game-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jun-23 12:06 mc_game-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      370 b- defN 23-Jun-23 12:06 mc_game-1.0.2.dist-info/RECORD
+-rw-a--     3.1 fat    48640 bx defN 23-Jun-21 18:43 mc_game/libwinpthread-1.dll
+-rwxa--     3.1 fat   158440 bx defN 23-Jun-21 18:44 mc_game/McLauncherCloud.exe
+-rwxa--     3.1 fat  1800552 bx defN 23-Jun-21 18:43 mc_game/MCLC.exe
+-rw-a--     3.1 fat  2978816 bx defN 23-Jun-21 18:44 mc_game/QtCore4.dll
+-rw-a--     3.1 fat  9909760 bx defN 23-Jun-21 18:44 mc_game/QtGui4.dll
+-rwxa--     3.1 fat   102400 bx defN 23-Jun-21 18:43 mc_game/unzip.exe
+-rwxa--     3.1 fat   627432 bx defN 23-Jun-21 18:43 mc_game/Upgrader.exe
+-rw-a--     3.1 fat   117262 bx defN 23-Jun-21 18:43 mc_game/libgcc_s_dw2-1.dll
+-rw-a--     3.1 fat   970766 bx defN 23-Jun-21 18:43 mc_game/libstdc++-6.dll
+14 files, 16714934 bytes uncompressed, 7164561 bytes compressed:  57.1%
```

## zipnote {}

```diff
@@ -1,43 +1,43 @@
 Filename: mc_game/__init__.py
 Comment: 
 
-Filename: mc_game-1.0.1.dist-info/METADATA
+Filename: mc_game-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: mc_game-1.0.1.dist-info/WHEEL
+Filename: mc_game-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: mc_game-1.0.1.dist-info/top_level.txt
+Filename: mc_game-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mc_game-1.0.1.dist-info/RECORD
+Filename: mc_game-1.0.2.dist-info/RECORD
 Comment: 
 
-Filename: MCLC.exe
+Filename: mc_game/libwinpthread-1.dll
 Comment: 
 
-Filename: QtCore4.dll
+Filename: mc_game/McLauncherCloud.exe
 Comment: 
 
-Filename: QtGui4.dll
+Filename: mc_game/MCLC.exe
 Comment: 
 
-Filename: unzip.exe
+Filename: mc_game/QtCore4.dll
 Comment: 
 
-Filename: Upgrader.exe
+Filename: mc_game/QtGui4.dll
 Comment: 
 
-Filename: libgcc_s_dw2-1.dll
+Filename: mc_game/unzip.exe
 Comment: 
 
-Filename: libstdc++-6.dll
+Filename: mc_game/Upgrader.exe
 Comment: 
 
-Filename: libwinpthread-1.dll
+Filename: mc_game/libgcc_s_dw2-1.dll
 Comment: 
 
-Filename: McLauncherCloud.exe
+Filename: mc_game/libstdc++-6.dll
 Comment: 
 
 Zip file comment:
```

## Comparing `MCLC.exe` & `mc_game/MCLC.exe`

 * *Files identical despite different names*

## Comparing `QtCore4.dll` & `mc_game/QtCore4.dll`

 * *Files identical despite different names*

## Comparing `QtGui4.dll` & `mc_game/QtGui4.dll`

 * *Files identical despite different names*

## Comparing `unzip.exe` & `mc_game/unzip.exe`

 * *Files identical despite different names*

## Comparing `Upgrader.exe` & `mc_game/Upgrader.exe`

 * *Files identical despite different names*

## Comparing `libgcc_s_dw2-1.dll` & `mc_game/libgcc_s_dw2-1.dll`

 * *Files identical despite different names*

## Comparing `libstdc++-6.dll` & `mc_game/libstdc++-6.dll`

 * *Files identical despite different names*

## Comparing `libwinpthread-1.dll` & `mc_game/libwinpthread-1.dll`

 * *Files identical despite different names*

## Comparing `McLauncherCloud.exe` & `mc_game/McLauncherCloud.exe`

 * *Files identical despite different names*

