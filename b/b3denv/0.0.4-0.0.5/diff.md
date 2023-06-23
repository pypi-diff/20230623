# Comparing `tmp/b3denv-0.0.4.tar.gz` & `tmp/b3denv-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b3denv-0.0.4.tar", last modified: Wed Jan 18 18:36:25 2023, max compression
+gzip compressed data, was "b3denv-0.0.5.tar", last modified: Fri Jun 23 16:25:06 2023, max compression
```

## Comparing `b3denv-0.0.4.tar` & `b3denv-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-01-18 18:36:25.476945 b3denv-0.0.4/
--rw-r--r--   0 robstenson   (501) staff       (20)      454 2023-01-18 18:36:25.476790 b3denv-0.0.4/PKG-INFO
--rw-r--r--   0 robstenson   (501) staff       (20)      430 2023-01-18 18:25:39.000000 b3denv-0.0.4/README.md
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-01-18 18:36:25.475450 b3denv-0.0.4/b3denv/
--rw-r--r--   0 robstenson   (501) staff       (20)     9838 2023-01-18 18:22:07.000000 b3denv-0.0.4/b3denv/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)       62 2022-11-09 19:31:16.000000 b3denv-0.0.4/b3denv/__main__.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-01-18 18:36:25.476523 b3denv-0.0.4/b3denv.egg-info/
--rw-r--r--   0 robstenson   (501) staff       (20)      454 2023-01-18 18:36:25.000000 b3denv-0.0.4/b3denv.egg-info/PKG-INFO
--rw-r--r--   0 robstenson   (501) staff       (20)      209 2023-01-18 18:36:25.000000 b3denv-0.0.4/b3denv.egg-info/SOURCES.txt
--rw-r--r--   0 robstenson   (501) staff       (20)        1 2023-01-18 18:36:25.000000 b3denv-0.0.4/b3denv.egg-info/dependency_links.txt
--rw-r--r--   0 robstenson   (501) staff       (20)       39 2023-01-18 18:36:25.000000 b3denv-0.0.4/b3denv.egg-info/entry_points.txt
--rw-r--r--   0 robstenson   (501) staff       (20)        7 2023-01-18 18:36:25.000000 b3denv-0.0.4/b3denv.egg-info/top_level.txt
--rw-r--r--   0 robstenson   (501) staff       (20)       38 2023-01-18 18:36:25.476993 b3denv-0.0.4/setup.cfg
--rw-r--r--   0 robstenson   (501) staff       (20)      745 2023-01-18 18:16:57.000000 b3denv-0.0.4/setup.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-06-23 16:25:06.728673 b3denv-0.0.5/
+-rw-r--r--   0 robstenson   (501) staff       (20)      453 2023-06-23 16:25:06.728531 b3denv-0.0.5/PKG-INFO
+-rw-r--r--   0 robstenson   (501) staff       (20)      430 2023-01-18 18:25:39.000000 b3denv-0.0.5/README.md
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-06-23 16:25:06.727460 b3denv-0.0.5/b3denv/
+-rw-r--r--   0 robstenson   (501) staff       (20)    10333 2023-06-23 16:24:37.000000 b3denv-0.0.5/b3denv/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)       62 2022-11-09 19:31:16.000000 b3denv-0.0.5/b3denv/__main__.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-06-23 16:25:06.728369 b3denv-0.0.5/b3denv.egg-info/
+-rw-r--r--   0 robstenson   (501) staff       (20)      453 2023-06-23 16:25:06.000000 b3denv-0.0.5/b3denv.egg-info/PKG-INFO
+-rw-r--r--   0 robstenson   (501) staff       (20)      209 2023-06-23 16:25:06.000000 b3denv-0.0.5/b3denv.egg-info/SOURCES.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)        1 2023-06-23 16:25:06.000000 b3denv-0.0.5/b3denv.egg-info/dependency_links.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)       39 2023-06-23 16:25:06.000000 b3denv-0.0.5/b3denv.egg-info/entry_points.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)        7 2023-06-23 16:25:06.000000 b3denv-0.0.5/b3denv.egg-info/top_level.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)       38 2023-06-23 16:25:06.728764 b3denv-0.0.5/setup.cfg
+-rw-r--r--   0 robstenson   (501) staff       (20)      744 2023-06-23 16:24:37.000000 b3denv-0.0.5/setup.py
```

### Comparing `b3denv-0.0.4/b3denv/__init__.py` & `b3denv-0.0.5/b3denv/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,21 @@
     
     blender = os.environ.get("BLENDER_PATH")
     #blender = config.get("BLENDER")
     
     if not blender:
         if on_mac():
             blender = "/Applications/Blender.app/"
+        elif on_windows():
+            folder = "C:\\Program Files\\Blender Foundation"
+            blenders = [os.path.join(folder, f) for f in os.listdir(folder) if os.path.isdir(os.path.join(folder, f))]
+            blenders.sort()
+            if len(blenders) == 0:
+                print("Could not find a blender installation. Either install one to the default location or specify one with environment variable BLENDER_PATH")
+            blender = os.path.join(blenders[-1], "blender.exe")
 
     blender = os.path.abspath(os.path.expanduser(blender))
 
     if on_mac():
         res = os.path.join(blender, "Contents/Resources")
         version = None
         for p in os.listdir(res):
@@ -252,15 +259,15 @@
         else:
             if a.startswith("-"):
                 dashes.append(a)
             else:
                 args.append(a)
     
     if "-v" in dashes or "--version" in dashes:
-        return "0.0.4"
+        return "0.0.5"
 
     if len(args) == 1:
         print("b3denv <action> <extension-name>?")
         return
 
     action = args[1]
     if len(args) > 2:
```

### Comparing `b3denv-0.0.4/setup.py` & `b3denv-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 ### Help with setting up bpy/blender/blender addons
 
 More info available at: [coldtype.xyz](https://coldtype.xyz)
 """
 
 setuptools.setup(
     name="b3denv",
-    version="0.0.4",
+    version="0.0.5",
     author="Rob Stenson / Coldtype",
     author_email="rob@goodhertz.com",
     description="Help with blender python",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/coldtype/b3denv",
+    url="https://github.com/stenson/b3denv",
     packages=[
         "b3denv",
     ],
     entry_points={
         'console_scripts': [
             'b3denv = b3denv:main'
         ],
```

