# Comparing `tmp/walt-client-7.tar.gz` & `tmp/walt-client-8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/walt-client-7.tar", last modified: Mon Feb  1 15:17:02 2021, max compression
+gzip compressed data, was "walt-client-8.0.tar", last modified: Fri Jun 23 07:38:23 2023, max compression
```

## Comparing `walt-client-7.tar` & `walt-client-8.0.tar`

### file list

```diff
@@ -1,83 +1,129 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:02.000000 walt-client-7/
--rw-r--r--   0 root         (0) root         (0)       32 2020-09-24 12:01:14.000000 walt-client-7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      279 2021-02-01 15:17:02.000000 walt-client-7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      126 2020-09-24 12:01:14.000000 walt-client-7/README.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:02.000000 walt-client-7/bash_completion/
--rw-r--r--   0 root         (0) root         (0)    16774 2020-09-24 12:01:14.000000 walt-client-7/bash_completion/walt
--rw-r--r--   0 root         (0) root         (0)       38 2021-02-01 15:17:02.000000 walt-client-7/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      340 2020-09-24 12:01:14.000000 walt-client-7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:02.000000 walt-client-7/walt/
--rw-r--r--   0 root         (0) root         (0)      147 2020-09-24 12:01:14.000000 walt-client-7/walt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:02.000000 walt-client-7/walt/client/
--rw-r--r--   0 root         (0) root         (0)       44 2020-09-24 12:01:14.000000 walt-client-7/walt/client/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1915 2020-09-24 12:01:14.000000 walt-client-7/walt/client/advanced.py
--rwxr-xr-x   0 root         (0) root         (0)     1617 2020-09-24 12:01:14.000000 walt-client-7/walt/client/application.py
--rw-r--r--   0 root         (0) root         (0)      711 2020-09-24 12:01:14.000000 walt-client-7/walt/client/auth.py
--rwxr-xr-x   0 root         (0) root         (0)     1846 2020-09-24 12:01:14.000000 walt-client-7/walt/client/client.py
--rw-r--r--   0 root         (0) root         (0)     4797 2020-09-24 12:01:14.000000 walt-client-7/walt/client/config.py
--rwxr-xr-x   0 root         (0) root         (0)     4413 2020-09-24 12:01:14.000000 walt-client-7/walt/client/device.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:02.000000 walt-client-7/walt/client/doc/
--rwxr-xr-x   0 root         (0) root         (0)        0 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     2247 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/color.py
--rw-r--r--   0 root         (0) root         (0)    11918 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/markdown.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:02.000000 walt-client-7/walt/client/doc/md/
--rw-r--r--   0 root         (0) root         (0)      933 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/__init__.py
--rw-r--r--   0 root         (0) root         (0)      834 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/admin.md
--rw-r--r--   0 root         (0) root         (0)      764 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/compatibility.md
--rw-r--r--   0 root         (0) root         (0)     1858 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/device-config.md
--rw-r--r--   0 root         (0) root         (0)     1211 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/device-sets.md
--rw-r--r--   0 root         (0) root         (0)     1536 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/help-intro.md
--rw-r--r--   0 root         (0) root         (0)      630 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/image-cp.md
--rw-r--r--   0 root         (0) root         (0)    11995 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/image-from-scratch.md
--rw-r--r--   0 root         (0) root         (0)     2157 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/image-spec-file.md
--rw-r--r--   0 root         (0) root         (0)     1699 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/log-cat.md
--rw-r--r--   0 root         (0) root         (0)      927 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/log-checkpoint.md
--rw-r--r--   0 root         (0) root         (0)     1661 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/log-echo.md
--rw-r--r--   0 root         (0) root         (0)      494 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/log-format.md
--rw-r--r--   0 root         (0) root         (0)      727 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/log-history.md
--rw-r--r--   0 root         (0) root         (0)     2828 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/log-monitor.md
--rw-r--r--   0 root         (0) root         (0)      479 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/log-realtime.md
--rw-r--r--   0 root         (0) root         (0)      432 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/log-tee.md
--rw-r--r--   0 root         (0) root         (0)     1104 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/log-wait.md
--rw-r--r--   0 root         (0) root         (0)     2913 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/logging.md
--rw-r--r--   0 root         (0) root         (0)     3724 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/networking.md
--rw-r--r--   0 root         (0) root         (0)     4093 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/new-node-support.md
--rw-r--r--   0 root         (0) root         (0)     5669 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/node-bootup.md
--rw-r--r--   0 root         (0) root         (0)     1325 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/node-cp.md
--rw-r--r--   0 root         (0) root         (0)     6402 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/node-install.md
--rw-r--r--   0 root         (0) root         (0)     1595 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/node-netsetup.md
--rw-r--r--   0 root         (0) root         (0)      957 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/node-terminology.md
--rw-r--r--   0 root         (0) root         (0)     4191 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/server-install.md
--rw-r--r--   0 root         (0) root         (0)     9882 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/server-network-config.md
--rw-r--r--   0 root         (0) root         (0)     5166 2021-02-01 15:15:54.000000 walt-client-7/walt/client/doc/md/server-setup-from-fresh-debian.md
--rw-r--r--   0 root         (0) root         (0)     1605 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/server-setup-from-image.md
--rw-r--r--   0 root         (0) root         (0)     7883 2021-02-01 15:15:54.000000 walt-client-7/walt/client/doc/md/server-upgrade.md
--rw-r--r--   0 root         (0) root         (0)     2427 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/shells.md
--rw-r--r--   0 root         (0) root         (0)     4109 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/switch-install.md
--rw-r--r--   0 root         (0) root         (0)    14836 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/tutorial.md
--rw-r--r--   0 root         (0) root         (0)     3926 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/md/vpn.md
--rw-r--r--   0 root         (0) root         (0)     3012 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/mdtable.py
--rwxr-xr-x   0 root         (0) root         (0)     3407 2020-09-24 12:01:14.000000 walt-client-7/walt/client/doc/pager.py
--rwxr-xr-x   0 root         (0) root         (0)     2567 2020-09-24 12:01:14.000000 walt-client-7/walt/client/expose.py
--rw-r--r--   0 root         (0) root         (0)      334 2020-09-24 12:01:14.000000 walt-client-7/walt/client/filesystem.py
--rwxr-xr-x   0 root         (0) root         (0)     6653 2020-09-24 12:01:14.000000 walt-client-7/walt/client/image.py
--rw-r--r--   0 root         (0) root         (0)      678 2021-02-01 15:16:44.000000 walt-client-7/walt/client/info.py
--rwxr-xr-x   0 root         (0) root         (0)     4189 2020-09-24 12:01:14.000000 walt-client-7/walt/client/interactive.py
--rwxr-xr-x   0 root         (0) root         (0)     2198 2020-09-24 12:01:14.000000 walt-client-7/walt/client/link.py
--rwxr-xr-x   0 root         (0) root         (0)    12149 2020-09-24 12:01:14.000000 walt-client-7/walt/client/log.py
--rw-r--r--   0 root         (0) root         (0)     3266 2020-09-24 12:01:14.000000 walt-client-7/walt/client/logo.py
--rw-r--r--   0 root         (0) root         (0)      676 2020-09-24 12:01:14.000000 walt-client-7/walt/client/myhelp.py
--rwxr-xr-x   0 root         (0) root         (0)    10324 2020-09-24 12:01:14.000000 walt-client-7/walt/client/node.py
--rwxr-xr-x   0 root         (0) root         (0)     3119 2020-09-24 12:01:14.000000 walt-client-7/walt/client/startup.py
--rwxr-xr-x   0 root         (0) root         (0)      964 2020-09-24 12:01:14.000000 walt-client-7/walt/client/term.py
--rw-r--r--   0 root         (0) root         (0)      783 2020-09-24 12:01:14.000000 walt-client-7/walt/client/timeout.py
--rw-r--r--   0 root         (0) root         (0)     2304 2020-09-24 12:01:14.000000 walt-client-7/walt/client/tools.py
--rw-r--r--   0 root         (0) root         (0)     3403 2020-09-24 12:01:14.000000 walt-client-7/walt/client/transfer.py
--rwxr-xr-x   0 root         (0) root         (0)     3961 2020-09-24 12:01:14.000000 walt-client-7/walt/client/vpn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-02-01 15:17:02.000000 walt-client-7/walt_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      279 2021-02-01 15:17:02.000000 walt-client-7/walt_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2141 2021-02-01 15:17:02.000000 walt-client-7/walt_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-02-01 15:17:02.000000 walt-client-7/walt_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2021-02-01 15:17:02.000000 walt-client-7/walt_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       64 2021-02-01 15:17:02.000000 walt-client-7/walt_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2021-02-01 15:17:02.000000 walt-client-7/walt_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.076477 walt-client-8.0/
+-rw-r--r--   0 root         (0) root         (0)       32 2022-03-29 14:58:03.000000 walt-client-8.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-23 07:38:23.076477 walt-client-8.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      126 2022-03-29 14:58:03.000000 walt-client-8.0/README.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 07:38:23.076477 walt-client-8.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-06-23 07:37:56.000000 walt-client-8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.072477 walt-client-8.0/walt/
+-rw-r--r--   0 root         (0) root         (0)      147 2023-06-21 15:19:09.000000 walt-client-8.0/walt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.072477 walt-client-8.0/walt/client/
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2443 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/advanced.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.072477 walt-client-8.0/walt/client/apiobject/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)    20082 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/base.py
+-rw-r--r--   0 root         (0) root         (0)     1695 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/config.py
+-rwxr-xr-x   0 root         (0) root         (0)     8074 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/images.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/logs.py
+-rwxr-xr-x   0 root         (0) root         (0)    12837 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/nodes.py
+-rwxr-xr-x   0 root         (0) root         (0)      972 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/root.py
+-rwxr-xr-x   0 root         (0) root         (0)      946 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/server.py
+-rwxr-xr-x   0 root         (0) root         (0)      379 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apiobject/tools.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/apitools.py
+-rwxr-xr-x   0 root         (0) root         (0)     1903 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/application.py
+-rw-r--r--   0 root         (0) root         (0)      565 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/auth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.072477 walt-client-8.0/walt/client/autocomplete/
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/autocomplete/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13122 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/autocomplete/dump.py
+-rwxr-xr-x   0 root         (0) root         (0)     1323 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/autocomplete/helper.py
+-rwxr-xr-x   0 root         (0) root         (0)     1785 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/client.py
+-rw-r--r--   0 root         (0) root         (0)    15266 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/config.py
+-rw-r--r--   0 root         (0) root         (0)     3017 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/console.py
+-rwxr-xr-x   0 root         (0) root         (0)     6644 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/device.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.072477 walt-client-8.0/walt/client/doc/
+-rwxr-xr-x   0 root         (0) root         (0)        0 2022-03-29 14:58:03.000000 walt-client-8.0/walt/client/doc/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     2252 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/color.py
+-rw-r--r--   0 root         (0) root         (0)    12579 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.076477 walt-client-8.0/walt/client/doc/md/
+-rw-r--r--   0 root         (0) root         (0)     1499 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/admin.md
+-rw-r--r--   0 root         (0) root         (0)      317 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/compatibility.md
+-rw-r--r--   0 root         (0) root         (0)     2454 2023-06-22 09:26:07.000000 walt-client-8.0/walt/client/doc/md/design-notes.md
+-rw-r--r--   0 root         (0) root         (0)     2290 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/device-config.md
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/device-expose.md
+-rw-r--r--   0 root         (0) root         (0)     1920 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/device-netsetup.md
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/device-sets.md
+-rw-r--r--   0 root         (0) root         (0)     4413 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/g5k.md
+-rw-r--r--   0 root         (0) root         (0)     4562 2023-06-22 09:26:07.000000 walt-client-8.0/walt/client/doc/md/help-intro.md
+-rw-r--r--   0 root         (0) root         (0)     2803 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/image-build.md
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/image-cp.md
+-rw-r--r--   0 root         (0) root         (0)    13931 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/image-from-scratch.md
+-rw-r--r--   0 root         (0) root         (0)     2157 2022-03-29 14:58:03.000000 walt-client-8.0/walt/client/doc/md/image-spec-file.md
+-rw-r--r--   0 root         (0) root         (0)     1716 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-cat.md
+-rw-r--r--   0 root         (0) root         (0)      927 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-checkpoint.md
+-rw-r--r--   0 root         (0) root         (0)     1678 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-echo.md
+-rw-r--r--   0 root         (0) root         (0)      494 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-format.md
+-rw-r--r--   0 root         (0) root         (0)      727 2022-03-29 14:58:03.000000 walt-client-8.0/walt/client/doc/md/log-history.md
+-rw-r--r--   0 root         (0) root         (0)      525 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-issuers.md
+-rw-r--r--   0 root         (0) root         (0)     2847 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-monitor.md
+-rw-r--r--   0 root         (0) root         (0)      479 2022-03-29 14:58:03.000000 walt-client-8.0/walt/client/doc/md/log-realtime.md
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-show.md
+-rw-r--r--   0 root         (0) root         (0)      432 2022-03-29 14:58:03.000000 walt-client-8.0/walt/client/doc/md/log-tee.md
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/log-wait.md
+-rw-r--r--   0 root         (0) root         (0)     3543 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/logging.md
+-rw-r--r--   0 root         (0) root         (0)     4515 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/networking.md
+-rw-r--r--   0 root         (0) root         (0)     4273 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/new-node-support.md
+-rw-r--r--   0 root         (0) root         (0)     5669 2022-03-29 14:58:03.000000 walt-client-8.0/walt/client/doc/md/node-bootup.md
+-rw-r--r--   0 root         (0) root         (0)      232 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/node-config.md
+-rw-r--r--   0 root         (0) root         (0)     1060 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/node-console.md
+-rw-r--r--   0 root         (0) root         (0)     1325 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/node-cp.md
+-rw-r--r--   0 root         (0) root         (0)      216 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/node-expose.md
+-rw-r--r--   0 root         (0) root         (0)     8365 2023-06-22 09:26:07.000000 walt-client-8.0/walt/client/doc/md/node-install.md
+-rw-r--r--   0 root         (0) root         (0)      364 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/node-netsetup.md
+-rw-r--r--   0 root         (0) root         (0)     2473 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/node-ownership.md
+-rw-r--r--   0 root         (0) root         (0)     3634 2023-06-22 09:26:07.000000 walt-client-8.0/walt/client/doc/md/optional-features.md
+-rw-r--r--   0 root         (0) root         (0)      842 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/packaging.md
+-rw-r--r--   0 root         (0) root         (0)     4895 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/registries.md
+-rw-r--r--   0 root         (0) root         (0)     2555 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/rpi-serial.md
+-rw-r--r--   0 root         (0) root         (0)     5014 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/scripting-images.md
+-rw-r--r--   0 root         (0) root         (0)     4924 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/scripting-logs.md
+-rw-r--r--   0 root         (0) root         (0)     7467 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/scripting-nodes.md
+-rw-r--r--   0 root         (0) root         (0)      643 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/scripting-tools.md
+-rw-r--r--   0 root         (0) root         (0)     5306 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/scripting.md
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/server-install.md
+-rw-r--r--   0 root         (0) root         (0)     9858 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/server-network-config.md
+-rw-r--r--   0 root         (0) root         (0)      788 2023-06-22 14:11:23.000000 walt-client-8.0/walt/client/doc/md/server-upgrade.md
+-rw-r--r--   0 root         (0) root         (0)      736 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/shell-completion.md
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/shells.md
+-rw-r--r--   0 root         (0) root         (0)     4982 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/switch-install.md
+-rw-r--r--   0 root         (0) root         (0)     2715 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/troubleshooting.md
+-rw-r--r--   0 root         (0) root         (0)    14874 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/tutorial.md
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/unmanaged-devices.md
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/md/vnode-networks.md
+-rw-r--r--   0 root         (0) root         (0)     3926 2022-03-29 14:58:03.000000 walt-client-8.0/walt/client/doc/md/vpn.md
+-rw-r--r--   0 root         (0) root         (0)     3286 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/mdtable.py
+-rwxr-xr-x   0 root         (0) root         (0)     9898 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/pager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.076477 walt-client-8.0/walt/client/doc/sphinx/
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/doc/sphinx/conf.py
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-23 07:37:56.000000 walt-client-8.0/walt/client/doc/sphinx/version.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/exceptions.py
+-rwxr-xr-x   0 root         (0) root         (0)     2388 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/expose.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/filesystem.py
+-rwxr-xr-x   0 root         (0) root         (0)    12590 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/image.py
+-rwxr-xr-x   0 root         (0) root         (0)     6593 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/interactive.py
+-rwxr-xr-x   0 root         (0) root         (0)     4545 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/link.py
+-rwxr-xr-x   0 root         (0) root         (0)    14029 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/logo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.076477 walt-client-8.0/walt/client/metadata/
+-rw-r--r--   0 root         (0) root         (0)      238 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/metadata/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/metadata/core.py
+-rw-r--r--   0 root         (0) root         (0)      755 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/myhelp.py
+-rwxr-xr-x   0 root         (0) root         (0)    16940 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/node.py
+-rwxr-xr-x   0 root         (0) root         (0)     2148 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/plugins.py
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/progress.py
+-rw-r--r--   0 root         (0) root         (0)    11444 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/speedup.py
+-rw-r--r--   0 root         (0) root         (0)      218 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/startup.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/timeout.py
+-rw-r--r--   0 root         (0) root         (0)      864 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/tools.py
+-rw-r--r--   0 root         (0) root         (0)     5882 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/transfer.py
+-rw-r--r--   0 root         (0) root         (0)      722 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/types.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/update.py
+-rwxr-xr-x   0 root         (0) root         (0)     3970 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/vpn.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-06-21 15:19:09.000000 walt-client-8.0/walt/client/wrap.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 07:38:23.076477 walt-client-8.0/walt_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-23 07:38:23.000000 walt-client-8.0/walt_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3512 2023-06-23 07:38:23.000000 walt-client-8.0/walt_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 07:38:23.000000 walt-client-8.0/walt_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      110 2023-06-23 07:38:23.000000 walt-client-8.0/walt_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       94 2023-06-23 07:38:23.000000 walt-client-8.0/walt_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-23 07:38:23.000000 walt-client-8.0/walt_client.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `walt-client-7/walt/client/advanced.py` & `walt-client-8.0/walt/client/advanced.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,81 @@
 from plumbum import cli
-from walt.client.link import ClientToServerLink
+from walt.client.application import WalTApplication, WalTCategoryApplication
 from walt.client.interactive import run_sql_prompt
-from walt.client.auth import get_auth_conf
-from walt.client.application import WalTCategoryApplication, WalTApplication
+from walt.client.link import ClientToServerLink
+
 
 class WalTAdvanced(WalTCategoryApplication):
     """advanced sub-commands"""
-    pass
+
+    ORDERING = 6
+
 
 @WalTAdvanced.subcommand("sql")
 class WalTAdvancedSql(WalTApplication):
-    """Start a remote SQL prompt on the WalT server database"""
+    """start a remote SQL prompt on the WalT server database"""
+
     def main(self):
         run_sql_prompt()
 
+
 @WalTAdvanced.subcommand("fix-image-owner")
 class WalTAdvancedFixImageOwner(WalTApplication):
     """fix the owner of images"""
-    _force = False # default
+
+    _force = False  # default
+
     def main(self, other_user):
         if not self._force:
             print("""\
 This will make you own all images of user '%s'. It is intended
 for maintenance only (i.e. if user '%s' is no longer working with
 walt).
 If this is really what you want, run:
 walt advanced fix-image-owner --yes-i-know-do-it-please %s
 """ % ((other_user,) * 3))
         else:
             with ClientToServerLink() as server:
                 server.fix_image_owner(other_user)
-    @cli.autoswitch(help='yes, I know, do it!')
+
+    @cli.autoswitch(help="yes, I know, do it!")
     def yes_i_know_do_it_please(self):
         self._force = True
 
+
 @WalTAdvanced.subcommand("update-hub-meta")
 class WalTUpdateHubMeta(WalTApplication):
     """update hub metadata (docker images pushed without walt)"""
-    _waltplatform_user = False # default
+
+    _waltplatform_user = False  # default
+
     def main(self):
         with ClientToServerLink() as server:
-            auth_conf = get_auth_conf(server)
-            server.update_hub_metadata(auth_conf, self._waltplatform_user)
-    @cli.autoswitch(help='update waltplatform user (walt devs only)')
+            registries = server.get_registries()
+            if "hub" not in tuple(reg_info[0] for reg_info in registries):
+                print(
+                    "Sorry, cannot run this command because the docker hub registry was"
+                    " disabled on this platform."
+                )
+                return False
+            return server.update_hub_metadata(self._waltplatform_user)
+
+    @cli.autoswitch(help="update waltplatform user (walt devs only)")
     def waltplatform_user(self):
         self._waltplatform_user = True
 
+
 @WalTAdvanced.subcommand("rescan-hub-account")
 class WalTRescanHubAccount(WalTUpdateHubMeta):
     """alias to 'update-hub-meta' subcommand"""
+
     pass
+
+
+@WalTAdvanced.subcommand("dump-bash-autocomplete")
+class WalTDumpBashAutocomplete(WalTApplication):
+    """dump bash auto-completion code"""
+
+    def main(self):
+        import walt.client.autocomplete.dump as dumper
+
+        dumper.dump_bash_autocomplete(self)
```

