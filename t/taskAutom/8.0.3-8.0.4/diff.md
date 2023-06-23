# Comparing `tmp/taskAutom-8.0.3.tar.gz` & `tmp/taskAutom-8.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskAutom-8.0.3.tar", last modified: Fri Jun  2 19:43:09 2023, max compression
+gzip compressed data, was "taskAutom-8.0.4.tar", last modified: Thu Jun 22 20:07:24 2023, max compression
```

## Comparing `taskAutom-8.0.3.tar` & `taskAutom-8.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 19:43:09.755346 taskAutom-8.0.3/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-8.0.3/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-06-02 19:43:09.755346 taskAutom-8.0.3/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-8.0.3/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-06-02 19:43:09.755346 taskAutom-8.0.3/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      999 2023-06-02 19:33:06.000000 taskAutom-8.0.3/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 19:43:09.751346 taskAutom-8.0.3/src/
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 19:43:09.751346 taskAutom-8.0.3/src/taskAutom/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       52 2023-06-02 19:32:38.000000 taskAutom-8.0.3/src/taskAutom/__init__.py
--rwxrwxr-x   0 lucas     (1000) lucas     (1000)    67035 2023-06-02 19:36:03.000000 taskAutom-8.0.3/src/taskAutom/taskAutom.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-02 19:43:09.755346 taskAutom-8.0.3/taskAutom.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-06-02 19:43:09.000000 taskAutom-8.0.3/taskAutom.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-06-02 19:43:09.000000 taskAutom-8.0.3/taskAutom.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-06-02 19:43:09.000000 taskAutom-8.0.3/taskAutom.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-06-02 19:43:09.000000 taskAutom-8.0.3/taskAutom.egg-info/entry_points.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-06-02 19:43:09.000000 taskAutom-8.0.3/taskAutom.egg-info/requires.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-06-02 19:43:09.000000 taskAutom-8.0.3/taskAutom.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-22 20:07:24.613219 taskAutom-8.0.4/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1527 2023-01-27 17:25:37.000000 taskAutom-8.0.4/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-06-22 20:07:24.613219 taskAutom-8.0.4/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     6721 2023-01-30 15:05:44.000000 taskAutom-8.0.4/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-06-22 20:07:24.613219 taskAutom-8.0.4/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      999 2023-06-22 20:06:56.000000 taskAutom-8.0.4/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-22 20:07:24.609219 taskAutom-8.0.4/src/
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-22 20:07:24.613219 taskAutom-8.0.4/src/taskAutom/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       52 2023-06-22 20:07:04.000000 taskAutom-8.0.4/src/taskAutom/__init__.py
+-rwxrwxr-x   0 lucas     (1000) lucas     (1000)    67644 2023-06-22 19:43:46.000000 taskAutom-8.0.4/src/taskAutom/taskAutom.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-06-22 20:07:24.613219 taskAutom-8.0.4/taskAutom.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      512 2023-06-22 20:07:24.000000 taskAutom-8.0.4/taskAutom.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      279 2023-06-22 20:07:24.000000 taskAutom-8.0.4/taskAutom.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-06-22 20:07:24.000000 taskAutom-8.0.4/taskAutom.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       59 2023-06-22 20:07:24.000000 taskAutom-8.0.4/taskAutom.egg-info/entry_points.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       80 2023-06-22 20:07:24.000000 taskAutom-8.0.4/taskAutom.egg-info/requires.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       14 2023-06-22 20:07:24.000000 taskAutom-8.0.4/taskAutom.egg-info/top_level.txt
```

### Comparing `taskAutom-8.0.3/LICENSE` & `taskAutom-8.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `taskAutom-8.0.3/PKG-INFO` & `taskAutom-8.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 8.0.3
+Version: 8.0.4
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `taskAutom-8.0.3/README.md` & `taskAutom-8.0.4/README.md`

 * *Files identical despite different names*

### Comparing `taskAutom-8.0.3/setup.py` & `taskAutom-8.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from importlib.metadata import entry_points
 from setuptools import setup
 
 setup(
     name='taskAutom',
-    version='8.0.3',
+    version='8.0.4',
     description='A simple task automation tool',
     long_description='A simple task automation tool for NOKIA SROS based routers',
     long_description_content_type='text/x-rst',
     url='https://github.com/laimaretto/taskAutom',
     author='Lucas Aimaretto',
     author_email='laimaretto@gmail.com',
     license='BSD 3-clause',
```

### Comparing `taskAutom-8.0.3/src/taskAutom/taskAutom.py` & `taskAutom-8.0.4/src/taskAutom/taskAutom.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import yaml
 import docx
 from docx.enum.style import WD_STYLE_TYPE 
 from docx.enum.text import WD_LINE_SPACING
 from docx.shared import Pt
 
 
-LATEST_VERSION = '8.0.3'
+LATEST_VERSION = '8.0.4'
 
 # Constants
 IP_LOCALHOST  = "127.0.0.1"
 LOG_GLOBAL    = []
 LOG_CONSOLE   = []
 DICT_PARAM    = dict(
 	outputJob        = 0,
@@ -89,14 +89,15 @@
 		SHOW             = "",
 		SEND_CMD_REGEX   = r"#\s+$",
 		MAJOR_ERROR_LIST = ["^FAILED:.+","^ERROR:.+","^Error:.+","invalid token","not allowed"],
 		MINOR_ERROR_LIST = ["^MINOR:.+"],
 		INFO_ERROR_LIST  = ["^INFO:.+"],
 		REMOTE_PORT      = 22,
 		SFTP_PORT        = 22,
+		SFTP_REGEX_CF    = r"(cf\d+:\/|cf\d+:)",
 	),
 	md_nokia_sros=dict(
 		START_SCRIPT     = "", 
 		FIRST_LINE       = "",
 		LAST_LINE        = "",
 		FIN_SCRIPT       = "",
 		VERSION 	     = "show version", # no \n in the end
@@ -108,14 +109,15 @@
 		SHOW             = "info json\n",
 		SEND_CMD_REGEX   = r"#\s+$",
 		MAJOR_ERROR_LIST = ["^FAILED:.+","^ERROR:.+","^Error:.+","invalid token","not allowed"],
 		MINOR_ERROR_LIST = ["^MINOR:.+"],
 		INFO_ERROR_LIST  = ["^INFO:.+"],
 		REMOTE_PORT      = 22,
 		SFTP_PORT        = 22,
+		SFTP_REGEX_CF    = r"(cf\d+:\/|cf\d+:)",
 	),	
 	nokia_sros_telnet=dict(
 		START_SCRIPT     = "", 
 		FIRST_LINE       = "\n/environment no more\n",
 		LAST_LINE        = "\nexit all\n",
 		FIN_SCRIPT       = "#FINSCRIPT",
 		VERSION 	     = "show version", # no \n in the end
@@ -127,14 +129,15 @@
 		SHOW             = "",
 		SEND_CMD_REGEX   = r"#\s+$",
 		MAJOR_ERROR_LIST = ["^FAILED:.+","^ERROR:.+","^Error:.+","invalid token","not allowed"],
 		MINOR_ERROR_LIST = ["^MINOR:.+"],
 		INFO_ERROR_LIST  = ["^INFO:.+"],
 		REMOTE_PORT      = 23,
 		SFTP_PORT        = 22,
+		SFTP_REGEX_CF    = r"(cf\d+:\/|cf\d+:)",
 	),
 )
 
 ####
 
 def fncPrintResults(listOfRouters, timeTotalStart, dictParam):
 
