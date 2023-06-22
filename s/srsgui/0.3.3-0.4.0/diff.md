# Comparing `tmp/srsgui-0.3.3.tar.gz` & `tmp/srsgui-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-wgfwh6vd\srsgui-0.3.3.tar", last modified: Wed Jun 14 20:06:43 2023, max compression
+gzip compressed data, was "C:\PyPI\srsgui\dist\.tmp-oktwxdg7\srsgui-0.4.0.tar", last modified: Thu Jun 22 23:50:07 2023, max compression
```

## Comparing `srsgui-0.3.3.tar` & `srsgui-0.4.0.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.304418 srsgui-0.3.3/
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.153942 srsgui-0.3.3/.github/
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.163914 srsgui-0.3.3/.github/workflows/
--rw-rw-rw-   0        0        0      388 2023-05-16 19:47:28.000000 srsgui-0.3.3/.github/workflows/pages.yml
--rw-rw-rw-   0        0        0     1356 2023-05-16 23:33:10.000000 srsgui-0.3.3/.gitignore
--rw-rw-rw-   0        0        0     1113 2023-05-16 18:54:46.000000 srsgui-0.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0     3965 2023-06-14 20:06:43.304418 srsgui-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     2985 2023-06-08 18:01:11.000000 srsgui-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.194236 srsgui-0.3.3/docs/
--rw-rw-rw-   0        0        0      654 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/Makefile
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.214237 srsgui-0.3.3/docs/_static/
--rw-rw-rw-   0        0        0    31067 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/cg-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    27242 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/cg-terminal-screen-capture.png
--rw-rw-rw-   0        0        0     5762 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/connect-dialog-box-capture.png
--rw-rw-rw-   0        0        0    88057 2023-06-08 18:01:11.000000 srsgui-0.3.3/docs/_static/dock_widget_floating.png
--rw-rw-rw-   0        0        0    97266 2023-06-08 18:01:11.000000 srsgui-0.3.3/docs/_static/dock_widgets_expanded.png
--rw-rw-rw-   0        0        0    71070 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/example-screen-capture-1.png
--rw-rw-rw-   0        0        0    71011 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/example-screen-capture-2.png
--rw-rw-rw-   0        0        0    56013 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/initial-screen-capture.png
--rw-rw-rw-   0        0        0    52123 2023-06-08 23:01:31.000000 srsgui-0.3.3/docs/_static/lockin-capture.png
--rw-rw-rw-   0        0        0    29667 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/osc-dir-terminal-screen-capture.png
--rw-rw-rw-   0        0        0    50740 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/second-task-screen-capture.png
--rw-rw-rw-   0        0        0    38581 2023-06-08 18:01:11.000000 srsgui-0.3.3/docs/_static/task_selection.png
--rw-rw-rw-   0        0        0    39412 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/terminal-with-example-2.png
--rw-rw-rw-   0        0        0    37573 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/_static/terminal-with-example.png
--rw-rw-rw-   0        0        0     8513 2023-06-12 22:58:25.000000 srsgui-0.3.3/docs/application.rst
--rw-rw-rw-   0        0        0      305 2023-05-24 20:30:53.000000 srsgui-0.3.3/docs/changelog.rst
--rw-rw-rw-   0        0        0     1924 2023-06-08 18:01:11.000000 srsgui-0.3.3/docs/conf.py
--rw-rw-rw-   0        0        0     6097 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/create-project.rst
--rw-rw-rw-   0        0        0     6656 2023-06-08 23:01:31.000000 srsgui-0.3.3/docs/create-task.rst
--rw-rw-rw-   0        0        0     6112 2023-06-08 23:01:31.000000 srsgui-0.3.3/docs/define-instrument.rst
--rw-rw-rw-   0        0        0    15640 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/example.rst
--rw-rw-rw-   0        0        0     3803 2023-06-13 16:35:19.000000 srsgui-0.3.3/docs/index.rst
--rw-rw-rw-   0        0        0     4405 2023-06-09 21:01:03.000000 srsgui-0.3.3/docs/installation.rst
--rwxrwxrwx   0        0        0      802 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/make.bat
--rw-rw-rw-   0        0        0       34 2023-05-16 19:47:28.000000 srsgui-0.3.3/docs/requirements..txt
--rw-rw-rw-   0        0        0      936 2023-05-16 18:43:29.000000 srsgui-0.3.3/docs/srsgui.inst.communications.rst
--rw-rw-rw-   0        0        0      930 2023-06-08 18:01:11.000000 srsgui-0.3.3/docs/srsgui.inst.rst
--rw-rw-rw-   0        0        0      113 2023-05-24 20:30:53.000000 srsgui-0.3.3/docs/srsgui.rst
--rw-rw-rw-   0        0        0     1077 2023-05-24 20:30:53.000000 srsgui-0.3.3/docs/srsgui.task.rst
--rw-rw-rw-   0        0        0     2065 2023-05-24 20:30:53.000000 srsgui-0.3.3/docs/srsgui.ui.commandtree.rst
--rw-rw-rw-   0        0        0      603 2023-05-24 20:30:53.000000 srsgui-0.3.3/docs/srsgui.ui.qt.rst
--rw-rw-rw-   0        0        0     1646 2023-05-24 20:30:53.000000 srsgui-0.3.3/docs/srsgui.ui.rst
--rw-rw-rw-   0        0        0      620 2023-06-14 16:11:01.000000 srsgui-0.3.3/docs/troubleshooting.rst
--rw-rw-rw-   0        0        0     1489 2023-06-14 20:05:33.000000 srsgui-0.3.3/pyproject.toml
--rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.3.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-14 20:06:43.314386 srsgui-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.214237 srsgui-0.3.3/srsgui/
--rw-rw-rw-   0        0        0     1537 2023-06-14 20:05:24.000000 srsgui-0.3.3/srsgui/__init__.py
--rw-rw-rw-   0        0        0      314 2023-05-15 21:54:54.000000 srsgui-0.3.3/srsgui/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.153942 srsgui-0.3.3/srsgui/examples/
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.224236 srsgui-0.3.3/srsgui/examples/oscilloscope example/
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.224236 srsgui-0.3.3/srsgui/examples/oscilloscope example/instruments/
--rw-rw-rw-   0        0        0     1828 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/instruments/cg635.py
--rw-rw-rw-   0        0        0     3146 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/instruments/sds1202.py
--rw-rw-rw-   0        0        0     1977 2023-05-15 21:54:54.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.234237 srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/
--rw-rw-rw-   0        0        0     2522 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/fifth.py
--rw-rw-rw-   0        0        0     1662 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/first.py
--rw-rw-rw-   0        0        0     4099 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/fourth.py
--rw-rw-rw-   0        0        0     2250 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/second.py
--rw-rw-rw-   0        0        0     2014 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/third.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.244265 srsgui-0.3.3/srsgui/inst/
--rw-rw-rw-   0        0        0     1074 2023-05-15 21:54:54.000000 srsgui-0.3.3/srsgui/inst/__init__.py
--rw-rw-rw-   0        0        0     9907 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/inst/commands.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.254237 srsgui-0.3.3/srsgui/inst/communications/
--rw-rw-rw-   0        0        0      126 2023-05-15 21:54:54.000000 srsgui-0.3.3/srsgui/inst/communications/__init__.py
--rw-rw-rw-   0        0        0     8308 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/inst/communications/interface.py
--rw-rw-rw-   0        0        0     1276 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/inst/communications/serial_ports.py
--rw-rw-rw-   0        0        0     8774 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/inst/communications/serialinterface.py
--rw-rw-rw-   0        0        0    11333 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/inst/communications/tcpipinterface.py
--rw-rw-rw-   0        0        0    15127 2023-06-08 18:01:11.000000 srsgui-0.3.3/srsgui/inst/component.py
--rw-rw-rw-   0        0        0      844 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/inst/exceptions.py
--rw-rw-rw-   0        0        0    10410 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/inst/indexcommands.py
--rw-rw-rw-   0        0        0     9826 2023-06-08 18:01:11.000000 srsgui-0.3.3/srsgui/inst/instrument.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.264267 srsgui-0.3.3/srsgui/task/
--rw-rw-rw-   0        0        0        2 2023-05-15 21:54:54.000000 srsgui-0.3.3/srsgui/task/__init__.py
--rw-rw-rw-   0        0        0      811 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/task/callbacks.py
--rw-rw-rw-   0        0        0     6606 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/task/config.py
--rw-rw-rw-   0        0        0     5417 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/task/inputs.py
--rw-rw-rw-   0        0        0     6938 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/task/sessionhandler.py
--rw-rw-rw-   0        0        0    23469 2023-06-08 18:01:11.000000 srsgui-0.3.3/srsgui/task/task.py
--rw-rw-rw-   0        0        0     4225 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/task/taskresult.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.284384 srsgui-0.3.3/srsgui/ui/
--rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.3.3/srsgui/ui/__init__.py
--rw-rw-rw-   0        0        0     3894 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/commandhandler.py
--rw-rw-rw-   0        0        0     6880 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/ui/commandterminal.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.304418 srsgui-0.3.3/srsgui/ui/commandtree/
--rw-rw-rw-   0        0        0        0 2023-05-19 00:30:39.000000 srsgui-0.3.3/srsgui/ui/commandtree/__init__.py
--rw-rw-rw-   0        0        0     3941 2023-05-23 19:11:06.000000 srsgui-0.3.3/srsgui/ui/commandtree/commanddelegate.py
--rw-rw-rw-   0        0        0     1603 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/commandtree/commandhandler.py
--rw-rw-rw-   0        0        0    12359 2023-06-08 18:01:11.000000 srsgui-0.3.3/srsgui/ui/commandtree/commanditem.py
--rw-rw-rw-   0        0        0     8669 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/ui/commandtree/commandmodel.py
--rw-rw-rw-   0        0        0     5109 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/ui/commandtree/commandspinbox.py
--rw-rw-rw-   0        0        0     3452 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/commandtree/commandtreeview.py
--rw-rw-rw-   0        0        0     4851 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/ui/commandtree/commandtreewidget.py
--rw-rw-rw-   0        0        0     4806 2023-05-15 21:54:55.000000 srsgui-0.3.3/srsgui/ui/commandtree/ui_commandtreewidget.py
--rw-rw-rw-   0        0        0     9798 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/connectdlg.py
--rw-rw-rw-   0        0        0     3975 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/deviceinfohandler.py
--rw-rw-rw-   0        0        0    15880 2023-06-08 18:01:11.000000 srsgui-0.3.3/srsgui/ui/dockhandler.py
--rw-rw-rw-   0        0        0    13826 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/ui/inputpanel.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.304418 srsgui-0.3.3/srsgui/ui/qt/
--rw-rw-rw-   0        0        0      799 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/qt/QtCore.py
--rw-rw-rw-   0        0        0      677 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/qt/QtGui.py
--rw-rw-rw-   0        0        0      777 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/qt/QtWidgets.py
--rw-rw-rw-   0        0        0     1449 2023-05-24 20:30:53.000000 srsgui-0.3.3/srsgui/ui/qt/__init__.py
--rw-rw-rw-   0        0        0     1285 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/qtloghandler.py
--rw-rw-rw-   0        0        0      268 2023-05-15 21:54:55.000000 srsgui-0.3.3/srsgui/ui/resource.qrc
--rw-rw-rw-   0        0        0    15479 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/resource_rc.py
--rw-rw-rw-   0        0        0     2717 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/signalhandler.py
--rw-rw-rw-   0        0        0    47891 2023-05-15 21:54:55.000000 srsgui-0.3.3/srsgui/ui/srslogo.jpg
--rw-rw-rw-   0        0        0     1005 2023-05-16 18:43:29.000000 srsgui-0.3.3/srsgui/ui/stdout.py
--rw-rw-rw-   0        0        0    25601 2023-06-08 23:01:31.000000 srsgui-0.3.3/srsgui/ui/taskmain.py
--rw-rw-rw-   0        0        0    10403 2023-05-15 21:54:55.000000 srsgui-0.3.3/srsgui/ui/taskmain.ui
--rw-rw-rw-   0        0        0    11293 2023-05-15 21:54:55.000000 srsgui-0.3.3/srsgui/ui/ui_taskmain.py
-drwxrwxrwx   0        0        0        0 2023-06-14 20:06:43.224236 srsgui-0.3.3/srsgui.egg-info/
--rw-rw-rw-   0        0        0     3965 2023-06-14 20:06:43.000000 srsgui-0.3.3/srsgui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3170 2023-06-14 20:06:43.000000 srsgui-0.3.3/srsgui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 20:06:43.000000 srsgui-0.3.3/srsgui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-14 20:06:43.000000 srsgui-0.3.3/srsgui.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      103 2023-06-14 20:06:43.000000 srsgui-0.3.3/srsgui.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-14 20:06:43.000000 srsgui-0.3.3/srsgui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.998221 srsgui-0.4.0/
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.877909 srsgui-0.4.0/.github/
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.888958 srsgui-0.4.0/.github/workflows/
+-rw-rw-rw-   0        0        0      388 2023-06-19 18:04:40.000000 srsgui-0.4.0/.github/workflows/pages.yml
+-rw-rw-rw-   0        0        0     1356 2023-05-16 23:33:10.000000 srsgui-0.4.0/.gitignore
+-rw-rw-rw-   0        0        0     1113 2023-05-16 18:54:46.000000 srsgui-0.4.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     3965 2023-06-22 23:50:06.998221 srsgui-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2985 2023-06-19 17:56:19.000000 srsgui-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.918705 srsgui-0.4.0/docs/
+-rw-rw-rw-   0        0        0      654 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/Makefile
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.938704 srsgui-0.4.0/docs/_static/
+-rw-rw-rw-   0        0        0    31067 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/cg-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    27242 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/cg-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0     5762 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/connect-dialog-box-capture.png
+-rw-rw-rw-   0        0        0    88057 2023-06-08 18:01:11.000000 srsgui-0.4.0/docs/_static/dock_widget_floating.png
+-rw-rw-rw-   0        0        0    97266 2023-06-08 18:01:11.000000 srsgui-0.4.0/docs/_static/dock_widgets_expanded.png
+-rw-rw-rw-   0        0        0    71070 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/example-screen-capture-1.png
+-rw-rw-rw-   0        0        0    71011 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/example-screen-capture-2.png
+-rw-rw-rw-   0        0        0    56013 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/initial-screen-capture.png
+-rw-rw-rw-   0        0        0    52123 2023-06-08 23:01:31.000000 srsgui-0.4.0/docs/_static/lockin-capture.png
+-rw-rw-rw-   0        0        0    29667 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/osc-dir-terminal-screen-capture.png
+-rw-rw-rw-   0        0        0    50740 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/second-task-screen-capture.png
+-rw-rw-rw-   0        0        0    38581 2023-06-08 18:01:11.000000 srsgui-0.4.0/docs/_static/task_selection.png
+-rw-rw-rw-   0        0        0    39412 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/terminal-with-example-2.png
+-rw-rw-rw-   0        0        0    37573 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/_static/terminal-with-example.png
+-rw-rw-rw-   0        0        0     8513 2023-06-15 00:44:23.000000 srsgui-0.4.0/docs/application.rst
+-rw-rw-rw-   0        0        0      839 2023-06-21 20:11:21.000000 srsgui-0.4.0/docs/changelog.rst
+-rw-rw-rw-   0        0        0     1924 2023-06-08 18:01:11.000000 srsgui-0.4.0/docs/conf.py
+-rw-rw-rw-   0        0        0     6097 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/create-project.rst
+-rw-rw-rw-   0        0        0     6656 2023-06-08 23:01:31.000000 srsgui-0.4.0/docs/create-task.rst
+-rw-rw-rw-   0        0        0     6112 2023-06-08 23:01:31.000000 srsgui-0.4.0/docs/define-instrument.rst
+-rw-rw-rw-   0        0        0    15640 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/example.rst
+-rw-rw-rw-   0        0        0     3803 2023-06-15 00:44:23.000000 srsgui-0.4.0/docs/index.rst
+-rw-rw-rw-   0        0        0     4405 2023-06-15 00:44:23.000000 srsgui-0.4.0/docs/installation.rst
+-rwxrwxrwx   0        0        0      802 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/make.bat
+-rw-rw-rw-   0        0        0       34 2023-05-16 19:47:28.000000 srsgui-0.4.0/docs/requirements..txt
+-rw-rw-rw-   0        0        0      936 2023-05-16 18:43:29.000000 srsgui-0.4.0/docs/srsgui.inst.communications.rst
+-rw-rw-rw-   0        0        0      930 2023-06-08 18:01:11.000000 srsgui-0.4.0/docs/srsgui.inst.rst
+-rw-rw-rw-   0        0        0      113 2023-05-24 20:30:53.000000 srsgui-0.4.0/docs/srsgui.rst
+-rw-rw-rw-   0        0        0     1077 2023-05-24 20:30:53.000000 srsgui-0.4.0/docs/srsgui.task.rst
+-rw-rw-rw-   0        0        0     2065 2023-05-24 20:30:53.000000 srsgui-0.4.0/docs/srsgui.ui.commandtree.rst
+-rw-rw-rw-   0        0        0      603 2023-05-24 20:30:53.000000 srsgui-0.4.0/docs/srsgui.ui.qt.rst
+-rw-rw-rw-   0        0        0     1646 2023-05-24 20:30:53.000000 srsgui-0.4.0/docs/srsgui.ui.rst
+-rw-rw-rw-   0        0        0      620 2023-06-15 00:44:23.000000 srsgui-0.4.0/docs/troubleshooting.rst
+-rw-rw-rw-   0        0        0     1489 2023-06-15 00:44:23.000000 srsgui-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       37 2023-01-30 16:55:49.000000 srsgui-0.4.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-22 23:50:06.998221 srsgui-0.4.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-02-09 00:46:42.000000 srsgui-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.938704 srsgui-0.4.0/srsgui/
+-rw-rw-rw-   0        0        0     1537 2023-06-21 20:11:21.000000 srsgui-0.4.0/srsgui/__init__.py
+-rw-rw-rw-   0        0        0      314 2023-05-15 21:54:54.000000 srsgui-0.4.0/srsgui/__main__.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.888958 srsgui-0.4.0/srsgui/examples/
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.948705 srsgui-0.4.0/srsgui/examples/oscilloscope example/
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.948705 srsgui-0.4.0/srsgui/examples/oscilloscope example/instruments/
+-rw-rw-rw-   0        0        0     1828 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/instruments/cg635.py
+-rw-rw-rw-   0        0        0     3146 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/instruments/sds1202.py
+-rw-rw-rw-   0        0        0     1977 2023-06-19 17:56:19.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.958705 srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/
+-rw-rw-rw-   0        0        0     2522 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/fifth.py
+-rw-rw-rw-   0        0        0     1662 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/first.py
+-rw-rw-rw-   0        0        0     4099 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/fourth.py
+-rw-rw-rw-   0        0        0     2250 2023-06-19 17:56:19.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/second.py
+-rw-rw-rw-   0        0        0     2014 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/third.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.958705 srsgui-0.4.0/srsgui/inst/
+-rw-rw-rw-   0        0        0     1074 2023-05-15 21:54:54.000000 srsgui-0.4.0/srsgui/inst/__init__.py
+-rw-rw-rw-   0        0        0     9907 2023-05-24 20:30:53.000000 srsgui-0.4.0/srsgui/inst/commands.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.968705 srsgui-0.4.0/srsgui/inst/communications/
+-rw-rw-rw-   0        0        0      126 2023-05-15 21:54:54.000000 srsgui-0.4.0/srsgui/inst/communications/__init__.py
+-rw-rw-rw-   0        0        0     8308 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/inst/communications/interface.py
+-rw-rw-rw-   0        0        0     1276 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/inst/communications/serial_ports.py
+-rw-rw-rw-   0        0        0     8774 2023-06-22 22:17:34.000000 srsgui-0.4.0/srsgui/inst/communications/serialinterface.py
+-rw-rw-rw-   0        0        0    11333 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/inst/communications/tcpipinterface.py
+-rw-rw-rw-   0        0        0    19291 2023-06-22 22:15:32.000000 srsgui-0.4.0/srsgui/inst/component.py
+-rw-rw-rw-   0        0        0      844 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/inst/exceptions.py
+-rw-rw-rw-   0        0        0    10410 2023-05-24 20:30:53.000000 srsgui-0.4.0/srsgui/inst/indexcommands.py
+-rw-rw-rw-   0        0        0     9990 2023-06-19 18:04:40.000000 srsgui-0.4.0/srsgui/inst/instrument.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.978705 srsgui-0.4.0/srsgui/task/
+-rw-rw-rw-   0        0        0        2 2023-05-15 21:54:54.000000 srsgui-0.4.0/srsgui/task/__init__.py
+-rw-rw-rw-   0        0        0      811 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/task/callbacks.py
+-rw-rw-rw-   0        0        0     6989 2023-06-21 20:11:21.000000 srsgui-0.4.0/srsgui/task/config.py
+-rw-rw-rw-   0        0        0     5856 2023-06-21 20:11:21.000000 srsgui-0.4.0/srsgui/task/inputs.py
+-rw-rw-rw-   0        0        0     6938 2023-05-24 20:30:53.000000 srsgui-0.4.0/srsgui/task/sessionhandler.py
+-rw-rw-rw-   0        0        0    23469 2023-06-08 18:01:11.000000 srsgui-0.4.0/srsgui/task/task.py
+-rw-rw-rw-   0        0        0     4225 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/task/taskresult.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.988215 srsgui-0.4.0/srsgui/ui/
+-rw-rw-rw-   0        0        0        0 2023-05-15 21:54:55.000000 srsgui-0.4.0/srsgui/ui/__init__.py
+-rw-rw-rw-   0        0        0     3894 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/commandhandler.py
+-rw-rw-rw-   0        0        0     6880 2023-05-24 20:30:53.000000 srsgui-0.4.0/srsgui/ui/commandterminal.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.998221 srsgui-0.4.0/srsgui/ui/commandtree/
+-rw-rw-rw-   0        0        0        0 2023-05-19 00:30:39.000000 srsgui-0.4.0/srsgui/ui/commandtree/__init__.py
+-rw-rw-rw-   0        0        0     3941 2023-05-23 19:11:06.000000 srsgui-0.4.0/srsgui/ui/commandtree/commanddelegate.py
+-rw-rw-rw-   0        0        0     1603 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/commandtree/commandhandler.py
+-rw-rw-rw-   0        0        0    12605 2023-06-22 21:23:49.000000 srsgui-0.4.0/srsgui/ui/commandtree/commanditem.py
+-rw-rw-rw-   0        0        0     8669 2023-05-24 20:30:53.000000 srsgui-0.4.0/srsgui/ui/commandtree/commandmodel.py
+-rw-rw-rw-   0        0        0     5109 2023-05-24 20:30:53.000000 srsgui-0.4.0/srsgui/ui/commandtree/commandspinbox.py
+-rw-rw-rw-   0        0        0     3452 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/commandtree/commandtreeview.py
+-rw-rw-rw-   0        0        0     4852 2023-06-19 18:04:40.000000 srsgui-0.4.0/srsgui/ui/commandtree/commandtreewidget.py
+-rw-rw-rw-   0        0        0     4806 2023-05-15 21:54:55.000000 srsgui-0.4.0/srsgui/ui/commandtree/ui_commandtreewidget.py
+-rw-rw-rw-   0        0        0     9798 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/connectdlg.py
+-rw-rw-rw-   0        0        0     3975 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/deviceinfohandler.py
+-rw-rw-rw-   0        0        0    15880 2023-06-08 18:01:11.000000 srsgui-0.4.0/srsgui/ui/dockhandler.py
+-rw-rw-rw-   0        0        0    14950 2023-06-21 20:11:21.000000 srsgui-0.4.0/srsgui/ui/inputpanel.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.998221 srsgui-0.4.0/srsgui/ui/qt/
+-rw-rw-rw-   0        0        0      799 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/qt/QtCore.py
+-rw-rw-rw-   0        0        0      677 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/qt/QtGui.py
+-rw-rw-rw-   0        0        0      777 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/qt/QtWidgets.py
+-rw-rw-rw-   0        0        0     1449 2023-05-24 20:30:53.000000 srsgui-0.4.0/srsgui/ui/qt/__init__.py
+-rw-rw-rw-   0        0        0     1285 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/qtloghandler.py
+-rw-rw-rw-   0        0        0      268 2023-05-15 21:54:55.000000 srsgui-0.4.0/srsgui/ui/resource.qrc
+-rw-rw-rw-   0        0        0    15479 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/resource_rc.py
+-rw-rw-rw-   0        0        0     2717 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/signalhandler.py
+-rw-rw-rw-   0        0        0    47891 2023-05-15 21:54:55.000000 srsgui-0.4.0/srsgui/ui/srslogo.jpg
+-rw-rw-rw-   0        0        0     1005 2023-05-16 18:43:29.000000 srsgui-0.4.0/srsgui/ui/stdout.py
+-rw-rw-rw-   0        0        0    26525 2023-06-21 20:11:21.000000 srsgui-0.4.0/srsgui/ui/taskmain.py
+-rw-rw-rw-   0        0        0    10403 2023-05-15 21:54:55.000000 srsgui-0.4.0/srsgui/ui/taskmain.ui
+-rw-rw-rw-   0        0        0    11293 2023-05-15 21:54:55.000000 srsgui-0.4.0/srsgui/ui/ui_taskmain.py
+drwxrwxrwx   0        0        0        0 2023-06-22 23:50:06.948705 srsgui-0.4.0/srsgui.egg-info/
+-rw-rw-rw-   0        0        0     3965 2023-06-22 23:50:06.000000 srsgui-0.4.0/srsgui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3170 2023-06-22 23:50:06.000000 srsgui-0.4.0/srsgui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-22 23:50:06.000000 srsgui-0.4.0/srsgui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-22 23:50:06.000000 srsgui-0.4.0/srsgui.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      103 2023-06-22 23:50:06.000000 srsgui-0.4.0/srsgui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-22 23:50:06.000000 srsgui-0.4.0/srsgui.egg-info/top_level.txt
```

### Comparing `srsgui-0.3.3/.gitignore` & `srsgui-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/LICENSE.txt` & `srsgui-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/PKG-INFO` & `srsgui-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.3.3
+Version: 0.4.0
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
```

### Comparing `srsgui-0.3.3/README.md` & `srsgui-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/Makefile` & `srsgui-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/_static/cg-dir-terminal-screen-capture.png` & `srsgui-0.4.0/docs/_static/cg-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/_static/cg-terminal-screen-capture.png` & `srsgui-0.4.0/docs/_static/cg-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/_static/connect-dialog-box-capture.png` & `srsgui-0.4.0/docs/_static/connect-dialog-box-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/_static/dock_widget_floating.png` & `srsgui-0.4.0/docs/_static/dock_widget_floating.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/_static/dock_widgets_expanded.png` & `srsgui-0.4.0/docs/_static/dock_widgets_expanded.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/_static/example-screen-capture-1.png` & `srsgui-0.4.0/docs/_static/example-screen-capture-1.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/_static/example-screen-capture-2.png` & `srsgui-0.4.0/docs/_static/example-screen-capture-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/_static/initial-screen-capture.png` & `srsgui-0.4.0/docs/_static/initial-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/_static/lockin-capture.png` & `srsgui-0.4.0/docs/_static/lockin-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/_static/osc-dir-terminal-screen-capture.png` & `srsgui-0.4.0/docs/_static/osc-dir-terminal-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/_static/second-task-screen-capture.png` & `srsgui-0.4.0/docs/_static/second-task-screen-capture.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/_static/task_selection.png` & `srsgui-0.4.0/docs/_static/task_selection.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/_static/terminal-with-example-2.png` & `srsgui-0.4.0/docs/_static/terminal-with-example-2.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/_static/terminal-with-example.png` & `srsgui-0.4.0/docs/_static/terminal-with-example.png`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/application.rst` & `srsgui-0.4.0/docs/application.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/conf.py` & `srsgui-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/create-project.rst` & `srsgui-0.4.0/docs/create-project.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/create-task.rst` & `srsgui-0.4.0/docs/create-task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/define-instrument.rst` & `srsgui-0.4.0/docs/define-instrument.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/example.rst` & `srsgui-0.4.0/docs/example.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/index.rst` & `srsgui-0.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/installation.rst` & `srsgui-0.4.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/make.bat` & `srsgui-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/srsgui.inst.communications.rst` & `srsgui-0.4.0/docs/srsgui.inst.communications.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/srsgui.inst.rst` & `srsgui-0.4.0/docs/srsgui.inst.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/srsgui.task.rst` & `srsgui-0.4.0/docs/srsgui.task.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/srsgui.ui.commandtree.rst` & `srsgui-0.4.0/docs/srsgui.ui.commandtree.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/srsgui.ui.qt.rst` & `srsgui-0.4.0/docs/srsgui.ui.qt.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/srsgui.ui.rst` & `srsgui-0.4.0/docs/srsgui.ui.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/docs/troubleshooting.rst` & `srsgui-0.4.0/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/pyproject.toml` & `srsgui-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/__init__.py` & `srsgui-0.4.0/srsgui/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,8 +22,8 @@
                         InstLoginFailureError, InstIdError, \
                         InstSetError, InstQueryError, InstIndexError
 
 from srsgui.inst import Interface, SerialInterface, TcpipInterface
 from srsgui.inst.instrument import Instrument
 from srsgui.inst.component import Component
 
-__version__ = "0.3.3"  # Global version number
+__version__ = "0.4.0"  # Global version number
```

