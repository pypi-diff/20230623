# Comparing `tmp/vplanet-2.3.46.tar.gz` & `tmp/vplanet-2.3.47.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vplanet-2.3.46.tar", last modified: Thu Jun  1 21:32:25 2023, max compression
+gzip compressed data, was "vplanet-2.3.47.tar", last modified: Fri Jun 23 18:21:50 2023, max compression
```

## Comparing `vplanet-2.3.46.tar` & `vplanet-2.3.47.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:32:25.196032 vplanet-2.3.46/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-01 21:32:23.000000 vplanet-2.3.46/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-01 21:32:25.196032 vplanet-2.3.46/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-06-01 21:32:23.000000 vplanet-2.3.46/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 21:32:25.196032 vplanet-2.3.46/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-01 21:32:24.000000 vplanet-2.3.46/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:32:25.196032 vplanet-2.3.46/src/
--rw-r--r--   0 runner    (1001) docker     (123)   152780 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/atmesc.c
--rw-r--r--   0 runner    (1001) docker     (123)    90413 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/binary.c
--rw-r--r--   0 runner    (1001) docker     (123)    45000 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/body.c
--rw-r--r--   0 runner    (1001) docker     (123)    35872 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/control.c
--rw-r--r--   0 runner    (1001) docker     (123)   261295 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/distorb.c
--rw-r--r--   0 runner    (1001) docker     (123)    83805 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/distrot.c
--rw-r--r--   0 runner    (1001) docker     (123)   172606 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/eqtide.c
--rw-r--r--   0 runner    (1001) docker     (123)    28904 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/evolve.c
--rw-r--r--   0 runner    (1001) docker     (123)    72889 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/flare.c
--rw-r--r--   0 runner    (1001) docker     (123)   142412 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/galhabit.c
--rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/halt.c
--rw-r--r--   0 runner    (1001) docker     (123)   116525 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/magmoc.c
--rw-r--r--   0 runner    (1001) docker     (123)    93363 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/module.c
--rw-r--r--   0 runner    (1001) docker     (123)   160366 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/options.c
--rw-r--r--   0 runner    (1001) docker     (123)    83311 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/output.c
--rw-r--r--   0 runner    (1001) docker     (123)   285197 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/poise.c
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/python_interface.c
--rw-r--r--   0 runner    (1001) docker     (123)   245678 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/radheat.c
--rw-r--r--   0 runner    (1001) docker     (123)    48492 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/spinbody.c
--rw-r--r--   0 runner    (1001) docker     (123)    68566 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/stellar.c
--rw-r--r--   0 runner    (1001) docker     (123)    33897 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/system.c
--rw-r--r--   0 runner    (1001) docker     (123)   195036 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/thermint.c
--rw-r--r--   0 runner    (1001) docker     (123)   159057 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/update.c
--rw-r--r--   0 runner    (1001) docker     (123)    43824 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/verify.c
--rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-06-01 21:32:24.000000 vplanet-2.3.46/src/vplanet.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:32:25.196032 vplanet-2.3.46/vplanet/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-01 21:32:24.000000 vplanet-2.3.46/vplanet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-01 21:32:24.000000 vplanet-2.3.46/vplanet/custom_units.py
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-06-01 21:32:24.000000 vplanet-2.3.46/vplanet/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-01 21:32:24.000000 vplanet-2.3.46/vplanet/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-06-01 21:32:24.000000 vplanet-2.3.46/vplanet/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10909 2023-06-01 21:32:24.000000 vplanet-2.3.46/vplanet/quantity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-01 21:32:24.000000 vplanet-2.3.46/vplanet/quantity_support.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-01 21:32:24.000000 vplanet-2.3.46/vplanet/vplanet_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-01 21:32:24.000000 vplanet-2.3.46/vplanet/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:32:25.196032 vplanet-2.3.46/vplanet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-01 21:32:25.000000 vplanet-2.3.46/vplanet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-01 21:32:25.000000 vplanet-2.3.46/vplanet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:32:25.000000 vplanet-2.3.46/vplanet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-01 21:32:25.000000 vplanet-2.3.46/vplanet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:32:25.000000 vplanet-2.3.46/vplanet.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-01 21:32:25.000000 vplanet-2.3.46/vplanet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 21:32:25.000000 vplanet-2.3.46/vplanet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:21:50.504038 vplanet-2.3.47/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-23 18:21:48.000000 vplanet-2.3.47/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-23 18:21:50.504038 vplanet-2.3.47/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-06-23 18:21:48.000000 vplanet-2.3.47/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 18:21:50.504038 vplanet-2.3.47/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-23 18:21:49.000000 vplanet-2.3.47/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:21:50.500037 vplanet-2.3.47/src/
+-rw-r--r--   0 runner    (1001) docker     (123)   152780 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/atmesc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    90413 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/binary.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45000 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/body.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35872 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/control.c
+-rw-r--r--   0 runner    (1001) docker     (123)   261295 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/distorb.c
+-rw-r--r--   0 runner    (1001) docker     (123)    83805 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/distrot.c
+-rw-r--r--   0 runner    (1001) docker     (123)   172606 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/eqtide.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28904 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/evolve.c
+-rw-r--r--   0 runner    (1001) docker     (123)    72892 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/flare.c
+-rw-r--r--   0 runner    (1001) docker     (123)   142412 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/galhabit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/halt.c
+-rw-r--r--   0 runner    (1001) docker     (123)   116525 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/magmoc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    93363 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)   160366 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/options.c
+-rw-r--r--   0 runner    (1001) docker     (123)    83311 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/output.c
+-rw-r--r--   0 runner    (1001) docker     (123)   285197 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/poise.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/python_interface.c
+-rw-r--r--   0 runner    (1001) docker     (123)   245678 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/radheat.c
+-rw-r--r--   0 runner    (1001) docker     (123)    48492 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/spinbody.c
+-rw-r--r--   0 runner    (1001) docker     (123)    68566 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/stellar.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33897 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/system.c
+-rw-r--r--   0 runner    (1001) docker     (123)   195036 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/thermint.c
+-rw-r--r--   0 runner    (1001) docker     (123)   159057 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/update.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43824 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/verify.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5463 2023-06-23 18:21:49.000000 vplanet-2.3.47/src/vplanet.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:21:50.504038 vplanet-2.3.47/vplanet/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-23 18:21:49.000000 vplanet-2.3.47/vplanet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-23 18:21:49.000000 vplanet-2.3.47/vplanet/custom_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-06-23 18:21:49.000000 vplanet-2.3.47/vplanet/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-23 18:21:49.000000 vplanet-2.3.47/vplanet/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-06-23 18:21:49.000000 vplanet-2.3.47/vplanet/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10909 2023-06-23 18:21:49.000000 vplanet-2.3.47/vplanet/quantity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-23 18:21:49.000000 vplanet-2.3.47/vplanet/quantity_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-23 18:21:49.000000 vplanet-2.3.47/vplanet/vplanet_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-23 18:21:49.000000 vplanet-2.3.47/vplanet/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 18:21:50.504038 vplanet-2.3.47/vplanet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10254 2023-06-23 18:21:50.000000 vplanet-2.3.47/vplanet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-23 18:21:50.000000 vplanet-2.3.47/vplanet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:21:50.000000 vplanet-2.3.47/vplanet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-23 18:21:50.000000 vplanet-2.3.47/vplanet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 18:21:50.000000 vplanet-2.3.47/vplanet.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-23 18:21:50.000000 vplanet-2.3.47/vplanet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-23 18:21:50.000000 vplanet-2.3.47/vplanet.egg-info/top_level.txt
```

### Comparing `vplanet-2.3.46/LICENSE` & `vplanet-2.3.47/LICENSE`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/PKG-INFO` & `vplanet-2.3.47/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vplanet
-Version: 2.3.46
+Version: 2.3.47
 Summary: The virtual planet simulator
 Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes
 Author-email: rkb9@uw.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vplanet Version: 2.3.46 Summary: The virtual planet
+Metadata-Version: 2.1 Name: vplanet Version: 2.3.47 Summary: The virtual planet
 simulator Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes Author-email: rkb9@uw.edu License: MIT Platform: UNKNOWN
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE
                         [docs/VPLanetLogo.png?raw=true]
               ****** VPLanet: The Virtual Planet Simulator ******
   [https://img.shields.io/badge/Read-the_docs-blue.svg?style=flat] [https://
```

