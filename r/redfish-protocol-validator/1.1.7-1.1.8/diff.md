# Comparing `tmp/redfish_protocol_validator-1.1.7.tar.gz` & `tmp/redfish_protocol_validator-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redfish_protocol_validator-1.1.7.tar", last modified: Fri Jun 16 20:11:41 2023, max compression
+gzip compressed data, was "redfish_protocol_validator-1.1.8.tar", last modified: Fri Jun 23 20:21:03 2023, max compression
```

## Comparing `redfish_protocol_validator-1.1.7.tar` & `redfish_protocol_validator-1.1.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:41.953263 redfish_protocol_validator-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-16 20:11:41.953263 redfish_protocol_validator-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:41.953263 redfish_protocol_validator-1.1.7/redfish_protocol_validator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/accounts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/console_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    32037 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14056 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/protocol_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    24902 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/redfish_logo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    21012 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    54306 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/security_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    48774 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/service_details.py
--rw-r--r--   0 runner    (1001) docker     (123)    65115 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/service_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    28978 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/service_responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16089 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/system_under_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13570 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 20:11:41.953263 redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-16 20:11:41.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-16 20:11:41.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 20:11:41.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-16 20:11:41.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-16 20:11:41.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-16 20:11:41.000000 redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 20:11:41.953263 redfish_protocol_validator-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-16 20:11:29.000000 redfish_protocol_validator-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:21:03.021843 redfish_protocol_validator-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-23 20:21:03.021843 redfish_protocol_validator-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:21:03.017843 redfish_protocol_validator-1.1.8/redfish_protocol_validator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator/console_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28971 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14056 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator/protocol_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24902 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator/redfish_logo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7595 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20593 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52525 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator/security_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46230 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator/service_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64565 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator/service_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28730 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator/service_responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16032 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator/system_under_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13570 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 20:21:03.021843 redfish_protocol_validator-1.1.8/redfish_protocol_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-06-23 20:21:02.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-23 20:21:02.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 20:21:02.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-23 20:21:02.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-23 20:21:02.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-23 20:21:02.000000 redfish_protocol_validator-1.1.8/redfish_protocol_validator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 20:21:03.021843 redfish_protocol_validator-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-23 20:20:51.000000 redfish_protocol_validator-1.1.8/setup.py
```

### Comparing `redfish_protocol_validator-1.1.7/LICENSE.md` & `redfish_protocol_validator-1.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.1.7/PKG-INFO` & `redfish_protocol_validator-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish_protocol_validator
-Version: 1.1.7
+Version: 1.1.8
 Summary: Redfish Protocol Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_protocol_validator-1.1.7/README.md` & `redfish_protocol_validator-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator/accounts.py` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator/accounts.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator/console_scripts.py` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator/console_scripts.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from redfish_protocol_validator import service_requests
 from redfish_protocol_validator import service_responses
 from redfish_protocol_validator import sessions
 from redfish_protocol_validator import utils
 from redfish_protocol_validator.constants import Result
 from redfish_protocol_validator.system_under_test import SystemUnderTest
 
-tool_version = '1.1.7'
+tool_version = '1.1.8'
 
 
 def perform_tests(sut: SystemUnderTest):
     """Perform the protocol validation tests on the resources."""
     protocol_details.test_protocol_details(sut)
     service_requests.test_service_requests(sut)
     service_responses.test_service_responses(sut)
```

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator/constants.py` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,50 +401,14 @@
         'error if the body of the request is conflicting.'
     )
     SERV_EVENT_ERROR_MUTUALLY_EXCL_PROPS = (
         'Services shall respond to a request to create a subscription with an '
         'error if the body of the request contains both RegistryPrefixes and '
         'MessageIds, and shall return the HTTP 400 Bad Request status code.'
     )
