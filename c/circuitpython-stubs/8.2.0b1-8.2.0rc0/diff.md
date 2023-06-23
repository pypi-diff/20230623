# Comparing `tmp/circuitpython-stubs-8.2.0b1.tar.gz` & `tmp/circuitpython-stubs-8.2.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-stubs-8.2.0b1.tar", last modified: Thu Jun  8 18:53:00 2023, max compression
+gzip compressed data, was "circuitpython-stubs-8.2.0rc0.tar", last modified: Fri Jun 23 18:32:31 2023, max compression
```

## Comparing `circuitpython-stubs-8.2.0b1.tar` & `circuitpython-stubs-8.2.0rc0.tar`

### file list

```diff
@@ -1,232 +1,232 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.273276 circuitpython-stubs-8.2.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 18:52:52.000000 circuitpython-stubs-8.2.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-08 18:53:00.273276 circuitpython-stubs-8.2.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-08 18:52:52.000000 circuitpython-stubs-8.2.0b1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.257275 circuitpython-stubs-8.2.0b1/_bleio/
--rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/_bleio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.257275 circuitpython-stubs-8.2.0b1/_eve/
--rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/_eve/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.257275 circuitpython-stubs-8.2.0b1/_pew/
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/_pew/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.257275 circuitpython-stubs-8.2.0b1/_pixelmap/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/_pixelmap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.257275 circuitpython-stubs-8.2.0b1/_stage/
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/_stage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/adafruit_bus_device/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/adafruit_bus_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/adafruit_bus_device/i2c_device/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/adafruit_bus_device/i2c_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/adafruit_bus_device/spi_device/
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/adafruit_bus_device/spi_device/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/adafruit_pixelbuf/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/adafruit_pixelbuf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/aesio/
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/aesio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/alarm/
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/alarm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/alarm/pin/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/alarm/pin/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/alarm/time/
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/alarm/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/alarm/touch/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/alarm/touch/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/analogbufio/
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/analogbufio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/analogio/
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/analogio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/atexit/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/atexit/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/audiobusio/
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/audiobusio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/audiocore/
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/audiocore/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/audioio/
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/audioio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/audiomixer/
--rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/audiomixer/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/audiomp3/
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/audiomp3/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/audiopwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/audiopwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/bitbangio/
--rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/bitbangio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/bitmaptools/
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/bitmaptools/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/bitops/
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/bitops/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/board/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/board/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/busio/
--rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/busio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/camera/
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/camera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/canio/
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/canio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.273276 circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-08 18:52:59.000000 circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-08 18:53:00.000000 circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:52:59.000000 circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:52:59.000000 circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-08 18:52:59.000000 circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/countio/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-08 18:52:49.000000 circuitpython-stubs-8.2.0b1/countio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/cyw43/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-08 18:52:52.000000 circuitpython-stubs-8.2.0b1/cyw43/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/digitalio/
--rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/digitalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/displayio/
--rw-r--r--   0 runner    (1001) docker     (123)    40379 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/displayio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/dualbank/
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/dualbank/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/espcamera/
--rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/espcamera/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/espidf/
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/espidf/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/espnow/
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/espnow/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/espulp/
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/espulp/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/floppyio/
--rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/floppyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.261276 circuitpython-stubs-8.2.0b1/fontio/
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/fontio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/framebufferio/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/framebufferio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/frequencyio/
--rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/frequencyio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/getpass/
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/getpass/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/gifio/
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/gifio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/gnss/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/gnss/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/hashlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/hashlib/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/i2ctarget/
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/i2ctarget/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/imagecapture/
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/imagecapture/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/ipaddress/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/ipaddress/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/is31fl3741/
--rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/is31fl3741/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/keypad/
--rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/keypad/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/math/
--rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/math/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/mdns/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/mdns/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/memorymap/
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/memorymap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/memorymonitor/
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/memorymonitor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/microcontroller/
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/microcontroller/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/msgpack/
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/msgpack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/neopixel_write/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/neopixel_write/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/nvm/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/nvm/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/onewireio/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/onewireio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/os/
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/os/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/paralleldisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/paralleldisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/picodvi/
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-08 18:52:52.000000 circuitpython-stubs-8.2.0b1/picodvi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/ps2io/
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/ps2io/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/pulseio/
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/pulseio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/pwmio/
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/pwmio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/qrio/
--rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/qrio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/rainbowio/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/rainbowio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/random/
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/random/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/rgbmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/rgbmatrix/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/rotaryio/
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/rotaryio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/rp2pio/
--rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-06-08 18:52:52.000000 circuitpython-stubs-8.2.0b1/rp2pio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/rtc/
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/rtc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/samd/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/samd/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/sdcardio/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/sdcardio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/sdioio/
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/sdioio/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:53:00.273276 circuitpython-stubs-8.2.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-08 18:52:52.000000 circuitpython-stubs-8.2.0b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/sharpdisplay/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/sharpdisplay/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.265276 circuitpython-stubs-8.2.0b1/socketpool/
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/socketpool/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ssl/
--rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/ssl/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/storage/
--rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/storage/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/struct/
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/struct/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/supervisor/
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/supervisor/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/synthio/
--rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/synthio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/terminalio/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/terminalio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/time/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/time/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/touchio/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/touchio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/traceback/
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/traceback/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/uheap/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/uheap/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/numpy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/numpy/carray/
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/numpy/carray/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/numpy/fft/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/numpy/fft/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/numpy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/numpy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/scipy/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/scipy/linalg/
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/scipy/linalg/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/scipy/optimize/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/scipy/optimize/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/user/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/user/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ulab/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/ulab/utils/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/usb/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/usb/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/usb/core/
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/usb/core/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/usb_cdc/
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/usb_cdc/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/usb_hid/
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/usb_hid/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/usb_host/
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/usb_host/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/usb_midi/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/usb_midi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/ustack/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/ustack/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/vectorio/
--rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/vectorio/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/watchdog/
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-08 18:52:50.000000 circuitpython-stubs-8.2.0b1/watchdog/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/wifi/
--rw-r--r--   0 runner    (1001) docker     (123)    10390 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/wifi/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:53:00.269276 circuitpython-stubs-8.2.0b1/zlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-08 18:52:51.000000 circuitpython-stubs-8.2.0b1/zlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.574568 circuitpython-stubs-8.2.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-23 18:32:23.000000 circuitpython-stubs-8.2.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-23 18:32:31.574568 circuitpython-stubs-8.2.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-23 18:32:23.000000 circuitpython-stubs-8.2.0rc0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/_bleio/
+-rw-r--r--   0 runner    (1001) docker     (123)    31094 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/_bleio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/_eve/
+-rw-r--r--   0 runner    (1001) docker     (123)    20379 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/_eve/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/_pew/
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/_pew/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/_pixelmap/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/_pixelmap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/_stage/
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/_stage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/adafruit_bus_device/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/adafruit_bus_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/adafruit_bus_device/i2c_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/adafruit_bus_device/i2c_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/adafruit_bus_device/spi_device/
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/adafruit_bus_device/spi_device/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/adafruit_pixelbuf/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/adafruit_pixelbuf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/aesio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/aesio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/alarm/
+-rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/alarm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/alarm/pin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/alarm/pin/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/alarm/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/alarm/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/alarm/touch/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/alarm/touch/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/analogbufio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/analogbufio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.558568 circuitpython-stubs-8.2.0rc0/analogio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/analogio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/atexit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/atexit/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/audiobusio/
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/audiobusio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/audiocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/audiocore/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/audioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/audioio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/audiomixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4424 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/audiomixer/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/audiomp3/
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/audiomp3/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/audiopwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/audiopwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/bitbangio/
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/bitbangio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/bitmaptools/
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/bitmaptools/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/bitops/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/bitops/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/board/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/board/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/busio/
+-rw-r--r--   0 runner    (1001) docker     (123)    20025 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/busio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/camera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/canio/
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/canio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.574568 circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-06-23 18:32:30.000000 circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5148 2023-06-23 18:32:31.000000 circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:32:30.000000 circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:32:30.000000 circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-23 18:32:30.000000 circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/countio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/countio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/cyw43/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-06-23 18:32:23.000000 circuitpython-stubs-8.2.0rc0/cyw43/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/digitalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5162 2023-06-23 18:32:20.000000 circuitpython-stubs-8.2.0rc0/digitalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/displayio/
+-rw-r--r--   0 runner    (1001) docker     (123)    40379 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/displayio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/dualbank/
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/dualbank/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/espcamera/
+-rw-r--r--   0 runner    (1001) docker     (123)    11830 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/espcamera/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/espidf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/espidf/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/espnow/
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/espnow/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/espulp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/espulp/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/floppyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/floppyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/fontio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/fontio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/framebufferio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/framebufferio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/frequencyio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3461 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/frequencyio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/getpass/
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/getpass/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/gifio/
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/gifio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/gnss/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/gnss/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/hashlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/hashlib/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/i2ctarget/
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/i2ctarget/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.562568 circuitpython-stubs-8.2.0rc0/imagecapture/
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/imagecapture/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/ipaddress/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/ipaddress/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/is31fl3741/
+-rw-r--r--   0 runner    (1001) docker     (123)     3873 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/is31fl3741/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/keypad/
+-rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/keypad/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     4805 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/math/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/mdns/
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/mdns/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/memorymap/
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/memorymap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/memorymonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/memorymonitor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/microcontroller/
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/microcontroller/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/msgpack/
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/msgpack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/neopixel_write/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/neopixel_write/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/nvm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/nvm/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/onewireio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/onewireio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/os/
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/os/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/paralleldisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/paralleldisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/picodvi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-23 18:32:23.000000 circuitpython-stubs-8.2.0rc0/picodvi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/ps2io/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/ps2io/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/pulseio/
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/pulseio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/pwmio/
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/pwmio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/qrio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/qrio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/rainbowio/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/rainbowio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/random/
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/random/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/rgbmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/rgbmatrix/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/rotaryio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/rotaryio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/rp2pio/
+-rw-r--r--   0 runner    (1001) docker     (123)    16742 2023-06-23 18:32:23.000000 circuitpython-stubs-8.2.0rc0/rp2pio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/rtc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/rtc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/samd/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/samd/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/sdcardio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/sdcardio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/sdioio/
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/sdioio/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 18:32:31.574568 circuitpython-stubs-8.2.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-23 18:32:23.000000 circuitpython-stubs-8.2.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/sharpdisplay/
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/sharpdisplay/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/socketpool/
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/socketpool/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/ssl/
+-rw-r--r--   0 runner    (1001) docker     (123)     4567 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/ssl/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/storage/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.566568 circuitpython-stubs-8.2.0rc0/struct/
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/struct/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/supervisor/
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/supervisor/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/synthio/
+-rw-r--r--   0 runner    (1001) docker     (123)    22728 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/synthio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/terminalio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/terminalio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/time/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/time/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/touchio/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/touchio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/traceback/
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/traceback/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/uheap/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/uheap/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)    15556 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/numpy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/numpy/carray/
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/numpy/carray/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/numpy/fft/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/numpy/fft/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/numpy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/numpy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/scipy/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/scipy/linalg/
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/scipy/linalg/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/scipy/optimize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/scipy/optimize/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/user/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ulab/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/ulab/utils/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/usb/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/usb/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/usb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/usb/core/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/usb_cdc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/usb_cdc/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/usb_hid/
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/usb_hid/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/usb_host/
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/usb_host/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/usb_midi/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/usb_midi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/ustack/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/ustack/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/vectorio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4828 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/vectorio/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/watchdog/
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-06-23 18:32:21.000000 circuitpython-stubs-8.2.0rc0/watchdog/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/wifi/
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/wifi/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:32:31.570568 circuitpython-stubs-8.2.0rc0/zlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-23 18:32:22.000000 circuitpython-stubs-8.2.0rc0/zlib/__init__.pyi
```

### Comparing `circuitpython-stubs-8.2.0b1/README.rst` & `circuitpython-stubs-8.2.0rc0/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/_bleio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/_bleio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/_eve/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/_eve/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/_pew/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/_pew/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/_pixelmap/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/_pixelmap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/_stage/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/_stage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/adafruit_bus_device/i2c_device/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/adafruit_bus_device/i2c_device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/adafruit_bus_device/spi_device/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/adafruit_bus_device/spi_device/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/adafruit_pixelbuf/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/adafruit_pixelbuf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/aesio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/aesio/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                                                         for CBC or CTR mode"""
         ...
     def encrypt_into(self, src: ReadableBuffer, dest: WriteableBuffer) -> None:
         """Encrypt the buffer from ``src`` into ``dest``.
 
         For ECB mode, the buffers must be 16 bytes long.  For CBC mode, the
         buffers must be a multiple of 16 bytes, and must be equal length.  For
