# Comparing `tmp/fastervit-0.8.8.tar.gz` & `tmp/fastervit-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-0qqt6cya/fastervit-0.8.8.tar", last modified: Wed Jun 21 01:50:06 2023, max compression
+gzip compressed data, was "/home/ali/Desktop/Gitlab_repos/FasterViT_pip_test/dist/.tmp-fhq3blvm/fastervit-0.8.9.tar", last modified: Fri Jun 23 00:41:06 2023, max compression
```

## Comparing `fastervit-0.8.8.tar` & `fastervit-0.8.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-21 01:50:06.000000 fastervit-0.8.8/
--rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-06-21 01:30:26.000000 fastervit-0.8.8/LICENSE
--rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-06-21 01:30:26.000000 fastervit-0.8.8/MANIFEST.in
--rw-rw-r--   0 ali       (1000) ali       (1000)     9390 2023-06-21 01:50:06.000000 fastervit-0.8.8/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)     8440 2023-06-21 01:49:57.000000 fastervit-0.8.8/README.md
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-21 01:50:06.000000 fastervit-0.8.8/fastervit/
--rw-rw-r--   0 ali       (1000) ali       (1000)       41 2023-06-21 01:30:26.000000 fastervit-0.8.8/fastervit/__init__.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-21 01:50:06.000000 fastervit-0.8.8/fastervit/assets/
--rw-rw-r--   0 ali       (1000) ali       (1000)   100537 2023-06-21 01:30:26.000000 fastervit-0.8.8/fastervit/assets/hierarchial_attn.png
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-21 01:50:06.000000 fastervit-0.8.8/fastervit/models/
--rw-rw-r--   0 ali       (1000) ali       (1000)       96 2023-06-21 01:30:26.000000 fastervit-0.8.8/fastervit/models/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    47103 2023-06-21 01:34:03.000000 fastervit-0.8.8/fastervit/models/faster_vit.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    48860 2023-06-21 01:36:32.000000 fastervit-0.8.8/fastervit/models/faster_vit_any_res.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     7844 2023-06-21 01:32:20.000000 fastervit-0.8.8/fastervit/models/registry.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-21 01:50:06.000000 fastervit-0.8.8/fastervit/scheduler/
--rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-06-21 01:30:26.000000 fastervit-0.8.8/fastervit/scheduler/__init__.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-06-21 01:30:26.000000 fastervit-0.8.8/fastervit/scheduler/cosine_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-06-21 01:30:26.000000 fastervit-0.8.8/fastervit/scheduler/multistep_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-06-21 01:30:26.000000 fastervit-0.8.8/fastervit/scheduler/plateau_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-06-21 01:30:26.000000 fastervit-0.8.8/fastervit/scheduler/poly_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-06-21 01:30:26.000000 fastervit-0.8.8/fastervit/scheduler/scheduler.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-06-21 01:30:26.000000 fastervit-0.8.8/fastervit/scheduler/scheduler_factory.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-06-21 01:30:26.000000 fastervit-0.8.8/fastervit/scheduler/step_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-06-21 01:30:26.000000 fastervit-0.8.8/fastervit/scheduler/tanh_lr.py
--rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-06-21 01:30:26.000000 fastervit-0.8.8/fastervit/tensorboard.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    49797 2023-06-21 01:30:26.000000 fastervit-0.8.8/fastervit/train.py
--rw-rw-r--   0 ali       (1000) ali       (1000)    16145 2023-06-21 01:30:26.000000 fastervit-0.8.8/fastervit/validate.py
-drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-21 01:50:06.000000 fastervit-0.8.8/fastervit.egg-info/
--rw-rw-r--   0 ali       (1000) ali       (1000)     9390 2023-06-21 01:50:06.000000 fastervit-0.8.8/fastervit.egg-info/PKG-INFO
--rw-rw-r--   0 ali       (1000) ali       (1000)      768 2023-06-21 01:50:06.000000 fastervit-0.8.8/fastervit.egg-info/SOURCES.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-06-21 01:50:06.000000 fastervit-0.8.8/fastervit.egg-info/dependency_links.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-06-21 01:50:06.000000 fastervit-0.8.8/fastervit.egg-info/requires.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-06-21 01:50:06.000000 fastervit-0.8.8/fastervit.egg-info/top_level.txt
--rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-06-21 01:50:06.000000 fastervit-0.8.8/setup.cfg
--rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-06-21 01:31:44.000000 fastervit-0.8.8/setup.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-23 00:41:06.000000 fastervit-0.8.9/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4146 2023-06-21 01:30:26.000000 fastervit-0.8.9/LICENSE
+-rw-rw-r--   0 ali       (1000) ali       (1000)       45 2023-06-21 01:30:26.000000 fastervit-0.8.9/MANIFEST.in
+-rw-rw-r--   0 ali       (1000) ali       (1000)     9830 2023-06-23 00:41:06.000000 fastervit-0.8.9/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)     8880 2023-06-23 00:40:23.000000 fastervit-0.8.9/README.md
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       41 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/__init__.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit/assets/
+-rw-rw-r--   0 ali       (1000) ali       (1000)   100537 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/assets/hierarchial_attn.png
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit/models/
+-rw-rw-r--   0 ali       (1000) ali       (1000)       96 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/models/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    47039 2023-06-23 00:32:18.000000 fastervit-0.8.9/fastervit/models/faster_vit.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    48796 2023-06-23 00:29:36.000000 fastervit-0.8.9/fastervit/models/faster_vit_any_res.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     7844 2023-06-21 01:32:20.000000 fastervit-0.8.9/fastervit/models/registry.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit/scheduler/
+-rw-rw-r--   0 ali       (1000) ali       (1000)      291 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/__init__.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4161 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/cosine_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     2098 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/multistep_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3457 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/plateau_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     4003 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/poly_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     5095 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/scheduler.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3907 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/scheduler_factory.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1902 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/step_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)     3936 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/scheduler/tanh_lr.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)      734 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/tensorboard.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    49797 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/train.py
+-rw-rw-r--   0 ali       (1000) ali       (1000)    16145 2023-06-21 01:30:26.000000 fastervit-0.8.9/fastervit/validate.py
+drwxrwxr-x   0 ali       (1000) ali       (1000)        0 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit.egg-info/
+-rw-rw-r--   0 ali       (1000) ali       (1000)     9830 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit.egg-info/PKG-INFO
+-rw-rw-r--   0 ali       (1000) ali       (1000)      768 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)        1 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       32 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit.egg-info/requires.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)       10 2023-06-23 00:41:06.000000 fastervit-0.8.9/fastervit.egg-info/top_level.txt
+-rw-rw-r--   0 ali       (1000) ali       (1000)      126 2023-06-23 00:41:06.000000 fastervit-0.8.9/setup.cfg
+-rw-rw-r--   0 ali       (1000) ali       (1000)     1549 2023-06-23 00:40:56.000000 fastervit-0.8.9/setup.py
```

### Comparing `fastervit-0.8.8/LICENSE` & `fastervit-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.8/PKG-INFO` & `fastervit-0.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6661 7374  : 2.1.Name: fast
 00000020: 6572 7669 740a 5665 7273 696f 6e3a 2030  ervit.Version: 0
-00000030: 2e38 2e38 0a53 756d 6d61 7279 3a20 4661  .8.8.Summary: Fa
+00000030: 2e38 2e39 0a53 756d 6d61 7279 3a20 4661  .8.9.Summary: Fa
 00000040: 7374 6572 5669 543a 2046 6173 7420 5669  sterViT: Fast Vi
 00000050: 7369 6f6e 2054 7261 6e73 666f 726d 6572  sion Transformer
 00000060: 7320 7769 7468 2048 6965 7261 7263 6869  s with Hierarchi
 00000070: 6361 6c20 4174 7465 6e74 696f 6e0a 486f  cal Attention.Ho
 00000080: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 00000090: 2f67 6974 6875 622e 636f 6d2f 4e56 6c61  /github.com/NVla
 000000a0: 6273 2f46 6173 7465 7256 6954 0a41 7574  bs/FasterViT.Aut
