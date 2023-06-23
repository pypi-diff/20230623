# Comparing `tmp/kafka_slurm_agent-1.0.3-py3-none-any.whl.zip` & `tmp/kafka_slurm_agent-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 29893 bytes, number of entries: 18
+Zip file size: 29992 bytes, number of entries: 18
 -rw-rw-r--  2.0 unx      164 b- defN 21-Nov-07 16:55 kafka_slurm_agent/__init__.py
--rw-rw-r--  2.0 unx     4083 b- defN 23-Jan-18 12:51 kafka_slurm_agent/cluster_agent.py
+-rw-rw-r--  2.0 unx     4150 b- defN 23-Jun-23 11:54 kafka_slurm_agent/cluster_agent.py
 -rw-rw-r--  2.0 unx     4929 b- defN 22-Oct-13 22:44 kafka_slurm_agent/command.py
 -rw-rw-r--  2.0 unx    11318 b- defN 21-Nov-04 13:26 kafka_slurm_agent/config_module.py
--rw-rw-r--  2.0 unx    27388 b- defN 23-Jun-22 23:25 kafka_slurm_agent/kafka_modules.py
+-rw-rw-r--  2.0 unx    27493 b- defN 23-Jun-23 11:54 kafka_slurm_agent/kafka_modules.py
 -rw-rw-r--  2.0 unx     4686 b- defN 22-Oct-21 17:16 kafka_slurm_agent/monitor_agent.py
--rw-rw-r--  2.0 unx     7406 b- defN 22-Oct-21 21:16 kafka_slurm_agent/runner.py
+-rw-rw-r--  2.0 unx     7422 b- defN 23-Jun-23 11:54 kafka_slurm_agent/runner.py
 -rw-rw-r--  2.0 unx     3463 b- defN 22-Oct-28 08:05 kafka_slurm_agent/worker_agent.py
--rwxrwxr-x  2.0 unx     2007 b- defN 22-Oct-21 21:14 kafka_slurm_agent-1.0.3.data/data/cluster_agent
--rw-rw-r--  2.0 unx     2083 b- defN 23-Apr-21 08:14 kafka_slurm_agent-1.0.3.data/data/kafkaslurm_cfg.py__
--rwxrwxr-x  2.0 unx     1991 b- defN 22-Oct-21 21:00 kafka_slurm_agent-1.0.3.data/data/monitor_agent
--rwxrwxr-x  2.0 unx     2011 b- defN 22-Oct-21 20:58 kafka_slurm_agent-1.0.3.data/data/worker_agent
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-22 23:27 kafka_slurm_agent-1.0.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2069 b- defN 23-Jun-22 23:27 kafka_slurm_agent-1.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       86 b- defN 23-Jun-22 23:27 kafka_slurm_agent-1.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       62 b- defN 23-Jun-22 23:27 kafka_slurm_agent-1.0.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       18 b- defN 23-Jun-22 23:27 kafka_slurm_agent-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1673 b- defN 23-Jun-22 23:27 kafka_slurm_agent-1.0.3.dist-info/RECORD
-18 files, 86794 bytes uncompressed, 27093 bytes compressed:  68.8%
+-rwxrwxr-x  2.0 unx     2007 b- defN 22-Oct-21 21:14 kafka_slurm_agent-1.1.0.data/data/cluster_agent
+-rw-rw-r--  2.0 unx     2116 b- defN 23-Jun-23 11:54 kafka_slurm_agent-1.1.0.data/data/kafkaslurm_cfg.py__
+-rwxrwxr-x  2.0 unx     1991 b- defN 22-Oct-21 21:00 kafka_slurm_agent-1.1.0.data/data/monitor_agent
+-rwxrwxr-x  2.0 unx     2011 b- defN 22-Oct-21 20:58 kafka_slurm_agent-1.1.0.data/data/worker_agent
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-23 11:55 kafka_slurm_agent-1.1.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2069 b- defN 23-Jun-23 11:55 kafka_slurm_agent-1.1.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       86 b- defN 23-Jun-23 11:55 kafka_slurm_agent-1.1.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       62 b- defN 23-Jun-23 11:55 kafka_slurm_agent-1.1.0.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       18 b- defN 23-Jun-23 11:55 kafka_slurm_agent-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1673 b- defN 23-Jun-23 11:55 kafka_slurm_agent-1.1.0.dist-info/RECORD
+18 files, 87015 bytes uncompressed, 27192 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -18,38 +18,38 @@
 
 Filename: kafka_slurm_agent/runner.py
 Comment: 
 
 Filename: kafka_slurm_agent/worker_agent.py
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.3.data/data/cluster_agent
+Filename: kafka_slurm_agent-1.1.0.data/data/cluster_agent
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.3.data/data/kafkaslurm_cfg.py__
+Filename: kafka_slurm_agent-1.1.0.data/data/kafkaslurm_cfg.py__
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.3.data/data/monitor_agent
+Filename: kafka_slurm_agent-1.1.0.data/data/monitor_agent
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.3.data/data/worker_agent
+Filename: kafka_slurm_agent-1.1.0.data/data/worker_agent
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.3.dist-info/LICENSE
+Filename: kafka_slurm_agent-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.3.dist-info/METADATA
+Filename: kafka_slurm_agent-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.3.dist-info/WHEEL
+Filename: kafka_slurm_agent-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.3.dist-info/entry_points.txt
+Filename: kafka_slurm_agent-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.3.dist-info/top_level.txt
+Filename: kafka_slurm_agent-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: kafka_slurm_agent-1.0.3.dist-info/RECORD
+Filename: kafka_slurm_agent-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## kafka_slurm_agent/cluster_agent.py

