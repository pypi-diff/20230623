# Comparing `tmp/mindsight_people_control_api-0.1.6.tar.gz` & `tmp/mindsight_people_control_api-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mindsight_people_control_api-0.1.6.tar", max compression
+gzip compressed data, was "mindsight_people_control_api-0.1.7.tar", max compression
```

## Comparing `mindsight_people_control_api-0.1.6.tar` & `mindsight_people_control_api-0.1.7.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1062 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/LICENSE
--rw-r--r--   0        0        0     1342 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/README.md
--rw-r--r--   0        0        0      407 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/__init__.py
--rw-r--r--   0        0        0        0 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/helpers/__init__.py
--rw-r--r--   0        0        0     5225 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/helpers/base_requests.py
--rw-r--r--   0        0        0      392 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/helpers/exceptions.py
--rw-r--r--   0        0        0     1869 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/helpers/models.py
--rw-r--r--   0        0        0      783 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/__init__.py
--rw-r--r--   0        0        0     4566 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/area_records.py
--rw-r--r--   0        0        0     7415 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/areas.py
--rw-r--r--   0        0        0     5513 2023-06-15 18:57:39.852065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_areas.py
--rw-r--r--   0        0        0     5591 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_managers.py
--rw-r--r--   0        0        0     5623 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_positions.py
--rw-r--r--   0        0        0     4896 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_records.py
--rw-r--r--   0        0        0    12367 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employees.py
--rw-r--r--   0        0        0     4721 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/parent_areas.py
--rw-r--r--   0        0        0     7060 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/positions.py
--rw-r--r--   0        0        0     7654 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/users.py
--rw-r--r--   0        0        0      843 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/settings.py
--rw-r--r--   0        0        0        0 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/utils/__init__.py
--rw-r--r--   0        0        0      308 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/mindsight_people_control_api/utils/aux_functions.py
--rw-r--r--   0        0        0      699 2023-06-15 18:57:39.856065 mindsight_people_control_api-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2227 1970-01-01 00:00:00.000000 mindsight_people_control_api-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-23 13:47:51.100993 mindsight_people_control_api-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1342 2023-06-23 13:47:51.100993 mindsight_people_control_api-0.1.7/README.md
+-rw-r--r--   0        0        0      428 2023-06-23 13:47:51.100993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/helpers/__init__.py
+-rw-r--r--   0        0        0     5225 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/helpers/base_requests.py
+-rw-r--r--   0        0        0      392 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/helpers/exceptions.py
+-rw-r--r--   0        0        0     1869 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/helpers/models.py
+-rw-r--r--   0        0        0      865 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/__init__.py
+-rw-r--r--   0        0        0     4566 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/area_records.py
+-rw-r--r--   0        0        0     7415 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/areas.py
+-rw-r--r--   0        0        0     5513 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/employee_areas.py
+-rw-r--r--   0        0        0     5591 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/employee_managers.py
+-rw-r--r--   0        0        0     5623 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/employee_positions.py
+-rw-r--r--   0        0        0     4896 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/employee_records.py
+-rw-r--r--   0        0        0    12367 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/employees.py
+-rw-r--r--   0        0        0     4721 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/parent_areas.py
+-rw-r--r--   0        0        0     2057 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/position_records.py
+-rw-r--r--   0        0        0     7060 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/positions.py
+-rw-r--r--   0        0        0     7654 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/users.py
+-rw-r--r--   0        0        0      895 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/settings.py
+-rw-r--r--   0        0        0        0 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/utils/__init__.py
+-rw-r--r--   0        0        0      308 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/mindsight_people_control_api/utils/aux_functions.py
+-rw-r--r--   0        0        0      699 2023-06-23 13:47:51.104993 mindsight_people_control_api-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2227 1970-01-01 00:00:00.000000 mindsight_people_control_api-0.1.7/PKG-INFO
```

### Comparing `mindsight_people_control_api-0.1.6/LICENSE` & `mindsight_people_control_api-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.6/README.md` & `mindsight_people_control_api-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.6/mindsight_people_control_api/helpers/base_requests.py` & `mindsight_people_control_api-0.1.7/mindsight_people_control_api/helpers/base_requests.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.6/mindsight_people_control_api/helpers/models.py` & `mindsight_people_control_api-0.1.7/mindsight_people_control_api/helpers/models.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/__init__.py` & `mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,8 +5,9 @@
 from mindsight_people_control_api.scripts.employee_areas import EmployeeAreas
 from mindsight_people_control_api.scripts.employee_managers import EmployeeManagers
 from mindsight_people_control_api.scripts.employee_positions import EmployeePositions
 from mindsight_people_control_api.scripts.employee_records import EmployeeRecord
 from mindsight_people_control_api.scripts.employees import Employees
 from mindsight_people_control_api.scripts.parent_areas import ParentAreas
 from mindsight_people_control_api.scripts.positions import Positions
+from mindsight_people_control_api.scripts.position_records import PositionRecords
 from mindsight_people_control_api.scripts.users import Users
```

### Comparing `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/area_records.py` & `mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/area_records.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/areas.py` & `mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/areas.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_areas.py` & `mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/employee_areas.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_managers.py` & `mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/employee_managers.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_positions.py` & `mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/employee_positions.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employee_records.py` & `mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/employee_records.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/employees.py` & `mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/employees.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/parent_areas.py` & `mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/parent_areas.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/positions.py` & `mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/positions.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.6/mindsight_people_control_api/scripts/users.py` & `mindsight_people_control_api-0.1.7/mindsight_people_control_api/scripts/users.py`

 * *Files identical despite different names*

### Comparing `mindsight_people_control_api-0.1.6/mindsight_people_control_api/settings.py` & `mindsight_people_control_api-0.1.7/mindsight_people_control_api/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,7 +22,8 @@
 API_ENDPOINT_AREAS_RECORDS = "/area_records"
 API_ENDPOINT_PARENT_AREAS = "/parent_areas"
 API_ENDPOINT_EMPLOYEE_AREAS = "/employee_areas"
 API_ENDPOINT_EMPLOYEE_POSITIONS = "/employee_positions"
 API_ENDPOINT_EMPLOYEE_MANAGERS = "/employee_managers"
 API_ENDPOINT_USERS = "/users"
 API_ENDPOINT_POSITIONS = "/positions"
+API_ENDPOINT_POSITION_RECORDS = "/position_records"
```

### Comparing `mindsight_people_control_api-0.1.6/pyproject.toml` & `mindsight_people_control_api-0.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mindsight-people-control-api"
-version = "0.1.6"
+version = "0.1.7"
 description = "Mindsight People Control API to create, update and delete records"
 authors = ["stone_people_analytics <systems-techpeople@stone.com.br>"]
 maintainers = [
     "diogo56 <diogo.amorim2001@gmail.com>",
     "guilherme_lsilva <manager.guilherme.silva@gmail.com>",
 ]
 readme = "README.md"
```

### Comparing `mindsight_people_control_api-0.1.6/PKG-INFO` & `mindsight_people_control_api-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mindsight-people-control-api
-Version: 0.1.6
+Version: 0.1.7
 Summary: Mindsight People Control API to create, update and delete records
 Home-page: https://github.com/people-analytics-tech/mindsight-people-control-api
 License: MIT
 Author: stone_people_analytics
 Author-email: systems-techpeople@stone.com.br
 Maintainer: diogo56
 Maintainer-email: diogo.amorim2001@gmail.com
```

