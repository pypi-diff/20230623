# Comparing `tmp/b4-0.9.0.tar.gz` & `tmp/b4-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b4-0.9.0.tar", last modified: Fri Jun 17 18:28:19 2022, max compression
+gzip compressed data, was "b4-0.9.1.tar", last modified: Tue Sep 13 14:19:39 2022, max compression
```

## Comparing `b4-0.9.0.tar` & `b4-0.9.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-17 18:28:19.259137 b4-0.9.0/
--rw-rw-r--   0 user      (1000) user      (1000)    18092 2010-03-23 23:34:05.000000 b4-0.9.0/COPYING
--rw-rw-r--   0 user      (1000) user      (1000)       52 2020-04-24 16:28:54.000000 b4-0.9.0/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)    19343 2022-06-17 18:28:19.258137 b4-0.9.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     2554 2022-06-17 18:00:01.000000 b4-0.9.0/README.rst
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-17 18:28:19.256137 b4-0.9.0/b4/
--rw-rw-r--   0 user      (1000) user      (1000)   100018 2022-06-17 18:13:00.000000 b4-0.9.0/b4/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      899 2021-05-11 17:54:21.000000 b4-0.9.0/b4/attest.py
--rw-rw-r--   0 user      (1000) user      (1000)    15423 2022-06-17 12:54:33.000000 b4-0.9.0/b4/command.py
--rw-rw-r--   0 user      (1000) user      (1000)     5518 2021-09-01 13:14:26.000000 b4-0.9.0/b4/diff.py
--rw-rw-r--   0 user      (1000) user      (1000)     3151 2021-08-31 16:48:41.000000 b4-0.9.0/b4/kr.py
--rw-rw-r--   0 user      (1000) user      (1000)    31747 2022-06-17 12:55:15.000000 b4-0.9.0/b4/mbox.py
--rw-rw-r--   0 user      (1000) user      (1000)    23386 2022-06-15 17:26:08.000000 b4-0.9.0/b4/pr.py
--rw-rw-r--   0 user      (1000) user      (1000)    25715 2022-03-30 19:22:47.000000 b4-0.9.0/b4/ty.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-17 18:28:19.257137 b4-0.9.0/b4.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    19343 2022-06-17 18:28:19.000000 b4-0.9.0/b4.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      394 2022-06-17 18:28:19.000000 b4-0.9.0/b4.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-06-17 18:28:19.000000 b4-0.9.0/b4.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       39 2022-06-17 18:28:19.000000 b4-0.9.0/b4.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)       74 2022-06-17 18:28:19.000000 b4-0.9.0/b4.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        3 2022-06-17 18:28:19.000000 b4-0.9.0/b4.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-17 18:28:19.258137 b4-0.9.0/man/
--rw-rw-r--   0 user      (1000) user      (1000)    20434 2022-06-17 13:52:22.000000 b4-0.9.0/man/b4.5
--rw-rw-r--   0 user      (1000) user      (1000)    18890 2022-06-17 13:52:14.000000 b4-0.9.0/man/b4.5.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2022-06-17 18:28:19.259137 b4-0.9.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1548 2022-06-17 18:22:52.000000 b4-0.9.0/setup.py
--rw-rw-r--   0 user      (1000) user      (1000)      836 2022-06-16 20:18:30.000000 b4-0.9.0/shazam-merge-template.example
--rw-rw-r--   0 user      (1000) user      (1000)     1429 2020-07-07 19:38:34.000000 b4-0.9.0/thanks-am-template.example
--rw-rw-r--   0 user      (1000) user      (1000)     1403 2020-07-07 19:38:34.000000 b4-0.9.0/thanks-pr-template.example
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-13 14:19:39.424676 b4-0.9.1/
+-rw-rw-r--   0 user      (1000) user      (1000)    18092 2010-03-23 23:34:05.000000 b4-0.9.1/COPYING
+-rw-rw-r--   0 user      (1000) user      (1000)       52 2020-04-24 16:28:54.000000 b4-0.9.1/MANIFEST.in
+-rw-r--r--   0 user      (1000) user      (1000)    19343 2022-09-13 14:19:39.424676 b4-0.9.1/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     2554 2022-06-17 18:00:01.000000 b4-0.9.1/README.rst
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-13 14:19:39.423675 b4-0.9.1/b4/
+-rw-r--r--   0 user      (1000) user      (1000)   100745 2022-09-13 14:10:01.000000 b4-0.9.1/b4/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)      899 2022-09-13 14:08:59.000000 b4-0.9.1/b4/attest.py
+-rw-r--r--   0 user      (1000) user      (1000)    15423 2022-09-13 14:08:59.000000 b4-0.9.1/b4/command.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5518 2021-09-01 13:14:26.000000 b4-0.9.1/b4/diff.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3151 2021-08-31 16:48:41.000000 b4-0.9.1/b4/kr.py
+-rw-r--r--   0 user      (1000) user      (1000)    31747 2022-09-13 14:08:59.000000 b4-0.9.1/b4/mbox.py
+-rw-r--r--   0 user      (1000) user      (1000)    23386 2022-09-13 14:08:59.000000 b4-0.9.1/b4/pr.py
+-rw-r--r--   0 user      (1000) user      (1000)    25715 2022-09-13 14:08:59.000000 b4-0.9.1/b4/ty.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-13 14:19:39.424676 b4-0.9.1/b4.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    19343 2022-09-13 14:19:39.000000 b4-0.9.1/b4.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      394 2022-09-13 14:19:39.000000 b4-0.9.1/b4.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2022-09-13 14:19:39.000000 b4-0.9.1/b4.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       39 2022-09-13 14:19:39.000000 b4-0.9.1/b4.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       74 2022-09-13 14:19:39.000000 b4-0.9.1/b4.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        3 2022-09-13 14:19:39.000000 b4-0.9.1/b4.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-09-13 14:19:39.424676 b4-0.9.1/man/
+-rw-r--r--   0 user      (1000) user      (1000)    20434 2022-09-13 14:08:59.000000 b4-0.9.1/man/b4.5
+-rw-r--r--   0 user      (1000) user      (1000)    18890 2022-09-13 14:08:59.000000 b4-0.9.1/man/b4.5.rst
+-rw-r--r--   0 user      (1000) user      (1000)       38 2022-09-13 14:19:39.425675 b4-0.9.1/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)     1548 2022-08-24 14:21:48.000000 b4-0.9.1/setup.py
+-rw-rw-r--   0 user      (1000) user      (1000)      836 2022-06-16 20:18:30.000000 b4-0.9.1/shazam-merge-template.example
+-rw-rw-r--   0 user      (1000) user      (1000)     1429 2020-07-07 19:38:34.000000 b4-0.9.1/thanks-am-template.example
+-rw-rw-r--   0 user      (1000) user      (1000)     1403 2020-07-07 19:38:34.000000 b4-0.9.1/thanks-pr-template.example
```

### Comparing `b4-0.9.0/COPYING` & `b4-0.9.1/COPYING`

 * *Files identical despite different names*

### Comparing `b4-0.9.0/PKG-INFO` & `b4-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: b4
-Version: 0.9.0
+Version: 0.9.1
 Summary: A tool to work with public-inbox and patch archives
 Home-page: https://git.kernel.org/pub/scm/utils/b4/b4.git/tree/README.rst
 Author: Konstantin Ryabitsev
 Author-email: mricon@kernel.org
 License: GPLv2+
 Project-URL: Community, https://lore.kernel.org/tools
 Keywords: git,lore.kernel.org,patches
 Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: COPYING
 
 B4
 ==
 ----------------------------------------------------
 Work with code submissions in a public-inbox archive
