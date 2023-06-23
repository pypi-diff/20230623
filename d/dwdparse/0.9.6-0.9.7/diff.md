# Comparing `tmp/dwdparse-0.9.6.tar.gz` & `tmp/dwdparse-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwdparse-0.9.6.tar", last modified: Tue May  9 09:40:23 2023, max compression
+gzip compressed data, was "dwdparse-0.9.7.tar", last modified: Fri Jun 23 11:58:58 2023, max compression
```

## Comparing `dwdparse-0.9.6.tar` & `dwdparse-0.9.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:23.789290 dwdparse-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-09 09:40:16.000000 dwdparse-0.9.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-09 09:40:23.789290 dwdparse-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-09 09:40:16.000000 dwdparse-0.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:23.789290 dwdparse-0.9.6/dwdparse/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    30696 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/stations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/units.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-09 09:40:16.000000 dwdparse-0.9.6/dwdparse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:23.789290 dwdparse-0.9.6/dwdparse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-05-09 09:40:23.000000 dwdparse-0.9.6/dwdparse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-09 09:40:23.000000 dwdparse-0.9.6/dwdparse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:40:23.000000 dwdparse-0.9.6/dwdparse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 09:40:23.000000 dwdparse-0.9.6/dwdparse.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 09:40:23.000000 dwdparse-0.9.6/dwdparse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-09 09:40:23.000000 dwdparse-0.9.6/dwdparse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-09 09:40:16.000000 dwdparse-0.9.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 09:40:23.789290 dwdparse-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-09 09:40:16.000000 dwdparse-0.9.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:40:23.789290 dwdparse-0.9.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-05-09 09:40:16.000000 dwdparse-0.9.6/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-09 09:40:16.000000 dwdparse-0.9.6/tests/test_stations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-09 09:40:16.000000 dwdparse-0.9.6/tests/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:58:58.372835 dwdparse-0.9.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-23 11:58:53.000000 dwdparse-0.9.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-23 11:58:58.368834 dwdparse-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-23 11:58:53.000000 dwdparse-0.9.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:58:58.368834 dwdparse-0.9.7/dwdparse/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-23 11:58:53.000000 dwdparse-0.9.7/dwdparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-23 11:58:53.000000 dwdparse-0.9.7/dwdparse/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-23 11:58:53.000000 dwdparse-0.9.7/dwdparse/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-06-23 11:58:53.000000 dwdparse-0.9.7/dwdparse/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34256 2023-06-23 11:58:53.000000 dwdparse-0.9.7/dwdparse/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-06-23 11:58:53.000000 dwdparse-0.9.7/dwdparse/stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-06-23 11:58:53.000000 dwdparse-0.9.7/dwdparse/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-23 11:58:53.000000 dwdparse-0.9.7/dwdparse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:58:58.368834 dwdparse-0.9.7/dwdparse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-23 11:58:58.000000 dwdparse-0.9.7/dwdparse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-23 11:58:58.000000 dwdparse-0.9.7/dwdparse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 11:58:58.000000 dwdparse-0.9.7/dwdparse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-23 11:58:58.000000 dwdparse-0.9.7/dwdparse.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-23 11:58:58.000000 dwdparse-0.9.7/dwdparse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-23 11:58:58.000000 dwdparse-0.9.7/dwdparse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-23 11:58:53.000000 dwdparse-0.9.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 11:58:58.372835 dwdparse-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-23 11:58:53.000000 dwdparse-0.9.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 11:58:58.368834 dwdparse-0.9.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17781 2023-06-23 11:58:53.000000 dwdparse-0.9.7/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-23 11:58:53.000000 dwdparse-0.9.7/tests/test_stations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-06-23 11:58:53.000000 dwdparse-0.9.7/tests/test_units.py
```

### Comparing `dwdparse-0.9.6/LICENSE` & `dwdparse-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.6/PKG-INFO` & `dwdparse-0.9.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwdparse
-Version: 0.9.6
+Version: 0.9.7
 Summary: Parsers for DWD's open weather data.
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/
 Project-URL: Tracker, https://github.com/jdemaeyer/dwdparse/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dwdparse Version: 0.9.6 Summary: Parsers for DWD's
+Metadata-Version: 2.1 Name: dwdparse Version: 0.9.7 Summary: Parsers for DWD's
 open weather data. Author: Jakob de Maeyer Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/ Project-URL:
 Tracker, https://github.com/jdemaeyer/dwdparse/issues/ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: lean License-File:
 LICENSE # dwdparse [![Build Status](https://img.shields.io/github/actions/
