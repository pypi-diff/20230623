# Comparing `tmp/iseqdockertools-0.0.2.tar.gz` & `tmp/iseqdockertools-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iseqdockertools-0.0.2.tar", last modified: Tue Aug 16 13:13:17 2022, max compression
+gzip compressed data, was "iseqdockertools-0.0.3.tar", last modified: Fri Jun 23 10:02:32 2023, max compression
```

## Comparing `iseqdockertools-0.0.2.tar` & `iseqdockertools-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2022-08-16 13:13:17.596533 iseqdockertools-0.0.2/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      461 2022-08-02 09:30:12.000000 iseqdockertools-0.0.2/LICENSE
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     2331 2022-08-16 13:13:17.596533 iseqdockertools-0.0.2/PKG-INFO
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     1870 2022-08-16 12:55:20.000000 iseqdockertools-0.0.2/README.md
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      104 2022-08-02 09:18:21.000000 iseqdockertools-0.0.2/pyproject.toml
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      619 2022-08-16 13:13:17.596533 iseqdockertools-0.0.2/setup.cfg
--rw-rw-r--   0 olaf      (1000) olaf      (1000)       69 2022-08-11 13:28:23.000000 iseqdockertools-0.0.2/setup.py
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2022-08-16 13:13:17.596533 iseqdockertools-0.0.2/src/
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2022-08-16 13:13:17.596533 iseqdockertools-0.0.2/src/iseqdocker/
--rwxr-xr-x   0 olaf      (1000) olaf      (1000)     4939 2022-08-11 10:46:08.000000 iseqdockertools-0.0.2/src/iseqdocker/dockerbuilder
-drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2022-08-16 13:13:17.596533 iseqdockertools-0.0.2/src/iseqdockertools.egg-info/
--rw-rw-r--   0 olaf      (1000) olaf      (1000)     2331 2022-08-16 13:13:17.000000 iseqdockertools-0.0.2/src/iseqdockertools.egg-info/PKG-INFO
--rw-rw-r--   0 olaf      (1000) olaf      (1000)      252 2022-08-16 13:13:17.000000 iseqdockertools-0.0.2/src/iseqdockertools.egg-info/SOURCES.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        1 2022-08-16 13:13:17.000000 iseqdockertools-0.0.2/src/iseqdockertools.egg-info/dependency_links.txt
--rw-rw-r--   0 olaf      (1000) olaf      (1000)        1 2022-08-16 13:13:17.000000 iseqdockertools-0.0.2/src/iseqdockertools.egg-info/top_level.txt
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2023-06-23 10:02:32.599017 iseqdockertools-0.0.3/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      461 2022-08-02 09:30:12.000000 iseqdockertools-0.0.3/LICENSE
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     3449 2023-06-23 10:02:32.599017 iseqdockertools-0.0.3/PKG-INFO
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     2988 2023-06-23 09:58:40.000000 iseqdockertools-0.0.3/README.md
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      104 2022-08-02 09:18:21.000000 iseqdockertools-0.0.3/pyproject.toml
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      619 2023-06-23 10:02:32.603016 iseqdockertools-0.0.3/setup.cfg
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)       69 2022-08-11 13:28:23.000000 iseqdockertools-0.0.3/setup.py
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2023-06-23 10:02:32.595017 iseqdockertools-0.0.3/src/
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2023-06-23 10:02:32.599017 iseqdockertools-0.0.3/src/iseqdocker/
+-rwxrwxr-x   0 olaf      (1000) olaf      (1000)     9466 2023-06-22 09:27:46.000000 iseqdockertools-0.0.3/src/iseqdocker/dockerbuilder
+drwxrwxr-x   0 olaf      (1000) olaf      (1000)        0 2023-06-23 10:02:32.599017 iseqdockertools-0.0.3/src/iseqdockertools.egg-info/
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)     3449 2023-06-23 10:02:32.000000 iseqdockertools-0.0.3/src/iseqdockertools.egg-info/PKG-INFO
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)      252 2023-06-23 10:02:32.000000 iseqdockertools-0.0.3/src/iseqdockertools.egg-info/SOURCES.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        1 2023-06-23 10:02:32.000000 iseqdockertools-0.0.3/src/iseqdockertools.egg-info/dependency_links.txt
+-rw-rw-r--   0 olaf      (1000) olaf      (1000)        1 2023-06-23 10:02:32.000000 iseqdockertools-0.0.3/src/iseqdockertools.egg-info/top_level.txt
```

### Comparing `iseqdockertools-0.0.2/PKG-INFO` & `iseqdockertools-0.0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: iseqdockertools
-Version: 0.0.2
-Summary: Intelliseq tools needed to manage dockers
-Home-page: https://gitlab.com/intelliseq/iseqdockertools
-Author: motfalo
-Author-email: olaf.tomaszewski@intelliseq.pl
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: Free for non-commercial use
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ##### Install iseqdockertools lib
 
 Optional steps (create virtual environment):
 ```
 python3 -m venv venv
 source tutorial_env/bin/activate
 ```