-        CTX mode, there are no restrictions."""
+        CTR mode, there are no restrictions."""
         ...
     def decrypt_into(self, src: ReadableBuffer, dest: WriteableBuffer) -> None:
         """Decrypt the buffer from ``src`` into ``dest``.
         For ECB mode, the buffers must be 16 bytes long.  For CBC mode, the
         buffers must be a multiple of 16 bytes, and must be equal length.  For
-        CTX mode, there are no restrictions."""
+        CTR mode, there are no restrictions."""
         ...
```

### Comparing `circuitpython-stubs-8.2.0b1/alarm/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/alarm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/alarm/pin/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/alarm/pin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/alarm/time/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/alarm/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/alarm/touch/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/alarm/touch/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/analogbufio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/analogbufio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/analogio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/analogio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/atexit/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/atexit/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/audiobusio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/audiobusio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/audiocore/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/audiocore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/audioio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/audioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/audiomixer/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/audiomixer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/audiomp3/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/audiomp3/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/audiopwmio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/audiopwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/bitbangio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/bitbangio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/bitmaptools/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/bitmaptools/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/bitops/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/bitops/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/board/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/board/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/busio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/busio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/camera/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/camera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/canio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/canio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/SOURCES.txt` & `circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/circuitpython_stubs.egg-info/top_level.txt` & `circuitpython-stubs-8.2.0rc0/circuitpython_stubs.egg-info/top_level.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/countio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/countio/__init__.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -63,14 +63,18 @@
             # Count rising edges only.
             pin_counter = countio.Counter(board.D1, edge=countio.Edge.RISE)
             # Reset the count after 100 counts.
             while True:
                 if pin_counter.count >= 100:
                     pin_counter.reset()
                 print(pin_counter.count)
+
+        **Limitations:** On RP2040, `Counter` uses the PWM peripheral, and
+        is limited to using PWM channel B pins due to hardware restrictions.
+        See the pin assignments for your board to see which pins can be used.
         """
         ...
     def deinit(self) -> None:
         """Deinitializes the Counter and releases any hardware resources for reuse."""
     def __enter__(self) -> Counter:
         """No-op used by Context Managers."""
     def __exit__(self) -> None:
