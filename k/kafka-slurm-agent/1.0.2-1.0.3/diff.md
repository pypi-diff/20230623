# Comparing `tmp/kafka_slurm_agent-1.0.2-py3-none-any.whl.zip` & `tmp/kafka_slurm_agent-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 29875 bytes, number of entries: 18
+Zip file size: 29893 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx      164 b- defN 21-Nov-07 16:55 kafka_slurm_agent/__init__.py
 -rw-rw-r--  2.0 unx     4083 b- defN 23-Jan-18 12:51 kafka_slurm_agent/cluster_agent.py
 -rw-rw-r--  2.0 unx     4929 b- defN 22-Oct-13 22:44 kafka_slurm_agent/command.py
 -rw-rw-r--  2.0 unx    11318 b- defN 21-Nov-04 13:26 kafka_slurm_agent/config_module.py
--rw-rw-r--  2.0 unx    27335 b- defN 23-Apr-21 09:49 kafka_slurm_agent/kafka_modules.py
+-rw-rw-r--  2.0 unx    27388 b- defN 23-Jun-22 23:25 kafka_slurm_agent/kafka_modules.py
 -rw-rw-r--  2.0 unx     4686 b- defN 22-Oct-21 17:16 kafka_slurm_agent/monitor_agent.py
 -rw-rw-r--  2.0 unx     7406 b- defN 22-Oct-21 21:16 kafka_slurm_agent/runner.py
 -rw-rw-r--  2.0 unx     3463 b- defN 22-Oct-28 08:05 kafka_slurm_agent/worker_agent.py
--rwxrwxr-x  2.0 unx     2007 b- defN 22-Oct-21 21:14 kafka_slurm_agent-1.0.2.data/data/cluster_agent
--rw-rw-r--  2.0 unx     2083 b- defN 23-Apr-21 08:14 kafka_slurm_agent-1.0.2.data/data/kafkaslurm_cfg.py__
--rwxrwxr-x  2.0 unx     1991 b- defN 22-Oct-21 21:00 kafka_slurm_agent-1.0.2.data/data/monitor_agent
--rwxrwxr-x  2.0 unx     2011 b- defN 22-Oct-21 20:58 kafka_slurm_agent-1.0.2.data/data/worker_agent
--rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-21 09:50 kafka_slurm_agent-1.0.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2069 b- defN 23-Apr-21 09:50 kafka_slurm_agent-1.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       86 b- defN 23-Apr-21 09:50 kafka_slurm_agent-1.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       62 b- defN 23-Apr-21 09:50 kafka_slurm_agent-1.0.2.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       18 b- defN 23-Apr-21 09:50 kafka_slurm_agent-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1673 b- defN 23-Apr-21 09:50 kafka_slurm_agent-1.0.2.dist-info/RECORD
-18 files, 86741 bytes uncompressed, 27075 bytes compressed:  68.8%
+-rwxrwxr-x  2.0 unx     2007 b- defN 22-Oct-21 21:14 kafka_slurm_agent-1.0.3.data/data/cluster_agent
+-rw-rw-r--  2.0 unx     2083 b- defN 23-Apr-21 08:14 kafka_slurm_agent-1.0.3.data/data/kafkaslurm_cfg.py__
+-rwxrwxr-x  2.0 unx     1991 b- defN 22-Oct-21 21:00 kafka_slurm_agent-1.0.3.data/data/monitor_agent
+-rwxrwxr-x  2.0 unx     2011 b- defN 22-Oct-21 20:58 kafka_slurm_agent-1.0.3.data/data/worker_agent
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-22 23:27 kafka_slurm_agent-1.0.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2069 b- defN 23-Jun-22 23:27 kafka_slurm_agent-1.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       86 b- defN 23-Jun-22 23:27 kafka_slurm_agent-1.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       62 b- defN 23-Jun-22 23:27 kafka_slurm_agent-1.0.3.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       18 b- defN 23-Jun-22 23:27 kafka_slurm_agent-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1673 b- defN 23-Jun-22 23:27 kafka_slurm_agent-1.0.3.dist-info/RECORD
+18 files, 86794 bytes uncompressed, 27093 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -18,38 +18,38 @@
 
 Filename: kafka_slurm_agent/runner.py
 Comment: 
 
 Filename: kafka_slurm_agent/worker_agent.py
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.2.data/data/cluster_agent
+Filename: kafka_slurm_agent-1.0.3.data/data/cluster_agent
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.2.data/data/kafkaslurm_cfg.py__
+Filename: kafka_slurm_agent-1.0.3.data/data/kafkaslurm_cfg.py__
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.2.data/data/monitor_agent
+Filename: kafka_slurm_agent-1.0.3.data/data/monitor_agent
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.2.data/data/worker_agent
+Filename: kafka_slurm_agent-1.0.3.data/data/worker_agent
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.2.dist-info/LICENSE
+Filename: kafka_slurm_agent-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.2.dist-info/METADATA
+Filename: kafka_slurm_agent-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.2.dist-info/WHEEL
+Filename: kafka_slurm_agent-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.2.dist-info/entry_points.txt
+Filename: kafka_slurm_agent-1.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.2.dist-info/top_level.txt
+Filename: kafka_slurm_agent-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.2.dist-info/RECORD
+Filename: kafka_slurm_agent-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kafka_slurm_agent/kafka_modules.py