### Comparing `vplanet-2.3.46/README.md` & `vplanet-2.3.47/README.md`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/setup.py` & `vplanet-2.3.47/setup.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/atmesc.c` & `vplanet-2.3.47/src/atmesc.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/binary.c` & `vplanet-2.3.47/src/binary.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/body.c` & `vplanet-2.3.47/src/body.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/control.c` & `vplanet-2.3.47/src/control.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/distorb.c` & `vplanet-2.3.47/src/distorb.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/distrot.c` & `vplanet-2.3.47/src/distrot.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/eqtide.c` & `vplanet-2.3.47/src/eqtide.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/evolve.c` & `vplanet-2.3.47/src/evolve.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/flare.c` & `vplanet-2.3.47/src/flare.c`

 * *Files 1% similar despite different names*

```diff
@@ -613,29 +613,29 @@
   options[OPT_FLAREBANDPASS].iType      = 3;
   options[OPT_FLAREBANDPASS].bMultiFile = 1;
   fnRead[OPT_FLAREBANDPASS]             = &ReadFlareBandPass;
   sprintf(options[OPT_FLAREBANDPASS].cLongDescr,
           /*
           "If UV or GOES is selected, the code will convert \n"
           "the input energy of flares from the UV band \n"
-          "(3000-4300 Å) or GOES band (1-8 Å) to the Kepler band \n"
-          "(4000-9000 Å) to calculate the FFD and the SXR \n"
-          "band (1.24 - 1239.85 Å) to calculate the luminosity.\n"
+          "(3000-4300A) or GOES band (1-8A) to the Kepler band \n"
+          "(4000-9000A) to calculate the FFD and the SXR \n"
+          "band (1.24 - 1239.85A) to calculate the luminosity.\n"
           " If SXR is selected, the code will convert the \n"
           "input energy of flares from the SXR band to the Kepler\n"
           "band to calculate the FFD and will use the same \n"
           "value of energy to calculate the luminosity .\n"
           "If KEPLER is selected, the code will use the same\n"
           "input energy to calculate the FFD and will convert \n"
           "the input energy to SXR band to calculate the \n"
           "luminosity. The conversion values are taken from \n"
           "Osten and Wolk (2015) (doi:10.1088/0004-637X/809/1/79).\n"
           "If TESSUV is selected, then the code will convert\n"
           "the input energy of flares using the conversion value\n"
-          "to the band U (2000-2800 Å) to the TESS data from \n"
+          "to the band U (2000-2800A) to the TESS data from \n"
           "Gunther et al 2020 (https://doi.org/10.3847/1538-3881/ab5d3a). \n"
           "If the BOLOMETRIC its selected, the code will convert the input \n"
           "energy of flares using the conversion values are taken \n"
           "from Osten and Wolk (2015) (doi:10.1088/0004-637X/809/1/79).\n"
           */
           "Currently suppressed due to execution errors."
   );
@@ -1739,16 +1739,16 @@
   int i, iLogEnergyMinERG, iLogEnergyMaxERG, iLogEnergyMin, iLogEnergyMax;
   double dEnergyMinXUV, dEnergyMaxXUV, dLogEnergyMinXUV;
   int iLogEnergyMinERGXUV, iLogEnergyMaxERGXUV, iLogEnergyMinXUV,
         iLogEnergyMaxXUV;
   double dEnergyStep, dEnergyStepXUV, dEnergyBin;
 
 
-  //######################### 1. Choosing how to calculate FFD: slopes(age) or
-  // slopes(constant)?##################################
+  // ######################### 1. Choosing how to calculate FFD: slopes(age) or
+  //  slopes(constant)?##################################
 
   if (body[iBody].iFlareFFD == FLARE_FFD_DAVENPORT) {
     // The coefficient values given here were given by Dr. James Davenport in
     // private comunication
     dFlareSlope =
           fdDavenport(-0.07, 0.79, -1.06, body[iBody].dAge,
                       body[iBody].dMass); //(-0.07054598,0.81225239,-1.07054511)
@@ -1763,29 +1763,29 @@
     /*dFlareSlopeErrorUpper = body[iBody].dFlareSlopeErrorUpper;
     dFlareSlopeErrorLower = body[iBody].dFlareSlopeErrorLower;
     dFlareYIntErrorUpper = body[iBody].dFlareYIntErrorUpper;
     dFlareYIntErrorLower = body[iBody].dFlareYIntErrorLower;*/
   }
   if (body[iBody].iFlareFFD == FLARE_FFD_DAVENPORT ||
       body[iBody].iFlareFFD == FLARE_FFD_LACY) {
-    //################# 2. Calculating the XUV energy (SXR 1.24 - 1239.85
-    //Å)#######################################################
+    // ################# 2. Calculating the XUV energy (SXR 1.24 - 1239.85
+    // Å)#######################################################
 
     dLogEnergyMinXUV = fdBandPassXUV(body, iBody, body[iBody].dFlareMinEnergy);
 
     // Defining the array size (dEnergybin) of energies
     dEnergyBin = body[iBody].dEnergyBin;
     iEnergyBin = (int)dEnergyBin;
 
     // Declaring the XUV Energy arrays of size dEnergyBin
     // double daEnergyJOUXUV[iEnergyBin + 1], daLogEnerXUV[iEnergyBin + 1],
     //      daEnergyERGXUV[iEnergyBin + 1];
 
-    //################# 3. Calculating the energy in the Kepler band pass (4000
-    //– 9000 Å) ##############################################
+    // ################# 3. Calculating the energy in the Kepler band pass (4000
+    // – 9000 Å) ##############################################
 
     dLogEnergyMin = fdBandPassKepler(body, iBody, body[iBody].dFlareMinEnergy);
     dLogEnergyMax = fdBandPassKepler(body, iBody, body[iBody].dFlareMaxEnergy);
 
     // 1.0 J = 1.0e7 ergs, but this is in log, so we have to sum 7.0, not
     // multiply by 1.0e7 Convert the units of the energy from Joules to ergs
     // because Davenport et al. 2019 model only accepts energy in ergs.
@@ -1797,16 +1797,16 @@
     // energy arrays
     dEnergyStep = (dLogEnergyMaxERG - dLogEnergyMinERG) / iEnergyBin;
 
     // Declaring the Kepler Energy arrays of size iEnergyBin
     // double daEnergyERG[iEnergyBin + 1], daEnergyJOU[iEnergyBin + 1],
     //      daLogEner[iEnergyBin + 1], daEnerJOU[iEnergyBin + 1];
 
-    //############################ 4. Filling the energy arrays
-    //########################################################################
+    // ############################ 4. Filling the energy arrays
+    // ########################################################################
 
     for (i = 0; i < iEnergyBin + 1; i++) {
       // XUV energy (energy_joules)
       body[iBody].daEnergyJOUXUV[i] =
             fdEnergyJoulesXUV(dLogEnergyMinXUV + i * dEnergyStep);
       // Kepler energy (log(energy_ergs))
       body[iBody].daLogEner[i] = dLogEnergyMinERG + i * dEnergyStep;
@@ -1817,16 +1817,16 @@
     body[iBody].dFlareEnergy1   = body[iBody].daEnerJOU[0];
     body[iBody].dFlareEnergy2   = body[iBody].daEnerJOU[1];
     body[iBody].dFlareEnergy3   = body[iBody].daEnerJOU[2];
     body[iBody].dFlareEnergy4   = body[iBody].daEnerJOU[3];
     body[iBody].dFlareEnergyMin = body[iBody].daEnerJOU[0];
     body[iBody].dFlareEnergyMid = body[iBody].daEnerJOU[iEnergyBin / 2];
     body[iBody].dFlareEnergyMax = body[iBody].daEnerJOU[iEnergyBin];
-    //############################ 5. Filling the FFD arrays
-    //########################################################################
+    // ############################ 5. Filling the FFD arrays
+    // ########################################################################
 
     // Declaring the Flare Frequency distribution (FFD) arrays of size
     // dEnergyBin
     // double daFFD[iEnergyBin + 1];
 
     // When DAVENPORT or LACY are selected, we have to calculate the FFD first.
     for (i = 0; i < iEnergyBin + 1; i++) {
@@ -1837,17 +1837,17 @@
     body[iBody].dFlareFreq1   = body[iBody].daFFD[0];
     body[iBody].dFlareFreq2   = body[iBody].daFFD[1];
     body[iBody].dFlareFreq3   = body[iBody].daFFD[2];
     body[iBody].dFlareFreq4   = body[iBody].daFFD[3];
     body[iBody].dFlareFreqMin = body[iBody].daFFD[0];
     body[iBody].dFlareFreqMid = body[iBody].daFFD[iEnergyBin / 2];
     body[iBody].dFlareFreqMax = body[iBody].daFFD[iEnergyBin];
-    //############################ 6. Calculating the XUV luminosity by flares
-    //########################################################################
-    // double daLXUVFlare[iEnergyBin];
+    // ############################ 6. Calculating the XUV luminosity by flares
+    // ########################################################################
+    //  double daLXUVFlare[iEnergyBin];
 
     // Calculating the luminosity by flares for DAVENPORT or LACY mode
     // if the user select to calculate the luminosity using a FFD model
     for (i = 0; i < iEnergyBin; i++) {
       body[iBody].daLXUVFlare[i] =
             (body[iBody].daEnergyJOUXUV[i + 1] -
              body[iBody].daEnergyJOUXUV[i]) *
```

