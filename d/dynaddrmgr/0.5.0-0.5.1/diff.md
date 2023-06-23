# Comparing `tmp/dynaddrmgr-0.5.0.tar.gz` & `tmp/dynaddrmgr-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynaddrmgr-0.5.0.tar", max compression
+gzip compressed data, was "dynaddrmgr-0.5.1.tar", max compression
```

## Comparing `dynaddrmgr-0.5.0.tar` & `dynaddrmgr-0.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1097 2023-01-18 20:13:38.224772 dynaddrmgr-0.5.0/LICENSE
--rw-r--r--   0        0        0     1606 2023-03-02 18:15:54.777115 dynaddrmgr-0.5.0/README.md
--rw-r--r--   0        0        0       59 2023-06-01 14:58:46.288353 dynaddrmgr-0.5.0/dynaddrmgr/__init__.py
--rw-r--r--   0        0        0     4856 2023-03-04 19:26:55.486165 dynaddrmgr-0.5.0/dynaddrmgr/app.py
--rw-r--r--   0        0        0     3885 2023-03-02 18:15:54.777115 dynaddrmgr-0.5.0/dynaddrmgr/dynhost.py
--rw-r--r--   0        0        0     2401 2023-05-25 14:23:01.570505 dynaddrmgr-0.5.0/dynaddrmgr/dynrules.py
--rw-r--r--   0        0        0     2189 2023-06-01 14:58:46.292353 dynaddrmgr-0.5.0/dynaddrmgr/dyntmpls.py
--rw-r--r--   0        0        0      655 2023-03-22 15:47:54.561241 dynaddrmgr-0.5.0/dynaddrmgr/foos.py
--rw-r--r--   0        0        0     5070 2023-03-02 18:15:54.777115 dynaddrmgr-0.5.0/dynaddrmgr/fwhdlr.py
--rw-r--r--   0        0        0      294 2023-03-02 18:15:54.777115 dynaddrmgr-0.5.0/dynaddrmgr/kinds.py
--rw-r--r--   0        0        0        0 2023-03-02 18:15:54.777115 dynaddrmgr-0.5.0/dynaddrmgr/py.typed
--rw-r--r--   0        0        0     3850 2023-03-02 18:15:54.777115 dynaddrmgr-0.5.0/dynaddrmgr/rule.py
--rw-r--r--   0        0        0     4256 2023-04-06 18:44:52.329724 dynaddrmgr-0.5.0/dynaddrmgr/tmplmgr.py
--rw-r--r--   0        0        0     8661 2023-03-02 18:15:54.777115 dynaddrmgr-0.5.0/dynaddrmgr/ufw.py
--rw-r--r--   0        0        0     1466 2023-06-01 14:58:46.296353 dynaddrmgr-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2692 1970-01-01 00:00:00.000000 dynaddrmgr-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-01-15 15:37:55.155474 dynaddrmgr-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1606 2023-02-09 13:27:57.592714 dynaddrmgr-0.5.1/README.md
+-rw-r--r--   0        0        0       59 2023-06-23 19:50:27.588565 dynaddrmgr-0.5.1/dynaddrmgr/__init__.py
+-rw-r--r--   0        0        0     5156 2023-06-23 19:50:27.588565 dynaddrmgr-0.5.1/dynaddrmgr/app.py
+-rw-r--r--   0        0        0     3885 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.1/dynaddrmgr/dynhost.py
+-rw-r--r--   0        0        0     2401 2023-06-19 17:51:53.034497 dynaddrmgr-0.5.1/dynaddrmgr/dynrules.py
+-rw-r--r--   0        0        0     2189 2023-06-19 17:51:53.034497 dynaddrmgr-0.5.1/dynaddrmgr/dyntmpls.py
+-rw-r--r--   0        0        0      655 2023-06-19 17:51:53.034497 dynaddrmgr-0.5.1/dynaddrmgr/foos.py
+-rw-r--r--   0        0        0     5070 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.1/dynaddrmgr/fwhdlr.py
+-rw-r--r--   0        0        0      294 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.1/dynaddrmgr/kinds.py
+-rw-r--r--   0        0        0        0 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.1/dynaddrmgr/py.typed
+-rw-r--r--   0        0        0     3850 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.1/dynaddrmgr/rule.py
+-rw-r--r--   0        0        0     4256 2023-06-19 17:51:53.038497 dynaddrmgr-0.5.1/dynaddrmgr/tmplmgr.py
+-rw-r--r--   0        0        0     8661 2023-01-23 13:03:17.636247 dynaddrmgr-0.5.1/dynaddrmgr/ufw.py
+-rw-r--r--   0        0        0     1480 2023-06-23 19:50:27.588565 dynaddrmgr-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2594 1970-01-01 00:00:00.000000 dynaddrmgr-0.5.1/PKG-INFO
```

### Comparing `dynaddrmgr-0.5.0/LICENSE` & `dynaddrmgr-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.0/README.md` & `dynaddrmgr-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.0/dynaddrmgr/app.py` & `dynaddrmgr-0.5.1/dynaddrmgr/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Misc variables:
     APPNM
 """
 import subprocess  # noqa: S404
 import sys
 from typing import List, Tuple, Union
 
+from dns.exception import DNSException
 from nslookup import DNSresponse, Nslookup
 from wtforglib.ipaddress_foos import ipv6_to_netprefix, is_ipv6_address
 from wtforglib.kinds import StrAnyDict
 from wtforglib.scribe import Scribe
 
 APPNM = "dynaddrmgr"
 
@@ -117,15 +118,15 @@
         for ip in ips:
             if is_ipv6_address(ip):
                 converted.append(ipv6_to_netprefix(ip, prefix_len))
             else:
                 converted.append(ip)
         return tuple(converted)
 
-    def _lookup_host(
+    def _lookup_host(  # noqa: WPS231
         self,
         name: str,
         ipv4: bool,
         ipv6: bool,
         ipv6net: int = 0,
     ) -> Tuple[str, ...]:
         """Retrun a unique list of IP source strings.