-    SERV_EVENT_PERSISTENT_ACROSS_RESTARTS = (
-        'Services shall retain subscriptions as persistent across service '
-        'restarts.'
-    )
-    SERV_EVENT_PUSH_ONLY_ON_SUBSCRIPTION = (
-        'Services shall not push events by using HTTP POST unless an event '
-        'subscription has been created.'
-    )
-    SERV_EVENT_PAYLOAD_SIZE_LIMIT = (
-        'Services shall not send a push event payload larger than 1 Mebibyte '
-        '(1 MiB). If there is more than 1 MiB worth of data to send the '
-        'service shall divide the payload on the nearest Event entry such '
-        'that the total payload transmitted to the client is less than 1 MiB.'
-    )
-    SERV_EVENT_METRIC_REPORT_FORMAT = (
-        'Metric report message objects sent to the specified client endpoint '
-        'shall contain the properties, as described in the Redfish '
-        'MetricReport schema.'
-    )
-    SERV_EVENT_OTHER_FORMAT = (
-        'Event message objects POSTed to the specified client endpoint shall '
-        'contain the properties as described in the Redfish Event schema.'
-    )
-    SERV_EVENT_MESSAGE_KEY_FORMAT = (
-        '[The MessageKey variable] shall not include spaces, periods, or '
-        'special characters.'
-    )
-    SERV_EVENT_OEM_NO_ADDITIONAL_MESSAGE_ARGS = (
-        'OEMs shall not supply additional message arguments beyond those in a '
-        'standard Message Registry.'
-    )
-    SERV_EVENT_OEM_NO_CHANGED_REGISTRY_VALUES = (
-        'OEMs may substitute their own Message Registry for the standard '
-        'registry to provide the OEM section within the registry but shall '
-        'not change the standard values, such as messages, in such registries.'
-    )
     SERV_SSDP_CAN_BE_DISABLED = (
         'Use of SSDP is optional, and if implemented, shall enable the user '
         'to disable the protocol through the ManagerNetworkProtocol resource.'
     )
     SERV_SSDP_USN_MATCHES_SERVICE_ROOT_UUID = (
         'The UUID in the USN field of the service shall equal the UUID '
         'property in the Service Root.'
@@ -474,20 +438,14 @@
         'The managed device shall provide clients with the AL header that '
         'points to the Redfish Service Root URL.'
     )
     SERV_SSDP_M_SEARCH_RESPONSE_FORMAT = (
         'The response to an M-SEARCH multicast or unicast query shall use '
         'the [example format shown].'
     )
-    SERV_SSDP_DISABLE_ADDITIONAL_UPNP_MESSAGES = (
-        'If [additional UPnP-defined SSDP messages to announce their '
-        'availability to software are] implemented, services shall allow the '
-        'end user to disable the traffic separately from the M-SEARCH '
-        'response functionality.'
-    )
     SERV_SSE_SUCCESSFUL_RESPONSE = (
         'Successful resource responses for SSE shall return the HTTP 200 OK '
         'status code and have a Content-Type header set as '
         '"text/event-stream" or "text/event-stream;charset=utf-8".'
     )
     SERV_SSE_UNSUCCESSFUL_RESPONSE = (
         'Unsuccessful resource responses for SSE shall return an HTTP status '
@@ -602,19 +560,14 @@
         'RFC7617, and shall use only connections that conform to TLS to '
         'transport the data between any third-party authentication service '
         'and clients.'
     )
     SEC_BASIC_AUTH_OVER_HTTPS = (
         'All requests that use HTTP Basic authentication shall require HTTPS.'
     )
