# Comparing `tmp/BoxKit-2023.6.tar.gz` & `tmp/BoxKit-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BoxKit-2023.6.tar", last modified: Fri Jun 23 17:36:11 2023, max compression
+gzip compressed data, was "BoxKit-3.0.tar", last modified: Thu Dec  8 16:50:54 2022, max compression
```

## Comparing `BoxKit-2023.6.tar` & `BoxKit-3.0.tar`

### file list

```diff
@@ -1,102 +1,105 @@
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.519286 BoxKit-2023.6/
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.515286 BoxKit-2023.6/BoxKit.egg-info/
--rw-rw-r--   0 akash     (1001) akash     (1001)     8416 2023-06-23 17:36:11.000000 BoxKit-2023.6/BoxKit.egg-info/PKG-INFO
--rw-rw-r--   0 akash     (1001) akash     (1001)     2617 2023-06-23 17:36:11.000000 BoxKit-2023.6/BoxKit.egg-info/SOURCES.txt
--rw-rw-r--   0 akash     (1001) akash     (1001)        1 2023-06-23 17:36:11.000000 BoxKit-2023.6/BoxKit.egg-info/dependency_links.txt
--rw-rw-r--   0 akash     (1001) akash     (1001)       62 2023-06-23 17:36:11.000000 BoxKit-2023.6/BoxKit.egg-info/requires.txt
--rw-rw-r--   0 akash     (1001) akash     (1001)        7 2023-06-23 17:36:11.000000 BoxKit-2023.6/BoxKit.egg-info/top_level.txt
--rw-rw-r--   0 akash     (1001) akash     (1001)      565 2022-10-12 20:08:44.000000 BoxKit-2023.6/LICENSE
--rw-rw-r--   0 akash     (1001) akash     (1001)      150 2022-12-05 19:23:32.000000 BoxKit-2023.6/MANIFEST.in
--rw-rw-r--   0 akash     (1001) akash     (1001)     8416 2023-06-23 17:36:11.519286 BoxKit-2023.6/PKG-INFO
--rw-rw-r--   0 akash     (1001) akash     (1001)     8173 2023-06-23 01:08:56.000000 BoxKit-2023.6/README.rst
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.519286 BoxKit-2023.6/bin/
--rw-rw-r--   0 akash     (1001) akash     (1001)     1494 2022-12-13 20:20:33.000000 BoxKit-2023.6/bin/boost.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     1900 2022-12-13 20:20:52.000000 BoxKit-2023.6/bin/cbox.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     5127 2023-06-23 01:08:56.000000 BoxKit-2023.6/bin/cmd.py
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.515286 BoxKit-2023.6/boxkit/
--rw-rw-r--   0 akash     (1001) akash     (1001)      169 2023-06-23 01:08:56.000000 BoxKit-2023.6/boxkit/__init__.py
--rw-rw-r--   0 akash     (1001) akash     (1001)      248 2023-06-23 01:08:56.000000 BoxKit-2023.6/boxkit/__meta__.py
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.515286 BoxKit-2023.6/boxkit/api/
--rw-rw-r--   0 akash     (1001) akash     (1001)      325 2023-06-23 01:08:56.000000 BoxKit-2023.6/boxkit/api/__init__.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     4946 2023-06-21 20:21:20.000000 BoxKit-2023.6/boxkit/api/_create.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     2534 2023-06-16 22:20:01.000000 BoxKit-2023.6/boxkit/api/_mean.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     3619 2023-06-16 22:31:06.000000 BoxKit-2023.6/boxkit/api/_mergeblocks.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     2180 2023-06-16 22:21:49.000000 BoxKit-2023.6/boxkit/api/_read.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     1742 2023-06-21 20:23:23.000000 BoxKit-2023.6/boxkit/api/_regionprops.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     2162 2023-06-16 22:38:44.000000 BoxKit-2023.6/boxkit/api/_resfilter.py
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.515286 BoxKit-2023.6/boxkit/cbox/
--rw-rw-r--   0 akash     (1001) akash     (1001)       67 2023-06-23 01:08:56.000000 BoxKit-2023.6/boxkit/cbox/__init__.py
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.519286 BoxKit-2023.6/boxkit/cbox/__pycache__/
--rw-rw-r--   0 akash     (1001) akash     (1001)      244 2023-06-23 00:39:50.000000 BoxKit-2023.6/boxkit/cbox/__pycache__/__init__.cpython-38.pyc
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.515286 BoxKit-2023.6/boxkit/cbox/include/
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.519286 BoxKit-2023.6/boxkit/cbox/include/cbox/
--rw-rw-r--   0 akash     (1001) akash     (1001)     2070 2022-12-07 16:06:43.000000 BoxKit-2023.6/boxkit/cbox/include/cbox/library.h
--rw-rw-r--   0 akash     (1001) akash     (1001)     2826 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/cbox/include/cbox/pytypes.hpp
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.515286 BoxKit-2023.6/boxkit/cbox/lib/
--rw-rw-r--   0 akash     (1001) akash     (1001)      737 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/cbox/lib/__init__.py
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.519286 BoxKit-2023.6/boxkit/cbox/lib/__pycache__/
--rw-rw-r--   0 akash     (1001) akash     (1001)      650 2022-08-06 19:53:36.000000 BoxKit-2023.6/boxkit/cbox/lib/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 akash     (1001) akash     (1001)      239 2022-12-07 16:32:12.000000 BoxKit-2023.6/boxkit/cbox/lib/__pycache__/boost.cpython-38.pyc
--rw-rw-r--   0 akash     (1001) akash     (1001)      481 2022-12-07 16:32:12.000000 BoxKit-2023.6/boxkit/cbox/lib/__pycache__/extern.cpython-38.pyc
--rw-rw-r--   0 akash     (1001) akash     (1001)       61 2022-12-07 16:07:12.000000 BoxKit-2023.6/boxkit/cbox/lib/boost.py
--rw-rw-r--   0 akash     (1001) akash     (1001)      372 2022-12-07 16:07:42.000000 BoxKit-2023.6/boxkit/cbox/lib/extern.py
--rwxrwxr-x   0 akash     (1001) akash     (1001)  1481192 2022-12-13 19:48:29.000000 BoxKit-2023.6/boxkit/cbox/lib/library.so
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.519286 BoxKit-2023.6/boxkit/cbox/source/
--rw-rw-r--   0 akash     (1001) akash     (1001)      635 2022-12-07 16:27:05.000000 BoxKit-2023.6/boxkit/cbox/source/Make.inc
--rw-rw-r--   0 akash     (1001) akash     (1001)      268 2022-12-07 16:21:06.000000 BoxKit-2023.6/boxkit/cbox/source/Makefile
--rw-rw-r--   0 akash     (1001) akash     (1001)      799 2022-12-07 16:09:57.000000 BoxKit-2023.6/boxkit/cbox/source/action.cpp
--rw-rw-r--   0 akash     (1001) akash     (1001)      175 2022-12-07 16:09:47.000000 BoxKit-2023.6/boxkit/cbox/source/block.cpp
--rw-rw-r--   0 akash     (1001) akash     (1001)      100 2022-12-07 16:10:18.000000 BoxKit-2023.6/boxkit/cbox/source/data.cpp
--rw-rw-r--   0 akash     (1001) akash     (1001)     1484 2022-12-07 16:10:40.000000 BoxKit-2023.6/boxkit/cbox/source/execute.cpp
--rw-rw-r--   0 akash     (1001) akash     (1001)     3023 2022-12-07 16:14:04.000000 BoxKit-2023.6/boxkit/cbox/source/library.cpp
--rw-rw-r--   0 akash     (1001) akash     (1001)     2167 2022-12-07 16:10:56.000000 BoxKit-2023.6/boxkit/cbox/source/monitor.cpp
--rw-rw-r--   0 akash     (1001) akash     (1001)      100 2022-12-07 16:11:03.000000 BoxKit-2023.6/boxkit/cbox/source/region.cpp
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.515286 BoxKit-2023.6/boxkit/depends/
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.519286 BoxKit-2023.6/boxkit/depends/indicators/
--rw-rw-r--   0 akash     (1001) akash     (1001)     1063 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/LICENSE
--rw-rw-r--   0 akash     (1001) akash     (1001)    11894 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/block_progress_bar.hpp
--rw-rw-r--   0 akash     (1001) akash     (1001)      191 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/color.hpp
--rw-rw-r--   0 akash     (1001) akash     (1001)     1394 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/cursor_control.hpp
--rw-rw-r--   0 akash     (1001) akash     (1001)     1283 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/cursor_movement.hpp
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.519286 BoxKit-2023.6/boxkit/depends/indicators/details/
--rw-rw-r--   0 akash     (1001) akash     (1001)     5791 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/details/stream_helper.hpp
--rw-rw-r--   0 akash     (1001) akash     (1001)    15169 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/display_width.hpp
--rw-rw-r--   0 akash     (1001) akash     (1001)     3621 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/dynamic_progress.hpp
--rw-rw-r--   0 akash     (1001) akash     (1001)      203 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/font_style.hpp
--rw-rw-r--   0 akash     (1001) akash     (1001)     9681 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/indeterminate_progress_bar.hpp
--rw-rw-r--   0 akash     (1001) akash     (1001)     2181 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/multi_progress.hpp
--rw-rw-r--   0 akash     (1001) akash     (1001)    14020 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/progress_bar.hpp
--rw-rw-r--   0 akash     (1001) akash     (1001)     9681 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/progress_spinner.hpp
--rw-rw-r--   0 akash     (1001) akash     (1001)      154 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/progress_type.hpp
--rw-rw-r--   0 akash     (1001) akash     (1001)     9235 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/setting.hpp
--rw-rw-r--   0 akash     (1001) akash     (1001)    21527 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/termcolor.hpp
--rw-rw-r--   0 akash     (1001) akash     (1001)     1061 2022-08-06 19:49:52.000000 BoxKit-2023.6/boxkit/depends/indicators/terminal_size.hpp
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.515286 BoxKit-2023.6/boxkit/library/
--rw-rw-r--   0 akash     (1001) akash     (1001)      397 2023-06-23 01:08:56.000000 BoxKit-2023.6/boxkit/library/__init__.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     2722 2023-06-23 01:08:56.000000 BoxKit-2023.6/boxkit/library/_action.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     9348 2023-06-16 04:08:50.000000 BoxKit-2023.6/boxkit/library/_block.py
--rw-rw-r--   0 akash     (1001) akash     (1001)    13529 2023-06-23 01:08:56.000000 BoxKit-2023.6/boxkit/library/_data.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     5635 2023-06-16 21:58:50.000000 BoxKit-2023.6/boxkit/library/_dataset.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     5232 2023-06-23 01:08:56.000000 BoxKit-2023.6/boxkit/library/_execute.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     1054 2023-06-23 01:08:56.000000 BoxKit-2023.6/boxkit/library/_monitor.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     4168 2023-06-16 21:58:56.000000 BoxKit-2023.6/boxkit/library/_region.py
--rw-rw-r--   0 akash     (1001) akash     (1001)      995 2022-12-14 00:40:29.000000 BoxKit-2023.6/boxkit/library/_resources.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     1586 2022-12-13 21:04:31.000000 BoxKit-2023.6/boxkit/library/_server.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     1204 2023-06-16 21:17:07.000000 BoxKit-2023.6/boxkit/library/_slice.py
--rw-rw-r--   0 akash     (1001) akash     (1001)      451 2023-06-16 21:07:32.000000 BoxKit-2023.6/boxkit/library/_timer.py
--rw-rw-r--   0 akash     (1001) akash     (1001)      125 2023-06-23 00:36:20.000000 BoxKit-2023.6/boxkit/options.py
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.515286 BoxKit-2023.6/boxkit/resources/
--rw-rw-r--   0 akash     (1001) akash     (1001)       46 2022-12-10 17:05:42.000000 BoxKit-2023.6/boxkit/resources/__init__.py
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.519286 BoxKit-2023.6/boxkit/resources/read/
--rw-rw-r--   0 akash     (1001) akash     (1001)      165 2022-12-10 17:05:15.000000 BoxKit-2023.6/boxkit/resources/read/__init__.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     2741 2022-12-13 22:39:41.000000 BoxKit-2023.6/boxkit/resources/read/_flash.py
--rw-rw-r--   0 akash     (1001) akash     (1001)     2066 2023-06-16 22:18:34.000000 BoxKit-2023.6/boxkit/resources/read/_sample.py
-drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2023-06-23 17:36:11.519286 BoxKit-2023.6/media/
--rw-rw-r--   0 akash     (1001) akash     (1001)      654 2022-12-16 04:52:14.000000 BoxKit-2023.6/media/book.svg
--rw-r--r--   0 akash     (1001) akash     (1001)      797 2022-10-14 20:25:51.000000 BoxKit-2023.6/media/icon.svg
--rw-rw-r--   0 akash     (1001) akash     (1001)    27691 2023-06-21 20:21:20.000000 BoxKit-2023.6/media/morton.png
--rw-rw-r--   0 akash     (1001) akash     (1001)    75136 2023-06-21 08:04:58.000000 BoxKit-2023.6/media/performance.png
--rw-rw-r--   0 akash     (1001) akash     (1001)   326203 2023-06-23 17:15:48.000000 BoxKit-2023.6/media/workflow.drawio
--rw-rw-r--   0 akash     (1001) akash     (1001)   208947 2023-06-23 17:15:48.000000 BoxKit-2023.6/media/workflow.png
--rw-rw-r--   0 akash     (1001) akash     (1001)       38 2023-06-23 17:36:11.519286 BoxKit-2023.6/setup.cfg
--rw-rw-r--   0 akash     (1001) akash     (1001)     1981 2022-12-16 20:50:52.000000 BoxKit-2023.6/setup.py
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.233574 BoxKit-3.0/
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.225574 BoxKit-3.0/BoxKit.egg-info/
+-rw-rw-r--   0 akash     (1001) akash     (1001)     2978 2022-12-08 16:50:54.000000 BoxKit-3.0/BoxKit.egg-info/PKG-INFO
+-rw-rw-r--   0 akash     (1001) akash     (1001)     2660 2022-12-08 16:50:54.000000 BoxKit-3.0/BoxKit.egg-info/SOURCES.txt
+-rw-rw-r--   0 akash     (1001) akash     (1001)        1 2022-12-08 16:50:54.000000 BoxKit-3.0/BoxKit.egg-info/dependency_links.txt
+-rw-rw-r--   0 akash     (1001) akash     (1001)       46 2022-12-08 16:50:54.000000 BoxKit-3.0/BoxKit.egg-info/requires.txt
+-rw-rw-r--   0 akash     (1001) akash     (1001)        7 2022-12-08 16:50:54.000000 BoxKit-3.0/BoxKit.egg-info/top_level.txt
+-rw-rw-r--   0 akash     (1001) akash     (1001)      565 2022-10-12 20:08:44.000000 BoxKit-3.0/LICENSE
+-rw-rw-r--   0 akash     (1001) akash     (1001)      150 2022-12-05 19:23:32.000000 BoxKit-3.0/MANIFEST.in
+-rw-rw-r--   0 akash     (1001) akash     (1001)     2978 2022-12-08 16:50:54.233574 BoxKit-3.0/PKG-INFO
+-rw-rw-r--   0 akash     (1001) akash     (1001)     2738 2022-10-19 20:21:33.000000 BoxKit-3.0/README.rst
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.229574 BoxKit-3.0/bin/
+-rw-rw-r--   0 akash     (1001) akash     (1001)     1458 2022-12-05 22:20:34.000000 BoxKit-3.0/bin/boost.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     1819 2022-12-07 17:42:18.000000 BoxKit-3.0/bin/cbox.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     4554 2022-12-07 17:42:59.000000 BoxKit-3.0/bin/cmd.py
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.225574 BoxKit-3.0/boxkit/
+-rw-rw-r--   0 akash     (1001) akash     (1001)      170 2022-12-07 16:29:05.000000 BoxKit-3.0/boxkit/__init__.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)      243 2022-12-08 16:50:28.000000 BoxKit-3.0/boxkit/__meta__.py
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.225574 BoxKit-3.0/boxkit/api/
+-rw-rw-r--   0 akash     (1001) akash     (1001)      144 2022-12-07 16:52:51.000000 BoxKit-3.0/boxkit/api/__init__.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     2622 2022-12-08 16:23:49.000000 BoxKit-3.0/boxkit/api/create.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     2937 2022-12-08 16:47:17.000000 BoxKit-3.0/boxkit/api/measure.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     1013 2022-12-08 16:23:49.000000 BoxKit-3.0/boxkit/api/read.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     2529 2022-12-08 16:26:52.000000 BoxKit-3.0/boxkit/api/reshape.py
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.225574 BoxKit-3.0/boxkit/cbox/
+-rw-rw-r--   0 akash     (1001) akash     (1001)       18 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/cbox/__init__.py
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.229574 BoxKit-3.0/boxkit/cbox/__pycache__/
+-rw-rw-r--   0 akash     (1001) akash     (1001)      185 2022-08-06 19:53:36.000000 BoxKit-3.0/boxkit/cbox/__pycache__/__init__.cpython-38.pyc
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.225574 BoxKit-3.0/boxkit/cbox/include/
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.229574 BoxKit-3.0/boxkit/cbox/include/cbox/
+-rw-rw-r--   0 akash     (1001) akash     (1001)     2070 2022-12-07 16:06:43.000000 BoxKit-3.0/boxkit/cbox/include/cbox/library.h
+-rw-rw-r--   0 akash     (1001) akash     (1001)     2826 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/cbox/include/cbox/pytypes.hpp
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.225574 BoxKit-3.0/boxkit/cbox/lib/
+-rw-rw-r--   0 akash     (1001) akash     (1001)      737 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/cbox/lib/__init__.py
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.229574 BoxKit-3.0/boxkit/cbox/lib/__pycache__/
+-rw-rw-r--   0 akash     (1001) akash     (1001)      650 2022-08-06 19:53:36.000000 BoxKit-3.0/boxkit/cbox/lib/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 akash     (1001) akash     (1001)      239 2022-12-07 16:32:12.000000 BoxKit-3.0/boxkit/cbox/lib/__pycache__/boost.cpython-38.pyc
+-rw-rw-r--   0 akash     (1001) akash     (1001)      481 2022-12-07 16:32:12.000000 BoxKit-3.0/boxkit/cbox/lib/__pycache__/extern.cpython-38.pyc
+-rw-rw-r--   0 akash     (1001) akash     (1001)       61 2022-12-07 16:07:12.000000 BoxKit-3.0/boxkit/cbox/lib/boost.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)      372 2022-12-07 16:07:42.000000 BoxKit-3.0/boxkit/cbox/lib/extern.py
+-rwxrwxr-x   0 akash     (1001) akash     (1001)  1481192 2022-12-08 16:37:55.000000 BoxKit-3.0/boxkit/cbox/lib/library.so
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.229574 BoxKit-3.0/boxkit/cbox/source/
+-rw-rw-r--   0 akash     (1001) akash     (1001)      635 2022-12-07 16:27:05.000000 BoxKit-3.0/boxkit/cbox/source/Make.inc
+-rw-rw-r--   0 akash     (1001) akash     (1001)      268 2022-12-07 16:21:06.000000 BoxKit-3.0/boxkit/cbox/source/Makefile
+-rw-rw-r--   0 akash     (1001) akash     (1001)      799 2022-12-07 16:09:57.000000 BoxKit-3.0/boxkit/cbox/source/action.cpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)      175 2022-12-07 16:09:47.000000 BoxKit-3.0/boxkit/cbox/source/block.cpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)      100 2022-12-07 16:10:18.000000 BoxKit-3.0/boxkit/cbox/source/data.cpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)     1484 2022-12-07 16:10:40.000000 BoxKit-3.0/boxkit/cbox/source/execute.cpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)     3023 2022-12-07 16:14:04.000000 BoxKit-3.0/boxkit/cbox/source/library.cpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)     2167 2022-12-07 16:10:56.000000 BoxKit-3.0/boxkit/cbox/source/monitor.cpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)      100 2022-12-07 16:11:03.000000 BoxKit-3.0/boxkit/cbox/source/region.cpp
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.225574 BoxKit-3.0/boxkit/depends/
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.229574 BoxKit-3.0/boxkit/depends/indicators/
+-rw-rw-r--   0 akash     (1001) akash     (1001)     1063 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/LICENSE
+-rw-rw-r--   0 akash     (1001) akash     (1001)    11894 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/block_progress_bar.hpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)      191 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/color.hpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)     1394 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/cursor_control.hpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)     1283 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/cursor_movement.hpp
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.229574 BoxKit-3.0/boxkit/depends/indicators/details/
+-rw-rw-r--   0 akash     (1001) akash     (1001)     5791 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/details/stream_helper.hpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)    15169 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/display_width.hpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)     3621 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/dynamic_progress.hpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)      203 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/font_style.hpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)     9681 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/indeterminate_progress_bar.hpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)     2181 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/multi_progress.hpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)    14020 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/progress_bar.hpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)     9681 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/progress_spinner.hpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)      154 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/progress_type.hpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)     9235 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/setting.hpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)    21527 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/termcolor.hpp
+-rw-rw-r--   0 akash     (1001) akash     (1001)     1061 2022-08-06 19:49:52.000000 BoxKit-3.0/boxkit/depends/indicators/terminal_size.hpp
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.229574 BoxKit-3.0/boxkit/library/
+-rw-rw-r--   0 akash     (1001) akash     (1001)      385 2022-12-08 03:52:43.000000 BoxKit-3.0/boxkit/library/__init__.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     2327 2022-12-08 05:41:15.000000 BoxKit-3.0/boxkit/library/_action.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     9105 2022-12-06 21:57:02.000000 BoxKit-3.0/boxkit/library/_block.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)    10703 2022-12-08 16:43:46.000000 BoxKit-3.0/boxkit/library/_data.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     3911 2022-12-08 16:42:38.000000 BoxKit-3.0/boxkit/library/_dataset.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     4882 2022-12-08 05:48:10.000000 BoxKit-3.0/boxkit/library/_execute.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)      660 2022-12-07 16:31:27.000000 BoxKit-3.0/boxkit/library/_monitor.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     4024 2022-12-06 21:57:02.000000 BoxKit-3.0/boxkit/library/_region.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     1465 2022-11-07 05:08:05.000000 BoxKit-3.0/boxkit/library/_server.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     1095 2022-08-06 19:49:53.000000 BoxKit-3.0/boxkit/library/_slice.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)      408 2022-12-07 17:38:27.000000 BoxKit-3.0/boxkit/library/_timer.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)       50 2022-12-08 16:37:48.000000 BoxKit-3.0/boxkit/options.py
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.229574 BoxKit-3.0/boxkit/resources/
+-rw-rw-r--   0 akash     (1001) akash     (1001)       69 2022-12-07 17:11:29.000000 BoxKit-3.0/boxkit/resources/__init__.py
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.229574 BoxKit-3.0/boxkit/resources/read/
+-rw-rw-r--   0 akash     (1001) akash     (1001)      165 2022-11-08 05:53:44.000000 BoxKit-3.0/boxkit/resources/read/__init__.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     2807 2022-11-08 05:53:44.000000 BoxKit-3.0/boxkit/resources/read/_flash.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)     1834 2022-12-05 22:48:31.000000 BoxKit-3.0/boxkit/resources/read/_sample.py
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.229574 BoxKit-3.0/boxkit/resources/stencils/
+-rw-rw-r--   0 akash     (1001) akash     (1001)      130 2022-12-08 07:17:06.000000 BoxKit-3.0/boxkit/resources/stencils/__init__.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)      762 2022-12-08 06:58:19.000000 BoxKit-3.0/boxkit/resources/stencils/_measure.py
+-rw-rw-r--   0 akash     (1001) akash     (1001)      766 2022-12-08 08:59:13.000000 BoxKit-3.0/boxkit/resources/stencils/_reshape.py
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.233574 BoxKit-3.0/media/
+-rw-r--r--   0 akash     (1001) akash     (1001)      797 2022-10-14 20:25:51.000000 BoxKit-3.0/media/icon.svg
+drwxrwxr-x   0 akash     (1001) akash     (1001)        0 2022-12-08 16:50:54.233574 BoxKit-3.0/options/
+-rw-rw-r--   0 akash     (1001) akash     (1001)       21 2022-12-05 21:20:15.000000 BoxKit-3.0/options/cbox.txt
+-rw-rw-r--   0 akash     (1001) akash     (1001)       39 2022-12-05 20:36:38.000000 BoxKit-3.0/options/dask.txt
+-rw-rw-r--   0 akash     (1001) akash     (1001)        8 2022-12-05 20:36:38.000000 BoxKit-3.0/options/pyarrow.txt
+-rw-rw-r--   0 akash     (1001) akash     (1001)        9 2022-12-05 20:36:38.000000 BoxKit-3.0/options/server.txt
+-rw-rw-r--   0 akash     (1001) akash     (1001)       21 2022-12-05 20:36:38.000000 BoxKit-3.0/options/testing.txt
+-rw-rw-r--   0 akash     (1001) akash     (1001)        5 2022-12-05 20:36:38.000000 BoxKit-3.0/options/zarr.txt
+-rw-rw-r--   0 akash     (1001) akash     (1001)       38 2022-12-08 16:50:54.233574 BoxKit-3.0/setup.cfg
+-rw-rw-r--   0 akash     (1001) akash     (1001)     1905 2022-12-07 16:21:32.000000 BoxKit-3.0/setup.py
```

### Comparing `BoxKit-2023.6/BoxKit.egg-info/SOURCES.txt` & `BoxKit-3.0/BoxKit.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -7,41 +7,41 @@
 ./BoxKit.egg-info/dependency_links.txt
 ./BoxKit.egg-info/requires.txt
 ./BoxKit.egg-info/top_level.txt
 ./boxkit/__init__.py
 ./boxkit/__meta__.py
 ./boxkit/options.py
 ./boxkit/api/__init__.py
