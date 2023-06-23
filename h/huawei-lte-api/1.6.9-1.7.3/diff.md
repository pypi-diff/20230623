# Comparing `tmp/huawei-lte-api-1.6.9.tar.gz` & `tmp/huawei-lte-api-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huawei-lte-api-1.6.9.tar", last modified: Mon Dec 19 05:32:24 2022, max compression
+gzip compressed data, was "huawei-lte-api-1.7.3.tar", last modified: Fri Jun 23 11:21:26 2023, max compression
```

## Comparing `huawei-lte-api-1.6.9.tar` & `huawei-lte-api-1.7.3.tar`

### file list

```diff
@@ -1,112 +1,114 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 05:32:24.732824 huawei-lte-api-1.6.9/
--rw-rw-rw-   0 root         (0) root         (0)       69 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6195 2022-12-19 05:32:24.732824 huawei-lte-api-1.6.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4062 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 05:32:24.720824 huawei-lte-api-1.6.9/huawei_lte_api/
--rw-rw-rw-   0 root         (0) root         (0)      136 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/ApiGroup.py
--rw-rw-rw-   0 root         (0) root         (0)      327 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/AuthorizedConnection.py
--rw-rw-rw-   0 root         (0) root         (0)     7098 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/Client.py
--rw-rw-rw-   0 root         (0) root         (0)     2020 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/Connection.py
--rw-rw-rw-   0 root         (0) root         (0)    12987 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/Session.py
--rw-rw-rw-   0 root         (0) root         (0)     2745 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/Tools.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 05:32:24.728824 huawei-lte-api-1.6.9/huawei_lte_api/api/
--rw-rw-rw-   0 root         (0) root         (0)      396 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/App.py
--rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Bluetooth.py
--rw-rw-rw-   0 root         (0) root         (0)      629 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Cradle.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Cwmp.py
--rw-rw-rw-   0 root         (0) root         (0)      411 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/DDns.py
--rw-rw-rw-   0 root         (0) root         (0)      364 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Developer.py
--rw-rw-rw-   0 root         (0) root         (0)     3281 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Device.py
--rw-rw-rw-   0 root         (0) root         (0)     2916 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Dhcp.py
--rw-rw-rw-   0 root         (0) root         (0)     1107 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Diagnosis.py
--rw-rw-rw-   0 root         (0) root         (0)     4223 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/DialUp.py
--rw-rw-rw-   0 root         (0) root         (0)      944 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/FileManager.py
--rw-rw-rw-   0 root         (0) root         (0)      566 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Global.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Host.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Lan.py
--rw-rw-rw-   0 root         (0) root         (0)      461 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Language.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Led.py
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Log.py
--rw-rw-rw-   0 root         (0) root         (0)      343 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/MLog.py
--rw-rw-rw-   0 root         (0) root         (0)     3123 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Monitoring.py
--rw-rw-rw-   0 root         (0) root         (0)     3105 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Net.py
--rw-rw-rw-   0 root         (0) root         (0)      538 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Ntwk.py
--rw-rw-rw-   0 root         (0) root         (0)     1907 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/OnlineUpdate.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Ota.py
--rw-rw-rw-   0 root         (0) root         (0)     4374 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Pb.py
--rw-rw-rw-   0 root         (0) root         (0)     1421 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Pin.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Redirection.py
--rw-rw-rw-   0 root         (0) root         (0)      507 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/SNtp.py
--rw-rw-rw-   0 root         (0) root         (0)     2847 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/SdCard.py
--rw-rw-rw-   0 root         (0) root         (0)     3755 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Security.py
--rw-rw-rw-   0 root         (0) root         (0)     6447 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Sms.py
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Staticroute.py
--rw-rw-rw-   0 root         (0) root         (0)      251 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Statistic.py
--rw-rw-rw-   0 root         (0) root         (0)      379 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Syslog.py
--rw-rw-rw-   0 root         (0) root         (0)     1051 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/System.py
--rw-rw-rw-   0 root         (0) root         (0)      212 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Time.py
--rw-rw-rw-   0 root         (0) root         (0)      218 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/TimeRule.py
--rw-rw-rw-   0 root         (0) root         (0)      232 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/UsbPrinter.py
--rw-rw-rw-   0 root         (0) root         (0)      330 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/UsbStorage.py
--rw-rw-rw-   0 root         (0) root         (0)     7148 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/User.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Ussd.py
--rw-rw-rw-   0 root         (0) root         (0)      233 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/VSim.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Voice.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/Vpn.py
--rw-rw-rw-   0 root         (0) root         (0)     9130 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/WLan.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/WebServer.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 05:32:24.732824 huawei-lte-api-1.6.9/huawei_lte_api/config/
--rw-rw-rw-   0 root         (0) root         (0)      234 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Device.py
--rw-rw-rw-   0 root         (0) root         (0)      269 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/DeviceInformation.py
--rw-rw-rw-   0 root         (0) root         (0)      633 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/DialUp.py
--rw-rw-rw-   0 root         (0) root         (0)      238 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/FastBoot.py
--rw-rw-rw-   0 root         (0) root         (0)      238 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Firewall.py
--rw-rw-rw-   0 root         (0) root         (0)      476 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Global.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/IPv6.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Lan.py
--rw-rw-rw-   0 root         (0) root         (0)      734 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Network.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Ota.py
--rw-rw-rw-   0 root         (0) root         (0)      226 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Pb.py
--rw-rw-rw-   0 root         (0) root         (0)      376 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/PcAssistant.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Pincode.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Sms.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Sntp.py
--rw-rw-rw-   0 root         (0) root         (0)      240 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Statistic.py
--rw-rw-rw-   0 root         (0) root         (0)      228 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Stk.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/UPnp.py
--rw-rw-rw-   0 root         (0) root         (0)      234 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Update.py
--rw-rw-rw-   0 root         (0) root         (0)      363 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Ussd.py
--rw-rw-rw-   0 root         (0) root         (0)      346 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Voice.py
--rw-rw-rw-   0 root         (0) root         (0)      232 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/WebSd.py
--rw-rw-rw-   0 root         (0) root         (0)      238 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/WebUICfg.py
--rw-rw-rw-   0 root         (0) root         (0)      625 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/Wifi.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 05:32:24.732824 huawei-lte-api-1.6.9/huawei_lte_api/enums/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/enums/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      456 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/enums/client.py
--rw-rw-rw-   0 root         (0) root         (0)      243 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/enums/cradle.py
--rw-rw-rw-   0 root         (0) root         (0)      278 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/enums/device.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/enums/dialup.py
--rw-rw-rw-   0 root         (0) root         (0)     1032 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/enums/net.py
--rw-rw-rw-   0 root         (0) root         (0)      668 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/enums/sms.py
--rw-rw-rw-   0 root         (0) root         (0)      506 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/enums/user.py
--rw-rw-rw-   0 root         (0) root         (0)      428 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/enums/wlan.py
--rw-rw-rw-   0 root         (0) root         (0)     1272 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)       14 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 05:32:24.732824 huawei-lte-api-1.6.9/huawei_lte_api/usermanual/
--rw-rw-rw-   0 root         (0) root         (0)      264 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/usermanual/PublicSysResources.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/huawei_lte_api/usermanual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 05:32:24.720824 huawei-lte-api-1.6.9/huawei_lte_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6195 2022-12-19 05:32:24.000000 huawei-lte-api-1.6.9/huawei_lte_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3025 2022-12-19 05:32:24.000000 huawei-lte-api-1.6.9/huawei_lte_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-19 05:32:24.000000 huawei-lte-api-1.6.9/huawei_lte_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2022-12-19 05:32:24.000000 huawei-lte-api-1.6.9/huawei_lte_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-12-19 05:32:24.000000 huawei-lte-api-1.6.9/huawei_lte_api.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       61 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      275 2022-12-19 05:32:24.732824 huawei-lte-api-1.6.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1570 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 05:32:24.732824 huawei-lte-api-1.6.9/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      180 2022-12-19 05:31:45.000000 huawei-lte-api-1.6.9/tests/test_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:21:26.149083 huawei-lte-api-1.7.3/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5326 2023-06-23 11:21:26.149083 huawei-lte-api-1.7.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4324 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:21:26.137083 huawei-lte-api-1.7.3/huawei_lte_api/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/ApiGroup.py
+-rw-rw-rw-   0 root         (0) root         (0)      327 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/AuthorizedConnection.py
+-rw-rw-rw-   0 root         (0) root         (0)     7098 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/Client.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/Connection.py
+-rw-rw-rw-   0 root         (0) root         (0)    12987 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/Session.py
+-rw-rw-rw-   0 root         (0) root         (0)     3278 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/Tools.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:21:26.145083 huawei-lte-api-1.7.3/huawei_lte_api/api/
+-rw-rw-rw-   0 root         (0) root         (0)      396 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/App.py
+-rw-rw-rw-   0 root         (0) root         (0)      554 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Bluetooth.py
+-rw-rw-rw-   0 root         (0) root         (0)      629 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Cradle.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Cwmp.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/DDns.py
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Developer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3822 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Device.py
+-rw-rw-rw-   0 root         (0) root         (0)     2916 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Dhcp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Diagnosis.py
+-rw-rw-rw-   0 root         (0) root         (0)     4223 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/DialUp.py
+-rw-rw-rw-   0 root         (0) root         (0)      944 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/FileManager.py
+-rw-rw-rw-   0 root         (0) root         (0)      566 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Global.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Host.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Lan.py
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Language.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Led.py
+-rw-rw-rw-   0 root         (0) root         (0)      210 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Log.py
+-rw-rw-rw-   0 root         (0) root         (0)      343 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/MLog.py
+-rw-rw-rw-   0 root         (0) root         (0)     3283 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Monitoring.py
+-rw-rw-rw-   0 root         (0) root         (0)     3525 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Net.py
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Ntwk.py
+-rw-rw-rw-   0 root         (0) root         (0)     1907 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/OnlineUpdate.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Ota.py
+-rw-rw-rw-   0 root         (0) root         (0)     4374 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Pb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1421 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Pin.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Redirection.py
+-rw-rw-rw-   0 root         (0) root         (0)      507 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/SNtp.py
+-rw-rw-rw-   0 root         (0) root         (0)     5085 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/SdCard.py
+-rw-rw-rw-   0 root         (0) root         (0)     3755 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Security.py
+-rw-rw-rw-   0 root         (0) root         (0)    12758 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Sms.py
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Staticroute.py
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Statistic.py
+-rw-rw-rw-   0 root         (0) root         (0)      379 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Syslog.py
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/System.py
+-rw-rw-rw-   0 root         (0) root         (0)      212 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Time.py
+-rw-rw-rw-   0 root         (0) root         (0)      218 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/TimeRule.py
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/UsbPrinter.py
+-rw-rw-rw-   0 root         (0) root         (0)      330 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/UsbStorage.py
+-rw-rw-rw-   0 root         (0) root         (0)     7373 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/User.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Ussd.py
+-rw-rw-rw-   0 root         (0) root         (0)      233 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/VSim.py
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Voice.py
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/Vpn.py
+-rw-rw-rw-   0 root         (0) root         (0)     9877 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/WLan.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/WebServer.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:21:26.145083 huawei-lte-api-1.7.3/huawei_lte_api/config/
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Device.py
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/DeviceInformation.py
+-rw-rw-rw-   0 root         (0) root         (0)      633 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/DialUp.py
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/FastBoot.py
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Firewall.py
+-rw-rw-rw-   0 root         (0) root         (0)      476 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Global.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/IPv6.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Lan.py
+-rw-rw-rw-   0 root         (0) root         (0)      734 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Network.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Ota.py
+-rw-rw-rw-   0 root         (0) root         (0)      226 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Pb.py
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/PcAssistant.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Pincode.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Sms.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Sntp.py
+-rw-rw-rw-   0 root         (0) root         (0)      240 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Statistic.py
+-rw-rw-rw-   0 root         (0) root         (0)      228 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Stk.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/UPnp.py
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Update.py
+-rw-rw-rw-   0 root         (0) root         (0)      363 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Ussd.py
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Voice.py
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/WebSd.py
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/WebUICfg.py
+-rw-rw-rw-   0 root         (0) root         (0)      625 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/Wifi.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:21:26.149083 huawei-lte-api-1.7.3/huawei_lte_api/enums/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/enums/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/enums/client.py
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/enums/cradle.py
+-rw-rw-rw-   0 root         (0) root         (0)      581 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/enums/device.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/enums/dialup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/enums/net.py
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/enums/sdcard.py
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/enums/sms.py
+-rw-rw-rw-   0 root         (0) root         (0)      506 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/enums/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/enums/wlan.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:21:26.149083 huawei-lte-api-1.7.3/huawei_lte_api/usermanual/
+-rw-rw-rw-   0 root         (0) root         (0)      264 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/usermanual/PublicSysResources.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/huawei_lte_api/usermanual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:21:26.137083 huawei-lte-api-1.7.3/huawei_lte_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5326 2023-06-23 11:21:26.000000 huawei-lte-api-1.7.3/huawei_lte_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-06-23 11:21:26.000000 huawei-lte-api-1.7.3/huawei_lte_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 11:21:26.000000 huawei-lte-api-1.7.3/huawei_lte_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-23 11:21:26.000000 huawei-lte-api-1.7.3/huawei_lte_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-23 11:21:26.000000 huawei-lte-api-1.7.3/huawei_lte_api.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-06-23 11:21:26.149083 huawei-lte-api-1.7.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 11:21:26.149083 huawei-lte-api-1.7.3/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-06-23 11:20:02.000000 huawei-lte-api-1.7.3/tests/test_init.py
```

### Comparing `huawei-lte-api-1.6.9/README.md` & `huawei-lte-api-1.7.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 * Huawei E3131
 * Huawei E3372
 * Huawei E3531
 
 
 #### 5G Routers:
 * Huawei 5G CPE Pro 2 (H122-373)
