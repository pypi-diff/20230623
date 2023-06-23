# Comparing `tmp/fileaccess-0.2.12.tar.gz` & `tmp/fileaccess-0.2.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fileaccess-0.2.12.tar", last modified: Wed Apr 26 23:24:10 2023, max compression
+gzip compressed data, was "fileaccess-0.2.13.tar", last modified: Fri Jun 23 19:36:19 2023, max compression
```

## Comparing `fileaccess-0.2.12.tar` & `fileaccess-0.2.13.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-04-26 23:24:10.993861 fileaccess-0.2.12/
--rw-r--r--   0 joehacobian   (501) staff       (20)     3311 2023-04-26 23:24:10.993639 fileaccess-0.2.12/PKG-INFO
--rw-r--r--   0 joehacobian   (501) staff       (20)     2580 2023-04-26 19:30:55.000000 fileaccess-0.2.12/README.md
-drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-04-26 23:24:10.991161 fileaccess-0.2.12/fileaccess/
--rw-r--r--   0 joehacobian   (501) staff       (20)     4375 2023-04-26 22:46:58.000000 fileaccess-0.2.12/fileaccess/__init__.py
-drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-04-26 23:24:10.993185 fileaccess-0.2.12/fileaccess.egg-info/
--rw-r--r--   0 joehacobian   (501) staff       (20)     3311 2023-04-26 23:24:10.000000 fileaccess-0.2.12/fileaccess.egg-info/PKG-INFO
--rw-r--r--   0 joehacobian   (501) staff       (20)      210 2023-04-26 23:24:10.000000 fileaccess-0.2.12/fileaccess.egg-info/SOURCES.txt
--rw-r--r--   0 joehacobian   (501) staff       (20)        1 2023-04-26 23:24:10.000000 fileaccess-0.2.12/fileaccess.egg-info/dependency_links.txt
--rw-r--r--   0 joehacobian   (501) staff       (20)        3 2023-04-26 23:24:10.000000 fileaccess-0.2.12/fileaccess.egg-info/requires.txt
--rw-r--r--   0 joehacobian   (501) staff       (20)       11 2023-04-26 23:24:10.000000 fileaccess-0.2.12/fileaccess.egg-info/top_level.txt
--rw-r--r--   0 joehacobian   (501) staff       (20)       38 2023-04-26 23:24:10.993971 fileaccess-0.2.12/setup.cfg
--rw-r--r--   0 joehacobian   (501) staff       (20)      942 2023-04-26 23:15:34.000000 fileaccess-0.2.12/setup.py
+drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-06-23 19:36:19.373391 fileaccess-0.2.13/
+-rw-r--r--   0 joehacobian   (501) staff       (20)     1060 2023-04-26 23:34:23.000000 fileaccess-0.2.13/LICENSE
+-rw-r--r--   0 joehacobian   (501) staff       (20)     3858 2023-06-23 19:36:19.373134 fileaccess-0.2.13/PKG-INFO
+-rw-r--r--   0 joehacobian   (501) staff       (20)     3015 2023-06-23 19:25:55.000000 fileaccess-0.2.13/README.md
+drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-06-23 19:36:19.371045 fileaccess-0.2.13/fileaccess/
+-rw-r--r--   0 joehacobian   (501) staff       (20)     4375 2023-04-26 22:46:58.000000 fileaccess-0.2.13/fileaccess/__init__.py
+drwxr-xr-x   0 joehacobian   (501) staff       (20)        0 2023-06-23 19:36:19.372786 fileaccess-0.2.13/fileaccess.egg-info/
+-rw-r--r--   0 joehacobian   (501) staff       (20)     3858 2023-06-23 19:36:19.000000 fileaccess-0.2.13/fileaccess.egg-info/PKG-INFO
+-rw-r--r--   0 joehacobian   (501) staff       (20)      218 2023-06-23 19:36:19.000000 fileaccess-0.2.13/fileaccess.egg-info/SOURCES.txt
+-rw-r--r--   0 joehacobian   (501) staff       (20)        1 2023-06-23 19:36:19.000000 fileaccess-0.2.13/fileaccess.egg-info/dependency_links.txt
+-rw-r--r--   0 joehacobian   (501) staff       (20)        3 2023-06-23 19:36:19.000000 fileaccess-0.2.13/fileaccess.egg-info/requires.txt
+-rw-r--r--   0 joehacobian   (501) staff       (20)       11 2023-06-23 19:36:19.000000 fileaccess-0.2.13/fileaccess.egg-info/top_level.txt
+-rw-r--r--   0 joehacobian   (501) staff       (20)       38 2023-06-23 19:36:19.373468 fileaccess-0.2.13/setup.cfg
+-rw-r--r--   0 joehacobian   (501) staff       (20)     1032 2023-06-23 19:25:51.000000 fileaccess-0.2.13/setup.py
```

### Comparing `fileaccess-0.2.12/PKG-INFO` & `fileaccess-0.2.13/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: fileaccess
-Version: 0.2.12
-Summary: A package for easier file access
+Version: 0.2.13
+Summary: A package for easier file access, automatically closes opened file handles, & provides for simple file/directory creation.
 Home-page: https://github.com/node0/Fileaccess
 Author: Joe Hacobian
 Author-email: joehacobian@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Fileaccess Utility Class
 
 ## Introduction
