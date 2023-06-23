# Comparing `tmp/pohan-0.0.5.tar.gz` & `tmp/pohan-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pohan-0.0.5.tar", last modified: Sun Apr  9 16:10:52 2023, max compression
+gzip compressed data, was "pohan-0.0.6.tar", last modified: Fri Jun 23 16:32:22 2023, max compression
```

## Comparing `pohan-0.0.5.tar` & `pohan-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 16:10:52.386173 pohan-0.0.5/
--rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 pohan-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2955 2023-04-09 16:10:52.386173 pohan-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2432 2023-04-09 11:32:50.000000 pohan-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 16:10:52.349036 pohan-0.0.5/pohan/
--rw-rw-rw-   0        0        0       25 2023-04-07 14:38:11.000000 pohan-0.0.5/pohan/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:10:52.379275 pohan-0.0.5/pohan/api/
--rw-rw-rw-   0        0        0       20 2023-04-09 11:28:35.000000 pohan-0.0.5/pohan/api/__init__.py
--rw-rw-rw-   0        0        0     1345 2023-04-09 16:10:12.000000 pohan-0.0.5/pohan/api/common.py
--rw-rw-rw-   0        0        0      402 2023-04-09 11:31:38.000000 pohan-0.0.5/pohan/api/普通话.py
--rw-rw-rw-   0        0        0      342 2023-04-09 06:22:08.000000 pohan-0.0.5/pohan/api/重庆话.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:10:52.381274 pohan-0.0.5/pohan/lib/
--rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pohan-0.0.5/pohan/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:10:52.371763 pohan-0.0.5/pohan.egg-info/
--rw-rw-rw-   0        0        0     2955 2023-04-09 16:10:52.000000 pohan-0.0.5/pohan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-04-09 16:10:52.000000 pohan-0.0.5/pohan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 16:10:52.000000 pohan-0.0.5/pohan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-09 11:26:51.000000 pohan-0.0.5/pohan.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-04-09 16:10:52.000000 pohan-0.0.5/pohan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      688 2023-04-09 16:10:52.389707 pohan-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 pohan-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-09 16:10:52.384177 pohan-0.0.5/tests/
--rw-rw-rw-   0        0        0      181 2023-04-05 16:44:51.000000 pohan-0.0.5/tests/__init__.py
--rw-rw-rw-   0        0        0      392 2023-04-07 14:16:56.000000 pohan-0.0.5/tests/test_pohan.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:32:22.404749 pohan-0.0.6/
+-rw-rw-rw-   0        0        0     1093 2022-09-13 01:21:27.000000 pohan-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2955 2023-06-23 16:32:22.405743 pohan-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2432 2023-04-09 11:32:50.000000 pohan-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 16:32:22.341434 pohan-0.0.6/pohan/
+-rw-rw-rw-   0        0        0       58 2023-06-23 16:13:54.000000 pohan-0.0.6/pohan/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:32:22.387519 pohan-0.0.6/pohan/api/
+-rw-rw-rw-   0        0        0       20 2023-04-09 11:28:35.000000 pohan-0.0.6/pohan/api/__init__.py
+-rw-rw-rw-   0        0        0     1404 2023-06-23 16:16:40.000000 pohan-0.0.6/pohan/api/common.py
+-rw-rw-rw-   0        0        0      402 2023-04-09 11:31:38.000000 pohan-0.0.6/pohan/api/普通话.py
+-rw-rw-rw-   0        0        0      342 2023-04-09 06:22:08.000000 pohan-0.0.6/pohan/api/重庆话.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:32:22.390517 pohan-0.0.6/pohan/lib/
+-rw-rw-rw-   0        0        0        0 2022-09-13 01:21:27.000000 pohan-0.0.6/pohan/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:32:22.394521 pohan-0.0.6/pohan/pinyin/
+-rw-rw-rw-   0        0        0       20 2023-06-23 16:13:06.000000 pohan-0.0.6/pohan/pinyin/__init__.py
+-rw-rw-rw-   0        0        0      629 2023-06-23 16:15:33.000000 pohan-0.0.6/pohan/pinyin/pinyin.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:32:22.374481 pohan-0.0.6/pohan.egg-info/
+-rw-rw-rw-   0        0        0     2955 2023-06-23 16:32:22.000000 pohan-0.0.6/pohan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2023-06-23 16:32:22.000000 pohan-0.0.6/pohan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 16:32:22.000000 pohan-0.0.6/pohan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-23 16:04:10.000000 pohan-0.0.6/pohan.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        9 2023-06-23 16:32:22.000000 pohan-0.0.6/pohan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-23 16:32:22.000000 pohan-0.0.6/pohan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      699 2023-06-23 16:32:22.409280 pohan-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      389 2022-10-23 08:47:10.000000 pohan-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 16:32:22.401745 pohan-0.0.6/tests/
+-rw-rw-rw-   0        0        0      181 2023-04-05 16:44:51.000000 pohan-0.0.6/tests/__init__.py
+-rw-rw-rw-   0        0        0      392 2023-04-07 14:16:56.000000 pohan-0.0.6/tests/test_pohan.py
```

### Comparing `pohan-0.0.5/LICENSE` & `pohan-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pohan-0.0.5/PKG-INFO` & `pohan-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pohan
-Version: 0.0.5
+Version: 0.0.6
 Summary: pip install pohan
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/pohan/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/pohan/blob/master/README.md
```

### Comparing `pohan-0.0.5/README.md` & `pohan-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pohan-0.0.5/pohan/api/common.py` & `pohan-0.0.6/pohan/api/common.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,50 +2,51 @@
 '''
 @Author  ：B站/抖音/微博/小红书/公众号，都叫：程序员晚枫
 @WeChat     ：CoderWanFeng
 @Blog      ：www.python-office.com
 @Date    ：2023/4/9 19:26 
 @Description     ：
 '''
