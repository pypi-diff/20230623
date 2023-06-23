# Comparing `tmp/gregory_online-0.3.6.tar.gz` & `tmp/gregory_online-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gregory_online-0.3.6.tar", last modified: Fri Jun 23 14:48:12 2023, max compression
+gzip compressed data, was "gregory_online-0.3.7.tar", last modified: Fri Jun 23 16:49:03 2023, max compression
```

## Comparing `gregory_online-0.3.6.tar` & `gregory_online-0.3.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 14:48:12.619422 gregory_online-0.3.6/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-23 14:48:12.615422 gregory_online-0.3.6/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-02 15:20:26.000000 gregory_online-0.3.6/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 14:48:12.611422 gregory_online-0.3.6/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    70902 2023-06-23 13:32:52.000000 gregory_online-0.3.6/bin/gregory_online
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 14:48:12.615422 gregory_online-0.3.6/gregory_online/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    28897 2023-06-23 14:26:22.000000 gregory_online-0.3.6/gregory_online/ascgeneric.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7269 2023-06-23 07:56:33.000000 gregory_online-0.3.6/gregory_online/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 14:48:12.615422 gregory_online-0.3.6/gregory_online/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    56290 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/Am241.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   503044 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/Cm247.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    53304 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/Np237.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    79580 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/Pa231.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    93285 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/Pu239.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59999 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/Th232.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    78694 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/U235.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    97718 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/U238.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   123572 2023-06-12 07:00:49.000000 gregory_online-0.3.6/gregory_online/data/decay_lara.parquet
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1139 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/data/testrebin.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3758 2023-06-12 07:00:49.000000 gregory_online-0.3.6/gregory_online/decay_db.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    15128 2023-06-23 07:56:33.000000 gregory_online-0.3.6/gregory_online/dpp2jpg.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3631 2023-06-23 07:56:33.000000 gregory_online-0.3.6/gregory_online/erlang.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12625 2023-06-12 07:00:49.000000 gregory_online-0.3.6/gregory_online/fetchnp.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4741 2023-06-23 13:32:00.000000 gregory_online-0.3.6/gregory_online/histo_analyze.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4169 2023-06-23 07:56:33.000000 gregory_online-0.3.6/gregory_online/histo_displ.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      833 2023-06-12 07:00:49.000000 gregory_online-0.3.6/gregory_online/histo_global_cont.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    19157 2023-06-23 14:23:01.000000 gregory_online-0.3.6/gregory_online/histo_io.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-06-05 13:33:05.000000 gregory_online-0.3.6/gregory_online/histo_np_ops.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-19 12:31:34.000000 gregory_online-0.3.6/gregory_online/key_enter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2594 2023-06-23 07:56:33.000000 gregory_online-0.3.6/gregory_online/topbar.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2023-03-15 09:15:19.000000 gregory_online-0.3.6/gregory_online/utilone.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3293 2023-06-12 07:00:49.000000 gregory_online-0.3.6/gregory_online/utils.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-23 14:48:12.000000 gregory_online-0.3.6/gregory_online/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 14:48:12.615422 gregory_online-0.3.6/gregory_online.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-23 14:48:12.000000 gregory_online-0.3.6/gregory_online.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1006 2023-06-23 14:48:12.000000 gregory_online-0.3.6/gregory_online.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-23 14:48:12.000000 gregory_online-0.3.6/gregory_online.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      127 2023-06-23 14:48:12.000000 gregory_online-0.3.6/gregory_online.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-23 14:48:12.000000 gregory_online-0.3.6/gregory_online.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-23 14:48:12.619422 gregory_online-0.3.6/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1275 2023-06-23 14:29:08.000000 gregory_online-0.3.6/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 16:49:03.835252 gregory_online-0.3.7/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-23 16:49:03.835252 gregory_online-0.3.7/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-23 16:48:58.000000 gregory_online-0.3.7/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 16:49:03.831252 gregory_online-0.3.7/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    71947 2023-06-23 16:49:01.000000 gregory_online-0.3.7/bin/gregory_online
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 16:49:03.835252 gregory_online-0.3.7/gregory_online/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2022-09-16 15:11:00.000000 gregory_online-0.3.7/gregory_online/__init__.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    28897 2023-06-23 15:08:16.000000 gregory_online-0.3.7/gregory_online/ascgeneric.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7269 2023-06-22 10:59:40.000000 gregory_online-0.3.7/gregory_online/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 16:49:03.835252 gregory_online-0.3.7/gregory_online/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    56290 2022-09-16 15:11:00.000000 gregory_online-0.3.7/gregory_online/data/Am241.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   503044 2022-09-16 15:11:00.000000 gregory_online-0.3.7/gregory_online/data/Cm247.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    53304 2022-09-16 15:11:00.000000 gregory_online-0.3.7/gregory_online/data/Np237.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    79580 2022-09-16 15:11:00.000000 gregory_online-0.3.7/gregory_online/data/Pa231.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    93285 2022-09-16 15:11:00.000000 gregory_online-0.3.7/gregory_online/data/Pu239.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59999 2022-09-16 15:11:00.000000 gregory_online-0.3.7/gregory_online/data/Th232.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    78694 2022-09-16 15:11:00.000000 gregory_online-0.3.7/gregory_online/data/U235.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    97718 2022-09-16 15:11:00.000000 gregory_online-0.3.7/gregory_online/data/U238.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   123572 2023-06-09 11:53:23.000000 gregory_online-0.3.7/gregory_online/data/decay_lara.parquet
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1139 2022-12-08 12:00:24.000000 gregory_online-0.3.7/gregory_online/data/testrebin.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3758 2023-06-15 17:28:12.000000 gregory_online-0.3.7/gregory_online/decay_db.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    15128 2023-06-22 14:04:43.000000 gregory_online-0.3.7/gregory_online/dpp2jpg.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3631 2023-06-20 16:28:39.000000 gregory_online-0.3.7/gregory_online/erlang.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12625 2023-06-09 14:56:20.000000 gregory_online-0.3.7/gregory_online/fetchnp.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4741 2023-06-23 13:33:45.000000 gregory_online-0.3.7/gregory_online/histo_analyze.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4169 2023-06-21 08:03:02.000000 gregory_online-0.3.7/gregory_online/histo_displ.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      833 2023-06-06 11:16:18.000000 gregory_online-0.3.7/gregory_online/histo_global_cont.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    19774 2023-06-23 16:29:34.000000 gregory_online-0.3.7/gregory_online/histo_io.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-06-05 13:29:49.000000 gregory_online-0.3.7/gregory_online/histo_np_ops.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-20 14:10:17.000000 gregory_online-0.3.7/gregory_online/key_enter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2594 2023-06-16 08:42:44.000000 gregory_online-0.3.7/gregory_online/topbar.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2022-09-16 15:11:00.000000 gregory_online-0.3.7/gregory_online/utilone.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3293 2023-06-09 14:10:12.000000 gregory_online-0.3.7/gregory_online/utils.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-23 16:49:03.000000 gregory_online-0.3.7/gregory_online/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 16:49:03.835252 gregory_online-0.3.7/gregory_online.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-23 16:49:03.000000 gregory_online-0.3.7/gregory_online.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1006 2023-06-23 16:49:03.000000 gregory_online-0.3.7/gregory_online.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-23 16:49:03.000000 gregory_online-0.3.7/gregory_online.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      127 2023-06-23 16:49:03.000000 gregory_online-0.3.7/gregory_online.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-23 16:49:03.000000 gregory_online-0.3.7/gregory_online.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-23 16:49:03.835252 gregory_online-0.3.7/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1275 2023-06-23 15:08:16.000000 gregory_online-0.3.7/setup.py
```

### Comparing `gregory_online-0.3.6/PKG-INFO` & `gregory_online-0.3.7/gregory_online.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: gregory_online
-Version: 0.3.6
+Name: gregory-online
+Version: 0.3.7
 Summary: Online watching HTTP server of ROOT on port 9009
