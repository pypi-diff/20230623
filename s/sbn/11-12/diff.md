# Comparing `tmp/sbn-11.tar.gz` & `tmp/sbn-12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbn-11.tar", last modified: Tue Jun 20 12:36:31 2023, max compression
+gzip compressed data, was "sbn-12.tar", last modified: Fri Jun 23 14:27:51 2023, max compression
```

## Comparing `sbn-11.tar` & `sbn-12.tar`

### file list

```diff
@@ -1,58 +1,76 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-20 12:36:31.168132 sbn-11/
--rw-r--r--   0 bart      (1000) bart      (1000)     2958 2023-06-20 12:36:31.168132 sbn-11/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     2396 2023-06-20 12:31:49.000000 sbn-11/README.rst
--rw-r--r--   0 bart      (1000) bart      (1000)      899 2023-06-20 12:32:28.000000 sbn-11/pyproject.toml
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-20 12:36:31.164132 sbn-11/sbn/
--rw-r--r--   0 bart      (1000) bart      (1000)      871 2023-06-19 11:01:18.000000 sbn-11/sbn/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2526 2023-06-20 12:35:00.000000 sbn-11/sbn/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      600 2023-06-19 11:01:18.000000 sbn-11/sbn/clients.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1110 2023-06-19 11:01:18.000000 sbn-11/sbn/clocked.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1631 2023-06-19 11:01:18.000000 sbn-11/sbn/command.py
--rw-r--r--   0 bart      (1000) bart      (1000)      180 2023-06-19 11:01:18.000000 sbn-11/sbn/configs.py
--rw-r--r--   0 bart      (1000) bart      (1000)      817 2023-06-19 11:01:18.000000 sbn-11/sbn/decoder.py
--rw-r--r--   0 bart      (1000) bart      (1000)      399 2023-06-19 11:01:18.000000 sbn-11/sbn/default.py
--rw-r--r--   0 bart      (1000) bart      (1000)      302 2023-06-19 11:01:18.000000 sbn-11/sbn/defines.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1344 2023-06-19 11:01:18.000000 sbn-11/sbn/encoder.py
--rw-r--r--   0 bart      (1000) bart      (1000)      381 2023-06-19 11:01:18.000000 sbn-11/sbn/errored.py
--rw-r--r--   0 bart      (1000) bart      (1000)      956 2023-06-19 11:01:18.000000 sbn-11/sbn/evented.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1974 2023-06-19 11:01:18.000000 sbn-11/sbn/handler.py
--rw-r--r--   0 bart      (1000) bart      (1000)      954 2023-06-19 11:01:18.000000 sbn-11/sbn/listens.py
--rw-r--r--   0 bart      (1000) bart      (1000)      466 2023-06-19 11:01:18.000000 sbn-11/sbn/logging.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-20 12:36:31.168132 sbn-11/sbn/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      553 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      596 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/cfg.py
--rw-r--r--   0 bart      (1000) bart      (1000)      234 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      730 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      439 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      979 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    20870 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      725 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3615 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17837 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/mdl.py
--rw-r--r--   0 bart      (1000) bart      (1000)      208 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2355 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)     7741 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)      377 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/sts.py
--rw-r--r--   0 bart      (1000) bart      (1000)      964 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1014 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2448 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1000)      236 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/upt.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5769 2023-06-19 11:01:18.000000 sbn-11/sbn/modules/wsd.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2033 2023-06-19 11:01:18.000000 sbn-11/sbn/objects.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2181 2023-06-19 11:01:18.000000 sbn-11/sbn/objfunc.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1839 2023-06-19 11:01:18.000000 sbn-11/sbn/parsers.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4739 2023-06-19 11:01:18.000000 sbn-11/sbn/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)      380 2023-06-19 11:01:18.000000 sbn-11/sbn/repeats.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2667 2023-06-20 12:34:11.000000 sbn-11/sbn/runtime.py
--rw-r--r--   0 bart      (1000) bart      (1000)      928 2023-06-19 11:01:18.000000 sbn-11/sbn/threads.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2949 2023-06-19 11:01:18.000000 sbn-11/sbn/utility.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-20 12:36:31.164132 sbn-11/sbn.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2958 2023-06-20 12:36:31.000000 sbn-11/sbn.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      933 2023-06-20 12:36:31.000000 sbn-11/sbn.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-06-20 12:36:31.000000 sbn-11/sbn.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       42 2023-06-20 12:36:31.000000 sbn-11/sbn.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-06-20 12:36:31.000000 sbn-11/sbn.egg-info/requires.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-06-20 12:36:31.000000 sbn-11/sbn.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-06-20 12:36:31.000000 sbn-11/sbn.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-06-20 12:36:31.168132 sbn-11/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      101 2023-06-19 11:01:18.000000 sbn-11/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-23 14:27:51.657055 sbn-12/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2958 2023-06-23 14:27:51.657055 sbn-12/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     2396 2023-06-20 12:31:49.000000 sbn-12/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-23 14:27:51.645054 sbn-12/files/
+-rw-r--r--   0 bart      (1000) bart      (1000)   180711 2023-06-22 12:55:52.000000 sbn-12/files/ECHAabilify.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   193757 2023-06-22 12:55:52.000000 sbn-12/files/ECHAclozapine.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   197697 2023-06-22 12:55:52.000000 sbn-12/files/ECHAhaldol.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   232313 2023-06-22 12:55:52.000000 sbn-12/files/ECHAzyprexa.png
+-rw-r--r--   0 bart      (1000) bart      (1000)  1685507 2023-06-22 11:04:43.000000 sbn-12/files/bevestigd.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)    69979 2023-06-22 12:56:01.000000 sbn-12/files/informed.jpg
+-rw-r--r--   0 bart      (1000) bart      (1000)   287102 2023-06-20 11:29:34.000000 sbn-12/files/skull3.png
+-rw-r--r--   0 bart      (1000) bart      (1000)   234877 2023-06-20 11:35:00.000000 sbn-12/files/verbatim2.png
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-23 14:27:51.653054 sbn-12/pdf/
+-rw-r--r--   0 bart      (1000) bart      (1000)   238330 2023-06-22 10:55:52.000000 sbn-12/pdf/EM_T04_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   236671 2023-06-22 10:55:52.000000 sbn-12/pdf/EM_T07_OTP-CR-117_19_001.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   257079 2023-06-22 10:55:52.000000 sbn-12/pdf/Elements-of-Crimes.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)    41559 2023-06-22 10:55:52.000000 sbn-12/pdf/Kamer.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   323490 2023-06-22 10:55:52.000000 sbn-12/pdf/Rome-Statute.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   571580 2023-06-22 10:55:52.000000 sbn-12/pdf/Rules-of-Procedure-and-Evidence.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)    50044 2023-06-22 10:55:52.000000 sbn-12/pdf/bevestigd.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)     1580 2023-06-22 13:08:51.000000 sbn-12/pyproject.toml
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-23 14:27:51.657055 sbn-12/sbn/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3213 2023-06-21 12:03:14.000000 sbn-12/sbn/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2521 2023-06-23 12:19:48.000000 sbn-12/sbn/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      600 2023-06-19 11:01:18.000000 sbn-12/sbn/clients.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1110 2023-06-19 11:01:18.000000 sbn-12/sbn/clocked.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2094 2023-06-22 10:49:46.000000 sbn-12/sbn/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      180 2023-06-19 11:01:18.000000 sbn-12/sbn/configs.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      817 2023-06-19 11:01:18.000000 sbn-12/sbn/decoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      399 2023-06-19 11:01:18.000000 sbn-12/sbn/default.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      302 2023-06-19 11:01:18.000000 sbn-12/sbn/defines.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1344 2023-06-19 11:01:18.000000 sbn-12/sbn/encoder.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      381 2023-06-19 11:01:18.000000 sbn-12/sbn/errored.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      956 2023-06-19 11:01:18.000000 sbn-12/sbn/evented.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1974 2023-06-19 11:01:18.000000 sbn-12/sbn/handler.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      954 2023-06-19 11:01:18.000000 sbn-12/sbn/listens.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      466 2023-06-19 11:01:18.000000 sbn-12/sbn/logging.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-23 14:27:51.657055 sbn-12/sbn/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      577 2023-06-21 14:58:57.000000 sbn-12/sbn/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      596 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/cfg.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      234 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      730 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      439 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      979 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    20870 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      725 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3615 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/mbx.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17837 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      208 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2355 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      830 2023-06-22 10:51:45.000000 sbn-12/sbn/modules/rld.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     7741 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      377 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/sts.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      964 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1014 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2448 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/udp.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      236 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/upt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5769 2023-06-19 11:01:18.000000 sbn-12/sbn/modules/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2033 2023-06-19 11:01:18.000000 sbn-12/sbn/objects.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2181 2023-06-19 11:01:18.000000 sbn-12/sbn/objfunc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1839 2023-06-19 11:01:18.000000 sbn-12/sbn/parsers.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     4739 2023-06-19 11:01:18.000000 sbn-12/sbn/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      380 2023-06-19 11:01:18.000000 sbn-12/sbn/repeats.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2671 2023-06-21 14:02:53.000000 sbn-12/sbn/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      928 2023-06-19 11:01:18.000000 sbn-12/sbn/threads.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2949 2023-06-19 11:01:18.000000 sbn-12/sbn/utility.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2023-06-23 14:27:51.657055 sbn-12/sbn.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2958 2023-06-23 14:27:51.000000 sbn-12/sbn.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1299 2023-06-23 14:27:51.000000 sbn-12/sbn.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-06-23 14:27:51.000000 sbn-12/sbn.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       42 2023-06-23 14:27:51.000000 sbn-12/sbn.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        7 2023-06-23 14:27:51.000000 sbn-12/sbn.egg-info/requires.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        4 2023-06-23 14:27:51.000000 sbn-12/sbn.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2023-06-23 14:27:51.000000 sbn-12/sbn.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2023-06-23 14:27:51.657055 sbn-12/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      101 2023-06-19 11:01:18.000000 sbn-12/setup.py
```

### Comparing `sbn-11/PKG-INFO` & `sbn-12/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbn
-Version: 11
+Version: 12
 Summary: Skull, Bones and Number (OTP-CR-117/19)
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/sbn
 Project-URL: bugs, https://github.com/bthate/sbn/issues
 Project-URL: source, https://github.com/bthate/sbn
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sbn-11/README.rst` & `sbn-12/README.rst`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/__main__.py` & `sbn-12/sbn/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from sbn.runtime import scanstr, waiter
 
 
 import sbn.modules
 Commands.modules = sbn.modules
 
 
-__VERSION__ = "11"
+__VERSION__ = "12"
 
 
 NAME = "sbn"
 
 
 Persist.workdir = os.path.expanduser(f"~/.{NAME}")
 
@@ -77,15 +77,15 @@
     try:
         old = termios.tcgetattr(fds)
     except termios.error:
         gotterm = False
     try:
         func()
     except (EOFError, KeyboardInterrupt):
-        print('')
+        pass
     finally:
         if gotterm:
             termios.tcsetattr(fds, termios.TCSADRAIN, old)
         waiter()
 
 
 def ver(event):
```