-./boxkit/api/_create.py
-./boxkit/api/_mean.py
-./boxkit/api/_mergeblocks.py
-./boxkit/api/_read.py
-./boxkit/api/_regionprops.py
-./boxkit/api/_resfilter.py
+./boxkit/api/create.py
+./boxkit/api/measure.py
+./boxkit/api/read.py
+./boxkit/api/reshape.py
 ./boxkit/cbox/__init__.py
 ./boxkit/cbox/lib/__init__.py
 ./boxkit/cbox/lib/boost.py
 ./boxkit/cbox/lib/extern.py
 ./boxkit/cbox/lib/library.so
 ./boxkit/library/__init__.py
 ./boxkit/library/_action.py
 ./boxkit/library/_block.py
 ./boxkit/library/_data.py
 ./boxkit/library/_dataset.py
 ./boxkit/library/_execute.py
 ./boxkit/library/_monitor.py
 ./boxkit/library/_region.py
-./boxkit/library/_resources.py
 ./boxkit/library/_server.py
 ./boxkit/library/_slice.py
 ./boxkit/library/_timer.py
 ./boxkit/resources/__init__.py
 ./boxkit/resources/read/__init__.py
 ./boxkit/resources/read/_flash.py
 ./boxkit/resources/read/_sample.py
+./boxkit/resources/stencils/__init__.py
+./boxkit/resources/stencils/_measure.py
+./boxkit/resources/stencils/_reshape.py
 bin/boost.py
 bin/cbox.py
 bin/cmd.py
 boxkit/cbox/__init__.py
 boxkit/cbox/__pycache__/__init__.cpython-38.pyc
 boxkit/cbox/include/cbox/library.h
 boxkit/cbox/include/cbox/pytypes.hpp
