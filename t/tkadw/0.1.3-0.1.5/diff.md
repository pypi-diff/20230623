# Comparing `tmp/tkadw-0.1.3.tar.gz` & `tmp/tkadw-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkadw-0.1.3.tar", max compression
+gzip compressed data, was "tkadw-0.1.5.tar", max compression
```

## Comparing `tkadw-0.1.3.tar` & `tkadw-0.1.5.tar`

### file list

```diff
@@ -1,218 +1,48 @@
--rw-r--r--   0        0        0      272 2023-06-23 07:54:02.049872 tkadw-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      101 2023-04-15 23:36:06.262325 tkadw-0.1.3/README.md
--rw-r--r--   0        0        0      112 2023-06-23 03:45:25.577456 tkadw-0.1.3/tkadw/__init__.py
--rw-r--r--   0        0        0      948 2023-06-23 07:49:26.692233 tkadw-0.1.3/tkadw/__main__.py
--rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.1.3/tkadw/app.config
--rw-r--r--   0        0        0      940 2023-06-09 11:52:45.801259 tkadw-0.1.3/tkadw/appconfig.py
--rw-r--r--   0        0        0      896 2023-06-23 07:36:10.506439 tkadw-0.1.3/tkadw/canvas/__init__.py
--rw-r--r--   0        0        0     1701 2023-06-23 07:38:42.890718 tkadw-0.1.3/tkadw/canvas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      124 2023-04-15 23:20:17.035856 tkadw-0.1.3/tkadw/canvas/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0    22885 2023-06-23 04:54:52.588047 tkadw-0.1.3/tkadw/canvas/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0     3479 2023-04-15 23:20:17.037902 tkadw-0.1.3/tkadw/canvas/__pycache__/button.cpython-38.pyc
--rw-r--r--   0        0        0    23239 2023-06-23 05:05:08.679421 tkadw-0.1.3/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc
--rw-r--r--   0        0        0    25982 2023-06-23 07:48:50.831965 tkadw-0.1.3/tkadw/canvas/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0    13288 2023-06-23 07:38:42.954769 tkadw-0.1.3/tkadw/canvas/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.1.3/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0        0        0    27824 2023-06-23 07:53:35.555717 tkadw-0.1.3/tkadw/canvas/__pycache__/textbox.cpython-311.pyc
--rw-r--r--   0        0        0        0 2023-06-10 10:53:44.353940 tkadw-0.1.3/tkadw/canvas/adwite/__init__.py
--rw-r--r--   0        0        0     1363 2023-06-10 11:23:03.996035 tkadw-0.1.3/tkadw/canvas/adwite/button.py
--rw-r--r--   0        0        0       80 2023-06-09 13:54:04.880107 tkadw-0.1.3/tkadw/canvas/atomize/__init__.py
--rw-r--r--   0        0        0     2520 2023-06-10 04:30:03.863844 tkadw-0.1.3/tkadw/canvas/atomize/button.py
--rw-r--r--   0        0        0    17270 2023-06-23 04:54:52.447686 tkadw-0.1.3/tkadw/canvas/button.py
--rw-r--r--   0        0        0    20382 2023-06-23 05:05:08.591410 tkadw-0.1.3/tkadw/canvas/drawengine.py
--rw-r--r--   0        0        0    22377 2023-06-23 07:48:50.714445 tkadw-0.1.3/tkadw/canvas/entry.py
--rw-r--r--   0        0        0      513 2023-06-09 23:26:21.009369 tkadw-0.1.3/tkadw/canvas/fluent/__init__.py
--rw-r--r--   0        0        0     8629 2023-06-23 05:15:43.010231 tkadw-0.1.3/tkadw/canvas/frame.py
--rw-r--r--   0        0        0     2051 2023-06-10 01:20:40.907297 tkadw-0.1.3/tkadw/canvas/fun.py
--rw-r--r--   0        0        0    15490 2023-06-10 01:25:11.532315 tkadw-0.1.3/tkadw/canvas/fun2.py
--rw-r--r--   0        0        0     8108 2023-06-10 01:29:02.970946 tkadw-0.1.3/tkadw/canvas/fun3.py
--rw-r--r--   0        0        0     3202 2023-06-10 03:27:44.231516 tkadw-0.1.3/tkadw/canvas/fun4.py
--rw-r--r--   0        0        0      942 2023-06-10 03:50:17.322506 tkadw-0.1.3/tkadw/canvas/fun5.py
--rw-r--r--   0        0        0     9870 2023-06-10 07:36:40.103845 tkadw-0.1.3/tkadw/canvas/fun6.py
--rw-r--r--   0        0        0     5690 2023-06-10 03:45:21.292347 tkadw-0.1.3/tkadw/canvas/poly.tcl
--rw-r--r--   0        0        0    22443 2023-06-23 07:53:27.298479 tkadw-0.1.3/tkadw/canvas/textbox.py
--rw-r--r--   0        0        0     4597 2023-05-27 23:04:22.860566 tkadw-0.1.3/tkadw/canvas/titlebar.py
--rw-r--r--   0        0        0       29 2023-06-23 03:52:51.957932 tkadw-0.1.3/tkadw/tkite/__init__.py
--rw-r--r--   0        0        0      181 2023-06-23 03:52:52.129145 tkadw-0.1.3/tkadw/tkite/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      283 2023-06-23 07:44:06.875178 tkadw-0.1.3/tkadw/tkite/gtk/__init__.py
--rw-r--r--   0        0        0      620 2023-06-23 07:44:06.983012 tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5020 2023-06-23 05:37:39.419391 tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc
--rw-r--r--   0        0        0     2902 2023-06-23 05:36:24.094777 tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc
--rw-r--r--   0        0        0     2457 2023-06-23 07:42:27.405172 tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc
--rw-r--r--   0        0        0     3908 2023-06-23 07:45:23.356231 tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc
--rw-r--r--   0        0        0     3898 2023-06-23 05:37:39.292931 tkadw-0.1.3/tkadw/tkite/gtk/button.py
--rw-r--r--   0        0        0     2201 2023-06-23 05:36:23.978561 tkadw-0.1.3/tkadw/tkite/gtk/entry.py
--rw-r--r--   0        0        0     1141 2023-06-23 07:40:36.374539 tkadw-0.1.3/tkadw/tkite/gtk/frame.py
--rw-r--r--   0        0        0      500 2023-06-23 00:56:14.658098 tkadw-0.1.3/tkadw/tkite/gtk/notebook.py
--rw-r--r--   0        0        0     2785 2023-06-23 07:45:23.240982 tkadw-0.1.3/tkadw/tkite/gtk/textbox.py
--rw-r--r--   0        0        0        0 2023-06-09 14:28:28.424277 tkadw-0.1.3/tkadw/ttk/__init__.py
--rw-r--r--   0        0        0      139 2023-06-09 14:38:22.776399 tkadw-0.1.3/tkadw/ttk/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1349 2023-06-09 14:41:39.497543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/__init__.py
--rw-r--r--   0        0        0     2722 2023-06-09 14:43:18.298069 tkadw-0.1.3/tkadw/ttk/atomize_ttk/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2961 2023-06-09 14:41:39.498543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/sun-valley.tcl
--rw-r--r--   0        0        0     5150 2023-05-14 15:25:00.266570 tkadw-0.1.3/tkadw/ttk/atomize_ttk/sv.tcl
--rw-r--r--   0        0        0      270 2023-06-09 14:41:39.500545 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/arrow-down.png
--rw-r--r--   0        0        0      261 2023-06-09 14:41:39.501544 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/arrow-right.png
--rw-r--r--   0        0        0      274 2023-06-09 14:41:39.501544 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/arrow-up.png
--rw-r--r--   0        0        0      262 2023-06-09 14:41:39.502544 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-accent-disabled.png
--rw-r--r--   0        0        0      373 2023-06-09 14:41:39.503545 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-accent-hover.png
--rw-r--r--   0        0        0      363 2023-06-09 14:41:39.503545 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-accent-pressed.png
--rw-r--r--   0        0        0      377 2023-06-09 14:41:39.504545 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-accent-rest.png
--rw-r--r--   0        0        0      274 2023-06-09 14:41:39.505542 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-close-hover.png
--rw-r--r--   0        0        0      274 2023-06-09 14:41:39.505542 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-close-pressed.png
--rw-r--r--   0        0        0      301 2023-06-09 14:41:39.506544 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-disabled.png
--rw-r--r--   0        0        0      276 2023-06-09 14:41:39.506544 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-hover.png
--rw-r--r--   0        0        0      288 2023-06-09 14:41:39.507543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-pressed.png
--rw-r--r--   0        0        0      301 2023-06-09 14:41:39.508543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-rest.png
--rw-r--r--   0        0        0      245 2023-06-09 14:41:39.508543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-titlebar-hover.png
--rw-r--r--   0        0        0      238 2023-06-09 14:41:39.509543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/button-titlebar-pressed.png
--rw-r--r--   0        0        0      386 2023-06-09 14:41:39.509543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/card.png
--rw-r--r--   0        0        0      383 2023-06-09 14:41:39.510542 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-disabled.png
--rw-r--r--   0        0        0      474 2023-06-09 14:41:39.511543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-hover.png
--rw-r--r--   0        0        0      460 2023-06-09 14:41:39.511543 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-pressed.png
--rw-r--r--   0        0        0      475 2023-06-09 14:41:39.512544 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-rest.png
--rw-r--r--   0        0        0      294 2023-06-09 14:41:39.513547 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-tri-disabled.png
--rw-r--r--   0        0        0      362 2023-06-09 14:41:39.514132 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-tri-hover.png
--rw-r--r--   0        0        0      358 2023-06-09 14:41:39.515137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-tri-pressed.png
--rw-r--r--   0        0        0      363 2023-06-09 14:41:39.515137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-tri-rest.png
--rw-r--r--   0        0        0      312 2023-06-09 14:41:39.516139 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-disabled.png
--rw-r--r--   0        0        0      353 2023-06-09 14:41:39.517139 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-hover.png
--rw-r--r--   0        0        0      302 2023-06-09 14:41:39.517139 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-pressed.png
--rw-r--r--   0        0        0      353 2023-06-09 14:41:39.518137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/check-unsel-rest.png
--rw-r--r--   0        0        0      129 2023-06-09 14:41:39.519137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/empty.png
--rw-r--r--   0        0        0      273 2023-06-09 14:41:39.519137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/entry-disabled.png
--rw-r--r--   0        0        0      335 2023-06-09 14:41:39.520136 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/entry-focus.png
--rw-r--r--   0        0        0      269 2023-06-09 14:41:39.521137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/entry-hover.png
--rw-r--r--   0        0        0      324 2023-06-09 14:41:39.522140 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/entry-invalid.png
--rw-r--r--   0        0        0      297 2023-06-09 14:41:39.522140 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/entry-rest.png
--rw-r--r--   0        0        0      337 2023-06-09 14:41:39.523139 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/notebook-border.png
--rw-r--r--   0        0        0      186 2023-06-09 14:41:39.524139 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/notebook.png
--rw-r--r--   0        0        0      193 2023-06-09 14:41:39.524139 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/progress-pbar-hor.png
--rw-r--r--   0        0        0      214 2023-06-09 14:41:39.525137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/progress-pbar-vert.png
--rw-r--r--   0        0        0      157 2023-06-09 14:41:39.526137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/progress-trough-hor.png
--rw-r--r--   0        0        0      160 2023-06-09 14:41:39.526137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/progress-trough-vert.png
--rw-r--r--   0        0        0      553 2023-06-09 14:41:39.527138 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-disabled.png
--rw-r--r--   0        0        0      853 2023-06-09 14:41:39.527138 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-hover.png
--rw-r--r--   0        0        0      786 2023-06-09 14:41:39.528137 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-pressed.png
--rw-r--r--   0        0        0      830 2023-06-09 14:41:39.528640 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-rest.png
--rw-r--r--   0        0        0      552 2023-06-09 14:41:39.529647 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-disabled.png
--rw-r--r--   0        0        0      602 2023-06-09 14:41:39.530644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-hover.png
--rw-r--r--   0        0        0      616 2023-06-09 14:41:39.530644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-pressed.png
--rw-r--r--   0        0        0      621 2023-06-09 14:41:39.531645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/radio-unsel-rest.png
--rw-r--r--   0        0        0      724 2023-06-09 14:41:39.532645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-disabled.png
--rw-r--r--   0        0        0      808 2023-06-09 14:41:39.532645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-hover.png
--rw-r--r--   0        0        0      735 2023-06-09 14:41:39.533645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-pressed.png
--rw-r--r--   0        0        0      771 2023-06-09 14:41:39.533645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-thumb-rest.png
--rw-r--r--   0        0        0      216 2023-06-09 14:41:39.534644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-trough-hor.png
--rw-r--r--   0        0        0      215 2023-06-09 14:41:39.534644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scale-trough-vert.png
--rw-r--r--   0        0        0      226 2023-06-09 14:41:39.535644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-down.png
--rw-r--r--   0        0        0      254 2023-06-09 14:41:39.536643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-hor-thumb.png
--rw-r--r--   0        0        0      338 2023-06-09 14:41:39.537644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-hor-trough.png
--rw-r--r--   0        0        0      233 2023-06-09 14:41:39.538644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-left.png
--rw-r--r--   0        0        0      227 2023-06-09 14:41:39.538644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-right.png
--rw-r--r--   0        0        0      236 2023-06-09 14:41:39.539644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-up.png
--rw-r--r--   0        0        0      264 2023-06-09 14:41:39.539644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-vert-thumb.png
--rw-r--r--   0        0        0      343 2023-06-09 14:41:39.540644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/scroll-vert-trough.png
--rw-r--r--   0        0        0      128 2023-06-09 14:41:39.541644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/separator.png
--rw-r--r--   0        0        0      276 2023-06-09 14:41:39.542647 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/sizegrip.png
--rw-r--r--   0        0        0      733 2023-06-09 14:41:39.542647 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-off-disabled.png
--rw-r--r--   0        0        0      945 2023-06-09 14:41:39.543645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-off-hover.png
--rw-r--r--   0        0        0      963 2023-06-09 14:41:39.544643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-off-pressed.png
--rw-r--r--   0        0        0      895 2023-06-09 14:41:39.545645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-off-rest.png
--rw-r--r--   0        0        0      623 2023-06-09 14:41:39.545645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-on-disabled.png
--rw-r--r--   0        0        0      927 2023-06-09 14:41:39.546644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-on-hover.png
--rw-r--r--   0        0        0      936 2023-06-09 14:41:39.547644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-on-pressed.png
--rw-r--r--   0        0        0      859 2023-06-09 14:41:39.547644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/switch-on-rest.png
--rw-r--r--   0        0        0      265 2023-06-09 14:41:39.548643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/tab-hover.png
--rw-r--r--   0        0        0      164 2023-06-09 14:41:39.549644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/tab-rest.png
--rw-r--r--   0        0        0      319 2023-06-09 14:41:39.549644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/tab-selected.png
--rw-r--r--   0        0        0      295 2023-06-09 14:41:39.550645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/treeheading-hover.png
--rw-r--r--   0        0        0      317 2023-06-09 14:41:39.551644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/treeheading-pressed.png
--rw-r--r--   0        0        0      321 2023-06-09 14:41:39.551644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark/treeheading-rest.png
--rw-r--r--   0        0        0    20188 2023-06-09 14:41:39.499549 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/dark.tcl
--rw-r--r--   0        0        0      278 2023-06-09 14:41:39.552643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/arrow-down.png
--rw-r--r--   0        0        0      273 2023-06-09 14:41:39.552643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/arrow-right.png
--rw-r--r--   0        0        0      285 2023-06-09 14:41:39.553645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/arrow-up.png
--rw-r--r--   0        0        0      271 2023-06-09 14:41:39.554647 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-accent-disabled.png
--rw-r--r--   0        0        0      219 2023-06-09 14:48:51.766400 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-accent-hover.png
--rw-r--r--   0        0        0      255 2023-06-09 14:53:14.082428 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-accent-pressed.png
--rw-r--r--   0        0        0      217 2023-06-09 14:48:47.641380 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-accent-rest.png
--rw-r--r--   0        0        0      326 2023-06-09 14:41:39.556644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-close-hover.png
--rw-r--r--   0        0        0      316 2023-06-09 14:41:39.557644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-close-pressed.png
--rw-r--r--   0        0        0      307 2023-06-09 14:41:39.557644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-disabled.png
--rw-r--r--   0        0        0      306 2023-06-09 14:41:39.558645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-hover.png
--rw-r--r--   0        0        0      289 2023-06-09 14:41:39.559644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-pressed.png
--rw-r--r--   0        0        0      303 2023-06-09 14:41:39.559644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-rest.png
--rw-r--r--   0        0        0      238 2023-06-09 14:41:39.560643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-titlebar-hover.png
--rw-r--r--   0        0        0      225 2023-06-09 14:41:39.561643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/button-titlebar-pressed.png
--rw-r--r--   0        0        0      479 2023-06-09 14:43:10.460434 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/card.png
--rw-r--r--   0        0        0      381 2023-06-09 14:41:39.562646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-disabled.png
--rw-r--r--   0        0        0      476 2023-06-09 14:41:39.562646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-hover.png
--rw-r--r--   0        0        0      467 2023-06-09 14:41:39.563646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-pressed.png
--rw-r--r--   0        0        0      473 2023-06-09 14:41:39.564644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-rest.png
--rw-r--r--   0        0        0      299 2023-06-09 14:41:39.564644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-tri-disabled.png
--rw-r--r--   0        0        0      365 2023-06-09 14:41:39.565643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-tri-hover.png
--rw-r--r--   0        0        0      362 2023-06-09 14:41:39.566644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-tri-pressed.png
--rw-r--r--   0        0        0      367 2023-06-09 14:41:39.566644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-tri-rest.png
--rw-r--r--   0        0        0      324 2023-06-09 14:41:39.567644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-unsel-disabled.png
--rw-r--r--   0        0        0      334 2023-06-09 14:41:39.568643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-unsel-hover.png
--rw-r--r--   0        0        0      302 2023-06-09 14:41:39.568643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-unsel-pressed.png
--rw-r--r--   0        0        0      333 2023-06-09 14:41:39.569646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/check-unsel-rest.png
--rw-r--r--   0        0        0      129 2023-06-09 14:41:39.569646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/empty.png
--rw-r--r--   0        0        0      289 2023-06-09 14:41:39.570644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/entry-disabled.png
--rw-r--r--   0        0        0      331 2023-06-09 14:41:39.571647 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/entry-focus.png
--rw-r--r--   0        0        0      302 2023-06-09 14:41:39.572644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/entry-hover.png
--rw-r--r--   0        0        0      324 2023-06-09 14:41:39.572644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/entry-invalid.png
--rw-r--r--   0        0        0      308 2023-06-09 14:41:39.573646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/entry-rest.png
--rw-r--r--   0        0        0      298 2023-06-09 14:41:39.573646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/notebook-border.png
--rw-r--r--   0        0        0      185 2023-06-09 14:41:39.574643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/notebook.png
--rw-r--r--   0        0        0      192 2023-06-09 14:41:39.575643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/progress-pbar-hor.png
--rw-r--r--   0        0        0      216 2023-06-09 14:41:39.575643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/progress-pbar-vert.png
--rw-r--r--   0        0        0      158 2023-06-09 14:41:39.576643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/progress-trough-hor.png
--rw-r--r--   0        0        0      161 2023-06-09 14:41:39.577644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/progress-trough-vert.png
--rw-r--r--   0        0        0      523 2023-06-09 14:41:39.578645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-disabled.png
--rw-r--r--   0        0        0      837 2023-06-09 14:41:39.578645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-hover.png
--rw-r--r--   0        0        0      764 2023-06-09 14:41:39.579645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-pressed.png
--rw-r--r--   0        0        0      773 2023-06-09 14:41:39.580644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-rest.png
--rw-r--r--   0        0        0      521 2023-06-09 14:41:39.581644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-disabled.png
--rw-r--r--   0        0        0      573 2023-06-09 14:41:39.582644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-hover.png
--rw-r--r--   0        0        0      636 2023-06-09 14:41:39.582644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-pressed.png
--rw-r--r--   0        0        0      576 2023-06-09 14:41:39.583644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/radio-unsel-rest.png
--rw-r--r--   0        0        0      658 2023-06-09 14:41:39.584643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-disabled.png
--rw-r--r--   0        0        0      749 2023-06-09 14:41:39.584643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-hover.png
--rw-r--r--   0        0        0      675 2023-06-09 14:41:39.585645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-pressed.png
--rw-r--r--   0        0        0      701 2023-06-09 14:41:39.586645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-thumb-rest.png
--rw-r--r--   0        0        0      208 2023-06-09 14:41:39.586645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-trough-hor.png
--rw-r--r--   0        0        0      214 2023-06-09 14:41:39.587646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scale-trough-vert.png
--rw-r--r--   0        0        0      229 2023-06-09 14:41:39.588644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-down.png
--rw-r--r--   0        0        0      234 2023-06-09 14:41:39.589644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-hor-thumb.png
--rw-r--r--   0        0        0      321 2023-06-09 14:41:39.589644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-hor-trough.png
--rw-r--r--   0        0        0      232 2023-06-09 14:41:39.590644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-left.png
--rw-r--r--   0        0        0      223 2023-06-09 14:41:39.590644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-right.png
--rw-r--r--   0        0        0      237 2023-06-09 14:41:39.591643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-up.png
--rw-r--r--   0        0        0      262 2023-06-09 14:41:39.592644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-vert-thumb.png
--rw-r--r--   0        0        0      324 2023-06-09 14:41:39.593644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/scroll-vert-trough.png
--rw-r--r--   0        0        0      128 2023-06-09 14:41:39.594646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/separator.png
--rw-r--r--   0        0        0      272 2023-06-09 14:41:39.594646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/sizegrip.png
--rw-r--r--   0        0        0      726 2023-06-09 14:41:39.595643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-off-disabled.png
--rw-r--r--   0        0        0      867 2023-06-09 14:41:39.596647 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-off-hover.png
--rw-r--r--   0        0        0      880 2023-06-09 14:41:39.597645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-off-pressed.png
--rw-r--r--   0        0        0      814 2023-06-09 14:41:39.597645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-off-rest.png
--rw-r--r--   0        0        0      590 2023-06-09 14:41:39.598645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-on-disabled.png
--rw-r--r--   0        0        0      906 2023-06-09 14:41:39.598645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-on-hover.png
--rw-r--r--   0        0        0      916 2023-06-09 14:41:39.599644 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-on-pressed.png
--rw-r--r--   0        0        0      857 2023-06-09 14:41:39.600643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/switch-on-rest.png
--rw-r--r--   0        0        0      295 2023-06-09 14:41:39.600643 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/tab-hover.png
--rw-r--r--   0        0        0      164 2023-06-09 14:41:39.601645 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/tab-rest.png
--rw-r--r--   0        0        0      318 2023-06-09 14:41:39.602649 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/tab-selected.png
--rw-r--r--   0        0        0      338 2023-06-09 14:41:39.602649 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/treeheading-hover.png
--rw-r--r--   0        0        0      318 2023-06-09 14:41:39.603646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/treeheading-pressed.png
--rw-r--r--   0        0        0      330 2023-06-09 14:41:39.603646 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light/treeheading-rest.png
--rw-r--r--   0        0        0    20371 2023-06-09 14:41:39.500545 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/light.tcl
--rw-r--r--   0        0        0     3045 2023-05-14 15:25:00.269895 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/sprites_dark.tcl
--rw-r--r--   0        0        0     3092 2023-05-14 15:25:00.270897 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/sprites_light.tcl
--rw-r--r--   0        0        0    18371 2023-05-14 15:25:00.272896 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/spritesheet_dark.png
--rw-r--r--   0        0        0     2649 2023-06-09 14:36:51.668892 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/spritesheet_light.png
--rw-r--r--   0        0        0    18462 2023-05-14 15:25:00.272896 tkadw-0.1.3/tkadw/ttk/atomize_ttk/theme/spritesheet_light2.png
--rw-r--r--   0        0        0      372 2023-06-09 14:40:30.166428 tkadw-0.1.3/tkadw/ttk/test.py
--rw-r--r--   0        0        0      629 1970-01-01 00:00:00.000000 tkadw-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      272 2023-06-23 09:08:46.990419 tkadw-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3059 2023-06-23 09:04:32.302087 tkadw-0.1.5/README.md
+-rw-r--r--   0        0        0      112 2023-06-23 03:45:25.577456 tkadw-0.1.5/tkadw/__init__.py
+-rw-r--r--   0        0        0      948 2023-06-23 07:49:26.692233 tkadw-0.1.5/tkadw/__main__.py
+-rw-r--r--   0        0        0       74 2023-06-09 11:52:45.827295 tkadw-0.1.5/tkadw/app.config
+-rw-r--r--   0        0        0      940 2023-06-09 11:52:45.801259 tkadw-0.1.5/tkadw/appconfig.py
+-rw-r--r--   0        0        0      896 2023-06-23 07:36:10.506439 tkadw-0.1.5/tkadw/canvas/__init__.py
+-rw-r--r--   0        0        0     1701 2023-06-23 07:38:42.890718 tkadw-0.1.5/tkadw/canvas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      124 2023-04-15 23:20:17.035856 tkadw-0.1.5/tkadw/canvas/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0    22885 2023-06-23 04:54:52.588047 tkadw-0.1.5/tkadw/canvas/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     3479 2023-04-15 23:20:17.037902 tkadw-0.1.5/tkadw/canvas/__pycache__/button.cpython-38.pyc
+-rw-r--r--   0        0        0    23239 2023-06-23 05:05:08.679421 tkadw-0.1.5/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc
+-rw-r--r--   0        0        0    25982 2023-06-23 07:48:50.831965 tkadw-0.1.5/tkadw/canvas/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0    13288 2023-06-23 07:38:42.954769 tkadw-0.1.5/tkadw/canvas/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0    15536 2023-06-10 07:35:47.433931 tkadw-0.1.5/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0    29855 2023-06-23 09:08:58.842594 tkadw-0.1.5/tkadw/canvas/__pycache__/textbox.cpython-311.pyc
+-rw-r--r--   0        0        0        0 2023-06-10 10:53:44.353940 tkadw-0.1.5/tkadw/canvas/adwite/__init__.py
+-rw-r--r--   0        0        0     1363 2023-06-10 11:23:03.996035 tkadw-0.1.5/tkadw/canvas/adwite/button.py
+-rw-r--r--   0        0        0       80 2023-06-09 13:54:04.880107 tkadw-0.1.5/tkadw/canvas/atomize/__init__.py
+-rw-r--r--   0        0        0     2520 2023-06-10 04:30:03.863844 tkadw-0.1.5/tkadw/canvas/atomize/button.py
+-rw-r--r--   0        0        0    17270 2023-06-23 04:54:52.447686 tkadw-0.1.5/tkadw/canvas/button.py
+-rw-r--r--   0        0        0    20382 2023-06-23 05:05:08.591410 tkadw-0.1.5/tkadw/canvas/drawengine.py
+-rw-r--r--   0        0        0    22377 2023-06-23 07:48:50.714445 tkadw-0.1.5/tkadw/canvas/entry.py
+-rw-r--r--   0        0        0      513 2023-06-09 23:26:21.009369 tkadw-0.1.5/tkadw/canvas/fluent/__init__.py
+-rw-r--r--   0        0        0     8629 2023-06-23 05:15:43.010231 tkadw-0.1.5/tkadw/canvas/frame.py
+-rw-r--r--   0        0        0     2051 2023-06-10 01:20:40.907297 tkadw-0.1.5/tkadw/canvas/fun.py
+-rw-r--r--   0        0        0    15490 2023-06-10 01:25:11.532315 tkadw-0.1.5/tkadw/canvas/fun2.py
+-rw-r--r--   0        0        0     8108 2023-06-10 01:29:02.970946 tkadw-0.1.5/tkadw/canvas/fun3.py
+-rw-r--r--   0        0        0     3202 2023-06-10 03:27:44.231516 tkadw-0.1.5/tkadw/canvas/fun4.py
+-rw-r--r--   0        0        0      942 2023-06-10 03:50:17.322506 tkadw-0.1.5/tkadw/canvas/fun5.py
+-rw-r--r--   0        0        0     9870 2023-06-10 07:36:40.103845 tkadw-0.1.5/tkadw/canvas/fun6.py
+-rw-r--r--   0        0        0     5690 2023-06-10 03:45:21.292347 tkadw-0.1.5/tkadw/canvas/poly.tcl
+-rw-r--r--   0        0        0    23435 2023-06-23 09:08:40.755238 tkadw-0.1.5/tkadw/canvas/textbox.py
+-rw-r--r--   0        0        0     4597 2023-05-27 23:04:22.860566 tkadw-0.1.5/tkadw/canvas/titlebar.py
+-rw-r--r--   0        0        0       29 2023-06-23 03:52:51.957932 tkadw-0.1.5/tkadw/tkite/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-23 03:52:52.129145 tkadw-0.1.5/tkadw/tkite/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      283 2023-06-23 07:44:06.875178 tkadw-0.1.5/tkadw/tkite/gtk/__init__.py
+-rw-r--r--   0        0        0      620 2023-06-23 07:44:06.983012 tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4518 2023-06-23 08:34:35.190496 tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc
+-rw-r--r--   0        0        0     3287 2023-06-23 08:39:30.900894 tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc
+-rw-r--r--   0        0        0     2457 2023-06-23 07:42:27.405172 tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc
+-rw-r--r--   0        0        0     3908 2023-06-23 07:45:23.356231 tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc
+-rw-r--r--   0        0        0     3726 2023-06-23 08:34:35.056325 tkadw-0.1.5/tkadw/tkite/gtk/button.py
+-rw-r--r--   0        0        0     2441 2023-06-23 08:39:30.782792 tkadw-0.1.5/tkadw/tkite/gtk/entry.py
+-rw-r--r--   0        0        0     1141 2023-06-23 07:40:36.374539 tkadw-0.1.5/tkadw/tkite/gtk/frame.py
+-rw-r--r--   0        0        0      500 2023-06-23 00:56:14.658098 tkadw-0.1.5/tkadw/tkite/gtk/notebook.py
+-rw-r--r--   0        0        0     2785 2023-06-23 07:45:23.240982 tkadw-0.1.5/tkadw/tkite/gtk/textbox.py
+-rw-r--r--   0        0        0     3491 1970-01-01 00:00:00.000000 tkadw-0.1.5/PKG-INFO
```

### Comparing `tkadw-0.1.3/tkadw/__main__.py` & `tkadw-0.1.5/tkadw/__main__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/appconfig.py` & `tkadw-0.1.5/tkadw/appconfig.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/__init__.py` & `tkadw-0.1.5/tkadw/canvas/__init__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.1.5/tkadw/canvas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/__pycache__/button.cpython-311.pyc` & `tkadw-0.1.5/tkadw/canvas/__pycache__/button.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/__pycache__/button.cpython-38.pyc` & `tkadw-0.1.5/tkadw/canvas/__pycache__/button.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc` & `tkadw-0.1.5/tkadw/canvas/__pycache__/drawengine.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/__pycache__/entry.cpython-311.pyc` & `tkadw-0.1.5/tkadw/canvas/__pycache__/entry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/__pycache__/frame.cpython-311.pyc` & `tkadw-0.1.5/tkadw/canvas/__pycache__/frame.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc` & `tkadw-0.1.5/tkadw/canvas/__pycache__/fun6.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/__pycache__/textbox.cpython-311.pyc` & `tkadw-0.1.5/tkadw/canvas/__pycache__/textbox.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x774f9564 (Fri Jun 23 07:53:27 2023 UTC)
-files sz: 22443
+moddate:  0x18619564 (Fri Jun 23 09:08:40 2023 UTC)
+files sz: 23435
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
       0x9700640064016c006d015a016d025a020100640064026c036d045a0401
