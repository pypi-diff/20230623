# Comparing `tmp/brightsky-2.0.5.tar.gz` & `tmp/brightsky-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brightsky-2.0.5.tar", last modified: Mon Jun 12 10:08:20 2023, max compression
+gzip compressed data, was "brightsky-2.0.6.tar", last modified: Fri Jun 23 12:40:59 2023, max compression
```

## Comparing `brightsky-2.0.5.tar` & `brightsky-2.0.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:08:20.388107 brightsky-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-12 10:08:11.000000 brightsky-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-12 10:08:20.388107 brightsky-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-06-12 10:08:11.000000 brightsky-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:08:20.384106 brightsky-2.0.5/brightsky/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/db.py
--rw-r--r--   0 runner    (1001) docker     (123)     9369 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     6950 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13624 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13410 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-12 10:08:11.000000 brightsky-2.0.5/brightsky/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:08:20.388107 brightsky-2.0.5/brightsky.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-12 10:08:20.000000 brightsky-2.0.5/brightsky.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-12 10:08:20.000000 brightsky-2.0.5/brightsky.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 10:08:20.000000 brightsky-2.0.5/brightsky.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-12 10:08:20.000000 brightsky-2.0.5/brightsky.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-12 10:08:20.000000 brightsky-2.0.5/brightsky.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-12 10:08:11.000000 brightsky-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 10:08:20.388107 brightsky-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-12 10:08:11.000000 brightsky-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 10:08:20.388107 brightsky-2.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_polling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-06-12 10:08:11.000000 brightsky-2.0.5/tests/test_web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:40:59.265739 brightsky-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-23 12:40:53.000000 brightsky-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-23 12:40:59.265739 brightsky-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-06-23 12:40:53.000000 brightsky-2.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:40:59.261739 brightsky-2.0.6/brightsky/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4898 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-23 12:40:53.000000 brightsky-2.0.6/brightsky/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:40:59.261739 brightsky-2.0.6/brightsky.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-23 12:40:59.000000 brightsky-2.0.6/brightsky.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-23 12:40:59.000000 brightsky-2.0.6/brightsky.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-23 12:40:59.000000 brightsky-2.0.6/brightsky.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-23 12:40:59.000000 brightsky-2.0.6/brightsky.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-23 12:40:59.000000 brightsky-2.0.6/brightsky.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-23 12:40:53.000000 brightsky-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-23 12:40:59.265739 brightsky-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-23 12:40:53.000000 brightsky-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-23 12:40:59.265739 brightsky-2.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22552 2023-06-23 12:40:53.000000 brightsky-2.0.6/tests/test_web.py
```

### Comparing `brightsky-2.0.5/LICENSE` & `brightsky-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.5/PKG-INFO` & `brightsky-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.5
+Version: 2.0.6
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.0.5/README.md` & `brightsky-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.5/brightsky/cli.py` & `brightsky-2.0.6/brightsky/cli.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.5/brightsky/db.py` & `brightsky-2.0.6/brightsky/db.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.5/brightsky/export.py` & `brightsky-2.0.6/brightsky/export.py`

 * *Files 25% similar despite different names*

```diff
@@ -81,14 +81,15 @@
 
     def export(self, records, fingerprint=None):
         with get_connection() as conn:
             for batch in batched(records, self.BATCH_SIZE):
                 self.export_batch(conn, batch)
             if fingerprint:
                 self.update_parsed_files(conn, fingerprint)
+            conn.commit()
 
     def export_batch(self, conn, batch):
         records = self.prepare_records(batch)
         sources = self.prepare_sources(batch)
         source_map = self.update_sources(conn, sources)
         self.map_source_ids(records, source_map)
         self.update_weather(conn, records)
@@ -269,7 +270,136 @@
         'precipitation_5',
         'source',
     ]
 
     def export_batch(self, conn, batch):
         records = self.prepare_records(batch)
         self.update_weather(conn, records)