+* Huawei 5G CPE Pro (H112-372)
 
 (probably will work for other Huawei LTE devices too)
 
 ### Will NOT work on:
 #### LTE Routers:
 * Huawei B2368-22 (Incompatible firmware, testing device needed!)
 * Huawei B593s-22 (Incompatible firmware, testing device needed!)
@@ -113,14 +114,16 @@
 
 Some code [examples](examples/) are in [/examples](examples/)  folder
 
 ### Monitoring
 
 * Monitoring traffic and signal https://github.com/littlejo/huawei-lte-examples
 * Set band, show signal level and bandwidth for Huawei mobile broadband B525s-23a. https://github.com/octave21/huawei-lte
+* Application that monitors Internet connectivity and restarts router when internet is not reachable https://github.com/Salamek/netkeeper
+* Monitoring app with nice TUI interface (just like htop) https://github.com/pdo-smith/5gtop
 
 ### SMS
 
 * Relay received SMS into your email https://github.com/chenwei791129/Huawei-LTE-Router-SMS-to-E-mail-Sender
 
 ## Ports to other languages
```

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/Client.py` & `huawei-lte-api-1.7.3/huawei_lte_api/Client.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/Connection.py` & `huawei-lte-api-1.7.3/huawei_lte_api/Connection.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                  username: Optional[str] = None,
                  password: Optional[str] = None,
                  login_on_demand: bool = False,
                  timeout: Union[float, Tuple[float, float], None] = None,
                  requests_session: Optional[requests.Session] = None
                  ):
         """
-        :param requests_session: requests Session to use, closing it is the caller's responsibility
+        :param requests_session: requests Session to use; if not None, closing it is the caller's responsibility
         """
         parsed_url = urlparse(url)
 
         # User login code
         username = username or parsed_url.username
         password = password if password else parsed_url.password
```

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/Session.py` & `huawei-lte-api-1.7.3/huawei_lte_api/Session.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/Tools.py` & `huawei-lte-api-1.7.3/huawei_lte_api/Tools.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import datetime
 from typing import Optional, Tuple, Iterator, TypeVar, Iterable
 
 from binascii import hexlify
 import math
 import base64
 from Cryptodome.Cipher import PKCS1_v1_5, PKCS1_OAEP
 from Cryptodome.PublicKey.RSA import construct
 
 
 T = TypeVar('T')
 