@@ -74,13 +74,14 @@
 boxkit/depends/indicators/progress_bar.hpp
 boxkit/depends/indicators/progress_spinner.hpp
 boxkit/depends/indicators/progress_type.hpp
 boxkit/depends/indicators/setting.hpp
 boxkit/depends/indicators/termcolor.hpp
 boxkit/depends/indicators/terminal_size.hpp
 boxkit/depends/indicators/details/stream_helper.hpp
-media/book.svg
 media/icon.svg
-media/morton.png
-media/performance.png
-media/workflow.drawio
-media/workflow.png
+options/cbox.txt
+options/dask.txt
+options/pyarrow.txt
+options/server.txt
+options/testing.txt
+options/zarr.txt
```

### Comparing `BoxKit-2023.6/LICENSE` & `BoxKit-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/bin/boost.py` & `BoxKit-3.0/bin/boost.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Custom commands for BoxKit setup."""
 
 import os
 import sys
 import subprocess
-from distutils.sysconfig import get_python_version  # pylint: disable=deprecated-module
+from distutils.sysconfig import get_python_version
 
 sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
 
-
 def boost_build():
     """Installation for Boost library"""
     subprocess.run(
         "git submodule update --init --recursive submodules/boost",
         shell=True,
         check=True,
         executable="/bin/bash",
@@ -38,19 +37,19 @@
     )
 
 
 def boost_install():
     """Install Boost library"""
     if os.path.exists(os.getenv("PWD") + "/boxkit/depends/boost"):
         subprocess.run(
-            "mkdir -pv build/lib/boxkit/depends/boost/lib",
+            f"mkdir -pv build/lib/boxkit/depends/boost/lib",
             shell=True,
             check=True,
             executable="/bin/bash",
         )
 
         subprocess.run(
-            "cp boxkit/depends/boost/lib/lib* build/lib/boxkit/depends/boost/lib/.",
+            f"cp boxkit/depends/boost/lib/lib* build/lib/boxkit/depends/boost/lib/.",
             shell=True,
             check=True,
             executable="/bin/bash",
         )
```

### Comparing `BoxKit-2023.6/bin/cbox.py` & `BoxKit-3.0/bin/cbox.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Custom commands for BoxKit setup."""
 
 import os
 import sys
 import subprocess
