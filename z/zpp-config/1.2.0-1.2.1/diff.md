# Comparing `tmp/zpp_config-1.2.0.tar.gz` & `tmp/zpp_config-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpp_config-1.2.0.tar", last modified: Tue Feb 14 18:29:57 2023, max compression
+gzip compressed data, was "zpp_config-1.2.1.tar", last modified: Fri Jun 23 07:31:14 2023, max compression
```

## Comparing `zpp_config-1.2.0.tar` & `zpp_config-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-02-14 18:29:57.900000 zpp_config-1.2.0/
--rw-rw-rw-   0        0        0     4470 2023-02-14 18:29:57.895000 zpp_config-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3789 2022-08-10 10:08:39.000000 zpp_config-1.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-02-14 18:29:57.899000 zpp_config-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0      803 2022-06-03 07:33:42.000000 zpp_config-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-14 18:29:57.861000 zpp_config-1.2.0/zpp_config/
--rw-rw-rw-   0        0        0      184 2023-02-14 18:27:45.000000 zpp_config-1.2.0/zpp_config/__init__.py
--rw-rw-rw-   0        0        0    13778 2023-02-14 18:27:35.000000 zpp_config-1.2.0/zpp_config/config.py
-drwxrwxrwx   0        0        0        0 2023-02-14 18:29:57.888000 zpp_config-1.2.0/zpp_config.egg-info/
--rw-rw-rw-   0        0        0     4470 2023-02-14 18:29:57.000000 zpp_config-1.2.0/zpp_config.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-02-14 18:29:57.000000 zpp_config-1.2.0/zpp_config.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-14 18:29:57.000000 zpp_config-1.2.0/zpp_config.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-02-14 18:29:57.000000 zpp_config-1.2.0/zpp_config.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 07:31:14.229000 zpp_config-1.2.1/
+-rw-rw-rw-   0        0        0     1106 2023-06-23 07:28:06.000000 zpp_config-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4529 2023-06-23 07:31:14.223000 zpp_config-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3789 2022-08-10 10:08:47.000000 zpp_config-1.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 07:31:14.228000 zpp_config-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 07:31:14.182000 zpp_config-1.2.1/zpp_config/
+-rw-rw-rw-   0        0        0      184 2023-02-14 18:29:45.000000 zpp_config-1.2.1/zpp_config/__init__.py
+-rw-rw-rw-   0        0        0    13115 2023-06-23 07:25:34.000000 zpp_config-1.2.1/zpp_config/config.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:31:14.216000 zpp_config-1.2.1/zpp_config.egg-info/
+-rw-rw-rw-   0        0        0     4529 2023-06-23 07:31:14.000000 zpp_config-1.2.1/zpp_config.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2023-06-23 07:31:14.000000 zpp_config-1.2.1/zpp_config.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 07:31:14.000000 zpp_config-1.2.1/zpp_config.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-23 07:31:14.000000 zpp_config-1.2.1/zpp_config.egg-info/top_level.txt
```

### Comparing `zpp_config-1.2.0/PKG-INFO` & `zpp_config-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: zpp_config
-Version: 1.2.0
+Version: 1.2.1
 Summary: Module pour le chargement et la modification de fichier de configuration
 Home-page: https://github.com/ZephyrOff/py-zpp_config
-Author: ZephyrOff
-Author-email: contact@apajak.fr
-License: MIT
+Author: 
+License: MIT License
+Project-URL: Documentation, https://github.com/ZephyrOff/py-zpp_config
 Keywords: config file terminal zephyroff
 Platform: ALL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # zpp-config
 ## Informations
 Librairie pour l'utilisation et la modification de fichier de configuration:<br>
 - Charger un ou plusieurs paramÃ¨tres
 - Modifier un paramÃ¨tre existant
 - Ajout un paramÃ¨tre ou une section
@@ -157,8 +158,7 @@
 
 <br>
 
 ### Liste les sections disponibles
 ```python
 data = c.list_section()
 ```
-
```

### Comparing `zpp_config-1.2.0/README.md` & `zpp_config-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `zpp_config-1.2.0/zpp_config/config.py` & `zpp_config-1.2.1/zpp_config/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,32 @@
-####################################################################
-#/ Nom du projet: py-zpp_config                                   /#
-#/ Nom du fichier: config.py                                      /#
-#/ Type de fichier: fichier principal                             /#
-#/ Fichier annexe:                                                /#
-#/                                                                /#
-#/ Auteur: ZephyrOff  (Alexandre Pajak)                           /#
-#/ Version: 1.2.0                                                 /#
-#/ Description: Module pour le chargement et la modification      /#
-#/              de fichier de configuration                       /#
-#/ Date: 14/02/2023                                               /#
-####################################################################
-
 import re
 import ast
 from os.path import isfile, exists
 
 
 class Config():
 	def __init__(self,file,separator=" = ", escape_line="#", auto_create=False, read_only=False):
 		self.reg = r'\[[0-9A-Za-z-_ ]*\]'
 
 		self.separator=separator
 		self.escape_line = escape_line
 
 		self.read_only = read_only
+		self.created = False
 
 		if isfile(file) and exists(file):
 			self.file = file
 		else:
 			if auto_create==False:
 				print("Error: File not exists")
 			else:
 				self.file = file
+				with open(self.file, 'a') as f:
+					pass
+				self.created = True
 
 	#Str to real type
 	def return_data(self, data):
 		if data=="true" or data=="True":
 			return True
 		elif data=="false" or data=="False":
 			return False
@@ -216,14 +207,17 @@
 
 	def add(self,val=None,key=None,section=None):
 		if self.read_only==False:
 			exist = True
 			new_content=None
 			lock=False
 
+			if key=="":
+				key = '""'
+
 			if hasattr(self,'file'):
 				if section!=None and section!="" and section not in self.list_section():
 					exist = False
 
 				if val!=None and val!="" and key!=None and not (isinstance(key,str) or isinstance(key,list) or isinstance(key,int) or isinstance(key,float) or isinstance(key,bool) or isinstance(key,dict)):
 					print("Key not supported")
 					return
@@ -236,14 +230,16 @@
 						else:
 							new_content+="\n\n["+section+"]"
 						if val!=None and val!="" and key!=None:
 							new_content+="\n"+val+self.separator+str(key)
 
 					else:
 						data = self.load()
+						if not len(data):
+							data = {"":{}}
 						if section!=None:
 							se_test = section
 						else:
 							se_test = ""
 
 						if val!=None:
 							se = data[se_test]
```

### Comparing `zpp_config-1.2.0/zpp_config.egg-info/PKG-INFO` & `zpp_config-1.2.1/zpp_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: zpp-config
-Version: 1.2.0
+Version: 1.2.1
 Summary: Module pour le chargement et la modification de fichier de configuration
 Home-page: https://github.com/ZephyrOff/py-zpp_config
-Author: ZephyrOff
-Author-email: contact@apajak.fr
-License: MIT
+Author: 
+License: MIT License
+Project-URL: Documentation, https://github.com/ZephyrOff/py-zpp_config
 Keywords: config file terminal zephyroff
 Platform: ALL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # zpp-config
 ## Informations
 Librairie pour l'utilisation et la modification de fichier de configuration:<br>
 - Charger un ou plusieurs paramÃ¨tres
 - Modifier un paramÃ¨tre existant
 - Ajout un paramÃ¨tre ou une section
@@ -157,8 +158,7 @@
 
 <br>
 
 ### Liste les sections disponibles
 ```python
 data = c.list_section()
 ```
-
```

