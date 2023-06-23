# Comparing `tmp/walt-common-7.tar.gz` & `tmp/walt-common-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/walt-common-7.tar", last modified: Mon Feb  1 15:17:00 2021, max compression
+gzip compressed data, was "walt-common-8.0.tar", last modified: Fri Jun 23 07:38:01 2023, max compression
```

## Comparing `walt-common-7.tar` & `walt-common-8.0.tar`

### file list

```diff
@@ -1,41 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:00.000000 walt-common-7/
--rw-r--r--   0 root         (0) root         (0)      288 2021-02-01 15:17:00.000000 walt-common-7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      144 2020-09-24 12:01:14.000000 walt-common-7/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-02-01 15:17:00.000000 walt-common-7/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      340 2020-09-24 12:01:14.000000 walt-common-7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:00.000000 walt-common-7/walt/
--rw-r--r--   0 root         (0) root         (0)      147 2020-09-24 12:01:14.000000 walt-common-7/walt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:00.000000 walt-common-7/walt/common/
--rw-r--r--   0 root         (0) root         (0)       44 2020-09-24 12:01:14.000000 walt-common-7/walt/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2561 2020-09-24 12:01:14.000000 walt-common-7/walt/common/api.py
--rwxr-xr-x   0 root         (0) root         (0)     7283 2020-09-24 12:01:14.000000 walt-common-7/walt/common/apilink.py
--rw-r--r--   0 root         (0) root         (0)      977 2020-09-24 12:01:14.000000 walt-common-7/walt/common/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:00.000000 walt-common-7/walt/common/crypto/
--rw-r--r--   0 root         (0) root         (0)      834 2020-09-24 12:01:14.000000 walt-common-7/walt/common/crypto/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19853 2020-09-24 12:01:14.000000 walt-common-7/walt/common/crypto/blowfish.py
--rwxr-xr-x   0 root         (0) root         (0)     2239 2020-09-24 12:01:14.000000 walt-common-7/walt/common/crypto/dh.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:00.000000 walt-common-7/walt/common/devices/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-24 12:01:14.000000 walt-common-7/walt/common/devices/__init__.py
--rw-r--r--   0 root         (0) root         (0)      675 2020-09-24 12:01:14.000000 walt-common-7/walt/common/devices/registry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:00.000000 walt-common-7/walt/common/devices/switches/
--rw-r--r--   0 root         (0) root         (0)       21 2020-09-24 12:01:14.000000 walt-common-7/walt/common/devices/switches/__init__.py
--rw-r--r--   0 root         (0) root         (0)      238 2020-09-24 12:01:14.000000 walt-common-7/walt/common/devices/switches/netgear.py
--rwxr-xr-x   0 root         (0) root         (0)     5184 2020-09-24 12:01:14.000000 walt-common-7/walt/common/evloop.py
--rwxr-xr-x   0 root         (0) root         (0)     2947 2020-09-24 12:01:14.000000 walt-common-7/walt/common/fifo.py
--rw-r--r--   0 root         (0) root         (0)      431 2021-02-01 15:16:44.000000 walt-common-7/walt/common/info.py
--rwxr-xr-x   0 root         (0) root         (0)     2603 2020-09-24 12:01:14.000000 walt-common-7/walt/common/io.py
--rw-r--r--   0 root         (0) root         (0)     1755 2020-09-24 12:01:14.000000 walt-common-7/walt/common/logs.py
--rw-r--r--   0 root         (0) root         (0)     1131 2020-09-24 12:01:14.000000 walt-common-7/walt/common/reusable.py
--rw-r--r--   0 root         (0) root         (0)     4233 2020-09-24 12:01:14.000000 walt-common-7/walt/common/tcp.py
--rw-r--r--   0 root         (0) root         (0)     7967 2020-09-24 12:01:14.000000 walt-common-7/walt/common/thread.py
--rw-r--r--   0 root         (0) root         (0)     7384 2020-09-24 12:01:14.000000 walt-common-7/walt/common/tools.py
--rwxr-xr-x   0 root         (0) root         (0)      937 2020-09-24 12:01:14.000000 walt-common-7/walt/common/tty.py
--rw-r--r--   0 root         (0) root         (0)      389 2020-09-24 12:01:14.000000 walt-common-7/walt/common/udp.py
--rw-r--r--   0 root         (0) root         (0)     1222 2020-09-24 12:01:14.000000 walt-common-7/walt/common/update.py
--rw-r--r--   0 root         (0) root         (0)       18 2021-02-01 15:16:44.000000 walt-common-7/walt/common/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:00.000000 walt-common-7/walt_common.egg-info/
--rw-r--r--   0 root         (0) root         (0)      288 2021-02-01 15:17:00.000000 walt-common-7/walt_common.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      802 2021-02-01 15:17:00.000000 walt-common-7/walt_common.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-01 15:17:00.000000 walt-common-7/walt_common.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       15 2021-02-01 15:17:00.000000 walt-common-7/walt_common.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2021-02-01 15:17:00.000000 walt-common-7/walt_common.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:01.264801 walt-common-8.0/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-23 07:38:01.264801 walt-common-8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      144 2022-03-29 14:58:03.000000 walt-common-8.0/README.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 07:38:01.264801 walt-common-8.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      749 2023-06-23 07:37:56.000000 walt-common-8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:01.260801 walt-common-8.0/walt/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-common-8.0/walt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:01.264801 walt-common-8.0/walt/common/
+-rw-r--r--   0 root         (0) root         (0)       71 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/api.py
+-rwxr-xr-x   0 root         (0) root         (0)    11877 2023-06-22 13:09:04.000000 walt-common-8.0/walt/common/apilink.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/busybox_init.py
+-rw-r--r--   0 root         (0) root         (0)     2962 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/config.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:01.264801 walt-common-8.0/walt/common/crypto/
+-rw-r--r--   0 root         (0) root         (0)      833 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/crypto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30717 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/crypto/blowfish.py
+-rwxr-xr-x   0 root         (0) root         (0)     2289 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/crypto/dh.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:01.264801 walt-common-8.0/walt/common/devices/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-03-29 14:58:03.000000 walt-common-8.0/walt/common/devices/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/devices/registry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:01.264801 walt-common-8.0/walt/common/devices/switches/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/devices/switches/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      203 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/devices/switches/netgear.py
+-rwxr-xr-x   0 root         (0) root         (0)    10436 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/evloop.py
+-rw-r--r--   0 root         (0) root         (0)     9360 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/fakeipxe.py
+-rwxr-xr-x   0 root         (0) root         (0)     2996 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/fifo.py
+-rw-r--r--   0 root         (0) root         (0)     6734 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/formatting.py
+-rwxr-xr-x   0 root         (0) root         (0)      960 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/io.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/logs.py
+-rw-r--r--   0 root         (0) root         (0)      542 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/netsetup.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/reusable.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/service.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/settings.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/setup.py
+-rw-r--r--   0 root         (0) root         (0)     5348 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/systemd.py
+-rw-r--r--   0 root         (0) root         (0)     4096 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/tcp.py
+-rwxr-xr-x   0 root         (0) root         (0)     3976 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/term.py
+-rw-r--r--   0 root         (0) root         (0)     8286 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/tools.py
+-rwxr-xr-x   0 root         (0) root         (0)      967 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/tty.py
+-rw-r--r--   0 root         (0) root         (0)      390 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/udp.py
+-rw-r--r--   0 root         (0) root         (0)     2629 2023-06-21 15:19:09.000000 walt-common-8.0/walt/common/unix.py
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-23 07:37:56.000000 walt-common-8.0/walt/common/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:01.264801 walt-common-8.0/walt_common.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      251 2023-06-23 07:38:01.000000 walt-common-8.0/walt_common.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-23 07:38:01.000000 walt-common-8.0/walt_common.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 07:38:01.000000 walt-common-8.0/walt_common.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       69 2023-06-23 07:38:01.000000 walt-common-8.0/walt_common.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 07:38:01.000000 walt-common-8.0/walt_common.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `walt-common-7/walt/common/api.py` & `walt-common-8.0/walt/common/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,69 @@
 # -*- coding: utf-8 -*-
 explorer = None
 
+
 def register_api_explorer(expl):
     global explorer
     explorer = expl
 
+
 # mark methods to be exposed by replacing them by
 # an instance of APIExposedMethod class.
 # (we cannot rename these attributes here, their 'name'
 # belongs to the class. That's why we need
 # the other decorator @api below.)
 class APIExposedMethod(object):
     def __init__(self, func):
         self.func = func
 
+
 def api_expose_method(func):
     return APIExposedMethod(func)
 
+
 # given an __init__ constructor and a set of
 # attributes that must be exposed, compute a decorated
 # __init__ function, that will rename the attrs at the
 # end of the provided constructor.
 class APIDecoratedInit(object):
     def __init__(self, attrs, init_func):
         self.attrs = attrs
+
         def decorated_init_func(obj, *args, **kwargs):
             init_func(obj, *args, **kwargs)
             for attr in attrs:
                 val = getattr(obj, attr)
-                setattr(obj, 'exposed_' + attr, val)
+                setattr(obj, "exposed_" + attr, val)
+
         self.decorated_init = decorated_init_func
 
+
 # return a decorator to be applied to an __init__ function
 # and able to handle a list of attributes that must be exposed.
 def api_expose_attrs(*attrs):
     def decorator(init_func):
         return APIDecoratedInit(attrs, init_func)
+
     return decorator
 
+
 # expose class attributes specified.
 def api_expose_class_attrs(*c_attrs):
     def decorator(cls):
         for c_attr in c_attrs:
             if explorer:
                 explorer.add_attr(cls, c_attr)
             val = getattr(cls, c_attr)
-            setattr(cls, 'exposed_' + c_attr, val)
+            setattr(cls, "exposed_" + c_attr, val)
         return cls
+
     return decorator
 
+
 # Behavior in production code:
 # loop through attributes of the class...
 # * look for any instance of class APIExposedMethod,
 # replace these by the original method, and
 # duplicate them by prefixing 'exposed_'
 # * look for any instance of class APIDecoratedInit,
 # replace these by the decorated __init__
@@ -69,8 +80,7 @@
             setattr(cls, "exposed_%s" % k, v.func)
         elif isinstance(v, APIDecoratedInit):
             if explorer:
                 for attr in v.attrs:
                     explorer.add_attr(cls, attr)
             setattr(cls, k, v.decorated_init)
     return cls
-
```

