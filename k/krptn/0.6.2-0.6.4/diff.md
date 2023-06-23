# Comparing `tmp/krptn-0.6.2.tar.gz` & `tmp/krptn-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krptn-0.6.2.tar", last modified: Fri May 26 15:45:04 2023, max compression
+gzip compressed data, was "krptn-0.6.4.tar", last modified: Thu Jun 22 20:46:25 2023, max compression
```

## Comparing `krptn-0.6.2.tar` & `krptn-0.6.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:45:04.902999 krptn-0.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:45:04.898999 krptn-0.6.2/CryptoLib/
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-26 15:44:40.000000 krptn-0.6.2/CryptoLib/CryptoLib.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-26 15:44:40.000000 krptn-0.6.2/CryptoLib/CryptoLib.h
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-26 15:44:40.000000 krptn-0.6.2/CryptoLib/OTPs.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-26 15:44:40.000000 krptn-0.6.2/CryptoLib/aes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-26 15:44:40.000000 krptn-0.6.2/CryptoLib/bases.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-05-26 15:44:40.000000 krptn-0.6.2/CryptoLib/ecc.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-26 15:44:40.000000 krptn-0.6.2/CryptoLib/hashes.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 15:44:40.000000 krptn-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-26 15:44:40.000000 krptn-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-26 15:45:04.902999 krptn-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-26 15:44:40.000000 krptn-0.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:45:04.898999 krptn-0.6.2/kr-openssl-config/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-26 15:45:02.000000 krptn-0.6.2/kr-openssl-config/ct_log_list.cnf
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-26 15:45:02.000000 krptn-0.6.2/kr-openssl-config/ct_log_list.cnf.dist
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-26 15:45:02.000000 krptn-0.6.2/kr-openssl-config/fipsmodule.cnf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:45:04.898999 krptn-0.6.2/kr-openssl-config/misc/
--rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-05-26 15:45:02.000000 krptn-0.6.2/kr-openssl-config/misc/CA.pl
--rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-05-26 15:45:02.000000 krptn-0.6.2/kr-openssl-config/misc/tsget.pl
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-26 15:45:02.000000 krptn-0.6.2/kr-openssl-config/openssl.cnf
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-05-26 15:45:02.000000 krptn-0.6.2/kr-openssl-config/openssl.cnf.dist
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:45:04.898999 krptn-0.6.2/krptn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-05-26 15:45:04.000000 krptn-0.6.2/krptn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-26 15:45:04.000000 krptn-0.6.2/krptn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:45:04.000000 krptn-0.6.2/krptn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 15:45:04.000000 krptn-0.6.2/krptn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 15:45:04.000000 krptn-0.6.2/krptn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:45:04.898999 krptn-0.6.2/krypton/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:45:04.898999 krptn-0.6.2/krypton/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/auth/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:45:04.902999 krptn-0.6.2/krypton/auth/django/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/auth/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/auth/django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/auth/django/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/auth/factors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:45:04.902999 krptn-0.6.2/krypton/auth/users/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/auth/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/auth/users/bases.py
--rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/auth/users/userModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/auth/users/userModelBaseAuth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/auth/users/userModelMFAAuth.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-05-26 15:44:40.000000 krptn-0.6.2/krypton/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-26 15:44:40.000000 krptn-0.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:45:04.902999 krptn-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-26 15:44:40.000000 krptn-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:46:25.542772 krptn-0.6.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:46:25.538772 krptn-0.6.4/CryptoLib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-06-22 20:46:03.000000 krptn-0.6.4/CryptoLib/CryptoLib.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-22 20:46:03.000000 krptn-0.6.4/CryptoLib/CryptoLib.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-22 20:46:03.000000 krptn-0.6.4/CryptoLib/OTPs.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-06-22 20:46:03.000000 krptn-0.6.4/CryptoLib/aes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-06-22 20:46:03.000000 krptn-0.6.4/CryptoLib/bases.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-06-22 20:46:03.000000 krptn-0.6.4/CryptoLib/ecc.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-22 20:46:03.000000 krptn-0.6.4/CryptoLib/hashes.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-22 20:46:03.000000 krptn-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-22 20:46:03.000000 krptn-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-22 20:46:25.542772 krptn-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-22 20:46:03.000000 krptn-0.6.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:46:25.538772 krptn-0.6.4/kr-openssl-config/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-22 20:46:23.000000 krptn-0.6.4/kr-openssl-config/ct_log_list.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-22 20:46:23.000000 krptn-0.6.4/kr-openssl-config/ct_log_list.cnf.dist
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-22 20:46:23.000000 krptn-0.6.4/kr-openssl-config/fipsmodule.cnf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:46:25.538772 krptn-0.6.4/kr-openssl-config/misc/
+-rw-r--r--   0 runner    (1001) docker     (123)     8062 2023-06-22 20:46:23.000000 krptn-0.6.4/kr-openssl-config/misc/CA.pl
+-rw-r--r--   0 runner    (1001) docker     (123)     6746 2023-06-22 20:46:23.000000 krptn-0.6.4/kr-openssl-config/misc/tsget.pl
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-22 20:46:23.000000 krptn-0.6.4/kr-openssl-config/openssl.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-06-22 20:46:23.000000 krptn-0.6.4/kr-openssl-config/openssl.cnf.dist
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:46:25.542772 krptn-0.6.4/krptn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-22 20:46:24.000000 krptn-0.6.4/krptn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-22 20:46:25.000000 krptn-0.6.4/krptn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:46:24.000000 krptn-0.6.4/krptn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-22 20:46:24.000000 krptn-0.6.4/krptn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 20:46:24.000000 krptn-0.6.4/krptn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:46:25.542772 krptn-0.6.4/krypton/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:46:25.542772 krptn-0.6.4/krypton/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/auth/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:46:25.542772 krptn-0.6.4/krypton/auth/django/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/auth/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/auth/django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/auth/django/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/auth/factors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:46:25.542772 krptn-0.6.4/krypton/auth/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/auth/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/auth/users/bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/auth/users/userModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9017 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/auth/users/userModelBaseAuth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5621 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/auth/users/userModelMFAAuth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8372 2023-06-22 20:46:03.000000 krptn-0.6.4/krypton/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-22 20:46:03.000000 krptn-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-22 20:46:25.542772 krptn-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-22 20:46:03.000000 krptn-0.6.4/setup.py
```

### Comparing `krptn-0.6.2/CryptoLib/CryptoLib.cpp` & `krptn-0.6.4/CryptoLib/CryptoLib.cpp`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/CryptoLib/CryptoLib.h` & `krptn-0.6.4/CryptoLib/CryptoLib.h`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/CryptoLib/OTPs.cpp` & `krptn-0.6.4/CryptoLib/OTPs.cpp`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/CryptoLib/aes.cpp` & `krptn-0.6.4/CryptoLib/aes.cpp`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/CryptoLib/bases.cpp` & `krptn-0.6.4/CryptoLib/bases.cpp`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/CryptoLib/ecc.cpp` & `krptn-0.6.4/CryptoLib/ecc.cpp`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/CryptoLib/hashes.cpp` & `krptn-0.6.4/CryptoLib/hashes.cpp`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/LICENSE` & `krptn-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/MANIFEST.in` & `krptn-0.6.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/PKG-INFO` & `krptn-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krptn
-Version: 0.6.2
+Version: 0.6.4
 Summary: Zero Knowledge security for Python
 Author-email: Krptn Project <contact@krptn.dev>
 Project-URL: Homepage, https://www.krptn.dev/
 Project-URL: Documentation, https://docs.krptn.dev/
 Project-URL: GitHub, https://github.com/krptn/krypton/
 Project-URL: Bug Tracker, https://github.com/krptn/krypton/issues
 Classifier: License :: OSI Approved :: Apache Software License
@@ -34,15 +34,15 @@
 pip install krptn
 ```
 
 ## What problem do we solve?
 
 **We all love Django and other web frameworks!** However, their primary focus is creating websites - not implementing secure storage for user data. One example is Django's built-in authentication system. While it hashes the password, it does not encrypt user data for you. Encryption is left to the developer...
 
