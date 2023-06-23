# Comparing `tmp/tahoma-2.2.8.tar.gz` & `tmp/tahoma-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahoma-2.2.8.tar", last modified: Sun Jun 11 12:11:44 2023, max compression
+gzip compressed data, was "tahoma-2.2.9.tar", last modified: Fri Jun 23 17:54:40 2023, max compression
```

## Comparing `tahoma-2.2.8.tar` & `tahoma-2.2.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-11 12:11:44.448171 tahoma-2.2.8/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma-2.2.8/LICENSE
--rwxrwx---   0 neptune   (1000) neptune   (1000)      142 2023-02-21 14:35:21.000000 tahoma-2.2.8/MANIFEST.in
--rwxrwx---   0 neptune   (1000) neptune   (1000)     7627 2023-06-11 12:11:44.448282 tahoma-2.2.8/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)     6965 2023-06-11 12:11:15.000000 tahoma-2.2.8/PYPI_README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     6964 2023-06-11 12:10:58.000000 tahoma-2.2.8/README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1201 2023-02-21 21:29:00.000000 tahoma-2.2.8/pyproject.toml
--rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-02-21 17:24:01.000000 tahoma-2.2.8/requirements.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-06-11 12:11:44.448613 tahoma-2.2.8/setup.cfg
--rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma-2.2.8/setup.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-11 12:11:44.443122 tahoma-2.2.8/tahoma/
--rwxrwx---   0 neptune   (1000) neptune   (1000)      134 2023-02-21 18:24:33.000000 tahoma-2.2.8/tahoma/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       22 2023-06-07 10:02:57.000000 tahoma-2.2.8/tahoma/__version__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)    11260 2023-06-07 10:08:50.000000 tahoma-2.2.8/tahoma/get_devices_url.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-11 12:11:44.446635 tahoma-2.2.8/tahoma/icons/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.8/tahoma/icons/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)    21160 2023-02-15 08:39:56.000000 tahoma-2.2.8/tahoma/icons/connected_house.png
--rwxrwx---   0 neptune   (1000) neptune   (1000)    29722 2023-02-15 17:48:11.000000 tahoma-2.2.8/tahoma/icons/water heater.png
--rwxrwx---   0 neptune   (1000) neptune   (1000)    46657 2023-06-07 13:12:56.000000 tahoma-2.2.8/tahoma/tahoma.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-11 12:11:44.447126 tahoma-2.2.8/tahoma/temp/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:32:54.000000 tahoma-2.2.8/tahoma/temp/__init__.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-11 12:11:44.447873 tahoma-2.2.8/tahoma/test/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.8/tahoma/test/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma-2.2.8/tahoma/test/test.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-11 12:11:44.445397 tahoma-2.2.8/tahoma.egg-info/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     7627 2023-06-11 12:11:44.000000 tahoma-2.2.8/tahoma.egg-info/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)      517 2023-06-11 12:11:44.000000 tahoma-2.2.8/tahoma.egg-info/SOURCES.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-06-11 12:11:44.000000 tahoma-2.2.8/tahoma.egg-info/dependency_links.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       46 2023-06-11 12:11:44.000000 tahoma-2.2.8/tahoma.egg-info/entry_points.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-06-11 12:11:44.000000 tahoma-2.2.8/tahoma.egg-info/requires.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        7 2023-06-11 12:11:44.000000 tahoma-2.2.8/tahoma.egg-info/top_level.txt
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-23 17:54:40.491258 tahoma-2.2.9/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma-2.2.9/LICENSE
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      142 2023-02-21 14:35:21.000000 tahoma-2.2.9/MANIFEST.in
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     7707 2023-06-23 17:54:40.491365 tahoma-2.2.9/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     7045 2023-06-23 17:52:14.000000 tahoma-2.2.9/PYPI_README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     7044 2023-06-23 17:52:07.000000 tahoma-2.2.9/README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1201 2023-02-21 21:29:00.000000 tahoma-2.2.9/pyproject.toml
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       50 2023-06-23 17:52:37.000000 tahoma-2.2.9/requirements.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-06-23 17:54:40.491734 tahoma-2.2.9/setup.cfg
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma-2.2.9/setup.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-23 17:54:40.485951 tahoma-2.2.9/tahoma/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      134 2023-02-21 18:24:33.000000 tahoma-2.2.9/tahoma/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2023-06-23 17:29:50.000000 tahoma-2.2.9/tahoma/__version__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    11260 2023-06-07 10:08:50.000000 tahoma-2.2.9/tahoma/get_devices_url.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-23 17:54:40.489594 tahoma-2.2.9/tahoma/icons/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.9/tahoma/icons/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    21160 2023-02-15 08:39:56.000000 tahoma-2.2.9/tahoma/icons/connected_house.png
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    29722 2023-02-15 17:48:11.000000 tahoma-2.2.9/tahoma/icons/water heater.png
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    48166 2023-06-23 17:45:50.000000 tahoma-2.2.9/tahoma/tahoma.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-23 17:54:40.490108 tahoma-2.2.9/tahoma/temp/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:32:54.000000 tahoma-2.2.9/tahoma/temp/__init__.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-23 17:54:40.490936 tahoma-2.2.9/tahoma/test/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.9/tahoma/test/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma-2.2.9/tahoma/test/test.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-06-23 17:54:40.488341 tahoma-2.2.9/tahoma.egg-info/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     7707 2023-06-23 17:54:40.000000 tahoma-2.2.9/tahoma.egg-info/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      517 2023-06-23 17:54:40.000000 tahoma-2.2.9/tahoma.egg-info/SOURCES.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-06-23 17:54:40.000000 tahoma-2.2.9/tahoma.egg-info/dependency_links.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       46 2023-06-23 17:54:40.000000 tahoma-2.2.9/tahoma.egg-info/entry_points.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       50 2023-06-23 17:54:40.000000 tahoma-2.2.9/tahoma.egg-info/requires.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        7 2023-06-23 17:54:40.000000 tahoma-2.2.9/tahoma.egg-info/top_level.txt
```

### Comparing `tahoma-2.2.8/LICENSE` & `tahoma-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.8/PKG-INFO` & `tahoma-2.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma
-Version: 2.2.8
+Version: 2.2.9
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma/issues
 Keywords: tahoma,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 It was created with Tahoma but can also works with Somfy Connectivity Kit, Connexoon, Cozytouch
 
 
 ![Somfy](https://www.voletsdusud.com/wp-content/uploads/2018/04/logo-tahoma.jpg)
 
 
 
-
+![GifTahoma.gif](https://github.com/pzim-devdata/tahoma/blob/main/GifTahoma.gif)
 
 # Install the main package :
 
 
 Install tahoma :
 
 #########################################
```

### Comparing `tahoma-2.2.8/PYPI_README.md` & `tahoma-2.2.9/PYPI_README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 It was created with Tahoma but can also works with Somfy Connectivity Kit, Connexoon, Cozytouch
 
 
 ![Somfy](https://www.voletsdusud.com/wp-content/uploads/2018/04/logo-tahoma.jpg)
 
 
 
-
+![GifTahoma.gif](https://github.com/pzim-devdata/tahoma/blob/main/GifTahoma.gif)
 
 # Install the main package :
 
 
 Install tahoma :
 
 #########################################
```

### Comparing `tahoma-2.2.8/README.md` & `tahoma-2.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 It was created with Tahoma but can also works with Somfy Connectivity Kit, Connexoon, Cozytouch
 
 
 ![Somfy](https://www.voletsdusud.com/wp-content/uploads/2018/04/logo-tahoma.jpg)
 
 
 
-
+![GifTahoma.gif](https://github.com/pzim-devdata/tahoma/blob/main/GifTahoma.gif)
 
 # Install the main package :
 
 
 Install tahoma :
 
 #########################################
```

### Comparing `tahoma-2.2.8/pyproject.toml` & `tahoma-2.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.8/tahoma/get_devices_url.py` & `tahoma-2.2.9/tahoma/get_devices_url.py`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.8/tahoma/icons/connected_house.png` & `tahoma-2.2.9/tahoma/icons/connected_house.png`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.8/tahoma/icons/water heater.png` & `tahoma-2.2.9/tahoma/icons/water heater.png`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.8/tahoma/tahoma.py` & `tahoma-2.2.9/tahoma/tahoma.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,17 +17,40 @@
 import time
 from pyoverkiz.const import SUPPORTED_SERVERS
 from pyoverkiz.client import OverkizClient
 from pyoverkiz.enums import OverkizCommand
 from pyoverkiz.models import Command
 from pyoverkiz.models import Scenario
 from tahoma import __version__
+import requests
+
+version_number=str(__version__.__version__)
+get_devices_url="from tahoma import get_devices_url"
+
+url_releases = 'https://api.github.com/repos/pzim-devdata/tahoma/releases'
+
+def check_last_release (show='y'):
+    try:
+        headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64)'}
+        response = requests.get(url_releases, headers=headers)
+        releases = response.json()
+        last_release = releases[0]['tag_name']
+        if str(last_release.lower()) == str(version_number).lower():
+            if show == 'y' :
+                print(" You are using the last version of Tahoma : " + str(last_release.lower()))
+        else :
+            print(" Last version of Tahoma is : " + str(last_release.lower()) + " and you are using the version : " + str(version_number).lower())
+            print(" Pypi version : sudo python3 -m pip install -U tahoma or pipx upgrade tahoma")
+            print(" Github version : https://github.com/pzim-devdata/tahoma/releases/latest/download/tahoma.zip")
+    except : pass
+
+check_last_release ('n')
 
 def main():
-    version ='tahoma - Version '+ str(__version__.__version__)+' - by @pzim-devdata'
+    version ='tahoma - Pypi version '+ str(__version__.__version__)+' - by @pzim-devdata'
 
     icon_app = os.path.dirname(os.path.abspath(__file__))+'/icons/connected_house.png'
     icon_chauffe_eau=os.path.dirname(os.path.abspath(__file__))+'/icons/water heater.png'
 
     passwd_file = os.path.dirname(os.path.abspath(__file__))+'/temp/identifier_file.txt'
 
     list_of_tahoma_devices = os.path.dirname(os.path.abspath(__file__))+'/temp/list_of_tahoma_devices.txt'
@@ -63,30 +86,30 @@
         f.close()
     except FileNotFoundError:
         serverchoice = "somfy_europe"
 
     def info():
         print( "" )
         print( "      ***************************************************************      " )
-        print( "------*     Tahoma version : "+version+"     *-------" )
+        print( "      Tahoma version : "+version+"     " )
         print( "      ***************************************************************        " )
-        print( "              sudo python3 -m pip install tahoma-pzim -U" )
+        print( "              sudo python3 -m pip install tahoma -U" )
         print( "                   https://pypi.org/project/tahoma/" )
         print( "                 https://github.com/pzim-devdata/tahoma" )
         print( "                          contact@pzim.fr" )
         print( "" )
         print( " USAGE : tahoma [ACTION] [CATEGORY] [NAME]" )
         print( "")
         print( " - List of possible ACTIONS : \n "+str(list_actions) )
         print( " - Liste des ACTIONS possibles : \n "+str(list_actions_french) )
         print( "" )
         print( " - List of possible CATEGORIES : \n "+str(list_categories) )
         print( " - Liste des CATEGORIES possibles : \n "+str(list_categories_french) )
         print( "" )
-        print( ' - List of available NAMES : tahoma --list-names \n - Liste des NOMS possibles : tahoma --list-names-french \n You must provide a part of the name you have assigned to the device in the Tahoma App. \n It must be a single and unic word, not taken by another device of the same category !\n For instance if you have two devices called <Alarm 1> and <Alarm 2> you will need to choose <2> as device [NAME] for <Alarm 2> and not <Alarm>).\n You can also use the full <NAME> with [""].\n For instance ["Alarm 2"]\n See tahoma --list or tahoma --help for info.')
+        print( ' - List of available NAMES : tahoma --list-names \n - Liste des NOMS possibles : tahoma --list-names-french \n You must provide a part of the name you have assigned to the device in the Tahoma App. \n It must be a single and unique word, not taken by another device of the same category !\n For instance if you have two devices called <Alarm 1> and <Alarm 2> you will need to choose <2> as device [NAME] for <Alarm 2> and not <Alarm>).\n You can also use the full NAME with [""].\n For instance ["Alarm 2"]\n See tahoma --list or tahoma --help for info.')
         print( "" )
         print( " You must provide at least 3 arguments" )
         print( " For instance : python3 tahoma open shutter kitchen")
         print( "\n You can close a shutter or a sunscreen to a specific level (IO protocols only)")
         print( " For instance :python3 tahoma 25 shutter kitchen. It will open the shutter to 75% or close it to 25%" )
         print( "" )
         print( " You can also provide, as many as you wish, orders on the same line." ) 
@@ -105,14 +128,17 @@
         print( "" )
         print( "                     To get help : tahoma -h " )
         print( "")
         print( "                   To show this sceen : tahoma -i" )
         print( "" )
         print( "      Il existe une aide en français : tahoma --help-french " )
         print( " ********************************************************************        " )
+        print( "" )
+        check_last_release ()
+        print( "" )
         print( "    Open your terminal in full screen mode to have a better view \n" )
     #    try :
     #        os.system("wmctrl -r ':ACTIVE:' -b toggle,fullscreen")
     #        print( " \n          <--- Appuyez sur F11 to close fullscreen --->\n")
     #        print( " \n             <--- Press F11 to close fullscreen --->\n")
     #    except Exception :
     #       print( "       Open your terminal in full screen to have a better view ")
@@ -130,15 +156,15 @@
             except IndexError: 
                 info()
                 exit()
 
     for arg in sys.argv :
         if arg == '-g' or arg == '--getlist' :
             try :
-                from tahoma import get_devices_url
+                exec(get_devices_url)
                 exit()
             except Exception as e: 
                 print(e)
 #                exec((open(os.path.dirname(os.path.abspath(__file__))+"/get_devices_url.py")).read())
                 exit()
 
     for arg in sys.argv :
@@ -208,20 +234,20 @@
                     print( passwd_file+" is removed" )
                 except : 
                     print("The file was already removed")
             exit()
 
     for arg in sys.argv :
         if arg == '-h' or arg == '--help' :
-            print("tahoma -h, --help : "+version+"\n\nUsage:\n tahoma <ACTION> <CATEGORY> <NAME> \n\n You must provide at least three arguments\n For instance : tahoma open shutter kitchen or tahoma ouvrir volet cuisine\n\n You can close a shutter or a sunscreen to a specific level (IO protocols only)\n For instance : tahoma 25 shutter kitchen. It will open the shutter to 75% or close it to 25%\n\n You can also provide, as many as you wish, orders on the same line\n Tahoma will execute all orders one by one in the same process ;-)\n For instance : tahoma open shutter kitchen arm alarm garden on plug room wait train garestation\n\nHelp options :\n -h,   --help                      Show this help\n -hf,  --help-french               Show this help in french\n -i,   --info                      Show more info\n\nPlugin options :\n -v,   --version                   Show the version of the plugin\n -c,   --configure                 To configure the plugin and store login and password in a text file which is located here : "+passwd_file+" Use with sudo !\n -u,   --username                  If you don't want to store the login, you can provide the mail-address with this option\n -p,   --password                  If you don't want to store the password, you can provide it with this option\n -g,   --getlist                   Download the list of devices and store them here : "+list_of_tahoma_devices+" Use with sudo !\n -l,   --list                      Show the complet list of devices installed\n -la,  --list-actions              Show the list of possible ACTIONS by CATEGORIES\n -lc,  --list-categories           Show all supported CATEGORIES of devices\n -lnf, --list-names                Show all installed devices by there NAMES\n\nCommand options :\n wait for <seconds>                Tahoma will wait for <seconds> seconds to execute next action\n sleep for <seconds>\n")
+            print("tahoma -h, --help : "+version+"\n\nUsage:\n tahoma ACTION CATEGORY NAME \n\n You must provide at least three arguments\n For instance : tahoma open shutter kitchen or tahoma ouvrir volet cuisine\n\n You can close a shutter or a sunscreen to a specific level (IO protocols only)\n For instance : tahoma 25 shutter kitchen. It will open the shutter to 75% or close it to 25%\n\n You can also provide, as many as you wish, orders on the same line\n Tahoma will execute all orders one by one in the same process ;-)\n For instance : tahoma open shutter kitchen arm alarm garden on plug room wait train garestation\n\nHelp options :\n -h,   --help                      Show this help\n -hf,  --help-french               Show this help in french\n -i,   --info                      Show more info\n\nPlugin options :\n -v,   --version                   Show the version of the plugin\n -c,   --configure                 To configure the plugin and store login and password in a text file which is located here : "+passwd_file+" Use with sudo !\n -u,   --username                  If you don't want to store the login, you can provide the mail-address with this option\n -p,   --password                  If you don't want to store the password, you can provide it with this option\n -g,   --getlist                   Download the list of devices and store them here : "+list_of_tahoma_devices+" Use with sudo !\n -l,   --list                      Show the complet list of devices installed\n -la,  --list-actions              Show the list of possible ACTIONS by CATEGORIES\n -lc,  --list-categories           Show all supported CATEGORIES of devices\n -lnf, --list-names                Show all installed devices by there NAMES\n\nCommand options :\n wait for <seconds>                Tahoma will wait for <seconds> seconds to execute next action\n sleep for <seconds>\n")
             exit()
 
     for arg in sys.argv :
         if arg == '-hf' or arg == '--help-french' :
-            print("tahoma -h --help : "+version+"\n\nUsage:\n tahoma <ACTION> <CATEGORIE> <NOM> \n\n Vous devez fournir au moins trois arguments\n Par exemple : tahoma ouvrir volet cuisine ou tahoma open shutter kitchen\n\n Vous pouvez fermer des rideaux ou des volets à un niveau precis (Seulement pour les équipements utilisant le protocole IO)\n Par exemple : tahoma 25 volet cuisine. Les volets vont s'ouvrir de 75% ou se fermer de 25%\n\n Vous pouvez aussi spécifier autant de commandes que vous le souhaitez sur la même ligne :\n Tahoma va executer chaque commande l'une aprés l'autre durant le même processus\n Par exemple : tahoma ouvrir volet cuisine confort chauffage salon\n\nOptions de l’aide :\n -h, --help                        Affiche les options de l’aide en anglais\n\nOptions de l’application :\n -v, --version                     Affiche la version de l’application\n -i, --info                        Afficher plus d'infos sur tahoma\n -c, --configure                   Renseigner l'identifiant et le mot de passe dans un fichier texte pour ne pas devoir les renseigner à chaque fois. Le fichier texte se situe dans : "+passwd_file+" Utiliser sudo !\n -u, --username                    Renseigner le nom d'utilisateur\n -p, --password                    Renseigner le mot de passe de Somfy-connect\n -g, --getlist                     Télécharge la liste des équipements et la stocke dans "+list_of_tahoma_devices+" Utiliser sudo !\n -l, --list                        Affiche la liste téléchargée des équipements\n -laf, --list-actions-french       Affiche la liste des ACTIONS possibles en français par CATEGORIES\n -lcf, --list-categories-french    Affiche toutes les CATEGORIES d'équipements pris en charge en français\n -lnf, --list-names-french         Affiche les NOMS des équipements installés par categories en français\n\nOptions de commande :\n attendre pendant <secondes>       Tahoma attendra <secondes> secondes avant d'éxécuter la commande suivante\n")
+            print("tahoma -h --help : "+version+"\n\nUsage:\n tahoma ACTION CATEGORIE NOM \n\n Vous devez fournir au moins trois arguments\n Par exemple : tahoma ouvrir volet cuisine ou tahoma open shutter kitchen\n\n Vous pouvez fermer des rideaux ou des volets à un niveau precis (Seulement pour les équipements utilisant le protocole IO)\n Par exemple : tahoma 25 volet cuisine. Les volets vont s'ouvrir de 75% ou se fermer de 25%\n\n Vous pouvez aussi spécifier autant de commandes que vous le souhaitez sur la même ligne :\n Tahoma va executer chaque commande l'une aprés l'autre durant le même processus\n Par exemple : tahoma ouvrir volet cuisine confort chauffage salon\n\nOptions de l’aide :\n -h, --help                        Affiche les options de l’aide en anglais\n\nOptions de l’application :\n -v, --version                     Affiche la version de l’application\n -i, --info                        Afficher plus d'infos sur tahoma\n -c, --configure                   Renseigner l'identifiant et le mot de passe dans un fichier texte pour ne pas devoir les renseigner à chaque fois. Le fichier texte se situe dans : "+passwd_file+" Utiliser sudo !\n -u, --username                    Renseigner le nom d'utilisateur\n -p, --password                    Renseigner le mot de passe de Somfy-connect\n -g, --getlist                     Télécharge la liste des équipements et la stocke dans "+list_of_tahoma_devices+" Utiliser sudo !\n -l, --list                        Affiche la liste téléchargée des équipements\n -laf, --list-actions-french       Affiche la liste des ACTIONS possibles en français par CATEGORIES\n -lcf, --list-categories-french    Affiche toutes les CATEGORIES d'équipements pris en charge en français\n -lnf, --list-names-french         Affiche les NOMS des équipements installés par categories en français\n\nOptions de commande :\n attendre pendant <secondes>       Tahoma attendra <secondes> secondes avant d'éxécuter la commande suivante\n")
             exit()
 
     for arg in sys.argv :
         if arg == '-lc' or arg == '--list-categories' :
             print( "tahoma can control this type of devices's categories :\n"+str(list_categories))
             exit()
 
@@ -243,15 +269,15 @@
                     master_list = content.split("\n")
                     master_list.remove('')
                     for i in master_list :
                         bad_name.append(i.split(",")[0])
                     print("\nHere is the list of the installed devices for the "+category.upper()+" category :\n"+str(bad_name))
                 except Exception as e:
                     print("\nCan't obtain any device from the "+category.upper()+" category\nDid you downloaded the list of Tahoma's devices ?\nIf not, execute tahoma --getlist \nFor more info execute tahoma -h")
-            print( "\nYou must provide a part of the <NAME> as argument \nIt must be a single and unic word, not taken by another device of the same category !\nFor instance : <Kitchen>\nIf you have two devices called <Alarm 1> and <Alarm 2> you will need to choose <2> as device <NAME> for <Alarm 2> and not <Alarm>. See tahoma --list or tahoma --help for more info")
+            print( '\nYou must provide a part of the NAME as argument \nt must be a single and unique word, not taken by another device of the same category !\n For instance if you have two devices called <Alarm 1> and <Alarm 2> you will need to choose <2> as device [NAME] for <Alarm 2> and not <Alarm>).\n You can also use the full NAME with [""].\n For instance ["Alarm 2"]\n See tahoma --list or tahoma --help for info.')
             exit()
 
     for arg in sys.argv :
         if arg == '-lnf' or arg == '--list-names-french' :
             print("\nPensez à exécuter la commande : tahoma --getlist pour vous assurer que la liste des équipements est complète")
             i=-1
             for i in range(-1,len(list_categories)-1) :
@@ -266,15 +292,15 @@
                     master_list.remove('')
                     for j in master_list :
                         bad_name.append(j.split(",")[0])
                     print("\nVoici la liste des équipements installés pour la catégorie "+list_categories_french[i].upper()+" :\n"+str(bad_name))
                 except Exception as e:
                     print(e)
                     print("\nImpossible d'obtenir la liste des équipements pour la catégorie "+list_categories_french[i].upper()+"\nAvez-vous téléchargé la liste des équipements installés ?\nSinon executez la commande : tahoma --getlist \nPour plus d'info : tahoma --help-french")
-            print( "\nVous devez fournir une partie du <NOM> comme argument \nCe NOM ne doit pas être utilisé par un autre équipement de la même categorie !\nSi vous avez deux équipements appelés par ex. <Alarme 1> et <Alarme 2> vous devrez renseigner comme <NOM> seulement <2> pour <Alarme 2> et non <Alarme> Consultez l'aide en français : tahoma --help-french ou tahoma --info pour plus d'informations.")
+            print( "\nVous devez fournir une partie du NOM comme argument \nCe NOM ne doit pas être utilisé par un autre équipement de la même categorie !\nSi vous avez deux équipements appelés par ex. <Alarme 1> et <Alarme 2> vous devrez renseigner comme NOM seulement <2> pour <Alarme 2> et non <Alarme> Consultez l'aide en français : tahoma --help-french ou tahoma --info pour plus d'informations.")
             exit()
 
     for arg in sys.argv :
         if arg == '-la' or arg == '--list-actions' :
             print( "List of actions by categories :")
             for i in range(0,len(list_actions)) :
                 print ( "For the category "+list_categories[i].upper()+" : "+list_actions[i] )
@@ -372,18 +398,18 @@
                         good_name.append(i.split(",")[0])
                 else :
                     if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
                          url.append(i.split(",")[1])
                          too_many_urls.append(i.split(",")[0])
                          good_name.append(i.split(",")[0])
             if len(url)== 0 :
-                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name.\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                print("There is no match. The NAME you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as NAME argument or use [''] with the full name.\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
             if len(url) > 1 :
-                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
+                print("There is more than one match. The NAME you gave is not exact. Choose a UNIQUE part of word from this results as NAME argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
                 exit()
 
             if remove_accent(action).upper() == "OPEN" or remove_accent(action).upper() == "OUVRIR" :
                 fonction = Command(OverkizCommand.OPEN)
             elif remove_accent(action).upper() == 'CLOSE' or remove_accent(action).upper() == "FERMER" :
                 fonction = Command(OverkizCommand.CLOSE)
             elif remove_accent(action).upper() == 'STOP' :
@@ -422,18 +448,18 @@
                         good_name.append(i.split(",")[0])
                 else :
                     if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
                          url.append(i.split(",")[1])
                          too_many_urls.append(i.split(",")[0])
                          good_name.append(i.split(",")[0])
             if len(url)== 0 :
-                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                print("There is no match. The NAME you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as NAME argument or use [''] with the full name\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
             if len(url) > 1 :
-                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
+                print("There is more than one match. The NAME you gave is not exact. Choose a UNIQUE part of word from this results as NAME argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
                 exit()
 
             if remove_accent(action).upper() == "OPEN" or remove_accent(action).upper() == "OUVRIR" :
                 fonction = Command(OverkizCommand.OPEN)
             elif remove_accent(action).upper() == 'CLOSE' or remove_accent(action).upper() == "FERMER" :
                 fonction = Command(OverkizCommand.CLOSE)
             elif remove_accent(action).upper() == 'STOP' :
@@ -482,18 +508,18 @@
                         good_name.append(i.split(",")[0])
                 else :
                     if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
                          url.append(i.split(",")[1])
                          too_many_urls.append(i.split(",")[0])
                          good_name.append(i.split(",")[0])
             if len(url)== 0 :
-                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                print("There is no match. The NAME you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as NAME argument or use [''] with the full name\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
             if len(url) > 1 :
-                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
+                print("There is more than one match. The NAME you gave is not exact. Choose a UNIQUE part of word from this results as NAME argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
                 exit()
 
             if remove_accent(action).upper() == "ON" or remove_accent(action).upper() == "ALLUMER" :
                 fonction = Command(OverkizCommand.ON)
             elif remove_accent(action).upper() == 'OFF' or remove_accent(action).upper() == "ETEINDRE" :
                 fonction = Command(OverkizCommand.OFF)
             else :
@@ -523,18 +549,18 @@
                         good_name.append(i.split(",")[0])
                 else :
                     if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
                          url.append(i.split(",")[1])
                          too_many_urls.append(i.split(",")[0])
                          good_name.append(i.split(",")[0])
             if len(url)== 0 :
-                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                print("There is no match. The NAME you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as NAME argument or use [''] with the full name\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
             if len(url) > 1 :
-                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
+                print("There is more than one match. The NAME you gave is not exact. Choose a UNIQUE part of word from this results as NAME argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
                 exit()
 
             if remove_accent(action).upper() == "ARM" or remove_accent(action).upper() == "ACTIVER" or remove_accent(action).upper() == "ON":
                 fonction = Command(OverkizCommand.ARM)
             elif remove_accent(action).upper() == 'DISARM' or remove_accent(action).upper() == "DESACTIVER" or remove_accent(action).upper() == "OFF" :
                 fonction = Command(OverkizCommand.DISARM)
             elif remove_accent(action).upper() == 'PARTIAL' or remove_accent(action).upper() == "PARTIEL" :
@@ -570,18 +596,18 @@
                         good_name.append(i.split(",")[0])
                 else :
                     if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
                          url.append(i.split(",")[1])
                          too_many_urls.append(i.split(",")[0])
                          good_name.append(i.split(",")[0])
             if len(url)== 0 :
-                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                print("There is no match. The NAME you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as NAME argument or use [''] with the full name\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
             if len(url) > 1 :
-                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
+                print("There is more than one match. The NAME you gave is not exact. Choose a UNIQUE part of word from this results as NAME argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
                 exit()
 
             if remove_accent(action).lower() == "comfort" or remove_accent(action).lower() == "confort" :
                 fonction = Command(OverkizCommand.SET_HEATING_LEVEL,['comfort'])
             elif remove_accent(action).lower() == 'comfort-1' or remove_accent(action).lower() == "confort-1" :
                 fonction = Command(OverkizCommand.SET_HEATING_LEVEL,['comfort-1'])
             elif remove_accent(action).lower() == 'comfort-2' or remove_accent(action).lower() == "confort-2" :
@@ -619,18 +645,18 @@
                 else :
                     if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
                          url.append(i.split(",")[1])
                          too_many_urls.append(i.split(",")[0])
                          good_name.append(i.split(",")[0])
 
             if len(url)== 0 :
-                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                print("There is no match. The NAME you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as NAME argument or use [''] with the full name\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
             if len(url) > 1 :
-                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIC part of word from this results as <NAME> argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
+                print("There is more than one match. The NAME you gave is not exact. Choose a UNIQUE part of word from this results as NAME argument or use [''] with the full name : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
                 exit()
 
             
             #fonction = Command(OverkizCommand.SET_HEATING_LEVEL,['comfort'])
             #exec_id = await client.execute_scenario(device_url)
 
             str1 = " "
@@ -668,15 +694,15 @@
                     if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
                          url.append(i.split(",")[1])
                          too_many_urls.append(i.split(",")[0])
                          good_name.append(i.split(",")[0])
                          command_state.append(i.split(",")[3])
 
             if len(url)== 0 :
-                print("There is no match. The <NAME> you gave is not exact or it's impossible to retrieve the state of '"+args.name+"'. \nPerhaps because it's RTS protocol and not IO. \n\nHere are supported devices : "+str(bad_name)+" \n\nChoose a UNIC part of word from this supported devices as <NAME> argument or if you want to indicate the exact <NAME> use square brackets AND quotation mark : ['<NAME>'] . \nFor exemple if you want to use the <NAME> <Heater Room 6> the syntax should be : ['Heater Room 6']. \n\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                print("There is no match. The NAME you gave is not exact or it's impossible to retrieve the state of '"+args.name+"'. \nPerhaps because it's RTS protocol and not IO. \n\nHere are supported devices : "+str(bad_name)+" \n\nChoose a UNIQUE part of word from this supported devices as NAME argument or if you want to indicate the exact NAME use square brackets AND quotation mark : ['NAME'] . \nFor exemple if you want to use the NAME <Heater Room 6> the syntax should be : ['Heater Room 6']. \n\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
                 exit()
 
 #            command_state=[]
 #            time.sleep(1)
 #            for i in master_list :
 #                if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
 #                     command_state.append(i.split(",")[3])
@@ -692,43 +718,47 @@
             print( "\nThe <CATEGORY> you have entered doesn't exist.\nChoose one of this category : "+str(list_categories)+"\nUse tahoma --help-categories or tahoma --list-categories for info")
 
 
     ##########################MAIN FUNCTION
 
         try:
             async def main() -> None:
-                async with OverkizClient(USERNAME, PASSWORD, SUPPORTED_SERVERS[serverchoice]) as client:
-                    await client.login()
-                    try :
-                        j=0
-                        for device_url in url :
-                            if str(device_url).isnumeric() == True :
-                                time.sleep(int(device_url))
-                                async with OverkizClient(USERNAME, PASSWORD, SUPPORTED_SERVERS[serverchoice]) as client:
-                                    await client.login()
-                            else :
+                try :
+                    j=0
+                    for device_url in url :
+                        if str(device_url).isnumeric() == True :
+                            time.sleep(int(device_url))
+                        else :
+                            if remove_accent(category) == 'scene' or remove_accent(category) == 'scenario':
                                 try :
-                                    exec_id = await client.execute_command( device_url, fonction )
+                                    async with OverkizClient(USERNAME, PASSWORD, SUPPORTED_SERVERS[serverchoice]) as client:
+                                        await client.login()
+                                        exec_id = await client.execute_scenario(device_url)
                                 except : pass
+                            elif remove_accent(category) == 'sensor' or remove_accent(category) == 'capteur':
+                                try:
+                                    async with OverkizClient(USERNAME, PASSWORD, SUPPORTED_SERVERS[serverchoice]) as client:
+                                        get_state = await client.get_state(device_url)
+                                        state_function=str(command_state[j]).replace("['","").replace("']","")
+                                        print('The '+str(good_name[j])+' is '+str(eval(state_function)))
+                                except :pass
+                            else :
                                 try :
-                                    exec_id = await client.execute_scenario(device_url)
+                                    async with OverkizClient(USERNAME, PASSWORD, SUPPORTED_SERVERS[serverchoice]) as client:
+                                        await client.login()
+                                        exec_id = await client.execute_command( device_url, fonction )
                                 except : pass
-                                try:
-                                    get_state = await client.get_state(device_url)
-                                    state_function=str(command_state[j]).replace("['","").replace("']","")
-                                    print('The '+str(good_name[j])+' is '+str(eval(state_function)))
-                                    j=j+1
-                                except :pass 
-                    except Exception as e:
-                        print(e) 
-                        try:
-                            if notification.lower() == 'y'or notification.lower() == 'yes':
-                                os.system("notify-send -i "+icon_app+" -t 150000 Tahoma "+"'Program failed. Here is the error message :\n\n "+str(e)+"'")
-                        except:pass
-                        exit()
+                            j=j+1
+                except Exception as e:
+                    print(e) 
+                    try:
+                        if notification.lower() == 'y'or notification.lower() == 'yes':
+                            os.system("notify-send -i "+icon_app+" -t 150000 Tahoma "+"'Program failed. Here is the error message :\n\n "+str(e)+"'")
+                    except:pass
+                    exit()
         except Exception as e:
             print( e )
             try :
                 if notification.lower() == 'y'or notification.lower() == 'yes':
                     os.system("notify-send -i "+icon_app+" -t 150000 Tahoma "+"'Program failed. Here is the error message :\n\n "+str(e)+"'")
             except: pass
```

### Comparing `tahoma-2.2.8/tahoma.egg-info/PKG-INFO` & `tahoma-2.2.9/tahoma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma
-Version: 2.2.8
+Version: 2.2.9
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma/issues
 Keywords: tahoma,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 It was created with Tahoma but can also works with Somfy Connectivity Kit, Connexoon, Cozytouch
 
 
 ![Somfy](https://www.voletsdusud.com/wp-content/uploads/2018/04/logo-tahoma.jpg)
 
 
 
-
+![GifTahoma.gif](https://github.com/pzim-devdata/tahoma/blob/main/GifTahoma.gif)
 
 # Install the main package :
 
 
 Install tahoma :
 
 #########################################
```

### Comparing `tahoma-2.2.8/tahoma.egg-info/SOURCES.txt` & `tahoma-2.2.9/tahoma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

