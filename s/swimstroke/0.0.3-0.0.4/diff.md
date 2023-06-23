# Comparing `tmp/swimstroke-0.0.3-py3-none-any.whl.zip` & `tmp/swimstroke-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 8453 bytes, number of entries: 14
--rw-r--r--  2.0 unx       23 b- defN 23-Jun-18 05:24 swimstroke/__init__.py
--rw-r--r--  2.0 unx      657 b- defN 23-Jun-18 05:24 swimstroke/__main__.py
--rw-r--r--  2.0 unx     3793 b- defN 23-Jun-18 05:24 swimstroke/ev3.py
--rw-r--r--  2.0 unx     5945 b- defN 23-Jun-18 05:24 swimstroke/helpers.py
--rw-r--r--  2.0 unx    13053 b- defN 23-Jun-18 05:24 swimstroke/hy3.py
--rw-r--r--  2.0 unx       86 b- defN 23-Jun-18 05:24 swimstroke/scb.py
--rw-r--r--  2.0 unx       47 b- defN 23-Jun-18 05:24 swimstroke/sd3.py
--rw-r--r--  2.0 unx      586 b- defN 23-Jun-18 05:24 swimstroke/util.py
--rw-r--r--  2.0 unx       47 b- defN 23-Jun-18 05:24 swimstroke/yaml.py
--rw-rw-rw-  2.0 unx     1103 b- defN 23-Jun-18 05:25 swimstroke-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx       77 b- defN 23-Jun-18 05:25 swimstroke-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-18 05:25 swimstroke-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-Jun-18 05:25 swimstroke-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1072 b- defN 23-Jun-18 05:25 swimstroke-0.0.3.dist-info/RECORD
-14 files, 26592 bytes uncompressed, 6681 bytes compressed:  74.9%
+Zip file size: 8562 bytes, number of entries: 14
+-rw-r--r--  2.0 unx       23 b- defN 23-Jun-23 09:29 swimstroke/__init__.py
+-rw-r--r--  2.0 unx      715 b- defN 23-Jun-23 09:29 swimstroke/__main__.py
+-rw-r--r--  2.0 unx     3793 b- defN 23-Jun-23 09:29 swimstroke/ev3.py
+-rw-r--r--  2.0 unx     6024 b- defN 23-Jun-23 09:29 swimstroke/helpers.py
+-rw-r--r--  2.0 unx    13349 b- defN 23-Jun-23 09:29 swimstroke/hy3.py
+-rw-r--r--  2.0 unx       86 b- defN 23-Jun-23 09:29 swimstroke/scb.py
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-23 09:29 swimstroke/sd3.py
+-rw-r--r--  2.0 unx      586 b- defN 23-Jun-23 09:29 swimstroke/util.py
+-rw-r--r--  2.0 unx       47 b- defN 23-Jun-23 09:29 swimstroke/yaml.py
+-rw-rw-rw-  2.0 unx     1103 b- defN 23-Jun-23 09:29 swimstroke-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx       77 b- defN 23-Jun-23 09:29 swimstroke-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 09:29 swimstroke-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Jun-23 09:29 swimstroke-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1072 b- defN 23-Jun-23 09:29 swimstroke-0.0.4.dist-info/RECORD
+14 files, 27025 bytes uncompressed, 6790 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: swimstroke/util.py
 Comment: 
 
 Filename: swimstroke/yaml.py
 Comment: 
 
-Filename: swimstroke-0.0.3.dist-info/LICENSE
+Filename: swimstroke-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: swimstroke-0.0.3.dist-info/METADATA
+Filename: swimstroke-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: swimstroke-0.0.3.dist-info/WHEEL
+Filename: swimstroke-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: swimstroke-0.0.3.dist-info/top_level.txt
+Filename: swimstroke-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: swimstroke-0.0.3.dist-info/RECORD
+Filename: swimstroke-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## swimstroke/__main__.py

