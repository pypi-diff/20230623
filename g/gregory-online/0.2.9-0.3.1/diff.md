# Comparing `tmp/gregory_online-0.2.9.tar.gz` & `tmp/gregory_online-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gregory_online-0.2.9.tar", last modified: Fri Jun  9 15:16:54 2023, max compression
+gzip compressed data, was "gregory_online-0.3.1.tar", last modified: Fri Jun 23 11:58:17 2023, max compression
```

## Comparing `gregory_online-0.2.9.tar` & `gregory_online-0.3.1.tar`

### file list

```diff
@@ -1,39 +1,42 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-09 15:16:54.394400 gregory_online-0.2.9/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-09 15:16:54.394400 gregory_online-0.2.9/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-09 15:16:51.000000 gregory_online-0.2.9/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-09 15:16:54.390401 gregory_online-0.2.9/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    54874 2023-06-09 15:15:39.000000 gregory_online-0.2.9/bin/gregory_online
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-09 15:16:54.394400 gregory_online-0.2.9/gregory_online/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/__init__.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     6435 2023-03-17 17:33:40.000000 gregory_online-0.2.9/gregory_online/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-09 15:16:54.394400 gregory_online-0.2.9/gregory_online/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    56290 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/Am241.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   503044 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/Cm247.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    53304 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/Np237.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    79580 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/Pa231.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    93285 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/Pu239.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59999 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/Th232.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    78694 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/U235.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    97718 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/data/U238.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   123572 2023-06-09 11:53:23.000000 gregory_online-0.2.9/gregory_online/data/decay_lara.parquet
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1139 2022-12-08 12:00:24.000000 gregory_online-0.2.9/gregory_online/data/testrebin.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3764 2023-06-09 14:40:20.000000 gregory_online-0.2.9/gregory_online/decay_db.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12625 2023-06-09 14:56:20.000000 gregory_online-0.2.9/gregory_online/fetchnp.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4527 2023-04-20 14:10:17.000000 gregory_online-0.2.9/gregory_online/histo_analyze.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3957 2023-06-02 15:39:44.000000 gregory_online-0.2.9/gregory_online/histo_displ.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      833 2023-06-06 11:16:18.000000 gregory_online-0.2.9/gregory_online/histo_global_cont.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    13381 2023-05-31 13:39:18.000000 gregory_online-0.2.9/gregory_online/histo_io.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-06-05 13:29:49.000000 gregory_online-0.2.9/gregory_online/histo_np_ops.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-20 14:10:17.000000 gregory_online-0.2.9/gregory_online/key_enter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2549 2023-04-20 14:10:17.000000 gregory_online-0.2.9/gregory_online/topbar.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2022-09-16 15:11:00.000000 gregory_online-0.2.9/gregory_online/utilone.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3293 2023-06-09 14:10:12.000000 gregory_online-0.2.9/gregory_online/utils.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-09 15:16:54.000000 gregory_online-0.2.9/gregory_online/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-09 15:16:54.394400 gregory_online-0.2.9/gregory_online.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1814 2023-06-09 15:16:54.000000 gregory_online-0.2.9/gregory_online.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      926 2023-06-09 15:16:54.000000 gregory_online-0.2.9/gregory_online.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-09 15:16:54.000000 gregory_online-0.2.9/gregory_online.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       80 2023-06-09 15:16:54.000000 gregory_online-0.2.9/gregory_online.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-09 15:16:54.000000 gregory_online-0.2.9/gregory_online.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-09 15:16:54.394400 gregory_online-0.2.9/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1217 2023-06-09 15:16:22.000000 gregory_online-0.2.9/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 11:58:17.371809 gregory_online-0.3.1/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-23 11:58:17.371809 gregory_online-0.3.1/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-02 15:20:26.000000 gregory_online-0.3.1/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 11:58:17.367809 gregory_online-0.3.1/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    69602 2023-06-23 11:58:12.000000 gregory_online-0.3.1/bin/gregory_online
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 11:58:17.367809 gregory_online-0.3.1/gregory_online/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/__init__.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    27793 2023-06-23 07:57:50.000000 gregory_online-0.3.1/gregory_online/ascgeneric.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7269 2023-06-23 07:56:33.000000 gregory_online-0.3.1/gregory_online/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 11:58:17.371809 gregory_online-0.3.1/gregory_online/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    56290 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/Am241.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   503044 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/Cm247.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    53304 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/Np237.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    79580 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/Pa231.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    93285 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/Pu239.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59999 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/Th232.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    78694 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/U235.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    97718 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/U238.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   123572 2023-06-12 07:00:49.000000 gregory_online-0.3.1/gregory_online/data/decay_lara.parquet
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1139 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/testrebin.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3758 2023-06-12 07:00:49.000000 gregory_online-0.3.1/gregory_online/decay_db.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    15128 2023-06-23 07:56:33.000000 gregory_online-0.3.1/gregory_online/dpp2jpg.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3631 2023-06-23 07:56:33.000000 gregory_online-0.3.1/gregory_online/erlang.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12625 2023-06-12 07:00:49.000000 gregory_online-0.3.1/gregory_online/fetchnp.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4543 2023-06-23 07:56:33.000000 gregory_online-0.3.1/gregory_online/histo_analyze.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4169 2023-06-23 07:56:33.000000 gregory_online-0.3.1/gregory_online/histo_displ.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      833 2023-06-12 07:00:49.000000 gregory_online-0.3.1/gregory_online/histo_global_cont.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    19155 2023-06-23 11:14:01.000000 gregory_online-0.3.1/gregory_online/histo_io.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-06-05 13:33:05.000000 gregory_online-0.3.1/gregory_online/histo_np_ops.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-19 12:31:34.000000 gregory_online-0.3.1/gregory_online/key_enter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2594 2023-06-23 07:56:33.000000 gregory_online-0.3.1/gregory_online/topbar.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/utilone.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3293 2023-06-12 07:00:49.000000 gregory_online-0.3.1/gregory_online/utils.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-23 11:58:17.000000 gregory_online-0.3.1/gregory_online/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 11:58:17.367809 gregory_online-0.3.1/gregory_online.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-23 11:58:17.000000 gregory_online-0.3.1/gregory_online.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1006 2023-06-23 11:58:17.000000 gregory_online-0.3.1/gregory_online.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-23 11:58:17.000000 gregory_online-0.3.1/gregory_online.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      116 2023-06-23 11:58:17.000000 gregory_online-0.3.1/gregory_online.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-23 11:58:17.000000 gregory_online-0.3.1/gregory_online.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-23 11:58:17.371809 gregory_online-0.3.1/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1259 2023-06-23 11:13:06.000000 gregory_online-0.3.1/setup.py
```

### Comparing `gregory_online-0.2.9/PKG-INFO` & `gregory_online-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: gregory_online
-Version: 0.2.9
+Version: 0.3.1
 Summary: Online watching HTTP server of ROOT on port 9009
-Home-page: UNKNOWN
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Project gregory~online~
 =======================
 
 *experimental code to online survey root spectra from THTTPServer*
 
@@ -79,9 +77,7 @@
   mock~server~.py         
   rebin.py                
   setup.py                
   topbar.py               
   utilone.py              
   version.py              
   ----------------------- ------------------------------
-
-
```

### Comparing `gregory_online-0.2.9/README.md` & `gregory_online-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/bin/gregory_online` & `gregory_online-0.3.1/bin/gregory_online`

 * *Files 20% similar despite different names*

```diff
@@ -21,24 +21,29 @@
 #from gregory_online import histo_np_ops
 from gregory_online.histo_np_ops import apply_calib, fill_h_with_np
 # CONTAINER:
 from gregory_online.histo_global_cont import histograms
 from gregory_online.histo_global_cont import canvases
 from gregory_online.histo_global_cont import range_and_peaks
 #
+# local calibration: list; a,b, database for fits
 from gregory_online.histo_global_cont import ECALIB, ECALIBa, ECALIBb, ECALIBdb
+#
 from gregory_online.histo_global_cont import last_fit_res # last fit result
 from gregory_online.histo_global_cont import gregory_started, is_zoomed
 # histo content manip
 from  gregory_online.histo_analyze import histo_details, histo_zoomenergy, \
     histo_zoombins, histo_unzoom, histo_area, bin2ene, ene2bin, \
     get_calib_coefs, histo_fit, get_ene_range
 
+
+import gregory_online.histo_io as histo_io
 from  gregory_online.histo_io import save_hist_txt, select_histo_to_load, load_hist_txt
 
+import gregory_online.ascgeneric as ascgeneric  # asc_stat_print - orig.  pd_detect_zeroes
 
 from  gregory_online.histo_displ import display_h_name, display_np, refresh_canvases
 from  gregory_online.decay_db import decay_candidates
 
 
 import threading
 import time
@@ -106,63 +111,22 @@
 deadtavg = [0,0] #  long term dt for histosave # NOT USED
 deadttot = 0
 # global h1np,h1np_diff,h1np_old,h1np_old_age,h1np_substr,h1np_backg,h1np_backg_lt, cala, calb, cala_bg, calb_bg
 
 LOCAL_GLOB_NONE_CALIB = 1 # global normally
 INFLUX = True
 
-
-# def udpsend(message):
-#     """
-#     send to local seread running instance
-#     """
-#     UDP_IP = "127.0.0.1"
-#     UDP_IP = "192.168.250.61"
-#     UDP_IP = config.CONFIG['udp_ip']
-#     UDP_PORT = 8100
-#     MESSAGE = message
-#     try:
-#         sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM) # UDP
-#         sock.sendto(bytes(MESSAGE, "utf-8"), (UDP_IP, UDP_PORT))
-#         print(f"D... {fg.green}UDPsent {MESSAGE}{fg.default}")
-#     except:
-#         print(f"D... {fg.red}NOTsent {MESSAGE}{fg.default}")
-
-
-
-
-
-# # influx prepare
-# def compose_udp( spectrumname, rate, pup=0, region=0, jsonpart=""):
-#     """
-#     get board and channel from spectrumname
-#     """
-#     if jsonpart!="":
-#         print(jsonpart)
-#         return
-
-#     # # # avoid 1st spectrum---------------difference huge
-#     # # if self.first_influx_omit:
-#     # #     self.first_influx_omit = False
-#     # #     return
-
-#     measurement = "hpge"
-#     board   = spectrumname[:2]
-#     channel = int(spectrumname[-2:])
-
-#     #pup = self.h1np_diff[1]/self.SECONDS # chnnel 1 is ZERO CHANNEL
-#     #rate = self.h1np_diff.sum()/self.SECONDS
-#     #reg = self.h1np_diff[:10].sum()/self.SECONDS # region
-
-#     udp_seread =f"gregory_{measurement}: {board} ch{channel} {rate:.3f} {pup:.3f} {region:.3f}"
-
-#     # rate, pup reg: region is  chanels 0-10
-#     # udpsend( udp_seread )
-#     return  udp_seread
-
+ascdf = None # DATAFRAME FOR ASC FILE
+ascdf_chan = None # DATAFRAME FOR ASC FILE
+ascfilename = None # asc filename
+iascfilename = None # ini filename if on http:// and then /tmp
+ascstart = None # ASCIFILE started
+TIMEWIN_US = 0 # Crutial window in ASC erlang analysis - dbl-zero limit
+TRGHOLD = 0
+#======================================== END OF GLOBALS ====================
 
 
 def refresh_canvases():
     """
     unselectively refresh every canvas
     """
     maxc = ROOT.gROOT.GetListOfCanvases().GetEntries()
