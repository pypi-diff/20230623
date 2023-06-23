# Comparing `tmp/jwskate-0.7.0.tar.gz` & `tmp/jwskate-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jwskate-0.7.0.tar", max compression
+gzip compressed data, was "jwskate-0.8.0.tar", max compression
```

## Comparing `jwskate-0.7.0.tar` & `jwskate-0.8.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0     1073 2023-04-19 10:02:25.020868 jwskate-0.7.0/LICENSE
--rw-r--r--   0        0        0    18475 2023-04-19 10:02:25.020868 jwskate-0.7.0/README.md
--rw-r--r--   0        0        0     3956 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/__init__.py
--rw-r--r--   0        0        0     2639 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/enums.py
--rw-r--r--   0        0        0     2809 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/__init__.py
--rw-r--r--   0        0        0     9627 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/base.py
--rw-r--r--   0        0        0     4692 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/ec.py
--rw-r--r--   0        0        0      323 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/encryption/__init__.py
--rw-r--r--   0        0        0     6245 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/encryption/aescbchmac.py
--rw-r--r--   0        0        0     3322 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/encryption/aesgcm.py
--rw-r--r--   0        0        0     1059 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/key_mgmt/__init__.py
--rw-r--r--   0        0        0     2427 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/key_mgmt/aesgcmkw.py
--rw-r--r--   0        0        0     2221 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/key_mgmt/aeskw.py
--rw-r--r--   0        0        0      740 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/key_mgmt/dir.py
--rw-r--r--   0        0        0     9770 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/key_mgmt/ecdh.py
--rw-r--r--   0        0        0     3551 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/key_mgmt/pbes2.py
--rw-r--r--   0        0        0     3471 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/key_mgmt/rsa.py
--rw-r--r--   0        0        0     4704 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/okp.py
--rw-r--r--   0        0        0      621 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/signature/__init__.py
--rw-r--r--   0        0        0     3669 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/signature/ec.py
--rw-r--r--   0        0        0     2421 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/signature/eddsa.py
--rw-r--r--   0        0        0     2058 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/signature/hmac.py
--rw-r--r--   0        0        0     3988 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwa/signature/rsa.py
--rw-r--r--   0        0        0      214 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwe/__init__.py
--rw-r--r--   0        0        0    12736 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwe/compact.py
--rw-r--r--   0        0        0      796 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/__init__.py
--rw-r--r--   0        0        0     6120 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/alg.py
--rw-r--r--   0        0        0    48771 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/base.py
--rw-r--r--   0        0        0     8246 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/ec.py
--rw-r--r--   0        0        0     6989 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/jwks.py
--rw-r--r--   0        0        0     6714 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/oct.py
--rw-r--r--   0        0        0    11437 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/okp.py
--rw-r--r--   0        0        0    10810 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwk/rsa.py
--rw-r--r--   0        0        0      265 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jws/__init__.py
--rw-r--r--   0        0        0     6111 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jws/compact.py
--rw-r--r--   0        0        0    10679 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jws/json.py
--rw-r--r--   0        0        0     5252 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jws/signature.py
--rw-r--r--   0        0        0      413 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwt/__init__.py
--rw-r--r--   0        0        0     8261 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwt/base.py
--rw-r--r--   0        0        0    11659 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwt/signed.py
--rw-r--r--   0        0        0     6688 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwt/signer.py
--rw-r--r--   0        0        0     5035 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/jwt/verifier.py
--rw-r--r--   0        0        0        0 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/py.typed
--rw-r--r--   0        0        0     4969 2023-04-19 10:02:25.024868 jwskate-0.7.0/jwskate/token.py
--rw-r--r--   0        0        0     2433 2023-04-19 10:02:25.024868 jwskate-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       75 2023-04-19 10:02:25.024868 jwskate-0.7.0/tests/.pydocstyle
--rw-r--r--   0        0        0       37 2023-04-19 10:02:25.024868 jwskate-0.7.0/tests/__init__.py
--rw-r--r--   0        0        0     2236 2023-04-19 10:02:25.024868 jwskate-0.7.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-19 10:02:25.024868 jwskate-0.7.0/tests/test_jwa/__init__.py
--rw-r--r--   0        0        0     2276 2023-04-19 10:02:25.024868 jwskate-0.7.0/tests/test_jwa/test_base.py
--rw-r--r--   0        0        0     2915 2023-04-19 10:02:25.024868 jwskate-0.7.0/tests/test_jwa/test_encryption.py
--rw-r--r--   0        0        0     7279 2023-04-19 10:02:25.024868 jwskate-0.7.0/tests/test_jwa/test_examples.py
--rw-r--r--   0        0        0     1601 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwa/test_key_mgmt.py
--rw-r--r--   0        0        0      316 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwa/test_signature.py
--rw-r--r--   0        0        0    31132 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwe.py
--rw-r--r--   0        0        0        0 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/__init__.py
--rw-r--r--   0        0        0     3962 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_alg.py
--rw-r--r--   0        0        0     4401 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_ec.py
--rw-r--r--   0        0        0     4264 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_generate.py
--rw-r--r--   0        0        0    21141 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_jwk.py
--rw-r--r--   0        0        0    10960 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_jwks.py
--rw-r--r--   0        0        0    11281 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_okp.py
--rw-r--r--   0        0        0    17351 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_rsa.py
--rw-r--r--   0        0        0     2437 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwk/test_symmetric.py
--rw-r--r--   0        0        0    22046 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jws.py
--rw-r--r--   0        0        0    25401 2023-04-19 10:02:25.028868 jwskate-0.7.0/tests/test_jwt.py
--rw-r--r--   0        0        0    19746 1970-01-01 00:00:00.000000 jwskate-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-23 11:45:56.677552 jwskate-0.8.0/LICENSE
+-rw-r--r--   0        0        0    18475 2023-06-23 11:45:56.677552 jwskate-0.8.0/README.md
+-rw-r--r--   0        0        0     3955 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/__init__.py
+-rw-r--r--   0        0        0     2639 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/enums.py
+-rw-r--r--   0        0        0     2809 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/__init__.py
+-rw-r--r--   0        0        0     9503 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/base.py
+-rw-r--r--   0        0        0     4716 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/ec.py
+-rw-r--r--   0        0        0      323 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/encryption/__init__.py
+-rw-r--r--   0        0        0     6207 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/encryption/aescbchmac.py
+-rw-r--r--   0        0        0     3322 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/encryption/aesgcm.py
+-rw-r--r--   0        0        0     1059 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/key_mgmt/__init__.py
+-rw-r--r--   0        0        0     2427 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/key_mgmt/aesgcmkw.py
+-rw-r--r--   0        0        0     2221 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/key_mgmt/aeskw.py
+-rw-r--r--   0        0        0      740 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/key_mgmt/dir.py
+-rw-r--r--   0        0        0     9749 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/key_mgmt/ecdh.py
+-rw-r--r--   0        0        0     3583 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/key_mgmt/pbes2.py
+-rw-r--r--   0        0        0     3471 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/key_mgmt/rsa.py
+-rw-r--r--   0        0        0     4766 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/okp.py
+-rw-r--r--   0        0        0      621 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/signature/__init__.py
+-rw-r--r--   0        0        0     3669 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/signature/ec.py
+-rw-r--r--   0        0        0     2421 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/signature/eddsa.py
+-rw-r--r--   0        0        0     2058 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/signature/hmac.py
+-rw-r--r--   0        0        0     3988 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwa/signature/rsa.py
+-rw-r--r--   0        0        0      216 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwe/__init__.py
+-rw-r--r--   0        0        0    12773 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwe/compact.py
+-rw-r--r--   0        0        0      796 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwk/__init__.py
+-rw-r--r--   0        0        0     6121 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwk/alg.py
+-rw-r--r--   0        0        0    47667 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwk/base.py
+-rw-r--r--   0        0        0     8264 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwk/ec.py
+-rw-r--r--   0        0        0     6988 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwk/jwks.py
+-rw-r--r--   0        0        0     8275 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwk/oct.py
+-rw-r--r--   0        0        0    11436 2023-06-23 11:45:56.677552 jwskate-0.8.0/jwskate/jwk/okp.py
+-rw-r--r--   0        0        0    10820 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jwk/rsa.py
+-rw-r--r--   0        0        0      265 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jws/__init__.py
+-rw-r--r--   0        0        0     6064 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jws/compact.py
+-rw-r--r--   0        0        0    10698 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jws/json.py
+-rw-r--r--   0        0        0     5262 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jws/signature.py
+-rw-r--r--   0        0        0      413 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jwt/__init__.py
+-rw-r--r--   0        0        0     9410 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jwt/base.py
+-rw-r--r--   0        0        0    11659 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jwt/signed.py
+-rw-r--r--   0        0        0     6688 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jwt/signer.py
+-rw-r--r--   0        0        0     5036 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/jwt/verifier.py
+-rw-r--r--   0        0        0        0 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/py.typed
+-rw-r--r--   0        0        0     4969 2023-06-23 11:45:56.681552 jwskate-0.8.0/jwskate/token.py
+-rw-r--r--   0        0        0     2360 2023-06-23 11:45:56.681552 jwskate-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/.pydocstyle
+-rw-r--r--   0        0        0       37 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/__init__.py
+-rw-r--r--   0        0        0     2236 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwa/__init__.py
+-rw-r--r--   0        0        0     2276 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwa/test_base.py
+-rw-r--r--   0        0        0     2915 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwa/test_encryption.py
+-rw-r--r--   0        0        0     7279 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwa/test_examples.py
+-rw-r--r--   0        0        0     1601 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwa/test_key_mgmt.py
+-rw-r--r--   0        0        0      259 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwa/test_signature.py
+-rw-r--r--   0        0        0    31129 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwe.py
+-rw-r--r--   0        0        0        0 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/__init__.py
+-rw-r--r--   0        0        0     3962 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_alg.py
+-rw-r--r--   0        0        0     4704 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_ec.py
+-rw-r--r--   0        0        0     4316 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_generate.py
+-rw-r--r--   0        0        0    21121 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_jwk.py
+-rw-r--r--   0        0        0    11153 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_jwks.py
+-rw-r--r--   0        0        0    11281 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_okp.py
+-rw-r--r--   0        0        0    17351 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_rsa.py
+-rw-r--r--   0        0        0     2425 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwk/test_symmetric.py
+-rw-r--r--   0        0        0    22043 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jws.py
+-rw-r--r--   0        0        0    25653 2023-06-23 11:45:56.681552 jwskate-0.8.0/tests/test_jwt.py
+-rw-r--r--   0        0        0    19452 1970-01-01 00:00:00.000000 jwskate-0.8.0/PKG-INFO
```

### Comparing `jwskate-0.7.0/LICENSE` & `jwskate-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/README.md` & `jwskate-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/jwskate/__init__.py` & `jwskate-0.8.0/jwskate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 The `jwskate` module implements the various Json Web Crypto-related
 standards: JWA, JWK, JWKS, JWE, JWT. Each standard has its own submodule, but
 for convenience, you can import any class or component directly from the root
 `jwskate` module.
 
 `jwskate` doesn't implement any actual cryptographic operation, it just
 provides a set of convenient wrappers around the `cryptography` module.
-
 """
 
 __author__ = """Guillaume Pujol"""
 __email__ = "guill.p.linux@gmail.com"
 
 from .enums import EncryptionAlgs, KeyManagementAlgs, KeyTypes, SignatureAlgs
 from .jwa import (
```

### Comparing `jwskate-0.7.0/jwskate/enums.py` & `jwskate-0.8.0/jwskate/enums.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/jwskate/jwa/__init__.py` & `jwskate-0.8.0/jwskate/jwa/__init__.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/jwskate/jwa/base.py` & `jwskate-0.8.0/jwskate/jwa/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-"""This module implement base classes used by Signature, Encryption and Key Management JWA algorithms."""
+"""This module implement base classes for the algorithms defined in JWA."""
 
 from __future__ import annotations
 
 from contextlib import contextmanager
 from typing import Generic, Iterator, SupportsBytes, Tuple, Type, TypeVar, Union
 
 import cryptography.exceptions
 from binapy import BinaPy
 from cryptography.hazmat.primitives import hashes
 from typing_extensions import Self, override
 
 
 class PrivateKeyRequired(AttributeError):
-    """Raised when a cryptographic operation requires a private key, and a public key has been provided instead."""
+    """Raised when a public key is provided for an operation that requires a private key."""
 
 
 class PublicKeyRequired(AttributeError):
-    """Raised when a cryptographic operation requires a public key, and a private key has been provided instead."""
+    """Raised when a private key is provided for an operation that requires a public key."""
 
 
 class BaseAlg:
     """Base class for all algorithms.
 
     An algorithm has a `name` and a `description`, whose reference is found in [IANA JOSE registry][IANA].
 
@@ -32,16 +32,16 @@
     """Alg use ('sig' or 'enc')"""
 
     name: str
     """Technical name of the algorithm."""
     description: str
     """Description of the algorithm (human readable)"""
     read_only: bool = False
-    """For algs that are considered insecure, set to True to allow only signature verification or decryption of existing
-    data, but don't allow new signatures or encryption."""
+    """For algs that are considered insecure, set to True to allow only signature verification or
+    decryption of existing data, but don't allow new signatures or encryption."""
 
     def __repr__(self) -> str:
         """Use the name of the alg as repr."""
         return self.name
 
     @classmethod
     def with_random_key(cls) -> Self:
@@ -84,15 +84,14 @@
         This is a convenience wrapper around `check_key(key)`.
 
         Args:
           key: the key to check for this alg class
 
         Returns:
           `True` if the key is suitable for this alg class, `False` otherwise
