# Comparing `tmp/python-matter-server-3.5.1.tar.gz` & `tmp/python-matter-server-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-matter-server-3.5.1.tar", last modified: Mon Jun 19 13:39:41 2023, max compression
+gzip compressed data, was "python-matter-server-3.5.2.tar", last modified: Fri Jun 23 14:52:34 2023, max compression
```

## Comparing `python-matter-server-3.5.1.tar` & `python-matter-server-3.5.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.250713 python-matter-server-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-06-19 13:39:41.250713 python-matter-server-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.246713 python-matter-server-3.5.1/matter_server/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.246713 python-matter-server-3.5.1/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.246713 python-matter-server-3.5.1/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.246713 python-matter-server-3.5.1/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.246713 python-matter-server-3.5.1/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.246713 python-matter-server-3.5.1/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    25613 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.246713 python-matter-server-3.5.1/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/matter_server/server/vendor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-06-19 13:39:27.000000 python-matter-server-3.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:39:41.250713 python-matter-server-3.5.1/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-06-19 13:39:40.000000 python-matter-server-3.5.1/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-19 13:39:41.000000 python-matter-server-3.5.1/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:39:40.000000 python-matter-server-3.5.1/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-19 13:39:40.000000 python-matter-server-3.5.1/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:39:38.000000 python-matter-server-3.5.1/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-19 13:39:41.000000 python-matter-server-3.5.1/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-19 13:39:41.000000 python-matter-server-3.5.1/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-19 13:39:41.250713 python-matter-server-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.373059 python-matter-server-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-06-23 14:52:34.373059 python-matter-server-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.369059 python-matter-server-3.5.2/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.369059 python-matter-server-3.5.2/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16286 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.369059 python-matter-server-3.5.2/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13636 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.369059 python-matter-server-3.5.2/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.369059 python-matter-server-3.5.2/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9147 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.373059 python-matter-server-3.5.2/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26821 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.373059 python-matter-server-3.5.2/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-23 14:52:18.000000 python-matter-server-3.5.2/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-06-23 14:52:21.000000 python-matter-server-3.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:52:34.373059 python-matter-server-3.5.2/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13793 2023-06-23 14:52:33.000000 python-matter-server-3.5.2/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-23 14:52:34.000000 python-matter-server-3.5.2/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:52:33.000000 python-matter-server-3.5.2/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-23 14:52:33.000000 python-matter-server-3.5.2/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:52:31.000000 python-matter-server-3.5.2/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-23 14:52:34.000000 python-matter-server-3.5.2/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 14:52:34.000000 python-matter-server-3.5.2/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-23 14:52:34.373059 python-matter-server-3.5.2/setup.cfg
```

### Comparing `python-matter-server-3.5.1/LICENSE` & `python-matter-server-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/PKG-INFO` & `python-matter-server-3.5.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,122 @@
-Metadata-Version: 2.1
-Name: python-matter-server
-Version: 3.5.1
-Summary: Python Matter WebSocket Server
-Author-email: The Home Assistant Authors <hello@home-assistant.io>
-License: Apache-2.0
-Platform: any
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Home Automation
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: server
-Provides-Extra: test
-License-File: LICENSE
-
 # Python Matter Server
 