### Comparing `walt-common-7/walt/common/crypto/__init__.py` & `walt-common-8.0/walt/common/crypto/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,7 @@
 #
 # Given these facts, we have implemented a simple process:
 # At each 'walt image publish' command:
 # 1) server and client generate a random key
 # 2) an encryption key is agreed using Diffie Hellman process
 # 3) the password is encrypted based on this encryption key
 #    using a pure-python implementation of the blowfish algorithm.
-
```

### Comparing `walt-common-7/walt/common/crypto/dh.py` & `walt-common-8.0/walt/common/crypto/dh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,68 @@
 #!/usr/bin/env python
 import random
 
+
 class DiffieHellman(object):
     BITSIZE = 2048
 
     # RFC 5114 section 2.3
-    p = int(''.join("""
+    p = int(
+        "".join("""
     87A8E61D B4B6663C FFBBD19C 65195999 8CEEF608 660DD0F2
     5D2CEED4 435E3B00 E00DF8F1 D61957D4 FAF7DF45 61B2AA30
     16C3D911 34096FAA 3BF4296D 830E9A7C 209E0C64 97517ABD
     5A8A9D30 6BCF67ED 91F9E672 5B4758C0 22E0B1EF 4275BF7B
     6C5BFC11 D45F9088 B941F54E B1E59BB8 BC39A0BF 12307F5C
     4FDB70C5 81B23F76 B63ACAE1 CAA6B790 2D525267 35488A0E
     F13C6D9A 51BFA4AB 3AD83477 96524D8E F6A167B5 A41825D9
     67E144E5 14056425 1CCACB83 E6B486F6 B3CA3F79 71506026
     C0B857F6 89962856 DED4010A BD0BE621 C3A3960A 54E710C3
     75F26375 D7014103 A4B54330 C198AF12 6116D227 6E11715F
     693877FA D7EF09CA DB094AE9 1E1A1597
-    """.split()), 16)
+    """.split()),
+        16,
+    )
 
