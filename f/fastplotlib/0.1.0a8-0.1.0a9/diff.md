# Comparing `tmp/fastplotlib-0.1.0a8.tar.gz` & `tmp/fastplotlib-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastplotlib-0.1.0a8.tar", last modified: Fri Jan 13 04:22:20 2023, max compression
+gzip compressed data, was "fastplotlib-0.1.0a9.tar", last modified: Thu Mar  9 07:35:47 2023, max compression
```

## Comparing `fastplotlib-0.1.0a8.tar` & `fastplotlib-0.1.0a9.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:22:20.005640 fastplotlib-0.1.0a8/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-01-13 04:22:20.005640 fastplotlib-0.1.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:22:19.977637 fastplotlib-0.1.0a8/fastplotlib/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:22:19.981637 fastplotlib-0.1.0a8/fastplotlib/graphics/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:22:19.981637 fastplotlib-0.1.0a8/fastplotlib/graphics/features/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/features/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/features/_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/features/_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/features/_present.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/features/_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/features/_thickness.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/line_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/line_slider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/graphics/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:22:19.981637 fastplotlib-0.1.0a8/fastplotlib/layouts/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/layouts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/layouts/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/layouts/_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/layouts/_gridplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12440 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/layouts/_subplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:22:19.985638 fastplotlib-0.1.0a8/fastplotlib/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:22:20.005640 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Accent
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Blues
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/BrBG
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/BuGn
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/BuPu
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/CMRmap
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Dark2
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/GnBu
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Greens
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Greys
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/OrRd
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Oranges
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/PRGn
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Paired
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Pastel1
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Pastel2
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/PiYG
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/PuBu
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/PuBuGn
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/PuOr
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/PuRd
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Purples
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/RdBu
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/RdGy
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/RdPu
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/RdYlBu
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/RdYlGn
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Reds
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Set1
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Set2
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Set3
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Spectral
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Wistia
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/YlGn
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/YlGnBu
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/YlOrBr
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/YlOrRd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/afmhot
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/autumn
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/binary
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/bone
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/brg
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/bwr
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/cividis
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/cool
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/coolwarm
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/copper
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/cubehelix
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/flag
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gist_earth
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gist_gray
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gist_heat
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gist_ncar
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gist_rainbow
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gist_stern
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gist_yarg
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gnuplot
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gnuplot2
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gray
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/hot
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/hsv
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/inferno
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/jet
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/magma
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/nipy_spectral
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/ocean
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/pink
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/plasma
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/prism
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/rainbow
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/seismic
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/spring
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:07.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/summer
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/tab10
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/tab20
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/tab20b
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/tab20c
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/terrain
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/turbo
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/twilight
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/twilight_shifted
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/viridis
--rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/winter
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/fastplotlib/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/fastplotlib/utils/generate_colormaps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:22:20.005640 fastplotlib-0.1.0a8/fastplotlib/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/fastplotlib/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32195 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/fastplotlib/widgets/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-13 04:22:19.977637 fastplotlib-0.1.0a8/fastplotlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-01-13 04:22:19.000000 fastplotlib-0.1.0a8/fastplotlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-01-13 04:22:19.000000 fastplotlib-0.1.0a8/fastplotlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-13 04:22:19.000000 fastplotlib-0.1.0a8/fastplotlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-01-13 04:22:19.000000 fastplotlib-0.1.0a8/fastplotlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-13 04:22:19.000000 fastplotlib-0.1.0a8/fastplotlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-13 04:22:20.005640 fastplotlib-0.1.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-01-13 04:22:08.000000 fastplotlib-0.1.0a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:35:47.134887 fastplotlib-0.1.0a9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-03-09 07:35:47.130887 fastplotlib-0.1.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:35:47.118888 fastplotlib-0.1.0a9/fastplotlib/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:35:47.118888 fastplotlib-0.1.0a9/fastplotlib/graphics/
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16682 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:35:47.118888 fastplotlib-0.1.0a9/fastplotlib/graphics/features/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7289 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/features/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/features/_colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6532 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/features/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/features/_present.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/features/_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/features/_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12851 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/line_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/line_slider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/graphics/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:35:47.118888 fastplotlib-0.1.0a9/fastplotlib/layouts/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/layouts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/layouts/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/layouts/_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/layouts/_gridplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/layouts/_subplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:35:47.122887 fastplotlib-0.1.0a9/fastplotlib/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:35:47.130887 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Accent
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Blues
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/BrBG
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/BuGn
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/BuPu
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/CMRmap
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Dark2
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/GnBu
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Greens
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Greys
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/OrRd
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Oranges
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/PRGn
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Paired
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Pastel1
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Pastel2
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/PiYG
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/PuBu
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/PuBuGn
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/PuOr
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/PuRd
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Purples
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/RdBu
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/RdGy
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/RdPu
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/RdYlBu
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/RdYlGn
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Reds
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Set1
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Set2
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Set3
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Spectral
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Wistia
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/YlGn
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/YlGnBu
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/YlOrBr
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/YlOrRd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/afmhot
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/autumn
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/binary
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/bone
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/brg
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/bwr
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/cividis
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/cool
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/coolwarm
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/copper
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/cubehelix
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/flag
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gist_earth
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gist_gray
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gist_heat
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gist_ncar
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gist_rainbow
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gist_stern
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gist_yarg
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gnuplot
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gnuplot2
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gray
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/hot
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/hsv
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/inferno
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/jet
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/magma
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/nipy_spectral
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/ocean
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/pink
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/plasma
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/prism
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/rainbow
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/seismic
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/spring
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/summer
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/tab10
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/tab20
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/tab20b
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/tab20c
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/terrain
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/turbo
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/twilight
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/twilight_shifted
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/viridis
+-rw-r--r--   0 runner    (1001) docker     (123)    25600 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/winter
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/utils/generate_colormaps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:35:47.130887 fastplotlib-0.1.0a9/fastplotlib/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33458 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/fastplotlib/widgets/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:35:47.118888 fastplotlib-0.1.0a9/fastplotlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-03-09 07:35:47.000000 fastplotlib-0.1.0a9/fastplotlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-03-09 07:35:47.000000 fastplotlib-0.1.0a9/fastplotlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 07:35:47.000000 fastplotlib-0.1.0a9/fastplotlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-03-09 07:35:47.000000 fastplotlib-0.1.0a9/fastplotlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-09 07:35:47.000000 fastplotlib-0.1.0a9/fastplotlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 07:35:47.134887 fastplotlib-0.1.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-09 07:35:37.000000 fastplotlib-0.1.0a9/setup.py
```

### Comparing `fastplotlib-0.1.0a8/LICENSE` & `fastplotlib-0.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/PKG-INFO` & `fastplotlib-0.1.0a9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 Metadata-Version: 2.1
 Name: fastplotlib
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: A fast plotting library built using the pygfx render engine
 Home-page: https://github.com/kushalkolar/fastplotlib
 Author: Kushal Kolar
 Author-email: 
 License: Apache 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fastplotlib
