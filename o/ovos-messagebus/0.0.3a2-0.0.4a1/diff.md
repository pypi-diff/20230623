# Comparing `tmp/ovos-messagebus-0.0.3a2.tar.gz` & `tmp/ovos-messagebus-0.0.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-messagebus-0.0.3a2.tar", last modified: Wed May 24 16:01:45 2023, max compression
+gzip compressed data, was "ovos-messagebus-0.0.4a1.tar", last modified: Fri Jun 23 16:37:19 2023, max compression
```

## Comparing `ovos-messagebus-0.0.3a2.tar` & `ovos-messagebus-0.0.4a1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:01:45.951281 ovos-messagebus-0.0.3a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-05-24 16:01:44.000000 ovos-messagebus-0.0.3a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 16:01:44.000000 ovos-messagebus-0.0.3a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-24 16:01:45.951281 ovos-messagebus-0.0.3a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-24 16:01:44.000000 ovos-messagebus-0.0.3a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:01:45.951281 ovos-messagebus-0.0.3a2/ovos_messagebus/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-24 16:01:44.000000 ovos-messagebus-0.0.3a2/ovos_messagebus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-24 16:01:44.000000 ovos-messagebus-0.0.3a2/ovos_messagebus/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-24 16:01:44.000000 ovos-messagebus-0.0.3a2/ovos_messagebus/event_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-24 16:01:44.000000 ovos-messagebus-0.0.3a2/ovos_messagebus/load_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-24 16:01:44.000000 ovos-messagebus-0.0.3a2/ovos_messagebus/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:01:45.951281 ovos-messagebus-0.0.3a2/ovos_messagebus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-24 16:01:45.000000 ovos-messagebus-0.0.3a2/ovos_messagebus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-24 16:01:45.000000 ovos-messagebus-0.0.3a2/ovos_messagebus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:01:45.000000 ovos-messagebus-0.0.3a2/ovos_messagebus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-24 16:01:45.000000 ovos-messagebus-0.0.3a2/ovos_messagebus.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-24 16:01:45.000000 ovos-messagebus-0.0.3a2/ovos_messagebus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-24 16:01:45.000000 ovos-messagebus-0.0.3a2/ovos_messagebus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-24 16:01:44.000000 ovos-messagebus-0.0.3a2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:01:45.951281 ovos-messagebus-0.0.3a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-05-24 16:01:44.000000 ovos-messagebus-0.0.3a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:37:19.800821 ovos-messagebus-0.0.4a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11423 2023-06-23 16:37:18.000000 ovos-messagebus-0.0.4a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 16:37:18.000000 ovos-messagebus-0.0.4a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-23 16:37:19.800821 ovos-messagebus-0.0.4a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-23 16:37:18.000000 ovos-messagebus-0.0.4a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:37:19.800821 ovos-messagebus-0.0.4a1/ovos_messagebus/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-23 16:37:18.000000 ovos-messagebus-0.0.4a1/ovos_messagebus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-23 16:37:18.000000 ovos-messagebus-0.0.4a1/ovos_messagebus/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-23 16:37:18.000000 ovos-messagebus-0.0.4a1/ovos_messagebus/event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-23 16:37:18.000000 ovos-messagebus-0.0.4a1/ovos_messagebus/load_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-23 16:37:18.000000 ovos-messagebus-0.0.4a1/ovos_messagebus/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 16:37:19.800821 ovos-messagebus-0.0.4a1/ovos_messagebus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-23 16:37:19.000000 ovos-messagebus-0.0.4a1/ovos_messagebus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-23 16:37:19.000000 ovos-messagebus-0.0.4a1/ovos_messagebus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 16:37:19.000000 ovos-messagebus-0.0.4a1/ovos_messagebus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-23 16:37:19.000000 ovos-messagebus-0.0.4a1/ovos_messagebus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-23 16:37:19.000000 ovos-messagebus-0.0.4a1/ovos_messagebus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-23 16:37:19.000000 ovos-messagebus-0.0.4a1/ovos_messagebus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-23 16:37:18.000000 ovos-messagebus-0.0.4a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 16:37:19.800821 ovos-messagebus-0.0.4a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-06-23 16:37:18.000000 ovos-messagebus-0.0.4a1/setup.py
```

### Comparing `ovos-messagebus-0.0.3a2/LICENSE.md` & `ovos-messagebus-0.0.4a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-messagebus-0.0.3a2/README.md` & `ovos-messagebus-0.0.4a1/README.md`

 * *Files identical despite different names*

### Comparing `ovos-messagebus-0.0.3a2/ovos_messagebus/__init__.py` & `ovos-messagebus-0.0.4a1/ovos_messagebus/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-messagebus-0.0.3a2/ovos_messagebus/__main__.py` & `ovos-messagebus-0.0.4a1/ovos_messagebus/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 processes. It implements a websocket server so can also be used by external
 systems to integrate with the Mycroft system.
 """
 
 from ovos_utils import create_daemon, wait_for_exit_signal
 from ovos_messagebus.load_config import load_message_bus_config
 from ovos_utils.log import LOG, init_service_logger
-from ovos_utils.process_utils import reset_sigint_handler, PIDLock
+from ovos_utils.process_utils import reset_sigint_handler
 from tornado import web, ioloop
 
 from ovos_messagebus.event_handler import MessageBusEventHandler
 
 
 def on_ready():
     LOG.info('Message bus service started!')
@@ -37,18 +37,16 @@
 
 
 def on_stopping():
     LOG.info('Message bus is shutting down...')
 
 
 def main(ready_hook=on_ready, error_hook=on_error, stopping_hook=on_stopping):
-    PIDLock.init()
     reset_sigint_handler()
     init_service_logger("bus")
-    PIDLock("bus")
     LOG.info('Starting message bus service...')
     config = load_message_bus_config()
     routes = [(config.route, MessageBusEventHandler)]
     application = web.Application(routes)
     application.listen(config.port, config.host)
     create_daemon(ioloop.IOLoop.instance().start)
     ready_hook()
```

### Comparing `ovos-messagebus-0.0.3a2/ovos_messagebus/event_handler.py` & `ovos-messagebus-0.0.4a1/ovos_messagebus/event_handler.py`

 * *Files identical despite different names*

### Comparing `ovos-messagebus-0.0.3a2/ovos_messagebus/load_config.py` & `ovos-messagebus-0.0.4a1/ovos_messagebus/load_config.py`

 * *Files identical despite different names*

### Comparing `ovos-messagebus-0.0.3a2/setup.py` & `ovos-messagebus-0.0.4a1/setup.py`

 * *Files identical despite different names*