```

### Comparing `b4-0.9.0/README.rst` & `b4-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `b4-0.9.0/b4/__init__.py` & `b4-0.9.1/b4/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 try:
     import patatt
     can_patatt = True
 except ModuleNotFoundError:
     can_patatt = False
 
-__VERSION__ = '0.9.0'
+__VERSION__ = '0.9.1'
 
 
 def _dkim_log_filter(record):
     # Hide all dkim logging output in normal operation by setting the level to
     # DEBUG. If debugging output has been enabled then prefix dkim logging
     # output to make its origin clear.
     record.levelno = logging.DEBUG
@@ -1069,18 +1069,25 @@
             else:
                 # See if date is included in the h: field
                 sh = hdata.get('h')
                 if 'date' in sh.lower().split(':'):
                     signtime = self.date
 
             self.msg._headers.append((hn, hval))  # noqa
-            res = dkim.verify(self.msg.as_bytes(), logger=dkimlogger)
+            try:
+                res = dkim.verify(self.msg.as_bytes(), logger=dkimlogger)
+                logger.debug('DKIM verify results: %s=%s', identity, res)
+            except Exception as ex:  # noqa
+                # Usually, this is due to some DNS resolver failure, which we can't
+                # possibly cleanly try/catch. Just mark it as failed and move on.
+                logger.debug('DKIM attestation failed: %s', ex)
+                errors.append(str(ex))
+                res = False
 
             attestor = LoreAttestorDKIM(res, identity, signtime, errors)
-            logger.debug('DKIM verify results: %s=%s', identity, res)
             if attestor.check_identity(self.fromemail):
                 # use this one, regardless of any other DKIM signatures
                 self._attestors.append(attestor)
                 return
 
             self.msg._headers.pop(-1)  # noqa
             seenatts.append(attestor)
@@ -2133,14 +2140,20 @@
         return None
 
     msgid = msgid.strip('<>')
     # Handle the case when someone pastes a full URL to the message
     matches = re.search(r'^https?://[^/]+/([^/]+)/([^/]+@[^/]+)', msgid, re.IGNORECASE)
     if matches:
         chunks = matches.groups()
+        config = get_main_config()
+        myloc = urllib.parse.urlparse(config['midmask'])
+        wantloc = urllib.parse.urlparse(msgid)
+        if myloc.netloc != wantloc.netloc:
+            logger.debug('Overriding midmask with passed url parameters')
+            config['midmask'] = f'{wantloc.scheme}://{wantloc.netloc}/{chunks[0]}/%s'
         msgid = urllib.parse.unquote(chunks[1])
         # Infer the project name from the URL, if possible
         if chunks[0] != 'r':
             cmdargs.useproject = chunks[0]
     # Handle special case when msgid is prepended by id: or rfc822msgid:
     if msgid.find('id:') >= 0:
         msgid = re.sub(r'^\w*id:', '', msgid)
@@ -2283,15 +2296,15 @@
     qmsgid = urllib.parse.quote_plus(msgid)
     config = get_main_config()
     loc = urllib.parse.urlparse(config['midmask'])
     # The public-inbox instance may provide a unified index at /all/.
     # In fact, /all/ naming is arbitrary, but for now we are going to
     # hardcode it to lore.kernel.org settings and maybe make it configurable
     # in the future, if necessary.
-    if loc.path.startswith('/all/'):
+    if loc.path.startswith('/all/') and not useproject:
         useproject = 'all'
     if useproject:
         projurl = '%s://%s/%s' % (loc.scheme, loc.netloc, useproject)
     else:
         # Grab the head from lore, to see where we are redirected
         midmask = config['midmask'] % qmsgid
         logger.info('Looking up %s', midmask)
```

