# Comparing `tmp/braintrust-0.0.5.tar.gz` & `tmp/braintrust-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braintrust-0.0.5.tar", last modified: Sat Jun 17 20:20:38 2023, max compression
+gzip compressed data, was "braintrust-0.0.6.tar", last modified: Thu Jun 22 22:13:35 2023, max compression
```

## Comparing `braintrust-0.0.5.tar` & `braintrust-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-17 20:20:38.555220 braintrust-0.0.5/
--rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-17 20:20:38.555093 braintrust-0.0.5/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.5/README.md
--rw-r--r--   0 ankur      (501) staff       (20)       38 2023-06-17 20:20:38.555256 braintrust-0.0.5/setup.cfg
--rw-r--r--   0 ankur      (501) staff       (20)     1623 2023-06-17 20:17:20.000000 braintrust-0.0.5/setup.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-17 20:20:38.552139 braintrust-0.0.5/src/
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-17 20:20:38.553587 braintrust-0.0.5/src/braintrust/
--rw-r--r--   0 ankur      (501) staff       (20)    17955 2023-06-17 20:19:20.000000 braintrust-0.0.5/src/braintrust/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)      123 2023-05-14 19:33:59.000000 braintrust-0.0.5/src/braintrust/cache.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-17 20:20:38.554586 braintrust-0.0.5/src/braintrust/cli/
--rw-r--r--   0 ankur      (501) staff       (20)        0 2023-06-17 20:17:20.000000 braintrust-0.0.5/src/braintrust/cli/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)     1406 2023-06-17 20:17:20.000000 braintrust-0.0.5/src/braintrust/cli/__main__.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-17 20:20:38.554935 braintrust-0.0.5/src/braintrust/cli/install/
--rw-r--r--   0 ankur      (501) staff       (20)      472 2023-06-17 20:17:20.000000 braintrust-0.0.5/src/braintrust/cli/install/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)     8239 2023-06-17 20:17:20.000000 braintrust-0.0.5/src/braintrust/cli/install/api.py
--rw-r--r--   0 ankur      (501) staff       (20)     7240 2023-06-17 20:17:20.000000 braintrust-0.0.5/src/braintrust/cli/install/redshift.py
--rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.5/src/braintrust/oai.py
--rw-r--r--   0 ankur      (501) staff       (20)       18 2023-06-12 19:52:09.000000 braintrust-0.0.5/src/braintrust/version.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-17 20:20:38.554378 braintrust-0.0.5/src/braintrust.egg-info/
--rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-17 20:20:38.000000 braintrust-0.0.5/src/braintrust.egg-info/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      521 2023-06-17 20:20:38.000000 braintrust-0.0.5/src/braintrust.egg-info/SOURCES.txt
--rw-r--r--   0 ankur      (501) staff       (20)        1 2023-06-17 20:20:38.000000 braintrust-0.0.5/src/braintrust.egg-info/dependency_links.txt
--rw-r--r--   0 ankur      (501) staff       (20)       60 2023-06-17 20:20:38.000000 braintrust-0.0.5/src/braintrust.egg-info/entry_points.txt
--rw-r--r--   0 ankur      (501) staff       (20)      302 2023-06-17 20:20:38.000000 braintrust-0.0.5/src/braintrust.egg-info/requires.txt
--rw-r--r--   0 ankur      (501) staff       (20)       11 2023-06-17 20:20:38.000000 braintrust-0.0.5/src/braintrust.egg-info/top_level.txt
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-22 22:13:35.238494 braintrust-0.0.6/
+-rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-22 22:13:35.238348 braintrust-0.0.6/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.6/README.md
+-rw-r--r--   0 ankur      (501) staff       (20)       38 2023-06-22 22:13:35.238539 braintrust-0.0.6/setup.cfg
+-rw-r--r--   0 ankur      (501) staff       (20)     1623 2023-06-21 20:59:50.000000 braintrust-0.0.6/setup.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-22 22:13:35.234596 braintrust-0.0.6/src/
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-22 22:13:35.236592 braintrust-0.0.6/src/braintrust/
+-rw-r--r--   0 ankur      (501) staff       (20)    19765 2023-06-22 22:10:44.000000 braintrust-0.0.6/src/braintrust/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)      427 2023-06-21 20:59:50.000000 braintrust-0.0.6/src/braintrust/aws.py
+-rw-r--r--   0 ankur      (501) staff       (20)      125 2023-06-22 22:10:44.000000 braintrust-0.0.6/src/braintrust/cache.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-22 22:13:35.237510 braintrust-0.0.6/src/braintrust/cli/
+-rw-r--r--   0 ankur      (501) staff       (20)        0 2023-06-21 20:59:50.000000 braintrust-0.0.6/src/braintrust/cli/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1406 2023-06-21 20:59:50.000000 braintrust-0.0.6/src/braintrust/cli/__main__.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-22 22:13:35.238147 braintrust-0.0.6/src/braintrust/cli/install/
+-rw-r--r--   0 ankur      (501) staff       (20)      472 2023-06-21 20:59:50.000000 braintrust-0.0.6/src/braintrust/cli/install/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     8207 2023-06-21 20:59:50.000000 braintrust-0.0.6/src/braintrust/cli/install/api.py
+-rw-r--r--   0 ankur      (501) staff       (20)     6421 2023-06-21 20:59:50.000000 braintrust-0.0.6/src/braintrust/cli/install/redshift.py
+-rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.6/src/braintrust/oai.py
+-rw-r--r--   0 ankur      (501) staff       (20)       18 2023-06-22 22:11:17.000000 braintrust-0.0.6/src/braintrust/version.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-22 22:13:35.237308 braintrust-0.0.6/src/braintrust.egg-info/
+-rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-22 22:13:35.000000 braintrust-0.0.6/src/braintrust.egg-info/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      543 2023-06-22 22:13:35.000000 braintrust-0.0.6/src/braintrust.egg-info/SOURCES.txt
+-rw-r--r--   0 ankur      (501) staff       (20)        1 2023-06-22 22:13:35.000000 braintrust-0.0.6/src/braintrust.egg-info/dependency_links.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       60 2023-06-22 22:13:35.000000 braintrust-0.0.6/src/braintrust.egg-info/entry_points.txt
+-rw-r--r--   0 ankur      (501) staff       (20)      302 2023-06-22 22:13:35.000000 braintrust-0.0.6/src/braintrust.egg-info/requires.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       11 2023-06-22 22:13:35.000000 braintrust-0.0.6/src/braintrust.egg-info/top_level.txt
```

### Comparing `braintrust-0.0.5/setup.py` & `braintrust-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.5/src/braintrust/__init__.py` & `braintrust-0.0.6/src/braintrust/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,20 +5,21 @@
 
 Install the library with pip.
 
 ```bash
 pip install braintrust
 ```
 
