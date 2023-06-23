# Comparing `tmp/pter-3.7.0.tar.gz` & `tmp/pter-3.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pter-3.7.0.tar", last modified: Thu May 11 17:29:24 2023, max compression
+gzip compressed data, was "pter-3.8.0.tar", last modified: Fri Jun 23 09:45:04 2023, max compression
```

## Comparing `pter-3.7.0.tar` & `pter-3.8.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.486706 pter-3.7.0/
--rw-r--r--   0 robert    (1000) robert    (1000)    11813 2023-05-11 17:23:02.000000 pter-3.7.0/CHANGELOG.md
--rw-r--r--   0 robert    (1000) robert    (1000)     1097 2022-04-15 06:59:55.000000 pter-3.7.0/LICENSE
--rw-r--r--   0 robert    (1000) robert    (1000)      218 2022-02-19 08:34:12.000000 pter-3.7.0/MANIFEST.in
--rw-r--r--   0 robert    (1000) robert    (1000)     2900 2023-05-11 17:29:24.483373 pter-3.7.0/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)     2313 2022-07-24 08:17:34.000000 pter-3.7.0/README.md
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.480039 pter-3.7.0/doc/
--rw-r--r--   0 robert    (1000) robert    (1000)   365846 2022-02-19 08:34:12.000000 pter-3.7.0/doc/pter-demo.gif
--rw-r--r--   0 robert    (1000) robert    (1000)    45973 2023-05-11 17:27:09.000000 pter-3.7.0/doc/pter.rst
--rw-r--r--   0 robert    (1000) robert    (1000)    29201 2022-02-19 08:34:12.000000 pter-3.7.0/doc/qpter.png
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.483373 pter-3.7.0/extras/
--rw-r--r--   0 robert    (1000) robert    (1000)     8834 2022-02-19 08:34:12.000000 pter-3.7.0/extras/example.conf
--rw-r--r--   0 robert    (1000) robert    (1000)      196 2022-02-19 08:34:12.000000 pter-3.7.0/extras/pter.desktop
--rw-r--r--   0 robert    (1000) robert    (1000)      296 2022-02-19 08:34:12.000000 pter-3.7.0/extras/qpter.desktop
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.483373 pter-3.7.0/man/
--rw-r--r--   0 robert    (1000) robert    (1000)    53014 2023-05-11 17:29:24.000000 pter-3.7.0/man/pter.1
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.483373 pter-3.7.0/pter/
--rw-r--r--   0 robert    (1000) robert    (1000)        0 2023-05-11 17:11:53.000000 pter-3.7.0/pter/__init__.py
--rw-r--r--   0 robert    (1000) robert    (1000)     5089 2023-05-11 17:11:53.000000 pter-3.7.0/pter/common.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6686 2023-05-11 17:11:53.000000 pter-3.7.0/pter/configuration.py
--rw-r--r--   0 robert    (1000) robert    (1000)    89000 2023-05-11 17:11:53.000000 pter-3.7.0/pter/curses.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.483373 pter-3.7.0/pter/docs/
--rw-r--r--   0 robert    (1000) robert    (1000)    83258 2023-05-11 17:29:24.000000 pter-3.7.0/pter/docs/pter.html
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.483373 pter-3.7.0/pter/icons/
--rw-r--r--   0 robert    (1000) robert    (1000)     1083 2022-02-19 08:34:12.000000 pter-3.7.0/pter/icons/qpter_16x16.png
--rw-r--r--   0 robert    (1000) robert    (1000)     1598 2022-02-19 08:34:12.000000 pter-3.7.0/pter/icons/qpter_32x32.png
--rw-r--r--   0 robert    (1000) robert    (1000)     5399 2023-05-11 17:11:53.000000 pter-3.7.0/pter/key.py
--rw-r--r--   0 robert    (1000) robert    (1000)     4358 2023-05-11 17:11:53.000000 pter-3.7.0/pter/main.py
--rw-r--r--   0 robert    (1000) robert    (1000)    75198 2023-05-11 17:11:53.000000 pter-3.7.0/pter/qtui.py
--rw-r--r--   0 robert    (1000) robert    (1000)    19345 2023-05-11 17:11:53.000000 pter-3.7.0/pter/searcher.py
--rw-r--r--   0 robert    (1000) robert    (1000)     2261 2023-05-11 17:11:53.000000 pter-3.7.0/pter/source.py
--rw-r--r--   0 robert    (1000) robert    (1000)       31 2023-05-11 17:11:53.000000 pter-3.7.0/pter/tr.py
--rw-r--r--   0 robert    (1000) robert    (1000)    17809 2023-05-11 17:11:53.000000 pter-3.7.0/pter/utils.py
--rw-r--r--   0 robert    (1000) robert    (1000)       23 2023-05-11 17:27:33.000000 pter-3.7.0/pter/version.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.483373 pter-3.7.0/pter.egg-info/
--rw-r--r--   0 robert    (1000) robert    (1000)     2900 2023-05-11 17:29:24.000000 pter-3.7.0/pter.egg-info/PKG-INFO
--rw-r--r--   0 robert    (1000) robert    (1000)      747 2023-05-11 17:29:24.000000 pter-3.7.0/pter.egg-info/SOURCES.txt
--rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-05-11 17:29:24.000000 pter-3.7.0/pter.egg-info/dependency_links.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       76 2023-05-11 17:29:24.000000 pter-3.7.0/pter.egg-info/entry_points.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       49 2023-05-11 17:29:24.000000 pter-3.7.0/pter.egg-info/requires.txt
--rw-r--r--   0 robert    (1000) robert    (1000)        5 2023-05-11 17:29:24.000000 pter-3.7.0/pter.egg-info/top_level.txt
--rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-05-11 17:29:24.486706 pter-3.7.0/setup.cfg
--rw-r--r--   0 robert    (1000) robert    (1000)     2773 2022-02-19 08:34:12.000000 pter-3.7.0/setup.py
-drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-05-11 17:29:24.483373 pter-3.7.0/tests/
--rw-r--r--   0 robert    (1000) robert    (1000)     1518 2022-02-19 08:34:12.000000 pter-3.7.0/tests/test_displaynames.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1684 2022-10-31 18:55:16.000000 pter-3.7.0/tests/test_priochange.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1221 2022-02-19 08:34:12.000000 pter-3.7.0/tests/test_pter.py
--rw-r--r--   0 robert    (1000) robert    (1000)     6496 2022-02-19 08:34:12.000000 pter-3.7.0/tests/test_rec.py
--rw-r--r--   0 robert    (1000) robert    (1000)    12855 2022-02-19 08:34:12.000000 pter-3.7.0/tests/test_searcher.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1618 2022-02-19 08:34:12.000000 pter-3.7.0/tests/test_sorting.py
--rw-r--r--   0 robert    (1000) robert    (1000)     1475 2022-02-19 08:34:12.000000 pter-3.7.0/tests/test_taskid.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.336876 pter-3.8.0/
+-rw-r--r--   0 robert    (1000) robert    (1000)    12126 2023-06-23 09:43:15.000000 pter-3.8.0/CHANGELOG.md
+-rw-r--r--   0 robert    (1000) robert    (1000)     1097 2022-04-15 06:59:55.000000 pter-3.8.0/LICENSE
+-rw-r--r--   0 robert    (1000) robert    (1000)      218 2022-02-19 08:34:12.000000 pter-3.8.0/MANIFEST.in
+-rw-r--r--   0 robert    (1000) robert    (1000)     2900 2023-06-23 09:45:04.336876 pter-3.8.0/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)     2313 2022-07-24 08:17:34.000000 pter-3.8.0/README.md
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.333542 pter-3.8.0/doc/
+-rw-r--r--   0 robert    (1000) robert    (1000)   365846 2022-02-19 08:34:12.000000 pter-3.8.0/doc/pter-demo.gif
+-rw-r--r--   0 robert    (1000) robert    (1000)    47149 2023-06-23 09:15:08.000000 pter-3.8.0/doc/pter.rst
+-rw-r--r--   0 robert    (1000) robert    (1000)    29201 2022-02-19 08:34:12.000000 pter-3.8.0/doc/qpter.png
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.333542 pter-3.8.0/extras/
+-rw-r--r--   0 robert    (1000) robert    (1000)     8834 2022-02-19 08:34:12.000000 pter-3.8.0/extras/example.conf
+-rw-r--r--   0 robert    (1000) robert    (1000)      196 2022-02-19 08:34:12.000000 pter-3.8.0/extras/pter.desktop
+-rw-r--r--   0 robert    (1000) robert    (1000)      296 2022-02-19 08:34:12.000000 pter-3.8.0/extras/qpter.desktop
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.333542 pter-3.8.0/man/
+-rw-r--r--   0 robert    (1000) robert    (1000)    54422 2023-06-23 09:45:04.000000 pter-3.8.0/man/pter.1
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.333542 pter-3.8.0/pter/
+-rw-r--r--   0 robert    (1000) robert    (1000)        0 2023-05-11 17:11:53.000000 pter-3.8.0/pter/__init__.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     5458 2023-06-23 08:05:52.000000 pter-3.8.0/pter/common.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     6844 2023-06-23 07:37:57.000000 pter-3.8.0/pter/configuration.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    94139 2023-06-23 09:40:58.000000 pter-3.8.0/pter/curses.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.333542 pter-3.8.0/pter/docs/
+-rw-r--r--   0 robert    (1000) robert    (1000)    85420 2023-06-23 09:45:04.000000 pter-3.8.0/pter/docs/pter.html
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.333542 pter-3.8.0/pter/icons/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1083 2022-02-19 08:34:12.000000 pter-3.8.0/pter/icons/qpter_16x16.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     1598 2022-02-19 08:34:12.000000 pter-3.8.0/pter/icons/qpter_32x32.png
+-rw-r--r--   0 robert    (1000) robert    (1000)     5399 2023-05-11 17:11:53.000000 pter-3.8.0/pter/key.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     4358 2023-06-23 08:13:15.000000 pter-3.8.0/pter/main.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    75198 2023-05-11 17:11:53.000000 pter-3.8.0/pter/qtui.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    19345 2023-05-11 17:11:53.000000 pter-3.8.0/pter/searcher.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     2261 2023-05-11 17:11:53.000000 pter-3.8.0/pter/source.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       31 2023-05-11 17:11:53.000000 pter-3.8.0/pter/tr.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    17809 2023-05-11 17:11:53.000000 pter-3.8.0/pter/utils.py
+-rw-r--r--   0 robert    (1000) robert    (1000)       23 2023-06-23 09:10:28.000000 pter-3.8.0/pter/version.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.333542 pter-3.8.0/pter.egg-info/
+-rw-r--r--   0 robert    (1000) robert    (1000)     2900 2023-06-23 09:45:04.000000 pter-3.8.0/pter.egg-info/PKG-INFO
+-rw-r--r--   0 robert    (1000) robert    (1000)      762 2023-06-23 09:45:04.000000 pter-3.8.0/pter.egg-info/SOURCES.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        1 2023-06-23 09:45:04.000000 pter-3.8.0/pter.egg-info/dependency_links.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       76 2023-06-23 09:45:04.000000 pter-3.8.0/pter.egg-info/entry_points.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       49 2023-06-23 09:45:04.000000 pter-3.8.0/pter.egg-info/requires.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)        5 2023-06-23 09:45:04.000000 pter-3.8.0/pter.egg-info/top_level.txt
+-rw-r--r--   0 robert    (1000) robert    (1000)       50 2023-06-23 08:59:37.000000 pter-3.8.0/pyproject.toml
+-rw-r--r--   0 robert    (1000) robert    (1000)       38 2023-06-23 09:45:04.336876 pter-3.8.0/setup.cfg
+-rw-r--r--   0 robert    (1000) robert    (1000)     2773 2022-02-19 08:34:12.000000 pter-3.8.0/setup.py
+drwxr-xr-x   0 robert    (1000) robert    (1000)        0 2023-06-23 09:45:04.336876 pter-3.8.0/tests/
+-rw-r--r--   0 robert    (1000) robert    (1000)     1518 2022-02-19 08:34:12.000000 pter-3.8.0/tests/test_displaynames.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1684 2022-10-31 18:55:16.000000 pter-3.8.0/tests/test_priochange.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1221 2022-02-19 08:34:12.000000 pter-3.8.0/tests/test_pter.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     6496 2022-02-19 08:34:12.000000 pter-3.8.0/tests/test_rec.py
+-rw-r--r--   0 robert    (1000) robert    (1000)    12855 2022-02-19 08:34:12.000000 pter-3.8.0/tests/test_searcher.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1618 2022-02-19 08:34:12.000000 pter-3.8.0/tests/test_sorting.py
+-rw-r--r--   0 robert    (1000) robert    (1000)     1475 2022-02-19 08:34:12.000000 pter-3.8.0/tests/test_taskid.py
```

### Comparing `pter-3.7.0/CHANGELOG.md` & `pter-3.8.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 # Changelog
 
 This file contains the changes made between released versions.
 
 The format is based on [Keep a changelog](https://keepachangelog.com/) and the versioning tries to follow
 [Semantic Versioning](https://semver.org).
 
+## 3.8.0
+### Added
+- Archiving is now a thing. Default key binding for `archive` function is `%`
+- Archive location can be configured, see `archive-is` configuration option
+- New function `edit-file-external`, by default not mapped to a key
+
+### Fixed
+- Trash file access is more forgiving and won't crash pter
+
 
 ## 3.7.0
 ### Changed
 - When using templates, the initial cursor position will be after the creation date or at the start of the field
 
 ### Added
 - When editing a task you can `Tab` through not-filled in keys, like `due:`
 
+
 ## 3.6.1
 ### Fixed
 - When scrolling past the end of list of tasks pter could crash (related to key sequences)
 
 
 ## 3.6.0
 ### Added
```

### Comparing `pter-3.7.0/LICENSE` & `pter-3.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/PKG-INFO` & `pter-3.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pter
-Version: 3.7.0
+Version: 3.8.0
 Summary: Console UI to manage your todo.txt file(s).
 Home-page: https://vonshednob.cc/pter
 Author: R
 Author-email: contact+pter@vonshednob.cc
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `pter-3.7.0/README.md` & `pter-3.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/doc/pter-demo.gif` & `pter-3.8.0/doc/pter-demo.gif`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/doc/pter.rst` & `pter-3.8.0/doc/pter.rst`

 * *Files 1% similar despite different names*

```diff
@@ -243,17 +243,33 @@
      - ``disabled``, no functionality at all. There is no delete. This is
        the default.
      - ``trash``, deleted tasks are moved to the trash file (see
        ``trash-file`` option below).
      - ``permanent``, actually deletes the task.
 
   ``trash-file``
-    What your trash file is. This option is only used if ``delete-is`` is
+    Where your trash file is. This option is only used if ``delete-is`` is
     set to ``trash``. Defaults to ``~/.config/pter/trash.txt``.
 
+  ``archive-is``
+    Defines the behaviour of the ``archive`` function. Can be one of these:
+
+     - ``relative``, the archive file is assumed to be in the same place as
+       the ``todo.txt`` file, but called ``archive.txt``,
+     - ``centralised``, there is only one archive file for all ``todo.txt``
+       files. Its location is controlled by ``archive-file``,
+     - ``disabled``, there is no archiving.
+
+    Defaults to ``centralised``.
+
+  ``archive-file``
+    Where your archive file is. This file will be used to receive archived
+    tasks if the ``archive-is`` option is set to ``centralised``. Defaults
+    to ``~/.config/pter/archive.txt``.
+
   ``reuse-recurring``
     Reuse existing recurring task entry instead of creating a new one. If
     set, completing a task with a ``rec:`` (recurring) tag will be reused
     for the follow-up task instead of creating a new task.
 
     Defaults to ``no``.
 
@@ -322,17 +338,19 @@
 
  - ``quit``: quit the program
  - ``show-help``: show the full screen help (only key bindings so far)
  - ``open-manual``: open this manual in a browser
  - ``create-task``: create a new task
  - ``edit-task``: edit the selected task
  - ``edit-external``: edit the selected task in an external text editor
+ - ``edit-file-external``: edit the todo.txt of the selected task in an external editor
  - ``delete-task``: delete the selected task or move it to trash, depends
    on the configuration option ``delete-is`` (by default not bound to any
    key)
+ - ``archive``: move the selected task to the designated archive file
  - ``load-search``: show the saved searches to load one
  - ``open-url``: open a URL of the selected task
  - ``refresh-screen``: rebuild the GUI
  - ``reload-tasks``: enforce reloading of all tasks from all sources
  - ``save-search``: save the current search
  - ``search``: enter a new search query
  - ``clear-search``: clear the search query
@@ -721,14 +739,22 @@
  - "l": load a named search
  - "s": save the current search
  - "L": load a named task template
  - "S": Save a task as a named template
  - "u": open a URL listed in the selected task
  - "t": Start/stop time tracking of the selected task
  - ">": Delegate the selected task
+ - "A": Set the priority of this task to ``(A)``
+ - "B": Set the priority of this task to ``(B)``
+ - "C": Set the priority of this task to ``(C)``
+ - "D": Set the priority of this task to ``(D)``
+ - "+": Increase the priority of this task
+ - "-": Decrease the priority of this task
+ - "=": Remove the priority of this task
+ - "%": Move this task into the archive
 
 In edit fields the following keyboard controls are available:
 
  - "←", "→" (cursor keys): move the cursor one character to the left or right
  - "Home": move the cursor to the first charater
  - "End": move the cursor to the last character
  - "Backspace", "^H": delete the character to the left of the cursor
```

### Comparing `pter-3.7.0/doc/qpter.png` & `pter-3.8.0/doc/qpter.png`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/extras/example.conf` & `pter-3.8.0/extras/example.conf`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/man/pter.1` & `pter-3.8.0/man/pter.1`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 . RE
 .\" indent \\n[an-margin]
 .\" old: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .nr rst2man-indent-level -1
 .\" new: \\n[rst2man-indent\\n[rst2man-indent-level]]
 .in \\n[rst2man-indent\\n[rst2man-indent-level]]u
 ..
-.TH "PTER"  "" "" ""
+.TH "PTER"  "" ""
 .SH NAME
 pter \- Personal Task Entropy Reducer
 .SH SYNOPSIS
 .INDENT 0.0
 .INDENT 3.5
 .sp
 .nf
@@ -317,17 +317,41 @@
 .IP \(bu 2
 \fBpermanent\fP, actually deletes the task.
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .TP
 .B \fBtrash\-file\fP
-What your trash file is. This option is only used if \fBdelete\-is\fP is
+Where your trash file is. This option is only used if \fBdelete\-is\fP is
 set to \fBtrash\fP\&. Defaults to \fB~/.config/pter/trash.txt\fP\&.
 .TP
+.B \fBarchive\-is\fP
+Defines the behaviour of the \fBarchive\fP function. Can be one of these:
+.INDENT 7.0
+.INDENT 3.5
+.INDENT 0.0
+.IP \(bu 2
+\fBrelative\fP, the archive file is assumed to be in the same place as
+the \fBtodo.txt\fP file, but called \fBarchive.txt\fP,
+.IP \(bu 2
+\fBcentralised\fP, there is only one archive file for all \fBtodo.txt\fP
+files. Its location is controlled by \fBarchive\-file\fP,
+.IP \(bu 2
+\fBdisabled\fP, there is no archiving.
+.UNINDENT
+.UNINDENT
+.UNINDENT
+.sp
+Defaults to \fBcentralised\fP\&.
+.TP
+.B \fBarchive\-file\fP
+Where your archive file is. This file will be used to receive archived
+tasks if the \fBarchive\-is\fP option is set to \fBcentralised\fP\&. Defaults
+to \fB~/.config/pter/archive.txt\fP\&.
+.TP
 .B \fBreuse\-recurring\fP
 Reuse existing recurring task entry instead of creating a new one. If
 set, completing a task with a \fBrec:\fP (recurring) tag will be reused
 for the follow\-up task instead of creating a new task.
 .sp
 Defaults to \fBno\fP\&.
 .TP
@@ -437,18 +461,22 @@
 .IP \(bu 2
 \fBcreate\-task\fP: create a new task
 .IP \(bu 2
 \fBedit\-task\fP: edit the selected task
 .IP \(bu 2
 \fBedit\-external\fP: edit the selected task in an external text editor
 .IP \(bu 2
+\fBedit\-file\-external\fP: edit the todo.txt of the selected task in an external editor
+.IP \(bu 2
 \fBdelete\-task\fP: delete the selected task or move it to trash, depends
 on the configuration option \fBdelete\-is\fP (by default not bound to any
 key)
 .IP \(bu 2
+\fBarchive\fP: move the selected task to the designated archive file
+.IP \(bu 2
 \fBload\-search\fP: show the saved searches to load one
 .IP \(bu 2
 \fBopen\-url\fP: open a URL of the selected task
 .IP \(bu 2
 \fBrefresh\-screen\fP: rebuild the GUI
 .IP \(bu 2
 \fBreload\-tasks\fP: enforce reloading of all tasks from all sources
@@ -1099,14 +1127,30 @@
 \(dqS\(dq: Save a task as a named template
 .IP \(bu 2
 \(dqu\(dq: open a URL listed in the selected task
 .IP \(bu 2
 \(dqt\(dq: Start/stop time tracking of the selected task
 .IP \(bu 2
 \(dq>\(dq: Delegate the selected task
+.IP \(bu 2
+\(dqA\(dq: Set the priority of this task to \fB(A)\fP
+.IP \(bu 2
+\(dqB\(dq: Set the priority of this task to \fB(B)\fP
+.IP \(bu 2
+\(dqC\(dq: Set the priority of this task to \fB(C)\fP
+.IP \(bu 2
+\(dqD\(dq: Set the priority of this task to \fB(D)\fP
+.IP \(bu 2
+\(dq+\(dq: Increase the priority of this task
+.IP \(bu 2
+\(dq\-\(dq: Decrease the priority of this task
+.IP \(bu 2
+\(dq=\(dq: Remove the priority of this task
+.IP \(bu 2
+\(dq%\(dq: Move this task into the archive
 .UNINDENT
 .UNINDENT
 .UNINDENT
 .sp
 In edit fields the following keyboard controls are available:
 .INDENT 0.0
 .INDENT 3.5
```

### Comparing `pter-3.7.0/pter/common.py` & `pter-3.8.0/pter/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     CACHEDIR = pathlib.Path(BaseDirectory.save_cache_path(PROGRAMNAME) or CACHEDIR)
     CACHEFILE = CACHEDIR / (PROGRAMNAME + ".settings")
 
 SEARCHES_FILE = CONFIGDIR / "searches.txt"
 TEMPLATES_FILE = CONFIGDIR / "templates.txt"
 LOGFILE = CACHEDIR / (PROGRAMNAME + ".log")
 DEFAULT_TRASHFILE = CONFIGDIR / "trash.txt"
+DEFAULT_ARCHIVE = CONFIGDIR / "archive.txt"
 
 URL_RE = re.compile(r'([A-Za-z][A-Za-z0-9+\-.]*)://([^ ]+)')
 
 DEFAULT_TASK_FORMAT = '{selection: >} {nr: >} {done} {tracking }{due }{(pri) }{description}'
 ATTR_TRACKING = 'tracking'
 ATTR_T = 't'
 ATTR_DUE = 'due'
@@ -43,14 +44,21 @@
 DELEGATE_ACTIONS = (DELEGATE_ACTION_NONE, DELEGATE_ACTION_MAIL)
 
 DELETE_OPTION_DISABLED = 'disabled'
 DELETE_OPTION_TRASH = 'trash'
 DELETE_OPTION_PERMANENT = 'permanent'
 DELETE_OPTIONS = (DELETE_OPTION_DISABLED, DELETE_OPTION_TRASH, DELETE_OPTION_PERMANENT)
 
+ARCHIVE_OPTION_RELATIVE = 'relative'
+ARCHIVE_OPTION_CENTRALISED = 'centralised'
+ARCHIVE_OPTION_DISABLED = 'disabled'
+ARCHIVE_OPTIONS = (ARCHIVE_OPTION_RELATIVE,
+                   ARCHIVE_OPTION_CENTRALISED,
+                   ARCHIVE_OPTION_DISABLED)
+
 DEFAULT_SORT_ORDER = 'completed,due_in,priority,linenr'
 DEFAULT_INFO_TIMEOUT = 5
 
 SETTING_GROUP_GENERAL = 'General'
 SETTING_GROUP_SYMBOLS = 'Symbols'
 SETTING_GROUP_COLORS = 'Colors'
 SETTING_GROUP_HIGHLIGHT = 'Highlight'
@@ -87,14 +95,16 @@
 SETTING_AUTO_ID = 'auto-id'
 SETTING_HIDE_SEQUENTIAL = 'hide-sequential'
 SETTING_CLICKABLE = 'clickable'
 SETTING_DAILY_RELOAD = 'daily-reload'
 SETTING_DELETE_IS = 'delete-is'
 SETTING_TRASHFILE = 'trash-file'
 SETTING_INFO_TIMEOUT = 'info-timeout'
+SETTING_ARCHIVE_FILE = 'archive-file'
+SETTING_ARCHIVE_IS = 'archive-is'
 SETTING_ICON_SELECTION = 'selection'
 SETTING_ICON_NOT_DONE = 'not-done'
 SETTING_ICON_DONE = 'done'
 SETTING_ICON_OVERFLOW_LEFT = 'overflow-left'
 SETTING_ICON_OVERFLOW_RIGHT = 'overflow-right'
 SETTING_ICON_OVERDUE = 'overdue'
 SETTING_ICON_DUE_TODAY = 'due-today'
```

### Comparing `pter-3.7.0/pter/configuration.py` & `pter-3.8.0/pter/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,18 @@
             common.SETTING_PROTOCOLS: 'http,https,mailto,ftp,ftps',
             common.SETTING_CREATE_FROM_SEARCH: 'no',
             common.SETTING_AUTO_ID: 'no',
             common.SETTING_HIDE_SEQUENTIAL: 'yes',
             common.SETTING_RELATED_SHOW_SELF: 'yes',
             common.SETTING_INFO_TIMEOUT: common.DEFAULT_INFO_TIMEOUT,
             common.SETTING_USE_COMPLETION: 'yes',
-            common.SETTING_DELETE_IS: 'disabled',
+            common.SETTING_DELETE_IS: common.DELETE_OPTION_DISABLED,
             common.SETTING_TRASHFILE: common.DEFAULT_TRASHFILE,
+            common.SETTING_ARCHIVE_IS: common.ARCHIVE_OPTION_CENTRALISED,
+            common.SETTING_ARCHIVE_FILE: common.DEFAULT_ARCHIVE,
         },
         common.SETTING_GROUP_SYMBOLS: {
             common.SETTING_ICON_SELECTION: '',
             common.SETTING_ICON_NOT_DONE: '[ ]',
             common.SETTING_ICON_DONE: '[x]',
             common.SETTING_ICON_OVERFLOW_LEFT: '←',
             common.SETTING_ICON_OVERFLOW_RIGHT: '→',
```

### Comparing `pter-3.7.0/pter/curses.py` & `pter-3.8.0/pter/curses.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import logging
 import os
 import sys
 import datetime
 import string
 import webbrowser
 import curses
-import curses.panel
 import traceback
 import tempfile
 import subprocess
 import shlex
 import shutil
 
-from pytodotxt import TodoTxt, Task
+from pytodotxt import TodoTxt, Task, TodoTxtParser
 
 from cursedspace import Application, Panel, ScrollPanel, InputLine, ShellContext, Completion
 
 from pter import common
 from pter import utils
 from pter import configuration
 from pter.searcher import Searcher
@@ -29,14 +28,16 @@
                'select-item': 'Select',
                'next-item': 'Next item',
                'prev-item': 'Previous item',
                'page-up': 'One page up',
                'page-down': 'One page down',
                'search': 'Search',
                'open-url': 'Open URL',
+               'edit-external': 'Edit task in external editor',
+               'edit-file-external': 'Edit todo.txt in external editor',
                'load-template': 'Load task template',
                'save-template': 'Save task as template',
                'load-search': 'Load search',
                'save-search': 'Save search',
                'search-context': 'Search for context of this task',
                'search-project': 'Search for project of this task',
                'clear-search': 'Clear the search',
@@ -58,14 +59,15 @@
                'del-left': 'Delete to the left',
                'del-right': 'Delete to the right',
                'del-to-bol': 'Delete to start of line',
                'submit-input': 'Apply changes',
                'select-file': 'Select file',
                'delegate': 'Delegate task',
                'delete': 'Delete task',
+               'archive': 'Archive task',
                'refresh-screen': 'Refresh screen',
                'reload-tasks': 'Reload todo files',
                'comp-next': 'Next completion option',
                'comp-prev': 'Previous completion option',
                'comp-use': 'Use selected completion option',
                'comp-close': 'Close the completion list',
                'prio-a': 'Set priority to (A)',
@@ -1265,14 +1267,16 @@
                                          common.SETTING_SCROLL_MARGIN)
         self.safe_save = conf.bool(common.SETTING_GROUP_GENERAL,
                                    common.SETTING_SAFE_SAVE, 'y')
         self.use_completion = conf.bool(common.SETTING_GROUP_GENERAL,
                                         common.SETTING_USE_COMPLETION, 'y')
         self.tab_cycles = conf.bool(common.SETTING_GROUP_GENERAL,
                                         common.SETTING_TAB_CYCLES, 'y')
+
+        # delete behaviour
         self.trash_file = conf.path(common.SETTING_GROUP_GENERAL,
                                     common.SETTING_TRASHFILE,
                                     common.DEFAULT_TRASHFILE);
         self.delete_is = conf.get(common.SETTING_GROUP_GENERAL,
                                   common.SETTING_DELETE_IS,
                                   common.DELETE_OPTION_DISABLED)
         if self.delete_is not in common.DELETE_OPTIONS:
@@ -1294,14 +1298,32 @@
             try:
                 with open(self.trash_file, 'a', encoding='utf-8'):
                     logging.debug(f"Using trash file {self.trash_file}")
             except OSError as exc:
                 logging.error(f"Could not open trash file '{self.trash_file}': {exc}")
                 self.delete_is = common.DELETE_OPTION_DISABLED
 
+        # archive behaviour
+        self.archive_file = conf.path(common.SETTING_GROUP_GENERAL,
+                                      common.SETTING_ARCHIVE_FILE,
+                                      common.DEFAULT_ARCHIVE)
+        self.archive_is = conf.get(common.SETTING_GROUP_GENERAL,
+                                   common.SETTING_ARCHIVE_IS,
+                                   common.ARCHIVE_OPTION_CENTRALISED)
+        if self.archive_is not in common.ARCHIVE_OPTIONS:
+            logging.error(f"Configuration option 'archive-is' ('{self.archive_is}') is invalid.")
+            self.archive_is = common.ARCHIVE_OPTION_DISABLED
+
+        if self.archive_is == common.ARCHIVE_OPTION_CENTRALISED:
+            try:
+                self.archive_file.parent.mkdir(parents=True, exist_ok=True)
+            except OSError as exc:
+                logging.error(f"Could not create path to archive file '{self.archive_file}': {exc}")
+                self.archive_is = common.ARCHIVE_OPTION_DISABLED
+
         # external editor
         self.external_editor = self.conf.get(common.SETTING_GROUP_GENERAL,
                                              common.SETTING_EXT_EDITOR)
 
         # protocols accepted to open with open-url
         self.protos = conf.list(common.SETTING_GROUP_GENERAL,
                                 common.SETTING_PROTOCOLS)
@@ -1350,14 +1372,15 @@
             ('A',): 'prio-a',
             ('B',): 'prio-b',
             ('C',): 'prio-c',
             ('D',): 'prio-d',
             ('+',): 'prio-up',
             ('-',): 'prio-down',
             ('=',): 'prio-none',
+            ('%',): 'archive',
             }
         self.editor_key_mapping = {
             '^C': 'cancel',
             '<escape>': 'cancel',
             '<left>': 'go-left',
             '<right>': 'go-right',
             '<tab>': 'goto-empty',
@@ -1393,24 +1416,26 @@
             'load-template': self.do_load_template,
             'save-template': self.do_save_template,
             'load-search': self.do_load_search,
             'save-search': self.do_save_search,
             'clear-search': self.do_clear_search,
             'edit-task': self.do_edit_task,
             'edit-external': self.do_edit_task_external,
+            'edit-file-external': self.do_edit_file_external,
             'create-task': self.do_create_task,
             'jump-to': self.do_jump_to,
             'open-url': self.do_open_url,
             'toggle-tracking': self.do_toggle_tracking,
             'toggle-done': self.do_toggle_done,
             'toggle-hidden': self.do_toggle_hidden,
             'show-help': self.do_show_help,
             'delegate': self.do_delegate,
             'open-manual': utils.open_manual,
             'delete-task': self.do_delete,
+            'archive': self.do_archive,
             'show-related': self.do_show_related,
             'prio-up': self.do_prio_up,
             'prio-down': self.do_prio_down,
             'prio-none': lambda: self.do_set_prio(None),
             'prio-a': lambda: self.do_set_prio('A'),
             'prio-b': lambda: self.do_set_prio('B'),
             'prio-c': lambda: self.do_set_prio('C'),
@@ -2015,25 +2040,60 @@
 
         with tempfile.NamedTemporaryFile("w+t", encoding="utf-8", suffix='.txt') as fh:
             fh.write(str(task.task))
             fh.flush()
             with ShellContext(self.screen, True):
                 subprocess.run(editor + [fh.name])
 
-            # only actually apply changes when editing the 'extra' tags
             fh.flush()
             fh.seek(0)
             tasktext = fh.read()
 
         tasktext = utils.dehumanize_dates(utils.auto_task_id(self.sources, tasktext))
         if tasktext != str(task.task):
             self.modify_task(task, lambda t: t.parse(tasktext))
 
         self.paint(True)
 
+    def do_edit_file_external(self):
+        taskline = self.tasks.selected_item
+        if taskline is None:
+            self.error(tr("No task selected"))
+            return
+
+        editor = self.resolve_editor()
+        if editor is None:
+            self.error(tr("Could not determine your external text editor"))
+            return
+
+        todotxt = taskline.source.source
+        tasks = todotxt.tasks[:]
+        with tempfile.NamedTemporaryFile("w+b", suffix='.txt') as fh:
+            todotxt.write_to_stream(fh, todotxt.linesep)
+            fh.flush()
+            with ShellContext(self.screen, True):
+                subprocess.run(editor + [fh.name])
+
+            fh.flush()
+            fh.seek(0)
+            parser = TodoTxtParser()
+            tasks = parser.parse_stream(fh)
+
+        todotxt.tasks = []
+        for task in tasks:
+            # one by one to make sure `auto_task_id` actually works
+            task = Task(utils.dehumanize_dates(utils.auto_task_id(self.sources, str(task))))
+            todotxt.add(task)
+            taskline.source.update_from_task(task)
+        taskline.source.save(safe=self.safe_save)
+        taskline.source.parse()
+        self.search.update_sources(self.sources)
+        self.update_tasks()
+        self.paint(True)
+
     def do_create_task(self):
         self.focus.append(TaskCreator(self.tasks))
         self.paint()
 
     def do_jump_to(self, init=''):
         if len(self.focus) == 0:
             return
@@ -2237,51 +2297,121 @@
                                        contexts,
                                        lambda c: self.set_search('@'+c),
                                        title="Select Context",
                                        numbered=True))
             self.paint(True)
 
     def do_delete(self):