+
 class Tools:
+    datetime_format = '%Y-%m-%d %H:%M:%S'
 
     @staticmethod
     def enforce_list_response(data: dict, singular_key_name: str, plural_key_name: Optional[str] = None) -> dict:
         """
         Make sure Hosts->Host is a list
         It may be returned as a single dict if only one is associated,
         as well as sometimes None.
@@ -78,7 +81,20 @@
                     if data_item.get(attr) != value:
                         break
                 else:
                     if getattr(data_item, attr) != value:
                         break
             else:
                 yield data_item
+
+    @staticmethod
+    def string_to_datetime(datetime_string: str) -> datetime.datetime:
+        """
+        Parses datetime in format 2022-12-22 18:01:09
+        :param datetime_string: string to parse
+        :return: datetime.datetime
+        """
+        return datetime.datetime.strptime(datetime_string, Tools.datetime_format)
+
+    @staticmethod
+    def datetime_to_string(date_time: datetime.datetime) -> str:
+        return date_time.strftime(Tools.datetime_format)
```

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/Bluetooth.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/Bluetooth.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/Cradle.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/Cradle.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/Device.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/Device.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import warnings
 from huawei_lte_api.ApiGroup import ApiGroup
 from huawei_lte_api.Session import GetResponseType, SetResponseType
-from huawei_lte_api.enums.device import AntennaTypeEnum, ControlModeEnum
+from huawei_lte_api.enums.device import AntennaTypeEnum, ControlModeEnum, ModeEnum
 
 
 class Device(ApiGroup):
     def information(self) -> GetResponseType:
         return self._session.get('device/information')
 
     def autorun_version(self) -> GetResponseType:
@@ -81,7 +81,24 @@
         """
         This endpoint is known to break the session with some devices
         that don't support it. Approach with care.
         """
         return self._session.post_get('device/vendorname', {
             'language': lang
         })
+
+    def mode(self, mode: ModeEnum) -> SetResponseType:
+        """
+        Sets mode of the device, it can enable telnet, set debug mode or production mode, see ModeEnum
+        :param mode: ModeEnum
+        :return: SetResponseType
+        """
+        return self._session.post_set('device/mode', {
+            'mode': mode
+        })
+
+    def compress_logfile(self) -> GetResponseType:
+        """
+        Returns link to archived log file
+        :return:
+        """
+        return self._session.get('device/compresslogfile')
```

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/Dhcp.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/Dhcp.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/Diagnosis.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/Diagnosis.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/DialUp.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/DialUp.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/FileManager.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/FileManager.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/Global.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/Global.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/Host.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/Host.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/Monitoring.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/Monitoring.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 
 
 class Monitoring(ApiGroup):
     def converged_status(self) -> GetResponseType:
         return self._session.get('monitoring/converged-status')
 
     def status(self) -> GetResponseType:
+        """
+        Returns status info of the router
+        Note: for signal some routers return correct value in SignalIcon some in SignalIconNr
+        """
         return self._session.get('monitoring/status')
 
     def check_notifications(self) -> GetResponseType:
         return self._session.get('monitoring/check-notifications')
 
     def traffic_statistics(self) -> GetResponseType:
         return self._session.get('monitoring/traffic-statistics')
```

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/Net.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/Net.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,14 +30,24 @@
             ('NetworkBand', networkband if isinstance(networkband, str) else hex(networkband)[2:]),
             ('LTEBand', lteband if isinstance(lteband, str) else hex(lteband)[2:]),
         )))
 
     def network(self) -> GetResponseType:
         return self._session.get('net/network')
 
+    def set_network(self, networkmode: str, networkband: str) -> SetResponseType:
+        """
+        :param networkmode: different value range than in net_mode/NetworkModeEnun
+        :param networkband: different value range than in net_mode
+        """
+        return self._session.post_set('net/network', OrderedDict((
+            ('NetworkMode', networkmode),
+            ('NetworkBand', networkband),
+        )))
+
     def register(self) -> GetResponseType:
         return self._session.get('net/register')
 
     def set_register(self, mode: str, plmn: str, rat: str) -> SetResponseType:
         """
         Sets network selection
         :param mode: "1": manual network selection, "0": auto