@@ -172,14 +136,16 @@
         ci.Update()
 
 
 
 
 
 
+def has_numbers(inputString):
+    return any(char.isdigit() for char in inputString)
 
 
 
 
 def time2seconds(TIME, defaulttime = "0:0:10"):
     """
 just convert hand input 1:2:3 to seconds
@@ -240,108 +206,169 @@
     #print( len(a),"X" ,len(b),  f" 6 -->  {6*sca+shi}" )
     #print( len(a),"X" ,len(b),  f" 22 -->  {22*sca+shi}" )
     return spectrumb
 
 
 
 
-def main( timeold = None , debug=False, server = None, histogram = None, polltime = None, OFFLINE = False):
+def main( target = None , timeold = None , debug=False, server = None, histogram = None, polltime = None, OFFLINE = False):
     '''
     Main function of the project
     Config is settled in the beginning
     '''
     #OFFLINE = True
     #online
     #if online:
     #OFFLINE = False
 
     #======== DEFINE THE CONFIG FILE HERE ========
-    print("i... OVERRIDE the CONFIG with")
-    print("i... -s 127.0.0.1 -h b0c01")
+    print("i... OVERRIDE the CONFIG with poll 5 sec.")
+    print("i... -s 127.0.0.1 -h b0c01 -p 5")
     print("i... ")
 
     # ---------------- container stuff
     global histograms, canvases, range_and_peaks
     global gregory_started
     global last_fit_res
     global ECALIB, ECALIBa, ECALIBb # calibrations
     global deadtavg, deadt, deadttot # avg not used; tot from h1np
     global LOCAL_GLOB_NONE_CALIB
     global INFLUX
+    global ascdf, ascfilename, iascfilename, ascstart, ascdf_chan, TIMEWIN_US, TRGHOLD # full file, fnname, channel-cut
     #
     # --------------    other stuff
     #global h1np,h1np_diff,h1np_old,h1np_old_age,h1np_substr,h1np_backg,h1np_backg_lt
     global h1np,h1np_diff,h1np_old,h1np_last_interval,h1np_substr,h1np_backg,h1np_backg_lt, cala, calb, cala_bg, calb_bg
 
+
+    def local_generate_erlangs():
+        erlang2 = ascgeneric.histo_erlang( ascdf_chan ) # nonzero events only
+        histograms['erlang2'] = erlang2
+        display_h_name( 'erlang2' , "c_erlang2" , filled = True, color = 1, simple = True)
+
+        dzeroes = ascgeneric.histo_dzeroes( ascdf_chan )
+        histograms['dzeroes'] = dzeroes
+        dzeroes.SetLineColor(2)
+        #dzeroes.SetFillStyle(3001)
+        #dzeroes.SetFillColor(2)
+        dzeroes.Draw("same")
+        #display_h_name( 'dzeroes' , "c_dzeroes" , filled = False, color = 2, simple = True)
+
+        szeroes = ascgeneric.histo_szeroes( ascdf_chan )
+        histograms['szeroes'] = szeroes
+        szeroes.SetLineColor(3)
+        #szeroes.SetFillStyle(3001)
+        #szeroes.SetFillColor(3)
+        szeroes.Draw("same")
+
+
     cmd = "" # no key command
 
     gregory_started = None # dt.datetime.now()
 
     config.CONFIG['filename'] = "~/.config/gregory_online/cfg.json"
-    config.CONFIG["poll_time"] = 2
+    config.CONFIG["poll_time"] = 3
+    config_version_code = config.CONFIG["version"]
 
 
+    #print(config.CONFIG["version"], config_version_code)
     config.load_config()
+    #print(config.CONFIG["version"],config_version_code)
     config.save_config() # UPDATE WITH THE STUFF HERE ABOVE
-    print(config.CONFIG)
-
-    # if cmd == "usage":
-    #     print(''' ... usage:
-    #     	 _
-    #     ''')
-    #     sys.exit(0)
+    #print(config.CONFIG)
+    #print(config.CONFIG["version"],config_version_code)
 
-    # if cmd == "test":
-    #     print("i... test")
+    if float(config_version_code)>float(config.CONFIG["version"]):
+        print(f"X... OLD CONFIG VERSION ON THE DISK: code={config_version_code} ; file={config.CONFIG['version']}")
+        sys.exit(1)
+
+    if target is None:
+        print(" ... give me the target....")
+        print()
+        selections = []
+        for i in config.CONFIG.keys():
+            if type(config.CONFIG[i]) is dict:
+                selections.append( f"      {i:15s}  {config.CONFIG[i]['description']}")
+
+        from simple_term_menu import TerminalMenu
+        terminal_menu = TerminalMenu( selections )
+        choice_index = terminal_menu.show()
+        target = selections[choice_index].strip().split(" ")[0]
+        print(f"                {bg.cyan}      {target}       {bg.default}")
+
+        #sys.exit(1)
+    elif target not in config.CONFIG:
+        print("X... give me the PROPER  target....")
+        for i in config.CONFIG.keys():
+            if type(config.CONFIG[i]) is dict:
+                print(i, type(config.CONFIG[i]) )
+        sys.exit(1)
+
+
+    # $$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$    CONFIG
+
+    if config.CONFIG[target]['online']:
+        spectrumname = config.CONFIG[target]['spectrum'] # "b0c01"
+        serverc = config.CONFIG[target]['server']  # "192.168.250.60"
+        TITLE = f"GREGORY_ONLINE:  polling the THttpServer on {serverc} port 9009"
+        print(f"{fg.white}")
+        print("_"*(len(TITLE)+22) )
+        print("_"*10, TITLE ,"_"*10)
+        print("_"*(len(TITLE)+22) )
+        print(f"{fg.default}")
+
+    else: # offline
+        spectrumname = None
+        serverc = None
+        INFLUX = False
+        print(f"""
+{fg.white}
+______________________________________________________________
+You are now in {fg.green} OFFLINE {fg.white} mode.
+You can list spectra via '{fg.green}l{fg.white}' or open spectra via '{fg.green}l#{fg.white}'
+                           OR
+list ASC files via '{fg.green}L{fg.white}' or open ASC files via '{fg.green}L#{fg.white}'
+FOLDER:
+{config.CONFIG[target]['data_folder']}
+______________________________________________________________ {fg.default}
 
 
+""")
 
-    spectrumname = config.CONFIG['spectrum'] # "b0c01"
-    serverc = config.CONFIG['server']  # "192.168.250.60"
 
+    # override from cmdline
     if server is not None:
         print("i... SERVER OVERRIDE:", server)
         serverc = server
     if histogram is not None:
         print("i... HISTOGRAM OVERRIDE:", histogram)
         spectrumname = histogram
-
-
-    TITLE = "GREGORY_ONLINE:  pollig the THttpServer on port 9009"
-    print("_"*(len(TITLE)+22) )
-    print("_"*10, TITLE ,"_"*10)
-    print("_"*(len(TITLE)+22) )
-
-
-    # INIT HISOGRAM AND SET STEP, PRESETIME
-
-    b0c01 = fetchnp.Histogram( serverc, spectrumname )
-
-
     if polltime is not None:
         config.CONFIG["poll_time"] = float(polltime)
-    b0c01.set_step( config.CONFIG["poll_time"])
 
 
-    # #   - SET THE RUNTIME ON AGE ??????  AGE will stand only for diffage spectrum
-    # arg = time2seconds(age)
-    # print(f"i... measurement time (current spectrum age) is set to {age} == {arg} s ") #
-    # b0c01.set_runtime( arg)
-    # #time.sleep(1)
-    # -------  timeold will work for server that doesnot use TITLE:  rt=123.4s
-    if timeold is not None:
-        arg = time2seconds(timeold)
-        print(f"i... measurement time (current spectrum age) is set to {timeold} == {arg} s ") #
-        b0c01.set_started_before( arg)
 
-    #OFFLINE = True
-    thr = threading.Thread( target=b0c01.start2collect , args=() )
-    if not OFFLINE:
+    # INIT HISOGRAM AND SET STEP, PRESETIME
+    if config.CONFIG[target]['online']:
+        b0c01 = fetchnp.Histogram( serverc, spectrumname )
+        b0c01.set_step( config.CONFIG["poll_time"])
+
+        # can get spectrum total time on cmdline
+        if timeold is not None:
+            arg = time2seconds(timeold)
+            print(f"i... total time ({spectrumname} age) is set to {timeold} == {arg} s ")
+            b0c01.set_started_before( arg)
+
+        thr = threading.Thread( target=b0c01.start2collect , args=() )
         thr.start()
 
+    else:
+        OFFLINE = True
+        thr = threading.Thread( target=None , args=() )
+
 
     top = topbar.Topbar( bgcolor = bg.blue)
     top2 = top.add(bgcolor = bg.black)
 
     #start the Keyboard thread AFTER TOPBAR
     #print("preparing kthread")
     # kthread = key_enter.KeyboardThread(key_enter.my_callback)
@@ -352,26 +379,21 @@
     #--------- init values for TOP
     deltat = 0
     rate = 0
     runtime = dt.datetime.now()
     runtime = dt.datetime.now() -runtime
     lenhistos = 0
 
-    # ### backg_np = None
-    # h1np = None
-    # h1np_diff = None
-    # h1np_substr = None
-    # h1np_backg = None
     d_last_interval = 0.0
     warn_del = fg.default
     unwarn_del = fg.default
 
     while thr.is_alive() or OFFLINE:
 
-        if  b0c01.fetch_flag():
+        if not OFFLINE and  b0c01.fetch_flag():
             # if fetched - get values ==========================
 
             h1np = b0c01.get_h1np()
             h1np_diff = b0c01.get_h1np_diff()
             deltat = b0c01.get_deltat()
             if runtime>b0c01.get_runtime():
                 deadtavg = [0,0]
@@ -475,15 +497,19 @@
                 # deadt = 0
                 # if  just_spesum !=0:
                 #     # print("D... diff[0]==", h1np_diff[0], h1np_diff[1], len(h1np_diff) )
                 #     deadt = h1np_diff[0]/just_spesum*100
                 if is_float(rate) and is_float(deadt):
                     infvals = f"rate_{spectrumname}={rate:.1f},deadt_{spectrumname}={deadt:.1f}"
                     # print("D...",infvals)
-                    influxwrite("test", f"greg",  infvals ) # hostname added automat
+                    try:
+                        influxwrite("test", f"greg",  infvals ) # hostname added automat
+                    except:
+                        INFLUX = False
+                        pass
 
 
 
 
             # IN ANY CASE... REFRESH ALL CANVASES
             refresh_canvases()
 
@@ -495,29 +521,29 @@
             #     print(f"i... new fetch: rate= {h1np_diff.sum()/deltat:.2f} (dt={deltat:.2f})")
 
             #--------------------------- influx stuff ---------------
 
             scr_outputed = False
             if rate>0:
                 # DONT SEND in the beginning (what about LARGE values?)
-                if runtime.total_seconds()>1:
+                if not OFFLINE and runtime.total_seconds()>1:
                     print(f"i... {fg.green} watchdog {fg.default} T_fetch={1000*b0c01.tcp_fetch_time:.0f}ms           ", end = "\r")
                     scr_outputed = True
 
                     # k40 = 0.
                     # if "last" in histograms:
                     #     histo_zoomenergy( histograms["last"], 1440.0, 1480.0  )
                     #     res = histo_fit( histograms["last"],  canvas = None )# "fitresult")
                     #     if res is not None:
                     #         if "area" in res.keys() and "E" in res.keys():
                     #             k40 = res["area"]
                     # print("test",f"{HOSTNAME}_grg",f"rate={rate:.1f},k40={k40}")
                     # #influxwrite("test",f"{HOSTNAME}_grg",f"rate={rate:.1f},k40={k40}")
 
-            if not scr_outputed: print(f"i... {fg.magenta} {dt.datetime.now()}  {fg.default}            ", end = "\r")
+            if not scr_outputed: print(f"i... {fg.magenta} {dt.datetime.now().strftime('%H:%M:%S.%f')[:10]}  {fg.default}            ", end = "\r")
             #if rate>0: # DONT SEND in the beginning (what about LARGE values?)
             #    if runtime.total_seconds()>1:
             #        msg = compose_udp( spectrumname, rate )
             #        udpsend( msg )
 
 
 
@@ -549,36 +575,46 @@
         if len(cmd.split(" "))>1:
             cmd = key.split()[0]
             #arg = key.split()[-1] # the last? NO. take all
             arg = " ".join(key.split()[1:]) # the last? NO. take all
             if cmd == arg:
                 arg=""
 
+        #
+        # FIRST PROCESSING THE COMMAND
+        #
         # nospace multiletter cmd  d    v q
+        #
+        #
         if (arg=="") and (len(cmd)>0):
             if cmd == "d":
                 #??
                 cmd = "d"  # total is default display
                 arg = "t"  # total is default display
             elif cmd[0] == "d": # for display
-                arg = cmd[0:]
+                arg = cmd[1:].strip()
                 cmd = "d"
             if cmd[0] == "l": # for load
-                arg = cmd[0:]
+                arg = cmd[1:].strip()
                 cmd = "l"
+            if cmd[0] == "L": # for load
+                arg = cmd[1:].strip(" ")
+                cmd = "L"
             print(f"i... cmd = {cmd} arg={arg}")
 
+
         #------------------------------------------COMMANDS
         #------------------------------------------COMMANDS
         #------------------------------------------COMMANDS
         #------------------------------------------COMMANDS
         #------------------------------------------COMMANDS
         #------------------------------------------COMMANDS
         #------------------------------------------COMMANDS
         #------------------------------------------COMMANDS
+        # ********************** CMD ***********************************
         if cmd == "h":     # ***CMD***  HELP =========
             yy=f"{fg.white}"
             ny=f"{fg.default}{bg.default}"
 
             yx=f"{fg.yellow}"
             nx=f"{fg.default}"
 
@@ -592,38 +628,54 @@
  {yy}f{ny} ... fit
  {yy}c{ny} ... calib (energy)
  {yy}i{ny} ... info               {yy}v{ny} ... view histo details
  {yy}u{ny} ... unzoom             {yy}z{ny} ... zoom
  {yy}n{ny} ... next               {yy}p{ny} ... previous
  {yy}w{ny} ... window width
  {yy}s{ny} ... save histogram     {yy}l{ny} ... load histogram
+                                  {yy}L{ny} ... load ascfile
  {yy}d{ny} ... display histo:
     {yx}t{nx} ... tot/total (also if t is omitted)
     {yx}r{nx} ... rat/rates (tot normalized on time)
     {yx}b{nx} ... bac/background  (must be loaded by l)
     {yx}s{nx} ... sub/substracted (rate - backg-rate) rate
     {yx}l{nx} ... last [age] seconds histogram (defined by a)
     {yx}m{nx} ... the few seconds [dt] difference histo
  {yy}q{ny} ... quit
 ----------------
 Histograms:   tot, rat, bac  diff  last  sub
 """)
