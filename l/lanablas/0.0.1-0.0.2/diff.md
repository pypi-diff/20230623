# Comparing `tmp/lanablas-0.0.1.tar.gz` & `tmp/lanablas-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanablas-0.0.1.tar", last modified: Tue Jun 20 10:14:59 2023, max compression
+gzip compressed data, was "lanablas-0.0.2.tar", last modified: Thu Jun 22 21:42:02 2023, max compression
```

## Comparing `lanablas-0.0.1.tar` & `lanablas-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-20 10:14:59.505854 lanablas-0.0.1/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      406 2023-06-20 10:14:59.505554 lanablas-0.0.1/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       12 2023-06-20 10:00:33.000000 lanablas-0.0.1/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-20 10:14:59.504047 lanablas-0.0.1/lanablas/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       59 2023-06-20 09:59:49.000000 lanablas-0.0.1/lanablas/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1987 2023-06-20 09:52:11.000000 lanablas-0.0.1/lanablas/matrix.c
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-20 10:14:59.505150 lanablas-0.0.1/lanablas.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      406 2023-06-20 10:14:58.000000 lanablas-0.0.1/lanablas.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      185 2023-06-20 10:14:59.000000 lanablas-0.0.1/lanablas.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-20 10:14:58.000000 lanablas-0.0.1/lanablas.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-20 10:14:59.000000 lanablas-0.0.1/lanablas.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-20 10:14:59.505954 lanablas-0.0.1/setup.cfg
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1097 2023-06-20 10:02:06.000000 lanablas-0.0.1/setup.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-22 21:42:02.201899 lanablas-0.0.2/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1060 2023-06-20 12:16:48.000000 lanablas-0.0.2/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1189 2023-06-22 21:42:02.201431 lanablas-0.0.2/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      777 2023-06-20 12:15:53.000000 lanablas-0.0.2/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-22 21:42:02.198089 lanablas-0.0.2/lanablas/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       78 2023-06-22 21:00:47.000000 lanablas-0.0.2/lanablas/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5451 2023-06-22 21:41:55.000000 lanablas-0.0.2/lanablas/matrix.c
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-06-22 21:42:02.200688 lanablas-0.0.2/lanablas.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1189 2023-06-22 21:42:01.000000 lanablas-0.0.2/lanablas.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-06-22 21:42:02.000000 lanablas-0.0.2/lanablas.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-06-22 21:42:01.000000 lanablas-0.0.2/lanablas.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       16 2023-06-22 21:42:01.000000 lanablas-0.0.2/lanablas.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-06-22 21:42:02.202044 lanablas-0.0.2/setup.cfg
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1116 2023-06-22 20:54:30.000000 lanablas-0.0.2/setup.py
```

### Comparing `lanablas-0.0.1/setup.py` & `lanablas-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,19 @@
     extra_compile_args=['-std=c11'],  # Set the C standard to C11
     include_dirs=['/usr/local/opt/openblas/include'],  # BLAS include directory
     library_dirs=['/usr/local/opt/openblas/lib'],  # BLAS library directory
 )
 
 setup(
 name='lanablas',
-    version='0.0.1',
+    version='0.0.2',
     description='Extension module for matrix multiplication',
     author='Marco Salvalaggio',
     author_email='mar.salvalaggio@gmail.com',
+    license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=['lanablas'],
     ext_modules=[module_extension],
     classifiers=[
           "Programming Language :: Python :: 3",
           "License :: OSI Approved :: MIT License",
```