+
+
+class AlertExporter(DBExporter):
+
+    UPDATE_ALERTS_STMT = sql.SQL("""
+        INSERT INTO alerts ({fields})
+        VALUES %s
+        ON CONFLICT
+            ON CONSTRAINT alerts_key DO UPDATE SET
+                {conflict_updates}
+        RETURNING id;
+    """)
+    UPDATE_ALERTS_CLEANUP = """
+        SELECT setval(
+            'alerts_id_seq',
+            GREATEST(%(max_id)s, (SELECT max(id) FROM alerts))
+        );
+    """
+    ELEMENT_FIELDS = [
+        'alert_id',
+        'effective',
+        'onset',
+        'expires',
+        'category',
+        'response_type',
+        'urgency',
+        'severity',
+        'certainty',
+        'event_code',
+        'event_en',
+        'event_de',
+        'headline_en',
+        'headline_de',
+        'description_en',
+        'description_de',
+        'instruction_en',
+        'instruction_de',
+    ]
+
+    def export(self, alerts, fingerprint=None):
+        alerts = list(alerts)
+        self.prepare_alerts(alerts)
+        with get_connection() as conn:
+            last_id = self.get_last_alert_id(conn)
+            self.clear_outdated_alerts(conn, alerts)
+            self.update_alerts(conn, alerts)
+            self.reset_alert_id(conn, last_id)
+            self.update_alert_cells(conn, alerts)
+            if fingerprint:
+                self.update_parsed_files(conn, fingerprint)
+            conn.commit()
+
+    def prepare_alerts(self, alerts):
+        for a in alerts:
+            a['alert_id'] = a.pop('id')
+
+    def get_last_alert_id(self, conn):
+        with conn.cursor() as cur:
+            cur.execute("SELECT MAX(id) FROM alerts")
+            return cur.fetchall()[0]['max']
+
+    def clear_outdated_alerts(self, conn, alerts):
+        with conn.cursor() as cur:
+            cur.execute("SELECT alert_id FROM alerts")
+            existing = set(row['alert_id'] for row in cur.fetchall())
+            outdated = existing.difference(a['alert_id'] for a in alerts)
+            if outdated:
+                logger.info("Deleting %d outdated alerts", len(outdated))
+                cur.execute(
+                    "DELETE FROM alerts WHERE alert_id IN %(outdated)s",
+                    {'outdated': tuple(outdated)},
+                )
+
+    def update_alerts(self, conn, alerts):
+        for fields, alerts in self.make_batches(alerts).items():
+            logger.info(
+                "Exporting %d alerts with fields %s",
+                len(alerts),
+                tuple(fields),
+            )
+            conflict_updates = sql.SQL(', ').join(
+                sql.SQL('{field} = EXCLUDED.{field}').format(
+                    field=sql.Identifier(f),
+                )
+                for f in fields
+            )
+            stmt = self.UPDATE_ALERTS_STMT.format(
+                fields=sql.SQL(', ').join(sql.Identifier(f) for f in fields),
+                conflict_updates=conflict_updates,
+            )
+            template = sql.SQL(
+                '({values})',
+            ).format(
+                values=sql.SQL(', ').join(
+                    sql.Placeholder(f) for f in fields
+                ),
+            )
+            with conn.cursor() as cur:
+                rows = execute_values(
+                    cur,
+                    stmt,
+                    alerts,
+                    template,
+                    page_size=1000,
+                    fetch=True,
+                )
+            for row, alert in zip(rows, alerts, strict=True):
+                alert['id'] = row['id']
+
+    def reset_alert_id(self, conn, max_id):
+        if max_id is None:
+            return
+        with conn.cursor() as cur:
+            cur.execute(self.UPDATE_ALERTS_CLEANUP, {'max_id': max_id})
+
+    def update_alert_cells(self, conn, alerts):
+        rows = [
+            (alert['id'], wcid)
+            for alert in alerts
+            for wcid in alert['warn_cell_ids']
+        ]
+        with conn.cursor() as cur:
+            cur.execute("DELETE FROM alert_cells")
+            execute_values(
+                cur,
+                "INSERT INTO alert_cells (alert_id, warn_cell_id) VALUES %s",
+                rows,
+                page_size=1000,
+            )
```

### Comparing `brightsky-2.0.5/brightsky/parsers.py` & `brightsky-2.0.6/brightsky/parsers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 
 import dwdparse.parsers
 import numpy as np
 from dateutil.tz import tzutc
 from isal import isal_zlib as zlib
 
 from brightsky.db import fetch