```diff
@@ -1,14 +1,14 @@
 import ast
 import os
 
 import faust
 import sys
 from pydoc import locate
-from kafka_slurm_agent.kafka_modules import config, HeartbeatSender
+from kafka_slurm_agent.kafka_modules import config, HeartbeatSender, ClusterAgent
 from concurrent.futures import ThreadPoolExecutor
 
 app = faust.App(config['CLUSTER_NAME'] + '_cluster_agent',
                 group_id=1,
                 broker='kafka://' + config['BOOTSTRAP_SERVERS'],
                 broker_credentials=config['KAFKA_FAUST_BROKER_CREDENTIALS'],
                 processing_guarantee='exactly_once',
@@ -17,15 +17,15 @@
                 topic_partitions=1)
 #store='rocksdb://',
 jobs_topic = app.topic(config['TOPIC_STATUS'], partitions=1)
 job_status = app.Table('job_status', default='')
 
 thread_pool = ThreadPoolExecutor(max_workers=1)
 sys.path.append(os.getcwd())
-ca_class = locate(config['CLUSTER_AGENT_CLASS'])
+ca_class = locate(config['CLUSTER_AGENT_CLASS']) if 'CLUSTER_AGENT_CLASS' in config else ClusterAgent
 ca = ca_class()
 heartbeat_sender = HeartbeatSender()
 
 
 def run_cluster_agent_check():
     run_timeout = None
     if 'CLUSTER_JOB_TIMEOUT' in config and config['CLUSTER_JOB_TIMEOUT']:
```

## kafka_slurm_agent/kafka_modules.py

