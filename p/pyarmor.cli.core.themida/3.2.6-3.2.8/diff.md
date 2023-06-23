# Comparing `tmp/pyarmor.cli.core.themida-3.2.6-cp39-none-any.whl.zip` & `tmp/pyarmor.cli.core.themida-3.2.8-cp39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7975751 bytes, number of entries: 7
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-15 04:30 pyarmor/cli/core/themida/__init__.py
--rwxr-xr-x  2.0 unx  4014110 b- defN 23-Jun-15 04:30 pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx  4913168 b- defN 23-Jun-15 04:30 pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
--rw-r--r--  2.0 unx      773 b- defN 23-Jun-15 04:30 pyarmor.cli.core.themida-3.2.6.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-15 04:30 pyarmor.cli.core.themida-3.2.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-15 04:30 pyarmor.cli.core.themida-3.2.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      690 b- defN 23-Jun-15 04:30 pyarmor.cli.core.themida-3.2.6.dist-info/RECORD
-7 files, 8928864 bytes uncompressed, 7974503 bytes compressed:  10.7%
+Zip file size: 7727798 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-23 10:06 pyarmor/cli/core/themida/__init__.py
+-rwxr-xr-x  2.0 unx  3844126 b- defN 23-Jun-23 10:06 pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx  4827152 b- defN 23-Jun-23 10:06 pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
+-rw-r--r--  2.0 unx      809 b- defN 23-Jun-23 10:06 pyarmor.cli.core.themida-3.2.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-23 10:06 pyarmor.cli.core.themida-3.2.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-23 10:06 pyarmor.cli.core.themida-3.2.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      690 b- defN 23-Jun-23 10:06 pyarmor.cli.core.themida-3.2.8.dist-info/RECORD
+7 files, 8672900 bytes uncompressed, 7726550 bytes compressed:  10.9%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd
 Comment: 
 
 Filename: pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd
 Comment: 
 
-Filename: pyarmor.cli.core.themida-3.2.6.dist-info/METADATA
+Filename: pyarmor.cli.core.themida-3.2.8.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli.core.themida-3.2.6.dist-info/WHEEL
+Filename: pyarmor.cli.core.themida-3.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli.core.themida-3.2.6.dist-info/top_level.txt
+Filename: pyarmor.cli.core.themida-3.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli.core.themida-3.2.6.dist-info/RECORD
+Filename: pyarmor.cli.core.themida-3.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyarmor/cli/core/themida/__init__.py

```diff
@@ -1 +1 @@
-__VERSION__ = '3.2.6'
+__VERSION__ = '3.2.8'
```

## Comparing `pyarmor.cli.core.themida-3.2.6.dist-info/METADATA` & `pyarmor.cli.core.themida-3.2.8.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli.core.themida
-Version: 3.2.6
-Summary: Provide extension module pytransform3 for Pyarmor
+Version: 3.2.8
+Summary: Provide pre-built extension module `pyarmor_runtime` protected by Themida for Pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free To Use But Restricted
```

## Comparing `pyarmor.cli.core.themida-3.2.6.dist-info/RECORD` & `pyarmor.cli.core.themida-3.2.8.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-pyarmor/cli/core/themida/__init__.py,sha256=EEOS7QK-aUBPMbsbHCO4KWvy47RPymoUq5zl-Ijg6N8,22
-pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd,sha256=i5eQaG25MzsTq8yBDPlHd6MTlmC1A-m48FQDWPfoqwI,4014110
-pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd,sha256=j323gMj04i6CEQsjfsTuTdXLnfeA3QwKvrKMoI83cew,4913168
-pyarmor.cli.core.themida-3.2.6.dist-info/METADATA,sha256=rkBX4eLkeFTNTAQohB3deZLj3VOrup6CBBo38odezic,773
-pyarmor.cli.core.themida-3.2.6.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
-pyarmor.cli.core.themida-3.2.6.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
-pyarmor.cli.core.themida-3.2.6.dist-info/RECORD,,
+pyarmor/cli/core/themida/__init__.py,sha256=PG51kpFg0wVpa349hmCcuGnAthuwDOr30Fft4rWT9MI,22
+pyarmor/cli/core/themida/windows/x86/pyarmor_runtime.pyd,sha256=mOjCebhUKOvXeU6bFtvoo3fzHJ7s7f1s1cx8BGAX-BQ,3844126
+pyarmor/cli/core/themida/windows/x86_64/pyarmor_runtime.pyd,sha256=IGgP6ZcqHMrfN5Mcho1wpJ9_ZYjnKqq3YfdkvErbw2g,4827152
+pyarmor.cli.core.themida-3.2.8.dist-info/METADATA,sha256=GtYJfVpgdQJzhq9ASXok_caaUdEkxRsPAh1qndDcqDo,809
+pyarmor.cli.core.themida-3.2.8.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
+pyarmor.cli.core.themida-3.2.8.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
+pyarmor.cli.core.themida-3.2.8.dist-info/RECORD,,
```

