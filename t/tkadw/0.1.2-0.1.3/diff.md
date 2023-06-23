# Comparing `tmp/tkadw-0.1.2.tar.gz` & `tmp/tkadw-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkadw-0.1.2.tar", max compression
+gzip compressed data, was "tkadw-0.1.3.tar", max compression
```

## Comparing `tkadw-0.1.2.tar` & `tkadw-0.1.3.tar`

### file list

```diff
@@ -1,218 +1,218 @@
--rw-r--r--   0        0        0      274 2023-06-23 07:49:33.316949 tkadw-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      101 2023-04-15 23:36:06.262325 tkadw-0.1.2/README.md
--rw-r--r--   0        0        0      112 2023-06-23 03:45:25.577456 tkadw-0.1.2/tkadw/__init__.py
--rw-r--r--   0        0        0      948 2023-06-23 07:49:26.692233 tkadw-0.1.2/tkadw/__main__.py
--rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.1.2/tkadw/app.config
--rw-r--r--   0        0        0      940 2023-06-09 11:52:45.801259 tkadw-0.1.2/tkadw/appconfig.py
--rw-r--r--   0        0        0      896 2023-06-23 07:36:10.506439 tkadw-0.1.2/tkadw/canvas/__init__.py
--rw-r--r--   0        0        0     1701 2023-06-23 07:38:42.890718 tkadw-0.1.2/tkadw/canvas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      124 2023-04-15 23:20:17.035856 tkadw-0.1.2/tkadw/canvas/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    22885 2023-06-23 04:54:52.588047 tkadw-0.1.2/tkadw/canvas/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0     3479 2023-04-15 23:20:17.037902 tkadw-0.1.2/tkadw/canvas/__pycache__/button.cpython-38.pyc
--rw-r--r--   0        0        0    23239 2023-06-23 05:05:08.679421 tkadw-0.1.2/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc
--rw-r--r--   0        0        0    25982 2023-06-23 07:48:50.831965 tkadw-0.1.2/tkadw/canvas/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0    13288 2023-06-23 07:38:42.954769 tkadw-0.1.2/tkadw/canvas/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.1.2/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0    27814 2023-06-23 07:48:50.836964 tkadw-0.1.2/tkadw/canvas/__pycache__/textbox.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-06-10 10:53:44.353940 tkadw-0.1.2/tkadw/canvas/adwite/__init__.py
--rw-r--r--   0        0        0     1363 2023-06-10 11:23:03.996035 tkadw-0.1.2/tkadw/canvas/adwite/button.py
--rw-r--r--   0        0        0       80 2023-06-09 13:54:04.880107 tkadw-0.1.2/tkadw/canvas/atomize/__init__.py
--rw-r--r--   0        0        0     2520 2023-06-10 04:30:03.863844 tkadw-0.1.2/tkadw/canvas/atomize/button.py
--rw-r--r--   0        0        0    17270 2023-06-23 04:54:52.447686 tkadw-0.1.2/tkadw/canvas/button.py
--rw-r--r--   0        0        0    20382 2023-06-23 05:05:08.591410 tkadw-0.1.2/tkadw/canvas/drawengine.py
--rw-r--r--   0        0        0    22377 2023-06-23 07:48:50.714445 tkadw-0.1.2/tkadw/canvas/entry.py
--rw-r--r--   0        0        0      513 2023-06-09 23:26:21.009369 tkadw-0.1.2/tkadw/canvas/fluent/__init__.py
--rw-r--r--   0        0        0     8629 2023-06-23 05:15:43.010231 tkadw-0.1.2/tkadw/canvas/frame.py
--rw-r--r--   0        0        0     2051 2023-06-10 01:20:40.907297 tkadw-0.1.2/tkadw/canvas/fun.py
--rw-r--r--   0        0        0    15490 2023-06-10 01:25:11.532315 tkadw-0.1.2/tkadw/canvas/fun2.py
--rw-r--r--   0        0        0     8108 2023-06-10 01:29:02.970946 tkadw-0.1.2/tkadw/canvas/fun3.py
--rw-r--r--   0        0        0     3202 2023-06-10 03:27:44.231516 tkadw-0.1.2/tkadw/canvas/fun4.py
--rw-r--r--   0        0        0      942 2023-06-10 03:50:17.322506 tkadw-0.1.2/tkadw/canvas/fun5.py
--rw-r--r--   0        0        0     9870 2023-06-10 07:36:40.103845 tkadw-0.1.2/tkadw/canvas/fun6.py
--rw-r--r--   0        0        0     5690 2023-06-10 03:45:21.292347 tkadw-0.1.2/tkadw/canvas/poly.tcl
--rw-r--r--   0        0        0    22421 2023-06-23 07:48:50.681445 tkadw-0.1.2/tkadw/canvas/textbox.py
--rw-r--r--   0        0        0     4597 2023-05-27 23:04:22.860566 tkadw-0.1.2/tkadw/canvas/titlebar.py
--rw-r--r--   0        0        0       29 2023-06-23 03:52:51.957932 tkadw-0.1.2/tkadw/tkite/__init__.py
--rw-r--r--   0        0        0      181 2023-06-23 03:52:52.129145 tkadw-0.1.2/tkadw/tkite/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      283 2023-06-23 07:44:06.875178 tkadw-0.1.2/tkadw/tkite/gtk/__init__.py
--rw-r--r--   0        0        0      620 2023-06-23 07:44:06.983012 tkadw-0.1.2/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5020 2023-06-23 05:37:39.419391 tkadw-0.1.2/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0     2902 2023-06-23 05:36:24.094777 tkadw-0.1.2/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0     2457 2023-06-23 07:42:27.405172 tkadw-0.1.2/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0     3908 2023-06-23 07:45:23.356231 tkadw-0.1.2/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc
--rw-r--r--   0        0        0     3898 2023-06-23 05:37:39.292931 tkadw-0.1.2/tkadw/tkite/gtk/button.py
--rw-r--r--   0        0        0     2201 2023-06-23 05:36:23.978561 tkadw-0.1.2/tkadw/tkite/gtk/entry.py
--rw-r--r--   0        0        0     1141 2023-06-23 07:40:36.374539 tkadw-0.1.2/tkadw/tkite/gtk/frame.py
--rw-r--r--   0        0        0      500 2023-06-23 00:56:14.658098 tkadw-0.1.2/tkadw/tkite/gtk/notebook.py
--rw-r--r--   0        0        0     2785 2023-06-23 07:45:23.240982 tkadw-0.1.2/tkadw/tkite/gtk/textbox.py
--rw-r--r--   0        0        0        0 2023-06-09 14:28:28.424277 tkadw-0.1.2/tkadw/ttk/__init__.py
--rw-r--r--   0        0        0      139 2023-06-09 14:38:22.776399 tkadw-0.1.2/tkadw/ttk/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1349 2023-06-09 14:41:39.497543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/__init__.py
--rw-r--r--   0        0        0     2722 2023-06-09 14:43:18.298069 tkadw-0.1.2/tkadw/ttk/atomize_ttk/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2961 2023-06-09 14:41:39.498543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/sun-valley.tcl
--rw-r--r--   0        0        0     5150 2023-05-14 15:25:00.266570 tkadw-0.1.2/tkadw/ttk/atomize_ttk/sv.tcl
--rw-r--r--   0        0        0      270 2023-06-09 14:41:39.500545 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/arrow-down.png
--rw-r--r--   0        0        0      261 2023-06-09 14:41:39.501544 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/arrow-right.png
--rw-r--r--   0        0        0      274 2023-06-09 14:41:39.501544 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/arrow-up.png
--rw-r--r--   0        0        0      262 2023-06-09 14:41:39.502544 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-accent-disabled.png
--rw-r--r--   0        0        0      373 2023-06-09 14:41:39.503545 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-accent-hover.png
--rw-r--r--   0        0        0      363 2023-06-09 14:41:39.503545 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-accent-pressed.png
--rw-r--r--   0        0        0      377 2023-06-09 14:41:39.504545 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-accent-rest.png
--rw-r--r--   0        0        0      274 2023-06-09 14:41:39.505542 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-close-hover.png
--rw-r--r--   0        0        0      274 2023-06-09 14:41:39.505542 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-close-pressed.png
--rw-r--r--   0        0        0      301 2023-06-09 14:41:39.506544 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-disabled.png
--rw-r--r--   0        0        0      276 2023-06-09 14:41:39.506544 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-hover.png
--rw-r--r--   0        0        0      288 2023-06-09 14:41:39.507543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-pressed.png
--rw-r--r--   0        0        0      301 2023-06-09 14:41:39.508543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-rest.png
--rw-r--r--   0        0        0      245 2023-06-09 14:41:39.508543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-titlebar-hover.png
--rw-r--r--   0        0        0      238 2023-06-09 14:41:39.509543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/button-titlebar-pressed.png
--rw-r--r--   0        0        0      386 2023-06-09 14:41:39.509543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/card.png
--rw-r--r--   0        0        0      383 2023-06-09 14:41:39.510542 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-disabled.png
--rw-r--r--   0        0        0      474 2023-06-09 14:41:39.511543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-hover.png
--rw-r--r--   0        0        0      460 2023-06-09 14:41:39.511543 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-pressed.png
--rw-r--r--   0        0        0      475 2023-06-09 14:41:39.512544 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-rest.png
--rw-r--r--   0        0        0      294 2023-06-09 14:41:39.513547 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-tri-disabled.png
--rw-r--r--   0        0        0      362 2023-06-09 14:41:39.514132 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-tri-hover.png
--rw-r--r--   0        0        0      358 2023-06-09 14:41:39.515137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-tri-pressed.png
--rw-r--r--   0        0        0      363 2023-06-09 14:41:39.515137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-tri-rest.png
--rw-r--r--   0        0        0      312 2023-06-09 14:41:39.516139 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-disabled.png
--rw-r--r--   0        0        0      353 2023-06-09 14:41:39.517139 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-hover.png
--rw-r--r--   0        0        0      302 2023-06-09 14:41:39.517139 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-pressed.png
--rw-r--r--   0        0        0      353 2023-06-09 14:41:39.518137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-rest.png
--rw-r--r--   0        0        0      129 2023-06-09 14:41:39.519137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/empty.png
--rw-r--r--   0        0        0      273 2023-06-09 14:41:39.519137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/entry-disabled.png
--rw-r--r--   0        0        0      335 2023-06-09 14:41:39.520136 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/entry-focus.png
--rw-r--r--   0        0        0      269 2023-06-09 14:41:39.521137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/entry-hover.png
--rw-r--r--   0        0        0      324 2023-06-09 14:41:39.522140 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/entry-invalid.png
--rw-r--r--   0        0        0      297 2023-06-09 14:41:39.522140 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/entry-rest.png
--rw-r--r--   0        0        0      337 2023-06-09 14:41:39.523139 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/notebook-border.png
--rw-r--r--   0        0        0      186 2023-06-09 14:41:39.524139 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/notebook.png
--rw-r--r--   0        0        0      193 2023-06-09 14:41:39.524139 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/progress-pbar-hor.png
--rw-r--r--   0        0        0      214 2023-06-09 14:41:39.525137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/progress-pbar-vert.png
--rw-r--r--   0        0        0      157 2023-06-09 14:41:39.526137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/progress-trough-hor.png
--rw-r--r--   0        0        0      160 2023-06-09 14:41:39.526137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/progress-trough-vert.png
--rw-r--r--   0        0        0      553 2023-06-09 14:41:39.527138 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-disabled.png
--rw-r--r--   0        0        0      853 2023-06-09 14:41:39.527138 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-hover.png
--rw-r--r--   0        0        0      786 2023-06-09 14:41:39.528137 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-pressed.png
--rw-r--r--   0        0        0      830 2023-06-09 14:41:39.528640 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-rest.png
--rw-r--r--   0        0        0      552 2023-06-09 14:41:39.529647 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-disabled.png
--rw-r--r--   0        0        0      602 2023-06-09 14:41:39.530644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-hover.png
--rw-r--r--   0        0        0      616 2023-06-09 14:41:39.530644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-pressed.png
--rw-r--r--   0        0        0      621 2023-06-09 14:41:39.531645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-rest.png
--rw-r--r--   0        0        0      724 2023-06-09 14:41:39.532645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-disabled.png
--rw-r--r--   0        0        0      808 2023-06-09 14:41:39.532645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-hover.png
--rw-r--r--   0        0        0      735 2023-06-09 14:41:39.533645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-pressed.png
--rw-r--r--   0        0        0      771 2023-06-09 14:41:39.533645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-rest.png
--rw-r--r--   0        0        0      216 2023-06-09 14:41:39.534644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-trough-hor.png
--rw-r--r--   0        0        0      215 2023-06-09 14:41:39.534644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-trough-vert.png
--rw-r--r--   0        0        0      226 2023-06-09 14:41:39.535644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-down.png
--rw-r--r--   0        0        0      254 2023-06-09 14:41:39.536643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-hor-thumb.png
--rw-r--r--   0        0        0      338 2023-06-09 14:41:39.537644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-hor-trough.png
--rw-r--r--   0        0        0      233 2023-06-09 14:41:39.538644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-left.png
--rw-r--r--   0        0        0      227 2023-06-09 14:41:39.538644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-right.png
--rw-r--r--   0        0        0      236 2023-06-09 14:41:39.539644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-up.png
--rw-r--r--   0        0        0      264 2023-06-09 14:41:39.539644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-vert-thumb.png
--rw-r--r--   0        0        0      343 2023-06-09 14:41:39.540644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scroll-vert-trough.png
--rw-r--r--   0        0        0      128 2023-06-09 14:41:39.541644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/separator.png
--rw-r--r--   0        0        0      276 2023-06-09 14:41:39.542647 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/sizegrip.png
--rw-r--r--   0        0        0      733 2023-06-09 14:41:39.542647 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-disabled.png
--rw-r--r--   0        0        0      945 2023-06-09 14:41:39.543645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-hover.png
--rw-r--r--   0        0        0      963 2023-06-09 14:41:39.544643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-pressed.png
--rw-r--r--   0        0        0      895 2023-06-09 14:41:39.545645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-rest.png
--rw-r--r--   0        0        0      623 2023-06-09 14:41:39.545645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-disabled.png
--rw-r--r--   0        0        0      927 2023-06-09 14:41:39.546644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-hover.png
--rw-r--r--   0        0        0      936 2023-06-09 14:41:39.547644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-pressed.png
--rw-r--r--   0        0        0      859 2023-06-09 14:41:39.547644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-rest.png
--rw-r--r--   0        0        0      265 2023-06-09 14:41:39.548643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/tab-hover.png
--rw-r--r--   0        0        0      164 2023-06-09 14:41:39.549644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/tab-rest.png
--rw-r--r--   0        0        0      319 2023-06-09 14:41:39.549644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/tab-selected.png
--rw-r--r--   0        0        0      295 2023-06-09 14:41:39.550645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/treeheading-hover.png
--rw-r--r--   0        0        0      317 2023-06-09 14:41:39.551644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/treeheading-pressed.png
--rw-r--r--   0        0        0      321 2023-06-09 14:41:39.551644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/treeheading-rest.png
--rw-r--r--   0        0        0    20188 2023-06-09 14:41:39.499549 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark.tcl
--rw-r--r--   0        0        0      278 2023-06-09 14:41:39.552643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/arrow-down.png
--rw-r--r--   0        0        0      273 2023-06-09 14:41:39.552643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/arrow-right.png
--rw-r--r--   0        0        0      285 2023-06-09 14:41:39.553645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/arrow-up.png
--rw-r--r--   0        0        0      271 2023-06-09 14:41:39.554647 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-accent-disabled.png
--rw-r--r--   0        0        0      219 2023-06-09 14:48:51.766400 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-accent-hover.png
--rw-r--r--   0        0        0      255 2023-06-09 14:53:14.082428 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-accent-pressed.png
--rw-r--r--   0        0        0      217 2023-06-09 14:48:47.641380 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-accent-rest.png
--rw-r--r--   0        0        0      326 2023-06-09 14:41:39.556644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-close-hover.png
--rw-r--r--   0        0        0      316 2023-06-09 14:41:39.557644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-close-pressed.png
--rw-r--r--   0        0        0      307 2023-06-09 14:41:39.557644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-disabled.png
--rw-r--r--   0        0        0      306 2023-06-09 14:41:39.558645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-hover.png
--rw-r--r--   0        0        0      289 2023-06-09 14:41:39.559644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-pressed.png
--rw-r--r--   0        0        0      303 2023-06-09 14:41:39.559644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-rest.png
--rw-r--r--   0        0        0      238 2023-06-09 14:41:39.560643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-titlebar-hover.png
--rw-r--r--   0        0        0      225 2023-06-09 14:41:39.561643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/button-titlebar-pressed.png
--rw-r--r--   0        0        0      479 2023-06-09 14:43:10.460434 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/card.png
--rw-r--r--   0        0        0      381 2023-06-09 14:41:39.562646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-disabled.png
--rw-r--r--   0        0        0      476 2023-06-09 14:41:39.562646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-hover.png
--rw-r--r--   0        0        0      467 2023-06-09 14:41:39.563646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-pressed.png
--rw-r--r--   0        0        0      473 2023-06-09 14:41:39.564644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-rest.png
--rw-r--r--   0        0        0      299 2023-06-09 14:41:39.564644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-tri-disabled.png
--rw-r--r--   0        0        0      365 2023-06-09 14:41:39.565643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-tri-hover.png
--rw-r--r--   0        0        0      362 2023-06-09 14:41:39.566644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-tri-pressed.png
--rw-r--r--   0        0        0      367 2023-06-09 14:41:39.566644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-tri-rest.png
--rw-r--r--   0        0        0      324 2023-06-09 14:41:39.567644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-unsel-disabled.png
--rw-r--r--   0        0        0      334 2023-06-09 14:41:39.568643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-unsel-hover.png
--rw-r--r--   0        0        0      302 2023-06-09 14:41:39.568643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-unsel-pressed.png
--rw-r--r--   0        0        0      333 2023-06-09 14:41:39.569646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/check-unsel-rest.png
--rw-r--r--   0        0        0      129 2023-06-09 14:41:39.569646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/empty.png
--rw-r--r--   0        0        0      289 2023-06-09 14:41:39.570644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/entry-disabled.png
--rw-r--r--   0        0        0      331 2023-06-09 14:41:39.571647 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/entry-focus.png
--rw-r--r--   0        0        0      302 2023-06-09 14:41:39.572644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/entry-hover.png
--rw-r--r--   0        0        0      324 2023-06-09 14:41:39.572644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/entry-invalid.png
--rw-r--r--   0        0        0      308 2023-06-09 14:41:39.573646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/entry-rest.png
--rw-r--r--   0        0        0      298 2023-06-09 14:41:39.573646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/notebook-border.png
--rw-r--r--   0        0        0      185 2023-06-09 14:41:39.574643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/notebook.png
--rw-r--r--   0        0        0      192 2023-06-09 14:41:39.575643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/progress-pbar-hor.png
--rw-r--r--   0        0        0      216 2023-06-09 14:41:39.575643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/progress-pbar-vert.png
--rw-r--r--   0        0        0      158 2023-06-09 14:41:39.576643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/progress-trough-hor.png
--rw-r--r--   0        0        0      161 2023-06-09 14:41:39.577644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/progress-trough-vert.png
--rw-r--r--   0        0        0      523 2023-06-09 14:41:39.578645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-disabled.png
--rw-r--r--   0        0        0      837 2023-06-09 14:41:39.578645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-hover.png
--rw-r--r--   0        0        0      764 2023-06-09 14:41:39.579645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-pressed.png
--rw-r--r--   0        0        0      773 2023-06-09 14:41:39.580644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-rest.png
--rw-r--r--   0        0        0      521 2023-06-09 14:41:39.581644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-disabled.png
--rw-r--r--   0        0        0      573 2023-06-09 14:41:39.582644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-hover.png
--rw-r--r--   0        0        0      636 2023-06-09 14:41:39.582644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-pressed.png
--rw-r--r--   0        0        0      576 2023-06-09 14:41:39.583644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-rest.png
--rw-r--r--   0        0        0      658 2023-06-09 14:41:39.584643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-disabled.png
--rw-r--r--   0        0        0      749 2023-06-09 14:41:39.584643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-hover.png
--rw-r--r--   0        0        0      675 2023-06-09 14:41:39.585645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-pressed.png
--rw-r--r--   0        0        0      701 2023-06-09 14:41:39.586645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-rest.png
--rw-r--r--   0        0        0      208 2023-06-09 14:41:39.586645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-trough-hor.png
--rw-r--r--   0        0        0      214 2023-06-09 14:41:39.587646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-trough-vert.png
--rw-r--r--   0        0        0      229 2023-06-09 14:41:39.588644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-down.png
--rw-r--r--   0        0        0      234 2023-06-09 14:41:39.589644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-hor-thumb.png
--rw-r--r--   0        0        0      321 2023-06-09 14:41:39.589644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-hor-trough.png
--rw-r--r--   0        0        0      232 2023-06-09 14:41:39.590644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-left.png
--rw-r--r--   0        0        0      223 2023-06-09 14:41:39.590644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-right.png
--rw-r--r--   0        0        0      237 2023-06-09 14:41:39.591643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-up.png
--rw-r--r--   0        0        0      262 2023-06-09 14:41:39.592644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-vert-thumb.png
--rw-r--r--   0        0        0      324 2023-06-09 14:41:39.593644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scroll-vert-trough.png
--rw-r--r--   0        0        0      128 2023-06-09 14:41:39.594646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/separator.png
--rw-r--r--   0        0        0      272 2023-06-09 14:41:39.594646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/sizegrip.png
--rw-r--r--   0        0        0      726 2023-06-09 14:41:39.595643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-disabled.png
--rw-r--r--   0        0        0      867 2023-06-09 14:41:39.596647 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-hover.png
--rw-r--r--   0        0        0      880 2023-06-09 14:41:39.597645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-pressed.png
--rw-r--r--   0        0        0      814 2023-06-09 14:41:39.597645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-rest.png
--rw-r--r--   0        0        0      590 2023-06-09 14:41:39.598645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-disabled.png
--rw-r--r--   0        0        0      906 2023-06-09 14:41:39.598645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-hover.png
--rw-r--r--   0        0        0      916 2023-06-09 14:41:39.599644 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-pressed.png
--rw-r--r--   0        0        0      857 2023-06-09 14:41:39.600643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-rest.png
--rw-r--r--   0        0        0      295 2023-06-09 14:41:39.600643 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/tab-hover.png
--rw-r--r--   0        0        0      164 2023-06-09 14:41:39.601645 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/tab-rest.png
--rw-r--r--   0        0        0      318 2023-06-09 14:41:39.602649 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/tab-selected.png
--rw-r--r--   0        0        0      338 2023-06-09 14:41:39.602649 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/treeheading-hover.png
--rw-r--r--   0        0        0      318 2023-06-09 14:41:39.603646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/treeheading-pressed.png
--rw-r--r--   0        0        0      330 2023-06-09 14:41:39.603646 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/treeheading-rest.png
--rw-r--r--   0        0        0    20371 2023-06-09 14:41:39.500545 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light.tcl
--rw-r--r--   0        0        0     3045 2023-05-14 15:25:00.269895 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/sprites_dark.tcl
--rw-r--r--   0        0        0     3092 2023-05-14 15:25:00.270897 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/sprites_light.tcl
--rw-r--r--   0        0        0    18371 2023-05-14 15:25:00.272896 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/spritesheet_dark.png
--rw-r--r--   0        0        0     2649 2023-06-09 14:36:51.668892 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/spritesheet_light.png
--rw-r--r--   0        0        0    18462 2023-05-14 15:25:00.272896 tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/spritesheet_light2.png
--rw-r--r--   0        0        0      372 2023-06-09 14:40:30.166428 tkadw-0.1.2/tkadw/ttk/test.py
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 tkadw-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      272 2023-06-23 07:54:02.049872 tkadw-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      101 2023-04-15 23:36:06.262325 tkadw-0.1.3/README.md
+-rw-r--r--   0        0        0      112 2023-06-23 03:45:25.577456 tkadw-0.1.3/tkadw/__init__.py
+-rw-r--r--   0        0        0      948 2023-06-23 07:49:26.692233 tkadw-0.1.3/tkadw/__main__.py
+-rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.1.3/tkadw/app.config
+-rw-r--r--   0        0        0      940 2023-06-09 11:52:45.801259 tkadw-0.1.3/tkadw/appconfig.py
+-rw-r--r--   0        0        0      896 2023-06-23 07:36:10.506439 tkadw-0.1.3/tkadw/canvas/__init__.py
+-rw-r--r--   0        0        0     1701 2023-06-23 07:38:42.890718 tkadw-0.1.3/tkadw/canvas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      124 2023-04-15 23:20:17.035856 tkadw-0.1.3/tkadw/canvas/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    22885 2023-06-23 04:54:52.588047 tkadw-0.1.3/tkadw/canvas/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     3479 2023-04-15 23:20:17.037902 tkadw-0.1.3/tkadw/canvas/__pycache__/button.cpython-38.pyc
+-rw-r--r--   0        0        0    23239 2023-06-23 05:05:08.679421 tkadw-0.1.3/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc
+-rw-r--r--   0        0        0    25982 2023-06-23 07:48:50.831965 tkadw-0.1.3/tkadw/canvas/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0    13288 2023-06-23 07:38:42.954769 tkadw-0.1.3/tkadw/canvas/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.1.3/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0    27824 2023-06-23 07:53:35.555717 tkadw-0.1.3/tkadw/canvas/__pycache__/textbox.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2023-06-10 10:53:44.353940 tkadw-0.1.3/tkadw/canvas/adwite/__init__.py
+-rw-r--r--   0        0        0     1363 2023-06-10 11:23:03.996035 tkadw-0.1.3/tkadw/canvas/adwite/button.py
+-rw-r--r--   0        0        0       80 2023-06-09 13:54:04.880107 tkadw-0.1.3/tkadw/canvas/atomize/__init__.py
+-rw-r--r--   0        0        0     2520 2023-06-10 04:30:03.863844 tkadw-0.1.3/tkadw/canvas/atomize/button.py
+-rw-r--r--   0        0        0    17270 2023-06-23 04:54:52.447686 tkadw-0.1.3/tkadw/canvas/button.py
+-rw-r--r--   0        0        0    20382 2023-06-23 05:05:08.591410 tkadw-0.1.3/tkadw/canvas/drawengine.py
+-rw-r--r--   0        0        0    22377 2023-06-23 07:48:50.714445 tkadw-0.1.3/tkadw/canvas/entry.py
+-rw-r--r--   0        0        0      513 2023-06-09 23:26:21.009369 tkadw-0.1.3/tkadw/canvas/fluent/__init__.py
+-rw-r--r--   0        0        0     8629 2023-06-23 05:15:43.010231 tkadw-0.1.3/tkadw/canvas/frame.py
+-rw-r--r--   0        0        0     2051 2023-06-10 01:20:40.907297 tkadw-0.1.3/tkadw/canvas/fun.py
+-rw-r--r--   0        0        0    15490 2023-06-10 01:25:11.532315 tkadw-0.1.3/tkadw/canvas/fun2.py
+-rw-r--r--   0        0        0     8108 2023-06-10 01:29:02.970946 tkadw-0.1.3/tkadw/canvas/fun3.py
+-rw-r--r--   0        0        0     3202 2023-06-10 03:27:44.231516 tkadw-0.1.3/tkadw/canvas/fun4.py
+-rw-r--r--   0        0        0      942 2023-06-10 03:50:17.322506 tkadw-0.1.3/tkadw/canvas/fun5.py
+-rw-r--r--   0        0        0     9870 2023-06-10 07:36:40.103845 tkadw-0.1.3/tkadw/canvas/fun6.py
+-rw-r--r--   0        0        0     5690 2023-06-10 03:45:21.292347 tkadw-0.1.3/tkadw/canvas/poly.tcl
+-rw-r--r--   0        0        0    22443 2023-06-23 07:53:27.298479 tkadw-0.1.3/tkadw/canvas/textbox.py
+-rw-r--r--   0        0        0     4597 2023-05-27 23:04:22.860566 tkadw-0.1.3/tkadw/canvas/titlebar.py
+-rw-r--r--   0        0        0       29 2023-06-23 03:52:51.957932 tkadw-0.1.3/tkadw/tkite/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-23 03:52:52.129145 tkadw-0.1.3/tkadw/tkite/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      283 2023-06-23 07:44:06.875178 tkadw-0.1.3/tkadw/tkite/gtk/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-23 07:44:06.983012 tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5020 2023-06-23 05:37:39.419391 tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     2902 2023-06-23 05:36:24.094777 tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0     2457 2023-06-23 07:42:27.405172 tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0     3908 2023-06-23 07:45:23.356231 tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc
+-rw-r--r--   0        0        0     3898 2023-06-23 05:37:39.292931 tkadw-0.1.3/tkadw/tkite/gtk/button.py
+-rw-r--r--   0        0        0     2201 2023-06-23 05:36:23.978561 tkadw-0.1.3/tkadw/tkite/gtk/entry.py
+-rw-r--r--   0        0        0     1141 2023-06-23 07:40:36.374539 tkadw-0.1.3/tkadw/tkite/gtk/frame.py
+-rw-r--r--   0        0        0      500 2023-06-23 00:56:14.658098 tkadw-0.1.3/tkadw/tkite/gtk/notebook.py
+-rw-r--r--   0        0        0     2785 2023-06-23 07:45:23.240982 tkadw-0.1.3/tkadw/tkite/gtk/textbox.py
+-rw-r--r--   0        0        0        0 2023-06-09 14:28:28.424277 tkadw-0.1.3/tkadw/ttk/__init__.py
+-rw-r--r--   0        0        0      139 2023-06-09 14:38:22.776399 tkadw-0.1.3/tkadw/ttk/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1349 2023-06-09 14:41:39.497543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/__init__.py
+-rw-r--r--   0        0        0     2722 2023-06-09 14:43:18.298069 tkadw-0.1.3/tkadw/ttk/atomize_ttk/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2961 2023-06-09 14:41:39.498543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/sun-valley.tcl
+-rw-r--r--   0        0        0     5150 2023-05-14 15:25:00.266570 tkadw-0.1.3/tkadw/ttk/atomize_ttk/sv.tcl
+-rw-r--r--   0        0        0      270 2023-06-09 14:41:39.500545 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/arrow-down.png
+-rw-r--r--   0        0        0      261 2023-06-09 14:41:39.501544 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/arrow-right.png
+-rw-r--r--   0        0        0      274 2023-06-09 14:41:39.501544 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/arrow-up.png
+-rw-r--r--   0        0        0      262 2023-06-09 14:41:39.502544 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-accent-disabled.png
+-rw-r--r--   0        0        0      373 2023-06-09 14:41:39.503545 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-accent-hover.png
+-rw-r--r--   0        0        0      363 2023-06-09 14:41:39.503545 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-accent-pressed.png
+-rw-r--r--   0        0        0      377 2023-06-09 14:41:39.504545 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-accent-rest.png
+-rw-r--r--   0        0        0      274 2023-06-09 14:41:39.505542 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-close-hover.png
+-rw-r--r--   0        0        0      274 2023-06-09 14:41:39.505542 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-close-pressed.png
+-rw-r--r--   0        0        0      301 2023-06-09 14:41:39.506544 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-disabled.png
+-rw-r--r--   0        0        0      276 2023-06-09 14:41:39.506544 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-hover.png
+-rw-r--r--   0        0        0      288 2023-06-09 14:41:39.507543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-pressed.png
+-rw-r--r--   0        0        0      301 2023-06-09 14:41:39.508543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-rest.png
+-rw-r--r--   0        0        0      245 2023-06-09 14:41:39.508543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-titlebar-hover.png
+-rw-r--r--   0        0        0      238 2023-06-09 14:41:39.509543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-titlebar-pressed.png
+-rw-r--r--   0        0        0      386 2023-06-09 14:41:39.509543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/card.png
+-rw-r--r--   0        0        0      383 2023-06-09 14:41:39.510542 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-disabled.png
+-rw-r--r--   0        0        0      474 2023-06-09 14:41:39.511543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-hover.png
+-rw-r--r--   0        0        0      460 2023-06-09 14:41:39.511543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-pressed.png
+-rw-r--r--   0        0        0      475 2023-06-09 14:41:39.512544 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-rest.png
+-rw-r--r--   0        0        0      294 2023-06-09 14:41:39.513547 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-tri-disabled.png
+-rw-r--r--   0        0        0      362 2023-06-09 14:41:39.514132 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-tri-hover.png
+-rw-r--r--   0        0        0      358 2023-06-09 14:41:39.515137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-tri-pressed.png
+-rw-r--r--   0        0        0      363 2023-06-09 14:41:39.515137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-tri-rest.png
+-rw-r--r--   0        0        0      312 2023-06-09 14:41:39.516139 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-disabled.png
+-rw-r--r--   0        0        0      353 2023-06-09 14:41:39.517139 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-hover.png
+-rw-r--r--   0        0        0      302 2023-06-09 14:41:39.517139 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-pressed.png
+-rw-r--r--   0        0        0      353 2023-06-09 14:41:39.518137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-rest.png
+-rw-r--r--   0        0        0      129 2023-06-09 14:41:39.519137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/empty.png
+-rw-r--r--   0        0        0      273 2023-06-09 14:41:39.519137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/entry-disabled.png
+-rw-r--r--   0        0        0      335 2023-06-09 14:41:39.520136 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/entry-focus.png
+-rw-r--r--   0        0        0      269 2023-06-09 14:41:39.521137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/entry-hover.png
+-rw-r--r--   0        0        0      324 2023-06-09 14:41:39.522140 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/entry-invalid.png
+-rw-r--r--   0        0        0      297 2023-06-09 14:41:39.522140 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/entry-rest.png
+-rw-r--r--   0        0        0      337 2023-06-09 14:41:39.523139 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/notebook-border.png
+-rw-r--r--   0        0        0      186 2023-06-09 14:41:39.524139 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/notebook.png
+-rw-r--r--   0        0        0      193 2023-06-09 14:41:39.524139 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/progress-pbar-hor.png
+-rw-r--r--   0        0        0      214 2023-06-09 14:41:39.525137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/progress-pbar-vert.png
+-rw-r--r--   0        0        0      157 2023-06-09 14:41:39.526137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/progress-trough-hor.png
+-rw-r--r--   0        0        0      160 2023-06-09 14:41:39.526137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/progress-trough-vert.png
+-rw-r--r--   0        0        0      553 2023-06-09 14:41:39.527138 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-disabled.png
+-rw-r--r--   0        0        0      853 2023-06-09 14:41:39.527138 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-hover.png
+-rw-r--r--   0        0        0      786 2023-06-09 14:41:39.528137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-pressed.png
+-rw-r--r--   0        0        0      830 2023-06-09 14:41:39.528640 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-rest.png
+-rw-r--r--   0        0        0      552 2023-06-09 14:41:39.529647 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-disabled.png
+-rw-r--r--   0        0        0      602 2023-06-09 14:41:39.530644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-hover.png
+-rw-r--r--   0        0        0      616 2023-06-09 14:41:39.530644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-pressed.png
+-rw-r--r--   0        0        0      621 2023-06-09 14:41:39.531645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-rest.png
+-rw-r--r--   0        0        0      724 2023-06-09 14:41:39.532645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-disabled.png
+-rw-r--r--   0        0        0      808 2023-06-09 14:41:39.532645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-hover.png
+-rw-r--r--   0        0        0      735 2023-06-09 14:41:39.533645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-pressed.png
+-rw-r--r--   0        0        0      771 2023-06-09 14:41:39.533645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-rest.png
+-rw-r--r--   0        0        0      216 2023-06-09 14:41:39.534644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-trough-hor.png
+-rw-r--r--   0        0        0      215 2023-06-09 14:41:39.534644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-trough-vert.png
+-rw-r--r--   0        0        0      226 2023-06-09 14:41:39.535644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-down.png
+-rw-r--r--   0        0        0      254 2023-06-09 14:41:39.536643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-hor-thumb.png
+-rw-r--r--   0        0        0      338 2023-06-09 14:41:39.537644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-hor-trough.png
+-rw-r--r--   0        0        0      233 2023-06-09 14:41:39.538644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-left.png
+-rw-r--r--   0        0        0      227 2023-06-09 14:41:39.538644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-right.png
+-rw-r--r--   0        0        0      236 2023-06-09 14:41:39.539644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-up.png
+-rw-r--r--   0        0        0      264 2023-06-09 14:41:39.539644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-vert-thumb.png
+-rw-r--r--   0        0        0      343 2023-06-09 14:41:39.540644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-vert-trough.png
+-rw-r--r--   0        0        0      128 2023-06-09 14:41:39.541644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/separator.png
+-rw-r--r--   0        0        0      276 2023-06-09 14:41:39.542647 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/sizegrip.png
+-rw-r--r--   0        0        0      733 2023-06-09 14:41:39.542647 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-off-disabled.png
+-rw-r--r--   0        0        0      945 2023-06-09 14:41:39.543645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-off-hover.png
+-rw-r--r--   0        0        0      963 2023-06-09 14:41:39.544643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-off-pressed.png
+-rw-r--r--   0        0        0      895 2023-06-09 14:41:39.545645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-off-rest.png
+-rw-r--r--   0        0        0      623 2023-06-09 14:41:39.545645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-on-disabled.png
+-rw-r--r--   0        0        0      927 2023-06-09 14:41:39.546644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-on-hover.png
+-rw-r--r--   0        0        0      936 2023-06-09 14:41:39.547644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-on-pressed.png
+-rw-r--r--   0        0        0      859 2023-06-09 14:41:39.547644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-on-rest.png
+-rw-r--r--   0        0        0      265 2023-06-09 14:41:39.548643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/tab-hover.png
+-rw-r--r--   0        0        0      164 2023-06-09 14:41:39.549644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/tab-rest.png
+-rw-r--r--   0        0        0      319 2023-06-09 14:41:39.549644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/tab-selected.png
+-rw-r--r--   0        0        0      295 2023-06-09 14:41:39.550645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/treeheading-hover.png
+-rw-r--r--   0        0        0      317 2023-06-09 14:41:39.551644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/treeheading-pressed.png
+-rw-r--r--   0        0        0      321 2023-06-09 14:41:39.551644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/treeheading-rest.png
+-rw-r--r--   0        0        0    20188 2023-06-09 14:41:39.499549 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark.tcl
+-rw-r--r--   0        0        0      278 2023-06-09 14:41:39.552643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/arrow-down.png
+-rw-r--r--   0        0        0      273 2023-06-09 14:41:39.552643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/arrow-right.png
+-rw-r--r--   0        0        0      285 2023-06-09 14:41:39.553645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/arrow-up.png
+-rw-r--r--   0        0        0      271 2023-06-09 14:41:39.554647 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-accent-disabled.png
+-rw-r--r--   0        0        0      219 2023-06-09 14:48:51.766400 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-accent-hover.png
+-rw-r--r--   0        0        0      255 2023-06-09 14:53:14.082428 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-accent-pressed.png
+-rw-r--r--   0        0        0      217 2023-06-09 14:48:47.641380 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-accent-rest.png
+-rw-r--r--   0        0        0      326 2023-06-09 14:41:39.556644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-close-hover.png
+-rw-r--r--   0        0        0      316 2023-06-09 14:41:39.557644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-close-pressed.png
+-rw-r--r--   0        0        0      307 2023-06-09 14:41:39.557644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-disabled.png
+-rw-r--r--   0        0        0      306 2023-06-09 14:41:39.558645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-hover.png
+-rw-r--r--   0        0        0      289 2023-06-09 14:41:39.559644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-pressed.png
+-rw-r--r--   0        0        0      303 2023-06-09 14:41:39.559644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-rest.png
+-rw-r--r--   0        0        0      238 2023-06-09 14:41:39.560643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-titlebar-hover.png
+-rw-r--r--   0        0        0      225 2023-06-09 14:41:39.561643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-titlebar-pressed.png
+-rw-r--r--   0        0        0      479 2023-06-09 14:43:10.460434 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/card.png
+-rw-r--r--   0        0        0      381 2023-06-09 14:41:39.562646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-disabled.png
+-rw-r--r--   0        0        0      476 2023-06-09 14:41:39.562646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-hover.png
+-rw-r--r--   0        0        0      467 2023-06-09 14:41:39.563646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-pressed.png
+-rw-r--r--   0        0        0      473 2023-06-09 14:41:39.564644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-rest.png
+-rw-r--r--   0        0        0      299 2023-06-09 14:41:39.564644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-tri-disabled.png
+-rw-r--r--   0        0        0      365 2023-06-09 14:41:39.565643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-tri-hover.png
+-rw-r--r--   0        0        0      362 2023-06-09 14:41:39.566644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-tri-pressed.png
+-rw-r--r--   0        0        0      367 2023-06-09 14:41:39.566644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-tri-rest.png
+-rw-r--r--   0        0        0      324 2023-06-09 14:41:39.567644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-unsel-disabled.png
+-rw-r--r--   0        0        0      334 2023-06-09 14:41:39.568643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-unsel-hover.png
+-rw-r--r--   0        0        0      302 2023-06-09 14:41:39.568643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-unsel-pressed.png
+-rw-r--r--   0        0        0      333 2023-06-09 14:41:39.569646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-unsel-rest.png
+-rw-r--r--   0        0        0      129 2023-06-09 14:41:39.569646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/empty.png
+-rw-r--r--   0        0        0      289 2023-06-09 14:41:39.570644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/entry-disabled.png
+-rw-r--r--   0        0        0      331 2023-06-09 14:41:39.571647 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/entry-focus.png
+-rw-r--r--   0        0        0      302 2023-06-09 14:41:39.572644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/entry-hover.png
+-rw-r--r--   0        0        0      324 2023-06-09 14:41:39.572644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/entry-invalid.png
+-rw-r--r--   0        0        0      308 2023-06-09 14:41:39.573646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/entry-rest.png
+-rw-r--r--   0        0        0      298 2023-06-09 14:41:39.573646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/notebook-border.png
+-rw-r--r--   0        0        0      185 2023-06-09 14:41:39.574643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/notebook.png
+-rw-r--r--   0        0        0      192 2023-06-09 14:41:39.575643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/progress-pbar-hor.png
+-rw-r--r--   0        0        0      216 2023-06-09 14:41:39.575643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/progress-pbar-vert.png
+-rw-r--r--   0        0        0      158 2023-06-09 14:41:39.576643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/progress-trough-hor.png
+-rw-r--r--   0        0        0      161 2023-06-09 14:41:39.577644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/progress-trough-vert.png
+-rw-r--r--   0        0        0      523 2023-06-09 14:41:39.578645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-disabled.png
+-rw-r--r--   0        0        0      837 2023-06-09 14:41:39.578645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-hover.png
+-rw-r--r--   0        0        0      764 2023-06-09 14:41:39.579645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-pressed.png
+-rw-r--r--   0        0        0      773 2023-06-09 14:41:39.580644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-rest.png
+-rw-r--r--   0        0        0      521 2023-06-09 14:41:39.581644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-disabled.png
+-rw-r--r--   0        0        0      573 2023-06-09 14:41:39.582644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-hover.png
+-rw-r--r--   0        0        0      636 2023-06-09 14:41:39.582644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-pressed.png
+-rw-r--r--   0        0        0      576 2023-06-09 14:41:39.583644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-rest.png
+-rw-r--r--   0        0        0      658 2023-06-09 14:41:39.584643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-disabled.png
+-rw-r--r--   0        0        0      749 2023-06-09 14:41:39.584643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-hover.png
+-rw-r--r--   0        0        0      675 2023-06-09 14:41:39.585645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-pressed.png
+-rw-r--r--   0        0        0      701 2023-06-09 14:41:39.586645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-rest.png
+-rw-r--r--   0        0        0      208 2023-06-09 14:41:39.586645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-trough-hor.png
+-rw-r--r--   0        0        0      214 2023-06-09 14:41:39.587646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-trough-vert.png
+-rw-r--r--   0        0        0      229 2023-06-09 14:41:39.588644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-down.png
+-rw-r--r--   0        0        0      234 2023-06-09 14:41:39.589644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-hor-thumb.png
+-rw-r--r--   0        0        0      321 2023-06-09 14:41:39.589644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-hor-trough.png
+-rw-r--r--   0        0        0      232 2023-06-09 14:41:39.590644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-left.png
+-rw-r--r--   0        0        0      223 2023-06-09 14:41:39.590644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-right.png
+-rw-r--r--   0        0        0      237 2023-06-09 14:41:39.591643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-up.png
+-rw-r--r--   0        0        0      262 2023-06-09 14:41:39.592644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-vert-thumb.png
+-rw-r--r--   0        0        0      324 2023-06-09 14:41:39.593644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-vert-trough.png
+-rw-r--r--   0        0        0      128 2023-06-09 14:41:39.594646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/separator.png
+-rw-r--r--   0        0        0      272 2023-06-09 14:41:39.594646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/sizegrip.png
+-rw-r--r--   0        0        0      726 2023-06-09 14:41:39.595643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-off-disabled.png
+-rw-r--r--   0        0        0      867 2023-06-09 14:41:39.596647 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-off-hover.png
+-rw-r--r--   0        0        0      880 2023-06-09 14:41:39.597645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-off-pressed.png
+-rw-r--r--   0        0        0      814 2023-06-09 14:41:39.597645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-off-rest.png
+-rw-r--r--   0        0        0      590 2023-06-09 14:41:39.598645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-on-disabled.png
+-rw-r--r--   0        0        0      906 2023-06-09 14:41:39.598645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-on-hover.png
+-rw-r--r--   0        0        0      916 2023-06-09 14:41:39.599644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-on-pressed.png
+-rw-r--r--   0        0        0      857 2023-06-09 14:41:39.600643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-on-rest.png
+-rw-r--r--   0        0        0      295 2023-06-09 14:41:39.600643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/tab-hover.png
+-rw-r--r--   0        0        0      164 2023-06-09 14:41:39.601645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/tab-rest.png
+-rw-r--r--   0        0        0      318 2023-06-09 14:41:39.602649 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/tab-selected.png
+-rw-r--r--   0        0        0      338 2023-06-09 14:41:39.602649 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/treeheading-hover.png
+-rw-r--r--   0        0        0      318 2023-06-09 14:41:39.603646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/treeheading-pressed.png
+-rw-r--r--   0        0        0      330 2023-06-09 14:41:39.603646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/treeheading-rest.png
+-rw-r--r--   0        0        0    20371 2023-06-09 14:41:39.500545 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light.tcl
+-rw-r--r--   0        0        0     3045 2023-05-14 15:25:00.269895 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/sprites_dark.tcl
+-rw-r--r--   0        0        0     3092 2023-05-14 15:25:00.270897 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/sprites_light.tcl
+-rw-r--r--   0        0        0    18371 2023-05-14 15:25:00.272896 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/spritesheet_dark.png
+-rw-r--r--   0        0        0     2649 2023-06-09 14:36:51.668892 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/spritesheet_light.png
+-rw-r--r--   0        0        0    18462 2023-05-14 15:25:00.272896 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/spritesheet_light2.png
+-rw-r--r--   0        0        0      372 2023-06-09 14:40:30.166428 tkadw-0.1.3/tkadw/ttk/test.py
+-rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 tkadw-0.1.3/PKG-INFO
```

### Comparing `tkadw-0.1.2/tkadw/__main__.py` & `tkadw-0.1.3/tkadw/__main__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/appconfig.py` & `tkadw-0.1.3/tkadw/appconfig.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/__init__.py` & `tkadw-0.1.3/tkadw/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.1.3/tkadw/canvas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/__pycache__/button.cpython-311.pyc` & `tkadw-0.1.3/tkadw/canvas/__pycache__/button.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/__pycache__/button.cpython-38.pyc` & `tkadw-0.1.3/tkadw/canvas/__pycache__/button.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc` & `tkadw-0.1.3/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/__pycache__/entry.cpython-311.pyc` & `tkadw-0.1.3/tkadw/canvas/__pycache__/entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/__pycache__/frame.cpython-311.pyc` & `tkadw-0.1.3/tkadw/canvas/__pycache__/frame.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc` & `tkadw-0.1.3/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/__pycache__/textbox.cpython-311.pyc` & `tkadw-0.1.3/tkadw/canvas/__pycache__/textbox.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x624e9564 (Fri Jun 23 07:48:50 2023 UTC)
-files sz: 22421
+moddate:  0x774f9564 (Fri Jun 23 07:53:27 2023 UTC)
+files sz: 22443
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -379,56 +379,56 @@
                stacksize : 7
                flags     : 15
                code
                   0x9501870097000200740100000000000000000000a6000000ab00000000
                   00000000006a0100000000000000007c037c017c02640164029c037c04a4
                   018e010100640164036c026d037d05010074090000000000000000000064
                   04a6010000ab01000000000000000089005f05000000000000000002007c