-import office
-from search4file import search_by_content
+
+# import office
+# from search4file import search_by_content
 
 """
 功能关键词
 """
 
 ################# Excel #################
 
-创建Excel = office.excel.fake2excel
-Excel转PDF = office.excel.excel2pdf
-
-################# PDF #################
-加密PDF = office.pdf.encrypt4pdf
-PDF转图片 = office.pdf.pdf2imgs
-PDF加水印 = office.pdf.add_watermark_by_parameters
-
-################# 图片 #################
-
-下载图片 = office.image.down4img
-图片加水印 = office.image.add_watermark
-
-################# Word #################
-
-Word转PDF = office.image.docx2pdf
-合并Word = office.image.merge4docx
-doc转docx = office.image.doc2docx
-docx转doc = office.image.docx2doc
-
-################# 文件 #################
-
-批量重命名 = office.file.replace4filename
-通过内容查找 = search_by_content
-拿到所有文件 = office.file.get_files
-
-################# PPT #################
-
-PPT批量转PDF = office.ppt.ppt2pdf
-
-################# 微信机器人 #################
-
-自动发信息 = office.wechat.send_message
-自动发文件 = office.wechat.send_file
+# 创建Excel = office.excel.fake2excel
+# Excel转PDF = office.excel.excel2pdf
+#
+# ################# PDF #################
+# 加密PDF = office.pdf.encrypt4pdf
+# PDF转图片 = office.pdf.pdf2imgs
+# PDF加水印 = office.pdf.add_watermark_by_parameters
+#
+# ################# 图片 #################
+#
+# 下载图片 = office.image.down4img
+# 图片加水印 = office.image.add_watermark
+#
+# ################# Word #################
+#
+# Word转PDF = office.word.docx2pdf
+# 合并Word = office.word.merge4docx
+# doc转docx = office.word.doc2docx
+# docx转doc = office.word.docx2doc
+#
+# ################# 文件 #################
+#
+# 批量重命名 = office.file.replace4filename
+# 通过内容查找 = search_by_content
+# 拿到所有文件 = office.file.get_files
+#
+# ################# PPT #################
+#
+# PPT批量转PDF = office.ppt.ppt2pdf
+#
+# ################# 微信机器人 #################
+#
+# 自动发信息 = office.wechat.send_message
+# 自动发文件 = office.wechat.send_file
```

### Comparing `pohan-0.0.5/pohan.egg-info/PKG-INFO` & `pohan-0.0.6/pohan.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pohan
-Version: 0.0.5
+Version: 0.0.6
 Summary: pip install pohan
 Home-page: https://www.python-office.com/
 Author: CoderWanFeng
 Author-email: 1957875073@qq.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CoderWanFeng/pohan/issues
 Project-URL: Documentation, https://github.com/CoderWanFeng/pohan/blob/master/README.md