-[![PyPI version](https://badge.fury.io/py/fastplotlib.svg)](https://badge.fury.io/py/fastplotlib) [![Gitter](https://badges.gitter.im/fastplotlib/community.svg)](https://gitter.im/fastplotlib/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+[![PyPI version](https://badge.fury.io/py/fastplotlib.svg)](https://badge.fury.io/py/fastplotlib)
+[![Documentation Status](https://readthedocs.org/projects/fastplotlib/badge/?version=latest)](https://fastplotlib.readthedocs.io/en/latest/?badge=latest)
+[![Gitter](https://badges.gitter.im/fastplotlib/community.svg)](https://gitter.im/fastplotlib/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
 [**Installation**](https://github.com/kushalkolar/fastplotlib#installation) | [**GPU Drivers**](https://github.com/kushalkolar/fastplotlib#install-vulkan-drivers) | [**Examples**](https://github.com/kushalkolar/fastplotlib#examples)
 
 A fast plotting library built using the [`pygfx`](https://github.com/pygfx/pygfx) render engine utilizing [Vulkan](https://en.wikipedia.org/wiki/Vulkan) via WGPU, so it is very fast! `fastplotlib` is focussed on very fast interactive plotting in the notebook using an expressive API. It also works within desktop applications using `glfw` or `Qt`.
 
 `fastplotlib` is currently in the **early alpha stage with breaking changes every ~week**, but you're welcome to try it out or contribute! See our [Roadmap for 2023](https://github.com/kushalkolar/fastplotlib/issues/55).
 
+**Documentation**: http://fastplotlib.readthedocs.io/ 
+
+The docs are not entirely thorough, we recommend the example notebooks to get started.
+
 Questions, ideas? Post an issue or [chat on gitter](https://gitter.im/fastplotlib/community?utm_source=share-link&utm_medium=link&utm_campaign=share-link).
 
 ![epic](https://user-images.githubusercontent.com/9403332/210304473-f36f2aaf-319e-435b-bcc8-0e8d3e1ef282.gif)
 
 # Examples
 
 **See the examples directory. Start out with `simple.ipynb`.**
@@ -119,15 +125,15 @@
 jupyter lab
 ```
 
 ## Install Vulkan drivers
 
 You will need a GPU that supports Vulkan (integrated GPUs in CPUs are usually fine). Generally if your GPU is from 2017 or later it should support Vulkan.
 
-For more information see: https://github.com/pygfx/wgpu-py#platform-requirements
+For more information see: https://wgpu-py.readthedocs.io/en/stable/start.html#platform-requirements
 
 ### Windows:
 Vulkan should be installed by default on Windows 11, but you will need to install your GPU manufacturer's driver package (Nvidia or AMD). If you have an integrated GPU within your CPU, you might still need to install a driver package too, check your CPU manufacturer's info. We recommend installing C compilers so that you can install `simplejpeg` which improves remote frame buffer performance in notebooks.
 
 ### Linux:
 Debian based distros:
```

### Comparing `fastplotlib-0.1.0a8/README.md` & `fastplotlib-0.1.0a9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 # fastplotlib
-[![PyPI version](https://badge.fury.io/py/fastplotlib.svg)](https://badge.fury.io/py/fastplotlib) [![Gitter](https://badges.gitter.im/fastplotlib/community.svg)](https://gitter.im/fastplotlib/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+[![PyPI version](https://badge.fury.io/py/fastplotlib.svg)](https://badge.fury.io/py/fastplotlib)
+[![Documentation Status](https://readthedocs.org/projects/fastplotlib/badge/?version=latest)](https://fastplotlib.readthedocs.io/en/latest/?badge=latest)
+[![Gitter](https://badges.gitter.im/fastplotlib/community.svg)](https://gitter.im/fastplotlib/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
 [**Installation**](https://github.com/kushalkolar/fastplotlib#installation) | [**GPU Drivers**](https://github.com/kushalkolar/fastplotlib#install-vulkan-drivers) | [**Examples**](https://github.com/kushalkolar/fastplotlib#examples)
 
 A fast plotting library built using the [`pygfx`](https://github.com/pygfx/pygfx) render engine utilizing [Vulkan](https://en.wikipedia.org/wiki/Vulkan) via WGPU, so it is very fast! `fastplotlib` is focussed on very fast interactive plotting in the notebook using an expressive API. It also works within desktop applications using `glfw` or `Qt`.
 
 `fastplotlib` is currently in the **early alpha stage with breaking changes every ~week**, but you're welcome to try it out or contribute! See our [Roadmap for 2023](https://github.com/kushalkolar/fastplotlib/issues/55).
 
+**Documentation**: http://fastplotlib.readthedocs.io/ 
+
+The docs are not entirely thorough, we recommend the example notebooks to get started.
+
 Questions, ideas? Post an issue or [chat on gitter](https://gitter.im/fastplotlib/community?utm_source=share-link&utm_medium=link&utm_campaign=share-link).
 
 ![epic](https://user-images.githubusercontent.com/9403332/210304473-f36f2aaf-319e-435b-bcc8-0e8d3e1ef282.gif)
 
 # Examples
 
 **See the examples directory. Start out with `simple.ipynb`.**
@@ -107,15 +113,15 @@
 jupyter lab
 ```
 
 ## Install Vulkan drivers
 
 You will need a GPU that supports Vulkan (integrated GPUs in CPUs are usually fine). Generally if your GPU is from 2017 or later it should support Vulkan.
 
-For more information see: https://github.com/pygfx/wgpu-py#platform-requirements
+For more information see: https://wgpu-py.readthedocs.io/en/stable/start.html#platform-requirements
 
 ### Windows:
 Vulkan should be installed by default on Windows 11, but you will need to install your GPU manufacturer's driver package (Nvidia or AMD). If you have an integrated GPU within your CPU, you might still need to install a driver package too, check your CPU manufacturer's info. We recommend installing C compilers so that you can install `simplejpeg` which improves remote frame buffer performance in notebooks.
 
 ### Linux:
 Debian based distros:
```

### Comparing `fastplotlib-0.1.0a8/fastplotlib/graphics/features/_base.py` & `fastplotlib-0.1.0a9/fastplotlib/graphics/features/_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,44 @@
 from abc import ABC, abstractmethod
 from inspect import getfullargspec
 from warnings import warn
 from typing import *
 
 import numpy as np
-from pygfx import Buffer
+from pygfx import Buffer, Texture
+
+
+supported_dtypes = [
+    np.uint8,
+    np.uint16,
+    np.uint32,
+    np.int8,
+    np.int16,
+    np.int32,
+    np.float16,
+    np.float32
+]
+
+
+def to_gpu_supported_dtype(array):
+    """
+    If ``array`` is a numpy array, converts it to a supported type. GPUs don't support 64 bit dtypes.
+    """
+    if isinstance(array, np.ndarray):
+        if array.dtype not in supported_dtypes:
+            if np.issubdtype(array.dtype, np.integer):
+                warn(f"converting {array.dtype} array to int32")
+                return array.astype(np.int32)
+            elif np.issubdtype(array.dtype, np.floating):
+                warn(f"converting {array.dtype} array to float32")
+                return array.astype(np.float32, copy=False)
+            else:
+                raise TypeError("Unsupported type, supported array types must be int or float dtypes")
+
+    return array
 
 
 class FeatureEvent:
     """
     type: <feature_name>, example: "colors"
     pick_info: dict in the form:
         {
@@ -38,18 +68,16 @@
         data: Any
 
         collection_index: int
             if part of a collection, index of this graphic within the collection
 
         """
         self._parent = parent
-        if isinstance(data, np.ndarray):
-            data = data.astype(np.float32)
 
-        self._data = data
+        self._data = to_gpu_supported_dtype(data)
 
         self._collection_index = collection_index
         self._event_handlers = list()
         self._block_events = False
 
     def __call__(self, *args, **kwargs):
         return self._data
@@ -194,36 +222,37 @@
 
     @abstractmethod
     def _update_range(self, key):
         pass
 
     @property
     @abstractmethod
-    def _buffer(self) -> Buffer:
+    def buffer(self) -> Union[Buffer, Texture]:
         pass
 
     @property
     def _upper_bound(self) -> int:
         return self._data.shape[0]
 
     def _update_range_indices(self, key):
         """Currently used by colors and positions data"""
         key = cleanup_slice(key, self._upper_bound)
 
         if isinstance(key, int):
-            self._buffer.update_range(key, size=1)
+            self.buffer.update_range(key, size=1)
             return
 
         # else if it's a slice obj
         if isinstance(key, slice):
             if key.step == 1:  # we cleaned up the slice obj so step of None becomes 1
                 # update range according to size using the offset
-                self._buffer.update_range(offset=key.start, size=key.stop - key.start)
+                self.buffer.update_range(offset=key.start, size=key.stop - key.start)
 
             else:
                 step = key.step
                 # convert slice to indices
                 ixs = range(key.start, key.stop, step)
                 for ix in ixs:
-                    self._buffer.update_range(ix, size=1)
+                    self.buffer.update_range(ix, size=1)
         else:
             raise TypeError("must pass int or slice to update range")
+
```

### Comparing `fastplotlib-0.1.0a8/fastplotlib/graphics/features/_colors.py` & `fastplotlib-0.1.0a9/fastplotlib/graphics/features/_colors.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from ._base import GraphicFeature, GraphicFeatureIndexable, cleanup_slice, FeatureEvent
 from ...utils import make_colors, get_cmap_texture
 from pygfx import Color
 
 
 class ColorFeature(GraphicFeatureIndexable):
     @property
-    def _buffer(self):
+    def buffer(self):
         return self._parent.world_object.geometry.colors
 
     def __getitem__(self, item):
-        return self._buffer.data[item]
+        return self.buffer.data[item]
 
     def __init__(self, parent, colors, n_colors: int, alpha: float = 1.0, collection_index: int = None):
         """
         ColorFeature
 
         Parameters
         ----------
@@ -109,15 +109,15 @@
                     "values since this sets the RGBA array data directly."
                 )
 
             if len(key) != 2:
                 raise ValueError("fancy indexing for colors must be 2-dimension, i.e. [n_datapoints, RGBA]")
 
             # set the user passed data directly
-            self._buffer.data[key] = value
+            self.buffer.data[key] = value
 
             # update range
             # first slice obj is going to be the indexing so use key[0]
             # key[1] is going to be RGBA so get rid of it to pass to _update_range
             # _key = cleanup_slice(key[0], self._upper_bound)
             self._update_range(key)
             self._feature_changed(key, value)
@@ -158,15 +158,15 @@
                     new_colors = value.ravel().astype(np.float32)
                 else:
                     new_colors = value.astype(np.float32)
 
             else:
                 raise ValueError("numpy array passed to color must be of shape (4,) or (n_colors_modify, 4)")
 
-        self._buffer.data[key] = new_colors
+        self.buffer.data[key] = new_colors
 
         self._update_range(key)
         self._feature_changed(key, new_colors)
 
     def _update_range(self, key):
         self._update_range_indices(key)
 
@@ -202,15 +202,15 @@
         key = cleanup_slice(key, self._upper_bound)
         if not isinstance(key, slice):
             raise TypeError("Cannot set cmap on single indices, must pass a slice object or "
                             "set it on the entire data.")
 
         n_colors = len(range(key.start, key.stop, key.step))
 
-        colors = make_colors(n_colors, cmap=value)
+        colors = make_colors(n_colors, cmap=value).astype(self._data.dtype)
         super(CmapFeature, self).__setitem__(key, colors)
 
 
 class ImageCmapFeature(GraphicFeature):
     """
     Colormap for ImageGraphic
     """
@@ -234,7 +234,20 @@
             "world_object": self._parent.world_object,
             "new_data": new_data
         }
 
         event_data = FeatureEvent(type="cmap", pick_info=pick_info)
 
         self._call_event_handlers(event_data)
+
+
+class HeatmapCmapFeature(ImageCmapFeature):
+    """
+    Colormap for HeatmapGraphic
+    """
+
+    def _set(self, cmap_name: str):
+        self._parent._material.map.texture.data[:] = make_colors(256, cmap_name)
+        self._parent._material.map.texture.update_range((0, 0, 0), size=(256, 1, 1))
+        self.name = cmap_name
+
+        self._feature_changed(key=None, new_data=self.name)
```

### Comparing `fastplotlib-0.1.0a8/fastplotlib/graphics/features/_data.py` & `fastplotlib-0.1.0a9/fastplotlib/graphics/features/_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,64 @@
 from typing import *
 
 import numpy as np
-from pygfx import Buffer, Texture
+from pygfx import Buffer, Texture, TextureView
 
-from ._base import GraphicFeatureIndexable, cleanup_slice, FeatureEvent
-
-
-def to_float32(array):
-    if isinstance(array, np.ndarray):
-        return array.astype(np.float32, copy=False)
-
-    return array
+from ._base import GraphicFeatureIndexable, cleanup_slice, FeatureEvent, to_gpu_supported_dtype
 
 
 class PointsDataFeature(GraphicFeatureIndexable):
     """
     Access to the vertex buffer data shown in the graphic.
     Supports fancy indexing if the data array also supports it.
     """
     def __init__(self, parent, data: Any, collection_index: int = None):
         data = self._fix_data(data, parent)
         super(PointsDataFeature, self).__init__(parent, data, collection_index=collection_index)
 
     @property
-    def _buffer(self) -> Buffer:
+    def buffer(self) -> Buffer:
         return self._parent.world_object.geometry.positions
 
     def __getitem__(self, item):
-        return self._buffer.data[item]
+        return self.buffer.data[item]
 
     def _fix_data(self, data, parent):
         graphic_type = parent.__class__.__name__
 
+        data = to_gpu_supported_dtype(data)
+
         if data.ndim == 1:
             # for scatter if we receive just 3 points in a 1d array, treat it as just a single datapoint
             # this is different from fix_data for LineGraphic since there we assume that a 1d array
             # is just y-values
             if graphic_type == "ScatterGraphic":
                 data = np.array([data])
             elif graphic_type == "LineGraphic":
-                data = np.dstack([np.arange(data.size), data])[0].astype(np.float32)
+                data = np.dstack([np.arange(data.size, dtype=data.dtype), data])[0]
 
         if data.shape[1] != 3:
             if data.shape[1] != 2:
                 raise ValueError(f"Must pass 1D, 2D or 3D data to {graphic_type}")
 
             # zeros for z
-            zs = np.zeros(data.shape[0], dtype=np.float32)
+            zs = np.zeros(data.shape[0], dtype=data.dtype)
 
             data = np.dstack([data[:, 0], data[:, 1], zs])[0]
 
         return data
 
     def __setitem__(self, key, value):
         # put data into right shape if they're only indexing datapoints
         if isinstance(key, (slice, int)):
             value = self._fix_data(value, self._parent)
         # otherwise assume that they have the right shape
         # numpy will throw errors if it can't broadcast
 
-        self._buffer.data[key] = value
+        self.buffer.data[key] = value
         self._update_range(key)
         # avoid creating dicts constantly if there are no events to handle
         if len(self._event_handlers) > 0:
             self._feature_changed(key, value)
 
     def _update_range(self, key):
         self._update_range_indices(key)
@@ -92,40 +87,102 @@
 
 class ImageDataFeature(GraphicFeatureIndexable):
     """
     Access to the TextureView buffer shown in an ImageGraphic.
     """
 
     def __init__(self, parent, data: Any):
-        if data.ndim != 2:
-            raise ValueError("`data.ndim !=2`, you must pass only a 2D array to an Image graphic")
+        if data.ndim not in (2, 3):
+            raise ValueError(
+                "`data.ndim` must be 2 or 3, ImageGraphic data shape must be "
+                "``[x_dim, y_dim]`` or ``[x_dim, y_dim, rgb]``"
+            )
 
-        data = to_float32(data)
         super(ImageDataFeature, self).__init__(parent, data)
 
     @property
-    def _buffer(self) -> Texture:
+    def buffer(self) -> Texture:
+        """Texture buffer for the image data"""
         return self._parent.world_object.geometry.grid.texture
 
+    def update_gpu(self):
+        """Update the GPU with the buffer"""
+        self._update_range(None)
+
+    def __call__(self, *args, **kwargs):
+        return self.buffer.data
+
     def __getitem__(self, item):
-        return self._buffer.data[item]
+        return self.buffer.data[item]
 
     def __setitem__(self, key, value):
         # make sure float32
-        value = to_float32(value)
+        value = to_gpu_supported_dtype(value)
+
+        self.buffer.data[key] = value
+        self._update_range(key)
+
+        # avoid creating dicts constantly if there are no events to handle
+        if len(self._event_handlers) > 0:
+            self._feature_changed(key, value)
+
+    def _update_range(self, key):
+        self.buffer.update_range((0, 0, 0), size=self.buffer.size)
+
+    def _feature_changed(self, key, new_data):
+        if key is not None:
+            key = cleanup_slice(key, self._upper_bound)
+        if isinstance(key, int):
+            indices = [key]
+        elif isinstance(key, slice):
+            indices = range(key.start, key.stop, key.step)
+        elif key is None:
+            indices = None
+
+        pick_info = {
+            "index": indices,
+            "world_object": self._parent.world_object,
+            "new_data": new_data
+        }
+
+        event_data = FeatureEvent(type="data", pick_info=pick_info)
+
+        self._call_event_handlers(event_data)
+
+
+class HeatmapDataFeature(ImageDataFeature):
+    @property
+    def buffer(self) -> List[Texture]:
+        """list of Texture buffer for the image data"""
+        return [img.geometry.grid.texture for img in self._parent.world_object.children]
+
+    def update_gpu(self):
+        """Update the GPU with the buffer"""
+        self._update_range(None)
+
+    def __getitem__(self, item):
+        return self._data[item]
+
+    def __call__(self, *args, **kwargs):
+        return self.buffer.data
+
+    def __setitem__(self, key, value):
+        # make sure supported type, not float64 etc.
+        value = to_gpu_supported_dtype(value)
 
-        self._buffer.data[key] = value
+        self._data[key] = value
         self._update_range(key)
 
         # avoid creating dicts constantly if there are no events to handle
         if len(self._event_handlers) > 0:
             self._feature_changed(key, value)
 
     def _update_range(self, key):
-        self._buffer.update_range((0, 0, 0), size=self._buffer.size)
+        for buffer in self.buffer:
+            buffer.update_range((0, 0, 0), size=buffer.size)
 
     def _feature_changed(self, key, new_data):
         if key is not None:
             key = cleanup_slice(key, self._upper_bound)
         if isinstance(key, int):
             indices = [key]
         elif isinstance(key, slice):
```

### Comparing `fastplotlib-0.1.0a8/fastplotlib/graphics/features/_present.py` & `fastplotlib-0.1.0a9/fastplotlib/graphics/features/_present.py`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/graphics/features/_thickness.py` & `fastplotlib-0.1.0a9/fastplotlib/graphics/features/_thickness.py`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/graphics/heatmap.py` & `fastplotlib-0.1.0a9/fastplotlib/graphics/heatmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,30 +49,32 @@
             cmap: str = 'plasma',
             selection_options: dict = None,
             *args,
             **kwargs
     ):
         """
         Create a Heatmap Graphic
+
         Parameters
         ----------
         data: array-like, must be 2-dimensional
             | array-like, usually numpy.ndarray, must support ``memoryview()``
-            | Tensorflow Tensors also work _I think_, but not thoroughly tested
+            | Tensorflow Tensors also work **probably**, but not thoroughly tested
         vmin: int, optional
             minimum value for color scaling, calculated from data if not provided
         vmax: int, optional
             maximum value for color scaling, calculated from data if not provided
         cmap: str, optional
             colormap to use to display the image data, default is ``"plasma"``
         selection_options
         args:
             additional arguments passed to Graphic
         kwargs:
             additional keyword arguments passed to Graphic
+
         """
         super().__init__(data, vmin, vmax, cmap, *args, **kwargs)
 
         self.selection_options = SelectionOptions()
         self.selection_options.callbacks = list()
 
         if selection_options is not None:
```

### Comparing `fastplotlib-0.1.0a8/fastplotlib/graphics/histogram.py` & `fastplotlib-0.1.0a9/fastplotlib/graphics/histogram.py`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/graphics/line.py` & `fastplotlib-0.1.0a9/fastplotlib/graphics/line.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 from ._base import Graphic, Interaction, PreviouslyModifiedData
 from .features import PointsDataFeature, ColorFeature, CmapFeature, ThicknessFeature
 from ..utils import make_colors
 
 
 class LineGraphic(Graphic, Interaction):
-    feature_events = [
+    feature_events = (
         "data",
         "colors",
         "cmap",
         "thickness",
         "present"
-    ]
+    )
 
     def __init__(
             self,
             data: Any,
             thickness: float = 2.0,
             colors: Union[str, np.ndarray, Iterable] = "w",
             alpha: float = 1.0,
```

### Comparing `fastplotlib-0.1.0a8/fastplotlib/graphics/scatter.py` & `fastplotlib-0.1.0a9/fastplotlib/graphics/scatter.py`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/layouts/_base.py` & `fastplotlib-0.1.0a9/fastplotlib/layouts/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,40 @@
             camera: Union[OrthographicCamera, PerspectiveCamera],
             controller: Union[PanZoomController, OrbitController],
             scene: Scene,
             canvas: WgpuCanvas,
             renderer: WgpuRenderer,
             name: str = None,
     ):
+        """
+        Base class for plot creation and management. ``PlotArea`` is not intended to be instantiated by users
+        but rather to provide functionallity for ``subplot`` in ``gridplot`` and single ``plot``.
+
+        Parameters
+        ----------
+        parent: PlotArea
+            parent class of subclasses will be a ``PlotArea`` instance
+        position: Any
+            typical use will be for ``subplots`` in a ``gridplot``, position would correspond to the ``[row, column]``
+            location of the ``subplot`` in its ``gridplot``
+        camera: pygfx OrthographicCamera or pygfx PerspectiveCamera
+            ``OrthographicCamera`` type is used to visualize 2D content and ``PerspectiveCamera`` type is used to view
+            3D content, used to view the scene
+        controller: pygfx PanZoomController or pygfx OrbitController
+            ``PanZoomController`` type is used for 2D pan-zoom camera control and ``OrbitController`` type is used for
+            rotating the camera around a center position, used to control the camera
+        scene: pygfx Scene
+            represents the root of a scene graph, will be viewed by the given ``camera``
+        canvas: WgpuCanvas
+            provides surface on which a scene will be rendered
+        renderer: WgpuRenderer
+            object used to render scenes using wgpu
+        name: str, optional
+            name of ``subplot`` or ``plot`` subclass being instantiated
+        """
         self._parent: PlotArea = parent
         self._position = position
 
         self._scene = scene
         self._canvas = canvas
         self._renderer = renderer
         if parent is None:
@@ -94,14 +120,15 @@
     def camera(self) -> Union[OrthographicCamera, PerspectiveCamera]:
         """camera used to view the scene"""
         return self._camera
 
     # in the future we can think about how to allow changing the controller
     @property
     def controller(self) -> Union[PanZoomController, OrbitController]:
+        """controller used to control camera"""
         return self._controller
 
     @property
     def graphics(self) -> Tuple[Graphic]:
         """returns the Graphics in the plot area"""
         return tuple(self._graphics)
```

### Comparing `fastplotlib-0.1.0a8/fastplotlib/layouts/_defaults.py` & `fastplotlib-0.1.0a9/fastplotlib/layouts/_defaults.py`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/layouts/_gridplot.py` & `fastplotlib-0.1.0a9/fastplotlib/layouts/_gridplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,41 +57,61 @@
             | same controllers for first 2 plots and last 2 plots: np.array([[0, 0, 1], [2, 3, 3]])
 
         canvas: WgpuCanvas, optional
             Canvas for drawing
 
         renderer: pygfx.Renderer, optional
             pygfx renderer instance
+
         """
         self.shape = shape
 
         if isinstance(cameras, str):
             if cameras not in valid_cameras:
                 raise ValueError(f"If passing a str, `cameras` must be one of: {valid_cameras}")
             # create the array representing the views for each subplot in the grid
             cameras = np.array([cameras] * self.shape[0] * self.shape[1]).reshape(self.shape)
 
-        if controllers == "sync":
-            controllers = np.zeros(self.shape[0] * self.shape[1], dtype=int).reshape(self.shape)
+        if isinstance(controllers, str):
+            if controllers == "sync":
+                controllers = np.zeros(self.shape[0] * self.shape[1], dtype=int).reshape(self.shape)
 
         if controllers is None:
             controllers = np.arange(self.shape[0] * self.shape[1]).reshape(self.shape)
 
         controllers = to_array(controllers)
 
         if controllers.shape != self.shape:
             raise ValueError
 
+        self._controllers = np.empty(shape=cameras.shape, dtype=object)
+
         cameras = to_array(cameras)
 
         if cameras.shape != self.shape:
             raise ValueError
 
-        if not np.all(np.sort(np.unique(controllers)) == np.arange(np.unique(controllers).size)):
-            raise ValueError("controllers must be consecutive integers")
+        # create controllers if the arguments were integers
+        if np.issubdtype(controllers.dtype, np.integer):
+            if not np.all(np.sort(np.unique(controllers)) == np.arange(np.unique(controllers).size)):
+                raise ValueError("controllers must be consecutive integers")
+
+            for controller in np.unique(controllers):
+                cam = np.unique(cameras[controllers == controller])
+                if cam.size > 1:
+                    raise ValueError(
+                        f"Controller id: {controller} has been assigned to multiple different camera types")
+
+                self._controllers[controllers == controller] = create_controller(cam[0])
+        # else assume it's a single pygfx.Controller instance or a list of controllers
+        else:
+            if isinstance(controllers, pygfx.Controller):
+                self._controllers = np.array([controllers] * shape[0] * shape[1]).reshape(shape)
+            else:
+                self._controllers = np.array(controllers).reshape(shape)
 
         if canvas is None:
             canvas = WgpuCanvas()
 
         if renderer is None:
             renderer = pygfx.renderers.WgpuRenderer(canvas)
 
@@ -106,26 +126,17 @@
         self.renderer = renderer
 
         nrows, ncols = self.shape
 
         self._subplots: np.ndarray[Subplot] = np.ndarray(shape=(nrows, ncols), dtype=object)
         # self.viewports: np.ndarray[Subplot] = np.ndarray(shape=(nrows, ncols), dtype=object)
 
-        self._controllers: List[pygfx.PanZoomController] = [
-            pygfx.PanZoomController() for i in range(np.unique(controllers).size)
-        ]
-
-        self._controllers = np.empty(shape=cameras.shape, dtype=object)
-
-        for controller in np.unique(controllers):
-            cam = np.unique(cameras[controllers == controller])
-            if cam.size > 1:
-                raise ValueError(f"Controller id: {controller} has been assigned to multiple different camera types")
-
-            self._controllers[controllers == controller] = create_controller(cam[0])
+        # self._controllers: List[pygfx.PanZoomController] = [
+        #     pygfx.PanZoomController() for i in range(np.unique(controllers).size)
+        # ]
 
         for i, j in self._get_iterator():
             position = (i, j)
             camera = cameras[i, j]
             controller = self._controllers[i, j]
 
             if self.names is not None:
```

### Comparing `fastplotlib-0.1.0a8/fastplotlib/layouts/_subplot.py` & `fastplotlib-0.1.0a9/fastplotlib/layouts/_subplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,37 @@
             camera: str = '2d',
             controller: Union[PanZoomController, OrbitOrthoController] = None,
             canvas: WgpuCanvas = None,
             renderer: WgpuRenderer = None,
             name: str = None,
             **kwargs
     ):
+        """
+        General plot object that composes a ``Gridplot``. Each ``Gridplot`` instance will have [n rows, n columns]
+        of subplots.
+
+        Parameters
+        ----------
+        position: int tuple, optional
+            corresponds to the [row, column] position of the subplot within a ``Gridplot``
+        parent_dims: int tuple, optional
+            dimensions of the parent ``GridPlot``
+        camera: str, default '2d'
+            indicates the kind of pygfx camera that will be instantiated, '2d' uses pygfx ``OrthographicCamera`` and
+            '3d' uses pygfx ``PerspectiveCamera``
+        controller: PanZoomController or OrbitOrthoController, optional
+            ``PanZoomController`` type is used for 2D pan-zoom camera control and ``OrbitController`` type is used for
+            rotating the camera around a center position, used to control the camera
+        canvas: WgpuCanvas, optional
+            provides surface on which a scene will be rendered
+        renderer: WgpuRenderer, optional
+            object used to render scenes using wgpu
+        name: str, optional
+            name of the subplot, will appear as ``TextGraphic`` above the subplot
+        """
         if canvas is None:
             canvas = WgpuCanvas()
 
         if renderer is None:
             renderer = WgpuRenderer(canvas)
 
         if position is None:
@@ -100,14 +123,15 @@
 
         graphic = graphic_class(*args, **kwargs)
         self.add_graphic(graphic, center=center)
 
         return graphic
 
     def set_title(self, text: Any):
+        """Sets the name of a subplot to 'top' viewport if defined."""
         if text is None:
             return
 
         text = str(text)
         if self._title_graphic is not None:
             self._title_graphic.update_text(text)
         else:
@@ -116,22 +140,24 @@
 
             self.docked_viewports["top"].size = 35
             self.docked_viewports["top"].add_graphic(tg)
 
             self.center_title()
 
     def center_title(self):
+        """Centers name of subplot."""
         if self._title_graphic is None:
             raise AttributeError("No title graphic is set")
 
         self._title_graphic.world_object.position.set(0, 0, 0)
         self.docked_viewports["top"].center_graphic(self._title_graphic, zoom=1.5)
         self._title_graphic.world_object.position.y = -3.5
 
     def get_rect(self):
+        """Returns the bounding box that defines the Subplot within the canvas."""
         row_ix, col_ix = self.position
         width_canvas, height_canvas = self.renderer.logical_size
 
         x_pos = ((width_canvas / self.ncols) + ((col_ix - 1) * (width_canvas / self.ncols))) + self.spacing
         y_pos = ((height_canvas / self.nrows) + ((row_ix - 1) * (height_canvas / self.nrows))) + self.spacing
         width_subplot = (width_canvas / self.ncols) - self.spacing
         height_subplot = (height_canvas / self.nrows) - self.spacing
@@ -221,27 +247,27 @@
         if func in self._animate_funcs_pre:
             self._animate_funcs_pre.remove(func)
 
         if func in self._animate_funcs_post:
             self._animate_funcs_post.remove(func)
 
     def add_graphic(self, graphic, center: bool = True):
+        """Adds a Graphic to the subplot."""
         graphic.world_object.position.z = len(self._graphics)
         super(Subplot, self).add_graphic(graphic, center)
 
-        if isinstance(graphic, graphics.HeatmapGraphic):
-            self.controller.scale.y = copysign(self.controller.scale.y, -1)
-
     def set_axes_visibility(self, visible: bool):
+        """Toggles axes visibility."""
         if visible:
             self.scene.add(self._axes)
         else:
             self.scene.remove(self._axes)
 
     def set_grid_visibility(self, visible: bool):
+        """Toggles grid visibility."""
         if visible:
             self.scene.add(self._grid)
         else:
             self.scene.remove(self._grid)
 
 
 class _DockedViewport(PlotArea):
```

### Comparing `fastplotlib-0.1.0a8/fastplotlib/plot.py` & `fastplotlib-0.1.0a9/fastplotlib/plot.py`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Accent` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Accent`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Blues` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Blues`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/BrBG` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/BrBG`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/BuGn` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/BuGn`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/BuPu` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/BuPu`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/CMRmap` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/CMRmap`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Dark2` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Dark2`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/GnBu` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/GnBu`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Greens` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Greens`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Greys` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Greys`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/OrRd` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/OrRd`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Oranges` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Oranges`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/PRGn` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/PRGn`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Paired` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Paired`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Pastel1` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Pastel1`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Pastel2` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Pastel2`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/PiYG` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/PiYG`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/PuBu` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/PuBu`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/PuBuGn` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/PuBuGn`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/PuOr` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/PuOr`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/PuRd` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/PuRd`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Purples` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Purples`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/RdBu` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/RdBu`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/RdGy` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/RdGy`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/RdPu` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/RdPu`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/RdYlBu` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/RdYlBu`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/RdYlGn` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/RdYlGn`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Reds` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Reds`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Set1` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Set1`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Set2` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Set2`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Set3` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Set3`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Spectral` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Spectral`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/Wistia` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/Wistia`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/YlGn` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/YlGn`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/YlGnBu` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/YlGnBu`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/YlOrBr` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/YlOrBr`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/YlOrRd` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/YlOrRd`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/afmhot` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/afmhot`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/autumn` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/autumn`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/binary` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/binary`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/bone` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/bone`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/brg` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/brg`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/bwr` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/bwr`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/cividis` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/cividis`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/cool` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/cool`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/coolwarm` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/coolwarm`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/copper` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/copper`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/cubehelix` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/cubehelix`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/flag` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/flag`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gist_earth` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gist_earth`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gist_gray` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gist_gray`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gist_heat` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gist_heat`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gist_ncar` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gist_ncar`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gist_rainbow` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gist_rainbow`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gist_stern` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gist_stern`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gist_yarg` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gist_yarg`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gnuplot` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gnuplot`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gnuplot2` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gnuplot2`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/gray` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/gray`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/hot` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/hot`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/hsv` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/hsv`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/inferno` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/inferno`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/jet` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/jet`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/magma` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/magma`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/nipy_spectral` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/nipy_spectral`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/ocean` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/ocean`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/pink` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/pink`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/plasma` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/plasma`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/prism` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/prism`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/rainbow` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/rainbow`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/seismic` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/seismic`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/spring` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/spring`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/summer` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/summer`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/tab10` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/tab10`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/tab20` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/tab20`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/tab20b` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/tab20b`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/tab20c` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/tab20c`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/terrain` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/terrain`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/turbo` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/turbo`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/twilight` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/twilight`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/twilight_shifted` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/twilight_shifted`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/viridis` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/viridis`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/colormaps/winter` & `fastplotlib-0.1.0a9/fastplotlib/utils/colormaps/winter`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/functions.py` & `fastplotlib-0.1.0a9/fastplotlib/utils/functions.py`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/utils/generate_colormaps.py` & `fastplotlib-0.1.0a9/fastplotlib/utils/generate_colormaps.py`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/fastplotlib/widgets/image.py` & `fastplotlib-0.1.0a9/fastplotlib/widgets/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -166,14 +166,15 @@
             dims_order: Union[str, Dict[int, str]] = None,
             slider_dims: Union[str, int, List[Union[str, int]]] = None,
             window_funcs: Union[int, Dict[str, int]] = None,
             frame_apply: Union[callable, Dict[int, callable]] = None,
             vmin_vmax_sliders: bool = False,
             grid_shape: Tuple[int, int] = None,
             names: List[str] = None,
+            grid_plot_kwargs: dict = None,
             **kwargs
     ):
         """
         A high level for displaying n-dimensional image data in conjunction with automatically generated sliders for
         navigating through 1-2 selected dimensions within the image data.
 
         Can display a single n-dimensional image array or a grid of n-dimensional images.
@@ -223,14 +224,17 @@
             | if `window_funcs` is used, then this function is applied after `window_funcs`
             | this function must be a callable that returns a 2D array
             | example use case: converting an RGB frame from video to a 2D grayscale frame
 
         grid_shape: Optional[Tuple[int, int]]
             manually provide the shape for a gridplot, otherwise a square gridplot is approximated.
 
+        grid_plot_kwargs: dict, optional
+            passed to `GridPlot`
+
         names: Optional[str]
             gives names to the subplots
 
         kwargs: Any
             passed to fastplotlib.graphics.Image
         """
         self._names = None
@@ -467,20 +471,20 @@
         if self._plot_type == "single":
             self._plot: Plot = Plot()
 
             minmax = quick_min_max(self.data[0])
 
             if vmin_vmax_sliders:
                 data_range = np.ptp(minmax)
-                data_range_30p = np.ptp(minmax) * 0.3
+                data_range_40p = np.ptp(minmax) * 0.3
 
                 minmax_slider = FloatRangeSlider(
                     value=minmax,
-                    min=minmax[0] - data_range_30p,
-                    max=minmax[1] + data_range_30p,
+                    min=minmax[0] - data_range_40p,
+                    max=minmax[1] + data_range_40p,
                     step=data_range / 150,
                     description=f"min-max",
                     readout=True,
                     readout_format='.3f',
                 )
 
                 minmax_slider.observe(
@@ -490,39 +494,43 @@
 
                 self.vmin_vmax_sliders.append(minmax_slider)
 
             if ("vmin" not in kwargs.keys()) or ("vmax" not in kwargs.keys()):
                 kwargs["vmin"], kwargs["vmax"] = minmax
 
             frame = self._process_indices(self.data[0], slice_indices=self._current_index)
+            frame = self._process_frame_apply(frame, 0)
 
             self.image_graphics: List[ImageGraphic] = [self.plot.add_image(data=frame, name="image", **kwargs)]
 
         elif self._plot_type == "grid":
-            self._plot: GridPlot = GridPlot(shape=grid_shape, controllers="sync")
+            if grid_plot_kwargs is None:
+                grid_plot_kwargs = {"controllers": "sync"}
+
+            self._plot: GridPlot = GridPlot(shape=grid_shape, **grid_plot_kwargs)
 
             self.image_graphics = list()
             for data_ix, (d, subplot) in enumerate(zip(self.data, self.plot)):
                 minmax = quick_min_max(self.data[data_ix])
 
                 if self._names is not None:
                     name = self._names[data_ix]
                     name_slider = name
                 else:
                     name = None
                     name_slider = ""
 
                 if vmin_vmax_sliders:
                     data_range = np.ptp(minmax)
-                    data_range_30p = np.ptp(minmax) * 0.4
+                    data_range_40p = np.ptp(minmax) * 0.4
 
                     minmax_slider = FloatRangeSlider(
                         value=minmax,
-                        min=minmax[0] - data_range_30p,
-                        max=minmax[1] + data_range_30p,
+                        min=minmax[0] - data_range_40p,
+                        max=minmax[1] + data_range_40p,
                         step=data_range / 150,
                         description=f"mm: {name_slider}",
                         readout=True,
                         readout_format='.3f',
                     )
 
                     minmax_slider.observe(
@@ -535,14 +543,15 @@
                 if ("vmin" not in kwargs.keys()) or ("vmax" not in kwargs.keys()):
                     _kwargs = deepcopy(kwargs)
                     _kwargs["vmin"], _kwargs["vmax"] = minmax
                 else:
                     _kwargs = kwargs
 
                 frame = self._process_indices(d, slice_indices=self._current_index)
+                frame = self._process_frame_apply(frame, data_ix)
                 ig = ImageGraphic(frame, name="image", **_kwargs)
                 subplot.add_graphic(ig)
                 subplot.name = name
                 subplot.set_title(name)
                 self.image_graphics.append(ig)
 
         self.plot.renderer.add_event_handler(self._set_slider_layout, "resize")
@@ -763,19 +772,25 @@
             half_window = int((window_size - 1) / 2)  # half-window size
             # get the max bound for that dimension
             max_bound = self._dims_max_bounds[dim_str]
             indices_dim = range(max(0, ix - half_window), min(max_bound, ix + half_window))
             return indices_dim
 
     def _process_frame_apply(self, array, data_ix) -> np.ndarray:
+        if callable(self.frame_apply):
+            return self.frame_apply(array)
+
         if data_ix not in self.frame_apply.keys():
             return array
-        if self.frame_apply[data_ix] is not None:
+
+        elif self.frame_apply[data_ix] is not None:
             return self.frame_apply[data_ix](array)
 
+        return array
+
     def _slider_value_changed(
             self,
             dimension: str,
             change: dict
     ):
         if self.block_sliders:
             return
@@ -797,14 +812,40 @@
 
         for vs in self._vertical_sliders:
             vs.layout = Layout(height=f"{h}px")
 
         for mm in self.vmin_vmax_sliders:
             mm.layout = Layout(width=f"{w}px")
 
+    def _get_vmin_vmax_range(self, data: np.ndarray) -> Tuple[int, int]:
+        minmax = quick_min_max(data)
+
+        data_range = np.ptp(minmax)
+        data_range_40p = np.ptp(minmax) * 0.4
+
+        _range = (
+            minmax,
+            data_range,
+            minmax[0] - data_range_40p,
+            minmax[1] + data_range_40p
+        )
+
+        return _range
+
+    def reset_vmin_vmax(self):
+        """
+        Reset the vmin and vmax w.r.t. the currently displayed image(s)
+        """
+        for i, ig in enumerate(self.image_graphics):
+            mm = self._get_vmin_vmax_range(ig.data())
+            self.vmin_vmax_sliders[i].min = mm[2]
+            self.vmin_vmax_sliders[i].max = mm[3]
+            self.vmin_vmax_sliders[i].step = mm[1] / 150
+            self.vmin_vmax_sliders[i].value = mm[0]
+
     def show(self):
         """
         Show the widget
 
         Returns
         -------
         VBox
```

### Comparing `fastplotlib-0.1.0a8/fastplotlib.egg-info/PKG-INFO` & `fastplotlib-0.1.0a9/fastplotlib.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 Metadata-Version: 2.1
 Name: fastplotlib
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: A fast plotting library built using the pygfx render engine
 Home-page: https://github.com/kushalkolar/fastplotlib
 Author: Kushal Kolar
 Author-email: 
 License: Apache 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # fastplotlib
-[![PyPI version](https://badge.fury.io/py/fastplotlib.svg)](https://badge.fury.io/py/fastplotlib) [![Gitter](https://badges.gitter.im/fastplotlib/community.svg)](https://gitter.im/fastplotlib/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+[![PyPI version](https://badge.fury.io/py/fastplotlib.svg)](https://badge.fury.io/py/fastplotlib)
+[![Documentation Status](https://readthedocs.org/projects/fastplotlib/badge/?version=latest)](https://fastplotlib.readthedocs.io/en/latest/?badge=latest)
+[![Gitter](https://badges.gitter.im/fastplotlib/community.svg)](https://gitter.im/fastplotlib/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
 [**Installation**](https://github.com/kushalkolar/fastplotlib#installation) | [**GPU Drivers**](https://github.com/kushalkolar/fastplotlib#install-vulkan-drivers) | [**Examples**](https://github.com/kushalkolar/fastplotlib#examples)
 
 A fast plotting library built using the [`pygfx`](https://github.com/pygfx/pygfx) render engine utilizing [Vulkan](https://en.wikipedia.org/wiki/Vulkan) via WGPU, so it is very fast! `fastplotlib` is focussed on very fast interactive plotting in the notebook using an expressive API. It also works within desktop applications using `glfw` or `Qt`.
 
 `fastplotlib` is currently in the **early alpha stage with breaking changes every ~week**, but you're welcome to try it out or contribute! See our [Roadmap for 2023](https://github.com/kushalkolar/fastplotlib/issues/55).
 
+**Documentation**: http://fastplotlib.readthedocs.io/ 
+
+The docs are not entirely thorough, we recommend the example notebooks to get started.
+
 Questions, ideas? Post an issue or [chat on gitter](https://gitter.im/fastplotlib/community?utm_source=share-link&utm_medium=link&utm_campaign=share-link).
 
 ![epic](https://user-images.githubusercontent.com/9403332/210304473-f36f2aaf-319e-435b-bcc8-0e8d3e1ef282.gif)
 
 # Examples
 
 **See the examples directory. Start out with `simple.ipynb`.**
@@ -119,15 +125,15 @@
 jupyter lab
 ```
 
 ## Install Vulkan drivers
 
 You will need a GPU that supports Vulkan (integrated GPUs in CPUs are usually fine). Generally if your GPU is from 2017 or later it should support Vulkan.
 
-For more information see: https://github.com/pygfx/wgpu-py#platform-requirements
+For more information see: https://wgpu-py.readthedocs.io/en/stable/start.html#platform-requirements
 
 ### Windows:
 Vulkan should be installed by default on Windows 11, but you will need to install your GPU manufacturer's driver package (Nvidia or AMD). If you have an integrated GPU within your CPU, you might still need to install a driver package too, check your CPU manufacturer's info. We recommend installing C compilers so that you can install `simplejpeg` which improves remote frame buffer performance in notebooks.
 
 ### Linux:
 Debian based distros:
```

### Comparing `fastplotlib-0.1.0a8/fastplotlib.egg-info/SOURCES.txt` & `fastplotlib-0.1.0a9/fastplotlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastplotlib-0.1.0a8/setup.py` & `fastplotlib-0.1.0a9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,14 @@
 from pathlib import Path
 
 
 install_requires = [
     'numpy',
     'pygfx>=0.1.10',
     'jupyterlab',
-    'jupyterlab-widgets==1.1.1',
-    'ipywidgets<8.0.0',
     'jupyter-rfb',
 ]
 
 
 with open(Path(__file__).parent.joinpath("README.md")) as f:
     readme = f.read()
```