-                  058900640189006a0500000000000000006405ac06a6040000ab04000000
-                  000000000089005f0600000000000000008900a007000000000000000000
-                  0000000000000000000000a6000000ab00000000000000000001008900a0
-                  080000000000000000000000000000000000000000a6000000ab00000000
-                  0000000000010089006a09000000000000000089005f0a00000000000000
-                  0089006a0b000000000000000089005f0c000000000000000089006a0d00
-                  0000000000000089005f0e000000000000000089006a0f00000000000000
-                  0089005f10000000000000000089006a11000000000000000089005f1200
-                  000000000000008900a01300000000000000000000000000000000000000
-                  00640789006a1400000000000000006408ac09a6030000ab030000000000
+                  058900640189006a05000000000000000064056401ac06a6050000ab0500
+                  0000000000000089005f0600000000000000008900a00700000000000000
+                  00000000000000000000000000a6000000ab000000000000000000010089
+                  00a0080000000000000000000000000000000000000000a6000000ab0000
+                  00000000000000010089006a09000000000000000089005f0a0000000000
+                  00000089006a0b000000000000000089005f0c000000000000000089006a
+                  0d000000000000000089005f0e000000000000000089006a0f0000000000
+                  00000089005f10000000000000000089006a11000000000000000089005f
+                  1200000000000000008900a0130000000000000000000000000000000000
+                  000000640789006a1400000000000000006408ac09a6030000ab03000000
+                  000000000001008900a01300000000000000000000000000000000000000
+                  00640a89006a1500000000000000006408ac09a6030000ab030000000000
                   00000001008900a013000000000000000000000000000000000000000064
