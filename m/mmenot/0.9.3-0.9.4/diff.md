# Comparing `tmp/mmenot-0.9.3-py3-none-any.whl.zip` & `tmp/mmenot-0.9.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 28770 bytes, number of entries: 22
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 07:40 __init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 07:40 mmenot/__init__.py
+Zip file size: 28888 bytes, number of entries: 22
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 10:51 __init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-17 05:36 mmenot/__init__.py
 -rw-r--r--  2.0 unx     2984 b- defN 23-Jun-06 11:15 mmenot/exporter.py
--rw-r--r--  2.0 unx     4675 b- defN 23-Jun-20 02:58 mmenot/hyp_searcher.py
+-rw-r--r--  2.0 unx     4722 b- defN 23-Jun-23 08:26 mmenot/hyp_searcher.py
 -rw-r--r--  2.0 unx     5567 b- defN 23-Jun-06 11:15 mmenot/labels.py
 -rw-r--r--  2.0 unx     1454 b- defN 23-Jun-02 17:43 mmenot/patches.py
 -rw-r--r--  2.0 unx     5732 b- defN 23-Jun-05 06:33 mmenot/pruner.py
 -rw-r--r--  2.0 unx      689 b- defN 23-Jun-05 06:33 mmenot/runner.py
 -rw-r--r--  2.0 unx     3081 b- defN 23-Jun-06 11:15 mmenot/tester.py
 -rw-r--r--  2.0 unx     5044 b- defN 23-Jun-06 11:15 mmenot/trainer.py
--rw-r--r--  2.0 unx      120 b- defN 23-Jun-02 17:47 mmenot/loops/__init__.py
--rw-r--r--  2.0 unx     2700 b- defN 23-Jun-06 11:35 mmenot/loops/epoch_optuna.py
+-rw-r--r--  2.0 unx      120 b- defN 23-Jun-02 17:48 mmenot/loops/__init__.py
+-rw-r--r--  2.0 unx     2700 b- defN 23-Jun-06 11:36 mmenot/loops/epoch_optuna.py
 -rw-r--r--  2.0 unx     6075 b- defN 23-Jun-06 11:15 mmenot/loops/epoch_pruning.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-21 07:40 mmenot/utils/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-06 11:20 mmenot/utils/__init__.py
 -rw-r--r--  2.0 unx    11727 b- defN 23-Jun-06 11:15 mmenot/utils/common.py
--rw-r--r--  2.0 unx     1742 b- defN 23-Jun-20 02:58 mmenot/utils/hpo.py
--rw-rw-rw-  2.0 unx    11338 b- defN 23-Jun-21 07:42 mmenot-0.9.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    14279 b- defN 23-Jun-21 07:42 mmenot-0.9.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-21 07:42 mmenot-0.9.3.dist-info/WHEEL
--rw-r--r--  2.0 unx      179 b- defN 23-Jun-21 07:42 mmenot-0.9.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       16 b- defN 23-Jun-21 07:42 mmenot-0.9.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1693 b- defN 23-Jun-21 07:42 mmenot-0.9.3.dist-info/RECORD
-22 files, 79187 bytes uncompressed, 26064 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx     2185 b- defN 23-Jun-23 08:26 mmenot/utils/hpo.py
+-rw-rw-rw-  2.0 unx    11338 b- defN 23-Jun-23 08:37 mmenot-0.9.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14279 b- defN 23-Jun-23 08:37 mmenot-0.9.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 08:37 mmenot-0.9.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx      179 b- defN 23-Jun-23 08:37 mmenot-0.9.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-Jun-23 08:37 mmenot-0.9.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1693 b- defN 23-Jun-23 08:37 mmenot-0.9.4.dist-info/RECORD
+22 files, 79677 bytes uncompressed, 26182 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: mmenot/utils/common.py
 Comment: 
 
 Filename: mmenot/utils/hpo.py
 Comment: 
 
-Filename: mmenot-0.9.3.dist-info/LICENSE
+Filename: mmenot-0.9.4.dist-info/LICENSE
 Comment: 
 
-Filename: mmenot-0.9.3.dist-info/METADATA
+Filename: mmenot-0.9.4.dist-info/METADATA
 Comment: 
 
-Filename: mmenot-0.9.3.dist-info/WHEEL
+Filename: mmenot-0.9.4.dist-info/WHEEL
 Comment: 
 
-Filename: mmenot-0.9.3.dist-info/entry_points.txt
+Filename: mmenot-0.9.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: mmenot-0.9.3.dist-info/top_level.txt
+Filename: mmenot-0.9.4.dist-info/top_level.txt
 Comment: 
 
-Filename: mmenot-0.9.3.dist-info/RECORD
+Filename: mmenot-0.9.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mmenot/hyp_searcher.py

```diff
@@ -51,15 +51,15 @@
         help='Learning rate range',
     )
     parser.add_argument(
         '--optimizers',
         type=str,
         default=['SGD', 'AdamW', 'RAdam'],
         nargs='+',
-        help='PyTorch optimizers',
+        help='PyTorch optimizers. SGD, Adam, AdamW and RAdam supported for now.',
     )
     parser.add_argument(
         '--warmup-range',
         type=int,
         default=[500, 1500],
         nargs=2,
         help='Warmup iterations range',
```

## mmenot/utils/hpo.py

