# Comparing `tmp/gregory_online-0.3.1.tar.gz` & `tmp/gregory_online-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gregory_online-0.3.1.tar", last modified: Fri Jun 23 11:58:17 2023, max compression
+gzip compressed data, was "gregory_online-0.3.3.tar", last modified: Fri Jun 23 13:33:13 2023, max compression
```

## Comparing `gregory_online-0.3.1.tar` & `gregory_online-0.3.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 11:58:17.371809 gregory_online-0.3.1/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-23 11:58:17.371809 gregory_online-0.3.1/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-02 15:20:26.000000 gregory_online-0.3.1/README.md
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 11:58:17.367809 gregory_online-0.3.1/bin/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    69602 2023-06-23 11:58:12.000000 gregory_online-0.3.1/bin/gregory_online
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 11:58:17.367809 gregory_online-0.3.1/gregory_online/
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/__init__.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    27793 2023-06-23 07:57:50.000000 gregory_online-0.3.1/gregory_online/ascgeneric.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7269 2023-06-23 07:56:33.000000 gregory_online-0.3.1/gregory_online/config.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 11:58:17.371809 gregory_online-0.3.1/gregory_online/data/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    56290 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/Am241.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   503044 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/Cm247.png
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    53304 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/Np237.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    79580 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/Pa231.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    93285 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/Pu239.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    59999 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/Th232.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    78694 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/U235.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)    97718 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/U238.svg
--rw-rw-r--   0 ojr       (1000) ojr       (1000)   123572 2023-06-12 07:00:49.000000 gregory_online-0.3.1/gregory_online/data/decay_lara.parquet
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1139 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/data/testrebin.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3758 2023-06-12 07:00:49.000000 gregory_online-0.3.1/gregory_online/decay_db.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    15128 2023-06-23 07:56:33.000000 gregory_online-0.3.1/gregory_online/dpp2jpg.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3631 2023-06-23 07:56:33.000000 gregory_online-0.3.1/gregory_online/erlang.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12625 2023-06-12 07:00:49.000000 gregory_online-0.3.1/gregory_online/fetchnp.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4543 2023-06-23 07:56:33.000000 gregory_online-0.3.1/gregory_online/histo_analyze.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4169 2023-06-23 07:56:33.000000 gregory_online-0.3.1/gregory_online/histo_displ.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)      833 2023-06-12 07:00:49.000000 gregory_online-0.3.1/gregory_online/histo_global_cont.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)    19155 2023-06-23 11:14:01.000000 gregory_online-0.3.1/gregory_online/histo_io.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-06-05 13:33:05.000000 gregory_online-0.3.1/gregory_online/histo_np_ops.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-19 12:31:34.000000 gregory_online-0.3.1/gregory_online/key_enter.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2594 2023-06-23 07:56:33.000000 gregory_online-0.3.1/gregory_online/topbar.py
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2023-03-15 09:15:19.000000 gregory_online-0.3.1/gregory_online/utilone.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3293 2023-06-12 07:00:49.000000 gregory_online-0.3.1/gregory_online/utils.py
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-23 11:58:17.000000 gregory_online-0.3.1/gregory_online/version.py
-drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 11:58:17.367809 gregory_online-0.3.1/gregory_online.egg-info/
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-23 11:58:17.000000 gregory_online-0.3.1/gregory_online.egg-info/PKG-INFO
--rw-rw-r--   0 ojr       (1000) ojr       (1000)     1006 2023-06-23 11:58:17.000000 gregory_online-0.3.1/gregory_online.egg-info/SOURCES.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-23 11:58:17.000000 gregory_online-0.3.1/gregory_online.egg-info/dependency_links.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)      116 2023-06-23 11:58:17.000000 gregory_online-0.3.1/gregory_online.egg-info/requires.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-23 11:58:17.000000 gregory_online-0.3.1/gregory_online.egg-info/top_level.txt
--rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-23 11:58:17.371809 gregory_online-0.3.1/setup.cfg
--rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1259 2023-06-23 11:13:06.000000 gregory_online-0.3.1/setup.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 13:33:13.047789 gregory_online-0.3.3/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-23 13:33:13.047789 gregory_online-0.3.3/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1560 2023-06-02 15:20:26.000000 gregory_online-0.3.3/README.md
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 13:33:13.043789 gregory_online-0.3.3/bin/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    70902 2023-06-23 13:32:52.000000 gregory_online-0.3.3/bin/gregory_online
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 13:33:13.043789 gregory_online-0.3.3/gregory_online/
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      261 2023-03-15 09:15:19.000000 gregory_online-0.3.3/gregory_online/__init__.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    28895 2023-06-23 13:04:50.000000 gregory_online-0.3.3/gregory_online/ascgeneric.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     7269 2023-06-23 07:56:33.000000 gregory_online-0.3.3/gregory_online/config.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 13:33:13.047789 gregory_online-0.3.3/gregory_online/data/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    56290 2023-03-15 09:15:19.000000 gregory_online-0.3.3/gregory_online/data/Am241.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   503044 2023-03-15 09:15:19.000000 gregory_online-0.3.3/gregory_online/data/Cm247.png
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    53304 2023-03-15 09:15:19.000000 gregory_online-0.3.3/gregory_online/data/Np237.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    79580 2023-03-15 09:15:19.000000 gregory_online-0.3.3/gregory_online/data/Pa231.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    93285 2023-03-15 09:15:19.000000 gregory_online-0.3.3/gregory_online/data/Pu239.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    59999 2023-03-15 09:15:19.000000 gregory_online-0.3.3/gregory_online/data/Th232.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    78694 2023-03-15 09:15:19.000000 gregory_online-0.3.3/gregory_online/data/U235.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)    97718 2023-03-15 09:15:19.000000 gregory_online-0.3.3/gregory_online/data/U238.svg
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)   123572 2023-06-12 07:00:49.000000 gregory_online-0.3.3/gregory_online/data/decay_lara.parquet
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1139 2023-03-15 09:15:19.000000 gregory_online-0.3.3/gregory_online/data/testrebin.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3758 2023-06-12 07:00:49.000000 gregory_online-0.3.3/gregory_online/decay_db.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    15128 2023-06-23 07:56:33.000000 gregory_online-0.3.3/gregory_online/dpp2jpg.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3631 2023-06-23 07:56:33.000000 gregory_online-0.3.3/gregory_online/erlang.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    12625 2023-06-12 07:00:49.000000 gregory_online-0.3.3/gregory_online/fetchnp.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4741 2023-06-23 13:32:00.000000 gregory_online-0.3.3/gregory_online/histo_analyze.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4169 2023-06-23 07:56:33.000000 gregory_online-0.3.3/gregory_online/histo_displ.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)      833 2023-06-12 07:00:49.000000 gregory_online-0.3.3/gregory_online/histo_global_cont.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)    19155 2023-06-23 11:14:01.000000 gregory_online-0.3.3/gregory_online/histo_io.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     4942 2023-06-05 13:33:05.000000 gregory_online-0.3.3/gregory_online/histo_np_ops.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     5961 2023-04-19 12:31:34.000000 gregory_online-0.3.3/gregory_online/key_enter.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     2594 2023-06-23 07:56:33.000000 gregory_online-0.3.3/gregory_online/topbar.py
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        0 2023-03-15 09:15:19.000000 gregory_online-0.3.3/gregory_online/utilone.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     3293 2023-06-12 07:00:49.000000 gregory_online-0.3.3/gregory_online/utils.py
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)       20 2023-06-23 13:33:12.000000 gregory_online-0.3.3/gregory_online/version.py
+drwxrwxr-x   0 ojr       (1000) ojr       (1000)        0 2023-06-23 13:33:13.043789 gregory_online-0.3.3/gregory_online.egg-info/
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1775 2023-06-23 13:33:12.000000 gregory_online-0.3.3/gregory_online.egg-info/PKG-INFO
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)     1006 2023-06-23 13:33:13.000000 gregory_online-0.3.3/gregory_online.egg-info/SOURCES.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)        1 2023-06-23 13:33:12.000000 gregory_online-0.3.3/gregory_online.egg-info/dependency_links.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)      116 2023-06-23 13:33:12.000000 gregory_online-0.3.3/gregory_online.egg-info/requires.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       15 2023-06-23 13:33:12.000000 gregory_online-0.3.3/gregory_online.egg-info/top_level.txt
+-rw-rw-r--   0 ojr       (1000) ojr       (1000)       38 2023-06-23 13:33:13.047789 gregory_online-0.3.3/setup.cfg
+-rwxrwxr-x   0 ojr       (1000) ojr       (1000)     1259 2023-06-23 11:13:06.000000 gregory_online-0.3.3/setup.py
```

### Comparing `gregory_online-0.3.1/PKG-INFO` & `gregory_online-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gregory_online
-Version: 0.3.1
+Version: 0.3.3
 Summary: Online watching HTTP server of ROOT on port 9009
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 
 Project gregory~online~
