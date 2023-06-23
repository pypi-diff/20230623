# Comparing `tmp/dartrig-0.1.8.tar.gz` & `tmp/dartrig-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dartrig-0.1.8.tar", last modified: Mon Jun  5 04:16:28 2023, max compression
+gzip compressed data, was "dist/dartrig-0.1.9.tar", last modified: Mon Jun  5 04:32:27 2023, max compression
```

## Comparing `dartrig-0.1.8.tar` & `dartrig-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:16:28.000000 dartrig-0.1.8/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-05 04:16:28.000000 dartrig-0.1.8/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.8/LICENSE
--rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.8/README.md
--rw-r--r--   0 nezah      (501) staff       (20)      693 2023-06-05 04:16:27.000000 dartrig-0.1.8/setup.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:16:28.000000 dartrig-0.1.8/dartrig/
--rw-r--r--   0 nezah      (501) staff       (20)    15575 2023-06-05 04:12:34.000000 dartrig-0.1.8/dartrig/__init__.py
--rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.8/dartrig/annotations.py
-drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:16:28.000000 dartrig-0.1.8/dartrig.egg-info/
--rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-05 04:16:28.000000 dartrig-0.1.8/dartrig.egg-info/PKG-INFO
--rw-r--r--   0 nezah      (501) staff       (20)      223 2023-06-05 04:16:28.000000 dartrig-0.1.8/dartrig.egg-info/SOURCES.txt
--rw-r--r--   0 nezah      (501) staff       (20)       31 2023-06-05 04:16:28.000000 dartrig-0.1.8/dartrig.egg-info/requires.txt
--rw-r--r--   0 nezah      (501) staff       (20)        8 2023-06-05 04:16:28.000000 dartrig-0.1.8/dartrig.egg-info/top_level.txt
--rw-r--r--   0 nezah      (501) staff       (20)        1 2023-06-05 04:16:28.000000 dartrig-0.1.8/dartrig.egg-info/dependency_links.txt
--rw-r--r--   0 nezah      (501) staff       (20)       38 2023-06-05 04:16:28.000000 dartrig-0.1.8/setup.cfg
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:32:27.000000 dartrig-0.1.9/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-05 04:32:27.000000 dartrig-0.1.9/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)     1081 2023-03-17 05:39:07.000000 dartrig-0.1.9/LICENSE
+-rw-r--r--   0 nezah      (501) staff       (20)     1061 2023-04-11 08:24:52.000000 dartrig-0.1.9/README.md
+-rw-r--r--   0 nezah      (501) staff       (20)      693 2023-06-05 04:32:26.000000 dartrig-0.1.9/setup.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:32:27.000000 dartrig-0.1.9/dartrig/
+-rw-r--r--   0 nezah      (501) staff       (20)    15949 2023-06-05 04:32:09.000000 dartrig-0.1.9/dartrig/__init__.py
+-rw-r--r--   0 nezah      (501) staff       (20)      682 2023-03-18 12:39:55.000000 dartrig-0.1.9/dartrig/annotations.py
+drwxr-xr-x   0 nezah      (501) staff       (20)        0 2023-06-05 04:32:27.000000 dartrig-0.1.9/dartrig.egg-info/
+-rw-r--r--   0 nezah      (501) staff       (20)     1485 2023-06-05 04:32:27.000000 dartrig-0.1.9/dartrig.egg-info/PKG-INFO
+-rw-r--r--   0 nezah      (501) staff       (20)      223 2023-06-05 04:32:27.000000 dartrig-0.1.9/dartrig.egg-info/SOURCES.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       31 2023-06-05 04:32:27.000000 dartrig-0.1.9/dartrig.egg-info/requires.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        8 2023-06-05 04:32:27.000000 dartrig-0.1.9/dartrig.egg-info/top_level.txt
+-rw-r--r--   0 nezah      (501) staff       (20)        1 2023-06-05 04:32:27.000000 dartrig-0.1.9/dartrig.egg-info/dependency_links.txt
+-rw-r--r--   0 nezah      (501) staff       (20)       38 2023-06-05 04:32:27.000000 dartrig-0.1.9/setup.cfg
```

### Comparing `dartrig-0.1.8/PKG-INFO` & `dartrig-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.8
+Version: 0.1.9
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dartrig-0.1.8/LICENSE` & `dartrig-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.8/README.md` & `dartrig-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.8/setup.py` & `dartrig-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="dartrig",
-    version="0.1.8",
+    version="0.1.9",
     install_requires=[
         'requests',
         'bs4',
         'adt_cache==0.0.12'
     ],
     license='MIT',
     author="cheddars",
