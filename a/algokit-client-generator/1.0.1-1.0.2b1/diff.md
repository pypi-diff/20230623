# Comparing `tmp/algokit_client_generator-1.0.1-py3-none-any.whl.zip` & `tmp/algokit_client_generator-1.0.2b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 18227 bytes, number of entries: 14
+Zip file size: 18295 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       91 b- defN 80-Jan-01 00:00 algokit_client_generator/__init__.py
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 algokit_client_generator/__main__.py
 -rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 algokit_client_generator/cli.py
 -rw-r--r--  2.0 unx     3199 b- defN 80-Jan-01 00:00 algokit_client_generator/document.py
 -rw-r--r--  2.0 unx    36317 b- defN 80-Jan-01 00:00 algokit_client_generator/generator.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_client_generator/py.typed
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_client_generator/spec.py
--rw-r--r--  2.0 unx     4372 b- defN 80-Jan-01 00:00 algokit_client_generator/utils.py
+-rw-r--r--  2.0 unx     4528 b- defN 80-Jan-01 00:00 algokit_client_generator/utils.py
 -rw-r--r--  2.0 unx      995 b- defN 80-Jan-01 00:00 algokit_client_generator/writer.py
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4754 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1288 b- defN 16-Jan-01 00:00 algokit_client_generator-1.0.1.dist-info/RECORD
-14 files, 62317 bytes uncompressed, 16031 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.2b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4756 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.2b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.2b1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.2b1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1298 b- defN 16-Jan-01 00:00 algokit_client_generator-1.0.2b1.dist-info/RECORD
+14 files, 62485 bytes uncompressed, 16079 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: algokit_client_generator/utils.py
 Comment: 
 
 Filename: algokit_client_generator/writer.py
 Comment: 
 
-Filename: algokit_client_generator-1.0.1.dist-info/LICENSE
+Filename: algokit_client_generator-1.0.2b1.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_client_generator-1.0.1.dist-info/METADATA
+Filename: algokit_client_generator-1.0.2b1.dist-info/METADATA
 Comment: 
 
-Filename: algokit_client_generator-1.0.1.dist-info/WHEEL
+Filename: algokit_client_generator-1.0.2b1.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_client_generator-1.0.1.dist-info/entry_points.txt
+Filename: algokit_client_generator-1.0.2b1.dist-info/entry_points.txt
 Comment: 
 
-Filename: algokit_client_generator-1.0.1.dist-info/RECORD
+Filename: algokit_client_generator-1.0.2b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_client_generator/utils.py

```diff
@@ -53,21 +53,24 @@
         case abi.StringType():
             return "str"
         case _:
             return "typing.Any"
 
 
 def map_abi_type_to_python(abi_type_str: str) -> str:
-    if abi_type_str == "void":
-        return "None"
+    match abi_type_str:
+        case "void":
+            return "None"
+        case abi.reference.ABIReferenceType.ASSET | abi.reference.ABIReferenceType.APPLICATION:
+            return "int"
+        case abi.reference.ABIReferenceType.ACCOUNT:
+            return "str | bytes"
     if abi.is_abi_transaction_type(abi_type_str):
         # TODO: generic TransactionWithSigner and/or allow unsigned types signed with signer used in transaction
         return "TransactionWithSigner"
-    if abi.is_abi_reference_type(abi_type_str):
-        return "int"
     abi_type = abi.ABIType.from_string(abi_type_str)
     return abi_type_to_python(abi_type)
 
 
 def get_unique_symbol_by_incrementing(existing_symbols: set[str], base_name: str) -> str:
     suffix = 0
     while True:
```

## Comparing `algokit_client_generator-1.0.1.dist-info/LICENSE` & `algokit_client_generator-1.0.2b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_client_generator-1.0.1.dist-info/METADATA` & `algokit_client_generator-1.0.2b1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-client-generator
-Version: 1.0.1
+Version: 1.0.2b1
 Summary: Algorand typed client Generator
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_client_generator-1.0.1.dist-info/RECORD` & `algokit_client_generator-1.0.2b1.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 algokit_client_generator/__init__.py,sha256=ikLxrMdPVjpmrVYDdHbunvzUwiXqrCdvp8Qi5x0gC0c,91
 algokit_client_generator/__main__.py,sha256=MlkUdDAWa2XH1QDdjvayVR_WaZEGkA9voNutHzWEfFo,54
 algokit_client_generator/cli.py,sha256=XwuLZUhym9ntuHRIayPZsfv2-vTSbEykt3evF7EdVq4,2550
 algokit_client_generator/document.py,sha256=X4xMvu_LfDcaosEy3AtjRoXpiLZoXRVCIoPNo8b-h08,3199
 algokit_client_generator/generator.py,sha256=kwWrqnxeEEzGbPs_4m_ZuPcpsB2kxe_CDA8UMjr78_o,36317
 algokit_client_generator/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 algokit_client_generator/spec.py,sha256=apgef1qcRbm2akT1ogF23d6HnSncPwnLdrqaVzJAKmo,7466
-algokit_client_generator/utils.py,sha256=d_HgWEJnJXmUFSULH3w97IqfpKDWiaBAUvYg0-tAhcw,4372
+algokit_client_generator/utils.py,sha256=7jWf23PWqUL5rcGDsJeIAxZGhuTT3Ucbo-Jxxbwmwgk,4528
 algokit_client_generator/writer.py,sha256=CynBYWnHlO1E4Ubcpjvzq8kRcgfYCpnO3nEAslBEr-s,995
-algokit_client_generator-1.0.1.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
-algokit_client_generator-1.0.1.dist-info/METADATA,sha256=zIniz9JcWw_4-33xpr2Nu8HAyRInFUDF9B0Rj1JmIis,4754
-algokit_client_generator-1.0.1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-algokit_client_generator-1.0.1.dist-info/entry_points.txt,sha256=RnsJToDSJC_LyXvGqv7LNpgkqipw1C7eQsc0bke--A0,67
-algokit_client_generator-1.0.1.dist-info/RECORD,,
+algokit_client_generator-1.0.2b1.dist-info/LICENSE,sha256=fkgfhUgPPyK1aS4tK9QOFRl5fWtuFEtkKx4zPQNT1bQ,1076
+algokit_client_generator-1.0.2b1.dist-info/METADATA,sha256=LyxHOW3j-C11j5ZbMSn3MmtOGtG_jpElOURVI5nGz0Y,4756
+algokit_client_generator-1.0.2b1.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+algokit_client_generator-1.0.2b1.dist-info/entry_points.txt,sha256=RnsJToDSJC_LyXvGqv7LNpgkqipw1C7eQsc0bke--A0,67
+algokit_client_generator-1.0.2b1.dist-info/RECORD,,
```

