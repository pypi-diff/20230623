# Comparing `tmp/pyhttpx-2.10.6.tar.gz` & `tmp/pyhttpx-2.10.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pyhttpx-2.10.6.tar", last modified: Thu Jun  1 08:45:16 2023, max compression
+gzip compressed data, was "dist\pyhttpx-2.10.7.tar", last modified: Fri Jun 23 00:57:17 2023, max compression
```

## Comparing `pyhttpx-2.10.6.tar` & `pyhttpx-2.10.7.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/
--rw-rw-rw-   0        0        0     1086 2022-08-12 14:37:21.000000 pyhttpx-2.10.6/LICENSE
--rw-rw-rw-   0        0        0       24 2022-08-15 03:00:31.000000 pyhttpx-2.10.6/MANIFEST.in
--rw-rw-rw-   0        0        0      339 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/PKG-INFO
--rw-rw-rw-   0        0        0     2592 2023-05-31 14:45:44.000000 pyhttpx-2.10.6/README.md
--rw-rw-rw-   0        0        0        0 2022-08-15 02:16:12.000000 pyhttpx-2.10.6/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx/
--rw-rw-rw-   0        0        0       81 2022-12-05 09:21:49.000000 pyhttpx-2.10.6/pyhttpx/__init__.py
--rw-rw-rw-   0        0        0      262 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/__version__.py
--rw-rw-rw-   0        0        0      106 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/compat.py
--rw-rw-rw-   0        0        0     1107 2022-12-05 07:47:21.000000 pyhttpx-2.10.6/pyhttpx/exception.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx/layers/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/__init__.py
--rw-rw-rw-   0        0        0     2308 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/aes.py
--rw-rw-rw-   0        0        0     1114 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/chacha20_poly1305.py
--rw-rw-rw-   0        0        0     4618 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/cipher_aead.py
--rw-rw-rw-   0        0        0     3910 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/cipher_block.py
--rw-rw-rw-   0        0        0      266 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/ciphers.py
--rw-rw-rw-   0        0        0     4293 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/ecc.py
--rw-rw-rw-   0        0        0     6180 2023-01-31 06:58:53.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/hkdf.py
--rw-rw-rw-   0        0        0      947 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/kx_algs.py
--rw-rw-rw-   0        0        0     1771 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/prf.py
--rw-rw-rw-   0        0        0     8016 2023-05-23 13:46:40.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/extensions.py
--rw-rw-rw-   0        0        0      123 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/fields.py
--rw-rw-rw-   0        0        0     1232 2022-10-27 08:35:29.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/handshake.py
--rw-rw-rw-   0        0        0     6750 2023-04-03 08:04:05.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/keyexchange.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/linux/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/linux/__init__.py
--rw-rw-rw-   0        0        0    10351 2023-05-29 10:31:50.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/pyaiossl.py
--rw-rw-rw-   0        0        0    19396 2023-05-23 13:31:03.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/pyssl.py
--rw-rw-rw-   0        0        0     2357 2023-05-17 03:53:54.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/socks.py
--rw-rw-rw-   0        0        0     4513 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/suites.py
--rw-rw-rw-   0        0        0    19146 2023-05-20 08:13:11.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/tls_context.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/window/
--rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.6/pyhttpx/layers/tls/window/__init__.py
--rw-rw-rw-   0        0        0     9335 2023-06-01 08:43:29.000000 pyhttpx-2.10.6/pyhttpx/models.py
--rw-rw-rw-   0        0        0    16766 2023-06-01 08:44:23.000000 pyhttpx-2.10.6/pyhttpx/session.py
--rw-rw-rw-   0        0        0     1991 2023-05-23 12:56:47.000000 pyhttpx-2.10.6/pyhttpx/utils.py
--rw-rw-rw-   0        0        0     8142 2023-05-30 00:24:03.000000 pyhttpx-2.10.6/pyhttpx/websocket.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx.egg-info/
--rw-rw-rw-   0        0        0      339 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1248 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-15 06:28:23.000000 pyhttpx-2.10.6/pyhttpx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       68 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/pyhttpx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/setup.cfg
--rw-rw-rw-   0        0        0     1576 2023-06-01 08:45:10.000000 pyhttpx-2.10.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-01 08:45:16.000000 pyhttpx-2.10.6/tests/
--rw-rw-rw-   0        0        0        0 2022-08-15 03:02:17.000000 pyhttpx-2.10.6/tests/__init__.py
--rw-rw-rw-   0        0        0     1007 2023-06-01 08:44:23.000000 pyhttpx-2.10.6/tests/requestTest.py
--rw-rw-rw-   0        0        0     1707 2023-05-31 14:30:48.000000 pyhttpx-2.10.6/tests/websocketTest.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/
+-rw-rw-rw-   0        0        0     1086 2022-08-12 14:37:21.000000 pyhttpx-2.10.7/LICENSE
+-rw-rw-rw-   0        0        0       24 2022-08-15 03:00:31.000000 pyhttpx-2.10.7/MANIFEST.in
+-rw-rw-rw-   0        0        0      339 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2592 2023-05-31 14:45:44.000000 pyhttpx-2.10.7/README.md
+-rw-rw-rw-   0        0        0        0 2022-08-15 02:16:12.000000 pyhttpx-2.10.7/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/pyhttpx/
+-rw-rw-rw-   0        0        0       81 2022-12-05 09:21:49.000000 pyhttpx-2.10.7/pyhttpx/__init__.py
+-rw-rw-rw-   0        0        0      262 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/__version__.py
+-rw-rw-rw-   0        0        0      106 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/compat.py
+-rw-rw-rw-   0        0        0     1107 2022-12-05 07:47:21.000000 pyhttpx-2.10.7/pyhttpx/exception.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/pyhttpx/layers/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/layers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/__init__.py
+-rw-rw-rw-   0        0        0     2308 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/aes.py
+-rw-rw-rw-   0        0        0     1114 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/chacha20_poly1305.py
+-rw-rw-rw-   0        0        0     4618 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/cipher_aead.py
+-rw-rw-rw-   0        0        0     3910 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/cipher_block.py
+-rw-rw-rw-   0        0        0      266 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/ciphers.py
+-rw-rw-rw-   0        0        0     4293 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/ecc.py
+-rw-rw-rw-   0        0        0     6180 2023-01-31 06:58:53.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/hkdf.py
+-rw-rw-rw-   0        0        0      947 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/kx_algs.py
+-rw-rw-rw-   0        0        0     1771 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/prf.py
+-rw-rw-rw-   0        0        0     8043 2023-06-03 00:48:29.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/extensions.py
+-rw-rw-rw-   0        0        0      123 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/fields.py
+-rw-rw-rw-   0        0        0     1232 2022-10-27 08:35:29.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/handshake.py
+-rw-rw-rw-   0        0        0     6750 2023-04-03 08:04:05.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/keyexchange.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/linux/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/linux/__init__.py
+-rw-rw-rw-   0        0        0    10286 2023-06-01 09:25:13.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/pyaiossl.py
+-rw-rw-rw-   0        0        0    19331 2023-06-03 00:48:29.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/pyssl.py
+-rw-rw-rw-   0        0        0     2357 2023-05-17 03:53:54.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/socks.py
+-rw-rw-rw-   0        0        0     4404 2023-06-01 09:51:28.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/suites.py
+-rw-rw-rw-   0        0        0    19146 2023-05-20 08:13:11.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/tls_context.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/window/
+-rw-rw-rw-   0        0        0        0 2022-09-23 08:01:24.000000 pyhttpx-2.10.7/pyhttpx/layers/tls/window/__init__.py
+-rw-rw-rw-   0        0        0     9501 2023-06-22 11:47:40.000000 pyhttpx-2.10.7/pyhttpx/models.py
+-rw-rw-rw-   0        0        0    16900 2023-06-23 00:57:09.000000 pyhttpx-2.10.7/pyhttpx/session.py
+-rw-rw-rw-   0        0        0     1991 2023-05-23 12:56:47.000000 pyhttpx-2.10.7/pyhttpx/utils.py
+-rw-rw-rw-   0        0        0     8142 2023-05-30 00:24:03.000000 pyhttpx-2.10.7/pyhttpx/websocket.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/pyhttpx.egg-info/
+-rw-rw-rw-   0        0        0      339 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/pyhttpx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1248 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/pyhttpx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/pyhttpx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-08-15 06:28:23.000000 pyhttpx-2.10.7/pyhttpx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       68 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/pyhttpx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/pyhttpx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/setup.cfg
+-rw-rw-rw-   0        0        0     1576 2023-06-23 00:57:09.000000 pyhttpx-2.10.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 00:57:17.000000 pyhttpx-2.10.7/tests/
+-rw-rw-rw-   0        0        0        0 2022-08-15 03:02:17.000000 pyhttpx-2.10.7/tests/__init__.py
+-rw-rw-rw-   0        0        0     1735 2023-06-23 00:57:09.000000 pyhttpx-2.10.7/tests/requestTest.py
+-rw-rw-rw-   0        0        0     1707 2023-05-31 14:30:48.000000 pyhttpx-2.10.7/tests/websocketTest.py
```

### Comparing `pyhttpx-2.10.6/LICENSE` & `pyhttpx-2.10.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/README.md` & `pyhttpx-2.10.7/README.md`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx/exception.py` & `pyhttpx-2.10.7/pyhttpx/exception.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/aes.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/chacha20_poly1305.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/chacha20_poly1305.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/cipher_aead.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/cipher_aead.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/cipher_block.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/cipher_block.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/ecc.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/ecc.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/hkdf.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/hkdf.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/kx_algs.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/kx_algs.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/crypto/prf.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/crypto/prf.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/extensions.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/extensions.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,20 +224,20 @@
     _type = 0x2b
     payload = '\x04\x03\x04\x03\x03'
     fields_desc = [
         _type,
         payload,
     ]
     def dump(self, host, context):
-
+        context.tls_max = 3
         if context.browser_type == 'chrome':
             if getattr(context, 'tls_max') == 3:
-                self.payload = '\x04\x8a\x8a\x03\x03'
+                self.payload = '\x04\x1a\x1a\x03\x03'
             else:
-                self.payload = '\x06\x8a\x8a\x03\x04\x03\x03'
+                self.payload = '\x06\x1a\x1a\x03\x04\x03\x03'
 
         else:
             self.payload = '\x04\x03\x04\x03\x03'
 
         self.fields_desc[1] = self.payload
         return super().dump(host, context)
 
@@ -248,15 +248,15 @@
     fields_desc = [
         _type,
         payload,
     ]
 
 class ExtPadding(_BaseExtension):
     _type = 0x15
-    payload = bytes(random.randint(100,300))
+    payload = bytes(random.randint(100,100))
     fields_desc = [
         _type,
         payload,
     ]
 
 
 def make_randext(host, ext_type, payload=None,context=None):
```

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/handshake.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/handshake.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/keyexchange.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/keyexchange.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/pyaiossl.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/pyaiossl.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,18 +207,18 @@
         self.supported_groups = None
         self.ec_points = None
         self.tls_max = 3
 
     def set_payload(self, browser_type=None,
                     ja3=None,
                     exts_payload=None,
-                    shuffle_extension_protocol=None):
+                    shuffle_proto=None):
         self.browser_type = browser_type or 'chrome'
         self.exts_payload = exts_payload