```

### Comparing `gregory_online-0.3.1/README.md` & `gregory_online-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/bin/gregory_online` & `gregory_online-0.3.3/bin/gregory_online`

 * *Files 1% similar despite different names*

```diff
@@ -618,45 +618,49 @@
             yx=f"{fg.yellow}"
             nx=f"{fg.default}"
 
             yg=f"{bg.green}{fg.white}"
             ng=f"{bg.default}{fg.default}"
             print(f"""{yg}----HELP---------------------------------------{ng}
  {yy}h{ny} ... this help
- {yy}t{ny} ... set time of real spectrum: 't 1:59:59'
- {yy}a{ny} ... age AKA last_interval for the "last" histo : e.g. "a 3600"
+({yy}t{ny} ... set time of real spectrum: 't 1:59:59')
+({yy}a{ny} ... age AKA last_interval for the "last" histo : e.g. "a 3600")
  {yy}r{ny} ... range,pk search    {yy}R{ny} ... Record range, pks to DISK
  {yy}f{ny} ... fit
  {yy}c{ny} ... calib (energy)
  {yy}i{ny} ... info               {yy}v{ny} ... view histo details
  {yy}u{ny} ... unzoom             {yy}z{ny} ... zoom
  {yy}n{ny} ... next               {yy}p{ny} ... previous
- {yy}w{ny} ... window width
+ {yy}w{ny} ... window (view on 1st zoom) width
  {yy}s{ny} ... save histogram     {yy}l{ny} ... load histogram
-                                  {yy}L{ny} ... load ascfile
+                           {yy}L{ny} ... load ASC file; {yy}h{ny} more help avail.
  {yy}d{ny} ... display histo:
     {yx}t{nx} ... tot/total (also if t is omitted)
     {yx}r{nx} ... rat/rates (tot normalized on time)
     {yx}b{nx} ... bac/background  (must be loaded by l)
     {yx}s{nx} ... sub/substracted (rate - backg-rate) rate
     {yx}l{nx} ... last [age] seconds histogram (defined by a)
     {yx}m{nx} ... the few seconds [dt] difference histo
  {yy}q{ny} ... quit
 ----------------
-Histograms:   tot, rat, bac  diff  last  sub
+Online Histograms:   tot, rat, bac  diff  last  sub
 """)
             if ascdf is not None:
                 print(f"""
-{yg}L {ng} ... load ASC file
-{yg}# {ng} ... select channel # from ASC (create ASC-chan frame)
-{yg}st{ng} ... stat ... statistics on ASC file
-{yg}sh{ng} ... show ... show a sample of ASC file
-{yg}cu{ng} ... cut ... 'cut from to' - use on ASC-chan frame
-{yg}er{ng} ... erlang ... plot erlang from  ASC-chan frame
-{yg}re{ng} ... reset ... discard current selections = ASC-chan frame
+ {yg}L {ng} ... load ASC file
+ {yg}# {ng} ... select channel # from ASC (create ASC-chan frame)
+ {yg}st{ng} ... stat ... statistics on ASC/ASC-chan file
+ {yg}sh{ng} ... show ... show a sample of ASC/ASC-chan file
+ {yg}cu{ng} ... cut ... 'cut from to' - use on ASC-chan frame
+ {yg}er{ng} ... erlang ... plot erlang from  ASC-chan frame
+ {yg}sp{ng} ... spectra ... plot energy spectrum from ASC-chan frame
+ {yg}sa{ng} ... save ... save energy spectrum from  ASC-chan frame
+ {yg}ti{ng} ... time ... plot rate vs. time for energy region for ASC-chan frame
+
+ {yg}re{ng} ... reset ... discard current selections = ASC-chan frame
 
 """)
 # diff ... what changed from the last read = last [dt] sec. histo
 # last ... tot - [age] seconds old histo = last [age] sec. histo
 # sub  ... tot - bac (normalized on rate)  ? last - bac ?  ? last - tot ?
 
 # Watchdog: for influx, log etc...
