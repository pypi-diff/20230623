# Comparing `tmp/gwinc-0.4.1.tar.gz` & `tmp/gwinc-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwinc-0.4.1.tar", last modified: Tue Nov 23 15:54:00 2021, max compression
+gzip compressed data, was "gwinc-0.5.0.tar", last modified: Fri Jun 23 16:37:28 2023, max compression
```

## Comparing `gwinc-0.4.1.tar` & `gwinc-0.5.0.tar`

### file list

```diff
@@ -1,82 +1,100 @@
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.526128 gwinc-0.4.1/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      456 2021-10-14 16:46:30.000000 gwinc-0.4.1/.flake8
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     2411 2020-10-05 12:48:10.000000 gwinc-0.4.1/CONTRIBUTING.md
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     3169 2020-11-24 17:09:04.000000 gwinc-0.4.1/HDF5_SCHEMATA.md
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1211 2019-02-23 10:33:16.000000 gwinc-0.4.1/LICENSE
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)       61 2020-11-24 17:09:04.000000 gwinc-0.4.1/MANIFEST.in
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    17505 2021-11-23 15:54:00.530126 gwinc-0.4.1/PKG-INFO
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    16362 2021-10-14 16:46:21.000000 gwinc-0.4.1/README.md
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     7210 2021-05-26 22:18:22.000000 gwinc-0.4.1/conftest.py
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.486144 gwinc-0.4.1/gwinc/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     9061 2021-10-14 16:46:30.000000 gwinc-0.4.1/gwinc/__init__.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    12095 2021-10-14 16:46:21.000000 gwinc-0.4.1/gwinc/__main__.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      142 2021-11-23 15:53:59.000000 gwinc-0.4.1/gwinc/_version.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      769 2019-09-30 23:46:32.000000 gwinc-0.4.1/gwinc/const.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     5191 2021-01-09 16:41:09.000000 gwinc-0.4.1/gwinc/gwinc_matlab.py
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.490142 gwinc-0.4.1/gwinc/ifo/
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.494141 gwinc-0.4.1/gwinc/ifo/Aplus/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      799 2020-11-24 17:09:04.000000 gwinc-0.4.1/gwinc/ifo/Aplus/__init__.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    12204 2021-10-14 16:46:21.000000 gwinc-0.4.1/gwinc/ifo/Aplus/ifo.yaml
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.494141 gwinc-0.4.1/gwinc/ifo/CE1/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1496 2021-10-14 16:46:21.000000 gwinc-0.4.1/gwinc/ifo/CE1/__init__.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    11617 2021-10-14 16:46:21.000000 gwinc-0.4.1/gwinc/ifo/CE1/ifo.yaml
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.498139 gwinc-0.4.1/gwinc/ifo/CE2silica/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1511 2021-10-14 16:46:21.000000 gwinc-0.4.1/gwinc/ifo/CE2silica/__init__.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    11613 2021-10-14 16:46:21.000000 gwinc-0.4.1/gwinc/ifo/CE2silica/ifo.yaml
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.498139 gwinc-0.4.1/gwinc/ifo/CE2silicon/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1542 2021-10-14 16:46:21.000000 gwinc-0.4.1/gwinc/ifo/CE2silicon/__init__.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    14352 2021-10-14 16:46:21.000000 gwinc-0.4.1/gwinc/ifo/CE2silicon/ifo.yaml
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.498139 gwinc-0.4.1/gwinc/ifo/Voyager/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      797 2020-11-24 17:09:04.000000 gwinc-0.4.1/gwinc/ifo/Voyager/__init__.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    15369 2021-10-14 16:46:21.000000 gwinc-0.4.1/gwinc/ifo/Voyager/ifo.yaml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      580 2020-12-16 16:39:27.000000 gwinc-0.4.1/gwinc/ifo/__init__.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1895 2021-02-24 00:55:06.000000 gwinc-0.4.1/gwinc/ifo/__main__.py
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.502138 gwinc-0.4.1/gwinc/ifo/aLIGO/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      705 2020-11-24 17:09:04.000000 gwinc-0.4.1/gwinc/ifo/aLIGO/__init__.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    11227 2021-10-14 16:46:21.000000 gwinc-0.4.1/gwinc/ifo/aLIGO/ifo.yaml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    25288 2021-11-23 15:47:29.000000 gwinc-0.4.1/gwinc/ifo/noises.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     4373 2020-11-24 17:09:04.000000 gwinc-0.4.1/gwinc/io.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    18220 2021-05-26 22:18:22.000000 gwinc-0.4.1/gwinc/nb.py
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.514133 gwinc-0.4.1/gwinc/noise/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      186 2018-05-24 06:47:43.000000 gwinc-0.4.1/gwinc/noise/__init__.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    34945 2021-01-05 22:58:26.000000 gwinc-0.4.1/gwinc/noise/coatingthermal.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     9356 2021-10-14 16:46:21.000000 gwinc-0.4.1/gwinc/noise/newtonian.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    34033 2021-10-14 16:46:30.000000 gwinc-0.4.1/gwinc/noise/quantum.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     4818 2021-10-14 16:46:21.000000 gwinc-0.4.1/gwinc/noise/residualgas.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     5164 2020-12-16 16:39:27.000000 gwinc-0.4.1/gwinc/noise/seismic.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     6182 2021-03-29 23:25:09.000000 gwinc-0.4.1/gwinc/noise/substratethermal.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     3661 2020-12-16 16:39:27.000000 gwinc-0.4.1/gwinc/noise/suspensionthermal.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1898 2021-06-10 03:15:19.000000 gwinc-0.4.1/gwinc/plot.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1468 2020-12-16 16:39:27.000000 gwinc-0.4.1/gwinc/squeeze.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    21791 2021-10-14 16:46:30.000000 gwinc-0.4.1/gwinc/struct.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    21318 2020-12-16 16:39:27.000000 gwinc-0.4.1/gwinc/suspension.py
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.518131 gwinc-0.4.1/gwinc/test/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)        0 2020-04-20 06:57:07.000000 gwinc-0.4.1/gwinc/test/__init__.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    12346 2020-11-24 17:09:04.000000 gwinc-0.4.1/gwinc/test/__main__.py
--rwxr-xr-x   0 jrollins  (1000) jrollins  (1000)      636 2020-10-05 12:48:10.000000 gwinc-0.4.1/gwinc/test/gen_cache.sh
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      658 2020-10-09 23:13:39.000000 gwinc-0.4.1/gwinc/test/test_io.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      205 2020-10-12 02:20:04.000000 gwinc-0.4.1/gwinc/test/test_nb.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     4144 2020-10-09 22:42:29.000000 gwinc-0.4.1/gwinc/test/test_struct.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     2707 2021-03-29 23:25:09.000000 gwinc-0.4.1/gwinc/trace.py
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.490142 gwinc-0.4.1/gwinc.egg-info/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)    17505 2021-11-23 15:53:59.000000 gwinc-0.4.1/gwinc.egg-info/PKG-INFO
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1449 2021-11-23 15:54:00.000000 gwinc-0.4.1/gwinc.egg-info/SOURCES.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)        1 2021-11-23 15:53:59.000000 gwinc-0.4.1/gwinc.egg-info/dependency_links.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)       47 2021-11-23 15:53:59.000000 gwinc-0.4.1/gwinc.egg-info/entry_points.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)       67 2021-11-23 15:53:59.000000 gwinc-0.4.1/gwinc.egg-info/requires.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)        6 2021-11-23 15:53:59.000000 gwinc-0.4.1/gwinc.egg-info/top_level.txt
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      382 2021-10-14 16:46:30.000000 gwinc-0.4.1/pytest.ini
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1629 2021-11-23 15:54:00.534125 gwinc-0.4.1/setup.cfg
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      496 2020-11-24 17:09:04.000000 gwinc-0.4.1/setup.py
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.466152 gwinc-0.4.1/test/
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.522130 gwinc-0.4.1/test/budgets/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      292 2021-05-26 22:18:22.000000 gwinc-0.4.1/test/budgets/test_budgets.py
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.526128 gwinc-0.4.1/test/inherit/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      280 2021-10-14 16:46:30.000000 gwinc-0.4.1/test/inherit/Aplus_mod.yaml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      215 2021-10-14 16:46:30.000000 gwinc-0.4.1/test/inherit/Aplus_mod2.yaml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)       59 2021-10-14 16:46:30.000000 gwinc-0.4.1/test/inherit/inherit_fail.yaml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)     1363 2021-10-14 16:46:30.000000 gwinc-0.4.1/test/inherit/test_inherit.py
-drwxr-xr-x   0 jrollins  (1000) jrollins  (1000)        0 2021-11-23 15:54:00.526128 gwinc-0.4.1/test/struct/
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)       76 2021-10-14 16:46:30.000000 gwinc-0.4.1/test/struct/test_load.yml
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      765 2021-10-14 16:46:30.000000 gwinc-0.4.1/test/struct/test_struct.py
--rw-r--r--   0 jrollins  (1000) jrollins  (1000)      239 2020-11-24 17:09:04.000000 gwinc-0.4.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.810861 gwinc-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)      456 2023-06-23 16:37:16.000000 gwinc-0.5.0/.flake8
+-rw-rw-rw-   0 root         (0) root         (0)     2411 2023-06-23 16:37:16.000000 gwinc-0.5.0/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     3169 2023-06-23 16:37:16.000000 gwinc-0.5.0/HDF5_SCHEMATA.md
+-rw-rw-rw-   0 root         (0) root         (0)     1211 2023-06-23 16:37:16.000000 gwinc-0.5.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-06-23 16:37:16.000000 gwinc-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    17467 2023-06-23 16:37:28.810861 gwinc-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    16344 2023-06-23 16:37:16.000000 gwinc-0.5.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     9916 2023-06-23 16:37:16.000000 gwinc-0.5.0/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.802861 gwinc-0.5.0/gwinc/
+-rw-rw-rw-   0 root         (0) root         (0)     9510 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12095 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-23 16:37:28.000000 gwinc-0.5.0/gwinc/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      769 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/const.py
+-rw-rw-rw-   0 root         (0) root         (0)     5191 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/gwinc_matlab.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.803861 gwinc-0.5.0/gwinc/ifo/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.803861 gwinc-0.5.0/gwinc/ifo/Aplus/
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/ifo/Aplus/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12204 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/ifo/Aplus/ifo.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.803861 gwinc-0.5.0/gwinc/ifo/CE1/
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/ifo/CE1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11617 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/ifo/CE1/ifo.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.803861 gwinc-0.5.0/gwinc/ifo/CE2silica/
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/ifo/CE2silica/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11613 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/ifo/CE2silica/ifo.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.804861 gwinc-0.5.0/gwinc/ifo/CE2silicon/
+-rw-rw-rw-   0 root         (0) root         (0)     1777 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/ifo/CE2silicon/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14352 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/ifo/CE2silicon/ifo.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.804861 gwinc-0.5.0/gwinc/ifo/Voyager/
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/ifo/Voyager/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15369 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/ifo/Voyager/ifo.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      580 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/ifo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1895 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/ifo/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.804861 gwinc-0.5.0/gwinc/ifo/aLIGO/
+-rw-rw-rw-   0 root         (0) root         (0)      909 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/ifo/aLIGO/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11227 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/ifo/aLIGO/ifo.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4493 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/ifo/noises.py
+-rw-rw-rw-   0 root         (0) root         (0)     4373 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/io.py
+-rw-rw-rw-   0 root         (0) root         (0)    20946 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/nb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.805861 gwinc-0.5.0/gwinc/noise/
+-rw-rw-rw-   0 root         (0) root         (0)      186 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/noise/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    37207 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/noise/coatingthermal.py
+-rw-rw-rw-   0 root         (0) root         (0)    10438 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/noise/newtonian.py
+-rw-rw-rw-   0 root         (0) root         (0)    37629 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/noise/quantum.py
+-rw-rw-rw-   0 root         (0) root         (0)     8667 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/noise/residualgas.py
+-rw-rw-rw-   0 root         (0) root         (0)     6121 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/noise/seismic.py
+-rw-rw-rw-   0 root         (0) root         (0)     7663 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/noise/substratethermal.py
+-rw-rw-rw-   0 root         (0) root         (0)     5459 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/noise/suspensionthermal.py
+-rw-rw-rw-   0 root         (0) root         (0)     1898 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)     1468 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/squeeze.py
+-rw-rw-rw-   0 root         (0) root         (0)    21791 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/struct.py
+-rw-rw-rw-   0 root         (0) root         (0)    21840 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/suspension.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.806861 gwinc-0.5.0/gwinc/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12346 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/test/__main__.py
+-rwxrwxrwx   0 root         (0) root         (0)      636 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/test/gen_cache.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2707 2023-06-23 16:37:16.000000 gwinc-0.5.0/gwinc/trace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.802861 gwinc-0.5.0/gwinc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17467 2023-06-23 16:37:28.000000 gwinc-0.5.0/gwinc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1925 2023-06-23 16:37:28.000000 gwinc-0.5.0/gwinc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 16:37:28.000000 gwinc-0.5.0/gwinc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-23 16:37:28.000000 gwinc-0.5.0/gwinc.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-06-23 16:37:28.000000 gwinc-0.5.0/gwinc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-23 16:37:28.000000 gwinc-0.5.0/gwinc.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      438 2023-06-23 16:37:16.000000 gwinc-0.5.0/pytest.ini
+-rw-rw-rw-   0 root         (0) root         (0)     1629 2023-06-23 16:37:28.811861 gwinc-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      496 2023-06-23 16:37:16.000000 gwinc-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.799861 gwinc-0.5.0/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.806861 gwinc-0.5.0/test/budgets/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.807861 gwinc-0.5.0/test/budgets/H1/
+-rw-rw-rw-   0 root         (0) root         (0)     5459 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/budgets/H1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12335 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/budgets/H1/ifo.yaml
+-rw-rw-rw-   0 root         (0) root         (0)   250127 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/budgets/H1/lho_o3.txt
+-rw-rw-rw-   0 root         (0) root         (0)  1000000 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/budgets/H1/lho_ref.txt
+-rw-rw-rw-   0 root         (0) root         (0)     8705 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/budgets/test_budgets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.808861 gwinc-0.5.0/test/inherit/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/inherit/Aplus_mod.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/inherit/Aplus_mod2.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       91 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/inherit/Aplus_mod3.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/inherit/inherit_fail.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       92 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/inherit/new_ifo.txt
+-rw-rw-rw-   0 root         (0) root         (0)    11285 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/inherit/new_ifo.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.809861 gwinc-0.5.0/test/inherit/subdir/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.809861 gwinc-0.5.0/test/inherit/subdir/CustomBudget/
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/inherit/subdir/CustomBudget/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12204 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/inherit/subdir/CustomBudget/ifo.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/inherit/subdir/CustomBudget_mod.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3428 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/inherit/test_inherit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.809861 gwinc-0.5.0/test/noises/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.809861 gwinc-0.5.0/test/noises/residualgas/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.809861 gwinc-0.5.0/test/noises/residualgas/AplusSuperGas/
+-rw-rw-rw-   0 root         (0) root         (0)     3473 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/noises/residualgas/AplusSuperGas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    28983 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/noises/residualgas/AplusSuperGas/beamtube_pressure.txt
+-rw-rw-rw-   0 root         (0) root         (0)    12204 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/noises/residualgas/AplusSuperGas/ifo.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     9451 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/noises/residualgas/test_residualgas.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/noises/test_quantum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 16:37:28.810861 gwinc-0.5.0/test/struct/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/struct/test_load.yml
+-rw-rw-rw-   0 root         (0) root         (0)      765 2023-06-23 16:37:16.000000 gwinc-0.5.0/test/struct/test_struct.py
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-06-23 16:37:16.000000 gwinc-0.5.0/tox.ini
```

### Comparing `gwinc-0.4.1/CONTRIBUTING.md` & `gwinc-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/HDF5_SCHEMATA.md` & `gwinc-0.5.0/HDF5_SCHEMATA.md`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/LICENSE` & `gwinc-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/PKG-INFO` & `gwinc-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: gwinc
-Version: 0.4.1
+Version: 0.5.0
 Summary: Gravitation Wave Interferometer Noise Calculator
 Home-page: https://git.ligo.org/gwinc/pygwinc
 Author: LIGO Scientific Collaboration
 Author-email: jameson.rollins@ligo.org
 License: UNLICENSE
 Project-URL: Bug Tracker, https://git.ligo.org/gwinc/pygwinc/issues
 Project-URL: Source Code, https://git.ligo.org/gwinc/pygwinc
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Science/Research
@@ -178,16 +177,16 @@
 in the specified budget module (see [budget
 interface](#budget-interface) below).  The budget `ifo` `gwinc.Struct`
 is available in the `budget.ifo` attribute.
 
 The budget `run()` method calculates all budget noises and the noise
 total and returns a `BudgetTrace` object with `freq`, `psd`, and `asd`
 properties.  The budget sub-traces are available through a dictionary
-(`trace['QuantumVacuum']`) interface and via attributes
-(`trace.QuantumVacumm`).
+(`trace['Quantum']`) interface and via attributes
+(`trace.Quantum`).
 
 The budget `freq` and `ifo` attributes can be updated at run time by
 passing them as keyword arguments to the `run()` method:
 ```python
 >>> budget = load_budget('aLIGO')
 >>> freq = np.logspace(1, 3, 1000)
 >>> ifo = Struct.from_file('/path/to/ifo_alt.yaml')