### Comparing `sbn-11/sbn/clients.py` & `sbn-12/sbn/clients.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/clocked.py` & `sbn-12/sbn/clocked.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/command.py` & `sbn-12/sbn/command.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import inspect
 
 
 from .errored import Errors
 from .evented import Event
 from .logging import Logging
-from .objects import Object, copy
+from .objects import Object, copy, keys
 
 
 def __dir__():
     return (
             'Commands',
            )
 
@@ -59,11 +59,25 @@
                 evt.show()
             except Exception as ex:
                 Errors.handle(ex)
         evt.ready()
         return evt
 
     @staticmethod
+    def remove(func) -> None:
+        cmd = func.__name__.split(".")[-1]
+        if cmd in keys(Commands.cmds):
+            delattr(Commands.cmds, cmd)
+        if cmd in keys(Commands.modnames):
+            delattr(Commands.modnames, cmd)
+
+    @staticmethod
+    def unload(mod):
+        for _key, cmd in inspect.getmembers(mod, inspect.isfunction):
+            if 'event' in cmd.__code__.co_varnames:
+                Commands.remove(cmd)
+
+    @staticmethod
     def scan(mod) -> None:
         for _key, cmd in inspect.getmembers(mod, inspect.isfunction):
             if 'event' in cmd.__code__.co_varnames:
                 Commands.add(cmd)