```

### Comparing `circuitpython-stubs-8.2.0b1/cyw43/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/cyw43/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/digitalio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/digitalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/displayio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/displayio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/dualbank/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/dualbank/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/espcamera/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/espcamera/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/espidf/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/espidf/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/espnow/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/espnow/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/espulp/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/espulp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/floppyio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/floppyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/fontio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/fontio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/framebufferio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/framebufferio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/frequencyio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/frequencyio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/getpass/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/getpass/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/gifio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/gifio/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -122,14 +122,20 @@
 
     def __init__(self, file: str) -> None:
         """Create an `OnDiskGif` object with the given file.
         The GIF frames are decoded into RGB565 big-endian format.
         `displayio` expects little-endian, so the example above uses `Colorspace.RGB565_SWAPPED`.
 
         :param file file: The name of the GIF file.
+
+        If the image is too large it will be cropped at the bottom and right when displayed.
+
+        **Limitations**: The image width is limited to 320 pixels at present. `ValueError`
+        will be raised if the image is too wide. The height
+        is not limited but images that are too large will cause a memory exception.
         """
         ...
     def __enter__(self) -> OnDiskGif:
         """No-op used by Context Managers."""
         ...
     def __exit__(self) -> None:
         """Automatically deinitializes the GIF when exiting a context. See
```

### Comparing `circuitpython-stubs-8.2.0b1/gnss/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/gnss/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/hashlib/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/hashlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/i2ctarget/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/i2ctarget/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/imagecapture/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/imagecapture/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/ipaddress/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/ipaddress/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/is31fl3741/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/is31fl3741/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/keypad/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/keypad/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/math/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/math/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/mdns/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/mdns/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/memorymap/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/memorymap/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/memorymonitor/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/memorymonitor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/microcontroller/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/microcontroller/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/msgpack/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/msgpack/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/neopixel_write/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/neopixel_write/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/nvm/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/nvm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/onewireio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/onewireio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/os/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/os/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/paralleldisplay/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/paralleldisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/picodvi/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/picodvi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/ps2io/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/ps2io/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/pulseio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/pulseio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/pwmio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/pwmio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/qrio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/qrio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/random/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/random/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/rgbmatrix/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/rgbmatrix/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/rotaryio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/rotaryio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/rp2pio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/rp2pio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/rtc/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/rtc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/samd/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/samd/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/sdcardio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/sdcardio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/sdioio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/sdioio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/setup.py` & `circuitpython-stubs-8.2.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/sharpdisplay/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/sharpdisplay/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/socketpool/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/socketpool/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/ssl/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/ssl/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/storage/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/struct/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/struct/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/supervisor/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/supervisor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/synthio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/synthio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/terminalio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/terminalio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/time/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/time/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/touchio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/touchio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/traceback/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/traceback/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/ulab/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/ulab/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/ulab/numpy/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/ulab/numpy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/ulab/numpy/carray/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/ulab/numpy/carray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/ulab/numpy/fft/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/ulab/numpy/fft/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/ulab/numpy/linalg/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/ulab/numpy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/ulab/scipy/linalg/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/ulab/scipy/linalg/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/ulab/scipy/optimize/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/ulab/scipy/optimize/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/usb/core/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/usb/core/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/usb_cdc/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/usb_cdc/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/usb_hid/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/usb_hid/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/usb_host/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/usb_host/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/usb_midi/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/usb_midi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/vectorio/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/vectorio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/watchdog/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/watchdog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `circuitpython-stubs-8.2.0b1/wifi/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/wifi/__init__.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -153,27 +153,32 @@
         ...
     def start_ap(
         self,
         ssid: Union[str | ReadableBuffer],
         password: Union[str | ReadableBuffer] = b"",
         *,
         channel: int = 1,
-        authmode: Optional[AuthMode] = None,
+        authmode: Iterable[AuthMode] = (),
         max_connections: Optional[int] = 4,
     ) -> None:
         """Starts running an access point with the specified ssid and password.
 
         If ``channel`` is given, the access point will use that channel unless
         a station is already operating on a different channel.
 