-        self.shuffle_extension_protocol = shuffle_extension_protocol
+        self.shuffle_proto = shuffle_proto
         #https://www.rfc-editor.org/rfc/rfc8701
         grease_list = [
             0x0A0A, 0x1A1A,
             0x2A2A, 0x3A3A,
             0x4A4A, 0x5A5A,
             0x6A6A, 0x7A7A,
             0x8A8A, 0x9A9A,
@@ -251,26 +251,26 @@
             if self.browser_type == 'chrome':
 
                 grease_ciphers = choose_grease()
                 grease_ext1 = choose_grease()
                 grease_ext2 = choose_grease()
                 self.grease_group = choose_grease()
                 exts = [grease_ext1,65281,18,27,43,0,5,51,13,11,17513,35,45,23,16,10,grease_ext2,21]
-                if self.shuffle_extension_protocol:
+                if self.shuffle_proto:
                     random.shuffle(exts)
 
                 exts = '-'.join(map(lambda x:str(x), exts))
                 self.ja3 = f"771,{grease_ciphers}-4865-4866-4867-49195-49199-49196-49200-52393-52392-49171-49172-156-157-47-53,{exts},{self.grease_group}-29-23-24,0"
                 self.exts_payload = {grease_ext2: b'\x00'}
 
 
             else:
                 #firefox_j,a3
                 exts=[0,23,65281,10,11,35,16,5,34,51,43,13,45,28,21]
-                if self.shuffle_extension_protocol:
+                if self.shuffle_proto:
                     random.shuffle(exts)
                 exts = '-'.join(map(lambda x:str(x), exts))
                 self.ja3 = f"771,4865-4867-4866-49195-49199-52393-52392-49196-49200-49162-49161-49171-49172-156-157-47-53,{exts},29-23-24-25-256-257,0"
 
 
         self.protocol, self.ciphers, self.exts, self.supported_groups, self.ec_points = self.ja3.split(',')
         self.ciphers = [int(i) for i in self.ciphers.split('-')]
```

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/pyssl.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/pyssl.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,18 @@
         self.application_layer_protocol_negotitaion = 'http/1.1'
         self.tlsversion = b'\x03\x03'
         self.tls_max = 4
 
     def set_payload(self, browser_type=None,
                     ja3=None,
                     exts_payload=None,
-                    shuffle_extension_protocol=None):
+                    shuffle_proto=None):
         self.browser_type = browser_type or 'chrome'
         self.exts_payload = exts_payload
-        self.shuffle_extension_protocol = shuffle_extension_protocol
+        self.shuffle_proto = shuffle_proto
 
         #https://www.rfc-editor.org/rfc/rfc8701
         grease_list = [
             0x0A0A, 0x1A1A,
             0x2A2A, 0x3A3A,
             0x4A4A, 0x5A5A,
             0x6A6A, 0x7A7A,
@@ -95,26 +95,26 @@
             if self.browser_type == 'chrome':
 
                 grease_ciphers = choose_grease()
                 grease_ext1 = choose_grease()
                 grease_ext2 = choose_grease()
                 self.grease_group = choose_grease()
                 exts = [grease_ext1,65281,18,27,43,0,5,51,13,11,17513,35,45,23,16,10,grease_ext2,21]
-                if self.shuffle_extension_protocol:
+                if self.shuffle_proto:
                     random.shuffle(exts)
 
                 exts = '-'.join(map(lambda x:str(x), exts))
                 self.ja3 = f"771,{grease_ciphers}-4865-4866-4867-49195-49199-49196-49200-52393-52392-49171-49172-156-157-47-53,{exts},{self.grease_group}-29-23-24,0"
                 self.exts_payload = {grease_ext2: b'\x00'}
 
 
             else:
                 #firefox_ja3
                 exts=[0,23,65281,10,11,35,16,5,34,51,43,13,45,28,21]
-                if self.shuffle_extension_protocol:
+                if self.shuffle_proto:
                     random.shuffle(exts)
                 exts = '-'.join(map(lambda x:str(x), exts))
                 self.ja3 = f"771,4865-4867-4866-49195-49199-52393-52392-49196-49200-49162-49161-49171-49172-156-157-47-53,{exts},29-23-24-25-256-257,0"
 
 
         self.protocol, self.ciphers, self.exts, self.supported_groups, self.ec_points = self.ja3.split(',')
         self.ciphers = [int(i) for i in self.ciphers.split('-')]
```

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/socks.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/socks.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/suites.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/suites.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,22 +4,15 @@
     0x1301,0x1302,0x1303,
     0xc02b,0xc02f,0xcca9, 0xcca8,
     0xc02c,0xc030,0xc00a,0xc009,
     0xc013, 0xc014, 0x009c, 0x009d,
     0x002f,0x0035
 ]
 
