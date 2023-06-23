# Comparing `tmp/kangtools-0.0.3.tar.gz` & `tmp/kangtools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kangtools-0.0.3.tar", last modified: Fri Jun 23 19:36:15 2023, max compression
+gzip compressed data, was "kangtools-0.0.4.tar", last modified: Fri Jun 23 19:40:09 2023, max compression
```

## Comparing `kangtools-0.0.3.tar` & `kangtools-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-23 19:36:15.884848 kangtools-0.0.3/
--rw-r--r--   0 kang       (501) staff       (20)     4408 2023-06-23 19:36:15.884735 kangtools-0.0.3/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)     4193 2023-06-23 19:34:01.000000 kangtools-0.0.3/README.md
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-23 19:36:15.883976 kangtools-0.0.3/kangtools/
--rw-r--r--   0 kang       (501) staff       (20)       49 2023-06-23 19:23:54.000000 kangtools-0.0.3/kangtools/__init__.py
--rwxr-xr-x   0 kang       (501) staff       (20)     1478 2023-06-23 19:31:19.000000 kangtools-0.0.3/kangtools/version_control.py
-drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-23 19:36:15.884579 kangtools-0.0.3/kangtools.egg-info/
--rw-r--r--   0 kang       (501) staff       (20)     4408 2023-06-23 19:36:15.000000 kangtools-0.0.3/kangtools.egg-info/PKG-INFO
--rw-r--r--   0 kang       (501) staff       (20)      237 2023-06-23 19:36:15.000000 kangtools-0.0.3/kangtools.egg-info/SOURCES.txt
--rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-23 19:36:15.000000 kangtools-0.0.3/kangtools.egg-info/dependency_links.txt
--rw-r--r--   0 kang       (501) staff       (20)       77 2023-06-23 19:36:15.000000 kangtools-0.0.3/kangtools.egg-info/entry_points.txt
--rw-r--r--   0 kang       (501) staff       (20)       10 2023-06-23 19:36:15.000000 kangtools-0.0.3/kangtools.egg-info/top_level.txt
--rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-23 19:36:15.884887 kangtools-0.0.3/setup.cfg
--rw-r--r--   0 kang       (501) staff       (20)      780 2023-06-23 19:36:00.000000 kangtools-0.0.3/setup.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-23 19:40:09.967411 kangtools-0.0.4/
+-rw-r--r--   0 kang       (501) staff       (20)     4408 2023-06-23 19:40:09.967294 kangtools-0.0.4/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)     4193 2023-06-23 19:34:01.000000 kangtools-0.0.4/README.md
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-23 19:40:09.966546 kangtools-0.0.4/kangtools/
+-rw-r--r--   0 kang       (501) staff       (20)       86 2023-06-23 19:39:26.000000 kangtools-0.0.4/kangtools/__init__.py
+-rwxr-xr-x   0 kang       (501) staff       (20)     1478 2023-06-23 19:31:19.000000 kangtools-0.0.4/kangtools/version_control.py
+drwxr-xr-x   0 kang       (501) staff       (20)        0 2023-06-23 19:40:09.967157 kangtools-0.0.4/kangtools.egg-info/
+-rw-r--r--   0 kang       (501) staff       (20)     4408 2023-06-23 19:40:09.000000 kangtools-0.0.4/kangtools.egg-info/PKG-INFO
+-rw-r--r--   0 kang       (501) staff       (20)      237 2023-06-23 19:40:09.000000 kangtools-0.0.4/kangtools.egg-info/SOURCES.txt
+-rw-r--r--   0 kang       (501) staff       (20)        1 2023-06-23 19:40:09.000000 kangtools-0.0.4/kangtools.egg-info/dependency_links.txt
+-rw-r--r--   0 kang       (501) staff       (20)       77 2023-06-23 19:40:09.000000 kangtools-0.0.4/kangtools.egg-info/entry_points.txt
+-rw-r--r--   0 kang       (501) staff       (20)       10 2023-06-23 19:40:09.000000 kangtools-0.0.4/kangtools.egg-info/top_level.txt
+-rw-r--r--   0 kang       (501) staff       (20)       38 2023-06-23 19:40:09.967442 kangtools-0.0.4/setup.cfg
+-rw-r--r--   0 kang       (501) staff       (20)      780 2023-06-23 19:39:42.000000 kangtools-0.0.4/setup.py
```

### Comparing `kangtools-0.0.3/PKG-INFO` & `kangtools-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kangtools
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package for version control.
 Author: xiaowen kang
 Author-email: kangxiaowen@gmail.com
 License: LICENSE
 Description-Content-Type: text/markdown
 
 # kangtools
```

### Comparing `kangtools-0.0.3/README.md` & `kangtools-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `kangtools-0.0.3/kangtools/version_control.py` & `kangtools-0.0.4/kangtools/version_control.py`

 * *Files identical despite different names*

### Comparing `kangtools-0.0.3/kangtools.egg-info/PKG-INFO` & `kangtools-0.0.4/kangtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kangtools
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package for version control.
 Author: xiaowen kang
 Author-email: kangxiaowen@gmail.com
 License: LICENSE
 Description-Content-Type: text/markdown
 
 # kangtools
```

### Comparing `kangtools-0.0.3/setup.py` & `kangtools-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='kangtools',  # 包的名字
-    version='0.0.3',  # 包的版本
+    version='0.0.4',  # 包的版本
     author='xiaowen kang',  # 你的名字
     author_email='kangxiaowen@gmail.com',  # 你的邮箱
     packages=['kangtools'],  # 包含的包，这是一个列表，如果你的项目包含多个包，都需要列在这里
     license='LICENSE',  # 许可证文件
     description='A Python package for version control.',  # 包的简短描述
     long_description=open('README.md').read(),  # 包的详细描述，通常从 README.md 文件读取
     long_description_content_type="text/markdown",  # 描述的格式，使用markdown格式
```