### Comparing `srsgui-0.3.3/srsgui/examples/oscilloscope example/instruments/cg635.py` & `srsgui-0.4.0/srsgui/examples/oscilloscope example/instruments/cg635.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/examples/oscilloscope example/instruments/sds1202.py` & `srsgui-0.4.0/srsgui/examples/oscilloscope example/instruments/sds1202.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig` & `srsgui-0.4.0/srsgui/examples/oscilloscope example/oscilloscope example project.taskconfig`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/fifth.py` & `srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/fifth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/first.py` & `srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/first.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/fourth.py` & `srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/fourth.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/second.py` & `srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/second.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/examples/oscilloscope example/tasks/third.py` & `srsgui-0.4.0/srsgui/examples/oscilloscope example/tasks/third.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/inst/__init__.py` & `srsgui-0.4.0/srsgui/inst/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/inst/commands.py` & `srsgui-0.4.0/srsgui/inst/commands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/inst/communications/interface.py` & `srsgui-0.4.0/srsgui/inst/communications/interface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/inst/communications/serial_ports.py` & `srsgui-0.4.0/srsgui/inst/communications/serial_ports.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/inst/communications/serialinterface.py` & `srsgui-0.4.0/srsgui/inst/communications/serialinterface.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         try:
             self._serial.write(bytecmd)
         except (self.port_not_open_error, AttributeError):
             raise InstCommunicationError('Port not open to write')
         except serial.SerialException:
             raise InstCommunicationError("Sending cmd '{}' to port '{}' failed".format(cmd, self._port))
 