@@ -141,26 +142,35 @@
         ipv6net : int
             Prefix length if ipv6 addreses represent networks
 
         Returns
         -------
         Tuple[str, ...]
             Unique list of IP source strings
+
+        Raises
+        ------
+        DNSException
+            If lookup failed
         """
         ips: DNSresponse
         if ipv4 and ipv6:
             ips = self.dns.dns_lookup_all(name)
         elif ipv4:
             ips = self.dns.dns_lookup(name)
         elif ipv6:
             ips = self.dns.dns_lookup6(name)
-        first_set = set(ips.answer)
-        if ipv6net and ipv6:
-            return self._six_to_net(ipv6net, list(first_set))
-        return tuple(first_set)
+        if ips.answer:
+            first_set = set(ips.answer)
+            if ipv6net and ipv6:
+                return self._six_to_net(ipv6net, list(first_set))
+            return tuple(first_set)
+        raise DNSException(  # type: ignore [no-untyped-call]
+            "'{0}' name not found.!!!".format(name),
+        )
 
     def _run_command(
         self,
         args: Tuple[str, ...],
         **kwargs,
     ) -> WtfProcessResult:
         """Runs commands specified by args."""
```

### Comparing `dynaddrmgr-0.5.0/dynaddrmgr/dynhost.py` & `dynaddrmgr-0.5.1/dynaddrmgr/dynhost.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.0/dynaddrmgr/dynrules.py` & `dynaddrmgr-0.5.1/dynaddrmgr/dynrules.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.0/dynaddrmgr/dyntmpls.py` & `dynaddrmgr-0.5.1/dynaddrmgr/dyntmpls.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.0/dynaddrmgr/foos.py` & `dynaddrmgr-0.5.1/dynaddrmgr/foos.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.0/dynaddrmgr/fwhdlr.py` & `dynaddrmgr-0.5.1/dynaddrmgr/fwhdlr.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.0/dynaddrmgr/rule.py` & `dynaddrmgr-0.5.1/dynaddrmgr/rule.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.0/dynaddrmgr/tmplmgr.py` & `dynaddrmgr-0.5.1/dynaddrmgr/tmplmgr.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.0/dynaddrmgr/ufw.py` & `dynaddrmgr-0.5.1/dynaddrmgr/ufw.py`

 * *Files identical despite different names*

### Comparing `dynaddrmgr-0.5.0/pyproject.toml` & `dynaddrmgr-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "dynaddrmgr"
 description = "Tools to manage actions based on dynamic host address changes."
-version = "0.5.0"
+version = "0.5.1"
 license = "MIT"
 
 authors = [
   "Quien Sabe <qs5779@mail.com>",
 ]
 
 readme = "README.md"
@@ -22,23 +22,23 @@
 ]
 
 [tool.poetry.scripts]
 dyntmplmgr = "dynaddrmgr.dyntmpls:main"
 dynfwrules = "dynaddrmgr.dynrules:main"
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = ">=3.8.1,<4.0"
 click = "^8.1.0"
 nslookup = "^1.7.0"
 wtforglib = ">= 0.8.2"
 jinja2 = "^3.1.2"
 
 [tool.poetry.group.test.dependencies]
 mypy = "^1.3.0"
-wemake-python-styleguide = "^0.17"
+wemake-python-styleguide = "^0.18"
 flake8-pytest-style = "^1.6"
 doc8 = "^1.0"
 nitpick = ">=0.32,<0.34"
 safety = "^2.3"
 pytest = "^7.3"
 pytest-cov = "^4.0"
 pytest-randomly = "^3.12"
@@ -47,15 +47,15 @@
 isort = { version = "<5.12.0", python = "<3.8" }
 requests-cache = ">=0.9,<1.1"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "^5.2"
+sphinx = ">=5.2,<8.0"
 sphinx-autodoc-typehints = "^1.23"
 m2r2 = "^0.3"
 tomli = "^2.0"
 
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
```

### Comparing `dynaddrmgr-0.5.0/PKG-INFO` & `dynaddrmgr-0.5.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 Metadata-Version: 2.1
 Name: dynaddrmgr
-Version: 0.5.0
+Version: 0.5.1
 Summary: Tools to manage actions based on dynamic host address changes.
 Home-page: https://github.com/wtfo-guru/dynaddrmgr
 License: MIT
 Author: Quien Sabe
 Author-email: qs5779@mail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: click (>=8.1.0,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: nslookup (>=1.7.0,<2.0.0)
```

