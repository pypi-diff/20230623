# Comparing `tmp/pynautobot-1.4.0.tar.gz` & `tmp/pynautobot-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynautobot-1.4.0.tar", max compression
+gzip compressed data, was "pynautobot-1.5.0.tar", max compression
```

## Comparing `pynautobot-1.4.0.tar` & `pynautobot-1.5.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     9612 2023-02-14 15:14:53.723211 pynautobot-1.4.0/LICENSE
--rw-r--r--   0        0        0     4873 2023-02-14 15:14:53.723211 pynautobot-1.4.0/README.md
--rw-r--r--   0        0        0      414 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/__init__.py
--rw-r--r--   0        0        0       59 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/core/__init__.py
--rw-r--r--   0        0        0     6308 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/core/api.py
--rw-r--r--   0        0        0     5307 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/core/app.py
--rw-r--r--   0        0        0    18593 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/core/endpoint.py
--rw-r--r--   0        0        0     5024 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/core/graphql.py
--rw-r--r--   0        0        0    14255 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/core/query.py
--rw-r--r--   0        0        0    14073 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/core/response.py
--rw-r--r--   0        0        0      148 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/core/util.py
--rw-r--r--   0        0        0       59 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/models/__init__.py
--rw-r--r--   0        0        0      814 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/models/circuits.py
--rw-r--r--   0        0        0     6145 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/models/dcim.py
--rw-r--r--   0        0        0     1212 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/models/extras.py
--rw-r--r--   0        0        0     2919 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/models/ipam.py
--rw-r--r--   0        0        0      724 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/models/users.py
--rw-r--r--   0        0        0      725 2023-02-14 15:14:53.727212 pynautobot-1.4.0/pynautobot/models/virtualization.py
--rw-r--r--   0        0        0     2168 2023-02-14 15:15:03.091409 pynautobot-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     5749 1970-01-01 00:00:00.000000 pynautobot-1.4.0/setup.py
--rw-r--r--   0        0        0     5927 1970-01-01 00:00:00.000000 pynautobot-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     9612 2023-06-23 21:16:51.681035 pynautobot-1.5.0/LICENSE
+-rw-r--r--   0        0        0     4873 2023-06-23 21:16:51.681035 pynautobot-1.5.0/README.md
+-rw-r--r--   0        0        0      414 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/__init__.py
+-rw-r--r--   0        0        0       59 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/core/__init__.py
+-rw-r--r--   0        0        0     6308 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/core/api.py
+-rw-r--r--   0        0        0     5317 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/core/app.py
+-rw-r--r--   0        0        0    19995 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/core/endpoint.py
+-rw-r--r--   0        0        0     5024 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/core/graphql.py
+-rw-r--r--   0        0        0    14255 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/core/query.py
+-rw-r--r--   0        0        0    14279 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/core/response.py
+-rw-r--r--   0        0        0      148 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/core/util.py
+-rw-r--r--   0        0        0       59 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/models/__init__.py
+-rw-r--r--   0        0        0      814 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/models/circuits.py
+-rw-r--r--   0        0        0     6143 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/models/dcim.py
+-rw-r--r--   0        0        0     1212 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/models/extras.py
+-rw-r--r--   0        0        0     2919 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/models/ipam.py
+-rw-r--r--   0        0        0      724 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/models/users.py
+-rw-r--r--   0        0        0      724 2023-06-23 21:16:51.685035 pynautobot-1.5.0/pynautobot/models/virtualization.py
+-rw-r--r--   0        0        0     2249 2023-06-23 21:17:03.629088 pynautobot-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     5919 1970-01-01 00:00:00.000000 pynautobot-1.5.0/PKG-INFO
```

### Comparing `pynautobot-1.4.0/LICENSE` & `pynautobot-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynautobot-1.4.0/README.md` & `pynautobot-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pynautobot-1.4.0/pynautobot/core/api.py` & `pynautobot-1.5.0/pynautobot/core/api.py`

 * *Files identical despite different names*

### Comparing `pynautobot-1.4.0/pynautobot/core/app.py` & `pynautobot-1.5.0/pynautobot/core/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
 
     """
 
     def __init__(self, api):
         self.api = api
 
     def __getattr__(self, name):
-        return App(self.api, "plugins/{}".format(name))
+        return App(self.api, f"plugins/{name.replace('_', '-')}")
 
     def installed_plugins(self):
         """Returns raw response with installed plugins
 
         :returns: Raw response Nautobot's installed plugins.
         :Example:
```

### Comparing `pynautobot-1.4.0/pynautobot/core/endpoint.py` & `pynautobot-1.5.0/pynautobot/core/endpoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 
 This file has been modified by NetworktoCode, LLC.
 """
+from typing import Dict
 from pynautobot.core.query import Request, RequestError
 from pynautobot.core.response import Record
 
 RESERVED_KWARGS = ("pk", "limit", "offset")
 
 
 def response_loader(req, return_obj, endpoint):
@@ -303,14 +304,51 @@
             token=self.token,
             http_session=self.api.http_session,
             api_version=api_version,
         ).post(args[0] if args else kwargs)
 
         return response_loader(req, self.return_obj, self)
 
+    def update(self, id: str, data: Dict[str, any]):
+        """
+        Update a resource with a dictionary.
+
+        Accepts the id of the object that needs to be updated as well as
+        a dictionary of k/v pairs used to update an object. The object
+        is directly updated on the server using a PATCH request without
+        fetching object information.
+
+        For fields requiring an object reference (such as a device location),
+        the API user is responsible for providing the object ID or the object
+        URL. This API will not accept the pynautobot object directly.
+
+        :arg str id: Identifier of the object being updated
+        :arg dict data: Dictionary containing the k/v to update the
+            record object with.
+        :returns: True if PATCH request was successful.
+        :example:
+
+        >>> nb.dcim.devices.update(id="0238a4e3-66f2-455a-831f-5f177215de0f", data={
+        ...     "name": "test-switch2",
+        ...     "serial": "ABC321",
+        ...     "location": "9b1f53c7-89fa-4fb2-a89a-b97364fef50c",
+        ... })
+        True
+        """
+        req = Request(
+            key=id,
+            base=self.url,
+            token=self.api.token,
+            http_session=self.api.http_session,
+            api_version=self.api.api_version,
+        )
+        if req.patch(data):
+            return True
+        return False
+
     def choices(self, api_version=None):
         """Returns all choices from the endpoint.
 
         The returned dict is also saved in the endpoint object (in
         ``_choices`` attribute) so that later calls will return the same data
         without recurring requests to Nautobot. When using ``.choices()`` in
         long-running applications, consider restarting them whenever Nautobot is
```

### Comparing `pynautobot-1.4.0/pynautobot/core/graphql.py` & `pynautobot-1.5.0/pynautobot/core/graphql.py`

 * *Files identical despite different names*

### Comparing `pynautobot-1.4.0/pynautobot/core/query.py` & `pynautobot-1.5.0/pynautobot/core/query.py`

 * *Files identical despite different names*

### Comparing `pynautobot-1.4.0/pynautobot/core/response.py` & `pynautobot-1.5.0/pynautobot/core/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,19 +75,20 @@
     object's attributes. If a missing attr is requested
     (e.g. requesting a field that's only present on a full response on
     a Record made from a nested response) the pynautobot will make a
     request for the full object and return the requsted value.
 
     :examples:
 
-    Default representation of the object is usually its name
+    Default representation of the object usually contains object's
+    class, object's name and it's location in memory
 
     >>> x = nb.dcim.devices.get(1)
     >>> x
-    test1-switch1
+    <pynautobot.models.dcim.Devices ('test1-switch1') at 0x1953d821250>
     >>>
 
     Querying a string field.
 
     >>> x = nb.dcim.devices.get(1)
     >>> x.serial
     'ABC123'