+            if ascdf is not None:
+                print(f"""
+{yg}L {ng} ... load ASC file
+{yg}# {ng} ... select channel # from ASC (create ASC-chan frame)
+{yg}st{ng} ... stat ... statistics on ASC file
+{yg}sh{ng} ... show ... show a sample of ASC file
+{yg}cu{ng} ... cut ... 'cut from to' - use on ASC-chan frame
+{yg}er{ng} ... erlang ... plot erlang from  ASC-chan frame
+{yg}re{ng} ... reset ... discard current selections = ASC-chan frame
+
+""")
 # diff ... what changed from the last read = last [dt] sec. histo
 # last ... tot - [age] seconds old histo = last [age] sec. histo
 # sub  ... tot - bac (normalized on rate)  ? last - bac ?  ? last - tot ?
 
 # Watchdog: for influx, log etc...
 
+
+        # ********************** CMD ***********************************
         elif cmd == "`":   # ***CMD***  TESTKEY ======
             print(f"i... [ ] {arg}   TEST KEY   ")
             if len(arg)>0:
                 thisname = arg.split()[0]
                 if thisname in histograms.keys():
                     print("test")
 
+
+        # ********************** CMD ***********************************
         elif cmd == "r":   # ***CMD***  range, pksearch  ======
             range_and_peaks["rng"] = None #spectrum name
             range_and_peaks["spe"] = None #spectrum name
             range_and_peaks["pks"] = None #list np
             print(f"i...  arg=/{arg}/   ... range+pksearch   #canvs=", len(canvases))
             # for i in list(canvases.keys()):
             #     print("i... CANVASES:",i,canvases[i].IsDrawn(),\
@@ -659,14 +711,15 @@
                     range_and_peaks["rng"] = get_ene_range(histograms[thisname])
                     range_and_peaks["spe"] = thisname
                     range_and_peaks["pks"] = xvecso
                     #print("i... ", len(xvecso), f" {thisname}:",xvecso)
                     print( f"i... {fg.green}OK{fg.default}",range_and_peaks )
 
 
+        # ********************** CMD ***********************************
         elif cmd == "R":  # ***CMD***  Record Range to DISK  ======
             print(f"i...  arg=/{arg}/   ... Range save to file")
             RAP = False
             if type(range_and_peaks) is not None and \
                "rng" in range_and_peaks and \
                "spe" in range_and_peaks and \
                "pks" in range_and_peaks:
@@ -681,14 +734,15 @@
                 # save comma separated
                 with open("ranges.txt","a+",newline='') as f:
                     f.write( f"{range_and_peaks['spe']}, {','.join([str(round(x,2)) for x in range_and_peaks['rng']])}, {','.join([str(round(x,2)) for x in range_and_peaks['pks']])}"+"\n" )
                 print(f"i... {bg.green}SAVED{bg.default} to ...  ranges.txt")
             else:
                 print(f"i... {fg.red} range and peaks not recorded to disk {fg.default}")
 
+        # ********************** CMD ***********************************
         elif cmd == "f":   # ***CMD***  FIT  ======
             RAP = False
             if "rng" in range_and_peaks and \
                "spe" in range_and_peaks and \
                "pks" in range_and_peaks and \
                type(range_and_peaks["pks"]) is list and\
                len(range_and_peaks["pks"])>0:
@@ -715,162 +769,183 @@
                             if i.find("area")>=0: print( f"          {i:10s} {res[i]:.4f} ")
 
                         # test to database - not here
                         #if "E" in res:
                         #    decay_candidates( res["E"] )
 
 
+        # ********************** CMD ***********************************
         elif cmd == "c":   # ***CMD***  CALIB =======
-            print(f"i... c: {arg}       datalen= {len(ECALIB)} _______________________" )
-            print("i...    c Ene     channel")
-            print("i...    c Isotope channel")
-            print("i...    c [Isotope|Ene]   f    ... for fit result as the bin")
-            print("i...    c r  ....  reset calibration data")
-            print("i...    c l  ....  override calibration to LOCAL")
-            print("i...    c g  ....  override calibration to GLOBAL")
-            print("i...    c n  ....  override calibration to NONE")
-            print("i...    c f  ....   search database for last fit E")
-            print("i...    c f de ....  search database for last fit E with dE")
-            for ik in ECALIBdb.keys():
-                print(f"i...         | {ik:7s} | {ECALIBdb[ik]:8.2f} |")
-            print( "             _________________________________")
+            print(f"i...    c: {arg}              datalen= {len(ECALIB)} _______________________" )
+            if len(arg)==0:
+                print(f"i...    {fg.yellow}c Ene     channel {fg.default}")
+                print(f"i...    {fg.yellow}c Isotope channel {fg.default}")
+                print(f"i...    {fg.yellow}c [Isotope|Ene]  f {fg.default}   ... for fit result as the bin")
+                print(f"i...    {fg.yellow}c r   {fg.default} ....  reset calibration data")
+                print(f"i...    {fg.yellow}c l   {fg.default} ....  override calibration to LOCAL")
+                print(f"i...    {fg.yellow}c g   {fg.default} ....  override calibration to GLOBAL")
+                print(f"i...    {fg.yellow}c n   {fg.default} ....  override calibration to NONE")
+                print(f"i...    {fg.yellow}c f   {fg.default} ....  search database for last fit E")
+                print(f"i...    {fg.yellow}c f de{fg.default} ....  same search  with defined dE")
+                for ik in ECALIBdb.keys():
+                    print(f"i...         | {ik:7s} | {ECALIBdb[ik]:8.2f} |")
+                print( "             _________________________________")
 
             if len(arg)>0:
                 eline = None # energy of the line
                 bline = None # bin of the line
                 dbline = 1
                 if len(arg.split())<1:
                     print(f"X... {fg.red} give me {bg.white}'c  ene bin'{bg.default} OR 'c  reset' ==  'c r'{fg.default}")
                     # break
                 elif arg.split()[0]=="reset" or arg.split()[0]=="r" :  # ** reset **
                     ECALIB = []
                     ECALIBa = 1
                     ECALIBb = 0
-                    print("i... {fg.yellow} RESET! e-calibration done{fg.default} ")
+                    print(f"i... {fg.yellow} RESET! e-calibration done{fg.default} ")
                 elif arg.split()[0]=="local" or arg.split()[0]=="l" :  # **
                     LOCAL_GLOB_NONE_CALIB = 0
-                    print("i... {fg.yellow} LOCAL! e-calibration NOW{fg.default} ")
+                    print(f"i... {fg.yellow} LOCAL! e-calibration NOW{fg.default} ")
                 elif arg.split()[0]=="global" or arg.split()[0]=="g" :  # **
                     LOCAL_GLOB_NONE_CALIB = 1
-                    print("i... {fg.yellow} GLOBAL! e-calibration NOW{fg.default} ")
+                    print(f"i... {fg.yellow} GLOBAL! e-calibration NOW{fg.default} ")
                 elif arg.split()[0]=="none" or arg.split()[0]=="n" :  # **
                     LOCAL_GLOB_NONE_CALIB = 2
-                    print("i... {fg.yellow} NONE! e-calibration NOW{fg.default} ")
+                    print(f"i... {fg.yellow} NONE! e-calibration NOW{fg.default} ")
 
                 # decompose the arguments....
                 else:
                     ok = True
                     eline, bline = None,None
                     if is_float(arg.split()[0]):   # ** energy was given **
                         eline = float(arg.split()[0])
                     elif arg.split()[0].upper() in ECALIBdb.keys(): #** 40K was given **
                         eline = ECALIBdb[arg.split()[0].upper()]
 
                     elif arg.split()[0].upper() == "F":
                         print("i... search in database:")