-    def _write_bibary(self, binary_array):
+    def _write_binary(self, binary_array):
         if type(binary_array) not in (bytes, bytearray):
             raise TypeError('_write_binary requires bytes or bytearray')
         try:
             self._serial.write(binary_array)
         except (self.port_not_open_error, AttributeError):
             raise InstCommunicationError('Port not open to write')
         except serial.SerialException:
```

### Comparing `srsgui-0.3.3/srsgui/inst/communications/tcpipinterface.py` & `srsgui-0.4.0/srsgui/inst/communications/tcpipinterface.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/inst/component.py` & `srsgui-0.4.0/srsgui/inst/component.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,15 +85,15 @@
 
         if not isinstance(parent.comm, Interface):
             raise TypeError('Invalid Interface instance')
 
         self._parent = parent
         self._parent._children.append(self)
         self.comm = parent.comm
-        self._add_parent_to_index_commands()
+        # self.add_parent_to_index_commands()  # it needs to run AFTER adding index commands in __init__() in a subclass
 
     def is_connected(self):
         """
         check if the current communication interface is open
         """
         return self.comm.is_connected()
 
@@ -113,37 +113,41 @@
 
         return self._name
 
     def update_components(self):
         """
         Update the communication interface of child components with the parent's
         """
-        self._add_parent_to_index_commands()
+        self.add_parent_to_index_commands()
         for child in self._children:
             child.comm = self.comm
             child.update_components()