### Comparing `b4-0.9.0/b4/attest.py` & `b4-0.9.1/b4/attest.py`

 * *Files identical despite different names*

### Comparing `b4-0.9.0/b4/command.py` & `b4-0.9.1/b4/command.py`

 * *Files identical despite different names*

### Comparing `b4-0.9.0/b4/diff.py` & `b4-0.9.1/b4/diff.py`

 * *Files identical despite different names*

### Comparing `b4-0.9.0/b4/kr.py` & `b4-0.9.1/b4/kr.py`

 * *Files identical despite different names*

### Comparing `b4-0.9.0/b4/mbox.py` & `b4-0.9.1/b4/mbox.py`

 * *Files identical despite different names*

### Comparing `b4-0.9.0/b4/pr.py` & `b4-0.9.1/b4/pr.py`

 * *Files identical despite different names*

### Comparing `b4-0.9.0/b4/ty.py` & `b4-0.9.1/b4/ty.py`

 * *Files identical despite different names*

### Comparing `b4-0.9.0/b4.egg-info/PKG-INFO` & `b4-0.9.1/b4.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: b4
-Version: 0.9.0
+Version: 0.9.1
 Summary: A tool to work with public-inbox and patch archives
 Home-page: https://git.kernel.org/pub/scm/utils/b4/b4.git/tree/README.rst
 Author: Konstantin Ryabitsev
 Author-email: mricon@kernel.org
 License: GPLv2+
 Project-URL: Community, https://lore.kernel.org/tools
 Keywords: git,lore.kernel.org,patches
 Platform: UNKNOWN
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: COPYING
 
 B4
 ==
 ----------------------------------------------------
 Work with code submissions in a public-inbox archive
```

### Comparing `b4-0.9.0/man/b4.5` & `b4-0.9.1/man/b4.5`

 * *Files identical despite different names*

### Comparing `b4-0.9.0/man/b4.5.rst` & `b4-0.9.1/man/b4.5.rst`

 * *Files identical despite different names*

### Comparing `b4-0.9.0/setup.py` & `b4-0.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,14 +42,14 @@
     keywords=['git', 'lore.kernel.org', 'patches'],
     install_requires=[
         'requests>=2.24,<3.0',
         'dnspython>=2.0,<3.0',
         'dkimpy>=1.0,<2.0',
         'patatt>=0.5,<2.0',
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     entry_points={
         'console_scripts': [
             'b4=b4.command:cmd'
         ],
     },
 )
```

### Comparing `b4-0.9.0/shazam-merge-template.example` & `b4-0.9.1/shazam-merge-template.example`

 * *Files identical despite different names*

### Comparing `b4-0.9.0/thanks-am-template.example` & `b4-0.9.1/thanks-am-template.example`

 * *Files identical despite different names*

### Comparing `b4-0.9.0/thanks-pr-template.example` & `b4-0.9.1/thanks-pr-template.example`

 * *Files identical despite different names*