+Home-page: UNKNOWN
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Project gregory~online~
 =======================
 
 *experimental code to online survey root spectra from THTTPServer*
 
@@ -77,7 +79,9 @@
   mock~server~.py         
   rebin.py                
   setup.py                
   topbar.py               
   utilone.py              
   version.py              
   ----------------------- ------------------------------
+
+
```

### Comparing `gregory_online-0.3.6/README.md` & `gregory_online-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/bin/gregory_online` & `gregory_online-0.3.7/bin/gregory_online`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 # histo content manip
 from  gregory_online.histo_analyze import histo_details, histo_zoomenergy, \
     histo_zoombins, histo_unzoom, histo_area, bin2ene, ene2bin, \
     get_calib_coefs, histo_fit, get_ene_range
 
 
 import gregory_online.histo_io as histo_io
-from  gregory_online.histo_io import save_hist_txt, select_histo_to_load, load_hist_txt
+from  gregory_online.histo_io import save_hist_txt, select_histo_to_load
 
 import gregory_online.ascgeneric as ascgeneric  # asc_stat_print - orig.  pd_detect_zeroes
 
 from  gregory_online.histo_displ import display_h_name, display_np, refresh_canvases
 from  gregory_online.decay_db import decay_candidates
 
 
@@ -535,15 +535,21 @@
                     #     res = histo_fit( histograms["last"],  canvas = None )# "fitresult")
                     #     if res is not None:
                     #         if "area" in res.keys() and "E" in res.keys():
                     #             k40 = res["area"]
                     # print("test",f"{HOSTNAME}_grg",f"rate={rate:.1f},k40={k40}")
                     # #influxwrite("test",f"{HOSTNAME}_grg",f"rate={rate:.1f},k40={k40}")
 
-            if not scr_outputed: print(f"i... {fg.magenta} {dt.datetime.now().strftime('%H:%M:%S.%f')[:10]}  {fg.default}            ", end = "\r")
+            if not scr_outputed:
+                #if not "key" in locals():
+                LISHIS = " ".join(  list(histograms.keys())  )
+                LISHIS = f"HISTOGRAMS: {fg.orange}{LISHIS}{fg.default}"
+                print(f"i... {fg.magenta}{dt.datetime.now().strftime('%H:%M:%S.%f')[:10]}{fg.default}  {LISHIS}      ",    end = "\r")
+                #else:
+                #    print(f"i... {fg.magenta}{dt.datetime.now().strftime('%H:%M:%S.%f')[:10]}{fg.default} >  {key}   ",    end = "\r")
             #if rate>0: # DONT SEND in the beginning (what about LARGE values?)
             #    if runtime.total_seconds()>1:
             #        msg = compose_udp( spectrumname, rate )
             #        udpsend( msg )
 
 
 
@@ -797,18 +803,22 @@
             if len(arg)>0:
                 eline = None # energy of the line
                 bline = None # bin of the line
                 dbline = 1
                 if len(arg.split())<1:
                     print(f"X... {fg.red} give me {bg.white}'c  ene bin'{bg.default} OR 'c  reset' ==  'c r'{fg.default}")
                     # break
+                # --------------------- APPLY TO HISTOGRAM ---------------------
                 elif arg.split()[0] in histograms.keys():  # ** APPLY FOR HISTO **
                     print("D... Aplly calib for histogram", arg.split()[0])
-                    LOCAL_GLOB_NONE_CALIB == 0
-                    binmax =  histograms[arg.split()[0]].GetXaxis().GetXmax()
+                    if ECALIBa==1 and ECALIBb==0:
+                        LOCAL_GLOB_NONE_CALIB =2
+                    else:
+                        LOCAL_GLOB_NONE_CALIB = 0
+                    binmax =  histograms[arg.split()[0]].GetXaxis().GetNbins()
                     limits_calib = 0*ECALIBa + ECALIBb,binmax*ECALIBa + ECALIBb
                     histograms[arg.split()[0]].GetXaxis().SetLimits( limits_calib[0],limits_calib[1] )
 
                 elif arg.split()[0]=="reset" or arg.split()[0]=="r" :  # ** reset **
                     ECALIB = []
                     ECALIBa = 1
                     ECALIBb = 0
@@ -835,15 +845,15 @@
                     elif arg.split()[0].upper() == "F":
                         print("i... search in database:")
                         eline = 0
                         deline = 0
                         if "channel" in last_fit_res:
                             eline = last_fit_res["E"]
                             deline = last_fit_res["dE"]
-                            deline = 3*deline # 3sigma
+                            deline = 3*deline + 0.15 # 3sigma PLUS systematic 0.15
                             print(f"i... LAST FITTED PEAK ENE = {eline:.2f} +- {deline:.2f}")
                         if len(arg.split())>1 and  is_float(arg.split()[1]):
                             deline = float(arg.split()[1])
                             print(f"i... LAST FITTED PEAK ENE = {eline:.2f} +- {deline:.2f}")
 
                         if eline !=0:
                             decay_candidates( eline, deline*3 )#deline*3 )
@@ -1494,20 +1504,27 @@
         # ********************** CMD ***********************************
         elif  cmd == "l":  # ***CMD***  LOAD ====== l
             if arg=="":
                 select_histo_to_load(  folder = config.CONFIG[target]['data_folder'] ) # load_txt()
                 print(f"i.. {fg.cyan} LOAD TXT WITH NUMBER like:    l1  l2 l3 ...  {fg.default}")
             else:
                 ii = arg# for ii in arg: ONE ASC / SPECTRUM AT A TIME....for ii in arg:
-                select_histo_to_load( ii , folder = config.CONFIG[target]['data_folder']) # load_txt() # all that are given in argument l67
-                limits_calib = histograms[f"s{ii}"].GetXaxis().GetXmin(),histograms[f"s{ii}"].GetXaxis().GetXmax()
-                print("D... limits calib:", limits_calib)
-                if limits_calib[0]==0:
-                    histograms[f"s{ii}"].SetTitle(  histograms[f"s{ii}"].GetTitle()+"; channels" )
-
+                details = select_histo_to_load( ii , folder = config.CONFIG[target]['data_folder']) # load_txt() # all that are given in argument l67
+                if details is not None:
+                    limits_calib = histograms[f"s{ii}"].GetXaxis().GetXmin(),histograms[f"s{ii}"].GetXaxis().GetXmax()
+                    print("D... limits calib:", limits_calib)
+                    # ONLY AT LOAD TIME I can set Xlabel..... still it is problematic
+                    if limits_calib[0]==0:
+                        histograms[f"s{ii}"].SetTitle(  histograms[f"s{ii}"].GetTitle()+"; channels" )
+                    #print("D... DETAILS=:",details)
+                    rate = details['rate']
+                    runtime = dt.timedelta( seconds = details['totaltime'] )
+                else:
+                    print(f"X... {fg.red} NO FILE LIKE THIS{fg.default}")
+                    limits_calib = None,None
 
         # ********************** CMD ***********************************
         elif cmd == "q":   # ***CMD***  QUIT  ======= q
             print("i... just q: doing exit...")
             # immediate
             config.CONFIG["poll_time"] = 1
             if not OFFLINE:
```

