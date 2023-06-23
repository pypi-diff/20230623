# Comparing `tmp/pyperf2-0.2-py3-none-any.whl.zip` & `tmp/pyperf2-0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 10883 bytes, number of entries: 6
--rw-r--r--  2.0 unx    22986 b- defN 23-Feb-05 08:31 pyperf2/__init__.py
--rwxr-xr-x  2.0 unx    11357 b- defN 23-Feb-05 08:32 pyperf2-0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3295 b- defN 23-Feb-05 08:32 pyperf2-0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-05 08:32 pyperf2-0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Feb-05 08:32 pyperf2-0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      453 b- defN 23-Feb-05 08:32 pyperf2-0.2.dist-info/RECORD
-6 files, 38191 bytes uncompressed, 10069 bytes compressed:  73.6%
+Zip file size: 11145 bytes, number of entries: 6
+-rw-r--r--  2.0 unx    24262 b- defN 23-Jun-23 09:06 pyperf2/__init__.py
+-rwxr-xr-x  2.0 unx    11357 b- defN 23-Jun-23 09:07 pyperf2-0.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3314 b- defN 23-Jun-23 09:07 pyperf2-0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-23 09:07 pyperf2-0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-23 09:07 pyperf2-0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      453 b- defN 23-Jun-23 09:07 pyperf2-0.3.dist-info/RECORD
+6 files, 39486 bytes uncompressed, 10331 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: pyperf2/__init__.py
 Comment: 
 
-Filename: pyperf2-0.2.dist-info/LICENSE
+Filename: pyperf2-0.3.dist-info/LICENSE
 Comment: 
 
-Filename: pyperf2-0.2.dist-info/METADATA
+Filename: pyperf2-0.3.dist-info/METADATA
 Comment: 
 
-Filename: pyperf2-0.2.dist-info/WHEEL
+Filename: pyperf2-0.3.dist-info/WHEEL
 Comment: 
 
-Filename: pyperf2-0.2.dist-info/top_level.txt
+Filename: pyperf2-0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pyperf2-0.2.dist-info/RECORD
+Filename: pyperf2-0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyperf2/__init__.py

```diff
@@ -36,14 +36,15 @@
         self.name = None
         self._running = False
         self.realtime = True
         self.bandwidth = "1000pps"
         self.port = "5001"
         self.status = "configured"
         self.packet_len = "1470"
+        self.dscp = None
         self._result_regex = None
         self._info_regex = None
         self._results = {}
         self.test_duration = "86400"
         self.client_source_port = None
         self.use_linux_namespace = None
         self._on_data_callbacks = []
@@ -171,15 +172,17 @@
                             ]
                         )
                         packets_received = self.expected_interval_packets - packets_lost
                         report_message["packets_lost"] = packets_lost
                         report_message["packets_received"] = packets_received
                         # print('{0} {1}'.format(packets_lost,packets_received))
 
-                    except IndexError:  # loss without event registred, can only be at interval_begin 0.0 -> ignore
+                    except (
+                        IndexError
+                    ):  # loss without event registred, can only be at interval_begin 0.0 -> ignore
                         # print('----------------------index error------------------------')
                         if interval_begin == 0:
                             report_message["packets_lost"] = 0
                             report_message[
                                 "packets_received"
                             ] = self.expected_interval_packets
                         else:
@@ -346,15 +349,14 @@
             if not event_begin:
                 event_begin = Decimal(result["interval_begin"])
             try:
                 if (
                     result["interval_end"]
                     != results_with_packet_loss[idx + 1]["interval_begin"]
                 ):
-
                     events.append(
                         {
                             "detail": event_data,
                             "summary": {
                                 "total_loss": event_loss,
                                 "begin": str(event_begin),
                                 "end": str(Decimal(result["interval_end"])),
@@ -475,14 +477,59 @@
 
         _cli.append("-b")
         _cli.append(self.bandwidth)
 
         _cli.append("-p")
         _cli.append(self.port)
 
+        if self.dscp:
+            accepted_tos_values = [
+                "af11",
+                "af12",
+                "af13",
+                "af21",
+                "af22",
+                "af23",
+                "af31",
+                "af32",
+                "af33",
+                "af41",
+                "af42",
+                "af43",
+                "cs0",
+                "cs1",
+                "cs2",
+                "cs3",
+                "cs4",
+                "cs5",
+                "cs6",
+                "cs7",
+                "ef",
+                "le",
+                "nqb",
+                "nqb2",
+                "ac_be",
+                "ac_bk",
+                "ac_vi",
+                "ac_vo",
+                "lowdelay",
+                "throughput",
+            ]
+            self.dscp = self.dscp.lower()
+            if str(self.dscp) in accepted_tos_values or (
+                int(self.dscp) > 0 and int(self.dscp) <= 255
+            ):
+                _cli.append("-S")
+                _cli.append(self.dscp)
+            else:
+                raise ValueError(f'"{self.dscp}" is not a valid DSCP Value')
+
+            _cli.append("-S")
+            _cli.append(self.dscp)
+
         return _cli
 
     def start(self, create_thread_function=threading.Thread):
         self._results = {}
         if self._cleanup_timer_thread:
             self._cleanup_timer_thread.join()
             del self._cleanup_timer_thread
```

## Comparing `pyperf2-0.2.dist-info/LICENSE` & `pyperf2-0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyperf2-0.2.dist-info/METADATA` & `pyperf2-0.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: pyperf2
-Version: 0.2
+Version: 0.3
 Summary: Abstraction layer for iperf2 linux binary
 Home-page: https://github.com/jinjamator/pyperf2
 Author: Wilhelm Putz
 Author-email: wp@aci.guru
 License: ASL V2
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: System :: Installation/Setup
 Classifier: Topic :: System :: Systems Administration
 Classifier: Topic :: Utilities
 Requires-Python: >=3.7
@@ -105,7 +106,8 @@
 
 For documentation please refer to https://pyperf2.readthedocs.io/en/latest/
 
 License
 -----------------
 
 This project is licensed under the Apache License Version 2.0
+
```