+        if self.delete_is == common.DELETE_OPTION_DISABLED:
+            return
+
         taskline = self.tasks.selected_item
         if taskline is None:
             return
 
         def _do_delete(t):
             t.todotxt.tasks.remove(t)
             t.parse("")
 
         can_perm_delete = self.last_perm_delete + self.perm_delete_timeout < datetime.datetime.now()
 
-        if self.delete_is == common.DELETE_OPTION_DISABLED:
-            return
-
-        elif self.delete_is == common.DELETE_OPTION_PERMANENT and can_perm_delete:
+        if self.delete_is == common.DELETE_OPTION_PERMANENT and can_perm_delete:
             success, _ = self.modify_task(taskline, _do_delete)
             if success:
                 self.last_perm_delete = datetime.datetime.now()
                 self.info(tr("Task deleted"))
                 self.tasks.paint(True)
 
         elif self.delete_is == common.DELETE_OPTION_TRASH:
             # first save the task in the trash
             trashfile = TodoTxt(self.trash_file)
-            trashfile.parse()
+            try:
+                trashfile.parse()
+            except OSError as exc:
+                logging.error(f"Failed to open {trashfile.filename}: {exc}")
+                self.error(tr("Could not access the trash file"))
+                return
             trashfile.tasks.append(taskline.task)