+                        eline = 0
+                        deline = 0
                         if "channel" in last_fit_res:
                             eline = last_fit_res["E"]
                             deline = last_fit_res["dE"]
                             deline = 3*deline # 3sigma
                             print(f"i... LAST FITTED PEAK ENE = {eline:.2f} +- {deline:.2f}")
                         if len(arg.split())>1 and  is_float(arg.split()[1]):
                             deline = float(arg.split()[1])
                             print(f"i... LAST FITTED PEAK ENE = {eline:.2f} +- {deline:.2f}")
 
-                        decay_candidates( eline, deline*3 )#deline*3 )
+                        if eline !=0:
+                            decay_candidates( eline, deline*3 )#deline*3 )
+                        else:
+                            print("X... you may not did the fit first....")
                         ok = False
 
                     else: # ** something else happened**
                         print("X... problem if not float nor in LIST",arg.split() )
                         ok = False
                     #print(f"D... ... eline {eline}")
 
+
                     #print(arg.split(), arg.split()[1], is_float(arg.split()[1]))
                     # BIN to be decoded
                     if len(arg.split())>1 and is_float(arg.split()[1]):   # ** bin **
                         bline = float(arg.split()[1])
                         #print(f"D... bline={bline}")
-                    # taking from fit....
+                    # taking from fit.... SECOND F
                     elif len(arg.split())>1 and arg.split()[1]=="f":      # ** f=fitted bin **
                         if "channel" in last_fit_res:
                             bline = last_fit_res["channel"]
                             dbline = last_fit_res["dchannel"]
                             print("i... GETTING LAST FITTED PEAK for calibration bin", bline)
                         else:
                             ok = False
                             print("X... no fit result stored to get bin from there...")
                     else:
-                        print("X... some problem, bin not given (nor 'f') ")
+                        #print("X... some problem, bin not given (nor 'f') ")
                         ok = False
+
+
                     if ok:
                         ECALIB.append( [ eline, bline, dbline ] ) # energy, channel, dchannel
                         print(ECALIB)
             ECALIBa, ECALIBb = ecalibration(ECALIB)
             print(f"i...  calculated energy calibration is {fg.green} E = {ECALIBa:.6f}*k + {ECALIBb:.3f} {fg.default}")
-            print(f"i... {fg.blue} REMEMBER!: spectra energy calibration comes from detector (for now)...  {fg.default}")
+            #print(f"i... {fg.blue} REMEMBER!: spectra energy calibration comes from detector (for now)...  {fg.default}")
             print(ECALIB)
 
 
+        # ********************** CMD ***********************************
         elif cmd == "i":   # ***CMD***  INFO =======
             print(f"i... i: {arg}    ")
+            #if len(arg) == 0:
+            print(f"D...  ... POSSIBLE keys: {histograms.keys()}")
             if len(arg)==0 and len(canvases)>=1:
                 arg = list(canvases.keys())[0].split("c_")[-1]
                 print("i... generated name for spectrum = ", arg)
             if len(arg)>0 and arg in histograms.keys():
                 tarea = histo_area(  histograms[arg] )
                 # when zoom:
                 binlo = histograms[arg].GetXaxis().GetFirst()
                 binhi = histograms[arg].GetXaxis().GetLast()
                 elo = bin2ene(binlo, histograms[arg])
                 ehi = bin2ene(binhi, histograms[arg])
                 zarea = histo_area(  histograms[arg] ,elo , ehi)
+                started = "not done yet for offline"
+                if "b0c01" in locals():
+                    started = b0c01.started
                 print(f"""
 ___________________________________________________________________
        Name  = {arg}                           i need to redo this
        Lenght= {len(histograms[arg])}
        Time  = {runtime}  (runtime)
-     Started = {b0c01.started} (server histogram -  b0c01 started)
+     Started = {started}
     TotalArea= {tarea:16.6f}
     ZoomeArea= {zarea:16.6f}
-        zoom = {elo} ... {ehi} (Energy)
+        zoom = {elo:.1f} ... {ehi:.1f} (Energy)
         zoom = {binlo} ... {binhi} (bins)
 
 """)
 
 
+        # ********************** CMD ***********************************
         elif cmd == "u":   # ***CMD***  UNZOOM =======
             print(f"i... u pressed ... unzoom:  {arg}    ")
             #print( list(canvases.keys() ) )
             if "is_zoomed" in locals() and is_zoomed[0]:
                 low,hi = None,None
                 if len(arg)==0 and len(canvases)>=1:
                     frhis = list(canvases.keys())[0].split("c_")[-1]
                     low = histograms[frhis].GetXaxis().GetFirst()
                     hi  = histograms[frhis].GetXaxis().GetLast()
 
                     low = histograms[frhis].GetXaxis().GetBinCenter(low)
                     hi  = histograms[frhis].GetXaxis().GetBinCenter(hi)
 
                     delt = hi-low
-                    if delt<2000:
-                        print(f"i... delta is {delt},     low {low}   high {hi}    {frhis[0]}" )
-                        low = low - delt
-                        hi = hi + delt
-                        print(f"i... delta is {delt}, new low {low}  new high {hi}" )
+                    if delt<4000:
+                        print(f"i... delta is {delt:.1f},     low {low:.1f}   high {hi:.1f}  USING:{frhis}" )
+                        if low - 0.2*delt<0:
+                            low = 0 # low - 0.3*delt
+                        else:
+                            low = low - 0.2*delt
+                        hi = hi + 0.2*delt
+                        print(f"i... delta is {delt:.1f}, new low {low:.1f}  new high {hi:.1f}" )
                         for i in histograms.keys():
                             histo_zoomenergy( histograms[i] ,
                                             int(low),   int(hi) )
                     else:
                         for i in histograms.keys():
                             histo_unzoom( histograms[i] )
                         is_zoomed =[ False, 0 ]
 
 
 
 
+        # ********************** CMD ***********************************
         elif cmd == "n":   # ***CMD***  NEXT ZOOM =======uses window
             print(f"i... n pressed ... nexzoom: arg=/{arg}/   allcanvases   ")
             low,hi = None,None
             if len(arg)==0 and len(canvases)>=1: # ANY # OF CANVASES
                 arg = list(canvases.keys())[0].split("c_")[-1]
             if len(arg)>0:
             #if len(histograms)>0:
@@ -879,29 +954,30 @@
                 low = histograms[frhis].GetXaxis().GetFirst()
                 hi  = histograms[frhis].GetXaxis().GetLast()
                 # this returns energy
                 low = histograms[frhis].GetXaxis().GetBinCenter(low)
                 hi  = histograms[frhis].GetXaxis().GetBinCenter(hi)
 
                 delt = hi-low
-                print(f"i... delta is {delt},     low {low}   high {hi}    {frhis[0]}" )
+                print(f"i... delta is {delt:.1f},     low {low:.1f}   high {hi:.1f}    {frhis[0]}" )
 
-                low = hi - 0.3*delt
-                hi = hi + delt - 0.3*delt
-                print(f"i... delta is {delt}, new low {low}  new high {hi}" )
+                low = hi - 0.2*delt
+                hi = hi + delt - 0.2*delt
+                print(f"i... delta is {delt:.1f}, new low {low:.1f}  new high {hi:.1f}" )
                 is_zoomed =[ True, (low+hi)/2 ]
                 print(is_zoomed)
                 for i in histograms.keys():
                     histo_zoomenergy( histograms[i] ,
                                     low,   hi )
                     #histo_zoombins( histograms[i] ,
                     #                int(low),   int(hi) )
 
+        # ********************** CMD ***********************************
         elif cmd == "p":   # ***CMD***  PREV ZOOM =======uses window
-            print(f"i... n pressed ... nexzoom: arg=/{arg}/   allcanvases   ")
+            print(f"i... p pressed ... nexzoom: arg=/{arg}/   allcanvases   ")
             low,hi = None,None
             if len(arg)==0 and len(canvases)>=1: # ANY # OF CANVASES
                 arg = list(canvases.keys())[0].split("c_")[-1]
             if len(arg)>0:
             #if len(histograms)>0:
                 #frhis = list(histograms.keys())
                 frhis = list(canvases.keys())[0].split("c_")[-1]
@@ -911,29 +987,30 @@
                 hi  = histograms[frhis].GetXaxis().GetLast()
 
                 # this returns energy
                 low = histograms[frhis].GetXaxis().GetBinCenter(low)
                 hi  = histograms[frhis].GetXaxis().GetBinCenter(hi)
 
                 delt = hi-low
-                print(f"i... delta is {delt},     low {low}   high {hi}    {frhis[0]}" )
+                print(f"i... delta is {delt:.1f},     low {low:.1f}   high {hi:.1f}    {frhis[0]}" )
 
-                low = low - delt + 0.3*delt
-                hi = hi - delt + 0.3*delt
-                print(f"i... delta is {delt}, new low {low}  new high {hi}" )
+                low = low - delt + 0.2*delt
+                hi = hi - delt + 0.2*delt
+                print(f"i... delta is {delt:.1f}, new low {low:.1f}  new high {hi:.1f}" )
                 is_zoomed =[ True, (low+hi)/2 ]
                 print(is_zoomed)
                 for i in histograms.keys():
                     histo_zoomenergy( histograms[i] ,
                                     low,   hi )
                     #histo_zoombins( histograms[i] ,
                     #                int(low),   int(hi) )
 
 
 
+        # ********************** CMD ***********************************
         elif cmd == "z":   # ***CMD***  ZOOM =======uses window
             print(f"i... z pressed ... zoom: arg=/{arg}/  allcanvases   ")
             #print( list(canvases.keys() ) )
             if len(arg)>0:
                 middle = None
                 try:
                     middle = float(arg.split()[0])
@@ -941,33 +1018,53 @@
                     print("X... zoom's  energy is not float")
                 if middle is not None:
                     is_zoomed =[ True, middle ]
                     for i in histograms.keys():
                         histo_zoomenergy( histograms[i] ,
                                       is_zoomed[1] - config.CONFIG["window"]/2,
                                       is_zoomed[1] + config.CONFIG["window"]/2 )
-            elif "is_zoomed" in locals() and is_zoomed[0]:
-                config.CONFIG["window"] = config.CONFIG["window"]/2
-                for i in histograms.keys():
-                    histo_zoomenergy( histograms[i] ,
-                                      is_zoomed[1] - config.CONFIG["window"]/2,
-                                      is_zoomed[1] + config.CONFIG["window"]/2 )
-
+            # elif "is_zoomed" in locals() and is_zoomed[0]:
+            #     config.CONFIG["window"] = config.CONFIG["window"]/2
+            #     for i in histograms.keys():
+            #         histo_zoomenergy( histograms[i] ,
+            #                           is_zoomed[1] - config.CONFIG["window"]/2,
+            #                           is_zoomed[1] + config.CONFIG["window"]/2 )
+            elif len(arg)==0 and len(canvases)>=1: # ANY # OF CANVASES
+                arg = list(canvases.keys())[0].split("c_")[-1]
+                if len(arg)>0:
+                    frhis = list(canvases.keys())[0].split("c_")[-1]
+                    # this returns bins it seems. I need to return energy
+                    low = histograms[frhis].GetXaxis().GetFirst()
+                    hi  = histograms[frhis].GetXaxis().GetLast()
+                    # this returns energy
+                    low = histograms[frhis].GetXaxis().GetBinCenter(low)
+                    hi  = histograms[frhis].GetXaxis().GetBinCenter(hi)
+                    delt = hi-low
+                    print(f"i... delta is {delt:.1f},     low {low:.1f}   high {hi:.1f}    {frhis[0]}" )
+                    low = low +  0.2*delt
+                    hi = hi -  0.2*delt
+                    print(f"i... delta is {delt:.1f}, new low {low:.1f}  new high {hi:.1f}" )
+                    is_zoomed =[ True, (low+hi)/2 ]
+                    print(is_zoomed)
+                    for i in histograms.keys():
+                        histo_zoomenergy( histograms[i] ,
+                                    low,   hi )
 
 
             #     thisname = arg.split()[0]
             #     if thisname in histograms.keys():
             #         try:
             #             fr,to = float(arg.split()[1]),float(arg.split()[2])
             #             print("i... zooming", thisname, histograms[thisname],f"range = {fr} ... {to} (energy)")
             #             histo_zoomenergy( histograms[thisname] , fr, to )
             #             print(f" ...  retains only when {thisname} was drawn")
             #         except:
             #             print(f"{fg.red}X... zoom problem{fg.default}")
 