-Then, run a simple experiment with the following code:
+Then, run a simple experiment with the following code (replace `YOUR_API_KEY` with
+your BrainTrust API key):
 
 ```python
 import braintrust
 
-experiment = braintrust.init(project="PyTest")
+experiment = braintrust.init(project="PyTest", api_key="YOUR_API_KEY")
 experiment.log(
     inputs={"test": 1},
     output="foo",
     expected="bar",
     scores={
         "n": 0.5,
     },
@@ -48,15 +49,15 @@
 
 import git
 import openai
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
-from .cache import API_INFO_PATH, CACHE_PATH
+from .cache import CACHE_PATH, LOGIN_INFO_PATH
 from .oai import run_cached_request
 
 
 class BrainTrustState:
     def __init__(self):
         self.current_project = None
         self.current_experiment = None
@@ -96,24 +97,24 @@
 @_cache
 def api_conn():
     return HTTPConnection(LOG_URL)  # TODO: Fix to use global install
 
 
 def api_get(object_type, args=None):
     resp = api_conn().get(f"/{object_type}", params=args)
-    assert resp.ok, resp.text
+    resp.raise_for_status()
     return resp.json()
 
 
 def api_insert(object_type, args):
     resp = api_conn().post(
         f"/{object_type}",
         json=args,
     )
-    assert resp.ok, resp.text
+    resp.raise_for_status()
     return resp.json()
 
 
 class ModelWrapper:
     _ENDPOINT = None
 
     def __getattr__(self, name: str) -> Any:
@@ -370,30 +371,29 @@
         return textwrap.dedent(
             f"""
         See results for all experiments in {self.project.name} at {project_url}
         See results for {self.name} at {experiment_url}"""
         )
 
 
-def init(project, experiment=None, description=None, api_url=None, org_name=None, disable_cache=False):
+def init(project, experiment=None, description=None, api_url=None, api_key=None, org_name=None, disable_cache=False):
     """
     Initialize a new experiment in a specified project. If the project does not exist, it will be created.
 
     :param project: The name of the project to create the experiment in.
     :param experiment: The name of the experiment to create. If not specified, a name will be generated automatically.
     :param description: An optional description of the experiment.
-    :param api_url: The URL of the BrainTrust API to use. If not specified, the default will be used.
+    :param api_url: The URL of the BrainTrust API. Defaults to https://www.braintrustdata.com.
+    :param api_key: The API key to use. If the parameter is not specified, will try to use the `BRAINTRUST_API_KEY` environment variable. If no API
+    key is specified, will prompt the user to login.
     :param org_name: (Optional) The name of a specific organization to connect to. This is useful if you belong to multiple.
     :param disable_cache: Do not use cached login information.
     :returns: The experiment object.
     """
-    kwargs = {"org_name": org_name, "disable_cache": disable_cache}
-    if api_url:
-        kwargs["api_url"] = api_url
-    login(**kwargs)
+    login(org_name=org_name, disable_cache=disable_cache, api_key=api_key, api_url=api_url)
 
     _state.current_project = Project(project)
     _state.current_experiment = Experiment(_state.current_project, name=experiment, description=description)
     return _state.current_experiment
 
 
 def log(inputs, output, expected, scores, metadata=None):
@@ -429,103 +429,146 @@
         raise Exception("Not initialized. Please call init() or login() first")
 
     return _state.current_experiment.log(
         inputs=inputs, output=output, expected=expected, scores=scores, metadata=metadata
     )
 
 
+def _check_org_info(org_info, org_name):
+    global ORG_ID, ORG_NAME, LOG_URL
+    for orgs in org_info:
+        if org_name is None or orgs["name"] == org_name:
+            ORG_ID = orgs["id"]
+            ORG_NAME = orgs["name"]
+            LOG_URL = orgs["api_url"]
+            break
+
+    if ORG_ID is None:
+        raise ValueError(
+            f"Organization {org_name} not found. Must be one of {', '.join([x['name'] for x in info['org_info']])}"
+        )
+
+
 def login(
-    api_url=os.environ.get("BRAINTRUST_API_URL", "https://www.braintrustdata.com"), org_name=None, disable_cache=False
+    api_url=None,
+    api_key=None,
+    org_name=None,
+    disable_cache=False,
 ):
     """
     Login to BrainTrust. This will prompt you for your API token, which you can find at
     https://www.braintrustdata.com/app/token. This method is called automatically by `init()`.
 
     :param api_url: The URL of the BrainTrust API. Defaults to https://www.braintrustdata.com.
+    :param api_key: The API key to use. If the parameter is not specified, will try to use the `BRAINTRUST_API_KEY` environment variable. If no API
+    key is specified, will prompt the user to login.
     :param org_name: (Optional) The name of a specific organization to connect to. This is useful if you belong to multiple.
     :param disable_cache: Do not use cached login information.
     """
-
     global API_URL, ORG_ID, ORG_NAME, LOG_URL
+    if ORG_ID is not None and ORG_NAME is not None and LOG_URL is not None:
+        # We have already logged in
+        return
 
-    API_URL = api_url
+    if api_url is None:
+        api_url = os.environ.get("BRAINTRUST_API_URL", "https://www.braintrustdata.com")
 
-    os.makedirs(CACHE_PATH, exist_ok=True)
+    if api_key is None:
+        api_key = os.environ.get("BRAINTRUST_API_KEY")
 
-    api_info = None
+    API_URL = api_url
+
+    login_key_info = None
     ping_ok = False
-    if os.path.exists(API_INFO_PATH) and not disable_cache:
-        with open(API_INFO_PATH) as f:
-            api_info = json.load(f)
-
-        LOG_URL = api_info.get("log_url")
-        ORG_ID = api_info.get("org_id")
-        ORG_NAME = api_info.get("org_name")
+
+    if api_key is not None:
+        resp = requests.post(_urljoin(API_URL, "/api/apikey/login"), json={"token": api_key})
+        resp.raise_for_status()
+        info = resp.json()
+
+        _check_org_info(info["org_info"], org_name)
+
         conn = api_conn()
+        conn.set_token(api_key)
 
-        token = api_info.get("token")
+        ping_resp = conn.get("ping")
+        ping_ok = ping_resp.ok
+
+    if not ping_ok and os.path.exists(LOGIN_INFO_PATH) and not disable_cache:
+        with open(LOGIN_INFO_PATH) as f:
+            login_key_info = json.load(f)
+
+        LOG_URL = login_key_info.get("log_url")
+        ORG_ID = login_key_info.get("org_id")
+        ORG_NAME = login_key_info.get("org_name")
+        conn = api_conn()
+
+        token = login_key_info.get("token")
         if token is not None:
             conn.set_token(token)
 
         ping_resp = conn.get("ping")
         ping_ok = ping_resp.ok
 
-    if not ping_ok and api_info and api_info.get("refresh_token"):
-        resp = requests.post(
-            _urljoin(API_URL, "/api/token/refresh"), json={"refresh_token": api_info.get("refresh_token")}
-        )
-        if resp.ok:
-            resp_data = resp.json()
-            token = resp_data["id_token"]
-            refresh_token = resp_data.get("refresh_token")
-
-            if not disable_cache:
-                _save_api_info({**api_info, "token": token, "refresh_token": refresh_token})
-
-            conn.set_token(token)
-            ping_resp = conn.get("ping")
-            ping_ok = ping_resp.ok
-        else:
-            _logger.warning(f"Failed to refresh token: [{resp.status_code}] {resp.text}")
+    # TODO: This logic should likely be removed permanently, because the use of refresh tokens
+    # has been superseded by API keys. However, I'm leaving it here for now in case we revisit
+    # that in the near term.
+    #
+    #    if not ping_ok and login_key_info and login_key_info.get("refresh_token"):
+    #        resp = requests.post(
+    #            _urljoin(API_URL, "/api/token/refresh"), json={"refresh_token": login_key_info.get("refresh_token")}
+    #        )
+    #        if resp.ok:
+    #            resp_data = resp.json()
+    #            token = resp_data["id_token"]
+    #            refresh_token = resp_data.get("refresh_token")
+    #
+    #            if not disable_cache:
+    #                _save_api_info({**login_key_info, "token": token, "refresh_token": refresh_token})
+    #
+    #            conn.set_token(token)
+    #            ping_resp = conn.get("ping")
+    #            ping_ok = ping_resp.ok
+    #        else:
+    #            _logger.warning(f"Failed to refresh token: [{resp.status_code}] {resp.text}")
+
+    if not ping_ok and (ORG_ID is None or ORG_NAME is None or LOG_URL is None):
+        print(
+            textwrap.dedent(
+                f"""\
+            The recommended way to login is to generate an API token at {API_URL}/app/settings.
+            However, BrainTrust also supports generating a temporary token for the SDK. This token
+            will expire after about an hour, so it is not recommended for long-term use.
 
-    if not ping_ok or (ORG_ID is None or ORG_NAME is None or LOG_URL is None):
-        print(f"Please copy your API token from {API_URL}/app/token")
+            Please copy your temporary token from {API_URL}/app/token."""
+            )
+        )
         temp_token = getpass("Token: ")
 
         resp = requests.post(_urljoin(API_URL, "/api/id-token"), json={"token": temp_token})
-        assert resp.ok, f"Failed to acquire token: {resp.text}"
+        resp.raise_for_status()
         info = resp.json()
         token = info["token"]
-        for orgs in info["org_info"]:
-            if org_name is None or orgs["name"] == org_name:
-                ORG_ID = orgs["id"]
-                ORG_NAME = orgs["name"]
-                LOG_URL = orgs["api_url"]
-                break
 
-        if ORG_ID is None:
-            raise ValueError(
-                f"Organization {org_name} not found. Must be one of {', '.join([x['name'] for x in info['org_info']])}"
-            )
+        _check_org_info(info["org_info"], org_name)
 
         if not disable_cache:
-            _save_api_info(
-                {"token": token, "org_id": ORG_ID, "log_url": LOG_URL, "refresh_token": info.get("refresh_token")}
-            )
+            _save_api_info({"token": token, "org_id": ORG_ID, "log_url": LOG_URL})
 
         conn = api_conn()
         conn.set_token(token)
 
     assert conn, "Conn should be set at this point (a bug)"
     resp = conn.get("ping")
-    assert resp.ok, "Invalid token: " + resp.text
+    resp.raise_for_status()
 
 
 def _save_api_info(api_info):
-    with open(API_INFO_PATH, "w") as f:
+    os.makedirs(CACHE_PATH, exist_ok=True)
+    with open(LOGIN_INFO_PATH, "w") as f:
         json.dump(api_info, f)
 
 
 def _urljoin(*parts):
     return "/".join([x.lstrip("/") for x in parts])
```