@@ -201,15 +202,15 @@
     def __getitem__(self, k):
         return dict(self)[k]
 
     def __str__(self):
         return getattr(self, "display", None) or getattr(self, "name", None) or getattr(self, "label", None) or ""
 
     def __repr__(self):
-        return str(self)
+        return "<{}.{} ('{}') at {}>".format(self.__class__.__module__, self.__class__.__name__, self, hex(id(self)))
 
     def __getstate__(self):
         return self.__dict__
 
     def __setstate__(self, d):
         self.__dict__.update(d)
```

### Comparing `pynautobot-1.4.0/pynautobot/models/circuits.py` & `pynautobot-1.5.0/pynautobot/models/circuits.py`

 * *Files identical despite different names*

### Comparing `pynautobot-1.4.0/pynautobot/models/dcim.py` & `pynautobot-1.5.0/pynautobot/models/dcim.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         uri_to_obj_class_map = {
             "dcim/cables": Cables,
             "dcim/front-ports": FrontPorts,
             "dcim/interfaces": Interfaces,
             "dcim/rear-ports": RearPorts,
         }
         ret = []
-        for (termination_a_data, cable_data, termination_b_data) in req.get():
+        for termination_a_data, cable_data, termination_b_data in req.get():
             this_hop_ret = []
             for hop_item_data in (termination_a_data, cable_data, termination_b_data):
                 # if not fully terminated then some items will be None
                 if not hop_item_data:
                     this_hop_ret.append(hop_item_data)
                     continue