```

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/Ntwk.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/Ntwk.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/OnlineUpdate.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/OnlineUpdate.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/Pb.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/Pb.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/Pin.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/Pin.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/Security.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/Security.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/System.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/System.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/User.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/User.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,31 @@
 from huawei_lte_api.exceptions import ResponseErrorException, \
     LoginErrorAlreadyLoginException, \
     LoginErrorUsernamePasswordModifyException, \
     LoginErrorUsernamePasswordOverrunException, \
     LoginErrorUsernamePasswordWrongException, \
     LoginErrorUsernameWrongException, \
     LoginErrorPasswordWrongException, \
+    ResponseErrorLoginRequiredException, \
     ResponseErrorNotSupportedException
 
 DEFAULT_USERNAME = 'admin'
 
 
 class UserSession:
     def __init__(self, session: Session, username: str = DEFAULT_USERNAME, password: Optional[str] = None):
         self.user = User(session)
         self.user.login(username, password, True)
 
     def close(self) -> None:
-        self.user.logout()
+        try:
+            self.user.logout()
+        except (ResponseErrorLoginRequiredException, ResponseErrorNotSupportedException):
+            # Idempotency/nothing further to do, suppress
+            pass
 
     def __enter__(self) -> 'UserSession':
         return self
 
     def __exit__(self, exc_type: Optional[Type[BaseException]],
                  exc_value: Optional[BaseException],
                  traceback: Optional[TracebackType]) -> None:
```

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/Voice.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/Voice.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/Vpn.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/Vpn.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from huawei_lte_api.ApiGroup import ApiGroup
-from huawei_lte_api.Session import GetResponseType
+from huawei_lte_api.Session import GetResponseType, SetResponseType
 
 
 class Vpn(ApiGroup):
 
     def feature_switch(self) -> GetResponseType:
         return self._session.get('vpn/feature-switch')
 