-    SEC_CHANNEL_AUTH_HEADER = (
-        # TODO(bdodd): needs clarification in the spec
-        'An authentication header shall accompany every request that '
-        'establishes a secure channel.'
-    )
     SEC_REQUIRE_LOGIN_SESSIONS = (
         'Service shall provide login sessions that conform with this '
         'specification.'
     )
     SEC_SESSIONS_URI_LOCATION = (
         'To establish a session, find the URI in either the Session '
         'Service\'s Sessions property or the Service Root\'s links property '
@@ -658,18 +611,14 @@
     SEC_PWD_CHANGE_REQ_DISALLOW_ALL_OTHERS = (
         'For all other operations [when using an account with '
         'PasswordChangeRequired set to true], the service shall respond with '
         'the HTTP 403 Forbidden status code and include a '
         '@Message.ExtendedInfo object that contains the '
         'PasswordChangeRequired message from the Base Message Registry.'
     )
-    SEC_PRIV_EQUIVALENT_ROLES = (
-        # TODO(bdodd): Difficult; try to implement at a future date
-        'Two roles with the same privileges shall behave equivalently.'
-    )
     SEC_PRIV_ONE_ROLE_PRE_USER = (
         'Each user shall be assigned exactly one role.'
     )
     SEC_PRIV_SUPPORT_PREDEFINED_ROLES = (
         'Services shall support the previous predefined roles [Administrator, '
         'Operator, and ReadOnly].'
     )
@@ -677,25 +626,13 @@
         'The AssignedPrivileges property in the Role resource for the '
         'predefined roles shall not be modifiable.'
     )
     SEC_PRIV_ROLE_ASSIGNED_AT_ACCOUNT_CREATE = (
         'A predefined role or a custom role shall be assigned to a user when '
         'a manager account is created.'
     )
-    SEC_PRIV_MODEL_SAME_FOR_ETAG_AND_ITS_DATA = (
-        # TODO(bdodd): Not sure how to test this
-        'Services shall enforce the same privilege model for ETag-related '
-        'activity as is enforced for the data being represented by the ETag.'
-    )
     SEC_PRIV_OPERATION_TO_PRIV_MAPPING = (
         'For every request that a client makes to a service, the service '
         'shall determine that the authenticated identity of the requester has '
         'the authorization to complete the requested operation on the '
         'resource in the request.'
     )
