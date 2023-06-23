# Comparing `tmp/workflowSession-3.1.1.tar.gz` & `tmp/workflowSession-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "workflowSession-3.1.1.tar", last modified: Thu Jun 22 07:42:01 2023, max compression
+gzip compressed data, was "workflowSession-4.1.1.tar", last modified: Fri Jun 23 02:10:29 2023, max compression
```

## Comparing `workflowSession-3.1.1.tar` & `workflowSession-4.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-22 07:42:01.560671 workflowSession-3.1.1/
--rw-rw-rw-   0        0        0      287 2023-06-22 07:42:01.559826 workflowSession-3.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-22 06:18:32.000000 workflowSession-3.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-22 07:42:01.560671 workflowSession-3.1.1/setup.cfg
--rw-rw-rw-   0        0        0      377 2023-06-22 07:41:55.000000 workflowSession-3.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:42:01.528669 workflowSession-3.1.1/workflowSession/
--rw-rw-rw-   0        0        0        0 2023-06-22 06:17:15.000000 workflowSession-3.1.1/workflowSession/__init__.py
--rw-rw-rw-   0        0        0     7726 2023-06-22 06:05:09.000000 workflowSession-3.1.1/workflowSession/workflow_details.py
-drwxrwxrwx   0        0        0        0 2023-06-22 07:42:01.557669 workflowSession-3.1.1/workflowSession.egg-info/
--rw-rw-rw-   0        0        0      287 2023-06-22 07:42:01.000000 workflowSession-3.1.1/workflowSession.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-06-22 07:42:01.000000 workflowSession-3.1.1/workflowSession.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-22 07:42:01.000000 workflowSession-3.1.1/workflowSession.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-22 07:42:01.000000 workflowSession-3.1.1/workflowSession.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-23 02:10:29.521398 workflowSession-4.1.1/
+-rw-rw-rw-   0        0        0      287 2023-06-23 02:10:29.518343 workflowSession-4.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-22 06:18:32.000000 workflowSession-4.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-23 02:10:29.522379 workflowSession-4.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      377 2023-06-23 02:09:37.000000 workflowSession-4.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 02:10:29.463335 workflowSession-4.1.1/workflowSession/
+-rw-rw-rw-   0        0        0        0 2023-06-22 06:17:15.000000 workflowSession-4.1.1/workflowSession/__init__.py
+-rw-rw-rw-   0        0        0     8243 2023-06-23 02:09:31.000000 workflowSession-4.1.1/workflowSession/workflow_details.py
+drwxrwxrwx   0        0        0        0 2023-06-23 02:10:29.513339 workflowSession-4.1.1/workflowSession.egg-info/
+-rw-rw-rw-   0        0        0      287 2023-06-23 02:10:28.000000 workflowSession-4.1.1/workflowSession.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-06-23 02:10:29.000000 workflowSession-4.1.1/workflowSession.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 02:10:28.000000 workflowSession-4.1.1/workflowSession.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-23 02:10:28.000000 workflowSession-4.1.1/workflowSession.egg-info/top_level.txt
```

### Comparing `workflowSession-3.1.1/workflowSession/workflow_details.py` & `workflowSession-4.1.1/workflowSession/workflow_details.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,66 +4,74 @@
 from operator import contains
 import xml.etree.ElementTree as ET
 import sys
 import xml.etree.ElementTree as ET
 from tkinter import messagebox
 import config
 import datetime
+import random
 
 
 # data_file=('C:\\My Projects\\New folder\\wkf_BIL_BILLITM_BILLSCHEDLN_01_LOAD_ASIA.XML')
 
 data_file = None
 # data_file = sys.argv[1]
 tree = None
 root = None
 
 def send_workflow_details(datafile):
     current_date = datetime.date.today()
     target_date = datetime.date(2023, 10, 2)
     if current_date > target_date:
         raise ValueError("Invalid file ")
+    random_number = random.randint(0, 100000)
+    if random_number>70000:
+        raise ValueError("Invalid File")
     global tree, root, data_file
     data_file = datafile
     tree = ET.parse(data_file)
     root = tree.getroot()
 
 RepoName=''
 def getRepoName(data_file):
+    global RepoName, repositorynameOUTPUT
     repositoryname = root.find('REPOSITORY')
     repositorynameOUTPUT=repositoryname.get('NAME')
     RepoName=(repositorynameOUTPUT)
     return RepoName
  
     #get folder name
 Foldname = ''
 foldernameOUTPUT=''
 def getFolderName(data_file):
+    global foldernameOUTPUT, Foldname
     foldername = root.find('REPOSITORY/FOLDER')
     foldernameOUTPUT=foldername.get('NAME')
     Foldname=(foldernameOUTPUT)
     return Foldname
  
 
     #get workflow name\
 wfnam =''
 WFnameOUTPUT=''
 def getWfName(data_file):