@@ -15,13 +15,23 @@
 
     def l2tp_settings(self) -> GetResponseType:
         return self._session.get('vpn/l2tp_settings')
 
     def pptp_settings(self) -> GetResponseType:
         return self._session.get('vpn/pptp_settings')
 
+    def toggle_status(self, enable: bool = True) -> SetResponseType:
+        data = {
+            "enable": "1" if enable else "0",
+        }
+        return self._session.post_set(
+            "vpn/l2tp_settings",
+            data=data,
+            is_encrypted=True,
+        )
+
     def status(self) -> GetResponseType:
         """
         Endpoint found by reverse engineering B310s-22 firmware, unknown usage
         :return:
         """
         return self._session.get('vpn/status')
```

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/WLan.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/WLan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dataclasses
 from collections import OrderedDict
-from typing import List, Optional
+from typing import List, Optional, Iterable
 
 from huawei_lte_api.ApiGroup import ApiGroup
 from huawei_lte_api.Session import GetResponseType, SetResponseType
 from huawei_lte_api.enums.wlan import AuthModeEnum, WepEncryptModeEnum, WpaEncryptModeEnum
 from huawei_lte_api.Tools import Tools
 
 
@@ -166,20 +166,37 @@
 
     def wps(self) -> GetResponseType:
         return self._session.get('wlan/wps')
 
     def wps_appin(self) -> GetResponseType:
         return self._session.get('wlan/wps-appin')
 
+    def set_wps_appin(self, wpsappintype: int = 0, wpsappin: Optional[int] = None) -> SetResponseType:
+        return self._session.post_set('wlan/wps-appin', OrderedDict((
+            ('wpsappintype', wpsappintype),
+            ('wpsappin', str(wpsappin) if wpsappin is not None else ''),
+        )))
+
     def wps_pbc(self) -> GetResponseType:
         return self._session.get('wlan/wps-pbc')
 
+    def set_wps_pbc(self, wpsmode: int = 1, ssidindex: int = 0) -> SetResponseType:
+        return self._session.post_set('wlan/wps-pbc', OrderedDict((
+            ('WPSMode', wpsmode),
+            ('ssidindex', ssidindex),
+        )))
+
     def wps_switch(self) -> GetResponseType:
         return self._session.get('wlan/wps-switch')
 
+    def set_wps_switch(self, appinenable: int) -> SetResponseType:
+        return self._session.post_set('wlan/wps-switch', OrderedDict((
+            ('appinenable', appinenable),
+        )))
+
     def status_switch_settings(self) -> GetResponseType:
         return self._session.get('wlan/status-switch-settings')
 
     def wifiprofile(self) -> GetResponseType:
         """
         Endpoint found by reverse engineering B310s-22 firmware, unknown usage, probably not implemented by Huawei
         :return:
@@ -214,15 +231,15 @@
         :param criteria: dict of key: value
         :return: List[WLanSettings]
         """
         multi_basic_settings = self.multi_basic_settings()
         ssids = map(WLanSettings.from_dict, multi_basic_settings['Ssids']['Ssid'])
         return list(Tools.filter_iter(ssids, criteria))
 
-    def save_wlan_settings(self, settings: List[WLanSettings]) -> SetResponseType:
+    def save_wlan_settings(self, settings: Iterable[WLanSettings]) -> SetResponseType:
         """
         Saves modified list of WLanSettings
         :param settings:
         :return: SetResponseType
         """
         return self.set_multi_basic_settings([item.to_dict() for item in settings])
```

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/api/WebServer.py` & `huawei-lte-api-1.7.3/huawei_lte_api/api/WebServer.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/config/DialUp.py` & `huawei-lte-api-1.7.3/huawei_lte_api/config/DialUp.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/config/Network.py` & `huawei-lte-api-1.7.3/huawei_lte_api/config/Network.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/config/Wifi.py` & `huawei-lte-api-1.7.3/huawei_lte_api/config/Wifi.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/enums/net.py` & `huawei-lte-api-1.7.3/huawei_lte_api/enums/net.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,10 +41,17 @@
 
     ALL = 0x3fffffff
     """Use alone, do not 'or' this with others."""
 
 
 @enum.unique
 class LTEBandEnum(enum.IntEnum):