```diff
@@ -1,16 +1,17 @@
 import sys
-from .helpers import load, get_events
+from .helpers import load, get_events, populate_heats
 from .util import swimtimefmt
 
 meetinfo = load(sys.argv[1])
 #print(repr(meetinfo.))
 
 for event in get_events(meetinfo):
-    print(event['event_number'],event['stroke'],event['distance'],event['course'],event['date'])
+    populate_heats(event)
+    print(event['event_number'],event['gender'],event['stroke'],event['distance'],event['course'],event['date'])
     for entry in event['entries']:
         #print(repr(entry))
         if entry['relay']:
             print(" * relay - ",entry['heat'],entry['lane'],entry['teamname'],', '.join([e['name'] for e in entry['swimmers']]),entry['event_type'])
         else:
             print(" * ",entry['heat'],entry['lane'],entry['swimmers'][0]['name'],swimtimefmt(entry['seed_time_ms']),entry['event_type'])
```

## swimstroke/helpers.py

```diff
@@ -52,15 +52,17 @@
     # pad some 0s on the event_str to make a lexicographic sort possible
     event_str = event['event']
     while len(event_str)<6:
         event_str = "0"+event_str
     return event_prefix+"-"+event_str
 
 def _event_key_from_entry(entry):
-    if entry['event_type'] is None:
+    if 'event_type' not in entry:
+        event_prefix="0"
+    elif entry['event_type'] is None:
         event_prefix="A"
     elif entry['event_type']=='Prelim':
         event_prefix="B"
     elif entry['event_type']=="Final":
         event_prefix="C"
 
     # pad some 0s on the event_str to make a lexicographic sort possible
@@ -81,24 +83,24 @@
                 swimmers_by_code[swimmer['swimmer_code']] = swimmer
             for entry in team['entries']:
                 event_key = _event_key_from_entry(entry)
                 if event_key not in events_by_key:
                     events_by_key[event_key] = {
                         "event":entry['event_str'],
                         "event_number":int(entry['event']),
-                        "date":entry['event_date'],
+                        "date":entry.get('event_date',None),
                         "gender":entry['event_gender'],
                         "gendercode":entry['event_gendercode'],
                         "course":entry['event_course'],
                         "coursecode":entry['event_coursecode'],
                         "stroke":entry['stroke'],
                         "strokeshort":entry['strokeshort'],
                         "distance":entry['distance'],
                         "relay":entry['relay'],
-                        "type":entry['event_type'],
+                        "type":entry.get('event_type',None),
                         "entries":[],
                         "num_heats":None
                     }
                     event = events_by_key[event_key]
                     name = "%s %d %s"%(event['gender'],event['distance'],event['strokeshort'])
                     if entry['relay']:
                         name += " Relay"
```

## swimstroke/hy3.py

```diff
@@ -17,14 +17,15 @@
     "E":"IM",
     "F":"Free Relay",
     "G":"Medley Relay"
 }
 HY3_EVENT_GENDER_CODES = {
     "M":"Men",
     "F":"Women",
+    "W":"Women",
     "B":"Boys",
     "G":"Girls",
     "X":"Mixed"
 }
 HY3_EVENT_COURSE_CODES = {
     "S":"SCM",
     "Y":"SCY",
@@ -96,14 +97,16 @@
                     "preferredname":pfname}
                 cur_team['swimmers'].append(cur_swimmer)
             elif rtype == b'E1':
                 strokecode = record[21:22].decode('latin')
                 #print("stroke",HY3_STROKE_CODES[strokecode])
                 distance = int(record[15:21].decode('latin'))
                 event_gendercode = record[14:15].decode('latin')
+                if event_gendercode not in HY3_EVENT_GENDER_CODES:
+                    print("unknown gender code",event_gendercode)
                 #print("distance",repr(record[67:71]))
                 #print("event #",record[72:76])
                 event_num_str = record[38:42].decode('latin').strip()
                 try:
                     event_num = int(event_num_str,10)
                 except ValueError:
                     #print("couldn't convert event_num, leaving as string",event_num_str)
@@ -129,14 +132,16 @@
                 cur_entry = {
                     "event":event_num,
                     "event_str":event_num_str,
                     "event_gendercode":event_gendercode,
                     "event_gender":HY3_EVENT_GENDER_CODES[event_gendercode] if event_gendercode in HY3_EVENT_GENDER_CODES else "Unknown",
                     "event_course":None,
                     "event_coursecode":None,
+                    "event_type":"Final", # is this the correct default?
+                    "event_date":None,
                     "heat":None,
                     "heat_number":None,
                     "lane":None,
                     "stroke":HY3_STROKE_CODES[strokecode],
                     "strokeshort":HY3_STROKE_CODES_SHORT[strokecode],
                     "distance":distance,
                     "seed_time":seed_time,
@@ -151,15 +156,15 @@
 
             elif rtype == b'E2':
 
                 event_type = record[2:3].decode('latin').strip()
                 if event_type in HY3_EVENT_TYPE_CODES:
                     cur_entry['event_type'] = HY3_EVENT_TYPE_CODES[event_type]
                 else:
-                    cur_entry['event_type'] = None
+                    cur_entry['event_type'] = "Final" # Is this the correct default?
                 cur_entry['event_typecode'] = event_type
                 cur_entry['heat'] = record[20:23].decode('latin').strip()
                 cur_entry['heat_number'] = int(cur_entry['heat'],10)
                 cur_entry['lane'] = record[23:26].decode('latin').strip()
 
                 cur_entry['event_datestr'] = record[87:95].decode('latin').strip()
                 cur_entry['event_date'] = _mmddyyyy_date_to_iso_date(cur_entry['event_datestr'])
```