-            trashfile.save()
+            try:
+                trashfile.save()
+            except OSError as exc:
+                logging.error(f"Failed to save to {trashfile.filename}: {exc}")
+                self.error(tr("Could not write to the trash file"))
+                return
 
             # attempt to delete the task
             success, _ = self.modify_task(taskline, _do_delete)
             if success:
                 self.info(tr("Task moved to trash"))
                 self.tasks.paint(True)
             else:
                 # deletion was not okay, remove the task again from the trash
                 trashfile.tasks.pop()
                 trashfile.save()
 
+        else:
+            self.error(tr("Configuration option 'delete-is' is not valid."))
+
+    def do_archive(self):
+        if self.archive_is == common.ARCHIVE_OPTION_DISABLED:
+            return
+
+        taskline = self.tasks.selected_item
+        if taskline is None:
+            return
+
+        if self.archive_is == common.ARCHIVE_OPTION_CENTRALISED:
+            archivefile = self.archive_file
+        elif self.archive_is == common.ARCHIVE_OPTION_RELATIVE:
+            archivefile = taskline.source.filename.parent / "archive.txt"
+        else:
+            self.error(tr("Configuration option 'archive-is' is not valid."))
+            return
+
+        if archivefile == taskline.source.filename:
+            self.error(tr("This task is already in the archive."))
+            return
+
+        try:
+            with open(archivefile, 'a+b'):
+                logging.debug(f"Using archive file {archivefile}")
+        except OSError as exc:
+            self.error(tr("Could not open archive file for writing"))
+            logging.error(f"Could not open archive file '{archivefile}' "
+                          f"for writing: {exc}")
+            return
+
+        archivefile = TodoTxt(archivefile)
+        try:
+            archivefile.parse()
+        except OSError as exc:
+            self.error(tr("Failed to access archive file"))
+            logging.error(f"Failed to read archive file {archivefile.filename}: {exc}")
+            return
+        archivefile.tasks.append(taskline.task)
+        try:
+            archivefile.save()
+        except OSError as exc:
+            self.error(tr("Could not write to archive file"))
+            logging.error(f"Failed to write to archive file {archivefile.filename}: {exc}")
+            return
+
+        def _do_delete(t):
+            t.todotxt.tasks.remove(t)
+            t.parse("")
+
+        success, _ = self.modify_task(taskline, _do_delete)
+        if success:
+            self.info(tr("Task moved to archive"))
+            self.tasks.paint(True)
+        else:
+            # task deletion failed, don't duplicate the task in the archive
+            archivefile.tasks.pop()
+            archivefile.save()
+
     def add_to_search(self, text):
         if len(self.search.text) > 0:
             text = ' ' + text
         self.set_search(self.search.text + text)
 
     def do_search_project(self):
         task = self.tasks.selected_item