```

### Comparing `dwdparse-0.9.6/README.md` & `dwdparse-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.6/dwdparse/api.py` & `dwdparse-0.9.7/dwdparse/api.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.6/dwdparse/cli.py` & `dwdparse-0.9.7/dwdparse/cli.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.6/dwdparse/parsers.py` & `dwdparse-0.9.7/dwdparse/parsers.py`

 * *Files 10% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         'ww': 'condition',
     }
 
     def parse(self, path):
         self.logger.info("Parsing %s", path)
         with zipfile.ZipFile(path) as zf:
             infolist = zf.infolist()
-            assert len(infolist) == 1, f'Unexpected zip content in {self.path}'
+            assert len(infolist) == 1, f'Unexpected zip content in {path}'
             with zf.open(infolist[0]) as f:
                 yield from self._parse_stream(f)
 
     def _parse_stream(self, f):
         timestamps = None
         source = None
         ns = {}
@@ -425,15 +425,15 @@
                     **record
                 }
 
     def parse_station_id(self, zf, **extra):
         for filename in zf.namelist():
             if (m := re.match(r'Metadaten_Geographie_(\d+)\.txt', filename)):
                 return m.group(1)
-        raise ValueError(f"Unable to parse station ID for {self.path}")
+        raise ValueError(f"Unable to parse station ID for {zf.filename}")
 
     def parse_lat_lon_history(self, zf, dwd_station_id, **extra):
         with zf.open(f'Metadaten_Geographie_{dwd_station_id}.txt') as f:
             reader = csv.DictReader(
                 io.TextIOWrapper(f, encoding='latin1'),
                 delimiter=';')
             history = {}
@@ -522,15 +522,15 @@
             ),
         }
 
     def parse_station_id(self, zf, **extra):
         for filename in zf.namelist():
             if (m := re.match(r'produkt_.*_(\d+)\.txt', filename)):
                 return m.group(1)
-        raise ValueError(f"Unable to parse station ID for {self.path}")
+        raise ValueError(f"Unable to parse station ID for {zf.filename}")
 
     def parse_lat_lon_history(self, zf, dwd_station_id, **extra):
         if 'meta_path' not in extra:
             raise ValueError(
                 f"Must supply a `meta_path` keyword argument for "
                 f"{self.__class__.__name__}",
             )
@@ -848,19 +848,126 @@
                 x * multiplier if x < 4096 else None
                 for x in raw[row*self.WIDTH:(row+1)*self.WIDTH]
             ]
             for row in reversed(range(self.HEIGHT))
         ]
 
 
+class CAPParser(Parser):
+
+    ns = {
+        'cap': 'urn:oasis:names:tc:emergency:cap:1.2',
+    }
+
+    TAG_MAP = {
+        'de': {
+            'event': 'event_de',
+            'headline': 'headline_de',
+            'description': 'description_de',
+            'instruction': 'instruction_de',
+        },
+        'en': {
+            'event': 'event_en',
+            'headline': 'headline_en',
+            'description': 'description_en',
+            'instruction': 'instruction_en',
+            'category': 'category',
+            'responseType': 'response_type',
+            'urgency': 'urgency',
+            'severity': 'severity',
+            'certainty': 'certainty',
+            'effective': 'effective',
+            'onset': 'onset',
+            'expires': 'expires',
+        }
+    }
+    OPTIONAL_FIELDS = [
+        'expires',
+    ]
+    TOKEN_FIELDS = [
+        'category',
+        'certainty',
+        'response_type',
+        'severity',
+        'urgency',
+    ]
+    TIMESTAMP_FIELDS = [
+        'effective',
+        'onset',
+        'expires',
+    ]
+
+    def parse(self, path):
+        self.logger.info("Parsing %s", path)
+        with zipfile.ZipFile(path) as zf:
+            for info in zf.infolist():
+                with zf.open(info) as f:
+                    yield self.parse_event(f)
+
+    def parse_event(self, f):
+        event = {}
+        for _, element in ET.iterparse(f):
+            if self._is_tag(element, 'cap:info'):
+                self._parse_info(event, element)
+                element.clear()
+            elif self._is_tag(element, 'cap:alert'):
+                event['id'] = element.find(
+                    'cap:identifier',
+                    self.ns,
+                ).text.rsplit('.', 1)[0]
+        self.sanitize_event(event)
+        return event
+
+    def _parse_info(self, event, element):
+        lang = element.find('cap:language', self.ns).text.split('-')[0]
+        tag_map = self.TAG_MAP.get(lang, {})
+        for tag, field in tag_map.items():
+            e = element.find(f'cap:{tag}', self.ns)
+            if e is not None:
+                event[field] = e.text
+            elif field in self.OPTIONAL_FIELDS:
+                event[field] = None
+            else:
+                raise ValueError("Unable to find <%s>" % tag)
+        if 'event_code' not in event:
+            event['event_code'] = self._parse_event_code(element)
+        if 'warn_cell_ids' not in event:
+            event['warn_cell_ids'] = list(self._parse_warn_cell_ids(element))
+
+    def _is_tag(self, element, tag):
+        prefix, tag = tag.split(':')
+        return element.tag == f'{{{self.ns[prefix]}}}{tag}'
+
+    def _parse_event_code(self, element):
+        for ec_element in element.findall('cap:eventCode', self.ns):
+            if ec_element.find('cap:valueName', self.ns).text == 'II':
+                return int(ec_element.find('cap:value', self.ns).text)
+
+    def _parse_warn_cell_ids(self, element):
+        for gc_element in element.findall('cap:area/cap:geocode', self.ns):
+            if gc_element.find('cap:valueName', self.ns).text == 'WARNCELLID':
+                yield int(gc_element.find('cap:value', self.ns).text)
+
+    def sanitize_event(self, event):
+        for field in self.TOKEN_FIELDS:
+            if event[field] is None:
+                continue
+            event[field] = event[field].lower()
+        for field in self.TIMESTAMP_FIELDS:
+            if event[field] is None:
+                continue
+            event[field] = datetime.datetime.fromisoformat(event[field])
+
+
 def get_parser(filename):
     parsers = {
         r'DE1200_RV': RADOLANParser,
         r'MOSMIX_(S|L)_LATEST(_240)?\.kmz$': MOSMIXParser,
         r'Z__C_EDZW_\d+_.*\.json\.bz2$': SYNOPParser,
+        r'Z_CAP_.*\.zip': CAPParser,
         r'\w{5}-BEOB\.csv$': CurrentObservationsParser,
         'stundenwerte_FF_': WindObservationsParser,
         'stundenwerte_N_': CloudCoverObservationsParser,
         'stundenwerte_P0_': PressureObservationsParser,
         'stundenwerte_RR_': PrecipitationObservationsParser,
         'stundenwerte_SD_': SunshineObservationsParser,
         'stundenwerte_TD_': DewPointObservationsParser,
```