-            child._add_parent_to_index_commands()
+            child.add_parent_to_index_commands()
 
     def get_lists(self, include_superclass=True):
         """
         Get the directory containing a list of subcomponents in this component,
         a list of commands available in the component,
         a list of  method available in the component and its superclass
         """
         return {
             'components': self.get_component_dict(),
             'commands': self.get_command_dict(include_superclass),
             'methods': self.get_method_list(include_superclass),
         }
 
-    def _add_parent_to_index_commands(self):
+    def add_parent_to_index_commands(self):
         # Add parent to ListCommands
         commands = self.get_command_dict()
         for cmd in commands:
-            instance = self.__class__.__dict__[cmd]
+            instance = None
+            if cmd in self.__class__.__dict__:
+                instance = instance = self.__class__.__dict__[cmd]
+            elif cmd in self.__dict__:
+                instance = instance = self.__dict__[cmd]
             if hasattr(instance, "_add_parent"):
                 instance._add_parent(self)
 
     def get_component_dict(self):
         """
         Get a dict of the child component of the component
 
@@ -172,29 +176,41 @@
             list(str)
                 list of commands
         """
         command_list = {}
         current_attributes = []
         end = -1 if include_superclass else 1
         for c in self.__class__.__mro__[:end]:  # loop through the classes including super classes