@@ -108,480 +108,508 @@
 000006b0: 0a0a 2d2d 2d20 0a0a 4661 7374 6572 5669  ..--- ..FasterVi
 000006c0: 5420 6163 6869 6576 6573 2061 206e 6577  T achieves a new
 000006d0: 2053 4f54 4120 5061 7265 746f 2d66 726f   SOTA Pareto-fro
 000006e0: 6e74 2069 6e0a 7465 726d 7320 6f66 2061  nt in.terms of a
 000006f0: 6363 7572 6163 7920 7673 2e20 696d 6167  ccuracy vs. imag
 00000700: 6520 7468 726f 7567 6870 7574 2028 6e6f  e throughput (no
 00000710: 2065 7874 7261 2074 7261 696e 696e 6720   extra training 
-00000720: 6461 7461 2021 290a 0a21 5b74 6561 7365  data !)..![tease
-00000730: 725d 282e 2f66 6173 7465 7276 6974 2f61  r](./fastervit/a
-00000740: 7373 6574 732f 706c 6f74 2e70 6e67 290a  ssets/plot.png).
-00000750: 0a0a 0a23 2320 f09f 92a5 204e 6577 7320  ...## .... News 
-00000760: f09f 92a5 0a0a 2d20 2a2a 5b30 362e 3138  ......- **[06.18
-00000770: 2e32 3032 335d 2a2a 20f0 9f94 a520 5765  .2023]** .... We
-00000780: 2068 6176 6520 7265 6c65 6173 6564 2074   have released t
-00000790: 6865 2046 6173 7465 7256 6954 205b 7069  he FasterViT [pi
-000007a0: 7020 7061 636b 6167 655d 2868 7474 7073  p package](https
-000007b0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-000007c0: 6563 742f 6661 7374 6572 7669 742f 2920  ect/fastervit/) 
-000007d0: 210a 2d20 2a2a 5b30 362e 3137 2e32 3032  !.- **[06.17.202
-000007e0: 335d 2a2a 20f0 9f94 a520 5b41 6e79 2d72  3]** .... [Any-r
-000007f0: 6573 6f6c 7574 696f 6e20 4661 7374 6572  esolution Faster
-00000800: 5669 545d 282e 2f66 6173 7465 7276 6974  ViT](./fastervit
-00000810: 2f6d 6f64 656c 732f 6661 7374 6572 5f76  /models/faster_v
-00000820: 6974 5f61 6e79 5f72 6573 2e70 7929 2020  it_any_res.py)  
-00000830: 6d6f 6465 6c20 6973 206e 6f77 2061 7661  model is now ava
-00000840: 696c 6162 6c65 2021 2074 6865 206d 6f64  ilable ! the mod
-00000850: 656c 2063 616e 2062 6520 7573 6564 2066  el can be used f
-00000860: 6f72 2076 6172 6965 7479 206f 6620 6170  or variety of ap
-00000870: 706c 6963 6174 696f 6e73 2073 7563 6820  plications such 
-00000880: 6173 2064 6574 6563 7469 6f6e 2061 6e64  as detection and
-00000890: 2073 6567 6d65 6e74 6174 696f 6e20 6f72   segmentation or
-000008a0: 2068 6967 682d 7265 736f 6c75 7469 6f6e   high-resolution
-000008b0: 2066 696e 652d 7475 6e69 6e67 2077 6974   fine-tuning wit
-000008c0: 6820 6172 6269 7472 6172 7920 696e 7075  h arbitrary inpu
-000008d0: 7420 696d 6167 6520 7265 736f 6c75 7469  t image resoluti
-000008e0: 6f6e 732e 200a 2d20 2a2a 5b30 362e 3039  ons. .- **[06.09
-000008f0: 2e32 3032 335d 2a2a 20f0 9f94 a5f0 9f94  .2023]** .......
-00000900: a520 5765 2068 6176 6520 7265 6c65 6173  . We have releas
-00000910: 6564 2073 6f75 7263 6520 636f 6465 2061  ed source code a
-00000920: 6e64 2049 6d61 6765 4e65 742d 314b 2046  nd ImageNet-1K F
-00000930: 6173 7465 7256 6954 2d6d 6f64 656c 7320  asterViT-models 
-00000940: 210a 0a23 2320 5175 6963 6b20 5374 6172  !..## Quick Star
-00000950: 740a 0a54 6865 2046 6173 7465 7256 6954  t..The FasterViT
-00000960: 2063 616e 2062 6520 636f 6e76 656e 6965   can be convenie
-00000970: 6e74 6c79 2069 6e73 7461 6c6c 6564 2062  ntly installed b
-00000980: 793a 0a0a 6060 6062 6173 680a 7069 7020  y:..```bash.pip 
-00000990: 696e 7374 616c 6c20 6661 7374 6572 7669  install fastervi
-000009a0: 740a 6060 600a 0a41 2046 6173 7465 7256  t.```..A FasterV
-000009b0: 6954 206d 6f64 656c 2077 6974 6820 6465  iT model with de
-000009c0: 6661 756c 7420 6879 7065 722d 7061 7261  fault hyper-para
-000009d0: 6d65 7465 7273 2063 616e 2062 6520 6372  meters can be cr
-000009e0: 6561 7465 6420 6173 2069 6e20 7468 6520  eated as in the 
-000009f0: 666f 6c6c 6f77 696e 673a 0a0a 6060 6070  following:..```p
-00000a00: 7974 686f 6e0a 3e3e 3e20 6672 6f6d 2066  ython.>>> from f
-00000a10: 6173 7465 7276 6974 2069 6d70 6f72 7420  astervit import 
-00000a20: 6372 6561 7465 5f6d 6f64 656c 0a0a 2320  create_model..# 
-00000a30: 4465 6669 6e65 2066 6173 7465 7276 6974  Define fastervit
-00000a40: 2d30 206d 6f64 656c 2077 6974 6820 3232  -0 model with 22
-00000a50: 3420 7820 3232 3420 7265 736f 6c75 7469  4 x 224 resoluti
-00000a60: 6f6e 0a3e 3e3e 206d 6f64 656c 203d 2063  on.>>> model = c
-00000a70: 7265 6174 655f 6d6f 6465 6c28 2766 6173  reate_model('fas
-00000a80: 7465 725f 7669 745f 305f 3232 3427 290a  ter_vit_0_224').
-00000a90: 6060 600a 0a57 6520 6361 6e20 616c 736f  ```..We can also
-00000aa0: 2075 7365 2074 6865 2061 6e79 2d72 6573   use the any-res
-00000ab0: 6f6c 7574 696f 6e20 4661 7374 6572 5669  olution FasterVi
-00000ac0: 5420 6d6f 6465 6c20 746f 2061 6363 6f6d  T model to accom
-00000ad0: 6d6f 6461 7465 2061 7262 6974 7261 7279  modate arbitrary
-00000ae0: 2069 6d61 6765 2072 6573 6f6c 7574 696f   image resolutio
-00000af0: 6e73 2e20 496e 2074 6865 2066 6f6c 6c6f  ns. In the follo
-00000b00: 7769 6e67 2c20 7765 2064 6566 696e 6520  wing, we define 
-00000b10: 616e 2061 6e79 2d72 6573 6f6c 7574 696f  an any-resolutio
-00000b20: 6e20 4661 7374 6572 5669 542d 310a 6d6f  n FasterViT-1.mo
-00000b30: 6465 6c20 7769 7468 2069 6e70 7574 2072  del with input r
-00000b40: 6573 6f6c 7574 696f 6e20 6f66 2035 3736  esolution of 576
-00000b50: 2078 2039 3630 2c20 7769 6e64 6f77 2073   x 960, window s
-00000b60: 697a 6573 206f 6620 3132 2061 6e64 2036  izes of 12 and 6
-00000b70: 2069 6e20 3372 6420 616e 6420 3474 6820   in 3rd and 4th 
-00000b80: 7374 6167 6573 2c20 6361 7272 6965 7220  stages, carrier 
-00000b90: 746f 6b65 6e20 7369 7a65 206f 6620 3220  token size of 2 
-00000ba0: 616e 6420 656d 6265 6464 696e 6720 6469  and embedding di
-00000bb0: 6d65 6e73 696f 6e20 6f66 0a31 3238 3a0a  mension of.128:.
-00000bc0: 0a60 6060 7079 7468 6f6e 0a3e 3e3e 2066  .```python.>>> f
-00000bd0: 726f 6d20 6661 7374 6572 7669 7420 696d  rom fastervit im
-00000be0: 706f 7274 2063 7265 6174 655f 6d6f 6465  port create_mode
-00000bf0: 6c0a 0a23 2044 6566 696e 6520 616e 792d  l..# Define any-
-00000c00: 7265 736f 6c75 7469 6f6e 2046 6173 7465  resolution Faste
-00000c10: 7256 6954 2d31 206d 6f64 656c 2077 6974  rViT-1 model wit
-00000c20: 6820 3537 3620 7820 3936 3020 7265 736f  h 576 x 960 reso
-00000c30: 6c75 7469 6f6e 0a3e 3e3e 206d 6f64 656c  lution.>>> model
-00000c40: 203d 2063 7265 6174 655f 6d6f 6465 6c28   = create_model(
-00000c50: 2766 6173 7465 725f 7669 745f 315f 616e  'faster_vit_1_an
-00000c60: 795f 7265 7327 2c20 0a20 2020 2020 2020  y_res', .       
-00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c80: 2020 2072 6573 6f6c 7574 696f 6e3d 5b35     resolution=[5
-00000c90: 3736 2c20 3936 305d 2c0a 2020 2020 2020  76, 960],.      
-00000ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cb0: 2020 2020 7769 6e64 6f77 5f73 697a 653d      window_size=
-00000cc0: 5b37 2c20 372c 2031 322c 2036 5d2c 0a20  [7, 7, 12, 6],. 
-00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ce0: 2020 2020 2020 2020 2063 745f 7369 7a65           ct_size
-00000cf0: 3d32 2c0a 2020 2020 2020 2020 2020 2020  =2,.            
-00000d00: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00000d10: 6d3d 3132 3829 0a60 6060 0a0a 2323 2043  m=128).```..## C
-00000d20: 6174 616c 6f67 0a2d 205b 785d 2049 6d61  atalog.- [x] Ima
-00000d30: 6765 4e65 742d 314b 2074 7261 696e 696e  geNet-1K trainin
-00000d40: 6720 636f 6465 0a2d 205b 785d 2049 6d61  g code.- [x] Ima
-00000d50: 6765 4e65 742d 314b 2070 7265 2d74 7261  geNet-1K pre-tra
-00000d60: 696e 6564 206d 6f64 656c 730a 2d20 5b78  ined models.- [x
-00000d70: 5d20 416e 792d 7265 736f 6c75 7469 6f6e  ] Any-resolution
-00000d80: 2046 6173 7465 7256 6954 0a2d 205b 785d   FasterViT.- [x]
-00000d90: 2046 6173 7465 7256 6954 2070 6970 2d70   FasterViT pip-p
-00000da0: 6163 6b61 6765 2072 656c 6561 7365 0a2d  ackage release.-
-00000db0: 205b 205d 2049 6d61 6765 4e65 742d 3231   [ ] ImageNet-21
-00000dc0: 4b20 7072 652d 7472 6169 6e65 6420 6d6f  K pre-trained mo
-00000dd0: 6465 6c73 0a2d 205b 205d 2049 6d61 6765  dels.- [ ] Image
-00000de0: 4e65 742d 3231 4b20 6669 6e65 2d74 756e  Net-21K fine-tun
-00000df0: 6520 7363 7269 7074 730a 2d20 5b20 5d20  e scripts.- [ ] 
-00000e00: 4465 7465 6374 696f 6e20 636f 6465 2028  Detection code (
-00000e10: 4449 4e4f 2920 2b20 6d6f 6465 6c73 0a2d  DINO) + models.-
-00000e20: 205b 205d 2053 6567 6d65 6e74 6174 696f   [ ] Segmentatio
-00000e30: 6e20 636f 6465 202b 206d 6f64 656c 730a  n code + models.
-00000e40: 0a2d 2d2d 200a 0a23 2320 5265 7375 6c74  .--- ..## Result
-00000e50: 7320 2b20 5072 6574 7261 696e 6564 204d  s + Pretrained M
-00000e60: 6f64 656c 730a 0a23 2323 2049 6d61 6765  odels..### Image
-00000e70: 4e65 742d 314b 0a2a 2a46 6173 7465 7256  Net-1K.**FasterV
-00000e80: 6954 2049 6d61 6765 4e65 742d 314b 2050  iT ImageNet-1K P
-00000e90: 7265 7472 6169 6e65 6420 4d6f 6465 6c73  retrained Models
-00000ea0: 2a2a 0a0a 3c74 6162 6c65 3e0a 2020 3c74  **..<table>.  <t
-00000eb0: 723e 0a20 2020 203c 7468 3e4e 616d 653c  r>.    <th>Name<
-00000ec0: 2f74 683e 0a20 2020 203c 7468 3e41 6363  /th>.    <th>Acc
-00000ed0: 4031 2825 293c 2f74 683e 0a20 2020 203c  @1(%)</th>.    <
-00000ee0: 7468 3e41 6363 4035 2825 293c 2f74 683e  th>Acc@5(%)</th>
-00000ef0: 0a20 2020 203c 7468 3e54 6872 6f75 6768  .    <th>Through
-00000f00: 7075 7428 496d 672f 5365 6329 3c2f 7468  put(Img/Sec)</th
-00000f10: 3e0a 2020 2020 3c74 683e 5265 736f 6c75  >.    <th>Resolu
-00000f20: 7469 6f6e 3c2f 7468 3e0a 2020 2020 3c74  tion</th>.    <t
-00000f30: 683e 2350 6172 616d 7328 4d29 3c2f 7468  h>#Params(M)</th
-00000f40: 3e0a 2020 2020 3c74 683e 464c 4f50 7328  >.    <th>FLOPs(
-00000f50: 4729 3c2f 7468 3e0a 2020 2020 3c74 683e  G)</th>.    <th>
-00000f60: 446f 776e 6c6f 6164 3c2f 7468 3e0a 2020  Download</th>.  
-00000f70: 3c2f 7472 3e0a 0a3c 7472 3e0a 2020 2020  </tr>..<tr>.    
-00000f80: 3c74 643e 4661 7374 6572 5669 542d 303c  <td>FasterViT-0<
-00000f90: 2f74 643e 0a20 2020 203c 7464 3e38 322e  /td>.    <td>82.
-00000fa0: 313c 2f74 643e 0a20 2020 203c 7464 3e39  1</td>.    <td>9
-00000fb0: 352e 393c 2f74 643e 0a20 2020 203c 7464  5.9</td>.    <td
-00000fc0: 3e35 3830 323c 2f74 643e 0a20 2020 203c  >5802</td>.    <
-00000fd0: 7464 3e32 3234 7832 3234 3c2f 7464 3e0a  td>224x224</td>.
-00000fe0: 2020 2020 3c74 643e 3331 2e34 3c2f 7464      <td>31.4</td
-00000ff0: 3e0a 2020 2020 3c74 643e 332e 333c 2f74  >.    <td>3.3</t
-00001000: 643e 0a20 2020 203c 7464 3e3c 6120 6872  d>.    <td><a hr
-00001010: 6566 3d22 6874 7470 733a 2f2f 6472 6976  ef="https://driv
-00001020: 652e 676f 6f67 6c65 2e63 6f6d 2f75 633f  e.google.com/uc?
-00001030: 6578 706f 7274 3d64 6f77 6e6c 6f61 6426  export=download&
-00001040: 6964 3d31 7477 4932 4c46 4a73 3339 3159  id=1twI2LFJs391Y
-00001050: 726a 384d 5234 5569 3950 6672 7657 716a  rj8MR4Ui9PfrvWqj
-00001060: 4531 6942 223e 6d6f 6465 6c3c 2f61 3e3c  E1iB">model</a><
-00001070: 2f74 643e 0a3c 2f74 723e 0a0a 3c74 723e  /td>.</tr>..<tr>
-00001080: 0a20 2020 203c 7464 3e46 6173 7465 7256  .    <td>FasterV
-00001090: 6954 2d31 3c2f 7464 3e0a 2020 2020 3c74  iT-1</td>.    <t
-000010a0: 643e 3833 2e32 3c2f 7464 3e0a 2020 2020  d>83.2</td>.    
-000010b0: 3c74 643e 3936 2e35 3c2f 7464 3e0a 2020  <td>96.5</td>.  
-000010c0: 2020 3c74 643e 3431 3838 3c2f 7464 3e0a    <td>4188</td>.
-000010d0: 2020 2020 3c74 643e 3232 3478 3232 343c      <td>224x224<
-000010e0: 2f74 643e 0a20 2020 203c 7464 3e35 332e  /td>.    <td>53.
-000010f0: 343c 2f74 643e 0a20 2020 203c 7464 3e35  4</td>.    <td>5
-00001100: 2e33 3c2f 7464 3e0a 2020 2020 3c74 643e  .3</td>.    <td>
-00001110: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001120: 2f64 7269 7665 2e67 6f6f 676c 652e 636f  /drive.google.co
-00001130: 6d2f 7563 3f65 7870 6f72 743d 646f 776e  m/uc?export=down
-00001140: 6c6f 6164 2669 643d 3172 3757 3130 6e35  load&id=1r7W10n5
-00001150: 2d62 4674 4d33 737a 3462 6d61 4c72 6f77  -bFtM3sz4bmaLrow
-00001160: 4e32 6759 506b 4c47 5422 3e6d 6f64 656c  N2gYPkLGT">model
-00001170: 3c2f 613e 3c2f 7464 3e0a 3c2f 7472 3e0a  </a></td>.</tr>.
-00001180: 0a3c 7472 3e0a 2020 2020 3c74 643e 4661  .<tr>.    <td>Fa
-00001190: 7374 6572 5669 542d 323c 2f74 643e 0a20  sterViT-2</td>. 
-000011a0: 2020 203c 7464 3e38 342e 323c 2f74 643e     <td>84.2</td>
-000011b0: 0a20 2020 203c 7464 3e39 362e 383c 2f74  .    <td>96.8</t
-000011c0: 643e 0a20 2020 203c 7464 3e33 3136 313c  d>.    <td>3161<
-000011d0: 2f74 643e 0a20 2020 203c 7464 3e32 3234  /td>.    <td>224
-000011e0: 7832 3234 3c2f 7464 3e0a 2020 2020 3c74  x224</td>.    <t
-000011f0: 643e 3735 2e39 3c2f 7464 3e0a 2020 2020  d>75.9</td>.    
-00001200: 3c74 643e 382e 373c 2f74 643e 0a20 2020  <td>8.7</td>.   
-00001210: 203c 7464 3e3c 6120 6872 6566 3d22 6874   <td><a href="ht
-00001220: 7470 733a 2f2f 6472 6976 652e 676f 6f67  tps://drive.goog
-00001230: 6c65 2e63 6f6d 2f75 633f 6578 706f 7274  le.com/uc?export
-00001240: 3d64 6f77 6e6c 6f61 6426 6964 3d31 6e5f  =download&id=1n_
-00001250: 6136 7330 7067 6930 6a56 5a4f 476d 4465  a6s0pgi0jVZOGmDe
-00001260: 6932 7658 4855 3545 3652 4835 7755 223e  i2vXHU5E6RH5wU">
-00001270: 6d6f 6465 6c3c 2f61 3e3c 2f74 643e 0a3c  model</a></td>.<
-00001280: 2f74 723e 0a0a 3c74 723e 0a20 2020 203c  /tr>..<tr>.    <
-00001290: 7464 3e46 6173 7465 7256 6954 2d33 3c2f  td>FasterViT-3</
-000012a0: 7464 3e0a 2020 2020 3c74 643e 3834 2e39  td>.    <td>84.9
-000012b0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3937  </td>.    <td>97
-000012c0: 2e32 3c2f 7464 3e0a 2020 2020 3c74 643e  .2</td>.    <td>
-000012d0: 3137 3830 3c2f 7464 3e0a 2020 2020 3c74  1780</td>.    <t
-000012e0: 643e 3232 3478 3232 343c 2f74 643e 0a20  d>224x224</td>. 
-000012f0: 2020 203c 7464 3e31 3539 2e35 3c2f 7464     <td>159.5</td
-00001300: 3e0a 2020 2020 3c74 643e 3138 2e32 3c2f  >.    <td>18.2</
-00001310: 7464 3e0a 2020 2020 3c74 643e 3c61 2068  td>.    <td><a h
-00001320: 7265 663d 2268 7474 7073 3a2f 2f64 7269  ref="https://dri
-00001330: 7665 2e67 6f6f 676c 652e 636f 6d2f 7563  ve.google.com/uc
-00001340: 3f65 7870 6f72 743d 646f 776e 6c6f 6164  ?export=download
-00001350: 2669 643d 3174 7657 456c 5a39 3153 6961  &id=1tvWElZ91Sia
-00001360: 3253 7358 5958 464d 4e59 5177 6669 7043  2SsXYXFMNYQwfipC
-00001370: 7874 4937 5822 3e6d 6f64 656c 3c2f 613e  xtI7X">model</a>
-00001380: 3c2f 7464 3e0a 3c2f 7472 3e0a 0a3c 7472  </td>.</tr>..<tr
-00001390: 3e0a 2020 2020 3c74 643e 4661 7374 6572  >.    <td>Faster
-000013a0: 5669 542d 343c 2f74 643e 0a20 2020 203c  ViT-4</td>.    <
-000013b0: 7464 3e38 352e 343c 2f74 643e 0a20 2020  td>85.4</td>.   
-000013c0: 203c 7464 3e39 372e 333c 2f74 643e 0a20   <td>97.3</td>. 
-000013d0: 2020 203c 7464 3e38 3439 3c2f 7464 3e0a     <td>849</td>.
-000013e0: 2020 2020 3c74 643e 3232 3478 3232 343c      <td>224x224<
-000013f0: 2f74 643e 0a20 2020 203c 7464 3e34 3234  /td>.    <td>424
-00001400: 2e36 3c2f 7464 3e0a 2020 2020 3c74 643e  .6</td>.    <td>
-00001410: 3336 2e36 3c2f 7464 3e0a 2020 2020 3c74  36.6</td>.    <t
-00001420: 643e 3c61 2068 7265 663d 2268 7474 7073  d><a href="https
-00001430: 3a2f 2f64 7269 7665 2e67 6f6f 676c 652e  ://drive.google.
-00001440: 636f 6d2f 7563 3f65 7870 6f72 743d 646f  com/uc?export=do
-00001450: 776e 6c6f 6164 2669 643d 3167 5968 5841  wnload&id=1gYhXA
-00001460: 3332 512d 5f39 4335 4458 656c 3137 6176  32Q-_9C5DXel17av
-00001470: 565f 5a4c 6f61 4877 6467 7a22 3e6d 6f64  V_ZLoaHwdgz">mod
-00001480: 656c 3c2f 613e 3c2f 7464 3e0a 3c2f 7472  el</a></td>.</tr
-00001490: 3e0a 0a3c 7472 3e0a 2020 2020 3c74 643e  >..<tr>.    <td>
-000014a0: 4661 7374 6572 5669 542d 353c 2f74 643e  FasterViT-5</td>
-000014b0: 0a20 2020 203c 7464 3e38 352e 363c 2f74  .    <td>85.6</t
-000014c0: 643e 0a20 2020 203c 7464 3e39 372e 343c  d>.    <td>97.4<
-000014d0: 2f74 643e 0a20 2020 203c 7464 3e34 3439  /td>.    <td>449
-000014e0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3232  </td>.    <td>22
-000014f0: 3478 3232 343c 2f74 643e 0a20 2020 203c  4x224</td>.    <
-00001500: 7464 3e39 3735 2e35 3c2f 7464 3e0a 2020  td>975.5</td>.  
-00001510: 2020 3c74 643e 3131 332e 303c 2f74 643e    <td>113.0</td>
-00001520: 0a20 2020 203c 7464 3e3c 6120 6872 6566  .    <td><a href
-00001530: 3d22 6874 7470 733a 2f2f 6472 6976 652e  ="https://drive.
-00001540: 676f 6f67 6c65 2e63 6f6d 2f75 633f 6578  google.com/uc?ex
-00001550: 706f 7274 3d64 6f77 6e6c 6f61 6426 6964  port=download&id
-00001560: 3d31 6d71 7061 6937 5869 484c 725f 6e31  =1mqpai7XiHLr_n1
-00001570: 746a 786a 7a54 3871 3336 3978 5443 715f  tjxjzT8q369xTCq_
-00001580: 7a2d 223e 6d6f 6465 6c3c 2f61 3e3c 2f74  z-">model</a></t
-00001590: 643e 0a3c 2f74 723e 0a0a 3c74 723e 0a20  d>.</tr>..<tr>. 
-000015a0: 2020 203c 7464 3e46 6173 7465 7256 6954     <td>FasterViT
-000015b0: 2d36 3c2f 7464 3e0a 2020 2020 3c74 643e  -6</td>.    <td>
-000015c0: 3835 2e38 3c2f 7464 3e0a 2020 2020 3c74  85.8</td>.    <t
-000015d0: 643e 3937 2e34 3c2f 7464 3e0a 2020 2020  d>97.4</td>.    
-000015e0: 3c74 643e 3335 323c 2f74 643e 0a20 2020  <td>352</td>.   
-000015f0: 203c 7464 3e32 3234 7832 3234 3c2f 7464   <td>224x224</td
-00001600: 3e0a 2020 2020 3c74 643e 3133 3630 2e30  >.    <td>1360.0
-00001610: 3c2f 7464 3e0a 2020 2020 3c74 643e 3134  </td>.    <td>14
-00001620: 322e 303c 2f74 643e 0a20 2020 203c 7464  2.0</td>.    <td
-00001630: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
-00001640: 2f2f 6472 6976 652e 676f 6f67 6c65 2e63  //drive.google.c
-00001650: 6f6d 2f75 633f 6578 706f 7274 3d64 6f77  om/uc?export=dow
-00001660: 6e6c 6f61 6426 6964 3d31 326a 7461 7652  nload&id=12jtavR
-00001670: 3251 786d 4d7a 634b 7750 7a57 6537 6b77  2QxmMzcKwPzWe7kw
-00001680: 2d6f 7933 3449 5969 3539 223e 6d6f 6465  -oy34IYi59">mode
-00001690: 6c3c 2f61 3e3c 2f74 643e 0a3c 2f74 723e  l</a></td>.</tr>
-000016a0: 0a0a 3c2f 7461 626c 653e 0a0a 0a23 2323  ..</table>...###
-000016b0: 2052 6f62 7573 746e 6573 7320 2849 6d61   Robustness (Ima
-000016c0: 6765 4e65 742d 4120 2d20 496d 6167 654e  geNet-A - ImageN
-000016d0: 6574 2d52 202d 2049 6d61 6765 4e65 742d  et-R - ImageNet-
-000016e0: 5632 290a 0a41 6c6c 206d 6f64 656c 7320  V2)..All models 
-000016f0: 7573 6520 6063 726f 705f 7063 743d 302e  use `crop_pct=0.
-00001700: 3837 3560 2e20 5265 7375 6c74 7320 6172  875`. Results ar
-00001710: 6520 6f62 7461 696e 6564 2062 7920 7275  e obtained by ru
-00001720: 6e6e 696e 6720 696e 6665 7265 6e63 6520  nning inference 
-00001730: 6f6e 2049 6d61 6765 4e65 742d 314b 2070  on ImageNet-1K p
-00001740: 7265 7472 6169 6e65 6420 6d6f 6465 6c73  retrained models
-00001750: 2077 6974 686f 7574 2066 696e 6574 756e   without finetun
-00001760: 696e 672e 0a3c 7461 626c 653e 0a20 203c  ing..<table>.  <
-00001770: 7472 3e0a 2020 2020 3c74 683e 4e61 6d65  tr>.    <th>Name
-00001780: 3c2f 7468 3e0a 2020 2020 3c74 683e 412d  </th>.    <th>A-
-00001790: 4163 6340 3128 2529 3c2f 7468 3e0a 2020  Acc@1(%)</th>.  
-000017a0: 2020 3c74 683e 412d 4163 6340 3528 2529    <th>A-Acc@5(%)
-000017b0: 3c2f 7468 3e0a 2020 2020 3c74 683e 522d  </th>.    <th>R-
-000017c0: 4163 6340 3128 2529 3c2f 7468 3e0a 2020  Acc@1(%)</th>.  
-000017d0: 2020 3c74 683e 522d 4163 6340 3528 2529    <th>R-Acc@5(%)
-000017e0: 3c2f 7468 3e0a 2020 2020 3c74 683e 5632  </th>.    <th>V2
-000017f0: 2d41 6363 4031 2825 293c 2f74 683e 0a20  -Acc@1(%)</th>. 
-00001800: 2020 203c 7468 3e56 322d 4163 6340 3528     <th>V2-Acc@5(
-00001810: 2529 3c2f 7468 3e0a 2020 3c2f 7472 3e0a  %)</th>.  </tr>.
-00001820: 0a3c 7472 3e0a 2020 2020 3c74 643e 4661  .<tr>.    <td>Fa
-00001830: 7374 6572 5669 542d 303c 2f74 643e 0a20  sterViT-0</td>. 
-00001840: 2020 203c 7464 3e32 332e 393c 2f74 643e     <td>23.9</td>
-00001850: 0a20 2020 203c 7464 3e35 372e 363c 2f74  .    <td>57.6</t
-00001860: 643e 0a20 2020 203c 7464 3e34 352e 393c  d>.    <td>45.9<
-00001870: 2f74 643e 0a20 2020 203c 7464 3e36 302e  /td>.    <td>60.
-00001880: 343c 2f74 643e 0a20 2020 203c 7464 3e37  4</td>.    <td>7
-00001890: 302e 393c 2f74 643e 0a20 2020 203c 7464  0.9</td>.    <td
-000018a0: 3e39 302e 303c 2f74 643e 0a3c 2f74 723e  >90.0</td>.</tr>
-000018b0: 0a0a 3c74 723e 0a20 2020 203c 7464 3e46  ..<tr>.    <td>F
-000018c0: 6173 7465 7256 6954 2d31 3c2f 7464 3e0a  asterViT-1</td>.
-000018d0: 2020 2020 3c74 643e 3331 2e32 3c2f 7464      <td>31.2</td
-000018e0: 3e0a 2020 2020 3c74 643e 3633 2e33 3c2f  >.    <td>63.3</
-000018f0: 7464 3e0a 2020 2020 3c74 643e 3437 2e35  td>.    <td>47.5
-00001900: 3c2f 7464 3e0a 2020 2020 3c74 643e 3631  </td>.    <td>61
-00001910: 2e39 3c2f 7464 3e0a 2020 2020 3c74 643e  .9</td>.    <td>
-00001920: 3732 2e36 3c2f 7464 3e0a 2020 2020 3c74  72.6</td>.    <t
-00001930: 643e 3931 2e30 3c2f 7464 3e0a 3c2f 7472  d>91.0</td>.</tr
-00001940: 3e0a 0a3c 7472 3e0a 2020 2020 3c74 643e  >..<tr>.    <td>
-00001950: 4661 7374 6572 5669 542d 323c 2f74 643e  FasterViT-2</td>
-00001960: 0a20 2020 203c 7464 3e33 382e 323c 2f74  .    <td>38.2</t
-00001970: 643e 0a20 2020 203c 7464 3e36 382e 393c  d>.    <td>68.9<
-00001980: 2f74 643e 0a20 2020 203c 7464 3e34 392e  /td>.    <td>49.
-00001990: 363c 2f74 643e 0a20 2020 203c 7464 3e36  6</td>.    <td>6
-000019a0: 332e 343c 2f74 643e 0a20 2020 203c 7464  3.4</td>.    <td
-000019b0: 3e37 332e 373c 2f74 643e 0a20 2020 203c  >73.7</td>.    <
-000019c0: 7464 3e39 312e 363c 2f74 643e 0a3c 2f74  td>91.6</td>.</t
-000019d0: 723e 0a0a 3c74 723e 0a20 2020 203c 7464  r>..<tr>.    <td
-000019e0: 3e46 6173 7465 7256 6954 2d33 3c2f 7464  >FasterViT-3</td
-000019f0: 3e0a 2020 2020 3c74 643e 3434 2e32 3c2f  >.    <td>44.2</
-00001a00: 7464 3e0a 2020 2020 3c74 643e 3733 2e30  td>.    <td>73.0
-00001a10: 3c2f 7464 3e0a 2020 2020 3c74 643e 3531  </td>.    <td>51
-00001a20: 2e39 3c2f 7464 3e0a 2020 2020 3c74 643e  .9</td>.    <td>
-00001a30: 3635 2e36 3c2f 7464 3e0a 2020 2020 3c74  65.6</td>.    <t
-00001a40: 643e 3735 2e30 3c2f 7464 3e0a 2020 2020  d>75.0</td>.    
-00001a50: 3c74 643e 3932 2e32 3c2f 7464 3e0a 3c2f  <td>92.2</td>.</
-00001a60: 7472 3e0a 0a3c 7472 3e0a 2020 2020 3c74  tr>..<tr>.    <t
-00001a70: 643e 4661 7374 6572 5669 542d 343c 2f74  d>FasterViT-4</t
-00001a80: 643e 0a20 2020 203c 7464 3e34 392e 303c  d>.    <td>49.0<
-00001a90: 2f74 643e 0a20 2020 203c 7464 3e37 352e  /td>.    <td>75.
-00001aa0: 343c 2f74 643e 0a20 2020 203c 7464 3e35  4</td>.    <td>5
-00001ab0: 362e 303c 2f74 643e 0a20 2020 203c 7464  6.0</td>.    <td
-00001ac0: 3e36 392e 363c 2f74 643e 0a20 2020 203c  >69.6</td>.    <
-00001ad0: 7464 3e37 352e 373c 2f74 643e 0a20 2020  td>75.7</td>.   
-00001ae0: 203c 7464 3e39 322e 373c 2f74 643e 0a3c   <td>92.7</td>.<
-00001af0: 2f74 723e 0a0a 3c74 723e 0a20 2020 203c  /tr>..<tr>.    <
-00001b00: 7464 3e46 6173 7465 7256 6954 2d35 3c2f  td>FasterViT-5</
-00001b10: 7464 3e0a 2020 2020 3c74 643e 3532 2e37  td>.    <td>52.7
-00001b20: 3c2f 7464 3e0a 2020 2020 3c74 643e 3737  </td>.    <td>77
-00001b30: 2e36 3c2f 7464 3e0a 2020 2020 3c74 643e  .6</td>.    <td>
-00001b40: 3536 2e39 3c2f 7464 3e0a 2020 2020 3c74  56.9</td>.    <t
-00001b50: 643e 3730 2e30 3c2f 7464 3e0a 2020 2020  d>70.0</td>.    
-00001b60: 3c74 643e 3736 2e30 3c2f 7464 3e0a 2020  <td>76.0</td>.  
-00001b70: 2020 3c74 643e 3933 2e30 3c2f 7464 3e0a    <td>93.0</td>.
-00001b80: 3c2f 7472 3e0a 0a3c 7472 3e0a 2020 2020  </tr>..<tr>.    
-00001b90: 3c74 643e 4661 7374 6572 5669 542d 363c  <td>FasterViT-6<
-00001ba0: 2f74 643e 0a20 2020 203c 7464 3e35 332e  /td>.    <td>53.
-00001bb0: 373c 2f74 643e 0a20 2020 203c 7464 3e37  7</td>.    <td>7
-00001bc0: 382e 343c 2f74 643e 0a20 2020 203c 7464  8.4</td>.    <td
-00001bd0: 3e35 372e 313c 2f74 643e 0a20 2020 203c  >57.1</td>.    <
-00001be0: 7464 3e37 302e 313c 2f74 643e 0a20 2020  td>70.1</td>.   
-00001bf0: 203c 7464 3e37 362e 313c 2f74 643e 0a20   <td>76.1</td>. 
-00001c00: 2020 203c 7464 3e39 332e 303c 2f74 643e     <td>93.0</td>
-00001c10: 0a3c 2f74 723e 0a0a 3c2f 7461 626c 653e  .</tr>..</table>
-00001c20: 0a0a 412c 2052 2061 6e64 2056 3220 6465  ..A, R and V2 de
-00001c30: 6e6f 7465 2049 6d61 6765 4e65 742d 412c  note ImageNet-A,
-00001c40: 2049 6d61 6765 4e65 742d 5220 616e 6420   ImageNet-R and 
-00001c50: 496d 6167 654e 6574 2d56 3220 7265 7370  ImageNet-V2 resp
-00001c60: 6563 7469 7665 6c79 2e20 0a23 2320 5472  ectively. .## Tr
-00001c70: 6169 6e69 6e67 0a0a 506c 6561 7365 2073  aining..Please s
-00001c80: 6565 205b 5452 4149 4e49 4e47 2e6d 645d  ee [TRAINING.md]
-00001c90: 2854 5241 494e 494e 472e 6d64 2920 666f  (TRAINING.md) fo
-00001ca0: 7220 6465 7461 696c 6564 2074 7261 696e  r detailed train
-00001cb0: 696e 6720 696e 7374 7275 6374 696f 6e73  ing instructions
-00001cc0: 206f 6620 616c 6c20 6d6f 6465 6c73 2e20   of all models. 
-00001cd0: 0a0a 2323 2045 7661 6c75 6174 696f 6e0a  ..## Evaluation.
-00001ce0: 0a54 6865 2046 6173 7465 7256 6954 206d  .The FasterViT m
-00001cf0: 6f64 656c 7320 6361 6e20 6265 2065 7661  odels can be eva
-00001d00: 6c75 6174 6564 206f 6e20 496d 6167 654e  luated on ImageN
-00001d10: 6574 2d31 4b20 7661 6c69 6461 7469 6f6e  et-1K validation
-00001d20: 2073 6574 2075 7369 6e67 2074 6865 2066   set using the f
-00001d30: 6f6c 6c6f 7769 6e67 3a20 0a0a 6060 600a  ollowing: ..```.
-00001d40: 7079 7468 6f6e 2076 616c 6964 6174 652e  python validate.
-00001d50: 7079 205c 0a2d 2d6d 6f64 656c 203c 6d6f  py \.--model <mo
-00001d60: 6465 6c2d 6e61 6d65 3e0a 2d2d 6368 6563  del-name>.--chec
-00001d70: 6b70 6f69 6e74 203c 6368 6563 6b70 6f69  kpoint <checkpoi
-00001d80: 6e74 2d70 6174 683e 0a2d 2d64 6174 615f  nt-path>.--data_
-00001d90: 6469 7220 3c69 6d61 6765 6e65 742d 7061  dir <imagenet-pa
-00001da0: 7468 3e0a 2d2d 6261 7463 682d 7369 7a65  th>.--batch-size
-00001db0: 203c 6261 7463 682d 7369 7a65 2d70 6572   <batch-size-per
-00001dc0: 2d67 7075 0a60 6060 200a 0a48 6572 6520  -gpu.``` ..Here 
-00001dd0: 602d 2d6d 6f64 656c 6020 6973 2074 6865  `--model` is the
-00001de0: 2046 6173 7465 7256 6954 2076 6172 6961   FasterViT varia
-00001df0: 6e74 2028 652e 672e 2060 6661 7374 6572  nt (e.g. `faster
-00001e00: 5f76 6974 5f30 5f32 3234 5f31 6b60 292c  _vit_0_224_1k`),
-00001e10: 2060 2d2d 6368 6563 6b70 6f69 6e74 6020   `--checkpoint` 
-00001e20: 6973 2074 6865 2070 6174 6820 746f 2070  is the path to p
-00001e30: 7265 7472 6169 6e65 6420 6d6f 6465 6c20  retrained model 
-00001e40: 7765 6967 6874 732c 2060 2d2d 6461 7461  weights, `--data
-00001e50: 5f64 6972 6020 6973 2074 6865 2070 6174  _dir` is the pat
-00001e60: 6820 746f 2049 6d61 6765 4e65 742d 314b  h to ImageNet-1K
-00001e70: 2076 616c 6964 6174 696f 6e20 7365 7420   validation set 
-00001e80: 616e 6420 602d 2d62 6174 6368 2d73 697a  and `--batch-siz
-00001e90: 6560 2069 7320 7468 6520 6e75 6d62 6572  e` is the number
-00001ea0: 206f 6620 6261 7463 6820 7369 7a65 2e20   of batch size. 
-00001eb0: 5765 2061 6c73 6f20 7072 6f76 6964 6520  We also provide 
-00001ec0: 6120 7361 6d70 6c65 2073 6372 6970 7420  a sample script 
-00001ed0: 5b68 6572 655d 282e 2f66 6173 7465 7276  [here](./fasterv
-00001ee0: 6974 2f76 616c 6964 6174 652e 7368 292e  it/validate.sh).
-00001ef0: 200a 0a0a 2323 2049 6e73 7461 6c6c 6174   ...## Installat
-00001f00: 696f 6e0a 0a54 6865 2064 6570 656e 6465  ion..The depende
-00001f10: 6e63 6965 7320 6361 6e20 6265 2069 6e73  ncies can be ins
-00001f20: 7461 6c6c 6564 2062 7920 7275 6e6e 696e  talled by runnin
-00001f30: 673a 0a0a 6060 6062 6173 680a 7069 7020  g:..```bash.pip 
-00001f40: 696e 7374 616c 6c20 2d72 2072 6571 7569  install -r requi
-00001f50: 7265 6d65 6e74 732e 7478 740a 6060 600a  rements.txt.```.
-00001f60: 0a23 2320 5468 6972 642d 7061 7274 7920  .## Third-party 
-00001f70: 4578 7465 6e74 696f 6e73 0a57 6520 616c  Extentions.We al
-00001f80: 7761 7973 2077 656c 636f 6d65 2074 6869  ways welcome thi
-00001f90: 7264 2d70 6172 7479 2065 7874 656e 7469  rd-party extenti
-00001fa0: 6f6e 732f 696d 706c 656d 656e 7461 7469  ons/implementati
-00001fb0: 6f6e 7320 616e 6420 7573 6167 6520 666f  ons and usage fo
-00001fc0: 7220 6f74 6865 7220 7075 7270 6f73 6573  r other purposes
-00001fd0: 2e20 4966 2079 6f75 2077 6f75 6c64 206c  . If you would l
-00001fe0: 696b 6520 796f 7572 2077 6f72 6b20 746f  ike your work to
-00001ff0: 2062 6520 6c69 7374 6564 2069 6e20 7468   be listed in th
-00002000: 6973 2072 6570 6f73 6974 6f72 792c 2070  is repository, p
-00002010: 6c65 6173 6520 7261 6973 6520 616e 6420  lease raise and 
-00002020: 6973 7375 6520 616e 6420 7072 6f76 6964  issue and provid
-00002030: 6520 7573 2077 6974 6820 6465 7461 696c  e us with detail
-00002040: 6564 2069 6e66 6f72 6d61 7469 6f6e 2e20  ed information. 
-00002050: 200a 0a0a 2323 2041 636b 6e6f 776c 6564   ...## Acknowled
-00002060: 6765 6d65 6e74 0a54 6869 7320 7265 706f  gement.This repo
-00002070: 7369 746f 7279 2069 7320 6275 696c 7420  sitory is built 
-00002080: 6f6e 2074 6f70 206f 6620 7468 6520 5b74  on top of the [t
-00002090: 696d 6d5d 2868 7474 7073 3a2f 2f67 6974  imm](https://git
-000020a0: 6875 622e 636f 6d2f 6875 6767 696e 6766  hub.com/huggingf
-000020b0: 6163 652f 7079 746f 7263 682d 696d 6167  ace/pytorch-imag
-000020c0: 652d 6d6f 6465 6c73 2920 7265 706f 7369  e-models) reposi
-000020d0: 746f 7279 2e20 5765 2074 6861 6e6b 205b  tory. We thank [
-000020e0: 526f 7373 2057 7269 6768 746d 616e 5d28  Ross Wrightman](
-000020f0: 6874 7470 733a 2f2f 7277 6967 6874 6d61  https://rwightma
-00002100: 6e2e 636f 6d2f 2920 666f 7220 6372 6561  n.com/) for crea
-00002110: 7469 6e67 2061 6e64 206d 6169 6e74 6169  ting and maintai
-00002120: 6e69 6e67 2074 6869 7320 6869 6768 2d71  ning this high-q
-00002130: 7561 6c69 7479 206c 6962 7261 7279 2e20  uality library. 
-00002140: 200a 0a23 2320 4369 7461 7469 6f6e 0a0a   ..## Citation..
-00002150: 506c 6561 7365 2063 6f6e 7369 6465 7220  Please consider 
-00002160: 6369 7469 6e67 2046 6173 7465 7256 6954  citing FasterViT
-00002170: 2069 6620 7468 6973 2072 6570 6f73 6974   if this reposit
-00002180: 6f72 7920 6973 2075 7365 6675 6c20 666f  ory is useful fo
-00002190: 7220 796f 7572 2077 6f72 6b3a 0a0a 6060  r your work:..``
-000021a0: 600a 4061 7274 6963 6c65 7b68 6174 616d  `.@article{hatam
-000021b0: 697a 6164 6568 3230 3233 6661 7374 6572  izadeh2023faster
-000021c0: 7669 742c 0a20 2074 6974 6c65 3d7b 4661  vit,.  title={Fa
-000021d0: 7374 6572 5669 543a 2046 6173 7420 5669  sterViT: Fast Vi
-000021e0: 7369 6f6e 2054 7261 6e73 666f 726d 6572  sion Transformer
-000021f0: 7320 7769 7468 2048 6965 7261 7263 6869  s with Hierarchi
-00002200: 6361 6c20 4174 7465 6e74 696f 6e7d 2c0a  cal Attention},.
-00002210: 2020 6175 7468 6f72 3d7b 4861 7461 6d69    author={Hatami
-00002220: 7a61 6465 682c 2041 6c69 2061 6e64 2048  zadeh, Ali and H
-00002230: 6569 6e72 6963 682c 2047 7265 6720 616e  einrich, Greg an
-00002240: 6420 5969 6e2c 2048 6f6e 6778 7520 616e  d Yin, Hongxu an
-00002250: 6420 5461 6f2c 2041 6e64 7265 7720 616e  d Tao, Andrew an
-00002260: 6420 416c 7661 7265 7a2c 204a 6f73 6520  d Alvarez, Jose 
-00002270: 4d20 616e 6420 4b61 7574 7a2c 204a 616e  M and Kautz, Jan
-00002280: 2061 6e64 204d 6f6c 6368 616e 6f76 2c20   and Molchanov, 
-00002290: 5061 766c 6f7d 2c0a 2020 6a6f 7572 6e61  Pavlo},.  journa
-000022a0: 6c3d 7b61 7258 6976 2070 7265 7072 696e  l={arXiv preprin
-000022b0: 7420 6172 5869 763a 3233 3036 2e30 3631  t arXiv:2306.061
-000022c0: 3839 7d2c 0a20 2079 6561 723d 7b32 3032  89},.  year={202
-000022d0: 337d 0a7d 0a60 6060 0a0a 2323 204c 6963  3}.}.```..## Lic
-000022e0: 656e 7365 730a 0a43 6f70 7972 6967 6874  enses..Copyright
-000022f0: 20c2 a920 3230 3233 2c20 4e56 4944 4941   .. 2023, NVIDIA
-00002300: 2043 6f72 706f 7261 7469 6f6e 2e20 416c   Corporation. Al
-00002310: 6c20 7269 6768 7473 2072 6573 6572 7665  l rights reserve
-00002320: 642e 0a0a 5468 6973 2077 6f72 6b20 6973  d...This work is
-00002330: 206d 6164 6520 6176 6169 6c61 626c 6520   made available 
-00002340: 756e 6465 7220 7468 6520 4e56 4944 4941  under the NVIDIA
-00002350: 2053 6f75 7263 6520 436f 6465 204c 6963   Source Code Lic
-00002360: 656e 7365 2d4e 432e 2043 6c69 636b 205b  ense-NC. Click [
-00002370: 6865 7265 5d28 4c49 4345 4e53 4529 2074  here](LICENSE) t
-00002380: 6f20 7669 6577 2061 2063 6f70 7920 6f66  o view a copy of
-00002390: 2074 6869 7320 6c69 6365 6e73 652e 0a0a   this license...
-000023a0: 466f 7220 6c69 6365 6e73 6520 696e 666f  For license info
-000023b0: 726d 6174 696f 6e20 7265 6761 7264 696e  rmation regardin
-000023c0: 6720 7468 6520 7469 6d6d 2072 6570 6f73  g the timm repos
-000023d0: 6974 6f72 792c 2070 6c65 6173 6520 7265  itory, please re
-000023e0: 6665 7220 746f 2069 7473 205b 7265 706f  fer to its [repo
-000023f0: 7369 746f 7279 5d28 6874 7470 733a 2f2f  sitory](https://
-00002400: 6769 7468 7562 2e63 6f6d 2f72 7769 6768  github.com/rwigh
-00002410: 746d 616e 2f70 7974 6f72 6368 2d69 6d61  tman/pytorch-ima
-00002420: 6765 2d6d 6f64 656c 7329 2e0a 0a46 6f72  ge-models)...For
-00002430: 206c 6963 656e 7365 2069 6e66 6f72 6d61   license informa
-00002440: 7469 6f6e 2072 6567 6172 6469 6e67 2074  tion regarding t
-00002450: 6865 2049 6d61 6765 4e65 7420 6461 7461  he ImageNet data
-00002460: 7365 742c 2070 6c65 6173 6520 7365 6520  set, please see 
-00002470: 7468 6520 5b49 6d61 6765 4e65 7420 6f66  the [ImageNet of
-00002480: 6669 6369 616c 2077 6562 7369 7465 5d28  ficial website](
-00002490: 6874 7470 733a 2f2f 7777 772e 696d 6167  https://www.imag
-000024a0: 652d 6e65 742e 6f72 672f 292e 200a       e-net.org/). .
+00000720: 6461 7461 2021 290a 0a3c 7020 616c 6967  data !)..<p alig
+00000730: 6e3d 2263 656e 7465 7222 3e0a 3c69 6d67  n="center">.<img
+00000740: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+00000750: 7468 7562 2e63 6f6d 2f4e 566c 6162 732f  thub.com/NVlabs/
+00000760: 4661 7374 6572 5669 542f 6173 7365 7473  FasterViT/assets
+00000770: 2f32 3638 3036 3339 342f 3235 3364 3161  /26806394/253d1a
+00000780: 3265 2d62 3566 352d 3461 3962 2d61 3336  2e-b5f5-4a9b-a36
+00000790: 322d 3663 6464 3136 6266 6363 6331 2220  2-6cdd16bfccc1" 
+000007a0: 7769 6474 683d 3632 2520 6865 6967 6874  width=62% height
+000007b0: 3d36 3225 200a 636c 6173 733d 2263 656e  =62% .class="cen
+000007c0: 7465 7222 3e0a 3c2f 703e 0a0a 0a3c 212d  ter">.</p>...<!-
+000007d0: 2d20 5765 2069 6e74 726f 6475 6365 2061  - We introduce a
+000007e0: 206e 6577 2073 656c 662d 6174 7465 6e74   new self-attent
+000007f0: 696f 6e20 6d65 6368 616e 6973 6d2c 2064  ion mechanism, d
+00000800: 656e 6f74 6564 2061 7320 4869 6572 6172  enoted as Hierar
+00000810: 6368 6963 616c 0a41 7474 656e 7469 6f6e  chical.Attention
+00000820: 2028 4841 5429 2c20 7468 6174 2063 6170   (HAT), that cap
+00000830: 7475 7265 7320 626f 7468 2073 686f 7274  tures both short
+00000840: 2061 6e64 206c 6f6e 672d 7261 6e67 6520   and long-range 
+00000850: 696e 666f 726d 6174 696f 6e20 6279 206c  information by l
+00000860: 6561 726e 696e 670a 6372 6f73 732d 7769  earning.cross-wi
+00000870: 6e64 6f77 2063 6172 7269 6572 2074 6f6b  ndow carrier tok
+00000880: 656e 732e 0a0a 215b 7465 6173 6572 5d28  ens...![teaser](
+00000890: 2e2f 6661 7374 6572 7669 742f 6173 7365  ./fastervit/asse
+000008a0: 7473 2f68 6965 7261 7263 6869 616c 5f61  ts/hierarchial_a
+000008b0: 7474 6e2e 706e 6729 202d 2d3e 0a0a 0a3c  ttn.png) -->...<
+000008c0: 212d 2d20 2323 20f0 9f92 a520 4e65 7773  !-- ## .... News
+000008d0: 20f0 9f92 a50a 0a2d 202a 2a5b 3036 2e31   ......- **[06.1
+000008e0: 382e 3230 3233 5d2a 2a20 f09f 94a5 2057  8.2023]** .... W
+000008f0: 6520 6861 7665 2072 656c 6561 7365 6420  e have released 
+00000900: 7468 6520 4661 7374 6572 5669 5420 5b70  the FasterViT [p
+00000910: 6970 2070 6163 6b61 6765 5d28 6874 7470  ip package](http
+00000920: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000930: 6a65 6374 2f66 6173 7465 7276 6974 2f29  ject/fastervit/)
+00000940: 2021 0a2d 202a 2a5b 3036 2e31 372e 3230   !.- **[06.17.20
+00000950: 3233 5d2a 2a20 f09f 94a5 205b 416e 792d  23]** .... [Any-
+00000960: 7265 736f 6c75 7469 6f6e 2046 6173 7465  resolution Faste
+00000970: 7256 6954 5d28 2e2f 6661 7374 6572 7669  rViT](./fastervi
+00000980: 742f 6d6f 6465 6c73 2f66 6173 7465 725f  t/models/faster_
+00000990: 7669 745f 616e 795f 7265 732e 7079 2920  vit_any_res.py) 
+000009a0: 206d 6f64 656c 2069 7320 6e6f 7720 6176   model is now av
+000009b0: 6169 6c61 626c 6520 2120 7468 6520 6d6f  ailable ! the mo
+000009c0: 6465 6c20 6361 6e20 6265 2075 7365 6420  del can be used 
+000009d0: 666f 7220 7661 7269 6574 7920 6f66 2061  for variety of a
+000009e0: 7070 6c69 6361 7469 6f6e 7320 7375 6368  pplications such
+000009f0: 2061 7320 6465 7465 6374 696f 6e20 616e   as detection an
+00000a00: 6420 7365 676d 656e 7461 7469 6f6e 206f  d segmentation o
+00000a10: 7220 6869 6768 2d72 6573 6f6c 7574 696f  r high-resolutio
+00000a20: 6e20 6669 6e65 2d74 756e 696e 6720 7769  n fine-tuning wi
+00000a30: 7468 2061 7262 6974 7261 7279 2069 6e70  th arbitrary inp
+00000a40: 7574 2069 6d61 6765 2072 6573 6f6c 7574  ut image resolut
+00000a50: 696f 6e73 2e20 0a2d 202a 2a5b 3036 2e30  ions. .- **[06.0
+00000a60: 392e 3230 3233 5d2a 2a20 f09f 94a5 f09f  9.2023]** ......
+00000a70: 94a5 2057 6520 6861 7665 2072 656c 6561  .. We have relea
+00000a80: 7365 6420 736f 7572 6365 2063 6f64 6520  sed source code 
+00000a90: 616e 6420 496d 6167 654e 6574 2d31 4b20  and ImageNet-1K 
+00000aa0: 4661 7374 6572 5669 542d 6d6f 6465 6c73  FasterViT-models
+00000ab0: 2021 202d 2d3e 0a0a 2323 2051 7569 636b   ! -->..## Quick
+00000ac0: 2053 7461 7274 0a0a 5468 6520 4661 7374   Start..The Fast
+00000ad0: 6572 5669 5420 6361 6e20 6265 2063 6f6e  erViT can be con
+00000ae0: 7665 6e69 656e 746c 7920 696e 7374 616c  veniently instal
+00000af0: 6c65 6420 6279 3a0a 0a60 6060 6261 7368  led by:..```bash
+00000b00: 0a70 6970 2069 6e73 7461 6c6c 2066 6173  .pip install fas
+00000b10: 7465 7276 6974 0a60 6060 0a0a 4120 4661  tervit.```..A Fa
+00000b20: 7374 6572 5669 5420 6d6f 6465 6c20 7769  sterViT model wi
+00000b30: 7468 2064 6566 6175 6c74 2068 7970 6572  th default hyper
+00000b40: 2d70 6172 616d 6574 6572 7320 6361 6e20  -parameters can 
+00000b50: 6265 2063 7265 6174 6564 2061 7320 696e  be created as in
+00000b60: 2074 6865 2066 6f6c 6c6f 7769 6e67 3a0a   the following:.
+00000b70: 0a60 6060 7079 7468 6f6e 0a3e 3e3e 2066  .```python.>>> f
+00000b80: 726f 6d20 6661 7374 6572 7669 7420 696d  rom fastervit im
+00000b90: 706f 7274 2063 7265 6174 655f 6d6f 6465  port create_mode
+00000ba0: 6c0a 0a23 2044 6566 696e 6520 6661 7374  l..# Define fast
+00000bb0: 6572 7669 742d 3020 6d6f 6465 6c20 7769  ervit-0 model wi
+00000bc0: 7468 2032 3234 2078 2032 3234 2072 6573  th 224 x 224 res
+00000bd0: 6f6c 7574 696f 6e0a 3e3e 3e20 6d6f 6465  olution.>>> mode
+00000be0: 6c20 3d20 6372 6561 7465 5f6d 6f64 656c  l = create_model
+00000bf0: 2827 6661 7374 6572 5f76 6974 5f30 5f32  ('faster_vit_0_2
+00000c00: 3234 2729 0a60 6060 0a0a 5765 2063 616e  24').```..We can
+00000c10: 2061 6c73 6f20 7573 6520 7468 6520 616e   also use the an
+00000c20: 792d 7265 736f 6c75 7469 6f6e 2046 6173  y-resolution Fas
+00000c30: 7465 7256 6954 206d 6f64 656c 2074 6f20  terViT model to 
+00000c40: 6163 636f 6d6d 6f64 6174 6520 6172 6269  accommodate arbi
+00000c50: 7472 6172 7920 696d 6167 6520 7265 736f  trary image reso
+00000c60: 6c75 7469 6f6e 732e 2049 6e20 7468 6520  lutions. In the 
+00000c70: 666f 6c6c 6f77 696e 672c 2077 6520 6465  following, we de
+00000c80: 6669 6e65 2061 6e20 616e 792d 7265 736f  fine an any-reso
+00000c90: 6c75 7469 6f6e 2046 6173 7465 7256 6954  lution FasterViT
+00000ca0: 2d31 0a6d 6f64 656c 2077 6974 6820 696e  -1.model with in
+00000cb0: 7075 7420 7265 736f 6c75 7469 6f6e 206f  put resolution o
+00000cc0: 6620 3537 3620 7820 3936 302c 2077 696e  f 576 x 960, win
+00000cd0: 646f 7720 7369 7a65 7320 6f66 2031 3220  dow sizes of 12 
+00000ce0: 616e 6420 3620 696e 2033 7264 2061 6e64  and 6 in 3rd and
+00000cf0: 2034 7468 2073 7461 6765 732c 2063 6172   4th stages, car
+00000d00: 7269 6572 2074 6f6b 656e 2073 697a 6520  rier token size 
+00000d10: 6f66 2032 2061 6e64 2065 6d62 6564 6469  of 2 and embeddi
+00000d20: 6e67 2064 696d 656e 7369 6f6e 206f 660a  ng dimension of.
+00000d30: 3132 383a 0a0a 6060 6070 7974 686f 6e0a  128:..```python.
+00000d40: 3e3e 3e20 6672 6f6d 2066 6173 7465 7276  >>> from fasterv
+00000d50: 6974 2069 6d70 6f72 7420 6372 6561 7465  it import create
+00000d60: 5f6d 6f64 656c 0a0a 2320 4465 6669 6e65  _model..# Define
+00000d70: 2061 6e79 2d72 6573 6f6c 7574 696f 6e20   any-resolution 
+00000d80: 4661 7374 6572 5669 542d 3120 6d6f 6465  FasterViT-1 mode
+00000d90: 6c20 7769 7468 2035 3736 2078 2039 3630  l with 576 x 960
+00000da0: 2072 6573 6f6c 7574 696f 6e0a 3e3e 3e20   resolution.>>> 
+00000db0: 6d6f 6465 6c20 3d20 6372 6561 7465 5f6d  model = create_m
+00000dc0: 6f64 656c 2827 6661 7374 6572 5f76 6974  odel('faster_vit
+00000dd0: 5f31 5f61 6e79 5f72 6573 272c 200a 2020  _1_any_res', .  
+00000de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000df0: 2020 2020 2020 2020 7265 736f 6c75 7469          resoluti
+00000e00: 6f6e 3d5b 3537 362c 2039 3630 5d2c 0a20  on=[576, 960],. 
+00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e20: 2020 2020 2020 2020 2077 696e 646f 775f           window_
+00000e30: 7369 7a65 3d5b 372c 2037 2c20 3132 2c20  size=[7, 7, 12, 
+00000e40: 365d 2c0a 2020 2020 2020 2020 2020 2020  6],.            
+00000e50: 2020 2020 2020 2020 2020 2020 2020 6374                ct
+00000e60: 5f73 697a 653d 322c 0a20 2020 2020 2020  _size=2,.       
+00000e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e80: 2020 2064 696d 3d31 3238 290a 6060 600a     dim=128).```.
+00000e90: 0a3c 212d 2d20 2323 2043 6174 616c 6f67  .<!-- ## Catalog
+00000ea0: 0a2d 205b 785d 2049 6d61 6765 4e65 742d  .- [x] ImageNet-
+00000eb0: 314b 2074 7261 696e 696e 6720 636f 6465  1K training code
+00000ec0: 0a2d 205b 785d 2049 6d61 6765 4e65 742d  .- [x] ImageNet-
+00000ed0: 314b 2070 7265 2d74 7261 696e 6564 206d  1K pre-trained m
+00000ee0: 6f64 656c 730a 2d20 5b78 5d20 416e 792d  odels.- [x] Any-
+00000ef0: 7265 736f 6c75 7469 6f6e 2046 6173 7465  resolution Faste
+00000f00: 7256 6954 0a2d 205b 785d 2046 6173 7465  rViT.- [x] Faste
+00000f10: 7256 6954 2070 6970 2d70 6163 6b61 6765  rViT pip-package
+00000f20: 2072 656c 6561 7365 0a2d 205b 205d 2055   release.- [ ] U
+00000f30: 7064 6174 6520 7472 6169 6e69 6e67 2073  pdate training s
+00000f40: 6372 6970 7473 2074 6f20 7375 7070 6f72  cripts to suppor
+00000f50: 7420 6d6f 6465 6c2e 636f 6d70 696c 652c  t model.compile,
+00000f60: 200a 2d20 5b20 5d20 496d 6167 654e 6574   .- [ ] ImageNet
+00000f70: 2d32 314b 2070 7265 2d74 7261 696e 6564  -21K pre-trained
+00000f80: 206d 6f64 656c 730a 2d20 5b20 5d20 496d   models.- [ ] Im
+00000f90: 6167 654e 6574 2d32 314b 2066 696e 652d  ageNet-21K fine-
+00000fa0: 7475 6e65 2073 6372 6970 7473 0a2d 205b  tune scripts.- [
+00000fb0: 205d 2044 6574 6563 7469 6f6e 2063 6f64   ] Detection cod
+00000fc0: 6520 2844 494e 4f29 202b 206d 6f64 656c  e (DINO) + model
+00000fd0: 730a 2d20 5b20 5d20 5365 676d 656e 7461  s.- [ ] Segmenta
+00000fe0: 7469 6f6e 2063 6f64 6520 2b20 6d6f 6465  tion code + mode
+00000ff0: 6c73 202d 2d3e 0a0a 2d2d 2d20 0a0a 2323  ls -->..--- ..##
+00001000: 2052 6573 756c 7473 202b 2050 7265 7472   Results + Pretr
+00001010: 6169 6e65 6420 4d6f 6465 6c73 0a0a 2323  ained Models..##
+00001020: 2320 496d 6167 654e 6574 2d31 4b0a 2a2a  # ImageNet-1K.**
+00001030: 4661 7374 6572 5669 5420 496d 6167 654e  FasterViT ImageN
+00001040: 6574 2d31 4b20 5072 6574 7261 696e 6564  et-1K Pretrained
+00001050: 204d 6f64 656c 732a 2a0a 0a3c 7461 626c   Models**..<tabl
+00001060: 653e 0a20 203c 7472 3e0a 2020 2020 3c74  e>.  <tr>.    <t
+00001070: 683e 4e61 6d65 3c2f 7468 3e0a 2020 2020  h>Name</th>.    
+00001080: 3c74 683e 4163 6340 3128 2529 3c2f 7468  <th>Acc@1(%)</th
+00001090: 3e0a 2020 2020 3c74 683e 4163 6340 3528  >.    <th>Acc@5(
+000010a0: 2529 3c2f 7468 3e0a 2020 2020 3c74 683e  %)</th>.    <th>
+000010b0: 5468 726f 7567 6870 7574 2849 6d67 2f53  Throughput(Img/S
+000010c0: 6563 293c 2f74 683e 0a20 2020 203c 7468  ec)</th>.    <th
+000010d0: 3e52 6573 6f6c 7574 696f 6e3c 2f74 683e  >Resolution</th>
+000010e0: 0a20 2020 203c 7468 3e23 5061 7261 6d73  .    <th>#Params
+000010f0: 284d 293c 2f74 683e 0a20 2020 203c 7468  (M)</th>.    <th
+00001100: 3e46 4c4f 5073 2847 293c 2f74 683e 0a20  >FLOPs(G)</th>. 
+00001110: 2020 203c 7468 3e44 6f77 6e6c 6f61 643c     <th>Download<
+00001120: 2f74 683e 0a20 203c 2f74 723e 0a0a 3c74  /th>.  </tr>..<t
+00001130: 723e 0a20 2020 203c 7464 3e46 6173 7465  r>.    <td>Faste
+00001140: 7256 6954 2d30 3c2f 7464 3e0a 2020 2020  rViT-0</td>.    
+00001150: 3c74 643e 3832 2e31 3c2f 7464 3e0a 2020  <td>82.1</td>.  
+00001160: 2020 3c74 643e 3935 2e39 3c2f 7464 3e0a    <td>95.9</td>.
+00001170: 2020 2020 3c74 643e 3538 3032 3c2f 7464      <td>5802</td
+00001180: 3e0a 2020 2020 3c74 643e 3232 3478 3232  >.    <td>224x22
+00001190: 343c 2f74 643e 0a20 2020 203c 7464 3e33  4</td>.    <td>3
+000011a0: 312e 343c 2f74 643e 0a20 2020 203c 7464  1.4</td>.    <td
+000011b0: 3e33 2e33 3c2f 7464 3e0a 2020 2020 3c74  >3.3</td>.    <t
+000011c0: 643e 3c61 2068 7265 663d 2268 7474 7073  d><a href="https
+000011d0: 3a2f 2f64 7269 7665 2e67 6f6f 676c 652e  ://drive.google.
+000011e0: 636f 6d2f 7563 3f65 7870 6f72 743d 646f  com/uc?export=do
+000011f0: 776e 6c6f 6164 2669 643d 3174 7749 324c  wnload&id=1twI2L
+00001200: 464a 7333 3931 5972 6a38 4d52 3455 6939  FJs391Yrj8MR4Ui9
+00001210: 5066 7276 5771 6a45 3169 4222 3e6d 6f64  PfrvWqjE1iB">mod
+00001220: 656c 3c2f 613e 3c2f 7464 3e0a 3c2f 7472  el</a></td>.</tr
+00001230: 3e0a 0a3c 7472 3e0a 2020 2020 3c74 643e  >..<tr>.    <td>
+00001240: 4661 7374 6572 5669 542d 313c 2f74 643e  FasterViT-1</td>
+00001250: 0a20 2020 203c 7464 3e38 332e 323c 2f74  .    <td>83.2</t
+00001260: 643e 0a20 2020 203c 7464 3e39 362e 353c  d>.    <td>96.5<
+00001270: 2f74 643e 0a20 2020 203c 7464 3e34 3138  /td>.    <td>418
+00001280: 383c 2f74 643e 0a20 2020 203c 7464 3e32  8</td>.    <td>2
+00001290: 3234 7832 3234 3c2f 7464 3e0a 2020 2020  24x224</td>.    
+000012a0: 3c74 643e 3533 2e34 3c2f 7464 3e0a 2020  <td>53.4</td>.  
+000012b0: 2020 3c74 643e 352e 333c 2f74 643e 0a20    <td>5.3</td>. 
+000012c0: 2020 203c 7464 3e3c 6120 6872 6566 3d22     <td><a href="
+000012d0: 6874 7470 733a 2f2f 6472 6976 652e 676f  https://drive.go
+000012e0: 6f67 6c65 2e63 6f6d 2f75 633f 6578 706f  ogle.com/uc?expo
+000012f0: 7274 3d64 6f77 6e6c 6f61 6426 6964 3d31  rt=download&id=1
+00001300: 7237 5731 306e 352d 6246 744d 3373 7a34  r7W10n5-bFtM3sz4
+00001310: 626d 614c 726f 774e 3267 5950 6b4c 4754  bmaLrowN2gYPkLGT
+00001320: 223e 6d6f 6465 6c3c 2f61 3e3c 2f74 643e  ">model</a></td>
+00001330: 0a3c 2f74 723e 0a0a 3c74 723e 0a20 2020  .</tr>..<tr>.   
+00001340: 203c 7464 3e46 6173 7465 7256 6954 2d32   <td>FasterViT-2
+00001350: 3c2f 7464 3e0a 2020 2020 3c74 643e 3834  </td>.    <td>84
+00001360: 2e32 3c2f 7464 3e0a 2020 2020 3c74 643e  .2</td>.    <td>
+00001370: 3936 2e38 3c2f 7464 3e0a 2020 2020 3c74  96.8</td>.    <t
+00001380: 643e 3331 3631 3c2f 7464 3e0a 2020 2020  d>3161</td>.    
+00001390: 3c74 643e 3232 3478 3232 343c 2f74 643e  <td>224x224</td>
+000013a0: 0a20 2020 203c 7464 3e37 352e 393c 2f74  .    <td>75.9</t
+000013b0: 643e 0a20 2020 203c 7464 3e38 2e37 3c2f  d>.    <td>8.7</
+000013c0: 7464 3e0a 2020 2020 3c74 643e 3c61 2068  td>.    <td><a h
+000013d0: 7265 663d 2268 7474 7073 3a2f 2f64 7269  ref="https://dri
+000013e0: 7665 2e67 6f6f 676c 652e 636f 6d2f 7563  ve.google.com/uc
+000013f0: 3f65 7870 6f72 743d 646f 776e 6c6f 6164  ?export=download
+00001400: 2669 643d 316e 5f61 3673 3070 6769 306a  &id=1n_a6s0pgi0j
+00001410: 565a 4f47 6d44 6569 3276 5848 5535 4536  VZOGmDei2vXHU5E6
+00001420: 5248 3577 5522 3e6d 6f64 656c 3c2f 613e  RH5wU">model</a>
+00001430: 3c2f 7464 3e0a 3c2f 7472 3e0a 0a3c 7472  </td>.</tr>..<tr
+00001440: 3e0a 2020 2020 3c74 643e 4661 7374 6572  >.    <td>Faster
+00001450: 5669 542d 333c 2f74 643e 0a20 2020 203c  ViT-3</td>.    <
+00001460: 7464 3e38 342e 393c 2f74 643e 0a20 2020  td>84.9</td>.   
+00001470: 203c 7464 3e39 372e 323c 2f74 643e 0a20   <td>97.2</td>. 
+00001480: 2020 203c 7464 3e31 3738 303c 2f74 643e     <td>1780</td>
+00001490: 0a20 2020 203c 7464 3e32 3234 7832 3234  .    <td>224x224
+000014a0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3135  </td>.    <td>15
+000014b0: 392e 353c 2f74 643e 0a20 2020 203c 7464  9.5</td>.    <td
+000014c0: 3e31 382e 323c 2f74 643e 0a20 2020 203c  >18.2</td>.    <
+000014d0: 7464 3e3c 6120 6872 6566 3d22 6874 7470  td><a href="http
+000014e0: 733a 2f2f 6472 6976 652e 676f 6f67 6c65  s://drive.google
+000014f0: 2e63 6f6d 2f75 633f 6578 706f 7274 3d64  .com/uc?export=d
+00001500: 6f77 6e6c 6f61 6426 6964 3d31 7476 5745  ownload&id=1tvWE
+00001510: 6c5a 3931 5369 6132 5373 5859 5846 4d4e  lZ91Sia2SsXYXFMN
+00001520: 5951 7766 6970 4378 7449 3758 223e 6d6f  YQwfipCxtI7X">mo
+00001530: 6465 6c3c 2f61 3e3c 2f74 643e 0a3c 2f74  del</a></td>.</t
+00001540: 723e 0a0a 3c74 723e 0a20 2020 203c 7464  r>..<tr>.    <td
+00001550: 3e46 6173 7465 7256 6954 2d34 3c2f 7464  >FasterViT-4</td
+00001560: 3e0a 2020 2020 3c74 643e 3835 2e34 3c2f  >.    <td>85.4</
+00001570: 7464 3e0a 2020 2020 3c74 643e 3937 2e33  td>.    <td>97.3
+00001580: 3c2f 7464 3e0a 2020 2020 3c74 643e 3834  </td>.    <td>84
+00001590: 393c 2f74 643e 0a20 2020 203c 7464 3e32  9</td>.    <td>2
+000015a0: 3234 7832 3234 3c2f 7464 3e0a 2020 2020  24x224</td>.    
+000015b0: 3c74 643e 3432 342e 363c 2f74 643e 0a20  <td>424.6</td>. 
+000015c0: 2020 203c 7464 3e33 362e 363c 2f74 643e     <td>36.6</td>
+000015d0: 0a20 2020 203c 7464 3e3c 6120 6872 6566  .    <td><a href
+000015e0: 3d22 6874 7470 733a 2f2f 6472 6976 652e  ="https://drive.
+000015f0: 676f 6f67 6c65 2e63 6f6d 2f75 633f 6578  google.com/uc?ex
+00001600: 706f 7274 3d64 6f77 6e6c 6f61 6426 6964  port=download&id
+00001610: 3d31 6759 6858 4133 3251 2d5f 3943 3544  =1gYhXA32Q-_9C5D
+00001620: 5865 6c31 3761 7656 5f5a 4c6f 6148 7764  Xel17avV_ZLoaHwd
+00001630: 677a 223e 6d6f 6465 6c3c 2f61 3e3c 2f74  gz">model</a></t
+00001640: 643e 0a3c 2f74 723e 0a0a 3c74 723e 0a20  d>.</tr>..<tr>. 
+00001650: 2020 203c 7464 3e46 6173 7465 7256 6954     <td>FasterViT
+00001660: 2d35 3c2f 7464 3e0a 2020 2020 3c74 643e  -5</td>.    <td>
+00001670: 3835 2e36 3c2f 7464 3e0a 2020 2020 3c74  85.6</td>.    <t
+00001680: 643e 3937 2e34 3c2f 7464 3e0a 2020 2020  d>97.4</td>.    
+00001690: 3c74 643e 3434 393c 2f74 643e 0a20 2020  <td>449</td>.   
+000016a0: 203c 7464 3e32 3234 7832 3234 3c2f 7464   <td>224x224</td
+000016b0: 3e0a 2020 2020 3c74 643e 3937 352e 353c  >.    <td>975.5<
+000016c0: 2f74 643e 0a20 2020 203c 7464 3e31 3133  /td>.    <td>113
+000016d0: 2e30 3c2f 7464 3e0a 2020 2020 3c74 643e  .0</td>.    <td>
+000016e0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000016f0: 2f64 7269 7665 2e67 6f6f 676c 652e 636f  /drive.google.co
+00001700: 6d2f 7563 3f65 7870 6f72 743d 646f 776e  m/uc?export=down
+00001710: 6c6f 6164 2669 643d 316d 7170 6169 3758  load&id=1mqpai7X
+00001720: 6948 4c72 5f6e 3174 6a78 6a7a 5438 7133  iHLr_n1tjxjzT8q3
+00001730: 3639 7854 4371 5f7a 2d22 3e6d 6f64 656c  69xTCq_z-">model
+00001740: 3c2f 613e 3c2f 7464 3e0a 3c2f 7472 3e0a  </a></td>.</tr>.
+00001750: 0a3c 7472 3e0a 2020 2020 3c74 643e 4661  .<tr>.    <td>Fa
+00001760: 7374 6572 5669 542d 363c 2f74 643e 0a20  sterViT-6</td>. 
+00001770: 2020 203c 7464 3e38 352e 383c 2f74 643e     <td>85.8</td>
+00001780: 0a20 2020 203c 7464 3e39 372e 343c 2f74  .    <td>97.4</t
+00001790: 643e 0a20 2020 203c 7464 3e33 3532 3c2f  d>.    <td>352</
+000017a0: 7464 3e0a 2020 2020 3c74 643e 3232 3478  td>.    <td>224x
+000017b0: 3232 343c 2f74 643e 0a20 2020 203c 7464  224</td>.    <td
+000017c0: 3e31 3336 302e 303c 2f74 643e 0a20 2020  >1360.0</td>.   
+000017d0: 203c 7464 3e31 3432 2e30 3c2f 7464 3e0a   <td>142.0</td>.
+000017e0: 2020 2020 3c74 643e 3c61 2068 7265 663d      <td><a href=
+000017f0: 2268 7474 7073 3a2f 2f64 7269 7665 2e67  "https://drive.g
+00001800: 6f6f 676c 652e 636f 6d2f 7563 3f65 7870  oogle.com/uc?exp
+00001810: 6f72 743d 646f 776e 6c6f 6164 2669 643d  ort=download&id=
+00001820: 3132 6a74 6176 5232 5178 6d4d 7a63 4b77  12jtavR2QxmMzcKw
+00001830: 507a 5765 376b 772d 6f79 3334 4959 6935  PzWe7kw-oy34IYi5
+00001840: 3922 3e6d 6f64 656c 3c2f 613e 3c2f 7464  9">model</a></td
+00001850: 3e0a 3c2f 7472 3e0a 0a3c 2f74 6162 6c65  >.</tr>..</table
+00001860: 3e0a 0a0a 2323 2320 526f 6275 7374 6e65  >...### Robustne
+00001870: 7373 2028 496d 6167 654e 6574 2d41 202d  ss (ImageNet-A -
+00001880: 2049 6d61 6765 4e65 742d 5220 2d20 496d   ImageNet-R - Im
+00001890: 6167 654e 6574 2d56 3229 0a0a 416c 6c20  ageNet-V2)..All 
+000018a0: 6d6f 6465 6c73 2075 7365 2060 6372 6f70  models use `crop
+000018b0: 5f70 6374 3d30 2e38 3735 602e 2052 6573  _pct=0.875`. Res
+000018c0: 756c 7473 2061 7265 206f 6274 6169 6e65  ults are obtaine
+000018d0: 6420 6279 2072 756e 6e69 6e67 2069 6e66  d by running inf
+000018e0: 6572 656e 6365 206f 6e20 496d 6167 654e  erence on ImageN
+000018f0: 6574 2d31 4b20 7072 6574 7261 696e 6564  et-1K pretrained
+00001900: 206d 6f64 656c 7320 7769 7468 6f75 7420   models without 
+00001910: 6669 6e65 7475 6e69 6e67 2e0a 3c74 6162  finetuning..<tab
+00001920: 6c65 3e0a 2020 3c74 723e 0a20 2020 203c  le>.  <tr>.    <
+00001930: 7468 3e4e 616d 653c 2f74 683e 0a20 2020  th>Name</th>.   
+00001940: 203c 7468 3e41 2d41 6363 4031 2825 293c   <th>A-Acc@1(%)<
+00001950: 2f74 683e 0a20 2020 203c 7468 3e41 2d41  /th>.    <th>A-A
+00001960: 6363 4035 2825 293c 2f74 683e 0a20 2020  cc@5(%)</th>.   
+00001970: 203c 7468 3e52 2d41 6363 4031 2825 293c   <th>R-Acc@1(%)<
+00001980: 2f74 683e 0a20 2020 203c 7468 3e52 2d41  /th>.    <th>R-A
+00001990: 6363 4035 2825 293c 2f74 683e 0a20 2020  cc@5(%)</th>.   
+000019a0: 203c 7468 3e56 322d 4163 6340 3128 2529   <th>V2-Acc@1(%)
+000019b0: 3c2f 7468 3e0a 2020 2020 3c74 683e 5632  </th>.    <th>V2
+000019c0: 2d41 6363 4035 2825 293c 2f74 683e 0a20  -Acc@5(%)</th>. 
+000019d0: 203c 2f74 723e 0a0a 3c74 723e 0a20 2020   </tr>..<tr>.   
+000019e0: 203c 7464 3e46 6173 7465 7256 6954 2d30   <td>FasterViT-0
+000019f0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3233  </td>.    <td>23
+00001a00: 2e39 3c2f 7464 3e0a 2020 2020 3c74 643e  .9</td>.    <td>
+00001a10: 3537 2e36 3c2f 7464 3e0a 2020 2020 3c74  57.6</td>.    <t
+00001a20: 643e 3435 2e39 3c2f 7464 3e0a 2020 2020  d>45.9</td>.    
+00001a30: 3c74 643e 3630 2e34 3c2f 7464 3e0a 2020  <td>60.4</td>.  
+00001a40: 2020 3c74 643e 3730 2e39 3c2f 7464 3e0a    <td>70.9</td>.
+00001a50: 2020 2020 3c74 643e 3930 2e30 3c2f 7464      <td>90.0</td
+00001a60: 3e0a 3c2f 7472 3e0a 0a3c 7472 3e0a 2020  >.</tr>..<tr>.  
+00001a70: 2020 3c74 643e 4661 7374 6572 5669 542d    <td>FasterViT-
+00001a80: 313c 2f74 643e 0a20 2020 203c 7464 3e33  1</td>.    <td>3
+00001a90: 312e 323c 2f74 643e 0a20 2020 203c 7464  1.2</td>.    <td
+00001aa0: 3e36 332e 333c 2f74 643e 0a20 2020 203c  >63.3</td>.    <
+00001ab0: 7464 3e34 372e 353c 2f74 643e 0a20 2020  td>47.5</td>.   
+00001ac0: 203c 7464 3e36 312e 393c 2f74 643e 0a20   <td>61.9</td>. 
+00001ad0: 2020 203c 7464 3e37 322e 363c 2f74 643e     <td>72.6</td>
+00001ae0: 0a20 2020 203c 7464 3e39 312e 303c 2f74  .    <td>91.0</t
+00001af0: 643e 0a3c 2f74 723e 0a0a 3c74 723e 0a20  d>.</tr>..<tr>. 
+00001b00: 2020 203c 7464 3e46 6173 7465 7256 6954     <td>FasterViT
+00001b10: 2d32 3c2f 7464 3e0a 2020 2020 3c74 643e  -2</td>.    <td>
+00001b20: 3338 2e32 3c2f 7464 3e0a 2020 2020 3c74  38.2</td>.    <t
+00001b30: 643e 3638 2e39 3c2f 7464 3e0a 2020 2020  d>68.9</td>.    
+00001b40: 3c74 643e 3439 2e36 3c2f 7464 3e0a 2020  <td>49.6</td>.  
+00001b50: 2020 3c74 643e 3633 2e34 3c2f 7464 3e0a    <td>63.4</td>.
+00001b60: 2020 2020 3c74 643e 3733 2e37 3c2f 7464      <td>73.7</td
+00001b70: 3e0a 2020 2020 3c74 643e 3931 2e36 3c2f  >.    <td>91.6</
+00001b80: 7464 3e0a 3c2f 7472 3e0a 0a3c 7472 3e0a  td>.</tr>..<tr>.
+00001b90: 2020 2020 3c74 643e 4661 7374 6572 5669      <td>FasterVi
+00001ba0: 542d 333c 2f74 643e 0a20 2020 203c 7464  T-3</td>.    <td
+00001bb0: 3e34 342e 323c 2f74 643e 0a20 2020 203c  >44.2</td>.    <
+00001bc0: 7464 3e37 332e 303c 2f74 643e 0a20 2020  td>73.0</td>.   
+00001bd0: 203c 7464 3e35 312e 393c 2f74 643e 0a20   <td>51.9</td>. 
+00001be0: 2020 203c 7464 3e36 352e 363c 2f74 643e     <td>65.6</td>
+00001bf0: 0a20 2020 203c 7464 3e37 352e 303c 2f74  .    <td>75.0</t
+00001c00: 643e 0a20 2020 203c 7464 3e39 322e 323c  d>.    <td>92.2<
+00001c10: 2f74 643e 0a3c 2f74 723e 0a0a 3c74 723e  /td>.</tr>..<tr>
+00001c20: 0a20 2020 203c 7464 3e46 6173 7465 7256  .    <td>FasterV
+00001c30: 6954 2d34 3c2f 7464 3e0a 2020 2020 3c74  iT-4</td>.    <t
+00001c40: 643e 3439 2e30 3c2f 7464 3e0a 2020 2020  d>49.0</td>.    
+00001c50: 3c74 643e 3735 2e34 3c2f 7464 3e0a 2020  <td>75.4</td>.  
+00001c60: 2020 3c74 643e 3536 2e30 3c2f 7464 3e0a    <td>56.0</td>.
+00001c70: 2020 2020 3c74 643e 3639 2e36 3c2f 7464      <td>69.6</td
+00001c80: 3e0a 2020 2020 3c74 643e 3735 2e37 3c2f  >.    <td>75.7</
+00001c90: 7464 3e0a 2020 2020 3c74 643e 3932 2e37  td>.    <td>92.7
+00001ca0: 3c2f 7464 3e0a 3c2f 7472 3e0a 0a3c 7472  </td>.</tr>..<tr
+00001cb0: 3e0a 2020 2020 3c74 643e 4661 7374 6572  >.    <td>Faster
+00001cc0: 5669 542d 353c 2f74 643e 0a20 2020 203c  ViT-5</td>.    <
+00001cd0: 7464 3e35 322e 373c 2f74 643e 0a20 2020  td>52.7</td>.   
+00001ce0: 203c 7464 3e37 372e 363c 2f74 643e 0a20   <td>77.6</td>. 
+00001cf0: 2020 203c 7464 3e35 362e 393c 2f74 643e     <td>56.9</td>
+00001d00: 0a20 2020 203c 7464 3e37 302e 303c 2f74  .    <td>70.0</t
+00001d10: 643e 0a20 2020 203c 7464 3e37 362e 303c  d>.    <td>76.0<
+00001d20: 2f74 643e 0a20 2020 203c 7464 3e39 332e  /td>.    <td>93.
+00001d30: 303c 2f74 643e 0a3c 2f74 723e 0a0a 3c74  0</td>.</tr>..<t
+00001d40: 723e 0a20 2020 203c 7464 3e46 6173 7465  r>.    <td>Faste
+00001d50: 7256 6954 2d36 3c2f 7464 3e0a 2020 2020  rViT-6</td>.    
+00001d60: 3c74 643e 3533 2e37 3c2f 7464 3e0a 2020  <td>53.7</td>.  
+00001d70: 2020 3c74 643e 3738 2e34 3c2f 7464 3e0a    <td>78.4</td>.
+00001d80: 2020 2020 3c74 643e 3537 2e31 3c2f 7464      <td>57.1</td
+00001d90: 3e0a 2020 2020 3c74 643e 3730 2e31 3c2f  >.    <td>70.1</
+00001da0: 7464 3e0a 2020 2020 3c74 643e 3736 2e31  td>.    <td>76.1
+00001db0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3933  </td>.    <td>93
+00001dc0: 2e30 3c2f 7464 3e0a 3c2f 7472 3e0a 0a3c  .0</td>.</tr>..<
+00001dd0: 2f74 6162 6c65 3e0a 0a41 2c20 5220 616e  /table>..A, R an
+00001de0: 6420 5632 2064 656e 6f74 6520 496d 6167  d V2 denote Imag
+00001df0: 654e 6574 2d41 2c20 496d 6167 654e 6574  eNet-A, ImageNet
+00001e00: 2d52 2061 6e64 2049 6d61 6765 4e65 742d  -R and ImageNet-
+00001e10: 5632 2072 6573 7065 6374 6976 656c 792e  V2 respectively.
+00001e20: 200a 2323 2054 7261 696e 696e 670a 0a50   .## Training..P
+00001e30: 6c65 6173 6520 7365 6520 5b54 5241 494e  lease see [TRAIN
+00001e40: 494e 472e 6d64 5d28 5452 4149 4e49 4e47  ING.md](TRAINING
+00001e50: 2e6d 6429 2066 6f72 2064 6574 6169 6c65  .md) for detaile
+00001e60: 6420 7472 6169 6e69 6e67 2069 6e73 7472  d training instr
+00001e70: 7563 7469 6f6e 7320 6f66 2061 6c6c 206d  uctions of all m
+00001e80: 6f64 656c 732e 200a 0a23 2320 4576 616c  odels. ..## Eval
+00001e90: 7561 7469 6f6e 0a0a 5468 6520 4661 7374  uation..The Fast
+00001ea0: 6572 5669 5420 6d6f 6465 6c73 2063 616e  erViT models can
+00001eb0: 2062 6520 6576 616c 7561 7465 6420 6f6e   be evaluated on
+00001ec0: 2049 6d61 6765 4e65 742d 314b 2076 616c   ImageNet-1K val
+00001ed0: 6964 6174 696f 6e20 7365 7420 7573 696e  idation set usin
+00001ee0: 6720 7468 6520 666f 6c6c 6f77 696e 673a  g the following:
+00001ef0: 200a 0a60 6060 0a70 7974 686f 6e20 7661   ..```.python va
+00001f00: 6c69 6461 7465 2e70 7920 5c0a 2d2d 6d6f  lidate.py \.--mo
+00001f10: 6465 6c20 3c6d 6f64 656c 2d6e 616d 653e  del <model-name>
+00001f20: 0a2d 2d63 6865 636b 706f 696e 7420 3c63  .--checkpoint <c
+00001f30: 6865 636b 706f 696e 742d 7061 7468 3e0a  heckpoint-path>.
+00001f40: 2d2d 6461 7461 5f64 6972 203c 696d 6167  --data_dir <imag
+00001f50: 656e 6574 2d70 6174 683e 0a2d 2d62 6174  enet-path>.--bat
+00001f60: 6368 2d73 697a 6520 3c62 6174 6368 2d73  ch-size <batch-s
+00001f70: 697a 652d 7065 722d 6770 750a 6060 6020  ize-per-gpu.``` 
+00001f80: 0a0a 4865 7265 2060 2d2d 6d6f 6465 6c60  ..Here `--model`
+00001f90: 2069 7320 7468 6520 4661 7374 6572 5669   is the FasterVi
+00001fa0: 5420 7661 7269 616e 7420 2865 2e67 2e20  T variant (e.g. 
+00001fb0: 6066 6173 7465 725f 7669 745f 305f 3232  `faster_vit_0_22
+00001fc0: 345f 316b 6029 2c20 602d 2d63 6865 636b  4_1k`), `--check
+00001fd0: 706f 696e 7460 2069 7320 7468 6520 7061  point` is the pa
+00001fe0: 7468 2074 6f20 7072 6574 7261 696e 6564  th to pretrained
+00001ff0: 206d 6f64 656c 2077 6569 6768 7473 2c20   model weights, 
+00002000: 602d 2d64 6174 615f 6469 7260 2069 7320  `--data_dir` is 
+00002010: 7468 6520 7061 7468 2074 6f20 496d 6167  the path to Imag
+00002020: 654e 6574 2d31 4b20 7661 6c69 6461 7469  eNet-1K validati
+00002030: 6f6e 2073 6574 2061 6e64 2060 2d2d 6261  on set and `--ba
+00002040: 7463 682d 7369 7a65 6020 6973 2074 6865  tch-size` is the
+00002050: 206e 756d 6265 7220 6f66 2062 6174 6368   number of batch
+00002060: 2073 697a 652e 2057 6520 616c 736f 2070   size. We also p
+00002070: 726f 7669 6465 2061 2073 616d 706c 6520  rovide a sample 
+00002080: 7363 7269 7074 205b 6865 7265 5d28 2e2f  script [here](./
+00002090: 6661 7374 6572 7669 742f 7661 6c69 6461  fastervit/valida
+000020a0: 7465 2e73 6829 2e20 0a0a 0a23 2320 496e  te.sh). ...## In
+000020b0: 7374 616c 6c61 7469 6f6e 0a0a 5468 6520  stallation..The 
+000020c0: 6465 7065 6e64 656e 6369 6573 2063 616e  dependencies can
+000020d0: 2062 6520 696e 7374 616c 6c65 6420 6279   be installed by
+000020e0: 2072 756e 6e69 6e67 3a0a 0a60 6060 6261   running:..```ba
+000020f0: 7368 0a70 6970 2069 6e73 7461 6c6c 202d  sh.pip install -
+00002100: 7220 7265 7175 6972 656d 656e 7473 2e74  r requirements.t
+00002110: 7874 0a60 6060 0a0a 2323 2054 6869 7264  xt.```..## Third
+00002120: 2d70 6172 7479 2045 7874 656e 7469 6f6e  -party Extention
+00002130: 730a 5765 2061 6c77 6179 7320 7765 6c63  s.We always welc
+00002140: 6f6d 6520 7468 6972 642d 7061 7274 7920  ome third-party 
+00002150: 6578 7465 6e74 696f 6e73 2f69 6d70 6c65  extentions/imple
+00002160: 6d65 6e74 6174 696f 6e73 2061 6e64 2075  mentations and u
+00002170: 7361 6765 2066 6f72 206f 7468 6572 2070  sage for other p
+00002180: 7572 706f 7365 732e 2049 6620 796f 7520  urposes. If you 
+00002190: 776f 756c 6420 6c69 6b65 2079 6f75 7220  would like your 
+000021a0: 776f 726b 2074 6f20 6265 206c 6973 7465  work to be liste
+000021b0: 6420 696e 2074 6869 7320 7265 706f 7369  d in this reposi
+000021c0: 746f 7279 2c20 706c 6561 7365 2072 6169  tory, please rai
+000021d0: 7365 2061 6e64 2069 7373 7565 2061 6e64  se and issue and
+000021e0: 2070 726f 7669 6465 2075 7320 7769 7468   provide us with
+000021f0: 2064 6574 6169 6c65 6420 696e 666f 726d   detailed inform
+00002200: 6174 696f 6e2e 2020 0a0a 0a23 2320 4163  ation.  ...## Ac
+00002210: 6b6e 6f77 6c65 6467 656d 656e 740a 5468  knowledgement.Th
+00002220: 6973 2072 6570 6f73 6974 6f72 7920 6973  is repository is
+00002230: 2062 7569 6c74 206f 6e20 746f 7020 6f66   built on top of
+00002240: 2074 6865 205b 7469 6d6d 5d28 6874 7470   the [timm](http
+00002250: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
+00002260: 7567 6769 6e67 6661 6365 2f70 7974 6f72  uggingface/pytor
+00002270: 6368 2d69 6d61 6765 2d6d 6f64 656c 7329  ch-image-models)
+00002280: 2072 6570 6f73 6974 6f72 792e 2057 6520   repository. We 
+00002290: 7468 616e 6b20 5b52 6f73 7320 5772 6967  thank [Ross Wrig
+000022a0: 6874 6d61 6e5d 2868 7474 7073 3a2f 2f72  htman](https://r
+000022b0: 7769 6768 746d 616e 2e63 6f6d 2f29 2066  wightman.com/) f
+000022c0: 6f72 2063 7265 6174 696e 6720 616e 6420  or creating and 
+000022d0: 6d61 696e 7461 696e 696e 6720 7468 6973  maintaining this
+000022e0: 2068 6967 682d 7175 616c 6974 7920 6c69   high-quality li
+000022f0: 6272 6172 792e 2020 0a0a 2323 2043 6974  brary.  ..## Cit
+00002300: 6174 696f 6e0a 0a50 6c65 6173 6520 636f  ation..Please co
+00002310: 6e73 6964 6572 2063 6974 696e 6720 4661  nsider citing Fa
+00002320: 7374 6572 5669 5420 6966 2074 6869 7320  sterViT if this 
+00002330: 7265 706f 7369 746f 7279 2069 7320 7573  repository is us
+00002340: 6566 756c 2066 6f72 2079 6f75 7220 776f  eful for your wo
+00002350: 726b 3a0a 0a60 6060 0a40 6172 7469 636c  rk:..```.@articl
+00002360: 657b 6861 7461 6d69 7a61 6465 6832 3032  e{hatamizadeh202
+00002370: 3366 6173 7465 7276 6974 2c0a 2020 7469  3fastervit,.  ti
+00002380: 746c 653d 7b46 6173 7465 7256 6954 3a20  tle={FasterViT: 
+00002390: 4661 7374 2056 6973 696f 6e20 5472 616e  Fast Vision Tran
+000023a0: 7366 6f72 6d65 7273 2077 6974 6820 4869  sformers with Hi
+000023b0: 6572 6172 6368 6963 616c 2041 7474 656e  erarchical Atten
+000023c0: 7469 6f6e 7d2c 0a20 2061 7574 686f 723d  tion},.  author=
+000023d0: 7b48 6174 616d 697a 6164 6568 2c20 416c  {Hatamizadeh, Al
+000023e0: 6920 616e 6420 4865 696e 7269 6368 2c20  i and Heinrich, 
+000023f0: 4772 6567 2061 6e64 2059 696e 2c20 486f  Greg and Yin, Ho
+00002400: 6e67 7875 2061 6e64 2054 616f 2c20 416e  ngxu and Tao, An
+00002410: 6472 6577 2061 6e64 2041 6c76 6172 657a  drew and Alvarez
+00002420: 2c20 4a6f 7365 204d 2061 6e64 204b 6175  , Jose M and Kau
+00002430: 747a 2c20 4a61 6e20 616e 6420 4d6f 6c63  tz, Jan and Molc
+00002440: 6861 6e6f 762c 2050 6176 6c6f 7d2c 0a20  hanov, Pavlo},. 
+00002450: 206a 6f75 726e 616c 3d7b 6172 5869 7620   journal={arXiv 
+00002460: 7072 6570 7269 6e74 2061 7258 6976 3a32  preprint arXiv:2
+00002470: 3330 362e 3036 3138 397d 2c0a 2020 7965  306.06189},.  ye
+00002480: 6172 3d7b 3230 3233 7d0a 7d0a 6060 600a  ar={2023}.}.```.
+00002490: 0a23 2320 4c69 6365 6e73 6573 0a0a 436f  .## Licenses..Co
+000024a0: 7079 7269 6768 7420 c2a9 2032 3032 332c  pyright .. 2023,
+000024b0: 204e 5649 4449 4120 436f 7270 6f72 6174   NVIDIA Corporat
+000024c0: 696f 6e2e 2041 6c6c 2072 6967 6874 7320  ion. All rights 
+000024d0: 7265 7365 7276 6564 2e0a 0a54 6869 7320  reserved...This 
+000024e0: 776f 726b 2069 7320 6d61 6465 2061 7661  work is made ava
+000024f0: 696c 6162 6c65 2075 6e64 6572 2074 6865  ilable under the
+00002500: 204e 5649 4449 4120 536f 7572 6365 2043   NVIDIA Source C
+00002510: 6f64 6520 4c69 6365 6e73 652d 4e43 2e20  ode License-NC. 
+00002520: 436c 6963 6b20 5b68 6572 655d 284c 4943  Click [here](LIC
+00002530: 454e 5345 2920 746f 2076 6965 7720 6120  ENSE) to view a 
+00002540: 636f 7079 206f 6620 7468 6973 206c 6963  copy of this lic
+00002550: 656e 7365 2e0a 0a46 6f72 206c 6963 656e  ense...For licen
+00002560: 7365 2069 6e66 6f72 6d61 7469 6f6e 2072  se information r
+00002570: 6567 6172 6469 6e67 2074 6865 2074 696d  egarding the tim
+00002580: 6d20 7265 706f 7369 746f 7279 2c20 706c  m repository, pl
+00002590: 6561 7365 2072 6566 6572 2074 6f20 6974  ease refer to it
+000025a0: 7320 5b72 6570 6f73 6974 6f72 795d 2868  s [repository](h
+000025b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000025c0: 6d2f 7277 6967 6874 6d61 6e2f 7079 746f  m/rwightman/pyto
+000025d0: 7263 682d 696d 6167 652d 6d6f 6465 6c73  rch-image-models
+000025e0: 292e 0a0a 466f 7220 6c69 6365 6e73 6520  )...For license 
+000025f0: 696e 666f 726d 6174 696f 6e20 7265 6761  information rega
+00002600: 7264 696e 6720 7468 6520 496d 6167 654e  rding the ImageN
+00002610: 6574 2064 6174 6173 6574 2c20 706c 6561  et dataset, plea
+00002620: 7365 2073 6565 2074 6865 205b 496d 6167  se see the [Imag
+00002630: 654e 6574 206f 6666 6963 6961 6c20 7765  eNet official we
+00002640: 6273 6974 655d 2868 7474 7073 3a2f 2f77  bsite](https://w
+00002650: 7777 2e69 6d61 6765 2d6e 6574 2e6f 7267  ww.image-net.org
+00002660: 2f29 2e20 0a0a                           /). ..
```

### Comparing `fastervit-0.8.8/README.md` & `fastervit-0.8.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,23 +14,32 @@
 
 
 --- 
 
 FasterViT achieves a new SOTA Pareto-front in
 terms of accuracy vs. image throughput (no extra training data !)
 