### Comparing `braintrust-0.0.5/src/braintrust/cli/__main__.py` & `braintrust-0.0.6/src/braintrust/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.5/src/braintrust/cli/install/api.py` & `braintrust-0.0.6/src/braintrust/cli/install/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import textwrap
 import time
 
-import boto3
 from botocore.exceptions import ClientError
 
+from ...aws import cloudformation
+
 
-_cloudformation = boto3.client("cloudformation")
 _logger = logging.getLogger("braintrust.install.api")
 
 PARAMS = {
     "OrgName": "org_name",
     "ProvisionedConcurrency": "provisioned_concurrency",
     "DwDatabase": "dw_database",
     "DwHost": "dw_host",
@@ -90,15 +90,15 @@
 
 
 def main(args):
     template = args.template or LATEST_TEMPLATE
 
     status = None
     try:
-        statuses = _cloudformation.describe_stacks(StackName=args.name)["Stacks"]
+        statuses = cloudformation.describe_stacks(StackName=args.name)["Stacks"]
         if len(statuses) == 1:
             status = statuses[0]
         _logger.debug(status)
     except ClientError as e:
         if "does not exist" not in str(e):
             raise
 
@@ -131,26 +131,26 @@
             https://www.braintrustdata.com/docs/getting-started/install or use the --create flag."""
             )
         )
         exit(1)
 
     if not exists:
         _logger.info(f"Creating stack with name {args.name}")