@@ -1194,35 +1197,44 @@
 	def fncUploadFile(self, connInfo):
 		### upload configFile via SFTP
 
 		def setTransport(ip, sftpPort):
 
 			transport = paramiko.Transport((ip,sftpPort))
 			transport.connect(None,connInfo['username'],connInfo['password'])
-
+			
 			# The routers with timos above 6.X do support SFTP.
 			# Otherwise we need to use SCP.
-
-			if connInfo['timosMajor'] > 6:
-				fncPrintConsole(connInfo['strConn'] + "uploading via SFTP: " + str(sftpPort))
-				sftp = paramiko.SFTPClient.from_transport(transport)
+			if connInfo['timosMajor'] != 'not-matched':
+				if connInfo['timosMajor'] > 6:
+					fncPrintConsole(connInfo['strConn'] + "uploading via SFTP: " + str(sftpPort))
+					sftp = paramiko.SFTPClient.from_transport(transport)
+				else:
+					fncPrintConsole(connInfo['strConn'] + "uploading via SCP: " + str(sftpPort))
+					sftp = SCPClient(transport)
 			else:
-				fncPrintConsole(connInfo['strConn'] + "uploading via SCP: " + str(sftpPort))
+				fncPrintConsole(connInfo['strConn'] + "TiMOS not-matched. Asuming SCP. Uploading via SCP: " + str(sftpPort))
 				sftp = SCPClient(transport)
 
 			return transport, sftp
 
 		def sendFiles(sftp,ftpFiles):
 
 			for i, (fileLocal,fileRemote) in enumerate(ftpFiles):
 
-				fncPrintConsole(connInfo['strConn'] + "uploading file: " + fileLocal + "->" + fileRemote)
+				match = re.match(DICT_VENDOR[connInfo['deviceType']]['SFTP_REGEX_CF'], fileRemote)
+
+				if not match:
+					fileRemote = "cf3:/" + fileRemote
+					fncPrintConsole(connInfo['strConn'] + "no CF specified; assuming cf3. Uploading file: " + fileLocal + "->" + fileRemote)
+				else:
+					fncPrintConsole(connInfo['strConn'] + "Uploading file: " + fileLocal + "->" + fileRemote)
 
 				try:
-					sftp.put(fileLocal,'cf3:/' + fileRemote)
+					sftp.put(fileLocal,fileRemote)
 					sftpStatus   = True
 					aluLogReason = 'sftpOk'
 				except Exception as e:
 					print(str(e))
 					sftpStatus   = False
 					aluLogReason = str(e)
 					return sftpStatus, aluLogReason, fileRemote, i
@@ -1261,15 +1273,14 @@
 			sftpStatus, aluLogReason, fileRemote, i = sendFiles(sftp,ftpFiles)
 
 			sftp.close()
 			transport.close()
 			sshServerSftp.stop()			
 
 		else:
-
 			sftpPort = connInfo['sftpPort']
 			transport, sftp = setTransport(connInfo['systemIP'], sftpPort)
 			sftpStatus, aluLogReason, fileRemote, i = sendFiles(sftp,ftpFiles)
 
 			sftp.close()
 			transport.close()
```

### Comparing `taskAutom-8.0.3/taskAutom.egg-info/PKG-INFO` & `taskAutom-8.0.4/taskAutom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskAutom
-Version: 8.0.3
+Version: 8.0.4
 Summary: A simple task automation tool
 Home-page: https://github.com/laimaretto/taskAutom
 Author: Lucas Aimaretto
 Author-email: laimaretto@gmail.com
 License: BSD 3-clause
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
```

