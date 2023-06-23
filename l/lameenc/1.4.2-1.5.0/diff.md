# Comparing `tmp/lameenc-1.4.2-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_24_i686.whl.zip` & `tmp/lameenc-1.5.0-pp39-pypy39_pp73-manylinux_2_5_i686.manylinux1_i686.manylinux_2_24_i686.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 163893 bytes, number of entries: 8
-drwxr-xr-x  2.0 unx        0 b- stor 22-Nov-27 12:48 lameenc.libs/
-drwxr-xr-x  2.0 unx        0 b- stor 22-Nov-27 12:48 lameenc-1.4.2.dist-info/
--rwxr-xr-x  2.0 unx   377344 b- defN 22-Nov-27 12:48 lameenc.pypy39-pp73-x86-linux-gnu.so
--rw-r--r--  2.0 unx        8 b- defN 22-Nov-27 12:48 lameenc-1.4.2.dist-info/top_level.txt
--rw-r--r--  2.0 unx      794 b- defN 22-Nov-27 12:48 lameenc-1.4.2.dist-info/METADATA
--rw-r--r--  2.0 unx    35128 b- defN 22-Nov-27 12:48 lameenc-1.4.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx      487 b- defN 22-Nov-27 12:48 lameenc-1.4.2.dist-info/RECORD
--rw-r--r--  2.0 unx      196 b- defN 22-Nov-27 12:48 lameenc-1.4.2.dist-info/WHEEL
-8 files, 413957 bytes uncompressed, 162799 bytes compressed:  60.7%
+Zip file size: 154399 bytes, number of entries: 8
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 15:13 lameenc-1.5.0.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-23 15:13 lameenc.libs/
+-rwxr-xr-x  2.0 unx   377344 b- defN 23-Jun-23 15:13 lameenc.pypy39-pp73-x86-linux-gnu.so
+-rw-rw-r--  2.0 unx      486 b- defN 23-Jun-23 15:13 lameenc-1.5.0.dist-info/RECORD
+-rw-r--r--  2.0 unx     7655 b- defN 23-Jun-23 15:13 lameenc-1.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      196 b- defN 23-Jun-23 15:13 lameenc-1.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      803 b- defN 23-Jun-23 15:13 lameenc-1.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-23 15:13 lameenc-1.5.0.dist-info/top_level.txt
+8 files, 386492 bytes uncompressed, 153305 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: lameenc.libs/
+Filename: lameenc-1.5.0.dist-info/
 Comment: 
 
-Filename: lameenc-1.4.2.dist-info/
+Filename: lameenc.libs/
 Comment: 
 
 Filename: lameenc.pypy39-pp73-x86-linux-gnu.so
 Comment: 
 
-Filename: lameenc-1.4.2.dist-info/top_level.txt
+Filename: lameenc-1.5.0.dist-info/RECORD
 Comment: 
 
-Filename: lameenc-1.4.2.dist-info/METADATA
+Filename: lameenc-1.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: lameenc-1.4.2.dist-info/LICENSE
+Filename: lameenc-1.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: lameenc-1.4.2.dist-info/RECORD
+Filename: lameenc-1.5.0.dist-info/METADATA
 Comment: 
 
-Filename: lameenc-1.4.2.dist-info/WHEEL
+Filename: lameenc-1.5.0.dist-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## lameenc.pypy39-pp73-x86-linux-gnu.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --symbols {}

```diff
@@ -505,15 +505,15 @@
     43: 000062b0   128 FUNC    LOCAL  DEFAULT   12 silence
     44: 00006330   124 FUNC    LOCAL  DEFAULT   12 setInSampleRate
     45: 000063b0   124 FUNC    LOCAL  DEFAULT   12 setBitRate
     46: 00006430   124 FUNC    LOCAL  DEFAULT   12 setQuality
     47: 000064b0   124 FUNC    LOCAL  DEFAULT   12 setChannels
     48: 000542e0    56 OBJECT  LOCAL  DEFAULT   24 lameenc_module
     49: 00054180   216 OBJECT  LOCAL  DEFAULT   24 EncoderType
-    50: 00054100     8 OBJECT  LOCAL  DEFAULT   24 EncoderClassName.10022
+    50: 00054100     8 OBJECT  LOCAL  DEFAULT   24 EncoderClassName.10101
     51: 00054260   128 OBJECT  LOCAL  DEFAULT   24 Encoder_methods
     52: 00054164     8 OBJECT  LOCAL  DEFAULT   24 module_name
     53: 00054120    68 OBJECT  LOCAL  DEFAULT   24 module_docstring
     54: 00054364    16 OBJECT  LOCAL  DEFAULT   25 module_methods
     55: 00000000     0 FILE    LOCAL  DEFAULT  ABS lame.c
     56: 00006631    93 FUNC    LOCAL  DEFAULT   12 filter_coef
     57: 0000668e   908 FUNC    LOCAL  DEFAULT   12 lame_init_params_ppflt
```

### strings --all --bytes=8 {}

```diff
@@ -898,15 +898,15 @@
 Encoder_new
 setInSampleRate
 setBitRate
 setQuality
 setChannels
 lameenc_module
 EncoderType
-EncoderClassName.10022
+EncoderClassName.10101
 Encoder_methods
 module_name
 module_docstring
 module_methods
 filter_coef
 lame_init_params_ppflt
 optimum_bandwidth
```

### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -16,15 +16,15 @@
   0x000000d0 5f646561 6c6c6f63 00456e63 6f646572 _dealloc.Encoder
   0x000000e0 5f6e6577 00736574 496e5361 6d706c65 _new.setInSample
   0x000000f0 52617465 00736574 42697452 61746500 Rate.setBitRate.
   0x00000100 73657451 75616c69 74790073 65744368 setQuality.setCh
   0x00000110 616e6e65 6c73006c 616d6565 6e635f6d annels.lameenc_m
   0x00000120 6f64756c 6500456e 636f6465 72547970 odule.EncoderTyp
   0x00000130 6500456e 636f6465 72436c61 73734e61 e.EncoderClassNa
-  0x00000140 6d652e31 30303232 00456e63 6f646572 me.10022.Encoder
+  0x00000140 6d652e31 30313031 00456e63 6f646572 me.10101.Encoder
   0x00000150 5f6d6574 686f6473 006d6f64 756c655f _methods.module_
   0x00000160 6e616d65 006d6f64 756c655f 646f6373 name.module_docs
   0x00000170 7472696e 67006d6f 64756c65 5f6d6574 tring.module_met
   0x00000180 686f6473 006c616d 652e6300 66696c74 hods.lame.c.filt
   0x00000190 65725f63 6f656600 6c616d65 5f696e69 er_coef.lame_ini
   0x000001a0 745f7061 72616d73 5f707066 6c74006f t_params_ppflt.o
   0x000001b0 7074696d 756d5f62 616e6477 69647468 ptimum_bandwidth
```

## Comparing `lameenc-1.4.2.dist-info/METADATA` & `lameenc-1.5.0.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: lameenc
-Version: 1.4.2
+Version: 1.5.0
 Summary: LAME encoding bindings
 Home-page: https://github.com/chrisstaite/lameenc
 Author: Chris Staite
 Author-email: chris@yourdreamnet.co.uk
-License: GPLv3
+License: LGPLv3
 Classifier: Topic :: Multimedia :: Sound/Audio :: Conversion
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 License-File: LICENSE
 
 
 Python 3 bindings for the LAME encoding library.
```