-                  0a89006a1500000000000000006408ac09a6030000ab0300000000000000
-                  0001008900a0130000000000000000000000000000000000000000640b89
-                  006a1600000000000000006408ac09a6030000ab03000000000000000001
-                  008900a0130000000000000000000000000000000000000000640c89006a
-                  1700000000000000006408ac09a6030000ab030000000000000000010089
-                  00a0130000000000000000000000000000000000000000640d89006a1800
-                  000000000000006408ac09a6030000ab030000000000000000010089006a
-                  060000000000000000a01300000000000000000000000000000000000000
-                  00640d89006a1800000000000000006408ac09a6030000ab030000000000
-                  00000001008900a013000000000000000000000000000000000000000064
-                  0e89006a1900000000000000006408ac09a6030000ab0300000000000000
-                  00010089006a060000000000000000a01300000000000000000000000000
-                  00000000000000640e89006a1900000000000000006408ac09a6030000ab
-                  03000000000000000001008900a013000000000000000000000000000000
-                  0000000000640f88006601641084086408ac09a6030000ab030000000000
-                  00000001008900a013000000000000000000000000000000000000000064
-                  1188006601641284086408ac09a6030000ab030000000000000000010089
-                  00a013000000000000000000000000000000000000000064138800660164
-                  1484086408ac09a6030000ab03000000000000000001008900a013000000
-                  0000000000000000000000000000000000641588006601641684086408ac
-                  09a6030000ab030000000000000000010089006a060000000000000000a0
-                  130000000000000000000000000000000000000000640f88006601641784
-                  086408ac09a6030000ab030000000000000000010089006a060000000000
-                  000000a01300000000000000000000000000000000000000006411880066
-                  01641884086408ac09a6030000ab030000000000000000010089006a0600
-                  00000000000000a013000000000000000000000000000000000000000064
-                  1388006601641984086408ac09a6030000ab030000000000000000010089
+                  0b89006a1600000000000000006408ac09a6030000ab0300000000000000
+                  0001008900a0130000000000000000000000000000000000000000640c89
+                  006a1700000000000000006408ac09a6030000ab03000000000000000001
+                  008900a0130000000000000000000000000000000000000000640d89006a
+                  1800000000000000006408ac09a6030000ab030000000000000000010089
                   006a060000000000000000a0130000000000000000000000000000000000