```diff
@@ -28,14 +28,15 @@
 from kafka_slurm_agent.command import Command
 from kafka_slurm_agent.config_module import Config
 
 CONFIG_FILE = 'kafkaslurm_cfg.py'
 
 config_defaults = {
     'CLUSTER_NAME': 'my_cluster',
+    'CLUSTER_JOB_NAME_SUFFIX': '_KSA',
     'POLL_INTERVAL': 30.0,
     'BOOTSTRAP_SERVERS': 'localhost:9092',
     'MONITOR_AGENT_URL': 'http://localhost:6066/',
     'WORKER_AGENT_URL': 'http://localhost:6068/',
     'MONITOR_AGENT_CONTEXT_PATH': '',
     'WORKER_AGENT_CONTEXT_PATH': '',
     'KAFKA_FAUST_BROKER_CREDENTIALS': None,
@@ -45,15 +46,15 @@
     'KAFKA_PASSWORD': None,
     'WORKER_AGENT_MAX_WORKERS': 2,
     'WORKER_JOB_TIMEOUT': 86400,  # = 24h
     'HEARTBEAT_INTERVAL': 0.0,
     'KAFKA_CONSUMER_HEARTBEAT_INTERVAL_MS': 2000,
     'MONITOR_HEARTBEAT_INTERVAL_MS': 3000,
     'MONITOR_ONLY_DO_NOT_SUBMIT': False,
-    'KAFKA_PARTITION_ASSIGNMENT_STRATEGY': [RoundRobinPartitionAssignor, RangePartitionAssignor]
+    'KAFKA_PARTITION_ASSIGNMENT_STRATEGY': [RoundRobinPartitionAssignor, RangePartitionAssignor],
 }
 
 
 class ConfigLoader:
     def __init__(self):
         self.config = None
 
@@ -434,14 +435,15 @@
             worker.start()
         self.queue.join()
 
 
 class ClusterAgent(WorkingAgent):
     def __init__(self):
         super(ClusterAgent, self).__init__()
+        self.job_name_suffix = config['CLUSTER_JOB_NAME_SUFFIX']
         self.logger = setupLogger(config['LOGS_DIR'], "clusteragent")
         self.logger.info('Cluster Agent Started')
 
     def check_queue_submit(self):
         func_name = 'self.slurm_get_idle_' + self.get_job_type(None) + 's'
         free = eval(func_name + "()")
         self.logger.info('Free {}s: {}'.format(config['SLURM_JOB_TYPE'].upper(), free))
```

## kafka_slurm_agent/runner.py

```diff
@@ -15,22 +15,22 @@
     'start_cluster_agent': '#!/bin/bash\nfaust -A kafka_slurm_agent.cluster_agent -l info worker\n',
     'my_monitor_agent.py': "from kafka_slurm_agent.monitor_agent import app, job_status, done_topic\n\n"
                         "#TODO Put your monitor agent code here\n\n\n"
                         "@app.agent(done_topic)\n"
                         "async def process_done(stream):\n"
                         "\tasync for msg in stream.events():\n"
                         "\t\tprint('Got {}: {}'.format(msg.key, msg.value))\n",
-    'my_cluster_agent.py': "from kafka_slurm_agent.kafka_modules import ClusterAgent\n\n"
-                           "class MyClusterAgent(ClusterAgent):\n"
-                           "\tdef __init__(self):\n"
-                           "\t\tsuper().__init__()\n"
-                           "\t\tself.script_name = 'run.py'\n"
-                           "\t\tself.job_name_suffix = '_MYJOBS'\n\n"
-                           "\tdef get_job_name(self, input_job_id):\n"
-                           "\t\treturn str(input_job_id) + self.job_name_suffix\n",
+    # 'my_cluster_agent.py': "from kafka_slurm_agent.kafka_modules import ClusterAgent\n\n"
+    #                        "class MyClusterAgent(ClusterAgent):\n"
+    #                        "\tdef __init__(self):\n"
+    #                        "\t\tsuper().__init__()\n"
+    #                        "\t\tself.script_name = 'run.py'\n"
+    #                        "\t\tself.job_name_suffix = '_MYJOBS'\n\n"
+    #                        "\tdef get_job_name(self, input_job_id):\n"
+    #                        "\t\treturn str(input_job_id) + self.job_name_suffix\n",
     'my_worker_agent.py': "from kafka_slurm_agent.kafka_modules import WorkerAgent\n\n"
                            "class MyWorkerAgent(WorkerAgent):\n"
                            "\tdef __init__(self):\n"
                            "\t\tsuper().__init__()\n"
                            "\t\tself.script_name = 'run.py'\n"
                            "\t\tself.job_name_suffix = '_MYJOBS'\n\n"
                            "\tdef get_job_name(self, input_job_id):\n"
```

## Comparing `kafka_slurm_agent-1.0.3.data/data/cluster_agent` & `kafka_slurm_agent-1.1.0.data/data/cluster_agent`

 * *Files identical despite different names*