-    g = int(''.join("""
+    g = int(
+        "".join("""
     3FB32C9B 73134D0B 2E775066 60EDBD48 4CA7B18F 21EF2054
     07F4793A 1A0BA125 10DBC150 77BE463F FF4FED4A AC0BB555
     BE3A6C1B 0C6B47B1 BC3773BF 7E8C6F62 901228F8 C28CBB18
     A55AE313 41000A65 0196F931 C77A57F2 DDF463E5 E9EC144B
     777DE62A AAB8A862 8AC376D2 82D6ED38 64E67982 428EBC83
     1D14348F 6F2F9193 B5045AF2 767164E1 DFC967C1 FB3F2E55
     A4BD1BFF E83B9C80 D052B985 D182EA0A DB2A3B73 13D3FE14
     C8484B1E 052588B9 B7D2BBD2 DF016199 ECD06E15 57CD0915
     B3353BBB 64E0EC37 7FD02837 0DF92B52 C7891428 CDC67EB6
     184B523D 1DB246C3 2F630784 90F00EF8 D647D148 D4795451
     5E2327CF EF98C582 664B4C0F 6CC41659
-    """.split()), 16)
+    """.split()),
+        16,
+    )
 
     @staticmethod
     def generate_priv_key():
         return random.getrandbits(DiffieHellman.BITSIZE)
 
     @staticmethod
     def generate_pub_key(priv_key):
         return pow(DiffieHellman.g, priv_key, DiffieHellman.p)
 
     @staticmethod
     def generate_symmetric_key(remote_pub_key, priv_key):
         return pow(remote_pub_key, priv_key, DiffieHellman.p)
 