### Comparing `gregory_online-0.3.6/gregory_online/ascgeneric.py` & `gregory_online-0.3.7/gregory_online/ascgeneric.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/config.py` & `gregory_online-0.3.7/gregory_online/config.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/data/Am241.svg` & `gregory_online-0.3.7/gregory_online/data/Am241.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/data/Cm247.png` & `gregory_online-0.3.7/gregory_online/data/Cm247.png`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/data/Np237.svg` & `gregory_online-0.3.7/gregory_online/data/Np237.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/data/Pa231.svg` & `gregory_online-0.3.7/gregory_online/data/Pa231.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/data/Pu239.svg` & `gregory_online-0.3.7/gregory_online/data/Pu239.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/data/Th232.svg` & `gregory_online-0.3.7/gregory_online/data/Th232.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/data/U235.svg` & `gregory_online-0.3.7/gregory_online/data/U235.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/data/U238.svg` & `gregory_online-0.3.7/gregory_online/data/U238.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/data/decay_lara.parquet` & `gregory_online-0.3.7/gregory_online/data/decay_lara.parquet`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/data/testrebin.py` & `gregory_online-0.3.7/gregory_online/data/testrebin.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/decay_db.py` & `gregory_online-0.3.7/gregory_online/decay_db.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/dpp2jpg.py` & `gregory_online-0.3.7/gregory_online/dpp2jpg.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/erlang.py` & `gregory_online-0.3.7/gregory_online/erlang.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/fetchnp.py` & `gregory_online-0.3.7/gregory_online/fetchnp.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/histo_analyze.py` & `gregory_online-0.3.7/gregory_online/histo_analyze.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/histo_displ.py` & `gregory_online-0.3.7/gregory_online/histo_displ.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/histo_global_cont.py` & `gregory_online-0.3.7/gregory_online/histo_global_cont.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/histo_io.py` & `gregory_online-0.3.7/gregory_online/histo_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 """
 load and save operations
 * load a textfile with LT A and B given in the filename
 * verify under/overfl bin present
 ____
 * definition of .details file INSIDE save_hist_txt