## Comparing `kafka_slurm_agent-1.0.3.data/data/kafkaslurm_cfg.py__` & `kafka_slurm_agent-1.1.0.data/data/kafkaslurm_cfg.py__`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 #from kafka.coordinator.assignors.roundrobin import RoundRobinPartitionAssignor
 
 
 #PREFIX = join(expanduser("~"), 'my_kafka_slurm')
 #SHARED_TMP = PREFIX + '/tmp'
 DEBUG = True
 CLUSTER_NAME = 'my_cluster'
-CLUSTER_AGENT_CLASS = 'my_cluster_agent.MyClusterAgent'
+# CLUSTER_AGENT_CLASS = 'my_cluster_agent.MyClusterAgent'
 BOOTSTRAP_SERVERS = 'localhost:9092'
 KAFKA_SECURITY_PROTOCOL = 'PLAINTEXT'
 # KAFKA_SECURITY_PROTOCOL = 'SASL_PLAINTEXT'
 # KAFKA_SASL_MECHANISM = 'PLAIN'
 # KAFKA_USERNAME = 'user'
 # KAFKA_PASSWORD = 'pass'
 # KAFKA_FAUST_BROKER_CREDENTIALS = faust.SASLCredentials(username=KAFKA_USERNAME, password=KAFKA_PASSWORD)
 
 #KAFKA_PARTITION_ASSIGNMENT_STRATEGY = [RoundRobinPartitionAssignor, RangePartitionAssignor]
+CLUSTER_JOB_NAME_SUFFIX='_KSA'
 TOPIC_NEW = 'kp-new'
 TOPIC_STATUS = 'kp-jobs'
 TOPIC_DONE = 'kp-done'
 TOPIC_ERROR = 'kp-error'
 TOPIC_HEARTBEAT = 'kp-heartbeat'
 CLUSTER_AGENT_NEW_GROUP = 'kp_agent_new'
 MONITOR_AGENT_NEW_GROUP = socket.gethostname() + '_monitor_agent_new'
```

## Comparing `kafka_slurm_agent-1.0.3.data/data/monitor_agent` & `kafka_slurm_agent-1.1.0.data/data/monitor_agent`

 * *Files identical despite different names*

## Comparing `kafka_slurm_agent-1.0.3.data/data/worker_agent` & `kafka_slurm_agent-1.1.0.data/data/worker_agent`

 * *Files identical despite different names*

## Comparing `kafka_slurm_agent-1.0.3.dist-info/LICENSE` & `kafka_slurm_agent-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `kafka_slurm_agent-1.0.3.dist-info/METADATA` & `kafka_slurm_agent-1.1.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-slurm-agent
-Version: 1.0.3
+Version: 1.1.0
 Summary: The Kafka Slurm Agent is a tool for submitting computing tasks to the Slurm queues on multiple clusters. It uses Kafka to asynchronously communicate with an agent installed on the cluster.It contains a monitoring tool and a job submitter.
 Home-page: https://github.com/prubach/kafka-slurm-agent
 Author: Paweł Rubach
 Author-email: pawel.rubach@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `kafka_slurm_agent-1.0.3.dist-info/RECORD` & `kafka_slurm_agent-1.1.0.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 kafka_slurm_agent/__init__.py,sha256=Z443N5Cv9w8TrZFQ5WxjHvLpZBks7iokln6SLAsEk74,164
-kafka_slurm_agent/cluster_agent.py,sha256=bdnMxGvnJPzVfZAR9YH7u5XVc9vxV7B7ZikAMp7ULwI,4083
+kafka_slurm_agent/cluster_agent.py,sha256=EvRVobm7Rz2e42bxP8To366Y3jsTXSAkXNQNeeXLTB8,4150
 kafka_slurm_agent/command.py,sha256=lAFVoo1V15SdpBuLBac8mmTmILxfHV9oGxXw0rcLZJw,4929
 kafka_slurm_agent/config_module.py,sha256=1JnZTmvrj08tdprZROST7RkYp2UlCRL3CdgRre-mYKs,11318
-kafka_slurm_agent/kafka_modules.py,sha256=62WPR5FyYWfzN9dmNwpQef_TLc9bpoD4c_bn2RcNlC8,27388
+kafka_slurm_agent/kafka_modules.py,sha256=JiZBGocyiKIZJBKjqjayEjdjal4PoE0rFNGAmuzSFZY,27493
 kafka_slurm_agent/monitor_agent.py,sha256=UVAQqAJT8Cpzx1-V-mzXkTJ0vULOhzTL-7wIiKKAlPM,4686