+
 class DHPeer(object):
     def __init__(self):
         self.priv_key = DiffieHellman.generate_priv_key()
         self.pub_key = DiffieHellman.generate_pub_key(self.priv_key)
         self.symmetric_key = None
+
     def get_pub_key(self):
         return self.pub_key
+
     def establish_session(self, remote_pub_key):
         self.symmetric_key = DiffieHellman.generate_symmetric_key(
-                    remote_pub_key, self.priv_key)
-
+            remote_pub_key, self.priv_key
+        )
```

### Comparing `walt-common-7/walt/common/devices/registry.py` & `walt-common-8.0/walt/common/devices/registry.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-import inspect
-from walt.common.devices import switches
-from walt.common.devices.switches import *
+PROBE_FUNCTIONS = None
 
-PROBE_FUNCTIONS = []
 
 def get_device_info_from_mac(mac):
+    if PROBE_FUNCTIONS is None:
+        register_all_probe_functions()
     for probe in PROBE_FUNCTIONS:
         info = probe(mac)
         if info is not None:
             return info
-    return {}     # no information found
+    return {}  # no information found
+
 
 def register_all_probe_functions():
+    global PROBE_FUNCTIONS
+    import inspect
+
+    from walt.common.devices import switches
+
     all_modules = []
     # add all modules in 'switches' subdir
     for package in (switches,):
