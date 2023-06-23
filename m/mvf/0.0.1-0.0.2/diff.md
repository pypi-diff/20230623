# Comparing `tmp/mvf-0.0.1.tar.gz` & `tmp/mvf-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mvf-0.0.1.tar", last modified: Fri Jun 23 14:31:23 2023, max compression
+gzip compressed data, was "mvf-0.0.2.tar", last modified: Fri Jun 23 15:47:38 2023, max compression
```

## Comparing `mvf-0.0.1.tar` & `mvf-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tom       (2032) users     (2000)        0 2023-06-23 14:31:23.908366 mvf-0.0.1/
--rw-r--r--   0 tom       (2032) users     (2000)      798 2023-06-23 13:09:57.000000 mvf-0.0.1/LICENSE
--rw-r--r--   0 tom       (2032) users     (2000)     1897 2023-06-23 14:31:23.904365 mvf-0.0.1/PKG-INFO
--rw-r--r--   0 tom       (2032) users     (2000)     1392 2023-06-22 14:15:26.000000 mvf-0.0.1/README.md
-drwxr-xr-x   0 tom       (2032) users     (2000)        0 2023-06-23 14:31:23.904365 mvf-0.0.1/mvf.egg-info/
--rw-r--r--   0 tom       (2032) users     (2000)     1897 2023-06-23 14:31:23.000000 mvf-0.0.1/mvf.egg-info/PKG-INFO
--rw-r--r--   0 tom       (2032) users     (2000)      198 2023-06-23 14:31:23.000000 mvf-0.0.1/mvf.egg-info/SOURCES.txt
--rw-r--r--   0 tom       (2032) users     (2000)        1 2023-06-23 14:31:23.000000 mvf-0.0.1/mvf.egg-info/dependency_links.txt
--rw-r--r--   0 tom       (2032) users     (2000)       80 2023-06-23 14:31:23.000000 mvf-0.0.1/mvf.egg-info/requires.txt
--rw-r--r--   0 tom       (2032) users     (2000)        1 2023-06-23 14:31:23.000000 mvf-0.0.1/mvf.egg-info/top_level.txt
--rw-r--r--   0 tom       (2032) users     (2000)       38 2023-06-23 14:31:23.908366 mvf-0.0.1/setup.cfg
--rw-r--r--   0 tom       (2032) users     (2000)     1348 2023-06-23 14:31:13.000000 mvf-0.0.1/setup.py
-drwxr-xr-x   0 tom       (2032) users     (2000)        0 2023-06-23 14:31:23.904365 mvf-0.0.1/test/
--rw-r--r--   0 tom       (2032) users     (2000)      102 2023-05-30 16:00:29.000000 mvf-0.0.1/test/test_python_testing_framework.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:47:38.876420 mvf-0.0.2/
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-06-23 15:47:35.000000 mvf-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-06-23 15:47:38.875420 mvf-0.0.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2301 2023-06-23 15:47:35.000000 mvf-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:47:38.875420 mvf-0.0.2/mvf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-06-23 15:47:38.000000 mvf-0.0.2/mvf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      198 2023-06-23 15:47:38.000000 mvf-0.0.2/mvf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 15:47:38.000000 mvf-0.0.2/mvf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       86 2023-06-23 15:47:38.000000 mvf-0.0.2/mvf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-23 15:47:38.000000 mvf-0.0.2/mvf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-23 15:47:38.876420 mvf-0.0.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1378 2023-06-23 15:47:35.000000 mvf-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-23 15:47:38.875420 mvf-0.0.2/test/
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-23 15:47:35.000000 mvf-0.0.2/test/test_python_testing_framework.py
```

### Comparing `mvf-0.0.1/LICENSE` & `mvf-0.0.2/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -5,9 +5,9 @@
 direct, indirect, incidental, special, exemplary, or consequential damages
 (including, but not limited to, procurement of substitute goods or services;
 loss of use, data, or profits; or business interruption) however caused and
 on any theory of liability, whether in contract, strict liability, or tort
 (including negligence or otherwise) arising in any way out of the use of this
 software, even if advised of the possibility of such damage.
 
-Copyright (c) 2000-2021 Certus Technology Associates Limited.
+Copyright (c) 2000-2023 Certus Technology Associates Limited.
 All Rights Reserved.
```

### Comparing `mvf-0.0.1/PKG-INFO` & `mvf-0.0.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: mvf
-Version: 0.0.1
-Summary: A package implementing a supervised model validation framework.
+Version: 0.0.2
+Summary: A package implementing a supervised learning model validation framework.
+Home-page: UNKNOWN
 Author: Tom Kim
 Author-email: tom.kim@certus-tech.com
