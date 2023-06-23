# Comparing `tmp/brnet-0.0.5.tar.gz` & `tmp/brnet-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brnet-0.0.5.tar", last modified: Thu Jun 22 23:46:29 2023, max compression
+gzip compressed data, was "brnet-0.0.6.tar", last modified: Fri Jun 23 00:33:21 2023, max compression
```

## Comparing `brnet-0.0.5.tar` & `brnet-0.0.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.163032 brnet-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-22 23:46:14.000000 brnet-0.0.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-22 23:46:14.000000 brnet-0.0.5/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-22 23:46:14.000000 brnet-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-22 23:46:14.000000 brnet-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-22 23:46:14.000000 brnet-0.0.5/01-phys-to-bridge
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-22 23:46:14.000000 brnet-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-22 23:46:14.000000 brnet-0.0.5/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-22 23:46:29.163032 brnet-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-22 23:46:14.000000 brnet-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-22 23:46:14.000000 brnet-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 23:46:14.000000 brnet-0.0.5/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-22 23:46:14.000000 brnet-0.0.5/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:14.000000 brnet-0.0.5/requirements/main.in
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-22 23:46:14.000000 brnet-0.0.5/requirements/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 23:46:29.163032 brnet-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/sh/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-22 23:46:14.000000 brnet-0.0.5/sh/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     5758 2023-06-22 23:46:14.000000 brnet-0.0.5/sh/brnet
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-22 23:46:14.000000 brnet-0.0.5/sh/pidp11.sh.diff
--rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-22 23:46:14.000000 brnet-0.0.5/sh/wait_for_if
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/src/brnet/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-22 23:46:14.000000 brnet-0.0.5/src/brnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-06-22 23:46:14.000000 brnet-0.0.5/src/brnet/brnet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/src/brnet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-22 23:46:29.000000 brnet-0.0.5/src/brnet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-22 23:46:29.000000 brnet-0.0.5/src/brnet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 23:46:29.000000 brnet-0.0.5/src/brnet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-22 23:46:29.000000 brnet-0.0.5/src/brnet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-22 23:46:29.000000 brnet-0.0.5/src/brnet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.159032 brnet-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:14.000000 brnet-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-22 23:46:14.000000 brnet-0.0.5/tests/object_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 23:46:29.163032 brnet-0.0.5/tests/support/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-06-22 23:46:14.000000 brnet-0.0.5/tests/support/ip
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-22 23:46:14.000000 brnet-0.0.5/tests/support/start_expected.txt
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 23:46:14.000000 brnet-0.0.5/tests/support/stop_expected.txt
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-22 23:46:14.000000 brnet-0.0.5/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-22 23:46:14.000000 brnet-0.0.5/wrapper.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:33:21.139589 brnet-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:33:21.135589 brnet-0.0.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-23 00:33:01.000000 brnet-0.0.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:33:21.135589 brnet-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-06-23 00:33:01.000000 brnet-0.0.6/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-23 00:33:01.000000 brnet-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-23 00:33:01.000000 brnet-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 00:33:01.000000 brnet-0.0.6/01-phys-to-bridge
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-23 00:33:01.000000 brnet-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-23 00:33:01.000000 brnet-0.0.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-23 00:33:21.139589 brnet-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-06-23 00:33:01.000000 brnet-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-23 00:33:01.000000 brnet-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:33:21.135589 brnet-0.0.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 00:33:01.000000 brnet-0.0.6/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-06-23 00:33:01.000000 brnet-0.0.6/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 00:33:01.000000 brnet-0.0.6/requirements/main.in
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-23 00:33:01.000000 brnet-0.0.6/requirements/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 00:33:21.139589 brnet-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:33:21.135589 brnet-0.0.6/sh/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-23 00:33:01.000000 brnet-0.0.6/sh/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5758 2023-06-23 00:33:01.000000 brnet-0.0.6/sh/brnet
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-23 00:33:01.000000 brnet-0.0.6/sh/pidp11.sh.diff
+-rwxr-xr-x   0 runner    (1001) docker     (123)      304 2023-06-23 00:33:01.000000 brnet-0.0.6/sh/wait_for_if
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:33:21.135589 brnet-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:33:21.135589 brnet-0.0.6/src/brnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-23 00:33:01.000000 brnet-0.0.6/src/brnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-06-23 00:33:01.000000 brnet-0.0.6/src/brnet/brnet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:33:21.139589 brnet-0.0.6/src/brnet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-06-23 00:33:21.000000 brnet-0.0.6/src/brnet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-23 00:33:21.000000 brnet-0.0.6/src/brnet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 00:33:21.000000 brnet-0.0.6/src/brnet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 00:33:21.000000 brnet-0.0.6/src/brnet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-23 00:33:21.000000 brnet-0.0.6/src/brnet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:33:21.139589 brnet-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 00:33:01.000000 brnet-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-23 00:33:01.000000 brnet-0.0.6/tests/object_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 00:33:21.139589 brnet-0.0.6/tests/support/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1018 2023-06-23 00:33:01.000000 brnet-0.0.6/tests/support/ip
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-23 00:33:01.000000 brnet-0.0.6/tests/support/start_expected.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-23 00:33:01.000000 brnet-0.0.6/tests/support/stop_expected.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-23 00:33:01.000000 brnet-0.0.6/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-23 00:33:01.000000 brnet-0.0.6/wrapper.sh
```

### Comparing `brnet-0.0.5/.github/workflows/ci.yaml` & `brnet-0.0.6/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `brnet-0.0.5/.gitignore` & `brnet-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `brnet-0.0.5/LICENSE` & `brnet-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `brnet-0.0.5/Makefile` & `brnet-0.0.6/Makefile`

 * *Files identical despite different names*