-* real usage of .details file in     load_hist_txt with load_details
+* real usage of .details file inside     load_hist_txt with load_details
  : these are used in load_hist_txt
  - livetime
  - a
  - b
  - entries
  - rate
 """
@@ -301,26 +301,29 @@
 def present_avadisc( avadisc , bgcolor=f"{bg.yellow}"):
     print()
     col = 0
 
     termsize = os.get_terminal_size()
     maxwid = termsize.columns
     maxname = 0
+
     for ke in sorted(avadisc.keys()):
         if len(avadisc[ke])>maxname:maxname = len(avadisc[ke])
-    maxname+=5
+
+    maxname+=6 # ADD
+
     ncols=int(maxwid/maxname)
     if ncols == 0: ncols =1
     print(maxwid, maxname, ncols )
     for ke in sorted(avadisc.keys()):
         col+=1
         brk = ""
         if col% ncols==0:
             brk = "\n"
-        print( f"  {bgcolor}{fg.black} {ke} {fg.default}{bg.default}  {avadisc[ke]:{maxname}s} ", end=brk)
+        print( f"{bgcolor}{fg.black} {str(ke):>2s} {fg.default}{bg.default} {avadisc[ke]:{maxname-5}s}", end=brk)
     print()
     print()
 
 
 # ================================================ HISTO AND DETAILS ==================
 
 
@@ -329,35 +332,36 @@
     full sequence list,present, load
     """
     f = folder
     if len(f)==0: f = "./"
     if f[-1]!="/": f=f+"/"
 
     avadisc = list_spectra_disc( folder = folder )