-![teaser](./fastervit/assets/plot.png)
+<p align="center">
+<img src="https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-6cdd16bfccc1" width=62% height=62% 
+class="center">
+</p>
 
 
+<!-- We introduce a new self-attention mechanism, denoted as Hierarchical
+Attention (HAT), that captures both short and long-range information by learning
+cross-window carrier tokens.
 
-## 💥 News 💥
+![teaser](./fastervit/assets/hierarchial_attn.png) -->
+
+
+<!-- ## 💥 News 💥
 
 - **[06.18.2023]** 🔥 We have released the FasterViT [pip package](https://pypi.org/project/fastervit/) !
 - **[06.17.2023]** 🔥 [Any-resolution FasterViT](./fastervit/models/faster_vit_any_res.py)  model is now available ! the model can be used for variety of applications such as detection and segmentation or high-resolution fine-tuning with arbitrary input image resolutions. 
-- **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models !
+- **[06.09.2023]** 🔥🔥 We have released source code and ImageNet-1K FasterViT-models ! -->
 
 ## Quick Start
 
 The FasterViT can be conveniently installed by:
 
 ```bash
 pip install fastervit
@@ -56,23 +65,24 @@
 >>> model = create_model('faster_vit_1_any_res', 
                           resolution=[576, 960],
                           window_size=[7, 7, 12, 6],
                           ct_size=2,
                           dim=128)
 ```
 
-## Catalog
+<!-- ## Catalog
 - [x] ImageNet-1K training code
 - [x] ImageNet-1K pre-trained models
 - [x] Any-resolution FasterViT
 - [x] FasterViT pip-package release
+- [ ] Update training scripts to support model.compile, 
 - [ ] ImageNet-21K pre-trained models
 - [ ] ImageNet-21K fine-tune scripts
 - [ ] Detection code (DINO) + models
-- [ ] Segmentation code + models
+- [ ] Segmentation code + models -->
 
 --- 
 
 ## Results + Pretrained Models
 
 ### ImageNet-1K
 **FasterViT ImageNet-1K Pretrained Models**
@@ -308,7 +318,8 @@
 Copyright © 2023, NVIDIA Corporation. All rights reserved.
 
 This work is made available under the NVIDIA Source Code License-NC. Click [here](LICENSE) to view a copy of this license.
 
 For license information regarding the timm repository, please refer to its [repository](https://github.com/rwightman/pytorch-image-models).
 
 For license information regarding the ImageNet dataset, please see the [ImageNet official website](https://www.image-net.org/). 
+
```

#### html2text {}

```diff
@@ -5,38 +5,30 @@
 developer.nvidia.com/blog/author/gheinrich/), [Hongxu (Danny) Yin](https://
 scholar.princeton.edu/hongxu), [Andrew Tao](https://developer.nvidia.com/blog/
 author/atao/), [Jose M. Alvarez](https://alvarezlopezjosem.github.io/), [Jan
 Kautz](https://jankautz.com/), [Pavlo Molchanov](https://www.pmolchanov.com/).
 For business inquiries, please visit our website and submit the form: [NVIDIA
 Research Licensing](https://www.nvidia.com/en-us/research/inquiries/) --
 - FasterViT achieves a new SOTA Pareto-front in terms of accuracy vs. image
-throughput (no extra training data !) ![teaser](./fastervit/assets/plot.png) ##
-ð¥ News ð¥ - **[06.18.2023]** ð¥ We have released the FasterViT [pip
-package](https://pypi.org/project/fastervit/) ! - **[06.17.2023]** ð¥ [Any-
-resolution FasterViT](./fastervit/models/faster_vit_any_res.py) model is now
-available ! the model can be used for variety of applications such as detection
-and segmentation or high-resolution fine-tuning with arbitrary input image
-resolutions. - **[06.09.2023]** ð¥ð¥ We have released source code and
-ImageNet-1K FasterViT-models ! ## Quick Start The FasterViT can be conveniently
-installed by: ```bash pip install fastervit ``` A FasterViT model with default
-hyper-parameters can be created as in the following: ```python >>> from
-fastervit import create_model # Define fastervit-0 model with 224 x 224
-resolution >>> model = create_model('faster_vit_0_224') ``` We can also use the
-any-resolution FasterViT model to accommodate arbitrary image resolutions. In
-the following, we define an any-resolution FasterViT-1 model with input
-resolution of 576 x 960, window sizes of 12 and 6 in 3rd and 4th stages,
-carrier token size of 2 and embedding dimension of 128: ```python >>> from
-fastervit import create_model # Define any-resolution FasterViT-1 model with
-576 x 960 resolution >>> model = create_model('faster_vit_1_any_res',
-resolution=[576, 960], window_size=[7, 7, 12, 6], ct_size=2, dim=128) ``` ##
-Catalog - [x] ImageNet-1K training code - [x] ImageNet-1K pre-trained models -
-[x] Any-resolution FasterViT - [x] FasterViT pip-package release - [ ]
-ImageNet-21K pre-trained models - [ ] ImageNet-21K fine-tune scripts - [ ]
-Detection code (DINO) + models - [ ] Segmentation code + models --- ## Results
-+ Pretrained Models ### ImageNet-1K **FasterViT ImageNet-1K Pretrained Models**
+throughput (no extra training data !)
+ [https://github.com/NVlabs/FasterViT/assets/26806394/253d1a2e-b5f5-4a9b-a362-
+                                 6cdd16bfccc1]
+  ## Quick Start The FasterViT can be conveniently installed by: ```bash pip
+install fastervit ``` A FasterViT model with default hyper-parameters can be
+created as in the following: ```python >>> from fastervit import create_model #
+Define fastervit-0 model with 224 x 224 resolution >>> model = create_model
+('faster_vit_0_224') ``` We can also use the any-resolution FasterViT model to
+accommodate arbitrary image resolutions. In the following, we define an any-
+resolution FasterViT-1 model with input resolution of 576 x 960, window sizes
+of 12 and 6 in 3rd and 4th stages, carrier token size of 2 and embedding
+dimension of 128: ```python >>> from fastervit import create_model # Define
+any-resolution FasterViT-1 model with 576 x 960 resolution >>> model =
+create_model('faster_vit_1_any_res', resolution=[576, 960], window_size=[7, 7,
+12, 6], ct_size=2, dim=128) ```  --- ## Results + Pretrained Models ###
+ImageNet-1K **FasterViT ImageNet-1K Pretrained Models**
 Name       Acc@1(%) Acc@5(%) Throughput Resolution #Params(M) FLOPs(G) Download
                              (Img/Sec)
 FasterViT- 82.1     95.9     5802       224x224    31.4       3.3      model
 0
 FasterViT- 83.2     96.5     4188       224x224    53.4       5.3      model
 1
 FasterViT- 84.2     96.8     3161       224x224    75.9       8.7      model
```

### Comparing `fastervit-0.8.8/fastervit/assets/hierarchial_attn.png` & `fastervit-0.8.9/fastervit/assets/hierarchial_attn.png`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.8/fastervit/models/faster_vit.py` & `fastervit-0.8.9/fastervit/models/faster_vit.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,18 +65,17 @@
 def window_partition(x, window_size):
     B, C, H, W = x.shape
     x = x.view(B, C, H // window_size, window_size, W // window_size, window_size)
     windows = x.permute(0, 2, 4, 3, 5, 1).reshape(-1, window_size*window_size, C)
     return windows
 
 
-def window_reverse(windows, window_size, H, W):
-    B = int(windows.shape[0] / (H * W / window_size / window_size))
-    x = windows.reshape(B, H // window_size, W // window_size, window_size, window_size, -1)
-    x = x.permute(0, 5, 1, 3, 2, 4).reshape(B,windows.shape[2], H, W)
+def window_reverse(windows, window_size, H, W, B):
+    x = windows.view(B, H // window_size, W // window_size, window_size, window_size, -1)
+    x = x.permute(0, 5, 1, 3, 2, 4).reshape(B, windows.shape[2], H, W)
     return x
 
 
 def ct_dewindow(ct, W, H, window_size):
     bs = ct.shape[0]
     N=ct.shape[2]
     ct2 = ct.view(-1, W//window_size, H//window_size, window_size, window_size, N).permute(0, 5, 1, 3, 2, 4)
@@ -847,15 +846,15 @@
         ct = self.global_tokenizer(x) if self.do_gt else None
         B, C, H, W = x.shape
         if self.transformer_block:
             x = window_partition(x, self.window_size)
         for bn, blk in enumerate(self.blocks):
             x, ct = blk(x, ct)
         if self.transformer_block:
-            x = window_reverse(x, self.window_size, H, W)
+            x = window_reverse(x, self.window_size, H, W, B)
         if self.downsample is None:
             return x
         return self.downsample(x)
 
 
 class FasterViT(nn.Module):
     """
```

### Comparing `fastervit-0.8.8/fastervit/models/faster_vit_any_res.py` & `fastervit-0.8.9/fastervit/models/faster_vit_any_res.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,18 +65,17 @@
 def window_partition(x, window_size):
     B, C, H, W = x.shape
     x = x.view(B, C, H // window_size, window_size, W // window_size, window_size)
     windows = x.permute(0, 2, 4, 3, 5, 1).reshape(-1, window_size*window_size, C)
     return windows
 
 
-def window_reverse(windows, window_size, H, W):
-    B = int(windows.shape[0] / (H * W / window_size / window_size))
-    x = windows.reshape(B, H // window_size, W // window_size, window_size, window_size, -1)
-    x = x.permute(0, 5, 1, 3, 2, 4).reshape(B,windows.shape[2], H, W)
+def window_reverse(windows, window_size, H, W, B):
+    x = windows.view(B, H // window_size, W // window_size, window_size, window_size, -1)
+    x = x.permute(0, 5, 1, 3, 2, 4).reshape(B, windows.shape[2], H, W)
     return x
 
 
 def ct_dewindow(ct, W, H, window_size):
     bs = ct.shape[0]
     N=ct.shape[2]
     ct2 = ct.view(-1, W//window_size, H//window_size, window_size, window_size, N).permute(0, 5, 1, 3, 2, 4)
@@ -870,15 +869,15 @@
         ct = self.global_tokenizer(x) if self.do_gt else None
         if self.transformer_block:
             x = window_partition(x, self.window_size)
         for bn, blk in enumerate(self.blocks):
             x, ct = blk(x, ct)
         if self.transformer_block:
             x = window_reverse(x, self
-                               .window_size, Hp, Wp)
+                               .window_size, Hp, Wp, B)
             if pad_r > 0 or pad_b > 0:
                 x = x[:, :, :H, :W].contiguous()
         if self.downsample is None:
             return x
         return self.downsample(x)
```

### Comparing `fastervit-0.8.8/fastervit/models/registry.py` & `fastervit-0.8.9/fastervit/models/registry.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.8/fastervit/scheduler/cosine_lr.py` & `fastervit-0.8.9/fastervit/scheduler/cosine_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.8/fastervit/scheduler/multistep_lr.py` & `fastervit-0.8.9/fastervit/scheduler/multistep_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.8/fastervit/scheduler/plateau_lr.py` & `fastervit-0.8.9/fastervit/scheduler/plateau_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.8/fastervit/scheduler/poly_lr.py` & `fastervit-0.8.9/fastervit/scheduler/poly_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.8/fastervit/scheduler/scheduler.py` & `fastervit-0.8.9/fastervit/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.8/fastervit/scheduler/scheduler_factory.py` & `fastervit-0.8.9/fastervit/scheduler/scheduler_factory.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.8/fastervit/scheduler/step_lr.py` & `fastervit-0.8.9/fastervit/scheduler/step_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.8/fastervit/scheduler/tanh_lr.py` & `fastervit-0.8.9/fastervit/scheduler/tanh_lr.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.8/fastervit/tensorboard.py` & `fastervit-0.8.9/fastervit/tensorboard.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.8/fastervit/train.py` & `fastervit-0.8.9/fastervit/train.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.8/fastervit/validate.py` & `fastervit-0.8.9/fastervit/validate.py`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.8/fastervit.egg-info/PKG-INFO` & `fastervit-0.8.9/fastervit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6661 7374  : 2.1.Name: fast
 00000020: 6572 7669 740a 5665 7273 696f 6e3a 2030  ervit.Version: 0
-00000030: 2e38 2e38 0a53 756d 6d61 7279 3a20 4661  .8.8.Summary: Fa
+00000030: 2e38 2e39 0a53 756d 6d61 7279 3a20 4661  .8.9.Summary: Fa
 00000040: 7374 6572 5669 543a 2046 6173 7420 5669  sterViT: Fast Vi
 00000050: 7369 6f6e 2054 7261 6e73 666f 726d 6572  sion Transformer
 00000060: 7320 7769 7468 2048 6965 7261 7263 6869  s with Hierarchi
 00000070: 6361 6c20 4174 7465 6e74 696f 6e0a 486f  cal Attention.Ho
 00000080: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 00000090: 2f67 6974 6875 622e 636f 6d2f 4e56 6c61  /github.com/NVla
 000000a0: 6273 2f46 6173 7465 7256 6954 0a41 7574  bs/FasterViT.Aut
@@ -108,480 +108,508 @@
 000006b0: 0a0a 2d2d 2d20 0a0a 4661 7374 6572 5669  ..--- ..FasterVi
 000006c0: 5420 6163 6869 6576 6573 2061 206e 6577  T achieves a new
 000006d0: 2053 4f54 4120 5061 7265 746f 2d66 726f   SOTA Pareto-fro
 000006e0: 6e74 2069 6e0a 7465 726d 7320 6f66 2061  nt in.terms of a
 000006f0: 6363 7572 6163 7920 7673 2e20 696d 6167  ccuracy vs. imag
 00000700: 6520 7468 726f 7567 6870 7574 2028 6e6f  e throughput (no
 00000710: 2065 7874 7261 2074 7261 696e 696e 6720   extra training 
-00000720: 6461 7461 2021 290a 0a21 5b74 6561 7365  data !)..![tease
-00000730: 725d 282e 2f66 6173 7465 7276 6974 2f61  r](./fastervit/a
-00000740: 7373 6574 732f 706c 6f74 2e70 6e67 290a  ssets/plot.png).
-00000750: 0a0a 0a23 2320 f09f 92a5 204e 6577 7320  ...## .... News 
-00000760: f09f 92a5 0a0a 2d20 2a2a 5b30 362e 3138  ......- **[06.18
-00000770: 2e32 3032 335d 2a2a 20f0 9f94 a520 5765  .2023]** .... We
-00000780: 2068 6176 6520 7265 6c65 6173 6564 2074   have released t
-00000790: 6865 2046 6173 7465 7256 6954 205b 7069  he FasterViT [pi
-000007a0: 7020 7061 636b 6167 655d 2868 7474 7073  p package](https
-000007b0: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-000007c0: 6563 742f 6661 7374 6572 7669 742f 2920  ect/fastervit/) 
-000007d0: 210a 2d20 2a2a 5b30 362e 3137 2e32 3032  !.- **[06.17.202
-000007e0: 335d 2a2a 20f0 9f94 a520 5b41 6e79 2d72  3]** .... [Any-r
-000007f0: 6573 6f6c 7574 696f 6e20 4661 7374 6572  esolution Faster
-00000800: 5669 545d 282e 2f66 6173 7465 7276 6974  ViT](./fastervit
-00000810: 2f6d 6f64 656c 732f 6661 7374 6572 5f76  /models/faster_v
-00000820: 6974 5f61 6e79 5f72 6573 2e70 7929 2020  it_any_res.py)  
-00000830: 6d6f 6465 6c20 6973 206e 6f77 2061 7661  model is now ava
-00000840: 696c 6162 6c65 2021 2074 6865 206d 6f64  ilable ! the mod
-00000850: 656c 2063 616e 2062 6520 7573 6564 2066  el can be used f
-00000860: 6f72 2076 6172 6965 7479 206f 6620 6170  or variety of ap
-00000870: 706c 6963 6174 696f 6e73 2073 7563 6820  plications such 
-00000880: 6173 2064 6574 6563 7469 6f6e 2061 6e64  as detection and
-00000890: 2073 6567 6d65 6e74 6174 696f 6e20 6f72   segmentation or
-000008a0: 2068 6967 682d 7265 736f 6c75 7469 6f6e   high-resolution
-000008b0: 2066 696e 652d 7475 6e69 6e67 2077 6974   fine-tuning wit
-000008c0: 6820 6172 6269 7472 6172 7920 696e 7075  h arbitrary inpu
-000008d0: 7420 696d 6167 6520 7265 736f 6c75 7469  t image resoluti
-000008e0: 6f6e 732e 200a 2d20 2a2a 5b30 362e 3039  ons. .- **[06.09
-000008f0: 2e32 3032 335d 2a2a 20f0 9f94 a5f0 9f94  .2023]** .......
-00000900: a520 5765 2068 6176 6520 7265 6c65 6173  . We have releas
-00000910: 6564 2073 6f75 7263 6520 636f 6465 2061  ed source code a
-00000920: 6e64 2049 6d61 6765 4e65 742d 314b 2046  nd ImageNet-1K F
-00000930: 6173 7465 7256 6954 2d6d 6f64 656c 7320  asterViT-models 
-00000940: 210a 0a23 2320 5175 6963 6b20 5374 6172  !..## Quick Star
-00000950: 740a 0a54 6865 2046 6173 7465 7256 6954  t..The FasterViT
-00000960: 2063 616e 2062 6520 636f 6e76 656e 6965   can be convenie
-00000970: 6e74 6c79 2069 6e73 7461 6c6c 6564 2062  ntly installed b
-00000980: 793a 0a0a 6060 6062 6173 680a 7069 7020  y:..```bash.pip 
-00000990: 696e 7374 616c 6c20 6661 7374 6572 7669  install fastervi
-000009a0: 740a 6060 600a 0a41 2046 6173 7465 7256  t.```..A FasterV
-000009b0: 6954 206d 6f64 656c 2077 6974 6820 6465  iT model with de
-000009c0: 6661 756c 7420 6879 7065 722d 7061 7261  fault hyper-para
-000009d0: 6d65 7465 7273 2063 616e 2062 6520 6372  meters can be cr
-000009e0: 6561 7465 6420 6173 2069 6e20 7468 6520  eated as in the 
-000009f0: 666f 6c6c 6f77 696e 673a 0a0a 6060 6070  following:..```p
-00000a00: 7974 686f 6e0a 3e3e 3e20 6672 6f6d 2066  ython.>>> from f
-00000a10: 6173 7465 7276 6974 2069 6d70 6f72 7420  astervit import 
-00000a20: 6372 6561 7465 5f6d 6f64 656c 0a0a 2320  create_model..# 
-00000a30: 4465 6669 6e65 2066 6173 7465 7276 6974  Define fastervit
-00000a40: 2d30 206d 6f64 656c 2077 6974 6820 3232  -0 model with 22
-00000a50: 3420 7820 3232 3420 7265 736f 6c75 7469  4 x 224 resoluti
-00000a60: 6f6e 0a3e 3e3e 206d 6f64 656c 203d 2063  on.>>> model = c
-00000a70: 7265 6174 655f 6d6f 6465 6c28 2766 6173  reate_model('fas
-00000a80: 7465 725f 7669 745f 305f 3232 3427 290a  ter_vit_0_224').
-00000a90: 6060 600a 0a57 6520 6361 6e20 616c 736f  ```..We can also
-00000aa0: 2075 7365 2074 6865 2061 6e79 2d72 6573   use the any-res
-00000ab0: 6f6c 7574 696f 6e20 4661 7374 6572 5669  olution FasterVi
-00000ac0: 5420 6d6f 6465 6c20 746f 2061 6363 6f6d  T model to accom
-00000ad0: 6d6f 6461 7465 2061 7262 6974 7261 7279  modate arbitrary
-00000ae0: 2069 6d61 6765 2072 6573 6f6c 7574 696f   image resolutio
-00000af0: 6e73 2e20 496e 2074 6865 2066 6f6c 6c6f  ns. In the follo
-00000b00: 7769 6e67 2c20 7765 2064 6566 696e 6520  wing, we define 
-00000b10: 616e 2061 6e79 2d72 6573 6f6c 7574 696f  an any-resolutio
-00000b20: 6e20 4661 7374 6572 5669 542d 310a 6d6f  n FasterViT-1.mo
-00000b30: 6465 6c20 7769 7468 2069 6e70 7574 2072  del with input r
-00000b40: 6573 6f6c 7574 696f 6e20 6f66 2035 3736  esolution of 576
-00000b50: 2078 2039 3630 2c20 7769 6e64 6f77 2073   x 960, window s
-00000b60: 697a 6573 206f 6620 3132 2061 6e64 2036  izes of 12 and 6
-00000b70: 2069 6e20 3372 6420 616e 6420 3474 6820   in 3rd and 4th 
-00000b80: 7374 6167 6573 2c20 6361 7272 6965 7220  stages, carrier 
-00000b90: 746f 6b65 6e20 7369 7a65 206f 6620 3220  token size of 2 
-00000ba0: 616e 6420 656d 6265 6464 696e 6720 6469  and embedding di
-00000bb0: 6d65 6e73 696f 6e20 6f66 0a31 3238 3a0a  mension of.128:.
-00000bc0: 0a60 6060 7079 7468 6f6e 0a3e 3e3e 2066  .```python.>>> f
-00000bd0: 726f 6d20 6661 7374 6572 7669 7420 696d  rom fastervit im
-00000be0: 706f 7274 2063 7265 6174 655f 6d6f 6465  port create_mode
-00000bf0: 6c0a 0a23 2044 6566 696e 6520 616e 792d  l..# Define any-
-00000c00: 7265 736f 6c75 7469 6f6e 2046 6173 7465  resolution Faste
-00000c10: 7256 6954 2d31 206d 6f64 656c 2077 6974  rViT-1 model wit
-00000c20: 6820 3537 3620 7820 3936 3020 7265 736f  h 576 x 960 reso
-00000c30: 6c75 7469 6f6e 0a3e 3e3e 206d 6f64 656c  lution.>>> model
-00000c40: 203d 2063 7265 6174 655f 6d6f 6465 6c28   = create_model(
-00000c50: 2766 6173 7465 725f 7669 745f 315f 616e  'faster_vit_1_an
-00000c60: 795f 7265 7327 2c20 0a20 2020 2020 2020  y_res', .       
-00000c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c80: 2020 2072 6573 6f6c 7574 696f 6e3d 5b35     resolution=[5
-00000c90: 3736 2c20 3936 305d 2c0a 2020 2020 2020  76, 960],.      
-00000ca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cb0: 2020 2020 7769 6e64 6f77 5f73 697a 653d      window_size=
-00000cc0: 5b37 2c20 372c 2031 322c 2036 5d2c 0a20  [7, 7, 12, 6],. 
-00000cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ce0: 2020 2020 2020 2020 2063 745f 7369 7a65           ct_size
-00000cf0: 3d32 2c0a 2020 2020 2020 2020 2020 2020  =2,.            
-00000d00: 2020 2020 2020 2020 2020 2020 2020 6469                di
-00000d10: 6d3d 3132 3829 0a60 6060 0a0a 2323 2043  m=128).```..## C
-00000d20: 6174 616c 6f67 0a2d 205b 785d 2049 6d61  atalog.- [x] Ima
-00000d30: 6765 4e65 742d 314b 2074 7261 696e 696e  geNet-1K trainin
-00000d40: 6720 636f 6465 0a2d 205b 785d 2049 6d61  g code.- [x] Ima
-00000d50: 6765 4e65 742d 314b 2070 7265 2d74 7261  geNet-1K pre-tra
-00000d60: 696e 6564 206d 6f64 656c 730a 2d20 5b78  ined models.- [x
-00000d70: 5d20 416e 792d 7265 736f 6c75 7469 6f6e  ] Any-resolution
-00000d80: 2046 6173 7465 7256 6954 0a2d 205b 785d   FasterViT.- [x]
-00000d90: 2046 6173 7465 7256 6954 2070 6970 2d70   FasterViT pip-p
-00000da0: 6163 6b61 6765 2072 656c 6561 7365 0a2d  ackage release.-
-00000db0: 205b 205d 2049 6d61 6765 4e65 742d 3231   [ ] ImageNet-21
-00000dc0: 4b20 7072 652d 7472 6169 6e65 6420 6d6f  K pre-trained mo
-00000dd0: 6465 6c73 0a2d 205b 205d 2049 6d61 6765  dels.- [ ] Image
-00000de0: 4e65 742d 3231 4b20 6669 6e65 2d74 756e  Net-21K fine-tun
-00000df0: 6520 7363 7269 7074 730a 2d20 5b20 5d20  e scripts.- [ ] 
-00000e00: 4465 7465 6374 696f 6e20 636f 6465 2028  Detection code (
-00000e10: 4449 4e4f 2920 2b20 6d6f 6465 6c73 0a2d  DINO) + models.-
-00000e20: 205b 205d 2053 6567 6d65 6e74 6174 696f   [ ] Segmentatio
-00000e30: 6e20 636f 6465 202b 206d 6f64 656c 730a  n code + models.
-00000e40: 0a2d 2d2d 200a 0a23 2320 5265 7375 6c74  .--- ..## Result
-00000e50: 7320 2b20 5072 6574 7261 696e 6564 204d  s + Pretrained M
-00000e60: 6f64 656c 730a 0a23 2323 2049 6d61 6765  odels..### Image
-00000e70: 4e65 742d 314b 0a2a 2a46 6173 7465 7256  Net-1K.**FasterV
-00000e80: 6954 2049 6d61 6765 4e65 742d 314b 2050  iT ImageNet-1K P
-00000e90: 7265 7472 6169 6e65 6420 4d6f 6465 6c73  retrained Models
-00000ea0: 2a2a 0a0a 3c74 6162 6c65 3e0a 2020 3c74  **..<table>.  <t
-00000eb0: 723e 0a20 2020 203c 7468 3e4e 616d 653c  r>.    <th>Name<
-00000ec0: 2f74 683e 0a20 2020 203c 7468 3e41 6363  /th>.    <th>Acc
-00000ed0: 4031 2825 293c 2f74 683e 0a20 2020 203c  @1(%)</th>.    <
-00000ee0: 7468 3e41 6363 4035 2825 293c 2f74 683e  th>Acc@5(%)</th>
-00000ef0: 0a20 2020 203c 7468 3e54 6872 6f75 6768  .    <th>Through
-00000f00: 7075 7428 496d 672f 5365 6329 3c2f 7468  put(Img/Sec)</th
-00000f10: 3e0a 2020 2020 3c74 683e 5265 736f 6c75  >.    <th>Resolu
-00000f20: 7469 6f6e 3c2f 7468 3e0a 2020 2020 3c74  tion</th>.    <t
-00000f30: 683e 2350 6172 616d 7328 4d29 3c2f 7468  h>#Params(M)</th
-00000f40: 3e0a 2020 2020 3c74 683e 464c 4f50 7328  >.    <th>FLOPs(
-00000f50: 4729 3c2f 7468 3e0a 2020 2020 3c74 683e  G)</th>.    <th>
-00000f60: 446f 776e 6c6f 6164 3c2f 7468 3e0a 2020  Download</th>.  
-00000f70: 3c2f 7472 3e0a 0a3c 7472 3e0a 2020 2020  </tr>..<tr>.    
-00000f80: 3c74 643e 4661 7374 6572 5669 542d 303c  <td>FasterViT-0<
-00000f90: 2f74 643e 0a20 2020 203c 7464 3e38 322e  /td>.    <td>82.
-00000fa0: 313c 2f74 643e 0a20 2020 203c 7464 3e39  1</td>.    <td>9
-00000fb0: 352e 393c 2f74 643e 0a20 2020 203c 7464  5.9</td>.    <td
-00000fc0: 3e35 3830 323c 2f74 643e 0a20 2020 203c  >5802</td>.    <
-00000fd0: 7464 3e32 3234 7832 3234 3c2f 7464 3e0a  td>224x224</td>.
-00000fe0: 2020 2020 3c74 643e 3331 2e34 3c2f 7464      <td>31.4</td
-00000ff0: 3e0a 2020 2020 3c74 643e 332e 333c 2f74  >.    <td>3.3</t
-00001000: 643e 0a20 2020 203c 7464 3e3c 6120 6872  d>.    <td><a hr
-00001010: 6566 3d22 6874 7470 733a 2f2f 6472 6976  ef="https://driv
-00001020: 652e 676f 6f67 6c65 2e63 6f6d 2f75 633f  e.google.com/uc?
-00001030: 6578 706f 7274 3d64 6f77 6e6c 6f61 6426  export=download&
-00001040: 6964 3d31 7477 4932 4c46 4a73 3339 3159  id=1twI2LFJs391Y
-00001050: 726a 384d 5234 5569 3950 6672 7657 716a  rj8MR4Ui9PfrvWqj
-00001060: 4531 6942 223e 6d6f 6465 6c3c 2f61 3e3c  E1iB">model</a><
-00001070: 2f74 643e 0a3c 2f74 723e 0a0a 3c74 723e  /td>.</tr>..<tr>
-00001080: 0a20 2020 203c 7464 3e46 6173 7465 7256  .    <td>FasterV
-00001090: 6954 2d31 3c2f 7464 3e0a 2020 2020 3c74  iT-1</td>.    <t
-000010a0: 643e 3833 2e32 3c2f 7464 3e0a 2020 2020  d>83.2</td>.    
-000010b0: 3c74 643e 3936 2e35 3c2f 7464 3e0a 2020  <td>96.5</td>.  
-000010c0: 2020 3c74 643e 3431 3838 3c2f 7464 3e0a    <td>4188</td>.
-000010d0: 2020 2020 3c74 643e 3232 3478 3232 343c      <td>224x224<
-000010e0: 2f74 643e 0a20 2020 203c 7464 3e35 332e  /td>.    <td>53.
-000010f0: 343c 2f74 643e 0a20 2020 203c 7464 3e35  4</td>.    <td>5
-00001100: 2e33 3c2f 7464 3e0a 2020 2020 3c74 643e  .3</td>.    <td>
-00001110: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00001120: 2f64 7269 7665 2e67 6f6f 676c 652e 636f  /drive.google.co
-00001130: 6d2f 7563 3f65 7870 6f72 743d 646f 776e  m/uc?export=down
-00001140: 6c6f 6164 2669 643d 3172 3757 3130 6e35  load&id=1r7W10n5
-00001150: 2d62 4674 4d33 737a 3462 6d61 4c72 6f77  -bFtM3sz4bmaLrow
-00001160: 4e32 6759 506b 4c47 5422 3e6d 6f64 656c  N2gYPkLGT">model
-00001170: 3c2f 613e 3c2f 7464 3e0a 3c2f 7472 3e0a  </a></td>.</tr>.
-00001180: 0a3c 7472 3e0a 2020 2020 3c74 643e 4661  .<tr>.    <td>Fa
-00001190: 7374 6572 5669 542d 323c 2f74 643e 0a20  sterViT-2</td>. 
-000011a0: 2020 203c 7464 3e38 342e 323c 2f74 643e     <td>84.2</td>
-000011b0: 0a20 2020 203c 7464 3e39 362e 383c 2f74  .    <td>96.8</t
-000011c0: 643e 0a20 2020 203c 7464 3e33 3136 313c  d>.    <td>3161<
-000011d0: 2f74 643e 0a20 2020 203c 7464 3e32 3234  /td>.    <td>224
-000011e0: 7832 3234 3c2f 7464 3e0a 2020 2020 3c74  x224</td>.    <t
-000011f0: 643e 3735 2e39 3c2f 7464 3e0a 2020 2020  d>75.9</td>.    
-00001200: 3c74 643e 382e 373c 2f74 643e 0a20 2020  <td>8.7</td>.   
-00001210: 203c 7464 3e3c 6120 6872 6566 3d22 6874   <td><a href="ht
-00001220: 7470 733a 2f2f 6472 6976 652e 676f 6f67  tps://drive.goog
-00001230: 6c65 2e63 6f6d 2f75 633f 6578 706f 7274  le.com/uc?export
-00001240: 3d64 6f77 6e6c 6f61 6426 6964 3d31 6e5f  =download&id=1n_
-00001250: 6136 7330 7067 6930 6a56 5a4f 476d 4465  a6s0pgi0jVZOGmDe
-00001260: 6932 7658 4855 3545 3652 4835 7755 223e  i2vXHU5E6RH5wU">
-00001270: 6d6f 6465 6c3c 2f61 3e3c 2f74 643e 0a3c  model</a></td>.<
-00001280: 2f74 723e 0a0a 3c74 723e 0a20 2020 203c  /tr>..<tr>.    <
-00001290: 7464 3e46 6173 7465 7256 6954 2d33 3c2f  td>FasterViT-3</
-000012a0: 7464 3e0a 2020 2020 3c74 643e 3834 2e39  td>.    <td>84.9
-000012b0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3937  </td>.    <td>97
-000012c0: 2e32 3c2f 7464 3e0a 2020 2020 3c74 643e  .2</td>.    <td>
-000012d0: 3137 3830 3c2f 7464 3e0a 2020 2020 3c74  1780</td>.    <t
-000012e0: 643e 3232 3478 3232 343c 2f74 643e 0a20  d>224x224</td>. 
-000012f0: 2020 203c 7464 3e31 3539 2e35 3c2f 7464     <td>159.5</td
-00001300: 3e0a 2020 2020 3c74 643e 3138 2e32 3c2f  >.    <td>18.2</
-00001310: 7464 3e0a 2020 2020 3c74 643e 3c61 2068  td>.    <td><a h
-00001320: 7265 663d 2268 7474 7073 3a2f 2f64 7269  ref="https://dri
-00001330: 7665 2e67 6f6f 676c 652e 636f 6d2f 7563  ve.google.com/uc
-00001340: 3f65 7870 6f72 743d 646f 776e 6c6f 6164  ?export=download
-00001350: 2669 643d 3174 7657 456c 5a39 3153 6961  &id=1tvWElZ91Sia
-00001360: 3253 7358 5958 464d 4e59 5177 6669 7043  2SsXYXFMNYQwfipC
-00001370: 7874 4937 5822 3e6d 6f64 656c 3c2f 613e  xtI7X">model</a>
-00001380: 3c2f 7464 3e0a 3c2f 7472 3e0a 0a3c 7472  </td>.</tr>..<tr
-00001390: 3e0a 2020 2020 3c74 643e 4661 7374 6572  >.    <td>Faster
-000013a0: 5669 542d 343c 2f74 643e 0a20 2020 203c  ViT-4</td>.    <
-000013b0: 7464 3e38 352e 343c 2f74 643e 0a20 2020  td>85.4</td>.   
-000013c0: 203c 7464 3e39 372e 333c 2f74 643e 0a20   <td>97.3</td>. 
-000013d0: 2020 203c 7464 3e38 3439 3c2f 7464 3e0a     <td>849</td>.
-000013e0: 2020 2020 3c74 643e 3232 3478 3232 343c      <td>224x224<
-000013f0: 2f74 643e 0a20 2020 203c 7464 3e34 3234  /td>.    <td>424
-00001400: 2e36 3c2f 7464 3e0a 2020 2020 3c74 643e  .6</td>.    <td>
-00001410: 3336 2e36 3c2f 7464 3e0a 2020 2020 3c74  36.6</td>.    <t
-00001420: 643e 3c61 2068 7265 663d 2268 7474 7073  d><a href="https
-00001430: 3a2f 2f64 7269 7665 2e67 6f6f 676c 652e  ://drive.google.
-00001440: 636f 6d2f 7563 3f65 7870 6f72 743d 646f  com/uc?export=do
-00001450: 776e 6c6f 6164 2669 643d 3167 5968 5841  wnload&id=1gYhXA
-00001460: 3332 512d 5f39 4335 4458 656c 3137 6176  32Q-_9C5DXel17av
-00001470: 565f 5a4c 6f61 4877 6467 7a22 3e6d 6f64  V_ZLoaHwdgz">mod
-00001480: 656c 3c2f 613e 3c2f 7464 3e0a 3c2f 7472  el</a></td>.</tr
-00001490: 3e0a 0a3c 7472 3e0a 2020 2020 3c74 643e  >..<tr>.    <td>
-000014a0: 4661 7374 6572 5669 542d 353c 2f74 643e  FasterViT-5</td>
-000014b0: 0a20 2020 203c 7464 3e38 352e 363c 2f74  .    <td>85.6</t
-000014c0: 643e 0a20 2020 203c 7464 3e39 372e 343c  d>.    <td>97.4<
-000014d0: 2f74 643e 0a20 2020 203c 7464 3e34 3439  /td>.    <td>449
-000014e0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3232  </td>.    <td>22
-000014f0: 3478 3232 343c 2f74 643e 0a20 2020 203c  4x224</td>.    <
-00001500: 7464 3e39 3735 2e35 3c2f 7464 3e0a 2020  td>975.5</td>.  
-00001510: 2020 3c74 643e 3131 332e 303c 2f74 643e    <td>113.0</td>
-00001520: 0a20 2020 203c 7464 3e3c 6120 6872 6566  .    <td><a href
-00001530: 3d22 6874 7470 733a 2f2f 6472 6976 652e  ="https://drive.
-00001540: 676f 6f67 6c65 2e63 6f6d 2f75 633f 6578  google.com/uc?ex
-00001550: 706f 7274 3d64 6f77 6e6c 6f61 6426 6964  port=download&id
-00001560: 3d31 6d71 7061 6937 5869 484c 725f 6e31  =1mqpai7XiHLr_n1
-00001570: 746a 786a 7a54 3871 3336 3978 5443 715f  tjxjzT8q369xTCq_
-00001580: 7a2d 223e 6d6f 6465 6c3c 2f61 3e3c 2f74  z-">model</a></t
-00001590: 643e 0a3c 2f74 723e 0a0a 3c74 723e 0a20  d>.</tr>..<tr>. 
-000015a0: 2020 203c 7464 3e46 6173 7465 7256 6954     <td>FasterViT
-000015b0: 2d36 3c2f 7464 3e0a 2020 2020 3c74 643e  -6</td>.    <td>
-000015c0: 3835 2e38 3c2f 7464 3e0a 2020 2020 3c74  85.8</td>.    <t
-000015d0: 643e 3937 2e34 3c2f 7464 3e0a 2020 2020  d>97.4</td>.    
-000015e0: 3c74 643e 3335 323c 2f74 643e 0a20 2020  <td>352</td>.   
-000015f0: 203c 7464 3e32 3234 7832 3234 3c2f 7464   <td>224x224</td
-00001600: 3e0a 2020 2020 3c74 643e 3133 3630 2e30  >.    <td>1360.0
-00001610: 3c2f 7464 3e0a 2020 2020 3c74 643e 3134  </td>.    <td>14
-00001620: 322e 303c 2f74 643e 0a20 2020 203c 7464  2.0</td>.    <td
-00001630: 3e3c 6120 6872 6566 3d22 6874 7470 733a  ><a href="https:
-00001640: 2f2f 6472 6976 652e 676f 6f67 6c65 2e63  //drive.google.c
-00001650: 6f6d 2f75 633f 6578 706f 7274 3d64 6f77  om/uc?export=dow
-00001660: 6e6c 6f61 6426 6964 3d31 326a 7461 7652  nload&id=12jtavR
-00001670: 3251 786d 4d7a 634b 7750 7a57 6537 6b77  2QxmMzcKwPzWe7kw
-00001680: 2d6f 7933 3449 5969 3539 223e 6d6f 6465  -oy34IYi59">mode
-00001690: 6c3c 2f61 3e3c 2f74 643e 0a3c 2f74 723e  l</a></td>.</tr>
-000016a0: 0a0a 3c2f 7461 626c 653e 0a0a 0a23 2323  ..</table>...###
-000016b0: 2052 6f62 7573 746e 6573 7320 2849 6d61   Robustness (Ima
-000016c0: 6765 4e65 742d 4120 2d20 496d 6167 654e  geNet-A - ImageN
-000016d0: 6574 2d52 202d 2049 6d61 6765 4e65 742d  et-R - ImageNet-
-000016e0: 5632 290a 0a41 6c6c 206d 6f64 656c 7320  V2)..All models 
-000016f0: 7573 6520 6063 726f 705f 7063 743d 302e  use `crop_pct=0.
-00001700: 3837 3560 2e20 5265 7375 6c74 7320 6172  875`. Results ar
-00001710: 6520 6f62 7461 696e 6564 2062 7920 7275  e obtained by ru
-00001720: 6e6e 696e 6720 696e 6665 7265 6e63 6520  nning inference 
-00001730: 6f6e 2049 6d61 6765 4e65 742d 314b 2070  on ImageNet-1K p
-00001740: 7265 7472 6169 6e65 6420 6d6f 6465 6c73  retrained models
-00001750: 2077 6974 686f 7574 2066 696e 6574 756e   without finetun
-00001760: 696e 672e 0a3c 7461 626c 653e 0a20 203c  ing..<table>.  <
-00001770: 7472 3e0a 2020 2020 3c74 683e 4e61 6d65  tr>.    <th>Name
-00001780: 3c2f 7468 3e0a 2020 2020 3c74 683e 412d  </th>.    <th>A-
-00001790: 4163 6340 3128 2529 3c2f 7468 3e0a 2020  Acc@1(%)</th>.  
-000017a0: 2020 3c74 683e 412d 4163 6340 3528 2529    <th>A-Acc@5(%)
-000017b0: 3c2f 7468 3e0a 2020 2020 3c74 683e 522d  </th>.    <th>R-
-000017c0: 4163 6340 3128 2529 3c2f 7468 3e0a 2020  Acc@1(%)</th>.  
-000017d0: 2020 3c74 683e 522d 4163 6340 3528 2529    <th>R-Acc@5(%)
-000017e0: 3c2f 7468 3e0a 2020 2020 3c74 683e 5632  </th>.    <th>V2
-000017f0: 2d41 6363 4031 2825 293c 2f74 683e 0a20  -Acc@1(%)</th>. 
-00001800: 2020 203c 7468 3e56 322d 4163 6340 3528     <th>V2-Acc@5(
-00001810: 2529 3c2f 7468 3e0a 2020 3c2f 7472 3e0a  %)</th>.  </tr>.
-00001820: 0a3c 7472 3e0a 2020 2020 3c74 643e 4661  .<tr>.    <td>Fa
-00001830: 7374 6572 5669 542d 303c 2f74 643e 0a20  sterViT-0</td>. 
-00001840: 2020 203c 7464 3e32 332e 393c 2f74 643e     <td>23.9</td>
-00001850: 0a20 2020 203c 7464 3e35 372e 363c 2f74  .    <td>57.6</t
-00001860: 643e 0a20 2020 203c 7464 3e34 352e 393c  d>.    <td>45.9<
-00001870: 2f74 643e 0a20 2020 203c 7464 3e36 302e  /td>.    <td>60.
-00001880: 343c 2f74 643e 0a20 2020 203c 7464 3e37  4</td>.    <td>7
-00001890: 302e 393c 2f74 643e 0a20 2020 203c 7464  0.9</td>.    <td
-000018a0: 3e39 302e 303c 2f74 643e 0a3c 2f74 723e  >90.0</td>.</tr>
-000018b0: 0a0a 3c74 723e 0a20 2020 203c 7464 3e46  ..<tr>.    <td>F
-000018c0: 6173 7465 7256 6954 2d31 3c2f 7464 3e0a  asterViT-1</td>.
-000018d0: 2020 2020 3c74 643e 3331 2e32 3c2f 7464      <td>31.2</td
-000018e0: 3e0a 2020 2020 3c74 643e 3633 2e33 3c2f  >.    <td>63.3</
-000018f0: 7464 3e0a 2020 2020 3c74 643e 3437 2e35  td>.    <td>47.5
-00001900: 3c2f 7464 3e0a 2020 2020 3c74 643e 3631  </td>.    <td>61
-00001910: 2e39 3c2f 7464 3e0a 2020 2020 3c74 643e  .9</td>.    <td>
-00001920: 3732 2e36 3c2f 7464 3e0a 2020 2020 3c74  72.6</td>.    <t
-00001930: 643e 3931 2e30 3c2f 7464 3e0a 3c2f 7472  d>91.0</td>.</tr
-00001940: 3e0a 0a3c 7472 3e0a 2020 2020 3c74 643e  >..<tr>.    <td>
-00001950: 4661 7374 6572 5669 542d 323c 2f74 643e  FasterViT-2</td>
-00001960: 0a20 2020 203c 7464 3e33 382e 323c 2f74  .    <td>38.2</t
-00001970: 643e 0a20 2020 203c 7464 3e36 382e 393c  d>.    <td>68.9<
-00001980: 2f74 643e 0a20 2020 203c 7464 3e34 392e  /td>.    <td>49.
-00001990: 363c 2f74 643e 0a20 2020 203c 7464 3e36  6</td>.    <td>6
-000019a0: 332e 343c 2f74 643e 0a20 2020 203c 7464  3.4</td>.    <td
-000019b0: 3e37 332e 373c 2f74 643e 0a20 2020 203c  >73.7</td>.    <
-000019c0: 7464 3e39 312e 363c 2f74 643e 0a3c 2f74  td>91.6</td>.</t
-000019d0: 723e 0a0a 3c74 723e 0a20 2020 203c 7464  r>..<tr>.    <td
-000019e0: 3e46 6173 7465 7256 6954 2d33 3c2f 7464  >FasterViT-3</td
-000019f0: 3e0a 2020 2020 3c74 643e 3434 2e32 3c2f  >.    <td>44.2</
-00001a00: 7464 3e0a 2020 2020 3c74 643e 3733 2e30  td>.    <td>73.0
-00001a10: 3c2f 7464 3e0a 2020 2020 3c74 643e 3531  </td>.    <td>51
-00001a20: 2e39 3c2f 7464 3e0a 2020 2020 3c74 643e  .9</td>.    <td>
-00001a30: 3635 2e36 3c2f 7464 3e0a 2020 2020 3c74  65.6</td>.    <t
-00001a40: 643e 3735 2e30 3c2f 7464 3e0a 2020 2020  d>75.0</td>.    
-00001a50: 3c74 643e 3932 2e32 3c2f 7464 3e0a 3c2f  <td>92.2</td>.</
-00001a60: 7472 3e0a 0a3c 7472 3e0a 2020 2020 3c74  tr>..<tr>.    <t
-00001a70: 643e 4661 7374 6572 5669 542d 343c 2f74  d>FasterViT-4</t
-00001a80: 643e 0a20 2020 203c 7464 3e34 392e 303c  d>.    <td>49.0<
-00001a90: 2f74 643e 0a20 2020 203c 7464 3e37 352e  /td>.    <td>75.
-00001aa0: 343c 2f74 643e 0a20 2020 203c 7464 3e35  4</td>.    <td>5
-00001ab0: 362e 303c 2f74 643e 0a20 2020 203c 7464  6.0</td>.    <td
-00001ac0: 3e36 392e 363c 2f74 643e 0a20 2020 203c  >69.6</td>.    <
-00001ad0: 7464 3e37 352e 373c 2f74 643e 0a20 2020  td>75.7</td>.   
-00001ae0: 203c 7464 3e39 322e 373c 2f74 643e 0a3c   <td>92.7</td>.<
-00001af0: 2f74 723e 0a0a 3c74 723e 0a20 2020 203c  /tr>..<tr>.    <
-00001b00: 7464 3e46 6173 7465 7256 6954 2d35 3c2f  td>FasterViT-5</
-00001b10: 7464 3e0a 2020 2020 3c74 643e 3532 2e37  td>.    <td>52.7
-00001b20: 3c2f 7464 3e0a 2020 2020 3c74 643e 3737  </td>.    <td>77
-00001b30: 2e36 3c2f 7464 3e0a 2020 2020 3c74 643e  .6</td>.    <td>
-00001b40: 3536 2e39 3c2f 7464 3e0a 2020 2020 3c74  56.9</td>.    <t
-00001b50: 643e 3730 2e30 3c2f 7464 3e0a 2020 2020  d>70.0</td>.    
-00001b60: 3c74 643e 3736 2e30 3c2f 7464 3e0a 2020  <td>76.0</td>.  
-00001b70: 2020 3c74 643e 3933 2e30 3c2f 7464 3e0a    <td>93.0</td>.
-00001b80: 3c2f 7472 3e0a 0a3c 7472 3e0a 2020 2020  </tr>..<tr>.    
-00001b90: 3c74 643e 4661 7374 6572 5669 542d 363c  <td>FasterViT-6<
-00001ba0: 2f74 643e 0a20 2020 203c 7464 3e35 332e  /td>.    <td>53.
-00001bb0: 373c 2f74 643e 0a20 2020 203c 7464 3e37  7</td>.    <td>7
-00001bc0: 382e 343c 2f74 643e 0a20 2020 203c 7464  8.4</td>.    <td
-00001bd0: 3e35 372e 313c 2f74 643e 0a20 2020 203c  >57.1</td>.    <
-00001be0: 7464 3e37 302e 313c 2f74 643e 0a20 2020  td>70.1</td>.   
-00001bf0: 203c 7464 3e37 362e 313c 2f74 643e 0a20   <td>76.1</td>. 
-00001c00: 2020 203c 7464 3e39 332e 303c 2f74 643e     <td>93.0</td>
-00001c10: 0a3c 2f74 723e 0a0a 3c2f 7461 626c 653e  .</tr>..</table>
-00001c20: 0a0a 412c 2052 2061 6e64 2056 3220 6465  ..A, R and V2 de
-00001c30: 6e6f 7465 2049 6d61 6765 4e65 742d 412c  note ImageNet-A,
-00001c40: 2049 6d61 6765 4e65 742d 5220 616e 6420   ImageNet-R and 
-00001c50: 496d 6167 654e 6574 2d56 3220 7265 7370  ImageNet-V2 resp
-00001c60: 6563 7469 7665 6c79 2e20 0a23 2320 5472  ectively. .## Tr
-00001c70: 6169 6e69 6e67 0a0a 506c 6561 7365 2073  aining..Please s
-00001c80: 6565 205b 5452 4149 4e49 4e47 2e6d 645d  ee [TRAINING.md]
-00001c90: 2854 5241 494e 494e 472e 6d64 2920 666f  (TRAINING.md) fo
-00001ca0: 7220 6465 7461 696c 6564 2074 7261 696e  r detailed train
-00001cb0: 696e 6720 696e 7374 7275 6374 696f 6e73  ing instructions
-00001cc0: 206f 6620 616c 6c20 6d6f 6465 6c73 2e20   of all models. 
-00001cd0: 0a0a 2323 2045 7661 6c75 6174 696f 6e0a  ..## Evaluation.
-00001ce0: 0a54 6865 2046 6173 7465 7256 6954 206d  .The FasterViT m
-00001cf0: 6f64 656c 7320 6361 6e20 6265 2065 7661  odels can be eva
-00001d00: 6c75 6174 6564 206f 6e20 496d 6167 654e  luated on ImageN
-00001d10: 6574 2d31 4b20 7661 6c69 6461 7469 6f6e  et-1K validation
-00001d20: 2073 6574 2075 7369 6e67 2074 6865 2066   set using the f
-00001d30: 6f6c 6c6f 7769 6e67 3a20 0a0a 6060 600a  ollowing: ..```.
-00001d40: 7079 7468 6f6e 2076 616c 6964 6174 652e  python validate.
-00001d50: 7079 205c 0a2d 2d6d 6f64 656c 203c 6d6f  py \.--model <mo
-00001d60: 6465 6c2d 6e61 6d65 3e0a 2d2d 6368 6563  del-name>.--chec
-00001d70: 6b70 6f69 6e74 203c 6368 6563 6b70 6f69  kpoint <checkpoi
-00001d80: 6e74 2d70 6174 683e 0a2d 2d64 6174 615f  nt-path>.--data_
-00001d90: 6469 7220 3c69 6d61 6765 6e65 742d 7061  dir <imagenet-pa
-00001da0: 7468 3e0a 2d2d 6261 7463 682d 7369 7a65  th>.--batch-size
-00001db0: 203c 6261 7463 682d 7369 7a65 2d70 6572   <batch-size-per
-00001dc0: 2d67 7075 0a60 6060 200a 0a48 6572 6520  -gpu.``` ..Here 
-00001dd0: 602d 2d6d 6f64 656c 6020 6973 2074 6865  `--model` is the
-00001de0: 2046 6173 7465 7256 6954 2076 6172 6961   FasterViT varia
-00001df0: 6e74 2028 652e 672e 2060 6661 7374 6572  nt (e.g. `faster
-00001e00: 5f76 6974 5f30 5f32 3234 5f31 6b60 292c  _vit_0_224_1k`),
-00001e10: 2060 2d2d 6368 6563 6b70 6f69 6e74 6020   `--checkpoint` 
-00001e20: 6973 2074 6865 2070 6174 6820 746f 2070  is the path to p
-00001e30: 7265 7472 6169 6e65 6420 6d6f 6465 6c20  retrained model 
-00001e40: 7765 6967 6874 732c 2060 2d2d 6461 7461  weights, `--data
-00001e50: 5f64 6972 6020 6973 2074 6865 2070 6174  _dir` is the pat
-00001e60: 6820 746f 2049 6d61 6765 4e65 742d 314b  h to ImageNet-1K
-00001e70: 2076 616c 6964 6174 696f 6e20 7365 7420   validation set 
-00001e80: 616e 6420 602d 2d62 6174 6368 2d73 697a  and `--batch-siz
-00001e90: 6560 2069 7320 7468 6520 6e75 6d62 6572  e` is the number
-00001ea0: 206f 6620 6261 7463 6820 7369 7a65 2e20   of batch size. 
-00001eb0: 5765 2061 6c73 6f20 7072 6f76 6964 6520  We also provide 
-00001ec0: 6120 7361 6d70 6c65 2073 6372 6970 7420  a sample script 
-00001ed0: 5b68 6572 655d 282e 2f66 6173 7465 7276  [here](./fasterv
-00001ee0: 6974 2f76 616c 6964 6174 652e 7368 292e  it/validate.sh).
-00001ef0: 200a 0a0a 2323 2049 6e73 7461 6c6c 6174   ...## Installat
-00001f00: 696f 6e0a 0a54 6865 2064 6570 656e 6465  ion..The depende
-00001f10: 6e63 6965 7320 6361 6e20 6265 2069 6e73  ncies can be ins
-00001f20: 7461 6c6c 6564 2062 7920 7275 6e6e 696e  talled by runnin
-00001f30: 673a 0a0a 6060 6062 6173 680a 7069 7020  g:..```bash.pip 
-00001f40: 696e 7374 616c 6c20 2d72 2072 6571 7569  install -r requi
-00001f50: 7265 6d65 6e74 732e 7478 740a 6060 600a  rements.txt.```.
-00001f60: 0a23 2320 5468 6972 642d 7061 7274 7920  .## Third-party 
-00001f70: 4578 7465 6e74 696f 6e73 0a57 6520 616c  Extentions.We al
-00001f80: 7761 7973 2077 656c 636f 6d65 2074 6869  ways welcome thi
-00001f90: 7264 2d70 6172 7479 2065 7874 656e 7469  rd-party extenti
-00001fa0: 6f6e 732f 696d 706c 656d 656e 7461 7469  ons/implementati
-00001fb0: 6f6e 7320 616e 6420 7573 6167 6520 666f  ons and usage fo
-00001fc0: 7220 6f74 6865 7220 7075 7270 6f73 6573  r other purposes
-00001fd0: 2e20 4966 2079 6f75 2077 6f75 6c64 206c  . If you would l
-00001fe0: 696b 6520 796f 7572 2077 6f72 6b20 746f  ike your work to
-00001ff0: 2062 6520 6c69 7374 6564 2069 6e20 7468   be listed in th
-00002000: 6973 2072 6570 6f73 6974 6f72 792c 2070  is repository, p
-00002010: 6c65 6173 6520 7261 6973 6520 616e 6420  lease raise and 
-00002020: 6973 7375 6520 616e 6420 7072 6f76 6964  issue and provid
-00002030: 6520 7573 2077 6974 6820 6465 7461 696c  e us with detail
-00002040: 6564 2069 6e66 6f72 6d61 7469 6f6e 2e20  ed information. 
-00002050: 200a 0a0a 2323 2041 636b 6e6f 776c 6564   ...## Acknowled
-00002060: 6765 6d65 6e74 0a54 6869 7320 7265 706f  gement.This repo
-00002070: 7369 746f 7279 2069 7320 6275 696c 7420  sitory is built 
-00002080: 6f6e 2074 6f70 206f 6620 7468 6520 5b74  on top of the [t
-00002090: 696d 6d5d 2868 7474 7073 3a2f 2f67 6974  imm](https://git
-000020a0: 6875 622e 636f 6d2f 6875 6767 696e 6766  hub.com/huggingf
-000020b0: 6163 652f 7079 746f 7263 682d 696d 6167  ace/pytorch-imag
-000020c0: 652d 6d6f 6465 6c73 2920 7265 706f 7369  e-models) reposi
-000020d0: 746f 7279 2e20 5765 2074 6861 6e6b 205b  tory. We thank [
-000020e0: 526f 7373 2057 7269 6768 746d 616e 5d28  Ross Wrightman](
-000020f0: 6874 7470 733a 2f2f 7277 6967 6874 6d61  https://rwightma
-00002100: 6e2e 636f 6d2f 2920 666f 7220 6372 6561  n.com/) for crea
-00002110: 7469 6e67 2061 6e64 206d 6169 6e74 6169  ting and maintai
-00002120: 6e69 6e67 2074 6869 7320 6869 6768 2d71  ning this high-q
-00002130: 7561 6c69 7479 206c 6962 7261 7279 2e20  uality library. 
-00002140: 200a 0a23 2320 4369 7461 7469 6f6e 0a0a   ..## Citation..
-00002150: 506c 6561 7365 2063 6f6e 7369 6465 7220  Please consider 
-00002160: 6369 7469 6e67 2046 6173 7465 7256 6954  citing FasterViT
-00002170: 2069 6620 7468 6973 2072 6570 6f73 6974   if this reposit
-00002180: 6f72 7920 6973 2075 7365 6675 6c20 666f  ory is useful fo
-00002190: 7220 796f 7572 2077 6f72 6b3a 0a0a 6060  r your work:..``
-000021a0: 600a 4061 7274 6963 6c65 7b68 6174 616d  `.@article{hatam
-000021b0: 697a 6164 6568 3230 3233 6661 7374 6572  izadeh2023faster
-000021c0: 7669 742c 0a20 2074 6974 6c65 3d7b 4661  vit,.  title={Fa
-000021d0: 7374 6572 5669 543a 2046 6173 7420 5669  sterViT: Fast Vi
-000021e0: 7369 6f6e 2054 7261 6e73 666f 726d 6572  sion Transformer
-000021f0: 7320 7769 7468 2048 6965 7261 7263 6869  s with Hierarchi
-00002200: 6361 6c20 4174 7465 6e74 696f 6e7d 2c0a  cal Attention},.
-00002210: 2020 6175 7468 6f72 3d7b 4861 7461 6d69    author={Hatami
-00002220: 7a61 6465 682c 2041 6c69 2061 6e64 2048  zadeh, Ali and H
-00002230: 6569 6e72 6963 682c 2047 7265 6720 616e  einrich, Greg an
-00002240: 6420 5969 6e2c 2048 6f6e 6778 7520 616e  d Yin, Hongxu an
-00002250: 6420 5461 6f2c 2041 6e64 7265 7720 616e  d Tao, Andrew an
-00002260: 6420 416c 7661 7265 7a2c 204a 6f73 6520  d Alvarez, Jose 
-00002270: 4d20 616e 6420 4b61 7574 7a2c 204a 616e  M and Kautz, Jan
-00002280: 2061 6e64 204d 6f6c 6368 616e 6f76 2c20   and Molchanov, 
-00002290: 5061 766c 6f7d 2c0a 2020 6a6f 7572 6e61  Pavlo},.  journa
-000022a0: 6c3d 7b61 7258 6976 2070 7265 7072 696e  l={arXiv preprin
-000022b0: 7420 6172 5869 763a 3233 3036 2e30 3631  t arXiv:2306.061
-000022c0: 3839 7d2c 0a20 2079 6561 723d 7b32 3032  89},.  year={202
-000022d0: 337d 0a7d 0a60 6060 0a0a 2323 204c 6963  3}.}.```..## Lic
-000022e0: 656e 7365 730a 0a43 6f70 7972 6967 6874  enses..Copyright
-000022f0: 20c2 a920 3230 3233 2c20 4e56 4944 4941   .. 2023, NVIDIA
-00002300: 2043 6f72 706f 7261 7469 6f6e 2e20 416c   Corporation. Al
-00002310: 6c20 7269 6768 7473 2072 6573 6572 7665  l rights reserve
-00002320: 642e 0a0a 5468 6973 2077 6f72 6b20 6973  d...This work is
-00002330: 206d 6164 6520 6176 6169 6c61 626c 6520   made available 
-00002340: 756e 6465 7220 7468 6520 4e56 4944 4941  under the NVIDIA
-00002350: 2053 6f75 7263 6520 436f 6465 204c 6963   Source Code Lic
-00002360: 656e 7365 2d4e 432e 2043 6c69 636b 205b  ense-NC. Click [
-00002370: 6865 7265 5d28 4c49 4345 4e53 4529 2074  here](LICENSE) t
-00002380: 6f20 7669 6577 2061 2063 6f70 7920 6f66  o view a copy of
-00002390: 2074 6869 7320 6c69 6365 6e73 652e 0a0a   this license...
-000023a0: 466f 7220 6c69 6365 6e73 6520 696e 666f  For license info
-000023b0: 726d 6174 696f 6e20 7265 6761 7264 696e  rmation regardin
-000023c0: 6720 7468 6520 7469 6d6d 2072 6570 6f73  g the timm repos
-000023d0: 6974 6f72 792c 2070 6c65 6173 6520 7265  itory, please re
-000023e0: 6665 7220 746f 2069 7473 205b 7265 706f  fer to its [repo
-000023f0: 7369 746f 7279 5d28 6874 7470 733a 2f2f  sitory](https://
-00002400: 6769 7468 7562 2e63 6f6d 2f72 7769 6768  github.com/rwigh
-00002410: 746d 616e 2f70 7974 6f72 6368 2d69 6d61  tman/pytorch-ima
-00002420: 6765 2d6d 6f64 656c 7329 2e0a 0a46 6f72  ge-models)...For
-00002430: 206c 6963 656e 7365 2069 6e66 6f72 6d61   license informa
-00002440: 7469 6f6e 2072 6567 6172 6469 6e67 2074  tion regarding t
-00002450: 6865 2049 6d61 6765 4e65 7420 6461 7461  he ImageNet data
-00002460: 7365 742c 2070 6c65 6173 6520 7365 6520  set, please see 
-00002470: 7468 6520 5b49 6d61 6765 4e65 7420 6f66  the [ImageNet of
-00002480: 6669 6369 616c 2077 6562 7369 7465 5d28  ficial website](
-00002490: 6874 7470 733a 2f2f 7777 772e 696d 6167  https://www.imag
-000024a0: 652d 6e65 742e 6f72 672f 292e 200a       e-net.org/). .
+00000720: 6461 7461 2021 290a 0a3c 7020 616c 6967  data !)..<p alig
+00000730: 6e3d 2263 656e 7465 7222 3e0a 3c69 6d67  n="center">.<img
+00000740: 2073 7263 3d22 6874 7470 733a 2f2f 6769   src="https://gi
+00000750: 7468 7562 2e63 6f6d 2f4e 566c 6162 732f  thub.com/NVlabs/
+00000760: 4661 7374 6572 5669 542f 6173 7365 7473  FasterViT/assets
+00000770: 2f32 3638 3036 3339 342f 3235 3364 3161  /26806394/253d1a
+00000780: 3265 2d62 3566 352d 3461 3962 2d61 3336  2e-b5f5-4a9b-a36
+00000790: 322d 3663 6464 3136 6266 6363 6331 2220  2-6cdd16bfccc1" 
+000007a0: 7769 6474 683d 3632 2520 6865 6967 6874  width=62% height
+000007b0: 3d36 3225 200a 636c 6173 733d 2263 656e  =62% .class="cen
+000007c0: 7465 7222 3e0a 3c2f 703e 0a0a 0a3c 212d  ter">.</p>...<!-
+000007d0: 2d20 5765 2069 6e74 726f 6475 6365 2061  - We introduce a
+000007e0: 206e 6577 2073 656c 662d 6174 7465 6e74   new self-attent
+000007f0: 696f 6e20 6d65 6368 616e 6973 6d2c 2064  ion mechanism, d
+00000800: 656e 6f74 6564 2061 7320 4869 6572 6172  enoted as Hierar
+00000810: 6368 6963 616c 0a41 7474 656e 7469 6f6e  chical.Attention
+00000820: 2028 4841 5429 2c20 7468 6174 2063 6170   (HAT), that cap
+00000830: 7475 7265 7320 626f 7468 2073 686f 7274  tures both short
+00000840: 2061 6e64 206c 6f6e 672d 7261 6e67 6520   and long-range 
+00000850: 696e 666f 726d 6174 696f 6e20 6279 206c  information by l
+00000860: 6561 726e 696e 670a 6372 6f73 732d 7769  earning.cross-wi
+00000870: 6e64 6f77 2063 6172 7269 6572 2074 6f6b  ndow carrier tok
+00000880: 656e 732e 0a0a 215b 7465 6173 6572 5d28  ens...![teaser](
+00000890: 2e2f 6661 7374 6572 7669 742f 6173 7365  ./fastervit/asse
+000008a0: 7473 2f68 6965 7261 7263 6869 616c 5f61  ts/hierarchial_a
+000008b0: 7474 6e2e 706e 6729 202d 2d3e 0a0a 0a3c  ttn.png) -->...<
+000008c0: 212d 2d20 2323 20f0 9f92 a520 4e65 7773  !-- ## .... News
+000008d0: 20f0 9f92 a50a 0a2d 202a 2a5b 3036 2e31   ......- **[06.1
+000008e0: 382e 3230 3233 5d2a 2a20 f09f 94a5 2057  8.2023]** .... W
+000008f0: 6520 6861 7665 2072 656c 6561 7365 6420  e have released 
+00000900: 7468 6520 4661 7374 6572 5669 5420 5b70  the FasterViT [p
+00000910: 6970 2070 6163 6b61 6765 5d28 6874 7470  ip package](http
+00000920: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000930: 6a65 6374 2f66 6173 7465 7276 6974 2f29  ject/fastervit/)
+00000940: 2021 0a2d 202a 2a5b 3036 2e31 372e 3230   !.- **[06.17.20
+00000950: 3233 5d2a 2a20 f09f 94a5 205b 416e 792d  23]** .... [Any-
+00000960: 7265 736f 6c75 7469 6f6e 2046 6173 7465  resolution Faste
+00000970: 7256 6954 5d28 2e2f 6661 7374 6572 7669  rViT](./fastervi
+00000980: 742f 6d6f 6465 6c73 2f66 6173 7465 725f  t/models/faster_
+00000990: 7669 745f 616e 795f 7265 732e 7079 2920  vit_any_res.py) 
+000009a0: 206d 6f64 656c 2069 7320 6e6f 7720 6176   model is now av
+000009b0: 6169 6c61 626c 6520 2120 7468 6520 6d6f  ailable ! the mo
+000009c0: 6465 6c20 6361 6e20 6265 2075 7365 6420  del can be used 
+000009d0: 666f 7220 7661 7269 6574 7920 6f66 2061  for variety of a
+000009e0: 7070 6c69 6361 7469 6f6e 7320 7375 6368  pplications such
+000009f0: 2061 7320 6465 7465 6374 696f 6e20 616e   as detection an
+00000a00: 6420 7365 676d 656e 7461 7469 6f6e 206f  d segmentation o
+00000a10: 7220 6869 6768 2d72 6573 6f6c 7574 696f  r high-resolutio
+00000a20: 6e20 6669 6e65 2d74 756e 696e 6720 7769  n fine-tuning wi
+00000a30: 7468 2061 7262 6974 7261 7279 2069 6e70  th arbitrary inp
+00000a40: 7574 2069 6d61 6765 2072 6573 6f6c 7574  ut image resolut
+00000a50: 696f 6e73 2e20 0a2d 202a 2a5b 3036 2e30  ions. .- **[06.0
+00000a60: 392e 3230 3233 5d2a 2a20 f09f 94a5 f09f  9.2023]** ......
+00000a70: 94a5 2057 6520 6861 7665 2072 656c 6561  .. We have relea
+00000a80: 7365 6420 736f 7572 6365 2063 6f64 6520  sed source code 
+00000a90: 616e 6420 496d 6167 654e 6574 2d31 4b20  and ImageNet-1K 
+00000aa0: 4661 7374 6572 5669 542d 6d6f 6465 6c73  FasterViT-models
+00000ab0: 2021 202d 2d3e 0a0a 2323 2051 7569 636b   ! -->..## Quick
+00000ac0: 2053 7461 7274 0a0a 5468 6520 4661 7374   Start..The Fast
+00000ad0: 6572 5669 5420 6361 6e20 6265 2063 6f6e  erViT can be con
+00000ae0: 7665 6e69 656e 746c 7920 696e 7374 616c  veniently instal
+00000af0: 6c65 6420 6279 3a0a 0a60 6060 6261 7368  led by:..```bash
+00000b00: 0a70 6970 2069 6e73 7461 6c6c 2066 6173  .pip install fas
+00000b10: 7465 7276 6974 0a60 6060 0a0a 4120 4661  tervit.```..A Fa
+00000b20: 7374 6572 5669 5420 6d6f 6465 6c20 7769  sterViT model wi
+00000b30: 7468 2064 6566 6175 6c74 2068 7970 6572  th default hyper
+00000b40: 2d70 6172 616d 6574 6572 7320 6361 6e20  -parameters can 
+00000b50: 6265 2063 7265 6174 6564 2061 7320 696e  be created as in
+00000b60: 2074 6865 2066 6f6c 6c6f 7769 6e67 3a0a   the following:.
+00000b70: 0a60 6060 7079 7468 6f6e 0a3e 3e3e 2066  .```python.>>> f
+00000b80: 726f 6d20 6661 7374 6572 7669 7420 696d  rom fastervit im
+00000b90: 706f 7274 2063 7265 6174 655f 6d6f 6465  port create_mode
+00000ba0: 6c0a 0a23 2044 6566 696e 6520 6661 7374  l..# Define fast
+00000bb0: 6572 7669 742d 3020 6d6f 6465 6c20 7769  ervit-0 model wi
+00000bc0: 7468 2032 3234 2078 2032 3234 2072 6573  th 224 x 224 res
+00000bd0: 6f6c 7574 696f 6e0a 3e3e 3e20 6d6f 6465  olution.>>> mode
+00000be0: 6c20 3d20 6372 6561 7465 5f6d 6f64 656c  l = create_model
+00000bf0: 2827 6661 7374 6572 5f76 6974 5f30 5f32  ('faster_vit_0_2
+00000c00: 3234 2729 0a60 6060 0a0a 5765 2063 616e  24').```..We can
+00000c10: 2061 6c73 6f20 7573 6520 7468 6520 616e   also use the an
+00000c20: 792d 7265 736f 6c75 7469 6f6e 2046 6173  y-resolution Fas
+00000c30: 7465 7256 6954 206d 6f64 656c 2074 6f20  terViT model to 
+00000c40: 6163 636f 6d6d 6f64 6174 6520 6172 6269  accommodate arbi
+00000c50: 7472 6172 7920 696d 6167 6520 7265 736f  trary image reso
+00000c60: 6c75 7469 6f6e 732e 2049 6e20 7468 6520  lutions. In the 
+00000c70: 666f 6c6c 6f77 696e 672c 2077 6520 6465  following, we de
+00000c80: 6669 6e65 2061 6e20 616e 792d 7265 736f  fine an any-reso
+00000c90: 6c75 7469 6f6e 2046 6173 7465 7256 6954  lution FasterViT
+00000ca0: 2d31 0a6d 6f64 656c 2077 6974 6820 696e  -1.model with in
+00000cb0: 7075 7420 7265 736f 6c75 7469 6f6e 206f  put resolution o
+00000cc0: 6620 3537 3620 7820 3936 302c 2077 696e  f 576 x 960, win
+00000cd0: 646f 7720 7369 7a65 7320 6f66 2031 3220  dow sizes of 12 
+00000ce0: 616e 6420 3620 696e 2033 7264 2061 6e64  and 6 in 3rd and
+00000cf0: 2034 7468 2073 7461 6765 732c 2063 6172   4th stages, car
+00000d00: 7269 6572 2074 6f6b 656e 2073 697a 6520  rier token size 
+00000d10: 6f66 2032 2061 6e64 2065 6d62 6564 6469  of 2 and embeddi
+00000d20: 6e67 2064 696d 656e 7369 6f6e 206f 660a  ng dimension of.
+00000d30: 3132 383a 0a0a 6060 6070 7974 686f 6e0a  128:..```python.
+00000d40: 3e3e 3e20 6672 6f6d 2066 6173 7465 7276  >>> from fasterv
+00000d50: 6974 2069 6d70 6f72 7420 6372 6561 7465  it import create
+00000d60: 5f6d 6f64 656c 0a0a 2320 4465 6669 6e65  _model..# Define
+00000d70: 2061 6e79 2d72 6573 6f6c 7574 696f 6e20   any-resolution 
+00000d80: 4661 7374 6572 5669 542d 3120 6d6f 6465  FasterViT-1 mode
+00000d90: 6c20 7769 7468 2035 3736 2078 2039 3630  l with 576 x 960
+00000da0: 2072 6573 6f6c 7574 696f 6e0a 3e3e 3e20   resolution.>>> 
+00000db0: 6d6f 6465 6c20 3d20 6372 6561 7465 5f6d  model = create_m
+00000dc0: 6f64 656c 2827 6661 7374 6572 5f76 6974  odel('faster_vit
+00000dd0: 5f31 5f61 6e79 5f72 6573 272c 200a 2020  _1_any_res', .  
+00000de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000df0: 2020 2020 2020 2020 7265 736f 6c75 7469          resoluti
+00000e00: 6f6e 3d5b 3537 362c 2039 3630 5d2c 0a20  on=[576, 960],. 
+00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e20: 2020 2020 2020 2020 2077 696e 646f 775f           window_
+00000e30: 7369 7a65 3d5b 372c 2037 2c20 3132 2c20  size=[7, 7, 12, 
+00000e40: 365d 2c0a 2020 2020 2020 2020 2020 2020  6],.            
+00000e50: 2020 2020 2020 2020 2020 2020 2020 6374                ct
+00000e60: 5f73 697a 653d 322c 0a20 2020 2020 2020  _size=2,.       
+00000e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e80: 2020 2064 696d 3d31 3238 290a 6060 600a     dim=128).```.
+00000e90: 0a3c 212d 2d20 2323 2043 6174 616c 6f67  .<!-- ## Catalog
+00000ea0: 0a2d 205b 785d 2049 6d61 6765 4e65 742d  .- [x] ImageNet-
+00000eb0: 314b 2074 7261 696e 696e 6720 636f 6465  1K training code
+00000ec0: 0a2d 205b 785d 2049 6d61 6765 4e65 742d  .- [x] ImageNet-
+00000ed0: 314b 2070 7265 2d74 7261 696e 6564 206d  1K pre-trained m
+00000ee0: 6f64 656c 730a 2d20 5b78 5d20 416e 792d  odels.- [x] Any-
+00000ef0: 7265 736f 6c75 7469 6f6e 2046 6173 7465  resolution Faste
+00000f00: 7256 6954 0a2d 205b 785d 2046 6173 7465  rViT.- [x] Faste
+00000f10: 7256 6954 2070 6970 2d70 6163 6b61 6765  rViT pip-package
+00000f20: 2072 656c 6561 7365 0a2d 205b 205d 2055   release.- [ ] U
+00000f30: 7064 6174 6520 7472 6169 6e69 6e67 2073  pdate training s
+00000f40: 6372 6970 7473 2074 6f20 7375 7070 6f72  cripts to suppor
+00000f50: 7420 6d6f 6465 6c2e 636f 6d70 696c 652c  t model.compile,
+00000f60: 200a 2d20 5b20 5d20 496d 6167 654e 6574   .- [ ] ImageNet
+00000f70: 2d32 314b 2070 7265 2d74 7261 696e 6564  -21K pre-trained
+00000f80: 206d 6f64 656c 730a 2d20 5b20 5d20 496d   models.- [ ] Im
+00000f90: 6167 654e 6574 2d32 314b 2066 696e 652d  ageNet-21K fine-
+00000fa0: 7475 6e65 2073 6372 6970 7473 0a2d 205b  tune scripts.- [
+00000fb0: 205d 2044 6574 6563 7469 6f6e 2063 6f64   ] Detection cod
+00000fc0: 6520 2844 494e 4f29 202b 206d 6f64 656c  e (DINO) + model
+00000fd0: 730a 2d20 5b20 5d20 5365 676d 656e 7461  s.- [ ] Segmenta
+00000fe0: 7469 6f6e 2063 6f64 6520 2b20 6d6f 6465  tion code + mode
+00000ff0: 6c73 202d 2d3e 0a0a 2d2d 2d20 0a0a 2323  ls -->..--- ..##
+00001000: 2052 6573 756c 7473 202b 2050 7265 7472   Results + Pretr
+00001010: 6169 6e65 6420 4d6f 6465 6c73 0a0a 2323  ained Models..##
+00001020: 2320 496d 6167 654e 6574 2d31 4b0a 2a2a  # ImageNet-1K.**
+00001030: 4661 7374 6572 5669 5420 496d 6167 654e  FasterViT ImageN
+00001040: 6574 2d31 4b20 5072 6574 7261 696e 6564  et-1K Pretrained
+00001050: 204d 6f64 656c 732a 2a0a 0a3c 7461 626c   Models**..<tabl
+00001060: 653e 0a20 203c 7472 3e0a 2020 2020 3c74  e>.  <tr>.    <t
+00001070: 683e 4e61 6d65 3c2f 7468 3e0a 2020 2020  h>Name</th>.    
+00001080: 3c74 683e 4163 6340 3128 2529 3c2f 7468  <th>Acc@1(%)</th
+00001090: 3e0a 2020 2020 3c74 683e 4163 6340 3528  >.    <th>Acc@5(
+000010a0: 2529 3c2f 7468 3e0a 2020 2020 3c74 683e  %)</th>.    <th>
+000010b0: 5468 726f 7567 6870 7574 2849 6d67 2f53  Throughput(Img/S
+000010c0: 6563 293c 2f74 683e 0a20 2020 203c 7468  ec)</th>.    <th
+000010d0: 3e52 6573 6f6c 7574 696f 6e3c 2f74 683e  >Resolution</th>
+000010e0: 0a20 2020 203c 7468 3e23 5061 7261 6d73  .    <th>#Params
+000010f0: 284d 293c 2f74 683e 0a20 2020 203c 7468  (M)</th>.    <th
+00001100: 3e46 4c4f 5073 2847 293c 2f74 683e 0a20  >FLOPs(G)</th>. 
+00001110: 2020 203c 7468 3e44 6f77 6e6c 6f61 643c     <th>Download<
+00001120: 2f74 683e 0a20 203c 2f74 723e 0a0a 3c74  /th>.  </tr>..<t
+00001130: 723e 0a20 2020 203c 7464 3e46 6173 7465  r>.    <td>Faste
+00001140: 7256 6954 2d30 3c2f 7464 3e0a 2020 2020  rViT-0</td>.    
+00001150: 3c74 643e 3832 2e31 3c2f 7464 3e0a 2020  <td>82.1</td>.  
+00001160: 2020 3c74 643e 3935 2e39 3c2f 7464 3e0a    <td>95.9</td>.
+00001170: 2020 2020 3c74 643e 3538 3032 3c2f 7464      <td>5802</td
+00001180: 3e0a 2020 2020 3c74 643e 3232 3478 3232  >.    <td>224x22
+00001190: 343c 2f74 643e 0a20 2020 203c 7464 3e33  4</td>.    <td>3
+000011a0: 312e 343c 2f74 643e 0a20 2020 203c 7464  1.4</td>.    <td
+000011b0: 3e33 2e33 3c2f 7464 3e0a 2020 2020 3c74  >3.3</td>.    <t
+000011c0: 643e 3c61 2068 7265 663d 2268 7474 7073  d><a href="https
+000011d0: 3a2f 2f64 7269 7665 2e67 6f6f 676c 652e  ://drive.google.
+000011e0: 636f 6d2f 7563 3f65 7870 6f72 743d 646f  com/uc?export=do
+000011f0: 776e 6c6f 6164 2669 643d 3174 7749 324c  wnload&id=1twI2L
+00001200: 464a 7333 3931 5972 6a38 4d52 3455 6939  FJs391Yrj8MR4Ui9
+00001210: 5066 7276 5771 6a45 3169 4222 3e6d 6f64  PfrvWqjE1iB">mod
+00001220: 656c 3c2f 613e 3c2f 7464 3e0a 3c2f 7472  el</a></td>.</tr
+00001230: 3e0a 0a3c 7472 3e0a 2020 2020 3c74 643e  >..<tr>.    <td>
+00001240: 4661 7374 6572 5669 542d 313c 2f74 643e  FasterViT-1</td>
+00001250: 0a20 2020 203c 7464 3e38 332e 323c 2f74  .    <td>83.2</t
+00001260: 643e 0a20 2020 203c 7464 3e39 362e 353c  d>.    <td>96.5<
+00001270: 2f74 643e 0a20 2020 203c 7464 3e34 3138  /td>.    <td>418
+00001280: 383c 2f74 643e 0a20 2020 203c 7464 3e32  8</td>.    <td>2
+00001290: 3234 7832 3234 3c2f 7464 3e0a 2020 2020  24x224</td>.    
+000012a0: 3c74 643e 3533 2e34 3c2f 7464 3e0a 2020  <td>53.4</td>.  
+000012b0: 2020 3c74 643e 352e 333c 2f74 643e 0a20    <td>5.3</td>. 
+000012c0: 2020 203c 7464 3e3c 6120 6872 6566 3d22     <td><a href="
+000012d0: 6874 7470 733a 2f2f 6472 6976 652e 676f  https://drive.go
+000012e0: 6f67 6c65 2e63 6f6d 2f75 633f 6578 706f  ogle.com/uc?expo
+000012f0: 7274 3d64 6f77 6e6c 6f61 6426 6964 3d31  rt=download&id=1
+00001300: 7237 5731 306e 352d 6246 744d 3373 7a34  r7W10n5-bFtM3sz4
+00001310: 626d 614c 726f 774e 3267 5950 6b4c 4754  bmaLrowN2gYPkLGT
+00001320: 223e 6d6f 6465 6c3c 2f61 3e3c 2f74 643e  ">model</a></td>
+00001330: 0a3c 2f74 723e 0a0a 3c74 723e 0a20 2020  .</tr>..<tr>.   
+00001340: 203c 7464 3e46 6173 7465 7256 6954 2d32   <td>FasterViT-2
+00001350: 3c2f 7464 3e0a 2020 2020 3c74 643e 3834  </td>.    <td>84
+00001360: 2e32 3c2f 7464 3e0a 2020 2020 3c74 643e  .2</td>.    <td>
+00001370: 3936 2e38 3c2f 7464 3e0a 2020 2020 3c74  96.8</td>.    <t
+00001380: 643e 3331 3631 3c2f 7464 3e0a 2020 2020  d>3161</td>.    
+00001390: 3c74 643e 3232 3478 3232 343c 2f74 643e  <td>224x224</td>
+000013a0: 0a20 2020 203c 7464 3e37 352e 393c 2f74  .    <td>75.9</t
+000013b0: 643e 0a20 2020 203c 7464 3e38 2e37 3c2f  d>.    <td>8.7</
+000013c0: 7464 3e0a 2020 2020 3c74 643e 3c61 2068  td>.    <td><a h
+000013d0: 7265 663d 2268 7474 7073 3a2f 2f64 7269  ref="https://dri
+000013e0: 7665 2e67 6f6f 676c 652e 636f 6d2f 7563  ve.google.com/uc
+000013f0: 3f65 7870 6f72 743d 646f 776e 6c6f 6164  ?export=download
+00001400: 2669 643d 316e 5f61 3673 3070 6769 306a  &id=1n_a6s0pgi0j
+00001410: 565a 4f47 6d44 6569 3276 5848 5535 4536  VZOGmDei2vXHU5E6
+00001420: 5248 3577 5522 3e6d 6f64 656c 3c2f 613e  RH5wU">model</a>
+00001430: 3c2f 7464 3e0a 3c2f 7472 3e0a 0a3c 7472  </td>.</tr>..<tr
+00001440: 3e0a 2020 2020 3c74 643e 4661 7374 6572  >.    <td>Faster
+00001450: 5669 542d 333c 2f74 643e 0a20 2020 203c  ViT-3</td>.    <
+00001460: 7464 3e38 342e 393c 2f74 643e 0a20 2020  td>84.9</td>.   
+00001470: 203c 7464 3e39 372e 323c 2f74 643e 0a20   <td>97.2</td>. 
+00001480: 2020 203c 7464 3e31 3738 303c 2f74 643e     <td>1780</td>
+00001490: 0a20 2020 203c 7464 3e32 3234 7832 3234  .    <td>224x224
+000014a0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3135  </td>.    <td>15
+000014b0: 392e 353c 2f74 643e 0a20 2020 203c 7464  9.5</td>.    <td
+000014c0: 3e31 382e 323c 2f74 643e 0a20 2020 203c  >18.2</td>.    <
+000014d0: 7464 3e3c 6120 6872 6566 3d22 6874 7470  td><a href="http
+000014e0: 733a 2f2f 6472 6976 652e 676f 6f67 6c65  s://drive.google
+000014f0: 2e63 6f6d 2f75 633f 6578 706f 7274 3d64  .com/uc?export=d
+00001500: 6f77 6e6c 6f61 6426 6964 3d31 7476 5745  ownload&id=1tvWE
+00001510: 6c5a 3931 5369 6132 5373 5859 5846 4d4e  lZ91Sia2SsXYXFMN
+00001520: 5951 7766 6970 4378 7449 3758 223e 6d6f  YQwfipCxtI7X">mo
+00001530: 6465 6c3c 2f61 3e3c 2f74 643e 0a3c 2f74  del</a></td>.</t
+00001540: 723e 0a0a 3c74 723e 0a20 2020 203c 7464  r>..<tr>.    <td
+00001550: 3e46 6173 7465 7256 6954 2d34 3c2f 7464  >FasterViT-4</td
+00001560: 3e0a 2020 2020 3c74 643e 3835 2e34 3c2f  >.    <td>85.4</
+00001570: 7464 3e0a 2020 2020 3c74 643e 3937 2e33  td>.    <td>97.3
+00001580: 3c2f 7464 3e0a 2020 2020 3c74 643e 3834  </td>.    <td>84
+00001590: 393c 2f74 643e 0a20 2020 203c 7464 3e32  9</td>.    <td>2
+000015a0: 3234 7832 3234 3c2f 7464 3e0a 2020 2020  24x224</td>.    
+000015b0: 3c74 643e 3432 342e 363c 2f74 643e 0a20  <td>424.6</td>. 
+000015c0: 2020 203c 7464 3e33 362e 363c 2f74 643e     <td>36.6</td>
+000015d0: 0a20 2020 203c 7464 3e3c 6120 6872 6566  .    <td><a href
+000015e0: 3d22 6874 7470 733a 2f2f 6472 6976 652e  ="https://drive.
+000015f0: 676f 6f67 6c65 2e63 6f6d 2f75 633f 6578  google.com/uc?ex
+00001600: 706f 7274 3d64 6f77 6e6c 6f61 6426 6964  port=download&id
+00001610: 3d31 6759 6858 4133 3251 2d5f 3943 3544  =1gYhXA32Q-_9C5D
+00001620: 5865 6c31 3761 7656 5f5a 4c6f 6148 7764  Xel17avV_ZLoaHwd
+00001630: 677a 223e 6d6f 6465 6c3c 2f61 3e3c 2f74  gz">model</a></t
+00001640: 643e 0a3c 2f74 723e 0a0a 3c74 723e 0a20  d>.</tr>..<tr>. 
+00001650: 2020 203c 7464 3e46 6173 7465 7256 6954     <td>FasterViT
+00001660: 2d35 3c2f 7464 3e0a 2020 2020 3c74 643e  -5</td>.    <td>
+00001670: 3835 2e36 3c2f 7464 3e0a 2020 2020 3c74  85.6</td>.    <t
+00001680: 643e 3937 2e34 3c2f 7464 3e0a 2020 2020  d>97.4</td>.    
+00001690: 3c74 643e 3434 393c 2f74 643e 0a20 2020  <td>449</td>.   
+000016a0: 203c 7464 3e32 3234 7832 3234 3c2f 7464   <td>224x224</td
+000016b0: 3e0a 2020 2020 3c74 643e 3937 352e 353c  >.    <td>975.5<
+000016c0: 2f74 643e 0a20 2020 203c 7464 3e31 3133  /td>.    <td>113
+000016d0: 2e30 3c2f 7464 3e0a 2020 2020 3c74 643e  .0</td>.    <td>
+000016e0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000016f0: 2f64 7269 7665 2e67 6f6f 676c 652e 636f  /drive.google.co
+00001700: 6d2f 7563 3f65 7870 6f72 743d 646f 776e  m/uc?export=down
+00001710: 6c6f 6164 2669 643d 316d 7170 6169 3758  load&id=1mqpai7X
+00001720: 6948 4c72 5f6e 3174 6a78 6a7a 5438 7133  iHLr_n1tjxjzT8q3
+00001730: 3639 7854 4371 5f7a 2d22 3e6d 6f64 656c  69xTCq_z-">model
+00001740: 3c2f 613e 3c2f 7464 3e0a 3c2f 7472 3e0a  </a></td>.</tr>.
+00001750: 0a3c 7472 3e0a 2020 2020 3c74 643e 4661  .<tr>.    <td>Fa
+00001760: 7374 6572 5669 542d 363c 2f74 643e 0a20  sterViT-6</td>. 
+00001770: 2020 203c 7464 3e38 352e 383c 2f74 643e     <td>85.8</td>
+00001780: 0a20 2020 203c 7464 3e39 372e 343c 2f74  .    <td>97.4</t
+00001790: 643e 0a20 2020 203c 7464 3e33 3532 3c2f  d>.    <td>352</
+000017a0: 7464 3e0a 2020 2020 3c74 643e 3232 3478  td>.    <td>224x
+000017b0: 3232 343c 2f74 643e 0a20 2020 203c 7464  224</td>.    <td
+000017c0: 3e31 3336 302e 303c 2f74 643e 0a20 2020  >1360.0</td>.   
+000017d0: 203c 7464 3e31 3432 2e30 3c2f 7464 3e0a   <td>142.0</td>.
+000017e0: 2020 2020 3c74 643e 3c61 2068 7265 663d      <td><a href=
+000017f0: 2268 7474 7073 3a2f 2f64 7269 7665 2e67  "https://drive.g
+00001800: 6f6f 676c 652e 636f 6d2f 7563 3f65 7870  oogle.com/uc?exp
+00001810: 6f72 743d 646f 776e 6c6f 6164 2669 643d  ort=download&id=
+00001820: 3132 6a74 6176 5232 5178 6d4d 7a63 4b77  12jtavR2QxmMzcKw
+00001830: 507a 5765 376b 772d 6f79 3334 4959 6935  PzWe7kw-oy34IYi5
+00001840: 3922 3e6d 6f64 656c 3c2f 613e 3c2f 7464  9">model</a></td
+00001850: 3e0a 3c2f 7472 3e0a 0a3c 2f74 6162 6c65  >.</tr>..</table
+00001860: 3e0a 0a0a 2323 2320 526f 6275 7374 6e65  >...### Robustne
+00001870: 7373 2028 496d 6167 654e 6574 2d41 202d  ss (ImageNet-A -
+00001880: 2049 6d61 6765 4e65 742d 5220 2d20 496d   ImageNet-R - Im
+00001890: 6167 654e 6574 2d56 3229 0a0a 416c 6c20  ageNet-V2)..All 
+000018a0: 6d6f 6465 6c73 2075 7365 2060 6372 6f70  models use `crop
+000018b0: 5f70 6374 3d30 2e38 3735 602e 2052 6573  _pct=0.875`. Res
+000018c0: 756c 7473 2061 7265 206f 6274 6169 6e65  ults are obtaine
+000018d0: 6420 6279 2072 756e 6e69 6e67 2069 6e66  d by running inf
+000018e0: 6572 656e 6365 206f 6e20 496d 6167 654e  erence on ImageN
+000018f0: 6574 2d31 4b20 7072 6574 7261 696e 6564  et-1K pretrained
+00001900: 206d 6f64 656c 7320 7769 7468 6f75 7420   models without 
+00001910: 6669 6e65 7475 6e69 6e67 2e0a 3c74 6162  finetuning..<tab
+00001920: 6c65 3e0a 2020 3c74 723e 0a20 2020 203c  le>.  <tr>.    <
+00001930: 7468 3e4e 616d 653c 2f74 683e 0a20 2020  th>Name</th>.   
+00001940: 203c 7468 3e41 2d41 6363 4031 2825 293c   <th>A-Acc@1(%)<
+00001950: 2f74 683e 0a20 2020 203c 7468 3e41 2d41  /th>.    <th>A-A
+00001960: 6363 4035 2825 293c 2f74 683e 0a20 2020  cc@5(%)</th>.   
+00001970: 203c 7468 3e52 2d41 6363 4031 2825 293c   <th>R-Acc@1(%)<
+00001980: 2f74 683e 0a20 2020 203c 7468 3e52 2d41  /th>.    <th>R-A
+00001990: 6363 4035 2825 293c 2f74 683e 0a20 2020  cc@5(%)</th>.   
+000019a0: 203c 7468 3e56 322d 4163 6340 3128 2529   <th>V2-Acc@1(%)
+000019b0: 3c2f 7468 3e0a 2020 2020 3c74 683e 5632  </th>.    <th>V2
+000019c0: 2d41 6363 4035 2825 293c 2f74 683e 0a20  -Acc@5(%)</th>. 
+000019d0: 203c 2f74 723e 0a0a 3c74 723e 0a20 2020   </tr>..<tr>.   
+000019e0: 203c 7464 3e46 6173 7465 7256 6954 2d30   <td>FasterViT-0
+000019f0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3233  </td>.    <td>23
+00001a00: 2e39 3c2f 7464 3e0a 2020 2020 3c74 643e  .9</td>.    <td>
+00001a10: 3537 2e36 3c2f 7464 3e0a 2020 2020 3c74  57.6</td>.    <t
+00001a20: 643e 3435 2e39 3c2f 7464 3e0a 2020 2020  d>45.9</td>.    
+00001a30: 3c74 643e 3630 2e34 3c2f 7464 3e0a 2020  <td>60.4</td>.  
+00001a40: 2020 3c74 643e 3730 2e39 3c2f 7464 3e0a    <td>70.9</td>.
+00001a50: 2020 2020 3c74 643e 3930 2e30 3c2f 7464      <td>90.0</td
+00001a60: 3e0a 3c2f 7472 3e0a 0a3c 7472 3e0a 2020  >.</tr>..<tr>.  
+00001a70: 2020 3c74 643e 4661 7374 6572 5669 542d    <td>FasterViT-
+00001a80: 313c 2f74 643e 0a20 2020 203c 7464 3e33  1</td>.    <td>3
+00001a90: 312e 323c 2f74 643e 0a20 2020 203c 7464  1.2</td>.    <td
+00001aa0: 3e36 332e 333c 2f74 643e 0a20 2020 203c  >63.3</td>.    <
+00001ab0: 7464 3e34 372e 353c 2f74 643e 0a20 2020  td>47.5</td>.   
+00001ac0: 203c 7464 3e36 312e 393c 2f74 643e 0a20   <td>61.9</td>. 
+00001ad0: 2020 203c 7464 3e37 322e 363c 2f74 643e     <td>72.6</td>
+00001ae0: 0a20 2020 203c 7464 3e39 312e 303c 2f74  .    <td>91.0</t
+00001af0: 643e 0a3c 2f74 723e 0a0a 3c74 723e 0a20  d>.</tr>..<tr>. 
+00001b00: 2020 203c 7464 3e46 6173 7465 7256 6954     <td>FasterViT
+00001b10: 2d32 3c2f 7464 3e0a 2020 2020 3c74 643e  -2</td>.    <td>
+00001b20: 3338 2e32 3c2f 7464 3e0a 2020 2020 3c74  38.2</td>.    <t
+00001b30: 643e 3638 2e39 3c2f 7464 3e0a 2020 2020  d>68.9</td>.    
+00001b40: 3c74 643e 3439 2e36 3c2f 7464 3e0a 2020  <td>49.6</td>.  
+00001b50: 2020 3c74 643e 3633 2e34 3c2f 7464 3e0a    <td>63.4</td>.
+00001b60: 2020 2020 3c74 643e 3733 2e37 3c2f 7464      <td>73.7</td
+00001b70: 3e0a 2020 2020 3c74 643e 3931 2e36 3c2f  >.    <td>91.6</
+00001b80: 7464 3e0a 3c2f 7472 3e0a 0a3c 7472 3e0a  td>.</tr>..<tr>.
+00001b90: 2020 2020 3c74 643e 4661 7374 6572 5669      <td>FasterVi
+00001ba0: 542d 333c 2f74 643e 0a20 2020 203c 7464  T-3</td>.    <td
+00001bb0: 3e34 342e 323c 2f74 643e 0a20 2020 203c  >44.2</td>.    <
+00001bc0: 7464 3e37 332e 303c 2f74 643e 0a20 2020  td>73.0</td>.   
+00001bd0: 203c 7464 3e35 312e 393c 2f74 643e 0a20   <td>51.9</td>. 
+00001be0: 2020 203c 7464 3e36 352e 363c 2f74 643e     <td>65.6</td>
+00001bf0: 0a20 2020 203c 7464 3e37 352e 303c 2f74  .    <td>75.0</t
+00001c00: 643e 0a20 2020 203c 7464 3e39 322e 323c  d>.    <td>92.2<
+00001c10: 2f74 643e 0a3c 2f74 723e 0a0a 3c74 723e  /td>.</tr>..<tr>
+00001c20: 0a20 2020 203c 7464 3e46 6173 7465 7256  .    <td>FasterV
+00001c30: 6954 2d34 3c2f 7464 3e0a 2020 2020 3c74  iT-4</td>.    <t
+00001c40: 643e 3439 2e30 3c2f 7464 3e0a 2020 2020  d>49.0</td>.    
+00001c50: 3c74 643e 3735 2e34 3c2f 7464 3e0a 2020  <td>75.4</td>.  
+00001c60: 2020 3c74 643e 3536 2e30 3c2f 7464 3e0a    <td>56.0</td>.
+00001c70: 2020 2020 3c74 643e 3639 2e36 3c2f 7464      <td>69.6</td
+00001c80: 3e0a 2020 2020 3c74 643e 3735 2e37 3c2f  >.    <td>75.7</
+00001c90: 7464 3e0a 2020 2020 3c74 643e 3932 2e37  td>.    <td>92.7
+00001ca0: 3c2f 7464 3e0a 3c2f 7472 3e0a 0a3c 7472  </td>.</tr>..<tr
+00001cb0: 3e0a 2020 2020 3c74 643e 4661 7374 6572  >.    <td>Faster
+00001cc0: 5669 542d 353c 2f74 643e 0a20 2020 203c  ViT-5</td>.    <
+00001cd0: 7464 3e35 322e 373c 2f74 643e 0a20 2020  td>52.7</td>.   
+00001ce0: 203c 7464 3e37 372e 363c 2f74 643e 0a20   <td>77.6</td>. 
+00001cf0: 2020 203c 7464 3e35 362e 393c 2f74 643e     <td>56.9</td>
+00001d00: 0a20 2020 203c 7464 3e37 302e 303c 2f74  .    <td>70.0</t
+00001d10: 643e 0a20 2020 203c 7464 3e37 362e 303c  d>.    <td>76.0<
+00001d20: 2f74 643e 0a20 2020 203c 7464 3e39 332e  /td>.    <td>93.
+00001d30: 303c 2f74 643e 0a3c 2f74 723e 0a0a 3c74  0</td>.</tr>..<t
+00001d40: 723e 0a20 2020 203c 7464 3e46 6173 7465  r>.    <td>Faste
+00001d50: 7256 6954 2d36 3c2f 7464 3e0a 2020 2020  rViT-6</td>.    
+00001d60: 3c74 643e 3533 2e37 3c2f 7464 3e0a 2020  <td>53.7</td>.  
+00001d70: 2020 3c74 643e 3738 2e34 3c2f 7464 3e0a    <td>78.4</td>.
+00001d80: 2020 2020 3c74 643e 3537 2e31 3c2f 7464      <td>57.1</td
+00001d90: 3e0a 2020 2020 3c74 643e 3730 2e31 3c2f  >.    <td>70.1</
+00001da0: 7464 3e0a 2020 2020 3c74 643e 3736 2e31  td>.    <td>76.1
+00001db0: 3c2f 7464 3e0a 2020 2020 3c74 643e 3933  </td>.    <td>93
+00001dc0: 2e30 3c2f 7464 3e0a 3c2f 7472 3e0a 0a3c  .0</td>.</tr>..<
+00001dd0: 2f74 6162 6c65 3e0a 0a41 2c20 5220 616e  /table>..A, R an
+00001de0: 6420 5632 2064 656e 6f74 6520 496d 6167  d V2 denote Imag
+00001df0: 654e 6574 2d41 2c20 496d 6167 654e 6574  eNet-A, ImageNet
+00001e00: 2d52 2061 6e64 2049 6d61 6765 4e65 742d  -R and ImageNet-
+00001e10: 5632 2072 6573 7065 6374 6976 656c 792e  V2 respectively.
+00001e20: 200a 2323 2054 7261 696e 696e 670a 0a50   .## Training..P
+00001e30: 6c65 6173 6520 7365 6520 5b54 5241 494e  lease see [TRAIN
+00001e40: 494e 472e 6d64 5d28 5452 4149 4e49 4e47  ING.md](TRAINING
+00001e50: 2e6d 6429 2066 6f72 2064 6574 6169 6c65  .md) for detaile
+00001e60: 6420 7472 6169 6e69 6e67 2069 6e73 7472  d training instr
+00001e70: 7563 7469 6f6e 7320 6f66 2061 6c6c 206d  uctions of all m
+00001e80: 6f64 656c 732e 200a 0a23 2320 4576 616c  odels. ..## Eval
+00001e90: 7561 7469 6f6e 0a0a 5468 6520 4661 7374  uation..The Fast
+00001ea0: 6572 5669 5420 6d6f 6465 6c73 2063 616e  erViT models can
+00001eb0: 2062 6520 6576 616c 7561 7465 6420 6f6e   be evaluated on
+00001ec0: 2049 6d61 6765 4e65 742d 314b 2076 616c   ImageNet-1K val
+00001ed0: 6964 6174 696f 6e20 7365 7420 7573 696e  idation set usin
+00001ee0: 6720 7468 6520 666f 6c6c 6f77 696e 673a  g the following:
+00001ef0: 200a 0a60 6060 0a70 7974 686f 6e20 7661   ..```.python va
+00001f00: 6c69 6461 7465 2e70 7920 5c0a 2d2d 6d6f  lidate.py \.--mo
+00001f10: 6465 6c20 3c6d 6f64 656c 2d6e 616d 653e  del <model-name>
+00001f20: 0a2d 2d63 6865 636b 706f 696e 7420 3c63  .--checkpoint <c
+00001f30: 6865 636b 706f 696e 742d 7061 7468 3e0a  heckpoint-path>.
+00001f40: 2d2d 6461 7461 5f64 6972 203c 696d 6167  --data_dir <imag
+00001f50: 656e 6574 2d70 6174 683e 0a2d 2d62 6174  enet-path>.--bat
+00001f60: 6368 2d73 697a 6520 3c62 6174 6368 2d73  ch-size <batch-s
+00001f70: 697a 652d 7065 722d 6770 750a 6060 6020  ize-per-gpu.``` 
+00001f80: 0a0a 4865 7265 2060 2d2d 6d6f 6465 6c60  ..Here `--model`
+00001f90: 2069 7320 7468 6520 4661 7374 6572 5669   is the FasterVi
+00001fa0: 5420 7661 7269 616e 7420 2865 2e67 2e20  T variant (e.g. 
+00001fb0: 6066 6173 7465 725f 7669 745f 305f 3232  `faster_vit_0_22
+00001fc0: 345f 316b 6029 2c20 602d 2d63 6865 636b  4_1k`), `--check
+00001fd0: 706f 696e 7460 2069 7320 7468 6520 7061  point` is the pa
+00001fe0: 7468 2074 6f20 7072 6574 7261 696e 6564  th to pretrained
+00001ff0: 206d 6f64 656c 2077 6569 6768 7473 2c20   model weights, 
+00002000: 602d 2d64 6174 615f 6469 7260 2069 7320  `--data_dir` is 
+00002010: 7468 6520 7061 7468 2074 6f20 496d 6167  the path to Imag
+00002020: 654e 6574 2d31 4b20 7661 6c69 6461 7469  eNet-1K validati
+00002030: 6f6e 2073 6574 2061 6e64 2060 2d2d 6261  on set and `--ba
+00002040: 7463 682d 7369 7a65 6020 6973 2074 6865  tch-size` is the
+00002050: 206e 756d 6265 7220 6f66 2062 6174 6368   number of batch
+00002060: 2073 697a 652e 2057 6520 616c 736f 2070   size. We also p
+00002070: 726f 7669 6465 2061 2073 616d 706c 6520  rovide a sample 
+00002080: 7363 7269 7074 205b 6865 7265 5d28 2e2f  script [here](./
+00002090: 6661 7374 6572 7669 742f 7661 6c69 6461  fastervit/valida
+000020a0: 7465 2e73 6829 2e20 0a0a 0a23 2320 496e  te.sh). ...## In
+000020b0: 7374 616c 6c61 7469 6f6e 0a0a 5468 6520  stallation..The 
+000020c0: 6465 7065 6e64 656e 6369 6573 2063 616e  dependencies can
+000020d0: 2062 6520 696e 7374 616c 6c65 6420 6279   be installed by
+000020e0: 2072 756e 6e69 6e67 3a0a 0a60 6060 6261   running:..```ba
+000020f0: 7368 0a70 6970 2069 6e73 7461 6c6c 202d  sh.pip install -
+00002100: 7220 7265 7175 6972 656d 656e 7473 2e74  r requirements.t
+00002110: 7874 0a60 6060 0a0a 2323 2054 6869 7264  xt.```..## Third
+00002120: 2d70 6172 7479 2045 7874 656e 7469 6f6e  -party Extention
+00002130: 730a 5765 2061 6c77 6179 7320 7765 6c63  s.We always welc
+00002140: 6f6d 6520 7468 6972 642d 7061 7274 7920  ome third-party 
+00002150: 6578 7465 6e74 696f 6e73 2f69 6d70 6c65  extentions/imple
+00002160: 6d65 6e74 6174 696f 6e73 2061 6e64 2075  mentations and u
+00002170: 7361 6765 2066 6f72 206f 7468 6572 2070  sage for other p
+00002180: 7572 706f 7365 732e 2049 6620 796f 7520  urposes. If you 
+00002190: 776f 756c 6420 6c69 6b65 2079 6f75 7220  would like your 
+000021a0: 776f 726b 2074 6f20 6265 206c 6973 7465  work to be liste
+000021b0: 6420 696e 2074 6869 7320 7265 706f 7369  d in this reposi
+000021c0: 746f 7279 2c20 706c 6561 7365 2072 6169  tory, please rai
+000021d0: 7365 2061 6e64 2069 7373 7565 2061 6e64  se and issue and
+000021e0: 2070 726f 7669 6465 2075 7320 7769 7468   provide us with
+000021f0: 2064 6574 6169 6c65 6420 696e 666f 726d   detailed inform
+00002200: 6174 696f 6e2e 2020 0a0a 0a23 2320 4163  ation.  ...## Ac
+00002210: 6b6e 6f77 6c65 6467 656d 656e 740a 5468  knowledgement.Th
+00002220: 6973 2072 6570 6f73 6974 6f72 7920 6973  is repository is
+00002230: 2062 7569 6c74 206f 6e20 746f 7020 6f66   built on top of
+00002240: 2074 6865 205b 7469 6d6d 5d28 6874 7470   the [timm](http
+00002250: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f68  s://github.com/h
+00002260: 7567 6769 6e67 6661 6365 2f70 7974 6f72  uggingface/pytor
+00002270: 6368 2d69 6d61 6765 2d6d 6f64 656c 7329  ch-image-models)
+00002280: 2072 6570 6f73 6974 6f72 792e 2057 6520   repository. We 
+00002290: 7468 616e 6b20 5b52 6f73 7320 5772 6967  thank [Ross Wrig
+000022a0: 6874 6d61 6e5d 2868 7474 7073 3a2f 2f72  htman](https://r
+000022b0: 7769 6768 746d 616e 2e63 6f6d 2f29 2066  wightman.com/) f
+000022c0: 6f72 2063 7265 6174 696e 6720 616e 6420  or creating and 
+000022d0: 6d61 696e 7461 696e 696e 6720 7468 6973  maintaining this
+000022e0: 2068 6967 682d 7175 616c 6974 7920 6c69   high-quality li
+000022f0: 6272 6172 792e 2020 0a0a 2323 2043 6974  brary.  ..## Cit
+00002300: 6174 696f 6e0a 0a50 6c65 6173 6520 636f  ation..Please co
+00002310: 6e73 6964 6572 2063 6974 696e 6720 4661  nsider citing Fa
+00002320: 7374 6572 5669 5420 6966 2074 6869 7320  sterViT if this 
+00002330: 7265 706f 7369 746f 7279 2069 7320 7573  repository is us
+00002340: 6566 756c 2066 6f72 2079 6f75 7220 776f  eful for your wo
+00002350: 726b 3a0a 0a60 6060 0a40 6172 7469 636c  rk:..```.@articl
+00002360: 657b 6861 7461 6d69 7a61 6465 6832 3032  e{hatamizadeh202
+00002370: 3366 6173 7465 7276 6974 2c0a 2020 7469  3fastervit,.  ti
+00002380: 746c 653d 7b46 6173 7465 7256 6954 3a20  tle={FasterViT: 
+00002390: 4661 7374 2056 6973 696f 6e20 5472 616e  Fast Vision Tran
+000023a0: 7366 6f72 6d65 7273 2077 6974 6820 4869  sformers with Hi
+000023b0: 6572 6172 6368 6963 616c 2041 7474 656e  erarchical Atten
+000023c0: 7469 6f6e 7d2c 0a20 2061 7574 686f 723d  tion},.  author=
+000023d0: 7b48 6174 616d 697a 6164 6568 2c20 416c  {Hatamizadeh, Al
+000023e0: 6920 616e 6420 4865 696e 7269 6368 2c20  i and Heinrich, 
+000023f0: 4772 6567 2061 6e64 2059 696e 2c20 486f  Greg and Yin, Ho
+00002400: 6e67 7875 2061 6e64 2054 616f 2c20 416e  ngxu and Tao, An
+00002410: 6472 6577 2061 6e64 2041 6c76 6172 657a  drew and Alvarez
+00002420: 2c20 4a6f 7365 204d 2061 6e64 204b 6175  , Jose M and Kau
+00002430: 747a 2c20 4a61 6e20 616e 6420 4d6f 6c63  tz, Jan and Molc
+00002440: 6861 6e6f 762c 2050 6176 6c6f 7d2c 0a20  hanov, Pavlo},. 
+00002450: 206a 6f75 726e 616c 3d7b 6172 5869 7620   journal={arXiv 
+00002460: 7072 6570 7269 6e74 2061 7258 6976 3a32  preprint arXiv:2
+00002470: 3330 362e 3036 3138 397d 2c0a 2020 7965  306.06189},.  ye
+00002480: 6172 3d7b 3230 3233 7d0a 7d0a 6060 600a  ar={2023}.}.```.
+00002490: 0a23 2320 4c69 6365 6e73 6573 0a0a 436f  .## Licenses..Co
+000024a0: 7079 7269 6768 7420 c2a9 2032 3032 332c  pyright .. 2023,
+000024b0: 204e 5649 4449 4120 436f 7270 6f72 6174   NVIDIA Corporat
+000024c0: 696f 6e2e 2041 6c6c 2072 6967 6874 7320  ion. All rights 
+000024d0: 7265 7365 7276 6564 2e0a 0a54 6869 7320  reserved...This 
+000024e0: 776f 726b 2069 7320 6d61 6465 2061 7661  work is made ava
+000024f0: 696c 6162 6c65 2075 6e64 6572 2074 6865  ilable under the
+00002500: 204e 5649 4449 4120 536f 7572 6365 2043   NVIDIA Source C
+00002510: 6f64 6520 4c69 6365 6e73 652d 4e43 2e20  ode License-NC. 
+00002520: 436c 6963 6b20 5b68 6572 655d 284c 4943  Click [here](LIC
+00002530: 454e 5345 2920 746f 2076 6965 7720 6120  ENSE) to view a 
+00002540: 636f 7079 206f 6620 7468 6973 206c 6963  copy of this lic
+00002550: 656e 7365 2e0a 0a46 6f72 206c 6963 656e  ense...For licen
+00002560: 7365 2069 6e66 6f72 6d61 7469 6f6e 2072  se information r
+00002570: 6567 6172 6469 6e67 2074 6865 2074 696d  egarding the tim
+00002580: 6d20 7265 706f 7369 746f 7279 2c20 706c  m repository, pl
+00002590: 6561 7365 2072 6566 6572 2074 6f20 6974  ease refer to it
+000025a0: 7320 5b72 6570 6f73 6974 6f72 795d 2868  s [repository](h
+000025b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000025c0: 6d2f 7277 6967 6874 6d61 6e2f 7079 746f  m/rwightman/pyto
+000025d0: 7263 682d 696d 6167 652d 6d6f 6465 6c73  rch-image-models
+000025e0: 292e 0a0a 466f 7220 6c69 6365 6e73 6520  )...For license 
+000025f0: 696e 666f 726d 6174 696f 6e20 7265 6761  information rega
+00002600: 7264 696e 6720 7468 6520 496d 6167 654e  rding the ImageN
+00002610: 6574 2064 6174 6173 6574 2c20 706c 6561  et dataset, plea
+00002620: 7365 2073 6565 2074 6865 205b 496d 6167  se see the [Imag
+00002630: 654e 6574 206f 6666 6963 6961 6c20 7765  eNet official we
+00002640: 6273 6974 655d 2868 7474 7073 3a2f 2f77  bsite](https://w
+00002650: 7777 2e69 6d61 6765 2d6e 6574 2e6f 7267  ww.image-net.org
+00002660: 2f29 2e20 0a0a                           /). ..
```

### Comparing `fastervit-0.8.8/fastervit.egg-info/SOURCES.txt` & `fastervit-0.8.9/fastervit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastervit-0.8.8/setup.py` & `fastervit-0.8.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='fastervit',
-    version='0.8.8',
+    version='0.8.9',
     description='FasterViT: Fast Vision Transformers with Hierarchical Attention',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/NVlabs/FasterViT',
     author='Ali Hatamizadeh',
     author_email='ahatamiz123@gmail.com',
     classifiers=[
```