-    SEC_PRIV_REDFISH_FORUM_PRIV_REGISTRY_DEF = (
-        # TODO(bdodd): See notes from Mike R. on testing
-        'If a service provides a Privilege Registry, the service shall use '
-        'the Redfish Forum\'s Privilege Registry definition as a base '
-        'operation-to-privilege mapping definition for operations that the '
-        'service supports to promote interoperability for Redfish clients.'
-    )
```

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator/protocol_details.py` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator/protocol_details.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator/redfish_logo.py` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator/redfish_logo.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator/report.py` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator/report.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator/resources.py` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator/resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,26 +50,14 @@
                             uri = m['@odata.id']
                             # uncomment next 2 lines if we need to read certs
                             # r = session.get(sut.rhost + uri)
                             # yield {'uri': uri, 'response': r}
                             sut.add_cert(coll_uri, uri)
 
 
-def get_all_resources(sut: SystemUnderTest, uri='/redfish/v1/',
-                      uris=None):
-    # TODO(bdodd): walk entire service, yielding the resource GET responses
-    raise NotImplementedError
-
-
-def get_select_resources(sut: SystemUnderTest, uri='/redfish/v1/',
-                         uris=None):
-    # TODO(bdodd): fetch specified URIs, yielding the resource GET responses
-    raise NotImplementedError
-
-
 def get_default_resources(sut: SystemUnderTest, uri='/redfish/v1/',
                           uris=None):
     """
     Generator function to retrieve the default set of resources to test
 
     :param sut: SystemUnderTest object
     :param uri: the starting URI (default is '/redfish/v1/')
```

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator/security_details.py` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator/security_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -439,20 +439,14 @@
         else:
             # request failed trying to use HTTP with basic auth
             sut.log(Result.PASS, response.request.method,
                     response.status_code, uri,
                     Assertion.SEC_BASIC_AUTH_OVER_HTTPS, 'Test passed')
 
 
-def test_security_channel_auth_header(sut: SystemUnderTest):
-    """Perform test for Assertion.SEC_CHANNEL_AUTH_HEADER"""
-    # TODO(bdodd): needs clarification in the spec
-    pass
-
-
 def test_require_login_sessions(sut: SystemUnderTest):
     """Perform test for Assertion.SEC_REQUIRE_LOGIN_SESSIONS"""
     response = sut.get_response('POST', sut.sessions_uri)
     if response is not None:
         if response.ok:
             location = response.headers.get('Location')
             token = response.headers.get('X-Auth-Token')
@@ -872,20 +866,14 @@
     else:
         msg = ('No PATCH request to account URI found using account with '
                'PasswordChangeRequired set; unable to test this assertion')
         sut.log(Result.NOT_TESTED, 'PATCH', '', '',
                 Assertion.SEC_PWD_CHANGE_REQ_ALLOW_PATCH_PASSWORD, msg)
 
 
-def test_priv_equivalent_roles(sut: SystemUnderTest):
-    """Perform test for Assertion.SEC_PRIV_EQUIVALENT_ROLES."""
-    # TODO(bdodd): Difficult; try to implement at a future date
-    pass
-
-
 def test_priv_one_role_per_user(sut: SystemUnderTest):
     """Perform test for Assertion.SEC_PRIV_ONE_ROLE_PRE_USER."""
     for uri, response in sut.get_responses_by_method(
             'GET', resource_type=ResourceType.MANAGER_ACCOUNT).items():
         if response.ok:
             data = response.json()
             role = data.get('RoleId')
@@ -943,82 +931,63 @@
 
 def test_priv_predefined_roles_not_modifiable(sut: SystemUnderTest):
     """Perform test for Assertion.SEC_PRIV_PREDEFINED_ROLE_NOT_MODIFIABLE."""
     read_only_found = False
     uri = None
     data = {}
     role = 'ReadOnly'
-    # TODO(bdodd): Add standard priv instead of made-up one? Or delete instead?
-    test_priv = 'RfProtoValTestPriv'
-    # locate ReadOnly role
+    test_priv = ['Login', 'ConfigureManager', 'ConfigureUsers',
+                 'ConfigureComponents', 'ConfigureSelf']
+    # locate the ReadOnly role
     for uri, response in sut.get_responses_by_method(
             'GET', resource_type=ResourceType.ROLE).items():
         if response.ok:
             data = response.json()
             if data.get('Id') == role:
                 read_only_found = True
                 break
     if read_only_found:
+        # Save the current privileges in case the PATCH is accepted
         privs = data.get('AssignedPrivileges')
-        if len(privs) and test_priv not in privs:
-            # build payload to add a new priv to AssignedPrivileges
-            new_privs = [{}] * len(privs)
-            if privs[-1] is None:
-                # rigid array type
-                for i in range(len(privs)):
-                    if privs[i] is None:
-                        new_privs[i] = test_priv
-                        break
-            else:
-                # variable or fixed array type
-                new_privs.append(test_priv)
-            payload = {'AssignedPrivileges': new_privs}
+        if privs:
+            # PATCH the test privileges
+            payload = {'AssignedPrivileges': test_priv}
             headers = utils.get_etag_header(sut, sut.session, uri)
-            # issue the PATCH
             response = sut.session.patch(sut.rhost + uri, json=payload,
                                          headers=headers)
             if response.ok:
                 msg = ('PATCH request to %s to modify the AssignedPrivileges '
                        'of predefined role %s succeeded with status %s; '
                        'expected it to fail' %
                        (uri, role, response.status_code))
                 sut.log(Result.FAIL, 'PATCH', response.status_code, uri,
                         Assertion.SEC_PRIV_PREDEFINED_ROLE_NOT_MODIFIABLE,
                         msg)
                 # PATCH succeeded unexpectedly; try to PATCH it back
                 r = sut.session.get(sut.rhost + uri)
                 if r.ok:
-                    d = r.json()
-                    patched_privs = d.get('AssignedPrivileges')
-                    if test_priv in patched_privs:
-                        payload = {'AssignedPrivileges': privs}
-                        etag = r.headers.get('ETag')
-                        headers = {'If-Match': etag} if etag else {}
-                        sut.session.patch(
-                            sut.rhost + uri, json=payload, headers=headers)
+                    payload = {'AssignedPrivileges': privs}
+                    etag = r.headers.get('ETag')
+                    headers = {'If-Match': etag} if etag else {}
+                    sut.session.patch(sut.rhost + uri, json=payload,
+                                      headers=headers)
             else:
                 sut.log(Result.PASS, 'PATCH', response.status_code, uri,
                         Assertion.SEC_PRIV_PREDEFINED_ROLE_NOT_MODIFIABLE,
                         'Test passed')
         else:
-            if len(privs):
-                msg = ('Test privilege %s already present in predefined role '
-                       '%s; unable to test this assertion' % (test_priv, role))
-            else:
-                msg = ('No AssignedPrivileges found in role %s; unable to '
-                       'test this assertion' % role)
+            msg = ('No AssignedPrivileges found in role %s; unable to '
+                   'test this assertion' % role)
             sut.log(Result.NOT_TESTED, 'PATCH', '', uri,
-                    Assertion.SEC_PRIV_PREDEFINED_ROLE_NOT_MODIFIABLE,
-                    msg)
+                    Assertion.SEC_PRIV_PREDEFINED_ROLE_NOT_MODIFIABLE, msg)
     else:
-        msg = ('Redefined role %s not found; unable to test this assertion'
+        msg = ('Predefined role %s not found; unable to test this assertion'
                % role)
         sut.log(Result.NOT_TESTED, 'PATCH', '', '',
-                Assertion.SEC_PRIV_PREDEFINED_ROLE_NOT_MODIFIABLE,
-                msg)
+                Assertion.SEC_PRIV_PREDEFINED_ROLE_NOT_MODIFIABLE, msg)
 
 
 def test_priv_roles_assigned_at_account_create(sut: SystemUnderTest):
     """Perform test for Assertion.SEC_PRIV_ROLE_ASSIGNED_AT_ACCOUNT_CREATE."""
     for uri, response in sut.get_responses_by_method(
             'GET', resource_type=ResourceType.MANAGER_ACCOUNT).items():
         if response.ok:
@@ -1034,20 +1003,14 @@
                     msg = ('Newly created account with username %s does not '
                            'have a RoleId property' % username)
                     sut.log(Result.FAIL, 'GET', response.status_code, uri,
                             Assertion.SEC_PRIV_ROLE_ASSIGNED_AT_ACCOUNT_CREATE,
                             msg)
 
 
-def test_priv_model_same_for_etag_and_its_data(sut: SystemUnderTest):
-    """Perform test for Assertion.SEC_PRIV_MODEL_SAME_FOR_ETAG_AND_ITS_DATA."""
-    # TODO(bdodd): Not sure how to test this
-    pass
-
-
 def test_priv_operation_to_priv_mapping(sut: SystemUnderTest):
     """Perform test for Assertion.SEC_PRIV_OPERATION_TO_PRIV_MAPPING."""
     response_found = False
     for uri, response in sut.get_responses_by_method(
             'PATCH', resource_type=ResourceType.MANAGER_ACCOUNT,
             request_type=RequestType.MODIFY_OTHER).items():
         response_found = True
@@ -1084,50 +1047,40 @@
         msg = ('No response found attempting to PATCH an account using the '
                'credentials of other user; unable to test this assertion')
         sut.log(Result.NOT_TESTED, 'PATCH', '', '',
                 Assertion.SEC_PRIV_OPERATION_TO_PRIV_MAPPING,
                 msg)
 
 
-def test_priv_redfish_forum_priv_regisistry_def(sut: SystemUnderTest):
-    """Perform test for Assertion.SEC_PRIV_REDFISH_FORUM_PRIV_REGISTRY_DEF."""
-    # TODO(bdodd): See notes from Mike R. on testing
-    pass
-
-
 def test_authentication(sut: SystemUnderTest):
     """Perform authentication tests"""
     test_basic_auth_standalone(sut)
     test_both_auth_types(sut)
     test_write_requires_auth(sut)
     test_read_requires_auth(sut)
     test_redirect_enforces_target_privs(sut)
     test_redirect_to_https(sut)
     test_no_priv_info_in_msgs(sut)
     test_headers_auth_before_etag(sut)
     test_no_auth_cookies(sut)
     test_support_basic_auth(sut)
     test_basic_auth_over_https(sut)
-    test_security_channel_auth_header(sut)
     test_require_login_sessions(sut)
     test_sessions_uri_location(sut)
     test_session_post_response(sut)
     if not sut.avoid_http_redirect:
         test_session_create_https_only(sut)
     test_session_termination_side_effects(sut)
     test_accounts_support_etags(sut)
     test_password_change_required(sut)
-    test_priv_equivalent_roles(sut)
     test_priv_one_role_per_user(sut)
     test_priv_support_predefined_roles(sut)
     test_priv_predefined_roles_not_modifiable(sut)
     test_priv_roles_assigned_at_account_create(sut)
-    test_priv_model_same_for_etag_and_its_data(sut)
     test_priv_operation_to_priv_mapping(sut)
-    test_priv_redfish_forum_priv_regisistry_def(sut)
 
 
 def test_protocols(sut: SystemUnderTest):
     """Perform security protocol tests"""
     test_tls_1_1(sut)
     test_default_cert_replacement(sut)
     test_certs_conform_to_x509v3(sut)
```

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator/service_details.py` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator/service_details.py`

 * *Files 8% similar despite different names*