-    present_avadisc(avadisc)
     if num is None:
-        return
+        present_avadisc(avadisc)
+        return None
 
     try:
         num = int(num)
     except:
         num = None
         print("X... no spectrum selected")
     if num in avadisc.keys():
-        load_hist_txt( avadisc[num] , f"s{num}" )
-
+        _,details = load_hist_txt( avadisc[num] , f"s{num}" )  # inside select_histo_to_load()
+        return details
 
 # ----------------------------------- loading spectra/histogram
 
 def load_details(fname):   # used in load_hist_txt: where histograms[hname] is created
                            # and rate interpretted
     res = None
     if os.path.exists(fname):
         with open(fname) as f:
             res = f.readlines()
+        # For reasons - every space after 1st one - changed to _
         res = [ (x.strip().split(" ")[0],"_".join(x.strip().split(" ")[1:])) for x in res]
         res = dict(res)
 
         # the following are gonna be converted and cause a crash if error
         res["totaltime"] = float(res["totaltime"]) # not always needed?
         # not floatres["started"] = float(res["started"]) # not always needed
         res["livetime"] = float(res["livetime"])
@@ -393,37 +397,23 @@
     # I use pandas as in pr_load.py ...
     #avadisc = list_spectra_disc()
     #present_avadisc(avadisc)
 
     hfilename = os.path.splitext(filename)[0]+".txt"
     dfilename = os.path.splitext(filename)[0]+".details"
     details = True