-    """For other values besides ALL, see set_net_mode docs."""
+    """For other values besides, see set_net_mode docs."""
+    B1 = 0x01
+    B3 = 0x04
+    B7 = 0x40
+    B8 = 0x80
+    B20 = 0x80000
+    B38 = 0x2000000000
+    B40 = 0x8000000000
     ALL = 0x7fffffffffffffff
     """Use alone, do not 'or' this with others."""
```

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api/exceptions.py` & `huawei-lte-api-1.7.3/huawei_lte_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `huawei-lte-api-1.6.9/huawei_lte_api.egg-info/SOURCES.txt` & `huawei-lte-api-1.7.3/huawei_lte_api.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 huawei_lte_api/ApiGroup.py
 huawei_lte_api/AuthorizedConnection.py
@@ -90,14 +91,15 @@
 huawei_lte_api/config/__init__.py
 huawei_lte_api/enums/__init__.py
 huawei_lte_api/enums/client.py
 huawei_lte_api/enums/cradle.py
 huawei_lte_api/enums/device.py
 huawei_lte_api/enums/dialup.py
 huawei_lte_api/enums/net.py
+huawei_lte_api/enums/sdcard.py
 huawei_lte_api/enums/sms.py
 huawei_lte_api/enums/user.py
 huawei_lte_api/enums/wlan.py
 huawei_lte_api/usermanual/PublicSysResources.py
 huawei_lte_api/usermanual/__init__.py
 tests/__init__.py
 tests/test_init.py
```

### Comparing `huawei-lte-api-1.6.9/setup.py` & `huawei-lte-api-1.7.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_readme() -> str:
     with open('README.md', 'r', encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name='huawei-lte-api',
-    version='1.6.9',
+    version='1.7.3',
     packages=find_packages(exclude=['tests', 'tests.*']),
     package_data={'huawei_lte_api': ['py.typed']},
     install_requires=[
         'requests',
         'xmltodict',
         'pycryptodomex'
     ],
@@ -31,19 +31,18 @@
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Topic :: Software Development',
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     project_urls={
         'Release notes': 'https://github.com/Salamek/huawei-lte-api/releases',
     },
 )
```