-from brightsky.export import DBExporter, RADOLANExporter, SYNOPExporter
+from brightsky.export import (
+    AlertExporter,
+    DBExporter,
+    RADOLANExporter,
+    SYNOPExporter,
+)
 from brightsky.settings import settings
 
 
 class BrightSkyMixin:
 
     PRIORITY = 10
     exporter = DBExporter
@@ -203,18 +208,24 @@
         #      we are replacing `None` with `0`!
         data = np.array(raw, dtype='i2')
         data[data > 4095] = 0
         data = np.flipud(data.reshape((1200, 1100)))
         return zlib.compress(np.ascontiguousarray(data))
 
 
+class CAPParser(BrightSkyMixin, dwdparse.parsers.CAPParser):
+
+    exporter = AlertExporter
+
+
 def get_parser(filename):
     parsers = {
         r'DE1200_RV': RADOLANParser,
         r'MOSMIX_(S|L)_LATEST(_240)?\.kmz$': MOSMIXParser,
+        r'Z_CAP_C_EDZW_LATEST_.*_COMMUNEUNION_MUL\.zip': CAPParser,
         r'Z__C_EDZW_\d+_.*\.json\.bz2$': SYNOPParser,
         r'\w{5}-BEOB\.csv$': CurrentObservationsParser,
         'stundenwerte_FF_': WindObservationsParser,
         'stundenwerte_N_': CloudCoverObservationsParser,
         'stundenwerte_P0_': PressureObservationsParser,
         'stundenwerte_RR_': PrecipitationObservationsParser,
         'stundenwerte_SD_': SunshineObservationsParser,
```

### Comparing `brightsky-2.0.5/brightsky/polling.py` & `brightsky-2.0.6/brightsky/polling.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 class DWDPoller:
 
     urls = [
         'https://opendata.dwd.de/weather/local_forecasts/mos/MOSMIX_L/'
         'all_stations/kml/',
         'https://opendata.dwd.de/weather/local_forecasts/mos/MOSMIX_S/'
         'all_stations/kml/',
+        'https://opendata.dwd.de/weather/alerts/cap/COMMUNEUNION_DWD_STAT/',
         'https://opendata.dwd.de/weather/radar/composite/rv/',
         'https://opendata.dwd.de/weather/weather_reports/synoptic/germany/'
         'json/',
         'https://opendata.dwd.de/weather/weather_reports/poi/',
     ] + [
         'https://opendata.dwd.de/climate_environment/CDC/observations_germany/'
         f'climate/hourly/{subfolder}/'
```

### Comparing `brightsky-2.0.5/brightsky/query.py` & `brightsky-2.0.6/brightsky/query.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 import datetime
+import json
+import os
+import tempfile
 from functools import cached_property
 
 import numpy as np
+import requests
 from dateutil.tz import tzutc
 from isal import isal_zlib as zlib
 from pyproj import CRS, Transformer
+from shapely import MultiPolygon, STRtree, Point
 
 from brightsky.db import fetch
+from brightsky.settings import settings
+from brightsky.utils import USER_AGENT
 
 
 def _make_dicts(rows):
     return [dict(row) for row in rows]
 
 
 def weather(
@@ -313,14 +320,102 @@
             ],
         }
 
 
 _transformer = RadarCoordinatesTransformer()
 
 
+def alerts(lat=None, lon=None, warn_cell_id=None):
+    if lat is not None and lon is not None:
+        meta = _warn_cells.find(lat, lon)
+    elif warn_cell_id is not None:
+        try:
+            meta = _warn_cells.get_meta(warn_cell_id)
+        except KeyError:
+            raise LookupError(
+                "Unknown warn_cell_id, please use commune (Gemeinden), not "
+                "district (Landkreis) ids"
+            )
+    else:
+        raise ValueError("Please supply lat/lon or warn_cell_id")
+    sql = """
+        SELECT *
+        FROM alerts
+        WHERE id IN (
+            SELECT alert_id
+            FROM alert_cells
+            WHERE warn_cell_id = %(warn_cell_id)s
+        )
+        ORDER BY severity DESC
+        """
+    params = {
+        'warn_cell_id': meta['warn_cell_id'],
+    }
+    rows = fetch(sql, params)
+    return {
+        'alerts': _make_dicts(rows),
+        'location': meta,
+    }
+
+
+class WarnCellManager:
+
+    CELLS_CACHE_PATH = os.path.join(tempfile.gettempdir(), 'alert_cells.json')
+
+    @cached_property
+    def tree(self):
+        self.cell_meta = {}
+        self.cell_meta_by_id = {}
+        for f in self.get_cell_data()['features']:
+            polygons = [
+                # shell, holes
+                (c[0], c[1:])
+                for c in f['geometry']['coordinates']
+            ]
+            p = MultiPolygon(polygons)
+            meta = {
+                'warn_cell_id': f['properties']['WARNCELLID'],
+                'name': f['properties']['NAME'],
+                'name_short': f['properties']['KURZNAME'],
+                'district': f['properties']['KREIS'],
+                'state': f['properties']['BUNDESLAND'],
+                'state_short': f['properties']['BL_KUERZEL'],
+            }
+            self.cell_meta[p] = meta
+            self.cell_meta_by_id[meta['warn_cell_id']] = meta
+        return STRtree(list(self.cell_meta.keys()))
+
+    def get_cell_data(self):
+        path = self.CELLS_CACHE_PATH
+        if not os.path.isfile(path):
+            resp = requests.get(
+                settings.WARN_CELLS_URL,
+                headers={'User-Agent': USER_AGENT},
+            )
+            with open(path, 'wb') as f:
+                f.write(resp.content)
+        with open(path) as f:
+            return json.load(f)
+
+    def find(self, lat, lon):
+        p = Point(lon, lat)
+        cell = self.tree.geometries[self.tree.nearest(p)]
+        if cell.distance(p) > 0.01:
+            raise LookupError("Requested position is not covered by the DWD")
+        return self.cell_meta[cell]
+
+    def get_meta(self, warn_cell_id):
+        # Make sure cells have been parsed
+        self.tree
+        return self.cell_meta_by_id[warn_cell_id]
+
+
+_warn_cells = WarnCellManager()
+
+
 def sources(
         lat=None, lon=None, dwd_station_id=None, wmo_station_id=None,
         source_id=None, observation_types=None, max_dist=50000,
         ignore_type=False, date=None, last_date=None):
     select = "*"
     order_by = "observation_type"
     params = {
```

### Comparing `brightsky-2.0.5/brightsky/settings.py` & `brightsky-2.0.6/brightsky/settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 ICON_WIND_THRESHOLD = 10.8
 IGNORED_CURRENT_OBSERVATIONS_STATIONS = ['K386']
 KEEP_DOWNLOADS = False
 MIN_DATE = datetime.datetime(2010, 1, 1, tzinfo=tzutc())
 MAX_DATE = None
 POLLING_CRONTAB_MINUTE = '*'
 REDIS_URL = 'redis://localhost'
+WARN_CELLS_URL = (
+    'https://maps.dwd.de/geoserver/wfs'
+    '?SERVICE=WFS&VERSION=2.0.0&REQUEST=GetFeature'
+    '&TYPENAMES=Warngebiete_Gemeinden&OUTPUTFORMAT=json'
+)
 
 
 def _make_bool(bool_str):
     return bool_str == '1'
 
 
 def _make_date(date_str):
```

### Comparing `brightsky-2.0.5/brightsky/tasks.py` & `brightsky-2.0.6/brightsky/tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.5/brightsky/utils.py` & `brightsky-2.0.6/brightsky/utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.5/brightsky/web.py` & `brightsky-2.0.6/brightsky/web.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,14 +296,32 @@
                     "The 'bbox' parameter must be a comma-separated list of "
                     "four integers: top, left, bottom, right (edges are "
                     "inclusive)."
                 )
                 raise falcon.HTTPBadRequest(description=description)
 
 
+class AlertsResource(BrightskyResource):
+
+    def on_get(self, req, resp):
+        lat, lon = self.parse_location(req)
+        warn_cell_id = req.get_param_as_int('warn_cell_id')
+        timezone = self.parse_timezone(req)
+        with convert_exceptions():
+            result = query.alerts(
+                lat=lat,
+                lon=lon,
+                warn_cell_id=warn_cell_id,
+            )
+        for row in result['alerts']:
+            for key in ['effective', 'onset', 'expires']:
+                self.process_timestamp(row, key, timezone)
+        resp.media = result
+
+
 class SourcesResource(BrightskyResource):
 
     def on_get(self, req, resp):
         lat, lon = self.parse_location(req)
         max_dist = self.parse_max_dist(req)
         source_id, dwd_station_id, wmo_station_id = self.parse_source_ids(req)
         with convert_exceptions():
@@ -356,14 +374,15 @@
         ),
     )
     app.add_route('/', StatusResource())
     app.add_route('/weather', WeatherResource())
     app.add_route('/current_weather', CurrentWeatherResource())
     app.add_route('/synop', SynopResource())
     app.add_route('/radar', RadarResource())