+    res = None
+
     if filename.find("http://")==0:
         dfilename = ascgeneric.get_ini_copy( dfilename )
-        res = load_details(  dfilename )
-        if res is None: details = False
-    else:
-        res = load_details(  dfilename )
-        if res is None: details = False
-
-    # #hole = os.path.splitext(filename)[0]
-    # if not os.path.exists(filename):
-    #     print("X... no file ", filename, end=" ...")
-    #     if os.path.exists(hole+".txt"):
-    #         filename = hole+".txt"
-    #         print("i... replacing with ", filename)
-    #     else:
-    #         print("X... no file ", filename)
-    #         return None
+    res = load_details(  dfilename )
+    if res is None: details = False
 
-    # res = load_details( hole+".details")
-    # details = True
-    # if res is None: details = False
 
-    print("D... histo-txt:", hfilename )
+    print("D... histo-txt:    ", hfilename )
     df = pd.read_csv(hfilename, delimiter=r"\s+", header=None, comment="#", nrows=2)
     ncols = df.shape[1]
     print(f"D... file {hfilename} with {ncols} columns, details found = {details}")
 
     np_c = None
     np_e = None # for rate into th1f
 
@@ -438,33 +428,48 @@
         np_e = df['err'].values
 
         # print( type(np_c), type(np_e), np_c)
         # df.to_csv("zest.txt", sep=' ', header = None)
 
 
     spe = np_c # ================= taking content
-    pure2n = ispure2n( len(spe) )
+    pure2n = ispure2n( len(spe) , silent = True)
     isunovf = ispure2n( len(spe)-2, silent = True )
     if pure2n:
-        print("i... ...  seems no under/overflow bins in the file")
+        print(f"i... ...  seems {fg.green}no under/overflow {fg.default} bins in the file")
+
+    # --------------------------------------find and compare start time
+    starttag = None
+    nounderdate = dt.datetime.strptime("2023-06-01","%Y-%m-%d")
+
+    if "." in res['started']:  # fractions seconds  ...  every " " changed to "_" in res
+        #print(res['started'])
+        starttag = dt.datetime.strptime(res['started'],"%Y-%m-%d_%H:%M:%S.%f")
+    else:
+        starttag = dt.datetime.strptime(res['started'],"%Y-%m-%d_%H:%M:%S")
+
+    if (starttag-nounderdate).total_seconds()<0:
+        #print(res['started'])
+        print(f"X... {fg.red} DATA before 2023/06/01 .... verify for the  underflow  {fg.default}")
+
 
     # ------------------------------------------ this part is tricky, FOR UND OVF LOAD
-    if underoverflow: print("I... supposing the UND/OVER FLOW bins are already present!!")
+    if underoverflow: print(f"I... {fg.red}supposing the UND/OVER FLOW bins are already present!!{fg.default}")
     if underoverflow and isunovf:
-        print("D... Under/overflow bins detected and loading")
+        print(f"D... {fg.red}Under/overflow bins detected and loading{fg.default}")
     if not(underoverflow) and isunovf:
         print(f"X... {fg.red} Under/overflow bins DETECTED but NOT loading {fg.default}")
     #
     if underoverflow and  pure2n:
         print(f"X... {fg.red} PROBLEM - file is 2^n but loading w U/OVF {fg.default}")
     if (not underoverflow) and  (not pure2n):
         print(f"X... {fg.red} PROBLEM - file is NOT 2^n but loading wout U/OVF {fg.default}")
     # ------------------------------------------ this part was tricky, FOR UND OVF LOAD
 