@@ -793,14 +797,21 @@
             if len(arg)>0:
                 eline = None # energy of the line
                 bline = None # bin of the line
                 dbline = 1
                 if len(arg.split())<1:
                     print(f"X... {fg.red} give me {bg.white}'c  ene bin'{bg.default} OR 'c  reset' ==  'c r'{fg.default}")
                     # break
+                elif arg.split()[0] in histograms.keys():  # ** APPLY FOR HISTO **
+                    print("D... Aplly calib for histogram", arg.split()[0])
+                    LOCAL_GLOB_NONE_CALIB == 0
+                    binmax =  histograms[arg.split()[0]].GetXaxis().GetXmax()
+                    limits_calib = 0*ECALIBa + ECALIBb,binmax*ECALIBa + ECALIBb
+                    histograms[arg.split()[0]].GetXaxis().SetLimits( limits_calib[0],limits_calib[1] )
+
                 elif arg.split()[0]=="reset" or arg.split()[0]=="r" :  # ** reset **
                     ECALIB = []
                     ECALIBa = 1
                     ECALIBb = 0
                     print(f"i... {fg.yellow} RESET! e-calibration done{fg.default} ")
                 elif arg.split()[0]=="local" or arg.split()[0]=="l" :  # **
                     LOCAL_GLOB_NONE_CALIB = 0
