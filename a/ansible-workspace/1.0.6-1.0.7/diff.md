# Comparing `tmp/ansible_workspace-1.0.6.tar.gz` & `tmp/ansible_workspace-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible_workspace-1.0.6.tar", last modified: Fri Jun 23 10:11:02 2023, max compression
+gzip compressed data, was "ansible_workspace-1.0.7.tar", last modified: Fri Jun 23 10:11:50 2023, max compression
```

## Comparing `ansible_workspace-1.0.6.tar` & `ansible_workspace-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:11:02.671176 ansible_workspace-1.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-23 10:10:56.000000 ansible_workspace-1.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-23 10:11:02.671176 ansible_workspace-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-23 10:10:56.000000 ansible_workspace-1.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:11:02.671176 ansible_workspace-1.0.6/ansible_workspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:10:56.000000 ansible_workspace-1.0.6/ansible_workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-23 10:10:56.000000 ansible_workspace-1.0.6/ansible_workspace/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-23 10:10:56.000000 ansible_workspace-1.0.6/ansible_workspace/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-23 10:10:56.000000 ansible_workspace-1.0.6/ansible_workspace/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-23 10:10:56.000000 ansible_workspace-1.0.6/ansible_workspace/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-23 10:10:56.000000 ansible_workspace-1.0.6/ansible_workspace/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-23 10:10:56.000000 ansible_workspace-1.0.6/ansible_workspace/output.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-23 10:10:56.000000 ansible_workspace-1.0.6/ansible_workspace/tmuxp.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-23 10:10:56.000000 ansible_workspace-1.0.6/ansible_workspace/vscode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:11:02.671176 ansible_workspace-1.0.6/ansible_workspace.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-23 10:11:02.000000 ansible_workspace-1.0.6/ansible_workspace.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-23 10:11:02.000000 ansible_workspace-1.0.6/ansible_workspace.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:11:02.000000 ansible_workspace-1.0.6/ansible_workspace.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 10:11:02.000000 ansible_workspace-1.0.6/ansible_workspace.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:11:02.000000 ansible_workspace-1.0.6/ansible_workspace.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 10:11:02.000000 ansible_workspace-1.0.6/ansible_workspace.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:11:02.671176 ansible_workspace-1.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-23 10:10:56.000000 ansible_workspace-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:11:50.491502 ansible_workspace-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-23 10:11:43.000000 ansible_workspace-1.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-23 10:11:50.491502 ansible_workspace-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-23 10:11:43.000000 ansible_workspace-1.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:11:50.491502 ansible_workspace-1.0.7/ansible_workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 10:11:43.000000 ansible_workspace-1.0.7/ansible_workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-23 10:11:43.000000 ansible_workspace-1.0.7/ansible_workspace/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-23 10:11:43.000000 ansible_workspace-1.0.7/ansible_workspace/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-23 10:11:43.000000 ansible_workspace-1.0.7/ansible_workspace/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-23 10:11:43.000000 ansible_workspace-1.0.7/ansible_workspace/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-23 10:11:43.000000 ansible_workspace-1.0.7/ansible_workspace/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-23 10:11:43.000000 ansible_workspace-1.0.7/ansible_workspace/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-23 10:11:43.000000 ansible_workspace-1.0.7/ansible_workspace/tmuxp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-23 10:11:43.000000 ansible_workspace-1.0.7/ansible_workspace/vscode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 10:11:50.491502 ansible_workspace-1.0.7/ansible_workspace.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-23 10:11:50.000000 ansible_workspace-1.0.7/ansible_workspace.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-23 10:11:50.000000 ansible_workspace-1.0.7/ansible_workspace.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 10:11:50.000000 ansible_workspace-1.0.7/ansible_workspace.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 10:11:50.000000 ansible_workspace-1.0.7/ansible_workspace.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:11:50.000000 ansible_workspace-1.0.7/ansible_workspace.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-23 10:11:50.000000 ansible_workspace-1.0.7/ansible_workspace.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 10:11:50.491502 ansible_workspace-1.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-06-23 10:11:43.000000 ansible_workspace-1.0.7/setup.py
```

### Comparing `ansible_workspace-1.0.6/LICENSE` & `ansible_workspace-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible_workspace-1.0.6/PKG-INFO` & `ansible_workspace-1.0.7/ansible_workspace.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ansible_workspace
-Version: 1.0.6
+Name: ansible-workspace
+Version: 1.0.7
 Summary: Create a workspace for multiple tools to easier develop ansible playbooks with roles.
 Home-page: https://github.com/rwxd/ansible_workspace
 Author: rwxd
 Author-email: rwxd@pm.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansible_workspace-1.0.6/README.md` & `ansible_workspace-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ansible_workspace-1.0.6/ansible_workspace/cli.py` & `ansible_workspace-1.0.7/ansible_workspace/cli.py`

 * *Files identical despite different names*

### Comparing `ansible_workspace-1.0.6/ansible_workspace/git.py` & `ansible_workspace-1.0.7/ansible_workspace/git.py`

 * *Files identical despite different names*

### Comparing `ansible_workspace-1.0.6/ansible_workspace/misc.py` & `ansible_workspace-1.0.7/ansible_workspace/misc.py`

 * *Files identical despite different names*

### Comparing `ansible_workspace-1.0.6/ansible_workspace.egg-info/PKG-INFO` & `ansible_workspace-1.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ansible-workspace
-Version: 1.0.6
+Name: ansible_workspace
+Version: 1.0.7
 Summary: Create a workspace for multiple tools to easier develop ansible playbooks with roles.
 Home-page: https://github.com/rwxd/ansible_workspace
 Author: rwxd
 Author-email: rwxd@pm.me
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ansible_workspace-1.0.6/ansible_workspace.egg-info/SOURCES.txt` & `ansible_workspace-1.0.7/ansible_workspace.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible_workspace-1.0.6/setup.py` & `ansible_workspace-1.0.7/setup.py`

 * *Files identical despite different names*