+    app.add_route('/alerts', AlertsResource())
     app.add_route('/sources', SourcesResource())
     return app
 
 
 app = make_app()
```

### Comparing `brightsky-2.0.5/brightsky/worker.py` & `brightsky-2.0.6/brightsky/worker.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.5/brightsky.egg-info/PKG-INFO` & `brightsky-2.0.6/brightsky.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brightsky
-Version: 2.0.5
+Version: 2.0.6
 Summary: JSON API for DWD's open weather data.
 Home-page: https://brightsky.dev/
 Author: Jakob de Maeyer
 Author-email: jakob@naboa.de
 Project-URL: Documentation, https://brightsky.dev/docs/
 Project-URL: Source, https://github.com/jdemaeyer/brightsky/
 Project-URL: Tracker, https://github.com/jdemaeyer/brightsky/issues/
```

### Comparing `brightsky-2.0.5/brightsky.egg-info/SOURCES.txt` & `brightsky-2.0.6/brightsky.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.5/setup.py` & `brightsky-2.0.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,9 +41,10 @@
         'parsel',
         'psycopg2-binary',
         'pyproj',
         'python-dateutil',
         'redis',
         'requests',
         'sentry-sdk',
+        'shapely',
     ],
 )
```

### Comparing `brightsky-2.0.5/tests/test_export.py` & `brightsky-2.0.6/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.5/tests/test_parsers.py` & `brightsky-2.0.6/tests/test_parsers.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.5/tests/test_polling.py` & `brightsky-2.0.6/tests/test_polling.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.5/tests/test_settings.py` & `brightsky-2.0.6/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.5/tests/test_tasks.py` & `brightsky-2.0.6/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.5/tests/test_utils.py` & `brightsky-2.0.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `brightsky-2.0.5/tests/test_web.py` & `brightsky-2.0.6/tests/test_web.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 import falcon
 import numpy as np
 import pytest
 from dateutil.tz import tzutc
 
 import brightsky
-from brightsky.export import DBExporter, RADOLANExporter, SYNOPExporter
-from brightsky.parsers import RADOLANParser
+from brightsky.export import DBExporter, SYNOPExporter
+from brightsky.parsers import CAPParser, RADOLANParser
+from brightsky.query import _warn_cells
 from brightsky.web import make_app
 
 from .utils import settings
 
 
 SOURCES = [
     # Ordered by their distance to (52, 7.6)
@@ -212,15 +213,23 @@
 def synop_data(db):
     SYNOPExporter().export(SYNOP_RECORDS)
 
 
 @pytest.fixture
 def radar_data(db, data_dir):
     p = RADOLANParser()
-    RADOLANExporter().export(p.parse(data_dir / 'DE1200_RV2305081330.tar.bz2'))
+    p.exporter().export(p.parse(data_dir / 'DE1200_RV2305081330.tar.bz2'))
+
+
+@pytest.fixture
+def alerts_data(db, data_dir):
+    p = CAPParser()
+    fn = 'Z_CAP_C_EDZW_LATEST_PVW_STATUS_PREMIUMDWD_COMMUNEUNION_MUL.zip'
+    p.exporter().export(p.parse(data_dir / fn))
+    _warn_cells.CELLS_CACHE_PATH = data_dir / 'alert_cells.json'
 
 
 def test_sources_required_parameters(data, api):
     assert api.simulate_get('/sources').status_code == 400
     assert api.simulate_get('/sources?lat=52').status_code == 400
     assert api.simulate_get('/sources?lon=7.6').status_code == 400
     assert api.simulate_get('/sources?lat=52&lon=7.6').status_code == 200
@@ -576,14 +585,52 @@
     for p, exp_p in zip(resp.json['geometry']['coordinates'], expected_coords):
         assert p[0] == pytest.approx(exp_p[0])
         assert p[1] == pytest.approx(exp_p[1])
     assert resp.json['latlon_position']['x'] == pytest.approx(14.326)
     assert resp.json['latlon_position']['y'] == pytest.approx(200.489)
 
 
+def test_alerts_response(alerts_data, api):
+    expected_ids = [
+        '2.49.0.0.276.0.DWD.PVW.1687514160000.'
+        '20999218-5d5e-4761-b271-6c243f695568',
+        '2.49.0.0.276.0.DWD.PVW.1687470000000.'
+        'fe90b61b-3755-4efb-8eda-b161251da9f7',
+    ]
+    # Query by lat/lon
+    resp = api.simulate_get('/alerts?lat=51.55&lon=9.9')
+    assert [
+        alert['alert_id'] for alert in resp.json['alerts']
+    ] == expected_ids
+    assert resp.json['location'] == {
+        'warn_cell_id': 803159016,
+        'name': 'Stadt Göttingen',
+        'name_short': 'Göttingen',
+        'district': 'Göttingen',
+        'state': 'Niedersachsen',
+        'state_short': 'NI',
+    }
+    # Query by warn cell id
+    resp = api.simulate_get('/alerts?warn_cell_id=803159016')
+    assert len(resp.json['alerts']) == 2
+    # Query by lat/lon, no alerts
+    resp = api.simulate_get('/alerts?lat=52&lon=7.6')
+    assert resp.status_code == 200
+    assert not resp.json['alerts']
+    assert resp.json['location']['name'] == 'Münster-Nord'
+    # Query by warn_cell_id, no alerts
+    resp = api.simulate_get('/alerts?warn_cell_id=705515101')
+    assert not resp.json['alerts']
+    # Query by lat/lon, outside of covered area
+    resp = api.simulate_get('/alerts?lat=32&lon=7.6')
+    assert resp.status_code == 404
+    resp = api.simulate_get('/alerts?warn_cell_id=0')
+    assert resp.status_code == 404
+
+
 def test_status_response(api):
     resp = api.simulate_get('/')
     assert resp.status_code == 200
     assert resp.json['name'] == 'brightsky'
     assert resp.json['version'] == brightsky.__version__
     assert resp.json['status'] == 'ok'
```