```

### Comparing `pynautobot-1.4.0/pynautobot/models/extras.py` & `pynautobot-1.5.0/pynautobot/models/extras.py`

 * *Files identical despite different names*

### Comparing `pynautobot-1.4.0/pynautobot/models/ipam.py` & `pynautobot-1.5.0/pynautobot/models/ipam.py`

 * *Files identical despite different names*

### Comparing `pynautobot-1.4.0/pynautobot/models/users.py` & `pynautobot-1.5.0/pynautobot/models/users.py`

 * *Files identical despite different names*

### Comparing `pynautobot-1.4.0/pynautobot/models/virtualization.py` & `pynautobot-1.5.0/pynautobot/models/virtualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,9 +15,8 @@
 
 This file has been modified by NetworktoCode, LLC.
 """
 from pynautobot.core.response import Record, JsonField
 
 
 class VirtualMachines(Record):
-
     config_context = JsonField
```

### Comparing `pynautobot-1.4.0/pyproject.toml` & `pynautobot-1.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file has been modified by NetworktoCode, LLC.
 
 [tool.poetry]
 name = "pynautobot"
-version = "v1.4.0"
+version = "v1.5.0"
 description = "Nautobot API client library"
 authors = ["Network to Code, LLC <opensource@networktocode.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Nautobot"]
 classifiers = [
   "Intended Audience :: Developers",
@@ -16,19 +16,20 @@
 ]
 repository = "https://github.com/nautobot/pynautobot"
 homepage = "https://nautobot.com"
 documentation = "https://pynautobot.readthedocs.io"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-requests = "^2.20.0"
+requests = "^2.30.0"
+# requests doesn't support `urllib3` 2.0 yet see: https://github.com/psf/requests/issues/6432
+urllib3 = ">=1.21.1 <1.27"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
-pytest-docker = "*"
 requests_mock = "*"
 pyyaml = "*"
 pylint = "*"
 pydocstyle = "*"
 yamllint = "*"
 invoke = "*"
 toml = "*"
@@ -86,8 +87,7 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = "tests/"
 addopts = "-vv"
-python_paths = "./"
```

### Comparing `pynautobot-1.4.0/setup.py` & `pynautobot-1.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,200 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pynautobot
+Version: 1.5.0
+Summary: Nautobot API client library
+Home-page: https://nautobot.com
+License: Apache-2.0
+Keywords: Nautobot
+Author: Network to Code, LLC
+Author-email: opensource@networktocode.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.6
+Provides-Extra: docs
+Requires-Dist: requests (>=2.30.0,<3.0.0)
+Requires-Dist: urllib3 (>=1.21.1,<1.27)
+Project-URL: Documentation, https://pynautobot.readthedocs.io
+Project-URL: Repository, https://github.com/nautobot/pynautobot
+Description-Content-Type: text/markdown
+
+![pynautobot](docs/nautobot_logo.svg "Nautobot logo")
+
+# Pynautobot
+
+Python API client library for [Nautobot](https://github.com/nautobot/nautobot).
+
+> Pynautobot was initially developed as a fork of [pynetbox](https://github.com/digitalocean/pynetbox/).
+> Pynetbox was originally developed by Zach Moody at DigitalOcean and the NetBox Community.
+
+The complete documentation for pynautobot can be found at [Read the Docs](https://pynautobot.readthedocs.io/en/stable/).
+
+Questions? Comments? Join us in the **#nautobot** Slack channel on [Network to Code](https://networktocode.slack.com)!
+
+## Installation
+
+You can install via [pip](#using-pip) or [poetry](#using-poetry)
+
+### Using pip
+
+```shell
+$ pip install pynautobot
+...
+```
+
+### Using poetry
+
+```shell
+$ git clone https://github.com/nautobot/pynautobot.git
+...
+$ pip install poetry
+...
+$ poetry shell
+Virtual environment already activated: /home/user/pynautobot/.venv
+$ poetry install
+...
+```
+
+## Quick Start
+
+A short introduction is provided here; the full documention for pynautobot is at [Read the Docs](http://pynautobot.readthedocs.io/).
+
+To begin, import pynautobot and instantiate an `Api` object, passing the `url` and `token`.
+
+```python
+import pynautobot
+nautobot = pynautobot.api(
+    url="http://localhost:8000",
+    token="d6f4e314a5b5fefd164995169f28ae32d987704f",
+)
+```
+
+The Api object provides access to the Apps in Nautobot.
+The Apps provide access to the Models and the field data stored in Nautobot.
+Pynautobot uses the `Endpoint` class to represent Models.
+For example, here is how to access **Devices** stored in Nautobot:
+
+```python
+devices = nautobot.dcim.devices
+devices
+<pynautobot.core.endpoint.Endpoint object at 0x7fe801e62fa0>
+```
+
+## Jobs
+
+Pynautobot provides a specialized `Endpoint` class to represent the Jobs model. This class is called `JobsEndpoint`.
+This extends the `Endpoint` class by adding the `run` method so pynautobot can be used to call/execute a job run.
+
+1. Run from a instance of a job.
+
+```python
+>>> gc_backup_job = nautobot.extras.jobs.all()[14]
+>>> job_result = gc_backup_job.run()
+>>> job_result.result.id
+'1838f8bd-440f-434e-9f29-82b46549a31d' # <-- Job Result ID.
+```
+
+2. Run with Job Inputs
+
+```python
+job = nautobot.extras.jobs.all()[7]
+job.run(data={"hostname_regex": ".*"})
+```
+
+3. Run by providing the job id
+
+```python
+>>> gc_backup_job = nautobot.extras.jobs.run(class_path=nautobot.extras.jobs.all()[14].id)
+>>> gc_backup_job.result.id
+'548832dc-e586-4c65-a7c1-a4e799398a3b' # <-- Job Result ID.
+```
+
+## Queries
+
+Pynautobot provides several ways to retrieve objects from Nautobot.
+Only the `get()` method is show here.
+To continue from the example above, the `Endpoint` object returned will be used to `get`
+the device named _hq-access-01_.
+
+```python
+switch = devices.get(nam="hq-access-01")
+```
+
+The object returned from the `get()` method is an implementation of the `Record` class.
+This object provides access to the field data from Nautobot.
+
+```python
+switch.id
+'6929b68d-8f87-4470-8377-e7fdc933a2bb'
+switch.name
+'hq-access-01'
+switch.site
+hq
+```
+
+### Threading
+
+Pynautobot supports multithreaded calls for `.filter()` and `.all()` queries. It is **highly recommended** you have `MAX_PAGE_SIZE` in your Nautobot install set to anything _except_ `0` or `None`. The default value of `1000` is usually a good value to use. To enable threading, add `threading=True` parameter when instantiating the `Api` object:
+
+```python
+nautobot = pynautobot.api(
+    url="http://localhost:8000",
+    token="d6f4e314a5b5fefd164995169f28ae32d987704f",
+    threading=True,
+)
+```
+
+### Versioning
+
+Used for Nautobot Rest API versioning. Versioning can be controlled globally by setting `api_version` on initialization of the `API` class and/or for a specific request e.g (`list()`, `get()`, `create()` etc.) by setting an optional `api_version` parameter.
+
+**Global versioning**
+
+```python
+import pynautobot
+nautobot = pynautobot.api(
+    url="http://localhost:8000",
+    token="d6f4e314a5b5fefd164995169f28ae32d987704f",
+    api_version="1.3"
+)
+```
+
+**Request specific versioning**
+
+```python
+import pynautobot
+nautobot = pynautobot.api(
+  url="http://localhost:8000", token="d6f4e314a5b5fefd164995169f28ae32d987704f",
+)
+tags = nautobot.extras.tags
+tags.create(name="Tag", slug="tag", api_version="1.2",)
+tags.list(api_version="1.3",)
+```
+
+### Retry logic
+
+By default, the client will not retry any operation. This behavior can be adjusted via the `retries` optional parameters. This will only affect for HTTP codes: 429, 500, 502, 503 and 504.
+
+**Retries**
+
+```python
+import pynautobot
+nautobot = pynautobot.api(
+    url="http://localhost:8000",
+    token="d6f4e314a5b5fefd164995169f28ae32d987704f",
+    retries=3
+)
+```
 
-packages = \
-['pynautobot', 'pynautobot.core', 'pynautobot.models']
+## Related projects
 
-package_data = \
-{'': ['*']}
+Please see [our wiki](https://github.com/nautobot/nautobot/wiki/Related-Projects)
+for a list of relevant community projects.
 
-install_requires = \
-['requests>=2.20.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'pynautobot',
-    'version': '1.4.0',
-    'description': 'Nautobot API client library',
-    'long_description': '![pynautobot](docs/nautobot_logo.svg "Nautobot logo")\n\n# Pynautobot\n\nPython API client library for [Nautobot](https://github.com/nautobot/nautobot).\n\n> Pynautobot was initially developed as a fork of [pynetbox](https://github.com/digitalocean/pynetbox/).\n> Pynetbox was originally developed by Zach Moody at DigitalOcean and the NetBox Community.\n\nThe complete documentation for pynautobot can be found at [Read the Docs](https://pynautobot.readthedocs.io/en/stable/).\n\nQuestions? Comments? Join us in the **#nautobot** Slack channel on [Network to Code](https://networktocode.slack.com)!\n\n## Installation\n\nYou can install via [pip](#using-pip) or [poetry](#using-poetry)\n\n### Using pip\n\n```shell\n$ pip install pynautobot\n...\n```\n\n### Using poetry\n\n```shell\n$ git clone https://github.com/nautobot/pynautobot.git\n...\n$ pip install poetry\n...\n$ poetry shell\nVirtual environment already activated: /home/user/pynautobot/.venv\n$ poetry install\n...\n```\n\n## Quick Start\n\nA short introduction is provided here; the full documention for pynautobot is at [Read the Docs](http://pynautobot.readthedocs.io/).\n\nTo begin, import pynautobot and instantiate an `Api` object, passing the `url` and `token`.\n\n```python\nimport pynautobot\nnautobot = pynautobot.api(\n    url="http://localhost:8000",\n    token="d6f4e314a5b5fefd164995169f28ae32d987704f",\n)\n```\n\nThe Api object provides access to the Apps in Nautobot.\nThe Apps provide access to the Models and the field data stored in Nautobot.\nPynautobot uses the `Endpoint` class to represent Models.\nFor example, here is how to access **Devices** stored in Nautobot:\n\n```python\ndevices = nautobot.dcim.devices\ndevices\n<pynautobot.core.endpoint.Endpoint object at 0x7fe801e62fa0>\n```\n\n## Jobs\n\nPynautobot provides a specialized `Endpoint` class to represent the Jobs model. This class is called `JobsEndpoint`.\nThis extends the `Endpoint` class by adding the `run` method so pynautobot can be used to call/execute a job run.\n\n1. Run from a instance of a job.\n\n```python\n>>> gc_backup_job = nautobot.extras.jobs.all()[14]\n>>> job_result = gc_backup_job.run()\n>>> job_result.result.id\n\'1838f8bd-440f-434e-9f29-82b46549a31d\' # <-- Job Result ID.\n```\n\n2. Run with Job Inputs\n\n```python\njob = nautobot.extras.jobs.all()[7]\njob.run(data={"hostname_regex": ".*"})\n```\n\n3. Run by providing the job id\n\n```python\n>>> gc_backup_job = nautobot.extras.jobs.run(class_path=nautobot.extras.jobs.all()[14].id)\n>>> gc_backup_job.result.id\n\'548832dc-e586-4c65-a7c1-a4e799398a3b\' # <-- Job Result ID.\n```\n\n## Queries\n\nPynautobot provides several ways to retrieve objects from Nautobot.\nOnly the `get()` method is show here.\nTo continue from the example above, the `Endpoint` object returned will be used to `get`\nthe device named _hq-access-01_.\n\n```python\nswitch = devices.get(nam="hq-access-01")\n```\n\nThe object returned from the `get()` method is an implementation of the `Record` class.\nThis object provides access to the field data from Nautobot.\n\n```python\nswitch.id\n\'6929b68d-8f87-4470-8377-e7fdc933a2bb\'\nswitch.name\n\'hq-access-01\'\nswitch.site\nhq\n```\n\n### Threading\n\nPynautobot supports multithreaded calls for `.filter()` and `.all()` queries. It is **highly recommended** you have `MAX_PAGE_SIZE` in your Nautobot install set to anything _except_ `0` or `None`. The default value of `1000` is usually a good value to use. To enable threading, add `threading=True` parameter when instantiating the `Api` object:\n\n```python\nnautobot = pynautobot.api(\n    url="http://localhost:8000",\n    token="d6f4e314a5b5fefd164995169f28ae32d987704f",\n    threading=True,\n)\n```\n\n### Versioning\n\nUsed for Nautobot Rest API versioning. Versioning can be controlled globally by setting `api_version` on initialization of the `API` class and/or for a specific request e.g (`list()`, `get()`, `create()` etc.) by setting an optional `api_version` parameter.\n\n**Global versioning**\n\n```python\nimport pynautobot\nnautobot = pynautobot.api(\n    url="http://localhost:8000",\n    token="d6f4e314a5b5fefd164995169f28ae32d987704f",\n    api_version="1.3"\n)\n```\n\n**Request specific versioning**\n\n```python\nimport pynautobot\nnautobot = pynautobot.api(\n  url="http://localhost:8000", token="d6f4e314a5b5fefd164995169f28ae32d987704f",\n)\ntags = nautobot.extras.tags\ntags.create(name="Tag", slug="tag", api_version="1.2",)\ntags.list(api_version="1.3",)\n```\n\n### Retry logic\n\nBy default, the client will not retry any operation. This behavior can be adjusted via the `retries` optional parameters. This will only affect for HTTP codes: 429, 500, 502, 503 and 504.\n\n**Retries**\n\n```python\nimport pynautobot\nnautobot = pynautobot.api(\n    url="http://localhost:8000",\n    token="d6f4e314a5b5fefd164995169f28ae32d987704f",\n    retries=3\n)\n```\n\n## Related projects\n\nPlease see [our wiki](https://github.com/nautobot/nautobot/wiki/Related-Projects)\nfor a list of relevant community projects.\n',
-    'author': 'Network to Code, LLC',
-    'author_email': 'opensource@networktocode.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://nautobot.com',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