### Comparing `walt-client-7/walt/client/auth.py` & `walt-client-8.0/walt/client/auth.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-from walt.common.crypto.dh import DHPeer
 from walt.common.crypto.blowfish import BlowFish
-from walt.client.config import conf
+from walt.common.crypto.dh import DHPeer
+
 
 # about password encryption:
 # set comment in walt/common/crypto/__init__.py
-def get_auth_conf(server):
+def get_encrypted_credentials(server_pub_key, username, password):
     client_dh_peer = DHPeer()
-    server_dh_peer_id, server_pub_key = server.create_dh_peer()
     client_dh_peer.establish_session(server_pub_key)
-    server.establish_dh_session(server_dh_peer_id, client_dh_peer.pub_key)
     cypher = BlowFish(client_dh_peer.symmetric_key)
-    encrypted_password = cypher.encrypt(conf['password'])
+    encrypted_password = cypher.encrypt(password)
     return dict(
-        username = conf['username'],
-        encrypted_password = encrypted_password,
-        dh_peer_id = server_dh_peer_id
+        username=username,
+        encrypted_password=encrypted_password,
+        client_pub_key=client_dh_peer.pub_key,
     )
```

### Comparing `walt-client-7/walt/client/doc/color.py` & `walt-client-8.0/walt/client/doc/color.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 #!/usr/bin/env python
 import re
 from collections import namedtuple
 
-FORMAT_ATTRS = ['bg_color', 'fg_color', 'underline', 'bold', 'dim']
+FORMAT_ATTRS = ["bg_color", "fg_color", "underline", "bold", "dim"]
 
 # values below match values of escape codes.
 # https://misc.flogisoft.com/bash/tip_colors_and_formatting
-UNDERLINE_ON = '4'
-UNDERLINE_OFF = '24'
-BOLD_ON = '1'
-DIM_ON = '2'
-DIM_AND_BOLD_OFF = '22'
-
-FG_COLOR_DEFAULT = '39'
-FG_COLOR_BLACK = '30'
-FG_COLOR_DARK_YELLOW = '38;5;172'
-FG_COLOR_BLUE = '34'
-FG_COLOR_DARK_RED = '38;5;88'
-
-BG_COLOR_DEFAULT = '49'
-BG_COLOR_WHITE = '107'
-BG_COLOR_LIGHT_GREY = '47'
+UNDERLINE_ON = "4"
+UNDERLINE_OFF = "24"
+BOLD_ON = "1"
+DIM_ON = "2"
+DIM_AND_BOLD_OFF = "22"
+
+FG_COLOR_DEFAULT = "39"
+FG_COLOR_BLACK = "30"
+FG_COLOR_DARK_YELLOW = "38;5;172"
+FG_COLOR_BLUE = "34"
+FG_COLOR_DARK_RED = "38;5;88"
+
+BG_COLOR_DEFAULT = "49"
+BG_COLOR_WHITE = "107"
+BG_COLOR_LIGHT_GREY = "47"
 
-RE_ESC_COLOR = re.compile("\x1b\[[0-9;]*m")
+RE_ESC_COLOR = re.compile("\x1b" + r"\[[0-9;]*m")
 
-class FormatState(namedtuple('FormatState', FORMAT_ATTRS)):
+
+class FormatState(namedtuple("FormatState", FORMAT_ATTRS)):
     def alter(self, **kwargs):
         state = dict(**self._asdict())
         state.update(**kwargs)
         return FormatState(**state)
 
+
 def get_transition_esc_sequence(old_format, new_format):
     transitions = set()
     codes = []
     # start by checking what changed
     for name in FORMAT_ATTRS:
         if getattr(new_format, name) != getattr(old_format, name):
             transitions.add(name)
     # bold and dim have to be carefully processed because of the
     # lack of a portable way to disable one of them individually
-    if 'bold' in transitions and new_format.bold is False:
+    if "bold" in transitions and new_format.bold is False:
         codes.append(DIM_AND_BOLD_OFF)
         if new_format.dim is True:
             codes.append(DIM_ON)
-    elif 'dim' in transitions and new_format.dim is False:
+    elif "dim" in transitions and new_format.dim is False:
         codes.append(DIM_AND_BOLD_OFF)
         if new_format.bold is True:
             codes.append(BOLD_ON)
     else:
-        if 'bold' in transitions:
-            codes.append(BOLD_ON)   # since bold off is treated above
-        if 'dim' in transitions:
-            codes.append(DIM_ON)    # since dim off is treated above
+        if "bold" in transitions:
+            codes.append(BOLD_ON)  # since bold off is treated above
+        if "dim" in transitions:
+            codes.append(DIM_ON)  # since dim off is treated above
     # underline is just a simple boolean
-    if 'underline' in transitions:
+    if "underline" in transitions:
         if new_format.underline is True:
             codes.append(UNDERLINE_ON)
         else:
             codes.append(UNDERLINE_OFF)
     # bg and fg colors are specified as color codes
-    for attr in ('bg_color', 'fg_color'):
+    for attr in ("bg_color", "fg_color"):
         if attr in transitions:
             codes.append(getattr(new_format, attr))
     # build the escape sequence
     if len(codes) == 0:
-        return ''
+        return ""
     else:
-        return '\x1b[' + ';'.join(codes) + 'm'
+        return "\x1b[" + ";".join(codes) + "m"
```

### Comparing `walt-client-7/walt/client/doc/markdown.py` & `walt-client-8.0/walt/client/doc/markdown.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,282 +1,341 @@
 #!/usr/bin/env python
-import commonmark, textwrap
+import termios
+import textwrap
+
 from pygments import highlight
-from pygments.lexers import get_lexer_by_name
 from pygments.formatters import Terminal256Formatter
-import termios
-from walt.client.doc.color import *
+from pygments.lexers import get_lexer_by_name
+from walt.client.doc.color import (
+    BG_COLOR_DEFAULT,
+    BG_COLOR_LIGHT_GREY,
+    BG_COLOR_WHITE,
+    FG_COLOR_BLACK,
+    FG_COLOR_BLUE,
+    FG_COLOR_DARK_RED,
+    FG_COLOR_DARK_YELLOW,
+    FG_COLOR_DEFAULT,
+    RE_ESC_COLOR,
+    FormatState,
+    get_transition_esc_sequence,
+)
 from walt.client.doc.mdtable import detect_table, render_table
-from walt.client.term import TTYSettings
+from walt.common.term import TTYSettings
 
 MAX_TARGET_WIDTH = 120
 
 FG_COLOR_MARKDOWN = FG_COLOR_BLACK
 BG_COLOR_MARKDOWN = BG_COLOR_WHITE
 FG_COLOR_SOURCE_CODE = FG_COLOR_DARK_YELLOW
 BG_COLOR_SOURCE_CODE = BG_COLOR_LIGHT_GREY
 FG_COLOR_URL = FG_COLOR_BLUE
 FG_COLOR_HEADING = FG_COLOR_DARK_RED
 
+
 class MarkdownRenderer:
     def __init__(self, *args, **kwargs):
         self.list_numbering = []
         # initialize context with current terminal setup (default for all attrs)
-        init_state = FormatState(bg_color=BG_COLOR_DEFAULT, fg_color=FG_COLOR_DEFAULT,
-                            underline=False, bold=False, dim=False)
-        self.contexts = [ init_state ]
+        init_state = FormatState(
+            bg_color=BG_COLOR_DEFAULT,
+            fg_color=FG_COLOR_DEFAULT,
+            underline=False,
+            bold=False,
+            dim=False,
+        )
+        self.contexts = [init_state]
         try:
             tty = TTYSettings()
             self.target_width = min(tty.cols, MAX_TARGET_WIDTH)
         except termios.error:
             # Stdout seems not to be a terminal
             self.target_width = 80  # Minimal requirement
-    def render(self, text):
-        parser = commonmark.Parser()
-        ast = parser.parse(text)
+
+    def render(self, ast, selected_link_num):
+        self.link_num = 0
+        self.selected_link_num = selected_link_num
         walker = ast.walker()
-        self.buf = ''
+        self.buf = ""
         event = walker.nxt()
         while event is not None:
-            type_ = event['node'].t
+            type_ = event["node"].t
             if not hasattr(self, type_):
                 raise NotImplementedError(type_)
-            getattr(self, type_)(event['node'], event['entering'])
+            getattr(self, type_)(event["node"], event["entering"])
             event = walker.nxt()
         return self.buf
+
     def document(self, node, entering):
         if entering:
-            self.stack_context( fg_color = FG_COLOR_MARKDOWN,
-                                bg_color = BG_COLOR_MARKDOWN)
+            self.stack_context(fg_color=FG_COLOR_MARKDOWN, bg_color=BG_COLOR_MARKDOWN)
         else:
             # markdown background color should span to right edge
-            self.buf = self.buf.replace('\n', '\033[K\n')
+            self.buf = self.buf.replace("\n", "\033[K\n")
             self.pop_context()
-    def lit(self, s):
+
+    def lit(self, s, reset=False):
+        if reset:
+            self.buf = ""
         self.buf += s
+
     def text(self, node, entering=None):
         self.lit(node.literal)
+
     def stack_context(self, **kwargs):
         curr_state = self.contexts[-1]
         new_state = curr_state.alter(**kwargs)
         self.lit(get_transition_esc_sequence(curr_state, new_state))
         self.contexts.append(new_state)
+
     def pop_context(self):
         curr_state = self.contexts[-1]
         new_state = self.contexts[-2]
         self.lit(get_transition_esc_sequence(curr_state, new_state))
         self.contexts = self.contexts[:-1]
+
     def cr(self):
-        self.lit('\n')
+        self.lit("\n")
+
     def softbreak(self, node=None, entering=None):
         self.cr()
+
     def linebreak(self, node=None, entering=None):
         self.cr()
+
     def html_inline(self, node, entering):
         self.lit(node.literal)
+
     def link(self, node, entering):
-        if entering:
-            pass
+        if node.destination.endswith(".md"):
+            if entering:
+                if self.link_num == self.selected_link_num:
+                    self.stack_context(bold=True, underline=True)
+            else:
+                if self.link_num == self.selected_link_num:
+                    self.pop_context()
+                self.link_num += 1
         else:
-            if node.destination.endswith('.md'):
-                # this is a link for the web browser, ignore here
-                return
-            self.lit(' (')
-            self.stack_context(fg_color = FG_COLOR_URL)
-            self.lit(node.destination)
-            self.pop_context()
-            self.lit(')')
+            if not entering:
+                # replace [<text>](<url>) -> <text> (<url>)
+                self.lit(" (")
+                self.stack_context(fg_color=FG_COLOR_URL)
+                self.lit(node.destination)
+                self.pop_context()
+                self.lit(")")
+
     def paragraph(self, node, entering):
         if entering:
             node.saved_buf = self.buf
-            self.buf = ''
+            self.buf = ""
         else:
             if detect_table(self.buf):
                 table_buf = self.buf
-                self.buf = node.saved_buf
+                self.lit(node.saved_buf, reset=True)
                 render_table(self, table_buf)
             else:
-                self.buf = node.saved_buf + self.wrap_escaped(self.buf)
+                escaped = self.wrap_escaped(self.buf)
+                self.lit(node.saved_buf + escaped, reset=True)
             self.cr()
             self.cr()
+
     def block_quote(self, node, entering):
         if entering:
             node.saved_buf = self.buf
             self.target_width -= 2
-            self.buf = ''
+            self.buf = ""
         else:
             self.buf = node.saved_buf + self.quoted(self.buf)
             self.target_width += 2
             self.cr()
+
     def justify(self, words, num_spaces):
         num_intervals = len(words) - 1
         if num_intervals == 0:
             # only one word, cannot justify
             return words[0]
         # Fill intervals evenly with appropriate number of spaces
