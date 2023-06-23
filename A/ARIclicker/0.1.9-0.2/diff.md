# Comparing `tmp/ARIclicker-0.1.9.tar.gz` & `tmp/ARIclicker-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ARIclicker-0.1.9.tar", last modified: Thu Jun 22 07:33:51 2023, max compression
+gzip compressed data, was "ARIclicker-0.2.tar", last modified: Fri Jun 23 07:42:26 2023, max compression
```

## Comparing `ARIclicker-0.1.9.tar` & `ARIclicker-0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 07:33:51.473695 ARIclicker-0.1.9/
-drwxrwxrwx   0        0        0        0 2023-06-22 07:33:51.426823 ARIclicker-0.1.9/ARIclicker/
--rw-rw-rw-   0        0        0     3099 2023-06-22 07:32:37.000000 ARIclicker-0.1.9/ARIclicker/__init__.py
--rw-rw-rw-   0        0        0     1530 2023-06-22 07:29:28.000000 ARIclicker-0.1.9/ARIclicker/a.py
--rw-rw-rw-   0        0        0        2 2023-05-03 11:07:38.000000 ARIclicker-0.1.9/ARIclicker/file.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:33:51.458072 ARIclicker-0.1.9/ARIclicker.egg-info/
--rw-rw-rw-   0        0        0     1601 2023-06-22 07:33:51.000000 ARIclicker-0.1.9/ARIclicker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-06-22 07:33:51.000000 ARIclicker-0.1.9/ARIclicker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 07:33:51.000000 ARIclicker-0.1.9/ARIclicker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-22 07:33:51.000000 ARIclicker-0.1.9/ARIclicker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-22 07:33:51.000000 ARIclicker-0.1.9/ARIclicker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1601 2023-06-22 07:33:51.473695 ARIclicker-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     1245 2023-06-22 04:08:21.000000 ARIclicker-0.1.9/README.md
--rw-rw-rw-   0        0        0     1093 2023-06-22 03:55:50.000000 ARIclicker-0.1.9/license.txt
--rw-rw-rw-   0        0        0       42 2023-06-22 07:33:51.473695 ARIclicker-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      673 2023-06-22 07:33:45.000000 ARIclicker-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:42:26.551392 ARIclicker-0.2/
+drwxrwxrwx   0        0        0        0 2023-06-23 07:42:26.488883 ARIclicker-0.2/ARIclicker/
+-rw-rw-rw-   0        0        0     3528 2023-06-23 07:39:43.000000 ARIclicker-0.2/ARIclicker/__init__.py
+-rw-rw-rw-   0        0        0     1530 2023-06-22 07:29:28.000000 ARIclicker-0.2/ARIclicker/a.py
+-rw-rw-rw-   0        0        0      422 2023-06-23 05:42:18.000000 ARIclicker-0.2/ARIclicker/aa.py
+-rw-rw-rw-   0        0        0        2 2023-05-03 11:07:38.000000 ARIclicker-0.2/ARIclicker/file.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:42:26.520126 ARIclicker-0.2/ARIclicker.egg-info/
+-rw-rw-rw-   0        0        0     1599 2023-06-23 07:42:26.000000 ARIclicker-0.2/ARIclicker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-06-23 07:42:26.000000 ARIclicker-0.2/ARIclicker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 07:42:26.000000 ARIclicker-0.2/ARIclicker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-06-23 07:42:26.000000 ARIclicker-0.2/ARIclicker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-23 07:42:26.000000 ARIclicker-0.2/ARIclicker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1599 2023-06-23 07:42:26.551392 ARIclicker-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1245 2023-06-22 04:08:21.000000 ARIclicker-0.2/README.md
+-rw-rw-rw-   0        0        0     1093 2023-06-22 03:55:50.000000 ARIclicker-0.2/license.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 07:42:26.551392 ARIclicker-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      694 2023-06-23 07:42:04.000000 ARIclicker-0.2/setup.py
```

### Comparing `ARIclicker-0.1.9/ARIclicker/__init__.py` & `ARIclicker-0.2/ARIclicker/a.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,68 +2,14 @@
 import threading
 from pynput.mouse import Button, Controller
 from pynput.keyboard import Listener, KeyCode
 import pynput
 import random
 
 