-This project implements a Matter Controller Server over WebSockets using the [official Matter (formerly CHIP) SDK](https://github.com/project-chip/connectedhomeip) as a base and provides both a server and client implementation.
-
-The goal of this project is primary to have Matter support in Home Assistant but its universal approach makes it suitable to be used in other projects too.
-
-This repository is for development only (so not for enduser support). For enabling Matter support within Home Assistant, please refer to the [Home Assistant documentation](https://www.home-assistant.io/integrations/matter/).
+This project implements a Matter Controller Server over WebSockets using the
+[official Matter (formerly CHIP) SDK](https://github.com/project-chip/connectedhomeip)
+as a base and provides both a server and client implementation.
+
+The goal of this project is primary to have Matter support in Home Assistant
+but its universal approach makes it suitable to be used in other projects too.
+
+## Support
+
+Got questions?
+
+You have several options to get them answered:
+
+  * The Home Assistant [Community Forum](https://community.home-assistant.io/).
+  * The Home Assistant [Discord Chat Server](https://discord.gg/c5DvZ4e).
+  * Join [the Reddit subreddit in /r/homeassistant](https://reddit.com/r/homeassistant).
+
+If you experience issues using Matter with Home Assistant, please open an issue
+report in the [Home Assistant Core repository](https://github.com/home-assistant/core/issues/new/choose).
+
+You may also open issues in this repository if you are absolutely sure that your
+issue is related to the Matter Server component.
+
+## Installation
+
+We strongly recommend to use Home Assistant OS along with the official Matter
+Server add-on to use Matter with Home Assistant. The Matter integration
+automatically installs the Python Matter Server add-on. Please refer to the
+[Home Assistant documentation](https://www.home-assistant.io/integrations/matter/).
+Home Assistant OS has been tested and tuned to be used with Matter and Thead,
+which makes this combination the best tested and largely worry free
+environment.
+
+If you still prefer a self-managed container installation, we do offer an
+official container image. Please keep in mind that you might experience
+communication issues with Matter devices, especially Thread based devices.
+This is mostly because the container installation uses host networking, and
+relies on the networking managed by your operating system.
+
+### Requirements to communicate with Wi-Fi/Ethernet based Thread devices
+
+Make sure your you run the container on the host network. The host network
+interface needs to be in the same network as the Android/iPhone device
+you are using for commissioning. Matter uses link-local multicast protocols
+which do not work accross different LANs or VLANs.
+
+The host network interface needs IPv6 support enabled.
+
+### Requirements to communicate with Thread devices through Thread border routers
+
+For communication through Thread border routers which are not running on the same
+host as the Matter Controller server to work, IPv6 routing needs to be properly
+working. IPv6 routing is largely setup automatically through the IPv6 Neighbor
+Discovery Protocol, specifically the Route Information Options (RIO). However,
+if IPv6 ND RIO's are processed, and processed correctly depends on the network
+management software your system is using. There may be bugs and cavats in
+processing this Route Information Options.
+
+In general, make sure the kernel option `CONFIG_IPV6_ROUTER_PREF` is enabled and
+that IPv6 forwarding is disabled (sysctl variable `net.ipv6.conf.all.forwarding`).
+If IPv6 forwarding is enabled, the Linux kernel doesn't employ reachability
+probing (RFC 4191), which can lead to longer outages (up to 30min) until
+network changes are detected.
+
+If you are using NetworkManager, make sure to use at least NetworkManager 1.42.
+Previous versions lose track of routes and stale routes can lead to unreachable
+Thread devices. All current released NetworkManager versions can't handle
+multiple routes to the same network properly. This means if you have multiple
+Thread border routers, the fallback won't work immediately (see [NetworkManager
+issue #1232](https://gitlab.freedesktop.org/NetworkManager/NetworkManager/-/issues/1232)).
+
+We currently don't have experience with systemd-networkd. It seems to have its
+own IPv6 Neighbor Discovery Protocol handling.
+
+If you don't use NetworkManager or systemd-networkd, you can use the kernel's
+IPv6 Neighbor Discovery Protocol handling.
+
+Make sure the kernel options `CONFIG_IPV6_ROUTE_INFO` is enabled and the
+following sysctl variables are set:
+
+```
+sysctl -w net.ipv6.conf.wlan0.accept_ra=1
+sysctl -w net.ipv6.conf.wlan0.accept_ra_rt_info_max_plen=64
+```
+
+If your system has IPv6 forwarding enabled (not recommended, see above), you'll
+have to use `2` for the accept_ra variable. See also the [Thread Border Router - Bidirectional IPv6 Connectivity and DNS-Based Service Discovery codelab](https://openthread.io/codelabs/openthread-border-router#6).
+
+### Running the Matter Server using container image
+
+With the following command you can run the Matter Server in a container using
+Docker. The Matter network data (fabric information) are stored in a newly
+created directory `data` in the current directory. Adjust the command to
+choose another location instead.
+
+```
+mkdir data
+docker run -d \
+  --name matter-server \
+  --restart=unless-stopped \
+  --security-opt apparmor=unconfined \
+  -v $(pwd)/data:/data \
+  -v /run/dbus:/run/dbus:ro \
+  --network=host \
+  ghcr.io/home-assistant-libs/python-matter-server:stable
+```
+
+### Running using Docker compose
+
+```sh
+docker compose up -d
+docker compose logs -f
+```
 
 NOTE: Both Matter and this implementation are in early (v1) state and features are probably missing or could be improved. See our [development notes](#development) how you can help out, with development and/or testing.
 
 ## Running the development server
 
 **For enabling Matter support within Home Assistant, please refer to the Home Assistant documentation. These instructions are for development/advanced scenarios only!**
```

### Comparing `python-matter-server-3.5.1/matter_server/client/client.py` & `python-matter-server-3.5.2/matter_server/client/client.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/matter_server/client/connection.py` & `python-matter-server-3.5.2/matter_server/client/connection.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/matter_server/client/exceptions.py` & `python-matter-server-3.5.2/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/matter_server/client/models/device_types.py` & `python-matter-server-3.5.2/matter_server/client/models/device_types.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/matter_server/client/models/node.py` & `python-matter-server-3.5.2/matter_server/client/models/node.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/matter_server/common/errors.py` & `python-matter-server-3.5.2/matter_server/common/errors.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/matter_server/common/helpers/api.py` & `python-matter-server-3.5.2/matter_server/common/helpers/api.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/matter_server/common/helpers/json.py` & `python-matter-server-3.5.2/matter_server/common/helpers/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Helpers to work with (de)serializing of json."""
 
 from base64 import b64encode
 from dataclasses import is_dataclass
 from typing import Any
 
+from chip.clusters.Attribute import ValueDecodeFailure
 from chip.clusters.Types import Nullable
+from chip.tlv import float32, uint
 import orjson
 
 from .util import dataclass_to_dict
 
 JSON_ENCODE_EXCEPTIONS = (TypeError, ValueError)
 JSON_DECODE_EXCEPTIONS = (orjson.JSONDecodeError,)
 
@@ -16,18 +18,22 @@
 def json_encoder_default(obj: Any) -> Any:
     """Convert Special objects.
 
     Hand other objects to the original method.
     """
     if getattr(obj, "do_not_serialize", None):
         return None
+    if isinstance(obj, ValueDecodeFailure):
+        return None
     if isinstance(obj, (set, tuple)):
         return list(obj)
-    if isinstance(obj, float):
+    if isinstance(obj, float32):
         return float(obj)
+    if isinstance(obj, uint):
+        return int(obj)
     if hasattr(obj, "as_dict"):
         return obj.as_dict()
     if is_dataclass(obj):
         return dataclass_to_dict(obj)
     if isinstance(obj, Nullable):
         return None
     if isinstance(obj, bytes):
```

### Comparing `python-matter-server-3.5.1/matter_server/common/helpers/util.py` & `python-matter-server-3.5.2/matter_server/common/helpers/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Utils for Matter server (and client)."""
 from __future__ import annotations
 
-from base64 import b64decode, b64encode
+from base64 import b64decode
 import binascii
 from dataclasses import MISSING, asdict, fields, is_dataclass
 from datetime import datetime
 from enum import Enum
 from functools import cache
 from importlib.metadata import PackageNotFoundError, version as pkg_version
 import logging
@@ -18,15 +18,15 @@
     Union,
     get_args,
     get_origin,
     get_type_hints,
 )
 
 from chip.clusters.ClusterObjects import ClusterAttributeDescriptor
-from chip.clusters.Types import Nullable, NullValue
+from chip.clusters.Types import Nullable
 from chip.tlv import float32, uint
 
 if TYPE_CHECKING:
     from _typeshed import DataclassInstance
 
     _T = TypeVar("_T", bound=DataclassInstance)
 
@@ -55,52 +55,25 @@
 
 def parse_attribute_path(attribute_path: str) -> tuple[int, int, int]:
     """Parse AttributePath string into endpoint_id, cluster_id, attribute_id."""
     endpoint_id_str, cluster_id_str, attribute_id_str = attribute_path.split("/")
     return (int(endpoint_id_str), int(cluster_id_str), int(attribute_id_str))
 
 
-def dataclass_to_dict(obj_in: DataclassInstance, skip_none: bool = False) -> dict:
-    """Convert dataclass instance to dict, optionally skip None values."""
-    if skip_none:
-        dict_obj = asdict(
-            obj_in, dict_factory=lambda x: {k: v for (k, v) in x if v is not None}
-        )
-    else:
-        dict_obj = asdict(obj_in)
-
-    def _convert_value(value: Any) -> Any:
-        """Do some common conversions."""
-        if isinstance(value, list):
-            return [_convert_value(x) for x in value]
-        if isinstance(value, Nullable) or value == NullValue:
-            return None
-        if isinstance(value, dict):
-            return _clean_dict(value)
-        if isinstance(value, Enum):
-            return value.value
-        if isinstance(value, bytes):
-            return b64encode(value).decode("utf-8")
-        if isinstance(value, float32):
-            return float(value)
-        if type(value) == type:
-            return f"{value.__module__}.{value.__qualname__}"
-        if isinstance(value, Exception):
-            return None
-        return value
-
-    def _clean_dict(_dict_obj: dict) -> dict:
-        _final = {}
-        for key, value in _dict_obj.items():
-            if isinstance(key, int):
-                key = str(key)
-            _final[key] = _convert_value(value)
-        return _final
+def dataclass_to_dict(obj_in: DataclassInstance) -> dict:
+    """Convert dataclass instance to dict."""
 
-    return _clean_dict(dict_obj)
+    return asdict(
+        obj_in,
+        dict_factory=lambda x: {
+            # ensure the dict key is a string
+            str(k): v
+            for (k, v) in x
+        },
+    )
 
 
 def parse_utc_timestamp(datetime_string: str) -> datetime:
     """Parse datetime from string."""
     return datetime.fromisoformat(datetime_string.replace("Z", "+00:00"))
```

### Comparing `python-matter-server-3.5.1/matter_server/common/models.py` & `python-matter-server-3.5.2/matter_server/common/models.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/matter_server/server/__main__.py` & `python-matter-server-3.5.2/matter_server/server/__main__.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/matter_server/server/client_handler.py` & `python-matter-server-3.5.2/matter_server/server/client_handler.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/matter_server/server/const.py` & `python-matter-server-3.5.2/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/matter_server/server/device_controller.py` & `python-matter-server-3.5.2/matter_server/server/device_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 from functools import partial
 import logging
 import time
 from typing import TYPE_CHECKING, Any, Callable, Coroutine, Deque, Type, TypeVar, cast
 
 from chip.ChipDeviceCtrl import CommissionableNode
 from chip.clusters import Attribute, Objects as Clusters
+from chip.clusters.Attribute import ValueDecodeFailure
 from chip.clusters.ClusterObjects import ALL_CLUSTERS, Cluster
 from chip.exceptions import ChipStackError
 
 from ..common.const import SCHEMA_VERSION
 from ..common.errors import (
     NodeCommissionFailed,
     NodeInterviewFailed,
     NodeNotExists,
     NodeNotResolving,
 )
 from ..common.helpers.api import api_command
+from ..common.helpers.json import json_dumps
 from ..common.helpers.util import (
     create_attribute_path,
     create_attribute_path_from_attribute,
     dataclass_from_dict,
 )
 from ..common.models import APICommand, EventType, MatterNodeData
 from .const import PAA_ROOT_CERTS_DIR
@@ -425,14 +427,18 @@
 
         def attribute_updated_callback(
             path: Attribute.TypedAttributePath,
             transaction: Attribute.SubscriptionTransaction,
         ) -> None:
             assert self.server.loop is not None
             new_value = transaction.GetAttribute(path)
+            # failsafe: ignore ValueDecodeErrors
+            # these are set by the SDK if parsing the value failed miserably
+            if isinstance(new_value, ValueDecodeFailure):
+                return
             node_logger.debug("Attribute updated: %s - new value: %s", path, new_value)
             attr_path = str(path.Path)
             node.attributes[attr_path] = new_value
 
             # schedule save to persistent storage
             self.server.storage.set(
                 DATA_KEY_NODES,
@@ -452,15 +458,14 @@
             data: Attribute.EventReadResult,
             transaction: Attribute.SubscriptionTransaction,
         ) -> None:
             # pylint: disable=unused-argument
             assert self.server.loop is not None
             node_logger.debug("Received node event: %s", data)
             self.event_history.append(data)
-            # TODO: This callback does not seem to fire ever or my test devices do not have events
             self.server.loop.call_soon_threadsafe(
                 self.server.signal_event, EventType.NODE_EVENT, data
             )
 
         def error_callback(
             chipError: int, transaction: Attribute.SubscriptionTransaction
         ) -> None:
@@ -623,14 +628,33 @@
                     # we are only interested in the raw values and let the client
                     # match back from the id's to the correct cluster/attribute classes
                     # attributes are stored in form of AttributePath:
                     # ENDPOINT/CLUSTER_ID/ATTRIBUTE_ID
                     attribute_path = create_attribute_path(
                         endpoint, cluster_cls.id, attr_cls.attribute_id
                     )
+                    # failsafe: ignore ValueDecodeErrors
+                    # these are set by the SDK if parsing the value failed miserably
+                    if isinstance(attr_value, ValueDecodeFailure):
+                        continue
+                    # failsafe: make sure the attribute is serializable
+                    # there is a chance we receive malformed data from the sdk
+                    # due to all magic parsing to/from TLV.
+                    # skip an attribute in that case to prevent serialization issues
+                    # of the whole node.
+                    try:
+                        json_dumps(attr_value)
+                    except TypeError as err:
+                        LOGGER.warning(
+                            "Unserializable data found - "
+                            "skip attribute %s - error details: %s",
+                            attribute_path,
+                            err,
+                        )
+                        continue
                     result[attribute_path] = attr_value
         return result
 
     async def _resolve_node(
         self, node_id: int, retries: int = 3, allow_pase: bool = False
     ) -> None:
         """Resolve a Node on the network."""
```

### Comparing `python-matter-server-3.5.1/matter_server/server/helpers/paa_certificates.py` & `python-matter-server-3.5.2/matter_server/server/helpers/paa_certificates.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/matter_server/server/server.py` & `python-matter-server-3.5.2/matter_server/server/server.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/matter_server/server/stack.py` & `python-matter-server-3.5.2/matter_server/server/stack.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/matter_server/server/storage.py` & `python-matter-server-3.5.2/matter_server/server/storage.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/matter_server/server/vendor_info.py` & `python-matter-server-3.5.2/matter_server/server/vendor_info.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.5.1/pyproject.toml` & `python-matter-server-3.5.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,65 +1,69 @@
 [build-system]
-requires = ["setuptools~=62.3", "wheel~=0.37.1"]
+requires = [
+    "setuptools~=62.3",
+    "wheel~=0.37.1",
+]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-matter-server"
-version = "3.5.1"
-license     = {text = "Apache-2.0"}
+version = "3.5.2"
 description = "Python Matter WebSocket Server"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
-    {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
+    { name = "The Home Assistant Authors", email = "hello@home-assistant.io" },
 ]
 classifiers = [
-  "Development Status :: 3 - Alpha",
-  "Intended Audience :: Developers",
-  "Environment :: Console",
-  "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
-  "Topic :: Home Automation",
+    "Development Status :: 3 - Alpha",
+    "Intended Audience :: Developers",
+    "Environment :: Console",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Home Automation",
 ]
 dependencies = [
-  "aiohttp",
-  "aiorun",
-  "coloredlogs",
-  "dacite",
-  "orjson",
-  "home-assistant-chip-clusters==2023.6.0"
+    "aiohttp",
+    "aiorun",
+    "coloredlogs",
+    "dacite",
+    "orjson",
+    "home-assistant-chip-clusters==2023.6.0",
 ]
 
+[project.license]
+text = "Apache-2.0"
+
 [project.optional-dependencies]
 server = [
-  "home-assistant-chip-core==2023.6.0",
-  "cryptography==41.0.1"
+    "home-assistant-chip-core==2023.6.0",
+    "cryptography==41.0.1",
 ]
 test = [
-  "black==23.3.0",
-  "flake8==6.0.0",
-  "flake8-docstrings==1.7.0",
-  "isort==5.12.0",
-  "mypy==1.3.0",
-  "pylint==2.17.4",
-  "pytest==7.3.2",
-  "pytest-aiohttp==1.0.4",
-  "pytest-cov==4.1.0",
+    "black==23.3.0",
+    "flake8==6.0.0",
+    "flake8-docstrings==1.7.0",
+    "isort==5.12.0",
+    "mypy==1.3.0",
+    "pylint==2.17.4",
+    "pytest==7.3.2",
+    "pytest-aiohttp==1.0.4",
+    "pytest-cov==4.1.0",
 ]
 
 [project.scripts]
 matter-server = "matter_server.server.__main__:main"
 
 [tool.codespell]
 ignore-words-list = "pase,"
 
 [tool.mypy]
 python_version = "3.10"
 check_untyped_defs = true
-#disallow_any_generics = true
 disallow_incomplete_defs = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 mypy_path = "matter_server/"
 no_implicit_optional = true
 show_error_codes = true
 warn_incomplete_stub = true
@@ -68,33 +72,38 @@
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
 ignore_missing_imports = true
 module = [
-  "aiorun",
-  "chip.*",
-  "coloredlogs",
+    "aiorun",
+    "chip.*",
+    "coloredlogs",
 ]
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.setuptools]
-platforms = ["any"]
-zip-safe  = false
+platforms = [
+    "any",
+]
+zip-safe = false
 include-package-data = true
 
 [tool.setuptools.package-data]
-matter_server = ["py.typed"]
+matter_server = [
+    "py.typed",
+]
 
 [tool.setuptools.packages.find]
-include = ["matter_server*"]
-
+include = [
+    "matter_server*",
+]
 
 [tool.pylint.BASIC]
 class-const-naming-style = "any"
 good-names = [
     "_",
     "ev",
     "ex",
@@ -104,38 +113,30 @@
     "j",
     "k",
     "Run",
     "ip",
 ]
 
 [tool.pylint."MESSAGES CONTROL"]
-# fixme - we are still a work in progress
-# too-many-instance-attributes - just because it is unavoidable
-# too-few-public-methods - just because it is unavoidable
-# too-many-arguments - just because it is unavoidable
 disable = [
     "fixme",
     "too-many-instance-attributes",
     "too-few-public-methods",
-    "too-many-arguments"
+    "too-many-arguments",
 ]
 
 [tool.isort]
-# https://github.com/PyCQA/isort/wiki/isort-Settings
 profile = "black"
-# will group `import x` and `from x import` of the same module.
 force_sort_within_sections = true
 src_paths = [
-  "matter_server/client",
-  "matter_server/common",
-  "matter_server/server",
+    "matter_server/client",
+    "matter_server/common",
+    "matter_server/server",
 ]
 known_first_party = [
     "matter_server",
     "tests",
 ]
 forced_separate = [
     "tests",
 ]
 combine_as_imports = true
-
-
```

### Comparing `python-matter-server-3.5.1/python_matter_server.egg-info/SOURCES.txt` & `python-matter-server-3.5.2/python_matter_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