```

### Comparing `sbn-11/sbn/decoder.py` & `sbn-12/sbn/decoder.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/encoder.py` & `sbn-12/sbn/encoder.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/evented.py` & `sbn-12/sbn/evented.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/handler.py` & `sbn-12/sbn/handler.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/listens.py` & `sbn-12/sbn/listens.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/modules/cfg.py` & `sbn-12/sbn/modules/cfg.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/modules/err.py` & `sbn-12/sbn/modules/err.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/modules/fnd.py` & `sbn-12/sbn/modules/fnd.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/modules/irc.py` & `sbn-12/sbn/modules/irc.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/modules/log.py` & `sbn-12/sbn/modules/log.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/modules/mbx.py` & `sbn-12/sbn/modules/mbx.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/modules/mdl.py` & `sbn-12/sbn/modules/mdl.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/modules/req.py` & `sbn-12/sbn/modules/req.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/modules/rss.py` & `sbn-12/sbn/modules/rss.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/modules/tdo.py` & `sbn-12/sbn/modules/tdo.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/modules/thr.py` & `sbn-12/sbn/modules/thr.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/modules/udp.py` & `sbn-12/sbn/modules/udp.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/modules/wsd.py` & `sbn-12/sbn/modules/wsd.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/objects.py` & `sbn-12/sbn/objects.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/objfunc.py` & `sbn-12/sbn/objfunc.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/parsers.py` & `sbn-12/sbn/parsers.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/persist.py` & `sbn-12/sbn/persist.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/runtime.py` & `sbn-12/sbn/runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 DATE = time.ctime(time.time()).replace("  ", " ")
 NAME = __name__.split('.', maxsplit=1)[0]
 STARTTIME = time.time()
 
 
 Cfg.debug = False
-Cfg.mod = "cmd,err,flt,mod,sts,thr,upt,ver"
+Cfg.mod = "cmd,err,flt,mod,rld,sts,thr,upt,ver"
 Cfg.skip = "PING,PONG,PRIVMSG"
 Cfg.threaded = False
 Cfg.version = "122"
 
 
 # FUNCTIONS
```

### Comparing `sbn-11/sbn/threads.py` & `sbn-12/sbn/threads.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn/utility.py` & `sbn-12/sbn/utility.py`

 * *Files identical despite different names*

### Comparing `sbn-11/sbn.egg-info/PKG-INFO` & `sbn-12/sbn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbn
-Version: 11
+Version: 12
 Summary: Skull, Bones and Number (OTP-CR-117/19)
 Author-email: Bart Thate <bthate@dds.nl>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/sbn
 Project-URL: bugs, https://github.com/bthate/sbn/issues
 Project-URL: source, https://github.com/bthate/sbn
 Classifier: Development Status :: 3 - Alpha
```

