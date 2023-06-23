# Comparing `tmp/walt-server-7.tar.gz` & `tmp/walt-server-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/walt-server-7.tar", last modified: Mon Feb  1 15:17:01 2021, max compression
+gzip compressed data, was "walt-server-8.0.tar", last modified: Fri Jun 23 07:38:14 2023, max compression
```

## Comparing `walt-server-7.tar` & `walt-server-8.0.tar`

### file list

```diff
@@ -1,160 +1,196 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/
--rw-r--r--   0 root         (0) root         (0)      184 2020-09-24 12:01:14.000000 walt-server-7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      284 2021-02-01 15:17:01.000000 walt-server-7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      126 2020-09-24 12:01:14.000000 walt-server-7/README.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-02-01 15:17:01.000000 walt-server-7/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      340 2020-09-24 12:01:14.000000 walt-server-7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/sh/
--rwxr-xr-x   0 root         (0) root         (0)     1335 2021-02-01 15:15:54.000000 walt-server-7/sh/walt-image-shell-helper
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/
--rw-r--r--   0 root         (0) root         (0)      147 2020-09-24 12:01:14.000000 walt-server-7/walt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/
--rw-r--r--   0 root         (0) root         (0)      101 2020-09-24 12:01:14.000000 walt-server-7/walt/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5271 2020-09-24 12:01:14.000000 walt-server-7/walt/server/autoglob.py
--rw-r--r--   0 root         (0) root         (0)      128 2020-09-24 12:01:14.000000 walt-server-7/walt/server/conf.py
--rw-r--r--   0 root         (0) root         (0)      613 2020-09-24 12:01:14.000000 walt-server-7/walt/server/const.py
--rwxr-xr-x   0 root         (0) root         (0)     1282 2021-02-01 15:15:54.000000 walt-server-7/walt/server/daemon.py
--rwxr-xr-x   0 root         (0) root         (0)      373 2020-09-24 12:01:14.000000 walt-server-7/walt/server/dhcpevent.py
--rw-r--r--   0 root         (0) root         (0)     2112 2021-02-01 15:15:54.000000 walt-server-7/walt/server/exttools.py
--rw-r--r--   0 root         (0) root         (0)      933 2021-02-01 15:16:44.000000 walt-server-7/walt/server/info.py
--rwxr-xr-x   0 root         (0) root         (0)     4458 2020-09-24 12:01:14.000000 walt-server-7/walt/server/netconfig.py
--rwxr-xr-x   0 root         (0) root         (0)     7158 2021-02-01 15:15:54.000000 walt-server-7/walt/server/postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/setup/
--rwxr-xr-x   0 root         (0) root         (0)     1009 2020-09-24 12:01:14.000000 walt-server-7/walt/server/setup/__init__.py
--rw-r--r--   0 root         (0) root         (0)      975 2021-02-01 15:15:54.000000 walt-server-7/walt/server/setup/walt-server.service
--rw-r--r--   0 root         (0) root         (0)      627 2021-02-01 15:15:54.000000 walt-server-7/walt/server/spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/threads/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/threads/blocking/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/blocking/__init__.py
--rw-r--r--   0 root         (0) root         (0)       70 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/blocking/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/threads/blocking/devices/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/blocking/devices/__init__.py
--rw-r--r--   0 root         (0) root         (0)      417 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/blocking/devices/poe.py
--rw-r--r--   0 root         (0) root         (0)      304 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/blocking/devices/topology.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/threads/blocking/images/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/blocking/images/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14381 2020-10-26 13:18:52.000000 walt-server-7/walt/server/threads/blocking/images/clone.py
--rw-r--r--   0 root         (0) root         (0)     2603 2020-10-26 10:19:09.000000 walt-server-7/walt/server/threads/blocking/images/metadata.py
--rw-r--r--   0 root         (0) root         (0)      537 2020-10-26 13:08:27.000000 walt-server-7/walt/server/threads/blocking/images/publish.py
--rw-r--r--   0 root         (0) root         (0)     7723 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/blocking/images/search.py
--rw-r--r--   0 root         (0) root         (0)      471 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/blocking/images/squash.py
--rw-r--r--   0 root         (0) root         (0)      687 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/blocking/logs.py
--rw-r--r--   0 root         (0) root         (0)     2685 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/blocking/thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/threads/hub/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/hub/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2915 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/hub/client.py
--rw-r--r--   0 root         (0) root         (0)      837 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/hub/thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/threads/main/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/threads/main/api/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/api/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    10307 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/api/cs.py
--rwxr-xr-x   0 root         (0) root         (0)      542 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/api/ns.py
--rwxr-xr-x   0 root         (0) root         (0)      664 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/api/ss.py
--rwxr-xr-x   0 root         (0) root         (0)      680 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/api/vs.py
--rwxr-xr-x   0 root         (0) root         (0)     2137 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/apisession.py
--rw-r--r--   0 root         (0) root         (0)     2285 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/blocking.py
--rwxr-xr-x   0 root         (0) root         (0)     7651 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/db.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/threads/main/devices/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/devices/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1444 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/devices/grouper.py
--rw-r--r--   0 root         (0) root         (0)    13694 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/devices/manager.py
--rw-r--r--   0 root         (0) root         (0)    24293 2021-02-01 15:15:54.000000 walt-server-7/walt/server/threads/main/devices/topology.py
--rw-r--r--   0 root         (0) root         (0)     1261 2021-02-01 15:15:54.000000 walt-server-7/walt/server/threads/main/exports.py
--rw-r--r--   0 root         (0) root         (0)     1021 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/filesystem.py
--rwxr-xr-x   0 root         (0) root         (0)     1234 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/hub.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/threads/main/images/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/__init__.py
--rw-r--r--   0 root         (0) root         (0)      853 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/clone.py
--rw-r--r--   0 root         (0) root         (0)      762 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/duplicate.py
--rw-r--r--   0 root         (0) root         (0)     2045 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/fixowner.py
--rw-r--r--   0 root         (0) root         (0)     4220 2021-02-01 15:15:54.000000 walt-server-7/walt/server/threads/main/images/image.py
--rw-r--r--   0 root         (0) root         (0)     7599 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/manager.py
--rw-r--r--   0 root         (0) root         (0)      485 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/metadata.py
--rw-r--r--   0 root         (0) root         (0)      498 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/publish.py
--rw-r--r--   0 root         (0) root         (0)      260 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/remove.py
--rw-r--r--   0 root         (0) root         (0)      793 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/rename.py
--rw-r--r--   0 root         (0) root         (0)      253 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/search.py
--rw-r--r--   0 root         (0) root         (0)     8008 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/setup.py
--rw-r--r--   0 root         (0) root         (0)     3948 2021-02-01 15:15:54.000000 walt-server-7/walt/server/threads/main/images/shell.py
--rw-r--r--   0 root         (0) root         (0)     1852 2021-02-01 15:15:54.000000 walt-server-7/walt/server/threads/main/images/show.py
--rw-r--r--   0 root         (0) root         (0)     1592 2021-02-01 15:15:54.000000 walt-server-7/walt/server/threads/main/images/spec.py
--rw-r--r--   0 root         (0) root         (0)      913 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/squash.py
--rw-r--r--   0 root         (0) root         (0)    11000 2020-10-26 13:18:52.000000 walt-server-7/walt/server/threads/main/images/store.py
--rwxr-xr-x   0 root         (0) root         (0)       97 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/walt-cat
--rwxr-xr-x   0 root         (0) root         (0)      301 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/walt-clock-sync
--rwxr-xr-x   0 root         (0) root         (0)      100 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/walt-echo
--rwxr-xr-x   0 root         (0) root         (0)      155 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/walt-env
--rwxr-xr-x   0 root         (0) root         (0)     5749 2020-10-26 13:18:52.000000 walt-server-7/walt/server/threads/main/images/walt-init
--rwxr-xr-x   0 root         (0) root         (0)      160 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/walt-log-cat
--rwxr-xr-x   0 root         (0) root         (0)     1776 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/walt-log-echo
--rwxr-xr-x   0 root         (0) root         (0)     2430 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/walt-log-tee
--rwxr-xr-x   0 root         (0) root         (0)     1636 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/walt-net-service
--rwxr-xr-x   0 root         (0) root         (0)      424 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/walt-nfs-watchdog
--rwxr-xr-x   0 root         (0) root         (0)      565 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/walt-notify-bootup
--rwxr-xr-x   0 root         (0) root         (0)      641 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/walt-rpc
--rwxr-xr-x   0 root         (0) root         (0)       97 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/walt-tee
--rwxr-xr-x   0 root         (0) root         (0)      309 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/images/walt-timeout
--rwxr-xr-x   0 root         (0) root         (0)     2190 2020-10-23 10:53:25.000000 walt-server-7/walt/server/threads/main/interactive.py
--rw-r--r--   0 root         (0) root         (0)    15093 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/logs.py
--rw-r--r--   0 root         (0) root         (0)    13334 2021-02-01 15:15:54.000000 walt-server-7/walt/server/threads/main/mydocker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/threads/main/network/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/network/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7063 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/network/dhcpd.py
--rw-r--r--   0 root         (0) root         (0)     1276 2021-02-01 15:15:54.000000 walt-server-7/walt/server/threads/main/network/nbfs.py
--rw-r--r--   0 root         (0) root         (0)      542 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/network/netsetup.py
--rw-r--r--   0 root         (0) root         (0)     1291 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/network/nfs.py
--rwxr-xr-x   0 root         (0) root         (0)     3731 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/network/setup.py
--rw-r--r--   0 root         (0) root         (0)     2308 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/network/tftp.py
--rwxr-xr-x   0 root         (0) root         (0)     3771 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/network/tools.py
--rwxr-xr-x   0 root         (0) root         (0)      734 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/network/waltvlanconf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/threads/main/nodes/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/nodes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1278 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/nodes/clock.py
--rwxr-xr-x   0 root         (0) root         (0)     3115 2020-10-26 13:18:52.000000 walt-server-7/walt/server/threads/main/nodes/expose.py
--rw-r--r--   0 root         (0) root         (0)    14740 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/nodes/manager.py
--rw-r--r--   0 root         (0) root         (0)     4248 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/nodes/netservice.py
--rw-r--r--   0 root         (0) root         (0)     6094 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/nodes/reboot.py
--rw-r--r--   0 root         (0) root         (0)     1520 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/nodes/register.py
--rw-r--r--   0 root         (0) root         (0)     4625 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/nodes/show.py
--rw-r--r--   0 root         (0) root         (0)     1262 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/nodes/wait.py
--rwxr-xr-x   0 root         (0) root         (0)     5772 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/parallel.py
--rwxr-xr-x   0 root         (0) root         (0)    11154 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/server.py
--rw-r--r--   0 root         (0) root         (0)    16880 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/threads/main/snmp/
--rw-r--r--   0 root         (0) root         (0)       62 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/snmp/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5006 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/snmp/base.py
--rwxr-xr-x   0 root         (0) root         (0)     1432 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/snmp/ipsetup.py
--rwxr-xr-x   0 root         (0) root         (0)     3967 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/snmp/lldp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/threads/main/snmp/mibs/
--rw-r--r--   0 root         (0) root         (0)    76945 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/snmp/mibs/LLDP-MIB.mib
--rwxr-xr-x   0 root         (0) root         (0)    23641 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/snmp/mibs/NETGEAR-POWER-ETHERNET-MIB.mib
--rwxr-xr-x   0 root         (0) root         (0)     9740 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/snmp/mibs/NETGEAR-REF-MIB.mib
--rwxr-xr-x   0 root         (0) root         (0)   217031 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/snmp/mibs/NETGEAR-SWITCHING-MIB.mib
--rw-r--r--   0 root         (0) root         (0)      643 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/snmp/mibs/TPLINK-LLDP-MIB.mib
--rw-r--r--   0 root         (0) root         (0)    26808 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/snmp/mibs/TPLINK-LLDPINFO-MIB.mib
--rw-r--r--   0 root         (0) root         (0)     1101 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/snmp/mibs/TPLINK-MIB.mib
--rw-r--r--   0 root         (0) root         (0)    15894 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/snmp/mibs/TPLINK-POWER-OVER-ETHERNET-MIB.mib
--rwxr-xr-x   0 root         (0) root         (0)      768 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/snmp/mibs/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6952 2021-02-01 15:15:54.000000 walt-server-7/walt/server/threads/main/snmp/poe.py
--rwxr-xr-x   0 root         (0) root         (0)     1000 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/snmp/proxy.py
--rwxr-xr-x   0 root         (0) root         (0)     4241 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/snmp/vlan.py
--rwxr-xr-x   0 root         (0) root         (0)      120 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/status.py
--rw-r--r--   0 root         (0) root         (0)     1308 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/task.py
--rwxr-xr-x   0 root         (0) root         (0)     1314 2020-10-26 13:18:52.000000 walt-server-7/walt/server/threads/main/thread.py
--rw-r--r--   0 root         (0) root         (0)    11119 2021-02-01 15:15:54.000000 walt-server-7/walt/server/threads/main/transfer.py
--rw-r--r--   0 root         (0) root         (0)     4484 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/tree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt/server/threads/main/ui/
--rw-r--r--   0 root         (0) root         (0)        0 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/ui/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2679 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/ui/manager.py
--rw-r--r--   0 root         (0) root         (0)     1335 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/vpn-proxy-setup.sh
--rw-r--r--   0 root         (0) root         (0)     8836 2020-09-24 12:01:14.000000 walt-server-7/walt/server/threads/main/vpn.py
--rw-r--r--   0 root         (0) root         (0)     5797 2020-09-24 12:01:14.000000 walt-server-7/walt/server/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:01.000000 walt-server-7/walt_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      284 2021-02-01 15:17:01.000000 walt-server-7/walt_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5380 2021-02-01 15:17:01.000000 walt-server-7/walt_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-01 15:17:01.000000 walt-server-7/walt_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      193 2021-02-01 15:17:01.000000 walt-server-7/walt_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      170 2021-02-01 15:17:01.000000 walt-server-7/walt_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2021-02-01 15:17:01.000000 walt-server-7/walt_server.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.652602 walt-server-8.0/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-06-21 15:19:09.000000 walt-server-8.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-23 07:38:14.652602 walt-server-8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      126 2022-03-29 14:58:03.000000 walt-server-8.0/README.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 07:38:14.652602 walt-server-8.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2846 2023-06-23 07:37:56.000000 walt-server-8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.640602 walt-server-8.0/sh/
+-rwxr-xr-x   0 root         (0) root         (0)     2016 2023-06-21 15:19:09.000000 walt-server-8.0/sh/walt-image-build-helper
+-rwxr-xr-x   0 root         (0) root         (0)     1335 2022-03-29 14:58:03.000000 walt-server-8.0/sh/walt-image-shell-helper
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.640602 walt-server-8.0/walt/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-server-8.0/walt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/
+-rw-r--r--   0 root         (0) root         (0)      352 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/annotatecmd.py
+-rw-r--r--   0 root         (0) root         (0)     5567 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/autoglob.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/config.py
+-rw-r--r--   0 root         (0) root         (0)      462 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/const.py
+-rwxr-xr-x   0 root         (0) root         (0)     2319 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/daemon.py
+-rwxr-xr-x   0 root         (0) root         (0)     1510 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/dhcpevent.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/exttools.py
+-rw-r--r--   0 root         (0) root         (0)      796 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/imagecheck.py
+-rw-r--r--   0 root         (0) root         (0)     5367 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/netconfig.py
+-rw-r--r--   0 root         (0) root         (0)     4207 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/popen.py
+-rw-r--r--   0 root         (0) root         (0)    14123 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/blocking/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       98 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/blocking/devices/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/devices/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/devices/grouper.py
+-rw-r--r--   0 root         (0) root         (0)    38624 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/devices/topology.py
+-rw-r--r--   0 root         (0) root         (0)     4448 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/devices/tree.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/blocking/images/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16127 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/clone.py
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/commit.py
+-rw-r--r--   0 root         (0) root         (0)     3291 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/metadata.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/publish.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/pull.py
+-rw-r--r--   0 root         (0) root         (0)     9389 2023-06-22 13:09:04.000000 walt-server-8.0/walt/server/processes/blocking/images/search.py
+-rw-r--r--   0 root         (0) root         (0)     1286 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/squash.py
+-rw-r--r--   0 root         (0) root         (0)      168 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/images/tools.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/logs.py
+-rw-r--r--   0 root         (0) root         (0)     6320 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/process.py
+-rw-r--r--   0 root         (0) root         (0)    11616 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/registries.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/blocking/snmp/
+-rw-r--r--   0 root         (0) root         (0)      105 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5542 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/base.py
+-rwxr-xr-x   0 root         (0) root         (0)     2209 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/bridge.py
+-rwxr-xr-x   0 root         (0) root         (0)     3896 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/lldp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/
+-rw-r--r--   0 root         (0) root         (0)    76945 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/LLDP-MIB.mib
+-rwxr-xr-x   0 root         (0) root         (0)    23641 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/NETGEAR-POWER-ETHERNET-MIB.mib
+-rwxr-xr-x   0 root         (0) root         (0)     9740 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/NETGEAR-REF-MIB.mib
+-rwxr-xr-x   0 root         (0) root         (0)   217031 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/NETGEAR-SWITCHING-MIB.mib
+-rw-r--r--   0 root         (0) root         (0)      643 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-LLDP-MIB.mib
+-rw-r--r--   0 root         (0) root         (0)    26808 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-LLDPINFO-MIB.mib
+-rw-r--r--   0 root         (0) root         (0)     1101 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-MIB.mib
+-rw-r--r--   0 root         (0) root         (0)    15894 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-POWER-OVER-ETHERNET-MIB.mib
+-rwxr-xr-x   0 root         (0) root         (0)      785 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/mibs/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     7023 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/poe.py
+-rwxr-xr-x   0 root         (0) root         (0)      815 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/blocking/snmp/proxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/db/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/db/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    17762 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/db/db.py
+-rw-r--r--   0 root         (0) root         (0)     9393 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/db/postgres.py
+-rw-r--r--   0 root         (0) root         (0)      778 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/db/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.644602 walt-server-8.0/walt/server/processes/hub/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/hub/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-06-22 12:43:15.000000 walt-server-8.0/walt/server/processes/hub/client.py
+-rw-r--r--   0 root         (0) root         (0)      848 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/hub/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.648602 walt-server-8.0/walt/server/processes/main/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.648602 walt-server-8.0/walt/server/processes/main/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12263 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/api/cs.py
+-rwxr-xr-x   0 root         (0) root         (0)      354 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/api/ns.py
+-rwxr-xr-x   0 root         (0) root         (0)      666 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/api/ss.py
+-rwxr-xr-x   0 root         (0) root         (0)      682 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/api/vs.py
+-rwxr-xr-x   0 root         (0) root         (0)     2164 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/apisession.py
+-rw-r--r--   0 root         (0) root         (0)    12653 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)     3214 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/blocking.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.648602 walt-server-8.0/walt/server/processes/main/devices/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/devices/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19096 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/devices/manager.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/exports.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/filesystem.py
+-rwxr-xr-x   0 root         (0) root         (0)     1208 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/hub.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.648602 walt-server-8.0/walt/server/processes/main/images/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2140 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/build.py
+-rw-r--r--   0 root         (0) root         (0)     1424 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/clone.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/duplicate.py
+-rw-r--r--   0 root         (0) root         (0)     2145 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/fixowner.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/image.py
+-rw-r--r--   0 root         (0) root         (0)    10015 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/manager.py
+-rw-r--r--   0 root         (0) root         (0)      426 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/metadata.py
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/publish.py
+-rw-r--r--   0 root         (0) root         (0)      506 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/remove.py
+-rw-r--r--   0 root         (0) root         (0)     1076 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/rename.py
+-rw-r--r--   0 root         (0) root         (0)      324 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/search.py
+-rw-r--r--   0 root         (0) root         (0)     8061 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/setup.py
+-rw-r--r--   0 root         (0) root         (0)     4574 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/shell.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/spec.py
+-rw-r--r--   0 root         (0) root         (0)      878 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/squash.py
+-rw-r--r--   0 root         (0) root         (0)    19795 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/store.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/tabular.py
+-rwxr-xr-x   0 root         (0) root         (0)       97 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-cat
+-rwxr-xr-x   0 root         (0) root         (0)      911 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-clock-sync
+-rwxr-xr-x   0 root         (0) root         (0)      100 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-echo
+-rwxr-xr-x   0 root         (0) root         (0)      228 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-env
+-rwxr-xr-x   0 root         (0) root         (0)      768 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-fs-watchdog
+-rwxr-xr-x   0 root         (0) root         (0)     6541 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-init
+-rwxr-xr-x   0 root         (0) root         (0)      160 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-log-cat
+-rwxr-xr-x   0 root         (0) root         (0)     1776 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-log-echo
+-rwxr-xr-x   0 root         (0) root         (0)     2430 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-log-tee
+-rwxr-xr-x   0 root         (0) root         (0)     3058 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-net-service
+-rwxr-xr-x   0 root         (0) root         (0)     3202 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-notify-bootup
+-rwxr-xr-x   0 root         (0) root         (0)     1238 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-rpc
+-rwxr-xr-x   0 root         (0) root         (0)      564 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-tar-send
+-rwxr-xr-x   0 root         (0) root         (0)       97 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-tee
+-rwxr-xr-x   0 root         (0) root         (0)      314 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/images/walt-timeout
+-rwxr-xr-x   0 root         (0) root         (0)     2434 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/interactive.py
+-rw-r--r--   0 root         (0) root         (0)    20534 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/logs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.652602 walt-server-8.0/walt/server/processes/main/network/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8301 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/dhcpd.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/nbfs.py
+-rw-r--r--   0 root         (0) root         (0)     2181 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/nfs.py
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/service.py
+-rw-r--r--   0 root         (0) root         (0)  3889008 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/tftp-standby.tar.gz
+-rw-r--r--   0 root         (0) root         (0)     5908 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/tftp.py
+-rw-r--r--   0 root         (0) root         (0)    67720 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/walt-x86-undionly.kpxe
+-rwxr-xr-x   0 root         (0) root         (0)      734 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/network/waltvlanconf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.652602 walt-server-8.0/walt/server/processes/main/nodes/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/clock.py
+-rwxr-xr-x   0 root         (0) root         (0)     3075 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/expose.py
+-rw-r--r--   0 root         (0) root         (0)    15228 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/manager.py
+-rw-r--r--   0 root         (0) root         (0)     4118 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/netservice.py
+-rw-r--r--   0 root         (0) root         (0)     9314 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/powersave.py
+-rw-r--r--   0 root         (0) root         (0)     7955 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/reboot.py
+-rw-r--r--   0 root         (0) root         (0)     2619 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/register.py
+-rw-r--r--   0 root         (0) root         (0)     5106 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/show.py
+-rwxr-xr-x   0 root         (0) root         (0)     3109 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/status.py
+-rw-r--r--   0 root         (0) root         (0)     2894 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/nodes/wait.py
+-rwxr-xr-x   0 root         (0) root         (0)     5973 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/parallel.py
+-rwxr-xr-x   0 root         (0) root         (0)     1353 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/process.py
+-rw-r--r--   0 root         (0) root         (0)    10155 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/registry.py
+-rw-r--r--   0 root         (0) root         (0)    15170 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/server.py
+-rw-r--r--   0 root         (0) root         (0)    26496 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/settings.py
+-rwxr-xr-x   0 root         (0) root         (0)      120 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/status.py
+-rw-r--r--   0 root         (0) root         (0)     1390 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/task.py
+-rw-r--r--   0 root         (0) root         (0)    11797 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/transfer.py
+-rwxr-xr-x   0 root         (0) root         (0)     1687 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/unix.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/vpn-proxy-setup.sh
+-rw-r--r--   0 root         (0) root         (0)     7696 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/vpn.py
+-rw-r--r--   0 root         (0) root         (0)      839 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/processes/main/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.652602 walt-server-8.0/walt/server/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3030 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/services/httpd.py
+-rwxr-xr-x   0 root         (0) root         (0)     1233 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/services/lldpd.py
+-rwxr-xr-x   0 root         (0) root         (0)     1197 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/services/ptpd.py
+-rwxr-xr-x   0 root         (0) root         (0)     1282 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/services/snmpd.py
+-rwxr-xr-x   0 root         (0) root         (0)     1430 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/services/tftpd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.652602 walt-server-8.0/walt/server/setup/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6476 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/apt.py
+-rw-r--r--   0 root         (0) root         (0)     8222 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/conf.py
+-rw-r--r--   0 root         (0) root         (0)    33338 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/conmon.gz
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/grub.py
+-rw-r--r--   0 root         (0) root         (0)     9458 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/main.py
+-rw-r--r--   0 root         (0) root         (0)    15334 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/netconf.py
+-rw-r--r--   0 root         (0) root         (0)    12575 2023-06-22 12:34:04.000000 walt-server-8.0/walt/server/setup/ossetup.py
+-rw-r--r--   0 root         (0) root         (0)    11525 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/regconf.py
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-dhcpd.service
+-rw-r--r--   0 root         (0) root         (0)      663 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-httpd.service
+-rw-r--r--   0 root         (0) root         (0)      946 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-lldpd.service
+-rw-r--r--   0 root         (0) root         (0)      582 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-netconfig.service
+-rw-r--r--   0 root         (0) root         (0)      381 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-podman.service
+-rw-r--r--   0 root         (0) root         (0)      139 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-podman.socket
+-rw-r--r--   0 root         (0) root         (0)      948 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-ptpd.service
+-rw-r--r--   0 root         (0) root         (0)      819 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-snmpd.service
+-rw-r--r--   0 root         (0) root         (0)      754 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server-tftpd.service
+-rw-r--r--   0 root         (0) root         (0)      967 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/setup/walt-server.service
+-rw-r--r--   0 root         (0) root         (0)      619 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/spec.py
+-rw-r--r--   0 root         (0) root         (0)     7280 2023-06-21 15:19:09.000000 walt-server-8.0/walt/server/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:14.652602 walt-server-8.0/walt_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      247 2023-06-23 07:38:14.000000 walt-server-8.0/walt_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6967 2023-06-23 07:38:14.000000 walt-server-8.0/walt_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 07:38:14.000000 walt-server-8.0/walt_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      544 2023-06-23 07:38:14.000000 walt-server-8.0/walt_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      805 2023-06-23 07:38:14.000000 walt-server-8.0/walt_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 07:38:14.000000 walt-server-8.0/walt_server.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `walt-server-7/sh/walt-image-shell-helper` & `walt-server-8.0/sh/walt-image-shell-helper`

 * *Files identical despite different names*

### Comparing `walt-server-7/walt/server/autoglob.py` & `walt-server-8.0/walt/server/autoglob.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,132 +1,159 @@
 from collections import defaultdict
+from functools import cache
 
 # Sample use:
 #
 # >>> from autoglob import autoglob
 # >>> words = [ 'rpi-b', 'rpi-2-b', 'rpi-3-b', 'qemu-arm', 'pc-x86-64', 'pc-x86-32' ]
 # >>> print(autoglob(words))
 # rpi-[b,2-b,3-b],qemu-arm,pc-x86-[64,32]
 # >>>
 #
 # The algorithm is not perfect but should be enough when doing prefix match.
 
+
 class State:
     def __init__(self, graph, name):
         self.graph = graph
         self.name = name
         self.routes = {}
         self.ref_count = 0
+
     def next(self, transition):
         return self.routes[transition]
+
     def is_used(self):
-        return self.ref_count > 0 or self.name == '__START__'
+        return self.ref_count > 0 or self.name == "__START__"
+
     def simplify(self):
-        if self.name == '__START__':
+        if self.name == "__START__":
             return False
         if len(self.routes) == 0:
             return False
         target_states = set(self.routes.values())
         if len(target_states) > 1:
             return False
         target_state = target_states.pop()
-        if target_state.name == '__END__':
+        if target_state.name == "__END__":
             return False
         for transition in list(self.routes.keys()):
             next_transition = self.graph.next_transitions[transition]
             self.routes[transition] = target_state.routes[next_transition]
             del target_state.routes[next_transition]
             target_state.ref_count -= 1
-            next_next_transition = self.graph.next_transitions.get(next_transition, None)
+            next_next_transition = self.graph.next_transitions.get(
+                next_transition, None
+            )
             if next_next_transition is None:
                 del self.graph.next_transitions[transition]
             else:
                 self.graph.next_transitions[transition] = next_next_transition
                 del self.graph.next_transitions[next_transition]
         self.name += target_state.name
         return True
-    def autoglob(self, current_transitions = None):
-        if self.name == '__END__':
-            return ''
+
+    def autoglob(self, current_transitions=None):
+        if self.name == "__END__":
+            return ""
         if current_transitions is None:
             current_transitions = tuple(self.routes.keys())
         selected_targets = defaultdict(set)
         for transition, target_state in self.routes.items():
             if transition not in current_transitions:
                 continue
             selected_targets[target_state].add(transition)
         target_globs = []
         for target_state, transitions in selected_targets.items():
-            target_transitions = tuple( \
-                    self.graph.next_transitions.get(transition) for transition in transitions)
+            target_transitions = tuple(
+                self.graph.next_transitions.get(transition)
+                for transition in transitions
+            )
             target_globs.append(target_state.autoglob(target_transitions))
-        if self.name == '__START__':
-            return ','.join(target_globs)
+        if self.name == "__START__":
+            return ",".join(target_globs)
         # if target_globs are <value> and <empty> this means that <value> is optional
         # in this case just return [<value>] and not [|<value>]
-        if len(target_globs) == 2 and '' in target_globs:
+        if len(target_globs) == 2 and "" in target_globs:
             optional_value = True
-            target_globs_option1 = [ tglob for tglob in target_globs if tglob != '' ]
+            target_globs_option1 = [tglob for tglob in target_globs if tglob != ""]
         else:
             optional_value = False
             target_globs_option1 = target_globs
-        option1 = self.name + '[' + '|'.join(target_globs_option1) + ']'
-        option2 = ','.join((self.name + tglob) for tglob in target_globs)
+        option1 = self.name + "[" + "|".join(target_globs_option1) + "]"
+        option2 = ",".join((self.name + tglob) for tglob in target_globs)
         if len(option1) < len(option2):
             return option1
         elif len(option1) > len(option2):
             return option2
-        elif optional_value:    # same length, but optional value notation may be more readable
+        elif optional_value:  # same length, but optional value notation may be
+            # more readable
             return option1
-        else:                   # same length, so keep it simple and repeat prefix
+        else:  # same length, so keep it simple and repeat prefix
             return option2
+
     def __str__(self):
         lines = [self.name]
         for transition, state in self.routes.items():
-            lines.append(' %d -> %s' % (transition, state.name))
-        lines += ['']
-        return '\n'.join(lines)
+            lines.append(" %d -> %s" % (transition, state.name))
+        lines += [""]
+        return "\n".join(lines)
+
 
 class HyperGraph:
     def __init__(self):
         self.states = None
         self.next_transitions = None
+
     def register_state(self, state_name):
         state = State(self, state_name)
         self.states[state_name] = state
         return state
+
     def construct(self, words):
         self.states = {}
         self.next_transitions = {}
-        self.start_state = self.register_state('__START__')
+        prev_state = None
+        self.start_state = self.register_state("__START__")
         transition = 0
         for word in words:
-            spelled = ['__START__'] + list(word) + ['__END__']
+            spelled = ["__START__"] + list(word) + ["__END__"]
             for state_name in spelled:
                 if state_name not in self.states:
                     self.register_state(state_name)
                 state = self.states[state_name]
-                if state_name != '__START__':
+                if state_name != "__START__":
+                    assert prev_state is not None
                     prev_state.routes[transition] = state
-                    self.next_transitions[transition-1] = transition
+                    self.next_transitions[transition - 1] = transition
                     state.ref_count += 1
                 prev_state = state
                 transition += 1
+
     def simplify(self):
         while True:
             changed = False
             for state_name, state in list(self.states.items()):
                 if not state.is_used():
                     del self.states[state_name]
                     changed = True
                 if state.simplify():
                     changed = True
             if not changed:
                 break
+
     def autoglob(self):
         return self.start_state.autoglob()
 
-def autoglob(words):
+
+@cache
+def autoglob_with_cache(words):
     graph = HyperGraph()
     graph.construct(words)
     graph.simplify()
     return graph.autoglob()
+
+
+def autoglob(words):
+    if len(words) == 1:
+        return words[0]
+    return autoglob_with_cache(tuple(words))
```

### Comparing `walt-server-7/walt/server/netconfig.py` & `walt-server-8.0/walt/server/netconfig.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,135 +1,167 @@
-import os, sys, os.path
-import random
-from walt.common.tools import do, failsafe_makedirs
+import os
+import os.path
+import sys
+import time
+
+from walt.common.tools import do, failsafe_makedirs, get_persistent_random_mac, succeeds
 from walt.server import conf
 
