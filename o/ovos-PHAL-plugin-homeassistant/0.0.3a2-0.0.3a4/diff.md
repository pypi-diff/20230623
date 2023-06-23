# Comparing `tmp/ovos-PHAL-plugin-homeassistant-0.0.3a2.tar.gz` & `tmp/ovos-PHAL-plugin-homeassistant-0.0.3a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.3a2.tar", last modified: Tue Jun 20 16:52:42 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-homeassistant-0.0.3a4.tar", last modified: Fri Jun 23 15:59:18 2023, max compression
```

## Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2.tar` & `ovos-PHAL-plugin-homeassistant-0.0.3a4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.333889 ovos-PHAL-plugin-homeassistant-0.0.3a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-20 16:52:42.333889 ovos-PHAL-plugin-homeassistant-0.0.3a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5626 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.321889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/
--rw-r--r--   0 runner    (1001) docker     (123)    35956 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.325889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/
--rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    28135 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/socketclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.325889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.325889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/
--rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml
--rw-r--r--   0 runner    (1001) docker     (123)    28521 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml
--rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.325889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/code/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/code/helper.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.329889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.329889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/delegates/
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.329889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.333889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:scene.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.325889 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-20 16:52:42.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-20 16:52:42.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:52:42.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 16:52:42.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-20 16:52:42.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-20 16:52:42.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:52:42.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.321889 ovos-PHAL-plugin-homeassistant-0.0.3a2/res/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.333889 ovos-PHAL-plugin-homeassistant-0.0.3a2/res/desktop/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/res/desktop/ovos-phal-homeassistant.desktop
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:52:42.333889 ovos-PHAL-plugin-homeassistant-0.0.3a2/res/icon/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/res/icon/ovos-phal-homeassistant.svg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:52:42.333889 ovos-PHAL-plugin-homeassistant-0.0.3a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-20 16:52:41.000000 ovos-PHAL-plugin-homeassistant-0.0.3a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:18.331025 ovos-PHAL-plugin-homeassistant-0.0.3a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-23 15:59:18.331025 ovos-PHAL-plugin-homeassistant-0.0.3a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:18.323025 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/
+-rw-r--r--   0 runner    (1001) docker     (123)    36273 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:18.327025 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)    15253 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/logic/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28135 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/logic/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/logic/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/logic/socketclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/logic/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:18.327025 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:18.327025 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/
+-rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     9896 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    28521 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    10880 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:18.327025 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/code/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/code/helper.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:18.327025 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:18.327025 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/delegates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:18.327025 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4357 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:18.331025 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:scene.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:18.327025 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-06-23 15:59:18.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-06-23 15:59:18.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:59:18.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-23 15:59:18.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-23 15:59:18.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-23 15:59:18.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 15:59:18.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:18.323025 ovos-PHAL-plugin-homeassistant-0.0.3a4/res/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:18.331025 ovos-PHAL-plugin-homeassistant-0.0.3a4/res/desktop/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/res/desktop/ovos-phal-homeassistant.desktop
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:59:18.331025 ovos-PHAL-plugin-homeassistant-0.0.3a4/res/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/res/icon/ovos-phal-homeassistant.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:59:18.331025 ovos-PHAL-plugin-homeassistant-0.0.3a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-23 15:59:14.000000 ovos-PHAL-plugin-homeassistant-0.0.3a4/setup.py
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/LICENSE` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/README.md` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,99 +1,114 @@
 # OVOS PHAL Home Assistant Plugin
 
 The PHAL Plugin provides GUI interfaces and API for Home Assistant Instants.
 
 NOTE: this plugin is roadmapped for merging with https://github.com/OpenVoiceOS/ovos-PHAL-plugin-commonIOT for ovos-core release 0.0.9, the UI will become IOT framework agnostic
 
 # Demo GIF
+
 ![HomeAssistant PHAL Demo](demo/demo.gif)
 
 ### Installation
 
 Plugin Support Two Installation Methods:
+
 1. Install from Github URL
 
 Note: PIP install from URL will not install the .desktop file and icon if installing to a venv or virtual environment, so you need to manually install them to the system or user directory.
 
 Note: PIP install will attempt to install the .desktop file and icon to the system directory, or user directory if the system directory is not writable. If this is not a virtual environemnt.
 
 ```bash
 pip install git+https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 ```
 
 2. Manual Install from Git Clone
+
 ```bash
 git clone https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant
 cd ovos-PHAL-plugin-homeassistant
 cp -r res/desktop/ovos-phal-homeassistant.desktop ~/.local/share/applications/
 cp -r res/icon/ovos-phal-homeassistant.png ~/.local/share/icons/
 pip install .
 ```
 
 ### Configuration (Instance Setup)
 
 Plugin Supports Two Configuration Methods:
+
 1. Using the GUI
+
    - Install the plugin
    - Open the application from the homescreen menu
    - Click the "Connect Instance" button
    - Enter the URL of the Home Assistant Instance
    - Enter the Long-Lived Access Token (API KEY)
-   - Press the "Confirm" button 
+   - Press the "Confirm" button
 
 2. Manually Editing the Config File
    - Add the following to the config file:
    ```json
         "PHAL": {
             "ovos-PHAL-plugin-homeassistant": {
                 "host": "https://someurl.toinstance",
                 "api_key": "api key from the instance"
             }
         }
    ```
 
-The config also takes an optional property, `brightness_increment`, which is the amount to increment/decrement the brightness of a light when the brightness up/down commands are sent. The default value is 10 and represents a percentage, e.g. 10%.
+The config also takes some optional properties:
+
+`brightness_increment` - the amount to increment/decrement the brightness of a light when the brightness up/down commands are sent. The default value is 10 and represents a percentage, e.g. 10%.
+`search_confidence_threshold` - the confidence threshold for the search skill to use when searching for devices. The default value is 0.5, or 50%. Must be a value between 0 and 1.
 
 Sample config:
 
 ```json
         "PHAL": {
             "ovos-PHAL-plugin-homeassistant": {
                 "host": "https://someurl.toinstance",
                 "api_key": "api key from the instance",
-                "brightness_increment": 5
+                "brightness_increment": 5,
+                "search_confidence_threshold": 0.6
             }
         }
 ```
 
 ### Usage
 
 The plugin provides a GUI interface for Home Assistant Instances. It also provides an API for other plugins or skills to user.
 
 The plugin is in early development, so there are some features that are not yet implemented. It currently supports the following entities:
+
 - Media Player
 - Light
 - Vacuum
 - Binary Sensor
 - Sensor
 
----------------------------------------  
+---
+
 #### BUS API (For Other Plugins / GUIs) - WIP / TODO Documentation
+
 #### EXPANDING DEVICE / ENTITY SUPPORT - WIP / TODO Documentation
----------------------------------------
+
+---
 
 ## Technical Documentation
 
 ### Python Controller Class Specification:
+
 Depending on how the controller communicates with the host instance, the minimum required connector initialization properties are:
 
 - **host** (type: string): Address to host instance
 - **api_key** (type: string): Access key for host instance authentication
 
 ### Python Device Class Specification:
+
 All devices are required to support the below minimal properties for device initialization.
 
 - **controller** (type: string): An instance of the controller class that handles all communications with the API the device talks to for example HomeAssistantConnector, All devices will use the controller class for any kind of communication.
 - **device_id** (type: string): A device id to associate all communications with this device with, for HomeAssistant device_id = entity_id, all device_id start with device_type.device_name.
 - **device_icon** (type: string): A device icon to associate the device display icon with including type, for example: "mdi:light" for device type light, "mdi:sensor" for device type sensor, "mdi:media_player" for device type media_player
 - **device_name** (type: string): A human readable device name that can be used for spoken and visual material
 - **device_state** (type: string): A device can have multiple states depending on which type of device it is, for example a light can have an "on", "off" and "unavailable" states, a media_player can have "playing", "paused", "off", "on" and "unavailable" states. Refer to HomeAssistant entities list for complete list of entity states
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/__init__.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,23 @@
         """ Get the brightness increment from the config
 
             Returns:
                 int: The brightness increment
         """
         return self.config.get("brightness_increment", 10)
 
+    @property
+    def search_confidence_threshold(self) -> int:
+        """ Get the search confidence threshold from the config
+
+            Returns:
+                int: The search confidence threshold value, default 0.5
+        """
+        return self.config.get("search_confidence_threshold", 0.5)
+
 # SETUP INSTANCE SUPPORT
     def validate_instance_connection(self, host, api_key):
         """ Validate the connection to the Home Assistant instance
 
             Args:
                 host (str): The Home Assistant instance URL
                 api_key (str): The Home Assistant API key
@@ -560,15 +569,15 @@
 
         Args:
             message (Message): The message object
         """
         device_id, spoken_device = self._gather_device_id(message)
         for device in self.registered_devices:
             if device.device_id == device_id:
-                brightness = device.decrease_brightness(self.brightness_increment)
+                device.decrease_brightness(self.brightness_increment)
                 return self.bus.emit(message.response(data={
                     "device": spoken_device,
                     "brightness": get_percentage_brightness_from_ha_value(device.get_brightness())
                     }))
         response = "Device id not provided"
         LOG.error(response)
         return self.bus.emit(message.response(data={"device": spoken_device, "response": response}))
@@ -821,13 +830,13 @@
 
 # UTILS
     def fuzzy_match_name(self, devices_list, spoken_name, device_names) -> Optional[str]:
         """Given a list of device names, fuzzy match the spoken name to the most likely one.
         Returns the device id of the most likely match or None if no match is found.
         """
         device, score = match_one(spoken_name, device_names)
-        if score > 0.75:
+        if score > self.search_confidence_threshold:
             return devices_list[device_names.index(device)].device_id
         else:
             LOG.info(f"Device name '{spoken_name}' not found, closest match is '{device}' with confidence score {score}")
             LOG.info(f"Score of {score} is too low, returning None")
             return None
```

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/connector.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/logic/connector.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/device.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/logic/device.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/integration.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/logic/integration.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/socketclient.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/logic/socketclient.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/logic/utils.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/logic/utils.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/Dashboard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/+mediacenter/InstanceSetup.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/Dashboard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/DeviceControlsLoader.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/InstanceGridButton.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/InstanceSetup.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/InstanceSetupFooterButtons.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/code/helper.js` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/code/helper.js`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/AutomationCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/BinarySensorCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/CameraCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/CircleSensorItemPercentType.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/LightCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/MediaPlayerCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/PowerSensorItemType.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/SceneCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/SensorCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/SwitchCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/dashcards/VacuumCard.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/delegates/DashboardDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/delegates/DeviceDashboardDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/ColorPickerControl.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightBrightness.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightColor.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LightDeviceStateButton.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaControl.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/devicecontrols/LocalMediaDelegate.qml`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-off.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/bulb-on.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_dark.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/ha_icon_light.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:automation.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:binary_sensor.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:camera.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:climate.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:grouped.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:light.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:media_player.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:sensor.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:switch.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:ungrouped.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/mdi:vacuum.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/power.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/qr-mobile.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant/ui/icons/token-device.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/ovos_PHAL_plugin_homeassistant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/res/icon/ovos-phal-homeassistant.svg` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/res/icon/ovos-phal-homeassistant.svg`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-homeassistant-0.0.3a2/setup.py` & `ovos-PHAL-plugin-homeassistant-0.0.3a4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 import os
 from setuptools import setup
 
 BASEDIR = os.path.abspath(os.path.dirname(__file__))
 
+
 def get_version():
     """ Find the version of the package"""
     version = None
     version_file = os.path.join(BASEDIR, 'ovos_PHAL_plugin_homeassistant', 'version.py')
     major, minor, build, alpha = (None, None, None, None)
     with open(version_file) as f:
         for line in f:
@@ -24,46 +25,56 @@
                     '# END_VERSION_BLOCK' in line):
                 break
     version = f"{major}.{minor}.{build}"
     if alpha and int(alpha) > 0:
         version += f"a{alpha}"
     return version
 
+
 def required(requirements_file):
     """ Read requirements file and remove comments and empty lines. """
     with open(os.path.join(BASEDIR, requirements_file), 'r') as f:
         requirements = f.read().splitlines()
         if 'MYCROFT_LOOSE_REQUIREMENTS' in os.environ:
             print('USING LOOSE REQUIREMENTS!')
             requirements = [r.replace('==', '>=').replace('~=', '>=') for r in requirements]
         return [pkg for pkg in requirements
                 if pkg.strip() and not pkg.startswith("#")]
 
+
 def package_files(directory):
     paths = []
     for (path, directories, filenames) in os.walk(directory):
         for filename in filenames:
             paths.append(os.path.join('..', path, filename))
     return paths
 
+
+def get_description():
+    with open(os.path.join(BASEDIR, "README.md"), "r") as f:
+        long_description = f.read()
+    return long_description
+
 PLUGIN_ENTRY_POINT = 'ovos-PHAL-plugin-homeassistant=ovos_PHAL_plugin_homeassistant:HomeAssistantPlugin'
 setup(
     name='ovos-PHAL-plugin-homeassistant',
     version=get_version(),
-    description='Notifications and Widgets plugin for OpenVoiceOS hardware abstraction layer',
+    description='Homeassistant PHAL plugin for OpenVoiceOS',
+    long_description=get_description(),
+    long_description_content_type="text/markdown",
     url='https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant',
     author='Aiix',
     author_email='aix.m@outlook.com',
     license='Apache-2.0',
     packages=['ovos_PHAL_plugin_homeassistant'],
     package_data={'': package_files('ovos_PHAL_plugin_homeassistant')},
     install_requires=required("requirements.txt"),
     zip_safe=True,
     include_package_data=True,
-    data_files = [
+    data_files=[
         ('share/applications', ['res/desktop/ovos-phal-homeassistant.desktop']),
         ('share/icons', ['res/icon/ovos-phal-homeassistant.svg'])
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Topic :: Utilities',
```

