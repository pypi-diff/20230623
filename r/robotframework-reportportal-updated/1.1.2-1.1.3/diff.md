# Comparing `tmp/robotframework-reportportal_updated-1.1.2.tar.gz` & `tmp/robotframework-reportportal_updated-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-reportportal_updated-1.1.2.tar", last modified: Mon May  8 12:33:34 2023, max compression
+gzip compressed data, was "robotframework-reportportal_updated-1.1.3.tar", last modified: Fri Jun 23 07:57:55 2023, max compression
```

## Comparing `robotframework-reportportal_updated-1.1.2.tar` & `robotframework-reportportal_updated-1.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.703762 robotframework-reportportal_updated-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-08 12:33:34.703762 robotframework-reportportal_updated-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.703762 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)    11240 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/listener.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/model.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/post_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/result_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/result_visitor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/static.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/static.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/time_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/variables.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:33:34.703762 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-08 12:33:34.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-08 12:33:34.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:33:34.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-08 12:33:34.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-08 12:33:34.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-08 12:33:34.000000 robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-08 12:33:34.703762 robotframework-reportportal_updated-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-08 12:33:30.000000 robotframework-reportportal_updated-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:57:55.431334 robotframework-reportportal_updated-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-23 07:57:55.431334 robotframework-reportportal_updated-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:57:55.427334 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/listener.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8176 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/model.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/post_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/result_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/result_visitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10727 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/static.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/time_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5251 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/variables.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 07:57:55.431334 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6931 2023-06-23 07:57:55.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-23 07:57:55.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 07:57:55.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 07:57:55.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-23 07:57:55.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-23 07:57:55.000000 robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-23 07:57:55.431334 robotframework-reportportal_updated-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-23 07:57:47.000000 robotframework-reportportal_updated-1.1.3/setup.py
```

### Comparing `robotframework-reportportal_updated-1.1.2/CONTRIBUTING.rst` & `robotframework-reportportal_updated-1.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.2/LICENSE.txt` & `robotframework-reportportal_updated-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.2/PKG-INFO` & `robotframework-reportportal_updated-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: robotframework-reportportal_updated
-Version: 1.1.2
+Version: 1.1.3
 Summary: Agent for reporting RobotFramework test results to Report Portal
 Home-page: https://github.com/reportportal/agent-Python-RobotFramework
-Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.1.2
+Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.1.3
 Author: Report Portal Team
 Author-email: support@reportportal.io
 Keywords: testing,reporting,robot framework,reportportal,agent
 Classifier: Framework :: Robot Framework
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ReportPortal RobotFramework agent
 
 [![PyPI](https://img.shields.io/pypi/v/robotframework-reportportal.svg?maxAge=259200)](https://pypi.python.org/pypi/robotframework-reportportal)
 [![Python versions](https://img.shields.io/pypi/pyversions/robotframework-reportportal.svg)](https://pypi.org/project/robotframework-reportportal)
@@ -39,15 +38,15 @@
 
 First you need to install RobotFramework:
 
     pip install robotframework
 
 The latest stable version of library is available on PyPI:
 
-    pip install robotframework-reportportal
+    pip install robotframework-reportportal-updated
 
 [reportportal-client](https://github.com/reportportal/client-Python)
 and [six](https://pypi.org/project/six/) will be installed as dependencies
 
 **IMPORTANT!**
 The latest version **does not** support Report Portal versions below 5.0.0.
 
@@ -71,16 +70,16 @@
 
 For reporting results to Report Portal you need to pass some variables
 to `robot` run:
 
 REQUIRED:
 
 ```
---listener robotframework_reportportal.listener
---variable RP_UUID:"your_user_uuid"
+--listener robotframework_reportportal_updated.listener
+--variable RP_API_KEY:"your_user_api_key"
 --variable RP_ENDPOINT:"your_reportportal_url"
 --variable RP_LAUNCH:"launch_name"
 --variable RP_PROJECT:"reportportal_project_name"
 ```
 
 NOT REQUIRED:
```

### Comparing `robotframework-reportportal_updated-1.1.2/README.md` & `robotframework-reportportal_updated-1.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 First you need to install RobotFramework:
 
     pip install robotframework
 
 The latest stable version of library is available on PyPI:
 
-    pip install robotframework-reportportal
+    pip install robotframework-reportportal-updated
 
 [reportportal-client](https://github.com/reportportal/client-Python)
 and [six](https://pypi.org/project/six/) will be installed as dependencies
 
 **IMPORTANT!**
 The latest version **does not** support Report Portal versions below 5.0.0.
 
@@ -52,16 +52,16 @@
 
 For reporting results to Report Portal you need to pass some variables
 to `robot` run:
 
 REQUIRED:
 
 ```
---listener robotframework_reportportal.listener
---variable RP_UUID:"your_user_uuid"
+--listener robotframework_reportportal_updated.listener
+--variable RP_API_KEY:"your_user_api_key"
 --variable RP_ENDPOINT:"your_reportportal_url"
 --variable RP_LAUNCH:"launch_name"
 --variable RP_PROJECT:"reportportal_project_name"
 ```
 
 NOT REQUIRED:
```

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/__init__.py` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/__init__.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/exception.py` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/exception.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/listener.py` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/listener.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,72 +12,90 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
 import logging
 import os
+from functools import wraps
 from mimetypes import guess_type
+from typing import List, Optional, Dict, Union, Any
 
 from reportportal_client.helpers import gen_attributes
 
 from .exception import RobotServiceException
 from .model import Keyword, Launch, Test, LogMessage, Suite
 from .service import RobotService
 from .static import MAIN_SUITE_ID, PABOT_WIHOUT_LAUNCH_ID_MSG
 from .variables import Variables
 
 logger = logging.getLogger(__name__)
 
 
-class listener(object):
+def check_rp_enabled(func):
+    """Verify is RP is enabled in config."""
+    @wraps(func)
+    def wrap(*args, **kwargs):
+        if args and isinstance(args[0], listener):
+            if not args[0].service:
+                return
+        func(*args, **kwargs)
+    return wrap
+
+
+class listener:
     """Robot Framework listener interface for reporting to Report Portal."""
 
+    _items: List = ...
+    _service: Optional[RobotService] = ...
+    _variables: Optional[Variables] = ...
     ROBOT_LISTENER_API_VERSION = 2
 
-    def __init__(self):
+    def __init__(self) -> None:
         """Initialize listener attributes."""
         self._items = []
         self._service = None
         self._variables = None
 
-    def _build_msg_struct(self, message):
+    def _build_msg_struct(self, message: Dict) -> LogMessage:
         """Check if the given message comes from our custom logger or not.
 
         :param message: Message passed by the Robot Framework
         """
         if isinstance(message['message'], LogMessage):
             msg = message['message']
         else:
             msg = LogMessage(message['message'])
             msg.level = message['level']
         if not msg.launch_log:
             msg.item_id = getattr(self.current_item, 'rp_item_id', None)
         return msg
 
-    def _finish_current_item(self):
+    def _finish_current_item(self) -> Union[Keyword, Launch, Suite, Test]:
         """Remove the last item from the self._items list."""
         return self._items.pop()
 
     @property
-    def current_item(self):
+    def current_item(self) -> Optional[Union[Keyword, Launch, Suite, Test]]:
         """Get the last item from the self._items list."""
         if self._items:
             return self._items[-1]
 
-    def log_message(self, message):
+    @check_rp_enabled
+    def log_message(self, message: Dict) -> None:
         """Send log message to the Report Portal.
 
         :param message: Message passed by the Robot Framework
         """
         msg = self._build_msg_struct(message)
         logger.debug('ReportPortal - Log Message: {0}'.format(message))
         self.service.log(message=msg)
 
-    def log_message_with_image(self, msg, image):
+    @check_rp_enabled
+    def log_message_with_image(self, msg: Dict, image: str):
         """Send log message to the Report Portal.
 
         :param msg:   Message passed by the Robot Framework
         :param image: Path to image
         """
         mes = self._build_msg_struct(msg)
         with open(image, 'rb') as fh:
@@ -87,44 +105,45 @@
                 'mime': guess_type(image)[0] or 'application/octet-stream'
             }
         logger.debug('ReportPortal - Log Message with Image: {0} {1}'
                      .format(mes, image))
         self.service.log(message=mes)
 
     @property
-    def parent_id(self):
+    def parent_id(self) -> Optional[str]:
         """Get rp_item_id attribute of the current item."""
         return getattr(self.current_item, 'rp_item_id', None)
 
     @property
-    def service(self):
+    def service(self) -> RobotService:
         """Initialize instance of the RobotService."""
-        if self._service is None:
+        if self.variables.enabled and self._service is None:
             self._service = RobotService()
             self._service.init_service(
                 endpoint=self.variables.endpoint,
                 project=self.variables.project,
-                uuid=self.variables.uuid,
+                api_key=self.variables.api_key,
                 log_batch_size=self.variables.log_batch_size,
                 pool_size=self.variables.pool_size,
                 skipped_issue=self.variables.skipped_issue,
                 verify_ssl=self.variables.verify_ssl,
                 log_batch_payload_size=self.variables.log_batch_payload_size,
                 launch_id=self.variables.launch_id,
             )
         return self._service
 
     @property
-    def variables(self):
+    def variables(self) -> Variables:
         """Get instance of the variables.Variables class."""
         if not self._variables:
             self._variables = Variables()
         return self._variables
 
-    def start_launch(self, attributes, ts=None):
+    @check_rp_enabled
+    def start_launch(self, attributes: Dict, ts: Optional[Any] = None) -> None:
         """Start a new launch at the Report Portal.
 
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         launch = Launch(self.variables.launch_name, attributes)
         launch.attributes = gen_attributes(self.variables.launch_attributes)
@@ -139,15 +158,16 @@
                 mode=self.variables.mode,
                 ts=ts,
                 rerun=self.variables.rerun,
                 rerun_of=self.variables.rerun_of)
         else:
             self.service.rp.launch_id = self.variables.launch_id
 
-    def start_suite(self, name, attributes, ts=None):
+    @check_rp_enabled
+    def start_suite(self, name: str, attributes: Dict, ts: Optional[Any] = None) -> None:
         """Start a new test suite at the Report Portal.
 
         :param name:       Test suite name
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         if attributes['id'] == MAIN_SUITE_ID:
@@ -163,15 +183,16 @@
         else:
             logger.debug('ReportPortal - Start Suite: {0}'.format(attributes))
             suite = Suite(name, attributes)
             suite.rp_parent_item_id = self.parent_id
             suite.rp_item_id = self.service.start_suite(suite=suite, ts=ts)
             self._items.append(suite)
 
-    def end_suite(self, _, attributes, ts=None):
+    @check_rp_enabled
+    def end_suite(self, _: Optional[str], attributes: Dict, ts: Optional[Any] = None) -> None:
         """Finish started test suite at the Report Portal.
 
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         if attributes['id'] == MAIN_SUITE_ID:
             suite = self._finish_current_item().update(attributes)
@@ -184,15 +205,16 @@
             self.service.finish_launch(launch=launch, ts=ts)
         else:
             suite = self._finish_current_item().update(attributes)
             logger.debug(
                 'ReportPortal - End Suite: {0}'.format(suite.attributes))
             self.service.finish_suite(suite=suite, ts=ts)
 
-    def start_test(self, name, attributes, ts=None):
+    @check_rp_enabled
+    def start_test(self, name: str, attributes: Dict, ts: Optional[Any] = None) -> None:
         """Start a new test case at the Report Portal.
 
         :param name:       Test case name
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         if 'source' not in attributes:
@@ -203,15 +225,16 @@
         logger.debug('ReportPortal - Start Test: {0}'.format(attributes))
         test.attributes = gen_attributes(
             self.variables.test_attributes + test.tags)
         test.rp_parent_item_id = self.parent_id
         test.rp_item_id = self.service.start_test(test=test, ts=ts)
         self._items.append(test)
 
-    def end_test(self, _, attributes, ts=None):
+    @check_rp_enabled
+    def end_test(self, _: Optional[str], attributes: Dict, ts: Optional[Any] = None) -> None:
         """Finish started test case at the Report Portal.
 
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         test = self.current_item.update(attributes)
         test.attributes = gen_attributes(
@@ -220,61 +243,64 @@
             test.status = 'SKIP'
         if test.message:
             self.log_message({'message': test.message, 'level': 'DEBUG'})
         logger.debug('ReportPortal - End Test: {0}'.format(test.attributes))
         self._finish_current_item()
         self.service.finish_test(test=test, ts=ts)
 
-    def start_keyword(self, name, attributes, ts=None):
+    @check_rp_enabled
+    def start_keyword(self, name: str, attributes: Dict, ts: Optional[Any] = None) -> None:
         """Start a new keyword(test step) at the Report Portal.
 
         :param name:       Keyword name
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         kwd = Keyword(name=name, parent_type=self.current_item.type,
                       attributes=attributes)
         kwd.rp_parent_item_id = self.parent_id
         logger.debug('ReportPortal - Start Keyword: {0}'.format(attributes))
         kwd.rp_item_id = self.service.start_keyword(keyword=kwd, ts=ts)
         self._items.append(kwd)
 
-    def end_keyword(self, _, attributes, ts=None):
+    @check_rp_enabled
+    def end_keyword(self, _: Optional[str], attributes: Dict, ts: Optional[Any] = None) -> None:
         """Finish started keyword at the Report Portal.
 
         :param attributes: Dictionary passed by the Robot Framework
         :param ts:         Timestamp(used by the ResultVisitor)
         """
         kwd = self._finish_current_item().update(attributes)
         logger.debug('ReportPortal - End Keyword: {0}'.format(kwd.attributes))
         self.service.finish_keyword(keyword=kwd, ts=ts)
 
-    def log_file(self, log_path):
+    def log_file(self, log_path: str) -> None:
         """Attach HTML log file created by Robot Framework to RP launch.
 
         :param log_path: Path to the log file
         """
         if self.variables.attach_log:
             message = {'message': 'Execution log', 'level': 'INFO'}
             self.log_message_with_image(message, log_path)
 
-    def report_file(self, report_path):
+    def report_file(self, report_path: str) -> None:
         """Attach HTML report created by Robot Framework to RP launch.
 
         :param report_path: Path to the report file
         """
         if self.variables.attach_report:
             message = {'message': 'Execution report', 'level': 'INFO'}
             self.log_message_with_image(message, report_path)
 
-    def xunit_file(self, xunit_path):
+    def xunit_file(self, xunit_path: str) -> None:
         """Attach XUnit file created by Robot Framework to RP launch.
 
         :param xunit_path: Path to the XUnit file
         """
         if self.variables.attach_xunit:
             message = {'message': 'XUnit result file', 'level': 'INFO'}
             self.log_message_with_image(message, xunit_path)
 
-    def close(self):
+    @check_rp_enabled
+    def close(self) -> None:
         """Call service terminate when the whole test execution is done."""
         self.service.terminate_service()
```

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/listener.pyi` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/listener.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/logger.py` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/logger.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/model.py` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/model.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/model.pyi` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/model.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/post_report.py` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/post_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 This will allow all the test results to be sent to ReportPortal, after the
 test is run. By doing this, we will not disturb the timing when the test is
 run. It also has the benefit of using the test result generated after running
 multiple parallel robot testing (eg. by using pabot).
 
 Command-line usage:
 
-    post_report --variable RP_UUID:"your_user_uuid"
+    post_report --variable RP_API_KEY:"your_user_api_key"
                 --variable RP_ENDPOINT:"your_reportportal_url"
                 --variable RP_PROJECT:"reportportal_project_name"
                 [--variable RP_LAUNCH:"launch_name"]
                 [--variable RP_LAUNCH_DOC:"some_documentation_for_launch"]
                 [--variable RP_LAUNCH_ATTRIBUTES:"RF tag_name:tag_value"]
                 [--variable RP_TEST_ATTRIBUTES:"Long"]
                 [--variable RP_LOG_BATCH_SIZE:"10"]
```

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/result_visitor.py` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/result_visitor.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/result_visitor.pyi` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/result_visitor.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/service.py` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,44 +66,44 @@
         """
         attributes = cmd_attrs or []
         system_attributes = get_launch_sys_attrs()
         system_attributes['agent'] = (
             '{}|{}'.format(self.agent_name, self.agent_version))
         return attributes + dict_to_payload(system_attributes)
 
-    def init_service(self, endpoint, project, uuid, log_batch_size, pool_size,
-                     skipped_issue=True, verify_ssl=True,
+    def init_service(self, endpoint, project, api_key, log_batch_size,
+                     pool_size, skipped_issue=True, verify_ssl=True,
                      log_batch_payload_size=MAX_LOG_BATCH_PAYLOAD_SIZE,
                      launch_id=None):
         """Initialize common Report Portal client.
 
         :param endpoint:               Report Portal API endpoint
         :param project:                Report Portal project
-        :param uuid:                   API token
+        :param api_key:                API key
         :param log_batch_size:         Number of logs to be sent within one
                                        batch
         :param pool_size:              HTTPAdapter max pool size
         :param skipped_issue:          Mark skipped test items with
                                        'To Investigate', default value 'True'
         :param verify_ssl:             Disable SSL verification.
         :param log_batch_payload_size: Maximum size of logs to be sent within
                                        one batch
         :param launch_id:              a launch id to use instead of starting
                                        own one
         """
         if self.rp is None:
             logger.debug(
                 'ReportPortal - Init service: '
-                'endpoint={0}, project={1}, uuid={2}'
-                .format(endpoint, project, uuid))
+                'endpoint={0}, project={1}, api_key={2}'
+                .format(endpoint, project, api_key))
             self.launch_id = launch_id
             self.rp = RPClient(
                 endpoint=endpoint,
                 project=project,
-                token=uuid,
+                api_key=api_key,
                 is_skipped_an_issue=skipped_issue,
                 log_batch_size=log_batch_size,
                 retries=True,
                 verify_ssl=verify_ssl,
                 max_pool_size=pool_size,
                 log_batch_payload_size=log_batch_payload_size,
                 launch_id=launch_id
```

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/service.pyi` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/service.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     agent_version: Text = ...
     rp: Optional[RPClient] = ...
 
     def __init__(self) -> None: ...
 
     def _get_launch_attributes(self, cmd_attrs: List) -> List: ...
 
-    def init_service(self, endpoint: Text, project: Text, uuid: Text,
+    def init_service(self, endpoint: Text, project: Text, api_key: Text,
                      log_batch_size: int, pool_size: int, skipped_issue: bool,
                      verify_ssl: Union[Text, bool],
                      log_batch_payload_size: int, launch_id: str) -> None: ...
 
     def terminate_service(self) -> None: ...
 
     def start_launch(self, launch: Launch, mode: Optional[Text] = ...,
```

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/static.py` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/static.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/static.pyi` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/static.pyi`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/time_visitor.py` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/time_visitor.py`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated/variables.pyi` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated/variables.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -17,20 +17,21 @@
 
 
 def get_variable(name: Text, default: Optional[Text] = ...) -> Optional[
     Text]: ...
 
 
 class Variables:
-    _endpoint: Optional[Text] = ...
-    _launch_name: Optional[Text] = ...
+    enabled: bool = ...
+    endpoint: Optional[Text] = ...
+    launch_name: Optional[Text] = ...
     _pabot_pool_id: Optional[int] = ...
     _pabot_used: Optional[Text] = ...
-    _project: Optional[Text] = ...
-    _uuid: Optional[Text] = ...
+    project: Optional[Text] = ...
+    api_key: Optional[Text] = ...
     attach_log: bool = ...
     attach_report: bool = ...
     attach_xunit: bool = ...
     launch_attributes: List = ...
     launch_id: Optional[Text] = ...
     launch_doc: Optional[Text] = ...
     log_batch_size: Optional[int] = ...
@@ -41,26 +42,14 @@
     test_attributes: Optional[List] = ...
     skipped_issue: bool = ...
     log_batch_payload_size: int = ...
 
     def __init__(self) -> None: ...
 
     @property
-    def endpoint(self) -> Text: ...
-
-    @property
-    def launch_name(self) -> Text: ...
-
-    @property
     def pabot_pool_id(self) -> int: ...
 
     @property
     def pabot_used(self) -> Optional[Text]: ...
 
     @property
-    def project(self) -> Text: ...
-
-    @property
-    def uuid(self) -> Text: ...
-
-    @property
     def verify_ssl(self) -> Union[bool, Text]: ...
```

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated.egg-info/PKG-INFO` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: robotframework-reportportal-updated
-Version: 1.1.2
+Version: 1.1.3
 Summary: Agent for reporting RobotFramework test results to Report Portal
 Home-page: https://github.com/reportportal/agent-Python-RobotFramework
-Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.1.2
+Download-URL: https://github.com/reportportal/agent-Python-RobotFramework/tarball/1.1.3
 Author: Report Portal Team
 Author-email: support@reportportal.io
 Keywords: testing,reporting,robot framework,reportportal,agent
 Classifier: Framework :: Robot Framework
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ReportPortal RobotFramework agent
 
 [![PyPI](https://img.shields.io/pypi/v/robotframework-reportportal.svg?maxAge=259200)](https://pypi.python.org/pypi/robotframework-reportportal)
 [![Python versions](https://img.shields.io/pypi/pyversions/robotframework-reportportal.svg)](https://pypi.org/project/robotframework-reportportal)
@@ -39,15 +38,15 @@
 
 First you need to install RobotFramework:
 
     pip install robotframework
 
 The latest stable version of library is available on PyPI:
 
-    pip install robotframework-reportportal
+    pip install robotframework-reportportal-updated
 
 [reportportal-client](https://github.com/reportportal/client-Python)
 and [six](https://pypi.org/project/six/) will be installed as dependencies
 
 **IMPORTANT!**
 The latest version **does not** support Report Portal versions below 5.0.0.
 
@@ -71,16 +70,16 @@
 
 For reporting results to Report Portal you need to pass some variables
 to `robot` run:
 
 REQUIRED:
 
 ```
---listener robotframework_reportportal.listener
---variable RP_UUID:"your_user_uuid"
+--listener robotframework_reportportal_updated.listener
+--variable RP_API_KEY:"your_user_api_key"
 --variable RP_ENDPOINT:"your_reportportal_url"
 --variable RP_LAUNCH:"launch_name"
 --variable RP_PROJECT:"reportportal_project_name"
 ```
 
 NOT REQUIRED:
```

### Comparing `robotframework-reportportal_updated-1.1.2/robotframework_reportportal_updated.egg-info/SOURCES.txt` & `robotframework-reportportal_updated-1.1.3/robotframework_reportportal_updated.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-reportportal_updated-1.1.2/setup.py` & `robotframework-reportportal_updated-1.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Setup instructions for the package."""
 
 import os
-from setuptools import setup, find_packages
 
+from setuptools import setup, find_packages
 
-__version__ = '1.1.2'
+__version__ = '1.1.3'
 
 
 def read_file(fname):
     """Read the given file.
 
     :param fname: Name of the file to be read
     :return:      Output of the given file
@@ -32,20 +32,19 @@
     download_url=(
         'https://github.com/reportportal/agent-Python-RobotFramework/'
         'tarball/{version}'.format(version=__version__)),
     keywords=['testing', 'reporting', 'robot framework', 'reportportal',
               'agent'],
     classifiers=[
         'Framework :: Robot Framework',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         ],
     install_requires=read_file('requirements.txt').splitlines(),
     entry_points={
         'console_scripts': [
             'post_report=robotframework_reportportal_updated.post_report:main'
         ]
     },
```