```

### Comparing `pter-3.7.0/pter/docs/pter.html` & `pter-3.8.0/pter/docs/pter.html`

 * *Files 2% similar despite different names*

#### Comparing `pter-3.7.0/pter/docs/pter.html` & `pter-3.8.0/pter/docs/pter.html`

```diff
@@ -1,15 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE html
   PUBLIC '-//W3C//DTD XHTML 1.0 Transitional//EN'
   'http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd'>
 <html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
-    <meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/"/>
+    <meta name="generator" content="Docutils 0.20.1: https://docutils.sourceforge.io/"/>
     <title>pter</title>
     <style type="text/css">/*
 :Author: David Goodger (goodger@python.org)
 :Id: $Id: html4css1.css 8954 2022-01-20 10:10:25Z milde $
 :Copyright: This stylesheet has been placed in the public domain.
 
 Default cascading style sheet for the HTML output of Docutils.
@@ -936,29 +936,93 @@
               </dd>
               <dt>
                 <tt class="docutils literal">
                   <span class="pre">trash-file</span>
                 </tt>
               </dt>
               <dd>
-                What your trash file is. This option is only used if
+                Where your trash file is. This option is only used if
                 <tt class="docutils literal">
                   <span class="pre">delete-is</span>
                 </tt>
                 is
 set to
                 <tt class="docutils literal">trash</tt>
                 . Defaults to
                 <tt class="docutils literal">
                   <span class="pre">~/.config/pter/trash.txt</span>
                 </tt>
                 .
               </dd>
               <dt>
                 <tt class="docutils literal">
+                  <span class="pre">archive-is</span>
+                </tt>
+              </dt>
+              <dd>
+                <p class="first">
+                  Defines the behaviour of the
+                  <tt class="docutils literal">archive</tt>
+                  function. Can be one of these:
+                </p>
+                <blockquote>
+                  <ul class="simple">
+                    <li>
+                      <tt class="docutils literal">relative</tt>
+                      , the archive file is assumed to be in the same place as
+the
+                      <tt class="docutils literal">todo.txt</tt>
+                      file, but called
+                      <tt class="docutils literal">archive.txt</tt>
+                      ,
+                    </li>
+                    <li>
+                      <tt class="docutils literal">centralised</tt>
+                      , there is only one archive file for all
+                      <tt class="docutils literal">todo.txt</tt>
+                      files. Its location is controlled by
+                      <tt class="docutils literal">
+                        <span class="pre">archive-file</span>
+                      </tt>
+                      ,
+                    </li>
+                    <li>
+                      <tt class="docutils literal">disabled</tt>
+                      , there is no archiving.
+                    </li>
+                  </ul>
+                </blockquote>
+                <p class="last">
+                  Defaults to
+                  <tt class="docutils literal">centralised</tt>
+                  .
+                </p>
+              </dd>
+              <dt>
+                <tt class="docutils literal">
+                  <span class="pre">archive-file</span>
+                </tt>
+              </dt>
+              <dd>
+                Where your archive file is. This file will be used to receive archived
+tasks if the
+                <tt class="docutils literal">
+                  <span class="pre">archive-is</span>
+                </tt>
+                option is set to
+                <tt class="docutils literal">centralised</tt>
+                . Defaults
+to
+                <tt class="docutils literal">
+                  <span class="pre">~/.config/pter/archive.txt</span>
+                </tt>
+                .
+              </dd>
+              <dt>
+                <tt class="docutils literal">
                   <span class="pre">reuse-recurring</span>
                 </tt>
               </dt>
               <dd>
                 <p class="first">
                   Reuse existing recurring task entry instead of creating a new one. If
 set, completing a task with a
@@ -1178,25 +1242,35 @@
                 <tt class="docutils literal">
                   <span class="pre">edit-external</span>
                 </tt>
                 : edit the selected task in an external text editor
               </li>
               <li>
                 <tt class="docutils literal">
+                  <span class="pre">edit-file-external</span>
+                </tt>
+                : edit the todo.txt of the selected task in an external editor
+              </li>
+              <li>
+                <tt class="docutils literal">
                   <span class="pre">delete-task</span>
                 </tt>
                 : delete the selected task or move it to trash, depends
 on the configuration option
                 <tt class="docutils literal">
                   <span class="pre">delete-is</span>
                 </tt>
                 (by default not bound to any
 key)
               </li>
               <li>
+                <tt class="docutils literal">archive</tt>
+                : move the selected task to the designated archive file
+              </li>
+              <li>
                 <tt class="docutils literal">
                   <span class="pre">load-search</span>
                 </tt>
                 : show the saved searches to load one
               </li>
               <li>
                 <tt class="docutils literal">
@@ -2192,14 +2266,34 @@
               <li>&quot;l&quot;: load a named search</li>
               <li>&quot;s&quot;: save the current search</li>
               <li>&quot;L&quot;: load a named task template</li>
               <li>&quot;S&quot;: Save a task as a named template</li>
               <li>&quot;u&quot;: open a URL listed in the selected task</li>
               <li>&quot;t&quot;: Start/stop time tracking of the selected task</li>
               <li>&quot;&gt;&quot;: Delegate the selected task</li>
+              <li>
+                &quot;A&quot;: Set the priority of this task to
+                <tt class="docutils literal">(A)</tt>
+              </li>
+              <li>
+                &quot;B&quot;: Set the priority of this task to
+                <tt class="docutils literal">(B)</tt>
+              </li>
+              <li>
+                &quot;C&quot;: Set the priority of this task to
+                <tt class="docutils literal">(C)</tt>
+              </li>
+              <li>
+                &quot;D&quot;: Set the priority of this task to
+                <tt class="docutils literal">(D)</tt>
+              </li>
+              <li>&quot;+&quot;: Increase the priority of this task</li>
+              <li>&quot;-&quot;: Decrease the priority of this task</li>
+              <li>&quot;=&quot;: Remove the priority of this task</li>
+              <li>&quot;%&quot;: Move this task into the archive</li>
             </ul>
           </blockquote>
           <p>In edit fields the following keyboard controls are available:</p>
           <blockquote>
             <ul class="simple">
               <li>&quot;←&quot;, &quot;→&quot; (cursor keys): move the cursor one character to the left or right</li>
               <li>&quot;Home&quot;: move the cursor to the first charater</li>
```

### Comparing `pter-3.7.0/pter/icons/qpter_16x16.png` & `pter-3.8.0/pter/icons/qpter_16x16.png`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/pter/icons/qpter_32x32.png` & `pter-3.8.0/pter/icons/qpter_32x32.png`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/pter/key.py` & `pter-3.8.0/pter/key.py`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/pter/main.py` & `pter-3.8.0/pter/main.py`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/pter/qtui.py` & `pter-3.8.0/pter/qtui.py`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/pter/searcher.py` & `pter-3.8.0/pter/searcher.py`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/pter/source.py` & `pter-3.8.0/pter/source.py`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/pter/utils.py` & `pter-3.8.0/pter/utils.py`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/pter.egg-info/PKG-INFO` & `pter-3.8.0/pter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pter
-Version: 3.7.0
+Version: 3.8.0
 Summary: Console UI to manage your todo.txt file(s).
 Home-page: https://vonshednob.cc/pter
 Author: R
 Author-email: contact+pter@vonshednob.cc
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console :: Curses
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `pter-3.7.0/pter.egg-info/SOURCES.txt` & `pter-3.8.0/pter.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 doc/pter-demo.gif
 doc/pter.rst
 doc/qpter.png
 extras/example.conf
 extras/pter.desktop
 extras/qpter.desktop
```

### Comparing `pter-3.7.0/setup.py` & `pter-3.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/tests/test_displaynames.py` & `pter-3.8.0/tests/test_displaynames.py`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/tests/test_priochange.py` & `pter-3.8.0/tests/test_priochange.py`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/tests/test_pter.py` & `pter-3.8.0/tests/test_pter.py`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/tests/test_rec.py` & `pter-3.8.0/tests/test_rec.py`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/tests/test_searcher.py` & `pter-3.8.0/tests/test_searcher.py`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/tests/test_sorting.py` & `pter-3.8.0/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `pter-3.7.0/tests/test_taskid.py` & `pter-3.8.0/tests/test_taskid.py`

 * *Files identical despite different names*