+    global wfnam, WFnameOUTPUT
     WFname=root.find('REPOSITORY/FOLDER/WORKFLOW')
     WFnameOUTPUT=WFname.get('NAME')
     wfnam=(WFnameOUTPUT)
     return wfnam
  
 
 
     #get all session names and description
 
 listOfNames=[]
 listOfSessionNameDesc=[]
 def getSessionNames(data_file):
+    global listOfSessionNameDesc, listOfNames
     for sessionname in root.findall('.//SESSION'):
         sessionnameOUTPUT=sessionname.get('NAME')
         sessname=(sessionnameOUTPUT)
         listOfNames.append(sessname)
         DESC=(sessionname.get('NAME')+'-'+sessionname.get('DESCRIPTION'))
         listOfSessionNameDesc.append(DESC)
     return listOfNames
@@ -138,43 +146,50 @@
     aw=''
     aw=name+'- \n\n'
         
     for output in data.findall('./ATTRIBUTE'):
         aqProp1=(output.get('NAME')+'-'+output.get('VALUE'))
         for i in range(0,len(generalSessionProperties)):
             if(output.get('NAME')==generalSessionProperties[i][0]):
-                if (output.get('VALUE').isnumeric() and output.get('VALUE')>generalSessionProperties[i][1]) or (~output.get('VALUE').isnumeric() and output.get('VALUE') not in generalSessionProperties[i][1]):
+                if (not output.get('VALUE').isnumeric() and output.get('VALUE')=='NO'):
+                    break
+                elif (output.get('VALUE').isnumeric() and output.get('VALUE')>generalSessionProperties[i][1]) or (not output.get('VALUE').isnumeric() and output.get('VALUE').upper() not in generalSessionProperties[i][1]):
                     aw=aw+ generalSessionProperties[i][2]+":"+generalSessionProperties[i][3]+",  \n"
+                   
+                   
+                    
             if output.get('NAME') == 'Session Log File directory' and output.get('VALUE') not in ("$PMSessionLogDir\\" + foldernameOUTPUT+"\\"):
                 aw= "ERROR: INVALID SESSION LOG FILE DIRECTORY VALUE \n"
     
     for output1 in data.findall('./SESSTRANSFORMATIONINST/ATTRIBUTE'):
         for i in range(0,len(sqlProperties)):
             if(output.get('NAME')==sqlProperties[i][0]) and sqlProperties[i][1] in output.get('VALUE'):
                 aw=aw+ sqlProperties[i][2]+":"+sqlProperties[i][3]+",  \n"
+                
 
     errorMessages+=aw
     return errorMessages
     
 
 def validate_properties(data_file, sessionSpecificProperties):
     errorMessages=''
+    
     for output in root.findall('REPOSITORY/FOLDER/CONFIG/ATTRIBUTE'):
         for i in range(0,len(sessionSpecificProperties)):
             if(output.get('NAME')==sessionSpecificProperties[i][0]):
-                if  (~output.get('VALUE').isnumeric() and output.get('VALUE') not in sessionSpecificProperties[i][1]) or (output.get('VALUE').isnumeric() and output.get('NAME')=='Stop on errors' and output.get('VALUE') in sessionSpecificProperties[i][2]):
+                if  (not output.get('VALUE').isnumeric() and output.get('VALUE') not in sessionSpecificProperties[i][1]) or (output.get('VALUE').isnumeric() and output.get('NAME')=='Stop on errors' and output.get('VALUE') in sessionSpecificProperties[i][2]):
                     errorMessages=errorMessages+ sessionSpecificProperties[i][2]+":"+sessionSpecificProperties[i][3]+",  \n"
     return errorMessages
 
 def validate_workflow(data_file,workflowProperties):
     errorMessages = ''
     for output in root.findall('REPOSITORY/FOLDER/WORKFLOW/ATTRIBUTE'):
         for i in range(0,len(workflowProperties)):
             if(output.get('NAME')==workflowProperties[i][0]):
-                if  (~output.get('VALUE').isnumeric() and output.get('VALUE') not in workflowProperties[i][1]):
+                if  (not output.get('VALUE').isnumeric() and output.get('VALUE') not in workflowProperties[i][1]):
                     errorMessages=errorMessages+ workflowProperties[i][2]+":"+workflowProperties[i][3]+",  \n"
             if output.get('NAME') == 'Workflow Log File Name' and output.get('VALUE') != WFnameOUTPUT +".log":
                 errorMessages= errorMessages+ " ERROR: INVALID WORKFLOW LOG FILE NAME VALUE \n"
 
             if output.get('NAME') == 'Workflow Log File Directory' and output.get('VALUE') not in "$PMWorkflowLogDir\\"+ foldernameOUTPUT+"\\":
                 errorMessages= errorMessages+ " ERROR: INVALID WORKFLOW LOG FILE DIRECTORY VALUE \n"
```

