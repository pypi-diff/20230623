# Comparing `tmp/zpp_args-1.3.2.tar.gz` & `tmp/zpp_args-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zpp_args-1.3.2.tar", last modified: Tue Jun 13 07:53:40 2023, max compression
+gzip compressed data, was "zpp_args-1.3.3.tar", last modified: Fri Jun 23 07:15:59 2023, max compression
```

## Comparing `zpp_args-1.3.2.tar` & `zpp_args-1.3.3.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 07:53:40.610000 zpp_args-1.3.2/
--rw-rw-rw-   0        0        0     1106 2023-06-13 07:51:54.000000 zpp_args-1.3.2/LICENSE
--rw-rw-rw-   0        0        0     3404 2023-06-13 07:53:40.606000 zpp_args-1.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     2718 2022-12-23 08:35:38.000000 zpp_args-1.3.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-13 07:53:40.609000 zpp_args-1.3.2/setup.cfg
--rw-rw-rw-   0        0        0      777 2022-08-05 08:05:21.000000 zpp_args-1.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:53:40.577000 zpp_args-1.3.2/zpp_args/
--rw-rw-rw-   0        0        0      246 2022-12-26 19:03:30.000000 zpp_args-1.3.2/zpp_args/__init__.py
--rw-rw-rw-   0        0        0    10766 2023-06-13 07:49:11.000000 zpp_args-1.3.2/zpp_args/args.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:53:40.602000 zpp_args-1.3.2/zpp_args.egg-info/
--rw-rw-rw-   0        0        0     3404 2023-06-13 07:53:40.000000 zpp_args-1.3.2/zpp_args.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-06-13 07:53:40.000000 zpp_args-1.3.2/zpp_args.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 07:53:40.000000 zpp_args-1.3.2/zpp_args.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 07:53:40.000000 zpp_args-1.3.2/zpp_args.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 07:15:59.557000 zpp_args-1.3.3/
+-rw-rw-rw-   0        0        0     1106 2023-06-13 07:51:54.000000 zpp_args-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0     3402 2023-06-23 07:15:59.552000 zpp_args-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2718 2022-12-23 08:35:38.000000 zpp_args-1.3.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 07:15:59.556000 zpp_args-1.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-23 07:15:59.510000 zpp_args-1.3.3/zpp_args/
+-rw-rw-rw-   0        0        0      246 2022-12-26 19:03:30.000000 zpp_args-1.3.3/zpp_args/__init__.py
+-rw-rw-rw-   0        0        0    10764 2023-06-18 11:42:07.000000 zpp_args-1.3.3/zpp_args/args.py
+drwxrwxrwx   0        0        0        0 2023-06-23 07:15:59.543000 zpp_args-1.3.3/zpp_args.egg-info/
+-rw-rw-rw-   0        0        0     3402 2023-06-23 07:15:59.000000 zpp_args-1.3.3/zpp_args.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      183 2023-06-23 07:15:59.000000 zpp_args-1.3.3/zpp_args.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 07:15:59.000000 zpp_args-1.3.3/zpp_args.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-23 07:15:59.000000 zpp_args-1.3.3/zpp_args.egg-info/top_level.txt
```

### Comparing `zpp_args-1.3.2/LICENSE` & `zpp_args-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `zpp_args-1.3.2/PKG-INFO` & `zpp_args-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpp_args
-Version: 1.3.2
+Version: 1.3.3
 Summary: Module pour le traitement des arguments d'une ligne de commande
 Home-page: https://github.com/ZephyrOff/py-zpp_args
 Author: 
 License: MIT License
 Project-URL: Documentation, https://github.com/ZephyrOff/py-zpp_args
 Keywords: terminal args zephyroff
 Platform: ALL
@@ -98,8 +98,7 @@
 <br>
 
 ### DÃ©sactiver le check sur les paramÃ¨tres
 Pour dÃ©sactiver le check du nombre de paramÃ¨tres Ã  envoyer, il suffit d'appeler la fonction suivante.
 ```python
 parse.disable_check()
 ```
-
```

### Comparing `zpp_args-1.3.2/README.md` & `zpp_args-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `zpp_args-1.3.2/zpp_args/args.py` & `zpp_args-1.3.3/zpp_args/args.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
 
 	def param_exist(self,name):
 		for el in self.available_param:
 			if el['name']==name:
 				return True
 		return False
 
-	def set_parameter(self, name, description=None):
+	def set_parameter(self, name, description=""):
 		if not self.param_exist(name):
 			insert = {'name': name, 'description': description}
 			self.available_param.append(insert)
 		else:
 			print(f"Parameter {name} already set")
```

### Comparing `zpp_args-1.3.2/zpp_args.egg-info/PKG-INFO` & `zpp_args-1.3.3/zpp_args.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zpp-args
-Version: 1.3.2
+Version: 1.3.3
 Summary: Module pour le traitement des arguments d'une ligne de commande
 Home-page: https://github.com/ZephyrOff/py-zpp_args
 Author: 
 License: MIT License
 Project-URL: Documentation, https://github.com/ZephyrOff/py-zpp_args
 Keywords: terminal args zephyroff
 Platform: ALL
@@ -98,8 +98,7 @@
 <br>
 
 ### DÃ©sactiver le check sur les paramÃ¨tres
 Pour dÃ©sactiver le check du nombre de paramÃ¨tres Ã  envoyer, il suffit d'appeler la fonction suivante.
 ```python
 parse.disable_check()
 ```
-
```