## Comparing `swimstroke-0.0.3.dist-info/LICENSE` & `swimstroke-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `swimstroke-0.0.3.dist-info/RECORD` & `swimstroke-0.0.4.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 swimstroke/__init__.py,sha256=HTxCVaw1TLgpHMH8guB3hHYQ80cX6_fSEoPT_hz2Y8w,23
-swimstroke/__main__.py,sha256=XtPUjZM3ZTd_fEMmgZBqFlkp65eqXXcVWTXmQR9PF_A,657
+swimstroke/__main__.py,sha256=kuYhv5b1p8hvGPsxbX95EroggUkDgQEjAgFXDa65Z-s,715
 swimstroke/ev3.py,sha256=P5IkzYCqAH3E5ZzhJMyFztxo0PE4_-wmwIyOsDkagws,3793
-swimstroke/helpers.py,sha256=HgdD5bPzPZXHRWQANyha_n0oloZFPpjZ4pccd_4ICDE,5945
-swimstroke/hy3.py,sha256=Exs_cjsISZqOGUBaowhOQrspL_lcGvcWbESQ6CI8ZZc,13053
+swimstroke/helpers.py,sha256=bfASARJrkJ2keypm2ql8aouFyi1axIxgGSGq0Bf_S4Y,6024
+swimstroke/hy3.py,sha256=bAL38mOpdn-mCJbNg0PCfpyqxu_XC7DrOTEb2R92Afk,13349
 swimstroke/scb.py,sha256=cC-rhzRvKpq60ux7MHm0ylj16qc21ZqhUBLQqxdJMQI,86
 swimstroke/sd3.py,sha256=JMYeTOk66YJInRReB3KMFyB1JKnX69sCHdC2_Ey2ypg,47
 swimstroke/util.py,sha256=s7cBEfHsdbYuID3bH2bAnw72zYHC2A4LroSf8iTH74o,586
 swimstroke/yaml.py,sha256=JMYeTOk66YJInRReB3KMFyB1JKnX69sCHdC2_Ey2ypg,47
-swimstroke-0.0.3.dist-info/LICENSE,sha256=ua_EyrQ3shMEJAhfgGjSeK_mFf6AIT-QiFG2lQfsntY,1103
-swimstroke-0.0.3.dist-info/METADATA,sha256=WgM6E9-UJM8e95NVtSxzEAA6LjkIwmA6-lYvbBXkHBk,77
-swimstroke-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-swimstroke-0.0.3.dist-info/top_level.txt,sha256=C15CTf7t6T4k83ycljKbwYVziBgz5vqOBEYdK8Y6FfY,11
-swimstroke-0.0.3.dist-info/RECORD,,
+swimstroke-0.0.4.dist-info/LICENSE,sha256=ua_EyrQ3shMEJAhfgGjSeK_mFf6AIT-QiFG2lQfsntY,1103
+swimstroke-0.0.4.dist-info/METADATA,sha256=kvNo4UesDqWBrgIwOrhbq2dhKu1iqSuIbtipgHaJO_g,77
+swimstroke-0.0.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+swimstroke-0.0.4.dist-info/top_level.txt,sha256=C15CTf7t6T4k83ycljKbwYVziBgz5vqOBEYdK8Y6FfY,11
+swimstroke-0.0.4.dist-info/RECORD,,
```