```diff
@@ -211,24 +211,24 @@
     def send(self, jobid, results, error):
         results['results']['error'] = str(error)
         results['results']['timestamp'] = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
         self.producer.send(config['TOPIC_ERROR'], key=jobid.encode('utf-8'), value=results)
 
 
 class JobSubmitter(KafkaSender):
-    def send(self, s_id, script='my_job.py', slurm_pars={'RESOURCES_REQUIRED': 1, 'JOB_TYPE': 'gpu'}, check=True, flush=True, ignore_error_status=False):
+    def send(self, s_id, script='my_job.py', slurm_pars={'RESOURCES_REQUIRED': 1, 'JOB_TYPE': 'cpu'}, check=True, flush=True, ignore_error_status=False, topic=config['TOPIC_NEW']):
         status = None
         if check:
             status = self.check_status(s_id)
             if status is not None:
                 if config['DEBUG']:
                     print('{} already processed: {}'.format(s_id, status))
                 if not ignore_error_status or (ignore_error_status and status != 'ERROR'):
                     return s_id, False, status
-        self.producer.send(config['TOPIC_NEW'], key=s_id.encode('utf-8'), value={'input_job_id': s_id, 'script': script,
+        self.producer.send(topic, key=s_id.encode('utf-8'), value={'input_job_id': s_id, 'script': script,
                                                                                  'slurm_pars': slurm_pars,
                                                                                  'timestamp': datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")})
         if flush:
             self.producer.flush()
         return s_id, True, status
 
     @staticmethod
@@ -241,18 +241,18 @@
             if status[s_id]:
                 return status[s_id]['status']
             else:
                 return None
         except URLError as e:
             raise ClusterAgentException('Cannot reach Monitor Agent at: ' + url)
 
-    def send_many(self, ids, script='my_job.py', slurm_pars={'RESOURCES_REQUIRED': 1, 'JOB_TYPE': 'gpu'}, check=True, ignore_error_status=False):
+    def send_many(self, ids, script='my_job.py', slurm_pars={'RESOURCES_REQUIRED': 1, 'JOB_TYPE': 'cpu'}, check=True, ignore_error_status=False, topic=config['TOPIC_NEW']):
         results = []
         for s_id in ids:
-            results.append(self.send(s_id, script=script, slurm_pars=slurm_pars, check=check, flush=False, ignore_error_status=ignore_error_status))
+            results.append(self.send(s_id, script=script, slurm_pars=slurm_pars, check=check, flush=False, ignore_error_status=ignore_error_status, topic=topic))
         self.producer.flush()
         return results
 
     def __del__(self):
         self.producer.flush()
```

## Comparing `kafka_slurm_agent-1.0.2.data/data/cluster_agent` & `kafka_slurm_agent-1.0.3.data/data/cluster_agent`

 * *Files identical despite different names*

## Comparing `kafka_slurm_agent-1.0.2.data/data/kafkaslurm_cfg.py__` & `kafka_slurm_agent-1.0.3.data/data/kafkaslurm_cfg.py__`

 * *Files identical despite different names*

## Comparing `kafka_slurm_agent-1.0.2.data/data/monitor_agent` & `kafka_slurm_agent-1.0.3.data/data/monitor_agent`

 * *Files identical despite different names*

## Comparing `kafka_slurm_agent-1.0.2.data/data/worker_agent` & `kafka_slurm_agent-1.0.3.data/data/worker_agent`

 * *Files identical despite different names*