@@ -23,25 +9,46 @@
 
 Obligatory steps:
 ```
 python3 -m pip install --upgrade pip
 pip install iseqdockertools
 ```
 
+##### File containing versions for tools: docker-versions.json
 
+In workflows' directory it is located in `src/main/resources/docker-versions.json`
+It contains info about the tools' versions in .json format.
+For example:
+```
+{
+    "PHARMCAT_VER": "2.3.0",
+    "FASTQC_VER": "0.12.1"
+}
+```
+To update it you need to use iseqresources.
+The details are there: https://gitlab.com/intelliseq/iseqresources
 
 ##### Build docker images
 
 Script automatically takes name and version of the docker image from its header.
 It has to be in the following format (at the beginning of the Dockerfile):
 ```
 # name: name
 # version: 1.0.0
 ```
 
+If you want to update the tools' versions automatically:
+1. Check if it is generated by iseqresources to the docker-versions.json
+2. Add to the beginning of dockerfile (below `FROM`)
+```
+ARG TOOL1_VER
+ARG TOOL2_VER
+```
+3. The version (if found) will be automatically taken from the docker-versions.json
+
 Building has default context to repository and you can use ADD with path to the files from here. 
 Default option is to push to the dockerhub. If the dockerfile exists it won't be pushed. To develop dockerimage locally use flag --nopush. 
 
 ##### Usage (when you are in workflows' root directory):
 ```
 dockerbuilder -d path/to/dockerfile
 ```
@@ -63,19 +70,31 @@
 ```
 dockerbuilder -d path/to/dockerfile --nocache
 ```
 4. Build separate images for all chromosomes
 ```
 dockerbuilder -d path/to/dockerfile --chromosome
 ```