-**Wouldn't it be nice if encryption would also be handled?** Perhaps it could be handled in a zero knowledge model, such that, without the user entering credentials, not even the database administrator can read it?! Maybe it could even use FIPS validated cryptography. This is exactly what we do!
+**Wouldn't it be nice if encryption would also be handled?** Perhaps it could be handled in a zero knowledge model, such that, without the user entering credentials, not even the database administrator can read it?! This is exactly what we do!
 
 **To prove that such is possible, we have a [Flask](https://github.com/krptn/flaskExample) and [Django](https://github.com/krptn/djangoExample) example on GitHub.**
 
 ![Krptn Visual](https://www.krptn.dev/krptnDiagram.webp)
 
 ## What do we do exactly?
```

### Comparing `krptn-0.6.2/README.md` & `krptn-0.6.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 pip install krptn
 ```
 
 ## What problem do we solve?
 
 **We all love Django and other web frameworks!** However, their primary focus is creating websites - not implementing secure storage for user data. One example is Django's built-in authentication system. While it hashes the password, it does not encrypt user data for you. Encryption is left to the developer...
 
-**Wouldn't it be nice if encryption would also be handled?** Perhaps it could be handled in a zero knowledge model, such that, without the user entering credentials, not even the database administrator can read it?! Maybe it could even use FIPS validated cryptography. This is exactly what we do!
+**Wouldn't it be nice if encryption would also be handled?** Perhaps it could be handled in a zero knowledge model, such that, without the user entering credentials, not even the database administrator can read it?! This is exactly what we do!
 
 **To prove that such is possible, we have a [Flask](https://github.com/krptn/flaskExample) and [Django](https://github.com/krptn/djangoExample) example on GitHub.**
 
 ![Krptn Visual](https://www.krptn.dev/krptnDiagram.webp)
 
 ## What do we do exactly?
```

### Comparing `krptn-0.6.2/kr-openssl-config/misc/CA.pl` & `krptn-0.6.4/kr-openssl-config/misc/CA.pl`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/kr-openssl-config/misc/tsget.pl` & `krptn-0.6.4/kr-openssl-config/misc/tsget.pl`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/kr-openssl-config/openssl.cnf.dist` & `krptn-0.6.4/kr-openssl-config/openssl.cnf.dist`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/krptn.egg-info/PKG-INFO` & `krptn-0.6.4/krptn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krptn
-Version: 0.6.2
+Version: 0.6.4
 Summary: Zero Knowledge security for Python
 Author-email: Krptn Project <contact@krptn.dev>
 Project-URL: Homepage, https://www.krptn.dev/
 Project-URL: Documentation, https://docs.krptn.dev/
 Project-URL: GitHub, https://github.com/krptn/krypton/
 Project-URL: Bug Tracker, https://github.com/krptn/krypton/issues
 Classifier: License :: OSI Approved :: Apache Software License
@@ -34,15 +34,15 @@
 pip install krptn
 ```
 
 ## What problem do we solve?
 
 **We all love Django and other web frameworks!** However, their primary focus is creating websites - not implementing secure storage for user data. One example is Django's built-in authentication system. While it hashes the password, it does not encrypt user data for you. Encryption is left to the developer...
 
-**Wouldn't it be nice if encryption would also be handled?** Perhaps it could be handled in a zero knowledge model, such that, without the user entering credentials, not even the database administrator can read it?! Maybe it could even use FIPS validated cryptography. This is exactly what we do!
+**Wouldn't it be nice if encryption would also be handled?** Perhaps it could be handled in a zero knowledge model, such that, without the user entering credentials, not even the database administrator can read it?! This is exactly what we do!
 
 **To prove that such is possible, we have a [Flask](https://github.com/krptn/flaskExample) and [Django](https://github.com/krptn/djangoExample) example on GitHub.**
 
 ![Krptn Visual](https://www.krptn.dev/krptnDiagram.webp)
 
 ## What do we do exactly?
```

### Comparing `krptn-0.6.2/krptn.egg-info/SOURCES.txt` & `krptn-0.6.4/krptn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/krypton/__init__.py` & `krptn-0.6.4/krypton/__init__.py`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/krypton/__main__.py` & `krptn-0.6.4/krypton/__main__.py`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/krypton/_load.py` & `krptn-0.6.4/krypton/_load.py`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/krypton/auth/_utils.py` & `krptn-0.6.4/krypton/auth/_utils.py`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/krypton/auth/django/middleware.py` & `krptn-0.6.4/krypton/auth/django/middleware.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Django middleware to add user object as needed to the request.
 """
 
 from django.http import HttpRequest
 from .users import djangoUser
-from ..users.userModel import UserError
+from ..users.bases import UserError
 
 
 def kryptonLoginMiddleware(get_response):
     """Django middleware to add user object as needed to the request.
 
 
     Arguments:
```

### Comparing `krptn-0.6.2/krypton/auth/factors.py` & `krptn-0.6.4/krypton/auth/factors.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,17 +117,15 @@
             secret -- The Shared secret
 
             otp -- The OTP
 
         Returns:
             True if success False otherwise
         """
-        if not base.verifyTOTP(secret, otp):
-            return False
-        return True
+        return base.verifyTOTP(secret, otp)
 
 class fido:
     """
     FIDO authentication support.
     """
     @staticmethod
     def register(userID:int, userName:str):
```

### Comparing `krptn-0.6.2/krypton/auth/users/bases.py` & `krptn-0.6.4/krypton/auth/users/bases.py`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/krypton/auth/users/userModel.py` & `krptn-0.6.4/krypton/auth/users/userModel.py`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/krypton/auth/users/userModelBaseAuth.py` & `krptn-0.6.4/krypton/auth/users/userModelBaseAuth.py`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/krypton/auth/users/userModelMFAAuth.py` & `krptn-0.6.4/krypton/auth/users/userModelMFAAuth.py`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/krypton/base.py` & `krptn-0.6.4/krypton/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 """
 Loads __CryptoLib and contains wrappers.
 """
 #pylint: disable=import-error
 # disbaled pylint because __CryptoLib is not built in CI/CD tests
 
-
 import ctypes
 import sys
 import base64
 import os
 from typing import ByteString
 from sqlalchemy import select
 from sqlalchemy.orm import scoped_session, Session
 try:
     import __CryptoLib
 except ImportError as err:
     if sys.platform == "win32" and not os.path.isfile("C:/Windows/System32/MSVCP140.dll"):
-        raise RuntimeError("This module requires Microsoft Visual C/C++ runtime. Please download it from https://learn.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist.") from err
+        raise RuntimeError("This module requires Microsoft Visual C/C++ runtime. "
+            "Please download it from https://learn.microsoft.com/en-US/cpp/windows/latest-supported-vc-redist."
+            ) from err
     raise err
 from . import configs, DBschemas, OPENSSL_CONFIG_FILE, OPENSSL_MODULES
 
 Adrr = id
 
 #: Load FIPS Validated resolver
 __CryptoLib.fipsInit(OPENSSL_CONFIG_FILE, OPENSSL_MODULES)
 
-#: Wrappers for __CryptoLib #
+#: Wrappers for __CryptoLib
 #: Help static analyzers automatically figure out function arguments, returns, etc..
 def restEncrypt(data:ByteString, key:bytes) -> bytes:
     """Encrypt Data for at rest storage
 
     Arguments:
         data -- Plain text
```

### Comparing `krptn-0.6.2/krypton/basic.py` & `krptn-0.6.4/krypton/basic.py`

 * *Files identical despite different names*

### Comparing `krptn-0.6.2/pyproject.toml` & `krptn-0.6.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0","wheel","pybind11>=2.10.3"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "krptn"
-version = "0.6.2"
+version = "0.6.4"
 description = "Zero Knowledge security for Python"
 readme = "README.md"
 authors = [
   { name="Krptn Project", email="contact@krptn.dev" },
 ]
 classifiers=[
     'License :: OSI Approved :: Apache Software License',
```

### Comparing `krptn-0.6.2/setup.py` & `krptn-0.6.4/setup.py`

 * *Files identical despite different names*

