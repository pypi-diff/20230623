# Comparing `tmp/google_play_developer_api-0.3.0.tar.gz` & `tmp/google_play_developer_api-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_play_developer_api-0.3.0.tar", max compression
+gzip compressed data, was "google_play_developer_api-0.4.0.tar", max compression
```

## Comparing `google_play_developer_api-0.3.0.tar` & `google_play_developer_api-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-06-23 04:12:46.830908 google_play_developer_api-0.3.0/LICENSE
--rw-r--r--   0        0        0      858 2023-06-23 04:12:46.830908 google_play_developer_api-0.3.0/README.md
--rw-r--r--   0        0        0       78 2023-06-23 04:12:46.830908 google_play_developer_api-0.3.0/google_play_developer_api/__init__.py
--rw-r--r--   0        0        0     7744 2023-06-23 04:12:46.830908 google_play_developer_api-0.3.0/google_play_developer_api/reporting.py
--rw-r--r--   0        0        0     2634 2023-06-23 04:12:46.830908 google_play_developer_api-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       37 2023-06-23 04:12:46.830908 google_play_developer_api-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1272 2023-06-23 04:12:46.830908 google_play_developer_api-0.3.0/tests/test_reporting_apis.py
--rw-r--r--   0        0        0     2910 1970-01-01 00:00:00.000000 google_play_developer_api-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-23 08:26:45.116266 google_play_developer_api-0.4.0/LICENSE
+-rw-r--r--   0        0        0      858 2023-06-23 08:26:45.116266 google_play_developer_api-0.4.0/README.md
+-rw-r--r--   0        0        0       78 2023-06-23 08:26:45.116266 google_play_developer_api-0.4.0/google_play_developer_api/__init__.py
+-rw-r--r--   0        0        0    10392 2023-06-23 08:26:45.116266 google_play_developer_api-0.4.0/google_play_developer_api/reporting.py
+-rw-r--r--   0        0        0     2697 2023-06-23 08:26:45.116266 google_play_developer_api-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       37 2023-06-23 08:26:45.116266 google_play_developer_api-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0     2337 2023-06-23 08:26:45.116266 google_play_developer_api-0.4.0/tests/test_reporting_apis.py
+-rw-r--r--   0        0        0     2967 1970-01-01 00:00:00.000000 google_play_developer_api-0.4.0/PKG-INFO
```

### Comparing `google_play_developer_api-0.3.0/LICENSE` & `google_play_developer_api-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google_play_developer_api-0.3.0/README.md` & `google_play_developer_api-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `google_play_developer_api-0.3.0/google_play_developer_api/reporting.py` & `google_play_developer_api-0.4.0/google_play_developer_api/reporting.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class ReportingService:
     def __init__(self, credentials_path: str):
         credentials = service_account.Credentials.from_service_account_file(
             credentials_path, scopes=["https://www.googleapis.com/auth/playdeveloperreporting"]
         )
-        self.reporting_service = build(
+        self._reporting_service = build(
             "playdeveloperreporting", "v1beta1", credentials=credentials, cache_discovery=False
         )
 
     def _get_report_data(
         self,
         app_package_name: str = "",
         timeline_spec: dict = {},
@@ -69,45 +69,45 @@
             "timelineSpec": timeline_spec,
             "pageSize": 100000,
         }
 
         # GET DATA
         if metric_set == "anrRateMetricSet":
             report = (
-                self.reporting_service.vitals()
+                self._reporting_service.vitals()
                 .anrrate()
                 .query(
                     name=f"apps/{app_package_name}/{metric_set}",
                     body=body,
                 )
                 .execute()
             )
         elif metric_set == "crashRateMetricSet":
             report = (
-                self.reporting_service.vitals()
+                self._reporting_service.vitals()
                 .crashrate()
                 .query(
                     name=f"apps/{app_package_name}/{metric_set}",
                     body=body,
                 )
                 .execute()
             )
         elif metric_set == "excessiveWakeupRateMetricSet":
             report = (
-                self.reporting_service.vitals()
+                self._reporting_service.vitals()
                 .excessivewakeuprate()
                 .query(
                     name=f"apps/{app_package_name}/{metric_set}",
                     body=body,
                 )
                 .execute()
             )
         elif metric_set == "stuckBackgroundWakelockRateMetricSet":
             report = (
-                self.reporting_service.vitals()
+                self._reporting_service.vitals()
                 .stuckbackgroundwakelockrate()
                 .query(
                     name=f"apps/{app_package_name}/{metric_set}",
                     body=body,
                 )
                 .execute()
             )
@@ -211,14 +211,101 @@
 
         start_time = datetime.datetime.strptime(start_time, "%Y-%m-%d %H:00")
         end_time = datetime.datetime.strptime(end_time, "%Y-%m-%d %H:00")
 
         timeline_spec = {
             "aggregationPeriod": "HOURLY",
             "startTime": {
+                "year": start_time.year,
+                "month": start_time.month,
+                "day": start_time.day,
+                "hours": start_time.hour,
+            },
+            "endTime": {
+                "year": end_time.year,
+                "month": end_time.month,
+                "day": end_time.day,
+                "hours": end_time.hour,
+            },
+        }
+
+        return self._get_report_data(
+            app_package_name=app_package_name,
+            timeline_spec=timeline_spec,
+            dimensions=dimensions,
+            metrics=metrics,
+            metric_set=metric_set,
+        )
+
+    def get_anr_rate_report_hourly(
+        self,
+        app_package_name: str = "",
+        start_time: str = "YYYY-MM-DD HH:00",
+        end_time: str = "YYYY-MM-DD HH:00",
+        dimensions: list[str] = [],
+        metrics: list[str] = [],
+    ) -> list[dict]:
+        """
+        Get ANR rate report hourly
+
+        Note:
+            Read this doc https://developers.google.com/play/developer/reporting/reference/rest/v1beta1/vitals.anrrate
+
+        Args:
+            app_package_name: App package name
+            start_time: Start time (format YYYY-MM-DD HH:00)
+            end_time: End time (format YYYY-MM-DD HH:00)
+            dimensions: Dimensions (see docs above)
+            metrics: Metrics (see docs above)
+
+        Returns:
+            List of dicts with report data
+        """
+        dimensions = (
+            [
+                "apiLevel",
+                "deviceBrand",
+                "versionCode",
+                "countryCode",
+                "deviceType",
+                "deviceModel",
+                "deviceRamBucket",
+                "deviceSocMake",
+                "deviceSocModel",
+                "deviceCpuMake",
+                "deviceCpuModel",
+                "deviceGpuMake",
+                "deviceGpuModel",
+                "deviceGpuVersion",
+                "deviceVulkanVersion",
+                "deviceGlEsVersion",
+                "deviceScreenSize",
+                "deviceScreenDpi",
+            ]
+            if not dimensions
+            else dimensions
+        )
+
+        metrics = (
+            [
+                "anrRate",
+                "userPerceivedAnrRate",
+                "distinctUsers",
+            ]
+            if not metrics
+            else metrics
+        )
+        metric_set = "anrRateMetricSet"
+
+        start_time = datetime.datetime.strptime(start_time, "%Y-%m-%d %H:00")
+        end_time = datetime.datetime.strptime(end_time, "%Y-%m-%d %H:00")
+
+        timeline_spec = {
+            "aggregationPeriod": "HOURLY",
+            "startTime": {
                 "year": start_time.year,
                 "month": start_time.month,
                 "day": start_time.day,
                 "hours": start_time.hour,
             },
             "endTime": {
                 "year": end_time.year,
```

