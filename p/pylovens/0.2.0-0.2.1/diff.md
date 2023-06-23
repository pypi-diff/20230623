# Comparing `tmp/pylovens-0.2.0.tar.gz` & `tmp/pylovens-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylovens-0.2.0.tar", last modified: Sat Jun 10 07:32:07 2023, max compression
+gzip compressed data, was "pylovens-0.2.1.tar", last modified: Fri Jun 23 06:36:26 2023, max compression
```

## Comparing `pylovens-0.2.0.tar` & `pylovens-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:32:07.899435 pylovens-0.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:32:07.899435 pylovens-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:32:07.899435 pylovens-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-10 07:31:58.000000 pylovens-0.2.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-10 07:31:58.000000 pylovens-0.2.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-10 07:31:58.000000 pylovens-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-10 07:31:58.000000 pylovens-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-10 07:32:07.899435 pylovens-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-10 07:31:58.000000 pylovens-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-10 07:31:58.000000 pylovens-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 07:32:07.903435 pylovens-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:32:07.899435 pylovens-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:32:07.899435 pylovens-0.2.0/src/pylovens/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-10 07:31:58.000000 pylovens-0.2.0/src/pylovens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-10 07:32:07.000000 pylovens-0.2.0/src/pylovens/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    26398 2023-06-10 07:31:58.000000 pylovens-0.2.0/src/pylovens/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:32:07.899435 pylovens-0.2.0/src/pylovens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-10 07:32:07.000000 pylovens-0.2.0/src/pylovens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-10 07:32:07.000000 pylovens-0.2.0/src/pylovens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 07:32:07.000000 pylovens-0.2.0/src/pylovens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-10 07:32:07.000000 pylovens-0.2.0/src/pylovens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 07:32:07.000000 pylovens-0.2.0/src/pylovens.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 07:32:07.899435 pylovens-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-10 07:31:58.000000 pylovens-0.2.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    12094 2023-06-10 07:31:58.000000 pylovens-0.2.0/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:36:26.907061 pylovens-0.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:36:26.907061 pylovens-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:36:26.907061 pylovens-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-23 06:36:17.000000 pylovens-0.2.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-23 06:36:17.000000 pylovens-0.2.1/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-23 06:36:17.000000 pylovens-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-23 06:36:17.000000 pylovens-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-06-23 06:36:26.907061 pylovens-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2023-06-23 06:36:17.000000 pylovens-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-23 06:36:17.000000 pylovens-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 06:36:26.907061 pylovens-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:36:26.907061 pylovens-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:36:26.907061 pylovens-0.2.1/src/pylovens/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-23 06:36:17.000000 pylovens-0.2.1/src/pylovens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-23 06:36:26.000000 pylovens-0.2.1/src/pylovens/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27756 2023-06-23 06:36:17.000000 pylovens-0.2.1/src/pylovens/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:36:26.907061 pylovens-0.2.1/src/pylovens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-06-23 06:36:26.000000 pylovens-0.2.1/src/pylovens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-23 06:36:26.000000 pylovens-0.2.1/src/pylovens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 06:36:26.000000 pylovens-0.2.1/src/pylovens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-23 06:36:26.000000 pylovens-0.2.1/src/pylovens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 06:36:26.000000 pylovens-0.2.1/src/pylovens.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 06:36:26.907061 pylovens-0.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-23 06:36:17.000000 pylovens-0.2.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12439 2023-06-23 06:36:17.000000 pylovens-0.2.1/tests/test_client.py
```

### Comparing `pylovens-0.2.0/.github/workflows/publish.yaml` & `pylovens-0.2.1/.github/workflows/publish.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -12,21 +12,21 @@
     runs-on: ubuntu-latest
     timeout-minutes: 10
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v3
         with:
           python-version: "3.x"
 
       - name: Build
         run: |
           pip3 install build
           python3 -m build
 
       - name: Publish to PyPI
         if: startsWith(github.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `pylovens-0.2.0/.gitignore` & `pylovens-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pylovens-0.2.0/LICENSE` & `pylovens-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pylovens-0.2.0/pyproject.toml` & `pylovens-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylovens-0.2.0/src/pylovens/client.py` & `pylovens-0.2.1/src/pylovens/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,14 +234,54 @@
                 f"till={quote(end_date.strftime('%Y-%m-%dT%H:%M:%S%z'))}"
             )
 
         response = get(url, headers=self._headers_with_auth)
         response.raise_for_status()
         return response.json()
 
+    def get_health(self, bike_id: int) -> list[dict]:
+        """
+        Get bike health status.
+
+        Args:
+            bike_id: The ID of the bike.
+
+        Returns:
+            A list of four dictionaries:
+            [
+              {
+                'key': 'last_connection',
+                'status': True,
+                'value': datetime(2023, 4, 1, 17, 10, 30, tzinfo=ZoneInfo(key='Europe/Amsterdam')),
+                'value_type': 'datetime'
+              },
+              {
+                'key': 'last_gps',
+                'status': False,
+                'value': datetime(2023, 3, 31, 16, 51, 22, tzinfo=ZoneInfo(key='Europe/Amsterdam')),
+                'value_type': 'datetime'
+              },
+              {
+                'key': 'gps_battery',
+                'status': True,
+                'value': '75%',
+                'value_type': 'string'
+              },
+              {
+                'key': 'bike_system',
+                'status': True,
+                'value': 'true',
+                'value_type': 'bool'
+              }
+            ]
+        """
+        response = get(f"https://lovens.api.bike.conneq.tech/bike/{bike_id}/health", headers=self._headers_with_auth)
+        response.raise_for_status()
+        return [self._parse_dates(d, keys={"value"}) if d["value_type"] == "datetime" else d for d in response.json()]
+
     def get_location(
         self, bike_id: int, start_date: datetime | date, end_date: datetime | date
     ) -> list[dict, bool, datetime | int | float]:
         """
         Get location history in a time range.
 
         If start_date and/or end_date is a date object, they are interpreted as the start and end of the day
@@ -315,15 +355,15 @@
 
         Args:
             bike_id: The ID of the bike.
             newest_first: If True, fetch the most recent ride first. Defaults to True.
             n: Number of rides to fetch. Defaults to 50.
 
         Returns:
-            An iterables of dictionaries describing the rides.
+            An list of dictionaries describing the rides.
             Each dictionary contains, among others, the following keys:
             {
                 "id": 123456,
                 "start_date": datetime(2023, 4, 1, 17, 1, 0, tzinfo=ZoneInfo(key='Europe/Amsterdam')),
                 "end_date": datetime(2023, 4, 1, 17, 6, 30, tzinfo=ZoneInfo(key='Europe/Amsterdam')),
                 "calories": 14,
                 "avg_speed": 21,
@@ -348,15 +388,15 @@
         Args:
             bike_id: The ID of the bike.
             newest_first: If True, fetch the most recent ride first. Defaults to True.
             batch_size: The number of rides to fetch at once.
             _offset: Used in pagination.
 
         Returns:
-            An iterables of dictionaries describing the rides.
+            An iterable of dictionaries describing the rides.
             Each dictionary contains, among others, the following keys:
             {
                 "id": 123456,
                 "start_date": datetime(2023, 4, 1, 17, 1, 0, tzinfo=ZoneInfo(key='Europe/Amsterdam')),
                 "end_date": datetime(2023, 4, 1, 17, 6, 30, tzinfo=ZoneInfo(key='Europe/Amsterdam')),
                 "calories": 14,
                 "avg_speed": 21,
```

### Comparing `pylovens-0.2.0/tests/conftest.py` & `pylovens-0.2.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pylovens-0.2.0/tests/test_client.py` & `pylovens-0.2.1/tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
     def test_get_ride(self, authenticated_client: LovensClient, ride: dict):
         ride_ = authenticated_client.get_ride(ride["id"])
         assert ride_ == ride
 
 
 @if_authenticated
-class TestSimpleMethods:
+class TestMisc:
     def test_user(self, authenticated_client: LovensClient):
         user = authenticated_client.get_user()
         assert "timezone" in user
         assert "username" in user
 
     def test_timezone(self, authenticated_client: LovensClient):
         # Timezone in the format 'Europe/Amsterdam'
@@ -156,14 +156,21 @@
         assert bikes[0] == authenticated_client.get_bike(bikes[0]["id"])
 
     def test_get_state(self, authenticated_client: LovensClient, bike_id: int):
         state = authenticated_client.get_state(bike_id)
         assert "powered_on" in state
         assert isinstance(state["last_full_charge"], datetime)
 
+    def test_get_health(self, authenticated_client: LovensClient, bike_id: int):
+        health = authenticated_client.get_health(bike_id)
+        assert isinstance(health[0]["value"], datetime)
+        assert isinstance(health[1]["value"], datetime)
+        assert isinstance(health[2]["value"], str)
+        assert isinstance(health[3]["value"], str)
+
 
 @if_authenticated
 class TestGeofences:
     @fixture(scope="class")
     def geofence(self, authenticated_client: LovensClient, bike_id: int) -> dict:
         geofence_data = authenticated_client.get_geofences(bike_id)
         if len(geofence_data) == 0:
```