-        all_modules.extend(module for name, module in \
-                    inspect.getmembers(package, inspect.ismodule))
-    for module in all_modules:
-        PROBE_FUNCTIONS.append(module.probe)
-
-register_all_probe_functions()
+        all_modules.extend(
+            module for name, module in inspect.getmembers(package, inspect.ismodule)
+        )
+    PROBE_FUNCTIONS = [module.probe for module in all_modules]
```

### Comparing `walt-common-7/walt/common/fifo.py` & `walt-common-8.0/walt/common/fifo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,85 +1,102 @@
 #!/usr/bin/env python
-import os, stat, select
-from walt.common.tools import failsafe_makedirs, fd_copy
+import os
+import select
+import stat
 from threading import Thread
 
-RW_ALL = stat.S_IRUSR | stat.S_IWUSR | \
-         stat.S_IRGRP | stat.S_IWGRP | \
-         stat.S_IROTH | stat.S_IWOTH
+from walt.common.tools import failsafe_makedirs, fd_copy
+
+RW_ALL = (
+    stat.S_IRUSR
+    | stat.S_IWUSR
+    | stat.S_IRGRP
+    | stat.S_IWGRP
+    | stat.S_IROTH
+    | stat.S_IWOTH
+)
 BUFFER_SIZE = 1024
 
-def failsafe_mkfifo(path, mode = None):
-    if mode == None:
+
+def failsafe_mkfifo(path, mode=None):
+    if mode is None:
         mode = RW_ALL
     # check if it does not exist already
     if os.path.exists(path):
         return
     # ensure parent dir exists
     failsafe_makedirs(os.path.dirname(path))
     # create the fifo
     os.mkfifo(path)
     os.chmod(path, mode)
 
+
 # fifos are special files.
 # * when opening on one end, it will block until another process attempts to
 #   open the other end.
 # * when closed on one end, we should also close on the other end. For example,
 #   if we are reading on /tmp/fifo and issuie 'echo test > /tmp/fifo' on another
 #   terminal, we will receive 'test' but then we cannot start reading again
 #   because the fifo has been closed on the 'echo' side. Instead, we should
 #   close and re-open the fifo in order to get the next request.
 # Because of that, we handle the fifo objects by running a dedicated thread
 # that releases the main thread from fifo management work. The dedicated thread
 # just dumps everything from the fifo to a pipe. The main thread reads the other
 # end of this pipe. This allows the main thread to implement usual IO mechanisms
 # (select(), etc.).
 
+
 class ReadableFifo(object):
     def __init__(self, path):
         self.path = path
+
     def open(self):
         failsafe_mkfifo(self.path)
         data_r, data_w = os.pipe()
         ctrl_r, self.ctrl_w = os.pipe()
         t = Thread(target=self.reader_thread, args=(data_w, ctrl_r))
         t.start()
-        self.file_r = os.fdopen(data_r, 'r', 0)
+        self.file_r = os.fdopen(data_r, "rb", 0)
+
     def reader_thread(self, data_w, ctrl_r):
         should_stop = False
         while not should_stop:
             fifo_fd = os.open(self.path, os.O_RDONLY | os.O_NONBLOCK)
             fds = [fifo_fd, ctrl_r]
             while len(fds) == 2:
-                r, w, e = select.select(fds,[],[])
+                r, w, e = select.select(fds, [], [])
                 if fifo_fd in r:
                     fd_copy(fifo_fd, data_w, BUFFER_SIZE) or fds.remove(fifo_fd)
                 else:
                     os.read(ctrl_r, 1)
                     should_stop = True
                     break
             os.close(fifo_fd)
         os.close(data_w)
         os.close(ctrl_r)
+
     def close(self):
         try:
-            os.write(self.ctrl_w, 'X')
+            os.write(self.ctrl_w, "X")
             os.close(self.ctrl_w)
-        except:
+        except Exception:
             pass
         try:
             self.file_r.close()
-        except:
+        except Exception:
             pass
+
     def __enter__(self):
         return self.file_r
+
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.close()
+
     # redirect other accesses to self.file_r
     def __getattr__(self, attr):
         return getattr(self.file_r, attr)
 
+
 def open_readable_fifo(path):
     fifo = ReadableFifo(path)
     fifo.open()
     return fifo