```diff
@@ -162,60 +162,14 @@
     else:
         msg = ('No event subscriptions URI found on the service; unable to '
                'test this assertion')
         sut.log(Result.NOT_TESTED, '', '', '',
                 Assertion.SERV_EVENT_ERROR_MUTUALLY_EXCL_PROPS, msg)
 
 
-def test_subscriptions_persistent_across_restart(sut: SystemUnderTest):
-    """Perform tests for Assertion.SERV_EVENT_PERSISTENT_ACROSS_RESTARTS."""
-    # TODO(bdodd): This may be difficult to implement in a way that does not
-    #  disrupt the tool since there will be side-effects like destroying
-    #  existing sessions.
-    pass
-
-
-def test_events_push_only_on_subscription(sut: SystemUnderTest):
-    """Perform tests for Assertion.SERV_EVENT_PUSH_ONLY_ON_SUBSCRIPTION."""
-    # TODO(bdodd): Testable?
-    pass
-
-
-def test_event_payload_size_limit(sut: SystemUnderTest):
-    """Perform tests for Assertion.SERV_EVENT_PAYLOAD_SIZE_LIMIT."""
-    pass
-
-
-def test_event_metric_report_format(sut: SystemUnderTest):
-    """Perform tests for Assertion.SERV_EVENT_METRIC_REPORT_FORMAT."""
-    pass
-
-
-def test_event_other_format(sut: SystemUnderTest):
-    """Perform tests for Assertion.SERV_EVENT_OTHER_FORMAT."""
-    pass
-
-
-def test_event_message_key_format(sut: SystemUnderTest):
-    """Perform tests for Assertion.SERV_EVENT_MESSAGE_KEY_FORMAT."""
-    pass
-
-
-def test_event_oem_no_additional_message_args(sut: SystemUnderTest):
-    """Perform tests for
-    Assertion.SERV_EVENT_OEM_NO_ADDITIONAL_MESSAGE_ARGS."""
-    pass
-
-
-def test_event_oem_no_changed_registry_values(sut: SystemUnderTest):
-    """Perform tests for
-    Assertion.SERV_EVENT_OEM_NO_CHANGED_REGISTRY_VALUES."""
-    pass
-
-
 def pre_ssdp(sut: SystemUnderTest):
     """Perform prerequisite SSDP steps"""
     # discover using the redfish search target
     services = utils.discover_ssdp(search_target=SSDP_REDFISH)
     sut.add_ssdp_services(SSDP_REDFISH, services)
 
     # discover using the ssdp:all search target
@@ -528,21 +482,14 @@
         sut.log(Result.FAIL, '', '', '',
                 Assertion.SERV_SSDP_M_SEARCH_RESPONSE_FORMAT, msg)
     else:
         sut.log(Result.PASS, '', '', '',
                 Assertion.SERV_SSDP_M_SEARCH_RESPONSE_FORMAT, 'Test passed')
 
 
-def test_ssdp_disable_additional_upnp_messages(sut: SystemUnderTest):
-    """Perform tests for
-    Assertion.SERV_SSDP_DISABLE_ADDITIONAL_UPNP_MESSAGES."""
-    # TODO(bdodd): There doesn't seem to be a standard way to test this
-    pass
-
-
 def test_sse_successful_response(sut: SystemUnderTest):
     """Perform tests for Assertion.SERV_SSE_SUCCESSFUL_RESPONSE."""
     if not sut.server_sent_event_uri:
         msg = 'No ServerSentEventUri available; unable to test this assertion'
         sut.log(Result.NOT_TESTED, '', '', '',
                 Assertion.SERV_SSE_SUCCESSFUL_RESPONSE, msg)
         return
@@ -1059,43 +1006,26 @@
 
 def test_eventing(sut: SystemUnderTest):
     """Perform eventing tests"""
     test_event_service_subscription(sut)
     test_push_style_eventing(sut)
     test_event_error_on_bad_request(sut)
     test_event_error_on_mutually_excl_props(sut)
-    test_subscriptions_persistent_across_restart(sut)
-    test_events_push_only_on_subscription(sut)
-    test_event_payload_size_limit(sut)
-    test_event_metric_report_format(sut)
-    test_event_other_format(sut)
-    test_event_message_key_format(sut)
-    test_event_oem_no_additional_message_args(sut)
-    test_event_oem_no_changed_registry_values(sut)
-
-
-def test_asynchronous_ops(sut: SystemUnderTest):
-    """Perform asynchronous operation tests"""
-    # TODO(bdodd): At this time, there seems to be no async operation that
-    #     would be implemented by many vendors and be non-invasive to test.
-    #     Revisit in future.
-    pass
 
 
 def test_discovery(sut: SystemUnderTest):
     """Perform service discovery tests"""
     pre_ssdp(sut)
     test_ssdp_can_be_disabled(sut)
     test_ssdp_usn_matches_service_root_uuid(sut)
     test_ssdp_uuid_in_canonical_format(sut)
     test_ssdp_msearch_responds_to_redfish_or_all(sut)
     test_ssdp_st_header_format(sut)
     test_ssdp_al_header_points_to_service_root(sut)
     test_ssdp_m_search_response_format(sut)
-    test_ssdp_disable_additional_upnp_messages(sut)
 
 
 def test_server_sent_events(sut: SystemUnderTest):
     """Perform server sent event tests"""
     response = test_sse_successful_response(sut)
     test_sse_unsuccessful_response(sut)
     events = read_sse_events(response)
@@ -1108,20 +1038,12 @@
     test_sse_close_connection_if_event_dest_deleted(sut, response, event_dest)
     test_sse_id_uniquely_identifies_payload(sut, events)
     test_sse_data_based_on_payload_format(sut, events)
     test_sse_json_event_message_format(sut, events)
     test_sse_json_metric_report_format(sut, events)
 
 
-def test_update_service(sut: SystemUnderTest):
-    """Perform update service tests"""
-    # TODO(bdodd): Initiating an update not practical at this time
-    pass
-
-
 def test_service_details(sut: SystemUnderTest):
     """Perform tests from the 'Service details' section of the spec."""
     test_eventing(sut)
-    test_asynchronous_ops(sut)
     test_discovery(sut)
     test_server_sent_events(sut)
-    test_update_service(sut)
```

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator/service_requests.py` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator/service_requests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1343,15 +1343,14 @@
                'unable to test query parameter assertions')
         sut.log(Result.NOT_TESTED, '', '', '',
                 Assertion.REQ_QUERY_PROTOCOL_FEATURES_SUPPORTED, msg)
     else:
         test_query_ignore_unsupported(sut)
         test_query_unsupported_dollar_params(sut)
         test_query_invalid_values(sut)
-        # TODO(bdodd): add assertions for $expand, $select, and $filter
 
 
 def test_head(sut: SystemUnderTest):
     """Perform tests from the 'HEAD' sub-section of the spec."""
     test_head_differ_from_get(sut)
 
 
@@ -1403,33 +1402,20 @@
 
 
 def test_post_action(sut: SystemUnderTest):
     """Perform tests from the 'POST (Action)' sub-section of the spec."""
     # NOTE(bdodd): Actions better tested in the Redfish-Usecase-Checkers
 
 
-def test_operation_apply_time(sut: SystemUnderTest):
-    """Perform tests from the 'Operation apply time' sub-section of the
-    spec."""
-    # TODO(bdodd): Need an operation to test that will be minimally disruptive
-
-
-def test_deep_operations(sut: SystemUnderTest):
-    """Perform tests from the 'Deep operations' sub-section of the spec."""
-    # TODO(bdodd): These will be challenging to test; defer for now
-
-
 def test_service_requests(sut: SystemUnderTest):
     """Perform tests from the 'Service requests' section of the spec."""
     test_request_headers(sut)
     test_get(sut)
     test_query_params(sut)
     test_head(sut)
     test_data_modification(sut)
     test_patch_update(sut)
     test_patch_array_props(sut)
     test_put(sut)
     test_post_create(sut)
     test_delete(sut)
     test_post_action(sut)
-    test_operation_apply_time(sut)
-    test_deep_operations(sut)
```

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator/service_responses.py` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator/service_responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,20 +9,14 @@
 import requests
 
 from redfish_protocol_validator import utils
 from redfish_protocol_validator.constants import Assertion, RequestType, ResourceType, Result
 from redfish_protocol_validator.system_under_test import SystemUnderTest
 
 
-def test_access_control_allow_origin_header(sut: SystemUnderTest):
-    """Perform tests for Assertion.RESP_HEADERS_ACCESS_CONTROL_ALLOW_ORIGIN."""
-    # TODO(bdodd): How can we test this?
-    pass
-
-
 def test_header_present(sut: SystemUnderTest, header, uri, method, response,
                         assertion):
     """Test that header is present in the response."""
     if response is None:
         msg = ('No response found for %s request to %s; unable to '
                'test this assertion' % (method, uri))
         status = response.status_code if response is not None else ''
@@ -575,15 +569,14 @@
                    'document is missing')
             sut.log(Result.FAIL, 'GET', response.status_code, uri,
                     Assertion.RESP_ODATA_SERVICE_VALUE_PROP, msg)
 
 
 def test_response_headers(sut: SystemUnderTest):
     """Perform tests from the 'Response headers' sub-section of the spec."""
-    test_access_control_allow_origin_header(sut)
     test_allow_header_method_not_allowed(sut)
     test_allow_header_get_or_head(sut)
     test_cache_control_header(sut)
     test_content_type_header(sut)
     test_etag_header(sut)
     test_link_header(sut)
     test_location_header(sut)
```

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator/sessions.py` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator/sessions.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator/system_under_test.py` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator/system_under_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,15 +478,14 @@
             # Redfish Session creation failed; fall back to basic auth
             session.auth = (self.username, self.password)
             logging.warning('Creating Redfish session failed with status %s; '
                             'using Basic authentication' %
                             response.status_code)
         session.headers.update({'OData-Version': '4.0'})
         session.headers.update({'Accept-Encoding': 'identity'})