-                  000000641588006601641a84086408ac09a6030000ab0300000000000000
-                  0001008900a01400000000000000000000000000000000000000006400a6
-                  010000ab010000000000000000010064005300
+                  000000640d89006a1800000000000000006408ac09a6030000ab03000000
+                  000000000001008900a01300000000000000000000000000000000000000
+                  00640e89006a1900000000000000006408ac09a6030000ab030000000000
+                  000000010089006a060000000000000000a0130000000000000000000000
+                  000000000000000000640e89006a1900000000000000006408ac09a60300
+                  00ab03000000000000000001008900a01300000000000000000000000000
+                  00000000000000640f88006601641084086408ac09a6030000ab03000000
+                  000000000001008900a01300000000000000000000000000000000000000
+                  00641188006601641284086408ac09a6030000ab03000000000000000001
+                  008900a01300000000000000000000000000000000000000006413880066
+                  01641484086408ac09a6030000ab03000000000000000001008900a01300
+                  000000000000000000000000000000000000006415880066016416840864
+                  08ac09a6030000ab030000000000000000010089006a0600000000000000
+                  00a0130000000000000000000000000000000000000000640f8800660164
+                  1784086408ac09a6030000ab030000000000000000010089006a06000000
+                  0000000000a0130000000000000000000000000000000000000000641188
+                  006601641884086408ac09a6030000ab030000000000000000010089006a
+                  060000000000000000a01300000000000000000000000000000000000000
+                  00641388006601641984086408ac09a6030000ab03000000000000000001
+                  0089006a060000000000000000a013000000000000000000000000000000
+                  0000000000641588006601641a84086408ac09a6030000ab030000000000
+                  00000001008900a014000000000000000000000000000000000000000064
+                  00a6010000ab010000000000000000010064005300
                              0 COPY_FREE_VARS           1
                              2 MAKE_CELL                0 (self)
                
                  7           4 RESUME                   0
                
                  9           6 PUSH_NULL
                              8 LOAD_GLOBAL              1 (NULL + super)