-
         """
         try:
             cls.check_key(key)
             return True
         except Exception:
             return False
 
@@ -260,23 +259,23 @@
     def encrypt(
         self,
         plaintext: Union[bytes, SupportsBytes],
         *,
         iv: Union[bytes, SupportsBytes],
         aad: Union[bytes, SupportsBytes, None] = None,
     ) -> Tuple[BinaPy, BinaPy]:
-        """Encrypt arbitrary data, with optional [Authenticated Encryption](https://wikipedia.org/wiki/Authenticated_encryption).
+        """Encrypt arbitrary data, with optional Authenticated Encryption.
 
-        This needs:
+        This needs as parameters:
 
         - the raw data to encrypt (`plaintext`)
         - a given random Initialisation Vector (`iv`) of the appropriate size
         - optional Additional Authentication Data (`aad`)
 
-        And returns a tuple (ciphered_data, authentication_tag).
+        And returns a tuple `(ciphered_data, authentication_tag)`.
 
         Args:
           plaintext: the data to encrypt
           iv: the Initialisation Vector to use
           aad: the Additional Authentication Data
 
         Returns:
@@ -327,8 +326,8 @@
 class BaseKeyManagementAlg(BaseAlg):
     """Base class for Key Management algorithms."""
 
     use = "enc"
 
 
 class MismatchingAuthTag(cryptography.exceptions.InvalidTag):
-    """Raised when trying to decrypt with an Authentication Tag that doesn't match the expected value."""
+    """Raised during decryption, when the Authentication Tag doesn't match the expected value."""
```

### Comparing `jwskate-0.7.0/jwskate/jwa/ec.py` & `jwskate-0.8.0/jwskate/jwa/ec.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,17 @@
     """A descriptive class for Elliptic Curves.
 
     Elliptic Curves have a name, a `cryptography.ec.EllipticCurve`, and a coordinate size.
 
     """
 
     name: str
-    """Curve name as defined in [IANA JOSE](https://www.iana.org/assignments/jose/jose.xhtml#web- key-elliptic-curve).
+    """Curve name as defined in [IANA JOSE](https://www.iana.org/assignments/jose/jose.xhtml#web-
+    key-elliptic-curve).
+
     This name will appear in `alg` or `enc` fields in JOSE headers.
     """
 
     cryptography_curve: ec.EllipticCurve
     """`cryptography` curve instance."""
 
     coordinate_size: int
@@ -51,25 +53,27 @@
         d = pn.private_value
         return x, y, d
 
     @classmethod
     def get_curve(
         cls, key: Union[ec.EllipticCurvePublicKey, ec.EllipticCurvePrivateKey]
     ) -> "EllipticCurve":
-        """Get the appropriate `EllipticCurve` instance for a given `cryptography` `EllipticCurvePublicKey`.
+        """Get the appropriate `EllipticCurve` instance for a given key.
+
+        The provided key must be an `EllipticCurvePublicKey` or `EllipticCurvePrivateKey`
+        from the `cryptography` module.
 
         Args:
           key: an Elliptic Curve private or public key from `cryptography`.
 
         Returns:
           the appropriate instance of EllipticCurve for the given key.
 
         Raises:
             NotImplementedError: if the curve is not supported
-
         """
         for c in cls.instances.values():
             if c.cryptography_curve.name == key.curve.name:
                 return c
         raise NotImplementedError(f"Unsupported Curve {key.curve.name}")
 
     @classmethod
@@ -84,26 +88,26 @@
           key: an Elliptic Curve public or private key from `cryptography`.
 
         Returns:
           a dict of JWK parameters matching that key
 
         Raises:
             TypeError: if the provided key is not an EllipticCurvePrivateKey or EllipticCurvePublicKey
-
         """
-        if not isinstance(key, (ec.EllipticCurvePrivateKey, ec.EllipticCurvePublicKey)):
-            raise TypeError(
-                "A EllipticCurvePrivateKey or a EllipticCurvePublicKey is required."
-            )
-        crv = cls.get_curve(key)
         public_numbers: ec.EllipticCurvePublicNumbers
         if isinstance(key, ec.EllipticCurvePrivateKey):
             public_numbers = key.public_key().public_numbers()
         elif isinstance(key, ec.EllipticCurvePublicKey):
             public_numbers = key.public_numbers()
+        else:
+            raise TypeError(
+                "A EllipticCurvePrivateKey or a EllipticCurvePublicKey is required."
+            )
+
+        crv = cls.get_curve(key)
         x = BinaPy.from_int(public_numbers.x, crv.coordinate_size).to("b64u").ascii()
         y = BinaPy.from_int(public_numbers.y, crv.coordinate_size).to("b64u").ascii()
         parameters = {"kty": KeyTypes.EC, "crv": crv.name, "x": x, "y": y}
         if isinstance(key, ec.EllipticCurvePrivateKey):
             pn = key.private_numbers()  # type: ignore[attr-defined]
             d = (
                 BinaPy.from_int(pn.private_value, crv.coordinate_size)
```

### Comparing `jwskate-0.7.0/jwskate/jwa/encryption/aescbchmac.py` & `jwskate-0.8.0/jwskate/jwa/encryption/aescbchmac.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """This module implements AES-CBC with HMAC-SHA based Encryption algorithms."""
 
 from typing import SupportsBytes, Tuple, Union
 
 from binapy import BinaPy
-from cryptography import exceptions
 from cryptography.hazmat.primitives import ciphers, constant_time, hashes, hmac, padding
 from cryptography.hazmat.primitives.ciphers import algorithms, modes
 
 from ..base import BaseAESEncryptionAlg, MismatchingAuthTag
 
 
 class BaseAesCbcHmacSha2(BaseAESEncryptionAlg):
@@ -49,15 +48,14 @@
         Args:
           ciphertext: the ciphertext
           iv: the Initialization Vector
           aad: the Additional Authenticated data
 
         Returns:
           the resulting MAC.
-
         """
         if not isinstance(ciphertext, bytes):
             ciphertext = bytes(ciphertext)
         if not isinstance(iv, bytes):
             iv = bytes(iv)
         if aad is None:  # pragma: no branch
             aad = b""
@@ -88,15 +86,14 @@
         Args:
           plaintext: the plain data to encrypt
           iv: the Initialization Vector
           aad: the Additional Authenticated Data, if any
 
         Returns:
           a tuple (encrypted_data, authentication_tag)
-
         """
         if not isinstance(plaintext, bytes):
             plaintext = bytes(plaintext)
         if not isinstance(iv, bytes):
             iv = bytes(iv)
         if aad is None:
             aad = b""
```

### Comparing `jwskate-0.7.0/jwskate/jwa/encryption/aesgcm.py` & `jwskate-0.8.0/jwskate/jwa/encryption/aesgcm.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/jwskate/jwa/key_mgmt/__init__.py` & `jwskate-0.8.0/jwskate/jwa/key_mgmt/__init__.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/jwskate/jwa/key_mgmt/aesgcmkw.py` & `jwskate-0.8.0/jwskate/jwa/key_mgmt/aesgcmkw.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/jwskate/jwa/key_mgmt/aeskw.py` & `jwskate-0.8.0/jwskate/jwa/key_mgmt/aeskw.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/jwskate/jwa/key_mgmt/dir.py` & `jwskate-0.8.0/jwskate/jwa/key_mgmt/dir.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/jwskate/jwa/key_mgmt/ecdh.py` & `jwskate-0.8.0/jwskate/jwa/key_mgmt/ecdh.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         private_key: Union[
             ec.EllipticCurvePrivateKey, x25519.X25519PrivateKey, x448.X448PrivateKey
         ],
         public_key: Union[
             ec.EllipticCurvePublicKey, x25519.X25519PublicKey, x448.X448PublicKey
         ],
     ) -> BinaPy:
-        """Perform an Elliptic Curve Diffie Hellman key exchange.
+        """Perform an Elliptic Curve Diffie-Hellman key exchange.
 
         This derives a shared key between a sender and a receiver, based on a public and a private key from each side.
         ECDH exchange produces the same key with either a sender private key and a recipient public key,
         or the matching sender public key and recipient private key.
 
         Args:
           private_key: a private EC key
@@ -195,15 +195,15 @@
             ec.EllipticCurvePublicKey, x25519.X25519PublicKey, x448.X448PublicKey
         ],
         *,
         alg: str,
         key_size: int,
         **headers: Any,
     ) -> BinaPy:
-        """Compute a shared key. This method is meant for use by the recipient of an encrypted message.
+        """Compute a shared key, for use by the recipient of an encrypted message.
 
         Args:
           ephemeral_public_key: the EPK, as received from sender
           alg: the content encryption algorithm identifier
           key_size: the CEK size
           **headers: additional headers as received from sender
```

### Comparing `jwskate-0.7.0/jwskate/jwa/key_mgmt/pbes2.py` & `jwskate-0.8.0/jwskate/jwa/key_mgmt/pbes2.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,15 +45,18 @@
 
         """
         if size < 8:
             raise ValueError("salts used for PBES2 must be at least 8 bytes long")
         return BinaPy.random(size)
 
     def derive(self, *, salt: bytes, count: int) -> BinaPy:
-        """Derive an encryption key based on the configured password, a given salt and the number of PBKDF iterations.
+        """Derive an encryption key.
+
+        Derivation is based on the configured password, a given salt and the number of
+        PBKDF iterations.
 
         Args:
           salt: the generated salt
           count: number of PBKDF iterations
 
         Returns:
             the generated encryption/decryption key
```

### Comparing `jwskate-0.7.0/jwskate/jwa/key_mgmt/rsa.py` & `jwskate-0.8.0/jwskate/jwa/key_mgmt/rsa.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/jwskate/jwa/okp.py` & `jwskate-0.8.0/jwskate/jwa/okp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-"""This module contains classes that describe CFRG Elliptic Curve Diffie-Hellman algorithms as specified in [RFC8037].
+"""This module implements CFRG Elliptic Curve Diffie-Hellman algorithms as specified in [RFC8037].
 
-[RFC8037]: https://www.rfc-editor.org/rfc/rfc8037.html
+[RFC8037]
+: https: //www.rfc-editor.org/rfc/rfc8037.html
 
 """
 
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Any, ClassVar, Dict, Tuple, Type, Union
@@ -38,24 +39,26 @@
     ) -> bytes:  # noqa: D102
         ...
 
     def public_key(self) -> PublicKeyProtocol:  # noqa: D102
         ...
 
     @classmethod
-    def generate(self) -> PrivateKeyProtocol:  # noqa: D102
+    def generate(cls) -> PrivateKeyProtocol:  # noqa: D102
         ...
 
 
 @dataclass
 class OKPCurve:
     """Represent an Octet Key Pair (OKP) Curve."""
 
     name: str
-    """Curve name as defined in [IANA JOSE](https://www.iana.org/assignments/jose/jose.xhtml#web- key-elliptic-curve).
+    """Curve name as defined in [IANA JOSE](https://www.iana.org/assignments/jose/jose.xhtml#web-
+    key-elliptic-curve).
+
     This name will appear in `crv` headers.
     """
 
     description: str
     """Curve description (human readable)."""
 
     cryptography_private_key_class: Type[Any]
@@ -90,25 +93,26 @@
             serialization.PrivateFormat.Raw,
             serialization.NoEncryption(),
         )
         return x, d
 
     @classmethod
     def get_curve(cls, key: Union[PublicKeyProtocol, PrivateKeyProtocol]) -> OKPCurve:
-        """Return the appropriate `OKPCurve` instance for a given `cryptography` private or public key.
+        """Return the appropriate `OKPCurve` instance for a given key.
+
+        This takes a `cryptography` private or public key as parameter. If the key type matches an OKP curve
 
         Args:
           key: `cryptography` private or public OKP key.
 
         Returns:
           OKPCurve: the appropriate `OKPCurve` for the given key
 
         Raises:
             NotImplementedError: if the required OKP curve is not supported
-
         """
         for c in cls.instances.values():
             if isinstance(
                 key, (c.cryptography_private_key_class, c.cryptography_public_key_class)
             ):
                 return c
         raise TypeError(
```

### Comparing `jwskate-0.7.0/jwskate/jwa/signature/__init__.py` & `jwskate-0.8.0/jwskate/jwa/signature/__init__.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/jwskate/jwa/signature/ec.py` & `jwskate-0.8.0/jwskate/jwa/signature/ec.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/jwskate/jwa/signature/eddsa.py` & `jwskate-0.8.0/jwskate/jwa/signature/eddsa.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/jwskate/jwa/signature/hmac.py` & `jwskate-0.8.0/jwskate/jwa/signature/hmac.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/jwskate/jwa/signature/rsa.py` & `jwskate-0.8.0/jwskate/jwa/signature/rsa.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/jwskate/jwe/compact.py` & `jwskate-0.8.0/jwskate/jwe/compact.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """This module implements the JWE Compact format."""
 
+from __future__ import annotations
+
 import warnings
 from functools import cached_property
 from typing import Any, Dict, Iterable, Mapping, Optional, SupportsBytes, Type, Union
 
 from binapy import BinaPy
 
 from jwskate.jwa import (
@@ -25,87 +27,86 @@
     """Represents a Json Web Encryption object, in compact representation, as defined in RFC7516.
 
     Args:
         value: the compact representation for this Jwe
 
     """
 
-    def __init__(self, value: Union[bytes, str]):
-        super().__init__(value)
+    def __init__(self, value: Union[bytes, str], max_size: int = 16 * 1024):
+        super().__init__(value, max_size)
 
         if self.value.count(b".") != 4:
             raise InvalidJwe(
                 "Invalid JWE: a JWE must contain a header, an encrypted key, an IV, a ciphertext and an authentication tag, separated by dots."
             )
 
         header, cek, iv, ciphertext, auth_tag = self.value.split(b".")
         try:
             headers = BinaPy(header).decode_from("b64u").parse_from("json")
-            enc = headers.get("enc")
-            if enc is None or not isinstance(enc, str):
-                raise InvalidJwe(
-                    "Invalid JWE header: this JWE doesn't have a valid 'enc' header."
-                )
-            self.headers = headers
-            self.additional_authenticated_data = header
         except ValueError:
             raise InvalidJwe(
                 "Invalid JWE header: it must be a Base64URL-encoded JSON object."
             )
+        enc = headers.get("enc")
+        if enc is None or not isinstance(enc, str):
+            raise InvalidJwe(
+                "Invalid JWE header: this JWE doesn't have a valid 'enc' header."
+            )
+        self.headers = headers
+        self.additional_authenticated_data = header
 
         try:
             self.wrapped_cek = BinaPy(cek).decode_from("b64u")
         except ValueError:
             raise InvalidJwe(
-                "Invalid JWE CEK: it must be a Base64URL-encoded binary data (bytes)."
+                "Invalid JWE CEK: it must be a Base64URL-encoded binary data."
             )
 
         try:
             self.initialization_vector = BinaPy(iv).decode_from("b64u")
         except ValueError:
             raise InvalidJwe(
-                "Invalid JWE IV: it must be a Base64URL-encoded binary data (bytes)"
+                "Invalid JWE IV: it must be a Base64URL-encoded binary data."
             )
 
         try:
             self.ciphertext = BinaPy(ciphertext).decode_from("b64u")
         except ValueError:
             raise InvalidJwe(
-                "Invalid JWE ciphertext: it must be a Base64URL-encoded binary data (bytes)"
+                "Invalid JWE ciphertext: it must be a Base64URL-encoded binary data."
             )
 
         try:
             self.authentication_tag = BinaPy(auth_tag).decode_from("b64u")
         except ValueError:
             raise InvalidJwe(
-                "Invalid JWE authentication tag: it must be a Base64URL-encoded binary data (bytes)"
+                "Invalid JWE authentication tag: it must be a Base64URL-encoded binary data."
             )
 
     @classmethod
     def from_parts(
         cls,
         *,
         headers: Mapping[str, Any],
         cek: bytes,
         iv: bytes,
         ciphertext: bytes,
         tag: bytes,
-    ) -> "JweCompact":
-        """Initialize a JWE from its different parts (header, cek, iv, ciphertext, tag).
+    ) -> JweCompact:
+        """Initialize a `JweCompact` from its different parts (header, cek, iv, ciphertext, tag).
 
         Args:
           headers: the headers (as a mapping of name: value)
           cek: the raw CEK
           iv: the raw IV
           ciphertext: the raw ciphertext
           tag: the authentication tag
 
         Returns:
-            the initialized JweCompact instance
-
+            the initialized `JweCompact` instance
         """
         return cls(
             b".".join(
                 (
                     BinaPy.serialize_to("json", headers).to("b64u"),
                     BinaPy(cek).to("b64u"),
                     BinaPy(iv).to("b64u"),
@@ -122,61 +123,59 @@
         The `enc` header contains the identifier of the CEK encryption algorithm.
 
         Returns:
             the enc value
 
         Raises:
             AttributeError: if there is no enc header or it is not a string
-
         """
         return self.get_header("enc")  # type: ignore[no-any-return]
         # header has been checked at init time
 
     @classmethod
     def encrypt(
         cls,
         plaintext: Union[bytes, SupportsBytes],
-        jwk: Union[Jwk, Dict[str, Any]],
+        key: Union[Jwk, Dict[str, Any], Any],
         *,
         enc: str,
         alg: Optional[str] = None,
         extra_headers: Optional[Dict[str, Any]] = None,
         cek: Optional[bytes] = None,
         iv: Optional[bytes] = None,
         epk: Optional[Jwk] = None,
-    ) -> "JweCompact":
-        """Encrypt an arbitrary plaintext into a JweCompact.
+    ) -> JweCompact:
+        """Encrypt an arbitrary plaintext into a `JweCompact`.
 
         Args:
           plaintext: the raw plaintext to encrypt
-          jwk: the public or symmetric key to use for encryption
+          key: the public or symmetric key to use for encryption
           enc: the encryption algorithm to use
           alg: the Key Management algorithm to use, if there is no 'alg' header defined in the Jwk
           extra_headers: additional headers to include in the generated token
           cek: the CEK to force use, for algorithms relying on a random CEK. Leave `None` to have a safe value generated by `jwskate`.
           iv: the IV to force use. Leave `None` to have a safe value generated by `jwskate`.
           epk: the EPK to force use. Leave `None` to have a safe value generated by `jwskate`.
 
         Returns:
             the generated JweCompact instance
-
         """
         extra_headers = extra_headers or {}
-        jwk = to_jwk(jwk)
+        key = to_jwk(key)
         alg = select_alg_class(
-            jwk.KEY_MANAGEMENT_ALGORITHMS, jwk_alg=jwk.alg, alg=alg
+            key.KEY_MANAGEMENT_ALGORITHMS, jwk_alg=key.alg, alg=alg
         ).name
 
-        cek_jwk, wrapped_cek, cek_headers = jwk.sender_key(
+        cek_jwk, wrapped_cek, cek_headers = key.sender_key(
             enc=enc, alg=alg, cek=cek, epk=epk, **extra_headers
         )
 
         headers = dict(extra_headers, **cek_headers, alg=alg, enc=enc)
-        if jwk.kid is not None:
-            headers["kid"] = jwk.kid
+        if key.kid is not None:
+            headers["kid"] = key.kid
 
         aad = BinaPy.serialize_to("json", headers).to("b64u")
 
         ciphertext, iv, tag = cek_jwk.encrypt(plaintext, aad=aad, iv=iv, alg=enc)
 
         return cls.from_parts(
             headers=headers, cek=wrapped_cek, iv=iv, ciphertext=ciphertext, tag=tag
@@ -185,62 +184,60 @@
     PBES2_ALGORITHMS: Mapping[str, Type[BasePbes2]] = {
         alg.name: alg
         for alg in [Pbes2_HS256_A128KW, Pbes2_HS384_A192KW, Pbes2_HS512_A256KW]
     }
 
     def unwrap_cek(
         self,
-        jwk_or_password: Union[Jwk, Dict[str, Any], bytes, str],
+        key_or_password: Union[Jwk, Dict[str, Any], bytes, str],
         alg: Optional[str] = None,
         algs: Optional[Iterable[str]] = None,
     ) -> Jwk:
         """Unwrap the CEK from this `Jwe` using the provided key or password.
 
         Args:
-          jwk_or_password: the decryption JWK or password
+          key_or_password: the decryption JWK or password
           alg: allowed key management algorithm, if there is only 1
           algs: allowed key managements algorithms, if there are several
 
         Returns:
             the unwrapped CEK, as a SymmetricJwk
-
         """
-        if isinstance(jwk_or_password, (bytes, str)):
-            password = jwk_or_password
+        if isinstance(key_or_password, (bytes, str)):
+            password = key_or_password
             return self.unwrap_cek_with_password(password)
 
-        jwk = Jwk(jwk_or_password)
+        jwk = to_jwk(key_or_password)
         select_alg_classes(
             jwk.KEY_MANAGEMENT_ALGORITHMS,
             jwk_alg=self.alg,
             alg=alg,
             algs=algs,
             strict=True,
         )
         cek = jwk.recipient_key(self.wrapped_cek, **self.headers)
         return cek
 
     def decrypt(
         self,
-        jwk: Union[Jwk, Dict[str, Any]],
+        key: Union[Jwk, Dict[str, Any], Any],
         alg: Optional[str] = None,
         algs: Optional[Iterable[str]] = None,
     ) -> BinaPy:
         """Decrypts this `Jwe` payload using a `Jwk`.
 
         Args:
-          jwk: the decryption key
+          key: the decryption key
           alg: allowed key management algorithm, if there is only 1
           algs: allowed keys management algorithms, if there are several
 
         Returns:
           the decrypted payload
-
         """
-        cek_jwk = self.unwrap_cek(jwk, alg=alg, algs=algs)
+        cek_jwk = self.unwrap_cek(key, alg=alg, algs=algs)
 
         plaintext = cek_jwk.decrypt(
             ciphertext=self.ciphertext,
             iv=self.initialization_vector,
             tag=self.authentication_tag,
             aad=self.additional_authenticated_data,
             alg=self.enc,
@@ -350,15 +347,17 @@
                 "Invalid JWE: invalid value for the 'p2c' header, must be a positive integer."
             )
         wrapper = keyalg(password)
         cek = wrapper.unwrap_key(self.wrapped_cek, salt=salt, count=p2c)
         return SymmetricJwk.from_bytes(cek)
 
     def decrypt_with_password(self, password: Union[bytes, str]) -> bytes:
-        """Decrypt the JWE token with a password. This only works for tokens encrypted with a password.
+        """Decrypt this JWE with a password.
+
+        This only works for tokens encrypted with a password.
 
         Args:
           password: the password to use
 
         Returns:
             the unencrypted payload
```

### Comparing `jwskate-0.7.0/jwskate/jwk/__init__.py` & `jwskate-0.8.0/jwskate/jwk/__init__.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/jwskate/jwk/alg.py` & `jwskate-0.8.0/jwskate/jwk/alg.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,16 +13,17 @@
 class ExpectedAlgRequired(ValueError):
     """Raised when the expected signature alg(s) must be provided."""
 
 
 class MismatchingAlg(ValueError):
     """Raised when attempting a cryptographic operation with an unexpected algorithm.
 
-    Signature verification or a decryption operation with an algorithm that does not
-    match the algorithm specified in the key or the token.
+    Signature verification or a decryption operation with an algorithm that does not match the
+    algorithm specified in the key or the token.
+
     """
 
     def __init__(
         self,
         target_alg: str,
         alg: Optional[str] = None,
         algs: Union[Iterable[str], None] = None,
```

### Comparing `jwskate-0.7.0/jwskate/jwk/base.py` & `jwskate-0.8.0/jwskate/jwk/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-"""This module implements the `Jwk` class, which provides the main interface for using or interacting with a JWK key.
+"""This module contains the `Jwk` class and associated helpers.
 
-Subclasses of `Jwk` will implement the specific key types, like RSA, EC, OKP, and will provide an interface to access
-the specific attributes for each key type.
-Unless you are dealing with a specific key type and want to access the internal attributes, you should only ever need
-to use the interface from `Jwk`.
+`Jwk` provides the main interface for using or interacting with JWK keys.
+
+Subclasses of `Jwk` will implement the specific key types, like RSA, EC, OKP, and will provide an
+interface to access the specific attributes for each key type. Unless you are dealing with a
+specific key type and want to access the internal attributes, you should only ever need to use the
+interface from `Jwk`.
 """
 
 from __future__ import annotations
 
 import warnings
 from dataclasses import dataclass
 from typing import (
@@ -94,70 +96,48 @@
 
         Args:
             alg: a signature or key management algorithm identifier
             **kwargs: specific parameters, depending on the key type, or additional members to include in the `Jwk`
 
         Returns:
             the generated `Jwk`
-
         """
         for kty, jwk_class in cls.subclasses.items():
-            alg_class: Optional[Type[BaseAlg]]
             try:
-                alg_class = jwk_class._get_alg_class(alg)
-                # special cases for AES or HMAC based algs which require a specific key size
-                if issubclass(alg_class, (BaseAESEncryptionAlg, BaseAesKeyWrap)):
-                    key_size = kwargs.get("key_size")
-                    if key_size is not None and key_size != alg_class.key_size:
-                        raise ValueError(
-                            f"Key for {alg} must be exactly {alg_class.key_size} bits. "
-                            "You should remove the `key_size` parameter to generate a key of the appropriate length."
-                        )
-                    kwargs.setdefault("key_size", alg_class.key_size)
-                elif issubclass(alg_class, BaseHMACSigAlg):
-                    key_size = kwargs.get("key_size")
-                    if key_size is not None and key_size < alg_class.min_key_size:
-                        warnings.warn(
-                            f"Symmetric keys to use with {alg} should be at least {alg_class.min_key_size} bits "
-                            "in order to make the key at least as hard to brute-force as the signature. "
-                            f"You requested a key size of {key_size} bits."
-                        )
-                    else:
-                        kwargs.setdefault("key_size", alg_class.min_key_size)
-
+                jwk_class._get_alg_class(alg)
                 return jwk_class.generate(alg=alg, **kwargs)
             except UnsupportedAlg:
                 continue
 
         raise UnsupportedAlg(alg)
 
-    """A dict of 'kty' values to subclasses implementing each specific Key Type."""
-
     @classmethod
     def generate_for_kty(cls, kty: str, **kwargs: Any) -> Jwk:
-        """Generate a key with a specific type and return the resulting Jwk.
+        """Generate a key with a specific type and return the resulting `Jwk`.
 
         Args:
           kty: key type to generate
-          **kwargs: specific parameters depending on the key type, or additional members to include in the Jwk
+          **kwargs: specific parameters depending on the key type, or additional members to include in the `Jwk`
 
         Returns:
-            the resulting Jwk
+            the resulting `Jwk`
 
         Raises:
-            UnsupportedKeyType: if the key type is not supported
+            UnsupportedKeyType: if the specified key type (`kty`) is not supported
 
         """
         jwk_class = cls.subclasses.get(kty)
         if jwk_class is None:
             raise UnsupportedKeyType("Unsupported Key Type:", kty)
         return jwk_class.generate(**kwargs)
 
     subclasses: Dict[str, Type[Jwk]] = {}
+    """A dict of 'kty' values to `Jwk` subclasses implementing each specific Key Type."""
     cryptography_key_types: Dict[Any, Type[Jwk]] = {}
+    """A dict of cryptography classes to equivalent `Jwk` subclasses."""
 
     PARAMS: Mapping[str, JwkParameter]
 
     KTY: ClassVar[str]
 
     CRYPTOGRAPHY_PRIVATE_KEY_CLASSES: ClassVar[Iterable[Any]]
     CRYPTOGRAPHY_PUBLIC_KEY_CLASSES: ClassVar[Iterable[Any]]
@@ -197,15 +177,14 @@
             - a `dict` with the parsed Jwk content
             - another Jwk, which will be used as-is instead of creating a copy
             - an instance from a `cryptography` public or private key class
 
         Args:
             key: a dict containing JWK parameters, or another Jwk instance, or a `cryptography` key
             **kwargs: additional members to include in the Jwk
-
         """
         if cls == Jwk:
             if isinstance(key, Jwk):
                 return cls.from_cryptography_key(key.cryptography_key, **kwargs)
             if isinstance(key, dict):
                 kty: Optional[str] = key.get("kty")
                 if kty is None:
@@ -268,15 +247,14 @@
 
     @property
     def is_private(self) -> bool:
         """Return `True` if the key is private, `False` otherwise.
 
         Returns:
             `True` if the key is private, `False` otherwise
-
         """
         return True
 
     @property
     def is_symmetric(self) -> bool:
         """Return `True` if the key is symmetric, `False` otherwise."""
         return False
@@ -347,31 +325,31 @@
             raise TypeError(f"invalid kid type {type(kid)}", kid)
         return kid
 
     @property
     def use(self) -> Optional[str]:
         """Return the key use.
 
-        If no `alg` parameter is present, this returns the `use` parameter from this JWK. If an `alg` parameter is
-        present, the use is deduced from this alg. To check for the presence of the `use` parameter, use
-        `jwk.get('use')`.
+        If no `alg` parameter is present, this returns the `use` parameter from this JWK. If an
+        `alg` parameter is present, the use is deduced from this alg. To check for the presence of
+        the `use` parameter, use `jwk.get('use')`.
 
         """
         if self.alg:
             return self._get_alg_class(self.alg).use
         else:
             return self.get("use")
 
     @property
     def key_ops(self) -> Tuple[str, ...]:
         """Return the key operations.
 
-        If no `alg` parameter is present, this returns the `key_ops` parameter from this JWK. If an `alg` parameter is
-        present, the key operations are deduced from this alg. To check for the presence of the `key_ops` parameter, use
-        `jwk.get('key_ops')`.
+        If no `alg` parameter is present, this returns the `key_ops` parameter from this JWK. If an
+        `alg` parameter is present, the key operations are deduced from this alg. To check for the
+        presence of the `key_ops` parameter, use `jwk.get('key_ops')`.
 
         """
         key_ops: Tuple[str, ...]
         if self.use == "sig":
             if self.is_symmetric:
                 key_ops = ("sign", "verify")
             elif self.is_private:
@@ -440,15 +418,17 @@
     def check(
         self,
         *,
         is_private: Optional[bool] = None,
         is_symmetric: Optional[bool] = None,
         kty: Optional[str] = None,
     ) -> Jwk:
-        """Check this key for type, privateness and/or symmetricness. Raise a ValueError if it not as expected.
+        """Check this key for type, privateness and/or symmetricness.
+
+        This raises a `ValueError` if the key is not as expected.
 
         Args:
             is_private: if `True`, check if the key is private, if `False`, check if it is public, if `None`, do nothing
             is_symmetric: if `True`, check if the key is symmetric, if `False`, check if it is asymmetric, if `None`, do nothing
             kty: the expected key type, if any
 
         Returns:
@@ -541,29 +521,33 @@
 
         # if key is used for signing, it must be private
         for op in self.get("key_ops", []):
             if op in ("sign", "unwrapKey") and not self.is_private:
                 raise InvalidJwk(f"Key Operation is '{op}' but the key is public")
 
     def signature_class(self, alg: Optional[str] = None) -> Type[BaseSignatureAlg]:
-        """Return the appropriate signature algorithm class (a `BaseSignatureAlg` subclass) to use with this key.
+        """Return the appropriate signature algorithm class to use with this key.
+
+        The returned class is a `BaseSignatureAlg` subclass.
 
         If this key doesn't have an `alg` parameter, you must supply one as parameter to this method.
 
         Args:
             alg: the algorithm identifier, if not already present in this Jwk
 
         Returns:
             the appropriate `BaseSignatureAlg` subclass
 
         """
         return select_alg_class(self.SIGNATURE_ALGORITHMS, jwk_alg=self.alg, alg=alg)
 
     def encryption_class(self, alg: Optional[str] = None) -> Type[BaseAESEncryptionAlg]:
-        """Return the appropriate encryption algorithm class (a `BaseAESEncryptionAlg` subclass) to use with this key.
+        """Return the appropriate encryption algorithm class to use with this key.
+
+        The returned class is a subclass of `BaseAESEncryptionAlg`.
 
         If this key doesn't have an `alg` parameter, you must supply one as parameter to this method.
 
         Args:
             alg: the algorithm identifier, if not already present in this Jwk
 
         Returns:
@@ -587,34 +571,38 @@
 
         """
         return select_alg_class(
             self.KEY_MANAGEMENT_ALGORITHMS, jwk_alg=self.alg, alg=alg
         )
 
     def signature_wrapper(self, alg: Optional[str] = None) -> BaseSignatureAlg:
-        """Initialize a  key management wrapper (an instance of a `BaseKeyManagementAlg` subclass) with this key.
+        """Initialize a  key management wrapper with this key.
+
+        This returns an instance of a `BaseSignatureAlg` subclass.
 
         If this key doesn't have an `alg` parameter, you must supply one as parameter to this method.
 
         Args:
             alg: the algorithm identifier, if not already present in this Jwk
 
         Returns:
-            a `BaseKeyManagementAlg` instance initialized with the current key
+            a `BaseSignatureAlg` instance initialized with the current key
 
         """
         alg_class = self.signature_class(alg)
         if issubclass(alg_class, BaseSymmetricAlg):
             return alg_class(self.key)
         elif issubclass(alg_class, BaseAsymmetricAlg):
             return alg_class(self.cryptography_key)
         raise UnsupportedAlg(alg)  # pragma: no cover
 
     def encryption_wrapper(self, alg: Optional[str] = None) -> BaseAESEncryptionAlg:
-        """Initialize an encryption wrapper (an instance of a `BaseAESEncryptionAlg` subclass) with this key.
+        """Initialize an encryption wrapper with this key.
+
+        This returns an instance of a `BaseAESEncryptionAlg` subclass.
 
         If this key doesn't have an `alg` parameter, you must supply one as parameter to this method.
 
         Args:
             alg: the algorithm identifier, if not already present in this Jwk
 
         Returns:
@@ -625,15 +613,17 @@
         if issubclass(alg_class, BaseSymmetricAlg):
             return alg_class(self.key)
         elif issubclass(alg_class, BaseAsymmetricAlg):  # pragma: no cover
             return alg_class(self.cryptography_key)  # pragma: no cover
         raise UnsupportedAlg(alg)  # pragma: no cover
 
     def key_management_wrapper(self, alg: Optional[str] = None) -> BaseKeyManagementAlg:
-        """Initialize a key management wrapper (an instance of a `BaseKeyManagementAlg` subclass) with this key.
+        """Initialize a key management wrapper with this key.
+
+        This returns an instance of a `BaseKeyManagementAlg` subclass.
 
         If this key doesn't have an `alg` parameter, you must supply one as parameter to this method.
 
         Args:
             alg: the algorithm identifier, if not already present in this Jwk
 
         Returns:
@@ -705,15 +695,14 @@
           data: the data to verify
           signature: the signature to verify
           alg: the allowed signature alg, if there is only one
           algs: the allowed signature algs, if there are several
 
         Returns:
           `True` if the signature matches, `False` otherwise
-
         """
         if not self.is_symmetric and self.is_private:
             warnings.warn(
                 "You are trying to validate a signature with a private key. "
                 "Signature should always be verified with a public key."
             )
             public_jwk = self.public_jwk()
@@ -1039,15 +1028,14 @@
           **kwargs: additional members to include in the Jwk (e.g. kid, use)
 
         Returns:
             the matching `Jwk` instance
 
         Raises:
             TypeError: if the key type is not supported
-
         """
         for cryptography_class, jwk_class in cls.cryptography_key_types.items():
             if isinstance(cryptography_key, cryptography_class):
                 return jwk_class.from_cryptography_key(cryptography_key, **kwargs)
 
         raise TypeError(
             f"Unsupported Jwk class for this Key Type: {type(cryptography_key).__name__}"
@@ -1056,15 +1044,14 @@
     def _to_cryptography_key(self) -> Any:
         """Return a key from the `cryptography` library that matches this Jwk.
 
         This is implemented by subclasses.
 
         Returns:
             a `cryptography`key instance initialized from the current key
-
         """
         raise NotImplementedError
 
     @classmethod
     def from_pem(
         cls,
         der: Union[bytes, str],
@@ -1076,15 +1063,14 @@
         Args:
           der: the PEM encoded data to load
           password: the password to decrypt the PEM, if required. Should be bytes. If it is a string, it will be encoded with UTF-8.
           **kwargs: additional members to include in the `Jwk` (e.g. `kid`, `use`)
 
         Returns:
             a `Jwk` instance from the loaded key
-
         """
         der = der.encode() if isinstance(der, str) else der
         password = password.encode("UTF-8") if isinstance(password, str) else password
 
         try:
             cryptography_key = serialization.load_pem_private_key(der, password)
         except Exception as private_exc:
@@ -1213,15 +1199,14 @@
         Args:
             alg: intended algorithm to use with the generated key
             kty: key type identifier
             **kwargs: specific parameters depending on the type of key, or additional members to include in the `Jwk`
 
         Returns:
             a `Jwk` instance with a generated key
-
         """
         if alg:
             key = cls.generate_for_alg(alg=alg, **kwargs)
             if kty is not None and key.kty != kty:
                 raise ValueError(
                     f"Incompatible `{alg=}` and `{kty=}` parameters. "
                     f"`{alg=}` points to key with `kty='{key.kty}'`."
@@ -1281,15 +1266,14 @@
             alg: the alg to use, if not present in this Jwk
             with_alg: whether to include an `alg` parameter
             with_use: whether to include a `use` parameter
             with_key_ops: whether to include a `key_ops` parameter
 
         Returns:
             a Jwk with the same key, with `alg`, `use` and `key_ops` parameters.
-
         """
         alg = alg or self.alg
 
         if not alg:
             raise ExpectedAlgRequired(
                 "An algorithm is required to set the usage parameters"
             )
@@ -1305,15 +1289,16 @@
             jwk["key_ops"] = jwk.key_ops
 
         return jwk
 
     def minimize(self) -> Jwk:
         """Strip out any optional or non-standard parameter from that key.
 
-        This will remove `alg`, `use`, `key_ops`, optional parameters from RSA keys, and other unknown parameters.
+        This will remove `alg`, `use`, `key_ops`, optional parameters from RSA keys, and other
+        unknown parameters.
 
         """
         jwk = self.copy()
         for key in self.keys():
             if key == "kty" or key in self.PARAMS and self.PARAMS[key].is_required:
                 continue
             del jwk[key]
@@ -1329,15 +1314,17 @@
 def to_jwk(
     key: Any,
     *,
     kty: Optional[str] = None,
     is_private: Optional[bool] = None,
     is_symmetric: Optional[bool] = None,
 ) -> Jwk:
-    """Convert any supported kind of key to a Jwk, and optionally check if that key is private or symmetric.
+    """Convert any supported kind of key to a `Jwk`.
+
+    This optionally check if that key is private or symmetric.
 
     The key can be any type supported by Jwk:
     - a `cryptography` key instance
     - a bytes, to initialize a symmetric key
     - a JWK, as a dict or as a JSON formatted string
     - an existing Jwk instance
     If the supplied param is already a Jwk, it is left untouched.
@@ -1346,11 +1333,10 @@
         key: the key material
         kty: the expected key type
         is_private: if `True`, check if the key is private, if `False`, check if it is public, if `None`, do nothing
         is_symmetric: if `True`, check if the key is symmetric, if `False`, check if it is asymmetric, if `None`, do nothing
 
     Returns:
         a Jwk key
-
     """
     jwk = key if isinstance(key, Jwk) else Jwk(key)
     return jwk.check(kty=kty, is_private=is_private, is_symmetric=is_symmetric)
```

### Comparing `jwskate-0.7.0/jwskate/jwk/ec.py` & `jwskate-0.8.0/jwskate/jwk/ec.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     """Raised when an unsupported Elliptic Curve is requested."""
 
 
 class ECJwk(Jwk):
     """Represent an Elliptic Curve key in JWK format.
 
     Elliptic Curve keys have Key Type `"EC"`.
+
     """
 
     KTY = KeyTypes.EC
 
     CRYPTOGRAPHY_PRIVATE_KEY_CLASSES = (ec.EllipticCurvePrivateKey,)
 
     CRYPTOGRAPHY_PUBLIC_KEY_CLASSES = (ec.EllipticCurvePublicKey,)
@@ -105,15 +106,14 @@
 
     @property
     def curve(self) -> EllipticCurve:
         """Get the `EllipticCurve` instance for this key.
 
         Returns:
             the `EllipticCurve` instance
-
         """
         return self.get_curve(self.crv)
 
     @classmethod
     def public(cls, *, crv: str, x: int, y: int, **params: str) -> ECJwk:
         """Initialize a public `ECJwk` from its public parameters.
 
@@ -121,15 +121,14 @@
           crv: the curve to use
           x: the x coordinate
           y: the y coordinate
           **params: additional member to include in the Jwk
 
         Returns:
           an ECJwk initialized with the supplied parameters
-
         """
         coord_size = cls.get_curve(crv).coordinate_size
         return cls(
             dict(
                 kty=cls.KTY,
                 crv=crv,
                 x=BinaPy.from_int(x, length=coord_size).to("b64u").ascii(),
@@ -226,15 +225,19 @@
                 x=self.x_coordinate,
                 y=self.y_coordinate,
                 curve=self.curve.cryptography_curve,
             ).public_key()
 
     @property
     def coordinate_size(self) -> int:
-        """The coordinate size to use with the key curve. This is 32, 48, or 66 bits."""
+        """The coordinate size to use with the key curve.
+
+        This is 32, 48, or 66 bits.
+
+        """
         return self.curve.coordinate_size
 
     @cached_property
     def x_coordinate(self) -> int:
         """Return the *x coordinate*, parameter `x` from this `ECJwk`."""
         return BinaPy(self.x).decode_from("b64u").to_int()
```

### Comparing `jwskate-0.7.0/jwskate/jwk/jwks.py` & `jwskate-0.8.0/jwskate/jwk/jwks.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 
     @property
     def jwks(self) -> List[Jwk]:
         """Return the list of keys from this JwkSet, as `Jwk` instances.
 
         Returns:
             a list of `Jwk`
-
         """
         return self.get("keys", [])
 
     def get_jwk_by_kid(self, kid: str) -> Jwk:
         """Return a Jwk from this JwkSet, based on its kid.
 
         Args:
@@ -63,15 +62,15 @@
         Returns:
             the key with the matching Key ID
 
         Raises:
             KeyError: if no key matches
 
         """
-        jwk = next(filter(lambda jwk: jwk.get("kid") == kid, self.jwks), None)
+        jwk = next(filter(lambda j: j.get("kid") == kid, self.jwks), None)
         if isinstance(jwk, Jwk):
             return jwk
         raise KeyError(kid)
 
     def __len__(self) -> int:
         """Return the number of Jwk in this JwkSet.
 
@@ -79,53 +78,52 @@
             the number of keys
 
         """
         return len(self.jwks)
 
     def add_jwk(
         self,
-        jwk: Union[Jwk, Dict[str, Any]],
+        key: Union[Jwk, Dict[str, Any], Any],
         kid: Optional[str] = None,
         use: Optional[str] = None,
     ) -> str:
         """Add a Jwk in this JwkSet.
 
         Args:
-          jwk: the Jwk to add (either a `Jwk` instance, or a dict containing the Jwk parameters)
+          key: the Jwk to add (either a `Jwk` instance, or a dict containing the Jwk parameters)
           kid: the kid to use, if `jwk` doesn't contain one
           use: the defined use for the added Jwk
 
         Returns:
           the kid from the added Jwk (it may be generated if no kid is provided)
 
         """
-        jwk = to_jwk(jwk)
+        key = to_jwk(key)
 
         self.setdefault("keys", [])
 
-        kid = jwk.get("kid", kid)
+        kid = key.get("kid", kid)
         if not kid:
-            kid = jwk.thumbprint()
-        jwk["kid"] = kid
-        use = jwk.get("use", use)
+            kid = key.thumbprint()
+        key["kid"] = kid
+        use = key.get("use", use)
         if use:
-            jwk["use"] = use
-        self.jwks.append(jwk)
+            key["use"] = use
+        self.jwks.append(key)
 
         return kid
 
     def remove_jwk(self, kid: str) -> None:
         """Remove a Jwk from this JwkSet, based on a `kid`.
 
         Args:
           kid: the `kid` from the key to be removed.
 
         Raises:
             KeyError: if no key matches
-
         """
         try:
             jwk = self.get_jwk_by_kid(kid)
             self.jwks.remove(jwk)
         except KeyError:
             pass
```

### Comparing `jwskate-0.7.0/jwskate/jwk/oct.py` & `jwskate-0.8.0/jwskate/jwk/oct.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """This module implements JWK representing Symmetric keys."""
 
 from __future__ import annotations
 
+import warnings
 from typing import Any, List, Optional, SupportsBytes, Tuple, Union
 
 from binapy import BinaPy
 from typing_extensions import override
 
 from jwskate.jwa import (
     A128CBC_HS256,
@@ -19,26 +20,29 @@
     A256CBC_HS512,
     A256GCM,
     A256GCMKW,
     A256KW,
     HS256,
     HS384,
     HS512,
+    BaseAesKeyWrap,
+    BaseHMACSigAlg,
     BaseSymmetricAlg,
     DirectKeyUse,
 )
 
-from .. import KeyTypes
+from .. import BaseAESEncryptionAlg, KeyTypes
 from .base import Jwk, JwkParameter
 
 
 class SymmetricJwk(Jwk):
     """Represent a Symmetric key in JWK format.
 
     Symmetric keys have key type `"oct"`.
+
     """
 
     KTY = KeyTypes.OCT
     CRYPTOGRAPHY_PRIVATE_KEY_CLASSES = (bytes,)
     CRYPTOGRAPHY_PUBLIC_KEY_CLASSES = (bytes,)
 
     PARAMS = {
@@ -95,23 +99,51 @@
 
         Args:
           k: the key to use
           **params: additional members to include in the `Jwk`
 
         Returns:
           the resulting `SymmetricJwk`
-
         """
         return cls(dict(kty=cls.KTY, k=BinaPy(k).to("b64u").ascii(), **params))
 
     @classmethod
     @override
-    def generate(cls, *, key_size: int = 128, **params: Any) -> SymmetricJwk:
+    def generate(
+        cls, *, alg: Optional[str] = None, key_size: Optional[int] = None, **params: Any
+    ) -> SymmetricJwk:
+        if alg:
+            alg_class = cls._get_alg_class(alg)
+            # special cases for AES or HMAC based algs which require a specific key size
+            if issubclass(alg_class, (BaseAESEncryptionAlg, BaseAesKeyWrap)):
+                if key_size is not None and key_size != alg_class.key_size:
+                    raise ValueError(
+                        f"Key for {alg} must be exactly {alg_class.key_size} bits. "
+                        "You should remove the `key_size` parameter to generate a key of the appropriate length."
+                    )
+                key_size = alg_class.key_size
+            elif issubclass(alg_class, BaseHMACSigAlg):
+                if key_size is not None and key_size < alg_class.min_key_size:
+                    warnings.warn(
+                        f"Symmetric keys to use with {alg} should be at least {alg_class.min_key_size} bits "
+                        "in order to make the key at least as hard to brute-force as the signature. "
+                        f"You requested a key size of {key_size} bits."
+                    )
+                else:
+                    key_size = alg_class.min_key_size
+
+        if key_size is None:
+            warnings.warn(
+                "Please provide a key_size or an alg parameter for jwskate to know the number of bits to generate. "
+                "Defaulting to 128 bits."
+            )
+            key_size = 128
+
         key = BinaPy.random_bits(key_size)
-        return cls.from_bytes(key, **params)
+        return cls.from_bytes(key, alg=alg, **params)
 
     @classmethod
     @override
     def from_cryptography_key(
         cls, cryptography_key: Any, **params: Any
     ) -> SymmetricJwk:
         return cls.from_bytes(cryptography_key, **params)
```

### Comparing `jwskate-0.7.0/jwskate/jwk/okp.py` & `jwskate-0.8.0/jwskate/jwk/okp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """This module implements JWK representing Octet Key Pairs from [RFC8037].
 
-[RFC8037]: https://www.rfc-editor.org/rfc/rfc8037.html
+[RFC8037]
+: https: //www.rfc-editor.org/rfc/rfc8037.html
 
 """
 
 from __future__ import annotations
 
 from functools import cached_property
 from typing import Any, Mapping, Optional
@@ -36,14 +37,15 @@
     """Raised when an unsupported OKP curve is requested."""
 
 
 class OKPJwk(Jwk):
     """Represent an Octet Key Pair keys in JWK format.
 
     Octet Key Pair keys have Key Type `"OKP"`.
+
     """
 
     KTY = KeyTypes.OKP
 
     CRYPTOGRAPHY_PRIVATE_KEY_CLASSES = (
         ed25519.Ed25519PrivateKey,
         ed448.Ed448PrivateKey,
@@ -98,15 +100,14 @@
           crv: a curve identifier
 
         Returns:
             the matching `OKPCurve` instance
 
         Raises:
             UnsupportedOKPCurve: if the curve is not supported
-
         """
         curve = cls.CURVES.get(crv)
         if curve is None:
             raise UnsupportedOKPCurve(crv)
         return curve
 
     @property
@@ -147,15 +148,14 @@
             private_key: the 32, 56 or 57 bytes private key, as raw `bytes`
             crv: the curve identifier to use
             use: the key usage
             **kwargs: additional members to include in the `Jwk`
 
         Returns:
             the matching `OKPJwk`
-
         """
         if crv and use:
             if (crv in ("Ed25519", "Ed448") and use != "sig") or (
                 crv in ("X25519", "X448") and use != "enc"
             ):
                 raise ValueError(
                     f"Inconsistent `crv={crv}` and `use={use}` parameters. "
@@ -277,15 +277,14 @@
         Args:
           crv: the key curve
           x: the public key
           **params: additional members to include in the `Jwk`
 
         Returns:
             the resulting `OKPJwk`
-
         """
         return cls(dict(kty=cls.KTY, crv=crv, x=BinaPy(x).to("b64u").ascii(), **params))
 
     @classmethod
     def private(cls, *, crv: str, x: bytes, d: bytes, **params: Any) -> OKPJwk:
         """Initialize a private `OKPJwk` based on the provided parameters.
 
@@ -293,15 +292,14 @@
           crv: the OKP curve
           x: the public key
           d: the private key
           **params: additional members to include in the `Jwk`
 
         Returns:
             the resulting `OKPJwk`
-
         """
         return cls(
             dict(
                 kty=cls.KTY,
                 crv=crv,
                 x=BinaPy(x).to("b64u").ascii(),
                 d=BinaPy(d).to("b64u").ascii(),
```

### Comparing `jwskate-0.7.0/jwskate/jwk/rsa.py` & `jwskate-0.8.0/jwskate/jwk/rsa.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from .base import Jwk, JwkParameter
 
 
 class RSAJwk(Jwk):
     """Represent an RSA key in JWK format.
 
     RSA (Rivest-Shamir-Adleman) keys have Key Type `"RSA"`.
+
     """
 
     KTY = KeyTypes.RSA
     CRYPTOGRAPHY_PRIVATE_KEY_CLASSES = (rsa.RSAPrivateKey,)
     CRYPTOGRAPHY_PUBLIC_KEY_CLASSES = (rsa.RSAPublicKey,)
 
     PARAMS = {
@@ -133,15 +134,14 @@
         Args:
           n: the modulus
           e: the exponent
           **params: additional parameters to include in the `Jwk`
 
         Returns:
           a `RsaJwk` initialized from the provided parameters
-
         """
         return cls(
             dict(
                 kty=cls.KTY,
                 n=BinaPy.from_int(n).to("b64u").ascii(),
                 e=BinaPy.from_int(e).to("b64u").ascii(),
                 **params,
@@ -173,15 +173,14 @@
           dp: the first factor CRT exponent
           dq: the second factor CRT exponent
           qi: the first CRT coefficient
           **params: additional parameters to include in the `Jwk`
 
         Returns:
             a `RSAJwk` initialized from the given parameters
-
         """
         return cls(
             dict(
                 kty=cls.KTY,
                 n=BinaPy.from_int(n).to("b64u").ascii(),
                 e=BinaPy.from_int(e).to("b64u").ascii(),
                 d=BinaPy.from_int(d).to("b64u").ascii(),
@@ -205,15 +204,14 @@
 
         Args:
           key_size: the key size to use for the generated key, in bits
           **params: additional parameters to include in the `Jwk`
 
         Returns:
           a generated `RSAJwk`
-
         """
         private_key = rsa.generate_private_key(65537, key_size=key_size)
         pn = private_key.private_numbers()
         return cls.private(
             n=pn.public_numbers.n,
             e=pn.public_numbers.e,
             d=pn.d,
@@ -281,15 +279,17 @@
     def first_crt_coefficient(self) -> int:
         """Return the first CRT coefficient `qi` from this `Jwk`."""
         if "qi" in self:
             return BinaPy(self.qi).decode_from("b64u").to_int()
         return rsa.rsa_crt_iqmp(self.first_prime_factor, self.second_prime_factor)
 
     def with_optional_private_parameters(self) -> RSAJwk:
-        """Compute the optional RSA private parameters and return a new `Jwk` with those additional params included.
+        """Compute the optional RSA private parameters.
+
+        This returns a new `Jwk` with those additional params included.
 
         The optional parameters are:
 
         - p: first prime factor
         - q: second prime factor
         - dp: first factor Chinese Remainder Theorem exponent
         - dq: second factor Chinese Remainder Theorem exponent
```

### Comparing `jwskate-0.7.0/jwskate/jws/compact.py` & `jwskate-0.8.0/jwskate/jws/compact.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     """Represents a Json Web Signature (JWS), using compact serialization, as defined in RFC7515.
 
     Args:
         value: the JWS token value
 
     """
 
-    def __init__(self, value: Union[bytes, str]):
-        super().__init__(value)
+    def __init__(self, value: Union[bytes, str], max_size: int = 16 * 1024):
+        super().__init__(value, max_size)
 
         if self.value.count(b".") != 2:
             raise InvalidJws(
                 "A JWS must contain a header, a payload and a signature, separated by dots"
             )
 
         header, payload, signature = BinaPy(self.value).split(b".")
@@ -59,49 +59,49 @@
                 "Invalid JWS signature: it must be a Base64URL-encoded binary data (bytes)"
             )
 
     @classmethod
     def sign(
         cls,
         payload: Union[bytes, SupportsBytes],
-        jwk: Union[Jwk, Dict[str, Any]],
+        key: Union[Jwk, Dict[str, Any], Any],
         alg: Optional[str] = None,
         extra_headers: Optional[Dict[str, Any]] = None,
     ) -> JwsCompact:
         """Sign a payload and returns the resulting JwsCompact.
 
         Args:
           payload: the payload to sign
-          jwk: the jwk to use to sign this payload
+          key: the jwk to use to sign this payload
           alg: the alg to use
           extra_headers: additional headers to add to the Jws Headers
 
         Returns:
           the resulting token
 
         """
-        jwk = to_jwk(jwk)
+        key = to_jwk(key)
 
         if not isinstance(payload, bytes):
             payload = bytes(payload)
 
         headers = dict(extra_headers or {}, alg=alg)
-        kid = jwk.get("kid")
+        kid = key.get("kid")
         if kid:
             headers["kid"] = kid
 
         signed_part = JwsSignature.assemble_signed_part(headers, payload)
-        signature = jwk.sign(signed_part, alg=alg)
+        signature = key.sign(signed_part, alg=alg)
         return cls.from_parts(signed_part, signature)
 
     @classmethod
     def from_parts(
         cls,
         signed_part: Union[bytes, SupportsBytes, str],
-        signature: Union[bytes, SupportsBytes, str],
+        signature: Union[bytes, SupportsBytes],
     ) -> JwsCompact:
         """Construct a JWS token based on its signed part and signature values.
 
         Signed part is the concatenation of the header and payload, both encoded in Base64-Url, and joined by a dot.
 
         Args:
           signed_part: the signed part
@@ -112,16 +112,14 @@
 
         """
         if isinstance(signed_part, str):
             signed_part = signed_part.encode("ascii")
         if not isinstance(signed_part, bytes):
             signed_part = bytes(signed_part)
 
-        if isinstance(signature, str):
-            signature = signature.encode("ascii")
         if not isinstance(signature, bytes):
             signature = bytes(signature)
 
         return cls(b".".join((signed_part, BinaPy(signature).to("b64u"))))
 
     @cached_property
     def signed_part(self) -> bytes:
@@ -131,32 +129,32 @@
             the signed part
 
         """
         return b".".join(self.value.split(b".", 2)[:2])
 
     def verify_signature(
         self,
-        jwk: Union[Jwk, Dict[str, Any]],
+        key: Union[Jwk, Dict[str, Any], Any],
         *,
         alg: Optional[str] = None,
         algs: Optional[Iterable[str]] = None,
     ) -> bool:
         """Verify the signature from this JwsCompact using a Jwk.
 
         Args:
-          jwk: the Jwk to use to validate this signature
+          key: the Jwk to use to validate this signature
           alg: the alg to use, if there is only 1 allowed
           algs: the allowed algs, if here are several
 
         Returns:
          `True` if the signature matches, `False` otherwise
 
         """
-        jwk = to_jwk(jwk)
-        return jwk.verify(self.signed_part, self.signature, alg=alg, algs=algs)
+        key = to_jwk(key)
+        return key.verify(self.signed_part, self.signature, alg=alg, algs=algs)
 
     def flat_json(self, unprotected_header: Any = None) -> JwsJsonFlat:
         """Create a JWS in JSON flat format based on this Compact JWS.
 
         Args:
           unprotected_header: optional unprotected header to include in the JWS JSON
```

### Comparing `jwskate-0.7.0/jwskate/jws/json.py` & `jwskate-0.8.0/jwskate/jws/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,36 +47,36 @@
             content["header"] = self.header
         return JwsSignature(content)
 
     @classmethod
     def sign(
         cls,
         payload: bytes,
-        jwk: Union[Jwk, Dict[str, Any]],
+        key: Union[Jwk, Dict[str, Any], Any],
         alg: Optional[str] = None,
         extra_protected_headers: Optional[Mapping[str, Any]] = None,
         header: Optional[Any] = None,
         **kwargs: Any,
     ) -> JwsJsonFlat:
         """Signs a payload into a JWS in JSON flat format.
 
         Args:
             payload: the data to sign.
-            jwk: the key to use
+            key: the key to use
             alg: the signature alg to use
             extra_protected_headers: additional protected headers to include
             header: the unprotected header to include
             **kwargs: extra attributes to include in the JWS
 
         Returns:
             The JWS with the payload, signature, header and extra claims.
 
         """
         signature = super().sign(
-            payload, jwk, alg, extra_protected_headers, header, **kwargs
+            payload, key, alg, extra_protected_headers, header, **kwargs
         )
         signature["payload"] = BinaPy(payload).to("b64u").ascii()
         return cls(signature)
 
     def generalize(self) -> JwsJsonGeneral:
         """Create a JWS in JSON general format from this JWS in JSON flat.
 
@@ -112,31 +112,31 @@
             A `JwsCompact` with the same payload and signature.
 
         """
         return JwsCompact.from_parts(self.signed_part(), self.signature)
 
     def verify_signature(
         self,
-        jwk: Union[Jwk, Dict[str, Any]],
+        key: Union[Jwk, Dict[str, Any], Any],
         *,
         alg: Optional[str] = None,
         algs: Optional[Iterable[str]] = None,
     ) -> bool:
         """Verify this JWS signature with a given key.
 
         Args:
-            jwk: the key to use to validate this signature.
+            key: the key to use to validate this signature.
             alg: the signature alg, if only 1 is allowed.
             algs: the allowed signature algs, if there are several.
 
         Returns:
             `True` if the signature is verified, `False` otherwise.
 
         """
-        return self.jws_signature.verify(self.payload, jwk, alg=alg, algs=algs)
+        return self.jws_signature.verify(self.payload, key, alg=alg, algs=algs)
 
 
 class JwsJsonGeneral(BaseJsonDict):
     """Represents a JWS in JSON general format (possibly with multiple signatures)."""
 
     @cached_property
     def payload(self) -> bytes:
@@ -196,43 +196,42 @@
 
     @cached_property
     def signatures(self) -> List[JwsSignature]:
         """The list of `JwsSignature` from this JWS.
 
         Returns:
             The list of signatures from this JWS.
-
         """
         signatures = self.get("signatures")
         if signatures is None:
             raise AttributeError("This Jws JSON does not contain a 'signatures' member")
         return [JwsSignature(sig) for sig in signatures]
 
     def add_signature(
         self,
-        jwk: Union[Jwk, Dict[str, Any]],
+        key: Union[Jwk, Dict[str, Any], Any],
         alg: Optional[str] = None,
         extra_protected_headers: Optional[Mapping[str, Any]] = None,
         header: Optional[Mapping[str, Any]] = None,
     ) -> JwsJsonGeneral:
         """Add a new signature in this JWS.
 
         Args:
-            jwk: the private key to use
+            key: the private key to use
             alg: the signature algorithm
             extra_protected_headers: additional headers to include, as a {key: value} mapping
             header: the raw unprotected header to include in the signature
 
         Returns:
             the same JWS with the new signature included.
 
         """
         self.setdefault("signatures", [])
         self["signatures"].append(
-            JwsSignature.sign(self.payload, jwk, alg, extra_protected_headers, header)
+            JwsSignature.sign(self.payload, key, alg, extra_protected_headers, header)
         )
         return self
 
     def signed_part(
         self,
         signature_chooser: Callable[
             [List[JwsSignature]], JwsSignature
@@ -297,28 +296,28 @@
             protected=signature.protected,
             header=signature.header,
             signature=signature.signature,
         )
 
     def verify_signature(
         self,
-        jwk: Union[Jwk, Dict[str, Any]],
+        key: Union[Jwk, Dict[str, Any], Any],
         *,
         alg: Optional[str] = None,
         algs: Optional[Iterable[str]] = None,
     ) -> bool:
         """Verify the signatures from this JWS.
 
         It will try to validate each signature with the given key, and returns `True` if at least one signature verifies.
         Args:
-            jwk: the public key to use
+            key: the public key to use
             alg: the signature algorithm to use, if only 1 is allowed.
             algs: the allowed signature algorithms, if there are several.
 
         Returns:
             `True` if any of the signature verifies with the given key, `False` otherwise.
 
         """
         for signature in self.signatures:
-            if signature.verify(self.payload, jwk, alg=alg, algs=algs):
+            if signature.verify(self.payload, key, alg=alg, algs=algs):
                 return True
         return False
```

### Comparing `jwskate-0.7.0/jwskate/jws/signature.py` & `jwskate-0.8.0/jwskate/jws/signature.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,43 +96,43 @@
             raise AttributeError("This Jws JSON does not contain a 'signature' member")
         return BinaPy(signature).decode_from("b64u")
 
     @classmethod
     def sign(
         cls: Type[S],
         payload: bytes,
-        jwk: Union[Jwk, Dict[str, Any]],
+        key: Union[Jwk, Dict[str, Any], Any],
         alg: Optional[str] = None,
         extra_protected_headers: Optional[Mapping[str, Any]] = None,
         header: Optional[Any] = None,
         **kwargs: Any,
     ) -> S:
         """Sign a payload and return the generated JWS signature.
 
         Args:
           payload: the raw data to sign
-          jwk: the signature key to use
+          key: the signature key to use
           alg: the signature algorithm to use
           extra_protected_headers: additional protected headers to include, if any
           header: the unprotected header, if any.
           **kwargs: additional members to include in this signature
 
         Returns:
             The generated signature.
 
         """
-        jwk = to_jwk(jwk)
+        key = to_jwk(key)
 
         headers = dict(extra_protected_headers or {}, alg=alg)
-        kid = jwk.get("kid")
+        kid = key.get("kid")
         if kid:
             headers["kid"] = kid
 
         signed_part = JwsSignature.assemble_signed_part(headers, payload)
-        signature = jwk.sign(signed_part, alg=alg)
+        signature = key.sign(signed_part, alg=alg)
         return cls.from_parts(
             protected=headers, signature=signature, header=header, **kwargs
         )
 
     @classmethod
     def assemble_signed_part(
         cls, headers: Dict[str, Any], payload: Union[bytes, str]
@@ -156,27 +156,27 @@
                 BinaPy(payload).to("b64u"),
             )
         )
 
     def verify(
         self,
         payload: bytes,
-        jwk: Union[Jwk, Dict[str, Any]],
+        key: Union[Jwk, Dict[str, Any], Any],
         *,
         alg: Optional[str] = None,
         algs: Optional[Iterable[str]] = None,
     ) -> bool:
         """Verify this signature against the given payload using the provided key.
 
         Args:
           payload: the raw payload
-          jwk: the validation key to use
+          key: the validation key to use
           alg: the signature alg t if only 1 is allowed
           algs: the allowed signature algs, if there are several
 
         Returns:
             `True` if the signature is verifier, `False` otherwise
 
         """
-        jwk = to_jwk(jwk)
+        key = to_jwk(key)
         signed_part = self.assemble_signed_part(self.protected, payload)
-        return jwk.verify(signed_part, self.signature, alg=alg, algs=algs)
+        return key.verify(signed_part, self.signature, alg=alg, algs=algs)
```

### Comparing `jwskate-0.7.0/jwskate/jwt/base.py` & `jwskate-0.8.0/jwskate/jwt/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -18,79 +18,108 @@
 class InvalidJwt(ValueError):
     """Raised when an invalid Jwt is parsed."""
 
 
 class Jwt(BaseCompactToken):
     """Represents a Json Web Token."""
 
-    def __new__(cls, value: Union[bytes, str]) -> Union[SignedJwt, JweCompact, Jwt]:  # type: ignore[misc]
+    def __new__(cls, value: Union[bytes, str], max_size: int = 16 * 1024) -> Union[SignedJwt, JweCompact, Jwt]:  # type: ignore[misc]
         """Allow parsing both Signed and Encrypted JWTs.
 
         This returns the appropriate subclass or instance depending on the number of dots (.) in the serialized JWT.
 
         Args:
             value: the token value
+            max_size: maximum allowed size for the token
 
         """
         if not isinstance(value, bytes):
             value = value.encode("ascii")
 
         if cls == Jwt:
             if value.count(b".") == 2:
                 from .signed import SignedJwt
 
                 return super().__new__(SignedJwt)
             elif value.count(b".") == 4:
                 from ..jwe import JweCompact
 
-                return JweCompact(value)
+                return JweCompact(value, max_size)
 
         return super().__new__(cls)
 
     @classmethod
     def sign(
         cls,
         claims: Dict[str, Any],
-        jwk: Union[Jwk, Dict[str, Any]],
+        key: Union[Jwk, Dict[str, Any], Any],
         alg: Optional[str] = None,
         extra_headers: Optional[Dict[str, Any]] = None,
     ) -> SignedJwt:
-        """Sign a JSON payload with a `Jwk` and returns the resulting `SignedJwt`.
+        """Sign a JSON payload with a private key and return the resulting `SignedJwt`.
 
         This method cannot generate a token without a signature. If you want to use an unsigned token (with alg=none),
         use `.unprotected()` instead.
 
         Args:
           claims: the payload to sign
-          jwk: the Jwk to use for signing
+          key: the key to use for signing
           alg: the alg to use for signing
           extra_headers: additional headers to include in the Jwt
 
         Returns:
           the resulting token
-
         """
-        from .signed import SignedJwt
-
-        jwk = to_jwk(jwk)
+        key = to_jwk(key)
 
-        alg = alg or jwk.get("alg")
+        alg = alg or key.get("alg")
 
         if alg is None:
             raise ValueError("a signing alg is required")
 
         extra_headers = extra_headers or {}
         headers = dict(alg=alg, **extra_headers)
-        if jwk.kid:
-            headers["kid"] = jwk.kid
+        if key.kid:
+            headers["kid"] = key.kid
+
+        return cls.sign_arbitrary(claims=claims, headers=headers, key=key, alg=alg)
+
+    @classmethod
+    def sign_arbitrary(
+        self,
+        claims: Dict[str, Any],
+        headers: Dict[str, Any],
+        key: Union[Jwk, Dict[str, Any], Any],
+        alg: Optional[str] = None,
+    ) -> SignedJwt:
+        """Sign provided headers and claims with a private key and return the resulting `SignedJwt`.
+
+        This does not check the consistency between headers, key, alg and kid.
+        DO NOT USE THIS METHOD UNLESS YOU KNOW WHAT YOU ARE DOING!!!
+        Use `Jwt.sign()` to make sure you are signing tokens properly.
+
+        Args:
+             claims: the payload to sign
+             headers: the headers to sign
+             key: the key to use for signing
+             alg: the alg to use for signing
+        """
+        from .signed import SignedJwt
+
+        key = to_jwk(key)
+
+        alg = alg or key.get("alg")
+
+        if alg is None:
+            raise ValueError("a signing alg is required")
 
         headers_part = BinaPy.serialize_to("json", headers).to("b64u")
         claims_part = BinaPy.serialize_to("json", claims).to("b64u")
         signed_value = b".".join((headers_part, claims_part))
-        signature = jwk.sign(signed_value, alg=alg).to("b64u")
+        signature = key.sign(signed_value, alg=alg).to("b64u")
         return SignedJwt(b".".join((signed_value, signature)))
 
     @classmethod
     def unprotected(
         cls,
         claims: Dict[str, Any],
         extra_headers: Optional[Dict[str, Any]] = None,
@@ -115,119 +144,121 @@
         signature = b""
         return SignedJwt(b".".join((signed_value, signature)))
 
     @classmethod
     def sign_and_encrypt(
         cls,
         claims: Dict[str, Any],
-        sign_jwk: Union[Jwk, Dict[str, Any]],
-        enc_jwk: Union[Jwk, Dict[str, Any]],
+        sign_key: Union[Jwk, Dict[str, Any], Any],
+        enc_key: Union[Jwk, Dict[str, Any], Any],
         enc: str,
         *,
         sign_alg: Optional[str] = None,
         enc_alg: Optional[str] = None,
         sign_extra_headers: Optional[Dict[str, Any]] = None,
         enc_extra_headers: Optional[Dict[str, Any]] = None,
     ) -> JweCompact:
         """Sign a JWT, then encrypt it as JWE payload.
 
         This is a convenience method to do both the signing and encryption, in appropriate order.
 
         Args:
           claims: the payload to encrypt
-          sign_jwk: the Jwk to use for signature
+          sign_key: the Jwk to use for signature
           sign_alg: the alg to use for signature
           sign_extra_headers: additional headers for the inner signed JWT
-          enc_jwk: the Jwk to use for encryption
+          enc_key: the Jwk to use for encryption
           enc_alg: the alg to use for CEK encryption
           enc: the alg to use for payload encryption
           enc_extra_headers: additional headers for the outer encrypted JWE
 
         Returns:
           the resulting JWE token, with the signed JWT as payload
 
         """
         enc_extra_headers = enc_extra_headers or {}
         enc_extra_headers.setdefault("cty", "JWT")
 
         inner_jwt = cls.sign(
-            claims, jwk=sign_jwk, alg=sign_alg, extra_headers=sign_extra_headers
+            claims, key=sign_key, alg=sign_alg, extra_headers=sign_extra_headers
         )
         jwe = JweCompact.encrypt(
-            inner_jwt, enc_jwk, enc=enc, alg=enc_alg, extra_headers=enc_extra_headers
+            inner_jwt, enc_key, enc=enc, alg=enc_alg, extra_headers=enc_extra_headers
         )
         return jwe
 
     @classmethod
     def decrypt_nested_jwt(
-        cls, jwe: Union[str, JweCompact], jwk: Union[Jwk, Dict[str, Any]]
+        cls, jwe: Union[str, JweCompact], key: Union[Jwk, Dict[str, Any], Any]
     ) -> Jwt:
         """Decrypt a JWE that contains a nested JWT.
 
         It will return a [Jwt] instance for the inner JWT.
 
         Args:
             jwe: the JWE containing a nested Token
-            jwk: the decryption key
+            key: the decryption key
 
         Returns:
             the inner JWT
 
         Raises:
             InvalidJwt: if the inner JWT is not valid
 
         """
         if not isinstance(jwe, JweCompact):
             jwe = JweCompact(jwe)
-        cleartext = jwe.decrypt(jwk)
+        cleartext = jwe.decrypt(key)
         return Jwt(cleartext)
 
     @classmethod
     def decrypt_and_verify(
         cls,
         jwt: Union[str, JweCompact],
-        enc_jwk: Union[Jwk, Dict[str, Any]],
-        sig_jwk: Union[Jwk, Dict[str, Any], None],
+        enc_key: Union[Jwk, Dict[str, Any], Any],
+        sig_key: Union[Jwk, Dict[str, Any], None, Any],
         sig_alg: Optional[str] = None,
         sig_algs: Optional[Iterable[str]] = None,
     ) -> SignedJwt:
         """Decrypt then verify the signature of a JWT nested in a JWE.
 
         This can only be used with signed then encrypted Jwt, such as those produce by `Jwt.sign_and_encrypt()`.
 
         Args:
             jwt: the JWE containing a nested signed JWT
-            enc_jwk: the decryption key
-            sig_jwk: the signature verification key
+            enc_key: the decryption key
+            sig_key: the signature verification key
             sig_alg: the signature verification alg, if only 1 is allowed
             sig_algs: the signature verifications algs, if several are allowed
 
         Returns:
             the nested signed JWT, in clear-text, signature already verified
 
         Raises:
             InvalidJwt: if the JWT is not valid
             InvalidSignature: if the nested JWT signature is not valid
 
         """
         from .signed import InvalidSignature, SignedJwt
 
-        nested_jwt = cls.decrypt_nested_jwt(jwt, enc_jwk)
+        nested_jwt = cls.decrypt_nested_jwt(jwt, enc_key)
         if not isinstance(nested_jwt, SignedJwt):
             raise ValueError("Nested JWT is not signed", nested_jwt)
 
-        if sig_jwk:
-            if nested_jwt.verify_signature(sig_jwk, sig_alg, sig_algs):
+        if sig_key:
+            if nested_jwt.verify_signature(sig_key, sig_alg, sig_algs):
                 return nested_jwt
 
         raise InvalidSignature()
 
     @classmethod
     def timestamp(cls, delta_seconds: int = 0) -> int:
-        """Return an integer timestamp that is suitable for use in Jwt tokens `iat`, `exp` and `nbf` claims.
+        """Return an integer timestamp that is suitable for use in Jwt tokens.
+
+        Timestamps are used in particular for `iat`, `exp` and `nbf` claims.
 
         A timestamp is a number of seconds since January 1st, 1970 00:00:00 UTC, ignoring leap seconds.
 
         By default, the current timestamp is returned. You can include `delta_seconds` to have a timestamp
         a number of seconds in the future (if positive) or in the past (if negative).
 
         Args:
@@ -246,10 +277,9 @@
         Returned datetime is always in the UTC timezone.
 
         Args:
             timestamp: a timestamp from a JWT token
 
         Returns:
             the corresponding `datetime` in UTC timezone
-
         """
         return datetime.fromtimestamp(timestamp, tz=timezone.utc)
```

### Comparing `jwskate-0.7.0/jwskate/jwt/signed.py` & `jwskate-0.8.0/jwskate/jwt/signed.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,44 +76,43 @@
           the signed part as bytes
 
         """
         return b".".join(self.value.split(b".", 2)[:2])
 
     def verify_signature(
         self,
-        jwk: Union[Jwk, Dict[str, Any]],
+        key: Union[Jwk, Dict[str, Any], Any],
         alg: Optional[str] = None,
         algs: Optional[Iterable[str]] = None,
     ) -> bool:
         """Verify this JWT signature using a given key and algorithm(s).
 
         Args:
-          jwk: the private Jwk to use to verify the signature
+          key: the private Jwk to use to verify the signature
           alg: the alg to use to verify the signature, if only 1 is allowed
           algs: the allowed signature algs, if there are several
 
         Returns:
             `True` if the token signature is verified, `False` otherwise
 
         """
-        jwk = to_jwk(jwk)
+        key = to_jwk(key)
 
-        return jwk.verify(
+        return key.verify(
             data=self.signed_part, signature=self.signature, alg=alg, algs=algs
         )
 
     def is_expired(self, leeway: int = 0) -> Optional[bool]:
         """Check if this token is expired, based on its `exp` claim.
 
         Args:
             leeway: additional number of seconds for leeway.
 
         Returns:
             `True` if the token is expired, `False` if it's not, `None` if there is no `exp` claim.
-
         """
         exp = self.expires_at
         if exp is None:
             return None
         return exp < (datetime.now(timezone.utc) + timedelta(seconds=leeway))
 
     @cached_property
@@ -121,15 +120,14 @@
         """Get the *Expires At* (`exp`) date from this token.
 
         Returns:
           a `datetime` initialized from the `exp` claim, or `None` if there is no `exp` claim
 
         Raises:
             AttributeError: if the `exp` claim cannot be parsed to a date
-
         """
         exp = self.get_claim("exp")
         if not exp:
             return None
         try:
             exp_dt = Jwt.timestamp_to_datetime(exp)
             return exp_dt
@@ -141,15 +139,14 @@
         """Get the *Issued At* (`iat`) date from this token.
 
         Returns:
           a `datetime` initialized from the `iat` claim, or `None` if there is no `iat` claim
 
         Raises:
             AttributeError: if the `iss` claim cannot be parsed to a date
-
         """
         iat = self.get_claim("iat")
         if not iat:
             return None
         try:
             iat_dt = Jwt.timestamp_to_datetime(iat)
             return iat_dt
@@ -181,15 +178,14 @@
         """Get the *Issuer* (`iss`) claim from this token.
 
         Returns:
           the issuer, as `str`, or `None` if there is no `ìss` claim
 
         Raises:
             AttributeError: if the `ìss` claim value is not a string
-
         """
         iss = self.get_claim("iss")
         if iss is None or isinstance(iss, str):
             return iss
         raise AttributeError("iss has an unexpected type", type(iss))
 
     @cached_property
@@ -199,15 +195,14 @@
         If this token has a single audience, this will return a `list` anyway.
 
         Returns:
             the list of audiences from this token, from the `aud` claim.
 
         Raises:
             AttributeError: if the audience is an unexpected type
-
         """
         aud = self.get_claim("aud")
         if aud is None:
             return []
         if isinstance(aud, str):
             return [aud]
         if isinstance(aud, list):
@@ -219,15 +214,14 @@
         """Get the *Subject* (`sub`) from this token.
 
         Returns:
           the subject, as `str`, or `None` if there is no `sub` claim
 
         Raises:
             AttributeError: if the `sub` value is not a string
-
         """
         sub = self.get_claim("sub")
         if sub is None or isinstance(sub, str):
             return sub
         raise AttributeError("sub has an unexpected type", type(sub))
 
     @cached_property
@@ -235,15 +229,14 @@
         """Get the *JWT Token ID* (`jti`) from this token.
 
         Returns:
           the token identifier, as `str`, or `None` if there is no `jti` claim
 
         Raises:
           AttributeError: if the `jti` value is not a string
-
         """
         jti = self.get_claim("jti")
         if jti is None or isinstance(jti, str):
             return jti
         raise AttributeError("jti has an unexpected type", type(jti))
 
     def get_claim(self, key: str, default: Any = None) -> Any:
@@ -290,30 +283,28 @@
         return value
 
     def __str__(self) -> str:
         """Return the Jwt serialized value, as `str`.
 
         Returns:
             the serialized token value.
-
         """
         return self.value.decode()
 
     def __bytes__(self) -> bytes:
         """Return the Jwt serialized value, as `bytes`.
 
         Returns:
             the serialized token value.
-
         """
         return self.value
 
     def validate(
         self,
-        jwk: Union[Jwk, Dict[str, Any]],
+        key: Union[Jwk, Dict[str, Any], Any],
         *,
         alg: Optional[str] = None,
         algs: Optional[Iterable[str]] = None,
         issuer: Optional[str] = None,
         audience: Union[None, str] = None,
         check_exp: bool = True,
         **kwargs: Any,
@@ -323,32 +314,31 @@
         This verifies the signature using the provided `jwk` and `alg`, then checks the token issuer, audience and expiration date.
         This can also check custom claims using extra `kwargs`, whose values can be:
 
         - a static value (`str`, `int`, etc.): the value from the token will be compared "as-is"
         - a callable, taking the claim value as parameter: if that callable returns `True`, the claim is considered as valid
 
         Args:
-          jwk: the signing key to use to verify the signature.
+          key: the signing key to use to verify the signature.
           alg: the signature alg to use to verify the signature.
           algs: allowed signature algs, if several
           issuer: the expected issuer for this token.
           audience: the expected audience for this token.
           check_exp: ìf `True` (default), check that the token is not expired.
           **kwargs: additional claims to check
 
         Returns:
           Raises exceptions if any validation check fails.
 
         Raises:
           InvalidSignature: if the signature is not valid
           InvalidClaim: if a claim doesn't validate
           ExpiredJwt: if the expiration date is passed
-
         """
-        if not self.verify_signature(jwk, alg, algs):
+        if not self.verify_signature(key, alg, algs):
             raise InvalidSignature("Signature is not valid.")
 
         if issuer is not None:
             if self.issuer != issuer:
                 raise InvalidClaim("iss", "Unexpected issuer", self.issuer)
 
         if audience is not None:
```

### Comparing `jwskate-0.7.0/jwskate/jwt/signer.py` & `jwskate-0.8.0/jwskate/jwt/signer.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
                 iat=now,
                 exp=exp,
                 nbf=nbf,
                 jti=jti,
             ).items()
             if value is not None
         }
-        return Jwt.sign(claims, jwk=self.jwk, alg=self.alg, extra_headers=extra_headers)
+        return Jwt.sign(claims, key=self.jwk, alg=self.alg, extra_headers=extra_headers)
 
     def generate_jti(self) -> str:
         """Generate Jwt Token ID (jti) values.
 
         Default uses UUID4. Can be overridden in subclasses.
 
         Returns:
```

### Comparing `jwskate-0.7.0/jwskate/jwt/verifier.py` & `jwskate-0.8.0/jwskate/jwt/verifier.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,9 +128,10 @@
                     raise ValueError("No foo!")
 
 
             verifier.verify(
                 "eyJhbGciOiJIUzI1NiIsImtpZCI6ImlfdXRLRXhBS05jXy1hd3FEUkFVYmFoTWd5RGFLREdfTTc1S01Cd2xBdkEifQ.eyJpc3MiOiJodHRwczovL2Zvby5iYXIiLCJmb28iOiJZRVMiLCJpYXQiOjE1MTYyMzkwMjJ9.hk2vnymjcww8K-OcOkNCPUiJK-8Rj--RKJqsHSKe4jM"
             )
             ```
+
         """
         self.verifiers.append(verifier)
```

### Comparing `jwskate-0.7.0/jwskate/token.py` & `jwskate-0.8.0/jwskate/token.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,17 +110,17 @@
         return typ
 
     @cached_property
     def cty(self) -> str:
         """Get the Type (typ) from this token headers.
 
         Returns:
-            the `typ` value
+            the `cty` value
         Raises:
-            AttributeError: if the `typ` header value is not a string
+            AttributeError: if the `cty` header value is not a string
 
         """
         cty = self.get_header("cty")
         if cty is None or not isinstance(cty, str):  # pragma: no branch
             raise AttributeError("This token doesn't have a valid 'cty' header")
         return cty
```

### Comparing `jwskate-0.7.0/pyproject.toml` & `jwskate-0.8.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "jwskate"
-version = "0.7.0"
+version = "0.8.0"
 homepage = "https://github.com/guillp/jwskate"
 description = "A Pythonic implementation of Json Web Signature, Keys, Algorithms, Tokens and Encryption (RFC7514 to 7519), on top of the `cryptography` module."
 authors = ["Guillaume Pujol <guill.p.linux@gmail.com>"]
 readme = "README.md"
 license =  "MIT"
 classifiers=[
     'Development Status :: 3 - Alpha',
@@ -23,49 +23,43 @@
     { include = "tests", format = "sdist" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 cryptography = ">=3.4"
 typing-extensions = ">=4.3.0"
-binapy = "^0.6.0"
-mypy = "^1.1.1"
+binapy = ">=0.6.1"
 
 [tool.poetry.dev-dependencies]
-black  = ">=22"
-coverage = ">=6.0"
-freezegun = "^1.2.2"
-isort  = ">=5.11.5"
+black  = ">=23.3"
+coverage = ">=7.2.3"
+freezegun = ">=1.2.2"
+isort  = ">=5.12"
 jwcrypto = ">=1.0"
-livereload = ">=2.0"
-mypy = ">=0.990"
+livereload = ">=2.6"
+mypy = ">=1.2"
 mkdocs  = ">=1.4.2"
-mkdocstrings = { version = ">=0.18.0", extras = ["python"] }
+mkdocstrings = { version = ">=0.21.2", extras = ["python"] }
 mkdocs-autorefs = ">=0.4"
 mkdocs-include-markdown-plugin  = ">=4.0.4"
-mkdocs-material  = ">=8.5.8"
+mkdocs-material  = ">=9.1.6"
 mkdocs-material-extensions  = ">=1.1"
 pip  = ">=22.0"
-pre-commit = ">=2.21.0"
-pytest  = ">=7.2"
-pytest-cov  = ">=3.0"
-pytest-mypy = ">=0.9"
-requests-mock = ">=1.9"
+pre-commit = ">=3.2.2"
+pytest  = ">=7.3"
+pytest-cov  = ">=4.0"
+pytest-mypy = ">=0.10"
 toml = ">=0.10"
-tox  = ">=3.25,<4.0"
-types-requests = ">=2.27"
+tomli = ">=2.0.1"
+tox  = ">=4.5.1"
 types-cryptography = ">=3.3"
 virtualenv  = ">=20.14.1"
-tox-poetry = ">=0.4.1"
-types-backports = "^0.1.3"
-tomli = "^2.0.1"
-
 
 [tool.poetry.extras]
-test = ["pytest", "pytest-cov", "jwcrypto"]
+test = ["pytest", "pytest-cov", "jwcrypto", "freezegun"]
 doc = ["mkdocs"]
 
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
@@ -104,7 +98,10 @@
 ignore_decorators = 'override'
 
 [tool.docformatter]
 recursive = true
 wrap-summaries = 120
 wrap-descriptions = 120
 blank = true
+
+[tool.isort]
+profile = "black"
```

### Comparing `jwskate-0.7.0/tests/conftest.py` & `jwskate-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/tests/test_jwa/test_base.py` & `jwskate-0.8.0/tests/test_jwa/test_base.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/tests/test_jwa/test_encryption.py` & `jwskate-0.8.0/tests/test_jwa/test_encryption.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/tests/test_jwa/test_examples.py` & `jwskate-0.8.0/tests/test_jwa/test_examples.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/tests/test_jwa/test_key_mgmt.py` & `jwskate-0.8.0/tests/test_jwa/test_key_mgmt.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/tests/test_jwe.py` & `jwskate-0.8.0/tests/test_jwe.py`

 * *Files 1% similar despite different names*

```diff
@@ -500,15 +500,15 @@
     encryption_jwk: Union[Jwk, SupportsBytes],
     key_management_alg: str,
     encryption_alg: str,
 ) -> JweCompact:
     if isinstance(encryption_jwk, Jwk):
         jwe = JweCompact.encrypt(
             plaintext=encryption_plaintext,
-            jwk=encryption_jwk,
+            key=encryption_jwk,
             alg=key_management_alg,
             enc=encryption_alg,
         )
     else:
         password = bytes(encryption_jwk)
         jwe = JweCompact.encrypt_with_password(
             plaintext=encryption_plaintext,
@@ -538,15 +538,15 @@
     encryption_alg: str,
     encrypted_jwe: JweCompact,
     decryption_jwk: Jwk,
 ) -> None:
     if isinstance(encryption_jwk, Jwk):
         jwe = JweCompact.encrypt(
             plaintext=SupportsBytesTester(encryption_plaintext),
-            jwk=encryption_jwk,
+            key=encryption_jwk,
             alg=key_management_alg,
             enc=encryption_alg,
         )
     else:
         password = bytes(encryption_jwk)
         jwe = JweCompact.encrypt_with_password(
             plaintext=SupportsBytesTester(encryption_plaintext),
@@ -600,15 +600,14 @@
 
     Args:
         encryption_plaintext: the expected plaintext
         encrypted_jwe: the Jwe encrypted by jwskate to decrypt
         decryption_jwk: the Jwk containing the decryption key
         key_management_alg: the key management alg
         encryption_alg: the encryption alg
-
     """
     import jwcrypto.jwe  # type: ignore[import]
     import jwcrypto.jwk  # type: ignore[import]
     from jwcrypto.common import InvalidJWEOperation, json_encode  # type: ignore[import]
 
     if key_management_alg in JWCRYPTO_UNSUPPORTED_ALGS:
         pytest.skip(f"jwcrypto doesn't support key management alg {key_management_alg}")
@@ -640,15 +639,14 @@
         encryption_plaintext: the plaintext to encrypt
         encryption_jwk: the Jwk to use to for encryption
         key_management_alg: the key management alg
         encryption_alg: the encryption alg
 
     Returns:
         a JWE token
-
     """
     import jwcrypto.jwe
     import jwcrypto.jwk
     from jwcrypto.common import json_encode
 
     if key_management_alg in JWCRYPTO_UNSUPPORTED_ALGS:
         pytest.skip(f"jwcrypto doesn't support key management alg {key_management_alg}")
@@ -681,15 +679,14 @@
 
     Args:
         encryption_plaintext: the plaintext
         jwcrypto_encrypted_jwe: the JWE to validate
         decryption_jwk: the decryption key
         key_management_alg: the key management alg
         encryption_alg: the encryption alg
-
     """
     jwe = JweCompact(jwcrypto_encrypted_jwe)
     assert jwe.alg == key_management_alg
     assert jwe.enc == encryption_alg
     try:
         assert jwe.decrypt(decryption_jwk) == encryption_plaintext
     except Exception:
```

### Comparing `jwskate-0.7.0/tests/test_jwk/test_alg.py` & `jwskate-0.8.0/tests/test_jwk/test_alg.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/tests/test_jwk/test_ec.py` & `jwskate-0.8.0/tests/test_jwk/test_ec.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+from cryptography.hazmat.primitives.asymmetric import ec
 
 from jwskate import (
     A128CBC_HS256,
     EcdhEs,
     ECJwk,
     Jwk,
     UnsupportedAlg,
@@ -46,15 +47,15 @@
     ):
         ECJwk.generate()
 
 
 def test_ecdh_es() -> None:
     alg = "ECDH-ES+A128KW"
     enc = "A128CBC-HS256"
-    private_jwk = Jwk.generate_for_alg(alg)
+    private_jwk = Jwk.generate(alg=alg, crv="P-256")
     assert private_jwk.crv == "P-256"
     public_jwk = private_jwk.public_jwk()
     sender_cek, wrapped_cek, headers = public_jwk.sender_key(enc)
     assert sender_cek
     assert wrapped_cek
     assert "epk" in headers
     epk = Jwk(headers["epk"])
@@ -136,7 +137,16 @@
             crv="P-256",
             x=41091394722340406951651919287101979028566994134304719828008599584440827098914,
             y=5099336126642036233987555101153084413345413137896124327269101893088581300336,
             d=8342345011805978907621665437908035545366143771247820774310445528411160853919,
         )
         == jwk
     )
+
+
+def test_from_cryptography_key() -> None:
+    key = ec.generate_private_key(curve=ec.SECP256R1())
+
+    assert Jwk.from_cryptography_key(key) == Jwk(key)
+
+    with pytest.raises(TypeError):
+        ECJwk.from_cryptography_key(object())
```

### Comparing `jwskate-0.7.0/tests/test_jwk/test_generate.py` & `jwskate-0.8.0/tests/test_jwk/test_generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import secrets
+import warnings
 from typing import Dict
 
 import pytest
 
 from jwskate import (
     P_521,
     EncryptionAlgs,
@@ -16,15 +17,16 @@
 )
 
 
 @pytest.mark.parametrize(
     "alg", SignatureAlgs.ALL | EncryptionAlgs.ALL | KeyManagementAlgs.ALL_KEY_BASED
 )
 def test_generate_for_alg(alg: str) -> None:
-    jwk = Jwk.generate_for_alg(alg).with_usage_parameters()
+    with warnings.catch_warnings():
+        jwk = Jwk.generate(alg=alg).with_usage_parameters()
     assert jwk.is_private
     if alg in SignatureAlgs.ALL_SYMMETRIC:
         assert jwk.kty == "oct"
         assert jwk.use == "sig"
         assert jwk.key_ops == ("sign", "verify")
         assert jwk.is_symmetric
         keysize = {
```

### Comparing `jwskate-0.7.0/tests/test_jwk/test_jwk.py` & `jwskate-0.8.0/tests/test_jwk/test_jwk.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     UnsupportedKeyType,
     select_alg_class,
     to_jwk,
 )
 
 
 def test_public_jwk() -> None:
-    private_jwk = Jwk.generate_for_alg("RS256")
+    private_jwk = Jwk.generate(alg="ES256")
     assert private_jwk.is_private
     public_jwk = private_jwk.public_jwk()
     assert not public_jwk.is_private
     assert public_jwk is public_jwk.public_jwk()
 
 
 def test_jwk_copy() -> None:
@@ -199,15 +199,15 @@
         ("A128GCM", "enc", ("encrypt", "decrypt"), ("encrypt", "decrypt")),
     ],
 )
 def test_use_key_ops_with_alg(
     alg: str, use: str, private_key_ops: Tuple[str], public_key_ops: Tuple[str]
 ) -> None:
     # if key has an 'alg' parameter, we can deduce the use and key ops
-    private_jwk = Jwk.generate_for_alg(alg)
+    private_jwk = Jwk.generate(alg=alg)
     assert "use" not in private_jwk
     assert "key_ops" not in private_jwk
     assert private_jwk.use == use
     assert private_jwk.key_ops == private_key_ops
 
     public_jwk = (
         private_jwk.public_jwk() if not private_jwk.is_symmetric else private_jwk
@@ -268,29 +268,29 @@
 def test_generate_for_alg() -> None:
     rsa15_jwk = Jwk.generate_for_alg("RSA1_5")
     assert isinstance(rsa15_jwk, RSAJwk)
     assert rsa15_jwk.alg == "RSA1_5"
 
 
 def test_signature_wrapper() -> None:
-    signature_jwk = Jwk.generate_for_alg("ES256")
+    signature_jwk = Jwk.generate(alg="ES256")
     signature_wrapper = signature_jwk.signature_wrapper()
     assert isinstance(signature_wrapper, ES256)
     assert signature_wrapper.key == signature_jwk.cryptography_key
 
 
 def test_encryption_wrapper() -> None:
-    encryption_jwk = Jwk.generate_for_alg("A128GCM")
+    encryption_jwk = Jwk.generate(alg="A128GCM")
     encryption_wrapper = encryption_jwk.encryption_wrapper()
     assert isinstance(encryption_wrapper, A128GCM)
     assert encryption_wrapper.key == encryption_jwk.cryptography_key
 
 
 def test_key_management_wrapper() -> None:
-    key_mgmt_jwk = Jwk.generate_for_alg("ECDH-ES+A128KW")
+    key_mgmt_jwk = Jwk.generate(alg="ECDH-ES+A128KW")
     key_mgmt_wrapper = key_mgmt_jwk.key_management_wrapper()
     assert isinstance(key_mgmt_wrapper, EcdhEs_A128KW)
     assert key_mgmt_wrapper.key == key_mgmt_jwk.cryptography_key
 
 
 def test_to_jwk() -> None:
     # symmetric key
```

### Comparing `jwskate-0.7.0/tests/test_jwk/test_jwks.py` & `jwskate-0.8.0/tests/test_jwk/test_jwks.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,17 @@
     jwks.remove_jwk(jwk.kid)
 
     assert jwks.is_private
 
     assert not jwks.verify(data, signature, "ES256")
     assert not jwks.verify(data, signature, "ES256")
 
+    with pytest.raises(ValueError, match="provide either 'alg' or 'algs' parameter"):
+        jwks.verify(data, signature)
+
     assert jwks.public_jwks() == {
         "keys": [
             {
                 "kty": "RSA",
                 "n": "mUdmf5vJ3svsPSQ8BCOQVfwQdP8AmAEW21sYYUC5eSKR-pdwnRDBuFrIEjon2ry8cU-uaMjAoEZikPXcCTErye2Sj8fWQ8Wyo8DoGacJlFOJvs_18-CmNBc7oL8gBlYax3-feZZnaVIiJjvxQwUw5GQA6JTFnO8n2pnKMOOd8Gf6YrG-r0T6NXdviw0-2IW4f2UMJApqlu37yF8sgRNGZwDljNOkUtPK76Uz5T513Va4ckOqsVfnt4WoAkAkCl3eVBwGw3TJIbp_DaLUq53go0pXBCNxCHRD9mst69ZuknBLqn0SwKbQ9zJH9QvoqrEZ2q7GzkFzw70F6qH5MDEx2-dxQz_QccFV0XBpq4pkfuWzS8qKVO4QjyC7A0vIJUzrRHE2_moOtWvKTDsa7gfvK6kpnAW0iKnNchzBV0fzXWIIxRJ3_cc8Ue-KPRU9Wxm3heBOx_Qh-bKv9s9fVY9X6rimyX-pIwf-jkgWG8_FgTBuGkKTRcLi-XnwsCFIVNOtolmakbQHlin_lgDQm9s0nHoDJbZgAtzQfkIorclBJBzr2t__xgaZCfpSCLdwZFQvGEh1mK4WbSMMt5-L3zKsNLCBfdMbn2fS9n2hylfRwU_NZCY8f2RHAdP-z402Vq1c9-m2Ew3_695OmV5HoinJQPagY9hI-_EW8nhNWf8l4FE",
                 "e": "AQAB",
                 "kid": "uzPODAa44gSUXvSI6zilPwxMJCULUHm0FmXoqXRfYdI",
@@ -57,15 +60,20 @@
                 "n": "ycSaZ7HWpKCY4vfmoLWCxsg2KvpD-3dfFlz-2YsrfnMwpJF0nuRrceAxhFF34NlzwTn-JgVc8-lUrOJmcrBcxQNtr7eaJ0QhcRxu_Wre72QhqTddJgNt4V5Zn9P8l8CplSqiLruVI4nKGoiPFQ7mftGY39wxYiiFB6BMb04lAshvCuUOIP8WFFvCb5Afqpugl-NKpO2-C5vWeN_4xNkSO0fEq49Do01oUkMM5t1D4kvE6_BDVA2jxPHSSulXwcnwHmGuhXEfpVh-ME9MW0S0g7v-uNfpJmjVl7VDV87au6C9GKXHQ3NEXt8DWM8HXqRyRQ0XidJLymDOdUnF1_DMtS_wOCDrPFO-4rG_ZH3dwm-fBRSl_chu324OBi_ER6XIQpjkFiQo2pqbD8bI4X6kH8kUASq5gVsBU_hfQUZljSJoR2gQtorNw5EK4rlAQ5jS-ww16WiSna6jzgT_M4ZLr9IPCloe7isVxSk35-gD87xXtl8PzmE1vdpFC9aArkdFL_PK7MOqDvYIb6MRIOBvoxOV524tFKZhNrZUowTLH3a_-sWFLmdvd14iGxuv_DaC-hCmgI0eq7rzE2wUNP5IVmZASoI-3rKb22QdDlAPHNzdsyJCX4JVIPAJrpLOwptObN30404_C4UUD0IN9OXHD-16NaX5SY1thge94shJpTE",
                 "e": "AQAB",
                 "kid": "IYIB72QYGIUGP5lYlGmnrBeVOFOxTk9SO_5ajWBu1QE",
             },
         ]
     }
 
-    jwks.remove_jwk("foo")  # this is a no op since there is not key 'foo'
+    jwks.remove_jwk("foo")  # this is a no op since there is no key 'foo'
+
+    jwks.add_jwk(jwk.with_usage_parameters())
+
+    assert jwks.get_jwk_by_kid(jwk.kid) == jwk
+    assert jwks.get_jwk_by_kid(jwk.kid).use == "sig"
 
 
 def test_empty_jwkset() -> None:
     jwks = JwkSet()
     assert len(jwks) == 0
 
     generated_jwk = Jwk.generate_for_kty("RSA")
@@ -124,42 +132,38 @@
         }
     )
     assert not jwks.is_private
     sig_keys = jwks.verification_keys()
     enc_keys = jwks.encryption_keys()
 
     sig_kids = set(jwk.kid for jwk in sig_keys)
-    assert sig_kids == set(
-        (
-            "7KJgpwNvHJp_zb6SybahlC7506kvAm2cvMG_EY6jmx8",
-            "ojHE_6b7DXtOwLKYTmeao38CV_7P9F9rYTLGm8BuJnk",
-            "m7XoZRBgXXjEFxGhWvb_urskl4rCLmOhhPRdC6278-E",
-        )
-    )
+    assert sig_kids == {
+        "7KJgpwNvHJp_zb6SybahlC7506kvAm2cvMG_EY6jmx8",
+        "ojHE_6b7DXtOwLKYTmeao38CV_7P9F9rYTLGm8BuJnk",
+        "m7XoZRBgXXjEFxGhWvb_urskl4rCLmOhhPRdC6278-E",
+    }
 
     enc_kids = set(jwk.kid for jwk in enc_keys)
-    assert enc_kids == set(
-        (
-            "xAgzqjWdBD8cRifXbpmcv-9vIgjKHTdjelI-Vvu0K9Q",
-            "zjY2pjFnBc4rOHWEwfS5Cjyxsjo2aprsctM-4oS1r8I",
-        )
-    )
+    assert enc_kids == {
+        "xAgzqjWdBD8cRifXbpmcv-9vIgjKHTdjelI-Vvu0K9Q",
+        "zjY2pjFnBc4rOHWEwfS5Cjyxsjo2aprsctM-4oS1r8I",
+    }
 
 
 def test_contains() -> None:
-    key1 = Jwk.generate_for_alg("RS256")
-    key2 = Jwk.generate_for_alg("ES256")
+    key1 = Jwk.generate(alg="RS256")
+    key2 = Jwk.generate(alg="ES256")
 
     jwkset = JwkSet(keys=(key1, key2.public_jwk()))
     assert key1 in jwkset.jwks
     assert key2.public_jwk() in jwkset.jwks
 
     assert key1.with_kid_thumbprint().with_usage_parameters() in jwkset.jwks
     assert (
         key2.public_jwk().with_kid_thumbprint().with_usage_parameters() in jwkset.jwks
     )
 
-    key3 = Jwk.generate_for_alg("HS256")
+    key3 = Jwk.generate(alg="HS256")
     assert key3 not in jwkset.jwks
 
     assert key1.public_jwk() not in jwkset.jwks
     assert key2 not in jwkset.jwks
```

### Comparing `jwskate-0.7.0/tests/test_jwk/test_okp.py` & `jwskate-0.8.0/tests/test_jwk/test_okp.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,24 +75,24 @@
         "x": "11qYAYKxCrfVS_7TyWQHOg7hcvPapiMlrwIaaPcHURo",
     }
 
     assert jwk.thumbprint() == "kPrK_qmxVWaYVA9wwBF6Iuo3vVzz7TxHCTwXBygrS4k"
 
     payload = "Example of Ed25519 signing".encode()
 
-    jws = JwsCompact.sign(payload, jwk=jwk, alg="EdDSA")
+    jws = JwsCompact.sign(payload, key=jwk, alg="EdDSA")
     assert jws.alg == "EdDSA"
     assert jws.headers == {"alg": "EdDSA"}
     assert jws.payload == payload
     assert (
         jws
         == "eyJhbGciOiJFZERTQSJ9.RXhhbXBsZSBvZiBFZDI1NTE5IHNpZ25pbmc.hgyY0il_MGCjP0JzlnLWG1PPOt7-09PGcvMg3AIbQR6dWbhijcNR4ki4iylGjg5BhVsPt9g7sVvpAr_MuM0KAg"
     )
 
-    assert jws.verify_signature(jwk=jwk.public_jwk(), alg="EdDSA")
+    assert jws.verify_signature(key=jwk.public_jwk(), alg="EdDSA")
 
 
 def test_rfc8037_x25519() -> None:
     """Test from [RFC8037 $A.6][https://www.rfc-editor.org/rfc/rfc8037.html#appendix-A.6]."""
     public_jwk = Jwk(
         {
             "kty": "OKP",
```

### Comparing `jwskate-0.7.0/tests/test_jwk/test_rsa.py` & `jwskate-0.8.0/tests/test_jwk/test_rsa.py`

 * *Files identical despite different names*

### Comparing `jwskate-0.7.0/tests/test_jwk/test_symmetric.py` & `jwskate-0.8.0/tests/test_jwk/test_symmetric.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         ("HS512", 512),
     ),
     ids=("256bits", "384bits", "512bits"),
 )
 def symmetric_jwk(request: pytest.FixtureRequest) -> SymmetricJwk:
     alg, min_key_size = request.param
     kid = f"my_{alg}_jwk"
-    jwk = Jwk.generate_for_alg(alg, kid=kid)
+    jwk = Jwk.generate(alg=alg, kid=kid)
     assert isinstance(jwk, SymmetricJwk)
     assert jwk.kty == "oct"
     assert jwk.alg == alg
     assert jwk.kid == kid
     assert isinstance(jwk.k, str)
     assert jwk.key_size >= min_key_size
 
@@ -44,15 +44,15 @@
     with pytest.raises(TypeError):
         private_jwk.to_pem()
 
 
 def test_aesgcmkw() -> None:
     alg = "A128GCMKW"
     enc = "A128GCM"
-    jwk = Jwk.generate_for_alg(alg)
+    jwk = Jwk.generate(alg=alg)
     sender_cek, wrapped_cek, headers = jwk.sender_key(enc)
     assert sender_cek
     assert wrapped_cek
     assert "iv" in headers
     assert "tag" in headers
 
     recipient_cek = jwk.recipient_key(wrapped_cek, enc, **headers)
@@ -84,8 +84,8 @@
         ("A256KW", 256),
         ("A128GCMKW", 128),
         ("A192GCMKW", 192),
         ("A256GCMKW", 256),
     ],
 )
 def test_generate_for_alg(alg: str, key_size: int) -> None:
-    assert SymmetricJwk.generate_for_alg(alg).key_size == key_size
+    assert SymmetricJwk.generate(alg=alg).key_size == key_size
```

### Comparing `jwskate-0.7.0/tests/test_jws.py` & `jwskate-0.8.0/tests/test_jws.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     OKPJwk,
     RSAJwk,
     SymmetricJwk,
 )
 
 
 def test_jws_compact(private_jwk: Jwk) -> None:
-    jws = JwsCompact.sign(payload=b"Hello World!", jwk=private_jwk, alg="RS256")
+    jws = JwsCompact.sign(payload=b"Hello World!", key=private_jwk, alg="RS256")
     assert (
         str(jws)
         == "eyJhbGciOiJSUzI1NiIsImtpZCI6IkpXSy1BQkNEIn0.SGVsbG8gV29ybGQh.1eucS9ZaTnAJyfVNhxLJ_phFN1rexm0l"
         "-nIXWBjUImdS29z55BuxH6NjGpltSXKrgYxYQxqGCsGIxlSVoIEhKVdhE1Vd9NPJRyw7I4zBRdwVvcqMRODMqDxCiqbDQ"
         "_5bI5jAqFEJAFCXZo2T4ixlxs-2eXtmSEp6vX51Tg1pvicM5_YrKfS8Jn3lt9xW5RaNKUJ94KVLlov_IncFsh2bg5jdo1"
         "SEoUxlB2II0JdlfCsgHohJd58eWjFToeNtH1eiXGeZOHblMLz5a5AhY8jY3C424-tggj6BK6fwpedddFD3mtFFTNw6KT-"
         "2EgTeOlEA09pQqW5hosCj2duAlR-FQQ"
@@ -305,15 +305,15 @@
 
 
 @pytest.fixture()
 def signed_jws_compact(
     signature_payload: bytes, signature_jwk: Jwk, signature_alg: str
 ) -> JwsCompact:
     jws = JwsCompact.sign(
-        payload=signature_payload, jwk=signature_jwk, alg=signature_alg
+        payload=signature_payload, key=signature_jwk, alg=signature_alg
     )
     assert isinstance(jws, JwsCompact)
     return jws
 
 
 class SupportsBytesTester:
     """A test class with a __bytes__ method to match SupportBytes interface."""
@@ -330,19 +330,19 @@
     signature_jwk: Jwk,
     signature_alg: str,
     signed_jws_compact: JwsCompact,
     verification_jwk: Jwk,
 ) -> None:
     jws = JwsCompact.sign(
         payload=SupportsBytesTester(signature_payload),
-        jwk=signature_jwk,
+        key=signature_jwk,
         alg=signature_alg,
     )
     if signature_alg not in ("ES256", "ES384", "ES512", "PS256", "PS384", "PS512"):
-        # those algs have non deterministic signatures
+        # those algs have non-deterministic signatures
         assert jws == signed_jws_compact
 
     assert jws.payload == signed_jws_compact.payload
     assert verification_jwk.verify(
         SupportsBytesTester(jws.signed_part),
         SupportsBytesTester(jws.signature),
         alg=signature_alg,
@@ -350,15 +350,15 @@
 
 
 @pytest.fixture()
 def signed_jws_json_flat(
     signature_payload: bytes, signature_jwk: Jwk, signature_alg: str
 ) -> JwsJsonFlat:
     jws = JwsJsonFlat.sign(
-        payload=signature_payload, jwk=signature_jwk, alg=signature_alg
+        payload=signature_payload, key=signature_jwk, alg=signature_alg
     )
     assert isinstance(jws, JwsJsonFlat)
     return jws
 
 
 @pytest.fixture()
 def signed_jws_json_general(
@@ -478,15 +478,14 @@
 ) -> None:
     """This test verifies tokens generated by `jwskate` using another lib `jwcrypto`.
 
     Args:
         signed_jws_compact: the Jws signed by jwskate to verify
         verification_jwk: the Jwk containing the verification key
         signature_alg: the signature alg
-
     """
     import jwcrypto.jwk  # type: ignore[import]
     import jwcrypto.jws  # type: ignore[import]
 
     jwk = jwcrypto.jwk.JWK(**verification_jwk)
     jws = jwcrypto.jws.JWS()
     jws.deserialize(str(signed_jws_compact))
@@ -502,15 +501,14 @@
     Args:
         signature_payload: the payload to sign
         signature_jwk: the key to use
         signature_alg: the alg to use
 
     Returns:
         a JWS token
-
     """
     import jwcrypto.jwk
     import jwcrypto.jws
 
     jwk = jwcrypto.jwk.JWK(**signature_jwk)
     jws = jwcrypto.jws.JWS(signature_payload)
 
@@ -528,15 +526,14 @@
 ) -> None:
     """Check that `jwskate` verifies tokens signed by `jwcrypto`.
 
     Args:
         jwcrypto_signed_jws: the JWS to verify
         verification_jwk: the public key to verify the signature
         signature_alg: the alg to use
-
     """
     assert JwsCompact(jwcrypto_signed_jws).verify_signature(
         verification_jwk, alg=signature_alg
     )
 
 
 def test_invalid_jws_compact() -> None:
```

### Comparing `jwskate-0.7.0/tests/test_jwt.py` & `jwskate-0.8.0/tests/test_jwt.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from builtins import ValueError
 from datetime import datetime, timezone
 
 import pytest
+from binapy import BinaPy
 from freezegun import freeze_time
 
 from jwskate import (
     ExpectedAlgRequired,
     ExpiredJwt,
     InvalidClaim,
     InvalidJwt,
@@ -64,23 +65,23 @@
     assert jwt.issued_at == datetime.fromtimestamp(1629204560, tz=timezone.utc)
     assert jwt.not_before == datetime.fromtimestamp(1629204560, tz=timezone.utc)
     assert jwt.nonce == jwt["nonce"]
 
     # validating with the appropriate key must work
 
     jwt.validate(
-        jwk=jwk.public_jwk(),
+        key=jwk.public_jwk(),
         issuer="https://myas.local",
         audience="client_id",
         check_exp=False,
     )
 
     # validating with another key must fail
     with pytest.raises(InvalidSignature):
-        jwt.validate(Jwk.generate_for_alg("RS256").public_jwk())
+        jwt.validate(Jwk.generate(alg="ES256").public_jwk())
 
     # invalid audience
     with pytest.raises(InvalidClaim, match="audience"):
         jwt.validate(
             jwk.public_jwk(),
             audience="foo",
         )
@@ -102,22 +103,22 @@
     assert jwt.iat == pytest.approx(now.timestamp())
     assert jwt.expires_at is not None
     assert jwt.expires_at > now
 
     verifier = signer.verifier(audience=audience)
 
     @verifier.custom_verifier
-    def foobar_verifier(jwt: SignedJwt) -> None:
-        if jwt.foo != "bar":
+    def foobar_verifier(j: SignedJwt) -> None:
+        if j.foo != "bar":
             raise ValueError("This JWT is not FooBar compliant!")
 
     verifier.verify(jwt)
 
     @verifier.custom_verifier
-    def failing_verifier(jwt: SignedJwt) -> None:
+    def failing_verifier(j: SignedJwt) -> None:
         raise ValueError("This token will never be valid")
 
     with pytest.raises(ValueError):
         verifier.verify(jwt)
 
 
 def test_invalid_signed_jwt() -> None:
@@ -155,18 +156,18 @@
     assert (
         str(jwt)
         == "eyJhbGciOiJSUzI1NiIsImtpZCI6IkpXSy1BQkNEIn0.e30.iQ6eyP9QrNDQVfKYwHpIWvnTBb0SXNEItDxMQ0VmsB5CA5FaRYtGvj01VjoUAHEegGvwFI4YI35MDY_-DUR3UIXqxVMOe9Hk2hb9paTjJLpDIa7Ml6LKDh9-4xmAAPjZcra4IYrpDux8ohg0LUzgxHn0xnKDuxKmlh9shCyNWEOfN_i_JX4v8aSD-zDBteftrY9GzHU4Y0mlvlm4FaAwafPXovZilb_dTgTBkiFLmXY0y5ESurhQ4LrQqLzBz45lSONLElil5OQu0ySrrC72CBKp-HjdpCsLyG9F9p_X-1r9mmqlN38zIcgwkbhek04ieX-rumyzvHLO_UzttxDQOg"
     )
     assert bytes(jwt) == str(jwt).encode()
     assert jwt.signed_part == b"eyJhbGciOiJSUzI1NiIsImtpZCI6IkpXSy1BQkNEIn0.e30"
 
-    jwt.validate(jwk=private_jwk.public_jwk(), check_exp=False)
+    jwt.validate(key=private_jwk.public_jwk(), check_exp=False)
 
     with pytest.raises(InvalidClaim):
-        jwt.validate(jwk=private_jwk.public_jwk())
+        jwt.validate(key=private_jwk.public_jwk())
 
 
 def test_validate() -> None:
     jwt = SignedJwt(
         "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaXNzIjoiaHR0cHM6Ly9pc3N1ZXIubG9jYWwiLCJhdWQiOiJodHRwczovL2F1ZGllbmNlLmxvY2FsIiwiZXhwIjoyMDAwMDAwMDAwLCJpYXQiOjE1MTYyMzkwMjIsImNsYWltMSI6IkkgaGF2ZSBhIDEifQ.bl5iNgXfkbmgDXItaUx7_1lUMNtOffihsShVP8MeE1g"
     )
     jwk = SymmetricJwk.from_bytes("your-256-bit-secret")
@@ -358,20 +359,16 @@
 
 
 def test_sign_and_encrypt() -> None:
     sign_alg = "ES256"
     enc_alg = "RSA-OAEP-256"
     enc = "A128GCM"
 
-    sign_jwk = (
-        Jwk.generate_for_alg(sign_alg).with_kid_thumbprint().with_usage_parameters()
-    )
-    enc_jwk = (
-        Jwk.generate_for_alg(enc_alg).with_kid_thumbprint().with_usage_parameters()
-    )
+    sign_jwk = Jwk.generate(alg=sign_alg).with_kid_thumbprint().with_usage_parameters()
+    enc_jwk = Jwk.generate(alg=enc_alg).with_kid_thumbprint().with_usage_parameters()
 
     claims = {"iat": 1661759343, "exp": 1661759403, "nbf": 1661759323, "sub": "mysub"}
     enc_jwt = Jwt.sign_and_encrypt(claims, sign_jwk, enc_jwk.public_jwk(), enc)
     assert isinstance(enc_jwt, JweCompact)
     assert enc_jwt.cty == "JWT"
     assert enc_jwt.alg == enc_alg
     assert enc_jwt.enc == enc
@@ -381,55 +378,58 @@
     assert isinstance(inner_jwt, SignedJwt)
     assert inner_jwt.alg == sign_alg
     assert inner_jwt.claims == claims
     assert inner_jwt.verify_signature(sign_jwk.public_jwk())
     assert inner_jwt.kid == sign_jwk.kid
 
     verified_inner_jwt = Jwt.decrypt_and_verify(
-        enc_jwt, enc_jwk=enc_jwk, sig_jwk=sign_jwk.public_jwk()
+        enc_jwt, enc_key=enc_jwk, sig_key=sign_jwk.public_jwk()
     )
     assert isinstance(verified_inner_jwt, SignedJwt)
 
     # try to encrypt a JWT with an altered signature
     altered_inner_jwt = bytes(verified_inner_jwt)[:-4] + (
         b"aaaa" if not verified_inner_jwt.value.endswith(b"aaaa") else b"bbbb"
     )
     enc_altered_jwe = JweCompact.encrypt(
-        altered_inner_jwt, jwk=enc_jwk.public_jwk(), enc=enc
+        altered_inner_jwt, key=enc_jwk.public_jwk(), enc=enc
     )
     with pytest.raises(InvalidSignature):
         Jwt.decrypt_and_verify(
-            enc_altered_jwe, enc_jwk=enc_jwk, sig_jwk=sign_jwk.public_jwk()
+            enc_altered_jwe, enc_key=enc_jwk, sig_key=sign_jwk.public_jwk()
         )
 
     # trying to decrypt and verify a JWE nested in a JWE will raise a ValueError
     inner_jwe = JweCompact.encrypt(
         b"this_is_a_test",
-        jwk=Jwk.generate_for_alg("ECDH-ES+A128KW").public_jwk(),
+        key=Jwk.generate(alg="ECDH-ES+A128KW", crv="P-256").public_jwk(),
         enc="A128GCM",
     )
-    nested_inner_jwe = JweCompact.encrypt(inner_jwe, jwk=enc_jwk.public_jwk(), enc=enc)
+    nested_inner_jwe = JweCompact.encrypt(inner_jwe, key=enc_jwk.public_jwk(), enc=enc)
     with pytest.raises(ValueError):
         Jwt.decrypt_and_verify(
-            nested_inner_jwe, enc_jwk=enc_jwk, sig_jwk=sign_jwk.public_jwk()
+            nested_inner_jwe, enc_key=enc_jwk, sig_key=sign_jwk.public_jwk()
         )
 
 
 def test_sign_without_alg() -> None:
-    jwk = Jwk.generate_for_kty("RSA")
-    with pytest.raises(ValueError):
+    jwk = Jwk.generate_for_kty("EC", crv="P-256")
+    with pytest.raises(ValueError, match="signing alg is required"):
         Jwt.sign({"foo": "bar"}, jwk)
 
+    with pytest.raises(ValueError, match="signing alg is required"):
+        Jwt.sign_arbitrary(claims={"foo": "bar"}, headers={}, key=jwk)
+
 
 def test_large_jwt() -> None:
-    with pytest.raises(ValueError):
+    with pytest.raises(ValueError, match="is abnormally big"):
         Jwt(
             "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9."
-            f"{'alargevalue' * 16 * 1024}"
-            "bl5iNgXfkbmgDXItaUx7_1lUMNtOffihsShVP8MeE1g"
+            f'{BinaPy.serialize_to("json", {f"claim{i}": f"value{i}" for i in range(16_000)}).ascii()}'
+            ".bl5iNgXfkbmgDXItaUx7_1lUMNtOffihsShVP8MeE1g"
         )
 
 
 def test_eq() -> None:
     jwt = "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiIxMjM0NTY3ODkwIiwibmFtZSI6IkpvaG4gRG9lIiwiaWF0IjoxNTE2MjM5MDIyfQ.SflKxwRJSMeKKF2QT4fwpMeJf36POk6yJV_adQssw5c"
     assert Jwt(jwt) == Jwt(jwt)
     assert Jwt(jwt) == jwt
@@ -509,20 +509,20 @@
             "x": "ftZqn6yrLR_4AytQz8Q_badHRTQ2Vc6Eg46ICsMuuMM",
             "y": "C4wIeHH0aIW5Tf1_EPnJkse-vcoDNd-kh8P6-Ci2MI8",
             "d": "3vyhseJLd51ZXdlrCHAPH1uv5Bp9IvnA8UB92ksu4MU",
         }
     )
     jwks = private_jwk.public_jwk().as_jwks()
 
-    def suject_verifier(jwt: SignedJwt) -> None:
-        if jwt.subject != subject:
+    def suject_verifier(j: SignedJwt) -> None:
+        if j.subject != subject:
             raise ValueError("Invalid Subject", jwt)
 
-    def not_foo(jwt: SignedJwt) -> None:
-        if "foo" in jwt.claims:
+    def not_foo(j: SignedJwt) -> None:
+        if "foo" in j.claims:
             raise ValueError("Token is foo!", jwt)
 
     verifier = JwtVerifier(
         jwks,
         issuer=issuer,
         audience=audience,
         alg="ES256",
```

### Comparing `jwskate-0.7.0/PKG-INFO` & `jwskate-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jwskate
-Version: 0.7.0
+Version: 0.8.0
 Summary: A Pythonic implementation of Json Web Signature, Keys, Algorithms, Tokens and Encryption (RFC7514 to 7519), on top of the `cryptography` module.
 Home-page: https://github.com/guillp/jwskate
 License: MIT
 Author: Guillaume Pujol
 Author-email: guill.p.linux@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 3 - Alpha
@@ -12,24 +12,18 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: doc
 Provides-Extra: test
-Requires-Dist: binapy (>=0.6.0,<0.7.0)
+Requires-Dist: binapy (>=0.6.1)
 Requires-Dist: cryptography (>=3.4)
-Requires-Dist: mypy (>=1.1.1,<2.0.0)
 Requires-Dist: typing-extensions (>=4.3.0)
 Description-Content-Type: text/markdown
 
 # JwSkate
 
 [![PyPi](https://img.shields.io/pypi/v/jwskate.svg)](https://pypi.python.org/pypi/jwskate)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

