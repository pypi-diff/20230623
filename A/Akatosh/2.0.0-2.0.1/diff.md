# Comparing `tmp/Akatosh-2.0.0.tar.gz` & `tmp/Akatosh-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Akatosh-2.0.0.tar", last modified: Fri Jun 23 11:22:21 2023, max compression
+gzip compressed data, was "Akatosh-2.0.1.tar", last modified: Fri Jun 23 11:51:39 2023, max compression
```

## Comparing `Akatosh-2.0.0.tar` & `Akatosh-2.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 11:22:21.813570 Akatosh-2.0.0/
-drwxrwxrwx   0        0        0        0 2023-06-23 11:22:21.799563 Akatosh-2.0.0/Akatosh/
--rw-rw-rw-   0        0        0      120 2023-06-23 07:41:14.000000 Akatosh-2.0.0/Akatosh/__init__.py
--rw-rw-rw-   0        0        0     4324 2023-06-23 11:20:36.000000 Akatosh-2.0.0/Akatosh/event.py
--rw-rw-rw-   0        0        0      387 2023-06-23 07:55:30.000000 Akatosh-2.0.0/Akatosh/logger.py
--rw-rw-rw-   0        0        0     6178 2023-06-23 08:29:24.000000 Akatosh-2.0.0/Akatosh/resource.py
--rw-rw-rw-   0        0        0      172 2023-06-22 11:35:11.000000 Akatosh-2.0.0/Akatosh/states.py
--rw-rw-rw-   0        0        0     2362 2023-06-23 05:37:35.000000 Akatosh-2.0.0/Akatosh/universe.py
-drwxrwxrwx   0        0        0        0 2023-06-23 11:22:21.809568 Akatosh-2.0.0/Akatosh.egg-info/
--rw-rw-rw-   0        0        0     2011 2023-06-23 11:22:21.000000 Akatosh-2.0.0/Akatosh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-06-23 11:22:21.000000 Akatosh-2.0.0/Akatosh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 11:22:21.000000 Akatosh-2.0.0/Akatosh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-23 11:22:21.000000 Akatosh-2.0.0/Akatosh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2011 2023-06-23 11:22:21.811569 Akatosh-2.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1482 2023-06-21 04:34:02.000000 Akatosh-2.0.0/README.md
--rw-rw-rw-   0        0        0      669 2023-06-23 11:21:48.000000 Akatosh-2.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-23 11:22:21.813570 Akatosh-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 11:51:39.302010 Akatosh-2.0.1/
+drwxrwxrwx   0        0        0        0 2023-06-23 11:51:39.287499 Akatosh-2.0.1/Akatosh/
+-rw-rw-rw-   0        0        0      120 2023-06-23 07:41:14.000000 Akatosh-2.0.1/Akatosh/__init__.py
+-rw-rw-rw-   0        0        0     4324 2023-06-23 11:20:36.000000 Akatosh-2.0.1/Akatosh/event.py
+-rw-rw-rw-   0        0        0      387 2023-06-23 07:55:30.000000 Akatosh-2.0.1/Akatosh/logger.py
+-rw-rw-rw-   0        0        0     6178 2023-06-23 08:29:24.000000 Akatosh-2.0.1/Akatosh/resource.py
+-rw-rw-rw-   0        0        0      172 2023-06-22 11:35:11.000000 Akatosh-2.0.1/Akatosh/states.py
+-rw-rw-rw-   0        0        0     2816 2023-06-23 11:50:47.000000 Akatosh-2.0.1/Akatosh/universe.py
+drwxrwxrwx   0        0        0        0 2023-06-23 11:51:39.298010 Akatosh-2.0.1/Akatosh.egg-info/
+-rw-rw-rw-   0        0        0     2011 2023-06-23 11:51:39.000000 Akatosh-2.0.1/Akatosh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-06-23 11:51:39.000000 Akatosh-2.0.1/Akatosh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 11:51:39.000000 Akatosh-2.0.1/Akatosh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 11:51:39.000000 Akatosh-2.0.1/Akatosh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2011 2023-06-23 11:51:39.300010 Akatosh-2.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1482 2023-06-21 04:34:02.000000 Akatosh-2.0.1/README.md
+-rw-rw-rw-   0        0        0      669 2023-06-23 11:48:57.000000 Akatosh-2.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 11:51:39.302010 Akatosh-2.0.1/setup.cfg
```

### Comparing `Akatosh-2.0.0/Akatosh/event.py` & `Akatosh-2.0.1/Akatosh/event.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.0.0/Akatosh/resource.py` & `Akatosh-2.0.1/Akatosh/resource.py`

 * *Files identical despite different names*

### Comparing `Akatosh-2.0.0/Akatosh/universe.py` & `Akatosh-2.0.1/Akatosh/universe.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,20 +15,27 @@
 class Universe:
     def __init__(self) -> None:
         self._resolution = 1
         self._now: int | float = 0
         self._future_events: List[Event] = list()
         self._current_events: List[Event] = list()
         self._past_events: List[Event] = list()
+        self._early_stop: bool = False
         self.set_logger(logging.ERROR)
 
-    async def akatosh(self):
+    async def akatosh(self, till: int | float | None = None):
         while len(self.future_events) != 0:
+            if self.early_stop:
+                return
+
             if self.now < min(event.at for event in self.future_events):
                 self._now = min(event.at for event in self.future_events)
+                if till:
+                    if self.now >= till:
+                        return
                 logger.debug(f"Time: {self.now}")
 
             for event in self.future_events:
                 if event.at == self.now:
                     if event.state == State.ACTIVE:
                         logger.debug(f"Event {event.label} is triggered.")
                         self.future_events.remove(event)
@@ -41,16 +48,16 @@
                         self.future_events.remove(event)
                         self.past_events.append(event)
                         event.state = State.ENDED
             self.current_events.sort(key=lambda event: event.priority)
 
             await asyncio.gather(*[actor._perform() for actor in self.current_events])
 
-    def simulate(self):
-        asyncio.run(self.akatosh())
+    def simulate(self, till: int | float | None = None):
+        asyncio.run(self.akatosh(till))
 
     def set_logger(self, level: int):
         logger.setLevel(level)
 
     @property
     def resolution(self) -> int:
         return self._resolution
@@ -67,9 +74,17 @@
     def current_events(self) -> List[Event]:
         return self._current_events
 
     @property
     def past_events(self) -> List[Event]:
         return self._past_events
 
+    @property
+    def early_stop(self) -> bool:
+        return self._early_stop
+
+    @early_stop.setter
+    def early_stop(self, value: bool):
+        self._early_stop = value
+
 
 mundus = Universe()
```

### Comparing `Akatosh-2.0.0/Akatosh.egg-info/PKG-INFO` & `Akatosh-2.0.1/Akatosh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.0.0
+Version: 2.0.1
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `Akatosh-2.0.0/PKG-INFO` & `Akatosh-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Akatosh
-Version: 2.0.0
+Version: 2.0.1
 Summary: A simple implement for discrete events simulation.
 Author-email: Yifei Ren <ryf0510@live.com>
 Project-URL: Homepage, https://github.com/ulfaric/Akatosh
 Project-URL: Bug Tracker, https://github.com/ulfaric/Akatosh/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `Akatosh-2.0.0/README.md` & `Akatosh-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Akatosh-2.0.0/pyproject.toml` & `Akatosh-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "Akatosh"
-version = "2.0.0"
+version = "2.0.1"
 authors = [{ name = "Yifei Ren", email = "ryf0510@live.com" }]
 description = "A simple implement for discrete events simulation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