@@ -463,271 +463,272 @@
                 15         116 PUSH_NULL
                            118 LOAD_FAST                5 (Text)
                            120 LOAD_DEREF               0 (self)
                            122 LOAD_CONST               1 (0)
                            124 LOAD_DEREF               0 (self)
                            126 LOAD_ATTR                5 (text_text_font)
                            136 LOAD_CONST               5 (True)
-                           138 KW_NAMES                 6
-                           140 PRECALL                  4
-                           144 CALL                     4
-                           154 LOAD_DEREF               0 (self)
-                           156 STORE_ATTR               6 (text)
-               
-                17         166 LOAD_DEREF               0 (self)
-                           168 LOAD_METHOD              7 (_other)
-                           190 PRECALL                  0
-                           194 CALL                     0
-                           204 POP_TOP
-               
-                19         206 LOAD_DEREF               0 (self)
-                           208 LOAD_METHOD              8 (default_palette)
-                           230 PRECALL                  0
-                           234 CALL                     0
-                           244 POP_TOP
-               
-                21         246 LOAD_DEREF               0 (self)
-                           248 LOAD_ATTR                9 (text_back)
-                           258 LOAD_DEREF               0 (self)
-                           260 STORE_ATTR              10 (_text_back)
-               
-                22         270 LOAD_DEREF               0 (self)
-                           272 LOAD_ATTR               11 (text_border)
-                           282 LOAD_DEREF               0 (self)
-                           284 STORE_ATTR              12 (_text_border)
-               
-                23         294 LOAD_DEREF               0 (self)
-                           296 LOAD_ATTR               13 (text_text_back)
-                           306 LOAD_DEREF               0 (self)
-                           308 STORE_ATTR              14 (_text_text_back)
-               
-                24         318 LOAD_DEREF               0 (self)
-                           320 LOAD_ATTR               15 (text_bottom_line)
-                           330 LOAD_DEREF               0 (self)
-                           332 STORE_ATTR              16 (_text_bottom_line)
-               
-                25         342 LOAD_DEREF               0 (self)
-                           344 LOAD_ATTR               17 (text_bottom_width)
-                           354 LOAD_DEREF               0 (self)
-                           356 STORE_ATTR              18 (_text_bottom_width)
-               
-                27         366 LOAD_DEREF               0 (self)
-                           368 LOAD_METHOD             19 (bind)
-                           390 LOAD_CONST               7 ('<Configure>')
-                           392 LOAD_DEREF               0 (self)
-                           394 LOAD_ATTR               20 (_draw)
-                           404 LOAD_CONST               8 ('+')
-                           406 KW_NAMES                 9
-                           408 PRECALL                  3
-                           412 CALL                     3
-                           422 POP_TOP
-               
-                28         424 LOAD_DEREF               0 (self)
-                           426 LOAD_METHOD             19 (bind)
-                           448 LOAD_CONST              10 ('<Button>')
-                           450 LOAD_DEREF               0 (self)
-                           452 LOAD_ATTR               21 (_click)
-                           462 LOAD_CONST               8 ('+')
-                           464 KW_NAMES                 9
-                           466 PRECALL                  3
-                           470 CALL                     3
-                           480 POP_TOP
-               
-                29         482 LOAD_DEREF               0 (self)
-                           484 LOAD_METHOD             19 (bind)
-                           506 LOAD_CONST              11 ('<Enter>')
-                           508 LOAD_DEREF               0 (self)
-                           510 LOAD_ATTR               22 (_hover)
-                           520 LOAD_CONST               8 ('+')
-                           522 KW_NAMES                 9
-                           524 PRECALL                  3
-                           528 CALL                     3
-                           538 POP_TOP
-               
-                30         540 LOAD_DEREF               0 (self)
-                           542 LOAD_METHOD             19 (bind)
-                           564 LOAD_CONST              12 ('<Leave>')
-                           566 LOAD_DEREF               0 (self)
-                           568 LOAD_ATTR               23 (_hover_release)
-                           578 LOAD_CONST               8 ('+')
-                           580 KW_NAMES                 9
-                           582 PRECALL                  3
-                           586 CALL                     3
-                           596 POP_TOP
-               
-                31         598 LOAD_DEREF               0 (self)
-                           600 LOAD_METHOD             19 (bind)
-                           622 LOAD_CONST              13 ('<FocusIn>')
-                           624 LOAD_DEREF               0 (self)
-                           626 LOAD_ATTR               24 (_focus)
-                           636 LOAD_CONST               8 ('+')
-                           638 KW_NAMES                 9
-                           640 PRECALL                  3
-                           644 CALL                     3
-                           654 POP_TOP
-               
-                32         656 LOAD_DEREF               0 (self)
-                           658 LOAD_ATTR                6 (text)
-                           668 LOAD_METHOD             19 (bind)
-                           690 LOAD_CONST              13 ('<FocusIn>')
-                           692 LOAD_DEREF               0 (self)
-                           694 LOAD_ATTR               24 (_focus)
-                           704 LOAD_CONST               8 ('+')
-                           706 KW_NAMES                 9
-                           708 PRECALL                  3
-                           712 CALL                     3
-                           722 POP_TOP
-               
-                33         724 LOAD_DEREF               0 (self)
-                           726 LOAD_METHOD             19 (bind)
-                           748 LOAD_CONST              14 ('<FocusOut>')
-                           750 LOAD_DEREF               0 (self)
-                           752 LOAD_ATTR               25 (_focusout)
-                           762 LOAD_CONST               8 ('+')
-                           764 KW_NAMES                 9
-                           766 PRECALL                  3
-                           770 CALL                     3
-                           780 POP_TOP
-               
-                34         782 LOAD_DEREF               0 (self)
-                           784 LOAD_ATTR                6 (text)
-                           794 LOAD_METHOD             19 (bind)
-                           816 LOAD_CONST              14 ('<FocusOut>')
-                           818 LOAD_DEREF               0 (self)
-                           820 LOAD_ATTR               25 (_focusout)
-                           830 LOAD_CONST               8 ('+')
-                           832 KW_NAMES                 9
-                           834 PRECALL                  3
-                           838 CALL                     3
-                           848 POP_TOP
-               
-                36         850 LOAD_DEREF               0 (self)
-                           852 LOAD_METHOD             19 (bind)
-                           874 LOAD_CONST              15 ('<Control-z>')
-                           876 LOAD_CLOSURE             0 (self)
-                           878 BUILD_TUPLE              1
-                           880 LOAD_CONST              16 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 36>)
-                           882 MAKE_FUNCTION            8 (closure)
-                           884 LOAD_CONST               8 ('+')
-                           886 KW_NAMES                 9
-                           888 PRECALL                  3
-                           892 CALL                     3
-                           902 POP_TOP
-               
-                37         904 LOAD_DEREF               0 (self)
-                           906 LOAD_METHOD             19 (bind)
-                           928 LOAD_CONST              17 ('<Control-Z>')
-                           930 LOAD_CLOSURE             0 (self)
-                           932 BUILD_TUPLE              1
-                           934 LOAD_CONST              18 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 37>)
-                           936 MAKE_FUNCTION            8 (closure)
-                           938 LOAD_CONST               8 ('+')
-                           940 KW_NAMES                 9
-                           942 PRECALL                  3
-                           946 CALL                     3
-                           956 POP_TOP
-               
-                38         958 LOAD_DEREF               0 (self)
-                           960 LOAD_METHOD             19 (bind)
-                           982 LOAD_CONST              19 ('<Control-Shift-z>')
-                           984 LOAD_CLOSURE             0 (self)
-                           986 BUILD_TUPLE              1
-                           988 LOAD_CONST              20 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 38>)
-                           990 MAKE_FUNCTION            8 (closure)
-                           992 LOAD_CONST               8 ('+')
-                           994 KW_NAMES                 9
-                           996 PRECALL                  3
-                          1000 CALL                     3
-                          1010 POP_TOP
-               
-                39        1012 LOAD_DEREF               0 (self)
-                          1014 LOAD_METHOD             19 (bind)
-                          1036 LOAD_CONST              21 ('<Control-Shift-Z>')
-                          1038 LOAD_CLOSURE             0 (self)
-                          1040 BUILD_TUPLE              1
-                          1042 LOAD_CONST              22 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 39>)
-                          1044 MAKE_FUNCTION            8 (closure)
-                          1046 LOAD_CONST               8 ('+')
-                          1048 KW_NAMES                 9
-                          1050 PRECALL                  3
-                          1054 CALL                     3
-                          1064 POP_TOP
-               
-                41        1066 LOAD_DEREF               0 (self)
-                          1068 LOAD_ATTR                6 (text)
-                          1078 LOAD_METHOD             19 (bind)
-                          1100 LOAD_CONST              15 ('<Control-z>')
-                          1102 LOAD_CLOSURE             0 (self)
-                          1104 BUILD_TUPLE              1
-                          1106 LOAD_CONST              23 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 41>)
-                          1108 MAKE_FUNCTION            8 (closure)
-                          1110 LOAD_CONST               8 ('+')
-                          1112 KW_NAMES                 9
-                          1114 PRECALL                  3
-                          1118 CALL                     3
-                          1128 POP_TOP
-               
-                42        1130 LOAD_DEREF               0 (self)
-                          1132 LOAD_ATTR                6 (text)
-                          1142 LOAD_METHOD             19 (bind)
-                          1164 LOAD_CONST              17 ('<Control-Z>')
-                          1166 LOAD_CLOSURE             0 (self)
-                          1168 BUILD_TUPLE              1
-                          1170 LOAD_CONST              24 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 42>)
-                          1172 MAKE_FUNCTION            8 (closure)
-                          1174 LOAD_CONST               8 ('+')
-                          1176 KW_NAMES                 9
-                          1178 PRECALL                  3
-                          1182 CALL                     3
-                          1192 POP_TOP
-               
-                43        1194 LOAD_DEREF               0 (self)
-                          1196 LOAD_ATTR                6 (text)
-                          1206 LOAD_METHOD             19 (bind)
-                          1228 LOAD_CONST              19 ('<Control-Shift-z>')
-                          1230 LOAD_CLOSURE             0 (self)
-                          1232 BUILD_TUPLE              1
-                          1234 LOAD_CONST              25 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 43>)
-                          1236 MAKE_FUNCTION            8 (closure)
-                          1238 LOAD_CONST               8 ('+')
-                          1240 KW_NAMES                 9
-                          1242 PRECALL                  3
-                          1246 CALL                     3
-                          1256 POP_TOP
-               
-                44        1258 LOAD_DEREF               0 (self)
-                          1260 LOAD_ATTR                6 (text)
-                          1270 LOAD_METHOD             19 (bind)
-                          1292 LOAD_CONST              21 ('<Control-Shift-Z>')
-                          1294 LOAD_CLOSURE             0 (self)
-                          1296 BUILD_TUPLE              1
-                          1298 LOAD_CONST              26 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 44>)
-                          1300 MAKE_FUNCTION            8 (closure)
-                          1302 LOAD_CONST               8 ('+')
-                          1304 KW_NAMES                 9
-                          1306 PRECALL                  3
-                          1310 CALL                     3
-                          1320 POP_TOP
-               
-                46        1322 LOAD_DEREF               0 (self)
-                          1324 LOAD_METHOD             20 (_draw)
-                          1346 LOAD_CONST               0 (None)
-                          1348 PRECALL                  1
-                          1352 CALL                     1
-                          1362 POP_TOP
-                          1364 LOAD_CONST               0 (None)
-                          1366 RETURN_VALUE
+                           138 LOAD_CONST               1 (0)
+                           140 KW_NAMES                 6
+                           142 PRECALL                  5
+                           146 CALL                     5
+                           156 LOAD_DEREF               0 (self)
+                           158 STORE_ATTR               6 (text)
+               
+                17         168 LOAD_DEREF               0 (self)
+                           170 LOAD_METHOD              7 (_other)
+                           192 PRECALL                  0
+                           196 CALL                     0
+                           206 POP_TOP
+               
+                19         208 LOAD_DEREF               0 (self)
+                           210 LOAD_METHOD              8 (default_palette)
+                           232 PRECALL                  0
+                           236 CALL                     0
+                           246 POP_TOP
+               
+                21         248 LOAD_DEREF               0 (self)
+                           250 LOAD_ATTR                9 (text_back)
+                           260 LOAD_DEREF               0 (self)
+                           262 STORE_ATTR              10 (_text_back)
+               
+                22         272 LOAD_DEREF               0 (self)
+                           274 LOAD_ATTR               11 (text_border)
+                           284 LOAD_DEREF               0 (self)
+                           286 STORE_ATTR              12 (_text_border)
+               
+                23         296 LOAD_DEREF               0 (self)
+                           298 LOAD_ATTR               13 (text_text_back)
+                           308 LOAD_DEREF               0 (self)
+                           310 STORE_ATTR              14 (_text_text_back)
+               
+                24         320 LOAD_DEREF               0 (self)
+                           322 LOAD_ATTR               15 (text_bottom_line)
+                           332 LOAD_DEREF               0 (self)
+                           334 STORE_ATTR              16 (_text_bottom_line)
+               
+                25         344 LOAD_DEREF               0 (self)
+                           346 LOAD_ATTR               17 (text_bottom_width)
+                           356 LOAD_DEREF               0 (self)
+                           358 STORE_ATTR              18 (_text_bottom_width)
+               
+                27         368 LOAD_DEREF               0 (self)
+                           370 LOAD_METHOD             19 (bind)
+                           392 LOAD_CONST               7 ('<Configure>')
+                           394 LOAD_DEREF               0 (self)
+                           396 LOAD_ATTR               20 (_draw)
+                           406 LOAD_CONST               8 ('+')
+                           408 KW_NAMES                 9
+                           410 PRECALL                  3
+                           414 CALL                     3
+                           424 POP_TOP
+               
+                28         426 LOAD_DEREF               0 (self)
+                           428 LOAD_METHOD             19 (bind)
+                           450 LOAD_CONST              10 ('<Button>')
+                           452 LOAD_DEREF               0 (self)
+                           454 LOAD_ATTR               21 (_click)
+                           464 LOAD_CONST               8 ('+')
+                           466 KW_NAMES                 9
+                           468 PRECALL                  3
+                           472 CALL                     3
+                           482 POP_TOP
+               
+                29         484 LOAD_DEREF               0 (self)
+                           486 LOAD_METHOD             19 (bind)
+                           508 LOAD_CONST              11 ('<Enter>')
+                           510 LOAD_DEREF               0 (self)
+                           512 LOAD_ATTR               22 (_hover)
+                           522 LOAD_CONST               8 ('+')
+                           524 KW_NAMES                 9
+                           526 PRECALL                  3
+                           530 CALL                     3
+                           540 POP_TOP
+               
+                30         542 LOAD_DEREF               0 (self)
+                           544 LOAD_METHOD             19 (bind)
+                           566 LOAD_CONST              12 ('<Leave>')
+                           568 LOAD_DEREF               0 (self)
+                           570 LOAD_ATTR               23 (_hover_release)
+                           580 LOAD_CONST               8 ('+')
+                           582 KW_NAMES                 9
+                           584 PRECALL                  3
+                           588 CALL                     3
+                           598 POP_TOP
+               
+                31         600 LOAD_DEREF               0 (self)
+                           602 LOAD_METHOD             19 (bind)
+                           624 LOAD_CONST              13 ('<FocusIn>')
+                           626 LOAD_DEREF               0 (self)
+                           628 LOAD_ATTR               24 (_focus)
+                           638 LOAD_CONST               8 ('+')
+                           640 KW_NAMES                 9
+                           642 PRECALL                  3
+                           646 CALL                     3
+                           656 POP_TOP
+               
+                32         658 LOAD_DEREF               0 (self)
+                           660 LOAD_ATTR                6 (text)
+                           670 LOAD_METHOD             19 (bind)
+                           692 LOAD_CONST              13 ('<FocusIn>')
+                           694 LOAD_DEREF               0 (self)
+                           696 LOAD_ATTR               24 (_focus)
+                           706 LOAD_CONST               8 ('+')
+                           708 KW_NAMES                 9
+                           710 PRECALL                  3
+                           714 CALL                     3
+                           724 POP_TOP
+               
+                33         726 LOAD_DEREF               0 (self)
+                           728 LOAD_METHOD             19 (bind)
+                           750 LOAD_CONST              14 ('<FocusOut>')
+                           752 LOAD_DEREF               0 (self)
+                           754 LOAD_ATTR               25 (_focusout)
+                           764 LOAD_CONST               8 ('+')
+                           766 KW_NAMES                 9
+                           768 PRECALL                  3
+                           772 CALL                     3
+                           782 POP_TOP
+               
+                34         784 LOAD_DEREF               0 (self)
+                           786 LOAD_ATTR                6 (text)
+                           796 LOAD_METHOD             19 (bind)
+                           818 LOAD_CONST              14 ('<FocusOut>')
+                           820 LOAD_DEREF               0 (self)
+                           822 LOAD_ATTR               25 (_focusout)
+                           832 LOAD_CONST               8 ('+')
+                           834 KW_NAMES                 9
+                           836 PRECALL                  3
+                           840 CALL                     3
+                           850 POP_TOP
+               
+                36         852 LOAD_DEREF               0 (self)
+                           854 LOAD_METHOD             19 (bind)
+                           876 LOAD_CONST              15 ('<Control-z>')
+                           878 LOAD_CLOSURE             0 (self)
+                           880 BUILD_TUPLE              1
+                           882 LOAD_CONST              16 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 36>)
+                           884 MAKE_FUNCTION            8 (closure)
+                           886 LOAD_CONST               8 ('+')
+                           888 KW_NAMES                 9
+                           890 PRECALL                  3
+                           894 CALL                     3
+                           904 POP_TOP
+               
+                37         906 LOAD_DEREF               0 (self)
+                           908 LOAD_METHOD             19 (bind)
+                           930 LOAD_CONST              17 ('<Control-Z>')
+                           932 LOAD_CLOSURE             0 (self)
+                           934 BUILD_TUPLE              1
+                           936 LOAD_CONST              18 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 37>)
+                           938 MAKE_FUNCTION            8 (closure)
+                           940 LOAD_CONST               8 ('+')
+                           942 KW_NAMES                 9
+                           944 PRECALL                  3
+                           948 CALL                     3
+                           958 POP_TOP
+               
+                38         960 LOAD_DEREF               0 (self)
+                           962 LOAD_METHOD             19 (bind)
+                           984 LOAD_CONST              19 ('<Control-Shift-z>')
+                           986 LOAD_CLOSURE             0 (self)
+                           988 BUILD_TUPLE              1
+                           990 LOAD_CONST              20 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 38>)
+                           992 MAKE_FUNCTION            8 (closure)
+                           994 LOAD_CONST               8 ('+')
+                           996 KW_NAMES                 9
+                           998 PRECALL                  3
+                          1002 CALL                     3
+                          1012 POP_TOP
+               
+                39        1014 LOAD_DEREF               0 (self)
+                          1016 LOAD_METHOD             19 (bind)
+                          1038 LOAD_CONST              21 ('<Control-Shift-Z>')
+                          1040 LOAD_CLOSURE             0 (self)
+                          1042 BUILD_TUPLE              1
+                          1044 LOAD_CONST              22 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 39>)
+                          1046 MAKE_FUNCTION            8 (closure)
+                          1048 LOAD_CONST               8 ('+')
+                          1050 KW_NAMES                 9
+                          1052 PRECALL                  3
+                          1056 CALL                     3
+                          1066 POP_TOP
+               
+                41        1068 LOAD_DEREF               0 (self)
+                          1070 LOAD_ATTR                6 (text)
+                          1080 LOAD_METHOD             19 (bind)
+                          1102 LOAD_CONST              15 ('<Control-z>')
+                          1104 LOAD_CLOSURE             0 (self)
+                          1106 BUILD_TUPLE              1
+                          1108 LOAD_CONST              23 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 41>)
+                          1110 MAKE_FUNCTION            8 (closure)
+                          1112 LOAD_CONST               8 ('+')
+                          1114 KW_NAMES                 9
+                          1116 PRECALL                  3
+                          1120 CALL                     3
+                          1130 POP_TOP
+               
+                42        1132 LOAD_DEREF               0 (self)
+                          1134 LOAD_ATTR                6 (text)
+                          1144 LOAD_METHOD             19 (bind)
+                          1166 LOAD_CONST              17 ('<Control-Z>')
+                          1168 LOAD_CLOSURE             0 (self)
+                          1170 BUILD_TUPLE              1
+                          1172 LOAD_CONST              24 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 42>)
+                          1174 MAKE_FUNCTION            8 (closure)
+                          1176 LOAD_CONST               8 ('+')
+                          1178 KW_NAMES                 9
+                          1180 PRECALL                  3
+                          1184 CALL                     3
+                          1194 POP_TOP
+               
+                43        1196 LOAD_DEREF               0 (self)
+                          1198 LOAD_ATTR                6 (text)
+                          1208 LOAD_METHOD             19 (bind)
+                          1230 LOAD_CONST              19 ('<Control-Shift-z>')
+                          1232 LOAD_CLOSURE             0 (self)
+                          1234 BUILD_TUPLE              1
+                          1236 LOAD_CONST              25 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 43>)
+                          1238 MAKE_FUNCTION            8 (closure)
+                          1240 LOAD_CONST               8 ('+')
+                          1242 KW_NAMES                 9
+                          1244 PRECALL                  3
+                          1248 CALL                     3
+                          1258 POP_TOP
+               
+                44        1260 LOAD_DEREF               0 (self)
+                          1262 LOAD_ATTR                6 (text)
+                          1272 LOAD_METHOD             19 (bind)
+                          1294 LOAD_CONST              21 ('<Control-Shift-Z>')
+                          1296 LOAD_CLOSURE             0 (self)
+                          1298 BUILD_TUPLE              1
+                          1300 LOAD_CONST              26 (<code object <lambda>, file "D:\tkadw\tkadw\canvas\textbox.py", line 44>)
+                          1302 MAKE_FUNCTION            8 (closure)
+                          1304 LOAD_CONST               8 ('+')
+                          1306 KW_NAMES                 9
+                          1308 PRECALL                  3
+                          1312 CALL                     3
+                          1322 POP_TOP
+               
+                46        1324 LOAD_DEREF               0 (self)
+                          1326 LOAD_METHOD             20 (_draw)
+                          1348 LOAD_CONST               0 (None)
+                          1350 PRECALL                  1
+                          1354 CALL                     1
+                          1364 POP_TOP
+                          1366 LOAD_CONST               0 (None)
+                          1368 RETURN_VALUE
                consts
                   None
                   0
                   ('width', 'height', 'highlightthickness')
                   ('Text',)
                   'TkDefaultFont'
                   True