### Comparing `brnet-0.0.5/PKG-INFO` & `brnet-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brnet
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tool to convert ethernet interface to bridge for emulation
 License: MIT License
         
         Copyright (c) 2020-2023 Adam Thornton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `brnet-0.0.5/README.md` & `brnet-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `brnet-0.0.5/pyproject.toml` & `brnet-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `brnet-0.0.5/requirements/dev.txt` & `brnet-0.0.6/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `brnet-0.0.5/sh/README.md` & `brnet-0.0.6/sh/README.md`

 * *Files identical despite different names*

### Comparing `brnet-0.0.5/sh/brnet` & `brnet-0.0.6/sh/brnet`

 * *Files identical despite different names*

### Comparing `brnet-0.0.5/src/brnet/brnet.py` & `brnet-0.0.6/src/brnet/brnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,25 +122,25 @@
             addl += f" metric {iface['metric']}"
         return addl
 
     def _bridge_phys_if(self) -> None:
         iface = self._interfaces[self._interface]
         for cmd in [
             f"ip addr del dev {self._interface} {self._ip}",
-            f"ip link dev {self._bridge} address {iface['mac']}",
-            f"ip link dev {self._interface} master {self._bridge}",
+            f"ip link set dev {self._interface} master {self._bridge}",
             f"ip addr replace dev {self._bridge} {self._ip}",
         ]:
             self._run(cmd, check=True)
         addl = self._get_gwinfo(iface)
-        for cmd in [
-            f"ip route add default metric dev {self._bridge} {addl}",
-            f"ip route del default dev {self._interface} {addl}",
-        ]:
-            self._run(cmd)
+        if addl:
+            for cmd in [
+                f"ip route add default dev {self._bridge} {addl}",
+                f"ip route del default dev {self._interface} {addl}",
+            ]:
+                self._run(cmd)
 
     def _extract_netinfo(self, interface: str) -> None:
         cmd = f"ip --json addr show dev {interface}"
         netinfo_resp = self._run(cmd)
         if netinfo_resp.stdout:
             netinfo = json.loads(netinfo_resp.stdout.decode())
             if type(netinfo) != list or len(netinfo) != 1:
@@ -240,15 +240,15 @@
                 f"ip route add default {self._interface} {addl}",
                 f"ip route del default dev {self._bridge} {addl}",
             ]:
                 self._run(cmd)
 
     def _delete_bridge(self) -> None:
         for cmd in [
-            f"ip link dev {self._bridge} down",
+            f"ip link set dev {self._bridge} down",
             f"ip link del {self._bridge} type bridge",
         ]:
             self._run(cmd, check=True)
 
     def _start(self) -> None:
         self._extract_netinfo(self._interface)
         self._create_bridge()
```

### Comparing `brnet-0.0.5/src/brnet.egg-info/PKG-INFO` & `brnet-0.0.6/src/brnet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brnet
-Version: 0.0.5
+Version: 0.0.6
 Summary: Tool to convert ethernet interface to bridge for emulation
 License: MIT License
         
         Copyright (c) 2020-2023 Adam Thornton
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `brnet-0.0.5/src/brnet.egg-info/SOURCES.txt` & `brnet-0.0.6/src/brnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brnet-0.0.5/tests/object_test.py` & `brnet-0.0.6/tests/object_test.py`

 * *Files identical despite different names*

### Comparing `brnet-0.0.5/tests/support/ip` & `brnet-0.0.6/tests/support/ip`

 * *Files identical despite different names*

### Comparing `brnet-0.0.5/tests/support/start_expected.txt` & `brnet-0.0.6/tests/support/start_expected.txt`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {'delete': '[16, 14, 13]',*

 * * 'insert': "[(13, 'ip link set dev eth0 master br0'), (15, 'ip route add default dev br0 via "*

 * *           "10.44.45.1 metric 666')]"}*

```diff
@@ -8,13 +8,12 @@
     "ip tuntap add mode tap tap1",
     "ip link set dev tap1 master br0 up",
     "ip tuntap add mode tap tap2",
     "ip link set dev tap2 master br0 up",
     "ip tuntap add mode tap tap3",
     "ip link set dev tap3 master br0 up",
     "ip addr del dev eth0 10.44.45.2/24",
-    "ip link dev br0 address 00:de:ad:be:ef:00",
-    "ip link dev eth0 master br0",
+    "ip link set dev eth0 master br0",
     "ip addr replace dev br0 10.44.45.2/24",
-    "ip route add default metric dev br0 via 10.44.45.1 metric 666",
+    "ip route add default dev br0 via 10.44.45.1 metric 666",
     "ip route del default dev eth0 via 10.44.45.1 metric 666"
 ]
```

### Comparing `brnet-0.0.5/tests/support/stop_expected.txt` & `brnet-0.0.6/tests/support/stop_expected.txt`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8888888888888888%*

 * *Differences: {'delete': '[15]', 'insert': "[(15, 'ip link set dev br0 down')]"}*

```diff
@@ -10,10 +10,10 @@
     "ip link set dev tap3 down",
     "ip tuntap del mode tap tap3",
     "ip addr del 10.44.45.2/24 dev br0",
     "ip link set dev eth0 nomaster",
     "ip addr replace 10.44.45.2/24 dev eth0",
     "ip route add default eth0 via 10.44.45.1 metric 666",
     "ip route del default dev br0 via 10.44.45.1 metric 666",
-    "ip link dev br0 down",
+    "ip link set dev br0 down",
     "ip link del br0 type bridge"
 ]
```

### Comparing `brnet-0.0.5/tox.ini` & `brnet-0.0.6/tox.ini`

 * *Files identical despite different names*

### Comparing `brnet-0.0.5/wrapper.sh` & `brnet-0.0.6/wrapper.sh`

 * *Files identical despite different names*