```

### Comparing `pohan-0.0.5/setup.cfg` & `pohan-0.0.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 6f68 616e 0d0a 7665 7273 696f   = pohan..versio
-00000020: 6e20 3d20 302e 302e 350d 0a64 6573 6372  n = 0.0.5..descr
+00000020: 6e20 3d20 302e 302e 360d 0a64 6573 6372  n = 0.0.6..descr
 00000030: 6970 7469 6f6e 203d 2070 6970 2069 6e73  iption = pip ins
 00000040: 7461 6c6c 2070 6f68 616e 0d0a 6c6f 6e67  tall pohan..long
 00000050: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
 00000060: 696c 653a 2052 4541 444d 452e 6d64 0d0a  ile: README.md..
 00000070: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
 00000080: 5f63 6f6e 7465 6e74 5f74 7970 6520 3d20  _content_type = 
 00000090: 7465 7874 2f6d 6172 6b64 6f77 6e0d 0a75  text/markdown..u
@@ -29,15 +29,16 @@
 000001c0: 6d61 7374 6572 2f52 4541 444d 452e 6d64  master/README.md
 000001d0: 0d0a 0953 6f75 7263 6520 436f 6465 203d  ...Source Code =
 000001e0: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
 000001f0: 636f 6d2f 436f 6465 7257 616e 4665 6e67  com/CoderWanFeng
 00000200: 2f70 6f68 616e 0d0a 0d0a 5b6f 7074 696f  /pohan....[optio
 00000210: 6e73 5d0d 0a70 6163 6b61 6765 7320 3d20  ns]..packages = 
 00000220: 6669 6e64 3a0d 0a69 6e73 7461 6c6c 5f72  find:..install_r
-00000230: 6571 7569 7265 7320 3d20 0d0a 7079 7468  equires = ..pyth
-00000240: 6f6e 5f72 6571 7569 7265 7320 3d20 3e3d  on_requires = >=
-00000250: 332e 360d 0a69 6e63 6c75 6465 5f70 6163  3.6..include_pac
-00000260: 6b61 6765 5f64 6174 6120 3d20 5472 7565  kage_data = True
-00000270: 0d0a 7a69 705f 7361 6665 203d 2046 616c  ..zip_safe = Fal
-00000280: 7365 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  se....[egg_info]
-00000290: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000002a0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+00000230: 6571 7569 7265 7320 3d20 0d0a 0970 7970  equires = ...pyp
+00000240: 696e 7969 6e0d 0a70 7974 686f 6e5f 7265  inyin..python_re
+00000250: 7175 6972 6573 203d 203e 3d33 2e36 0d0a  quires = >=3.6..
+00000260: 696e 636c 7564 655f 7061 636b 6167 655f  include_package_
+00000270: 6461 7461 203d 2054 7275 650d 0a7a 6970  data = True..zip
+00000280: 5f73 6166 6520 3d20 4661 6c73 650d 0a0d  _safe = False...
+00000290: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+000002a0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+000002b0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

