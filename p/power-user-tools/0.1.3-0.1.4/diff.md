# Comparing `tmp/power-user-tools-0.1.3.tar.gz` & `tmp/power-user-tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "power-user-tools-0.1.3.tar", last modified: Tue Jun 20 11:07:22 2023, max compression
+gzip compressed data, was "power-user-tools-0.1.4.tar", last modified: Fri Jun 23 09:51:47 2023, max compression
```

## Comparing `power-user-tools-0.1.3.tar` & `power-user-tools-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-06-20 11:07:22.821775 power-user-tools-0.1.3/
--rw-r--r--   0 davmeyer   (503) staff       (20)     1095 2022-11-24 13:41:28.000000 power-user-tools-0.1.3/LICENSE
--rw-r--r--   0 davmeyer   (503) staff       (20)      576 2023-06-20 11:07:22.821965 power-user-tools-0.1.3/PKG-INFO
--rw-r--r--   0 davmeyer   (503) staff       (20)      546 2023-06-06 07:35:46.000000 power-user-tools-0.1.3/README.md
-drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-06-20 11:07:22.810014 power-user-tools-0.1.3/commands/
--rw-r--r--   0 davmeyer   (503) staff       (20)        0 2022-11-24 15:12:46.000000 power-user-tools-0.1.3/commands/__init__.py
--rwxr-xr-x   0 davmeyer   (503) staff       (20)     1291 2023-06-05 13:36:27.000000 power-user-tools-0.1.3/commands/devutils.py
--rwxr-xr-x   0 davmeyer   (503) staff       (20)     6468 2023-06-20 11:05:53.000000 power-user-tools-0.1.3/commands/dockertools.py
--rw-r--r--   0 davmeyer   (503) staff       (20)     4158 2023-06-05 13:37:33.000000 power-user-tools-0.1.3/commands/helpers.py
--rwxr-xr-x   0 davmeyer   (503) staff       (20)     2101 2023-06-05 13:42:55.000000 power-user-tools-0.1.3/commands/sshutils.py
-drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-06-20 11:07:22.812578 power-user-tools-0.1.3/power_user_tools.egg-info/
--rw-r--r--   0 davmeyer   (503) staff       (20)      576 2023-06-20 11:07:22.000000 power-user-tools-0.1.3/power_user_tools.egg-info/PKG-INFO
--rw-r--r--   0 davmeyer   (503) staff       (20)      572 2023-06-20 11:07:22.000000 power-user-tools-0.1.3/power_user_tools.egg-info/SOURCES.txt
--rw-r--r--   0 davmeyer   (503) staff       (20)        1 2023-06-20 11:07:22.000000 power-user-tools-0.1.3/power_user_tools.egg-info/dependency_links.txt
--rw-r--r--   0 davmeyer   (503) staff       (20)      356 2023-06-20 11:07:22.000000 power-user-tools-0.1.3/power_user_tools.egg-info/entry_points.txt
--rw-r--r--   0 davmeyer   (503) staff       (20)        1 2023-06-20 11:07:22.000000 power-user-tools-0.1.3/power_user_tools.egg-info/not-zip-safe
--rw-r--r--   0 davmeyer   (503) staff       (20)       93 2023-06-20 11:07:22.000000 power-user-tools-0.1.3/power_user_tools.egg-info/requires.txt
--rw-r--r--   0 davmeyer   (503) staff       (20)        9 2023-06-20 11:07:22.000000 power-user-tools-0.1.3/power_user_tools.egg-info/top_level.txt
--rw-r--r--   0 davmeyer   (503) staff       (20)      152 2023-06-20 11:07:22.822638 power-user-tools-0.1.3/setup.cfg
--rw-r--r--   0 davmeyer   (503) staff       (20)     1807 2023-06-20 11:06:54.000000 power-user-tools-0.1.3/setup.py
-drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-06-20 11:07:22.821150 power-user-tools-0.1.3/shell/
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      521 2020-12-23 09:23:36.000000 power-user-tools-0.1.3/shell/dtimg
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      645 2020-02-11 08:02:45.000000 power-user-tools-0.1.3/shell/dtip
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      426 2020-02-11 08:02:45.000000 power-user-tools-0.1.3/shell/dtnet
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      200 2020-10-13 14:08:48.000000 power-user-tools-0.1.3/shell/dtports
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      239 2020-11-17 08:09:21.000000 power-user-tools-0.1.3/shell/dtrestart
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      492 2021-01-15 06:06:32.000000 power-user-tools-0.1.3/shell/dtrm
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      235 2020-02-11 08:02:45.000000 power-user-tools-0.1.3/shell/dtstart
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      233 2020-02-11 08:02:45.000000 power-user-tools-0.1.3/shell/dtstop
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      416 2022-11-25 14:27:10.000000 power-user-tools-0.1.3/shell/xpgrmhistory
--rwxr-xr-x   0 davmeyer   (503) staff       (20)      502 2022-11-25 14:27:10.000000 power-user-tools-0.1.3/shell/xppr
--rwxr-xr-x   0 davmeyer   (503) staff       (20)       55 2022-11-25 14:27:10.000000 power-user-tools-0.1.3/shell/xprandpw
+drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-06-23 09:51:47.728786 power-user-tools-0.1.4/
+-rw-r--r--   0 davmeyer   (503) staff       (20)     1095 2022-11-24 13:41:28.000000 power-user-tools-0.1.4/LICENSE
+-rw-r--r--   0 davmeyer   (503) staff       (20)      576 2023-06-23 09:51:47.728930 power-user-tools-0.1.4/PKG-INFO
+-rw-r--r--   0 davmeyer   (503) staff       (20)      546 2023-06-06 07:35:46.000000 power-user-tools-0.1.4/README.md
+drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-06-23 09:51:47.716959 power-user-tools-0.1.4/commands/
+-rw-r--r--   0 davmeyer   (503) staff       (20)        0 2022-11-24 15:12:46.000000 power-user-tools-0.1.4/commands/__init__.py
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)     1291 2023-06-05 13:36:27.000000 power-user-tools-0.1.4/commands/devutils.py
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)     7239 2023-06-23 09:50:41.000000 power-user-tools-0.1.4/commands/dockertools.py
+-rw-r--r--   0 davmeyer   (503) staff       (20)     4158 2023-06-05 13:37:33.000000 power-user-tools-0.1.4/commands/helpers.py
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)     2101 2023-06-05 13:42:55.000000 power-user-tools-0.1.4/commands/sshutils.py
+drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-06-23 09:51:47.720462 power-user-tools-0.1.4/power_user_tools.egg-info/
+-rw-r--r--   0 davmeyer   (503) staff       (20)      576 2023-06-23 09:51:47.000000 power-user-tools-0.1.4/power_user_tools.egg-info/PKG-INFO
+-rw-r--r--   0 davmeyer   (503) staff       (20)      572 2023-06-23 09:51:47.000000 power-user-tools-0.1.4/power_user_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 davmeyer   (503) staff       (20)        1 2023-06-23 09:51:47.000000 power-user-tools-0.1.4/power_user_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 davmeyer   (503) staff       (20)      393 2023-06-23 09:51:47.000000 power-user-tools-0.1.4/power_user_tools.egg-info/entry_points.txt
+-rw-r--r--   0 davmeyer   (503) staff       (20)        1 2023-06-23 09:51:47.000000 power-user-tools-0.1.4/power_user_tools.egg-info/not-zip-safe
+-rw-r--r--   0 davmeyer   (503) staff       (20)       93 2023-06-23 09:51:47.000000 power-user-tools-0.1.4/power_user_tools.egg-info/requires.txt
+-rw-r--r--   0 davmeyer   (503) staff       (20)        9 2023-06-23 09:51:47.000000 power-user-tools-0.1.4/power_user_tools.egg-info/top_level.txt
+-rw-r--r--   0 davmeyer   (503) staff       (20)      152 2023-06-23 09:51:47.729411 power-user-tools-0.1.4/setup.cfg
+-rw-r--r--   0 davmeyer   (503) staff       (20)     1859 2023-06-23 09:26:04.000000 power-user-tools-0.1.4/setup.py
+drwxr-xr-x   0 davmeyer   (503) staff       (20)        0 2023-06-23 09:51:47.728307 power-user-tools-0.1.4/shell/
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      521 2020-12-23 09:23:36.000000 power-user-tools-0.1.4/shell/dtimg
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      645 2020-02-11 08:02:45.000000 power-user-tools-0.1.4/shell/dtip
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      426 2020-02-11 08:02:45.000000 power-user-tools-0.1.4/shell/dtnet
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      200 2020-10-13 14:08:48.000000 power-user-tools-0.1.4/shell/dtports
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      239 2020-11-17 08:09:21.000000 power-user-tools-0.1.4/shell/dtrestart
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      492 2021-01-15 06:06:32.000000 power-user-tools-0.1.4/shell/dtrm
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      235 2020-02-11 08:02:45.000000 power-user-tools-0.1.4/shell/dtstart
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      233 2020-02-11 08:02:45.000000 power-user-tools-0.1.4/shell/dtstop
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      416 2022-11-25 14:27:10.000000 power-user-tools-0.1.4/shell/xpgrmhistory
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)      502 2022-11-25 14:27:10.000000 power-user-tools-0.1.4/shell/xppr
+-rwxr-xr-x   0 davmeyer   (503) staff       (20)       55 2022-11-25 14:27:10.000000 power-user-tools-0.1.4/shell/xprandpw
```

### Comparing `power-user-tools-0.1.3/LICENSE` & `power-user-tools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `power-user-tools-0.1.3/PKG-INFO` & `power-user-tools-0.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-user-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Power User Tools make your life so much easier
 Home-page: https://github.com/dameyerdave/power-user-tools
 Author: dameyerdave
 Author-email: dameyerdave@gmail.com
 License: MIT
 Keywords: power user tools ssh sshd reverse tunnel docker easy development
 Classifier: Programming Language :: Python :: 3
```