-            if not issubclass(c, Component):  # it should be subclass of Component
+            if not issubclass(c, Component):  # it should be a subclass of Component
                 break
             if c == Component:  # But it should not be Component
                 break
             for key in c.__dict__:
                 if key.startswith('_'):
                     continue
                 if key in current_attributes:
                     continue
                 current_attributes.append(key)
 
                 instance = c.__dict__[key]
                 if issubclass(instance.__class__, Command) or \
                    issubclass(instance.__class__, IndexCommand):
                     command_list[key] = (instance.__class__.__name__, instance.remote_command)
+        for key in self.__dict__:
+            if key.startswith('_'):
+                continue
+            if key in current_attributes:
+                continue
+            current_attributes.append(key)
+
+            instance = self.__dict__[key]
+            if issubclass(instance.__class__, Command) or \
+                    issubclass(instance.__class__, IndexCommand):
+                command_list[key] = (instance.__class__.__name__, instance.remote_command)
+
         return command_list
 
     def get_method_list(self, include_superclass=False):
         """
         get a list of names of methods available from the component
         including methods inherited from the superclasses
 
@@ -224,17 +240,21 @@
                     continue
                 current_attributes.append(key)
                 if callable(child):
                     method_list.append('{}'.format(key))
         return method_list
 
     def get_command_info(self, command_name):
-        if not hasattr(self.__class__, command_name):
+        if hasattr(self.__class__, command_name):
+            cmd = self.__class__.__dict__[command_name]
+        elif hasattr(self, command_name):
+            cmd = self.__dict__[command_name]
+        else:
             raise AttributeError("No command named '{}' in {}".format(command_name, self.__class__.__name__))
-        cmd = self.__class__.__dict__[command_name]
+
         if issubclass(cmd.__class__, DictCommand):
             info = (cmd.__class__.__name__, cmd.remote_command,
                     cmd.set_dict, cmd.get_dict, None)
         elif issubclass(cmd.__class__, DictIndexCommand):
             info = (cmd.__class__.__name__, cmd.remote_command,
                     cmd.set_dict, cmd.get_dict, cmd.index_dict)
         elif issubclass(cmd.__class__, IndexCommand):
@@ -254,23 +274,27 @@
 
     def assert_command_key(self, command, key):
         """
         It asserts if the component has the command as a DictCommand and DictIndexCommand, and
         the command has the key in its set_dict.
         """
 
-        if not hasattr(self.__class__, command):
+        if hasattr(self.__class__, command):
+            cmd = self.__class__.__dict__[command]
+        elif hasattr(self, command):
+            cmd = self.__dict__[command]
+        else:
             raise AttributeError("No command named '{}' in {}".format(command, self.__class__.__name__))
 
-        cmd = self.__class__.__dict__[command]
         if not issubclass(cmd.__class__, DictCommand) and not issubclass(cmd.__class__, DictIndexCommand):
             raise TypeError("'{}' is not a DictCommand or DictIndexCommand in {}"
                             .format(command, self.__class__.__name__))
         if key not in cmd.set_dict:
-            raise KeyError(f" '{key}' is in {cmd.set_dict} of command '{command}'.")
+            raise KeyError(f" '{key}' is NOT in {cmd.set_dict} of command '{command}'.")
+        return True
 
     def capture_commands(self, include_query_only=False, include_set_only=False,
                          include_excluded=False, include_methods=False, show_raw_cmds=False):
         """
         Query all commands with both set and get methods in the component
         and its subcomponents
         """
@@ -286,14 +310,91 @@
                     if not include_excluded:
                         continue
                 commands[j] = instance.capture_commands(include_query_only, include_set_only,
                                     include_excluded, include_methods, show_raw_cmds)
 
         # Capture commands from the current component
         current_attributes = []
+
+        for key in self.__dict__:  # loop through the instance
+            cmd_instance = self.__dict__[key]
+            if key in current_attributes:
+                continue
+            current_attributes.append(key)
+
+            if show_raw_cmds and \
+               (issubclass(cmd_instance.__class__, Command) or \
+                issubclass(cmd_instance.__class__, IndexCommand)):
+                k = key + f' <{cmd_instance.remote_command}>'
+            else:
+                k = key
+            if callable(cmd_instance):
+                if issubclass(cmd_instance.__class__, type):
+                    continue
+                if cmd_instance in self.exclude_capture:
+                    if include_excluded:
+                        commands[k + '() [M][EX]'] = ''
+                if include_methods and not k.startswith('_'):
+                    commands[k + '() [M]'] = ''
+                continue
+
+            if cmd_instance in self.exclude_capture:
+                if include_excluded:
+                    commands[k + ' [EX]'] = ''
+                continue
+
+            if issubclass(cmd_instance.__class__, Command):
+                if include_set_only:
+                    if cmd_instance._set_enable and not cmd_instance._get_enable:
+                        commands[k + ' [SO]'] = ''
+                        continue
+
+                if include_query_only:
+                    allowed = cmd_instance._get_enable
+                else:
+                    allowed = cmd_instance._set_enable and cmd_instance._get_enable
+                if not allowed:
+                    continue
+
+                if not cmd_instance._set_enable:
+                    name = k + ' [QO]'
+                else:
+                    name = k
+                commands[name] = cmd_instance.__get__(self, self.__class__)
+
+            elif issubclass(cmd_instance.__class__, IndexCommand):
+                if include_query_only:
+                    allowed = cmd_instance._get_enable
+                else:
+                    allowed = cmd_instance._set_enable and cmd_instance._get_enable
+                if not allowed:
+                    continue
+
+                if not cmd_instance._set_enable:
+                    name = k + ' [QO]'
+                else:
+                    name = k
+                print('Name: {}'.format(name))
+
+                commands[name] = {}
+                index = cmd_instance.index_min
+                while index <= cmd_instance.index_max:
+                    try:
+                        if cmd_instance.index_dict is None:
+                            commands[name][index] = cmd_instance.__getitem__(index)
+                        else:
+                            for key, value in cmd_instance.index_dict.items():
+                                if value == index:
+                                    commands[name][key] = cmd_instance.__getitem__(index)
+                                    break
+                        index += 1
+                    except Exception as e:
+                        print(f'  {type(e)} {e} command:{k} index: {index}')
+                        break
+
         for c in self.__class__.__mro__:  # loop through the classes including super classes
             if not issubclass(c, Component):  # it should be subclass of Component
                 break
             if c == Component:  # But it should not be Component
                 break
 
             for key in c.__dict__:
```

### Comparing `srsgui-0.3.3/srsgui/inst/exceptions.py` & `srsgui-0.4.0/srsgui/inst/exceptions.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/inst/indexcommands.py` & `srsgui-0.4.0/srsgui/inst/indexcommands.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/inst/instrument.py` & `srsgui-0.4.0/srsgui/inst/instrument.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,21 +96,25 @@
         """
         term_char = self.get_term_char()  # To retain the term char when reopening
         if self.comm.is_connected():
             self.comm.disconnect()
             time.sleep(0.1)
         if not interface_type:
             return