-if 1==0:
-    CIPHER_SUITES = [
 
-        #0xc02b,0xc02f,
-        #0xcca8,0xcca9,
-        0x002f,0x0035,
-
-    ]
 TLS_SUITES = {
     0x1301: {'name': 'TLS_AES_128_GCM_SHA256','key_len': 16,
              'sha': 'sha256','type': 'aead','kct': 'ECDHE',},
     0x1302: {'name': 'TLS_AES_256_GCM_SHA384', 'key_len': 32,
              'sha': 'sha384', 'type': 'aead', 'kct': 'ECDHE', },
 
     0x1303: {'name': 'TLS_CHACHA20_POLY1305_SHA256', 'key_len': 32,
```

### Comparing `pyhttpx-2.10.6/pyhttpx/layers/tls/tls_context.py` & `pyhttpx-2.10.7/pyhttpx/layers/tls/tls_context.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx/models.py` & `pyhttpx-2.10.7/pyhttpx/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,21 +128,27 @@
 
             if self.headers.get('content-length'):
                 self.content_length = int(self.headers.get('content-length', 0))
             else:
                 self.content_length = None
 
             if self.content_length == 0:
+
                 self.read_ended = True
 
         if self.headers:
-            if self.transfer_encoding == self.headers.get('transfer-encoding'):
-                #chunked 
-                if self.plaintext_buffer.endswith(b'0\r\n\r\n'):
-                    self.body = self.plaintext_buffer
+
+            if 'chunked'  == self.headers.get('transfer-encoding'):
+                #chunked
+                #if self.plaintext_buffer.endswith(b'\r\n0\r\n'):
+                #if self.plaintext_buffer.endswith(b'\r\n0\r\n'):
+                tmp = self.plaintext_buffer.split(b'\r\n')
+                if b'0' in tmp:
+                    
+                    self.body = b'\r\n'.join(tmp[:-2])
                     self.read_ended = True
 
             else:
 
                 if self.content_length:
                     if self.content_length <= len(self.plaintext_buffer):
                         self.body = self.plaintext_buffer[:self.content_length]
@@ -152,16 +158,18 @@
                     self.body = self.plaintext_buffer[:]
 
     @property
     def content(self):
         if self._content:
             return self._content
         else:
-            if self.headers.get('transfer-encoding') == self.transfer_encoding :
+
+            if self.headers.get('transfer-encoding') == 'chunked' :
                 str_chunks = self.body
+
                 html = b''
                 m = memoryview(str_chunks)
                 right = 0
                 left = 0
                 while len(str_chunks) > right:
                     index = str_chunks.index(b'\r\n', right)
                     right = index
```

### Comparing `pyhttpx-2.10.6/pyhttpx/session.py` & `pyhttpx-2.10.7/pyhttpx/session.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from urllib.parse import urlencode
 
 from pyhttpx.layers.tls import pyssl
 from pyhttpx.compat import *
 from pyhttpx.models import Request
 from pyhttpx.utils import default_headers,log,Conf
 from pyhttpx.models import Response,Http2Response
-from pyhttpx.exception import TooManyRedirects,ConnectionClosed
+from pyhttpx.exception import TooManyRedirects,ConnectionClosed,ReadTimeout
 
 
 from hpack import (
     Encoder,
     Decoder,
 )
 class CookieJar(object):
@@ -63,15 +63,15 @@
         self.ja3 = kwargs.get('ja3')
         self.browser_type = kwargs.get('browser_type')
         self.exts_payload = kwargs.get('exts_payload')
 
         self.http2 = kwargs.get('http2')
         self.poolconnections = LifoQueue(maxsize=self.maxsize)
         self.lock = RLock()
-        self.shuffle_proto = kwargs.get('shuffle_extension_protocol')
+        self.shuffle_proto = kwargs.get('shuffle_proto')
 
     def _new_conn(self):
 
         context = pyssl.SSLContext(http2=self.http2)
         context.set_payload(self.browser_type, self.ja3, self.exts_payload,
                             self.shuffle_proto
                             )
@@ -108,28 +108,40 @@
 
 
 class HttpSession(object):
     def __init__(self, ja3=None,
                  exts_payload=None,
                  browser_type=None,
                  http2=False ,
+                 settings=None,
+                 window_update=None,
                  ):
         #默认开启http2, 最终协议由服务器协商完成
         self.http2 = http2
         self.tls_session = None
         self.cookie_manger = CookieManger()
         self.browser_type = None
         self.active_addr = None
         self.tlss = {}
         self.browser_type = browser_type or 'chrome'
         self.exts_payload = exts_payload
         self.lock = RLock()
         self.ja3 = ja3
-        self.shuffle_proto = False
-        
+        self.shuffle_proto = shuffle_proto
+
+        self.SETTINGS = settings or [
+            "HEADER_TABLE_SIZE = 65536",
+            "ENABLE_PUSH = 0",
+            "MAX_CONCURRENT_STREAMS = 1000",
+            "INITIAL_WINDOW_SIZE = 6291456",
+            "MAX_HEADER_LIST_SIZE = 262144"
+        ]
+        self.WINDOW_UPDATE = window_update or 15663105
+
+
     def handle_cookie(self, req, set_cookies):
         #
         if not set_cookies:
             return
         c = {}
         if isinstance(set_cookies, str):
             for set_cookie in set_cookies.split(';'):
@@ -184,40 +196,38 @@
             _cookies = self.cookie_manger.get(get_top_domain(self.req.host))
         send_kw  = {}
 
         if _cookies:
             send_kw['cookie'] = '; '.join('{}={}'.format(k,v) for k,v in _cookies.items())
 
 
-        #if conn.context.application_layer_protocol_negotitaion
         addr = (req.host, req.port)
         self.connpool, self.conn = self.get_conn(req, addr)
 
         if self.conn.context.application_layer_protocol_negotitaion == 'h2':
-            resp = self.http2_send(req,)
+             resp = self.http2_send(req,)
 
         else:
             msg = self.prep_request(req, send_kw)
             resp = self.send(req, msg, update_cookies)
 
         return resp
 
-    def handle_redirect(self, resp):
+    def handle_redirect(self, resp, **kwargs):
 
-        if resp.status_code == 302 and resp.request.allow_redirects:
+        if resp.status_code == 302 and resp.request.allow_redirects and resp.headers['location'] != []:
             location = resp.headers['location']
             from urllib.parse import urlsplit
-            parse_location  =urlsplit(location)
-
+            parse_location  = urlsplit(location)
             if not parse_location.netloc:
                 location = f'https://{resp.request.host}{location}'
 
 
             for i in range(Conf.max_allow_redirects):
-                resp = self.request('GET', location)
+                resp = self.request('GET', location,**kwargs)
 
                 if resp.status_code != 302:
                     break
             else:
                 raise TooManyRedirects('too many redirects')
 
         return resp
@@ -266,34 +276,35 @@
             connpool = HTTPSConnectionPool(request=req,
                                            host=req.host,
                                            port=req.host,
                                            ja3=self.ja3,
                                            exts_payload=self.exts_payload,
                                            browser_type = self.browser_type,
                                            http2 = self.http2,
-                                           shuffle_extension_protocol =self.shuffle_proto
+                                           shuffle_proto =self.shuffle_proto
 
                                            )
 
 
-            # 代理连接池没有实现,如果使用代理,会导致使用同一个代理ip连接
-            # http2 存在bug
-            # closed
-            # self.tlss[addr] = connpool
+
             conn = connpool._get_conn()
 
         return connpool, conn
 
     def send(self, req, msg, update_cookies):
-        #http/1.1
-        #msg = bytes.fromhex('474554202f434349452f5363686564756c655f4c61622f434349454f6e6c696e652f434349454f6e6c696e6520485454502f312e310d0a486f73743a20636369652e636c6f7564617070732e636973636f2e636f6d0d0a557365722d4167656e743a204d6f7a696c6c612f352e30202857696e646f7773204e542031302e303b2057696e36343b207836343b2072763a3130362e3029204765636b6f2f32303130303130312046697265666f782f3130362e300d0a4163636570743a20746578742f68746d6c2c6170706c69636174696f6e2f7868746d6c2b786d6c2c6170706c69636174696f6e2f786d6c3b713d302e392c696d6167652f617669662c696d6167652f776562702c2a2f2a3b713d302e380d0a4163636570742d4c616e67756167653a207a682d434e2c7a683b713d302e382c7a682d54573b713d302e372c7a682d484b3b713d302e352c656e2d55533b713d302e332c656e3b713d302e320d0a4163636570742d456e636f64696e673a20677a69702c206465666c6174652c2062720d0a444e543a20310d0a436f6e6e656374696f6e3a206b6565702d616c6976650d0a557067726164652d496e7365637572652d52657175657374733a20310d0a5365632d46657463682d446573743a20646f63756d656e740d0a5365632d46657463682d4d6f64653a206e617669676174650d0a5365632d46657463682d536974653a206e6f6e650d0a5365632d46657463682d557365723a203f310d0a507261676d613a206e6f2d63616368650d0a43616368652d436f6e74726f6c3a206e6f2d63616368650d0a0d0a')
+        #h1
         self.conn.sendall(msg)
         response = Response()
+        sts = time.time()
+        timeout = req.timeout or 60
         while 1:
             r = self.conn.recv()
+            if (time.time() - sts) > timeout:
+                #chunked
+                raise ReadTimeout('read timeout')
             if not r:
                 self.conn.isclosed = True
                 break
             else:
                 response.flush(r)
 
             connection = response.headers.get('connection','')
@@ -323,18 +334,52 @@
 
         if not self.conn.isclosed:
             self.connpool._put_conn(self.conn)
 
         return response
 
     def http2_send(self, req):
-
-        self.first_load = True
+        setting_identifiers = {
+            'HEADER_TABLE_SIZE': 1,
+            'ENABLE_PUSH': 2,
+            'MAX_CONCURRENT_STREAMS': 3,
+            'INITIAL_WINDOW_SIZE': 4,
+            'MAX_HEADER_LIST_SIZE': 6,
+        }
         self.stream_id = 1
-        self.settings = bytes.fromhex('505249202a20485454502f322e300d0a0d0a534d0d0a0d0a00001e0400000000000001000100000002000000000003000003e800040060000000060004000000000408000000000000ef0001')
+        magic_frame = bytes.fromhex('505249202a20485454502f322e300d0a0d0a534d0d0a0d0a')
+
+        setting_block = b''
+        for s in self.SETTINGS:
+            key,value = map(lambda x:x.strip(),s.split('='))
+
+            setting_block += struct.pack('>H', setting_identifiers[key])
+            setting_block += struct.pack('>I', int(value))
+
+
+        setting_frame = b''.join([
+            struct.pack('!I', 30)[1:],
+            b'\x04',
+            b'\x00',
+            b'\x00\x00\x00\x00',
+            setting_block
+        ]
+        )
+        window_update_frame = b''.join([
+            struct.pack('!I', 4)[1:],
+            b'\x08',
+            b'\x00',
+            b'\x00\x00\x00\x00',
+            struct.pack('>I', int(self.WINDOW_UPDATE))
+        ]
+        )
+        #self.settings = bytes.fromhex('505249202a20485454502f322e300d0a0d0a534d0d0a0d0a00001e0400000000000001000100000002000000000003000003e800040060000000060004000000000408000000000000ef0001')
+        self.settings = b''.join(
+            [magic_frame,setting_frame,window_update_frame]
+        )
 
         if req.data:
             if isinstance(req.data, str):
                 req_body = req.data.encode('latin1')
 
             elif isinstance(req.data, dict):
                 req_body = urlencode(req.data).encode('latin1')
@@ -389,17 +434,15 @@
             struct.pack('!I', self.stream_id),
             stream_dependency_weight,
             weight,
             request_msg
         ])
         #update = b'\x00\x00\x04\x08\x00' + struct.pack('!I', self.stream_id) + b'\x00\xbe\x00\x00'
 