```diff
@@ -15,19 +15,29 @@
         warmup = trial.suggest_int(
             name='warmup',
             low=self.config['low_warmup'],
             high=self.config['high_warmup'],
         )
         optimizer = trial.suggest_categorical(name='optimizer', choices=self.config['optimizers'])
 
+        default_optimizer_options = self.config['optim_wrapper']['optimizer']
+
+        opt_kwargs = {}
+
         if optimizer == 'SGD':
-            self.config['optim_wrapper']['optimizer']['momentum'] = 0.9
+            for parameter in ('momentum', 'weight_decay'):
+                if parameter in default_optimizer_options:
+                    opt_kwargs[parameter] = default_optimizer_options[parameter]
+
+        if optimizer in ('Adam', 'AdamW', 'RAdam'):
+            for parameter in ('betas', 'weight_decay'):
+                if parameter in default_optimizer_options:
+                    opt_kwargs[parameter] = default_optimizer_options[parameter]
 
-        self.config['optim_wrapper']['optimizer']['type'] = optimizer
-        self.config['optim_wrapper']['optimizer']['lr'] = lr
+        self.config['optim_wrapper']['optimizer'] = dict(type=optimizer, lr=lr, **opt_kwargs)
         self.config['param_scheduler'][0]['end'] = warmup
         self.config['work_dir'] = self.config['base_work_dir'] + f'/lr={lr:1.7f}_wu={warmup}_opt={optimizer}'
         runner = Runner.from_cfg(self.config)
         runner.trial = trial  # type: ignore
         runner.train()
         return runner.objective
```

## Comparing `mmenot-0.9.3.dist-info/LICENSE` & `mmenot-0.9.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mmenot-0.9.3.dist-info/METADATA` & `mmenot-0.9.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmenot
-Version: 0.9.3
+Version: 0.9.4
 Summary: ENOT Framework integration package for OpenMMLab codebase
 Author-email: ENOT LLC <enot@enot.ai>
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

## Comparing `mmenot-0.9.3.dist-info/RECORD` & `mmenot-0.9.4.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 __init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mmenot/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mmenot/exporter.py,sha256=jpIA-IadAUG6dGtROQvPzbg4OvWrN_54PRI5frWQVXY,2984
-mmenot/hyp_searcher.py,sha256=A9ivzzOFkF-P0MJ293Gp4i5peMBkMntOKmPe5gHAm7s,4675
+mmenot/hyp_searcher.py,sha256=kidAVMYNeRPxn7CZI-YQI0lWBqSR8g9Z8lmvao34ZJY,4722
 mmenot/labels.py,sha256=hrUDRLunoRj0e8zvWd_4C-cxmDOS-U5Cqvzz2YGBiJU,5567
 mmenot/patches.py,sha256=eAAA_cTW8L2jEhCp3_QGMKGSJia9kugy5C26lAGeZvQ,1454
 mmenot/pruner.py,sha256=aFTaD5z6xVAWrv4GvrbbYaidJeBHa2ihA9FT9BdnW_0,5732
 mmenot/runner.py,sha256=mV2Me-1EVkVWrMBFvnZyHZHc3D03q6CKHX6n0DLClNk,689
 mmenot/tester.py,sha256=STRaECaGWo88YglT6JPz3SmpqeUKjNwKI55lKIKXYg0,3081
 mmenot/trainer.py,sha256=LmQOD2D-YMjEtWS03omqffsYA33onFCBwWqttMj7NAI,5044
 mmenot/loops/__init__.py,sha256=OoUG7Z9n3SvZFV_R9sLk-2B5C_INFDh7ecJP20MqZTM,120
 mmenot/loops/epoch_optuna.py,sha256=NShq6HfgDUE6FxI1M-49jiYdX_FdW8UPwO5NCa4bCiQ,2700
 mmenot/loops/epoch_pruning.py,sha256=q60fqumaQPuQf4d_mu-DcXkp-VYrE-R206dajuHGj8U,6075
 mmenot/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mmenot/utils/common.py,sha256=DNEhes3E4vF0JdvoP7xL5mQ9t-Fsm00pnk-7JcaINVA,11727
-mmenot/utils/hpo.py,sha256=cAy_lhbkgizRg657m2l-XMb29PxxQzCHj4Fwyr9g_6k,1742
-mmenot-0.9.3.dist-info/LICENSE,sha256=iWLEJUustLjDYQcmBAwQmj0-kh3XqQi2kHpvDIc8suA,11338
-mmenot-0.9.3.dist-info/METADATA,sha256=hCv4IGeAqDDlJDOeFY6hmNsYCN4k0wj6ogSvEoXLhj4,14279
-mmenot-0.9.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mmenot-0.9.3.dist-info/entry_points.txt,sha256=m8G4sSO_-5Cm3QTYwDE5MgovucW9CQ5NV-cpw6qbVqQ,179
-mmenot-0.9.3.dist-info/top_level.txt,sha256=hvzXbej5hbn5YET1ne-y6ZJc6cSeCAMmha4HDiFCA5Q,16
-mmenot-0.9.3.dist-info/RECORD,,
+mmenot/utils/hpo.py,sha256=IbC-5sM-jC7efRq3GHVASKZnTCKWLVf0qh-DU9hgQT0,2185
+mmenot-0.9.4.dist-info/LICENSE,sha256=iWLEJUustLjDYQcmBAwQmj0-kh3XqQi2kHpvDIc8suA,11338
+mmenot-0.9.4.dist-info/METADATA,sha256=Dv3Hr2osLdYfHIzEgVyF7AdQ6rbslfFFljnAP5R2iNc,14279
+mmenot-0.9.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mmenot-0.9.4.dist-info/entry_points.txt,sha256=m8G4sSO_-5Cm3QTYwDE5MgovucW9CQ5NV-cpw6qbVqQ,179
+mmenot-0.9.4.dist-info/top_level.txt,sha256=hvzXbej5hbn5YET1ne-y6ZJc6cSeCAMmha4HDiFCA5Q,16
+mmenot-0.9.4.dist-info/RECORD,,
```

