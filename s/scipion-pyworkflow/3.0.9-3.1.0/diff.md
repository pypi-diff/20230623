# Comparing `tmp/scipion-pyworkflow-3.0.9.tar.gz` & `tmp/scipion-pyworkflow-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-pyworkflow-3.0.9.tar", last modified: Mon Feb  1 09:45:05 2021, max compression
+gzip compressed data, was "scipion-pyworkflow-3.1.0.tar", last modified: Fri Jun 23 15:09:55 2023, max compression
```

## Comparing `scipion-pyworkflow-3.0.9.tar` & `scipion-pyworkflow-3.1.0.tar`

### file list

```diff
@@ -1,270 +1,268 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.612883 scipion-pyworkflow-3.0.9/
--rw-r--r--   0 runner    (1001) docker     (122)    35148 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      251 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4022 2021-02-01 09:45:05.612883 scipion-pyworkflow-3.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2243 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.588883 scipion-pyworkflow-3.0.9/pyworkflow/
--rw-r--r--   0 runner    (1001) docker     (122)     1246 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.588883 scipion-pyworkflow-3.0.9/pyworkflow/apps/
--rw-r--r--   0 runner    (1001) docker     (122)     1187 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1356 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     1829 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_plot.py
--rw-r--r--   0 runner    (1001) docker     (122)     3055 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_project.py
--rw-r--r--   0 runner    (1001) docker     (122)     5368 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1952 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_mpirun.py
--rw-r--r--   0 runner    (1001) docker     (122)     2707 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_remote.py
--rw-r--r--   0 runner    (1001) docker     (122)     1635 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_run.py
--rw-r--r--   0 runner    (1001) docker     (122)    11868 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (122)     9040 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_schedule_run.py
--rw-r--r--   0 runner    (1001) docker     (122)     1443 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_sleep.py
--rw-r--r--   0 runner    (1001) docker     (122)    16530 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_sync_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     2595 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_viewer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8393 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     4464 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)      507 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.588883 scipion-pyworkflow-3.0.9/pyworkflow/gui/
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23402 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/browser.py
--rw-r--r--   0 runner    (1001) docker     (122)    36994 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/canvas.py
--rw-r--r--   0 runner    (1001) docker     (122)    27922 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/dialog.py
--rw-r--r--   0 runner    (1001) docker     (122)   106438 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/form.py
--rw-r--r--   0 runner    (1001) docker     (122)     8810 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     9856 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/graph_layout.py
--rw-r--r--   0 runner    (1001) docker     (122)    16949 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/gui.py
--rw-r--r--   0 runner    (1001) docker     (122)     7086 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/matplotlib_image.py
--rw-r--r--   0 runner    (1001) docker     (122)     8116 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/plotter.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.588883 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/
--rw-r--r--   0 runner    (1001) docker     (122)     1118 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7694 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1852 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     7251 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/labels.py
--rw-r--r--   0 runner    (1001) docker     (122)    18168 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/project.py
--rw-r--r--   0 runner    (1001) docker     (122)     3057 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    19468 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/viewdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    21347 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/viewprojects.py
--rw-r--r--   0 runner    (1001) docker     (122)   109042 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/project/viewprotocols.py
--rw-r--r--   0 runner    (1001) docker     (122)    27645 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/text.py
--rw-r--r--   0 runner    (1001) docker     (122)     8531 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/tooltip.py
--rw-r--r--   0 runner    (1001) docker     (122)    22023 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/tree.py
--rw-r--r--   0 runner    (1001) docker     (122)    10761 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/gui/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.592883 scipion-pyworkflow-3.0.9/pyworkflow/mapper/
--rw-r--r--   0 runner    (1001) docker     (122)     1219 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7354 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/mapper/mapper.py
--rw-r--r--   0 runner    (1001) docker     (122)    54781 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/mapper/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (122)     4724 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/mapper/sqlite_db.py
--rw-r--r--   0 runner    (1001) docker     (122)    10720 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/mapper/xmlmapper.py
--rw-r--r--   0 runner    (1001) docker     (122)    48759 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/object.py
--rw-r--r--   0 runner    (1001) docker     (122)    25158 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.592883 scipion-pyworkflow-3.0.9/pyworkflow/project/
--rw-r--r--   0 runner    (1001) docker     (122)     1384 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11818 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6706 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    67249 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/project.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.592883 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (122)     2580 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/clean_projects.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2921 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2488 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/create.py
--rw-r--r--   0 runner    (1001) docker     (122)     2909 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/edit_workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      890 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/fix_links.py
--rw-r--r--   0 runner    (1001) docker     (122)     2685 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/load.py
--rw-r--r--   0 runner    (1001) docker     (122)     2564 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/refresh.py
--rw-r--r--   0 runner    (1001) docker     (122)     3461 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/schedule.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      901 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/stack2volume.py
--rw-r--r--   0 runner    (1001) docker     (122)     2452 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/stop.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.592883 scipion-pyworkflow-3.0.9/pyworkflow/protocol/
--rw-r--r--   0 runner    (1001) docker     (122)     1413 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2122 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (122)     2976 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    14633 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/executor.py
--rw-r--r--   0 runner    (1001) docker     (122)    11869 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/hosts.py
--rw-r--r--   0 runner    (1001) docker     (122)     9256 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/launch.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/package.py
--rw-r--r--   0 runner    (1001) docker     (122)    23108 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/params.py
--rw-r--r--   0 runner    (1001) docker     (122)    85721 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/protocol/protocol.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.604883 scipion-pyworkflow-3.0.9/pyworkflow/resources/
--rw-r--r--   0 runner    (1001) docker     (122)     6187 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/ChimeraLogoSmall.gif
--rw-r--r--   0 runner    (1001) docker     (122)     6798 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/I2PC.gif
--rw-r--r--   0 runner    (1001) docker     (122)    64364 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/background_section.gif
--rw-r--r--   0 runner    (1001) docker     (122)      987 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/bookmark.gif
--rw-r--r--   0 runner    (1001) docker     (122)     3771 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/ccp4_200.gif
--rw-r--r--   0 runner    (1001) docker     (122)      161 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/class_obj.gif
--rw-r--r--   0 runner    (1001) docker     (122)    16491 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/cryoem_logo.gif
--rw-r--r--   0 runner    (1001) docker     (122)    34177 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/cryomethods_logo.gif
--rw-r--r--   0 runner    (1001) docker     (122)       99 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/debug.gif
--rw-r--r--   0 runner    (1001) docker     (122)      586 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/doc_icon.gif
--rw-r--r--   0 runner    (1001) docker     (122)      418 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/download_icon.gif
--rw-r--r--   0 runner    (1001) docker     (122)    27027 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/error_page.jpg
--rw-r--r--   0 runner    (1001) docker     (122)      103 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-arrow-left.gif
--rw-r--r--   0 runner    (1001) docker     (122)      105 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-arrow-up.gif
--rw-r--r--   0 runner    (1001) docker     (122)       83 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-ban.gif
--rw-r--r--   0 runner    (1001) docker     (122)       67 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-bars.gif
--rw-r--r--   0 runner    (1001) docker     (122)       73 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-check.gif
--rw-r--r--   0 runner    (1001) docker     (122)       72 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-checked.gif
--rw-r--r--   0 runner    (1001) docker     (122)      343 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-cog.gif
--rw-r--r--   0 runner    (1001) docker     (122)       87 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-cogs.gif
--rw-r--r--   0 runner    (1001) docker     (122)       78 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-database.gif
--rw-r--r--   0 runner    (1001) docker     (122)       92 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-delete-operation.gif
--rw-r--r--   0 runner    (1001) docker     (122)       75 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-download.gif
--rw-r--r--   0 runner    (1001) docker     (122)      257 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-exclamation-triangle_alert.gif
--rw-r--r--   0 runner    (1001) docker     (122)       77 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-external-link.gif
--rw-r--r--   0 runner    (1001) docker     (122)       78 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-eye.gif
--rw-r--r--   0 runner    (1001) docker     (122)       89 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-failure.gif
--rw-r--r--   0 runner    (1001) docker     (122)       78 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-file-o.gif
--rw-r--r--   0 runner    (1001) docker     (122)       82 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-files-o.gif
--rw-r--r--   0 runner    (1001) docker     (122)       76 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-folder-open.gif
--rw-r--r--   0 runner    (1001) docker     (122)      113 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-home.gif
--rw-r--r--   0 runner    (1001) docker     (122)       84 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-iconmoon-link.gif
--rw-r--r--   0 runner    (1001) docker     (122)      266 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-info-circle_alert.gif
--rw-r--r--   0 runner    (1001) docker     (122)       66 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-install.gif
--rw-r--r--   0 runner    (1001) docker     (122)       90 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-installed.gif
--rw-r--r--   0 runner    (1001) docker     (122)       74 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-laptop.gif
--rw-r--r--   0 runner    (1001) docker     (122)       77 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-lightbulb-o.gif
--rw-r--r--   0 runner    (1001) docker     (122)       76 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-list-ul.gif
--rw-r--r--   0 runner    (1001) docker     (122)       79 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-magic.gif
--rw-r--r--   0 runner    (1001) docker     (122)       67 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-minus-square.gif
--rw-r--r--   0 runner    (1001) docker     (122)       75 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-next.gif
--rw-r--r--   0 runner    (1001) docker     (122)       74 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-paint-brush.gif
--rw-r--r--   0 runner    (1001) docker     (122)       79 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-pencil.gif
--rw-r--r--   0 runner    (1001) docker     (122)       91 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-play-circle-o.gif
--rw-r--r--   0 runner    (1001) docker     (122)      110 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-plus-circle.gif
--rw-r--r--   0 runner    (1001) docker     (122)       73 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-plus-square.gif
--rw-r--r--   0 runner    (1001) docker     (122)       75 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-previous.gif
--rw-r--r--   0 runner    (1001) docker     (122)       88 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-processing.gif
--rw-r--r--   0 runner    (1001) docker     (122)       79 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-question-circle.gif
--rw-r--r--   0 runner    (1001) docker     (122)       77 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-refresh.gif
--rw-r--r--   0 runner    (1001) docker     (122)       77 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-rocket.gif
--rw-r--r--   0 runner    (1001) docker     (122)       82 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-save.gif
--rw-r--r--   0 runner    (1001) docker     (122)       79 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-search.gif
--rw-r--r--   0 runner    (1001) docker     (122)       78 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-sign-in.gif
--rw-r--r--   0 runner    (1001) docker     (122)       79 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-sign-out.gif
--rw-r--r--   0 runner    (1001) docker     (122)       76 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-sitemap.gif
--rw-r--r--   0 runner    (1001) docker     (122)       91 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-stop-workflow.gif
--rw-r--r--   0 runner    (1001) docker     (122)       73 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-stop.gif
--rw-r--r--   0 runner    (1001) docker     (122)      691 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-tags.gif
--rw-r--r--   0 runner    (1001) docker     (122)      277 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-times-circle_alert.gif
--rw-r--r--   0 runner    (1001) docker     (122)       76 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-times.gif
--rw-r--r--   0 runner    (1001) docker     (122)       87 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-to_install.gif
--rw-r--r--   0 runner    (1001) docker     (122)       81 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-trash-o.gif
--rw-r--r--   0 runner    (1001) docker     (122)       70 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-unchecked.gif
--rw-r--r--   0 runner    (1001) docker     (122)       76 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-undo.gif
--rw-r--r--   0 runner    (1001) docker     (122)       68 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-uninstall.gif
--rw-r--r--   0 runner    (1001) docker     (122)       76 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-update.gif
--rw-r--r--   0 runner    (1001) docker     (122)       75 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/fa-upload.gif
--rw-r--r--   0 runner    (1001) docker     (122)      718 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/favicon.gif
--rw-r--r--   0 runner    (1001) docker     (122)     1150 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)     3808 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file.gif
--rw-r--r--   0 runner    (1001) docker     (122)      216 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_folder.gif
--rw-r--r--   0 runner    (1001) docker     (122)      340 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_generic.gif
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_image.gif
--rw-r--r--   0 runner    (1001) docker     (122)      570 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_java.gif
--rw-r--r--   0 runner    (1001) docker     (122)      249 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_log.gif
--rw-r--r--   0 runner    (1001) docker     (122)      564 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_md.gif
--rw-r--r--   0 runner    (1001) docker     (122)      544 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_python.gif
--rw-r--r--   0 runner    (1001) docker     (122)      545 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_sqlite.gif
--rw-r--r--   0 runner    (1001) docker     (122)      104 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_stack.gif
--rw-r--r--   0 runner    (1001) docker     (122)      561 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_text.gif
--rw-r--r--   0 runner    (1001) docker     (122)     1072 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/file_vol.gif
--rw-r--r--   0 runner    (1001) docker     (122)    16824 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/loading.gif
--rw-r--r--   0 runner    (1001) docker     (122)      876 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/logoInstruct.gif
--rw-r--r--   0 runner    (1001) docker     (122)     4345 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/logo_cnb_without_title.gif
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/logo_i2pc_with_title.gif
--rw-r--r--   0 runner    (1001) docker     (122)      465 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/newProt.gif
--rw-r--r--   0 runner    (1001) docker     (122)    16902 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/no-image.gif
--rw-r--r--   0 runner    (1001) docker     (122)     3660 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/no-image.jpg
--rw-r--r--   0 runner    (1001) docker     (122)     6923 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/no-image128.gif
--rw-r--r--   0 runner    (1001) docker     (122)    28320 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/phenix.gif
--rw-r--r--   0 runner    (1001) docker     (122)      343 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/prot_disabled.gif
--rw-r--r--   0 runner    (1001) docker     (122)      544 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/python_file.gif
--rw-r--r--   0 runner    (1001) docker     (122)     1176 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/question.gif
--rw-r--r--   0 runner    (1001) docker     (122)       83 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/rename.gif
--rw-r--r--   0 runner    (1001) docker     (122)       68 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/root.gif
--rw-r--r--   0 runner    (1001) docker     (122)    42677 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_bn.gif
--rw-r--r--   0 runner    (1001) docker     (122)     1428 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon.gif
--rw-r--r--   0 runner    (1001) docker     (122)   126140 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon.svg
--rw-r--r--   0 runner    (1001) docker     (122)     3900 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon_proj.gif
--rw-r--r--   0 runner    (1001) docker     (122)     6251 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon_projs.gif
--rw-r--r--   0 runner    (1001) docker     (122)     4878 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon_prot.gif
--rw-r--r--   0 runner    (1001) docker     (122)     1004 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_logo.gif
--rw-r--r--   0 runner    (1001) docker     (122)    13219 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_logo_normal.gif
--rw-r--r--   0 runner    (1001) docker     (122)     2958 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_logo_small.gif
--rw-r--r--   0 runner    (1001) docker     (122)     3725 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_logo_small_web.gif
--rw-r--r--   0 runner    (1001) docker     (122)     3304 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_logo_transparent.gif
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.608883 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/arrowDown.png
--rw-r--r--   0 runner    (1001) docker     (122)      276 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/arrowUp.png
--rw-r--r--   0 runner    (1001) docker     (122)   284666 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/background_section.png
--rw-r--r--   0 runner    (1001) docker     (122)      208 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/colRowModeOff.png
--rw-r--r--   0 runner    (1001) docker     (122)      180 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/colRowModeOn.png
--rw-r--r--   0 runner    (1001) docker     (122)      624 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/delete.png
--rw-r--r--   0 runner    (1001) docker     (122)     1015 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/doc_icon.png
--rw-r--r--   0 runner    (1001) docker     (122)      792 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/download_icon.png
--rw-r--r--   0 runner    (1001) docker     (122)      493 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/enabled_gallery.png
--rw-r--r--   0 runner    (1001) docker     (122)      173 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/galleryViewOff.png
--rw-r--r--   0 runner    (1001) docker     (122)      159 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/galleryViewOn.png
--rw-r--r--   0 runner    (1001) docker     (122)      451 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/goto.png
--rw-r--r--   0 runner    (1001) docker     (122)     2736 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/menu.png
--rw-r--r--   0 runner    (1001) docker     (122)      288 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/separator.png
--rw-r--r--   0 runner    (1001) docker     (122)      200 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/tableViewOff.png
--rw-r--r--   0 runner    (1001) docker     (122)      172 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/tableViewOn.png
--rw-r--r--   0 runner    (1001) docker     (122)      262 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (122)      332 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 runner    (1001) docker     (122)      280 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (122)      751 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/volumeOff.png
--rw-r--r--   0 runner    (1001) docker     (122)      614 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/volumeOn.png
--rw-r--r--   0 runner    (1001) docker     (122)      118 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/resources/users.gif
--rw-r--r--   0 runner    (1001) docker     (122)     8702 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/template.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.608883 scipion-pyworkflow-3.0.9/pyworkflow/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    12576 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      493 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10673 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/tests/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.608883 scipion-pyworkflow-3.0.9/pyworkflow/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     1429 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14943 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     3442 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/echo.py
--rw-r--r--   0 runner    (1001) docker     (122)    31140 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/file_transfer.py
--rw-r--r--   0 runner    (1001) docker     (122)     5365 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/graph.py
--rw-r--r--   0 runner    (1001) docker     (122)     4636 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     5703 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/mpi.py
--rw-r--r--   0 runner    (1001) docker     (122)    14765 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (122)     4349 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (122)     2218 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (122)     5345 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (122)    18461 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/properties.py
--rw-r--r--   0 runner    (1001) docker     (122)     4189 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/reflection.py
--rw-r--r--   0 runner    (1001) docker     (122)     7399 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/remote.py
--rw-r--r--   0 runner    (1001) docker     (122)    24116 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     8534 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/utils/which.py
--rw-r--r--   0 runner    (1001) docker     (122)    10941 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.608883 scipion-pyworkflow-3.0.9/pyworkflow/webservices/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/webservices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      575 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/webservices/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     6242 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/webservices/notifier.py
--rw-r--r--   0 runner    (1001) docker     (122)     2365 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/webservices/repository.py
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflow/wizard.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.608883 scipion-pyworkflow-3.0.9/pyworkflowtests/
--rw-r--r--   0 runner    (1001) docker     (122)     1616 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2102 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (122)    28478 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/objects.py
--rw-r--r--   0 runner    (1001) docker     (122)     4460 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.612883 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2685 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_canvas.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1624 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (122)     4272 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (122)    13558 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_mappers.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    14592 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_object.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_project.py
--rw-r--r--   0 runner    (1001) docker     (122)     2430 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_protocol_execution.py
--rw-r--r--   0 runner    (1001) docker     (122)     3291 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_protocol_export.py
--rw-r--r--   0 runner    (1001) docker     (122)     5755 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_protocol_output.py
--rw-r--r--   0 runner    (1001) docker     (122)     5544 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      116 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2021-02-01 09:45:05.612883 scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4022 2021-02-01 09:45:05.000000 scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     8734 2021-02-01 09:45:05.000000 scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2021-02-01 09:45:05.000000 scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       55 2021-02-01 09:45:05.000000 scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      117 2021-02-01 09:45:05.000000 scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2021-02-01 09:45:05.000000 scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2021-02-01 09:45:05.612883 scipion-pyworkflow-3.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     9111 2021-02-01 09:44:54.000000 scipion-pyworkflow-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.481531 scipion-pyworkflow-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-23 15:09:55.477531 scipion-pyworkflow-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.437531 scipion-pyworkflow-3.1.0/pyworkflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.441531 scipion-pyworkflow-3.1.0/pyworkflow/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_protocol_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_protocol_mpirun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_protocol_remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_protocol_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10355 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12456 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_schedule_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_sleep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17175 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_sync_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15892 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.445531 scipion-pyworkflow-3.1.0/pyworkflow/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41189 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34490 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110339 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9085 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/graph_layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19186 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/matplotlib_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/plotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.445531 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/searchprotocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/searchrun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5530 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12008 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19471 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/viewdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22545 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/viewprojects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84839 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/viewprotocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21331 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/project/viewprotocols_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28483 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/tooltip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23038 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11157 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/gui/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.445531 scipion-pyworkflow-3.1.0/pyworkflow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7354 2023-06-23 15:09:42.000000 scipion-pyworkflow-3.1.0/pyworkflow/mapper/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60735 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/mapper/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/mapper/sqlite_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/mapper/xmlmapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51658 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28103 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.445531 scipion-pyworkflow-3.1.0/pyworkflow/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6706 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71104 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.449531 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2600 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/clean_projects.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2942 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/edit_workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/fix_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/schedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      941 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/stack2volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/stop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.449531 scipion-pyworkflow-3.1.0/pyworkflow/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16262 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11515 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12213 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95568 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/protocol/protocol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.469531 scipion-pyworkflow-3.1.0/pyworkflow/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/backward-solid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/beta.png
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/binoculares.png
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/bookmark.png
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/broom-solid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/class_obj.png
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/clipboard-regular.png
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/code-branch-solid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/debug.png
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-arrow-down.png
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-arrow-left.png
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-arrow-up.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-ban.png
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-bars.png
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-check.png
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-checked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-cog.png
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-cogs.png
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-database.png
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-delete-operation.png
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-download.png
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-exclamation-triangle_alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-external-link.png
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-eye.png
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-failure.png
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-file-o.png
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-files-o.png
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-folder-open.png
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-home.png
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-info-circle_alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-install.png
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-installed.png
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-lightbulb-o.png
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-list-ul.png
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-magic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-minus-square.png
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-next.png
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-pencil.png
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-play-circle-o.png
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-plus-square.png
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-previous.png
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-processing.png
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-question-circle.png
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-refresh.png
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-rocket.png
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-save.png
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-search.png
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-sign-in.png
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-sign-out.png
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-sitemap.png
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-stop-workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-stop.png
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-tags.png
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-times-circle_alert.png
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-times.png
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-to_install.png
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-trash-o.png
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-unchecked.png
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-undo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-uninstall.png
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-update.png
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/fa-upload.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_folder.png
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_folder_link.png
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_generic.png
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_generic_link.png
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_image.png
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_image_link.png
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_java.png
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_log.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_md.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_md_link.png
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_python.png
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_sqlite.png
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_stack.png
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_stack_link.png
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_text.png
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/file_vol.png
+-rw-r--r--   0 runner    (1001) docker     (123)    16824 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/new.png
+-rw-r--r--   0 runner    (1001) docker     (123)    29510 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/no-image.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13217 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/no-image128.png
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/paste-solid.png
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/power-off-solid.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/production.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/prot_disabled.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/question.png
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/rename.png
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/root.png
+-rw-r--r--   0 runner    (1001) docker     (123)   113916 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_bn.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)   126140 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon_proj.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon_projs.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon_prot.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35151 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_logo_normal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_logo_small.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.473531 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/arrowDown.png
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/arrowUp.png
+-rw-r--r--   0 runner    (1001) docker     (123)   284666 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/background_section.png
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/colRowModeOff.png
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/colRowModeOn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/delete.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/doc_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/download_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/enabled_gallery.png
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/galleryViewOff.png
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/galleryViewOn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/goto.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/menu.png
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/separator.png
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/tableViewOff.png
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/tableViewOn.png
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/volumeOff.png
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/volumeOn.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/updated.png
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/users.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/wait.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/resources/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.473531 scipion-pyworkflow-3.1.0/pyworkflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.473531 scipion-pyworkflow-3.1.0/pyworkflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14943 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5349 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19427 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/reflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26700 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/utils/which.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10966 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.473531 scipion-pyworkflow-3.1.0/pyworkflow/webservices/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/webservices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/webservices/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/webservices/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/webservices/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflow/wizard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.473531 scipion-pyworkflow-3.1.0/pyworkflowtests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26247 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5482 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.477531 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_canvas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1624 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_mappers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18094 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_protocol_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_protocol_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_protocol_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6489 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 15:09:55.477531 scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-23 15:09:55.000000 scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-06-23 15:09:55.000000 scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-23 15:09:55.000000 scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-23 15:09:55.000000 scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-23 15:09:55.000000 scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 15:09:55.000000 scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 15:09:55.481531 scipion-pyworkflow-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    10147 2023-06-23 15:09:43.000000 scipion-pyworkflow-3.1.0/setup.py
```

### Comparing `scipion-pyworkflow-3.0.9/LICENSE.txt` & `scipion-pyworkflow-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/__init__.py` & `scipion-pyworkflow-3.1.0/pyworkflow/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/apps/__init__.py` & `scipion-pyworkflow-3.1.0/pyworkflow/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_manager.py` & `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_manager.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_plot.py` & `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_plot.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_project.py` & `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_project.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 import os
 
 from pyworkflow import Config
 from pyworkflow.project import Manager
 from pyworkflow.gui.project import ProjectWindow
 import pyworkflow.utils as pwutils
 
+import logging
+logger = logging.getLogger(__name__)
 
 def openProject(projectName):
     """ Opens a scipion project:
 
     :param projectName: Name of a existing project to open,
             or "here" to create a project in the current working dir,
             or "last" to open the most recent project
@@ -76,18 +78,20 @@
     elif projName == 'last':  # Get last project
         projects = manager.listProjects()
         if not projects:
             sys.exit("No projects yet, cannot open the last one.")
         projName = projects[0].projName
 
     projPath = manager.getProjectPath(projName)
-    projWindow = ProjectWindow(projPath)
-
-    projWindow.show()
 
+    if os.path.exists(projPath):
+        projWindow = ProjectWindow(projPath)
+        projWindow.show()
+    else:
+        logger.error("Can't open project %s. It does not exist" % projPath)
 
 if __name__ == '__main__':
 
     if len(sys.argv) > 1:
         openProject(sys.argv[1])
     else:
-        print("usage: pw_project.py PROJECT_NAME or here or last")
+        logger.info("usage: pw_project.py PROJECT_NAME or here or last")
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_list.py` & `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_protocol_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,16 +124,16 @@
             print("\n=== ", group, "(%d protocols)\n" % len(prots))
             printProtocols(prots)
 
     elif withDoc:
         for group, prots in iterGroups(protDict):
             print("Package: ", group, "(%d protocols)" % len(prots))
             for p in prots:
-                print("   %s ( %s )" % (p[0], p[1].getClassLabel()))
-                print("      doc: ", p[1].__doc__)
+                print("   %s ( %s ):" % (p[1].getClassLabel(), p[0]))
+                print("    ", p[1].__doc__)
             print("-" * 100)
 
     else:
         if extended:
             formatStr = "{:<15}\t{:<35}\t{:<35}" + "\t{:<20}" * 6
             print(formatStr.format("PACKAGE", "PROTOCOL",
                                    "LABEL", "DOUBLE_INHERITANCE",
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_mpirun.py` & `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_protocol_mpirun.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_remote.py` & `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_protocol_remote.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_protocol_run.py` & `scipion-pyworkflow-3.1.0/pyworkflow/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python
 # **************************************************************************
 # *
 # * Authors:     J.M. De la Rosa Trevin (jmdelarosa@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
@@ -21,23 +20,19 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 """
-This module is responsible for launching protocol executions.
+This module contains utilities functions and classes.
 """
-import sys
 
-if __name__ == '__main__':
-
-    if len(sys.argv) > 2:
-        projPath = sys.argv[1]
-        dbPath = sys.argv[2]
-        protId = int(sys.argv[3])
-        from pyworkflow.protocol import runProtocolMain
-        runProtocolMain(projPath, dbPath, protId)
-        
-    else:
-        from os.path import basename
-        print("usage: %s dbPath protocolID" % basename(sys.argv[0]))
+from .utils import *
+from .path import *
+from .process import *
+from .which import *
+from .graph import *
+from .reflection import *
+from .log import *
+from .properties import *
+from .progressbar import ProgressBar
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_run_tests.py` & `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_run_tests.py`

 * *Files 13% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # **************************************************************************
 
 """
 Run or show the selected tests. Tests can be selected by giving
 the "case", or by giving the paths and file pattern to use for
 searching them.
 """
-from os.path import basename
+from pyworkflow.utils import LoggingConfigurator
 import argparse
 from collections import OrderedDict
 
 import pyworkflow.tests as pwtests
 from pyworkflow import getTestsScript, SCIPION_TESTS_CMD, Config
 
 from pyworkflow.tests import *
@@ -42,15 +42,14 @@
 MODULE = 0
 CLASS = 1
 TEST = 2
 
 
 class Tester:
     def main(self, args=None):
-        print("Running tests....")
 
         # Trigger plugin's variable definition
         Config.getDomain().getPlugins()
 
         parser = argparse.ArgumentParser(prog=self.getTestsCommand(), description=__doc__)
         g = parser.add_mutually_exclusive_group()
         g.add_argument('--run', action='store_true', help='run the selected tests')
@@ -72,78 +71,89 @@
         add('tests', metavar='TEST', nargs='*',
             help='test case from string identifier (module, class or callable)')
         args = parser.parse_args(args)
 
         if not args.run and not args.show and not args.tests:
             sys.exit(parser.format_help())
 
+        # Logging stuff first
+        self.log = args.log
+
+        if self.log:
+            LoggingConfigurator.setupLogging(logFile=self.log)
+        else:
+            logging.basicConfig(level=Config.SCIPION_LOG_LEVEL, format=Config.SCIPION_LOG_FORMAT)
+
+        self.logger = logging.getLogger(__name__)
+
+        # This goes intentionally to the output. Is not a logging line._S
+        print("Running tests....")
+
         testsDict = OrderedDict()
         testLoader = unittest.defaultTestLoader
 
         if args.tests:
             # In this case the tests are passed as argument.
             # The full name of the test will be used to load it.
             testsDict['tests'] = unittest.TestSuite()
             for t in args.tests:
                 try:
                     testsDict['tests'].addTests(testLoader.loadTestsFromName(t))
                 except Exception as e:
-                    print('Cannot load test %s -- skipping' % t)
-                    import traceback
-                    traceback.print_exc()
+                    self.logger.error('Cannot load test %s -- skipping' % t, exc_info=True)
         else:
             # In this other case, we will load the test available
             # from pyworkflow and the other plugins
             # self.paths = [('pyworkflow', os.path.dirname(os.path.dirname(pw.__file__)))]
             self.paths = []
             for name, plugin in pw.Config.getDomain().getPlugins().items():
                 self.paths.append((name, os.path.dirname(plugin.__path__[0])))
             for k, p in self.paths:
                 testPath = os.path.join(p, k, 'tests')
                 if os.path.exists(testPath):
+                    self.logger.debug("Discovering tests at %s" % testPath)
                     testsDict[k] = testLoader.discover(testPath,
                                                        pattern=args.pattern,
                                                        top_level_dir=p)
 
         self.grep = [g.lower() for g in args.grep] if args.grep else []
         self.skip = args.skip
         self.mode = args.mode
-        self.log = args.log
 
         if args.tests:
             self.runSingleTest(testsDict['tests'])
 
         elif args.run:
             for moduleName, tests in testsDict.items():
-                print(pwutils.cyan(">>>> %s" % moduleName))
+                self.logger.info(pwutils.cyanStr(">>>> %s" % moduleName))
                 self.runTests(moduleName, tests)
 
         elif args.grep:
             pattern = args.grep[0]
             for moduleName, tests in testsDict.items():
                 self.printTests(pattern, tests)
 
         else:
             for moduleName, tests in testsDict.items():
                 if self._match(moduleName):
-                    print(pwutils.cyan(">>>> %s" % moduleName))
+                    print(pwutils.cyanStr(">>>> %s" % moduleName))
                     self.printTests(moduleName, tests)
 
     def _match(self, itemName):
         itemLower = itemName.lower()
         grep = (not self.grep or
                 all(g.lower() in itemLower for g in self.grep))
         skip = (self.skip and
                 any(g.lower() in itemLower for g in self.skip))
 
         return grep and not skip
 
     def __iterTests(self, test):
         """ Recursively iterate over a testsuite. """
-        print("__iterTests: %s, is-suite: %s" % (str(test.__class__),
+        self.logger.debug("__iterTests: %s, is-suite: %s" % (str(test.__class__),
                                                  isinstance(test, unittest.TestSuite)))
 
         if isinstance(test, unittest.TestSuite):
             for t in test:
                 self.__iterTests(t)
         else:
             yield test
@@ -177,16 +187,16 @@
                 testModuleName, className, testName = t.id().rsplit('.', 2)
 
                 # If there is a failure loading the test, show it
                 errorStr = 'unittest.loader._FailedTest.'
                 if testModuleName.startswith(errorStr):
                     newName = t.id().replace(errorStr, '')
                     if self._match(newName):
-                        print(pwutils.red('Error loading the test. Please, run the test for more information:'),
-                              newName)
+                        self.logger.error(
+                            pwutils.redStr('Error loading the test. Please, run the test for more information: ' + newName))
                     continue
 
                 if testModuleName != lastModule:
                     lastModule = testModuleName
                     if mode != 'onlyclasses':
                         newItemCallback(MODULE, "%s" % testModuleName)
 
@@ -196,111 +206,55 @@
                                     % (testModuleName, className))
 
                 if mode == 'all':
                     newItemCallback(TEST, "%s.%s.%s"
                                     % (testModuleName, className, testName))
         else:
             if not self.grep:
-                print(pwutils.green(' The plugin does not have any test'))
+                self.logger.warning(pwutils.greenStr(' The plugin does not have any test'))
 
     def _printNewItem(self, itemType, itemName):
         if self._match(itemName):
             spaces = (itemType * 2) * ' '
+            # Do not use intentionally the logger. This is not a logging output but a GUI output
             print("%s %s %s" % (spaces, self.getTestsCommand(), itemName))
 
     def getTestsCommand(self):
         return os.environ.get(SCIPION_TESTS_CMD, getTestsScript())
 
     def printTests(self, moduleName, tests):
         self._visitTests(moduleName, tests, self._printNewItem)
 
-    def _logTest(self, cmd, runTime, result, logFile):
-        with open(self.testLog, "r+") as f:
-            lines = f.readlines()
-            f.seek(0)
-            for l in lines:
-                if '<!-- LAST_ROW -->' in l:
-                    rowStr = "<tr><td>%s</td><td>%s</td><td>%s</td><td>%s</td><td>%s</td></tr>"
-                    if result:  # != 0 means failed in os.system
-                        resultStr = '<font color="red">[FAILED]</font>'
-                    else:
-                        resultStr = '<font color="green">[SUCCEED]</font>'
-                    logStr = '<a href="file://%s">%s</a>' % (logFile, basename(logFile))
-
-                    f.write(rowStr % (self.testCount, cmd, runTime, resultStr, logStr))
-                    f.write('\n')
-                if self.headerPrefix in l:
-                    f.write(self.headerPrefix + self.testTimer.getToc() + '</h3>\n')
-                else:
-                    f.write(l)
-            f.close()
-
     def _runNewItem(self, itemType, itemName):
         if self._match(itemName):
             spaces = (itemType * 2) * ' '
             script = getTestsScript()
             cmd = "%s %s %s %s" % (pw.PYTHON, script, spaces, itemName)
             run = ((itemType == MODULE and self.mode == 'modules') or
                    (itemType == CLASS and self.mode in ('classes', 'onlyclasses')) or
                    (itemType == TEST and self.mode == 'all'))
             if run:
                 if self.log:
-                    logFile = join(self.testsDir, '%s.txt' % itemName)
-                    cmdFull = cmd + " > %s 2>&1" % logFile
+                    # logFile = join(self.testsDir, '%s.txt' % itemName)
+                    cmdFull = cmd + " >> %s 2>&1" % self.log
                 else:
                     logFile = ''
                     cmdFull = cmd
 
-                print(pwutils.green(cmdFull))
+                self.logger.info(pwutils.greenStr(cmdFull))
                 t = pwutils.Timer()
                 t.tic()
                 self.testCount += 1
-                result = os.system(cmdFull)
-                if self.log:
-                    self._logTest(cmd, t.getToc(), result, logFile)
+                os.system(cmdFull)
 
     def runTests(self, moduleName, tests):
-        self.testCount = 0
 
-        if self.log:
-            self.testsDir = join(pw.Config.SCIPION_USER_DATA, 'Tests', self.log)
-            pwutils.cleanPath(self.testsDir)
-            pwutils.makePath(self.testsDir)
-            self.testLog = join(self.testsDir, 'tests.html')
-            self.testTimer = pwutils.Timer()
-            self.testTimer.tic()
-            self.headerPrefix = '<h3>Test results (%s) Duration: ' % pwutils.prettyTime()
-            f = open(self.testLog, 'w')
-            f.write("""<!DOCTYPE html>
-    <html>
-    <body>
-    """)
-            f.write(self.headerPrefix + '</h3>')
-            f.write("""    
-     <table style="width:100%" border="1">
-      <tr>
-        <th>#</th>
-        <th>Command</th>
-        <th>Time</th>
-        <th>Result</th>
-        <th>Log file</th>
-      </tr>
-    <!-- LAST_ROW -->
-    </table> 
-    
-    </body>
-    </html>""")
-
-            f.close()
+        self.testCount = 0
         self._visitTests(moduleName, tests, self._runNewItem)
 
-        if self.log:
-            print("\n\nOpen results in your browser: \nfile:///%s"
-                  % self.testLog)
-
     def runSingleTest(self, tests):
         result = pwtests.GTestResult()
         tests.run(result)
         result.doReport()
         resultPassed = result.numberTests - result.testFailed
         sys.exit(1 if result.testFailed > 0 or resultPassed == 0 else 0)
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_schedule_run.py` & `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_schedule_run.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,218 +21,302 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
+import logging
+
+from pyworkflow.utils import LoggingConfigurator
+
 import os
 import sys
 import time
 import argparse
 
 from pyworkflow.protocol import (getProtocolFromDb,
                                  STATUS_FINISHED, STATUS_ABORTED, STATUS_FAILED,
-                                 Set, Protocol)
-
-# Add callback for remote debugging if available.
-from pyworkflow.utils import prettyTimestamp, getFileLastModificationDate
+                                 STATUS_RUNNING, STATUS_SCHEDULED, STATUS_SAVED,
+                                 STATUS_LAUNCHED, Set, Protocol, MAX_SLEEP_TIME)
+from pyworkflow.constants import PROTOCOL_UPDATED
 
-try:
-    from rpdb2 import start_embedded_debugger
-    from signal import signal, SIGUSR2
-
-    signal(SIGUSR2, lambda sig, frame: start_embedded_debugger('a'))
-except ImportError:
-    pass
+stopStatuses = [STATUS_FINISHED, STATUS_ABORTED, STATUS_FAILED]
 
 
 class RunScheduler:
     """ Check that all dependencies are met before launching a run. """
 
-    def _parseArgs(self):
-        parser = argparse.ArgumentParser()
-        _addArg = parser.add_argument  # short notation
-
-        _addArg("projPath", metavar='PROJECT_NAME',
-                help="Project database path.")
-
-        _addArg("dbPath", metavar='DATABASE_PATH',
-                help="Protocol database path.")
-
-        _addArg("protId", type=int, metavar='PROTOCOL_ID',
-                help="Protocol ID.")
-
-        _addArg("--sleep_time", type=int, default=15,
-                dest='sleepTime', metavar='SECONDS',
-                help="Sleeping time (in seconds) between updates.")
+    def __init__(self, args, logger):
+        self._args = args
+        # Enter to the project directory and load protocol from db
+        self.protocol = self._loadProtocol()
+        self.project = self.protocol.getProject()
+        self.log = logger
+        self.protPid = os.getpid()
+        self.protocol.setPid(self.protPid)
+        self.protocol._store(self.protocol._pid)
+        self.prerequisites = list(map(int, self.protocol.getPrerequisites()))
+        # Keep track of the last time the protocol was checked and
+        # its modification date to avoid unnecessary db opening
+        self.updatedProtocols = dict()
+        self.initial_sleep = self._args.initial_sleep
 
-        _addArg("--wait_for", nargs='*', type=int, default=[],
-                dest='waitProtIds', metavar='PROTOCOL_ID',
-                help="List of protocol ids that should be not running "
-                     "(i.e, finished, aborted or failed) before this "
-                     "run will be executed.")
+    def getSleepTime(self):
+        return self._args.sleepTime
 
-        self._args = parser.parse_args()
+    def getInitialSleepTime(self):
+        return self.initial_sleep
 
-    def _loadProtocol(self):
+    def _loadProtocol(self) -> Protocol:
         return getProtocolFromDb(self._args.projPath,
                                  self._args.dbPath,
                                  self._args.protId, chdir=True)
 
-    def main(self):
-        self._parseArgs()
+    def _log(self, msg):
+        self.log.info(msg)
 
-        stopStatuses = [STATUS_FINISHED, STATUS_ABORTED, STATUS_FAILED]
+    def _updateProtocol(self, protocol):
 
-        # Enter to the project directory and load protocol from db
-        protocol = self._loadProtocol()
-        mapper = protocol.getMapper()
-
-        log = open(protocol.getScheduleLog(), 'w')
-        pid = os.getpid()
-        protocol.setPid(pid)
+        protId = protocol.getObjId()
 
-        prerequisites = list(map(int, protocol.getPrerequisites()))
+        if protId in self.updatedProtocols:
+            return self.updatedProtocols[protId]
 
-        def _log(msg):
-            log.write("%s: %s\n" % (prettyTimestamp(), msg))
-            log.flush()
+        protDb = protocol.getDbPath()
 
-        _log("Scheduling protocol %s, pid: %s, prerequisites: %s"
-             % (protocol.getObjId(), pid, prerequisites))
+        if os.path.exists(protDb):
+            updateResult = self.project._updateProtocol(protocol)
+            if updateResult == PROTOCOL_UPDATED:
+                self._log("Updated protocol: %s (%s)" % (protId, protocol))
+            else:
+                self._log("The protocol %s (%s) is up to date" % (protId, protocol))
+            self.updatedProtocols[protId] = protocol
 
-        mapper.store(protocol)
-        mapper.commit()
-        mapper.close()
+        return protocol
 
-        # Keep track of the last time the protocol was checked and
-        # its modification date to avoid unnecessary db opening
-        lastCheckedDict = {}
-        updatedProtocols = []
+    def _getProtocolFromPointer(self, pointer):
+        """
+        The function return a protocol from an attribute
+
+           A) When the pointer points to a protocol
+
+           B) When the pointer points to another object (INDIRECTLY).
+              - The pointer has an _extended value (new parameters
+                configuration in the protocol)
+
+           C) When the pointer points to another object (DIRECTLY).
+              - The pointer has not an _extended value (old parameters
+                configuration in the protocol)
+        """
+        output = pointer.get()
+        if isinstance(output, Protocol):  # case A
+            protocol = output
+        else:
+            if pointer.hasExtended():  # case B
+                protocol = pointer.getObjValue()
+            else:  # case C
+                protocol = self.project.getNode(str(output.getObjParentId())).run
+        return protocol
+
+    def _getSecondsToWait(self, inProt):
+        """
+        Assigns a timeout penalty or reward depending on the status of the
+        input protocol (inProt)
+        If inProt status is stopped we assign a reward i.o.c a penalty
+        """
+        protStatus = inProt.getStatus()
+        inStreaming = inProt.worksInStreaming()
+        meStreaming = self.protocol.worksInStreaming()
+
+        penaltyRewardValues = {
+            STATUS_LAUNCHED: 5 if inStreaming else 10,
+            STATUS_RUNNING: -2 if inStreaming else 3,
+            STATUS_SCHEDULED: int(self.getSleepTime()/2),
+            STATUS_SAVED: self.getSleepTime(),
+        }
+
+        secondToWait = penaltyRewardValues.get(protStatus, -3)
+
+        if not meStreaming:
+            secondToWait += 3 * self.getSleepTime()
+
+        return secondToWait
+
+    def _checkPrerequisites(self, prerequisites, project):
+        # Check if we need to wait for required protocols
+        wait = False
+        # For each protocol that is a prerequisite that has not finished,
+        # we'll penalize with 3 more seconds of waiting
+        penalize = 0
+        self._log("Checking prerequisites... %s" % prerequisites)
+        for protId in prerequisites:
+            # Check if prerequisites exist. In the case of metaprotocols, it
+            # may be necessary to load them from the project database.
+            node = project.getRunsGraph().getNode(str(protId))
+
+            if node is None:
+                self._log("Updating runs graph. Missing protocol ... %s" % protId)
+                project.getRunsGraph(refresh=True)
+
+            node = project.getRunsGraph().getNode(str(protId))
+            # Check if the protocol is within our workflow
+            if node is None:
+                self._log("Protocol can't wait for %s. Missing prerequisite " % protId)
+                break
 
-        def _updateProtocol(protocol, project):
+            prot = project.getRunsGraph().getNode(str(protId)).run
+            if prot is not None:
+                prot = self._updateProtocol(prot)
+                penalize += self._getSecondsToWait(prot)
+                if prot.getStatus() not in stopStatuses:
+                    wait = True
+                    self._log("   ...waiting for %s" % prot)
+        return wait, penalize
+
+    def _checkMissingInput(self):
+        """
+         Check if there are missing inputs
+         In case of having them, check if protocol is in streaming
+        """
+        inputMissing = False
+        # For each input that is not ready we'll penalize with 3 more
+        # seconds of waiting
+        penalize = 0
+
+        self._log("Checking input data...")
+        # Updating input protocols
+        for key, attr in self.protocol.iterInputAttributes():
+            self.log.debug("Turn for %s" % key)
+            inputProt = self._getProtocolFromPointer(attr)
+            inputProt = self._updateProtocol(inputProt)
+            penalize += self._getSecondsToWait(inputProt)
+
+        validation = self.protocol.validate()
+        if len(validation) > 0:
+            inputMissing = True
+            self._log("%s doesn't validate:\n\t- %s" % (self.protocol.getObjLabel(),
+                                                        '\n\t- '.join(
+                                                            validation)))
+        elif not self.protocol.worksInStreaming():
+            for key, attr in self.protocol.iterInputAttributes():
+                inSet = attr.get()
+                if isinstance(inSet, Set) and inSet.isStreamOpen():
+                    inputMissing = True
+                    self._log("Waiting for closing %s... (does not work in "
+                              "streaming)" % inSet)
+                    break
+                elif isinstance(inSet, Protocol) and not inSet.isFinished():  # Then is a pointer to a protocol
+                    inputMissing = True
+                    self._log("Waiting for protocol %s to finish... (does not work in "
+                              "streaming)" % inSet)
+                    break
+
+                else:
+                    self._log("%s is not blocking this protocol. All ready." % inSet)
+
+        if not inputMissing:
+            inputProtocolIds = self.protocol.getProtocolsToUpdate()
+            for protId in inputProtocolIds:
+                protocol = self.project.getProtocol(protId)
+                self.log.debug("Turn from inputProtocolDict for %s" % protocol)
+                self._updateProtocol(protocol)
+
+        return inputMissing, penalize
+
+    def schedule(self):
+        self._log("Scheduling protocol %s, PID: %s,prerequisites: %s, works in streaming: %s." %
+                  (self.protocol.getObjId(), self.protPid, self.prerequisites,
+                   self.protocol.worksInStreaming()))
+
+        initialSleepTime = runScheduler.getInitialSleepTime()
+        self._log("Waiting %s seconds before start checking inputs " % initialSleepTime)
+        time.sleep(initialSleepTime)
 
-            protId = protocol.getObjId()
+        while True:
+            # Clear the list of protocols updated in the previous loop
+            self.updatedProtocols.clear()
+            sleepTime = self.getSleepTime()
+            # FIXME: This does not cover all the cases:
+            # When the user registers new coordinates after clicking the
+            # "Analyze result" button, this action is registered in the project.sqlite
+            # and not in it's own run.db and never gets updated. It is not critical and
+            # will only affect a combination of json import with extended that will
+            # appear after clicking on the "Analyze result" button.
 
-            if protId in updatedProtocols:
-                return
+            # Check if there are missing inputs
+            missing, penalize = self._checkMissingInput()
+            sleepTime += penalize
 
-            protDb = protocol.getDbPath()
+            # Check the prerequisites
+            wait, penalize = self._checkPrerequisites(self.prerequisites,
+                                                      self.project)
+            sleepTime += penalize
 
-            if os.path.exists(protDb):
-                lastChecked = lastCheckedDict.get(protId, None)
-                lastModified = getFileLastModificationDate(protDb)
+            if not missing and not wait:
+                break
 
-                if lastChecked is None or (lastModified > lastChecked):
-                    project._updateProtocol(protocol,
-                                            skipUpdatedProtocols=False)
-                    _log("Updated protocol %s" % protId)
-                    updatedProtocols.append(protId)
+            sleepTime = max(min(sleepTime, MAX_SLEEP_TIME), self.getSleepTime())
 
-        def _getProtocolFromPointer(pointer):
-            """
-            The function return a protocol from an attribute
+            self._log("Still not ready, sleeping %s seconds...\n" % sleepTime)
+            time.sleep(sleepTime)
 
-               A) When the pointer points to a protocol
+        self._log("Launching the protocol >>>>")
+        self.project.launchProtocol(self.protocol, scheduled=True, force=True)
 
-               B) When the pointer points to another object (INDIRECTLY).
-                  - The pointer has an _extended value (new parameters
-                    configuration in the protocol)
+def parseArgs():
+    parser = argparse.ArgumentParser()
+    _addArg = parser.add_argument  # short notation
 
-               C) When the pointer points to another object (DIRECTLY).
-                  - The pointer has not an _extended value (old parameters
-                    configuration in the protocol)
-            """
-            output = pointer.get()
-            if isinstance(output, Protocol):  # case A
-                protocol = output
-            else:
-                if pointer.hasExtended():  # case B
-                    protocol = pointer.getObjValue()
-                else:  # case C
-                    protocol = self.getProject().getProtocol(
-                        output.getObjParentId())
-            return protocol
+    _addArg("projPath", metavar='PROJECT_NAME',
+            help="Project database path.")
 
-        while True:
-            protocol = self._loadProtocol()
-            project = protocol.getProject()
+    _addArg("dbPath", metavar='DATABASE_PATH',
+            help="Protocol database path.")
 
-            # Check if there are missing inputs
-            missing = False
-            # Check if there are input protocols failed or aborted
-            failedInputProtocols = False
+    _addArg("protId", type=int, metavar='PROTOCOL_ID',
+            help="Protocol ID.")
 
-            # Clear the list of protocols updated in the previous loop
-            updatedProtocols.clear()
+    _addArg("logPath", metavar='LOG_PATH', help='Path to the log file.')
 
-            _log("Checking input data...")
-            # FIXME: This does not cover all the cases:
-            # When the user registers new coordinates after clicking the
-            # "Analyze result" button, this action is registered in the project.sqlite
-            # and not in it's own run.db and never gets updated. It is not critical and
-            # will only affect a combination of json import with extended that will
-            # appear after clicking on the "Analyze result" button.
-            for key, attr in protocol.iterInputAttributes():
-                inputProt = _getProtocolFromPointer(attr)
-                _updateProtocol(inputProt, project)
-                if (inputProt.getStatus() == STATUS_ABORTED or
-                        inputProt.getStatus() == STATUS_FAILED):
-                    failedInputProtocols = True
-
-            if not failedInputProtocols:
-                _updateProtocol(protocol, project)
-                validation = protocol.validate()
-                if len(validation) > 0:
-                    missing  = True
-                    _log("%s doesn't validate:\n\t- %s"
-                         % (protocol.getObjLabel(),
-                            '\n\t- '.join(validation)))
-                elif not protocol.worksInStreaming():
-                    for key, attr in protocol.iterInputAttributes():
-                        inSet = attr.get()
-                        if isinstance(inSet, Set) and inSet.isStreamOpen():
-                            missing = True
-                            _log("Waiting for closing %s... "
-                                 "(%s does not work in streaming)"
-                                 % (inSet, protocol))
-                            break
-
-                if not missing:
-                    inputProtocolDict = protocol.inputProtocolDict()
-                    for prot in inputProtocolDict.values():
-                        _updateProtocol(prot, project)
-
-            _log("Checking prerequisites... %s" % prerequisites)
-
-            wait = False  # Check if we need to wait for required protocols
-            for protId in prerequisites:
-                prot = project.getProtocol(protId)
-                if prot is not None:
-                    _updateProtocol(prot, project)
-                    if prot.getStatus() not in stopStatuses:
-                        wait = True
-                        _log("   ...waiting for %s" % prot)
+    _addArg("--initial_sleep", type=int, default=0,
+            dest='initial_sleep', metavar='SECONDS',
+            help="Initial sleeping time (in seconds)")
 
-            if not missing and not wait:
-                break
+    _addArg("--sleep_time", type=int, default=15,
+            dest='sleepTime', metavar='SECONDS',
+            help="Sleeping time (in seconds) between updates.")
 
-            project.mapper.commit()
-            project.mapper.close()
+    _addArg("--wait_for", nargs='*', type=int, default=[],
+            dest='waitProtIds', metavar='PROTOCOL_ID',
+            help="List of protocol ids that should be not running "
+                 "(i.e, finished, aborted or failed) before this "
+                 "run will be executed.")
 
-            _log("Still not ready, sleeping %s seconds...\n"
-                 % self._args.sleepTime)
-            time.sleep(self._args.sleepTime)
-
-        _log("Launching the protocol >>>>")
-        log.close()
-        project.launchProtocol(protocol, scheduled=True, force=True)
+    return parser.parse_args()
 
 
 if __name__ == '__main__':
-    try:
-        scheduler = RunScheduler()
-        scheduler.main()
-    except Exception as ex:
-        print(ex)
-        print("Schedule fail with this parameters: ", sys.argv)
+
+    # Create a child process
+    # using os.fork() method
+    pid = os.fork()
+
+    # pid greater than 0 represents
+    # the parent process
+    if pid > 0:
+        sys.exit(0)
+    else:
+        try:
+            # Parse arguments
+            args = parseArgs()
+
+            # Configure logging
+            LoggingConfigurator.setUpProtocolSchedulingLog(args.logPath)
+            logger = logging.getLogger(__name__)
+
+            runScheduler = RunScheduler(args, logger)
+            runScheduler.schedule()
+
+        except Exception as ex:
+            print("Scheduling failed with these parameters: ", sys.argv)
+            raise ex from None
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_sleep.py` & `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_sleep.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_sync_data.py` & `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_sync_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 # **************************************************************************
 
 """
 Scipion data synchronization.
 
 Get(put) tests data, from(to) the server to(from) the $SCIPION_TESTS folder.
 """
+import logging
+logger = None
+
 import sys
 import os
 from os.path import join, isdir, exists, relpath, dirname
 from subprocess import call
 import time
 import argparse
 import hashlib
@@ -42,84 +45,94 @@
 from urllib.request import urlopen, urlretrieve
 
 import pyworkflow as pw
 from pyworkflow.utils import redB, red, green, yellow
 
 
 def main():
+
+    #Configure logging
+    logging.basicConfig(level=pw.Config.SCIPION_LOG_LEVEL, format=pw.Config.SCIPION_LOG_FORMAT)
+    global logger
+    logger = logging.getLogger(__name__)
+
     # Get arguments.
     args = get_parser().parse_args()
 
     # Dispatch the easy cases first (list and check), and then take care of
     # the more complex ones.
     if args.list:
         listDatasets(args.url)
         sys.exit(0)
 
-    if args.check_all:
-        datasets = [x.decode("utf-8").strip('./\n') for x in urlopen('%s/MANIFEST' % args.url)]
-        print('Checking datasets: %s' % ' '.join(datasets))
+    if args.check:
+        if not args.datasets:
+            datasets = [x.decode("utf-8").strip('./\n') for x in urlopen('%s/MANIFEST' % args.url)]
+        else:
+            datasets = args.datasets
+
+        logger.info('Checking %s at %s.' % (' '.join(datasets), args.url))
 
         all_uptodate = True
         for dataset in datasets:
             all_uptodate &= check(dataset, url=args.url, verbose=args.verbose)
         if all_uptodate:
-            print('All datasets are up-to-date.')
+            logger.info('All datasets are up-to-date.')
             sys.exit(0)
         else:
-            print('Some datasets are not updated.')
+            logger.error('Some datasets are not updated.')
             sys.exit(1)
 
     if not args.datasets:
-        sys.exit('At least --list, --check-all or datasets needed.\n'
+        sys.exit('At least --list, --check or datasets needed.\n'
                  'Run with --help for more info.')
 
-    print('Selected datasets: %s' % yellow(' '.join(args.datasets)))
+    logger.info('Selected datasets: %s' % yellow(' '.join(args.datasets)))
 
     testFolder = pw.Config.SCIPION_TESTS
 
     if args.format:
         for dataset in args.datasets:
             datasetFolder = join(testFolder, dataset)
-            print('Formatting %s (creating MANIFEST file)' % dataset)
+            logger.info('Formatting %s (creating MANIFEST file)' % dataset)
 
             if not exists(datasetFolder):
                 sys.exit('ERROR: %s does not exist in datasets folder %s.' %
                          (dataset, testFolder))
             createMANIFEST(datasetFolder)
         sys.exit(0)
 
     if args.download:
         # Download datasets.
         try:
             for dataset in args.datasets:
                 if exists(join(testFolder, dataset)):
-                    print('Local copy of dataset %s detected.' % dataset)
-                    print('Checking for updates...')
+                    logger.info('Local copy of dataset %s detected.' % dataset)
+                    logger.info('Checking for updates...')
                     update(dataset, url=args.url, verbose=args.verbose)
                 else:
-                    print('Dataset %s not in local machine. '
+                    logger.info('Dataset %s not in local machine. '
                           'Downloading...' % dataset)
                     download(dataset, url=args.url, verbose=args.verbose)
         except IOError as e:
-            print('Warning: %s' % e)
+            logger.warning('%s' % e)
             if e.errno == 13:  # permission denied
-                print('Maybe you need to run as the user that '
+                logger.warning('Maybe you need to run as the user that '
                       'did the global installation?')
             sys.exit(1)
         sys.exit(0)
 
     if args.upload:
         # Upload datasets.
         for dataset in args.datasets:
             try:
                 upload(dataset, login=args.login,
                        remoteFolder=args.remotefolder, delete=args.delete)
             except Exception as e:
-                print('Error when uploading dataset %s: %s' % (dataset, e))
+                logger.error('Error when uploading dataset %s: %s' % (dataset, e))
                 if ask() != 'y':
                     sys.exit(1)
         sys.exit(0)
 
     # If we get here, we did not use the right arguments. Show a little help.
     get_parser().print_usage()
 
@@ -145,15 +158,15 @@
     add('datasets', metavar='DATASET', nargs='*', help='Name of a dataset.')
     add('--delete', action='store_true',
         help=('When uploading, delete any remote files in the dataset not '
               'present in local. It leaves the remote scipion data directory '
               'as it is in the local one. Dangerous, use with caution.'))
     add('-u', '--url', default=pw.Config.SCIPION_URL_TESTDATA,
         help='URL where remote datasets will be looked for.')
-    add('--check-all', action='store_true',
+    add('--check', action='store_true',
         help='See if there is any remote dataset not in sync with locals.')
     add('-l', '--login', default='scipion@scipion.cnb.csic.es', help='ssh login string. For upload')
     add('-rf', '--remotefolder', default='scipionfiles/downloads/scipion/data/tests',
         help='remote folder to put the dataset there. For upload.')
     add('-v', '--verbose', action='store_true', help='Print more details.')
 
     return parser
@@ -172,22 +185,22 @@
                 print("  * %s (not in dataset format)" % folder)
 
     try:
         print("\nRemote datasets in %s" % yellow(url))
         for line in sorted(urlopen('%s/MANIFEST' % url)):
             print("  * %s" % line.decode("utf-8").strip('./\n'))
     except Exception as e:
-        print("Error reading %s (%s)" % (url, e))
+        logger.info("Error reading %s (%s)" % (url, e))
 
 
 def check(dataset, url, verbose=False, updateMANIFEST=False):
     """ See if our local copy of dataset is the same as the remote one.
     Return True if it is (if all the checksums are equal), False if not.
     """
-    def vlog(txt): sys.stdout.write(txt) if verbose else None  # verbose log
+    def vlog(txt): logger.info(txt) if verbose else None  # verbose log
 
     vlog("Checking dataset %s ... " % dataset)
 
     if updateMANIFEST:
         createMANIFEST(join(pw.Config.SCIPION_TESTS, dataset))
     else:
         vlog("(not updating local MANIFEST) ")
@@ -212,45 +225,45 @@
                     vlog("  %s: %s\n" % (txt, ' '.join(lst)))
             show("Local files missing in the server", flocal - fremote)
             show("Remote files missing locally", fremote - flocal)
             show("Files with differences", [f for f in fremote & flocal
                                             if md5sLocal[f] != md5sRemote[f]])
             return False
     except Exception as e:
-        vlog("\terror: %s\n" % e)
+        logger.error("Can't check dataset %s." % dataset, exc_info=e)
         return False
 
 
 def download(dataset, destination=None, url=None, verbose=False):
     """ Download all the data files mentioned in url/dataset/MANIFEST """
     # Get default values for variables if we got None.
     destination = destination or pw.Config.SCIPION_TESTS
 
     # First make sure that we ask for a known dataset.
     if dataset not in [x.decode('utf-8').strip('./\n') for x in urlopen('%s/MANIFEST' % url)]:
-        print("Unknown dataset: %s" % red(dataset))
-        print("Use --list to see the available datasets.")
+        logger.info("Unknown dataset: %s" % red(dataset))
+        logger.info("Use --list to see the available datasets.")
         return
 
     # Retrieve the dataset's MANIFEST file.
     # It contains a list of "file md5sum" of all files included in the dataset.
     datasetFolder = join(destination, dataset)
     os.makedirs(datasetFolder)
     manifest = join(destination, dataset, 'MANIFEST')
     try:
         if verbose:
-            print("Retrieving MANIFEST file")
+            logger.info("Retrieving MANIFEST file")
         open(manifest, 'wb').writelines(
             urlopen('%s/%s/MANIFEST' % (url, dataset)))
     except Exception as e:
-        print("ERROR reading %s/%s/MANIFEST (%s)" % (url, dataset, e))
+        logger.info("ERROR reading %s/%s/MANIFEST (%s)" % (url, dataset, e))
         return
 
     # Now retrieve all of the files mentioned in MANIFEST, and check their md5.
-    print('Fetching files of dataset "%s"...' % dataset)
+    logger.info('Fetching files of dataset "%s"...' % dataset)
     lines = open(manifest).readlines()
     done = 0.0  # fraction already done
     inc = 1.0 / len(lines)  # increment, how much each iteration represents
     for line in lines:
         fname, md5Remote = line.strip().split()
         fpath = join(datasetFolder, fname)
         try:
@@ -262,145 +275,146 @@
 
             md5 = md5sum(fpath)
             assert md5 == md5Remote, \
                 "Bad md5. Expected: %s Computed: %s" % (md5Remote, md5)
 
             done += inc
             if verbose:
-                print(redB("%3d%% " % (100 * done)), fname)
+                logger.info(redB("%3d%% " % (100 * done)) + fname)
             else:
                 sys.stdout.write(redB("#") * (int(50*done)-int(50*(done-inc))))
                 sys.stdout.flush()
         except Exception as e:
-            print("\nError in %s (%s)" % (fname, e))
-            print("URL: %s/%s/%s" % (url, dataset, fname))
-            print("Destination: %s" % fpath)
+            logger.info("\nError in %s (%s)" % (fname, e))
+            logger.info("URL: %s/%s/%s" % (url, dataset, fname))
+            logger.info("Destination: %s" % fpath)
             if ask("Continue downloading? (y/[n]): ", ['y', 'n', '']) != 'y':
                 return
 
 
 def update(dataset, workingCopy=None, url=None, verbose=False):
     """ Update local dataset with the contents of the remote one.
     It compares the md5 of remote files in url/dataset/MANIFEST with the
     ones in workingCopy/dataset/MANIFEST, and downloads only when necessary.
     """
     # Get default values for variables if we got None.
     workingCopy = workingCopy or pw.Config.SCIPION_TESTS
 
     # Verbose log
-    def vlog(txt): sys.stdout.write(txt) if verbose else None
+    def vlog(txt): logger.info(txt) if verbose else None
 
     # Read contents of *remote* MANIFEST file, and create a dict {fname: md5}
     manifest = urlopen('%s/%s/MANIFEST' % (url, dataset)).readlines()
     md5sRemote = dict(x.decode("utf-8").strip().split() for x in manifest)
 
     # Update and read contents of *local* MANIFEST file, and create a dict
     datasetFolder = join(workingCopy, dataset)
     try:
         last = max(os.stat(join(datasetFolder, x)).st_mtime for x in md5sRemote)
         t_manifest = os.stat(join(datasetFolder, 'MANIFEST')).st_mtime
         assert t_manifest > last and time.time() - t_manifest < 60*60*24*7
     except (OSError, IOError, AssertionError) as e:
-        print("Regenerating local MANIFEST...")
+        logger.info("Regenerating local MANIFEST...")
         createMANIFEST(datasetFolder)
     md5sLocal = dict(x.strip().split() for x in open(join(datasetFolder, 'MANIFEST')))
 
     # Check that all the files mentioned in MANIFEST are up-to-date
-    print("Verifying MD5s...")
+    logger.info("Verifying MD5s...")
 
     filesUpdated = 0  # number of files that have been updated
     taintedMANIFEST = False  # can MANIFEST be out of sync?
     downloadingPrinted = False
     for fname in md5sRemote:
         fpath = join(datasetFolder, fname)
         try:
             if exists(fpath) and md5sLocal[fname] == md5sRemote[fname]:
                 vlog("\r  %s  %s\n" % (green("OK"), fname))
                 pass  # just to emphasize that we do nothing in this case
             else:
                 if not downloadingPrinted:
                     verboseMsg = " Next time use -v for more details." if not verbose else ""
-                    print("Differences detected. Downloading data.%s" % verboseMsg)
+                    logger.info("%s differs. Downloading new version.%s" % (fname, verboseMsg))
 
                 vlog("\r  %s  %s  (downloading... " % (red("XX"), fname))
                 if not isdir(dirname(fpath)):
                     os.makedirs(dirname(fpath))
 
                 urlretrieve('%s/%s/%s' % (url, dataset, fname)
                             , fpath)
 
-                vlog("done)\n")
+                vlog("done)")
                 filesUpdated += 1
         except Exception as e:
-            print("\nError while updating %s: %s" % (fname, e))
+            logger.error("Couldn't update %s." % fname, exc_info= e)
             taintedMANIFEST = True  # if we don't update, it can be wrong
 
-    print("...done. Updated files: %d" % filesUpdated)
+    logger.info("...done. Updated files: %d" % filesUpdated)
 
     # Save the new MANIFEST file in the folder of the downloaded dataset
     if filesUpdated > 0:
         open(join(datasetFolder, 'MANIFEST'), 'w').writelines(md5sRemote)
 
     if taintedMANIFEST:
-        print("Some files could not be updated. Regenerating local MANIFEST ...")
+        logger.info("Some files could not be updated. Regenerating local MANIFEST ...")
         createMANIFEST(datasetFolder)
 
 
 def upload(dataset, login, remoteFolder, delete=False):
     """ Upload a dataset to our repository """
 
     localFolder = join(pw.Config.SCIPION_TESTS, dataset)
 
     if not exists(localFolder):
         sys.exit("ERROR: local folder %s does not exist." % localFolder)
 
-    print("Warning: Uploading, please BE CAREFUL! This can be dangerous.")
-    print('You are going to be connected to "%s" to write in folder '
+    logger.info("Warning: Uploading, please BE CAREFUL! This can be dangerous.")
+    logger.info('You are going to be connected to "%s" to write in folder '
           '"%s" the dataset "%s".' % (login, remoteFolder, dataset))
     if ask() == 'n':
         return
 
     # First make sure we have our MANIFEST file up-to-date
-    print("Updating local MANIFEST file with MD5 info...")
+    logger.info("Updating local MANIFEST file with MD5 info...")
     createMANIFEST(localFolder)
 
     # Upload the dataset files (with rsync)
-    print("Uploading files...")
+    logger.info("Uploading files...")
     call(['rsync', '-rlv', '--chmod=a+r', localFolder,
           '%s:%s' % (login, remoteFolder)] + (['--delete'] if delete else []))
 
     # Regenerate remote MANIFEST (which contains a list of datasets)
-    print("Regenerating remote MANIFEST file...")
+    logger.info("Regenerating remote MANIFEST file...")
     call(['ssh', login,
           'cd %s && find -type d -mindepth 1 -maxdepth 1 > MANIFEST' % remoteFolder])
     # This is a file that just contains the name of the directories
     # in remoteFolder. Nothing to do with the MANIFEST files in
     # the datasets, which contain file names and md5s.
 
     # Leave a register (log file)
-    print("Logging modification attempt in modifications.log ...")
+    logger.info("Logging modification attempt in modifications.log ...")
     log = """++++
 Modification to %s dataset made at
 %s
 by %s at %s
 ----""" % (dataset, time.asctime(), getpass.getuser(), ' '.join(os.uname()))
     call(['ssh', login,
           'echo "%s" >> %s' % (log, join(remoteFolder, 'modifications.log'))])
-    print("...done.")
+    logger.info("...done.")
 
 
 def createMANIFEST(path):
     """ Create a MANIFEST file in path with the md5 of all files below """
 
     with open(join(path, 'MANIFEST'), 'w') as manifest:
         for root, dirs, files in os.walk(path):
             for filename in set(files) - {'MANIFEST'}:  # all but ourselves
                 fn = join(root, filename)  # file to check
+                logger.info("Calculating md5 for local %s ... " % filename)
                 manifest.write('%s %s\n' % (relpath(fn, path), md5sum(fn)))
-
+                logger.info(green("DONE!"))
 
 def md5sum(fname):
     """ Return the md5 hash of file fname """
 
     mhash = hashlib.md5()
     with open(fname, 'rb') as f:
         for chunk in iter(lambda: f.read(128 * mhash.block_size), b""):
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/apps/pw_viewer.py` & `scipion-pyworkflow-3.1.0/pyworkflow/apps/pw_viewer.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/__init__.py` & `scipion-pyworkflow-3.1.0/pyworkflow/protocol/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,17 +19,20 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-from .gui import *
-from .canvas import *
-from .widgets import *
-from .graph import *
-from .graph_layout import *
-from .tree import *
-from .browser import *
-from .text import *
+"""
+This modules contains classes required for the workflow
+execution and tracking like: Step and Protocol
+"""
 
-from . import tooltip
+from .protocol import *
+from .executor import *
+from .constants import *
+from .params import *
+
+from .launch import *
+
+from .hosts import HostConfig
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/browser.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,17 +29,19 @@
 A concrete use of ObjectBrowser is FileBrowser, where the
 elements to inspect and preview are files.
 """
 import os.path
 import stat
 import tkinter as tk
 import time
+import logging
+logger = logging.getLogger(__name__)
 
 import pyworkflow.utils as pwutils
-from . import gui
+from . import gui, LIST_TREEVIEW
 from .tree import BoundTree, TreeProvider
 from .text import TaggedText, openTextFileEditor
 from .widgets import Button, HotButton
 from .. import Config
 
 PARENT_FOLDER = ".."
 
@@ -80,15 +82,15 @@
             p.paneconfig(rightPanel, minsize=200)
 
             # Register a callback when the item is clicked
             self.tree.itemClick = self._itemClicked
 
     def _fillLeftPanel(self, frame):
         gui.configureWeigths(frame)
-        self.tree = BoundTree(frame, self.treeProvider)
+        self.tree = BoundTree(frame, self.treeProvider, style=LIST_TREEVIEW)
         self.tree.grid(row=0, column=0, sticky='news')
         self.itemConfig = self.tree.itemConfig
         self.getImage = self.tree.getImage
 
     def _fillRightPanel(self, frame):
         frame.columnconfigure(0, weight=1)
 
@@ -104,36 +106,38 @@
         bottom.grid(row=1, column=0, sticky='news')
         frame.rowconfigure(1, weight=1)
         gui.configureWeigths(bottom)
         bottom.rowconfigure(1, weight=1)
         self._fillRightBottom(bottom)
 
     def _fillRightTop(self, top):
-        self.noImage = self.getImage('no-image128.gif')
+        self.noImage = self.getImage(pwutils.Icon.NO_IMAGE_128)
         self.label = tk.Label(top, image=self.noImage)
         self.label.grid(row=0, column=0, sticky='news')
 
     def _fillRightBottom(self, bottom):
-        self.text = TaggedText(bottom, width=40, height=15, bg='white',
+        self.text = TaggedText(bottom, width=40, height=15, bg=Config.SCIPION_BG_COLOR,
                                takefocus=0)
         self.text.grid(row=0, column=0, sticky='news')
 
     def _itemClicked(self, obj):
         self._lastSelected = obj
         img, desc = self.treeProvider.getObjectPreview(obj)
         # Update image preview
         if self.showPreviewTop:
             if isinstance(img, str):
                 img = self.getImage(img)
             if img is None:
                 img = self.noImage
             self.label.config(image=img)
+
         # Update text preview
         self.text.setReadOnly(False)
         self.text.clear()
+
         if desc is not None:
             self.text.addText(desc)
         self.text.setReadOnly(True)
         if hasattr(self, 'entryLabel') and not self._lastSelected.isDir():
             self.entryVar.set(self._lastSelected.getFileName())
 
     def getSelected(self):
@@ -174,35 +178,38 @@
 
     def getDateStr(self):
         return pwutils.dateStr(self.getDate()) if self._stat else '0'
 
     def getDate(self):
         return self._stat.st_mtime if self._stat else 0
 
+    def isLink(self):
+        return os.path.islink(self._fullpath)
+
 
 class FileHandler(object):
     """ This class will be used to get the icon, preview and info
     from the different types of objects.
     It should be used with FileTreeProvider, where different
     types of handlers can be registered.
     """
 
     def getFileIcon(self, objFile):
         """ Return the icon name for a given file. """
         if objFile.isDir():
-            icon = 'file_folder.gif'
+            icon = pwutils.Icon.FOLDER if not objFile.isLink() else pwutils.Icon.FOLDER_LINK
         else:
-            icon = 'file_generic.gif'
+            icon = pwutils.Icon.FILE if not objFile.isLink() else pwutils.Icon.FILE_LINK
 
         return icon
 
     def getFilePreview(self, objFile):
         """ Return the preview image and description for the specific object."""
         if objFile.isDir():
-            return 'fa-folder-open.gif', None
+            return pwutils.Icon.FOLDER_OPEN, None
         return None, None
 
     def getFileActions(self, objFile):
         """ Return actions that can be done with this object.
         Actions will be displayed in the context menu 
         and the first one will be the default when double-click.
         """
@@ -216,15 +223,15 @@
 
     def getFileIcon(self, objFile):
         return self._icon
 
 
 class SqlFileHandler(FileHandler):
     def getFileIcon(self, objFile):
-        return 'file_sqlite.gif'
+        return pwutils.Icon.DB
 
 
 class FileTreeProvider(TreeProvider):
     """ Populate a tree with files and folders of a given path """
 
     _FILE_HANDLERS = {}
     _DEFAULT_HANDLER = FileHandler()
@@ -236,47 +243,66 @@
         """ Register a FileHandler for a given file extension. 
         Params:
             fileHandler: the FileHandler that will take care of extensions.
             *extensions: the extensions list that will be associated to this
                 FileHandler.
         """
         for fileExt in extensions:
-            cls._FILE_HANDLERS[fileExt] = fileHandler
+            handlersList = cls._FILE_HANDLERS.get(fileExt, [])
+            handlersList.append(fileHandler)
+            cls._FILE_HANDLERS[fileExt] = handlersList
 
     def __init__(self, currentDir=None, showHidden=False, onlyFolders=False):
         TreeProvider.__init__(self, sortingColumnName=self.FILE_COLUMN)
         self._currentDir = os.path.abspath(currentDir)
         self._showHidden = showHidden
         self._onlyFolders = onlyFolders
         self.getColumns = lambda: [(self.FILE_COLUMN, 300),
                                    (self.SIZE_COLUMN, 70), ('Time', 150)]
 
-    def getFileHandler(self, obj):
+    def getFileHandlers(self, obj):
         filename = obj.getFileName()
         fileExt = pwutils.getExt(filename)
-        return self._FILE_HANDLERS.get(fileExt, self._DEFAULT_HANDLER)
+        return self._FILE_HANDLERS.get(fileExt, [self._DEFAULT_HANDLER])
 
     def getObjectInfo(self, obj):
         filename = obj.getFileName()
-        fileHandler = self.getFileHandler(obj)
-        icon = fileHandler.getFileIcon(obj)
+        fileHandlers = self.getFileHandlers(obj)
+        icon = fileHandlers[0].getFileIcon(obj)
 
         info = {'key': filename, 'text': filename,
                 'values': (obj.getSizeStr(), obj.getDateStr()), 'image': icon
                 }
 
         return info
 
     def getObjectPreview(self, obj):
-        fileHandler = self.getFileHandler(obj)
-        return fileHandler.getFilePreview(obj)
+
+        try:
+            # Look for any preview available
+            fileHandlers = self.getFileHandlers(obj)
+
+            for fileHandler in fileHandlers:
+                preview = fileHandler.getFilePreview(obj)
+                if preview:
+                    img, desc = preview
+                    if obj.isLink():
+                        desc = "Is a link" if desc is None else desc + "\nIs a link."
+                    return img, desc
+
+        except Exception as e:
+            msg = "Couldn't get preview for %s" % obj
+            logger.error(msg, exc_info=e)
+            return None, msg + " See scipion GUI log window for more details."
 
     def getObjectActions(self, obj):
-        fileHandler = self.getFileHandler(obj)
-        actions = fileHandler.getFileActions(obj)
+        fileHandlers = self.getFileHandlers(obj)
+        actions = []
+        for fileHandler in fileHandlers:
+            actions += fileHandler.getFileActions(obj)
         # Always allow the option to open as text
         # specially useful for unknown formats
         fn = obj.getPath()
         actions.append(("Open external Editor",
                         lambda: openTextFileEditor(fn), pwutils.Icon.ACTION_REFERENCES))
 
         return actions
@@ -301,15 +327,15 @@
                 # Do not add hidden files if not requested
                 if not self._showHidden and f.startswith('.'):
                     continue
 
                 # All ok...add item.
                 fileInfoList.append(FileInfo(self._currentDir, f))
         except Exception as e:
-            print("Can't list files at " + self._currentDir, e)
+            logger.error("Can't list files at " + self._currentDir, e)
 
         # Sort objects
         fileInfoList.sort(key=self.fileKey, reverse=not self.isSortingAscending())
 
         return fileInfoList
 
     def fileKey(self, f):
@@ -334,28 +360,47 @@
 
 
 class FileBrowser(ObjectBrowser):
     """ The FileBrowser is a particular class of ObjectBrowser
     where the "objects" are just files and directories.
     """
 
+    _lastSelectedFile = None
+    "Class scope attribute to keep the lastSelected file"
+
+    _fileSelectedAtLoading = None
+    "Class scope attribute to offer *Recent* shortcut"
+
     def __init__(self, parent, initialDir='.',
                  selectionType=SELECT_FILE,
                  selectionSingle=True,
                  allowFilter=True,
                  filterFunction=None,
                  previewDim=144,
                  showHidden=False,  # Show hidden files or not?
                  selectButton='Select',  # Change the Select button text
                  entryLabel=None,  # Display an entry for some input
                  entryValue='',  # Display a value in the entry field
                  showInfo=None,  # Used to notify errors or messages
                  shortCuts=None,  # Shortcuts to common locations/paths
                  onlyFolders=False
                  ):
+        """
+
+        :param parent: Parent tkinter window.
+        :param initialDir: Folder to show when loading the dialog.
+        :param selectionType: Any of SELECT_NONE, SELECT_FILE, SELECT_FOLDER, SELECT_PATH.
+        :param showHidden: Pass True to show hidden files.
+        :param selectButton: text for the select button. Defaults to *Select*.
+        :param entryLabel: text for the entry widget. Default None. There will be no entry.
+        :param entryValue: default value for the entry. Needs entryLabel.
+        :param showInfo: callback to show a string message, otherwise _showInfo will be used.
+        :param shortCuts: list of extra :class:`ShortCut`
+        :param onlyFolders: Pass True to show only folders.
+        """
         self.pathVar = tk.StringVar()
         self.pathVar.set(os.path.abspath(initialDir))
         self.pathEntry = None
         self.previousSearch = None
         self.previousSearchTS = None
         self.shortCuts = shortCuts
         self._provider = FileTreeProvider(initialDir, showHidden, onlyFolders)
@@ -375,17 +420,17 @@
             selectButton = None
 
         buttonsFrame = tk.Frame(self)
         self._fillButtonsFrame(buttonsFrame)
         buttonsFrame.grid(row=1, column=0)
 
     def _showInfo(self, msg):
-        """ Default way (print to console) to show a message with a given info.
+        """ Default way (logger.info to console) to show a message with a given info.
         """
-        print(msg)
+        logger.info(msg)
 
     def _fillLeftPanel(self, frame):
         """ Redefine this method to include a buttons toolbar and
         also include a filter bar at the bottom of the Tree.
         """
         # Tree with files
         frame.columnconfigure(0, weight=1)
@@ -419,16 +464,17 @@
         if self.entryLabel:
             entryFrame = tk.Frame(frame)
             entryFrame.grid(row=2, column=0, sticky='new')
             tk.Label(entryFrame, text=self.entryLabel).grid(row=0, column=0,
                                                             sticky='nw', pady=3)
             tk.Entry(entryFrame,
                      textvariable=self.entryVar,
-                     bg='white',
-                     width=65).grid(row=0, column=1, sticky='nw', pady=3)
+                     bg=Config.SCIPION_BG_COLOR,
+                     width=65,
+                     font=gui.getDefaultFont()).grid(row=0, column=1, sticky='nw', pady=3)
 
         frame.rowconfigure(treeRow, weight=1)
 
     def _addButton(self, frame, text, image, command):
         btn = tk.Label(frame, text=text, image=self.getImage(image),
                        compound=tk.LEFT, cursor='hand2')
         btn.bind('<Button-1>', command)
@@ -445,14 +491,19 @@
         self._addButton(frame, 'Home', pwutils.Icon.HOME, self._actionHome)
         self._addButton(frame, 'Launch folder', pwutils.Icon.ROCKET,
                         self._actionLaunchFolder)
         self._addButton(frame, 'Working dir', pwutils.Icon.ACTION_BROWSE,
                         self._actionWorkingDir)
         self._addButton(frame, 'Up', pwutils.Icon.ARROW_UP, self._actionUp)
 
+        self._fileSelectedAtLoading = FileBrowser._lastSelectedFile
+
+        if self._fileSelectedAtLoading is not None:
+            self._addButton(frame, 'Recent', None, self._actionRecent)
+
         # Add shortcuts
         self._addShortCuts(frame)
 
     def _addShortCuts(self, frame):
         """ Add shortcuts if available"""
         if self.shortCuts:
             for shortCut in self.shortCuts:
@@ -492,20 +543,26 @@
         if PARENT_FOLDER not in self.tree._objDict:
             itemKeyToFocus = self.tree.get_children()[0]
 
         # Focusing on a item, but nothing is selected 
         # Current dir remains in _lastSelected
         self._lastSelected = FileInfo(os.path.dirname(newDir),
                                       os.path.basename(newDir))
+
+        FileBrowser._lastSelectedFile = self._lastSelected
+
         self.tree.focus(itemKeyToFocus)
 
     def _actionUp(self, e=None):
         parentFolder = pwutils.getParentFolder(self.treeProvider.getDir())
         self._goDir(parentFolder)
 
+    def _actionRecent(self, e=None):
+        self._goDir(self._fileSelectedAtLoading.getPath())
+
     def _actionHome(self, e=None):
         self._goDir(pwutils.getHomePath())
 
     def _actionRoot(self, e=None):
         self._goDir("/")
 
     def _actionLaunchFolder(self, e=None):
@@ -561,28 +618,29 @@
             self._goDir(path)
 
         else:
             self.showInfo("Path '%s' does not exists. " % path)
             self.pathEntry.focus()
 
     def onClose(self):
+        """ This onClose is replaced at init time in the FileBrowserWindow with its own callback"""
         pass
 
-    def onSelect(self, obj):
-        print(obj, "type: ", type(obj))
-
     def _close(self, e=None):
+        """ This _close is bound to the close button"""
         self.onClose()
 
     def _select(self, e=None):
-        _lastSelected = self.getSelected()
-        if _lastSelected is not None:
-            self.onSelect(_lastSelected)
+
+        self._lastSelected = self.getSelected()
+
+        if self._lastSelected is not None:
+            self.onSelect(self._lastSelected)
         else:
-            print('Select a valid file/folder')
+            self.showInfo('Select a valid file/folder')
 
     def getEntryValue(self):
         return self.entryVar.get()
 
     def getCurrentDir(self):
         return self.treeProvider.getDir()
 
@@ -634,35 +692,35 @@
         self.registerHandlers()
         browser = FileBrowser(self.root, path,
                               showInfo=lambda msg: self.showInfo(msg, "Info"),
                               shortCuts=shortCuts,
                               **kwargs)
         if onSelect:
             def selected(obj):
-                onSelect(obj)
                 self.close()
+                onSelect(obj)
 
             browser.onSelect = selected
         browser.onClose = self.close
         self.setBrowser(browser)
 
     def getEntryValue(self):
         return self.browser.getEntryValue()
 
     def getCurrentDir(self):
         return self.browser.getCurrentDir()
 
     def registerHandlers(self):
         register = FileTreeProvider.registerFileHandler  # shortcut
 
-        register(TextFileHandler('file_text.gif'),
+        register(TextFileHandler(pwutils.Icon.TXT_FILE),
                  '.txt', '.log', '.out', '.err', '.stdout', '.stderr', '.emx',
                  '.json', '.xml', '.pam')
-        register(TextFileHandler('file_python.gif'), '.py')
-        register(TextFileHandler('file_java.gif'), '.java')
+        register(TextFileHandler(pwutils.Icon.PYTHON_FILE), '.py')
+        register(TextFileHandler(pwutils.Icon.JAVA_FILE), '.java')
         register(SqlFileHandler(), '.sqlite', '.db')
         # register(MdFileHandler(), '.xmd', '.star', '.pos', '.ctfparam', '.doc')
         # register(ParticleFileHandler(),
         #          '.xmp', '.tif', '.tiff', '.spi', '.mrc', '.map', '.raw',
         #          '.inf', '.dm3', '.em', '.pif', '.psd', '.spe', '.ser', '.img',
         #          '.hed', *STANDARD_IMAGE_EXTENSIONS)
         # register(VolFileHandler(), '.vol')
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/canvas.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/canvas.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,21 @@
 # *
 # **************************************************************************
 """
 This module extends the functionalities of a normal Tkinter Canvas.
 The new Canvas class allows to easily display Texboxes and Edges
 that can be interactively dragged and clicked.
 """
+import logging
+logger = logging.getLogger(__name__)
 import math
 import tkinter as tk
 import operator
 
+from pyworkflow import Config
 from pyworkflow.gui import gui, getDefaultFont, cfgFontSize
 from pyworkflow.gui.widgets import Scrollable
 
 DEFAULT_ZOOM = 100
 
 DEFAULT_FONT_SIZE = cfgFontSize
 
@@ -45,15 +48,15 @@
 
 class Canvas(tk.Canvas, Scrollable):
     """Canvas to draw some objects.
     It will really contains a Frame, a Canvas and scrollbars"""
     _images = {}
 
     def __init__(self, parent, tooltipCallback=None, tooltipDelay=1500, **kwargs):
-        defaults = {'bg': 'white'}
+        defaults = {'bg': Config.SCIPION_BG_COLOR}
         defaults.update(kwargs)
         Scrollable.__init__(self, parent, tk.Canvas, **defaults)
 
         self.lastItem = None  # Track last item selected
         self.lastPos = (0, 0)  # Track last clicked position
         self.eventPos = (0, 0)
         self.firstPos = None  # Track first clicked position (for a drag action)
@@ -85,14 +88,15 @@
         self._tooltipId = None
         self._tooltipOn = False  # True if the tooltip is displayed
         self._tooltipCallback = tooltipCallback
         self._tooltipDelay = tooltipDelay
 
         self._runsFont = getDefaultFont().copy()
         self._zoomFactor = DEFAULT_ZOOM
+        self.nodeList = None
 
         if tooltipCallback:
             self.bind('<Motion>', self.onMotion)
             # self.bind('<Leave>', self.onLeave)
             self._createTooltip()  # This should set
 
         self._menu = tk.Menu(self, tearoff=0)
@@ -164,14 +168,16 @@
 
     def _findItem(self, xc, yc):
         """ Find if there is any item in the canvas
         in the mouse event coordinates.
         Return None if not Found
         """
         items = self.find_overlapping(xc - 1, yc - 1, xc + 1, yc + 1)
+        if self.lastItem is not None and self.lastItem.id in items:
+            return self.lastItem
         for i in items:
             if i in self.items:
                 return self.items[i]
         return None
 
     def _handleMouseEvent(self, event, callback):
         # Store last event coordinates
@@ -211,17 +217,27 @@
         if actions:
             self._menu.delete(0, tk.END)
             for a in actions:
                 if a is None:
                     self._menu.add_separator()
                 else:
                     img = ''
-                    if len(a) > 2:  # image for the action
+                    label= a[0]
+                    size = len(a)
+
+                    if size > 2:  # image for the action
                         img = self.getImage(a[2])
-                    self._menu.add_command(label=a[0], command=a[1],
+
+                        # Shortcuts
+                        if size > 3:
+                            shortCut = a[3]
+                            if shortCut:
+                                label= "%s (%s)" % (label, shortCut)
+
+                    self._menu.add_command(label=label, command=a[1],
                                            image=img, compound=tk.LEFT,
                                            font=gui.getDefaultFont())
             self._menu.post(e.x_root, e.y_root)
             unpost = False
         if unpost:
             self._menu.unpost()
 
@@ -358,42 +374,69 @@
 
     def zoomerP(self, event):
         self.__zoom(event, 1.111111)
 
     def zoomerM(self, event):
         self.__zoom(event, 0.9)
 
-    def drawGraph(self, graph, layout=None, drawNode=None):
+    def moveTo(self, x, y):
+
+        if x > 1 or y > 1:
+            x0,y0,x1,y1 = self.bbox("all")
+
+            # x dim
+            x = x / (x0+x1)
+            start, end = self.xview()
+            visisble_length = end - start
+            x = x - (visisble_length/2)
+
+            # Same with y
+            y = y / (y0+y1)
+            start, end = self.yview()
+            visible_length = end - start
+            y = y - (visible_length / 2)
+
+        self.xview("moveto", x)
+        self.yview("moveto", y)
+
+    def drawGraph(self, graph, layout=None, drawNode=None, nodeList=None):
         """ Draw a graph in the canvas.
         nodes in the graph should have x and y.
         If layout is not None, it will be used to 
         reorganize the node positions.
         Provide drawNode if you want to customize how
         to create the boxes for each graph node.
         """
 
         # Reset the zoom and font
         scale = self._zoomFactor / DEFAULT_ZOOM
         self._zoomFactor = DEFAULT_ZOOM
         self._runsFont['size'] = DEFAULT_FONT_SIZE
+        self.nodeList = nodeList
 
         if drawNode is None:
             self.drawNode = self._drawNode
         else:
             self.drawNode = drawNode
 
         self._drawNodes(graph.getRoot(), {})
 
         if layout is not None:
             layout.draw(graph)
+            # Update node positions
+            self._updatePositions(graph.getRoot(), {})
+        self.updateScrollRegion()
+        self.__zoom(None, scale)
+
+    def reorganizeGraph(self, graph, layout=None):
 
+        layout.draw(graph)
         # Update node positions
-        self._updatePositions(graph.getRoot(), {})
+        self._updatePositions(graph.getRoot(), {}, createEdges=False)
         self.updateScrollRegion()
-        self.__zoom(None, scale)
 
     def _drawNode(self, canvas, node):
         """ Default implementation to draw nodes as textboxes. """
         return TextBox(self, node.getLabel(), 0, 0,
                        bgColor="#99DAE8", textColor='black')
 
     def _drawNodes(self, node, visitedDict={}):
@@ -405,44 +448,94 @@
             node.width, node.height = item.getDimensions()
             node.item = item
             item.node = node
             self.addItem(item)
 
             if getattr(node, 'expanded', True):
                 for child in node.getChilds():
-                    self._drawNodes(child, visitedDict)
+                    if self.nodeList is None:
+                        self._drawNodes(child, visitedDict)
+                    elif self.nodeList.getNode(child.run.getObjId()).isVisible():
+                        self._drawNodes(child, visitedDict)
+                    else:
+                        self._setupParentProperties(node, visitedDict)
             else:
                 self._setupParentProperties(node, visitedDict)
 
+    def _connectParents(self, item):
+        """
+        Establishes a connection between the visible parents of node's children
+        with node
+        """
+        logger.debug("Connecting item %s with parents:" % item)
+        visibleParents = self._visibleParents(item, [])
+        for visibleParent in visibleParents:
+            if visibleParent != item:
+                try:
+                    logger.debug("Visible parent: %s" % visibleParent)
+                    dest = self.items[item.item.id]
+                    source = self.items[visibleParent.item.id]
+                    visibleParentNode = self.nodeList.getNode(visibleParent.run.getObjId())
+                    itemNode = self.nodeList.getNode(item.run.getObjId())
+
+                    if visibleParent not in item.getParents() and visibleParentNode.isExpanded():
+                        self.createEdge(source, dest)
+                    if not itemNode.isExpanded():
+                        self.createEdge(source, dest)
+                except:
+                    logger.warning("Can't connect node %s to parent %s" % (item, visibleParent))
+
+    def _visibleParents(self, node, parentlist):
+        """
+        Return a list with the visible parents of the node's children
+        """
+        for child in node.getChilds():
+            parents = child.getParents()
+            for parent in parents:
+                parentNode = self.nodeList.getNode(parent.run.getObjId())
+                if parentNode.isVisible() and parent != node and parent not in parentlist:
+                        parentlist.append(parent)
+        return parentlist
+
     def _setupParentProperties(self, node, visitedDict):
         """ This methods is used for collapsed nodes, in which 
         the properties (width, height, x and y) is propagated
         to the hidden childs.
         """
         for child in node.getChilds():
             if child.getName() not in visitedDict:
                 child.width = node.width
                 child.height = node.height
                 child.x = node.x
                 child.y = node.y
                 self._setupParentProperties(child, visitedDict)
 
-    def _updatePositions(self, node, visitedDict={}):
+    def _updatePositions(self, node, visitedDict=None, createEdges=True):
         """ Update position of nodes and create the edges. """
         nodeName = node.getName()
 
         if nodeName not in visitedDict:
             visitedDict[nodeName] = True
             item = node.item
+            logger.debug("Updating position for node: %s, item: %s" % (node, item))
             item.moveTo(node.x, node.y)
 
             if getattr(node, 'expanded', True):
                 for child in node.getChilds():
-                    self.createEdge(item, child.item)
-                    self._updatePositions(child, visitedDict)
+                    if self.nodeList is None:
+                        self.createEdge(item, child.item)
+                        self._updatePositions(child, visitedDict, createEdges)
+                    elif self.nodeList.getNode(child.run.getObjId()).isVisible():
+                        if createEdges:
+                            self.createEdge(item, child.item)
+                        self._updatePositions(child, visitedDict, createEdges)
+            else:
+                if createEdges:
+                    self._connectParents(node)
+                self._updatePositions(node, visitedDict, createEdges)
 
 
 def findClosestPoints(list1, list2):
     candidates = []
     for c1 in list1:
         for c2 in list2:
             candidates.append([c1, c2, math.hypot(c2[0] - c1[0], c2[1] - c1[1])])
@@ -580,21 +673,29 @@
         socket = self.sockets[name]
         return self.getSocketCoordsAt(socket["verticalLocation"], socket["position"],
                                       self.countSockets(socket["verticalLocation"]))
 
     def getSocketCoordsAt(self, verticalLocation, position=1, socketsCount=1):
         x1, y1, x2, y2 = self.getCorners()
         xc = (x2 + x1) / 2.0
+        yc = (y1 + y2) / 2.0
+
         socketsGroupSize = (socketsCount - 1) * self.socketSeparation
         socketsGroupStart = xc - (socketsGroupSize / 2)
         x = socketsGroupStart + (position - 1) * self.socketSeparation
         if verticalLocation == "top":
             y = y1
-        else:
+        elif verticalLocation == 'bottom':
             y = y2
+        elif verticalLocation == 'left':
+            y = yc
+            x = x1
+        else:
+            y = yc
+            x = x2
         return x, y
 
     def relocateSockets(self, verticalLocation, count):
         sockets = self.getSocketsAt(verticalLocation)
         for socket in sockets:
             o = socket["object"]
             x, y = self.getSocketCoordsAt(verticalLocation, socket["position"], count)
@@ -642,23 +743,29 @@
         self._selected = value
         bw = 0
         bc = 'black'
         if value:
             bw = 2
             self.lift()
             # bc = 'Firebrick'
+        else:
+            self.lower()
+
         self.canvas.itemconfig(self.id, width=bw, outline=bc)
         self._notifySelectionListeners(value)
 
     def getSelected(self):
         return self._selected
 
     def lift(self):
         self.canvas.lift(self.id)
 
+    def lower(self):
+        self.canvas.lower(self.id)
+
 
 class TextItem(Item):
     """This class will serve to paint and store rectangle boxes with some text.
        x and y are the coordinates of the center of this item"""
 
     def __init__(self, canvas, text, x, y, bgColor, textColor='black'):
         super(TextItem, self).__init__(canvas, x, y)
@@ -698,14 +805,19 @@
         super(TextItem, self).move(dx, dy)
         self.canvas.move(self.id_text, dx, dy)
 
     def lift(self):
         super(TextItem, self).lift()
         self.canvas.lift(self.id_text)
 
+    def lower(self):
+        self.canvas.lower(self.id_text)
+        super(TextItem, self).lower()
+
+
 
 class TextBox(TextItem):
     def __init__(self, canvas, text, x, y, bgColor, textColor='black'):
         super(TextBox, self).__init__(canvas, text, x, y, bgColor, textColor)
 
     def _paintBounds(self, x, y, w, h, fillColor):
         return self.canvas.create_rectangle(x, y, w, h, fill=fillColor, outline=fillColor)
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/dialog.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/text.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,791 +1,769 @@
 # **************************************************************************
 # *
-# * Authors:     J.M. De la Rosa Trevin (jmdelarosa@cnb.csic.es)
-# *              Jose Gutierrez (jose.gutierrez@cnb.csic.es)
+# * Authors:     J.M. De la Rosa Trevin (delarosatrevin@scilifelab.se) [1]
 # *
-# * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
+# * [1] SciLifeLab, Stockholm University
 # *
-# * This program is free software; you can redistribute it and/or modify
+# * This program is free software: you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
-# * the Free Software Foundation; either version 3 of the License, or
+# * the Free Software Foundation, either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
 # * You should have received a copy of the GNU General Public License
-# * along with this program; if not, write to the Free Software
-# * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
-# * 02111-1307  USA
+# * along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 """
-Module to handling Dialogs
-some code was taken from tkSimpleDialog
+Text based widgets.
 """
-import tkinter as tk
-import traceback
-from tkinter.colorchooser import askcolor as _askColor
-
-from pyworkflow.exceptions import PyworkflowException
-from pyworkflow.utils import Message, Icon
-from . import gui
-from .tree import BoundTree
-from .text import Text, TaggedText
 
-# Possible result values for a Dialog
-RESULT_YES = 0
-RESULT_NO = 1
-RESULT_CANCEL = 2
-RESULT_RUN_SINGLE = 3
-RESULT_RUN_ALL = 4
-
-
-class Dialog(tk.Toplevel):
-    _images = {}  # Images cache
-    """Implementation of our own dialog to display messages
-    It will have by default a three buttons: YES, NO and CANCEL
-    Subclasses can rename the labels of the buttons like: OK, CLOSE or others
-    The buttons(and theirs order) can be changed.
-    An image name can be passed to display left to the message.
-    """
 
-    def __init__(self, parent, title, **kwargs):
-        """Initialize a dialog.
-        Arguments:
-            parent -- a parent window (the application window)
-            title -- the dialog title
-        **args accepts:
-            buttons -- list of buttons tuples containing which buttons to display
-        """
-
-        if parent is None:
-            parent = tk.Tk()
-            parent.withdraw()
-            gui.setCommonFonts()
-
-        tk.Toplevel.__init__(self, parent)
-
-        self.withdraw()  # remain invisible for now
-        # If the master is not viewable, don't
-        # make the child transient, or else it
-        # would be opened withdrawn
-        if parent.winfo_viewable():
-            self.transient(parent)
-
-        if title:
-            self.title(title)
-
-        self.parent = parent
-        # Default to CANCEL so if window is "Closed" behaves the same.
-        self.result = RESULT_CANCEL
-        self.initial_focus = None
-
-        bodyFrame = tk.Frame(self)
-        # Call subclass method body to create that region
-        self.body(bodyFrame)
-        bodyFrame.grid(row=0, column=0, sticky='news',
-                       padx=5, pady=5)
-
-        self.icons = kwargs.get('icons',
-                                {RESULT_YES: Icon.BUTTON_SELECT,
-                                 RESULT_NO: Icon.BUTTON_CLOSE,
-                                 RESULT_CANCEL: Icon.BUTTON_CANCEL})
-
-        self.buttons = kwargs.get('buttons', [('OK', RESULT_YES),
-                                              ('Cancel', RESULT_CANCEL)])
-        self.defaultButton = kwargs.get('default', 'OK')
-        btnFrame = tk.Frame(self)
-        # Create buttons 
-        self.buttonbox(btnFrame)
-        btnFrame.grid(row=1, column=0, sticky='sew',
-                      padx=5, pady=(0, 5))
-
-        gui.configureWeigths(self)
-
-        if self.initial_focus is None:
-            self.initial_focus = self
-
-        self.protocol("WM_DELETE_WINDOW", self.cancel)
-
-        if self.parent is not None:
-            position = kwargs.get('position', (parent.winfo_rootx() + 50,
-                                               parent.winfo_rooty() + 50))
-            self.geometry("+%d+%d" % position)
-
-        self.deiconify()  # become visible now
-        self.initial_focus.focus_set()
-        # Pablo: I've commented this when migrating to python3 since I was getting and exception:
-        # window ".139897767953072.139897384058440" was deleted before its visibility changed
-        # wait for window to appear on screen before calling grab_set
-        self.wait_visibility()
-        self.grab_set()
-        self.wait_window(self)
-
-    def destroy(self):
-        """Destroy the window"""
-        self.initial_focus = None
-        tk.Toplevel.destroy(self)
-
-    #
-    # construction hooks
-
-    def body(self, master):
-        """create dialog body.
-        return widget that should have initial focus.
-        This method should be overridden, and is called
-        by the __init__ method.
-        """
-        pass
-
-    def _createButton(self, frame, text, result):
-        icon = None
-        if result in self.icons.keys():
-            icon = self.getImage(self.icons[result])
-        return tk.Button(frame, text=text, image=icon,
-                         compound=tk.LEFT,
-                         command=lambda: self._handleResult(result))
-
-    def buttonbox(self, btnFrame):
-        frame = tk.Frame(btnFrame)
-        btnFrame.columnconfigure(0, weight=1)
-        frame.grid(row=0, column=0)
-        col = 0
-        for btnLabel, btnResult in self.buttons:
-            btn = self._createButton(frame, btnLabel, btnResult)
-            btn.grid(row=0, column=col, padx=5, pady=5)
-            if (btnLabel == self.defaultButton and
-                    self.initial_focus is None):
-                self.initial_focus = btn
-            col += 1
-        self.bind("<Return>", self._handleReturn)
-        self.bind("<KP_Enter>", self._handleReturn)
-        self.bind("<Escape>", lambda e: self._handleResult(RESULT_CANCEL))
-
-    def _handleResult(self, resultValue):
-        """This method will be called when any button is pressed.
-        It will set the resultValue associated with the button
-        and close the Dialog"""
-        self.result = resultValue
-        noCancel = self.result != RESULT_CANCEL
+import os
+import sys
+import time
+import webbrowser
+import subprocess
+import tkinter.ttk as ttk
+import tkinter as tk
+import tkinter.messagebox as tkMessageBox
 
-        if noCancel and not self.validate():
-            self.initial_focus.focus_set()  # put focus back
-            return
+import pyworkflow as pw
+from pyworkflow import ASCII_COLOR_2_TKINTER
+from pyworkflow.utils import (HYPER_BOLD, HYPER_ITALIC, HYPER_LINK1, HYPER_LINK2,
+                              parseHyperText, renderLine, renderTextFile,
+                              which, envVarOn, expandPattern)
+from pyworkflow.utils.properties import Message, Color, Icon
+from . import gui
+from .widgets import Scrollable, IconButton
+from .tooltip import ToolTip
 
-        self.withdraw()
-        self.update_idletasks()
 
+# Define a function to open files cleanly in a system-dependent way
+if sys.platform.startswith('darwin'):  # macs use the "open" command
+    def _open_cmd(path, tkParent=None):
+        subprocess.Popen(['open', path])
+elif os.name == 'nt':  # there is a function os.startfile for windows
+    def _open_cmd(path, tkParent=None):
+        os.startfile(path)
+elif os.name == 'posix':  # linux systems and so on
+    def find_prog(*args):
+        """Return the first argument that is a program in PATH"""
+        for command in args:
+            if which(command):
+                return command
+        return None
+
+    x_open = find_prog('xdg-open', 'gnome-open', 'kde-open', 'gvfs-open')
+    editor = find_prog('pluma', 'gedit', 'kwrite', 'geany', 'kate',
+                       'emacs', 'nedit', 'mousepad', 'code')
+
+    def _open_cmd(path, tkParent=None):
+        # If it is an url, open with browser.
+        if path.startswith('http://') or path.startswith('https://') or path.endswith('.html'):
+            try:
+                webbrowser.open_new_tab(path)
+                return
+            except:
+                pass
+        # OK, it is a file. Check if it does exist
+        # and notify if it does not
+        if not os.path.isfile(path):
+            try:
+                # if tkRoot is null the error message may be behind
+                # other windows
+                tkMessageBox.showerror("File Error",  # bar title
+                                       "File not found\n(%s)" % path,  # message
+                                       parent=tkParent)
+                return
+            except:
+                return
+
+        if x_open:  # standard way to open
+            proc = subprocess.Popen([x_open, path])
+            time.sleep(1)
+            if proc.poll() in [None, 0]:
+                return  # yay! that's the way to do it!
+        if editor:  # last card: try to open it in an editor
+            proc = subprocess.Popen([editor, path])
+            time.sleep(1)
+            if proc.poll() in [None, 0]:
+                return  # hope we found your fav editor :)
+        print('WARNING: Cannot open %s' % path)  # nothing worked! :(
+else:
+    def _open_cmd(path, tkParent=None):
         try:
-            if noCancel:
-                self.apply()
-        finally:
-            self.cancel()
-
-    def _handleReturn(self, e=None):
-        """Handle press return key"""
-        # Check which of the buttons is the default
-        for button, result in self.buttons:
-            if self.defaultButton == button:
-                self._handleResult(result)
-
-    def cancel(self, event=None):
-        # put focus back to the parent window
-        if self.parent is not None:
-            self.parent.focus_set()
-        self.destroy()
-
-    #
-    # command hooks
-
-    def validate(self):
-        """validate the data
-        This method is called automatically to validate the data before the
-        dialog is destroyed. By default, it always validates OK.
-        """
-        return 1  # override
-
-    def apply(self):
-        """process the data
-        This method is called automatically to process the data, *after*
-        the dialog is destroyed. By default, it does nothing.
-        """
-        pass  # override
-
-    def getImage(self, imgName):
-        """A shortcut to get an image from its name"""
-        return gui.getImage(imgName, self._images)
-
-    def getResult(self):
-        return self.result
-
-    def resultYes(self):
-        return self.result == RESULT_YES
-
-    def resultNo(self):
-        return self.result == RESULT_NO
-
-    def resultCancel(self):
-        return self.result == RESULT_CANCEL
-
-
-def fillMessageText(text, message):
-    # Insert lines of text
-    if isinstance(message, list):
-        lines = message
-    else:
-        lines = message.splitlines()
-    text.setReadOnly(False)
-    text.clear()
-    w = 0
-    for l in lines:
-        w = max(w, len(l))
-        text.addLine(l)
-    w = min(w + 5, 80)
-    h = min(len(lines) + 3, 30)
-    text.config(height=h, width=w)
-    text.addNewline()
-    text.setReadOnly(True)
-
-
-def createMessageBody(bodyFrame, message, image,
-                      frameBg='white',
-                      textBg='white',
-                      textPad=5):
-    """ Create a Text containing the message.
-    Params:
-        bodyFrame: tk.Frame to be filled.
-        msg: a str or list with the lines.
-    """
-    bodyFrame.config(bg=frameBg, bd=0)
-    text = TaggedText(bodyFrame, bg=textBg, bd=0, highlightthickness=0)
-    # Insert image
-    if image:
-        label = tk.Label(bodyFrame, image=image, bg=textBg, bd=0)
-        label.grid(row=0, column=0, sticky='nw')
-
-    text.frame.grid(row=0, column=1, sticky='news',
-                    padx=textPad, pady=textPad)
-    fillMessageText(text, message)
-    bodyFrame.rowconfigure(0, weight=1)
-    bodyFrame.columnconfigure(1, weight=1)
-
-    return text
-
-
-class MessageDialog(Dialog):
-    """Dialog subclasses to show message info, questions or errors.
-    It can display an icon with the message"""
-
-    def __init__(self, parent, title, msg, iconPath, **args):
-        self.msg = msg
-        self.iconPath = iconPath
-        if 'buttons' not in args:
-            args['buttons'] = [('OK', RESULT_YES)]
-            args['default'] = 'OK'
-        Dialog.__init__(self, parent, title, **args)
-
-    def body(self, bodyFrame):
-        self.image = gui.getImage(self.iconPath)
-        createMessageBody(bodyFrame, self.msg, self.image)
-
-
-class ExceptionDialog(MessageDialog):
-    def __init__(self, *args, **kwargs):
-        self._exception = None if "exception" not in kwargs else kwargs['exception']
-        super().__init__(*args, **kwargs)
-
-    def body(self, bodyFrame):
-        super().body(bodyFrame)
-
-        def addTraceback(event):
-            detailsText = TaggedText(bodyFrame, bg='white', bd=0, highlightthickness=0)
-            traceStr = traceback.format_exc()
-            fillMessageText(detailsText, traceStr)
-            detailsText.frame.grid(row=row+1, column=0, columnspan=2, sticky='news', padx=5, pady=5)
-            event.widget.grid_forget()
-
-        row = 1
-        if self._exception:
-
-            if isinstance(self._exception, PyworkflowException):
-                helpUrl = self._exception.getUrl()
-                labelUrl = TaggedText(bodyFrame, bg='white', bd=0, highlightthickness=0)
-                fillMessageText(labelUrl,"Please go here for more details: %s" % helpUrl)
-                labelUrl.grid(row=row, column=0, columnspan=2, sticky='news')
-                row += 1
-
-            label = tk.Label(bodyFrame, text="Show details...", bg='white', bd=0)
-            label.grid(row=row, column=0, columnspan=2, sticky='news')
-            label.bind("<Button-1>", addTraceback)
-
-
-class YesNoDialog(MessageDialog):
-    """Ask a question with YES/NO answer"""
-
-    def __init__(self, master, title, msg, **kwargs):
-        buttonList = [('Yes', RESULT_YES), ('No', RESULT_NO)]
-
-        if kwargs.get('showCancel', False):
-            buttonList.append(('Cancel', RESULT_CANCEL))
-
-        MessageDialog.__init__(self, master, title, msg,
-                               'fa-exclamation-triangle_alert.gif', default='No',
-                               buttons=buttonList)
+            tkMessageBox.showerror("Unknown System",  # bar title
+                                   'Unknown system, so cannot open %s' % path,  # message
+                                   parent=tkParent)
+            return
+        except:
+            pass
 
 
-class GenericDialog(Dialog):
-    """
-    Create a dialog with many buttons
-    Arguments:
-            parent -- a parent window (the application window)
-            title -- the dialog title
-            msg  -- message to display into the dialog
-            iconPath -- path of the image to show into the dialog
-
-        **args accepts:
-            buttons -- list of buttons tuples containing which buttons to display and theirs values
-            icons -- list of icons for all buttons
-            default -- button default
-
-            Example:
-                buttons=[('Single', RESULT_RUN_SINGLE),
-                         ('All', RESULT_RUN_ALL),
-                         ('Cancel', RESULT_CANCEL)],
-                default='Cancel',
-                icons={RESULT_CANCEL: Icon.BUTTON_CANCEL,
-                       RESULT_RUN_SINGLE: Icon.BUTTON_SELECT,
-                       RESULT_RUN_ALL: Icon.ACTION_EXECUTE})
+class HyperlinkManager:
+    """ Tkinter Text Widget Hyperlink Manager, taken from:
+    http://effbot.org/zone/tkinter-text-hyperlink.htm """
+    def __init__(self, text):
+        self.text = text
+        self.text.tag_config("hyper", foreground=pw.Config.SCIPION_MAIN_COLOR, underline=1)
+        self.text.tag_bind("hyper", "<Enter>", self._enter)
+        self.text.tag_bind("hyper", "<Leave>", self._leave)
+        self.text.tag_bind("hyper", "<Button-1>", self._click)
+        self.reset()
+
+    def reset(self):
+        self.links = {}
+
+    def add(self, action):
+        # add an action to the manager.  returns tags to use in
+        # associated text widget
+        tag = "hyper-%d" % len(self.links)
+        self.links[tag] = action
+        return "hyper", tag
+
+    def _enter(self, event):
+        self.text.config(cursor="hand2")
+
+    def _leave(self, event):
+        self.text.config(cursor="")
+
+    def _click(self, event):
+        for tag in self.text.tag_names(tk.CURRENT):
+            if tag[:6] == "hyper-":
+                self.links[tag]()
+                return
+
+
+class Text(tk.Text, Scrollable):    
+    """ Base Text widget with some functionality
+    that will be used by children classes.
     """
-
-    def __init__(self, master, title, msg, iconPath, **kwargs):
-        self.msg = msg
-        self.iconPath = iconPath
-        Dialog.__init__(self, master, title, **kwargs)
-
-    def body(self, bodyFrame):
-        self.image = gui.getImage(self.iconPath)
-        createMessageBody(bodyFrame, self.msg, self.image)
-
-
-class EntryDialog(Dialog):
-    """Dialog to ask some entry"""
-
-    def __init__(self, parent, title, entryLabel, entryWidth=20,
-                 defaultValue='', headerLabel=None):
-        self.entryLabel = entryLabel
-        self.entryWidth = entryWidth
-        self.headerLabel = headerLabel
-        self.tkvalue = tk.StringVar()
-        self.tkvalue.set(defaultValue)
-        self.value = None
-        Dialog.__init__(self, parent, title)
-
-    def body(self, bodyFrame):
-        bodyFrame.config(bg='white')
-        frame = tk.Frame(bodyFrame, bg='white')
-        frame.grid(row=0, column=0, padx=20, pady=20)
-        row = 0
-        if self.headerLabel:
-            label = tk.Label(bodyFrame, text=self.headerLabel, bg='white', bd=0)
-            label.grid(row=row, column=0, columnspan=2, sticky='nw', padx=(15, 10), pady=15)
-            row += 1
-        label = tk.Label(bodyFrame, text=self.entryLabel, bg='white', bd=0)
-        label.grid(row=row, column=0, sticky='nw', padx=(15, 10), pady=15)
-        self.entry = tk.Entry(bodyFrame, bg=gui.cfgEntryBgColor,
-                              width=self.entryWidth, textvariable=self.tkvalue)
-        self.entry.grid(row=row, column=1, sticky='new', padx=(0, 15), pady=15)
-        self.initial_focus = self.entry
-
-    def apply(self):
-        self.value = self.entry.get()
-
-    def validate(self):
-        if len(self.entry.get().strip()) == 0:
-            showError("Validation error", "Value is empty", self)
-            return False
-        return True
-
-
-class EditObjectDialog(Dialog):
-    """Dialog to edit some text"""
-
-    def __init__(self, parent, title, obj, mapper, **kwargs):
-        self.obj = obj
-        self.mapper = mapper
-
-        self.textWidth = 5
-        self.textHeight = 1
-        self.labelText = kwargs.get('labelText', Message.TITLE_LABEL)
-        self.valueText = self.obj.getObjLabel()
-
-        self.commentLabel = Message.TITLE_COMMENT
-        self.commentWidth = 50
-        self.commentHeight = 15
-        self.valueComment = self.obj.getObjComment()
-
-        Dialog.__init__(self, parent, title, **kwargs)
-
-    def body(self, bodyFrame):
-        bodyFrame.config(bg='white')
-        frame = tk.Frame(bodyFrame, bg='white')
-        frame.grid(row=0, column=0, padx=20, pady=20)
-
-        # Label
-        label_text = tk.Label(bodyFrame, text=self.labelText, bg='white', bd=0)
-        label_text.grid(row=0, column=0, sticky='nw', padx=(15, 10), pady=15)
-        # Label box
-        var = tk.StringVar()
-        var.set(self.valueText)
-        self.textLabel = tk.Entry(bodyFrame, width=self.textWidth, textvariable=var, font=gui.getDefaultFont())
-        self.textLabel.grid(row=0, column=1, sticky='news', padx=5, pady=5)
-
-        # Comment
-        label_comment = tk.Label(bodyFrame, text=self.commentLabel, bg='white', bd=0)
-        label_comment.grid(row=1, column=0, sticky='nw', padx=(15, 10), pady=15)
-        # Comment box
-        self.textComment = Text(bodyFrame, height=self.commentHeight,
-                                width=self.commentWidth)
-        self.textComment.setReadOnly(False)
-        self.textComment.setText(self.valueComment)
-        self.textComment.grid(row=1, column=1, sticky='news', padx=5, pady=5)
-        self.initial_focus = self.textLabel
-
-    def getLabel(self):
-        return self.textLabel.get()
-
-    def getComment(self):
-        return self.textComment.getText()
-
-    def apply(self):
-        self.obj.setObjLabel(self.getLabel())
-        self.obj.setObjComment(self.getComment())
-
-        if self.obj.hasObjId():
-            self.mapper.store(self.obj)
-            self.mapper.commit()
-
-    def buttonbox(self, btnFrame):
-        # Cancel the binding of <Return> key
-        Dialog.buttonbox(self, btnFrame)
-        # self.bind("<Return>", self._noReturn)
-        self.unbind("<Return>")
-
-    def _noReturn(self, e):
+    def __init__(self, master, **opts):
+        if 'handlers' in opts:
+            self.handlers = opts.pop('handlers')
+        else:
+            self.handlers = {}
+        opts['font'] = gui.fontNormal
+        defaults = self.getDefaults()
+        defaults.update(opts)
+        Scrollable.__init__(self, master, tk.Text, wrap=tk.WORD, **opts)
+        self._createWidgets(master, **defaults)
+        self.configureTags()
+
+    def _createWidgets(self, master, **opts):
+        """This is an internal function to create the Text, the Scrollbar and the Frame"""
+        
+        # create a popup menu
+        self.menu = tk.Menu(master, tearoff=0, postcommand=self.updateMenu)
+        self.menu.add_command(label="Copy to clipboard", command=self.copyToClipboard)
+        self.menu.add_command(label="Open path", command=self.openFile)
+        # Associate with right click
+        self.bind("<Button-1>", self.onClick)
+        self.bind("<Button-3>", self.onRightClick)
+        
+    def getDefaults(self):
+        """This should be implemented in subclasses to provide defaults"""
+        return {}
+    
+    def configureTags(self):
+        """This should be implemented to create specific tags"""
         pass
-
-
-""" Functions to display dialogs """
-
-
-def askYesNo(title, msg, parent):
-    d = YesNoDialog(parent, title, msg)
-    return d.resultYes()
-
-
-def askYesNoCancel(title, msg, parent):
-    d = YesNoDialog(parent, title, msg, showCancel=True)
-    return d.result
-
-
-def askSingleAllCancel(title, msg, parent):
-    d = GenericDialog(parent, title, msg,
-                      'fa-exclamation-triangle_alert.gif',
-                      buttons=[('Single', RESULT_RUN_SINGLE),
-                               ('All', RESULT_RUN_ALL),
-                               ('Cancel', RESULT_CANCEL)],
-                      default='Single',
-                      icons={RESULT_CANCEL: Icon.BUTTON_CANCEL,
-                             RESULT_RUN_SINGLE: Icon.BUTTON_SELECT,
-                             RESULT_RUN_ALL: Icon.ACTION_EXECUTE})
-
-    return d.result
-
-
-def showInfo(title, msg, parent):
-    MessageDialog(parent, title, msg, 'fa-info-circle_alert.gif')
-
-
-def showWarning(title, msg, parent):
-    MessageDialog(parent, title, msg, 'fa-exclamation-triangle_alert.gif')
-
-
-def showError(title, msg, parent, exception=None):
-    ExceptionDialog(parent, title, msg, 'fa-times-circle_alert.gif', exception=exception)
-
-
-def askString(title, label, parent, entryWidth=20, defaultValue='', headerLabel=None):
-    d = EntryDialog(parent, title, label, entryWidth, defaultValue, headerLabel)
-    return d.value
-
-
-def askColor(defaultColor='black'):
-    (rgbcolor, hexcolor) = _askColor(defaultColor)
-    return hexcolor
-
-
-class ListDialog(Dialog):
-    """
-    Dialog to select an element from a list.
-    It is implemented using the Tree widget.
-    """
-
-    def __init__(self, parent, title, provider, message=None, **kwargs):
-        """ From kwargs:
-                message: message tooltip to show when browsing.
-                selected: the item that should be selected.
-                validateSelectionCallback:
-                    a callback function to validate selected items.
-                allowSelect: if set to False, the 'Select' button will not
-                    be shown.
-                allowsEmptySelection: if set to True, it will not validate
-                    that at least one element was selected.
-        """
-        self.values = []
-        self.provider = provider
-        self.message = message
-        self.validateSelectionCallback = kwargs.get('validateSelectionCallback',
-                                                    None)
-        self._selectmode = kwargs.get('selectmode', 'extended')
-        self._selectOnDoubleClick = kwargs.get('selectOnDoubleClick', False)
-        self._allowsEmptySelection = kwargs.get('allowsEmptySelection', False)
-
-        buttons = []
-        if kwargs.get('allowSelect', True):
-            buttons.append(('Select', RESULT_YES))
-        buttons.append(('Cancel', RESULT_CANCEL))
-
-        Dialog.__init__(self, parent, title, buttons=buttons, **kwargs)
-
-    def body(self, bodyFrame):
-        bodyFrame.config()
-        gui.configureWeigths(bodyFrame)
-        dialogFrame = tk.Frame(bodyFrame)
-        dialogFrame.grid(row=0, column=0, sticky='news', padx=5, pady=5)
-        dialogFrame.config()
-        gui.configureWeigths(dialogFrame, row=1)
-        self._createFilterBox(dialogFrame)
-        self._createTree(dialogFrame)
-        if self.message:
-            label = tk.Label(bodyFrame, text=self.message, compound=tk.LEFT,
-                             image=self.getImage(Icon.LIGHTBULB))
-            label.grid(row=2, column=0, sticky='nw', padx=5, pady=5)
-        self.initial_focus = self.tree
-
-    def _createTree(self, parent):
-        self.tree = BoundTree(parent, self.provider, selectmode=self._selectmode)
-        if self._selectOnDoubleClick:
-            self.tree.itemDoubleClick = lambda obj: self._handleResult(RESULT_YES)
-        self.tree.grid(row=1, column=0)
-
-    def _createFilterBox(self, content):
-        """ Create the Frame with Filter widgets """
-
-        def _onSearch(e=None):
-
-            def comparison():
-                pattern = self._searchVar.get().lower()
-                return [w[0] for w in self.lista.items()
-                        if pattern in self.lista.get(w[0]).lower()]
-
-            self.tree.update()
-            self.lista = {}
-
-            for item in self.tree.get_children():
-
-                itemStr = self.tree.item(item)['text']
-                for value in self.tree.item(item)['values']:
-                    if isinstance(value, int):
-                        itemStr = itemStr + ' ' + str(value)
-                    else:
-                        itemStr = itemStr + ' ' + value
-
-                self.lista[item] = itemStr
-
-            if self._searchVar.get() != '':
-                matchs = comparison()
-                if matchs:
-                    for item in self.tree.get_children():
-                        if item not in matchs:
-                            self.tree.delete(item)
-                else:
-                    self.tree.delete(*self.tree.get_children())
-
-        self.searchBoxframe = tk.Frame(content)
-        label = tk.Label(self.searchBoxframe, text="Filter")
-        label.grid(row=0, column=0, sticky='nw')
-        self._searchVar = tk.StringVar(value='')
-        self.entry = tk.Entry(self.searchBoxframe, bg='white',
-                              textvariable=self._searchVar, width=40,
-                              font=gui.getDefaultFont())
-
-        self.entry.bind('<KeyRelease>', _onSearch)
-        self.entry.focus_set()
-        self.entry.grid(row=0, column=1, sticky='news')
-        self.searchBoxframe.grid(row=0, column=0, sticky='news', padx=5,
-                                 pady=(10, 5))
-
-    def apply(self):
-        self.values = self.tree.getSelectedObjects()
-
-    def validate(self):
-        self.apply()  # load self.values with selected items
-        err = ''
-
-        if self.values:
-            if self.validateSelectionCallback:
-                err = self.validateSelectionCallback(self.values)
+    
+    def addLine(self, line):
+        """Should be implemented to add a line """
+        self.insert(tk.END, line + '\n')
+        
+    def addNewline(self):
+        self.insert(tk.END, '\n')
+        
+    def goBegin(self):
+        self.see(0.0)
+        
+    def goEnd(self):
+        self.see(tk.END)
+        
+    def isAtEnd(self):
+        return self.scrollbar.get() == 1.0
+        
+    def clear(self):
+        self.delete(0.0, tk.END)
+
+    def getText(self):
+
+        textWithNewLine = self.get(0.0, tk.END)
+
+        # Remove the last new line
+        return textWithNewLine.rstrip('\n')
+
+    def setText(self, text):
+        """ Replace the current text with new one. """
+        self.clear()
+        self.addText(text)
+        
+    def addText(self, text):
+        """ Add some text to the current state. """
+        if isinstance(text, list):
+            for line in text:
+                self.addLine(line)
         else:
-            if not self._allowsEmptySelection:
-                err = "Please select an element"
+            for line in text.splitlines():
+                self.addLine(line)
+        
+    def onClick(self, e=None): 
+        self.selection = None
+        self.selection_clear()
+        self.menu.unpost()
+        
+    def onRightClick(self, e):
+        try:
+            self.selection = self.selection_get().strip()
+            self.menu.post(e.x_root, e.y_root)    
+        except tk.TclError as e:
+            pass
+    
+    def copyToClipboard(self, e=None):
+        self.clipboard_clear()
+        self.clipboard_append(self.selection)
+
+    def openFile(self):
+        # What happens when you right-click and select "Open path"
+        self.openPath(self.selection)
+
+    def openPath(self, path):
+        """Try to open the selected path"""
+        path = expandPattern(path)
+
+        # If the path is a dir, open it with scipion browser dir <path>
+        if os.path.isdir(path):
+            dpath = (path if os.path.isabs(path)
+                     else os.path.join(os.getcwd(), path))
+            subprocess.Popen([pw.PYTHON, pw.getViewerScript(), dpath])
+            return
 
-        if err:
-            showError("Validation error", err, self)
-            return False
+        # If it is a file, interpret it correctly and open it with DataView
+        dirname = os.path.dirname(path)
+        fname = os.path.basename(path)
+        if '@' in fname:
+            path = os.path.join(dirname, fname.split('@', 1)[-1])
+        else:
+            path = os.path.join(dirname, fname)
 
+        if os.path.exists(path):
+            from pwem import emlib
+            fn = emlib.FileName(path)
+            if fn is not None and (fn.isImage() or fn.isMetaData()):
+                # fn is None if xmippLib is the xmippLib ghost library
+                from pwem.viewers import DataView
+                DataView(path).show()
+            else:
+                _open_cmd(path)
+        else:
+            # This is probably one special reference, like sci-open:... that
+            # can be interpreted with our handlers.
+            tag = path.split(':', 1)[0] if ':' in path else None
+            if tag in self.handlers:
+                self.handlers[tag](path.split(':', 1)[-1])
+            else:
+                print("Can't find %s" % path)
+
+    def updateMenu(self, e=None):
+        state = 'normal'
+        # if not xmippExists(self.selection):
+        #    state = 'disabled'#self.menu.entryconfig(1, background="green")
+        self.menu.entryconfig(1, state=state)
+        
+    def setReadOnly(self, value):
+        state = tk.NORMAL
+        if value:
+            state = tk.DISABLED
+        self.config(state=state) 
+        
+    def highlight(self, pattern, tag, start="1.0", end="end", regexp=False):
+        """ Apply the given tag to all text that matches the given pattern
+
+        If 'regexp' is set to True, pattern will be treated as a regular expression
+        Taken from: 
+            http://stackoverflow.com/questions/3781670/tkinter-text-highlighting-in-python
+        """
+        start = self.index(start)
+        end = self.index(end)
+        self.mark_set("matchStart", start)
+        self.mark_set("matchEnd", start)
+        self.mark_set("searchLimit", end)
+
+        count = tk.IntVar()
+        while True:
+            index = self.search(pattern, "matchEnd", "searchLimit",
+                                count=count, regexp=regexp)
+            if index == "":
+                break
+            self.mark_set("matchStart", index)
+            self.mark_set("matchEnd", "%s+%sc" % (index, count.get()))
+            self.tag_add(tag, "matchStart", "matchEnd")
+
+
+def configureColorTags(text):
+    """ Create tags in text (of type tk.Text) for all the supported colors. """
+    try:
+        for color in ASCII_COLOR_2_TKINTER.values():
+            text.tag_config(color, foreground=color)
         return True
+    except Exception as e:
+        print("Colors still not available (%s)" % e)
+        return False
 
-
-class ToolbarButton:
+       
+class TaggedText(Text):  
     """
-    Store information about the buttons that will be added to the toolbar.
-    """
-
-    def __init__(self, text, command, icon=None, tooltip=None):
-        self.text = text
-        self.command = command
-        self.icon = icon
-        self.tooltip = tooltip
+    Implement a Text that will recognize some basic tags
+    *some_text* will display some_text in bold
+    _some_text_ will display some_text in italic
+    some_link or [[some_link][some_label]] will display some_link
+     as hyperlink or some_label as hyperlink to some_link
+    also colors are recognized if set option colors=True
+    """           
+    def __init__(self, master, colors=True, **opts):  
+        self.colors = colors
+        Text.__init__(self, master, **opts)
+        self.hm = HyperlinkManager(self)
+
+    def getDefaults(self):
+        return {'bg': pw.Config.SCIPION_BG_COLOR, 'bd': 0}
+        # It used to have also 'font': gui.fontNormal  but that stops
+        # this file from running. Apparently there is no fontNormal in gui.
+
+    def configureTags(self):
+        self.tag_config('normal', justify=tk.LEFT, font=gui.fontNormal)
+        self.tag_config(HYPER_BOLD, justify=tk.LEFT, font=gui.fontBold)
+        self.tag_config(HYPER_ITALIC, justify=tk.LEFT, font=gui.fontItalic)
+        if self.colors:            
+            self.colors = configureColorTags(self)
+            # Color can be unavailable, so disable use of colors
+        
+    @staticmethod
+    def openLink(link):
+        webbrowser.open_new_tab(link)  # Open in the same browser, new tab
+
+    @staticmethod
+    def mailTo(email):
+        webbrowser.open("mailto:" + email)
+
+    def matchHyperText(self, match, tag):
+        """ Process when a match a found and store indexes inside string."""
+        self.insert(tk.END, self.line[self.lastIndex:match.start()])
+        g1 = match.group(tag)
+
+        if tag == HYPER_BOLD or tag == HYPER_ITALIC:
+            self.insert(tk.END, ' ' + g1, tag)
+        elif tag == HYPER_LINK1:
+            self.insert(tk.END, g1, self.hm.add(lambda: self.openLink(g1)))
+        elif tag == HYPER_LINK2:
+            label = match.group('link2_label')
+            if g1.startswith('http'):
+                self.insert(tk.END, label, self.hm.add(lambda: self.openLink(g1)))
+            elif g1.startswith('mailto:'):
+                self.insert(tk.END, label, self.hm.add(lambda: self.mailTo(g1)))
+            else:
+                self.insert(tk.END, label, self.hm.add(lambda: self.openPath(g1)))
+        self.lastIndex = match.end()
+        
+        return g1
+
+    def addLine(self, line):
+        self.line = line
+        self.lastIndex = 0
+        if line is not None:
+            parseHyperText(line, self.matchHyperText)
+            Text.addLine(self, line[self.lastIndex:])
 
 
-class ToolbarListDialog(ListDialog):
+class OutputText(Text):
     """
-    This class extend from ListDialog to allow an
-    extra toolbar to handle operations over the elements
-    in the list (e.g. Edit, New, Delete).
+    Implement a Text that will show file content
+    and handle console metacharacter for colored output
     """
+    def __init__(self, master, filename, colors=True, t_refresh=0, maxSize=400, **opts):
+        """ colors flag indicate if try to parse color meta-characters
+            t_refresh is the refresh time in seconds, 0 means no refresh
+        """
+        self.filename = filename
+        self.colors = colors
+        self.t_refresh = t_refresh
+        self.maxSize = maxSize
+
+        self.refreshAlarm = None  # Identifier returned by after()
+        self.lineNo = 0
+        self.offset = 0
+        self.lastLine = ''
+        Text.__init__(self, master, **opts)
+        self.hm = HyperlinkManager(self)
+        self.doRefresh()
+
+    def getDefaults(self):
+        return {'bg': "black", 'fg': 'white', 'bd': 0,
+                'height': 30,  'width': 100}
+        # It used to have also  'font': gui.fontNormal  but that stops this
+        # file from running. Apparently there is no fontNormal in gui.
+        
+    def configureTags(self):
+        if self.colors:
+            configureColorTags(self)
+
+    def _removeLastLine(self):
+        line = int(self.index(tk.END).split('.')[0])
+        if line > 0:
+            line -= 1
+            self.delete('%d.0' % line, tk.END)
+        
+    def addLine(self, line):
+        renderLine(line, self._addChunk, self.lineNo)
 
-    def __init__(self, parent, title, provider,
-                 message=None, toolbarButtons=None, **kwargs):
-        """ From kwargs:
-                message: message tooltip to show when browsing.
-                selected: the item that should be selected.
-                validateSelectionCallback:
-                    a callback function to validate selected items.
-                allowSelect: if set to False, the 'Select' button will not
-                    be shown.
+    def _addChunk(self, txt, fmt=None):
+        """
+        Add text txt to the widget, with format fmt.
+        fmt can be a color (like 'red') or a link that looks like 'link:url'.
         """
-        self.toolbarButtons = toolbarButtons
-        self._itemDoubleClick = kwargs.get('itemDoubleClick', None)
-        ListDialog.__init__(self, parent, title, provider, message, **kwargs)
-
-    def body(self, bodyFrame):
-        bodyFrame.config(bg='white')
-        gui.configureWeigths(bodyFrame, 1, 0)
-
-        # Add an extra frame to insert the Toolbar
-        # and another one for the ListDialog's body
-        self.toolbarFrame = tk.Frame(bodyFrame, bg='white')
-        self.toolbarFrame.grid(row=0, column=0, sticky='new')
-        if self.toolbarButtons:
-            for i, b in enumerate(self.toolbarButtons):
-                self._addButton(b, i)
-
-        subBody = tk.Frame(bodyFrame)
-        subBody.grid(row=1, column=0, sticky='news', padx=5, pady=5)
-        ListDialog.body(self, subBody)
-        if self._itemDoubleClick:
-            self.tree.itemDoubleClick = self._itemDoubleClick
-
-    def _addButton(self, button, col):
-        btn = tk.Label(self.toolbarFrame, text=button.text,
-                       image=self.getImage(button.icon),
-                       compound=tk.LEFT, cursor='hand2', bg='white')
-        btn.grid(row=0, column=col, sticky='nw', padx=(5, 0), pady=(5, 0))
-        btn.bind('<Button-1>', button.command)
-
-
-class FlashMessage:
-    def __init__(self, master, msg, delay=5, relief='solid', func=None):
-        self.root = tk.Toplevel(master=master)
-        # hides until know geometry
-        self.root.withdraw()
-        self.root.wm_overrideredirect(1)
-        tk.Label(self.root, text="   %s   " % msg,
-                 bd=1, bg='DodgerBlue4', fg='white').pack()
-        gui.centerWindows(self.root, refWindows=master)
-        self.root.deiconify()
-        self.root.grab_set()
-        self.msg = msg
-
-        if func:
-            self.root.update_idletasks()
-            self.root.after(10, self.process, func)
+        if self.colors and fmt is not None:
+            if fmt.startswith('link:'):
+                fname = fmt.split(':', 1)[-1]
+                self.insert(tk.END, txt, self.hm.add(lambda: openTextFileEditor(fname)))
+            else:
+                self.insert(tk.END, txt, fmt)
         else:
-            self.root.after(int(delay * 1000), self.close)
-        self.root.wait_window(self.root)
-
-    def process(self, func):
-        func()
-        self.root.destroy()
+            self.insert(tk.END, txt)
 
-    def close(self):
-        self.root.destroy()
-
-
-class FloatingMessage:
-    def __init__(self, master, msg, xPos=750, yPos=80, textWidth=280,
-                 font='Helvetica', size=12, bd=1, bg='#6E6E6E', fg='white'):
-        self.floatingMessage = tk.Label(master, text="   %s   " % msg,
-                                        bd=bd, bg=bg, fg=fg)
-        self.floatingMessage.place(x=xPos, y=yPos, width=textWidth)
-        self.floatingMessage.config(font=(font, size))
-
-    def show(self):
-        self.floatingMessage.update_idletasks()
-
-    def close(self):
-        self.floatingMessage.destroy()
-
-
-class FileBrowseDialog(Dialog):
-    """Dialog to select files from the filesystem."""
-
-    def __init__(self, parent, title, provider, message=None, **args):
-        """ From args:
-                message: message tooltip to show when browsing.
-                selected: the item that should be selected.
-        """
-        self.value = None
-        self.provider = provider
-        self.message = args.get('message', None)
-        Dialog.__init__(self, parent, title,
-                        buttons=[('Select', RESULT_YES), ('Cancel', RESULT_CANCEL)])
-
-    def body(self, bodyFrame):
-        bodyFrame.config(bg='white')
-        gui.configureWeigths(bodyFrame)
-        self._createTree(bodyFrame)
-        if self.message:
-            label = tk.Label(bodyFrame, text=self.message, bg='white',
-                             image=self.getImage('fa-lightbulb-o.gif'), compound=tk.LEFT)
-            label.grid(row=1, column=0, sticky='nw', padx=5, pady=5)
-        self.initial_focus = self.tree
-
-    def _createTree(self, parent):
-        self.tree = BoundTree(parent, self.provider)
-
-    def apply(self):
-        index = self.tree.index(self.tree.getFirst())
-        self.value = self.tree._objects[index]
-
-    def validate(self):
-        if self.tree.getFirst() is None:
-            showError("Validation error", "Please select an element", self)
-            return False
-        return True
+    def _notifyLine(self, line):
+        if '\r' in self.lastLine and '\r' in line:
+            self._removeLastLine()
+            self.addNewline()
+            
+        self.lastLine = line        
+        
+    def readFile(self, clear=False):
+        self.setReadOnly(False)
+        
+        if clear:
+            self.offset = 0
+            self.lineNo = 0
+            self.clear()
+
+        if os.path.exists(self.filename):
+            self.offset, self.lineNo = renderTextFile(self.filename, 
+                                                      self._addChunk,
+                                                      offset=self.offset, 
+                                                      lineNo=self.lineNo,
+                                                      maxSize=self.maxSize, 
+                                                      notifyLine=self._notifyLine,
+                                                      errors='replace')
+
+        # I'm cancelling this message. If file does not exist ... text is empty.
+        # else:
+        #     self.insert(tk.END, "File '%s' doesn't exist" % self.filename)
+
+        self.setReadOnly(True)
+        # self.goEnd()
+      
+    def doRefresh(self):
+        # First stop pending refreshes
+        if self.refreshAlarm:
+            self.after_cancel(self.refreshAlarm)
+            self.refreshAlarm = None
+
+        self.readFile()
+
+        if self.t_refresh > 0:
+            self.refreshAlarm = self.after(self.t_refresh*1000, self.doRefresh)
+
+
+class TextFileViewer(tk.Frame):
+    """ Implementation of a simple text file viewer """
+    
+    # Not used? --> LabelBgColor = "white"
+    
+    def __init__(self, master, fileList=[],
+                 allowSearch=True, allowRefresh=True, allowOpen=False,
+                 font=None, maxSize=400, width=100, height=30):
+        tk.Frame.__init__(self, master)
+        self.searchList = None
+        self.lastSearch = None
+        self.refreshAlarm = None
+        self._lastTabIndex = None
+        self.fileList = []  # Files being visualized
+        self.taList = []  # Text areas (OutputText, a scrollable TkText)
+        self.fontDict = {}
+        self._allowSearch = allowSearch
+        self._allowRefresh = allowRefresh
+        self._allowOpen = allowOpen
+        self._font = font  # allow a font to be passed as argument to be used
+        self.maxSize = maxSize
+        self.width = width
+        self.height = height
+
+        self.createWidgets(fileList)
+        self.master = master
+        self.addBinding()
+        
+    def addFile(self, filename):
+        self.fileList.append(filename)
+        self._addFileTab(filename)
+        
+    def clear(self):
+        """ Remove all added files. """
+        self.fileList = []
+        for _ in self.taList:
+            self.notebook.forget(0)       
+        self.taList = []
+        self._lastTabIndex = None
+        
+    def _addFileTab(self, filename):
+        tab = tk.Frame(self.notebook)
+        tab.rowconfigure(0, weight=1)
+        tab.columnconfigure(0, weight=1)
+        kwargs = {'bg': 'black',
+                  'fg': 'white'}
+        
+        if self._font is not None:
+            kwargs['font'] = self._font
+
+        t = OutputText(tab, filename, width=self.width, height=self.height,
+                       maxSize=self.maxSize, **kwargs)
+        t.frame.grid(column=0, row=0, padx=5, pady=5, sticky='nsew')
+        self.taList.append(t)
+        tabText = "   %s   " % os.path.basename(filename)
+        self.notebook.add(tab, text=tabText)        
+    
+    def createWidgets(self, fileList):
+        # registerCommonFonts()
+        self.columnconfigure(0, weight=1)
+        self.rowconfigure(1, weight=1)        
+
+        # Create toolbar frame
+        toolbarFrame = tk.Frame(self)
+        toolbarFrame.grid(column=0, row=0, padx=5, sticky='new')
+        gui.configureWeigths(toolbarFrame)
+        # Add the search box
+        right = tk.Frame(toolbarFrame)
+        right.grid(column=1, row=0, sticky='ne')        
+        self.searchVar = tk.StringVar()
+        if self._allowSearch:
+            tk.Label(right, text='Search:').grid(row=0, column=3, padx=5)
+            self.searchEntry = tk.Entry(right, textvariable=self.searchVar,
+                                        font=self._font)
+            self.searchEntry.grid(row=0, column=4, sticky='ew', padx=5)
+
+            # self.searchEntry.bind('<Return>', self.findText)
+            # self.searchEntry.bind('<KP_Enter>', self.findText)
+            # # btn = IconButton(right, "Search", Icon.ACTION_SEARCH,
+            #                  tooltip=Message.TOOLTIP_SEARCH,
+            #                  command=self.findText, bg=None)
+            # btn.grid(row=0, column=5, padx=(0, 5))
+
+            btn = IconButton(right, "Next", Icon.ACTION_FIND_NEXT,
+                             tooltip=Message.TOOLTIP_SEARCH_NEXT,
+                             command=self.findText, bg=None)
+            btn.grid(row=0, column=5, padx=(0, 5))
+
+            btn = IconButton(right, "Previous", Icon.ACTION_FIND_PREVIOUS,
+                             tooltip=Message.TOOLTIP_SEARCH_PREVIOUS,
+                             command=self.findPrevText, bg=None)
+            btn.grid(row=0, column=6, padx=(0, 5))
+
+        if self._allowRefresh:
+            btn = IconButton(right, "Refresh", Icon.ACTION_REFRESH,
+                             tooltip=Message.TOOLTIP_REFRESH,
+                             command=self._onRefresh, bg=None)
+            btn.grid(row=0, column=7, padx=(0, 5), pady=2)
+        if self._allowOpen:
+            btn = IconButton(right, "Open external", Icon.ACTION_REFERENCES,
+                             tooltip=Message.TOOLTIP_EXTERNAL,
+                             command=self._openExternal, bg=None)
+            btn.grid(row=0, column=8, padx=(0, 5), pady=2)
+
+        # Create tabs frame
+        tabsFrame = tk.Frame(self)
+        tabsFrame.grid(column=0, row=1, padx=5, pady=(0, 5), sticky="nsew")
+        tabsFrame.columnconfigure(0, weight=1)
+        tabsFrame.rowconfigure(0, weight=1)
+        self.notebook = ttk.Notebook(tabsFrame)  
+        self.notebook.rowconfigure(0, weight=1)
+        self.notebook.columnconfigure(0, weight=1)      
+        for f in fileList:
+            self._addFileTab(f)
+        self.notebook.grid(column=0, row=0, sticky='nsew', padx=5, pady=5)   
+        self.notebook.bind('<<NotebookTabChanged>>', self._tabChanged)
+
+    def _tabChanged(self, e=None):
+        self._lastTabIndex = self.notebook.select()
+        # reset the search
+        self.lastSearch = None
+        # Setting the focus, captures it when selecting protocols and
+        # therefore "deleting" using keys or other future shortcut for the canvas
+        # will not work.
+        # self.searchEntry.focus_set()
+
+    def addBinding(self):
+
+        shortcutDefinitions = [(lambda e: self.findText(), "Trigger the search", ['<Return>']),
+                               (lambda e: self.findText(), "Trigger the search", ['<KP_Enter>']),
+                               (lambda e: self.findText(matchCase=True), "Trigger a case sensitive search", ['<Shift-Return>']),
+                               (lambda e: self.findText(), "Move to the next highlighted item", ["<Down>", '<F3>']),
+                               (lambda e: self.findText(-1), "Move to the previous highlighted item", ["<Up>", '<Shift-F3>']),
+                               (lambda e: self.modifyFontSize(pw.Config.SCIPION_FONT_SIZE + 2), "Increase the font size",["<Control-KP_Add>"]),
+                               (lambda e: self.modifyFontSize(pw.Config.SCIPION_FONT_SIZE), "Increase the font size",["<Control-KP_Subtract>"]),
+                               ]
+        tooltip = "Shortcuts:"
+
+        for callback, help, keys in shortcutDefinitions:
+            tooltip += "\n" + help + ": "
+            for key in keys:
+                self.searchEntry.bind(key, callback)
+                tooltip += key
+
+        # Add a tooltip
+        ToolTip(self.searchEntry, tooltip, 800)
+
+    def getIndex(self):
+        """ Return the index of the selected tab. """
+        selected = self.notebook.select()
+        if selected:
+            return self.notebook.index(selected)
+        return -1
+    
+    def setIndex(self, index):
+        """ Select the tab with the given index. """
+        if index != -1:
+            self.notebook.select(self.notebook.tabs()[index])
+    
+    def selectedText(self):
+        index = self.getIndex()
+        if index != -1:
+            return self.taList[index]
+        return None
+    
+    def changeFont(self, event=""):
+        for font in self.fontDict.values():
+            gui.changeFontSize(font, event)
+              
+    def refreshAll(self, clear=False, goEnd=False):
+        """ Refresh all output textareas. """
+        for ta in self.taList:
+            ta.readFile(clear)
+            if goEnd:
+                ta.goEnd()
+        if self._lastTabIndex is not None:
+            self.notebook.select(self._lastTabIndex)
+            
+    def _onRefresh(self, e=None):
+        """ Action triggered when the 'Refresh' icon is clicked. """
+        self.refreshAll(clear=False, goEnd=True)
+        
+    def refreshOutput(self, e=None):
+        if self.refreshAlarm:
+            self.after_cancel(self.refreshAlarm)
+            self.refreshAlarm = None
+        text = self.selectedText()
+        if text:
+            text.readFile()
+        
+    def changePosition(self, index):
+        self.selectedText().see(index)
+
+    def findPrevText(self):
+        self.findText(-1)
+
+    def modifyFontSize(self, newSize):
+        text = self.selectedText()
+        text['font']=(None, newSize)
+
+    def findText(self, direction=1, matchCase=0):
+        text = self.selectedText()
+        str = self.searchVar.get()
+        if text:
+            if str is None or str != self.lastSearch:
+                self.buildSearchList(text, str, matchCase=matchCase)
+                self.lastSearch = str
+
+            else:
+                self.nextSearchIndex(text, direction)
+            self.searchEntry.focus_set()
+        
+    def buildSearchList(self, text, str, matchCase=0):
+        text.tag_remove('found', '1.0', tk.END)
+        list = []
+        if str:
+            idx = '1.0'
+            while True:
+                idx = text.search(str, idx, nocase=not matchCase, stopindex=tk.END)
+                if not idx:
+                    break
+                lastidx = '%s+%dc' % (idx, len(str))
+                text.tag_add('found', idx, lastidx)
+                list.append((idx, lastidx))
+                idx = lastidx
+        text.tag_config('found', foreground='white', background='blue')
+        # Set class variables
+        self.searchList = list
+        self.currentIndex = -1
+        self.nextSearchIndex(text)  # select first element
+    
+    def nextSearchIndex(self, text, direction=1):
+        # use direction=-1 to go backward
+        text.tag_remove('found_current', '1.0', tk.END)
+        if len(self.searchList) == 0:
+            return
+        self.currentIndex = (self.currentIndex + direction) % len(self.searchList)
+        idx, lastidx = self.searchList[self.currentIndex]
+        text.tag_config('found_current', foreground='yellow', background='red')
+        text.tag_add('found_current', idx, lastidx)
+        text.see(idx)
+        
+    def _openExternal(self):
+        """ Open a new window with an external viewer. """
+        if envVarOn('SCIPION_EXTERNAL_VIEWER'):
+            if not self.taList:
+                return
+            openTextFileEditor(self.taList[max(self.getIndex(), 0)].filename)
+        else:
+            showTextFileViewer("File viewer", self.fileList, self.windows)
+  
+  
+def openTextFile(filename):
+    """ Open a text file with an external or default viewer. """
+    if envVarOn('SCIPION_EXTERNAL_VIEWER'):
+        openTextFileEditor(filename)
+    else:
+        showTextFileViewer("File viewer", [filename])    
+    
+    
+def openTextFileEditor(filename, tkParent=None):
+    try:
+        _open_cmd(filename, tkParent)
+    except:
+        showTextFileViewer("File viewer", [filename])
+    
+    
+def showTextFileViewer(title, filelist, parent=None, main=False):
+    w = gui.Window(title, parent, minsize=(600, 400))
+    viewer = TextFileViewer(w.root, filelist, maxSize=-1, font=w.font)
+    viewer.grid(row=0, column=0, sticky='news')
+    gui.configureWeigths(w.root)
+    w.show()
+
+
+if __name__ == '__main__':
+    root = tk.Tk()
+    root.withdraw()
+    root.title("View files")
+    l = TextFileViewer(root, fileList=sys.argv[1:])
+    l.pack(side=tk.TOP, fill=tk.BOTH)
+    gui.centerWindows(root)
+    root.deiconify()
+    root.mainloop()
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/form.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/form.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,36 +24,37 @@
 # *
 # **************************************************************************
 """
 This modules implements the automatic
 creation of protocol form GUI from its
 params definition.
 """
+import logging
+logger = logging.getLogger(__name__)
 import os
 import tkinter as tk
 import tkinter.ttk as ttk
 from collections import OrderedDict
 from datetime import datetime
 
 import pyworkflow as pw
 import pyworkflow.utils as pwutils
 import pyworkflow.object as pwobj
 import pyworkflow.protocol as pwprot
 from pyworkflow.mapper import Mapper
 from pyworkflow.viewer import DESKTOP_TKINTER
-from pyworkflow.protocol.constants import MODE_RESTART
+from pyworkflow.protocol.constants import MODE_RESTART, MODE_RESUME
 
-from . import gui
+from . import gui, RESULT_RUN_SINGLE
 from pyworkflow.gui.project.utils import getStatusColorFromRun
 from .gui import configureWeigths, Window
 from .browser import FileBrowserWindow
 from .widgets import Button, HotButton, IconButton
 from .dialog import (showInfo, showError, showWarning, EditObjectDialog,
-                     ListDialog, askYesNo, Dialog, RESULT_CANCEL,
-                     askSingleAllCancel, RESULT_RUN_ALL, RESULT_RUN_SINGLE)
+                     ListDialog, Dialog, RESULT_CANCEL,  RESULT_RUN_ALL)
 from .canvas import Canvas
 from .tree import TreeProvider, BoundTree
 from .text import Text
 from ..project.project import ModificationNotAllowedException
 
 THREADS = 'Threads'
 MPI = 'MPI'
@@ -214,14 +215,19 @@
     def remove(self):
         """ Remove first element selected. """
         values = self.getSelectedObjects()
         for v in values:
             self.provider.removeObject(v)
         self._updateObjectsList()
 
+    def clear(self):
+        self.provider.clear()
+        self._updateObjectsList()
+
+
     def getSelectedObjects(self):
         return self.tree.getSelectedObjects()
 
     def get(self):
         return self.provider.getObjects()
 
 
@@ -297,14 +303,17 @@
     def getColumns(self):
         return [('Object', 250), ('Info', 150)]
 
     def getObjectInfo(self, obj):
         label, info = getPointerLabelAndInfo(obj, self._mapper)
         return {'key': obj._strId, 'text': label, 'values': ('  ' + info,)}
 
+    def clear(self):
+        self._objectDict.clear()
+
 
 class ComboVar:
     """ Create a variable that display strings (for combobox)
     but the values are integers (for the underlying EnumParam).
     """
 
     def __init__(self, enum):
@@ -474,32 +483,50 @@
                 try:
                     # paramName and attr must be set to None 
                     # Otherwise, if a protocol has failed and the corresponding output object of type XX does not exist 
                     # any other protocol that uses objects of type XX as input will not be able to choose then using
                     # the magnifier glass (object selector of type XX)
                     paramName = None
                     attr = None
-                    for paramName, attr in prot.iterOutputAttributes():
+                    for paramName, attr in prot.iterOutputAttributes(includePossible=True):
                         def _checkParam(paramName, attr):
                             # If attr is a sub-classes of any desired one, add it to the list
                             # we should also check if there is a condition, the object
                             # must comply with the condition
                             p = None
-                            if (any(isinstance(attr, c) for c in classes) and
-                                    (not condition or
-                                     attr.evalCondition(condition))):
-                                p = pwobj.Pointer(prot, extended=paramName)
-                                p._allowsSelection = True
-                                objects.append(p)
+
+                            match = False
+                            cancelConditionEval = False
+                            possibleOutput = isinstance(attr, type)
+
+                            # Go through all compatible Classes coming from in pointerClass string
+                            for c in classes:
+                                # If attr is instance
+                                if isinstance(attr, c):
+                                    match = True
+                                    break
+                                # If it is a class already: "possibleOutput" case. In this case attr is the class and not
+                                # an instance of c. In this special case
+                                elif possibleOutput and attr == c:
+                                    match = True
+                                    cancelConditionEval = True
+
+                            # If attr matches the class
+                            if match:
+                                if cancelConditionEval or not condition or attr.evalCondition(condition):
+                                    p = pwobj.Pointer(prot, extended=paramName)
+                                    p._allowsSelection = True
+                                    objects.append(p)
+                                    return
 
                             # JMRT: For all sets, we don't want to include the
                             # subitems here for performance reasons (e.g SetOfParticles)
                             # Thus, a Set class can define EXPOSE_ITEMS = True
                             # to enable the inclusion of its items here
-                            if getattr(attr, 'EXPOSE_ITEMS', False):
+                            if getattr(attr, 'EXPOSE_ITEMS', False) and not possibleOutput:
                                 # If the ITEM type match any of the desired classes
                                 # we will add some elements from the set
                                 if (attr.ITEM_TYPE is not None and
                                         any(issubclass(attr.ITEM_TYPE, c) for c in classes)):
                                     if p is None:  # This means the set have not be added
                                         p = pwobj.Pointer(prot, extended=paramName)
                                         p._allowsSelection = False
@@ -538,15 +565,15 @@
 
         return objects
 
     def _sortObjects(self, objects):
         objects.sort(key=self.objectKey, reverse=not self.isSortingAscending())
 
     def objectKey(self, pobj):
-
+        """ Returns the value to be evaluated during sorting based on _sortingColumnName"""
         obj = self._getParentObject(pobj, pobj)
 
         if self._sortingColumnName == SubclassesTreeProvider.CREATION_COLUMN:
             return self._getObjectCreation(obj.get())
         elif self._sortingColumnName == SubclassesTreeProvider.INFO_COLUMN:
             return self._getObjectInfoValue(obj.get())
         elif self._sortingColumnName == SubclassesTreeProvider.ID_COLUMN:
@@ -590,22 +617,24 @@
 
     @staticmethod
     def _getObjectId(pobj):
         return pobj.getObjValue().getObjId()
 
     @staticmethod
     def _getObjectCreation(obj):
-
-        return obj.getObjCreation() if obj.getObjCreation() else "Empty"
+        """ Returns the Object creation time stamp or 'Not ready' for those not yet ready or possibleOutputs"""
+        return obj.getObjCreation() if obj is not None and obj.getObjCreation() else "Not ready"
 
     @staticmethod
     def _getObjectInfoValue(obj):
-
-        return str(obj).replace(obj.getClassName(), '')
-
+        """ Returns the best summary of the object in a string."""
+        if obj is not None:
+            return str(obj).replace(obj.getClassName(), '')
+        else: # possible Outputs are not output already so here comes None
+            return "Possible output"
     def _getPointerLabel(self, pobj, parent=None):
 
         # If parent is not provided, try to get it, it might have none.
         if parent is None:
             parent = self._getParentObject(pobj)
 
         # If there is no parent
@@ -866,21 +895,21 @@
                                     bg=bgColor, name="sectionheaderlabel")
         self.headerLabel.grid(row=0, column=0, sticky='nw')
 
     def _createContent(self):
         self.canvasFrame = tk.Frame(self, name="sectioncontentframe")
         configureWeigths(self.canvasFrame)
         self.canvas = Canvas(self.canvasFrame, width=625, height=self.height,
-                             bg="white", highlightthickness=0, name="sectioncanvas")
+                             bg=pw.Config.SCIPION_BG_COLOR, highlightthickness=0, name="sectioncanvas")
         self.canvas.grid(row=0, column=0, sticky='news')
         self.canvasFrame.grid(row=1, column=0, sticky='news')
 
         configureWeigths(self.canvas)
 
-        self.contentFrame = tk.Frame(self.canvas, bg='white', bd=0,
+        self.contentFrame = tk.Frame(self.canvas, bg=pw.Config.SCIPION_BG_COLOR, bd=0,
                                      name="sectioncanvasframe")
         self.contentFrame.grid(row=1, column=0, sticky='news')
         self.contentId = self.canvas.create_window(0, 0, anchor=tk.NW,
                                                    window=self.contentFrame)
 
         self.contentFrame.bind('<Configure>', self._configure_interior)
         self.canvas.bind('<Configure>', self._configure_canvas)
@@ -990,17 +1019,17 @@
 
     def __init__(self, row, paramName, param, window, parent, value,
                  callback=None, visualizeCallback=None, column=0,
                  showButtons=True):
         self.window = window
         self._protocol = self.window.protocol
         if self._protocol.getProject() is None:
-            print(">>> ERROR: Project is None for protocol: %s, "
+            logger.error(">>> ERROR: Project is None for protocol: %s, "
                   "start winpdb to debug it" % self._protocol)
-            pwutils.startDebugger()
+
         self.row = row
         self.column = column
         self.paramName = paramName
         self.param = param
         self.parent = parent
         self.visualizeCallback = visualizeCallback
         self.var = None
@@ -1024,37 +1053,37 @@
             self._labelSticky = 'ne'
             self._padx, self._pady = 2, 2
             self._entryWidth = 10
             if self.param.isImportant():
                 self._labelFont = self.window.fontBold
             self.parent.columnconfigure(0, minsize=250)
             self.parent.columnconfigure(1, minsize=250)
-            self.btnFrame = tk.Frame(self.parent, bg='white')
+            self.btnFrame = tk.Frame(self.parent, bg=pw.Config.SCIPION_BG_COLOR)
         else:
             self.btnFrame = None
             self._labelSticky = 'ne'
             self._padx, self._pady = 2, 0
             self._labelFont = self.window.fontItalic
             self._entryWidth = 8
         self._onlyLabel = False
 
     def _getParamLabel(self):
         return self.param.label.get()
 
     def _createLabel(self):
-        bgColor = 'white'
+        bgColor = pw.Config.SCIPION_BG_COLOR
 
         if self.param.isExpert():
             bgColor = 'lightgrey'
 
         self.label = tk.Label(self.parent, text=self._getParamLabel(),
                               bg=bgColor, font=self._labelFont, wraplength=500)
 
     def _createContent(self):
-        self.content = tk.Frame(self.parent, bg='white')
+        self.content = tk.Frame(self.parent, bg=pw.Config.SCIPION_BG_COLOR)
         gui.configureWeigths(self.content)
         # self.var should be set after this
         self._createContentWidgets(self.param, self.content)
 
     def _addButton(self, text, imgPath, cmd):
         if self.btnFrame:
             btn = IconButton(self.btnFrame, text, imgPath,
@@ -1074,14 +1103,17 @@
 
     def _showWarning(self, msg):
         showWarning("Warning", msg, self.parent)
 
     def _showWizard(self, e=None):
         wizClass = self.window.wizards[self.wizParamName]
         wizard = wizClass()
+        # wizParamName: form attribute, the wizard object can check from which parameter it was called
+        # Used into VariableWizard objects (scipion-chem), where input and output parameters used for each wizard are defined
+        self.window.wizParamName = self.wizParamName
         wizard.show(self.window)
 
     def _findParamWizard(self):
         """ Search if there are registered wizards for this param
         or any of its subparams (for the case of Line groups)
         """
         if self.paramName in self.window.wizards:
@@ -1093,30 +1125,37 @@
                 if name in self.window.wizards:
                     self.wizParamName = name
                     return True
         # Search in sub-params
         return False
 
     @staticmethod
-    def createBoolWidget(parent, **args):
+    def createBoolWidget(parent, display=pwprot.BooleanParam.DISPLAY_YES_NO, **args):
         """ Return a BoolVar associated with a yes/no selection.
         **args: extra arguments passed to tk.Radiobutton and tk.Frame
             constructors.
+
+            :param checkbox: will use a Checkbutton instead.
         """
         var = BoolVar()
         frameArgs = dict(args)
         if 'font' in frameArgs:
             del frameArgs['font']
         frame = tk.Frame(parent, **frameArgs)
-        rb1 = tk.Radiobutton(frame, text='Yes', variable=var.tkVar,
-                             highlightthickness=0, value=1, **args)
-        rb1.grid(row=0, column=0, padx=2, sticky='w')
-        rb2 = tk.Radiobutton(frame, text='No', variable=var.tkVar,
-                             highlightthickness=0, value=0, **args)
-        rb2.grid(row=0, column=1, padx=2, sticky='w')
+
+        if display == pwprot.BooleanParam.DISPLAY_CHECKBOX:
+            chk = tk.Checkbutton(frame, variable=var.tkVar, **args)
+            chk.grid(row=0, column=0, padx=2, sticky="w")
+        else:
+            rb1 = tk.Radiobutton(frame, text='Yes', variable=var.tkVar,
+                                 highlightthickness=0, value=1, **args)
+            rb1.grid(row=0, column=0, padx=2, sticky='w')
+            rb2 = tk.Radiobutton(frame, text='No', variable=var.tkVar,
+                                 highlightthickness=0, value=0, **args)
+            rb2.grid(row=0, column=1, padx=2, sticky='w')
 
         return var, frame
 
     def _createContentWidgets(self, param, content):
         """Create the specific widgets inside the content frame"""
         # Create widgets for each type of param
         t = type(param)
@@ -1127,47 +1166,49 @@
         selectFunc = None
         removeFunc = None
 
         if t is pwprot.HiddenBooleanParam:
             var = 0
 
         elif t is pwprot.BooleanParam:
-            var, frame = ParamWidget.createBoolWidget(content, bg='white',
+            var, frame = ParamWidget.createBoolWidget(content, display=param.display,
+                                                      bg=pw.Config.SCIPION_BG_COLOR,
                                                       font=self.window.font)
             frame.grid(row=0, column=0, sticky='w')
 
         elif t is pwprot.EnumParam:
             var = ComboVar(param)
             if param.display == pwprot.EnumParam.DISPLAY_COMBO:
                 combo = ttk.Combobox(content, textvariable=var.tkVar,
                                      state='readonly', font=self.window.font)
                 combo['values'] = param.choices
                 combo.grid(row=0, column=0, sticky='we')
             elif param.display == pwprot.EnumParam.DISPLAY_LIST:
                 for i, opt in enumerate(param.choices):
                     rb = tk.Radiobutton(content, text=opt, variable=var.tkVar,
                                         value=opt, font=self.window.font,
-                                        bg='white', highlightthickness=0)
+                                        bg=pw.Config.SCIPION_BG_COLOR, highlightthickness=0)
                     rb.grid(row=i, column=0, sticky='w')
             elif param.display == pwprot.EnumParam.DISPLAY_HLIST:
-                rbFrame = tk.Frame(content, bg='white')
+                rbFrame = tk.Frame(content, bg=pw.Config.SCIPION_BG_COLOR)
                 rbFrame.grid(row=0, column=0, sticky='w')
                 for i, opt in enumerate(param.choices):
                     rb = tk.Radiobutton(rbFrame, text=opt, variable=var.tkVar,
                                         value=opt, font=self.window.font,
-                                        bg='white')
+                                        bg=pw.Config.SCIPION_BG_COLOR)
                     rb.grid(row=0, column=i, sticky='w', padx=(0, 5))
             else:
                 raise Exception("Invalid display value '%s' for EnumParam"
                                 % str(param.display))
 
         elif t is pwprot.MultiPointerParam:
             tp = MultiPointerTreeProvider(self._protocol.mapper)
             tree = BoundTree(content, tp, height=5)
             var = MultiPointerVar(tp, tree)
+            var.trace('w', self.window._onPointerChanged)
             tree.grid(row=0, column=0, sticky='we')
             self._addButton("Select", pwutils.Icon.ACTION_SEARCH, self._browseObject)
             self._addButton("Remove", pwutils.Icon.ACTION_DELETE, self._removeObject)
             self._selectmode = 'extended'  # allows multiple object selection
             self.visualizeCallback = self._visualizeMultiPointerParam
 
         elif t is pwprot.PointerParam or t is pwprot.RelationParam:
@@ -1234,17 +1275,17 @@
                     sticky = 'w'
             else:
                 selectFunc = self._browseScalar
                 var = ScalarWithPointerVar(self._protocol,
                                            self.window._onPointerChanged)
                 self._selectmode = 'browse'
                 sticky = 'ew'
-
+            state = tk.DISABLED if param.readOnly else tk.NORMAL
             entry = tk.Entry(content, width=entryWidth, textvariable=var,
-                             font=self.window.font)
+                             font=self.window.font, state=state)
 
             # Select all content on focus
             entry.bind("<FocusIn>",
                        lambda event: entry.selection_range(0, tk.END))
 
             entry.grid(row=0, column=0, sticky=sticky)
 
@@ -1340,24 +1381,28 @@
         dlg = ListDialog(self.parent, title, tp,
                          "Double click selects the item, right-click allows "
                          "you to visualize it",
                          validateSelectionCallback=validateSelected,
                          selectmode=self._selectmode, selectOnDoubleClick=True)
 
         if dlg.values:
-            if isinstance(self.param, pwprot.MultiPointerParam):
+            if self.isMultiPointer():
                 self.set(dlg.values)
             elif isinstance(self.param, pwprot.PointerParam):
                 self.set(dlg.values[0])
             else:
                 raise Exception('Invalid param class: %s' % type(self.param))
 
+    def isMultiPointer(self):
+        """ True if dealing with MultiPointer params """
+        return isinstance(self.param, pwprot.MultiPointerParam)
+
     def _browseScalar(self, e=None):
         """Select a scalar from outputs
-        This function is suppose to be used only for Scalar Params
+        This function is supposed to be used only for Scalar Params
         It's a copy of browseObject...so there could be a refactor here."""
         value = self.get()
         selected = []
         if isinstance(value, list):
             selected = value
         else:
             selected = [value]
@@ -1385,14 +1430,24 @@
         if dlg.values:
             self.set(dlg.values[0])
 
     def _removeObject(self, e=None):
         """ Remove an object from a MultiPointer param. """
         self.var.remove()
 
+    def clear(self):
+
+        # If dealing with Multipointers ...
+        if self.isMultiPointer():
+            # .. use var clear to remove all eletents since
+            # _removeObject() will remove only the selected ones
+            self.var.clear()
+        else:
+            self._removeObject()
+
     def _browseRelation(self, e=None):
         """Select a relation from DB
         This function is suppose to be used only for RelationParam. """
         try:
             tp = RelationsTreeProvider(self._protocol, self.param,
                                        selected=self.get())
             dlg = ListDialog(self.parent, "Select object", tp,
@@ -1533,15 +1588,15 @@
         pass
 
     def _createLabel(self):
         pass
 
     def _createContent(self):
         self.content = tk.LabelFrame(self.parent, text=self.param.getLabel(),
-                                     bg='white')
+                                     bg=pw.Config.SCIPION_BG_COLOR)
         gui.configureWeigths(self.content, column=1)
 
     def show(self):
         self.content.grid(row=self.row, column=0, sticky='news', columnspan=6,
                           padx=5, pady=5)
 
     def hide(self):
@@ -1586,22 +1641,23 @@
         Window.__init__(self, title, master, icon=pwutils.Icon.SCIPION_ICON_PROT,
                         weight=False, minsize=(600, 450), **kwargs)
 
         # Some initialization
         self.callback = callback
         self.widgetDict = {}  # Store tkVars associated with params
         self.visualizeDict = kwargs.get('visualizeDict', {})
+        self.disableRunMode = kwargs.get('disableRunMode', False)
         self.bindings = []
         self.hostList = hostList
         self.protocol = protocol
         # This control when to close or not after execute
         self.visualizeMode = kwargs.get('visualizeMode', False)
-        self.headerBgColor = pwutils.Color.RED_COLOR
+        self.headerBgColor = pw.Config.SCIPION_MAIN_COLOR
         if self.visualizeMode:
-            self.headerBgColor = pwutils.Color.DARK_GREY_COLOR
+            self.headerBgColor = pwutils.Color.ALT_COLOR_DARK
         # Allow to open child protocols form (for workflows)
         self.childMode = kwargs.get('childMode', False)
         self.updateProtocolCallback = kwargs.get('updateProtocolCallback', None)
         domain = pw.Config.getDomain()
         self.wizards = domain.findWizards(protocol, DESKTOP_TKINTER)
 
         # Call legacy for compatibility on protocol
@@ -1642,21 +1698,28 @@
         package = prot.getClassPackage()
 
         # Consider legacy protocols
         if self._isLegacyProtocol():
             t = ('  Missing protocol: %s'
                  % (Mapper.getObjectPersistingClassName(prot)))
         else:
-            t = '  Protocol: %s' % (prot.getClassLabel())
+            t = '  %s' % (prot.getClassLabel())
 
         logoPath = prot.getPluginLogoPath() or getattr(package, '_logo', '')
 
         if logoPath and os.path.exists(logoPath):
+            # Tolerate error loading icons
+            try:
+                img = self.getImage(logoPath, maxheight=40)
+            except Exception as e:
+                print("Can't load plugin icon (%s): %s" % (logoPath, e))
+                img = None
+
             headerLabel = tk.Label(headerFrame, text=t, font=self.fontBig,
-                                   image=self.getImage(logoPath, maxheight=40),
+                                   image=img,
                                    compound=tk.LEFT)
         else:
             headerLabel = tk.Label(headerFrame, text=t, font=self.fontBig)
         headerLabel.grid(row=0, column=0, padx=5, pady=(5, 0), sticky='nw')
 
         # Add status label
         status = prot.status.get()
@@ -1717,15 +1780,15 @@
             if not (allowThreads or allowMpi or allowGpu):
                 return
 
             self._createHeaderLabel(runFrame, pwutils.Message.LABEL_PARALLEL, bold=True,
                                     sticky='e', row=r, pady=0)
 
             if allowThreads or allowMpi:
-                procFrame = tk.Frame(runFrame, bg='white')
+                procFrame = tk.Frame(runFrame, bg=pw.Config.SCIPION_BG_COLOR)
                 r2 = 0
                 c2 = 0
                 sticky = 'e'
 
                 if mode == pwprot.STEPS_PARALLEL:
                     self.procTypeVar = tk.StringVar()
 
@@ -1736,19 +1799,19 @@
                             prot.numberOfThreads.set(1)
                         else:
                             procs = numberOfThreads
                             self.procTypeVar.set(THREADS)
                             prot.numberOfMpi.set(1)
 
                         self.procTypeVar.trace('w', self._setThreadsOrMpi)
-                        procCombo = tk.Frame(procFrame, bg='white')
+                        procCombo = tk.Frame(procFrame, bg=pw.Config.SCIPION_BG_COLOR)
                         for i, opt in enumerate([THREADS, MPI]):
                             rb = tk.Radiobutton(procCombo, text=opt,
                                                 variable=self.procTypeVar,
-                                                value=opt, bg='white',
+                                                value=opt, bg=pw.Config.SCIPION_BG_COLOR,
                                                 highlightthickness=0)
                             rb.grid(row=0, column=i, sticky='w', padx=(0, 5))
 
                         procCombo.grid(row=r2, column=0, sticky='w', pady=15)
                         procEntry = self._createBoundEntry(procFrame,
                                                            pwutils.Message.VAR_THREADS,
                                                            func=self._setThreadsOrMpi,
@@ -1791,26 +1854,26 @@
                 procFrame.grid(row=r, column=1, sticky='ew', columnspan=2)
 
                 r += 1
 
             if allowGpu:
                 self._createHeaderLabel(runFrame, "GPU IDs", bold=True,
                                         sticky='e', row=r, column=0, pady=0)
-                gpuFrame = tk.Frame(runFrame, bg='white')
+                gpuFrame = tk.Frame(runFrame, bg=pw.Config.SCIPION_BG_COLOR)
                 gpuFrame.grid(row=r, column=1, sticky='ew', columnspan=2)
 
                 self.useGpuVar = tk.IntVar()
 
                 # For protocols that require GPU, there is not the option to choose
                 if not prot.requiresGpu():
                     self.useGpuVar.set(int(prot.useGpu.get()))
                     for i, opt in enumerate(['Yes', 'No']):
                         rb = tk.Radiobutton(gpuFrame, text=opt,
                                             variable=self.useGpuVar,
-                                            value=1 - i, bg='white',
+                                            value=1 - i, bg=pw.Config.SCIPION_BG_COLOR,
                                             highlightthickness=0)
                         rb.grid(row=0, column=i, sticky='w', padx=(0, 5), pady=5)
 
                 self.gpuListVar = tk.StringVar()
                 self.gpuListVar.set(prot.getAttributeValue(pwprot.GPU_LIST, ''))
                 gpuEntry = tk.Entry(gpuFrame, width=9, font=self.font,
                                     textvariable=self.gpuListVar)
@@ -1839,15 +1902,15 @@
         configureWeigths(commonFrame)
 
         # ---------- Run section ---------
         runSection = SectionFrame(commonFrame, label=pwutils.Message.TITLE_RUN,
                                   headerBgColor=self.headerBgColor,
                                   name="runsection")
 
-        runFrame = tk.Frame(runSection.contentFrame, bg='white', name="runframe")
+        runFrame = tk.Frame(runSection.contentFrame, bg=pw.Config.SCIPION_BG_COLOR, name="runframe")
         runFrame.grid(row=0, column=0, sticky='new')
 
         r = 0  # Run name
         self._createHeaderLabel(runFrame, pwutils.Message.LABEL_RUNNAME, bold=True,
                                 sticky='ne')
         self.runNameVar = tk.StringVar()
         entry = tk.Label(runFrame, font=self.font, width=25,
@@ -1868,26 +1931,26 @@
                          highlightthickness=0, command=self._editObjParams)
         btn.grid(row=r, column=c + 2, padx=(5, 0), pady=5, sticky='w')
 
         self.updateLabelAndCommentVars()
 
         r = 1  # Execution
 
-        modeFrame = tk.Frame(runFrame, bg='white')
+        modeFrame = tk.Frame(runFrame, bg=pw.Config.SCIPION_BG_COLOR)
 
-        if not self.protocol.isSaved():
+        if not self.disableRunMode:
             self._createHeaderLabel(runFrame, pwutils.Message.LABEL_EXECUTION,
                                     bold=True,
                                     sticky='e', row=r, pady=0)
 
             runMode = self._createBoundOptions(modeFrame, pwutils.Message.VAR_RUN_MODE,
                                                pwprot.MODE_CHOICES,
                                                self.protocol.runMode.get(),
                                                self._onRunModeChanged,
-                                               bg='white', font=self.font)
+                                               bg=pw.Config.SCIPION_BG_COLOR, font=self.font)
             runMode.grid(row=0, column=0, sticky='e', padx=(0, 5), pady=5)
             btnHelp = IconButton(modeFrame, pwutils.Message.TITLE_COMMENT, pwutils.Icon.ACTION_HELP,
                                  highlightthickness=0,
                                  command=self._createHelpCommand(pwutils.Message.HELP_RUNMODE))
             btnHelp.grid(row=0, column=2, padx=(5, 0), pady=2, sticky='e')
         modeFrame.columnconfigure(0, weight=1)
         modeFrame.grid(row=r, column=1, sticky='ew', columnspan=2)
@@ -1909,27 +1972,28 @@
         self._createParallel(runFrame, r)
 
         # ---- QUEUE ----
         self._createHeaderLabel(runFrame, pwutils.Message.LABEL_QUEUE, row=r,
                                 sticky='e',
                                 column=c)
 
-        var, frame = ParamWidget.createBoolWidget(runFrame, bg='white',
+        var, frame = ParamWidget.createBoolWidget(runFrame, bg=pw.Config.SCIPION_BG_COLOR,
                                                   font=self.font)
         btn = IconButton(frame, pwutils.Message.LABEL_BUTTON_WIZ, pwutils.Icon.ACTION_EDIT,
                          highlightthickness=0, command=self._editQueueParams, tooltip="Edit queue parameters")
         btn.grid(row=0, column=2, sticky='nes', padx=1, pady=4)
         frame.columnconfigure(2, weight=1)
 
         self._addVarBinding(pwutils.Message.VAR_QUEUE, var)
         frame.grid(row=r, column=c + 1, pady=5, sticky='ew')
 
         btnHelp = IconButton(runFrame, pwutils.Message.TITLE_COMMENT, pwutils.Icon.ACTION_HELP,
                              highlightthickness=0,
-                             command=self._createHelpCommand(pwutils.Message.HELP_USEQUEUE % pw.Config.SCIPION_HOSTS))
+                             command=self._createHelpCommand(pwutils.Message.HELP_USEQUEUE %
+                                                             (pw.Config.SCIPION_HOSTS, pw.DOCSITEURLS.HOST_CONFIG)))
 
         btnHelp.grid(row=r, column=c + 2, padx=(5, 0), pady=5, sticky='w')
 
         r = 3  # ---- Wait for other protocols (SCHEDULE) ----
         self._createHeaderLabel(runFrame, pwutils.Message.LABEL_WAIT_FOR, row=r, sticky='e',
                                 column=c, padx=(15, 5), pady=0)
         self.waitForVar = tk.StringVar()
@@ -1938,15 +2002,15 @@
                            textvariable=self.waitForVar)
         entryWf.grid(row=r, column=c + 1, padx=(0, 5), pady=5, sticky='ew')
 
         self.waitForVar.trace('w', self._setWaitFor)
 
         btnHelp = IconButton(runFrame, pwutils.Message.TITLE_COMMENT, pwutils.Icon.ACTION_HELP,
                              highlightthickness=0,
-                             command=self._createHelpCommand(pwutils.Message.HELP_WAIT_FOR))
+                             command=self._createHelpCommand(pwutils.Message.HELP_WAIT_FOR % pw.DOCSITEURLS.WAIT_FOR))
         btnHelp.grid(row=r, column=c + 2, padx=(5, 0), pady=2, sticky='e')
 
         # Run Name not editable
         # entry.configure(state='readonly')
         # Run mode
         # self._createHeaderLabel(runFrame, pwutils.Message.LABEL_RUNMODE).grid(row=1, column=0, sticky='ne', padx=5, pady=5)
         # runSection.addContent()
@@ -2017,25 +2081,25 @@
 
     def _isLegacyProtocol(self):
         return isinstance(self.protocol, pwprot.LegacyProtocol)
 
     def _createLegacyInfo(self, parent):
         frame = tk.Frame(parent, name="legacy")
         t = tk.Label(frame,
-                     text="This protocol is missing from the installation. "
+                     text="This protocol is missing in this installation. "
                           "\nThis could be because you are opening an old "
-                          "project and some of \nthe executed protocols does "
-                          "not exist in the current version and were deprecated"
+                          "project and some of \nthe executed protocols do "
+                          "not exist anymore and were deprecated"
                           ",\n or because your scipion installation requires a "
                           "plugin where this protocol can be found.\n\n"
                           "If you are a developer, it could be the case that "
                           "you have changed \nto another branch where the "
                           "protocol does not exist.\n\n"
                           "Anyway, you can still inspect the parameters by "
-                          "opening the DB from the toolbar."
+                          "opening the DB from the toolbar activating the Debug mode."
                      )
         t.grid(row=0, column=0, padx=5, pady=5)
 
         return frame
 
     def _createSections(self, parent):
         """Create section widgets"""
@@ -2074,17 +2138,21 @@
         if (not self.visualizeMode and not self.childMode and
                 not self._isLegacyProtocol()):
             # Check editable or not:
             btnState = tk.DISABLED if (self.protocol.isActive()
                                        and not self.protocol.isInteractive()) \
                 else tk.NORMAL
 
+            btnSaveState = tk.DISABLED if (btnState == tk.DISABLED or
+                                           self.protocol.getOutputsSize()) \
+                else tk.NORMAL
+
             self.btnSave = Button(btnFrame, pwutils.Message.LABEL_BUTTON_RETURN,
                                   pwutils.Icon.ACTION_SAVE, command=self.save,
-                                  state=btnState)
+                                  state=btnSaveState)
             self.btnSave.grid(row=0, column=1, padx=5, pady=5, sticky='se')
             self.btnExecute = HotButton(btnFrame, pwutils.Message.LABEL_BUTTON_EXEC,
                                         pwutils.Icon.ACTION_EXECUTE,
                                         command=self.execute, state=btnState)
             self.btnExecute.grid(row=0, column=2, padx=(5, 28),
                                  pady=5, sticky='se')
             self._onPointerChanged()
@@ -2135,15 +2203,15 @@
 
         return frame
 
     def _createHeaderLabel(self, parent, text, bold=False, **gridArgs):
         font = self.font
         if bold:
             font = self.fontBold
-        label = tk.Label(parent, text=text, font=font, bg='white')
+        label = tk.Label(parent, text=text, font=font, bg=pw.Config.SCIPION_BG_COLOR)
         if gridArgs:
             gridDefaults = {'row': 0, 'column': 0, 'padx': 5, 'pady': 5}
             gridDefaults.update(gridArgs)
             label.grid(**gridDefaults)
         return label
 
     def resize(self, frame):
@@ -2177,57 +2245,46 @@
         """ Check if queue is active, if so ask for params if missing"""
         if self.protocol.hasQueueParams() and self.protocol.queueShown:
             return True
         else:
             return self._editQueueParams()
 
     def execute(self, e=None):
-
         if self.protocol.useQueue():
             if not self._getQueueReady():
                 return
         else:  # use queue = No
             hostConfig = self._getHostConfig()
             cores = self.protocol.numberOfMpi.get(1) * self.protocol.numberOfThreads.get(1)
             mandatory = hostConfig.queueSystem.getMandatory()
 
             if mandatory and cores >= mandatory:
                 self.showWarning("You need to submit the job to queue since you \n"
                                  "are requesting a total of *%d* cores (MPI * threads)\n\n"
                                  "*Note*: Your system is configured with MANDATORY = %d.\n"
                                  "        This value can be changed in Scipion/config/hosts.conf" % (cores, mandatory))
                 return
-        if self.protocol.getRunMode() == MODE_RESTART:
-            protocolList = ""
-            if self.protocol.getObjId():
-                project = self.protocol.getProject()
-                errorProList, workflowProtocolList = self.protocol.getProject()._checkWorkflowErrors(self.protocol)
-                for prot in workflowProtocolList:
-                    protocolList += ("\n* " + self.protocol.getProject().getProtocol(prot).getRunName())
-                if len(workflowProtocolList) > 1:
-                    result = askSingleAllCancel(pwutils.Message.TITLE_RESTART_FORM,
-                                                pwutils.Message.LABEL_RESTART_FORM % ('%s\n' % protocolList),
-                                                self.root)
-                    if result == RESULT_RUN_ALL:
-                        self.protocol._store()
-                        self.protocol.getProject()._storeProtocol(self.protocol)
-                        project.launchWorkflow(self.protocol, mode=MODE_RESTART)
-                        self.close()
-                        return
-                    elif result == RESULT_RUN_SINGLE and not self.protocol.isSaved():
-                        project.resetWorkFlow(self.protocol)
-                    elif result == RESULT_CANCEL:
-                        return
-                elif not askYesNo(pwutils.Message.TITLE_RESTART_FORM,
-                                  pwutils.Message.LABEL_RESTART_FORM % (
-                                          '*%s*' % self.protocol.getRunName()),
-                                  self.root):
-                    return
 
-        errors = self.protocol.validate()
+        errors = []
+        resultAction = RESULT_RUN_SINGLE
+        mode = MODE_RESTART if self.protocol.getRunMode() == MODE_RESTART else MODE_RESUME
+
+        # we only take into account the protocols that are already part of the workflow
+        if not self.protocol.isNew():
+            from pyworkflow.gui.project.viewprotocols import ProtocolsView
+            errors, resultAction = ProtocolsView._launchSubWorkflow(self.protocol,
+                                                                    mode, self.root,
+                                                                    askSingleAll=True)
+        if resultAction == RESULT_CANCEL:
+            return
+        elif resultAction == RESULT_RUN_ALL:
+            self._close()
+            return
+
+        errors += self.protocol.validate()
 
         if errors:
             self.showInfo(errors)
         else:
             warns = self.protocol.warnings()
             if warns and not self.askYesNo("There are some warnings",
                                            '\n'.join(warns + ['\nDo you want to continue?'])):
@@ -2235,14 +2292,18 @@
             self._close()
 
     def _close(self, onlySave=False, doSchedule=False):
         try:
             # Set the protocol label
             self.updateProtocolLabel()
 
+            # Clear parameters that are pointers and do not match the condition
+            # to avoid ghost inputs
+            self._checkAllChanges(toggleWidgetVisibility=False)
+
             message = self.callback(self.protocol, onlySave, doSchedule)
             if not self.visualizeMode:
                 if len(message):
                     self.showInfo(message, "Protocol action")
                 if not onlySave:
                     self.close()
         except ModificationNotAllowedException as ex:
@@ -2368,41 +2429,50 @@
                                  value=self.getWidgetValue(protVar, param),
                                  callback=self._checkChanges, visualizeCallback=visualizeCallback,
                                  column=c, showButtons=False)
             widget.show()  # Show always, conditions will be checked later
             c += 2
             self.widgetDict[paramName] = widget
 
-    def _checkCondition(self, paramName):
+    def _checkCondition(self, paramName, toggleWidgetVisibility=True):
         """Check if the condition of a param is satisfied
         hide or show it depending on the result"""
         widget = self.widgetDict.get(paramName, None)
 
         if isinstance(widget, ParamWidget):  # Special vars like MPI, threads or runName are not real widgets
             if isinstance(widget, LineWidget) or isinstance(widget, GroupWidget):
                 param = widget.param
             else:
                 param = self.protocol.getParam(paramName)
-            cond = self.protocol.evalParamCondition(paramName) and self.protocol.evalParamExpertLevel(param)
-            widget.display(cond)
+
+            showLevel = self.protocol.evalParamExpertLevel(param)
+            showCondition = self.protocol.evalParamCondition(paramName)
+            show = showCondition and showLevel
+
+            if toggleWidgetVisibility:
+                widget.display(show)
+            else:
+                # If condition is false and param is a pointer, or Multipointer ...
+                if (not showCondition) and isinstance(param, pwprot.PointerParam):
+                    widget.clear()
 
     def _checkChanges(self, paramName):
         """Check the conditions of all params affected
         by this param"""
         self.setParamFromVar(paramName)
         param = self.protocol.getParam(paramName)
 
         for d in param._dependants:
             self._checkCondition(d)
 
         self.adjustSections()
 
-    def _checkAllChanges(self):
+    def _checkAllChanges(self, toggleWidgetVisibility=True):
         for paramName in self.widgetDict:
-            self._checkCondition(paramName)
+            self._checkCondition(paramName, toggleWidgetVisibility=toggleWidgetVisibility)
 
     def _onExpertLevelChanged(self, *args):
         self._checkAllChanges()
         self.root.update_idletasks()
         self.adjustSections()
 
     def adjustSections(self):
@@ -2522,23 +2592,28 @@
 
     def _onPointerChanged(self, *args):
         btnExecute = getattr(self, 'btnExecute', None)
 
         # This event can be fired even before the button is created
         if btnExecute is None:
             return
+        btnState = tk.DISABLED if (self.protocol.isActive() and not self.protocol.isInteractive()) else tk.NORMAL
+        emptyInput, openSetPointer, emptyPointers = self.protocol.getInputStatus()
+
+        if emptyInput:
+            btnState = tk.DISABLED
 
-        if self.protocol.hasLinkedInputs():
+        if openSetPointer or emptyPointers:
             btnText = 'Schedule'
             cmd = self.schedule
         else:
             btnText = pwutils.Message.LABEL_BUTTON_EXEC
             cmd = self.execute
 
-        btnExecute.config(text=btnText, command=cmd)
+        btnExecute.config(text=btnText, command=cmd, state=btnState)
 
 
 def editObject(self, title, root, obj, mapper):
     """ Show a Text area to edit the protocol label and comment. """
     return EditObjectDialog(root, title, obj, mapper)
 
 
@@ -2560,20 +2635,20 @@
         # preserve values when temporarily changed
         # from one queue to another    
         self.allQueueParams = {self.queueName: queueParams}
 
         Dialog.__init__(self, window.root, "Queue parameters")
 
     def body(self, bodyFrame):
-        bodyFrame.config(bg='white')
-        self.content = tk.Frame(bodyFrame, bg='white')
+        bodyFrame.config(bg=pw.Config.SCIPION_BG_COLOR)
+        self.content = tk.Frame(bodyFrame, bg=pw.Config.SCIPION_BG_COLOR)
         self.content.grid(row=0, column=0, padx=20, pady=20)
 
         label = tk.Label(self.content, text='Submit to queue',
-                         font=self.window.fontBold, bg='white')
+                         font=self.window.fontBold, bg=pw.Config.SCIPION_BG_COLOR)
         label.grid(row=0, column=0, sticky='ne', padx=5, pady=5)
         self.queueVar = tk.StringVar()
         self.queueVar.trace('w', self._onQueueChanged)
         combo = ttk.Combobox(self.content, textvariable=self.queueVar,
                              state='readonly', width=14)
         combo.grid(row=0, column=1, sticky='nw', padx=5, pady=5)
         queueKeys = list(self.queueDict.keys())
@@ -2606,15 +2681,15 @@
                 name, value, label = p
                 helpMsg = None
             elif len(p) == 4:
                 name, value, label, helpMsg = p
             else:
                 raise Exception('Incorrect number of params for %s, expected 3 or 4' % p[0])
 
-            label = tk.Label(self.content, text=label, bg='white')
+            label = tk.Label(self.content, text=label, bg=pw.Config.SCIPION_BG_COLOR)
             label.grid(row=r, column=0, sticky='ne', padx=5, pady=(0, 5))
             var = tk.StringVar()
             # Set the value coming in the protocol 
             var.set(selectedParams.get(name, value))
 
             entry = tk.Entry(self.content, textvariable=var, width=15)
             entry.grid(row=r, column=1, sticky='nw', padx=5, pady=(0, 5))
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/graph.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,16 +126,14 @@
         """ If not createNode is specified, this one will be used
         by default. 
         """
         if canvas is None:
             raise Exception("method setCanvas should be called before using _defaultCreateNode")
         nodeText = node.getLabel()
         textColor = 'black'
-        if nodeText.startswith('Project'):
-            textColor = 'white'
 
         return canvas.createTextbox(nodeText, 100, y, bgColor='light blue', textColor=textColor, margin=0)
 
     def _defaultCreateEdge(self, srcItem, dstItem):
         if self.canvas is None:
             raise Exception("method setCanvas should be called before using _defaultCreateEdge")
         self.canvas.createEdge(srcItem, dstItem)
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/graph_layout.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/graph_layout.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,98 +19,72 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-from pyworkflow import Config
+import logging
+
+from pyworkflow.gui import cfgFontSize
+
+logger = logging.getLogger(__name__)
+
+from pyworkflow import Config, SCIPION_DEFAULT_FONT_SIZE
+
 
 
 class GraphLayout(object):
     """ Base class for all algorithm that implement
     functions to organize a graph in a plane.
     """
-    
-    def draw(self, graph, **kwargs):
-        """ Setup the nodes position in the plane. """
-        pass
-
-
-class BasicLayout(GraphLayout):
-    """ This layout will keep node position as much as possible.
-    It will try to allocate the nodes with x=0 and y=0.
-    """
-    
     def __init__(self):
-        GraphLayout.__init__(self)
+        super().__init__()
         self.DY = 65
         self.DX = 15
-        
-    def draw(self, graph, **kwargs):
-        """ Organize nodes of the graph in the plane.
-        Nodes should have: x, y, width and height attributes
-        x and y will be modified.
+        self._fontScaleFactor = None
+
+    def getY(self):
         """
-        for node in graph.getNodes():
-            if hasattr(node, 'x') and hasattr(node, 'y'):
-                if getattr(node, 'x', 0) == 0 or node.y == 0:
-                    self._drawNode(node)
-                
-    def _drawNode(self, node):
-        """ Allocate node with x=0 and y=0. """
+        :return: Y distance affected by the font size
 
-        try:
-            parents = node.getParents()
-            if not parents:
-                print("EMPTY NODE ask JM")
-                return
-            maxParent = parents[0]
-
-            for p in parents[1:]:
-                if p.y > maxParent.y:
-                    maxParent = p
-
-            siblings = maxParent.getChilds()
-
-            if len(siblings) == 1:
-                node.x = maxParent.x
-                node.y = maxParent.y + self.DY
-            else:
-                rightSibling = siblings[0]
-                for s in siblings:
-                    if s.x > rightSibling.x:
-                        rightSibling = s
-                node.x = rightSibling.x + rightSibling.width/2 + self.DX + node.width/2
-                node.y = rightSibling.y
-        except Exception as e:
-            from pyworkflow.utils import envVarOn
-            if Config.debugOn():
-                print("Can't draw node: %s" % node, e)
-                import traceback
-                traceback.print_stack()
-            else:
-                # Do nothing
-                return
+        """
+
+        return self.DY*self.getFontScaleFactor()
+
+    def getFontScaleFactor(self):
+        """
+        :return: The scale factor between default font size 10, and current one
+
+        """
+        if self._fontScaleFactor is None:
+
+            self._fontScaleFactor = cfgFontSize/SCIPION_DEFAULT_FONT_SIZE
+
+        return self._fontScaleFactor
+
+    def draw(self, graph, **kwargs):
+        """ Setup the nodes position in the plane. """
+        pass
 
 
 class LevelTreeLayout(GraphLayout):
     """ Organize the nodes of the graph by levels.
-    It will recursively organize childs and then
-    fit two sibling trees. """
+    It will recursively organize children and then
+    fit the sibling trees. """
     
-    def __init__(self):
+    def __init__(self, partial=False):
         GraphLayout.__init__(self)
-        self.DY = 65
-        self.DX = 15
         self.maxLevel = 9999
-                        
+        self.partial = partial
+
     def draw(self, graph, **kwargs):
-        """ Organize nodes of the graph in the plane.
-        Nodes should have: x, y, width and height attributes
+        """
+        Organize nodes of the graph in the plane.
+        Nodes should have x, y, width and height attributes.
         x and y will be modified.
         """
         rootNode = graph.getRoot()
         
         # Setup empty layout for each node
         for node in graph.getNodes():
             node._layout = {}
@@ -119,45 +93,53 @@
         self._setLayoutLevel(rootNode,  1, None)
         self._computeNodeOffsets(rootNode, 1)
         # Compute extreme left limit
         m = 9999
         for left, _ in rootNode._layout['hLimits']:
             m = min(m, left)
         
-        self._applyNodeOffsets(rootNode, -m + self.DY)
+        self._applyNodeOffsets(rootNode, -m + self.getY())
         
         # Clean temporary _layout attributes
         for node in graph.getNodes():
             del node._layout
+
+    def _isNewNode(self, node):
+        return node.x == 0 or node.y == 0 or node.isRoot()
         
     def _setLayoutLevel(self, node, level, parent):
         """ Iterate over all nodes and set _layout dict.
         Also set the node level, which is defined
         as the max level of a parent + 1
         """
         if level > self.maxLevel:
             return 
         
         layout = node._layout
         
         if level > layout.get('level', 0):
             # Calculate the y-position depending on the level
             # and the delta-Y (DY)
-            node.y = level * self.DY
+            if not self.partial or self._isNewNode(node):
+                node.y = level * self.getY()
             layout['level'] = level
             layout['parent'] = parent
-            half = node.width / 2
+            if hasattr(node, 'width'):
+                half = node.width / 2
+            else:
+                half = 50
             layout['half'] = half
             layout['hLimits'] = [[-half, half]]
             layout['offset'] = 0
     
             if self.__isNodeExpanded(node):
                 for child in node.getChilds():
+                    logger.debug("%s: Setting layout for child %s" % ("-" * level, child))
                     self._setLayoutLevel(child, level+1, node)
-    
+
     def __isNodeExpanded(self, node):
         """ Check if the status of the node is expanded or collapsed. """
         return getattr(node, 'expanded', True)
         
     def __setNodeOffset(self, node, offset):
         node._layout['offset'] = offset
         
@@ -270,14 +252,16 @@
     def _applyNodeOffsets(self, node, x):
         """ Adjust the x-position of the nodes by applying the offsets.
         """
         if node._layout['level'] == self.maxLevel:
             return 
         
         layout = node._layout
-        node.x = x + layout['offset']
+
+        if not self.partial or self._isNewNode(node):
+            node.x = x + layout['offset']
         
         childs = self.__getNodeChilds(node)
         
         for child in childs:
             self._applyNodeOffsets(child, node.x)
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/gui.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,58 +21,65 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 import os
 import tkinter as tk
 import tkinter.font as tkFont
 import queue
+from functools import partial
+from tkinter.ttk import Style
 
-from pyworkflow.object import OrderedObject
 import pyworkflow as pw
-from pyworkflow.utils import Message, Color, Icon
-
+from pyworkflow.object import Object
+from pyworkflow.utils import Message, Icon
+from PIL import Image, ImageTk
 from .widgets import Button
+import numpy as np
 
 # --------------- GUI CONFIGURATION parameters -----------------------
 # TODO: read font size and name from config file
 FONT_ITALIC = 'fontItalic'
 FONT_NORMAL = 'fontNormal'
 FONT_BOLD = 'fontBold'
 FONT_BIG = 'fontBig'
 cfgFontName = pw.Config.SCIPION_FONT_NAME
 cfgFontSize = pw.Config.SCIPION_FONT_SIZE
 cfgFontBigSize = cfgFontSize + 8
 # TextColor
-cfgCitationTextColor = "dark olive green"
-cfgLabelTextColor = "black"
-cfgSectionTextColor = "blue4"
+# cfgCitationTextColor = "dark olive green"
+# cfgLabelTextColor = "black"
+# cfgSectionTextColor = "blue4"
 # Background Color
-cfgBgColor = "light grey"
-cfgLabelBgColor = "white"
-cfgHighlightBgColor = cfgBgColor
-cfgButtonFgColor = "white"
-cfgButtonActiveFgColor = "white"
-cfgButtonBgColor = Color.RED_COLOR
-cfgButtonActiveBgColor = "#A60C0C"
+# cfgBgColor = "light grey"
+# cfgLabelBgColor = "white"
+# cfgHighlightBgColor = cfgBgColor
+cfgButtonFgColor = pw.Config.SCIPION_BG_COLOR
+cfgButtonActiveFgColor = pw.Config.SCIPION_BG_COLOR
+cfgButtonBgColor = pw.Config.SCIPION_MAIN_COLOR
+cfgButtonActiveBgColor = pw.Config.getActiveColor()
 cfgEntryBgColor = "lemon chiffon"
-cfgExpertLabelBgColor = "light salmon"
-cfgSectionBgColor = cfgButtonBgColor
+# cfgExpertLabelBgColor = "light salmon"
+# cfgSectionBgColor = cfgButtonBgColor
 # Color
-cfgListSelectColor = "DeepSkyBlue4"
-cfgBooleanSelectColor = "white"
-cfgButtonSelectColor = "DeepSkyBlue2"
+# cfgListSelectColor = "DeepSkyBlue4"
+# cfgBooleanSelectColor = "white"
+# cfgButtonSelectColor = "DeepSkyBlue2"
 # Dimensions limits
-cfgMaxHeight = 650
+# cfgMaxHeight = 650
 cfgMaxWidth = 800
-cfgMaxFontSize = 14
-cfgMinFontSize = 6
+# cfgMaxFontSize = 14
+# cfgMinFontSize = 6
 cfgWrapLenght = cfgMaxWidth - 50
 
+# Style of treeviews where row height is variable based on the font size
+LIST_TREEVIEW = 'List.Treeview'
+
+image_cache = dict()
 
-class Config(OrderedObject):
+class Config(Object):
     pass
 
 
 def saveConfig(filename):
     from pyworkflow.mapper import SqliteMapper
     from pyworkflow.object import String, Integer
 
@@ -169,58 +176,85 @@
     changeFontSizeByDeltha(font, deltha, minSize, maxSize)
 
 
 # --------------- IMAGE related variables and functions -----------------------
 def getImage(imageName, imgDict=None, tkImage=True, percent=100,
              maxheight=None):
     """ Search for the image in the RESOURCES path list. """
+
+    global image_cache
+
     if imageName is None:
         return None
-    if imgDict is not None and imageName in imgDict:
-        return imgDict[imageName]
+
+    # Rename .gif by .png. In Linux with pillow 9.2.0 gif transparency is broken so
+    # we need to go for png. But in the past, in Macs png didn't work and made us go from png to gif
+    # We are now providing the 2 formats, prioritising pngs. If png work in MAC and windows then gif
+    # could be deleted. Otherwise, we may need to do this replacement based on the OS.
+    # NOTE: "convert  my-image.gif PNG32:my-image.png" has converted gifs to pngs RGBA (32 bits) it seems pillow
+    # needs RGBA format to deal with transparencies.
+
+    if not os.path.isabs(imageName) and imageName not in [Icon.WAITING]:
+        imageName = imageName.replace(".gif", ".png")
+
+    if imageName in image_cache:
+        return image_cache[imageName]
+
     if not os.path.isabs(imageName):
         imagePath = pw.findResource(imageName)
     else:
         imagePath = imageName
     image = None
     if imagePath:
-        from PIL import Image
         image = Image.open(imagePath)
+        # For a future dark mode we might need to invert the image but it requires some extra work to make it look nice:
+        # image = invertImage(image)
         w, h = image.size
         newSize = None
         if percent != 100:  # Display image with other dimensions
             fp = float(percent) / 100.0
             newSize = int(fp * w), int(fp * h)
         elif maxheight and h > maxheight:
             newSize = int(w * float(maxheight) / h), maxheight
         if newSize:
             image.thumbnail(newSize, Image.ANTIALIAS)
         if tkImage:
-            from PIL import ImageTk
             image = ImageTk.PhotoImage(image)
-        if imgDict is not None:
-            imgDict[imageName] = image
+
+        image_cache[imageName] = image
     return image
 
+def invertImage(img):
+    # Creating a numpy array out of the image object
+    img_arry = np.array(img)
+
+    # Maximum intensity value of the color mode
+    I_max = 255
+
+    # Subtracting 255 (max value possible in a given image
+    # channel) from each pixel values and storing the result
+    img_arry = I_max - img_arry
 
+    # Creating an image object from the resultant numpy array
+    return Image.fromarray(img_arry)
 # ---------------- Windows geometry utilities -----------------------
 def getGeometry(win):
     """ Return the geometry information of the windows
     It will be a tuple (width, height, x, y)
     """
     return (win.winfo_reqwidth(), win.winfo_reqheight(),
             win.winfo_x(), win.winfo_y())
 
 
 def centerWindows(root, dim=None, refWindows=None):
     """Center a windows in the middle of the screen 
     or in the middle of other windows(refWindows param)"""
     root.update_idletasks()
     if dim is None:
-        gw, gh, gx, gy = getGeometry(root)
+        gw, gh, _, _ = getGeometry(root)
     else:
         gw, gh = dim
     if refWindows:
         rw, rh, rx, ry = getGeometry(refWindows)
         x = rx + (rw - gw) / 2
         y = ry + (rh - gh) / 2
     else:
@@ -236,20 +270,37 @@
     """This function is a shortcut to a common
     used pair of calls: rowconfigure and columnconfigure
     for making childs widgets take the space available"""
     widget.columnconfigure(column, weight=1)
     widget.rowconfigure(row, weight=1)
 
 
+def defineStyle():
+    """
+    Defines some specific behaviour of the style.
+    """
+
+    # To specify the height of the rows based on the font size.
+    # Should be centralized somewhere.
+    style = Style()
+    defaultFont = getDefaultFont()
+    rowheight = defaultFont.metrics()['linespace']
+
+    style.configure(LIST_TREEVIEW, rowheight=rowheight,
+                    background=pw.Config.SCIPION_BG_COLOR,
+                    fieldbackground=pw.Config.SCIPION_BG_COLOR)
+    style.configure(LIST_TREEVIEW+".Heading", font=(defaultFont["family"],defaultFont["size"]))
+
+
 class Window:
     """Class to manage a Tk windows.
-    It will encapsulates some basic creation and 
+    It will encapsulate some basic creation and
     setup functions. """
     # To allow plugins to add their own menus
-    _pluginMenus = list()
+    _pluginMenus = dict()
 
     def __init__(self, title='', masterWindow=None, weight=True,
                  minsize=(500, 300), icon=Icon.SCIPION_ICON, **kwargs):
         """Create a Tk window.
         title: string to use as title for the windows.
         master: if not provided, the windows create will be the principal one
         weight: if true, the first col and row will be configured with weight=1
@@ -267,17 +318,18 @@
             # called from the command line, so there's no Scipion main window. In that case, a tk.Tk() exists because if
             # a tk.TopLevel(), as the dialog, is directly launched, it automatically generates a main tk.Tk(). Thus,
             # after that first auto-tk.Tk(), another tk.Tk() was created here, and so the previous information was lost.
             # Solution proposed is to generate the root as an invisible window if it doesn't exist previously, and make
             # he first window generated a tk.Toplevel. After that, all steps executed later will go through the else
             # statement, being that way each new tk.Toplevel() correctly referenced.
             tk.Tk().withdraw()  # Main window, invisible
-            self.root = tk.Toplevel()  # Toplevel of main window
+            self.root = tk.Toplevel(class_="Scipion Framework")  # Toplevel of main window
         else:
-            self.root = tk.Toplevel(masterWindow.root)
+            self.root = tk.Toplevel(masterWindow.root, class_="Scipion Framework")
+            self.root.group(masterWindow.root)
             self._images = masterWindow._images
 
         self.root.withdraw()
         self.root.title(title)
 
         if weight:
             configureWeigths(self.root)
@@ -406,52 +458,55 @@
         return menu
 
     def _addMenuChilds(self, menu, menuConfig):
         """Add entries of menuConfig in menu
         (using add_cascade or add_command for sub-menus and final options)."""
         # Helper function to create the main menu.
         for sub in menuConfig:
-            menuLabel = sub.text.get()
+            menuLabel = sub.text
             if not menuLabel:  # empty or None label means a separator
                 menu.add_separator()
             elif len(sub) > 0:  # sub-menu
                 submenu = tk.Menu(self.root, tearoff=0, font=self.font)
                 menu.add_cascade(label=menuLabel, menu=submenu)
                 self._addMenuChilds(submenu, sub)  # recursive filling
             else:  # menu option
                 # If there is an entry called "Browse files", when clicked it
                 # will call the method onBrowseFiles() (it has to be defined!)
                 def callback(name):
                     """Return a callback function named "on<Name>"."""
                     f = "on%s" % "".join(x.capitalize() for x in name.split())
                     return lambda: getattr(self, f)()
 
-                if sub.shortCut.get() is not None:
-                    menuLabel += ' (' + sub.shortCut.get() + ')'
+                if sub.shortCut is not None:
+                    menuLabel += ' (' + sub.shortCut + ')'
 
                 menu.add_command(label=menuLabel, compound=tk.LEFT,
-                                 image=self.getImage(sub.icon.get()),
-                                 command=callback(name=sub.text.get()))
+                                 image=self.getImage(sub.icon),
+                                 command=callback(name=sub.text))
 
     def _addPluginMenus(self, menu):
 
         if self._pluginMenus:
             submenu = tk.Menu(self.root, tearoff=0, font=self.font)
             menu.add_cascade(label="Others", menu=submenu)
 
             # For each plugin menu
-            for label, callback, icon in self._pluginMenus:
+            for label in self._pluginMenus:
                 submenu.add_command(label=label, compound=tk.LEFT,
-                                    image=self.getImage(icon),
-                                    command=callback)
+                                    image=self.getImage(self._pluginMenus.get(label)[1]),
+                                    command=partial(self.plugin_callback, label))
+
+    def plugin_callback(self, label):
+        return self._pluginMenus.get(label)[0](self)
 
     @classmethod
     def registerPluginMenu(cls, label, callback, icon=None):
         # TODO: have a proper model instead of a tuple?
-        cls._pluginMenus.append((label, callback, icon))
+        cls._pluginMenus[label] = (callback, icon)
 
     def showError(self, msg, header="Error", exception=None):
         """Pops up a dialog with the error message
         :param msg Message to display
         :param header Title of the dialog
         :param exception: Optional. exception associated"""
         from .dialog import showError
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/matplotlib_image.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/matplotlib_image.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/plotter.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/plotter.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/__init__.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/base.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,23 +24,22 @@
 
 
 import os
 import webbrowser
 import tkinter as tk
 
 import pyworkflow as pw
-from pyworkflow.gui import Window, Message, Color, getBigFont
+from pyworkflow.gui import Window, Message, Color, getBigFont, defineStyle
 from pyworkflow.gui.widgets import GradientFrame
 from pyworkflow.utils.properties import Icon
 
 from .viewprojects import ProjectsView
 from .viewprotocols import ProtocolsView
 from .viewdata import ProjectDataView
 
-
 VIEW_PROJECTS = Message.VIEW_PROJECTS
 VIEW_PROTOCOLS = Message.VIEW_PROTOCOLS
 VIEW_DATA = Message.VIEW_DATA
 VIEW_LIST = [VIEW_PROTOCOLS, VIEW_DATA]
 
 
 class ProjectBaseWindow(Window):
@@ -54,21 +53,23 @@
         
         content = tk.Frame(self.root)
         content.columnconfigure(0, weight=1)
         content.rowconfigure(1, weight=1)
         content.grid(row=0, column=0, sticky='news')
         self.content = content
 
+        defineStyle()
+
         if getattr(self, 'menuCfg', None):
             Window.createMainMenu(self, self.menuCfg)
         
         self.header = self.createHeaderFrame(content)
         self.header.grid(row=0, column=0, sticky='new')
         
-        self.footer = tk.Frame(content, bg='white')
+        self.footer = tk.Frame(content, bg=pw.Config.SCIPION_BG_COLOR)
         self.footer.grid(row=1, column=0, sticky='news') 
         
         self.view, self.viewWidget = None, None
         
         self.viewFuncs = {VIEW_PROJECTS: ProjectsView,
                           VIEW_PROTOCOLS: ProtocolsView,
                           VIEW_DATA: ProjectDataView,
@@ -78,53 +79,55 @@
         
         """ Create the Header frame at the top of the windows.
         It has (from left to right):
             - Main application Logo
             - Project Name
             - View selection combobox
         """
-        header = tk.Frame(parent, bg='white')        
+        header = tk.Frame(parent, bg=pw.Config.SCIPION_BG_COLOR)
         header.columnconfigure(1, weight=1)
         header.columnconfigure(2, weight=1)
         # Create the SCIPION logo label
         logoImg = self.getImage(self.generalCfg.logo.get())
         logoLabel = tk.Label(header, image=logoImg, 
-                             borderwidth=0, anchor='nw', bg='white')
+                             borderwidth=0, anchor='nw', bg=pw.Config.SCIPION_BG_COLOR)
         logoLabel.grid(row=0, column=0, sticky='nw', padx=(5, 0), pady=5)
-        versionLabel = tk.Label(header, text=os.environ['SCIPION_VERSION'],
-                                bg='white')
+        version = "%s - %s (core)" % (os.environ.get('SCIPION_VERSION', ""), pw.LAST_VERSION)
+
+        versionLabel = tk.Label(header, text=version,
+                                bg=pw.Config.SCIPION_BG_COLOR)
         versionLabel.grid(row=0, column=1, sticky='sw', pady=20)
         
         # Create the Project Name label
         projName = getattr(self, 'projName', '')
         projLabel = tk.Label(header, text=projName, font=getBigFont(),
-                             borderwidth=0, anchor='nw', bg='white',
-                             fg=Color.DARK_GREY_COLOR)
+                             borderwidth=0, anchor='nw', bg=pw.Config.SCIPION_BG_COLOR,
+                             fg=Color.ALT_COLOR_DARK)
         projLabel.grid(row=0, column=2, sticky='sw', padx=(20, 5), pady=10)
         # Create gradient
         GradientFrame(header, height=8, borderwidth=0).grid(row=1, column=0,
                                                             columnspan=3,
                                                             sticky='new')
         return header
 
     def addViewList(self, header):
         """Create the view selection frame (Protocols|Data) in the header.
         """
         # This function is called from createHeaderFrame() in ProjectWindow
-        viewFrame = tk.Frame(header, bg='white')
+        viewFrame = tk.Frame(header, bg=pw.Config.SCIPION_BG_COLOR)
         viewFrame.grid(row=0, column=2, sticky='se', padx=5, pady=10)
 
         def addLink(elementText):
             btn = tk.Label(viewFrame, text=elementText, cursor='hand2',
-                           fg="#6F3232", bg="white")
+                           fg=pw.Config.SCIPION_MAIN_COLOR, bg=pw.Config.SCIPION_BG_COLOR)
             btn.bind('<Button-1>', lambda e: self._viewComboSelected(elementText))
             return btn
         
         def addTube():        
-            return tk.Label(viewFrame, text="|", fg="#6F3232", bg="white", padx=5)
+            return tk.Label(viewFrame, text="|", fg=pw.Config.SCIPION_MAIN_COLOR, bg=pw.Config.SCIPION_BG_COLOR, padx=5)
 
         for i, elementText in enumerate(VIEW_LIST):
             btn = addLink(elementText)
             btn.grid(row=0, column=i*2)
             
             if i < len(VIEW_LIST)-1:
                 tube = addTube()
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/labels.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/labels.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 # *
 # **************************************************************************
 """
 Tree widget implementation.
 """
         
 import tkinter as tk
-
+from pyworkflow import Config
 from pyworkflow.project import Label
 from pyworkflow.gui import Icon, configureWeigths
 from pyworkflow.gui.tree import TreeProvider
 import pyworkflow.gui.dialog as dialog
 
 
 class LabelsTreeProvider(TreeProvider):
@@ -144,44 +144,44 @@
 class EditLabelDialog(dialog.Dialog):
     """ Dialog to edit a label (name, color) """
     def __init__(self, parent, title, label, **kwargs):
         self.label = label
         dialog.Dialog.__init__(self, parent, title)
 
     def body(self, bodyFrame):
-        bodyFrame.config(bg='white')
+        bodyFrame.config(bg=Config.SCIPION_BG_COLOR)
         configureWeigths(bodyFrame, 1, 1)
 
         # Label
-        label_text = tk.Label(bodyFrame, text="Name", bg='white', bd=0)
+        label_text = tk.Label(bodyFrame, text="Name", bg=Config.SCIPION_BG_COLOR, bd=0)
         label_text.grid(row=0, column=0, sticky='nw', padx=(15, 10), pady=15)
         # Label box
         var = tk.StringVar()
         var.set(self.label.getName())
         self.textVar = var
         self.textLabel = tk.Entry(bodyFrame, width=20, textvariable=var)
         self.textLabel.grid(row=0, column=1, sticky='news', padx=5, pady=5)
 
         # Comment
         colorLabel = tk.Label(bodyFrame, text='Color \n(Click to change)',
-                              bg='white', bd=0)
+                              bg=Config.SCIPION_BG_COLOR, bd=0)
         colorLabel.grid(row=1, column=0, sticky='nw', padx=(15, 10), pady=15)
         self.colorVar = tk.StringVar()
         self.colorVar.set(self.label.getColor())
         self.colorBox = tk.Frame(bodyFrame, bg=self.colorVar.get())
         self.colorBox.grid(row=1, column=1, sticky='news', padx=5, pady=5)
         colorLabel.bind('<Button-1>', self._changeColor)
         self.colorBox.bind('<Button-1>', self._changeColor)
 
     def apply(self):
         self.label.setName(self.textVar.get())
         self.label.setColor(self.colorVar.get())
 
     def _changeColor(self, e=None):
-        hexColor = dialog.askColor(self.colorVar.get())
+        hexColor = dialog.askColor(parent=self, defaultColor=self.colorVar.get())
         if hexColor is not None:
             self.colorBox.config(bg=hexColor)
             self.colorVar.set(hexColor)
 
     def validate(self):
 
         validationMsg = None
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/project.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/project.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,16 @@
 Main Project window implementation.
 It is composed by three panels:
 1. Left: protocol tree.
 2. Right upper: VIEWS (Data/Protocols)
 3. Summary/Details
 """
 
-
+import logging
+logger = logging.getLogger(__name__)
 import os
 import threading
 import shlex
 import subprocess
 import socketserver
 import tempfile
 
@@ -75,47 +76,51 @@
         self.project = self.loadProject()
 
         # TODO: put the menu part more nicely. From here:
         menu = MenuConfig()
 
         projMenu = menu.addSubMenu('Project')
         projMenu.addSubMenu('Browse files', 'browse',
-                            icon='fa-folder-open.gif')
+                            icon=Icon.FOLDER_OPEN)
         projMenu.addSubMenu('Remove temporary files', 'delete',
-                            icon='fa-trash-o.gif')
+                            icon=Icon.ACTION_DELETE)
         projMenu.addSubMenu('Manage project labels', 'labels',
                             icon=Icon.TAGS)
         projMenu.addSubMenu('Toggle color mode', 'color_mode',
                             shortCut="Ctrl+t", icon=Icon.ACTION_VISUALIZE)
         projMenu.addSubMenu('Select all protocols', 'select all',
-                            shortCut="Ctrl+a")
-        projMenu.addSubMenu('Find protocol to add', 'find protocol',
-                            shortCut="Ctrl+f")
+                            shortCut="Ctrl+a", icon=Icon.SELECT_ALL)
+        projMenu.addSubMenu('Add a protocol', 'find protocol',
+                            shortCut="Ctrl+f", icon=Icon.FIND)
+        projMenu.addSubMenu('Locate a protocol', 'locate protocol',
+                            shortCut="Ctrl+l")
         projMenu.addSubMenu('', '')  # add separator
         projMenu.addSubMenu('Import workflow', 'load_workflow',
-                            icon='fa-download.gif')
+                            icon=Icon.DOWNLOAD)
         projMenu.addSubMenu('Search workflow', 'search_workflow',
-                            icon='fa-search.gif')
+                            icon=Icon.ACTION_SEARCH)
         if pw.Config.debugOn():
             projMenu.addSubMenu('Export tree graph', 'export_tree')
         projMenu.addSubMenu('', '')  # add separator
         projMenu.addSubMenu('Debug Mode', 'debug mode',
-                            shortCut="Ctrl+d", icon='debug.gif')
+                            shortCut="Ctrl+D", icon=Icon.DEBUG)
         projMenu.addSubMenu('', '')  # add separator
-        projMenu.addSubMenu('Notes', 'notes', icon='fa-pencil.gif')
+        projMenu.addSubMenu('Notes', 'notes', icon=Icon.ACTION_EDIT)
+        projMenu.addSubMenu('Scipion log', 'scipion log',
+                            icon=Icon.FILE_BW)
         projMenu.addSubMenu('', '')  # add separator
-        projMenu.addSubMenu('Exit', 'exit', icon='fa-sign-out.gif')
+        projMenu.addSubMenu('Exit', 'exit', icon=Icon.ACTION_OUT)
 
         helpMenu = menu.addSubMenu('Help')
         helpMenu.addSubMenu('Online help', 'online_help',
-                            icon='fa-external-link.gif')
+                            icon=Icon.ACTION_EXPORT)
         helpMenu.addSubMenu('About', 'about',
-                            icon='fa-question-circle.gif')
+                            icon=Icon.ACTION_HELP)
         helpMenu.addSubMenu('Contact support', 'contact_us',
-                            icon='fa-question-circle.gif')
+                            icon=Icon.ACTION_HELP)
 
         self.menuCfg = menu
 
         if self.project.openedAsReadOnly():
             self.projName += "<READ ONLY>"
 
         # Notify about the workflow in this project
@@ -146,27 +151,27 @@
         self.settings.write()
         
     def _onClosing(self):
         try:
             if not self.project.openedAsReadOnly():
                 self.saveSettings()
         except Exception as ex:
-            print("%s %s" % (Message.NO_SAVE_SETTINGS, str(ex)))
+            logger.info("%s %s" % (Message.NO_SAVE_SETTINGS, str(ex)))
         ProjectBaseWindow._onClosing(self)
      
     def loadProject(self):
         proj = pw.project.Project(pw.Config.getDomain(), self.projPath)
         proj.load()
 
         # Check if we have settings.sqlite, generate if not
         settingsPath = os.path.join(proj.path, proj.settingsPath)
         if os.path.exists(settingsPath):
             self.settings = proj.getSettings()
         else:
-            print('Warning: settings.sqlite not found! '
+            logger.info('Warning: settings.sqlite not found! '
                   'Creating default settings..')
             self.settings = proj.createSettings()
 
         self.generalCfg = self.settings.getConfig()
 
         return proj
 
@@ -225,55 +230,63 @@
                 # TODO: think what to do with directories. Delete? Report?
             self.showInfo("Deleted content of %s -- %d file(s)." % (tmpPath, n))
         except Exception as e:
             self.showError(str(e))
         
     def _loadWorkflow(self, obj):
         try:
+            self.getViewWidget().info('Importing workflow %s' % obj.getPath())
             self.project.loadProtocols(obj.getPath())
-            self.getViewWidget().updateRunsGraph(True, reorganize=True)
+            self.getViewWidget().updateRunsGraph(True)
+            self.getViewWidget().cleanInfo()
         except Exception as ex:
-            self.showError(str(ex))
+            self.showError(str(ex), exception=ex)
             
     def onImportWorkflow(self):
         FileBrowserWindow("Select workflow .json file",
                           self, self.project.getPath(''),
                           onSelect=self._loadWorkflow,
                           selectButton='Import'
                           ).show()
 
     def onSearchWorkflow(self):
         WorkflowRepository().search()
 
     def onExportTreeGraph(self):
-        runsGraph = self.project.getRunsGraph(refresh=True)
+        runsGraph = self.project.getRunsGraph()
         useId = not pwutils.envVarOn('SCIPION_TREE_NAME')
         dotStr = runsGraph.printDot(useId=useId)
         with tempfile.NamedTemporaryFile(suffix='.gv', mode="w") as dotFile:
             dotFile.write(dotStr)
             dotFile.flush()
             openTextFileEditor(dotFile.name)
 
         if useId:
-            print("\nexport SCIPION_TREE_NAME=1 # to use names instead of ids")
+            logger.info("\nexport SCIPION_TREE_NAME=1 # to use names instead of ids")
         else:
-            print("\nexport SCIPION_TREE_NAME=0 # to use ids instead of names")
+            logger.info("\nexport SCIPION_TREE_NAME=0 # to use ids instead of names")
 
     def onManageProjectLabels(self):
         self.manageLabels()
 
     def onToggleColorMode(self):
         self.getViewWidget()._toggleColorScheme(None)
 
     def onSelectAllProtocols(self):
         self.getViewWidget()._selectAllProtocols(None)
 
-    def onFindProtocolToAdd(self):
+    def onAddAProtocol(self):
         self.getViewWidget()._findProtocol(None)
 
+    def onLocateAProtocol(self):
+        self.getViewWidget()._locateProtocol(None)
+
+    def onScipionLog(self):
+        self.getViewWidget()._scipionLog(None)
+
     def manageLabels(self):
         return LabelsDialog(self.root,
                             self.project.settings.getLabels(),
                             allowSelect=True)
 
     def initProjectTCPServer(self):
         server = ProjectTCPServer((self.project.address, self.project.port),
@@ -309,24 +322,23 @@
             else:
                 inputId = int(inputStrId)
                 inputObj = project.mapper.selectById(inputId)
 
             func = self._OBJECT_COMMANDS.get(cmd, None)
 
             if func is None:
-                print("Error, command '%s' not found. " % cmd)
+                logger.info("Error, command '%s' not found. " % cmd)
             else:
                 def myfunc():
                     func(inputObj, objId)
                     inputObj.close()
                 self.enqueue(myfunc)
 
         except Exception as ex:
-            print("There was an error executing object command !!!:")
-            print(ex)
+            logger.error("There was an error executing object command !!!:", exc_info=ex)
     
     def recalculateCTF(self, inputObjId, sqliteFile):
         """ Load the project and launch the protocol to
         create the subset.
         """
         # Retrieve project, input protocol and object from db
         project = self.project
@@ -347,38 +359,39 @@
         # Launch the protocol
         self.getViewWidget().executeProtocol(prot)
 
 
 class ProjectManagerWindow(ProjectBaseWindow):
     """ Windows to manage all projects. """
     # To allow plugins to add their own menus
-    _pluginMenus = list()
+    _pluginMenus = dict()
 
     def __init__(self, **kwargs):
         # Load global configuration
         settings = ProjectSettings()
 
         # TODO: put the menu part more nicely. From here:
         menu = MenuConfig()
 
         fileMenu = menu.addSubMenu('File')
-        fileMenu.addSubMenu('Browse files', 'browse', icon='fa-folder-open.gif')
-        fileMenu.addSubMenu('Exit', 'exit', icon='fa-sign-out.gif')
+        fileMenu.addSubMenu('Browse files', 'browse', icon=Icon.FOLDER_OPEN)
+        fileMenu.addSubMenu('Exit', 'exit', icon=Icon.ACTION_OUT)
 
         confMenu = menu.addSubMenu('Configuration')
         if os.path.exists(pw.Config.SCIPION_CONFIG):
             confMenu.addSubMenu('General', 'general')
         confMenu.addSubMenu('Hosts', 'hosts')
-        confMenu.addSubMenu('Protocols', 'protocols')
+        if os.path.exists(pw.Config.SCIPION_PROTOCOLS):
+            confMenu.addSubMenu('Protocols', 'protocols')
         if os.path.exists(pw.Config.SCIPION_LOCAL_CONFIG):
             confMenu.addSubMenu('User', 'user')
 
         helpMenu = menu.addSubMenu('Help')
-        helpMenu.addSubMenu('Online help', 'online_help', icon='fa-external-link.gif')
-        helpMenu.addSubMenu('About', 'about', icon='fa-question-circle.gif')
+        helpMenu.addSubMenu('Online help', 'online_help', icon=Icon.ACTION_EXPORT)
+        helpMenu.addSubMenu('About', 'about', icon=Icon.ACTION_HELP)
 
         self.menuCfg = menu
         self.generalCfg = settings.getConfig()
 
         try:
             title = '%s (%s on %s)' % (Message.LABEL_PROJECTS, 
                                        pwutils.getLocalUserName(),
@@ -421,20 +434,14 @@
     def onProtocols():
         ProjectManagerWindow._openConfigFile(pw.Config.SCIPION_PROTOCOLS)
 
     @staticmethod
     def onUser():
         ProjectManagerWindow._openConfigFile(pw.Config.SCIPION_LOCAL_CONFIG)
 
-    # Moved to scipion-app
-    # def onPlugins(self):
-    #     # Config -> Plugins
-    #     PluginManager("Plugin Manager", self, pw.Config.SCIPION_USER_DATA,
-    #                   selectButton=None).show()
-
 
 class ProjectTCPServer(socketserver.ThreadingMixIn, socketserver.TCPServer):
     pass
 
 
 class ProjectTCPRequestHandler(socketserver.BaseRequestHandler):
 
@@ -442,14 +449,16 @@
         try:
             project = self.server.project
             window = self.server.window
             msg = self.request.recv(1024)
             msg = msg.decode()
             tokens = shlex.split(msg)
             if msg.startswith('run protocol'):
+                
+                logger.debug("run protocol messaged arrived: %s" % msg)
                 protocolName = tokens[2]
                 protocolClass = pw.Config.getDomain().getProtocols()[protocolName]
                 # Create the new protocol instance and set the input values
                 protocol = project.newProtocol(protocolClass)
 
                 for token in tokens[3:]:
                     param, value = token.split('=')
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/viewdata.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/viewdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 """
 
 
 import tkinter as tk
 import tkinter.ttk as ttk
 import tkinter.font as tkFont
 
+from pyworkflow import Config
 import pyworkflow.utils as pwutils
 import pyworkflow.protocol as pwprot
 import pyworkflow.viewer as pwviewer
 
 import pyworkflow.gui as gui
 from pyworkflow.gui.tree import Tree
 from pyworkflow.gui.dialog import EditObjectDialog
@@ -46,31 +47,26 @@
 
 ACTION_EDIT = pwutils.Message.LABEL_EDIT
 ACTION_COPY = pwutils.Message.LABEL_COPY
 ACTION_DELETE = pwutils.Message.LABEL_DELETE
 ACTION_REFRESH = pwutils.Message.LABEL_REFRESH
 ACTION_STEPS = pwutils.Message.LABEL_BROWSE
 ACTION_TREE = pwutils.Message.LABEL_TREE
-ACTION_LIST = pwutils.Message.LABEL_LIST
 ACTION_STOP = pwutils.Message.LABEL_STOP
 ACTION_DEFAULT = pwutils.Message.LABEL_DEFAULT
 ACTION_CONTINUE = pwutils.Message.LABEL_CONTINUE
 ACTION_RESULTS = pwutils.Message.LABEL_ANALYZE
 
-RUNS_TREE = pwutils.Icon.RUNS_TREE
-RUNS_LIST = pwutils.Icon.RUNS_LIST
- 
 ActionIcons = {
     ACTION_EDIT: pwutils.Icon.ACTION_EDIT,
     ACTION_COPY: pwutils.Icon.ACTION_COPY,
     ACTION_DELETE:  pwutils.Icon.ACTION_DELETE,
     ACTION_REFRESH:  pwutils.Icon.ACTION_REFRESH,
     ACTION_STEPS:  pwutils.Icon.ACTION_STEPS,
     ACTION_TREE:  None,  # should be set
-    ACTION_LIST:  pwutils.Icon.ACTION_LIST,
     ACTION_STOP: pwutils.Icon.ACTION_STOP,
     ACTION_CONTINUE: pwutils.Icon.ACTION_CONTINUE,
     ACTION_RESULTS: pwutils.Icon.ACTION_RESULTS,
 }
 
 STATUS_COLORS = {
     pwprot.STATUS_SAVED: '#D9F1FA',
@@ -123,24 +119,24 @@
         
     def _createContent(self):
         """ Create the Data View for the Project.
         It has two panes:
             Left: containing the Protocol classes tree
             Right: containing the Data list
         """
-        p = tk.PanedWindow(self, orient=tk.HORIZONTAL, bg='white')
+        p = tk.PanedWindow(self, orient=tk.HORIZONTAL, bg=Config.SCIPION_BG_COLOR)
         
         # Left pane, contains Data tree
-        leftFrame = tk.Frame(p, bg='white')
+        leftFrame = tk.Frame(p, bg=Config.SCIPION_BG_COLOR)
         bgColor = '#eaebec'
         self._createDataTree(leftFrame, bgColor)
         gui.configureWeigths(leftFrame)
         
         # Right pane
-        rightFrame = tk.Frame(p, bg='white')
+        rightFrame = tk.Frame(p, bg=Config.SCIPION_BG_COLOR)
         rightFrame.columnconfigure(0, weight=1)
         rightFrame.rowconfigure(1, weight=1)
         # rightFrame.rowconfigure(0, minsize=label.winfo_reqheight())
         self._fillRightPane(rightFrame)
 
         # Add sub-windows to PanedWindows
         p.add(leftFrame, padx=5, pady=5)
@@ -152,23 +148,23 @@
     
     def _createDataTree(self, parent, bgColor):
         """Create a tree on the left panel to store how 
         many object are from each type and the hierarchy.
         """
         defaultFont = gui.getDefaultFont()
         self.style.configure("W.Treeview",
-                             background=pwutils.Color.LIGHT_GREY_COLOR,
+                             background=pwutils.Color.ALT_COLOR,
                              borderwidth=0,
                              rowheight=defaultFont.metrics()['linespace'])
         self.dataTree = Tree(parent, show='tree', style='W.Treeview')
         self.dataTree.column('#0', minwidth=300)
         self.dataTree.tag_configure('protocol',
-                                    image=self.getImage('python_file.gif'))
+                                    image=self.getImage(pwutils.Icon.PRODUCTION))
         self.dataTree.tag_configure('protocol_base',
-                                    image=self.getImage('class_obj.gif'))
+                                    image=self.getImage(pwutils.Icon.GROUP))
         f = tkFont.Font(family='helvetica', size='10', weight='bold')
         self.dataTree.tag_configure('non-empty', font=f)
         self.dataTree.grid(row=0, column=0, sticky='news')
 
         # bind click events
         self.dataTree.tag_bind(DATA_TAG, '<Double-1>', self._dataItemClick)
         self.dataTree.tag_bind(DATA_TAG, '<Return>', self._dataItemClick)
@@ -216,39 +212,39 @@
         # Create the right Pane that will be composed by:
         # a Action Buttons TOOLBAR in the top
         # and another vertical Pane with:
         # Runs History (at Top)
         # Selected run info (at Bottom)
         """
         # Create the Action Buttons TOOLBAR
-        toolbar = tk.Frame(parent, bg='white')
+        toolbar = tk.Frame(parent, bg=Config.SCIPION_BG_COLOR)
         toolbar.grid(row=0, column=0, sticky='news')
         gui.configureWeigths(toolbar)
         # toolbar.columnconfigure(0, weight=1)
         toolbar.columnconfigure(1, weight=1)
         
-        self.runsToolbar = tk.Frame(toolbar, bg='white')
+        self.runsToolbar = tk.Frame(toolbar, bg=Config.SCIPION_BG_COLOR)
         self.runsToolbar.grid(row=0, column=0, sticky='sw')
         # On the left of the toolbar will be other
         # actions that can be applied to all runs (refresh, graph view...)
-        self.allToolbar = tk.Frame(toolbar, bg='white')
+        self.allToolbar = tk.Frame(toolbar, bg=Config.SCIPION_BG_COLOR)
         self.allToolbar.grid(row=0, column=10, sticky='se')
         # self.createActionToolbar()
 
         # Create the Run History tree
         v = ttk.PanedWindow(parent, orient=tk.VERTICAL)
         # runsFrame = ttk.Labelframe(v, text=' History ', width=500, height=500)
-        runsFrame = tk.Frame(v, bg='white')
+        runsFrame = tk.Frame(v, bg=Config.SCIPION_BG_COLOR)
         self._createDataGraph(runsFrame)
         gui.configureWeigths(runsFrame)
         
         # Create the Selected Run Info
         infoFrame = tk.Frame(v)
         gui.configureWeigths(infoFrame)
-        self._infoText = TaggedText(infoFrame, bg='white',
+        self._infoText = TaggedText(infoFrame, bg=Config.SCIPION_BG_COLOR,
                                     handlers={'sci-open': self._openProtocolFormFromId})
         self._infoText.grid(row=0, column=0, sticky='news')
         
         v.add(runsFrame, weight=3)
         v.add(infoFrame, weight=1)
         v.grid(row=1, column=0, sticky='news')
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/viewprojects.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/viewprojects.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,15 +17,19 @@
 # * You should have received a copy of the GNU General Public License
 # * along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+import datetime
+import logging
 
+REFRESH_WAIT_SEC = 60
+logger = logging.getLogger(__name__)
 
 import os
 import tkinter as tk
 import tkinter.font as tkFont
 
 import pyworkflow as pw
 from pyworkflow.project import Project
@@ -33,30 +37,32 @@
 from pyworkflow.utils.path import getHomePath
 
 from pyworkflow.project import Manager
 import pyworkflow.gui as pwgui
 from pyworkflow.gui.text import TaggedText
 from pyworkflow.gui.dialog import askString, askYesNo, showError
 
-from pyworkflow.gui import Message, Window, cfgEntryBgColor
+from pyworkflow.gui import Message, Window, cfgEntryBgColor, ToolTip
 from pyworkflow.gui.browser import FileBrowserWindow
 from pyworkflow.gui.widgets import IconButton, HotButton, Button
 from pyworkflow.utils.properties import Icon
 
 
 class ProjectsView(tk.Frame):
     _PROJ_CONTAINER = "projectsframe"
 
     def __init__(self, parent, windows, **args):
-        tk.Frame.__init__(self, parent, bg='white', **args)
+        tk.Frame.__init__(self, parent, bg=pw.Config.SCIPION_BG_COLOR, **args)
         self.windows = windows
         self.manager = windows.manager
         self.root = windows.root
+        self.lastLoad = None
 
-        # tkFont.Font(size=12, family='verdana', weight='bold')
+        # Bind to root "focus in"
+        self.root.bind("<FocusIn>", self._onWindowFocusIn)
         bigSize = pwgui.cfgFontSize + 2
         smallSize = pwgui.cfgFontSize - 2
         fontName = pwgui.cfgFontName
 
         self.projNameFont = tkFont.Font(size=bigSize, family=fontName,
                                         weight='bold')
         self.projDateFont = tkFont.Font(size=smallSize, family=fontName)
@@ -66,27 +72,35 @@
 
         self.filter = tk.StringVar()
         self.filterBox = None
         self.addActionsFrame()
 
         self.columnconfigure(0, weight=1)
         self.rowconfigure(1, weight=1)
-        text = TaggedText(self, width=40, height=15, bd=0, bg='white')
+        text = TaggedText(self, width=40, height=15, bd=0, bg=pw.Config.SCIPION_BG_COLOR)
         text.grid(row=1, columnspan=2, column=0, sticky='news')
-
-        self.createProjectList(text)
         text.setReadOnly(True)
         self.text = text
         self.filterBox.focus_set()
 
+        # Content load happens automatically _onWindowFocusIn
+
+    def _onWindowFocusIn(self, event):
+        """ Refresh on windows get focus """
+        if event.widget == self.root:
+            # Get the delta from the last time refreshed
+            delta = REFRESH_WAIT_SEC if self.lastLoad is None else (datetime.datetime.now() - self.lastLoad).seconds
+            if delta >= REFRESH_WAIT_SEC:
+                self.createProjectList()
+
     def addActionsFrame(self):
         """ Add the "toolbar" for actions like create project, import
          project or filter"""
         # Add the create project button
-        bg = "white"
+        bg = pw.Config.SCIPION_BG_COLOR
         btnFrame = tk.Frame(self, bg=bg)
         btn = HotButton(btnFrame, text=Message.LABEL_CREATE_PROJECT,
                         font=self.projNameFont,
                         command=self._onCreateProject)
         btn.grid(row=0, column=0, sticky='nw', padx=10, pady=10)
         # Add the Import project button
         btn = Button(btnFrame, text=Message.LABEL_IMPORT_PROJECT,
@@ -99,39 +113,46 @@
         # Add the Import project button
         btn = tk.Label(btnFrame, bg=bg, text="Filter:", font=self.projNameFont)
         btn.grid(row=0, column=2, sticky='nse', padx=10, pady=10)
         self.filterBox = tk.Entry(btnFrame, font=self.projNameFont, textvariable=self.filter)
         self.filterBox.grid(row=0, column=3, sticky='ne', padx=10, pady=12)
         self.filterBox.bind('<Return>', self._onFilter)
         self.filterBox.bind('<KP_Enter>', self._onFilter)
+        self.filterBox.bind("<F5>", self.createProjectList)
+        ToolTip(self.filterBox, "Return/enter to filter. F5 to refresh the list")
+
 
-    def createProjectList(self, text):
+    def createProjectList(self, event=None):
         """Load the list of projects"""
+
+        self.lastLoad = datetime.datetime.now()
         r = 0
+        text = self.text
         text.setReadOnly(False)
         text.clear()
-        parent = tk.Frame(text, bg='white', name=self._PROJ_CONTAINER)
+        parent = tk.Frame(text, bg=pw.Config.SCIPION_BG_COLOR, name=self._PROJ_CONTAINER)
         parent.columnconfigure(0, weight=1)
-        colors = ['white', '#EAEBFF']
+        colors = [pw.Config.SCIPION_BG_COLOR, '#EAEBFF']
         for i, p in enumerate(self.manager.listProjects()):
             try:
                 # Add creation time to project info
                 # Add if it's a link
                 p.index = "index%s" % i
 
                 # Consider the filter
                 if not self._doesProjectMatchFilter(p):
                     continue
 
                 frame = self.createProjectLabel(parent, p, color=colors[i % 2])
                 frame.grid(row=r, column=0, padx=10, pady=5, sticky='new')
                 r += 1
+
             except Exception as ex:
-                print("ERROR loading project: %s" % p.getName())
-                print(ex)
+                logger.error("Couldn't load project %s" % p.getName(), exc_info=True)
+
         text.window_create(tk.INSERT, window=parent)
         text.bindWidget(parent)
         text.setReadOnly(True)
 
     def createProjectLabel(self, parent, projInfo, color):
         frame = tk.Frame(parent, bg=color, name=projInfo.index)
         # ROW1
@@ -162,27 +183,27 @@
             lblLink = tk.Label(frame, text=linkMsg, font=self.projDateFont, bg=color, fg='grey', justify=tk.LEFT)
             lblLink.grid(row=2, column=0, columnspan=3, sticky='w')
 
         return frame
 
     def createNewProject(self, projName, projLocation):
         proj = self.manager.createProject(projName, location=projLocation)
-        self.createProjectList(self.text)
+        self.createProjectList()
         self.openProject(proj.getShortName())
 
     def _onCreateProject(self, e=None):
         projWindow = ProjectCreateWindow("Create project", self)
         projWindow.show()
 
     def _onImportProject(self, e=None):
         importProjWindow = ProjectImportWindow("Import project", self)
         importProjWindow.show()
 
     def _onFilter(self, e=None):
-        self.createProjectList(self.text)
+        self.createProjectList()
 
     def _setFocusToList(self, e=None):
         self.text.focus_set()
 
     def _doesProjectMatchFilter(self, project):
         """ Returns true if the project matches the filter"""
         # Lets' use the name anc creation date for now:
@@ -191,28 +212,30 @@
                                  prettyTime(project.cTime, time=False)])
 
         return self.filter.get().lower() in searchString
 
     def importProject(self, projLocation, copyFiles, projName, searchLocation):
 
         self.manager.importProject(projLocation, copyFiles, projName, searchLocation)
-        self.createProjectList(self.text)
+        self.createProjectList()
         self.openProject(projName)
 
     def openProject(self, projName):
         from subprocess import Popen
         script = pw.join(pw.APPS, 'pw_project.py')
         Popen([pw.PYTHON, script, projName])
 
     def deleteProject(self, projInfo):
 
         projName = projInfo.projName
 
         if askYesNo(Message.TITLE_DELETE_PROJECT,
                     "Project *%s*. " % projName + Message.MESSAGE_DELETE_PROJECT, self.root):
+
+            logger.info("User agreed to delete project %s" % projName)
             self.manager.deleteProject(projName)
 
             #Delete the frame
             self.text.children[self._PROJ_CONTAINER].children[projInfo.index].grid_forget()
 
 
     def renameProject(self, projName):
@@ -220,69 +243,69 @@
         if not newName or newName == projName:
             return
         if self.manager.hasProject(newName):
             showError("Rename cancelled",
                       "Project name already exists: %s" % newName, self.root)
             return
         self.manager.renameProject(projName, newName)
-        self.createProjectList(self.text)
+        self.createProjectList()
 
 
 class ProjectCreateWindow(Window):
     """ Windows to create a project. """
 
     def __init__(self, title, parent=None, weight=True, minsize=(400, 110),
                  icon=Icon.SCIPION_ICON, **args):
         """
          We assume the parent should be of ProjectsView
         """
         Window.__init__(self, title, parent.windows, weight=weight,
                         icon=icon, minsize=minsize, enableQueue=True)
-        self.root['background'] = 'white'
+        self.root['background'] = pw.Config.SCIPION_BG_COLOR
 
         self.parent = parent
         self.projectsPath = self.parent.manager.PROJECTS
         self.projName = tk.StringVar()
         self.projName.set('')
         self.projLocation = tk.StringVar()
         self.projLocation.set(self.projectsPath)
 
         content = tk.Frame(self.root)
         content.columnconfigure(0, weight=1)
         content.columnconfigure(1, weight=3)
-        content.config(bg='white')
+        content.config(bg=pw.Config.SCIPION_BG_COLOR)
         content.grid(row=0, column=0, sticky='news', padx=5, pady=5)
 
         # Info line
-        labelInfo = tk.Label(content, text="Spaces will be replaced by underscores!", bg='white', bd=0)
+        labelInfo = tk.Label(content, text="Spaces will be replaced by underscores!", bg=pw.Config.SCIPION_BG_COLOR, bd=0)
         labelInfo.grid(row=0, sticky=tk.W, padx=5, pady=5)
         #  Project name line
-        labelName = tk.Label(content, text=Message.LABEL_PROJECT + ' name', bg='white', bd=0)
+        labelName = tk.Label(content, text=Message.LABEL_PROJECT + ' name', bg=pw.Config.SCIPION_BG_COLOR, bd=0)
         labelName.grid(row=1, sticky=tk.W, padx=5, pady=5)
         entryName = tk.Entry(content, bg=cfgEntryBgColor, width=20, textvariable=self.projName)
         entryName.grid(row=1, column=1, columnspan=2, sticky=tk.EW, padx=5, pady=5)
         entryName.bind("<Return>", self._create)
         entryName.bind("<KP_Enter>", self._create)
         # Project location line
-        labelLocation = tk.Label(content, text=Message.LABEL_PROJECT + ' location', bg='white', bd=0)
+        labelLocation = tk.Label(content, text=Message.LABEL_PROJECT + ' location', bg=pw.Config.SCIPION_BG_COLOR, bd=0)
         labelLocation.grid(row=2, column=0, sticky='nw', padx=5, pady=5)
 
         self.entryBrowse = tk.Entry(content, bg=cfgEntryBgColor, width=40, textvariable=self.projLocation)
         self.entryBrowse.grid(row=2, column=1, sticky='nw', padx=5, pady=5)
         self.btnBrowse = IconButton(content, 'Browse', Icon.ACTION_BROWSE,
                                     highlightthickness=0, command=self._browsePath)
         self.btnBrowse.grid(row=2, column=2, sticky='e', padx=5, pady=5)
 
         self.initial_focus = entryName
         self.initial_focus.focus()
 
         btnFrame = tk.Frame(content)
         btnFrame.columnconfigure(0, weight=1)
         btnFrame.grid(row=3, column=0, sticky='sew', padx=5, pady=(0, 5), columnspan=2)
-        btnFrame.config(bg='white')
+        btnFrame.config(bg=pw.Config.SCIPION_BG_COLOR)
 
         # Create buttons
         btnCreate = HotButton(btnFrame, 'Create', Icon.BUTTON_SELECT, command=self._create)
         btnCreate.grid(row=0, column=0, sticky='e', padx=5, pady=5)
         btnCancel = Button(btnFrame, 'Cancel', Icon.BUTTON_CANCEL, command=self.close)
         btnCancel.grid(row=0, column=1, sticky='e', padx=5, pady=5)
 
@@ -332,15 +355,15 @@
     def __init__(self, title, parent=None, weight=True, minsize=(400, 150),
                  icon=Icon.SCIPION_ICON, **args):
         """
          We assume the parent should be ProjectsView
         """
         Window.__init__(self, title, parent.windows, weight=weight,
                         icon=icon, minsize=minsize, enableQueue=True)
-        self.root['background'] = 'white'
+        self.root['background'] = pw.Config.SCIPION_BG_COLOR
         self.parent = parent
         # Dirty hack, need to add a slash for the explorer to pick up the right default path.
         self.projectsPath = getHomePath() + "/"
         self.projLocation = tk.StringVar()
         self.projLocation.set(self.projectsPath)
 
         self.projName = tk.StringVar()
@@ -348,51 +371,51 @@
 
         self.searchLocation = tk.StringVar()
         self.searchLocation.set('')
 
         content = tk.Frame(self.root)
         content.columnconfigure(0, weight=1)
         content.columnconfigure(1, weight=1)
-        content.config(bg='white')
+        content.config(bg=pw.Config.SCIPION_BG_COLOR)
         content.grid(row=0, column=0, sticky='news',
                      padx=5, pady=5)
 
         # Path explorer
-        labelProjectLocation = tk.Label(content, text="Project location", bg='white', bd=0)
+        labelProjectLocation = tk.Label(content, text="Project location", bg=pw.Config.SCIPION_BG_COLOR, bd=0)
         labelProjectLocation.grid(row=0, column=0, sticky='nw', padx=5, pady=5)
         # it seems tk.Entry does not uses default font...grrrr!!
         self.entryBrowse = tk.Entry(content, bg=cfgEntryBgColor, width=40,
                                     textvariable=self.projLocation, font=self.font)
         self.entryBrowse.grid(row=0, column=1, sticky='nw', padx=5, pady=5)
         self.btnBrowse = IconButton(content, 'Browse', Icon.ACTION_BROWSE, highlightthickness=0,
                                     command=self._browseProjectLocation)
         self.btnBrowse.grid(row=0, column=2, sticky='e', padx=5, pady=5)
 
         # Copy files check
-        labelCheck = tk.Label(content, text="Copy project", bg='white', borderwidth=0)
+        labelCheck = tk.Label(content, text="Copy project", bg=pw.Config.SCIPION_BG_COLOR, borderwidth=0)
         labelCheck.grid(row=1, column=0, sticky='nw', padx=5, pady=5)
 
         self.tkCheckVar = tk.IntVar()
-        btnCheck = tk.Checkbutton(content, variable=self.tkCheckVar, highlightthickness=0, activebackground='white',
-                                  bg='white', bd=0)
+        btnCheck = tk.Checkbutton(content, variable=self.tkCheckVar, highlightthickness=0, activebackground=pw.Config.SCIPION_BG_COLOR,
+                                  bg=pw.Config.SCIPION_BG_COLOR, bd=0)
         btnCheck.grid(row=1, column=1, sticky='nw', padx=0, pady=5)
 
         btnCopyHelp = IconButton(content, Message.LABEL_BUTTON_HELP, Icon.ACTION_HELP, highlightthickness=0,
                                  command=lambda: self.showInfo(
                                      'If checked, \"Project location\" will be copied. Otherwise a soft link to it will be created.'))
         btnCopyHelp.grid(row=1, column=3, sticky='e', padx=2, pady=2)
 
         # Project name
-        labelName = tk.Label(content, text='Project name (Optional)', bg='white', bd=0)
+        labelName = tk.Label(content, text='Project name (Optional)', bg=pw.Config.SCIPION_BG_COLOR, bd=0)
         labelName.grid(row=2, column=0, sticky='nw', padx=5, pady=5)
         entryName = tk.Entry(content, bg='white', width=20, textvariable=self.projName, font=self.font)
         entryName.grid(row=2, column=1, sticky='nw', padx=5, pady=5)
 
         # Path to search for raw data and restore broken links.
-        labelSearchLocation = tk.Label(content, text="Raw files location (Optional)", bg='white', bd=0)
+        labelSearchLocation = tk.Label(content, text="Raw files location (Optional)", bg=pw.Config.SCIPION_BG_COLOR, bd=0)
         labelSearchLocation.grid(row=3, column=0, sticky='nw', padx=5, pady=5)
 
         self.entrySearchLocation = tk.Entry(content, bg='white', width=40,
                                             textvariable=self.searchLocation, font=self.font)
         self.entrySearchLocation.grid(row=3, column=1, sticky='nw', padx=5, pady=5)
         self.btnSearch = IconButton(content, 'Browse', Icon.ACTION_BROWSE,
                                     highlightthickness=0, command=self._browseSearchLocation)
@@ -405,15 +428,15 @@
         self.initial_focus = entryName
         self.initial_focus.focus()
         btnCheck.select()
 
         btnFrame = tk.Frame(content)
         btnFrame.columnconfigure(0, weight=1)
         btnFrame.grid(row=4, column=0, sticky='sew', padx=5, pady=(0, 5), columnspan=2)
-        btnFrame.config(bg='white')
+        btnFrame.config(bg=pw.Config.SCIPION_BG_COLOR)
 
         # Create buttons
         btnSelect = HotButton(btnFrame, 'Import', Icon.BUTTON_SELECT, command=self._select)
         btnSelect.grid(row=0, column=0, sticky='e', padx=5, pady=5)
         btnCancel = Button(btnFrame, 'Cancel', Icon.BUTTON_CANCEL, command=self.close)
         btnCancel.grid(row=0, column=1, sticky='e', padx=5, pady=5)
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/project/viewprotocols.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/project/viewprotocols.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python
+# -*- coding: utf-8 -*-
 # **************************************************************************
 # *
 # * Authors:     J.M. De la Rosa Trevin (delarosatrevin@scilifelab.se) [1]
 # *
 # * [1] SciLifeLab, Stockholm University
 # *
 # * This program is free software: you can redistribute it and/or modify
@@ -18,585 +18,134 @@
 # * You should have received a copy of the GNU General Public License
 # * along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-from configparser import ConfigParser
+import logging
+import threading
 
-from pyworkflow.project import MenuConfig
 from pyworkflow import Config
+from pyworkflow.gui import TextFileViewer, getDefaultFont, LIST_TREEVIEW, \
+    ShortCut, ToolTip, RESULT_RUN_ALL, RESULT_RUN_SINGLE, RESULT_CANCEL
+from pyworkflow.gui.project.constants import *
+from pyworkflow.protocol import SIZE_1MB, SIZE_1GB, SIZE_1TB
 
-INIT_REFRESH_SECONDS = 3
+INIT_REFRESH_SECONDS = Config.SCIPION_GUI_REFRESH_INITIAL_WAIT
 
 """
 View with the protocols inside the main project window.
 """
 
 import os
 import json
 import re
 import tempfile
 from collections import OrderedDict
 import tkinter as tk
 import tkinter.ttk as ttk
 import datetime as dt
 
-import pyworkflow.object as pwobj
+from pyworkflow import Config, TK
 import pyworkflow.utils as pwutils
 import pyworkflow.protocol as pwprot
-import pyworkflow.gui as pwgui
-from pyworkflow.gui.dialog import askColor, FloatingMessage
 from pyworkflow.viewer import DESKTOP_TKINTER, ProtocolViewer
-from pyworkflow.utils.properties import Message, Icon, Color, KEYSYM
-from pyworkflow.gui.project.utils import getStatusColorFromNode
-from pyworkflow.gui.form import FormWindow
+from pyworkflow.utils.properties import Color, KEYSYM, Icon, Message
 from pyworkflow.webservices import WorkflowRepository
 
+import pyworkflow.gui as pwgui
+from pyworkflow.gui.form import FormWindow
+from pyworkflow.gui.project.utils import getStatusColorFromNode, inspectObj
+from pyworkflow.gui.project.searchprotocol import SearchProtocolWindow, ProtocolTreeProvider
+from pyworkflow.gui.project.steps import StepsWindow
+from pyworkflow.gui.project.viewprotocols_extra import RunIOTreeProvider, ProtocolTreeConfig
+from pyworkflow.gui.project.searchrun import RunsTreeProvider, SearchRunWindow
+
+logger = logging.getLogger(__name__)
+
 DEFAULT_BOX_COLOR = '#f8f8f8'
 
-ACTION_EDIT = Message.LABEL_EDIT
-ACTION_RENAME = Message.LABEL_RENAME
-ACTION_SELECT_TO = Message.LABEL_SELECT_TO
-ACTION_COPY = Message.LABEL_COPY
-ACTION_DELETE = Message.LABEL_DELETE
-ACTION_REFRESH = Message.LABEL_REFRESH
-ACTION_STEPS = Message.LABEL_STEPS
-ACTION_BROWSE = Message.LABEL_BROWSE
-ACTION_DB = Message.LABEL_DB
-ACTION_TREE = Message.LABEL_TREE
-ACTION_LIST = Message.LABEL_LIST
-ACTION_STOP = Message.LABEL_STOP
-ACTION_DEFAULT = Message.LABEL_DEFAULT
-ACTION_CONTINUE = Message.LABEL_CONTINUE
-ACTION_RESULTS = Message.LABEL_ANALYZE
-ACTION_EXPORT = Message.LABEL_EXPORT
-ACTION_EXPORT_UPLOAD = Message.LABEL_EXPORT_UPLOAD
-ACTION_SWITCH_VIEW = 'Switch_View'
-ACTION_COLLAPSE = 'Collapse'
-ACTION_EXPAND = 'Expand'
-ACTION_LABELS = 'Labels'
-ACTION_RESTART_WORKFLOW = Message.LABEL_RESTART_WORKFLOW
-ACTION_CONTINUE_WORKFLOW = Message.LABEL_CONTINUE_WORKFLOW
-ACTION_STOP_WORKFLOW = Message.LABEL_STOP_WORKFLOW
-ACTION_RESET_WORKFLOW = Message.LABEL_RESET_WORKFLOW
 
 RUNS_TREE = Icon.RUNS_TREE
-RUNS_LIST = Icon.RUNS_LIST
 
 VIEW_LIST = 0
 VIEW_TREE = 1
 VIEW_TREE_SMALL = 2
 
-ActionIcons = {
-    ACTION_EDIT: Icon.ACTION_EDIT,
-    ACTION_SELECT_TO: Icon.ACTION_SELECT_TO,
-    ACTION_COPY: Icon.ACTION_COPY,
-    ACTION_DELETE: Icon.ACTION_DELETE,
-    ACTION_REFRESH: Icon.ACTION_REFRESH,
-    ACTION_RENAME: Icon.ACTION_RENAME,
-    ACTION_STEPS: Icon.ACTION_STEPS,
-    ACTION_BROWSE: Icon.ACTION_BROWSE,
-    ACTION_DB: Icon.ACTION_DB,
-    ACTION_TREE: None,  # should be set
-    ACTION_LIST: Icon.ACTION_LIST,
-    ACTION_STOP: Icon.ACTION_STOP,
-    ACTION_CONTINUE: Icon.ACTION_CONTINUE,
-    ACTION_RESULTS: Icon.ACTION_RESULTS,
-    ACTION_EXPORT: Icon.ACTION_EXPORT,
-    ACTION_EXPORT_UPLOAD: Icon.ACTION_EXPORT_UPLOAD,
-    ACTION_COLLAPSE: 'fa-minus-square.gif',
-    ACTION_EXPAND: 'fa-plus-square.gif',
-    ACTION_LABELS: Icon.TAGS,
-    ACTION_RESTART_WORKFLOW: Icon.ACTION_EXECUTE,
-    ACTION_CONTINUE_WORKFLOW: Icon.ACTION_CONTINUE,
-    ACTION_STOP_WORKFLOW: Icon.ACTION_STOP_WORKFLOW,
-    ACTION_RESET_WORKFLOW: Icon.ACTION_REFRESH
-}
-
-
-class RunsTreeProvider(pwgui.tree.ProjectRunsTreeProvider):
-    """Provide runs info to populate tree"""
-
-    def __init__(self, project, actionFunc):
-        pwgui.tree.ProjectRunsTreeProvider.__init__(self, project)
-        self.actionFunc = actionFunc
-        self._selection = project.getSettings().runSelection
-
-    def getActionsFromSelection(self):
-        """ Return the list of options available for selection. """
-        n = len(self._selection)
-        single = n == 1
-        if n:
-            prot = self.project.getProtocol(self._selection[0])
-            status = prot.getStatus()
-            nodeInfo = self.project.getSettings().getNodeById(prot.getObjId())
-            expanded = nodeInfo.isExpanded() if nodeInfo else True
-        else:
-            status = None
-
-        stoppable = status in [pwprot.STATUS_RUNNING, pwprot.STATUS_SCHEDULED, 
-                               pwprot.STATUS_LAUNCHED]
-
-        return [(ACTION_EDIT, single),
-                (ACTION_RENAME, single),
-                (ACTION_COPY, True),
-                (ACTION_DELETE, status != pwprot.STATUS_RUNNING),
-                (ACTION_STEPS, single and Config.debugOn()),
-                (ACTION_BROWSE, single),
-                (ACTION_DB, single and Config.debugOn()),
-                (ACTION_STOP, stoppable and single),
-                (ACTION_EXPORT, not single),
-                (ACTION_EXPORT_UPLOAD, not single),
-                (ACTION_COLLAPSE, single and status and expanded),
-                (ACTION_EXPAND, single and status and not expanded),
-                (ACTION_LABELS, True),
-                (ACTION_SELECT_TO, True),
-                (ACTION_RESTART_WORKFLOW, single),
-                (ACTION_CONTINUE_WORKFLOW, single),
-                (ACTION_STOP_WORKFLOW, single),
-                (ACTION_RESET_WORKFLOW, single)
-                ]
-
-    def getObjectActions(self, obj):
-
-        def addAction(actionLabel):
-            if actionLabel:
-                text = actionLabel
-                action = actionLabel
-                actionLabel = (text, lambda: self.actionFunc(action),
-                               ActionIcons.get(action, None))
-            return actionLabel
-
-        actions = [addAction(a)
-                   for a, cond in self.getActionsFromSelection() if cond]
-
-        if hasattr(obj, 'getActions'):
-            for text, action in obj.getActions():
-                actions.append((text, action, None))
-
-        return actions
-
-
-class ProtocolTreeProvider(pwgui.tree.ObjectTreeProvider):
-    """Create the tree elements for a Protocol run"""
-
-    def __init__(self, protocol):
-        self.protocol = protocol
-        # This list is create to group the protocol parameters
-        # in the tree display
-        self.status = pwobj.List(objName='_status')
-        self.params = pwobj.List(objName='_params')
-        self.statusList = ['status', 'initTime', 'endTime', 'error',
-                           'interactive', 'mode']
-
-        objList = [] if protocol is None else [protocol]
-        pwgui.tree.ObjectTreeProvider.__init__(self, objList)
-
-
-class StepsTreeProvider(pwgui.tree.TreeProvider):
-    """Create the tree elements for a Protocol run"""
-
-    def __init__(self, stepsList):
-        for i, s in enumerate(stepsList):
-            if not s._index:
-                s._index = i + 1
-
-        self._stepsList = stepsList
-        self.getColumns = lambda: [('Index', 50), ('Step', 200),
-                                   ('Time', 150), ('Class', 100)]
-        self._parentDict = {}
-
-    def getObjects(self):
-        return self._stepsList
-
-    @staticmethod
-    def getObjectInfo(obj):
-        info = {'key': obj._index,
-                'values': (str(obj), pwutils.prettyDelta(obj.getElapsedTime()),
-                           obj.getClassName())}
-        return info
-
-    @staticmethod
-    def getObjectPreview(obj):
-
-        args = json.loads(obj.argsStr.get())
-        msg = "*Prerequisites*: %s \n" % str(obj._prerequisites)
-        msg += "*Arguments*: " + '\n  '.join([str(a) for a in args])
-        if hasattr(obj, 'resultFiles'):
-            results = json.loads(obj.resultFiles.get())
-            if len(results):
-                msg += "\n*Result files:* " + '\n  '.join(results)
-
-        return None, msg
-
-
-class StepsWindow(pwgui.browser.BrowserWindow):
-    def __init__(self, title, parentWindow, protocol, **args):
-        self._protocol = protocol
-        provider = StepsTreeProvider(protocol.loadSteps())
-        pwgui.browser.BrowserWindow.__init__(self, title, parentWindow,
-                                             weight=False, **args)
-        # Create buttons toolbar
-        self.root.columnconfigure(0, weight=1)
-        self.root.rowconfigure(1, weight=1)
-
-        toolbar = tk.Frame(self.root)
-        toolbar.grid(row=0, column=0, sticky='nw', padx=5, pady=5)
-        btn = tk.Label(toolbar, text="Tree",
-                       image=self.getImage(Icon.RUNS_TREE),
-                       compound=tk.LEFT, cursor='hand2')
-        btn.bind('<Button-1>', self._showTree)
-        btn.grid(row=0, column=0, sticky='nw')
-        # Create and set browser
-        browser = pwgui.browser.ObjectBrowser(self.root, provider,
-                                              showPreviewTop=False)
-        self.setBrowser(browser, row=1, column=0)
-
-    # noinspection PyUnusedLocal
-    def _showTree(self, e=None):
-        g = self._protocol.getStepsGraph()
-        w = pwgui.Window("Protocol steps", self, minsize=(800, 600))
-        root = w.root
-        canvas = pwgui.Canvas(root, width=600, height=500,
-                              tooltipCallback=self._stepTooltip,)
-        canvas.grid(row=0, column=0, sticky='nsew')
-        canvas.drawGraph(g, pwgui.LevelTreeLayout())
-        w.show()
-
-    def _stepTooltip(self, tw, item):
-        """ Create the contents of the tooltip to be displayed
-        for the given step.
-        Params:
-            tw: a tk.TopLevel instance (ToolTipWindow)
-            item: the selected step.
-        """
-
-        if not hasattr(item.node, 'step'):
-            return
-
-        step = item.node.step
-
-        tm = str(step.funcName)
 
-        if not hasattr(tw, 'tooltipText'):
-            frame = tk.Frame(tw)
-            frame.grid(row=0, column=0)
-            tw.tooltipText = pwgui.dialog.createMessageBody(
-                frame, tm, None, textPad=0, textBg=Color.LIGHT_GREY_COLOR_2)
-            tw.tooltipText.config(bd=1, relief=tk.RAISED)
-        else:
-            pwgui.dialog.fillMessageText(tw.tooltipText, tm)
-
-
-class SearchProtocolWindow(pwgui.Window):
+class ScipionLogWindow(pwgui.Window):
+    """Class that create a windows where the system log is display """
     def __init__(self, parentWindow, **kwargs):
-        pwgui.Window.__init__(self, title="Search for a protocol",
-                              masterWindow=parentWindow)
-        content = tk.Frame(self.root, bg='white')
-        self._createContent(content)
+        pwgui.Window.__init__(self, title="Scipion log",
+                              masterWindow=parentWindow,
+                              minsize=(1000, 400))
+        content = tk.Frame(self.root)
         content.grid(row=0, column=0, sticky='news')
-        content.columnconfigure(0, weight=1)
-        content.rowconfigure(1, weight=1)
-
-    def _createContent(self, content):
-        self._createSearchBox(content)
-        self._createResultsBox(content)
-
-    def _createSearchBox(self, content):
-        """ Create the Frame with Search widgets """
-        frame = tk.Frame(content, bg='white')
-
-        label = tk.Label(frame, text="Search", bg='white')
-        label.grid(row=0, column=0, sticky='nw')
-        self._searchVar = tk.StringVar()
-        entry = tk.Entry(frame, bg='white', textvariable=self._searchVar)
-        entry.bind('<Return>', self._onSearchClick)
-        entry.bind('<KP_Enter>', self._onSearchClick)
-        entry.focus_set()
-        entry.grid(row=0, column=1, sticky='nw')
-        btn = pwgui.widgets.IconButton(frame, "Search",
-                                       imagePath=Icon.ACTION_SEARCH,
-                                       command=self._onSearchClick)
-        btn.grid(row=0, column=2, sticky='nw')
-
-        frame.grid(row=0, column=0, sticky='new', padx=5, pady=(10, 5))
-
-    def _createResultsBox(self, content):
-        frame = tk.Frame(content, bg=Color.LIGHT_GREY_COLOR, padx=5, pady=5)
-        pwgui.configureWeigths(frame)
-        self._resultsTree = self.master.getViewWidget()._createProtocolsTree(
-            frame, show=None, columns=("protocol", "streaming", "installed", "help", "score"))
-        self._configureTreeColumns()
-        self._resultsTree.grid(row=0, column=0, sticky='news')
-        frame.grid(row=1, column=0, sticky='news', padx=5, pady=5)
-
-    def _configureTreeColumns(self):
-        self._resultsTree.column('#0', width=0, stretch=tk.FALSE)
-        self._resultsTree.column('protocol', width=300, stretch=tk.FALSE)
-        self._resultsTree.column('streaming', width=100, stretch=tk.FALSE)
-        self._resultsTree.column('installed', width=110, stretch=tk.FALSE)
-        self._resultsTree.column('help', minwidth=300, stretch=tk.YES)
-        self._resultsTree.column('score', width=50, stretch=tk.FALSE)
-        self._resultsTree.heading('protocol', text='Protocol', command=lambda: self._resultsTree.sortByColumn("protocol", False))
-        self._resultsTree.heading('streaming', text='Streamified', command=lambda: self._resultsTree.sortByColumn("streaming", False))
-        self._resultsTree.heading('installed', text='Installation', command=lambda: self._resultsTree.sortByColumn("installed", False))
-        self._resultsTree.heading('help', text='Help', command=lambda: self._resultsTree.sortByColumn("help", False))
-        self._resultsTree.heading('score', text='Score', command=lambda: self._resultsTree.sortByColumn("score", False, casting=int))
-
-    def _onSearchClick(self, e=None):
-        self._resultsTree.clear()
-        keyword = self._searchVar.get().lower().strip()
-        emProtocolsDict = Config.getDomain().getProtocols()
-        protList = []
-
-        def addSearchWeight(line2Search, searchtext):
-            # Adds a weight value for the search
-            weight = 0
-
-            # prioritize findings in label
-            if searchtext in line2Search[1]:
-                weight += 10
-
-            for value in line2Search[2:]:
-                weight += 5 if searchtext in value else 0
-
-            if " " in searchtext:
-                for word in searchtext.split():
-                    if word in line2Search[1]:
-                        weight += 3
-
-                    for value in line2Search[2:]:
-                        weight += 1 if word in value else 0
-
-            return line2Search + (weight,)
-
-        for key, prot in emProtocolsDict.items():
-            if ProtocolTreeConfig.isAFinalProtocol(prot, key):
-                label = prot.getClassLabel().lower()
-                line = (key, label,
-                        "installed" if prot.isInstalled() else "missing installation",
-                        prot.getHelpText().strip().replace('\r', '').replace('\n', '').lower(),
-                        "streamified" if prot.worksInStreaming() else "static")
-
-                line = addSearchWeight(line, keyword)
-                # something was found: weight > 0
-                if line[5] != 0:
-                    protList.append(line)
-
-        # Sort by weight
-        protList.sort(reverse=True, key=lambda x: x[5])
-
-        for key, label, installed, help, streamified, weight in protList:
-            tag = ProtocolTreeConfig.getProtocolTag(installed == 'installed')
-            self._resultsTree.insert(
-                '', 'end', key, text="", tags=tag,
-                values=(label, streamified, installed, help, weight))
-
-
-class RunIOTreeProvider(pwgui.tree.TreeProvider):
-    """Create the tree elements from a Protocol Run input/output childs"""
-
-    def __init__(self, parent, protocol, mapper):
-        # TreeProvider.__init__(self)
-        self.parent = parent
-        self.protocol = protocol
-        self.mapper = mapper
-
-    @staticmethod
-    def getColumns():
-        return [('Attribute', 200), ('Info', 100)]
-
-    def getObjects(self):
-        objs = []
-        if self.protocol:
-            # Store a dict with input parents (input, PointerList)
-            self.inputParentDict = OrderedDict()
-            inputs = []
-            inputObj = pwobj.String(Message.LABEL_INPUT)
-            inputObj._icon = Icon.ACTION_IN
-            self.inputParentDict['_input'] = inputObj
-            inputParents = [inputObj]
-
-            for key, attr in self.protocol.iterInputAttributes():
-                attr._parentKey = key
-                # Repeated keys means there are inside a pointerList
-                # since the same key is yielded for all items inside
-                # so update the parent dict with a new object
-                if key in self.inputParentDict:
-                    if self.inputParentDict[key] == inputObj:
-                        parentObj = pwobj.String(key)
-                        parentObj._icon = Icon.ACTION_IN
-                        parentObj._parentKey = '_input'
-                        inputParents.append(parentObj)
-                        self.inputParentDict[key] = parentObj
-                else:
-                    self.inputParentDict[key] = inputObj
-                inputs.append(attr)
-
-            outputs = [attr for _, attr in
-                       self.protocol.iterOutputAttributes()]
-            self.outputStr = pwobj.String(Message.LABEL_OUTPUT)
-            objs = inputParents + inputs + [self.outputStr] + outputs
-        return objs
-
-    def _visualizeObject(self, ViewerClass, obj):
-        viewer = ViewerClass(project=self.protocol.getProject(),
-                             protocol=self.protocol,
-                             parent=self.parent.windows)
-        viewer.visualize(obj)
-
-    def _editObject(self, obj):
-        """Open the Edit GUI Form given an instance"""
-        pwgui.dialog.EditObjectDialog(self.parent, Message.TITLE_EDIT_OBJECT,
-                                      obj, self.mapper)
-
-    def _deleteObject(self, obj):
-        """ Remove unnecessary output, specially for Coordinates. """
-        prot = self.protocol
-        try:
-            objLabel = self.getObjectLabel(obj, prot)
-            if self.parent.windows.askYesNo("Delete object",
-                                            "Are you sure to delete *%s* object?"
-                                            % objLabel):
-                prot.getProject().deleteProtocolOutput(prot, obj)
-                self.parent._fillSummary()
-                self.parent.windows.showInfo("Object *%s* successfully deleted."
-                                             % objLabel)
-        except Exception as ex:
-            self.parent.windows.showError(str(ex))
-
-    @staticmethod
-    def getObjectPreview(obj):
-        desc = "<name>: " + obj.getName()
-        return None, desc
-
-    def getObjectActions(self, obj):
-        if isinstance(obj, pwobj.Pointer):
-            obj = obj.get()
-            isPointer = True
-        else:
-            isPointer = False
-        actions = []
-
-        viewers = Config.getDomain().findViewers(obj.getClassName(), DESKTOP_TKINTER)
-
-        def viewerCallback(viewer):
-            return lambda: self._visualizeObject(viewer, obj)
-
-        for v in viewers:
-            actions.append(('Open with %s' % v.__name__,
-                            viewerCallback(v),
-                            Icon.ACTION_VISUALIZE))
-        # EDIT
-        actions.append((Message.LABEL_EDIT,
-                        lambda: self._editObject(obj),
-                        Icon.ACTION_EDIT))
-        # DELETE
-        # Special case to allow delete outputCoordinates
-        # since we can end up with several outputs and
-        # we may want to clean up
-        if self.protocol.allowsDelete(obj) and not isPointer:
-            actions.append((Message.LABEL_DELETE_ACTION,
-                            lambda: self._deleteObject(obj),
-                            Icon.ACTION_DELETE))
-        return actions
-
-    @staticmethod
-    def getObjectLabel(obj, parent):
-        """ We will try to show in the list the string representation
-        that is more readable for the user to pick the desired object.
-        """
-        label = 'None'
-        if obj:
-            label = obj.getObjLabel()
-            if not len(label.strip()):
-                parentLabel = parent.getObjLabel() if parent else 'None'
-                label = "%s -> %s" % (parentLabel, obj.getLastName())
-        return label
-
-    def getObjectInfo(self, obj):
-        if obj is None or not obj.hasValue():
-            return None
-
-        if isinstance(obj, pwobj.String):
-            value = obj.get()
-            info = {'key': value, 'text': value, 'values': '', 'open': True}
-            if hasattr(obj, '_parentKey'):
-                info['parent'] = self.inputParentDict[obj._parentKey]
-        else:
-            # All attributes are considered output, unless they are pointers
-            image = Icon.ACTION_OUT
-            parent = self.outputStr
-
-            if isinstance(obj, pwobj.Pointer):
-                name = obj.getLastName()
-                # Remove ugly item notations inside lists
-                name = name.replace('__item__000', '')
-                # Consider Pointer as inputs
-                image = getattr(obj, '_icon', '')
-                parent = self.inputParentDict[obj._parentKey]
-
-                suffix = ''
-                if obj.hasExtended():
-                    # getExtended method remove old attributes conventions.
-                    extendedValue = obj.getExtended()
-                    if obj.hasExtended():
-                        suffix = '[%s]' % extendedValue
-                    # else:
-                    #     suffix = '[Item %s]' % extendedValue
-
-                    # Tolerate loading projects:
-                    # When having only the project sqlite..an obj.get() will
-                    # the load of the set...and if it is missing this whole
-                    # "thread" fails.
-                    try:
-                        if obj.get() is None:
-                            labelObj = obj.getObjValue()
-                            suffix = ''
-                        else:
-                            labelObj = obj.get()
-                    except Exception as e:
-                        return {'parent': parent, 'image': image, 'text': name,
-                                'values': ("Couldn't read object attributes.",)}
-                else:
-                    labelObj = obj.get()
-
-                objKey = obj._parentKey + str(labelObj.getObjId())
-                label = self.getObjectLabel(labelObj,
-                                            self.mapper.getParent(labelObj))
-                name += '   (from %s %s)' % (label, suffix)
-            else:
-                name = self.getObjectLabel(obj, self.protocol)
-                objKey = str(obj.getObjId())
-                labelObj = obj
-
-            # To tolerate str(labelObj) in case xmippLib is missing, but
-            # still being able to open a project.
+        pwgui.configureWeigths(content)
+        self.showScipionLog = threading.Thread(name="scipion_log",
+                                              target=self._showScipionLog,
+                                              args=(content,))
+        self.showScipionLog.start()
+
+    def _showScipionLog(self, content):
+        """
+        Create a content of the system log window
+        """
+
+        # Fill the Output Log
+        terminal = tk.Frame(content)
+        terminal.grid(row=0, column=0, sticky='news')
+        pwgui.configureWeigths(terminal)
+
+        self.textLog = TextFileViewer(terminal, font=getDefaultFont(),
+                                      height=30, width=100)
+        self.textLog.grid(row=0, column=0, sticky='news')
+
+        fileLogPath = Config.SCIPION_LOG
+        self.fileLog = open(fileLogPath, 'r')
+        # Create a tab where the log will appear
+        self.textLog.createWidgets([fileLogPath])
+        self.textLog.refreshAll(goEnd=True)
+        # Refreshing the log every 3 seconds
+        self.threadRefresh = threading.Thread(name="refresh_log",
+                                              target=self._refreshLogComponent,
+                                              args=(3,))
+        self.threadRefresh.start()
+
+    def _refreshLogComponent(self, wait=3):
+        """ Refresh the Plugin Manager log """
+        import time
+        while True:
+            time.sleep(wait)
+            # Taking the vertical scroll position. If this action fail, assume
+            # that the log window was closed and finalized the refresh thread
             try:
-                value = str(labelObj)
-            except Exception as e:
-                print("Can not convert object %s - %s to string." % (objKey, name))
-                value = str(e)
-
-            info = {'key': objKey, 'parent': parent, 'image': image,
-                    'text': name, 'values': (value,)}
-        return info
-
+                vsPos = self.textLog.taList[0].getVScroll()
+                if vsPos[1] == 1.0:
+                    self.textLog.refreshAll(goEnd=True)
+                else:
+                    self.textLog.refreshAll(goEnd=False)
+            except Exception:
+                break
 
 # noinspection PyAttributeOutsideInit
 class ProtocolsView(tk.Frame):
     """ What you see when the "Protocols" tab is selected.
 
     In the main project window there are three tabs: "Protocols | Data | Hosts".
     This extended tk.Frame is what will appear when Protocols is on.
     """
 
     RUNS_CANVAS_NAME = "runs_canvas"
+
+    SIZE_COLORS = {SIZE_1MB: "green",
+                    SIZE_1GB: "orange",
+                    SIZE_1TB: "red"}
+
     _protocolViews = None
 
     def __init__(self, parent, windows, **args):
         tk.Frame.__init__(self, parent, **args)
         # Load global configuration
         self.windows = windows
         self.project = windows.project
@@ -610,56 +159,43 @@
         self._items = {}
         self._lastSelectedProtId = None
         self._lastStatus = None
         self.selectingArea = False
         self._lastRightClickPos = None  # Keep last right-clicked position
 
         self.style = ttk.Style()
-        self.root.bind("<F5>", self.refreshRuns)
         self.root.bind("<Control-f>", self._findProtocol)
         self.root.bind("<Control-a>", self._selectAllProtocols)
         self.root.bind("<Control-t>", self._toggleColorScheme)
-        self.root.bind("<Control-d>", self._toggleDebug)
+        self.root.bind("<Control-D>", self._toggleDebug)
+        self.root.bind("<Control-l>", self._locateProtocol)
+
         if Config.debugOn():
             self.root.bind("<Control-i>", self._inspectProtocols)
 
-        # To bind key press to methods
-        # Listen to any key: send event to keyPressed method
-        self.root.bind("<Key>", self.keyPressed)
-        self.keybinds = dict()
-
-        # Register key binds
-        self._bindKeyPress(KEYSYM.DELETE, self._onDelPressed)
 
         self.__autoRefresh = None
         self.__autoRefreshCounter = INIT_REFRESH_SECONDS  # start by 3 secs
 
+        self.refreshSemaphore = True
+        self.repeatRefresh = False
+
         c = self.createContent()
         pwgui.configureWeigths(self)
         c.grid(row=0, column=0, sticky='news')
 
-    def _bindKeyPress(self, key, method):
-
-        self.keybinds[key] = method
-
-    def keyPressed(self, event):
-
-        if event.keysym in self.keybinds:
-            method = self.keybinds[event.keysym]
-
-            method()
 
     def createContent(self):
         """ Create the Protocols View for the Project.
         It has two panes:
             Left: containing the Protocol classes tree
             Right: containing the Runs list
         """
-        p = tk.PanedWindow(self, orient=tk.HORIZONTAL, bg='white')
-        bgColor = Color.LIGHT_GREY_COLOR
+        p = tk.PanedWindow(self, orient=tk.HORIZONTAL, bg=Config.SCIPION_BG_COLOR)
+        bgColor = Color.ALT_COLOR
         # Left pane, contains Protocols Pane
         leftFrame = tk.Frame(p, bg=bgColor)
         leftFrame.columnconfigure(0, weight=1)
         leftFrame.rowconfigure(1, weight=1)
 
         # Protocols Tree Pane
         protFrame = tk.Frame(leftFrame, width=300, height=500, bg=bgColor)
@@ -670,38 +206,38 @@
         self.updateProtocolsTree(self.protCfg)
         # Create the right Pane that will be composed by:
         # a Action Buttons TOOLBAR in the top
         # and another vertical Pane with:
         # Runs History (at Top)
 
         # Selected run info (at Bottom)
-        rightFrame = tk.Frame(p, bg='white')
+        rightFrame = tk.Frame(p, bg=Config.SCIPION_BG_COLOR)
         rightFrame.columnconfigure(0, weight=1)
         rightFrame.rowconfigure(1, weight=1)
         # rightFrame.rowconfigure(0, minsize=label.winfo_reqheight())
 
         # Create the Action Buttons TOOLBAR
-        toolbar = tk.Frame(rightFrame, bg='white')
+        toolbar = tk.Frame(rightFrame, bg=Config.SCIPION_BG_COLOR)
         toolbar.grid(row=0, column=0, sticky='news')
         pwgui.configureWeigths(toolbar)
         # toolbar.columnconfigure(0, weight=1)
         toolbar.columnconfigure(1, weight=1)
 
-        self.runsToolbar = tk.Frame(toolbar, bg='white')
+        self.runsToolbar = tk.Frame(toolbar, bg=Config.SCIPION_BG_COLOR)
         self.runsToolbar.grid(row=0, column=0, sticky='sw')
         # On the left of the toolbar will be other
         # actions that can be applied to all runs (refresh, graph view...)
-        self.allToolbar = tk.Frame(toolbar, bg='white')
+        self.allToolbar = tk.Frame(toolbar, bg=Config.SCIPION_BG_COLOR)
         self.allToolbar.grid(row=0, column=10, sticky='se')
         self.createActionToolbar()
 
         # Create the Run History tree
         v = ttk.PanedWindow(rightFrame, orient=tk.VERTICAL)
         # runsFrame = ttk.Labelframe(v, text=' History ', width=500, height=500)
-        runsFrame = tk.Frame(v, bg='white')
+        runsFrame = tk.Frame(v, bg=Config.SCIPION_BG_COLOR)
         # runsFrame.grid(row=1, column=0, sticky='news', pady=5)
         self.runsTree = self.createRunsTree(runsFrame)
         pwgui.configureWeigths(runsFrame)
 
         self.createRunsGraph(runsFrame)
 
         if self.runsView == VIEW_LIST:
@@ -711,64 +247,69 @@
 
         treeWidget.grid(row=0, column=0, sticky='news')
 
         # Create the Selected Run Info
         infoFrame = tk.Frame(v)
         infoFrame.columnconfigure(0, weight=1)
         infoFrame.rowconfigure(1, weight=1)
+        # Create the info label
+        self.infoLabel = tk.Label(infoFrame)
+        self.infoLabel.grid(row=0, column=0, sticky='w', padx=3)
         # Create the Analyze results button
         self.btnAnalyze = pwgui.Button(infoFrame, text=Message.LABEL_ANALYZE,
-                                       fg='white', bg=Color.RED_COLOR,
+                                       fg='white', bg=Config.SCIPION_MAIN_COLOR,
                                        image=self.getImage(Icon.ACTION_VISUALIZE),
                                        compound=tk.LEFT,
                                        activeforeground='white',
-                                       activebackground='#A60C0C',
+                                       activebackground=Config.getActiveColor(),
                                        command=self._analyzeResultsClicked)
         self.btnAnalyze.grid(row=0, column=0, sticky='ne', padx=15)
         # self.style.configure("W.TNotebook")#, background='white')
         tab = ttk.Notebook(infoFrame)  # , style='W.TNotebook')
 
         # Summary tab
-        dframe = tk.Frame(tab, bg='white')
+        dframe = tk.Frame(tab, bg=Config.SCIPION_BG_COLOR)
         pwgui.configureWeigths(dframe, row=0)
         pwgui.configureWeigths(dframe, row=2)
-        provider = RunIOTreeProvider(self, self.getSelectedProtocol(),
-                                     self.project.mapper)
+        # Just configure the provider, later below, in updateSelection, it will be
+        # provided with the protocols.
+        provider = RunIOTreeProvider(self, None,
+                                     self.project.mapper, self.info)
 
         rowheight = pwgui.getDefaultFont().metrics()['linespace']
-        self.style.configure("NoBorder.Treeview", background='white',
+        self.style.configure("NoBorder.Treeview", background=Config.SCIPION_BG_COLOR,
                              borderwidth=0, font=self.windows.font,
-                             rowheight=rowheight)
+                             rowheight=rowheight, fieldbackground=Config.SCIPION_BG_COLOR)
         self.infoTree = pwgui.browser.BoundTree(dframe, provider, height=6,
                                                 show='tree',
                                                 style="NoBorder.Treeview")
         self.infoTree.grid(row=0, column=0, sticky='news')
-        label = tk.Label(dframe, text='SUMMARY', bg='white',
+        label = tk.Label(dframe, text='SUMMARY', bg=Config.SCIPION_BG_COLOR,
                          font=self.windows.fontBold)
         label.grid(row=1, column=0, sticky='nw', padx=(15, 0))
 
         hView = {'sci-open': self._viewObject,
                  'sci-bib': self._bibExportClicked}
 
         self.summaryText = pwgui.text.TaggedText(dframe, width=40, height=5,
-                                                 bg='white', bd=0,
+                                                 bg=Config.SCIPION_BG_COLOR, bd=0,
                                                  font=self.windows.font,
                                                  handlers=hView)
         self.summaryText.grid(row=2, column=0, sticky='news', padx=(30, 0))
 
         # Method tab
         mframe = tk.Frame(tab)
         pwgui.configureWeigths(mframe)
         # Methods text box
         self.methodText = pwgui.text.TaggedText(mframe, width=40, height=15,
-                                                bg='white', handlers=hView)
+                                                bg=Config.SCIPION_BG_COLOR, handlers=hView)
         self.methodText.grid(row=0, column=0, sticky='news')
         # Reference export button
         # btnExportBib = pwgui.Button(mframe, text=Message.LABEL_BIB_BTN,
-        #                             fg='white', bg=Color.RED_COLOR,
+        #                             fg='white', bg=Color.MAIN_COLOR,
         #                             image=self.getImage(Icon.ACTION_BROWSE),
         #                             compound=tk.LEFT,
         #                             activeforeground='white',
         #                             activebackground='#A60C0C',
         #                             command=self._bibExportClicked)
         # btnExportBib.grid(row=2, column=0, sticky='w', padx=0)
 
@@ -778,14 +319,21 @@
         self.outputViewer = pwgui.text.TextFileViewer(ologframe, allowOpen=True,
                                                       font=self.windows.font)
         self.outputViewer.grid(row=0, column=0, sticky='news')
         self.outputViewer.windows = self.windows
 
         self._updateSelection()
 
+        # Move to the selected protocol
+        if self._isSingleSelection():
+            prot = self.getSelectedProtocol()
+            node = self.runsGraph.getNode(str(prot.getObjId()))
+            self._selectNode(node)
+
+
         # Add all tabs
 
         tab.add(dframe, text=Message.LABEL_SUMMARY)
         tab.add(mframe, text=Message.LABEL_METHODS)
         tab.add(ologframe, text=Message.LABEL_LOGS_OUTPUT)
         #         tab.add(elogframe, text=Message.LABEL_LOGS_ERROR)
         #         tab.add(slogframe, text=Message.LABEL_LOGS_SCIPION)
@@ -827,87 +375,171 @@
 
     def _isSingleSelection(self):
         return len(self._selection) == 1
 
     def _noSelection(self):
         return len(self._selection) == 0
 
-    # noinspection PyUnusedLocal
+    def info(self, message):
+        self.infoLabel.config(text=message)
+        self.infoLabel.update_idletasks()
+
+    def cleanInfo(self):
+        self.info("")
+
     def refreshRuns(self, e=None, initRefreshCounter=True, checkPids=False):
+        """
+        Refresh the protocol runs workflow. If the variable REFRESH_WITH_THREADS
+        exits, then use a threads to refresh, i.o.c use normal behavior
+        """
+        useThreads = Config.refreshInThreads()
+        if useThreads:
+            import threading
+            # Refresh the status of displayed runs.
+            if self.refreshSemaphore:
+                # print("Launching a thread to refresh the runs...")
+                threadRefreshRuns = threading.Thread(name="Refreshing runs",
+                                                     target=self.refreshDisplayedRuns,
+                                                     args=(e, initRefreshCounter,
+                                                           checkPids))
+                threadRefreshRuns.start()
+            else:
+                self.repeatRefresh = True
+        else:
+            self.refreshDisplayedRuns(e, initRefreshCounter, checkPids)
+
+    # noinspection PyUnusedLocal
+    def refreshDisplayedRuns(self, e=None, initRefreshCounter=True, checkPids=False):
         """ Refresh the status of displayed runs.
          Params:
             e: Tk event input
             initRefreshCounter: if True the refresh counter will be set to 3 secs
              then only case when False is from _automaticRefreshRuns where the
              refresh time is doubled each time to avoid refreshing too often.
         """
+        self.viewButtons[ACTION_REFRESH]['state'] = tk.DISABLED
+        self.info('Refreshing...')
+        self.refreshSemaphore = False
         if Config.debugOn():
             import psutil
             proc = psutil.Process(os.getpid())
             mem = psutil.virtual_memory()
-            print("------------- refreshing ---------- ")
+            logger.debug("------------- refreshing ---------- ")
             files = proc.open_files()
-            print("  open files: ", len(files))
+            logger.debug("  open files: %s" % len(files))
             for f in files:
-                print("    - %s, %s" % (f.path, f.fd))
-            print("  memory percent: ", proc.memory_percent())
+                logger.debug("    - %s, %s" % (f.path, f.fd))
+            logger.debug("  memory percent: %s" % proc.memory_percent())
 
-        self.updateRunsGraph(True, checkPids=checkPids)
-        self.updateRunsTree(False)
+        if self.runsView == VIEW_LIST:
+            self.updateRunsTree(True)
+        else:
+            self.updateRunsGraph(True, checkPids=checkPids)
+            self._updateSelection()
 
         if initRefreshCounter:
 
             self.__autoRefreshCounter = INIT_REFRESH_SECONDS  # start by 3 secs
             if self.__autoRefresh:
                 self.runsTree.after_cancel(self.__autoRefresh)
                 self.__autoRefresh = self.runsTree.after(
                     self.__autoRefreshCounter * 1000,
                     self._automaticRefreshRuns)
+        self.refreshSemaphore = True
+        if self.repeatRefresh:
+            self.repeatRefresh = False
+            self.refreshRuns()
+        self.cleanInfo()
+        self.viewButtons[ACTION_REFRESH]['state'] = tk.NORMAL
 
     # noinspection PyUnusedLocal
     def _automaticRefreshRuns(self, e=None):
         """ Schedule automatic refresh increasing the time between refreshes. """
-        if pwutils.envVarOn('DO_NOT_AUTO_REFRESH'):
+        if pwutils.envVarOn(Config.SCIPION_GUI_CANCEL_AUTO_REFRESH):
             return
 
-        if self.project.needRefresh():
-            self.refreshRuns(initRefreshCounter=False)
-            secs = self.__autoRefreshCounter
-        else:
-            secs = INIT_REFRESH_SECONDS // 2
-
+        self.refreshRuns(initRefreshCounter=False, checkPids=True)
+        secs = self.__autoRefreshCounter
         # double the number of seconds up to 30 min
         self.__autoRefreshCounter = min(2 * secs, 1800)
         self.__autoRefresh = self.runsTree.after(secs * 1000,
                                                  self._automaticRefreshRuns)
 
     # noinspection PyUnusedLocal
     def _findProtocol(self, e=None):
         """ Find a desired protocol by typing some keyword. """
         window = SearchProtocolWindow(self.windows)
         window.show()
 
+    def _locateProtocol(self, e=None):
+
+        window = SearchRunWindow(self.windows, self.runsGraph, onDoubleClick=self._onRunClick)
+        window.show()
+        # self._moveCanvas(0,1)
+
+    def _onRunClick(self, e=None):
+        """ Callback to be called when a click happens o a run in the SearchRunWindow.tree"""
+        tree = e.widget
+        protId = tree.getFirst()
+        node = self.runsGraph.getNode(protId)
+        self._selectNode(node)
+
+    def _selectNode(self, node):
+
+        x = node.x
+        y = node.y
+        self._moveCanvas(x,y)
+
+        # Select the protocol
+        self._selectItemProtocol(node.run)
+        self.refreshDisplayedRuns()
+
+    def _moveCanvas(self, X, Y):
+
+        self.runsGraphCanvas.moveTo(X, Y)
+
+    def _scipionLog(self, e=None):
+        windows = ScipionLogWindow(self.windows)
+        windows.show()
+
     def createActionToolbar(self):
         """ Prepare the buttons that will be available for protocol actions. """
 
         self.actionButtons = {}
-        self.actionList = [ACTION_EDIT, ACTION_COPY, ACTION_DELETE,
-                           ACTION_STEPS, ACTION_BROWSE, ACTION_DB,
-                           ACTION_STOP, ACTION_CONTINUE, ACTION_RESULTS,
-                           ACTION_EXPORT, ACTION_EXPORT_UPLOAD, ACTION_COLLAPSE,
-                           ACTION_EXPAND, ACTION_LABELS]
+        actionList = [
+            ACTION_EDIT, ACTION_RENAME, ACTION_DUPLICATE, ACTION_COPY, ACTION_PASTE,  ACTION_DELETE,
+            ACTION_BROWSE,
+            ACTION_STOP, ACTION_STOP_WORKFLOW, ACTION_CONTINUE, ACTION_CONTINUE_WORKFLOW, ACTION_RESTART_WORKFLOW, ACTION_RESET_WORKFLOW,
+            ACTION_RESULTS,
+            ACTION_EXPORT, ACTION_EXPORT_UPLOAD,
+            ACTION_COLLAPSE, ACTION_EXPAND,
+            ACTION_LABELS, ACTION_SEARCH,
+            ACTION_SELECT_FROM, ACTION_SELECT_TO,
+            ACTION_STEPS, ACTION_DB
+        ]
 
         def addButton(action, text, toolbar):
-            btn = tk.Label(toolbar, text=text,
+            btn = tk.Label(toolbar, text="",
                            image=self.getImage(ActionIcons.get(action, None)),
-                           compound=tk.LEFT, cursor='hand2', bg='white')
-            btn.bind('<Button-1>', lambda e: self._runActionClicked(action))
+                           compound=tk.LEFT, cursor='hand2', bg=Config.SCIPION_BG_COLOR)
+
+            callback = lambda e: self._runActionClicked(action, event=e)
+            btn.bind(TK.LEFT_CLICK, callback)
+
+            # Shortcuts:
+            shortCut = ActionShortCuts.get(action, None)
+            if shortCut:
+                text += " (%s)" % shortCut
+                self.root.bind(shortCut, callback)
+
+            ToolTip(btn,text , 500)
+
             return btn
 
-        for action in self.actionList:
+        for action in actionList:
             self.actionButtons[action] = addButton(action, action,
                                                    self.runsToolbar)
 
         ActionIcons[ACTION_TREE] = RUNS_TREE
 
         self.viewButtons = {}
 
@@ -926,15 +558,15 @@
         # Add refresh button
         btn = addButton(ACTION_REFRESH, ACTION_REFRESH, self.allToolbar)
         btn.grid(row=0, column=2)
         self.viewButtons[ACTION_REFRESH] = btn
 
     def _createViewCombo(self, parent):
         """ Create the select-view combobox. """
-        label = tk.Label(parent, text='View:', bg='white')
+        label = tk.Label(parent, text='View:', bg=Config.SCIPION_BG_COLOR)
         label.grid(row=0, column=0)
         viewChoices = ['List', 'Tree', 'Tree - small']
         self.switchCombo = pwgui.widgets.ComboBox(parent, width=10,
                                                   choices=viewChoices,
                                                   values=[VIEW_LIST, VIEW_TREE, VIEW_TREE_SMALL],
                                                   initial=viewChoices[self.runsView],
                                                   onChange=lambda e: self._runActionClicked(
@@ -958,45 +590,42 @@
                 else:
                     action.grid_remove()
 
         for i, actionTuple in enumerate(self.provider.getActionsFromSelection()):
             action, cond = actionTuple
             displayAction(action, i, cond)
 
-    def _createProtocolsTree(self, parent, background=Color.LIGHT_GREY_COLOR,
+    def _createProtocolsTree(self, parent,
                              show='tree', columns=None):
-        defaultFont = pwgui.getDefaultFont()
-        self.style.configure("W.Treeview", background=background, borderwidth=0,
-                             fieldbackground=background,
-                             rowheight=defaultFont.metrics()['linespace'])
-        t = pwgui.tree.Tree(parent, show=show, style='W.Treeview',
+
+        t = pwgui.tree.Tree(parent, show=show, style=LIST_TREEVIEW,
                             columns=columns)
         t.column('#0', minwidth=300)
-        # Protocol nodes
-        t.tag_configure(ProtocolTreeConfig.TAG_PROTOCOL,
-                        image=self.getImage('python_file.gif'))
-        t.tag_bind(ProtocolTreeConfig.TAG_PROTOCOL,
-                   '<Double-1>', self._protocolItemClick)
-        t.tag_bind(ProtocolTreeConfig.TAG_PROTOCOL,
-                   '<Return>', self._protocolItemClick)
-        t.tag_bind(ProtocolTreeConfig.TAG_PROTOCOL,
-                   '<KP_Enter>', self._protocolItemClick)
 
-        # Disable protocols (not installed) are allowed to be added.
-        t.tag_configure(ProtocolTreeConfig.TAG_PROTOCOL_DISABLED,
-                        image=self.getImage('prot_disabled.gif'))
-        t.tag_bind(ProtocolTreeConfig.TAG_PROTOCOL_DISABLED,
-                   '<Double-1>', self._protocolItemClick)
-        t.tag_bind(ProtocolTreeConfig.TAG_PROTOCOL_DISABLED,
-                   '<Return>', self._protocolItemClick)
-        t.tag_bind(ProtocolTreeConfig.TAG_PROTOCOL_DISABLED,
-                   '<KP_Enter>', self._protocolItemClick)
+        def configureTag(tag, img):
+            # Protocol nodes
+            t.tag_configure(tag, image=self.getImage(img))
+            t.tag_bind(tag, TK.LEFT_DOUBLE_CLICK, self._protocolItemClick)
+            t.tag_bind(tag, TK.RETURN, self._protocolItemClick)
+            t.tag_bind(tag, TK.ENTER, self._protocolItemClick)
 
-        t.tag_configure('protocol_base', image=self.getImage('class_obj.gif'))
-        t.tag_configure('protocol_group', image=self.getImage('class_obj.gif'))
+        # Protocol nodes
+        configureTag(ProtocolTreeConfig.TAG_PROTOCOL, Icon.PRODUCTION)
+        # New protocols
+        configureTag(ProtocolTreeConfig.TAG_PROTOCOL_NEW, Icon.NEW)
+        # Beta protocols
+        configureTag(ProtocolTreeConfig.TAG_PROTOCOL_BETA, Icon.BETA)
+        # Disable protocols (not installed) are allowed to be added.
+        configureTag(ProtocolTreeConfig.TAG_PROTOCOL_DISABLED,
+                     Icon.PROT_DISABLED)
+        # Updates protocols
+        configureTag(ProtocolTreeConfig.TAG_PROTOCOL_UPDATED,
+                     Icon.UPDATED)
+        t.tag_configure('protocol_base', image=self.getImage(Icon.GROUP))
+        t.tag_configure('protocol_group', image=self.getImage(Icon.GROUP))
         t.tag_configure('section', font=self.windows.fontBold)
         return t
 
     def _createProtocolsPanel(self, parent, bgColor):
         """Create the protocols Tree displayed in left panel"""
         comboFrame = tk.Frame(parent, bg=bgColor)
         tk.Label(comboFrame, text='View', bg=bgColor).grid(row=0, column=0,
@@ -1055,21 +684,25 @@
         """
         protView = combo.getText()
         self.settings.setProtocolView(protView)
         self.protCfg = self.getCurrentProtocolView()
         self.updateProtocolsTree(self.protCfg)
 
     def populateTree(self, tree, treeItems, prefix, obj, subclassedDict, level=0):
-        text = obj.text.get()
+
+        # If node does not have leaves (protocols) do not add it
+        if not obj.visible:
+            return
+
+        text = obj.text
         if text:
-            value = obj.value.get(text)
+            value = obj.value if obj.value is not None else text
             key = '%s.%s' % (prefix, value)
-
-            img = obj.icon.get('')
-            tag = obj.tag.get('')
+            img = obj.icon if obj.icon is not None else ''
+            tag = obj.tag if obj.tag is not None else ''
 
             if len(img):
                 img = self.getImage(img)
                 # If image is none
                 img = img if img is not None else ''
 
             protClassName = value.split('.')[-1]  # Take last part
@@ -1086,78 +719,63 @@
                 text = prot.getClassLabel()
 
             item = tree.insert(prefix, 'end', key, text=text, image=img, tags=tag)
             treeItems[item] = obj
             # Check if the attribute should be open or close
             openItem = getattr(obj, 'openItem', level < 2)
             if openItem:
-                tree.item(item, open=True)
+                tree.item(item, open=openItem)
 
-            if obj.value.hasValue() and tag == 'protocol_base':
-                if prot is not None:
-                    tree.item(item, image=self.getImage('class_obj.gif'))
-
-                    for k, v in emProtocolsDict.items():
-                        if (k not in subclassedDict and v is not prot and
-                           issubclass(v, prot)):
-                            key = '%s.%s' % (item, k)
-                            t = v.getClassLabel()
-                            tree.insert(item, 'end', key, text=t, tags='protocol')
-                else:
-                    raise Exception("Class '%s' not found" % obj.value.get())
+            # I think this mode is deprecated
+            if obj.value is not None and tag == 'protocol_base':
+                logger.warning('protocol_base tags are deprecated')
         else:
             key = prefix
 
         for sub in obj:
             self.populateTree(tree, treeItems, key, sub, subclassedDict,
                               level + 1)
 
     def updateProtocolsTree(self, protCfg):
 
         try:
             self.protCfg = protCfg
             self.protTree.clear()
-            self.protTree.unbind('<<TreeviewOpen>>')
-            self.protTree.unbind('<<TreeviewClose>>')
+            self.protTree.unbind(TK.TREEVIEW_OPEN)
+            self.protTree.unbind(TK.TREEVIEW_CLOSE)
             self.protTreeItems = {}
             subclassedDict = {}  # Check which classes serve as base to not show them
             emProtocolsDict = self.domain.getProtocols()
             for _, v1 in emProtocolsDict.items():
                 for k2, v2 in emProtocolsDict.items():
                     if v1 is not v2 and issubclass(v1, v2):
                         subclassedDict[k2] = True
             self.populateTree(self.protTree, self.protTreeItems, '', self.protCfg,
                               subclassedDict)
-            self.protTree.bind('<<TreeviewOpen>>',
+            self.protTree.bind(TK.TREEVIEW_OPEN,
                                lambda e: self._treeViewItemChange(True))
-            self.protTree.bind('<<TreeviewClose>>',
+            self.protTree.bind(TK.TREEVIEW_CLOSE,
                                lambda e: self._treeViewItemChange(False))
         except Exception as e:
             # Tree can't be loaded report back, but continue
             print("Protocols tree couldn't be loaded: %s" % e)
 
     def _treeViewItemChange(self, openItem):
         item = self.protTree.focus()
         if item in self.protTreeItems:
-            self.protTreeItems[item].openItem.set(openItem)
+            self.protTreeItems[item].openItem = openItem
 
     def createRunsTree(self, parent):
         self.provider = RunsTreeProvider(self.project, self._runActionClicked)
 
         # This line triggers the getRuns for the first time.
         # Ne need to force the check pids here, temporary
         self.provider._checkPids = True
 
-        # To specify the height of the rows based on the font size.
-        # Should be centralized somewhere.
-        style = ttk.Style()
-        rowheight = pwgui.getDefaultFont().metrics()['linespace']
-        style.configure('List.Treeview', rowheight=rowheight)
-
-        t = pwgui.tree.BoundTree(parent, self.provider, style='List.Treeview')
+        t = pwgui.tree.BoundTree(parent, self.provider, style=LIST_TREEVIEW)
         self.provider._checkPids = False
 
         t.itemDoubleClick = self._runItemDoubleClick
         t.itemClick = self._runTreeItemClick
 
         return t
 
@@ -1190,49 +808,59 @@
         parent.grid_rowconfigure(0, weight=1)
 
         self.settings.getNodes().updateDict()
         self.settings.getLabels().updateDict()
 
         self.updateRunsGraph()
 
-    def updateRunsGraph(self, refresh=False, reorganize=False, checkPids=False):
+    def updateRunsGraph(self, refresh=False, checkPids=False):
 
         self.runsGraph = self.project.getRunsGraph(refresh=refresh,
                                                    checkPids=checkPids)
-        self.drawRunsGraph(reorganize)
+        self.drawRunsGraph()
 
     def drawRunsGraph(self, reorganize=False):
 
-        self.runsGraphCanvas.clear()
-
         # Check if there are positions stored
-        if reorganize or len(self.settings.getNodes()) == 0:
+        if reorganize:
             # Create layout to arrange nodes as a level tree
             layout = pwgui.LevelTreeLayout()
+            self.runsGraphCanvas.reorganizeGraph(self.runsGraph, layout)
         else:
-            layout = pwgui.BasicLayout()
-
-        # Create empty nodeInfo for new runs
-        for node in self.runsGraph.getNodes():
-            nodeId = node.run.getObjId() if node.run else 0
-            nodeInfo = self.settings.getNodeById(nodeId)
-            if nodeInfo is None:
-                self.settings.addNode(nodeId, x=0, y=0, expanded=True)
+            self.runsGraphCanvas.clear()
+            layout = pwgui.LevelTreeLayout(partial=True)
 
-        self.runsGraphCanvas.drawGraph(self.runsGraph, layout,
-                                       drawNode=self.createRunItem)
+            # Create empty nodeInfo for new runs
+            for node in self.runsGraph.getNodes():
+                nodeId = node.run.getObjId() if node.run else 0
+                nodeInfo = self.settings.getNodeById(nodeId)
+                if nodeInfo is None:
+                    self.settings.addNode(nodeId, x=0, y=0, expanded=True,
+                                          visible=True)
+
+            self.runsGraphCanvas.drawGraph(self.runsGraph, layout,
+                                           drawNode=self.createRunItem,
+                                           nodeList=self.settings.nodeList)
+
+            projectSize = len(self.runsGraph.getNodes())
+            settingsNodeSize = len(self.settings.getNodes())
+            if projectSize < settingsNodeSize -1:
+                logger.info("Settings nodes list (%s) is bigger than current project nodes (%s). "
+                            "Clean up needed?" % (settingsNodeSize, projectSize) )
+                self.settings.cleanUpNodes(self.runsGraph.getNodeNames(), toRemove=False)
 
     def createRunItem(self, canvas, node):
 
         nodeId = node.run.getObjId() if node.run else 0
         nodeInfo = self.settings.getNodeById(nodeId)
 
         # Extend attributes: use some from nodeInfo
         node.expanded = nodeInfo.isExpanded()
         node.x, node.y = nodeInfo.getPosition()
+        node.visible = nodeInfo.isVisible()
         nodeText = self._getNodeText(node)
 
         # Get status color
         statusColor = getStatusColorFromNode(node)
 
         # Get the box color (depends on color mode: label or status)
         boxColor = self._getBoxColor(nodeInfo, statusColor, node)
@@ -1246,16 +874,15 @@
 
         # Paint the oval..if apply.
         self._paintOval(item, statusColor)
 
         # Paint the bottom line (for now only labels are painted there).
         self._paintBottomLine(item)
 
-        if nodeId in self._selection:
-            item.setSelected(True)
+        item.setSelected(nodeId in self._selection)
         return item
 
     def _getBoxColor(self, nodeInfo, statusColor, node):
 
         try:
 
             # If the color has to go to the box
@@ -1282,14 +909,21 @@
                         protAge = ts - creationTime
 
                         boxColor = self._ageColor('#6666ff', elapsedTime,
                                                   protAge)
                 else:
                     boxColor = DEFAULT_BOX_COLOR
 
+            elif self.settings.sizeColorMode():
+
+                # Get the protocol size
+                protSize = self._getRunSize(node)
+
+                boxColor = self._sizeColor(protSize)
+
             # ... box is for the labels.
             elif self.settings.labelsColorMode():
                 # If there is only one label use the box for the color.
                 if self._getLabelsCount(nodeInfo) == 1:
 
                     labelId = nodeInfo.getLabels()[0]
                     label = self.settings.getLabels().getLabel(labelId)
@@ -1304,30 +938,60 @@
                 else:
                     boxColor = DEFAULT_BOX_COLOR
             else:
                 boxColor = DEFAULT_BOX_COLOR
 
             return boxColor
         except Exception as e:
+            logger.debug("Can't get color for %s. %s" % (node, e))
             return DEFAULT_BOX_COLOR
 
     @staticmethod
-    def _ageColor(rgbColor, projectAge, protocolAge):
+    def _getRunSize(node):
+        """
+        Returns the size "recursively" of a run
+
+        :param node: node of the graph.
+        :return: size in bytes
+
+        """
+
+        if not node.run:
+            return 0
+        else:
+            return node.run.getSize()
+
+    @classmethod
+    def _sizeColor(cls, size):
+        """
+        Returns the color that corresponds to the size
+        :param size:
+        :return:
+        """
+
+        for threshold, color in cls.SIZE_COLORS.items():
+            if size <= threshold:
+                return color
+
+        return "#000000"
+    @staticmethod
+    def _ageColor(rgbColorStr, projectAge, protocolAge):
 
         #  Get the ratio
         ratio = protocolAge.seconds / float(projectAge.seconds)
 
         # Invert direction: older = white = 100%, newest = rgbColor = 0%
         ratio = 1 - ratio
 
         # There are cases coming with protocols older than the project.
         ratio = 0 if ratio < 0 else ratio
 
-        return pwutils.rgb_to_hex(pwutils.lighter(pwutils.hex_to_rgb(rgbColor),
-                                                  ratio))
+        hexTuple = pwutils.hex_to_rgb(rgbColorStr)
+        lighterTuple = pwutils.lighter(hexTuple, ratio)
+        return pwutils.rgb_to_hex(lighterTuple)
 
     @staticmethod
     def _getLabelsCount(nodeInfo):
 
         return 0 if nodeInfo.getLabels() is None else len(nodeInfo.getLabels())
 
     def _paintBottomLine(self, item):
@@ -1364,19 +1028,19 @@
     def _getNodeText(self, node):
         nodeText = node.getLabel()
         # Truncate text to prevent overflow
         if len(nodeText) > 40:
             nodeText = nodeText[:37] + "..."
 
         if node.run:
-            expandedStr = '' if node.expanded else ' (+)'
+            expandedStr = '' if node.expanded else '\n ➕ %s more' % str(node.countChilds({}))
             if self.runsView == VIEW_TREE_SMALL:
                 nodeText = node.getName() + expandedStr
             else:
-                nodeText += expandedStr + '\n' + node.run.getStatusMessage()
+                nodeText += expandedStr + '\n' + node.run.getStatusMessage() if not expandedStr else expandedStr
                 if node.run.summaryWarnings:
                     nodeText += u' \u26a0'
         return nodeText
 
     def _addLabels(self, item):
         # If there is only one label it should be already used in the box color.
         if self._getLabelsCount(item.nodeInfo) < 2:
@@ -1415,55 +1079,76 @@
                                 labelWidth, labelHeight, color=label.getColor(),
                                 anchor=item)
             else:
 
                 item.nodeInfo.getLabels().remove(labelId)
 
     def switchRunsView(self):
-        previousView = self.runsView
         viewValue = self.switchCombo.getValue()
         self.runsView = viewValue
         self.settings.setRunsView(viewValue)
 
         if viewValue == VIEW_LIST:
             self.runsTree.grid(row=0, column=0, sticky='news')
             self.runsGraphCanvas.frame.grid_remove()
-            self.updateRunsTreeSelection()
+            self.updateRunsTree()
             self.viewButtons[ACTION_TREE].grid_remove()
             self._lastRightClickPos = None
         else:
             self.runsTree.grid_remove()
-            self.updateRunsGraph(reorganize=(previousView != VIEW_LIST))
+            self.updateRunsGraph()
             self.runsGraphCanvas.frame.grid(row=0, column=0, sticky='news')
             self.viewButtons[ACTION_TREE].grid(row=0, column=1)
 
     def _protocolItemClick(self, e=None):
         # Get the tree widget that originated the event
         # it could be the left panel protocols tree or just
         # the search protocol dialog tree
         tree = e.widget
         protClassName = tree.getFirst().split('.')[-1]
         protClass = self.domain.getProtocols().get(protClassName)
         prot = self.project.newProtocol(protClass)
-        self._openProtocolForm(prot)
+        self._openProtocolForm(prot, disableRunMode=True)
 
     def _toggleColorScheme(self, e=None):
 
         currentMode = self.settings.getColorMode()
 
         if currentMode >= len(self.settings.COLOR_MODES) - 1:
             currentMode = -1
 
         nextColorMode = currentMode + 1
 
         self.settings.setColorMode(nextColorMode)
         self._updateActionToolbar()
         # self.updateRunsGraph()
         self.drawRunsGraph()
+        self._infoAboutColorScheme()
+
+    def _infoAboutColorScheme(self):
+        """ Writes in the info widget a brief description abot the color scheme."""
+
+        colorScheme = self.settings.getColorMode()
+
+        msg = "Color mode changed to %s. %s"
+        if colorScheme == self.settings.COLOR_MODE_AGE:
+            msg = msg % ("AGE", "Young boxes will have an darker color.")
+        elif colorScheme == self.settings.COLOR_MODE_SIZE:
+            keys = list(self.SIZE_COLORS.keys())
+            msg = msg % ("SIZE", "Semaphore color scheme. Green <= %s, Orange <=%s, Red <=%s, Dark quite big." %
+                         (pwutils.prettySize(keys[0]),
+                          pwutils.prettySize(keys[1]),
+                          pwutils.prettySize(keys[2]))
+                         )
+        elif colorScheme == self.settings.COLOR_MODE_STATUS:
+            msg = msg % ("STATUS", "Color based on the status. A black circle indicates it has labels")
+        elif colorScheme == self.settings.COLOR_MODE_LABELS:
+            msg = msg % ("LABELS", "Color based on custom labels you've assigned. Small circles reflect the protocol status")
 
+        self.info(msg)
     def _toggleDebug(self, e=None):
         Config.toggleDebug()
 
     def _selectAllProtocols(self, e=None):
         self._selection.clear()
 
         # WHY GOING TO THE db?
@@ -1538,15 +1223,15 @@
 
         self._updateSelection()
         self.runsGraphCanvas.update_idletasks()
 
     def _deselectItems(self, item):
         """ Deselect all items except the item one
         """
-        g = self.project.getRunsGraph(refresh=False)
+        g = self.project.getRunsGraph()
 
         for node in g.getNodes():
             if node.run and node.run.getObjId() in self._selection:
                 # This option is only for compatibility with all projects
                 if hasattr(node, 'item'):
                     node.item.setSelected(False)
         item.setSelected(True)
@@ -1567,15 +1252,16 @@
             prot = item.node.run
             if prot is None:  # in case it is the main "Project" node
                 return
             self._deselectItems(item)
         self._selectItemProtocol(prot)
 
     def _runItemDoubleClick(self, e=None):
-        self._runActionClicked(ACTION_EDIT)
+        if e.nodeInfo.isExpanded():
+            self._runActionClicked(ACTION_EDIT)
 
     def _runItemMiddleClick(self, e=None):
         self._runActionClicked(ACTION_SELECT_TO)
 
     def _runItemRightClick(self, item=None):
         prot = item.node.run
         if prot is None:  # in case it is the main "Project" node
@@ -1635,23 +1321,26 @@
             tw: a tk.TopLevel instance (ToolTipWindow)
             item: the selected item.
         """
         prot = item.node.run
 
         if prot:
             tm = '*%s*\n' % prot.getRunName()
-            tm += '   Id: %s\n' % prot.getObjId()
-            tm += 'State: %s\n' % prot.getStatusMessage()
-            tm += ' Time: %s\n' % pwutils.prettyDelta(prot.getElapsedTime())
+            tm += 'Identifier :%s\n' % prot.getObjId()
+            tm += 'Status: %s\n' % prot.getStatusMessage()
+            tm += 'Wall time: %s\n' % pwutils.prettyDelta(prot.getElapsedTime())
+            tm += 'CPU time: %s\n' % pwutils.prettyDelta(dt.timedelta(seconds=prot.cpuTime))
+            tm += 'Folder size: %s\n' % pwutils.prettySize(prot.getSize())
+
             if not hasattr(tw, 'tooltipText'):
                 frame = tk.Frame(tw)
                 frame.grid(row=0, column=0)
                 tw.tooltipText = pwgui.dialog.createMessageBody(frame, tm, None,
                                                                 textPad=0,
-                                                                textBg=Color.LIGHT_GREY_COLOR_2)
+                                                                textBg=Color.ALT_COLOR_2)
                 tw.tooltipText.config(bd=1, relief=tk.RAISED)
             else:
                 pwgui.dialog.fillMessageText(tw.tooltipText, tm)
 
     @staticmethod
     def _selectItemsWithinArea(x1, y1, x2, y2, enclosed=False):
         """
@@ -1685,21 +1374,22 @@
         #         if not item.node.isRoot():
         #             item.setSelected(True)
         #             self._selection.append(itemId)
         #             update = True
         #
         # if update is not None: self._updateSelection()
 
-    def _openProtocolForm(self, prot):
+    def _openProtocolForm(self, prot, disableRunMode=False):
         """Open the Protocol GUI Form given a Protocol instance"""
 
         w = FormWindow(Message.TITLE_NAME_RUN + prot.getClassName(),
                        prot, self._executeSaveProtocol, self.windows,
                        hostList=self.project.getHostNames(),
-                       updateProtocolCallback=self._updateProtocol(prot))
+                       updateProtocolCallback=self._updateProtocol,
+                       disableRunMode=disableRunMode)
         w.adjustSize()
         w.show(center=True)
 
     def _browseSteps(self):
         """ Open a new window with the steps list. """
         window = StepsWindow(Message.TITLE_BROWSE_DATA, self.windows,
                              self.getSelectedProtocol())
@@ -1715,25 +1405,27 @@
 
     def _browseRunDirectory(self):
         """ Open a file browser to inspect the files generated by the run. """
         protocol = self.getSelectedProtocol()
         workingDir = protocol.getWorkingDir()
         if os.path.exists(workingDir):
 
+            protFolderShortCut = ShortCut.factory(workingDir,name="Protocol folder", icon=None ,toolTip="Protocol directory")
             window = pwgui.browser.FileBrowserWindow("Browsing: " + workingDir,
                                                      master=self.windows,
-                                                     path=workingDir)
+                                                     path=workingDir,
+                                                     shortCuts=[protFolderShortCut])
             window.show()
         else:
             self.windows.showInfo("Protocol working dir does not exists: \n %s"
                                   % workingDir)
 
     def _iterSelectedProtocols(self):
         for protId in sorted(self._selection):
-            prot = self.project.getProtocol(protId)
+            prot = self.project.getRunsGraph().getNode(str(protId)).run
             if prot:
                 yield prot
 
     def _getSelectedProtocols(self):
         return [prot for prot in self._iterSelectedProtocols()]
 
     def _iterSelectedNodes(self):
@@ -1764,15 +1456,15 @@
         self.infoTree.clear()
         n = len(self._selection)
 
         if n == 1:
             prot = self.getSelectedProtocol()
 
             if prot:
-                provider = RunIOTreeProvider(self, prot, self.project.mapper)
+                provider = RunIOTreeProvider(self, prot, self.project.mapper, self.info)
                 self.infoTree.setProvider(provider)
                 self.infoTree.grid(row=0, column=0, sticky='news')
                 self.infoTree.update_idletasks()
                 # Update summary
                 self.summaryText.addText(prot.summary())
             else:
                 self.infoTree.clear()
@@ -1809,41 +1501,48 @@
                     self.methodText.addLine(cite)
 
             self.methodText.setReadOnly(True)
         except Exception as e:
             self.methodText.addLine('Could not load all methods:' + str(e))
 
     def _fillLogs(self):
-        prot = self.getSelectedProtocol()
+        try:
+            prot = self.getSelectedProtocol()
 
-        if not self._isSingleSelection() or not prot:
-            self.outputViewer.clear()
-            self._lastStatus = None
-        elif prot.getObjId() != self._lastSelectedProtId:
-            self._lastStatus = prot.getStatus()
-            i = self.outputViewer.getIndex()
-            self.outputViewer.clear()
-            # Right now skip the err tab since we are redirecting
-            # stderr to stdout
-            out, _, log, schedule = prot.getLogPaths()
-            self.outputViewer.addFile(out)
-            self.outputViewer.addFile(log)
-            if os.path.exists(schedule):
-                self.outputViewer.addFile(schedule)
-            self.outputViewer.setIndex(i)  # Preserve the last selected tab
-            self.outputViewer.selectedText().goEnd()
-            # when there are not logs, force re-load next time
-            if (not os.path.exists(out) or
-                    not os.path.exists(log)):
+            if not self._isSingleSelection() or not prot:
+                self.outputViewer.clear()
                 self._lastStatus = None
-
-        elif prot.isActive() or prot.getStatus() != self._lastStatus:
-            doClear = self._lastStatus is None
-            self._lastStatus = prot.getStatus()
-            self.outputViewer.refreshAll(clear=doClear, goEnd=doClear)
+            elif prot.getObjId() != self._lastSelectedProtId:
+                self._lastStatus = prot.getStatus()
+                i = self.outputViewer.getIndex()
+                self.outputViewer.clear()
+                # Right now skip the err tab since we are redirecting
+                # stderr to stdout
+                out, err, schedule = prot.getLogPaths()
+                self.outputViewer.addFile(out)
+                self.outputViewer.addFile(err)
+                if os.path.exists(schedule):
+                    self.outputViewer.addFile(schedule)
+                elif i == 2:
+                    i = 0
+                self.outputViewer.setIndex(i)  # Preserve the last selected tab
+                self.outputViewer.selectedText().goEnd()
+                # when there are not logs, force re-load next time
+                if (not os.path.exists(out) or
+                        not os.path.exists(err)):
+                    self._lastStatus = None
+
+            elif prot.isActive() or prot.getStatus() != self._lastStatus:
+                doClear = self._lastStatus is None
+                self._lastStatus = prot.getStatus()
+                self.outputViewer.refreshAll(clear=doClear, goEnd=doClear)
+        except Exception as e:
+            self.info("Something went wrong filling %s's logs: %s. Check terminal for details" % (prot, e))
+            import traceback
+            traceback.print_exc()
 
     def _scheduleRunsUpdate(self, secs=1):
         # self.runsTree.after(secs*1000, self.refreshRuns)
         self.windows.enqueue(self.refreshRuns)
 
     def executeProtocol(self, prot):
         """ Function to execute a protocol called not
@@ -1870,14 +1569,15 @@
             self._updateSelection()
             self._lastStatus = None  # clear lastStatus to force re-load the logs
             msg = ""
 
         # Update runs list display, even in save we
         # need to get the updated copy of the protocol
         self._scheduleRunsUpdate()
+        self._selectItemProtocol(prot)
 
         return msg
 
     def _updateProtocol(self, prot):
         """ Callback to notify about the change of a protocol
         label or comment. 
         """
@@ -1893,189 +1593,278 @@
         # proceed with the delete action
 
         # get the widget with the focus
         widget = self.focus_get()
 
         # Call the delete action only if the widget is the canvas
         if str(widget).endswith(ProtocolsView.RUNS_CANVAS_NAME):
-            self._deleteProtocol()
+            try:
+                self._deleteProtocol()
+            except Exception as ex:
+                self.windows.showError(str(ex))
 
     def _deleteProtocol(self):
         protocols = self._getSelectedProtocols()
 
         if len(protocols) == 0:
             return
 
         protStr = '\n  - '.join(['*%s*' % p.getRunName() for p in protocols])
 
         if pwgui.dialog.askYesNo(Message.TITLE_DELETE_FORM,
                                  Message.LABEL_DELETE_FORM % protStr,
                                  self.root):
+            self.info('Deleting protocols...')
             self.project.deleteProtocol(*protocols)
+            self.settings.cleanUpNodes([str(prot.getObjId()) for prot in protocols])
             self._selection.clear()
             self._updateSelection()
             self._scheduleRunsUpdate()
+            self.cleanInfo()
+
+
+    def _editProtocol(self, protocol):
+        disableRunMode = False
+        if protocol.isSaved():
+            disableRunMode = True
+        self._openProtocolForm(protocol, disableRunMode=disableRunMode)
+
+    def _pasteProtocolsFromClipboard(self, e=None):
+        """ Pastes the content of the clipboard providing is a json workflow"""
+
+        try:
+
+            self.project.loadProtocols(jsonStr=self.clipboard_get())
+            self.info("Clipboard content pasted successfully.")
+        except Exception as e:
+            self.info("Paste failed, maybe clipboard content is not valid content? See GUI log for details.")
+            logger.error("Clipboard content couldn't be pasted." , exc_info=e)
+
+    def _copyProtocolsToClipboard(self, e=None):
+
+        protocols = self._getSelectedProtocols()
 
-    def _copyProtocols(self):
+        jsonStr = self.project.getProtocolsJson(protocols)
+
+        self.clipboard_clear()
+        self.clipboard_append(jsonStr)
+        self.info("Protocols copied to the clipboard. Now you can paste them here, another project or in a template or ... anywhere!.")
+
+    def _copyProtocols(self, e=None):
         protocols = self._getSelectedProtocols()
         if len(protocols) == 1:
             newProt = self.project.copyProtocol(protocols[0])
             if newProt is None:
                 self.windows.showError("Error copying protocol.!!!")
             else:
-                self._openProtocolForm(newProt)
+                self._openProtocolForm(newProt, disableRunMode=True)
         else:
+            self.info('Copying the protocols...')
             self.project.copyProtocol(protocols)
             self.refreshRuns()
+            self.cleanInfo()
 
     def _stopWorkFlow(self, action):
 
         protocols = self._getSelectedProtocols()
-        errorList = []
-        if pwgui.dialog.askYesNo(Message.TITLE_STOP_WORKFLOW_FORM,
-                                 Message.TITLE_STOP_WORKFLOW, self.root):
-            defaultModeMessage = 'Stopping the workflow...'
-            message = FloatingMessage(self.root, defaultModeMessage)
-            message.show()
-            errorList = self.project.stopWorkFlow(protocols[0])
-            self.refreshRuns()
-            message.close()
-        if errorList:
-            msg = ''
-            for errorProt in errorList:
-                error = ("The protocol: %s  is active\n" %
-                         (self.project.getProtocol(errorProt).getRunName()))
-                msg += str(error)
-            pwgui.dialog.MessageDialog(
-                self, Message.TITLE_STOPPED_WORKFLOW_FAILED,
-                Message.TITLE_STOPPED_WORKFLOW_FAILED + msg,
-                'fa-times-circle_alert.gif')
+
+        # TODO: use filterCallback param and we may not need to return 2 elements
+        workflowProtocolList, activeProtList = self.project._getSubworkflow(protocols[0],
+                                                                            fixProtParam=False,
+                                                                            getStopped=False)
+        if activeProtList:
+            errorProtList = []
+            if pwgui.dialog.askYesNo(Message.TITLE_STOP_WORKFLOW_FORM,
+                                     Message.TITLE_STOP_WORKFLOW, self.root):
+                self.info('Stopping the workflow...')
+                errorProtList = self.project.stopWorkFlow(activeProtList)
+                self.cleanInfo()
+                self.refreshRuns()
+            if errorProtList:
+                msg = '\n'
+                for prot in errorProtList:
+                    msg += str(prot.getObjLabel()) + '\n'
+                pwgui.dialog.MessageDialog(
+                    self, Message.TITLE_STOPPED_WORKFLOW_FAILED,
+                    Message.TITLE_STOPPED_WORKFLOW_FAILED + ' with: ' + msg,
+                    Icon.ERROR)
 
     def _resetWorkFlow(self, action):
 
         protocols = self._getSelectedProtocols()
-        errorList = []
+        errorProtList = []
         if pwgui.dialog.askYesNo(Message.TITLE_RESET_WORKFLOW_FORM,
                                  Message.TITLE_RESET_WORKFLOW, self.root):
-            defaultModeMessage = 'Resetting the workflow...'
-            message = FloatingMessage(self.root, defaultModeMessage)
-            message.show()
-            errorList = self.project.resetWorkFlow(protocols[0])
+            self.info('Resetting the workflow...')
+            workflowProtocolList, activeProtList = self.project._getSubworkflow(protocols[0])
+            errorProtList = self.project.resetWorkFlow(workflowProtocolList)
+            self.cleanInfo()
             self.refreshRuns()
-            message.close()
-        if errorList:
-            msg = ''
-            for errorProt in errorList:
-                error = ("The protocol: %s  is active\n" %
-                         (self.project.getProtocol(errorProt).getRunName()))
-                msg += str(error)
+        if errorProtList:
+            msg = '\n'
+            for prot in errorProtList:
+                msg += str(prot.getObjLabel()) + '\n'
             pwgui.dialog.MessageDialog(
                 self, Message.TITLE_RESETED_WORKFLOW_FAILED,
-                Message.TITLE_RESETED_WORKFLOW_FAILED + msg,
-                'fa-times-circle_alert.gif')
+                Message.TITLE_RESETED_WORKFLOW_FAILED + ' with: ' + msg,
+                Icon.ERROR)
 
     def _launchWorkFlow(self, action):
         """
         This function can launch a workflow from a selected protocol in two
         modes depending on the 'action' value (RESTART, CONTINUE)
         """
         protocols = self._getSelectedProtocols()
-        errorList = []
-        defaultMode = pwprot.MODE_CONTINUE
-        defaultModeMessage = 'Checking the workflow to continue...'
-
-        if action == ACTION_RESTART_WORKFLOW:
-            if pwgui.dialog.askYesNo(Message.TITLE_RESTART_WORKFLOW_FORM,
-                                     Message.TITLE_RESTART_WORKFLOW, self.root):
-                defaultMode = pwprot.MODE_RESTART
-                defaultModeMessage = 'Checking the workflow to restart...'
-
-                message = FloatingMessage(self.root, defaultModeMessage)
-                message.show()
-                errorList = self.project.launchWorkflow(protocols[0],
-                                                        defaultMode)
-                self.refreshRuns()
-                message.close()
-        elif action == ACTION_CONTINUE_WORKFLOW:
-            message = FloatingMessage(self.root, defaultModeMessage)
-            message.show()
-            errorList = self.project.launchWorkflow(protocols[0],
-                                                    defaultMode)
-            self.refreshRuns()
-            message.close()
+        mode = pwprot.MODE_RESTART if action == ACTION_RESTART_WORKFLOW else pwprot.MODE_RESUME
+        errorList, _ = self._launchSubWorkflow(protocols[0], mode,  self.root)
 
         if errorList:
             msg = ''
             for errorProt in errorList:
-                error = ("The protocol: %s  is active\n" %
-                         (self.project.getProtocol(errorProt).getRunName()))
-                msg += str(error)
+                msg += str(errorProt) + '\n'
             pwgui.dialog.MessageDialog(
                 self, Message.TITLE_LAUNCHED_WORKFLOW_FAILED_FORM,
                 Message.TITLE_LAUNCHED_WORKFLOW_FAILED + "\n" + msg,
-                'fa-times-circle_alert.gif')
+                Icon.ERROR)
+        self.refreshRuns()
+
+    @staticmethod
+    def _launchSubWorkflow(protocol, mode, root, askSingleAll=False):
+        """
+        Method to launch a subworkflow
+        mode: mode value (RESTART, CONTINUE)
+        askSingleAll: specify if this method was launched from the form or from the menu
+        """
+        project = protocol.getProject()
+        workflowProtocolList, activeProtList = project._getSubworkflow(protocol)
+
+        # Check if exists active protocols
+        activeProtocols = ""
+        if activeProtList:
+            for protId, activeProt in activeProtList.items():
+                activeProtocols += ("\n* " + activeProt.getRunName())
+
+        # by default, we assume RESTART workflow option
+        title = Message.TITLE_RESTART_WORKFLOW_FORM
+        message = Message.MESSAGE_RESTART_WORKFLOW_WITH_RESULTS % ('%s\n' % activeProtocols) if len(activeProtList) else Message.MESSAGE_RESTART_WORKFLOW
+
+        if mode == pwprot.MODE_RESUME:
+             message = Message.MESSAGE_CONTINUE_WORKFLOW_WITH_RESULTS % ('%s\n' % activeProtocols) if len(activeProtList) else Message.MESSAGE_CONTINUE_WORKFLOW
+             title = Message.TITLE_CONTINUE_WORKFLOW_FORM
+
+        if not askSingleAll:
+            if pwgui.dialog.askYesNo(title,  message, root):
+                project.launchWorkflow(workflowProtocolList, mode)
+                return [], RESULT_RUN_ALL
+            return [], RESULT_CANCEL
+        else:  # launching from a form
+            if len(workflowProtocolList) > 1:
+                title = Message.TITLE_RESTART_FORM if mode == pwprot.MODE_RESTART else Message.TITLE_CONTINUE_FORM
+                message += Message.MESSAGE_ASK_SINGLE_ALL
+                result = pwgui.dialog.askSingleAllCancel(title, message,
+                                                         root)
+                if result == RESULT_RUN_ALL:
+                    if mode == pwprot.MODE_RESTART:
+                        project._restartWorkflow(workflowProtocolList)
+                    else:
+                        project._continueWorkflow(workflowProtocolList)
+
+                    return [], RESULT_RUN_ALL
+
+                elif result == RESULT_RUN_SINGLE:
+                    errorList = project.resetWorkFlow(workflowProtocolList)
+                    return errorList, RESULT_RUN_SINGLE
+
+                elif result == RESULT_CANCEL:
+                    return [], RESULT_CANCEL
+
+            else:  # is a single protocol
+                if not protocol.isSaved():
+                    title = Message.TITLE_RESTART_FORM
+                    message = Message.MESSAGE_RESTART_FORM % ('%s\n' % protocol.getRunName())
+                    if mode == pwprot.MODE_RESUME:
+                        title = Message.TITLE_CONTINUE_FORM
+                        message = Message.MESSAGE_CONTINUE_FORM % ('%s\n' % protocol.getRunName())
+
+                    result = pwgui.dialog.askYesNo(title,  message,  root)
+                    resultRun = RESULT_RUN_SINGLE if result else RESULT_CANCEL
+                    return [], resultRun
+
+                return [], RESULT_RUN_SINGLE
 
     def _selectLabels(self):
         selectedNodes = self._getSelectedNodes()
 
         if selectedNodes:
             dlg = self.windows.manageLabels()
 
             if dlg.resultYes():
                 for node in selectedNodes:
                     node.setLabels([label.getName() for label in dlg.values])
 
                 # self.updateRunsGraph()
                 self.drawRunsGraph()
 
-    def _selectAncestors(self, childRun=None):
+    def _selectAncestors(self):
+        self._selectNodes(down=False)
+
+    def _selectDescendants(self):
+        self._selectNodes(down=True)
 
-        children = []
+    def _selectNodes(self, down=True, fromRun=None):
+        """ Selects all nodes in the specified direction, defaults to down."""
+        nodesToSelect = []
         # If parent param not passed...
-        if childRun is None:
+        if fromRun is None:
             # ..use selection, must be first call
             for protId in self._selection:
                 run = self.runsGraph.getNode(str(protId))
-                children.append(run)
+                nodesToSelect.append(run)
         else:
-            name = childRun.getName()
+            name = fromRun.getName()
 
             if not name.isdigit():
                 return
             else:
                 name = int(name)
 
             # If already selected (may be this should be centralized)
             if name not in self._selection:
-                children = (childRun,)
+                nodesToSelect = (fromRun,)
                 self._selection.append(name)
-        # Go up .
-        for run in children:
+
+        # Go in the direction .
+        for run in nodesToSelect:
+            # Choose the direction: down or up.
+            direction = run.getChilds if down else run.getParents
+
             # Select himself plus ancestors
-            for parent in run.getParents():
-                self._selectAncestors(parent)
+            for parent in direction():
+                self._selectNodes(down, parent)
+
         # Only update selection at the end, avoid recursion
-        if childRun is None:
+        if fromRun is None:
             self._lastSelectedProtId = None
             self._updateSelection()
             self.drawRunsGraph()
 
+
     def _exportProtocols(self, defaultPath=None, defaultBasename=None):
         protocols = self._getSelectedProtocols()
 
         def _export(obj):
             filename = os.path.join(browser.getCurrentDir(),
                                     browser.getEntryValue())
             try:
                 if (not os.path.exists(filename) or
                     self.windows.askYesNo("File already exists",
                                           "*%s* already exists, do you want "
                                           "to overwrite it?" % filename)):
                     self.project.exportProtocols(protocols, filename)
-                    self.windows.showInfo("Workflow successfully saved to '%s' "
+                    logger.info("Workflow successfully saved to '%s' "
                                           % filename)
                 else:  # try again
                     self._exportProtocols(defaultPath=browser.getCurrentDir(),
                                           defaultBasename=browser.getEntryValue())
             except Exception as ex:
                 import traceback
                 traceback.print_exc()
@@ -2116,15 +1905,19 @@
                                      parent=self.windows)
 
             if isinstance(firstViewer, ProtocolViewer):
                 firstViewer.visualize(prot, windows=self.windows)
             else:
                 firstViewer.visualize(prot)
         else:
+            outputList = []
             for _, output in prot.iterOutputAttributes():
+                outputList.append(output)
+
+            for output in outputList:
                 viewers = self.domain.findViewers(output.getClassName(), DESKTOP_TKINTER)
                 if len(viewers):
                     # Instantiate the first available viewer
                     # TODO: If there are more than one viewer we should display
                     # TODO: a selection menu
                     viewerclass = viewers[0]
                     firstViewer = viewerclass(project=self.project,
@@ -2191,81 +1984,121 @@
             kwargs['position'] = self._lastRightClickPos
 
         dlg = pwgui.dialog.EditObjectDialog(self.runsGraphCanvas, Message.TITLE_EDIT_OBJECT,
                                             prot, self.project.mapper, **kwargs)
         if dlg.resultYes():
             self._updateProtocol(prot)
 
-    def _runActionClicked(self, action):
-        prot = self.getSelectedProtocol()
-        if prot:
-            try:
-                if action == ACTION_DEFAULT:
-                    pass
-                elif action == ACTION_EDIT:
-                    self._openProtocolForm(prot)
-                elif action == ACTION_RENAME:
-                    self._renameProtocol(prot)
-                elif action == ACTION_COPY:
-                    self._copyProtocols()
-                elif action == ACTION_DELETE:
-                    self._deleteProtocol()
-                elif action == ACTION_STEPS:
-                    self._browseSteps()
-                elif action == ACTION_BROWSE:
-                    self._browseRunDirectory()
-                elif action == ACTION_DB:
-                    self._browseRunData()
-                elif action == ACTION_STOP:
-                    self._stopProtocol(prot)
-                elif action == ACTION_CONTINUE:
-                    self._continueProtocol(prot)
-                elif action == ACTION_RESULTS:
-                    self._analyzeResults(prot)
-                elif action == ACTION_EXPORT:
-                    self._exportProtocols(defaultPath=pwutils.getHomePath())
-                elif action == ACTION_EXPORT_UPLOAD:
-                    self._exportUploadProtocols()
-                elif action == ACTION_COLLAPSE:
-                    nodeInfo = self.settings.getNodeById(prot.getObjId())
-                    nodeInfo.setExpanded(False)
-                    self.updateRunsGraph(True, reorganize=True)
-                    self._updateActionToolbar()
-                elif action == ACTION_EXPAND:
-                    nodeInfo = self.settings.getNodeById(prot.getObjId())
-                    nodeInfo.setExpanded(True)
-                    self.updateRunsGraph(True, reorganize=True)
-                    self._updateActionToolbar()
-                elif action == ACTION_LABELS:
-                    self._selectLabels()
-                elif action == ACTION_SELECT_TO:
-                    self._selectAncestors()
-                elif action == ACTION_RESTART_WORKFLOW:
-                    self._launchWorkFlow(action)
-                elif action == ACTION_CONTINUE_WORKFLOW:
-                    self._launchWorkFlow(action)
-                elif action == ACTION_STOP_WORKFLOW:
-                    self._stopWorkFlow(action)
-                elif action == ACTION_RESET_WORKFLOW:
-                    self._resetWorkFlow(action)
+    def _runActionClicked(self, action, event=None):
 
-            except Exception as ex:
-                self.windows.showError(str(ex))
-                if Config.debugOn():
-                    import traceback
-                    traceback.print_exc()
+        if event is not None:
+            # log Search box events are reaching here
+            # Since this method is bound to the window events
+            if event.widget.widgetName == 'entry':
+                return
 
         # Following actions do not need a select run
         if action == ACTION_TREE:
-            self.updateRunsGraph(True, reorganize=True)
+            self.drawRunsGraph(reorganize=True)
         elif action == ACTION_REFRESH:
             self.refreshRuns(checkPids=True)
+        elif action == ACTION_PASTE:
+            self._pasteProtocolsFromClipboard()
 
         elif action == ACTION_SWITCH_VIEW:
             self.switchRunsView()
+        else:
+            prot = self.getSelectedProtocol()
+            if prot:
+                try:
+                    if action == ACTION_DEFAULT:
+                        pass
+                    elif action == ACTION_EDIT:
+                        self._editProtocol(prot)
+                    elif action == ACTION_RENAME:
+                        self._renameProtocol(prot)
+                    elif action == ACTION_DUPLICATE:
+                        self._copyProtocols()
+                    elif action == ACTION_COPY:
+                        self._copyProtocolsToClipboard()
+                    elif action == ACTION_DELETE:
+                        self._deleteProtocol()
+                    elif action == ACTION_STEPS:
+                        self._browseSteps()
+                    elif action == ACTION_BROWSE:
+                        self._browseRunDirectory()
+                    elif action == ACTION_DB:
+                        self._browseRunData()
+                    elif action == ACTION_STOP:
+                        self._stopProtocol(prot)
+                    elif action == ACTION_CONTINUE:
+                        self._continueProtocol(prot)
+                    elif action == ACTION_RESULTS:
+                        self._analyzeResults(prot)
+                    elif action == ACTION_EXPORT:
+                        self._exportProtocols(defaultPath=pwutils.getHomePath())
+                    elif action == ACTION_EXPORT_UPLOAD:
+                        self._exportUploadProtocols()
+                    elif action == ACTION_COLLAPSE:
+                        node = self.runsGraph.getNode(str(prot.getObjId()))
+                        nodeInfo = self.settings.getNodeById(prot.getObjId())
+                        nodeInfo.setExpanded(False)
+                        self.setVisibleNodes(node, visible=False)
+                        self.updateRunsGraph(True)
+                        self._updateActionToolbar()
+                    elif action == ACTION_EXPAND:
+                        node = self.runsGraph.getNode(str(prot.getObjId()))
+                        nodeInfo = self.settings.getNodeById(prot.getObjId())
+                        nodeInfo.setExpanded(True)
+                        self.setVisibleNodes(node, visible=True)
+                        self.updateRunsGraph(True)
+                        self._updateActionToolbar()
+                    elif action == ACTION_LABELS:
+                        self._selectLabels()
+                    elif action == ACTION_SELECT_FROM:
+                        self._selectDescendants()
+                    elif action == ACTION_SELECT_TO:
+                        self._selectAncestors()
+                    elif action == ACTION_RESTART_WORKFLOW:
+                        self._launchWorkFlow(action)
+                    elif action == ACTION_CONTINUE_WORKFLOW:
+                        self._launchWorkFlow(action)
+                    elif action == ACTION_STOP_WORKFLOW:
+                        self._stopWorkFlow(action)
+                    elif action == ACTION_RESET_WORKFLOW:
+                        self._resetWorkFlow(action)
+                    elif action == ACTION_SEARCH:
+                        self._searchProtocol()
+
+                except Exception as ex:
+                    self.windows.showError(str(ex))
+                    if Config.debugOn():
+                        import traceback
+                        traceback.print_exc()
+            else:
+                self.info("Action '%s' not implemented." % action)
+
+    def setVisibleNodes(self, node, visible=True):
+        hasParentHidden = False
+        for child in node.getChilds():
+            prot = child.run
+            nodeInfo = self.settings.getNodeById(prot.getObjId())
+            if visible:
+                hasParentHidden = self.hasParentHidden(child)
+            if not hasParentHidden:
+                nodeInfo.setVisible(visible)
+                self.setVisibleNodes(child, visible)
+
+    def hasParentHidden(self, node):
+        for parent in node.getParents():
+            prot = parent.run
+            nodeInfo = self.settings.getNodeById(prot.getObjId())
+            if not nodeInfo.isVisible() or not nodeInfo.isExpanded():
+                return True
+        return False
 
 
 class RunBox(pwgui.TextBox):
     """ Just override TextBox move method to keep track of 
     position changes in the graph.
     """
 
@@ -2279,459 +2112,7 @@
         self.nodeInfo.setPosition(self.x, self.y)
 
     def moveTo(self, x, y):
         pwgui.TextBox.moveTo(self, x, y)
         self.nodeInfo.setPosition(self.x, self.y)
 
 
-def inspectObj(obj, filename, prefix='', maxDeep=5, inspectDetail=2, memoryDict=None):
-    """ Creates a .CSV file in the filename path with
-        all its members and recursively with a certain maxDeep,
-        if maxDeep=0 means no maxDeep (until all members are inspected).
-        
-        inspectDetail can be:
-         - 1: All attributes are shown
-         - 2: All attributes are shown and iterable values are also inspected
-
-        prefix and memoryDict will be updated in the recursive entries:
-         - prefix is a compound of the two first columns (DEEP and Tree)
-         - memoryDict is a dictionary with the memory address and an identifier
-    """
-    END_LINE = '\n'  # end of line char
-    COL_DELIM = '\t'  # column delimiter
-    INDENT_COUNTER = '/'  # character append in each indention (it's not written)
-
-    NEW_CHILD = '  |------>  '  # new item indention
-    BAR_CHILD = '  | ' + INDENT_COUNTER  # bar indention
-    END_CHILD = ('       -- '+COL_DELIM)*4 + END_LINE  # Child ending
-    column1 = '    - Name - ' + COL_DELIM
-    column2 = '    - Type - ' + COL_DELIM
-    column3 = '    - Value - ' + COL_DELIM
-    column4 = '  - Memory Address -'
-
-    #  Constants to distinguish the first, last and middle rows
-    IS_FIRST = 1
-    IS_LAST = -1
-    IS_MIDDLE = 0
-
-    memoryDict = memoryDict or {}
-
-    def writeRow(name, value, prefix, posList=False):
-        """ Writes a row item. """
-        # we will avoid to recursively print the items wrote before 
-        #  (ie. with the same memory address), thus we store a dict with the
-        #  addresses and the flag isNew is properly set
-        if str(hex(id(value))) in memoryDict:
-            memorySTR = memoryDict[str(hex(id(value)))]
-            isNew = False
-        else:
-            # if the item is new, we save its memory address in the memoryDict
-            #   and we pass the name and the line on the file as a reference.
-            memorySTR = str(hex(id(value)))
-            file = open(filename, 'r')
-            lineNum = str(len(file.readlines())+1)
-            file.close()
-            nameDict = str(name)[0:15]+' ...' if len(str(name)) > 25 else str(name)
-            memoryDict[str(hex(id(value)))] = '>>> '+nameDict + ' - L:'+lineNum
-            isNew = True
-        
-        if posList:
-            # if we have a List, the third column is 'pos/lenght'
-            thirdCol = posList
-        else:
-            # else, we print the value avoiding the EndOfLine char (// instead)
-            thirdCol = str(value).replace(END_LINE, ' // ')
-
-        # we will print the indentation deep number in the first row
-        indentionDeep = prefix.count(INDENT_COUNTER)
-        deepStr = str(indentionDeep) + COL_DELIM
-
-        # the prefix without the indentCounters is 
-        #   the tree to be printed in the 2nd row
-        prefixToWrite = prefix.replace(INDENT_COUNTER, '')
-        
-        file = open(filename, 'a')   
-        file.write(deepStr + prefixToWrite + COL_DELIM +
-                   str(name) + COL_DELIM +
-                   str(type(value)) + COL_DELIM +
-                   thirdCol + COL_DELIM +
-                   memorySTR + END_LINE)
-        file.close()
-
-        return isNew
-
-    def recursivePrint(value, prefix, isFirstOrLast):
-        """ We print the childs items of tuples, lists, dicts and classes. """ 
-
-        # if it's the last item, its childs has not the bar indention
-        if isFirstOrLast == IS_LAST:  # void indention when no more items
-            prefixList = prefix.split(INDENT_COUNTER)
-            prefixList[-2] = prefixList[-2].replace('|', ' ')
-            prefix = INDENT_COUNTER.join(prefixList)
-
-        # recursive step with the new prefix and memory dict.
-        inspectObj(value, filename, prefix+BAR_CHILD, maxDeep, inspectDetail, 
-                   memoryDict)
-        
-        if isFirstOrLast == IS_FIRST:
-            deepStr = str(indentionDeep) + COL_DELIM
-        else:
-            # When it was not the first item, the deep is increased
-            #   to improve the readability when filter 
-            deepStr = str(indentionDeep+1) + COL_DELIM
-
-        prefix = prefix.replace(INDENT_COUNTER, '') + COL_DELIM
-
-        # We introduce the end of the child and 
-        #   also the next header while it is not the last
-        file = open(filename, 'a')
-        file.write(deepStr + prefix + END_CHILD)
-        if isFirstOrLast != IS_LAST:
-            # header
-            file.write(deepStr + prefix + 
-                       column1 + column2 + column3 + column4 + END_LINE)
-        file.close()
-
-    def isIterable(obj):
-        """ Returns true if obj is a tuple, list, dict or calls. """
-        isTupleListDict = (isinstance(obj, tuple) or
-                           isinstance(obj, dict) or
-                           isinstance(obj, list)) and len(value) > 1
-
-        # FIX ME: I don't know how to assert if is a class or not... 
-        isClass = str(type(obj))[1] == 'c'
-
-        return isClass or (isTupleListDict and inspectDetail < 2)
-
-    indentionDeep = prefix.count(INDENT_COUNTER)
-    if indentionDeep == 0:
-        prefix = ' - Root - '
-
-        # dict with name and value pairs of the members
-        if len(obj) == 1:
-            # if only one obj is passed in the input list,
-            #   we directly inspect that obj.
-            obj_dict = obj[0].__dict__
-            obj = obj[0]
-
-        #  setting the header row
-        treeHeader = ' - Print on ' + str(dt.datetime.now())
-        prefixHeader = '-DEEP-' + COL_DELIM + treeHeader + COL_DELIM
-        col1 = '    - Name - (value for Lists and Tuples)' + COL_DELIM
-        col3 = '    - Value - (Pos./Len for Lists and Tuples) ' + COL_DELIM
-
-        #  writing the header row
-        file = open(filename, 'w')
-        file.write(prefixHeader + col1 + column2 + col3 + column4 + END_LINE)
-        file.close()
-
-        #  writing the root object
-        writeRow(obj.__class__.__name__, obj, prefix)
-        #  adding the child bar to the prefix
-        prefix = '  ' + BAR_CHILD
-    else:
-        # firsts settings depending on the type of the obj
-        if str(type(obj))[1] == 'c':
-            obj_dict = obj.__dict__
-        elif (isinstance(obj, tuple) or
-              isinstance(obj, list)):
-            column1 = '    - Value - ' + COL_DELIM
-            column3 = '  - Pos./Len. - ' + COL_DELIM
-        elif isinstance(obj, dict):
-            column1 = '    - Key - ' + COL_DELIM
-            obj_dict = obj
-        else:  # if is not of the type above it not make sense to continue
-            return
-
-    indentionDeep = prefix.count(INDENT_COUNTER)
-    deepStr = str(indentionDeep) + COL_DELIM
-    isBelowMaxDeep = indentionDeep < maxDeep if maxDeep > 0 else True 
-
-    prefixToWrite = prefix.replace(INDENT_COUNTER, '') + COL_DELIM
-    file = open(filename, 'a')
-    file.write(deepStr + prefixToWrite + 
-               column1 + column2 + column3 + column4 + END_LINE)
-    file.close()
-
-    #  we update the prefix to put the NEW_CHILD string  ( |----> )
-    prefixList = prefix.split(INDENT_COUNTER)
-    prefixList[-2] = NEW_CHILD
-    #  we return to the string structure
-    #    with a certain indention if it's the root
-    prefixToWrite = '  ' + INDENT_COUNTER.join(prefixList) if indentionDeep == 1 \
-        else INDENT_COUNTER.join(prefixList)
-
-    isNew = True
-    if str(type(obj))[1] == 'c' or isinstance(obj, dict):
-        counter = 0
-        for key, value in obj_dict.items():
-            counter += 1
-            # write the variable
-            isNew = writeRow(key, value, prefixToWrite)
-
-            # managing the extremes of the loop
-            if counter == 1:
-                isFirstOrLast = IS_FIRST
-            elif counter == len(obj_dict):
-                isFirstOrLast = IS_LAST
-            else:
-                isFirstOrLast = IS_MIDDLE
-
-            # show attributes for objects and items for lists and tuples 
-            if isBelowMaxDeep and isNew and isIterable(value):
-                recursivePrint(value, prefix, isFirstOrLast)
-    else:
-        for i in range(0, len(obj)):
-            # write the variable
-            isNew = writeRow(obj[i], obj[i], prefixToWrite, 
-                             str(i+1)+'/'+str(len(obj)))
-
-            # managing the extremes of the loop
-            if i == 0:
-                isFirstOrLast = IS_FIRST
-            elif len(obj) == i+1:
-                isFirstOrLast = IS_LAST
-            else:
-                isFirstOrLast = IS_MIDDLE
-
-            # show attributes for objects and items for lists and tuples 
-            if isBelowMaxDeep and isNew and isIterable(obj[i]):
-                recursivePrint(obj[i], prefix, isFirstOrLast)
-
-
-class ProtocolTreeConfig:
-    """ Handler class that groups functions and constants
-    related to the protocols tree configuration.
-    """
-    ALL_PROTOCOLS = "All"
-    TAG_PROTOCOL_DISABLED = 'protocol-disabled'
-    TAG_PROTOCOL = 'protocol'
-    TAG_SECTION = 'section'
-    TAG_PROTOCOL_GROUP = 'protocol_group'
-    PLUGIN_CONFIG_PROTOCOLS = 'protocols.conf'
-
-    @classmethod
-    def getProtocolTag(cls, isInstalled):
-        """ Return the proper tag depending if the protocol is installed or not.
-        """
-        return cls.TAG_PROTOCOL if isInstalled else cls.TAG_PROTOCOL_DISABLED
-
-    @classmethod
-    def isAFinalProtocol(cls, v, k):
-        if (issubclass(v, ProtocolViewer) or
-                v.isBase() or v.isDisabled()):
-            return False
-
-        return v.__name__ == k
-
-    @classmethod
-    def __addToTree(cls, menu, item, checkFunction=None):
-        """ Helper function to recursively add items to a menu.
-        Add item (a dictionary that can contain more dictionaries) to menu
-        If check function is added will use it to check if the value must be added.
-        """
-        children = item.pop('children', [])
-
-        if checkFunction is not None:
-            add = checkFunction(item)
-            if not add:
-                return
-        subMenu = menu.addSubMenu(**item)  # we expect item={'text': ...}
-        for child in children:
-            cls.__addToTree(subMenu, child, checkFunction)  # add recursively to sub-menu
-
-        return subMenu
-
-    @classmethod
-    def __inSubMenu(cls, child, subMenu):
-        """
-        Return True if child belongs to subMenu
-        """
-        for ch in subMenu:
-            if child['tag'] == cls.TAG_PROTOCOL:
-                if not ch.value.empty() and ch.value == child['value']:
-                    return ch
-            elif ch.text == child['text']:
-                return ch
-        return None
-
-    @classmethod
-    def _orderSubMenu(cls, session):
-        """
-        Order all children of a given session:
-        The protocols first, then the sessions(the 'more' session at the end)
-        """
-        lengthSession = len(session.childs)
-        if lengthSession > 1:
-            childs = session.childs
-            lastChildPos = lengthSession - 1
-            if childs[lastChildPos].tag == cls.TAG_PROTOCOL:
-                for i in range(lastChildPos - 1, -1, -1):
-                    if childs[i].tag == cls.TAG_PROTOCOL:
-                        break
-                    else:
-                        tmp = childs[i + 1]
-                        childs[i + 1] = childs[i]
-                        childs[i] = tmp
-            else:
-                for i in range(lastChildPos - 1, -1, -1):
-                    if childs[i].tag == cls.TAG_PROTOCOL:
-                        break
-                    elif 'more' in str(childs[i].text).lower():
-                        tmp = childs[i + 1]
-                        childs[i + 1] = childs[i]
-                        childs[i] = tmp
-
-    @classmethod
-    def __findTreeLocation(cls, subMenu, children, parent):
-        """
-        Locate the protocol position in the given view
-        """
-        for child in children:
-            sm = cls.__inSubMenu(child, subMenu)
-            if sm is None:
-                cls.__addToTree(parent, child, cls.__checkItem)
-                cls._orderSubMenu(parent)
-            elif child['tag'] == cls.TAG_PROTOCOL_GROUP or child['tag'] == cls.TAG_SECTION:
-                cls.__findTreeLocation(sm.childs, child['children'], sm)
-
-    @classmethod
-    def __checkItem(cls, item):
-        """ Function to check if the protocol has to be added or not.
-        Params:
-            item: {"tag": "protocol", "value": "ProtImportMovies",
-                   "text": "import movies"}
-        """
-        if item["tag"] != cls.TAG_PROTOCOL:
-            return True
-
-        # It is a protocol as this point, get the class name and
-        # check if it is disabled
-        protClassName = item["value"]
-        protClass = Config.getDomain().getProtocols().get(protClassName)
-
-        return False if protClass is None else not protClass.isDisabled()
-
-    @classmethod
-    def __addAllProtocols(cls, domain, protocols):
-        # Add all protocols
-        allProts = domain.getProtocols()
-
-        # Sort the dictionary
-        allProtsSorted = OrderedDict(sorted(allProts.items(),
-                                            key=lambda e: e[1].getClassLabel()))
-        allProtMenu = ProtocolConfig(cls.ALL_PROTOCOLS)
-        packages = {}
-
-        # Group protocols by package name
-        for k, v in allProtsSorted.items():
-            if cls.isAFinalProtocol(v, k):
-                packageName = v.getClassPackageName()
-                # Get the package submenu
-                packageMenu = packages.get(packageName)
-
-                # If no package menu available
-                if packageMenu is None:
-                    # Add it to the menu ...
-                    packageLine = {"tag": "package", "value": packageName,
-                                   "text": packageName}
-                    packageMenu = cls.__addToTree(allProtMenu, packageLine)
-
-                    # Store it in the dict
-                    packages[packageName] = packageMenu
-
-                # Add the protocol
-                tag = cls.getProtocolTag(v.isInstalled())
-
-                protLine = {"tag": tag, "value": k,
-                            "text": v.getClassLabel(prependPackageName=False)}
-
-                # If it's a new protocol
-                if v.isNew() and v.isInstalled():
-                    # add the new icon
-                    protLine["icon"] = "newProt.gif"
-
-                cls.__addToTree(packageMenu, protLine)
-
-        protocols[cls.ALL_PROTOCOLS] = allProtMenu
-
-    @classmethod
-    def __addProtocolsFromConf(cls, protocols, protocolsConfPath):
-        """
-        Load the protocols in the tree from a given protocols.conf file,
-        either the global one in Scipion or defined in a plugin.
-        """
-        # Populate the protocols menu from the plugin config file.
-        if os.path.exists(protocolsConfPath):
-            cp = ConfigParser()
-            cp.optionxform = str  # keep case
-            cp.read(protocolsConfPath)
-            #  Ensure that the protocols section exists
-            if cp.has_section('PROTOCOLS'):
-                for menuName in cp.options('PROTOCOLS'):
-                    if menuName not in protocols:  # The view has not been inserted
-                        menu = ProtocolConfig(menuName)
-                        children = json.loads(cp.get('PROTOCOLS', menuName))
-                        for child in children:
-                            cls.__addToTree(menu, child, cls.__checkItem)
-                        protocols[menuName] = menu
-                    else:  # The view has been inserted
-                        menu = protocols.get(menuName)
-                        children = json.loads(cp.get('PROTOCOLS',
-                                                     menuName))
-                        cls.__findTreeLocation(menu.childs, children, menu)
-
-    @classmethod
-    def load(cls, domain, protocolsConf):
-        """ Read the protocol configuration from a .conf file similar to the
-        one in scipion/config/protocols.conf,
-        which is the default one when no file is passed.
-        """
-        protocols = OrderedDict()
-        # Read the protocols.conf from Scipion (base) and create an initial
-        # tree view
-        cls.__addProtocolsFromConf(protocols, protocolsConf)
-
-        # Read the protocols.conf of any installed plugin
-        pluginDict = domain.getPlugins()
-        pluginList = pluginDict.keys()
-        for pluginName in pluginList:
-            try:
-
-                # if the plugin has a path
-                if pwutils.isModuleAFolder(pluginName):
-                    # Locate the plugin protocols.conf file
-                    protocolsConfPath = os.path.join(
-                        pluginDict[pluginName].__path__[0],
-                        cls.PLUGIN_CONFIG_PROTOCOLS)
-                    cls.__addProtocolsFromConf(protocols, protocolsConfPath)
-
-            except Exception as e:
-                print('Failed to read settings. The reported error was:\n  %s\n'
-                      'To solve it, fix %s and run again.' % (
-                          e, os.path.abspath(protocolsConfPath)))
-
-            # Add all protocols to All view
-        cls.__addAllProtocols(Config.getDomain(), protocols)
-
-        return protocols
-
-
-class ProtocolConfig(MenuConfig):
-    """Store protocols configuration """
-
-    def __init__(self, text=None, value=None, **args):
-        MenuConfig.__init__(self, text, value, **args)
-        if 'openItem' not in args:
-            self.openItem.set(self.tag.get() != 'protocol_base')
-
-    def addSubMenu(self, text, value=None, shortCut=None, **args):
-        if 'icon' not in args:
-            tag = args.get('tag', None)
-            if tag == 'protocol':
-                args['icon'] = 'python_file.gif'
-            elif tag == 'protocol_base':
-                args['icon'] = 'class_obj.gif'
-
-        args['shortCut'] = shortCut
-        return MenuConfig.addSubMenu(self, text, value, **args)
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/text.py` & `scipion-pyworkflow-3.1.0/pyworkflow/utils/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -17,739 +17,866 @@
 # * You should have received a copy of the GNU General Public License
 # * along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-"""
-Text based widgets.
-"""
+import logging
+logger = logging.getLogger(__name__)
 
-
-import os
+import contextlib
 import sys
-import time
-import webbrowser
-import subprocess
-import tkinter.ttk as ttk
-import tkinter as tk
-import tkinter.messagebox as tkMessageBox
-
-import pyworkflow as pw
-from pyworkflow.utils import (HYPER_BOLD, HYPER_ITALIC, HYPER_LINK1, HYPER_LINK2,
-                              parseHyperText, renderLine, renderTextFile, colorName,
-                              which, envVarOn, expandPattern)
-from pyworkflow.utils.properties import Message, Color, Icon
-from . import gui
-from .widgets import Scrollable, IconButton
-from .tooltip import ToolTip
-
-
-# Define a function to open files cleanly in a system-dependent way
-if sys.platform.startswith('darwin'):  # macs use the "open" command
-    def _open_cmd(path, tkParent=None):
-        subprocess.Popen(['open', path])
-elif os.name == 'nt':  # there is a function os.startfile for windows
-    def _open_cmd(path, tkParent=None):
-        os.startfile(path)
-elif os.name == 'posix':  # linux systems and so on
-    def find_prog(*args):
-        """Return the first argument that is a program in PATH"""
-        for command in args:
-            if which(command):
-                return command
-        return None
+import os
+import re
+from datetime import datetime
+import traceback
+import sysconfig
 
-    x_open = find_prog('xdg-open', 'gnome-open', 'kde-open', 'gvfs-open')
-    editor = find_prog('pluma', 'gedit', 'kwrite', 'geany', 'kate',
-                       'emacs', 'nedit', 'mousepad', 'code')
-
-    def _open_cmd(path, tkParent=None):
-        # If it is an url, open with browser.
-        if path.startswith('http://') or path.startswith('https://') or path.endswith('.html'):
-            try:
-                webbrowser.open_new_tab(path)
-                return
-            except:
-                pass
-        # OK, it is a file. Check if it does exist
-        # and notify if it does not
-        if not os.path.isfile(path):
-            try:
-                # if tkRoot is null the error message may be behind
-                # other windows
-                tkMessageBox.showerror("File Error",  # bar title
-                                       "File not found\n(%s)" % path,  # message
-                                       parent=tkParent)
-                return
-            except:
-                return
-
-        if x_open:  # standard way to open
-            proc = subprocess.Popen([x_open, path])
-            time.sleep(1)
-            if proc.poll() in [None, 0]:
-                return  # yay! that's the way to do it!
-        if editor:  # last card: try to open it in an editor
-            proc = subprocess.Popen([editor, path])
-            time.sleep(1)
-            if proc.poll() in [None, 0]:
-                return  # hope we found your fav editor :)
-        print('WARNING: Cannot open %s' % path)  # nothing worked! :(
-else:
-    def _open_cmd(path, tkParent=None):
-        try:
-            tkMessageBox.showerror("Unknown System",  # bar title
-                                   'Unknown system, so cannot open %s' % path,  # message
-                                   parent=tkParent)
-            return
-        except:
-            pass
+import bibtexparser
+import numpy as np
+import math
+
+from pyworkflow import Config, StrColors
+
+
+def prettyDate(time=False):
+    """
+    Get a datetime object or a int() Epoch timestamp and return a
+    pretty string like 'an hour ago', 'Yesterday', '3 months ago',
+    'just now', etc
+    """
+    now = datetime.now()
+    if type(time) is int:
+        diff = now - datetime.fromtimestamp(time)
+    elif type(time) is float:
+        diff = now - datetime.fromtimestamp(int(time))
+    elif isinstance(time, datetime):
+        diff = now - time
+    elif not time:
+        # Avoid now - now (sonar cloud bug)
+        copy = now
+        diff = now - copy
+    second_diff = diff.seconds
+    day_diff = diff.days
+
+    if day_diff < 0:
+        return ''
+
+    if day_diff == 0:
+        if second_diff < 10:
+            return "just now"
+        if second_diff < 60:
+            return str(second_diff) + " seconds ago"
+        if second_diff < 120:
+            return "a minute ago"
+        if second_diff < 3600:
+            return str(int(second_diff / 60)) + " minutes ago"
+        if second_diff < 7200:
+            return "an hour ago"
+        if second_diff < 86400:
+            return str(int(second_diff / 3600)) + " hours ago"
+    if day_diff == 1:
+        return "Yesterday"
+    if day_diff < 7:
+        return str(day_diff) + " days ago"
+    if day_diff < 31:
+        return str(int(day_diff / 7)) + " weeks ago"
+    if day_diff < 365:
+        return str(int(day_diff / 30)) + " months ago"
+    return str(int(day_diff / 365)) + " years ago"
+
+
+def dateStr(dt=None, time=True, secs=False, dateFormat=None):
+    """ Get a normal string representation of datetime. 
+    If dt is None, use NOW.
+    """
+    if dt is None:
+        dt = datetime.now()
+    elif isinstance(dt, float) or isinstance(dt, int):
+        dt = datetime.fromtimestamp(dt)
+
+    if dateFormat is None:
+        dateFormat = '%d-%m-%Y'
+        if time:
+            dateFormat += ' %H:%M'
+            if secs:
+                dateFormat += ':%S'
+
+    return dt.strftime(dateFormat)
+
+
+prettyTime = dateStr
+
+
+def prettyTimestamp(dt=None, format='%Y-%m-%d_%H%M%S'):
+    if dt is None:
+        dt = datetime.now()
+
+    return dt.strftime(format)
+
+
+def prettySize(size):
+    """ Human friendly file size. """
+    unit_list = list(zip(['bytes', 'kB', 'MB', 'GB', 'TB', 'PB'],
+                         [0, 0, 1, 2, 2, 2]))
+    if size > 1:
+        exponent = min(int(math.log(size, 1024)), len(unit_list) - 1)
+        quotient = float(size) / 1024 ** exponent
+        unit, num_decimals = unit_list[exponent]
+        format_string = '{:.%sf} {}' % num_decimals
+        return format_string.format(quotient, unit)
+    if size == 0:
+        return '0 bytes'
+    if size == 1:
+        return '1 byte'
+
+
+def prettyDelta(timedelta):
+    """ Remove the milliseconds of the timedelta. """
+    return str(timedelta).split('.')[0]
+
+class UtcConverter:
+    """ Class to make date conversions to utc"""
+    utc_delta = datetime.utcnow() - datetime.now()
+
+    def __call__(cls, t):
+        return t + cls.utc_delta
+# Use to_utc like a function: to_utc(date)
+to_utc = UtcConverter()
+
+def prettyLog(msg):
+    logger.info(cyanStr(msg))
+
+
+class Timer(object):
+    """ Simple Timer base in datetime.now and timedelta. """
+
+    def __init__(self, message=""):
+        self._message = message
+
+    def tic(self):
+        self._dt = datetime.now()
+
+    def getElapsedTime(self):
+        return datetime.now() - self._dt
+
+    def toc(self, message='Elapsed:'):
+        logger.info(message + str(self.getElapsedTime()))
+
+    def getToc(self):
+        return prettyDelta(self.getElapsedTime())
+
+    def __enter__(self):
+        self.tic()
+
+    def __exit__(self, type, value, traceback):
+        self.toc(self._message)
+
+
+def timeit(func):
+    """
+    Decorator function to have a simple measurement of the execution time of a given function.
+    To use it ::
+
+        @timeit
+        def func(...)
+            ...
+
+    """
+
+    def timedFunc(*args, **kwargs):
+        t = Timer()
+        t.tic()
+        result = func(*args, **kwargs)
+        t.toc("Function '%s' took" % func)
+
+        return result
+
+    return timedFunc
+
+
+def trace(nlevels, separator=' --> ', stream=sys.stdout):
+    # Example:
+    #   @trace(3)
+    #   def doRefresh(...
+    # gives as output whenever doRefresh is called lines like:
+    #   text.py:486 _addFileTab --> text.py:330 __init__ --> doRefresh
+
+    def realTrace(f):
+        """ Decorator function to print stack call in a human-readable way.
+        """
+
+        def tracedFunc(*args, **kwargs):
+            stack = traceback.extract_stack()[-nlevels - 1:-1]
+            fmt = lambda x: '%s:%d %s' % (os.path.basename(x[0]), x[1], x[2])
+            stList = list(map(fmt, stack))
+            stream.write(separator.join(stList + [f.__name__]) + '\n')
+            return f(*args, **kwargs)
+
+        return tracedFunc
+
+    return realTrace
+
+
+def prettyDict(d):
+    print("{")
+    for k, v in d.items():
+        print("    %s: %s" % (k, v))
+    print("}")
+
+
+def prettyXml(elem, level=0):
+    """ Add indentation for XML elements for more human readable text. """
+    i = "\n" + level * "  "
+    if len(elem):
+        if not elem.text or not elem.text.strip():
+            elem.text = i + "  "
+        if not elem.tail or not elem.tail.strip():
+            elem.tail = i
+        for _elem in elem:
+            prettyXml(_elem, level + 1)
+        if not _elem.tail or not _elem.tail.strip():
+            _elem.tail = i
+
+
+def getUniqueItems(originalList):
+    """ Method to remove repeated items from one list 
+    originalList -- Original list with repeated items, or not.
+    returns -- New list with the content of original list without repeated items
+    """
+    auxDict = {}
+    resultList = [auxDict.setdefault(x, x) for x in originalList if x not in auxDict]
+    return resultList
+
+def sortListByList(inList, priorityList):
+    """ Returns a list sorted by some elements in a second priorityList"""
+    if priorityList:
+        sortedList = priorityList + [item for item in inList
+                                                     if item not in priorityList]
+        return sortedList
+    else:
+        return inList
+
+
+def executeRemoteX(command, hostName, userName, password):
+    """
+    Execute a remote command with X11 forwarding. Currently not used.
+
+    :param command: Command to execute.
+    :param hostName: Remote host name.
+    :param userName: User name.
+    :param password: Password.
+
+    :returns Tuple with standard output and error output.
+    """
+    scriptPath = os.path.abspath(os.path.join(os.path.dirname(__file__), "sshAskPass.sh"))
+    pswCommand = "echo '" + password + "' | " + scriptPath + " ssh -X " + userName + "@" + hostName + " " + command
+    import subprocess
+    p = subprocess.Popen(pswCommand, shell=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    stdout, stderr = p.communicate()
+    return stdout, stderr
+
+
+def executeRemote(command, hostName, userName, password):
+    """ Execute a remote command. Currently not used
+
+    :param command: Command to execute.
+    :param hostName: Remote host name.
+    :param userName: User name.
+    :param password: Password.
+
+    :returns Tuple with standard input, standard output and error output.
+    """
+    import paramiko
+    ssh = paramiko.SSHClient()
+    ssh.load_system_host_keys()
+    ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
+    ssh.connect(hostName, 22, userName, password)
+    stdin, stdout, stderr = ssh.exec_command(command)
+    ssh.close()
+    return stdin, stdout, stderr
+
+
+def executeLongRemote(command, hostName, userName, password):
+    """ Execute a remote command.
+
+    :param command: Command to execute.
+    :param hostName: Remote host name.
+    :param userName: User name.
+    :param password: Password.
+
+    :returns Tuple with standard input, standard output and error output.
+
+    """
+    import paramiko
+    import select
+    ssh = paramiko.SSHClient()
+    ssh.load_system_host_keys()
+    ssh.set_missing_host_key_policy(paramiko.AutoAddPolicy())
+    ssh.connect(hostName, 22, userName, password)
+    transport = ssh.get_transport()
+    channel = transport.open_session()
+    channel.exec_command(command)
+    while True:
+        if channel.exit_status_ready():
+            break
+        rl, wl, xl = select.select([channel], [], [], 0.0)
+        if len(rl) > 0:
+            print(channel.recv(1024))
+
+
+def getLocalUserName():
+    """ Recover local machine user name.
+    returns: Local machine user name.
+    """
+    import getpass
+    return getpass.getuser()
+
+
+def getLocalHostName():
+    return getHostName()
+
+
+def getHostName():
+    """ Return the name of the local machine. """
+    import socket
+    return socket.gethostname()
+
+
+def getHostFullName():
+    """ Return the fully-qualified name of the local machine. """
+    import socket
+    return socket.getfqdn()
+
+def getPython():
+    return sys.executable
+
+def getPythonPackagesFolder():
+    # This does not work on MAC virtual envs
+    # import site
+    # return site.getsitepackages()[0]
+
+    return sysconfig.get_path("platlib")
+
+
+# ******************************File utils *******************************
+
+def isInFile(text, filePath):
+    """
+    Checks if given text is in the given file.
+
+    :param text: Text to check.
+    :param filePath: File path to check.
+
+    :returns True if the given text is in the given file,
+        False if it is not in the file.
+
+    """
+    return any(text in line for line in open(filePath))
+
+
+def getLineInFile(text, fileName):
+    """ Find the line where the given text is located in the given file.
+
+    :param text: Text to check.
+    :param filePath: File path to check.
+
+    :return line number where the text was located.
+
+    """
+    with open(fileName) as f:
+        for i, line in enumerate(f):
+            if text in line:
+                return i + 1
+    return None
+
+def hasAnyFileChanged(files, time):
+    """ Returns true if any of the files in files list has been changed after 'time'"""
+    for file in files:
+        if hasFileChangedSince(file, time):
+            return True
+
+    return False
+
+def hasFileChangedSince(file, time):
+    """ Returns true if the file has changed after 'time'"""
+    modTime = datetime.datetime.fromtimestamp(getmtime(file))
+    return time < modTime
+
+
+# ------------- Colored message strings -----------------------------
+
+
+def getColorStr(text, color, bold=False):
+    """ Add ANSI color codes to the string if there is a terminal sys.stdout.
+
+    :param text: text to be colored
+    :param color: red or green
+    :param bold: bold the text
+    """
+    if not Config.colorsInTerminal():
+        return text
+
+    attr = [str(color.value)]
+
+    if bold:
+        attr.append('1')
+    return '\x1b[%sm%s\x1b[0m' % (';'.join(attr), text)
+
+
+def grayStr(text):
+    return getColorStr(text, color=StrColors.gray)
+
+
+def redStr(text):
+    return getColorStr(text, color=StrColors.red)
+
+
+def greenStr(text):
+    return getColorStr(text, color=StrColors.green)
+
+
+def yellowStr(text):
+    return getColorStr(text, color=StrColors.yellow)
+
+
+def blueStr(text):
+    return getColorStr(text, color=StrColors.blue)
+
+
+def magentaStr(text):
+    return getColorStr(text, color=StrColors.magenta)
+
+
+def cyanStr(text):
+    return getColorStr(text, color=StrColors.cyan)
 
 
-class HyperlinkManager:
-    """ Tkinter Text Widget Hyperlink Manager, taken from:
-    http://effbot.org/zone/tkinter-text-hyperlink.htm """
-    def __init__(self, text):
-        self.text = text
-        self.text.tag_config("hyper", foreground=Color.RED_COLOR, underline=1)
-        self.text.tag_bind("hyper", "<Enter>", self._enter)
-        self.text.tag_bind("hyper", "<Leave>", self._leave)
-        self.text.tag_bind("hyper", "<Button-1>", self._click)
-        self.reset()
-
-    def reset(self):
-        self.links = {}
-
-    def add(self, action):
-        # add an action to the manager.  returns tags to use in
-        # associated text widget
-        tag = "hyper-%d" % len(self.links)
-        self.links[tag] = action
-        return "hyper", tag
-
-    def _enter(self, event):
-        self.text.config(cursor="hand2")
-
-    def _leave(self, event):
-        self.text.config(cursor="")
-
-    def _click(self, event):
-        for tag in self.text.tag_names(tk.CURRENT):
-            if tag[:6] == "hyper-":
-                self.links[tag]()
-                return
-
-
-class Text(tk.Text, Scrollable):    
-    """ Base Text widget with some functionality
-    that will be used by children classes.
-    """
-    def __init__(self, master, **opts):
-        if 'handlers' in opts:
-            self.handlers = opts.pop('handlers')
+def ansi(n, bold=False):
+    """Return function that escapes text with ANSI color n."""
+    return lambda txt: '\x1b[%d%sm%s\x1b[0m' % (n, ';1' if bold else '', txt)
+
+
+black, red, green, yellow, blue, magenta, cyan, white = map(ansi, range(30, 38))
+blackB, redB, greenB, yellowB, blueB, magentaB, cyanB, whiteB = [
+    ansi(i, bold=True) for i in range(30, 38)]
+
+# -------------- Hyper text highlighting ----------------------------
+#
+# We use a subset of TWiki hyper text conventions.
+# In particular:
+#     *some_text* will display some_text in bold
+#     _some_text_ will display some_text in italic
+#     Links:
+#         http://www.link-page.com  -> hyperlink using the url as label
+#         [[http://www.link-page.com][Link page]] -> hyperlink using "Link page" as label
+
+# Types of recognized styles
+HYPER_BOLD = 'bold'
+HYPER_ITALIC = 'italic'
+HYPER_LINK1 = 'link1'
+HYPER_SCIPION_OPEN = 'sci-open'
+HYPER_LINK2 = 'link2'
+HYPER_ALL = 'all'
+
+# Associated regular expressions
+PATTERN_BOLD = "(^|[\s])[*](?P<bold>[^\s*][^*]*[^\s*]|[^\s*])[*]"
+# PATTERN_BOLD = r"[\s]+[*]([^\s][^*]+[^\s])[*][\s]+"
+PATTERN_ITALIC = "(^|[\s])[_](?P<italic>[^\s_][^_]*[^\s_]|[^\s_])[_]"
+# PATTERN_ITALIC = r"[\s]+[_]([^\s][^_]+[^\s])[_][\s]+"
+PATTERN_LINK1 = '(?P<link1>http[s]?://(?:[a-zA-Z]|[0-9]|[$-_@.&+#]|[!*\(\),]|(?:%[0-9a-fA-F][0-9a-fA-F]))+)'
+PATTERN_LINK2 = "[\[]{2}(?P<link2>[^\s][^\]]+[^\s])[\]][\[](?P<link2_label>[^\s][^\]]+[^\s])[\]]{2}"
+# __PATTERN_LINK2 should be first since it could contain __PATTERN_LINK1
+PATTERN_ALL = '|'.join([PATTERN_BOLD, PATTERN_ITALIC, PATTERN_LINK2, PATTERN_LINK1])
+
+# Compiled regex
+# Not need now, each pattern compiled separately
+# HYPER_REGEX = {
+#               HYPER_BOLD: re.compile(PATTERN_BOLD),
+#               HYPER_ITALIC: re.compile(PATTERN_ITALIC),
+#               HYPER_LINK1: re.compile(PATTERN_LINK1),
+#               HYPER_LINK2: re.compile(PATTERN_LINK1),
+#               }
+HYPER_ALL_RE = re.compile(PATTERN_ALL)
+
+
+def parseHyperText(text, matchCallback):
+    """ Parse the text recognizing Hyper definitions below.
+
+    :param matchCallback: a callback function to processing each matching,
+        it should accept the type of match (HYPER_BOLD, ITALIC or LINK)
+
+    :return The input text with the replacements made by matchCallback
+    """
+
+    def _match(match):
+        """ Call the proper matchCallback with some extra info. """
+        m = match.group().strip()
+        if m.startswith('*'):
+            tag = HYPER_BOLD
+        elif m.startswith('_'):
+            tag = HYPER_ITALIC
+        elif m.startswith('http'):
+            tag = HYPER_LINK1
+        elif m.startswith('[['):
+            tag = HYPER_LINK2
         else:
-            self.handlers = {}
-        opts['font'] = gui.fontNormal
-        defaults = self.getDefaults()
-        defaults.update(opts)
-        Scrollable.__init__(self, master, tk.Text, wrap=tk.WORD, **opts)
-        self._createWidgets(master, **defaults)
-        self.configureTags()
-
-    def _createWidgets(self, master, **opts):
-        """This is an internal function to create the Text, the Scrollbar and the Frame"""
-        
-        # create a popup menu
-        self.menu = tk.Menu(master, tearoff=0, postcommand=self.updateMenu)
-        self.menu.add_command(label="Copy to clipboard", command=self.copyToClipboard)
-        self.menu.add_command(label="Open path", command=self.openFile)
-        # Associate with right click
-        self.bind("<Button-1>", self.onClick)
-        self.bind("<Button-3>", self.onRightClick)
-        
-    def getDefaults(self):
-        """This should be implemented in subclasses to provide defaults"""
-        return {}
-    
-    def configureTags(self):
-        """This should be implemented to create specific tags"""
-        pass
-    
-    def addLine(self, line):
-        """Should be implemented to add a line """
-        self.insert(tk.END, line + '\n')
-        
-    def addNewline(self):
-        self.insert(tk.END, '\n')
-        
-    def goBegin(self):
-        self.see(0.0)
-        
-    def goEnd(self):
-        self.see(tk.END)
-        
-    def isAtEnd(self):
-        return self.scrollbar.get() == 1.0
-        
-    def clear(self):
-        self.delete(0.0, tk.END)
-
-    def getText(self):
-
-        textWithNewLine = self.get(0.0, tk.END)
-
-        # Remove the last new line
-        return textWithNewLine.rstrip('\n')
-
-    def setText(self, text):
-        """ Replace the current text with new one. """
-        self.clear()
-        self.addText(text)
-        
-    def addText(self, text):
-        """ Add some text to the current state. """
-        if isinstance(text, list):
-            for line in text:
-                self.addLine(line)
+            raise Exception("Bad prefix for HyperText match")
+        return matchCallback(match, tag)
+
+    return HYPER_ALL_RE.sub(_match, text)
+
+
+#    for hyperMode, hyperRegex in HYPER_REGEX.iteritems():
+#        text = hyperRegex.sub(lambda match: matchCallback(match, hyperMode), text)
+#
+#    return text
+
+class LazyDict(object):
+    """ Dictionary to be initialized in the moment it is accessed for the first time.
+    Initialization is done by a callback passed at instantiation"""
+    def __init__(self, callback=dict):
+        """ :param callback: method to initialize the dictionary. SHould return a dictionary"""
+        self.data = None
+        self.callback = callback
+
+    def evaluate_callback(self):
+        self.data = self.callback()
+
+    def __getitem__(self, name):
+        if self.data is None:
+            self.evaluate_callback()
+        return self.data.__getitem__(name)
+
+    def __setitem__(self, name, value):
+        if self.data is None:
+            self.evaluate_callback()
+        return self.data.__setitem__(name, value)
+
+    def __getattr__(self, name):
+        if self.data is None:
+            self.evaluate_callback()
+        return getattr(self.data, name)
+
+    def __iter__(self):
+        if self.data is None:
+            self.evaluate_callback()
+        return self.data.__iter__()
+
+
+def parseBibTex(bibtexStr):
+    """ Parse a bibtex file and return a dictionary. """
+
+    return bibtexparser.loads(bibtexStr).entries_dict
+
+
+
+def isPower2(num):
+    """ Return True if 'num' is a power of 2. """
+    return num != 0 and ((num & (num - 1)) == 0)
+
+
+# ---------------------------------------------------------------------------
+# Parsing of arguments
+# ---------------------------------------------------------------------------
+
+def getListFromRangeString(rangeStr):
+    """ Create a list of integers from a string with range definitions.
+    Examples:
+    "1,5-8,10" -> [1,5,6,7,8,10]
+    "2,6,9-11" -> [2,6,9,10,11]
+    "2 5, 6-8" -> [2,5,6,7,8]
+    """
+    # Split elements by command or space
+    elements = re.split(',|\s', rangeStr)
+    values = []
+    for e in elements:
+        if '-' in e:
+            limits = e.split('-')
+            values += range(int(limits[0]), int(limits[1]) + 1)
         else:
-            for line in text.splitlines():
-                self.addLine(line)
-        
-    def onClick(self, e=None): 
-        self.selection = None
-        self.selection_clear()
-        self.menu.unpost()
-        
-    def onRightClick(self, e):
-        try:
-            self.selection = self.selection_get().strip()
-            self.menu.post(e.x_root, e.y_root)    
-        except tk.TclError as e:
-            pass
-    
-    def copyToClipboard(self, e=None):
-        self.clipboard_clear()
-        self.clipboard_append(self.selection)
-
-    def openFile(self):
-        # What happens when you right-click and select "Open path"
-        self.openPath(self.selection)
-
-    def openPath(self, path):
-        """Try to open the selected path"""
-        path = expandPattern(path)
-
-        # If the path is a dir, open it with scipion browser dir <path>
-        if os.path.isdir(path):
-            dpath = (path if os.path.isabs(path)
-                     else os.path.join(os.getcwd(), path))
-            subprocess.Popen([pw.PYTHON, pw.getViewerScript(), dpath])
-            return
+            # If values are separated by comma also splitted 
+            values += map(int, e.split())
+    return values
+
 
-        # If it is a file, interpret it correctly and open it with DataView
-        dirname = os.path.dirname(path)
-        fname = os.path.basename(path)
-        if '@' in fname:
-            path = os.path.join(dirname, fname.split('@', 1)[-1])
+def getRangeStringFromList(list):
+    left = None
+    right = None
+    ranges = []
+
+    def addRange():
+        if left == right:  # Single element
+            ranges.append("%d" % right)
         else:
-            path = os.path.join(dirname, fname)
+            ranges.append("%(left)d-%(right)d" % locals())
 
-        if os.path.exists(path):
-            from pwem import emlib
-            fn = emlib.FileName(path)
-            if fn is not None and (fn.isImage() or fn.isMetaData()):
-                # fn is None if xmippLib is the xmippLib ghost library
-                from pwem.viewers import DataView
-                DataView(path).show()
-            else:
-                _open_cmd(path)
+    for item in list:
+        if right is None:
+            left = right = item
         else:
-            # This is probably one special reference, like sci-open:... that
-            # can be interpreted with our handlers.
-            tag = path.split(':', 1)[0] if ':' in path else None
-            if tag in self.handlers:
-                self.handlers[tag](path.split(':', 1)[-1])
+            if item == right + 1:
+                right += 1
             else:
-                print("Can't find %s" % path)
-
-    def updateMenu(self, e=None):
-        state = 'normal'
-        # if not xmippExists(self.selection):
-        #    state = 'disabled'#self.menu.entryconfig(1, background="green")
-        self.menu.entryconfig(1, state=state)
-        
-    def setReadOnly(self, value):
-        state = tk.NORMAL
-        if value:
-            state = tk.DISABLED
-        self.config(state=state) 
-        
-    def highlight(self, pattern, tag, start="1.0", end="end", regexp=False):
-        """ Apply the given tag to all text that matches the given pattern
-
-        If 'regexp' is set to True, pattern will be treated as a regular expression
-        Taken from: 
-            http://stackoverflow.com/questions/3781670/tkinter-text-highlighting-in-python
-        """
-        start = self.index(start)
-        end = self.index(end)
-        self.mark_set("matchStart", start)
-        self.mark_set("matchEnd", start)
-        self.mark_set("searchLimit", end)
-
-        count = tk.IntVar()
-        while True:
-            index = self.search(pattern, "matchEnd", "searchLimit",
-                                count=count, regexp=regexp)
-            if index == "":
-                break
-            self.mark_set("matchStart", index)
-            self.mark_set("matchEnd", "%s+%sc" % (index, count.get()))
-            self.tag_add(tag, "matchStart", "matchEnd")
+                addRange()
+                left = right = item
+    addRange()
+    return ','.join(ranges)
 
 
-def configureColorTags(text):
-    """ Create tags in text (of type tk.Text) for all the supported colors. """
-    try:
-        for color in colorName.values():
-            text.tag_config(color, foreground=color)
-        return True
-    except Exception as e:
-        print("Colors still not available (%s)" % e)
-        return False
+def getListFromValues(valuesStr, length=None, caster=str):
+    """ Convert a string representing list items into a list.
+    The items should be separated by spaces or commas and a multiplier 'x' can be used.
+    If length is not None, then the last element will be repeated
+    until the desired length is reached.
+
+    Examples:
+    '1 1 2x2 4 4' -> ['1', '1', '2', '2', '4', '4']
+    '2x3, 3x4, 1' -> ['3', '3', '4', '4', '4', '1']
 
-       
-class TaggedText(Text):  
     """
-    Implement a Text that will recognize some basic tags
-    *some_text* will display some_text in bold
-    _some_text_ will display some_text in italic
-    some_link or [[some_link][some_label]] will display some_link
-     as hyperlink or some_label as hyperlink to some_link
-    also colors are recognized if set option colors=True
-    """           
-    def __init__(self, master, colors=True, **opts):  
-        self.colors = colors
-        Text.__init__(self, master, **opts)
-        self.hm = HyperlinkManager(self)
-
-    def getDefaults(self):
-        return {'bg': "white", 'bd': 0}
-        # It used to have also 'font': gui.fontNormal  but that stops
-        # this file from running. Apparently there is no fontNormal in gui.
-
-    def configureTags(self):
-        self.tag_config('normal', justify=tk.LEFT, font=gui.fontNormal)
-        self.tag_config(HYPER_BOLD, justify=tk.LEFT, font=gui.fontBold)
-        self.tag_config(HYPER_ITALIC, justify=tk.LEFT, font=gui.fontItalic)
-        if self.colors:            
-            self.colors = configureColorTags(self)
-            # Color can be unavailable, so disable use of colors
-        
-    @staticmethod
-    def openLink(link):
-        webbrowser.open_new_tab(link)  # Open in the same browser, new tab
-
-    @staticmethod
-    def mailTo(email):
-        webbrowser.open("mailto:" + email)
-
-    def matchHyperText(self, match, tag):
-        """ Process when a match a found and store indexes inside string."""
-        self.insert(tk.END, self.line[self.lastIndex:match.start()])
-        g1 = match.group(tag)
-
-        if tag == HYPER_BOLD or tag == HYPER_ITALIC:
-            self.insert(tk.END, ' ' + g1, tag)
-        elif tag == HYPER_LINK1:
-            self.insert(tk.END, g1, self.hm.add(lambda: self.openLink(g1)))
-        elif tag == HYPER_LINK2:
-            label = match.group('link2_label')
-            if g1.startswith('http:'):
-                self.insert(tk.END, label, self.hm.add(lambda: self.openLink(g1)))
-            elif g1.startswith('mailto:'):
-                self.insert(tk.END, label, self.hm.add(lambda: self.mailTo(g1)))
-            else:
-                self.insert(tk.END, label, self.hm.add(lambda: self.openPath(g1)))
-        self.lastIndex = match.end()
-        
-        return g1
-
-    def addLine(self, line):
-        self.line = line
-        self.lastIndex = 0
-        if line is not None:
-            parseHyperText(line, self.matchHyperText)
-            Text.addLine(self, line[self.lastIndex:])
-
-
-class OutputText(Text):
-    """
-    Implement a Text that will show file content
-    and handle console metacharacter for colored output
-    """
-    def __init__(self, master, filename, colors=True, t_refresh=0, maxSize=400, **opts):
-        """ colors flag indicate if try to parse color meta-characters
-            t_refresh is the refresh time in seconds, 0 means no refresh
-        """
-        self.filename = filename
-        self.colors = colors
-        self.t_refresh = t_refresh
-        self.maxSize = maxSize
-
-        self.refreshAlarm = None  # Identifier returned by after()
-        self.lineNo = 0
-        self.offset = 0
-        self.lastLine = ''
-        Text.__init__(self, master, **opts)
-        self.hm = HyperlinkManager(self)
-        self.doRefresh()
-
-    def getDefaults(self):
-        return {'bg': "black", 'fg': 'white', 'bd': 0,
-                'height': 30,  'width': 100}
-        # It used to have also  'font': gui.fontNormal  but that stops this
-        # file from running. Apparently there is no fontNormal in gui.
-        
-    def configureTags(self):
-        if self.colors:
-            configureColorTags(self)
-
-    def _removeLastLine(self):
-        line = int(self.index(tk.END).split('.')[0])
-        if line > 0:
-            line -= 1
-            self.delete('%d.0' % line, tk.END)
-        
-    def addLine(self, line):
-        renderLine(line, self._addChunk, self.lineNo)
+    result = []
+    valuesStr = valuesStr.replace(","," ")
+    for chunk in valuesStr.split():
+        values = chunk.split('x')
+        n = len(values)
+        if n == 1:  # 'x' is not present in the chunk, single value
+            result += [caster(values[0])]
+        elif n == 2:  # multiple the values by the number after 'x'
+            result += [caster(values[1])] * int(values[0])
+        else:
+            raise Exception("More than one 'x' is not allowed in list string value.")
+
+    # If length is passed, we fill the list with 
+    # the last element until length is reached
+    if length is not None and length > len(result):
+        item = result[-1]
+        result += [caster(item)] * (length - len(result))
+
+    return result
+
+
+def getFloatListFromValues(valuesStr, length=None):
+    """ Convert a string to a list of floats"""
+    return [float(v) for v in getListFromValues(valuesStr, length)]
+
+
+def getBoolListFromValues(valuesStr, length=None):
+    """ Convert a string to a list of booleans"""
+    from pyworkflow.object import Boolean
+    return [Boolean(value=v).get() for v in getListFromValues(valuesStr, length)]
 
-    def _addChunk(self, txt, fmt=None):
+
+def getStringListFromValues(valuesStr, length=None):
+    """ Convert a string to a list of booleans"""
+    from pyworkflow.object import String
+    return [String(value=v).get() for v in getListFromValues(valuesStr, length)]
+
+
+class Environ(dict):
+    """ Some utilities to handle environment settings. """
+    REPLACE = 0
+    BEGIN = 1
+    END = 2
+
+    def getFirst(self, keys, mandatory=False):
+        """ Return the value of the first key present in the environment.
+        If none is found, returns the 'defaultValue' parameter.
         """
-        Add text txt to the widget, with format fmt.
-        fmt can be a color (like 'red') or a link that looks like 'link:url'.
+        for k in keys:
+            if k in self:
+                return self.get(k)
+
+        if mandatory:
+            logger.info("None of the variables: %s found in the Environment. "
+                  "Please check scipion.conf files." % (str(keys)))
+
+        return None
+
+    def set(self, varName, varValue, position=REPLACE):
+        """ Modify the value for some variable.
+
+        :param varName: for example LD_LIBRARY_PATH
+        :param varValue: the value to set, prefix or suffix.
+        :param position: controls how the value will be changed.
+            If REPLACE, it will overwrite the value of
+            the var. BEGIN or END will preserve the current value
+            and will add, at the beginning or end, the new value.
+
         """
-        if self.colors and fmt is not None:
-            if fmt.startswith('link:'):
-                fname = fmt.split(':', 1)[-1]
-                self.insert(tk.END, txt, self.hm.add(lambda: openTextFileEditor(fname)))
-            else:
-                self.insert(tk.END, txt, fmt)
+        if varName in self and position != self.REPLACE:
+            if position == self.BEGIN:
+                self[varName] = varValue + os.pathsep + self[varName]
+            elif position == self.END:
+                self[varName] = self[varName] + os.pathsep + varValue
         else:
-            self.insert(tk.END, txt)
+            self[varName] = varValue
+
+    def update(self, valuesDict, position=REPLACE):
+        """ Use set for each key, value pair in valuesDict. """
+        for k, v in valuesDict.items():
+            self.set(k, v, position)
+
+    def addLibrary(self, libraryPath, position=BEGIN):
+        """ Adds a path to LD_LIBRARY_PATH at the requested position
+        if the provided paths exist. """
+
+        if libraryPath is None:
+            return
 
-    def _notifyLine(self, line):
-        if '\r' in self.lastLine and '\r' in line:
-            self._removeLastLine()
-            self.addNewline()
-            
-        self.lastLine = line        
-        
-    def readFile(self, clear=False):
-        self.setReadOnly(False)
-        
-        if clear:
-            self.offset = 0
-            self.lineNo = 0
-            self.clear()
-
-        if os.path.exists(self.filename):
-            self.offset, self.lineNo = renderTextFile(self.filename, 
-                                                      self._addChunk,
-                                                      offset=self.offset, 
-                                                      lineNo=self.lineNo,
-                                                      maxSize=self.maxSize, 
-                                                      notifyLine=self._notifyLine)
+        if existsVariablePaths(libraryPath):
+            self.update({'LD_LIBRARY_PATH': libraryPath}, position=position)
         else:
-            self.insert(tk.END, "File '%s' doesn't exist" % self.filename)
+            logger.info("Some paths do not exist in: % s" % libraryPath)
 
-        self.setReadOnly(True)
-        # self.goEnd()
-      
-    def doRefresh(self):
-        # First stop pending refreshes
-        if self.refreshAlarm:
-            self.after_cancel(self.refreshAlarm)
-            self.refreshAlarm = None
-
-        self.readFile()
-
-        if self.t_refresh > 0:
-            self.refreshAlarm = self.after(self.t_refresh*1000, self.doRefresh)
-
-
-class TextFileViewer(tk.Frame):
-    """ Implementation of a simple text file viewer """
-    
-    LabelBgColor = "white"
-    
-    def __init__(self, master, fileList=[],
-                 allowSearch=True, allowRefresh=True, allowOpen=False,
-                 font=None, maxSize=400, width=100, height=30):
-        tk.Frame.__init__(self, master)
-        self.searchList = None
-        self.lastSearch = None
-        self.refreshAlarm = None
-        self._lastTabIndex = None
-        self.fileList = []  # Files being visualized
-        self.taList = []  # Text areas (OutputText, a scrollable TkText)
-        self.fontDict = {}
-        self._allowSearch = allowSearch
-        self._allowRefresh = allowRefresh
-        self._allowOpen = allowOpen
-        self._font = font  # allow a font to be passed as argument to be used
-        self.maxSize = maxSize
-        self.width = width
-        self.height = height
-
-        self.createWidgets(fileList)
-        self.master = master
-        self.addBinding()
-        
-    def addFile(self, filename):
-        self.fileList.append(filename)
-        self._addFileTab(filename)
-        
-    def clear(self):
-        """ Remove all added files. """
-        self.fileList = []
-        for _ in self.taList:
-            self.notebook.forget(0)       
-        self.taList = []
-        self._lastTabIndex = None
-        
-    def _addFileTab(self, filename):
-        tab = tk.Frame(self.notebook)
-        tab.rowconfigure(0, weight=1)
-        tab.columnconfigure(0, weight=1)
-        kwargs = {'bg': 'black',
-                  'fg': 'white'}
-        
-        if self._font is not None:
-            kwargs['font'] = self._font
-
-        t = OutputText(tab, filename, width=self.width, height=self.height,
-                       maxSize=self.maxSize, **kwargs)
-        t.frame.grid(column=0, row=0, padx=5, pady=5, sticky='nsew')
-        self.taList.append(t)
-        tabText = "   %s   " % os.path.basename(filename)
-        self.notebook.add(tab, text=tabText)        
-    
-    def createWidgets(self, fileList):
-        # registerCommonFonts()
-        self.columnconfigure(0, weight=1)
-        self.rowconfigure(1, weight=1)        
-
-        # Create toolbar frame
-        toolbarFrame = tk.Frame(self)
-        toolbarFrame.grid(column=0, row=0, padx=5, sticky='new')
-        gui.configureWeigths(toolbarFrame)
-        # Add the search box
-        right = tk.Frame(toolbarFrame)
-        right.grid(column=1, row=0, sticky='ne')        
-        self.searchVar = tk.StringVar()
-        if self._allowSearch:
-            tk.Label(right, text='Search:').grid(row=0, column=3, padx=5)
-            self.searchEntry = tk.Entry(right, textvariable=self.searchVar,
-                                        font=self._font)
-            self.searchEntry.grid(row=0, column=4, sticky='ew', padx=5)
-            self.searchEntry.bind('<Return>', self.findText)
-            self.searchEntry.bind('<KP_Enter>', self.findText)
-            # btn = IconButton(right, "Search", Icon.ACTION_SEARCH,
-            #                  tooltip=Message.TOOLTIP_SEARCH,
-            #                  command=self.findText, bg=None)
-            # btn.grid(row=0, column=5, padx=(0, 5))
-
-            btn = IconButton(right, "Next", Icon.ACTION_FIND_NEXT,
-                             tooltip=Message.TOOLTIP_SEARCH_NEXT,
-                             command=self.findText, bg=None)
-            btn.grid(row=0, column=5, padx=(0, 5))
-
-            btn = IconButton(right, "Previous", Icon.ACTION_FIND_PREVIOUS,
-                             tooltip=Message.TOOLTIP_SEARCH_PREVIOUS,
-                             command=self.findPrevText, bg=None)
-            btn.grid(row=0, column=6, padx=(0, 5))
-
-        if self._allowRefresh:
-            btn = IconButton(right, "Refresh", Icon.ACTION_REFRESH,
-                             tooltip=Message.TOOLTIP_REFRESH,
-                             command=self._onRefresh, bg=None)
-            btn.grid(row=0, column=7, padx=(0, 5), pady=2)
-        if self._allowOpen:
-            btn = IconButton(right, "Open external", Icon.ACTION_REFERENCES,
-                             tooltip=Message.TOOLTIP_EXTERNAL,
-                             command=self._openExternal, bg=None)
-            btn.grid(row=0, column=8, padx=(0, 5), pady=2)
-
-        # Create tabs frame
-        tabsFrame = tk.Frame(self)
-        tabsFrame.grid(column=0, row=1, padx=5, pady=(0, 5), sticky="nsew")
-        tabsFrame.columnconfigure(0, weight=1)
-        tabsFrame.rowconfigure(0, weight=1)
-        self.notebook = ttk.Notebook(tabsFrame)  
-        self.notebook.rowconfigure(0, weight=1)
-        self.notebook.columnconfigure(0, weight=1)      
-        for f in fileList:
-            self._addFileTab(f)
-        self.notebook.grid(column=0, row=0, sticky='nsew', padx=5, pady=5)   
-        self.notebook.bind('<<NotebookTabChanged>>', self._tabChanged)
-
-    def _tabChanged(self, e=None):
-        self._lastTabIndex = self.notebook.select()
-        # reset the search
-        self.lastSearch = None
-        self.searchEntry.focus_set()
-
-    def addBinding(self):
-
-        shortcutDefinitions = [(lambda e: self.findText(), "Trigger the search", ['<Return>']),
-                               (lambda e: self.findText(), "Trigger the search", ['<KP_Enter>']),
-                               (lambda e: self.findText(matchCase=True), "Trigger a case sensitive search", ['<Shift-Return>']),
-                               (lambda e: self.findText(), "Move to the next highlighted item", ["<Down>", '<F3>']),
-                               (lambda e: self.findText(-1), "Move to the previous highlighted item", ["<Up>", '<Shift-F3>']),
-                               ]
-        tooltip = "Shortcuts:"
-
-        for callback, help, keys in shortcutDefinitions:
-            tooltip += "\n" + help + ": "
-            for key in keys:
-                self.searchEntry.bind(key, callback)
-                tooltip += key
-
-        # Add a tooltip
-        ToolTip(self.searchEntry, tooltip, 800)
-
-    def getIndex(self):
-        """ Return the index of the selected tab. """
-        selected = self.notebook.select()
-        if selected:
-            return self.notebook.index(selected)
-        return -1
-    
-    def setIndex(self, index):
-        """ Select the tab with the given index. """
-        if index != -1:
-            self.notebook.select(self.notebook.tabs()[index])
-    
-    def selectedText(self):
-        index = self.getIndex()
-        if index != -1:
-            return self.taList[index]
-        return None
-    
-    def changeFont(self, event=""):
-        for font in self.fontDict.values():
-            gui.changeFontSize(font, event)
-              
-    def refreshAll(self, clear=False, goEnd=False):
-        """ Refresh all output textareas. """
-        for ta in self.taList:
-            ta.readFile(clear)
-            if goEnd:
-                ta.goEnd()
-        if self._lastTabIndex is not None:
-            self.notebook.select(self._lastTabIndex)
-            
-    def _onRefresh(self, e=None):
-        """ Action triggered when the 'Refresh' icon is clicked. """
-        self.refreshAll(clear=False, goEnd=True)
-        
-    def refreshOutput(self, e=None):
-        if self.refreshAlarm:
-            self.after_cancel(self.refreshAlarm)
-            self.refreshAlarm = None
-        text = self.selectedText()
-        if text:
-            text.readFile()
-        
-    def changePosition(self, index):
-        self.selectedText().see(index)
-
-    def findPrevText(self):
-        self.findText(-1)
-
-    def findText(self, direction=1, matchCase=0):
-        text = self.selectedText()
-        str = self.searchVar.get()
-        if text:
-            if str is None or str != self.lastSearch:
-                self.buildSearchList(text, str, matchCase=matchCase)
-                self.lastSearch = str
+    def setPrepend(self, prepend):
+        """ Use this method to set a prepend string that will be added at
+        the beginning of any command that will be run in this environment.
+        This can be useful for example when 'modules' need to be loaded and
+        a simple environment variables setup is not enough.
+        """
+        setattr(self, '__prepend', prepend)
 
-            else:
-                self.nextSearchIndex(text, direction)
-            self.searchEntry.focus_set()
-        
-    def buildSearchList(self, text, str, matchCase=0):
-        text.tag_remove('found', '1.0', tk.END)
-        list = []
-        if str:
-            idx = '1.0'
-            while True:
-                idx = text.search(str, idx, nocase=not matchCase, stopindex=tk.END)
-                if not idx:
-                    break
-                lastidx = '%s+%dc' % (idx, len(str))
-                text.tag_add('found', idx, lastidx)
-                list.append((idx, lastidx))
-                idx = lastidx
-        text.tag_config('found', foreground='white', background='blue')
-        # Set class variables
-        self.searchList = list
-        self.currentIndex = -1
-        self.nextSearchIndex(text)  # select first element
-    
-    def nextSearchIndex(self, text, direction=1):
-        # use direction=-1 to go backward
-        text.tag_remove('found_current', '1.0', tk.END)
-        if len(self.searchList) == 0:
-            return
-        self.currentIndex = (self.currentIndex + direction) % len(self.searchList)
-        idx, lastidx = self.searchList[self.currentIndex]
-        text.tag_config('found_current', foreground='yellow', background='red')
-        text.tag_add('found_current', idx, lastidx)
-        text.see(idx)
-        
-    def _openExternal(self):
-        """ Open a new window with an external viewer. """
-        if envVarOn('SCIPION_EXTERNAL_VIEWER'):
-            if not self.taList:
-                return
-            openTextFileEditor(self.taList[max(self.getIndex(), 0)].filename)
+    def getPrepend(self):
+        """ Return if there is any prepend value. See setPrepend function. """
+        return getattr(self, '__prepend', '')
+
+
+def existsVariablePaths(variableValue):
+    """ Check if the path (or paths) in variableValue exists.
+    Multiple paths are allowed if separated by os."""
+    return all(os.path.exists(p)
+               for p in variableValue.split(os.pathsep) if p.split())
+
+
+def environAdd(varName, newValue, valueFirst=False):
+    """ Add a new value to some environ variable.
+    If valueFirst is true, the new value will be at the beginning.
+    """
+    varList = [os.environ[varName]]
+    i = 1
+    if valueFirst:
+        i = 0
+    varList.insert(i, newValue)
+    os.environ[varName] = os.pathsep.join(varList)
+
+
+def envVarOn(varName, env=None):
+    """ Is variable set to True in the environment? """
+    v = env.get(varName) if env else os.environ.get(varName)
+    return strToBoolean(v)
+
+def strToBoolean(string):
+    """ Converts a string into a Boolean if the string is on of true, yes, on, 1. Case insensitive."""
+    return string is not None and string.lower() in ['true', 'yes', 'on', '1']
+
+
+def getMemoryAvailable():
+    """ Return the total memory of the system in MB """
+    from psutil import virtual_memory
+    return virtual_memory().total // 1024 ** 2
+
+
+def getFreePort(basePort=0, host=''):
+    import socket
+    try:
+        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        s.bind((host, basePort))
+        ipaddr, port = s.getsockname()
+        s.close()
+    except Exception as e:
+        logger.error("Can't get a free port", exc_info=e)
+        return 0
+    return port
+
+
+def readProperties(propsFile):
+    myprops = {}
+    with open(propsFile, 'r') as f:
+        for line in f:
+            line = line.rstrip()  # removes trailing whitespace and '\n' chars
+
+            if "=" not in line:
+                continue  # skips blanks and comments w/o =
+            if line.startswith("#"):
+                continue  # skips comments which contain =
+
+            k, v = line.split("=", 1)
+            myprops[k] = v
+    return myprops
+
+
+# ---------------------Color utils --------------------------
+def hex_to_rgb(value):
+    value = value.lstrip('#')
+    lv = len(value)
+    return tuple(int(value[i:i + lv // 3], 16) for i in range(0, lv, lv // 3))
+
+
+def rgb_to_hex(rgb):
+    return '#%02x%02x%02x' % (int(rgb[0]), int(rgb[1]), int(rgb[2]))
+
+
+def lighter(color, percent):
+    """assumes color is rgb between (0, 0, 0) and (255, 255, 255)"""
+    color = np.array(color)
+    white = np.array([255, 255, 255])
+    vector = white - color
+    return tuple(np.around(color + vector * percent))
+
+
+def formatExceptionInfo(level=6):
+    error_type, error_value, trbk = sys.exc_info()
+    tb_list = traceback.format_tb(trbk, level)
+    s = "Error: %s \nDescription: %s \nTraceback:" % (error_type.__name__,
+                                                      error_value)
+    for i in tb_list:
+        s += "\n" + i
+    return s
+
+
+def printTraceBack():
+    traceback.print_stack()
+
+
+def getEnvVariable(variableName, default=None, exceptionMsg=None):
+    """ Returns the value of an environment variable or raise an exception message.
+    Useful when adding variable to the config file and report accurate messages"""
+    value = os.getenv(variableName)
+
+    if exceptionMsg is None:
+        exceptionMsg = ("Environment variable %s not found. "
+                        "Please check scipion configuration. "
+                        "Try running : scipion config." % variableName)
+
+    if value is None:
+        if default is None:
+            raise Exception(exceptionMsg)
         else:
-            showTextFileViewer("File viewer", self.fileList, self.windows)
-  
-  
-def openTextFile(filename):
-    """ Open a text file with an external or default viewer. """
-    if envVarOn('SCIPION_EXTERNAL_VIEWER'):
-        openTextFileEditor(filename)
+            return default
     else:
-        showTextFileViewer("File viewer", [filename])    
-    
-    
-def openTextFileEditor(filename, tkParent=None):
+        return value
+
+
+@contextlib.contextmanager
+def weakImport(package):
+    """
+    This method can be used to tolerate imports that may fail.
+
+    e.g::
+
+        from .protocol_ctffind import CistemProtCTFFind
+        with weakImport('tomo'):
+            from .protocol_ts_ctffind import CistemProtTsCtffind
+
+    In this case CistemProtTsCtffind should fail if tomo package is missing,
+    but exception is captured and all the imports above should be available
+
+    :param package: name of the package that is expected to fail
+
+    """
     try:
-        _open_cmd(filename, tkParent)
-    except:
-        showTextFileViewer("File viewer", [filename])
-    
-    
-def showTextFileViewer(title, filelist, parent=None, main=False):
-    w = gui.Window(title, parent, minsize=(600, 400))
-    viewer = TextFileViewer(w.root, filelist, maxSize=-1, font=w.font)
-    viewer.grid(row=0, column=0, sticky='news')
-    gui.configureWeigths(w.root)
-    w.show()
-
-
-if __name__ == '__main__':
-    root = tk.Tk()
-    root.withdraw()
-    root.title("View files")
-    l = TextFileViewer(root, fileList=sys.argv[1:])
-    l.pack(side=tk.TOP, fill=tk.BOTH)
-    gui.centerWindows(root)
-    root.deiconify()
-    root.mainloop()
+        yield
+    except ImportError as e:
+        if "'%s'" % package not in str(e):
+            raise e
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/tooltip.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/tooltip.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/tree.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 # **************************************************************************
 
 
 import os
 import tkinter as tk
 import tkinter.ttk as ttk
 
-from pyworkflow.object import Scalar
 from pyworkflow.mapper import SqliteMapper
 from pyworkflow.utils import prettyDelta
 from . import gui
 from .widgets import Scrollable
 
 FIRST_TREE_COLUMN = '#0'
 
@@ -279,14 +278,15 @@
         self.heading(FIRST_TREE_COLUMN, text=cols[0][0],
                      command=lambda: self.sortTree(FIRST_TREE_COLUMN, cols[0][0]))
         self.column(FIRST_TREE_COLUMN, width=cols[0][1])
         # Set other columns
         for c, w in cols[1:]:
             self.column(c, width=w)
             self.heading(c, text=c, command=lambda _c=c: self.sortTree(_c, _c))
+
         self.grid(row=0, column=0, sticky='news')
 
         self.menu = tk.Menu(self, tearoff=0)
 
         self.setProvider(provider)
 
         self.bind("<Button-3>", self._onRightClick)
@@ -401,15 +401,15 @@
                         self.itemConfig(obj, open=True)
 
                     if objDict.get('selected', False):
                         self.selectChild(obj._treeId)
 
                 except Exception as ex:
                     print("error: ", ex)
-                    if obj.getObjId():
+                    if hasattr(obj, "getObjId") and obj.getObjId():
                         print("error object with id=%d (%s) is duplicated!!!"
                               % (obj.getObjId(), str(obj)))
                     else:
                         print("error, object %s does not have an id. This could"
                               " be due to the load of old project that does not"
                               " have recently added attributes "
                               "(e.g.:datastreaming)" % str(obj))
@@ -494,16 +494,17 @@
                 t += " = None"
         else:
             t += " = %s" % str(obj)
 
         info = {'key': obj.getObjId(),
                 'parent': self._parentDict.get(obj.getObjId(), None),
                 'text': t, 'values': (obj.strId(), cls)}
-        if issubclass(obj.__class__, Scalar):
-            info['image'] = 'step.gif'
+        # This image step.gif is missing, I guess we are not showing Scalars
+        # if issubclass(obj.__class__, Scalar):
+        #     info['image'] = 'step.gif'
 
         return info
 
     def getObjectPreview(self, obj):
         return None, None
 
     def getObjectActions(self, obj):
@@ -647,7 +648,35 @@
         return info
 
     def getText(self, obj):
         return obj.pluginName + '-' + obj.templateName
 
     def getValues(self, obj):
         return (obj.description,)
+
+class AttributesTreeProvider(ListTreeProviderString):
+    def __init__(self, item):
+        TreeProvider.__init__(self)
+        self.objList = self._attributesToObjectList(item)
+        self.getColumns = lambda: [('attribute', 250),
+                                   ('value', 125)]
+        self.getObjects = lambda: self.objList
+
+    def _attributesToObjectList(self, item):
+        """ Returns a list of all available attributes ready as a list of objects for the tree"""
+        objList = []
+
+        for key, attr in item.getAttributesToStore():
+            clone = attr.clone()
+            clone.attrName = key
+            objList.append(clone)
+        return objList
+
+    def getObjectInfo(self, obj):
+        info = {'key': obj.attrName, 'text': self.getText(obj), 'values': self.getValues(obj)}
+        return info
+
+    def getText(self, obj):
+        return obj.attrName
+
+    def getValues(self, obj):
+        return (obj.get(),)
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/gui/widgets.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,17 @@
 """
 
 import tkinter as tk
 import tkinter.ttk as ttk
 
 from math import ceil
 
-from pyworkflow import TK_GRAY_DEFAULT
+import pyworkflow
+from pyworkflow import TK_GRAY_DEFAULT, Config
+
 from . import gui
 from .tooltip import ToolTip
 
 
 class Button(tk.Button):
     _images = {}
 
@@ -81,15 +83,15 @@
         Button.__init__(self, master, text, imagePath, tooltip, **defaults)
 
 
 class IconButton(HotButton):
     """ Hot button, but only with image and no border """
 
     def __init__(self, master, text, imagePath, tooltip=None, **opts):
-        defaults = {'bd': 0, 'bg': 'white', 'compound': tk.NONE}
+        defaults = {'bd': 0, 'bg': Config.SCIPION_BG_COLOR, 'compound': tk.NONE}
         defaults.update(opts)
         HotButton.__init__(self, master, text, imagePath, tooltip, **defaults)
 
 
 class AutoScrollbar(tk.Scrollbar):
     """"A scrollbar that hides itself if it's not needed."""
 
@@ -126,31 +128,46 @@
             self.grid_remove = self.frame.grid_remove
         else:
             WidgetClass.__init__(self, master, **opts)
 
         # Bind ourselves
         self.bindWidget(self)
 
+
     def scroll(self, event):
-        # print "scrolling, event.num", event.num, "delta", event.delta
+        print("Deprecated, use scrollV")
+        self.scrollV(event)
+
+    def scrollV(self, event):
+        self._basescroll(event, self.yview)
+
+    def scrollH(self, event):
+        self._basescroll(event, self.xview)
+
+    def _basescroll(self, event, view):
+
         if event.num == 5 or event.delta < 0:
             count = 1
         if event.num == 4 or event.delta > 0:
             count = -1
-        self.yview("scroll", count, "units")
+        view("scroll", count, "units")
 
     def bindWidget(self, widget):
         """ Make the scroll in the widget, respond to this.
         Useful for child widgets.
         """
         # with Windows OS
-        widget.bind("<MouseWheel>", self.scroll)
+        widget.bind("<MouseWheel>", self.scrollV)
         # with Linux OS
-        widget.bind("<Button-4>", self.scroll)
-        widget.bind("<Button-5>", self.scroll)
+        widget.bind("<Button-4>", self.scrollV)
+        widget.bind("<Button-5>", self.scrollV)
+
+        widget.bind("<Control-Button-4>", self.scrollH)
+        widget.bind("<Control-Button-5>", self.scrollH)
+
 
     def getVScroll(self):
         return self.vscroll.get()
 
     def getHScroll(self):
         return self.hscroll.get()
 
@@ -260,16 +277,16 @@
     """A gradient frame which uses a canvas to draw the background
     Taken from:
         http://stackoverflow.com/questions/11892521/tkinter-custom-window
     """
 
     def __init__(self, parent, **args):
         tk.Canvas.__init__(self, parent, **args)
-        self._color1 = "#d2a7a7"
-        self._color2 = "#820808"
+        self._color1 = Config.SCIPION_BG_COLOR #"#d2a7a7"
+        self._color2 = Config.SCIPION_MAIN_COLOR #"#820808"
         self.bind("<Configure>", self._draw_gradient)
 
     def _draw_gradient(self, event=None):
         self.delete("gradient")
         width = self.winfo_width()
         height = self.winfo_height()
         limit = width // 2
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/mapper/__init__.py` & `scipion-pyworkflow-3.1.0/pyworkflow/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/mapper/mapper.py` & `scipion-pyworkflow-3.1.0/pyworkflow/mapper/mapper.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/mapper/sqlite.py` & `scipion-pyworkflow-3.1.0/pyworkflow/mapper/sqlite.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,21 +18,25 @@
 # * You should have received a copy of the GNU General Public License
 # * along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-
+import logging
+logger = logging.getLogger(__name__)
+import re
+from collections import OrderedDict
 
 from pyworkflow.utils import replaceExt, joinExt
+from .sqlite_db import SqliteDb, OperationalError
 from .mapper import Mapper
-from .sqlite_db import SqliteDb
 
 ID = 'id'
+CREATION = 'creation'
 PARENT_ID = 'parent_id'
 CLASSNAME = 'classname'
 NAME = 'name'
 
 
 class SqliteMapper(Mapper):
     """Specific Mapper implementation using Sqlite database"""
@@ -66,15 +70,15 @@
                 self.updatePendingPointers.append(obj)
                 value = "Pending update" 
             
         return value
         
     def __insert(self, obj, namePrefix=None):
         if not hasattr(obj, '_objDoStore'):
-            print("MAPPER: object '%s' doesn't seem to be an Object subclass,"
+            logger.info("MAPPER: object '%s' doesn't seem to be an Object subclass,"
                   "       it does not have attribute '_objDoStore'. "
                   "Insert skipped." % obj)
             return
         obj._objId = self.db.insertObject(obj._objName, obj.getClassName(),
                                           self.__getObjectValue(obj),
                                           obj._objParentId,
                                           obj._objLabel, obj._objComment)
@@ -88,15 +92,15 @@
         
     def insert(self, obj):
         """Insert a new object into the system, the id will be set"""
         self.__insert(obj)
         
     def insertChild(self, obj, key, attr, namePrefix=None):
         if not hasattr(attr, '_objDoStore'):
-            print("MAPPER: object '%s' doesn't seem to be an Object subclass,"
+            logger.info("MAPPER: object '%s' doesn't seem to be an Object subclass,"
                   "       it does not have attribute '_objDoStore'. \n"
                   "Insert skipped." % attr)
             return 
 
         if namePrefix is None:
             namePrefix = self.__getNamePrefix(obj)
         attr._objName = joinExt(namePrefix, key)
@@ -128,18 +132,18 @@
     
     def __getNamePrefix(self, obj):
         if len(obj._objName) > 0 and '.' in obj._objName:
             return replaceExt(obj._objName, obj.strId())
         return obj.strId()
     
     def __printObj(self, obj):
-        print("obj._objId", obj._objId)
-        print("obj._objParentId", obj._objParentId)
-        print("obj._objName", obj._objName)
-        print("obj.getObjValue()", obj.getObjValue())
+        logger.info("obj._objId: %s" % obj._objId)
+        logger.info("obj._objParentId: %s" % obj._objParentId)
+        logger.info("obj._objName: %s"% obj._objName)
+        logger.info("obj.getObjValue(): %s" % obj.getObjValue())
 
     def updateTo(self, obj, level=1):
         self.__initUpdateDict()
         self.__updateTo(obj, level)
         # Update pending pointers to objects
         for ptr in self.updatePendingPointers:
             self.db.updateObject(ptr._objId, ptr._objName,
@@ -197,52 +201,81 @@
 
     def getParent(self, obj):
         """ Retrieve the parent object of another. """
         return self.selectById(obj._objParentId)
         
     def fillObjectWithRow(self, obj, objRow):
         """ Fill the object with row data. """
+
+        rowId = objRow[ID]
+        rowName = self._getStrValue(objRow['name'])
+
         if not hasattr(obj, '_objId'):
             raise Exception("Entry '%s' (id=%s) in the database, stored as '%s'"
                             ", is being mapped to %s object. " %
-                            (self._getStrValue(objRow['name']), objRow[ID],
+                            (rowName, rowId,
                              objRow['classname'], type(obj)))
 
-        obj._objId = objRow[ID]
-        self.objDict[obj._objId] = obj
-        obj._objName = self._getStrValue(objRow['name'])
+        obj._objId = rowId
+
+        self.objDict[rowId] = obj
+        obj._objName = rowName
         obj._objLabel = self._getStrValue(objRow['label'])
         obj._objComment = self._getStrValue(objRow['comment'])
-        obj._objCreation = self._getStrValue(objRow['creation'])
+        obj._objCreation = self._getStrValue(objRow[CREATION])
         objValue = objRow['value']
         obj._objParentId = objRow[PARENT_ID]
         
         if obj.isPointer():
             if objValue is not None:
                 objValue = self.selectById(int(objValue))
-            else:
-                objValue = None
-        obj.set(objValue)
+            # This is necessary in some specific cases. E.g.:
+            # CTF consensus creating:
+            #   A.- Micrographs
+            #   B.- CTFs --> pointing to micrographs in this same protocol(#1)
+            # When loading this kind of protocol the sequence is as follows:
+            #  1 Loading of protocol consuming consensus CTF output ..
+            #    ...
+            #    finds inputCtf (DIRECT pointer to B)
+            #    2 loads set properties
+            #      ...
+            #      2.4 pointer to micrographs (Pointer to Consensus + extended)
+            #        2.4.1 pointee loads (Consensus protocol)
+            #        ...
+            #        ...
+            #        2.4.n _extended of 2.4 is loaded since is a child of consensus
+            #      2.4 obj.set() for 2.4 pointer --> will reset the extended to None.
+            obj.set(objValue, cleanExtended=False)
+        else:
+            obj.set(objValue)
         
     def fillObject(self, obj, objRow, includeChildren=True):
         self.fillObjectWithRow(obj, objRow)
         namePrefix = self.__getNamePrefix(obj)
 
         if includeChildren:
             childs = self.db.selectObjectsByAncestor(namePrefix)
 
             for childRow in childs:
+
                 childParts = childRow[NAME].split('.')
                 childName = childParts[-1]
+                childId = childRow[ID]
                 parentId = int(childParts[-2])
                 # Here we are assuming that always the parent have
                 # been processed first, so it will be in the dictionary
                 parentObj = self.objDict.get(parentId, None)
                 if parentObj is None:  # Something went wrong
                     continue
+
+                # If id already in the objDict skip all this
+                if childId in self.objDict.keys():
+                    setattr(parentObj, childName, self.objDict[childId])
+                    continue
+
                 childObj = getattr(parentObj, childName, None)
                 if childObj is None:
                     childObj = self._buildObjectFromClass(childRow[CLASSNAME])
                     # If we have any problem building the object, just ignore it
                     if childObj is None:
                         continue
                     setattr(parentObj, childName, childObj)
@@ -262,15 +295,15 @@
             name = self._getNameFromRow(row)
             childParts = name.split('.')
             childName = childParts[-1]
 
             # Get the parent, we should have it cached
             parentObj = self.objDict.get(parentId, None)
             if parentObj is None:  # Something went wrong
-                print("WARNING: Parent object (id=%d) was not found, "
+                logger.warning("Parent object (id=%d) was not found, "
                       "object: %s. Ignored." % (parentId, name))
                 return None
 
             childObj = getattr(parentObj, childName, None)
 
             # If parent object does not have that attribute
             if childObj is None:
@@ -379,27 +412,42 @@
             if obj is not None and objectFilter is None or objectFilter(obj):
                 objs.append(obj)
 
         return objs
 
     def _getObjectFromRow(self, row):
 
+        # Get the ID first
+        identifier = row[ID]
+
+        # If already in the dictionary we skipp al this
+        if identifier in self.objDict.keys():
+            return self.objDict[identifier]
+
         # Build the object without children
         obj = self.__buildObject(row)
 
         # If an object was created
         if obj is not None:
-            # Fill object attributes with row values
-            self.fillObjectWithRow(obj, row)
-
-            # Add it to the obj cache, we might need it latter to assign
-            # attributes
-            self.objDict[obj._objId] = obj
-
-            return obj
+            try:
+                # Fill object attributes with row values
+                self.fillObjectWithRow(obj, row)
+
+                # Add it to the obj cache, we might need it later to assign
+                # attributes
+                self.objDict[obj._objId] = obj
+
+                return obj
+
+            except Exception as e:
+                # Tolerate errors when loading attributes.
+                # This could happen then a protocol has change a param to a new type not compatible
+                # with previous values. Warn properly about it.
+                logger.warning("Can't load the row (%s, %s, %s) form the database to memory. This could cause future error." %
+                             (identifier, row[NAME], row[PARENT_ID]))
 
     def _getObjectFromDictionary(self, objId):
         return self.objDict[objId]
 
     @staticmethod
     def _getIdFromRow(row):
         return SqliteMapper._getFieldFromRow(ID, row)
@@ -489,24 +537,26 @@
     It will create connection, execute queries and commands"""
     # Maintain the current version of the DB schema
     # useful for future updates and backward compatibility
     # version should be an integer number
     VERSION = 1
     
     SELECT = ("SELECT id, parent_id, name, classname, value, label, comment, "
-              "datetime(creation, 'localtime') as creation FROM Objects WHERE ")
+              "datetime(creation, 'localtime') as creation FROM Objects")
     DELETE = "DELETE FROM Objects WHERE "
     DELETE_SEQUENCE = "DELETE FROM SQLITE_SEQUENCE WHERE name='Objects'"
     
     SELECT_RELATION = ("SELECT object_%s_id AS id FROM Relations "
                        "WHERE name=? AND object_%s_id=?")
     SELECT_RELATIONS = "SELECT * FROM Relations WHERE "
     EXISTS = "SELECT EXISTS(SELECT 1 FROM Objects WHERE %s=? LIMIT 1)"
     
     def selectCmd(self, whereStr, orderByStr=' ORDER BY id'):
+
+        whereStr = " WHERE " + whereStr if whereStr is not None else ''
         return self.SELECT + whereStr + orderByStr
     
     def __init__(self, dbName, timeout=1000, pragmas=None):
         SqliteDb.__init__(self)
         self._pragmas = pragmas or {}
         self._createConnection(dbName, timeout)
         self._initialize()
@@ -577,18 +627,18 @@
         try:
             self.executeCommand(
                 'INSERT INTO Objects (parent_id, name, classname, value, label, comment, creation)' +
                 ' VALUES (?, ?, ?, ?, ?, ?, datetime(\'now\'))',
                 (parent_id, name, classname, value, label, comment))
             return self.cursor.lastrowid
         except Exception as ex:
-            print("insertObject: ERROR")
-            print('INSERT INTO Objects (parent_id, name, classname, value, label, comment, creation)' +
+            logger.error("insertObject: ERROR")
+            logger.error('INSERT INTO Objects (parent_id, name, classname, value, label, comment, creation)' +
                   ' VALUES (?, ?, ?, ?, ?, ?, datetime(\'now\'))')
-            print((parent_id, name, classname, value, label, comment))
+            logger.error((parent_id, name, classname, value, label, comment))
             raise ex
         
     def insertRelation(self, relName, parent_id, object_parent_id, object_child_id, 
                        object_parent_extended=None, object_child_extended=None, **kwargs):
         """Execute command to insert a new object. Return the inserted object id"""
         self.executeCommand("INSERT INTO Relations "
                             "(parent_id, name, object_parent_id, object_child_id, creation, "
@@ -709,14 +759,15 @@
 
 class SqliteFlatMapper(Mapper):
     """Specific Flat Mapper implementation using Sqlite database"""
     def __init__(self, dbName, dictClasses=None, tablePrefix='',
                  indexes=None):
         Mapper.__init__(self, dictClasses)
         self._objTemplate = None
+        self._attributesToStore = None
         try:
             # We (ROB and JMRT) are playing with different
             # PRAGMAS (see https://www.sqlite.org/pragma.html)
             # for the SqliteFlatMapper instances
             # We have been playing with the following
             # pragmas: {synchronous, journal_mode, temp_store and
             #  cache_size} and inside scipion no improvement
@@ -736,14 +787,15 @@
                 # #'synchronous': 'OFF', # ON
                 # DELETE | TRUNCATE | PERSIST | MEMORY | WAL | OFF
                 # #'journal_mode': 'OFF', # DELETE
                 # FILE 0 | DEFAULT | 1 | FILE | 2 | MEMORY;
                 # #'temp_store': 'MEMORY',
                 # PRAGMA schema.cache_size = pages;
                 # #'cache_size': '5000' # versus -2000
+                # "temp_store_directory": "'.'",
             }
             self.db = SqliteFlatDb(dbName, tablePrefix,
                                    pragmas=pragmas, indexes=indexes)
             self.doCreateTables = self.db.missingTables()
             
             if not self.doCreateTables:
                 self.__loadObjDict()
@@ -760,16 +812,32 @@
         
     def insert(self, obj):
         if self.doCreateTables:
             self.db.createTables(obj.getObjDict(includeClass=True))
             self.doCreateTables = False
         """Insert a new object into the system, the id will be set"""
         self.db.insertObject(obj.getObjId(), obj.isEnabled(), obj.getObjLabel(), obj.getObjComment(), 
-                             *obj.getObjDict().values())
-        
+                             *self._getValuesFromObject(obj).values())
+
+    def getAttributes2Store(self, item):
+
+        if self._attributesToStore is None:
+            self._attributesToStore = [key for key, value in item.getAttributesToStore()]
+
+        return self._attributesToStore
+
+    def _getValuesFromObject(self, item):
+
+        valuesDict = OrderedDict()
+
+        for attr in self.getAttributes2Store(item):
+            item.fillObjDict('', valuesDict, False, attr, getattr(item, attr))
+
+        return valuesDict
+
     def enableAppend(self):
         """ This will allow to append items to existing db. 
         This is by default not allow, since most sets are not 
         modified after creation.
         """
         if not self.doCreateTables:
             obj = self.selectFirst()
@@ -864,20 +932,20 @@
         obj = self._objTemplate  # self.__buildAndFillObj()
         obj.setObjId(objRow[ID])
         obj.setObjLabel(self._getStrValue(objRow['label']))
         obj.setObjComment(self._getStrValue(objRow['comment']))
         
         try:
             obj.setEnabled(objRow['enabled'])
-            obj.setObjCreation(self._getStrValue(objRow['creation']))
+            obj.setObjCreation(self._getStrValue(objRow[CREATION]))
         except Exception:
-            # THIS SHOULD NOT HAPPENS
-            print("WARNING: 'creation' column not found in object: %s" % obj.getObjId())
-            print("         db: %s" % self.db.getDbName())
-            print("         objRow: ", dict(objRow))
+            # THIS SHOULD NOT HAPPEN
+            logger.warning("'creation' column not found in object: %s" % obj.getObjId())
+            logger.warning("         db: %s" % self.db.getDbName())
+            logger.warning("         objRow: %s." % dict(objRow))
 
         for c, attrName in self._objColumns:
             obj.setAttributeValue(attrName, objRow[c])
 
         return obj
         
     def __iterObjectsFromRows(self, objRows, objectFilter=None):
@@ -910,21 +978,52 @@
         # Just a sanity check for emtpy sets, that doesn't contains
         # 'Properties' table
         if not self.db.hasTable('Properties'):
             return iter([]) if iterate else []
             
         if self._objTemplate is None:
             self.__loadObjDict()
-        objRows = self.db.selectAll(orderBy=orderBy,
-                                    direction=direction,
-                                    where=where,
-                                    limit=limit)
+        try:
+            objRows = self.db.selectAll(orderBy=orderBy,
+                                        direction=direction,
+                                        where=where,
+                                        limit=limit)
+        except OperationalError as e:
+            msg="""Error executing selectAll command: %s.
+You may want to change the directory used by sqlite to create temporary files
+to one that has enough free space. By default this directory is /tmp
+You may achieve this goal by defining the SQLITE_TMPDIR environment variable
+and restarting scipion. Export command:
+    export SQLITE_TMPDIR=. """ % str(e)
+            raise OperationalError(msg)
         
         return self.__objectsFromRows(objRows, iterate, objectFilter) 
 
+    def unique(self, labels, where=None):
+        """ Returns a list (for a single label) or a dictionary with unique values for the passed labels.
+        If more than one label is passed it will be unique rows similar ti SQL unique clause.
+
+        :param labels (string or list) item attribute/s to retrieve unique row values
+        :param where (string) condition to filter the results"""
+
+        if isinstance(labels, str):
+            labels = [labels]
+
+        rows = self.db.unique(labels, where)
+        result = {label: [] for label in labels}  # Initialize the results dictionary
+        for row in rows:
+            for label in labels:
+                result[label].append(row[label])
+
+        # If there is only one label,
+        if len(labels) == 1:
+            return result[labels[0]]
+        else:
+            return result
+
     def aggregate(self, operations, operationLabel, groupByLabels=None):
         rows = self.db.aggregate(operations, operationLabel, groupByLabels)
         results = []
         for row in rows:
             values = {}
             for label in operations:
                 values[label] = row[label]
@@ -956,15 +1055,22 @@
         return self.db.setProperty(key, value)
     
     def deleteProperty(self, key):
         return self.db.deleteProperty(key)
     
     def getPropertyKeys(self):
         return self.db.getPropertyKeys()
-        
+
+    @staticmethod
+    def fmtDate(date):
+        """ Formats a python date into a valid string to be used in a where term
+        Currently creation files is stored in utc time and is has no microseconds.
+
+        :param date: python date un utc. use datetime.datetime.utcnow() instead of now()"""
+        return "datetime('%s')" % date.replace(microsecond=0)
 
 class SqliteFlatMapperException(Exception):
     pass
 
 
 SELF = 'self'
 
@@ -998,15 +1104,15 @@
         # and only setting to True when the tablePrefix is non-empty, which is
         # the case for classes that are different tables in the same db and it
         # logical to reuse the connection.
         self._reuseConnections = bool(tablePrefix)
 
         self.CHECK_TABLES = ("SELECT name FROM sqlite_master WHERE type='table'"
                              " AND name='%sObjects';" % tablePrefix)
-        self.SELECT = "SELECT * FROM %sObjects WHERE " % tablePrefix
+        self.SELECT = "SELECT * FROM %sObjects" % tablePrefix
         self.FROM = "FROM %sObjects" % tablePrefix
         self.DELETE = "DELETE FROM %sObjects WHERE " % tablePrefix
         self.INSERT_CLASS = ("INSERT INTO %sClasses (label_property, "
                              "column_name, class_name) VALUES (?, ?, ?)"
                              % tablePrefix)
         self.SELECT_CLASS = "SELECT * FROM %sClasses;" % tablePrefix
         self.EXISTS = "SELECT EXISTS(SELECT 1 FROM Objects WHERE %s=? LIMIT 1)"
@@ -1069,14 +1175,16 @@
         keys = [r[0] for r in self.cursor.fetchall()]
         return keys        
 
     def deleteProperty(self, key):
         self.executeCommand(self.DELETE_PROPERTY, (key,))
 
     def selectCmd(self, whereStr, orderByStr=' ORDER BY ' + ID):
+
+        whereStr = "" if whereStr is None else " WHERE " + whereStr
         return self.SELECT + whereStr + orderByStr
 
     def missingTables(self):
         """ Return True is the needed Objects and Classes table are not
         created yet. """
         self.executeCommand(self.CHECK_TABLES)
         result = self.cursor.fetchone()
@@ -1093,15 +1201,15 @@
     def createTables(self, objDict):
         """Create the Classes and Object table to store items of a Set.
         Each object will be stored in a single row.
         Each nested property of the object will be stored as a column value.
         """
         self.setVersion(self.VERSION)
         for pragma in self._pragmas.items():
-            print("executing pragma", pragma)
+            logger.debug("Executing pragma: %s" % pragma)
             self.executeCommand("PRAGMA %s = %s;" % pragma)
         # Create a general Properties table to store some needed values
         self.executeCommand("""CREATE TABLE IF NOT EXISTS Properties
                      (key       TEXT UNIQUE, -- property key                 
                       value     TEXT  DEFAULT NULL -- property value
                       )""")
         # Create the Classes table to store each column name and type
@@ -1195,47 +1303,39 @@
 
     def doesRowExist(self, objId):
         """Return True if a row with a given id exists"""
         self.executeCommand(self.EXISTS % ID, (objId,))
         one = self.cursor.fetchone()
         return one[0] == 1
 
+    def _getRealCol(self, colName):
+        """ Transform the column name taking into account
+         special columns such as: id or RANDOM(), and
+         getting the mapping translation otherwise.
+        """
+        if colName in [ID, 'RANDOM()', CREATION]:
+            return colName
+        elif colName in self._columnsMapping:
+            return self._columnsMapping[colName]
+        else:
+            return None
     def selectAll(self, iterate=True, orderBy=ID, direction='ASC',
-                  where='1', limit=None):
+                  where=None, limit=None):
         # Handle the specials orderBy values of 'id' and 'RANDOM()'
         # other columns names should be mapped to table column
         # such as: _micId -> c04
 
-        def _getRealCol(colName):
-            """ Transform the column name taking into account
-             special columns such as: id or RANDOM(), and
-             getting the mapping translation otherwise.
-            """
-            if colName in ['id', 'RANDOM()', 'creation']:
-                return colName
-            else:
-                return self._columnsMapping[colName]
-
         if isinstance(orderBy, str):
-            orderByCol = _getRealCol(orderBy)
+            orderByCol = self._getRealCol(orderBy)
         elif isinstance(orderBy, list):
-            orderByCol = ','.join([_getRealCol(c) for c in orderBy])
+            orderByCol = ','.join([self._getRealCol(c) for c in orderBy])
         else:
             raise Exception('Invalid type for orderBy: %s' % type(orderBy))
 
-        # Parse the where string to replace the column name with
-        # the real table column name ( for example: _micId -> c01 )
-        # Right now we are assuming a simple where string in the form
-        # colName=VALUE
-        if '=' in where:
-            whereCol = where.split('=')[0]
-            whereRealCol = _getRealCol(whereCol)
-            whereStr = where.replace(whereCol, whereRealCol)
-        else:
-            whereStr = where
+        whereStr = self._whereToWhereStr(where)
 
         cmd = self.selectCmd(whereStr,
                              orderByStr=' ORDER BY %s %s'
                                         % (orderByCol, direction))
         # If there is a limit
         if limit:
             # if it is a tuple
@@ -1246,14 +1346,67 @@
             # If we need to skip rows
             skipPart = "%s," % skipRows if skipRows else ""
             cmd += " LIMIT %s %s" % (skipPart, limit)
 
         self.executeCommand(cmd)
         return self._results(iterate)
 
+    def _whereToWhereStr(self, where):
+        """ Parse the where string to replace the column name with
+        the real table column name ( for example: _micId -> c01 )
+        Right now we are assuming a simple where string in the form
+        colName=VALUE
+
+        :param where string with pair of terms separated by "=" where left
+        element is an attribute of the item
+
+        >>> Example:
+        >>> _micId=3 OR _micId=4
+        """
+        if where is None:
+            return
+
+        whereStr = where
+        # Split by valid where operators: =, <, >
+        result = re.split('<=|<=|=|<|>|AND|OR', where)
+        # For each item
+        for term in result:
+            # trim it
+            term = term.strip()
+            whereRealCol = self._getRealCol(term)
+            if whereRealCol is not  None:
+                whereStr = whereStr.replace(term, whereRealCol)
+
+        return whereStr
+
+    def unique(self, labels, where=None):
+        """ Returns the results of the execution of a UNIQUE query
+
+        :param labels: list of attributes which you want unique values from
+        :param where: condition to match in the form: attrName=value
+        :return:
+        """
+        # let us count for testing
+        selectStr = 'SELECT DISTINCT '
+        separator = ' '
+        # This cannot be like the following line should be expressed in terms
+        # of c01, c02 etc (actual fields)....
+        for label in labels:
+            selectStr += "%s %s AS %s " % (separator, self._getRealCol(label), label)
+            separator = ', '
+
+        sqlCommand = selectStr + self.FROM
+
+        whereStr = self._whereToWhereStr(where)
+        if whereStr is not None:
+            sqlCommand += " WHERE " + whereStr
+
+        self.executeCommand(sqlCommand)
+        return self._results(iterate=False)
+
     def aggregate(self, operations, operationLabel, groupByLabels=None):
         # let us count for testing
         selectStr = 'SELECT '
         separator = ' '
         # This cannot be like the following line should be expressed in terms
         # of C1, C2 etc....
         for operation in operations:
@@ -1288,14 +1441,15 @@
     # FIXME: Seems to be duplicated and a subset of selectAll
     def selectObjectsBy(self, iterate=False, **args):
         """More flexible select where the constrains can be passed
         as a dictionary, the concatenation is done by an AND"""
         whereList = ['%s=?' % k for k in args.keys()]
         whereStr = ' AND '.join(whereList)
         whereTuple = tuple(args.values())
+        whereStr = self._whereToWhereStr(whereStr)
         self.executeCommand(self.selectCmd(whereStr), whereTuple)
         return self._results(iterate)
 
     # FIXME: Seems to be duplicated and a subset of selectAll
     # Moreover, it does not translate between "user columns" and
     # "internal" Objects table columns
     def selectObjectsWhere(self, whereStr, iterate=False):
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/mapper/sqlite_db.py` & `scipion-pyworkflow-3.1.0/pyworkflow/mapper/sqlite_db.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,66 +25,81 @@
 # **************************************************************************
 
 
 """
 This module contains some sqlite basic tools to handle Databases.
 """
 
+import logging
+logger = logging.getLogger(__name__)
 from sqlite3 import dbapi2 as sqlite
-
-from pyworkflow import SCIPION_DEBUG_SQLITE
-from pyworkflow.utils import envVarOn
+from sqlite3 import OperationalError as OperationalError
+from pyworkflow.utils import STATUS, getExtraLogInfo, Config
 
 
 class SqliteDb:
     """Class to handle a Sqlite database.
     It will create connection, execute queries and commands.
     """
     OPEN_CONNECTIONS = {}  # Store all connections made
-    
+
     def __init__(self):
         self._reuseConnections = False
-        
+
     def _createConnection(self, dbName, timeout):
         """Establish db connection"""
         self._dbName = dbName
         if self._reuseConnections and dbName in self.OPEN_CONNECTIONS:
             self.connection = self.OPEN_CONNECTIONS[dbName]
         else:
+            # self.closeConnection(dbName)  # Close the connect if exists for this db
             self.connection = sqlite.Connection(dbName, timeout, check_same_thread=False)
             self.connection.row_factory = sqlite.Row
             self.OPEN_CONNECTIONS[dbName] = self.connection
-            
+            logger.debug("Connection open for %s" % dbName, extra=getExtraLogInfo(
+                "CONNECTIONS",
+                STATUS.START,
+                dbfilename=dbName))
+
         self.cursor = self.connection.cursor()
         # Define some shortcuts functions
-        if envVarOn(SCIPION_DEBUG_SQLITE):
+        if Config.debugSQLOn():
             self.executeCommand = self._debugExecute
         else:
             self.executeCommand = self.cursor.execute
         self.commit = self.connection.commit
         
     @classmethod
     def closeConnection(cls, dbName):
         if dbName in cls.OPEN_CONNECTIONS:
             connection = cls.OPEN_CONNECTIONS[dbName]
             del cls.OPEN_CONNECTIONS[dbName]
             connection.close()
-        
+            logger.debug("Connection closed for %s" % dbName,
+                         extra=getExtraLogInfo('CONNECTIONS', STATUS.STOP, dbfilename=dbName))
+
     def getDbName(self):
         return self._dbName
     
     def close(self):
         self.connection.close()
+        logger.debug("Connection closed for %s" % self._dbName,
+                     extra=getExtraLogInfo(
+                                        "CONNECTIONS",
+                                        STATUS.STOP,
+                                        dbfilename=self._dbName))
         if self._dbName in self.OPEN_CONNECTIONS:
             del self.OPEN_CONNECTIONS[self._dbName]
         
     def _debugExecute(self, *args):
         try:
-            print("COMMAND: ", args[0], self._dbName)
-            print("ARGUMENTS: ", args[1:])
+            logger.debug("COMMAND: %s; %s" %(args[0] , self._dbName),
+                extra=getExtraLogInfo("QUERY", STATUS.EVENT, dbfilename=self._dbName)
+            )
+            logger.debug("ARGUMENTS: " + str(args[1:]))
             return self.cursor.execute(*args)
         except Exception as ex:
             print(">>>> FAILED cursor.execute on db: '%s'" % self._dbName)
             raise ex
 
     def _iterResults(self):
         row = self.cursor.fetchone()
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/mapper/xmlmapper.py` & `scipion-pyworkflow-3.1.0/pyworkflow/mapper/xmlmapper.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/object.py` & `scipion-pyworkflow-3.1.0/pyworkflow/object.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,19 +24,22 @@
 # *
 # **************************************************************************
 """
 This modules holds the base classes for the ORM implementation.
 The Object class is the root in the hierarchy and some other
 basic classes.
 """
-import os
+import logging
+logger = logging.getLogger(__name__)
+
 from collections import OrderedDict
 import datetime as dt
+from os.path import getmtime
 
-from pyworkflow import utils
+from pyworkflow.utils import getListFromValues, getListFromRangeString
 from pyworkflow.utils.reflection import getSubclasses
 
 
 # Binary relations always involve two objects, we 
 # call them parent-child objects, the following
 # constants reflect which direction of the relation we refer
 RELATION_CHILDS = 0
@@ -50,26 +53,38 @@
 
 # Then column name of the parent id relation
 OBJECT_PARENT_ID = 'object_parent_id'
 
 
 class Object(object):
     """ All objects in our Domain should inherit from this class
-    that will contains all base properties"""
+    that will contain all base properties"""
 
     def __init__(self, value=None, **kwargs):
         object.__init__(self)
-        self._objIsPointer = kwargs.get('objIsPointer', False)  # True if will be treated as a reference for storage
-        self._objId = kwargs.get('objId', None)  # Unique identifier of this object in some context
-        self._objParentId = kwargs.get('objParentId', None)  # identifier of the parent object
-        self._objName = kwargs.get('objName', '')  # The name of the object will contains the whole path of ancestors
-        self._objLabel = kwargs.get('objLabel', '')  # This will serve to label the objects
-        self._objComment = kwargs.get('objComment', '')
-        self._objTag = kwargs.get('objTag', None)  # This attribute serve to make some annotation on the object.
-        self._objDoStore = kwargs.get('objDoStore', True)  # True if this object will be stored from his parent
+        if len(kwargs) == 0:
+            self._objIsPointer =  False  # True if will be treated as a reference for storage
+            self._objId =  None  # Unique identifier of this object in some context
+            self._objParentId =  None  # identifier of the parent object
+            self._objName = ''  # The name of the object will contains the whole path of ancestors
+            self._objLabel =  ''  # This will serve to label the objects
+            self._objComment = ''
+            # Performance: self._objTag =  None  # This attribute serve to make some annotation on the object.
+            self._objDoStore = True
+        else:
+
+            self._objIsPointer = kwargs.get('objIsPointer', False)  # True if will be treated as a reference for storage
+            self._objId = kwargs.get('objId', None)  # Unique identifier of this object in some context
+            self._objParentId = kwargs.get('objParentId', None)  # identifier of the parent object
+            self._objName = kwargs.get('objName', '')  # The name of the object will contains the whole path of ancestors
+            self._objLabel = kwargs.get('objLabel', '')  # This will serve to label the objects
+            self._objComment = kwargs.get('objComment', '')
+            #Performance: self._objTag = kwargs.get('objTag', None)  # This attribute serve to make some annotation on the object.
+            self._objDoStore = kwargs.get('objDoStore', True)  # True if this object will be stored from his parent
+
         self._objCreation = None
         self._objParent = None  # Reference to parent object
         self._objEnabled = True
         self.set(value)
 
     def getClassName(self):
         return self.__class__.__name__
@@ -127,32 +142,32 @@
                 if ignoreMissing:
                     return
                 raise Exception("Object.setAttributeValue: obj is None! attrName: "
                                 "%s, part: %s" % (attrName, partName))
         obj.set(value)
         
     def getAttributes(self):
-        """Return the list of attributes than are
+        """Return the list of attributes that are
         subclasses of Object"""
-        for key, attr in self.__dict__.items():
-            if issubclass(attr.__class__, Object):
-                yield key, attr
+        for name in vars(self):
+            value = getattr(self, name)
+            if isinstance(value, Object):
+                yield name, value
                 
     def getAttributesToStore(self):
         """Return the list of attributes than are
         subclasses of Object and will be stored"""
         for key, attr in self.getAttributes():
-            if not hasattr(attr, '_objDoStore'):
-                print("Object.getAttributesToStore: attribute '%s' seems to "
-                      "be overwritten," % key)
-                print("   since '_objDoStore' was not found. "
-                      "Ignoring attribute. ")
-            else:
+            try:
                 if attr is not None and attr._objDoStore:
                     yield key, attr
+            except Exception as e:
+                logger.info("Object.getAttributesToStore: attribute '%s' (%s) seems to "
+                      "be overwritten, since '_objDoStore' was not found. Ignoring attribute." % (key, type(attr)))
+                logger.debug("Exception: %s" % e)
 
     def isPointer(self):
         """If this is true, the value field is a pointer 
         to another object"""
         return self._objIsPointer
         
     def _convertValue(self, value):
@@ -324,17 +339,15 @@
             v2 = getattr(other, k)
             if issubclass(type(v1), Object):
                 comp = v1.equalAttributes(v2, ignore=ignore, verbose=verbose)
             else:
                 comp = v1 == v2
             if not comp:
                 if verbose:
-                    print("Different attributes: ")
-                    print("self.%s = %s" % (k, v1))
-                    print("other.%s = %s" % (k, v2))
+                    logger.info("Different attributes: self.%s = %s, other.%s = %s" % (k, v1, k, v2))
                 return False
         return True
             
     def copyAttributes(self, other, *attrNames):
         """ Copy attributes in attrNames from other to self. 
         If the name X is in attrNames, it would be equivalent to:
         self.X.set(other.X.get())
@@ -348,40 +361,52 @@
             if attr is None:
                 setattr(self, name, otherAttr.clone())
             elif isinstance(attr, Pointer):
                 attr.copy(otherAttr)
             elif isinstance(attr, PointerList):
                 for pointer in otherAttr:
                     attr.append(pointer)
+            elif isinstance(attr, Scalar) and otherAttr.hasPointer():
+                attr.copy(otherAttr)
             else:
                 attr.set(otherAttr.get())
             
     def __getObjDict(self, prefix, objDict, includeClass):
         if prefix:
             prefix += '.'
         for k, v in self.getAttributesToStore():
-            if not v.isPointer():
-                kPrefix = prefix + k
-                if includeClass:
-                    objDict[kPrefix] = (v.getClassName(), v.getObjValue())
-                else:
-                    objDict[kPrefix] = v.getObjValue()
-                if not isinstance(v, Scalar):
-                    v.__getObjDict(kPrefix, objDict, includeClass)
-            
+            self.fillObjDict(prefix, objDict, includeClass, k, v)
+
+    @staticmethod
+    def fillObjDict(prefix, objDict, includeClass, k, v):
+
+        if not v.isPointer():
+            kPrefix = prefix + k
+            if includeClass:
+                objDict[kPrefix] = (v.getClassName(), v.getObjValue())
+            else:
+                objDict[kPrefix] = v.getObjValue()
+            if not isinstance(v, Scalar):
+                v.__getObjDict(kPrefix, objDict, includeClass)
+
     def getObjDict(self, includeClass=False, includeBasic=False):
-        """ Return all attributes and values in a dictionary.
+        """
+        Return all attributes and values in a dictionary.
         Nested attributes will be separated with a dot in the dict key.
-        Params:
-            includeClass: if True, the values will be a tuple (ClassName, value)
-                otherwise only the values of the attributes
-            includeBasic: if True include the id, label and comment.
-                object.id: objId
-                object.label: objLabel
-                object.comment: objComment
+
+        :param includeClass: if True, the values will be a tuple (ClassName, value)
+            otherwise only the values of the attributes
+        :param includeBasic: if True include the id, label and comment.
+
+        includeBasic example::
+
+            object.id: objId
+            object.label: objLabel
+            object.comment: objComment
+
         """
         d = OrderedDict()
 
         if includeClass:
             d['self'] = (self.getClassName(),)
 
         if includeBasic:
@@ -435,20 +460,22 @@
         """
         return [self.getNestedValue(k) for k in objDict if k != 'self']
     
     def getValuesFromMappedDict(self, mappedDict):
         return [v.getObjValue() for v in mappedDict.values()]
     
     def copy(self, other, copyId=True, ignoreAttrs=[]):
-        """ Copy all attributes values from one object to the other.
+        """
+        Copy all attributes values from one object to the other.
         The attributes will be created if needed with the corresponding type.
-        Params:
-            other: the other object from which to make the copy.
-            copyId: if true, the _objId will be also copied.
+
+        :param other: the other object from which to make the copy.
+        :param copyId: if true, the _objId will be also copied.
             ignoreAttrs: pass a list with attributes names to ignore.
+
         """
         copyDict = {'internalPointers': []} 
         self._copy(other, copyDict, copyId, ignoreAttrs=ignoreAttrs)
         self._updatePointers(copyDict)
         return copyDict
         
     def _updatePointers(self, copyDict):
@@ -498,23 +525,27 @@
     
     def clone(self):
         clone = self.getClass()()
         clone.copy(self)        
         return clone    
     
     def evalCondition(self, condition):
-        """ Check if condition is meet.
-        Params:
-            condition: the condition string, it can contains variables
-                or methods without arguments to be evaluated.
-            Examples:
-                hasCTF
-                hasCTF and not hasAlignment
-        Return:
-            The value of the condition evaluated with values
+        """
+        Check if condition is meet.
+
+        Examples of condition::
+
+            "hasCTF"
+            "hasCTF and not hasAlignment"
+
+        :param condition: the condition string, it can contain variables
+            or methods without arguments to be evaluated.
+
+        :return The value of the condition evaluated with values
+
         """
         # Split in possible tokens
         import re
         tokens = re.split('\W+', condition)
         condStr = condition
         
         for t in tokens:
@@ -524,74 +555,34 @@
     
     def printAll(self, name=None, level=0):
         """Print object and all its attributes.
         Mainly for debugging"""
         tab = ' ' * (level*3)
         idStr = ''  # ' (id = %s, pid = %s)' % (self.getObjId(), self._objParentId)
         if name is None:
-            print(tab, self.getClassName(), idStr)
+            logger.info(tab, self.getClassName(), idStr)
         else:
             if name == 'submitTemplate':  # Skip this because very large value
                 value = '...'
             else:
                 value = self.getObjValue()
                 
-            print(tab, '%s = %s' % (name, value), idStr)
+            logger.info(tab, '%s = %s' % (name, value), idStr)
         for k, v in self.getAttributes():
             v.printAll(k, level + 1)
             
     def printObjDict(self, includeClasses=False):
         """Print object dictionary. Mainly for debugging"""
         import pprint
         pp = pprint.PrettyPrinter(indent=4)
         pp.pprint(dict(self.getObjDict(includeClasses)))        
 
-
 class OrderedObject(Object):
-    """This is based on Object, but keep the list
-    of the attributes to store in the same order
-    of insertion, this can be useful where order matters"""
-    def __init__(self, value=None, **kwargs):
-        object.__setattr__(self, '_attributes', [])
-        Object.__init__(self, value, **kwargs)
-
-    def __attrPointed(self, name, value):
-        """ Check if a value is already pointed by other
-        attribute. This will prevent to storing pointed
-        attributes such as:
-        self.inputMics = self.inputMicrographs.get()
-        In this case we want to avoid to store self.inputMics as 
-        another attribute of this object.
-        """
-        for key in self._attributes:
-            attr = getattr(self, key)
-            if attr is not None and attr.isPointer():
-                if attr.get() is value:
-                    return True
-        return False
-    
-    def __setattr__(self, name, value):
-        if (name not in self._attributes and
-            issubclass(value.__class__, Object) and
-                not self.__attrPointed(name, value) and value._objDoStore):
-            self._attributes.append(name)
-        Object.__setattr__(self, name, value)
-    
-    def getAttributes(self):
-        """Return the list of attributes than are
-        subclasses of Object and will be stored"""
-        for key in self._attributes:
-            yield key, getattr(self, key)
-                
-    def deleteAttribute(self, attrName):
-        """ Delete an attribute. """
-        if attrName in self._attributes:
-            self._attributes.remove(attrName)
-            delattr(self, attrName)
-
+    """Legacy class, to be removed. Object should give same functionality and is faster"""
+    pass
                 
 class Scalar(Object):
     """Base class for basic types"""
     def hasValue(self):        
         return self._objValue is not None
     
     def equalAttributes(self, other, ignore=[], verbose=False):
@@ -638,22 +629,28 @@
     def __ge__(self, other):
         return self.__cmp(other) >= 0
 
     def get(self, default=None):
         """Get the value, if internal value is None
         the default argument passed is returned. """
         if self.hasPointer():
-            return self._pointer.get().get(default)
+            # Get pointed value
+            pointedValue = self._pointer.get()
+
+            return default if pointedValue is None else pointedValue.get(default)
 
         if self.hasValue():
             return self._objValue
         return default
     
     def _copy(self, other, *args, **kwargs):
-        self.set(other.get())
+        if other.hasPointer():
+            self.setPointer(other.getPointer())
+        else:
+            self.set(other.get())
         
     def swap(self, other):
         """ Swap the contained value between
         self and other objects.
         """
         tmp = self._objValue
         self._objValue = other._objValue
@@ -709,19 +706,21 @@
 class String(Scalar):
     """String object. """
     DATETIME_FORMAT = "%Y-%m-%d %H:%M:%S"
     FS = ".%f"  # Femto seconds
 
     @classmethod
     def getDatetime(cls, strValue, formatStr=None, fs=True):
-        """ Get the datetime from the given string value.
-        Params:
-            strValue: string representation of the date
-            formatStr: if is None, use the default DATETIME_FORMAT.
-            fs: Use femto seconds or not, only when format=None
+        """
+        Converts the given string value to a datetime object.
+
+        :param strValue: string representation of the date
+        :param formatStr: if None, uses the default cls:String.DATETIME_FORMAT.
+        :param fs: Use femto seconds or not, only when format=None
+
         """
         if formatStr is None:
             try:
                 formatStr = cls.DATETIME_FORMAT
                 if fs:
                     formatStr += cls.FS
                 datetime = dt.datetime.strptime(strValue, formatStr)
@@ -743,14 +742,23 @@
             return True
         return len(self.get().strip()) == 0
 
     def datetime(self, formatStr=None, fs=True):
         """ Get the datetime from this object string value. """
         return String.getDatetime(self._objValue, formatStr, fs)
 
+    def getListFromValues(self, length=None, caster=int):
+        """ Returns a list from a string with values as described at getListFromValues. Useful for """
+        return getListFromValues(self._objValue, length, caster)
+
+    def getListFromRange(self):
+        """ Returns a list from a string with values as described at getListFromRangeString.
+         Useful for NumericRangeParam params"""
+        return getListFromRangeString(self._objValue)
+
 
 class Float(Scalar):
     """Float object"""
     EQUAL_PRECISION = 0.001
     
     @classmethod
     def setPrecision(cls, newPrecision):
@@ -794,17 +802,17 @@
     
     def __nonzero__(self):
         if not self.hasValue():
             return False
         return self.get() 
     
     def __bool__(self):
-        return self.get()  
-    
-    
+        return self.get()
+
+
 class Pointer(Object):
     """Reference object to other one"""
     EXTENDED_ATTR = '__attribute__'
     EXTENDED_ITEMID = '__itemid__'
     _ERRORS = {}
     
     def __init__(self, value=None, **kwargs):
@@ -844,31 +852,31 @@
         """
         extended = self._extended.get()
         if extended:
             ext = self.__clean(extended)
             parts = ext.split('.')
             value = self._objValue
             for p in parts:
-                if p.isdigit():
+                if hasattr(value, "__getitem__") and p.isdigit():
                     value = value[int(p)]  # item case
                 else:
                     value = getattr(value, p, None)
                 if value is None:
                     break
         else:
             value = self._objValue
             
         return value
     
-    def set(self, other):
+    def set(self, other, cleanExtended=True):
         """ Set the pointer value but cleaning the extended property. """
         Object.set(self, other)
         # This check is needed because set is call from the Object constructor
         # when this attribute is not setup yet (a dirty patch, I know)
-        if hasattr(self, '_extended'):
+        if cleanExtended and hasattr(self, '_extended'):
             self._extended.set(None)
         
     def hasExtended(self):
         return bool(self._extended.get())  # consider empty string as false
     
     def getExtended(self):
         return self.__clean(self._extended.get(''))
@@ -1030,15 +1038,20 @@
                     self.append(self._pType(s))
             elif isinstance(value, list) or isinstance(value, tuple):
                 for s in value:
                     self.append(self._pType(s))
             else:
                 raise Exception("CsvList.set: Invalid value type: ",
                                 type(value))
-            
+
+    def equalAttributes(self, other, ignore=[], verbose=False):
+        """Compare that all attributes are equal"""
+
+        return self == other
+
     def getObjValue(self):
         self._objValue = ','.join(map(str, self))
         return self._objValue
     
     def get(self):
         return self.getObjValue()
     
@@ -1054,32 +1067,31 @@
     def __eq__(self, other):
         """ Comparison for scalars should be by value
         and for other objects by reference.
         """
         return all(a == b for a, b in zip(self, other))
 
 
-class Set(OrderedObject):
+class Set(Object):
     """ This class will be a container implementation for elements.
     It will use an extra sqlite file to store the elements.
-    All items will have an unique id that identifies each element in the set.
+    All items will have a unique id that identifies each element in the set.
     """
     ITEM_TYPE = None  # This property should be defined to know the item type
     
     # This will be used for stream Set where data is populated on the fly
     STREAM_OPEN = 1
     STREAM_CLOSED = 2
 
-    FILE_TEMPLATE_NAME = 'set%s.sqlite'
     indexes = ['_index']
     
     def __init__(self, filename=None, prefix='', 
                  mapperClass=None, classesDict=None, **kwargs):
         # Use the object value to store the filename
-        OrderedObject.__init__(self, **kwargs)
+        super().__init__(**kwargs)
         self._mapper = None
         self._idCount = 0
         self._size = Integer(0)  # cached value of the number of images
         # It is a bit contradictory that initially a set is Closed
         # but this is the default behaviour of the Set before Streaming extension
         self._streamState = Integer(self.STREAM_CLOSED)  
         self.setMapperClass(mapperClass)
@@ -1090,54 +1102,101 @@
 
         # If filename is passed in the constructor, it means that
         # we want to create a new object, so we need to delete it if
         # the file exists
         if filename:
             self._mapperPath.set('%s, %s' % (filename, prefix))
             self.load()
-            
+
+    def copy(self, other, copyId=True, ignoreAttrs=['_mapperPath', '_size', '_streamState']):
+        """ Copies the attributes of the set
+
+        :param other: Set to copy attributes from
+        :param copyId: True. Copies the objId.
+        :param ignoreAttrs: Attributes list to ignore while copying. _mapperPath, _size and _streamState
+        are ignored by default.
+        
+        """
+        
+        # Note: By default this behaves properly for cloning non identical objects. 
+        # This is to clone a set from another new set that is based on "other".
+        # For exact clone, we need to pass empty ignoreAttrs. This case happens in Protocol.__tryUpdateOutputSet
+        super().copy(other, copyId, ignoreAttrs)
+
     def _getMapper(self):
         """ This method will open the connection to the items
         database on demand. That's why this method should 
         be used instead of accessing directly _mapper.
         """
         if self._mapper is None:
             self.load()
         return self._mapper
             
     def aggregate(self, operations, operationLabel, groupByLabels=None):
+        """
+         This method operate on sets of values. They are used with a
+         GROUP BY clause to group values into subsets
+        :param operations: list of aggregate function such as COUNT, MAX, MIN,...
+        :param operationLabel: label to use by the aggregate function
+        :param groupByLabels: list of labels to group
+        :return: the aggregated value of each group
+        """
         return self._getMapper().aggregate(operations, operationLabel, groupByLabels)
 
     def setMapperClass(self, MapperClass):
         """ Set the mapper to be used for storage. """
         if MapperClass is None:
             from pyworkflow.mapper.sqlite import SqliteFlatMapper
             MapperClass = SqliteFlatMapper
         Object.__setattr__(self, '_MapperClass', MapperClass)
         
     def __getitem__(self, itemId):
-        """ Get the image with the given id. """
-        return self._getMapper().selectById(itemId)
+        """ Get the image with the given id.
+
+        NOTE: Performance warning: this method is expensive in terms of performance use of
+        iterItems is preferred. Use this one only for a single item retrieval.
+
+        :param itemId: the objId (integer) of the item. Alternatively itemId could be a dictionary like
+
+            {_alternative_identifier: 'RG-1234'}
+
+            where '_alternative_identifier' is an attribute of the item and 'RG-1234' the value to look for
+            only the first matching item is returned in case there are more
+
+        """
+        closedMapper = self._mapper is None
+
+        if isinstance(itemId, dict):
+            for obj in self._getMapper().selectBy(**itemId):
+                item = obj
+                break
+        else:
+            item = self._getMapper().selectById(itemId)
+
+        if closedMapper:
+            self.close()
+        return item
 
     def __contains__(self, itemId):
         """ element in Set """
         return self._getMapper().exists(itemId)
 
-    def iterItems(self, orderBy='id', direction='ASC', where='1',
-                  limit=None):
+    def iterItems(self, orderBy='id', direction='ASC', where=None,
+                  limit=None, iterate=True):
         return self._getMapper().selectAll(orderBy=orderBy,
                                            direction=direction,
                                            where=where,
-                                           limit=limit)  # has flat mapper, iterate is true
+                                           limit=limit,
+                                           iterate=iterate)  # has flat mapper, iterate is true
 
     def getFirstItem(self):
         """ Return the first item in the Set. """
         # This function is used in many contexts where the mapper can be
-        # left open and could be problematic locking other db
-        # So, we looking if the mapper was closed before, in which case
+        # left open and could be problematic locking the db for other processes
+        # So, we look if the mapper was closed before, in which case
         # we will close it after that
         closedMapper = self._mapper is None
         firstItem = self._getMapper().selectFirst()
         if closedMapper:
             self.close()
         return firstItem
     
@@ -1164,19 +1223,20 @@
         if len(self._mapperPath) > 1:
             return self._mapperPath[1]
         return None
     
     def write(self, properties=True):
         """
         Commit the changes made to the Set underlying database.
-        Params:
-            properties: this flag controls when to write Set attributes to 
-                special table 'Properties' in the database. False value is 
-                use for example in SetOfClasses for not writing each Class2D 
-                properties.
+
+        :param properties: this flag controls when to write Set attributes to
+            special table 'Properties' in the database. False value is
+            use for example in SetOfClasses for not writing each Class2D
+            properties.
+
         """
         if properties:
             self._getMapper().setProperty('self', self.getClassName())
             objDict = self.getObjDict()
             for key, value in objDict.items():
                 self._getMapper().setProperty(key, value)
         self._getMapper().commit()
@@ -1290,18 +1350,15 @@
         """ Retrieve all properties stored by the mapper. """
         for key in self._getMapper().getPropertyKeys():
             if key != 'self':
                 self.loadProperty(key)
         
     def getIdSet(self):
         """ Return a Python set object containing all ids. """
-        s = set()
-        for item in self.iterItems():
-            s.add(item.getObjId())
-        return s
+        return set(self.getUniqueValues('id'))
     
     def getFiles(self):
         files = set()
         if self.getFileName():
             files.add(self.getFileName())
         return files
     
@@ -1321,32 +1378,48 @@
         """ By default, when a Set is loaded, it is opened
         in read-only mode, so no new insertions are allowed.
         This function will allow to append more items
         to an existing set.
         """
         self._getMapper().enableAppend()
 
-    @classmethod
-    def create(cls, path, template=None, suffix='', **kwargs):
-        """ Create a set and set the filename using the suffix.
-        If the file exists, it will be delete. """
-
-        if template is None:
-            template = cls.FILE_TEMPLATE_NAME
-
-        setFn = os.path.join(path, template % suffix)
-        # Close the connection to the database if
-        # it is open before deleting the file
-        utils.cleanPath(setFn)
-        import pyworkflow.mapper as pwmapper
-        pwmapper.SqliteDb.closeConnection(setFn)
-        setObj = cls(filename=setFn, **kwargs)
-        return setObj
 
 
+
+    # ******* Streaming helpers to deal with sets **********
+    def hasChangedSince(self, time):
+        """ Returns if the set has changed since the timestamp passed as parameter. It will check the
+        the last modified time of the file this set uses to persists.
+
+        :parameter time: timestamp to compare to the last modification time  """
+
+        if time is None:
+            return True
+
+        # Get the file name
+        localFile = self.getFileName()
+
+        #self.lastCheck = getattr(self, 'lastCheck', now)
+        # Get the last time it was modified
+        modTime = dt.datetime.fromtimestamp(getmtime(localFile))
+        return time < modTime
+
+    def getUniqueValues(self, attributes, where=None):
+        """ Returns a list (for a single label) or a dictionary with unique values for the passed labels.
+        If more than one label is passed it will be unique rows similar ti SQL unique clause.
+
+        :param attributes (string or list) item attribute/s to retrieve unique row values
+        :param where (string) condition to filter the results"""
+
+        return self._getMapper().unique(attributes, where)
+
+    def fmtDate(self, date):
+        """ Formats a python date to a valid string for the mapper"""
+        return self._getMapper().fmtDate(date)
+
 def ObjectWrap(value):
     """This function will act as a simple Factory
     to create objects from Python basic types"""
     t = type(value)
     if issubclass(t, Object):
         return value
     if t is int:
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/plugin.py` & `scipion-pyworkflow-3.1.0/pyworkflow/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,22 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+import logging
+import sys
+
+from .protocol import Protocol
+from .viewer import Viewer
+from .wizard import Wizard
+
+logger = logging.getLogger(__name__)
 import glob
 import os
 import importlib
 import inspect
 import traceback
 import types
 import pkg_resources
@@ -37,76 +45,100 @@
 from collections import OrderedDict
 from abc import ABCMeta, abstractmethod
 
 import pyworkflow as pw
 import pyworkflow.utils as pwutils
 import pyworkflow.object as pwobj
 from pyworkflow.template import Template
+from pyworkflow.utils import sortListByList
 
 from .constants import *
 
 
 class Domain:
     """ Class to represent the application domain.
     It will allow to specify new objects, protocols, viewers and wizards
     through the registration of new plugins.
     """
 
     # The following classes should be defined in subclasses of Domain
-    _name = None
-    _protocolClass = None
+    _name = __name__
+    _protocolClass = Protocol
     _objectClass = pwobj.Object
-    _viewerClass = None
-    _wizardClass = None
+    _viewerClass = Viewer
+    _wizardClass = Wizard
     _baseClasses = {}  # Update this with the base classes of the Domain
 
     # Dictionaries to store different type of objects
     _plugins = {}
     _protocols = {}
     _objects = {}
     _viewers = {}
     _wizards = {}
 
     @classmethod
     def registerPlugin(cls, name):
         """ Register a new plugin. This function should only be called when
         creating a class with __metaclass__=PluginMeta that will trigger this.
         """
-        m = importlib.import_module(name)
+        try:
+            m = importlib.import_module(name)
 
-        # Define variables
-        m.Plugin._defineVariables()
-        m.Domain = cls  # Register the domain class for this module
-        # TODO avoid loading bibtex here and make a lazy load like the rest.
-        # Load bibtex
-        m._bibtex = {}
-        bib = cls.__getSubmodule(name, 'bibtex')
-        if bib is not None:
-            if hasattr(bib, "_bibtex"):
-                print("WARNING FOR DEVELOPERS:  %s/%s._bibtex unnecessarily declared. Just the doc string is enough." % (name, "bibtex"))
-            else:
-                try:
-                    m._bibtex = pwutils.LazyDict(lambda: pwutils.parseBibTex(bib.__doc__))
-                except Exception:
-                    pass
-        cls._plugins[name] = m  # Register the name to as a plugin
+            # Define variables
+            m.Plugin._defineVariables()
+            m._pluginInstance = m.Plugin()
+
+            m.Domain = cls  # Register the domain class for this module
+            # TODO avoid loading bibtex here and make a lazy load like the rest.
+            # Load bibtex
+            m._bibtex = {}
+            bib = cls.__getSubmodule(name, 'bibtex')
+            if bib is not None:
+                if hasattr(bib, "_bibtex"):
+                    logger.info("WARNING FOR DEVELOPERS:  %s/%s._bibtex unnecessarily declared. Just the doc string is enough." % (name, "bibtex"))
+                else:
+                    try:
+                        m._bibtex = pwutils.LazyDict(lambda: pwutils.parseBibTex(bib.__doc__))
+                    except Exception:
+                        pass
+            cls._plugins[name] = m  # Register the name to as a plugin
+
+        # Catch any import exception, warn about it but continue.
+        except ModuleNotFoundError:
+            # This is probably due to a priority package like pwchem not being installed
+            pass
+        except Exception as e:
+
+            (pwutils.yellow("WARNING!!: Plugin containing module %s does not import properly. "
+                                 "All its content will be missing in this execution." % name))
+            logger.info("Please, contact developers at %s and send this ugly information below. They'll understand it!." % DOCSITEURLS.CONTACTUS)
+            logger.info(pwutils.yellow(traceback.format_exc()))
 
     @classmethod
     def getPlugins(cls):
         """ Return existing plugins for this Domain. """
         loaded = getattr(cls, '_pluginsLoaded', False)
         if not loaded:  # Load plugin only once
             cls._discoverPlugins()
             cls._pluginsLoaded = True
         return dict(cls._plugins)
 
     @classmethod
     def _discoverPlugins(cls):
+        # Get the list of plugins registered
+        plugin_modules = []
         for entry_point in pkg_resources.iter_entry_points('pyworkflow.plugin'):
-            cls.registerPlugin(entry_point.name)
+            plugin_modules.append(entry_point.name)
+
+        # Sort the list taking into account the priority
+        plugin_modules = sortListByList(plugin_modules, pw.Config.getPriorityPackageList())
+
+        for module in plugin_modules:
+            cls.registerPlugin(module)
+
 
     @classmethod
     def _discoverGUIPlugins(cls):
         for entry_point in pkg_resources.iter_entry_points('pyworkflow.guiplugin'):
             entry_point.load()
 
     @classmethod
@@ -153,15 +185,15 @@
                         module_visit.remove(module)
                         break
                     except Exception as ex:
                         pass
 
     @classmethod
     def __getSubclasses(cls, submoduleName, BaseClass,
-                        updateBaseClasses=False):
+                        updateBaseClasses=False, setPackage=False):
         """ Load all detected subclasses of a given BaseClass.
         Params:
             updateBaseClasses: if True, it will try to load classes from the
                 Domain submodule that was not imported as globals()
         """
         subclasses = getattr(cls, '_%s' % submoduleName)
 
@@ -170,34 +202,39 @@
                 sub = cls.__getSubmodule(cls.getName(), submoduleName)
                 if sub is not None:
                     for name in cls.getModuleClasses(sub):
                         attr = getattr(sub, name)
                         if inspect.isclass(attr) and issubclass(attr, BaseClass):
                             cls._baseClasses[name] = attr
 
-            for pluginName, plugin in cls.getPlugins().items():
+            for pluginName, module in cls.getPlugins().items():
                 sub = cls.__getSubmodule(pluginName, submoduleName)
                 if sub is not None:
                     for name in cls.getModuleClasses(sub):
                         attr = getattr(sub, name)
                         if inspect.isclass(attr) and issubclass(attr, BaseClass):
 
                             # Check if the class already exists (to prevent
                             # naming collisions)
                             if name in subclasses:
                                 # Get already added class plugin
                                 pluginCollision = subclasses[name]._package.__name__
-                                print("ERROR: Name collision (%s) detected "
+                                logger.info("ERROR: Name collision (%s) detected "
                                       "while discovering %s.%s.\n"
                                       " It conflicts with %s" %
                                       (name, pluginName, submoduleName,
                                        pluginCollision))
                             else:
                                 # Set this special property used by Scipion
-                                attr._package = plugin
+                                # Protocols need the package to be set
+                                if setPackage:
+
+                                    attr._plugin = getattr(module, "_pluginInstance", None)
+                                    attr._package = module
+
                                 subclasses[name] = attr
             subclasses.update(
                 pwutils.getSubclasses(BaseClass, cls._baseClasses))
 
         return subclasses
 
     @classmethod
@@ -213,26 +250,31 @@
         for name, declaredClass in inspect.getmembers(module, inspect.isclass):
             if moduleName in declaredClass.__module__:
                 yield name
 
     @classmethod
     def getProtocols(cls):
         """ Return all Protocol subclasses from all plugins for this domain."""
-        return cls.__getSubclasses('protocols', cls._protocolClass)
+        return cls.__getSubclasses('protocols', cls._protocolClass, setPackage=True)
 
     @classmethod
     def getObjects(cls):
         """ Return all EMObject subclasses from all plugins for this domain."""
         return cls.__getSubclasses('objects', cls._objectClass)
 
     @classmethod
+    def viewersLoaded(cls):
+        """ Returns true if viewers have been already discovered"""
+        return len(cls._viewers) != 0
+
+    @classmethod
     def getViewers(cls):
         """ Return all Viewer subclasses from all plugins for this domain."""
         return cls.__getSubclasses('viewers', cls._viewerClass,
-                                   updateBaseClasses=True)
+                                   updateBaseClasses=True, setPackage=True)
 
     @classmethod
     def getWizards(cls):
         """ Return all Wizard subclasses from all plugins for this domain."""
         return cls.__getSubclasses('wizards', cls._wizardClass)
 
     @classmethod
@@ -253,22 +295,28 @@
     @classmethod
     def getName(cls):
         """ Return the name of this Domain. """
         return cls._name
 
     @staticmethod
     def importFromPlugin(module, objects=None, errorMsg='', doRaise=False):
-        """ This method try to import either a list of objects from the
-            module/plugin or the whole module/plugin and returns what is
-            imported if not fails.
-            When the import fails (due to the plugin or the object is not found),
-            it prints a common message + optional errorMsg;
-            or it raise an error with the same message, if doRaise is True.
+        """
+        This method try to import either a list of objects from the
+        module/plugin or the whole module/plugin and returns what is
+        imported if not fails.
+        When the import fails (due to the plugin or the object is not found),
+        it prints a common message + optional errorMsg;
+        or it raise an error with the same message, if doRaise is True.
+
+        :param module: Module name to import
+        :param objects: Optional, string with objects to return present in module
+        :param errorMsg: Optional, extra error message to append to the main message.
+        :param doRaise: If True it will raise an exception instead of tolerating the import error
 
-         -> Usages:
+        Usages::
 
              # Import the whole plugin 'plugin1' as 'plug1'
              plug1 = importFromPlugin('plugin1')
 
              # Import a plugin's module
              pl1Cons = importFromPlugin('plug1.constants')
 
@@ -335,19 +383,18 @@
             try:
                 viewerModule, viewerClassName = prefViewerStr.rsplit('.', 1)
                 prefViewer = cls.importFromPlugin(viewerModule,
                                                   viewerClassName,
                                                   doRaise=True)
                 viewers.append(prefViewer)
             except Exception as e:
-                print("Couldn't load \"%s\" as preferred viewer.\n"
+                logger.error("Couldn't load \"%s\" as preferred viewer for %s.\n"
                       "There might be a typo in your VIEWERS variable "
                       "or an error in the viewer's plugin installation"
-                      % prefViewerStr)
-                print(e)
+                      % (prefViewerStr, className), exc_info=e)
         return viewers
 
     @classmethod
     def findViewers(cls, className, environment):
         """ Find the available viewers in this Domain for this class. """
         viewers = []
         try:
@@ -375,32 +422,33 @@
             # Catch if there is a missing plugin, we will get Legacy which triggers and Exception
             pass
 
         return viewers
 
     @classmethod
     def findWizards(cls, protocol, environment):
-        """ Find available wizards for this class, in this Domain.
-        Params:
-            protocols: Protocol instance for which wizards will be search.
-            environment: The environment name for wizards (e.g TKINTER)
-        Returns:
-            a dict with the paramName and wizards for this class."""
+        """
+        Find available wizards for this class, in this Domain.
+
+        :param protocol: Protocol instance for which wizards will be search.
+        :param environment: The environment name for wizards (e.g TKINTER)
+
+        :return A dict with the paramName and wizards for the protocol passed."""
         return cls.__findWizardsFromDict(protocol, environment,
                                          cls.getWizards())
 
     @classmethod
     def printInfo(cls):
         """ Simple function (mainly for debugging) that prints basic
         information about this Domain. """
-        print("Domain: %s" % cls._name)
-        print("     objects: %s" % len(cls._objects))
-        print("   protocols: %s" % len(cls._protocols))
-        print("     viewers: %s" % len(cls._viewers))
-        print("     wizards: %s" % len(cls._wizards))
+        logger.info("Domain: %s" % cls._name)
+        logger.info("     objects: %s" % len(cls._objects))
+        logger.info("   protocols: %s" % len(cls._protocols))
+        logger.info("     viewers: %s" % len(cls._viewers))
+        logger.info("     wizards: %s" % len(cls._wizards))
 
     # ---------- Private methods of Domain class ------------------------------
     @staticmethod
     def __pluginNotFound(plugName, errorMsg='', doRaise=False):
         """ Prints or raise (depending on the doRaise) telling why it is failing
         """
         hint = ("   Check the plugin manager (Configuration->Plugins in "
@@ -435,15 +483,15 @@
             line = stackList[callIdx][1]
             calling = "  Called by %s, line %s" % (callBy, line)
 
         raiseMsg = "%s\n %s\n%s\n" % (msgStr, calling, hint)
         if doRaise:
             raise Exception("\n\n" + raiseMsg)
         else:
-            print(raiseMsg)
+            logger.info(raiseMsg)
 
     @staticmethod
     def __getSubmodule(name, subname):
         try:
             completeModuleText = '%s.%s' % (name, subname)
             if pwutils.isModuleAFolder(name):
                 return importlib.import_module(completeModuleText)
@@ -477,40 +525,44 @@
 class Plugin:
     __metaclass__ = ABCMeta
 
     _vars = {}
     _homeVar = ''  # Change in subclasses to define the "home" variable
     _pathVars = []
     _supportedVersions = []
-    _name = ""
     _url = ""  # For the plugin
     _condaActivationCmd = None
 
+    def __init__(self):
+        self._path = None
+        self._inDevelMode = None
+        self._name = None
+
     @classmethod
     def _defineVar(cls, varName, defaultValue):
         """ Internal method to define variables trying to get it from the environment first. """
         cls._addVar(varName, os.environ.get(varName, defaultValue))
 
     @classmethod
     def _addVar(cls, varName, value):
         """ Adds a variable to the local variable dictionary directly. Avoiding the environment"""
         cls._vars[varName] = value
 
     @classmethod
     @abstractmethod
     def getEnviron(cls):
-        """ Setup the environment variables needed to launch programs. """
+        """ Set up the environment variables needed to launch programs. """
         pass
 
     @classmethod
     def getCondaActivationCmd(cls):
         if cls._condaActivationCmd is None:
-            condaActivationCmd = os.environ.get(CONDA_ACTIVATION_CMD_VAR, "")
+            condaActivationCmd = pw.Config.CONDA_ACTIVATION_CMD
             if not condaActivationCmd:
-                print("WARNING!!_condaActivationCmd: %s variable not defined. "
+                logger.info("WARNING!!_condaActivationCmd: %s variable not defined. "
                       "Relying on conda being in the PATH" % CONDA_ACTIVATION_CMD_VAR)
             elif condaActivationCmd[-1] not in [";", "&"]:
                 condaActivationCmd += "&&"
 
             cls._condaActivationCmd = condaActivationCmd
 
         return cls._condaActivationCmd
@@ -553,86 +605,107 @@
     @classmethod
     def getSupportedVersions(cls):
         """ Return the list of supported binary versions. """
         return cls._supportedVersions
 
     @classmethod
     def getActiveVersion(cls, home=None, versions=None):
-        """ Return the version of the binaries that are currently active.
-        In the current implementation it will be inferred from the *_HOME
+        """
+        Returns the version of the binaries that are currently active.
+        In the current implementation it will be inferred from the \*_HOME
         variable, so it should contain the version number in it. """
+
         # FIXME: (JMRT) Use the basename might alleviate the issue with matching
         # the binaries version, but we might consider to find a better solution
         home = os.path.basename(home or cls.getHome())
         versions = versions or cls.getSupportedVersions()
 
         for v in versions:
             if v in home:
                 return v
 
         return ''
 
     @classmethod
-    def getName(cls):
-        return cls.__module__
-
-    @classmethod
     def validateInstallation(cls):
         """
         Check if the binaries are properly installed and if not, return
         a list with the error messages.
 
         The default implementation will check if the _pathVars exists.
         """
         try:
             missing = ["%s: %s" % (var, cls.getVar(var))
                        for var in cls._pathVars if not os.path.exists(cls.getVar(var))]
 
-            return (["Missing variables:"] + missing) if missing else []
+            return (["Missing paths: the variables below point to non existing paths."]
+                    + missing + [
+                     "Either install the software ( %s )" % DOCSITEURLS.PLUGIN_MANAGER,
+                    "or edit the config file ( %s )" % DOCSITEURLS.CONFIG]) if missing else []
         except Exception as e:
             return ["validateInstallation fails: %s" % e]
 
     @classmethod
-    def getPluginTemplateDir(cls):
-        return os.path.join(pw.getModuleFolder(cls.getName()), 'templates')
+    def getUrl(cls, protClass=None):
+        """ Url for the plugin to point users to it"""
+        return cls._url
 
-    @classmethod
-    def getTemplates(cls):
+    # -------------- Instance methods ----------------
+    def getName(self):
+        if self._name is None:
+            self._name=  self.__class__.__module__
+
+        return self._name
+
+    def getPluginDir(self):
+        return self.getPath()
+
+    def getPluginTemplateDir(self):
+        return os.path.join(self.getPath(), 'templates')
+
+
+    def getTemplates(self):
         """ Get the plugin templates from the templates directory.
             If more than one template is found or passed, a dialog is raised
             to choose one.
         """
         tempList = []
-        pluginName = cls.getName()
-        tDir = cls.getPluginTemplateDir()
+        pluginName = self.getName()
+        tDir = self.getPluginTemplateDir()
         if os.path.exists(tDir):
             for file in glob.glob1(tDir, "*" + SCIPION_JSON_TEMPLATES):
                 t = Template(pluginName, os.path.join(tDir, file))
                 tempList.append(t)
 
         return tempList
 
-    @classmethod
-    def getUrl(cls, protClass=None):
-        """ Url for the plugin to point users to it"""
-        return cls._url
+    def getPath(self):
+        if self._path is None:
+            self._path = sys.modules[self.__class__.__module__].__path__[0]
+
+        return self._path
+    def inDevelMode(self)-> bool:
+        """ Returns true if code is not in python's site-packages folder"""
+        if self._inDevelMode is None:
+            self._inDevelMode = pwutils.getPythonPackagesFolder() not in self.getPath()
+        return self._inDevelMode
 
 
 class PluginInfo:
     """
     Information related to a given plugin when it is installed via PIP
     """
     def __init__(self, name):
         try:
             dist = pkg_resources.get_distribution(name)
             lines = [l for l in dist._get_metadata(dist.PKG_INFO)]
             tuples = message_from_string('\n'.join(lines))
 
         except Exception:
-            print("Plugin %s seems is not a pip module yet. "
+            logger.info("Plugin %s seems is not a pip module yet. "
                   "No metadata found" % name)
             tuples = message_from_string('Author: plugin in development mode?')
 
         self._name = name
         self._metadata = OrderedDict()
 
         for v in tuples.items():
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/project/__init__.py` & `scipion-pyworkflow-3.1.0/pyworkflow/project/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/project/config.py` & `scipion-pyworkflow-3.1.0/pyworkflow/project/config.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,37 +20,34 @@
 # * along with this program.  If not, see <https://www.gnu.org/licenses/>.
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-
-import os
+import logging
+logger = logging.getLogger(__name__)
 import json
 import datetime as dt
-from collections import OrderedDict
-from configparser import ConfigParser
 
-import pyworkflow as pw
 import pyworkflow.object as pwobj
 from pyworkflow.mapper import SqliteMapper
-from pyworkflow.utils import isModuleAFolder
 
 
-class ProjectSettings(pwobj.OrderedObject):
+class ProjectSettings(pwobj.Object):
     """ Store settings related to a project. """
 
     COLOR_MODE_STATUS = 0
     COLOR_MODE_LABELS = 1
     COLOR_MODE_AGE = 2
-    COLOR_MODES = (COLOR_MODE_STATUS, COLOR_MODE_LABELS, COLOR_MODE_AGE)
+    COLOR_MODE_SIZE = 3
+    COLOR_MODES = (COLOR_MODE_STATUS, COLOR_MODE_LABELS, COLOR_MODE_AGE, COLOR_MODE_SIZE)
 
     def __init__(self, confs={}, **kwargs):
-        pwobj.OrderedObject.__init__(self, **kwargs)
+        super().__init__(**kwargs)
         self.config = ProjectConfig()
         # Store the current view selected by the user
         self.currentProtocolsView = pwobj.String()
         # Store the color mode: 0= Status, 1=Labels, ...
         self.colorMode = pwobj.Integer(ProjectSettings.COLOR_MODE_STATUS)
         # Store graph nodes positions and other info
         self.nodeList = NodeConfigList()
@@ -126,14 +123,17 @@
 
     def labelsColorMode(self):
         return self.getColorMode() == self.COLOR_MODE_LABELS
 
     def ageColorMode(self):
         return self.getColorMode() == self.COLOR_MODE_AGE
 
+    def sizeColorMode(self):
+        return self.getColorMode() == self.COLOR_MODE_SIZE
+
     def write(self, dbPath=None):
         self.setName('ProjectSettings')
         if dbPath is not None:
             self.mapper = SqliteMapper(dbPath, globals())
         else:
             if self.mapper is None:
                 raise Exception("Can't write ProjectSettings without "
@@ -142,20 +142,51 @@
         self.mapper.deleteAll()
         self.mapper.insert(self)
         self.mapper.commit()
 
     def getNodes(self):
         return self.nodeList
 
+    def cleanUpNodes(self, runsIds, toRemove=True):
+        """ This will clean up all the nodes that do not have a matching run.
+        This is because until now, the nodes here weren't removes when protocols were removed.
+
+        :param runsIds: iterable with protocol's objId to be removed.
+        :param toRemove: Passed is are to be removed. Otherwise, are the ones to keep
+        """
+
+        try:
+            logger.info("Cleaning up unused graphical nodes.")
+
+            nodesToDelete = []
+            for node  in self.getNodes():
+                nodeId = str(node.getId())
+                # if it is not the root node
+                if nodeId != '0':
+
+                    if (nodeId in runsIds) == toRemove:
+                        nodesToDelete.append(node.getId())
+
+            logger.info("Following graphical nodes %s unmatched. Deleting them" % nodesToDelete)
+            for key in nodesToDelete:
+                self.getNodes().removeNode(key)
+                
+        except Exception as e:
+            logger.error("Couldn't clean up graphical nodes.", exc_info=e)
+
     def getNodeById(self, nodeId):
         return self.nodeList.getNode(nodeId)
 
     def addNode(self, nodeId, **kwargs):
         return self.nodeList.addNode(nodeId, **kwargs)
 
+    def removeNode(self, nodeId):
+        """ Removes a graphical node based on its id"""
+        self.nodeList.removeNode(nodeId)
+
     def getLabels(self):
         return self.labelsList
 
     @classmethod
     def load(cls, dbPath):
         """ Load a ProjectSettings from dbPath. """
         classDict = dict(globals())
@@ -172,47 +203,48 @@
 
         settings = settingList[0]
         settings.mapper = mapper
 
         return settings
 
 
-class ProjectConfig(pwobj.OrderedObject):
+class ProjectConfig(pwobj.Object):
     """A simple base class to store ordered parameters"""
 
     def __init__(self, **args):
-        pwobj.OrderedObject.__init__(self, **args)
-        self.logo = pwobj.String('scipion_logo_small.gif')
+        super().__init__(**args)
+        self.logo = pwobj.String('scipion_logo_small.png')
         # Do not store this object, unless we implement some kind of
         # icon customization
         self._objDoStore = False
 
 
 class MenuConfig(object):
     """Menu configuration in a tree fashion.
-    Each menu can contains submenus.
+    Each menu can contain submenus.
     Leaf elements can contain actions"""
 
     def __init__(self, text=None, value=None,
-                 icon=None, tag=None, **kwargs):
+                 icon=None, tag=None, shortCut=None, openItem=False, visible=True):
         """Constructor for the Menu config item.
         Arguments:
           text: text to be displayed
           value: internal value associated with the item.
           icon: display an icon with the item
           tag: put some tags to items
         **args: pass other options to base class.
         """
-        self.text = pwobj.String(text)
-        self.value = pwobj.String(value)
-        self.icon = pwobj.String(icon)
-        self.tag = pwobj.String(tag)
-        self.shortCut = pwobj.String(kwargs.get('shortCut', None))
+        self.text = text
+        self.value = value
+        self.icon = icon
+        self.tag = tag
+        self.shortCut = shortCut
+        self.openItem = openItem
+        self.visible = visible
         self.childs = pwobj.List()
-        self.openItem = pwobj.Boolean(kwargs.get('openItem', False))
 
     def addSubMenu(self, text, value=None, **args):
         subMenu = type(self)(text, value, **args)
         self.childs.append(subMenu)
         return subMenu
 
     def __iter__(self):
@@ -225,22 +257,24 @@
     def isEmpty(self):
         return len(self.childs) == 0
 
 
 class NodeConfig(pwobj.Scalar):
     """ Store Graph node information such as x, y. """
 
-    def __init__(self, nodeId=0, x=None, y=None, selected=False, expanded=True):
+    def __init__(self, nodeId=0, x=None, y=None, selected=False, expanded=True,
+                 visible=True):
         pwobj.Scalar.__init__(self)
         # Special node id 0 for project node
         self._values = {'id': nodeId,
                         'x': pwobj.Integer(x).get(0),
                         'y': pwobj.Integer(y).get(0),
                         'selected': selected,
                         'expanded': expanded,
+                        'visible': pwobj.Boolean(visible).get(0),
                         'labels': []}
 
     def _convertValue(self, value):
         """Value should be a str with comma separated values
         or a list.
         """
         self._values = json.loads(value)
@@ -282,14 +316,22 @@
 
     def setExpanded(self, expanded):
         self._values['expanded'] = expanded
 
     def isExpanded(self):
         return self._values['expanded']
 
+    def setVisible(self, visible):
+        self._values['visible'] = visible
+
+    def isVisible(self):
+        if self._values.get('visible') is None:
+            self._values['visible'] = True
+        return self._values['visible']
+
     def setLabels(self, labels):
         self._values['labels'] = labels
 
     def getLabels(self):
         return self._values.get('labels', None)
 
     def __str__(self):
@@ -311,14 +353,20 @@
 
     def addNode(self, nodeId, **kwargs):
         node = NodeConfig(nodeId, **kwargs)
         self._nodesDict[node.getId()] = node
         self.append(node)
         return node
 
+    def removeNode(self, nodeId):
+        """ Removes a node with the id = nodeId"""
+        nodeToRemove = self._nodesDict[nodeId]
+        self._nodesDict.pop(nodeId)
+        self.remove(nodeToRemove)
+
     def updateDict(self):
         self._nodesDict.clear()
         for node in self:
             self._nodesDict[node.getId()] = node
 
     def clear(self):
         pwobj.List.clear(self)
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/project/manager.py` & `scipion-pyworkflow-3.1.0/pyworkflow/project/manager.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/project/project.py` & `scipion-pyworkflow-3.1.0/pyworkflow/project/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,42 +20,46 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+import logging
+
+ROOT_NODE_NAME = "PROJECT"
+logger = logging.getLogger(__name__)
 
 import datetime as dt
 import json
 import os
 import re
 import time
 import traceback
 from collections import OrderedDict
 
 import pyworkflow as pw
+from pyworkflow.constants import PROJECT_DBNAME, PROJECT_SETTINGS
 import pyworkflow.object as pwobj
 import pyworkflow.protocol as pwprot
 import pyworkflow.utils as pwutils
 from pyworkflow.mapper import SqliteMapper
-from pyworkflow.protocol.constants import (MODE_RESTART, MODE_CONTINUE,
-                                           STATUS_INTERACTIVE, ACTIVE_STATUS, UNKNOWN_JOBID)
+from pyworkflow.protocol.constants import (MODE_RESTART, MODE_RESUME,
+                                           STATUS_INTERACTIVE, ACTIVE_STATUS,
+                                           UNKNOWN_JOBID, INITIAL_SLEEP_TIME)
 from pyworkflow.protocol.protocol import ProtImportBase
 
 from . import config
 
 
 OBJECT_PARENT_ID = pwobj.OBJECT_PARENT_ID
-PROJECT_DBNAME = 'project.sqlite'
 PROJECT_LOGS = 'Logs'
 PROJECT_RUNS = 'Runs'
 PROJECT_TMP = 'Tmp'
 PROJECT_UPLOAD = 'Uploads'
-PROJECT_SETTINGS = 'settings.sqlite'
 PROJECT_CONFIG = '.config'
 PROJECT_CREATION_TIME = 'CreationTime'
 
 # Regex to get numbering suffix and automatically propose runName
 REGEX_NUMBER_ENDING = re.compile('(?P<prefix>.+)(?P<number>\(\d*\))\s*$')
 REGEX_NUMBER_ENDING_CP = re.compile('(?P<prefix>.+\s\(copy)(?P<number>.*)\)\s*$')
 
@@ -210,36 +214,37 @@
         classesDict = pwobj.Dict(default=pwprot.LegacyProtocol)
         classesDict.update(self._domain.getMapperDict())
         classesDict.update(config.__dict__)
         return SqliteMapper(sqliteFn, classesDict)
 
     def load(self, dbPath=None, hostsConf=None, protocolsConf=None, chdir=True,
              loadAllConfig=True):
-        """ Load project data, configuration and settings.
-        Params:
-            dbPath: the path to the project database.
-                If None, use the project.sqlite in the project folder.
-            hosts: where to read the host configuration. 
-                If None, check if exists in .config/hosts.conf
-                or read from ~/.config/scipion/hosts.conf
-            settings: where to read the settings.
-                If None, use the settings.sqlite in project folder.
-                If forProtocol is True, the settings and protocols.conf will
-                not be loaded.
+        """
+        Load project data, configuration and settings.
+
+        :param dbPath: the path to the project database.
+            If None, use the project.sqlite in the project folder.
+        :param hostsConf: where to read the host configuration.
+            If None, check if exists in .config/hosts.conf
+            or read from ~/.config/scipion/hosts.conf
+        :param protocolsConf: Not used
+        :param chdir: If True, os.cwd will be set to project's path.
+        :param loadAllConfig: If True, settings from settings.sqlite will also be loaded
+
         """
 
         if not os.path.exists(self.path):
             raise Exception("Cannot load project, path doesn't exist: %s"
                             % self.path)
 
         # If folder is read only, flag it and warn about it.
         if not os.access(self.path, os.W_OK):
             self._isInReadOnlyFolder = True
-            print("WARNING on project \"%s\": don't have write permissions "
-                  "for project folder. Loading as READ-ONLY." % self.shortName)
+            logger.warning("Project \"%s\": you don't have write permissions "
+                  "for project folder. Loading asd READ-ONLY." % self.shortName)
 
         if chdir:
             os.chdir(self.path)  # Before doing nothing go to project dir
 
         try:
             self._loadDb(dbPath)
             self._loadHosts(hostsConf)
@@ -248,34 +253,34 @@
 
                 # FIXME: Handle settings argument here
 
                 # It is possible that settings does not exists if
                 # we are loading a project after a Project.setDbName,
                 # used when running protocols
                 settingsPath = os.path.join(self.path, self.settingsPath)
-                if pw.Config.debugOn():
-                    print("settingsPath: %s" % settingsPath)
+
+                logger.debug("settingsPath: %s" % settingsPath)
 
                 if os.path.exists(settingsPath):
                     self.settings = config.ProjectSettings.load(settingsPath)
                 else:
-                    print("settings is None")
+                    logger.info("settings is None")
                     self.settings = None
 
             self._loadCreationTime()
 
         # Catch DB not found exception (when loading a project from a folder
         #  without project.sqlite
         except MissingProjectDbException as noDBe:
             # Raise it at before: This is a critical error and should be raised
             raise noDBe
 
         # Catch any less severe exception..to allow at least open the project.
         # except Exception as e:
-        #     print("ERROR: Project %s load failed.\n"
+        #     logger.info("ERROR: Project %s load failed.\n"
         #           "       Message: %s\n" % (self.path, e))
 
     def _loadCreationTime(self):
         # Load creation time, it should be in project.sqlite or
         # in some old projects it is found in settings.sqlite
 
         creationTime = self.mapper.selectBy(name=PROJECT_CREATION_TIME)
@@ -334,35 +339,37 @@
         return list(self._hosts.keys())
 
     def getHostConfig(self, hostName):
         if hostName in self._hosts:
             hostKey = hostName
         else:
             hostKey = self.getHostNames()[0]
-            print("PROJECT: Warning, protocol host '%s' not found." % hostName)
-            print("         Using '%s' instead." % hostKey)
+            logger.warning("Protocol host '%s' not found." % hostName)
+            logger.warning("         Using '%s' instead." % hostKey)
 
         return self._hosts[hostKey]
 
     def getProtocolView(self):
         """ Returns de view selected in the tree when it was persisted"""
         return self.settings.getProtocolView()
 
     def create(self, runsView=1, readOnly=False, hostsConf=None,
                protocolsConf=None):
         """Prepare all required paths and files to create a new project.
-        Params:
-         hosts: a list of configuration hosts associated to this projects
-               (class ExecutionHostConfig)
+
+        :param runsView: default view to associate the project with
+        :param readOnly: If True, project will be loaded as read only.
+        :param hostsConf: Path to the host.conf to be used when executing protocols
+        :param protocolsConf: Not used.
         """
         # Create project path if not exists
         pwutils.path.makePath(self.path)
         os.chdir(self.path)  # Before doing nothing go to project dir
         self._cleanData()
-        print("Creating project at: ", os.path.abspath(self.dbPath))
+        logger.info("Creating project at %s" % os.path.abspath(self.dbPath))
         # Create db through the mapper
         self.mapper = self.createMapper(self.dbPath)
         # Store creation time
         self._storeCreationTime(dt.datetime.now())
         # Load settings from .conf files and write .sqlite
         self.settings = self.createSettings(runsView=runsView,
                                             readOnly=readOnly)
@@ -401,42 +408,47 @@
                                 the  database
                        1.1.1.2 Change the protocol status (SAVED)
                        1.1.1.3 Schedule the protocol
                    Else Restart the workflow from that point (RESTART ACTION) if
                    at least one protocol in streaming has been launched
         """
         if continuedProtList is not None:
-            for protocolId in continuedProtList:
-                protocol = self.getProtocol(protocolId)
+            for protocol, level in continuedProtList.values():
                 if not protocol.isInteractive():
+                    if protocol.isScheduled():
+                        continue
                     if protocol.worksInStreaming():
                         attrSet = [attr for name, attr in
                                    protocol.iterOutputAttributes(pwprot.Set)]
                         try:
                             if attrSet:
                                 for attr in attrSet:
                                     attr.setStreamState(attr.STREAM_OPEN)
                                     attr.write()
                                     attr.close()
                             protocol.setStatus(pwprot.STATUS_SAVED)
-                            protocol._setStatusSteps(pwprot.STATUS_SAVED)
+                            protocol._updateSteps(lambda step: step.setStatus(pwprot.STATUS_SAVED))
                             protocol.setMapper(self.createMapper(protocol.getDbPath()))
                             protocol._store()
                             self._storeProtocol(protocol)
-                            self.scheduleProtocol(protocol)
+                            self.scheduleProtocol(protocol,
+                                                  initialSleepTime=level*INITIAL_SLEEP_TIME)
                         except Exception as ex:
                             errorsList.append("Error trying to launch the "
                                               "protocol: %s\nERROR: %s\n" %
                                               (protocol.getObjLabel(), ex))
                             break
                     else:
-                        if protocolId != continuedProtList[0]:
+                        if level != 0:
                             # we make sure that at least one protocol in streaming
                             # has been launched
-                            self._restartWorkflow([protocolId], errorsList)
+                            if protocol.isActive():
+                                self.stopProtocol(protocol)
+                            self._restartWorkflow({protocol.getObjId(): (protocol, level)},
+                                                  errorsList)
 
                         else:
                             errorsList.append(("Error trying to launch the "
                                                "protocol: %s\nERROR: The protocol is "
                                                "not in streaming" %
                                                (protocol.getObjLabel())))
                             break
@@ -448,20 +460,24 @@
         Actions done here are:
         1. Set the protocol run mode (RESTART). All previous results will be
            deleted
         2. Schedule the protocol if not is an interactive protocol
         3. For each of the dependents protocols, repeat from step 1
         """
         if restartedProtList is not None:
-            for protocolId in restartedProtList:
-                protocol = self.getProtocol(protocolId)
+            for protocol, level in restartedProtList.values():
                 if not protocol.isInteractive():
                     try:
+                        if protocol.isScheduled():
+                            continue
+                        elif protocol.isActive():
+                            self.stopProtocol(protocol)
                         protocol.runMode.set(MODE_RESTART)
-                        self.scheduleProtocol(protocol)
+                        self.scheduleProtocol(protocol,
+                                              initialSleepTime=level*INITIAL_SLEEP_TIME)
                     except Exception as ex:
                         errorsList.append("Error trying to restart a protocol: %s"
                                           "\nERROR: %s\n" % (protocol.getObjLabel(),
                                                              ex))
                         break
                 else:
                     protocol.setStatus(pwprot.STATUS_SAVED)
@@ -471,105 +487,106 @@
                     protocol.makePathsAndClean()  # Create working dir if necessary
                     # Delete the relations created by this protocol
                     self.mapper.deleteRelations(self)
                     self.mapper.commit()
                     self.mapper.store(protocol)
                     self.mapper.commit()
 
-    def _fixWorkflowConfiguration(self, protocolList=None):
+    def _fixProtParamsConfiguration(self, protocol=None):
         """
         This function fix:
-        1. The old parameters configuration in the protocols list.
+        1. The old parameters configuration in the protocols.
            Now, dependent protocols have a pointer to the parent protocol, and
            the extended parameter has a parent output value
         """
-        if protocolList is not None:
-            for protocolId in protocolList:
-                protocol = self.getProtocol(protocolId)
-
-                # Take the old configuration attributes and fix the pointer
-                oldStylePointerList = [item for key, item in
-                                       protocol.iterInputAttributes()
-                                       if not isinstance(item.getObjValue(),
-                                                         pwprot.Protocol)]
-                if oldStylePointerList:
-                    # Fix the protocol parameters
-                    for pointer in oldStylePointerList:
-                        auxPointer = pointer.getObjValue()
-                        pointer.set(self.getProtocol(pointer.get().getObjParentId()))
-                        pointer.setExtended(auxPointer.getLastName())
-                        protocol._store()
-                        self._storeProtocol(protocol)
-                        self._updateProtocol(protocol)
-                        self.mapper.commit()
-                        print("The parameters configuration in the "
-                              "protocol \"%s\" has been modified \n" %
-                              protocol.getObjLabel())
+        # Take the old configuration attributes and fix the pointer
+        oldStylePointerList = [item for key, item in
+                               protocol.iterInputAttributes()
+                               if not isinstance(item.getObjValue(),
+                                                 pwprot.Protocol)]
+        if oldStylePointerList:
+            # Fix the protocol parameters
+            for pointer in oldStylePointerList:
+                auxPointer = pointer.getObjValue()
+                pointer.set(self.getRunsGraph().getNode(str(pointer.get().getObjParentId())).run)
+                pointer.setExtended(auxPointer.getLastName())
+                protocol._store()
+                self._storeProtocol(protocol)
+                self._updateProtocol(protocol)
+                self.mapper.commit()
 
-    def stopWorkFlow(self, initialProtocol):
+    def stopWorkFlow(self, activeProtList):
         """
         This function can stop a workflow from a selected protocol
         :param initialProtocol: selected protocol
         """
-        if initialProtocol:
-            errorsList, workflowProtocolList = self._checkWorkflowErrors(initialProtocol)
-            for protocolId in workflowProtocolList:
-                protocol = self.getProtocol(protocolId)
-                if protocol.getStatus() in ACTIVE_STATUS:
-                    try:
-                        self.stopProtocol(protocol)
-                    except Exception as err:
-                        print(err)
+        errorProtList = []
+        for protocol in activeProtList.values():
+            try:
+                self.stopProtocol(protocol)
+            except Exception:
+                errorProtList.append(protocol)
+        return errorProtList
 
-    def resetWorkFlow(self, initialProtocol):
+    def resetWorkFlow(self, workflowProtocolList):
         """
         This function can reset a workflow from a selected protocol
         :param initialProtocol: selected protocol
         """
-        if initialProtocol:
-            errorsList, workflowProtocolList = self._checkWorkflowErrors(initialProtocol)
-            for protocolId in workflowProtocolList:
-                protocol = self.getProtocol(protocolId)
-                try:
-                    self.resetProtocol(protocol)
-                except Exception as err:
-                    print(err)
+        errorProtList = []
+        if workflowProtocolList:
+            for protocol, level in workflowProtocolList.values():
+                if protocol.getStatus() != pwprot.STATUS_SAVED:
+                    try:
+                        self.resetProtocol(protocol)
+                    except Exception:
+                        errorProtList.append(protocol)
+        return errorProtList
 
-    def launchWorkflow(self, initialProtocol, mode=MODE_CONTINUE):
+    def launchWorkflow(self, workflowProtocolList, mode=MODE_RESUME):
         """
         This function can launch a workflow from a selected protocol in two
         modes depending on the 'mode' value (RESTART, CONTINUE)
         Actions done here are:
+
         1. Check if the workflow has active protocols.
         2. Fix the workflow if is not properly configured
         3. Restart or Continue a workflow starting from the protocol depending
-           of the 'mode' value
+            on the 'mode' value
+
         """
-        if initialProtocol:
-            errorsList, workflowProtocolList = self._checkWorkflowErrors(initialProtocol)
-            if not errorsList:
-                self._fixWorkflowConfiguration(workflowProtocolList)
-                if mode == MODE_RESTART:
-                    self._restartWorkflow(workflowProtocolList, errorsList)
-                else:
-                    self._continueWorkflow(workflowProtocolList, errorsList)
-            return errorsList
+        errorsList = []
+        if mode == MODE_RESTART:
+            self._restartWorkflow(workflowProtocolList, errorsList)
+        else:
+            self._continueWorkflow(workflowProtocolList, errorsList)
+        return errorsList
 
     def launchProtocol(self, protocol, wait=False, scheduled=False,
                        force=False):
         """ In this function the action of launching a protocol
         will be initiated. Actions done here are:
+
         1. Store the protocol and assign name and working dir
         2. Create the working dir and also the protocol independent db
         3. Call the launch method in protocol.job to handle submission:
-           mpi, thread, queue,
-        and also take care if the execution is remotely.
+            mpi, thread, queue,
+            and also take care if the execution is remotely.
 
         If the protocol has some prerequisites (other protocols that
         needs to be finished first), it will be scheduled.
+
+        :param protocol: Protocol instance to launch
+        :param wait: Optional. If true, this method
+            will wait until execution is finished. Used in tests.
+        :param scheduled: Optional. If true, run.db and paths
+            already exist and are preserved.
+        :param force: Optional. If true, launch is forced, regardless
+            latter dependent executions. Used when restarting many protocols a once.
+
         """
         if protocol.getPrerequisites() and not scheduled:
             return self.scheduleProtocol(protocol)
 
         isRestart = protocol.getRunMode() == MODE_RESTART
 
         if not force:
@@ -603,21 +620,24 @@
         # Commit changes
         if wait:  # This is only useful for launching tests...
             self._updateProtocol(protocol)
         else:
             self.mapper.store(protocol)
         self.mapper.commit()
 
-    def scheduleProtocol(self, protocol, prerequisites=[]):
+    def scheduleProtocol(self, protocol, prerequisites=[], initialSleepTime=0):
         """ Schedule a new protocol that will run when the input data
         is available and the prerequisites are finished.
-        Params:
-            protocol: the protocol that will be scheduled.
-            prerequisites: a list with protocols ids that the scheduled
-                protocol will wait for.
+
+        :param protocol: the protocol that will be scheduled.
+        :param prerequisites: a list with protocols ids that the scheduled
+            protocol will wait for.
+        :param initialSleepTime: number of seconds to wait before
+            checking input's availability
+
         """
         isRestart = protocol.getRunMode() == MODE_RESTART
 
         protocol.setStatus(pwprot.STATUS_SCHEDULED)
         protocol.addPrerequisites(*prerequisites)
 
         self._setupProtocol(protocol)
@@ -628,52 +648,50 @@
         self.mapper.commit()
 
         # Prepare a separate db for this run
         # NOTE: now we are simply copying the entire project db, this can be
         # changed later to only create a subset of the db need for the run
         pwutils.path.copyFile(self.dbPath, protocol.getDbPath())
         # Launch the protocol, the jobId should be set after this call
-        pwprot.schedule(protocol)
+        pwprot.schedule(protocol, initialSleepTime=initialSleepTime)
         self.mapper.store(protocol)
         self.mapper.commit()
 
     def _updateProtocol(self, protocol, tries=0, checkPid=False,
                         skipUpdatedProtocols=True):
 
         # If this is read only exit
         if self.openedAsReadOnly():
-            return
-
-        if skipUpdatedProtocols:
-            # If we are already updated, comparing timestamps
-            if pwprot.isProtocolUpToDate(protocol):
-                return
+            return pw.NOT_UPDATED_READ_ONLY
 
         try:
+
             # Backup the values of 'jobId', 'label' and 'comment'
             # to be restored after the .copy
             jobId = protocol.getJobId()
             label = protocol.getObjLabel()
             comment = protocol.getObjComment()
 
-            # Capture the db timestamp before loading.
-            lastUpdateTime = pwutils.getFileLastModificationDate(
-                                                        protocol.getDbPath())
+            if skipUpdatedProtocols:
+                # If we are already updated, comparing timestamps
+                if pwprot.isProtocolUpToDate(protocol):
+                    return pw.NOT_UPDATED_UNNECESSARY
+
 
             # If the protocol database has ....
             #  Comparing date will not work unless we have a reliable
             # lastModificationDate of a protocol in the project.sqlite
             # TODO: when launching remote protocols, the db should be
             # TODO: retrieved in a different way.
             prot2 = pwprot.getProtocolFromDb(self.path,
                                              protocol.getDbPath(),
                                              protocol.getObjId())
 
-            if checkPid:
-                self.checkPid(prot2)
+            # Capture the db timestamp before loading.
+            lastUpdateTime = pwutils.getFileLastModificationDate(protocol.getDbPath())
 
             # Copy is only working for db restored objects
             protocol.setMapper(self.mapper)
 
             localOutputs = list(protocol._outputs)
             protocol.copy(prot2, copyId=False, excludeInputs=True)
 
@@ -684,49 +702,62 @@
                     protocol._outputs.append(attr)
 
             # Restore backup values
             protocol.setJobId(jobId)
             protocol.setObjLabel(label)
             protocol.setObjComment(comment)
             # Use the run.db timestamp instead of the system TS to prevent
-            # possible inconsistencies
-            # protocol.lastUpdateTimeStamp.set(datetime.datetime.now())
+            # possible inconsistencies.
             protocol.lastUpdateTimeStamp.set(lastUpdateTime)
 
+            # Check pid at the end, once updated
+            if checkPid:
+                self.checkPid(protocol)
+
+
             self.mapper.store(protocol)
 
             # Close DB connections
             prot2.getProject().closeMapper()
             prot2.closeMappers()
 
         except Exception as ex:
-            print("Error trying to update protocol: %s(jobId=%s)\n "
-                  "ERROR: %s, tries=%d"
-                  % (protocol.getObjName(), jobId, ex, tries))
             if tries == 3:  # 3 tries have been failed
                 traceback.print_exc()
                 # If any problem happens, the protocol will be marked
                 # with a FAILED status
-                protocol.setFailed(str(ex))
-                self.mapper.store(protocol)
+                try:
+                    protocol.setFailed(str(ex))
+                    self.mapper.store(protocol)
+                except Exception:
+                    pass
+                return pw.NOT_UPDATED_ERROR
             else:
+                logger.warning("Couldn't update protocol %s(jobId=%s) from it's own database. ERROR: %s, attempt=%d"
+                             % (protocol.getObjName(), jobId, ex, tries))
                 time.sleep(0.5)
                 self._updateProtocol(protocol, tries + 1)
 
+
+        return pw.PROTOCOL_UPDATED
+
     def stopProtocol(self, protocol):
         """ Stop a running protocol """
         try:
-            pwprot.stop(protocol)
-        except Exception:
+            if protocol.getStatus() in ACTIVE_STATUS:
+                pwprot.stop(protocol)
+        except Exception as e:
+            logger.error("Couldn't stop the protocol: %s" % e)
             raise
         finally:
             protocol.setAborted()
             protocol.setMapper(self.createMapper(protocol.getDbPath()))
             protocol._store()
             self._storeProtocol(protocol)
+            protocol.getMapper().close()
 
     def resetProtocol(self, protocol):
         """ Stop a running protocol """
         try:
             if protocol.getStatus() in ACTIVE_STATUS:
                 pwprot.stop(protocol)
         except Exception:
@@ -760,16 +791,17 @@
         in order to avoid any modification.
         """
         return (not self.__protocolInList(child, protocols) and
                 not child.isSaved() and not child.isScheduled())
 
     def _getProtocolsDependencies(self, protocols):
         error = ''
+        runsGraph = self.getRunsGraph()
         for prot in protocols:
-            node = self.getRunsGraph().getNode(prot.strId())
+            node = runsGraph.getNode(prot.strId())
             if node:
                 childs = [node.run for node in node.getChilds() if
                           self.__validDependency(prot, node.run, protocols)]
                 if childs:
                     deps = [' ' + c.getRunName() for c in childs]
                     error += '\n *%s* is referenced from:\n   - ' % prot.getRunName()
                     error += '\n   - '.join(deps)
@@ -793,61 +825,74 @@
         this group of protocols. 
         """
         if self.openedAsReadOnly():
             raise Exception(msg + " Running in READ-ONLY mode.")
 
         self._checkProtocolsDependencies(protocols, msg)
 
-    def _checkWorkflowErrors(self, protocol):
-        """
-        This function checks if there are active protocols excluding
-        interactive protocols. Also, save the workflow from "protocol"
-        If there are no errors, the function return None
+    def _getSubworkflow(self, protocol, fixProtParam=True, getStopped=True):
         """
-        errorsList = []
-        configuredProtList = []
-        if protocol:
-            auxProList = []
-            configuredProtList.append(protocol.getObjId())
-            auxProList.append(protocol.getObjId())
-            while auxProList:
-                protocol = self.getProtocol(auxProList.pop(0))
-                if protocol.isActive() and protocol.getStatus() != STATUS_INTERACTIVE:
-                    errorsList.append(protocol.getObjId())
-                node = self.getRunsGraph().getNode(protocol.strId())
-                if node:
-                    dependencies = [node.run for node in node.getChilds()]
-                    for dep in dependencies:
-                        if dep.getObjId() in auxProList:
-                            auxProList.remove(dep.getObjId())
-                            auxProList.append(dep.getObjId())
-                        else:
-                            auxProList.append(dep.getObjId())
+        This function get the workflow from "protocol" and determine the
+        protocol level into the graph. Also, checks if there are active
+        protocols excluding interactive protocols.
+        :param protocol from where to start the subworkflow (included)
+        :param fixProtParam fix the old parameters configuration in the protocols
+        :param getStopped takes into account protocols that aren't stopped
+        """
+        affectedProtocols = {}
+        affectedProtocolsActive = {}
+        auxProtList = []
+        # store the protocol and your level into the workflow
+        affectedProtocols[protocol.getObjId()] = [protocol, 0]
+        auxProtList.append([protocol.getObjId(), 0])
+        runGraph = self.getRunsGraph()
+
+        while auxProtList:
+            protId, level = auxProtList.pop(0)
+            protocol = runGraph.getNode(str(protId)).run
+
+            # Increase the level for the children
+            level = level + 1
+
+            if fixProtParam:
+                self._fixProtParamsConfiguration(protocol)
+
+            if not getStopped and protocol.isActive():
+                affectedProtocolsActive[protocol.getObjId()] = protocol
+            elif not protocol.getObjId() in affectedProtocolsActive.keys() and getStopped and \
+                    not protocol.isSaved() and protocol.getStatus() != STATUS_INTERACTIVE:
+                affectedProtocolsActive[protocol.getObjId()] = protocol
+
+            node = runGraph.getNode(protocol.strId())
+            dependencies = [node.run for node in node.getChilds()]
+            for dep in dependencies:
+                if not dep.getObjId() in auxProtList:
+                    auxProtList.append([dep.getObjId(), level])
+
+                if not dep.getObjId() in affectedProtocols.keys():
+                    affectedProtocols[dep.getObjId()] = [dep, level]
+                elif level > affectedProtocols[dep.getObjId()][1]:
+                    affectedProtocols[dep.getObjId()][1] = level
 
-                        if dep.getObjId() in configuredProtList:
-                            configuredProtList.remove(dep.getObjId())
-                            configuredProtList.append(dep.getObjId())
-                        else:
-                            configuredProtList.append(dep.getObjId())
-        return errorsList, configuredProtList
+        return affectedProtocols, affectedProtocolsActive
 
     def deleteProtocol(self, *protocols):
         self._checkModificationAllowed(protocols, 'Cannot DELETE protocols')
 
         for prot in protocols:
             # Delete the relations created by this protocol
             self.mapper.deleteRelations(prot)
             # Delete from protocol from database
             self.mapper.delete(prot)
             wd = prot.workingDir.get()
 
             if wd.startswith(PROJECT_RUNS):
                 prot.cleanWorkingDir()
             else:
-                print("Error path: ", wd)
+                logger.info("Can't delete protocol %s. Its workingDir %s does not starts with %s " % (prot, wd, PROJECT_RUNS))
 
         self.mapper.commit()
 
     def deleteProtocolOutput(self, protocol, output):
         """ Delete a given object from the project.
         Usually to clean up some outputs.
         """
@@ -883,15 +928,15 @@
             otherProtLabel = prot.getObjLabel()
             m = REGEX_NUMBER_ENDING.match(otherProtLabel)
             if m and m.groupdict()['prefix'].strip() == defaultLabel:
                 stringSuffix = m.groupdict()['number'].strip('(').strip(')')
                 try:
                     maxSuffix = max(int(stringSuffix), maxSuffix)
                 except:
-                    print("stringSuffix", stringSuffix)
+                    logger.error("Couldn't set protocol's label. %s" % stringSuffix)
             elif otherProtLabel == defaultLabel:  # When only we have the prefix,
                 maxSuffix = max(1, maxSuffix)     # this REGEX don't match.
 
         if maxSuffix:
             protLabel = '%s (%d)' % (defaultLabel, maxSuffix+1)
         else:
             protLabel = defaultLabel
@@ -974,14 +1019,15 @@
             newProtLabel = newProtPrefix + ')'
         else:
             newProtLabel = '%s %d)' % (newProtPrefix, newNumber)
 
         newProt.setObjLabel(newProtLabel)
         newProt.copyDefinitionAttributes(protocol)
         newProt.copyAttributes(protocol, 'hostName', '_useQueue', '_queueParams')
+        newProt.runMode.set(MODE_RESTART)
 
         return newProt
 
     def copyProtocol(self, protocol):
         """ Make a copy of the protocol,
         Return a new instance with copied values. """
         result = None
@@ -995,15 +1041,15 @@
             newDict = {}
 
             for prot in protocol:
                 newProt = self.__cloneProtocol(prot)
                 newDict[prot.getObjId()] = newProt
                 self.saveProtocol(newProt)
 
-            g = self.getRunsGraph(refresh=False)
+            g = self.getRunsGraph()
 
             for prot in protocol:
                 node = g.getNode(prot.strId())
                 newProt = newDict[prot.getObjId()]
 
                 for childNode in node.getChilds():
                     newChildProt = newDict.get(childNode.run.getObjId(), None)
@@ -1013,15 +1059,21 @@
                         # node and childNode
                         matches = self.__getIOMatches(node, childNode)
                         # For each match, set the pointer and the extend
                         # attribute to reproduce the dependencies in the
                         # new workflow
                         for oKey, iKey in matches:
                             childPointer = getattr(newChildProt, iKey)
-                            if isinstance(childPointer, pwobj.PointerList):
+
+                            # Scalar with pointer case: If is a scalar with a pointer
+                            if isinstance(childPointer, pwobj.Scalar) and childPointer.hasPointer():
+                              # In this case childPointer becomes the contained Pointer
+                              childPointer = childPointer.getPointer()
+
+                            elif isinstance(childPointer, pwobj.PointerList):
                                 for p in childPointer:
                                     if p.getObjValue().getObjId() == prot.getObjId():
                                         childPointer = p
                             childPointer.set(newProt)
                             childPointer.setExtended(oKey)
                         self.mapper.store(newChildProt)
 
@@ -1029,35 +1081,35 @@
         else:
             raise Exception("Project.copyProtocol: invalid input protocol ' "
                             "'type '%s'." % type(protocol))
 
         return result
 
     def getProtocolsDict(self, protocols=None, namesOnly=False):
-        """ Create a dict with the information of the given protocols.
-         Params:
-            protocols: list of protocols or None to include all.
-            namesOnly: the output list will contain only the protocol names.
+        """ Creates a dict with the information of the given protocols.
+
+        :param protocols: list of protocols or None to include all.
+        :param namesOnly: the output list will contain only the protocol names.
+
         """
         protocols = protocols or self.getRuns()
 
         # If the nameOnly, we will simply return a json list with their names
         if namesOnly:
             return {i: prot.getClassName() for i, prot in enumerate(protocols)}
 
         # Handle the copy of a list of protocols
         # for this case we need to update the references of input/outputs
         newDict = OrderedDict()
 
         for prot in protocols:
             newDict[prot.getObjId()] = prot.getDefinitionDict()
 
-        g = self.getRunsGraph(refresh=False)
+        g = self.getRunsGraph()
 
-        # pwutils.startDebugger('a')
         for prot in protocols:
             protId = prot.getObjId()
             node = g.getNode(prot.strId())
 
             for childNode in node.getChilds():
                 childId = childNode.run.getObjId()
                 childProt = childNode.run
@@ -1074,91 +1126,107 @@
                         else:
                             childDict[iKey] = '%s.%s' % (
                                 protId, oKey)  # equivalent to pointer.getUniqueId
 
         return newDict
 
     def getProtocolsJson(self, protocols=None, namesOnly=False):
-        """ Wraps getProtocolsDict to get a json string
-             Params:
-                protocols: list of protocols or None to include all.
-                namesOnly: the output list will contain only the protocol names.
+        """
+        Wraps getProtocolsDict to get a json string
+
+        :param protocols: list of protocols or None to include all.
+        :param namesOnly: the output list will contain only the protocol names.
+
         """
         newDict = self.getProtocolsDict(protocols=protocols, namesOnly=namesOnly)
         return json.dumps(list(newDict.values()),
                           indent=4, separators=(',', ': '))
 
     def exportProtocols(self, protocols, filename):
         """ Create a text json file with the info
         to import the workflow into another project.
-        This methods is very similar to copyProtocol
-        Params:
-            protocols: a list of protocols to export.
-            filename: the filename where to write the workflow.
+        This method is very similar to copyProtocol
+
+        :param protocols: a list of protocols to export.
+        :param filename: the filename where to write the workflow.
+
         """
         jsonStr = self.getProtocolsJson(protocols)
         f = open(filename, 'w')
         f.write(jsonStr)
         f.close()
 
     def loadProtocols(self, filename=None, jsonStr=None):
         """ Load protocols generated in the same format as self.exportProtocols.
-        Params:
-            filename: the path of the file where to read the workflow.
-            jsonStr: read the protocols from a string instead of file.
+
+        :param filename: the path of the file where to read the workflow.
+        :param jsonStr:
+
         Note: either filename or jsonStr should be not None.
+
         """
-        f = open(filename)
-        importDir = os.path.dirname(filename)
-        protocolsList = json.load(f)
+        importDir = None
+        if filename:
+            with open(filename) as f:
+                importDir = os.path.dirname(filename)
+                protocolsList = json.load(f)
+
+        elif jsonStr:
+            protocolsList = json.loads(jsonStr)
+        else:
+            logger.error("Invalid call to  loadProcols. Either filename or jsonStr has to be passed.")
+            return
 
         emProtocols = self._domain.getProtocols()
         newDict = OrderedDict()
 
         # First iteration: create all protocols and setup parameters
         for i, protDict in enumerate(protocolsList):
             protClassName = protDict['object.className']
             protId = protDict['object.id']
             protClass = emProtocols.get(protClassName, None)
 
             if protClass is None:
-                print("ERROR: protocol class name '%s' not found" % protClassName)
+                logger.error("Protocol with class name '%s' not found. Are you missing its plugin?." % protClassName)
             else:
                 protLabel = protDict.get('object.label', None)
                 prot = self.newProtocol(protClass,
                                         objLabel=protLabel,
                                         objComment=protDict.get('object.comment', None))
-                protocolsList[i] = prot.processImportDict(protDict, importDir)
+                protocolsList[i] = prot.processImportDict(protDict, importDir) if importDir else protDict
 
                 prot._useQueue.set(protDict.get('_useQueue', False))
                 prot._queueParams.set(protDict.get('_queueParams', None))
                 prot._prerequisites.set(protDict.get('_prerequisites', None))
+                prot.forceSchedule.set(protDict.get('forceSchedule', False))
                 newDict[protId] = prot
                 self.saveProtocol(prot)
 
         # Second iteration: update pointers values
         def _setPointer(pointer, value):
             # Properly setup the pointer value checking if the 
             # id is already present in the dictionary
-            parts = value.split('.')
-            target = newDict.get(parts[0], None)
-            pointer.set(target)
-            if not pointer.pointsNone():
-                pointer.setExtendedParts(parts[1:])
+            # Value to pointers could be None: Partial workflows
+            if value:
+                parts = value.split('.')
+                target = newDict.get(parts[0], None)
+                pointer.set(target)
+                if not pointer.pointsNone():
+                    pointer.setExtendedParts(parts[1:])
 
         def _setPrerequisites(prot):
             prerequisites = prot.getPrerequisites()
             if prerequisites:
                 newPrerequisites = []
                 for prerequisite in prerequisites:
                     if prerequisite in newDict:
                         newProtId = newDict[prerequisite].getObjId()
                         newPrerequisites.append(newProtId)
                     else:
-                        print('Wait for id %s missing: ignored' % prerequisite)
+                        logger.info('"Wait for" id %s missing: ignored.' % prerequisite)
                 prot._prerequisites.set(newPrerequisites)
 
         for protDict in protocolsList:
             protId = protDict['object.id']
 
             if protId in newDict:
                 prot = newDict[protId]
@@ -1176,20 +1244,27 @@
                             attribute = protDict[paramName]
                             if attribute is None:
                                 continue
                             for value in attribute:
                                 p = pwobj.Pointer()
                                 _setPointer(p, value)
                                 attr.append(p)
-                        # For "normal" parameters we just set the string value 
+                        # For "normal" parameters we just set the string value
                         else:
-                            attr.set(protDict[paramName])
+                            try:
+                                attr.set(protDict[paramName])
+                            # Case for Scalars with pointers. So far this will work for Numbers. With Strings (still there are no current examples)
+                            # We will need something different to test if the value look like a pointer: regex? ####.text
+                            except ValueError as e:
+                                newPointer = pwobj.Pointer()
+                                _setPointer(newPointer, protDict[paramName])
+                                attr.setPointer(newPointer)
+
                 self.mapper.store(prot)
 
-        f.close()
         self.mapper.commit()
 
         return newDict
 
     def saveProtocol(self, protocol):
         self._checkModificationAllowed([protocol], 'Cannot SAVE protocol')
 
@@ -1291,14 +1366,17 @@
                     r.closeMappers()
 
             # Use new selectAll Batch
             # self.runs = self.mapper.selectAll(iterate=False,
             #               objectFilter=lambda o: isinstance(o, pwprot.Protocol))
             self.runs = self.mapper.selectAllBatch(objectFilter=lambda o: isinstance(o, pwprot.Protocol))
 
+            # Invalidate _runsGraph because the runs are updated
+            self._runsGraph = None
+
             for r in self.runs:
 
                 self._setProtocolMapper(r)
 
                 # Check for run warnings
                 r.checkSummaryWarnings()
 
@@ -1342,15 +1420,22 @@
         """ Check if a running protocol is still alive or not.
         The check will only be done for protocols that have not been sent
         to a queue system.
         """
         from pyworkflow.protocol.launch import _runsLocally
         pid = protocol.getPid()
 
-        if (protocol.isRunning() and _runsLocally(protocol)
+        if pid == 0:
+            return
+
+        # Include running and scheduling ones
+        # Exclude interactive protocols
+        # NOTE: This may be happening even with successfully finished protocols
+        # which PID is gone.
+        if (protocol.isActive() and not protocol.isInteractive() and _runsLocally(protocol)
             and not protocol.useQueue()
                 and not pwutils.isProcessAlive(pid)):
             protocol.setFailed("Process %s not found running on the machine. "
                                "It probably has died or been killed without "
                                "reporting the status to Scipion. Logs might "
                                "have information about what happened to this "
                                "process." % pid)
@@ -1363,53 +1448,63 @@
             objectFilter: a filter function to discard some of the retrieved
             objects."""
         for objClass in classesName.split(","):
             for obj in self.mapper.selectByClass(objClass.strip(), iterate=True,
                                                  objectFilter=objectFilter):
                 yield obj
 
-    def getRunsGraph(self, refresh=True, checkPids=False):
+    def getRunsGraph(self, refresh=False, checkPids=False):
         """ Build a graph taking into account the dependencies between
         different runs, ie. which outputs serves as inputs of other protocols. 
         """
 
         if refresh or self._runsGraph is None:
             runs = [r for r in self.getRuns(refresh=refresh, checkPids=checkPids)
                     if not r.isChild()]
             self._runsGraph = self.getGraphFromRuns(runs)
 
         return self._runsGraph
 
     def getGraphFromRuns(self, runs):
-        """ This function will build a dependencies graph from a set
-         of given runs.
+        """
+        This function will build a dependencies graph from a set
+        of given runs.
+
         :param runs: The input runs to build the graph
         :return: The graph taking into account run dependencies
+
         """
         outputDict = {}  # Store the output dict
-        g = pwutils.Graph(rootName='PROJECT')
+        g = pwutils.Graph(rootName=ROOT_NODE_NAME)
 
         for r in runs:
             n = g.createNode(r.strId())
             n.run = r
-            n.setLabel(r.getRunName())
+
+            # Legacy protocols do not have a plugin!!
+            develTxt =''
+            plugin=r.getPlugin()
+            if plugin and plugin.inDevelMode():
+                develTxt='ẟ '
+
+            n.setLabel('%s%s' % (develTxt , r.getRunName()))
             outputDict[r.getObjId()] = n
             for _, attr in r.iterOutputAttributes():
                 # mark this output as produced by r
                 outputDict[attr.getObjId()] = n
 
         def _checkInputAttr(node, pointed):
             """ Check if an attr is registered as output"""
             if pointed is not None:
                 pointedId = pointed.getObjId()
 
                 if pointedId in outputDict:
                     parentNode = outputDict[pointedId]
                     if parentNode is node:
-                        print("WARNING: Found a cyclic dependence from node "
+                        logger.warning("WARNING: Found a cyclic dependence from node "
                               "%s to itself, probably a bug. " % pointedId)
                     else:
                         parentNode.addChild(node)
                         return True
             return False
 
         for r in runs:
@@ -1420,26 +1515,26 @@
                     # Only checking pointed object and its parent, if more
                     # levels we need to go up to get the correct dependencies
                     if not _checkInputAttr(node, pointed):
                         parent = self.mapper.getParent(pointed)
                         _checkInputAttr(node, parent)
         rootNode = g.getRoot()
         rootNode.run = None
-        rootNode.label = "PROJECT"
+        rootNode.label = ROOT_NODE_NAME
 
         for n in g.getNodes():
             if n.isRoot() and n is not rootNode:
                 rootNode.addChild(n)
         return g
 
     def _getRelationGraph(self, relation=pwobj.RELATION_SOURCE, refresh=False):
         """ Retrieve objects produced as outputs and
         make a graph taking into account the SOURCE relation. """
         relations = self.mapper.getRelationsByName(relation)
-        g = pwutils.Graph(rootName='PROJECT')
+        g = pwutils.Graph(rootName=ROOT_NODE_NAME)
         root = g.getRoot()
         root.pointer = None
         runs = self.getRuns(refresh=refresh)
 
         for r in runs:
             for paramName, attr in r.iterOutputAttributes():
                 p = pwobj.Pointer(r, extended=paramName)
@@ -1450,62 +1545,62 @@
                 g.aliasNode(node, p2.getUniqueId())
 
         for rel in relations:
             pObj = self.getObject(rel[OBJECT_PARENT_ID])
 
             # Duplicated ...
             if pObj is None:
-                print("WARNING: Relation seems to point to a deleted object. "
+                logger.warning("Relation seems to point to a deleted object. "
                       "%s: %s" % (OBJECT_PARENT_ID, rel[OBJECT_PARENT_ID]))
                 continue
 
             pExt = rel['object_parent_extended']
             pp = pwobj.Pointer(pObj, extended=pExt)
 
             if pObj is None or pp.get() is None:
-                print("project._getRelationGraph: ERROR, pointer to parent is "
+                logger.error("project._getRelationGraph: pointer to parent is "
                       "None. IGNORING IT.\n")
                 for key in rel.keys():
-                    print("%s: %s" % (key, rel[key]))
+                    logger.info("%s: %s" % (key, rel[key]))
 
                 continue
 
             pid = pp.getUniqueId()
             parent = g.getNode(pid)
 
             while not parent and pp.hasExtended():
                 pp.removeExtended()
                 parent = g.getNode(pp.getUniqueId())
 
             if not parent:
-                print("project._getRelationGraph: ERROR, parent Node "
-                      "is None: ", pid)
+                logger.error("project._getRelationGraph: parent Node "
+                      "is None: %s" % pid)
             else:
                 cObj = self.getObject(rel['object_child_id'])
                 cExt = rel['object_child_extended']
 
                 if cObj is not None:
                     if cObj.isPointer():
                         cp = cObj
                         if cExt:
                             cp.setExtended(cExt)
                     else:
                         cp = pwobj.Pointer(cObj, extended=cExt)
                     child = g.getNode(cp.getUniqueId())
 
                     if not child:
-                        print("project._getRelationGraph: ERROR, child Node "
-                              "is None: ", cp.getUniqueId())
-                        print("   parent: ", pid)
+                        logger.error("project._getRelationGraph: child Node "
+                              "is None: %s." % cp.getUniqueId())
+                        logger.error("   parent: %s" % pid)
                     else:
                         parent.addChild(child)
                 else:
-                    print("project._getRelationGraph: ERROR, child Obj "
-                          "is None, id: ", rel['object_child_id'])
-                    print("   parent: ", pid)
+                    logger.error("project._getRelationGraph: child Obj "
+                          "is None, id: %s " %  rel['object_child_id'])
+                    logger.error("   parent: %s" % pid)
 
         for n in g.getNodes():
             if n.isRoot() and n is not root:
                 root.addChild(n)
 
         return g
 
@@ -1535,33 +1630,36 @@
                                                        refresh)
 
         return self._sourceGraph
 
     def getRelatedObjects(self, relation, obj, direction=pwobj.RELATION_CHILDS,
                           refresh=False):
         """ Get all objects related to obj by a give relation.
-        Params:
-            relation: the relation name to search for.
-            obj: object from which the relation will be search,
-                actually not only this, but all other objects connected
-                to this one by the pwobj.RELATION_TRANSFORM.
-            direction: this say if search for childs or parents in the relation.
+
+        :param relation: the relation name to search for.
+        :param obj: object from which the relation will be search,
+            actually not only this, but all other objects connected
+            to this one by the pwobj.RELATION_TRANSFORM.
+        :parameter direction: Not used
+        :param refresh: If True, cached objects will be refreshed
+
         """
+
         graph = self.getTransformGraph(refresh)
         relations = self.mapper.getRelationsByName(relation)
         connection = self._getConnectedObjects(obj, graph)
 
         objects = []
         objectsDict = {}
 
         for rel in relations:
             pObj = self.getObject(rel[OBJECT_PARENT_ID])
 
             if pObj is None:
-                print("WARNING: Relation seems to point to a deleted object. "
+                logger.warning("Relation seems to point to a deleted object. "
                       "%s: %s" % (OBJECT_PARENT_ID, rel[OBJECT_PARENT_ID]))
                 continue
             pExt = rel['object_parent_extended']
             pp = pwobj.Pointer(pObj, extended=pExt)
 
             if pp.getUniqueId() in connection:
                 cObj = self.getObject(rel['object_child_id'])
@@ -1571,15 +1669,15 @@
                     objects.append(cp)
                     objectsDict[cp.getUniqueId()] = True
 
         return objects
 
     def _getConnectedObjects(self, obj, graph):
         """ Given a TRANSFORM graph, return the elements that
-        are connected to an object, either childs, ancestors or siblings. 
+        are connected to an object, either children, ancestors or siblings.
         """
         n = graph.getNode(obj.strId())
         # Get the oldest ancestor of a node, before reaching the root node
         while n is not None and not n.getParent().isRoot():
             n = n.getParent()
 
         connection = {}
@@ -1605,40 +1703,45 @@
     def openedAsReadOnly(self):
         return self.isReadOnly() or self.isInReadOnlyFolder()
 
     def setReadOnly(self, value):
         self.settings.setReadOnly(value)
 
     def fixLinks(self, searchDir):
+        logger.info("Fixing project links. Searching at %s" % searchDir)
         runs = self.getRuns()
 
         for prot in runs:
+            print (prot)
             broken = False
-            if isinstance(prot, ProtImportBase):
+            if isinstance(prot, ProtImportBase) or prot.getClassName() == "ProtImportMovies":
+                logger.info("Import detected")
                 for _, attr in prot.iterOutputAttributes():
-                    fn = attr.getFiles()
                     for f in attr.getFiles():
                         if ':' in f:
                             f = f.split(':')[0]
 
                         if not os.path.exists(f):
                             if not broken:
                                 broken = True
-                                print("Found broken links in run: ",
+                                logger.info("Found broken links in run: %s" %
                                       pwutils.magenta(prot.getRunName()))
-                            print("  Missing: ", pwutils.magenta(f))
+                            logger.info("  Missing: %s" % pwutils.magenta(f))
+
                             if os.path.islink(f):
-                                print("    -> ", pwutils.red(os.path.realpath(f)))
-                            newFile = pwutils.findFile(os.path.basename(f),
+                                sourceFile = os.path.realpath(f)
+                                logger.info("    -> %s" % pwutils.red(sourceFile))
+
+                                newFile = pwutils.findFile(os.path.basename(sourceFile),
                                                        searchDir,
                                                        recursive=True)
-                            if newFile:
-                                print("  Found file %s, creating link..." % newFile,
-                                      pwutils.green("   %s -> %s" % (f, newFile)))
-                                pwutils.createAbsLink(newFile, f)
+                                if newFile:
+                                    logger.info("  Found file %s, creating link... %s" % (newFile,
+                                        pwutils.green("   %s -> %s" % (f, newFile))))
+                                    pwutils.createAbsLink(newFile, f)
 
     @staticmethod
     def cleanProjectName(projectName):
         """ Cleans a project name to avoid common errors
         Use it whenever you want to get the final project name pyworkflow will endup.
         Spaces will be replaced by _ """
         return projectName.replace(" ", "_")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/clean_projects.py` & `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/clean_projects.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,16 @@
 from pyworkflow.project import Manager
 
 
 def usage(error):
     print("""
     ERROR: %s
     
-    Usage: scipion python scripts/clean_projects.py [SCIPION_USER_DATA] [--delete]
-        Clean projects that has expired (now - creation time > life time)
+    Usage: scipion python -m pyworkflow.project.scripts.clean_projects [SCIPION_USER_DATA] [--delete]
+        Clean projects that have expired (now - creation time > life time)
         Optional to pass SCIPION_USER_DATA folder from which to read 'projects'.
         If --delete is not passed, only a message with the projects to be deleted
         will be shown. If used --delete, the projects will be deleted from filesystem.
     """ % error)
     sys.exit(1)
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/config.py` & `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,18 +34,18 @@
 from pyworkflow.object import Boolean
 
 
 def usage(error):
     print("""
     ERROR: %s
     
-    Usage: scipion python scripts/config_projects.py ProjectName [readOnly=True|False] [lifeTime=X|None]
-        This script show (or edit) some of the configuration of the project.
-        Use readOnly=True (or False) to set/unset read only property
-        Use lifeTime=X for setting X hours or None to unset life time of the project.
+    Usage: scipion python -m pyworkflow.project.scripts.config_projects ProjectName [readOnly=True|False] [lifeTime=X|None]
+        This script shows (or edits) some of the configuration of the project.
+        Use readOnly=True (or False) to set/unset read-only property.
+        Use lifeTime=X for setting X hours or None to unset lifetime of the project.
     """ % error)
     sys.exit(1)    
 
 
 n = len(sys.argv)
 
 if n < 2 or n > 4:
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/create.py` & `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/create.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,18 +32,19 @@
 import pyworkflow.utils as pwutils
 
 
 def usage(error):
     print("""
     ERROR: %s
 
-    Usage: scipion python scripts/create_project.py
-        name="project name"
-        [workflow="file"] path to a Scipion json workflow
-        [location="folder"] where to create it, defaults to scipion default location
+    Usage: scipion python -m pyworkflow.project.scripts.create NAME [WORKFLOW] [LOCATION]
+        NAME: project name
+        WORKFLOW: path to a Scipion json workflow
+        LOCATION: where to create it, defaults to scipion default location
+
         This script will create a project project, optionally based on a workflow file
     """ % error)
     sys.exit(1)
 
 
 n = len(sys.argv)
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/edit_workflow.py` & `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/edit_workflow.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from pyworkflow.gui.project import ProjectWindow
 
 
 def usage(error):
     print("""
     ERROR: %s
     
-    Usage: scipion python scripts/edit_workflow.py workflow.json
+    Usage: scipion python -m pyworkflow.project.scripts.edit_workflow workflow.json
         Edit the provide json file with scipion workflow.
         It will create a project, import the workflow and save
         the workflow back before closing the project.
         After that, the project will be deleted.
     """ % error)
     sys.exit(1)    
 
@@ -73,15 +73,15 @@
 proj.loadProtocols(jsonFn)
 
 
 class EditorProjectWindow(ProjectWindow):
     def close(self, e=None):
         try:
             print("Writing protocols to: ", jsonFn)
-            proj.getRunsGraph()  # Build project runs graph
+            proj.getRunsGraph(refresh=True)  # Build project runs graph
             proj.exportProtocols(proj.getRuns(), jsonFn)
             print("Deleting temporary folder: ", customUserData)
             pwutils.cleanPath(customUserData)
         except Exception as ex:
             print("Error saving the workflow: ", ex)
         ProjectWindow.close(self, e)
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/fix_links.py` & `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/fix_links.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 #!/usr/bin/env python
 
 import sys
 import os
+import logging
+logging.basicConfig(level="INFO")
 
 from pyworkflow.project import Manager
 import pyworkflow.utils as pwutils
 
 
 def usage(error):
     print("""
     ERROR: %s
     
-    Usage: fixlinks.py PROJECT SEARCH_DIR
-        PROJECT: provide the project name to fix broken links in the imports.
-        SEARCH_DIR: provide a directory where to look for the files.
-        and fix the links.    
+    Usage: scipion python -m pyworkflow.project.scripts.fix_links PROJECT SEARCH_DIR
+        PROJECT: provide the project name to fix broken links in the imports
+        SEARCH_DIR: provide a directory where to look for the files and fix the links    
     """ % error)
-    sys.exit(1)    
+    os._exit(1)
 
+def main():
+    if len(sys.argv) != 3:
+        usage("Incorrect number of input parameters")
 
-if len(sys.argv) != 3:
-    usage("Incorrect number of input parameters")
+    projName = sys.argv[1]
+    searchDir = os.path.abspath(sys.argv[2])
 
-projName = sys.argv[1]
-searchDir = os.path.abspath(sys.argv[2])
+    # Create a new project
+    manager = Manager()
 
-# Create a new project
-manager = Manager()
+    if not manager.hasProject(projName):
+        usage("Nonexistent project: %s" % pwutils.red(projName))
 
-if not manager.hasProject(projName):
-    usage("Nonexistent project: %s" % pwutils.red(projName))
-    
-if not os.path.exists(searchDir):
-    usage("Nonexistent SEARCH_DIR: %s" % pwutils.red(searchDir))
-    
-project = manager.loadProject(projName)
+    if not os.path.exists(searchDir):
+        usage("Nonexistent SEARCH_DIR: %s" % pwutils.red(searchDir))
+
+    project = manager.loadProject(projName)
+
+    project.fixLinks(searchDir)
 
-project.fixLinks(searchDir)
+if __name__ == '__main__':
+    main()
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/load.py` & `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from pyworkflow.gui.project import ProjectWindow
 
 
 def usage(error):
     print("""
     ERROR: %s
     
-    Usage: scipion python scripts/load_project.py /path/to/project
+    Usage: scipion python -m pyworkflow.project.scripts.load /path/to/project
         This script allows to quickly load a project folder without
         importing that in the general user data folder
     """ % error)
     sys.exit(1)    
 
 
 n = len(sys.argv)
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/refresh.py` & `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/refresh.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 import pyworkflow.utils as pwutils
 
 
 def usage(error):
     print("""
     ERROR: %s
 
-    Usage: scipion python scripts/refresh_project.py project_name [refresh_period]
+    Usage: scipion python -m scripts.project.refresh_project project_name [refresh_period]
         This script will refresh the project.sqlite file of the specified project.
         We can specify how often it will refresh in seconds (defaults 60).
         e.g.
-        scipion python scripts/refresh_project.py TestExtractParticles 15
+        scipion python -m scripts.project.refresh_project TestExtractParticles 15
     """ % error)
     sys.exit(1)
 
 
 n = len(sys.argv)
 
 if n > 3:
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/schedule.py` & `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/schedule.py`

 * *Files 13% similar despite different names*

```diff
@@ -29,26 +29,27 @@
 import os
 import time
 
 import pyworkflow as pw
 from pyworkflow.project import Manager
 from pyworkflow.project import Project
 import pyworkflow.utils as pwutils
+from pyworkflow.protocol import INITIAL_SLEEP_TIME
 
 
 def usage(error):
     print("""
     ERROR: %s
     
-    Usage: scipion python -m pyworkflow/project/scripts/schedule projectName 
+    Usage: scipion python -m pyworkflow.project.scripts.schedule projectName 
     
               options: --ignore ProtClassName1 ProtClassName2 ProtClassLabel1 ...
               
         This script will schedule all the protocols in a project. If '--ignore' 
-          options is passed, it doesn't schedule those protocols that belongs to 
+          option is passed, it doesn't schedule those protocols that belongs to 
           ProtClassName1 or ProtClassName2 class, also those protocols with a 
           objLabel equals to ProtClassLabel1
     """ % error)
     sys.exit(1)
 
 
 n = len(sys.argv)
@@ -69,31 +70,42 @@
 # Create a new project
 manager = Manager()
 
 if not manager.hasProject(projName):
     usage("There is no project with this name: %s"
           % pwutils.red(projName))
 
-# the project may be a soft link which may be unavailable to the cluster so get the real path
+# the project may be a soft link which may be unavailable to the cluster
+# so get the real path
+
 try:
     projectPath = os.readlink(manager.getProjectPath(projName))
 except:
     projectPath = manager.getProjectPath(projName)
 
 project = Project(pw.Config.getDomain(), projectPath)
 project.load()
 
-runs = project.getRuns()
+runGraph = project.getRunsGraph()
+roots = runGraph.getRootNodes()
 
 # Now assuming that there is no dependencies between runs
 # and the graph is lineal
-for prot in runs:
-    protClassName = prot.getClassName()
-    protLabelName = prot.getObjLabel()
-    if (protClassName not in sys.argv[3:] and
-            protLabelName not in sys.argv[3:]):
-        project.scheduleProtocol(prot)
-        # Wait 1 seconds to avoid concurrent activity
-        time.sleep(0.7)
-    else:
-        print(pwutils.blueStr("\nNot scheduling '%s' protocol named '%s'.\n"
-                              % (protClassName, protLabelName)))
+
+for root in roots:
+    for child in root.getChilds():
+        workflow, _ = project._getSubworkflow(child.run)
+        for prot, level in workflow.values():
+            if prot.forceSchedule.get():
+                print(pwutils.blueStr("\nStopping scheduling at '%s'. Force scheduling found.\n"
+                                      % protLabelName))
+                sys.exit()
+
+            protClassName = prot.getClassName()
+            protLabelName = prot.getObjLabel()
+            if (protClassName not in sys.argv[3:] and
+                    protLabelName not in sys.argv[3:]):
+                project.scheduleProtocol(prot,
+                                         initialSleepTime=level*INITIAL_SLEEP_TIME)
+            else:
+                print(pwutils.blueStr("\nNot scheduling '%s' protocol named '%s'.\n"
+                                      % (protClassName, protLabelName)))
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/stack2volume.py` & `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/stack2volume.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,18 +8,18 @@
 import pyworkflow.utils as pwutils
 
 
 def usage(error):
     print("""
     ERROR: %s
     
-    stack2Volume will swap the dimension in the header of stack to make them 
-    volumes. Something like 10 x 1 x 10 x 10 will be change to 1 x 10 x 10 x 10
-    Usage: stack2volume.py PATH
-        PATH: path to look for stack files    
+    Usage: scipion python -m pyworkflow.project.scripts.stack2volume PATH
+        PATH: path to look for stack files
+    The script will swap the dimensions in the header of a stack to make them 
+    volumes. Something like 10 x 1 x 10 x 10 will be changed to 1 x 10 x 10 x 10
     """ % error)
     sys.exit(1)    
 
 
 if len(sys.argv) != 2:
     usage("Incorrect number of input parameters")
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/project/scripts/stop.py` & `scipion-pyworkflow-3.1.0/pyworkflow/project/scripts/stop.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,18 +34,16 @@
 from pyworkflow.project import Manager, Project
 
 
 def usage(error):
     print("""
     ERROR: %s
 
-    Usage: scipion python scripts/stop.py project_name
+    Usage: scipion python -m pyworkflow.project.scripts.stop project_name
         This script will stop all running protocols of the specified project.
-        e.g.
-        scipion python scripts/stop.py MyProject
     """ % error)
     sys.exit(1)
 
 
 n = len(sys.argv)
 
 if n > 2:
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/protocol/__init__.py` & `scipion-pyworkflow-3.1.0/pyworkflow/gui/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,20 +19,18 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
-"""
-This modules contains classes required for the workflow
-execution and tracking like: Step and Protocol
-"""
+from .gui import *
+from .canvas import *
+from .widgets import *
+from .graph import *
+from .graph_layout import *
+from .tree import *
+from .browser import *
+from .text import *
+from .dialog import *
 
-from .protocol import *
-from .executor import *
-from .constants import *
-from .params import *
-
-from .launch import *
-
-from .hosts import HostConfig
+from . import tooltip
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/protocol/bibtex.py` & `scipion-pyworkflow-3.1.0/pyworkflow/protocol/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/protocol/constants.py` & `scipion-pyworkflow-3.1.0/pyworkflow/protocol/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,14 +50,23 @@
 # Execution modes
 MODE_RESUME = 0    # Try to starting at the first changed step, skipping unchanged ones
 MODE_RESTART = 1   # Restart the protocol from the beginning, deleting all previous results
 MODE_CONTINUE = 2  # Continue from specific step, not widely used //DEPRECATED.
 # JMRT: We now use 'Continue' label instead of 'Resume' which is more intuitive for users.
 MODE_CHOICES = ('Continue', 'Restart')  # , 'Continue')
 
+# Initial sleeping time (in seconds) in order to launch a scheduled protocol.
+# This value is multiply to the protocol level into the workflow.
+INITIAL_SLEEP_TIME = 30
+
+# Maximum time (in seconds) waiting for a scheduled protocol to check if it
+# can be launched.
+MAX_SLEEP_TIME = 120
+
+
 # Steps execution mode
 STEPS_SERIAL = 0      # Execute steps serially, some of the steps can be mpi programs
 STEPS_PARALLEL = 1    # Execute steps in parallel, through threads or mpi
 
 # Level of expertise for the input parameters, mainly used in the protocol form
 LEVEL_NORMAL = 0
 LEVEL_ADVANCED = 1
@@ -65,7 +74,13 @@
 
 # Param names for GPU processing
 USE_GPU = 'useGpu'
 GPU_LIST = 'gpuList'
 
 # Job management
 UNKNOWN_JOBID = -1
+
+# File sizes
+SIZE_1KB = 1024
+SIZE_1MB = SIZE_1KB * SIZE_1KB
+SIZE_1GB = SIZE_1MB * SIZE_1KB
+SIZE_1TB = SIZE_1GB * SIZE_1KB
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/protocol/executor.py` & `scipion-pyworkflow-3.1.0/pyworkflow/protocol/executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 """
 This module have the classes for execution of protocol steps.
 The basic one will run steps, one by one, after completion.
 There is one based on threads to execute steps in parallel
 using different threads and the last one with MPI processes.
 """
 
-
+import logging
+logger = logging.getLogger(__name__)
 import time
 import datetime
-import traceback
 import threading
 import os
 import re
 from subprocess import Popen, PIPE
 
 import pyworkflow.utils.process as process
 from pyworkflow.utils.path import getParentFolder, removeExt
@@ -97,15 +97,15 @@
         # In this way we can take into account the steps graph
         # dependency and also the case when using streaming
 
         delta = datetime.timedelta(seconds=stepsCheckSecs)
         lastCheck = datetime.datetime.now()
 
         while True:
-            # Get an step to run, if there is one
+            # Get a step to run, if there is any
             runnableSteps = self._getRunnable(steps)
 
             if runnableSteps:
                 step = runnableSteps[0]
                 # We found a step to work in, so let's start a new
                 # thread to do the job and book it.
                 step.setRunning()
@@ -144,22 +144,22 @@
 
     def run(self):
         error = None
         try:
             self.step._run()  # not self.step.run() , to avoid race conditions
         except Exception as e:
             error = str(e)
-            traceback.print_exc()
+            logger.error("Couldn't run the code in a thread." , exc_info=e)
         finally:
             with self.lock:
                 if error is None:
-                    self.step.setStatus(cts.STATUS_FINISHED)
+                    self.step.setFinished()
                 else:
                     self.step.setFailed(error)
-                self.step.endTime.set(datetime.datetime.now())
+
 
 
 class ThreadStepExecutor(StepExecutor):
     """ Run steps in parallel using threads. """
     def __init__(self, hostConfig, nThreads, **kwargs):
         StepExecutor.__init__(self, hostConfig, **kwargs)
         self.numberOfProcs = nThreads
@@ -189,20 +189,26 @@
         or empty list if not using GPUs. """
         return self.gpuDict.get(threading.currentThread().thId, [])
         
     def runSteps(self, steps, 
                  stepStartedCallback, 
                  stepFinishedCallback,
                  stepsCheckCallback,
-                 stepsCheckSecs=3):
-        """ Create threads and synchronize the steps execution.
-        n: the number of threads.
-        stepsCheckSecs:
-            rate of how many seconds between stepsCheckCallback calls
+                 stepsCheckSecs=5):
+        """
+        Creates threads and synchronize the steps execution.
+
+        :param steps: list of steps to run
+        :param stepStartedCallback: callback to be called before starting any step
+        :param stepFinishedCallback: callback to be run after all steps are done
+        :param stepsCheckCallback: callback to check if there are new steps to add (streaming)
+        :param stepsCheckSecs: seconds between stepsCheckCallback calls
+
         """
+
         delta = datetime.timedelta(seconds=stepsCheckSecs)
         lastCheck = datetime.datetime.now()
 
         sharedLock = threading.Lock()
 
         runningSteps = {}  # currently running step in each node ({node: step})
         freeNodes = list(range(self.numberOfProcs))  # available nodes to send jobs
@@ -274,14 +280,25 @@
             self.threadCommands[threadId] = 0
 
         if nThreads > 1:
             self.runJobs = ThreadStepExecutor.runSteps
         else:
             self.runJobs = StepExecutor.runSteps
 
+        self.renameGpuIds()
+
+    def renameGpuIds(self):
+        """ Reorganize the gpus ids starting from 0 since the queue engine is the one assigning them.
+        https://docs.nvidia.com/cuda/cuda-c-programming-guide/index.html#env-vars """
+        for threadId, gpuList in self.gpuDict.items():
+            for i in range(len(gpuList)):
+                self.gpuDict[threadId][i] = i
+
+        logger.debug("Updated gpus ids rebase starting from 0: %s per thread" %self.gpuDict)
+
     def runJob(self, log, programName, params, numberOfMpi=1, numberOfThreads=1, env=None, cwd=None):
         threadId = threading.current_thread().thId
         submitDict = dict(self.hostConfig.getQueuesDefault())
         submitDict.update(self.submitDict)
         submitDict['JOB_COMMAND'] = process.buildRunCommand(programName, params, numberOfMpi,
                                                             self.hostConfig, env,
                                                             gpuList=self.getGpuList())
@@ -290,15 +307,15 @@
         submitDict['JOB_NAME'] = submitDict['JOB_NAME'] + subthreadId
         submitDict['JOB_SCRIPT'] = os.path.abspath(removeExt(submitDict['JOB_SCRIPT']) + subthreadId + ".job")
         submitDict['JOB_LOGS'] = os.path.join(getParentFolder(submitDict['JOB_SCRIPT']), submitDict['JOB_NAME'])
 
         jobid = _submit(self.hostConfig, submitDict, cwd, env)
 
         if (jobid is None) or (jobid == UNKNOWN_JOBID):
-            print("jobId is none therefore we set it to fail")
+            logger.info("jobId is none therefore we set it to fail")
             raise Exception("Failed to submit to queue.")
 
         status = cts.STATUS_RUNNING
         wait = 3
 
         # Check status while job running
         # REVIEW this to minimize the overhead in time put by this delay check
@@ -306,31 +323,34 @@
             time.sleep(wait)
             if wait < 300:
                 wait += 3
 
         return status
 
     def _checkJobStatus(self, hostConfig, jobid):
-
         command = hostConfig.getCheckCommand() % {"JOB_ID": jobid}
+        logger.debug("checking job status for %s: %s" %(jobid, command))
         p = Popen(command, shell=True, stdout=PIPE, preexec_fn=os.setsid)
 
-        out = p.communicate()[0]
+        out = p.communicate()[0].decode(errors='backslashreplace')
 
         jobDoneRegex = hostConfig.getJobDoneRegex()
-
+        logger.debug("Queue engine replied %s, variable JOB_DONE_REGEX has %s" %(out, jobDoneRegex))
         # If nothing is returned we assume job is no longer in queue and thus finished
         if out == "":
+            logger.warning("Empty response from queue system to job (%s)" %jobid)
             return cts.STATUS_FINISHED
         # If some string is returned we use the JOB_DONE_REGEX variable (if present) to infer the status
         elif jobDoneRegex is not None:
             s = re.search(jobDoneRegex, out)
             if s:
+                logger.debug("Job (%s) finished" %jobid)
                 return cts.STATUS_FINISHED
             else:
+                logger.debug("Job (%s) still running" %jobid)
                 return cts.STATUS_RUNNING
         # If JOB_DONE_REGEX is not defined and queue has returned something we assume that job is still running
         else:
             return cts.STATUS_RUNNING
 
 
 class MPIStepExecutor(ThreadStepExecutor):
@@ -351,16 +371,28 @@
                   numberOfMpi, hostConfig=self.hostConfig, env=env, cwd=cwd,
                   gpuList=self.getGpuList())
 
     def runSteps(self, steps, 
                  stepStartedCallback, 
                  stepFinishedCallback,
                  checkStepsCallback,
-                 stepsCheckSecs=3):
-        ThreadStepExecutor.runSteps(self, steps, 
+                 stepsCheckSecs=5):
+        """
+        Creates mpiprocesses using numpy and synchronize the steps execution.
+
+        :param steps: list of steps to run
+        :param stepStartedCallback: callback to be called before starting any step
+        :param stepFinishedCallback: callback to be run after all steps are done
+        :param stepsCheckCallback: callback to check if there are new steps to add (streaming)
+        :param stepsCheckSecs: seconds between stepsCheckCallback calls
+
+        """
+
+
+        ThreadStepExecutor.runSteps(self, steps,
                                     stepStartedCallback, 
                                     stepFinishedCallback,
                                     checkStepsCallback,
                                     stepsCheckSecs=stepsCheckSecs)
 
         # Import mpi here so if MPI4py was not properly compiled
         # we can still run in parallel with threads.
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/protocol/hosts.py` & `scipion-pyworkflow-3.1.0/pyworkflow/protocol/hosts.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,120 +32,120 @@
 import os
 import sys
 import json
 from configparser import RawConfigParser
 from collections import OrderedDict
 
 import pyworkflow as pw
-from pyworkflow.object import OrderedObject, String, Integer, Boolean
+from pyworkflow.object import Object, String, Integer, Boolean
 
-        
-class HostConfig(OrderedObject):
+
+class HostConfig(Object):
     """ Main store the configuration for execution hosts. """
-    
+
     def __init__(self, **kwargs):
-        OrderedObject.__init__(self, **kwargs)
+        super().__init__(**kwargs)
         self.label = String(kwargs.get('label', None))
         self.hostName = String(kwargs.get('hostName', None))
         self.userName = String()
         self.password = String()
         self.hostPath = String()
         self.mpiCommand = String()
         self.scipionHome = String()
         self.scipionConfig = String()
         self.address = String()
         self.queueSystem = QueueSystemConfig()
-    
+
     def getLabel(self):
         return self.label.get()
-    
+
     def getHostName(self):
         return self.hostName.get()
-    
+
     def getUserName(self):
         return self.userName.get()
-    
+
     def getPassword(self):
         return self.password.get()
-    
+
     def getHostPath(self):
         return self.hostPath.get()
-    
+
     def getSubmitCommand(self):
         return self.queueSystem.submitCommand.get()
-    
+
     def getSubmitPrefix(self):
         return self.queueSystem.submitPrefix.get()
 
     def getCheckCommand(self):
         return self.queueSystem.checkCommand.get()
 
     def getCancelCommand(self):
         return self.queueSystem.cancelCommand.get()
-    
+
     def isQueueMandatory(self):
         return self.queueSystem.mandatory.get()
-    
+
     def getSubmitTemplate(self):
         return self.queueSystem.getSubmitTemplate()
-    
+
     def getQueuesDefault(self):
         return self.queueSystem.queuesDefault
-    
+
     def getMpiCommand(self):
         return self.mpiCommand.get()
-    
+
     def getQueueSystem(self):
         return self.queueSystem
 
     def getJobDoneRegex(self):
         return self.queueSystem.jobDoneRegex.get()
-    
+
     def setLabel(self, label):
         self.label.set(label)
-    
+
     def setHostName(self, hostName):
         self.hostName.set(hostName)
-    
+
     def setUserName(self, userName):
         self.userName.set(userName)
-    
+
     def setPassword(self, password):
         self.password.set(password)
-    
+
     def setHostPath(self, hostPath):
         self.hostPath.set(hostPath)
-    
+
     def setMpiCommand(self, mpiCommand):
-        self.mpiCommand.set(mpiCommand)  
-        
+        self.mpiCommand.set(mpiCommand)
+
     def setQueueSystem(self, queueSystem):
         self.queueSystem = queueSystem
-        
+
     def getScipionHome(self):
-        """ Return the path where Scipion is installed in 
+        """ Return the path where Scipion is installed in
         the host. This is useful when launching remote jobs.
-        """ 
+        """
         return self.scipionHome.get()
-    
+
     def setScipionHome(self, newScipionHome):
         self.scipionHome.set(newScipionHome)
-        
+
     def getScipionConfig(self):
-        """ From which file to read the configuration file in 
+        """ From which file to read the configuration file in
         this hosts. Useful for remote jobs.
         """
         return self.scipionConfig.get()
-    
+
     def setScipionConfig(self, newConfig):
         self.scipionConfig.set(newConfig)
-        
+
     def getAddress(self):
         return self.address.get()
-    
+
     def setAddress(self, newAddress):
         return self.address.set(newAddress)
 
     @classmethod
     def writeBasic(cls, configFn):
         """ Write a very basic Host configuration for testing purposes. """
         with open(configFn, 'w') as f:
@@ -218,21 +218,21 @@
                     hostQueue.queuesDefault = getDict('QUEUES_DEFAULT')
 
                 hosts[hostName] = host
 
             return hosts
         except Exception as e:
             sys.exit('Failed to read settings. The reported error was:\n  %s\n'
-                     'To solve it, delete %s and run again.'
+                     'Review %s and run again.'
                      % (e, os.path.abspath(hostsConf)))
 
 
-class QueueSystemConfig(OrderedObject):
+class QueueSystemConfig(Object):
     def __init__(self, **kwargs):
-        OrderedObject.__init__(self, **kwargs)
+        super().__init__(**kwargs)
         self.name = String()
         # Number of cores from which the queue is mandatory
         # 0 means no mandatory at all
         # 1 will force to launch all jobs through the queue
         self.mandatory = Integer()
         self.queues = None  # List for queue configurations
         self.submitCommand = String()
@@ -243,112 +243,112 @@
         self.checkCommand = String()
         self.cancelCommand = String()
         self.submitTemplate = String()
         self.jobDoneRegex = String()
 
     def hasName(self):
         return self.name.hasValue()
-    
+
     def hasValue(self):
         return self.hasName() and len(self.queues)
-    
+
     def getName(self):
         return self.name.get()
-    
+
     def getMandatory(self):
         return self.mandatory.get()
-    
+
     def getSubmitTemplate(self):
         return self.submitTemplate.get()
-    
+
     def getSubmitCommand(self):
         return self.submitCommand.get()
-    
+
     def getCheckCommand(self):
         return self.checkCommand.get()
-    
+
     def getCancelCommand(self):
         return self.cancelCommand.get()
-    
+
     def getQueues(self):
         return self.queues
-    
+
     def setName(self, name):
         self.name.set(name)
-    
+
     def setMandatory(self, mandatory):
         # This condition is to be backward compatible
         # when mandatory was a boolean
         # now it should use the number of CPU
         # that should force to use the queue
         if mandatory in ['False', 'false']:
             mandatory = 0
         elif mandatory in ['True', 'true']:
             mandatory = 1
-            
+
         self.mandatory.set(mandatory)
-    
+
     def setSubmitTemplate(self, submitTemplate):
         self.submitTemplate.set(submitTemplate)
-    
+
     def setSubmitCommand(self, submitCommand):
         self.submitCommand.set(submitCommand)
-    
+
     def setCheckCommand(self, checkCommand):
         self.checkCommand.set(checkCommand)
-    
+
     def setCancelCommand(self, cancelCommand):
         self.cancelCommand.set(cancelCommand)
 
     def setJobDoneRegex(self, jobDoneRegex):
         self.jobDoneRegex.set(jobDoneRegex)
-    
+
     def setQueues(self, queues):
         self.queues = queues
-        
+
     def getQueueConfig(self, objId):
         if objId is not None and self.queues is not None:
             for queueConfig in self.queues:
                 if objId == queueConfig.getObjId():
                     return queueConfig
         return None
-        
-        
+
+
 # TODO: maybe deprecated
-class QueueConfig(OrderedObject):
+class QueueConfig(Object):
     def __init__(self, **kwargs):
-        OrderedObject.__init__(self, **kwargs)
+        super().__init__(**kwargs)
         self.name = String('default')
         self.maxCores = Integer()
         self.allowMPI = Boolean()
         self.allowThreads = Boolean()
         self.maxHours = Integer()
-        
+
     def getName(self):
         return self.name.get()
-    
+
     def getMaxCores(self):
         return self.maxCores.get()
-    
+
     def getAllowMPI(self):
         return self.allowMPI.get()
-    
+
     def getAllowThreads(self):
         return self.allowThreads.get()
-    
+
     def getMaxHours(self):
         return self.maxHours.get()
-    
+
     def setName(self, name):
         self.name.set(name)
-    
+
     def setMaxCores(self, maxCores):
         self.maxCores.set(maxCores)
-        
+
     def setAllowMPI(self, allowMPI):
         self.allowMPI.set(allowMPI)
-    
+
     def setAllowThreads(self, allowThreads):
         self.allowThreads.set(allowThreads)
-    
+
     def setMaxHours(self, maxHours):
         self.maxHours.set(maxHours)
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/protocol/launch.py` & `scipion-pyworkflow-3.1.0/pyworkflow/protocol/launch.py`

 * *Files 24% similar despite different names*

```diff
@@ -38,16 +38,19 @@
 2- Copy necessary files to remote host.
 3- Run a local process (for local execution, see case A) in the remote host
 4- Get the result back after launching remotely
 """
 
 import os
 import re
+import logging
+logger = logging.getLogger(__file__)
 from subprocess import Popen, PIPE
 import pyworkflow as pw
+from pyworkflow.exceptions import PyworkflowException
 from pyworkflow.utils import (redStr, greenStr, makeFilePath, join, process,
                               getHostFullName)
 from pyworkflow.protocol.constants import UNKNOWN_JOBID
 
 LOCALHOST = 'localhost'
 
 
@@ -74,22 +77,24 @@
     """
     if _isLocal(protocol):
         return _stopLocal(protocol)
     else:
         return _stopRemote(protocol)
 
 
-def schedule(protocol, wait=False):
+def schedule(protocol, initialSleepTime=0, wait=False):
     """ Use this function to schedule protocols that are not ready to
     run yet. Right now it only make sense to schedule jobs locally.
     """
     cmd = '%s %s' % (pw.PYTHON, pw.getScheduleScript())
-    cmd += ' "%s" "%s" %s' % (protocol.getProject().path,
+    cmd += ' "%s" "%s" %s "%s" --initial_sleep %s' % (protocol.getProject().path,
                               protocol.getDbPath(),
-                              protocol.strId())
+                              protocol.strId(),
+                              protocol.getScheduleLog(),
+                              initialSleepTime)
     jobId = _run(cmd, wait)
     protocol.setJobId(jobId)
 
     return jobId
 
 
 # ******************************************************************
@@ -112,21 +117,50 @@
 def _getAppsProgram(prog):
     """ Get a command to launch a program under the apps folder.
     """
     return "%s %s" % (pw.PYTHON, pw.join(pw.APPS, prog))
 
 
 def _launchLocal(protocol, wait, stdin=None, stdout=None, stderr=None):
-    # Check first if we need to launch with MPI or not
-    command = ('%s %s "%s" "%s" %s'
-               % (pw.PYTHON, pw.join(pw.APPS, 'pw_protocol_run.py'),
-                  protocol.getProject().path, protocol.getDbPath(),
-                  protocol.strId()))
+    """
+
+    :param protocol: Protocol to launch
+    :param wait: Pass true if you want to wait for the process to finish
+    :param stdin: stdin object to direct stdin to
+    :param stdout: stdout object to send process stdout
+    :param stderr: stderr object to send process stderr
+    :return: PID of queue's JOBID
+    """
+
+    command = '{python} {prot_run} "{project_path}" "{db_path}" {prot_id} "{stdout_log}" "{stderr_log}"'.format(
+        python=pw.PYTHON,
+        prot_run=pw.join(pw.APPS, 'pw_protocol_run.py'),
+        project_path=protocol.getProject().path,
+        db_path=protocol.getDbPath(),
+        prot_id=protocol.strId(),
+        # We make them absolute in case working dir is not passed to the node when running through a queue.
+        # The reason is that since 3.0.27, the first thing that is affected by the current working dir is the
+        # creation of the logs. Before event than loading the project, which was and is setting the working dir to
+        # the project path. IMPORTANT: This assumes the paths before the queue and after the queue (nodes) are the same
+        # Which I think is safe since we are passing here "project_path" that is absolute.
+        stdout_log=os.path.abspath(protocol.getStdoutLog()),
+        stderr_log=os.path.abspath(protocol.getStderrLog())
+    )
+
+    #command = ('%s %s "%s" "%s" %s "%s" "%s"'
+    #           % (pw.PYTHON, pw.join(pw.APPS, 'pw_protocol_run.py'),
+    #              protocol.getProject().path, protocol.getDbPath(),
+    #              protocol.strId()))
+
     hostConfig = protocol.getHostConfig()
     useQueue = protocol.useQueue()
+
+    # Empty PID: 0
+    protocol.setPid(0)
+
     # Check if need to submit to queue    
     if useQueue and (protocol.getSubmitDict()["QUEUE_FOR_JOBS"] == "N"):
         submitDict = dict(hostConfig.getQueuesDefault())
         submitDict.update(protocol.getSubmitDict())
         submitDict['JOB_COMMAND'] = command
         jobId = _submit(hostConfig, submitDict)
     else:
@@ -159,15 +193,15 @@
             'scipion': host.getScipionHome(),
             'config': host.getScipionConfig(),
             'project': projectPath,
             'protDb': protocol.getDbPath(),
             'protId': protocol.getObjId()
             }
     cmd = tpl % args
-    print("** Running remote: %s" % greenStr(cmd))
+    logger.info("** Running remote: %s" % greenStr(cmd))
     p = Popen(cmd, shell=True, stdout=PIPE)
 
     return p
 
 
 def _launchRemote(protocol, wait):
     p = _runRemote(protocol, 'run')
@@ -197,53 +231,89 @@
     remotePath = protocol.getHostConfig().getHostPath()
 
     for f in protocol.getFiles():
         remoteFile = join(remotePath, f)
         rpath.putFile(f, remoteFile)
 
 
+def analyzeFormattingTypeError(string, dictionary):
+    """ receives a string with %(VARS) to be replaced with a dictionary
+     it splits te string by \n and test the formatting per line. Raises an exception if any line fails
+     with all problems found"""
+
+    # Do the replacement line by line
+    lines = string.split("\n")
+
+    problematicLines = []
+    for line in lines:
+        try:
+            line % dictionary
+        except KeyError as e:
+            problematicLines.append(line + " --> variable not present in this context.")
+        except Exception as e:
+            problematicLines.append(line + " --> " + str(e))
+
+    if problematicLines:
+        return PyworkflowException('Following lines in %s seems to be problematic.\n'
+                                   'Values known in this context are: \n%s'
+                                   'Please review its format or content.\n%s' % (dictionary, pw.Config.SCIPION_HOSTS, "\n".join(problematicLines)),
+                                   url=pw.DOCSITEURLS.HOST_CONFIG)
+
 def _submit(hostConfig, submitDict, cwd=None, env=None):
     """ Submit a protocol to a queue system. Return its job id.
     """
     # Create first the submission script to be launched
     # formatting using the template
-    template = hostConfig.getSubmitTemplate() % submitDict
+    template = hostConfig.getSubmitTemplate()
+
+    try:
+        template = template % submitDict
+    except Exception as e:
+        # Capture parsing errors
+        exception = analyzeFormattingTypeError(template, submitDict)
+
+        if exception:
+            raise exception
+        else:
+            # If there is no exception, then raise actual one
+            raise e
+
     # FIXME: CREATE THE PATH FIRST
     scripPath = submitDict['JOB_SCRIPT']
     f = open(scripPath, 'w')
     # Ensure the path exists
     makeFilePath(scripPath)
     # Add some line ends because in some clusters it fails
     # to submit jobs if the submit script does not have end of line
     f.write(template + '\n\n')
     f.close()
     # This should format the command using a template like: 
     # "qsub %(JOB_SCRIPT)s"
     command = hostConfig.getSubmitCommand() % submitDict
     gcmd = greenStr(command)
-    print("** Submitting to queue: '%s'" % gcmd)
+    logger.info("** Submitting to queue: '%s'" % gcmd)
 
     p = Popen(command, shell=True, stdout=PIPE, cwd=cwd, env=env)
     out = p.communicate()[0]
     # Try to parse the result of qsub, searching for a number (jobId)
     # Review this, seems to exclusive to torque batch system
     s = re.search('(\d+)', str(out))
     if p.returncode == 0 and s:
         job = int(s.group(0))
-        print("Launched job with id %s" % job)
+        logger.info("Launched job with id %s" % job)
         return job
     else:
-        print("Couldn't submit to queue for reason: %s " % redStr(out.decode()))
+        logger.info("Couldn't submit to queue for reason: %s " % redStr(out.decode()))
         return UNKNOWN_JOBID
 
 
 def _run(command, wait, stdin=None, stdout=None, stderr=None):
     """ Execute a command in a subprocess and return the pid. """
     gcmd = greenStr(command)
-    print("** Running command: '%s'" % gcmd)
+    logger.info("** Running command: '%s'" % gcmd)
     p = Popen(command, shell=True, stdout=stdout, stderr=stderr)
     jobId = p.pid
     if wait:
         p.wait()
 
     return jobId
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/protocol/package.py` & `scipion-pyworkflow-3.1.0/pyworkflow/protocol/package.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/protocol/params.py` & `scipion-pyworkflow-3.1.0/pyworkflow/protocol/params.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,21 +26,21 @@
 import re
 import collections
 
 from pyworkflow.object import *
 from .constants import *
 
 
-class FormElement(OrderedObject):
+class FormElement(Object):
     """Base for any element on the form"""
     ATTRIBUTES = ['label', 'expertLevel', 'condition', 'important', 'help',
                   'default', 'paramClass']
     
     def __init__(self, **args):
-        OrderedObject.__init__(self, **args)
+        super().__init__(**args)
         self.label = String(args.get('label', None))
         self.expertLevel = Integer(args.get('expertLevel', LEVEL_NORMAL))
         self.condition = String(args.get('condition', None))
         self._isImportant = Boolean(args.get('important', False))
         self.help = String(args.get('help', None))
         # This two list will be filled by the Form
         # which have a global-view of all parameters
@@ -87,14 +87,15 @@
         # This should be defined in subclasses
         self.paramClass = args.get('paramClass', None)
         self.default = String(args.get('default', None))
 
         # Allow pointers (used for scalars)
         self.allowsPointers = args.get('allowsPointers', False)
         self.validators = args.get('validators', [])
+        self.readOnly = args.get("readOnly", False)
         
     def __str__(self):
         return "    label: %s" % self.label.get()
     
     def addValidator(self, validator):
         """ Validators should be callables that 
         receive a value and return a list of errors if so.
@@ -228,15 +229,19 @@
         """ Register a given param in the form. """
         self._paramsDict[paramName] = param        
         self._analizeCondition(paramName, param)
         
     def addParam(self, *args, **kwargs):
         """Add a new param to last section"""
         return self.lastSection.addParam(*args, **kwargs)
-    
+
+    # Adhoc method for specific params
+    def addBooleanParam(self, name, label, help, default=True, **kwargs):
+        return self.addParam(name, BooleanParam, label=label, help=help, default=default, **kwargs)
+
     def addHidden(self, *args, **kwargs):
         return self.lastSection.addHidden(*args, **kwargs)
     
     def _analizeCondition(self, paramName, param):
         if param.hasCondition():
             param._conditionParams = []
             tokens = re.split('\W+', param.condition.get())
@@ -326,29 +331,35 @@
                            'of this particular run and start from the beginning. This option'
                            'should be used carefully.'
                       )
   
     def addParallelSection(self, threads=1, mpi=8, condition="",
                            hours=72, jobsize=0):
 
+        """ Adds the parallelization section to the form
+            pass threads=0 to disable threads parameter and mpi=0 to disable mpi params
+
+        :param threads: default value for of threads, defaults to 1
+        :param mpi: default value for mpi, defaults to 8"""
+
         self.addSection(label='Parallelization')
         self.addParam('hostName', StringParam, default="localhost",
                       label='Execution host',
                       help='Select in which of the available do you want to launch this protocol.')
         if threads > 0:
             self.addParam('numberOfThreads', IntParam, default=threads,
                           label='Threads',
                           help='This option provides shared-memory parallelization on multi-core machines.'
-                                'It does not require any additional software, other than <Xmipp>')
+                                'It does not require any additional software.')
         if mpi > 0:
             self.addParam('numberOfMpi', IntParam, default=mpi,
                           label='MPI processes',
                           help='This option provides the number of independent processes spawned'
                                 'in parallel by <mpirun> command in a cluster, usually through'
-                                'a queue system. This will require that you have compile <Xmipp>'
+                                'a queue system. This will require that you have compile this software '
                                 'with <mpi> support.')
         if jobsize > 0:
             self.addParam('mpiJobSize', IntParam, default=jobsize,
                           label='MPI job size', condition="numberOfMpi>1",
                           help='Minimum size of jobs in mpi processes.'
                                'Set to 1 for large images (e.g. 500x500)'
                                'and to 10 for small images (e.g. 100x100)')
@@ -421,16 +432,25 @@
     def __init__(self, **args):
         Param.__init__(self, paramClass=Float, **args)
         self.addValidator(Format(float, error="should be a float",
                                  allowsNull=args.get('allowsNull', False)))
 
         
 class BooleanParam(Param):
-    def __init__(self, **args):
+    """ Param to store boolean values. By default it will be displayed as 2 radio buttons with Yes/no labels.
+    Alternatively, if you pass checkbox it will be displayed as a checkbox.
+
+    :param display: (Optional) default DISPLAY_YES_NO.  (Yes /no)
+                    Alternatively use BooleanParam.DISPLAY_CHECKBOX to use checkboxes """
+    DISPLAY_YES_NO = 1
+    DISPLAY_CHECKBOX = 2
+
+    def __init__(self, display=DISPLAY_YES_NO, **args):
         Param.__init__(self, paramClass=Boolean, **args)
+        self.display = display
         self.addValidator(NonEmptyBool)
 
 
 class HiddenBooleanParam(BooleanParam):
     def __init__(self, **args):
         Param.__init__(self, paramClass=Boolean, **args)
 
@@ -438,27 +458,36 @@
 class PointerParam(Param):
     """ This type of Param will serve to select existing objects
     in the database that will be input for some protocol.
     """
     def __init__(self,  paramClass=Pointer, **args):
         Param.__init__(self, paramClass=paramClass, **args)
         # This will be the class to be pointed
-        pointerClass = args.get('pointerClass')
-        if ',' in pointerClass:
-            self.pointerClass = CsvList()
-            self.pointerClass.set(pointerClass)
-        else:
-            self.pointerClass = String(pointerClass) 
-
+        self.setPointerClass(args['pointerClass'])
         # Some conditions on the pointed candidates
         self.pointerCondition = String(args.get('pointerCondition', None))
         self.allowsNull = Boolean(args.get('allowsNull', False))
         
     def setPointerClass(self, newPointerClass):
-        self.pointerClass.set(newPointerClass)
+
+        # Tolerate passing classes instead of their names
+        if isinstance(newPointerClass, list):
+            self.pointerClass = CsvList()
+            self.pointerClass.set(",". join([clazz.__name__ for clazz in newPointerClass]))
+
+        elif(isinstance(newPointerClass, str)):
+            if ',' in newPointerClass:
+                self.pointerClass = CsvList()
+                self.pointerClass.set(newPointerClass)
+            else:
+                self.pointerClass = String(newPointerClass)
+
+        # Single class item, not the string
+        else:
+            self.pointerClass = String(newPointerClass.__name__)
 
 
 class MultiPointerParam(PointerParam):
     """ This type of Param will serve to select objects
     with DIFFERENT types from the database to be input for some protocol.
     """
     def __init__(self, **args):
@@ -520,33 +549,77 @@
     def __init__(self, **args):
         StringParam.__init__(self, **args)
         self.addValidator(NumericListValidator())
         
         
 class NumericRangeParam(StringParam):
     """ This class will serve to specify range of numbers with a string representation.
-     Possible notation are:
+     Possible notation are::
+
         "1,5-8,10" -> [1,5,6,7,8,10]
         "2,6,9-11" -> [2,6,9,10,11]
         "2 5, 6-8" -> [2,5,6,7,8]
+
     """
     def __init__(self, **args):
         StringParam.__init__(self, **args)
-        # TODO: ADD a syntax validator
+        self.addValidator(NumericRangeValidator())
         
         
 class TupleParam(Param):
     """ This class will condense a tuple of several
     other params of the same type and related concept.
     For example: min and max, low and high.
     """
     def __init__(self, **args):
         Param.__init__(self, **args)
 
 
+class DeprecatedParam:
+    """ Deprecated param. To be used when you want to rename an existing param
+    and still be able to recover old param value. It acts like a redirector, passing the
+    value received when its value is set to the new renamed parameter
+
+    usage: In defineParams method, before the renamed param definition line add the following:
+
+    self.oldName = DeprecatedParam("newName", self)
+    form.addParam('newName', ...)
+
+    """
+    def __init__(self, newParamName, prot):
+        """
+
+        :param newParamName: Name of the renamed param
+        :param prot: Protocol hosting this and the renamed param
+
+        """
+        self._newParamName = newParamName
+        self.prot = prot
+        # Need to fake being a Object at loading time
+        self._objId = None
+        self._objIsPointer = False
+
+    def set(self, value, cleanExtended=False):
+        if hasattr(self.prot, self._newParamName):
+            newParam = self._getNewParam()
+            if newParam.isPointer():
+                newParam.set(value, cleanExtended)
+                self._extended = newParam._extended
+            else:
+                newParam.set(value)
+
+    def isPointer(self):
+        return self._getNewParam().isPointer()
+
+    def getObjValue(self):
+        return None
+
+    def _getNewParam(self):
+        return getattr(self.prot, self._newParamName)
+
 # -----------------------------------------------------------------------------
 #         Validators
 # -----------------------------------------------------------------------------
 class Validator(object):
     pass
 
 
@@ -608,37 +681,54 @@
         Conditional.__init__(self, error)
         self._condition = lambda value: value > threshold
 
 
 class GE(Conditional):
     def __init__(self, thresold, error='Value should be greater or equal than the threshold'):
         Conditional.__init__(self, error)
-        self._condition = lambda value: value >= thresold               
+        self._condition = lambda value: value is not None and value >= thresold
 
 
 class Range(Conditional):
     def __init__(self, minValue, maxValue, error='Value is outside range'):
         Conditional.__init__(self, error)
         self._condition = lambda value: minValue <= value <= maxValue
         
         
 class NumericListValidator(Conditional):
     """ Validator for ListParam. See ListParam. """
-    def __init__(self, error='Incorrect format for numeric list param. '):
+    def __init__(self, error='Incorrect format for numeric list param'):
         Conditional.__init__(self, error)
         
     def _condition(self, value):
         try:
-            value = value.replace('x', '')
-            parts = value.split()
+            parts = re.split(r"[x\s]", value)
+            parts = list(filter(None, parts))
+            for p in parts:
+                float(p)
+            return True
+        except Exception:
+            return False
+
+
+class NumericRangeValidator(Conditional):
+    """ Validator for RangeParam. See RangeParam. """
+
+    def __init__(self, error='Incorrect format for numeric range param'):
+        Conditional.__init__(self, error)
+
+    def _condition(self, value):
+        try:
+            parts = re.split(r"[-,\s]", value)
+            parts = list(filter(None, parts))
             for p in parts:
                 float(p)
             return True
         except Exception:
-            return False    
+            return False
 
 
 class NonEmptyBoolCondition(Conditional):
     def __init__(self, error='Boolean param needs to be set.'):
         Conditional.__init__(self, error)
         self._condition = lambda value: value is not None
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/protocol/protocol.py` & `scipion-pyworkflow-3.1.0/pyworkflow/protocol/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,39 +21,44 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 """
 This modules contains classes required for the workflow
 execution and tracking like: Step and Protocol
 """
-import sys
+import sys, os
 import json
+import threading
 import time
 
 import pyworkflow as pw
 from pyworkflow.exceptions import ValidationException, PyworkflowException
 from pyworkflow.object import *
 import pyworkflow.utils as pwutils
-from pyworkflow.utils.log import ScipionLogger
+from pyworkflow.utils.log import LoggingConfigurator, getExtraLogInfo, STATUS, setDefaultLoggingContext
 from .executor import (StepExecutor, ThreadStepExecutor, MPIStepExecutor,
                        QueueStepExecutor)
 from .constants import *
 from .params import Form
+from ..utils import getFileSize
 
-SCHEDULE_LOG = 'schedule.log'
 
+import  logging
+# Get the root logger
+logger = logging.getLogger(__name__)
 
-class Step(OrderedObject):
+
+class Step(Object):
     """ Basic execution unit.
     It should defines its Input, Output
     and define a run method.
     """
 
     def __init__(self, **kwargs):
-        OrderedObject.__init__(self, **kwargs)
+        Object.__init__(self, **kwargs)
         self._prerequisites = CsvList()  # which steps needs to be done first
         self.status = String()
         self.initTime = String()
         self.endTime = String()
         self._error = String()
         self.interactive = Boolean(False)
         self._resultFiles = String()
@@ -104,23 +109,30 @@
         return self._error
 
     def getErrorMessage(self):
         return self.getError().get('')
 
     def setFailed(self, msg):
         """ Set the run failed and store an error message. """
-        self.endTime.set(dt.datetime.now())
-        self._error.set(msg)
-        self.status.set(STATUS_FAILED)
+        self._finalizeStep(STATUS_FAILED, msg=msg)
 
     def setAborted(self):
-        """ Set the status to aborted and updated the endTime. """
+        """ Set the status to aborted and updates the endTime. """
+        self._finalizeStep(STATUS_ABORTED, "Aborted by user.")
+
+    def setFinished(self):
+        """ Set the status to finish updates the end time """
+        self._finalizeStep(STATUS_FINISHED)
+
+    def _finalizeStep(self, status, msg=None):
+        """ Closes the step, setting up the endTime and optionally an error message"""
         self.endTime.set(dt.datetime.now())
-        self._error.set("Aborted by user.")
-        self.status.set(STATUS_ABORTED)
+        if msg:
+            self._error.set(msg)
+        self.status.set(status)
 
     def setSaved(self):
         """ Set the status to saved and updated the endTime. """
         self.initTime.set(None)
         self.endTime.set(None)
         self.status.set(STATUS_SAVED)
         self._error.set(None)  # Clean previous error message
@@ -145,14 +157,17 @@
             elapsed = t2 - t1
 
         return elapsed
 
     def setStatus(self, value):
         return self.status.set(value)
 
+    def isNew(self):
+        return self.getStatus() == STATUS_NEW
+
     def setInteractive(self, value):
         return self.interactive.set(value)
 
     def isActive(self):
         return self.getStatus() in ACTIVE_STATUS
 
     def isFinished(self):
@@ -309,48 +324,62 @@
     """ The Protocol is a higher type of Step.
     It also have the inputs, outputs and other Steps properties,
     but contains a list of steps that are executed
     """
 
     # Version where protocol appeared first time
     _lastUpdateVersion = pw.VERSION_1
-    _stepsCheckSecs = 3
+    _stepsCheckSecs = pw.Config.getStepsCheckSeconds()
+    # Protocol develop status: PROD, BETA, NEW
+    _devStatus = pw.PROD
+
+    """" Possible Outputs:
+    This is an optional but recommended attribute to fill.
+    It has to be an enum with names being the name of the output and value the class of the output:
+    
+        class MyOutput(enum.Enum):
+            outputMicrographs = SetOfMicrographs
+            outputMicrographDW = SetOfMicrographs
+    
+    When defining outputs you can, optionally, use this enum like:
+    self._defineOutputs(**{MyOutput.outputMicrographs.name, setOfMics})
+    It will help to keep output names consistently
+    
+    Alternative an inline dictionary will work:
+    _possibleOutputs = {"outputMicrographs" : SetOfMicrographs}
+    
+    For a more fine detailed/dynamic output based on parameters, you can overwrite the getter:
+    getPossibleOutputs() in your protocol.
+    
+    """
+    _possibleOutputs = None
+
+    # Cache package and plugin
+    _package = None
+    _plugin = None
 
     def __init__(self, **kwargs):
         Step.__init__(self, **kwargs)
+        self._size = None
         self._steps = []  # List of steps that will be executed
+        self._newSteps = False  # Boolean to annotate when there are new steps added to the above list. And need persistence.
         # All generated filePaths should be inside workingDir
         self.workingDir = String(kwargs.get('workingDir', '.'))
         self.mapper = kwargs.get('mapper', None)
         self._inputs = []
         self._outputs = CsvList()
         # This flag will be used to annotate it output are already "migrated"
         #  and available in the _outputs list. Therefore iterating
         self._useOutputList = Boolean(False)
         # Expert level needs to be defined before parsing params
         self.expertLevel = Integer(kwargs.get('expertLevel', LEVEL_NORMAL))
         self._definition = Form(self)
         self._defineParams(self._definition)
         self._createVarsFromDefinition(**kwargs)
-        self.__stdOut = None
-        self.__stdErr = None
-        self.__fOut = None
-        self.__fErr = None
-
-        class BasicLog:
-            def warning(self, message, redirectStandard=True):
-                print("WARNING", message)
-
-            def info(self, message, redirectStandard=True):
-                print("INFO", message)
-
-            def error(self, message, redirectStandard=True):
-                print("ERROR", message)
-
-        self._log = BasicLog()
+        self._log = logger
         self._buffer = ''  # text buffer for reading log files
         # Project to which the protocol belongs
         self.__project = kwargs.get('project', None)
         # Filename templates dict that will be used by _getFileName
         self.__filenamesDict = {}
 
         # This will be used at project load time to check if
@@ -392,26 +421,30 @@
         # and queue parameters (only meaningful if _useQueue=True)
         self._queueParams = String()
         self.queueShown = False
         self._jobId = String()  # Store queue job id
         self._pid = Integer()
         self._stepsExecutor = None
         self._stepsDone = Integer(0)
+        self._cpuTime = Integer(0)
         self._numberOfSteps = Integer(0)
         # For visualization
         self.allowHeader = Boolean(True)
         # Create an String variable to allow some protocol to precompute
         # the summary message
         self.summaryVar = String()
         self.methodsVar = String()
         # Create a variable to know if the protocol has expert params
         self._hasExpert = None
 
         # Store warnings here
         self.summaryWarnings = []
+        # Get a lock for threading execution
+        self._lock = threading.Lock()
+        self.forceSchedule = Boolean(False)
 
     def _storeAttributes(self, attrList, attrDict):
         """ Store all attributes in attrDict as
         attributes of self, also store the key in attrList.
         """
         for key, value in attrDict.items():
             if key not in attrList:
@@ -437,49 +470,59 @@
         self._storeAttributes(self._outputs, kwargs)
 
         # Persist outputs list
         self._insertChild("_outputs", self._outputs)
         self._useOutputList.set(True)
         self._insertChild("_useOutputList", self._useOutputList)
 
+    def _closeOutputSet(self):
+        """Close all output set"""
+        for outputName, output in self.iterOutputAttributes():
+            if isinstance(output, Set) and output.isStreamOpen():
+                self.__tryUpdateOutputSet(outputName, output, state=Set.STREAM_CLOSED)
+
     def _updateOutputSet(self, outputName, outputSet,
                          state=Set.STREAM_OPEN):
         """ Use this function when updating an Stream output set.
         """
-        self.__tryUpdateOuputSet(outputName, outputSet, state)
+        self.__tryUpdateOutputSet(outputName, outputSet, state)
 
-    def __tryUpdateOuputSet(self, outputName, outputSet,
-                            state=Set.STREAM_OPEN, tries=1):
+    def __tryUpdateOutputSet(self, outputName, outputSet,
+                            state=Set.STREAM_OPEN, tries=1, firstException=None):
         try:
             # Update the set with the streamState value (either OPEN or CLOSED)
             outputSet.setStreamState(state)
 
             if self.hasAttribute(outputName):
                 outputSet.write()  # Write to commit changes
                 outputAttr = getattr(self, outputName)
                 # Copy the properties to the object contained in the protocol
-                outputAttr.copy(outputSet, copyId=False)
+                # Default Set.copy ignores some attributes like size or mapperPath.
+                # In this case we want all to be copied
+                outputAttr.copy(outputSet, copyId=False, ignoreAttrs=[])
                 # Persist changes
                 self._store(outputAttr)
             else:
                 # Here the defineOutputs function will call the write() method
                 self._defineOutputs(**{outputName: outputSet})
                 self._store(outputSet)
             # Close set database to avoid locking it
             outputSet.close()
 
         except Exception as ex:
-            print("Error trying to update output of protocol, tries=%d" % tries)
 
-            if tries > 3:
-                raise ex
+            if tries > pw.Config.getUpdateSetAttempts():
+                raise BlockingIOError("Can't update %s (output) of %s after %s attempts. Reason: %s. "
+                                      "Concurrency, a non writable file system or a quota exceeded could be among the causes." %
+                                      (outputName, self,tries-1, ex)) from firstException
             else:
-                time.sleep(tries)
-                self.__tryUpdateOuputSet(outputName, outputSet, state,
-                                         tries + 1)
+                logger.warning("Trying to update %s (output) of protocol %s, attempt=%d: %s " % (outputName, self, tries, ex))
+                time.sleep(pw.Config.getUpdateSetAttemptsWait())
+                self.__tryUpdateOutputSet(outputName, outputSet, state,
+                                          tries + 1, firstException= ex if tries==1 else firstException)
 
     def hasExpert(self):
         """ This function checks if the protocol has
         any expert parameter"""
         if self._hasExpert is None:
             self._hasExpert = False
             for paraName, param in self._definition.iterAllParams():
@@ -500,38 +543,43 @@
         """ Check if the protocol has some definition.
         This can help to detect "abstract" protocol that
         only serve as base for other, not to be instantiated.
         """
         return hasattr(cls, '_definition')
 
     @classmethod
-    def getLastUpdateVersion(cls):
-        return cls._lastUpdateVersion
+    def isNewDev(cls):
+        if cls._devStatus == pw.NEW:
+            return True
+
+    @classmethod
+    def isBeta(cls):
+        return cls._devStatus == pw.BETA
 
     @classmethod
-    def isNew(cls):
-        version = cls.getLastUpdateVersion()
-        return version not in pw.OLD_VERSIONS
+    def isUpdated(cls):
+        return cls._devStatus == pw.UPDATED
 
     def getDefinition(self):
         """ Access the protocol definition. """
         return self._definition
 
     def getParam(self, paramName):
         """ Return a _definition param give its name. """
         return self._definition.getParam(paramName)
 
     def getEnumText(self, paramName):
         """ This function will retrieve the text value
         of an enum parameter in the definition, taking the actual value in
         the protocol.
-        Params:
-            paramName: the name of the enum param.
-        Returns:
-            the string value corresponding to the enum choice.
+
+        :param paramName: the name of the enum param.
+
+        :returns: the string value corresponding to the enum choice.
+
         """
         index = getattr(self, paramName).get()
         return self.getParam(paramName).choices[index]
 
     def evalParamCondition(self, paramName):
         """ Eval if the condition of paramName in _definition
         is satisfied with the current values of the protocol attributes.
@@ -609,16 +657,17 @@
                     # to group them inside the same tree element
                     yield key, item
             if attr.isPointer() and attr.hasValue():
                 yield key, attr
 
             # Consider here scalars with pointers inside
             elif isinstance(attr, Scalar) and attr.hasPointer():
-                if attr.get() is not None:
-                    yield key, attr.getPointer()
+                # Scheduling was stale cause this Scalar with pointers where not returned
+                #if attr.get() is not None:
+                yield key, attr.getPointer()
 
     def iterInputPointers(self):
         """ This function is similar to iterInputAttributes, but it yields
         all input Pointers, independently if they have value or not.
         """
         for key, attr in self.getAttributes():
             if not isinstance(attr, Object):
@@ -629,89 +678,95 @@
                     # the same key is returned for all items inside the
                     # PointerList, this is used in viewprotocols.py
                     # to group them inside the same tree element
                     yield key, item
             elif attr.isPointer():
                 yield key, attr
 
-    def inputProtocolDict(self):
+    def getProtocolsToUpdate(self):
         """
-        This function returns a dictionary of protocols that need to update
+        This function returns a list of protocols ids that need to update
         their database to launch this protocol (this method is only used
         when a WORKFLOW is restarted or continued).
         Actions done here are:
-        1. Iterate over the main input Pointer of this protocol
-           (here, 3 different cases are analyzed)
 
-           A) When the pointer points to a protocol
+        #. Iterate over the main input Pointer of this protocol
+            (here, 3 different cases are analyzed):
 
-           B) When the pointer points to another object (INDIRECTLY).
-              - The pointer has an _extended value (new parameters configuration
+            A #. When the pointer points to a protocol
+
+            B #. When the pointer points to another object (INDIRECTLY).
+                The pointer has an _extended value (new parameters configuration
                 in the protocol)
 
-           C) When the pointer points to another object (DIRECTLY).
+            C #. When the pointer points to another object (DIRECTLY).
+
               - The pointer has not an _extended value (old parameters
                 configuration in the protocol)
 
-        2. The PROTOCOL to which the pointer points is determined and saved in
-           the dictionary
+        #. The PROTOCOL to which the pointer points is determined and saved in
+            the list
+
+        #. If this pointer points to a set (case B and C):
 
-        3. If this pointer points to another object (case B and C):
-           - Iterate over the main attributes of this pointer
-           - if any attribute is a pointer, then we move to PROTOCOL and repeat
-             this procedure from step 1
+          - Iterate over the main attributes of the set
+            - if attribute is a pointer then we add the pointed protocol to the ids list
         """
-        protocolDict = {}
+        protocolIds = []
         protocol = None
         for key, attrInput in self.iterInputAttributes():
             output = attrInput.get()
             if isinstance(output, Protocol):  # case A
                 protocol = output
-                output = None
             else:
                 if attrInput.hasExtended():  # case B
                     protocol = attrInput.getObjValue()
                 else:  # case C
 
                     if self.getProject() is not None:
-
-                        protocol = self.getProject().getProtocol(output.getObjParentId())
+                        protocol = self.getProject().getRunsGraph(refresh=True).getNode(str(output.getObjParentId())).run
                     else:
                         # This is a problem, since protocols coming from
                         # Pointers do not have the __project set.
-                        # We do not have an clear way to get the protocol if
+                        # We do not have a clear way to get the protocol if
                         # we do not have the project object associated
                         # This case implies Direct Pointers to Sets
                         # (without extended): hopefully this will only be
                         # created from tests
-                        print("Can't get protocol info from input attribute."
+                        logger.warning("Can't get %s info from %s."
                               " This could render unexpected results when "
-                              "scheduling protocols.")
+                              "scheduling protocols. Value: %s" % (key, self, attrInput))
                         continue
 
+                # If there is output
                 if output is not None:
+                    # For each output attribute: Looking for pointers like SetOfCoordinates.micrographs
                     for k, attr in output.getAttributes():
+                        # If it's a pointer
                         if isinstance(attr, Pointer):
-                            if attr.get() is not None:
-                                auxDict = protocol.inputProtocolDict()
-                                for auxKey in auxDict:
-                                    if auxKey not in protocolDict.keys():
-                                        protocolDict[auxKey] = auxDict[auxKey]
-                                break
-
-            protocolDict[protocol.getObjId()] = protocol
-
-        return protocolDict
-
-    def hasLinkedInputs(self):
-        """ Return if True if some of the input pointers are referring to
-        an output that is not ready yet.
-        """
-        linkedPointers = []
-        emptyPointers = []
+                            logger.debug("Pointer found in output: %s.%s (%s)" % (output, k, attr))
+                            prot = attr.getObjValue()
+                            if prot is not None:
+                                if isinstance(prot, Protocol):
+                                    protocolIds.append(prot.getObjId())
+                                else:
+                                    logger.warning(f"We have found that {output}.{key} points to {attr} "
+                                                   f"and is a direct pointer. Direct pointers are less reliable "
+                                                   f"in streaming scenarios. Developers should avoid them.")
+            protocolIds.append(protocol.getObjId())
+
+        return protocolIds
+
+    def getInputStatus(self):
+        """ Returns if any input pointer is not ready yet and if there is
+         any pointer to an open set
+        """
+        emptyPointers = False
+        openSetPointer = False
+        emptyInput = False
 
         for paramName, attr in self.iterInputPointers():
 
             param = self.getParam(paramName)
             # Issue #1597: New data loaded with old code.
             # If the input pointer is not a param:
             # This could happen in backward incompatibility cases,
@@ -722,32 +777,52 @@
                       "This could happen when loading new code with older "
                       "scipion versions." % paramName)
                 continue
 
             condition = self.evalParamCondition(paramName)
 
             obj = attr.get()
+            if isinstance(obj, Protocol) and obj.getStatus() == STATUS_SAVED:  # the pointer points to a protocol
+                emptyPointers = True
+            if obj is None and attr.hasValue():
+                emptyPointers = True
             if condition and obj is None and not param.allowsNull:
-                if attr.hasValue():
-                    linkedPointers.append(paramName)
-                else:
-                    emptyPointers.append(paramName)
+                if not attr.hasValue():
+                   emptyInput = True
 
-        return linkedPointers and not emptyPointers
+            if not self.worksInStreaming() and isinstance(obj, Set) and obj.isStreamOpen():
+                openSetPointer = True
 
-    def iterOutputAttributes(self, outputClass=None):
+        return emptyInput, openSetPointer, emptyPointers
+
+    def iterOutputAttributes(self, outputClass=None, includePossible=False):
         """ Iterate over the outputs produced by this protocol. """
 
         iterator = self._iterOutputsNew if self._useOutputList else self._iterOutputsOld
 
-        # Iterate
+        hasOutput=False
+
+        # Iterate through actual outputs
         for key, attr in iterator():
             if outputClass is None or isinstance(attr, outputClass):
+                hasOutput = True
                 yield key, attr
 
+        # NOTE: This will only happen in case there is no actual output.
+        # There is no need to avoid duplication of actual output and possible output.
+        if includePossible and not hasOutput and self.getPossibleOutputs() is not None:
+            for possibleOutput in self.getPossibleOutputs():
+                if isinstance(possibleOutput, str):
+                    yield possibleOutput, self._possibleOutputs[possibleOutput]
+                else:
+                    yield possibleOutput.name, possibleOutput.value
+
+    def getPossibleOutputs(self):
+        return self._possibleOutputs
+
     def _iterOutputsNew(self):
         """ This methods iterates through a list where outputs have been
         annotated"""
 
         # Loop through the output list
         for attrName in self._outputs:
 
@@ -841,17 +916,21 @@
         from the Protocol Class definition, taking into account
         the variable type and default values.
         """
         if hasattr(self, '_definition'):
             for paramName, param in self._definition.iterParams():
                 # Create the var with value coming from kwargs or from
                 # the default param definition
-                var = param.paramClass(value=kwargs.get(paramName,
-                                                        param.default.get()))
-                setattr(self, paramName, var)
+                try:
+                    value = kwargs.get(paramName, param.default.get())
+                    var = param.paramClass(value=value)
+                    setattr(self, paramName, var)
+                except Exception as e:
+                    raise ValueError("Can't create parameter '%s' and set it to %s" %
+                                     (paramName, value)) from e
         else:
             print("FIXME: Protocol '%s' has not DEFINITION"
                   % self.getClassName())
 
     def _getFileName(self, key, **kwargs):
         """ This function will retrieve filenames given a key and some
         keywords arguments. The __filenamesDict attribute should be
@@ -866,20 +945,21 @@
         self.__filenamesDict.update(fnDict)
 
     def _store(self, *objs):
         """ Stores objects of the protocol using the mapper.
         If not objects are passed, the whole protocol is stored.
         """
         if self.mapper is not None:
-            if len(objs) == 0:
-                self.mapper.store(self)
-            else:
-                for obj in objs:
-                    self.mapper.store(obj)
-            self.mapper.commit()
+            with self._lock:
+                if len(objs) == 0:
+                    self.mapper.store(self)
+                else:
+                    for obj in objs:
+                        self.mapper.store(obj)
+                self.mapper.commit()
 
     def _insertChild(self, key, child):
         """ Insert a new child not stored previously.
         If stored previously, _store should be used.
         The child will be set as self.key attribute
         """
         try:
@@ -904,42 +984,80 @@
         Params:
             form: this is the form to be populated with sections and params.
         """
         pass
 
     def __insertStep(self, step, **kwargs):
         """ Insert a new step in the list.
-        Params:
-         **kwargs:
-            prerequisites: a list with the steps index that need to be done
-                           previous than the current one."""
+
+        :param prerequisites: a single integer or a list with the steps index that need to be done
+                           previous to the current one."""
         prerequisites = kwargs.get('prerequisites', None)
 
         if prerequisites is None:
             if len(self._steps):
                 # By default add the previous step as prerequisite
                 step.addPrerequisites(len(self._steps))
         else:
+            # Allow passing just an id
+            if not isinstance(prerequisites, list):
+                prerequisites = [prerequisites]
+
             step.addPrerequisites(*prerequisites)
 
         self._steps.append(step)
+        self._newSteps = True
         # Setup and return step index
         step.setIndex(len(self._steps))
 
         return step.getIndex()
 
-    def _setStatusSteps(self, status):
-        """Set the status of all steps"""
+    def setRunning(self):
+        """ Do not reset the init time in RESUME_MODE"""
+        previousStart = self.initTime.get()
+        super().setRunning()
+        if self.getRunMode() == MODE_RESUME and previousStart is not None:
+            self.initTime.set(previousStart)
+        else:
+            self._cpuTime.set(0)
+
+    def setAborted(self):
+        """ Abort the protocol, finalize the steps and close all open sets"""
+        try:
+            super().setAborted()
+            self._updateSteps(lambda step: step.setAborted(), where="status='%s'" % STATUS_RUNNING)
+            self._closeOutputSet()
+        except Exception as e:
+            print("An error occurred aborting the protocol (%s)" % e)
+
+    def setFailed(self, msg):
+        """ Set the run failed and close all open  sets. """
+        super().setFailed(msg)
+        self._closeOutputSet()
+
+    def _finalizeStep(self, status, msg=None):
+        """ Closes the step and setting up the protocol process id """
+        super()._finalizeStep(status, msg)
+        self._pid.set(None)
+
+    def _updateSteps(self, updater, where="1"):
+        """Set the status of all steps
+        :parameter updater callback/lambda receiving a step and editing it inside
+        :parameter where condition to filter the set with."""
         stepsSet = StepSet(filename=self.getStepsFile())
-        for step in stepsSet:
-            step.setStatus(status)
+        for step in stepsSet.iterItems(where=where):
+            updater(step)
             stepsSet.update(step)
         stepsSet.write()
         stepsSet.close()  # Close the connection
 
+    def getPath(self, *paths):
+        """ Same as _getPath but without underscore. """
+        return self._getPath(*paths)
+
     def _getPath(self, *paths):
         """ Return a path inside the workingDir. """
         return os.path.join(self.workingDir.get(), *paths)
 
     def _getExtraPath(self, *paths):
         """ Return a path inside the extra folder. """
         return self._getPath("extra", *paths)
@@ -965,32 +1083,33 @@
 
     def _getBasePath(self, path):
         """ Take the basename of the path and get the path
         relative to working dir of the protocol.
         """
         return self._getPath(os.path.basename(path))
 
-    def _insertFunctionStep(self, funcName, *funcArgs, **kwargs):
+    def _insertFunctionStep(self, func, *funcArgs, **kwargs):
         """
          Params:
-           funcName: the string name of the function to be run in the Step.
+           func: the function itself or, optionally, the name (string) of the function to be run in the Step.
            *funcArgs: the variable list of arguments to pass to the function.
            **kwargs: see __insertStep
         """
-        # Get the function give its name
-        func = getattr(self, funcName, None)
+        if isinstance(func, str):
+            # Get the function give its name
+            func = getattr(self, func, None)
 
         # Ensure the protocol instance have it and is callable
         if not func:
             raise Exception("Protocol._insertFunctionStep: '%s' function is "
-                            "not member of the protocol" % funcName)
+                            "not member of the protocol" % func)
         if not callable(func):
             raise Exception("Protocol._insertFunctionStep: '%s' is not callable"
-                            % funcName)
-        step = FunctionStep(func, funcName, *funcArgs, **kwargs)
+                            % func)
+        step = FunctionStep(func, func.__name__, *funcArgs, **kwargs)
 
         return self.__insertStep(step, **kwargs)
 
     def _insertRunJobStep(self, progName, progArguments, resultFiles=[],
                           **kwargs):
         """ Insert an Step that will simple call runJob function
         **args: see __insertStep
@@ -1130,15 +1249,20 @@
         self._stepsSet.write()
 
     def _stepStarted(self, step):
         """This function will be called whenever an step
         has started running.
         """
         self.info(pwutils.magentaStr("STARTED") + ": %s, step %d, time %s" %
-                  (step.funcName.get(), step._index, step.initTime.datetime()))
+                  (step.funcName.get(), step._index, step.initTime.datetime()),
+                  extra=getExtraLogInfo("PROTOCOL", STATUS.START,
+                                        project_name=self.getProject().getName(),
+                                        prot_id=self.getObjId(),
+                                        prot_name=self.getClassName(),
+                                        step_id=step._index))
         self.__updateStep(step)
 
     def _stepFinished(self, step):
         """This function will be called whenever an step
         has finished its run.
         """
         doContinue = True
@@ -1150,18 +1274,24 @@
                 "Protocol failed: " + step.getErrorMessage())
             self.setFailed(errorMsg)
             self.error(errorMsg)
         self.lastStatus = step.getStatus()
 
         self.__updateStep(step)
         self._stepsDone.increment()
-        self._store(self._stepsDone)
+        self._cpuTime.set(self._cpuTime.get() + step.getElapsedTime().total_seconds())
+        self._store(self._stepsDone,  self._cpuTime)
 
         self.info(pwutils.magentaStr(step.getStatus().upper()) + ": %s, step %d, time %s"
-                  % (step.funcName.get(), step._index, step.endTime.datetime()))
+                  % (step.funcName.get(), step._index, step.endTime.datetime()),
+                  extra=getExtraLogInfo("PROTOCOL",STATUS.STOP,
+                                        project_name=self.getProject().getName(),
+                                        prot_id=self.getObjId(),
+                                        prot_name=self.getClassName(),
+                                        step_id=step._index))
         if step.isFailed() and self.stepsExecutionMode == STEPS_PARALLEL:
             # In parallel mode the executor will exit to close
             # all working threads, so we need to close
             self._endRun()
         return doContinue
 
     def _stepsCheck(self):
@@ -1198,39 +1328,48 @@
         It will remove output attributes from mapper and object.
         """
         attributes = [a[0] for a in self.iterOutputAttributes()]
 
         for attrName in attributes:
             attr = getattr(self, attrName)
             self.mapper.delete(attr)
-            self.deleteAttribute(attrName)
+            delattr(self, attrName)
 
         self._outputs.clear()
         self.mapper.store(self._outputs)
 
     def findAttributeName(self, attr2Find):
         for attrName, attr in self.iterOutputAttributes():
             if attr.getObjId() == attr2Find.getObjId():
                 return attrName
         return None
 
     def deleteOutput(self, output):
         attrName = self.findAttributeName(output)
         self.mapper.delete(output)
-        self.deleteAttribute(attrName)
+        delattr(self,attrName)
         if attrName in self._outputs:
             self._outputs.remove(attrName)
         self.mapper.store(self._outputs)
         self.mapper.commit()
 
     def __copyRelations(self, other):
         """ This will copy relations from protocol other to self """
         pass
 
     def copy(self, other, copyId=True, excludeInputs=False):
+        """
+        Copies its attributes into the passed protocol
+
+        :param other: protocol instance to copt the attributes to
+        :param copyId: True (default) copies the identifier
+        :param excludeInputs: False (default). If true input attributes are excluded
+
+        """
+
         # Input attributes list
         inputAttributes = []
 
         # If need to exclude input attributes
         if excludeInputs:
             # Get all the input attributes, to be ignored at copy():
             for key, attr in self.iterInputAttributes():
@@ -1311,14 +1450,25 @@
 
         if os.path.islink(tmpFolder):
             pwutils.cleanPath(os.path.realpath(tmpFolder))
             os.remove(tmpFolder)
         else:
             pwutils.cleanPath(tmpFolder)
 
+        self._cleanExtraFiles()
+    def _cleanExtraFiles(self):
+        """ This method will be called when the protocol finishes correctly.
+        It is the responsibility of the protocols to implement this method to make extra cleanup
+        of its folders, like iterations folder and files that are not needed when finished
+        """
+
+        logger.info("Nothing to clean up")
+        logger.debug('FOR DEVELOPERS: implement Protocol._cleanExtraFiles this protocol could'
+                     ' free up some space upon finishing.')
+
     def _run(self):
         # Check that a proper Steps executor have been set
         if self._stepsExecutor is None:
             raise Exception('Protocol.run: Steps executor should be set before '
                             'running protocol')
         # Check the parameters are correct
         errors = self.validate()
@@ -1356,37 +1506,49 @@
 
         self._stepsExecutor.runJob(self._log, program, arguments, **kwargs)
 
     def run(self):
         """ Before calling this method, the working dir for the protocol
         to run should exists.
         """
-        self.__initLogs()
-
-        self.info(pwutils.greenStr('RUNNING PROTOCOL -----------------'))
-
-        # Store the full machine name where the protocol is running
-        # and also its PID
-        self.setPid(os.getpid())
-        self.setHostFullName(pwutils.getHostFullName())
-
-        self.info('Hostname: %s' % self.getHostFullName())
-        self.info('PID: %s' % self.getPid())
-        self.info('pyworkflow: %s' % pw.__version__)
-        self.info('plugin: %s' % self.getClassPackageName())
-        if hasattr(self.getClassPackage(), "__version__"):
-            self.info('plugin v: %s' % self.getClassPackage().__version__)
-        self.info('currentDir: %s' % os.getcwd())
-        self.info('workingDir: %s' % self.workingDir)
-        self.info('runMode: %s' % MODE_CHOICES[self.runMode.get()])
         try:
-            self.info('          MPI: %d' % self.numberOfMpi)
-            self.info('      threads: %d' % self.numberOfThreads)
+            self.info(pwutils.greenStr('RUNNING PROTOCOL -----------------'))
+            self.info("Protocol starts", extra=getExtraLogInfo("PROTOCOL", STATUS.START,
+                                                               project_name=self.getProject().getName(),
+                                                               prot_id=self.getObjId(),
+                                                               prot_name=self.getClassName()))
+            # Store the full machine name where the protocol is running
+            # and also its PID
+            self.setPid(os.getpid())
+            self.setHostFullName(pwutils.getHostFullName())
+
+            self.info('Hostname: %s' % self.getHostFullName())
+            self.info('PID: %s' % self.getPid())
+            self.info('pyworkflow: %s' % pw.__version__)
+            plugin = self.getPlugin()
+            self.info('plugin: %s' %  plugin.getName())
+            package = self.getClassPackage()
+            if hasattr(package, "__version__"):
+                self.info('plugin v: %s%s' %(package.__version__, ' (devel)' if plugin.inDevelMode() else '(production)'))
+            self.info('plugin binary v: %s' % plugin.getActiveVersion())
+            self.info('currentDir: %s' % os.getcwd())
+            self.info('workingDir: %s' % self.workingDir)
+            self.info('runMode: %s' % MODE_CHOICES[self.runMode.get()])
+            try:
+                self.info('          MPI: %d' % self.numberOfMpi)
+                self.info('      threads: %d' % self.numberOfThreads)
+            except Exception as e:
+                self.info('  * Cannot get information about MPI/threads (%s)' % e)
+        # Something went wrong ans at this point status is launched. We mark it as failed.
         except Exception as e:
-            self.info('  * Cannot get information about MPI/threads (%s)' % e)
+            print(e)
+            self.setFailed(str(e))
+            self._store(self.status, self.getError())
+            self._endRun()
+            return
 
         Step.run(self)
         if self.isFailed():
             self._store()
         self._endRun()
 
     def _endRun(self):
@@ -1400,71 +1562,41 @@
             self.warning('Not cleaning temp folder since '
                          '%s is set to True.' % pw.SCIPION_DEBUG_NOCLEAN)
         elif not self.isFailed():
             self.info('Cleaning temp folder....')
             self.cleanTmp()
 
         self.info(pwutils.greenStr('------------------- PROTOCOL ' +
-                                   self.getStatusMessage().upper()))
-        self.__closeLogs()
+                                   self.getStatusMessage().upper()),
+                  extra=getExtraLogInfo("PROTOCOL",STATUS.STOP,
+                                        project_name=self.getProject().getName(),
+                                        prot_id=self.getObjId(),
+                                        prot_name=self.getClassName()))
 
-    def __initLogs(self):
-        """ Open the log file overwriting its content if the protocol is going
-        to be execute from zero.
-        Otherwise append the new content to the old one.
-        Also open logs files and redirect the systems streams.
-        """
-        self._log = ScipionLogger(self.getLogPaths()[2])
-
-        if self.runMode.get() == MODE_RESTART:
-            mode = 'w+'
-        else:
-            mode = 'a'
-        # Backup the the system streams
-        self.__stdErr = sys.stderr
-        self.__stdOut = sys.stdout
-        self.__openLogsFiles(mode)
-        # Redirect the system streams to the protocol files
-        sys.stdout = self.__fOut
-        if pwutils.envVarOn('SCIPION_SEPARATE_STDERR'):
-            sys.stderr = self.__fErr
-        else:
-            sys.stderr = self.__fOut  # send stderr to wherever stdout appears
-            # TODO: maybe do not show separate "run.stdout" and "run.stderr"
-            # in the "Output Log" section if we put them together.
 
     def getLogPaths(self):
-        return list(map(self._getLogsPath,
-                        ['run.stdout', 'run.stderr', 'run.log', SCHEDULE_LOG]))
+        return [self.getStdoutLog(),self.getStderrLog() , self.getScheduleLog()]
+
+    def getStdoutLog(self):
+        return self._getLogsPath("run.stdout")
+
+    def getStderrLog(self):
+        return self._getLogsPath('run.stderr')
 
     def getScheduleLog(self):
-        return self._getLogsPath(SCHEDULE_LOG)
+        return self._getLogsPath('schedule.log')
 
     def getSteps(self):
         """ Return the steps.sqlite file under logs directory. """
         return self._steps
 
     def getStepsFile(self):
         """ Return the steps.sqlite file under logs directory. """
         return self._getLogsPath('steps.sqlite')
 
-    def __openLogsFiles(self, mode):
-        self.__fOut = open(self.getLogPaths()[0], mode)
-        self.__fErr = open(self.getLogPaths()[1], mode)
-
-    def __closeLogsFiles(self):
-        self.__fOut.close()
-        self.__fErr.close()
-
-    def __closeLogs(self):
-        self._log.close()
-        # Restore system streams
-        sys.stderr = self.__stdErr
-        sys.stdout = self.__stdOut
-        self.__closeLogsFiles()
 
     def _addChunk(self, txt, fmt=None):
         """
         Add text txt to self._buffer, with format fmt.
         fmt can be a color (like 'red') or a link that looks like 'link:url'.
         """
         # Make the text html-safe first.
@@ -1495,50 +1627,55 @@
                 self._buffer = ''
                 pwutils.renderTextFile(fname, self._addChunk)
                 outputs.append(self._buffer)
             else:
                 outputs.append('File "%s" does not exist' % fname)
         return outputs
 
-    def getLogsLastLines(self, lastLines=None):
+    def getLogsLastLines(self, lastLines=None, logFile=0):
         """
-        Get the log last(lastLines) lines
+        Get the last(lastLines) lines of a log file.
+
+        :param lastLines, if None, will try 'PROT_LOGS_LAST_LINES' env variable, otherwise 20
+        :param logFile: Log file to take the lines from, default = 0 (std.out). 1 for stdErr.
         """
         if not lastLines:
             lastLines = int(os.environ.get('PROT_LOGS_LAST_LINES', 20))
 
-        if not all(os.path.exists(p) for p in self.getLogPaths()):
+        # Get stdout
+        stdoutFn =self.getLogPaths()[logFile]
+
+        if not os.path.exists(stdoutFn):
             return []
 
-        self.__openLogsFiles('r')
-        iterlen = lambda it: sum(1 for _ in it)
-        numLines = iterlen(self.__fOut)
-
-        lastLines = min(lastLines, numLines)
-        sk = numLines - lastLines
-        sk = max(sk, 0)
-
-        self.__fOut.seek(0, 0)
-        output = [l.strip('\n') for k, l in enumerate(self.__fOut)
-                  if k >= sk]
-        self.__closeLogsFiles()
-        return output
+        with  open(stdoutFn, 'r') as stdout:
+
+            iterlen = lambda it: sum(1 for _ in it)
+            numLines = iterlen(stdout)
+
+            lastLines = min(lastLines, numLines)
+            sk = numLines - lastLines
+            sk = max(sk, 0)
+
+            stdout.seek(0, 0)
+            output = [l.strip('\n') for k, l in enumerate(stdout)
+                      if k >= sk]
+            return output
 
     def warning(self, message, redirectStandard=True):
-        self._log.warning(message, redirectStandard)
+        self._log.warning(message)
 
-    def info(self, message, redirectStandard=True):
-        self._log.info(message, redirectStandard)
+    def info(self, message, extra=None):
+        self._log.info(message, extra= extra)
 
     def error(self, message, redirectStandard=True):
-        self._log.error(message, redirectStandard)
+        self._log.error(message)
 
     def debug(self, message):
-        if pw.Config.debugOn():
-            self.info(message)
+        self._log.debug(message)
 
     def getWorkingDir(self):
         return self.workingDir.get()
 
     def setWorkingDir(self, path):
         self.workingDir.set(path)
 
@@ -1621,26 +1758,26 @@
     def getClassPackage(cls):
         """ Return the package module to which this protocol belongs.
         This function will only work, if for the given Domain, the
         method Domain.getProtocols() has been called once. After calling
         this method the protocol classes are registered with it Plugin
         and Domain info.
         """
-        # import pyworkflow.em as em
-        # em.Domain.getProtocols()  # make sure the _package is set for each Protocol class
-        # TODO: Check if we need to return scipion by default anymore
-        # Now the basic EM protocols are defined by scipion-em (pwem)
-        return getattr(cls, '_package', None)
+        return cls._package
 
     @classmethod
     def getClassPlugin(cls):
-        package = cls.getClassPackage()
-        return getattr(package, 'Plugin', None)
+
+        logger.warning("Deprecated on 04-2023. Use Protocol.getPlugin instead.")
+        return cls.getPlugin()
 
     @classmethod
+    def getPlugin(cls):
+        return cls._plugin
+    @classmethod
     def getClassPackageName(cls):
         return cls.getClassPackage().__name__ if cls.getClassPackage() else "orphan"
 
     @classmethod
     def getClassDomain(cls):
         """ Return the Domain class where this Protocol class is defined. """
         return pw.Config.getDomain()
@@ -1655,22 +1792,24 @@
         else:
             logoPath = None
 
         return logoPath
 
     @classmethod
     def validatePackageVersion(cls, varName, errors):
-        """ Function to validate the the package version specified in
+        """
+        Function to validate the package version specified in
         configuration file ~/.config/scipion/scipion.conf is among the available
         options and it is properly installed.
-        Params:
-            package: the package object (ej: eman2 or relion). Package should contain the
-                     following methods: getVersion(), getSupportedVersions()
-            varName: the expected environment var containing the path (and version)
-            errors: list to added error if found
+
+        :param package: the package object (ej: eman2 or relion). Package should contain the
+            following methods: getVersion(), getSupportedVersions()
+        :param varName: the expected environment var containing the path (and version)
+        :param errors: list of strings to add errors if found
+
         """
         package = cls.getClassPackage()
         packageName = cls.getClassPackageName()
         varValue = package.Plugin.getVar(varName)
         versions = ','.join(package.Plugin.getSupportedVersions())
 
         errorMsg = None
@@ -1692,15 +1831,19 @@
             errors.append("After fixed, you NEED TO RESTART THE PROJECT WINDOW")
 
     @classmethod
     def getClassLabel(cls, prependPackageName=True):
         """ Return a more readable string representing the protocol class """
         label = cls.__dict__.get('_label', cls.__name__)
         if prependPackageName:
-            label = "%s - %s" % (cls.getClassPackageName(), label)
+            try:
+                label = "%s - %s" % (cls.getPlugin().getName(), label)
+            except Exception as e:
+                label = "%s -%s" % ("missing", label)
+                logger.error("Couldn't get the plugin name for %s" % label, exc_info=e)
         return label
 
     @classmethod
     def isDisabled(cls):
         """ Return True if this Protocol is disabled.
         Disabled protocols will not be offered in the available protocols."""
         return False
@@ -1761,21 +1904,27 @@
         return self._numberOfSteps.get(0)
 
     @property
     def stepsDone(self):
         """ Return the number of steps executed. """
         return self._stepsDone.get(0)
 
+    @property
+    def cpuTime(self):
+        """ Return the sum of all durations of the finished steps"""
+        return self._cpuTime.get()
+
     def updateSteps(self):
         """ After the steps list is modified, this methods will update steps
         information. It will save the steps list and also the number of steps.
         """
         self._storeSteps()
         self._numberOfSteps.set(len(self._steps))
         self._store(self._numberOfSteps)
+        self._newSteps = False
 
     def getStatusMessage(self):
         """ Return the status string and if running the steps done.
         """
         msg = self.getStatus()
         if self.isRunning() or self.isAborted() or self.isFailed():
             msg += " (done %d/%d)" % (self.stepsDone, self.numberOfSteps)
@@ -1816,15 +1965,15 @@
         """ This function can be overwritten by subclasses.
         Used from the public validate function.
         """
         return []
 
     @classmethod
     def getUrl(cls):
-        return cls.getClassPlugin().getUrl(cls)
+        return cls.getPlugin().getUrl(cls)
 
     @classmethod
     def isInstalled(cls):
         # We a consider a protocol installed if there are not errors
         # from the _validateInstallation function
         return not cls.validateInstallation()
 
@@ -1921,28 +2070,36 @@
         """ Should be implemented in subclasses. See summary. """
         return ["No summary information."]
 
     def summary(self):
         """ Return a summary message to provide some information to users. """
         try:
             baseSummary = self._summary() or ['No summary information.']
+
+            if isinstance(baseSummary, str):
+                baseSummary = [baseSummary]
+
+            if not isinstance(baseSummary, list):
+                raise Exception("Developers error: _summary() is not returning "
+                                "a list")
+
+            comments = self.getObjComment()
+            if comments:
+                baseSummary += ['', '*COMMENTS:* ', comments]
+
+            if self.getError().hasValue():
+                baseSummary += ['', '*ERROR:*', self.getError().get()]
+
+            if self.summaryWarnings:
+                baseSummary += ['', '*WARNINGS:*']
+                baseSummary += self.summaryWarnings
+
         except Exception as ex:
             baseSummary = [str(ex)]
 
-        comments = self.getObjComment()
-        if comments:
-            baseSummary += ['', '*COMMENTS:* ', comments]
-
-        if self.getError().hasValue():
-            baseSummary += ['', '*ERROR:*', self.getError().get()]
-
-        if self.summaryWarnings:
-            baseSummary += ['', '*WARNINGS:*']
-            baseSummary += self.summaryWarnings
-
         return baseSummary
 
     def getFileTag(self, fn):
         return "[[%s]]" % fn
 
     def getObjectTag(self, objName):
         if isinstance(objName, str):
@@ -1976,23 +2133,26 @@
             text = "Reference with key *%s* not found." % citeStr
         return text
 
     def _getCiteText(self, cite, useKeyLabel=False):
         try:
 
             journal = cite.get("journal", cite.get("booktitle", ""))
-            doi = cite.get("doi", "")
+            doi = cite.get("doi", "").strip()
+            url = cite.get("url", "").strip()
             # Get the first author surname
             if useKeyLabel:
                 label = cite['ID']
             else:
                 label = cite['author'].split(' and ')[0].split(',')[0].strip()
                 label += ' et al., %s, %s' % (journal, cite['year'])
-            if len(doi.strip()) > 0:
-                text = '[[%s][%s]] ' % (doi.strip(), label)
+            if len(doi) > 0:
+                text = '[[%s][%s]] ' % (doi, label)
+            elif len(url) > 0:
+                text = '[[%s][%s]] ' % (url, label)
             else:
                 text = label.strip()
             return text
 
         except Exception as ex:
             print("Error with citation: " + label)
             print(ex)
@@ -2035,30 +2195,30 @@
         refs = getattr(self.getClassPackage(), "_references", [])
         return self.__getCitationsDict(refs, bibTexOutput=bibTexOutput)
 
     def citations(self):
         """ Return a citation message to provide some information to users. """
         citations = list(self.getCitations().values())
         if citations:
-            citations.insert(0, '*References:* ')
+            citations.insert(0, '*Protocol references:* ')
 
         packageCitations = self.getPackageCitations().values()
         if packageCitations:
-            citations.append('*Package References:*')
+            citations.append('*Package references:*')
             citations += packageCitations
         if not citations:
             return ['No references provided']
         return citations
 
     @classmethod
     def getHelpText(cls):
         """Get help text to show in the protocol help button"""
         helpText = cls.getDoc()
-        # NOt used since getClassPlugin is always None
-        # plugin = self.getClassPlugin()
+        # NOt used since getPlugin is always None
+        # plugin = self.getPlugin()
         # if plugin:
         #     pluginMetadata = plugin.metadata
         #     helpText += "\n\nPlugin info:\n"
         #     for key, value in pluginMetadata.iteritems():
         #         helpText += "%s: \t%s\n" % (key, value)
         return helpText
 
@@ -2161,14 +2321,20 @@
 
     def legacyCheck(self):
         """ Hook defined to run some compatibility checks
         before display the protocol.
         """
         pass
 
+    def getSize(self):
+        """ Returns the size of the folder corresponding to this protocol"""
+        if not self._size:
+            self._size = getFileSize(self.getPath())
+
+        return self._size
 
 class LegacyProtocol(Protocol):
     """ Special subclass of Protocol to be used when a protocol class
     is not found. It means that have been removed or it is in another
     development branch. In such, we will use the LegacyProtocol to
     simply store the parameters and inputs/outputs."""
 
@@ -2181,25 +2347,31 @@
     def getClassDomain(cls):
         return pw.Config.getDomain()
 
 
 # ---------- Helper functions related to Protocols --------------------
 
 def runProtocolMain(projectPath, protDbPath, protId):
-    """ Main entry point when a protocol will be executed.
-    This function should be called when:
-    scipion runprotocol ...
-    Params:
-        projectPath: the absolute path to the project directory.
-        protDbPath: path to protocol db relative to projectPath
-        protId: id of the protocol object in db.
     """
+    Main entry point when a protocol will be executed.
+    This function should be called when::
+
+        scipion runprotocol ...
+
+    :param projectPath: the absolute path to the project directory.
+    :param protDbPath: path to protocol db relative to projectPath
+    :param protId: id of the protocol object in db.
+
+    """
+
     # Enter to the project directory and load protocol from db
     protocol = getProtocolFromDb(projectPath, protDbPath, protId, chdir=True)
 
+    setDefaultLoggingContext(protId, protocol.getProject().getShortName())
+
     hostConfig = protocol.getHostConfig()
 
     # Create the steps executor
     executor = None
     nThreads = max(protocol.numberOfThreads.get(), 1)
 
     if protocol.stepsExecutionMode == STEPS_PARALLEL:
@@ -2307,16 +2479,60 @@
 
     if protTS is None:
         return False
 
     dbTS = pwutils.getFileLastModificationDate(protocol.getDbPath())
 
     if not (protTS and dbTS):
-        print("Can't compare if protocol is up to date: "
+        logger.info("Can't compare if protocol is up to date: "
               "Protocol %s, protocol time stamp: %s, %s timeStamp: %s"
               % (protocol, protTS, protocol, dbTS))
     else:
-        return protTS > dbTS
+        return protTS >= dbTS
 
 
 class ProtImportBase(Protocol):
     """ Base Import protocol"""
+
+class ProtStreamingBase(Protocol):
+    """ Base protocol to implement streaming protocols.
+    stepsGeneratorStep should be implemented (see its description) and output
+    should be created at the end of the processing Steps created by the stepsGeneratorStep.
+    To avoid concurrency error, when creating the output, do it in a with self._lock: block.
+    Minimum number of threads is 3 and should run in parallel mode.
+    """
+
+    def __init__(self, **kwargs):
+
+        super().__init__()
+        self.stepsExecutionMode = STEPS_PARALLEL
+    def _insertAllSteps(self):
+        # Insert the step that generates the steps
+        self._insertFunctionStep(self.stepsGeneratorStep)
+
+    def _stepsCheck(self):
+
+        # Just store steps created in checkNewInputStep
+        if self._newSteps:
+            self.updateSteps()
+
+    def stepsGeneratorStep(self):
+        """
+        This step should be implemented by any streaming protocol.
+        It should check its input and when ready conditions are met
+        call the self._insertFunctionStep method.
+
+        :return: None
+        """
+        pass
+
+    def _validateThreads(self, messages:list):
+
+        if self.numberOfThreads.get() < 3:
+            messages.append("At least 3 threads are needed for running this protocol. 1 for the core process, "
+                            "1 for the 'step-generator step' and one more for the actual processing" )
+    def _validate(self):
+        """ If you want to implement a validate method do it but call _validateThreads or validate threads value."""
+        errors = []
+        self._validateThreads(errors)
+
+        return errors
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/resources/loading.gif` & `scipion-pyworkflow-3.1.0/pyworkflow/resources/loading.gif`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/resources/scipion_icon.svg` & `scipion-pyworkflow-3.1.0/pyworkflow/resources/scipion_icon.svg`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/background_section.png` & `scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/background_section.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/delete.png` & `scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/delete.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/doc_icon.png` & `scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/doc_icon.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/download_icon.png` & `scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/download_icon.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/menu.png` & `scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/menu.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/volumeOff.png` & `scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/volumeOff.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/resources/showj/volumeOn.png` & `scipion-pyworkflow-3.1.0/pyworkflow/resources/showj/volumeOn.png`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/template.py` & `scipion-pyworkflow-3.1.0/pyworkflow/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,15 +257,15 @@
         :return: a list of templates
         """
         # Check if other plugins have json.templates
         domain = Config.getDomain()
         # Check if there is any .json.template in the template folder
         # get the template folder (we only want it to be included once)
         for pluginName, pluginModule in domain.getPlugins().items():
-            tempListPlugin = pluginModule.Plugin.getTemplates()
+            tempListPlugin = pluginModule._pluginInstance.getTemplates()
             for t in tempListPlugin:
                 if tempId is not None:
                     if t.getObjId() == tempId:
                         self.addTemplate(t)
                         break
                 else:
                     self.addTemplate(t)
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/tests/tests.py` & `scipion-pyworkflow-3.1.0/pyworkflow/tests/tests.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,31 @@
+import logging
+logger = logging.getLogger(__name__)
+
 import sys
 import os
 import time
 from traceback import format_exception
 import unittest
 from os.path import join, relpath
 
 import pyworkflow as pw
 import pyworkflow.utils as pwutils
 from pyworkflow.project import Manager
 from pyworkflow.protocol import MODE_RESTART, getProtocolFromDb
+from pyworkflow.object import Set
 
 SMALL = 'small'
 PULL_REQUEST = 'pull'
 DAILY = 'daily'
 WEEKLY = 'weekly'
 
+# Type hint when creating protocols
+from typing import TypeVar
+T = TypeVar('T')
 
 # Procedure to check if a test class has an attribute called _labels and if so
 # then it checks if the class test matches any of the labels in input label parameter.
 def hasLabel(TestClass, labels):
     # Get _labels attributes in class if any.
     classLabels = getattr(TestClass, '_labels', None)
 
@@ -56,18 +63,18 @@
         """
         assert name in cls._datasetDict, "Dataset: %s dataset doesn't exist." % name
 
         ds = cls._datasetDict[name]
         folder = ds.folder
         url = '' if ds.url is None else ' -u ' + ds.url
 
-        if not pwutils.envVarOn('SCIPION_TEST_NOSYNC'):
+        if not pwutils.strToBoolean(pw.Config.SCIPION_TEST_NOSYNC):
             command = ("%s %s --download %s %s"
                        % (pw.PYTHON, pw.getSyncDataScript(), folder, url))
-            print(">>>> %s" % command)
+            logger.info(">>>> %s" % command)
             os.system(command)
 
         return cls._datasetDict[name]
 
 
 class BaseTest(unittest.TestCase):
     _labels = [WEEKLY]
@@ -82,19 +89,19 @@
     def getRelPath(cls, basedir, filename):
         """Return the path relative to SCIPION_HOME/tests"""
         return relpath(filename, basedir)
 
     @classmethod
     def launchProtocol(cls, prot, **kwargs):
         """ Launch a given protocol using cls.proj.
-        Accepted **kwargs:
-            wait: if True the function will return after the protocol runs.
-                If not specified, then if waitForOutput is passed, wait is
-                false.
-            waitForOutputs: a list of expected outputs, ignored if wait=True
+
+        :param wait: if True the function will return after the protocol runs.
+            If not specified, then if waitForOutput is passed, wait is false.
+        :param waitForOutputs: a list of expected outputs, ignored if wait=True
+
         """
         wait = kwargs.get('wait', None)
         waitForOutputs = kwargs.get('waitForOutput', [])
 
         if wait is None:
             wait = not waitForOutputs
 
@@ -104,49 +111,54 @@
                 while True:
                     time.sleep(10)
                     prot = cls.updateProtocol(prot)
                     if all(prot.hasAttribute(o) for o in waitForOutputs):
                         return prot
 
         if prot.isFailed():
-            print("\n>>> ERROR running protocol %s" % prot.getRunName())
-            print("    FAILED with error: %s\n" % prot.getErrorMessage())
-
-            BaseTest.printLastLogLines(prot)
 
-            raise Exception("ERROR launching protocol.")
+            cls.printLastLogLines(prot)
+            raise Exception("Protocol %s execution failed. See last log lines above for more details." % prot.getRunName())
 
         if not prot.isFinished() and not prot.useQueue():  # when queued is not finished yet
-            print("\n>>> ERROR running protocol %s" % prot.getRunName())
 
-            BaseTest.printLastLogLines(prot)
-
-            raise Exception("ERROR: Protocol not finished")
+            cls.printLastLogLines(prot)
+            raise Exception("Protocol %s didn't finish. See last log lines above for more details." % prot.getRunName())
 
         return prot
 
     @staticmethod
     def printLastLogLines(prot):
+        """ Prints the last log lines (50 or  'PROT_LOGS_LAST_LINES' env variable) from stdout and stderr log files
+
+        :param prot: Protocol to take the logs from
+
+        """
+        logs = {"STD OUT": 0, "STD ERR":1}
 
         lastLines = int(os.environ.get('PROT_LOGS_LAST_LINES', 50))
-        print(pwutils.cyanStr("\n*************** LAST %s LINES OF THE LOG *********************\n" % lastLines))
-        logLines = prot.getLogsLastLines(lastLines)
-        for i in range(0, len(logLines)):
-            print(logLines[i])
-        print(pwutils.cyanStr("\n*************** END OF THE LOG *********************\n"))
 
-        sys.stdout.flush()
+        # For each log file to print
+        for key in logs:
+
+            logger.info(pwutils.cyanStr("\n*************** last %s lines of %s *********************\n" % (lastLines, key)))
+            logLines = prot.getLogsLastLines(lastLines, logFile=logs[key])
+            for i in range(0, len(logLines)):
+                logger.info(logLines[i])
+            logger.info(pwutils.cyanStr("\n*************** end of %s *********************\n" % key))
+
+            sys.stdout.flush()
 
     @classmethod
     def saveProtocol(cls, prot):
-        """ Save protocol using cls.proj """
+        """ Saves a protocol using cls.proj """
         cls.proj.saveProtocol(prot)
 
     @classmethod
-    def _waitOutput(cls, prot, outputAttributeName):
+    def _waitOutput(cls, prot, outputAttributeName, sleepTime=20, timeOut=5000):
         """ Wait until the output is being generated by the protocol. """
 
         def _loadProt():
             # Load the last version of the protocol from its own database
             loadedProt = getProtocolFromDb(prot.getProject().path,
                                            prot.getDbPath(),
                                            prot.getObjId())
@@ -154,26 +166,29 @@
             loadedProt.getProject().closeMapper()
             loadedProt.closeMappers()
             return loadedProt
 
         counter = 1
         prot2 = _loadProt()
 
+        numberOfSleeps = timeOut/sleepTime
+
         while (not prot2.hasAttribute(outputAttributeName)) and prot2.isActive():
-            time.sleep(5)
+            time.sleep(sleepTime)
             prot2 = _loadProt()
-            if counter > 1000:
+            if counter > numberOfSleeps:
+                logger.warning("Timeout (%s) reached waiting for %s at %s" % (timeOut, outputAttributeName, prot))
                 break
             counter += 1
 
         # Update the protocol instance to get latest changes
         cls.proj._updateProtocol(prot)
 
     @classmethod
-    def newProtocol(cls, protocolClass, **kwargs):
+    def newProtocol(cls, protocolClass:T, **kwargs)->T:
         """ Create new protocols instances through the project
         and return a newly created protocol of the given class
         """
         # Try to continue from previous execution
         if pwutils.envVarOn('SCIPION_TEST_CONTINUE'):
             candidates = cls.proj.mapper.selectByClass(protocolClass.__name__)
             if candidates:
@@ -188,40 +203,50 @@
     @classmethod
     def compareSets(cls, test, set1, set2):
         """ Iterate the elements of both sets and check
         that all elements have equal attributes. """
         for item1, item2 in zip(set1, set2):
             areEqual = item1.equalAttributes(item2)
             if not areEqual:
-                print("item 1 and item2 are different: ")
+                logger.info("item 1 and item2 are different: ")
                 item1.printAll()
                 item2.printAll()
             test.assertTrue(areEqual)
 
+    def compareSetProperties(self, set1:Set, set2:Set, ignore = ["_size", "_mapperPath"]):
+        """ Compares 2 sets' properties"""
+
+        self.assertTrue(set1.equalAttributes(set2, ignore=ignore, verbose=True), "Set1 (%s) properties differs from set2 (%s)." % (set1, set2))
+        self.assertTrue(set2.equalAttributes(set1, ignore=ignore, verbose=True), 'Set2 (%s) has properties that set1 (%s) does not have.' % (set2, set1))
+
     def assertSetSize(self, setObject, size=None, msg=None, diffDelta=None):
         """ Check if a pyworkflow Set is not None nor is empty, or of a determined size or
         of a determined size with a percentage (base 1) of difference"""
         self.assertIsNotNone(setObject, msg)
         setObjSize = setObject.getSize()
 
         if size is None:
             # Test is not empty
             self.assertNotEqual(setObjSize, 0, msg)
         else:
             if diffDelta:
                 self.assertLessEqual(abs(setObjSize - size), round(diffDelta * size), msg)
             else:
-                self.assertEqual(setObjSize, size)
+                self.assertEqual(setObjSize, size, msg)
 
     def assertIsNotEmpty(self, setObject, msg=None):
         """ Check if the pyworkflow object is not None nor is empty"""
         self.assertIsNotNone(setObject, msg)
 
         self.assertIsNotNone(setObject.get(), msg)
 
+    @classmethod
+    def setupTestOutput(cls):
+        setupTestOutput(cls)
+
 
 def setupTestOutput(cls):
     """ Create the output folder for a give Test class. """
     cls.outputPath = join(pw.Config.SCIPION_TESTS_OUTPUT, cls.__name__)
     pwutils.cleanPath(cls.outputPath)
     pwutils.makePath(cls.outputPath)
 
@@ -229,15 +254,15 @@
 def setupTestProject(cls, writeLocalConfig=False):
     """ Create and setup a Project for a give Test class. """
     projName = cls.__name__
     hostsConfig = None
 
     if writeLocalConfig:
         hostsConfig = '/tmp/hosts.conf'
-        print("Writing local config: %s" % hostsConfig)
+        logger.info("Writing local config: %s" % hostsConfig)
         import pyworkflow.protocol as pwprot
         pwprot.HostConfig.writeBasic(hostsConfig)
 
     if os.environ.get('SCIPION_TEST_CONTINUE', None) == '1':
         proj = Manager().loadProject(projName)
     else:
         proj = Manager().createProject(projName, hostsConf=hostsConfig)
@@ -263,22 +288,22 @@
         self.startTimeAll = time.time()
 
     def openXmlReport(self, classname, filename):
         pass
 
     def doReport(self):
         secs = time.time() - self.startTimeAll
-        sys.stderr.write("\n%s run %d tests (%0.3f secs)\n" %
+        logger.info("\n%s run %d tests (%0.3f secs)\n" %
                          (pwutils.greenStr("[==========]"),
                           self.numberTests, secs))
         if self.testFailed:
-            sys.stderr.write("%s %d tests\n"
+            logger.info("%s %d tests\n"
                              % (pwutils.redStr("[  FAILED  ]"),
                                 self.testFailed))
-        sys.stdout.write("%s %d tests\n"
+        logger.info("%s %d tests\n"
                          % (pwutils.greenStr("[  PASSED  ]"),
                             self.numberTests - self.testFailed))
 
     def tic(self):
         self.startTime = time.time()
 
     def toc(self):
@@ -294,22 +319,22 @@
         name = parts[0]
         parts = parts[1].split('.')
         classname = parts[-1].replace(")", "")
         return "%s.%s" % (classname, name)
 
     def addSuccess(self, test):
         secs = self.toc()
-        sys.stderr.write("%s %s (%0.3f secs)\n" %
+        logger.info("%s %s (%0.3f secs)\n" %
                          (pwutils.greenStr('[ RUN   OK ]'),
                           self.getTestName(test), secs))
 
     def reportError(self, test, err):
-        sys.stderr.write("%s %s\n" % (pwutils.redStr('[   FAILED ]'),
+        logger.info("%s %s\n" % (pwutils.redStr('[   FAILED ]'),
                                       self.getTestName(test)))
-        sys.stderr.write("\n%s"
+        logger.info("\n%s"
                          % pwutils.redStr("".join(format_exception(*err))))
         self.testFailed += 1
 
     def addError(self, test, err):
         self.reportError(test, err)
 
     def addFailure(self, test, err):
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/utils/dataset.py` & `scipion-pyworkflow-3.1.0/pyworkflow/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/utils/echo.py` & `scipion-pyworkflow-3.1.0/pyworkflow/utils/echo.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/utils/graph.py` & `scipion-pyworkflow-3.1.0/pyworkflow/utils/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,25 @@
         """
         for child in self._childs:
             for c in child.iterChilds():
                 yield c
 
         yield self
 
+    def countChilds(self, visitedNode=None, count=0):
+        """ Iterate over all childs and subchilds.
+        Nodes can be visited once
+        """
+        for child in self._childs:
+            if child._name not in visitedNode:
+                visitedNode[child._name] = True
+            child.countChilds(visitedNode)
+        return len(visitedNode)
+
+
     def iterChildsBreadth(self):
         """ Iter child nodes in a breadth-first order
         """
         for child in self._childs:
             yield child
 
         for child in self._childs:
@@ -138,14 +149,18 @@
     def aliasNode(self, node, aliasName):
         """ Register an alias name for the node. """
         self._nodesDict[aliasName] = node
 
     def getNode(self, nodeName):
         return self._nodesDict.get(nodeName, None)
 
+    def getNodeNames(self):
+        """ Returns all the keys in the node dictionary"""
+        return self._nodesDict.keys()
+
     def getNodes(self):
         return self._nodes
 
     def getRootNodes(self):
         """ Return all nodes that have no parent. """
         return [n for n in self._nodes if n.isRoot()]
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/utils/mpi.py` & `scipion-pyworkflow-3.1.0/pyworkflow/utils/mpi.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/utils/path.py` & `scipion-pyworkflow-3.1.0/pyworkflow/utils/path.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,35 +29,45 @@
 
 import os
 import shutil
 import sys
 from glob import glob
 import datetime
 
-from pyworkflow import SCIPION_SCRATCH, DOCSITEURLS
+from pyworkflow import SCIPION_SCRATCH, DOCSITEURLS, ASCII_COLOR_2_TKINTER
 from pyworkflow.exceptions import PyworkflowException
 from pyworkflow.config import Config
 
 ROOT = "/"
 
 
 def findFileRecursive(filename, path):
+    """
+    Finds a file/folder in a single path recursively
+
+    :param filename: Name (myfile.txt) of the file to look for.
+    :param path: folder to start the search from.
+    :return: The absolute path to the 'filename' found or None if not found.
+    """
     for root, dirs, files in os.walk(path):
-        if filename in files:
+        if filename in files or filename in dirs:
             return os.path.join(root, filename)
     return None   
         
-        
-def findFile(filename, *paths, **kwargs):
-    """ Search if the file is present in some path in the *paths provided.
-    Return None if not found.
-    'recursive' can be passed in kwargs to iterate into subfolders.
+
+def findFile(filename, *paths, recursive=False):
     """
-    recursive = kwargs.get('recursive', False)
-    
+    Search if a file/folder is present in any of the paths provided.
+
+    :param filename: Name (myfile.txt) of the file to look for.
+    :param paths: N number of folders to look at.
+    :param recursive: If True it will iterate into the subfolders.
+    :return: None if nothing is found.
+    """
+
     if filename:
         for p in paths:
             fn = os.path.join(p, filename)
             if os.path.exists(fn):
                 return fn
             if recursive:
                 f = findFileRecursive(filename, p)
@@ -169,16 +179,18 @@
         if scratchPath is None:  # Case when SCIPION_SCRATCH doesn't exist. TMP folder is created
             os.makedirs(tmpPath)
         else:
             try:
                 project = protocol.getProject()
                 folderId = "_".join([project.getShortName(),project.getProtWorkingDir(protocol)])
                 tmpScratchFolder = os.path.join(scratchPath, folderId)
+                if os.path.exists(tmpScratchFolder):
+                    cleanPath(tmpScratchFolder)
                 os.makedirs(tmpScratchFolder)  # Create scratch folder
-                createAbsLink(tmpScratchFolder, tmpPath)
+                createAbsLink(tmpScratchFolder, tmpPath)  # Create a sym link
 
             except Exception as e:
                 raise PyworkflowException("Couldn't create the temporary folder %s at:\n %s\nPlease, review %s variable." %
                                 (folderId, scratchPath, SCIPION_SCRATCH), url=DOCSITEURLS.CONFIG_SECTION % "scratch-folder") from e
 
 
 def makeFilePath(*files):
@@ -296,38 +308,28 @@
     It uses the python os.path.commonprefix and 
     then the direname over it since the former is
     implemented in char-by-char base.
     """
     return os.path.dirname(os.path.commonprefix(*paths))
 
 
-# Console (and XMIPP) escaped colors, and the related tags that we create
-# with Text.tag_config(). This dict is used in OutputText:addLine()
-# See also http://www.termsys.demon.co.uk/vtansi.htm#colors
-colorName = {'30': 'gray',
-             '31': 'red',
-             '32': 'green',
-             '33': 'yellow',
-             '34': 'blue',
-             '35': 'magenta',
-             '36': 'cyan',
-             '37': 'white'}
-
 
 def renderTextFile(fname, add, offset=0, lineNo=0, numberLines=True,
-                   maxSize=400, headSize=40, tailSize=None, notifyLine=None):
+                   maxSize=400, headSize=40, tailSize=None, notifyLine=None, errors='strict'):
     """
     Call callback function add() on each fragment of text from file fname,
     delimited by lines and/or color codes.
-      add: callback function add(txt, tag='normal')
-      offset: byte offset - we start reading the file from there
-      lineNo: lines will be numbered from this value on
-      numberLines: whether to prepend the line numbers
+
+    :param add: callback function with signature (txt, tag='normal')
+    :param offset: byte offset - we start reading the file from there
+    :param lineNo: lines will be numbered from this value on
+    :param numberLines: whether to prepend the line numbers
+
     """
-    textfile = open(fname, encoding='utf-8')
+    textfile = open(fname, encoding='utf-8', errors=errors)
     size = (os.stat(fname).st_size - offset) / 1024  # in kB
 
     for line in iterBigFile(textfile, offset, size,
                             maxSize, headSize, tailSize):
         if line is not None:
             lineNo += 1
             if notifyLine is not None:
@@ -382,15 +384,15 @@
             break
         code = line[start+2:end]
 
         # See what attribute to use from now on, and update pos
         if code == '0':
             attribute = None
         else:
-            attribute = colorName.get(code[-2:], None)
+            attribute = ASCII_COLOR_2_TKINTER.get(code[-2:], None)
         pos = end + 1  # go to the character next to "m", the closing char
 
 
 def iterBigFile(textfile, offset=0, size=None,
                 maxSize=400, headSize=40, tailSize=None):
     """
     Yield lines from file textfile. If the size to read is bigger
@@ -440,20 +442,34 @@
         if not os.path.os.path.exists(uni_fn):
             return uni_fn
 
     return None
 
 
 def getFileSize(fn):
-    """ Shortcut to inspect the size of a file. """
-    return os.stat(fn).st_size
+    """ Shortcut to inspect the size of a file or a folder. """
+
+    if not os.path.exists(fn):
+        return  0
+
+    elif os.path.isdir(fn):
+        total_size = 0
+        for dirpath, dirnames, filenames in os.walk(fn):
+            for f in filenames:
+                fp = os.path.join(dirpath, f)
+                if not os.path.islink(fp):
+                    total_size += os.path.getsize(fp)
+        return total_size
+
+    else:
+        return os.path.getsize(fn)
 
 
 def getFileLastModificationDate(fn):
     """ Returns the last modification date of a file or None
     if it doesn't exist. """
-    if os.path.os.path.exists(fn):
+    if os.path.exists(fn):
         ts = os.path.getmtime(fn)
         return datetime.datetime.fromtimestamp(ts)
     else:
         print(fn + " does not exist!!. Can't check last modification date.")
         return None
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/utils/process.py` & `scipion-pyworkflow-3.1.0/pyworkflow/utils/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,42 +24,47 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 """
 This module handles process execution
 """
 
+import logging
+logger = logging.getLogger(__name__)
+
 import sys
 from subprocess import check_call
+import psutil
 
 from .utils import greenStr
 from pyworkflow import Config
 
 
 # The job should be launched from the working directory!
 def runJob(log, programname, params,           
            numberOfMpi=1, numberOfThreads=1, 
            hostConfig=None, env=None, cwd=None, gpuList=None):
 
     command = buildRunCommand(programname, params, numberOfMpi, hostConfig,
                               env, gpuList=gpuList)
     
     if log is None:
-        print("** Running command: %s" % greenStr(command))
-    else:
-        log.info(greenStr(command), True)
+        log = logger
+
+    log.info("** Running command: **")
+    log.info(greenStr(command))
 
     return runCommand(command, env, cwd)
         
 
 def runCommand(command, env=None, cwd=None):
     """ Execute command with given environment env and directory cwd """
 
     # First let us create core dumps if in debug mode
-    if Config.debugOn(env):
+    if Config.debugOn():
         import resource
         resource.setrlimit(resource.RLIMIT_CORE,
                            (resource.RLIM_INFINITY, resource.RLIM_INFINITY))
         # This is like "ulimit -u 99999999", so we can create core dumps
 
     # TODO: maybe have to set PBS_NODEFILE in case it is used by "command"
     # (useful for example with gnu parallel)
@@ -75,49 +80,53 @@
     # Convert our list of params to a string, with each element escaped
     # with "" in case there are spaces.
     if not isinstance(params, str):
         params = ' '.join('"%s"' % p for p in params)
 
     if gpuList:
         params = params % {'GPU': ' '.join(str(g) for g in gpuList)}
+        if "CUDA_VISIBLE_DEVICES" in programname:
+            sep = "," if len(gpuList) > 1 else ""
+            programname = programname % {'GPU': sep.join(str(g) for g in gpuList)}
+
+    prepend = '' if env is None else env.getPrepend()
 
     if numberOfMpi <= 1:
-        return '%s %s' % (programname, params)
+        return '%s %s %s' % (prepend, programname, params)
     else:
         assert hostConfig is not None, 'hostConfig needed to launch MPI processes.'
 
         if programname.startswith('xmipp') and not programname.startswith('xmipp_mpi'):
             programname = programname.replace('xmipp', 'xmipp_mpi')
             
         mpiFlags = '' if env is None else env.get('SCIPION_MPI_FLAGS', '') 
 
-        return hostConfig.mpiCommand.get() % {
+        mpiCmd = hostConfig.mpiCommand.get() % {
             'JOB_NODES': numberOfMpi,
             'COMMAND': "%s `which %s` %s" % (mpiFlags, programname, params),
         }
+        return '%s %s' % (prepend, mpiCmd)
 
 
 def killWithChilds(pid):
     """ Kill the process with given pid and all children processes.
-    Params:
-     pid: the process id to terminate
+
+    :param pid: the process id to terminate
     """
-    import psutil
     proc = psutil.Process(pid)
     for c in proc.children(recursive=True):
         if c.pid is not None:
-            print("Terminating child pid: %d" % c.pid)
+            logger.info("Terminating child pid: %d" % c.pid)
             c.kill()
-    print("Terminating process pid: %s" % pid)
+    logger.info("Terminating process pid: %s" % pid)
     if pid is None:
-        print("WARNING! Got None PID!!!")
+        logger.warning("Got None PID!!!")
     else:
         proc.kill()
 
 
 def isProcessAlive(pid):
-    import psutil
     try:
-        proc = psutil.Process(pid)
-        return proc.is_running()
-    except psutil.NoSuchProcess:
+        psutil.Process(pid)
+        return True
+    except Exception:
         return False
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/utils/profiler.py` & `scipion-pyworkflow-3.1.0/pyworkflow/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/utils/progressbar.py` & `scipion-pyworkflow-3.1.0/pyworkflow/utils/progressbar.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,35 +33,38 @@
 
 class ProgressBar(object):
     """ Text progress bar class for Python.
 
     A text progress bar is typically used to display the progress of a long
     running operation, providing a visual cue that processing is underway.
 
-    Example:
+    Example::
+
         N = 1000
         pb = ProgressBar(N, fmt=ProgressBar.FULL)
         pb.start()
-        for x in xrange(N):
+        for x in range(N):
             pb.update(x+1)
             sleep(0.1)
         pb.finish()
+
     """
     DEFAULT = 'Progress: %(bar)s %(percent)3d%%'
     FULL = '%(bar)s %(current)d/%(total)d (%(percent)3d%%) %(remaining)d to go'
     # scipion uses variable fonts so the bar size changes
     # since the space width is different from the = width
     NOBAR = '%(current)d/%(total)d (%(percent)3d%%) %(remaining)d to go'
     OBJID = '%(bar)s %(current)d/%(total)d (%(percent)3d%%) (objectId=%(objectId)d)'
     DOT = '.'
 
     def __init__(self, total, width=40, fmt=DEFAULT, symbol='=',
                  output=None, extraArgs=None):
         """
         Create a new ProgressBar object.
+
         :param total: The total amount that will be running the progress bar.
             The value in the update() method can no go greater than this value.
         :param width: progress bar width (without the percentage and number of
             iterations loop)
         :param fmt: predefined format string, so far DEFAULT, FULL, OBJID and
             DOT are defined.
         :param symbol: progress bar is made with this symbol
@@ -114,14 +117,15 @@
     def start(self):
         """ Print empty progress bar. """
         self.update(0)
 
     def update(self, value):
         """
         Update the current value and print the progress.
+
         :param value: New value, should be greater than the previous
             value and less or equal the total value
         :return:
         """
         if value < 0 or value <= self._current or value > self._total:
             raise Exception("Incorrect value provided. It should be greater "
                             "than previous value and between 0 and total. ")
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/utils/properties.py` & `scipion-pyworkflow-3.1.0/pyworkflow/utils/properties.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 """
 This module defines the text used in the application.
 """
-
+# NOTE: DO NOT REMOVE UNTIL plugin manager uses Config.SCIPION_MAIN_COLOR and is released
+from pyworkflow.constants import Color
 
 class Message:
     # Example Usage: 
     # MyMessage = Message()
     # print MyMessage.label
 
     # Header List
@@ -64,33 +65,28 @@
     LABEL_PROTTREE_NONE = 'None'
 
     # -- Toolbar --
     LABEL_NEW = 'New'
     LABEL_NEW_ACTION = 'New     '
     LABEL_EDIT = 'Edit'
     LABEL_RENAME = 'Rename '
-    LABEL_EDIT_ACTION = 'Edit     '
     LABEL_COPY = 'Copy'
-    LABEL_COPY_ACTION = 'Copy   '
+    LABEL_PASTE = 'Paste'
+    LABEL_DUPLICATE = 'Duplicate'
     LABEL_DELETE = 'Delete'
-    LABEL_DELETE_ACTION = 'Delete    '
     LABEL_STEPS = 'Steps'
     LABEL_BROWSE = 'Browse'
-    LABEL_BROWSE_ACTION = 'Browse '
     LABEL_DB = 'Db'
     LABEL_STOP = 'Stop'
-    LABEL_STOP_ACTION = 'Stop execution'
     LABEL_ANALYZE = 'Analyze Results'
     LABEL_TREE = 'Tree'
     LABEL_SMALLTREE = 'Small Tree'
-    LABEL_LIST = 'List'
     LABEL_REFRESH = 'Refresh'
     LABEL_DEFAULT = 'Default'
     LABEL_CONTINUE = 'Continue'
-    LABEL_CONTINUE_ACTION = 'Approve continue'
     LABEL_EXPORT = 'Export'
     LABEL_EXPORT_UPLOAD = 'Export & upload'
     LABEL_RESTART_WORKFLOW = 'Restart workflow'
     LABEL_CONTINUE_WORKFLOW = 'Continue workflow'
     LABEL_STOP_WORKFLOW = 'Stop from here'
     LABEL_RESET_WORKFLOW = 'Reset from here'
 
@@ -125,15 +121,15 @@
     LABEL_RUNNAME = 'Run name'
     LABEL_EXECUTION = 'Run mode'
     LABEL_RUNMODE = 'Mode'
     LABEL_PARALLEL = 'Parallel'
     LABEL_HOST = 'Host'
     LABEL_THREADS = 'Threads'
     LABEL_MPI = 'MPI'
-    LABEL_QUEUE = 'Use queue?'
+    LABEL_QUEUE = 'Use a queue engine?'
     LABEL_QUEUE_FOR_JOBS = 'Use queue for Jobs?'
 
     LABEL_WAIT_FOR = 'Wait for'
     
     LABEL_EXPERT = 'Expert Level'
     LABEL_EXPERT_NORMAL = 'Normal'
     LABEL_EXPERT_ADVANCE = 'Advanced'
@@ -154,29 +150,35 @@
        over the network (or the same computer).
 *Threads*: This refers to different execution threads 
        in the same process that can share memory. They run in
        the same computer.     
     """
 
     HELP_USEQUEUE = """
-    Click *Yes* if you want to submit a single job per protocol to a Queue system.
-    The queue commands to launch and stop jobs should be configured
-    for the current host in the _%s_ file.
+    Click Yes if you want to send this execution to a queue engine like Slurm, Torque, ...
+    The queue commands to launch and stop jobs should be configured at
+    _%s_ file.
+    
+    See %s for more information.
         """
     HELP_USEQUEUEPERJOB = """
     Click *Yes* if you want to submit the multiple jobs per protocol to a Queue system.
     The queue commands for launch and stop jobs should be configured
     for the current host in the _hosts.conf_ file.
     """
 
     HELP_WAIT_FOR = """
     Specify a comma separated list of protocol IDs if you want
-that this protocol starts after the input protocols in the list
-are finished. This function will allow you to "schedule" many
-runs that will be executed after each other.
+    to *schedule* this protocol and wait for those protocols to finish before
+    starting this one.
+    
+    This function will allow you to "schedule" many
+    runs that will be executed after each other.
+     
+    See %s for more information.
     """
     
     TITLE_NAME_RUN = ' Protocol Run: '
     TITLE_RUN = 'Run'
     TITLE_LABEL = 'Label'
     LABEL_OPT_COMMENT = 'Describe your run here...'
     TITLE_COMMENT = 'Comment'
@@ -268,51 +270,78 @@
     TITLE_LAUNCHED = 'Success'
     LABEL_LAUNCHED = 'The protocol was launched successfully.'
     LABEL_FOUND_ERROR = 'Errors found'
     TITLE_SAVED_FORM = 'Success'
     LABEL_SAVED_FORM = 'The protocol was saved successfully.'
     TITLE_DELETE_FORM = 'Confirm DELETE'
     TITLE_RESTART_FORM = 'Confirm RESTART'
+    TITLE_CONTINUE_FORM = 'Confirm CONTINUE'
     LABEL_DELETE_FORM = """
 You are going to *DELETE* the run(s): 
   - %s
 *ALL DATA* related will be permanently removed.
 
 Do you really want to continue?'
 """
-    LABEL_RESTART_FORM = """
+    MESSAGE_RESTART_FORM = """
 You are going to *RESTART* the run: 
   %s
 
-Do you really want to restart?'
+Do you really want to restart it?
 """
-    LABEL_RESTART_PROTOCOL = """
-    Do you want to *RESTART* ONLY the run: 
-      %s 
-    *ALL DATA* related with the rest of protocols that depends on this, 
-    will be permanently removed.  
+    MESSAGE_CONTINUE_FORM = """
+    You are going to *CONTINUE* the run: 
+      %s
+
+    Do you really want to continue it?
+    """
+
+    MESSAGE_RESTART_WORKFLOW_WITH_RESULTS = """
+    All previous results of the following protocols will be deleted:
+        %s
+
+        Do you really want to *RESTART* the workflow?'
+    """
+
+    MESSAGE_CONTINUE_WORKFLOW_WITH_RESULTS = """
+        All previous results of the following protocols will be affected: 
+        %s
+
+        Do you really want to *CONTINUE* the workflow?
+        """
+
+    MESSAGE_ASK_SINGLE_ALL = """
+        What do you want to do?
+
+        *Single* : Just this protocol.
+        *All*: All above listed protocols will be launched.
     """
+
+
     TITLE_STOP_FORM = 'Confirm STOP'
     LABEL_STOP_FORM = 'Do you really want to *STOP* this run?'
     
     NO_VIEWER_FOUND = 'There is no viewer for protocol:'
     
     TITLE_SAVE_OUTPUT = 'Save protocol output'
     LABEL_SAVE_OUTPUT = 'Do you wish to save protocol output?'
 
-    TITLE_RESTART_WORKFLOW_FORM = 'Confirm RESTART'
+    TITLE_RESTART_WORKFLOW_FORM = 'Confirm RESTART workflow'
+    TITLE_CONTINUE_WORKFLOW_FORM = 'Confirm CONTINUE workflow'
     TITLE_STOP_WORKFLOW_FORM = 'Confirm STOP'
     TITLE_RESET_WORKFLOW_FORM = 'Confirm RESET'
-    TITLE_RESTART_WORKFLOW = 'Do you really want to *RESTART* this Workflow? All previous results will be deleted'
+    MESSAGE_RESTART_WORKFLOW = 'Do you really want to *RESTART* this workflow?'
+    MESSAGE_CONTINUE_WORKFLOW = 'Do you really want to *CONTINUE* this workflow?'
     TITLE_STOP_WORKFLOW = 'Do you really want to *STOP* this Workflow?'
     TITLE_RESET_WORKFLOW = 'Do you really want to *RESET* this Workflow?'
     TITLE_LAUNCHED_WORKFLOW_FAILED_FORM = 'Error while launching the workflow'
     TITLE_STOPPED_WORKFLOW_FAILED = 'Error while stopping the workflow'
     TITLE_RESETED_WORKFLOW_FAILED = 'Error while resetting the workflow'
     TITLE_LAUNCHED_WORKFLOW_FAILED = 'The workflow can not be relaunched from this protocol.\n'
+    TITLE_ACTIVE_PROTOCOLS = 'The following protocols are active:'
     
     # SHOWJ_WEB
     SHOWJ_TITLE = 'Showj'
     
     LABEL_RESLICE = 'Reslice'
     RESLICE_Z_NEGATIVE = 'Z Negative (Front)'
     RESLICE_Y_NEGATIVE = 'Y Negative (Top)'
@@ -381,120 +410,132 @@
     INSTALLED = 'installed'
     PRECESSING = 'processing'
     FAILURE = 'failure'
     AVAILABLE_RELEASE = 'available_release'
     TO_UPDATE = 'to_update'
     SUCCESS = 'success'
     ERRORS = 'errors'
+    WAITING = 'waiting'
 
 
 class PluginInformation:
     PLUGIN_URL = 'pluginURL'
     PLUGIN_NAME = 'pluginName'
     PLUGIN_VERSION = 'pluginVersion'
     PLUGIN_RELEASE_DATE = 'pluginUploadedDate'
     PLUGIN_DESCRIPTION = 'pluginDescription'
     PLUGIN_AUTHORS = 'pluginAuthor'
 
 
 # To get font awesome icons into png use: http://fa2png.io/
 class Icon:
-    # Project Content Template
-    RUNS_TREE = 'fa-sitemap.gif'
-    RUNS_LIST = 'fa-bars.gif'
-    ACTION_NEW = 'fa-plus-circle.gif'
-    ACTION_EDIT = 'fa-pencil.gif'
-    ACTION_SELECT_TO = 'fa-arrow-up.gif'
-    ACTION_COPY = 'fa-files-o.gif'
-    ACTION_DELETE = 'fa-trash-o.gif'
-    ACTION_REFRESH = 'fa-refresh.gif'
-    ACTION_RENAME = 'rename.gif'
-    # TODO: change action_steps icon - fa-codefork?
-    ACTION_STEPS = 'fa-list-ul.gif'
-    ACTION_BROWSE = 'fa-folder-open.gif'
-    ACTION_DB = 'fa-database.gif'
+    # Protocols status
+    PROT_DISABLED = 'prot_disabled.png'
+    BETA = 'beta.png'
+    NEW = 'new.png'
+    PRODUCTION = 'production.png'
+    UPDATED = 'updated.png'
+    GROUP = 'class_obj.png'
+    DEBUG = 'debug.png'
+    DOWNLOAD = 'fa-download.png'
+    FILE_BW = 'fa-file-o.png'
+    FIND = 'binoculares.png'
+    SELECT_ALL = 'workflow.png'
+    ERROR = 'fa-times-circle_alert.png'
+    INFO = 'fa-info-circle_alert.png'
+    ALERT = 'fa-exclamation-triangle_alert.png'
+    JAVA_FILE = 'file_java.png'
+    PYTHON_FILE = 'file_python.png'
+    # Project window icons
+    RUNS_TREE = 'fa-sitemap.png'
+    ACTION_NEW = 'fa-plus-circle.png'
+    ACTION_EDIT = 'fa-pencil.png'
+    ACTION_SELECT_FROM = 'fa-arrow-down.png'
+    ACTION_SELECT_TO = 'fa-arrow-up.png'
+    ACTION_COPY = 'clipboard-regular.png'
+    ACTION_PASTE = 'paste-solid.png'
+    ACTION_DUPLICATE = 'fa-files-o.png'
+    ACTION_DELETE = 'fa-trash-o.png'
+    ACTION_REFRESH = 'fa-refresh.png'
+    ACTION_RENAME = 'rename.png'
+    ACTION_STEPS = 'fa-list-ul.png'
+    ACTION_BROWSE = 'fa-folder-open.png'
+    ACTION_DB = 'fa-database.png'
     ACTION_TREE = None
-    ACTION_LIST = 'fa-bars.gif'
-    ACTION_STOP = 'fa-stop.gif'
-    ACTION_CONTINUE = 'fa-play-circle-o.gif'
-    ACTION_STOP_WORKFLOW = 'fa-stop-workflow.gif'
-    ACTION_RESULTS = 'fa-eye.gif'
-    ACTION_CLOSE = 'fa-times.gif'
-    ACTION_SAVE = 'fa-save.gif'
-    ACTION_VISUALIZE = 'fa-eye.gif'
-    ACTION_WIZ = 'fa-magic.gif'
-    ACTION_HELP = 'fa-question-circle.gif'
-    ACTION_REFERENCES = 'fa-external-link.gif'
-    ACTION_EXPORT = 'fa-external-link.gif'
-    ACTION_EXPORT_UPLOAD = 'fa-upload.gif'
-
-    ACTION_SEARCH = 'fa-search.gif'
-    ACTION_EXECUTE = 'fa-cogs.gif'
-    ACTION_IN = 'fa-sign-in.gif'
-    ACTION_OUT = 'fa-sign-out.gif'
-    ACTION_FIND_NEXT = 'fa-next.gif'
-    ACTION_FIND_PREVIOUS = 'fa-previous.gif'
+    ACTION_STOP = 'fa-stop.png'
+    ACTION_CONTINUE = 'fa-play-circle-o.png'
+    ACTION_STOP_WORKFLOW = 'fa-stop-workflow.png'
+    ACTION_RESULTS = 'fa-eye.png'
+    ACTION_CLOSE = 'fa-times.png'
+    ACTION_SAVE = 'fa-save.png'
+    ACTION_VISUALIZE = 'fa-eye.png'
+    ACTION_WIZ = 'fa-magic.png'
+    ACTION_HELP = 'fa-question-circle.png'
+    ACTION_REFERENCES = 'fa-external-link.png'
+    ACTION_EXPORT = 'fa-external-link.png'
+    ACTION_EXPORT_UPLOAD = 'fa-upload.png'
+    ACTION_SEARCH = 'fa-search.png'
+    ACTION_EXECUTE = 'fa-cogs.png'
+    ACTION_IN = 'fa-sign-in.png'
+    ACTION_OUT = 'fa-sign-out.png'
+    ACTION_FIND_NEXT = 'fa-next.png'
+    ACTION_FIND_PREVIOUS = 'fa-previous.png'
+    ACTION_COLLAPSE = 'fa-minus-square.png'
+    ACTION_EXPAND ='fa-plus-square.png'
     # Host template
-    BUTTON_SELECT = 'fa-check.gif'
-    BUTTON_CLOSE = 'fa-times.gif'
-    BUTTON_CANCEL = 'fa-ban.gif'
+    BUTTON_SELECT = 'fa-check.png'
+    BUTTON_CLOSE = 'fa-times.png'
+    BUTTON_CANCEL = 'fa-ban.png'
     BUTTON_SAVE = ACTION_SAVE
-    BUTTON_PC = 'fa-laptop.gif'
-    
-    ARROW_UP = 'fa-arrow-up.gif'
-    ARROW_LEFT = 'fa-arrow-left.gif'
-    BRUSH = 'fa-paint-brush.gif'
-    TAGS = 'fa-tags.gif'
-    HOME = 'fa-home.gif'
-    LIGHTBULB = 'fa-lightbulb-o.gif'
-    PLUS_CIRCLE = 'fa-plus-circle.gif'
-    LINK = 'fa-iconmoon-link.gif'
-    ROOT = 'root.gif'
-    ROCKET = 'fa-rocket.gif'
-
-    SCIPION_ICON = 'scipion_icon.gif'
-    SCIPION_ICON_PROJ = SCIPION_ICON  # 'scipion_icon_proj.gif'
-    SCIPION_ICON_PROJS = SCIPION_ICON  # 'scipion_icon_projs.gif'
-    SCIPION_ICON_PROT = SCIPION_ICON  # 'scipion_icon_prot.gif'
+
+    ARROW_UP = 'fa-arrow-up.png'
+    TAGS = 'fa-tags.png'
+    HOME = 'fa-home.png'
+    LIGHTBULB = 'fa-lightbulb-o.png'
+    PLUS_CIRCLE = 'fa-plus-circle.png'
+    ROCKET = 'fa-rocket.png'
+    NO_IMAGE_128 = 'no-image128.png'
+    FOLDER = 'file_folder.png'
+    FOLDER_LINK = 'file_folder_link.png'
+    FILE = 'file_generic.png'
+    FILE_LINK = 'file_generic_link.png'
+    FOLDER_OPEN = 'fa-folder-open.png'
+    DB = 'file_sqlite.png'
+    TXT_FILE = 'file_text.png'
+    POWER_OFF = 'power-off-solid.png'
+    BROOM = 'broom-solid.png'
+    BACKWARD = 'backward-solid.png'
+    CODE_BRANCH = 'code-branch-solid.png'
+
+    SCIPION_ICON = 'scipion_icon.png'
+    SCIPION_ICON_PROJ = SCIPION_ICON  # 'scipion_icon_proj.png'
+    SCIPION_ICON_PROJS = SCIPION_ICON  # 'scipion_icon_projs.png'
+    SCIPION_ICON_PROT = SCIPION_ICON  # 'scipion_icon_prot.png'
 
     # PLUGIN MANAGER ICONS
-    CHECKED = 'fa-checked.gif'
-    UNCHECKED = 'fa-unchecked.gif'
-    INSTALL = 'fa-install.gif'
-    UNINSTALL = 'fa-uninstall.gif'
-    TO_INSTALL = 'fa-to_install.gif'
-    INSTALLED = 'fa-installed.gif'
-    PROCESSING = 'fa-processing.gif'
-    FAILURE = 'fa-failure.gif'
-    DELETE_OPERATION = 'fa-delete-operation.gif'
-    TO_UPDATE = 'fa-update.gif'
-    ACTION_UNDO = 'fa-undo.gif'
-
-    PLUGIN_AUTHORS = 'users.gif'
-    PLUGIN_DESCRIPTION = 'file_stack.gif'
-    PLUGIN_RELEASE_DATE = 'fa-upload.gif'
-    PLUGIN_VERSION = 'file_vol.gif'
-    PLUGIN_PACKAGE = 'file_folder.gif'
-
-
-class Color:
-    RED_COLOR = 'Firebrick'  # Red color for background label  = #B22222
-    LIGHT_RED_COLOR = '#F3CBCB'  # Very light red for row selection
-    LIGHT_BLUE_COLOR = '#EAEBFF'  # Very light blue for even rows
-    LIGHT_GREY_COLOR = '#EAEBEC'  # Light grey for background color in form, protocol, table header and west container
-    LIGHT_GREY_COLOR_2 = '#F2F2F2'  # Very light grey for odd rows, input background, etc
-    DARK_GREY_COLOR = '#6E6E6E'  # Very dark grey for project title, tubes, etc
-    
-    STATUS_SAVED = '#D9F1FA', 
-    STATUS_LAUNCHED = '#D9F1FA', 
-    STATUS_RUNNING = '#FCCE62', 
-    STATUS_FINISHED = '#D2F5CB', 
-    STATUS_FAILED = '#F5CCCB', 
-    STATUS_INTERACTIVE = '#F3F5CB',
-    STATUS_ABORTED = '#F5CCCB',
+    CHECKED = 'fa-checked.png'
+    UNCHECKED = 'fa-unchecked.png'
+    INSTALL = 'fa-install.png'
+    UNINSTALL = 'fa-uninstall.png'
+    TO_INSTALL = 'fa-to_install.png'
+    INSTALLED = 'fa-installed.png'
+    PROCESSING = 'fa-processing.png'
+    FAILURE = 'fa-failure.png'
+    DELETE_OPERATION = 'fa-delete-operation.png'
+    TO_UPDATE = 'fa-update.png'
+    WAITING = 'wait.gif'
+    ACTION_UNDO = 'fa-undo.png'
+
+    PLUGIN_AUTHORS = 'users.png'
+    PLUGIN_DESCRIPTION = 'file_stack.png'
+    PLUGIN_RELEASE_DATE = 'fa-upload.png'
+    PLUGIN_VERSION = 'file_vol.png'
+    PLUGIN_PACKAGE = 'file_folder.png'
+
+
 
 
 class colorText:
     """printing in colors, bold, etc,
        example: print colorText.BOLD + 'Hello World !' + color.END
     """
     PURPLE = '\033[95m'
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/utils/reflection.py` & `scipion-pyworkflow-3.1.0/pyworkflow/utils/reflection.py`

 * *Files 7% similar despite different names*

```diff
@@ -91,15 +91,16 @@
 
 def getSubclasses(BaseClass, inputDict):
     """ Iterate over inputDict and find all subclasses
     of BaseClass, that will be set in outputDict.
     """
     outputDict = {}
     for k, v in inputDict.items():
-        if isclass(v) and issubclass(v, BaseClass):
+        # Do not add the base class that is imported in all modules
+        if (not v==BaseClass) and isclass(v) and issubclass(v, BaseClass):
             outputDict[k] = v
     return outputDict
 
 
 def checkPlugin(module):
     if not getattr(module, '_plugin', None):
         print('WARNING: module "%s" using old package structure, '
@@ -115,7 +116,14 @@
 
 def isModuleAFolder(modulename):
     """ Returns True if a python module is a folder"""
     # So far e can test for the filename
     module = sys.modules[modulename]
 
     return module.__file__.endswith("__init__.py")
+
+
+def isModuleLoaded(modulename):
+    """
+    Return True if a python module is loaded, False otherwise
+    """
+    return modulename in sys.modules
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/utils/which.py` & `scipion-pyworkflow-3.1.0/pyworkflow/utils/which.py`

 * *Files 11% similar despite different names*

```diff
@@ -88,30 +88,31 @@
 
         
 # ---- module API
 
 def whichgen(command, path=None, verbose=0, exts=None):
     """Return a generator of full paths to the given command.
     
-    "command" is a the name of the executable to search for.
-    "path" is an optional alternate path list to search. The default it
+    :param command: is a the name of the executable to search for.
+    :param path: is an optional alternate path list to search. The default it
         to use the PATH environment variable.
-    "verbose", if true, will cause a 2-tuple to be returned for each
+    :param verbose: if true, will cause a 2-tuple to be returned for each
         match. The second element is a textual description of where the
         match was found.
-    "exts" optionally allows one to specify a list of extensions to use
+    :param exts: optionally allows one to specify a list of extensions to use
         instead of the standard list for this system. This can
         effectively be used as an optimization to, for example, avoid
         stat's of "foo.vbs" when searching for "foo" and you know it is
         not a VisualBasic script but ".vbs" is on PATHEXT. This option
         is only supported on Windows.
 
-    This method returns a generator which yields either full paths to
-    the given command or, if verbose, tuples of the form (<path to
-    command>, <where path found>).
+    :return: This method returns a generator which yields either full paths to
+        the given command or, if verbose, tuples of the form (<path to
+        command>, <where path found>).
+
     """
     matches = []
     if path is None:
         usingGivenPath = 0
         path = os.environ.get("PATH", "").split(os.pathsep)
         if sys.platform.startswith("win"):
             path.insert(0, os.curdir)  # implied by Windows shell
@@ -175,28 +176,29 @@
                 else:
                     yield match[0]
 
 
 def which(command, path=None, verbose=0, exts=None):
     """Return the full path to the first match of the given command on
     the path.
-    
-    "command" is a the name of the executable to search for.
-    "path" is an optional alternate path list to search. The default is
-        to use the PATH environment variable.
-    "verbose", if true, will cause a 2-tuple to be returned. The second
-        element is a textual description of where the match was found.
-    "exts" optionally allows one to specify a list of extensions to use
+
+    :param command: is a the name of the executable to search for.
+    :param path: is an optional alternate path list to search.
+        The default is to use the PATH environment variable.
+    :param verbose: if true, will cause a 2-tuple to be returned.
+        The second element is a textual description of where the match was found.
+    :param exts: optionally allows one to specify a list of extensions to use
         instead of the standard list for this system. This can
         effectively be used as an optimization to, for example, avoid
         stat's of "foo.vbs" when searching for "foo" and you know it is
         not a VisualBasic script but ".vbs" is on PATHEXT. This option
         is only supported on Windows.
 
-    If no match is found for the command, an empty String is returned.
+    :return If no match is found for the command, an empty string is returned.
+
     """
     try:
         match = next(whichgen(command, path, verbose, exts))
     except StopIteration:
         return ''
     return match
 
@@ -206,21 +208,22 @@
     return path != ''
 
 
 def whichall(command, path=None, verbose=0, exts=None):
     """Return a list of full paths to all matches of the given command
     on the path.  
 
-    "command" is a the name of the executable to search for.
-    "path" is an optional alternate path list to search. The default it
+    :param command: is a the name of the executable to search for.
+    :param path: is an optional alternate path list to search. The default it
         to use the PATH environment variable.
-    "verbose", if true, will cause a 2-tuple to be returned for each
+    :param verbose: if true, will cause a 2-tuple to be returned for each
         match. The second element is a textual description of where the
         match was found.
-    "exts" optionally allows one to specify a list of extensions to use
+    :param exts: optionally allows one to specify a list of extensions to use
         instead of the standard list for this system. This can
         effectively be used as an optimization to, for example, avoid
         stat's of "foo.vbs" when searching for "foo" and you know it is
         not a VisualBasic script but ".vbs" is on PATHEXT. This option
         is only supported on Windows.
+
     """
     return list(whichgen(command, path, verbose, exts))
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/viewer.py` & `scipion-pyworkflow-3.1.0/pyworkflow/viewer.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,14 +117,15 @@
     
     The _targets class property should contain a list of string
     with the class names that this viewer is able to visualize.
     For example: _targets = ['Image', 'SetOfImages']
     """
     _targets = []
     _environments = [DESKTOP_TKINTER]
+    _name = None
     
     def __init__(self, tmpPath='./Tmp', **args):
         self._tmpPath = tmpPath
         self._project = args.get('project')
         if self._project is None:
             raise Exception('Can not initialize a Viewer with None project.')
         self.protocol = args.get('protocol', None)
@@ -284,16 +285,18 @@
         for k, v in self._getVisualizeDict().items():
             if self.getAttributeValue(k, False):
                 v(k)
                 
     def _citations(self):
         return self.protocol._citations()
 
-    # TODO: This method should not be necessary, instead NumericListParam should
-    # return a list and not a String
+    def validateInstallation(self):
+        return
+
+    # TODO deprecate this method, it's duplicate of one from pwutils.utils
     def _getListFromRangeString(self, rangeStr):
         """ Create a list of integer from a string with range definitions
         Examples:
         "1,5-8,10" -> [1,5,6,7,8,10]
         "2,6,9-11" -> [2,6,9,10,11]
         "2 5, 6-8" -> [2,5,6,7,8]
         """
@@ -303,8 +306,7 @@
             if '-' in e:
                 limits = e.split('-')
                 values += range(int(limits[0]), int(limits[1])+1)
             else:
                 # If values are separated by comma also split
                 values += map(int, e.split())
         return values
-
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/webservices/config.py` & `scipion-pyworkflow-3.1.0/pyworkflow/webservices/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Variable related to the online services (workflow stats and repository) that Scipion reports to or communicate.
 # These variables may change between Scipion versions but do not depend on the user or system
 
 # Web that gathers protocol usage
-SCIPION_STATS_SERVER = 'http://scipion.i2pc.es'
+SCIPION_STATS_SERVER = 'https://scipion.i2pc.es'
 SCIPION_STATS_WORKFLOW_APP = SCIPION_STATS_SERVER + '/report_protocols/api/workflow/workflow/'
 
 # Web that handles workflows
-WORKFLOW_REPOSITORY_SERVER = 'http://workflows.scipion.i2pc.es/'
+WORKFLOW_REPOSITORY_SERVER = 'https://workflows.scipion.i2pc.es/'
 WORKFLOW_PROG_STEP1 = 'workflowProgStep1_add/'
 WORKFLOW_PROG_STEP2 = 'workflowProgStep2_add/'
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/webservices/notifier.py` & `scipion-pyworkflow-3.1.0/pyworkflow/webservices/notifier.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/webservices/repository.py` & `scipion-pyworkflow-3.1.0/pyworkflow/webservices/repository.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflow/wizard.py` & `scipion-pyworkflow-3.1.0/pyworkflow/wizard.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,38 +30,35 @@
 """
 
 DESKTOP_TKINTER = 'tkinter'
 WEB_DJANGO = 'django'
 
 
 class Wizard(object):
-    """ This is a special case of GUI to help the user
-    selecting important parameters.
-    The _targets will serve to define to which Definition and 
-    parameters the Wizard is defined, it will be a list of tuples such as:
-    _targets = [(DefImportMicrographs, ['voltage', sphericalAberration']),
-                (DefCTFMicrographs, ['lowRes', 'highRes'])]
-    The _environments will serve to define when this wizard can be used.
-    For example>
-    _environments = [DESKTOP_TKINTER, WEB_DJANGO]
+    """ This is a special case of GUI to help the user selecting important parameters.
+
+    The _targets attribute is used to define to which parameters the Wizard can deal with.
+    It will be a list of tuples such as::
+
+        _targets = [(DefImportMicrographs, ['voltage', sphericalAberration']), (DefCTFMicrographs, ['lowRes', 'highRes'])]
+
     """
+
     _targets = []
-    _environments = [DESKTOP_TKINTER]
-    
+    _environments = [DESKTOP_TKINTER] # This can be ignored
+
     def show(self, form, *params):
-        """ This will show up the wizard to select parameters.
-        Params:
-            form: the protocol form, given access to to all parameters.
-                Some times the same wizard will modify several elements
-                in the form.
-            *params: a list of params to modify, sometimes the wizard can 
-                be generic and can be used for different parameters in the
-                same form.
+        """
+        EMPTY METHOD. Needs to be implemented in your class. This will be called to show the wizard.
+
+        :param form: the protocol form, given access to to all parameters. Some times the same wizard will modify several elements in the form.
+        :param params: a list of params to modify. Sometimes the wizard can be generic and can be used for different parameters in the same form.
         """
         pass
     
     def getView(self):
-        """ This method should return the string value of the view in web
+        """
+        EMPTY METHOD. Deprecated.This method should return the string value of the view in web
         that will respond to this wizard. This method only should be implemented
         in those wizards that have WEB_DJANGO environment defined. 
         """
         return None
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflowtests/__init__.py` & `scipion-pyworkflow-3.1.0/pyworkflowtests/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,26 +25,27 @@
 """
 Mock Domain definition that will be used by basic tests.
 """
 
 from pyworkflow.protocol import Protocol
 from pyworkflow.wizard import Wizard
 from pyworkflow.viewer import Viewer
+from pyworkflow.utils import getSubclasses
 from pyworkflow.plugin import Domain as pwDomain, Plugin as pwPlugin
 
 from .objects import MockObject
 
 
 class TestDomain(pwDomain):
     _name = __name__
     _objectClass = MockObject
     _protocolClass = Protocol
     _viewerClass = Viewer
     _wizardClass = Wizard
-    _baseClasses = globals()
+    _baseClasses = getSubclasses(MockObject, globals())
 
 
 Domain = TestDomain
 
 
 class Plugin(pwPlugin):
     pass
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflowtests/bibtex.py` & `scipion-pyworkflow-3.1.0/pyworkflowtests/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflowtests/objects.py` & `scipion-pyworkflow-3.1.0/pyworkflowtests/objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,24 +23,27 @@
 # *
 # **************************************************************************
 """
 Definition of Mock objects to be used within the tests in the Mock Domain
 """
 
 import os
+import logging
+logger = logging.getLogger(__name__)
 
 import pyworkflow.object as pwobj
+from pyworkflow.utils import cleanPath
 
 NO_INDEX = 0
 
 
-class MockObject(pwobj.OrderedObject):
+class MockObject(pwobj.Object):
     """Base object for all Mock classes"""
     def __init__(self, **kwargs):
-        pwobj.OrderedObject.__init__(self, **kwargs)
+        super().__init__(**kwargs)
 
     def __str__(self):
         return self.getClassName()
 
     def getFiles(self):
         """ Get all filePaths """
         return None
@@ -479,14 +482,39 @@
             else:
                 if itemDataIterator is not None:
                     next(itemDataIterator)  # just skip disabled data row
 
     def getFiles(self):
         return pwobj.Set.getFiles(self)
 
+    @classmethod
+    def create(cls, outputPath,
+               prefix=None, suffix=None, ext=None,
+               **kwargs):
+        """ Create an empty set from the current Set class.
+         Params:
+            outputPath: where the output file will be written.
+            prefix: prefix of the created file, if None, it will be deduced
+                from the ClassName.
+            suffix: additional suffix that will be added to the prefix with a
+                "_" in between.
+            ext: extension of the output file, be default will use .sqlite
+        """
+        fn = prefix or cls.__name__.lower().replace('setof', '')
+
+        if suffix:
+            fn += '_%s' % suffix
+
+        fn += '.%s' % (ext or 'sqlite')
+
+        setPath = os.path.join(outputPath, fn)
+        cleanPath(setPath)
+
+        return cls(filename=setPath, **kwargs)
+
 
 class MockSetOfImages(MockSet):
     """ Represents a set of Images """
     ITEM_TYPE = MockImage
 
     def __init__(self, **kwargs):
         MockSet.__init__(self, **kwargs)
@@ -584,28 +612,28 @@
         return self.getFirstItem().getDim()
 
     def __str__(self):
         """ String representation of a set of images. """
         sampling = self.getSamplingRate()
 
         if not sampling:
-            print("FATAL ERROR: Object %s has no sampling rate!!!"
+            logger.info("FATAL ERROR: Object %s has no sampling rate!!!"
                   % self.getName())
             sampling = -999.0
 
         s = "%s (%d items, %s, %0.2f Å/px%s)" % \
             (self.getClassName(), self.getSize(),
              self._dimStr(), sampling, self._appendStreamState())
         return s
 
     def _dimStr(self):
         """ Return the string representing the dimensions. """
         return str(self._firstDim)
 
-    def iterItems(self, orderBy='id', direction='ASC', where='1', limit=None):
+    def iterItems(self, orderBy='id', direction='ASC', where=None, limit=None):
         """ Redefine iteration to set the acquisition to images. """
         for img in pwobj.Set.iterItems(self, orderBy=orderBy, direction=direction,
                                        where=where, limit=limit):
 
             # Sometimes the images items in the set could
             # have the acquisition info per data row and we
             # don't want to override with the set acquisition for this case
@@ -785,99 +813,7 @@
 
     def setMicName(self, micName):
         self._micName.set(micName)
 
     def getMicName(self):
         return self._micName.get()
 
-
-class SetOfCoordinates(MockSet):
-    """ Encapsulate the logic of a set of particles coordinates.
-    Each coordinate has a (x,y) position and is related to a Micrograph
-    The SetOfCoordinates can also have information about TiltPairs.
-    """
-    ITEM_TYPE = MockCoordinate
-
-    def __init__(self, **kwargs):
-        MockSet.__init__(self, **kwargs)
-        self._micrographsPointer = pwobj.Pointer()
-        self._boxSize = pwobj.Integer()
-
-    def getBoxSize(self):
-        """ Return the box size of the particles.
-        """
-        return self._boxSize.get()
-
-    def setBoxSize(self, boxSize):
-        """ Set the box size of the particles. """
-        self._boxSize.set(boxSize)
-
-    def iterMicrographs(self):
-        """ Iterate over the micrographs set associated with this
-        set of coordinates.
-        """
-        return self.getMicrographs()
-
-    def iterMicrographCoordinates(self, micrograph):
-        """ Iterates over the set of coordinates belonging to that micrograph.
-        """
-        pass
-
-    def iterCoordinates(self, micrograph=None):
-        """ Iterate over the coordinates associated with a micrograph.
-        If micrograph=None, the iteration is performed over the whole
-        set of coordinates.
-        """
-        if micrograph is None:
-            micId = None
-        elif isinstance(micrograph, int):
-            micId = micrograph
-        elif isinstance(micrograph, MockMicrograph):
-            micId = micrograph.getObjId()
-        else:
-            raise Exception('Invalid input micrograph of type %s'
-                            % type(micrograph))
-
-        # Iterate over all coordinates if micId is None,
-        # otherwise use micId to filter the where selection
-        coordWhere = '1' if micId is None else '_micId=%d' % micId
-
-        for coord in self.iterItems(where=coordWhere):
-            yield coord
-
-    def getMicrographs(self):
-        """ Returns the SetOfMicrographs associated with
-        this SetOfCoordinates"""
-        return self._micrographsPointer.get()
-
-    def setMicrographs(self, micrographs):
-        """ Set the micrographs associated with this set of coordinates.
-        Params:
-            micrographs: Either a SetOfMicrographs object or a pointer to it.
-        """
-        if micrographs.isPointer():
-            self._micrographsPointer.copy(micrographs)
-        else:
-            self._micrographsPointer.set(micrographs)
-        
-    def getFiles(self):
-        filePaths = set()
-        filePaths.add(self.getFileName())
-        return filePaths
-
-    def __str__(self):
-        """ String representation of a set of coordinates. """
-        if self._boxSize.hasValue():
-            boxSize = self._boxSize.get()
-            boxStr = ' %d x %d' % (boxSize, boxSize)
-        else:
-            boxStr = 'No-Box'
-        s = "%s (%d items, %s%s)" % (self.getClassName(), self.getSize(),
-                                     boxStr, self._appendStreamState())
-
-        return s
-
-    def copyInfo(self, other):
-        """ Copy basic information (boxsize)
-                from other set of coordinates to current one"""
-        self.copyAttributes(other, '_boxSize')
-
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflowtests/protocols.py` & `scipion-pyworkflow-3.1.0/pyworkflowtests/protocols.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,54 +22,88 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 """
 Definition of Mock protocols to be used within the tests in the Mock Domain
 """
 
+import time
+import datetime
 import pyworkflow.utils as pwutils
 import pyworkflow.object as pwobj
 import pyworkflow.protocol as pwprot
-
+from pyworkflowtests.objects import MockSetOfImages, MockImage
 
 class SleepingProtocol(pwprot.Protocol):
     def __init__(self, **args):
         pwprot.Protocol.__init__(self, **args)
         self.name = pwobj.String(args.get('name', None))
         self.numberOfSleeps = pwobj.Integer(args.get('n', 1))
         self.runMode = pwobj.Integer(pwprot.MODE_RESUME)
 
-    def sleepStep(self, t, s):
+    def sleepStep(self, t):
         log = self._getPath("step_%02d.txt" % t)
-        import time
-        import datetime
         f = open(log, 'w+')
         f.write("Going to sleep at %s\n"
                 % pwutils.dateStr(datetime.datetime.now(), True))
         time.sleep(t)
         f.write("  Slept: %d seconds\n" % t)
         f.write("Awakened at %s\n"
                 % pwutils.dateStr(datetime.datetime.now(), True))
         f.close()
         return [log]
 
     def _insertAllSteps(self):
         print("Inserting all steps...")
         for i in range(self.numberOfSleeps.get()):
-            self._insertFunctionStep('sleepStep', i + 1, 'sleeping %d' % i)
+            self._insertFunctionStep('sleepStep', i + 1)
 
 
 class ParallelSleepingProtocol(SleepingProtocol):
     def _insertAllSteps(self):
-        step1 = self._insertFunctionStep('sleepStep', 1, '1')
+        step1 = self._insertFunctionStep('sleepStep', 1)
         n = 2
         deps = [step1]
         for i in range(n):
             self._insertFunctionStep('sleepStep')
 
+class ConcurrencyProtocol(SleepingProtocol):
+    """ Protocol to test concurrency access to sets"""
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+        self.stepsExecutionMode = pwprot.STEPS_PARALLEL
+
+    def _defineParams(self, form):
+        form.addParallelSection(threads=2, mpi=0)
+
+    def _insertAllSteps(self):
+        n = 2
+        for i in range(n):
+            self._insertFunctionStep('sleepAndOutput', 1, prerequisites=[])
+
+    def sleepAndOutput(self, secs):
+        self.sleepStep(secs)
+
+        outputSet = self.getOutputSet("myOutput", MockSetOfImages)
+        newImage = MockImage()
+        with self._lock:
+            outputSet.append(newImage)
+            outputSet.write()
+        self._store()
+
+
+    def getOutputSet(self, attrName, setClass):
+        output = getattr(self, attrName, None)
+
+        if output is None:
+            output = setClass.create(self._getExtraPath())
+            self._defineOutputs(**{attrName: output})
+
+        return output
 
 class ProtOutputTest(pwprot.Protocol):
     """ Protocol to test scalar output and input linking"""
     _label = 'test output'
 
     def __init__(self, **args):
         pwprot.Protocol.__init__(self, **args)
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_canvas.py` & `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_canvas.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_domain.py` & `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_domain.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_mappers.py` & `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_mappers.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,17 +25,20 @@
 # **************************************************************************
 
 
 import pyworkflow as pw
 import pyworkflow.object as pwobj
 import pyworkflow.tests as pwtests
 import pyworkflow.mapper as pwmapper
+from pyworkflow.mapper.sqlite import ID
 from pyworkflowtests.objects import Complex, MockImage
 import pyworkflowtests
 
+IMAGES_STK = 'images.stk'
+
 
 class TestSqliteMapper(pwtests.BaseTest):
     @classmethod
     def setUpClass(cls):
         pwtests.setupTestOutput(cls)
 
     def test_SqliteMapper(self):
@@ -94,18 +97,14 @@
         mapper.insertRelation(relName, creator, b2, p)
 
         # Save changes to file
         mapper.commit()
         self.assertEqual(1, mapper.db.getVersion())
         mapper.close()
 
-        # TODO: Maybe some mapper test for backward compatibility can be
-        # include in scipion-em, where we already have defined datasets
-        # and reference old sqlite files
-
         # Test using SqliteDb class
         db = pwmapper.SqliteDb()
         db._createConnection(fn, timeout=1000)
         tables = ['Objects', 'Relations']
         self.assertEqual(tables, db.getTables())
         # Test getting the version, for the gold file it should be 0
         self.assertEqual(1, db.getVersion())
@@ -262,44 +261,59 @@
         self.assertEqual(0, mapper.count())
         self.assertEqual(0, mapper.maxId())
         n = 10
 
         indexes = list(range(1, n + 1))
         for i in indexes:
             img = MockImage()
-            img.setLocation(i, 'images.stk')
+            img.setLocation(i, IMAGES_STK)
             mapper.insert(img)
 
         self.assertEqual(n, mapper.count())
         self.assertEqual(n, mapper.maxId())
 
         # Store one more image with bigger id
         img = MockImage()
         bigId = 1000
-        img.setLocation(i + 1, 'images.stk')
+        img.setLocation(i + 1, IMAGES_STK)
         img.setObjId(bigId)
         mapper.insert(img)
         self.assertEqual(bigId, mapper.maxId())
 
         # Insert another image with None as id, it should take bigId + 1
-        img.setLocation(i + 2, 'images.stk')
+        img.setLocation(i + 2, IMAGES_STK)
         img.setObjId(None)
         mapper.insert(img)
         self.assertEqual(bigId + 1, mapper.maxId())
 
         mapper.setProperty('samplingRate', '3.0')
         mapper.setProperty('defocusU', 1000)
         mapper.setProperty('defocusV', 1000)
         mapper.setProperty('defocusU', 2000)  # Test update a property value
         mapper.deleteProperty('defocusV')  # Test delete a property
         mapper.commit()
         self.assertEqual(1, mapper.db.getVersion())
+
+        # Test where parsing
+        self.assertIsNone(mapper.db._whereToWhereStr(None), "A where = None does not return None")
+        self.assertEqual(mapper.db._whereToWhereStr("missing1=missing2"), "missing1=missing2", "a where with missing fields does not work")
+        self.assertEqual(mapper.db._whereToWhereStr("_samplingRate=value2"), "c03=value2", "simple = where does not work")
+        self.assertEqual(mapper.db._whereToWhereStr("_samplingRate=_samplingRate"), "c03=c03", "simple = where with 2 fields does not work")
+        self.assertEqual(mapper.db._whereToWhereStr("_samplingRate = _samplingRate"), "c03 = c03", "simple = spaced where with 2 fields does not work")
+        self.assertEqual(mapper.db._whereToWhereStr("_samplingRate < 3"), "c03 < 3", "a where with < does not work")
+        self.assertEqual(mapper.db._whereToWhereStr("_samplingRate >= 4"), "c03 >= 4", "a where with >= does not work")
+        self.assertEqual(mapper.db._whereToWhereStr("5 <= _samplingRate"), "5 <= c03", "a where with <= does not work")
+        self.assertEqual(mapper.db._whereToWhereStr("5 <= _samplingRate OR 3=_index"), "5 <= c03 OR 3=c01", "a where with OR does not work")
+
+        # Tests actual where used in queries
+        self.assertEqual(len(mapper.unique(ID, "_index = 1 OR _index = 2")), 2, "unique with OR in where does not work.")
+        self.assertEqual(len(mapper.unique(ID, ID + " >= 20 ")), 2, "unique >= in where does not work.")
         mapper.close()
 
-        # Test that values where stored properly
+        # Test that values were stored properly
         mapper2 = pwmapper.SqliteFlatMapper(dbName, pw.Config.getDomain().getMapperDict())
         indexes.extend([bigId, bigId + 1])
         for i, obj in enumerate(mapper2.selectAll(iterate=True)):
             self.assertEqual(obj.getIndex(), i + 1)
             self.assertEqual(obj.getObjId(), indexes[i])
 
         self.assertTrue(mapper2.hasProperty('samplingRate'))
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_object.py` & `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_object.py`

 * *Files 18% similar despite different names*

```diff
@@ -22,21 +22,29 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import os
 import datetime as dt
-from collections import OrderedDict
+from logging import DEBUG, lastResort
+from time import sleep
 
 import pyworkflow.object as pwobj
 import pyworkflow.tests as pwtests
+from pyworkflow.mapper.sqlite import ID, CREATION
 from ..objects import (Complex, MockSetOfImages, MockImage, MockObject,
                        MockAcquisition, MockMicrograph)
 
+IMAGES_STK = "images.stk"
+
+NUMERIC_ATRIBUTE_NAME = "1"
+
+NUMERIC_ATTRIBUTE_VALUE = "numeric_attribute"
+
 
 class ListContainer(pwobj.Object):
     def __init__(self, **args):
         pwobj.Object.__init__(self, **args)
         self.csv = pwobj.CsvList()
     
     
@@ -44,15 +52,15 @@
     @classmethod
     def setUpClass(cls):
         pwtests.setupTestOutput(cls)
 
     def test_ObjectsDict(self):
         # Validate that the object dict is populated correctly
         basicObjNames = [
-            'Object', 'Scalar', 'Integer', 'Float', 'String', 'Pointer',
+            'Scalar', 'Integer', 'Float', 'String', 'Pointer', 'Boolean',
             'OrderedObject', 'List', 'CsvList', 'PointerList', 'Set'
         ]
         self.assertTrue(all(name in pwobj.OBJECTS_DICT
                             for name in basicObjNames))
 
     def test_Object(self):
         value = 2
@@ -129,23 +137,36 @@
         self.assertFalse(s2.empty(),
                          "s2 string should not be empty after value")
 
         now = dt.datetime.now()
         s.set(now)
         self.assertEqual(now, s.datetime())
 
+        # Ranges and values
+        s2.set("1 2 3 4")
+        self.assertEqual(s2.getListFromValues(caster=float), [1.,2.,3.,4.])
+        self.assertEqual(s2.getListFromRange(), [1, 2, 3, 4])
+
+        # Values ...
+        s2.set("2x4, 4, 7")
+        self.assertEqual(s2.getListFromValues(), [4, 4, 4, 7])
+
+        # Ranges
+        s2.set("2-8, 1-2, 7")
+        self.assertEqual(s2.getListFromRange(), [2, 3, 4, 5, 6, 7, 8, 1, 2, 7])
+
     def test_Pointer(self):
         c = Complex.createComplex()
         p = pwobj.Pointer()
         p.set(c)
         p.setExtended('Name')
         c.Name = pwobj.String('Paquito')
 
         self.assertEqual(p.get(), 'Paquito')
-        stackFn = "images.stk"
+        stackFn = IMAGES_STK
         mrcsFn = "images.mrcs"
         fn = self.getOutputPath('test_images.sqlite')
         imgSet = MockSetOfImages(filename=fn)
         imgSet.setSamplingRate(1.0)
         for i in range(10):
             img = MockImage()
             img.setLocation(i+1, stackFn)
@@ -173,19 +194,21 @@
         self.assertEqual(img7.getFileName(), mrcsFn)
 
         o = MockObject()
 
         o.pointer = pwobj.Pointer()
         o.pointer.set(imgSet)
 
-        o.refC = o.pointer.get()
-        attrNames = [k for k, a in o.getAttributes()]
-        # Check that 'refC' should not appear in attributes
-        # since it is only an "alias" to an existing pointed value
-        self.assertNotIn('refC', attrNames)
+        # This is not true anymore ans is allowed unless we see is needed
+        # The main reason is a boost in performance.
+        # o.refC = o.pointer.get()
+        # attrNames = [k for k, a in o.getAttributes()]
+        # # Check that 'refC' should not appear in attributes
+        # # since it is only an "alias" to an existing pointed value
+        # self.assertNotIn('refC', attrNames)
 
         self.assertFalse(o.pointer.hasExtended(),
                          'o.pointer should not have extended at this point')
 
         o.pointer.setExtended(7)
 
         self.assertTrue(o.pointer.hasExtended())
@@ -203,15 +226,15 @@
         self.assertTrue(ptr.hasExtended())
         self.assertEqual(ptr.getExtended(), "7")
 
         # Check that the Item 7 of the set is properly
         # retrieved by the pointer after setting the extended to 7
         self.assertEqual(imgSet[7], ptr.get())
 
-        o2 = pwobj.OrderedObject()
+        o2 = pwobj.Object()
         o2.outputImages = imgSet
         ptr2 = pwobj.Pointer()
         ptr2.set(o2)
         # Test nested extended attributes
         ptr2.setExtended('outputImages.7')
         self.assertEqual(imgSet[7], ptr2.get())
 
@@ -221,37 +244,49 @@
 
         # Test copy between pointer objects
         ptr4 = pwobj.Pointer()
         ptr4.copy(ptr3)
         self.assertEqual(imgSet[7], ptr4.get())
         self.assertEqual(ptr4.getExtended(), 'outputImages.7')
 
+        # Test numeric attributes.
+        setattr(o2, NUMERIC_ATRIBUTE_NAME, NUMERIC_ATTRIBUTE_VALUE)
+        ptr5 = pwobj.Pointer(value=o2, extended=NUMERIC_ATRIBUTE_NAME)
+        self.assertEqual(NUMERIC_ATTRIBUTE_VALUE, ptr5.get())
+
     def test_Sets(self):
-        stackFn = "images.stk"
+        stackFn = IMAGES_STK
         fn = self.getOutputPath('test_images2.sqlite')
-        print("Writing to sqlite: %s" % fn)
 
         imgSet = MockSetOfImages(filename=fn)
-        imgSet.setSamplingRate(1.0)
+
+        halfTimeStamp = None
 
         for i in range(10):
             img = MockImage()
             img.setLocation(i + 1, stackFn)
+            img.setSamplingRate(i % 3)
             imgSet.append(img)
-
+            if i == 4:
+                sleep(1)
+                halfTimeStamp = dt.datetime.utcnow().replace(microsecond=0)
         imgSet.write()
 
         # Test size is 10
         self.assertSetSize(imgSet, 10)
 
+        # Test hasChangedSince
+        timeStamp = dt.datetime.now()
+        self.assertFalse(imgSet.hasChangedSince(timeStamp), "Set.hasChangedSince returns true when it hasn't changed.")
+        # Remove 10 seconds
+        self.assertTrue(imgSet.hasChangedSince(timeStamp-dt.timedelta(0,10)), "Set.hasChangedSince returns false when it has changed.")
+
         # PERFORMANCE functionality
         def checkSetIteration(limit, skipRows=None):
 
-            print("Checking set iteration with limit:%s and skipRows: %s"
-                  % (limit, skipRows))
             expectedId = 1 if skipRows is None else skipRows+1
             index = 0
             for item in imgSet.iterItems(limit=(limit, skipRows)):
                 self.assertEqual(item.getIndex(), expectedId+index,
                                  "Wrong item in set when using limits.")
                 index += 1
 
@@ -260,14 +295,65 @@
 
         # Check iteration with limit
         checkSetIteration(2)
 
         # Check iteration with limit and skip rows
         checkSetIteration(3, 2)
 
+        # Tests unique method
+        # Requesting 1 unique value as string
+        result = imgSet.getUniqueValues("_samplingRate")
+        self.assertEqual(len(result), 3, "Unique values wrong for 1 attribute and 3 value")
+
+        # Requesting 1 unique value as list
+        result = imgSet.getUniqueValues(["_samplingRate"])
+        self.assertEqual(len(result), 3, "Unique values wrong for 1 attribute and one value as list")
+        
+        # Requesting several unique values as string
+        result = imgSet.getUniqueValues("_index")
+        self.assertEqual(len(result), 10, "Unique values wrong for id attribute")
+
+        # Requesting several unique values with several columns
+        result = imgSet.getUniqueValues(["_filename", "_samplingRate"])
+        # Here we should have 2 keys containing 2 list
+        self.assertEqual(len(result), 2, "Unique values dictionary length wrong")
+        self.assertEqual(len(result["_filename"]), 3, "Unique values dict item size wrong")
+
+        # Requesting unique values with where
+        result = imgSet.getUniqueValues("_index",where="_samplingRate = 2")
+        # Here we should have 2 values
+        self.assertEqual(len(result), 3, "Unique values with filter not working")
+
+        # Request id list
+        result = imgSet.getUniqueValues(ID)
+        # Here we should have 10 values
+        self.assertEqual(len(result), 10, "Unique values with ID")
+
+        # Use creation timestamp
+        # Request id list
+        result = imgSet.getUniqueValues(ID, where="%s>=%s" % (CREATION , imgSet.fmtDate(halfTimeStamp)))
+        self.assertEqual(len(result), 5, "Unique values after a time stamp does not work")
+
+        # Test getIdSet
+        ids = imgSet.getIdSet()
+        self.assertIsInstance(ids, set, "getIdSet does not return a set")
+        self.assertIsInstance(next(iter(ids)), int, "getIdSet items are not integer")
+        self.assertEqual(len(ids), 10, "getIdSet does not return 10 items")
+
+        # Test load properties queries
+        from pyworkflow.mapper.sqlite_db import logger
+        logger.setLevel(DEBUG)
+        lastResort.setLevel(DEBUG)
+        imgSetVerbose = MockSetOfImages(filename=fn)
+        imgSetVerbose.loadAllProperties()
+
+        # Compare sets are "equal"
+        self.compareSetProperties(imgSet, imgSetVerbose, ignore=[])
+
+
     def test_copyAttributes(self):
         """ Check that after copyAttributes, the values
         were properly copied.
         """
         c1 = Complex(imag=10., real=11.)
         c2 = Complex(imag=0., real=1.0001)
         
@@ -320,20 +406,16 @@
                                dosePerFrame=1)
         m1 = MockMicrograph(
             'my_movie.mrc', objId=1, objLabel='test micrograph',
             objComment='Testing store and retrieve from dict.')
         m1.setSamplingRate(1.6)
         m1.setAcquisition(acq1)
         m1Dict = m1.getObjDict(includeBasic=True)
-        for k, v in m1Dict.items():
-            if isinstance(v, str):
-                v = "'%s'" % v
-            print("('%s', %s)," % (k, v))
 
-        goldDict1 = OrderedDict([
+        goldDict1 = dict([
             ('object.id', 1),
             ('object.label', 'test micrograph'),
             ('object.comment', 'Testing store and retrieve from dict.'),
             ('_index', 0),
             ('_filename', 'my_movie.mrc'),
             ('_samplingRate', 1.6),
             ('_micName', None),
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_project.py` & `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_project.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,17 +24,19 @@
 # **************************************************************************
 
 from pyworkflow.project.project import Project
 from unittest import TestCase
 from unittest.mock import patch
 
 
+# NOTE: This test as it is might serve as a skeleton for future testing the fixLinks
+# but as it is now it does not test anything at all. I leave it as an example of using patch (mock testing)
 class TestProject(TestCase):
 
     def test_fixlinks(self):
         """ Test fixlinks call."""
 
         with patch("pyworkflow.project.Project.getRuns") as getruns:
 
-            getruns.return_value = [1]
+            getruns.return_value = []
             proj = Project("domain", "path")
             proj.fixLinks("foo")
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_protocol_execution.py` & `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_protocol_execution.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import pyworkflow.tests as pwtests
 import pyworkflow.mapper as pwmapper
 import pyworkflow.protocol as pwprot
+from pyworkflow.project import Project
 
 
 # TODO: this test seems not to be finished.
 from pyworkflowtests.protocols import SleepingProtocol
 from pyworkflowtests import Domain
 
 
@@ -43,22 +44,26 @@
         """Test the list with several Complex"""
         fn = self.getOutputPath("protocol.sqlite")
         print("Writing to db: %s" % fn)
 
         # Discover objects and protocols
         mapperDict = Domain.getMapperDict()
 
+        # Associate the project
+        proj = Project(Domain, path=self.getOutputPath(''))
+
         # Check that the protocol has associated package
         mapper = pwmapper.SqliteMapper(fn, mapperDict)
-        prot = SleepingProtocol(mapper=mapper, n=2,
+        prot = SleepingProtocol(mapper=mapper, n=2, project= proj,
                                 workingDir=self.getOutputPath(''))
         domain = prot.getClassDomain()
         domain.printInfo()
 
         prot.setStepsExecutor(pwprot.StepExecutor(hostConfig=None))
+        prot.makeWorkingDir()
         prot.run()
         mapper.commit()
         mapper.close()
 
         self.assertEqual(prot._steps[0].getStatus(), pwprot.STATUS_FINISHED)
         
         mapper2 = pwmapper.SqliteMapper(fn, mapperDict)
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_protocol_export.py` & `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_protocol_export.py`

 * *Files identical despite different names*

### Comparing `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_protocol_output.py` & `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_protocol_output.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,20 +21,22 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+import os
 
 import pyworkflow as pw
 import pyworkflow.object as pwobj
 import pyworkflow.tests as pwtests
 import pyworkflow.mapper as pwmapper
 import pyworkflow.protocol as pwprot
+from pyworkflow.project import Project
 from pyworkflowtests.protocols import ProtOutputTest
 from pyworkflowtests import Domain, MockObject
 
 
 # Protocol to output of basic scipion objects
 class TestProtocolOutputs(pwtests.BaseTest):
     @classmethod
@@ -49,33 +51,40 @@
         """Test the list with several Complex"""
         fn = self.getOutputPath("protocol.sqlite")
 
         # Discover objects and protocols
         mapperDict = Domain.getMapperDict()
 
         mapper = pwmapper.SqliteMapper(fn, mapperDict)
-        prot = ProtOutputTest(mapper=mapper, n=2,
+        # Associate the project
+        proj = Project(Domain, path=self.getOutputPath(''))
+
+        prot = ProtOutputTest(mapper=mapper, n=2, project=proj,
                               workingDir=self.getOutputPath(''))
 
         # Add and old style o, not in the outputs dictionary
         prot.output1 = MockObject()
 
         self.assertFalse(prot._useOutputList.get(),
                          "useOutputList wrongly initialized")
 
         outputs = [o for o in prot.iterOutputAttributes()]
         self.assertTrue(1, len(outputs))
 
         prot._stepsExecutor = pwprot.StepExecutor(hostConfig=None)
+
+        #Create the logs folder
+        prot.makeWorkingDir()
+
         prot.run()
 
         self.assertEqual(prot._steps[0].getStatus(),
                          pwprot.STATUS_FINISHED)
 
-        # Check there is an o
+        # Check there is an output
         self.assertOutput(prot)
 
         outputs = [o for o in prot.iterOutputAttributes()]
 
         # We are intentionally ignoring a protocol with o (EMObject)
         # That has been continued, We do not find a real case now.
         self.assertEqual(1, len(outputs),
```

### Comparing `scipion-pyworkflow-3.0.9/pyworkflowtests/tests/test_utils.py` & `scipion-pyworkflow-3.1.0/pyworkflowtests/tests/test_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from subprocess import Popen
 from io import StringIO
 
 from pyworkflow import APPS
 from pyworkflow.utils.process import killWithChilds
 from pyworkflow.tests import *
-from pyworkflow.utils import utils, prettyDict
+from pyworkflow.utils import utils, prettyDict, getListFromValues
 from pyworkflow.utils import ProgressBar
 
 
 class TestBibtex(BaseTest):
     """ Some minor tests to the bibtexparser library. """
 
     @classmethod
@@ -76,24 +76,47 @@
         time.sleep(5)
         killWithChilds(p.pid)
 
 
 class TestGetListFromRangeString(BaseTest):
 
     def test_getListFromRangeString(self):
-        inputStrings = ["1,5-8,10",         "2,6,9-11",        "2 5, 6-8"]
-        outputLists = [[1, 5, 6, 7, 8, 10], [2, 6, 9, 10, 11], [2, 5, 6, 7, 8]]
+        inputStrings = ["1,5-8,10"        , "2,6,9-11"       , "2 5, 6-8"     , "1-4 8"]
+        outputLists = [[1, 5, 6, 7, 8, 10], [2, 6, 9, 10, 11], [2, 5, 6, 7, 8], [1,2,3,4, 8]]
 
         for s, o in zip(inputStrings, outputLists):
             self.assertEqual(o, pwutils.getListFromRangeString(s))
             # Check that also works properly with spaces as delimiters
             s2 = s.replace(',', ' ')
             self.assertEqual(o, pwutils.getListFromRangeString(s2))
 
 
+class TestListFromValues(unittest.TestCase):
+    """ Tests list created from str"""
+
+    def _callAndAssert(self, strValue, expected, length=None, caster=str):
+
+        result = getListFromValues( strValue, length, caster)
+
+        self.assertEqual(result, expected, "List from string does not work for %s" % strValue)
+
+    def test_getListFromValues(self):
+        """ Test numeric list definitions like:
+            '1 1 2x2 4 4' -> ['1', '1', '2', '2', '4', '4']
+            '2x3, 3x4, 1' -> ['3', '3', '4', '4', '4', '1']"
+        """
+
+        self._callAndAssert('1 1 2x2 4 4', ['1', '1', '2', '2', '4', '4'])
+        self._callAndAssert('2x3, 3x4, 1',['3', '3', '4', '4', '4', '1'])
+        self._callAndAssert('2,3,4,1', [2, 3, 4, 1], caster=int)
+        self._callAndAssert('2 , 3 , 4 , 1', [2, 3, 4, 1], caster=int)
+        self._callAndAssert('2,3.3,4', [2.0, 3.3, 4.0], caster=float)
+
+
+
 class TestProgressBar(unittest.TestCase):
 
     def caller(self, total, step, fmt, resultGold):
         ti = time.time()
         result = StringIO()
         pb = ProgressBar(total=total, fmt=fmt, output=result,
                          extraArgs={'objectId': 33})
```

### Comparing `scipion-pyworkflow-3.0.9/scipion_pyworkflow.egg-info/SOURCES.txt` & `scipion-pyworkflow-3.1.0/scipion_pyworkflow.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -40,18 +40,22 @@
 pyworkflow/gui/tree.py
 pyworkflow/gui/widgets.py
 pyworkflow/gui/project/__init__.py
 pyworkflow/gui/project/base.py
 pyworkflow/gui/project/constants.py
 pyworkflow/gui/project/labels.py
 pyworkflow/gui/project/project.py
+pyworkflow/gui/project/searchprotocol.py
+pyworkflow/gui/project/searchrun.py
+pyworkflow/gui/project/steps.py
 pyworkflow/gui/project/utils.py
 pyworkflow/gui/project/viewdata.py
 pyworkflow/gui/project/viewprojects.py
 pyworkflow/gui/project/viewprotocols.py
+pyworkflow/gui/project/viewprotocols_extra.py
 pyworkflow/mapper/__init__.py
 pyworkflow/mapper/mapper.py
 pyworkflow/mapper/sqlite.py
 pyworkflow/mapper/sqlite_db.py
 pyworkflow/mapper/xmlmapper.py
 pyworkflow/project/__init__.py
 pyworkflow/project/config.py
@@ -72,122 +76,117 @@
 pyworkflow/protocol/constants.py
 pyworkflow/protocol/executor.py
 pyworkflow/protocol/hosts.py
 pyworkflow/protocol/launch.py
 pyworkflow/protocol/package.py
 pyworkflow/protocol/params.py
 pyworkflow/protocol/protocol.py
-pyworkflow/resources/ChimeraLogoSmall.gif
-pyworkflow/resources/I2PC.gif
-pyworkflow/resources/background_section.gif
-pyworkflow/resources/bookmark.gif
-pyworkflow/resources/ccp4_200.gif
-pyworkflow/resources/class_obj.gif
-pyworkflow/resources/cryoem_logo.gif
-pyworkflow/resources/cryomethods_logo.gif
-pyworkflow/resources/debug.gif
-pyworkflow/resources/doc_icon.gif
-pyworkflow/resources/download_icon.gif
-pyworkflow/resources/error_page.jpg
-pyworkflow/resources/fa-arrow-left.gif
-pyworkflow/resources/fa-arrow-up.gif
-pyworkflow/resources/fa-ban.gif
-pyworkflow/resources/fa-bars.gif
-pyworkflow/resources/fa-check.gif
-pyworkflow/resources/fa-checked.gif
-pyworkflow/resources/fa-cog.gif
-pyworkflow/resources/fa-cogs.gif
-pyworkflow/resources/fa-database.gif
-pyworkflow/resources/fa-delete-operation.gif
-pyworkflow/resources/fa-download.gif
-pyworkflow/resources/fa-exclamation-triangle_alert.gif
-pyworkflow/resources/fa-external-link.gif
-pyworkflow/resources/fa-eye.gif
-pyworkflow/resources/fa-failure.gif
-pyworkflow/resources/fa-file-o.gif
-pyworkflow/resources/fa-files-o.gif
-pyworkflow/resources/fa-folder-open.gif
-pyworkflow/resources/fa-home.gif
-pyworkflow/resources/fa-iconmoon-link.gif
-pyworkflow/resources/fa-info-circle_alert.gif
-pyworkflow/resources/fa-install.gif
-pyworkflow/resources/fa-installed.gif
-pyworkflow/resources/fa-laptop.gif
-pyworkflow/resources/fa-lightbulb-o.gif
-pyworkflow/resources/fa-list-ul.gif
-pyworkflow/resources/fa-magic.gif
-pyworkflow/resources/fa-minus-square.gif
-pyworkflow/resources/fa-next.gif
-pyworkflow/resources/fa-paint-brush.gif
-pyworkflow/resources/fa-pencil.gif
-pyworkflow/resources/fa-play-circle-o.gif
-pyworkflow/resources/fa-plus-circle.gif
-pyworkflow/resources/fa-plus-square.gif
-pyworkflow/resources/fa-previous.gif
-pyworkflow/resources/fa-processing.gif
-pyworkflow/resources/fa-question-circle.gif
-pyworkflow/resources/fa-refresh.gif
-pyworkflow/resources/fa-rocket.gif
-pyworkflow/resources/fa-save.gif
-pyworkflow/resources/fa-search.gif
-pyworkflow/resources/fa-sign-in.gif
-pyworkflow/resources/fa-sign-out.gif
-pyworkflow/resources/fa-sitemap.gif
-pyworkflow/resources/fa-stop-workflow.gif
-pyworkflow/resources/fa-stop.gif
-pyworkflow/resources/fa-tags.gif
-pyworkflow/resources/fa-times-circle_alert.gif
-pyworkflow/resources/fa-times.gif
-pyworkflow/resources/fa-to_install.gif
-pyworkflow/resources/fa-trash-o.gif
-pyworkflow/resources/fa-unchecked.gif
-pyworkflow/resources/fa-undo.gif
-pyworkflow/resources/fa-uninstall.gif
-pyworkflow/resources/fa-update.gif
-pyworkflow/resources/fa-upload.gif
-pyworkflow/resources/favicon.gif
-pyworkflow/resources/favicon.ico
-pyworkflow/resources/file.gif
-pyworkflow/resources/file_folder.gif
-pyworkflow/resources/file_generic.gif
-pyworkflow/resources/file_image.gif
-pyworkflow/resources/file_java.gif
-pyworkflow/resources/file_log.gif
-pyworkflow/resources/file_md.gif
-pyworkflow/resources/file_python.gif
-pyworkflow/resources/file_sqlite.gif
-pyworkflow/resources/file_stack.gif
-pyworkflow/resources/file_text.gif
-pyworkflow/resources/file_vol.gif
+pyworkflow/resources/backward-solid.png
+pyworkflow/resources/beta.png
+pyworkflow/resources/binoculares.png
+pyworkflow/resources/bookmark.png
+pyworkflow/resources/broom-solid.png
+pyworkflow/resources/class_obj.png
+pyworkflow/resources/clipboard-regular.png
+pyworkflow/resources/code-branch-solid.png
+pyworkflow/resources/debug.png
+pyworkflow/resources/fa-arrow-down.png
+pyworkflow/resources/fa-arrow-left.png
+pyworkflow/resources/fa-arrow-up.png
+pyworkflow/resources/fa-ban.png
+pyworkflow/resources/fa-bars.png
+pyworkflow/resources/fa-check.png
+pyworkflow/resources/fa-checked.png
+pyworkflow/resources/fa-cog.png
+pyworkflow/resources/fa-cogs.png
+pyworkflow/resources/fa-database.png
+pyworkflow/resources/fa-delete-operation.png
+pyworkflow/resources/fa-download.png
+pyworkflow/resources/fa-exclamation-triangle_alert.png
+pyworkflow/resources/fa-external-link.png
+pyworkflow/resources/fa-eye.png
+pyworkflow/resources/fa-failure.png
+pyworkflow/resources/fa-file-o.png
+pyworkflow/resources/fa-files-o.png
+pyworkflow/resources/fa-folder-open.png
+pyworkflow/resources/fa-home.png
+pyworkflow/resources/fa-info-circle_alert.png
+pyworkflow/resources/fa-install.png
+pyworkflow/resources/fa-installed.png
+pyworkflow/resources/fa-lightbulb-o.png
+pyworkflow/resources/fa-list-ul.png
+pyworkflow/resources/fa-magic.png
+pyworkflow/resources/fa-minus-square.png
+pyworkflow/resources/fa-next.png
+pyworkflow/resources/fa-pencil.png
+pyworkflow/resources/fa-play-circle-o.png
+pyworkflow/resources/fa-plus-square.png
+pyworkflow/resources/fa-previous.png
+pyworkflow/resources/fa-processing.png
+pyworkflow/resources/fa-question-circle.png
+pyworkflow/resources/fa-refresh.png
+pyworkflow/resources/fa-rocket.png
+pyworkflow/resources/fa-save.png
+pyworkflow/resources/fa-search.png
+pyworkflow/resources/fa-sign-in.png
+pyworkflow/resources/fa-sign-out.png
+pyworkflow/resources/fa-sitemap.png
+pyworkflow/resources/fa-stop-workflow.png
+pyworkflow/resources/fa-stop.png
+pyworkflow/resources/fa-tags.png
+pyworkflow/resources/fa-times-circle_alert.png
+pyworkflow/resources/fa-times.png
+pyworkflow/resources/fa-to_install.png
+pyworkflow/resources/fa-trash-o.png
+pyworkflow/resources/fa-unchecked.png
+pyworkflow/resources/fa-undo.png
+pyworkflow/resources/fa-uninstall.png
+pyworkflow/resources/fa-update.png
+pyworkflow/resources/fa-upload.png
+pyworkflow/resources/file.png
+pyworkflow/resources/file_folder.png
+pyworkflow/resources/file_folder_link.png
+pyworkflow/resources/file_generic.png
+pyworkflow/resources/file_generic_link.png
+pyworkflow/resources/file_image.png
+pyworkflow/resources/file_image_link.png
+pyworkflow/resources/file_java.png
+pyworkflow/resources/file_log.png
+pyworkflow/resources/file_md.png
+pyworkflow/resources/file_md_link.png
+pyworkflow/resources/file_python.png
+pyworkflow/resources/file_sqlite.png
+pyworkflow/resources/file_stack.png
+pyworkflow/resources/file_stack_link.png
+pyworkflow/resources/file_text.png
+pyworkflow/resources/file_vol.png
 pyworkflow/resources/loading.gif
-pyworkflow/resources/logoInstruct.gif
-pyworkflow/resources/logo_cnb_without_title.gif
-pyworkflow/resources/logo_i2pc_with_title.gif
-pyworkflow/resources/newProt.gif
-pyworkflow/resources/no-image.gif
-pyworkflow/resources/no-image.jpg
-pyworkflow/resources/no-image128.gif
-pyworkflow/resources/phenix.gif
-pyworkflow/resources/prot_disabled.gif
-pyworkflow/resources/python_file.gif
-pyworkflow/resources/question.gif
-pyworkflow/resources/rename.gif
-pyworkflow/resources/root.gif
-pyworkflow/resources/scipion_bn.gif
-pyworkflow/resources/scipion_icon.gif
+pyworkflow/resources/new.png
+pyworkflow/resources/no-image.png
+pyworkflow/resources/no-image128.png
+pyworkflow/resources/paste-solid.png
+pyworkflow/resources/power-off-solid.png
+pyworkflow/resources/production.png
+pyworkflow/resources/prot_disabled.png
+pyworkflow/resources/question.png
+pyworkflow/resources/rename.png
+pyworkflow/resources/root.png
+pyworkflow/resources/scipion_bn.png
+pyworkflow/resources/scipion_icon.png
 pyworkflow/resources/scipion_icon.svg
-pyworkflow/resources/scipion_icon_proj.gif
-pyworkflow/resources/scipion_icon_projs.gif
-pyworkflow/resources/scipion_icon_prot.gif
-pyworkflow/resources/scipion_logo.gif
-pyworkflow/resources/scipion_logo_normal.gif
-pyworkflow/resources/scipion_logo_small.gif
-pyworkflow/resources/scipion_logo_small_web.gif
-pyworkflow/resources/scipion_logo_transparent.gif
-pyworkflow/resources/users.gif
+pyworkflow/resources/scipion_icon_proj.png
+pyworkflow/resources/scipion_icon_projs.png
+pyworkflow/resources/scipion_icon_prot.png
+pyworkflow/resources/scipion_logo.png
+pyworkflow/resources/scipion_logo_normal.png
+pyworkflow/resources/scipion_logo_small.png
+pyworkflow/resources/updated.png
+pyworkflow/resources/users.png
+pyworkflow/resources/wait.gif
+pyworkflow/resources/workflow.png
 pyworkflow/resources/showj/arrowDown.png
 pyworkflow/resources/showj/arrowUp.png
 pyworkflow/resources/showj/background_section.png
 pyworkflow/resources/showj/colRowModeOff.png
 pyworkflow/resources/showj/colRowModeOn.png
 pyworkflow/resources/showj/delete.png
 pyworkflow/resources/showj/doc_icon.png
@@ -207,25 +206,23 @@
 pyworkflow/resources/showj/volumeOn.png
 pyworkflow/tests/__init__.py
 pyworkflow/tests/test_utils.py
 pyworkflow/tests/tests.py
 pyworkflow/utils/__init__.py
 pyworkflow/utils/dataset.py
 pyworkflow/utils/echo.py
-pyworkflow/utils/file_transfer.py
 pyworkflow/utils/graph.py
 pyworkflow/utils/log.py
 pyworkflow/utils/mpi.py
 pyworkflow/utils/path.py
 pyworkflow/utils/process.py
 pyworkflow/utils/profiler.py
 pyworkflow/utils/progressbar.py
 pyworkflow/utils/properties.py
 pyworkflow/utils/reflection.py
-pyworkflow/utils/remote.py
 pyworkflow/utils/utils.py
 pyworkflow/utils/which.py
 pyworkflow/webservices/__init__.py
 pyworkflow/webservices/config.py
 pyworkflow/webservices/notifier.py
 pyworkflow/webservices/repository.py
 pyworkflowtests/__init__.py
@@ -238,14 +235,15 @@
 pyworkflowtests/tests/test_logs.py
 pyworkflowtests/tests/test_mappers.py
 pyworkflowtests/tests/test_object.py
 pyworkflowtests/tests/test_project.py
 pyworkflowtests/tests/test_protocol_execution.py
 pyworkflowtests/tests/test_protocol_export.py
 pyworkflowtests/tests/test_protocol_output.py
+pyworkflowtests/tests/test_streaming.py
 pyworkflowtests/tests/test_utils.py
 scipion_pyworkflow.egg-info/PKG-INFO
 scipion_pyworkflow.egg-info/SOURCES.txt
 scipion_pyworkflow.egg-info/dependency_links.txt
 scipion_pyworkflow.egg-info/entry_points.txt
 scipion_pyworkflow.egg-info/requires.txt
 scipion_pyworkflow.egg-info/top_level.txt
```

### Comparing `scipion-pyworkflow-3.0.9/setup.py` & `scipion-pyworkflow-3.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,14 +42,33 @@
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 # Read requirements.txt
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
+required = []
+dependency_links = []
+
+# Do not add to required lines pointing to Git repositories
+EGG_MARK = '#egg='
+for line in requirements:
+    if line.startswith('-e git:') or line.startswith('-e git+') or \
+            line.startswith('git:') or line.startswith('git+'):
+        line = line.lstrip('-e ')  # in case that is using "-e"
+        if EGG_MARK in line:
+            package_name = line[line.find(EGG_MARK) + len(EGG_MARK):]
+            repository = line[:line.find(EGG_MARK)]
+            required.append('%s @ %s' % (package_name, repository))
+            dependency_links.append(line)
+        else:
+            print('Dependency to a git repository should have the format:')
+            print('git+ssh://git@github.com/xxxxx/xxxxxx#egg=package_name')
+    else:
+        required.append(line)
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -117,32 +136,34 @@
     # For a list of valid classifiers, see
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 4 - Beta',
         # Indicate who your project is intended for
         'Intended Audience :: Science/Research',
         # Pick your license as you wish
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Topic :: Scientific/Engineering'
     ],
 
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a string of words separated by whitespace, not a list.
-    keywords='workflows science scipion electron-microscopy cryo-em '
+    keywords='workflows science electron-microscopy cryo-em '
              'structural-biology image-processing scipion',  # Optional
 
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
     #
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
@@ -154,17 +175,18 @@
     packages=find_packages(),
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=[requirements
+    install_requires=[required
                       ],  # Optional
 
+    dependency_links=dependency_links,
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
     # Similar to `install_requires` above, these must be valid existing
@@ -195,14 +217,17 @@
     # "scripts" keyword. Entry points provide cross-platform support and allow
     # `pip` to create the appropriate form of executable for the target
     # platform.
     #
     # For example, the following would provide a command called `sample` which
     # executes the function `main` from this package when invoked:
     entry_points={
+        'console_scripts': [
+            'fix_links = pyworkflow.project.scripts.fix_links:main',
+        ],
         'pyworkflow.plugin': 'pyworkflowtests = pyworkflowtests'
     },
 
     # List additional URLs that are relevant to your project as a dict.
     #
     # This field corresponds to the "Project-URL" metadata fields:
     # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
```