-from distutils import sysconfig  # pylint: disable=deprecated-module
+from distutils import sysconfig
 
 sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
 
 # Dictionary of Makefile variables for CBox
 # These variables are defined in boxkit/cbox/source/Make.inc
 # and are assigned here to build and compile when setting up the
 # Python library
@@ -35,24 +35,23 @@
 for key, value in CBOX_MAKE_DICT.items():
     CBOX_MAKE_ARGS = CBOX_MAKE_ARGS + " " + f"{key}={value}"
 
 # CBox build command which goes into cbox directory and compiles
 # the source code
 def cbox_build():
     """Compile and build cbox"""
-    from find_libpython import find_libpython  # pylint: disable=import-outside-toplevel
+    from find_libpython import find_libpython
 
     subprocess.run(
         f"cd boxkit/cbox/source && make {CBOX_MAKE_ARGS} python_lib_path={find_libpython()}",
         shell=True,
         check=True,
         executable="/bin/bash",
     )
 
-
 # Clean CBox environment
 def cbox_clean():
     """Clean cbox objects"""
     subprocess.run(
         "cd boxkit/cbox/source && make clean && cd ../../../",
         shell=True,
         check=True,
```

### Comparing `BoxKit-2023.6/bin/cmd.py` & `BoxKit-3.0/bin/cmd.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from setuptools.command.develop import develop
 
 sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
 
 # Import cbox_build from cbox
 # module located in the 'bin' folder of the
 # package directory
-from cbox import cbox_build  # pylint: disable=wrong-import-position
-from boost import boost_install  # pylint: disable=wrong-import-position
+from cbox import cbox_build
+from boost import boost_install
 
 # custom command
 class CustomCmd:
     """Custom command."""
 
     user_options = [
         ("with-cbox", None, "With C++ backend"),
@@ -23,104 +23,96 @@
         ("with-zarr", None, "With zarr data backend"),
         ("with-dask", None, "With dask data/parallel backend"),
         ("with-server", None, "With remote server utilitiy"),
         ("enable-testing", None, "Enable testing mode"),
     ]
 
     def initialize_options(self):
-        """
-        Initialize options
-        """
-        self.with_cbox = 0  # pylint: disable=attribute-defined-outside-init
-        self.with_pyarrow = 0  # pylint: disable=attribute-defined-outside-init
-        self.with_zarr = 0  # pylint: disable=attribute-defined-outside-init
-        self.with_dask = 0  # pylint: disable=attribute-defined-outside-init
-        self.with_server = 0  # pylint: disable=attribute-defined-outside-init
-        self.enable_testing = 0  # pylint: disable=attribute-defined-outside-init
+        self.with_cbox = 0
+        self.with_pyarrow = 0
+        self.with_zarr = 0
+        self.with_dask = 0
+        self.with_server = 0
+        self.enable_testing = 0
 
     def finalize_options(self):
-        """
-        Finalize options
-        """
         for option in [
             "with_cbox",
             "with_pyarrow",
             "with_zarr",
             "with_dask",
             "with_server",
             "enable_testing",
         ]:
             if getattr(self, option) not in [0, 1]:
                 raise ValueError(f"{option} is a flag")
 
     def run(self, user):
-        """
-        Run command
-        """
+
         if user:
             with_user = "--user"
         else:
             with_user = ""
 
         if self.with_cbox:
             subprocess.run(
-                f"{sys.executable} -m pip install -r requirements/cbox.txt {with_user}",
+                f"{sys.executable} -m pip install -r options/cbox.txt {with_user}",
                 shell=True,
                 check=True,
                 executable="/bin/bash",
             )
 
         if self.with_pyarrow:
             subprocess.run(
-                f"{sys.executable} -m pip install -r requirements/pyarrow.txt {with_user}",
+                f"{sys.executable} -m pip install -r options/pyarrow.txt {with_user}",
                 shell=True,
                 check=True,
                 executable="/bin/bash",
             )
 
         if self.with_zarr:
             subprocess.run(
-                f"{sys.executable} -m pip install -r requirements/zarr.txt {with_user}",
+                f"{sys.executable} -m pip install -r options/zarr.txt {with_user}",
                 shell=True,
                 check=True,
                 executable="/bin/bash",
             )
 
         if self.with_dask:
             subprocess.run(
-                f"{sys.executable} -m pip install -r requirements/dask.txt {with_user}",
+                f"{sys.executable} -m pip install -r options/dask.txt {with_user}",
                 shell=True,
                 check=True,
                 executable="/bin/bash",
             )
 
         if self.with_server:
             subprocess.run(
-                f"{sys.executable} -m pip install -r requirements/server.txt {with_user}",
+                f"{sys.executable} -m pip install -r options/server.txt {with_user}",
                 shell=True,
                 check=True,
                 executable="/bin/bash",
             )
 
         if self.enable_testing:
             subprocess.run(
-                f"{sys.executable} -m pip install -r requirements/testing.txt {with_user}",
+                f"{sys.executable} -m pip install -r options/testing.txt {with_user}",
                 shell=True,
                 check=True,
                 executable="/bin/bash",
             )
 
-        with open("boxkit/options.py", "w", encoding="ascii") as optfile:
+        with open("boxkit/options.py", "w") as optfile:
 
-            optfile.write(f"CBOX={self.with_cbox}\n")
-            optfile.write(f"PYARROW={self.with_pyarrow}\n")
-            optfile.write(f"ZARR={self.with_zarr}\n")
-            optfile.write(f"DASK={self.with_dask}\n")
-            optfile.write(f"SERVER={self.with_server}\n")
-            optfile.write(f"TESTING={self.enable_testing}\n")
+            optfile.write(f"cbox={self.with_cbox}\n")
+            optfile.write(f"pyarrow={self.with_pyarrow}\n")
+            optfile.write(f"zarr={self.with_zarr}\n")
+            optfile.write(f"dask={self.with_dask}\n")
+            optfile.write(f"server={self.with_server}\n")
+            optfile.write(f"testing={self.enable_testing}\n")
 
 
 # replaces the default build command for setup.py
 class InstallCmd(install, CustomCmd):
     """Custom build command."""
 
     user_options = install.user_options + CustomCmd.user_options
```

### Comparing `BoxKit-2023.6/boxkit/cbox/include/cbox/library.h` & `BoxKit-3.0/boxkit/cbox/include/cbox/library.h`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/cbox/include/cbox/pytypes.hpp` & `BoxKit-3.0/boxkit/cbox/include/cbox/pytypes.hpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/cbox/lib/__init__.py` & `BoxKit-3.0/boxkit/cbox/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/cbox/lib/__pycache__/__init__.cpython-38.pyc` & `BoxKit-3.0/boxkit/cbox/lib/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/cbox/lib/library.so` & `BoxKit-3.0/boxkit/cbox/lib/library.so`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/cbox/source/Make.inc` & `BoxKit-3.0/boxkit/cbox/source/Make.inc`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/cbox/source/action.cpp` & `BoxKit-3.0/boxkit/cbox/source/action.cpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/cbox/source/execute.cpp` & `BoxKit-3.0/boxkit/cbox/source/execute.cpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/cbox/source/library.cpp` & `BoxKit-3.0/boxkit/cbox/source/library.cpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/cbox/source/monitor.cpp` & `BoxKit-3.0/boxkit/cbox/source/monitor.cpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/depends/indicators/LICENSE` & `BoxKit-3.0/boxkit/depends/indicators/LICENSE`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/depends/indicators/block_progress_bar.hpp` & `BoxKit-3.0/boxkit/depends/indicators/block_progress_bar.hpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/depends/indicators/cursor_control.hpp` & `BoxKit-3.0/boxkit/depends/indicators/cursor_control.hpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/depends/indicators/cursor_movement.hpp` & `BoxKit-3.0/boxkit/depends/indicators/cursor_movement.hpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/depends/indicators/details/stream_helper.hpp` & `BoxKit-3.0/boxkit/depends/indicators/details/stream_helper.hpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/depends/indicators/display_width.hpp` & `BoxKit-3.0/boxkit/depends/indicators/display_width.hpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/depends/indicators/dynamic_progress.hpp` & `BoxKit-3.0/boxkit/depends/indicators/dynamic_progress.hpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/depends/indicators/indeterminate_progress_bar.hpp` & `BoxKit-3.0/boxkit/depends/indicators/indeterminate_progress_bar.hpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/depends/indicators/multi_progress.hpp` & `BoxKit-3.0/boxkit/depends/indicators/multi_progress.hpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/depends/indicators/progress_bar.hpp` & `BoxKit-3.0/boxkit/depends/indicators/progress_bar.hpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/depends/indicators/progress_spinner.hpp` & `BoxKit-3.0/boxkit/depends/indicators/progress_spinner.hpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/depends/indicators/setting.hpp` & `BoxKit-3.0/boxkit/depends/indicators/setting.hpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/depends/indicators/termcolor.hpp` & `BoxKit-3.0/boxkit/depends/indicators/termcolor.hpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/depends/indicators/terminal_size.hpp` & `BoxKit-3.0/boxkit/depends/indicators/terminal_size.hpp`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/boxkit/library/_action.py` & `BoxKit-3.0/boxkit/library/_action.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Module with implementation of Action utility"""
-from types import GeneratorType
+
 import copy
 
-from boxkit import library  # pylint: disable=cyclic-import
+from .. import library
 
 
-class Action:  # pylint: disable=too-many-arguments
+class Action:
     """Default class for an action."""
 
     type_ = "default"
 
     @staticmethod
     def toparg(*args):
-        """Method to get top argument from args"""
+        """Method to get top argument from *args"""
 
         top = args[0]
 
         args = list(args)
         args.pop(0)
         args = tuple(args)
 
@@ -24,31 +24,33 @@
 
     def __init__(
         self,
         target=None,
         nthreads=1,
         monitor=False,
         backend="serial",
+        unit=None,
     ):
         """Initialize the  object and allocate the data.
 
         Parameters
         ----------
-        target   : function/task operates on an parallel_obj ---> def target(parallel_obj, *args)
-                   actual call passes obj_list ---> target(obj_list, *args)
+        target   : function/task operates on an unit ---> def target(unit, *args)
+                   actual call passes unitlist ---> target(unitlist, *args)
         nthreads : number of nthreads (only relevant for parallel operations)
         monitor  : flag (True or False) to show progress bar for task
         backend  : 'serial', 'loky', 'dask'
-        parallel_obj     : parallel_obj type
+        unit     : unit type
         """
         super().__init__()
         self.target = target
         self.nthreads = nthreads
         self.monitor = monitor
         self.backend = backend
+        self.unit = unit
         self.batch = "auto"
 
     def __call__(self, *args, **kwargs):
         """Call wrapper"""
 
         if self.target is None:
             self.target = args[0]
@@ -63,33 +65,27 @@
         """Custom copy method"""
 
         return copy.copy(self)
 
     def execute(self, *args, **kwargs):
         """Custom call signature"""
 
-        toparg, args = Action.toparg(*args)
+        unitlist, args = Action.toparg(*args)
 
-        if not isinstance(toparg, GeneratorType) and not isinstance(toparg, list):
-            raise ValueError(
-                "[boxkit.library.Action] First argument "
-                + f"must be {GeneratorType!r} or {list!r} not {type(toparg)!r}"
-            )
+        self._check_unitlist(unitlist)
 
-        obj_list = list(toparg)
-        del toparg
-        self.__class__.chk_obj_list(obj_list)
+        return library.exectask(self, unitlist, *args, **kwargs)
 
-        return library.exectask(self, obj_list, *args, **kwargs)
+    def _check_unitlist(self, unitlist):
+        """Check if unitlist matches the unit type"""
 
-    @staticmethod
-    def chk_obj_list(obj_list):
-        """Check if obj_list matches the parallel_obj type"""
+        if not isinstance(unitlist, list):
+            raise ValueError(
+                "[boxkit.library.Action] Top argument must be a list of units"
+            )
 
-        first_obj = obj_list[0]
-        for index, parallel_obj in enumerate(obj_list):
-            if not isinstance(parallel_obj, type(first_obj)):
+        for unit in unitlist:
+            if not isinstance(unit, self.unit):
                 raise ValueError(
-                    "[boxkit.library.Action] Inconsistent type "
-                    + f"{type(parallel_obj)} vs {type(first_obj)} at index "
-                    + f'"{index}" in parallel object list'
+                    "[boxkit.library.Action] Unit type not consistent."
+                    + f'Expected "{self.unit}" but got "{type(unit)}"'
                 )
```

### Comparing `BoxKit-2023.6/boxkit/library/_block.py` & `BoxKit-3.0/boxkit/library/_block.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module with implementation of the Block class."""
 
 import numpy
 import pymorton
 
 
-class Block:  # pylint: disable=too-many-instance-attributes
+class Block:
     """Default class for a Block.
 
     Parameters
     ----------
     data       : data object
     attributes : dictionary
                { 'dx'   : grid spacing in x dir
@@ -17,33 +17,34 @@
                  'xmin' : low  bound in x dir
                  'ymin' : low  bound in y dir
                  'zmin' : low  bound in z dir
                  'xmax' : high bound in x dir
                  'ymax' : high bound in y dir
                  'zmax' : high bound in z dir
                  'tag'  : block ID }
+
+    Auxillary attributes
+    --------------------
+    { 'nxb' : number of points in x dir
+      'nyb' : number of points in y dir
+      'nzb' : number of points in z dir
+      'xguard' : number of guard cells in x dir
+      'yguard' : number of guard cells in y dir
+      'zguard' : number of guard cells in z dir
+      'xcenter' : block xcenter
+      'ycenter' : block ycenter
+      'zcenter' : block zcenter }
     """
 
     type_ = "default"
 
     def __init__(self, data=None, **attributes):
         """Initialize the  object and allocate the data."""
         super().__init__()
 
-        self.dx, self.dy, self.dz = [1.0, 1.0, 1.0]  # pylint: disable=invalid-name
-        self.xmin, self.ymin, self.zmin = [0.0, 0.0, 0.0]
-        self.xmax, self.ymax, self.zmax = [0.0, 0.0, 0.0]
-        self.tag = 0
-        self.level = 1
-        self.inputproc = None
-        self.leaf = True
-        self.xcenter, self.ycenter, self.zcenter = [0.0, 0.0, 0.0]
-        self.nxb, self.nyb, self.nzb = [1, 1, 1]
-        self.xguard, self.yguard, self.zguard = [0, 0, 0]
-
         self._set_attributes(attributes)
         self._map_data(data)
 
     def __repr__(self):
         """Return a representation of the object."""
         return (
             "Block:\n"
@@ -57,71 +58,83 @@
             + f" - leaf         : {self.leaf}\n"
         )
 
     def __getitem__(self, varkey):
         """
         Get variable data
         """
-        return self._data[varkey][self.tag, :]  # .to_numpy()[:]
+        return self._data[varkey][self.tag]  # .to_numpy()[:]
 
     def __setitem__(self, varkey, value):
         """
         Set variable data
         """
-        self._data[varkey][self.tag, :] = value  # .to_numpy()[:] = value
+        self._data[varkey][self.tag] = value  # .to_numpy()[:] = value
 
     def xrange(self, location):
         """
         Get xrange of the block
         """
         range_dict = {
-            "center": self.__class__.get_center_loc,
-            "node": self.__class__.get_node_loc,
+            "center": self.__class__._get_center_loc,
+            "node": self.__class__._get_node_loc,
         }
 
-        return range_dict[location](self.xmin, self.xmax, self.dx, self.nxb)
+        return range_dict[location](
+            self.xmin, self.xmax, self.dx, self.xguard, self.nxb
+        )
 
     def yrange(self, location):
         """
         Get yrange of the block
         """
         range_dict = {
-            "center": self.__class__.get_center_loc,
-            "node": self.__class__.get_node_loc,
+            "center": self.__class__._get_center_loc,
+            "node": self.__class__._get_node_loc,
         }
 
-        return range_dict[location](self.ymin, self.ymax, self.dy, self.nyb)
+        return range_dict[location](
+            self.ymin, self.ymax, self.dy, self.yguard, self.nyb
+        )
 
     def zrange(self, location):
         """
         Get zrange of the block
         """
         range_dict = {
-            "center": self.__class__.get_center_loc,
-            "node": self.__class__.get_node_loc,
+            "center": self.__class__._get_center_loc,
+            "node": self.__class__._get_node_loc,
         }
 
-        return range_dict[location](self.zmin, self.zmax, self.dz, self.nzb)
+        return range_dict[location](
+            self.zmin, self.zmax, self.dz, self.zguard, self.nzb
+        )
 
     @staticmethod
-    def get_center_loc(min_val, max_val, delta, num_points):
+    def _get_center_loc(min_val, max_val, delta, guard, num_points):
         """Private method for center location"""
         return numpy.linspace(min_val + delta / 2, max_val - delta / 2, num_points)
 
     @staticmethod
-    def get_node_loc(
-        min_val, max_val, delta, num_points
-    ):  # pylint: disable=unused-argument
+    def _get_node_loc(min_val, max_val, delta, guard, num_points):
         """Private method for face location"""
-        return numpy.linspace(min_val, max_val, num_points)
+        return numpy.linspace(min_val, max_val, num_points + 1)
 
     def _set_attributes(self, attributes):
         """
         Private method for intialization
         """
+        self.dx, self.dy, self.dz = [1.0, 1.0, 1.0]
+        self.xmin, self.ymin, self.zmin = [0.0, 0.0, 0.0]
+        self.xmax, self.ymax, self.zmax = [0.0, 0.0, 0.0]
+        self.tag = 0
+        self.level = 1
+        self.inputproc = None
+        self.leaf = True
+
         for key, value in attributes.items():
             if hasattr(self, key):
                 setattr(self, key, value)
             else:
                 raise ValueError(
                     "[boxkit.library.create.Block] "
                     + f"Attribute {key} not present in class Block"
@@ -223,45 +236,31 @@
 
         self.neighdict.update(dict(zip(locations, neighlist)))
 
     def write_neighbuffer(self, varkey):
         """
         Write block data to buffer for halo exchange
         """
-        pass  # pylint: disable=W0107
 
     def read_neighbuffer(self, varkey):
         """
         Read neighbor buffer and perform halo exchange
         """
-        pass  # pylint: disable=W0107
 
     def neighdata(self, varkey, neighkey):
         """
         Get neighbor data
         """
         neighdata = None
 
         if self.neighdict[neighkey] is not None:
             neighdata = self._data[varkey][self.neighdict[neighkey]]  # .to_numpy()[:]
 
         return neighdata
 
-    def get_relative_loc(self, origin):
-        """
-        Get offset from origin
-        """
-        iloc, jloc, kloc = [
-            round((self.xmin - origin[0]) / (self.xmax - self.xmin + 1e-13)),
-            round((self.ymin - origin[1]) / (self.ymax - self.ymin + 1e-13)),
-            round((self.zmin - origin[2]) / (self.zmax - self.zmin + 1e-13)),
-        ]
-
-        return iloc, jloc, kloc
-
     def exchange_neighdata(self, varkey):
         """
         Exchange information
         """
         blockdata = self._data[varkey][self.tag]
 
         for guard in range(self.xguard):
```

### Comparing `BoxKit-2023.6/boxkit/library/_data.py` & `BoxKit-3.0/boxkit/library/_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 """Module with implementation of the Data class."""
 
 import os
 import string
 import random
 import shutil
-import h5py
-import h5pickle
+
 import numpy
 
-from boxkit import options
+from .. import options
 
-if options.DASK:
+if options.dask:
     import dask.array as dsarray
 
-if options.PYARROW:
+if options.pyarrow:
     import pyarrow
 
-if options.ZARR:
+if options.zarr:
     import zarr
 
-if options.CBOX:
+if options.cbox:
     from ..cbox.lib import boost as cbox
 
-    _DataBase = cbox.library.Data  # pylint: disable=c-extension-no-member
+    _DataBase = cbox.library.Data
 
 else:
     _DataBase = object
 
 
-class Data(_DataBase):  # pylint: disable=too-many-instance-attributes
+class Data(_DataBase):
     """Default class to store data"""
 
     type_ = "default"
 
     def __init__(self, **attributes):
         """Initialize the class object
 
@@ -48,27 +47,14 @@
                        'zguard'    : number of guard cells in z dir,
                        'inputfile' : hdf5 inputfile default (None),
                        'remotefile': sftp remote file default (None),
                        'variables' : dictionary of variables default ({}),
                        'storage'   : ('numpy', 'zarr', 'dask', 'pyarrow')}
         """
         super().__init__()
-
-        self.nblocks = 1
-        self.inputfile = None
-        self.remotefile = None
-        self.outfile = {}
-        self.boxmem = None
-        self.nxb, self.nyb, self.nzb = [1, 1, 1]
-        self.xguard, self.yguard, self.zguard = [0, 0, 0]
-        self.storage = "numpy-memmap"
-        self.variables = {}
-        self.dtype = {}
-        self.varlist = []
-
         self._set_attributes(attributes)
         self._set_data()
 
     def __repr__(self):
         """
         Return a representation of the object
         """
@@ -87,67 +73,33 @@
 
     def __setitem__(self, varkey, value):
         """
         Set variable data
         """
         self.variables[varkey] = value
 
-    def purge(self, purgeflag="all"):
-        """
-        Clean up data and close it
-        """
-        if self.boxmem and purgeflag in ("all", "boxmem"):
-            try:
-                shutil.rmtree(self.boxmem)
-            except os.error:
-                pass
-
-        if self.inputfile and purgeflag in ("all", "inputfile"):
-            self.inputfile.close()
-
-        if self.remotefile and purgeflag in ("all", "remotefile"):
-            self.remotefile.close()
-
-    def addvar(self, varkey, dtype=float):
-        """
-        Add a variables to data
-        """
-        if varkey in self.variables:
-            raise ValueError(
-                f"[boxkit.library.data] Variable {varkey!r} already present in dataset"
-            )
-
-        self.variables[varkey] = None
-        self.dtype[varkey] = dtype if dtype in [float, int, bool] else float
-        self.varlist.append(varkey)
-        self._set_data()
-
-    def delvar(self, varkey):
-        """
-        Delete a variable
-        """
-        del self.variables[varkey]
-        del self.dtype[varkey]
-
-        if self.boxmem:
-            outputfile = os.path.join(self.boxmem, varkey)
-            try:
-                shutil.rmtree(outputfile)
-            except os.error:
-                pass
-
-        self.varlist = list(self.variables.keys())
-
     def _set_attributes(self, attributes):
         """
         Private method for intialization
         """
+
+        self.nblocks = 1
+        self.inputfile = None
+        self.remotefile = None
+        self.boxmem = None
+        self.variables = {}
+        self.nxb, self.nyb, self.nzb = [1, 1, 1]
+        self.xguard, self.yguard, self.zguard = [0, 0, 0]
+        self.storage = "numpy-memmap"
+        self.dtype = {}
+        self.varlist = []
+
         for key, value in attributes.items():
             if hasattr(self, key):
-                if isinstance(type(getattr(self, key)), type(value)) and (
+                if (type(getattr(self, key)) != type(value)) and (
                     key not in ["inputfile", "remotefile"]
                 ):
                     print(key, type(getattr(self, key)), type(value))
                     raise ValueError(
                         "[boxkit.library.create.Data] "
                         + f'Type mismatch for attribute "{key}" in class Data'
                     )
@@ -158,85 +110,38 @@
                 raise ValueError(
                     "[boxkit.library.create.Data] "
                     + f'Attribute "{key}" not present in class Data'
                 )
 
         for key, value in self.variables.items():
             self.varlist.append(key)
-            if value is not None:
+            if value != None:
                 self.dtype[key] = type(value)
             else:
                 self.dtype[key] = float
 
     def _set_data(self):
         """
         Private method for setting new data
         """
         if self.storage == "numpy":
             self._create_numpy_arrays()
         elif self.storage == "numpy-memmap":
             self._create_numpy_memmap()
-        elif self.storage == "h5-datasets":
-            self._create_h5_datasets()
         elif self.storage == "zarr":
             self._create_zarr_objects()
         elif self.storage == "dask":
             self._create_numpy_memmap()
             self._create_dask_objects()
         else:
             raise NotImplementedError(
                 "[boxkit.library.create.Data] "
                 + f'Storage format "{self.storage}" not implemented'
             )
 
-    def _create_h5_datasets(self):
-        """
-        Create h5 datasets for empty keys in variables dictionary
-        """
-        emptykeys = [
-            key
-            for key, value in self.variables.items()
-            if isinstance(value, type(None))
-        ]
-        if not emptykeys:
-            return
-
-        if not self.boxmem:
-            namerandom = "".join(
-                random.choice(string.ascii_lowercase) for i in range(5)
-            )
-            self.boxmem = "".join(["./boxmem/", namerandom])
-        try:
-            os.makedirs(self.boxmem)
-        except FileExistsError:
-            pass
-
-        for varkey in emptykeys:
-            outputfile = h5py.File(os.path.join(self.boxmem, varkey), "w")
-
-            outputshape = [
-                self.nblocks,
-                self.nzb + 2 * self.zguard,
-                self.nyb + 2 * self.yguard,
-                self.nxb + 2 * self.xguard,
-            ]
-
-            outputfile.create_dataset(
-                varkey, data=numpy.zeros(outputshape, dtype=self.dtype[varkey])
-            )
-            outputfile.close()
-            del outputfile
-
-            self.outfile[varkey] = h5pickle.File(
-                os.path.join(self.boxmem, varkey), "r+", skip_cache=True
-            )
-
-            self.variables[varkey] = self.outfile[varkey][varkey]
-            self.dtype[varkey] = type(self.variables[varkey])
-
     def _create_numpy_memmap(self):
         """
         Create numpy memory maps for empty keys in variables dictionary
         """
         emptykeys = [
             key
             for key, value in self.variables.items()
@@ -245,61 +150,53 @@
         if not emptykeys:
             return
 
         if not self.boxmem:
             namerandom = "".join(
                 random.choice(string.ascii_lowercase) for i in range(5)
             )
-            self.boxmem = "".join(["./boxmem/", namerandom])
+            self.boxmem = "".join(["./boxmem_", namerandom])
         try:
-            os.makedirs(self.boxmem)
+            os.mkdir(self.boxmem)
         except FileExistsError:
             pass
 
         for varkey in emptykeys:
             outputfile = os.path.join(self.boxmem, varkey)
             outputshape = (
                 self.nblocks,
                 self.nzb + 2 * self.zguard,
                 self.nyb + 2 * self.yguard,
                 self.nxb + 2 * self.xguard,
             )
             self.variables[varkey] = numpy.memmap(
                 outputfile, dtype=self.dtype[varkey], shape=outputshape, mode="w+"
             )
-            self.variables[varkey].flush()
-            del self.variables[varkey]
-
-            self.variables[varkey] = numpy.memmap(
-                outputfile, dtype=self.dtype[varkey], shape=outputshape, mode="r+"
-            )
-
-            self.dtype[varkey] = type(self.variables[varkey])
 
     def _create_zarr_objects(self):
         """
         Create zarr objects
         """
 
-        if options.ZARR:
+        if options.zarr:
             emptykeys = [
                 key
                 for key, value in self.variables.items()
                 if isinstance(value, type(None))
             ]
             if not emptykeys:
                 return
 
             if not self.boxmem:
                 namerandom = "".join(
                     random.choice(string.ascii_lowercase) for i in range(5)
                 )
-                self.boxmem = "".join(["./boxmem/", namerandom])
+                self.boxmem = "".join(["./boxmem_", namerandom])
             try:
-                os.makedirs(self.boxmem)
+                os.mkdir(self.boxmem)
             except FileExistsError:
                 pass
 
             for varkey in emptykeys:
                 outputfile = os.path.join(self.boxmem, varkey)
                 outputshape = (
                     self.nblocks,
@@ -315,30 +212,14 @@
                         1,
                         self.nzb + 2 * self.zguard,
                         self.nyb + 2 * self.yguard,
                         self.nxb + 2 * self.xguard,
                     ),
                     dtype=self.dtype[varkey],
                 )
-                del self.variables[varkey]
-
-                self.variables[varkey] = zarr.open(
-                    outputfile,
-                    mode="r+",
-                    shape=outputshape,
-                    chunks=(
-                        1,
-                        self.nzb + 2 * self.zguard,
-                        self.nyb + 2 * self.yguard,
-                        self.nxb + 2 * self.xguard,
-                    ),
-                    dtype=self.dtype[varkey],
-                )
-
-                self.dtype[varkey] = type(self.variables[varkey])
 
         else:
             raise NotImplementedError(
                 "[boxkit.library.data] enable zarr using --with-zarr during install"
             )
 
     def _create_numpy_arrays(self):
@@ -360,21 +241,19 @@
                 self.nyb + 2 * self.yguard,
                 self.nxb + 2 * self.xguard,
             )
             self.variables[varkey] = numpy.ndarray(
                 dtype=self.dtype[varkey], shape=outputshape
             )
 
-            self.dtype[varkey] = type(self.variables[varkey])
-
     def _create_dask_objects(self):
         """
         Create dask array representation of data
         """
-        if options.DASK:
+        if options.dask:
             emptykeys = [
                 key
                 for key, value in self.variables.items()
                 if isinstance(value, type(None))
             ]
             if not emptykeys:
                 return
@@ -387,44 +266,84 @@
                             1,
                             self.nzb + 2 * self.zguard,
                             self.nyb + 2 * self.yguard,
                             self.nxb + 2 * self.xguard,
                         ),
                     )
 