```

### Comparing `dartrig-0.1.8/dartrig/__init__.py` & `dartrig-0.1.9/dartrig/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,36 +113,48 @@
                 logger.debug(f"dsaf001_report cache set for rcp_no {rcp_no}")
         except Exception as ex:
             logger.exception(ex)
             raise ValueError(f"dcm number fetch failed for rcp_no : [{rcp_no}]")
 
         return dcm_no
 
-    def get_dsaf_meta(self, rcp_no, keyword="연결재무") -> Dict[str, any]:
+    def get_dsaf_meta(self, rcp_no, keywords=None) -> Dict[str, any]:
+        """
+        :param rcp_no:
+        :param keywords: [연결재무, 재무에관한]
+        :return:
+        """
         cache_key = f"dcm_meta_{rcp_no}"
         try:
             if self.cache is not None:
                 cached: Dict = self.cache.hget(cache_key)
                 if cached is not None and len(cached) > 0:
                     logger.debug(f"dsaf001_meta cache hit for rcp_no {rcp_no} => {cached}")
                     return cached
 
             html_text = self._try_file_cache_request(f"{URLS['DART_DSAF']}?rcpNo={rcp_no}", "dsaf", rcp_no)
             numbers = re.findall("\d{7}", html_text)
             dcm_no = numbers[2]
-            find1_num = html_text.index(keyword)  # 여기 viewDoc에서 필요한 정보가 다 들어있음
-            res_text = remove_strs_list(html_text[find1_num:find1_num + 250],
+            find1_num, ele_id, offset, length = [-1] * 4
+
+            while find1_num == -1:
+                for keyword in keywords:
+                    find1_num = html_text.find(keyword)  # 여기 viewDoc에서 필요한 정보가 다 들어있음
+                    if find1_num != -1:
+                        break
+            if find1_num == -1:
+                res_text = remove_strs_list(html_text[find1_num:find1_num + 250],
                                         ['\t', '\n', "\'", 'node1', 'dart3', '"', "'"])
 
-            find1_list = list(filter(lambda x: x is not None, map(fun_splitter, res_text.split(";"))))
-            ele_id = find1_list[3]
-            offset = find1_list[4]
-            length = find1_list[5]
+                find1_list = list(filter(lambda x: x is not None, map(fun_splitter, res_text.split(";"))))
+                ele_id = find1_list[3]
+                offset = find1_list[4]
+                length = find1_list[5]
 
-            meta = { "dcm_no" : dcm_no, "ele_id" : ele_id, "offset" : offset, "length" : length }
+            meta = { "dcm_no" : dcm_no, "ele_id" : ele_id, "offset" : offset, "length": length }
             if self.cache is not None:
                 self.cache.hset(cache_key, meta)
                 logger.debug(f"dsaf001_meta cache set for rcp_no {rcp_no}")
 
             return meta
         except Exception as ex:
             logger.exception(ex)
```

### Comparing `dartrig-0.1.8/dartrig/annotations.py` & `dartrig-0.1.9/dartrig/annotations.py`

 * *Files identical despite different names*

### Comparing `dartrig-0.1.8/dartrig.egg-info/PKG-INFO` & `dartrig-0.1.9/dartrig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dartrig
-Version: 0.1.8
+Version: 0.1.9
 Summary: dartrig api wrapper
 Home-page: https://github.com/cheddars/dart_rigger
 Author: cheddars
 Author-email: nezahrish@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