-kafka_slurm_agent/runner.py,sha256=3xKS_DUtbFXdmFC17qwXKpuqWzeW6GRFTA_H9tgOWe8,7406
+kafka_slurm_agent/runner.py,sha256=SiSj6ihLhN3nb5lpYlN96sjYeR7zqi9bsp0ENzPX9E0,7422
 kafka_slurm_agent/worker_agent.py,sha256=qS4ymnvnfdLozzj88Wf3CV1IaAfmdulWGFZXJmrnEic,3463
-kafka_slurm_agent-1.0.3.data/data/cluster_agent,sha256=1tsn3OhOaReuH42EkkotbpO2TRjfiemKazr5g-c_JAE,2007
-kafka_slurm_agent-1.0.3.data/data/kafkaslurm_cfg.py__,sha256=YSLNEz9u_jP7xkJt4A0IebdfSs7YFg3DbqwEFHy1dis,2083
-kafka_slurm_agent-1.0.3.data/data/monitor_agent,sha256=nzf6GYqA45xaPkOSrMKLhZXLmqvrEPJ-lcgI_PRp1VQ,1991
-kafka_slurm_agent-1.0.3.data/data/worker_agent,sha256=s6mcqKJLJlSxclFzWv6FbnBRHQtYaNCOWotLaKQTG7o,2011
-kafka_slurm_agent-1.0.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-kafka_slurm_agent-1.0.3.dist-info/METADATA,sha256=IOxt-PokFmq17W9HBcUfS5pInlCqJWyy1sa9PHkqb20,2069
-kafka_slurm_agent-1.0.3.dist-info/WHEEL,sha256=DueAsW6E8XIw2snDYANiEbP441s0xNQrJIWO3pKUKFM,86
-kafka_slurm_agent-1.0.3.dist-info/entry_points.txt,sha256=pZiTuEXiq16U2FWuWE49x2_2xLoxtgGlzB9Mc389kmg,62
-kafka_slurm_agent-1.0.3.dist-info/top_level.txt,sha256=ot5Idwc6vKowyJdvWhOZepKDqtzCTFN52Oe7iIrtfVQ,18
-kafka_slurm_agent-1.0.3.dist-info/RECORD,,
+kafka_slurm_agent-1.1.0.data/data/cluster_agent,sha256=1tsn3OhOaReuH42EkkotbpO2TRjfiemKazr5g-c_JAE,2007
+kafka_slurm_agent-1.1.0.data/data/kafkaslurm_cfg.py__,sha256=KDpMNZ2hO86l78YaH3w-yeSuqjlv9llUErAawM4GqdM,2116
+kafka_slurm_agent-1.1.0.data/data/monitor_agent,sha256=nzf6GYqA45xaPkOSrMKLhZXLmqvrEPJ-lcgI_PRp1VQ,1991
+kafka_slurm_agent-1.1.0.data/data/worker_agent,sha256=s6mcqKJLJlSxclFzWv6FbnBRHQtYaNCOWotLaKQTG7o,2011
+kafka_slurm_agent-1.1.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+kafka_slurm_agent-1.1.0.dist-info/METADATA,sha256=YurssyeDMl43ndj7MtGysmaSxHhvmwWlKo611pgkSts,2069
+kafka_slurm_agent-1.1.0.dist-info/WHEEL,sha256=DueAsW6E8XIw2snDYANiEbP441s0xNQrJIWO3pKUKFM,86
+kafka_slurm_agent-1.1.0.dist-info/entry_points.txt,sha256=pZiTuEXiq16U2FWuWE49x2_2xLoxtgGlzB9Mc389kmg,62
+kafka_slurm_agent-1.1.0.dist-info/top_level.txt,sha256=ot5Idwc6vKowyJdvWhOZepKDqtzCTFN52Oe7iIrtfVQ,18
+kafka_slurm_agent-1.1.0.dist-info/RECORD,,
```

