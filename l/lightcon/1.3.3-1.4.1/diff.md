# Comparing `tmp/lightcon-1.3.3.tar.gz` & `tmp/lightcon-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightcon-1.3.3.tar", last modified: Mon May 29 15:06:35 2023, max compression
+gzip compressed data, was "lightcon-1.4.1.tar", last modified: Fri Jun 23 12:49:59 2023, max compression
```

## Comparing `lightcon-1.3.3.tar` & `lightcon-1.4.1.tar`

### file list

```diff
@@ -1,79 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.938265 lightcon-1.3.3/
--rw-rw-rw-   0        0        0     1082 2023-05-29 15:04:59.000000 lightcon-1.3.3/LICENCE
--rw-rw-rw-   0        0        0     6247 2023-05-29 15:06:35.938265 lightcon-1.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     5605 2023-05-29 15:04:59.000000 lightcon-1.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.343361 lightcon-1.3.3/lightcon/
--rw-rw-rw-   0        0        0        0 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/__config__.py
--rw-rw-rw-   0        0        0       21 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/_globals.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.358984 lightcon-1.3.3/lightcon/beam_alignment/
--rw-rw-rw-   0        0        0       47 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/beam_alignment/__init__.py
--rw-rw-rw-   0        0        0     2105 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/beam_alignment/beam_alignment.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.358984 lightcon-1.3.3/lightcon/calculate/
--rw-rw-rw-   0        0        0      113 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/calculate/__init__.py
--rw-rw-rw-   0        0        0     2997 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/calculate/beam_profiling_gauss.py
--rw-rw-rw-   0        0        0     3393 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/calculate/beam_profiling_iso.py
--rw-rw-rw-   0        0        0     1407 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/calculate/calculate_motor_parameters.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.358984 lightcon-1.3.3/lightcon/camera_app_client/
--rw-rw-rw-   0        0        0       40 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/camera_app_client/__init__.py
--rw-rw-rw-   0        0        0     2965 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/camera_app_client/camera_app_client.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.358984 lightcon-1.3.3/lightcon/common/
--rw-rw-rw-   0        0        0      324 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/__init__.py
--rw-rw-rw-   0        0        0      931 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/converters.py
--rw-rw-rw-   0        0        0     3155 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/http_methods.py
--rw-rw-rw-   0        0        0     5606 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/leprecan_provider.py
--rw-rw-rw-   0        0        0    20146 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/motor_parameters.py
--rw-rw-rw-   0        0        0     1042 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/serial_tools.py
--rw-rw-rw-   0        0        0      506 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/stage_parameters.py
--rw-rw-rw-   0        0        0     5151 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/common/udp_locator.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.358984 lightcon-1.3.3/lightcon/eth_motor_board/
--rw-rw-rw-   0        0        0       44 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/eth_motor_board/__init__.py
--rw-rw-rw-   0        0        0    15094 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/eth_motor_board/eth_motor_board.py
--rw-rw-rw-   0        0        0     1918 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/eth_motor_board/eth_motor_board_leprecan_provider.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.358984 lightcon-1.3.3/lightcon/fast_daq/
--rw-rw-rw-   0        0        0    70144 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/fast_daq/FTD2XX_NET.dll
--rw-rw-rw-   0        0        0    25088 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/fast_daq/LightConversion.Abstractions.dll
--rw-rw-rw-   0        0        0    23552 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/fast_daq/LightConversion.Hardware.FastDaq.dll
--rw-rw-rw-   0        0        0    29600 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/fast_daq/System.Threading.dll
--rw-rw-rw-   0        0        0       60 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/fast_daq/__init__.py
--rw-rw-rw-   0        0        0     5442 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/fast_daq/fast_daq.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.374611 lightcon-1.3.3/lightcon/harpia/
--rw-rw-rw-   0        0        0      138 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia/__init__.py
--rw-rw-rw-   0        0        0    24801 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia/harpia.py
--rw-rw-rw-   0        0        0     2220 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia/harpia_leprecan_provider.py
--rw-rw-rw-   0        0        0     8813 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia/harpia_model_decoder.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.938265 lightcon-1.3.3/lightcon/harpia_daq/
--rw-rw-rw-   0        0        0    70144 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia_daq/FTD2XX_NET.dll
--rw-rw-rw-   0        0        0    17920 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia_daq/LightConversion.Abstractions.dll
--rw-rw-rw-   0        0        0    26624 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia_daq/LightConversion.Hardware.HarpiaDaq.dll
--rw-rw-rw-   0        0        0    29600 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia_daq/System.Threading.dll
--rw-rw-rw-   0        0        0       40 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia_daq/__init__.py
--rw-rw-rw-   0        0        0     5744 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/harpia_daq/harpia_daq.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.938265 lightcon-1.3.3/lightcon/laser_clients/
--rw-rw-rw-   0        0        0       42 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/laser_clients/__init__.py
--rw-rw-rw-   0        0        0     8633 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/laser_clients/laser_clients.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.938265 lightcon-1.3.3/lightcon/style/
--rw-rw-rw-   0        0        0      100 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/style/__init__.py
--rw-rw-rw-   0        0        0    48590 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/style/lclogo.png
--rw-rw-rw-   0        0        0     4585 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/style/lcstyle.mplstyle
--rw-rw-rw-   0        0        0     7839 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/style/plotstyle_1d.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.938265 lightcon-1.3.3/lightcon/timing_controller/
--rw-rw-rw-   0        0        0      101 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/timing_controller/__init__.py
--rw-rw-rw-   0        0        0     6325 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/timing_controller/timing_controller.py
--rw-rw-rw-   0        0        0     7233 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/timing_controller/timing_controller_v2.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.938265 lightcon-1.3.3/lightcon/wintopas/
--rw-rw-rw-   0        0        0       30 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/wintopas/__init__.py
--rw-rw-rw-   0        0        0     1567 2023-05-29 15:04:59.000000 lightcon-1.3.3/lightcon/wintopas/wintopas.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.358984 lightcon-1.3.3/lightcon.egg-info/
--rw-rw-rw-   0        0        0     6247 2023-05-29 15:06:35.000000 lightcon-1.3.3/lightcon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2105 2023-05-29 15:06:35.000000 lightcon-1.3.3/lightcon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 15:06:35.000000 lightcon-1.3.3/lightcon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-05-29 15:06:35.000000 lightcon-1.3.3/lightcon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-29 15:06:35.000000 lightcon-1.3.3/lightcon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 15:06:35.938265 lightcon-1.3.3/setup.cfg
--rw-rw-rw-   0        0        0     2524 2023-05-29 15:04:59.000000 lightcon-1.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:35.938265 lightcon-1.3.3/tests/
--rw-rw-rw-   0        0        0        0 2023-05-29 15:04:59.000000 lightcon-1.3.3/tests/__init__.py
--rw-rw-rw-   0        0        0      820 2023-05-29 15:04:59.000000 lightcon-1.3.3/tests/test_leprecan_providers.py
--rw-rw-rw-   0        0        0     1444 2023-05-29 15:04:59.000000 lightcon-1.3.3/tests/test_motor_parameters.py
--rw-rw-rw-   0        0        0      105 2023-05-29 15:04:59.000000 lightcon-1.3.3/tests/test_style.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:49:59.820604 lightcon-1.4.1/
+-rw-rw-rw-   0        0        0     1082 2023-06-23 12:47:15.000000 lightcon-1.4.1/LICENCE
+-rw-rw-rw-   0        0        0      249 2023-06-23 12:47:15.000000 lightcon-1.4.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6252 2023-06-23 12:49:59.820604 lightcon-1.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5605 2023-06-23 12:47:15.000000 lightcon-1.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 12:49:59.820604 lightcon-1.4.1/lightcon/
+-rw-rw-rw-   0        0        0        0 2023-06-23 12:47:15.000000 lightcon-1.4.1/lightcon/__config__.py
+-rw-rw-rw-   0        0        0      715 2023-06-23 12:47:15.000000 lightcon-1.4.1/lightcon/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-23 12:47:15.000000 lightcon-1.4.1/lightcon/_globals.py
+drwxrwxrwx   0        0        0        0 2023-06-23 12:49:59.820604 lightcon-1.4.1/lightcon/datasets/
+drwxrwxrwx   0        0        0        0 2023-06-23 12:49:59.820604 lightcon-1.4.1/lightcon/datasets/data/
+-rw-rw-rw-   0        0        0    11967 2023-06-23 12:49:16.000000 lightcon-1.4.1/lightcon/datasets/data/motor_parameters.json
+-rw-rw-rw-   0        0        0     3335 2023-06-23 12:49:16.000000 lightcon-1.4.1/lightcon/datasets/data/stage_parameters.json
+drwxrwxrwx   0        0        0        0 2023-06-23 12:49:59.820604 lightcon-1.4.1/lightcon.egg-info/
+-rw-rw-rw-   0        0        0     6252 2023-06-23 12:49:59.000000 lightcon-1.4.1/lightcon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-06-23 12:49:59.000000 lightcon-1.4.1/lightcon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 12:49:59.000000 lightcon-1.4.1/lightcon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-23 12:49:59.000000 lightcon-1.4.1/lightcon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 12:49:59.000000 lightcon-1.4.1/lightcon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 12:49:59.820604 lightcon-1.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1744 2023-06-23 12:47:15.000000 lightcon-1.4.1/setup.py
```

### Comparing `lightcon-1.3.3/LICENCE` & `lightcon-1.4.1/LICENCE`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.3/PKG-INFO` & `lightcon-1.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: lightcon
-Version: 1.3.3
+Version: 1.4.1
 Summary: A set of APIs to Light Conversion devices
 Home-page: https://bitbucket.org/harpiasoftware/light-conversion-apis.git
 Author: Vytautas Butkus
 Author-email: vytautas.butkus@lightcon.com
-Project-URL: Examples, https://bitbucket.org/harpiasoftware/light-conversion-apis/src/master/examples/
+Project-URL: Documentation, https://lightconupdater.blob.core.windows.net/documentation/lightcon/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `lightcon-1.3.3/README.md` & `lightcon-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `lightcon-1.3.3/lightcon.egg-info/PKG-INFO` & `lightcon-1.4.1/lightcon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: lightcon
-Version: 1.3.3
+Version: 1.4.1
 Summary: A set of APIs to Light Conversion devices
 Home-page: https://bitbucket.org/harpiasoftware/light-conversion-apis.git
 Author: Vytautas Butkus
 Author-email: vytautas.butkus@lightcon.com
-Project-URL: Examples, https://bitbucket.org/harpiasoftware/light-conversion-apis/src/master/examples/
+Project-URL: Documentation, https://lightconupdater.blob.core.windows.net/documentation/lightcon/index.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