### Comparing `power-user-tools-0.1.3/README.md` & `power-user-tools-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `power-user-tools-0.1.3/commands/devutils.py` & `power-user-tools-0.1.4/commands/devutils.py`

 * *Files identical despite different names*

### Comparing `power-user-tools-0.1.3/commands/dockertools.py` & `power-user-tools-0.1.4/commands/dockertools.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Tools to manage Docker.
 """
 
 import os
 import sys
 import click
 import sh
+import json
 from commands.helpers import Executor as E, Message as M, TableOutput as T
 from os.path import isfile, isdir
 from dotenv import load_dotenv
 import traceback
 
 # declare the commands globally
 bash = sh.Command("bash")
@@ -134,28 +135,46 @@
 
 @click.command()
 @click.argument("filter", required=False)
 def dtins(filter: str = None):
     rows = []
     args = ["ps", "-a", "--format", "{{.Names}}"]
     if filter:
-        args.append("--filter ")
+        args.append("--filter")
         args.append(f"name={filter}")
     for container in docker(*args, _iter=True):
         container = container.rstrip("\n")
         insp = docker(
             "inspect",
             "-f",
             "{{ .State.Status }}#{{ .HostConfig.RestartPolicy.Name }}",
             container,
         )
-        rows.append(f"{container}#{insp}")
+        rows.append(f"{container}#{insp.rstrip()}")
     T.out(rows, headers=("Name", "Status", "Restart"))
 
 
+@click.command()
+@click.argument("filter", required=False)
+def dtvols(filter: str = None):
+    list_args = ["volume", "list", "--format", "{{ .Name }}"]
+    if filter:
+        list_args.append("--filter")
+        list_args.append(f"name={filter}")
+    vols = docker(*list_args).split("\n")[:-1]
+    rows = []
+    for vol in vols:
+        args = ["volume", "inspect"]
+        insp = json.loads(docker(*args, vol).stdout)[0]
+        rows.append(
+            f"{insp['Name']}#{insp['CreatedAt']}#{insp['Mountpoint']}#{insp['Labels']['com.docker.compose.project'] if 'Labels' in insp and insp['Labels'] and 'com.docker.compose.project' in insp['Labels'] else 'Unknown'}"
+        )
+    T.out(rows, headers=("Name", "CreatedAt", "Mountpoint", "Project"))
+
+
 def __get_container_name(pattern):
     containers = E.run('docker ps -a --format "{{.Names}}"').split("\n")
     found_containers = []
     for container in containers:
         if pattern in container:
             found_containers.append(container)
     if len(found_containers) == 1:
```

### Comparing `power-user-tools-0.1.3/commands/helpers.py` & `power-user-tools-0.1.4/commands/helpers.py`

 * *Files identical despite different names*

### Comparing `power-user-tools-0.1.3/commands/sshutils.py` & `power-user-tools-0.1.4/commands/sshutils.py`

 * *Files identical despite different names*

### Comparing `power-user-tools-0.1.3/power_user_tools.egg-info/PKG-INFO` & `power-user-tools-0.1.4/power_user_tools.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: power-user-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Power User Tools make your life so much easier
 Home-page: https://github.com/dameyerdave/power-user-tools
 Author: dameyerdave
 Author-email: dameyerdave@gmail.com
 License: MIT
 Keywords: power user tools ssh sshd reverse tunnel docker easy development
 Classifier: Programming Language :: Python :: 3
```

### Comparing `power-user-tools-0.1.3/power_user_tools.egg-info/SOURCES.txt` & `power-user-tools-0.1.4/power_user_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `power-user-tools-0.1.3/setup.py` & `power-user-tools-0.1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 long_description = "Power User Tools make your life so much easier."
 
 setup(
     name="power-user-tools",
-    version="0.1.3",
+    version="0.1.4",
     author="dameyerdave",
     author_email="dameyerdave@gmail.com",
     url="https://github.com/dameyerdave/power-user-tools",
     description="Power User Tools make your life so much easier",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
@@ -20,14 +20,15 @@
             "sumount = commands.sshutils:sumount",
             "dcc = commands.dockertools:dcc",
             "dtls = commands.dockertools:dtls",
             "dtail = commands.dockertools:dtail",
             "dtsh = commands.dockertools:dtsh",
             "dtclean = commands.dockertools:dtclean",
             "dtins = commands.dockertools:dtins",
+            "dtvols = commands.dockertools:dtvols",
             "xpgl = commands.devutils:xpgl",
         ]
     },
     scripts=[
         "shell/dtip",
         "shell/dtports",
         "shell/dtnet",
```

### Comparing `power-user-tools-0.1.3/shell/dtimg` & `power-user-tools-0.1.4/shell/dtimg`

 * *Files identical despite different names*

### Comparing `power-user-tools-0.1.3/shell/dtip` & `power-user-tools-0.1.4/shell/dtip`

 * *Files identical despite different names*