-                    self.dtype[varkey] = type(self.variables[varkey])
-
         else:
             raise NotImplementedError(
                 "[boxkit.library.data] enable dask using --with-dask during install"
             )
 
     def _create_pyarrow_objects(self):
         """
         Create a pyarrow tensor objects
         """
-        if options.PYARROW:
+        if options.pyarrow:
             emptykeys = [
                 key
                 for key, value in self.variables.items()
                 if isinstance(value, type(None))
             ]
             if not emptykeys:
                 return
 
             for varkey in emptykeys:
-                if not isinstance(
-                    self.variables[varkey],
-                    pyarrow.lib.Tensor,  # pylint: disable=c-extension-no-member
-                ):
+                if not isinstance(self.variables[varkey], pyarrow.lib.Tensor):
                     templist = []
                     for lblock in range(self.nblocks):
                         templist.append(
                             pyarrow.Tensor.from_numpy(self.variables[varkey][lblock])
                         )
                     self.variables[varkey] = templist
-                    self.dtype[varkey] = type(self.variables[varkey])
 
         else:
             raise NotImplementedError(
                 "[boxkit.library.data] enable pyarrow using --with-pyarrow during install"
             )
+
+    def purge(self, purgeflag="all"):
+        """
+        Clean up data and close it
+        """
+        if self.boxmem and purgeflag in ("all", "boxmem"):
+            try:
+                shutil.rmtree(self.boxmem)
+            except:
+                pass
+
+        if self.inputfile and purgeflag in ("all", "inputfile"):
+            self.inputfile.close()
+
+        if self.remotefile and purgeflag in ("all", "remotefile"):
+            self.remotefile.close()
+
+    def addvar(self, varkey, dtype=float):
+        """
+        Add a variables to data
+        """
+        if varkey in self.variables:
+            raise ValueError(
+                f"[boxkit.library.data] Variable {varkey!r} already present in dataset"
+            )
+
+        self.variables[varkey] = None
+        self.dtype[varkey] = dtype if dtype in [float, int, bool] else float
+        self.varlist.append(varkey)
+        self._set_data()
+
+    def delvar(self, varkey):
+        """
+        Delete a variable
+        """
+        del self.variables[varkey]
+        del self.dtype[varkey]
+
+        if self.boxmem:
+            outputfile = os.path.join(self.boxmem, varkey)
+            try:
+                shutil.rmtree(outputfile)
+            except:
+                pass
+
+        self.varlist = list(self.variables.keys())
```

### Comparing `BoxKit-2023.6/boxkit/library/_region.py` & `BoxKit-3.0/boxkit/library/_region.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Module with implementation of the Region class."""
 
 
-class Region:  # pylint: disable=too-few-public-methods, disable=too-many-instance-attributes
+class Region:
     """Base class for a Region."""
 
     type_ = "base"
 
-    def __init__(self, blocklist, **attributes):
+    def __init__(self, blocklist=[], **attributes):
         """Initialize the Region object and allocate the data.
 
         Parameters
         ----------
         blocklist  : list of objects
         attributes : dictionary
                      { 'xmin' : low  bound in x dir
@@ -18,19 +18,14 @@
                        'zmin' : low  bound in z dir
                        'xmax' : high bound in x dir
                        'ymax' : high bound in y dir
                        'zmax' : high bound in z dir}
 
         """
         super().__init__()
-
-        self.xmin, self.ymin, self.zmin = [-1e10, -1e10, -1e10]
-        self.xmax, self.ymax, self.zmax = [1e10, 1e10, 1e10]
-        self.xcenter, self.ycenter, self.zcenter = [0.0, 0.0, 0.0]
-
         self._set_attributes(attributes)
         self._map_blocklist(blocklist)
 
     def __repr__(self):
         """Return a representation of the object."""
         return (
             "Region:\n"
@@ -40,14 +35,18 @@
             + f"[{self.xmin}, {self.xmax}]\n"
         )
 
     def _set_attributes(self, attributes):
         """`
         Private method for intialization
         """
+
+        self.xmin, self.ymin, self.zmin = [-1e10, -1e10, -1e10]
+        self.xmax, self.ymax, self.zmax = [1e10, 1e10, 1e10]
+
         for key, value in attributes.items():
             if hasattr(self, key):
                 setattr(self, key, value)
             else:
                 raise ValueError(
                     "[boxkit.library.create.Region] "
                     + f'Attribute "{key}" not present in class Region'
```