-        _cloudformation.create_stack(
+        cloudformation.create_stack(
             StackName=args.name,
             TemplateURL=template,
             Parameters=[
                 {"ParameterKey": param, "ParameterValue": str(args.__dict__[arg_name] or DEFAULTS.get(param, ""))}
                 for (param, arg_name) in PARAMS.items()
             ],
             Capabilities=CAPABILITIES,
         )
 
         for _ in range(120):
-            status = _cloudformation.describe_stacks(StackName=args.name)["Stacks"][0]
+            status = cloudformation.describe_stacks(StackName=args.name)["Stacks"][0]
             if status["StackStatus"] != "CREATE_IN_PROGRESS":
                 exists = True
                 break
             _logger.info("Waiting for stack to be created...")
             time.sleep(5)
         else:
             _logger.error(
@@ -176,30 +176,30 @@
         if args.__dict__[arg_name] is not None:
             param_updates[param] = args.__dict__[arg_name]
     if len(param_updates) > 0 or args.update_template:
         template_kwargs = {"TemplateURL": template} if args.update_template else {"UsePreviousTemplate": True}
         _logger.info(
             f"Updating stack with name {args.name} with params: {param_updates} and template: {template_kwargs}"
         )
-        _cloudformation.update_stack(
+        cloudformation.update_stack(
             StackName=args.name,
             Parameters=[
                 {"ParameterKey": param, "ParameterValue": str(update)} for (param, update) in param_updates.items()
             ]
             + [
                 {"ParameterKey": param, "UsePreviousValue": True}
                 for param in PARAMS.keys()
                 if param not in param_updates
             ],
             Capabilities=CAPABILITIES,
             **template_kwargs,
         )
 
         for _ in range(120):
-            status = _cloudformation.describe_stacks(StackName=args.name)["Stacks"][0]
+            status = cloudformation.describe_stacks(StackName=args.name)["Stacks"][0]
             if status["StackStatus"] != "UPDATE_IN_PROGRESS":
                 exists = True
                 break
             _logger.info("Waiting for stack to be updated...")
             time.sleep(5)
         else:
             _logger.error(
```

### Comparing `braintrust-0.0.5/src/braintrust/cli/install/redshift.py` & `braintrust-0.0.6/src/braintrust/cli/install/redshift.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 import json
 import logging
 import re
 import textwrap
 from hashlib import md5
 
-import boto3
+from ... import api_conn, login
+from ...aws import iam, redshift_serverless
 
 
-_redhshift = boto3.client("redshift")
-_redshift_serverless = boto3.client("redshift-serverless")
-_iam = boto3.client("iam")
 _logger = logging.getLogger("braintrust.install.redshift")
 
-TABLE_NAME = "braintrust_logs"
-
 
 def build_parser(subparsers, parents):
     parser = subparsers.add_parser(
         "redshift", help="Setup Redshift to ingest from BrainTrust (Kafka)", parents=parents
     )
 
     parser.add_argument("name", help="Name of the Redshift cluster (or namespace) to create or update")
@@ -36,18 +32,18 @@
         required=True,
     )
     parser.add_argument(
         "--msk-topic-name",
         help="The name of a specific MSK topic to map into Redshift. The policy will allow access to all topics in the cluster, to support future topics",
         default="braintrust",
     )
+
     parser.add_argument(
-        "--schema-name",
-        help="The name of a Redshift schema to create that maps to the Kafka cluster",
-        default="braintrust_streaming",
+        "--org-name",
+        help="The name of your organization (optional, only needed if you belong to multiple orgs)",
     )
 
     parser.set_defaults(func=main)
 
 
 def main(args):
     if args.create:
@@ -55,21 +51,21 @@
 
     if args.msk_topic_name.lower() != args.msk_topic_name:
         raise ValueError("Kafka topic names must be lowercase (b/c of Redshift case sensitivity issues)")
 
     role_name = args.iam_role or ("bt-redshift-" + md5(args.msk_cluster_arn.encode("utf-8")).hexdigest())
     role = None
     try:
-        role = _iam.get_role(RoleName=role_name)
-    except _iam.exceptions.NoSuchEntityException:
+        role = iam.get_role(RoleName=role_name)
+    except iam.exceptions.NoSuchEntityException:
         pass
 
     if role is None:
         _logger.info("Creating IAM Role %s", role_name)
-        role = _iam.create_role(
+        role = iam.create_role(
             RoleName=role_name,
             AssumeRolePolicyDocument=json.dumps(
                 {
                     "Version": "2012-10-17",
                     "Statement": [
                         {
                             "Effect": "Allow",
@@ -80,16 +76,16 @@
                 }
             ),
             Description="BrainTrust Redshift Kafka Reader",
         )
 
     role_policy = None
     try:
-        role_policy = _iam.get_role_policy(RoleName=role_name, PolicyName=args.iam_policy)
-    except _iam.exceptions.NoSuchEntityException:
+        role_policy = iam.get_role_policy(RoleName=role_name, PolicyName=args.iam_policy)
+    except iam.exceptions.NoSuchEntityException:
         pass
 
     # See definitions here: https://docs.aws.amazon.com/msk/latest/developerguide/iam-access-control.html
     msk_cluster_arn = args.msk_cluster_arn
     account_info, path = msk_cluster_arn.rsplit(":", 1)
     cluster_ident, cluster_name, cluster_uuid = path.split("/")
     if cluster_ident != "cluster":
@@ -112,28 +108,28 @@
                         msk_cluster_arn,
                         msk_topic_arn,
                     ],
                 },
                 {"Sid": "MSKPolicy", "Effect": "Allow", "Action": ["kafka:GetBootstrapBrokers"], "Resource": "*"},
             ],
         }
-        role_policy = _iam.put_role_policy(
+        role_policy = iam.put_role_policy(
             RoleName=role_name, PolicyName=args.iam_policy, PolicyDocument=json.dumps(policy)
         )
 
     role_arn = role["Role"]["Arn"]
     if args.serverless:
-        namespace = _redshift_serverless.get_namespace(namespaceName=args.name)
+        namespace = redshift_serverless.get_namespace(namespaceName=args.name)
         if namespace is None:
             raise ValueError(f"Serverless Redshift namespace {args.name} does not exist")
 
         existing_roles = [re.search(r"iamRoleArn=(.*)(,|\))", d).group(1) for d in namespace["namespace"]["iamRoles"]]
         if role_arn not in existing_roles:
             _logger.info("Adding IAM Role %s to Serverless Redshift namespace %s", role_arn, args.name)
-            _redshift_serverless.update_namespace(namespaceName=args.name, iamRoles=existing_roles + [role_arn])
+            redshift_serverless.update_namespace(namespaceName=args.name, iamRoles=existing_roles + [role_arn])
     else:
         raise NotImplementedError("Only Serverless Redshift is currently supported")
 
     #    if args.serverless:
     #        workgroup = None
     #        next_token = {}
     #        while workgroup is None:
@@ -154,34 +150,13 @@
     #            if database:
     #                kwargs["dbName"] = database
     #            return _redshift_serverless.get_credentials(workgroupName=args.name, **kwargs)
     #
     #    else:
     #        raise NotImplementedError("Only Serverless Redshift is currently supported")
 
-    print(
-        textwrap.dedent(
-            f"""
-        The CLI does not yet support running the setup queries against Redshift. Often, Redshift
-        is not accessible from the public internet. You can run queries by visiting the SQL workbench,
-        e.g. https://us-east-1.console.aws.amazon.com/sqlworkbench (fill in your region appropriately).
-
-        Once connected, run the following commands to complete the setup process:
-
-        CREATE EXTERNAL SCHEMA "{args.schema_name}"
-            FROM MSK
-            IAM_ROLE  '{role['Role']['Arn']}'
-            AUTHENTICATION iam
-            CLUSTER_ARN '{msk_cluster_arn}';
-
-
-        CREATE MATERIALIZED VIEW "{TABLE_NAME}" AUTO REFRESH YES AS
-            SELECT "kafka_partition",
-            "kafka_offset",
-            "kafka_timestamp_type",
-            "kafka_timestamp",
-            "kafka_key",
-            JSON_PARSE("kafka_value") as data,
-            "kafka_headers"
-            FROM "{args.schema_name}"."{args.msk_topic_name}";"""
-        )
-    )
+    login_kwargs = {"org_name": args.org_name, "disable_cache": True} if args.org_name else {}
+    login(**login_kwargs)
+
+    resp = api_conn().get("/dw-test", params={"iam_role": role["Role"]["Arn"], "msk_cluster_arn": msk_cluster_arn})
+    resp.raise_for_status()
+    _logger.info(f"Finished setting up Redshift: {resp.json()}")
```

### Comparing `braintrust-0.0.5/src/braintrust/oai.py` & `braintrust-0.0.6/src/braintrust/oai.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.5/src/braintrust.egg-info/SOURCES.txt` & `braintrust-0.0.6/src/braintrust.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 setup.py
 src/braintrust/__init__.py
+src/braintrust/aws.py
 src/braintrust/cache.py
 src/braintrust/oai.py
 src/braintrust/version.py
 src/braintrust.egg-info/PKG-INFO
 src/braintrust.egg-info/SOURCES.txt
 src/braintrust.egg-info/dependency_links.txt
 src/braintrust.egg-info/entry_points.txt
```