-        # TODO(bdodd): any other default headers to set?
         # session.headers.update({'Accept': 'application/json'})
         session.verify = self.verify
         self._set_session(session)
         return session
 
     def logout(self):
         if self.active_session_uri:
```

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator/utils.py` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator/utils.py`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/PKG-INFO` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redfish-protocol-validator
-Version: 1.1.7
+Version: 1.1.8
 Summary: Redfish Protocol Validator
 Home-page: https://github.com/DMTF/Redfish-Protocol-Validator
 Author: DMTF, https://www.dmtf.org/standards/feedback
 License: BSD 3-clause "New" or "Revised License"
 Keywords: Redfish
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `redfish_protocol_validator-1.1.7/redfish_protocol_validator.egg-info/SOURCES.txt` & `redfish_protocol_validator-1.1.8/redfish_protocol_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redfish_protocol_validator-1.1.7/setup.py` & `redfish_protocol_validator-1.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from codecs import open
 
 with open("README.md", "r", "utf-8") as f:
     long_description = f.read()
 
 setup(
     name="redfish_protocol_validator",
-    version="1.1.7",
+    version="1.1.8",
     description="Redfish Protocol Validator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="DMTF, https://www.dmtf.org/standards/feedback",
     license="BSD 3-clause \"New\" or \"Revised License\"",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