### Comparing `google_play_developer_api-0.3.0/pyproject.toml` & `google_play_developer_api-0.4.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "google-play-developer-api"
-version = "0.3.0"
+version = "0.4.0"
 homepage = "https://github.com/ikameglobal/google-play-developer-api"
 description = "Wrapper for APIs"
 authors = ["ikameglobal <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
@@ -40,25 +40,27 @@
 mkdocs-autorefs = { version = "^0.4.1", optional = true }
 pre-commit = { version = "^3.3.2", optional = true }
 toml = { version = "^0.10.2", optional = true }
 livereload = { version = "^2.6.3", optional = true }
 pyreadline = { version = "^2.1", optional = true }
 mike = { version = "^1.1.2", optional = true }
 requests = { version = "^2.31.0", optional = true }
+pandas = { version = "^2.0.2", optional = true }
 google-api-python-client = "^2.89.0"
 
 [tool.poetry.extras]
 test = [
     "pytest",
     "black",
     "isort",
     "flake8",
     "flake8-docstrings",
     "pytest-cov",
-    "requests"
+    "requests",
+    "pandas"
 ]
 
 dev = ["tox", "pre-commit", "virtualenv", "pip", "twine", "toml"]
 
 doc = [
     "mkdocs",
     "mkdocs-include-markdown-plugin",
```

### Comparing `google_play_developer_api-0.3.0/tests/test_reporting_apis.py` & `google_play_developer_api-0.4.0/tests/test_reporting_apis.py`

 * *Files 20% similar despite different names*

```diff
@@ -32,7 +32,33 @@
     end_date = end_date.strftime("%Y-%m-%d %H:%M")
 
     report_data = report.get_crash_rate_report_hourly(app_package_name=app_package_name,
                                                       start_time=start_date,
                                                       end_time=end_date)
 
     assert len(report_data) > 0
+
+
+def test_anr_rate_report_hourly(credentials_path):
+    app_package_name = os.environ.get("APP_PACKAGE", None)
+    assert app_package_name is not None
+
+    report = ReportingService(credentials_path=credentials_path)
+    assert report is not None
+
+    # Set start_date to Yesterday 00:00 and end_date to Yesterday 02:00
+    start_date = datetime.datetime.now() - datetime.timedelta(days=1)
+    start_date = start_date.replace(hour=0, minute=0, second=0, microsecond=0)
+    end_date = start_date + datetime.timedelta(hours=10)
+
+    start_date = start_date.strftime("%Y-%m-%d %H:%M")
+    end_date = end_date.strftime("%Y-%m-%d %H:%M")
+
+    report_data = report.get_anr_rate_report_hourly(app_package_name=app_package_name,
+                                                    start_time=start_date,
+                                                    end_time=end_date)
+
+    assert len(report_data) > 0
+    # create  dataframes and write to csv
+    # import pandas as pd
+    # df = pd.DataFrame(report_data)
+    # df.to_csv("anr_rate_report_hourly.csv", index=False)
```

### Comparing `google_play_developer_api-0.3.0/PKG-INFO` & `google_play_developer_api-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-play-developer-api
-Version: 0.3.0
+Version: 0.4.0
 Summary: Wrapper for APIs
 Home-page: https://github.com/ikameglobal/google-play-developer-api
 License: MIT
 Author: ikameglobal
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -26,14 +26,15 @@
 Requires-Dist: mike (>=1.1.2,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocs (>=1.4.3,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-autorefs (>=0.4.1,<0.5.0) ; extra == "doc"
 Requires-Dist: mkdocs-include-markdown-plugin (>=4.0.4,<5.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material (>=9.1.14,<10.0.0) ; extra == "doc"
 Requires-Dist: mkdocs-material-extensions (>=1.0.3,<2.0.0) ; extra == "doc"
 Requires-Dist: mkdocstrings-python (>=1.0.0,<2.0.0) ; extra == "doc"
+Requires-Dist: pandas (>=2.0.2,<3.0.0) ; extra == "test"
 Requires-Dist: pip (>=23.1.2,<24.0.0) ; extra == "dev"
 Requires-Dist: pre-commit (>=3.3.2,<4.0.0) ; extra == "dev"
 Requires-Dist: pyreadline (>=2.1,<3.0)
 Requires-Dist: pytest (>=7.0.1,<8.0.0) ; extra == "test"
 Requires-Dist: pytest-cov (>=4.0.0,<5.0.0) ; extra == "test"
 Requires-Dist: requests (>=2.31.0,<3.0.0) ; extra == "test"
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "dev"
```