-        added_spaces = [ ' ' * (num_spaces//num_intervals)  ] * num_intervals
-        num_spaces -= (num_spaces//num_intervals) * num_intervals
+        added_spaces = [" " * (num_spaces // num_intervals)] * num_intervals
+        num_spaces -= (num_spaces // num_intervals) * num_intervals
         # Because of the integer division, a few remaining spaces should be added
         # (less than the number of intervals).
         # Preferably add one more space after ponctuation marks.
-        for signs in ('.!?', ':;', ','):
+        for signs in (".!?", ":;", ","):
             for i, word in enumerate(words[:-1]):
                 if num_spaces == 0:
                     break
                 if word[-1] in signs:
-                    added_spaces[i] += ' '
+                    added_spaces[i] += " "
                     num_spaces -= 1
         # For better understanding of what we will do with any space still remaining,
         # let's take an example:
         # if we have 15 intervals and 4 remaining spaces, distribute evenly
         # these 4 spaces at intervals 1*15/5=3, 2*15/5=6, 3*15/5=9 and 4*15/5=12.
-        for i in range(1, num_spaces+1):
-            added_spaces[i*num_intervals//(num_spaces+1)] += ' '
+        for i in range(1, num_spaces + 1):
+            added_spaces[i * num_intervals // (num_spaces + 1)] += " "
         # add a fake ending 'interval' for the zip() function below
-        added_spaces += [ '' ]
-        return ''.join((word + spacing) for word, spacing in zip(words, added_spaces))
+        added_spaces += [""]
+        return "".join((word + spacing) for word, spacing in zip(words, added_spaces))
+
     def real_text_len(self, text):
-        return len(''.join(RE_ESC_COLOR.split(text)))
+        return len("".join(RE_ESC_COLOR.split(text)))
+
     def wrap_escaped(self, text):
         # textwrap.fill does not work well because of the escape sequences
         wrapped_lines = []
         curr_words = []
         curr_words_no_color = []
-        for line in text.split('\n'):
-            for word in line.split(' '):
-                word_no_color = ''.join(RE_ESC_COLOR.split(word))
-                min_line_no_color = ' '.join(curr_words_no_color + [ word_no_color ])
+        for line in text.split("\n"):
+            for word in line.split(" "):
+                word_no_color = "".join(RE_ESC_COLOR.split(word))
+                min_line_no_color = " ".join(curr_words_no_color + [word_no_color])
                 min_len = len(min_line_no_color)
                 if 1 + min_len > self.target_width:
                     # cannot include the new word, format previous ones into a line
-                    len_no_space = len(''.join(curr_words_no_color))
+                    len_no_space = len("".join(curr_words_no_color))
                     num_spaces = self.target_width - 1 - len_no_space
                     curr_line = self.justify(curr_words, num_spaces)
-                    wrapped_lines.append(' ' + curr_line)
+                    wrapped_lines.append(" " + curr_line)
                     # the new word will be included into next line
-                    curr_words = [ word ]
-                    curr_words_no_color = [ word_no_color ]
+                    curr_words = [word]
+                    curr_words_no_color = [word_no_color]
                 else:
                     # ok, include this new word into the current line
                     curr_words.append(word)
                     curr_words_no_color.append(word_no_color)
-            wrapped_lines.append(' ' + ' '.join(curr_words))
+            wrapped_lines.append(" " + " ".join(curr_words))
             curr_words, curr_words_no_color = [], []
         # after wrapping is validated, we can revert non-breaking spaces
         # to regular space.
-        return '\n'.join(wrapped_lines).replace('\xa0', ' ')
+        return "\n".join(wrapped_lines).replace("\xa0", " ")
+
     def quoted(self, text):
-        return '\n'.join((' \u2588' + line) for line in text.rstrip('\n').split('\n')) + '\n'
+        return (
+            "\n".join((" \u2588" + line) for line in text.rstrip("\n").split("\n"))
+            + "\n"
+        )
+
     def heading(self, node, entering):
         if entering:
             level = 1 if node.level is None else node.level
             self.cr()
-            self.stack_context(fg_color = FG_COLOR_HEADING, bold = True)
-            self.lit('#'*level + ' ')
+            self.stack_context(fg_color=FG_COLOR_HEADING, bold=True)
+            self.lit("#" * level + " ")
             self.underline(None, True)
         else:
             self.underline(None, False)
             self.pop_context()
             self.cr()
             self.cr()
+
     def underline(self, node, entering):
         if entering:
-            self.stack_context(underline = True)
+            self.stack_context(underline=True)
         else:
             self.pop_context()
+
     def strong(self, node, entering):
         if entering:
-            self.stack_context(bold = True)
+            self.stack_context(bold=True)
         else:
             self.pop_context()
+
     def emph(self, node, entering):
         if entering:
-            self.stack_context(dim = True)
+            self.stack_context(dim=True)
         else:
             self.pop_context()
+
     def code(self, node, entering):
-        self.stack_context( fg_color = FG_COLOR_SOURCE_CODE,
-                            bg_color = BG_COLOR_SOURCE_CODE)
+        self.stack_context(fg_color=FG_COLOR_SOURCE_CODE, bg_color=BG_COLOR_SOURCE_CODE)
         # replace spaces with non-breaking space
         # (this should be reverted after the paragraph has been wrapped, see above)
-        self.lit(node.literal.replace(' ', '\xa0'))
+        self.lit(node.literal.replace(" ", "\xa0"))
         self.pop_context()
+
     def pre_format_code_block(self, text):
         text = textwrap.dedent(text)
-        text = '\n'.join(line.rstrip() for line in text.rstrip('\n').split('\n'))
+        text = "\n".join(line.rstrip() for line in text.rstrip("\n").split("\n"))
         return text
+
     # Since pygments output includes escape codes to reset the foreground
     # or background color, we have to make a pass to revert those escape
     # codes and get the default colors we want.
     def fix_pygments_default_colors(self, s, default_fg, default_bg):
         reset_all = "0;%s;%s" % (str(default_fg), str(default_bg))
         mapping = {
-                    39: str(default_fg), # default fg color
-                    49: str(default_bg), # default bg color
-                     0: reset_all
+            39: str(default_fg),  # default fg color
+            49: str(default_bg),  # default bg color
+            0: reset_all,
         }
-        s2 = ''
+        s2 = ""
         start = 0
         end = 0
         for m in RE_ESC_COLOR.finditer(s):
             start = m.start()
-            s2 += s[end:start] + '\x1b['
-            codes = (int(c) for c in m.group()[2:-1].split(';'))
-            s2 += ';'.join(mapping.get(code, str(code)) for code in codes) + 'm'
+            s2 += s[end:start] + "\x1b["
+            codes = (int(c) for c in m.group()[2:-1].split(";"))
+            s2 += ";".join(mapping.get(code, str(code)) for code in codes) + "m"
             end = m.end()
         s2 += s[end:]
         return s2
+
     def code_block(self, node, entering):
         code_text = self.pre_format_code_block(node.literal)
-        code_width = max(len(line) for line in code_text.split('\n')) + 1
+        code_width = max(len(line) for line in code_text.split("\n")) + 1
         code_width = max(code_width, self.target_width)
         try:
             lexer = get_lexer_by_name(node.info)
             colored_text = highlight(code_text, lexer, Terminal256Formatter())
-            colored_text = self.fix_pygments_default_colors(colored_text,
-                                   FG_COLOR_SOURCE_CODE, BG_COLOR_SOURCE_CODE)
-        except:
+            colored_text = self.fix_pygments_default_colors(
+                colored_text, FG_COLOR_SOURCE_CODE, BG_COLOR_SOURCE_CODE
+            )
+        except Exception:
             colored_text = code_text
         for code_line, colored_line in zip(
-                    code_text.split('\n'), colored_text.split('\n')):
-            self.stack_context( fg_color = FG_COLOR_SOURCE_CODE,
-                                bg_color = BG_COLOR_SOURCE_CODE)
+            code_text.split("\n"), colored_text.split("\n")
+        ):
+            self.stack_context(
+                fg_color=FG_COLOR_SOURCE_CODE, bg_color=BG_COLOR_SOURCE_CODE
+            )
             # paste the colored line, then kill ('\e[K') in order to paint the rest
             # with background color of source code, then move to the right ('\e[<N>C')
             # up to the edge of code block
-            self.lit(colored_line + '\x1b[K\x1b[%dC' % (code_width-len(code_line)))
+            self.lit(colored_line + "\x1b[K\x1b[%dC" % (code_width - len(code_line)))
             # this will restore markdown background color
             self.pop_context()
             # line feed
             self.cr()
         self.cr()
+
     def list(self, node, entering):
         if entering:
-            if node.list_data['type'] == 'bullet':
+            if node.list_data["type"] == "bullet":
                 self.list_numbering.append(None)
             else:
                 self.list_numbering.append(1)
         else:
             self.list_numbering = self.list_numbering[:-1]
             self.cr()
+
     def item(self, node, entering):
         if entering:
             node.saved_buf = self.buf
-            self.buf = ''
+            self.buf = ""
             numbering = self.list_numbering[-1]
-            node.prefix = '  ' * len(self.list_numbering)
+            node.prefix = "  " * len(self.list_numbering)
             if numbering is None:
-                node.prefix += '\u2022 '
+                node.prefix += "\u2022 "
             else:
-                node.prefix += '%d. ' % numbering
+                node.prefix += "%d. " % numbering
                 self.list_numbering[-1] += 1
             self.target_width -= len(node.prefix)
         else:
             self.buf = node.saved_buf + self.item_prefix(self.buf, node.prefix)
             self.target_width += len(node.prefix)
+
     def item_prefix(self, text, prefix):
         out = []
-        for line in text.rstrip('\n').split('\n'):
+        for line in text.rstrip("\n").split("\n"):
             out.append(prefix + line)
             # from 2nd line, prefix is all space
-            prefix = ' ' * len(prefix)
-        return '\n'.join(out) + '\n'
+            prefix = " " * len(prefix)
+        return "\n".join(out) + "\n"
```

### Comparing `walt-client-7/walt/client/doc/md/device-config.md` & `walt-client-8.0/walt/client/doc/md/device-config.md`

 * *Files 10% similar despite different names*

```diff
@@ -9,33 +9,38 @@
 $ walt node config virt-node ram=384M           # modify
 ```
 
 One may also show or change several settings at once, and/or show or update them on several devices at once. (See also: [`walt help show device-sets`](device-sets.md))
 For instance:
 ```
 $ walt device config all-switches               # show
-$ walt device config all-switches lldp.explore=true poe.reboot=true
+$ walt device config all-switches lldp.explore=true poe.reboots=true
 $ walt node config virt-node-1,virt-node-2 ram=384M
 ```
 
 You can also use this command to indicate to walt server that an unknown device is actually a switch:
 ```
 $ walt device config unknown-a2f2d3 type=switch
 ```
 
 Here is the set of settings currently allowed:
 
-| Name           | possible values        | Applies to:       | Notes |
-|----------------|------------------------|-------------------|-------|
-| lldp.explore   | true or false          | switches          | (1)   |
-| poe.reboots    | true or false          | switches          | (1)   |
-| snmp.version   | 1 or 2                 | switches          | (1)   |
-| snmp.community | e.g. 'private'         | switches          | (1)   |
-| type           | 'switch'               | 'unknown' devices | (2)   |
-| netsetup       | 'NAT' or 'LAN'         | nodes             | (3)   |
-| ram            | e.g. '384M' or '1G'    | virtual nodes     |       |
-| cpu.cores      | e.g. 1 or 4            | virtual nodes     |       |
+| Name           | possible values         | Applies to:         | Notes |
+|----------------|-------------------------|---------------------|-------|
+| lldp.explore   | true or false           | switches            | (1)   |
+| poe.reboots    | true or false           | switches            | (1)   |
+| snmp.version   | 1 or 2                  | switches            | (1)   |
+| snmp.community | e.g. 'private'          | switches            | (1)   |
+| type           | 'switch'                | 'unknown' devices   | (2)   |
+| netsetup       | 'NAT' or 'LAN'          | devices of walt-net | (3)   |
+| ram            | e.g. '384M' or '1G'     | virtual nodes       |       |
+| cpu.cores      | e.g. 1 or 4             | virtual nodes       |       |
+| disks          | e.g. '8G' or '32G,1T'   | virtual nodes       |       |
+| networks       | e.g. 'walt-net,ext-net' | virtual nodes       | (4)   |
+| kexec.allow    | true or false           | nodes               | (5)   |
 
 Notes:
 1. See [`walt help show switch-install`](switch-install.md)
 2. Only allowed when changing device type from 'unknown' to 'switch'
-3. See [`walt help show node-netsetup`](node-netsetup.md)
+3. See [`walt help show device-netsetup`](device-netsetup.md)
+4. See [`walt help show vnode-networks`](vnode-networks.md)
+5. Default is true: allow kexec-rebooting if the optional script `[walt-image]:/bin/walt-reboot` implements it.
```

### Comparing `walt-client-7/walt/client/doc/md/device-sets.md` & `walt-client-8.0/walt/client/doc/md/device-sets.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# Device and node sets: targetting several devices in a single walt command
+# Device and node sets: use several devices at once
 
 Many walt commands allow you to target several devices (e.g. nodes, switches) at once.
 
 For instance:
 ```
 $ walt node run my-nodes hostname
 ```
@@ -16,13 +16,14 @@
 To specify this kind of command parameter, the following options are allowed:
 * specify a single device (e.g. `node1`)
 * specify a coma-separated list of devices (e.g. `node1,node2,node3`) with no space
 * use one of the predefined sets (see below)
 * combine previous options (e.g. `server,explorable-switches`)
 
 Here is the list of predefined sets:
-* `my-nodes`: nodes the user currently owns
+* `my-nodes`: nodes the user currently owns (see [`walt help show node-ownership`](node-ownership.md))
+* `free-nodes`: nodes that no one currently owns
 * `all-nodes`: all nodes of the platform
 * `all-switches`: all switches of the platform
 * `all-devices`: all devices (nodes, switches, unknown devices, and the server)
 * `explorable-switches`: all switches with `lldp.explore` set to `true`
```

### Comparing `walt-client-7/walt/client/doc/md/image-cp.md` & `walt-client-8.0/walt/client/doc/md/image-cp.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# transfering files to or from a walt image
+# Transfering files to or from a walt image
 
 `walt image cp` allows to transfer files to or from a walt image.
 Its interface is very similar to `scp`, but simplified. Two forms are allowed:
 ```
 $ walt image cp <image>:<path> <local-path>
 $ walt image cp <local-path> <image>:<path>
 ```
```

### Comparing `walt-client-7/walt/client/doc/md/image-from-scratch.md` & `walt-client-8.0/walt/client/doc/md/image-from-scratch.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Creating a WalT image from scratch
 
-Most users just need to modify existing images built by other users, such as the official images build by walt platform developers (with docker user `waltplatform`). In order to modify an image easily, they can use `walt image shell` or `walt image cp`. However, for specific needs, it is sometimes useful to create a whole new operating system image for WalT. This page describes how to achieve this.
+Most users just need to modify existing images built by other users, such as the official images build by walt platform developers (with docker user `waltplatform`). In order to modify an image easily, they can use `walt image shell`, [`walt image cp`](image-cp.md) or [`walt image build`](image-build.md). However, for specific needs, it is sometimes useful to create a whole new operating system image for WalT. This page describes how to achieve this.
 
 This procedure is dedicated to advanced users that are familiar with operating systems operation and `docker` classical tools.
 
 ## A) Introduction
 
 A WalT image is just a [docker image](https://docs.docker.com/engine/getstarted/); as such, you can use docker usual procedure to build it:
 * create a Dockerfile
@@ -117,15 +117,15 @@
 ### 6- an init system
 
 The init system of your image should be available at `/sbin/init`.
 
 ### 7- busybox and classical unix commands
 
 For proper handling of the bootup procedure, you should provide a `busybox` multi-call binary at `/bin/busybox`.
-This busybox binary should at least include the following applets: `awk` `cat` `chroot` `ls` `mktemp` `mkfifo` `nc` `reboot` `rm` `sed` `sh` `sleep` `timeout`.
+This busybox binary should at least include the following applets: `awk` `cat` `chroot` `ls` `mktemp` `mkfifo` `nc` `realpath` `reboot` `rm` `sed` `sh` `sleep` `timeout` `uname`.
 If this busybox binary is not statically compiled (on a debian-based image: `apt-get install busybox-static`), you must also provide a `ldd` binary.
 
 The following commands should also be provided in the image (either through `busybox` applets or not, it does not matter):
 `chmod` `chroot` `cp` `date` `echo` `grep` `head` `ln` `mkdir` `mount` `reboot` `sed` `setsid` `sh` `timeout` `tr` `umount`.
 
 ### 8- a ssh server set up to listen on port 22
 
@@ -226,21 +226,47 @@
 
 ```
 $ apt-get install avahi-daemon libnss-mdns
 ```
 
 ### 4- walt-node python package
 
-If your image provides python2.7 and systemd, you can install the walt-node python package:
+If your image provides python3.6+ and systemd, you can install the walt-node python package:
 
 ```
-$ pip install walt-node
+$ pip3 install walt-node
+$ walt-node-setup
 ```
 
-This will provide enhanced walt logging features (see [`walt help show logging`](logging.md)). Note that without this package, you can still use the standard logging features.
+This will provide:
+* Enhanced walt logging features (see [`walt help show logging`](logging.md)). Note that without this package, you can still use the standard logging features.
+* Tool `walt-ipxe-kexec-reboot`, allowing to implement faster reboots. This only works if the image is based on iPXE boot scripts and has kexec tool installed. To enable this, link this command to `/bin/walt-reboot` (see below).
 
 ### 5- led-blinking script
 
 The `walt node blink <node-name>` command may be used to visually identify a node, by making a led blink.
 
 This will work only if the image provides an executable file at `/bin/blink`. Calling `/bin/blink 1` should make the led start to blink, `/bin/blink 0` should make it stop.
 
+### 6- custom reboot script
+
+If the image provides an executable command `/bin/walt-reboot`, then this command will be called when (soft-)rebooting the node.
+
+Providing this file may be useful in various cases. For instance:
+* Ensuring a result file is flushed in `/persist` before rebooting
+* Providing a faster way to reboot, e.g. kexec
+
+If `/bin/walt-reboot` returns, even successfully, the calling script `walt-net-service` will consider the reboot failed and run `busybox reboot -f`.
+
+Caution: if providing an advanced way to reboot (e.g. kexec), one must take care not blindly rebooting the same kernel and initrd: the node may have been associated to a different image.
+
+### 7- label "walt.image.preferred-name"
+
+If this image will be the default image for several new node models, one may specify this label to indicate the "preferred image name" (see explanation below).
+For example:
+
+```
+LABEL walt.image.preferred-name="rpi-default:latest"
+```
+
+When a new user types `walt image show` for the first time, a set of default images is automatically cloned. These are the default images for the node models already present on the platform.
+However, a default image often handles several node models. For instance, the default image for raspberry pi boards can handle all B models, from rpi-b to rpi-4-b. In earlier walt versions, the new user obtained various clones of this image, named `rpi-b-default`, `rpi-b-plus-default`, ... and `rpi-4-b-default` (as long as all these models are present on the platform). Now only one clone will be created, and it will be named according to this label if defined.
```

### Comparing `walt-client-7/walt/client/doc/md/image-spec-file.md` & `walt-client-8.0/walt/client/doc/md/image-spec-file.md`

 * *Files identical despite different names*

### Comparing `walt-client-7/walt/client/doc/md/log-cat.md` & `walt-client-8.0/walt/client/doc/md/log-cat.md`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ```
 
 This will catch all loglines emitted from my nodes. (see [`walt help show log-realtime`](log-realtime.md) for more info)
 
 Then, on a second terminal:
 ```
 $ walt node shell node1
-Caution: changes will be lost on next node reboot.
+Caution: changes outside /persist will be lost on next node reboot.
 Run 'walt help show shells' for more info.
 
 root@node1:~# dmesg | walt-log-cat kernel-log
 root@node1:~#
 ```
 
 And immediately log lines are catched on first terminal:
```

### Comparing `walt-client-7/walt/client/doc/md/log-checkpoint.md` & `walt-client-8.0/walt/client/doc/md/log-checkpoint.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# log checkpoints
+# Log checkpoints
 
 A checkpoint is a kind of marker in time. It allows to easily reference the associated point in time by just giving its name.
 
 Here is a sample workflow:
 ```
 $ walt log add-checkpoint exp1-start
 [... run experience exp1 ...]
```

### Comparing `walt-client-7/walt/client/doc/md/log-echo.md` & `walt-client-8.0/walt/client/doc/md/log-echo.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ```
 
 This will catch all loglines emitted from my nodes. (see [`walt help show log-realtime`](log-realtime.md) for more info)
 
 Then, on a second terminal:
 ```
 $ walt node shell node1
-Caution: changes will be lost on next node reboot.
+Caution: changes outside /persist will be lost on next node reboot.
 Run 'walt help show shells' for more info.
 
 root@node1:~# walt-log-echo 'exp1' 'this is a logline of exp1'
 root@node1:~#
 ```
 
 And immediately the logline is catched on first terminal:
```

### Comparing `walt-client-7/walt/client/doc/md/log-history.md` & `walt-client-8.0/walt/client/doc/md/log-history.md`

 * *Files identical despite different names*

### Comparing `walt-client-7/walt/client/doc/md/log-monitor.md` & `walt-client-8.0/walt/client/doc/md/log-monitor.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 ```
 
 There is, however, a difference: `walt-log-monitor` will run `<command...>` in a virtual terminal. Therefore, `<command...>` should behave exactly the same whether you typed it directly or you prefixed with `walt-log-monitor`.
 We wrote this tool because some commands act differently when then detect their output is not a terminal. For example, if `tcpdump` detects its output is a pipe (like in the `walt-log-cat` construct), it will bufferize its output differently. As a result, you may get different results whether you type the command alone or with the pipe plus `walt-log-cat` construct. On the contrary, it should act exactly the same if you prefix the command with `walt-log-monitor`.
 
 ## Installation
 
-If your image does not provide `walt-log-monitor`, but it already provides python and systemd, then you can get it by installing python package `walt-node`:
+If your image does not provide `walt-log-monitor`, but it already provides python3.6+ and systemd, then you can get it by installing python package `walt-node`:
 ```
-[image-shell]$ pip install walt-node
-[image-shell]$ walt-setup-systemd
+[image-shell]$ pip3 install walt-node
+[image-shell]$ walt-node-setup
 ```
 
 ## Simple example
 
 I first run this in a first terminal:
 ```
 $ walt log show --realtime
@@ -42,15 +42,15 @@
 ```
 
 This will catch all loglines emitted from my nodes. (see [`walt help show log-realtime`](log-realtime.md) for more info)
 
 Then, on a second terminal:
 ```
 $ walt node shell node1
-Caution: changes will be lost on next node reboot.
+Caution: changes outside /persist will be lost on next node reboot.
 Run 'walt help show shells' for more info.
 
 root@node1:~# walt-log-monitor tcpdump -l -i wlan0
 tcpdump: verbose output suppressed, [...]
 listening on eth0, link-type EN10MB [...]
 10:57:58.4151 IP 10.8.1.3.85 > 10.8.1.1.56: [...]
 10:57:58.4157 IP 10.8.1.1.56 > 10.8.1.3.85: [...]
```

### Comparing `walt-client-7/walt/client/doc/md/log-wait.md` & `walt-client-8.0/walt/client/doc/md/log-wait.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 # Synchronizing a script based on expected logs
 
 `walt log wait` allows to wait for a given log trace to be emitted. The command returns when it occurs.
 
-Option `--nodes` allows to specify the set of nodes monitored. If unspecified, the nodes you own (see [`walt help show node-terminology`](node-terminology.md)) will be selected.
+Option `--issuers` allows to specify the set of devices monitored. If unspecified, the nodes you own (see [`walt help show node-ownership`](node-ownership.md)) will be selected.
 
-The default behavior (`--mode ANY`) of this command is to wait until a logline emitted by **one** of the selected nodes matches the specified regular expression. In some cases, one may require a different behavior by using option `--mode ALL`. With this option, the command will wait until **all** selected nodes emit a given logline.
+The default behavior (`--mode ANY`) of this command is to wait until a logline emitted by **one** of the selected issuers matches the specified regular expression. In some cases, one may require a different behavior by using option `--mode ALL`. With this option, the command will wait until **all** selected issuers emit a given logline.
 
 For example, let's consider an experiment run using scripts automatically started on node's bootup. These scripts send a logline `"DONE"` at the end of the experiment. In order to wait until all nodes are done with the experiment, the user can use:
 ```
 $ walt node wait --mode ALL --nodes node1,node2,node3 DONE
 ```
 This command will return when a logline including `"DONE"` has been received from all the specified experiment nodes.
```

### Comparing `walt-client-7/walt/client/doc/md/logging.md` & `walt-client-8.0/walt/client/doc/md/logging.md`

 * *Files 26% similar despite different names*

```diff
@@ -3,20 +3,40 @@
 
 ## Introduction
 
 WalT provides a subsystem to save and query experiment logs. This page describes how this subsystem works and how to use it.
 
 Let's start with some basic notions:
 * A **logline** is a line of text transmitted from a node to the server, and then to any client that would query it.
-* A **timestamp** and a **sender** (the WalT node that emitted it) is associated with each logline.
+* A **timestamp** and an **issuer** (the device that emitted it, i.e. a node or the server) is associated with each logline.
 * A **logstream** is a subset of loglines. Logstreams have a name, which can be used to filter logs easily.
 
 All loglines and logstreams are saved in a database on the server.
 
-## How to generate experiment logs
+Two kinds of logs exist:
+* Platform-generated logs
+* Experiment logs
+
+
+## Platform logs
+
+The platform generates log lines by itself when an important event occurs, or for debugging purpose.
+
+For instance, the following command displays log lines in realtime when an important event occur:
+```
+$ walt log show --realtime --platform
+```
+
+This other example fetches and displays walt server daemon logs generated during the 5 last minutes:
+```
+$ walt log show --history -5m: --server
+```
+
+
+## Experiment logs
 
 WalT will not generate experiment logs by itself. However, all WalT nodes provide tools you can use in order to emit loglines while your experiment is running. For example, you could write an experiment script `experiment1.sh` such as:
 ```bash
 #!/bin/bash
 
 init_exp()
 {
@@ -59,20 +79,21 @@
 
 Do not hesitate to check their respective help page.
 These tools are actually copied by the server, before an image is made accessible to nodes through TFTP and NFS. This ensures that these tools will always be available on nodes.
 
 Another tool is provided on a subset of WalT images:
 * `walt-log-monitor`  (see [`walt help show log-monitor`](log-monitor.md))
 
-This one is not always available because it is based on a python package, and some minimal images may not provide python. In order to install it in your own images, if it is missing, you can use `pip install walt-node`.
+This one is not always available because it is based on a python package and systemd, and some minimal images may not provide python3 or systemd. See [`walt help show log-monitor`](log-monitor.md) for installing it when it is missing.
 
 ## How to query / display / work with experiment logs
 
-The main entrypoint to display experiment logs is subcommand `walt log show`.
+The main entrypoint to display experiment logs is subcommand `walt log show` (see [`walt help show log-show`](log-show.md)).
 
-Depending on what you want to achieve, checkout the appropriate help page in the following list.
+Depending on what you want to achieve, you may get more information in the following help pages:
 
 * Retrieving past logs: [`walt help show log-history`](log-history.md)
 * Printing logs in real time: [`walt help show log-realtime`](log-realtime.md)
 * Updating log display format: [`walt help show log-format`](log-format.md)
+* Filtering log issuers: [`walt help show log-issuers`](log-issuers.md)
 * Synchronizing a script based on logs: [`walt help show log-wait`](log-wait.md)
 * Using log checkpoints: [`walt help show log-checkpoint`](log-checkpoint.md)
```

### Comparing `walt-client-7/walt/client/doc/md/networking.md` & `walt-client-8.0/walt/client/doc/md/networking.md`

 * *Files 24% similar despite different names*

```diff
@@ -30,50 +30,68 @@
 
 
 ## walt-net and walt-out networks
 
 As shown in the figure, there are two main requirements regarding network setup:
 * The server should have internet connectivity, in order to be able to communicate with the docker hub.
   In these documentation pages, this is sometimes refered as `walt-out`.
-* The platform LAN (or VLAN) MUST be fully dedicated to WALT. The WALT server will fully manage this
-  platform network, by providing various network services, such as DHCP, NFS, TFTP, PTP, etc. We call
-  this platform network `walt-net` in these documentation pages and in configuration files.
+* The platform LAN (or, sometimes, VLAN) MUST be fully dedicated to WALT. The WALT server will fully
+  manage this platform network, by providing various network services, such as DHCP, NFS, TFTP, etc.
+  We call this platform network `walt-net` in these documentation pages and in configuration files.
 
 Of course we can cascade several switches to extend `walt-net`, as shown on the figure.
 Caution: connecting a walt node directly to the server (with no intermediate switch) will not work!
 
 Isolating networks `walt-net` and `walt-out` allows better experiment reproducibility. Thus, in the
 default configuration, they are isolated one from each other. However, one can alter this configuration
 and allow a specific set of nodes to access internet. Check-out [`walt help show node-netsetup`](node-netsetup.md)
 for more info.
 
 
-## Network switch remote administration features
+## walt-adm: optional admin network
 
-The WALT server, if allowed, may send SNMP queries to a given switch, for one of these two purposes:
-* retrieve LLDP data (Link Layer Discovery Protocol), for network discovery
-* activate / deactivate PoE on one of the ports (for remotely hard-rebooting a walt node)
+If WALT is installed in a building and reuses an existing network infrastructure, there is usually
+a dedicated VLAN already in place for remote administration of switches.
 
-These two requests are disabled by default. You can activate and configure them for a given switch
-using `walt device config <switch> <parameter>...` (see [`walt help show device-config`](device-config.md)).
+Instead of allowing remote administration (i.e. SNMP requests, see below) from network `walt-net`,
+admins usually prefer to give the WALT server access to this dedicated admin network.
 
-Of course this is only possible if the switch provides related features.
-Check-out [`walt help show switch-install`](switch-install.md) for more info.
+We call this optional network `walt-adm` in these documentation pages and in configuration files.
 
 
-## walt-adm: optional network admin network
+## Configuring WalT
 
-If WALT is installed in a building and reuses an existing network infrastructure, there is usually
-a dedicated VLAN already in place for remote administration of switches.
+WalT networking configuration is responsible for defining `walt-net` and optionally `walt-adm`.
+`walt-out` is out of scope because the default OS configuration providing internet connectivity
+is fine.
+
+This configuration is most easily modified by running `walt-server-setup --edit-conf`.
+Check-out [`walt help show server-network-config`](server-network-config.md) for more info.
+
+It is possible to configure a virtual-only platform where `walt-net` is not linked to a physical
+network interface. In this case, it will not be possible to detect physical nodes, but users can
+still work with virtual nodes. Such a virtual-only platform can be reconfigured later to accept
+physical nodes by running `walt-server-setup --edit-conf` again.
 
-Instead of allowing remote administration (i.e. SNMP requests) from network `walt-net`, admins usually
-prefer to give the WALT server access to this dedicated admin network.
 
-We call this optional network `walt-adm` in these documentation pages and in configuration files.
+## Network switch remote administration features
+
+When configured to do so, the WALT server may send SNMP queries to a given switch, for one of these
+purposes:
+* retrieve LLDP data (Link Layer Discovery Protocol), for network discovery
+* activate / deactivate PoE on one of the ports (for remotely hard-rebooting a walt node or saving power)
+
+These requests are disabled by default. You can activate and configure them for a given switch
+using `walt device config <switch> <parameter>...` (see [`walt help show device-config`](device-config.md)).
+
+Of course this is only possible if the switch provides related features.
+See [`walt help show optional-features`](optional-features.md) for more info.
 
 Note that if `walt-adm` is configured, WALT may send SNMP requests on both `walt-net` and `walt-adm`
 networks. To clarify, let's consider WALT has been installed in a large building, and some wall plugs
-have been dedicated to the experimentation network (thus there are associated to `walt-net`).
-In order to perform an small experiment with a few nodes on your desk, you could connect a small
+have been dedicated to the experimentation network (thus they are associated to `walt-net`).
+In order to perform a small experiment with a few nodes on your desk, you could connect a small
 switch to one of these wall plugs, and connect your nodes on it. In this case, WALT will have to use
 `walt-net` to reach this small switch, and `walt-adm` to reach the switch managing the wall plug.
 
+
+
```

### Comparing `walt-client-7/walt/client/doc/md/new-node-support.md` & `walt-client-8.0/walt/client/doc/md/new-node-support.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 # Adding support for a new node in WalT
 
 ## Introduction
 
 WalT is currently provided with support for several kinds of nodes:
-* Raspberry Pi boards: models B, B+, 2B, 3B and 3B+
+* Raspberry Pi boards: models B, B+, 2B, 3B, 3B+ and 4B
 * Standard PC machines (x86 32bit or 64bit CPU)
 * Virtual nodes
 
 Check-out [`walt help show node-install`](node-install.md) for more info.
 
 But WalT can also support any other kind of hardware, without having to update
 its internal source code.
@@ -20,14 +20,19 @@
 First, you should open an issue at https://github.com/drakkar-lig/walt-python-packages/issues
 in order to let us assist you in this process.
 
 On the technical side, support for a new kind of node in WalT requires:
 * A network bootloader with appropriate configuration
 * A default walt image that will be assigned to newly detected nodes of this kind
 
+In the meantime, or if this process proves impossible to achieve (e.g., there is no
+way to flash a network bootloader on this device), the WalT platform can still provide
+a limited set of useful features to interact with unmanaged devices
+(cf. [`walt help show unmanaged-devices`](unmanaged-devices.md)).
+
 
 ## Network bootloader
 
 First, you may clone git repository https://github.com/drakkar-lig/walt-node-boot.
 This repository currently allows to generate SD card content of walt raspberry pi nodes, and
 USB device image of walt PC nodes. It can be a good starting point. Feel free to issue a
 pull request if you want your work on this repository to be included.
@@ -56,18 +61,16 @@
 
 
 ## Default walt image
 
 In order to create a default walt image appropriate for this board, you should check out
 [`walt help show image-from-scratch`](image-from-scratch.md).
 
-As an example, the default image of raspberry pi boards is generated by the repository at:
-https://github.com/drakkar-lig/walt-rpi-debian.
-And the default image of PC nodes is generated by the repository at:
-https://github.com/drakkar-lig/walt-pc-debian.
+As an example, the default images we provide are generated by the repository at:
+https://github.com/drakkar-lig/walt-images.
 
 In order to let walt use your image as the default for this node type, you must import it
 in walt own repository and rename it to `waltplatform/<node-type>-default:latest`.
 For this, run the following as root on the server:
 ```
 $ podman pull docker-daemon:<docker-image>:<tag>
 $ podman tag docker.io/<docker-image>:<tag> docker.io/waltplatform/<node-type>-default:latest
```

### Comparing `walt-client-7/walt/client/doc/md/node-bootup.md` & `walt-client-8.0/walt/client/doc/md/node-bootup.md`

 * *Files identical despite different names*

### Comparing `walt-client-7/walt/client/doc/md/node-cp.md` & `walt-client-8.0/walt/client/doc/md/node-cp.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# transfering files to or from a node
+# Transfering files to or from a node
 
 `walt node cp` allows to transfer files to or from a node.
 Its interface is very similar to `scp`, but simplified. Three forms are allowed:
 ```
 $ walt node cp <node>:<path> <local-path>
 $ walt node cp <local-path> <node>:<path>
 $ walt node cp <node>:<path> booted-image
```

### Comparing `walt-client-7/walt/client/doc/md/node-install.md` & `walt-client-8.0/walt/client/doc/md/node-install.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# How to install and connect a new WalT node
+# WalT node installation
 
 ## Introduction
 
 The WALT server exposes the content of walt images to nodes using netboot-compatible protocols (TFTP and NFS).
 Thus, WalT nodes can boot their OS over the network.
 This means that the walt image is never transfered as a whole to the node: it remains on the server.
 
@@ -16,24 +16,29 @@
 
 The following sections will show how to set up a new node, depending on its model.
 Then, last section will explain how walt users can start to use such a new node.
 
 
 ## PC nodes
 
-Download image `pc-usb.dd.gz` at https://github.com/drakkar-lig/walt-project/releases/latest.
-Flash it to a USB flash drive (a small one is enough, the image just needs a few tens of megabytes),
-using unix tool `dd` or similar.
+Any PC can be turned into a walt node.
+
+If the PC supports PXE booting, the procedure is obvious:
+1. Connect the PC to the WALT network.
+2. Select "PXE booting" as the first boot option (by using the BIOS/firmware screen).
 
-Then, any PC can be turned into a walt node:
-* connect the PC to the WALT network
-* boot on this USB flash drive (by setting BIOS/firmware options appropriately)
+If not, download image `pc-usb.dd.gz` at https://github.com/drakkar-lig/walt-project/releases/latest.
+Flash it to a USB flash drive (a small one is enough, the image just needs a few tens of megabytes),
+using unix tool `dd` or similar. Then:
+1. Plug the USB flash drive to the PC.
+2. Connect the PC to the WALT network.
+3. Boot on the USB flash drive (by using the BIOS/firmware screen).
 
-It should be compatible with most BIOS-based and UEFI-based machines, and old 32-bits PCs, provided
-the network bootloader can handle the network card.
+The USB image should be compatible with most BIOS-based and UEFI-based machines, and old 32-bits PCs,
+provided the network bootloader can handle the network card.
 
 
 ## Virtual nodes
 
 WalT allows you to create virtual nodes. Virtual nodes are actually `kvm` virtual machines running
 on the server. When you list nodes, virtual nodes will be displayed the same as PC nodes, because
 their virtual hardware reflects the one of a standard PC.
@@ -49,90 +54,119 @@
 ```
 
 
 ## Raspberry Pi boards
 
 ### Hardware tips
 
-WalT supports raspberry pi models B, B+, 2B, 3B, 3B+, and 4B.
+WalT supports raspberry pi models B, B+, 2B, 3B, 3B+, 4B, and Pi-400.
 
-We recommend raspberry pi model 3B+ or 4B, with the official PoE HAT addon board of the raspberry pi foundation.
+We recommend raspberry pi model 3B+ or 4B.
+
+PoE support is usually provided by the official PoE HAT addon board of the raspberry pi foundation.
+
+As an alternative, we have also tested compact external PoE splitters (YuanLey brand) which are cheaper,
+more silent (no fan), and work fine.
+Take care on puchasing the right model for powering your board:
+- rpi 4B boards need a splitter model with a USB-C connector,
+- rpi 3B+ boards need a splitter model with a USB micro-B connector.
 
 You will also need at least one SD card for the first bootup (see below). You may use the same SD card to
 perform this first bootup of each node.
 
 
-### standard boot method: using a SD card
+### Standard boot method: using a SD card
 
 Download archive `rpi-sd-files.tar.gz` at https://github.com/drakkar-lig/walt-project/releases/latest.
 Extract and copy files to a USB flash drive formatted the usual way (1 single partition, FAT32 fileystem).
 A small one is enough, total size of files is just a few tens of megabytes.
 
 Then:
 * insert this SD card in its slot
 * connect the board to the WALT network (and, if PoE is not provided, power it on)
 
 The board will boot as a walt node.
 
 
-### network boot method: no SD card
+### Network boot method: no SD card
 
 Raspberry Pi 3B+ and 4B boards have a more advanced firmware that may be used to boot over the network.
 In this case, the SD card is no longer needed. However, due to incorrect firmware behavior (3B+ model),
-and to the fact walt server has to detect the board model, you should boot the board at least once using
-a SD card (see previous subsection).
+eeprom flashing requirement (4B model), and to the fact walt server has to detect the board model, you
+must boot the board at least once using a SD card (see previous subsection).
 Once done, you can remove the SD card, and next bootups should work without it.
 
-Notes:
-* The SD card is the most fragile part of a raspberry pi board, thus working without it prevents most
-  common hardware problems. Note, however, that the smart bootup mechanism used in walt allows to keep
-  the SD card readonly, which greatly improves its lifetime.
+Important notes:
+* If using a 4B board, the eeprom has to be flashed to allow network boot. This should be done
+  automatically when the board is first booted (with the SD card), thanks to appropriate boot files in
+  `rpi-sd-files.tar.gz`. However, in order to prevent this operation to repeat each time the board is
+  rebooted, the firmware renames `recovery.bin` to `RECOVERY.000`. Thus, if you want to use the same SD
+  card for the first boot of several 4B boards, after each boot rename `RECOVERY.000` back to
+  `recovery.bin` on the SD card before inserting it in another board.
 * This boot method is not as robust as the previous one: if, for any reason, communication with
   the server is temporarily broken, the board may fail to reboot and hang. (With the other boot method,
   the board would reboot as many times as required until the communication with the server is recovered.)
   If PoE is used to power the board, and PoE reboots are allowed on the switch, then walt will allow you
   to "hard-reboot" (i.e. power-cycle) the board remotely. Otherwise, one would have to manually disconnect
   and reconnect the power source of the board to unblock it.
-* On the Raspberry Pi 4B board, the network boot method of the firmware must be activated first. This is
-  done automatically by script `/bin/on-bootup` of default image. As a result, when you will boot the
-  board for the first time, with a SD card, the firmware update will be applied and the board will
-  automatically reboot. Once this second boot is done, the board can work without the SD card.
+* The SD card is the most fragile part of a raspberry pi board, thus working without it prevents most
+  common hardware problems. Note, however, that the smart bootup mechanism used in walt allows to keep
+  the SD card readonly, which greatly improves its lifetime anyway.
 
 
-## How to identify and use the new node
+## Google Coral Dev Boards
 
-When WALT server detects a node for the first time, it names it 'node-<6-hex-chars>' (for instance node-8a7b6c).
-The hex chars are taken from the right side of the node's mac address.
+First, follow the standard startup procedure at https://coral.ai/docs/dev-board/get-started.
+Then run the following on the board (with a proper internet access):
+```
+$ cd /tmp
+$ wget https://github.com/drakkar-lig/walt-project/releases/latest/download/coral-devb-boot.tar.gz
+$ cd /boot
+$ mv boot.scr boot.scr.orig
+$ tar xfz /tmp/coral-devb-boot.tar.gz
+```
+
+You can now connect the board to a WALT network and it will boot as a WALT node.
+For PoE, we recommend the compact PoE splitter with a USB-C connector (cf. hardware tips about raspberry pi boards above).
+
+
+## How to identify and use the new node
 
-If LLDP (link layer discovery protocol) is available, just wait a little (10 minutes) after you have booted
-the new node, for the LLDP table to be updated on the switch.
+When WALT server detects a node for the first time, a log line is emitted.
 
-Then run:
+Thus, you should be able to identify the new node by checking the logs as follows:
 ```
-$ walt device rescan
-$ walt device tree
+$ walt log show --platform --history -5m:
+10:45:49.188989 walt-server.platform.devices -> new node name=node-f26782 model=rpi-3-b-plus mac=b8:27:eb:f2:67:82 ip=192.168.152.14
+$
 ```
 
-The tree view should display your new node connected on the appropriate switch and port number.
-
-If LLDP is not available, use `walt node show --all` and look for those named 'node-<6-hex-chars>'.
-The node model (e.g. `rpi-b-plus`, `rpi-2-b`, etc.) is diplayed too.
-If unsure which node is which, you can use `walt node blink <node>`. Currently, on raspberry pi boards,
-this will make a tiny led blink in heartbeat mode. Or use `walt node reboot <node>` and check which
-board is temporarily powered off.
+Important notes:
+* The first time a given model of walt node is connected, the server has to download a default walt image to handle it, which takes time.
+* In this more complex case, the logs will first indicate the new node is a device of 'unknown' type, and once the image is downloaded, it will be turned into a real walt node.
+* `--platform` allows to select platform internal logs (as opposed to experiment logs generated by walt nodes).
+* `--history -5m:` allows to select logs issued up to 5 minutes ago and up to now (you may increase this number
+  if the node was connected longer ago).
 
-In any case, as soon as the node is identified, it is strongly advised to rename it. A naming scheme
+In this example the log line indicates that the new node has been named `node-f26782`.
+The hex chars are taken from the right side of the node's mac address.
+As soon as the node is identified, it is strongly advised to rename it. A naming scheme
 such as `<type>-<location>-<id>` is handy. For instance, considering the node is in room 412:
 ```
-$ walt device rename node-8a7b6c rpi3b-412-A
+$ walt device rename node-f26782 rpi3bp-412-A
 ```
 
+The new node first boots a default image, thus it belongs to nobody.
+It will be listed as a "free" node when you use `walt node show --all`.
+To make this node yours, run `walt node acquire <node>` or let it boot one of your images by using `walt node boot <node> <image>`
+(see [`walt help show node-ownership`](node-ownership.md)).
+
 Troubleshooting notes:
-* If ever the node failed to boot over the network (this probably means the network is misconfigured),
-  the server might still detect it but it may not know that this device is a node. Thus, the server
-  will name it 'unknown-<6-hex-chars>' instead of 'node-<6-hex-chars>'. And the node will not appear
-  when typing `walt node show --all`. You can use `walt device show` instead.
-  The first time the node boots correctly, it will be automatically renamed to 'node-<6-hex-chars>',
-  and appear in the output of `walt node show --all`.
+* If ever the node failed to boot over the network (this probably means the network or the node
+  bootloader is misconfigured), the server might still detect it but it may not know that this device
+  is a node. In this case `walt log show` will still print a line but mention a `"new device"`
+  instead of a `"new node"`. This node will obviously not appear when typing `walt node show --all`, but
+  it will be listed when you use `walt device show`.
+  The first time the node boots correctly, its type will be automatically updated and it will appear
+  in the output of `walt node show --all`.
 * In case of trouble, you can monitor walt service logs on the server, while connecting the new node,
-  by typing `journalctl -f -u walt-server`. Or use a network sniffer (such as wireshark).
-
+  by typing `journalctl -b -afu walt-server`. Or use a network sniffer (such as wireshark).
```

### Comparing `walt-client-7/walt/client/doc/md/shells.md` & `walt-client-8.0/walt/client/doc/md/shells.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 `walt node shell` just wraps a ssh session to the node.
 
 Be warned that a WalT node is a very **volatile** environment. Each time a node reboots, it loses all modifications made on files (created, suppressed, modified), and restarts from the original files of the image it boots.
 This ensures that a node booting a given image will always act the same.
 (See [`walt help show node-bootup`](node-bootup.md) for a more technical explanation on this aspect.)
 
+However, for convenience, a directory `/persist` is available on each node. Data stored there do remain available accross reboots.
+You can use it to store large experiment results files for instance. `/persist` is a read-write NFS-mount: data is actually stored on the server.
+
 ## `walt image shell`: modification of operating system
 
 If you want to modify files in a permanent way, you must modify the image the node boots. `walt image shell` is the most common way to do this. It provides a shell running in a virtual environment (docker container) where you can make the changes, such as installing packages for example.
 
 Since the image is expected to be booted by a node, and the CPU architecture of the node may be different from the one of the server (e.g. ARM-based raspberry pi versus amd64-based server), the binaries found inside an image may not be compatible with the server CPU. In this case, any binary you run in this shell will involve **CPU emulation**, which leads to a slower behavior. Avoid heavy processing, such as compiling of a large source code base. In this case, cross-compiling on another machine and importing the build artefacts in the virtual environment (through the emulated network) should be the prefered option.
 Also, keep in mind that in the virtual environment (docker container) no services are running (no init process, etc). Actually, the only process running in this virtual environment when you enter it is the shell process itself.
```

### Comparing `walt-client-7/walt/client/doc/md/switch-install.md` & `walt-client-8.0/walt/client/doc/md/switch-install.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-# How to install a switch on WalT platform network
+# Switch installation in WalT network
 
 ## Scope
 
 For a general view of networking topic, see [`walt help show networking`](networking.md) first.
 
 This documentation page explains how to plug and configure a switch connected to the dedicated WalT platform
 network (sometimes called `walt-net`).
@@ -14,21 +14,24 @@
 this case you should contact your network admins.
 
 
 ## Recommended switch features
 
 The following WalT features are optional:
 * Node "hard-reboots" (being able to remotely stop powering a given node to force a reboot in case of problem)
+* Automatic power savings (by powering off unused nodes)
 * Network topology exploration
 
 In order to enable those features, the switches you connect to `walt-net` must provide the following features:
 * PoE (Power-Over-Ethernet) ports
 * LLDP support (Link Layer Discovery Protocol)
 * SNMP remote administration, with support for standard MIBs (POWER-OVER-ETHERNET.mib, IF.mib and LLDP.mib)
 
+See [`walt help show optional-features`](optional-features.md) for more info.
+
 
 ## Hardware recommendation
 
 We recommend the switch netgear gs110tp. It is a cost-effective switch, with useful features in the context of
 a WalT platform:
 * 8 PoE ports
 * LLDP support (Link Layer Discovery Protocol)
@@ -39,44 +42,72 @@
 
 Alternatively, WalT also works with switch TP-Link T1500G-10PS. You just have to configure it to request
 its management IP through DHCP. Other default settings are OK.
 
 Note: if you test another switch model, we would be happy to get the results of your test.
 
 
-## Configuring the switch in WalT
+## How to identify the new switch in WALT
+
+When WALT server detects a switch for the first time, a log line is emitted.
+Thus, you should be able to identify the new switch by checking the logs as follows:
+
+```
+$ walt log show --platform --history -5m: "new"
+10:50:15.498660 walt-server.platform.devices -> new switch name=switch-18d55d mac=6c:b0:ce:18:d5:5d ip=192.168.152.11
+$
+```
+
+If WALT is unable to detect this device is a switch, the log line will look like this instead:
+```
+10:50:15.498660 walt-server.platform.devices -> new device name=unknown-18d55d type=unknown mac=6c:b0:ce:18:d5:5d ip=192.168.152.11
+```
+In this example we see that WALT registered this unknown device with name `unknown-18d55d`.
+The hex chars are taken from the right side of the switch mac address.
+
+In such a case, run the following to let WALT know this new device is actually a switch:
+```
+$ walt device config unknown-18d55d type=switch
+Renaming unknown-18d55d to switch-18d55d for clarity.
+Done.
+$
+```
+
+In any case, when your switch is identified you can give it a more convenient name, for instance:
+```
+$ walt device rename switch-18d55d switch-netgear-426
+```
+
+
+## Enabling LLDP and/or PoE
+
+In some complex environments, remote administration of a given switch by WalT may not be allowed;
+or LLDP/PoE may not be available. Thus, these features are disabled by default. As a result, WALT
+must be explicitely allowed to use these features on a given switch, by using `walt device config`
+(see next section).
 
-By default, WalT may not detect that the equipment is a switch. Moreover, in some complex environments,
-remote administration of a given switch by WalT may not be allowed. Thus, in order to let WalT use these
-features, you must:
-
-* Run `walt device show` and look for any new device that was detected by WALT server. The first field of the
-  line will report the default name WALT gave to your switch. It should be `switch-<hhhhhh>` if WALT
-  could detect it is a switch, or `unknown-<hhhhhh>` otherwise.
-* Run `walt device rename "<type>-<hhhhhh>" "<your-switch-name>"` for convenience.
-* If the device type is `unknown`, run `walt device config <your-switch-name> type=switch`.
-* If your switch supports LLDP and/or PoE use `walt device config <your-switch-name> <settings>` to configure it. See next section.
-* If LLDP is enabled, run `walt device rescan` and `walt device tree`. Your switch should appear in the topology tree.
+When LLDP is enabled, after a little time (e.g. 10 minutes) you can run `walt device rescan` and
+`walt device tree`; your switch should appear in the network topology tree.
 
 Notes:
 - LLDP only works between two devices (two switches, or a switch and a node) when both devices have LLDP enabled.
   On a node, this means the running walt image must embed a LLDP daemon.
-- LLDP detection may need a few minutes.
 - In any case, keep in mind that topology exploration and PoE reboots are optional features. It should not prevent
   you from working with nodes.
 
 
 ## Switch configuration settings
 
-If you want to enable LLDP or PoE reboots, WalT server will have to communicate with the switch by using SNMP.
+If you want to enable LLDP or PoE reboots and power savings, WalT server will have to communicate with the switch by using SNMP.
 Thus you should specify SNMP configuration parameters `snmp.version` (with value `1` or `2`) and `snmp.community`.
 Then, you can enable LLDP by specifying `lldp.explore=true`.
 And finally you can enable node hard-reboots using PoE by specifying `poe.reboots=true`.
+This setting also activates automatic power savings.
 Note that you cannot enable `poe.reboots` without enabling `lldp.explore` (since WalT needs to know on which PoE
-switch port a node is connected in order to hard-reboot it).
+switch port a node is connected in order to hard-reboot it or power it off).
 
 For instance, on the netgear gs110tp in its default configuration, one may run:
 ```
 $ walt device config <switch-name> snmp.version=2 snmp.community='private' lldp.explore=true poe.reboots=true
 ```
 
 For general information about this command, see [`walt help show device-config`](device-config.md).
```

### Comparing `walt-client-7/walt/client/doc/md/tutorial.md` & `walt-client-8.0/walt/client/doc/md/tutorial.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,30 @@
-# Getting Started
+# User Tutorial
 
 ## Prerequisites
 
-You can use the walt client application on any Mac OS X or GNU/Linux machine.
-Since WalT interacts with the docker hub, you need an account there.
-If you do not have one already, please register at: https://hub.docker.com/
+If you want to interact with the docker hub to clone or publish OS images,
+you will need an account there. If you do not have one already, you can register
+at: https://hub.docker.com/.
 
-## Install walt-client
+## (Optional) Install walt-client
 
-The Walt client is written in python and hosted on [PyPi](https://pypi.python.org/pypi), so it can be installed using pip:
+Most users use ssh to connect to the WalT server and use the walt client already
+installed there.
 
-```console
-$ sudo pip install walt-client
-```
-
-Don’t forget to frequently check for updates:
+If you want to install the WalT client on your own machine (Mac OS X or GNU/Linux)
+instead, you can type:
 
 ```console
-$ sudo pip install walt-client --upgrade
+$ sudo pip install walt-client
 ```
 
 ## The `walt` command
 
-`walt` is the client entry point of the walt platform management.
-
-On the very first launch, this command will prompt for a small set of parameters:
-* IP or hostname of the WalT server
-* your docker hub credentials
+`walt` is the entry point of the walt platform management.
 
 You can get an overview of walt subcommands categories by just typing:
 ```console
 $ walt
 No sub-command given
 ------
 
@@ -100,14 +94,17 @@
        ├─5: (rpi-kfet-3)
        └─7: switch-3
              ├─1: rpi-D318-1
 [...]
 $
 ```
 
+This tree view requires proper LLDP configuration, see [`walt help show switch-install`](switch-install.md).
+However, LLDP is an optional feature and the other WalT commands can work without it.
+
 Table form:
 
 ```console
 $ walt device show
 
 The WalT network contains the following devices:
 
@@ -144,15 +141,15 @@
 
 name           type  image            ip             reachable
 -------------  ----  ---------------  -------------  ---------
 rpi-D314-1     rpi   rpi-jessie       192.168.12.16  yes
 rpi-D314-jtag  rpi   rpi-jtag-target  192.168.12.2   yes
 [...]
 
-The following nodes are free (they have never been used):
+The following nodes are free (they boot a default image):
 
 name           type  ip              reachable
 -------------  ----  --------------  ---------
 rpi-D106-5     rpi   192.168.12.111  NO
 rpi-D301B-4    rpi   192.168.12.164  yes
 
 The following nodes are likely to be used by other users, since you do
@@ -164,22 +161,22 @@
 rpi-D31-2  rpi   zyta         server:zyta/rpi-fix   192.168.12.18  NO
 [...]
 $
 ```
 
 Three categories of nodes are listed:
 
-1. the nodes that you **own**: in WalT terminology, if node <N> boots an image created by user <U>, we consider that “<U> owns <N>”. Thus, if you just started using WalT, this category is empty for now.
-2. the nodes that are **free**: no user ever booted an image on these nodes. The server associated a default image to them.
+1. the nodes that you **own**: in WalT terminology, if node `<N>` boots an image created by user `<U>`, we consider that “`<U>` owns `<N>`”. Thus, if you just started using WalT, this category is empty for now.
+2. the nodes that are **free**: they boot a default image (users currently do not use them).
 3. the nodes that are **owned by someone else**: the image they are running belongs to another user. If you want to use them, make sure this user is ok. This category is not shown unless you specify the `--all` option.
 
 For more information on this topic, you can type:
 
 ```console
-$ walt help show node-terminology
+$ walt help show node-ownership
 ```
 
 ## The images
 
 In the previous section we’ve seen that a Raspberry Pi was running an image named `rpi-jessie`. Let’s have a little explanation.
 An image is the operating system a device is running. For example `rpi-jessie` is a lightweight Debian Jessie built for Raspberry Pi.
 
@@ -195,16 +192,16 @@
 rpi-jessie       True     2016-02-29 10:35:02  True
 rpi-openocd      False    2016-03-23 18:06:03  True
 $
 ```
 
 You can see the names of the different images, if they are currently used, their creation date, and whether they are ready (when downloading an image, you will see Ready = False until the download completes).
 
-If you just started using WalT, this list of images is empty.
-You will have to `clone` existing images in order to make them “yours”.
+If you just started using WalT, this list of images is initialized with a set of default images.
+You may `clone` other images in order to make them “yours”.
 
 You can `search` for images available for cloning as follows:
 
 ```console
 $ walt image search jessie
 User          Image name       Location           Clonable link
 ------------  ---------------  -----------        ----------------------------
@@ -218,16 +215,17 @@
 
 WalT images are internally packaged as [Docker](https://www.docker.com/whatisdocker) images.
 Listed images may be stored in one of the following locations:
 
 * docker hub (clonable link prefix 'hub:')
 * local server, managed by docker daemon (clonable link prefix 'docker:')
 * already in walt internal storage (clonable link prefix 'walt:')
+* possibly other custom registries configured on the WalT server.
 
-In the last case, only images of other users are listed, since the images you already own do not need to be cloned.
+In the third case, only images of other users are listed, since the images you already own do not need to be cloned.
 
 Let’s choose one and clone it:
 
 ```console
 $ walt image clone walt:brunisholz/rpi-jessie
 [...]
 $
@@ -248,28 +246,28 @@
 ```console
 $ walt image shell rpi-jessie
 ```
 
 You should now be logged into the image as indicated by the prompt:
 
 ```console
-root@image-shell:/#
+root@image-shell:~#
 ```
 
 Now install `avahi-daemon` in order to allow discovery through the devices and `netcat` to set up a lightweight client/server architecture.
 
 ```console
-root@image-shell:/# apt-get install avahi-daemon netcat
+root@image-shell:~# apt-get install avahi-daemon netcat
 ```
 
 Now go to the root directory, create and edit a file named pong.sh. It will be our master server:
 
 ```console
-root@image-shell:/# cd root/
-root@image-shell:/# vim pong.sh
+root@image-shell:~# cd root/
+root@image-shell:~# vim pong.sh
 ```
 
 And copy the following script:
 
 ```bash
 #!/bin/bash
 
@@ -392,21 +390,19 @@
 > For example a Raspberry Pi located in the D317 office could be named:* \
 > `rpi-D317-tutorial`
 
 Then we boot nodes:
 
 ```console
 $ walt node boot rpi-sw3-3-pong rpi-entertainment
-rpi-sw3-3-pong was powered off.
-rpi-sw3-3-pong will now boot rpi-entertainment.
-rpi-sw3-3-pong was powered on.
+Node rpi-sw3-3-pong will now boot rpi-entertainment.
+Node rpi-sw3-3-pong: rebooted ok.
 $ walt node boot rpi-sw3-2-ping rpi-entertainment
-rpi-sw3-2-ping was powered off.
-rpi-sw3-2-ping will now boot rpi-entertainment.
-rpi-sw3-2-ping was powered on.
+Node rpi-sw3-2-ping will now boot rpi-entertainment.
+Node rpi-sw3-2-ping: rebooted ok.
 ```
 
 Nodes are now booting the OS contained in our image.
 You could wait until they are fully booted by typing:
 ```console
 $ walt node wait rpi-sw3-2-ping,rpi-sw3-3-pong
 ```
@@ -414,25 +410,25 @@
 
 ## Connecting to devices and monitoring experimentations
 
 Now that our image is running on two nodes, we can connect to them and start the ping pong game.
 
 ```console
 $ walt node shell rpi-sw3-3-pong
-Caution: changes will be lost on next node reboot.
+Caution: changes outside /persist will be lost on next node reboot.
 Run 'walt help show shells' for more info.
 
 root@rpi-sw3-3-pong:~# ./pong.sh
 ```
 
 On another terminal connect to the other Raspberry Pi and start the client side.
 
 ```console
 $ walt node shell rpi-sw3-2-ping
-Caution: changes will be lost on next node reboot.
+Caution: changes outside /persist will be lost on next node reboot.
 Run 'walt help show shells' for more info.
 
 root@rpi-sw3-2-ping:~# ./ping.sh
 ```
 
 They should start playing ping pong together!
```

### Comparing `walt-client-7/walt/client/doc/md/vpn.md` & `walt-client-8.0/walt/client/doc/md/vpn.md`

 * *Files identical despite different names*

### Comparing `walt-client-7/walt/client/doc/mdtable.py` & `walt-client-8.0/walt/client/doc/mdtable.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,103 @@
 import re
 
 RE_HEADER_SEP_LINE = re.compile("-+:? *[|] *:?-+")
 ALIGN_LEFT = -1
 ALIGN_CENTER = 0
 ALIGN_RIGHT = 1
 
+
 def detect_table(buf):
     return RE_HEADER_SEP_LINE.search(buf) is not None
 
+
 def analyse_table(buf):
     lines = buf.splitlines()
     for idx, line in enumerate(lines):
         if RE_HEADER_SEP_LINE.search(line):
             header_idx = idx
             header_sep_line = line
             break
     alignments = []
-    for sep in header_sep_line.strip().strip('|').split('|'):
+    for sep in header_sep_line.strip().strip("|").split("|"):
         sep = sep.strip()
-        aligndef = (sep.startswith(':'), sep.endswith(':'))
-        alignments.append({
-            (False, False): ALIGN_LEFT,
-            (True, False): ALIGN_LEFT,
-            (True, True): ALIGN_CENTER,
-            (False, True): ALIGN_RIGHT
-        }[aligndef])
+        aligndef = (sep.startswith(":"), sep.endswith(":"))
+        alignments.append(
+            {
+                (False, False): ALIGN_LEFT,
+                (True, False): ALIGN_LEFT,
+                (True, True): ALIGN_CENTER,
+                (False, True): ALIGN_RIGHT,
+            }[aligndef]
+        )
     num_cols = len(alignments)
     table_content = []
     for idx, line in enumerate(lines):
         if idx == header_idx:
             continue
-        if line.strip() == '':
+        if line.strip() == "":
             continue
-        row = [ cell.strip() for cell in line.strip().strip('|').split('|') ]
+        row = [cell.strip() for cell in line.strip().strip("|").split("|")]
         row = row[:num_cols]
-        row += [''] * (num_cols - len(row))
+        row += [""] * (num_cols - len(row))
         table_content.append(row)
     return table_content, alignments
 
+
 def align(text, real_text_len, field_len, alignment):
     if alignment == ALIGN_LEFT:
-        return text + ' ' * (field_len - real_text_len)
+        return text + " " * (field_len - real_text_len)
     elif alignment == ALIGN_RIGHT:
-        return ' ' * (field_len - real_text_len) + text
-    else:   # center
-        left_len = (field_len - real_text_len)//2
+        return " " * (field_len - real_text_len) + text
+    else:  # center
+        left_len = (field_len - real_text_len) // 2
         right_len = field_len - real_text_len - left_len
-        return ' ' * left_len + text + ' ' * right_len
+        return " " * left_len + text + " " * right_len
+
 
 def horizontal_line(col_widths, left_char, sep_char, right_char):
-    return left_char + sep_char.join('\u2500' * (w+2) for w in col_widths) + right_char + '\n'
+    return (
+        left_char
+        + sep_char.join("\u2500" * (w + 2) for w in col_widths)
+        + right_char
+        + "\n"
+    )
+
 
 def render_table(md_renderer, buf):
     table_content, alignments = analyse_table(buf)
-    col_widths = [ max(md_renderer.real_text_len(cell) for cell in col) \
-            for col in zip(*table_content) ]
+    col_widths = [
+        max(md_renderer.real_text_len(cell) for cell in col)
+        for col in zip(*table_content)
+    ]
     # print top line
-    md_renderer.lit(horizontal_line(col_widths, '\u250c', '\u252c', '\u2510'))
+    md_renderer.lit(horizontal_line(col_widths, "\u250c", "\u252c", "\u2510"))
     # print header
     for col_idx, word in enumerate(table_content[0]):
-        md_renderer.lit('\u2502 ')
-        md_renderer.stack_context(bold = True)
-        md_renderer.lit(align(word, md_renderer.real_text_len(word), col_widths[col_idx], ALIGN_CENTER))
+        md_renderer.lit("\u2502 ")
+        md_renderer.stack_context(bold=True)
+        md_renderer.lit(
+            align(
+                word, md_renderer.real_text_len(word), col_widths[col_idx], ALIGN_CENTER
+            )
+        )
         md_renderer.pop_context()
-        md_renderer.lit(' ')
-    md_renderer.lit('\u2502\n')
+        md_renderer.lit(" ")
+    md_renderer.lit("\u2502\n")
     # print value rows
-    separation_line = horizontal_line(col_widths, '\u251c', '\u253c', '\u2524')
+    separation_line = horizontal_line(col_widths, "\u251c", "\u253c", "\u2524")
     for row_idx, row in enumerate(table_content[1:]):
         md_renderer.lit(separation_line)
         for col_idx, word in enumerate(row):
-            md_renderer.lit('\u2502 ')
-            md_renderer.lit(align(word, md_renderer.real_text_len(word), col_widths[col_idx], alignments[col_idx]))
-            md_renderer.lit(' ')
-        md_renderer.lit('\u2502\n')
+            md_renderer.lit("\u2502 ")
+            md_renderer.lit(
+                align(
+                    word,
+                    md_renderer.real_text_len(word),
+                    col_widths[col_idx],
+                    alignments[col_idx],
+                )
+            )
+            md_renderer.lit(" ")
+        md_renderer.lit("\u2502\n")
     # print bottom line
-    md_renderer.lit(horizontal_line(col_widths, '\u2514', '\u2534', '\u2518'))
+    md_renderer.lit(horizontal_line(col_widths, "\u2514", "\u2534", "\u2518"))
```

### Comparing `walt-client-7/walt/client/expose.py` & `walt-client-8.0/walt/client/expose.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,66 @@
 #!/usr/bin/env python
-from walt.client.config import conf
 from select import select
-from walt.common.constants import WALT_SERVER_TCP_PORT
+
+from walt.client.link import connect_to_tcp_server
 from walt.common.io import read_and_copy
-from walt.common.tcp import Requests, write_pickle, client_sock_file, \
-                            server_socket, SmartSocketFile
+from walt.common.tcp import Requests, RWSocketFile, server_socket, write_pickle
+
 
 class TCPExposer:
     def __init__(self, local_port, node_ip, node_port):
         self.local_port = local_port
-        self.params = dict(
-            node_ip = node_ip,
-            node_port = node_port
-        )
+        self.params = dict(node_ip=node_ip, node_port=node_port)
         self.associations = {}
+
     def run(self):
         self.local_server_s = server_socket(self.local_port)
         while True:
-            read_socks = list(self.associations.keys()) + [ self.local_server_s ]
-            select_args = [ read_socks, [], read_socks ]
+            read_socks = list(self.associations.keys()) + [self.local_server_s]
+            select_args = [read_socks, [], read_socks]
             rlist, wlist, elist = select(*select_args)
             if len(elist) > 0 or len(rlist) == 0:
                 break
             sock_r = rlist[0]
             if sock_r == self.local_server_s:
-                if self.event_on_server_s() == False:
+                if self.event_on_server_s() is False:
                     break
             else:
                 paired_sock = self.associations[sock_r]
-                if read_and_copy(sock_r, paired_sock) == False:
+                if read_and_copy(sock_r, paired_sock) is False:
                     for s in (sock_r, paired_sock):
                         s.close()
                     del self.associations[sock_r]
                     del self.associations[paired_sock]
+
     def open_channel_to_node(self):
         # connect
-        server_host = conf['server']
-        sock_file = client_sock_file(server_host, WALT_SERVER_TCP_PORT)
+        sock_file = connect_to_tcp_server()
         # write request id
         Requests.send_id(sock_file, Requests.REQ_TCP_TO_NODE)
         # send parameters
         write_pickle(self.params, sock_file)
         # wait for the status message from the server
         status = sock_file.readline().strip()
-        if status == b'OK':
-            print('New connection forwarded to node.')
+        if status == b"OK":
+            print("New connection forwarded to node.")
             return sock_file
         else:
             sock_file.close()
-            print(status)
+            print(status.decode("utf-8"))
             return None
+
     def event_on_server_s(self):
         conn_s, addr = self.local_server_s.accept()
         node_channel = self.open_channel_to_node()
-        if node_channel == None:
+        if node_channel is None:
             conn_s.close()
             return
-        client_channel = SmartSocketFile(conn_s)
+        client_channel = RWSocketFile(conn_s)
         self.associations[client_channel] = node_channel
         self.associations[node_channel] = client_channel
+
     def close(self):
         for f1, f2 in self.associations.items():
             f1.close()
             f2.close()
         self.local_server_s.close()
```

### Comparing `walt-client-7/walt/client/image.py` & `walt-client-8.0/walt/client/apiobject/images.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,159 +1,242 @@
-#!/usr/bin/env python
-import os, sys
-from plumbum import cli
-from walt.client.link import ClientToServerLink
-from walt.client.tools import confirm
-from walt.client.interactive import run_image_shell_prompt
-from walt.client.transfer import run_transfer_with_image
-from walt.client.auth import get_auth_conf
-from walt.client.application import WalTCategoryApplication, WalTApplication
+import re
+import sys
+from collections import defaultdict
+from pathlib import Path
+
+from walt.client.apiobject.base import (
+    APIItemClassFactory,
+    APIItemInfoCache,
+    APIObjectBase,
+    APISetOfItemsClassFactory,
+)
+from walt.client.apitools import silent_server_link
+from walt.client.config import conf
+from walt.client.exceptions import NoSuchImageNameException
+from walt.client.transfer import run_transfer_for_image_build
+from walt.common.tools import parse_image_fullname
+
+
+class APIImageInfoCache(APIItemInfoCache):
+    def __init__(self):
+        super().__init__(show_aliases=True)
+
+    def do_refresh(self, server):
+        fields = ("id", "name", "fullname", "in_use", "created", "compatibility:tuple")
+        tabular_data = server.get_images_tabular_data(
+            conf.walt.username, refresh=False, fields=fields
+        )
+        # remove ':<suffix>' on field names
+        fields = list(re.sub(r"([^:]*):.*", r"\1", f) for f in fields)
+        # replace rows with dicts
+        image_infos = list(
+            {f: val for f, val in zip(fields, row)} for row in tabular_data
+        )
+        # populate attributes
+        self.info_per_id = {}
+        self.id_per_name = {}
+        self.names_per_id = defaultdict(set)
+        for info in image_infos:
+            name = info.pop("name")
+            image_id = info["id"]
+            self.id_per_name[name] = image_id
+            self.info_per_id[image_id] = info
+            self.names_per_id[image_id].add(name)
+
+    def do_remove_item(self, server, item_name):
+        return server.remove_image(item_name)
+
+    def do_rename_item(self, server, item_name, new_item_name):
+        return server.rename_image(item_name, new_item_name)
+
+
+__info_cache__ = APIImageInfoCache()
+
+
+class APIImageBase:
+    """Base class of all APIImage classes, for use in isinstance()"""
 
-class WalTImage(WalTCategoryApplication):
-    """management of WalT-nodes operating system images"""
     pass
 
-@WalTImage.subcommand("search")
-class WalTImageSearch(WalTApplication):
-    """search for remote WalT node OS images"""
-    def main(self, keyword=None):
-        with ClientToServerLink() as server_link:
-            server_link.set_busy_label('Searching')
-            tty_mode = os.isatty(sys.stdout.fileno())
-            server_link.search_images(keyword, tty_mode)
-
-@WalTImage.subcommand("clone")
-class WalTImageClone(WalTApplication):
-    """clone a remote image into your working set"""
-    _force = False # default
-    def main(self, clonable_image_link, image_name=None):
-        with ClientToServerLink() as server_link:
-            server_link.set_busy_label('Validating / Cloning')
-            server_link.clone_image(clonable_image_link,
-                                    force=self._force, image_name=image_name)
-    @cli.autoswitch(help='do it, even if it overwrites an existing image.')
-    def force(self):
-        self._force = True
-
-@WalTImage.subcommand("publish")
-class WalTImagePublish(WalTApplication):
-    """publish a WalT image on the docker hub"""
-    def main(self, image_name):
-        with ClientToServerLink() as server_link:
-            server_link.set_busy_label('Validating / Publishing')
-            auth_conf = get_auth_conf(server_link)
-            server_link.publish_image(auth_conf, image_name)
-
-@WalTImage.subcommand("show")
-class WalTImageShow(WalTApplication):
-    """display your working set of walt images"""
-    _refresh = False # default
-    def main(self):
-        with ClientToServerLink() as server:
-            print(server.show_images(self._refresh))
-    @cli.autoswitch(help='resync image list from Docker daemon.')
-    def refresh(self):
-        self._refresh = True
-
-@WalTImage.subcommand("shell")
-class WalTImageShell(WalTApplication):
-    """modify an image through an interactive shell"""
-    def main(self, image_name):
-        with ClientToServerLink() as server:
-            session_info = server.create_image_shell_session(
-                            image_name, 'shell session')
-            if session_info == None:
-                return  # issue already reported
-            session_id, image_fullname, container_name, default_new_name = \
-                            session_info
-            run_image_shell_prompt(image_fullname, container_name)
-            try:
-                while True:
-                    new_name = input(\
-                        'New image name [%s]: ' % default_new_name)
-                    if new_name == '':
-                        new_name = default_new_name
-                        print('Selected: %s' % new_name)
-                    res = server.image_shell_session_save(
-                                    session_id, new_name, name_confirmed = False)
-                    if res == 'NAME_NOT_OK':
-                        continue
-                    if res == 'NAME_NEEDS_CONFIRM':
-                        if confirm(komsg = None):
-                            server.image_shell_session_save(
-                                    session_id, new_name, name_confirmed = True)
-                        else:
-                            continue
-                    break
-            except (KeyboardInterrupt, EOFError):
-                print('Aborted.')
-            # leaving the API session scoped by the with construct
-            # will cause the server to cleanup session data on server side.
-
-@WalTImage.subcommand("remove")
-class WalTImageRemove(WalTApplication):
-    """remove an image from your working set"""
-    def main(self, image_name):
-        with ClientToServerLink() as server:
-            server.remove_image(image_name)
-
-@WalTImage.subcommand("rename")
-class WalTImageRename(WalTApplication):
-    """rename an image of your working set"""
-    def main(self, image_name, new_image_name):
-        with ClientToServerLink() as server:
-            server.rename_image(image_name, new_image_name)
-
-@WalTImage.subcommand("duplicate")
-class WalTImageDuplicate(WalTApplication):
-    """duplicate an image of your working set"""
-    def main(self, image_name, new_image_name):
-        with ClientToServerLink() as server:
-            server.duplicate_image(image_name, new_image_name)
-
-@WalTImage.subcommand("cp")
-class WalTImageCp(WalTApplication):
-    """transfer files (client machine <-> image)"""
-    USAGE="""\
-    walt image cp <local-path> <image>:<path>
-    walt image cp <image>:<path> <local-path>
-    """
-    def main(self, src, dst):
-        with ClientToServerLink() as server:
-            info = server.validate_image_cp(src, dst)
-            if info == None:
-                return
-            if info['status'] == 'NEEDS_CONFIRM':
-                if confirm():
-                    info['status'] = 'OK'
-                else:
-                    return  # give up
-            if info['status'] == 'FAILED':
+
+class APISetOfImagesBase:
+    """Base class of all APISetOfImages classes, for use in isinstance()"""
+
+    pass
+
+
+class APIImageFactory:
+    __images_per_name__ = {}
+
+    @staticmethod
+    def create(in_image_name):
+        api_image = APIImageFactory.__images_per_name__.get(in_image_name)
+        if api_image is not None:
+            return api_image
+        item_cls = APIItemClassFactory.create(
+            __info_cache__, in_image_name, "image", APIImageBase, APISetOfImagesFactory
+        )
+
+        class APIImage(item_cls, APIImageBase):
+            def remove(self):
+                name = self.name
+                self.__remove_from_cache__()
+                if name in __info_cache__:
+                    return  # __remove_from_cache__ failed
+                del APIImageFactory.__images_per_name__[name]
+
+            def rename(self, new_name):
+                name = self.name
+                self.__rename_in_cache__(new_name)
+                if name in __info_cache__:
+                    return  # __rename_in_cache__ failed
+                APIImageFactory.__images_per_name__[new_name] = (
+                    APIImageFactory.__images_per_name__.pop(name)
+                )
+
+        api_image = APIImage()
+        APIImageFactory.__images_per_name__[in_image_name] = api_image
+        __info_cache__.register_obj(api_image)
+        return api_image
+
+
+class APISetOfImagesFactory:
+    @classmethod
+    def create(item_set_factory, in_names):
+        item_set_cls = APISetOfItemsClassFactory.create(
+            __info_cache__,
+            in_names,
+            "image",
+            APIImageBase,
+            APIImageFactory,
+            APISetOfImagesBase,
+            item_set_factory,
+        )
+
+        class APISetOfImages(item_set_cls, APISetOfImagesBase):
+            """Set of WalT images"""
+
+            pass
+
+        return APISetOfImages()
+
+
+class APIImagesSubModule(APIObjectBase):
+    """API submodule for WALT images"""
+
+    def get_images(self):
+        """Return images of your working set"""
+        return get_images()
+
+    def build(self, image_name, dir_or_url):
+        """Build an image using a Dockerfile"""
+        mode = "dir" if Path(dir_or_url).exists() else "url"
+        info = dict(mode=mode, image_name=image_name)
+        if mode == "dir":
+            if not Path(dir_or_url).is_dir():
+                sys.stderr.write(
+                    "Failed: parameter dir_or_url must be a directory or a git"
+                    " repository URL.\n"
+                )
                 return
-            session_info = server.create_image_shell_session(
-                            info['image_name'], 'file transfer')
-            if session_info == None:
+            info["src_dir"] = str(dir_or_url)
+        else:
+            info["url"] = dir_or_url
+        with silent_server_link() as server:
+            info = server.create_image_build_session(**info)
+            if info is None:
                 return  # issue already reported
-            session_id, image_fullname, container_name, default_new_name = \
-                            session_info
-            info.update(image_fullname = image_fullname,
-                        container_name = container_name)
-            try:
-                run_transfer_with_image(**info)
-                if info['client_operand_index'] == 0:
-                    # client was sending -> image has been modified
-                    # save the image under the same name
-                    server.image_shell_session_save(
-                            session_id, default_new_name, True)
-            except (KeyboardInterrupt, EOFError):
-                print()
-                print('Aborted.')
-
-@WalTImage.subcommand("squash")
-class WalTImageSquash(WalTApplication):
-    """squash all layers of an image into one"""
-    def main(self, image_name):
-        with ClientToServerLink() as server:
-            status = server.squash_image(image_name, False)
-            if status == 'NEEDS_CONFIRM':
-                if confirm():
-                    server.squash_image(image_name, True)
+            image_overwrite = info.pop("image_overwrite")
+            if image_overwrite:
+                sys.stderr.write("Failed: An image with this name already exists.\n")
+                return
+            session_id = info.pop("session_id")
+            if mode == "dir":
+                try:
+                    if not run_transfer_for_image_build(**info):
+                        return
+                except (KeyboardInterrupt, EOFError):
+                    print()
+                    print("Aborted.")
+                    return
+            else:
+                if not server.run_image_build_from_url(session_id):
+                    # failed
+                    return
+            server.finalize_image_build_session(session_id)
+        __info_cache__.refresh()  # detect the new image
+        return APIImageFactory.create(image_name)
+
+    def clone(self, clonable_image_link, force=False, image_name=None):
+        """Clone a remote image into your working set"""
+        with silent_server_link() as server:
+            res = server.clone_image(
+                clonable_image_link, force=force, image_name=image_name
+            )
+            if res["status"] == "OK":
+                __info_cache__.refresh()  # detect the new image
+                image_name = res["image_name"]
+                print("The image was cloned successfully.")
+                return APIImageFactory.create(image_name)
+            else:
+                return  # issue
+
+
+class APIClonableImage(APIObjectBase):
+    def clone(self, force=False, image_name=None):
+        """Clone this image into your working set"""
+        images_submodule = get_api_images_submodule()
+        return images_submodule.clone(
+            self.clonable_link, force=force, image_name=image_name
+        )
+
+
+class APIDefaultImage(APIClonableImage):
+    def __init__(self, model):
+        super().__init__()
+        self.model = model
+        self.owner = "waltplatform"
+        self.fullname = f"waltplatform/{model}-default:latest"
+        self.clonable_link = f"walt:{self.fullname}"
+        self.__doc__ = f"default for {self.model} nodes"
+
+
+class APIOtherUserImage(APIClonableImage):
+    def __init__(self, fullname):
+        super().__init__()
+        self.fullname, self.owner, self.name = parse_image_fullname(fullname)
+        self.clonable_link = f"walt:{self.fullname}"
+        self.__doc__ = f'''{self.owner}'s "{self.name}"'''
+
+
+def get_image_object_from_fullname(image_fullname):
+    image_fullname, image_user, image_name = parse_image_fullname(image_fullname)
+    if image_user == "waltplatform" and image_name.endswith("-default"):
+        model = image_fullname[len("waltplatform/") : -len("-default:latest")]
+        return APIDefaultImage(model)
+    elif image_user != conf.walt.username:
+        return APIOtherUserImage(image_fullname)
+    else:
+        return APIImageFactory.create(image_name)
+
+
+def get_image_from_name(image_name):
+    """Return the image having given name"""
+    api_images = get_images()
+    image = api_images.get(image_name, None)
+    if image is None:
+        raise NoSuchImageNameException()
+    return image
+
+
+def get_images():
+    """Return images of your working set"""
+    names = set(__info_cache__.names())
+    return APISetOfImagesFactory.create(names)
+
+
+def update_image_cache():
+    __info_cache__.refresh()
+
+
+def get_api_images_submodule():
+    return APIImagesSubModule()
```

### Comparing `walt-client-7/walt/client/log.py` & `walt-client-8.0/walt/client/image.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,288 +1,355 @@
-import sys, re, datetime, pickle
-from walt.common.constants import WALT_SERVER_TCP_PORT
-from walt.common.tcp import read_pickle, write_pickle, client_sock_file, \
-                            Requests
+#!/usr/bin/env python
+import re
+
 from plumbum import cli
-from walt.client.application import WalTCategoryApplication, WalTApplication
+from walt.client.application import WalTApplication, WalTCategoryApplication
 from walt.client.config import conf
 from walt.client.link import ClientToServerLink
 from walt.client.tools import confirm
-from walt.client.timeout import start_timeout, stop_timeout, timeout_reached, cli_timeout_switch
-
-DATE_FORMAT_STRING= '%Y-%m-%d %H:%M:%S'
-DATE_FORMAT_STRING_HUMAN= '<YYYY>-<MM>-<DD> <hh>:<mm>:<ss>'
-DATE_FORMAT_STRING_EXAMPLE= '2015-09-28 15:16:39'
-
-DEFAULT_FORMAT_STRING= \
-   '{timestamp:%H:%M:%S.%f} {sender}.{stream} -> {line}'
-
-SECONDS_PER_UNIT = {'s':1, 'm':60, 'h':3600, 'd':86400}
-NUM_LOGS_CONFIRM_TRESHOLD = 1000
-
-MSG_INVALID_CHECKPOINT_NAME="""\
-Invalid checkpoint name:
-* Only alnum and dash(-) characters are allowed.
-* dash(-) is not allowed as the 1st character.
+from walt.client.types import (
+    IMAGE,
+    IMAGE_BUILD_NAME,
+    IMAGE_CLONE_URL,
+    IMAGE_CP_DST,
+    IMAGE_CP_SRC,
+)
+
+MSG_WS_IS_EMPTY = """\
+Your working set is empty.
+Use 'walt image search [<keyword>]' to search for images
+you could build upon.
+Then use 'walt image clone <clonable_link>' to clone them
+into your working set.
 """
 
-def isatty():
-    return sys.stdout.isatty() and sys.stdin.isatty()
 
-def validate_checkpoint_name(name):
-    return re.match('^[a-zA-Z0-9]+[a-zA-Z0-9\-]+$', name)
+class WalTImage(WalTCategoryApplication):
+    """management of WalT-nodes operating system images"""
 
-def compute_relative_date(server_time, rel_date):
-    try:
-        delay = datetime.timedelta(
-                seconds = int(rel_date[1:-1]) * \
-                    SECONDS_PER_UNIT[rel_date[-1]])
-    except:
-        print("Invalid relative date. Should be: -<int>[dhms] (e.g. '-6h' for 'six hours ago')")
-        sys.exit(1)
-    return pickle.dumps(server_time - delay)
-
-class LogsFlowFromServer(object):
-    def __init__(self, walt_server_host):
-        self.f = client_sock_file(walt_server_host, WALT_SERVER_TCP_PORT)
-    def read_log_record(self):
-        return read_pickle(self.f)
-    def request_log_dump(self, **kwargs):
-        Requests.send_id(self.f, Requests.REQ_DUMP_LOGS)
-        write_pickle(kwargs, self.f)
-    def close(self):
-        self.f.close()
-
-class WalTLog(WalTCategoryApplication):
-    """management of logs"""
-    pass
-
-class WalTLogShowOrWait(WalTApplication):
-    """Implements options and features common to "show" and "wait" subcommands"""
-    format_string = cli.SwitchAttr(
-                "--format",
-                str,
-                argname = 'LOG_FORMAT',
-                default = DEFAULT_FORMAT_STRING,
-                help= """format used to print logs (see walt help show log-format)""")
-    set_of_nodes = cli.SwitchAttr(
-                "--nodes",
-                str,
-                argname = 'SET_OF_NODES',
-                default = 'my-nodes',
-                help= """targeted nodes (see walt help show node-terminology)""")
-    streams = cli.SwitchAttr(
-                "--streams",
-                str,
-                argname = 'STREAMS_REGEXP',
-                default = None,
-                help= """selected log streams (as a regular expr.)""")
-
-    @staticmethod
-    def analyse_history_range(server, history_range):
-        server_time = pickle.loads(server.get_pickled_time())
-        MALFORMED=(False,)
-        try:
-            if history_range.lower() == 'none':
-                return True, None
-            elif history_range.lower() == 'full':
-                return True, (None, None)
-            parts = history_range.split(':')
-            if len(parts) != 2:
-                return MALFORMED
-            history = []
-            for part in parts:
-                if part == '':
-                    history.append(None)
-                elif part.startswith('-'):
-                    rel_date = compute_relative_date(server_time, part)
-                    history.append(rel_date)
-                elif validate_checkpoint_name(part):
-                    cptime = server.get_pickled_checkpoint_time(part)
-                    if cptime == None:
-                        return MALFORMED
-                    history.append(cptime)
-                else:
-                    return MALFORMED
-            if history[0] and history[1]:
-                if pickle.loads(history[0]) > pickle.loads(history[1]):
-                    print('Issue with the HISTORY_RANGE specified: ' + \
-                            'the starting point is newer than the ending point.')
-                    return MALFORMED
-            return True, tuple(history)
-        except Exception as e:
-            return MALFORMED
-
-    @staticmethod
-    def verify_regexps(*regexps):
-        for regexp in regexps:
-            if regexp is None:
-                continue
-            try:
-                re.compile(regexp)
-            except:
-                print('Invalid regular expression: %s.' % regexp)
+    ORDERING = 1
+
+
+@WalTImage.subcommand("search")
+class WalTImageSearch(WalTApplication):
+    """search for remote WalT node OS images"""
+
+    ORDERING = 2
+
+    def main(self, keyword=None):
+        with ClientToServerLink() as server_link:
+            server_link.set_busy_label("Searching")
+            server_link.search_images(keyword)
+
+
+@WalTImage.subcommand("clone")
+class WalTImageClone(WalTApplication):
+    """clone a remote image into your working set"""
+
+    ORDERING = 3
+    _force = False  # default
+
+    def main(self, clonable_image_link: IMAGE_CLONE_URL, image_name=None):
+        with ClientToServerLink() as server_link:
+            server_link.set_busy_label("Validating / Cloning")
+            res = server_link.clone_image(
+                clonable_image_link, force=self._force, image_name=image_name
+            )
+            if res["status"] == "OK":
+                print(
+                    f'Image "{res["image_name"]}" was cloned successfully'
+                    " (cf. walt image show)."
+                )
+                return True  # success
+            else:
+                return False  # issue
+
+    @cli.autoswitch(help="do it, even if it overwrites an existing image.")
+    def force(self):
+        self._force = True
+
+
+@WalTImage.subcommand("publish")
+class WalTImagePublish(WalTApplication):
+    """publish a WalT image on the hub (or other registry)"""
+
+    ORDERING = 10
+    registry = cli.SwitchAttr(
+        ["--registry"],
+        str,
+        argname="REGISTRY",
+        default="auto",
+        help="""select which image registry to publish to""",
+    )
+
+    def main(self, image_name: IMAGE):
+        with ClientToServerLink() as server_link:
+            from walt.common.formatting import columnate
+            registries = server_link.get_registries()
+            if len(registries) == 0:
+                print("Sorry, no image registry is configured on this platform.")
                 return False
-        return True
+            if self.registry == "auto":
+                if len(registries) > 1:
+                    print("Several image registries are configured on this platform:")
+                    print()
+                    print(columnate(registries, ("Registry", "Description")))
+                    print()
+                    print(
+                        "Please specify the target registry by using option"
+                        " '--registry'."
+                    )
+                    return False
+                # there is a single registry => 'auto' is OK.
+                self.registry = registries[0][0]
+            else:
+                if self.registry not in tuple(reg_info[0] for reg_info in registries):
+                    print(f"Invalid registry '{self.registry}'.")
+                    print("The following registries are available:")
+                    print()
+                    print(columnate(registries, ("Registry", "Description")))
+                    return False
+            server_link.set_busy_label("Validating / Publishing")
+            res = server_link.publish_image(self.registry, image_name)
+            if res[0] is False:
+                return False
+            print(f"OK, image was published at:\n{res[1]}")
+
+
+@WalTImage.subcommand("show")
+class WalTImageShow(WalTApplication):
+    """display your working set of walt images"""
+
+    ORDERING = 1
+    _refresh = False  # default
+    _names_only = False  # default
+
+    def main(self):
+        if self._names_only:
+            fields = ("name",)
+        else:
+            fields = ("name", "in_use", "created", "compatibility:compact")
+        with ClientToServerLink() as server:
+            tabular_data = server.get_images_tabular_data(
+                conf.walt.username, self._refresh, fields
+            )
+        if self._names_only:
+            print("\n".join(row[0] for row in tabular_data))
+        else:
+            if len(tabular_data) == 0:
+                print(MSG_WS_IS_EMPTY)
+            else:
+                header = list(
+                    re.sub(r"([^:]*):.*", r"\1", f).capitalize().replace("_", "-")
+                    for f in fields
+                )
+                from walt.common.formatting import columnate
+                print(columnate(tabular_data, header))
+
+    @cli.autoswitch(help="resync image list from podman storage")
+    def refresh(self):
+        self._refresh = True
+
+    @cli.autoswitch(help="list image names only")
+    def names_only(self):
+        self._names_only = True
+
+
+@WalTImage.subcommand("shell")
+class WalTImageShell(WalTApplication):
+    """modify an image through an interactive shell"""
 
-    @staticmethod
-    def start_streaming(format_string, history_range, realtime, senders, streams,
-                        logline_regexp, stop_test, timeout = -1):
-        conn = LogsFlowFromServer(conf['server'])
-        conn.request_log_dump(  history = history_range,
-                                realtime = realtime,
-                                senders = senders,
-                                streams = streams,
-                                logline_regexp = logline_regexp)
-        if timeout > 0:
-            start_timeout(timeout)
-        while True:
+    ORDERING = 4
+
+    def main(self, image_name: IMAGE):
+        with ClientToServerLink() as server:
+            session_info = server.create_image_shell_session(
+                image_name, "shell session"
+            )
+            if session_info is None:
+                return  # issue already reported
+            session_id, image_fullname, container_name, default_new_name = session_info
+            from walt.client.interactive import run_image_shell_prompt
+            run_image_shell_prompt(image_fullname, container_name)
             try:
-                record = conn.read_log_record()
-                # sigalarm is caught by pickle, it will just abort the read
-                # and record will be None.
-                # Since we cannot get a TimeoutException, we check with timeout_reached().
-                if timeout > 0 and timeout_reached():
-                    print('Timeout was reached.')
-                    break
-                if record == None:
-                    break
-                print(format_string.format(**record))
-                sys.stdout.flush()
-                if stop_test is not None and stop_test(**record):
+                while True:
+                    new_name = input("New image name [%s]: " % default_new_name)
+                    if new_name == "":
+                        new_name = default_new_name
+                        print("Selected: %s" % new_name)
+                    res = server.image_shell_session_save(
+                        conf.walt.username, session_id, new_name, name_confirmed=False
+                    )
+                    if res == "NAME_NOT_OK":
+                        continue
+                    if res == "NAME_NEEDS_CONFIRM":
+                        if confirm(komsg=None):
+                            server.image_shell_session_save(
+                                conf.walt.username,
+                                session_id,
+                                new_name,
+                                name_confirmed=True,
+                            )
+                        else:
+                            continue
                     break
-            except KeyboardInterrupt:
-                print()
-                break
-            except Exception as e:
-                print('Could not display the log record.')
-                print('Verify your format string.')
-                break
-        if timeout > 0:
-            stop_timeout()
-
-@WalTLog.subcommand("show")
-class WalTLogShow(WalTLogShowOrWait):
-    """Dump logs on standard output"""
-    realtime = cli.Flag(
-                "--realtime",
-                default = False,
-                help= """enable realtime mode (see walt help show log-realtime)""")
-    history_range = cli.SwitchAttr(
-                "--history",
-                str,
-                argname = 'HISTORY_RANGE',
-                default = 'none',
-                help= """history range to be retrieved (see walt help show log-history)""")
-
-    def main(self, logline_regexp = None):
-        if self.realtime == False and self.history_range == 'none':
-            print('You must specify at least 1 of the options --realtime and --history.')
-            print("See 'walt help show log-realtime' and 'walt help show log-history' for more info.")
-            return
-        if not WalTLogShowOrWait.verify_regexps(self.streams, logline_regexp):
-            return
-        with ClientToServerLink() as server:
-            senders = server.parse_set_of_nodes(self.set_of_nodes)
-            if senders == None:
-                return
-            range_analysis = WalTLogShowOrWait.analyse_history_range(server, self.history_range)
-            if not range_analysis[0]:
-                print('''Invalid HISTORY_RANGE. See 'walt help show log-history' for more info.''')
-                return
-            history_range = range_analysis[1]
-            # Note : if a regular expression is specified, we do not bother computing the number
-            # of log records, because this computation would be too expensive, and the number of
-            # matching lines is probably low.
-            if history_range and logline_regexp is None and isatty():
-                num_logs = server.count_logs(history = history_range, senders = senders, streams = self.streams)
-                if num_logs > NUM_LOGS_CONFIRM_TRESHOLD:
-                    print('This will display approximately %d log records from history.' % num_logs)
-                    if not confirm():
-                        return
-        WalTLogShowOrWait.start_streaming(self.format_string, history_range, self.realtime,
-                                            senders, self.streams, logline_regexp, None)
-
-@WalTLog.subcommand("add-checkpoint")
-class WalTLogAddCheckpoint(WalTApplication):
-    """Record a checkpoint (reference point in time)"""
-    date = cli.SwitchAttr("--date", str, default=None,
-                          help="specify date (see walt help show log-checkpoint)")
-    def main(self, checkpoint_name):
+            except (KeyboardInterrupt, EOFError):
+                print("Aborted.")
+            # leaving the API session scoped by the with construct
+            # will cause the server to cleanup session data on server side.
+
+
+@WalTImage.subcommand("remove")
+class WalTImageRemove(WalTApplication):
+    """remove an image from your working set"""
+
+    ORDERING = 8
+
+    def main(self, image_name: IMAGE):
         with ClientToServerLink() as server:
-            if self.date:
-                if self.date.startswith('-'):
-                    server_time = pickle.loads(server.get_pickled_time())
-                    self.date = compute_relative_date(server_time, self.date)
-                else:
-                    try:
-                        self.date = pickle.dumps(datetime.datetime.strptime(\
-                                        self.date, DATE_FORMAT_STRING))
-                    except:
-                        print('Could not parse the date specified.')
-                        print('Expected format is: %s' % DATE_FORMAT_STRING_HUMAN)
-                        print('Example: %s' % DATE_FORMAT_STRING_EXAMPLE)
-                        return
-            if not validate_checkpoint_name(checkpoint_name):
-                sys.stderr.write(MSG_INVALID_CHECKPOINT_NAME)
-                return
-            server.add_checkpoint(checkpoint_name, self.date)
+            return server.remove_image(image_name)
+
+
+@WalTImage.subcommand("rename")
+class WalTImageRename(WalTApplication):
+    """rename an image of your working set"""
+
+    ORDERING = 9
 
-@WalTLog.subcommand("remove-checkpoint")
-class WalTLogRemoveCheckpoint(WalTApplication):
-    """Remove a checkpoint"""
-    def main(self, checkpoint_name):
+    def main(self, image_name: IMAGE, new_image_name):
         with ClientToServerLink() as server:
-            server.remove_checkpoint(checkpoint_name)
+            return server.rename_image(image_name, new_image_name)
 
-@WalTLog.subcommand("list-checkpoints")
-class WalTLogListCheckpoints(WalTApplication):
-    """List checkpoints"""
-    def main(self):
+
+@WalTImage.subcommand("duplicate")
+class WalTImageDuplicate(WalTApplication):
+    """duplicate an image of your working set"""
+
+    ORDERING = 7
+
+    def main(self, image_name: IMAGE, new_image_name):
         with ClientToServerLink() as server:
-            server.list_checkpoints()
+            return server.duplicate_image(image_name, new_image_name)
 
-@WalTLog.subcommand("wait")
-class WalTLogWait(WalTLogShowOrWait):
-    """Wait for a given log line"""
-    mode = cli.SwitchAttr(
-                "--mode",
-                cli.Set("ALL", "ANY", case_sensitive = False),
-                argname = 'MODE',
-                default = 'ANY',
-                help= """specify mode (see walt help show log-wait)""")
-    time_margin = cli.SwitchAttr(
-                "--time-margin",
-                int,
-                argname = 'SECONDS',
-                default = 0,
-                help= """also look in recent past logs if they matched""")
-    timeout = cli_timeout_switch()
 
-    def main(self, logline_regexp):
-        if not WalTLogShowOrWait.verify_regexps(self.streams, logline_regexp):
+@WalTImage.subcommand("build")
+class WalTImageBuild(WalTApplication):
+    """build a WalT image using a Dockerfile"""
+
+    ORDERING = 5
+    USAGE = """\
+    walt image build --from-url <git-repo-url> <image-name>
+    walt image build --from-dir <local-directory> <image-name>
+
+    See 'walt help show image-build' for more info.
+    """
+    src_url = cli.SwitchAttr(
+        "--from-url",
+        str,
+        argname="GIT_URL",
+        default=None,
+        help="""Git repository URL containing a Dockerfile""",
+    )
+    src_dir = cli.SwitchAttr(
+        "--from-dir",
+        str,
+        argname="DIRECTORY",
+        default=None,
+        help="""Local directory containing a Dockerfile""",
+    )
+
+    # note: we should not use type IMAGE like most other subcommands
+    # because IMAGE only selects existing image names whereas the user
+    # can specify a new image name here.
+    def main(self, image_name: IMAGE_BUILD_NAME):
+        if self.src_url is None and self.src_dir is None:
+            print("You must specify 1 of the options --from-url and --from-dir.")
+            print("See 'walt help show image-build' for more info.")
             return
+        mode = "dir" if self.src_url is None else "url"
         with ClientToServerLink() as server:
-            senders = server.parse_set_of_nodes(self.set_of_nodes)
-            if senders == None:
-                return
-            if self.time_margin != 0:
-                history_range = '-%ds:' % self.time_margin
-                range_analysis = WalTLogShowOrWait.analyse_history_range(server, history_range)
-                history_range = range_analysis[1]
+            info = dict(mode=mode, image_name=image_name)
+            if mode == "dir":
+                info["src_dir"] = self.src_dir
             else:
-                history_range = None
-        if self.mode == 'ANY':
-            # as soon as a logline matches, we stop
-            def stop_test(**record):
-                return True
-        else:
-            # we stop when all nodes have emitted a matching logline
-            missing_senders = set(senders)
-            def stop_test(**record):
-                missing_senders.discard(record['sender'])
-                if len(missing_senders) == 0:
-                    return True     # yes, we should stop
+                info["url"] = self.src_url
+            info = server.create_image_build_session(**info)
+            if info is None:
+                return False  # issue already reported
+            image_overwrite = info.pop("image_overwrite")
+            if image_overwrite:
+                if not confirm():
+                    return False
+            session_id = info.pop("session_id")
+            if mode == "dir":
+                from walt.client.transfer import run_transfer_for_image_build
+                try:
+                    if not run_transfer_for_image_build(**info):
+                        print("See 'walt help show image-build' for help.")
+                        return False
+                except (KeyboardInterrupt, EOFError):
+                    print()
+                    print("Aborted.")
+                    return False
+            else:
+                if not server.run_image_build_from_url(session_id):
+                    # failed
+                    print("See 'walt help show image-build' for help.")
+                    return False
+            server.finalize_image_build_session(session_id)
+
+
+@WalTImage.subcommand("cp")
+class WalTImageCp(WalTApplication):
+    """transfer files (client machine <-> image)"""
+
+    ORDERING = 6
+    USAGE = """\
+    walt image cp <local-path> <image>:<path>
+    walt image cp <image>:<path> <local-path>
+    """
+
+    def main(self, src: IMAGE_CP_SRC, dst: IMAGE_CP_DST):
+        with ClientToServerLink() as server:
+            info = server.validate_image_cp(src, dst)
+            if info is None:
+                return
+            if info["status"] == "NEEDS_CONFIRM":
+                if confirm():
+                    info["status"] = "OK"
                 else:
-                    return False    # no, we are not done yet
-        WalTLogShowOrWait.start_streaming(self.format_string, history_range, True,
-                                    senders, self.streams, logline_regexp, stop_test, self.timeout)
+                    return  # give up
+            if info["status"] == "FAILED":
+                return
+            session_info = server.create_image_shell_session(
+                info["image_name"], "file transfer"
+            )
+            if session_info is None:
+                return  # issue already reported
+            session_id, image_fullname, container_name, default_new_name = session_info
+            info.update(image_fullname=image_fullname, container_name=container_name)
+            from walt.client.transfer import run_transfer_with_image
+            try:
+                run_transfer_with_image(**info)
+                if info["client_operand_index"] == 0:
+                    # client was sending -> image has been modified
+                    # save the image under the same name
+                    server.image_shell_session_save(
+                        conf.walt.username, session_id, default_new_name, True
+                    )
+            except (KeyboardInterrupt, EOFError):
+                print()
+                print("Aborted.")
+
+
+@WalTImage.subcommand("squash")
+class WalTImageSquash(WalTApplication):
+    """squash all layers of an image into one"""
+
+    ORDERING = 11
+
+    def main(self, image_name: IMAGE):
+        with ClientToServerLink() as server:
+            status = server.squash_image(image_name, False)
+            if status == "NEEDS_CONFIRM":
+                if confirm():
+                    server.squash_image(image_name, True)
```

### Comparing `walt-client-7/walt/client/vpn.py` & `walt-client-8.0/walt/client/vpn.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,115 @@
-import os, sys
-from plumbum import cli
-from walt.client.link import ClientToServerLink
-from walt.client.application import WalTCategoryApplication, WalTApplication
+import os
+import sys
+
+from walt.client.application import WalTApplication, WalTCategoryApplication
+from walt.client.link import ClientToServerLink, connect_to_tcp_server
 from walt.client.tools import yes_or_no
-from walt.client.config import conf
-from walt.common.tcp import write_pickle, client_sock_file, \
-                            Requests
-from walt.common.constants import WALT_SERVER_TCP_PORT
+from walt.common.tcp import Requests, write_pickle
+
 
 class WalTVPN(WalTCategoryApplication):
     """VPN related sub-commands"""
-    pass
 
-WAIT_VPN_BUSY_LABEL='\
-Waiting for next VPN connection attempt (press ctrl-C to stop)'
+    ORDERING = 5
+
+
+WAIT_VPN_BUSY_LABEL = "Waiting for next VPN connection attempt (press ctrl-C to stop)"
+
 
 @WalTVPN.subcommand("monitor")
 class WalTVPNMonitor(WalTApplication):
-    """Monitor VPN and accept/deny new connection requests"""
+    """monitor VPN and accept/deny new connection requests"""
+
     def main(self):
         with ClientToServerLink() as server:
             while True:
                 server.set_busy_label(WAIT_VPN_BUSY_LABEL)
                 try:
                     device_mac = server.vpn_wait_grant_request()
                 except KeyboardInterrupt:
                     print()
                     break
-                print('New VPN access request from device ' + device_mac + '.')
-                grant_ok = yes_or_no('Should this device be granted VPN access?')
-                print('Transmitting to walt server...')
+                print("New VPN access request from device " + device_mac + ".")
+                grant_ok = yes_or_no("Should this device be granted VPN access?")
+                print("Transmitting to walt server...")
                 server.set_default_busy_label()
                 result, comment = server.vpn_respond_grant_request(device_mac, grant_ok)
-                if result == 'OK':
+                if result == "OK":
                     print(comment)
                 else:
-                    print('FAILED! ' + comment)
+                    print("FAILED! " + comment)
+
 
 @WalTVPN.subcommand("setup-proxy")
 class WalTVPNSetupProxy(WalTApplication):
-    """Setup an ssh frontend server as a WalT VPN proxy"""
+    """setup an ssh frontend server as a WalT VPN proxy"""
+
     def main(self):
         with ClientToServerLink() as server:
             script_content = server.get_vpn_proxy_setup_script()
-            with open('proxy-setup.sh', 'w') as f:
+            with open("proxy-setup.sh", "w") as f:
                 f.write(script_content)
-                os.fchmod(f.fileno(), 0o755)    # set it executable
+                os.fchmod(f.fileno(), 0o755)  # set it executable
         print("A script 'proxy-setup.sh' has been generated in current directory.")
         print("Copy and run it on the host you want to use as a walt vpn proxy.")
 
+
 def read_vpn_node_image(entrypoint):
     # connect to server
-    sock = client_sock_file(conf['server'], WALT_SERVER_TCP_PORT)
+    sock = connect_to_tcp_server()
     # send the request id
     Requests.send_id(sock, Requests.REQ_VPN_NODE_IMAGE)
     # wait for the READY message from the server
     sock.readline()
     # write the parameters
-    write_pickle(dict(model='rpi-3-b-plus', entrypoint=entrypoint), sock)
+    write_pickle(dict(model="rpi-3-b-plus", entrypoint=entrypoint), sock)
     # initial communication loop
     while True:
-        line = sock.readline().decode('UTF-8').strip()
+        line = sock.readline().decode("UTF-8").strip()
         words = line.split()
-        if words[0] == 'MSG':
-            print(' '.join(words[1:]))
-        elif words[0] == 'ERR':
-            print(' '.join(words[1:]), file=sys.stderr)
+        if words[0] == "MSG":
+            print(" ".join(words[1:]))
+        elif words[0] == "ERR":
+            print(" ".join(words[1:]), file=sys.stderr)
             return
-        elif words[0] == 'START':
+        elif words[0] == "START":
             break
         else:
-            print('Unexpected communication issue with walt server!', file=sys.stderr)
+            print("Unexpected communication issue with walt server!", file=sys.stderr)
             return
     # starting transfer
-    with open('rpi3bp-vpn.dd', 'wb') as f:
+    with open("rpi3bp-vpn.dd", "wb") as f:
         while True:
             chunk = sock.read(2048)
             if len(chunk) == 0:
                 break
             f.write(chunk)
     sock.close()
     print("A file 'rpi3bp-vpn.dd' has been generated in current directory.")
-    print("Flash it (using dd tool or similar) on the SD card of the rpi3b+ board you want to use as a VPN node.")
+    print(
+        "Flash it (using dd tool or similar) on the SD card of the rpi3b+ board you"
+        " want to use as a VPN node."
+    )
+
 
 @WalTVPN.subcommand("setup-node")
 class WalTVPNSetupNode(WalTApplication):
-    """Setup a WalT VPN node"""
+    """setup a WalT VPN node"""
+
     def main(self):
-        print("Note: for now only raspberry pi 3B+ boards can be used as a walt VPN node.")
+        print(
+            "Note: for now only raspberry pi 3B+ boards can be used as a walt VPN node."
+        )
         print("This procedure will generate an appropriate SD card image.")
-        entrypoint = ''
-        while entrypoint == '':
-            print('Please indicate the WalT VPN entrypoint (hostname or IP address) this node will connect to:', end=' ')
+        entrypoint = ""
+        while entrypoint == "":
+            print(
+                (
+                    "Please indicate the WalT VPN entrypoint (hostname or IP address)"
+                    " this node will connect to:"
+                ),
+                end=" ",
+            )
             entrypoint = input()
-        print('OK.\n')
+        print("OK.\n")
         read_vpn_node_image(entrypoint)
```

### Comparing `walt-client-7/walt_client.egg-info/SOURCES.txt` & `walt-client-8.0/walt_client.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,74 +1,117 @@
 MANIFEST.in
 README.txt
 setup.py
-bash_completion/walt
 walt/__init__.py
 walt/client/__init__.py
 walt/client/advanced.py
+walt/client/apitools.py
 walt/client/application.py
 walt/client/auth.py
 walt/client/client.py
 walt/client/config.py
+walt/client/console.py
 walt/client/device.py
+walt/client/exceptions.py
 walt/client/expose.py
 walt/client/filesystem.py
 walt/client/image.py
-walt/client/info.py
 walt/client/interactive.py
 walt/client/link.py
 walt/client/log.py
 walt/client/logo.py
 walt/client/myhelp.py
 walt/client/node.py
+walt/client/plugins.py
+walt/client/progress.py
+walt/client/speedup.py
 walt/client/startup.py
-walt/client/term.py
 walt/client/timeout.py
 walt/client/tools.py
 walt/client/transfer.py
+walt/client/types.py
+walt/client/update.py
 walt/client/vpn.py
+walt/client/wrap.py
+walt/client/apiobject/__init__.py
+walt/client/apiobject/base.py
+walt/client/apiobject/config.py
+walt/client/apiobject/images.py
+walt/client/apiobject/logs.py
+walt/client/apiobject/nodes.py
+walt/client/apiobject/root.py
+walt/client/apiobject/server.py
+walt/client/apiobject/tools.py
+walt/client/autocomplete/__init__.py
+walt/client/autocomplete/dump.py
+walt/client/autocomplete/helper.py
 walt/client/doc/__init__.py
 walt/client/doc/color.py
 walt/client/doc/markdown.py
 walt/client/doc/mdtable.py
 walt/client/doc/pager.py
 walt/client/doc/md/__init__.py
 walt/client/doc/md/admin.md
 walt/client/doc/md/compatibility.md
+walt/client/doc/md/design-notes.md
 walt/client/doc/md/device-config.md
+walt/client/doc/md/device-expose.md
+walt/client/doc/md/device-netsetup.md
 walt/client/doc/md/device-sets.md
+walt/client/doc/md/g5k.md
 walt/client/doc/md/help-intro.md
+walt/client/doc/md/image-build.md
 walt/client/doc/md/image-cp.md
 walt/client/doc/md/image-from-scratch.md
 walt/client/doc/md/image-spec-file.md
 walt/client/doc/md/log-cat.md
 walt/client/doc/md/log-checkpoint.md
 walt/client/doc/md/log-echo.md
 walt/client/doc/md/log-format.md
 walt/client/doc/md/log-history.md
+walt/client/doc/md/log-issuers.md
 walt/client/doc/md/log-monitor.md
 walt/client/doc/md/log-realtime.md
+walt/client/doc/md/log-show.md
 walt/client/doc/md/log-tee.md
 walt/client/doc/md/log-wait.md
 walt/client/doc/md/logging.md
 walt/client/doc/md/networking.md
 walt/client/doc/md/new-node-support.md
 walt/client/doc/md/node-bootup.md
+walt/client/doc/md/node-config.md
+walt/client/doc/md/node-console.md
 walt/client/doc/md/node-cp.md
+walt/client/doc/md/node-expose.md
 walt/client/doc/md/node-install.md
 walt/client/doc/md/node-netsetup.md
-walt/client/doc/md/node-terminology.md
+walt/client/doc/md/node-ownership.md
+walt/client/doc/md/optional-features.md
+walt/client/doc/md/packaging.md
+walt/client/doc/md/registries.md
+walt/client/doc/md/rpi-serial.md
+walt/client/doc/md/scripting-images.md
+walt/client/doc/md/scripting-logs.md
+walt/client/doc/md/scripting-nodes.md
+walt/client/doc/md/scripting-tools.md
+walt/client/doc/md/scripting.md
 walt/client/doc/md/server-install.md
 walt/client/doc/md/server-network-config.md
-walt/client/doc/md/server-setup-from-fresh-debian.md
-walt/client/doc/md/server-setup-from-image.md
 walt/client/doc/md/server-upgrade.md
+walt/client/doc/md/shell-completion.md
 walt/client/doc/md/shells.md
 walt/client/doc/md/switch-install.md
+walt/client/doc/md/troubleshooting.md
 walt/client/doc/md/tutorial.md
+walt/client/doc/md/unmanaged-devices.md
+walt/client/doc/md/vnode-networks.md
 walt/client/doc/md/vpn.md
+walt/client/doc/sphinx/conf.py
+walt/client/doc/sphinx/version.py
+walt/client/metadata/__init__.py
+walt/client/metadata/core.py
 walt_client.egg-info/PKG-INFO
 walt_client.egg-info/SOURCES.txt
 walt_client.egg-info/dependency_links.txt
 walt_client.egg-info/entry_points.txt
 walt_client.egg-info/requires.txt
 walt_client.egg-info/top_level.txt
```