+        # ********************** CMD ***********************************
         elif cmd == "w":   # ***CMD***  W? ======== set window like 10kev
             if "is_zoomed" in locals() and is_zoomed[0]:
                 print("i... w pressed ... window width ... like 10 (in keV).../",is_zoomed)
                 if len(arg)>0:
                     print(f"i... interpreting argument {arg}")
                     window = config.CONFIG["window"]
                     try:
@@ -980,14 +1077,15 @@
                     except:
                         print("X... float expected, not given in", arg)
                     config.CONFIG["window"] = window
             else:
                 print("X... is_zoomed must be initialized by zooming")
 
 
+        # ********************** CMD ***********************************
         elif  cmd == "v":  # ***CMD***  ViewDetails ==== v view details
             #
             if "tot" in histograms:
                 # Started = {gregory_started} (server histogram - greg started)
                 cala, calb = get_calib_coefs( histograms["tot"] )
                 area = histo_area( histograms["tot"] )
                 print(f"""
@@ -1006,57 +1104,74 @@
             else:
                 print("X...   'tot' not in histograms; offline mode?")
                 #histo_details( histograms[ spectrumname] )
             print(f"i... canvases  : {list(canvases.keys())}")
             print(f"i... histograms:{list(histograms.keys())}")
 
 
+        # ********************** CMD ***********************************
         elif cmd == "t":   # ***CMD***  TIME ========== t time from start
             if  arg=="":
                 print("i... cmd t needs time from start 3600s 1h 1:00:00")
                 continue
             arg = time2seconds(arg)
             print(f"i... arg: seconds == {arg} ")
             b0c01.set_started_before( arg) # ON "T" time
 
         elif cmd == "s":   # ***CMD*** #============= s save
-            #deadt2 = 0
-            #if deadtavg[1]>0:
-            #    deadt2 = deadtavg[0]/deadtavg[1]
-            print("i... just save total, deadtime = ",deadttot)
-            save_hist_txt( "tot" , total_time = runtime.total_seconds() , started = b0c01.started, deadtime = deadttot/100 )
-            if len(arg)>0:
-                thisname = arg.split()[0]
-                if thisname in histograms.keys():
-                    save_hist_txt( thisname , total_time = runtime.total_seconds() , started = b0c01.started, deadtime = deadttot/100 , errors = True)
-
+            if "b0c01" in locals():
+                #deadt2 = 0
+                #if deadtavg[1]>0:
+                #    deadt2 = deadtavg[0]/deadtavg[1]
+                print("i... just save total, deadtime = ",deadttot)
+                save_hist_txt( "tot" , total_time = runtime.total_seconds() , started = b0c01.started, deadtime = deadttot/100 )
+                if len(arg)>0:
+                    thisname = arg.split()[0]
+                    if thisname in histograms.keys():
+                        save_hist_txt( thisname , total_time = runtime.total_seconds() , started = b0c01.started, deadtime = deadttot/100 , errors = True)
+            else:
+                print("X... You may be in OFFLINE MODE, b0c0 does not exists in this universe")
+                print("X... in  OFFLINE MODE - - use sa filename_without_extension ")
 
+        # ********************** CMD ***********************************
         elif cmd == "a":   # ***CMD***  AGE ========== a age_of_diff histo
             if  arg=="":
                 print("i... cmd a needs time")
                 continue
             arg = time2seconds(arg)
             print(f"i... arg: seconds == {arg} / LAST {arg} seconds histogram ")
             h1np_last_interval = arg
 
 
+        # ********************** CMD ***********************************
         elif cmd == "d":   # ***CMD***  DISPL ============= d
             first_h = True # more histograms on the same canvas
 
             # i blindly try
-            ROOT.gStyle.SetOptStat(1111111) # WORKS
+            ROOT.gStyle.SetOptStat(1111111) # WORKSsp
+
+            print(arg)
+            if has_numbers(arg):
+                arg = arg.split(" ")
+                print(arg)
+                #if len(arg)==1:
+                #    arg = [arg]
+                print(arg)
 
-            for ic in arg: # plot one by one
+            for ic in arg: # plot letter par letter ....... one by one
                 print("   i... interpretting display argument:",ic)
                 if "t" in ic: # TOTAL
-                    display_np( h1np, "tot", "c_tot" , None , limits_calib=limits_calib)
-                    first_h = False
+                    if h1np is not None:
+                        display_np( h1np, "tot", "c_tot" , None , limits_calib=limits_calib)
+                        first_h = False
+                    else:
+                        print(f"X... {fg.red} histogram /tot/ doesnt exist {fg.red} try e.g. l1 ds1? ")
 
                 # fast way to displ hists one by one
-                for ii in range(1,10):
+                for ii in range(1,99):
                     if f"{ii}" in ic: #
                         #display_np( h1np, "s{ii}", "c_s{ii}" , None , limits_calib=limits_calib)
                         display_h_name(f"s{ii}", cname=f"c_s{ii}" , filled = True, color = ii+39)
                         first_h = False
 
 
                 if "r" in ic: # RATE
@@ -1192,74 +1307,206 @@
                 ROOT.gPad.SetGridy()
                 ROOT.gPad.Modified()
                 ROOT.gPad.Update()
 
 
 
 
+        # ********************** CMD *********************************** L
+        elif  cmd == "L":  # ***CMD***  LOAD ASC ====== L but only 1 spectrum
+            if arg=="":
+                histo_io.select_asc_to_load( folder = config.CONFIG[target]['data_folder'] )
+                print(f"i.. {fg.cyan} LOAD ASC WITH NUMBER like:    L1  L2 L3 ...  {fg.default}")
+            else:
+                ii = arg# for ii in arg: ONE ASC / SPECTRUM AT A TIME....
+                # ascstart is dt
+                ascdf,ascfilename,iascfilename, ascstart = histo_io.select_asc_to_load( ii ,
+                                                            folder = config.CONFIG[target]['data_folder']) # FULL DF
+                print(f" {bg.white}{fg.black} INPUT channel number now: {fg.default}{bg.default} OR 'show' 'stat' to look at data ")
+
+
+        # ********************** CMD *********************************** 0 1 2 3 4 5 6 7 8
+        elif cmd in [ str(x) for x in range(9) ]:
+            if ascdf is not None:
+                print(f"i... {bg.cyan}{fg.white}selected channel {int(cmd)} from ASC file /{ascfilename}/ {fg.default}{bg.default}" )
+                # ascdf_chan = ascgeneric.select_channels(ascdf, int(cmd),  delete_original = True) # more channels possible as a list
+                ascdf_chan = ascgeneric.select_channels(ascdf, int(cmd),  delete_original = True) # if no delete, problems
+                TRGHOLD,PEAKHOLD, TIMEWIN_US,ECALIBa, ECALIBb = ascgeneric.load_ini_file( iascfilename , int(cmd) )
+                TIMEWIN_US = PEAKHOLD
+
+                if ascdf_chan is not None:
+                    if 'dtus' in ascdf_chan: # never happens
+                        print("X... YOU NEED TO RELOAD BEFORE SELECTING DIFFERENT CHANNEL")
+                    else:
+                        ascdf_chan = ascgeneric.enhance_dt(ascdf_chan)
+                        ascgeneric.asc_stat_print(ascdf_chan, TIMEWIN_US, filename = ascfilename , TRGHOLD = TRGHOLD)
+                        t0 = ascdf_chan['time'].min()
+                        t1 = ascdf_chan['time'].max()
+                        rate = len(ascdf_chan)/(t1-t0) # divided by total time
+                        runtime = dt.timedelta( seconds = t1-t0 )
+                        if   'c_erlang2' in canvases:
+                            if ascdf_chan is not None:
+                                local_generate_erlangs()
+            else:
+                print("X... NO ASC FILE LOADED .. ( awaits asc file channel number) ")
+
+
+        # ********************** CMD *********************************** asc
+        elif  cmd in ['stat','st','show','sh',"cu","cut","reset","re", "er","erlang", "sp","spectrum", "sa", "save","ti","time"]:
+            ROOT.gStyle.SetOptStat(1111111) # WORKS
+            if ascdf is not None:
+
+                print(f"i... {bg.cyan}{fg.white} Data overview -  ASC file /{ascfilename}/ {fg.default}{bg.default}" )
+                if cmd.find("st")==0:
+                    if ascdf_chan is not None:
+                        deadttot = ascgeneric.asc_stat_print(ascdf_chan, TIMEWIN_US,  filename = ascfilename,  TRGHOLD = TRGHOLD)
+
+                    else:
+                        ascgeneric.asc_stat_print(ascdf, TIMEWIN_US,  filename = ascfilename, TRGHOLD = TRGHOLD)
+
+                if cmd.find("ti")==0:  # time histogram
+                    if ascdf_chan is not None:
+                        if len(canvases)>0:
+                            arg = list(canvases.keys())[0].split("c_")[-1]
+                            binlo = histograms[arg].GetXaxis().GetFirst()
+                            binhi = histograms[arg].GetXaxis().GetLast()
+                            elo = bin2ene(binlo, histograms[arg])
+                            ehi = bin2ene(binhi, histograms[arg])
+                        else:
+                            binlo = 0
+                            binhi = 99999
+                            elo   = 0
+                            ehi   = 99999
+
+                        print(f"D... REGION:  {binlo}..{binhi}  (in channels)  crosscheck4E: {elo:.1f}..{ehi:.1f} ")
+                        histt = ascgeneric.histo_time( ascdf_chan, "time" , binlo, binhi )
+                        histograms['time'] = histt
+                        display_h_name( 'time' , "c_time" , filled = False, color = 2, simple = True)
+                    else:
+                        print(f"X...  {fg.red} Select channel before time profile plot {fg.default}")
+
+                if cmd.find("sp")==0:  # energy spectrum
+                    if ascdf_chan is not None:
+                        hiene = ascgeneric.histo_energy( ascdf_chan , calibration = (ECALIBa, ECALIBb) )
+                        histograms['energy'] = hiene
+                        display_h_name( 'energy' , "c_energy" , filled = False, color = 1, simple = True)
+                    else:
+                        print(f"X...  {fg.red} Select channel before spectrum plot {fg.default}")
+
+
+                if cmd.find("sh")==0:
+                    if ascdf_chan is not None:
+                        print(ascdf_chan)
+                    else:
+                        print(ascdf)
+
+                if cmd.find("sa")==0:
+                    done = False
+                    if ascdf_chan is not None:
+                        if not 'energy' in histograms.keys():
+                            hiene = ascgeneric.histo_energy( ascdf_chan , calibration = (ECALIBa, ECALIBb) )
+                            histograms['energy'] = hiene
+                        if 'energy' in histograms.keys():
+                            done = True
+                            mychan = ascdf_chan['ch'].min()
+                            newname = f"{ascfilename}_ch{mychan}"
+                            print("D...", newname)
+                            histograms[newname] = histograms['energy']
+                            histograms[newname].SetName(newname)
+
+                            t0 = ascdf_chan['time'].min()
+                            t1 = ascdf_chan['time'].max()
+                            myrtime = runtime.total_seconds()
+                            myrtime = t1-t0 # WHEN CUT
+                            mystart = ascstart + dt.timedelta(seconds=t0)
+                            print(f"D... start = {ascstart}, dead = {deadttot} in % , ")
+                            print("i... just save total, deadtime = ",deadttot)
+                            save_hist_txt( newname , total_time = myrtime ,
+                                           started = mystart,
+                                           deadtime = deadttot/100 )
+
+                    if not done:
+                        print("X... NOT SAVED....  select channel '#' and  create spectrum 'sp' then 'sa' ")
+
+                if   cmd.find("er")==0:
+                    if ascdf_chan is not None:
+                        local_generate_erlangs() # internal function in this function
+                    else:
+                        print(f"X... {fg.red} Select channel before erlang plot {fg.default}")
+
+                if cmd.find("re")==0:
+                    if ascdf_chan is not None:
+                        ascdf_chan.drop(ascdf_chan.index, inplace=True)
+                        ascdf_chan = None
+                        rate = 0
+                        runtime = dt.datetime.now()
+                        runtime = dt.datetime.now() -runtime
+
+                        print(f"X... {fg.green}reset done, enter new channel to  select  {fg.default}")
+                    else:
+                        print(f"X... {fg.red}No reset done, channel cut is not present {fg.default}")
+
+                if cmd.find("cu")==0:
+                    if ascdf_chan is not None:
+                        t_from = None
+                        t_to = None
+                        arg = arg.split(" ")
+                        if len(arg)==2:
+                            t_from = arg[0]
+                            t_to = arg[1]
+                            ascdf_chan = ascgeneric.cut_asc(ascdf_chan, t_from, t_to)
+                            print(f"i... {fg.green}CUT DONE ({t_from},{t_to})  {fg.default}")
+                            t0 = ascdf_chan['time'].min()
+                            t1 = ascdf_chan['time'].max()
+                            rate = len(ascdf_chan)/(t1-t0) # divided by total time
+                            runtime = dt.timedelta( seconds = t1-t0 )
+
+                        else:
+                            print(f"X... {fg.red} NO times from - to - in seconds were given... {fg.default}", arg )
+                    else:
+                        # ascdf = ascgeneric.cut_asc(ascdf)
+                        print(f"X... {fg.red}  I dont cut the base ASC file, select channel first {fg.default}")
+
+
+            else:
+                print("X... ASC file is not loaded, type 'L' or 'L1' ... ")
+
+
+
+
+        # ********************** CMD ***********************************
         elif  cmd == "l":  # ***CMD***  LOAD ====== l
             if arg=="":
-                select_histo_to_load(  ) # load_txt()
-                print(f"i.. {fg.cyan} LOAD WITH NUMBER like:    l1  l2 l3 ...  {fg.default}")
+                select_histo_to_load(  folder = config.CONFIG[target]['data_folder'] ) # load_txt()
+                print(f"i.. {fg.cyan} LOAD TXT WITH NUMBER like:    l1  l2 l3 ...  {fg.default}")
             else:
-                for ii in arg:
-                    select_histo_to_load( ii ) # load_txt() # all that are given in argument l67
-            #continue # arg="bg"
-            # #-------------standard manipulation:  _lt...txt
-            # lis = glob.glob(f"{arg}_lt*_a*_b*.txt")
-            # filename = ""
-            # print(lis)
-            # if len(lis)>0:
-            #     filename = lis[0]
-            #     print(f"i... loading {filename}")
-            #     grp = re.search(r'[\w\d]+_lt([\d\.]+)_a([\d\.]+)_b([\-\d\.]+)\.txt',filename)
-            #     print(f"{fg.green} {grp.groups()} {fg.default}")
-            #     h1np_backg_lt = float(grp.groups()[0])
-            #     cala_bg = float(grp.groups()[1])
-            #     calb_bg = float(grp.groups()[2])
-            #     #arg = lis[0]
-            #     #h1np_backg_lt = arg.split("_lt")[-1]
-            #     #h1np_backg_lt = float(h1np_backg_lt.split(".txt")[0])
-            #     #print(f"i...  background live time {h1np_backg_lt} seconds")
-            # else:
-            #     #break
-            #     #arg=f"{arg}.txt"
-            #     arg=""
-            #     print(f"{fg.red}X... no live time {arg}_lt****.txt found....{fg.default}")
-
-            # print(f"i... loading spectrum /{filename}/")
-            # if os.path.exists(filename):
-            #     with open(filename) as f:
-            #         spe = f.readlines()
-            #     spe = [ float(x.strip()) for x in spe]
-            #     spe.insert(0,0) # to be compatible with underflow and overflow
-            #     spe.append(0)
-            #     h1np_backg = np.array( spe )
-            #     print(h1np_backg, "L=",len(h1np_backg))
-            #     # normalize
-            #     fill_h_with_np( h1np_backg,"bac", h1np_backg_lt, limits_calib=[calb_bg, cala_bg*(len(h1np_backg)-2)+calb_bg ])
-            # else:
-            #     print(f"{fg.red}X... NO bac backgroung loaded{fg.default}")
+                ii = arg# for ii in arg: ONE ASC / SPECTRUM AT A TIME....for ii in arg:
+                select_histo_to_load( ii , folder = config.CONFIG[target]['data_folder']) # load_txt() # all that are given in argument l67
+                limits_calib = histograms[f"s{ii}"].GetXaxis().GetXmin(),histograms[f"s{ii}"].GetXaxis().GetXmax()
 
+
+        # ********************** CMD ***********************************
         elif cmd == "q":   # ***CMD***  QUIT  ======= q
             print("i... just q: doing exit...")
             # immediate
             config.CONFIG["poll_time"] = 1
-            b0c01.set_step( config.CONFIG["poll_time"])
+            if not OFFLINE:
+                b0c01.set_step( config.CONFIG["poll_time"])
             thr.do_run = False
             #kthread.do_run = False # NO NEED IN SSH VERSION
             break
             sys.exit(0) # I must kill in ssh version....
 
+        # ********************** CMD ***********************************
         elif len(cmd)>0:   # ***CMD***  ?
             print(f"{fg.red}X... unknown command cmd=/{cmd}/ arg=/{arg}/ ...{fg.default}")
-            lis = glob.glob(f"*.txt")
-            print("i... available TXT==",lis)
-            lis = glob.glob(f"*_lt*.txt")
-            print("i... available BG ==",lis)
+            #lis = glob.glob(f"*.txt")
+            #print("i... available TXT==",lis)
+            #lis = glob.glob(f"*_lt*.txt")
+            #print("i... available BG ==",lis)
 
 
 
 
 
         #=============================================================END OF COMMMANDS==========
         #=============================================================END OF COMMMANDS==========
@@ -1272,35 +1519,44 @@
         rdays = runtime.days# floor(runtime.total_seconds()/3600/24)
         rhours = floor(runtime.seconds/3600)
         rminsec = runtime.total_seconds() - (rdays*24+rhours)*3600
         rminu = floor(rminsec/60)
         rsec = int(rminsec - rminu*60)
 
         # total histogram time
+
         rditime = f"{rdays*24+rhours:03d}:{rminu:02d}:{rsec:02d}"
+
         # was ....RUN= str(runtime)[0:10]
 
         # prima = str(dt.datetime.now())[:-5]
         if OFFLINE:
-            prima = f"{bg.green}{fg.white}{fx.bold}OFFLINE{fg.default}{bg.blue}"
+            if ascdf is not None:
+                prima = f"{bg.red}{fg.white}{fx.bold}{ascfilename}{fg.default}{bg.blue}"
+            else:
+                prima = f"{bg.green}{fg.white}{fx.bold}OFFLINE{fg.default}{bg.blue}"
         else:
             prima = f"{bg.green}{fg.white}{fx.bold}{spectrumname}{fg.default}{bg.blue}"
 
 
-        if LOCAL_GLOB_NONE_CALIB==0:LOCAL_GLOB_NONE_CALIBname="loca"
-        if LOCAL_GLOB_NONE_CALIB==1:LOCAL_GLOB_NONE_CALIBname="glob"
-        if LOCAL_GLOB_NONE_CALIB==2:LOCAL_GLOB_NONE_CALIBname="none"
-        top.print_to( 0, f" {prima} {fg.white}{fx.bold} dt={deltat:.2f} sec. {fg.yellow} rate={rate:7.1f} {fg.white} RUN={rditime} MEM={lenhistos:4}  D[{h1np_last_interval:.0f}s]={warn_del} {d_last_interval:.2f} {unwarn_del} {fg.default} : INFL={INFLUX} : CAL:{LOCAL_GLOB_NONE_CALIBname}" )
+        if LOCAL_GLOB_NONE_CALIB==0:LOCAL_GLOB_NONE_CALIBname=f"{bg.orange}{fg.white}CAL_loca{fg.default}{bg.default}"
+        if LOCAL_GLOB_NONE_CALIB==1:LOCAL_GLOB_NONE_CALIBname=f"{bg.green}{fg.white}CAL_glob{fg.default}{bg.default}"
+        if LOCAL_GLOB_NONE_CALIB==2:LOCAL_GLOB_NONE_CALIBname=f"{bg.black}{fg.white}CAL_none{fg.default}{bg.default}"
+
+        if INFLUX: INFLUXp = f"{bg.green}  INFLUX{bg.default}"
+        else: INFLUXp = f"{bg.orange}{fg.black}NOINFLUX{fg.default}{bg.default}"
+
+        top.print_to( 0, f" {prima} {fg.white}{fx.bold} dt={deltat:.2f} sec. {fg.yellow} rate={rate:7.1f} {fg.white} RUN={rditime} MEM={lenhistos:4}  D[{h1np_last_interval:.0f}s]={warn_del} {d_last_interval:.2f} {unwarn_del} {fg.default} : {INFLUXp} : {LOCAL_GLOB_NONE_CALIBname}" )
 
         if len(key)==0:
             top2.print_to( 0, f"{fg.cyan}{bg.black}{' '*80}{bg.black}")
         else:
             top2.print_to( 0, f"{fg.white}{bg.red} > {fx.bold}{a_abc}{fg.yellow}_{fg.white}{b_abc}{fx.default}{fg.default}{bg.default} ")
         #top.place()
 
         #top2.print_to( (1,2), f"{fg.black}{bg.yellow} > {key}{fg.default}{bg.default}")
         time.sleep(0.05)
 
-    print(f"i... gregory online DONE; {bg.red}waiting{bg.default} if threads need to finish.... {fg.red}few seconds...{fg.default} ")
+    print(f"i... FINISHED; {bg.red}waiting{bg.default} for threads .... {fg.red}maybe few seconds OR Ctrl-C...{fg.default} ")
 
 if __name__=="__main__":
     Fire(main)
```

### Comparing `gregory_online-0.2.9/gregory_online/config.py` & `gregory_online-0.3.1/gregory_online/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,20 +6,49 @@
 import os
 import sys
 
 
 
 
 #-------==========---------------------------
+# changing 20230616
+# common :  polltime  window
+# def online0 online1 ...
 CONFIG={
-    "spectrum":"b0c01",
-    "server":"127.0.0.1",
-    "udp_ip":"127.0.0.1",
+    "version":3,
     "poll_time":5,
-    "window":10,
+    "window":30,
+    "online0":{
+        "online":True,
+        "spectrum":"b0c00",
+        "description":"local server - channel 0",
+        "server":"127.0.0.1",
+        "udp_ip":"127.0.0.1",
+        "influx":False,
+        "data_folder":"./",
+    },
+    "online1":{
+        "online":True,
+        "spectrum":"b0c01",
+        "description":"local server - channel 1",
+        "server":"127.0.0.1",
+        "udp_ip":"127.0.0.1",
+        "influx":False,
+        "data_folder":"./",
+    },
+    "offline":{
+        "online":False,
+        "description":"offline, local files",
+        "data_folder":"./",
+    },
+    "offlineweb":{
+        "online":False,
+        "description":"offline, NAS 20 concrete files",
+        "data_folder":"http://10.10.104.20/WEBDATA/20220906_LOCAL_NPI_REZ_ORTEC_ALL/DATA_20230605_20230614_concrete2/"
+    },
     "placeholder": True
 }
```

### Comparing `gregory_online-0.2.9/gregory_online/data/Am241.svg` & `gregory_online-0.3.1/gregory_online/data/Am241.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/gregory_online/data/Cm247.png` & `gregory_online-0.3.1/gregory_online/data/Cm247.png`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/gregory_online/data/Np237.svg` & `gregory_online-0.3.1/gregory_online/data/Np237.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/gregory_online/data/Pa231.svg` & `gregory_online-0.3.1/gregory_online/data/Pa231.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/gregory_online/data/Pu239.svg` & `gregory_online-0.3.1/gregory_online/data/Pu239.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/gregory_online/data/Th232.svg` & `gregory_online-0.3.1/gregory_online/data/Th232.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/gregory_online/data/U235.svg` & `gregory_online-0.3.1/gregory_online/data/U235.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/gregory_online/data/U238.svg` & `gregory_online-0.3.1/gregory_online/data/U238.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/gregory_online/data/decay_lara.parquet` & `gregory_online-0.3.1/gregory_online/data/decay_lara.parquet`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/gregory_online/data/testrebin.py` & `gregory_online-0.3.1/gregory_online/data/testrebin.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/gregory_online/decay_db.py` & `gregory_online-0.3.1/gregory_online/decay_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,18 +52,18 @@
     print(f"i... {len(dfo)} gammas total", end="")
     dfo = dfo.loc[ dfo["E"]>etrsh ]
 
     df = dfo
     df = df.loc[ df["I"]>itrsh ]
     # df = df.loc[ df["E"]>etrsh ]
     df = df.loc[ df["T12"]>t12low ]
-    print(f"i... limited to {len(dfo)}  E>{etrsh}; I>{itrsh}; t12>{nicetime(t12low)}", end="")
+    print(f"; limited to {len(dfo)}: E>{etrsh}; I>{itrsh}; t12>{nicetime(t12low)}", end="")
 
     df = df.loc[ (df["E"]>e-de) & (df["E"]<e+de) ]
-    print(f"i... {len(df)} candidate(s) for dE={de:.2f}")#; limited E>{etrsh}; I>{itrsh}; t12>{nicetime(t12low)}")
+    print(f"; {len(df)} candidate(s) for dE={de:.2f}")#; limited E>{etrsh}; I>{itrsh}; t12>{nicetime(t12low)}")
     #print(f"i... {len(df)} candidates; limited E>{etrsh}; I>{itrsh}; t12>{nicetime(t12low)}")
     # susp = list(df['name'].values.tolist())
 
 
     table_data = []
 
     column=-1
```

### Comparing `gregory_online-0.2.9/gregory_online/fetchnp.py` & `gregory_online-0.3.1/gregory_online/fetchnp.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/gregory_online/histo_analyze.py` & `gregory_online-0.3.1/gregory_online/histo_analyze.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,28 +82,28 @@
     intg = h.Integral( ene2bin(elo,h), ene2bin(ehi,h) )
     return intg
 
 def histo_zoomenergy( h, xlo, xhi ):
     """
     input: TH1
     """
-    print(f"i... zooming with energy  {xlo}...{xhi}" )
+    print(f"i... zooming with energy  {xlo:.1f}...{xhi:.1f}" )
     intg = h.Integral( )
     #print(f"i... integral before zoom = {intg:16.6f}")
     h.GetXaxis().SetRangeUser( xlo, xhi ) # using energy
     intg = h.Integral( ene2bin(xlo,h), ene2bin(xhi,h) )
     #print(f"i... integral after  zoom = {intg:16.6f}")
 
     return
 
 def histo_zoombins( h, xlo, xhi ):
     """
      input: TH1
     """
-    print(f"i... zooming with bins {xlo}...{xhi}" )
+    print(f"i... zooming with bins {xlo:.1f}...{xhi:.1f}" )
     intg = h.Integral( )
     #print(f"i... integral before zoom = {intg}")
     h.GetXaxis().SetRange( xlo, xhi ) # using bins
     intg = h.Integral( xlo, xhi)
     #print(f"i... integral after zoom = {intg}")
     return
```

### Comparing `gregory_online-0.2.9/gregory_online/histo_displ.py` & `gregory_online-0.3.1/gregory_online/histo_displ.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         ci.Modified()
         ci.Update()
 
 
 
 
 
-def display_h_name( hname="tot", cname = "c_tot", filled = False , color = 39, title=None):
+def display_h_name( hname="tot", cname = "c_tot", filled = False , color = 39, title=None, simple=False):
     """
     display (e.g. substracted) histograms NEVER USED
     """
     global histograms,canvases
     if not  ROOT.gDirectory.FindObject(hname): # this naver happens
         print(f"i... histo {hname} is NOT found")
         return
@@ -66,15 +66,21 @@
         #histograms[hname].Draw("EX0")
         #histograms[hname].SetFillColor(19)
         histograms[hname].SetMarkerStyle(7)
         #histograms[hname].SetLineColor(16) # gray
         if filled:
             histograms[hname].SetFillStyle(3001)
             histograms[hname].SetFillColor(39)
-            histograms[hname].Draw("hEX0")
+            if simple:
+                histograms[hname].Draw("")
+            else:
+                histograms[hname].Draw("hEX0")
+        elif simple:
+            histograms[hname].SetLineColor(color)
+            histograms[hname].Draw("")
         else:
             histograms[hname].Draw("EX0")
         print("D... GRIDS HERE")
         ROOT.gPad.SetGridx()
         ROOT.gPad.SetGridy()
         ROOT.gPad.Modified()
         ROOT.gPad.Update()
```

### Comparing `gregory_online-0.2.9/gregory_online/histo_global_cont.py` & `gregory_online-0.3.1/gregory_online/histo_global_cont.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/gregory_online/histo_io.py` & `gregory_online-0.3.1/gregory_online/histo_io.py`

 * *Files 19% similar despite different names*

```diff
@@ -41,14 +41,22 @@
 import ROOT #  for tests here with gDirectory ls
 import time
 # JUST FOR TESTS
 from  gregory_online.histo_displ import display_np, refresh_canvases
 from gregory_online.histo_analyze import histo_fit,histo_zoomenergy
 # --------------------------------------- for  tests -----------
 
+import gregory_online.ascgeneric as ascgeneric
+
+import configparser
+
+
+import ascgeneric
+import requests
+from bs4 import BeautifulSoup
 
 def ispure2n( slen ,silent = False):
     """
     detect if it is 2^n bins or 2^n + 2 under/ovelrflow added
     """
     expon = 0
     pure2n = True
@@ -93,15 +101,15 @@
     with open( fname+".details", "w" ) as f:
         TTS = total_time
         DTP = deadtime*100
         DTS = total_time*deadtime
         LTS = TTS - DTS
         SUM = histograms[ name ].GetEntries()
         RATE = SUM/TTS
-        now = dt.datetime.now()
+        now = dt.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         if RATE>100000:
             print(f"X... {fg.red} NON REALISTIC TOTAL TIME {fg.default} ")
 
         a,b = get_calib_coefs( histograms[ name ])
         f.write(f"totaltime {TTS:.2f}\n")
         f.write(f"livetime {LTS:.2f}\n")
         f.write(f"deadtimeprc {DTP:.2f}\n")
@@ -122,55 +130,217 @@
 
     print()
     return
 
 
 
 # -------------------------------------- for load interface
-def list_spectra_disc():
+def list_spectra_disc( folder = "./" ):
     """
     look at spectra and details files. determine valid spectrum filename
     """
+    f = folder
+    if len(f)==0: f = "./"
+    if f[-1]!="/": f=f+"/"
+
     avadisc = {}
-    res = glob.glob("*.txt")
-    red = glob.glob("*.details")
+    res = None
+    red = None
+    if f.find("http://")==0:
+        res = get_url_paths(folder, "txt")
+        red = get_url_paths(folder, "details")
+    else:
+        res = glob.glob(f+"*.txt")
+        red = glob.glob(f+"*.details")
+
     num = 1
     for i in res:
         tst = os.path.splitext(i)[0]
         for j in red:
             if tst == os.path.splitext(j)[0]:
                 avadisc[num] = tst
                 num+=1
     return avadisc
 
 
+# -------------------------------------- for load interface ASC
+
+def get_url_paths(url, ext='', params={}):
+    """
+    list files from NAS - http/web exposed folder
+    """
+    if url[-1] != "/":
+        url+="/"
+    response = requests.get(url, params=params)
+    if response.ok:
+        response_text = response.text
+    else:
+        return response.raise_for_status()
+    soup = BeautifulSoup(response_text, 'html.parser')
+    parent = [url + node.get('href') for node in soup.find_all('a') if node.get('href').endswith(ext)]
+    return parent
+
+
+# -------------------------------------- for load interface ASC
+def list_asc_disc( folder = "./"):
+    """
+    look at spectra and details files. determine valid spectrum filename
+    """
+    f = folder
+    if len(f)==0: f = "./"
+    if f[-1]!="/": f=f+"/"
+    avadisc = {}
+    res = None
+    red = None
+    if f.find("http://")==0:
+        res = get_url_paths(folder, "asc")
+        red = get_url_paths(folder, "ini")
+    else:
+        res = glob.glob(f+"*.asc")
+        red = glob.glob(f+"*.ini")
+    num = 1
+    for i in res:
+        tst = os.path.splitext(i)[0]
+        for j in red:
+            if tst == os.path.splitext(j)[0]:
+                avadisc[num] = os.path.basename(tst)
+                num+=1
+    return avadisc
+
+
+# ================================================ ASC AND INI ==================
+#
+# I like it here, bc menu interaction
+#
+def load_asc( filename  ):  # complete filena or address
+    """
+    loads asc file, needs ini file too
+
+    returns DF and inifile
+    """
+    # f = folder
+    # if len(f)==0: f = "./"
+    # if f[-1]!="/": f=f+"/"
+
+    #avadisc = list_asc_disc( folder = folder)
+    # # present_avadisc(avadisc)
+
+
+    inifilename = os.path.splitext(filename)[0]+".ini"
+    ascfilename = os.path.splitext(filename)[0]+".asc"
+
+    exini = False
+    if filename.find("http://")==0:
+        inifilename = ascgeneric.get_ini_copy( inifilename )
+        print(" ... ",inifilename)
+        #exini = True
+
+    else:
+        #print("X... no file ", filename, end=" ...")
+        if os.path.exists(ascfilename):
+            pass
+            # filename = f+hole+".asc"
+            # print("i... replacing with ", filename)
+        else:
+            print("X... no file ", ascfilename)
+            return None, None
+
+    res = ascgeneric.load_ini_file( inifilename ) # I never need channel here.. Later, after CUT
+    inifile = True
+
+    if res is None:
+        print(f"x... {bg.red}NO INI FILE PRESENT{bg.default}")
+        inifile = False
+        return None, None
+    else:
+        print(f"i... {bg.green} INI FILE PRESENT{bg.default}")
+        start = ascgeneric.filename_decomp( filename )   #  - get start from filename TO REPORT
+        print("D... started", start, type(start) )
+        print(f" {bg.white}{fg.black} ... LOADING {ascfilename} ... {fg.default}{bg.default}")
+        wastart = dt.datetime.now()
+        df = ascgeneric.pd_read_table( ascfilename, sort = True,  fourcolumns = False)
+        wastop = dt.datetime.now()-wastart
+        print(f" {bg.white}{fg.green} ... LOADED {len(df)/1000/1000:.2f} Mrows ... {len(df)/wastop.total_seconds()/1000/1000:.2f} Mrows/sec {fg.default}{bg.default}")
+        print()
+
+        #df = pd.DataFrame( range(10) )
+        #print(df)
+
+    return df, inifilename, start
+
+
+def select_asc_to_load( num=None , folder = "./"):
+    """
+    present available asc files and/or load one
+
+    load_asc .... return df,filename
+    """
+    avadisc = list_asc_disc( folder = folder )
+    if num is None:
+        present_avadisc(avadisc, bgcolor = f"{bg.white}")
+        return None,None,None, None
+
+    try:
+        num = int(num)
+    except:
+        num = None
+        print("X... no spectrum selected")
+    if num in avadisc.keys():
+        f = folder
+        if len(f)==0: f = "./"
+        if f[-1]!="/": f=f+"/"
+
+        # return DF and name
+        print(f"D...  s.a.t.l. {avadisc[num]}")
+        df, ininame,start = load_asc( f+avadisc[num]  )
+        # returning from  select_asc_to_load - called from bin
+        return  df, avadisc[num], ininame,start
+    return None,None,None, None
+
 
-def present_avadisc( avadisc ):
+
+def present_avadisc( avadisc , bgcolor=f"{bg.yellow}"):
     print()
     col = 0
 
+    termsize = os.get_terminal_size()
+    maxwid = termsize.columns
+    maxname = 0
+    for ke in sorted(avadisc.keys()):
+        if len(avadisc[ke])>maxname:maxname = len(avadisc[ke])
+    maxname+=5
+    ncols=int(maxwid/maxname)
+    if ncols == 0: ncols =1
+    print(maxwid, maxname, ncols )
     for ke in sorted(avadisc.keys()):
         col+=1
         brk = ""
-        if col%3==0:
+        if col% ncols==0:
             brk = "\n"
-        print( f"  {bg.yellow}{fg.black} {ke} {fg.default}{bg.default}  {avadisc[ke]:35s} ", end=brk)
+        print( f"  {bgcolor}{fg.black} {ke} {fg.default}{bg.default}  {avadisc[ke]:{maxname}s} ", end=brk)
     print()
     print()
 
 
-def select_histo_to_load( num=None ):
+# ================================================ HISTO AND DETAILS ==================
+
+
+def select_histo_to_load( num=None , folder = "./"):
     """
     full sequence list,present, load
     """
-    avadisc = list_spectra_disc()
+    f = folder
+    if len(f)==0: f = "./"
+    if f[-1]!="/": f=f+"/"
+
+    avadisc = list_spectra_disc( folder = folder )
     present_avadisc(avadisc)
     if num is None:
         return
-        #num = input()
+
     try:
         num = int(num)
     except:
         num = None
         print("X... no spectrum selected")
     if num in avadisc.keys():
         load_hist_txt( avadisc[num] , f"s{num}" )
@@ -187,61 +357,86 @@
         res = [ (x.strip().split(" ")[0],"_".join(x.strip().split(" ")[1:])) for x in res]
         res = dict(res)
 
         # the following are gonna be converted and cause a crash if error
         res["totaltime"] = float(res["totaltime"]) # not always needed?
         # not floatres["started"] = float(res["started"]) # not always needed
         res["livetime"] = float(res["livetime"])
-        res["a"] = float(res["a"])
-        res["b"] = float(res["b"])
+        try:
+            res["a"] = float(res["a"])
+            res["b"] = float(res["b"])
+        except:
+            res["a"] = 1
+            res["b"] = 0
+            print(f"X... {fg.red} I dont see a calibration in the details file {fg.default}" )
         res["entries"] = float(res["entries"])
         res["rate"] = float(res["rate"])
     return res
 
 
 
 
+
+# ----------------------------------------------------
+
+
+
+
+
+
+
 def load_hist_txt( filename, hname , underoverflow = False):
     """
     loads histo : full or rate w. details file.
     histograms[] will get NORMALIZED version;  underover bit is appended just for TH1
     returns nparray without under over flow.
     """
     # I use pandas as in pr_load.py ...
-    avadisc = list_spectra_disc()
-    present_avadisc(avadisc)
-
-    hole = os.path.splitext(filename)[0]
-    if not os.path.exists(filename):
-        print("X... no file ", filename, end=" ...")
-        if os.path.exists(hole+".txt"):
-            filename = hole+".txt"
-            print("i... replacing with ", filename)
-        else:
-            print("X... no file ", filename)
-            return None
+    #avadisc = list_spectra_disc()
+    #present_avadisc(avadisc)
 
-    res = load_details( hole+".details")
+    hfilename = os.path.splitext(filename)[0]+".txt"
+    dfilename = os.path.splitext(filename)[0]+".details"
     details = True
-    if res is None: details = False
+    if filename.find("http://")==0:
+        dfilename = ascgeneric.get_ini_copy( dfilename )
+        res = load_details(  dfilename )
+        if res is None: details = False
+    else:
+        res = load_details(  dfilename )
+        if res is None: details = False
 
+    # #hole = os.path.splitext(filename)[0]
+    # if not os.path.exists(filename):
+    #     print("X... no file ", filename, end=" ...")
+    #     if os.path.exists(hole+".txt"):
+    #         filename = hole+".txt"
+    #         print("i... replacing with ", filename)
+    #     else:
+    #         print("X... no file ", filename)
+    #         return None
+
+    # res = load_details( hole+".details")
+    # details = True
+    # if res is None: details = False
 
-    df = pd.read_csv(filename, delimiter="\s+", header=None, comment="#", nrows=2)
+    print("D... histo-txt:", hfilename )
+    df = pd.read_csv(hfilename, delimiter=r"\s+", header=None, comment="#", nrows=2)
     ncols = df.shape[1]
-    print(f"D... file {filename} with {ncols} columns, details found = {details}")
+    print(f"D... file {hfilename} with {ncols} columns, details found = {details}")
 
     np_c = None
     np_e = None # for rate into th1f
 
     if (ncols==1):
-        df = pd.read_csv(filename, delimiter="\s+", header=None, comment="#", names = ['cont'] )
+        df = pd.read_csv(hfilename, delimiter=r"\s+", header=None, comment="#", names = ['cont'] )
         print(df)
         np_c = df['cont'].values
     if (ncols==3):
-        df = pd.read_csv(filename, delimiter="\s+", header=None, comment="#", names = ['bin','cont','err'] )
+        df = pd.read_csv(hfilename, delimiter=r"\s+", header=None, comment="#", names = ['bin','cont','err'] )
         print(df)
         np_c = df['cont'].values
         np_e = df['err'].values
 
         # print( type(np_c), type(np_e), np_c)
         # df.to_csv("zest.txt", sep=' ', header = None)
 
@@ -291,15 +486,15 @@
 
     #  create a normalized histo in the histograms[]
     fill_h_with_np( h1np_backg, hname,
                                  runtime = res["livetime"], errors = np_e,
                                  limits_calib=[res["b"], res["a"]*(len(h1np_backg)-2)+res["b"] ]
     )
     histograms[hname].SetEntries( res["entries"] )
-    histograms[hname].SetTitle( hole)
+    histograms[hname].SetTitle(  os.path.basename(hfilename) )
     histograms[hname].Print()
     print(f" ... Name= {histograms[hname].GetName()}  Title={histograms[hname].GetTitle()}" )
 
     if not underoverflow:
         # artificialy added unovf, removing again
         return h1np_backg[1:-1]
     else:
```

### Comparing `gregory_online-0.2.9/gregory_online/histo_np_ops.py` & `gregory_online-0.3.1/gregory_online/histo_np_ops.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/gregory_online/key_enter.py` & `gregory_online-0.3.1/gregory_online/key_enter.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/gregory_online/topbar.py` & `gregory_online-0.3.1/gregory_online/topbar.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,17 @@
             self.BCOL = bgcolor #bg.blue
         elif pos==2:
             self.BCOL = bgcolor # bg.white
         #self.t = threading.currentThread()
 
         try:
             #print("report_cursor to appear")
-            print( "i... topbar: pos/cursor",pos, report_cursor() )
+            #print( "i... topbar: pos/cursor",pos, report_cursor() )
+            pos
+            report_cursor()
             #print("report done")
         except:
             print("X... problem with report_cursor")
 
         #print("i... topbar bar started")
```

### Comparing `gregory_online-0.2.9/gregory_online/utils.py` & `gregory_online-0.3.1/gregory_online/utils.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.2.9/gregory_online.egg-info/PKG-INFO` & `gregory_online-0.3.1/gregory_online.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: gregory-online
-Version: 0.2.9
+Version: 0.3.1
 Summary: Online watching HTTP server of ROOT on port 9009
-Home-page: UNKNOWN
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 Project gregory~online~
 =======================
 
 *experimental code to online survey root spectra from THTTPServer*
 
@@ -79,9 +77,7 @@
   mock~server~.py         
   rebin.py                
   setup.py                
   topbar.py               
   utilone.py              
   version.py              
   ----------------------- ------------------------------
-
-
```

### Comparing `gregory_online-0.2.9/gregory_online.egg-info/SOURCES.txt` & `gregory_online-0.3.1/gregory_online.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 README.md
 setup.py
 bin/gregory_online
 gregory_online/__init__.py
+gregory_online/ascgeneric.py
 gregory_online/config.py
 gregory_online/decay_db.py
+gregory_online/dpp2jpg.py
+gregory_online/erlang.py
 gregory_online/fetchnp.py
 gregory_online/histo_analyze.py
 gregory_online/histo_displ.py
 gregory_online/histo_global_cont.py
 gregory_online/histo_io.py
 gregory_online/histo_np_ops.py
 gregory_online/key_enter.py
```

### Comparing `gregory_online-0.2.9/setup.py` & `gregory_online-0.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,9 +29,9 @@
     license="GPL2",
     version=get_version("gregory_online/version.py"),
     packages=['gregory_online'],
     package_data={'gregory_online': ['data/*']},
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     scripts = ['bin/gregory_online'],
-    install_requires = ['fire','scipy','pyfromroot','pytermgui','readchar','fastnumbers','sshkeyboard','terminaltables'],
+    install_requires = ['fire','scipy','pyfromroot','pytermgui','readchar','fastnumbers','sshkeyboard','terminaltables','fastparquet','tables','simple_term_menu'],
 )
```