-WALT_STATUS_DIR  = '/var/lib/walt'
-IFACE_STATE_FILE = WALT_STATUS_DIR + '/.%(iface)s.state'
-IFACE_MAC_FILE   = WALT_STATUS_DIR + '/.%(iface)s.mac'
-DOT1Q_FILTER     = '''\
+WALT_STATUS_DIR = "/var/lib/walt"
+IFACE_STATE_FILE = WALT_STATUS_DIR + "/.%(iface)s.state"
+IFACE_MAC_FILE = WALT_STATUS_DIR + "/.%(iface)s.mac"
+DOT1Q_FILTER = """\
 ebtables -t filter -A FORWARD -p 802_1Q \
-    -i %(src)s -o %(dst)s -j DROP'''
-
-def generate_random_mac():
-    return [ 0x52, 0x54, 0x00,
-            random.randint(0x00, 0x7f),
-            random.randint(0x00, 0xff),
-            random.randint(0x00, 0xff) ]
+    -i %(src)s -o %(dst)s -j DROP"""
+WAIT_INTERFACE_DELAY = 10  # seconds
 
-def get_random_mac():
-    return ':'.join(["%02x" % x for x in generate_random_mac()])
 
 def filter_out_8021q(iface_src, iface_dst):
     do(DOT1Q_FILTER % dict(src=iface_src, dst=iface_dst))
 
+
 def get_state_file(iface):
     return IFACE_STATE_FILE % dict(iface=iface)
 
+
 def open_state_file(iface, mode):
     return open(get_state_file(iface), mode)
 
+
 def remove_state_file(iface):
     os.remove(get_state_file(iface))
 
+
 def get_mac_file(iface):
     return IFACE_MAC_FILE % dict(iface=iface)
 
-def open_mac_file(iface, mode):
-    return open(get_mac_file(iface),mode)
 
 def remove_mac_file(iface):
     os.remove(get_mac_file(iface))
 
+
 def get_vlan(iface_conf):
-    if 'vlan' in iface_conf:
-        return iface_conf['vlan']
-    else:
-        return None
+    return iface_conf.get("vlan", None)
+
+
+def get_raw_iface(iface_conf):
+    return iface_conf.get("raw-device", None)
+
 
 def set_iface_up(iface):
-    do('ip link set up dev %s' % iface)
+    do("ip link set up dev %s" % iface)
+
 
 def create_dummy_iface(iface, state_file):
-    do('ip link add %s type dummy' % iface)
+    do("ip link add %s type dummy" % iface)
     set_iface_up(iface)
-    state_file.write(iface + '\n')
+    state_file.write(iface + "\n")
+
 
 def create_vlan_iface(raw_iface, vlan, vlan_iface, state_file):
-    do('ip link add link %s name %s type vlan id %d' % \
-        (raw_iface, vlan_iface, vlan))
+    do("ip link add link %s name %s type vlan id %d" % (raw_iface, vlan_iface, vlan))
     set_iface_up(vlan_iface)
-    state_file.write(vlan_iface + '\n')
+    state_file.write(vlan_iface + "\n")
+
 
 def create_bridge_iface(br_iface, interfaces, state_file):
-    do('ip link add %s type bridge' % br_iface)
-    if os.path.exists(get_mac_file(br_iface)):
-        with open_mac_file(br_iface, 'r') as mac_file:
-            mac = mac_file.readline()
-    else:
-        mac = get_random_mac()
-        with open_mac_file(br_iface, 'w') as mac_file:
-            mac_file.write(mac + '\n')
-            mac_file.flush()
-    do('ip link set dev %s address %s' % (br_iface, mac))
+    mac = get_persistent_random_mac(get_mac_file(br_iface))
+    do(f"ip link add {br_iface} address {mac} type bridge")
     for iface in interfaces:
-        do('ip link set dev %s master %s' % (iface, br_iface))
+        do("ip link set dev %s master %s" % (iface, br_iface))
     set_iface_up(br_iface)
-    state_file.write(br_iface + '\n')
+    state_file.write(br_iface + "\n")
+
 
 def setup_native_conf(raw_iface, iface, state_file):
-    create_bridge_iface(iface, (raw_iface,), state_file)
-    # isc-dhcp-server reads packets in raw mode on its interface
-    # thus it detects 8021q (VLAN-tagged) packets it should not see.
-    # In order to work around this issue we do not let 8021q
-    # packets cross the bridge and reach our interface.
-    filter_out_8021q(raw_iface, iface)
+    if raw_iface is None:
+        # we cannot set a bridge interface up if no interface is
+        # linked to it. so we create a dummy interface device to
+        # fix this.
+        dummy_iface = f"{iface}-dummy"
+        create_dummy_iface(dummy_iface, state_file)
+        create_bridge_iface(iface, (dummy_iface,), state_file)
+    else:
+        create_bridge_iface(iface, (raw_iface,), state_file)
+        # isc-dhcp-server reads packets in raw mode on its interface
+        # thus it detects 8021q (VLAN-tagged) packets it should not see.
+        # In order to work around this issue we do not let 8021q
+        # packets cross the bridge and reach our interface.
+        filter_out_8021q(raw_iface, iface)
+
 
 def setup_vlan_conf(raw_iface, vlan, iface, state_file):
-    vlan_iface = raw_iface + '.' + str(vlan)
+    vlan_iface = raw_iface + "." + str(vlan)
     create_vlan_iface(raw_iface, vlan, vlan_iface, state_file)
     create_bridge_iface(iface, (vlan_iface,), state_file)
 
+
 def setup_ip_conf(iface, ip_conf):
-    if ip_conf == 'dhcp':
-        do('dhclient %s' % iface)
+    if ip_conf == "dhcp":
+        do("dhclient %s" % iface)
     else:
-        do('ip addr add %s dev %s' % (
-                ip_conf, iface))
+        do("ip addr add %s dev %s" % (ip_conf, iface))
+
 
-def up(iface, network_conf):
-    with open_state_file(iface, 'w') as state_file:
-        if iface in network_conf:
-            iface_conf = network_conf[iface]
-            raw_iface = iface_conf['raw-device']
+def up(iface, iface_conf):
+    raw_iface = get_raw_iface(iface_conf)
+    vlan = get_vlan(iface_conf)
+    if raw_iface is None and vlan is not None:
+        sys.exit(f'{iface} has wrong configuration: "vlan" but no "raw-device".')
+    if raw_iface is not None:
+        # If the machine is booting, we may be here before the network interface
+        # card effectively appears.  Wait for it a little here.
+        if not succeeds("ip link show dev %s" % raw_iface):
+            print("Interface %s not found, waiting for it to appear…" % raw_iface)
+            time.sleep(WAIT_INTERFACE_DELAY)
+            if not succeeds("ip link show dev %s" % raw_iface):
+                # Here, it is really an error.  Interface should exist.
+                raise RuntimeError("Interface %s does not exist" % raw_iface)
+    with open_state_file(iface, "w") as state_file:
+        if raw_iface is not None:
             set_iface_up(raw_iface)
-            vlan = get_vlan(iface_conf)
-            if vlan:
-                setup_vlan_conf(raw_iface, vlan, iface, state_file)
-            else:
-                setup_native_conf(raw_iface, iface, state_file)
-            if 'ip' in iface_conf:
-                setup_ip_conf(iface, iface_conf['ip'])
+        if vlan:
+            setup_vlan_conf(raw_iface, vlan, iface, state_file)
+        else:
+            setup_native_conf(raw_iface, iface, state_file)
+        if "ip" in iface_conf:
+            setup_ip_conf(iface, iface_conf["ip"])
+
 
 def down(iface):
-    with open_state_file(iface, 'r') as state_file:
+    with open_state_file(iface, "r") as state_file:
         for line in state_file.readlines():
             sub_iface = line.strip()
-            do('ip link del dev %s' % sub_iface)
+            do("ip link del dev %s" % sub_iface)
     remove_state_file(iface)
 
+
 def run():
+    # Handle argument
     if len(sys.argv) < 2:
         sys.exit('Missing 1st argument: "up" or "down".')
     action = sys.argv[1]
-    if action not in ('up', 'down'):
+    if action not in ("up", "down"):
         sys.exit('1st argument must be "up" or "down".')
-    iface = os.environ.get('IFACE')
-    if iface is None:
-        sys.exit('IFACE environment variable is missing.')
+    # Handle IFACE environment variable
+    iface = os.environ.get("IFACE")
+    if iface is not None:
+        print(f"Using interface {iface} from environment variable IFACE.")
+        try:
+            iface_conf = conf["network"][iface]
+        except LookupError:
+            sys.exit(f"{iface}: interface is not listed in configuration file.")
+        network_confs = {iface: iface_conf}
+    else:
+        # Activate all interfaces
+        network_confs = conf["network"]
+    # Do the job
     failsafe_makedirs(WALT_STATUS_DIR)
-    if action == 'up':
-        network_conf = conf['network']
-        up(iface, network_conf)
-    elif action == 'down':
-        down(iface)
+    for iface, iface_conf in network_confs.items():
+        if action == "up":
+            up(iface, iface_conf)
+        elif action == "down":
+            down(iface)
+
 
+if __name__ == "__main__":
+    run()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `walt-server-7/walt/server/postgres.py` & `walt-server-8.0/walt/server/processes/db/postgres.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,67 +1,114 @@
-#!/usr/bin/env python
+import shlex
+import uuid
+from subprocess import PIPE, Popen
+from sys import stderr
 
-from walt.server.const import WALT_DBNAME, WALT_DBUSER
-from walt.server.tools import columnate
-import psycopg2, shlex, uuid
+import psycopg2
 from psycopg2.extras import NamedTupleCursor
-from subprocess import Popen, PIPE
-from sys import stderr
+from walt.common.formatting import columnate
+from walt.server.const import WALT_DBNAME, WALT_DBUSER
+from walt.server.tools import SerializableNT, build_named_tuple_cls
+
+
+# we wrap database record objects otherwise they cannot be pickled
+class DBRecord(SerializableNT):
+    pass
+
+
+class DBRecordSet:
+    def __init__(self, records=None):
+        self.records = records
 
-class PostgresDB():
+    def __getstate__(self):
+        return [row._asdict() for row in self.records]
 
+    def __setstate__(self, dict_records):
+        if len(dict_records) == 0:
+            self.records = []
+        else:
+            nt_cls = build_named_tuple_cls(dict_records[0])
+            self.records = [nt_cls(**row) for row in dict_records]
+
+    def __iter__(self):
+        return iter(self.records)
+
+    def __len__(self):
+        return len(self.records)
+
+    def __getitem__(self, i):
+        return self.records[i]
+
+
+class PostgresDB:
     def __init__(self):
-        self.conn = None
-        while self.conn == None:
-            try:
-                self.conn = psycopg2.connect(
-                        database=WALT_DBNAME, user=WALT_DBUSER)
-            except psycopg2.OperationalError:
-                self.create_db_and_user()
-        # allow name-based access to columns
-        self.c = self.conn.cursor(cursor_factory = NamedTupleCursor)
+        self.conn, self.c = None, None
         self.server_cursors = {}
         self.schema_cache = {}
 
+    def prepare(self):
+        try:
+            # Do catch exception here to create DB and users if there does not exist
+            self.conn = psycopg2.connect(database=WALT_DBNAME, user=WALT_DBUSER)
+        except psycopg2.OperationalError:
+            self.create_db_and_user()
+            # Do not catch any exception here to let the user know if something
+            # happens bad
+            self.conn = psycopg2.connect(database=WALT_DBNAME, user=WALT_DBUSER)
+        # allow name-based access to columns
+        self.c = self.conn.cursor(cursor_factory=NamedTupleCursor)
+
     def __del__(self):
-        self.conn.commit()
-        self.c.close()
-        self.conn.close()
+        if self.conn is not None:
+            self.conn.commit()
+            self.c.close()
+            self.conn.close()
+            self.conn, self.c = None, None
 
     def create_db_and_user(self):
         # we must use the postgres admin user for this
-        args = shlex.split('su -c psql -l postgres')
+        args = shlex.split("su -c psql -l postgres")
         popen = Popen(args, stdin=PIPE, stdout=None, stderr=stderr)
-        popen.stdin.write(('''
+        popen.stdin.write(("""
                 CREATE USER %(user)s;
                 ALTER ROLE %(user)s WITH CREATEDB;
                 CREATE DATABASE %(db)s OWNER %(user)s;