+License: UNKNOWN
 Keywords: python,R,machine learning,validation,framework
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Jupyter
 Classifier: License :: Free For Educational Use
 Classifier: Operating System :: Unix
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# Model Validation Framework
-
 description here...
 
 ## Getting Started
 
 For full documentation of the project and instructions on how to get started, visit the [documentation site](https://tomkimcta.gitlab.io/model-validation-framework).
 
 ## Project Administration
@@ -33,17 +34,44 @@
 ### Git
 
 This project operates using two Git branches
 
 - dev
 - main
 
-All development work should be undertaken on the development branch. The dev branch should then be merged into the master branch when key milestones are met.
+All development work should be undertaken on the development branch. The dev branch should then be merged into the master branch to deploy a new version of the package. 
+
+### CI/CD
+
+This project uses GitLab CI/CD. There are currently three stages in the CI/CD pipeline
+
+* **test** - Runs any CI/CD tests using [pytest](https://docs.pytest.org).
+* **build_deploy_package** - Builds the Python package and deploys to [PyPI](https://pypi.org/).
+* **build_deploy_docs** - Builds the documentation site and deploys to [GitLab Pages](https://docs.gitlab.com/ee/user/project/pages/).
+
+The **test** stage runs on every commit. The **build_deploy_package** and **build_deploy_docs** stages only run on commits to the `main` branch. All CI/CD stages run in a Docker container. This project uses `node:latest` for the **build_deploy_docs** stage and a custom R/Python container for the remaining stages.
+
+#### Docker
 
-### Testing Framework
+To update the container in the registry, navigate to the project root and run
 
-Tests run in CI on every commit. Python code is tested using [pytest](https://docs.pytest.org) in a Python Virtual Environment specified by `requirements.txt`. 
+```
+sudo docker login registry.gitlab.com
+```
+
+Enter your GitLab username and password (only for members of the project). Then run
+
+```
+sudo docker build -t registry.gitlab.com/tomkimcta/model-validation-framework .
+sudo docker push registry.gitlab.com/tomkimcta/model-validation-framework
+```
+
+#### PyPI
+
+The version stored in the `version` file must be incremented for a deployment of the package to be successful.
 
 ### Documentation
 
-This project uses a static site generator called [Docusaurus](https://docusaurus.io) to create its documentation. The content for the documentation site is contained in `documentation/docs/`. Any updates to documentation can be verified in a development server by running `npm i && npm start` from the `documentation/` directory. The public documentation site is rebuilt only for commits to the main branch. This is primarily to economise CI minutes.
+This project uses a static site generator called [Docusaurus](https://docusaurus.io) to create its documentation. The content for the documentation site is contained in `documentation/docs/`. Any updates to documentation can be verified in a development server by running `npm i && npm start` from the `documentation/` directory.
+
+
```

### Comparing `mvf-0.0.1/README.md` & `mvf-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-# Model Validation Framework
-
 description here...
 
 ## Getting Started
 
 For full documentation of the project and instructions on how to get started, visit the [documentation site](https://tomkimcta.gitlab.io/model-validation-framework).
 
 ## Project Administration
@@ -17,17 +15,42 @@
 ### Git
 
 This project operates using two Git branches
 
 - dev
 - main
 
-All development work should be undertaken on the development branch. The dev branch should then be merged into the master branch when key milestones are met.
+All development work should be undertaken on the development branch. The dev branch should then be merged into the master branch to deploy a new version of the package. 
+
+### CI/CD
+
+This project uses GitLab CI/CD. There are currently three stages in the CI/CD pipeline
+
+* **test** - Runs any CI/CD tests using [pytest](https://docs.pytest.org).
+* **build_deploy_package** - Builds the Python package and deploys to [PyPI](https://pypi.org/).
+* **build_deploy_docs** - Builds the documentation site and deploys to [GitLab Pages](https://docs.gitlab.com/ee/user/project/pages/).
+
+The **test** stage runs on every commit. The **build_deploy_package** and **build_deploy_docs** stages only run on commits to the `main` branch. All CI/CD stages run in a Docker container. This project uses `node:latest` for the **build_deploy_docs** stage and a custom R/Python container for the remaining stages.
+
+#### Docker
+
+To update the container in the registry, navigate to the project root and run
+
+```
+sudo docker login registry.gitlab.com
+```
+
+Enter your GitLab username and password (only for members of the project). Then run
+
+```
+sudo docker build -t registry.gitlab.com/tomkimcta/model-validation-framework .
+sudo docker push registry.gitlab.com/tomkimcta/model-validation-framework
+```
 
-### Testing Framework
+#### PyPI
 
-Tests run in CI on every commit. Python code is tested using [pytest](https://docs.pytest.org) in a Python Virtual Environment specified by `requirements.txt`. 
+The version stored in the `version` file must be incremented for a deployment of the package to be successful.
 
 ### Documentation
 
-This project uses a static site generator called [Docusaurus](https://docusaurus.io) to create its documentation. The content for the documentation site is contained in `documentation/docs/`. Any updates to documentation can be verified in a development server by running `npm i && npm start` from the `documentation/` directory. The public documentation site is rebuilt only for commits to the main branch. This is primarily to economise CI minutes.
+This project uses a static site generator called [Docusaurus](https://docusaurus.io) to create its documentation. The content for the documentation site is contained in `documentation/docs/`. Any updates to documentation can be verified in a development server by running `npm i && npm start` from the `documentation/` directory.
```

### Comparing `mvf-0.0.1/mvf.egg-info/PKG-INFO` & `mvf-0.0.2/mvf.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: mvf
-Version: 0.0.1
-Summary: A package implementing a supervised model validation framework.
+Version: 0.0.2
+Summary: A package implementing a supervised learning model validation framework.
+Home-page: UNKNOWN
 Author: Tom Kim
 Author-email: tom.kim@certus-tech.com
+License: UNKNOWN
 Keywords: python,R,machine learning,validation,framework
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Framework :: Jupyter
 Classifier: License :: Free For Educational Use
 Classifier: Operating System :: Unix
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# Model Validation Framework
-
 description here...
 
 ## Getting Started
 
 For full documentation of the project and instructions on how to get started, visit the [documentation site](https://tomkimcta.gitlab.io/model-validation-framework).
 
 ## Project Administration
@@ -33,17 +34,44 @@
 ### Git
 
 This project operates using two Git branches
 
 - dev
 - main
 
-All development work should be undertaken on the development branch. The dev branch should then be merged into the master branch when key milestones are met.
+All development work should be undertaken on the development branch. The dev branch should then be merged into the master branch to deploy a new version of the package. 
+
+### CI/CD
+
+This project uses GitLab CI/CD. There are currently three stages in the CI/CD pipeline
+
+* **test** - Runs any CI/CD tests using [pytest](https://docs.pytest.org).
+* **build_deploy_package** - Builds the Python package and deploys to [PyPI](https://pypi.org/).
+* **build_deploy_docs** - Builds the documentation site and deploys to [GitLab Pages](https://docs.gitlab.com/ee/user/project/pages/).
+
+The **test** stage runs on every commit. The **build_deploy_package** and **build_deploy_docs** stages only run on commits to the `main` branch. All CI/CD stages run in a Docker container. This project uses `node:latest` for the **build_deploy_docs** stage and a custom R/Python container for the remaining stages.
+
+#### Docker
 
-### Testing Framework
+To update the container in the registry, navigate to the project root and run
 
-Tests run in CI on every commit. Python code is tested using [pytest](https://docs.pytest.org) in a Python Virtual Environment specified by `requirements.txt`. 
+```
+sudo docker login registry.gitlab.com
+```
+
+Enter your GitLab username and password (only for members of the project). Then run
+
+```
+sudo docker build -t registry.gitlab.com/tomkimcta/model-validation-framework .
+sudo docker push registry.gitlab.com/tomkimcta/model-validation-framework
+```
+
+#### PyPI
+
+The version stored in the `version` file must be incremented for a deployment of the package to be successful.
 
 ### Documentation
 
-This project uses a static site generator called [Docusaurus](https://docusaurus.io) to create its documentation. The content for the documentation site is contained in `documentation/docs/`. Any updates to documentation can be verified in a development server by running `npm i && npm start` from the `documentation/` directory. The public documentation site is rebuilt only for commits to the main branch. This is primarily to economise CI minutes.
+This project uses a static site generator called [Docusaurus](https://docusaurus.io) to create its documentation. The content for the documentation site is contained in `documentation/docs/`. Any updates to documentation can be verified in a development server by running `npm i && npm start` from the `documentation/` directory.
+
+
```

### Comparing `mvf-0.0.1/setup.py` & `mvf-0.0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 setup(
     name='mvf',
     version=_get_version(),
     author='Tom Kim',
     author_email='tom.kim@certus-tech.com',
-    description='A package implementing a supervised model validation framework.',
+    description='A package implementing a supervised learning model validation framework.',
     long_description=_get_long_description(),
     long_description_content_type='text/markdown',
     packages=find_packages(
         exclude=[
             'test*',
             'documentation*',
             'examples*',
@@ -37,14 +37,15 @@
         'rpy2-r6',
         'scikit-learn',
     ],
     extras_require={
         'dev': [
             'coverage',
             'pytest',
+            'twine',
         ]
     },
     keywords=[
         'python',
         'R',
         'machine learning',
         'validation',
```