+        matched = False
         for interface, _ in self.available_interfaces:
             if interface_type == interface.NAME:
+                matched = True
                 self.comm = interface()
                 self.set_term_char(term_char)
                 self.comm.connect(*args)
                 self.update_components()
                 break
+        if not matched:
+            raise TypeError("Invalid interface_type: {}".format(interface_type))
 
     def disconnect(self):
         """
         Disconnect from the instrument
         """
         if self.comm.is_connected():
             self.comm.disconnect()
```

### Comparing `srsgui-0.3.3/srsgui/task/callbacks.py` & `srsgui-0.4.0/srsgui/task/callbacks.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/task/config.py` & `srsgui-0.4.0/srsgui/task/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 import os
 import logging
 from pathlib import Path
 from importlib import import_module, reload, invalidate_caches
 
 from srsgui.task.task import Task, GreenNormal, RedNormal
 
-# from srs_insts.baseinsts import BaseInst
 from srsgui.inst.instrument import Instrument
 
 logger = logging.getLogger(__name__)
 
 
 class Config(object):
     ResultDirectory = 'task-results'
     DataRootDirectory = str(Path.home() / ResultDirectory)
     LocalModulePath = ['tasks', 'instruments', 'plots']
 
     def __init__(self):
         self.inst_dict = {}
         self.task_dict = {}
         self.task_path_dict = {}
+        self.docs_dict = {}
         self.task_dict_name = 'No tasks loaded'
         self.local_db_name = None
         self.base_data_dir = self.DataRootDirectory
         p = Path(self.base_data_dir)
         if not p.exists():
             p.mkdir(parents=True)
         self.base_log_file_name = self.get_base_log_file_name()
@@ -63,15 +63,16 @@
                         k = k.strip().lower()
                         v = v.strip()
                         if k == 'task':
                             self.load_task_from_line(v)
 
                         elif k == 'inst':
                             self.load_inst_from_line(v)
-
+                        elif k == 'docs':
+                            self.load_docs_from_line(v)
                         elif k == 'name':
                             self.task_dict_name = v
                         else:
                             raise KeyError('Invalid key: {}'.format(k))
 
             logger.info('TaskConfig file "{}" loaded'.format(file_name))
 
@@ -137,15 +138,15 @@
         inst_class_name = items[2].strip()
         mod = import_module(inst_module_name)
         logger.debug('Instrument module {} for "{}" loaded'.format(mod.__file__, inst_key))
         inst_class_name = inst_class_name
 
         if hasattr(mod, inst_class_name):
             inst_class = getattr(mod, inst_class_name)
-            inst_class.__version = None
+            inst_class.__version__ = None
             if hasattr(mod, '__version__'):
                 inst_class.__version__ = getattr(mod, "__version__")
             logger.debug('Instrument class {} from "{}" loaded'.format(inst_class_name, inst_key))
         else:
             logger.error('No inst class "{}" in module "{}"'.format(inst_class_name, inst_module_name))
             return
 
@@ -160,14 +161,24 @@
             try:
                 parameter_string = items[3]
                 inst = self.inst_dict[inst_key]
                 inst.connect_with_parameter_string(parameter_string)
             except Exception as e:
                 logger.error(e)
 
+    def load_docs_from_line(self, v):
+        items = v.split(',')
+        if len(items) != 2:
+            logger.error('invalid docs line: {}'.format(v))
+            return
+
+        doc_key = items[0].strip()
+        doc_url = items[1].strip()
+        self.docs_dict[doc_key] = doc_url
+
     def get_base_log_file_name(self):
         max_file_number = 20
         return_value = None
         file_name_format = self.base_data_dir + '/mainlog-{:02d}.txt'
         for i in range(max_file_number):
             try:
                 file_name = file_name_format.format(i)
```

### Comparing `srsgui-0.3.3/srsgui/task/inputs.py` & `srsgui-0.4.0/srsgui/task/inputs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ##! 
 ##! Coptright(c) 2022, 2023 Stanford Research Systems, All right reserved
 ##! Subject to the MIT License
 ##! 
 
 """
-Interface for input variables between :class:`Task <srsgui.task.task.Task>` instance
+Interface for input parameters in  :class:`Task <srsgui.task.task.Task>` instance
 and :class:`InputPanel <srsgui.ui.inputpanel.InputPanel>` instance in GUI
 
 """
 
 
 class BaseInput:
     def __init__(self, default_value):
@@ -166,26 +166,37 @@
                 li.append(str(num))
             except:
                 raise ValueError(msg.format(octet, self.value))
         return '.'.join(li)
 
 
 class CommandInput(IntegerInput):
-    def __init__(self, cmd_name, cmd_instance, default_value=None):
-        super().__init__(default_value)
+    """
+    It provides the interface to :class:`InputPanel <srsgui.ui.inputpanel.InputPanel>`
+    to query the value of a command and to change the set value of the command.
+    Currently InputPanel does not update self.value. Do not use get_value().
+    Query the command directly in a task.
+    """
+
+    def __init__(self, cmd_name, cmd_instance=None):
+        super().__init__(None)
 
         self.inst_name = ''
         self.cmd_name = cmd_name
         self.cmd_instance = cmd_instance
         self.cmd = ''
 
     def set_inst_name(self, inst_name):
         self.inst_name = inst_name
         self.cmd = f'{self.inst_name}.{self.cmd_name}'
 
     def get_value(self):
+        """
+        Do not use. The command handler used in the InputPanel that performs command query
+        does not set the self.value.
+        """
         v = None
         if hasattr(self.cmd_instance, 'get_dict'):
             v = self.cmd_instance.key_type(self.text)
         else:
             v = self.value
         return v
```

### Comparing `srsgui-0.3.3/srsgui/task/sessionhandler.py` & `srsgui-0.4.0/srsgui/task/sessionhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/task/task.py` & `srsgui-0.4.0/srsgui/task/task.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/task/taskresult.py` & `srsgui-0.4.0/srsgui/task/taskresult.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/commandhandler.py` & `srsgui-0.4.0/srsgui/ui/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/commandterminal.py` & `srsgui-0.4.0/srsgui/ui/commandterminal.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/commandtree/commanddelegate.py` & `srsgui-0.4.0/srsgui/ui/commandtree/commanddelegate.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/commandtree/commandhandler.py` & `srsgui-0.4.0/srsgui/ui/commandtree/commandhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/commandtree/commanditem.py` & `srsgui-0.4.0/srsgui/ui/commandtree/commanditem.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,16 @@
         else:
             self.name_buffer.append(item.name)
         if item.parent():
             self.get_name_string(item.parent())
 
     @classmethod
     def load(cls, comp, parent: "CommandItem" = None) -> "CommandItem":