@@ -58,233 +58,235 @@
                 36 MAKE_FUNCTION            0
                 38 LOAD_CONST               4 ('AdwDrawBasicText')
                 40 LOAD_NAME                4 (AdwDrawEngine)
                 42 PRECALL                  3
                 46 CALL                     3
                 56 STORE_NAME               5 (AdwDrawBasicText)
    
-   221          58 PUSH_NULL
+   254          58 PUSH_NULL
                 60 LOAD_BUILD_CLASS
-                62 LOAD_CONST               5 (<code object AdwDrawText, file "D:\tkadw\tkadw\canvas\textbox.py", line 221>)
+                62 LOAD_CONST               5 (<code object AdwDrawText, file "D:\tkadw\tkadw\canvas\textbox.py", line 254>)
                 64 MAKE_FUNCTION            0
                 66 LOAD_CONST               6 ('AdwDrawText')
                 68 LOAD_NAME                5 (AdwDrawBasicText)
                 70 PRECALL                  3
                 74 CALL                     3
                 84 STORE_NAME               6 (AdwDrawText)
    
-   226          86 PUSH_NULL
+   259          86 PUSH_NULL
                 88 LOAD_BUILD_CLASS
-                90 LOAD_CONST               7 (<code object AdwDrawDarkText, file "D:\tkadw\tkadw\canvas\textbox.py", line 226>)
+                90 LOAD_CONST               7 (<code object AdwDrawDarkText, file "D:\tkadw\tkadw\canvas\textbox.py", line 259>)
                 92 MAKE_FUNCTION            0
                 94 LOAD_CONST               8 ('AdwDrawDarkText')
                 96 LOAD_NAME                5 (AdwDrawBasicText)
                 98 PRECALL                  3
                102 CALL                     3
                112 STORE_NAME               7 (AdwDrawDarkText)
    
-   232         114 PUSH_NULL
+   265         114 PUSH_NULL
                116 LOAD_BUILD_CLASS
-               118 LOAD_CONST               9 (<code object AdwDrawBasicRoundText, file "D:\tkadw\tkadw\canvas\textbox.py", line 232>)
+               118 LOAD_CONST               9 (<code object AdwDrawBasicRoundText, file "D:\tkadw\tkadw\canvas\textbox.py", line 265>)
                120 MAKE_FUNCTION            0
                122 LOAD_CONST              10 ('AdwDrawBasicRoundText')
                124 LOAD_NAME                5 (AdwDrawBasicText)
                126 PRECALL                  3
                130 CALL                     3
                140 STORE_NAME               8 (AdwDrawBasicRoundText)
    
-   410         142 PUSH_NULL
+   443         142 PUSH_NULL
                144 LOAD_BUILD_CLASS
-               146 LOAD_CONST              11 (<code object AdwDrawRoundText, file "D:\tkadw\tkadw\canvas\textbox.py", line 410>)
+               146 LOAD_CONST              11 (<code object AdwDrawRoundText, file "D:\tkadw\tkadw\canvas\textbox.py", line 443>)
                148 MAKE_FUNCTION            0
                150 LOAD_CONST              12 ('AdwDrawRoundText')
                152 LOAD_NAME                8 (AdwDrawBasicRoundText)
                154 PRECALL                  3
                158 CALL                     3
                168 STORE_NAME               9 (AdwDrawRoundText)
    
-   415         170 PUSH_NULL
+   448         170 PUSH_NULL
                172 LOAD_BUILD_CLASS
-               174 LOAD_CONST              13 (<code object AdwDrawRoundDarkText, file "D:\tkadw\tkadw\canvas\textbox.py", line 415>)
+               174 LOAD_CONST              13 (<code object AdwDrawRoundDarkText, file "D:\tkadw\tkadw\canvas\textbox.py", line 448>)
                176 MAKE_FUNCTION            0
                178 LOAD_CONST              14 ('AdwDrawRoundDarkText')
                180 LOAD_NAME                8 (AdwDrawBasicRoundText)
                182 PRECALL                  3
                186 CALL                     3
                196 STORE_NAME              10 (AdwDrawRoundDarkText)
    
-   420         198 PUSH_NULL
+   453         198 PUSH_NULL
                200 LOAD_BUILD_CLASS
-               202 LOAD_CONST              15 (<code object AdwDrawBasicRoundText3, file "D:\tkadw\tkadw\canvas\textbox.py", line 420>)
+               202 LOAD_CONST              15 (<code object AdwDrawBasicRoundText3, file "D:\tkadw\tkadw\canvas\textbox.py", line 453>)
                204 MAKE_FUNCTION            0
                206 LOAD_CONST              16 ('AdwDrawBasicRoundText3')
                208 LOAD_NAME                5 (AdwDrawBasicText)
                210 PRECALL                  3
                214 CALL                     3
                224 STORE_NAME              11 (AdwDrawBasicRoundText3)
    
-   604         226 PUSH_NULL
+   637         226 PUSH_NULL
                228 LOAD_BUILD_CLASS
-               230 LOAD_CONST              17 (<code object AdwDrawRoundText3, file "D:\tkadw\tkadw\canvas\textbox.py", line 604>)
+               230 LOAD_CONST              17 (<code object AdwDrawRoundText3, file "D:\tkadw\tkadw\canvas\textbox.py", line 637>)
                232 MAKE_FUNCTION            0
                234 LOAD_CONST              18 ('AdwDrawRoundText3')
                236 LOAD_NAME               11 (AdwDrawBasicRoundText3)
                238 PRECALL                  3
                242 CALL                     3
                252 STORE_NAME              12 (AdwDrawRoundText3)
    
-   609         254 PUSH_NULL
+   642         254 PUSH_NULL
                256 LOAD_BUILD_CLASS
-               258 LOAD_CONST              19 (<code object AdwDrawRoundDarkText3, file "D:\tkadw\tkadw\canvas\textbox.py", line 609>)
+               258 LOAD_CONST              19 (<code object AdwDrawRoundDarkText3, file "D:\tkadw\tkadw\canvas\textbox.py", line 642>)
                260 MAKE_FUNCTION            0
                262 LOAD_CONST              20 ('AdwDrawRoundDarkText3')
                264 LOAD_NAME               11 (AdwDrawBasicRoundText3)
                266 PRECALL                  3
                270 CALL                     3
                280 STORE_NAME              13 (AdwDrawRoundDarkText3)
    
-   614         282 LOAD_NAME               14 (__name__)
+   647         282 LOAD_NAME               14 (__name__)
                284 LOAD_CONST              21 ('__main__')
                286 COMPARE_OP               2 (==)
                292 POP_JUMP_FORWARD_IF_FALSE   242 (to 778)
    
-   615         294 LOAD_CONST               0 (0)
+   648         294 LOAD_CONST               0 (0)
                296 LOAD_CONST              22 (('Tk',))
                298 IMPORT_NAME             15 (tkinter)
                300 IMPORT_FROM             16 (Tk)
                302 STORE_NAME              16 (Tk)
                304 POP_TOP
    
-   617         306 PUSH_NULL
+   650         306 PUSH_NULL
                308 LOAD_NAME               16 (Tk)
                310 PRECALL                  0
                314 CALL                     0
                324 STORE_NAME              17 (root)
    
-   619         326 PUSH_NULL
+   652         326 PUSH_NULL
                328 LOAD_NAME                6 (AdwDrawText)
                330 PRECALL                  0
                334 CALL                     0
                344 STORE_NAME              18 (text1)
    
-   620         346 LOAD_NAME               18 (text1)
+   653         346 LOAD_NAME               18 (text1)
                348 LOAD_METHOD             19 (pack)
                370 LOAD_CONST              23 ('x')
                372 LOAD_CONST              24 (5)
                374 LOAD_CONST              24 (5)
                376 KW_NAMES                25
                378 PRECALL                  3
                382 CALL                     3
                392 POP_TOP
    
-   622         394 PUSH_NULL
+   655         394 PUSH_NULL
                396 LOAD_NAME                7 (AdwDrawDarkText)
                398 PRECALL                  0
                402 CALL                     0
                412 STORE_NAME              20 (text2)
    
-   623         414 LOAD_NAME               20 (text2)
+   656         414 LOAD_NAME               20 (text2)
                416 LOAD_METHOD             19 (pack)
                438 LOAD_CONST              23 ('x')
                440 LOAD_CONST              24 (5)
                442 LOAD_CONST              24 (5)
                444 KW_NAMES                25
                446 PRECALL                  3
                450 CALL                     3
                460 POP_TOP
    
-   625         462 PUSH_NULL
+   658         462 PUSH_NULL
                464 LOAD_NAME                9 (AdwDrawRoundText)
                466 PRECALL                  0
                470 CALL                     0
                480 STORE_NAME              21 (text3)
    
-   626         482 LOAD_NAME               21 (text3)
+   659         482 LOAD_NAME               21 (text3)
                484 LOAD_METHOD             19 (pack)
                506 LOAD_CONST              23 ('x')
                508 LOAD_CONST              24 (5)
                510 LOAD_CONST              24 (5)
                512 KW_NAMES                25
                514 PRECALL                  3
                518 CALL                     3
                528 POP_TOP
    
-   628         530 PUSH_NULL
+   661         530 PUSH_NULL
                532 LOAD_NAME               10 (AdwDrawRoundDarkText)
                534 PRECALL                  0
                538 CALL                     0
                548 STORE_NAME              22 (text4)
    
-   629         550 LOAD_NAME               22 (text4)
+   662         550 LOAD_NAME               22 (text4)
                552 LOAD_METHOD             19 (pack)
                574 LOAD_CONST              23 ('x')
                576 LOAD_CONST              24 (5)
                578 LOAD_CONST              24 (5)
                580 KW_NAMES                25
                582 PRECALL                  3
                586 CALL                     3
                596 POP_TOP
    
-   631         598 PUSH_NULL
+   664         598 PUSH_NULL
                600 LOAD_NAME               12 (AdwDrawRoundText3)
                602 PRECALL                  0
                606 CALL                     0
                616 STORE_NAME              23 (text5)
    
-   632         618 LOAD_NAME               23 (text5)
+   665         618 LOAD_NAME               23 (text5)
                620 LOAD_METHOD             19 (pack)
                642 LOAD_CONST              23 ('x')
                644 LOAD_CONST              24 (5)
                646 LOAD_CONST              24 (5)
                648 KW_NAMES                25
                650 PRECALL                  3
                654 CALL                     3
                664 POP_TOP
    
-   634         666 PUSH_NULL
+   667         666 PUSH_NULL
                668 LOAD_NAME               13 (AdwDrawRoundDarkText3)
                670 PRECALL                  0
                674 CALL                     0
                684 STORE_NAME              24 (text6)
    
-   635         686 LOAD_NAME               24 (text6)
+   668         686 LOAD_NAME               24 (text6)
                688 LOAD_METHOD             19 (pack)
                710 LOAD_CONST              23 ('x')
                712 LOAD_CONST              24 (5)
                714 LOAD_CONST              24 (5)
                716 KW_NAMES                25
                718 PRECALL                  3
                722 CALL                     3
                732 POP_TOP
    
-   637         734 LOAD_NAME               17 (root)
+   670         734 LOAD_NAME               17 (root)
                736 LOAD_METHOD             25 (mainloop)
                758 PRECALL                  0
                762 CALL                     0
                772 POP_TOP
                774 LOAD_CONST              26 (None)
                776 RETURN_VALUE
    
-   614     >>  778 LOAD_CONST              26 (None)
+   647     >>  778 LOAD_CONST              26 (None)
                780 RETURN_VALUE
    consts
       0
       ('Font', 'nametofont')
       ('AdwDrawEngine',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x8700970065005a0164005a026401640264039c02880066016404840a5a
-            03640584005a04640684005a05640784005a06640884005a076415640a84
-            015a086415640b84015a096415640c84015a0a6415640d84015a0b641564
-            0e84015a0c6415640f650d6602641084055a0e641184005a0f641284005a
-            10641384005a116415641484015a12880078015a135300
+            03640584005a04640684005a05640784005a06640884005a07640984005a
+            08640a84005a09640b84005a0a640c84005a0b640d84005a0c640e84005a
+            0d640f84005a0e641084005a0f641184005a10641284005a11641384005a
+            126420641584015a136420641684015a146420641784015a156420641884
+            015a166420641984015a176420641a65186602641b84055a19641c84005a
+            1a641d84005a1b641e84005a1c6420641f84015a1d880078015a1e5300
                        0 MAKE_CELL                0 (__class__)
          
            6           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicText')
                       10 STORE_NAME               2 (__qualname__)
@@ -295,83 +297,127 @@
                       18 BUILD_CONST_KEY_MAP      2
                       20 LOAD_CLOSURE             0 (__class__)
                       22 BUILD_TUPLE              1
                       24 LOAD_CONST               4 (<code object __init__, file "D:\tkadw\tkadw\canvas\textbox.py", line 7>)
                       26 MAKE_FUNCTION           10 (kwdefaults, closure)
                       28 STORE_NAME               3 (__init__)
          
-          48          30 LOAD_CONST               5 (<code object undo, file "D:\tkadw\tkadw\canvas\textbox.py", line 48>)
+          48          30 LOAD_CONST               5 (<code object tbbox, file "D:\tkadw\tkadw\canvas\textbox.py", line 48>)
                       32 MAKE_FUNCTION            0
-                      34 STORE_NAME               4 (undo)
+                      34 STORE_NAME               4 (tbbox)
          
-          54          36 LOAD_CONST               6 (<code object redo, file "D:\tkadw\tkadw\canvas\textbox.py", line 54>)
+          51          36 LOAD_CONST               6 (<code object compare, file "D:\tkadw\tkadw\canvas\textbox.py", line 51>)
                       38 MAKE_FUNCTION            0
-                      40 STORE_NAME               5 (redo)
+                      40 STORE_NAME               5 (compare)
          
-          60          42 LOAD_CONST               7 (<code object _other, file "D:\tkadw\tkadw\canvas\textbox.py", line 60>)
+          54          42 LOAD_CONST               7 (<code object count, file "D:\tkadw\tkadw\canvas\textbox.py", line 54>)
                       44 MAKE_FUNCTION            0
-                      46 STORE_NAME               6 (_other)
+                      46 STORE_NAME               6 (count)
          
-          64          48 LOAD_CONST               8 (<code object _draw, file "D:\tkadw\tkadw\canvas\textbox.py", line 64>)
+          57          48 LOAD_CONST               8 (<code object debug, file "D:\tkadw\tkadw\canvas\textbox.py", line 57>)
                       50 MAKE_FUNCTION            0
-                      52 STORE_NAME               7 (_draw)
+                      52 STORE_NAME               7 (debug)
          
-          92          54 LOAD_CONST              21 ((None,))
-                      56 LOAD_CONST              10 (<code object _focus, file "D:\tkadw\tkadw\canvas\textbox.py", line 92>)
-                      58 MAKE_FUNCTION            1 (defaults)
-                      60 STORE_NAME               8 (_focus)
+          60          54 LOAD_CONST               9 (<code object tdelete, file "D:\tkadw\tkadw\canvas\textbox.py", line 60>)
+                      56 MAKE_FUNCTION            0
+                      58 STORE_NAME               8 (tdelete)
          
-         101          62 LOAD_CONST              21 ((None,))
-                      64 LOAD_CONST              11 (<code object _focusout, file "D:\tkadw\tkadw\canvas\textbox.py", line 101>)
-                      66 MAKE_FUNCTION            1 (defaults)
-                      68 STORE_NAME               9 (_focusout)
+          63          60 LOAD_CONST              10 (<code object dump, file "D:\tkadw\tkadw\canvas\textbox.py", line 63>)
+                      62 MAKE_FUNCTION            0
+                      64 STORE_NAME               9 (dump)
          
-         110          70 LOAD_CONST              21 ((None,))
-                      72 LOAD_CONST              12 (<code object _click, file "D:\tkadw\tkadw\canvas\textbox.py", line 110>)
-                      74 MAKE_FUNCTION            1 (defaults)
-                      76 STORE_NAME              10 (_click)
+          66          66 LOAD_CONST              11 (<code object get, file "D:\tkadw\tkadw\canvas\textbox.py", line 66>)
+                      68 MAKE_FUNCTION            0
+                      70 STORE_NAME              10 (get)
          
-         113          78 LOAD_CONST              21 ((None,))
-                      80 LOAD_CONST              13 (<code object _hover, file "D:\tkadw\tkadw\canvas\textbox.py", line 113>)
-                      82 MAKE_FUNCTION            1 (defaults)
-                      84 STORE_NAME              11 (_hover)
+          69          72 LOAD_CONST              12 (<code object tindex, file "D:\tkadw\tkadw\canvas\textbox.py", line 69>)
+                      74 MAKE_FUNCTION            0
+                      76 STORE_NAME              11 (tindex)
          
-         116          86 LOAD_CONST              21 ((None,))
-                      88 LOAD_CONST              14 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\textbox.py", line 116>)
-                      90 MAKE_FUNCTION            1 (defaults)
-                      92 STORE_NAME              12 (_hover_release)
+          72          78 LOAD_CONST              13 (<code object tinsert, file "D:\tkadw\tkadw\canvas\textbox.py", line 72>)
+                      80 MAKE_FUNCTION            0
+                      82 STORE_NAME              12 (tinsert)
          
-         127          94 LOAD_CONST              21 ((None,))
-                      96 LOAD_CONST              15 ('font')
-                      98 LOAD_NAME               13 (Font)
-                     100 BUILD_TUPLE              2
-                     102 LOAD_CONST              16 (<code object font, file "D:\tkadw\tkadw\canvas\textbox.py", line 127>)
-                     104 MAKE_FUNCTION            5 (defaults, annotations)
-                     106 STORE_NAME              14 (font)
+          75          84 LOAD_CONST              14 (<code object search, file "D:\tkadw\tkadw\canvas\textbox.py", line 75>)
+                      86 MAKE_FUNCTION            0
+                      88 STORE_NAME              13 (search)
          
-         133         108 LOAD_CONST              17 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 133>)
+          78          90 LOAD_CONST              15 (<code object see, file "D:\tkadw\tkadw\canvas\textbox.py", line 78>)
+                      92 MAKE_FUNCTION            0
+                      94 STORE_NAME              14 (see)
+         
+          81          96 LOAD_CONST              16 (<code object undo, file "D:\tkadw\tkadw\canvas\textbox.py", line 81>)
+                      98 MAKE_FUNCTION            0
+                     100 STORE_NAME              15 (undo)
+         
+          87         102 LOAD_CONST              17 (<code object redo, file "D:\tkadw\tkadw\canvas\textbox.py", line 87>)
+                     104 MAKE_FUNCTION            0
+                     106 STORE_NAME              16 (redo)
+         
+          93         108 LOAD_CONST              18 (<code object _other, file "D:\tkadw\tkadw\canvas\textbox.py", line 93>)
                      110 MAKE_FUNCTION            0
-                     112 STORE_NAME              15 (default_palette)
+                     112 STORE_NAME              17 (_other)
          
-         136         114 LOAD_CONST              18 (<code object palette_light, file "D:\tkadw\tkadw\canvas\textbox.py", line 136>)
+          97         114 LOAD_CONST              19 (<code object _draw, file "D:\tkadw\tkadw\canvas\textbox.py", line 97>)
                      116 MAKE_FUNCTION            0
-                     118 STORE_NAME              16 (palette_light)
+                     118 STORE_NAME              18 (_draw)
          
