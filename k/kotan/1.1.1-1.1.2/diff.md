# Comparing `tmp/kotan-1.1.1.tar.gz` & `tmp/kotan-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kotan-1.1.1.tar", max compression
+gzip compressed data, was "kotan-1.1.2.tar", max compression
```

## Comparing `kotan-1.1.1.tar` & `kotan-1.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2023-06-16 06:27:17.818625 kotan-1.1.1/README.md
--rw-r--r--   0        0        0       45 2023-06-16 08:34:32.185679 kotan-1.1.1/kotan/__init__.py
--rw-r--r--   0        0        0      749 2023-06-16 06:27:17.818625 kotan-1.1.1/kotan/const.py
--rw-r--r--   0        0        0     2727 2023-06-16 06:27:17.818625 kotan-1.1.1/kotan/job.py
--rw-r--r--   0        0        0      168 2023-06-16 06:27:17.818625 kotan-1.1.1/kotan/tasks/__init__.py
--rw-r--r--   0        0        0     5084 2023-06-16 08:34:15.725890 kotan-1.1.1/kotan/tasks/data_augmentation.py
--rw-r--r--   0        0        0     3602 2023-06-16 08:34:15.725890 kotan-1.1.1/kotan/tasks/machine_translation.py
--rw-r--r--   0        0        0     2208 2023-06-16 06:27:17.818625 kotan-1.1.1/kotan/tasks/style_convert.py
--rw-r--r--   0        0        0      344 2023-06-16 08:34:29.201717 kotan-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 kotan-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-23 05:09:04.017757 kotan-1.1.2/README.md
+-rw-r--r--   0        0        0       45 2023-06-23 05:27:14.330371 kotan-1.1.2/kotan/__init__.py
+-rw-r--r--   0        0        0      749 2023-06-23 05:09:04.017757 kotan-1.1.2/kotan/const.py
+-rw-r--r--   0        0        0     2727 2023-06-23 05:09:04.017757 kotan-1.1.2/kotan/job.py
+-rw-r--r--   0        0        0      168 2023-06-23 05:09:04.017757 kotan-1.1.2/kotan/tasks/__init__.py
+-rw-r--r--   0        0        0     5084 2023-06-23 05:09:04.017757 kotan-1.1.2/kotan/tasks/data_augmentation.py
+-rw-r--r--   0        0        0     3602 2023-06-23 05:09:04.017757 kotan-1.1.2/kotan/tasks/machine_translation.py
+-rw-r--r--   0        0        0     2226 2023-06-23 05:24:36.664203 kotan-1.1.2/kotan/tasks/style_convert.py
+-rw-r--r--   0        0        0      344 2023-06-23 05:26:56.678580 kotan-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      587 1970-01-01 00:00:00.000000 kotan-1.1.2/PKG-INFO
```

### Comparing `kotan-1.1.1/kotan/const.py` & `kotan-1.1.2/kotan/const.py`

 * *Files identical despite different names*

### Comparing `kotan-1.1.1/kotan/job.py` & `kotan-1.1.2/kotan/job.py`

 * *Files identical despite different names*

### Comparing `kotan-1.1.1/kotan/tasks/data_augmentation.py` & `kotan-1.1.2/kotan/tasks/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `kotan-1.1.1/kotan/tasks/machine_translation.py` & `kotan-1.1.2/kotan/tasks/machine_translation.py`

 * *Files identical despite different names*

### Comparing `kotan-1.1.1/kotan/tasks/style_convert.py` & `kotan-1.1.2/kotan/tasks/style_convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,19 +54,20 @@
             text (str): input text
             style (str): speech style
 
         Returns:
             output (list): Style conversion results
         """
 
-        if len(text) > 1:
+        if type(text) == type([]):
             input_text = []
             
             for txt in text:
                 input_text.append(f"{self.style} 형식으로 변환:" + txt)
+        
         else:
             input_text = f"{self.style} 형식으로 변환:" + text
 
         
         inputs = self.tokenizer(input_text, max_length=128, return_tensors="pt")["input_ids"]
             
         convert_tokens = self.model.generate(
```

### Comparing `kotan-1.1.1/PKG-INFO` & `kotan-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kotan
-Version: 1.1.1
+Version: 1.1.2
 Summary: 
 Author: jisukim
 Author-email: jisukim8873@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