## Comparing `kafka_slurm_agent-1.0.2.dist-info/LICENSE` & `kafka_slurm_agent-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kafka_slurm_agent-1.0.2.dist-info/METADATA` & `kafka_slurm_agent-1.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-slurm-agent
-Version: 1.0.2
+Version: 1.0.3
 Summary: The Kafka Slurm Agent is a tool for submitting computing tasks to the Slurm queues on multiple clusters. It uses Kafka to asynchronously communicate with an agent installed on the cluster.It contains a monitoring tool and a job submitter.
 Home-page: https://github.com/prubach/kafka-slurm-agent
 Author: Paweł Rubach
 Author-email: pawel.rubach@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `kafka_slurm_agent-1.0.2.dist-info/RECORD` & `kafka_slurm_agent-1.0.3.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 kafka_slurm_agent/__init__.py,sha256=Z443N5Cv9w8TrZFQ5WxjHvLpZBks7iokln6SLAsEk74,164
 kafka_slurm_agent/cluster_agent.py,sha256=bdnMxGvnJPzVfZAR9YH7u5XVc9vxV7B7ZikAMp7ULwI,4083
 kafka_slurm_agent/command.py,sha256=lAFVoo1V15SdpBuLBac8mmTmILxfHV9oGxXw0rcLZJw,4929
 kafka_slurm_agent/config_module.py,sha256=1JnZTmvrj08tdprZROST7RkYp2UlCRL3CdgRre-mYKs,11318
-kafka_slurm_agent/kafka_modules.py,sha256=_fSawcqYIoG8Dj7WftUQ4CFuhwSDJtlOl70Kz4S67PQ,27335
+kafka_slurm_agent/kafka_modules.py,sha256=62WPR5FyYWfzN9dmNwpQef_TLc9bpoD4c_bn2RcNlC8,27388
 kafka_slurm_agent/monitor_agent.py,sha256=UVAQqAJT8Cpzx1-V-mzXkTJ0vULOhzTL-7wIiKKAlPM,4686
 kafka_slurm_agent/runner.py,sha256=3xKS_DUtbFXdmFC17qwXKpuqWzeW6GRFTA_H9tgOWe8,7406
 kafka_slurm_agent/worker_agent.py,sha256=qS4ymnvnfdLozzj88Wf3CV1IaAfmdulWGFZXJmrnEic,3463
-kafka_slurm_agent-1.0.2.data/data/cluster_agent,sha256=1tsn3OhOaReuH42EkkotbpO2TRjfiemKazr5g-c_JAE,2007
-kafka_slurm_agent-1.0.2.data/data/kafkaslurm_cfg.py__,sha256=YSLNEz9u_jP7xkJt4A0IebdfSs7YFg3DbqwEFHy1dis,2083
-kafka_slurm_agent-1.0.2.data/data/monitor_agent,sha256=nzf6GYqA45xaPkOSrMKLhZXLmqvrEPJ-lcgI_PRp1VQ,1991
-kafka_slurm_agent-1.0.2.data/data/worker_agent,sha256=s6mcqKJLJlSxclFzWv6FbnBRHQtYaNCOWotLaKQTG7o,2011
-kafka_slurm_agent-1.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-kafka_slurm_agent-1.0.2.dist-info/METADATA,sha256=9nCbQZcVfhY3ESVNHXzYH1EVFmB7afIfVAxVeBzEkpg,2069
-kafka_slurm_agent-1.0.2.dist-info/WHEEL,sha256=yYV-D90-NW-UlZINH_90hGjz3BXXubiZbvu2N2r2uFU,86
-kafka_slurm_agent-1.0.2.dist-info/entry_points.txt,sha256=pZiTuEXiq16U2FWuWE49x2_2xLoxtgGlzB9Mc389kmg,62
-kafka_slurm_agent-1.0.2.dist-info/top_level.txt,sha256=ot5Idwc6vKowyJdvWhOZepKDqtzCTFN52Oe7iIrtfVQ,18
-kafka_slurm_agent-1.0.2.dist-info/RECORD,,
+kafka_slurm_agent-1.0.3.data/data/cluster_agent,sha256=1tsn3OhOaReuH42EkkotbpO2TRjfiemKazr5g-c_JAE,2007
+kafka_slurm_agent-1.0.3.data/data/kafkaslurm_cfg.py__,sha256=YSLNEz9u_jP7xkJt4A0IebdfSs7YFg3DbqwEFHy1dis,2083
+kafka_slurm_agent-1.0.3.data/data/monitor_agent,sha256=nzf6GYqA45xaPkOSrMKLhZXLmqvrEPJ-lcgI_PRp1VQ,1991
+kafka_slurm_agent-1.0.3.data/data/worker_agent,sha256=s6mcqKJLJlSxclFzWv6FbnBRHQtYaNCOWotLaKQTG7o,2011
+kafka_slurm_agent-1.0.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+kafka_slurm_agent-1.0.3.dist-info/METADATA,sha256=IOxt-PokFmq17W9HBcUfS5pInlCqJWyy1sa9PHkqb20,2069
+kafka_slurm_agent-1.0.3.dist-info/WHEEL,sha256=DueAsW6E8XIw2snDYANiEbP441s0xNQrJIWO3pKUKFM,86
+kafka_slurm_agent-1.0.3.dist-info/entry_points.txt,sha256=pZiTuEXiq16U2FWuWE49x2_2xLoxtgGlzB9Mc389kmg,62
+kafka_slurm_agent-1.0.3.dist-info/top_level.txt,sha256=ot5Idwc6vKowyJdvWhOZepKDqtzCTFN52Oe7iIrtfVQ,18
+kafka_slurm_agent-1.0.3.dist-info/RECORD,,
```