-         158         120 LOAD_CONST              19 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\textbox.py", line 158>)
-                     122 MAKE_FUNCTION            0
-                     124 STORE_NAME              17 (palette_dark)
-         
-         180         126 LOAD_CONST              21 ((None,))
-                     128 LOAD_CONST              20 (<code object palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 180>)
-                     130 MAKE_FUNCTION            1 (defaults)
-                     132 STORE_NAME              18 (palette)
-                     134 LOAD_CLOSURE             0 (__class__)
-                     136 COPY                     1
-                     138 STORE_NAME              19 (__classcell__)
-                     140 RETURN_VALUE
+         125         120 LOAD_CONST              32 ((None,))
+                     122 LOAD_CONST              21 (<code object _focus, file "D:\tkadw\tkadw\canvas\textbox.py", line 125>)
+                     124 MAKE_FUNCTION            1 (defaults)
+                     126 STORE_NAME              19 (_focus)
+         
+         134         128 LOAD_CONST              32 ((None,))
+                     130 LOAD_CONST              22 (<code object _focusout, file "D:\tkadw\tkadw\canvas\textbox.py", line 134>)
+                     132 MAKE_FUNCTION            1 (defaults)
+                     134 STORE_NAME              20 (_focusout)
+         
+         143         136 LOAD_CONST              32 ((None,))
+                     138 LOAD_CONST              23 (<code object _click, file "D:\tkadw\tkadw\canvas\textbox.py", line 143>)
+                     140 MAKE_FUNCTION            1 (defaults)
+                     142 STORE_NAME              21 (_click)
+         
+         146         144 LOAD_CONST              32 ((None,))
+                     146 LOAD_CONST              24 (<code object _hover, file "D:\tkadw\tkadw\canvas\textbox.py", line 146>)
+                     148 MAKE_FUNCTION            1 (defaults)
+                     150 STORE_NAME              22 (_hover)
+         
+         149         152 LOAD_CONST              32 ((None,))
+                     154 LOAD_CONST              25 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\textbox.py", line 149>)
+                     156 MAKE_FUNCTION            1 (defaults)
+                     158 STORE_NAME              23 (_hover_release)
+         
+         160         160 LOAD_CONST              32 ((None,))
+                     162 LOAD_CONST              26 ('font')
+                     164 LOAD_NAME               24 (Font)
+                     166 BUILD_TUPLE              2
+                     168 LOAD_CONST              27 (<code object font, file "D:\tkadw\tkadw\canvas\textbox.py", line 160>)
+                     170 MAKE_FUNCTION            5 (defaults, annotations)
+                     172 STORE_NAME              25 (font)
+         
+         166         174 LOAD_CONST              28 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 166>)
+                     176 MAKE_FUNCTION            0
+                     178 STORE_NAME              26 (default_palette)
+         
+         169         180 LOAD_CONST              29 (<code object palette_light, file "D:\tkadw\tkadw\canvas\textbox.py", line 169>)
+                     182 MAKE_FUNCTION            0
+                     184 STORE_NAME              27 (palette_light)
+         
+         191         186 LOAD_CONST              30 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\textbox.py", line 191>)
+                     188 MAKE_FUNCTION            0
+                     190 STORE_NAME              28 (palette_dark)
+         
+         213         192 LOAD_CONST              32 ((None,))
+                     194 LOAD_CONST              31 (<code object palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 213>)
+                     196 MAKE_FUNCTION            1 (defaults)
+                     198 STORE_NAME              29 (palette)
+                     200 LOAD_CLOSURE             0 (__class__)
+                     202 COPY                     1
+                     204 STORE_NAME              30 (__classcell__)
+                     206 RETURN_VALUE
          consts
             'AdwDrawBasicText'
             120
             80
             ('width', 'height')
             code
                argcount  : 1
@@ -953,38 +999,368 @@
                name       '__init__'
                firstlineno 7
                lnotab
                   0x06023a020c022802340228022802180118011801180118023a013a013a
                   013a013a0144013a01440236013601360136024001400140014002
             code
                argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 15
+               code
+                  0x970002007c006a0000000000000000006a0100000000000000007c0169
+                  007c02a4018e015300
+                48           0 RESUME                   0
+               
+                49           2 PUSH_NULL
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (text)
+                            16 LOAD_ATTR                1 (bbox)
+                            26 LOAD_FAST                1 (args)
+                            28 BUILD_MAP                0
+                            30 LOAD_FAST                2 (kwargs)
+                            32 DICT_MERGE               1
+                            34 CALL_FUNCTION_EX         1
+                            36 RETURN_VALUE
+               consts
+                  None
+               names      ('text', 'bbox')
+               varnames   ('self', 'args', 'kwargs')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
+               name       'tbbox'
+               firstlineno 48
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 15
+               code
+                  0x970002007c006a0000000000000000006a0100000000000000007c0169
+                  007c02a4018e015300
+                51           0 RESUME                   0
+               
+                52           2 PUSH_NULL
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (text)
+                            16 LOAD_ATTR                1 (compare)
+                            26 LOAD_FAST                1 (args)
+                            28 BUILD_MAP                0
+                            30 LOAD_FAST                2 (kwargs)
+                            32 DICT_MERGE               1
+                            34 CALL_FUNCTION_EX         1
+                            36 RETURN_VALUE
+               consts
+                  None
+               names      ('text', 'compare')
+               varnames   ('self', 'args', 'kwargs')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
+               name       'compare'
+               firstlineno 51
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 15
+               code
+                  0x970002007c006a0000000000000000006a0100000000000000007c0169
+                  007c02a4018e015300
+                54           0 RESUME                   0
+               
+                55           2 PUSH_NULL
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (text)
+                            16 LOAD_ATTR                1 (count)
+                            26 LOAD_FAST                1 (args)
+                            28 BUILD_MAP                0
+                            30 LOAD_FAST                2 (kwargs)
+                            32 DICT_MERGE               1
+                            34 CALL_FUNCTION_EX         1
+                            36 RETURN_VALUE
+               consts
+                  None
+               names      ('text', 'count')
+               varnames   ('self', 'args', 'kwargs')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
+               name       'count'
+               firstlineno 54
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 15
+               code
+                  0x970002007c006a0000000000000000006a0100000000000000007c0169
+                  007c02a4018e015300
+                57           0 RESUME                   0
+               
+                58           2 PUSH_NULL
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (text)
+                            16 LOAD_ATTR                1 (debug)
+                            26 LOAD_FAST                1 (args)
+                            28 BUILD_MAP                0
+                            30 LOAD_FAST                2 (kwargs)
+                            32 DICT_MERGE               1
+                            34 CALL_FUNCTION_EX         1
+                            36 RETURN_VALUE
+               consts
+                  None
+               names      ('text', 'debug')
+               varnames   ('self', 'args', 'kwargs')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
+               name       'debug'
+               firstlineno 57
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 15
+               code
+                  0x970002007c006a0000000000000000006a0100000000000000007c0169
+                  007c02a4018e015300
+                60           0 RESUME                   0
+               
+                61           2 PUSH_NULL
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (text)
+                            16 LOAD_ATTR                1 (delete)
+                            26 LOAD_FAST                1 (args)
+                            28 BUILD_MAP                0
+                            30 LOAD_FAST                2 (kwargs)
+                            32 DICT_MERGE               1
+                            34 CALL_FUNCTION_EX         1
+                            36 RETURN_VALUE
+               consts
+                  None
+               names      ('text', 'delete')
+               varnames   ('self', 'args', 'kwargs')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
+               name       'tdelete'
+               firstlineno 60
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 15
+               code
+                  0x970002007c006a0000000000000000006a0100000000000000007c0169
+                  007c02a4018e015300
+                63           0 RESUME                   0
+               
+                64           2 PUSH_NULL
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (text)
+                            16 LOAD_ATTR                1 (dump)
+                            26 LOAD_FAST                1 (args)
+                            28 BUILD_MAP                0
+                            30 LOAD_FAST                2 (kwargs)
+                            32 DICT_MERGE               1
+                            34 CALL_FUNCTION_EX         1
+                            36 RETURN_VALUE
+               consts
+                  None
+               names      ('text', 'dump')
+               varnames   ('self', 'args', 'kwargs')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
+               name       'dump'
+               firstlineno 63
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 15
+               code
+                  0x970002007c006a0000000000000000006a0100000000000000007c0169
+                  007c02a4018e015300
+                66           0 RESUME                   0
+               
+                67           2 PUSH_NULL
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (text)
+                            16 LOAD_ATTR                1 (get)
+                            26 LOAD_FAST                1 (args)
+                            28 BUILD_MAP                0
+                            30 LOAD_FAST                2 (kwargs)
+                            32 DICT_MERGE               1
+                            34 CALL_FUNCTION_EX         1
+                            36 RETURN_VALUE
+               consts
+                  None
+               names      ('text', 'get')
+               varnames   ('self', 'args', 'kwargs')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
+               name       'get'
+               firstlineno 66
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 15
+               code
+                  0x970002007c006a0000000000000000006a0100000000000000007c0169
+                  007c02a4018e015300
+                69           0 RESUME                   0
+               
+                70           2 PUSH_NULL
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (text)
+                            16 LOAD_ATTR                1 (index)
+                            26 LOAD_FAST                1 (args)
+                            28 BUILD_MAP                0
+                            30 LOAD_FAST                2 (kwargs)
+                            32 DICT_MERGE               1
+                            34 CALL_FUNCTION_EX         1
+                            36 RETURN_VALUE
+               consts
+                  None
+               names      ('text', 'index')
+               varnames   ('self', 'args', 'kwargs')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
+               name       'tindex'
+               firstlineno 69
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 15
+               code
+                  0x970002007c006a0000000000000000006a0100000000000000007c0169
+                  007c02a4018e015300
+                72           0 RESUME                   0
+               
+                73           2 PUSH_NULL
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (text)
+                            16 LOAD_ATTR                1 (insert)
+                            26 LOAD_FAST                1 (args)
+                            28 BUILD_MAP                0
+                            30 LOAD_FAST                2 (kwargs)
+                            32 DICT_MERGE               1
+                            34 CALL_FUNCTION_EX         1
+                            36 RETURN_VALUE
+               consts
+                  None
+               names      ('text', 'insert')
+               varnames   ('self', 'args', 'kwargs')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
+               name       'tinsert'
+               firstlineno 72
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 15
+               code
+                  0x970002007c006a0000000000000000006a0100000000000000007c0169
+                  007c02a4018e015300
+                75           0 RESUME                   0
+               
+                76           2 PUSH_NULL
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (text)
+                            16 LOAD_ATTR                1 (search)
+                            26 LOAD_FAST                1 (args)
+                            28 BUILD_MAP                0
+                            30 LOAD_FAST                2 (kwargs)
+                            32 DICT_MERGE               1
+                            34 CALL_FUNCTION_EX         1
+                            36 RETURN_VALUE
+               consts
+                  None
+               names      ('text', 'search')
+               varnames   ('self', 'args', 'kwargs')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
+               name       'search'
+               firstlineno 75
+               lnotab 0x0201
+            code
+               argcount  : 1
+               nlocals   : 3
+               stacksize : 5
+               flags     : 15
+               code
+                  0x970002007c006a0000000000000000006a0100000000000000007c0169
+                  007c02a4018e015300
+                78           0 RESUME                   0
+               
+                79           2 PUSH_NULL
+                             4 LOAD_FAST                0 (self)
+                             6 LOAD_ATTR                0 (text)
+                            16 LOAD_ATTR                1 (see)
+                            26 LOAD_FAST                1 (args)
+                            28 BUILD_MAP                0
+                            30 LOAD_FAST                2 (kwargs)
+                            32 DICT_MERGE               1
+                            34 CALL_FUNCTION_EX         1
+                            36 RETURN_VALUE
+               consts
+                  None
+               names      ('text', 'see')
+               varnames   ('self', 'args', 'kwargs')
+               freevars   ()
+               cellvars   ()
+               filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
+               name       'see'
+               firstlineno 78
+               lnotab 0x0201
+            code
+               argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970009007c006a000000000000000000a0010000000000000000000000
                   000000000000000000a6000000ab00000000000000000001006400530023
                   000100590064005300780359007701
-                48           0 RESUME                   0
+                81           0 RESUME                   0
                
-                49           2 NOP
+                82           2 NOP
                
-                50           4 LOAD_FAST                0 (self)
+                83           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (text)
                             16 LOAD_METHOD              1 (edit_undo)
                             38 PRECALL                  0
                             42 CALL                     0
                             52 POP_TOP
                             54 LOAD_CONST               0 (None)
                             56 RETURN_VALUE
                        >>   58 PUSH_EXC_INFO
                
-                51          60 POP_TOP
+                84          60 POP_TOP
                
-                52          62 POP_EXCEPT
+                85          62 POP_EXCEPT
                             64 LOAD_CONST               0 (None)
                             66 RETURN_VALUE
                        >>   68 COPY                     3
                             70 POP_EXCEPT
                             72 RERAISE                  1
                ExceptionTable:
                  4 to 52 -> 58 [0]
@@ -993,42 +1369,42 @@
                   None
                names      ('text', 'edit_undo')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'undo'
-               firstlineno 48
+               firstlineno 81
                lnotab 0x0201020138010201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x970009007c006a000000000000000000a0010000000000000000000000
                   000000000000000000a6000000ab00000000000000000001006400530023
                   000100590064005300780359007701
-                54           0 RESUME                   0
+                87           0 RESUME                   0
                
-                55           2 NOP
+                88           2 NOP
                
-                56           4 LOAD_FAST                0 (self)
+                89           4 LOAD_FAST                0 (self)
                              6 LOAD_ATTR                0 (text)
                             16 LOAD_METHOD              1 (edit_redo)
                             38 PRECALL                  0
                             42 CALL                     0
                             52 POP_TOP
                             54 LOAD_CONST               0 (None)
                             56 RETURN_VALUE
                        >>   58 PUSH_EXC_INFO
                
-                57          60 POP_TOP
+                90          60 POP_TOP
                
-                58          62 POP_EXCEPT
+                91          62 POP_EXCEPT
                             64 LOAD_CONST               0 (None)
                             66 RETURN_VALUE
                        >>   68 COPY                     3
                             70 POP_EXCEPT
                             72 RERAISE                  1
                ExceptionTable:
                  4 to 52 -> 58 [0]
@@ -1037,61 +1413,61 @@
                   None
                names      ('text', 'edit_redo')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'redo'
-               firstlineno 54
+               firstlineno 87
                lnotab 0x0201020138010201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007401000000000000000000007c006401a6020000ab020000000000
                   000000721e7c00a00100000000000000000000000000000000000000007c
                   006a0200000000000000006402ac03a6020000ab02000000000000000001
                   006400530064005300
-                60           0 RESUME                   0
+                93           0 RESUME                   0
                
-                61           2 LOAD_GLOBAL              1 (NULL + hasattr)
+                94           2 LOAD_GLOBAL              1 (NULL + hasattr)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_CONST               1 ('button_frame_back')
                             18 PRECALL                  2
                             22 CALL                     2
                             32 POP_JUMP_FORWARD_IF_FALSE    30 (to 94)
                
-                62          34 LOAD_FAST                0 (self)
+                95          34 LOAD_FAST                0 (self)
                             36 LOAD_METHOD              1 (configure)
                             58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                2 (button_frame_back)
                             70 LOAD_CONST               2 (0)
                             72 KW_NAMES                 3
                             74 PRECALL                  2
                             78 CALL                     2
                             88 POP_TOP
                             90 LOAD_CONST               0 (None)
                             92 RETURN_VALUE
                
-                61     >>   94 LOAD_CONST               0 (None)
+                94     >>   94 LOAD_CONST               0 (None)
                             96 RETURN_VALUE
                consts
                   None
                   'button_frame_back'
                   0
                   ('background', 'borderwidth')
                names      ('hasattr', 'configure', 'button_frame_back')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_other'
-               firstlineno 60
+               firstlineno 93
                lnotab 0x020120013cff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 9
                flags     : 3
                code
@@ -1125,174 +1501,174 @@
                   00000000000000000000000000000000007c006a0e0000000000000000a6
                   010000ab01000000000000000001007c00a00f0000000000000000000000
                   0000000000000000007c006a0e00000000000000007c006a0b0000000000
                   000000a6020000ab02000000000000000001007c006a0a00000000000000
                   00a01000000000000000000000000000000000000000007c006a06000000
                   00000000007c006a11000000000000000064097c006a1100000000000000
                   00ac0aa6040000ab040000000000000000010064005300
-                64           0 RESUME                   0
+                97           0 RESUME                   0
                
-                65           2 LOAD_FAST                0 (self)
+                98           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-                67          44 LOAD_FAST                0 (self)
+               100          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_rectangle)
                
-                68          68 LOAD_CONST               2 (0)
+               101          68 LOAD_CONST               2 (0)
                             70 LOAD_CONST               2 (0)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (1)
                            112 BINARY_OP               10 (-)
                            116 LOAD_FAST                0 (self)
                            118 LOAD_METHOD              3 (winfo_height)
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (1)
                            156 BINARY_OP               10 (-)
                
-                69         160 LOAD_FAST                0 (self)
+               102         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (text_border_width)
                
-                70         172 LOAD_FAST                0 (self)
+               103         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (_text_border)
                            184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_text_back)
                
-                67         196 KW_NAMES                 4
+               100         196 KW_NAMES                 4
                            198 PRECALL                  7
                            202 CALL                     7
                            212 LOAD_FAST                0 (self)
                            214 STORE_ATTR               7 (text_frame)
                
-                73         224 LOAD_FAST                0 (self)
+               106         224 LOAD_FAST                0 (self)
                            226 LOAD_METHOD              8 (create_window)
                
-                74         248 LOAD_FAST                0 (self)
+               107         248 LOAD_FAST                0 (self)
                            250 LOAD_METHOD              2 (winfo_width)
                            272 PRECALL                  0
                            276 CALL                     0
                            286 LOAD_CONST               5 (2)
                            288 BINARY_OP               11 (/)
                            292 LOAD_FAST                0 (self)
                            294 LOAD_METHOD              3 (winfo_height)
                            316 PRECALL                  0
                            320 CALL                     0
                            330 LOAD_CONST               5 (2)
                            332 BINARY_OP               11 (/)
                
-                75         336 LOAD_FAST                0 (self)
+               108         336 LOAD_FAST                0 (self)
                            338 LOAD_METHOD              2 (winfo_width)
                            360 PRECALL                  0
                            364 CALL                     0
                            374 LOAD_FAST                0 (self)
                            376 LOAD_ATTR                4 (text_border_width)
                            386 BINARY_OP               10 (-)
                            390 LOAD_CONST               6 (5)
                            392 BINARY_OP               10 (-)
                            396 LOAD_FAST                0 (self)
                            398 LOAD_ATTR                9 (text_padding)
                            408 LOAD_CONST               2 (0)
                            410 BINARY_SUBSCR
                            420 BINARY_OP               10 (-)
                
-                76         424 LOAD_FAST                0 (self)
+               109         424 LOAD_FAST                0 (self)
                            426 LOAD_METHOD              3 (winfo_height)
                            448 PRECALL                  0
                            452 CALL                     0
                            462 LOAD_FAST                0 (self)
                            464 LOAD_ATTR                4 (text_border_width)
                            474 BINARY_OP               10 (-)
                            478 LOAD_CONST               6 (5)
                            480 BINARY_OP               10 (-)
                            484 LOAD_FAST                0 (self)
                            486 LOAD_ATTR                9 (text_padding)
                            496 LOAD_CONST               3 (1)
                            498 BINARY_SUBSCR
                            508 BINARY_OP               10 (-)
                
-                77         512 LOAD_FAST                0 (self)
+               110         512 LOAD_FAST                0 (self)
                            514 LOAD_ATTR               10 (text)
                
-                73         524 KW_NAMES                 7
+               106         524 KW_NAMES                 7
                            526 PRECALL                  5
                            530 CALL                     5
                            540 LOAD_FAST                0 (self)
                            542 STORE_ATTR              11 (text_text)
                
-                80         552 LOAD_FAST                0 (self)
+               113         552 LOAD_FAST                0 (self)
                            554 LOAD_METHOD              1 (create_rectangle)
                            576 LOAD_CONST               3 (1)
                            578 LOAD_FAST                0 (self)
                            580 LOAD_METHOD              3 (winfo_height)
                            602 PRECALL                  0
                            606 CALL                     0
                            616 LOAD_FAST                0 (self)
                            618 LOAD_ATTR               12 (_text_bottom_width)
                            628 BINARY_OP               10 (-)
                            632 LOAD_CONST               3 (1)
                            634 BINARY_OP               10 (-)
                
-                81         638 LOAD_FAST                0 (self)
+               114         638 LOAD_FAST                0 (self)
                            640 LOAD_METHOD              2 (winfo_width)
                            662 PRECALL                  0
                            666 CALL                     0
                            676 LOAD_CONST               3 (1)
                            678 BINARY_OP               10 (-)
                            682 LOAD_FAST                0 (self)
                            684 LOAD_METHOD              3 (winfo_height)
                            706 PRECALL                  0
                            710 CALL                     0
                            720 LOAD_CONST               3 (1)
                            722 BINARY_OP               10 (-)
                
-                82         726 LOAD_FAST                0 (self)
+               115         726 LOAD_FAST                0 (self)
                            728 LOAD_ATTR               13 (_text_bottom_line)
                            738 LOAD_FAST                0 (self)
                            740 LOAD_ATTR               13 (_text_bottom_line)
                
-                83         750 LOAD_CONST               2 (0)
+               116         750 LOAD_CONST               2 (0)
                
-                80         752 KW_NAMES                 8
+               113         752 KW_NAMES                 8
                            754 PRECALL                  7
                            758 CALL                     7
                            768 LOAD_FAST                0 (self)
                            770 STORE_ATTR              14 (text_bottom)
                
-                85         780 LOAD_FAST                0 (self)
+               118         780 LOAD_FAST                0 (self)
                            782 LOAD_ATTR               12 (_text_bottom_width)
                            792 LOAD_CONST               2 (0)
                            794 COMPARE_OP               2 (==)
                            800 POP_JUMP_FORWARD_IF_FALSE    26 (to 854)
                
-                86         802 LOAD_FAST                0 (self)
+               119         802 LOAD_FAST                0 (self)
                            804 LOAD_METHOD              0 (delete)
                            826 LOAD_FAST                0 (self)
                            828 LOAD_ATTR               14 (text_bottom)
                            838 PRECALL                  1
                            842 CALL                     1
                            852 POP_TOP
                
-                88     >>  854 LOAD_FAST                0 (self)
+               121     >>  854 LOAD_FAST                0 (self)
                            856 LOAD_METHOD             15 (tag_raise)
                            878 LOAD_FAST                0 (self)
                            880 LOAD_ATTR               14 (text_bottom)
                            890 LOAD_FAST                0 (self)
                            892 LOAD_ATTR               11 (text_text)
                            902 PRECALL                  2
                            906 CALL                     2
                            916 POP_TOP
                
-                90         918 LOAD_FAST                0 (self)
+               123         918 LOAD_FAST                0 (self)
                            920 LOAD_ATTR               10 (text)
                            930 LOAD_METHOD             16 (configure)
                            952 LOAD_FAST                0 (self)
                            954 LOAD_ATTR                6 (_text_back)
                            964 LOAD_FAST                0 (self)
                            966 LOAD_ATTR               17 (_text_text_back)
                            976 LOAD_CONST               9 (True)