-class ClickMouse(threading.Thread):
-    def __init__(self, delay_min, delay_max, button):
-        super(ClickMouse, self).__init__()
-        self.delay_min = delay_min
-        self.delay_max = delay_max
-        self.button = button
-        self.running = False
-        self.program_running = True
-
-    def start_clicking(self):
-        self.running = True
-
-    def stop_clicking(self):
-        self.running = False
-
-    def exit(self):
-        self.stop_clicking()
-        self.program_running = False
-
-    def run(self):
-        mouse=Controller()
-        while self.program_running:
-            while self.running:
-                mouse.click(self.button)
-                time.sleep(random.uniform(self.delay_min, self.delay_max))
-
-
-def autoclick(start_stop_key_character, end_key_character, delay_min, delay_max, button):
-    if button == "left":
-        button = Button.left
-    if button == "right":
-        button = Button.right
-    start_stop_key = KeyCode(char=start_stop_key_character)
-    stop_key = KeyCode(char=end_key_character)
-    mouse = pynput.mouse.Controller()
-    click_thread = ClickMouse(delay_min, delay_max, button)
-    click_thread.start()
-
-    def on_press(key):
-        if key == start_stop_key:
-            if click_thread.running:
-                click_thread.stop_clicking()
-            else:
-                click_thread.start_clicking()
-        elif key == stop_key:
-            click_thread.exit()
-            listener.stop()
-
-    with Listener(on_press=on_press) as listener:
-        listener.join()
-        start_listening_click = True
-
-
-
 def autopress(start_stop_key_character, end_key_character, button):
     class PressKey(threading.Thread):
         def __init__(self, button):
             super(PressKey, self).__init__()
             self.button = button
             self.running = False
             self.program_running = True
@@ -82,23 +28,26 @@
             key = pynput.keyboard.Controller()
             while self.program_running:
                 while self.running:
                     key.press(button)
 
     start_stop_key = KeyCode(char=start_stop_key_character)
     stop_key = KeyCode(char=end_key_character)
+    print(start_stop_key)
     press_thread = PressKey(button)
     press_thread.start()
 
     def on_press(key):
+        print(key)
         if key == start_stop_key:
             if press_thread.running:
                 press_thread.stop_pressing()
             else:
                 press_thread.start_pressing()
         elif key == stop_key:
             press_thread.exit()
             listener.stop()
+          
     with Listener(on_press=on_press) as listener:
         listener.join()
 
 autopress("q","w","e")
```

### Comparing `ARIclicker-0.1.9/ARIclicker.egg-info/PKG-INFO` & `ARIclicker-0.2/ARIclicker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 0.1.9
+Version: 0.2
 Summary: AutoRandomIntervalClicker
 Home-page: UNKNOWN
 Author: lin_zhe
 Author-email: 2081812728@qq.com
 Maintainer: lin_zhe
 License: MIT License
 Keywords: AutoRandomIntervalClicker
```

### Comparing `ARIclicker-0.1.9/PKG-INFO` & `ARIclicker-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ARIclicker
-Version: 0.1.9
+Version: 0.2
 Summary: AutoRandomIntervalClicker
 Home-page: UNKNOWN
 Author: lin_zhe
 Author-email: 2081812728@qq.com
 Maintainer: lin_zhe
 License: MIT License
 Keywords: AutoRandomIntervalClicker
```

### Comparing `ARIclicker-0.1.9/README.md` & `ARIclicker-0.2/README.md`

 * *Files identical despite different names*

### Comparing `ARIclicker-0.1.9/license.txt` & `ARIclicker-0.2/license.txt`

 * *Files identical despite different names*

