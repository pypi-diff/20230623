# Comparing `tmp/pykeadhcp-0.5.0.tar.gz` & `tmp/pykeadhcp-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykeadhcp-0.5.0.tar", max compression
+gzip compressed data, was "pykeadhcp-0.5.1.tar", max compression
```

## Comparing `pykeadhcp-0.5.0.tar` & `pykeadhcp-0.5.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0    11356 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/LICENSE
--rw-r--r--   0        0        0     7331 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/README.md
--rw-r--r--   0        0        0       30 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/__init__.py
--rw-r--r--   0        0        0      174 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/daemons/__init__.py
--rw-r--r--   0        0        0     4508 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/daemons/ctrlagent.py
--rw-r--r--   0        0        0     4526 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/daemons/ddns.py
--rw-r--r--   0        0        0    25840 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/daemons/dhcp4.py
--rw-r--r--   0        0        0    22098 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/daemons/dhcp6.py
--rw-r--r--   0        0        0     2718 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/exceptions.py
--rw-r--r--   0        0        0     8243 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/kea.py
--rw-r--r--   0        0        0        0 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/__init__.py
--rw-r--r--   0        0        0        0 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/ctrlagent/__init__.py
--rw-r--r--   0        0        0      457 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/ctrlagent/config.py
--rw-r--r--   0        0        0        0 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp4/__init__.py
--rw-r--r--   0        0        0      331 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp4/client_class.py
--rw-r--r--   0        0        0      798 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp4/config.py
--rw-r--r--   0        0        0      212 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp4/lease.py
--rw-r--r--   0        0        0      303 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp4/reservation.py
--rw-r--r--   0        0        0      453 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp4/shared_network.py
--rw-r--r--   0        0        0      684 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp4/subnet.py
--rw-r--r--   0        0        0        0 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp6/__init__.py
--rw-r--r--   0        0        0      253 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp6/client_class.py
--rw-r--r--   0        0        0      922 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp6/config.py
--rw-r--r--   0        0        0      346 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp6/lease.py
--rw-r--r--   0        0        0      438 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp6/pd_pool.py
--rw-r--r--   0        0        0      212 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp6/reservation.py
--rw-r--r--   0        0        0      296 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp6/server_id.py
--rw-r--r--   0        0        0      380 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp6/shared_network.py
--rw-r--r--   0        0        0      501 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/dhcp6/subnet.py
--rw-r--r--   0        0        0     1550 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/enums.py
--rw-r--r--   0        0        0      169 2023-06-22 21:53:11.124817 pykeadhcp-0.5.0/pykeadhcp/models/generic/__init__.py
--rw-r--r--   0        0        0      181 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/api_response.py
--rw-r--r--   0        0        0      477 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/authentication.py
--rw-r--r--   0        0        0      435 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/base.py
--rw-r--r--   0        0        0      415 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/client_class.py
--rw-r--r--   0        0        0     1394 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/config.py
--rw-r--r--   0        0        0      396 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/control_socket.py
--rw-r--r--   0        0        0     2458 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/daemon.py
--rw-r--r--   0        0        0      734 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/database.py
--rw-r--r--   0        0        0      399 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/dhcp_common.py
--rw-r--r--   0        0        0      873 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/dhcp_ddns.py
--rw-r--r--   0        0        0      158 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/dhcp_queue_control.py
--rw-r--r--   0        0        0      183 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/hook.py
--rw-r--r--   0        0        0      403 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/lease.py
--rw-r--r--   0        0        0      538 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/logger.py
--rw-r--r--   0        0        0      181 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/multi_threading.py
--rw-r--r--   0        0        0      259 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/option_data.py
--rw-r--r--   0        0        0      294 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/option_def.py
--rw-r--r--   0        0        0      306 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/pool.py
--rw-r--r--   0        0        0      141 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/relay.py
--rw-r--r--   0        0        0      379 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/reservation.py
--rw-r--r--   0        0        0      112 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/sanity_check.py
--rw-r--r--   0        0        0      175 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/shared_network.py
--rw-r--r--   0        0        0      249 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/sockets.py
--rw-r--r--   0        0        0      477 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/status.py
--rw-r--r--   0        0        0      390 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/models/generic/subnet.py
--rw-r--r--   0        0        0      152 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/parsers/__init__.py
--rw-r--r--   0        0        0      508 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/parsers/ctrlagent.py
--rw-r--r--   0        0        0        0 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/parsers/ddns.py
--rw-r--r--   0        0        0    17838 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/parsers/dhcp4.py
--rw-r--r--   0        0        0    20361 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/parsers/dhcp6.py
--rw-r--r--   0        0        0     3436 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/parsers/exceptions.py
--rw-r--r--   0        0        0      825 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pykeadhcp/parsers/generic.py
--rw-r--r--   0        0        0      447 2023-06-22 21:53:11.128817 pykeadhcp-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     7936 1970-01-01 00:00:00.000000 pykeadhcp-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/LICENSE
+-rw-r--r--   0        0        0     7331 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/README.md
+-rw-r--r--   0        0        0       30 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/daemons/__init__.py
+-rw-r--r--   0        0        0     4508 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/daemons/ctrlagent.py
+-rw-r--r--   0        0        0     4526 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/daemons/ddns.py
+-rw-r--r--   0        0        0    26078 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/daemons/dhcp4.py
+-rw-r--r--   0        0        0    22336 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/daemons/dhcp6.py
+-rw-r--r--   0        0        0     2718 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/exceptions.py
+-rw-r--r--   0        0        0     8243 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/kea.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/ctrlagent/__init__.py
+-rw-r--r--   0        0        0      457 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/ctrlagent/config.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/__init__.py
+-rw-r--r--   0        0        0      331 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/client_class.py
+-rw-r--r--   0        0        0      798 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/config.py
+-rw-r--r--   0        0        0      212 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/lease.py
+-rw-r--r--   0        0        0      303 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/reservation.py
+-rw-r--r--   0        0        0      453 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/shared_network.py
+-rw-r--r--   0        0        0      684 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/subnet.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/__init__.py
+-rw-r--r--   0        0        0      253 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/client_class.py
+-rw-r--r--   0        0        0      922 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/config.py
+-rw-r--r--   0        0        0      346 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/lease.py
+-rw-r--r--   0        0        0      438 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/pd_pool.py
+-rw-r--r--   0        0        0      212 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/reservation.py
+-rw-r--r--   0        0        0      296 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/server_id.py
+-rw-r--r--   0        0        0      380 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/shared_network.py
+-rw-r--r--   0        0        0      501 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/subnet.py
+-rw-r--r--   0        0        0     1550 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/enums.py
+-rw-r--r--   0        0        0      169 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/api_response.py
+-rw-r--r--   0        0        0      477 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/authentication.py
+-rw-r--r--   0        0        0      435 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/base.py
+-rw-r--r--   0        0        0      415 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/client_class.py
+-rw-r--r--   0        0        0     1394 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/config.py
+-rw-r--r--   0        0        0      396 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/control_socket.py
+-rw-r--r--   0        0        0     2458 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/daemon.py
+-rw-r--r--   0        0        0      734 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/database.py
+-rw-r--r--   0        0        0      399 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/dhcp_common.py
+-rw-r--r--   0        0        0      873 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/dhcp_ddns.py
+-rw-r--r--   0        0        0      158 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/dhcp_queue_control.py
+-rw-r--r--   0        0        0      183 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/hook.py
+-rw-r--r--   0        0        0      403 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/lease.py
+-rw-r--r--   0        0        0      538 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/logger.py
+-rw-r--r--   0        0        0      181 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/multi_threading.py
+-rw-r--r--   0        0        0      259 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/option_data.py
+-rw-r--r--   0        0        0      294 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/option_def.py
+-rw-r--r--   0        0        0      306 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/pool.py
+-rw-r--r--   0        0        0      141 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/relay.py
+-rw-r--r--   0        0        0      379 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/reservation.py
+-rw-r--r--   0        0        0      112 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/sanity_check.py
+-rw-r--r--   0        0        0      175 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/shared_network.py
+-rw-r--r--   0        0        0      249 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/sockets.py
+-rw-r--r--   0        0        0      477 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/status.py
+-rw-r--r--   0        0        0      390 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/models/generic/subnet.py
+-rw-r--r--   0        0        0      152 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/parsers/__init__.py
+-rw-r--r--   0        0        0      508 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/parsers/ctrlagent.py
+-rw-r--r--   0        0        0        0 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/parsers/ddns.py
+-rw-r--r--   0        0        0    17838 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/parsers/dhcp4.py
+-rw-r--r--   0        0        0    20361 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/parsers/dhcp6.py
+-rw-r--r--   0        0        0     3436 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/parsers/exceptions.py
+-rw-r--r--   0        0        0      825 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pykeadhcp/parsers/generic.py
+-rw-r--r--   0        0        0      447 2023-06-23 08:50:16.307685 pykeadhcp-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     7936 1970-01-01 00:00:00.000000 pykeadhcp-0.5.1/PKG-INFO
```

### Comparing `pykeadhcp-0.5.0/LICENSE` & `pykeadhcp-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/README.md` & `pykeadhcp-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/daemons/ctrlagent.py` & `pykeadhcp-0.5.1/pykeadhcp/daemons/ctrlagent.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/daemons/ddns.py` & `pykeadhcp-0.5.1/pykeadhcp/daemons/ddns.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/daemons/dhcp4.py` & `pykeadhcp-0.5.1/pykeadhcp/daemons/dhcp4.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,20 +227,27 @@
 
         Args:
             subnets:        List of subnet IDs to fetch leases for
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease4-get-all
         """
-        data = self.api.send_command_with_arguments(
-            command="lease4-get-all",
-            service=self.service,
-            arguments={"subnets": subnets},
-            required_hook="lease_cmds",
-        )
+        if subnets:
+            data = self.api.send_command_with_arguments(
+                command="lease4-get-all",
+                service=self.service,
+                arguments={"subnets": subnets},
+                required_hook="lease_cmds",
+            )
+        else:
+            data = self.api.send_command(
+                command="lease4-get-all",
+                service=self.service,
+                required_hook="lease_cmds",
+            )
 
         if data.result == 3:
             raise KeaLeaseNotFoundException(data.text)
 
         leases = [Lease4.parse_obj(lease) for lease in data.arguments["leases"]]
         return leases
```

### Comparing `pykeadhcp-0.5.0/pykeadhcp/daemons/dhcp6.py` & `pykeadhcp-0.5.1/pykeadhcp/daemons/dhcp6.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,20 +206,27 @@
 
         Args:
             subnets:        List of subnet IDs to fetch leases for
 
         Kea API Reference:
             https://kea.readthedocs.io/en/kea-2.2.0/api.html#lease6-get-all
         """