-                  ('bd', 'font', 'undo')
+                  ('bd', 'font', 'undo', 'highlightthickness')
                   '<Configure>'
                   '+'
                   ('add',)
                   '<Button>'
                   '<Enter>'
                   '<Leave>'
                   '<FocusIn>'
@@ -948,15 +949,15 @@
                varnames   ('self', 'width', 'height', 'args', 'kwargs', 'Text')
                freevars   ('__class__',)
                cellvars   ('self',)
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '__init__'
                firstlineno 7
                lnotab
-                  0x06023a020c022802320228022802180118011801180118023a013a013a
+                  0x06023a020c022802340228022802180118011801180118023a013a013a
                   013a013a0144013a01440236013601360136024001400140014002
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
```

### Comparing `tkadw-0.1.2/tkadw/canvas/adwite/button.py` & `tkadw-0.1.3/tkadw/canvas/adwite/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/atomize/button.py` & `tkadw-0.1.3/tkadw/canvas/atomize/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/button.py` & `tkadw-0.1.3/tkadw/canvas/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/drawengine.py` & `tkadw-0.1.3/tkadw/canvas/drawengine.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/entry.py` & `tkadw-0.1.3/tkadw/canvas/entry.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/fluent/__init__.py` & `tkadw-0.1.3/tkadw/canvas/fluent/__init__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/frame.py` & `tkadw-0.1.3/tkadw/canvas/frame.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/fun.py` & `tkadw-0.1.3/tkadw/canvas/fun.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/fun2.py` & `tkadw-0.1.3/tkadw/canvas/fun2.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/fun3.py` & `tkadw-0.1.3/tkadw/canvas/fun3.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/fun4.py` & `tkadw-0.1.3/tkadw/canvas/fun4.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/fun5.py` & `tkadw-0.1.3/tkadw/canvas/fun5.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/fun6.py` & `tkadw-0.1.3/tkadw/canvas/fun6.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/poly.tcl` & `tkadw-0.1.3/tkadw/canvas/poly.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/canvas/textbox.py` & `tkadw-0.1.3/tkadw/canvas/textbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
         super().__init__(*args, width=width, height=height, highlightthickness=0, **kwargs)
 
         from tkinter import Text
 
         self.text_text_font = nametofont("TkDefaultFont")
 