-        """Create a 'root' CommandItem from a Component and 
+        """
+        Create a 'root' CommandItem from a Component and
         populate its subcomponent and commands recursively.
 
         Returns:
             root_item: CommandItem
         """
         root_item = CommandItem(parent)
         root_item.name = "root"
@@ -209,14 +210,15 @@
                     child.comp = instance
                     if instance in comp.exclude_capture:
                         child.excluded = True
                     child.comp_type = type(instance)
                     root_item.appendChild(child)
 
             current_attributes = []
+
             for c in comp.__class__.__mro__:  # loop through the classes including super classes
                 if not issubclass(c, Component):  # it should be a subclass of Component
                     break
                 if c == Component:  # But it should not be Component
                     break
 
                 for key in c.__dict__:
@@ -229,32 +231,37 @@
                         child = cls.load(cmd_instance, root_item)
                         child.name = key
                         child.comp = cmd_instance
                         child.comp_type = type(cmd_instance)
 
                         root_item.appendChild(child)
 
-                    elif issubclass(cmd_instance.__class__, IndexCommand):
-                        child = cls.load(cmd_instance, root_item)
-                        child.name = key
-                        child.comp = cmd_instance
-                        child.comp_type = type(cmd_instance)
-                        root_item.appendChild(child)
-
                     elif callable(cmd_instance):
                         if issubclass(cmd_instance.__class__, type):
                             continue
                         if key.startswith('_'):
                             continue
                         
                         child = cls.load(cmd_instance, root_item)
                         child.name = key
                         child.comp = cmd_instance
                         child.comp_type = type(cmd_instance)
                         root_item.appendChild(child)
+
+            for key in comp.__dict__:  # Loop through the instance of the component
+                cmd_instance = comp.__dict__[key]
+                if key in current_attributes:
+                    continue
+                current_attributes.append(key)
+                if issubclass(cmd_instance.__class__, IndexCommand):
+                    child = cls.load(cmd_instance, root_item)
+                    child.name = key
+                    child.comp = cmd_instance
+                    child.comp_type = type(cmd_instance)
+                    root_item.appendChild(child)
         else:
             if callable(comp):
                 root_item.comp = comp
                 root_item.comp_type = type(comp)
                 root_item.excluded = comp in root_item.parent().comp.exclude_capture
                 root_item.is_method = True
```

### Comparing `srsgui-0.3.3/srsgui/ui/commandtree/commandmodel.py` & `srsgui-0.4.0/srsgui/ui/commandtree/commandmodel.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/commandtree/commandspinbox.py` & `srsgui-0.4.0/srsgui/ui/commandtree/commandspinbox.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/commandtree/commandtreeview.py` & `srsgui-0.4.0/srsgui/ui/commandtree/commandtreeview.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/commandtree/commandtreewidget.py` & `srsgui-0.4.0/srsgui/ui/commandtree/commandtreewidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.query_only_included = False
         self.set_only_included = False
         self.excluded_included = False
         self.method_included = False
         self.show_raw_command = False
 
         self.capture_time = 0.0  # time of the last capture
-        self.capture_time_limit = 5.0  # seconds before a new capture
+        self.capture_time_limit = 10.0  # seconds before a new capture
 
         self.model = CommandModel()
         self.tree_view.setItemDelegate(CommandDelegate())
         self.tree_view.setModel(self.model)
 
         self.expand_button.hide()
```

### Comparing `srsgui-0.3.3/srsgui/ui/commandtree/ui_commandtreewidget.py` & `srsgui-0.4.0/srsgui/ui/commandtree/ui_commandtreewidget.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/connectdlg.py` & `srsgui-0.4.0/srsgui/ui/connectdlg.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/deviceinfohandler.py` & `srsgui-0.4.0/srsgui/ui/deviceinfohandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/dockhandler.py` & `srsgui-0.4.0/srsgui/ui/dockhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/inputpanel.py` & `srsgui-0.4.0/srsgui/ui/inputpanel.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import math
 from .qt.QtCore import Qt
 from .qt.QtWidgets import QWidget, QDoubleSpinBox, QSpinBox, QComboBox, \
                           QLineEdit, QLabel, QGridLayout, QPushButton, QScrollArea
 
 from srsgui.inst.commands import Command, IntCommand, FloatCommand, DictCommand
-from srsgui.inst.indexcommands import IntIndexCommand, FloatIndexCommand, DictIndexCommand
+from srsgui.inst.indexcommands import IndexCommand, IntIndexCommand, FloatIndexCommand, DictIndexCommand
 
 from srsgui.task.task import Task
 from srsgui.task.inputs import IntegerInput, FloatInput, StringInput, \
                                ListInput, InstrumentInput, CommandInput
 
 import logging
 logger = logging.getLogger(__name__)
@@ -92,14 +92,15 @@
                         raise ValueError('CommandInput defined "{}" before any instrumentInput'
                                          .format(p.cmd_name))
 
                     if not self.inst_dict[self.inst_name].is_connected:
                         raise ValueError('{} is not connected'.format(self.inst_name))
 
                     p.set_inst_name(self.inst_name)
+                    p.cmd_instance = self.get_cmd_instance(p)
                     if issubclass(p.cmd_instance.__class__, IntCommand) or \
                        issubclass(p.cmd_instance.__class__, IntIndexCommand):
                         widget = QSpinBox()
                         widget.setSuffix(' ' + p.cmd_instance.unit)
                         widget.setMaximum(p.cmd_instance.maximum)
                         widget.setMinimum(p.cmd_instance.minimum)
                         widget.setSingleStep(p.cmd_instance.step)
@@ -214,16 +215,18 @@
                     if type(params[name]) == CommandInput:
                         cmd = '{} = "{}"'.format(params[name].cmd, params[name].default_value)
                 elif type(widget) == QComboBox and type(params[name].default_value) == int:
                     params[name].value = params[name].default_value
                     widget.setCurrentIndex(params[name].default_value)
                     params[name].text = widget.currentText()
                     if type(params[name]) == CommandInput:
-                        if hasattr(params[name].cmd_instance, 'key_type') and \
-                           getattr(params[name].cmd_instance, 'key_type') == 'int':
+                        p = params[name]
+                        p.cmd_instance = self.get_cmd_instance(p)
+                        if hasattr(p.cmd_instance, 'key_type') and \
+                           getattr(p.cmd_instance, 'key_type') == 'int':
                             cmd = '{} = {}'.format(params[name].cmd, params[name].default_value)
                         else:
                             cmd = '{} = "{}"'.format(params[name].cmd, params[name].text)
                 elif type(widget) == QSpinBox and type(params[name].default_value) == int:
                     params[name].value = params[name].default_value
                     widget.setValue(params[name].default_value)
                     if type(params[name]) == CommandInput:
@@ -253,16 +256,18 @@
                     if type(params[name]) == CommandInput:
                         cmd = '{} = "{}"'.format(params[name].cmd, widget.text())
 
                 elif type(widget) == QComboBox:
                     params[name].value = widget.currentIndex()
                     params[name].text = widget.currentText()
                     if type(params[name]) == CommandInput:
-                        if hasattr(params[name].cmd_instance, 'key_type') and \
-                           getattr(params[name].cmd_instance, 'key_type') is str:
+                        p = params[name]
+                        p.cmd_instance = self.get_cmd_instance(p)
+                        if hasattr(p.cmd_instance, 'key_type') and \
+                           getattr(p.cmd_instance, 'key_type') is str:
                             fmt = '{} = "{}"'
                         else:
                             fmt = '{} = {}'
                         cmd = fmt.format(params[name].cmd, widget.currentText())
 
                 elif type(widget) in (QSpinBox, QDoubleSpinBox):
                     params[name].value = widget.value()
@@ -287,13 +292,38 @@
 
                 elif type(self.command_dict[cmd]) == QComboBox:
                     index = self.command_dict[cmd].findText(reply)
                     self.command_dict[cmd].setCurrentIndex(index)
 
                 elif type(self.command_dict[cmd]) == QLineEdit:
                     self.command_dict[cmd].setText(reply)
-
                 else:
                     logger.error('Unhandled Command: {}'.format(cmd))
 
         except Exception as e:
             logger.error(e)
+
+    def get_cmd_instance(self, cmd_input):
+        """
+        Find the command instance in CommandInput from cmd_name
+        """
+
+        found = False
+        new_comp = self.inst_dict[cmd_input.inst_name]
+        if not new_comp.is_connected():
+            raise IOError('Instrument not connected')
+
+        comp_names = cmd_input.cmd_name.split('.')
+        for c in comp_names:
+            name = c.split('[')[0]  # Do not include '[]'
+            try:
+                new_comp = getattr(new_comp.__class__, name)
+            except AttributeError:
+                new_comp = getattr(new_comp, name)
+
+            if issubclass(type(new_comp), (Command, IndexCommand)):
+                found = True
+                break
+        if not found:
+            raise TypeError('get_cmd_instance: No Command instance found')
+
+        return new_comp
```

### Comparing `srsgui-0.3.3/srsgui/ui/qt/QtCore.py` & `srsgui-0.4.0/srsgui/ui/qt/QtCore.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/qt/QtGui.py` & `srsgui-0.4.0/srsgui/ui/qt/QtGui.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/qt/QtWidgets.py` & `srsgui-0.4.0/srsgui/ui/qt/QtWidgets.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/qt/__init__.py` & `srsgui-0.4.0/srsgui/ui/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/qtloghandler.py` & `srsgui-0.4.0/srsgui/ui/qtloghandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/resource_rc.py` & `srsgui-0.4.0/srsgui/ui/resource_rc.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/signalhandler.py` & `srsgui-0.4.0/srsgui/ui/signalhandler.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/srslogo.jpg` & `srsgui-0.4.0/srsgui/ui/srslogo.jpg`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/stdout.py` & `srsgui-0.4.0/srsgui/ui/stdout.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/taskmain.py` & `srsgui-0.4.0/srsgui/ui/taskmain.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 import sys
 
 import logging
 import logging.handlers
 
 from pathlib import Path
+import webbrowser
 
 from .qt import QT_BINDER, PYSIDE6, QT_BINDER_VERSION
 from .qt.QtCore import QTimer, QSettings
 from .qt.QtWidgets import QMainWindow, QApplication, QTextBrowser,\
                                 QVBoxLayout, QMessageBox, \
                                 QInputDialog, QFileDialog, \
                                 QMenu, QAction
@@ -50,14 +51,17 @@
 
     OrganizationName = 'srsinst'
     ApplicationName = 'srsgui'
 
     LogoImageFile = 'srslogo.jpg'
     LogoFile = str(Path(__file__).parent / LogoImageFile)
 
+    DocsSuffix = ' documentation'
+    TextAbout = 'About'
+
     def __init__(self, parent=None):
         super(TaskMain, self).__init__(parent)
         self.setupUi(self)
         # self.taskResult.setFontFamily('monospace')
 
         QApplication.setOrganizationName(self.OrganizationName)
         QApplication.setApplicationName(self.ApplicationName)
@@ -71,14 +75,15 @@
         self.task_method = None
 
         self.question_result = None
         self.question_result_value = None
 
         # data_dict hold data shared among task. It will inject to a task when run
         self.data_dict = {}
+        self.docs_dict = {}
 
         # self.inst_dict holds instances of subclass of Instrument
         self.inst_dict = {}
         self.inst_info_handler = DeviceInfoHandler(self)
 
         self.dock_handler = DockHandler(self)
         self.command_handler = self.dock_handler.terminal_command_handler
@@ -135,21 +140,17 @@
         self.default_config_file = self.settings.value("ConfigFile", "", type=str)
         if not self.default_config_file:
             self.default_config_file = default_config_file
 
         self.statusbar.showMessage('Waiting for task selection')
         self.stdout = StdOut(self.print_redirect)
 
-        self.about = QAction(self)
-        self.about.setText('About')
-        self.menu_Help.addAction(self.about)
-        self.about.triggered.connect(self.onAbout)
-
         self.menu_Tasks.triggered.connect(self.onTaskSelect)
         self.menu_Instruments.triggered.connect(self.onInstrumentSelect)
+        self.menu_Help.triggered.connect(self.onHelp)
 
     def load_tasks(self):
         """
         Load configuration info from a .taskconfig file specified from
             #. Command line argument
             #. Settings saved in the registry
             #. Application default .taskconfig file