### Comparing `vplanet-2.3.46/src/galhabit.c` & `vplanet-2.3.47/src/galhabit.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/halt.c` & `vplanet-2.3.47/src/halt.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/magmoc.c` & `vplanet-2.3.47/src/magmoc.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/module.c` & `vplanet-2.3.47/src/module.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/options.c` & `vplanet-2.3.47/src/options.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/output.c` & `vplanet-2.3.47/src/output.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/poise.c` & `vplanet-2.3.47/src/poise.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/python_interface.c` & `vplanet-2.3.47/src/python_interface.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/radheat.c` & `vplanet-2.3.47/src/radheat.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/spinbody.c` & `vplanet-2.3.47/src/spinbody.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/stellar.c` & `vplanet-2.3.47/src/stellar.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/system.c` & `vplanet-2.3.47/src/system.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/thermint.c` & `vplanet-2.3.47/src/thermint.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/update.c` & `vplanet-2.3.47/src/update.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/verify.c` & `vplanet-2.3.47/src/verify.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/src/vplanet.c` & `vplanet-2.3.47/src/vplanet.c`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/vplanet/custom_units.py` & `vplanet-2.3.47/vplanet/custom_units.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/vplanet/log.py` & `vplanet-2.3.47/vplanet/log.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/vplanet/output.py` & `vplanet-2.3.47/vplanet/output.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/vplanet/quantity.py` & `vplanet-2.3.47/vplanet/quantity.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/vplanet/quantity_support.py` & `vplanet-2.3.47/vplanet/quantity_support.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/vplanet/wrapper.py` & `vplanet-2.3.47/vplanet/wrapper.py`

 * *Files identical despite different names*

### Comparing `vplanet-2.3.46/vplanet.egg-info/PKG-INFO` & `vplanet-2.3.47/vplanet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vplanet
-Version: 2.3.46
+Version: 2.3.47
 Summary: The virtual planet simulator
 Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes
 Author-email: rkb9@uw.edu
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vplanet Version: 2.3.46 Summary: The virtual planet
+Metadata-Version: 2.1 Name: vplanet Version: 2.3.47 Summary: The virtual planet
 simulator Home-page: https://github.com/VirtualPlanetaryLaboratory/vplanet
 Author: Rory Barnes Author-email: rkb9@uw.edu License: MIT Platform: UNKNOWN
 Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
 LICENSE
                         [docs/VPLanetLogo.png?raw=true]
               ****** VPLanet: The Virtual Planet Simulator ******
   [https://img.shields.io/badge/Read-the_docs-blue.svg?style=flat] [https://
```

### Comparing `vplanet-2.3.46/vplanet.egg-info/SOURCES.txt` & `vplanet-2.3.47/vplanet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