### Comparing `dwdparse-0.9.6/dwdparse/stations.py` & `dwdparse-0.9.7/dwdparse/stations.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.6/dwdparse/units.py` & `dwdparse-0.9.7/dwdparse/units.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.6/dwdparse.egg-info/PKG-INFO` & `dwdparse-0.9.7/dwdparse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwdparse
-Version: 0.9.6
+Version: 0.9.7
 Summary: Parsers for DWD's open weather data.
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/
 Project-URL: Tracker, https://github.com/jdemaeyer/dwdparse/issues/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dwdparse Version: 0.9.6 Summary: Parsers for DWD's
+Metadata-Version: 2.1 Name: dwdparse Version: 0.9.7 Summary: Parsers for DWD's
 open weather data. Author: Jakob de Maeyer Author-email: jakob@naboa.de
 Project-URL: Source, https://github.com/jdemaeyer/dwdparse/ Project-URL:
 Tracker, https://github.com/jdemaeyer/dwdparse/issues/ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.8
 Description-Content-Type: text/markdown Provides-Extra: lean License-File:
 LICENSE # dwdparse [![Build Status](https://img.shields.io/github/actions/
```

### Comparing `dwdparse-0.9.6/setup.py` & `dwdparse-0.9.7/setup.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.6/tests/test_parsers.py` & `dwdparse-0.9.7/tests/test_parsers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import datetime
 
 from dwdparse.parsers import (
+    CAPParser,
     CloudCoverObservationsParser,
     CurrentObservationsParser,
     DewPointObservationsParser,
     MOSMIXParser,
     PrecipitationObservationsParser,
     PressureObservationsParser,
     RADOLANParser,
@@ -434,20 +435,63 @@
         [ .02,  .03,  .03,    0,    0],  # noqa: E201
         [ .03,  .04,  .01,    0,  .03],  # noqa: E201
         [None,  .08,    0,    0,    0],
         [None, None, None, None, None],
     ]
 
 