-`Fileaccess` is a utility class for safely dealing with files. This class can be used to read, write, or append to a file, as well as create a file or directory.
+`Fileaccess` is a utility class for safely dealing with files. This class can be used to read, write, or append to a file, as well as create a file or directory. A nice benefit of using it is the automatic file handle management it provides.  
+
+The main productivity benefit of using this class is the createFile() method which creates file and directory paths automatically for a given file or directory asset, as well as allowing the writing of file contents together in a single method call. If you find yourself writing out a directory tree or a lot of files, this can save you frustration.  
 
 ## Usage
 ### Reading a File
 To read a file, use the `with` statement and specify the file name and mode as the `Fileaccess` class parameters. Here's an example:
 
 ```python
 with Fileaccess("filename.txt", "r") as file:
```

### Comparing `fileaccess-0.2.12/README.md` & `fileaccess-0.2.13/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Fileaccess Utility Class
 
 ## Introduction
-`Fileaccess` is a utility class for safely dealing with files. This class can be used to read, write, or append to a file, as well as create a file or directory.
+`Fileaccess` is a utility class for safely dealing with files. This class can be used to read, write, or append to a file, as well as create a file or directory. A nice benefit of using it is the automatic file handle management it provides.  
+
+The main productivity benefit of using this class is the createFile() method which creates file and directory paths automatically for a given file or directory asset, as well as allowing the writing of file contents together in a single method call. If you find yourself writing out a directory tree or a lot of files, this can save you frustration.  
 
 ## Usage
 ### Reading a File
 To read a file, use the `with` statement and specify the file name and mode as the `Fileaccess` class parameters. Here's an example:
 
 ```python
 with Fileaccess("filename.txt", "r") as file:
```

### Comparing `fileaccess-0.2.12/fileaccess/__init__.py` & `fileaccess-0.2.13/fileaccess/__init__.py`

 * *Files identical despite different names*

### Comparing `fileaccess-0.2.12/fileaccess.egg-info/PKG-INFO` & `fileaccess-0.2.13/fileaccess.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 Metadata-Version: 2.1
 Name: fileaccess
-Version: 0.2.12
-Summary: A package for easier file access
+Version: 0.2.13
+Summary: A package for easier file access, automatically closes opened file handles, & provides for simple file/directory creation.
 Home-page: https://github.com/node0/Fileaccess
 Author: Joe Hacobian
 Author-email: joehacobian@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Fileaccess Utility Class
 
 ## Introduction
-`Fileaccess` is a utility class for safely dealing with files. This class can be used to read, write, or append to a file, as well as create a file or directory.
+`Fileaccess` is a utility class for safely dealing with files. This class can be used to read, write, or append to a file, as well as create a file or directory. A nice benefit of using it is the automatic file handle management it provides.  
+
+The main productivity benefit of using this class is the createFile() method which creates file and directory paths automatically for a given file or directory asset, as well as allowing the writing of file contents together in a single method call. If you find yourself writing out a directory tree or a lot of files, this can save you frustration.  
 
 ## Usage
 ### Reading a File
 To read a file, use the `with` statement and specify the file name and mode as the `Fileaccess` class parameters. Here's an example:
 
 ```python
 with Fileaccess("filename.txt", "r") as file:
```

### Comparing `fileaccess-0.2.12/setup.py` & `fileaccess-0.2.13/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name="fileaccess",
-    version="0.2.12",
+    version="0.2.13",
     packages=find_packages(),
     install_requires=[
         "sh"
     ],
     author="Joe Hacobian",
     author_email="joehacobian@gmail.com",
-    description="A package for easier file access",
+    description="A package for easier file access, automatically closes opened file handles, & provides for simple file/directory creation.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/node0/Fileaccess",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