-                ''' % dict(user=WALT_DBUSER, db=WALT_DBNAME)).encode('ascii'))
+                """ % dict(user=WALT_DBUSER, db=WALT_DBNAME)).encode("ascii"))
         popen.stdin.close()
         popen.wait()
 
     def commit(self):
         self.conn.commit()
 
-    def execute(self, query, query_args = None):
+    def execute(self, query, query_args=None):
         self.c.execute(query, query_args)
-        return self.c
+        if self.c.description is None:  # it was not a select query
+            return None
+        return DBRecordSet(self.c.fetchall())
 
     # with server cursors, the resultset is not sent all at once to the client.
-    def create_server_cursor(self):
+    def create_server_cursor(self, sql, args):
         name = str(uuid.uuid4())
         # we share a database connection, thus we have to create a cursor
-        # WITH HOLD, otherwise any other thread issuing a commit would
+        # WITH HOLD, otherwise any other process issuing a commit would
         # cause the cursor to be discarded.
-        self.server_cursors[name] = self.conn.cursor(
-                                        name = name,
-                                        cursor_factory = NamedTupleCursor,
-                                        withhold = True)
+        cursor = self.conn.cursor(
+            name=name, cursor_factory=NamedTupleCursor, withhold=True
+        )
+        cursor.execute(sql, args)
+        self.server_cursors[name] = cursor
         return name
 
+    def step_server_cursor(self, name):
+        row = self.server_cursors[name].fetchone()
+        if row is None:
+            return None
+        else:
+            return DBRecord(row)
+
     def delete_server_cursor(self, name):
         self.server_cursors[name].close()
         del self.server_cursors[name]
 
     def get_column_names(self, table):
         res = self.schema_cache.get(table)
         if res is None:
@@ -70,118 +117,140 @@
             self.schema_cache[table] = res
         return res
 
     # from a dictionary of the form <col_name> -> <value>
     # we want to filter-out keys that are not column names,
     # and return ([<col_name>, ...], [<value>, ...]).
     def get_cols_and_values(self, table, dictionary):
-        # retrieve fields names for this table 
+        # retrieve fields names for this table
         col_names = set(self.get_column_names(table))
         res = {}
         for k in dictionary:
-            # filter-out keys of dictionary that are not 
+            # filter-out keys of dictionary that are not
             # a column name
             if k not in col_names:
                 continue
             # store in the result dict
             res[k] = dictionary[k]
         # we prefer a tuple ([k,...],[v,...]) instead of
         # a dictionary, because in an insert query,
-        # we need a list of keys and a list of values 
+        # we need a list of keys and a list of values
         # with the same ordering.
         items = list(res.items())
-        return (list(t[0] for t in items),
-                list(t[1] for t in items))
+        return (list(t[0] for t in items), list(t[1] for t in items))
 
     # format a where clause with ANDs on the specified constraints
     def get_where_clause_from_constraints(self, constraints):
         if len(constraints) > 0:
-            return "WHERE %s" % (' AND '.join(constraints));
+            return "WHERE %s" % " AND ".join(constraints)
         else:
             return ""
 
     # format a where clause with ANDs on the specified columns
     def get_where_clause_pattern(self, cols):
-        constraints = [ "%s=%%s" % col for col in cols ]
+        constraints = ["%s=%%s" % col for col in cols]
         return self.get_where_clause_from_constraints(constraints)
 
+    def get_insert_cols_and_values(self, table, rows_kwargs):
+        values_formats = []
+        all_values = []
+        for kwargs in rows_kwargs:
+            cols, values = self.get_cols_and_values(table, kwargs)
+            values_format = "(" + ",".join(["%s"] * len(values)) + ")"
+            values_formats.append(values_format)
+            all_values.extend(values)
+        return ",".join(cols), ",".join(values_formats), tuple(all_values)
+
     # allow statements like:
     # db.insert("network", ip=ip, switch_ip=swip)
     def insert(self, table, returning=None, **kwargs):
-        # insert and return True or return False
-        cols, values = self.get_cols_and_values(table, kwargs)
+        return self.insert_multiple(table, [kwargs], returning=returning)
+
+    # insert multiple rows at once
+    def insert_multiple(
+        self, table, rows_kwargs, returning=None, bypass_conflicting=False
+    ):
+        cols, formats, values = self.get_insert_cols_and_values(table, rows_kwargs)
         sql = """INSERT INTO %s(%s)
-                VALUES (%s)""" % (
-                    table,
-                    ','.join(cols),
-                    ','.join(['%s'] * len(values)))
+                VALUES %s""" % (
+            table,
+            cols,
+            formats,
+        )
+        if bypass_conflicting:
+            sql += " ON CONFLICT DO NOTHING"
         if returning:
             sql += " RETURNING %s" % returning
-        self.c.execute(sql + ';', tuple(values))
+        self.c.execute(sql + ";", values)
         if returning:
             return self.c.fetchone()[0]
 
     # allow statements like:
     # db.delete("topology", switch_mac=swmac, switch_port=swport)
     def delete(self, table, **kwargs):
+        """Delete entries from a table matching given fields"""
         cols, values = self.get_cols_and_values(table, kwargs)
         where_clause = self.get_where_clause_pattern(cols)
         sql = "DELETE FROM %s %s;" % (table, where_clause)
         self.c.execute(sql, values)
         return self.c.rowcount  # number of rows deleted
 
     # allow statements like:
     # db.update("topology", "mac", switch_mac=swmac, switch_port=swport)
     def update(self, table, primary_key_name, **kwargs):
         cols, values = self.get_cols_and_values(table, kwargs)
-        if len(cols) > 1:   # if updating at least one field (pk counts as 1 in cols)
+        if len(cols) > 1:  # if updating at least one field (pk counts as 1 in cols)
             values.append(kwargs[primary_key_name])
-            self.c.execute("""
-                UPDATE %s 
+            self.c.execute(
+                """
+                UPDATE %s
                 SET %s
-                WHERE %s = %%s;""" % (
-                    table,
-                    ','.join("%s = %%s" % col for col in cols),
-                    primary_key_name),
-                    values)
+                WHERE %s = %%s;"""
+                % (table, ",".join("%s = %%s" % col for col in cols), primary_key_name),
+                values,
+            )
             return self.c.rowcount  # number of rows updated
         else:
             return 0
 
+    # caution when calling select_no_fetch() not to let the
+    # returned cursor leave db process
     def select_no_fetch(self, table, **kwargs):
         cols, values = self.get_cols_and_values(table, kwargs)
         where_clause = self.get_where_clause_pattern(cols)
         sql = "SELECT * FROM %s %s;" % (table, where_clause)
         self.c.execute(sql, values)
         return self.c
 
     # allow statements like:
     # mem_db.select("network", ip=ip)
     def select(self, table, **kwargs):
-        try:
-            return self.select_no_fetch(table, **kwargs).fetchall()
-        except psycopg2.ProgrammingError:
-            # workaround psycopg sometimes issuing a "no results to fetch" error
-            return []
+        return DBRecordSet(self.select_no_fetch(table, **kwargs).fetchall())
 
     # same as above but expect only one matching record
     # and return it.
     def select_unique(self, table, **kwargs):
         record_list = self.select(table, **kwargs)
         if len(record_list) == 0:
             return None
         else:
-            return record_list[0]
+            return DBRecord(record_list[0])
 
     def pretty_printed_table(self, table):
         return self.pretty_printed_select("select * from %s;" % table)
 
     def pretty_printed_select(self, *args):
-        self.execute(*args)
+        self.c.execute(*args)
         col_names = [col_desc[0] for col_desc in self.c.description]
         return columnate(self.c.fetchall(), header=col_names)
 
+    def pretty_print_select_info(self, *args):
+        self.c.execute(*args)
+        col_names = [col_desc[0] for col_desc in self.c.description]
+        return DBRecordSet(self.c.fetchall()), col_names
+
     def pretty_printed_resultset(self, res):
         if len(res) == 0:
-            raise Exception('pretty_printed_resultset() does not work if resultset is empty!')
+            raise Exception(
+                "pretty_printed_resultset() does not work if resultset is empty!"
+            )
         return columnate(res, header=res[0]._fields)
-
```

### Comparing `walt-server-7/walt/server/setup/walt-server.service` & `walt-server-8.0/walt/server/setup/walt-server.service`

 * *Files 24% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 #
 # The WalT platform provides a lightweight distributed testbed for
 # sensor networks, distributed protocols, distributed data
 # management.
 
 [Unit]
 Description=WalT server daemon
+Requires=walt-server-netconfig.service
+After=walt-server-netconfig.service
 # needs lldp
-Requires=lldpd.service
-After=lldpd.service
-# needs ptpd, but we must be initialized (ip on walt-net)
-# otherwise ptpd will fail to start (thus the 'Before=',
-# and the 'Type=notify' below).
-Wants=ptpd.service
-Before=ptpd.service
+Wants=walt-server-lldpd.service
+# we need a configuration file
+ConditionPathExists=/etc/walt/server.conf
 
 [Service]
 Environment=PYTHONUNBUFFERED=1
 # After the initialization phase, we will notify systemd
 # that we are started successfully.
 Type=notify
 NotifyAccess=all
 # no startup timeout, because it can take a long time
 # if the user is installing the platform.
-TimeoutStartSec=0
+TimeoutStartSec=infinity
+RuntimeDirectory=walt/daemon
+StateDirectory=walt
 EnvironmentFile=-/etc/default/walt-server
 EnvironmentFile=-/etc/sysconfig/walt-server
-ExecStart=/usr/local/bin/walt-server-daemon $DAEMON_ARGS
+ExecStart=walt-server-daemon $DAEMON_ARGS
 ExecReload=kill -HUP $MAINPID
 Restart=on-failure
 
 [Install]
 WantedBy=multi-user.target
```

### Comparing `walt-server-7/walt/server/spec.py` & `walt-server-8.0/walt/server/spec.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,29 @@
-from walt.common.tools import read_json
+from pathlib import Path
 
-SERVER_SPEC_PATH = '/etc/walt/server.spec'
+from walt.common.config import load_conf
+
+SERVER_SPEC_PATH = Path("/etc/walt/server.spec")
 SERVER_SPEC = None
 
+
 def get_server_spec():
     global SERVER_SPEC
     if SERVER_SPEC is None:
-        try:
-            SERVER_SPEC = read_json(SERVER_SPEC_PATH)
-        except:
-            sys.stderr.write('Failed to parse /etc/walt/server.spec (should be json).')
+        SERVER_SPEC = load_conf(SERVER_SPEC_PATH, optional=True)
+        if SERVER_SPEC is None:
+            SERVER_SPEC = {}
     return SERVER_SPEC
 
+
 def reload_server_spec():
     global SERVER_SPEC
     SERVER_SPEC = None
     get_server_spec()
 
+
 def get_server_features():
-    return set(get_server_spec().get('features', []))
+    return set(get_server_spec().get("features", []))
+
 
 def server_has_feature(feature):
     return feature in get_server_features()
```

### Comparing `walt-server-7/walt/server/threads/blocking/images/clone.py` & `walt-server-8.0/walt/server/processes/blocking/images/clone.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,336 +1,473 @@
-import requests, uuid
-from walt.server.threads.blocking.images.search import \
-        LOCATION_WALT_SERVER, LOCATION_DOCKER_HUB, LOCATION_DOCKER_DAEMON, \
-        LOCATION_LABEL, LOCATION_PER_LABEL
-from walt.server.threads.blocking.images.metadata import \
-            pull_user_metadata
-from walt.common.tools import format_sentence
+from __future__ import annotations
+
+import re
+import subprocess
+import typing
+import uuid
+
+from walt.common.formatting import format_sentence
+from walt.server.exttools import docker
+from walt.server.processes.blocking.images.metadata import pull_user_metadata
+from walt.server.processes.blocking.registries import (
+    DockerDaemonClient,
+    DockerHubClient,
+    get_custom_registry_client,
+)
+from walt.server.tools import get_clone_url_locations
+
+if typing.TYPE_CHECKING:
+    from walt.server.processes.main.server import Server
 
 # About terminology: See comment about it in image.py.
 
 # Implementation notes:
 # walt image clone relies on a complex process.
 # depending on what we are cloning, who we are,
-# what are the existing docker images and whether
+# what are the existing images and whether
 # we want to overwrite these existing images or not,
 # we have many cases to think about.
 # that's why we have organised this process as follows:
 # 1- we search for existing images
 # 2- we perform basic validation of the request
 # 3- we compute a workflow (a list of function calls)
 # 4- we execute this workflow.
 #
-# (also note that since docker downloads may take a long time,
+# (also note that since docker-hub downloads may take a long time,
 # we also have to implement this in an asynchronous task.)
 
 MSG_IMAGE_NOT_REMOTE_BELONGS_TO_WS = """\
 Invalid clonable image link.
 Images of the form 'walt:%s/<image_name>' already belong to
 your working set and thus are not clonable.
 """
-MSG_USE_FORCE = """\
+MSG_USE_FORCE_CLI = """\
 If this is what you want, rerun with --force:
 $ %s
 """
+MSG_USE_FORCE_API = """\
+If this is what you want, use force=True.
+"""
 MSG_INVALID_CLONABLE_LINK = """\
 Invalid clonable image link. Format must be:
-[walt|docker|hub]:<user>/<image_name>[:<tag>]
+{link_format}
 (tip: walt image search [<keyword>])
 """
 MSG_INCOMPATIBLE_MODELS = """\
 Sorry, cannot proceed. There is an image with the same name in your
 working set. Overriding it is not allowed because it is currently
 in use, and the target image is not compatible with %s.
 """
 
+
 # Subroutines
 # -----------
+def fix_image_name(requester, image_name):
+    new_name = re.sub("[^a-z0-9:]+", "-", image_name.lower())
+    if new_name != image_name:
+        requester.stdout.write(
+            f'Image will be recorded as "{new_name}" since original name is not valid'
+            " in WALT.\n"
+        )
+    return new_name
+
+
 def parse_clonable_link(requester, clonable_link):
     bad = False
-    parts = clonable_link.split(':', 1)
+    parts = clonable_link.split(":", 1)
     if len(parts) != 2:
         bad = True
     if not bad:
         location = parts[0]
-        if location not in LOCATION_LABEL.values():
+        if location not in get_clone_url_locations():
             bad = True
     if not bad:
-        parts = parts[1].split('/')
+        parts = parts[1].split("/")
         if len(parts) != 2:
             bad = True
     if not bad:
         user, image_name = parts
-        parts = image_name.split(':')
+        parts = image_name.split(":")
         if len(parts) == 1:
-            image_name += ':latest'
+            image_name += ":latest"
         elif len(parts) != 2:
             bad = True
     if not bad:
-        return (LOCATION_PER_LABEL[location], user, image_name)
+        return (location, user, image_name)
     if bad:
-        requester.stderr.write(MSG_INVALID_CLONABLE_LINK)
+        locations_or = "|".join(get_clone_url_locations())
+        link_format = f"[{locations_or}]:<user>/<image_name>[:<tag>]"
+        requester.stderr.write(
+            MSG_INVALID_CLONABLE_LINK.format(link_format=link_format)
+        )
         return None, None, None
 
+
 def get_temp_image_fullname():
-    return 'clone-temp/walt-image:' + str(uuid.uuid4()).split('-')[0]
+    return "walt/clone-temp:" + str(uuid.uuid4()).split("-")[0]
+
 
 def exit_no_such_image(requester):
+    requester.stderr.write("No such remote image. Use walt image search <keyword>.\n")
+    return ("FAILED",)
+
+
+def exit_image_without_models(requester):
     requester.stderr.write(
-            'No such remote image. Use walt image search <keyword>.\n')
-    return ('FAILED',)
+        "Failed. This remote image does not indicate compatible node models.\n"
+    )
+    return ("FAILED",)
+
 
 # workflow functions
 # ------------------
 
+
 # Note: we save initial images, because:
 # * in some cases we want to retain the filesystem layers otherwise we
 # would need to download them again (case of the overwrite of a server
 # image with its updated hub version)
 # * if we detect an issue late in the workflow, we can still restore them.
-def save_initial_images(saved_images,
-                        ws_image_fullname, remote_image_fullname,
-                        existing_server_image, existing_ws_image,
-                        docker, **args):
+def save_initial_images(
+    saved_images,
+    ws_image_fullname,
+    remote_image_fullname,
+    existing_server_image,
+    existing_ws_image,
+    walt_local_repo,
+    **args,
+):
     initial_image_fullnames = set()
-    for fullname, exists in (   (ws_image_fullname, existing_ws_image),
-                                (remote_image_fullname, existing_server_image)):
+    for fullname, exists in (
+        (ws_image_fullname, existing_ws_image),
+        (remote_image_fullname, existing_server_image),
+    ):
         if exists:
             initial_image_fullnames.add(fullname)
     for image_fullname in initial_image_fullnames:
         image_backup = get_temp_image_fullname()
-        docker.local.tag(image_fullname, image_backup)
+        walt_local_repo.tag(image_fullname, image_backup)
         saved_images[image_fullname] = image_backup
 
+
 def error_image_belongs_to_ws(requester, username, **args):
-    requester.stderr.write(
-        MSG_IMAGE_NOT_REMOTE_BELONGS_TO_WS % username)
+    requester.stderr.write(MSG_IMAGE_NOT_REMOTE_BELONGS_TO_WS % username)
     return False
 
-def verify_overwrite(image_store, requester, clonable_link,
-                    ws_image_fullname, force, image_name, **args):
+
+def verify_overwrite(
+    image_store, requester, clonable_link, ws_image_fullname, force, image_name, **args
+):
     if not force:
-        image_store.warn_overwrite_image(requester, ws_image_fullname)
-        force_clone = "walt image clone --force " + clonable_link
-        if image_name is not None:
-            force_clone += ' ' + image_name
-        requester.stderr.write(MSG_USE_FORCE % force_clone)
+        client_type = requester.get_client_type()
+        if client_type is None:
+            return False  # already disconnected
+        msg = image_store.get_image_overwrite_warning(ws_image_fullname)
+        if client_type == "cli":
+            force_clone = "walt image clone --force " + clonable_link
+            if image_name is not None and not clonable_link.endswith(image_name):
+                force_clone += " " + image_name
+            msg += MSG_USE_FORCE_CLI % force_clone
+        elif client_type == "api":
+            msg += MSG_USE_FORCE_API
+        requester.stderr.write(msg)
         return False
 
+
 # check possible compatibility issue regarding node models
-def verify_compatibility_issue(image_store, requester, clonable_link,
-                    ws_image_fullname, remote_image_fullname,
-                    docker, target_node_models, nodes_manager, **args):
+def verify_compatibility_issue(
+    image_store, requester, ws_image_fullname, target_node_models, nodes_manager, **args
+):
     ws_image = image_store[ws_image_fullname]
-    if not ws_image.in_use:
+    if not ws_image.in_use():
         return  # no problem
     # there is a risk of overwritting the mounted ws image with
     # a target image that is incompatible.
-    nodes = nodes_manager.get_nodes_using_image(ws_image_fullname)
-    needed_models = set(node.model for node in nodes)
+    needed_models = nodes_manager.get_node_models_using_image(ws_image_fullname)
     image_compatible_models = set(target_node_models)
     incompatible_models = needed_models - image_compatible_models
     if len(incompatible_models) > 0:
-        sentence = format_sentence(MSG_INCOMPATIBLE_MODELS, incompatible_models,
-                        None, 'node model', 'node models')
+        sentence = format_sentence(
+            MSG_INCOMPATIBLE_MODELS,
+            incompatible_models,
+            None,
+            "node model",
+            "node models",
+        )
         requester.stderr.write(sentence)
-        return False    # give up
+        return False  # give up
 
-def remove_ws_image(docker, ws_image_fullname, **args):
-    docker.local.untag(ws_image_fullname)
 
-def remove_server_image(docker, remote_image_fullname, **args):
-    docker.local.untag(remote_image_fullname)
+def remove_ws_image(image_store, walt_local_repo, ws_image_fullname, **args):
+    ws_image = image_store[ws_image_fullname]
+    ws_image.filesystem.close()
+    walt_local_repo.untag(ws_image_fullname)
+
+
+def remove_server_image(walt_local_repo, remote_image_fullname, **args):
+    walt_local_repo.untag(remote_image_fullname)
 
-def restore_initial_ws_image(docker, ws_image_fullname,
-                                saved_images, **args):
+
+def restore_initial_ws_image(walt_local_repo, ws_image_fullname, saved_images, **args):
     ws_image_backup = saved_images[ws_image_fullname]
-    docker.local.tag(ws_image_backup, ws_image_fullname)
+    walt_local_repo.tag(ws_image_backup, ws_image_fullname)
+
 
-def restore_initial_server_image(docker, remote_image_fullname,
-                                saved_images, **args):
+def restore_initial_server_image(
+    walt_local_repo, remote_image_fullname, saved_images, **args
+):
     server_image_backup = saved_images[remote_image_fullname]
-    docker.local.tag(server_image_backup, remote_image_fullname)
+    walt_local_repo.tag(server_image_backup, remote_image_fullname)
+
+
+def tag_server_image_to_requester(
+    walt_local_repo, ws_image_fullname, remote_image_fullname, **args
+):
+    walt_local_repo.tag(remote_image_fullname, ws_image_fullname)
+
+
+def pull_image(requester, server, remote_location, remote_image_fullname, **args):
+    if remote_location == "hub":
+        hub = DockerHubClient()
+        hub.pull(requester, server, remote_image_fullname)
+    elif remote_location == "docker":
+        docker_daemon = DockerDaemonClient()
+        docker_daemon.pull(requester, server, remote_image_fullname)
+    else:
+        registry = get_custom_registry_client(remote_location)
+        registry.pull(requester, server, remote_image_fullname)
 
-def tag_server_image_to_requester(docker,
-                ws_image_fullname, remote_image_fullname, **args):
-    docker.local.tag(remote_image_fullname, ws_image_fullname)
-
-def pull_image(docker, requester, remote_location, remote_image_fullname, **args):
-    if remote_location == LOCATION_DOCKER_HUB:
-        docker.hub.pull(remote_image_fullname, requester)
-    elif remote_location == LOCATION_DOCKER_DAEMON:
-        docker.daemon.pull(remote_image_fullname, requester)
 
 class WorkflowCleaner:
     def __init__(self, context):
         self.context = context
+
     def __enter__(self):
         pass
+
     def __exit__(self, exc_type, exc_value, traceback):
-        if exc_type is None:    # ok, no exception
+        if exc_type is None:  # ok, no exception
             self.cleanup(True, **self.context)
-        else:                   # not ok, an exception occured!
+        else:  # not ok, an exception occured!
             self.cleanup(False, **self.context)
-    def cleanup(self, ok, docker, image_store, saved_images,
-                ws_image_fullname, remote_image_fullname,
-                existing_server_image, existing_ws_image, **args):
+
+    def cleanup(
+        self,
+        ok,
+        walt_local_repo,
+        image_store,
+        saved_images,
+        ws_image_fullname,
+        remote_image_fullname,
+        **args,
+    ):
         if not ok:  # only if an exception occured
             # remove any temporary images created there
-            docker.local.untag(ws_image_fullname, ignore_missing=True)
-            docker.local.untag(remote_image_fullname, ignore_missing=True)
+            walt_local_repo.untag(ws_image_fullname, ignore_missing=True)
+            walt_local_repo.untag(remote_image_fullname, ignore_missing=True)
             # restore the backups
             for image_fullname, backup_fullname in saved_images.items():
-                docker.local.tag(backup_fullname, image_fullname)
+                walt_local_repo.tag(backup_fullname, image_fullname)
+        # in any case cleanup the backup tags
+        for backup_fullname in saved_images.values():
+            walt_local_repo.untag(backup_fullname)
         # if ok, update the image store
         # (otherwise we just restored things from backup, so there was no change)
         if ok:
-            docker.local.clear_name_cache()
-            image_store.refresh()
-            image_store.update_image_mounts()
-        # in any case cleanup the backup tags
-        for backup_fullname in saved_images.values():
-            docker.local.untag(backup_fullname)
+            image_store.resync_from_registry()
+            image_store.trigger_update_image_mounts()
+
 
 # workflow management functions
 # -----------------------------
 def workflow_exit(**context):
     return False
 
+
 def workflow_if(condition_func, workflow_if_true, workflow_if_false):
     def workflow_if_instance(**context):
-        if condition_func(**context) != False:
+        if condition_func(**context) is not False:
             return workflow_run(workflow_if_true, **context)
         else:
             return workflow_run(workflow_if_false, **context)
+
     return workflow_if_instance
 
+
 def workflow_run(workflow, **context):
     for f in workflow:
         res = f(**context)
-        if res == False:
-            return False # issue, stop here
+        if res is False:
+            return False  # issue, stop here
     return True
 
+
 # walt image clone implementation
 # -------------------------------
-def perform_clone(requester, docker, nodes_manager, clonable_link, image_store, force, image_name):
+def perform_clone(requester, clonable_link, image_store, force, image_name, **kwargs):
     username = requester.get_username()
     if not username:
-        return ('FAILED',) # client already disconnected, give up
+        return ("FAILED",)  # client already disconnected, give up
     remote_location, remote_user, remote_image_name = parse_clonable_link(
-                                                requester, clonable_link)
-    if remote_location == None:
-        return ('FAILED',) # error already reported
+        requester, clonable_link
+    )
+    if remote_location is None:
+        return ("FAILED",)  # error already reported
 
     if image_name is None:
         # if not specified, name it the same as remote image
-        ws_image_fullname = "%s/%s" % (username, remote_image_name)
-    else:
-        ws_image_fullname = "%s/%s" % (username, image_name)
-        if ':' not in image_name:
-            ws_image_fullname += ':latest'
+        image_name = fix_image_name(requester, remote_image_name)
+
+    ws_image_fullname = "%s/%s" % (username, image_name)
+    if ":" not in image_name:
+        ws_image_fullname += ":latest"
     remote_image_fullname = "%s/%s" % (remote_user, remote_image_name)
 
     # analyse our context
-    existing_server_image = remote_image_fullname in image_store
-    existing_ws_image = ws_image_fullname in image_store
-    same_image = (remote_image_fullname == ws_image_fullname)
-    image_is_local = (remote_location == LOCATION_WALT_SERVER)
+    existing_server_image = image_store.__contains__(remote_image_fullname)
+    existing_ws_image = image_store.__contains__(ws_image_fullname)
+    same_image = remote_image_fullname == ws_image_fullname
+    image_is_local = remote_location == "walt"
 
     # check that the requested image really exists,
     # and fetch compatibility info
-    if remote_location == LOCATION_WALT_SERVER:
-        if remote_image_fullname not in image_store:
+    if remote_location == "walt":
+        if not image_store.__contains__(remote_image_fullname):
             return exit_no_such_image(requester)
-        target_node_models = image_store[remote_image_fullname].get_node_models()
-    if remote_location == LOCATION_DOCKER_HUB:
-        remote_user_metadata = pull_user_metadata(docker, remote_user)
-        if remote_image_fullname not in remote_user_metadata['walt.user.images']:
+        labels = image_store[remote_image_fullname].get_labels()
+    elif remote_location == "hub":
+        hub = DockerHubClient()
+        remote_user_metadata = pull_user_metadata(hub, remote_user)
+        if remote_image_fullname not in remote_user_metadata["walt.user.images"]:
             return exit_no_such_image(requester)
-        image_info = remote_user_metadata['walt.user.images'][remote_image_fullname]
-        target_node_models = image_info['labels']['walt.node.models'].split(',')
-    if remote_location == LOCATION_DOCKER_DAEMON:
-        labels = None
+        image_info = remote_user_metadata["walt.user.images"][remote_image_fullname]
+        labels = image_info["labels"]
+    elif remote_location == "docker":
+        if docker is None:
+            requester.stderr.write("Docker is not available on the server.\n")
+            return ("FAILED",)
+        try:
+            docker_daemon = DockerDaemonClient()
+            labels = docker_daemon.get_labels(requester, remote_image_fullname)
+        except subprocess.CalledProcessError:
+            requester.stderr.write("Error while loading images from Docker.\n")
+            return ("FAILED",)
+    else:
+        registry = get_custom_registry_client(remote_location)
         try:
-            labels = docker.daemon.get_labels(remote_image_fullname)
-        except:
+            labels = registry.get_labels(requester, remote_image_fullname)
+        except Exception:
             return exit_no_such_image(requester)
-        target_node_models = labels['walt.node.models'].split(',')
+    if "walt.node.models" not in labels:
+        return exit_image_without_models(requester)
+    target_node_models = labels["walt.node.models"].split(",")
 
     # compute the workflow
     # --------------------
     # obvious facts:
     # * if image_is_local is True, existing_server_image is True
     # * if same_image is True, existing_server_image == existing_ws_image
     # that's why not all workflow entries are possible.
     workflow_selector = {
         # image_is_local, existing_server_image, existing_ws_image, same_image
-        (True, True, False, False): [ tag_server_image_to_requester ],
-        (True, True, True, False):  [ verify_compatibility_issue, verify_overwrite,
-                                                        remove_ws_image, tag_server_image_to_requester ],
-        (True, True, True, True):   [ error_image_belongs_to_ws ],
-
-        (False, False, False, False): [ pull_image, tag_server_image_to_requester, remove_server_image ],
-        (False, False, True, False):  [ verify_compatibility_issue, verify_overwrite, pull_image,
-                                                        remove_ws_image, \
-                                                        tag_server_image_to_requester, remove_server_image ],
-        (False, True, False, False):  [ remove_server_image, pull_image,
-                                                        tag_server_image_to_requester, remove_server_image,
-                                                        restore_initial_server_image ],
-        (False, True, True, False):   [ verify_compatibility_issue, verify_overwrite,
-                                                        remove_server_image, pull_image,
-                                                        remove_ws_image, tag_server_image_to_requester,
-                                                        remove_server_image, restore_initial_server_image ],
-        (False, False, False, True):  [ pull_image ],
-        (False, True, True, True):    [ verify_compatibility_issue, verify_overwrite, remove_ws_image,
-                                                        pull_image ],
+        (True, True, False, False): [tag_server_image_to_requester],
+        (True, True, True, False): [
+            verify_compatibility_issue,
+            verify_overwrite,
+            remove_ws_image,
+            tag_server_image_to_requester,
+        ],
+        (True, True, True, True): [error_image_belongs_to_ws],
+        (False, False, False, False): [
+            pull_image,
+            tag_server_image_to_requester,
+            remove_server_image,
+        ],
+        (False, False, True, False): [
+            verify_compatibility_issue,
+            verify_overwrite,
+            pull_image,
+            remove_ws_image,
+            tag_server_image_to_requester,
+            remove_server_image,
+        ],
+        (False, True, False, False): [
+            remove_server_image,
+            pull_image,
+            tag_server_image_to_requester,
+            remove_server_image,
+            restore_initial_server_image,
+        ],
+        (False, True, True, False): [
+            verify_compatibility_issue,
+            verify_overwrite,
+            remove_server_image,
+            pull_image,
+            remove_ws_image,
+            tag_server_image_to_requester,
+            remove_server_image,
+            restore_initial_server_image,
+        ],
+        (False, False, False, True): [pull_image],
+        (False, True, True, True): [
+            verify_compatibility_issue,
+            verify_overwrite,
+            remove_ws_image,
+            pull_image,
+        ],
     }
-    workflow = [ save_initial_images ]     # this is always called first
-    workflow += workflow_selector[(image_is_local, existing_server_image, existing_ws_image, same_image)]
-    print('clone workflow is:', ', '.join([ f.__name__ for f in workflow ]))
+    workflow = [save_initial_images]  # this is always called first
+    workflow += workflow_selector[
+        (image_is_local, existing_server_image, existing_ws_image, same_image)
+    ]
+    print("clone workflow is:", ", ".join([f.__name__ for f in workflow]))
 
     # proceed
     # -------
     context = dict(
-        image_name = image_name,
-        remote_location = remote_location,
-        username = username,
-        ws_image_fullname = ws_image_fullname,
-        remote_image_fullname = remote_image_fullname,
-        existing_server_image = existing_server_image,
-        existing_ws_image = existing_ws_image,
-        image_store = image_store,
-        docker = docker,
-        requester = requester,
-        force = force,
-        saved_images = {},
-        clonable_link = clonable_link,
-        target_node_models = target_node_models,
-        nodes_manager = nodes_manager
+        image_name=image_name,
+        remote_location=remote_location,
+        username=username,
+        ws_image_fullname=ws_image_fullname,
+        remote_image_fullname=remote_image_fullname,
+        existing_server_image=existing_server_image,
+        existing_ws_image=existing_ws_image,
+        image_store=image_store,
+        requester=requester,
+        force=force,
+        saved_images={},
+        clonable_link=clonable_link,
+        target_node_models=target_node_models,
+        **kwargs,
     )
 
     # we use a context manager ("with-construct") to ensure
     # the WorkflowCleaner.cleanup function will be called,
     # even in case of an exception.
-    # this fonction will remove any temporary docker image.
+    # this fonction will remove any temporary image.
     res = False
     with WorkflowCleaner(context):
         res = workflow_run(workflow, **context)
 
     if res:
-        requester.stdout.write('Done.\n')
         if existing_ws_image:
-            return ('OK_BUT_REBOOT_NODES', ws_image_fullname)
+            return ("OK_BUT_REBOOT_NODES", ws_image_fullname)
         else:
-            return ('OK',)
+            return ("OK", ws_image_fullname)
     else:
-        return ('FAILED',)
+        return ("FAILED",)
 
-# this implements walt image clone
-def clone(requester, server, **kwargs):
-    return perform_clone(  requester = requester,
-                    docker = server.docker,
-                    image_store = server.images.store,
-                    nodes_manager = server.nodes,
-                    **kwargs)
 
+# this implements walt image clone
+def clone(requester, server: Server, **kwargs):
+    try:
+        return perform_clone(
+            requester=requester,
+            server=server,
+            walt_local_repo=server.registry,
+            image_store=server.images.store,
+            nodes_manager=server.nodes,
+            **kwargs,
+        )
+    except Exception as e:
+        requester.stderr.write(str(e) + "\n")
+        return ("FAILED",)
```

### Comparing `walt-server-7/walt/server/threads/blocking/images/metadata.py` & `walt-server-8.0/walt/server/processes/blocking/images/metadata.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,90 @@
-#!/usr/bin/env python
+from __future__ import annotations
+
+import asyncio
+import base64
+import json
+
 from walt.server.exttools import buildah
-import json, base64
+from walt.server.processes.blocking.registries import DockerHubClient
+from walt.server.tools import async_gather_tasks
+
+
+def collect_user_metadata(hub, user):
+    return asyncio.run(async_collect_user_metadata(hub, user))
+
+
+async def async_collect_user_metadata(hub, user):
+    tasks = []
+    async for repo in hub.async_list_user_repos(user):
+        reponame = user + "/" + repo
+        tasks += [asyncio.create_task(async_collect_repo_metadata(hub, reponame))]
+    results = await async_gather_tasks(tasks)
+    walt_images = {}
+    for repo_images in results:
+        walt_images.update(repo_images)
+    return {"walt.user.images": walt_images}
+
 
-def collect_user_metadata(docker, user):
+async def async_collect_repo_metadata(hub, reponame):
+    tasks, fullnames = [], []
+    async for tag in hub.async_list_image_tags(reponame):
+        fullname = reponame + ":" + tag
+        task = asyncio.create_task(hub.async_get_labels(None, fullname))
+        tasks.append(task)
+        fullnames.append(fullname)
+    results = await async_gather_tasks(tasks)
     walt_images = {}
-    for repo in docker.hub.list_user_repos(user):
-        reponame = user + '/' + repo
-        for tag in docker.hub.list_image_tags(reponame):
-            fullname = reponame + ':' + tag
-            labels = docker.hub.get_labels(fullname)
-            if 'walt.node.models' in labels:
-                walt_images[fullname] = dict(
-                    labels = labels
-                )
-    return { 'walt.user.images': walt_images }
-
-def push_user_metadata(docker, dh_peer, auth_conf, requester, user, metadata):
-    encoded = base64.b64encode(json.dumps(metadata).encode('UTF-8'))
-    encoded = encoded.decode('UTF-8')
-    fullname = '%(user)s/walt_metadata:latest' % dict(user = user)
-    cont_name = buildah('from', 'scratch')
+    for fullname, labels in zip(fullnames, results):
+        if "walt.node.models" in labels:
+            walt_images[fullname] = dict(labels=labels)
+    return walt_images
+
+
+def push_user_metadata(requester, hub, user, metadata):
+    encoded = base64.b64encode(json.dumps(metadata).encode("UTF-8"))
+    encoded = encoded.decode("UTF-8")
+    fullname = "%(user)s/walt_metadata:latest" % dict(user=user)
+    cont_name = buildah("from", "scratch")
     # for the future (OCI images show only annotations in their manifest)
-    buildah.config('--annotation', 'metadata=' + encoded, cont_name)
+    buildah.config("--annotation", "metadata=" + encoded, cont_name)
     # for the present (legacy walt code parses only manifests with docker format)
-    buildah.config('--label', 'metadata=' + encoded, cont_name)
+    buildah.config("--label", "metadata=" + encoded, cont_name)
     # for now, save metadata images with docker manifest format
-    buildah.commit('--format', 'docker', cont_name, fullname)
+    buildah.commit("--format", "docker", cont_name, fullname)
     buildah.rm(cont_name)
-    docker.hub.push(fullname, dh_peer, auth_conf, requester)
+    success = hub.push(requester, fullname)
     buildah.rmi(fullname)
+    return success
+
+
+def pull_user_metadata(hub, user):
+    return asyncio.run(async_pull_user_metadata(hub, user))
 
-def pull_user_metadata(docker, user):
+
+async def async_pull_user_metadata(hub, user):
     try:
-        labels = docker.hub.get_labels(
-                '%(user)s/walt_metadata:latest' % dict(user = user))
-        encoded = labels['metadata']
-        return json.loads(base64.b64decode(encoded).decode('UTF-8'))
-    except:     # user did not push metadata yet
-        return { 'walt.user.images': {} }
-
-def update_user_metadata_for_image(docker, image_store, dh_peer, auth_conf, \
-                                   requester, image_fullname):
-    user = image_fullname.split('/')[0]
-    # read labels
-    labels = image_store[image_fullname].labels
+        labels = await hub.async_get_labels(
+            None, "%(user)s/walt_metadata:latest" % dict(user=user)
+        )
+        encoded = labels["metadata"]
+        return json.loads(base64.b64decode(encoded).decode("UTF-8"))
+    except Exception:  # user did not push metadata yet
+        return {"walt.user.images": {}}
+
+
+def update_user_metadata_for_image(requester, hub, image_fullname, labels):
+    hub_username = requester.get_registry_username("hub")
     # retrieve existing metadata (i.e. for other images...)
-    metadata = pull_user_metadata(docker, user)
+    metadata = pull_user_metadata(hub, hub_username)
     # update metadata of this image
-    metadata['walt.user.images'][image_fullname] = dict(
-        labels = labels
-    )
+    metadata["walt.user.images"][image_fullname] = dict(labels=labels)
     # push back on docker hub
-    push_user_metadata(docker, dh_peer, auth_conf, requester, user, metadata)
+    return push_user_metadata(requester, hub, hub_username, metadata)
+
 
-def update_hub_metadata(requester, server, dh_peer, auth_conf, user):
+def update_hub_metadata(requester, user):
+    hub = DockerHubClient()
     # collect
-    metadata = collect_user_metadata(server.docker, user)
+    metadata = collect_user_metadata(hub, user)
     # push back on docker hub
-    push_user_metadata(server.docker, dh_peer, auth_conf, requester, user, metadata)
+    return push_user_metadata(requester, hub, user, metadata)
```

### Comparing `walt-server-7/walt/server/threads/blocking/logs.py` & `walt-server-8.0/walt/server/processes/blocking/logs.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-
 def stream_db_logs(db, logs_handler, **params):
     # ensure all past logs are commited
     db.commit()
     # let the logs handler start buffering realtime logs
     logs_handler.notify_history_processing_startup()
     db.commit()
     # create a server cursor
-    cursor_name = db.create_server_cursor()
+    cursor_name = db.create_server_logs_cursor(**params)
     # start streaming db logs
-    for record in db.get_logs(cursor_name, **params):
+    while True:
+        record = db.step_server_cursor(cursor_name)
+        if record is None:
+            break
         d = record._asdict()
-        if logs_handler.write_to_client(
-                    senders_filtered = True, **d) == False:
+        if logs_handler.write_to_client(issuers_filtered=True, **d) is False:
             break
     # delete server cursor
     db.delete_server_cursor(cursor_name)
     # notify history dump is complete
     logs_handler.notify_history_processed()
-
```

### Comparing `walt-server-7/walt/server/threads/main/api/ss.py` & `walt-server-8.0/walt/server/processes/main/api/ss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from walt.common.api import api, api_expose_method
-from walt.server.threads.main.apisession import APISession
+from walt.server.processes.main.apisession import APISession
 
 # Server -> Server API (thus the name SSAPI)
 # Provides remote calls performed from one server executable
 # to another one.
 # For instance walt-dhcp-event sends requests to walt-server-daemon
 # when a new DHCP address is assigned.
 # Note that since both executables belong to the server code,
 # API versioning is not relevant here. But for clarity we use
 # the same decorators as for the other APIs.
 
+
 @api
 class SSAPI(APISession):
-
     @api_expose_method
     def register_device(self, context, *args):
         context.server.add_or_update_device(*args)
```

### Comparing `walt-server-7/walt/server/threads/main/api/vs.py` & `walt-server-8.0/walt/server/processes/main/api/vs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from walt.common.api import api, api_expose_method
-from walt.server.threads.main.apisession import APISession
+from walt.server.processes.main.apisession import APISession
 
 # Virtual component -> Server API (thus the name VSAPI)
 # Provides remote calls performed from a virtual component to the server.
 
+
 @api
 class VSAPI(APISession):
-
     @api_expose_method
     def register_device(self, context, *args):
         context.server.add_or_update_device(*args)
 
     @api_expose_method
     def get_device_info(self, context, device_mac):
         return context.server.get_device_info(device_mac)
```

### Comparing `walt-server-7/walt/server/threads/main/apisession.py` & `walt-server-8.0/walt/server/processes/main/apisession.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,67 @@
 from walt.common.tools import SimpleContainer
-from walt.server.threads.main.task import APISessionTask
+from walt.server.processes.main.task import APISessionTask
 
-class APISession(object):
 
-    NEXT_ID = 0
+class APISession(object):
     SESSIONS = {}
     TARGET_APIS = {}
     SERVER_CONTEXT = None
 
     @staticmethod
     def register_target_api(name, cls):
         APISession.TARGET_APIS[name] = cls
 
     @staticmethod
-    def create(server, target_api, remote_ip):
-        session_id = APISession.NEXT_ID
-        APISession.NEXT_ID += 1
+    def create(server, session_id, target_api, remote_ip):
         cls = APISession.TARGET_APIS[target_api]
         APISession.SESSIONS[session_id] = cls(server, remote_ip)
-        print('session %d: connected' % session_id)
-        return session_id
+        # print("session %d: connected" % session_id)
 
     @staticmethod
     def destroy(session_id):
-        print('session %d: disconnected' % session_id)
+        # print("session %d: disconnected" % session_id)
         APISession.SESSIONS[session_id].cleanup()
         del APISession.SESSIONS[session_id]
 
     @staticmethod
     def cleanup_all():
         for session in APISession.SESSIONS.values():
             session.cleanup()
 
     @staticmethod
-    def get(session_id):
+    def get(server, session_id, target_api, remote_ip):
+        if session_id not in APISession.SESSIONS:
+            APISession.create(server, session_id, target_api, remote_ip)
         return APISession.SESSIONS[session_id]
 
     def __init__(self, server, remote_ip):
         self.session_objects = []
-        if APISession.SERVER_CONTEXT == None:
+        if APISession.SERVER_CONTEXT is None:
             APISession.SERVER_CONTEXT = SimpleContainer(
-                    server = server,
-                    images = server.images,
-                    devices = server.devices,
-                    topology = server.topology,
-                    nodes = server.nodes,
-                    logs = server.logs
+                server=server,
+                images=server.images,
+                devices=server.devices,
+                blocking=server.blocking,
+                nodes=server.nodes,
+                logs=server.logs,
             )
         self.context = APISession.SERVER_CONTEXT.copy().update(
-            remote_ip = remote_ip,
+            remote_ip=remote_ip,
         )
 
     def run_task(self, rpc_context, attr, args, kwargs):
         task = APISessionTask(rpc_context, self, attr, args, kwargs)
-        task.run()
+        return task.run()
 
     def register_session_object(self, obj):
         obj_id = len(self.session_objects)
         self.session_objects.append(obj)
         return obj_id
 
     def get_session_object(self, obj_id):
         return self.session_objects[obj_id]
 
     def cleanup(self):
         for obj in self.session_objects:
-            if hasattr(obj, 'cleanup'):
+            if hasattr(obj, "cleanup"):
                 obj.cleanup()
-
```

### Comparing `walt-server-7/walt/server/threads/main/blocking.py` & `walt-server-8.0/walt/server/processes/main/blocking.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,75 @@
-from walt.common.thread import RPCThreadConnector
-from walt.common.apilink import AttrCallRunner, AttrCallAggregator
+from walt.server.process import RPCProcessConnector, RPCService
+
+
+class BlockingTasksManager(RPCProcessConnector):
+    def __init__(self, server):
+        super().__init__(
+            default_service=RPCService(server=server),
+            local_context=False,
+            label="main-to-blocking",
+        )
+        self.server = server
 
-class BlockingTasksManager(RPCThreadConnector):
     def session(self, requester):
-        # we will receive:
-        # service.<func>(rpc_context, <args...>)
-        # and we must forward the call as:
-        # requester.<func>(<args...>)
-        # the following code handles this forwarding
-        # and removal of the 'rpc_context' parameter.
-        runner = AttrCallRunner(requester)
-        def forward_to_requester(attr, args, kwargs):
-            return runner.do(attr, args[1:], kwargs)
-        service = AttrCallAggregator(forward_to_requester)
-        return self.local_service(service)
+        local_service = RPCService(requester=requester, server=self.server)
+        return self.create_session(local_service=local_service)
 
     def clone_image(self, requester, result_cb, *args, **kwargs):
         self.session(requester).do_async.clone_image(*args, **kwargs).then(result_cb)
 
     def search_image(self, requester, result_cb, *args, **kwargs):
         self.session(requester).do_async.search_image(*args, **kwargs).then(result_cb)
 
     def publish_image(self, requester, result_cb, *args, **kwargs):
         self.session(requester).do_async.publish_image(*args, **kwargs).then(result_cb)
 
     def squash_image(self, requester, result_cb, *args, **kwargs):
         self.session(requester).do_async.squash_image(*args, **kwargs).then(result_cb)
 
+    def commit_image(self, requester, result_cb, *args, **kwargs):
+        self.session(requester).do_async.commit_image(*args, **kwargs).then(result_cb)
+
     def update_hub_metadata(self, requester, result_cb, *args, **kwargs):
-        self.session(requester).do_async.update_hub_metadata(*args, **kwargs).then(result_cb)
+        self.session(requester).do_async.update_hub_metadata(*args, **kwargs).then(
+            result_cb
+        )
+
+    def pull_image(self, requester, image_fullname, result_cb):
+        if requester is None:
+            self.do_async.pull_image(image_fullname, anonymous=True).then(result_cb)
+        else:
+            self.session(requester).do_async.pull_image(
+                image_fullname, anonymous=False
+            ).then(result_cb)
 
-    def pull_image(self, image_fullname, result_cb):
-        self.do_async.pull_image(image_fullname).then(result_cb)
+    def registry_login(self, requester, result_cb, *args, **kwargs):
+        self.session(requester).do_async.registry_login(*args, **kwargs).then(result_cb)
 
     def stream_db_logs(self, logs_handler):
         # request the blocking task to stream db logs
-        self.session(logs_handler).do_async.stream_db_logs(
-                            **logs_handler.params)
+        self.session(logs_handler).do_async.stream_db_logs(**logs_handler.params)
 
     def rescan_topology(self, requester, result_cb, *args, **kwargs):
-        self.session(requester).do_async.rescan_topology(*args, **kwargs).then(result_cb)
+        self.session(requester).do_async.rescan_topology(*args, **kwargs).then(
+            result_cb
+        )
+
+    def topology_tree(self, requester, result_cb, *args, **kwargs):
+        self.session(requester).do_async.topology_tree(*args, **kwargs).then(result_cb)
+
+    def nodes_set_poe(self, result_cb, *args, **kwargs):
+        self.do_async.nodes_set_poe(*args, **kwargs).then(result_cb)
+
+    def restore_poe_on_all_ports(self):
+        self.do_async.restore_poe_on_all_ports()
+
+    def run_shell_cmd(self, requester, result_cb, cmd, **kwargs):
+        self.session(requester).do_async.run_shell_cmd(cmd, **kwargs).then(result_cb)
 
-    def nodes_set_poe(self, requester, result_cb, *args, **kwargs):
-        self.session(requester).do_async.nodes_set_poe(*args, **kwargs).then(result_cb)
+    # sync calls will block the 'main' process, so should only be used e.g. during
+    # service startup.
+    def sync_list_docker_daemon_images(self):
+        return self.session(None).do_sync.list_docker_daemon_images()
 
-    def run_shell_cmd(self, requester, result_cb, cmd):
-        self.session(requester).do_async.run_shell_cmd(cmd).then(result_cb)
+    def sync_pull_docker_daemon_image(self, fullname):
+        return self.session(None).do_sync.pull_docker_daemon_image(fullname)
```

### Comparing `walt-server-7/walt/server/threads/main/devices/grouper.py` & `walt-server-8.0/walt/server/processes/blocking/devices/grouper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 #!/usr/bin/env python
-from itertools import count
 from collections import defaultdict
+from itertools import count
+
 
 class Grouper:
     def __init__(self):
         self.group_ids = count()
         self.items_per_group_id = defaultdict(set)
         self.group_id_per_item = {}
+
     def add_isolated_item(self, item):
         group_id = next(self.group_ids)
         self.items_per_group_id[group_id].add(item)
         self.group_id_per_item[item] = group_id
         return group_id
+
     def get_group_id(self, item):
         group_id = self.group_id_per_item.get(item, None)
         if group_id is None:
             # item was not known yet, register it
             group_id = self.add_isolated_item(item)
         return group_id
+
     def group_items(self, item1, item2):
         item1_group_id = self.get_group_id(item1)
         item2_group_id = self.get_group_id(item2)
         item2_friends = self.items_per_group_id.pop(item2_group_id)
         for item in item2_friends:
             self.group_id_per_item[item] = item1_group_id
         self.items_per_group_id[item1_group_id] |= item2_friends
+
     def num_groups(self):
         return len(self.items_per_group_id)
+
     def is_same_group(self, item1, item2):
         return self.get_group_id(item1) == self.get_group_id(item2)
+
     def __contains__(self, item):
         return item in self.group_id_per_item
+
     def debug(self):
         for group_id, items in self.items_per_group_id.items():
             print(group_id, items)
```

### Comparing `walt-server-7/walt/server/threads/main/devices/manager.py` & `walt-server-8.0/walt/server/processes/main/devices/manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,326 +1,489 @@
-#!/usr/bin/env python
-from walt.server.threads.main.network.tools import set_static_ip_on_switch, \
-                            ip_in_walt_network, get_walt_subnet, get_server_ip
-from walt.server.threads.main.network.netsetup import NetSetup
-from walt.common.tools import format_sentence, get_mac_address
-from walt.server.tools import format_paragraph, to_named_tuple, merge_named_tuples
+import re
+
+from walt.common.formatting import columnate, format_paragraph
+from walt.common.netsetup import NetSetup
+from walt.common.tools import do, get_mac_address
 from walt.server import const
-import re, json
+from walt.server.tools import (
+    get_server_ip,
+    get_walt_subnet,
+    ip_in_walt_network,
+    merge_named_tuples,
+    to_named_tuple,
+)
 
-DEVICE_NAME_NOT_FOUND="""No device with name '%s' found.\n"""
+DEVICE_NAME_NOT_FOUND = """No device with name '%s' found.\n"""
 
 NEW_NAME_ERROR_AND_GUIDELINES = """\
 Failed: invalid new name.
 This name must be a valid network hostname.
 Only alphanumeric characters and '-' are allowed.
 The 1st character must be an alphabet letter.
 The name must be at least 2-chars long.
 (Example: rpi-D327)
 """
 
 DEVICES_QUERY = """\
-SELECT name, ip, mac,
+WITH infodev AS (SELECT name, ip, mac,
        CASE WHEN type = 'node' AND virtual THEN 'node (virtual)'
             WHEN type = 'node' AND mac like '52:54:00:%%' THEN 'node (vpn)'
             WHEN type = 'node' THEN 'node (physical)'
             ELSE type
-       END as type
-FROM devices
+       END as type,
+COALESCE((conf->'netsetup')::int, 0) as int_netsetup
+FROM devices)
+SELECT name, ip, mac, type,
+CASE WHEN int_netsetup = 0 THEN 'LAN'
+     WHEN int_netsetup = 1 THEN 'NAT'
+END as netsetup
+FROM infodev
 WHERE type %(unknown_op)s 'unknown'
 ORDER BY type, name;"""
 
 MY_NODES_QUERY = """\
 SELECT  d.mac as mac
-FROM devices d, nodes n, images i
+FROM devices d, nodes n
 WHERE   d.mac = n.mac
-AND     n.image = i.fullname
-AND     i.ready = True
 AND     split_part(n.image, '/', 1) = '%s'
 ORDER BY name;"""
 
 DEVICE_SET_QUERIES = {
-        'all-nodes': """
+    "all-nodes": """
             SELECT  d.mac as mac
-            FROM devices d, nodes n, images i
+            FROM devices d, nodes n
             WHERE   d.mac = n.mac
-            AND     n.image = i.fullname
-            AND     i.ready = True
             ORDER BY d.name;""",
-        'all-switches': """
+    "free-nodes": """
+            SELECT  d.mac as mac
+            FROM devices d, nodes n
+            WHERE   d.mac = n.mac
+            AND     n.image = ('waltplatform/' || n.model || '-default:latest')
+            ORDER BY name;""",
+    "all-switches": """
             SELECT  d.mac as mac
             FROM devices d
             WHERE   d.type = 'switch'
             ORDER BY name;""",
-        'all-devices': """
+    "all-devices": """
             SELECT  d.mac as mac
             FROM devices d
             ORDER BY type, name;""",
-        'explorable-switches': """
+    "explorable-switches": """
             SELECT  d.mac as mac
             FROM devices d
             WHERE   d.type = 'switch'
             AND     COALESCE((d.conf->'lldp.explore')::boolean, False) = True
-            ORDER BY d.name;"""
+            ORDER BY d.name;""",
 }
 
 TITLE_DEVICE_SHOW_MAIN = """\
 The WalT network contains the following devices:"""
 
 FOOTNOTE_DEVICE_SHOW_MAIN = """\
 tips:
 - use 'walt device tree' for a tree view of the network
 - use 'walt device forget <device_name>' to make WalT forget about an obsolete device"""
 
 TITLE_SOME_UNKNOWN_DEVICES = """\
 WalT also detected the following devices but could not detect their type:"""
 
 FOOTNOTE_SOME_UNKNOWN_DEVICES = """\
-If one of them is actually a switch, use 'walt device config <name> type=switch' to fix this."""
+If one of them is actually a switch,\
+ use 'walt device config <name> type=switch' to fix this."""
+
+CMD_ADD_SSH_KNOWN_HOST = (
+    "  mkdir -p /root/.ssh && ssh-keygen -F %(ip)s ||                            "
+    " ssh-keyscan -t ecdsa %(ip)s >> /root/.ssh/known_hosts"
+)
 
-class DevicesManager(object):
 
-    def __init__(self, db):
-        self.db = db
+class DevicesManager(object):
+    def __init__(self, server):
+        self.db = server.db
+        self.logs = server.logs
+        self.server_mac = get_mac_address(const.WALT_INTF)
         self.server_ip = get_server_ip()
         self.netmask = str(get_walt_subnet().netmask)
 
+    def prepare(self):
+        # prepare the network setup for NAT support
+        self.prepare_netsetup()
+
+    def cleanup(self):
+        self.cleanup_netsetup()
+
+    def get_server_mac(self):
+        return self.server_mac
+
     def validate_device_name(self, requester, name):
-        if self.get_device_info(requester, name, err_message = None) != None:
+        if self.get_device_info(requester, name, err_message=None) is not None:
             if requester is not None:
-                requester.stderr.write("""Failed: a device with name '%s' already exists.\n""" % name)
+                requester.stderr.write(
+                    """Failed: a device with name '%s' already exists.\n""" % name
+                )
             return False
-        if len(name) < 2 or not re.match('^[a-zA-Z][a-zA-Z0-9-]*$', name):
+        if len(name) < 2 or not re.match("^[a-zA-Z][a-zA-Z0-9-]*$", name):
             if requester is not None:
                 requester.stderr.write(NEW_NAME_ERROR_AND_GUIDELINES)
             return False
         return True
 
     def rename(self, requester, old_name, new_name):
         device_info = self.get_device_info(requester, old_name)
-        if device_info == None:
-            return
+        if device_info is None:
+            return False
         if not self.validate_device_name(requester, new_name):
-            return
+            return False
         # all is fine, let's update it
-        self.db.update("devices", 'mac', mac = device_info.mac, name = new_name)
+        self.db.update("devices", "mac", mac=device_info.mac, name=new_name)
         self.db.commit()
+        return True
 
     def get_type(self, mac):
         device_info = self.db.select_unique("devices", mac=mac)
         if not device_info:
             return None
         return device_info.type
 
-    def get_device_info(self, requester, device_name, \
-                        err_message = DEVICE_NAME_NOT_FOUND):
+    def get_device_info(
+        self, requester, device_name, err_message=DEVICE_NAME_NOT_FOUND
+    ):
         device_info = self.db.select_unique("devices", name=device_name)
-        if device_info == None and err_message != None and requester is not None:
+        if device_info is None and err_message is not None and requester is not None:
             requester.stderr.write(err_message % device_name)
         return device_info
 
     def get_complete_device_info(self, mac):
         device_info = self.db.select_unique("devices", mac=mac)
-        if device_info == None:
+        if device_info is None:
             return None
         device_type = device_info.type
-        if device_type == 'node':
+        if device_type == "node":
             node_info = self.db.select_unique("nodes", mac=mac)
-            if device_info.conf.get('netsetup', 0) == NetSetup.NAT:
+            # netsetup=NAT can actually be applied to all devices, not only
+            # nodes. However, considering only nodes ensures these devices
+            # will really boot in walt-net and the netmask + gateway pair
+            # will be correct. So we only expose this information to nodes.
+            if device_info.conf.get("netsetup", 0) == NetSetup.NAT:
                 gateway = self.server_ip
             else:
-                gateway = ''
+                gateway = ""
             node_info = to_named_tuple(node_info._asdict())
-            node_info = node_info.update(
-                gateway = gateway,
-                netmask = self.netmask
-            )
+            node_info = node_info.update(gateway=gateway, netmask=self.netmask)
             device_info = merge_named_tuples(device_info, node_info)
-        elif device_type == 'switch':
+        elif device_type == "switch":
             switch_info = self.db.select_unique("switches", mac=mac)
             device_info = merge_named_tuples(device_info, switch_info)
         return device_info
 
     def get_name_from_ip(self, ip):
         device_info = self.db.select_unique("devices", ip=ip)
+        if device_info is None:
+            return None
         return device_info.name
 
     def notify_unknown_ip(self, requester, device_name):
-        requester.stderr.write('Sorry, IP address of %s in unknown.\n' \
-                            % device_name)
+        requester.stderr.write("Sorry, IP address of %s in unknown.\n" % device_name)
 
     def get_device_ip(self, requester, device_name):
         device_info = self.get_device_info(requester, device_name)
-        if device_info == None:
-            return None # error already reported
-        if device_info.ip == None:
+        if device_info is None:
+            return None  # error already reported
+        if device_info.ip is None:
             self.notify_unknown_ip(requester, device_name)
         return device_info.ip
 
     def generate_device_name(self, type, mac, **kwargs):
-        if type == 'server':
-            return 'walt-server'
+        if type == "server":
+            return "walt-server"
         else:
-            prefix = "%s-%s" % (type, "".join(mac.split(':')[3:]))
+            prefix = "%s-%s" % (type, "".join(mac.split(":")[3:]))
             i = 1
             while True:
                 if i == 1:
                     name = prefix
                 else:
                     name = "%s-%d" % (prefix, i)
                 device_info = self.db.select_unique("devices", name=name)
-                if device_info == None:
+                if device_info is None:
                     # ok name does not exist in db yet
                     return name
                 else:
                     # device name already exists! Check next one.
                     i += 1
 
-    def add_or_update(self, **args_data):
-        """Return True if a new equipment (node, switch) was identified, False otherwise"""
-        if 'type' not in args_data:
-            args_data['type'] = 'unknown'
+    def add_or_update(self, requester=None, **args_data):
+        """Returns whether a new equipment (node, switch) was identified"""
+        if "type" not in args_data:
+            args_data["type"] = "unknown"
         new_equipment = False
         modified = False
-        db_data = self.db.select_unique("devices", mac=args_data['mac']);
+        newly_identified = False
+        db_data = self.db.select_unique("devices", mac=args_data["mac"])
         if db_data:
             # -- device found in db
             updates = {}
             name = db_data.name
-            if db_data.type == 'unknown' and args_data['type'] != 'unknown':
+            if db_data.type == "unknown" and args_data["type"] != "unknown":
                 # device was in db, but type was unknown.
-                if 'unknown' in db_data.name:
+                if "unknown" in db_data.name:
                     # device name has not been updated by the user,
                     # we will generate a new one more appropriate for the new type
                     name = self.generate_device_name(**args_data)
-                    updates['name'] = name
-                    if 'requester' in args_data:
-                        requester = args_data['requester']
-                        requester.stdout.write('Renaming %s to %s for clarity.\n' % (
-                            db_data.name, name
-                        ))
+                    updates["name"] = name
+                    self.logs.platform_log(
+                        "devices", f"renamed {db_data.name} to {name} for clarity"
+                    )
+                    if requester is not None:
+                        requester.stdout.write(
+                            f"Renaming {db_data.name} to {name} for clarity.\n"
+                        )
                 # now we know its type, so we consider we have a new equipment here.
                 new_equipment = True
-                print('Device: %s updating type, unknown -> %s' % (name, args_data['type']))
-                updates['type'] = args_data['type']
-            if db_data.ip is None and args_data['ip'] is not None:
-                print('Device: %s updating ip, unknown -> %s' % (name, args_data['ip']))
-                updates['ip'] = args_data['ip']
-            elif db_data.ip is not None and args_data['ip'] is not None and \
-                    not ip_in_walt_network(db_data.ip) and ip_in_walt_network(args_data['ip']):
+                newly_identified = True
+                print(
+                    "Device: %s updating type, unknown -> %s"
+                    % (name, args_data["type"])
+                )
+                updates["type"] = args_data["type"]
+            if db_data.ip is None and args_data.get("ip", None) is not None:
+                print("Device: %s updating ip, unknown -> %s" % (name, args_data["ip"]))
+                updates["ip"] = args_data["ip"]
+            elif (
+                db_data.ip is not None
+                and args_data.get("ip", None) is not None
+                and not ip_in_walt_network(db_data.ip)
+                and ip_in_walt_network(args_data["ip"])
+            ):
                 # the device updated its IP by requesting our managed DHCP server
-                print('Device: %s updating ip, %s -> %s (now in walt network)' % (name, db_data.ip, args_data['ip']))
-                updates['ip'] = args_data['ip']
+                print(
+                    "Device: %s updating ip, %s -> %s (now in walt network)"
+                    % (name, db_data.ip, args_data["ip"])
+                )
+                updates["ip"] = args_data["ip"]
             if len(updates) > 0:
                 modified = True
-                self.db.update("devices", 'mac', mac=args_data['mac'], **updates)
+                self.db.update("devices", "mac", mac=args_data["mac"], **updates)
         else:
             # device was not known in db yet
             # generate a name for this device
-            if 'name' not in args_data:
-                args_data['name'] = self.generate_device_name(**args_data)
-            print('Device: %s is new, adding (%s, %s)' % (args_data['name'], args_data['ip'], args_data['type']))
+            if "name" not in args_data:
+                args_data["name"] = self.generate_device_name(**args_data)
+            print(
+                "Device: %s is new, adding (%s, %s)"
+                % (args_data["name"], args_data["ip"], args_data["type"])
+            )
             self.db.insert("devices", **args_data)
             modified = True
-            if args_data['type'] != 'unknown':
-                new_equipment = True
+            new_equipment = True
         # if new switch or node, insert in relevant table
+        # and submit platform logline
+        # but first, refresh after prev updates
+        db_data = self.db.select_unique("devices", mac=args_data["mac"])
         if new_equipment:
-            if args_data['type'] == 'switch':
-                self.db.insert('switches', **args_data)
-            elif args_data['type'] == 'node':
-                self.db.insert('nodes', **args_data)
-        else:   # otherwise update them
-            if args_data['type'] == 'switch':
-                self.db.update('switches', 'mac', **args_data)
-            elif args_data['type'] == 'node':
-                self.db.update('nodes', 'mac', **args_data)
+            if newly_identified:
+                ident_log_line = " (device type previously unknown)"
+            else:
+                ident_log_line = ""
+            if db_data.type == "switch":
+                self.db.insert("switches", **args_data)
+                dtype = "switch"
+                details = ""
+            elif db_data.type == "node":
+                self.db.insert("nodes", **args_data)
+                dtype = "node"
+                details = f" model={args_data['model']}"
+            else:
+                dtype = "device"
+                details = f" type={db_data.type}"
+            info = f"name={db_data.name}{details} mac={db_data.mac} ip={db_data.ip}"
+            logline = f"new {dtype}{ident_log_line} {info}"
+            self.logs.platform_log("devices", logline)
+        else:  # otherwise update them
+            if db_data.type == "switch":
+                self.db.update("switches", "mac", **args_data)
+            elif db_data.type == "node":
+                self.db.update("nodes", "mac", **args_data)
         if modified:
             self.db.commit()
         return new_equipment
 
+    def show_device_table(self, unknown_or_not):
+        unknown_op = "=" if unknown_or_not else "!="
+        q = DEVICES_QUERY % dict(unknown_op=unknown_op)
+        rows, header = self.db.pretty_print_select_info(q)
+        # Do no print the netsetup status for the server
+        # or devices outside walt-net
+        idx_type = header.index("type")
+        idx_ip = header.index("ip")
+        idx_netsetup = header.index("netsetup")
+        fixed_rows = []
+        for row in rows:
+            if (
+                row[idx_type] == "server"
+                or row[idx_ip] is None
+                or not ip_in_walt_network(row[idx_ip])
+            ):
+                row = list(row)  # for assignment, it was a tuple
+                row[idx_netsetup] = ""
+            fixed_rows.append(row)
+        return columnate(fixed_rows, header)
+
     def show(self):
-        q = DEVICES_QUERY % dict(unknown_op = '!=')
         msg = format_paragraph(
-                TITLE_DEVICE_SHOW_MAIN,
-                self.db.pretty_printed_select(q),
-                FOOTNOTE_DEVICE_SHOW_MAIN)
-        unknown_devices = self.db.select('devices', type='unknown')
+            TITLE_DEVICE_SHOW_MAIN,
+            self.show_device_table(False),
+            FOOTNOTE_DEVICE_SHOW_MAIN,
+        )
+        unknown_devices = self.db.select("devices", type="unknown")
         if len(unknown_devices) > 0:
-            q = DEVICES_QUERY % dict(unknown_op = '=')
             msg += format_paragraph(
-                        TITLE_SOME_UNKNOWN_DEVICES,
-                        self.db.pretty_printed_select(q),
-                        FOOTNOTE_SOME_UNKNOWN_DEVICES)
+                TITLE_SOME_UNKNOWN_DEVICES,
+                self.show_device_table(True),
+                FOOTNOTE_SOME_UNKNOWN_DEVICES,
+            )
         return msg
 
-    def includes_devices_not_owned(self, requester, device_set, warn):
-        username = requester.get_username()
-        if not username:
-            return False    # client already disconnected, give up
-        devices = self.parse_device_set(requester, device_set)
-        if devices is None:
-            return None
-        not_owned = [d for d in devices
-                     if not (d.type == "node" and
-                             (d.image.startswith(username + '/') or d.image.startswith('waltplatform/'))
-                             or d.type != "node")]
-        if len(not_owned) == 0:
-            return False
-        else:
-            if warn:
-                requester.stderr.write(format_sentence(
-                    'Warning: %s seems(seem) to be used by another(other) user(users).',
-                    [d.name for d in not_owned], "No device", "Device", "Devices") + '\n')
-            return True
-
-    def parse_device_set(self, requester, device_set, allow_empty=False):
-        if ',' in device_set:
-            devices = []
-            for subset in device_set.split(','):
-                subset_devices = self.parse_device_set(requester, subset, True)
+    def parse_device_set(
+        self, requester, device_set, allowed_device_set=None, allow_empty=False
+    ):
+        devices = []
+        if "," in device_set:
+            for subset in device_set.split(","):
+                subset_devices = self.parse_device_set(
+                    requester, subset, allow_empty=True
+                )
                 if subset_devices is None:
                     return None
                 devices += subset_devices
-            return devices
-        elif device_set == 'server':
-            server_mac = get_mac_address(const.WALT_INTF)
-            # register the server in the device list, if missing
-            self.add_or_update(
-                    mac = server_mac, ip = str(get_server_ip()),
-                type = 'server')
-            return [self.get_complete_device_info(server_mac)]
+        elif device_set == "server":
+            devices = [self.get_complete_device_info(self.server_mac)]
         else:
             username = requester.get_username()
             if not username:
-                return None    # client already disconnected, give up
+                return None  # client already disconnected, give up
             # check keywords
             sql = None
-            if device_set is None or device_set == 'my-nodes':
+            if device_set is None or device_set == "my-nodes":
                 sql = MY_NODES_QUERY % username
             elif device_set in DEVICE_SET_QUERIES:
                 sql = DEVICE_SET_QUERIES[device_set]
             if sql is not None:
                 # retrieve devices from database
                 device_macs = [record[0] for record in self.db.execute(sql)]
             else:
                 # otherwise a specific device is requested by name
                 dev_name = device_set
                 dev_info = self.get_device_info(requester, dev_name)
                 if dev_info is None:
                     return None
-                device_macs = [ dev_info.mac ]
+                device_macs = [dev_info.mac]
             # get complete devices info
             devices = [self.get_complete_device_info(mac) for mac in device_macs]
-            if len(devices) == 0 and not allow_empty:
-                requester.stderr.write('No matching devices found! (tip: walt help show node-terminology)\n')
-                return None
-            return sorted(devices)
+        # verify selected devices are allowed
+        if allowed_device_set is not None:
+            allowed_dev_names = set(
+                d.name for d in self.parse_device_set(requester, allowed_device_set)
+            )
+            for d in devices:
+                if d.name not in allowed_dev_names:
+                    requester.stderr.write(
+                        f"Invalid value '{device_set}'; allowed devices belong to"
+                        f" '{allowed_device_set}'\n"
+                    )
+                    return None
+        if len(devices) == 0 and not allow_empty:
+            requester.stderr.write(
+                "No matching devices found! (tip: walt help show node-ownership)\n"
+            )
+            return None
+        return sorted(devices)
 
     def as_device_set(self, names):
-        return ','.join(sorted(names))
+        return ",".join(sorted(names))
 
     def develop_device_set(self, requester, device_set):
         devices = self.parse_device_set(requester, device_set)
         if devices is None:
             return None
         return self.as_device_set(d.name for d in devices)
+
+    def get_connectivity_info(self, device_mac):
+        # we look for a record where mac1 or mac2 equals device_mac
+        records = list(self.db.select("topology", mac1=device_mac))
+        records += list(self.db.select("topology", mac2=device_mac))
+        if len(records) != 1:
+            return (None, None)
+        record = records[0]
+        if record.mac1 == device_mac:
+            switch_mac, switch_port = record.mac2, record.port2
+        else:
+            switch_mac, switch_port = record.mac1, record.port1
+        switch_info = self.get_complete_device_info(switch_mac)
+        return switch_info, switch_port
+
+    def prepare_netsetup(self):
+        # force-create the chain WALT and assert it is empty
+        do("iptables --new-chain WALT")
+        do("iptables --flush WALT")
+        do("iptables --append WALT --jump DROP")
+        # allow traffic on the bridge (virtual <-> physical nodes)
+        do(
+            "iptables --append FORWARD "
+            "--in-interface walt-net --out-interface walt-net "
+            "--jump ACCEPT"
+        )
+        # allow connections back to WalT
+        do(
+            "iptables --append FORWARD "
+            "--out-interface walt-net --match state --state RELATED,ESTABLISHED "
+            "--jump ACCEPT"
+        )
+        # jump to WALT chain for other traffic
+        do("iptables --append FORWARD --in-interface walt-net --jump WALT")
+        # NAT nodes traffic that is allowed to go outside
+        do(
+            "iptables --table nat --append POSTROUTING "
+            "! --out-interface walt-net --source %s "
+            "--jump MASQUERADE"
+            % str(get_walt_subnet())
+        )
+        # Set the configuration of all NAT-ed devices
+        for device_info in self.db.execute("""\
+                SELECT ip FROM devices
+                WHERE COALESCE((conf->'netsetup')::int, 0) = %d;
+                """ % NetSetup.NAT):
+            do("iptables --insert WALT --source '%s' --jump ACCEPT" % device_info.ip)
+
+    def cleanup_netsetup(self):
+        # drop rules set by prepare_netsetup
+        do(
+            "iptables --table nat --delete POSTROUTING "
+            "! --out-interface walt-net --source %s "
+            "--jump MASQUERADE"
+            % str(get_walt_subnet())
+        )
+        do("iptables --delete FORWARD --in-interface walt-net --jump WALT")
+        do(
+            "iptables --delete FORWARD "
+            "--out-interface walt-net --match state --state RELATED,ESTABLISHED "
+            "--jump ACCEPT"
+        )
+        do(
+            "iptables --delete FORWARD "
+            "--in-interface walt-net --out-interface walt-net "
+            "--jump ACCEPT"
+        )
+        do("iptables --flush WALT")
+        do("iptables --delete-chain WALT")
+
+    def prepare_ssh_access_for_ip(self, ip):
+        cmd = CMD_ADD_SSH_KNOWN_HOST % dict(ip=ip)
+        do(cmd, shell=True)
+
+    def prepare_ssh_access(self, requester, device_set):
+        devices = self.parse_device_set(requester, device_set)
+        if devices is None:
+            return
+        for device in devices:
+            self.prepare_ssh_access_for_ip(device.ip)
```

### Comparing `walt-server-7/walt/server/threads/main/exports.py` & `walt-server-8.0/walt/server/processes/main/exports.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 from walt.common.tools import failsafe_makedirs
-from walt.server.threads.main.network.tools import get_walt_subnet
-from walt.server.threads.main.network import nfs, nbfs
+from walt.server.processes.main.network import nbfs
+from walt.server.processes.main.network.nfs import NFSExporter
+from walt.server.tools import get_walt_subnet
 
-PERSISTENT_PATH = "/var/lib/walt/nodes/%(node_mac)s/persist"
+PERSISTENT_PATH = "/var/lib/walt/nodes/%(node_mac)s/persist_dir"
 
-def get_fsid(image):
-    return image.image_id[:32]   # 32 first characters
 
-def get_exports_info(images, nodes):
-    # compute the set of root filesystem images
-    # note: we may have duplicate images refering to the same
-    # mountpoint, we should export them only once.
-    root_paths = {}
-    for image in images:
-        if image.ready and image.mounted and image.mount_path not in root_paths:
-            root_paths[image.mount_path] = get_fsid(image)
-    # compute persistent node directories
-    persist_paths = []
-    for node in nodes:
-        persist_path = PERSISTENT_PATH % dict(node_mac=node.mac)
-        # ensure directory exists
-        failsafe_makedirs(persist_path)
-        persist_paths.append(persist_path)
-    return root_paths, persist_paths
-
-def update_exported_filesystems(images, nodes):
-    subnet = get_walt_subnet()
-    root_paths, persist_paths = get_exports_info(images, nodes)
-    nfs.update_exports(root_paths.items(), persist_paths, subnet)
-    nbfs.update_exports(root_paths.keys(), subnet)
+class FilesystemsExporter:
+    def __init__(self, evloop):
+        self.nfs = NFSExporter(evloop)
+        self.nbfs = nbfs
+
+    def get_fsid(self, image_id):
+        return image_id[:32]  # 32 first characters
+
+    def get_exports_info(self, images_info, nodes):
+        # compute the root filesystems of given images
+        root_paths = {
+            mount_path: self.get_fsid(image_id)
+            for (image_id, mount_path) in images_info
+        }
+        # compute persistent node directories
+        persist_paths = []
+        for node in nodes:
+            persist_path = PERSISTENT_PATH % dict(node_mac=node.mac)
+            # ensure directory exists
+            failsafe_makedirs(persist_path)
+            persist_paths.append(persist_path)
+        return root_paths, persist_paths
+
+    def wf_update_exported_filesystems(self, wf, images_info, nodes, **env):
+        subnet = get_walt_subnet()
+        root_paths, persist_paths = self.get_exports_info(images_info, nodes)
+        root_paths = list(root_paths.items())
+        self.nbfs.update_exports(root_paths, subnet)
+        wf.update_env(root_paths=root_paths, persist_paths=persist_paths, subnet=subnet)
+        wf.insert_steps([self.nfs.wf_update_exports])
+        wf.next()
```

### Comparing `walt-server-7/walt/server/threads/main/hub.py` & `walt-server-8.0/walt/server/processes/main/hub.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-from walt.server.threads.main.apisession import APISession
-from walt.common.thread import RPCThreadConnector
-from walt.server.threads.main.api.cs import CSAPI
-from walt.server.threads.main.api.ns import NSAPI
-from walt.server.threads.main.api.vs import VSAPI
-from walt.server.threads.main.api.ss import SSAPI
+from walt.server.process import RPCProcessConnector
+from walt.server.processes.main.api.cs import CSAPI
+from walt.server.processes.main.api.ns import NSAPI
+from walt.server.processes.main.api.ss import SSAPI
+from walt.server.processes.main.api.vs import VSAPI
+from walt.server.processes.main.apisession import APISession
 
-class ServiceToHubThread(object):
+
+class ServiceToHubProcess(object):
     def __init__(self, hub_rpc, server):
         self.hub_rpc = hub_rpc
         self.server = server
-    def create_session(self, rpc_context, target_api, remote_ip):
-        return APISession.create(
-            self.server, target_api, remote_ip)
+
     def destroy_session(self, rpc_context, session_id):
         APISession.destroy(session_id)
-    def run_task(self, rpc_context, session_id, attr, args, kwargs):
-        session = APISession.get(session_id)
-        session.run_task(rpc_context, attr, args, kwargs)
 
-class HubRPCThreadConnector(RPCThreadConnector):
+    def run_task(
+        self, rpc_context, session_id, target_api, remote_ip, attr, args, kwargs
+    ):
+        session = APISession.get(self.server, session_id, target_api, remote_ip)
+        return session.run_task(rpc_context, attr, args, kwargs)
+
+
+class HubRPCProcessConnector(RPCProcessConnector):
     def __init__(self, server):
-        service = ServiceToHubThread(self, server)
-        RPCThreadConnector.__init__(self, service)
+        service = ServiceToHubProcess(self, server)
+        RPCProcessConnector.__init__(self, service, label="main-to-hub")
 
-APISession.register_target_api('NSAPI', NSAPI)
-APISession.register_target_api('VSAPI', VSAPI)
-APISession.register_target_api('CSAPI', CSAPI)
-APISession.register_target_api('SSAPI', SSAPI)
 
+APISession.register_target_api("NSAPI", NSAPI)
+APISession.register_target_api("VSAPI", VSAPI)
+APISession.register_target_api("CSAPI", CSAPI)
+APISession.register_target_api("SSAPI", SSAPI)
```

### Comparing `walt-server-7/walt/server/threads/main/images/fixowner.py` & `walt-server-8.0/walt/server/processes/main/images/fixowner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,71 @@
+from __future__ import annotations
 
-MSG_SAME_USER="""\
+import typing
+
+if typing.TYPE_CHECKING:
+    from walt.server.processes.main.registry import WalTLocalRegistry
+
+MSG_SAME_USER = """\
 Invalid username. According to your walt.conf file, you are '%s'!
 """
 
-MSG_IN_USE="""\
+MSG_IN_USE = """\
 Cannot proceed because some images of %s are in use:
 %s
 """
 
-MSG_OVERWRITING="""\
+MSG_OVERWRITING = """\
 Cannot proceed because the following images of %s would overwrite
 those with the same name in your working set:
 %s
 """
 
-MSG_NO_SUCH_USER="""\
+MSG_NO_SUCH_USER = """\
 Connot find any images belonging to a user with name '%s'.
 Make sure you typed it correctly.
 """
 
-MSG_CHANGED_OWNER="""\
+MSG_CHANGED_OWNER = """\
 Image %s now belongs to you.
 """
 
-def fix_owner(images, docker, requester, other_user):
+
+def fix_owner(images, registry: WalTLocalRegistry, requester, other_user):
     username = requester.get_username()
     if not username:
-        return None     # client already disconnected, give up
+        return None  # client already disconnected, give up
     if username == other_user:
         requester.stderr.write(MSG_SAME_USER % other_user)
         return
     in_use = set()
     candidates = set()
     for image in images.values():
         if image.user == other_user:
-            if image.in_use:
+            if image.in_use():
                 in_use.add(image.name)
             else:
                 candidates.add(image)
     if len(in_use) > 0:
-        requester.stderr.write(MSG_IN_USE % \
-                (other_user, ', '.join(in_use)))
+        requester.stderr.write(MSG_IN_USE % (other_user, ", ".join(in_use)))
         return
     problematic = set()
     for image in candidates:
-        if images.get_user_image_from_name(requester, image.name,
-                                    expected = None, ready_only = False):
+        if images.get_user_image_from_name(requester, image.name, expected=None):
             problematic.add(image.name)
     if len(problematic) > 0:
-        requester.stderr.write(MSG_OVERWRITING % \
-                (other_user, ', '.join(problematic)))
+        requester.stderr.write(MSG_OVERWRITING % (other_user, ", ".join(problematic)))
         return
     if len(candidates) == 0:
         requester.stderr.write(MSG_NO_SUCH_USER % other_user)
         return
     # ok, let's do it
     for image in candidates:
-        # rename the docker image
+        image.filesystem.close()
+        # rename the image
         old_fullname = image.fullname
-        new_fullname = username + old_fullname.split('/')[1]
-        docker.local.tag(old_fullname, new_fullname)
-        docker.local.rmi(old_fullname)
+        new_fullname = username + old_fullname.split("/")[1]
+        registry.tag(old_fullname, new_fullname)
+        registry.rmi(old_fullname)
         # update the store
         images.rename(old_fullname, new_fullname)
         requester.stdout.write(MSG_CHANGED_OWNER % image.name)
-
```

### Comparing `walt-server-7/walt/server/threads/main/images/manager.py` & `walt-server-8.0/walt/server/processes/main/images/manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,148 +1,243 @@
-from walt.server.threads.main.images.shell import ImageShellSession
-from walt.server.threads.main.images.search import search
-from walt.server.threads.main.images.clone import clone
-from walt.server.threads.main.images.publish import publish
-from walt.server.threads.main.images.squash import squash
-from walt.server.threads.main.images.metadata import update_hub_metadata
-from walt.server.threads.main.images.show import show
-from walt.server.threads.main.images.rename import rename
-from walt.server.threads.main.images.remove import remove
-from walt.server.threads.main.images.duplicate import duplicate
-from walt.server.threads.main.images.fixowner import fix_owner
-from walt.server.threads.main.images.store import NodeImageStore
-from walt.server.threads.main.network import tftp
-from walt.common.tools import format_sentence, format_sentence_about_nodes
+from __future__ import annotations
+
+import typing
+
+from walt.common.formatting import format_sentence, format_sentence_about_nodes
+from walt.common.tools import format_image_fullname
+from walt.server.processes.main.images.build import ImageBuildSession
+from walt.server.processes.main.images.clone import clone
+from walt.server.processes.main.images.duplicate import duplicate
+from walt.server.processes.main.images.fixowner import fix_owner
+from walt.server.processes.main.images.image import validate_image_name
+from walt.server.processes.main.images.metadata import update_hub_metadata
+from walt.server.processes.main.images.publish import publish
+from walt.server.processes.main.images.remove import remove
+from walt.server.processes.main.images.rename import rename
+from walt.server.processes.main.images.search import search
+from walt.server.processes.main.images.shell import ImageShellSession
+from walt.server.processes.main.images.squash import squash
+from walt.server.processes.main.images.store import NodeImageStore
+from walt.server.processes.main.images.tabular import get_tabular_data
+from walt.server.processes.main.workflow import Workflow
+
+if typing.TYPE_CHECKING:
+    from walt.server.processes.main.server import Server
 
 # About terminology: See comment about it in image.py.
 MSG_BOOT_DEFAULT_IMAGE = """\
-%s will now boot its(their) default image (other users will see it(they) is(are) 'free')."""
+%s will now boot its(their) default image \
+(other users will see it(they) is(are) 'free')."""
 MSG_INCOMPATIBLE_MODELS = """\
 Sorry, this image is not compatible with %s.
 """
 
-class NodeImageManager(object):
-    def __init__(self, db, blocking_manager, dhcpd, docker):
-        self.db = db
-        self.blocking = blocking_manager
-        self.dhcpd = dhcpd
-        self.docker = docker
-        self.store = NodeImageStore(self.docker, self.db)
+
+class NodeImageManager:
+    def __init__(self, server: Server):
+        self.server = server
+        self.db = server.db
+        self.blocking = server.blocking
+        self.dhcpd = server.dhcpd
+        self.registry = server.registry
+        self.store = NodeImageStore(server)
+
     def prepare(self):
         pass
-    def update(self, startup = False):
-        self.store.refresh(startup)
-        self.store.update_image_mounts()
-        tftp.update(self.db, self.store)
+
+    def update(self, startup=False):
+        self.store.resync_from_db()
+        self.store.trigger_update_image_mounts()
+
     def search(self, requester, task, keyword, tty_mode):
         return search(self.blocking, requester, task, keyword, tty_mode)
+
     def clone(self, **kwargs):
-        return clone(blocking = self.blocking, **kwargs)
+        return clone(blocking=self.blocking, **kwargs)
+
     def publish(self, requester, task, image_name, **kwargs):
         return publish(self.store, self.blocking, requester, task, image_name, **kwargs)
+
     def squash(self, requester, task_callback, image_name, confirmed):
-        return squash(self.store, self.blocking, requester, task_callback, image_name, confirmed)
-    def show(self, requester, refresh):
-        return show(self.db, self.docker, self.store, requester, refresh)
+        return squash(
+            self.store, self.blocking, requester, task_callback, image_name, confirmed
+        )
+
+    def get_tabular_data(self, requester, username, refresh, fields):
+        return get_tabular_data(
+            self.db, self.store, requester, username, refresh, fields
+        )
+
     def rename(self, requester, image_name, new_name):
-        rename(self.store, self.docker, requester, image_name, new_name)
+        return rename(self.store, self.registry, requester, image_name, new_name)
+
     def remove(self, requester, image_name):
-        remove(self.store, self.docker, requester, image_name)
+        return remove(self.store, self.registry, requester, image_name)
+
     def duplicate(self, requester, image_name, new_name):
-        duplicate(self.store, self.docker, requester, image_name, new_name)
+        return duplicate(self.store, self.registry, requester, image_name, new_name)
+
     def validate_cp_entity(self, requester, image_name, index, **info):
-        if image_name == 'booted-image':
+        if image_name == "booted-image":
             username = requester.get_username()
-            image_fullname = info['node_image']
+            image_fullname = info["node_image"]
             image = self.store[image_fullname]
             if image.user != username:
                 # modifying the image of others is not possible
-                requester.stderr.write('Cannot proceed because the booted image does not belong to you.\n')
-                return 'FAILED'
+                requester.stderr.write(
+                    "Cannot proceed because the booted image does not belong to you.\n"
+                )
+                return "FAILED"
             if self.store.warn_if_would_reboot_nodes(requester, image_fullname):
-                return 'NEEDS_CONFIRM'
+                return "NEEDS_CONFIRM"
         else:
             if not self.has_image(requester, image_name, False):
-                return 'FAILED'
+                return "FAILED"
             if index == 1:  # image is destination, it will be modified
                 if self.store.warn_if_would_reboot_nodes(requester, image_name):
-                    return 'NEEDS_CONFIRM'
-        return 'OK'
+                    return "NEEDS_CONFIRM"
+        return "OK"
+
+    def get_image_filesystem(self, requester, image_name):
+        image = self.store.get_user_image_from_name(requester, image_name)
+        if image is None:
+            return None
+        return image.filesystem
+
     def get_cp_entity_filesystem(self, requester, image_name, **info):
-        if image_name == 'booted-image':
-            image_fullname = info['node_image']
+        if image_name == "booted-image":
+            image_fullname = info["node_image"]
             return self.store[image_fullname].filesystem
         else:
-            return self.store.get_user_image_from_name(requester, image_name).filesystem
+            return self.get_image_filesystem(requester, image_name)
+
     def get_cp_entity_attrs(self, requester, image_name, **info):
         return dict(image_name=image_name)
+
     def fix_owner(self, requester, other_user):
-        fix_owner(self.store, self.docker, requester, other_user)
+        fix_owner(self.store, self.registry, requester, other_user)
+
     def cleanup(self):
         # un-mount images
         self.store.cleanup()
-    def has_image(self, requester, image_name, default_allowed):
-        if default_allowed and image_name == 'default':
+
+    def has_image(self, requester, image_name, default_allowed, expected=True):
+        if default_allowed and image_name == "default":
             return True
         else:
-            return self.store.get_user_image_from_name(requester, image_name) != None
+            image = self.store.get_user_image_from_name(
+                requester, image_name, expected=expected
+            )
+            return image is not None
+
     def set_image(self, requester, nodes, image_name):
+        is_default = image_name == "default"
         # if image tag is specified, let's get its fullname
-        if image_name != 'default':
+        if not is_default:
             image = self.store.get_user_image_from_name(requester, image_name)
-            if image == None:
+            if image is None:
                 return False
             image_compatible_models = set(image.get_node_models())
             node_models = set(node.model for node in nodes)
             incompatible_models = node_models - image_compatible_models
             if len(incompatible_models) > 0:
-                sentence = format_sentence(MSG_INCOMPATIBLE_MODELS, incompatible_models,
-                                None, 'node model', 'node models')
+                sentence = format_sentence(
+                    MSG_INCOMPATIBLE_MODELS,
+                    incompatible_models,
+                    None,
+                    "node model",
+                    "node models",
+                )
                 requester.stderr.write(sentence)
                 return False
-            image_fullnames = { node.mac: image.fullname for node in nodes }
+            ignored_names = set(
+                node.name for node in nodes if node.image == image.fullname
+            )
+            image_fullnames = {
+                node.mac: image.fullname
+                for node in nodes
+                if node.name not in ignored_names
+            }
         else:
+            ignored_names = set()
             image_fullnames = {}
             # since the 'default' keyword was specified, we might have to associate
             # different images depending on the type of each WalT node.
             # we compute the appropriate image fullname here.
             for node in nodes:
-                image_fullnames[node.mac] = self.store.get_default_image_fullname(node.model)
-        # let's update the database about which node is mounting what
-        for node_mac, image_fullname in image_fullnames.items():
-            self.db.update('nodes', 'mac',
-                    mac=node_mac,
-                    image=image_fullname)
-        self.store.update_image_mounts(requester = requester)
-        tftp.update(self.db, self.store)
-        self.db.commit()
-        self.dhcpd.update()
-        # inform requester
-        if image_name == 'default':
-            sentence = MSG_BOOT_DEFAULT_IMAGE
-        else:
-            sentence = '%s will now boot ' + image_name + '.'
-        requester.stdout.write(format_sentence_about_nodes(
-            sentence, [n.name for n in nodes]) + '\n')
+                image_fullname = self.store.get_default_image_fullname(node.model)
+                if node.image == image_fullname:
+                    ignored_names.add(node.name)
+                else:
+                    image_fullnames[node.mac] = image_fullname
+        ok_names = set(n.name for n in nodes if n.name not in ignored_names)
+        if len(ok_names) > 0:
+            # let's update the database about which node is mounting what
+            for node_mac, image_fullname in image_fullnames.items():
+                self.db.update("nodes", "mac", mac=node_mac, image=image_fullname)
+                self.server.nodes.powersave.handle_event(
+                    "set_image", node_mac, is_default
+                )
+            self.db.commit()
+            wf = Workflow([self.store.wf_update_image_mounts, self.dhcpd.wf_update])
+            wf.run()
+            # inform requester
+            if is_default:
+                sentence = MSG_BOOT_DEFAULT_IMAGE
+            else:
+                sentence = "%s will now boot " + image_name + "."
+            requester.stdout.write(
+                format_sentence_about_nodes(sentence, ok_names) + "\n"
+            )
+        if len(ignored_names) > 0:
+            requester.stdout.write(
+                format_sentence_about_nodes(
+                    "%s: ignored, it(they) is(are) already using this image.",
+                    ignored_names,
+                )
+                + "\n"
+            )
         return True
+
     def create_shell_session(self, requester, image_name, task_label):
         image = self.store.get_user_image_from_name(requester, image_name)
         if image is None:
             return None
         if not image.editable:
-            requester.stderr.write(('Cannot open image %(image_name)s because it has already reached its max number of layers.\n' +
-                                    '(tip: walt image squash %(image_name)s)\n') % dict(image_name = image_name))
+            requester.stderr.write(
+                (
+                    "Cannot open image %(image_name)s because it has already reached"
+                    " its max number of layers.\n"
+                    + "(tip: walt image squash %(image_name)s)\n"
+                )
+                % dict(image_name=image_name)
+            )
             return None
         if image.task_label:
-            requester.stderr.write('Cannot open image %s because a %s is already running.\n' % \
-                                    (image_name, image.task_label))
+            requester.stderr.write(
+                "Cannot open image %s because a %s is already running.\n"
+                % (image_name, image.task_label)
+            )
             return None
         session = ImageShellSession(self.store, image, task_label)
         return session
-    def update_hub_metadata(self, context, auth_conf, dh_peer, waltplatform_user):
-        update_hub_metadata(blocking = self.blocking,
-                           requester = context.requester.do_sync,
-                                task = context.task,
-                             dh_peer = dh_peer,
-                           auth_conf = auth_conf,
-                   waltplatform_user = waltplatform_user)
 
+    def update_hub_metadata(self, context, waltplatform_user):
+        return update_hub_metadata(
+            blocking=self.blocking,
+            requester=context.requester,
+            task=context.task,
+            waltplatform_user=waltplatform_user,
+        )
+
+    def create_build_session(self, requester, image_name, **info):
+        if not validate_image_name(requester, image_name):
+            return None
+        image_fullname = format_image_fullname(requester.get_username(), image_name)
+        image_overwrite = self.has_image(requester, image_name, False, expected=None)
+        if image_overwrite:
+            msg = self.store.get_image_overwrite_warning(image_fullname)
+            requester.stderr.write(msg)
+        session = ImageBuildSession(
+            self.blocking, self.store, image_fullname, image_overwrite, **info
+        )
+        return session
```

### Comparing `walt-server-7/walt/server/threads/main/images/rename.py` & `walt-server-8.0/walt/server/processes/main/images/duplicate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,29 @@
-from walt.server.threads.main.images.image import validate_image_name, format_image_fullname
+from __future__ import annotations
 
-def do_rename(images, docker, image, new_name):
+import typing
+
+from walt.common.tools import format_image_fullname
+from walt.server.processes.main.images.image import validate_image_name
+
+if typing.TYPE_CHECKING:
+    from walt.server.processes.main.registry import WalTLocalRegistry
+
+
+def do_duplicate(images, registry: WalTLocalRegistry, image, new_name):
+    image.filesystem.close()
     new_fullname = format_image_fullname(image.user, new_name)
-    # rename the docker image
-    docker.local.tag(image.fullname, new_fullname)
-    docker.local.rmi(image.fullname)
+    # add a tag to the image
+    registry.tag(image.fullname, new_fullname)
     # update the store
-    images.rename(image.fullname, new_fullname)
+    images.register_image(new_fullname)
+
 
-def rename(images, docker, requester, image_name, new_name):
+def duplicate(images, registry: WalTLocalRegistry, requester, image_name, new_name):
     if not validate_image_name(requester, new_name):
-        return
-    image = images.get_user_unused_image_from_name(requester, image_name)
-    if image:   # otherwise issue is already reported
+        return False
+    image = images.get_user_image_from_name(requester, image_name)
+    if image:  # otherwise issue is already reported
         if not images.get_user_image_from_name(requester, new_name, expected=False):
-            do_rename(images, docker, image, new_name)
-
+            do_duplicate(images, registry, image, new_name)
+            return True
+    return False
```

### Comparing `walt-server-7/walt/server/threads/main/images/shell.py` & `walt-server-8.0/walt/server/processes/main/images/shell.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,115 @@
+from __future__ import annotations
+
+import typing
 import uuid
-from walt.server.threads.main.images.image import validate_image_name, format_image_fullname
+
+from walt.common.tools import parse_image_fullname
+from walt.server.processes.main.workflow import Workflow
+
+if typing.TYPE_CHECKING:
+    from walt.server.processes.main.images.image import NodeImage
+    from walt.server.processes.main.images.store import NodeImageStore
+
 
 # About terminology: See comment about it in image.py.
 class ImageShellSession(object):
-
-    def __init__(self, images, image, task_label):
+    def __init__(self, images: NodeImageStore, image: NodeImage, task_label):
         self.images = images
-        self.docker = images.docker
+        self.registry = images.registry
         self.image = image
         self.container_name = str(uuid.uuid4())
-        self.docker_events = self.docker.local.events()
+        self.events = self.registry.events()
         self.image.task_label = task_label
 
     def get_parameters(self):
         # return an immutable object (a tuple, not a dict)
         # otherwise we will cause other RPC calls
         # default new name is to propose the same name
         # (and override the image if user confirms)
         return self.image.fullname, self.container_name, self.image.name
 
-    def save(self, requester, new_image_name, name_confirmed):
-        username = requester.get_username()
-        if not username:
-            return 'GIVE_UP'    # client already disconnected, give up
+    def save(
+        self, blocking, requester, image_fullname, name_confirmed, cb_return_status
+    ):
         # 1st step: validate new name
-        existing_image = self.images.get_user_image_from_name(
-                                        requester,
-                                        new_image_name,
-                                        expected=None)
-        if self.image.name == new_image_name:
+        if self.image.fullname == image_fullname:
             if name_confirmed:
                 pass
             else:
                 # same name for the modified image.
                 # this would overwrite the existing one.
                 # we will let the user confirm this.
-                self.images.warn_overwrite_image(requester, self.image.name)
-                return 'NAME_NEEDS_CONFIRM'
-        else:   # save as a different name
-            if existing_image:
-                requester.stderr.write('Bad name: Image already exists.\n')
-                return 'NAME_NOT_OK'
-        # verify name syntax
-        if not validate_image_name(requester, new_image_name):
-            return 'NAME_NOT_OK'
+                msg = self.images.get_image_overwrite_warning(image_fullname)
+                requester.stderr.write(msg)
+                cb_return_status("NAME_NEEDS_CONFIRM")
+                return
+        else:  # save as a different name
+            if image_fullname in self.images:
+                requester.stderr.write("Bad name: Image already exists.\n")
+                cb_return_status("NAME_NOT_OK")
+                return
         # ok, all is fine
 
         # 2nd step: save the image
-        image_fullname = format_image_fullname(username, new_image_name)
         # with the walt image cp command, the client sends a request to start a
         # container for receiving, then immediately starts to send a tar archive,
         # and then tries to commit the container through rpc commands.
         # we have to ensure here that the container was run and completed its job.
         while True:
-            event = next(self.docker_events)
-            if 'Status' not in event or 'Name' not in event:
+            event = next(self.events)
+            if "Status" not in event or "Name" not in event:
                 continue
-            if event['Status'] in ('cleanup', 'died') and event['Name'] == self.container_name:
+            if (
+                event["Status"] in ("cleanup", "died")
+                and event["Name"] == self.container_name
+            ):
                 break
-        # if we modified an image in use, umount/mount it in order to make changes
-        # available to nodes
-        need_remount = (self.image.fullname == image_fullname) and self.image.in_use
-        if need_remount:
-            self.images.umount_used_image(self.image)
-        print('committing %s...' % self.container_name)
-        self.docker.local.commit(self.container_name, image_fullname)
-        if need_remount:
-            self.images.update_image_mounts()
+        # if overriding, ensure the filesystem is not locking the image
+        if self.image.fullname == image_fullname:
+            self.image.filesystem.close()
+        fullname, username, new_image_name = parse_image_fullname(image_fullname)
+        wf = Workflow(
+            [
+                self.wf_commit_image,
+                self.wf_on_commit,
+                self.images.wf_update_image_mounts,
+                self.wf_end_image_save,
+            ],
+            requester=requester,
+            blocking=blocking,
+            cb_return_status=cb_return_status,
+            new_image_name=new_image_name,
+            image_fullname=image_fullname,
+        )
+        wf.run()
+
+    def wf_commit_image(self, wf, requester, blocking, image_fullname, **env):
+        print("committing %s..." % self.container_name)
+        blocking.commit_image(requester, wf.next, self.container_name, image_fullname)
+
+    def wf_on_commit(self, wf, result, **env):
+        wf.next()  # ignore result, success is assumed since there was no Exception
+
+    def wf_end_image_save(
+        self, wf, requester, cb_return_status, new_image_name, image_fullname, **env
+    ):
+        # inform user and return
         if self.image.fullname == image_fullname:
             # same name, we are modifying the image
-            requester.stdout.write('Image %s updated.\n' % new_image_name)
-            self.image.task_label = None
-            return 'OK_BUT_REBOOT_NODES'
+            requester.stdout.write("Image %s updated.\n" % new_image_name)
+            status = "OK_BUT_REBOOT_NODES"
         else:
             # we are saving changes to a new image, leaving the initial one
             # unchanged
-            self.images.register_image(image_fullname, True)
-            requester.stdout.write('New image %s saved.\n' % new_image_name)
-            self.image.task_label = None
-            return 'OK_SAVED'
+            requester.stdout.write("New image %s saved.\n" % new_image_name)
+            status = "OK_SAVED"
+        cb_return_status(status)
+        self.cleanup()
 
     def cleanup(self):
-        print('shell cleanup')
-        self.docker_events.close()
-        self.docker.local.stop_container(self.container_name)
-        self.image.task_label = None
-
+        if self.container_name is not None:
+            print("shell cleanup")
+            self.events.close()
+            self.registry.stop_container(self.container_name)
+            self.image.task_label = None
+            self.container_name = None
```

### Comparing `walt-server-7/walt/server/threads/main/images/spec.py` & `walt-server-8.0/walt/server/processes/main/images/spec.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,48 @@
-import os, shutil, shlex
-from walt.common.tools import read_json
-from walt.server.threads.main.network.tools import get_server_ip
-from walt.server.tools import update_template
-from walt.server.spec import get_server_features, SERVER_SPEC_PATH
-from walt.common.tools import failsafe_makedirs
+import os
+import shlex
+import shutil
+from pathlib import Path
+
 from plumbum.cmd import chroot
+from walt.common.config import load_conf
+from walt.common.tools import failsafe_makedirs
+from walt.server.spec import SERVER_SPEC_PATH, get_server_features
+from walt.server.tools import update_template
+
+IMAGE_SPEC_PATH = "/etc/walt/image.spec"
 
-IMAGE_SPEC_PATH = '/etc/walt/image.spec'
 
 def read_image_spec(image_path):
-    return read_json(image_path + IMAGE_SPEC_PATH)
+    return load_conf(Path(image_path + IMAGE_SPEC_PATH), optional=True)
+
 
 def do_chroot(mount_path, cmd):
     args = shlex.split(cmd)
-    return chroot(mount_path, *args, retcode = None).strip()
+    return chroot(mount_path, *args, retcode=None).strip()
+
 
 def enable_matching_features(mount_path, image_spec):
     try:
         server_feature_set = get_server_features()
-        image_feature_set = set(image_spec.get('features', []))
+        image_feature_set = set(image_spec.get("features", []))
         # intersection of sets
         available_feature_set = server_feature_set & image_feature_set
         for feature in available_feature_set:
-            enabling_cmd = image_spec['features'][feature]
-            print("""enabling '%s' feature by running '%s'.""" % \
-                            (feature, enabling_cmd))
+            enabling_cmd = image_spec["features"][feature]
+            print(
+                """enabling '%s' feature by running '%s'.""" % (feature, enabling_cmd)
+            )
             print(do_chroot(mount_path, enabling_cmd))
     except Exception as e:
         print("""WARNING: Caught exception '%s'""" % str(e))
 
+
 def update_templates(image_path, image_spec, template_env):
-    for template_file in image_spec.get('templates', []):
+    for template_file in image_spec.get("templates", []):
         update_template(image_path + template_file, template_env)
 
+
 def copy_server_spec_file(image_path):
-    target_path = image_path + SERVER_SPEC_PATH
+    target_path = image_path + str(SERVER_SPEC_PATH)
     failsafe_makedirs(os.path.dirname(target_path))
     shutil.copy(SERVER_SPEC_PATH, target_path)
```

### Comparing `walt-server-7/walt/server/threads/main/images/squash.py` & `walt-server-8.0/walt/server/processes/main/images/squash.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 def squash(store, blocking, requester, task_callback, image_name, confirmed):
     image = store.get_user_image_from_name(requester, image_name)
-    if image == None:
+    if image is None:
         # issue already reported, return to unblock the client
-        task_callback('FAILED')
+        task_callback("FAILED")
         return
     if image.task_label:
-        requester.stderr.write('Cannot open image %s because a %s is already running.\n' % \
-                                (image_name, image.task_label))
-        task_callback('FAILED')
+        requester.stderr.write(
+            "Cannot open image %s because a %s is already running.\n"
+            % (image_name, image.task_label)
+        )
+        task_callback("FAILED")
         return
     if not confirmed and store.warn_if_would_reboot_nodes(requester, image_name):
-        task_callback('NEEDS_CONFIRM')
+        task_callback("NEEDS_CONFIRM")
         return
-    image.task_label = 'squash process'
+    image.task_label = "squash process"
+
     def task_callback_2(res):
         image.task_label = None
         task_callback(res)
+
     return blocking.squash_image(
-                requester,
-                task_callback_2,
-                image_fullname = image.fullname)
+        requester, task_callback_2, image_fullname=image.fullname
+    )
```

### Comparing `walt-server-7/walt/server/threads/main/images/walt-log-echo` & `walt-server-8.0/walt/server/processes/main/images/walt-log-echo`

 * *Files identical despite different names*

### Comparing `walt-server-7/walt/server/threads/main/images/walt-log-tee` & `walt-server-8.0/walt/server/processes/main/images/walt-log-tee`

 * *Files identical despite different names*

### Comparing `walt-server-7/walt/server/threads/main/images/walt-net-service` & `walt-server-8.0/walt/server/processes/main/images/walt-net-service`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 #!/bin/sh
 set -e
 MSG_NO_BLINK_EXEC='/bin/blink unavailable or not executable on image'
 MSG_BLINK_FAILED='/bin/blink returned a non-zero error code'
+MSG_WALT_REBOOT_NO_EXEC='/bin/walt-reboot is not executable on image'
 
 final_root="$1"
 
+# Uncomment this for debug log in /persist
+#set -x
+#exec >> "$final_root/persist/walt-net-service.log"
+#exec 2>&1
+
 on_exit()
 {
     echo "[bg] walt-net-service exited! What happened?? Let's reboot!"
     sleep 5
     reboot -f
 }
 
@@ -28,29 +34,72 @@
 
 # pipe fd 5 to standard output of nc (we will read
 # requests from the server there)
 # pipe fd 6 to standard input of nc (we will send
 # results there)
 exec 6>$fifo_out 5<$fifo_in
 
+do_walt_reboot() {
+    cd "$final_root"
+    echo "Calling bin/walt-reboot"
+    chroot . bin/walt-reboot
+    # if we are here, this means bin/walt-reboot failed
+    # to reboot the OS.
+    echo -n "Command 'bin/walt-reboot' failed. "
+    echo "Falling back to standard 'reboot -f'."
+    cd /
+    reboot -f
+}
+
+# Caution with optional files /bin/walt-reboot & /bin/blink:
+# Tests such as
+# [ -e "$final_root/bin/walt-reboot" ]
+# will not work when these files are symlinks to an
+# absolute target, since the target path should also be
+# interpreted from the chroot.
+# Therefore
+# chroot "$final_root" [ -e "/bin/walt-reboot" ]
+# is the correct expression.
+
 # loop and handle coming requests
 while read req args <&5
 do
     # respond to server if it checks whether we are alive
     [ "$req" = "PING" ] && {
         echo OK >&6
     }
+    # respond to DMESG requests
+    [ "$req" = "DMESG" ] && {
+        echo OK >&6
+        echo >&6
+        busybox dmesg >&6
+    }
+    # respond to SHELL requests
+    [ "$req" = "SHELL" ] && {
+        echo OK >&6
+        echo >&6
+        busybox sh -i <&5 >&6 2>&1
+    }
     # reboot the node when we receive REBOOT
     [ "$req" = "REBOOT" ] && {
-        echo OK >&6
-        reboot -f
+        chroot "$final_root" [ -e "/bin/walt-reboot" ] && {
+            chroot "$final_root" [ -x "/bin/walt-reboot" ] && {
+                echo OK >&6
+                do_walt_reboot
+            } || {
+                echo KO $MSG_WALT_REBOOT_NO_EXEC >&6
+            }
+        } || {
+            echo OK >&6
+            reboot -f
+        }
     }
     # start /bin/blink [0|1] when we receive BLINK [0|1]
     [ "$req" = "BLINK" ] && {
-        [ -e "$final_root/bin/blink" ] && {
+        chroot "$final_root" [ -x "/bin/blink" ] && {
             cd "$final_root"
             chroot . bin/blink $args && {
                 # all is fine
                 echo OK >&6
             } || {
                 # /bin/blink apparently failed
                 echo KO $MSG_BLINK_FAILED >&6
```

### Comparing `walt-server-7/walt/server/threads/main/mydocker.py` & `walt-server-8.0/walt/server/processes/main/server.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,298 +1,384 @@
-from walt.common.crypto.blowfish import BlowFish
-from walt.server.tools import indicate_progress
-from walt.server.exttools import buildah, podman, skopeo, mount, umount, findmnt, docker
-from walt.server import const
-from datetime import datetime
-from subprocess import run, CalledProcessError, PIPE, Popen
-import time, re, os, sys, requests, json, itertools
-
-DOCKER_HUB_TIMEOUT=None
-DELAY_BEFORE_RETRY=3
-REGISTRY='docker.io'
-MAX_IMAGE_LAYERS = 128
-
-def parse_date(created_at):
-    # strptime does not support parsing nanosecond precision
-    # remove last 3 decimals of this number
-    created_at = re.sub(r'([0-9]{6})[0-9]*', r'\1', created_at)
-    dt = datetime.strptime(created_at, "%Y-%m-%d %H:%M:%S.%f %z %Z")
-    # remove subsecond precision (not needed)
-    dt = dt.replace(microsecond=0)
-    # convert to local time
-    return dt.astimezone().replace(tzinfo=None)
-
-# 'buildah mount' does not mount the overlay filesystem with appropriate options to allow nfs export.
-# let's fix this.
-def remount_with_nfs_export_option(mountpoint):
-    # retrieve mount info
-    json_info = findmnt('--json', mountpoint)
-    mount_info = json.loads(json_info)['filesystems'][0]
-    source = mount_info['source']
-    fstype = mount_info['fstype']
-    options = mount_info['options']
-    # add appropriate options
-    options += ',index=on,nfs_export=on'
-    # umount
-    umount(mountpoint)
-    # re-mount
-    mount('-t', fstype, '-o', options, source, mountpoint)
-
-def mount_exists(mountpoint):
-    try:
-        findmnt('--json', mountpoint)
-    except CalledProcessError:
-        return False
-    return True
-
-class DockerLocalClient:
-    def __init__(self):
-        self.names_cache = {}
-        self.metadata_cache = {}
-    def clear_name_cache(self):
-        self.names_cache = {}
-    def tag(self, old_fullname, new_fullname):
-        if self.image_exists(new_fullname):
-            # take care not making previous version of image a dangling image
-            podman.rmi('docker.io/' + new_fullname)
-        if old_fullname in self.names_cache:
-            self.names_cache[new_fullname] = self.names_cache[old_fullname]
+import re
+from pathlib import Path
+
+from walt.common.constants import WALT_SERVER_TCP_PORT
+from walt.common.devices.registry import get_device_info_from_mac
+from walt.common.formatting import format_sentence
+from walt.common.tcp import TCPServer
+from walt.common.tools import format_image_fullname, parse_image_fullname
+from walt.server import conf
+from walt.server.process import SyncRPCProcessConnector
+from walt.server.processes.main.apisession import APISession
+from walt.server.processes.main.autocomplete import shell_autocomplete
+from walt.server.processes.main.blocking import BlockingTasksManager
+from walt.server.processes.main.devices.manager import DevicesManager
+from walt.server.processes.main.images.manager import NodeImageManager
+from walt.server.processes.main.interactive import InteractionManager
+from walt.server.processes.main.logs import LogsManager
+from walt.server.processes.main.network import tftp
+from walt.server.processes.main.network.dhcpd import DHCPServer
+from walt.server.processes.main.nodes.manager import NodesManager
+from walt.server.processes.main.registry import WalTLocalRegistry
+from walt.server.processes.main.settings import SettingsManager
+from walt.server.processes.main.transfer import (
+    TransferManager,
+    format_node_to_booted_image_transfer_cmd,
+    validate_cp,
+)
+from walt.server.processes.main.unix import UnixSocketServer
+from walt.server.processes.main.vpn import VPNManager
+from walt.server.processes.main.workflow import Workflow
+
+KVM_DEV_FILE = Path("/dev/kvm")
+
+
+class Server(object):
+    def __init__(self, ev_loop):
+        self.ev_loop = ev_loop
+        self.db = SyncRPCProcessConnector(label="main-to-db")
+        self.registry = WalTLocalRegistry()
+        self.blocking = BlockingTasksManager(self)
+        self.tcp_server = TCPServer(WALT_SERVER_TCP_PORT)
+        self.logs = LogsManager(self.db, self.tcp_server, self.blocking, self.ev_loop)
+        self.devices = DevicesManager(self)
+        self.dhcpd = DHCPServer(self.db, self.ev_loop)
+        self.images = NodeImageManager(self)
+        self.interaction = InteractionManager(self.tcp_server, self.ev_loop)
+        self.unix_server = UnixSocketServer()
+        self.transfer = TransferManager(self.tcp_server, self.ev_loop)
+        self.nodes = NodesManager(self)
+        self.settings = SettingsManager(server=self)
+        self.vpn = VPNManager()
+
+    def prepare(self):
+        self.logs.prepare()
+        self.logs.catch_std_streams()
+        self.registry.prepare()
+        tftp.prepare()
+        self.tcp_server.prepare(self.ev_loop)
+        self.unix_server.prepare(self.ev_loop)
+        # ensure the dhcp server is running,
+        # otherwise the switches may have ip addresses
+        # outside the WalT network, and we will not be able
+        # to communicate with them when trying to update
+        # the topology.
+        self.dhcpd.update(force=True)
+        self.images.prepare()
+        self.devices.prepare()
+        self.nodes.prepare()
+
+    def update(self):
+        # mount images needed
+        self.images.update(startup=True)
+        # enable PoE if some ports remained off
+        self.blocking.restore_poe_on_all_ports()
+        # restores nodes setup
+        self.nodes.restore()
+
+    def cleanup(self):
+        APISession.cleanup_all()
+        tftp.cleanup(self.db)
+        self.images.cleanup()
+        self.nodes.cleanup()
+        self.devices.cleanup()
+        self.logs.logs_to_db.flush()
+
+    def get_registries(self):
+        return tuple(
+            (reg_info["label"], reg_info["description"])
+            for reg_info in conf["registries"]
+        )
+
+    def set_image(self, requester, node_set, image_tag):
+        nodes = self.nodes.parse_node_set(requester, node_set)
+        if nodes is None:
+            return False  # error already reported
+        return self.images.set_image(requester, nodes, image_tag)
+
+    def cleanup_device_name(self, name):
+        return re.sub("[^a-zA-Z0-9-]+", "-", name.split(".")[0])
+
+    def add_or_update_device(
+        self, vci="", uci="", ip=None, mac=None, name=None, **kwargs
+    ):
+        # let's try to identify this device given its mac address
+        # and/or the vci field of the DHCP request.
+        if uci.startswith("walt.node"):
+            auto_id = uci
+        elif vci.startswith("walt.node"):
+            auto_id = vci
         else:
-            self.names_cache.pop(new_fullname, None)
-        podman.tag(old_fullname, 'docker.io/' + new_fullname)
-    def rmi(self, fullname, ignore_missing = False):
-        self.untag(fullname, ignore_missing = ignore_missing)
-    def untag(self, fullname, ignore_missing = False):
-        if ignore_missing and not self.image_exists(fullname):
-            return  # nothing to do
-        # caution: we are not using "podman untag" because its behaviour is
-        # unexpected (at least in version 1.9.3: when an image has several docker tags,
-        # it removes all docker tags irrespectively of the one specified).
-        podman.rmi('docker.io/' + fullname)
-        self.names_cache.pop(fullname, None)
-    def deep_inspect(self, image_id_or_fullname):
-        podman_id = image_id_or_fullname
-        if '/' in podman_id:
-            podman_id = 'docker.io/' + podman_id
-        image_info = podman.inspect('--format',
-            '{ "labels": "{{.Labels}}", "num_layers": {{len .RootFS.Layers}}, "created_at": "{{.Created}}" }',
-            podman_id)
-        image_info = json.loads(image_info)
-        # unfortunately some recent versions of podman do not work with {{json .Labels}} format,
-        # so we parse the default format obtained with {{.Labels}}.
-        # we get a value such as "map[walt.node.models:pc-x86-64 walt.server.minversion:4]"
-        labels = image_info['labels'].split('[')[1].split(']')[0]
-        labels = { l:v for l, v in (lv.split(':') for lv in labels.split()) }
-        editable = (image_info['num_layers'] < MAX_IMAGE_LAYERS)
-        created_at = parse_date(image_info['created_at'])
-        return {
-            'labels': labels,
-            'editable': editable,
-            'created_at': created_at
-        }
-    def image_exists(self, fullname):
-        try:
-            podman.image.exists('docker.io/' + fullname)
-            return True
-        except CalledProcessError:
-            return False
-    def refresh_cache(self):
-        self.names_cache = {}
-        for line in buildah.images('--format', '{{.ID}}|{{.Name}}:{{.Tag}}',
-                                   '--filter', 'dangling=false',
-                                   '--no-trunc').splitlines():
-            sha_id, buildah_image_name = line.split('|')
-            image_id = sha_id[7:]   # because it starts with "sha256:"
-            # buildah may manage several repos, we do not need it here, discard this repo prefix
-            fullname = buildah_image_name.split('/', 1)[1]
-            if not '/' in fullname:
-                continue
-            if 'clone-temp/walt-image:' in fullname:
-                continue
-            self.names_cache[fullname] = image_id
-        old_metadata_cache = self.metadata_cache
-        self.metadata_cache = {}
-        for image_id in set(self.names_cache.values()):
-            if image_id in self.metadata_cache:
-                continue
-            if image_id in old_metadata_cache:
-                self.metadata_cache[image_id] = old_metadata_cache[image_id]
-                continue
-            self.metadata_cache[image_id] = self.get_metadata(image_id)
-    def get_images(self):
-        self.refresh_cache()
-        for fullname, image_id in self.names_cache.items():
-            if 'walt.node.models' not in self.metadata_cache[image_id]['labels']:
-                continue
-            yield fullname
-    def get_metadata(self, image_id_or_fullname):
-        if ':' in image_id_or_fullname:
-            # fullname
-            fullname = image_id_or_fullname
-            image_id = self.names_cache.get(fullname)
-            if image_id is None:
-                self.refresh_cache()
-            image_id = self.names_cache.get(fullname)
-            if image_id is None:
-                return None
+            auto_id = None
+        if auto_id is None:
+            info = get_device_info_from_mac(mac)
+            info["type"] = info.get("type", "unknown")
         else:
-            # image_id
-            image_id = image_id_or_fullname
-        metadata = self.metadata_cache.get(image_id)
-        if metadata is None:
-            metadata = dict(
-                image_id = image_id,
-                **self.deep_inspect(image_id))
-            self.metadata_cache[image_id] = metadata
-        return metadata
-    def stop_container(self, cont_name):
-        podman.rm("-f", "-i", cont_name)
-    def commit(self, cid_or_cname, dest_fullname, tool=podman, opts=()):
-        # we commit with 'docker' format to make these images compatible with
-        # older walt server versions
-        opts += ('-f', 'docker')
-        if self.image_exists(dest_fullname):
-            # take care not making previous version of image a dangling image
-            image_tempname = 'localhost/walt-commit-' + dest_fullname
-            args = opts + (cid_or_cname, image_tempname)
-            image_id = tool.commit(*args).strip()
-            tool.rm(cid_or_cname)
-            podman.rmi('-f', 'docker.io/' + dest_fullname)
-            podman.tag(image_tempname, 'docker.io/' + dest_fullname)
-            podman.rmi(image_tempname)
+            model = auto_id[10:]
+            info = {"type": "node", "model": model}
+        kwargs.update(**info)
+        if name is not None:
+            name = self.cleanup_device_name(name)
+            if self.devices.validate_device_name(None, name):
+                # name seems meaningful...
+                kwargs.update(name=name)
+        # what is the current status of this device in db?
+        db_info = self.db.select_unique("devices", mac=mac)
+        if db_info is None:
+            status = "new"
         else:
-            args = opts + (cid_or_cname, 'docker.io/' + dest_fullname)
-            image_id = tool.commit(*args).strip()
-            tool.rm(cid_or_cname)
-        self.names_cache[dest_fullname] = image_id
-    def events(self):
-        return podman.events.stream('--format', 'json', converter = (lambda line: json.loads(line)))
-    def image_mount(self, image_id, mount_path):
-        # if server daemon was killed and restarted, the mount may still be there
-        if mount_exists(mount_path):
-            return False    # nothing to do
-        cont_name = 'mount:' + image_id
-        try:
-            buildah('from', '--pull-never', '--name', cont_name, image_id)
-        except CalledProcessError:
-            print('Note: walt server was probably not stopped properly and container still exists. Going on.')
-        dir_name = buildah.mount(cont_name)
-        remount_with_nfs_export_option(dir_name)
-        mount('--bind', dir_name, mount_path)
-        return True
-    def image_umount(self, image_id, mount_path):
-        cont_name = 'mount:' + image_id
-        while True:
-            try:
-                umount(mount_path)
-                break
-            except:
-                time.sleep(0.1)
-                continue
-        buildah.umount(cont_name)
-        buildah.rm(cont_name)
-    def squash(self, image_fullname):
-        cont_name = 'squash:' + image_fullname
-        try:
-            buildah('from', '--pull-never', '--name', cont_name, image_fullname)
-        except CalledProcessError:
-            print('Note: walt server was probably not stopped properly and container still exists.')
-            print('      removing container and restarting command.')
-            buildah.rm(cont_name)
-            buildah('from', '--pull-never', '--name', cont_name, image_fullname)
-        self.commit(cont_name, image_fullname, tool=buildah, opts=('--squash',))
-
-class DockerDaemonClient:
-    def images(self):
-        for line in docker.image.ls('--format', '{{.Repository}} {{.Tag}}',
-                                    '--filter', 'dangling=false',
-                                    '--filter', 'label=walt.node.models').splitlines():
-            repo_name, tag = line.strip().split()
-            if tag == '<none>':
-                continue
-            yield repo_name + ':' + tag
-    def get_labels(self, image_fullname):
-        json_labels = docker.image.inspect('--format', '{{json .Config.Labels}}', image_fullname)
-        return json.loads(json_labels)
-    def checker(self, line):
-        if 'error' in line.lower():
-            raise Exception(line.strip())
-    def pull(self, image_fullname, requester = None):
-        label = 'Downloading %s' % image_fullname
-        stream = podman.pull.stream('docker-daemon:' + image_fullname, out_stream='stderr')
-        indicate_progress(sys.stdout, label, stream, self.checker)
-
-class DockerHubClient:
-    def checker(self, line):
-        if 'error' in line.lower():
-            raise Exception(line.strip())
-    def pull(self, image_fullname, requester = None):
-        label = 'Downloading %s' % image_fullname
-        stream = podman.pull.stream(image_fullname, out_stream='stderr')
-        indicate_progress(sys.stdout, label, stream, self.checker)
-    def login(self, dh_peer, auth_conf, requester):
-        try:
-            symmetric_key = dh_peer.symmetric_key
-            cypher = BlowFish(symmetric_key)
-            password = cypher.decrypt(auth_conf['encrypted_password'])
-            # Note: the docker hub API requires the email argument
-            # to be provided because it may be used to register a new user.
-            # Here, the user already exists, so the email will not be used.
-            podman.login(   '-u', auth_conf['username'], '--password-stdin', REGISTRY,
-                            input=password)
-        except Exception as e:
-            print(e)
-            requester.stdout.write('FAILED.\n')
+            status = db_info.type
+        # new nodes whose default image is not available yet are first recorded
+        # as simple devices of unknown type because downloading their default
+        # image may fail.
+        if status in ("new", "unknown") and kwargs["type"] == "node":
+            image_fullname = self.images.store.get_default_image_fullname(info["model"])
+            if image_fullname not in self.images.store:
+                kwargs["type"] = "unknown"
+        self.devices.add_or_update(ip=ip, mac=mac, **kwargs)
+        if status in ("new", "unknown") and info["type"] == "node":
+            # register the walt node or convert the unknown device to a walt node
+            self.nodes.register_node(mac=mac, model=info.get("model"))
+        self.dhcpd.update()
+
+    def get_device_info(self, device_mac):
+        return dict(self.devices.get_complete_device_info(device_mac)._asdict())
+
+    def rename_device(self, requester, old_name, new_name):
+        result = self.devices.rename(requester, old_name, new_name)
+        if result is True:
+            self.dhcpd.update()
+            tftp.update(self.db, self.images.store)
+        return result
+
+    def device_rescan(self, requester, task, remote_ip, device_set):
+        devices = self.devices.parse_device_set(requester, device_set)
+        if devices is None:
+            return False  # error already reported
+        # the result of the task the hub process submitted to us
+        # will not be available right now
+        task.set_async()
+
+        # function that will be called when blocking process has done the job
+        def cb(res):
+            self.dhcpd.update()
+            tftp.update(self.db, self.images.store)
+            task.return_result(res)
+
+        self.blocking.rescan_topology(
+            requester, cb, remote_ip=remote_ip, devices=devices
+        )
+
+    def forget_device(self, requester, task, device_name):
+        device = self.devices.get_device_info(requester, device_name)
+        if device is None:
+            return False
+        task.set_async()
+        # note: if it's a node and no other node uses its image,
+        # this image should be unmounted.
+        wf = Workflow(
+            [
+                self.nodes.powersave.wf_forget_device,
+                self.wf_forget_device_other_steps,
+                self.images.store.wf_update_image_mounts,
+                self.wf_unblock_client,
+            ],
+            requester=requester,
+            device=device,
+            task=task,
+        )
+        wf.run()
+
+    def wf_forget_device_other_steps(self, wf, task, device, **env):
+        self.logs.forget_device(device)
+        self.db.forget_device(device.name)
+        self.dhcpd.update()
+        wf.next()
+
+    def wf_unblock_client(self, wf, task, **env):
+        task.return_result(True)
+        wf.next()
+
+    def create_vnode(self, requester, task, name):
+        if not KVM_DEV_FILE.exists():
+            requester.stderr.write(
+                "Failed because virtualization is not enabled on server CPU"
+                f" (missing {KVM_DEV_FILE}).\n"
+            )
             return False
-        return True
-    def push(self, image_fullname, dh_peer, auth_conf, requester):
-        if not self.login(dh_peer, auth_conf, requester):
+        if not self.devices.validate_device_name(requester, name):
             return False
-        stream = podman.push.stream(image_fullname, REGISTRY + '/' + image_fullname)
-        label = 'Pushing %s' % image_fullname
-        indicate_progress(sys.stdout, label, stream, self.checker)
-        return True
-    def search(self, term):
-        results = []
-        for page in itertools.count(1):
-            url = 'https://index.docker.io/v1/search?q=%(term)s&n=100&page=%(page)s' % \
-                    dict(   term = term,
-                            page = page)
-            page_info = requests.get(url).json()
-            results += page_info['results']
-            if page_info['num_pages'] == page:
-                break
-        return results
-    def list_user_repos(self, user):
-        url = 'https://hub.docker.com/v2/repositories/%(user)s/?page_size=100' % \
-                    dict(user = user)
-        while url is not None:
-            page_info = requests.get(url).json()
-            for res in page_info['results']:
-                yield res['name']
-            url = page_info['next']
-    def list_image_tags(self, image_name):
-        url = 'https://registry.hub.docker.com/v1/repositories/%(image_name)s/tags' % \
-                    dict(image_name = image_name)
-        for elem in requests.get(url, timeout=DOCKER_HUB_TIMEOUT).json():
-            tag = requests.utils.unquote(elem['name'])
-            yield tag
-    def get_config(self, fullname):
-        print('retrieving config from hub: ' + fullname)
-        return json.loads(skopeo.inspect('--config', 'docker://docker.io/' + fullname))
-    def get_labels(self, fullname):
-        config = self.get_config(fullname)
-        if 'config' not in config:
-            print('{fullname}: unknown image config format.'.format(fullname=fullname))
-            return {}
-        if'Labels' not in config['config']:
-            print('{fullname}: image has no labels.'.format(fullname=fullname))
-            return {}
-        return config['config']['Labels']
-
-class DockerClient(object):
-    def __init__(self):
-        self.local = DockerLocalClient()
-        self.hub = DockerHubClient()
-        self.daemon = DockerDaemonClient()
-    def self_test(self):
-        return True
+        username = requester.get_username()
+        if username is None:
+            return False  # username already disconnected, give up
+        mac, ip, model = self.nodes.generate_vnode_info()
+        default_image_fullname = format_image_fullname(
+            "waltplatform", model + "-default"
+        )
+
+        def on_default_image_ready():
+            default_image_labels = self.images.store[default_image_fullname].labels
+            image_name = default_image_labels.get("walt.image.preferred-name")
+            if image_name is None:
+                # no 'preferred-name' tag, reuse name of default image
+                image_name = model + "-default"
+            user_image_fullname = format_image_fullname(username, image_name)
+            if user_image_fullname not in self.images.store:
+                self.registry.tag(default_image_fullname, user_image_fullname)
+                self.images.store.register_image(user_image_fullname)
+                requester.stdout.write(
+                    f'Default image for {model} was saved as "{image_name}" in your'
+                    " working set.\n"
+                )
+            requester.set_busy_label("Registering virtual node")
+            self.create_vnode_using_image(name, mac, ip, model, user_image_fullname)
+            requester.set_default_busy_label()
+            requester.stdout.write(
+                f'Node {name} is now booting your image "{image_name}".\n'
+            )
+            requester.stdout.write(
+                f"Use `walt node boot {name} <other-image>` if needed.\n"
+            )
+
+        if default_image_fullname not in self.images.store:
+            requester.set_busy_label(f'Downloading default image for "{model}"')
+            task.set_async()
+
+            def callback(pull_result):
+                if pull_result[0]:
+                    on_default_image_ready()
+                    task.return_result(True)
+                else:
+                    failure = pull_result[1]
+                    requester.stderr.write(failure + "\n")
+                    task.return_result(False)
+
+            self.blocking.pull_image(requester, default_image_fullname, callback)
+        else:
+            on_default_image_ready()
+            return True
+
+    def create_vnode_using_image(self, name, mac, ip, model, image_fullname):
+        # declare node in db
+        self.devices.add_or_update(
+            type="node", model=model, ip=ip, mac=mac, name=name, virtual=True
+        )
+        self.nodes.register_node(mac=mac, model=model, image_fullname=image_fullname)
+        # start background vm
+        # note: create_vnode_using_image() is called after the default image
+        # is downloaded, so we know register_node() completed its process
+        # synchronously and we can proceed with the following steps.
+        node = self.devices.get_complete_device_info(mac)
+        self.nodes.start_vnode(node)
+
+    def remove_vnode(self, requester, task, name):
+        info = self.nodes.get_virtual_node_info(requester, name)
+        if info is None:
+            return False  # error already reported
+        self.nodes.forget_vnode(info.mac)
+        return self.forget_device(requester, task, name)
+
+    def reboot_nodes_after_image_change(self, requester, task_callback, image_fullname):
+        nodes = self.nodes.get_nodes_using_image(image_fullname)
+        if len(nodes) == 0:
+            # nothing to do
+            task_callback("OK")
+            return
+        requester.stdout.write(
+            format_sentence(
+                "Trying to reboot %s using this image...\n",
+                [n.name for n in nodes],
+                None,
+                "node",
+                "nodes",
+            )
+        )
+        self.nodes.reboot_nodes(requester, task_callback, nodes, False)
+
+    def image_shell_session_save(
+        self, requester, cb_return, session, image_fullname, name_confirmed
+    ):
+        def cb_handle_return_status(status):
+            if status == "OK_BUT_REBOOT_NODES":
+
+                def cb_reboot(res):
+                    return cb_return("OK_SAVED")
+
+                self.reboot_nodes_after_image_change(
+                    requester, cb_reboot, image_fullname
+                )
+            else:
+                cb_return(status)
+
+        session.save(
+            self.blocking,
+            requester,
+            image_fullname,
+            name_confirmed,
+            cb_handle_return_status,
+        )
+
+    def squash_image(self, requester, task, image_name, confirmed):
+        task.set_async()
+
+        def task_callback(status):
+            if status == "OK_BUT_REBOOT_NODES":
+                image_fullname = format_image_fullname(
+                    requester.get_username(), image_name
+                )
+
+                def task_callback_2(res):
+                    return task.return_result("OK")
+
+                self.reboot_nodes_after_image_change(
+                    requester, task_callback_2, image_fullname
+                )
+            else:
+                task.return_result(status)
+
+        return self.images.squash(
+            requester=requester,
+            task_callback=task_callback,
+            image_name=image_name,
+            confirmed=confirmed,
+        )
+
+    def validate_cp(self, requester, image_or_node_label, src, dst):
+        return validate_cp(image_or_node_label, self, requester, src, dst)
+
+    def node_cp_to_booted_image(
+        self, requester, task, api_session, node_name, **path_info
+    ):
+        node_info = self.nodes.get_node_info(requester, node_name)
+        if node_info is None:
+            return  # error already reported
+        fullname, username, image_name = parse_image_fullname(node_info.image)
+        session = self.images.create_shell_session(
+            requester, image_name, "file transfer"
+        )
+        if session is None:
+            return  # issue already reported
+        # ensure session.cleanup() will be called when client disconnects
+        api_session.register_session_object(session)
+        cmd = format_node_to_booted_image_transfer_cmd(
+            node_ip=node_info.ip,
+            image_fullname=fullname,
+            container_name=session.container_name,
+            **path_info,
+        )
+        task.set_async()
+
+        # callbacks that will be called when blocking process has done the job
+        def cb_unblock_client(res):
+            task.return_result(None)
+
+        def cb(res):
+            requester.set_default_busy_label()
+            self.image_shell_session_save(
+                requester, cb_unblock_client, session, fullname, True
+            )
+
+        requester.set_busy_label("Transfering")
+        self.blocking.run_shell_cmd(requester, cb, cmd, shell=True)
+
+    def shell_autocomplete(self, requester, username, argv, debug=False):
+        return shell_autocomplete(self, requester, username, argv, debug=debug)
```

### Comparing `walt-server-7/walt/server/threads/main/network/nbfs.py` & `walt-server-8.0/walt/server/processes/main/network/nbfs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,53 @@
+import os
+import signal
 from pathlib import Path
-import os, signal
+
 from walt.server.spec import server_has_feature
 
-NBFSD_PID_PATH = Path('/var/lib/nbfs/nbfsd.pid')
-NBFS_EXPORTS_PATH = Path('/etc/nbfs/exports')
+NBFSD_PID_PATH = Path("/var/lib/nbfs/nbfsd.pid")
+NBFS_EXPORTS_PATH = Path("/etc/nbfs/exports.d/walt.exports")
 
 IMAGE_EXPORT_PATTERN = """\
-%(image_mountpoint)s %(walt_subnet)s
+%(image_mountpoint)s %(walt_subnet)s(fsid=%(fsid)s)
 """
 
-def generate_exports_file(root_paths, subnet):
-    NBFS_EXPORTS_PATH.parent.mkdir(parents=True, exist_ok=True)
+
+def generate_exports_file_content(root_paths, subnet):
     lines = [
         "# WALT nbfs exports: this file is automatically generated.\n",
         "# Root filesystem images\n",
     ]
-    for root_path in root_paths:
-        lines.append(IMAGE_EXPORT_PATTERN % dict(
-                image_mountpoint=root_path,
-                walt_subnet=subnet))
-    NBFS_EXPORTS_PATH.write_text(''.join(lines))
+    for root_path, fsid in sorted(root_paths):
+        lines.append(
+            IMAGE_EXPORT_PATTERN
+            % dict(image_mountpoint=root_path, walt_subnet=subnet, fsid=fsid)
+        )
+    return "".join(lines)
+
 
 def get_nbfsd_pid():
     try:
         pid = int(NBFSD_PID_PATH.read_text())
-        os.kill(pid, 0)    # signum = 0: check if process still exists
+        os.kill(pid, 0)  # signum = 0: check if process still exists
         return pid
-    except:
+    except Exception:
         return None
 
+
 def update_exports(root_paths, subnet):
-    if server_has_feature('nbfs'):
-        generate_exports_file(root_paths, subnet)
+    if server_has_feature("nbfs"):
+        NBFS_EXPORTS_PATH.parent.mkdir(parents=True, exist_ok=True)
+        if NBFS_EXPORTS_PATH.exists():
+            prev_content = NBFS_EXPORTS_PATH.read_text()
+        else:
+            prev_content = ""
+        content = generate_exports_file_content(root_paths, subnet)
+        if content == prev_content:  # no changes
+            return
+        NBFS_EXPORTS_PATH.write_text(content)
         nbfsd_pid = get_nbfsd_pid()
         if nbfsd_pid is None:
             # nbfsd probably not installed or running
             return
         # notify nbfsd it should re-read its exports file
         os.kill(nbfsd_pid, signal.SIGHUP)
```

### Comparing `walt-server-7/walt/server/threads/main/network/waltvlanconf.py` & `walt-server-8.0/walt/server/processes/main/network/waltvlanconf.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 #!/usr/bin/env python
-from walt.server.threads.main.snmp.vlan import PortConfig, SwitchConfig
+from walt.server.processes.main.snmp.vlan import PortConfig, SwitchConfig
+
 
 def configure_main_switch_if_needed(snmp_proxy):
-    if snmp_proxy.vlan.vlan_exists('walt-out'):
-        print('the main switch is already configured')
-        return False    # already configured
+    if snmp_proxy.vlan.vlan_exists("walt-out"):
+        print("the main switch is already configured")
+        return False  # already configured
     else:
-        print('configuring the main switch...')
+        print("configuring the main switch...")
         config = SwitchConfig()
-        config.register_vlan(1, 'walt')
-        config.register_vlan(169, 'walt-out')
+        config.register_vlan(1, "walt")
+        config.register_vlan(169, "walt-out")
         config.add_port_config(PortConfig(1).access(169))
-        config.add_port_config(PortConfig(2).trunk([1,169]))
+        config.add_port_config(PortConfig(2).trunk([1, 169]))
         # other ports keep their default config (access mode, vlan 1)
         snmp_proxy.vlan.apply_config_to_device(config)
         return True
-
-
```

### Comparing `walt-server-7/walt/server/threads/main/nodes/clock.py` & `walt-server-8.0/walt/server/processes/main/nodes/clock.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 from time import time
 
+
 class NodesClockSyncInfo:
-    """ Walt nodes bootup synchronization handler.
+    """Walt nodes bootup synchronization handler.
 
-        walt nodes get approximate time synchronization at
-        bootup by requesting a unix timestamp from the server.
-        It is of course possible (and recommended) to install a
-        more precise synchronization protocol (preferably PTP)
-        into the image.
+    walt nodes get approximate time synchronization at
+    bootup by requesting a unix timestamp from the server.
+    It is of course possible (and recommended) to install a
+    more precise synchronization protocol (preferably PTP)
+    into the image.
     """
+
     def __init__(self, ev_loop):
         self.ev_loop = ev_loop
         self.tasks = {}
 
     def sync(self, task):
         # busybox can set date with only 1-second granularity,
         # so we wait until next second change before returning result.
-        task.set_async()   # result will be available later
+        task.set_async()  # result will be available later
         task_id = id(task)
         self.tasks[task_id] = task
         # compute time of next second change
-        target_ts = int(time() + 1)     # round to next int
+        target_ts = int(time() + 1)  # round to next int
         # plan event to be recalled at this time
         self.ev_loop.plan_event(
-            ts = target_ts,
-            target = self,
-            task_id = task_id,
-            target_ts = target_ts
+            ts=target_ts, target=self, task_id=task_id, target_ts=target_ts
         )
 
     def handle_planned_event(self, task_id, target_ts):
         # return timestamp and unblock the node
         self.tasks[task_id].return_result(target_ts)
         # cleanup
         del self.tasks[task_id]
```

### Comparing `walt-server-7/walt/server/threads/main/nodes/expose.py` & `walt-server-8.0/walt/server/processes/main/nodes/expose.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,79 +1,89 @@
 #!/usr/bin/env python
-import socket
 from walt.common.io import read_and_copy
-from walt.common.tcp import read_pickle, Requests, client_sock_file
+from walt.common.tcp import Requests, client_sock_file, read_pickle
+
 
 class NodeExposeFeedbackListener:
     def __init__(self, env):
         self.env = env
+
     # let the event loop know what we are reading on
     def fileno(self):
         return self.env.node_sock_file.fileno()
+
     # when the event loop detects an event for us, this means
     # the node wrote something on the socket
     # we just have to copy this to the user socket
     def handle_event(self, ts):
-        return read_and_copy(
-                self.env.node_sock_file, self.env.client_sock_file)
+        return read_and_copy(self.env.node_sock_file, self.env.client_sock_file)
+
     def close(self):
         self.env.close()
 
+
 class NodeExposeSocketListener:
     REQ_ID = Requests.REQ_TCP_TO_NODE
+
     def __init__(self, ev_loop, sock_file, **kwargs):
         self.ev_loop = ev_loop
         self.node_ip_and_port = None
         self.client_sock_file = sock_file
         self.node_sock_file = None
+
     def open_channel_to_node(self):
         return client_sock_file(*self.node_ip_and_port)
+
     def start(self):
         try:
             self.node_sock_file = self.open_channel_to_node()
-        except:
-            self.client_sock_file.write(('Could not connect to %s:%d!\n' % \
-                                    self.node_ip_and_port).encode('utf-8'))
-            return False    # we should close
+        except Exception:
+            self.client_sock_file.write(
+                ("Could not connect to %s:%d!\n" % self.node_ip_and_port).encode(
+                    "utf-8"
+                )
+            )
+            return False  # we should close
         # create a new listener on the event loop for reading
         # what the node outputs
         feedback_listener = NodeExposeFeedbackListener(self)
         self.ev_loop.register_listener(feedback_listener)
-        self.client_sock_file.write(b'OK\n')
+        self.client_sock_file.write(b"OK\n")
+
     # let the event loop know what we are reading on
     def fileno(self):
         if self.client_sock_file.closed:
             return None
         return self.client_sock_file.fileno()
+
     # handle_event() will be called when the event loop detects
     # new input data for us.
     def handle_event(self, ts):
-        if self.node_ip_and_port == None:
+        if self.node_ip_and_port is None:
             # we did not get the parameters yet, let's do it
             params = read_pickle(self.client_sock_file)
-            if params == None:
-                self.close()    # issue
+            if params is None:
+                self.close()  # issue
                 return False
-            self.node_ip_and_port = (params['node_ip'], params['node_port'])
+            self.node_ip_and_port = (params["node_ip"], params["node_port"])
             # we now have all info to connect to the node
             return self.start()
         else:
             # otherwise we are all set. Thus, getting input data means
             # data was sent on the other end.
-            return read_and_copy(
-                self.client_sock_file, self.node_sock_file)
+            return read_and_copy(self.client_sock_file, self.node_sock_file)
+
     def close(self):
         if self.client_sock_file:
             self.client_sock_file.close()
             self.client_sock_file = None
         if self.node_sock_file:
             self.node_sock_file.close()
             self.node_sock_file = None
 
+
 class ExposeManager(object):
     def __init__(self, tcp_server, ev_loop):
-        for cls in [ NodeExposeSocketListener ]:
+        for cls in [NodeExposeSocketListener]:
             tcp_server.register_listener_class(
-                    req_id = cls.REQ_ID,
-                    cls = cls,
-                    ev_loop = ev_loop)
-
+                req_id=cls.REQ_ID, cls=cls, ev_loop=ev_loop
+            )
```

### Comparing `walt-server-7/walt/server/threads/main/nodes/netservice.py` & `walt-server-8.0/walt/server/processes/main/nodes/netservice.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,115 +1,117 @@
-import socket, errno
-from time import time
+import errno
+import socket
 from collections import defaultdict
+from time import time
+
 from walt.common.evloop import POLL_OPS_READ, POLL_OPS_WRITE
 from walt.server.const import WALT_NODE_NET_SERVICE_PORT
 
 NODE_REQUEST_DELAY_SECS = 15.0
 
+
 class REQUEST_STATUS:
     INIT = 0
     CONNECTING = 1
     WAITING_RESPONSE = 2
     DONE = 3
 
+
 def non_blocking_connect(sock, ip, port):
     try:
         sock.connect((ip, port))
     except BlockingIOError as e:
         if e.errno == errno.EINPROGRESS:
-            pass    # ok, ignore
+            pass  # ok, ignore
         else:
-            raise   # unexpected, raise
+            raise  # unexpected, raise
+
 
 class ServerToNodeRequest:
     def __init__(self, ev_loop, node, req, cb, env):
         self.ev_loop = ev_loop
         self.node = node
         self.req = req
         self.cb = cb
         self.env = env
         self.sock = None
         self.status = REQUEST_STATUS.INIT
+
     def run(self):
         self.sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         # connect call should not block, thus we use non-blocking mode
         # and let the event loop recall us when we can *write* on the socket
-        self.sock.setblocking(False)    # connect call should not block
+        self.sock.setblocking(False)  # connect call should not block
         non_blocking_connect(self.sock, self.node.ip, WALT_NODE_NET_SERVICE_PORT)
         self.status = REQUEST_STATUS.CONNECTING
         self.ev_loop.register_listener(self, POLL_OPS_WRITE)
         # we also set a timeout on the event loop
         timeout_at = time() + NODE_REQUEST_DELAY_SECS
-        self.ev_loop.plan_event(
-            ts = timeout_at,
-            callback = self.on_timeout
-        )
+        self.ev_loop.plan_event(ts=timeout_at, callback=self.on_timeout)
+
     def on_timeout(self):
         if self.status != REQUEST_STATUS.DONE:
+            self.ev_loop.remove_listener(self)
             self.close()
             if self.status == REQUEST_STATUS.CONNECTING:
-                result_msg = 'Connection timed out'
+                result_msg = "Connection timed out"
             else:
-                result_msg = 'Timed out waiting for reply'
+                result_msg = "Timed out waiting for reply"
             self.cb(self.env, self.node, result_msg)
-            self.ev_loop.remove_listener(self)
             self.status = REQUEST_STATUS.DONE
+
     def handle_event(self, ts):
         # the event loop detected an event for us
         if self.status == REQUEST_STATUS.CONNECTING:
             self.sock.setblocking(True)
             try:
-                self.sock.send(self.req.encode('ascii') + b'\n')
+                self.sock.send(self.req.encode("ascii") + b"\n")
             except (ConnectionRefusedError, OSError) as e:
-                self.close()
                 if isinstance(e, ConnectionRefusedError):
-                    result_msg = 'Connection refused'
+                    result_msg = "Connection refused"
                 else:
                     result_msg = e.strerror
                 print(result_msg)
                 self.cb(self.env, self.node, result_msg)
-                return False    # ev_loop should remove this listener
+                return False  # ev_loop should remove this listener
             self.status = REQUEST_STATUS.WAITING_RESPONSE
             self.ev_loop.update_listener(self, POLL_OPS_READ)
         elif self.status == REQUEST_STATUS.WAITING_RESPONSE:
             rfile = self.sock.makefile()
-            resp = rfile.readline().split(' ',1)
+            resp = rfile.readline().split(" ", 1)
             rfile.close()
             resp = tuple(part.strip() for part in resp)
-            if resp[0] == 'OK':
-                self.cb(self.env, self.node, 'OK')
+            if resp[0] == "OK":
+                self.cb(self.env, self.node, "OK")
             elif len(resp) == 2:
                 self.cb(self.env, self.node, resp[1])
-            self.close()
-            return False    # ev_loop should remove this listener
+            return False  # ev_loop should remove this listener
+
     # let the event loop know what we are reading on
     def fileno(self):
         return self.sock.fileno()
+
     def close(self):
         if self.sock is not None:
             self.sock.close()
             self.sock = None
         self.status = REQUEST_STATUS.DONE
 
+
 def node_request_cb(env, node, result_msg):
-    env['results'][result_msg].append(node)
-    env['num_nodes'] -= 1
-    if env['num_nodes'] == 0:   # done
-        cb, cb_kwargs, results = env['cb'], env['cb_kwargs'], env['results']
+    env["results"][result_msg].append(node)
+    env["num_nodes"] -= 1
+    if env["num_nodes"] == 0:  # done
+        cb, cb_kwargs, results = env["cb"], env["cb_kwargs"], env["results"]
         cb(results, **cb_kwargs)
 
+
 def node_request(ev_loop, nodes, req, cb, cb_kwargs):
     num_nodes = len(nodes)
     results = defaultdict(list)
     if num_nodes == 0:
         cb(results, **cb_kwargs)
         return
-    env = dict(
-        num_nodes = num_nodes,
-        results = results,
-        cb = cb,
-        cb_kwargs = cb_kwargs
-    )
+    env = dict(num_nodes=num_nodes, results=results, cb=cb, cb_kwargs=cb_kwargs)
     for node in nodes:
         request = ServerToNodeRequest(ev_loop, node, req, node_request_cb, env)
         request.run()
```

### Comparing `walt-server-7/walt/server/threads/main/nodes/show.py` & `walt-server-8.0/walt/server/processes/main/nodes/show.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,119 +1,158 @@
-from walt.server.threads.main.network.netsetup import NetSetup
-from walt.server.tools import format_paragraph, columnate
+from walt.common.formatting import columnate, format_paragraph
+from walt.common.netsetup import NetSetup
 
 NODE_SHOW_QUERY = """
+    WITH powersave_macs AS (
+        SELECT n.mac
+        FROM nodes n, topology t, poeoff po
+        WHERE po.reason = 'powersave' AND (
+            (n.mac = t.mac1 AND t.mac2 = po.mac AND t.port2 = po.port) OR
+            (n.mac = t.mac2 AND t.mac1 = po.mac AND t.port1 = po.port)))
     SELECT  d.name as name, n.model as model,
         split_part(n.image, '/', 1) as image_owner,
         split_part(n.image, '/', 2) as image_name,
-        i.ready as image_ready,
         d.virtual as virtual, d.mac as mac,
         d.ip as ip, COALESCE((d.conf->'netsetup')::int, 0) as netsetup,
-        (case when n.booted then 'yes' else 'NO' end) as booted
-    FROM devices d, nodes n, images i
+        (CASE WHEN n.booted THEN 'yes'
+              WHEN n.mac in (SELECT mac FROM powersave_macs) THEN 'no (powersave)'
+              ELSE 'NO' END) as booted
+    FROM devices d, nodes n
     WHERE   d.type = 'node'
     AND     d.mac = n.mac
-    AND     n.image = i.fullname
     ORDER BY image_owner, name;"""
 
 MSG_USING_NO_NODES = """\
-You are currently using no nodes. (tip: walt help show node-terminology)"""
+You currently do not own any nodes."""
 
 MSG_RERUN_WITH_ALL = """\
 Re-run with --all to see all available nodes."""
 
+MSG_TIP = """\
+Type `walt help show node-ownership` for help."""
+
 TITLE_NODE_SHOW_FREE_NODES_PART = """\
-The following nodes are free (they boot a default image):"""
+The following nodes are currently free:"""
 
 TITLE_NODE_SHOW_USER_NODES_PART = """\
-The following nodes are running one of your images:"""
+You currently own the following nodes:"""
 
 TITLE_NODE_SHOW_OTHER_NODES_PART = """\
-The following nodes are likely to be used by other users, since you do
-not own the image they boot."""
-
-TITLE_NODE_SHOW_NOT_READY_NODES_PART = """\
-The following nodes were detected but are not available for now:
-the startup OS image they will boot is being downloaded."""
+The following nodes currently belong to other users:"""
 
 MSG_NO_NODES = """\
 No nodes detected!"""
 
 MSG_NO_OTHER_NODES = """\
 No other nodes were detected (apart from the ones listed above)."""
 
+
 def short_image_name(image_name):
-    if image_name.endswith(':latest'):
+    if image_name.endswith(":latest"):
         image_name = image_name[:-7]
     return image_name
 
+
 def node_type(mac, virtual):
-    if mac.startswith('52:54:00'):
+    if mac.startswith("52:54:00"):
         if virtual:
-            return 'virtual'
+            return "virtual"
         else:
-            return 'vpn'
+            return "vpn"
     else:
-        return 'physical'
+        return "physical"
+
 
 def get_table_value(record, col_title):
-    if col_title == 'type':
+    if col_title == "type":
         return node_type(record.mac, record.virtual)
-    elif col_title == 'image':
+    elif col_title == "image":
         return short_image_name(record.image_name)
-    elif col_title == 'netsetup':
+    elif col_title == "netsetup":
         return NetSetup(record.netsetup).readable_string()
-    elif col_title == 'clonable_image_link':
-        return 'walt:%s/%s' % (record.image_owner, short_image_name(record.image_name))
+    elif col_title == "clonable_image_link":
+        return "walt:%s/%s" % (record.image_owner, short_image_name(record.image_name))
     else:
         return getattr(record, col_title)
 
+
 def generate_table(title, footnote, records, *col_titles):
-    table = [ tuple(get_table_value(record, col_title) for col_title in col_titles) \
-              for record in records ]
+    table = [
+        tuple(get_table_value(record, col_title) for col_title in col_titles)
+        for record in records
+    ]
     header = list(col_titles)
     return format_paragraph(title, columnate(table, header=header), footnote)
 
-def show(db, username, show_all):
-    res_user, res_free, res_other, res_not_ready = [], [], [], []
+
+def show(db, username, show_all, names_only):
+    res_user, res_free, res_other = [], [], []
     res = db.execute(NODE_SHOW_QUERY)
     for record in res:
-        if not record.image_ready:
-            res_not_ready.append(record)
+        if record.image_owner == username:
+            res_user.append(record)
+        elif record.image_owner == "waltplatform":
+            res_free.append(record)
         else:
-            if record.image_owner == username:
-                res_user.append(record)
-            elif record.image_owner == 'waltplatform':
-                res_free.append(record)
-            else:
-                res_other.append(record)
-    result_msg = ''
+            res_other.append(record)
+    if names_only:
+        if show_all:
+            all_records = res_user + res_free + res_other
+        else:
+            all_records = res_user
+        return "\n".join(record.name for record in all_records)
+    result_msg = ""
+    footnotes = ()
     if len(res_user) == 0 and not show_all:
-        return MSG_USING_NO_NODES + '\n' + MSG_RERUN_WITH_ALL
-    if len(res_user) > 0:
-        # display nodes of requester
-        footnote = None
-        if not show_all:
-            footnote = MSG_RERUN_WITH_ALL
-        result_msg += generate_table(TITLE_NODE_SHOW_USER_NODES_PART, footnote, res_user,
-                        'name', 'type', 'model', 'image', 'ip', 'netsetup', 'booted')
-    if not show_all:
-        return result_msg
-    if len(res_free) > 0:
-        # display free nodes
-        result_msg += generate_table(TITLE_NODE_SHOW_FREE_NODES_PART, None, res_free,
-                        'name', 'type', 'model', 'ip', 'netsetup', 'booted')
-    if len(res_other) + len(res_user) + len(res_free) + len(res_not_ready) == 0:
-        return MSG_NO_NODES + '\n'
-    if len(res_free) + len(res_other) + len(res_not_ready) == 0:
-        result_msg += MSG_NO_OTHER_NODES + '\n'
+        footnotes += (MSG_USING_NO_NODES, MSG_RERUN_WITH_ALL)
+    elif len(res_other) + len(res_user) + len(res_free) == 0:
+        footnotes += (MSG_NO_NODES,)
     else:
-        if len(res_other) > 0:
-            # display nodes of other users
-            result_msg += generate_table(TITLE_NODE_SHOW_OTHER_NODES_PART, None, res_other,
-                            'name', 'type', 'model', 'image_owner', 'clonable_image_link', 'ip', 'netsetup', 'booted')
-        if len(res_not_ready) > 0:
-            # display nodes whose image is currently being downloaded
-            result_msg += generate_table(TITLE_NODE_SHOW_NOT_READY_NODES_PART, None, res_not_ready,
-                            'name', 'type', 'model', 'ip', 'netsetup')
-    return result_msg
-
+        if len(res_user) > 0:
+            # display nodes of requester
+            if not show_all:
+                footnotes += (MSG_RERUN_WITH_ALL,)
+            result_msg += generate_table(
+                TITLE_NODE_SHOW_USER_NODES_PART,
+                None,
+                res_user,
+                "name",
+                "type",
+                "model",
+                "image",
+                "ip",
+                "netsetup",
+                "booted",
+            )
+        if show_all:
+            if len(res_free) + len(res_other) == 0:
+                footnotes += (MSG_NO_OTHER_NODES,)
+            if len(res_free) > 0:
+                # display free nodes
+                result_msg += generate_table(
+                    TITLE_NODE_SHOW_FREE_NODES_PART,
+                    None,
+                    res_free,
+                    "name",
+                    "type",
+                    "model",
+                    "ip",
+                    "netsetup",
+                    "booted",
+                )
+            if len(res_other) > 0:
+                # display nodes of other users
+                result_msg += generate_table(
+                    TITLE_NODE_SHOW_OTHER_NODES_PART,
+                    None,
+                    res_other,
+                    "name",
+                    "type",
+                    "model",
+                    "image_owner",
+                    "clonable_image_link",
+                    "ip",
+                    "netsetup",
+                    "booted",
+                )
+    footnotes += (MSG_TIP,)
+    return result_msg + "\n".join(footnotes)
```

### Comparing `walt-server-7/walt/server/threads/main/parallel.py` & `walt-server-8.0/walt/server/processes/main/parallel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,131 +1,156 @@
 #!/usr/bin/env python
-import os, pty, shlex, fcntl, termios, sys, threading, socket, signal
-from subprocess import Popen, STDOUT
-from walt.common.io import SmartFile, read_and_copy
+import os
+import pickle
+import pty
+import shlex
+import signal
+import sys
+
+from walt.common.io import read_and_copy
 from walt.common.tcp import read_pickle
-from walt.common.tty import set_tty_size_raw
-from walt.common.tools import set_close_on_exec
+from walt.common.tty import set_tty_size, set_tty_size_raw
+
 
 class ForkPtyProcessListener(object):
     def __init__(self, slave_pid, env):
         self.slave_pid = slave_pid
         self.env = env
+
     # let the event loop know what we are reading on
     def fileno(self):
-        return self.env.slave_sock_file.fileno()
+        return self.env.slave_r.fileno()
+
     # when the event loop detects an event for us, this means
     # the slave proces wrote something on its output
     # we just have to copy this to the user socket
     def handle_event(self, ts):
-        return read_and_copy(
-                self.env.slave_sock_file, self.env.client_sock_file)
+        return read_and_copy(self.env.slave_r, self.env.client_sock_file)
+
     def end_child(self):
         try:
-            os.kill(self.slave_pid, signal.SIGTERM)
+            os.kill(self.slave_pid, signal.SIGKILL)
         except OSError:
             pass
-        os.wait()   # wait for child's end
+
     def close(self):
         self.end_child()
         self.env.close()
 
+
 class ParallelProcessSocketListener(object):
     def __init__(self, ev_loop, sock_file, **kwargs):
         self.ev_loop = ev_loop
         self.params = None
         self.client_sock_file = sock_file
-        self.slave_sock_file = None
-        self.send_client('READY\n')
+        self.slave_r, self.slave_w = None, None
+        self.send_client("READY\n")
+
     def send_client(self, s):
-        self.client_sock_file.write(s.encode('UTF-8'))
+        self.client_sock_file.write(s.encode("UTF-8"))
+
     def update_params(self):
         pass  # override in subclasses if needed
+
     def prepare(self, **params):
         return True  # override in subclasses if needed
+
     def get_command(self, **params):
-        '''this should be defined in subclasses'''
+        """this should be defined in subclasses"""
         raise NotImplementedError
+
     def start(self):
-        cmd_args = shlex.split(self.params['cmd'])
+        cmd_args = shlex.split(self.params["cmd"])
         env = os.environ.copy()
-        if 'env' in self.params:
-            env.update(self.params['env'])
-        if 'want_tty' in self.params and self.params['want_tty'] \
-                and 'client_tty' in self.params and self.params['client_tty']:
-            self.start_pty(cmd_args, env)
+        if "env" in self.params:
+            env.update(self.params["env"])
+        if "tty_mode" in self.params and self.params["tty_mode"] is True:
+            return self.start_pty(cmd_args, env)
         else:
-            self.start_popen(cmd_args, env)
+            return self.start_popen(cmd_args, env)
+
     def start_pty(self, cmd_args, env):
+        # print(f'{self.client_sock_file.fileno()}: start_pty {cmd_args}')
         # fork a child process in its own virtual terminal
         slave_pid, fd_slave = pty.fork()
         # the child (slave process) should execute the command
         if slave_pid == 0:
             # set the window size appropriate for the remote client
-            if 'win_size' in self.params:
-                set_tty_size_raw(sys.stdout.fileno(), self.params['win_size'])
+            if "win_size" in self.params:
+                set_tty_size_raw(sys.stdout.fileno(), self.params["win_size"])
             os.execvpe(cmd_args[0], cmd_args, env)
         # the parent should communicate.
         # use unbuffered communication with the slave process
-        slave_r = os.fdopen(os.dup(fd_slave), 'rb', 0)
-        slave_w = os.fdopen(os.dup(fd_slave), 'wb', 0)
-        self.slave_sock_file = SmartFile(slave_r, slave_w)
+        self.slave_r = os.fdopen(os.dup(fd_slave), "rb", 0)
+        self.slave_w = os.fdopen(fd_slave, "wb", 0)
         # create a new listener on the event loop for reading
         # what the slave process outputs
         process_listener = ForkPtyProcessListener(slave_pid, self)
         self.ev_loop.register_listener(process_listener)
+
     def start_popen(self, cmd_args, env):
-        # For efficiency, we let the popen object read directly from the socket.
-        # Thus the ev_loop should not longer detect input data on this socket,
-        # it should only detect errors, that is why we call update_listener() below.
-        set_close_on_exec(self.client_sock_file, False)
-        self.popen = Popen(cmd_args, env=env, bufsize=1024*1024,
-                        stdin=self.client_sock_file, stdout=self.client_sock_file, stderr=STDOUT)
-        set_close_on_exec(self.client_sock_file, True)
-        self.ev_loop.update_listener(self, 0)
-        self.popen_set_finalize_callback()
-    # when the popen object exits, close its output in order
-    # to notify the end of transmission to the client.
-    def popen_set_finalize_callback(self):
-        def monitor_popen(popen, client_sock_file):
-            popen.wait()
-            client_sock_file.close()
-            return
-        self.popen.monitor_thread = threading.Thread(
-                                target=monitor_popen,
-                                args=(self.popen, self.client_sock_file))
-        self.popen.monitor_thread.start()
+        # For efficiency, we fork a child process which will read & write directly
+        # on the socket.
+        # print(f'{self.client_sock_file.fileno()}: start_popen {cmd_args}')
+        if os.fork() == 0:
+            # - child -
+            sock_fd = self.client_sock_file.fileno()
+            for std_fd in (0, 1, 2):
+                os.dup2(sock_fd, std_fd)
+            os.close(sock_fd)
+            os.execvpe(cmd_args[0], cmd_args, env)
+        # - parent -
+        # the child will do the work, we are no longer needed,
+        # so let the event loop remove us.
+        return False
+
     # let the event loop know what we are reading on
     def fileno(self):
         if self.client_sock_file.closed:
             return None
         return self.client_sock_file.fileno()
+
     # handle_event() will be called when the event loop detects
     # new input data for us.
     def handle_event(self, ts):
-        if self.params == None:
-            # we did not get the parameters yet, let's do it
-            self.params = read_pickle(self.client_sock_file)
-            if self.params == None:
-                self.close()    # issue
-                return False
-            self.update_params()
-            if self.prepare(**self.params) == False:
-                self.close()    # issue
-                return False
-            self.params['cmd'] = self.get_command(**self.params)
-            # we now have all info to start the child process
-            self.start()
-        else:
-            # otherwise we are all set. Thus, getting input data means
-            # the user wrote something on the prompt (i.e. the socket)
-            # we just have to copy this to the slave process input
-            return read_and_copy(
-                self.client_sock_file, self.slave_sock_file)
+        try:
+            if self.params is None:
+                # we did not get the parameters yet, let's do it
+                self.params = read_pickle(self.client_sock_file)
+                if self.params is None:
+                    print(f"{self.client_sock_file.fileno()}: malformed params")
+                    return False  # issue, this will call self.close()
+                self.update_params()
+                if self.prepare(**self.params) is False:
+                    # print(f'{self.client_sock_file.fileno()}: closing due to params')
+                    return False  # issue, this will call self.close()
+                self.params["cmd"] = self.get_command(**self.params)
+                # we now have all info to start the child process
+                return self.start()
+            else:
+                # otherwise we are all set. Getting here means
+                # we got input data or the child process ended.
+                # the fact we are still alive and listening implies
+                # we are in the tty mode.
+                # in this mode input data and window resize events are
+                # multiplexed on the socket.
+                evt_info = pickle.load(self.client_sock_file)
+                if evt_info["evt"] == "input_data":
+                    self.slave_w.write(evt_info["data"])
+                    self.slave_w.flush()
+                elif evt_info["evt"] == "window_resize":
+                    win_size = (evt_info["lines"], evt_info["columns"])
+                    set_tty_size(self.slave_w.fileno(), win_size)
+        except Exception as e:
+            print(self, "exception:", repr(e))
+            return False  # issue, this will call self.close()
+
     def close(self):
         if self.client_sock_file:
             self.client_sock_file.close()
             self.client_sock_file = None
-        if self.slave_sock_file:
-            self.slave_sock_file.close()
-            self.slave_sock_file = None
-
+        if self.slave_r:
+            self.slave_r.close()
+            self.slave_r = None
+        if self.slave_w:
+            self.slave_w.close()
+            self.slave_w = None
```

### Comparing `walt-server-7/walt/server/threads/main/snmp/base.py` & `walt-server-8.0/walt/server/processes/blocking/snmp/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,135 +1,172 @@
 #!/usr/bin/env python
-import re, pickle
-from snimpy import manager, snmp
+import pickle
+import re
+from pathlib import Path
+
+from snimpy import snmp
+
+VARIANTS_CACHE_FILE = Path("/var/cache/walt/snmp.variants")
+
 
 class SNMPBitField(object):
-    def __init__(self, snmpfield, shift = 0):
-        hex_string = snmpfield.encode('hex')
-        self.bitlength = len(hex_string)*4
+    def __init__(self, snmpfield, shift=0):
+        hex_string = snmpfield.encode("hex")
+        self.bitlength = len(hex_string) * 4
         self.value = int(hex_string, 16)
         self.shift = shift
+
     def __str__(self):
-        format_string = '{:0%db}' % self.bitlength
+        format_string = "{:0%db}" % self.bitlength
         return format_string.format(self.value)
+
     def bit_index(self, index):
         return self.bitlength - index - 1 + self.shift
+
     def __getitem__(self, index):
         bitindex = self.bit_index(index)
         return (self.value & (1 << bitindex)) >> bitindex
+
     def __setitem__(self, index, val):
         currval = self[index]
         if val != currval:
-            self.value ^= (1 << self.bit_index(index))
+            self.value ^= 1 << self.bit_index(index)
         # otherwise, nothing to do.
+
     def toOctetString(self):
-        format_string = '{:0%dx}' % (self.bitlength / 4)
-        return format_string.format(self.value).decode('hex')
+        format_string = "{:0%dx}" % (self.bitlength / 4)
+        return format_string.format(self.value).decode("hex")
+
 
 # For ports-related bitfields, the indexing starts at 1
 # because there is no port 0.
 # e.g. port 1 status is the left-most bit
 # So we use the 'shift = 1' constructor option.
 class PortsBitField(SNMPBitField):
     def __init__(self, snmpfield):
-        SNMPBitField.__init__(self, snmpfield, shift = 1)
+        SNMPBitField.__init__(self, snmpfield, shift=1)
+
 
 def decode_ipv4_address(octet_string):
-    return '.'.join(str(i) for i in octet_string)
+    return ".".join(str(i) for i in octet_string)
+
+
+def decode_mac_address(value):
+    if value.__class__.__name__ == "OctetString":
+        return ":".join(re.findall("..", value.hex()))
+    elif value.__class__.__name__ == "String":
+        # input value may have high order zero chars ommitted,
+        # e.g. 0:d:b9:45:f8:90, let's restore them
+        return ":".join("%02x" % int(byte, base=16) for byte in value.split(":"))
+    else:
+        raise Exception(f"Could not decode {value} as a mac address")
 
-def decode_mac_address(octet_string):
-    return ':'.join(re.findall('..', octet_string.hex()))
 
 def enum_label(enum):
     return enum.entity.enum[enum.real]
 
+
 class NoSNMPVariantFound(Exception):
     pass
 
+
 # In the worst case, on the WalT platform we
 # could find devices of several vendors.
 # In this case we usually have to unload a mib and load another one,
 # and sometimes target a vendor-specific implementation
 # each time we pass from one vendor to another.
 # In order to handle this, we use classes implementing vendor-specific
 # variants, and a wrapper around the SNMP proxy.
 
 # In this file, we implement base classes. They are used in files
 # lldp.py and poe.py.
 
+
 class Variant:
     @classmethod
     def try_load(cls, snmp_proxy):
         cls.load()
         try:
-            dummy = cls.test_or_exception(snmp_proxy)
-            return True # ok previous line passed with no error
-        except (snmp.SNMPException,
-                snmp.SNMPNoSuchObject,
-                snmp.SNMPNoSuchInstance,
-                snmp.SNMPEndOfMibView,
-                ValueError):
+            cls.test_or_exception(snmp_proxy)
+            return True  # ok previous line passed with no error
+        except (
+            snmp.SNMPException,
+            snmp.SNMPNoSuchObject,
+            snmp.SNMPNoSuchInstance,
+            snmp.SNMPEndOfMibView,
+            ValueError,
+        ):
             cls.unload()
             return False
 
+
 class VariantsCache:
     def __init__(self):
-        try:
-            with open('/var/lib/walt/snmp.cache', 'rb') as f:
-                self.cache = pickle.load(f)
-        except:
+        if VARIANTS_CACHE_FILE.exists():
+            self.cache = pickle.loads(VARIANTS_CACHE_FILE.read_bytes())
+        else:
             self.cache = {}
+
     def save(self):
-        with open('/var/lib/walt/snmp.cache', 'wb') as f:
-            pickle.dump(self.cache, f)
+        if not VARIANTS_CACHE_FILE.exists():
+            VARIANTS_CACHE_FILE.parent.mkdir(parents=True, exist_ok=True)
+        VARIANTS_CACHE_FILE.write_bytes(pickle.dumps(self.cache))
+
     def get(self, topic_msg, host):
         return self.cache.get((topic_msg, host), None)
+
     def set(self, topic_msg, host, variant_name):
         self.cache[(topic_msg, host)] = variant_name
         self.save()
 
+
 VARIANTS_CACHE = VariantsCache()
 
+
 class VariantsSet:
     def __init__(self, topic_msg, variants):
         self.topic_msg = topic_msg
         self.variants = variants
         self.loaded = None
+
     def load_auto(self, snmp_proxy, host):
         if self.loaded is not None:
             self.loaded.unload()
             self.loaded = None
         variant_name = VARIANTS_CACHE.get(self.topic_msg, host)
         if variant_name is not None:
             for variant in self.variants:
                 if variant.__name__ == variant_name:
                     variant.load()
                     self.loaded = variant
                     return variant
-        else:   # not in cache => probe
+        else:  # not in cache => probe
             for variant in self.variants:
                 if variant.try_load(snmp_proxy):
                     self.loaded = variant
                     VARIANTS_CACHE.set(self.topic_msg, host, variant.__name__)
                     return variant
             raise NoSNMPVariantFound(
-                'Device %s does not seem to handle %s.' % \
-                    (host, self.topic_msg))
+                "Device %s does not seem to handle %s." % (host, self.topic_msg)
+            )
+
     def ensure_variant(self, variant):
         if self.loaded is not variant:
             if self.loaded is not None:
                 self.loaded.unload()
                 self.loaded = None
             variant.load()
             self.loaded = variant
 
+
 # The VariantProxy wrapper ensures that each time
 # the SNMP proxy is accessed, the appropriate MIB is loaded, and
 # variant-specific code is executed.
 
+
 class VariantProxy(object):
     def __init__(self, snmp_proxy, host, variants):
         self.unsafe_proxy = snmp_proxy
         self.variants = variants
         self.selected_variant = variants.load_auto(snmp_proxy, host)
 
     @property
```

### Comparing `walt-server-7/walt/server/threads/main/snmp/lldp.py` & `walt-server-8.0/walt/server/processes/blocking/snmp/lldp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 #!/usr/bin/env python
 import re
-from walt.server.threads.main.snmp.mibs import load_mib, unload_mib
-from walt.server.threads.main.snmp.base import decode_ipv4_address, \
-                    decode_mac_address, enum_label, Variant, VariantsSet, VariantProxy
+
+from walt.server.processes.blocking.snmp.base import (
+    Variant,
+    VariantProxy,
+    VariantsSet,
+    decode_ipv4_address,
+    decode_mac_address,
+    enum_label,
+)
+from walt.server.processes.blocking.snmp.mibs import load_mib, unload_mib
+
 
 class StandardLLDP(Variant):
     @staticmethod
     def test_or_exception(snmp_proxy):
         dict(snmp_proxy.lldpRemChassisIdSubtype)
 
     @staticmethod
@@ -15,52 +23,51 @@
 
     @staticmethod
     def unload():
         unload_mib(b"LLDP-MIB")
 
     @staticmethod
     def get_neighbors(snmp_proxy):
-
         mac_per_port = {}
         ip_per_port = {}
         sysname_per_port = {}
 
         # perform SNMP requests
         chassis_types = dict(snmp_proxy.lldpRemChassisIdSubtype)
         chassis_values = dict(snmp_proxy.lldpRemChassisId)
         sys_names = dict(snmp_proxy.lldpRemSysName)
         ip_info = list(snmp_proxy.lldpRemManAddrIfSubtype)
 
         # retrieve mac address and sysname of neighbors
         for neighbor_key in chassis_types:
-            if enum_label(chassis_types[neighbor_key]) == 'macAddress':
+            if enum_label(chassis_types[neighbor_key]) == "macAddress":
                 timeMark, port, index = neighbor_key
                 port = int(port)
-                mac_per_port[port] = decode_mac_address(
-                                chassis_values[neighbor_key])
+                mac_per_port[port] = decode_mac_address(chassis_values[neighbor_key])
                 if neighbor_key in sys_names:
                     sysname_per_port[port] = str(sys_names[neighbor_key])
                 else:
-                    sysname_per_port[port] = ''
+                    sysname_per_port[port] = ""
 
         # retrieve ip addresses of neighbors
         for neighbor_ip_info in ip_info:
             timeMark, port, index, subtype, encoded_ip = neighbor_ip_info
-            if enum_label(subtype).lower() == 'ipv4':
+            if enum_label(subtype).lower() == "ipv4":
                 ip_per_port[int(port)] = decode_ipv4_address(encoded_ip)
 
         # merge info
         neighbors = {}
         for port, mac in mac_per_port.items():
             ip = ip_per_port[port] if port in ip_per_port else None
             sysname = sysname_per_port[port]
-            neighbors[port] = { 'mac': mac, 'ip': ip, 'sysname': sysname }
+            neighbors[port] = {"mac": mac, "ip": ip, "sysname": sysname}
 
         return neighbors
 
+
 class TPLinkLLDP(Variant):
     @staticmethod
     def test_or_exception(snmp_proxy):
         dict(snmp_proxy.lldpNeighborChassisIdType)
 
     @staticmethod
     def load():
@@ -72,41 +79,40 @@
     def unload():
         unload_mib(b"TPLINK-LLDPINFO-MIB")
         unload_mib(b"TPLINK-LLDP-MIB")
         unload_mib(b"TPLINK-MIB")
 
     @staticmethod
     def get_neighbors(snmp_proxy):
-
-        mac_per_port = {}
-        sysname_per_port = {}
         neighbors = {}
 
         # perform SNMP requests
         chassis_types = dict(snmp_proxy.lldpNeighborChassisIdType)
         chassis_values = dict(snmp_proxy.lldpNeighborChassisId)
         sys_names = dict(snmp_proxy.lldpNeighborDeviceName)
         port_info = dict(snmp_proxy.lldpLocalPortId)
 
         # retrieve mac address and sysname of neighbors
         for neighbor_key in chassis_types:
-            if bytes(chassis_types[neighbor_key]) == b'MAC address':
+            if bytes(chassis_types[neighbor_key]) == b"MAC address":
                 port_id, index = neighbor_key
-                port_str = bytes(port_info[int(port_id)]).decode('ascii')
-                port = int(re.split(r'[^\d]+', port_str)[-1])
-                mac = bytes(chassis_values[neighbor_key]).decode('ascii').lower()
+                port_str = bytes(port_info[int(port_id)]).decode("ascii")
+                port = int(re.split(r"[^\d]+", port_str)[-1])
+                mac = bytes(chassis_values[neighbor_key]).decode("ascii").lower()
                 if neighbor_key in sys_names:
-                    sysname = bytes(sys_names[neighbor_key]).decode('ascii')
+                    sysname = bytes(sys_names[neighbor_key]).decode("ascii")
                 else:
-                    sysname = ''
-            neighbors[port] = { 'mac': mac, 'ip': None, 'sysname': sysname }
+                    sysname = ""
+            neighbors[port] = {"mac": mac, "ip": None, "sysname": sysname}
 
         return neighbors
 
 
-LLDP_VARIANTS = VariantsSet('LLDP neighbor table retrieval', (StandardLLDP, TPLinkLLDP))
+LLDP_VARIANTS = VariantsSet("LLDP neighbor table retrieval", (StandardLLDP, TPLinkLLDP))
+
 
 class LLDPProxy(VariantProxy):
     def __init__(self, snmp_proxy, host):
         VariantProxy.__init__(self, snmp_proxy, host, LLDP_VARIANTS)
+
     def get_neighbors(self):
         return self.variant.get_neighbors(self.snmp)
```

### Comparing `walt-server-7/walt/server/threads/main/snmp/mibs/LLDP-MIB.mib` & `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/LLDP-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-7/walt/server/threads/main/snmp/mibs/NETGEAR-POWER-ETHERNET-MIB.mib` & `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/NETGEAR-POWER-ETHERNET-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-7/walt/server/threads/main/snmp/mibs/NETGEAR-REF-MIB.mib` & `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/NETGEAR-REF-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-7/walt/server/threads/main/snmp/mibs/NETGEAR-SWITCHING-MIB.mib` & `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/NETGEAR-SWITCHING-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-7/walt/server/threads/main/snmp/mibs/TPLINK-LLDP-MIB.mib` & `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-LLDP-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-7/walt/server/threads/main/snmp/mibs/TPLINK-LLDPINFO-MIB.mib` & `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-LLDPINFO-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-7/walt/server/threads/main/snmp/mibs/TPLINK-MIB.mib` & `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-7/walt/server/threads/main/snmp/mibs/TPLINK-POWER-OVER-ETHERNET-MIB.mib` & `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/TPLINK-POWER-OVER-ETHERNET-MIB.mib`

 * *Files identical despite different names*

### Comparing `walt-server-7/walt/server/threads/main/snmp/mibs/__init__.py` & `walt-server-8.0/walt/server/processes/blocking/snmp/mibs/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 #!/usr/bin/env python
-import snimpy.mib, snimpy.manager, os.path
+import os.path
+
+import snimpy.manager
+import snimpy.mib
 from pkg_resources import resource_filename
 
 PATH_SET = False
 
+
 def load_mib(mib):
     global PATH_SET
     if not PATH_SET:
         # add this directory to MIB path
-        this_file = resource_filename(__name__, '__init__.py')
+        this_file = resource_filename(__name__, "__init__.py")
         this_dir = os.path.dirname(this_file)
-        mib_path = snimpy.mib.path() + ':' + this_dir
+        mib_path = snimpy.mib.path() + ":" + this_dir
         snimpy.mib.path(mib_path)
         PATH_SET = True
-    if not mib in snimpy.manager.loaded:
+    if mib not in snimpy.manager.loaded:
         snimpy.manager.load(mib)
 
+
 def unload_mib(mib):
     snimpy.manager.loaded.remove(mib)
 
+
 def get_loaded_mibs():
     return snimpy.manager.loaded
 
+
 def unload_any_of_these_mibs(mibs):
     for mib in mibs:
         if mib in snimpy.manager.loaded:
             unload_mib(mib)
```

### Comparing `walt-server-7/walt/server/threads/main/snmp/poe.py` & `walt-server-8.0/walt/server/processes/blocking/snmp/poe.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 #!/usr/bin/env python
-from walt.server.threads.main.snmp.base import Variant, VariantsSet, VariantProxy
-from walt.server.threads.main.snmp.mibs import load_mib, unload_mib, get_loaded_mibs
-
-POE_PORT_ENABLED=1
-POE_PORT_DISABLED=2
-POE_PORT_SPEEDS=(10**7, 10**8, 10**9)   # 10Mb/s 100Mb/s 1Gb/s
+from walt.server.processes.blocking.snmp.base import Variant, VariantProxy, VariantsSet
+from walt.server.processes.blocking.snmp.mibs import (
+    get_loaded_mibs,
+    load_mib,
+    unload_mib,
+)
+
+POE_PORT_ENABLED = 1
+POE_PORT_DISABLED = 2
+POE_PORT_SPEEDS = (10**7, 10**8, 10**9)  # 10Mb/s 100Mb/s 1Gb/s
 
 POE_PORT_MAPPING_CACHE = {}
 
 # In POWER-ETHERNET-MIB, PoE ports are identified using a
 # tuple (grp_index, port_index).
 # grp_index identifies a PoE port group (box in the stack,
 # module in a rack, etc. or 1 for non-modular devices).
@@ -34,46 +38,53 @@
 
 MSG_ISSUE_POE_PORT_MAPPING = """\
 WalT could not guess how to correlate PoE ports and LLDP ports
 on switch %s. Sorry."""
 
 ETHERNETCSMACD = 6
 
+
 def get_poe_port_mapping(snmp_proxy, host):
-    if not host in POE_PORT_MAPPING_CACHE:
+    if host not in POE_PORT_MAPPING_CACHE:
         if b"IF-MIB" not in get_loaded_mibs():
             load_mib(b"IF-MIB")
         iface_port_indexes = list(
-                int(k) for k, v in snmp_proxy.ifSpeed.items()
-                if v in POE_PORT_SPEEDS)
+            int(k) for k, v in snmp_proxy.ifSpeed.items() if v in POE_PORT_SPEEDS
+        )
         iface_type_indexes = list(
-                int(k) for k, v in snmp_proxy.ifType.items()
-                if int(v) == ETHERNETCSMACD)
+            int(k) for k, v in snmp_proxy.ifType.items() if int(v) == ETHERNETCSMACD
+        )
         poe_port_indexes = list(
-                (int(grp_idx), int(grp_port)) \
-                for grp_idx, grp_port in snmp_proxy.pethPsePortAdminEnable.keys())
+            (int(grp_idx), int(grp_port))
+            for grp_idx, grp_port in snmp_proxy.pethPsePortAdminEnable.keys()
+        )
         # check if we have the same number of poe ports and 10/100/1000 ports
         if len(iface_port_indexes) == len(poe_port_indexes):
             # this probably means we can associate iface_port_indexes and
             # poe_port_indexes one by one:
-            iface_to_poe_index = { a: b for a, b in \
-                    zip(iface_port_indexes, poe_port_indexes) }
+            iface_to_poe_index = {
+                a: b for a, b in zip(iface_port_indexes, poe_port_indexes)
+            }
         # otherwise, check if we have a linear range of ethernet ports
         # (i.e. there are no holes in those port indexes)
-        elif max(a-b for a, b in \
-                zip(iface_type_indexes[1:], iface_type_indexes[:-1])) == 1:
+        elif (
+            max(a - b for a, b in zip(iface_type_indexes[1:], iface_type_indexes[:-1]))
+            == 1
+        ):
             # this probably means we can associate iface_type_indexes and
             # poe_port_indexes one by one:
-            iface_to_poe_index = { a: b for a, b in \
-                    zip(iface_type_indexes, poe_port_indexes) }
+            iface_to_poe_index = {
+                a: b for a, b in zip(iface_type_indexes, poe_port_indexes)
+            }
         else:
             raise RuntimeError(MSG_ISSUE_POE_PORT_MAPPING % host)
         POE_PORT_MAPPING_CACHE[host] = iface_to_poe_index
     return POE_PORT_MAPPING_CACHE[host]
 
+
 class StandardPoE(Variant):
     @classmethod
     def test_or_exception(cls, snmp_proxy):
         list(snmp_proxy.pethPsePortAdminEnable.keys())
 
     @classmethod
     def load(cls):
@@ -93,30 +104,33 @@
         port_state = POE_PORT_ENABLED if active_or_not else POE_PORT_DISABLED
         poe_port = port_mapping[switch_port]
         snmp_proxy.pethPsePortAdminEnable[poe_port] = port_state
 
     @classmethod
     def check_poe_in_use(cls, snmp_proxy, port_mapping, switch_port):
         poe_port = port_mapping[switch_port]
-        return int(snmp_proxy.pethPsePortDetectionStatus[poe_port]) == 3  # 'deliveringPower'
+        # value 3 means 'deliveringPower'
+        return int(snmp_proxy.pethPsePortDetectionStatus[poe_port]) == 3
 
     @classmethod
     def get_poe_port_mapping(cls, snmp_proxy, host):
         return get_poe_port_mapping(snmp_proxy, host)
 
+
 # Netgear variant is the same as standard one except that the loaded MIB is not the same
 class NetgearPoE(StandardPoE):
     @classmethod
     def load(cls):
         load_mib(b"NETGEAR-POWER-ETHERNET-MIB")
 
     @classmethod
     def unload(cls):
         unload_mib(b"NETGEAR-POWER-ETHERNET-MIB")
 
+
 # TP-link variant (not standard)
 class TPLinkPoE(Variant):
     @classmethod
     def test_or_exception(cls, snmp_proxy):
         dict(snmp_proxy.tpPoePortStatus)
 
     @classmethod
@@ -143,23 +157,28 @@
     @classmethod
     def check_poe_in_use(cls, snmp_proxy, port_mapping, switch_port):
         poe_port = port_mapping[switch_port]
         return int(snmp_proxy.tpPoePowerStatus[poe_port]) == 2  # 'on'
 
     @classmethod
     def get_poe_port_mapping(cls, snmp_proxy, host):
-        return { int(k): int(k) for k in dict(snmp_proxy.tpPoePortStatus).keys() }
+        return {int(k): int(k) for k in dict(snmp_proxy.tpPoePortStatus).keys()}
+
+
+# TP-link should be first, otherwise sending invalid requests when probing other
+# variants seem to cause it to temporarily stop answering all requests (DoS mitigation?)
+POE_VARIANTS = VariantsSet("PoE SNMP requests", (TPLinkPoE, StandardPoE, NetgearPoE))
 
-# TP-link should be first, otherwise sending invalid requests when probing other variants
-# seem to cause it to temporarily stop answering all requests (DoS mitigation?)
-POE_VARIANTS = VariantsSet('PoE SNMP requests', (TPLinkPoE, StandardPoE, NetgearPoE))
 
 class PoEProxy(VariantProxy):
     def __init__(self, snmp_proxy, host):
         VariantProxy.__init__(self, snmp_proxy, host, POE_VARIANTS)
         self.port_mapping = self.variant.get_poe_port_mapping(snmp_proxy, host)
+
     def check_poe_enabled(self, switch_port):
         return self.variant.check_poe_enabled(self.snmp, self.port_mapping, switch_port)
+
     def set_port(self, switch_port, active_or_not):
         self.variant.set_port(self.snmp, self.port_mapping, switch_port, active_or_not)
+
     def check_poe_in_use(self, switch_port):
         return self.variant.check_poe_in_use(self.snmp, self.port_mapping, switch_port)
```

### Comparing `walt-server-7/walt/server/threads/main/snmp/proxy.py` & `walt-server-8.0/walt/server/processes/blocking/snmp/proxy.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 #!/usr/bin/env python
 from snimpy.manager import Manager
-from walt.server.threads.main.snmp.poe import PoEProxy
-from walt.server.threads.main.snmp.lldp import LLDPProxy
-from walt.server.threads.main.snmp.vlan import VlanProxy
-from walt.server.threads.main.snmp.ipsetup import IPSetupProxy
 from walt.server import const
+from walt.server.processes.blocking.snmp.bridge import BridgeProxy
+from walt.server.processes.blocking.snmp.lldp import LLDPProxy
+from walt.server.processes.blocking.snmp.poe import PoEProxy
 
-SNMP_OPTS = {
-    'retries': 2,
-    'timeout': const.SNMP_TIMEOUT,
-    'cache': True
-}
+SNMP_OPTS = {"retries": 2, "timeout": const.SNMP_TIMEOUT, "cache": True}
 
-class Proxy(object):
-        def __init__(self, host, snmp_conf, poe=False, lldp=False, vlan=False, ipsetup=False):
-            opts = SNMP_OPTS.copy()
-            opts.update(host = host)
-            opts.update(snmp_conf)
-            self.host = host
-            self.snmp = Manager(**opts)
-            if poe:
-                self.poe = PoEProxy(self.snmp, host)
-            if lldp:
-                self.lldp = LLDPProxy(self.snmp, host)
-            if vlan:
-                self.vlan = VlanProxy(self.snmp)
-            if ipsetup:
-                self.ipsetup = IPSetupProxy(self.snmp)
 
+class Proxy(object):
+    def __init__(self, host, snmp_conf, poe=False, lldp=False, bridge=False):
+        opts = SNMP_OPTS.copy()
+        opts.update(host=host)
+        opts.update(snmp_conf)
+        self.host = host
+        self.snmp = Manager(**opts)
+        if poe:
+            self.poe = PoEProxy(self.snmp, host)
+        if lldp:
+            self.lldp = LLDPProxy(self.snmp, host)
+        if bridge:
+            self.bridge = BridgeProxy(self.snmp, host)
```

### Comparing `walt-server-7/walt/server/threads/main/task.py` & `walt-server-8.0/walt/server/processes/main/task.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 import sys
+
 # This object represents a task that was requested by the hub
-# and that must be performed by the main thread.
+# and that must be performed by the main process.
+
 
 class APISessionTask(object):
     def __init__(self, rpc_context, api_session, attr, args, kwargs):
         self.api_session = api_session
         self.attr = attr
         self.args = args
         self.kwargs = kwargs
         self.rpc_context = rpc_context
-        self.async_mode = False
         self.context = api_session.context.copy().update(
-            task = self,
-            requester = rpc_context.requester
+            task=self, requester=rpc_context.remote_service.do_sync.requester
         )
+
     def set_async(self):
-        self.async_mode = True
+        self.rpc_context.task.set_async()
+
     def is_async(self):
-        return self.async_mode
+        return self.rpc_context.task.is_async()
+
     def return_result(self, res):
         self.rpc_context.task.return_result(res)
+
     def run(self):
         try:
             # lookup task
             m = getattr(self.api_session, self.attr)
             # run task
             res = m(self.context, *self.args, **self.kwargs)
         except BaseException as e:
-            print('Exception occured while performing API request:')
+            print("Exception occured while performing API request:")
             sys.excepthook(*sys.exc_info())
             res = e
         # return result, unless async mode was set
         if not self.is_async():
-            self.return_result(res)
+            return res
+
     def is_alive(self):
-        return self.context.requester.do_sync.is_alive()
+        # note: if the requester is disconnected, is_alive() actually returns None.
+        return self.context.requester.is_alive() is True
```

### Comparing `walt-server-7/walt/server/threads/main/thread.py` & `walt-server-8.0/walt/server/processes/main/process.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 import os
-from walt.common.thread import EvThread
-from walt.server.threads.main.network.setup import setup
-from walt.server.threads.main.server import Server
-from walt.server.threads.main.ui.manager import UIManager
-from walt.server.threads.main.hub import HubRPCThreadConnector
-
-class ServerMainThread(EvThread):
-    def __init__(self, tman):
-        EvThread.__init__(self, tman, 'server-main')
-        self.ui = UIManager()
-        self.server = Server(self, self.ui)
+
+from walt.server.process import EvProcess
+from walt.server.processes.main.hub import HubRPCProcessConnector
+from walt.server.processes.main.server import Server
+
+
+class ServerMainProcess(EvProcess):
+    def __init__(self, tman, level):
+        EvProcess.__init__(self, tman, "server-main", level)
+        self.server = Server(self.ev_loop)
+        self.db = self.server.db
+        tman.attach_file(self, self.db)
         self.blocking = self.server.blocking
-        self.hub = HubRPCThreadConnector(self.server)
+        tman.attach_file(self, self.blocking)
+        self.hub = HubRPCProcessConnector(self.server)
+        tman.attach_file(self, self.hub)
 
     def prepare(self):
-        self.server.prepare()
         self.register_listener(self.hub)
         self.register_listener(self.blocking)
-        setup(self.ui)
+        self.register_listener(self.db)
+        self.server.prepare()
         self.notify_systemd()
-        self.server.ui.set_status('Ready.')
         self.server.update()
+        print("Ready.")
 
     def notify_systemd(self):
-        if 'NOTIFY_SOCKET' in os.environ:
+        if "NOTIFY_SOCKET" in os.environ:
             import sdnotify
+
             sdnotify.SystemdNotifier().notify("READY=1")
             # note: podman hangs (at least on debian buster) if we
             # do not disable systemd notify mechanism.
             # at this point we no longer need it, so let's discard
             # the env variable.
-            del os.environ['NOTIFY_SOCKET']
+            del os.environ["NOTIFY_SOCKET"]
 
     def cleanup(self):
         self.server.cleanup()
```

### Comparing `walt-server-7/walt/server/threads/main/transfer.py` & `walt-server-8.0/walt/server/processes/main/transfer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,289 +1,348 @@
+import os
+import random
 
 from walt.common.tcp import Requests
-from walt.server.threads.main.parallel import ParallelProcessSocketListener
 from walt.server.const import SSH_COMMAND
-import os, random
+from walt.server.processes.main.images.setup import script_path
+from walt.server.processes.main.parallel import ParallelProcessSocketListener
 
 TYPE_CLIENT = 0
 TYPE_IMAGE_OR_NODE = 1
 TYPE_BOOTED_IMAGE = 2
 
 HELP_INVALID = dict(
-    node = """\
+    node="""\
 Usage:
 $ walt node cp <local_file_path> <node>:<file_path>
 or
 $ walt node cp <node>:<file_path> <local_file_path>
 or
 $ walt node cp <node>:<file_path> booted-image
 
 Regular files as well as directories are accepted.
-The 3rd form (with keyword 'booted-image') allows to transfer files directly from the selected node
-to the image it has booted. It is a shortcut to using 'walt node cp' and 'walt image cp' in sequence.
+The 3rd form (with keyword 'booted-image') allows\
+ to transfer files directly from the selected node
+to the image it has booted. It is a shortcut to using\
+ 'walt node cp' and 'walt image cp' in sequence.
 
 """,
-    image = """\
+    image="""\
 Usage:
 $ walt image cp <local_file_path> <image>:<file_path>
 or
 $ walt image cp <image>:<file_path> <local_file_path>
 
 Regular files as well as directories are accepted.
-""")
+""",
+)
+
+NODE_TFTP_ROOT = "/var/lib/walt/nodes/%(node_id)s/tftp"
 
-NODE_TFTP_ROOT = "/var/lib/walt/nodes/%(node_mac)s/tftp"
 
 def get_random_suffix():
-    return ''.join(random.choice('0123456789ABCDEF') for i in range(8))
+    return "".join(random.choice("0123456789ABCDEF") for i in range(8))
+
 
-def analyse_file_types(requester, operand_types, src_path, src_fs, dst_path, dst_fs, **kwargs):
-    bad = dict(valid = False)
+def analyse_file_types(
+    requester, operand_types, src_path, src_fs, dst_path, dst_fs, **kwargs
+):
+    bad = dict(valid=False)
     dst_dir = None
     src_type = src_fs.get_file_type(src_path)
     dst_type = dst_fs.get_file_type(dst_path)
     if dst_type is None:
         # maybe this is just the target filename, let's verify that the parent
         # directory exists
         parent_path = os.path.dirname(dst_path)
-        if dst_fs.get_file_type(parent_path) == 'd':
+        if dst_fs.get_file_type(parent_path) == "d":
             # walt node cp <path> <node>:<existing_dir>/<new_entry>
-            dst_type = 'd'
+            dst_type = "d"
             dst_name = os.path.basename(dst_path)
             dst_dir = parent_path
     for ftype, path in [(src_type, src_path), (dst_type, dst_path)]:
         if ftype is None:
-            requester.stderr.write('No such file or directory: %s\n' % path)
+            requester.stderr.write("No such file or directory: %s\n" % path)
             return bad
-    if dst_type == 'f':
-        if src_type == 'd':
+    if dst_type == "f":
+        if src_type == "d":
             requester.stderr.write(
-                "Invalid request. " + \
-                "Overwriting regular file %s with directory %s is not allowed.\n" % \
-                    (dst_path, src_path))
+                "Invalid request. "
+                + "Overwriting regular file %s with directory %s is not allowed.\n"
+                % (dst_path, src_path)
+            )
             return bad
         # overwriting a file
-        dst_type = 'd'
+        dst_type = "d"
         dst_name = os.path.basename(dst_path)
         dst_dir = os.path.dirname(dst_path)
     elif operand_types[1] == TYPE_BOOTED_IMAGE:
         # walt node cp <node>:/<existing_dir> booted-image
         # dir content should be merged into <existing_dir> in booted image
         dst_name = os.path.basename(dst_path)
         dst_dir = os.path.dirname(dst_path)
     elif dst_dir is None:
-        if os.path.basename(src_path) is '.':
+        if os.path.basename(src_path) == ".":
             # walt node cp '.' <node>:/<existing_dir>
             # dir content should be merged into <existing_dir>
             dst_name = os.path.basename(dst_path)
             dst_dir = os.path.dirname(dst_path)
         else:
             # walt node cp <path> <node>:/<existing_dir>
             # we have to keep the source name
             dst_name = os.path.basename(src_path)
             dst_dir = dst_path
-    kwargs.update(
-        valid = True,
-        dst_dir = dst_dir,
-        dst_name = dst_name
-    )
+    kwargs.update(valid=True, dst_dir=dst_dir, dst_name=dst_name)
     return kwargs
 
+
 def get_manager(server, image_or_node_label):
-    if image_or_node_label == 'node':
+    if image_or_node_label == "node":
         return server.nodes
     else:
         return server.images
 
-def validate_cp(image_or_node_label, server,
-                requester, src, dst):
+
+def validate_cp(image_or_node_label, server, requester, src, dst):
     invalid = False
     operand_types = []
     client_operand_index = -1
     filesystems = []
     paths = []
     needs_confirm = False
     info = {}
     for index, operand in enumerate([src, dst]):
-        parts = operand.rsplit(':', 1)  # caution, we may have <image>:<tag>:<path>
-        if operand == 'booted-image' or len(parts) > 1:
-            if operand == 'booted-image':
+        parts = operand.rsplit(":", 1)  # caution, we may have <image>:<tag>:<path>
+        if operand == "booted-image" or len(parts) > 1:
+            if operand == "booted-image":
                 operand_type = TYPE_BOOTED_IMAGE
-                if image_or_node_label == 'image':
-                    requester.stderr.write(\
-                        "Keyword 'booted-image' is only available with command 'walt node cp'.\n")
-                    return { 'status': 'FAILED' }
+                if image_or_node_label == "image":
+                    requester.stderr.write(
+                        "Keyword 'booted-image' is only available with command"
+                        " 'walt node cp'.\n"
+                    )
+                    return {"status": "FAILED"}
                 elif index == 0:
-                    requester.stderr.write(\
-                        "Keyword 'booted-image' can only be used as destination, not source.\n")
-                    return { 'status': 'FAILED' }
+                    requester.stderr.write(
+                        "Keyword 'booted-image' can only be used as destination,"
+                        " not source.\n"
+                    )
+                    return {"status": "FAILED"}
                 elif operand_types[0] != TYPE_IMAGE_OR_NODE:
                     invalid = True
                     break
-                image_tag_or_node, path = 'booted-image', paths[0]
+                image_tag_or_node, path = "booted-image", paths[0]
                 manager = server.images
             else:
                 operand_type = TYPE_IMAGE_OR_NODE
                 image_tag_or_node, path = parts
                 manager = get_manager(server, image_or_node_label)
-            status = manager.validate_cp_entity(requester, image_tag_or_node, index, **info)
-            if status == 'FAILED':
-                return { 'status': 'FAILED' }
-            elif status == 'NEEDS_CONFIRM':
+            status = manager.validate_cp_entity(
+                requester, image_tag_or_node, index, **info
+            )
+            if status == "FAILED":
+                return {"status": "FAILED"}
+            elif status == "NEEDS_CONFIRM":
                 needs_confirm = True
             filesystem = manager.get_cp_entity_filesystem(
-                                    requester, image_tag_or_node, **info)
+                requester, image_tag_or_node, **info
+            )
             if not filesystem.ping():
-                requester.stderr.write(\
-                    "Could not reach %s. Try again later.\n" % image_tag_or_node)
-                return { 'status': 'FAILED' }
+                requester.stderr.write(
+                    "Could not reach %s. Try again later.\n" % image_tag_or_node
+                )
+                return {"status": "FAILED"}
             info.update(
-                **manager.get_cp_entity_attrs(requester, image_tag_or_node, **info))
+                **manager.get_cp_entity_attrs(requester, image_tag_or_node, **info)
+            )
             filesystems.append(filesystem)
-            paths.append(path.rstrip('/'))
+            paths.append(path.rstrip("/"))
         else:
             operand_type = TYPE_CLIENT
             filesystems.append(requester.filesystem)
-            paths.append(operand.rstrip('/'))
+            paths.append(operand.rstrip("/"))
             client_operand_index = index
         operand_types.append(operand_type)
     if not invalid:
         if tuple(operand_types) not in (
-                (TYPE_CLIENT, TYPE_IMAGE_OR_NODE),
-                (TYPE_IMAGE_OR_NODE, TYPE_CLIENT),
-                (TYPE_IMAGE_OR_NODE, TYPE_BOOTED_IMAGE)):
+            (TYPE_CLIENT, TYPE_IMAGE_OR_NODE),
+            (TYPE_IMAGE_OR_NODE, TYPE_CLIENT),
+            (TYPE_IMAGE_OR_NODE, TYPE_BOOTED_IMAGE),
+        ):
             invalid = True
     if invalid:
         requester.stderr.write(HELP_INVALID[image_or_node_label])
-        return { 'status': 'FAILED' }
+        return {"status": "FAILED"}
     src_fs, dst_fs = filesystems
     src_path, dst_path = [
-            path if path.startswith('/') else './' + path
-            for path in paths ]
-    info.update(**analyse_file_types(  requester, operand_types,
-                                src_path, src_fs,
-                                dst_path, dst_fs))
-    if info.pop('valid') == False:
-        return { 'status': 'FAILED' }
+        path if path.startswith("/") else "./" + path for path in paths
+    ]
+    info.update(
+        **analyse_file_types(
+            requester, operand_types, src_path, src_fs, dst_path, dst_fs
+        )
+    )
+    if info.pop("valid") is False:
+        return {"status": "FAILED"}
     # all seems fine
     info.update(
-        status = ('NEEDS_CONFIRM' if needs_confirm else 'OK'),
-        src_path = src_path,
-        client_operand_index = client_operand_index
+        status=("NEEDS_CONFIRM" if needs_confirm else "OK"),
+        src_path=src_path,
+        client_operand_index=client_operand_index,
     )
     print(info)
     return info
 
-def docker_wrap_cmd(cmd, input_needed = False):
-    input_opt = '-i' if input_needed else ''
-    return '''\
-        podman run -q %(input_opt)s --name %%(container_name)s -w /root \
-        --entrypoint /bin/sh %%(image_fullname)s -c "%(cmd)s; sync; sync"
-    ''' % dict(cmd = cmd, input_opt = input_opt)
+
+def docker_wrap_cmd(cmd, input_needed=False):
+    input_opt = "-i" if input_needed else ""
+    walt_tar_send = script_path("walt-tar-send")
+    return f"""\
+        podman run -q {input_opt} --name %(container_name)s -w /root \
+        -v {walt_tar_send}:/bin/walt-tar-send \
+        --entrypoint /bin/sh %(image_fullname)s -c "{cmd}; sync; sync" """
+
 
 def ssh_wrap_cmd(cmd):
     return SSH_COMMAND + ' root@%(node_ip)s "' + cmd + '"'
 
-TarSendCommand='''\
-        mkdir -p /tmp/%(tmp_name)s && \
-        ln -s %(src_path)s /tmp/%(tmp_name)s/%(dst_name)s && \
-        cd /tmp/%(tmp_name)s && \
-        tar c -h %(dst_name)s && cd / && rm -rf /tmp/%(tmp_name)s '''
+
+TarSendCommand = """\
+        walt-tar-send %(src_path)s %(dst_name)s \
+        """
+
 
 def get_absolute_path(path):
-    if not path.startswith('/'):
-        # relative path, turn to absolute
-        return '$PWD/' + path
+    if not path.startswith("/"):
+        # relative path, turn to absolute.
+        # all transfers use the root user,
+        # so let's prefix with the home of root.
+        return "/root/" + path
     return path
 
-TarReceiveCommand='''\
-        cd %(dst_dir)s && tar x'''
+
+TarReceiveCommand = """\
+        cd %(dst_dir)s && tar x"""
+
 
 class ImageTarSender(ParallelProcessSocketListener):
     REQ_ID = Requests.REQ_TAR_FROM_IMAGE
+
     def get_command(self, src_path, **params):
         src_path = get_absolute_path(src_path)
         return docker_wrap_cmd(TarSendCommand) % dict(
-            tmp_name = '.' + get_random_suffix(),
-            src_path = src_path,
-            **params
+            tmp_name="." + get_random_suffix(), src_path=src_path, **params
         )
 
+
 class ImageTarReceiver(ParallelProcessSocketListener):
     REQ_ID = Requests.REQ_TAR_TO_IMAGE
+
     def get_command(self, **params):
-        return docker_wrap_cmd(\
-                TarReceiveCommand, input_needed = True) % params
+        return docker_wrap_cmd(TarReceiveCommand, input_needed=True) % params
+
 
 class NodeTarSender(ParallelProcessSocketListener):
     REQ_ID = Requests.REQ_TAR_FROM_NODE
+
     def get_command(self, src_path, **params):
         src_path = get_absolute_path(src_path)
         return ssh_wrap_cmd(TarSendCommand) % dict(
-            tmp_name = '.' + get_random_suffix(),
-            src_path = src_path,
-            **params
+            tmp_name="." + get_random_suffix(), src_path=src_path, **params
         )
 
+
 class NodeTarReceiver(ParallelProcessSocketListener):
     REQ_ID = Requests.REQ_TAR_TO_NODE
+
     def get_command(self, **params):
         return ssh_wrap_cmd(TarReceiveCommand) % params
 
+
+IMAGE_BUILD_TAR_RECEIVER_COMMAND = """\
+walt-annotate-cmd --mode pickle4 \
+    walt-image-build-helper --from-stdin %(image_fullname)s"""
+
+
+class ImageBuildTarReceiver(ParallelProcessSocketListener):
+    REQ_ID = Requests.REQ_TAR_FOR_IMAGE_BUILD
+
+    def get_command(self, **params):
+        return IMAGE_BUILD_TAR_RECEIVER_COMMAND % params
+
+
 class NodeFakeTFTPGet(ParallelProcessSocketListener):
     REQ_ID = Requests.REQ_FAKE_TFTP_GET
-    def prepare(self, **params):
-        full_path = (NODE_TFTP_ROOT + '%(path)s') % params
+
+    def prepare(self, node_mac=None, node_ip=None, **params):
+        if node_mac is not None:
+            params["node_id"] = node_mac
+        elif node_ip is not None:
+            params["node_id"] = node_ip
+        else:
+            self.send_client("NO MAC OR IP SPECIFIED\n")
+            return False
+        full_path = (NODE_TFTP_ROOT + "%(path)s") % params
         if os.path.exists(full_path):
-            self.send_client('OK\n')
+            self.send_client("OK\n")
             # send file length
             # (client will be able to close connection immediately after
             # the transfer, this is faster than detecting the end of the
             # 'cat' command)
-            self.send_client(str(os.stat(full_path).st_size) + '\n')
+            self.send_client(str(os.stat(full_path).st_size) + "\n")
             # save full_path for get_command() below
-            self.params['full_path'] = full_path
+            self.params["full_path"] = full_path
             return True
         else:
-            self.send_client('NO SUCH FILE\n')
+            self.send_client("NO SUCH FILE\n")
             return False
+
     def get_command(self, **params):
         return 'cat "%(full_path)s"' % params
 
+
 class VPNNodeImageDump(ParallelProcessSocketListener):
     REQ_ID = Requests.REQ_VPN_NODE_IMAGE
+
     def prepare(self, **params):
-        if 'model' not in params or 'entrypoint' not in params:
-            self.send_client('ERR Invalid request!\n')
+        if "model" not in params or "entrypoint" not in params:
+            self.send_client("ERR Invalid request!\n")
             return False
-        if params['model'] != 'rpi-3-b-plus':
-            self.send_client('ERR Only rpi-3-b-plus boards can be used as a WalT node.\n')
+        if params["model"] != "rpi-3-b-plus":
+            self.send_client(
+                "ERR Only rpi-3-b-plus boards can be used as a WalT node.\n"
+            )
             return False
-        self.send_client('MSG Generating image... Please be patient.\n')
-        self.send_client('START\n')
+        self.send_client("MSG Generating image... Please be patient.\n")
+        self.send_client("START\n")
         return True
+
     def get_command(self, **params):
-        return 'podman run -q --rm waltplatform/rpi3bp-vpn-sd-dump "%(entrypoint)s"' % params
+        return (
+            "podman run -q --rm docker.io/waltplatform/rpi3bp-vpn-sd-dump"
+            ' "%(entrypoint)s"' % params
+        )
+
 
 class TransferManager(object):
     def __init__(self, tcp_server, ev_loop):
-        for cls in [    ImageTarSender,
-                        ImageTarReceiver,
-                        NodeTarSender,
-                        NodeTarReceiver,
-                        NodeFakeTFTPGet,
-                        VPNNodeImageDump ]:
+        for cls in [
+            ImageTarSender,
+            ImageTarReceiver,
+            NodeTarSender,
+            NodeTarReceiver,
+            ImageBuildTarReceiver,
+            NodeFakeTFTPGet,
+            VPNNodeImageDump,
+        ]:
             tcp_server.register_listener_class(
-                    req_id = cls.REQ_ID,
-                    cls = cls,
-                    ev_loop = ev_loop)
+                req_id=cls.REQ_ID, cls=cls, ev_loop=ev_loop
+            )
+
 
 def format_node_to_booted_image_transfer_cmd(src_path, **params):
     src_path = get_absolute_path(src_path)
     node_send_cmd = ssh_wrap_cmd(TarSendCommand) % dict(
-        tmp_name = '.' + get_random_suffix(),
-        src_path = src_path,
-        **params
+        tmp_name="." + get_random_suffix(), src_path=src_path, **params
     )
-    image_recv_cmd = docker_wrap_cmd(
-            TarReceiveCommand, input_needed = True) % params
-    return node_send_cmd + ' | ' + image_recv_cmd
+    image_recv_cmd = docker_wrap_cmd(TarReceiveCommand, input_needed=True) % params
+    return node_send_cmd + " | " + image_recv_cmd
```

### Comparing `walt-server-7/walt/server/threads/main/tree.py` & `walt-server-8.0/walt/server/processes/blocking/devices/tree.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,113 +1,135 @@
 #!/usr/bin/env python
 
 from collections import OrderedDict
+
 from walt.server.tools import try_encode
 
+
 # special characters used to display the tree (if possible)
 class UNICODE_CHARSET:
-    WHOLE_V = '\u2502'         # whole vertical bar
-    WHOLE_V_RIGHT_H = '\u251c' # whole vertical + right horizontal bars
-    WHOLE_H = '\u2500'         # whole horizontal bar
-    UPPER_V_RIGHT_H = '\u2514' # upper vertical + right horizontal bars
-    SPACE = ' '
-
-SPECIAL_CHARS = ''.join(
-        v for k, v in UNICODE_CHARSET.__dict__.items() \
-                if isinstance(v, str))
+    WHOLE_V = "\u2502"  # whole vertical bar
+    WHOLE_V_RIGHT_H = "\u251c"  # whole vertical + right horizontal bars
+    WHOLE_H = "\u2500"  # whole horizontal bar
+    UPPER_V_RIGHT_H = "\u2514"  # upper vertical + right horizontal bars
+    SPACE = " "
+
+
+SPECIAL_CHARS = "".join(
+    v for k, v in UNICODE_CHARSET.__dict__.items() if isinstance(v, str)
+)
+
 
 # simpler characters (fallback)
 class ASCII_CHARSET:
-    WHOLE_V = '|'
-    WHOLE_V_RIGHT_H = '|'
-    WHOLE_H = '-'
-    UPPER_V_RIGHT_H = '|'
-    SPACE = ' '
+    WHOLE_V = "|"
+    WHOLE_V_RIGHT_H = "|"
+    WHOLE_H = "-"
+    UPPER_V_RIGHT_H = "|"
+    SPACE = " "
+
 
 class Tree(object):
     """Class allowing to display an object graph as a tree."""
+
     def __init__(self, stdout_encoding):
         self.nodes = OrderedDict()
         self.up_to_date = False
         if try_encode(SPECIAL_CHARS, stdout_encoding):
             self.charset = UNICODE_CHARSET
         else:
             self.charset = ASCII_CHARSET
+
     def add_node(self, key, label):
-        self.nodes[key] = dict(
-            key=key,
-            label=label,
-            children=[],
-            prune=None)
+        self.nodes[key] = dict(key=key, label=label, children=[], prune=None)
         self.up_to_date = False
+
     def add_child(self, node_key, child_pos, child_key):
-        self.nodes[node_key]['children'].append((child_pos, child_key))
+        self.nodes[node_key]["children"].append((child_pos, child_key))
+
     def prune(self, node_key, msg):
         if node_key in self.nodes:
-            self.nodes[node_key]['prune'] = msg
+            self.nodes[node_key]["prune"] = msg
+
     def sort_children(self):
         if not self.up_to_date:
             # sort children by child_pos
             for node in self.nodes.values():
-                node['children'] = sorted(node['children'],
-                          key=lambda t: (-1, t[1]) if t[0] is None else (t[0], t[1]))
+                node["children"] = sorted(
+                    node["children"],
+                    key=lambda t: (-1, t[1]) if t[0] is None else (t[0], t[1]),
+                )
             self.up_to_date = True
+
     def printed(self, root):
         self.root_node = self.nodes[root]
         self.sort_children()
         return self.print_elem(**self.root_node)
-    def print_elem(self, key, label, children, prune,
-                        child_pos = None, prefix = '',
-                        last_child = False, seen = None, **kwargs):
-        if seen == None:
+
+    def print_elem(
+        self,
+        key,
+        label,
+        children,
+        prune,
+        child_pos=None,
+        prefix="",
+        last_child=False,
+        seen=None,
+        **kwargs
+    ):
+        if seen is None:
             seen = set()
-        if key in seen and child_pos == None:
+        if key in seen and child_pos is None:
             # there is not much we can print here
-            return ''
-        if self.root_node['key'] == key and key not in seen:  # root element
+            return ""
+        if self.root_node["key"] == key and key not in seen:  # root element
             output = "%s\n" % label
             # align to 2nd letter of the name
             subtree_offset = 1
-            prefix += (self.charset.SPACE * subtree_offset)
+            prefix += self.charset.SPACE * subtree_offset
         else:
             if key in seen:
-                label = '~> back to %s' % label
-            if child_pos == None:
+                label = "~> back to %s" % label
+            if child_pos is None:
                 label = "?: %s" % label
                 subtree_offset = 3
             else:
                 label = "%d: %s" % (child_pos, label)
                 # align to 2nd letter of the name
                 subtree_offset = len("%d" % child_pos) + 2
             if last_child:
                 sep_char_item = self.charset.UPPER_V_RIGHT_H
                 sep_char_child = self.charset.SPACE
             else:
                 sep_char_item = self.charset.WHOLE_V_RIGHT_H
                 sep_char_child = self.charset.WHOLE_V
-            output = "%s%s%s%s\n" % \
-                    (prefix, sep_char_item, self.charset.WHOLE_H, label)
-            prefix += sep_char_child + (self.charset.SPACE * (subtree_offset+1))
+            output = "%s%s%s%s\n" % (prefix, sep_char_item, self.charset.WHOLE_H, label)
+            prefix += sep_char_child + (self.charset.SPACE * (subtree_offset + 1))
         if key not in seen:
             seen.add(key)
             if prune is None:
                 num_children = len(children)
                 for idx, child in enumerate(children):
-                        child_pos, child_key = child
-                        last_child = (idx == num_children-1)
-                        child = self.nodes[child_key]
-                        output += self.print_elem(
-                                        child_pos = child_pos,
-                                        prefix = prefix,
-                                        last_child = last_child,
-                                        seen = seen,
-                                        **child)
+                    child_pos, child_key = child
+                    last_child = idx == num_children - 1
+                    child = self.nodes[child_key]
+                    output += self.print_elem(
+                        child_pos=child_pos,
+                        prefix=prefix,
+                        last_child=last_child,
+                        seen=seen,
+                        **child
+                    )
             else:
                 # prune: display the message as a fake child
-                output += "%s%s%s%s\n" % \
-                    (prefix, self.charset.UPPER_V_RIGHT_H, self.charset.WHOLE_H, prune)
+                output += "%s%s%s%s\n" % (
+                    prefix,
+                    self.charset.UPPER_V_RIGHT_H,
+                    self.charset.WHOLE_H,
+                    prune,
+                )
         return output
+
     def children(self, key):
         self.sort_children()
-        return [child[1] for child in self.nodes[key]['children']]
-
-
+        return [child[1] for child in self.nodes[key]["children"]]
```

### Comparing `walt-server-7/walt/server/threads/main/vpn-proxy-setup.sh` & `walt-server-8.0/walt/server/processes/main/vpn-proxy-setup.sh`

 * *Files identical despite different names*

### Comparing `walt-server-7/walt/server/threads/main/vpn.py` & `walt-server-8.0/walt/server/processes/main/vpn.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-import tempfile, sys
+import sys
+import tempfile
 from pathlib import Path
 from time import time
-from collections import defaultdict
+
 from pkg_resources import resource_string
-from walt.common.tools import do, chown_tree
 from walt.common.constants import UNSECURE_ECDSA_KEYPAIR
+from walt.common.tools import do
 
 # Walt VPN clients should first connect with our unsecure key pair (written below).
 # They will be forcibly directed to "walt-vpn-auth-tool" command.
 # This command connects to walt-server-daemon and asks for generation of VPN client
 # credentials.
 # If someone has been running "walt vpn monitor" when this happened, he can accept
 # or deny the request. Otherwise the request is immediately denied (except in a
@@ -22,164 +23,149 @@
 # "walt vpn monitor" is run in a loop in order to easily accept a batch of access
 # requests. It first calls API function wait_grant_request(). When a device requests
 # VPN access, wait_grant_request() is unblocked and the "walt vpn monitor" command
 # prompts the request to the user. When the user answers, its response is transmitted
 # to the server using API function respond_grant_request(), and the device request
 # is unblocked with an appropriate result. Then, "walt vpn monitor" restarts its loop
 # and calls API function wait_grant_request() again, waiting for next device request.
-# However, if the user does not respond immediately to a given request, another device may
-# try to request a grant at this time. Since the "walt vpn monitor" loop is blocked on
-# user input, the server has no pending wait_grant_request(). Because of this,
-# we record the fact a given device request is pending user response. And, for a short
+# However, if the user does not respond immediately to a given request, another device
+# may try to request a grant at this time. Since the "walt vpn monitor" loop is blocked
+# on user input, the server has no pending wait_grant_request(). Because of this, we
+# record the fact a given device request is pending user response. And, for a short
 # period of time, we allow any other device request to wait for "walt vpn monitor" to
 # loop again and respond to this new request.
 
-WALT_VPN_USER = dict(
-    home_dir = Path("/var/lib/walt/vpn"),
-    authorized_keys_pattern = """
-# walt VPN secured access
-cert-authority,restrict,command="walt-vpn-endpoint" %(ca_pub_key)s
-# walt VPN authentication step
-restrict,command="walt-vpn-auth-tool $SSH_ORIGINAL_COMMAND" %(unsecure_pub_key)s
-""")
-
-VPN_CA_KEY = WALT_VPN_USER['home_dir'] / '.ssh' / 'vpn-ca-key'
-VPN_CA_KEY_PUB = WALT_VPN_USER['home_dir'] / '.ssh' / 'vpn-ca-key.pub'
+WALT_VPN_USER_HOME = Path("/var/lib/walt/vpn")
+VPN_CA_KEY = WALT_VPN_USER_HOME / ".ssh" / "vpn-ca-key"
+VPN_CA_KEY_PUB = WALT_VPN_USER_HOME / ".ssh" / "vpn-ca-key.pub"
 
-UNSECURE_KEY, UNSECURE_KEY_PUB = UNSECURE_ECDSA_KEYPAIR['openssh-priv'], UNSECURE_ECDSA_KEYPAIR['openssh-pub']
-
-PENDING_USER_RESPONSE_DELAY = 5*60  # seconds
+PENDING_USER_RESPONSE_DELAY = 5 * 60  # seconds
 
 WAITING = 0
 PENDING_USER_RESPONSE = 1
 
+UNSECURE_KEY = UNSECURE_ECDSA_KEYPAIR["openssh-priv"].decode("ascii")
+UNSECURE_KEY_PUB = UNSECURE_ECDSA_KEYPAIR["openssh-pub"].decode("ascii")
+
+
 class VPNManager:
     def __init__(self):
         self.waiting_requests = {}
         self.waiting_monitors = set()
-        self.verify_conf()
 
     # when a user types "walt vpn monitor", we get here
     def wait_grant_request(self, task):
         self.cleanup()
         # check if another device was waiting for this "walt vpn monitor" to loop again.
         for device_mac, request_task_info in self.waiting_requests.items():
-            if request_task_info['status'] == WAITING:
+            if request_task_info["status"] == WAITING:
                 # yes, immediately indicate to "walt vpn monitor" that it should respond
                 # the request of this device (by returning its mac),
                 # and update the device request task status.
-                request_task_info['status'] = PENDING_USER_RESPONSE
-                request_task_info['timeout'] = time() + PENDING_USER_RESPONSE_DELAY
+                request_task_info["status"] = PENDING_USER_RESPONSE
+                request_task_info["timeout"] = time() + PENDING_USER_RESPONSE_DELAY
                 return device_mac
         # otherwise, there is no device request pending
-        task.set_async()   # result will be available later
+        task.set_async()  # result will be available later
         self.waiting_monitors.add(task)
 
     # cleanup disconnected tasks and those which timed out
     def cleanup(self):
         for mac, task_info in self.waiting_requests.copy().items():
-            task = task_info['task']
+            task = task_info["task"]
             if not task.is_alive():
                 del self.waiting_requests[mac]
                 continue
-            if task_info['timeout'] < time():
-                task.return_result(('FAILED', "Timed out waiting for user response!"))
+            if task_info["timeout"] < time():
+                task.return_result(("FAILED", "Timed out waiting for user response!"))
                 del self.waiting_requests[mac]
                 continue
         for task in self.waiting_monitors.copy():
             if not task.is_alive():
                 self.waiting_monitors.remove(task)
 
-    # check if some of the current "walt vpn monitor" commands are waiting for user input.
+    # check if some of the current "walt vpn monitor" commands are waiting for
+    # user input.
     def have_pending_user_responses(self):
         for request_task_info in self.waiting_requests.values():
-            if request_task_info['status'] == PENDING_USER_RESPONSE:
+            if request_task_info["status"] == PENDING_USER_RESPONSE:
                 return True
         return False
 
     # a device requesting VPN access grant will call this method.
     def request_grant(self, task, device_mac):
-        print('vpn grant request', device_mac)
+        print("vpn grant request", device_mac)
         self.cleanup()
         if len(self.waiting_monitors) == 0 and not self.have_pending_user_responses():
-            return ('FAILED', "No pending 'walt vpn monitor' command.")
-        task.set_async()   # result will be available later
+            return ("FAILED", "No pending 'walt vpn monitor' command.")
+        task.set_async()  # result will be available later
         if len(self.waiting_monitors) > 0:
             task_status = PENDING_USER_RESPONSE
             for monitor_task in self.waiting_monitors:
                 monitor_task.return_result(device_mac)
             self.waiting_monitors = set()
-        else:   # some monitors are there but not connected
-                # (waiting for user response about another device)
+        else:  # some monitors are there but not connected
+            # (waiting for user response about another device)
             task_status = WAITING
         timeout = time() + PENDING_USER_RESPONSE_DELAY
         self.waiting_requests[device_mac] = {
-                    'task': task,
-                    'status': task_status,
-                    'timeout': timeout,
+            "task": task,
+            "status": task_status,
+            "timeout": timeout,
         }
 
-    # "walt vpn monitor" calls this function to transmit user's response about a device request.
+    # "walt vpn monitor" calls this function to transmit user's response about a
+    # device request.
     def respond_grant_request(self, device_mac, auth_ok):
         request_task_info = self.waiting_requests.get(device_mac, None)
         if request_task_info is None:
-            return ('FAILED', "No such device (it may have been processed by another 'walt vpn monitor' command).")
-        request_task = request_task_info['task']
+            return (
+                "FAILED",
+                (
+                    "No such device (it may have been processed by another"
+                    " 'walt vpn monitor' command)."
+                ),
+            )
+        request_task = request_task_info["task"]
         if auth_ok:
             keypair = self.generate_device_keys(device_mac)
-            request_task.return_result(('OK',) + keypair)
-            result = ('OK', 'Device access was granted.')
+            request_task.return_result(("OK",) + keypair)
+            result = ("OK", "Device access was granted.")
         else:
-            request_task.return_result(('FAILED', "Denied!"))
-            result = ('OK', 'Device access was denied.')
+            request_task.return_result(("FAILED", "Denied!"))
+            result = ("OK", "Device access was denied.")
         self.waiting_requests.pop(device_mac)
         return result
 
-    def verify_conf(self):
-        home_dir = WALT_VPN_USER['home_dir']
-        if not home_dir.exists():     # if not configured
-            # create user walt-vpn
-            home_dir = WALT_VPN_USER['home_dir']
-            do("useradd -U -d %(home_dir)s walt-vpn" % dict(
-                home_dir = str(home_dir)
-            ))
-            # generate VPN CA key
-            VPN_CA_KEY.parent.mkdir(parents=True)
-            do("ssh-keygen -N '' -t ecdsa -b 521 -f %s" % str(VPN_CA_KEY))
-            ca_pub_key = VPN_CA_KEY_PUB.read_text().strip()
-            # create appropriate authorized_keys file
-            authorized_keys_file = home_dir / '.ssh' / 'authorized_keys'
-            authorized_keys_file.write_text(
-                WALT_VPN_USER['authorized_keys_pattern'] % dict(
-                ca_pub_key = ca_pub_key,
-                unsecure_pub_key = UNSECURE_KEY_PUB
-            ))
-            # fix owner to 'walt-vpn'
-            chown_tree(home_dir, 'walt-vpn', 'walt-vpn')
-
     def generate_device_keys(self, device_mac):
-        device_id = 'vpn_' + device_mac.replace(':', '')
+        device_id = "vpn_" + device_mac.replace(":", "")
         with tempfile.TemporaryDirectory() as tmpdirname:
-            do("ssh-keygen -C %(comment)s -N '' -t ecdsa -b 384 -f %(tmpdir)s/key" % dict(
-                    comment = 'walt-vpn@' + device_id,
-                    tmpdir = tmpdirname
-            ))
-            do("ssh-keygen -s %(vpn_ca_key)s -I '%(device_id)s' -n %(principal)s %(tmpdir)s/key.pub" % dict(
-                    vpn_ca_key = str(VPN_CA_KEY),
-                    device_id = device_id,
-                    principal = 'walt-vpn',
-                    tmpdir = tmpdirname
-            ))
+            do(
+                "ssh-keygen -C %(comment)s -N '' -t ecdsa -b 384 -f %(tmpdir)s/key"
+                % dict(comment="walt-vpn@" + device_id, tmpdir=tmpdirname)
+            )
+            do(
+                "ssh-keygen -s %(vpn_ca_key)s -I '%(device_id)s' -n %(principal)s"
+                " %(tmpdir)s/key.pub"
+                % dict(
+                    vpn_ca_key=str(VPN_CA_KEY),
+                    device_id=device_id,
+                    principal="walt-vpn",
+                    tmpdir=tmpdirname,
+                )
+            )
             tmpdir = Path(tmpdirname)
-            priv_key = (tmpdir / 'key').read_text()
-            pub_cert_key = (tmpdir / 'key-cert.pub').read_text()
+            priv_key = (tmpdir / "key").read_text()
+            pub_cert_key = (tmpdir / "key-cert.pub").read_text()
             return (priv_key, pub_cert_key)
 
     def get_unsecure_key_pair(self):
         return (UNSECURE_KEY, UNSECURE_KEY_PUB)
 
     def get_vpn_proxy_setup_script(self):
-        script_content = resource_string(__name__, "vpn-proxy-setup.sh").decode(sys.getdefaultencoding())
+        script_content = resource_string(__name__, "vpn-proxy-setup.sh").decode(
+            sys.getdefaultencoding()
+        )
         return script_content % dict(
-            ca_pub_key = VPN_CA_KEY_PUB.read_text().strip(),
-            unsecure_pub_key = UNSECURE_KEY_PUB
+            ca_pub_key=VPN_CA_KEY_PUB.read_text().strip(),
+            unsecure_pub_key=UNSECURE_KEY_PUB,
         )
```