-
```

### Comparing `walt-common-7/walt/common/logs.py` & `walt-common-8.0/walt/common/logs.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,47 @@
+import re
+import sys
+
 from plumbum import cli
-import sys, re
+
 
 class TeeStream:
     def __init__(self, std_stream, log_file, log_prefix):
         self.start_of_line = True
         self.streams = (std_stream,)
         if log_file is not None:
-            self.streams += (open(log_file, 'w'),)
+            self.streams += (open(log_file, "w"),)
         self.log_prefix = log_prefix
+
     def write_all(self, buf):
         for i, stream in enumerate(self.streams):
             stream.write(buf)
             if i > 0:
                 stream.flush()
+
     def write(self, buf):
         if self.log_prefix is None:
             self.write_all(buf)
         else:
-            for chunk in re.split('([\r\n])', buf):
+            for chunk in re.split("([\r\n])", buf):
                 if len(chunk) > 0:
                     if self.start_of_line:
                         self.write_all("[" + self.log_prefix + "] ")
                         self.start_of_line = False
                     self.write_all(chunk)
-                    if chunk in '\r\n':
+                    if chunk in "\r\n":
                         self.start_of_line = True
+
     def flush(self):
         return self.streams[0].flush()
+
     def fileno(self):
         return self.streams[0].fileno()
 
+
 class LoggedApplication(cli.Application):
     _log_file = None
     _log_prefix = None
 
     def init_logs(self):
         if self._log_file is not None or self._log_prefix is not None:
             sys.stdout = TeeStream(sys.stdout, self._log_file, self._log_prefix)
@@ -44,8 +52,7 @@
         """specify log filename for stdin / stderr"""
         self._log_file = log_file
 
     @cli.switch("--log-prefix", str)
     def set_log_prefix(self, log_prefix):
         """specify prefix to identify logs"""
         self._log_prefix = log_prefix
-
```

### Comparing `walt-common-7/walt/common/reusable.py` & `walt-common-8.0/walt/common/reusable.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import weakref, threading, atexit
-
 # This allows to define the 'reusable' decorator.
 # You can try for instance:
 #
 # @reusable
 # class C(object):
 #     def __init__(self, t):
 #         self.t = t
@@ -17,30 +15,33 @@
 # c = C(4)
 # c = None
 #
 # When decorated this way, if its constructor is invoked twice
 # with the same arguments, the same object will be found in
 # cache and returned.
 
+
 class ReusePool(object):
     def __init__(self, cls):
         self.cls = cls
         self.pool = {}
+
     def get(self, *args, **kwargs):
         argdesc = args, tuple(kwargs.items())
         if argdesc in self.pool:
             obj = self.pool[argdesc]
         else:
             obj = self.cls(*args, **kwargs)
             self.pool[argdesc] = obj
         return obj
 
+
 def reusable(cls):
     pool = ReusePool(cls)
+
     # we decorate a class but we return a function:
     # what seems to be a call to the class constructor
     # will actually be a call to this function.
     def func(*args, **kwargs):
         return pool.get(*args, **kwargs)
-    return func
-
 
+    return func
```

### Comparing `walt-common-7/walt/common/tcp.py` & `walt-common-8.0/walt/common/tcp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,139 +1,155 @@
-import socket, pickle
+import pickle
+import socket
+
+from walt.common.service import GenericServer, ServiceRequests
 from walt.common.tools import set_close_on_exec
-from walt.common.io import SmartFile
 
-class Requests(object):
+PICKLE_VERSION = 4  # from python 3.4
+
+
+class Requests(ServiceRequests):
     REQ_NEW_INCOMING_LOGS = 0
     REQ_DUMP_LOGS = 1
     REQ_SQL_PROMPT = 2
     REQ_DOCKER_PROMPT = 3
     REQ_NODE_CMD = 4
     REQ_DEVICE_PING = 5
     REQ_TAR_FROM_IMAGE = 6
     REQ_TAR_TO_IMAGE = 7
     REQ_TAR_FROM_NODE = 8
     REQ_TAR_TO_NODE = 9
     REQ_API_SESSION = 10
     REQ_TCP_TO_NODE = 11
     REQ_FAKE_TFTP_GET = 12
     REQ_VPN_NODE_IMAGE = 13