### Comparing `BoxKit-2023.6/boxkit/library/_slice.py` & `BoxKit-3.0/boxkit/library/_slice.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 """Module with implementation of the Slice class."""
 
-from boxkit.library import Region  # pylint: disable=cyclic-import
+from . import Region
 
 
-class Slice(Region):  # pylint: disable=too-few-public-methods
+class Slice(Region):
     """Derived class for a Slice."""
 
     type_ = "derived"
 
-    def __init__(self, blocklist, **attributes):  # pylint: disable=W0235
+    def __init__(self, blocklist=[], **attributes):
         """Initialize the Slice object and allocate the data.
 
         Parameters
         ----------
         blocklist  : list of blocks
         attributes : dictionary
                      { 'xmin' : low  bound in x dir
                        'ymin' : low  bound in y dir
                        'zmin' : low  bound in z dir
                        'xmax' : high bound in x dir
                        'ymax' : high bound in y dir
                        'zmax' : high bound in z dir}
         """
+
         super().__init__(blocklist, **attributes)
 
     def __repr__(self):
         """Return a representation of the object."""
         return (
             "Region:\n"
             + f" - type          : {type(self)}\n"
```

### Comparing `BoxKit-2023.6/boxkit/resources/read/_flash.py` & `BoxKit-3.0/boxkit/resources/read/_flash.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,21 +18,23 @@
     data_attributes  : dictionary containing data attributes
     block_attributes : dictionary containg block attributes
     """
     if server:
         # Read from remote path
         remotefile = server["sftp"].open(filename)
         remotefile.set_pipelined()
-        inputfile = h5py.File(remotefile, "r", skip_cache=True)
-        print("[boxkit.resource.read]: Avoid multiprocessing for remote files")
+        inputfile = h5py.File(remotefile, "r", skip_cache=False)
+        print(
+            "[boxkit.resource.read]: Remote files cannot be pickled. Multithreading should not be used"
+        )
 
     else:
         # Read from local path
         remotefile = None
-        inputfile = h5pickle.File(filename, "r", skip_cache=True)
+        inputfile = h5pickle.File(filename, "r", skip_cache=False)
 
     # Set variable dictionary for datasets
     variables = {}
 
     # Loop over unknowns and populate variable dict
     # with simulation datasets
     for unkvar in inputfile["unknown names"][:]:
@@ -77,14 +79,14 @@
             "ymin": inputfile["bounding box"][lblock][1][0],
             "zmin": inputfile["bounding box"][lblock][2][0],
             "xmax": inputfile["bounding box"][lblock][0][1],
             "ymax": inputfile["bounding box"][lblock][1][1],
             "zmax": inputfile["bounding box"][lblock][2][1],
             "tag": lblock,
             "level": inputfile["refine level"][lblock],
-            "leaf": bool(inputfile["node type"][lblock] == 1),
+            "leaf": (True if inputfile["node type"][lblock] == 1 else False),
             "inputproc": inputfile["processor number"][lblock],
         }
         for lblock in range(nblocks)
     ]
 
     return data_attributes, block_attributes
```

### Comparing `BoxKit-2023.6/boxkit/resources/read/_sample.py` & `BoxKit-3.0/boxkit/resources/read/_sample.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 """Module to read attributes from default files"""
 
 import h5pickle as h5py
 
 
-def read_test_sample(filename, server):  # pylint: disable=too-many-locals
+def read_test_sample(filename, server):
     """
     Read dataset from BoxKit test sample
 
     Parameters
     ----------
     filename : string containing file name
     server : server dictionary
 
     Returns
     -------
     data_attributes  : dictionary containing data attributes
     block_attributes : dictionary containg block attributes
     """
-    if server:
-        raise NotImplementedError("[boxkit.read.test_sample] Cannot read from server")
 
     # Read the hdf5 file
-    inputfile = h5py.File(filename, "r", skip_cache=True)
+    inputfile = h5py.File(filename, "r", skip_cache=False)
 
     # Extract data
     nblocks = inputfile["numbox"][0] * inputfile["numbox"][1] * inputfile["numbox"][2]
     nxb = inputfile["sizebox"][0]
     nyb = inputfile["sizebox"][1]
     nzb = inputfile["sizebox"][2]
     xmin = inputfile["boundbox/min"][:, 0]
     ymin = inputfile["boundbox/min"][:, 1]
     zmin = inputfile["boundbox/min"][:, 2]
     xmax = inputfile["boundbox/max"][:, 0]
     ymax = inputfile["boundbox/max"][:, 1]
     zmax = inputfile["boundbox/max"][:, 2]
-    dx = inputfile["deltas"][0]  # pylint: disable=invalid-name
-    dy = inputfile["deltas"][1]  # pylint: disable=invalid-name
-    dz = inputfile["deltas"][2]  # pylint: disable=invalid-name
+    dx = inputfile["deltas"][0]
+    dy = inputfile["deltas"][1]
+    dz = inputfile["deltas"][2]
 
     variables = {}
     variables.update(inputfile["quantities"])
 
     # Create data attributes
     data_attributes = {
         "nblocks": int(nblocks),
```

### Comparing `BoxKit-2023.6/media/icon.svg` & `BoxKit-3.0/media/icon.svg`

 * *Files identical despite different names*

### Comparing `BoxKit-2023.6/setup.py` & `BoxKit-3.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,39 +7,46 @@
 from setuptools import setup, find_packages
 
 sys.path.insert(0, os.path.dirname(os.path.abspath(__file__)))
 
 # Import bin from current working directory
 # sys.path.insert makes sure that current file path is searched
 # first to find this module
-import bin.cmd as bin_cmd  # pylint: disable=wrong-import-position
+import bin.cmd as bin_cmd
 
 # Parse README and get long
 # description
-with open("README.rst", mode="r", encoding="ascii") as readme:
+with open("README.rst", mode="r") as readme:
     long_description = readme.read()
 
 
 # Open metadata file to extract package information
-with open("boxkit/__meta__.py", mode="r", encoding="ascii") as source:
+with open("boxkit/__meta__.py", mode="r") as source:
     content = source.read().strip()
     metadata = {
         key: re.search(key + r'\s*=\s*[\'"]([^\'"]*)[\'"]', content).group(1)
         for key in [
             "__pkgname__",
             "__version__",
             "__authors__",
             "__license__",
             "__description__",
         ]
     }
 
 # core dependancies for the package
-with open("requirements/core.txt", mode="r", encoding="ascii") as core_reqs:
-    DEPENDENCIES = core_reqs.read()
+DEPENDENCIES = [
+    "numpy",
+    "h5py",
+    "h5pickle",
+    "pymorton",
+    "joblib",
+    "tqdm",
+    "toml",
+]
 
 # Call setup command with necessary arguments
 # replace existing build and develop commands
 # with custom commands defined in 'bin.cmd'
 setup(
     name=metadata["__pkgname__"],
     version=metadata["__version__"],
```