@@ -886,23 +897,28 @@
                 tarea = histo_area(  histograms[arg] )
                 # when zoom:
                 binlo = histograms[arg].GetXaxis().GetFirst()
                 binhi = histograms[arg].GetXaxis().GetLast()
                 elo = bin2ene(binlo, histograms[arg])
                 ehi = bin2ene(binhi, histograms[arg])
                 zarea = histo_area(  histograms[arg] ,elo , ehi)
+                #
+                myrate = tarea/runtime.total_seconds()
+                myratea = zarea/runtime.total_seconds()
                 started = "not done yet for offline"
                 if "b0c01" in locals():
                     started = b0c01.started
                 print(f"""
 ___________________________________________________________________
-       Name  = {arg}                           i need to redo this
-       Lenght= {len(histograms[arg])}
-       Time  = {runtime}  (runtime)
+       Name  = {fg.white}{arg}{fg.default}                           i need to redo this
+      Lenght = {len(histograms[arg])}
      Started = {started}
+       Time  = {runtime}  (runtime)
+       Rate  = {myrate:.2f} cps    (if total histogram)
+   RateArea  = {myratea:.2f} cps
     TotalArea= {tarea:16.6f}
     ZoomeArea= {zarea:16.6f}
         zoom = {elo:.1f} ... {ehi:.1f} (Energy)
         zoom = {binlo} ... {binhi} (bins)
 
 """)
 
@@ -1361,16 +1377,18 @@
                         deadttot = ascgeneric.asc_stat_print(ascdf_chan, TIMEWIN_US,  filename = ascfilename,  TRGHOLD = TRGHOLD)
 
                     else:
                         ascgeneric.asc_stat_print(ascdf, TIMEWIN_US,  filename = ascfilename, TRGHOLD = TRGHOLD)
 
                 if cmd.find("ti")==0:  # time histogram
                     if ascdf_chan is not None:
-                        if len(canvases)>0:
-                            arg = list(canvases.keys())[0].split("c_")[-1]
+                        #if len(canvases)>0:
+                        if "c_energy" in canvases.keys():
+                            arg = "energy"
+                            #arg = list(canvases.keys())[0].split("c_")[-1]
                             binlo = histograms[arg].GetXaxis().GetFirst()
                             binhi = histograms[arg].GetXaxis().GetLast()
                             elo = bin2ene(binlo, histograms[arg])
                             ehi = bin2ene(binhi, histograms[arg])
                         else:
                             binlo = 0
                             binhi = 99999