+    REQ_NOTIFY_BOOTUP_STATUS = 14
+    REQ_DEVICE_SHELL = 15
+    REQ_TAR_FOR_IMAGE_BUILD = 16
 
-    # the request id message may be specified directly as
-    # as a decimal string (e.g. '4') or by the corresponding
-    # name (e.g. 'REQ_NODE_CMD')
-    @staticmethod
-    def get_id(s):
-        try:
-            return int(s)
-        except:
-            try:
-                return getattr(Requests, s)
-            except:
-                return None
     @staticmethod
     def read_id(stream):
         try:
-            return Requests.get_id(stream.readline().decode('ascii').strip())
-        except:
+            return Requests.get_id(stream.readline().decode("ascii").strip())
+        except Exception:
             return None
+
     @staticmethod
     def send_id(stream, req_id):
-        stream.write(b'%d\n' % req_id)
+        stream.write(b"%d\n" % req_id)
         stream.flush()
 
+
 def read_pickle(stream):
     try:
         return pickle.load(stream)
-    except Exception as e:
+    except Exception:
         return None
 
+
 def write_pickle(obj, stream):
-    pickle.dump(obj, stream, pickle.HIGHEST_PROTOCOL)
+    pickle.dump(obj, stream, PICKLE_VERSION)
     stream.flush()
 
-class SmartSocketFile(SmartFile):
+
+class RWSocketFile:
     def __init__(self, sock):
         self.sock = sock
-        sock_r = sock.makefile('rb', 0)
-        sock_w = sock.makefile('wb', 0)
-        SmartFile.__init__(self, sock_r, sock_w)
+        self.file_r = sock.makefile("rb", 0)
+        self.file_w = sock.makefile("wb", 0)
+
     def shutdown(self, mode):
         return self.sock.shutdown(mode)
+
+    def getpeername(self):
+        return self.sock.getpeername()
+
+    def setsockopt(self, *args):
+        return self.sock.setsockopt(*args)
+
+    def __getattr__(self, attr):
+        if attr in ("write", "flush"):
+            f = self.file_w
+        else:
+            f = self.file_r
+        return getattr(f, attr)
+
+    @property
+    def closed(self):
+        return self.file_r is None
+
     def close(self):
+        if self.file_r is not None:
+            self.file_r.close()
+            self.file_r = None
+        if self.file_w is not None:
+            self.file_w.close()
+            self.file_w = None
         if self.sock is not None:
             self.sock.close()
             self.sock = None
-            SmartFile.close(self)
-    def getpeername(self):
-        return self.sock.getpeername()
+
+    def __del__(self):
+        self.close()
+
 
 def client_sock_file(host, port):
     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     # set close-on-exec flag (subprocesses should not inherit it)
     set_close_on_exec(s, True)
-    s.connect((host, port))
-    return SmartSocketFile(s)
+    try:
+        s.connect((host, port))
+    except Exception:
+        s.close()
+        raise
+    return RWSocketFile(s)
+
 
 class ServerSocketWrapper:
     def __init__(self, s):
         self.s = s
+
     def accept(self):
         s_conn, address = self.s.accept()
         # set close-on-exec flag (subprocesses should not inherit it)
         set_close_on_exec(s_conn, True)
         return s_conn, address
+
     def __getattr__(self, attr):
         return getattr(self.s, attr)
 
+
 def server_socket(port):
     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+    s.bind(("", port))
+    s.listen(1)
     # set close-on-exec flag (subprocesses should not inherit it)
     set_close_on_exec(s, True)
-    s.bind(('', port))
-    s.listen(1)
     return ServerSocketWrapper(s)
 