-5. Push image even if exists in repository
+5. Provide custom path to docker-versions.json
+```
+dockerbuilder -d path/to/dockerfile --versions
+```
+6. Ignore docker-versions.json
+```
+dockerbuilder -d path/to/dockerfile --ignore-versions
+```
+7. Ignore version number from image name (for example # name tool-1.15b version won't be updated to the newest found (tool-1.18c) in docker-versions.json)
+```
+dockerbuilder -d path/to/dockerfile --ignore-name-version
+```
+8. Push image even if exists in repository
 ```
 dockerbuilder -d path/to/dockerfile --forcepush
 ```
-6. Set current directory as context
+9. Set current directory as context
 ```
 dockerbuilder -d path/to/dockerfile --context
 ```
 
 You can mix flags whenever you need to.
 
 ##### Name of the docker image vs location of its dockerfile
@@ -83,8 +102,8 @@
 Location: 
 ```src/main/docker/[catalog-name]/[version]/Dockefile```
 
 Name of the image: ```intelliseqngs/[catalog-name]:[version]```
 
 
 More info here:
-https://workflows-dev-documentation.readthedocs.io/en/latest/Docker.html
+https://workflows-dev-documentation.readthedocs.io/en/latest/Docker.html
```

### Comparing `iseqdockertools-0.0.2/README.md` & `iseqdockertools-0.0.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: iseqdockertools
+Version: 0.0.3
+Summary: Intelliseq tools needed to manage dockers
+Home-page: https://gitlab.com/intelliseq/iseqdockertools
+Author: motfalo
+Author-email: olaf.tomaszewski@intelliseq.pl
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: Free for non-commercial use
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ##### Install iseqdockertools lib
 
 Optional steps (create virtual environment):
 ```
 python3 -m venv venv
 source tutorial_env/bin/activate
 ```
@@ -9,25 +23,46 @@
 
 Obligatory steps:
 ```
 python3 -m pip install --upgrade pip
 pip install iseqdockertools
 ```
 
+##### File containing versions for tools: docker-versions.json
 
+In workflows' directory it is located in `src/main/resources/docker-versions.json`
+It contains info about the tools' versions in .json format.
+For example:
+```
+{
+    "PHARMCAT_VER": "2.3.0",
+    "FASTQC_VER": "0.12.1"
+}
+```
+To update it you need to use iseqresources.
+The details are there: https://gitlab.com/intelliseq/iseqresources
 
 ##### Build docker images
 
 Script automatically takes name and version of the docker image from its header.
 It has to be in the following format (at the beginning of the Dockerfile):
 ```
 # name: name
 # version: 1.0.0
 ```
 
+If you want to update the tools' versions automatically:
+1. Check if it is generated by iseqresources to the docker-versions.json
+2. Add to the beginning of dockerfile (below `FROM`)
+```
+ARG TOOL1_VER
+ARG TOOL2_VER
+```
+3. The version (if found) will be automatically taken from the docker-versions.json
+
 Building has default context to repository and you can use ADD with path to the files from here. 
 Default option is to push to the dockerhub. If the dockerfile exists it won't be pushed. To develop dockerimage locally use flag --nopush. 
 
 ##### Usage (when you are in workflows' root directory):
 ```
 dockerbuilder -d path/to/dockerfile
 ```
@@ -49,19 +84,31 @@
 ```
 dockerbuilder -d path/to/dockerfile --nocache
 ```
 4. Build separate images for all chromosomes
 ```
 dockerbuilder -d path/to/dockerfile --chromosome
 ```
-5. Push image even if exists in repository
+5. Provide custom path to docker-versions.json
+```
+dockerbuilder -d path/to/dockerfile --versions
+```
+6. Ignore docker-versions.json
+```
+dockerbuilder -d path/to/dockerfile --ignore-versions
+```
+7. Ignore version number from image name (for example # name tool-1.15b version won't be updated to the newest found (tool-1.18c) in docker-versions.json)
+```
+dockerbuilder -d path/to/dockerfile --ignore-name-version
+```
+8. Push image even if exists in repository
 ```
 dockerbuilder -d path/to/dockerfile --forcepush
 ```
-6. Set current directory as context
+9. Set current directory as context
 ```
 dockerbuilder -d path/to/dockerfile --context
 ```
 
 You can mix flags whenever you need to.
 
 ##### Name of the docker image vs location of its dockerfile
@@ -69,8 +116,8 @@
 Location: 
 ```src/main/docker/[catalog-name]/[version]/Dockefile```
 
 Name of the image: ```intelliseqngs/[catalog-name]:[version]```
 
 
 More info here:
-https://workflows-dev-documentation.readthedocs.io/en/latest/Docker.html
+https://workflows-dev-documentation.readthedocs.io/en/latest/Docker.html
```

### Comparing `iseqdockertools-0.0.2/setup.cfg` & `iseqdockertools-0.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iseqdockertools
-version = 0.0.2
+version = 0.0.3
 author = motfalo
 author_email = olaf.tomaszewski@intelliseq.pl
 description = Intelliseq tools needed to manage dockers
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/intelliseq/iseqdockertools
 classifiers =
```

### Comparing `iseqdockertools-0.0.2/src/iseqdockertools.egg-info/PKG-INFO` & `iseqdockertools-0.0.3/src/iseqdockertools.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iseqdockertools
-Version: 0.0.2
+Version: 0.0.3
 Summary: Intelliseq tools needed to manage dockers
 Home-page: https://gitlab.com/intelliseq/iseqdockertools
 Author: motfalo
 Author-email: olaf.tomaszewski@intelliseq.pl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free for non-commercial use
 Classifier: Operating System :: OS Independent
@@ -23,25 +23,46 @@
 
 Obligatory steps:
 ```
 python3 -m pip install --upgrade pip
 pip install iseqdockertools
 ```
 
+##### File containing versions for tools: docker-versions.json
 
+In workflows' directory it is located in `src/main/resources/docker-versions.json`
+It contains info about the tools' versions in .json format.
+For example:
+```
+{
+    "PHARMCAT_VER": "2.3.0",
+    "FASTQC_VER": "0.12.1"
+}
+```
+To update it you need to use iseqresources.
+The details are there: https://gitlab.com/intelliseq/iseqresources
 
 ##### Build docker images
 
 Script automatically takes name and version of the docker image from its header.
 It has to be in the following format (at the beginning of the Dockerfile):
 ```
 # name: name
 # version: 1.0.0
 ```
 
+If you want to update the tools' versions automatically:
+1. Check if it is generated by iseqresources to the docker-versions.json
+2. Add to the beginning of dockerfile (below `FROM`)
+```
+ARG TOOL1_VER
+ARG TOOL2_VER
+```
+3. The version (if found) will be automatically taken from the docker-versions.json
+
 Building has default context to repository and you can use ADD with path to the files from here. 
 Default option is to push to the dockerhub. If the dockerfile exists it won't be pushed. To develop dockerimage locally use flag --nopush. 
 
 ##### Usage (when you are in workflows' root directory):
 ```
 dockerbuilder -d path/to/dockerfile
 ```
@@ -63,19 +84,31 @@
 ```
 dockerbuilder -d path/to/dockerfile --nocache
 ```
 4. Build separate images for all chromosomes
 ```
 dockerbuilder -d path/to/dockerfile --chromosome
 ```
-5. Push image even if exists in repository
+5. Provide custom path to docker-versions.json
+```
+dockerbuilder -d path/to/dockerfile --versions
+```
+6. Ignore docker-versions.json
+```
+dockerbuilder -d path/to/dockerfile --ignore-versions
+```
+7. Ignore version number from image name (for example # name tool-1.15b version won't be updated to the newest found (tool-1.18c) in docker-versions.json)
+```
+dockerbuilder -d path/to/dockerfile --ignore-name-version
+```
+8. Push image even if exists in repository
 ```
 dockerbuilder -d path/to/dockerfile --forcepush
 ```
-6. Set current directory as context
+9. Set current directory as context
 ```
 dockerbuilder -d path/to/dockerfile --context
 ```
 
 You can mix flags whenever you need to.
 
 ##### Name of the docker image vs location of its dockerfile
```

