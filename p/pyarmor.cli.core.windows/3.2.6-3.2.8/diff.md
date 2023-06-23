# Comparing `tmp/pyarmor.cli.core.windows-3.2.6-cp39-none-any.whl.zip` & `tmp/pyarmor.cli.core.windows-3.2.8-cp39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1377653 bytes, number of entries: 9
--rw-r--r--  2.0 unx       22 b- defN 23-Jun-15 04:29 pyarmor/cli/core/windows/__init__.py
--rwxr-xr-x  2.0 unx   762894 b- defN 23-Jun-15 04:29 pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx   860672 b- defN 23-Jun-15 04:29 pyarmor/cli/core/windows/x86/pytransform3.pyd
--rwxr-xr-x  2.0 unx   617472 b- defN 23-Jun-15 04:29 pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx   720896 b- defN 23-Jun-15 04:29 pyarmor/cli/core/windows/x86_64/pytransform3.pyd
--rw-r--r--  2.0 unx      773 b- defN 23-Jun-15 04:29 pyarmor.cli.core.windows-3.2.6.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-15 04:29 pyarmor.cli.core.windows-3.2.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-15 04:29 pyarmor.cli.core.windows-3.2.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      883 b- defN 23-Jun-15 04:29 pyarmor.cli.core.windows-3.2.6.dist-info/RECORD
-9 files, 2963713 bytes uncompressed, 1376099 bytes compressed:  53.6%
+Zip file size: 1382929 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       22 b- defN 23-Jun-23 10:05 pyarmor/cli/core/windows/__init__.py
+-rwxr-xr-x  2.0 unx   762894 b- defN 23-Jun-23 10:05 pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx   864768 b- defN 23-Jun-23 10:05 pyarmor/cli/core/windows/x86/pytransform3.pyd
+-rwxr-xr-x  2.0 unx   617472 b- defN 23-Jun-23 10:05 pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx   724992 b- defN 23-Jun-23 10:05 pyarmor/cli/core/windows/x86_64/pytransform3.pyd
+-rw-r--r--  2.0 unx      808 b- defN 23-Jun-23 10:05 pyarmor.cli.core.windows-3.2.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-23 10:05 pyarmor.cli.core.windows-3.2.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-23 10:05 pyarmor.cli.core.windows-3.2.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      883 b- defN 23-Jun-23 10:05 pyarmor.cli.core.windows-3.2.8.dist-info/RECORD
+9 files, 2971940 bytes uncompressed, 1381375 bytes compressed:  53.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd
 Comment: 
 
 Filename: pyarmor/cli/core/windows/x86_64/pytransform3.pyd
 Comment: 
 
-Filename: pyarmor.cli.core.windows-3.2.6.dist-info/METADATA
+Filename: pyarmor.cli.core.windows-3.2.8.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli.core.windows-3.2.6.dist-info/WHEEL
+Filename: pyarmor.cli.core.windows-3.2.8.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli.core.windows-3.2.6.dist-info/top_level.txt
+Filename: pyarmor.cli.core.windows-3.2.8.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli.core.windows-3.2.6.dist-info/RECORD
+Filename: pyarmor.cli.core.windows-3.2.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyarmor/cli/core/windows/__init__.py

```diff
@@ -1 +1 @@
-__VERSION__ = '3.2.6'
+__VERSION__ = '3.2.8'
```

## Comparing `pyarmor.cli.core.windows-3.2.6.dist-info/METADATA` & `pyarmor.cli.core.windows-3.2.8.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli.core.windows
-Version: 3.2.6
-Summary: Provide extension module pytransform3 for Pyarmor
+Version: 3.2.8
+Summary: Provide pre-built extension modules `pytransform3` and `pyarmor_runtime` for Pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free To Use But Restricted
```

## Comparing `pyarmor.cli.core.windows-3.2.6.dist-info/RECORD` & `pyarmor.cli.core.windows-3.2.8.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pyarmor/cli/core/windows/__init__.py,sha256=EEOS7QK-aUBPMbsbHCO4KWvy47RPymoUq5zl-Ijg6N8,22
-pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd,sha256=HqYecBhipSwk4oIlXSXz_kf4RqJfD0bhKWNJvsnrQjg,762894
-pyarmor/cli/core/windows/x86/pytransform3.pyd,sha256=DiUbHwOHxstkbr32m2ezmXNVQeE5MvoCDh2-bX_tWUM,860672
-pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd,sha256=voUKz_sUT48UKnMs-FuCPJn-qtc6pR8omBp34KoMgKg,617472
-pyarmor/cli/core/windows/x86_64/pytransform3.pyd,sha256=0RFTLDDOaHi8X_VxaCPoaetyAb2C7v_eVuHwgToA0L8,720896
-pyarmor.cli.core.windows-3.2.6.dist-info/METADATA,sha256=V9CNz6Qlx3wkYlwVV6uI6D_c-9yYCPuo_DGr4_-fTQs,773
-pyarmor.cli.core.windows-3.2.6.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
-pyarmor.cli.core.windows-3.2.6.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
-pyarmor.cli.core.windows-3.2.6.dist-info/RECORD,,
+pyarmor/cli/core/windows/__init__.py,sha256=PG51kpFg0wVpa349hmCcuGnAthuwDOr30Fft4rWT9MI,22
+pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd,sha256=In0VDR4Ds-WjH6mU86ZU-bxzFoDwAg-xjkFT5h5nTtE,762894
+pyarmor/cli/core/windows/x86/pytransform3.pyd,sha256=G8nM1qfGXoUV0ZoCWRBc3Cl86c7EdUkCezBtgWtBzlM,864768
+pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd,sha256=0-xE0YDYlJ5HGYP0Fq6nB6Y4-aB1UWbGjdU8PSOJb68,617472
+pyarmor/cli/core/windows/x86_64/pytransform3.pyd,sha256=oRW7J_wY3y3_J221k_x0kR6m0bAzYzLW2APCAulAhC8,724992
+pyarmor.cli.core.windows-3.2.8.dist-info/METADATA,sha256=u4IKJhCuPsbRpqNlOTIJfd1DID8ohOL19rpBWkSXmNU,808
+pyarmor.cli.core.windows-3.2.8.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
+pyarmor.cli.core.windows-3.2.8.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
+pyarmor.cli.core.windows-3.2.8.dist-info/RECORD,,
```