-    if not underoverflow:
+    if not underoverflow: # ADD ARTIFICIALLY
         print("D... adding artificially undeflow/overflow bins...")
         np_c = np.concatenate(([0],np_c,[0]))
         if np_e is not None:
             np_e = np.concatenate(([0],np_e,[0]))
     else:
         print("D... underflow/overflow bits (must be) already present in source file")
 
@@ -483,27 +488,33 @@
     #print( res["a"] )
     #print( float(res["a"])*(len(h1np_backg)-2) )
     #print( res["b"]  )
 
     #  create a normalized histo in the histograms[]
     fill_h_with_np( h1np_backg, hname,
                                  runtime = res["livetime"], errors = np_e,
-                                 limits_calib=[res["b"], res["a"]*(len(h1np_backg)-2)+res["b"] ]
+                    # I assume here udenr overflow !!!
+                                 #limits_calib=[res["b"], res["a"]*(len(h1np_backg)-2)+res["b"] ]
+                                 limits_calib=[res["b"], res["a"]*(len(h1np_backg) )+res["b"] ]
     )
+
     histograms[hname].SetEntries( res["entries"] )
     histograms[hname].SetTitle(  os.path.basename(hfilename) )
     histograms[hname].Print()
     print(f" ... Name= {histograms[hname].GetName()}  Title={histograms[hname].GetTitle()}" )
 
-    if not underoverflow:
-        # artificialy added unovf, removing again
-        return h1np_backg[1:-1]
-    else:
-        # already present in spe
-        return h1np_backg[1:-1]
+    # if not underoverflow:
+    #     # I did artificially add a second ago - to comply with fill_h_with_np!
+    #     # artificialy added unovf, removing again
+    #     return h1np_backg[1:-1], res
+    # else:
+    #     # already present in spe
+
+    # ANYCASE- I STRIP BACK UNDEROVER  + details==res
+    return h1np_backg[1:-1], res
 
 
 
 
     # grp = re.search(r'[\w\d]+_lt([\d\.]+)_a([\d\.]+)_b([\-\d\.]+)\.txt',filename)
     # print(f"D... histo decoded  lt,a,b={fg.green} {grp.groups()} {fg.default}")
     # h1np_backg_lt = float(grp.groups()[0])
@@ -570,15 +581,15 @@
 
 
 
 def main():# fname, hname):
     """
     I can load txt file when lt a b  are in the filename...
     """
-    #load_hist_txt(fname, hname)
+
     select_histo_to_load()
     ROOT.gDirectory.ls()
 
     for i in histograms.keys():
         # histograms[i].Draw()
         hnp,enp = get_np_from_h(histograms[i] )
         # this is in h already...
```

### Comparing `gregory_online-0.3.6/gregory_online/histo_np_ops.py` & `gregory_online-0.3.7/gregory_online/histo_np_ops.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/key_enter.py` & `gregory_online-0.3.7/gregory_online/key_enter.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/topbar.py` & `gregory_online-0.3.7/gregory_online/topbar.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online/utils.py` & `gregory_online-0.3.7/gregory_online/utils.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/gregory_online.egg-info/PKG-INFO` & `gregory_online-0.3.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: gregory-online
-Version: 0.3.6
+Name: gregory_online
+Version: 0.3.7
 Summary: Online watching HTTP server of ROOT on port 9009
+Home-page: UNKNOWN
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Project gregory~online~
 =======================
 
 *experimental code to online survey root spectra from THTTPServer*
 
@@ -77,7 +79,9 @@
   mock~server~.py         
   rebin.py                
   setup.py                
   topbar.py               
   utilone.py              
   version.py              
   ----------------------- ------------------------------
+
+
```

### Comparing `gregory_online-0.3.6/gregory_online.egg-info/SOURCES.txt` & `gregory_online-0.3.7/gregory_online.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.6/setup.py` & `gregory_online-0.3.7/setup.py`

 * *Files identical despite different names*

