# Comparing `tmp/kangtools-0.0.1.tar.gz` & `tmp/kangtools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kangtools-0.0.1.tar", last modified: Fri Jun 23 19:26:55 2023, max compression
+gzip compressed data, was "kangtools-0.0.3.tar", last modified: Fri Jun 23 19:36:15 2023, max compression
```

## Comparing `kangtools-0.0.1.tar` & `kangtools-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-23 19:26:55.081010 kangtools-0.0.1/
--rw-r--r--   0 kang       (501) staff       (20)      288 2023-06-23 19:26:55.080879 kangtools-0.0.1/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)       72 2023-06-23 19:19:31.000000 kangtools-0.0.1/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-23 19:26:55.080186 kangtools-0.0.1/kangtools/
--rw-r--r--   0 kang       (501) staff       (20)       49 2023-06-23 19:23:54.000000 kangtools-0.0.1/kangtools/__init__.py
--rw-r--r--   0 kang       (501) staff       (20)     1277 2023-06-23 19:22:58.000000 kangtools-0.0.1/kangtools/version_control.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-23 19:26:55.080724 kangtools-0.0.1/kangtools.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)      288 2023-06-23 19:26:55.000000 kangtools-0.0.1/kangtools.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      201 2023-06-23 19:26:55.000000 kangtools-0.0.1/kangtools.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-23 19:26:55.000000 kangtools-0.0.1/kangtools.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)       10 2023-06-23 19:26:55.000000 kangtools-0.0.1/kangtools.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-23 19:26:55.081048 kangtools-0.0.1/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      658 2023-06-23 19:26:06.000000 kangtools-0.0.1/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-23 19:36:15.884848 kangtools-0.0.3/
+-rw-r--r--   0 kang       (501) staff       (20)     4408 2023-06-23 19:36:15.884735 kangtools-0.0.3/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)     4193 2023-06-23 19:34:01.000000 kangtools-0.0.3/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-23 19:36:15.883976 kangtools-0.0.3/kangtools/
+-rw-r--r--   0 kang       (501) staff       (20)       49 2023-06-23 19:23:54.000000 kangtools-0.0.3/kangtools/__init__.py
+-rwxr-xr-x   0 kang       (501) staff       (20)     1478 2023-06-23 19:31:19.000000 kangtools-0.0.3/kangtools/version_control.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-23 19:36:15.884579 kangtools-0.0.3/kangtools.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)     4408 2023-06-23 19:36:15.000000 kangtools-0.0.3/kangtools.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      237 2023-06-23 19:36:15.000000 kangtools-0.0.3/kangtools.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-23 19:36:15.000000 kangtools-0.0.3/kangtools.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)       77 2023-06-23 19:36:15.000000 kangtools-0.0.3/kangtools.egg-info/entry_points.txt
+-rw-r--r--   0 kang       (501) staff       (20)       10 2023-06-23 19:36:15.000000 kangtools-0.0.3/kangtools.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-23 19:36:15.884887 kangtools-0.0.3/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      780 2023-06-23 19:36:00.000000 kangtools-0.0.3/setup.py
```

### Comparing `kangtools-0.0.1/kangtools/version_control.py` & `kangtools-0.0.3/kangtools/version_control.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,41 +1,49 @@
+#!/usr/bin/env python3
+
 import os
 import re
 
-version_file_path = "version.txt"
-commit_message = input("Enter commit message: ")
 
-# Check if version.txt exists, create it if it doesn't
-if not os.path.exists(version_file_path):
-    with open(version_file_path, 'w') as f:
-        f.write("V.0.1\n")
-
-# Read previous version and commit history
-with open(version_file_path, 'r') as f:
-    content = f.readlines()
-    # Initialize version as default
-    version = "V.0.1"
-    # Start from the last line and move upwards
-    for line in reversed(content):
-        # If this line looks like a version number, use it and stop
-        if line.strip().startswith("V.0."):
-            version = line.strip()
-            break
-
-# Extract version number
-version_number = int(re.search(r'\d+(?=\s|$)', version).group())
-# version_number = int(re.search(r'\d+$', version).group())
-
-# Increment version number
-new_version_number = version_number + 1
-
-# Update version file
-with open(version_file_path, 'a') as f:
-    # f.write(f"V.0.{new_version_number}\n")
-    f.write(f"V.0.{new_version_number} - {commit_message}\n")
-
-# Execute git commands
-os.system("git add -A")
-os.system(f'git commit -m "V.0.{new_version_number} - {commit_message}"')
-os.system("git push")
+def main():
+    version_file_path = "version.txt"
+    commit_message = input("Enter commit message: ")
+
+    # Check if version.txt exists, create it if it doesn't
+    if not os.path.exists(version_file_path):
+        with open(version_file_path, 'w') as f:
+            f.write("V.0.1\n")
+
+    # Read previous version and commit history
+    with open(version_file_path, 'r') as f:
+        content = f.readlines()
+        # Initialize version as default
+        version = "V.0.1"
+        # Start from the last line and move upwards
+        for line in reversed(content):
+            # If this line looks like a version number, use it and stop
+            if line.strip().startswith("V.0."):
+                version = line.strip()
+                break
+
+    # Extract version number
+    version_number = int(re.search(r'\d+(?=\s|$)', version).group())
+    # version_number = int(re.search(r'\d+$', version).group())
+
+    # Increment version number
+    new_version_number = version_number + 1
+
+    # Update version file
+    with open(version_file_path, 'a') as f:
+        # f.write(f"V.0.{new_version_number}\n")
+        f.write(f"V.0.{new_version_number} - {commit_message}\n")
+
+    # Execute git commands
+    os.system("git add -A")
+    os.system(f'git commit -m "V.0.{new_version_number} - {commit_message}"')
+    os.system("git push")
+
+    print(f"Committed Version V.0.{new_version_number}")
+
 
-print(f"Committed Version V.0.{new_version_number}")
+if __name__ == "__main__":
+    main()
```

