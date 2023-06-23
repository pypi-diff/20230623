# Comparing `tmp/pybarb-0.3.5.tar.gz` & `tmp/pybarb-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybarb-0.3.5.tar", last modified: Tue Jun  6 16:58:31 2023, max compression
+gzip compressed data, was "pybarb-0.3.6.tar", last modified: Fri Jun 23 14:03:27 2023, max compression
```

## Comparing `pybarb-0.3.5.tar` & `pybarb-0.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:58:31.521280 pybarb-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-06 16:58:31.521280 pybarb-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-06 16:58:23.000000 pybarb-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:58:31.521280 pybarb-0.3.5/pybarb/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-06 16:58:23.000000 pybarb-0.3.5/pybarb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24065 2023-06-06 16:58:23.000000 pybarb-0.3.5/pybarb/pybarb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 16:58:31.521280 pybarb-0.3.5/pybarb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-06 16:58:31.000000 pybarb-0.3.5/pybarb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-06 16:58:31.000000 pybarb-0.3.5/pybarb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 16:58:31.000000 pybarb-0.3.5/pybarb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-06 16:58:31.000000 pybarb-0.3.5/pybarb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-06 16:58:31.000000 pybarb-0.3.5/pybarb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 16:58:31.521280 pybarb-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-06 16:58:23.000000 pybarb-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:03:27.654268 pybarb-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-23 14:03:27.654268 pybarb-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-06-23 14:03:13.000000 pybarb-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:03:27.654268 pybarb-0.3.6/pybarb/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-23 14:03:13.000000 pybarb-0.3.6/pybarb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32202 2023-06-23 14:03:13.000000 pybarb-0.3.6/pybarb/pybarb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 14:03:27.654268 pybarb-0.3.6/pybarb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-23 14:03:27.000000 pybarb-0.3.6/pybarb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-23 14:03:27.000000 pybarb-0.3.6/pybarb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 14:03:27.000000 pybarb-0.3.6/pybarb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-23 14:03:27.000000 pybarb-0.3.6/pybarb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-23 14:03:27.000000 pybarb-0.3.6/pybarb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 14:03:27.654268 pybarb-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-23 14:03:13.000000 pybarb-0.3.6/setup.py
```

### Comparing `pybarb-0.3.5/README.md` & `pybarb-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `pybarb-0.3.5/pybarb/pybarb.py` & `pybarb-0.3.6/pybarb/pybarb.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,61 @@
 import requests
 import json
 import pandas as pd
 import numpy as np
 import sqlalchemy
 import plotly.graph_objs as go
 import re
+import time
 
 
 class BarbAPI:
     """
-    A class for connecting to the Barb API and making queries.
+    Represents the Barb API.
 
     Attributes:
         api_key (str): The API key for accessing the Barb API.
-        connected (bool): Whether the API is currently connected.
-
+        api_root (str): The root URL of the Barb API.
+        connected (bool): Whether the Barb API is connected.
+        headers (dict): The headers for the Barb API.
+        current_job_id (str): The current job id for the Barb API.
+    
     Methods:
-        connect(): Connects to the Barb API.
-        programme_ratings(min_transmission_date, max_transmission_date, station=None, panel=None, consolidated=True, last_updated_greater_than=None, use_reporting_days=True, limit=5000): Gets the programme ratings for a given date range.
-        advertising_spots(min_transmission_date, max_transmission_date, station=None, panel=None, advertiser=None, buyer=None, consolidated=True, standardise_audiences=None, use_reporting_days=True, last_updated_greater_than=None, limit=5000): Gets the advertising spots for a given date range.
-        audiences_by_time(min_transmission_date, max_transmission_date, time_period_length, viewing_status, station=None, panel=None, use_polling_days=True, last_updated_greater_than=None, limit=5000): Gets the audiences by time for a given date range.
-        audiences_by_day(min_transmission_date, max_transmission_date, station=None, panel=None, use_polling_days=True, last_updated_greater_than=None, limit=5000): Gets the audiences by day for a given date range.
-
+        connect: Connects to the Barb API.
+        get_station_code: Gets the station code for a given station name.
+        get_viewing_station_code: Gets the station code for a given station name.
+        get_panel_code: Gets the panel code for a given panel region.
+        programme_ratings: Gets the programme ratings for a given date range.
+        advertising_spots: Gets the advertising spots for a given date range.
+        audiences_by_time: Gets the audiences by time for a given date range.
+        list_stations: Lists the stations available in the API.
+        list_viewing_stations: Lists the stations available in the API.
+        list_panels: Lists the panels available in the API.
+        list_buyers: Lists the buyers available in the API.
+        query_asynch_endpoint: Queries the asynch endpoint.
+        get_asynch_file_urls: Gets the asynch file urls.
+        get_asynch_files: Gets the asynch files.
+        ping_job_status: Pings the job status.
     """
 
-    def __init__(self, api_key: str):
+
+    def __init__(self, api_key: str, api_root="https://barb-api.co.uk/api/v1/"):
         """
         Initializes a new instance of the BarbAPI class.
 
         Args:
             api_key (str): The API key for accessing the Barb API.
+            api_root (str): The root URL of the Barb API.
+
         """
         self.api_key = api_key
-        self.api_root = "https://barb-api.co.uk/api/v1/"
+        self.api_root = api_root
         self.connected = False
         self.headers = None
+        self.current_job_id = None
 
     def connect(self):
         """
         Connects to the Barb API.
         """
         # Code to connect to the Barb API
         self.connected = True
@@ -66,14 +83,36 @@
         station_code = [s["station_code"]
                         for s in api_data if station_name.lower() == s['station_name'].lower()]
         if len(station_code) == 1:
             station_code = station_code[0]
         else:
             raise Exception(f"Station name {station_name} not found.")
         return station_code
+    
+    def get_viewing_station_code(self, viewing_station_name):
+        """
+        Gets the viewing_station code for a given viewing_station name.
+
+        Args:
+            viewing_station_name (str): The name of the viewing_station to query.
+
+        Returns:
+            str: The viewing_station code.
+        """
+
+        api_url = f"{self.api_root}viewing_stations/"
+        r = requests.get(url=api_url, headers=self.headers)
+        api_data = r.json()
+        viewing_station_code = [s["viewing_station_code"]
+                        for s in api_data if viewing_station_name.lower() == s['viewing_station_name'].lower()]
+        if len(viewing_station_code) == 1:
+            viewing_station_code = viewing_station_code[0]
+        else:
+            raise Exception(f"Viewing station name {viewing_station_name} not found.")
+        return viewing_station_code
 
     def get_panel_code(self, panel_region):
         """
         Gets the panel code for a given panel region.
 
         Args:
             panel_region (str): The name of the panel to query.
@@ -188,14 +227,49 @@
                   "limit": limit}
 
         api_response_data = self.query_event_endpoint(
             "audiences_by_time", params)
 
         return AudiencesByTimeResultSet(api_response_data)
     
+    def viewing(self, min_session_date, max_session_date, viewing_station=None, panel=None, activity_type=None, last_updated_greater_than=None, output_format="parquet", limit=5000):
+        """
+        Gets the viewing for a given date range.
+
+            Args:
+                min_session_date (str): The minimum session date to query.
+                max_session_date (str): The maximum session date to query.
+                viewing_station (str): The name of the viewing_station to query.
+                panel (str): The name of the panel to query.
+                activity_type (str): The activity type to query.
+                last_updated_greater_than (str): The last updated date to query.
+                output_format (str): The output format to query.
+                limit (int): The maximum number of results to return.
+
+            Returns:
+                ViewingResultSet: The viewing result set.
+        """
+
+        # The query parameters
+        params = {"min_session_date": min_session_date, "max_session_date": max_session_date,
+                  "viewing_station_code":  None if viewing_station is None else self.get_viewing_station_code(viewing_station),
+                  "panel_code":  None if panel is None else self.get_panel_code(panel),
+                  "output_format": output_format,
+                  "limit": limit}
+        
+        if activity_type is not None:
+            params["activity_type"] = activity_type
+
+        if last_updated_greater_than is not None:
+            params["last_updated_greater_than"] = last_updated_greater_than
+
+        api_response_data = self.query_asynch_endpoint("async-batch/viewing/", parameters=params)
+
+        print(f"{api_response_data['message']} The job id is {api_response_data['job_id']}")
+    
     def query_event_endpoint(self, endpoint, parameters):
         """
         Queries the event endpoint.  
             Args:
                 endpoint (str): The endpoint to query.
                 parameters (dict): The query parameters.
 
@@ -223,25 +297,47 @@
         Lists the stations available in the API.
 
             Returns:
                 list: The stations result set.
         """
 
         api_url = f"{self.api_root}stations"
+
         api_response_data = requests.get(url=api_url, headers=self.headers)
 
         list_of_stations = [x['station_name'] for x in api_response_data.json()]
 
         if regex_filter is not None:
 
             regex = re.compile(regex_filter)
             list_of_stations = list(filter(regex.search, list_of_stations))
 
         return list_of_stations
     
+    def list_viewing_stations(self, regex_filter=None):
+        """
+        Lists the stations available in the API.
+
+            Returns:
+                list: The stations result set.
+        """
+
+        api_url = f"{self.api_root}viewing_stations"
+
+        api_response_data = requests.get(url=api_url, headers=self.headers)
+
+        list_of_stations = [x['viewing_station_name'] for x in api_response_data.json()]
+
+        if regex_filter is not None:
+
+            regex = re.compile(regex_filter)
+            list_of_stations = list(filter(regex.search, list_of_stations))
+
+        return list_of_stations
+    
     def list_panels(self, regex_filter=None):
         """
         Lists the panels available in the API.
 
             Returns:
                 list: The panels result set.
         """
@@ -273,16 +369,97 @@
 
         if regex_filter is not None:
 
             regex = re.compile(regex_filter)
             list_of_buyers = list(filter(regex.search, list_of_buyers))
 
         return list_of_buyers
+    
+    def query_asynch_endpoint(self, endpoint, parameters):
+        """
+        Queries the asynch endpoint.
+
+            Args:
+                endpoint (str): The endpoint to query.
+                parameters (dict): The query parameters.
+
+            Returns:
+                dict: The API response data.
+        """ 
 
 
+        api_url = f"{self.api_root}{endpoint}"
+
+        # Query the API and turn the response into json
+        r = requests.post(url=api_url, json=parameters, headers=self.headers)
+        r_json = r.json()
+        self.current_job_id = r_json['job_id']
+        return r_json
+    
+    def get_asynch_file_urls(self, job_id=None):
+        """
+        Gets the asynch file urls.
+            
+            Args:
+                job_id (str): The job id to query.
+
+            Returns:
+                list: The asynch file urls.
+        """
+        
+
+        if job_id is None:
+            job_id = self.current_job_id
+        
+        api_url = f"{self.api_root}async-batch/results/{job_id}"
+        r = requests.get(url=api_url, headers=self.headers)
+        r_json = r.json()
+        if len(r_json['result']) == 0:
+            return False
+        urls = [x['data'] for x in r_json['result']]
+        return urls
+    
+    def get_asynch_files(self):
+        """
+        Gets the asynch files.
+            
+            Returns:
+                ViewingResultSet: The viewing result set.
+        """
+        
+
+        results = pd.DataFrame()
+        for file in self.current_file_urls:
+            df = pd.read_parquet(file)
+            results = pd.concat([results, df])
+        return ViewingResultSet(results)
+
+    def ping_job_status(self, job_id=None):
+        """
+        Pings the job status.
+                
+            Args:
+                job_id (str): The job id to query.
+
+            Returns:
+                list: The asynch file urls.
+        """ 
+
+        if job_id is None:
+            job_id = self.current_job_id
+
+        while self.get_asynch_file_urls(job_id) is False:
+            print("Job not ready yet. Sleeping for 60 seconds.")
+            time.sleep(60)
+
+        self.current_file_urls = self.get_asynch_file_urls(job_id)
+
+        print(f"Job complete. {len(self.current_file_urls)} files are ready for download.")
+        
+
 class APIResultSet:
     """
     Represents a result set from the Barb API.
     """
 
     def __init__(self, api_response_data: dict):
         """
@@ -388,15 +565,14 @@
         # create the figure with the traces and layout
         fig = go.Figure(data=traces, layout=layout)
 
         # display the chart
         return fig
 
 
-
 class ProgrammeRatingsResultSet(APIResultSet):
     """
     Represents a programme ratings result set from the Barb API.
     """
     
     def to_dataframe(self):
         """
@@ -534,8 +710,79 @@
         audience_data['transmission_time_period_start'] = pd.to_datetime(audience_data['transmission_time_period_start'])
 
         # Add the audience category names. We have a temporary problem with duplicates in this data set hence the dropping of duplicates.
         audience_categories_df = pd.DataFrame(self.api_response_data['audience_categories']).drop_duplicates(subset=['audience_code'])
         audience_data = audience_data.merge(audience_categories_df, how="left", on="audience_code").drop("audience_code", axis=1)
 
         return audience_data
+    
+
+class ViewingResultSet(APIResultSet):
+
+    def __init__(self, api_response_data):
+        """
+        Initialises a new instance of the APIResultSet class.
+
+        Args:
+            api_response_data (dict): The API response data.
+        """
+
+        bool_columns = ['TARGETED_PROMOTION', 'SKY_ULTRA_HD']
+        api_response_data[bool_columns] = api_response_data[bool_columns].astype(bool)
+
+        json_columns = [
+            'SESSION_START',
+            'SESSION_END',
+            'HOUSEHOLD',
+            'DEVICE',
+            'PANEL_VIEWERS',
+            'GUEST_VIEWERS',
+            'PROGRAMMES_VIEWED',
+            'SPOTS_VIEWED',
+            'PANEL',
+            'VIEWING_STATION',
+            'START_OF_RECORDING',
+            'VOD_PROVIDER']
+
+        for column in json_columns:
+            api_response_data[column] = api_response_data[column].apply(json.loads)
+        
+        self.api_response_data = api_response_data
+
+    def to_dataframe(self, unpack=None):
+        """
+        Converts the API response data into a pandas dataframe.
+
+        Args:
+            unpack (list): The columns to unpack
+            
+        Returns:
+            pandas.DataFrame: A dataframe containing the API response data.
+        """
+
+        if set(unpack) == set(["viewers", "programmes"]):
+
+            data_as_dict = self.api_response_data.to_dict(orient='records')
+            rows = []
+            for item in data_as_dict:
+                row = {}
+                row.update(item['HOUSEHOLD'])
+                row.update(item['DEVICE'])
+
+                for programme in item['PROGRAMMES_VIEWED']:
+                    if 'programme_start_datetime' in programme.keys():
+                        for viewer in item['PANEL_VIEWERS']:
+                            inner_row = {}
+                            inner_row.update({'programme_start_datetime': programme['programme_start_datetime']['standard_datetime'],
+                                            'programme_name': programme['programme_content']['content_name'],})
+                            inner_row.update(viewer)
+                            inner_row.update(row)
+                            rows.append(inner_row)
+
+        # Drop all columns from df with datatype that is a dict
+
+        df = pd.DataFrame(rows)
+        df = df.drop(columns=["panel_member_weights", "tv_set_properties"]).drop_duplicates()
+
+        return df
+
```