+def test_cap_parser(data_dir):
+    p = CAPParser()
+    fn = 'Z_CAP_C_EDZW_LATEST_PVW_STATUS_PREMIUMDWD_COMMUNEUNION_MUL.zip'
+    records = list(p.parse(data_dir / fn))
+    expected_ids = set(
+        f'2.49.0.0.276.0.DWD.PVW.{suffix}'
+        for suffix in [
+            '1687514160000.20999218-5d5e-4761-b271-6c243f695568',
+            '1687511640000.0d1a4fb5-251a-46fc-aae3-a688d2021e71',
+            '1687470000000.fe90b61b-3755-4efb-8eda-b161251da9f7',
+        ]
+    )
+    assert len(records) == 3
+    assert set(r['id'] for r in records) == expected_ids
+    assert records[1] == {
+        'id': '2.49.0.0.276.0.DWD.PVW.1687511640000.0d1a4fb5-251a-46fc-aae3-a688d2021e71',  # noqa
+        'event_de': 'STARKREGEN',
+        'headline_de': 'Amtliche WARNUNG vor STARKREGEN',
+        'description_de': 'Es tritt Starkregen auf. Dabei werden Niederschlagsmengen zwischen 20 l/m² und 30 l/m² in 6 Stunden erwartet.',  # noqa
+        'instruction_de': 'ACHTUNG! Hinweis auf mögliche Gefahren: Während des Platzregens sind kurzzeitig Verkehrsbehinderungen möglich.',  # noqa
+        'event_code': 61,
+        'warn_cell_ids': [
+          812069270,
+          812063189,
+          812069018
+        ],
+        'event_en': 'heavy rain',
+        'headline_en': 'Official WARNING of HEAVY RAIN',
+        'description_en': 'There is a risk of heavy rain (Level 2 of 4).\nPrecipitation amounts: 20-30 l/m²/6h',  # noqa
+        'instruction_en': 'NOTE: Be aware of the following possible dangers: The downpours can cause temporary traffic disruption.',  # noqa
+        'category': 'met',
+        'response_type': 'prepare',
+        'urgency': 'immediate',
+        'severity': 'moderate',
+        'certainty': 'likely',
+        'effective': datetime.datetime(2023, 6, 23, 9, 14, tzinfo=utc),
+        'onset': datetime.datetime(2023, 6, 23, 9, 14, tzinfo=utc),
+        'expires': datetime.datetime(2023, 6, 23, 13, 0, tzinfo=utc),
+    }
+
+
 def test_get_parser():
     synop_with_timestamp = (
         'Z__C_EDZW_20200617114802_bda01,synop_bufr_GER_999999_999999__MW_617'
         '.json.bz2')
     synop_latest = (
         'Z__C_EDZW_latest_bda01,synop_bufr_GER_999999_999999__MW_XXX.json.bz2')
+    cap_latest = (
+        'Z_CAP_C_EDZW_LATEST_PVW_STATUS_PREMIUMDWD_COMMUNEUNION_MUL.zip')
     expected = {
         '10minutenwerte_extrema_wind_00427_akt.zip': (
             WindGustsObservationsParser),
         '10minutenwerte_SOLAR_01766_now.zip': SolarRadiationObservationsParser,
         'stundenwerte_FF_00011_akt.zip': WindObservationsParser,
         'stundenwerte_FF_00090_akt.zip': WindObservationsParser,
         'stundenwerte_N_01766_akt.zip': CloudCoverObservationsParser,
@@ -458,10 +502,11 @@
         'stundenwerte_TU_00161_akt.zip': TemperatureObservationsParser,
         'stundenwerte_VV_00161_akt.zip': VisibilityObservationsParser,
         'MOSMIX_S_LATEST_240.kmz': MOSMIXParser,
         'DE1200_RV2305081330.tar.bz2': RADOLANParser,
         'K611_-BEOB.csv': CurrentObservationsParser,
         synop_with_timestamp: SYNOPParser,
         synop_latest: None,
+        cap_latest: CAPParser,
     }
     for filename, expected_parser in expected.items():
         assert get_parser(filename) is expected_parser
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dwdparse-0.9.6/tests/test_stations.py` & `dwdparse-0.9.7/tests/test_stations.py`

 * *Files identical despite different names*

### Comparing `dwdparse-0.9.6/tests/test_units.py` & `dwdparse-0.9.7/tests/test_units.py`

 * *Files identical despite different names*