-        if self.first_load or 1==1:
-            self.conn.sendall(self.settings)
-
+        self.conn.sendall(self.settings)
 
         self.conn.sendall(stream_header)
         if req.method == 'POST':
             size = 2 ** 12
             while req_body:
                 block = req_body[:size]
                 req_body = req_body[size:]
@@ -413,15 +456,14 @@
                     struct.pack('!I', self.stream_id),
                     block
                 ])
                 self.conn.sendall(stream_data)
 
         response = Http2Response()
         cache = b''
-        self.first_load = False
         while 1:
 
             r = self.conn.recv()
             if not r:
                 self.conn.isclosed = True
                 break
 
@@ -482,16 +524,17 @@
         _cookies = self.cookie_manger.get(get_top_domain(self.req.host))
         return _cookies
 
     @cookies.setter
     def cookies(self, value):
         self.cookie_manger.cookies[get_top_domain(self.req.host)] = value
     def get(self, url, **kwargs):
+
         resp = self.request('GET', url, **kwargs)
-        resp = self.handle_redirect(resp)
+        resp = self.handle_redirect(resp, **kwargs)
         return resp
 
     def post(self,url, **kwargs):
         return self.request('POST', url, **kwargs)
 
     @property
     def content(self):
```

### Comparing `pyhttpx-2.10.6/pyhttpx/utils.py` & `pyhttpx-2.10.7/pyhttpx/utils.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx/websocket.py` & `pyhttpx-2.10.7/pyhttpx/websocket.py`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/pyhttpx.egg-info/SOURCES.txt` & `pyhttpx-2.10.7/pyhttpx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhttpx-2.10.6/setup.py` & `pyhttpx-2.10.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         sys.exit(errno)
 
 
 
 packages = find_packages()
 setup(
     name = "pyhttpx",
-    version = "2.10.6",
+    version = "2.10.7",
     keywords = ["pip", "pyhttpx"],
     description = "HTTP library.",
     long_description = "HTTP library, TLS supported version：tls1.2/tls1.3, HTTP supported version: http1.1/http2",
     license = "MIT Licence",
 
     url = "https://github.com/zero3301/pyhttpx",
     author = "3301",
```

### Comparing `pyhttpx-2.10.6/tests/websocketTest.py` & `pyhttpx-2.10.7/tests/websocketTest.py`

 * *Files identical despite different names*