@@ -1478,14 +1496,17 @@
             if arg=="":
                 select_histo_to_load(  folder = config.CONFIG[target]['data_folder'] ) # load_txt()
                 print(f"i.. {fg.cyan} LOAD TXT WITH NUMBER like:    l1  l2 l3 ...  {fg.default}")
             else:
                 ii = arg# for ii in arg: ONE ASC / SPECTRUM AT A TIME....for ii in arg:
                 select_histo_to_load( ii , folder = config.CONFIG[target]['data_folder']) # load_txt() # all that are given in argument l67
                 limits_calib = histograms[f"s{ii}"].GetXaxis().GetXmin(),histograms[f"s{ii}"].GetXaxis().GetXmax()
+                print("D... limits calib:", limits_calib)
+                if limits_calib[0]==0:
+                    histograms[f"s{ii}"].SetTitle(  histograms[f"s{ii}"].GetTitle()+"; channels" )
 
 
         # ********************** CMD ***********************************
         elif cmd == "q":   # ***CMD***  QUIT  ======= q
             print("i... just q: doing exit...")
             # immediate
             config.CONFIG["poll_time"] = 1
```

### Comparing `gregory_online-0.3.1/gregory_online/ascgeneric.py` & `gregory_online-0.3.3/gregory_online/ascgeneric.py`

 * *Files 2% similar despite different names*

```diff
@@ -522,15 +522,15 @@
       2nd phase - SZ and DZ - make one event from these PILEUPs
       3rd phase - create
 
     #len_zeroes,len_dzeroes,len_szeroes,len_izeroes,len_stazeroes,zoutput = ascgeneric.pd_detect_zeroes(df1, chan, TIMEWIN_US=4.48) # df1[ (df1.E==0) ]
     #print(zoutput)
 
     """
-    print( f"D... detection of zeroes: WINDOW == {bg.red}{fg.white} {TIMEWIN_US} us {bg.default}{fg.default}")
+    print( f"D... detection of zeroes: WINDOW == {bg.red}{fg.white} {TIMEWIN_US:.1f} us {bg.default}{fg.default}")
 
 
 
     # vycisteny kanal, ----------------------------------- DFZ
     # I PREPARE SEVERAL VIEWS : only this channel :
     dfz = df[:-1] # WHY????????????
     chan_available = df['ch'].unique()
@@ -540,15 +540,15 @@
         return None
     channel = chan_available[0]
     #index_names = dfz[  (dfz.ch!=channel)].index
     #dfz = dfz.drop(  index_names )
     zeroes = len(  dfz.loc[ (dfz.E==0) ] )
     #print( f" ... TOTAL ZEROES  = {zeroes}")
 
-    # same as dfz for the moment -------------------------- DFALONE
+    # same as dfz for the moment -------------------------- DFALONE IS ALONE !!!!!!!!!!
     dfalone = df # drop the close (cluster) events to count standalones
     index_names = dfalone[ (dfalone.ch!=channel)].index
     dfalone = dfalone.drop( index_names )
     # STANDALONE EVENTS  - drop all events close to another event
     index_names = dfalone[ (dfalone.dtus<=TIMEWIN_US) | (dfalone.dtuspr<=TIMEWIN_US)  ].index
     dfalone = dfalone.drop( index_names) # NOT inplace, else it changes the df!!! # LAST REDEFINITION ALONE
 
@@ -585,14 +585,27 @@
     t1 = df['time'].max()
     t0 = df['time'].min()
     rate = len(df)/(t1-t0)
     # ---------------
     wind_erlang = erlang.erlang_cum(float(TIMEWIN_US)*1e-6, rate, 1)*100  # in %    bellow window 4.48us
     trgh_erlang = erlang.erlang_cum(float(TRGHOLD)*1e-6, rate, 1)*100  # in %    bellow window 4.48us
 
+    satun_n_ch = None # n saturations
+    Tsatu_ch = None # time max in satu
+    Tsatu_pr = None # percent max in satu
+    if 'extras' in df:
+        #print(f"D... extras    present: {df1['extras'].unique()}... 1..satur,3..roll,4..reset,8..fake" )
+        satu_n_ch = len(df.loc[ (df['extras']&1)!=0] )
+        Tsatu_ch = df.loc[ (df['extras']&1)!=0]["prev_satu"].sum()/1e+6   # in sec...
+        Tsatu_pr = 100*Tsatu_ch/(t1-t0)
+        #print(f"D... SATURATIONS {satu_n_ch} total: {Tsatu_ch} sec. at maximum")
+        #print(f"D... SATURATIONS {satu_n_ch} total: {100*Tsatu_ch/interval:.2f} % at maximum")
+
+        #print(f"D... number of saturations: ",len( df.loc[ (df['extras']&1)==1] ) , f" {Tsatu_ch:.2f} sec. at max;  {Tsatu_pr:.2f} % at max"   )
+
 
     output = f"""________________________________________________________________________
  {filename:40s}        {t0:.2f} ... {t1:.2f} sec.
 ________________________________________________________________________
     D... total    events (chan={channel}) = {len(df):8d}
     D... isolated events (chan={channel}) = {isoevents:8d}
     D... clusterd events (chan={channel}) = {len(df)-isoevents:8d}  (in {nclusters} clusters)