-        If ``authmode`` is not None, the access point will use that Authentication
-        mode. If a non-empty password is given, ``authmode`` must not be ``OPEN``.
-        If ``authmode`` is not given or is None,
-        ``OPEN`` will be used when the password is the empty string,
-        otherwise ``authmode`` will be ``WPA_WPA2_PSK``.
+        If ``authmode`` is not None, the access point will use the given authentication modes.
+        If a non-empty password is given, ``authmode`` must not include ``OPEN``.
+        If ``authmode`` is not given or is an empty iterable,
+        ``(wifi.AuthMode.OPEN,)`` will be used when the password is the empty string,
+        otherwise ``authmode`` will be ``(wifi.AuthMode.WPA, wifi.AuthMode.WPA2, wifi.AuthMode.PSK)``.
+
+        **Limitations:** On Espressif, ``authmode`` with a non-empty password must include
+        `wifi.AuthMode.PSK`, and one or both of `wifi.AuthMode.WPA` and `wifi.AuthMode.WPA2`.
+        On Pi Pico W, ``authmode`` is ignored; it is always ``(wifi.AuthMode.WPA2, wifi.AuthMode.PSK)`
+        with a non-empty password, or ``(wifi.AuthMode.OPEN,)`` when no password is given.
 
         The length of ``password`` must be 8-63 characters if it is ASCII,
         or exactly 64 hexadecimal characters if it is the hex form of the 256-bit key.
 
         If ``max_connections`` is given, the access point will allow up to
         that number of stations to connect."""
         ...
```

### Comparing `circuitpython-stubs-8.2.0b1/zlib/__init__.pyi` & `circuitpython-stubs-8.2.0rc0/zlib/__init__.pyi`

 * *Files identical despite different names*

