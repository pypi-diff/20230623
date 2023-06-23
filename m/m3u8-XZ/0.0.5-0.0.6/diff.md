# Comparing `tmp/m3u8_XZ-0.0.5.tar.gz` & `tmp/m3u8_XZ-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "H:\PythonProject\XZlib\packaging_m3u8\dist\.tmp-vky5il48\m3u8_XZ-0.0.5.tar", last modified: Tue Jun  6 12:06:56 2023, max compression
+gzip compressed data, was "H:\PythonProject\XZlib\packaging_m3u8\dist\.tmp-mpnavpmr\m3u8_XZ-0.0.6.tar", last modified: Fri Jun 23 07:51:48 2023, max compression
```

## Comparing `m3u8_XZ-0.0.5.tar` & `m3u8_XZ-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 12:06:56.347078 m3u8_XZ-0.0.5/
--rw-rw-rw-   0        0        0     1091 2023-03-23 03:00:43.000000 m3u8_XZ-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      835 2023-06-06 12:06:56.347078 m3u8_XZ-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      458 2023-06-06 11:17:28.000000 m3u8_XZ-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-06 12:06:56.338104 m3u8_XZ-0.0.5/m3u8_XZ/
--rw-rw-rw-   0        0        0      177 2023-06-06 11:01:44.000000 m3u8_XZ-0.0.5/m3u8_XZ/__init__.py
--rw-rw-rw-   0        0        0      678 2023-05-05 05:15:21.000000 m3u8_XZ-0.0.5/m3u8_XZ/cryptoModel.py
--rw-rw-rw-   0        0        0     6810 2023-06-06 10:41:28.000000 m3u8_XZ-0.0.5/m3u8_XZ/xz.py
-drwxrwxrwx   0        0        0        0 2023-06-06 12:06:56.345085 m3u8_XZ-0.0.5/m3u8_XZ.egg-info/
--rw-rw-rw-   0        0        0      835 2023-06-06 12:06:56.000000 m3u8_XZ-0.0.5/m3u8_XZ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-06-06 12:06:56.000000 m3u8_XZ-0.0.5/m3u8_XZ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 12:06:56.000000 m3u8_XZ-0.0.5/m3u8_XZ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-06 12:06:56.000000 m3u8_XZ-0.0.5/m3u8_XZ.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-06 12:06:56.000000 m3u8_XZ-0.0.5/m3u8_XZ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      522 2023-03-23 11:30:25.000000 m3u8_XZ-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-06 12:06:56.347078 m3u8_XZ-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      768 2023-06-06 12:06:35.000000 m3u8_XZ-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:51:48.559203 m3u8_XZ-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-03-23 03:00:43.000000 m3u8_XZ-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      835 2023-06-23 07:51:48.558213 m3u8_XZ-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2023-06-06 11:17:28.000000 m3u8_XZ-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 07:51:48.544244 m3u8_XZ-0.0.6/m3u8_XZ/
+-rw-rw-rw-   0        0        0      170 2023-06-23 07:09:11.000000 m3u8_XZ-0.0.6/m3u8_XZ/__init__.py
+-rw-rw-rw-   0        0        0      678 2023-05-05 05:15:21.000000 m3u8_XZ-0.0.6/m3u8_XZ/cryptoModel.py
+-rw-rw-rw-   0        0        0     6875 2023-06-23 07:27:16.000000 m3u8_XZ-0.0.6/m3u8_XZ/xz.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:51:48.557209 m3u8_XZ-0.0.6/m3u8_XZ.egg-info/
+-rw-rw-rw-   0        0        0      835 2023-06-23 07:51:48.000000 m3u8_XZ-0.0.6/m3u8_XZ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-06-23 07:51:48.000000 m3u8_XZ-0.0.6/m3u8_XZ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 07:51:48.000000 m3u8_XZ-0.0.6/m3u8_XZ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-23 07:51:48.000000 m3u8_XZ-0.0.6/m3u8_XZ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-23 07:51:48.000000 m3u8_XZ-0.0.6/m3u8_XZ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      522 2023-03-23 11:30:25.000000 m3u8_XZ-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-23 07:51:48.559203 m3u8_XZ-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      768 2023-06-23 07:51:21.000000 m3u8_XZ-0.0.6/setup.py
```

### Comparing `m3u8_XZ-0.0.5/LICENSE` & `m3u8_XZ-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `m3u8_XZ-0.0.5/PKG-INFO` & `m3u8_XZ-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3u8_XZ
-Version: 0.0.5
+Version: 0.0.6
 Summary: download m3u8 video by m3u8 url or by local m3u8 file
 Author: XZ
 Author-email: 345841407@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `m3u8_XZ-0.0.5/m3u8_XZ/cryptoModel.py` & `m3u8_XZ-0.0.6/m3u8_XZ/cryptoModel.py`

 * *Files identical despite different names*

### Comparing `m3u8_XZ-0.0.5/m3u8_XZ/xz.py` & `m3u8_XZ-0.0.6/m3u8_XZ/xz.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,17 @@
     def set_cry(self, text, url=""):
         # 获取加密参数
         x_key = re.findall('#EXT-X-KEY:(.*?)\n', text)
         cry_obj = dict()
         if len(x_key) > 0:
             # 提取
             for item in x_key[0].split(','):
-                cry_obj[item.split('=')[0]] = item.split('=')[1].replace('"', '')
+                key = item.split('=')[0]
+                value = item.replace(key, '')[1:].replace('"', '')
+                cry_obj[key] = value
             # format
             if cry_obj['URI'] and not cry_obj['URI'].startswith('http'):
                 cry_obj['URI'] = self.get_full_ts_url(url, cry_obj['URI'])
             # 获取key
             res = req.get(cry_obj['URI'], headers=self.headers)
             self.cry['key'] = res.content
             # 加密方式
```

### Comparing `m3u8_XZ-0.0.5/m3u8_XZ.egg-info/PKG-INFO` & `m3u8_XZ-0.0.6/m3u8_XZ.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m3u8-XZ
-Version: 0.0.5
+Version: 0.0.6
 Summary: download m3u8 video by m3u8 url or by local m3u8 file
 Author: XZ
 Author-email: 345841407@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `m3u8_XZ-0.0.5/pyproject.toml` & `m3u8_XZ-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `m3u8_XZ-0.0.5/setup.py` & `m3u8_XZ-0.0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="m3u8_XZ",
-    version="0.0.5",
+    version="0.0.6",
     author="XZ",
     author_email="345841407@qq.com",
     description="download m3u8 video by m3u8 url or by local m3u8 file",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