@@ -607,14 +620,16 @@
     D... single   zeroes (chan={channel}) = {szeroes:8d} (E-0)  /{100*szeroes/len(df):.2f} %/
     D... double   zeroes (chan={channel}) = {dzeroes:8d} (0-0)  /{2*100*dzeroes/len(df):.2f} %/ {fg.yellow}/?clusters/{fg.default}
     D... ilogic   zeroes (chan={channel}) = {izeroes:8d} (0-E)  /should be 0/
     D... double   E      (chan={channel}) = {dnonzeroes:8d} (E-E)  /should be 0/
 
     D... blind erlang    (chan={channel}) = {wind_erlang:.2f} %  {fg.green}/DT from ERLANG/{fg.default} {TIMEWIN_US:.1f} us
     D... blind erlang    (chan={channel}) = {trgh_erlang:.2f} %  {fg.green}/DT from ERLANG/{fg.default} {TRGHOLD:.1f} us
+
+    D... n_sat,tmax_sat  (chan={channel}) = {satu_n_ch:8d}, {Tsatu_ch:.2f} s. {Tsatu_pr:.1f} %  {fg.green}/DT from ERLANG/{fg.default} {TRGHOLD:.1f} us
 all blind10==lost ~~ all zeroes+blind0.5==lost; maybe some 0 are exagerated @ortec; NEED [satur-median] estimation HERE
 _______________________________________________________________________________
 """
     # {fg.red}D... double zeroes (chan={channel}) = {dzeroes:8d} ~  {2*dzeroes/len(df)*100:5.2f}% ( % counted correctly 2x){fg.default}
     # D... => zrs@HigherClusters  = {zeroes-isozeroes-2*dzeroes:8d}  (zeroes in longer than 2 clusters)
     # D... ______________________ end of zero detection
     # D...  window {TIMEWIN_US} us   ....  crutial for correct double zeroes detection
@@ -757,25 +772,30 @@
     print("D... max E", maxc)
 
     #chan0 = df1.ch.min()
     chan = df1.ch.max()
 
     if calibration is not None:
         units = "[keV]"
+        print("D... calibration",calibration)
+        if calibration[0]==1 and calibration[1]==0:
+            units  = "(chan)"
+    else:
+        units = "[chan]"
     hisene = column_to_newhisto(df1['E'].loc[(df1.E!=0)],
                                 binmax=maxc, himax=maxc,
                                 hname = f"{hname}; Energy {units}; channel {chan}", calibration = calibration)
     hisene.Print()
     return hisene
 
 
 def histo_time( df1 , hname = 'time' , lowe=-99999, hie=99999 ):
     maxc = df1.time.max()
     c = df1.ch.max()
     hist = column_to_newhisto(  df1['time'].loc[ (df1.E!=0) & (df1.E>=lowe) & (df1.E<=hie) ],
-                                       binmax=2**6, himax=maxc,
+                                       binmax=int(maxc)+1, himax=maxc,
                                   hname = f"{hname}; time [s]; chan {c}")
 
 
     #print( df1.loc[ (df1.E!=0) & (df1.E>=lowe) & (df1.E<=hie) ] )
     hist.Print()
     return hist
```

### Comparing `gregory_online-0.3.1/gregory_online/config.py` & `gregory_online-0.3.3/gregory_online/config.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/data/Am241.svg` & `gregory_online-0.3.3/gregory_online/data/Am241.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/data/Cm247.png` & `gregory_online-0.3.3/gregory_online/data/Cm247.png`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/data/Np237.svg` & `gregory_online-0.3.3/gregory_online/data/Np237.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/data/Pa231.svg` & `gregory_online-0.3.3/gregory_online/data/Pa231.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/data/Pu239.svg` & `gregory_online-0.3.3/gregory_online/data/Pu239.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/data/Th232.svg` & `gregory_online-0.3.3/gregory_online/data/Th232.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/data/U235.svg` & `gregory_online-0.3.3/gregory_online/data/U235.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/data/U238.svg` & `gregory_online-0.3.3/gregory_online/data/U238.svg`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/data/decay_lara.parquet` & `gregory_online-0.3.3/gregory_online/data/decay_lara.parquet`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/data/testrebin.py` & `gregory_online-0.3.3/gregory_online/data/testrebin.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/decay_db.py` & `gregory_online-0.3.3/gregory_online/decay_db.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/dpp2jpg.py` & `gregory_online-0.3.3/gregory_online/dpp2jpg.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/erlang.py` & `gregory_online-0.3.3/gregory_online/erlang.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/fetchnp.py` & `gregory_online-0.3.3/gregory_online/fetchnp.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/histo_analyze.py` & `gregory_online-0.3.3/gregory_online/histo_analyze.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 And send data to influx (stored at ~/.seread.discover8086 ++ )
 """
 from fire import Fire
 #from tdb_io import influxwrite
 import tdb_io
 
 # let's see if we can fit