-        self.text = Text(self, bd=0, font=self.text_text_font, undo=True)
+        self.text = Text(self, bd=0, font=self.text_text_font, undo=True, highlightthickness=0)
 
         self._other()
 
         self.default_palette()
 
         self._text_back = self.text_back
         self._text_border = self.text_border
```

### Comparing `tkadw-0.1.2/tkadw/canvas/titlebar.py` & `tkadw-0.1.3/tkadw/canvas/titlebar.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc` & `tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc` & `tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc` & `tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc` & `tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/tkite/gtk/button.py` & `tkadw-0.1.3/tkadw/tkite/gtk/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/tkite/gtk/entry.py` & `tkadw-0.1.3/tkadw/tkite/gtk/entry.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/tkite/gtk/frame.py` & `tkadw-0.1.3/tkadw/tkite/gtk/frame.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/tkite/gtk/textbox.py` & `tkadw-0.1.3/tkadw/tkite/gtk/textbox.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/__init__.py` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/__init__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/sun-valley.tcl` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/sun-valley.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/sv.tcl` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/sv.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-disabled.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-hover.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-pressed.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-rest.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-disabled.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-hover.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-pressed.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-rest.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-disabled.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-hover.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-pressed.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-rest.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-disabled.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-off-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-hover.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-off-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-pressed.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-off-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-off-rest.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-off-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-disabled.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-on-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-hover.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-on-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-pressed.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-on-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark/switch-on-rest.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-on-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/dark.tcl` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-disabled.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-hover.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-pressed.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-rest.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-disabled.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-hover.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-pressed.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-rest.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-disabled.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-hover.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-pressed.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-rest.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-disabled.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-off-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-hover.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-off-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-pressed.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-off-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-off-rest.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-off-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-disabled.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-on-disabled.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-hover.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-on-hover.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-pressed.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-on-pressed.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light/switch-on-rest.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-on-rest.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/light.tcl` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/sprites_dark.tcl` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/sprites_dark.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/sprites_light.tcl` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/sprites_light.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/spritesheet_dark.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/spritesheet_dark.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/spritesheet_light.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/spritesheet_light.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/tkadw/ttk/atomize_ttk/theme/spritesheet_light2.png` & `tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/spritesheet_light2.png`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.2/PKG-INFO` & `tkadw-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkadw
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: XiangQinxi
 Author-email: 1379773753@qq.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