-class TCPServer(object):
+
+class TCPServer(GenericServer):
     def __init__(self, port):
-        self.s = server_socket(port)
-        self.listener_classes = {}
+        GenericServer.__init__(self)
+        self._port = port
 
-    def join_event_loop(self, ev_loop):
-        self.ev_loop = ev_loop
-        ev_loop.register_listener(self)
-
-    # let the event loop know what we are reading on
-    def fileno(self):
-        return self.s.fileno()
-
-    def register_listener_class(self, req_id, cls, **ctor_args):
-        self.listener_classes[req_id] = dict(
-            cls = cls,
-            ctor_args = ctor_args
-        )
+    def prepare(self, ev_loop):
+        self.s = server_socket(self._port)
+        self.join_event_loop(ev_loop)
 
-    # when the event loop detects an event for us, this is 
+    # when the event loop detects an event for us, this is
     # what we will do: accept the tcp connection, read
-    # the request and create the appropriate listener, 
+    # the request and create the appropriate listener,
     # and register this listener in the event loop.
     def handle_event(self, ts):
         conn_s, addr = self.s.accept()
-        sock_file = SmartSocketFile(conn_s)
+        sock_file = RWSocketFile(conn_s)
         req_id = Requests.read_id(sock_file)
-        if req_id is None or req_id not in self.listener_classes:
-            print('Invalid request.')
-            sock_file.close()
-            return
-        # create the appropriate listener given the req_id
-        listener_info = self.listener_classes[req_id]
-        cls = listener_info['cls']
-        ctor_args = listener_info['ctor_args'].copy()
-        ctor_args.update(dict(
-                    sock_file = sock_file))
-        listener = cls(**ctor_args)
-        self.ev_loop.register_listener(listener)
-
-    def close(self):
-        self.s.close()
-
+        listener = self.get_listener(req_id, sock_file=sock_file)
+        if listener is None:
+            sock_file.close()  # failed
+        else:
+            self.ev_loop.register_listener(listener)
+        # even if there was an issue when starting this listener,
+        # the server itself should continue running
+        return True
```

### Comparing `walt-common-7/walt/common/tty.py` & `walt-common-8.0/walt/common/tty.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,29 +1,37 @@
-import os, termios, struct, fcntl, re
+import fcntl
+import os
+import re
+import struct
+import termios
+
+TTY_CONTROL_CHARS = "".join(map(chr, list(range(0, 32)) + list(range(127, 160))))
+TTY_CONTROL_CHARS_RE = re.compile("[%s]" % re.escape(TTY_CONTROL_CHARS))
 
-TTY_CONTROL_CHARS = ''.join(map(chr, list(range(0,32)) + list(range(127,160))))
-TTY_CONTROL_CHARS_RE = re.compile('[%s]' % re.escape(TTY_CONTROL_CHARS))
 
 def remove_control_chars(s):
-    return TTY_CONTROL_CHARS_RE.sub('', s)
+    return TTY_CONTROL_CHARS_RE.sub("", s)
+
 
 def set_tty_size_raw(fd, tty_size_raw):
     fcntl.ioctl(fd, termios.TIOCSWINSZ, tty_size_raw)
 
+
 def set_tty_size(fd, tty_size):
     tty_rows, tty_cols = tty_size
     packed = struct.pack("HHHH", tty_rows, tty_cols, 0, 0)
     set_tty_size_raw(fd, packed)
 
+
 def acquire_controlling_tty(tty_fd):
     # we need to be a session leader
     os.setsid()
     # just opening the file descriptor *without* the flag O_NOCTTY
     # should be enough
     ttyname = os.ttyname(tty_fd)
     os.close(os.open(ttyname, os.O_RDONLY))
 
+
 def tty_disable_echoctl(fd):
     attrs = termios.tcgetattr(fd)
     attrs[3] = attrs[3] & ~termios.ECHOCTL
     termios.tcsetattr(fd, termios.TCSADRAIN, attrs)
-
```