@@ -463,29 +462,29 @@
 There are various way to extract single noise terms from the Budget
 interface.  The most straightforward way is to run the full budget,
 and extract the noise data the output traces dictionary:
 
 ```python
 budget = load_budget('/path/to/MyBudget', freq)
 trace = budget.run()
-quantum_trace = trace['QuantumVacuum']
+quantum_trace = trace['Quantum']
 ```
 
 You can also calculate the final calibrated output noise for just a
 single term using the Budget `calc_noise()` method:
 ```python
-data = budget.calc_noise('QuantumVacuum')
+data = budget.calc_noise('Quantum')
 ```
 
 You can also calculate a noise at it's source, without applying any
 calibrations, by using the Budget `__getitem__` interface to extract
 the specific Noise BudgetItem for the noise you're interested in, and
-running it's `calc()` method directly:
+running it's `calc_trace()` method directly:
 ```python
-data = budget['QuantumVacuum'].calc()
+data = budget['Quantum'].calc_trace()
 ```
 
 
 # inspiral range
 
 The [`inspiral_range`](https://git.ligo.org/gwinc/inspiral-range)
 package can be used to calculate various common "inspiral range"
@@ -530,9 +529,7 @@
 <!-- This will produce a summary page of the various noise spectra that -->
 <!-- differ between matgwinc and pygwinc. -->
 
 <!-- Latest comparison plots from continuous integration: -->
 
 <!-- * [aLIGO comparison](https://gwinc.docs.ligo.org/pygwinc/aLIGO_test.png) -->
 <!-- * [A+ comparison](https://gwinc.docs.ligo.org/pygwinc/A+_test.png) -->
-
-
```

### Comparing `gwinc-0.4.1/README.md` & `gwinc-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -149,16 +149,16 @@
 in the specified budget module (see [budget
 interface](#budget-interface) below).  The budget `ifo` `gwinc.Struct`
 is available in the `budget.ifo` attribute.
 
 The budget `run()` method calculates all budget noises and the noise
 total and returns a `BudgetTrace` object with `freq`, `psd`, and `asd`
 properties.  The budget sub-traces are available through a dictionary
-(`trace['QuantumVacuum']`) interface and via attributes
-(`trace.QuantumVacumm`).
+(`trace['Quantum']`) interface and via attributes
+(`trace.Quantum`).
 
 The budget `freq` and `ifo` attributes can be updated at run time by
 passing them as keyword arguments to the `run()` method:
 ```python
 >>> budget = load_budget('aLIGO')
 >>> freq = np.logspace(1, 3, 1000)
 >>> ifo = Struct.from_file('/path/to/ifo_alt.yaml')
@@ -434,29 +434,29 @@
 There are various way to extract single noise terms from the Budget
 interface.  The most straightforward way is to run the full budget,
 and extract the noise data the output traces dictionary:
 
 ```python
 budget = load_budget('/path/to/MyBudget', freq)
 trace = budget.run()
-quantum_trace = trace['QuantumVacuum']
+quantum_trace = trace['Quantum']
 ```
 
 You can also calculate the final calibrated output noise for just a
 single term using the Budget `calc_noise()` method:
 ```python
-data = budget.calc_noise('QuantumVacuum')
+data = budget.calc_noise('Quantum')
 ```
 
 You can also calculate a noise at it's source, without applying any
 calibrations, by using the Budget `__getitem__` interface to extract
 the specific Noise BudgetItem for the noise you're interested in, and
-running it's `calc()` method directly:
+running it's `calc_trace()` method directly:
 ```python
-data = budget['QuantumVacuum'].calc()
+data = budget['Quantum'].calc_trace()
 ```
 
 
 # inspiral range
 
 The [`inspiral_range`](https://git.ligo.org/gwinc/inspiral-range)
 package can be used to calculate various common "inspiral range"
```

### Comparing `gwinc-0.4.1/conftest.py` & `gwinc-0.5.0/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,14 +36,22 @@
         "--no-preclear",
         action="store_true",
         default=False,
         dest='no_preclear',
         help="Do not preclear tpaths",
     )
 
+    parser.addoption(
+        "--generate",
+        action="store_true",
+        default=False,
+        dest="generate",
+        help="Generate test data",
+    )
+
 
 @pytest.fixture
 def plot(request):
     return request.config.getvalue('--plot')
     return request.config.option.plot
 
 
@@ -266,7 +274,87 @@
     if isinstance(post, (list, tuple)):
         post = path.join(post)
     if post is not None:
         return relfile(_file_, testname, post, fname = fname)
     else:
         return relfile(_file_, testname, fname = fname)
 
+
+@pytest.fixture
+def compare_noise(pprint):
+    """
+    Fixture to compare two sets of traces
+
+    A list of noises passed, failed, and skipped are printed. Comparisons are
+    skipped if the psd's are sufficiently small (controlled by psd_tol) indicating
+    that the noise is essentially zero or if a trace is missing.
+
+    An assertion error is raised if any noises fail.
+    """
+    import numpy as np
+
+    def compare(traces, ref_traces, psd_tol=1e-52):
+        passed = []
+        failed = []
+        skipped = []
+        if ref_traces.budget:
+            for ref_trace in ref_traces:
+                if np.all(ref_trace.psd < psd_tol):
+                    skipped.append(ref_trace.name)
+                    continue
+
+                try:
+                    trace = traces[ref_trace.name]
+                except KeyError:
+                    skipped.append(ref_trace.name)
+                    continue
+
+                if np.allclose(trace.psd, ref_trace.psd, atol=0):
+                    passed.append(trace.name)
+                else:
+                    failed.append(trace.name)
+        else:
+            if np.allclose(ref_traces.psd, traces.psd, atol=0):
+                passed.append(traces.name)
+            else:
+                failed.append(traces.name)
+
+        pprint('Noises failed:')
+        pprint(40 * '-')
+        for noise in failed:
+            pprint(noise)
+        pprint(40 * '+')
+        pprint('Noises passed:')
+        pprint(40 * '-')
+        for noise in passed:
+            pprint(noise)
+        pprint(40 * '+')
+        pprint('Noises skipped:')
+        pprint(40 * '-')
+        for noise in skipped:
+            pprint(noise)
+
+        assert len(failed) == 0
+
+    return compare
+
+
+def pytest_collection_modifyitems(config, items):
+    """
+    Modifies tests to be selectively skipped with command line options
+
+    https://docs.pytest.org/en/latest/example/simple.html#control-skipping-of-tests-according-to-command-line-option
+    """
+    # run tests marked as generate if and only if --generate is given
+    # skip all others in this case
+    if config.getoption('--generate'):
+        skip = pytest.mark.skip(
+            reason='only running tests that generate data')
+        for item in items:
+            if 'generate' not in item.keywords:
+                item.add_marker(skip)
+    else:
+        skip = pytest.mark.skip(
+            reason='generates test data: needs --generate to run')
+        for item in items:
+            if 'generate' in item.keywords:
+                item.add_marker(skip)
```

### Comparing `gwinc-0.4.1/gwinc/__init__.py` & `gwinc-0.5.0/gwinc/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,24 +40,24 @@
     None the DEFAULT_FREQ specification is used.
 
     """
     if isinstance(spec, np.ndarray):
         return spec
     elif spec is None:
         spec = DEFAULT_FREQ
-    fspec = spec.split(':')
     try:
+        fspec = spec.split(':')
         if len(fspec) == 2:
             fspec = fspec[0], DEFAULT_FREQ.split(':')[1], fspec[1]
         return np.logspace(
             np.log10(float(fspec[0])),
             np.log10(float(fspec[2])),
             int(fspec[1]),
         )
-    except (ValueError, IndexError):
+    except (ValueError, IndexError, AttributeError):
         raise InvalidFrequencySpec(f'Improper frequency specification: {spec}')
 
 
 def load_module(name_or_path):
     """Load module from name or path.
 
     Return loaded module and module path.
@@ -121,44 +121,56 @@
             logger.info("loading struct {}...".format(path))
             ifo = Struct.from_file(path, _pass_inherit=True)
 
             inherit_ifo = ifo.get('+inherit', None)
             if inherit_ifo is not None:
                 del ifo['+inherit']
                 # make the inherited path relative to the loaded path
-                # if it is a yml file
-                if os.path.splitext(inherit_ifo)[1] in Struct.STRUCT_EXT:
-                    base = os.path.split(path)[0]
-                    inherit_ifo = os.path.join(base, inherit_ifo)
+                # if it is a yml file or a directory
+                head = os.path.split(path)[0]
+                rel_path = os.path.join(head, inherit_ifo)
+                if os.path.splitext(inherit_ifo)[1] in Struct.STRUCT_EXT or os.path.exists(rel_path):
+                    inherit_ifo = rel_path
 
                 inherit_budget = load_budget(inherit_ifo, freq=freq, bname=bname)
                 pre_ifo = inherit_budget.ifo
-                pre_ifo.update(ifo, overwrite_atoms=False)
+                pre_ifo.update(
+                    ifo,
+                    overwrite_atoms=False,
+                    clear_test=lambda v: isinstance(v, str) and v == '<unset>'
+                )
                 inherit_budget.update(ifo=pre_ifo)
                 return inherit_budget
             else:
                 modname = 'gwinc.ifo.aLIGO'
-        else:
+                bname = bname or 'aLIGO'
+
+        elif ext == '':
             bname = bname or base
             modname = path
 
+        else:
+            raise RuntimeError(
+                "Unknown file type: {} (supported types: {}).".format(
+                    ext, Struct.STRUCT_EXT))
+
     else:
         if name_or_path not in IFOS:
             raise RuntimeError("Unknown IFO '{}' (available IFOs: {}).".format(
                 name_or_path,
                 IFOS,
             ))
         bname = bname or name_or_path
         modname = 'gwinc.ifo.' + name_or_path
 
     logger.info(f"loading budget '{bname}' from {modname}...")
     mod, modpath = load_module(modname)
     Budget = getattr(mod, bname)
     if freq is None:
-        freq = getattr(Budget, 'freq', None)
+        freq = getattr(Budget, '_freq', None)
     freq = freq_from_spec(freq)
     ifopath = os.path.join(modpath, 'ifo.yaml')
     if not ifo and os.path.exists(ifopath):
         ifo = Struct.from_file(ifopath)
     return Budget(freq=freq, ifo=ifo)
```

### Comparing `gwinc-0.4.1/gwinc/__main__.py` & `gwinc-0.5.0/gwinc/__main__.py`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/const.py` & `gwinc-0.5.0/gwinc/const.py`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/gwinc_matlab.py` & `gwinc-0.5.0/gwinc/gwinc_matlab.py`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/ifo/Aplus/ifo.yaml` & `gwinc-0.5.0/gwinc/ifo/Aplus/ifo.yaml`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/ifo/CE1/__init__.py` & `gwinc-0.5.0/gwinc/ifo/CE2silicon/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-from gwinc.ifo.noises import *
 from gwinc.ifo import PLOT_STYLE
+from gwinc import noise
+from gwinc import nb
+from gwinc.ifo.noises import Strain
 
 
-class QuantumVacuum(nb.Budget):
+class Quantum(nb.Budget):
     """Quantum Vacuum
 
     """
     style = dict(
         label='Quantum Vacuum',
         color='#ad03de',
     )
 
     noises = [
-        QuantumVacuumAS,
-        QuantumVacuumArm,
-        QuantumVacuumSEC,
-        QuantumVacuumFilterCavity,
-        QuantumVacuumInjection,
-        QuantumVacuumReadout,
-        QuantumVacuumQuadraturePhase,
+        noise.quantum.AS,
+        noise.quantum.Arm,
+        noise.quantum.SEC,
+        noise.quantum.FilterCavity,
+        noise.quantum.Injection,
+        noise.quantum.Readout,
+        noise.quantum.QuadraturePhase,
     ]
 
 
 class Newtonian(nb.Budget):
     """Newtonian Gravity
 
     """
@@ -31,17 +33,17 @@
 
     style = dict(
         label='Newtonian',
         color='#15b01a',
     )
 
     noises = [
-        NewtonianRayleigh,
-        NewtonianBody,
-        NewtonianInfrasound,
+        noise.newtonian.Rayleigh,
+        noise.newtonian.Body,
+        noise.newtonian.Infrasound,
     ]
 
 
 class Coating(nb.Budget):
     """Coating Thermal
 
     """
@@ -50,16 +52,16 @@
 
     style = dict(
         label='Coating Thermal',
         color='#fe0002',
     )
 
     noises = [
-        CoatingBrownian,
-        CoatingThermoOptic,
+        noise.coatingthermal.CoatingBrownian,
+        noise.coatingthermal.CoatingThermoOptic,
     ]
 
 
 class Substrate(nb.Budget):
     """Substrate Thermal
 
     """
@@ -68,31 +70,32 @@
 
     style = dict(
         label='Substrate Thermal',
         color='#fb7d07',
     )
 
     noises = [
-        SubstrateBrownian,
-        SubstrateThermoElastic,
+        noise.substratethermal.ITMThermoRefractive,
+        noise.substratethermal.SubstrateBrownian,
+        noise.substratethermal.SubstrateThermoElastic,
     ]
 
 
-class CE1(nb.Budget):
+class CE2silicon(nb.Budget):
 
-    name = 'Cosmic Explorer 1'
+    name = 'Cosmic Explorer 2 (Silicon)'
 
     noises = [
-        QuantumVacuum,
-        Seismic,
+        Quantum,
+        noise.seismic.Seismic,
         Newtonian,
-        SuspensionThermal,
+        noise.suspensionthermal.SuspensionThermal,
         Coating,
         Substrate,
-        ExcessGas,
+        noise.residualgas.ResidualGas,
     ]
 
     calibrations = [
         Strain,
     ]
 
     plot_style = PLOT_STYLE
```

### Comparing `gwinc-0.4.1/gwinc/ifo/CE1/ifo.yaml` & `gwinc-0.5.0/gwinc/ifo/CE1/ifo.yaml`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/ifo/CE2silica/__init__.py` & `gwinc-0.5.0/gwinc/ifo/CE1/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-from gwinc.ifo.noises import *
 from gwinc.ifo import PLOT_STYLE
+from gwinc import noise
+from gwinc import nb
+from gwinc.ifo.noises import Strain
 
 
-class QuantumVacuum(nb.Budget):
+class Quantum(nb.Budget):
     """Quantum Vacuum
 
     """
     style = dict(
         label='Quantum Vacuum',
         color='#ad03de',
     )
 
     noises = [
-        QuantumVacuumAS,
-        QuantumVacuumArm,
-        QuantumVacuumSEC,
-        QuantumVacuumFilterCavity,
-        QuantumVacuumInjection,
-        QuantumVacuumReadout,
-        QuantumVacuumQuadraturePhase,
+        noise.quantum.AS,
+        noise.quantum.Arm,
+        noise.quantum.SEC,
+        noise.quantum.FilterCavity,
+        noise.quantum.Injection,
+        noise.quantum.Readout,
+        noise.quantum.QuadraturePhase,
     ]
 
 
 class Newtonian(nb.Budget):
     """Newtonian Gravity
 
     """
@@ -31,17 +33,17 @@
 
     style = dict(
         label='Newtonian',
         color='#15b01a',
     )
 
     noises = [
-        NewtonianRayleigh,
-        NewtonianBody,
-        NewtonianInfrasound,
+        noise.newtonian.Rayleigh,
+        noise.newtonian.Body,
+        noise.newtonian.Infrasound,
     ]
 
 
 class Coating(nb.Budget):
     """Coating Thermal
 
     """
@@ -50,16 +52,16 @@
 
     style = dict(
         label='Coating Thermal',
         color='#fe0002',
     )
 
     noises = [
-        CoatingBrownian,
-        CoatingThermoOptic,
+        noise.coatingthermal.CoatingBrownian,
+        noise.coatingthermal.CoatingThermoOptic,
     ]
 
 
 class Substrate(nb.Budget):
     """Substrate Thermal
 
     """
@@ -68,31 +70,31 @@
 
     style = dict(
         label='Substrate Thermal',
         color='#fb7d07',
     )
 
     noises = [
-        SubstrateBrownian,
-        SubstrateThermoElastic,
+        noise.substratethermal.SubstrateBrownian,
+        noise.substratethermal.SubstrateThermoElastic,
     ]
 
 
-class CE2silica(nb.Budget):
+class CE1(nb.Budget):
 
-    name = 'Cosmic Explorer 2 (Silica)'
+    name = 'Cosmic Explorer 1'
 
     noises = [
-        QuantumVacuum,
-        Seismic,
+        Quantum,
+        noise.seismic.Seismic,
         Newtonian,
-        SuspensionThermal,
+        noise.suspensionthermal.SuspensionThermal,
         Coating,
         Substrate,
-        ExcessGas,
+        noise.residualgas.ResidualGas,
     ]
 
     calibrations = [
         Strain,
     ]
 
     plot_style = PLOT_STYLE
```

### Comparing `gwinc-0.4.1/gwinc/ifo/CE2silica/ifo.yaml` & `gwinc-0.5.0/gwinc/ifo/CE2silica/ifo.yaml`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/ifo/CE2silicon/ifo.yaml` & `gwinc-0.5.0/gwinc/ifo/CE2silicon/ifo.yaml`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/ifo/Voyager/ifo.yaml` & `gwinc-0.5.0/gwinc/ifo/Voyager/ifo.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -366,17 +366,17 @@
   Type: 'Freq Dependent'
   AmplitudedB: 10                  # SQZ amplitude [dB]
   InjectionLoss: 0.05              # power loss to sqz
   SQZAngle: 0                      # SQZ phase [radians]
 
   # Parameters for frequency dependent squeezing
   FilterCavity:
-    fdetune: -25      # detuning [Hz] zz['x'][0][1]
+    fdetune: -27.3    # detuning [Hz] zz['x'][0][1]
     L: 300            # cavity length [m]
-    Ti: 6.15e-4       # input mirror transmission [Power] zz['x'][0][2]
+    Ti: 6.88e-4       # input mirror transmission [Power] zz['x'][0][2]
     Te: 0e-6          # end mirror transmission
     Lrt: 10e-6        # round-trip loss in the cavity
     Rot: 0            # phase rotation after cavity
 
   ## Variational Output Parameters
   # Define the output filter cavity chain
   #   None = ignore the output filter settings
```

### Comparing `gwinc-0.4.1/gwinc/ifo/__init__.py` & `gwinc-0.5.0/gwinc/ifo/__init__.py`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/ifo/__main__.py` & `gwinc-0.5.0/gwinc/ifo/__main__.py`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/ifo/aLIGO/ifo.yaml` & `gwinc-0.5.0/gwinc/ifo/aLIGO/ifo.yaml`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/io.py` & `gwinc-0.5.0/gwinc/io.py`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/nb.py` & `gwinc-0.5.0/gwinc/nb.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import itertools
 import collections
 import numpy as np
 import scipy.interpolate
 
 from . import logger
 from .trace import BudgetTrace
+from .struct import Struct
 
 
 def precomp(*precomp_funcs, **precomp_fmaps):
     """BudgetItem.calc decorator to add pre-computed functions
 
     This is intended to decorate BudgetItem.calc() methods with common
     functions whose return value are cached for later use.  The
@@ -70,26 +71,85 @@
 
     kwargs = {
         name: _precomp[pc_func] for name, pc_func in getattr(func, '_precomp_mapped', {}).items()
     }
     return kwargs
 
 
+def list_or_dict_iter(list_or_dict, return_items=False):
+    """Iterator over elements of a list or values of a dict or Struct
+
+    If return_items is True, the items instead of values of a dict or
+    struct are returned
+    """
+    if isinstance(list_or_dict, list):
+        return list_or_dict
+    elif isinstance(list_or_dict, (dict, Struct)):
+        if return_items:
+            return list_or_dict.items()
+        else:
+            return list_or_dict.values()
+    else:
+        raise ValueError('Input should be either a list, dict, or Struct')
+
+
 def quadsum(data):
     """Calculate quadrature sum of list of data arrays.
 
     Provided data are assumed to be power-referred, so this is a
     simple point-by-point sum.
 
     NaNs in sum elements do not contribute to sum.
 
     """
     return np.nansum(data, 0)
 
 
+def _forward_noises(noises, subbudgets):
+    """Extract noises and calibrations from a list of sub-budgets
+
+    Useful for forwarding a list of noises in a sub-budget into an upper level
+    budget. This then groups the noises in the upper level budget without
+    having to analyze the sub-budgets independently.
+
+    Parameters
+    ----------
+    noises : list or dict of Noises
+    subbudgets : list or dict of Budgets
+      List of the sub-budgets whose noises will be forwarded.
+
+    The noises and their calibrations in subbudgets are added to noises
+    """
+    if not isinstance(subbudgets, (list, dict)):
+        raise ValueError('Only lists and dicts can be forwarded')
+
+    for budget in list_or_dict_iter(subbudgets, return_items=True):
+        if isinstance(subbudgets, dict):
+            bname, budget = budget
+        if not isinstance(budget, (tuple, list)):
+            budget = (budget,)
+        b = budget[0]
+        cals = tuple(budget[1:])
+        cals += tuple(b.calibrations)
+
+        if isinstance(subbudgets, list):
+            noises_frwd = [
+                n + cals if isinstance(n, (tuple, list))
+                else (n,) + cals for n in b.noises
+            ]
+            noises.extend(noises_frwd)
+
+        elif isinstance(subbudgets, dict):
+            noises_frwd = {
+                k: n + cals if isinstance(n, (tuple, list))
+                else (n,) + cals for k, n in b.noises.items()
+            }
+            noises.update(noises_frwd)
+
+
 class BudgetItem:
     """GWINC BudgetItem class
 
     """
     def load(self):
         """Overload method for initial loading of static data.
 
@@ -135,28 +195,41 @@
         If not provided, then a pre-defined `freq` attribute of the
         BudgetItem class should exist.
 
         Additional keyword arguments are written as attribute
         variables to the initialized object.
 
         """
-        if freq is not None:
-            assert isinstance(freq, np.ndarray)
-            self.freq = freq
+        assert isinstance(freq, np.ndarray) or freq is None
+        self._freq = freq
         self.ifo = None
         for key, val in kwargs.items():
             setattr(self, key, val)
         self._loaded = False
         self._precomp = dict()
 
     @property
     def name(self):
         """"Name of this BudgetItem class."""
         return self.__class__.__name__
 
+    @property
+    def freq(self):
+        """Frequency array [Hz]"""
+        return self._freq
+
+    @freq.setter
+    def freq(self, val):
+        assert isinstance(val, np.ndarray)
+        # clear the precomp cache
+        self._precomp = dict()
+        # use update instead of setting _freq directly so that Budget.update
+        # recurses through all cal_objs and noise_objs
+        self.update(_freq=val)
+
     def __str__(self):
         # FIXME: provide info on internal state (load/update/calc/etc.)
         return '<{} {}>'.format(
             ', '.join([c.__name__ for c in self.__class__.__bases__]),
             self.name,
         )
 
@@ -267,15 +340,15 @@
                 ifo._orig_keys = tuple(k for k, v in ifo.walk())
                 ifo_hash = ifo.hash()
                 kwargs['ifo'] = ifo
             else:
                 ifo_hash = ifo.hash(ifo._orig_keys)
                 if ifo_hash != getattr(self, '_ifo_hash', 0):
                     logger.debug("ifo hash change")
-                    kwargs['ifo'] = self.ifo
+                    kwargs['ifo'] = ifo
             self._ifo_hash = ifo_hash
 
         if kwargs:
             self.update(**kwargs)
             # clear precomp cache
             self._precomp = dict()
 
@@ -322,14 +395,19 @@
     initialization argument to sub noises.
 
     """
 
     noises = []
     """List of constituent noise classes, or (noise, cal) tuples"""
 
+    noises_forward = []
+    """List of constituent noise classes, or (noise, cal) tuples.
+    These are not saved in a sub-budget, but applied into this budget directly.
+    """
+
     calibrations = []
     """List of calibrations to be applied to all budget noises (not references)"""
 
     references = []
     """List of reference noise classes, or (ref, cal) tuples"""
 
     accumulate = quadsum
@@ -349,15 +427,15 @@
         # store kwargs for later use
         self.kwargs = kwargs
         # record the frequency array as a kwarg if it's definied as a
         # class attribute
         if freq is not None:
             self.kwargs['freq'] = freq
         else:
-            self.kwargs['freq'] = getattr(self, 'freq', None)
+            self.kwargs['freq'] = getattr(self, '_freq', None)
         # FIXME: special casing the ifo kwarg here, in case it's
         # defined as a class attribute rather than passed at
         # initialization.  we do this because we're not defining a
         # standard way to extract IFO variables that get passed around
         # in a reasonable way.  how can we clarify this?
         if 'ifo' not in kwargs and getattr(self, 'ifo', None):
             self.kwargs['ifo'] = getattr(self, 'ifo', None)
@@ -365,24 +443,25 @@
         self._noise_objs = collections.OrderedDict()
         # all cal objects keyed by name
         self._cal_objs = {}
         # set of calibration names to apply to noise
         self._noise_cals = collections.defaultdict(set)
         # set of all constituent budget noise names
         self._budget_noises = set()
+        _forward_noises(self.noises, self.noises_forward)
         # initialize all noise objects
-        for nc in self.noises:
+        for nc in list_or_dict_iter(self.noises):
             name = self.__init_noise(nc, noises)
             if name:
                 self._budget_noises.add(name)
         # initialize common calibrations and add to all budget noises
-        for cal in self.calibrations:
+        for cal in list_or_dict_iter(self.calibrations):
             self.__add_calibration(cal, self._budget_noises)
         # initialize references, without common calibrations
-        for nc in self.references:
+        for nc in list_or_dict_iter(self.references):
             self.__init_noise(nc, noises)
         # error if requested noise is not present
         if noises:
             sset = set(noises)
             nset = set([name for name in self._noise_objs.keys()])
             if not sset <= nset:
                 raise AttributeError("unknown noise terms: {}".format(' '.join(sset-nset)))
@@ -494,15 +573,15 @@
         """Load all noise and cal objects."""
         for name, item in itertools.chain(
                 self._cal_objs.items(),
                 self._noise_objs.items()):
             logger.debug("load {}".format(item))
             item.load()
 
-    def update(self, _precomp=None, **kwargs):
+    def update(self, **kwargs):
         """Recursively update all noise and cal objects with supplied kwargs.
 
         See BudgetItem.update() for more info.
 
         """
         for key, val in kwargs.items():
             setattr(self, key, val)
```

### Comparing `gwinc-0.4.1/gwinc/noise/coatingthermal.py` & `gwinc-0.5.0/gwinc/noise/coatingthermal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,68 @@
 '''Functions to calculate coating thermal noise
 
 '''
 from __future__ import division, print_function
 import numpy as np
 from numpy import pi, exp, real, imag, sqrt, sin, cos, sinh, cosh, ceil, log
+import copy
 
 from .. import const
 from ..const import BESSEL_ZEROS as zeta
 from ..const import J0M as j0m
+from .. import nb
+from ..ifo.noises import arm_cavity
+
+
+class CoatingBrownian(nb.Noise):
+    """Coating Brownian
+
+    """
+    style = dict(
+        label='Coating Brownian',
+        color='#fe0002',
+    )
+
+    def calc(self):
+        ITM = mirror_struct(self.ifo, 'ITM')
+        ETM = mirror_struct(self.ifo, 'ETM')
+        cavity = arm_cavity(self.ifo)
+        wavelength = self.ifo.Laser.Wavelength
+        nITM = coating_brownian(
+            self.freq, ITM, wavelength, cavity.wBeam_ITM
+        )
+        nETM = coating_brownian(
+            self.freq, ETM, wavelength, cavity.wBeam_ETM
+        )
+        return (nITM + nETM) * 2
+
+
+class CoatingThermoOptic(nb.Noise):
+    """Coating Thermo-Optic
+
+    """
+    style = dict(
+        label='Coating Thermo-Optic',
+        color='#02ccfe',
+        linestyle='--',
+    )
+
+    def calc(self):
+        wavelength = self.ifo.Laser.Wavelength
+        materials = self.ifo.Materials
+        ITM = mirror_struct(self.ifo, 'ITM')
+        ETM = mirror_struct(self.ifo, 'ETM')
+        cavity = arm_cavity(self.ifo)
+        nITM, _, _, _ = coating_thermooptic(
+            self.freq, ITM, wavelength, cavity.wBeam_ITM,
+        )
+        nETM, _, _, _ = coating_thermooptic(
+            self.freq, ETM, wavelength, cavity.wBeam_ETM,
+        )
+        return (nITM + nETM) * 2
 
 
 def coating_brownian(f, mirror, wavelength, wBeam, power=None):
     """Coating brownian noise for a given collection of coating layers
 
     This function calculates Coating Brownian noise using
     Hong et al . PRD 87, 082001 (2013).
@@ -1024,7 +1075,32 @@
             def Philown(f):
                 return coat.Philown * (f / 100)**coat.Philown_slope
             lossBlown = lossSlown = Philown
         else:
             lossBlown = lossSlown = lambda f: coat.Philown
 
     return lossBhighn, lossShighn, lossBlown, lossSlown
+
+
+def mirror_struct(ifo, tm):
+    """Create a "mirror" Struct for a LIGO core optic
+
+    This is a copy of the ifo.Materials Struct, containing Substrate
+    and Coating sub-Structs, as well as some basic geometrical
+    properties of the optic.
+
+    """
+    # NOTE: we deepcopy this struct since we'll be modifying it (and
+    # it would otherwise be stored by reference)
+    mirror = copy.deepcopy(ifo.Materials)
+    optic = ifo.Optics.get(tm)
+    if 'CoatLayerOpticalThickness' in optic:
+        mirror.Coating.dOpt = optic['CoatLayerOpticalThickness']
+    else:
+        T = optic.Transmittance
+        dL = optic.CoatingThicknessLown
+        dCap = optic.CoatingThicknessCap
+        mirror.Coating.dOpt = getCoatDopt(mirror, T, dL, dCap=dCap)
+    mirror.update(optic)
+    mirror.MassVolume = pi * mirror.MassRadius**2 * mirror.MassThickness
+    mirror.MirrorMass = mirror.MassVolume * mirror.Substrate.MassDensity
+    return mirror
```

### Comparing `gwinc-0.4.1/gwinc/noise/newtonian.py` & `gwinc-0.5.0/gwinc/noise/newtonian.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,72 @@
 import numpy as np
 from numpy import pi, sqrt, exp, log10
 import scipy.integrate as scint
 import scipy.special as sp
 
 from .seismic import seismic_ground_NLNM
 from .. import const
+from .. import nb
+
+
+class Newtonian(nb.Noise):
+    """Newtonian Gravity
+
+    """
+    style = dict(
+        label='Newtonian Gravity',
+        color='#15b01a',
+    )
+
+    def calc(self):
+        n = gravg(self.freq, self.ifo.Seismic)
+        return n * 4
+
+
+class Rayleigh(nb.Noise):
+    """Newtonian Gravity, Rayleigh waves
+
+    """
+    style = dict(
+        label='Rayleigh waves',
+        color='#1b2431',
+    )
+
+    def calc(self):
+        n = gravg_rayleigh(self.freq, self.ifo.Seismic)
+        return n * 2
+
+
+class Body(nb.Noise):
+    """Newtonian Gravity, body waves
+
+    """
+    style = dict(
+        label='Body waves',
+        color='#85a3b2',
+    )
+
+    def calc(self):
+        np = gravg_pwave(self.freq, self.ifo.Seismic)
+        ns = gravg_swave(self.freq, self.ifo.Seismic)
+        return (np + ns) * 4
+
+
+class Infrasound(nb.Noise):
+    """Newtonian Gravity, infrasound
+
+    """
+    style = dict(
+        label='Infrasound)',
+        color='#ffa62b',
+    )
+
+    def calc(self):
+        n = atmois(self.freq, self.ifo.Atmospheric, self.ifo.Seismic)
+        return n * 2
 
 
 def gravg(f, seismic):
     """Gravity gradient noise for single test mass
 
     :f: frequency array in Hz
     :seismic: gwinc Seismic struct
```

### Comparing `gwinc-0.4.1/gwinc/noise/quantum.py` & `gwinc-0.5.0/gwinc/noise/quantum.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,21 +6,179 @@
 from numpy import pi, sqrt, arctan, sin, cos, exp, log10, conj
 from copy import deepcopy
 from collections.abc import Sequence
 
 from .. import logger
 from .. import const
 from ..struct import Struct
+from .. import nb
+from ..suspension import precomp_suspension
 
 
-def sqzOptimalSqueezeAngle(Mifo, eta):
-    vHD = np.array([[sin(eta), cos(eta)]])
-    H = getProdTF(vHD, Mifo)[0]
-    alpha = arctan(abs(H[1]), abs(H[0]))
-    return alpha
+@nb.precomp(sustf=precomp_suspension)
+def precomp_quantum(f, ifo, sustf):
+    from ..ifo import noises
+    pc = Struct()
+    power = noises.ifo_power(ifo)
+    noise_dict = shotrad(f, ifo, sustf, power)
+    pc.ASvac = noise_dict['ASvac']
+    pc.SEC = noise_dict['SEC']
+    pc.Arm = noise_dict['arm']
+    pc.Injection = noise_dict['injection']
+    pc.PD = noise_dict['pd']
+
+    # FC0 are the noises from the filter cavity losses and FC0_unsqzd_back
+    # are noises from the unsqueezed vacuum injected at the back mirror
+    # Right now there are at most one filter cavity in all the models;
+    # if there were two, there would also be FC1 and FC1_unsqzd_back, etc.
+    # keys = list(noise_dict.keys())
+    fc_keys = [key for key in noise_dict.keys() if 'FC' in key]
+    pc.FC = np.zeros_like(pc.ASvac)
+    if fc_keys:
+        for key in fc_keys:
+            pc.FC += noise_dict[key]
+
+    if 'phase' in noise_dict.keys():
+        pc.Phase = noise_dict['phase']
+
+    if 'ofc' in noise_dict.keys():
+        pc.OFC = noise_dict['OFC']
+
+    return pc
+
+
+
+class QuantumVacuum(nb.Noise):
+    """Quantum Vacuum
+
+    """
+    style = dict(
+        label='Quantum Vacuum',
+        color='#ad03de',
+    )
+
+    @nb.precomp(quantum=precomp_quantum)
+    def calc(self, quantum):
+        total = np.zeros_like(quantum.ASvac)
+        for nn in quantum.values():
+            total += nn
+        return total
+
+
+class AS(nb.Noise):
+    """Quantum vacuum from the AS port
+
+    """
+    style = dict(
+        label='AS Port Vacuum',
+        color='xkcd:emerald green'
+    )
+
+    @nb.precomp(quantum=precomp_quantum)
+    def calc(self, quantum):
+        return quantum.ASvac
+
+
+class Arm(nb.Noise):
+    """Quantum vacuum due to arm cavity loss
+
+    """
+    style = dict(
+        label='Arm Loss',
+        color='xkcd:orange brown'
+    )
+
+    @nb.precomp(quantum=precomp_quantum)
+    def calc(self, quantum):
+        return quantum.Arm
+
+
+class SEC(nb.Noise):
+    """Quantum vacuum due to SEC loss
+
+    """
+    style = dict(
+        label='SEC Loss',
+        color='xkcd:cerulean'
+    )
+
+    @nb.precomp(quantum=precomp_quantum)
+    def calc(self, quantum):
+        return quantum.SEC
+
+
+class FilterCavity(nb.Noise):
+    """Quantum vacuum due to filter cavity loss
+
+    """
+    style = dict(
+        label='Filter Cavity Loss',
+        color='xkcd:goldenrod'
+    )
+
+    @nb.precomp(quantum=precomp_quantum)
+    def calc(self, quantum):
+        return quantum.FC
+
+
+class Injection(nb.Noise):
+    """Quantum vacuum due to injection loss
+
+    """
+    style = dict(
+        label='Injection Loss',
+        color='xkcd:fuchsia'
+    )
+
+    @nb.precomp(quantum=precomp_quantum)
+    def calc(self, quantum):
+        return quantum.Injection
+
+
+class Readout(nb.Noise):
+    """Quantum vacuum due to readout loss
+
+    """
+    style = dict(
+        label='Readout Loss',
+        color='xkcd:mahogany'
+    )
+
+    @nb.precomp(quantum=precomp_quantum)
+    def calc(self, quantum):
+        return quantum.PD
+
+
+class QuadraturePhase(nb.Noise):
+    """Quantum vacuum noise due to quadrature phase noise
+    """
+    style = dict(
+        label='Quadrature Phase',
+        color='xkcd:slate'
+    )
+
+    @nb.precomp(quantum=precomp_quantum)
+    def calc(self, quantum):
+        return quantum.Phase
+
+
+class StandardQuantumLimit(nb.Noise):
+    """Standard Quantum Limit
+
+    """
+    style = dict(
+        label="Standard Quantum Limit",
+        color="#000000",
+        linestyle=":",
+    )
+
+    def calc(self):
+        from .coatingthermal import mirror_struct
+        ETM = mirror_struct(self.ifo, 'ETM')
+        return 8 * const.hbar / (ETM.MirrorMass * (2 * np.pi * self.freq) ** 2)
 
 
 def getSqzParams(ifo):
     """Determine squeezer type, if any, and extract common parameters
 
     Returns a struct with the following attributes:
     SQZ_DB: squeezing in dB
@@ -29,22 +187,24 @@
     lambda_in: loss to squeezing before injection [Power]
     etaRMS: quadrature noise [rad]
     eta: homodyne angle [rad]
     """
     params = Struct()
 
     if 'Squeezer' not in ifo:
-        sqzType = None
+        sqzType = 'None'
+    elif ifo.Squeezer.AmplitudedB == 0:
+        sqzType = 'None'
     else:
         sqzType = ifo.Squeezer.get('Type', 'Freq Independent')
 
     params.sqzType = sqzType
 
     # extract squeezer parameters
-    if sqzType is None:
+    if sqzType == 'None':
         params.SQZ_DB = 0
         params.ANTISQZ_DB = 0
         params.alpha = 0
         params.lambda_in = 0
         params.etaRMS = 0
 
     else:
```

### Comparing `gwinc-0.4.1/gwinc/noise/seismic.py` & `gwinc-0.5.0/gwinc/noise/seismic.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,59 @@
 '''Functions to calculate seismic noise in suspended optics.
 
 '''
 from __future__ import division
 import numpy as np
 from scipy.interpolate import PchipInterpolator as interp1d
 
+from .. import nb
+from ..suspension import precomp_suspension
+
+
+def Seismic_constructor(direction):
+    """Seismic noise for a single direction
+
+    """
+    if direction == 'horiz':
+        label = 'Horizontal'
+        color = 'xkcd:muted blue'
+    elif direction == 'vert':
+        label = 'Vertical'
+        color = 'xkcd:brick red'
+
+    class SeismicDirection(nb.Noise):
+        name = label
+        style = dict(
+            label=label,
+            color=color,
+        )
+
+        @nb.precomp(sustf=precomp_suspension)
+        def calc(self, sustf):
+            nt, nr = platform_motion(self.freq, self.ifo)
+            n = seismic_suspension_filtered(sustf, nt, direction)
+            return n * 4
+
+    return SeismicDirection
+
+
+class Seismic(nb.Budget):
+    """Seismic
+
+    """
+    style = dict(
+        label='Seismic',
+        color='#855700',
+    )
+
+    noises = [
+        Seismic_constructor('vert'),
+        Seismic_constructor('horiz'),
+    ]
+
 
 def seismic_suspension_filtered(sustf, in_trans, direction):
     """Seismic displacement noise for single suspended test mass.
 
     :sustf: sus transfer function Struct
     :in_trans: input translational displacement spectrum
     :direction: 'horiz' for horizontal or 'vert' for vertical
```

### Comparing `gwinc-0.4.1/gwinc/noise/substratethermal.py` & `gwinc-0.5.0/gwinc/noise/substratethermal.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,14 +6,73 @@
 from numpy import exp, inf, pi, sqrt
 import scipy.special
 import scipy.integrate
 
 from .. import const
 from ..const import BESSEL_ZEROS as zeta
 from ..const import J0M as j0m
+from .. import nb
+from ..ifo.noises import arm_cavity, ifo_power
+
+
+class ITMThermoRefractive(nb.Noise):
+    """ITM Thermo-Refractive
+
+    """
+    style = dict(
+        label='ITM Thermo-Refractive',
+        color='#448ee4',
+        linestyle='--',
+    )
+
+    def calc(self):
+        power = ifo_power(self.ifo)
+        gPhase = power.finesse * 2/np.pi
+        cavity = arm_cavity(self.ifo)
+        n = substrate_thermorefractive(
+            self.freq, self.ifo.Materials, cavity.wBeam_ITM)
+        return n * 2 / gPhase**2
+
+
+class SubstrateBrownian(nb.Noise):
+    """Substrate Brownian
+
+    """
+    style = dict(
+        label='Substrate Brownian',
+        color='#fb7d07',
+        linestyle='--',
+    )
+
+    def calc(self):
+        cavity = arm_cavity(self.ifo)
+        nITM = substrate_brownian(
+            self.freq, self.ifo.Materials, cavity.wBeam_ITM)
+        nETM = substrate_brownian(
+            self.freq, self.ifo.Materials, cavity.wBeam_ETM)
+        return (nITM + nETM) * 2
+
+
+class SubstrateThermoElastic(nb.Noise):
+    """Substrate Thermo-Elastic
+
+    """
+    style = dict(
+        label='Substrate Thermo-Elastic',
+        color='#f5bf03',
+        linestyle='--',
+    )
+
+    def calc(self):
+        cavity = arm_cavity(self.ifo)
+        nITM = substrate_thermoelastic(
+            self.freq, self.ifo.Materials, cavity.wBeam_ITM)
+        nETM = substrate_thermoelastic(
+            self.freq, self.ifo.Materials, cavity.wBeam_ETM)
+        return (nITM + nETM) * 2
 
 
 def substrate_thermorefractive(f, materials, wBeam, exact=False):
     """Substrate thermal displacement noise spectrum from thermorefractive fluctuations
 
     :f: frequency array in Hz
     :materials: gwinc optic materials structure
```

### Comparing `gwinc-0.4.1/gwinc/noise/suspensionthermal.py` & `gwinc-0.5.0/gwinc/noise/suspensionthermal.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,15 +2,84 @@
 
 '''
 from __future__ import division
 import numpy as np
 from numpy import pi, imag
 
 from ..const import kB
-from ..suspension import getJointParams
+from ..suspension import getJointParams, precomp_suspension
+from .. import nb
+
+
+
+def SuspensionThermal_constructor(stage_num, direction):
+    """Suspension thermal for a single stage in one direction
+
+    """
+    if stage_num == 0:
+        stage_name = 'Top'
+        color = 'xkcd:orangeish'
+    elif stage_num == 1:
+        stage_name = 'UIM'
+        color = 'xkcd:mustard'
+    elif stage_num == 2:
+        stage_name = 'PUM'
+        color = 'xkcd:turquoise'
+    elif stage_num == 3:
+        stage_name = 'Test mass'
+        color = 'xkcd:bright purple'
+
+    if direction == 'horiz':
+        name0 = 'Horiz' + stage_name
+        label = 'Horiz. ' + stage_name
+        linestyle = '-'
+    elif direction == 'vert':
+        name0 = 'Vert' + stage_name
+        label = 'Vert. ' + stage_name
+        linestyle = '--'
+
+    class SuspensionThermalStage(nb.Noise):
+        name = name0
+        style = dict(
+            label=label,
+            color=color,
+            linestyle=linestyle,
+            alpha=0.7,
+        )
+
+        @nb.precomp(sustf=precomp_suspension)
+        def calc(self, sustf):
+            n = susptherm_stage(
+                self.freq, self.ifo.Suspension, sustf, stage_num, direction)
+            return abs(n) * 4
+
+    return SuspensionThermalStage
+
+
+class SuspensionThermal(nb.Budget):
+    """Suspension Thermal
+
+    """
+
+    name = 'SuspensionThermal'
+
+    style = dict(
+        label='Suspension Thermal',
+        color='#0d75f8',
+    )
+
+    noises = [
+        SuspensionThermal_constructor(0, 'horiz'),
+        SuspensionThermal_constructor(1, 'horiz'),
+        SuspensionThermal_constructor(2, 'horiz'),
+        SuspensionThermal_constructor(3, 'horiz'),
+        SuspensionThermal_constructor(0, 'vert'),
+        SuspensionThermal_constructor(1, 'vert'),
+        SuspensionThermal_constructor(2, 'vert'),
+    ]
 
 
 def getJointTempSusceptibility(sus, sustf, stage_num, isUpper, direction):
     """Get the product of the temperature and the susceptibility of a joint
 
     :sus: the suspension struct
     :sustf: suspension transfer function struct
```

### Comparing `gwinc-0.4.1/gwinc/plot.py` & `gwinc-0.5.0/gwinc/plot.py`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/squeeze.py` & `gwinc-0.5.0/gwinc/squeeze.py`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/struct.py` & `gwinc-0.5.0/gwinc/struct.py`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/suspension.py` & `gwinc-0.5.0/gwinc/suspension.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,31 @@
 from __future__ import division
 from numpy import pi, sqrt, sin, cos, tan, real, imag
 import numpy as np
 
 from . import logger
-from .const import g
+from . import const
+from .struct import Struct
+
+
+def precomp_suspension(f, ifo):
+    pc = Struct()
+    pc.VHCoupling = Struct()
+    if 'VHCoupling' in ifo.Suspension:
+        pc.VHCoupling.theta = ifo.Suspension.VHCoupling.theta
+    else:
+        pc.VHCoupling.theta = ifo.Infrastructure.Length / const.R_earth
+    hForce, vForce, hTable, vTable, tst_suscept = suspQuad(
+        f, ifo.Suspension)
+    pc.hForce = hForce
+    pc.vForce = vForce
+    pc.hTable = hTable
+    pc.vTable = vTable
+    pc.tst_suscept = tst_suscept
+    return pc
 
 
 # supported fiber geometries
 FIBER_TYPES = [
     'Round',
     'Ribbon',
     'Tapered',
@@ -410,15 +428,15 @@
     FiberType = sus.FiberType
     assert FiberType in FIBER_TYPES
 
     ##############################
     # Compute cumulative weight of suspension
     masses = np.array([stage.Mass for stage in stages])
     # weight support by lower stages
-    Mgs = g * np.flipud(np.cumsum(np.flipud(masses)))
+    Mgs = const.g * np.flipud(np.cumsum(np.flipud(masses)))
 
     ##############################
     # Complex spring constants
     khr = np.zeros([len(stages), len(w)])
     khi = np.zeros([len(stages), 2, len(w)])
     kvr = np.zeros([len(stages), len(w)])
     kvi = np.zeros([len(stages), 2, len(w)])
```

### Comparing `gwinc-0.4.1/gwinc/test/__main__.py` & `gwinc-0.5.0/gwinc/test/__main__.py`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/test/gen_cache.sh` & `gwinc-0.5.0/gwinc/test/gen_cache.sh`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc/trace.py` & `gwinc-0.5.0/gwinc/trace.py`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/gwinc.egg-info/PKG-INFO` & `gwinc-0.5.0/gwinc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: gwinc
-Version: 0.4.1
+Version: 0.5.0
 Summary: Gravitation Wave Interferometer Noise Calculator
 Home-page: https://git.ligo.org/gwinc/pygwinc
 Author: LIGO Scientific Collaboration
 Author-email: jameson.rollins@ligo.org
 License: UNLICENSE
 Project-URL: Bug Tracker, https://git.ligo.org/gwinc/pygwinc/issues
 Project-URL: Source Code, https://git.ligo.org/gwinc/pygwinc
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Intended Audience :: Science/Research
@@ -178,16 +177,16 @@
 in the specified budget module (see [budget
 interface](#budget-interface) below).  The budget `ifo` `gwinc.Struct`
 is available in the `budget.ifo` attribute.
 
 The budget `run()` method calculates all budget noises and the noise
 total and returns a `BudgetTrace` object with `freq`, `psd`, and `asd`
 properties.  The budget sub-traces are available through a dictionary
-(`trace['QuantumVacuum']`) interface and via attributes
-(`trace.QuantumVacumm`).
+(`trace['Quantum']`) interface and via attributes
+(`trace.Quantum`).
 
 The budget `freq` and `ifo` attributes can be updated at run time by
 passing them as keyword arguments to the `run()` method:
 ```python
 >>> budget = load_budget('aLIGO')
 >>> freq = np.logspace(1, 3, 1000)
 >>> ifo = Struct.from_file('/path/to/ifo_alt.yaml')
@@ -463,29 +462,29 @@
 There are various way to extract single noise terms from the Budget
 interface.  The most straightforward way is to run the full budget,
 and extract the noise data the output traces dictionary:
 
 ```python
 budget = load_budget('/path/to/MyBudget', freq)
 trace = budget.run()
-quantum_trace = trace['QuantumVacuum']
+quantum_trace = trace['Quantum']
 ```
 
 You can also calculate the final calibrated output noise for just a
 single term using the Budget `calc_noise()` method:
 ```python
-data = budget.calc_noise('QuantumVacuum')
+data = budget.calc_noise('Quantum')
 ```
 
 You can also calculate a noise at it's source, without applying any
 calibrations, by using the Budget `__getitem__` interface to extract
 the specific Noise BudgetItem for the noise you're interested in, and
-running it's `calc()` method directly:
+running it's `calc_trace()` method directly:
 ```python
-data = budget['QuantumVacuum'].calc()
+data = budget['Quantum'].calc_trace()
 ```
 
 
 # inspiral range
 
 The [`inspiral_range`](https://git.ligo.org/gwinc/inspiral-range)
 package can be used to calculate various common "inspiral range"
@@ -530,9 +529,7 @@
 <!-- This will produce a summary page of the various noise spectra that -->
 <!-- differ between matgwinc and pygwinc. -->
 
 <!-- Latest comparison plots from continuous integration: -->
 
 <!-- * [aLIGO comparison](https://gwinc.docs.ligo.org/pygwinc/aLIGO_test.png) -->
 <!-- * [A+ comparison](https://gwinc.docs.ligo.org/pygwinc/A+_test.png) -->
-
-
```

### Comparing `gwinc-0.4.1/gwinc.egg-info/SOURCES.txt` & `gwinc-0.5.0/gwinc.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -49,17 +49,29 @@
 gwinc/noise/residualgas.py
 gwinc/noise/seismic.py
 gwinc/noise/substratethermal.py
 gwinc/noise/suspensionthermal.py
 gwinc/test/__init__.py
 gwinc/test/__main__.py
 gwinc/test/gen_cache.sh
-gwinc/test/test_io.py
-gwinc/test/test_nb.py
-gwinc/test/test_struct.py
 test/budgets/test_budgets.py
+test/budgets/H1/__init__.py
+test/budgets/H1/ifo.yaml
+test/budgets/H1/lho_o3.txt
+test/budgets/H1/lho_ref.txt
 test/inherit/Aplus_mod.yaml
 test/inherit/Aplus_mod2.yaml
+test/inherit/Aplus_mod3.yaml
 test/inherit/inherit_fail.yaml
+test/inherit/new_ifo.txt
+test/inherit/new_ifo.yaml
 test/inherit/test_inherit.py
+test/inherit/subdir/CustomBudget_mod.yaml
+test/inherit/subdir/CustomBudget/__init__.py
+test/inherit/subdir/CustomBudget/ifo.yaml
+test/noises/test_quantum.py
+test/noises/residualgas/test_residualgas.py
+test/noises/residualgas/AplusSuperGas/__init__.py
+test/noises/residualgas/AplusSuperGas/beamtube_pressure.txt
+test/noises/residualgas/AplusSuperGas/ifo.yaml
 test/struct/test_load.yml
 test/struct/test_struct.py
```

### Comparing `gwinc-0.4.1/setup.cfg` & `gwinc-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `gwinc-0.4.1/test/struct/test_struct.py` & `gwinc-0.5.0/test/struct/test_struct.py`

 * *Files identical despite different names*