@@ -187,42 +188,56 @@
             logger.debug('Set the current directory to "{}"'.format(current_dir))
             self.config.load(self.default_config_file)
             logger.debug('TaskConfig file: "{}"  loading done'.format(self.default_config_file))
 
             for instr in prev_inst_dict:
                 del instr
             self.inst_dict = self.config.inst_dict
+            self.task_dict = self.config.task_dict
+            self.docs_dict = self.config.docs_dict
 
             self.dock_handler.reset_inst_docks()
 
             self.inst_info_handler.update_tabs()
             for inst_name in self.inst_dict:
                 self.inst_info_handler.update_info(inst_name)
 
-            self.task_dict = self.config.task_dict
-
             self.setWindowTitle(self.config.task_dict_name)
             self.dock_handler.display_image(self.get_logo_file())
 
             self.session_handler = SessionHandler(True, False, False)
             self.session_handler.set_data_directory(self.config.base_data_dir, self.config.task_dict_name)
             self.session_handler.open_session(0, False)
 
         except Exception as e:
             logger.error('{}: {}'.format(e.__class__.__name__, e))
 
         try:
+            actions = self.menu_Help.actions()
+            for action in actions:
+                self.menu_Help.removeAction(action)
+
+            action_about = QAction(self)
+            action_about.setText(self.TextAbout)
+            self.menu_Help.addAction(action_about)
+
+            for item in self.docs_dict:
+                action_docs = QAction(self)
+                action_docs.setText(item + self.DocsSuffix)
+                self.menu_Help.addAction(action_docs)
+
             actions = self.menu_Instruments.actions()
             for action in actions:
                 self.menu_Instruments.removeAction(action)
             for item in self.inst_dict:
                 action_inst = QAction(self)
                 action_inst.setText(item)
                 self.menu_Instruments.addAction(action_inst)
             logger.debug('Added new actions to Instruments menu')
+
             # Remove previous actions from Task menu
             actions = self.menu_Tasks.actions()
             for action in actions:
                 self.menu_Tasks.removeAction(action)
 
             # Add new actions to Task menu
             for name in self.task_dict:
@@ -602,15 +617,27 @@
                 if i_file:
                     image_file = i_file
             self.dock_handler.display_image(image_file)
             return
         except Exception as e:
             logger.error(f"Error in handle_initial_image: {e}")
 
-    def onAbout(self,checked):
+    def onHelp(self, help_action):
+        try:
+            name = help_action.text()
+            if name == self.TextAbout:
+                self.onAbout()
+            else:
+                name = name[:-len(self.DocsSuffix)]
+                if name in self.docs_dict:
+                    webbrowser.open(self.docs_dict[name])
+        except Exception as e:
+            logger.error(e)
+
+    def onAbout(self):
         msg = ''
         for name in self.inst_dict:
             inst = self.inst_dict[name]
             if hasattr(inst, "__version__"):
                 version = inst.__version__
             else:
                 version = 'N/A'
```

### Comparing `srsgui-0.3.3/srsgui/ui/taskmain.ui` & `srsgui-0.4.0/srsgui/ui/taskmain.ui`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui/ui/ui_taskmain.py` & `srsgui-0.4.0/srsgui/ui/ui_taskmain.py`

 * *Files identical despite different names*

### Comparing `srsgui-0.3.3/srsgui.egg-info/PKG-INFO` & `srsgui-0.4.0/srsgui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srsgui
-Version: 0.3.3
+Version: 0.4.0
 Summary: Framework to run instrument-controlling Python scripts in GUI
 Author: Chulhoon Kim
 License: MIT license
 Project-URL: homepage, https://github.com/thinkSRS/srsgui
 Project-URL: repository, https://github.com/thinkSRS/srsgui.git
 Project-URL: documentation, https://thinksrs.github.io/srsgui
 Project-URL: changelog, https://thinksrs.github.io/srsgui/changelog.html
```

### Comparing `srsgui-0.3.3/srsgui.egg-info/SOURCES.txt` & `srsgui-0.4.0/srsgui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