@@ -1318,15 +1694,15 @@
                   ('background', 'foreground', 'autoseparators', 'insertbackground')
                names      ('delete', 'create_rectangle', 'winfo_width', 'winfo_height', 'text_border_width', '_text_border', '_text_back', 'text_frame', 'create_window', 'text_padding', 'text', 'text_text', '_text_bottom_width', '_text_bottom_line', 'text_bottom', 'tag_raise', 'configure', '_text_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_draw'
-               firstlineno 64
+               firstlineno 97
                lnotab
                   0x02012a0218015c010c0118fd1c0618015801580158010cfc1c07560158
                   01180102fd1c05160134024002
             None
             code
                argcount  : 2
                nlocals   : 2
@@ -1335,42 +1711,42 @@
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-                92           0 RESUME                   0
+               125           0 RESUME                   0
                
-                93           2 LOAD_FAST                0 (self)
+               126           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (text_focusin_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_text_back)
                
-                94          26 LOAD_FAST                0 (self)
+               127          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (text_focusin_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_text_border)
                
-                95          50 LOAD_FAST                0 (self)
+               128          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (text_focusin_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_text_text_back)
                
-                96          74 LOAD_FAST                0 (self)
+               129          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (text_focusin_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_text_bottom_line)
                
-                97          98 LOAD_FAST                0 (self)
+               130          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (text_focusin_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_text_bottom_width)
                
-                99         122 LOAD_FAST                0 (self)
+               132         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -1378,56 +1754,56 @@
                   None
                names      ('text_focusin_back', '_text_back', 'text_focusin_border', '_text_border', 'text_focusin_text_back', '_text_text_back', 'text_focusin_bottom_line', '_text_bottom_line', 'text_focusin_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_focus'
-               firstlineno 92
+               firstlineno 125
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               101           0 RESUME                   0
+               134           0 RESUME                   0
                
-               102           2 LOAD_FAST                0 (self)
+               135           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (text_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_text_back)
                
-               103          26 LOAD_FAST                0 (self)
+               136          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (text_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_text_border)
                
-               104          50 LOAD_FAST                0 (self)
+               137          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (text_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_text_text_back)
                
-               105          74 LOAD_FAST                0 (self)
+               138          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (text_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_text_bottom_line)
                
-               106          98 LOAD_FAST                0 (self)
+               139          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (text_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_text_bottom_width)
                
-               108         122 LOAD_FAST                0 (self)
+               141         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -1435,66 +1811,66 @@
                   None
                names      ('text_back', '_text_back', 'text_border', '_text_border', 'text_text_back', '_text_text_back', 'text_bottom_line', '_text_bottom_line', 'text_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_focusout'
-               firstlineno 101
+               firstlineno 134
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               110           0 RESUME                   0
+               143           0 RESUME                   0
                
-               111           2 LOAD_FAST                0 (self)
+               144           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_set)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('focus_set',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_click'
-               firstlineno 110
+               firstlineno 143
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x970064017c005f00000000000000000064005300
-               113           0 RESUME                   0
+               146           0 RESUME                   0
                
-               114           2 LOAD_CONST               1 (True)
+               147           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                   True
                names      ('hover',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_hover'
-               firstlineno 113
+               firstlineno 146
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
@@ -1502,177 +1878,177 @@
                   00ab000000000000000000735a64017c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c006a0a00000000000000007c005f0b00000000000000007c00a0
                   0c00000000000000000000000000000000000000006400a6010000ab0100
                   0000000000000001006400530064005300
-               116           0 RESUME                   0
+               149           0 RESUME                   0
                
-               117           2 LOAD_FAST                0 (self)
+               150           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_get)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_JUMP_FORWARD_IF_TRUE    90 (to 222)
                
-               118          42 LOAD_CONST               1 (False)
+               151          42 LOAD_CONST               1 (False)
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (hover)
                
-               119          56 LOAD_FAST                0 (self)
+               152          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (text_back)
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (_text_back)
                
-               120          80 LOAD_FAST                0 (self)
+               153          80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                4 (text_border)
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               5 (_text_border)
                
-               121         104 LOAD_FAST                0 (self)
+               154         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                6 (text_text_back)
                            116 LOAD_FAST                0 (self)
                            118 STORE_ATTR               7 (_text_text_back)
                
-               122         128 LOAD_FAST                0 (self)
+               155         128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                8 (text_bottom_line)
                            140 LOAD_FAST                0 (self)
                            142 STORE_ATTR               9 (_text_bottom_line)
                
-               123         152 LOAD_FAST                0 (self)
+               156         152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR               10 (text_bottom_width)
                            164 LOAD_FAST                0 (self)
                            166 STORE_ATTR              11 (_text_bottom_width)
                
-               125         176 LOAD_FAST                0 (self)
+               158         176 LOAD_FAST                0 (self)
                            178 LOAD_METHOD             12 (_draw)
                            200 LOAD_CONST               0 (None)
                            202 PRECALL                  1
                            206 CALL                     1
                            216 POP_TOP
                            218 LOAD_CONST               0 (None)
                            220 RETURN_VALUE
                
-               117     >>  222 LOAD_CONST               0 (None)
+               150     >>  222 LOAD_CONST               0 (None)
                            224 RETURN_VALUE
                consts
                   None
                   False
                names      ('focus_get', 'hover', 'text_back', '_text_back', 'text_border', '_text_border', 'text_text_back', '_text_text_back', 'text_bottom_line', '_text_bottom_line', 'text_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_hover_release'
-               firstlineno 116
+               firstlineno 149
                lnotab 0x020128010e01180118011801180118022ef8
             'font'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               127           0 RESUME                   0
+               160           0 RESUME                   0
                
-               128           2 LOAD_FAST                1 (font)
+               161           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               129           6 LOAD_FAST                0 (self)
+               162           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (text_text_font)
                             18 RETURN_VALUE
                
-               131     >>   20 LOAD_FAST                1 (font)
+               164     >>   20 LOAD_FAST                1 (font)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (text_text_font)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('text_text_font',)
                varnames   ('self', 'font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'font'
-               firstlineno 127
+               firstlineno 160
                lnotab 0x020104010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               133           0 RESUME                   0
+               166           0 RESUME                   0
                
-               134           2 LOAD_FAST                0 (self)
+               167           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 133
+               firstlineno 166
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 16
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640564086409640a640b640c640d9c0da60100
                   00ab010000000000000000010064005300
-               136           0 RESUME                   0
+               169           0 RESUME                   0
                
-               137           2 LOAD_FAST                0 (self)
+               170           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               139          26 LOAD_CONST               1 ((3, 4))
+               172          26 LOAD_CONST               1 ((3, 4))
                
-               141          28 LOAD_CONST               2 ('#f3f3f3')
+               174          28 LOAD_CONST               2 ('#f3f3f3')
                
-               142          30 LOAD_CONST               3 (1)
+               175          30 LOAD_CONST               3 (1)
                
-               143          32 LOAD_CONST               4 (0)
+               176          32 LOAD_CONST               4 (0)
                
-               145          34 LOAD_CONST               5 ('#eaeaea')
+               178          34 LOAD_CONST               5 ('#eaeaea')
                
-               146          36 LOAD_CONST               6 ('#fdfdfd')
+               179          36 LOAD_CONST               6 ('#fdfdfd')
                
-               147          38 LOAD_CONST               7 ('#5f5f5f')
+               180          38 LOAD_CONST               7 ('#5f5f5f')
                
-               148          40 LOAD_CONST               5 ('#eaeaea')
+               181          40 LOAD_CONST               5 ('#eaeaea')
                
-               150          42 LOAD_CONST               8 ('#e2e2e2')
+               183          42 LOAD_CONST               8 ('#e2e2e2')
                
-               151          44 LOAD_CONST               9 ('#f9f9f9')
+               184          44 LOAD_CONST               9 ('#f9f9f9')
                
-               152          46 LOAD_CONST              10 ('#1a1a1a')
+               185          46 LOAD_CONST              10 ('#1a1a1a')
                
-               153          48 LOAD_CONST              11 ('#185fb4')
+               186          48 LOAD_CONST              11 ('#185fb4')
                
-               154          50 LOAD_CONST              12 (2)
+               187          50 LOAD_CONST              12 (2)
                
-               138          52 LOAD_CONST              13 (('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
+               171          52 LOAD_CONST              13 (('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
                             54 BUILD_CONST_KEY_MAP     13
                
-               137          56 PRECALL                  1
+               170          56 PRECALL                  1
                             60 CALL                     1
                             70 POP_TOP
                             72 LOAD_CONST               0 (None)
                             74 RETURN_VALUE
                consts
                   None
                   (3, 4)
@@ -1690,62 +2066,62 @@
                   ('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette_light'
-               firstlineno 136
+               firstlineno 169
                lnotab
                   0x0201180202020201020102020201020102010202020102010201020102
                   f004ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 16
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   02640364046405640664076408640464096407640a640b640c9c0da60100
                   00ab010000000000000000010064005300
-               158           0 RESUME                   0
+               191           0 RESUME                   0
                
-               159           2 LOAD_FAST                0 (self)
+               192           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               161          26 LOAD_CONST               1 ((3, 4))
+               194          26 LOAD_CONST               1 ((3, 4))
                
-               163          28 LOAD_CONST               2 ('#202020')
+               196          28 LOAD_CONST               2 ('#202020')
                
-               164          30 LOAD_CONST               3 (1)
+               197          30 LOAD_CONST               3 (1)
                
-               166          32 LOAD_CONST               4 ('#454545')
+               199          32 LOAD_CONST               4 ('#454545')
                
-               167          34 LOAD_CONST               5 ('#353535')
+               200          34 LOAD_CONST               5 ('#353535')
                
-               168          36 LOAD_CONST               6 ('#cecece')
+               201          36 LOAD_CONST               6 ('#cecece')
                
-               169          38 LOAD_CONST               7 ('#ffffff')
+               202          38 LOAD_CONST               7 ('#ffffff')
                
-               170          40 LOAD_CONST               8 (0)
+               203          40 LOAD_CONST               8 (0)
                
-               172          42 LOAD_CONST               4 ('#454545')
+               205          42 LOAD_CONST               4 ('#454545')
                
-               173          44 LOAD_CONST               9 ('#2f2f2f')
+               206          44 LOAD_CONST               9 ('#2f2f2f')
                
-               174          46 LOAD_CONST               7 ('#ffffff')
+               207          46 LOAD_CONST               7 ('#ffffff')
                
-               175          48 LOAD_CONST              10 ('#4cc2ff')
+               208          48 LOAD_CONST              10 ('#4cc2ff')
                
-               176          50 LOAD_CONST              11 (2)
+               209          50 LOAD_CONST              11 (2)
                
-               160          52 LOAD_CONST              12 (('text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
+               193          52 LOAD_CONST              12 (('text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
                             54 BUILD_CONST_KEY_MAP     13
                
-               159          56 PRECALL                  1
+               192          56 PRECALL                  1
                             60 CALL                     1
                             70 POP_TOP
                             72 LOAD_CONST               0 (None)
                             74 RETURN_VALUE
                consts
                   None
                   (3, 4)
@@ -1762,15 +2138,15 @@
                   ('text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette_dark'
-               firstlineno 158
+               firstlineno 191
                lnotab
                   0x0201180202020201020202010201020102010202020102010201020102
                   f004ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 11
@@ -1791,154 +2167,154 @@
                   00000000000000000000006400a6010000ab010000000000000000010064
                   0053002300741c0000000000000000000024007204010059006400530077
                   007803590077017c006a0000000000000000007c006a0100000000000000
                   007c006a0200000000000000007c006a0700000000000000007c006a0300
                   000000000000007c006a0400000000000000007c006a0500000000000000
                   007c006a0800000000000000007c006a0900000000000000007c006a0a00
                   00000000000000640e9c0a5300
-               180           0 RESUME                   0
+               213           0 RESUME                   0
                
-               181           2 LOAD_FAST                1 (dict)
+               214           2 LOAD_FAST                1 (dict)
                              4 POP_JUMP_FORWARD_IF_NONE   210 (to 426)
                
-               182           6 LOAD_FAST                1 (dict)
+               215           6 LOAD_FAST                1 (dict)
                              8 LOAD_CONST               1 ('text_padding')
                             10 BINARY_SUBSCR
                             20 LOAD_FAST                0 (self)
                             22 STORE_ATTR               0 (text_padding)
                
-               184          32 LOAD_FAST                1 (dict)
+               217          32 LOAD_FAST                1 (dict)
                             34 LOAD_CONST               2 ('text_frame_back')
                             36 BINARY_SUBSCR
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               1 (text_frame_back)
                
-               185          58 LOAD_FAST                1 (dict)
+               218          58 LOAD_FAST                1 (dict)
                             60 LOAD_CONST               3 ('text_border_width')
                             62 BINARY_SUBSCR
                             72 LOAD_FAST                0 (self)
                             74 STORE_ATTR               2 (text_border_width)
                
-               187          84 LOAD_FAST                1 (dict)
+               220          84 LOAD_FAST                1 (dict)
                             86 LOAD_CONST               4 ('text_border')
                             88 BINARY_SUBSCR
                             98 LOAD_FAST                0 (self)
                            100 STORE_ATTR               3 (text_border)
                
-               188         110 LOAD_FAST                1 (dict)
+               221         110 LOAD_FAST                1 (dict)
                            112 LOAD_CONST               5 ('text_back')
                            114 BINARY_SUBSCR
                            124 LOAD_FAST                0 (self)
                            126 STORE_ATTR               4 (text_back)
                
-               189         136 LOAD_FAST                1 (dict)
+               222         136 LOAD_FAST                1 (dict)
                            138 LOAD_CONST               6 ('text_text_back')
                            140 BINARY_SUBSCR
                            150 LOAD_FAST                0 (self)
                            152 STORE_ATTR               5 (text_text_back)
                
-               190         162 LOAD_FAST                1 (dict)
+               223         162 LOAD_FAST                1 (dict)
                            164 LOAD_CONST               7 ('text_bottom_line')
                            166 BINARY_SUBSCR
                            176 LOAD_FAST                0 (self)
                            178 STORE_ATTR               6 (text_bottom_line)
                
-               191         188 LOAD_FAST                1 (dict)
+               224         188 LOAD_FAST                1 (dict)
                            190 LOAD_CONST               8 ('text_bottom_width')
                            192 BINARY_SUBSCR
                            202 LOAD_FAST                0 (self)
                            204 STORE_ATTR               7 (text_bottom_width)
                
-               193         214 LOAD_FAST                1 (dict)
+               226         214 LOAD_FAST                1 (dict)
                            216 LOAD_CONST               9 ('text_focusin_border')
                            218 BINARY_SUBSCR
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               8 (text_focusin_border)
                
-               194         240 LOAD_FAST                1 (dict)
+               227         240 LOAD_FAST                1 (dict)
                            242 LOAD_CONST              10 ('text_focusin_back')
                            244 BINARY_SUBSCR
                            254 LOAD_FAST                0 (self)
                            256 STORE_ATTR               9 (text_focusin_back)
                
-               195         266 LOAD_FAST                1 (dict)
+               228         266 LOAD_FAST                1 (dict)
                            268 LOAD_CONST              11 ('text_focusin_text_back')
                            270 BINARY_SUBSCR
                            280 LOAD_FAST                0 (self)
                            282 STORE_ATTR              10 (text_focusin_text_back)
                
-               196         292 LOAD_FAST                1 (dict)
+               229         292 LOAD_FAST                1 (dict)
                            294 LOAD_CONST              12 ('text_focusin_bottom_line')
                            296 BINARY_SUBSCR
                            306 LOAD_FAST                0 (self)
                            308 STORE_ATTR              11 (text_focusin_bottom_line)
                
-               197         318 LOAD_FAST                1 (dict)
+               230         318 LOAD_FAST                1 (dict)
                            320 LOAD_CONST              13 ('text_focusin_bottom_width')
                            322 BINARY_SUBSCR
                            332 LOAD_FAST                0 (self)
                            334 STORE_ATTR              12 (text_focusin_bottom_width)
                
-               199         344 NOP
+               232         344 NOP
                
-               200         346 LOAD_FAST                0 (self)
+               233         346 LOAD_FAST                0 (self)
                            348 LOAD_METHOD             13 (_draw)
                            370 LOAD_CONST               0 (None)
                            372 PRECALL                  1
                            376 CALL                     1
                            386 POP_TOP
                            388 LOAD_CONST               0 (None)
                            390 RETURN_VALUE
                        >>  392 PUSH_EXC_INFO
                
-               201         394 LOAD_GLOBAL             28 (AttributeError)
+               234         394 LOAD_GLOBAL             28 (AttributeError)
                            406 CHECK_EXC_MATCH
                            408 POP_JUMP_FORWARD_IF_FALSE     4 (to 418)
                            410 POP_TOP
                
-               202         412 POP_EXCEPT
+               235         412 POP_EXCEPT
                            414 LOAD_CONST               0 (None)
                            416 RETURN_VALUE
                
-               201     >>  418 RERAISE                  0
+               234     >>  418 RERAISE                  0
                        >>  420 COPY                     3
                            422 POP_EXCEPT
                            424 RERAISE                  1
                
-               205     >>  426 LOAD_FAST                0 (self)
+               238     >>  426 LOAD_FAST                0 (self)
                            428 LOAD_ATTR                0 (text_padding)
                
-               207         438 LOAD_FAST                0 (self)
+               240         438 LOAD_FAST                0 (self)
                            440 LOAD_ATTR                1 (text_frame_back)
                
-               208         450 LOAD_FAST                0 (self)
+               241         450 LOAD_FAST                0 (self)
                            452 LOAD_ATTR                2 (text_border_width)
                
-               209         462 LOAD_FAST                0 (self)
+               242         462 LOAD_FAST                0 (self)
                            464 LOAD_ATTR                7 (text_bottom_width)
                
-               211         474 LOAD_FAST                0 (self)
+               244         474 LOAD_FAST                0 (self)
                            476 LOAD_ATTR                3 (text_border)
                
-               212         486 LOAD_FAST                0 (self)
+               245         486 LOAD_FAST                0 (self)
                            488 LOAD_ATTR                4 (text_back)
                
-               213         498 LOAD_FAST                0 (self)
+               246         498 LOAD_FAST                0 (self)
                            500 LOAD_ATTR                5 (text_text_back)
                
-               215         510 LOAD_FAST                0 (self)
+               248         510 LOAD_FAST                0 (self)
                            512 LOAD_ATTR                8 (text_focusin_border)
                
-               216         522 LOAD_FAST                0 (self)
+               249         522 LOAD_FAST                0 (self)
                            524 LOAD_ATTR                9 (text_focusin_back)
                
-               217         534 LOAD_FAST                0 (self)
+               250         534 LOAD_FAST                0 (self)
                            536 LOAD_ATTR               10 (text_focusin_text_back)
                
-               204         546 LOAD_CONST              14 (('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back'))
+               237         546 LOAD_CONST              14 (('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back'))
                            548 BUILD_CONST_KEY_MAP     10
                            550 RETURN_VALUE
                ExceptionTable:
                  346 to 386 -> 392 [0]
                  392 to 410 -> 420 [1] lasti
                  418 to 418 -> 420 [1] lasti
                consts
@@ -1959,141 +2335,141 @@
                   ('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back')
                names      ('text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette'
-               firstlineno 180
+               firstlineno 213
                lnotab
                   0x020104011a021a011a021a011a011a011a011a021a011a011a011a011a
                   0202013001120106ff08040c020c010c010c020c010c010c020c010c010c
                   f3
             (None,)
-         names      ('__name__', '__module__', '__qualname__', '__init__', 'undo', 'redo', '_other', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
+         names      ('__name__', '__module__', '__qualname__', '__init__', 'tbbox', 'compare', 'count', 'debug', 'tdelete', 'dump', 'get', 'tindex', 'tinsert', 'search', 'see', 'undo', 'redo', '_other', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawBasicText'
          firstlineno 6
          lnotab
-            0x0c011229060606060604061c0809080908030803080b0e060603061606
-            16
+            0x0c01122906030603060306030603060306030603060306030603060606
+            060604061c0809080908030803080b0e06060306160616
       'AdwDrawBasicText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         221           0 RESUME                   0
+         254           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawText')
                        8 STORE_NAME               2 (__qualname__)
          
-         222          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 222>)
+         255          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 255>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               222           0 RESUME                   0
+               255           0 RESUME                   0
                
-               223           2 LOAD_FAST                0 (self)
+               256           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 222
+               firstlineno 255
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawText'
-         firstlineno 221
+         firstlineno 254
          lnotab 0x0a01
       'AdwDrawText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         226           0 RESUME                   0
+         259           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawDarkText')
                        8 STORE_NAME               2 (__qualname__)
          
-         227          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 227>)
+         260          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 260>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawDarkText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               227           0 RESUME                   0
+               260           0 RESUME                   0
                
-               228           2 LOAD_FAST                0 (self)
+               261           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 227
+               firstlineno 260
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawDarkText'
-         firstlineno 226
+         firstlineno 259
          lnotab 0x0a01
       'AdwDrawDarkText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
@@ -2101,91 +2477,91 @@
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
             126404650565067a0700006602640584055a07640684005a086412640784
             015a096412640884015a0a6412640984015a0b6412640a84015a0c641264
             0b84015a0d6412640c650e6602640d84055a0f640e84005a10640f84005a
             11641084005a126412641184015a13880078015a145300
                        0 MAKE_CELL                0 (__class__)
          
-         232           2 RESUME                   0
+         265           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundText')
                       10 STORE_NAME               2 (__qualname__)
          
-         233          12 LOAD_CLOSURE             0 (__class__)
+         266          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\textbox.py", line 233>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\textbox.py", line 266>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         236          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\textbox.py", line 236>)
+         269          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\textbox.py", line 269>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_other)
          
-         239          28 LOAD_CONST              18 ((None,))
+         272          28 LOAD_CONST              18 ((None,))
                       30 LOAD_CONST               4 ('radius')
                       32 LOAD_NAME                5 (float)
                       34 LOAD_NAME                6 (int)
                       36 BINARY_OP                7 (|)
                       40 BUILD_TUPLE              2
-                      42 LOAD_CONST               5 (<code object border_radius, file "D:\tkadw\tkadw\canvas\textbox.py", line 239>)
+                      42 LOAD_CONST               5 (<code object border_radius, file "D:\tkadw\tkadw\canvas\textbox.py", line 272>)
                       44 MAKE_FUNCTION            5 (defaults, annotations)
                       46 STORE_NAME               7 (border_radius)
          
-         245          48 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\canvas\textbox.py", line 245>)
+         278          48 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\canvas\textbox.py", line 278>)
                       50 MAKE_FUNCTION            0
                       52 STORE_NAME               8 (_draw)
          
-         275          54 LOAD_CONST              18 ((None,))
-                      56 LOAD_CONST               7 (<code object _focus, file "D:\tkadw\tkadw\canvas\textbox.py", line 275>)
+         308          54 LOAD_CONST              18 ((None,))
+                      56 LOAD_CONST               7 (<code object _focus, file "D:\tkadw\tkadw\canvas\textbox.py", line 308>)
                       58 MAKE_FUNCTION            1 (defaults)
                       60 STORE_NAME               9 (_focus)
          
-         284          62 LOAD_CONST              18 ((None,))
-                      64 LOAD_CONST               8 (<code object _focusout, file "D:\tkadw\tkadw\canvas\textbox.py", line 284>)
+         317          62 LOAD_CONST              18 ((None,))
+                      64 LOAD_CONST               8 (<code object _focusout, file "D:\tkadw\tkadw\canvas\textbox.py", line 317>)
                       66 MAKE_FUNCTION            1 (defaults)
                       68 STORE_NAME              10 (_focusout)
          
-         293          70 LOAD_CONST              18 ((None,))
-                      72 LOAD_CONST               9 (<code object _click, file "D:\tkadw\tkadw\canvas\textbox.py", line 293>)
+         326          70 LOAD_CONST              18 ((None,))
+                      72 LOAD_CONST               9 (<code object _click, file "D:\tkadw\tkadw\canvas\textbox.py", line 326>)
                       74 MAKE_FUNCTION            1 (defaults)
                       76 STORE_NAME              11 (_click)
          
-         296          78 LOAD_CONST              18 ((None,))
-                      80 LOAD_CONST              10 (<code object _hover, file "D:\tkadw\tkadw\canvas\textbox.py", line 296>)
+         329          78 LOAD_CONST              18 ((None,))
+                      80 LOAD_CONST              10 (<code object _hover, file "D:\tkadw\tkadw\canvas\textbox.py", line 329>)
                       82 MAKE_FUNCTION            1 (defaults)
                       84 STORE_NAME              12 (_hover)
          
-         299          86 LOAD_CONST              18 ((None,))
-                      88 LOAD_CONST              11 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\textbox.py", line 299>)
+         332          86 LOAD_CONST              18 ((None,))
+                      88 LOAD_CONST              11 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\textbox.py", line 332>)
                       90 MAKE_FUNCTION            1 (defaults)
                       92 STORE_NAME              13 (_hover_release)
          
-         310          94 LOAD_CONST              18 ((None,))
+         343          94 LOAD_CONST              18 ((None,))
                       96 LOAD_CONST              12 ('font')
                       98 LOAD_NAME               14 (Font)
                      100 BUILD_TUPLE              2
-                     102 LOAD_CONST              13 (<code object font, file "D:\tkadw\tkadw\canvas\textbox.py", line 310>)
+                     102 LOAD_CONST              13 (<code object font, file "D:\tkadw\tkadw\canvas\textbox.py", line 343>)
                      104 MAKE_FUNCTION            5 (defaults, annotations)
                      106 STORE_NAME              15 (font)
          
-         316         108 LOAD_CONST              14 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 316>)
+         349         108 LOAD_CONST              14 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 349>)
                      110 MAKE_FUNCTION            0
                      112 STORE_NAME              16 (default_palette)
          
-         319         114 LOAD_CONST              15 (<code object palette_light, file "D:\tkadw\tkadw\canvas\textbox.py", line 319>)
+         352         114 LOAD_CONST              15 (<code object palette_light, file "D:\tkadw\tkadw\canvas\textbox.py", line 352>)
                      116 MAKE_FUNCTION            0
                      118 STORE_NAME              17 (palette_light)
          
-         343         120 LOAD_CONST              16 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\textbox.py", line 343>)
+         376         120 LOAD_CONST              16 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\textbox.py", line 376>)
                      122 MAKE_FUNCTION            0
                      124 STORE_NAME              18 (palette_dark)
          
-         367         126 LOAD_CONST              18 ((None,))
-                     128 LOAD_CONST              17 (<code object palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 367>)
+         400         126 LOAD_CONST              18 ((None,))
+                     128 LOAD_CONST              17 (<code object palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 400>)
                      130 MAKE_FUNCTION            1 (defaults)
                      132 STORE_NAME              19 (palette)
                      134 LOAD_CLOSURE             0 (__class__)
                      136 COPY                     1
                      138 STORE_NAME              20 (__classcell__)
                      140 RETURN_VALUE
          consts
@@ -2196,17 +2572,17 @@
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               233           2 RESUME                   0
+               266           2 RESUME                   0
                
-               234           4 PUSH_NULL
+               267           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -2219,29 +2595,29 @@
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '__init__'
-               firstlineno 233
+               firstlineno 266
                lnotab 0x0401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c006a
                   010000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab0100000000000000006402ac03a6020000ab02000000
                   0000000000010064005300
-               236           0 RESUME                   0
+               269           0 RESUME                   0
                
-               237           2 LOAD_FAST                0 (self)
+               270           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (configure)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (master)
                             38 LOAD_METHOD              2 (cget)
                             60 LOAD_CONST               1 ('bg')
                             62 PRECALL                  1
                             66 CALL                     1
@@ -2259,49 +2635,49 @@
                   ('background', 'borderwidth')
                names      ('configure', 'master', 'cget')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_other'
-               firstlineno 236
+               firstlineno 269
                lnotab 0x0201
             None
             'radius'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               239           0 RESUME                   0
+               272           0 RESUME                   0
                
-               240           2 LOAD_FAST                1 (radius)
+               273           2 LOAD_FAST                1 (radius)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               241           6 LOAD_FAST                0 (self)
+               274           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_radius)
                             18 RETURN_VALUE
                
-               243     >>   20 LOAD_FAST                1 (radius)
+               276     >>   20 LOAD_FAST                1 (radius)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_radius)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_radius',)
                varnames   ('self', 'radius')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'border_radius'
-               firstlineno 239
+               firstlineno 272
                lnotab 0x020104010e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -2337,27 +2713,27 @@
                   000000000000000000000000007c006a100000000000000000a6010000ab
                   01000000000000000001007c00a011000000000000000000000000000000
                   00000000007c006a1000000000000000007c006a0c0000000000000000a6
                   020000ab02000000000000000001007c006a0b0000000000000000a01200
                   000000000000000000000000000000000000007c006a0700000000000000
                   007c006a1300000000000000007c006a130000000000000000ac0ba60300
                   00ab030000000000000000010064005300
-               245           0 RESUME                   0
+               278           0 RESUME                   0
                
-               246           2 LOAD_FAST                0 (self)
+               279           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               248          44 LOAD_FAST                0 (self)
+               281          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect2)
                
-               249          68 LOAD_CONST               2 (2)
+               282          68 LOAD_CONST               2 (2)
                             70 LOAD_CONST               2 (2)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (3)
                            112 BINARY_OP               10 (-)
@@ -2366,159 +2742,159 @@
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (3)
                            156 BINARY_OP               10 (-)
                            160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (text_radius)
                
-               250         172 LOAD_FAST                0 (self)
+               283         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (text_border_width)
                
-               251         184 LOAD_FAST                0 (self)
+               284         184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_text_border)
                            196 LOAD_FAST                0 (self)
                            198 LOAD_ATTR                7 (_text_back)
                
-               248         208 KW_NAMES                 4
+               281         208 KW_NAMES                 4
                            210 PRECALL                  8
                            214 CALL                     8
                            224 LOAD_FAST                0 (self)
                            226 STORE_ATTR               8 (text_frame)
                
-               254         236 LOAD_FAST                0 (self)
+               287         236 LOAD_FAST                0 (self)
                            238 LOAD_METHOD              9 (create_window)
                
-               255         260 LOAD_FAST                0 (self)
+               288         260 LOAD_FAST                0 (self)
                            262 LOAD_METHOD              2 (winfo_width)
                            284 PRECALL                  0
                            288 CALL                     0
                            298 LOAD_CONST               2 (2)
                            300 BINARY_OP               11 (/)
                            304 LOAD_FAST                0 (self)
                            306 LOAD_METHOD              3 (winfo_height)
                            328 PRECALL                  0
                            332 CALL                     0
                            342 LOAD_CONST               2 (2)
                            344 BINARY_OP               11 (/)
                
-               256         348 LOAD_FAST                0 (self)
+               289         348 LOAD_FAST                0 (self)
                            350 LOAD_METHOD              2 (winfo_width)
                            372 PRECALL                  0
                            376 CALL                     0
                            386 LOAD_FAST                0 (self)
                            388 LOAD_ATTR                5 (text_border_width)
                            398 BINARY_OP               10 (-)
                            402 LOAD_CONST               5 (5)
                            404 BINARY_OP               10 (-)
                            408 LOAD_FAST                0 (self)
                            410 LOAD_ATTR               10 (text_padding)
                            420 LOAD_CONST               6 (0)
                            422 BINARY_SUBSCR
                            432 BINARY_OP               10 (-)
                
-               257         436 LOAD_FAST                0 (self)
+               290         436 LOAD_FAST                0 (self)
                            438 LOAD_METHOD              3 (winfo_height)
                            460 PRECALL                  0
                            464 CALL                     0
                            474 LOAD_FAST                0 (self)
                            476 LOAD_ATTR                5 (text_border_width)
                            486 BINARY_OP               10 (-)
                            490 LOAD_CONST               5 (5)
                            492 BINARY_OP               10 (-)
                            496 LOAD_FAST                0 (self)
                            498 LOAD_ATTR               10 (text_padding)
                            508 LOAD_CONST               7 (1)
                            510 BINARY_SUBSCR
                            520 BINARY_OP               10 (-)
                
-               258         524 LOAD_FAST                0 (self)
+               291         524 LOAD_FAST                0 (self)
                            526 LOAD_ATTR               11 (text)
                
-               254         536 KW_NAMES                 8
+               287         536 KW_NAMES                 8
                            538 PRECALL                  5
                            542 CALL                     5
                            552 LOAD_FAST                0 (self)
                            554 STORE_ATTR              12 (text_text)
                
-               261         564 LOAD_FAST                0 (self)
+               294         564 LOAD_FAST                0 (self)
                            566 LOAD_METHOD             13 (create_rectangle)
                            588 LOAD_CONST               3 (3)
                            590 LOAD_FAST                0 (self)
                            592 LOAD_ATTR                4 (text_radius)
                            602 LOAD_CONST               2 (2)
                            604 BINARY_OP               11 (/)
                            608 BINARY_OP                0 (+)
                
-               262         612 LOAD_FAST                0 (self)
+               295         612 LOAD_FAST                0 (self)
                            614 LOAD_METHOD              3 (winfo_height)
                            636 PRECALL                  0
                            640 CALL                     0
                            650 LOAD_FAST                0 (self)
                            652 LOAD_ATTR               14 (_text_bottom_width)
                            662 BINARY_OP               10 (-)
                            666 LOAD_CONST               3 (3)
                            668 BINARY_OP               10 (-)
                
-               263         672 LOAD_FAST                0 (self)
+               296         672 LOAD_FAST                0 (self)
                            674 LOAD_METHOD              2 (winfo_width)
                            696 PRECALL                  0
                            700 CALL                     0
                            710 LOAD_CONST               3 (3)
                            712 BINARY_OP               10 (-)
                            716 LOAD_FAST                0 (self)
                            718 LOAD_ATTR                4 (text_radius)
                            728 LOAD_CONST               2 (2)
                            730 BINARY_OP               11 (/)
                            734 BINARY_OP               10 (-)
                
-               264         738 LOAD_FAST                0 (self)
+               297         738 LOAD_FAST                0 (self)
                            740 LOAD_METHOD              3 (winfo_height)
                            762 PRECALL                  0
                            766 CALL                     0
                            776 LOAD_CONST               9 (3.5)
                            778 BINARY_OP               10 (-)
                
-               265         782 LOAD_FAST                0 (self)
+               298         782 LOAD_FAST                0 (self)
                            784 LOAD_ATTR               15 (_text_bottom_line)
                            794 LOAD_FAST                0 (self)
                            796 LOAD_ATTR               15 (_text_bottom_line)
                
-               266         806 LOAD_CONST               6 (0)
+               299         806 LOAD_CONST               6 (0)
                
-               261         808 KW_NAMES                10
+               294         808 KW_NAMES                10
                            810 PRECALL                  7
                            814 CALL                     7
                            824 LOAD_FAST                0 (self)
                            826 STORE_ATTR              16 (text_bottom)
                
-               268         836 LOAD_FAST                0 (self)
+               301         836 LOAD_FAST                0 (self)
                            838 LOAD_ATTR               14 (_text_bottom_width)
                            848 LOAD_CONST               6 (0)
                            850 COMPARE_OP               2 (==)
                            856 POP_JUMP_FORWARD_IF_FALSE    26 (to 910)
                
-               269         858 LOAD_FAST                0 (self)
+               302         858 LOAD_FAST                0 (self)
                            860 LOAD_METHOD              0 (delete)
                            882 LOAD_FAST                0 (self)
                            884 LOAD_ATTR               16 (text_bottom)
                            894 PRECALL                  1
                            898 CALL                     1
                            908 POP_TOP
                
-               271     >>  910 LOAD_FAST                0 (self)
+               304     >>  910 LOAD_FAST                0 (self)
                            912 LOAD_METHOD             17 (tag_raise)
                            934 LOAD_FAST                0 (self)
                            936 LOAD_ATTR               16 (text_bottom)
                            946 LOAD_FAST                0 (self)
                            948 LOAD_ATTR               12 (text_text)
                            958 PRECALL                  2
                            962 CALL                     2
                            972 POP_TOP
                
-               273         974 LOAD_FAST                0 (self)
+               306         974 LOAD_FAST                0 (self)
                            976 LOAD_ATTR               11 (text)
                            986 LOAD_METHOD             18 (configure)
                           1008 LOAD_FAST                0 (self)
                           1010 LOAD_ATTR                7 (_text_back)
                           1020 LOAD_FAST                0 (self)
                           1022 LOAD_ATTR               19 (_text_text_back)
                           1032 LOAD_FAST                0 (self)
@@ -2544,15 +2920,15 @@
                   ('background', 'foreground', 'insertbackground')
                names      ('delete', 'create_round_rect2', 'winfo_width', 'winfo_height', 'text_radius', 'text_border_width', '_text_border', '_text_back', 'text_frame', 'create_window', 'text_padding', 'text', 'text_text', 'create_rectangle', '_text_bottom_width', '_text_bottom_line', 'text_bottom', 'tag_raise', 'configure', '_text_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_draw'
-               firstlineno 245
+               firstlineno 278
                lnotab
                   0x02012a02180168010c0118fd1c0618015801580158010cfc1c0730013c
                   0142012c01180102fb1c07160134024002
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -2560,42 +2936,42 @@
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               275           0 RESUME                   0
+               308           0 RESUME                   0
                
-               276           2 LOAD_FAST                0 (self)
+               309           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (text_focusin_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_text_back)
                
-               277          26 LOAD_FAST                0 (self)
+               310          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (text_focusin_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_text_border)
                
-               278          50 LOAD_FAST                0 (self)
+               311          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (text_focusin_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_text_text_back)
                
-               279          74 LOAD_FAST                0 (self)
+               312          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (text_focusin_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_text_bottom_line)
                
-               280          98 LOAD_FAST                0 (self)
+               313          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (text_focusin_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_text_bottom_width)
                
-               282         122 LOAD_FAST                0 (self)
+               315         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -2603,56 +2979,56 @@
                   None
                names      ('text_focusin_back', '_text_back', 'text_focusin_border', '_text_border', 'text_focusin_text_back', '_text_text_back', 'text_focusin_bottom_line', '_text_bottom_line', 'text_focusin_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_focus'
-               firstlineno 275
+               firstlineno 308
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               284           0 RESUME                   0
+               317           0 RESUME                   0
                
-               285           2 LOAD_FAST                0 (self)
+               318           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (text_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_text_back)
                
-               286          26 LOAD_FAST                0 (self)
+               319          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (text_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_text_border)
                
-               287          50 LOAD_FAST                0 (self)
+               320          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (text_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_text_text_back)
                
-               288          74 LOAD_FAST                0 (self)
+               321          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (text_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_text_bottom_line)
                
-               289          98 LOAD_FAST                0 (self)
+               322          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (text_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_text_bottom_width)
                
-               291         122 LOAD_FAST                0 (self)
+               324         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -2660,66 +3036,66 @@
                   None
                names      ('text_back', '_text_back', 'text_border', '_text_border', 'text_text_back', '_text_text_back', 'text_bottom_line', '_text_bottom_line', 'text_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_focusout'
-               firstlineno 284
+               firstlineno 317
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               293           0 RESUME                   0
+               326           0 RESUME                   0
                
-               294           2 LOAD_FAST                0 (self)
+               327           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_set)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('focus_set',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_click'
-               firstlineno 293
+               firstlineno 326
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x970064017c005f00000000000000000064005300
-               296           0 RESUME                   0
+               329           0 RESUME                   0
                
-               297           2 LOAD_CONST               1 (True)
+               330           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                   True
                names      ('hover',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_hover'
-               firstlineno 296
+               firstlineno 329
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
@@ -2727,179 +3103,179 @@
                   00ab000000000000000000735a64017c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c006a0a00000000000000007c005f0b00000000000000007c00a0
                   0c00000000000000000000000000000000000000006400a6010000ab0100
                   0000000000000001006400530064005300
-               299           0 RESUME                   0
+               332           0 RESUME                   0
                
-               300           2 LOAD_FAST                0 (self)
+               333           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_get)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_JUMP_FORWARD_IF_TRUE    90 (to 222)
                
-               301          42 LOAD_CONST               1 (False)
+               334          42 LOAD_CONST               1 (False)
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (hover)
                
-               302          56 LOAD_FAST                0 (self)
+               335          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (text_back)
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (_text_back)
                
-               303          80 LOAD_FAST                0 (self)
+               336          80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                4 (text_border)
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               5 (_text_border)
                
-               304         104 LOAD_FAST                0 (self)
+               337         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                6 (text_text_back)
                            116 LOAD_FAST                0 (self)
                            118 STORE_ATTR               7 (_text_text_back)
                
-               305         128 LOAD_FAST                0 (self)
+               338         128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                8 (text_bottom_line)
                            140 LOAD_FAST                0 (self)
                            142 STORE_ATTR               9 (_text_bottom_line)
                
-               306         152 LOAD_FAST                0 (self)
+               339         152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR               10 (text_bottom_width)
                            164 LOAD_FAST                0 (self)
                            166 STORE_ATTR              11 (_text_bottom_width)
                
-               308         176 LOAD_FAST                0 (self)
+               341         176 LOAD_FAST                0 (self)
                            178 LOAD_METHOD             12 (_draw)
                            200 LOAD_CONST               0 (None)
                            202 PRECALL                  1
                            206 CALL                     1
                            216 POP_TOP
                            218 LOAD_CONST               0 (None)
                            220 RETURN_VALUE
                
-               300     >>  222 LOAD_CONST               0 (None)
+               333     >>  222 LOAD_CONST               0 (None)
                            224 RETURN_VALUE
                consts
                   None
                   False
                names      ('focus_get', 'hover', 'text_back', '_text_back', 'text_border', '_text_border', 'text_text_back', '_text_text_back', 'text_bottom_line', '_text_bottom_line', 'text_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_hover_release'
-               firstlineno 299
+               firstlineno 332
                lnotab 0x020128010e01180118011801180118022ef8
             'font'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               310           0 RESUME                   0
+               343           0 RESUME                   0
                
-               311           2 LOAD_FAST                1 (font)
+               344           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               312           6 LOAD_FAST                0 (self)
+               345           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (text_text_font)
                             18 RETURN_VALUE
                
-               314     >>   20 LOAD_FAST                1 (font)
+               347     >>   20 LOAD_FAST                1 (font)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (text_text_font)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('text_text_font',)
                varnames   ('self', 'font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'font'
-               firstlineno 310
+               firstlineno 343
                lnotab 0x020104010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               316           0 RESUME                   0
+               349           0 RESUME                   0
                
-               317           2 LOAD_FAST                0 (self)
+               350           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 316
+               firstlineno 349
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640864066409640a640b640c640d640e9c0ea6
                   010000ab010000000000000000010064005300
-               319           0 RESUME                   0
+               352           0 RESUME                   0
                
-               320           2 LOAD_FAST                0 (self)
+               353           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               322          26 LOAD_CONST               1 (6)
+               355          26 LOAD_CONST               1 (6)
                
-               324          28 LOAD_CONST               2 ((3, 4))
+               357          28 LOAD_CONST               2 ((3, 4))
                
-               326          30 LOAD_CONST               3 ('#f3f3f3')
+               359          30 LOAD_CONST               3 ('#f3f3f3')
                
-               327          32 LOAD_CONST               4 (1)
+               360          32 LOAD_CONST               4 (1)
                
-               328          34 LOAD_CONST               5 (0)
+               361          34 LOAD_CONST               5 (0)
                
-               330          36 LOAD_CONST               6 ('#eaeaea')
+               363          36 LOAD_CONST               6 ('#eaeaea')
                
-               331          38 LOAD_CONST               7 ('#fdfdfd')
+               364          38 LOAD_CONST               7 ('#fdfdfd')
                
-               332          40 LOAD_CONST               8 ('#5f5f5f')
+               365          40 LOAD_CONST               8 ('#5f5f5f')
                
-               333          42 LOAD_CONST               6 ('#eaeaea')
+               366          42 LOAD_CONST               6 ('#eaeaea')
                
-               335          44 LOAD_CONST               9 ('#e2e2e2')
+               368          44 LOAD_CONST               9 ('#e2e2e2')
                
-               336          46 LOAD_CONST              10 ('#f9f9f9')
+               369          46 LOAD_CONST              10 ('#f9f9f9')
                
-               337          48 LOAD_CONST              11 ('#1a1a1a')
+               370          48 LOAD_CONST              11 ('#1a1a1a')
                
-               338          50 LOAD_CONST              12 ('#185fb4')
+               371          50 LOAD_CONST              12 ('#185fb4')
                
-               339          52 LOAD_CONST              13 (2)
+               372          52 LOAD_CONST              13 (2)
                
-               321          54 LOAD_CONST              14 (('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
+               354          54 LOAD_CONST              14 (('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
                             56 BUILD_CONST_KEY_MAP     14
                
-               320          58 PRECALL                  1
+               353          58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
                             74 LOAD_CONST               0 (None)
                             76 RETURN_VALUE
                consts
                   None
                   6
@@ -2918,64 +3294,64 @@
                   ('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette_light'
-               firstlineno 319
+               firstlineno 352
                lnotab
                   0x0201180202020202020102010202020102010201020202010201020102
                   0102ee04ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640864096405640a6408640b640c640d9c0ea6
                   010000ab010000000000000000010064005300
-               343           0 RESUME                   0
+               376           0 RESUME                   0
                
-               344           2 LOAD_FAST                0 (self)
+               377           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               346          26 LOAD_CONST               1 (6)
+               379          26 LOAD_CONST               1 (6)
                
-               348          28 LOAD_CONST               2 ((3, 4))
+               381          28 LOAD_CONST               2 ((3, 4))
                
-               350          30 LOAD_CONST               3 ('#202020')
+               383          30 LOAD_CONST               3 ('#202020')
                
-               351          32 LOAD_CONST               4 (1)
+               384          32 LOAD_CONST               4 (1)
                
-               353          34 LOAD_CONST               5 ('#454545')
+               386          34 LOAD_CONST               5 ('#454545')
                
-               354          36 LOAD_CONST               6 ('#353535')
+               387          36 LOAD_CONST               6 ('#353535')
                
-               355          38 LOAD_CONST               7 ('#cecece')
+               388          38 LOAD_CONST               7 ('#cecece')
                
-               356          40 LOAD_CONST               8 ('#ffffff')
+               389          40 LOAD_CONST               8 ('#ffffff')
                
-               357          42 LOAD_CONST               9 (0)
+               390          42 LOAD_CONST               9 (0)
                
-               359          44 LOAD_CONST               5 ('#454545')
+               392          44 LOAD_CONST               5 ('#454545')
                
-               360          46 LOAD_CONST              10 ('#2f2f2f')
+               393          46 LOAD_CONST              10 ('#2f2f2f')
                
-               361          48 LOAD_CONST               8 ('#ffffff')
+               394          48 LOAD_CONST               8 ('#ffffff')
                
-               362          50 LOAD_CONST              11 ('#4cc2ff')
+               395          50 LOAD_CONST              11 ('#4cc2ff')
                
-               363          52 LOAD_CONST              12 (2)
+               396          52 LOAD_CONST              12 (2)
                
-               345          54 LOAD_CONST              13 (('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
+               378          54 LOAD_CONST              13 (('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
                             56 BUILD_CONST_KEY_MAP     14
                
-               344          58 PRECALL                  1
+               377          58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
                             74 LOAD_CONST               0 (None)
                             76 RETURN_VALUE
                consts
                   None
                   6
@@ -2993,15 +3369,15 @@
                   ('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette_dark'
-               firstlineno 343
+               firstlineno 376
                lnotab
                   0x0201180202020202020102020201020102010201020202010201020102
                   0102ee04ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 11
@@ -3023,160 +3399,160 @@
                   000000000000006400a6010000ab01000000000000000001006400530023
                   00741e000000000000000000002400720401005900640053007700780359
                   0077017c006a0100000000000000007c006a0200000000000000007c006a
                   0300000000000000007c006a0800000000000000007c006a040000000000
                   0000007c006a0500000000000000007c006a0600000000000000007c006a
                   0900000000000000007c006a0a00000000000000007c006a0b0000000000
                   000000640f9c0a5300
-               367           0 RESUME                   0
+               400           0 RESUME                   0
                
-               368           2 LOAD_FAST                1 (dict)
+               401           2 LOAD_FAST                1 (dict)
                              4 POP_JUMP_FORWARD_IF_NONE   223 (to 452)
                
-               369           6 LOAD_FAST                1 (dict)
+               402           6 LOAD_FAST                1 (dict)
                              8 LOAD_CONST               1 ('text_radius')
                             10 BINARY_SUBSCR
                             20 LOAD_FAST                0 (self)
                             22 STORE_ATTR               0 (text_radius)
                
-               371          32 LOAD_FAST                1 (dict)
+               404          32 LOAD_FAST                1 (dict)
                             34 LOAD_CONST               2 ('text_padding')
                             36 BINARY_SUBSCR
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               1 (text_padding)
                
-               373          58 LOAD_FAST                1 (dict)
+               406          58 LOAD_FAST                1 (dict)
                             60 LOAD_CONST               3 ('text_frame_back')
                             62 BINARY_SUBSCR
                             72 LOAD_FAST                0 (self)
                             74 STORE_ATTR               2 (text_frame_back)
                
-               374          84 LOAD_FAST                1 (dict)
+               407          84 LOAD_FAST                1 (dict)
                             86 LOAD_CONST               4 ('text_border_width')
                             88 BINARY_SUBSCR
                             98 LOAD_FAST                0 (self)
                            100 STORE_ATTR               3 (text_border_width)
                
-               376         110 LOAD_FAST                1 (dict)
+               409         110 LOAD_FAST                1 (dict)
                            112 LOAD_CONST               5 ('text_border')
                            114 BINARY_SUBSCR
                            124 LOAD_FAST                0 (self)
                            126 STORE_ATTR               4 (text_border)
                
-               377         136 LOAD_FAST                1 (dict)
+               410         136 LOAD_FAST                1 (dict)
                            138 LOAD_CONST               6 ('text_back')
                            140 BINARY_SUBSCR
                            150 LOAD_FAST                0 (self)
                            152 STORE_ATTR               5 (text_back)
                
-               378         162 LOAD_FAST                1 (dict)
+               411         162 LOAD_FAST                1 (dict)
                            164 LOAD_CONST               7 ('text_text_back')
                            166 BINARY_SUBSCR
                            176 LOAD_FAST                0 (self)
                            178 STORE_ATTR               6 (text_text_back)
                
-               379         188 LOAD_FAST                1 (dict)
+               412         188 LOAD_FAST                1 (dict)
                            190 LOAD_CONST               8 ('text_bottom_line')
                            192 BINARY_SUBSCR
                            202 LOAD_FAST                0 (self)
                            204 STORE_ATTR               7 (text_bottom_line)
                
-               380         214 LOAD_FAST                1 (dict)
+               413         214 LOAD_FAST                1 (dict)
                            216 LOAD_CONST               9 ('text_bottom_width')
                            218 BINARY_SUBSCR
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               8 (text_bottom_width)
                
-               382         240 LOAD_FAST                1 (dict)
+               415         240 LOAD_FAST                1 (dict)
                            242 LOAD_CONST              10 ('text_focusin_border')
                            244 BINARY_SUBSCR
                            254 LOAD_FAST                0 (self)
                            256 STORE_ATTR               9 (text_focusin_border)
                
-               383         266 LOAD_FAST                1 (dict)
+               416         266 LOAD_FAST                1 (dict)
                            268 LOAD_CONST              11 ('text_focusin_back')
                            270 BINARY_SUBSCR
                            280 LOAD_FAST                0 (self)
                            282 STORE_ATTR              10 (text_focusin_back)
                
-               384         292 LOAD_FAST                1 (dict)
+               417         292 LOAD_FAST                1 (dict)
                            294 LOAD_CONST              12 ('text_focusin_text_back')
                            296 BINARY_SUBSCR
                            306 LOAD_FAST                0 (self)
                            308 STORE_ATTR              11 (text_focusin_text_back)
                
-               385         318 LOAD_FAST                1 (dict)
+               418         318 LOAD_FAST                1 (dict)
                            320 LOAD_CONST              13 ('text_focusin_bottom_line')
                            322 BINARY_SUBSCR
                            332 LOAD_FAST                0 (self)
                            334 STORE_ATTR              12 (text_focusin_bottom_line)
                
-               386         344 LOAD_FAST                1 (dict)
+               419         344 LOAD_FAST                1 (dict)
                            346 LOAD_CONST              14 ('text_focusin_bottom_width')
                            348 BINARY_SUBSCR
                            358 LOAD_FAST                0 (self)
                            360 STORE_ATTR              13 (text_focusin_bottom_width)
                
-               388         370 NOP
+               421         370 NOP
                
-               389         372 LOAD_FAST                0 (self)
+               422         372 LOAD_FAST                0 (self)
                            374 LOAD_METHOD             14 (_draw)
                            396 LOAD_CONST               0 (None)
                            398 PRECALL                  1
                            402 CALL                     1
                            412 POP_TOP
                            414 LOAD_CONST               0 (None)
                            416 RETURN_VALUE
                        >>  418 PUSH_EXC_INFO
                
-               390         420 LOAD_GLOBAL             30 (AttributeError)
+               423         420 LOAD_GLOBAL             30 (AttributeError)
                            432 CHECK_EXC_MATCH
                            434 POP_JUMP_FORWARD_IF_FALSE     4 (to 444)
                            436 POP_TOP
                
-               391         438 POP_EXCEPT
+               424         438 POP_EXCEPT
                            440 LOAD_CONST               0 (None)
                            442 RETURN_VALUE
                
-               390     >>  444 RERAISE                  0
+               423     >>  444 RERAISE                  0
                        >>  446 COPY                     3
                            448 POP_EXCEPT
                            450 RERAISE                  1
                
-               394     >>  452 LOAD_FAST                0 (self)
+               427     >>  452 LOAD_FAST                0 (self)
                            454 LOAD_ATTR                1 (text_padding)
                
-               396         464 LOAD_FAST                0 (self)
+               429         464 LOAD_FAST                0 (self)
                            466 LOAD_ATTR                2 (text_frame_back)
                
-               397         476 LOAD_FAST                0 (self)
+               430         476 LOAD_FAST                0 (self)
                            478 LOAD_ATTR                3 (text_border_width)
                
-               398         488 LOAD_FAST                0 (self)
+               431         488 LOAD_FAST                0 (self)
                            490 LOAD_ATTR                8 (text_bottom_width)
                
-               400         500 LOAD_FAST                0 (self)
+               433         500 LOAD_FAST                0 (self)
                            502 LOAD_ATTR                4 (text_border)
                
-               401         512 LOAD_FAST                0 (self)
+               434         512 LOAD_FAST                0 (self)
                            514 LOAD_ATTR                5 (text_back)
                
-               402         524 LOAD_FAST                0 (self)
+               435         524 LOAD_FAST                0 (self)
                            526 LOAD_ATTR                6 (text_text_back)
                
-               404         536 LOAD_FAST                0 (self)
+               437         536 LOAD_FAST                0 (self)
                            538 LOAD_ATTR                9 (text_focusin_border)
                
-               405         548 LOAD_FAST                0 (self)
+               438         548 LOAD_FAST                0 (self)
                            550 LOAD_ATTR               10 (text_focusin_back)
                
-               406         560 LOAD_FAST                0 (self)
+               439         560 LOAD_FAST                0 (self)
                            562 LOAD_ATTR               11 (text_focusin_text_back)
                
-               393         572 LOAD_CONST              15 (('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back'))
+               426         572 LOAD_CONST              15 (('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back'))
                            574 BUILD_CONST_KEY_MAP     10
                            576 RETURN_VALUE
                ExceptionTable:
                  372 to 412 -> 418 [0]
                  418 to 436 -> 446 [1] lasti
                  444 to 444 -> 446 [1] lasti
                consts
@@ -3198,139 +3574,139 @@
                   ('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back')
                names      ('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette'
-               firstlineno 367
+               firstlineno 400
                lnotab
                   0x020104011a021a021a011a021a011a011a011a011a021a011a011a011a
                   011a0202013001120106ff08040c020c010c010c020c010c010c020c010c
                   010cf3
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'float', 'int', 'border_radius', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawBasicRoundText'
-         firstlineno 232
+         firstlineno 265
          lnotab 0x0c010a0306031406061e0809080908030803080b0e06060306180618
       'AdwDrawBasicRoundText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         410           0 RESUME                   0
+         443           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundText')
                        8 STORE_NAME               2 (__qualname__)
          
-         411          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 411>)
+         444          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 444>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               411           0 RESUME                   0
+               444           0 RESUME                   0
                
-               412           2 LOAD_FAST                0 (self)
+               445           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 411
+               firstlineno 444
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawRoundText'
-         firstlineno 410
+         firstlineno 443
          lnotab 0x0a01
       'AdwDrawRoundText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         415           0 RESUME                   0
+         448           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkText')
                        8 STORE_NAME               2 (__qualname__)
          
-         416          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 416>)
+         449          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 449>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkText'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               416           0 RESUME                   0
+               449           0 RESUME                   0
                
-               417           2 LOAD_FAST                0 (self)
+               450           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 416
+               firstlineno 449
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawRoundDarkText'
-         firstlineno 415
+         firstlineno 448
          lnotab 0x0a01
       'AdwDrawRoundDarkText'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
@@ -3338,91 +3714,91 @@
             0x8700970065005a0164005a0288006601640184085a03640284005a0464
             126404650565067a0700006602640584055a07640684005a086412640784
             015a096412640884015a0a6412640984015a0b6412640a84015a0c641264
             0b84015a0d6412640c650e6602640d84055a0f640e84005a10640f84005a
             11641084005a126412641184015a13880078015a145300
                        0 MAKE_CELL                0 (__class__)
          
-         420           2 RESUME                   0
+         453           2 RESUME                   0
                        4 LOAD_NAME                0 (__name__)
                        6 STORE_NAME               1 (__module__)
                        8 LOAD_CONST               0 ('AdwDrawBasicRoundText3')
                       10 STORE_NAME               2 (__qualname__)
          
-         421          12 LOAD_CLOSURE             0 (__class__)
+         454          12 LOAD_CLOSURE             0 (__class__)
                       14 BUILD_TUPLE              1
-                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\textbox.py", line 421>)
+                      16 LOAD_CONST               1 (<code object __init__, file "D:\tkadw\tkadw\canvas\textbox.py", line 454>)
                       18 MAKE_FUNCTION            8 (closure)
                       20 STORE_NAME               3 (__init__)
          
-         424          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\textbox.py", line 424>)
+         457          22 LOAD_CONST               2 (<code object _other, file "D:\tkadw\tkadw\canvas\textbox.py", line 457>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               4 (_other)
          
-         427          28 LOAD_CONST              18 ((None,))
+         460          28 LOAD_CONST              18 ((None,))
                       30 LOAD_CONST               4 ('radius')
                       32 LOAD_NAME                5 (float)
                       34 LOAD_NAME                6 (int)
                       36 BINARY_OP                7 (|)
                       40 BUILD_TUPLE              2
-                      42 LOAD_CONST               5 (<code object border_radius, file "D:\tkadw\tkadw\canvas\textbox.py", line 427>)
+                      42 LOAD_CONST               5 (<code object border_radius, file "D:\tkadw\tkadw\canvas\textbox.py", line 460>)
                       44 MAKE_FUNCTION            5 (defaults, annotations)
                       46 STORE_NAME               7 (border_radius)
          
-         433          48 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\canvas\textbox.py", line 433>)
+         466          48 LOAD_CONST               6 (<code object _draw, file "D:\tkadw\tkadw\canvas\textbox.py", line 466>)
                       50 MAKE_FUNCTION            0
                       52 STORE_NAME               8 (_draw)
          
-         469          54 LOAD_CONST              18 ((None,))
-                      56 LOAD_CONST               7 (<code object _focus, file "D:\tkadw\tkadw\canvas\textbox.py", line 469>)
+         502          54 LOAD_CONST              18 ((None,))
+                      56 LOAD_CONST               7 (<code object _focus, file "D:\tkadw\tkadw\canvas\textbox.py", line 502>)
                       58 MAKE_FUNCTION            1 (defaults)
                       60 STORE_NAME               9 (_focus)
          
-         478          62 LOAD_CONST              18 ((None,))
-                      64 LOAD_CONST               8 (<code object _focusout, file "D:\tkadw\tkadw\canvas\textbox.py", line 478>)
+         511          62 LOAD_CONST              18 ((None,))
+                      64 LOAD_CONST               8 (<code object _focusout, file "D:\tkadw\tkadw\canvas\textbox.py", line 511>)
                       66 MAKE_FUNCTION            1 (defaults)
                       68 STORE_NAME              10 (_focusout)
          
-         487          70 LOAD_CONST              18 ((None,))
-                      72 LOAD_CONST               9 (<code object _click, file "D:\tkadw\tkadw\canvas\textbox.py", line 487>)
+         520          70 LOAD_CONST              18 ((None,))
+                      72 LOAD_CONST               9 (<code object _click, file "D:\tkadw\tkadw\canvas\textbox.py", line 520>)
                       74 MAKE_FUNCTION            1 (defaults)
                       76 STORE_NAME              11 (_click)
          
-         490          78 LOAD_CONST              18 ((None,))
-                      80 LOAD_CONST              10 (<code object _hover, file "D:\tkadw\tkadw\canvas\textbox.py", line 490>)
+         523          78 LOAD_CONST              18 ((None,))
+                      80 LOAD_CONST              10 (<code object _hover, file "D:\tkadw\tkadw\canvas\textbox.py", line 523>)
                       82 MAKE_FUNCTION            1 (defaults)
                       84 STORE_NAME              12 (_hover)
          
-         493          86 LOAD_CONST              18 ((None,))
-                      88 LOAD_CONST              11 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\textbox.py", line 493>)
+         526          86 LOAD_CONST              18 ((None,))
+                      88 LOAD_CONST              11 (<code object _hover_release, file "D:\tkadw\tkadw\canvas\textbox.py", line 526>)
                       90 MAKE_FUNCTION            1 (defaults)
                       92 STORE_NAME              13 (_hover_release)
          
-         504          94 LOAD_CONST              18 ((None,))
+         537          94 LOAD_CONST              18 ((None,))
                       96 LOAD_CONST              12 ('font')
                       98 LOAD_NAME               14 (Font)
                      100 BUILD_TUPLE              2
-                     102 LOAD_CONST              13 (<code object font, file "D:\tkadw\tkadw\canvas\textbox.py", line 504>)
+                     102 LOAD_CONST              13 (<code object font, file "D:\tkadw\tkadw\canvas\textbox.py", line 537>)
                      104 MAKE_FUNCTION            5 (defaults, annotations)
                      106 STORE_NAME              15 (font)
          
-         510         108 LOAD_CONST              14 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 510>)
+         543         108 LOAD_CONST              14 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 543>)
                      110 MAKE_FUNCTION            0
                      112 STORE_NAME              16 (default_palette)
          
-         513         114 LOAD_CONST              15 (<code object palette_light, file "D:\tkadw\tkadw\canvas\textbox.py", line 513>)
+         546         114 LOAD_CONST              15 (<code object palette_light, file "D:\tkadw\tkadw\canvas\textbox.py", line 546>)
                      116 MAKE_FUNCTION            0
                      118 STORE_NAME              17 (palette_light)
          
-         537         120 LOAD_CONST              16 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\textbox.py", line 537>)
+         570         120 LOAD_CONST              16 (<code object palette_dark, file "D:\tkadw\tkadw\canvas\textbox.py", line 570>)
                      122 MAKE_FUNCTION            0
                      124 STORE_NAME              18 (palette_dark)
          
-         561         126 LOAD_CONST              18 ((None,))
-                     128 LOAD_CONST              17 (<code object palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 561>)
+         594         126 LOAD_CONST              18 ((None,))
+                     128 LOAD_CONST              17 (<code object palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 594>)
                      130 MAKE_FUNCTION            1 (defaults)
                      132 STORE_NAME              19 (palette)
                      134 LOAD_CLOSURE             0 (__class__)
                      136 COPY                     1
                      138 STORE_NAME              20 (__classcell__)
                      140 RETURN_VALUE
          consts
@@ -3433,17 +3809,17 @@
                stacksize : 5
                flags     : 15
                code
                   0x950197000200740100000000000000000000a6000000ab000000000000
                   0000006a0100000000000000007c0169007c02a4018e01010064005300
                              0 COPY_FREE_VARS           1
                
-               421           2 RESUME                   0
+               454           2 RESUME                   0
                
-               422           4 PUSH_NULL
+               455           4 PUSH_NULL
                              6 LOAD_GLOBAL              1 (NULL + super)
                             18 PRECALL                  0
                             22 CALL                     0
                             32 LOAD_ATTR                1 (__init__)
                             42 LOAD_FAST                1 (args)
                             44 BUILD_MAP                0
                             46 LOAD_FAST                2 (kwargs)
@@ -3456,29 +3832,29 @@
                   None
                names      ('super', '__init__')
                varnames   ('self', 'args', 'kwargs')
                freevars   ('__class__',)
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '__init__'
-               firstlineno 421
+               firstlineno 454
                lnotab 0x0401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
                flags     : 3
                code
                   0x97007c00a00000000000000000000000000000000000000000007c006a
                   010000000000000000a00200000000000000000000000000000000000000
                   006401a6010000ab0100000000000000006402ac03a6020000ab02000000
                   0000000000010064005300
-               424           0 RESUME                   0
+               457           0 RESUME                   0
                
-               425           2 LOAD_FAST                0 (self)
+               458           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (configure)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (master)
                             38 LOAD_METHOD              2 (cget)
                             60 LOAD_CONST               1 ('bg')
                             62 PRECALL                  1
                             66 CALL                     1
@@ -3496,49 +3872,49 @@
                   ('background', 'borderwidth')
                names      ('configure', 'master', 'cget')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_other'
-               firstlineno 424
+               firstlineno 457
                lnotab 0x0201
             None
             'radius'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               427           0 RESUME                   0
+               460           0 RESUME                   0
                
-               428           2 LOAD_FAST                1 (radius)
+               461           2 LOAD_FAST                1 (radius)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               429           6 LOAD_FAST                0 (self)
+               462           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (button_radius)
                             18 RETURN_VALUE
                
-               431     >>   20 LOAD_FAST                1 (radius)
+               464     >>   20 LOAD_FAST                1 (radius)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (button_radius)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('button_radius',)
                varnames   ('self', 'radius')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'border_radius'
-               firstlineno 427
+               firstlineno 460
                lnotab 0x020104010e02
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 10
                flags     : 3
                code
@@ -3574,195 +3950,195 @@
                   00000000000000000000000000000000007c006a100000000000000000a6
                   010000ab01000000000000000001007c00a0110000000000000000000000
                   0000000000000000007c006a1000000000000000007c006a0c0000000000
                   000000a6020000ab02000000000000000001007c006a0b00000000000000
                   00a01200000000000000000000000000000000000000007c006a07000000
                   00000000007c006a1300000000000000007c006a130000000000000000ac
                   0aa6030000ab030000000000000000010064005300
-               433           0 RESUME                   0
+               466           0 RESUME                   0
                
-               434           2 LOAD_FAST                0 (self)
+               467           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (delete)
                             26 LOAD_CONST               1 ('all')
                             28 PRECALL                  1
                             32 CALL                     1
                             42 POP_TOP
                
-               436          44 LOAD_FAST                0 (self)
+               469          44 LOAD_FAST                0 (self)
                             46 LOAD_METHOD              1 (create_round_rect4)
                
-               437          68 LOAD_CONST               2 (0)
+               470          68 LOAD_CONST               2 (0)
                
-               438          70 LOAD_CONST               2 (0)
+               471          70 LOAD_CONST               2 (0)
                
-               439          72 LOAD_FAST                0 (self)
+               472          72 LOAD_FAST                0 (self)
                             74 LOAD_METHOD              2 (winfo_width)
                             96 PRECALL                  0
                            100 CALL                     0
                            110 LOAD_CONST               3 (1)
                            112 BINARY_OP               10 (-)
                
-               440         116 LOAD_FAST                0 (self)
+               473         116 LOAD_FAST                0 (self)
                            118 LOAD_METHOD              3 (winfo_height)
                            140 PRECALL                  0
                            144 CALL                     0
                            154 LOAD_CONST               3 (1)
                            156 BINARY_OP               10 (-)
                
-               441         160 LOAD_FAST                0 (self)
+               474         160 LOAD_FAST                0 (self)
                            162 LOAD_ATTR                4 (text_radius)
                
-               442         172 LOAD_FAST                0 (self)
+               475         172 LOAD_FAST                0 (self)
                            174 LOAD_ATTR                5 (text_border_width)
                
-               443         184 LOAD_FAST                0 (self)
+               476         184 LOAD_FAST                0 (self)
                            186 LOAD_ATTR                6 (_text_border)
                            196 LOAD_FAST                0 (self)
                            198 LOAD_ATTR                7 (_text_back)
                
-               436         208 KW_NAMES                 4
+               469         208 KW_NAMES                 4
                            210 PRECALL                  8
                            214 CALL                     8
                            224 POP_TOP
                
-               446         226 LOAD_CONST               5 ('button_frame')
+               479         226 LOAD_CONST               5 ('button_frame')
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               8 (text_frame)
                
-               448         240 LOAD_FAST                0 (self)
+               481         240 LOAD_FAST                0 (self)
                            242 LOAD_METHOD              9 (create_window)
                
-               449         264 LOAD_FAST                0 (self)
+               482         264 LOAD_FAST                0 (self)
                            266 LOAD_METHOD              2 (winfo_width)
                            288 PRECALL                  0
                            292 CALL                     0
                            302 LOAD_CONST               6 (2)
                            304 BINARY_OP               11 (/)
                            308 LOAD_FAST                0 (self)
                            310 LOAD_METHOD              3 (winfo_height)
                            332 PRECALL                  0
                            336 CALL                     0
                            346 LOAD_CONST               6 (2)
                            348 BINARY_OP               11 (/)
                
-               450         352 LOAD_FAST                0 (self)
+               483         352 LOAD_FAST                0 (self)
                            354 LOAD_METHOD              2 (winfo_width)
                            376 PRECALL                  0
                            380 CALL                     0
                            390 LOAD_FAST                0 (self)
                            392 LOAD_ATTR                5 (text_border_width)
                            402 BINARY_OP               10 (-)
                            406 LOAD_FAST                0 (self)
                            408 LOAD_ATTR               10 (text_padding)
                            418 LOAD_CONST               2 (0)
                            420 BINARY_SUBSCR
                            430 BINARY_OP               10 (-)
                            434 LOAD_CONST               6 (2)
                            436 BINARY_OP               10 (-)
                
-               451         440 LOAD_FAST                0 (self)
+               484         440 LOAD_FAST                0 (self)
                            442 LOAD_METHOD              3 (winfo_height)
                            464 PRECALL                  0
                            468 CALL                     0
                            478 LOAD_FAST                0 (self)
                            480 LOAD_ATTR                5 (text_border_width)
                            490 BINARY_OP               10 (-)
                            494 LOAD_FAST                0 (self)
                            496 LOAD_ATTR               10 (text_padding)
                            506 LOAD_CONST               3 (1)
                            508 BINARY_SUBSCR
                            518 BINARY_OP               10 (-)
                            522 LOAD_CONST               6 (2)
                            524 BINARY_OP               10 (-)
                
-               452         528 LOAD_FAST                0 (self)
+               485         528 LOAD_FAST                0 (self)
                            530 LOAD_ATTR               11 (text)
                
-               448         540 KW_NAMES                 7
+               481         540 KW_NAMES                 7
                            542 PRECALL                  5
                            546 CALL                     5
                            556 LOAD_FAST                0 (self)
                            558 STORE_ATTR              12 (text_text)
                
-               455         568 LOAD_FAST                0 (self)
+               488         568 LOAD_FAST                0 (self)
                            570 LOAD_METHOD             13 (create_rectangle)
                            592 LOAD_CONST               3 (1)
                            594 LOAD_FAST                0 (self)
                            596 LOAD_ATTR                4 (text_radius)
                            606 LOAD_CONST               8 (5)
                            608 BINARY_OP               11 (/)
                            612 BINARY_OP                0 (+)
                
-               456         616 LOAD_FAST                0 (self)
+               489         616 LOAD_FAST                0 (self)
                            618 LOAD_METHOD              3 (winfo_height)
                            640 PRECALL                  0
                            644 CALL                     0
                            654 LOAD_FAST                0 (self)
                            656 LOAD_ATTR               14 (_text_bottom_width)
                            666 BINARY_OP               10 (-)
                            670 LOAD_CONST               3 (1)
                            672 BINARY_OP               10 (-)
                
-               457         676 LOAD_FAST                0 (self)
+               490         676 LOAD_FAST                0 (self)
                            678 LOAD_METHOD              2 (winfo_width)
                            700 PRECALL                  0
                            704 CALL                     0
                            714 LOAD_CONST               3 (1)
                            716 BINARY_OP               10 (-)
                            720 LOAD_FAST                0 (self)
                            722 LOAD_ATTR                4 (text_radius)
                            732 LOAD_CONST               8 (5)
                            734 BINARY_OP               11 (/)
                            738 BINARY_OP               10 (-)
                
-               458         742 LOAD_FAST                0 (self)
+               491         742 LOAD_FAST                0 (self)
                            744 LOAD_METHOD              3 (winfo_height)
                            766 PRECALL                  0
                            770 CALL                     0
                            780 LOAD_CONST               3 (1)
                            782 BINARY_OP               10 (-)
                
-               459         786 LOAD_FAST                0 (self)
+               492         786 LOAD_FAST                0 (self)
                            788 LOAD_ATTR               15 (_text_bottom_line)
                            798 LOAD_FAST                0 (self)
                            800 LOAD_ATTR               15 (_text_bottom_line)
                
-               460         810 LOAD_CONST               2 (0)
+               493         810 LOAD_CONST               2 (0)
                
-               455         812 KW_NAMES                 9
+               488         812 KW_NAMES                 9
                            814 PRECALL                  7
                            818 CALL                     7
                            828 LOAD_FAST                0 (self)
                            830 STORE_ATTR              16 (text_bottom)
                
-               462         840 LOAD_FAST                0 (self)
+               495         840 LOAD_FAST                0 (self)
                            842 LOAD_ATTR               14 (_text_bottom_width)
                            852 LOAD_CONST               2 (0)
                            854 COMPARE_OP               2 (==)
                            860 POP_JUMP_FORWARD_IF_FALSE    26 (to 914)
                
-               463         862 LOAD_FAST                0 (self)
+               496         862 LOAD_FAST                0 (self)
                            864 LOAD_METHOD              0 (delete)
                            886 LOAD_FAST                0 (self)
                            888 LOAD_ATTR               16 (text_bottom)
                            898 PRECALL                  1
                            902 CALL                     1
                            912 POP_TOP
                
-               465     >>  914 LOAD_FAST                0 (self)
+               498     >>  914 LOAD_FAST                0 (self)
                            916 LOAD_METHOD             17 (tag_raise)
                            938 LOAD_FAST                0 (self)
                            940 LOAD_ATTR               16 (text_bottom)
                            950 LOAD_FAST                0 (self)
                            952 LOAD_ATTR               12 (text_text)
                            962 PRECALL                  2
                            966 CALL                     2
                            976 POP_TOP
                
-               467         978 LOAD_FAST                0 (self)
+               500         978 LOAD_FAST                0 (self)
                            980 LOAD_ATTR               11 (text)
                            990 LOAD_METHOD             18 (configure)
                           1012 LOAD_FAST                0 (self)
                           1014 LOAD_ATTR                7 (_text_back)
                           1024 LOAD_FAST                0 (self)
                           1026 LOAD_ATTR               19 (_text_text_back)
                           1036 LOAD_FAST                0 (self)
@@ -3787,15 +4163,15 @@
                   ('background', 'foreground', 'insertbackground')
                names      ('delete', 'create_round_rect4', 'winfo_width', 'winfo_height', 'text_radius', 'text_border_width', '_text_border', '_text_back', 'text_frame', 'create_window', 'text_padding', 'text', 'text_text', 'create_rectangle', '_text_bottom_width', '_text_bottom_line', 'text_bottom', 'tag_raise', 'configure', '_text_text_back')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_draw'
-               firstlineno 433
+               firstlineno 466
                lnotab
                   0x02012a021801020102012c012c010c010c0118f9120a0e021801580158
                   0158010cfc1c0730013c0142012c01180102fb1c07160134024002
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
@@ -3803,42 +4179,42 @@
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               469           0 RESUME                   0
+               502           0 RESUME                   0
                
-               470           2 LOAD_FAST                0 (self)
+               503           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (text_focusin_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_text_back)
                
-               471          26 LOAD_FAST                0 (self)
+               504          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (text_focusin_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_text_border)
                
-               472          50 LOAD_FAST                0 (self)
+               505          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (text_focusin_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_text_text_back)
                
-               473          74 LOAD_FAST                0 (self)
+               506          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (text_focusin_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_text_bottom_line)
                
-               474          98 LOAD_FAST                0 (self)
+               507          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (text_focusin_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_text_bottom_width)
                
-               476         122 LOAD_FAST                0 (self)
+               509         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -3846,56 +4222,56 @@
                   None
                names      ('text_focusin_back', '_text_back', 'text_focusin_border', '_text_border', 'text_focusin_text_back', '_text_text_back', 'text_focusin_bottom_line', '_text_bottom_line', 'text_focusin_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_focus'
-               firstlineno 469
+               firstlineno 502
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007c006a0000000000000000007c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c00a00a00000000000000000000000000000000000000006400a6
                   010000ab010000000000000000010064005300
-               478           0 RESUME                   0
+               511           0 RESUME                   0
                
-               479           2 LOAD_FAST                0 (self)
+               512           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (text_back)
                             14 LOAD_FAST                0 (self)
                             16 STORE_ATTR               1 (_text_back)
                
-               480          26 LOAD_FAST                0 (self)
+               513          26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                2 (text_border)
                             38 LOAD_FAST                0 (self)
                             40 STORE_ATTR               3 (_text_border)
                
-               481          50 LOAD_FAST                0 (self)
+               514          50 LOAD_FAST                0 (self)
                             52 LOAD_ATTR                4 (text_text_back)
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               5 (_text_text_back)
                
-               482          74 LOAD_FAST                0 (self)
+               515          74 LOAD_FAST                0 (self)
                             76 LOAD_ATTR                6 (text_bottom_line)
                             86 LOAD_FAST                0 (self)
                             88 STORE_ATTR               7 (_text_bottom_line)
                
-               483          98 LOAD_FAST                0 (self)
+               516          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                8 (text_bottom_width)
                            110 LOAD_FAST                0 (self)
                            112 STORE_ATTR               9 (_text_bottom_width)
                
-               485         122 LOAD_FAST                0 (self)
+               518         122 LOAD_FAST                0 (self)
                            124 LOAD_METHOD             10 (_draw)
                            146 LOAD_CONST               0 (None)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 POP_TOP
                            164 LOAD_CONST               0 (None)
                            166 RETURN_VALUE
@@ -3903,66 +4279,66 @@
                   None
                names      ('text_back', '_text_back', 'text_border', '_text_border', 'text_text_back', '_text_text_back', 'text_bottom_line', '_text_bottom_line', 'text_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_focusout'
-               firstlineno 478
+               firstlineno 511
                lnotab 0x020118011801180118011802
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               487           0 RESUME                   0
+               520           0 RESUME                   0
                
-               488           2 LOAD_FAST                0 (self)
+               521           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_set)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('focus_set',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_click'
-               firstlineno 487
+               firstlineno 520
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code 0x970064017c005f00000000000000000064005300
-               490           0 RESUME                   0
+               523           0 RESUME                   0
                
-               491           2 LOAD_CONST               1 (True)
+               524           2 LOAD_CONST               1 (True)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (hover)
                             16 LOAD_CONST               0 (None)
                             18 RETURN_VALUE
                consts
                   None
                   True
                names      ('hover',)
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_hover'
-               firstlineno 490
+               firstlineno 523
                lnotab 0x0201
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
@@ -3970,179 +4346,179 @@
                   00ab000000000000000000735a64017c005f0100000000000000007c006a
                   0200000000000000007c005f0300000000000000007c006a040000000000
                   0000007c005f0500000000000000007c006a0600000000000000007c005f
                   0700000000000000007c006a0800000000000000007c005f090000000000
                   0000007c006a0a00000000000000007c005f0b00000000000000007c00a0
                   0c00000000000000000000000000000000000000006400a6010000ab0100
                   0000000000000001006400530064005300
-               493           0 RESUME                   0
+               526           0 RESUME                   0
                
-               494           2 LOAD_FAST                0 (self)
+               527           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (focus_get)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_JUMP_FORWARD_IF_TRUE    90 (to 222)
                
-               495          42 LOAD_CONST               1 (False)
+               528          42 LOAD_CONST               1 (False)
                             44 LOAD_FAST                0 (self)
                             46 STORE_ATTR               1 (hover)
                
-               496          56 LOAD_FAST                0 (self)
+               529          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (text_back)
                             68 LOAD_FAST                0 (self)
                             70 STORE_ATTR               3 (_text_back)
                
-               497          80 LOAD_FAST                0 (self)
+               530          80 LOAD_FAST                0 (self)
                             82 LOAD_ATTR                4 (text_border)
                             92 LOAD_FAST                0 (self)
                             94 STORE_ATTR               5 (_text_border)
                
-               498         104 LOAD_FAST                0 (self)
+               531         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                6 (text_text_back)
                            116 LOAD_FAST                0 (self)
                            118 STORE_ATTR               7 (_text_text_back)
                
-               499         128 LOAD_FAST                0 (self)
+               532         128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                8 (text_bottom_line)
                            140 LOAD_FAST                0 (self)
                            142 STORE_ATTR               9 (_text_bottom_line)
                
-               500         152 LOAD_FAST                0 (self)
+               533         152 LOAD_FAST                0 (self)
                            154 LOAD_ATTR               10 (text_bottom_width)
                            164 LOAD_FAST                0 (self)
                            166 STORE_ATTR              11 (_text_bottom_width)
                
-               502         176 LOAD_FAST                0 (self)
+               535         176 LOAD_FAST                0 (self)
                            178 LOAD_METHOD             12 (_draw)
                            200 LOAD_CONST               0 (None)
                            202 PRECALL                  1
                            206 CALL                     1
                            216 POP_TOP
                            218 LOAD_CONST               0 (None)
                            220 RETURN_VALUE
                
-               494     >>  222 LOAD_CONST               0 (None)
+               527     >>  222 LOAD_CONST               0 (None)
                            224 RETURN_VALUE
                consts
                   None
                   False
                names      ('focus_get', 'hover', 'text_back', '_text_back', 'text_border', '_text_border', 'text_text_back', '_text_text_back', 'text_bottom_line', '_text_bottom_line', 'text_bottom_width', '_text_bottom_width', '_draw')
                varnames   ('self', 'evt')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       '_hover_release'
-               firstlineno 493
+               firstlineno 526
                lnotab 0x020128010e01180118011801180118022ef8
             'font'
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c0180077c006a00000000000000000053007c017c005f00000000
                   000000000064005300
-               504           0 RESUME                   0
+               537           0 RESUME                   0
                
-               505           2 LOAD_FAST                1 (font)
+               538           2 LOAD_FAST                1 (font)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               506           6 LOAD_FAST                0 (self)
+               539           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (text_text_font)
                             18 RETURN_VALUE
                
-               508     >>   20 LOAD_FAST                1 (font)
+               541     >>   20 LOAD_FAST                1 (font)
                             22 LOAD_FAST                0 (self)
                             24 STORE_ATTR               0 (text_text_font)
                             34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                consts
                   None
                names      ('text_text_font',)
                varnames   ('self', 'font')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'font'
-               firstlineno 504
+               firstlineno 537
                lnotab 0x020104010e02
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               510           0 RESUME                   0
+               543           0 RESUME                   0
                
-               511           2 LOAD_FAST                0 (self)
+               544           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 510
+               firstlineno 543
                lnotab 0x0201
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640864066409640a640b640c640d640e9c0ea6
                   010000ab010000000000000000010064005300
-               513           0 RESUME                   0
+               546           0 RESUME                   0
                
-               514           2 LOAD_FAST                0 (self)
+               547           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               516          26 LOAD_CONST               1 (13)
+               549          26 LOAD_CONST               1 (13)
                
-               518          28 LOAD_CONST               2 ((6, 4))
+               551          28 LOAD_CONST               2 ((6, 4))
                
-               520          30 LOAD_CONST               3 ('#f3f3f3')
+               553          30 LOAD_CONST               3 ('#f3f3f3')
                
-               521          32 LOAD_CONST               4 (1)
+               554          32 LOAD_CONST               4 (1)
                
-               522          34 LOAD_CONST               5 (0)
+               555          34 LOAD_CONST               5 (0)
                
-               524          36 LOAD_CONST               6 ('#eaeaea')
+               557          36 LOAD_CONST               6 ('#eaeaea')
                
-               525          38 LOAD_CONST               7 ('#fdfdfd')
+               558          38 LOAD_CONST               7 ('#fdfdfd')
                
-               526          40 LOAD_CONST               8 ('#5f5f5f')
+               559          40 LOAD_CONST               8 ('#5f5f5f')
                
-               527          42 LOAD_CONST               6 ('#eaeaea')
+               560          42 LOAD_CONST               6 ('#eaeaea')
                
-               529          44 LOAD_CONST               9 ('#e2e2e2')
+               562          44 LOAD_CONST               9 ('#e2e2e2')
                
-               530          46 LOAD_CONST              10 ('#f9f9f9')
+               563          46 LOAD_CONST              10 ('#f9f9f9')
                
-               531          48 LOAD_CONST              11 ('#1a1a1a')
+               564          48 LOAD_CONST              11 ('#1a1a1a')
                
-               532          50 LOAD_CONST              12 ('#185fb4')
+               565          50 LOAD_CONST              12 ('#185fb4')
                
-               533          52 LOAD_CONST              13 (2)
+               566          52 LOAD_CONST              13 (2)
                
-               515          54 LOAD_CONST              14 (('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
+               548          54 LOAD_CONST              14 (('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
                             56 BUILD_CONST_KEY_MAP     14
                
-               514          58 PRECALL                  1
+               547          58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
                             74 LOAD_CONST               0 (None)
                             76 RETURN_VALUE
                consts
                   None
                   13
@@ -4161,64 +4537,64 @@
                   ('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette_light'
-               firstlineno 513
+               firstlineno 546
                lnotab
                   0x0201180202020202020102010202020102010201020202010201020102
                   0102ee04ff
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 17
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000640164
                   0264036404640564066407640864096405640a6408640b640c640d9c0ea6
                   010000ab010000000000000000010064005300
-               537           0 RESUME                   0
+               570           0 RESUME                   0
                
-               538           2 LOAD_FAST                0 (self)
+               571           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette)
                
-               540          26 LOAD_CONST               1 (13)
+               573          26 LOAD_CONST               1 (13)
                
-               542          28 LOAD_CONST               2 ((3, 4))
+               575          28 LOAD_CONST               2 ((3, 4))
                
-               544          30 LOAD_CONST               3 ('#202020')
+               577          30 LOAD_CONST               3 ('#202020')
                
-               545          32 LOAD_CONST               4 (1)
+               578          32 LOAD_CONST               4 (1)
                
-               547          34 LOAD_CONST               5 ('#454545')
+               580          34 LOAD_CONST               5 ('#454545')
                
-               548          36 LOAD_CONST               6 ('#353535')
+               581          36 LOAD_CONST               6 ('#353535')
                
-               549          38 LOAD_CONST               7 ('#cecece')
+               582          38 LOAD_CONST               7 ('#cecece')
                
-               550          40 LOAD_CONST               8 ('#ffffff')
+               583          40 LOAD_CONST               8 ('#ffffff')
                
-               551          42 LOAD_CONST               9 (0)
+               584          42 LOAD_CONST               9 (0)
                
-               553          44 LOAD_CONST               5 ('#454545')
+               586          44 LOAD_CONST               5 ('#454545')
                
-               554          46 LOAD_CONST              10 ('#2f2f2f')
+               587          46 LOAD_CONST              10 ('#2f2f2f')
                
-               555          48 LOAD_CONST               8 ('#ffffff')
+               588          48 LOAD_CONST               8 ('#ffffff')
                
-               556          50 LOAD_CONST              11 ('#4cc2ff')
+               589          50 LOAD_CONST              11 ('#4cc2ff')
                
-               557          52 LOAD_CONST              12 (2)
+               590          52 LOAD_CONST              12 (2)
                
-               539          54 LOAD_CONST              13 (('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
+               572          54 LOAD_CONST              13 (('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width'))
                             56 BUILD_CONST_KEY_MAP     14
                
-               538          58 PRECALL                  1
+               571          58 PRECALL                  1
                             62 CALL                     1
                             72 POP_TOP
                             74 LOAD_CONST               0 (None)
                             76 RETURN_VALUE
                consts
                   None
                   13
@@ -4236,15 +4612,15 @@
                   ('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width')
                names      ('palette',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette_dark'
-               firstlineno 537
+               firstlineno 570
                lnotab
                   0x0201180202020202020102020201020102010201020202010201020102
                   0102ee04ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 11
@@ -4266,160 +4642,160 @@
                   000000000000006400a6010000ab01000000000000000001006400530023
                   00741e000000000000000000002400720401005900640053007700780359
                   0077017c006a0100000000000000007c006a0200000000000000007c006a
                   0300000000000000007c006a0800000000000000007c006a040000000000
                   0000007c006a0500000000000000007c006a0600000000000000007c006a
                   0900000000000000007c006a0a00000000000000007c006a0b0000000000
                   000000640f9c0a5300
-               561           0 RESUME                   0
+               594           0 RESUME                   0
                
-               562           2 LOAD_FAST                1 (dict)
+               595           2 LOAD_FAST                1 (dict)
                              4 POP_JUMP_FORWARD_IF_NONE   223 (to 452)
                
-               563           6 LOAD_FAST                1 (dict)
+               596           6 LOAD_FAST                1 (dict)
                              8 LOAD_CONST               1 ('text_radius')
                             10 BINARY_SUBSCR
                             20 LOAD_FAST                0 (self)
                             22 STORE_ATTR               0 (text_radius)
                
-               565          32 LOAD_FAST                1 (dict)
+               598          32 LOAD_FAST                1 (dict)
                             34 LOAD_CONST               2 ('text_padding')
                             36 BINARY_SUBSCR
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               1 (text_padding)
                
-               567          58 LOAD_FAST                1 (dict)
+               600          58 LOAD_FAST                1 (dict)
                             60 LOAD_CONST               3 ('text_frame_back')
                             62 BINARY_SUBSCR
                             72 LOAD_FAST                0 (self)
                             74 STORE_ATTR               2 (text_frame_back)
                
-               568          84 LOAD_FAST                1 (dict)
+               601          84 LOAD_FAST                1 (dict)
                             86 LOAD_CONST               4 ('text_border_width')
                             88 BINARY_SUBSCR
                             98 LOAD_FAST                0 (self)
                            100 STORE_ATTR               3 (text_border_width)
                
-               570         110 LOAD_FAST                1 (dict)
+               603         110 LOAD_FAST                1 (dict)
                            112 LOAD_CONST               5 ('text_border')
                            114 BINARY_SUBSCR
                            124 LOAD_FAST                0 (self)
                            126 STORE_ATTR               4 (text_border)
                
-               571         136 LOAD_FAST                1 (dict)
+               604         136 LOAD_FAST                1 (dict)
                            138 LOAD_CONST               6 ('text_back')
                            140 BINARY_SUBSCR
                            150 LOAD_FAST                0 (self)
                            152 STORE_ATTR               5 (text_back)
                
-               572         162 LOAD_FAST                1 (dict)
+               605         162 LOAD_FAST                1 (dict)
                            164 LOAD_CONST               7 ('text_text_back')
                            166 BINARY_SUBSCR
                            176 LOAD_FAST                0 (self)
                            178 STORE_ATTR               6 (text_text_back)
                
-               573         188 LOAD_FAST                1 (dict)
+               606         188 LOAD_FAST                1 (dict)
                            190 LOAD_CONST               8 ('text_bottom_line')
                            192 BINARY_SUBSCR
                            202 LOAD_FAST                0 (self)
                            204 STORE_ATTR               7 (text_bottom_line)
                
-               574         214 LOAD_FAST                1 (dict)
+               607         214 LOAD_FAST                1 (dict)
                            216 LOAD_CONST               9 ('text_bottom_width')
                            218 BINARY_SUBSCR
                            228 LOAD_FAST                0 (self)
                            230 STORE_ATTR               8 (text_bottom_width)
                
-               576         240 LOAD_FAST                1 (dict)
+               609         240 LOAD_FAST                1 (dict)
                            242 LOAD_CONST              10 ('text_focusin_border')
                            244 BINARY_SUBSCR
                            254 LOAD_FAST                0 (self)
                            256 STORE_ATTR               9 (text_focusin_border)
                
-               577         266 LOAD_FAST                1 (dict)
+               610         266 LOAD_FAST                1 (dict)
                            268 LOAD_CONST              11 ('text_focusin_back')
                            270 BINARY_SUBSCR
                            280 LOAD_FAST                0 (self)
                            282 STORE_ATTR              10 (text_focusin_back)
                
-               578         292 LOAD_FAST                1 (dict)
+               611         292 LOAD_FAST                1 (dict)
                            294 LOAD_CONST              12 ('text_focusin_text_back')
                            296 BINARY_SUBSCR
                            306 LOAD_FAST                0 (self)
                            308 STORE_ATTR              11 (text_focusin_text_back)
                
-               579         318 LOAD_FAST                1 (dict)
+               612         318 LOAD_FAST                1 (dict)
                            320 LOAD_CONST              13 ('text_focusin_bottom_line')
                            322 BINARY_SUBSCR
                            332 LOAD_FAST                0 (self)
                            334 STORE_ATTR              12 (text_focusin_bottom_line)
                
-               580         344 LOAD_FAST                1 (dict)
+               613         344 LOAD_FAST                1 (dict)
                            346 LOAD_CONST              14 ('text_focusin_bottom_width')
                            348 BINARY_SUBSCR
                            358 LOAD_FAST                0 (self)
                            360 STORE_ATTR              13 (text_focusin_bottom_width)
                
-               582         370 NOP
+               615         370 NOP
                
-               583         372 LOAD_FAST                0 (self)
+               616         372 LOAD_FAST                0 (self)
                            374 LOAD_METHOD             14 (_draw)
                            396 LOAD_CONST               0 (None)
                            398 PRECALL                  1
                            402 CALL                     1
                            412 POP_TOP
                            414 LOAD_CONST               0 (None)
                            416 RETURN_VALUE
                        >>  418 PUSH_EXC_INFO
                
-               584         420 LOAD_GLOBAL             30 (AttributeError)
+               617         420 LOAD_GLOBAL             30 (AttributeError)
                            432 CHECK_EXC_MATCH
                            434 POP_JUMP_FORWARD_IF_FALSE     4 (to 444)
                            436 POP_TOP
                
-               585         438 POP_EXCEPT
+               618         438 POP_EXCEPT
                            440 LOAD_CONST               0 (None)
                            442 RETURN_VALUE
                
-               584     >>  444 RERAISE                  0
+               617     >>  444 RERAISE                  0
                        >>  446 COPY                     3
                            448 POP_EXCEPT
                            450 RERAISE                  1
                
-               588     >>  452 LOAD_FAST                0 (self)
+               621     >>  452 LOAD_FAST                0 (self)
                            454 LOAD_ATTR                1 (text_padding)
                
-               590         464 LOAD_FAST                0 (self)
+               623         464 LOAD_FAST                0 (self)
                            466 LOAD_ATTR                2 (text_frame_back)
                
-               591         476 LOAD_FAST                0 (self)
+               624         476 LOAD_FAST                0 (self)
                            478 LOAD_ATTR                3 (text_border_width)
                
-               592         488 LOAD_FAST                0 (self)
+               625         488 LOAD_FAST                0 (self)
                            490 LOAD_ATTR                8 (text_bottom_width)
                
-               594         500 LOAD_FAST                0 (self)
+               627         500 LOAD_FAST                0 (self)
                            502 LOAD_ATTR                4 (text_border)
                
-               595         512 LOAD_FAST                0 (self)
+               628         512 LOAD_FAST                0 (self)
                            514 LOAD_ATTR                5 (text_back)
                
-               596         524 LOAD_FAST                0 (self)
+               629         524 LOAD_FAST                0 (self)
                            526 LOAD_ATTR                6 (text_text_back)
                
-               598         536 LOAD_FAST                0 (self)
+               631         536 LOAD_FAST                0 (self)
                            538 LOAD_ATTR                9 (text_focusin_border)
                
-               599         548 LOAD_FAST                0 (self)
+               632         548 LOAD_FAST                0 (self)
                            550 LOAD_ATTR               10 (text_focusin_back)
                
-               600         560 LOAD_FAST                0 (self)
+               633         560 LOAD_FAST                0 (self)
                            562 LOAD_ATTR               11 (text_focusin_text_back)
                
-               587         572 LOAD_CONST              15 (('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back'))
+               620         572 LOAD_CONST              15 (('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back'))
                            574 BUILD_CONST_KEY_MAP     10
                            576 RETURN_VALUE
                ExceptionTable:
                  372 to 412 -> 418 [0]
                  418 to 436 -> 446 [1] lasti
                  444 to 444 -> 446 [1] lasti
                consts
@@ -4441,139 +4817,139 @@
                   ('text_padding', 'text_frame_back', 'text_border_width', 'text_bottom_width', 'text_border', 'text_back', 'text_text_back', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back')
                names      ('text_radius', 'text_padding', 'text_frame_back', 'text_border_width', 'text_border', 'text_back', 'text_text_back', 'text_bottom_line', 'text_bottom_width', 'text_focusin_border', 'text_focusin_back', 'text_focusin_text_back', 'text_focusin_bottom_line', 'text_focusin_bottom_width', '_draw', 'AttributeError')
                varnames   ('self', 'dict')
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'palette'
-               firstlineno 561
+               firstlineno 594
                lnotab
                   0x020104011a021a021a011a021a011a011a011a011a021a011a011a011a
                   011a0202013001120106ff08040c020c010c010c020c010c010c020c010c
                   010cf3
             (None,)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_other', 'float', 'int', 'border_radius', '_draw', '_focus', '_focusout', '_click', '_hover', '_hover_release', 'Font', 'font', 'default_palette', 'palette_light', 'palette_dark', 'palette', '__classcell__')
          varnames   ()
          freevars   ()
          cellvars   ('__class__',)
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawBasicRoundText3'
-         firstlineno 420
+         firstlineno 453
          lnotab 0x0c010a030603140606240809080908030803080b0e06060306180618
       'AdwDrawBasicRoundText3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         604           0 RESUME                   0
+         637           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundText3')
                        8 STORE_NAME               2 (__qualname__)
          
-         605          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 605>)
+         638          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 638>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundText3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               605           0 RESUME                   0
+               638           0 RESUME                   0
                
-               606           2 LOAD_FAST                0 (self)
+               639           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_light)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_light',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 605
+               firstlineno 638
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawRoundText3'
-         firstlineno 604
+         firstlineno 637
          lnotab 0x0a01
       'AdwDrawRoundText3'
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 1
          flags     : 0
          code 0x970065005a0164005a02640184005a0364025300
-         609           0 RESUME                   0
+         642           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('AdwDrawRoundDarkText3')
                        8 STORE_NAME               2 (__qualname__)
          
-         610          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 610>)
+         643          10 LOAD_CONST               1 (<code object default_palette, file "D:\tkadw\tkadw\canvas\textbox.py", line 643>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (default_palette)
                       16 LOAD_CONST               2 (None)
                       18 RETURN_VALUE
          consts
             'AdwDrawRoundDarkText3'
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c00a0000000000000000000000000000000000000000000a60000
                   00ab000000000000000000010064005300
-               610           0 RESUME                   0
+               643           0 RESUME                   0
                
-               611           2 LOAD_FAST                0 (self)
+               644           2 LOAD_FAST                0 (self)
                              4 LOAD_METHOD              0 (palette_dark)
                             26 PRECALL                  0
                             30 CALL                     0
                             40 POP_TOP
                             42 LOAD_CONST               0 (None)
                             44 RETURN_VALUE
                consts
                   None
                names      ('palette_dark',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
                name       'default_palette'
-               firstlineno 610
+               firstlineno 643
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', 'default_palette')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
          name       'AdwDrawRoundDarkText3'
-         firstlineno 609
+         firstlineno 642
          lnotab 0x0a01
       'AdwDrawRoundDarkText3'
       '__main__'
       ('Tk',)
       'x'
       5
       ('fill', 'padx', 'pady')
@@ -4582,10 +4958,10 @@
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\canvas\\textbox.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020110010c041c7f00581c051c061c7f00331c051c051c7f00391c
+      0x00ff020110010c041c7f00791c051c061c7f00331c051c051c7f00391c
       051c050c010c021402140130021401300214013002140130021401300214
       0130022ce9
```

### Comparing `tkadw-0.1.3/tkadw/canvas/adwite/button.py` & `tkadw-0.1.5/tkadw/canvas/adwite/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/atomize/button.py` & `tkadw-0.1.5/tkadw/canvas/atomize/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/button.py` & `tkadw-0.1.5/tkadw/canvas/button.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/drawengine.py` & `tkadw-0.1.5/tkadw/canvas/drawengine.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/entry.py` & `tkadw-0.1.5/tkadw/canvas/entry.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/fluent/__init__.py` & `tkadw-0.1.5/tkadw/canvas/fluent/__init__.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/frame.py` & `tkadw-0.1.5/tkadw/canvas/frame.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/fun.py` & `tkadw-0.1.5/tkadw/canvas/fun.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/fun2.py` & `tkadw-0.1.5/tkadw/canvas/fun2.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/fun3.py` & `tkadw-0.1.5/tkadw/canvas/fun3.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/fun4.py` & `tkadw-0.1.5/tkadw/canvas/fun4.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/fun5.py` & `tkadw-0.1.5/tkadw/canvas/fun5.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/fun6.py` & `tkadw-0.1.5/tkadw/canvas/fun6.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/poly.tcl` & `tkadw-0.1.5/tkadw/canvas/poly.tcl`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/canvas/textbox.py` & `tkadw-0.1.5/tkadw/canvas/textbox.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,47 @@
         self.text.bind("<Control-z>", lambda event: self.undo(), add="+")
         self.text.bind("<Control-Z>", lambda event: self.undo(), add="+")
         self.text.bind("<Control-Shift-z>", lambda event: self.redo(), add="+")
         self.text.bind("<Control-Shift-Z>", lambda event: self.redo(), add="+")
 
         self._draw(None)
 
+    def tbbox(self, *args, **kwargs):
+        return self.text.bbox(*args, **kwargs)
+
+    def compare(self, *args, **kwargs):
+        return self.text.compare(*args, **kwargs)
+
+    def count(self, *args, **kwargs):
+        return self.text.count(*args, **kwargs)
+
+    def debug(self, *args, **kwargs):
+        return self.text.debug(*args, **kwargs)
+
+    def tdelete(self, *args, **kwargs):
+        return self.text.delete(*args, **kwargs)
+
+    def dump(self, *args, **kwargs):
+        return self.text.dump(*args, **kwargs)
+
+    def get(self, *args, **kwargs):
+        return self.text.get(*args, **kwargs)
+
+    def tindex(self, *args, **kwargs):
+        return self.text.index(*args, **kwargs)
+
+    def tinsert(self, *args, **kwargs):
+        return self.text.insert(*args, **kwargs)
+
+    def search(self, *args, **kwargs):
+        return self.text.search(*args, **kwargs)
+
+    def see(self, *args, **kwargs):
+        return self.text.see(*args, **kwargs)
+
     def undo(self):
         try:
             self.text.edit_undo()
         except:
             pass
 
     def redo(self):
```

### Comparing `tkadw-0.1.3/tkadw/canvas/titlebar.py` & `tkadw-0.1.5/tkadw/canvas/titlebar.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc` & `tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc` & `tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/button.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,36 +1,36 @@
 magic:    0xa70d0d0a
-moddate:  0xa32f9564 (Fri Jun 23 05:37:39 2023 UTC)
-files sz: 3898
+moddate:  0x1b599564 (Fri Jun 23 08:34:35 2023 UTC)
+files sz: 3726
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100020047006402840064036501a60300
       00ab0300000000000000005a02020047006404840064056502a6030000ab
       0300000000000000005a03020047006406840064076502a6030000ab0300
       000000000000005a04020047006408840064096502a6030000ab03000000
-      00000000005a056506640a6b020000000072d96400640b6c076d085a0801
-      0002006508a6000000ab0000000000000000005a096509a00a0000000000
-      000000000000000000000000000000640cac0da6010000ab010000000000
-      0000000100020065036403640e8400ac0fa6020000ab0200000000000000
-      005a0b650ba00c0000000000000000000000000000000000000000641064
-      1164116411ac12a6040000ab040000000000000000010002006503640564
-      138400640cac14a6030000ab0300000000000000005a0d650da00c000000
-      00000000000000000000000000000000006410641164116411ac12a60400
-      00ab040000000000000000010002006504640764158400ac0fa6020000ab
-      0200000000000000005a0e650ea00c000000000000000000000000000000
-      00000000006410641164116411ac12a6040000ab04000000000000000001
-      0002006505640964168400ac0fa6020000ab0200000000000000005a0f65
-      0fa00c000000000000000000000000000000000000000064106411641164
-      11ac12a6040000ab04000000000000000001006509a01000000000000000
-      00000000000000000000000000a6000000ab000000000000000000010064
-      17530064175300
+      00000000005a056506640a6b020000000072e06400640b6c076d085a0801
+      006400640c6c006d095a096d0a5a0a010002006508a6000000ab00000000
+      00000000005a0b650ba00c00000000000000000000000000000000000000
+      00640dac0ea6010000ab010000000000000000010002006509650ba60100
+      00ab0100000000000000005a0d02006502650d6a0d000000000000000064
+      03ac0fa6020000ab0200000000000000005a0e650ea00f00000000000000
+      000000000000000000000000006410641164116411ac12a6040000ab0400
+      000000000000000100650da00f0000000000000000000000000000000000
+      000000641364146415ac16a6030000ab0300000000000000000100020065
+      0a650ba6010000ab0100000000000000005a100200650365106a0d000000
+      00000000006405ac0fa6020000ab0200000000000000005a116511a00f00
+      000000000000000000000000000000000000006410641164116411ac12a6
+      040000ab04000000000000000001006510a00f0000000000000000000000
+      000000000000000000641364146417ac16a6030000ab0300000000000000
+      000100650ba0120000000000000000000000000000000000000000a60000
+      00ab00000000000000000001006418530064185300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('AdwDrawRoundButton3',))
                  6 IMPORT_NAME              0 (tkadw)
                  8 IMPORT_FROM              1 (AdwDrawRoundButton3)
                 10 STORE_NAME               1 (AdwDrawRoundButton3)
@@ -75,132 +75,132 @@
                110 PRECALL                  3
                114 CALL                     3
                124 STORE_NAME               5 (GTkSuggestedButton)
    
    111         126 LOAD_NAME                6 (__name__)
                128 LOAD_CONST              10 ('__main__')
                130 COMPARE_OP               2 (==)
-               136 POP_JUMP_FORWARD_IF_FALSE   217 (to 572)
+               136 POP_JUMP_FORWARD_IF_FALSE   224 (to 586)
    
    112         138 LOAD_CONST               0 (0)
                140 LOAD_CONST              11 (('Tk',))
                142 IMPORT_NAME              7 (tkinter)
                144 IMPORT_FROM              8 (Tk)
                146 STORE_NAME               8 (Tk)
                148 POP_TOP
    
-   114         150 PUSH_NULL
-               152 LOAD_NAME                8 (Tk)
-               154 PRECALL                  0
-               158 CALL                     0
-               168 STORE_NAME               9 (root)
-   
-   115         170 LOAD_NAME                9 (root)
-               172 LOAD_METHOD             10 (configure)
-               194 LOAD_CONST              12 ('#1e1e1e')
-               196 KW_NAMES                13
-               198 PRECALL                  1
-               202 CALL                     1
-               212 POP_TOP
-   
-   117         214 PUSH_NULL
-               216 LOAD_NAME                3 (GTkDarkButton)
-               218 LOAD_CONST               3 ('GTkButton')
-               220 LOAD_CONST              14 (<code object <lambda>, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 117>)
-               222 MAKE_FUNCTION            0
-               224 KW_NAMES                15
-               226 PRECALL                  2
-               230 CALL                     2
-               240 STORE_NAME              11 (button)
-   
-   118         242 LOAD_NAME               11 (button)
-               244 LOAD_METHOD             12 (pack)
-               266 LOAD_CONST              16 ('x')
-               268 LOAD_CONST              17 (5)
-               270 LOAD_CONST              17 (5)
-               272 LOAD_CONST              17 (5)
-               274 KW_NAMES                18
-               276 PRECALL                  4
-               280 CALL                     4
-               290 POP_TOP
-   
-   120         292 PUSH_NULL
-               294 LOAD_NAME                3 (GTkDarkButton)
-               296 LOAD_CONST               5 ('GTkDarkButton')
-               298 LOAD_CONST              19 (<code object <lambda>, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 120>)
-               300 MAKE_FUNCTION            0
-               302 LOAD_CONST              12 ('#1e1e1e')
-               304 KW_NAMES                20
-               306 PRECALL                  3
-               310 CALL                     3
-               320 STORE_NAME              13 (button2)
-   
-   121         322 LOAD_NAME               13 (button2)
-               324 LOAD_METHOD             12 (pack)
-               346 LOAD_CONST              16 ('x')
-               348 LOAD_CONST              17 (5)
-               350 LOAD_CONST              17 (5)
-               352 LOAD_CONST              17 (5)
-               354 KW_NAMES                18
-               356 PRECALL                  4
-               360 CALL                     4
-               370 POP_TOP
-   
-   123         372 PUSH_NULL
-               374 LOAD_NAME                4 (GTkDestructiveButton)
-               376 LOAD_CONST               7 ('GTkDestructiveButton')
-               378 LOAD_CONST              21 (<code object <lambda>, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 123>)
-               380 MAKE_FUNCTION            0
-               382 KW_NAMES                15
-               384 PRECALL                  2
-               388 CALL                     2
-               398 STORE_NAME              14 (button3)
-   
-   124         400 LOAD_NAME               14 (button3)
-               402 LOAD_METHOD             12 (pack)
-               424 LOAD_CONST              16 ('x')
-               426 LOAD_CONST              17 (5)
-               428 LOAD_CONST              17 (5)
-               430 LOAD_CONST              17 (5)
-               432 KW_NAMES                18
-               434 PRECALL                  4
-               438 CALL                     4
-               448 POP_TOP
-   
-   126         450 PUSH_NULL
-               452 LOAD_NAME                5 (GTkSuggestedButton)
-               454 LOAD_CONST               9 ('GTkSuggestedButton')
-               456 LOAD_CONST              22 (<code object <lambda>, file "D:\tkadw\tkadw\tkite\gtk\button.py", line 126>)
-               458 MAKE_FUNCTION            0
-               460 KW_NAMES                15
-               462 PRECALL                  2
-               466 CALL                     2
-               476 STORE_NAME              15 (button4)
-   
-   127         478 LOAD_NAME               15 (button4)
-               480 LOAD_METHOD             12 (pack)
-               502 LOAD_CONST              16 ('x')
-               504 LOAD_CONST              17 (5)
-               506 LOAD_CONST              17 (5)
-               508 LOAD_CONST              17 (5)
-               510 KW_NAMES                18
-               512 PRECALL                  4
-               516 CALL                     4
-               526 POP_TOP
-   
-   129         528 LOAD_NAME                9 (root)
-               530 LOAD_METHOD             16 (mainloop)
-               552 PRECALL                  0
-               556 CALL                     0
-               566 POP_TOP
-               568 LOAD_CONST              23 (None)
-               570 RETURN_VALUE
+   113         150 LOAD_CONST               0 (0)
+               152 LOAD_CONST              12 (('GTkFrame', 'GTkDarkFrame'))
+               154 IMPORT_NAME              0 (tkadw)
+               156 IMPORT_FROM              9 (GTkFrame)
+               158 STORE_NAME               9 (GTkFrame)
+               160 IMPORT_FROM             10 (GTkDarkFrame)
+               162 STORE_NAME              10 (GTkDarkFrame)
+               164 POP_TOP
+   
+   115         166 PUSH_NULL
+               168 LOAD_NAME                8 (Tk)
+               170 PRECALL                  0
+               174 CALL                     0
+               184 STORE_NAME              11 (root)
+   
+   116         186 LOAD_NAME               11 (root)
+               188 LOAD_METHOD             12 (configure)
+               210 LOAD_CONST              13 ('#1e1e1e')
+               212 KW_NAMES                14
+               214 PRECALL                  1
+               218 CALL                     1
+               228 POP_TOP
+   
+   118         230 PUSH_NULL
+               232 LOAD_NAME                9 (GTkFrame)
+               234 LOAD_NAME               11 (root)
+               236 PRECALL                  1
+               240 CALL                     1
+               250 STORE_NAME              13 (frame)
+   
+   120         252 PUSH_NULL
+               254 LOAD_NAME                2 (GTkButton)
+               256 LOAD_NAME               13 (frame)
+               258 LOAD_ATTR               13 (frame)
+               268 LOAD_CONST               3 ('GTkButton')
+               270 KW_NAMES                15
+               272 PRECALL                  2
+               276 CALL                     2
+               286 STORE_NAME              14 (button1)
+   
+   121         288 LOAD_NAME               14 (button1)
+               290 LOAD_METHOD             15 (pack)
+               312 LOAD_CONST              16 ('x')
+               314 LOAD_CONST              17 (5)
+               316 LOAD_CONST              17 (5)
+               318 LOAD_CONST              17 (5)
+               320 KW_NAMES                18
+               322 PRECALL                  4
+               326 CALL                     4
+               336 POP_TOP
+   
+   123         338 LOAD_NAME               13 (frame)
+               340 LOAD_METHOD             15 (pack)
+               362 LOAD_CONST              19 ('both')
+               364 LOAD_CONST              20 ('yes')
+               366 LOAD_CONST              21 ('right')
+               368 KW_NAMES                22
+               370 PRECALL                  3
+               374 CALL                     3
+               384 POP_TOP
+   
+   125         386 PUSH_NULL
+               388 LOAD_NAME               10 (GTkDarkFrame)
+               390 LOAD_NAME               11 (root)
+               392 PRECALL                  1
+               396 CALL                     1
+               406 STORE_NAME              16 (frame2)
+   
+   127         408 PUSH_NULL
+               410 LOAD_NAME                3 (GTkDarkButton)
+               412 LOAD_NAME               16 (frame2)
+               414 LOAD_ATTR               13 (frame)
+               424 LOAD_CONST               5 ('GTkDarkButton')
+               426 KW_NAMES                15
+               428 PRECALL                  2
+               432 CALL                     2
+               442 STORE_NAME              17 (button2)
+   
+   128         444 LOAD_NAME               17 (button2)
+               446 LOAD_METHOD             15 (pack)
+               468 LOAD_CONST              16 ('x')
+               470 LOAD_CONST              17 (5)
+               472 LOAD_CONST              17 (5)
+               474 LOAD_CONST              17 (5)
+               476 KW_NAMES                18
+               478 PRECALL                  4
+               482 CALL                     4
+               492 POP_TOP
+   
+   130         494 LOAD_NAME               16 (frame2)
+               496 LOAD_METHOD             15 (pack)
+               518 LOAD_CONST              19 ('both')
+               520 LOAD_CONST              20 ('yes')
+               522 LOAD_CONST              23 ('left')
+               524 KW_NAMES                22
+               526 PRECALL                  3
+               530 CALL                     3
+               540 POP_TOP
+   
+   132         542 LOAD_NAME               11 (root)
+               544 LOAD_METHOD             18 (mainloop)
+               566 PRECALL                  0
+               570 CALL                     0
+               580 POP_TOP
+               582 LOAD_CONST              24 (None)
+               584 RETURN_VALUE
    
-   111     >>  572 LOAD_CONST              23 (None)
-               574 RETURN_VALUE
+   111     >>  586 LOAD_CONST              24 (None)
+               588 RETURN_VALUE
    consts
       0
       ('AdwDrawRoundButton3',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
@@ -736,125 +736,30 @@
          filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
          name       'GTkSuggestedButton'
          firstlineno 106
          lnotab 0x0a01
       'GTkSuggestedButton'
       '__main__'
       ('Tk',)
+      ('GTkFrame', 'GTkDarkFrame')
       '#1e1e1e'
       ('background',)
-      code
-         argcount  : 0
-         nlocals   : 0
-         stacksize : 3
-         flags     : 3
-         code
-            0x97007401000000000000000000006401a6010000ab0100000000000000
-            005300
-         117           0 RESUME                   0
-                       2 LOAD_GLOBAL              1 (NULL + print)
-                      14 LOAD_CONST               1 ('button1 clicked')
-                      16 PRECALL                  1
-                      20 CALL                     1
-                      30 RETURN_VALUE
-         consts
-            None
-            'button1 clicked'
-         names      ('print',)
-         varnames   ()
-         freevars   ()
-         cellvars   ()
-         filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
-         name       '<lambda>'
-         firstlineno 117
-         lnotab 0x
-      ('text', 'command')
+      ('text',)
       'x'
       5
       ('fill', 'ipadx', 'padx', 'pady')
-      code
-         argcount  : 0
-         nlocals   : 0
-         stacksize : 3
-         flags     : 3
-         code
-            0x97007401000000000000000000006401a6010000ab0100000000000000
-            005300
-         120           0 RESUME                   0
-                       2 LOAD_GLOBAL              1 (NULL + print)
-                      14 LOAD_CONST               1 ('button2 clicked')
-                      16 PRECALL                  1
-                      20 CALL                     1
-                      30 RETURN_VALUE
-         consts
-            None
-            'button2 clicked'
-         names      ('print',)
-         varnames   ()
-         freevars   ()
-         cellvars   ()
-         filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
-         name       '<lambda>'
-         firstlineno 120
-         lnotab 0x
-      ('text', 'command', 'background')
-      code
-         argcount  : 0
-         nlocals   : 0
-         stacksize : 3
-         flags     : 3
-         code
-            0x97007401000000000000000000006401a6010000ab0100000000000000
-            005300
-         123           0 RESUME                   0
-                       2 LOAD_GLOBAL              1 (NULL + print)
-                      14 LOAD_CONST               1 ('button3 clicked')
-                      16 PRECALL                  1
-                      20 CALL                     1
-                      30 RETURN_VALUE
-         consts
-            None
-            'button3 clicked'
-         names      ('print',)
-         varnames   ()
-         freevars   ()
-         cellvars   ()
-         filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
-         name       '<lambda>'
-         firstlineno 123
-         lnotab 0x
-      code
-         argcount  : 0
-         nlocals   : 0
-         stacksize : 3
-         flags     : 3
-         code
-            0x97007401000000000000000000006401a6010000ab0100000000000000
-            005300
-         126           0 RESUME                   0
-                       2 LOAD_GLOBAL              1 (NULL + print)
-                      14 LOAD_CONST               1 ('button4 clicked')
-                      16 PRECALL                  1
-                      20 CALL                     1
-                      30 RETURN_VALUE
-         consts
-            None
-            'button4 clicked'
-         names      ('print',)
-         varnames   ()
-         freevars   ()
-         cellvars   ()
-         filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
-         name       '<lambda>'
-         firstlineno 126
-         lnotab 0x
+      'both'
+      'yes'
+      'right'
+      ('fill', 'expand', 'side')
+      'left'
       None
-   names      ('tkadw', 'AdwDrawRoundButton3', 'GTkButton', 'GTkDarkButton', 'GTkDestructiveButton', 'GTkSuggestedButton', '__name__', 'tkinter', 'Tk', 'root', 'configure', 'button', 'pack', 'button2', 'button3', 'button4', 'mainloop')
+   names      ('tkadw', 'AdwDrawRoundButton3', 'GTkButton', 'GTkDarkButton', 'GTkDestructiveButton', 'GTkSuggestedButton', '__name__', 'tkinter', 'Tk', 'GTkFrame', 'GTkDarkFrame', 'root', 'configure', 'frame', 'button1', 'pack', 'frame2', 'button2', 'mainloop')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\button.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff02010c031c5c1c051c051c050c010c0214012c021c0132021e0132
-      021c0132021c0132022cee
+      0x00ff02010c031c5c1c051c051c050c010c01100214012c021602240132
+      02300216022401320230022ceb
```

### Comparing `tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc` & `tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/entry.cpython-311.pyc`

 * *Files 27% similar despite different names*

#### Python bytecode

```diff
@@ -1,28 +1,34 @@
 magic:    0xa70d0d0a
-moddate:  0x572f9564 (Fri Jun 23 05:36:23 2023 UTC)
-files sz: 2201
+moddate:  0x425a9564 (Fri Jun 23 08:39:30 2023 UTC)
+files sz: 2441
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x9700640064016c006d015a010100020047006402840064036501a60300
       00ab0300000000000000005a02020047006404840064056502a6030000ab
-      0300000000000000005a03650464066b02000000007286640064076c056d
-      065a06010002006506a6000000ab0000000000000000005a076507a00800
-      000000000000000000000000000000000000006408ac09a6010000ab0100
-      000000000000000100020065036403ac0aa6010000ab0100000000000000
-      005a096509a00a0000000000000000000000000000000000000000640b64
-      0c640c640cac0da6040000ab0400000000000000000100020065036405ac
-      0aa6010000ab0100000000000000005a0b650ba00a000000000000000000
-      0000000000000000000000640b640c640c640cac0da6040000ab04000000
-      000000000001006507a00c00000000000000000000000000000000000000
-      00a6000000ab0000000000000000000100640e5300640e5300
+      0300000000000000005a03650464066b020000000072e0640064076c056d
+      065a060100640064086c006d075a076d085a086d025a026d035a03010002
+      006506a6000000ab0000000000000000005a096509a00a00000000000000
+      000000000000000000000000006409ac0aa6010000ab0100000000000000
+      000100020065076509a6010000ab0100000000000000005a0b0200650265
+      0b6a0b0000000000000000a6010000ab0100000000000000005a0c650ca0
+      0d0000000000000000000000000000000000000000640b640c640c640cac
+      0da6040000ab0400000000000000000100650ba00d000000000000000000
+      0000000000000000000000640e640f6410ac11a6030000ab030000000000
+      0000000100020065086509a6010000ab0100000000000000005a0e020065
+      03650e6a0b0000000000000000a6010000ab0100000000000000005a0f65
+      0fa00d0000000000000000000000000000000000000000640b640c640c64
+      0cac0da6040000ab0400000000000000000100650ea00d00000000000000
+      00000000000000000000000000640e640f6412ac11a6030000ab03000000
+      000000000001006509a01000000000000000000000000000000000000000
+      00a6000000ab00000000000000000001006413530064135300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('AdwDrawRoundEntry3',))
                  6 IMPORT_NAME              0 (tkadw)
                  8 IMPORT_FROM              1 (AdwDrawRoundEntry3)
                 10 STORE_NAME               1 (AdwDrawRoundEntry3)
@@ -47,85 +53,132 @@
                 54 PRECALL                  3
                 58 CALL                     3
                 68 STORE_NAME               3 (GTkDarkEntry)
    
     65          70 LOAD_NAME                4 (__name__)
                 72 LOAD_CONST               6 ('__main__')
                 74 COMPARE_OP               2 (==)
-                80 POP_JUMP_FORWARD_IF_FALSE   134 (to 350)
+                80 POP_JUMP_FORWARD_IF_FALSE   224 (to 530)
    
     66          82 LOAD_CONST               0 (0)
                 84 LOAD_CONST               7 (('Tk',))
                 86 IMPORT_NAME              5 (tkinter)
                 88 IMPORT_FROM              6 (Tk)
                 90 STORE_NAME               6 (Tk)
                 92 POP_TOP
    
-    68          94 PUSH_NULL
-                96 LOAD_NAME                6 (Tk)
-                98 PRECALL                  0
-               102 CALL                     0
-               112 STORE_NAME               7 (root)
-   
-    69         114 LOAD_NAME                7 (root)
-               116 LOAD_METHOD              8 (configure)
-               138 LOAD_CONST               8 ('#1e1e1e')
-               140 KW_NAMES                 9
-               142 PRECALL                  1
-               146 CALL                     1
-               156 POP_TOP
-   
-    71         158 PUSH_NULL
-               160 LOAD_NAME                3 (GTkDarkEntry)
-               162 LOAD_CONST               3 ('GTkEntry')
+    67          94 LOAD_CONST               0 (0)
+                96 LOAD_CONST               8 (('GTkFrame', 'GTkDarkFrame', 'GTkEntry', 'GTkDarkEntry'))
+                98 IMPORT_NAME              0 (tkadw)
+               100 IMPORT_FROM              7 (GTkFrame)
+               102 STORE_NAME               7 (GTkFrame)
+               104 IMPORT_FROM              8 (GTkDarkFrame)
+               106 STORE_NAME               8 (GTkDarkFrame)
+               108 IMPORT_FROM              2 (GTkEntry)
+               110 STORE_NAME               2 (GTkEntry)
+               112 IMPORT_FROM              3 (GTkDarkEntry)
+               114 STORE_NAME               3 (GTkDarkEntry)
+               116 POP_TOP
+   
+    69         118 PUSH_NULL
+               120 LOAD_NAME                6 (Tk)
+               122 PRECALL                  0
+               126 CALL                     0
+               136 STORE_NAME               9 (root)
+   
+    70         138 LOAD_NAME                9 (root)
+               140 LOAD_METHOD             10 (configure)
+               162 LOAD_CONST               9 ('#1f1f1f')
                164 KW_NAMES                10
                166 PRECALL                  1
                170 CALL                     1
-               180 STORE_NAME               9 (entry)
+               180 POP_TOP
    
-    72         182 LOAD_NAME                9 (entry)
-               184 LOAD_METHOD             10 (pack)
-               206 LOAD_CONST              11 ('x')
-               208 LOAD_CONST              12 (5)
-               210 LOAD_CONST              12 (5)
-               212 LOAD_CONST              12 (5)
-               214 KW_NAMES                13
-               216 PRECALL                  4
-               220 CALL                     4
-               230 POP_TOP
-   
-    74         232 PUSH_NULL
-               234 LOAD_NAME                3 (GTkDarkEntry)
-               236 LOAD_CONST               5 ('GTkDarkEntry')
-               238 KW_NAMES                10
-               240 PRECALL                  1
-               244 CALL                     1
-               254 STORE_NAME              11 (entry2)
-   
-    75         256 LOAD_NAME               11 (entry2)
-               258 LOAD_METHOD             10 (pack)
-               280 LOAD_CONST              11 ('x')
-               282 LOAD_CONST              12 (5)
-               284 LOAD_CONST              12 (5)
-               286 LOAD_CONST              12 (5)
-               288 KW_NAMES                13
-               290 PRECALL                  4
-               294 CALL                     4
-               304 POP_TOP
-   
-    77         306 LOAD_NAME                7 (root)
-               308 LOAD_METHOD             12 (mainloop)
-               330 PRECALL                  0
-               334 CALL                     0
-               344 POP_TOP
-               346 LOAD_CONST              14 (None)
-               348 RETURN_VALUE
+    72         182 PUSH_NULL
+               184 LOAD_NAME                7 (GTkFrame)
+               186 LOAD_NAME                9 (root)
+               188 PRECALL                  1
+               192 CALL                     1
+               202 STORE_NAME              11 (frame)
+   
+    74         204 PUSH_NULL
+               206 LOAD_NAME                2 (GTkEntry)
+               208 LOAD_NAME               11 (frame)
+               210 LOAD_ATTR               11 (frame)
+               220 PRECALL                  1
+               224 CALL                     1
+               234 STORE_NAME              12 (entry1)
+   
+    75         236 LOAD_NAME               12 (entry1)
+               238 LOAD_METHOD             13 (pack)
+               260 LOAD_CONST              11 ('x')
+               262 LOAD_CONST              12 (5)
+               264 LOAD_CONST              12 (5)
+               266 LOAD_CONST              12 (5)
+               268 KW_NAMES                13
+               270 PRECALL                  4
+               274 CALL                     4
+               284 POP_TOP
+   
+    77         286 LOAD_NAME               11 (frame)
+               288 LOAD_METHOD             13 (pack)
+               310 LOAD_CONST              14 ('both')
+               312 LOAD_CONST              15 ('yes')
+               314 LOAD_CONST              16 ('right')
+               316 KW_NAMES                17
+               318 PRECALL                  3
+               322 CALL                     3
+               332 POP_TOP
+   
+    79         334 PUSH_NULL
+               336 LOAD_NAME                8 (GTkDarkFrame)
+               338 LOAD_NAME                9 (root)
+               340 PRECALL                  1
+               344 CALL                     1
+               354 STORE_NAME              14 (frame2)
+   
+    81         356 PUSH_NULL
+               358 LOAD_NAME                3 (GTkDarkEntry)
+               360 LOAD_NAME               14 (frame2)
+               362 LOAD_ATTR               11 (frame)
+               372 PRECALL                  1
+               376 CALL                     1
+               386 STORE_NAME              15 (entry2)
+   
+    82         388 LOAD_NAME               15 (entry2)
+               390 LOAD_METHOD             13 (pack)
+               412 LOAD_CONST              11 ('x')
+               414 LOAD_CONST              12 (5)
+               416 LOAD_CONST              12 (5)
+               418 LOAD_CONST              12 (5)
+               420 KW_NAMES                13
+               422 PRECALL                  4
+               426 CALL                     4
+               436 POP_TOP
+   
+    84         438 LOAD_NAME               14 (frame2)
+               440 LOAD_METHOD             13 (pack)
+               462 LOAD_CONST              14 ('both')
+               464 LOAD_CONST              15 ('yes')
+               466 LOAD_CONST              18 ('left')
+               468 KW_NAMES                17
+               470 PRECALL                  3
+               474 CALL                     3
+               484 POP_TOP
+   
+    86         486 LOAD_NAME                9 (root)
+               488 LOAD_METHOD             16 (mainloop)
+               510 PRECALL                  0
+               514 CALL                     0
+               524 POP_TOP
+               526 LOAD_CONST              19 (None)
+               528 RETURN_VALUE
    
-    65     >>  350 LOAD_CONST              14 (None)
-               352 RETURN_VALUE
+    65     >>  530 LOAD_CONST              19 (None)
+               532 RETURN_VALUE
    consts
       0
       ('AdwDrawRoundEntry3',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
@@ -435,22 +488,29 @@
          filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\entry.py'
          name       'GTkDarkEntry'
          firstlineno 60
          lnotab 0x0a01
       'GTkDarkEntry'
       '__main__'
       ('Tk',)
-      '#1e1e1e'
+      ('GTkFrame', 'GTkDarkFrame', 'GTkEntry', 'GTkDarkEntry')
+      '#1f1f1f'
       ('background',)
-      ('text',)
       'x'
       5
       ('fill', 'ipadx', 'padx', 'pady')
+      'both'
+      'yes'
+      'right'
+      ('fill', 'expand', 'side')
+      'left'
       None
-   names      ('tkadw', 'AdwDrawRoundEntry3', 'GTkEntry', 'GTkDarkEntry', '__name__', 'tkinter', 'Tk', 'root', 'configure', 'entry', 'pack', 'entry2', 'mainloop')
+   names      ('tkadw', 'AdwDrawRoundEntry3', 'GTkEntry', 'GTkDarkEntry', '__name__', 'tkinter', 'Tk', 'GTkFrame', 'GTkDarkFrame', 'root', 'configure', 'frame', 'entry1', 'pack', 'frame2', 'entry2', 'mainloop')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'D:\\tkadw\\tkadw\\tkite\\gtk\\entry.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c031c381c050c010c0214012c0218013202180132022cf4
+   lnotab
+      0x00ff02010c031c381c050c010c01180214012c02160220013202300216
+      022001320230022ceb
```

### Comparing `tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc` & `tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/frame.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc` & `tkadw-0.1.5/tkadw/tkite/gtk/__pycache__/textbox.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/tkite/gtk/button.py` & `tkadw-0.1.5/tkadw/tkite/gtk/button.py`

 * *Files 22% similar despite different names*

```diff
@@ -106,24 +106,27 @@
 class GTkSuggestedButton(GTkButton):
     def default_palette(self):
         self.palette_gtk_blue()
 
 
 if __name__ == '__main__':
     from tkinter import Tk
+    from tkadw import GTkFrame, GTkDarkFrame
 
     root = Tk()
     root.configure(background="#1e1e1e")
 
-    button = GTkDarkButton(text="GTkButton", command=lambda: print("button1 clicked"))
-    button.pack(fill="x", ipadx=5, padx=5, pady=5)
+    frame = GTkFrame(root)
 
-    button2 = GTkDarkButton(text="GTkDarkButton", command=lambda: print("button2 clicked"), background="#1e1e1e")
-    button2.pack(fill="x", ipadx=5, padx=5, pady=5)
+    button1 = GTkButton(frame.frame, text="GTkButton")
+    button1.pack(fill="x", ipadx=5, padx=5, pady=5)
+
+    frame.pack(fill="both", expand="yes", side="right")
 
-    button3 = GTkDestructiveButton(text="GTkDestructiveButton", command=lambda: print("button3 clicked"))
-    button3.pack(fill="x", ipadx=5, padx=5, pady=5)
+    frame2 = GTkDarkFrame(root)
+
+    button2 = GTkDarkButton(frame2.frame, text="GTkDarkButton")
+    button2.pack(fill="x", ipadx=5, padx=5, pady=5)
 
-    button4 = GTkSuggestedButton(text="GTkSuggestedButton", command=lambda: print("button4 clicked"))
-    button4.pack(fill="x", ipadx=5, padx=5, pady=5)
+    frame2.pack(fill="both", expand="yes", side="left")
 
     root.mainloop()
```

### Comparing `tkadw-0.1.3/tkadw/tkite/gtk/entry.py` & `tkadw-0.1.5/tkadw/tkite/gtk/entry.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,18 +60,27 @@
 class GTkDarkEntry(GTkEntry):
     def default_palette(self):
         self.palette_gtk_dark()
 
 
 if __name__ == '__main__':
     from tkinter import Tk
+    from tkadw import GTkFrame, GTkDarkFrame, GTkEntry, GTkDarkEntry
 
     root = Tk()
-    root.configure(background="#1e1e1e")
+    root.configure(background="#1f1f1f")
 
-    entry = GTkDarkEntry(text="GTkEntry")
-    entry.pack(fill="x", ipadx=5, padx=5, pady=5)
+    frame = GTkFrame(root)
 
-    entry2 = GTkDarkEntry(text="GTkDarkEntry")
+    entry1 = GTkEntry(frame.frame)
+    entry1.pack(fill="x", ipadx=5, padx=5, pady=5)
+
+    frame.pack(fill="both", expand="yes", side="right")
+
+    frame2 = GTkDarkFrame(root)
+
+    entry2 = GTkDarkEntry(frame2.frame)
     entry2.pack(fill="x", ipadx=5, padx=5, pady=5)
 
+    frame2.pack(fill="both", expand="yes", side="left")
+
     root.mainloop()
```

### Comparing `tkadw-0.1.3/tkadw/tkite/gtk/frame.py` & `tkadw-0.1.5/tkadw/tkite/gtk/frame.py`

 * *Files identical despite different names*

### Comparing `tkadw-0.1.3/tkadw/tkite/gtk/textbox.py` & `tkadw-0.1.5/tkadw/tkite/gtk/textbox.py`

 * *Files identical despite different names*