-from pyfromroot import  prun
+try:
+    from pyfromroot import  prun
+except:
+    print("X... pyfrom root not imported.... ")
 
 import datetime as dt
 import time
 
 from console import fg,bg
 
 
@@ -135,17 +138,20 @@
     """
     input: TH1
     """
     hname = h.GetName()
     print("i... fitting gauss in the range")
 
     # zoom?
-    res = prun.loadpy("fit",f"{hname} gpol1", canvas = canvas)
-
-    if res['area']<0: res['area']=-res['area']
+    if "prun" in locals() or "prun" in globals() :
+        res = prun.loadpy("fit",f"{hname} gpol1", canvas = canvas)
+        if res['area']<0: res['area']=-res['area']
+    else:
+        print("X... pyfromroot NOT IMPORTED")
+        res = None
 
     if abs(res['diff_fit_int_proc'])>1:
         print(f"X...  {fg.yellow}BAD DESCRIPTION - DIFF MORE THAN 1%{fg.default} ")
         time.sleep(0.2)
 
     if not( res['noerror']):
         print(f"X...  {fg.red}BAD DESCRIPTION - SOME ERROR OF FIT{fg.default}")
```

### Comparing `gregory_online-0.3.1/gregory_online/histo_displ.py` & `gregory_online-0.3.3/gregory_online/histo_displ.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/histo_global_cont.py` & `gregory_online-0.3.3/gregory_online/histo_global_cont.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/histo_io.py` & `gregory_online-0.3.3/gregory_online/histo_io.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/histo_np_ops.py` & `gregory_online-0.3.3/gregory_online/histo_np_ops.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/key_enter.py` & `gregory_online-0.3.3/gregory_online/key_enter.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/topbar.py` & `gregory_online-0.3.3/gregory_online/topbar.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online/utils.py` & `gregory_online-0.3.3/gregory_online/utils.py`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/gregory_online.egg-info/PKG-INFO` & `gregory_online-0.3.3/gregory_online.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gregory-online
-Version: 0.3.1
+Version: 0.3.3
 Summary: Online watching HTTP server of ROOT on port 9009
 Author: me
 Author-email: jaromrax@gmail.com
 License: GPL2
 Description-Content-Type: text/markdown
 
 Project gregory~online~
```

### Comparing `gregory_online-0.3.1/gregory_online.egg-info/SOURCES.txt` & `gregory_online-0.3.3/gregory_online.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gregory_online-0.3.1/setup.py` & `gregory_online-0.3.3/setup.py`

 * *Files identical despite different names*