-        data = self.api.send_command_with_arguments(
-            command="lease6-get-all",
-            service=self.service,
-            arguments={"subnets": subnets},
-            required_hook="lease_cmds",
-        )
+        if subnets:
+            data = self.api.send_command_with_arguments(
+                command="lease6-get-all",
+                service=self.service,
+                arguments={"subnets": subnets},
+                required_hook="lease_cmds",
+            )
+        else:
+            data = self.api.send_command(
+                command="lease6-get-all",
+                service=self.service,
+                required_hook="lease_cmds",
+            )
 
         if data.result == 3:
             raise KeaLeaseNotFoundException(data.text)
 
         leases = [Lease6.parse_obj(lease) for lease in data.arguments["leases"]]
         return leases
```

### Comparing `pykeadhcp-0.5.0/pykeadhcp/exceptions.py` & `pykeadhcp-0.5.1/pykeadhcp/exceptions.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/kea.py` & `pykeadhcp-0.5.1/pykeadhcp/kea.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/models/dhcp4/config.py` & `pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/config.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/models/dhcp4/subnet.py` & `pykeadhcp-0.5.1/pykeadhcp/models/dhcp4/subnet.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/models/dhcp6/config.py` & `pykeadhcp-0.5.1/pykeadhcp/models/dhcp6/config.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/models/enums.py` & `pykeadhcp-0.5.1/pykeadhcp/models/enums.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/models/generic/config.py` & `pykeadhcp-0.5.1/pykeadhcp/models/generic/config.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/models/generic/daemon.py` & `pykeadhcp-0.5.1/pykeadhcp/models/generic/daemon.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/models/generic/database.py` & `pykeadhcp-0.5.1/pykeadhcp/models/generic/database.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/models/generic/dhcp_ddns.py` & `pykeadhcp-0.5.1/pykeadhcp/models/generic/dhcp_ddns.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/models/generic/logger.py` & `pykeadhcp-0.5.1/pykeadhcp/models/generic/logger.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/parsers/dhcp4.py` & `pykeadhcp-0.5.1/pykeadhcp/parsers/dhcp4.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/parsers/dhcp6.py` & `pykeadhcp-0.5.1/pykeadhcp/parsers/dhcp6.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/parsers/exceptions.py` & `pykeadhcp-0.5.1/pykeadhcp/parsers/exceptions.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/pykeadhcp/parsers/generic.py` & `pykeadhcp-0.5.1/pykeadhcp/parsers/generic.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.5.0/PKG-INFO` & `pykeadhcp-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykeadhcp
-Version: 0.5.0
+Version: 0.5.1
 Summary: Wrapper around requests module to query ISC Kea DHCP API Daemons (ctrlagent, dhcp4, dhcp6, ddns)
 License: Apache 2.0
 Author: Brandon Spendlove
 Author-email: brandon-spendlove@hotmail.co.uk
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

